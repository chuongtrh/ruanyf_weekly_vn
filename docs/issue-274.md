# Bản tin chia sẻ công nghệ (Số 274): Mảnh ghép cuối cùng của truyền thông mã hóa

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3529) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101507.webp)

Bức ảnh chụp công trình Nhà hát Khoa học Viễn tưởng Thành Đô vừa được khánh thành gần đây. Tòa nhà tọa lạc bên bờ hồ Tinh Dung, quận Phi Đô, thành phố Thành Đô, được thiết kế chuyên dụng để tổ chức các sự kiện triển lãm, hội nghị lớn. Vào ngày 18 tháng 10 vừa qua, Hội nghị Khoa học Viễn tưởng Thế giới lần thứ 81 và lễ trao giải Hugo danh giá đã chính thức khai mạc tại đây. (Nguồn: [IT Home](https://www.ithome.com/0/724/950.htm))

## 加密通信的最后一块拼图

Vào kỳ nghỉ tháng 10 vừa qua, Cloudflare – nhà cung cấp dịch vụ phân phối nội dung (CDN) lớn nhất thế giới – đã đăng tải [một bài viết trên blog kỹ thuật](https://blog.cloudflare.com/announcing-encrypted-client-hello/) công bố việc triển khai một giải pháp công nghệ mới mà họ gọi là “mảnh ghép cuối cùng của truyền thông mã hóa”.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101508.webp)

Đây là một bước tiến công nghệ rất quan trọng và có tầm ảnh hưởng lớn đến thế giới Internet, vì vậy trong số bản tin tuần này tôi muốn phân tích chi tiết về chủ đề này cùng bạn đọc.

Trước hết, chúng ta hãy cùng thảo luận: Giao thức kết nối bảo mật HTTPS có thực sự là một kênh truyền thông được mã hóa hoàn toàn?

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101601.webp)

Về cơ bản, câu trả lời là có. Bởi vì toàn bộ nội dung dữ liệu trao đổi qua lại giữa máy tính của bạn và máy chủ web đều đã được mã hóa an toàn, các bên trung gian hoàn toàn không thể nghe lén hay thay đổi nội dung đó.

Tuy nhiên, nếu xét một cách triệt để, HTTPS vẫn chưa phải là kênh mã hóa hoàn hảo 100%. **Vẫn còn một thông tin cực kỳ quan trọng được gửi đi dưới dạng văn bản thô (không mã hóa), đó chính là tên miền (Domain Name) của trang web bạn đang truy cập.** Do đó, các nhà cung cấp dịch vụ mạng (ISP) hay các bộ định tuyến trung gian vẫn có thể dễ dàng biết được bạn đang truy cập vào trang web nào.

Tại sao tên miền lại không được mã hóa trong kết nối HTTPS thông thường?

Nguyên nhân do khóa giải mã bảo mật được lưu giữ trên máy chủ web. Một máy chủ vật lý thường lưu trữ nhiều website khác nhau với các chứng chỉ bảo mật riêng biệt. Máy chủ bắt buộc phải biết chính xác người dùng đang muốn truy cập vào tên miền nào thì mới gửi đúng chứng chỉ bảo mật và khóa mã hóa tương ứng về cho máy khách. Do đó, việc gửi thông tin tên miền lên máy chủ phải diễn ra trước khi thiết lập kênh kết nối mã hóa.

Công nghệ mới của Cloudflare được thiết kế ra chính là để giải quyết lỗ hổng bảo mật này, công nghệ này có tên gọi là **ECH (Encrypted Client Hello)**.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101704.webp)

Cơ chế vận hành của ECH vô cùng thông minh. Nó áp dụng cấu trúc bọc dữ liệu hai lớp (Double-layer format) cho tên miền:
* Lớp vỏ ngoài (Outer) được gửi dưới dạng văn bản thô công khai, hiển thị tên miền dùng chung mặc định là `cloudflare-ech.com`.
* Lớp lõi trong (Inner) chứa thông tin tên miền thực tế mà người dùng muốn truy cập và toàn bộ lớp lõi này đã được mã hóa bảo mật.

Bằng phương pháp này, **các thiết bị mạng trung gian chỉ nhìn thấy máy tính của bạn đang thực hiện kết nối tới tên miền dùng chung `cloudflare-ech.com`, hoàn toàn không thể biết được bạn đang thực sự truy cập vào website cụ thể nào ở lớp lõi bên trong**, giúp bảo đảm quyền riêng tư tuyệt đối cho người dùng.

Đó là tóm tắt về mặt kỹ thuật, còn dưới đây là góc nhìn cá nhân của tôi về công nghệ này. Khi tìm hiểu sâu về cơ chế vận hành của ECH, tôi lập tức đặt ra một nghi vấn lớn về tính ổn định của hệ thống:

Nếu tên miền dùng chung `cloudflare-ech.com` gặp sự cố kỹ thuật hoặc bị chặn truy cập vì lý do nào đó, liệu toàn bộ các trang web đang sử dụng dịch vụ của Cloudflare trên toàn thế giới có bị rơi vào tình trạng mất kết nối hoàn toàn hay không?

Đây là một rủi ro rất thực tế, bởi vì Cloudflare hiện đang quản lý hạ tầng cho một tỷ lệ rất lớn các trang web trên Internet. Hơn nữa, hãng đã tự động kích hoạt tính năng ECH này cho toàn bộ các tài khoản sử dụng dịch vụ miễn phí mà không cung cấp tùy chọn tắt đi (tính năng tắt ECH chỉ dành cho các tài khoản trả phí doanh nghiệp). Điều này vô tình biến lượng lớn người dùng miễn phí thành đối tượng thử nghiệm cho công nghệ mới.

Do đó, tôi viết bài phân tích này nhằm đưa ra cảnh báo sớm cho bạn đọc. **Trong trường hợp xảy ra sự cố kết nối do công nghệ ECH khiến trang web của bạn không thể truy cập được, chúng ta sẽ có hai giải pháp xử lý:**

* **Đối với chủ sở hữu website**: Bạn có thể cân nhắc nâng cấp tài khoản Cloudflare lên gói trả phí để có quyền chủ động tắt tính năng ECH trong trang quản trị.
* **Đối với người dùng truy cập**: Bạn hãy tắt tính năng DNS mã hóa (DoH hoặc DoT) trên trình duyệt hoặc thiết bị của mình. Do công nghệ ECH bắt buộc phải dựa vào giao thức DNS mã hóa để lấy khóa công khai từ trước, việc sử dụng DNS thông thường sẽ không kích hoạt ECH, giúp kết nối trở lại bình thường.

## [活动] Diễn đàn công nghệ: Cách mạng quản lý trong kỷ nguyên trí tuệ nhân tạo

Vào Thứ Bảy tuần sau (ngày 28 tháng 10), tại Bắc Kinh sẽ diễn ra buổi hội thảo công nghệ quy mô lớn mang tên “Diễn đàn Sáng tạo Juejin”.

Chủ đề chính của diễn đàn năm nay là **“Cách mạng quản lý trong kỷ nguyên AI”** với sự tham gia chia sẻ trực tiếp của 13 chuyên gia, học giả và nhà quản lý công nghệ hàng đầu trong lĩnh vực Internet tại Trung Quốc.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101813.webp)

