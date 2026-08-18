# Bản tin chia sẻ công nghệ (Số 329): D2 - Công cụ vẽ sơ đồ cực đỉnh

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/5610) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121117.webp)

Khu tổ hợp thế giới Băng tuyết Cáp Nhĩ Tân chuẩn bị khai viên chào đón du khách. Hiện tại, các công nhân đang tích cực khai thác đá trên dòng sông Tùng Hoa, với khối lượng khai thác hằng ngày đạt xấp xỉ gần vạn khối băng lớn để phục vụ thi công các công trình điêu khắc băng khổng lồ. (Nguồn: [Xinhua](https://app.xinhuanet.com/news/article.html?articleId=451916149ce4dde7e6035e935eb5a37f))

## 示意图利器 D2

Có rất nhiều công cụ hỗ trợ vẽ sơ đồ và biểu đồ quy trình hiện nay.

Bản thân tôi luôn đặc biệt yêu thích các công cụ vẽ sơ đồ bằng câu lệnh văn bản (text-to-diagram) để thiết kế các mô hình khung dây (wireframes), tiêu biểu là các công cụ như Mermaid, PlantUML hay Graphviz.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121201.webp)

Ưu điểm vượt trội của giải pháp này là khả năng sinh ảnh tự động từ các dòng lệnh mô tả tối giản, rất thích hợp để lưu trữ trực tiếp trong các kho chứa mã nguồn (repositories) giúp dễ dàng quản lý phiên bản (version control) qua Git.

Mới đây, tôi vừa phát hiện ra một công cụ tương tự có chất lượng trải nghiệm vượt trội hơn hẳn mang tên [D2](https://d2lang.com). Công cụ này sở hữu cú pháp vô cùng trực quan, dễ học cùng bộ tính năng mạnh mẽ. Tôi xin chia sẻ chi tiết về công cụ này với các bạn.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120613.webp)

D2 hỗ trợ vận hành linh hoạt dưới dạng công cụ dòng lệnh (CLI) hoặc chạy trực tiếp trên môi trường trình duyệt. Giả sử bạn đang sở hữu một tệp chứa các câu lệnh mô tả sơ đồ mang tên `example.d2`, lệnh để tự động biên dịch và sinh hình ảnh tương ứng như sau:

> $ d2 example.d2

Thông thường, tôi thích sử dụng công cụ này trực tiếp trên trình duyệt hơn. Hãng phát triển cung cấp một trình biên tập trực tuyến miễn phí tại địa chỉ [play.d2lang.com](https://play.d2lang.com/) (hình dưới). Bạn chỉ cần dán đoạn mã mô tả vào khung soạn thảo và nhấp nút "Compile" là hệ thống sẽ lập tức hiển thị hình ảnh sơ đồ tương ứng ở khung bên cạnh.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121202.webp)

Nếu muốn tạo một khối nút (node) đơn giản (ví dụ nút mang nhãn hiển thị là A), bạn chỉ cần gõ ký tự A:

> A

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120601.webp)

Mặc định ký tự gõ vào sẽ vừa làm mã định danh vừa làm nhãn hiển thị của nút đó. Nếu muốn tùy biến nội dung nhãn hiển thị chi tiết bằng tiếng Việt hoặc tiếng Trung, bạn có thể viết như sau:

> A: Giáp

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120602.webp)

Tiếp theo, hãy thử tạo thêm một nút B:

> A: Giáp  
> B: Ất

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120603.webp)

Bây giờ chúng ta sẽ liên kết hai nút này lại với nhau:

> A: Giáp  
> B: Ất  
> A -> B

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120604.webp)

D2 hỗ trợ nhiều kiểu mũi tên liên kết đa dạng: mũi tên xuôi (`->`), mũi tên ngược (`<-`), hoặc mũi tên hai chiều (`<->`). Nếu bạn không muốn hiển thị mũi tên mà chỉ muốn một đường nối thẳng đơn giản, hãy sử dụng ký hiệu hai dấu gạch ngang (`--`).

Chúng ta cũng có thể dễ dàng chèn thêm các đoạn văn bản ghi chú trực tiếp trên đường mũi tên liên kết:

> A: Giáp  
> B: Ất  
> A -> B: Liên kết

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120606.webp)

Giữa hai nút hoàn toàn có thể thiết lập nhiều đường liên kết song song với nhau:

