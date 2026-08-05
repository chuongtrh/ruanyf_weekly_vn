# 科技爱好者周刊：第 82 期 (Bản tin chia sẻ công nghệ số 82)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110813.jpg)

Ảnh bìa: Ngày 2/11, thủ đô New Delhi của Ấn Độ ghi nhận tình trạng ô nhiễm không khí cực kỳ nghiêm trọng, chỉ số chất lượng không khí PM 2.5 (AQI) vượt ngưỡng 900.

## 刊首语 (Lời tựa)

Tuần này tôi muốn giới thiệu [một bài viết](https://erikbern.com/2019/09/12/misc-unsolicited-career-advice.html) của một kỹ sư phần mềm cao cấp người Mỹ chia sẻ về cách lựa chọn định hướng nghề nghiệp.

Tác giả vốn xuất thân là một người ngoại đạo, nhưng nhờ sự nỗ lực bền bỉ, anh đã gia nhập một công ty chuyên về học máy (Machine Learning) và hiện tại đang có sự phát triển sự nghiệp rất tốt. Từ trải nghiệm thực tế của bản thân, anh đúc kết ra một quan điểm: **Khi tìm kiếm việc làm, hãy luôn ưu tiên lựa chọn những ngành công nghiệp đang có tốc độ tăng trưởng nhanh nhất.**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111413.jpg)

> Việc gia nhập những công ty đang ở trạng thái bão hòa hoặc phát triển chậm chạp thực chất là một trò chơi có tổng bằng không (zero-sum game).
> 
> Nếu bạn muốn thăng tiến, bạn bắt buộc phải chờ đợi những người ở vị trí trên nghỉ việc hoặc chuyển đi để trống chỗ. Thứ bạn nhận được chắc chắn là thứ mà người khác vừa mất đi. Ngược lại, tại những doanh nghiệp đang tăng trưởng thần tốc, số lượng nhân sự mới liên tục gia nhập giúp quy mô công ty mở rộng, kết quả là hầu như tất cả mọi người đều có cơ hội thăng tiến lên các nấc thang mới!
> 
> Quan trọng hơn cả, tốc độ phát triển của hoạt động kinh doanh luôn nhanh hơn tốc độ tuyển dụng nhân sự, điều này sẽ tạo ra một lực đẩy vô hình "kéo bạn đi lên" các vị trí quản lý cao hơn.

Tác giả lấy chính câu chuyện của mình làm minh chứng: anh vốn không có nền tảng chuyên môn sâu về học máy, nhưng do doanh nghiệp mở rộng quy mô quá nhanh, anh bắt buộc phải đứng ra xây dựng và quản lý đội ngũ kỹ sư mới, từ đó nghiễm nhiên trở thành quản lý cấp trung. Chính môi trường tăng trưởng nhanh đã "kéo" anh lên một vị trí cao hơn, mang lại nhiều cơ hội và tài nguyên hơn.

Điều này khiến tôi liên tưởng đến môi trường đại học tôi từng công tác trước đây. Hàng năm, chỉ tiêu xét duyệt thăng chức giáo sư và phó giáo sư của trường là cực kỳ hạn chế. Mọi người phải cạnh tranh gay gắt, nếu năm nay trượt thì bắt buộc phải chờ ít nhất một năm nữa. Có những giảng viên cống hiến đến bạc cả mái đầu mới được phong học hàm phó giáo sư. Đó chính là hệ quả của một hệ thống phát triển chậm chạp. Lựa chọn cống hiến ở những nơi như vậy thực sự là một sự lãng phí thanh xuân.

Bài viết cũng đề cập đến một luận điểm khác mà tôi rất đồng tình: Mục đích cốt lõi của công việc thời trẻ là để tích lũy hai loại vốn: vốn năng lực (Human Capital) và vốn tài chính (Financial Capital). Đối với những người trẻ tuổi, vốn năng lực đóng vai trò quan trọng hơn rất nhiều. **Khi tìm việc, ưu tiên hàng đầu của người trẻ phải là tốc độ gia tăng vốn năng lực của bản thân.** Bởi xét về dài hạn, vốn năng lực sẽ mang lại tỷ suất sinh lời vượt trội hơn nhiều so với vốn tài chính.

