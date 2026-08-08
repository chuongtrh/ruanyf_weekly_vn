# 科技爱好者周刊（第 213 期）：知识孤岛，知识软件

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần。

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn。

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2483) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập。

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070501.webp)

Ngày 22 tháng 6, tại Giải vô địch bơi lội thế giới, một vận động viên người Mỹ bất ngờ bị ngất xỉu và chìm xuống đáy hồ bơi khi đang thi đấu. Huấn luyện viên của cô phát hiện điều bất thường đã lập tức lao xuống nước và cứu cô lên kịp thời. (Nguồn: [MP](https://mp.weixin.qq.com/s/X_KCtGbrqmZDVj_JCMMF3w))

## 本周话题：知识孤岛，知识软件

### （一）

Trang web hỏi đáp lập trình lớn nhất thế giới [Stack Overflow](https://stackoverflow.com/) vừa công bố kết quả cuộc khảo sát lập trình viên thường niên [năm 2022](https://survey.stackoverflow.co/2022/).

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070711.webp)

Năm nay, bảng khảo sát bổ sung thêm một câu hỏi đáng chú ý:

> *"Những yếu tố nào ảnh hưởng nhiều nhất đến hiệu suất làm việc của bạn? Chúng có thường xuyên xảy ra không và làm tiêu tốn bao nhiêu thời gian?"*

### （二）

Kết quả cho thấy, 68% lập trình viên khẳng định: **Rào cản lớn nhất đối với hiệu suất làm việc là không tìm thấy câu trả lời cho các vấn đề kỹ thuật.** Khi gặp sự cố, họ rơi vào tình trạng bế tắc do thiếu tài liệu hướng dẫn hoặc không có người để hỏi.

Tỷ lệ này càng cao đối với các kỹ sư cấp cao (Senior Developers). Họ thường phải đối mặt với các vấn đề đặc thù, hiếm gặp trong thực tế nên việc tìm kiếm câu trả lời càng khó khăn hơn.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070505.webp)

Trung bình một lập trình viên tốn khoảng 30 phút mỗi ngày chỉ để tìm kiếm câu trả lời cho các sự cố, và 25% số người được hỏi phải dành tới hơn một giờ đồng hồ mỗi ngày cho việc này. Đây là sự lãng phí rất lớn về mặt năng suất lao động đối với cả cá nhân và doanh nghiệp.

Hiện tượng này được gọi bằng thuật ngữ **"Đảo tri thức" (knowledge silos)** - biểu thị tình trạng thông tin, kiến thức bị chia cắt, cục bộ giống như các hòn đảo cô lập giữa đại dương, không thể kết nối và chia sẻ rộng rãi.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070506.webp)

Kiến thức thực tế luôn tồn tại ở đâu đó trong tổ chức, nhưng bạn không biết nó nằm ở đâu và làm sao để truy cập. Đây chính là nỗi đau trong kỷ nguyên kinh tế tri thức: **Kiến thức thiếu tính lưu thông, khó tìm kiếm và khó chia sẻ.**

### （三）

Để giải quyết bài toán này, các sản phẩm phần mềm chuyên biệt về **quản trị tri thức (Knowledge management software)** đang ngày một phát triển mạnh mẽ.

Tôi luôn tin rằng các phần mềm quản trị tri thức có tiềm năng thị trường rất lớn. Hệ thống thông tin càng phức tạp thì người dùng càng cần các công cụ quản lý tri thức mạnh mẽ. Đây cũng là hướng đi được khuyến khích để tối ưu hóa năng suất lao động. Nếu có thể giúp mỗi lập trình viên giảm thời gian tìm kiếm câu trả lời từ 30 phút xuống còn 25 phút mỗi ngày, hiệu quả mang lại cho doanh nghiệp sẽ cực kỳ lớn.

Một phần mềm quản trị tri thức tốt cần đáp ứng tối thiểu 3 yêu cầu:

1. **Khả năng ghi chép hiệu quả:** Chuyển đổi các tri thức giao tiếp ngắn hạn thành tài liệu lưu trữ dài hạn.
2. **Tổ chức khoa học:** Cung cấp cổng tra cứu tri thức tập trung và được phân loại rõ ràng (tương tự như các trang MDN hay Arch Wiki).
3. **Khả năng lưu thông:** Giúp kiến thức dễ dàng được chuyển giao giữa các cá nhân và dễ dàng tích hợp cùng các nguồn tri thức khác.