> A: Giáp  
> B: Ất  
> A -> B: Yêu cầu  
> A <- B: Phản hồi

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120609.webp)

Các mối liên kết liên tục của các nút cũng có thể được viết thu gọn trên cùng một dòng lệnh:

> Giáp -> Bính <- Ất: Liên kết

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120610.webp)

Hoặc mô tả một quy trình tuần hoàn liên tục:

> Giai đoạn 1 -> Giai đoạn 2 -> Giai đoạn 3 -> Giai đoạn 4  
> Giai đoạn 4 -> Giai đoạn 1: Phản hồi

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120611.webp)

Chỉ với bấy nhiêu cú pháp cơ bản kể trên là bạn đã có thể tự tin vẽ được hầu hết các sơ đồ quy trình và sơ đồ kiến trúc hệ thống thông thường rồi, thực sự vô cùng đơn giản và nhanh chóng.

Bên cạnh đó, D2 còn sở hữu năng lực thiết kế các sơ đồ cực kỳ phức tạp với hệ thống cú pháp nâng cao phong phú, các bạn quan tâm có thể chủ động tra cứu thêm tại [Tài liệu hướng dẫn chính thức](https://d2lang.com/tour/intro).

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120614.webp)

Một thủ thuật nhỏ cuối cùng: Nếu muốn thay đổi hình dáng mặc định của khối nút từ hình chữ nhật sang hình tròn, bạn có thể viết cấu hình như sau:

> A: Giáp  
> A.shape: circle

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120607.webp)

Thậm chí bạn có thể chuyển hình dáng nút thành hình đám mây để biểu diễn các dịch vụ điện toán đám mây (Cloud Services):

> A: Giáp  
> A.shape: cloud

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120608.webp)

Và dễ dàng điều chỉnh màu sắc viền của khối nút:

> A: Giáp  
> A.style.stroke: red

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120612.webp)

## [活动] AI 编程挑战赛

Dành cho các bạn lập trình viên: Một giải đấu lập trình ứng dụng AI quy mô quốc tế mang tên **AI Lập Trình Điên Phong Khiêu Chiến Sài** (AI Programming Challenge) chính thức được khởi động.

Chỉ cần bạn làm chủ các kỹ năng tương tác với AI, ứng dụng trợ lý AI để xây dựng các sản phẩm phần mềm sáng tạo độc đáo hoặc giải nhanh các bài toán thuật toán hóc búa là đã hoàn toàn đủ điều kiện đăng ký tham gia tranh tài.

Việc tham gia cuộc thi không chỉ giúp bạn rèn luyện và nâng cao năng lực lập trình cộng tác cùng AI mà còn giúp làm phong phú thêm hồ sơ năng lực cá nhân của bạn, tạo điểm nhấn ấn tượng trong CV trước các nhà tuyển dụng.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121211.webp)

(1) Cơ cấu giải thưởng vô cùng hấp dẫn với tổng giá trị giải thưởng lên tới 200.000 nhân dân tệ, trong đó **giải Nhất trị giá 40.000 nhân dân tệ**. Cuộc thi chia bảng chấm giải độc lập giữa nhóm thí sinh sinh viên và nhóm thí sinh tự do. Các thí sinh đạt thứ hạng cao sẽ nhận được cơ hội tuyển dụng đặc cách (rút ngắn quy trình đi thẳng vào vòng phỏng vấn cuối cùng cho cả vị trí thực tập lẫn chính thức).

(2) **Giải đấu chia làm hai phân nhánh tranh tài độc lập: Nhánh Thuật toán và Nhánh Ứng dụng**. Bạn có thể chọn gửi các sản phẩm ứng dụng phần mềm tự phát triển hoặc đăng ký giải các bài toán thuật toán hệ thống.

(3) Cổng đăng ký tham gia giải đấu hiện đã chính thức mở. Nhánh Ứng dụng sáng tạo sẽ bắt đầu mở cổng nhận sản phẩm dự thi từ ngày 16 tháng 12. Trong khi đó, nhánh Thuật toán hiện đã cho phép thí sinh tham gia các vòng loại trực tuyến, vòng chung kết sẽ được tổ chức dưới dạng cuộc thi hackathon offline.

(4) Tại vòng chung kết của cả hai nhánh đấu, ban tổ chức yêu cầu các thí sinh bắt buộc phải sử dụng trợ lý lập trình thông minh Doubao MarsCode làm công cụ hỗ trợ chính.

