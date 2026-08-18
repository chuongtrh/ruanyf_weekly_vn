# Bản tin chia sẻ công nghệ (Số 341): Lập trình Low-code e rằng sẽ không thành công

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/6189) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031213.webp)

Tại Thành Đô mới đây xuất hiện mô hình ăn lẩu giữa ruộng hoa cải vô cùng độc đáo. Quán lẩu ngoài trời này được dựng ngay giữa cánh đồng hoa cải đang nở rộ và dự kiến chỉ vận hành trong vòng hai tháng của mùa hoa. (Nguồn: [163.com](https://www.163.com/dy/article/JPP0TJOJ0552XKPD.html))

## 低代码编程，恐怕不会成功

Trong suốt hơn một thập kỷ qua, làn sóng các lập trình viên nối tiếp nhau dấn thân nghiên cứu phát triển các giải pháp lập trình Low-code (bao gồm cả No-code). Ngay xung quanh tôi cũng đã ghi nhận ba bốn nhóm khởi nghiệp theo đuổi định hướng này.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031208.webp)

Theo cách hiểu của tôi, bản chất của lập trình Low-code là cho phép người dùng kéo thả các thành phần giao diện trực quan trên một khung thiết kế đồ họa, từ đó hệ thống sẽ tự động biên dịch sinh ra mã nguồn giao diện (UI) tương ứng phía sau để giảm thiểu tối đa thao tác viết code thủ công.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031210.webp)

Ý tưởng này vô cùng tuyệt vời và giải quyết tốt nhu cầu thực tế của rất nhiều người, đặc biệt là những người hoàn toàn không biết lập trình. Đối với họ, đây gần như là giải pháp khả thi duy nhất để tự tạo ra một ứng dụng phần mềm.

Tuy nhiên điều kỳ lạ là hầu hết các dự án này đều đi đến thất bại mà không có ngoại lệ. Các công cụ Low-code được phát triển ban đầu có thể thu hút một lượng người dùng tò mò dùng thử, nhưng họ cũng nhanh chóng rời bỏ sản phẩm. Lượng người dùng sụt giảm nhanh chóng và về sau ngay cả khi dự án được chuyển đổi sang dạng mã nguồn mở miễn phí cũng hầu như không còn ai ngó ngàng.

Đáng chú ý hơn, đây hoàn toàn không phải là một hiện tượng cá biệt. **Hầu như toàn bộ các công cụ Low-code trên thị trường đều không đạt được sự thành công thương mại bền vững**. Rất khó để chúng ta có thể chỉ ra được một ứng dụng phần mềm phổ biến nào trên thị trường hiện nay được phát triển hoàn toàn từ một công cụ Low-code.

Hệ quả này xuất phát từ nguyên nhân cốt lõi nào? Do quy trình thực thi chưa đúng cách hay do chính bản chất của triết lý lập trình Low-code vốn dĩ không khả thi?

Tôi từng dành nhiều thời gian suy ngẫm mà vẫn chưa tìm được câu trả lời thỏa đáng. Dù không thực sự đánh giá cao, tôi vẫn nhen nhóm một kỳ vọng rằng biết đâu vào một ngày nào đó, lập trình Low-code sẽ vươn lên thành xu hướng chủ đạo, cho phép bất kỳ ai cũng có thể tự tạo ứng dụng di động hay ứng dụng máy tính chỉ bằng vài thao tác kéo thả chuột đơn giản.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031209.webp)

Chỉ đến tuần trước, sau khi đọc được bài phân tích mang tựa đề [《Lập trình Low-code đang bị mắc kẹt vào hình thức hiển thị》](https://interjectedfuture.com/visual-programming-is-stuck-on-the-form/) (hình dưới), tôi mới hoàn toàn thấu suốt vấn đề: **Lập trình Low-code sở hữu một khuyết tật bẩm sinh về mặt triết lý thiết kế và đó là lý do e rằng nó sẽ không bao giờ thành công**.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031211.webp)

Tác giả lập luận rằng mọi tác phẩm phần mềm xuất sắc đều là sự kết hợp hài hòa thống nhất giữa Hình thức (Form - giao diện hiển thị) và Công năng (Function - logic vận hành bên dưới). Trong đó, **hình thức bắt buộc phải phục vụ công năng, và chính công năng sẽ quyết định hình thức** (form follows function).

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031212.webp)

Đối với một lập trình viên xuất sắc, chỉ cần họ thấu suốt và xây dựng tốt logic vận hành bên dưới hệ thống, cấu trúc giao diện người dùng (UI) tương ứng sẽ tự động hiển hiện một cách vô cùng tự nhiên và hợp lý.

**Điểm nghẽn cốt lõi của lập trình Low-code nằm ở chỗ nó đi ngược lại quy luật này: thiết lập Hình thức (UI) trước rồi mới biên dịch sinh ra Công năng (mã nguồn logic) sau**.

Người dùng tiến hành kéo thả để phác họa ra giao diện UI trước, sau đó hệ thống mới dựa trên giao diện này để tự động chắp vá sinh ra các đoạn code vận hành phía sau. Quy trình 본末倒置 (đảo ngược gốc ngọn) này ép buộc mã nguồn logic bên dưới phải tìm cách thích ứng với giao diện hiển thị đã được định hình cứng, dẫn đến việc cả hai thành phần đều phát sinh lỗi: Giao diện UI được tạo ra dựa trên sự tưởng tượng chủ quan thiếu thực tế, còn mã nguồn logic sinh ra để đáp ứng UI đó chắc chắn sẽ vô cùng rườm rà và kém hiệu quả.

Do đó, các ứng dụng phần mềm chất lượng cao không bao giờ có thể được kiến tạo nên từ phương thức phát triển này, và lập trình Low-code khó lòng thành công.

