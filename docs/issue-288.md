# Bản tin chia sẻ công nghệ (Số 288): Bí quyết hàng đầu của viết tài liệu kỹ thuật

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3814) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011602.webp)

Tại Cung điện Mùa hè (Di Hòa Viên) ở Bắc Kinh, hồ Côn Minh đã đóng băng hoàn toàn và trở thành sân trượt băng tự nhiên thu hút đông đảo du khách. Khi hoàng hôn buông xuống, cầu 17 nhịp hiện lên hiện tượng quang học kỳ thú "Ánh vàng xuyên qua lỗ cầu" (Kim quang xuyên động). (Nguồn: [66wz](https://news.66wz.com/system/2024/01/15/105618610.shtml))

## 技术写作的首要诀窍

Viết tài liệu kỹ thuật (technical writing) đóng vai trò vô cùng quan trọng trong việc phát triển, quảng bá và bảo trì sản phẩm công nghệ.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012307.webp)

Khác với suy nghĩ của nhiều người, **chất lượng của một bài viết kỹ thuật ít phụ thuộc vào trình độ văn chương, mà cốt lõi nằm ở phương pháp và kỹ năng trình bày**.

Bởi vì tiêu chuẩn đánh giá của viết tài liệu kỹ thuật không nằm ở tính nghệ thuật, mà nằm ở chỗ thông tin truyền tải có rõ ràng và dễ hiểu hay không. Nó không cần những từ ngữ hoa mỹ, những phép so sánh ẩn dụ phức tạp hay những cảm nhận sâu sắc, mà chỉ cần mô tả chính xác vấn đề cần giải quyết.

**Chìa khóa để mô tả rõ ràng vấn đề nằm ở chỗ tư duy của bạn có mạch lạc hay không.**

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012308.webp)

Một khi đã hiểu sâu sắc vấn đề, chỉ cần nắm vững một vài nguyên tắc cốt lõi, bạn hoàn toàn có thể viết nên một tài liệu kỹ thuật xuất sắc.

Hôm nay, tôi xin chia sẻ bí quyết hàng đầu trong viết tài liệu kỹ thuật. Quy tắc rất đơn giản, gói gọn trong một câu: **Bài viết cần áp dụng cấu trúc tuyến tính đơn (Single-line structure)**.

Khái niệm "cấu trúc tuyến tính đơn" (còn gọi là cấu trúc một con đường) nghĩa là bài viết chỉ tập trung giải quyết duy nhất một vấn đề, và dẫn dắt thông tin theo một trình tự tuyến tính tuần tự: từ nông đến sâu, từ đơn giản đến phức tạp, trình bày mạch lạc và từng bước tiến tới.

Phương pháp này tương tự như sơ đồ tham quan của một khu du lịch: chỉ thiết kế duy nhất một lối đi từ cổng vào đến cổng ra. Khách tham quan chỉ cần đi theo biển chỉ dẫn mũi tên dọc đường là có thể chiêm ngưỡng đầy đủ các cảnh quan mà không bị nhầm lẫn.

If đồng thời có nhiều tuyến đường, du khách chắc chắn sẽ bối rối: không biết nên đi lối nào, hay lo lắng liệu mình có bỏ lỡ cảnh đẹp nào không. Tệ hơn nữa, các lối đi đan chéo sẽ khiến dòng người hỗn loạn và dễ bị lạc đường.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012309.webp)

*(Chú thích ảnh: Nhìn vào sơ đồ tuyến đường của khu du lịch trên, liệu bạn có dễ dàng chọn được lối đi phù hợp?)*

Chỉ cần tuân thủ cấu trúc tuyến tính đơn này, tài liệu kỹ thuật của bạn chắc chắn sẽ đạt yêu cầu cơ bản. Dù nội dung có phức tạp hay khó hiểu đến đâu, ít nhất cấu trúc bài viết vẫn rõ ràng mạch lạc, các luận điểm kết nối chặt chẽ giúp người đọc dễ dàng định vị điểm họ gặp khó khăn. Chỉ cần vượt qua điểm nghẽn đó, họ có thể tiếp tục tự tin đọc tiếp mà không lo bị rơi vào mê cung thông tin không lối thoát.