Giải đấu lập trình đỉnh cao này do Doubao MarsCode phối hợp cùng cộng đồng công nghệ Juejin đồng tổ chức. Các thông tin chi tiết về thể lệ thi đấu và cổng đăng ký tham dự có thể tra cứu trực tiếp tại [Trang chủ sự kiện](https://zjsms.com/iUNhdBEk/) hoặc quét mã QR trên poster. Chúc các bạn độc giả sẽ gặt hái được những thành tích cao tại giải đấu.

## 科技动态

1、[Dự án làm mát đô thị bằng nước hồ sâu](https://www.theglobeandmail.com/business/industry-news/property-report/article-the-worlds-largest-deep-lake-water-cooling-project-just-got-bigger/)

Toronto — thành phố lớn nhất của Canada — nằm ngay cạnh bờ hồ Ontario xinh đẹp. Hồ Ontario là một trong những hồ nước ngọt có độ sâu rất lớn, với điểm sâu nhất đạt tới 244 mét.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041412.webp)

Chính quyền thành phố Toronto hiện đang triển khai xây dựng một công trình hạ tầng vô cùng độc đáo: Khai thác nguồn nước lạnh ở đáy hồ Ontario để làm hệ thống điều hòa nhiệt độ tự nhiên cho toàn bộ khu vực trung tâm thành phố.

Nước ở tầng đáy của hồ Ontario luôn duy trì nhiệt độ rất thấp quanh năm. Hệ thống đường ống của dự án sẽ lấy nước từ độ sâu 85 mét dưới đáy hồ, nơi nhiệt độ nước luôn giữ ở mức ổn định khoảng 4 độ C ngay cả vào giữa mùa hè nóng nực.

Nguồn nước lạnh tự nhiên này sẽ được dẫn qua hệ thống đường ống dài 40km chảy về các trạm trao đổi nhiệt đặt tại trung tâm thành phố để cung cấp nguồn khí mát tự nhiên cho các tòa nhà, giúp tiết kiệm đáng kể điện năng tiêu thụ.

2、[Chiếc bàn gỗ tự bước đi](https://www.decarpentier.nl/carpentopod)

Một kỹ sư nước ngoài vừa chế tạo thành công một chiếc bàn gỗ độc đáo có khả năng tự bước đi theo tín hiệu điều khiển.

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024091217.webp)

Chiếc bàn gỗ này được thiết kế với hệ thống 12 chiếc chân cơ học. Mỗi chu kỳ bước đi, hệ thống sẽ phối hợp di chuyển đồng thời 3 chiếc chân dưới sự truyền động trực tiếp từ các động cơ điện độc lập.

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024091218.webp)

Bên trong thân bàn được lắp đặt bộ thu tín hiệu không dây để nhận các câu lệnh điều khiển từ xa. Một máy tính điều khiển ngoài sẽ chịu trách nhiệm phân tích dữ liệu, tự động tính toán trình tự bước đi của từng chân cùng góc độ và biên độ xoay tương ứng của động cơ để chiếc bàn di chuyển mượt mà.

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024091219.webp)

3、[Robot chó hỗ trợ phá sóng mạng Wi-Fi](https://www.tomshardware.com/tech-industry/big-tech/dog-like-robot-jams-home-networks-and-disables-devices-during-police-raids-dhs-develops-neo-robot-for-walking-denial-of-service-attacks)

Nhiều băng nhóm tội phạm thường lắp đặt hệ thống camera giám sát không dây dày đặc xung quanh căn cứ để kịp thời phát hiện mọi động tĩnh tiếp cận của lực lượng chức năng.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072405.webp)

Để giải quyết bài toán này, Bộ An ninh Nội địa Mỹ đã nghiên cứu và thử nghiệm thành công một dòng robot bốn chân (chó robot) chuyên dụng có tính năng phá hủy kết nối mạng của camera giám sát.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072406.webp)

Chú chó robot này được trang bị một hệ thống anten công suất lớn. Khi tiếp cận khu vực mục tiêu, robot sẽ tự động quét và phân tích tần số sóng cũng như kênh truyền Wi-Fi đang hoạt động xung quanh, sau đó phát ra các luồng tín hiệu nhiễu cực mạnh gây tắc nghẽn băng thông, làm tê liệt hoàn toàn kết nối.