Sự kiện được thiết kế dưới hình thức phối hợp giữa “Hội thảo chính và các phiên họp kín chuyên đề”, nơi các diễn giả sẽ chia sẻ về lộ trình ứng dụng AI thực tế tại doanh nghiệp của mình, phân tích các xu hướng công nghệ mới và thảo luận về những cơ hội, thách thức do làn sóng công nghệ AI tạo sinh mang lại.

Địa điểm tổ chức sự kiện tại Khách sạn Crowne Plaza Sun Palace, Bắc Kinh. **Các bạn lập trình viên muốn cập nhật các xu hướng phát triển AI mới nhất và giao lưu trực tiếp với các chuyên gia đầu ngành xin đừng bỏ lỡ cơ hội này.**

Hiện ban tổ chức đang mở cổng đăng ký vé tham dự. Độc giả của bản tin có thể **đăng ký nhận vé miễn phí** tham dự phiên hội thảo chính (trị giá gốc 3.999 Nhân dân tệ) bằng cách truy cập [liên kết đăng ký này](https://www.bagevent.com/event/8047254?bag_track=ruanyifeng) hoặc quét mã QR trong ảnh trên để nhận vé ưu đãi, số lượng vé tặng có hạn dành cho các độc giả đăng ký sớm nhất.

## 科技动态

1、[Adobe trình diễn công nghệ váy thông minh có khả năng đổi màu sắc họa tiết thời gian thực](https://people.com/adobe-debuts-interactive-dress-8358152)

Tại hội nghị công nghệ Adobe MAX 2023 diễn ra tuần trước, hãng phần mềm Adobe đã gây bất ngờ lớn khi trình diễn mẫu thiết kế váy thời trang thông minh có khả năng tự động thay đổi hoa văn hiển thị trên thân váy:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101607.webp)

Trưởng dự án nghiên cứu, cô Christine Dierk, đã trực tiếp mặc chiếc váy đặc biệt này lên sân khấu biểu diễn. Thân váy được kết tạo từ hàng trăm phiến vảy điện tử nhỏ có khả năng thay đổi màu sắc và hiển thị các họa tiết đồ họa chuyển động liên tục.

Hệ thống hiển thị của váy được điều khiển thông qua một nút bấm vật lý tích hợp sẵn hoặc điều khiển không dây bằng ứng dụng trên điện thoại di động. Nó có khả năng hiển thị trực tiếp các họa tiết thiết kế được tạo ra từ các công cụ sáng tạo của hãng như Adobe Firefly, After Effects hay Illustrator:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101608.webp)