Phương pháp nhanh nhất để tích lũy vốn năng lực là gia nhập những môi trường tập trung nhiều người thông minh, học hỏi trực tiếp từ những người giỏi hơn bạn. Làm việc cùng các chuyên gia hàng đầu sẽ giúp bạn trưởng thành với tốc độ chóng mặt. Dù các tập đoàn lớn có rất nhiều nhân tài, nhưng nếu bạn không được trực tiếp làm việc tương tác cùng họ thì cũng vô ích. **Gia nhập một đội ngũ tinh gọn gồm những người thông minh trong một ngành công nghiệp đang tăng trưởng nhanh chính là công thức tối ưu nhất cho sự thành công.**

## Khóa học miễn phí dành cho Kiến trúc sư Frontend

Nền tảng đào tạo công nghệ Kaikeba mới đây đã ra mắt chương trình học miễn phí mang tên **《Con đường thăng tiến của Kiến trúc sư Frontend》** dành tặng cộng đồng.

Giảng viên đứng lớp là anh Đại Thánh - cựu kiến trúc sư frontend tại Baidu và Qihoo 360 với hơn 8 năm kinh nghiệm lập trình thực chiến.

Nội dung chương trình tập trung chia sẻ: (1) Hành trình cá nhân của giảng viên từ một lập trình viên thông thường vươn lên thành kiến trúc sư full-stack tại Baidu và 360, cùng các bí quyết vượt qua vòng phỏng vấn kỹ thuật của các tập đoàn lớn (BAT); (2) Phương pháp tự học công nghệ hệ thống và lập kế hoạch phát triển bản thân khoa học để tránh đi đường vòng; (3) Phân tích môi trường làm việc, văn hóa doanh nghiệp và mặt bằng thu nhập thực tế của các nhóm công ty công nghệ khác nhau; (4) Các bài học kinh nghiệm thực tế giúp lập trình viên frontend nhanh chóng bứt phá giới hạn năng lực và xây dựng lộ trình thăng tiến sự nghiệp rõ ràng.

Khóa học rất phù hợp cho các lập trình viên mới vào nghề hoặc đã có từ 1 đến 3 năm kinh nghiệm nhưng đang thiếu phương pháp làm việc khoa học và hệ thống tri thức bài bản để tiết kiệm thời gian tự học.

Độc giả quan tâm có thể quét mã QR WeChat dưới đây để nhận khóa học. **Chương trình quà tặng đợt này giới hạn chỉ 499 suất miễn phí**:

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111301.jpg)

## 资讯 (Tin tức)

1. **Sự dịch chuyển từ xe xăng sang xe điện đe dọa sự tồn tại của hệ thống trạm xăng truyền thống tại Mỹ**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100505.jpg)

Sự phổ cập nhanh chóng của phương tiện chạy điện tại Mỹ đang làm sụt giảm mạnh nhu cầu tiêu thụ xăng dầu, ảnh hưởng trực tiếp đến hoạt động kinh doanh của các trạm xăng. Nhiều chủ trạm xăng đã buộc phải chuyển đổi một phần mặt bằng làm điểm nhận hàng ký gửi của Amazon (ảnh trên) hoặc liên kết mở cửa hàng tiện lợi, đồ ăn nhanh.

Dự báo lượng tiêu thụ xăng dầu tại Mỹ sẽ bắt đầu đi xuống rõ rệt từ giai đoạn 2025-2027. Nếu không chủ động chuyển đổi mô hình kinh doanh sang tích hợp trạm sạc điện, ước tính khoảng 60% đến 80% trạm xăng truyền thống sẽ phải đóng cửa vào năm 2035.

Thực tế số lượng trạm xăng tại Mỹ đã liên tục suy giảm từ mức khoảng 200.000 trạm trong thập niên 1990 xuống còn khoảng 135.000 trạm hiện nay. Dưới đây là ý tưởng thiết kế trạm sạc điện tự động dành cho các dòng xe tự lái trong tương lai:

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100506.jpg)