Toàn bộ các thiết bị nhà thông minh sử dụng kết nối không dây xung quanh khu vực (bao gồm cả camera giám sát) sẽ lập tức bị mất kết nối và dừng hoạt động. Bài học rút ra là đối với các vị trí an ninh trọng yếu, hệ thống camera giám sát bắt buộc phải sử dụng kết nối dây cáp truyền thống để đảm bảo an toàn.

4、[Công nghệ sản xuất cà phê không hạt (Beanless Coffee)](https://www.bbc.com/news/articles/c4gv0rvx0dvo)

Một số công ty khởi nghiệp phương Tây mới đây đã giới thiệu dòng sản phẩm "cà phê không hạt" độc đáo, tức sản phẩm cà phê được pha chế hoàn toàn không sử dụng đến hạt cà phê truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024091303.webp)

Quy trình sản xuất ứng dụng công nghệ tái chế các hạt chà là hoặc hạt trái cây bỏ đi để chiết xuất sinh khối chất hữu cơ, sau đó bổ sung thêm hoạt chất caffeine tự nhiên được chiết xuất từ lá trà xanh để tạo nên hương vị đặc trưng của cà phê.

Giải pháp này được đánh giá cao nhờ tính thân thiện với môi trường, giúp giảm thiểu đáng kể lượng rác thải hữu cơ trong ngành thực phẩm, đồng thời giảm áp lực phá rừng để lấy đất canh tác các đồn điền cà phê.

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024091304.webp)

Những người đã trải nghiệm cho biết hương vị của sản phẩm cà phê không hạt này đạt độ tương đồng cực cao so với các dòng cà phê hạt chất lượng tốt, khiến người uống phổ thông khó lòng phân biệt được sự khác nhau. Tuy nhiên, giá thành sản xuất hiện tại của sản phẩm vẫn còn tương đối cao, nhỉnh hơn một chút so với hạt cà phê truyền thống.

## 文章