Ý tưởng công nghệ này hứa hẹn sẽ tạo nên cuộc cách mạng cho ngành thời trang trong tương lai, khi người dùng chỉ cần tải về các tệp thiết kế để thay đổi màu sắc trang phục hàng ngày. Trước mắt, Adobe dự kiến sẽ thử nghiệm ứng dụng công nghệ hiển thị này lên các dòng sản phẩm túi xách thời trang cao cấp.

2、[Nghiên cứu mới về lịch sử tiến hóa chiều dài cổ của loài hươu cao cổ](https://www.nytimes.com/2022/06/02/science/giraffe-neck-evolution.html)

Tại sao hươu cao cổ lại sở hữu chiếc cổ dài vượt trội so với các loài động vật khác?

Thuyết tiến hóa truyền thống của Darwin giải thích rằng chiếc cổ dài giúp hươu cao cổ dễ dàng tiếp cận nguồn lá cây trên các ngọn cây cao mà các loài khác không tới được. Tuy nhiên, một công trình nghiên cứu khảo cổ học mới đây lại đưa ra giả thuyết rằng chiếc cổ dài ra thực chất là kết quả của việc cạnh tranh giành lợi thế khi chiến đấu:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082101.webp)

Các nhà khảo cổ học đã phát hiện một mẫu hóa thạch của loài tổ tiên hươu cao cổ tại lưu vực Chuẩn Cát Nhĩ, Tân Cương, Trung Quốc. Mẫu hóa thạch cho thấy loài tổ tiên này chưa có chiếc cổ dài như hiện nay, nhưng phần xương đỉnh đầu lại phát triển rất dày và phẳng trông giống như một chiếc mũ bảo hiểm kiên cố:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082102.webp)

Nghiên cứu chỉ ra cấu trúc xương này chứng minh hành vi chiến đấu tranh giành bạn tình của loài này là dùng đầu húc trực tiếp vào nhau với lực rất mạnh. Để gia tăng lực quán tính và giành lợi thế khi húc đầu chiến đấu, những cá thể sở hữu chiếc cổ dài hơn và khỏe hơn sẽ chiếm ưu thế vượt trội, dẫn tới quá trình chọn lọc tự nhiên khiến chiếc cổ của loài ngày một dài ra qua các thế hệ.

3、[Thương vụ mua lại phần mềm ghi màn hình Loom trị giá 1 tỷ USD của gã khổng lồ Atlassian](https://www.atlassian.com/blog/announcements/atlassian-acquires-loom)

Tập đoàn phần mềm quản trị dự án lớn của Úc Atlassian vừa qua đã công bố hoàn tất thương vụ mua lại ứng dụng ghi hình màn hình Loom với mức giá lên tới 1 tỷ USD. Thương vụ khiến giới công nghệ bất ngờ khi một công cụ có tính năng đơn giản như ghi màn hình lại đạt giá trị thương mại lớn đến vậy.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101304.webp)

Được thành lập từ năm 2015, Loom khởi đầu chỉ là một tiện ích mở rộng (extension) đơn giản trên trình duyệt Chrome (hình dưới), sau đó mới phát triển thêm các phiên bản phần mềm cho máy tính và điện thoại di động:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101302.webp)