Tôi hoàn toàn đồng ý với góc nhìn phân tích này của tác giả. **Lập trình Low-code không có khả năng khắc phục được khuyết tật bẩm sinh này**, dẫn đến việc không gian ứng dụng thực tế của nó vô cùng hạn chế, phần lớn chỉ phù hợp để xử lý các tác vụ quản lý dữ liệu đơn giản hoặc tạo nhanh các bản mẫu thử nghiệm (prototypes) giao diện chứ không thể trở thành công cụ lập trình chủ đạo. Các lập trình viên nên hết sức thận trọng khi quyết định đầu tư thời gian phát triển dòng công cụ này do nguy cơ cao toàn bộ nỗ lực sẽ đổ sông đổ bể.

Đến đây, một câu hỏi thú vị được đặt ra là: **Liệu lập trình ứng dụng AI có thể được coi là một dạng lập trình Low-code (hoặc No-code) thế hệ mới hay không?** Nếu Low-code khó thành công, liệu lập trình bằng AI có thể đi đến thành công hay không?

Tôi cho rằng AI sở hữu triết lý vận hành khác biệt hoàn toàn so với Low-code. Trong khi lập trình Low-code đòi hỏi người dùng phải tự thiết kế giao diện UI trước để hệ thống sinh code sau, thì AI đảm nhận việc đồng thời kiến tạo cả giao diện UI lẫn mã nguồn logic bên dưới dựa trên các mô tả yêu cầu bằng ngôn ngữ tự nhiên từ phía người dùng.

Trong kịch bản này, sự kết hợp thống nhất giữa hình thức và công năng của sản phẩm sẽ phụ thuộc hoàn toàn vào năng lực nhận thức và xử lý của hệ thống AI. Nếu trong tương lai, công nghệ AI có thể tự sinh ra các đoạn video chất lượng cao với hình ảnh đẹp mắt và cốt truyện mạch lạc, thì lập trình AI chắc chắn cũng sẽ đi đến thành công để tự kiến tạo nên các ứng dụng phần mềm có sự đồng nhất hoàn hảo giữa giao diện và logic vận hành.

## 小程序容器 FinClip

Các bạn có chú ý đến một xu hướng phát triển công nghệ nổi bật của các ứng dụng di động trong những năm gần đây hay không?

Đó chính là **xu hướng tích hợp các bộ khung chạy ứng dụng nhỏ (Mini Program Containers)** để biến ứng dụng của mình thành một nền tảng (super app) có khả năng vận hành trực tiếp các phần mềm nhỏ của bên thứ ba.

Xu hướng này không chỉ bùng nổ mạnh mẽ tại thị trường nội địa Trung Quốc mà còn đang được nhiều siêu ứng dụng trên thị trường quốc tế tích cực học hỏi triển khai, tiêu biểu như YouTube, Telegram hay Line.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030908.webp)

Bức ảnh phía trên giới thiệu tính năng "Playables" (Trò chơi nhỏ) được tích hợp trực tiếp bên trong ứng dụng YouTube, hoạt động với cơ chế hoàn toàn tương tự như các chương trình nhỏ (Mini Programs) của WeChat.

Nguyên nhân dẫn đến xu hướng này xuất phát từ việc cấu trúc ứng dụng nhỏ sở hữu tính linh hoạt cực cao, cho phép dễ dàng tích hợp và cập nhật nhanh các tính năng mới mà không cần cập nhật toàn bộ app, giúp xây dựng hệ sinh thái đối tác phong phú và gia tăng cơ hội thương mại hóa sản phẩm.

Hôm nay tôi xin giới thiệu một giải pháp công nghệ quản lý ứng dụng nhỏ nội địa chất lượng cao mang tên **FinClip**. Nếu bạn đang tìm kiếm giải pháp tích hợp hệ sinh thái ứng dụng nhỏ vào ứng dụng di động cá nhân, đây là công cụ vô cùng hữu ích.

FinClip cung cấp một giải pháp công nghệ ứng dụng nhỏ toàn diện và ăn liền, cung cấp sẵn các gói SDK chuyên dụng giúp nhà phát triển dễ dàng **nhúng môi trường chạy ứng dụng nhỏ trực tiếp vào bên trong ứng dụng di động của mình**.

Với sự hỗ trợ của FinClip, bất kỳ nhà phát triển nào cũng có thể nhanh chóng xây dựng nên một "vũ trụ ứng dụng nhỏ" riêng biệt hoạt động đa nền tảng từ iOS, Android cho đến HarmonyOS. Hình dưới đây giới thiệu danh sách các nền tảng thiết bị được FinClip hỗ trợ nhúng SDK:

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030909.webp)

Có thể thấy ngoài hệ điều hành di động thông thường, công cụ còn hỗ trợ nhúng tốt vào các ứng dụng chạy trên máy tính (Desktop), hệ thống màn hình điều khiển ô tô (In-Car), TV thông minh...

Bên cạnh đó, giải pháp còn sở hữu một số ưu thế kỹ thuật vượt trội:

**（1）Khả năng tương thích tuyệt vời**: Hệ thống tương thích hoàn toàn với cấu trúc mã nguồn của ứng dụng nhỏ WeChat, Alipay và Douyin. Nhà phát triển có thể trực tiếp đưa các ứng dụng nhỏ WeChat hiện có vào vận hành ngay trong ứng dụng của mình mà không cần sửa đổi bất kỳ dòng code nào.

**（2）Quy trình cập nhật linh hoạt**: Các bản cập nhật của ứng dụng nhỏ tích hợp qua FinClip được phân phối trực tiếp từ máy chủ mà hoàn toàn không cần trải qua quy trình kiểm duyệt phức tạp của các kho ứng dụng (App Store/Google Play), giúp rút ngắn chu kỳ cập nhật xuống mức vài giờ.