1、[Bộ quy tắc thiết lập lại CSS (Phiên bản 2024)](https://www.joshwcomeau.com/css/custom-css-reset/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024102501.webp)

Tác giả đề xuất bộ cấu hình CSS Reset (khởi tạo lại các thuộc tính hiển thị mặc định của trình duyệt) tối giản mới nhất chỉ bao gồm vỏn vẹn 9 quy tắc cốt lõi, đi kèm phần phân tích chi tiết ý nghĩa kỹ thuật của từng quy tắc.

2、[Lịch sử ra đời của bộ phối màu lập trình kinh điển Monokai](https://monokai.pro/history) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024103102.webp)

Bài viết chia sẻ về chặng đường ra đời và phát triển của Monokai — một trong những bộ phối màu giao diện (color scheme) dành cho trình soạn thảo mã nguồn được cộng đồng lập trình viên yêu thích nhất trên thế giới.

3、[Phân biệt khái niệm xử lý đồng thời (Concurrency) và xử lý song song (Parallelism)](https://www.rugu.dev/en/blog/concurrency-and-parallelism/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024091302.webp)

Bài phân tích cơ bản giúp lập trình viên phân biệt rõ rệt hai khái niệm dễ gây nhầm lẫn là Concurrency và Parallelism, đi kèm các ví dụ minh họa trực quan bằng ngôn ngữ JavaScript.

4、[Hướng dẫn cấu hình liên kết trực tiếp đến một đoạn văn bản chỉ định trên trang web](https://alfy.blog/2024/10/19/linking-directly-to-web-page-content.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024102409.webp)

Các trình duyệt hiện đại đã hỗ trợ cơ chế chèn thêm tham số vào URL để tự động cuộn trang và làm nổi bật (highlight) chính xác một đoạn văn bản chỉ định (text fragment) khi người dùng click vào link. Bài viết hướng dẫn chi tiết cách khai thác tính năng này.

5、[Tìm hiểu cơ chế hoạt động của giải pháp đa địa chỉ DNS (Round-Robin DNS)](https://blog.hyperknot.com/p/understanding-round-robin-dns) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024102705.webp)

Giải pháp Round-Robin DNS cho phép cấu hình gán nhiều địa chỉ IP máy chủ đích khác nhau cho cùng một tên miền duy nhất nhằm phục vụ phân tải lưu lượng (load balancing). Tác giả đã tiến hành các bài kiểm thử thực tế để đánh giá hiệu quả thực tế của giải pháp này.

6、[Tìm hiểu khái niệm cơ bản về mạng thần kinh nhân tạo Perceptron](https://medium.com/@vincentlambert0/it-all-started-with-a-perceptron-86bd0fb80b96) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024102908.webp)

Bài viết cơ bản giải thích dễ hiểu về khái niệm "Perceptron" (Tế bào thần kinh nhân tạo) — viên gạch đặt nền móng đầu tiên cấu thành nên các mạng thần kinh học sâu phức tạp hiện nay.

## 工具

1、[EasyTransfer](https://github.com/WCY-dt/EasyTransfer)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120701.webp)

Công cụ truyền tải tệp tin trực tuyến mã nguồn mở hỗ trợ mã hóa bảo mật đầu cuối, cho phép người dùng nhanh chóng kết nối và chia sẻ tệp tin ẩn danh giữa các thiết bị mà không cần đăng ký tài khoản. Ứng dụng được phát triển trên WebRTC và Vue.js. Trải nghiệm bản [Demo](https://file.ch3nyang.top). (Đóng góp từ [@ch3ny4ng](https://github.com/ruanyf/weekly/issues/5653))

2、[Screen Sharing](https://screensharing.net)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120702.webp)

Ứng dụng web tối giản hỗ trợ người dùng nhanh chóng chia sẻ màn hình máy tính của mình cho người khác trực tiếp trên trình duyệt mà không cần cài đặt thêm phần mềm bổ trợ. (Đóng góp từ [@markliuyuxiang](https://github.com/ruanyf/weekly/issues/5657))

3、[PMAtron](https://github.com/maskerprc/pmatron)

Dự án ứng dụng Electron để đóng gói công cụ quản trị cơ sở dữ liệu quen thuộc phpMyAdmin thành một phần mềm máy tính (Desktop App) chạy độc lập và đa nền tảng. (Đóng góp từ [@MaskerPRC](https://github.com/ruanyf/weekly/issues/5666))

4、[FastExcel](https://github.com/CodePhiliaX/fastexcel)

Thư viện hiệu năng cao viết bằng ngôn ngữ Java chuyên dụng hỗ trợ xử lý đọc ghi và trích xuất dữ liệu từ các tệp tin Excel lớn một cách nhanh chóng và tối ưu bộ nhớ. (Đóng góp từ [@JerryFan626](https://github.com/ruanyf/weekly/issues/5671))

5、[Readest](https://github.com/chrox/readest)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120703.webp)

Ứng dụng đọc sách điện tử (e-book reader) mã nguồn mở và đa nền tảng dành cho máy tính, được phát triển dựa trên bộ khung Next.js 15 kết hợp với Tauri v2. (Đóng góp từ [@chrox](https://github.com/ruanyf/weekly/issues/5663))

6、[IMG2AVIF](https://img2avif.com)

Công cụ trực tuyến tiện lợi hỗ trợ người dùng nhanh chóng chuyển đổi định dạng các tệp hình ảnh thông thường sang chuẩn nén hình ảnh chất lượng cao AVIF. (Đóng góp từ [@malagebidi](https://github.com/ruanyf/weekly/issues/5678))

7、[YT Pics](https://www.ytpics.com/)

Ứng dụng web tiện lợi: Người dùng chỉ cần cung cấp liên kết một video YouTube và chỉ định mốc thời gian cụ thể, hệ thống sẽ tự động chụp và kết xuất hình ảnh chất lượng cao tại đúng khung hình đó.

8、[Web2pdf](https://github.com/dvcoolarun/web2pdf)

Công cụ dòng lệnh mạnh mẽ hỗ trợ chuyển đổi nội dung từ một liên kết trang web bất kỳ sang định dạng tệp tin PDF, tích hợp các tùy chỉnh nâng cao như thay đổi CSS hiển thị hoặc tự động tạo mục lục.

9、[CheerpJ](https://labs.leaningtech.com/blog/cheerpj-3.0)

Giải pháp biên dịch máy ảo Java (JVM) chạy trực tiếp trên trình duyệt web, giúp các nhà phát triển có thể vận hành các ứng dụng viết bằng Java ngay trên trình duyệt mà không cần cài đặt JRE.

10、[fuzzy-search](https://github.com/m31coding/fuzzy-search)

Thư viện JavaScript hỗ trợ tìm kiếm mờ (fuzzy search) ở frontend, được tối ưu hóa tốt cho việc nhận diện các ký tự ngôn ngữ Đông Á.

## AI 相关

1、[BabelDuck](https://github.com/Orenoid/BabelDuck)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121002.webp)

Ứng dụng hỗ trợ học tập và thực hành giao tiếp nói ngoại ngữ trực tuyến ứng dụng trí tuệ nhân tạo. (Đóng góp từ [@Orenoid](https://github.com/ruanyf/weekly/issues/5669))

2、[AIGIF](https://aigif.net)

Công cụ tìm kiếm ảnh động GIF tích hợp tính năng AI cho phép người dùng thực hiện thay đổi khuôn mặt nhân vật trong ảnh động một cách tự nhiên. (Đóng góp từ [@markliuyuxiang](https://github.com/ruanyf/weekly/issues/5682))

3、[Imagenie](https://github.com/zhongweili/imagenie)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121206.webp)

Ứng dụng máy tính đa nền tảng hỗ trợ xử lý hình ảnh bằng AI ngoại tuyến (offline) ngay tại máy cục bộ, hỗ trợ các tính năng làm nét ảnh chân dung, nâng cao độ phân giải hoặc tự động xóa ảnh nền. (Đóng góp từ [@zhongweili](https://github.com/ruanyf/weekly/issues/5688))

## 资源

1、[Quy trình khởi động hệ thống: So sánh Android và Linux](https://xdaforums.com/t/info-boot-process-android-vs-linux.3785254/)

Bài viết phân tích chuyên sâu đối chiếu chi tiết chuỗi trình tự các bước khởi động hệ thống (boot process) của hai hệ điều hành Android và Linux.

2、[Cẩm nang thiết kế hệ thống tính sẵn sàng cao (High Availability)](https://www.thebyte.com.cn)

Tài liệu điện tử tiếng Trung chia sẻ miễn phí trực tuyến, hệ thống hóa toàn bộ các kiến thức nền tảng về mạng máy tính, điện toán đám mây, container (Docker), và kiến trúc cụm máy chủ (clusters). (Đóng góp từ [@isno](https://github.com/ruanyf/weekly/issues/5683))

3、[English News in Levels](https://englishnewsinlevels.com)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121207.webp)

Trang web học tiếng Anh qua tin tức thế giới được cập nhật hằng ngày. Mỗi bản tin đều được biên soạn lại thành 3 cấp độ từ vựng từ dễ đến khó đi kèm tệp âm thanh nghe bài đọc và các câu hỏi trắc nghiệm kiểm tra độ hiểu bài. (Đóng góp từ [@meterscao](https://github.com/ruanyf/weekly/issues/5699))

4、[GitHub Weekly](https://iohub.inshub.cn)

Trang web tổng hợp và hiển thị các sản phẩm công nghệ từ khu vực thảo luận của bản tin này dưới dạng các thẻ thông tin (news cards) trực quan và bắt mắt. (Đóng góp từ [@inshub](https://github.com/ruanyf/weekly/issues/5701))

## 图片

1、[Bí ẩn về bức ảnh căn phòng trống (The Backrooms)](https://archive.org/details/backrooms-original-footage)

Vào khoảng năm 2010, cộng đồng mạng Hoa Kỳ bắt đầu lan truyền rộng rãi một bức ảnh chụp một căn phòng trống trải mang màu sắc vô cùng huyền bí và cô độc.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024060904.webp)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024060905.webp)

Bức ảnh hoàn toàn không có bất kỳ dòng mô tả nào đi kèm, không ai biết nó được chụp ở đâu và do ai chụp.

Chính sự thiếu hụt thông tin này đã khơi gợi trí tưởng tượng phong phú của cư dân mạng: Một không gian mang ánh đèn vàng hiu hắt, lớp thảm sàn ẩm mốc cũ kỹ, những mảng tường vàng lạnh lẽo mở ra các lối đi vô tận không có cửa sổ, tạo cảm giác người xem bị giam cầm vĩnh viễn bên trong.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024060906.webp)

Qua các lượt chia sẻ rộng rãi, bức ảnh đã trở thành một biểu tượng kinh điển của văn hóa mạng Mỹ, trở thành nguồn cảm hứng thiết kế cho hàng loạt các tựa game và phim điện ảnh nổi tiếng (như *The Adjustment Bureau*, *Dark City*, hay *Cube*).

Mới đây, nhờ nỗ lực điều tra của tổ chức Lưu trữ Internet (Internet Archive), nguồn gốc thực tế của bức ảnh đã chính thức được làm sáng tỏ: Đây chỉ là bức ảnh chụp khu vực tầng hai của một cửa hàng đồ nội thất cũ đang trong quá trình cải tạo mặt bằng tại Mỹ vào năm 2002, và những căn phòng trống thực chất chính là các gian trưng bày sản phẩm cũ.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024060907.webp)

## 文摘

1、[Sự đồng điệu của thị hiếu thẩm mỹ đại chúng toàn cầu](https://www.alexmurrell.co.uk/articles/the-age-of-average)

Ý niệm thế nào là đẹp và thế nào là xấu của mỗi cá nhân thực ra chịu ảnh hưởng cực kỳ sâu sắc từ xã hội xung quanh, và rất ít người sở hữu một tiêu chuẩn thẩm mỹ hoàn toàn độc lập của riêng mình.

Vào đầu những năm 1990, hai nghệ sĩ người Nga đã thuê một công ty nghiên cứu thị trường tiến hành một cuộc khảo sát quy mô lớn trên 1.001 người Mỹ với danh sách các câu hỏi như sau:

> - Tông màu sắc yêu thích nhất của bạn là gì?
> - Bạn thích các đường nét thiết kế sắc sảo hay các đường cong mềm mại hơn?
> - Bạn yêu thích các nét vẽ trơn láng hay các nét cọ dày dặn?
> - Bạn thích các bức tranh vẽ nhân vật khỏa thân hay mặc trang phục chỉnh tề hơn?
> - Bạn thích hình ảnh người đang thư giãn hay đang làm việc hơn?
> - Bạn thích bối cảnh trong nhà hay ngoài trời hơn?
> - Bạn thích phong cảnh thiên nhiên như thế nào?

Sau khi thu thập xong kết quả, hai nghệ sĩ đã tiến hành vẽ nên một bức tranh đáp ứng đúng các tùy chọn của số đông người được khảo sát. Về mặt lý thuyết, tác phẩm này sẽ phải là bức tranh nhận được sự yêu thích nhất của đại bộ phận công chúng Mỹ.

Sau đó, họ tiếp tục mang bảng câu hỏi này đi khảo sát tại nhiều quốc gia khác trên thế giới và thu được một kết quả kinh ngạc: Thị hiếu thẩm mỹ đại chúng của hầu hết các quốc gia đều đạt độ tương đồng đến khó tin.

> "Mọi người trên thế giới đều mong muốn một bức tranh phong cảnh thiên nhiên, có vài nhân vật xuất hiện, phía tiền cảnh có động vật và tông màu chủ đạo bao trùm là màu xanh lam."

Hai nghệ sĩ đã vẽ nên 11 bức tranh dựa trên kết quả khảo sát của 11 quốc gia khác nhau, và khi đặt cạnh nhau, 11 bức tranh này trông hầu như không có sự khác biệt rõ rệt.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032914.webp)

Kết quả nghiên cứu chứng minh thị hiếu thẩm mỹ đại chúng toàn cầu đang ngày một đồng hóa mạnh mẽ. Từ điện ảnh, thời trang, kiến trúc cho đến quảng cáo, con người ở các quốc gia khác nhau đang có xu hướng yêu thích những thứ tương tự nhau, tính độc bản văn hóa ngày một suy giảm.

Ví dụ dễ thấy nhất là thiết kế nội thất của các căn hộ cho thuê trên Airbnb hiện nay: Dù bạn đặt phòng ở bất kỳ quốc gia nào, phong cách decor của chúng cũng đều mang một nét tương đồng kỳ lạ (được gọi là thẩm mỹ Airbnb): những mảng tường trắng tinh, đồ gỗ tự nhiên, máy pha cà phê viên nén, ghế tựa lưng, những mảng tường gạch trần, kệ gỗ treo tường và bóng đèn dây tóc trang trí.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032915.webp)

Phong cách thẩm mỹ Airbnb này là sự kết hợp khéo léo giữa nét mộc mạc thô ráp của chủ nghĩa công nghiệp và nét thanh lịch tối giản của phong cách cổ điển.

Xu hướng thẩm mỹ này nhanh chóng lan rộng và ảnh hưởng sâu sắc đến cả ngành thiết kế quán cà phê.

Các quán cà phê và nhà hàng trên khắp thế giới hiện nay cũng đang dần trở nên giống nhau: những chiếc bàn gỗ thô mộc, hệ thống cửa sổ kính lớn ngập tràn ánh sáng và những chiếc đèn thả tối giản.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032916.webp)

Tóm lại, sự phổ cập của mạng Internet kết nối toàn cầu đang định hình nên một quy chuẩn thẩm mỹ đại chúng thống nhất. Trong tương lai, dù bạn có đi du lịch đến bất kỳ quốc gia nào, các quán cà phê hay khách sạn bạn ghé thăm rất có thể cũng sẽ sở hữu phong cách thiết kế nội thất y hệt nhau.

## 言论

1、

Quy trình giúp tôi gặt hái được những thành công trong cuộc sống đều tuân theo chuỗi 4 bước sau:

(1) Tôi dành sự tập trung tối đa cho những lĩnh vực mà bản thân thực sự yêu thích.

(2) Tôi tìm kiếm mọi phương pháp để có thể làm công việc đó nhiều hơn hằng ngày.

(3) Tôi chủ động chia sẻ để những người có cùng chí hướng dễ dàng nhận biết công việc tôi đang làm.

(4) Tôi chủ động kết nối và hợp tác cùng họ triển khai các dự án thực tế.

-- [Henrik Karlsson](https://www.henrikkarlsson.xyz/p/unfolding)

2、

Những nhà khoa học vĩ đại luôn sở hữu những ý tưởng vô cùng táo bạo, nhưng đồng thời họ cũng luôn duy trì một thái độ phản biện cực kỳ khắt khe đối với chính ý tưởng của mình. Trước khi chấp nhận một giả thuyết do mình đặt ra, họ sẽ tìm đủ mọi cách để tự chứng minh giả thuyết đó là sai trước.

Chỉ khi nào họ không thể tìm ra lập luận bác bỏ được giả thuyết đó, họ mới tin tưởng nhận định của mình là chính xác.

-- [Karl Popper](https://igorpak.wordpress.com/2020/12/10/what-if-they-are-all-wrong/), nhà triết học khoa học nổi tiếng

3、

Là một kỹ sư phần mềm đã từng tham gia phát triển các dự án thương mại bằng hơn 10 ngôn ngữ lập trình khác nhau, tôi hoàn toàn không đồng ý với quan điểm cho rằng ngôn ngữ lập trình này giúp viết code nhanh hơn ngôn ngữ lập trình kia.

Tốc độ lập trình thực tế phụ thuộc hoàn toàn vào năng lực cá nhân của mỗi kỹ sư. Ngôn ngữ nào phù hợp nhất với kinh nghiệm thực tế và thói quen tư duy của lập trình viên đó sẽ giúp họ viết mã nguồn nhanh nhất.

-- [Ý kiến độc giả trên diễn đàn Hacker News](https://news.ycombinator.com/item?id=41616851)

4、

Tôi từng giữ quan niệm lâu năm rằng Trái Đất là một "hành tinh nước" do bề mặt của nó được bao phủ bởi những đại dương bao la.

Cho đến khi tôi thực hiện các phép tính toán học thực tế và nhận ra Trái Đất thực chất chỉ là một khối đá khô cằn bay giữa vũ trụ, và lượng nước trên bề mặt của nó chỉ mỏng tương đương với việc bạn dùng bình xịt phun sương vài lần lên bề mặt của một quả bóng bowling mà thôi.

-- [Ý kiến độc giả trên diễn đàn Hacker News](https://news.ycombinator.com/item?id=41238102)

## 往年回顾

[Tìm hiểu về các chính sách định hướng phát triển hạ tầng công nghệ thế hệ mới](https://www.ruanyifeng.com/blog/2023/10/weekly-issue-282.html) (2023 #282)

[Đánh giá và giới thiệu các phần mềm thiết kế đồ họa 2D chất lượng](https://www.ruanyifeng.com/blog/2022/11/weekly-issue-232.html) (2022 #232)

[Bàn về những rủi ro tài chính đằng sau các chiến dịch khuyến mãi cho người dùng mới](https://www.ruanyifeng.com/blog/2021/11/weekly-issue-182.html) (2021 #182)

[Bàn về khái niệm năng lực phản ứng nhanh (Fast) và năng lực tích lũy sâu (Slow)](https://www.ruanyifeng.com/blog/2020/11/weekly-issue-132.html) (2020 #132)

(Hết)