Tính năng cốt lõi của Loom là tự động tải video ghi màn hình của người dùng lên máy chủ đám mây ngay khi dừng ghi và sinh nhanh một liên kết chia sẻ (URL). Người dùng chỉ cần gửi link này cho đồng nghiệp là họ có thể xem ngay video giải thích công việc trên trang web của Loom mà không cần tải file về:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101303.webp)

Tiện ích này đặc biệt hữu dụng cho công việc cộng tác nhóm từ xa của các doanh nghiệp khi cần giải thích các lỗi phần mềm hay hướng dẫn thao tác. Hiện Loom sở hữu hơn 20 vạn khách hàng trả phí doanh nghiệp và xử lý hơn 5 triệu lượt ghi hình mỗi tháng, mang lại giá trị chuyển nhượng lên tới tỷ USD. Điều này chứng minh một triết lý sản phẩm: ngay cả một tính năng phổ thông nếu được tối ưu hóa trải nghiệm người dùng đạt mức xuất sắc vẫn có thể tạo nên thành công kinh doanh lớn.

4、[Google thử nghiệm tích hợp bảng tin tức tổng hợp lên trang chủ công cụ tìm kiếm](https://arstechnica.com/gadgets/2023/10/google-com-tests-a-news-filled-homepage-just-like-bing-and-yahoo/)

Kể từ khi thành lập cho đến nay, giao diện trang chủ của công cụ tìm kiếm Google luôn trung thành với phong cách tối giản tuyệt đối: chỉ gồm logo hãng và một ô tìm kiếm duy nhất ở trung tâm:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101613.webp)

Tuy nhiên, phong cách thiết kế này có thể sẽ thay đổi trong tương lai. Các báo cáo công nghệ ghi nhận Google đang tiến hành thử nghiệm một giao diện trang chủ hoàn toàn mới tại thị trường Ấn Độ, tích hợp thêm các bảng thông tin thời tiết, tin tức đời sống và biến động thị trường chứng khoán ở phần dưới trang:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101614.webp)

Mặc dù đại diện Google khẳng định đây mới chỉ là một cuộc thử nghiệm giao diện trên quy mô nhỏ và chưa có kế hoạch áp dụng rộng rãi ra toàn cầu, sự thay đổi này cho thấy Google cũng đang có xu hướng biến trang chủ tìm kiếm của mình thành một cổng thông tin tổng hợp tương tự như Yahoo, Bing hay Baidu.

## Bài viết

1\. [Câu chuyện khởi nghiệp đầy kịch tính của Pavel Durov – nhà sáng lập ứng dụng bảo mật Telegram](https://finance.sina.cn/blockchain/2023-10-17/detail-imzrkyrm8917643.d.html)（Tiếng Trung）

Bài viết chi tiết khắc họa cuộc đời và chặng đường khởi nghiệp đầy thách thức của Pavel Durov – từ chỗ xây dựng mạng xã hội lớn nhất nước Nga VKontakte cho đến khi phải rời bỏ quê hương để sáng lập nên ứng dụng nhắn tin bảo mật Telegram và tham vọng xây dựng hệ sinh thái mã hóa tự do của ông.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101810.webp)