**（3）Hỗ trợ công cụ chạy game chuyên dụng**: Đi kèm hệ thống là bộ khung tương tác nội dung game thời gian thực mang tên RealClip cung cấp môi trường vận hành tối ưu cho các tựa game nhỏ di động.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031005.webp)

Bộ khung này được tối ưu hóa sâu về mặt hiệu năng và độ tương thích đồ họa cho game di động, tương thích tốt với mã nguồn game WeChat và hỗ trợ các công cụ phát triển game phổ biến trên thị trường như Unity, Cocos, Laya, Egret Engine cũng như WebView. Điều này đồng nghĩa với việc hầu như mọi tựa game nhỏ được xây dựng từ các công cụ phổ biến đều có thể chạy mượt mà ngay trên app của bạn.

**（4）Bộ công cụ hỗ trợ FinClip Studio**: Công cụ hỗ trợ chuyển đổi nhanh toàn bộ mã nguồn của ứng dụng nhỏ hoặc game nhỏ hiện có thành một ứng dụng độc lập (standalone app) chỉ bằng một click chuột, tự động đóng gói thành các tệp tin cài đặt tương ứng cho hệ điều hành iOS, Android và HarmonyOS.

Tóm lại, nếu bạn đang lên kế hoạch tích hợp hệ sinh thái ứng dụng nhỏ vào app của mình, hoặc mong muốn ứng dụng nhỏ hiện tại của mình có thể vận hành trên các ứng dụng khác (máy tính hoặc di động), **FinClip** là giải pháp rất đáng để trải nghiệm thử.

Các bạn có thể truy cập [trang chủ FinClip](https://www.finclip.com/landpage-product/?from=ruan) để tìm hiểu thêm thông tin chi tiết và đăng ký trải nghiệm dịch vụ hoàn toàn miễn phí. Mọi thắc mắc kỹ thuật có thể tham gia trao đổi trực tiếp tại cộng đồng nhà phát triển của hãng (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030910.webp)

## [活动] AI 创意挑战赛，开始投票了

Như đã giới thiệu trong số bản tin tuần trước, bảng đấu "Đề xuất Ý tưởng" thuộc khuôn khổ giải đấu lập trình ứng dụng AI cấp quốc gia đầu tiên đã chính thức mở cổng nhận bài thi dành cho toàn bộ công chúng có ý tưởng sáng tạo mà không yêu cầu kỹ năng viết code.

Sau khi thông tin được phát hành, chương trình đã nhận được sự quan tâm vô cùng lớn từ cộng đồng. Thông tin từ ban tổ chức cho biết hệ thống đã ghi nhận hàng trăm ý tưởng sáng tạo độc đáo được gửi về dự thi.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031307.webp)

Kể từ ngày hôm nay (14 tháng 3), **cuộc thi chính thức bước vào giai đoạn bình chọn từ cộng đồng**. Xin mời các bạn cùng tham gia bình chọn cho những ý tưởng sáng tạo hấp dẫn và khả thi nhất. Đây cũng là cơ hội tuyệt vời để các bạn tìm kiếm thêm nguồn cảm hứng sáng tạo cho các dự án phát triển cá nhân của mình.

**Toàn bộ người dùng tham gia bình chọn đều có cơ hội nhận lượt bốc thăm trúng thưởng** các phần quà lưu niệm dễ thương từ ban tổ chức như đèn ngủ mini, bao đựng thẻ nhân viên, quạt cầm tay di động... Do lượt bình chọn được đặt lại hằng ngày, bạn hoàn toàn có thể quay lại bình chọn vào ngày hôm sau để nhận thêm nhiều lượt quay thưởng may mắn.

Đối với những bạn vẫn chưa kịp gửi ý tưởng dự thi, cổng nhận bài thi của bảng đấu "Đề xuất Ý tưởng" vẫn tiếp tục mở để đón nhận bài thi của các bạn.

Các thí sinh đã gửi bài dự thi **đừng quên chủ động chia sẻ liên kết bài thi** lên các nền tảng mạng xã hội cá nhân (như WeChat Official Accounts, Bilibili, Xiaohongshu, vòng kết nối bạn bè, các cộng đồng công nghệ...) để kêu gọi bình chọn từ cộng đồng nhằm gia tăng cơ hội đạt giải thưởng cao nhất của cuộc thi.