2. **Paper Phone - Ý tưởng in thông tin điện thoại ra giấy của Google giúp giảm sự phụ thuộc vào màn hình**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110304.jpg)

Điện thoại thông minh ngày càng chiếm lĩnh nhiều thời gian và khiến con người lệ thuộc vào chúng. Nhằm giúp người dùng cai nghiện màn hình điện thoại mà vẫn không bỏ lỡ các công việc quan trọng, Google triển khai dự án thử nghiệm mang tên *Paper Phone*.

Hãng phát triển một ứng dụng Android cho phép người dùng tick chọn các thông tin thiết yếu cần dùng trong ngày (như danh bạ quan trọng, lịch hẹn, sơ đồ đường đi bản đồ, ghi chú ghi nhớ). Ứng dụng sẽ tự động dàn trang và in toàn bộ thông tin này ra một tờ giấy A4 duy nhất được gấp gọn. Người dùng chỉ cần mang theo tờ giấy này bên mình suốt cả ngày mà không cần phải liên tục mở màn hình điện thoại.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110305.jpg)

3. **Cải tiến tuổi thọ công trình bê tông cốt thép bằng công nghệ sợi thủy tinh và sợi carbon**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110401.jpg)

Các công trình kiến trúc bê tông cốt thép hiện đại thường có niên hạn sử dụng thực tế dao động từ 60 đến 100 năm. Nguyên nhân chính là do cấu trúc bê tông xuất hiện các vết nứt chân chim theo thời gian, tạo điều kiện cho nước và oxy lọt vào gây rỉ sét phần cốt thép bên trong. Lõi thép rỉ sét sẽ trương nở thể tích làm nứt vỡ bê tông từ bên trong làm suy giảm nghiêm trọng khả năng chịu lực của công trình.

Các nhà nghiên cứu Úc đề xuất giải pháp thay thế lõi thép truyền thống bằng các thanh chịu lực làm từ sợi thủy tinh và sợi carbon siêu bền không bị oxy hóa. Mặc dù chi phí vật liệu ban đầu cao hơn, giải pháp này giúp loại bỏ hoàn toàn nguy cơ rỉ sét, kéo dài tuổi thọ công trình lên hàng trăm năm mà không tốn chi phí bảo trì.

Hướng nghiên cứu tiếp theo là ứng dụng đá bazan nấu chảy ép thành sợi bazan để sản xuất thanh cốt sợi composite giúp hạ giá thành sản xuất và thân thiện hơn với môi trường so với sợi carbon.

4. **Tranh cãi quanh việc ứng dụng thiết bị vòng đeo trán cảm biến sóng não học đường tại Trung Quốc**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110402.jpg)

Truyền thông đưa tin về một trường tiểu học tại Kim Hoa (Zhejiang) thử nghiệm cho học sinh đeo các thiết bị vòng đeo trán cảm biến sóng não (EEG) trong giờ học. Thiết bị có khả năng đo đạc các tín hiệu điện não để phân tích mức độ tập trung của học sinh khi nghe giảng hoặc làm bài tập, đồng thời gửi báo cáo kết quả theo thời gian thực về máy tính của giáo viên và nhóm chat của phụ huynh.

Thiết bị do một doanh nghiệp công nghệ tại Thâm Quyến phát triển và được cựu học sinh thành đạt tài trợ cho nhà trường. Đơn vị phát triển khẳng định mục tiêu của thiết bị không phải để giám sát học sinh mà là công cụ hỗ trợ rèn luyện khả năng tự tập trung (neurofeedback) cho trẻ. Thiết bị cảm biến sóng não này trước đó đã được ứng dụng thử nghiệm tại một số trường trung học ở Boston (Mỹ) và các lớp học hè của Đại học Yale.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110404.jpg)

5. **Giải mã lý do pháp lý và kế toán giúp tập đoàn Amazon hợp pháp hóa việc không phải nộp thuế thu nhập**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110901.jpg)

Mặc dù ghi nhận mức lợi nhuận kỷ lục lên tới 11 tỷ USD vào năm 2018, gã khổng lồ thương mại điện tử Amazon hoàn toàn không phải đóng một đồng thuế thu nhập doanh nghiệp liên bang nào tại Mỹ một cách hợp pháp.