Có [một bài viết tiếng Anh](https://thisisimportant.net/posts/content-as-a-graph/) minh họa cấu trúc bài viết bằng các sơ đồ trực quan rất sinh động.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012310.webp)

Sơ đồ trên minh họa cấu trúc tuyến tính đơn, phát triển tuần tự từng bước theo chiều mũi tên chỉ dẫn.

Đối với những bài toán phức tạp liên quan đến nhiều yếu tố tương tác, cấu trúc thông tin có thể phát triển theo dạng hình sao (star structure).

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012311.webp)

Hoặc phát triển theo cấu trúc phân tầng (hierarchical structure).

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012312.webp)

Trong các trường hợp này, lời khuyên là bạn nên chủ động chia nhỏ bài viết thành chuỗi nhiều bài viết ngắn độc lập. Mỗi bài viết nhỏ chỉ tập trung phân tích sâu một khía cạnh duy nhất theo cấu trúc tuyến tính đơn để đảm bảo thông tin được truyền tải trọn vẹn nhất.

Mặc dù nguyên tắc cấu trúc tuyến tính đơn nghe qua có vẻ đơn giản, nhưng việc thực hiện lại không hề dễ dàng. Khó khăn lớn nhất nằm ở chỗ tư duy tự nhiên của con người thường mang tính đa luồng, phi tuyến tính và dễ nhảy cóc.

Để chuyển đổi những suy nghĩ hỗn độn và nhảy cóc đó thành một cấu trúc tuyến tính mạch lạc giúp người khác dễ dàng tiếp thu đòi hỏi người viết phải đầu tư nhiều thời gian để liên tục gọt giũa và cô đọng luận điểm.

Ví dụ, luồng suy nghĩ tự nhiên của chúng ta thường giống như sơ đồ dưới đây, với nhiều điểm thông tin phát tán kết nối chằng chịt.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012313.webp)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012314.webp)

Tư duy hỗn độn ban đầu không phải là điều đáng ngại, điều đáng sợ là bạn mang nguyên cấu trúc rối rắm đó vào bài viết kỹ thuật mà không chịu kiên nhẫn bóc tách và sắp xếp chúng thành một con đường mạch lạc.

## 科技动态

1、[Robot nhân hình vận hành trong kho hàng của Amazon](https://www.businessinsider.com/new-amazon-warehouse-robot-humanoid-2023-10)

Tập đoàn Amazon mới đây đã bắt đầu thử nghiệm vận hành dòng robot nhân hình tại các kho hàng của mình.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120804.webp)

Dài dòng robot này được thiết kế để thực hiện các tác vụ phân loại và vận chuyển hàng hóa, với chi phí vận hành ước tính khoảng 10 đến 12 USD mỗi giờ. Khi được đưa vào sản xuất và ứng dụng quy mô lớn, chi phí vận hành kỳ vọng có thể giảm xuống mức 2 đến 3 USD mỗi giờ.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120805.webp)

Robot làm việc phối hợp trực tiếp cùng các nhân viên kho (hình dưới). Nhiều công nhân bày tỏ lo ngại về việc robot sẽ sớm thay thế vị trí công việc của họ trong tương lai. Phía Amazon khẳng định dòng robot này được thiết kế với mục đích hỗ trợ công việc và giảm tải cường độ lao động cho con người chứ không nhằm mục đích thay thế.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120806.webp)

Tuy nhiên, việc phải làm việc cạnh một robot có năng suất cao không cần nghỉ ngơi và không đòi hỏi lương thưởng chắc chắn sẽ tạo áp lực tâm lý không nhỏ cho bất kỳ nhân viên nào.

2、[Giải pháp quét mã vạch mini để nghiên cứu hành vi đàn ong](https://theapiarist.org/barcoding-bees/)

Trong các dự án nghiên cứu sinh học, các nhà khoa học cần theo dõi chính xác hành vi của từng cá thể ong. Làm thế nào để phân biệt chính xác từng con ong trong một đàn ong hàng ngàn con giống hệt nhau?

Các nhà nghiên cứu đã đưa ra giải pháp độc đáo: dán một nhãn mã QR siêu nhỏ lên lưng mỗi con ong.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011901.webp)