Các bạn có thể truy cập [địa chỉ liên kết của cuộc thi](https://sourl.co/5thdnz) hoặc quét mã QR trên poster để xem chi tiết danh sách bài thi và tham gia bình chọn.

## 科技动态

1、[Mốc lịch sử mới của y học: Bệnh nhân đầu tiên sống sót với trái tim nhân tạo](https://www.theguardian.com/australia-news/2025/mar/12/australian-man-survives-100-days-with-artificial-heart-in-world-first-success)

Một bệnh nhân nam người Úc sau khi được phẫu thuật cấy ghép thiết bị tim nhân tạo (hình dưới) đã sống sót ổn định qua mốc 100 ngày và chính thức được xuất viện về nhà, xác lập một kỷ lục y khoa thế giới mới.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031205.webp)

Thiết bị hoạt động tương tự như một hệ thống bơm máu cơ học được cấy trực tiếp vào lồng ngực, hoạt động liên tục 24/7 để thúc đẩy tuần hoàn máu cho cơ thể thay thế hoàn toàn cho quả tim sinh học đã suy yếu.

Bệnh nhân này hiện là người duy nhất trên thế giới đang duy trì sự sống bằng thiết bị tim nhân tạo cơ học này, và đây là ca cấy ghép thành công thứ 6 trong lịch sử y học thế giới. Trong 5 ca cấy ghép trước đó, thiết bị chỉ đóng vai trò hỗ trợ tạm thời trong thời gian bệnh nhân chờ đợi nguồn tạng hiến tặng từ người khác để tiến hành cấy ghép sinh học.

Nếu công nghệ chế tạo tim nhân tạo cơ học đạt độ chín muồi trong tương lai, tuổi thọ trung bình của nhân loại hứa hẹn sẽ được kéo dài một cách đáng kể.

2、[Giải pháp tái chế bo mạch điện thoại cũ thành thiết bị định tuyến](https://www.cnx-software.com/2025/03/02/citronics-built-a-router-based-on-the-fairphone-2-mainboard/)

Chúng ta có thể làm gì để tái chế các dòng điện thoại thông minh lỗi thời?

Một doanh nghiệp tại Bỉ đã đưa ra giải pháp tháo dỡ bo mạch chủ của điện thoại cũ, tích hợp thêm các cổng kết nối mạng LAN và cổng USB chuyên dụng để chuyển đổi nó thành một thiết bị định tuyến (router) mạng hiệu năng cao.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030620.webp)

Bức ảnh bên trái hiển thị bo mạch gốc của điện thoại di động và bức ảnh bên phải hiển thị kết quả sau khi nhúng bo mạch này vào bo mạch mở rộng chuyên dụng để tạo thành bo mạch chủ hoàn chỉnh cho router.

Do tận dụng lại được bộ vi xử lý CPU, modem kết nối và bộ nhớ RAM hiệu năng cao có sẵn của điện thoại, chi phí chế tạo thiết bị đạt mức rất thấp. Đồng thời, cấu hình phần cứng của điện thoại thông minh thường vượt trội hơn nhiều so với các dòng router thông dụng trên thị trường, mang lại hiệu năng xử lý định tuyến vô cùng mạnh mẽ.

3、[Sự thay đổi nhỏ trên phím bấm tắt tiếng của Apple](https://www.macrumors.com/2025/03/07/new-macbook-air-corrects-design-mistake/)

Dòng máy tính xách tay MacBook Air chip M4 vừa được Apple giới thiệu vào tuần trước đã âm thầm ghi nhận một thay đổi nhỏ về mặt thiết kế biểu tượng phím bấm vốn đã tồn tại suốt 26 năm qua của hãng.

Hãng đã tiến hành bổ sung thêm một đường gạch chéo đè lên biểu tượng chiếc loa trên phím tắt tiếng (phím F10 trên bàn phím).

Hình ảnh biểu tượng phím tắt tiếng truyền thống trước đây của hãng:

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030905.webp)

Và hình ảnh biểu tượng mới được cập nhật trên dòng máy mới:

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030906.webp)

Một chi tiết thiết kế nhỏ và trực quan như vậy nhưng hãng Apple đã mất tới 26 năm mới chính thức thực hiện thay đổi.

4、[Xu hướng quay trở lại ứng dụng nút bấm vật lý trên ô tô](https://www.autocar.co.uk/car-news/new-cars/volkswagen-reintroducing-physical-controls-vital-functions)

Tập đoàn sản xuất ô tô Volkswagen (Đức) công bố kế hoạch trong tương lai toàn bộ các dòng xe mới của hãng sẽ được thiết kế song song cả màn hình cảm ứng trung tâm kết hợp cùng hệ thống các phím bấm vật lý truyền thống cho các tính năng cốt lõi.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030904.webp)

Bức ảnh phía trên giới thiệu không gian điều khiển cabin của dòng xe điện Volkswagen ID.3, với khu vực màn hình cảm ứng lớn ở phía trên kết hợp cùng dãy nút bấm vật lý được bố trí trực quan ở phía dưới.

Đại diện hãng sản xuất chia sẻ ô tô là phương tiện di chuyển đòi hỏi tính an toàn cao chứ không đơn thuần là một chiếc điện thoại di động cỡ lớn, do đó việc phó mặc toàn bộ các thao tác điều khiển cho màn hình cảm ứng là rất thiếu an toàn. Các tính năng vận hành thiết yếu bắt buộc phải được bố trí ở các vị trí cố định và đi kèm cảm giác phản hồi vật lý chân thực giúp người lái dễ dàng thao tác mà không cần rời mắt khỏi mặt đường.

5、**Các tin tức khác**

(1) Một doanh nghiệp công nghệ sinh học tại Anh công bố nghiên cứu thành công giống chuối biến đổi gen đặc biệt có khả năng duy trì lớp vỏ màu vàng tươi sáng trong suốt thời gian dài vận chuyển và tiêu thụ mà hoàn toàn không bị thâm đen hay xỉn màu do quá trình oxy hóa.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030903.webp)

Ngay cả ở điều kiện sau khi bóc vỏ 12 tiếng, phần thịt chuối vẫn giữ nguyên màu sắc tươi mới ban đầu giúp giảm thiểu đáng kể tỷ lệ hao hụt thực phẩm cho các đơn vị phân phối.

(2) Hệ điều hành Android 15 dự kiến sẽ tích hợp sẵn một ứng dụng terminal Linux mặc định, cung cấp môi trường ảo hóa chạy một bản phân phối Linux Debian hoàn chỉnh trực tiếp trên điện thoại cho người dùng khai thác.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031104.webp)

Tính năng này vận hành dựa trên cơ chế máy ảo (virtual machine), hỗ trợ đắc lực cho cộng đồng lập trình viên trong việc tận dụng trực tiếp chiếc điện thoại Android cá nhân làm một máy tính chạy Linux di động tiện lợi.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031105.webp)

## 文章