2\. [Hướng dẫn các phương pháp ghi đè xóa sạch dữ liệu trên ổ cứng an toàn trong Linux](https://mp.weixin.qq.com/s/w-pMU3_TD3dEPoW-XEde-A)（Tiếng Trung）

Việc xóa tệp bằng trình quản lý tệp tin đồ họa hoặc sử dụng câu lệnh `rm` thông thường thực chất chỉ gỡ bỏ liên kết chỉ mục, dữ liệu vật lý vẫn lưu trên ổ đĩa và có thể khôi phục lại dễ dàng. Bài viết hướng dẫn 3 công cụ dòng lệnh chuyên dụng trong Linux giúp ghi đè dữ liệu ngẫu nhiên nhiều lần để xóa sạch hoàn toàn dấu vết thông tin trên ổ cứng. (Đóng góp của [@xxxsalted](https://github.com/ruanyf/weekly/issues/3566))

3\. [Trình duyệt Firefox và Safari chính thức hỗ trợ cú pháp viết lồng quy tắc CSS gốc](https://webkit.org/blog/14571/css-nesting-and-the-cascade/)（Tiếng Anh）

Trước đây để sử dụng cú pháp viết lồng phần tử (Nesting CSS), lập trình viên bắt buộc phải sử dụng các công cụ biên dịch như SASS hay LESS. Hiện tại, các phiên bản chính thức của Firefox và Safari đã hỗ trợ trực tiếp cú pháp viết lồng nguyên bản (Native CSS Nesting), giúp mã nguồn CSS gọn gàng và dễ bảo trì hơn mà không cần qua bước build.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100513.webp)

4\. [Phân tích chi tiết phương pháp thiết lập bộ reset CSS tối ưu cho năm 2023](https://chriscoyier.net/2023/10/03/being-picky-about-a-css-reset-for-fun-pleasure/)（Tiếng Anh）

Bài viết mới nhất của chuyên gia CSS Chris Coyier (người sáng lập CSS-Tricks) phân tích chi tiết từng dòng mã trong bộ thiết lập lại thuộc tính hiển thị mặc định của trình duyệt (CSS Reset) hiện đại, giải thích lý do tại sao mỗi thuộc tính lại cần thiết cho quá trình phát triển giao diện hiện nay.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101611.webp)

5\. [Chia sẻ trải nghiệm tự xây dựng toàn bộ trang web cá nhân bằng Web Components](https://www.thesoftwarephilosopher.com/articles/2023-08-07-modern-90s-web-dev.html)（Tiếng Anh）

Tác giả chia sẻ chi tiết quá trình lập trình xây dựng giao diện website cá nhân sử dụng hoàn toàn công nghệ thành phần web nguyên bản (Web Components) được tích hợp sẵn trong các trình duyệt hiện đại mà không cần dùng đến các framework lớn như React hay Vue, mang lại tốc độ tải trang cực nhanh và cấu trúc mã nguồn gọn nhẹ.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080806.webp)

6\. [Chia sẻ bộ công cụ công nghệ phục vụ khởi nghiệp của một lập trình viên độc lập](https://getwaitlist.com/blog/solo-dev-startup-stack)（Tiếng Anh）

Một nhà phát triển độc lập chia sẻ danh sách các công cụ, dịch vụ SaaS và nền tảng hạ tầng đám mây (ưu tiên sử dụng các gói miễn phí) được anh lựa chọn sử dụng để xây dựng, vận hành và tiếp thị cho dự án startup cá nhân của mình một cách tối ưu chi phí nhất.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080807.webp)

7\. [Chào đón kỷ nguyên mới của các phần mềm dòng lệnh CLI và giao diện terminal TUI](https://www.trickster.dev/post/back-to-the-terminal-the-new-era-of-cli-and-tui-software/)（Tiếng Anh）

Mặc dù phần mềm giao diện đồ họa (GUI) là xu hướng chính, những năm gần đây chứng kiến sự phát triển mạnh mẽ của thế hệ các công cụ dòng lệnh (CLI) và giao diện đồ họa chạy trên terminal (TUI) viết bằng Go hay Rust với giao diện trực quan, tốc độ xử lý nhanh và phím tắt tiện lợi giúp nâng cao hiệu suất làm việc của lập trình viên.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080909.webp)

8\. [Hướng dẫn lập trình trích xuất siêu dữ liệu EXIF từ ảnh chụp của iPhone](https://hturan.com/writing/exploring-exif)（Tiếng Anh）

Bài viết hướng dẫn kỹ thuật viết mã script để tự động trích xuất các thông số EXIF (như tọa độ GPS, thời gian chụp, thông số khẩu độ, tiêu cự ống kính) từ kho ảnh chụp của iPhone và tổ chức lưu trữ vào cơ sở dữ liệu để thực hiện các phân tích thống kê thói quen chụp ảnh thú vị.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090702.webp)

## 工具

1、[Mycelite: Công cụ hỗ trợ đồng bộ dữ liệu thời gian thực giữa các file SQLite](https://github.com/mycelial/mycelite)

Một extension hữu ích dành cho cơ sở dữ liệu SQLite, hỗ trợ tự động theo dõi biến động dữ liệu và thực hiện đồng bộ hóa (replication) thời gian thực giữa các file SQLite cục bộ lên máy chủ, thích hợp cho các ứng dụng chạy offline-first.

2、[Pictode: Trình vẽ sơ đồ đồ họa mã nguồn mở chạy trên trình duyệt web](https://github.com/JessYan0913/pictode)

Một thư viện mã nguồn mở hỗ trợ xây dựng công cụ vẽ sơ đồ thiết kế, bảng vẽ tư duy trực quan ngay trên nền tảng web với khả năng tùy biến cao. (Đóng góp của [@JessYan0913](https://github.com/ruanyf/weekly/issues/3567))

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101901.webp)

3、[Squircle-CE: Trình biên tập mã nguồn mở viết code trực tiếp trên điện thoại Android](https://github.com/massivemadness/Squircle-CE)

Ứng dụng di động mã nguồn mở dành cho lập trình viên sử dụng điện thoại Android, cung cấp trình soạn thảo code hỗ trợ highlight cú pháp của hầu hết các ngôn ngữ lập trình phổ biến giúp sửa code nhanh khi đang di chuyển.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062813.webp)

4、[LocalSend: Công cụ truyền tải file đa nền tảng không cần kết nối Internet](https://localsend.org/)

Một phần mềm mã nguồn mở cho phép truyền nhận tệp tin nhanh chóng giữa các thiết bị khác nhau (Windows, macOS, Linux, Android, iOS) cùng kết nối trong một mạng Wi-Fi nội bộ mà không cần tải file lên máy chủ trung gian qua Internet.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101903.webp)

5、[Uninstallr: Phần mềm hỗ trợ gỡ cài đặt sạch sẽ các ứng dụng trên Windows](https://uninstalr.com/)

Công cụ miễn phí dành cho người dùng Windows, hỗ trợ quét sâu hệ thống để gỡ bỏ hoàn toàn mã nguồn của phần mềm, tự động dọn dẹp các khóa đăng ký registry và tệp tin rác phát sinh trong quá trình sử dụng để giải phóng bộ nhớ máy tính.

6、[Auto-i18n: Công cụ tự động dịch thuật tài liệu Markdown bằng ChatGPT](https://github.com/linyuxuanlin/Auto-i18n)

Giải pháp kỹ thuật tự động hóa: sử dụng kết hợp dịch vụ GitHub Actions và API của ChatGPT để tự động phát hiện các thay đổi và tiến hành dịch thuật các tệp tài liệu Markdown trong kho lưu trữ sang các ngôn ngữ khác phục vụ làm web đa ngôn ngữ. (Đóng góp của [@linyuxuanlin](https://github.com/ruanyf/weekly/issues/3564))

7、[ffmpeg online: Công cụ biên tập và xử lý video bằng ffmpeg trực tiếp trên web](https://ffmpeg-online.vercel.app/)

Một trang web ứng dụng công nghệ WebAssembly cho phép chạy các câu lệnh biên tập, chuyển đổi định dạng và cắt ghép video bằng công cụ ffmpeg trực tiếp trên trình duyệt mà không cần cài đặt phần mềm về máy tính.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101610.webp)

8、[little-rat: Tiện ích Chrome hỗ trợ giám sát kết nối mạng của các extension khác](https://github.com/dnakov/little-rat)

Extension bảo mật dành cho trình duyệt Chrome, có khả năng thống kê chi tiết toàn bộ các yêu cầu HTTP kết nối ra ngoài mạng của các extension khác đang cài đặt trên máy để phát hiện xem có extension nào đang âm thầm gửi dữ liệu người dùng lên máy chủ lạ hay không.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082302.webp)

9、[Fooocus: Phần mềm máy tính hỗ trợ sinh ảnh nghệ thuật từ văn bản chạy offline](https://github.com/lllyasviel/Fooocus)

Một công cụ máy tính để bàn cho phép người dùng chạy trực tiếp mô hình Stable Diffusion offline để vẽ tranh từ các câu lệnh văn bản (Text-to-Image) với giao diện tinh giản, dễ thao tác hơn so với các bản phân phối khác.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081304.webp)

10\. [try: Công cụ tạo môi trường hộp cát thử nghiệm các câu lệnh trong Linux](https://github.com/binpash/try)

Một công cụ dòng lệnh độc đáo dành cho các quản trị viên hệ thống Linux: tự động tạo ra một môi trường hộp cát (sandbox) tạm thời để chạy thử nghiệm các lệnh cài đặt phần mềm hay chạy thử script hệ thống nhằm đánh giá tác động trước khi quyết định áp dụng thực tế lên hệ điều hành gốc.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062508.webp)

## 资源

1\. [Google Coding Competitions: Trang web lưu trữ đề thi lập trình của Google](https://zibada.guru/gcj/)

Website cộng đồng thu thập toàn bộ dữ liệu đề thi, kết quả và các bài giải mẫu của các kỳ thi lập trình quy mô toàn cầu do Google tổ chức qua các năm (như Google Code Jam) để lập trình viên tự ôn luyện thuật toán.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060304.webp)

2、[dbdb.io: Bách khoa toàn thư giới thiệu các hệ quản trị cơ sở dữ liệu thế giới](https://dbdb.io/)

Trang web thư viện chuyên thu thập thông tin giới thiệu chi tiết về kiến trúc kỹ thuật, tính năng và lịch sử phát triển của hơn 900 hệ quản trị cơ sở dữ liệu (từ SQL truyền thống đến các cơ sở dữ liệu phân tán mới) trên thế giới.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023083002.webp)

3\. [STAT.md: Thống kê số lượng trang web đăng ký theo các tên miền cao cấp](https://github.com/tb0hdan/domains/blob/master/STATS.md)

Một file tài liệu thống kê chi tiết trong kho lưu trữ GitHub, cung cấp danh sách xếp hạng tất cả các tên miền cao cấp (TLD như `.com`, `.net`, `.io`) sắp xếp theo thứ tự số lượng website đăng ký hoạt động thực tế trên thế giới.

4\. [Nix start: Tài liệu hướng dẫn nhập môn công cụ quản lý gói Nix](https://gitlab.com/engmark/nix-start)

Tài liệu hướng dẫn cơ bản dành cho những lập trình viên bắt đầu tiếp cận công cụ quản lý gói Nix (Nix Package Manager), giải thích phương pháp cấu hình môi trường phát triển độc lập cho dự án.

5\. [Flash Museum: Kho lưu trữ trực tuyến các tác phẩm nghệ thuật và game bằng Flash](https://flashmuseum.org/)

Trang web lưu trữ hàng ngàn game mini, phim hoạt hình và tác phẩm nghệ thuật tương tác được phát triển bằng công nghệ Adobe Flash thời kỳ đầu, tích hợp sẵn công cụ giả lập để chạy trực tiếp trên các trình duyệt hiện đại.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072914.webp)

## 图片

1、**Bộ ảnh chụp nghệ thuật thế giới thủy sinh sinh động của National Geographic**

Một nhiếp ảnh gia của tạp chí địa lý nổi tiếng *National Geographic* đã dành nhiều năm thực hiện bộ ảnh chụp chuyên sâu về đời sống của các loài bạch tuộc, hải mã và sứa biển:

* Hình ảnh cận cảnh chi tiết một chú bạch tuộc:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062706.webp)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062707.webp)

* Vẻ đẹp của loài hải mã dưới đại dương:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062708.webp)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062709.webp)

* Vẻ đẹp lung linh huyền ảo của loài sứa phát quang:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062710.webp)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062711.webp)

2、**Khám phá khả năng ngụy trang hòa mình vào thiên nhiên ấn tượng của loài chim cú**

Loài chim cú mèo có cấu trúc lông đặc biệt giúp chúng dễ dàng ẩn mình vào vỏ cây hay các khe đá xung quanh để tránh kẻ thù và rình rập săn mồi:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111004.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111005.webp)

Hai bức ảnh trên ghi lại các khoảnh khắc ngụy trang thực tế của chim cú, bạn đọc có nhận diện được vị trí chú chim cú đang lẩn trốn trong ảnh hay không?

## ✍️ Bài đọc thêm

### Tại sao các tàu vũ trụ trong phim khoa học viễn tưởng luôn gặp lỗi thiết kế hệ thống trọng lực nhân tạo?

Trong hầu hết các bộ phim điện ảnh viễn tưởng lấy bối cảnh du hành không gian, người xem luôn thấy các phi hành gia đi lại tự do trong khoang tàu giống hệt như đang ở mặt đất. Đây thực chất là một hạt sạn kỹ thuật lớn.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101804.webp)

Trong môi trường không gian vũ trụ ngoài Trái Đất, lực hấp dẫn gần như bằng không và các phi hành gia bắt buộc phải ở trạng thái lơ lửng mất trọng lực. Việc các đạo diễn thiết kế cảnh đi lại bình thường chủ yếu nhằm mục đích giúp người xem dễ đồng cảm với nhân vật và tiết kiệm chi phí dàn dựng kỹ xảo lơ lửng.

Tại sao các kỹ sư vũ trụ hiện nay vẫn chưa thể thiết lập được hệ thống trọng lực nhân tạo trên các trạm vũ trụ?

Về mặt vật lý học, phương án khả thi duy nhất hiện nay để tạo ra trọng lực nhân tạo trong không gian là thiết kế trạm vũ trụ dưới dạng một vòng tròn xoay quanh một trục trung tâm để tận dụng lực ly tâm. Lực ly tâm hướng ra phía ngoài vòng xoay sẽ ép chân người dùng vào thành trong của vòng, đóng vai trò tương tự như lực hấp dẫn kéo chúng ta xuống sàn nhà trên Trái Đất:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101805.webp)

Trong một con tàu vũ trụ dạng vòng xoay này, phi hành gia sẽ đi bộ vuông góc với trục của con tàu, lúc này phần tường ngoài của tàu sẽ đóng vai trò là sàn nhà:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101806.webp)

Tuy nhiên, rào cản lớn nhất nằm ở Kích thước vật lý của con tàu. Lực ly tâm phụ thuộc vào tốc độ tự quay và bán kính vòng quay. Bán kính vòng quay càng nhỏ thì tốc độ tự quay bắt buộc phải càng nhanh để đạt được lực ly tâm cần thiết. Do cơ thể con người không thể chịu đựng được cảm giác chóng mặt do tốc độ tự quay quá nhanh, chúng ta bắt buộc phải xây dựng các con tàu có kích thước vòng quay vô cùng khổng lồ để giảm tốc độ quay xuống mức an toàn.

Để tạo ra lực ly tâm tương đương với trọng lực Trái Đất (1g) với tốc độ quay an toàn cho cơ thể người là chỉ quay đúng 1 vòng trong ngày (24 giờ), chúng ta cần chế tạo một vòng xoay có đường kính lên tới **3,71 triệu km** (lớn gấp gần 300 lần đường kính của Trái Đất) với tốc độ quay của vành ngoài đạt 486.000 km/h:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101807.webp)

Với quy mô khổng lồ đó, việc chế tạo một con tàu vũ trụ có trọng lực nhân tạo bằng lực ly tâm là điều bất khả thi đối với trình độ kỹ thuật hiện nay của nhân loại. Các phi hành gia muốn trải nghiệm lại cảm giác có trọng lực bắt buộc phải đáp xuống bề mặt của các hành tinh khác.

Trên Internet có chia sẻ [một đoạn video ngắn](https://erikwernquist.com/one-revolution-per-minute) mang tên *“Một vòng mỗi phút”* (One revolution per minute) mô phỏng chân thực và trực quan cuộc sống sinh hoạt bên trong một trạm vũ trụ dạng vòng xoay lực ly tâm khổng lồ, một tài liệu rất đáng xem dành cho những bạn đọc yêu thích khoa học vũ trụ.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101808.webp)

## Lịch sử tuần này

- 2022年（第 227 期）：[Văn hóa doanh nghiệp: Tìm hiểu quy trình đào tạo và hòa nhập văn hóa dành cho nhân viên mới tại Facebook](http://www.ruanyifeng.com/blog/2022/10/weekly-issue-227.html)
- 2021年（第 177 期）：[Thiết bị di động: Thảo luận về những vai trò và ứng dụng thực tế phù hợp nhất của máy tính bảng iPad](http://www.ruanyifeng.com/blog/2021/09/weekly-issue-177.html)
- 2020年（第 127 期）：[Xu hướng công nghệ: Dự báo tương lai khi lập trình không code phổ cập giúp ai cũng có thể tạo phần mềm](http://www.ruanyifeng.com/blog/2020/09/weekly-issue-127.html)
- 2019年（第 77 期）：[Giải trí: Giới thiệu và phân tích ý tưởng công nghệ AR độc đáo trong bộ phim truyền hình Hàn Quốc “Ký ức Alhambra”](http://www.ruanyifeng.com/blog/2019/10/weekly-issue-77.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