Trong đó, yếu tố lưu thông đòi hỏi tri thức phải được trình bày một cách dễ hiểu, trực quan. Bởi việc tiếp thu kiến thức phức tạp là một gánh nặng tâm lý lớn đòi hỏi sự nỗ lực làm giảm độ hỗn loạn (giảm entropy) từ phía người học. **Phần mềm quản trị tri thức tốt là phần mềm giúp giảm thiểu gánh nặng này.**

Mạng xã hội hỏi đáp Zhihu đang gặp phải vấn đề này khi thuật toán khuyến khích các câu trả lời dài dòng, phức tạp hóa vấn đề. Thay vì giải thích rõ ràng trong vài câu ngắn gọn, người viết thường kéo dài nội dung làm tăng mức độ rối rắm thông tin cho người đọc.

Một công cụ tốt cần đơn giản hóa các nguyên lý cơ bản để người mới dễ tiếp cận, đồng thời trình bày chi tiết các cấu phần kỹ thuật sâu để các kỹ sư có kinh nghiệm tham khảo giải quyết vấn đề.

## 活动

1、[Bài phát biểu của tác giả Evan You tại Hội nghị Juejin 2022](https://conf.juejin.cn/xdc2022/wap/?utm_source=ruanyfblogjiangshi)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070609.webp)

Evan You - tác giả của Vue.js và công cụ đóng gói Vite sẽ có bài chia sẻ mang tên **《Frontend Trends 2022》** tại Hội nghị nhà phát triển稀土开发者大会 diễn ra vào ngày 22 tháng 7 tới. Bài viết sẽ tập trung chia sẻ góc nhìn của ông về xu hướng phát triển Front-end, bao gồm: mô hình phát triển của các framework, hướng đi của công cụ đóng gói build tools và xu hướng phát triển ứng dụng full-stack JavaScript.

Bạn đọc quan tâm có thể quét mã QR trên hải báo phía dưới để đăng ký tham gia trực tuyến miễn phí và có cơ hội nhận các phần quà hấp dẫn từ ban tổ chức:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070610.webp)

## 科技动态

1、[Coca-Cola thay đổi thiết kế nắp chai gắn liền vỏ chai tại Anh](https://www.cocacolaep.com/gb/news/2022/coca-cola-begins-introduction-of-attached-caps-across-entire-portfolio-to-boost-collection-and-recylcing-and-help-to-prevent-litter/)

Hãng nước giải khát Coca-Cola vừa công bố thiết kế nắp chai mới tại thị trường Anh với phần nắp được gắn liền vào vòng cổ chai không thể tháo rời:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052102.webp)

Thay đổi này nhằm thúc đẩy tỷ lệ thu gom và tái chế nhựa đồng bộ cả phần nắp và thân chai, tránh tình trạng nắp chai nhựa bị vứt bỏ riêng lẻ gây ô nhiễm môi trường.

2、[Quy trình thu âm tiếng động thực địa độc đáo của phim điện ảnh viễn tưởng Dune](https://www.nytimes.com/2022/03/16/movies/dune-denis-villeneuve-sound-sound/)

Bộ phim điện ảnh viễn tưởng đình đám Dune (2021) lấy bối cảnh trên một hành tinh sa mạc đầy cát bụi. Để tái hiện chân thực không gian rộng lớn này, đội ngũ âm thanh đã thực hiện thu âm tiếng động thực địa tại sa mạc Death Valley (California) thay vì trong phòng thu thông thường:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032001.webp)

Để mô phỏng tiếng cát lún chứa hạt "hương liệu" đặc biệt dưới chân nhân vật, các chuyên gia đã rải bánh quy giòn lên cát và thu âm tiếng bước chân giẫm lên để tạo ra tiếng rào rạo tinh tế đặc trưng:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032002.webp)

Cả bộ phim đã sử dụng hơn 3.200 hiệu ứng âm thanh thực địa được thu bằng cách chôn microphone dưới cát hoặc dùng búa gỗ gõ lên bề mặt các cồn cát:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032003.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032004.webp)

3、[Hoa Kỳ dự kiến bắt buộc lắp đặt thiết bị kiểm tra nồng độ cồn hơi thở trên xe ô tô mới](https://jalopnik.com/we-can-cut-traffic-deaths-in-half-but-nobody-wants-to-1848892809)

Năm 2021, nước Mỹ ghi nhận khoảng 43.000 người tử vong vì tai nạn giao thông - mức cao nhất trong vòng 15 năm qua. Để hạn chế tình trạng này, chính phủ đang xem xét đạo luật bắt buộc lắp đặt thiết bị đo nồng độ cồn hơi thở tích hợp trên các dòng xe mới bán ra:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052110.webp)