1、[Tổng hợp toàn cảnh các bước tiến đột phá của mô hình lớn AI trong năm 2024](https://simonwillison.net/2025/Mar/8/nicar-llms/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030907.webp)

Nội dung bài phát biểu chi tiết ngày 7 tháng 3 của lập trình viên nổi tiếng Simon Willison, giới thiệu một cách dễ hiểu và trực quan về những bước tiến công nghệ thần tốc của ngành công nghiệp trí tuệ nhân tạo trong suốt năm vừa qua. Đây là bài viết tổng hợp vô cùng chất lượng cho cộng đồng công nghệ.

2、[Hướng dẫn ứng dụng công cụ Claude Code để dịch ngược mã nguồn (Decompile)](https://ghuntley.com/tradecraft/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030616.webp)

Tác giả chia sẻ một thử nghiệm thực tế kinh ngạc khi ứng dụng trợ lý lập trình Claude Code của Anthropic để phân tích các tệp tin nén thành phẩm sinh ra từ Webpack và thực hiện dịch ngược thành công toàn bộ mã nguồn ban đầu của dự án.

3、[Tìm hiểu kỹ thuật chuyển trang mượt mà bằng CSS View Transitions](https://simonwillison.net/2025/Mar/10/building-websites-with-llms/) (tiếng Anh)

Bài viết hướng dẫn cách thức khai thác tính năng chuyển đổi giao diện mới (View Transitions API) trong CSS để tạo ra hiệu ứng chuyển trang vô cùng mượt mà cho các ứng dụng nhiều trang (MPA) tương tự như trải nghiệm của ứng dụng một trang (SPA).

4、[Cảnh báo nguy cơ bảo mật từ việc tự động tải tệp tin .env của Cursor](https://forum.cursor.com/t/env-file-question/60165) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031206.webp)

Cộng đồng người dùng trình soạn thảo mã nguồn Cursor đang chia sẻ rộng rãi cảnh báo sau khi phát hiện phần mềm có cơ chế tự động đồng bộ tải tệp tin `.env` (nơi lưu trữ các khóa bảo mật và cấu hình môi trường nhạy cảm của dự án) lên máy chủ đám mây, tiềm ẩn nhiều nguy cơ rò rỉ thông tin nghiêm trọng cho doanh nghiệp.

5、[Phân tích quy tắc sắp xếp thứ tự thuộc tính trong JSON và JavaScript](https://blog.gslin.org/archives/2025/03/07/12299/json-%E8%88%87-javascript-%E5%86%8D-object-%E8%A3%A1%E9%9D%A2%E5%85%83%E7%B4%A0%E9%A0%86%E5%BA%8F%E7%9A%84%E5%B7%AE%E7%95%B0/) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030702.webp)

Liệu cấu trúc dữ liệu JSON và đối tượng Object trong JavaScript có quy định cụ thể về thứ tự xuất hiện của các thuộc tính thành phần bên trong hay không? Bài viết phân tích chi tiết các quy chuẩn kỹ thuật quy định vấn đề này.

6、[Đánh giá những ưu điểm vượt trội của cơ chế xử lý lỗi trong ngôn ngữ Go](https://rauljordan.com/why-go-error-handling-is-awesome/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031102.webp)

Ngôn ngữ Go sở hữu cơ chế xử lý ngoại lệ vô cùng đặc thù khi hoàn toàn không ứng dụng cấu trúc `try...catch` truyền thống mà coi lỗi hiển thị như một giá trị trả về thông thường. Tác giả phân tích những giá trị thiết thực và sự mạch lạc trong tư duy lập trình do cơ chế này mang lại.

## 工具

1、[TypeScript 7 (Trình biên dịch tsc viết bằng Go)](https://github.com/microsoft/typescript-go)

Tập đoàn Microsoft công bố dự án tái cấu trúc toàn bộ trình biên dịch TypeScript (tsc) bằng ngôn ngữ Go, hứa hẹn mang lại tốc độ biên dịch mã nguồn nhanh gấp 10 lần so với phiên bản cũ. Tham khảo thêm bài viết [giới thiệu chi tiết từ hãng](https://devblogs.microsoft.com/typescript/typescript-native-port/).

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031207.webp)

Phiên bản TypeScript hiện tại đang ở mốc 5.8. Ngay sau khi trình biên dịch viết bằng Go đạt độ ổn định cao, dự án sẽ chính thức được phát hành ra thị trường dưới phiên bản TypeScript 7.

2、[QR Code Generator](https://fietkau.software/qr)

Ứng dụng web trực quan hỗ trợ người dùng tự do thiết kế và tùy biến các hoa văn trang trí, màu sắc hiển thị và chèn logo cá nhân vào mã QR.

3、[WatchYourLAN](https://github.com/aceberg/WatchYourLAN)

Dự án phần mềm mã nguồn mở hỗ trợ quản trị viên mạng nhanh chóng quét và lập bản đồ phân bổ địa chỉ IP trong mạng cục bộ (LAN), tự động gửi cảnh báo qua ứng dụng nhắn tin ngay khi phát hiện có thiết bị lạ kết nối hoặc ngắt kết nối.

4、[XPipe](https://github.com/xpipe-io/xpipe)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031305.webp)

Ứng dụng máy tính đa nền tảng cung cấp giao diện đồ họa quản trị trực quan hỗ trợ quản lý tập trung toàn bộ các kết nối máy chủ từ xa của doanh nghiệp tại một nơi duy nhất.

5、[TransBridge](https://github.com/fruitbars/transbridge)

Dự án mã nguồn mở xây dựng cổng trung gian kết nối (API Gateway) chuyên dụng cho dịch vụ dịch thuật, hỗ trợ kết nối đồng thời với nhiều dòng mô hình ngôn ngữ lớn khác nhau để cung cấp dịch vụ dịch thuật tối ưu. Trải nghiệm [trang chạy thử Demo](https://transbridge.fanyimao.cn/). (Đóng góp từ [@fruitbars](https://github.com/ruanyf/weekly/issues/6238))

6、[DouYin Downloader](https://github.com/jiji262/douyin-downloader)

Bộ kịch bản Python mã nguồn mở hỗ trợ người dùng tự động tải các video ngắn từ nền tảng Douyin về máy tính một cách nhanh chóng. (Đóng góp từ [@jiji262](https://github.com/ruanyf/weekly/issues/6240))

7、[Java Thread Dump Analyzer](https://www.threadanalyzer.online/)

Dịch vụ web miễn phí hỗ trợ nhà phát triển Java phân tích nhanh các tệp tin kết xuất trạng thái luồng (thread dump) sinh ra từ công cụ jstack để nhanh chóng chẩn đoán các sự cố nghẽn luồng của ứng dụng. (Đóng góp từ [@HbOrea](https://github.com/ruanyf/weekly/issues/6259))

8、[Mono](https://mono.cards/zh)

Dịch vụ trực tuyến miễn phí hỗ trợ người dùng nhanh chóng thiết kế và tạo các bức ảnh poster chia sẻ trích dẫn đẹp mắt. (Đóng góp từ [@RiverTwilight](https://github.com/ruanyf/weekly/issues/6264))

9、[Telegram Files](https://github.com/jarvis2f/telegram-files)

Dự án mã nguồn mở hỗ trợ tải hàng loạt tệp tin từ nhiều kênh chia sẻ và tài khoản Telegram khác nhau về máy tính một cách tự động. (Đóng góp từ [@jarvis2f](https://github.com/ruanyf/weekly/issues/6268))

10、[Obsidian Cloud Sync Plugin](https://github.com/ai-bytedance/obsidian-cloud-sync)

Tiện ích mở rộng mã nguồn mở dành cho ứng dụng ghi chú Obsidian hỗ trợ tự động đồng bộ hóa toàn bộ kho ghi chú cá nhân lên nhiều dịch vụ lưu trữ đám mây phổ biến. (Đóng góp từ [@ai-bytedance](https://github.com/ruanyf/weekly/issues/6275))

## AI 相关

1、[Mistral OCR](https://mistral.ai/news/mistral-ocr)

Hãng phát triển AI Mistral AI vừa giới thiệu công cụ nhận diện chữ viết hình ảnh OCR được đánh giá là mạnh nhất hiện nay trên thế giới, sở hữu năng lực nhận diện và trích xuất cực tốt các cấu trúc phức tạp như công thức toán học và các bảng dữ liệu. Xem thêm [bài viết giới thiệu chi tiết](https://finance.sina.com.cn/tech/roll/2025-03-07/doc-inenuzhm5927298.shtml).

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031306.webp)

Độc giả [@monsoonw](https://github.com/ruanyf/weekly/issues/6248) đã tự xây dựng một trang web hỗ trợ trải nghiệm nhanh tính năng này hoàn toàn miễn phí tại địa chỉ [mistralocr.net](https://mistralocr.net/).

Lập trình viên nổi tiếng Simon Willison cũng chia sẻ công khai [bản kịch bản Python](https://github.com/simonw/tools/blob/main/python/mistral_ocr.py) minh họa chi tiết cách thức gọi cổng kết nối API Mistral OCR trong lập trình thực tế.

2、[Free QWQ](https://qwq.aigpu.cn/)

Nền tảng điện toán đám mây miễn phí cung cấp quyền truy cập API không giới hạn vào dòng mô hình lớn chuyên về lập trình toán học QwQ 32B của hãng Qwen dành cho cộng đồng phát triển. (Đóng góp từ [@nexmoe](https://github.com/ruanyf/weekly/issues/6260))

3、[Code-Review-LLM-Gitlab](https://github.com/mimo-x/Code-Review-GPT-Gitlab)

Công cụ hỗ trợ tự động kết nối mô hình ngôn ngữ lớn để tiến hành đánh giá, rà soát lỗi mã nguồn (Code Review) cho các dự án lập trình lưu trữ trên nền tảng GitLab. (Đóng góp từ [@mimo-x](https://github.com/ruanyf/weekly/issues/6261))

4、[Nhân Thoại Phiên Dịch Khí (人话翻译器)](https://github.com/DemoJ/HumanizeText)

Tiện ích mở rộng trình duyệt Chrome ứng dụng AI hỗ trợ chuyển đổi các đoạn văn bản tiếng Trung học thuật hoặc kỹ thuật phức tạp khó hiểu thành các câu văn giản dị dễ hiểu hơn cho người đọc. (Đóng góp từ [@DemoJ](https://github.com/ruanyf/weekly/issues/6277))

## 资源

1、[Thần Vũ Lạc Nhạn Thể (辰宇落雁体)](https://github.com/Chenyu-otf/chenyuluoyan_thin)

Dự án cung cấp bộ phông chữ viết tay tiếng Trung mã nguồn mở và miễn phí vô cùng nét nghệ thuật.

2、[JetBrains Maple Mono](https://github.com/SpaceTimee/Fusion-JetBrainsMapleMono)

Dự án thiết kế bộ phông chữ lập trình kết hợp: Giải quyết triệt để vấn đề thiếu hụt phông chữ tiếng Trung mặc định của phông chữ nổi tiếng JetBrains Mono, bảo đảm hiển thị các ký tự tiếng Trung và tiếng Anh theo tỷ lệ chiều rộng chuẩn xác 2:1 đồng đều. (Đóng góp từ [@SpaceTimee](https://github.com/ruanyf/weekly/issues/6244))

3、[BeddyStories](https://beddystories.com/zh)

Trang web tổng hợp và chia sẻ kho tàng các câu chuyện cổ tích và truyện kể trước giờ đi ngủ kinh điển dành cho trẻ em trên toàn thế giới hỗ trợ đa ngôn ngữ. (Đóng góp từ [@yimiqidage](https://github.com/ruanyf/weekly/issues/6272))

4、[IP Thám Tử (IP 侦探)](https://ip.aolifu.org/)

Dịch vụ trực tuyến miễn phí hỗ trợ người dùng nhanh chóng truy vấn và kiểm tra thông tin nhà mạng và vị trí địa lý của địa chỉ IP. (Đóng góp từ [@Oliverwqcwrw](https://github.com/ruanyf/weekly/issues/6271))

Tiện ích mở rộng Chrome tương tự **IP Location Finder** hỗ trợ quét và hiển thị nhanh vị trí địa lý của bất kỳ địa chỉ IP nào được bôi đen trên trang web. (Đóng góp từ [@Yanel85](https://github.com/ruanyf/weekly/issues/6278))

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031301.webp)

## 图片

1、[Mô phỏng hình ảnh hiển thị dưới mắt người mắc hội chứng mù màu đỏ - xanh lá](https://www.theverge.com/23650428/colorblindness-design-ui-accessibility-wordle)

Người mắc chứng mù màu đỏ - xanh lá hoàn toàn không có khả năng phân biệt hai sắc màu này. Trong mắt của họ, cả hai màu sắc này đều hiển thị dưới dạng sắc tố màu vàng.

Bức ảnh phía dưới chụp chiếc lá với một nửa màu đỏ và một nửa màu xanh lá thông thường:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040802.webp)

Và đây là hình ảnh tương đương hiển thị dưới góc nhìn của một bệnh nhân mù màu đỏ - xanh lá:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040803.webp)

Thống kê cho thấy tỷ lệ người mắc chứng mù màu hoặc suy giảm thị lực màu sắc chiếm tới khoảng 5% dân số (trung bình cứ 20 người lại có 1 người gặp vấn đề này). Do đó, khi thiết kế giao diện người dùng, việc lạm dụng phối màu đỏ và xanh lá để biểu thị các thông tin đối lập là một giải pháp thiết kế rất thiếu thân thiện.

Bức ảnh dưới đây là một giao diện lịch làm việc ứng dụng màu xanh lá và màu hồng để phân biệt các sự kiện đặc biệt:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040804.webp)

Và đây là giao diện tương đương hiển thị dưới mắt người mù màu, hoàn toàn không thể phân biệt được các ngày đặc biệt:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040805.webp)

Do đó, các nhà thiết kế giao diện nên hết sức hạn chế việc sử dụng màu đỏ và xanh lá làm yếu tố nhận diện thông tin duy nhất cho sản phẩm.

## 文摘

1、[Kịch bản cuộc sống của nhân loại khi AI và hệ thống robot đảm nhận toàn bộ công việc](https://hyponymo.us/2013/01/29/100-percent-unemployment/)

Gần đây tôi thường xuyên suy ngẫm về một câu hỏi: Nếu công nghệ AI phát triển vượt bậc và vượt trội hơn con người ở mọi lĩnh vực, kết hợp cùng hệ thống robot tự động đảm nhận toàn bộ các tác vụ sản xuất xã hội, khi đó nhân loại sẽ làm gì để tìm kiếm ý nghĩa cuộc sống?

Nhà tương lai học Kevin Kelly đưa ra quan điểm lạc quan rằng khi các công việc tay chân nhọc nhằn được giao phó cho máy móc, con người sẽ được tự do để dấn thân vào các công việc sáng tạo thú vị hơn, tương tự như những gì đã xảy ra sau cuộc cách mạng công nghiệp trước đây.

Quan điểm này có vẻ hợp lý trong ngắn hạn, nhưng nó dựa trên một giả định cốt lõi: Con người luôn sở hữu những năng lực đặc thù mà máy tính không bao giờ có thể bắt chước được.

Tuy nhiên dưới góc nhìn cá nhân, tôi thấy hoàn toàn không có cơ sở khoa học nào bảo đảm giả định này sẽ tồn tại vĩnh viễn.

Ngoại trừ kịch bản chính phủ ban hành các sắc lệnh hành chính cấm đoán máy tính tham gia vào một số lĩnh vực dịch vụ đặc thù để bảo vệ việc làm cho con người. Nhưng nếu làm như vậy, các ngành công nghiệp đó nhiều khả năng sẽ rơi vào trạng thái trì trệ công nghệ. Một ngành công nghiệp trì trệ sẽ không còn sức hút phát triển, thu nhập của nhân sự không thể gia tăng và bản thân những người làm việc tại đó cũng khó tìm kiếm được sự thỏa mãn trong công việc.

Chúng ta hãy cùng giả định một kịch bản cực đoan: Khi máy móc vượt trội hơn con người ở mọi khía cạnh và phần lớn người dân trong xã hội hoàn toàn không còn khả năng đóng góp giá trị lao động cho nền kinh tế, khi đó thế giới sẽ ra sao?

Khi một cá nhân hoàn toàn mất đi khả năng đóng góp giá trị cho xã hội, giá trị kinh tế của người đó thực chất sẽ tiệm cận về số 0. Ngay cả khi họ vẫn được bảo đảm quyền sinh tồn cơ bản nhờ các khoản trợ cấp xã hội từ chính phủ, ý nghĩa cuộc sống đối với họ khi đó sẽ là gì? Đơn thuần chỉ là việc tồn tại qua ngày một cách vô nghĩa?

Ở thời điểm hiện tại, câu hỏi này có vẻ vẫn còn tương đối xa vời và kịch bản đó nếu xảy ra cũng cần một thời gian rất dài sắp tới. Vấn đề thực tế và cấp bách hơn trước mắt là sự xuất hiện của AI đang làm sụt giảm nhanh chóng số lượng các công việc văn phòng có mức thu nhập cao. Khi năng lực của máy tính ngày một mạnh mẽ, giá trị của các công việc bàn giấy truyền thống đang bị thu hẹp một cách nhanh chóng, khiến đại bộ phận người lao động ngày càng khó tìm kiếm được một công việc có mức thu nhập tốt và mang lại sự thỏa mãn cá nhân.

Đây chính là cuộc khủng hoảng thực tế đang diễn ra ngay trước mắt chúng ta hằng ngày: Số lượng các vị trí công việc chất lượng cao ngày càng thu hẹp và trở nên khó tiếp cận hơn đối với số đông.

## 言论

1、

Trước đây, những chiếc vé xem ca nhạc, vé xem phim, vé tàu hay vé tham quan du lịch luôn được in dưới dạng giấy vật lý để người dùng giữ lại làm kỷ niệm. Đến nay, toàn bộ chúng đã bị dịch chuyển hoàn toàn sang định dạng kỹ thuật số hiển thị trên màn hình điện thoại.

Toàn bộ ký ức cuộc sống của chúng ta hiện nay chỉ được lưu giữ dưới dạng các pixel trên điện thoại và chúng ta không còn sở hữu các vật chứng kỷ niệm thực tế nào nữa.

-- *Trích bài phân tích đăng tải trên Bloomberg*

2、

Khi hầu hết các ứng dụng phần mềm đều có xu hướng chuyển dịch lên môi trường web trực tuyến, sự khác biệt về mặt tính năng giữa các hệ điều hành máy tính sẽ ngày một giảm đi. Đây chính là lý do tại sao sự ra đời của dòng chip xử lý M1 lại đóng vai trò quyết định đối với tương lai phát triển của máy tính Mac.

Apple cần nhanh chóng tận dụng làn sóng AI hiện nay để phát huy tối đa ưu thế phần cứng chip xử lý của mình, khuyến khích cộng đồng lập trình viên ưu tiên phát triển các giải pháp chạy các mô hình AI trực tiếp trên phần cứng máy vật lý (local run).

-- *Trích bài phân tích 《Tiềm năng chuyển dịch nền tảng AI của Apple》* (Bài viết chỉ ra rằng chip xử lý của Apple hoàn toàn đủ năng lực chạy cục bộ các mô hình lớn mà không bắt buộc phải trang bị card đồ họa chuyên dụng của Nvidia, và Apple nên tận dụng điểm này để gia tăng doanh số bán hàng)

3、

Kể từ khi có sự hỗ trợ của các công cụ AI, tôi nhận thấy bản thân mình không còn cảm giác lo lắng hay e ngại trước những dự án lập trình có quy mô lớn hoặc đòi hỏi khai thác những ngôn ngữ, công nghệ lập trình mới mà bản thân chưa từng tiếp xúc. Mọi rào cản kỹ thuật đều trở nên dễ dàng giải quyết hơn nhiều.

Tôi đang bắt đầu khởi động lại hàng loạt ý tưởng dự án cá nhân từng bị xếp xó trước đây do tự đánh giá nó quá phức tạp hoặc vượt quá giới hạn năng lực lập trình của mình để tự mình thử nghiệm thực thi khi có thời gian rảnh. Chúng ta đang thực sự sống trong một kỷ nguyên công nghệ vô cùng thú vị.

-- *Trích bài chia sẻ 《Thời đại của AI yêu cầu bạn phải suy nghĩ lớn hơn》*

4、

Tôi nhận định rằng toán học hiện đại thực tế đã không còn tồn tại nhiều bài toán mở thực sự có giá trị lớn nữa. Số lượng các chủ đề nghiên cứu lớn có khả năng thu hút sự quan tâm của giới toán học toàn cầu đang giảm dần qua từng năm và hiện tại hầu như không còn lại bao nhiêu.

Hoạt động nghiên cứu toán học ngày nay đang dần bị thu hẹp vào các chủ đề vô cùng nhỏ nhặt và chuyên biệt của một nhóm nhỏ các học giả. Ngay cả các học viên sau đại học cũng thường xuyên gặp khủng hoảng trước tính chất chuyên biệt hóa cực đoan và sự trừu tượng hóa quá mức của các đề tài nghiên cứu hiện nay.

Thế hệ nghiên cứu sinh tương lai nhiều khả năng sẽ không còn cần thiết phải nỗ lực tìm kiếm và chứng minh các định lý hoàn toàn mới nữa. Thay vào đó, nhiệm vụ cốt lõi của họ sẽ là tìm cách đơn giản hóa và hệ thống hóa lại các kết quả nghiên cứu đồ sộ của thế hệ đi trước.

-- *Trích bài phân tích 《Ngành toán học đang dần cạn kiệt các bài toán nghiên cứu》*

## 往年回顾

- Số #294: [Chiêm nghiệm lịch sử từ sự kiện trận hải chiến Nhai Môn](https://www.ruanyifeng.com/blog/2024/03/weekly-issue-294.html)
- Số #244: [Thảo luận về luận điểm: Ngành công nghiệp Dữ liệu lớn (Big Data) thực tế đã kết thúc](https://www.ruanyifeng.com/blog/2023/03/weekly-issue-244.html)
- Số #194: [Chiêm nghiệm cuộc sống: Người bi quan thường có xu hướng nhận định đúng, nhưng người lạc quan mới là người đi đến thành công](https://www.ruanyifeng.com/blog/2022/02/weekly-issue-194.html)
- Số #144: [Phân tích về giải pháp cốt lõi và duy nhất giúp gia tăng mức thu nhập thực tế của cá nhân](https://www.ruanyifeng.com/blog/2021/01/weekly-issue-144.html)

(Hết)