Thực tế này bắt nguồn từ hai cơ chế ưu đãi thuế của luật pháp Mỹ: Thứ nhất, doanh nghiệp được phép khấu trừ thuế đối với toàn bộ phần lợi nhuận được tái đầu tư vào hoạt động nghiên cứu phát triển (R&D) và xây dựng hạ tầng. Thứ hai, luật pháp cho phép doanh nghiệp tính phần chênh lệch giá trị cổ phiếu thưởng phát cho nhân viên làm chi phí hoạt động của doanh nghiệp để giảm trừ thuế. Trong bối cảnh giá cổ phiếu Amazon tăng vọt năm 2018 mang lại khoản lợi nhuận lớn cho nhân viên nắm giữ quyền chọn, phần giá trị này được Amazon hạch toán làm chi phí để khấu trừ toàn bộ nghĩa vụ thuế thu nhập.

6. **Tin vắn**

- Thống kê của Cục điều tra dân số Mỹ cho biết thời gian đi làm (commute time) trung bình của người dân Mỹ năm 2018 đạt mức kỷ lục 27 phút, trong đó khoảng 10% người dân mất hơn 60 phút di chuyển mỗi lượt đi làm.

- Tập đoàn SoftBank (Nhật Bản) ghi nhận khoản lỗ vận hành kỷ lục theo quý lên tới 6.5 tỷ USD, chủ yếu do sự sụt giảm định giá nghiêm trọng của hai khoản đầu tư lớn vào Uber và startup không gian làm việc chung WeWork sau khi IPO thất bại.

- Một hãng phim Hollywood công bố dự án phim mới khởi công vào năm sau sẽ sử dụng công nghệ đồ họa máy tính CGI để tái tạo chân dung cố diễn viên huyền thoại James Dean (đã qua đời năm 1954 từ tai nạn xe hơi) làm nhân vật nam chính cho bộ phim.

- Bức ảnh chụp hiện tượng Sao Thủy đi qua đĩa Mặt Trời (Mercury transit) diễn ra ngày 11/11 ghi lại hình ảnh Sao Thủy như một chấm đen nhỏ di chuyển cắt ngang bề mặt Thái Dương (ảnh dưới).

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111211.jpg)

## 文章 (Bài viết)