Thiết bị này được kết nối trực tiếp với hệ thống đề nổ động cơ. Trước khi lái xe, tài xế bắt buộc phải thổi nồng độ cồn vào ống đo, hệ thống chỉ cho phép khởi động xe khi chỉ số cồn nằm dưới ngưỡng quy định. Hiện tại đã có khoảng 350.000 xe tại Mỹ tự nguyện lắp đặt thiết bị này.

4、[Garmin ra mắt thiết bị camera hành trình kiêm radar cảnh báo cho xe đạp](https://news.mydrivers.com/1/833/833294.htm)

Hãng công nghệ Garmin giới thiệu thiết bị gắn sau yên xe đạp tích hợp 3 tính năng: camera hành trình, radar cảnh báo và đèn hậu:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052303.webp)

Thiết bị giúp truyền trực tiếp hình ảnh hành trình phía sau về màn hình điện thoại của người lái. Đồng thời, hệ thống radar tích hợp sẽ tự động phát hiện và gửi tín hiệu cảnh báo trên điện thoại khi phát hiện có phương tiện đang tiến lại gần từ phía sau ở khoảng cách 140 mét:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052304.webp)

5、[Đội xe taxi tự lái Cruise gặp sự cố gây tắc nghẽn giao thông tại San Francisco](https://thelastdriverlicenseholder.com/2022/06/29/driverless-robotaxi-fleet-paralyzed-for-hours-in-san-francisco/)

Thành phố San Francisco vừa trở thành đô thị lớn đầu tiên trên thế giới cho phép taxi tự lái không người lái vận hành thương mại vào khung giờ từ 22:00 đêm đến 05:00 sáng hôm sau:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070201.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070202.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070203.webp)

Tuy nhiên, vào đêm ngày 29 tháng 6, hơn 12 chiếc robotaxi của hãng Cruise đã đột ngột dừng đỗ chết cứng tại một ngã tư lớn không rõ nguyên nhân. Sự cố khiến giao thông khu vực bị tê liệt nhiều giờ liền cho đến khi nhân viên kỹ thuật trực tiếp tới hiện trường để di dời xe về bãi đỗ:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070204.webp)

Sự cố cho thấy việc tích hợp xe tự lái vào hạ tầng giao thông đô thị hiện hữu vẫn còn nhiều thách thức phức tạp, việc quy hoạch các tuyến đường chuyên dụng cho xe tự lái có thể là giải pháp an toàn hơn ở giai đoạn đầu.

## 文章

1、[Huawei Nhậm Chính Phi chia sẻ về mục tiêu thành lập Ủy ban chuyên gia công nghệ](https://www.163.com/dy/article/HBFKD26S0519QIKK.html)（Tiếng Trung）

Bài viết ghi lại nội dung cuộc đối thoại nội bộ của ông Nhậm Chính Phi giải thích lý do thành lập Ủy ban chuyên gia công nghệ làm diễn đàn chia sẻ ý tưởng học thuật, kết nối và thúc đẩy tư duy sáng tạo cho hơn 6.000 chuyên gia khoa học và hàng trăm ngàn kỹ sư của tập đoàn.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070502.webp)