Diện tích của mỗi nhãn mã QR này chỉ vỏn vẹn 2,1 mm² (chiều dài cạnh chưa đầy 1,5 mm), với trọng lượng siêu nhẹ 0,6 mg (tương đương 0,7% trọng lượng cơ thể ong thợ), dải mã hóa hỗ trợ phân biệt tối đa 2048 cá thể ong khác nhau.

Các nhà khoa học đã thực hiện dán thủ công nhãn mã QR này lên tổng cộng 1400 con ong thợ. Thông qua hệ thống camera tốc độ cao, các mã QR này sẽ được nhận diện tự động để phân tích hành vi của từng cá thể.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011902.webp)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011903.webp)

Bằng cách phân tích hình ảnh phóng đại từ tổ ong nơi hàng ngàn con ong di chuyển liên tục, hệ thống máy tính có thể vẽ nên sơ đồ di chuyển của từng con ong thợ (hình dưới), từ đó phân tích các hoạt động tương tác và cộng tác của chúng.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011904.webp)

3、[Thiết bị chuột điều khiển bằng lưỡi độc đáo](https://www.nbcnews.com/tech/tech-news/tongue-controlled-touchscreens-hit-market-year-rcna133270)

Tại Triển lãm Điện tử Tiêu dùng CES tổ chức tại Las Vegas năm nay, một doanh nghiệp đã giới thiệu thiết bị điều khiển độc đáo mang tên "chuột lưỡi".

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011905.webp)

Thiết bị có cấu trúc giống như một khay niềng răng tích hợp bàn di chuột mini áp vào vòm họng trên. Người dùng hoàn toàn không cần dùng tay mà chỉ cần dùng đầu lưỡi di chuyển trên khay để điều khiển con trỏ chuột trên màn hình.

Mục tiêu thiết kế ban đầu của thiết bị nhằm hỗ trợ những người bị chấn thương tay hoặc bại liệt có thể dễ dàng sử dụng máy tính. Tuy nhiên, nhà sản xuất phát hiện thiết bị cũng nhận được sự quan tâm lớn từ nhóm người dùng thông thường như các kỹ sư cơ khí hay bác sĩ phẫu thuật - những người muốn điều khiển máy tính trong khi hai tay đang bận thao tác công việc khác.

4、[Hộp nhựa bảo vệ chống trộm hàng hóa tại các siêu thị](https://www.curbed.com/2023/01/shoplifting-crime-wave-spam-keeper-retail-loss-prevention-design.html)

Các cửa hàng bán lẻ và siêu thị quy mô nhỏ tại Âu Mỹ đang ngày càng áp dụng rộng rãi giải pháp khóa bảo vệ hàng hóa trong các hộp nhựa chống trộm.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011702.webp)

Các hộp nhựa trong suốt này được thiết kế khóa bảo vệ chắc chắn. Khách mua hàng không thể tự ý lấy sản phẩm ra mà phải nhờ nhân viên siêu thị dùng khóa chuyên dụng để mở.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011703.webp)

Hộp nhựa cũng được tích hợp chip RFID cảm biến, hệ thống còi báo động ở cửa ra vào sẽ tự động kích hoạt nếu hộp hàng bị mang ra ngoài bất hợp pháp. Giải pháp này giúp giảm thiểu đáng kể tình trạng mất cắp và thất thoát hàng hóa tại các cửa hàng.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011704.webp)

## Bài viết