1、[Bài viết] [Con đường thăng tiến職 cấp dành cho kỹ sư phần mềm chuyên nghiệp](https://blog.pragmaticengineer.com/software-engineering-promotions/) (Tiếng Anh)

Chia sẻ các bài học kinh nghiệm và quy trình xét duyệt thăng tiến chức danh kỹ sư phần mềm (từ Junior lên Senior và Staff Engineer) tại các tập đoàn công nghệ lớn: những kỹ năng cần chứng minh bên cạnh năng lực viết code đơn thuần.

2、[Bài viết] [Giải nghĩa trực quan về thuật toán mã hóa đường cong Elliptic (ECC)](https://fangpenlin.com/posts/2019/10/07/elliptic-curve-cryptography-explained/) (Tiếng Anh)

Tác giả lược bỏ toàn bộ các công thức toán học đại số phức tạp để tập trung giải thích bản chất hình học của thuật toán mã hóa đường cong Elliptic - nền tảng của các hệ thống chữ ký số và bảo mật HTTPS hiện đại.

3、[Bài viết] [Timsort - Thuật toán sắp xếp tốc độ cao mặc định ẩn mình bên trong Python và Java](https://skerritt.blog/timsort-the-fastest-sorting-algorithm-youve-never-heard-of/) (Tiếng Anh)

Giới thiệu về thuật toán sắp xếp lai Timsort (kết hợp giữa Merge Sort và Insertion Sort) được tối ưu hóa cực tốt cho các dữ liệu thực tế đã có sẵn một phần trật tự, hiện đang là thuật toán sắp xếp mặc định của ngôn ngữ Python và công cụ Java V8.

## 软件 (Phần mềm)

1、[Apache Guacamole — Cổng kết nối máy tính từ xa (Remote Desktop Gateway) chạy trực tiếp trên nền trình duyệt](https://guacamole.apache.org/)

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100712.jpg)

Giải pháp mã nguồn mở cho phép người dùng truy cập và điều khiển máy tính từ xa (hỗ trợ các giao thức VNC, RDP, SSH) trực tiếp trên trình duyệt web hỗ trợ HTML5 mà không cần cài thêm plugin hay client chuyên dụng.

2、[HTTP Toolkit — Công cụ giám sát, đánh chặn và giả lập (Mock) dữ liệu yêu cầu HTTP/HTTPS](https://httptoolkit.tech/mock/)

Giúp các nhà phát triển dễ dàng gỡ lỗi mạng: tự động đánh chặn toàn bộ request gửi đi từ trình duyệt hoặc ứng dụng di động, phân tích chi tiết header/body và viết luật giả lập phản hồi của server để test các tình huống lỗi.

3、[imgproxy — Dịch vụ proxy xử lý, định dạng lại kích thước hình ảnh tốc độ cao viết bằng Go](https://github.com/imgproxy/imgproxy)

Giải pháp tối ưu hiệu năng xử lý ảnh tĩnh cho các hệ thống web lớn: tự động tải ảnh gốc từ bộ chứa đám mây, thực hiện crop, resize và nén định dạng (như WebP) theo các tham số truyền trên đường dẫn rồi lưu cache để phân phối tốc độ cao.

4、[AltStore — Cửa hàng ứng dụng thay thế (Alternative App Store) cho hệ điều hành iOS không cần jailbreak](https://9to5mac.com/2019/09/25/altstore-is-an-ios-app-store-alternative-that-doesnt-require-a-jailbreak-heres-how-to-use-it/)

Giải pháp cài đặt các ứng dụng ngoài (sideload) cho thiết bị iPhone/iPad thông qua việc tận dụng chứng chỉ nhà phát triển cá nhân của Apple mà không yêu cầu bẻ khóa hệ thống (jailbreak).

5、[GitHub Mobile — Ứng dụng di động chính thức từ nền tảng GitHub](https://github.com/mobile)

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111401.jpg)

Lần đầu tiên GitHub phát hành ứng dụng di động chính thức hỗ trợ các lập trình viên theo dõi thông báo, duyệt code, xử lý các issue và phê duyệt Pull Request (PR) nhanh chóng ngay trên điện thoại di động (phiên bản iOS phát hành trước, Android ra mắt sau).

## 资源 (Tài nguyên)

1、[Tài liệu] [Tài liệu học tập ảo hóa container LXC từ nhà phát triển cốt lõi](https://stgraber.org/2013/12/20/lxc-1-0-blog-post-series/) (Tiếng Anh)

Chuỗi bài viết chuyên sâu giới thiệu về công nghệ ảo hóa container LXC (Linux Containers) - nền tảng đặt nền móng cho sự phát triển của Docker sau này, giúp lập trình viên hiểu sâu về các cơ chế cô lập tài nguyên hạt nhân Linux (namespaces, cgroups).

2、[Trang web] [Pháp Tín - Công cụ tra cứu hệ thống văn bản quy phạm pháp luật Trung Quốc](http://www.faxin.cn/keyword/index.aspx)

Cơ sở dữ liệu luật pháp chính quy hỗ trợ tìm kiếm nhanh các điều luật, tiền lệ pháp lý và các văn bản hướng dẫn tố tụng tòa án dành cho giới luật sư và các doanh nghiệp trong nước.

## 图片 (Hình ảnh)

1. **Vòng đời phát triển kỳ diệu của loài bướm珍 hiếm qua ống kính nhà sinh học**

Nhà sinh học Tim Wong thực hiện dự án nhân giống bảo tồn dòng bướm đuôi kiếm Battus philenor quý hiếm tại vườn nhà đã ghi lại chi tiết các cột mốc sinh trưởng: từ khi bướm mẹ đẻ trứng đỏ lên kẽ lá rồi chết đi, trứng nở thành sâu bướm phàm ăn, sâu hóa nhộng bọc kén và sau cùng lột xác thành chú bướm rực rỡ sắc màu.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091610.jpg)

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091612.jpg)

2. **Thiết kế cầu sinh thái (Eco-Link) dành riêng cho động vật hoang dã vượt cao tốc an toàn**

Singapore và Hà Lan đi đầu thế giới trong việc xây dựng các cây cầu sinh thái phủ đầy cây xanh bắc ngang qua các tuyến đường cao tốc chạy xuyên rừng để tạo lối đi tự nhiên an toàn cho các loài thú hoang dã di chuyển, giảm thiểu tai nạn giao thông.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019092003.jpg)

Hà Lan hiện là quốc gia sở hữu số lượng cầu vượt sinh thái cho động vật nhiều nhất thế giới với hơn 30 cây cầu quy mô lớn.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019092006.jpg)

## 文摘 (Văn trích)

1. **Khám phá y học về muối Lithium - Liều thuốc xoa dịu tâm thần từng hiện diện trong lon nước ngọt 7 Up**

Nhà y học người Úc John Cade là người đầu tiên phát hiện ra đặc tính xoa dịu tâm thần kỳ diệu của nguyên tố Lithium đối với các bệnh nhân mắc chứng hưng trầm cảm (bipolar disorder). Ngày nay, Lithium được ví như chất kháng sinh penicillin của ngành tâm thần học - dòng thuốc đặc trị đầu tiên có hiệu quả thực tế rõ rệt.

John Cade sinh năm 1912 trong gia đình có cha làm bác sĩ tại bệnh viện tâm thần nên từ nhỏ anh đã tiếp xúc với các bệnh nhân. Ông luôn tin rằng bản chất của chứng tâm thần phân liệt và hưng cảm bắt nguồn từ sự mất cân bằng sinh hóa trong não bộ chứ không phải do chấn thương tâm lý như thuyết phân tâm học của Freud mô tả.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100501.jpg)

Trong các thử nghiệm, ông phát hiện việc tiêm muối Lithium giúp các chú chuột thí nghiệm trở nên vô cùng điềm tĩnh. Sau khi tự mình uống thử Lithium để kiểm tra độ an toàn, năm 1949 ông công bố bài báo khoa học chứng minh Lithium giúp cắt nhanh cơn hưng cảm của bệnh nhân.

Tuy nhiên do Lithium là khoáng chất tự nhiên đơn giản không thể đăng ký bằng sáng chế độc quyền, các hãng dược phẩm lớn nhận định sản phẩm không mang lại lợi nhuận thương mại cao nên từ chối đầu tư sản xuất quy mô lớn. Phải mất nhiều thập kỷ thử nghiệm lâm sàng độc lập, FDA mới chính thức phê duyệt đưa Lithium vào danh mục thuốc điều trị chính thức, giúp cứu sống hàng vạn bệnh nhân trầm cảm và giảm thiểu tỷ lệ tự sát.

Thực tế trước khi được y học chứng minh, muối Lithium đã âm thầm hiện diện trong đời sống. Lon nước ngọt có ga nổi tiếng phát hành năm 1929 mang tên *7 Up* (Thất Hỷ) ban đầu có chứa thành phần Citrate Lithium để tạo cảm giác sảng khoái, giảm căng thẳng cho người uống. Thành phần này sau đó đã được nhà sản xuất loại bỏ vào năm 1948 trước khi dòng nước ngọt này phổ biến toàn cầu.

## 言论 (Danh ngôn)

1、

> "Để chứng minh vai trò vượt trội của mình so với các kho tài nguyên thông tin trên mạng internet, nhiều thư viện đại học ngày nay đang đổ rất nhiều ngân sách vào việc cải tạo kiến trúc nội thất lộng lẫy hoặc trang bị các công nghệ thời thượng như máy in 3D. Tuy nhiên, các khảo sát thực tế cho thấy thứ sinh viên thực sự cần nhất ở thư viện lại cực kỳ đơn giản: một không gian yên tĩnh tuyệt đối để tự học, dịch vụ in ấn luận văn giá rẻ và kho sách giấy phong phú để tra cứu."
> 
> -- Trích bài viết *Sinh viên chỉ cần những thư viện truyền thống đơn giản*

(Hết)