2、[Nghiên cứu khoa học: Hành trình di cư hàng vạn cây số của loài chim yến Bắc Kinh](https://www.bjnews.com.cn/detail/165692908214307.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070710.webp)

Hàng năm vào tháng 4, quần thể chim yến sẽ bay đến làm tổ tại khu vực Di Hòa Viên (Bắc Kinh) và di cư đi nơi khác vào tháng 7. Nhờ lắp đặt thiết bị định vị siêu nhỏ, các nhà khoa học đã vẽ được lộ trình bay di cư khổng lồ của chúng qua Tân Cương, Trung Á, Trung Đông để tới trú đông tại Nam Phi.

3、[Kinh nghiệm tự học và phát triển ứng dụng di động đa nền tảng từ con số 0](https://imf.ms/web/2022/07/05/my-first-web-hybird-project-experience/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070608.webp)

Tác giả chia sẻ chi tiết lộ trình học tập công nghệ và các bước tự xây dựng thành công dự án Web/Hybrid hoàn chỉnh hoạt động ổn định trên cả trình duyệt, hệ điều hành Android và iOS từ xuất phát điểm chưa có kinh nghiệm. (Đóng góp của [@imfms](https://github.com/ruanyf/weekly/issues/2492))

4、[Cơ chế hoạt động giải phóng oxy khẩn cấp của các dòng nến oxy](https://minearc.com/oxygen-candles-providing-emergency-air/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051005.webp)

Ngược lại với nến thông thường tiêu thụ oxy khi cháy, nến oxy sử dụng hỗn hợp hóa chất (như natri clorat và sắt) khi kích hoạt phản ứng nhiệt sẽ giải phóng lượng lớn khí oxy sạch phục vụ cứu hộ khẩn cấp trong hầm mỏ hoặc tàu ngầm.

5、[Đề xuất sử dụng JavaScript và máy ảo Deno làm tiêu chuẩn container ứng dụng](https://tinyclouds.org/javascript_containers)（Tiếng Anh）

Tác giả Ryan Dahl (cha đẻ của Node.js và Deno) đề xuất ý tưởng sử dụng JS làm ngôn ngữ container tiêu chuẩn chạy trực tiếp trên máy ảo Deno, giúp đơn giản hóa quy trình đóng gói phần mềm khi lập trình viên không cần tự build file image container phức tạp.

6、[Kinh nghiệm tuyển chọn trường học và chương trình đào tạo Thạc sĩ CNTT tại Mỹ](https://evanp.me/2022/05/04/masters-degree-in-computer-science/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050708.webp)

Một lập trình viên chia sẻ cẩm nang các tiêu chí đánh giá chương trình học, học phí và cơ hội việc làm thực tế hỗ trợ các kỹ sư CNTT lựa chọn trường học thạc sĩ phù hợp tại Mỹ.

7、[Tổng hợp các ứng dụng web tự host vận hành trong gia đình của tác giả](https://noted.lol/what-are-your-most-used-self-hosted-applications/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050509.webp)

Tác giả giới thiệu danh sách các dịch vụ SaaS tự host (như Nextcloud, Vaultwarden, Plex) đang chạy trên hệ thống mạng nội bộ gia đình phục vụ lưu trữ dữ liệu cá nhân an toàn.

8、[Giải pháp cào dữ liệu trang web thông qua việc trích xuất bộ nhớ máy ảo JS](https://www.adriancooney.ie/blog/web-scraping-via-javascript-heap-snapshots)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050917.webp)

Đối với các trang web ứng dụng client-side rendering phức tạp gây khó khăn cho việc cào dữ liệu (scraping), tác giả đề xuất giải pháp chụp nhanh phân tích bộ nhớ RAM (heap snapshot) của máy ảo JavaScript trên trình duyệt để trích xuất trực tiếp dữ liệu dạng cấu trúc.

## 工具

1、[KOReader: Phần mềm đọc sách điện tử nguồn mở đa năng](https://koreader.rocks/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050910.webp)

Trình đọc sách hỗ trợ nhiều định dạng file (EPUB, PDF, MOBI) tối ưu hiển thị mượt mà cho các dòng máy đọc sách E-ink (Kindle, Kobo) và thiết bị Android.

2、[Pointless: Tiện ích bảng trắng vẽ tranh tương tác trực tuyến gọn nhẹ](https://github.com/kkoomen/pointless)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050911.webp)

Ứng dụng white-board trực tuyến hỗ trợ nhiều người dùng cùng tham gia phác thảo ý tưởng, vẽ sơ đồ quy trình trực quan trên giao diện web.

3、[PyScript: Công cụ hỗ trợ chạy trực tiếp mã nguồn Python trên trình duyệt](https://pyscript.net/)

Dự án do Anaconda phát triển cho phép lập trình viên nhúng trực tiếp mã nguồn Python chạy trên nền trình duyệt Web tận dụng sức mạnh biên dịch của WebAssembly.

4、[MacCopier: Tiện ích tự động trích xuất và sao chép mã OTP từ SMS trên macOS](https://github.com/DreamSaddle/MacCopier)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070607.webp)

Công cụ hỗ trợ quét hòm thư tin nhắn được chuyển tiếp từ iPhone sang máy Mac để tự động phát hiện, trích xuất mã xác thực OTP và lưu vào clipboard giúp đăng nhập nhanh. (Đóng góp của [@DreamSaddle](https://github.com/ruanyf/weekly/issues/2489))

5、[doctree: Tiện ích tự động phân tích mã nguồn sinh trang web tài liệu API](https://github.com/sourcegraph/doctree)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050916.webp)

Công cụ hỗ trợ quét thư mục dự án đa ngôn ngữ để tự động trích xuất các cấu trúc khai báo hàm, lớp dữ liệu và kết xuất thành trang web tài liệu tra cứu API chuyên nghiệp.

6、[htmx: Thư viện JS hỗ trợ thực hiện các yêu cầu AJAX trực tiếp từ thẻ HTML](https://htmx.org/)

Thư viện nhỏ gọn cho phép lập trình viên Front-end thực hiện gọi API HTTP GET/POST và cập nhật DOM cục bộ trực tiếp từ các thuộc tính thẻ HTML không cần viết mã JS.

7、[USWDS: Bộ thiết kế giao diện UI hệ thống chuẩn hóa của Chính phủ Mỹ](https://designsystem.digital.gov/)

Thư viện thiết kế và các component UI được thiết lập đồng bộ nhằm chuẩn hóa trải nghiệm người dùng và khả năng tiếp cận thông tin trên toàn bộ các cổng thông tin điện tử của chính phủ.

8、[JBake: Bộ công cụ tạo trang web tĩnh viết bằng Java](https://jbake.org/)

Tiện ích static site generator hỗ trợ viết tài liệu bằng định dạng Markdown, AsciiDoc và kết xuất trang web tĩnh nhanh chóng cho các lập trình viên Java.

9、[Repo Visualizer: Tiện ích tự động vẽ sơ đồ cấu trúc mã nguồn của GitHub](https://github.com/githubocto/repo-visualizer)

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040302.webp)

Công cụ do GitHub phát triển chạy qua GitHub Actions giúp tự động vẽ sơ đồ dạng hình tròn biểu diễn dung lượng và thư mục của mã nguồn dưới dạng file ảnh SVG động cập nhật theo lịch sử commit.

## 资源

1、[How a Mechanical Watch Works (Nguyên lý cơ học hoạt động của đồng hồ cơ)](https://ciechanow.ski/mechanical-watch/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050709.webp)

Bài phân tích chi tiết giới thiệu cách thức hoạt động phối hợp của các bộ phận lò xo dây cót, bánh xe cân bằng và bánh răng cơ học để duy trì nhịp đếm thời gian chính xác của đồng hồ cơ thông qua các hình vẽ 3D tương tác tuyệt đẹp.

2、[Bản dịch tiếng Trung đối chiếu song ngữ của cuốn sách Software Engineering at Google](https://qiangmzsx.github.io/Software-Engineering-at-Google/)

Dự án dịch thuật cộng đồng chia sẻ bản dịch chi tiết giới thiệu các quy chuẩn văn hóa lập trình, quy trình quản lý dự án và công nghệ kỹ nghệ phần mềm đang vận hành tại Google. (Đóng góp của [@zhang14725804](https://github.com/ruanyf/weekly/issues/2484))

3、[Chuỗi cẩm nang hướng dẫn lập trình ứng dụng máy tính đa nền tảng bằng Tauri](https://www.zhihu.com/column/c_1519079232848785408)

Loạt bài viết hướng dẫn lập trình viên sử dụng framework Tauri kết hợp Rust và Webview hệ thống để xây dựng các ứng dụng desktop đa nền tảng gọn nhẹ thay thế cho Electron tiêu tốn tài nguyên RAM. (Đóng góp của [@lencx](https://github.com/ruanyf/weekly/issues/2486))

4、[VueJS Challenges: Kho bài tập rèn luyện kỹ năng viết code VueJS](https://cn-vuejs-challenges.netlify.app/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070606.webp)

Trang web tổng hợp các thử thách viết code tương tác, xử lý state trong Vue với nhiều cấp độ từ dễ đến khó giúp lập trình viên củng cố kiến thức. (Đóng góp của [@webfansplz](https://github.com/ruanyf/weekly/issues/2487))

5、[Learning Synths by Ableton (Giáo trình tìm hiểu nguyên lý thiết kế âm thanh tương tác)](https://learningsynths.ableton.com/zh-Hans)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050710.webp)

Giáo trình tương tác trực quan (hỗ trợ tiếng Việt) giới thiệu nguyên lý hoạt động của các bộ tổng hợp âm thanh (synthesizer) bằng các ví dụ thực hành âm thanh trực tiếp trên web.

## 图片

1\. [Thiết kế mẫu quan tài hình ren xoắn ốc độc đáo](https://kottke.org/22/03/the-inventor-of-the-screw-in-coffin)

Một kỹ sư người Mỹ đã đăng ký bằng sáng chế cho thiết kế quan tài hình ren xoắn ốc độc đáo:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030507.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030508.webp)

Quan tài được thiết kế hình trụ tròn có ren xoắn ngoài cho phép vặn vít trực tiếp chìm thẳng đứng xuống lòng đất bằng máy tự động giúp giảm thiểu tối đa diện tích huyệt mộ. Khi cần di dời cải táng, đơn vị kỹ thuật chỉ cần dùng máy xoay ngược chiều để đưa quan tài lên nguyên vẹn một cách nhanh chóng.

2\. [Mẹo thiết kế xoay nghiêng màn hình rộng để tăng dòng hiển thị code](https://sprocketfox.io/xssfox/2021/12/02/xrandr/)

Người dùng màn hình siêu rộng (Ultra-wide 21:9) thường gặp rào cản thiếu chiều cao hiển thị khi đọc tài liệu web hoặc viết code nếu đặt màn hình nằm ngang thông qua giá đỡ:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120302.webp)

Nếu xoay dọc màn hình 90 độ, việc xem video giải trí hoặc hiển thị các cửa sổ rộng lại gặp khó khăn:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120303.webp)

Một lập trình viên đã đề xuất giải pháp xoay nghiêng màn hình một góc 22 độ trên Linux, giúp đường chéo màn hình 21:9 nằm ở vị trí nằm ngang:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120304.webp)

Thiết kế độc đáo này giúp tối ưu hóa chiều dài hiển thị dòng code và cho phép mở nhiều cửa sổ làm việc song song trực quan hơn.

## 💡 Bài đọc thêm

### Tại sao số lượng bài báo khoa học xuất bản khổng lồ không giúp tăng tốc độ khoa học?

Nghiên cứu đăng tải trên Kỷ yếu Viện Hàn lâm Khoa học Quốc gia Mỹ (PNAS) chỉ ra thực tế đáng suy ngẫm: việc bùng nổ số lượng bài báo khoa học xuất bản hàng năm hiện nay không giúp thúc đẩy nhanh tiến bộ khoa học tương ứng:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070712.webp)

Nguyên nhân chính do các cơ sở nghiên cứu và trường đại học lấy chỉ tiêu số lượng bài báo xuất bản làm thước đo chính để đánh giá hiệu quả công việc và xét duyệt tài trợ nghiên cứu cho các nhà khoa học.

Tuy nhiên, lượng bài viết quá nhiều dẫn tới việc các học giả gặp quá tải thông tin, không đủ thời gian để đọc và phát hiện ra các ý tưởng đột phá thực sự trong mớ bài viết chắp vá. 

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070713.webp)

Sự bão hòa thông tin khiến lượng trích dẫn học thuật có xu hướng tập trung cục bộ vào một vài bài viết kinh điển đã nổi tiếng trước đó, còn các bài viết mới chất lượng thường bị chìm nghỉm trong đại dương thông tin hỗn loạn, làm chậm đà phát triển của các lĩnh vực khoa học mới.

## 历史上的本周

- 2021年（第 165 期）：[Thảo luận lập trình: Xu hướng chuyển dịch và phát triển của các ứng dụng đa nền tảng (All-in-one Apps)](https://www.ruanyifeng.com/blog/2021/07/weekly-issue-165.html)
- 2020年（第 114 期）：[Nhìn nhận thực tế: Xu hướng sống tự chủ không ràng buộc doanh nghiệp (U-disk life style) và sự bùng nổ của thị trường việc làm tự do qua app](https://www.ruanyifeng.com/blog/2020/07/weekly-issue-114.html)
- 2019年（第 63 期）：[Phân tích thị trường: Xu hướng tập trung hóa thị phần và quyền lực của các tập đoàn công nghệ lớn trên Internet](https://www.ruanyifeng.com/blog/2019/07/weekly-issue-63.html)
- 2018年（第 12 期）：[Thảo luận kinh tế xã hội: Áp lực già hóa dân số và bài toán thiếu hụt quỹ hưu trí quốc gia](https://www.ruanyifeng.com/blog/2018/07/weekly-issue-12.html)

## 鸣谢

Nền tảng quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070801.webp)

（Hết）