1\. [Tìm hiểu giải pháp kỹ thuật đếm ngược đèn giao thông trên bản đồ AutoNavi](https://mp.weixin.qq.com/s/3_LNM62zoHaJsmvAryujEw)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012401.webp)

Ứng dụng bản đồ AutoNavi (Gaode Maps) hỗ trợ tính năng hiển thị thời gian đếm ngược của đèn giao thông theo thời gian thực. Bài viết phân tích các sáng chế và công nghệ phía sau tính năng này.

2\. [Tổng hợp xu hướng và nhận định công nghệ Frontend năm 2023](https://mp.weixin.qq.com/s/LiygBJqMN8U_vSpAjxMibQ)（Tiếng Trung）

Báo cáo công nghệ chi tiết do nhóm phát triển Tencent Cloud phối hợp cùng đội ngũ Frontend Tencent MoonWebTeam xây dựng. (Đóng góp của [@ryantang1991](https://github.com/ruanyf/weekly/issues/3917))

3\. [Phân tích cơ chế hoạt động của phương thức every() trên mảng rỗng trong JavaScript](https://humanwhocodes.com/blog/2023/09/javascript-wtf-why-does-every-return-true-for-empty-array/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120209.webp)

Tìm hiểu nguyên nhân giải thích vì sao phương thức `every()` trong JavaScript luôn trả về giá trị `true` khi thực thi trên một mảng rỗng.

4\. [Giới thiệu 8 phần mềm quản lý mật khẩu mã nguồn mở uy tín](https://itsfoss.com/open-source-password-managers/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120205.webp)

Phần mềm quản lý mật khẩu là công cụ đắc lực giúp bảo mật thông tin tài khoản cá nhân. Bài viết giới thiệu 8 giải pháp mã nguồn mở an toàn được cộng đồng tin dùng.

5\. [Tổng hợp các kỹ thuật tạo hiệu ứng chuyển động CSS ấn tượng](https://codersblock.com/blog/the-surprising-things-that-css-can-animate/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120513.webp)

Bài viết chia sẻ các mẹo và kỹ thuật nâng cao giúp lập trình viên tối ưu hóa hiệu ứng chuyển động (animations) bằng CSS.

6\. [Tìm hiểu chi tiết về cấu trúc và nguyên lý hoạt động của giao thức HTTP/3](https://www.smashingmagazine.com/2021/08/http3-core-concepts-part1/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091202.webp)

Chuỗi bài viết giới thiệu một cách hệ thống cho người mới bắt đầu về kiến trúc thiết kế của giao thức HTTP/3 và so sánh các điểm cải tiến cốt lõi so với thế hệ HTTP/2 tiền nhiệm.

7、[Minh họa chi tiết quy trình sản xuất bộ vi xử lý CPU từ cát thạch anh](https://blog.robertelder.org/how-to-make-a-cpu/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102301.webp)

Tác giả sử dụng hệ thống hình ảnh minh họa chi tiết để giải thích một cách trực quan quy trình sản xuất chip xử lý CPU từ nguyên liệu cát đá trong tự nhiên. Bài viết giúp người đọc nhanh chóng nắm bắt các công đoạn chế tạo bán dẫn phức tạp.

## 工具

1\. [Gemini Pro Chat](https://github.com/lchh5/GeminiPro-Next-Web)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012005.webp)

Tác giả đã tiến hành tùy biến mã nguồn dự án ChatGPT Next Web để hỗ trợ gọi các API của Gemini Pro. Bạn đọc có thể trải nghiệm bản [Demo tại đây](https://chat.googlegemini.co/). (Đóng góp của [@lchh5](https://github.com/ruanyf/weekly/issues/3923))

2\. [WoodenFish (Mộc Ngư Online)](https://github.com/jwenjian/wooden-fish)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012006.webp)

Ứng dụng web giải trí gõ mộc ngư: khi mở trên thiết bị di động, hệ thống tận dụng cảm biến con quay hồi chuyển (gyroscope) để phát hiện chuyển động lắc của điện thoại như hành động gõ mộc ngư thực tế để tính điểm. (Đóng góp của [@jwenjian](https://github.com/ruanyf/weekly/issues/3929))

3\. [Moodist (Hệ thống tạo tiếng ồn nền)](https://github.com/geekyouth/moodist)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012301.webp)

Dự án Docker hỗ trợ triển khai nhanh trang web tạo tiếng ồn nền với hơn 50 tùy chọn âm thanh tự nhiên (tiếng mưa, tiếng gió, âm thanh quán cafe...). Xem bản trải nghiệm [Demo tại đây](https://moodist.java666.cn/). (Đóng góp của [@geekyouth](https://github.com/ruanyf/weekly/issues/3943))

4\. [Echo UI](https://echoui.dev/zh/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012302.webp)

Bộ thư viện thành phần giao diện (UI library) được thiết kế chuyên biệt cho Web Audio API, giúp lập trình viên nhanh chóng xây dựng các ứng dụng xử lý âm thanh trên web. (Đóng góp của [@codeacme17](https://github.com/ruanyf/weekly/issues/3946))

5\. [Photor](https://www.photor.fun/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012303.webp)

Công cụ hỗ trợ làm đẹp ảnh chụp màn hình trực tuyến, tương thích tốt cả dạng ứng dụng web độc lập lẫn tiện ích mở rộng trên trình duyệt. (Đóng góp của [@sleepy-zone](https://github.com/ruanyf/weekly/issues/3948))

6\. [Message Nest](https://github.com/engigu/Message-Push-Nest)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012304.webp)

Nền tảng quản lý và đẩy thông báo mã nguồn mở, hỗ trợ tích hợp đa dạng các kênh truyền thông như Email, DingTalk, WeChat Enterprise... (Đóng góp của [@engigu](https://github.com/ruanyf/weekly/issues/3947))

7\. [Tiny RDM](https://redis.tinycraft.cc/zh/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012306.webp)

Phần mềm quản trị cơ sở dữ liệu Redis giao diện trực quan, tương thích tốt trên các nền tảng macOS, Windows và Linux. (Đóng góp của [@tiny-craft](https://github.com/ruanyf/weekly/issues/3955))

8\. [Frigate](https://github.com/blakeblackshear/frigate)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111906.webp)

Giải pháp quản lý camera an ninh mã nguồn mở tích hợp thuật toán nhận diện vật thể thời gian thực.

9\. [InstantID](https://github.com/InstantID/InstantID)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012402.webp)

Mô hình AI hỗ trợ trích xuất đặc trưng khuôn mặt chỉ từ một bức ảnh mẫu để ghép nối logic vào các phong cách ảnh vẽ nghệ thuật khác nhau. Trải nghiệm bản dùng thử [Demo tại đây](https://instantid.org/#playground). (Đóng góp của [@zinc1234596](https://github.com/ruanyf/weekly/issues/3959))

10\. [HandBrake](https://handbrake.fr/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111910.webp)

Phần mềm mã nguồn mở đa nền tảng hỗ trợ chuyển đổi định dạng và mã hóa mã nguồn video chuyên nghiệp.

11\. [Animotion](https://cssanimotion.pages.dev/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111911.webp)

Công cụ trực tuyến giúp thiết kế và tạo các hiệu ứng chuyển động CSS trực quan đi kèm tính năng xuất mã nguồn tự động.

12\. [Ada](https://github.com/ada-url/ada)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112102.webp)

Thư viện phân tích cú pháp địa chỉ URL hiệu năng cao viết bằng C++, tuân thủ các đặc tả kỹ thuật tiêu chuẩn mới nhất.

13\. [Inpaint-web](https://github.com/lxfater/inpaint-web)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012501.webp)

Dự án mã nguồn mở cung cấp công cụ phục hồi ảnh và nâng cao độ phân giải chạy trực tiếp trên trình duyệt mà không cần gửi dữ liệu về server. (Đóng góp của [@lxfater](https://github.com/ruanyf/weekly/issues/3964))

14\. [Công cụ tạo và tùy biến nhân vật SVG](https://sinqi.tools/zh/avatar)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012502.webp)

Ứng dụng web hỗ trợ thiết kế và tùy biến các hình ảnh nhân vật vectơ dựa trên bộ tài nguyên mở [Open Peeps](https://www.openpeeps.com/). (Đóng góp của [@zerosoul](https://github.com/ruanyf/weekly/issues/3968))

## 资源

1\. [Trang tổng hợp sách điện tử song ngữ Đường Thư (TangLib)](http://www.tanglib.com/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012003.webp)

Trang web chia sẻ các tác phẩm văn học kinh điển thế giới hỗ trợ đọc song ngữ Trung - Anh kèm tính năng phát âm thanh đọc sách tương ứng. (Đóng góp của [@bigtang5](https://github.com/ruanyf/weekly/issues/3918))

2\. [Thư viện phông chữ nghệ thuật tạo bằng AI](https://www.ai.zitijia.com/list/1)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012007.webp)

Trang web tổng hợp và cung cấp các bộ phông chữ nghệ thuật được thiết kế bằng công nghệ AI, hỗ trợ người dùng kết xuất văn bản trực tuyến.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012008.webp)

Hệ thống cũng hỗ trợ người dùng viết tay 8 ký tự mẫu trực tiếp trên màn hình để AI tự động phân tích và tạo nên bộ phông chữ cá nhân độc quyền. (Đóng góp của [@qq345386817](https://github.com/ruanyf/weekly/issues/3930))

3\. [Chợ ứng dụng Cloud Native (Grapps Hub)](https://hub.grapps.cn/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012305.webp)

Trang web hỗ trợ tìm kiếm và cài đặt nhanh các ứng dụng cloud native lên các môi trường Docker, Kubernetes, Rainbond đi kèm các đường link mirror tăng tốc tải dữ liệu. (Đóng góp của [@RainBondsongyg](https://github.com/ruanyf/weekly/issues/3956))

4\. [iHateRegex](https://ihateregex.io/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012009.webp)

Trang web tổng hợp các biểu thức chính quy (regular expressions) phổ biến được minh họa cấu trúc bằng sơ đồ trực quan dựa trên dự án regexper. (Đóng góp của [@zkerhcy](https://github.com/ruanyf/weekly/issues/3938))

5\. [AsPoem (Trang giới thiệu thơ cổ Trung Quốc)](https://aspoem.com/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012010.webp)

Trang web học tập và thưởng thức vẻ đẹp của các tác phẩm thơ ca cổ điển Trung Quốc. (Đóng góp của [@meetqy](https://github.com/ruanyf/weekly/issues/3941))

6\. [mblog (Dịch vụ tạo trang blog cá nhân tối giản)](https://dev.mblog.club/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012004.webp)

Dịch vụ lưu trữ và thiết kế blog cá nhân tối giản phát triển dựa trên NextJS kết hợp dịch vụ cloud Laf, cung cấp tên miền phụ miễn phí cho người đăng ký. (Đóng góp của [@kingwrcy](https://github.com/ruanyf/weekly/issues/3922))

## 图片

1\. [Dự án phủ xanh vỉa hè đi bộ tại thành phố San Francisco](https://zachklein.com/Sidewalk+Garden)

Hình ảnh một đoạn vỉa hè đi bộ tại thành phố San Francisco vào thời điểm năm 2015.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082603.webp)

Một nhà thiết kế đã quyết định cải tạo dải bê tông thô cứng này thành một không gian xanh mát dạng "rừng đô thị".

Với tổng chiều rộng vỉa hè khoảng 3,66 mét, anh giữ lại khoảng không gian trung tâm phục vụ người đi bộ di chuyển, phần diện tích hai bên mép đường được bóc tách lớp bê tông để trồng cây xanh.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082604.webp)

Sau khi hoàn tất công đoạn cải tạo mặt đường đi bộ ở giữa, anh bắt đầu trồng các cây xanh và hoa cỏ ở hai bên dải đất vào năm 2016.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082605.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082606.webp)

Đến năm 2022, đoạn đường đi bộ thô cứng ban đầu đã chuyển mình thành không gian xanh tuyệt đẹp như thế này:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082607.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082608.webp)

Hình ảnh này gợi nhớ đến câu nói nổi tiếng: "Thời điểm tốt nhất để trồng một cái cây là 10 năm trước, và thời điểm tốt thứ hai chính là ngay bây giờ."

## ✍️ Bài đọc thêm

### Câu chuyện vận hành bền bỉ của một máy chủ cài đặt hệ điều hành NetBSD

Vào một ngày trong năm 2010, tôi nhận được yêu cầu từ một khách hàng.

Khách hàng muốn thiết lập một máy chủ nội bộ để chạy các dịch vụ cơ bản trong mạng LAN (bao gồm cấp phát IP DHCP, DNS nội bộ, web server Apache + PHP, chia sẻ tệp tin NFS và Samba).

Tôi đã tư vấn khách hàng đầu tư các thiết bị phần cứng máy chủ chuyên dụng, nhưng họ quyết định tận dụng lại một case máy tính cá nhân sẵn có: không có nguồn dự phòng, không có tính năng quản lý từ xa và ổ cứng lưu trữ cũng là dòng ổ cứng thông thường.

Ban đầu khách hàng có ý định cài đặt hệ điều hành Windows Server 2008 để chạy các dịch vụ trên. Tuy nhiên do thời gian chuẩn bị rất gấp chỉ có hai ngày, tôi đã thuyết phục họ chuyển sang cài đặt hệ điều hành NetBSD và nhận được sự đồng thuận.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012315.webp)

Sau khi hoàn tất cài đặt và chuyển giao hệ thống, trong suốt tháng đầu tiên vận hành, ngoại trừ một số sự cố trễ mạng nhỏ, hệ thống hoạt động hoàn toàn ổn định và nhận được phản hồi tốt từ khách hàng.

Trong vòng 2-3 năm tiếp theo, tôi thỉnh thoảng đăng nhập vào hệ thống để cập nhật một vài thông số nhỏ, sau đó mất liên lạc dần với khách hàng.

Đến tháng 2 năm 2021, tôi bất ngờ nhận được cuộc gọi từ chính vị khách hàng đó yêu cầu thiết lập một hệ thống tường lửa mới. Điều này đồng nghĩa với việc máy chủ chạy NetBSD năm xưa vẫn đang hoạt động bền bỉ! Với sự tò mò lớn, tôi đã nhận lời thực hiện công việc.

Khi kiểm tra hệ thống, tôi vô cùng kinh ngạc khi thấy máy chủ này vẫn đang hoạt động hoàn toàn bình thường. Dù không còn kết nối ra Internet nhưng các dịch vụ chia sẻ NFS, SMB, DNS, SMTP nội bộ vẫn chạy ổn định, đáp ứng khoảng 80% khối lượng công việc ban đầu thiết lập.

Điều khiến tôi ngạc nhiên nhất chính là thông số thời gian hoạt động liên tục (uptime) của máy chủ. Lần khởi động lại gần nhất của hệ thống là vào năm 2012 khi khu vực xảy ra một trận động đất nhỏ. Nhờ hệ thống máy phát điện dự phòng của khách hàng hoạt động tốt nên máy chủ luôn duy trì nguồn điện ổn định.

Khó có thể hình dung một chiếc máy tính cá nhân thông thường, chỉ mất vài giờ cài đặt ban đầu lại có thể chạy liên tục suốt 9 năm trời không cần khởi động lại và hầu như không cần bất kỳ hoạt động bảo trì, quản lý nào của kỹ sư.

Trải nghiệm này giúp tôi hiểu ra nguyên nhân vì sao phong cách làm việc của mình khó có thể giúp bản thân trở nên giàu có. Cấp trên trước đây của tôi thường phàn nàn việc tôi luôn tư vấn các giải pháp kỹ thuật quá ổn định và bền bỉ cho khách hàng, điều này vô hình trung làm sụt giảm nguồn thu từ phí bảo trì dài hạn của công ty. Theo ông, một hệ thống thỉnh thoảng phát sinh lỗi cần kỹ sư đến sửa chữa mới là giải pháp tối ưu hóa doanh thu. Nhưng đối với tôi, một sản phẩm kỹ thuật xuất sắc phải là một sản phẩm hoạt động bền bỉ và không đòi hỏi các hoạt động sửa chữa liên tục.

Đến nay, tôi không chắc liệu chiếc máy chủ đó có còn hoạt động hay không, nhưng nếu có cơ hội tôi rất muốn quay lại kiểm tra. Tôi thực sự biết ơn NetBSD - một hệ điều hành nhẹ nhàng, vô cùng ổn định, an toàn và hiệu quả, dù thực tế nó vẫn chưa nhận được vị thế và sự đánh giá xứng đáng từ cộng đồng công nghệ.

## Lịch sử tuần này

- 2023年（第 241 期）：[Kinh tế vĩ mô: Nhận định về việc động lực tăng trưởng kinh tế tiếp theo của Trung Quốc nằm ở khu vực nội địa](https://www.ruanyifeng.com/blog/2023/02/weekly-issue-241.html)
- 2022年（第 191 期）：[Con đường sự nghiệp: Chia sẻ của một lập trình viên về hành trình tự chủ tài chính](https://www.ruanyifeng.com/blog/2022/01/weekly-issue-191.html)
- 2021年（第 141 期）：[Triết lý sản phẩm: Thảo luận về sự thành công và ưu thế của các mô hình hệ sinh thái khép kín](https://www.ruanyifeng.com/blog/2021/01/weekly-issue-141.html)
- 2020年（第 91 期）：[Góc nhìn xã hội: Phân tích nguyên nhân vì sao giá nhà tại Mumbai (Ấn Độ) lại đắt đỏ ngang với Bắc Kinh](https://www.ruanyifeng.com/blog/2020/01/weekly-issue-91.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
