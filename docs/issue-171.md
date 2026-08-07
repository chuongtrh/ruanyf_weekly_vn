# 科技爱好者周刊（第 171 期）：云服务流量有多贵？

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1870) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080213.jpg)

Hình ảnh cận cảnh các cánh quạt khổng lồ của tuabin gió đang được vận chuyển lên đỉnh núi lộng gió tại thành phố Bình Hương, tỉnh Giang Tây. (Nguồn: [WeChat](https://mp.weixin.qq.com/s/KDyJcFWBrtTR3HS2PfT_aQ))

## 主带话题：Chi phí băng thông đám mây đắt đỏ đến mức nào?

Tháng trước, trang blog chính thức của Cloudflare đã đăng tải một bài viết hiếm hoi của CEO chỉ trích gay gắt chính sách tính phí lưu lượng dữ liệu (data egress fees) đắt đỏ một cách bất hợp lý của AWS (Amazon Web Services).

Hôm nay chúng ta sẽ cùng phân tích xem chi phí băng thông của các dịch vụ đám mây thực tế đắt đỏ đến mức độ nào.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080801.jpg)

Amazon hiện là nhà cung cấp dịch vụ điện toán đám mây lớn nhất thế giới, cung cấp mọi hạ tầng mạng cốt lõi. Bất kỳ ai từng sử dụng AWS đều biết rằng trong hóa đơn thanh toán hàng tháng, chi phí phần cứng (như CPU, RAM, dung lượng ổ cứng) chỉ chiếm một phần nhỏ, còn chi phí lưu lượng truyền tải dữ liệu (data egress) mới là phần chiếm tỷ trọng lớn nhất và đắt đỏ nhất.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080802.jpg)

Chi phí này đắt đỏ ra sao? Theo tính toán của Cloudflare dựa trên mức giá băng thông bán sỉ (wholesale price) thực tế tại các trung tâm dữ liệu, mức phí lưu lượng dữ liệu mà AWS thu từ người dùng tại khu vực Bắc Mỹ và châu Âu cao gấp **80 lần** so với giá bán sỉ!

Cụ thể, giá bán sỉ băng thông tại cổng trung tâm dữ liệu chỉ khoảng 0,08 USD cho mỗi 1 Mbps, nhưng khi qua tay AWS bán lại cho các nhà phát triển, mức giá lập tức vọt lên tới 6,37 USD! (Chúng ta sẽ giải thích công thức quy đổi giữa băng thông Mbps và lưu lượng dữ liệu GB ở phần dưới).

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080803.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081017.jpg)

Hãy cùng làm một bài toán nhỏ để xem chi phí để vận hành một trang web quy mô nhỏ trên hạ tầng của AWS sẽ tốn bao nhiêu tiền hàng tháng.

Giả sử trang web của bạn nhận được lượng truy cập trung bình khoảng 2.500 lượt xem trang (pageviews) mỗi ngày, dung lượng trung bình của mỗi trang web là 2 MB (bao gồm mã nguồn, hình ảnh, CSS, JS). Như vậy, lượng dữ liệu truyền tải mỗi ngày là 5 GB, tương đương khoảng 150 GB lưu lượng dữ liệu mỗi tháng.

Sử dụng công cụ tính giá chính thức của AWS (AWS Pricing Calculator), chúng ta chọn cấu hình phần cứng tối thiểu cho một máy chủ ảo EC2 và nhập thông số lưu lượng truyền tải đi là 150 GB/tháng.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081018.jpg)

Kết quả tính toán cho thấy hóa đơn hàng tháng sẽ rơi vào khoảng 16,31 USD (tương đương khoảng 380.000 VND), trong đó riêng chi phí truyền dữ liệu (data transfer) đã chiếm tới 13,41 USD. Như vậy, chỉ để chạy một trang web cực kỳ nhỏ, bạn phải chi trả tới hơn 4 triệu VND mỗi năm. Nếu lượng truy cập tăng gấp 10 lần lên mức 1.500 GB/tháng (vẫn là một trang web quy mô nhỏ), chi phí này sẽ tăng vọt lên thành hàng chục triệu VND mỗi năm.

Một trường hợp thực tế dở khóc dở cười được chia sẻ bởi một nhà phát triển: Hóa đơn hàng tháng thông thường cho server của anh chỉ ở mức 23,00 USD, nhưng sau một đêm thức dậy, anh bàng hoàng nhận được thông báo hóa đơn nợ lên tới 2.657,68 USD do trang web bất ngờ phát sinh lưu lượng dữ liệu khổng lồ ngoài ý muốn.

Cần lưu ý rằng chính sách phí băng thông đắt đỏ này không chỉ là đặc sản của riêng Amazon. Google Cloud cũng thu mức phí tương đương khoảng 16,73 USD/tháng cho cùng một cấu hình trang web (với 12,75 USD tiền băng thông). Các nhà cung cấp đám mây nội địa của Trung Quốc như Alibaba Cloud hay Tencent Cloud cũng áp dụng mức giá tương tự.

Tuy nhiên, các nhà cung cấp đám mây tại Trung Quốc có một điểm cộng là hỗ trợ lựa chọn thanh toán theo băng thông cố định (bandwidth pricing mode) thay vì tính theo lưu lượng thực tế. Lựa chọn này giúp ngăn ngừa hoàn toàn nguy cơ hóa đơn tăng vọt không kiểm soát, vì khi lượng truy cập vượt quá giới hạn băng thông đã mua, server sẽ chỉ phản hồi chậm hoặc từ chối kết nối mới chứ không tính thêm tiền. (Băng thông 1 Mbps hoạt động 100% công suất liên tục trong 1 tháng tương đương với khoảng 328 GB lưu lượng dữ liệu truyền tải. Giả sử hiệu suất sử dụng trung bình thực tế đạt 20%, để đáp ứng 150 GB lưu lượng/tháng bạn cần mua gói băng thông khoảng 2,3 Mbps).

Kết luận rút ra là: Các trang web nhỏ tốt nhất không nên host trực tiếp trên hạ tầng của các ông lớn đám mây toàn cầu nếu không có nguồn ngân sách dồi dào để chi trả cho hóa đơn băng thông. Nếu bắt buộc phải sử dụng, hãy tận dụng tối đa các giải pháp bộ nhớ đệm CDN để giảm tải tối đa lượng dữ liệu truyền trực tiếp từ máy chủ gốc.

## Thực chiến phát triển công cụ Front-end No-Code/Low-Code

Mới đây, dịch vụ tạo trang web không cần viết code (no-code site builder) Bubble.io đã công bố gọi vốn thành công 100 triệu USD vòng Series A, cho thấy xu hướng phát triển các công cụ Low-Code/No-Code đang ngày càng thu hút sự quan tâm của giới đầu tư công nghệ trên toàn cầu.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081201.jpg)

Triển vọng của Low-Code và No-Code giúp mở rộng tệp người dùng không chuyên tiếp cận công nghệ nhanh chóng, đồng thời hỗ trợ các lập trình viên chuyên nghiệp giải phóng khỏi các tác vụ xây dựng giao diện lặp đi lặp lại để tập trung vào kiến trúc lõi. Nhiều tập đoàn công nghệ lớn hiện nay đều đang đầu tư xây dựng các công cụ tự động sinh mã nguồn (code generator) cho riêng mình.

Khóa học chuyên đề **《Front-end No-Code/Low-Code Practical Workshop》** sẽ hướng dẫn học viên cách lập trình xây dựng các công cụ tự động sinh mã nguồn (code generator) nhắm đến hai bài toán thực tế phổ biến nhất:

1. **Design-to-Code:** Quét dữ liệu từ bản vẽ thiết kế (UI mockup) để tự động biên dịch cấu trúc thành code HTML/CSS hoàn chỉnh.
2. **API-to-Component:** Đọc file đặc tả API (Swagger/OpenAPI) để tự động sinh ra các components giao diện biểu mẫu (form) nhập liệu tương ứng.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081203.jpg)

Lớp học giúp lập trình viên Front-end chuyển đổi tư duy từ người "thực thi nghiệp vụ" sang người "chế tạo công cụ năng suất", giúp rút ngắn thời gian phát triển dự án xuống nhiều lần.

Khóa học được phối hợp tổ chức bởi **Jingcheng Yideng** (đơn vị đào tạo Front-end được chứng nhận bởi Tencent Class) giảng dạy bởi các chuyên gia giàu kinh nghiệm:
- **Thầy Dương Phàm:** Sáng lập kiêm CEO của LightSpeed Software, cựu kỹ sư Senior thuộc nhóm dự án Tencent PC QQ.
- **Thầy Lão Viên:** Sáng lập của Jingcheng Yideng, cựu kỹ sư phát triển của Baidu Maps.

Độc giả bản tin có thể quét mã QR dưới đây để đăng ký tham gia lớp học chuyên đề:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081204.jpg)

Học phí gốc của khóa học là 98 NDT, độc giả đăng ký sớm hôm nay chỉ cần chi trả mức phí ưu đãi trải nghiệm **0,02 NDT**. 50 học viên đăng ký đầu tiên sẽ được tặng kèm bộ tài liệu phỏng vấn Front-end chuyên sâu trị giá 299 NDT.

## 科技动态

1、[Thống kê số tiền thưởng phát hiện lỗi bảo mật của Google](https://security.googleblog.com/2021/07/a-new-chapter-for-googles-vulnerability.html)

Google công bố số liệu thống kê thú vị: Trong vòng 10 năm qua, hãng đã chi trả tổng cộng 29.357.516 USD tiền thưởng (bug bounty) cho 11.055 báo cáo lỗ hổng bảo mật được gửi về từ 2.022 lập trình viên và chuyên gia bảo mật thuộc 84 quốc gia trên thế giới. Tính trung bình, mỗi lỗ hổng bảo mật được Google trả thưởng khoảng 2.656 USD.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072811.jpg)

Đây được đánh giá là một khoản đầu tư vô cùng hiệu quả của các tập đoàn công nghệ lớn. Chỉ với ngân sách chưa tới 3 triệu USD mỗi năm, Google đã phát hiện và vá thành công hơn 1.000 lỗi hệ thống trước khi chúng bị các tổ chức tin tặc lợi dụng phá hoại, gây ra các thiệt hại tài chính và uy tín lớn hơn gấp nhiều lần.

2、[Trung Quốc vận hành trạm chuyển đổi điện ngoài khơi quy mô lớn nhất thế giới](http://finance.people.com.cn/n1/2021/0720/c1004-32163850.html)

Trạm chuyển đổi điện xoay chiều sang dòng điện một chiều (HVDC) ngoài khơi có quy mô lớn nhất thế giới đã được lắp đặt thành công tại vùng biển cách bờ biển Như Đông, tỉnh Giang Tô khoảng 100 km.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081207.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081209.jpg)

Trạm đóng vai trò như một trái tim thu gom toàn bộ nguồn điện năng sản sinh từ 3 trang trại điện gió ngoài khơi xung quanh, chuyển đổi thành dòng điện một chiều điện áp cao để truyền tải về đất liền qua đường cáp ngầm nhằm giảm thiểu tổn thất điện năng trên đường truyền xa. Công trình có diện tích tương đương một sân bóng đá tiêu chuẩn, chiều cao bằng tòa nhà 15 tầng, cung cấp sản lượng điện năng 2,4 tỷ kWh mỗi năm cho hơn 1 triệu hộ gia đình.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081306.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081210.jpg)

3、[Honda ra mắt ý tưởng xe điện cân bằng một bánh độc đáo](https://www.yankodesign.com/2021/07/22/this-self-balancing-honda-electric-scooter-redefines-futuristic-urban-commuting/)

Hãng xe máy Honda giới thiệu ý tưởng thiết kế xe điện cân bằng một bánh (electric self-balancing scooter) vô cùng độc đáo hướng tới nhu cầu di chuyển cá nhân linh hoạt tại các đô thị đông đúc tương lai.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072410.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072411.jpg)

Dòng xe một bánh này giúp tiết kiệm tối đa diện tích đỗ xe và chi phí sản xuất phần cứng so với các dòng xe máy điện hai bánh truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072412.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072413.jpg)

4、[Vẹt mào Úc học hỏi lẫn nhau cách lật mở nắp thùng rác công cộng](https://www.smithsonianmag.com/science-nature/cockatoos-learn-open-garbage-bins-observing-their-peers-180978248/)

Các nhà điểu học tại Úc công bố nghiên cứu thực địa ghi nhận khả năng học hỏi hành vi xã hội đáng kinh ngạc của loài vẹt mào (cockatoo). Họ đã ghi lại được hình ảnh một chú vẹt đứng quan sát tỉ mỉ cách một chú vẹt khác dùng mỏ và chân để bẩy và lật mở nắp thùng rác công cộng tìm kiếm thức ăn:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072408.jpg)

Chỉ sau vài tuần quan sát lan truyền, hơn 50 chú vẹt mào hoang dã sinh sống trong cùng khu dân cư đã tự học được kỹ năng mở nắp thùng rác tương tự mà không cần con người huấn luyện:

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=o3263y9ud2v" allowFullScreen="true" width="600" height="400"></iframe>

5、[Hệ thống AI của Alibaba đạt điểm số đọc hiểu hình ảnh vượt qua con người](https://zhuanlan.zhihu.com/p/398939467)

Hệ thống AI trí tuệ nhân tạo mang tên AliceMind do viện nghiên cứu Đamo (Alibaba Damo Academy) phát triển (đã được open source trên [GitHub](https://github.com/alibaba/AliceMind)) đã giành vị trí quán quân tại cuộc thi Visual Question Answering (VQA) toàn cầu năm 2021 với điểm số kỷ lục lần đầu tiên vượt qua mức điểm trung bình của con người.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081006.jpg)

VQA là bài toán kiểm thử yêu cầu hệ thống máy tính phải "đọc hiểu" nội dung hình ảnh để trả lời các câu hỏi logic phức tạp của người dùng chứ không chỉ nhận diện vật thể đơn thuần. Ví dụ, thay vì chỉ nhận biết bức ảnh có chứa một chiếc máy bay, hệ thống phải trả lời được câu hỏi chiếc máy bay thuộc dòng nào, được sản xuất vào năm nào và làm từ chất liệu gì:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081007.jpg)

Công nghệ VQA hứa hẹn sẽ nâng tầm khả năng tìm kiếm hình ảnh thông minh và ứng dụng hiệu quả trong chẩn đoán y khoa dựa trên phim chụp X-quang hoặc hỗ trợ lái xe tự động nhận diện biển báo giao thông.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081008.jpg)

6、[Framework ra mắt dòng máy tính xách tay tự lắp ráp DIY](https://frame.work/products/laptop-diy-edition)

Startup Framework tại Mỹ chính thức giới thiệu mẫu laptop màn hình 13,5 inch dạng module DIY (Do-It-Yourself). Người mua sẽ nhận được một hộp đựng chứa đầy đủ các bảng mạch linh kiện rời để tự tay lắp ráp thành một chiếc máy tính hoàn chỉnh.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072404.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072403.jpg)

Thiết kế dạng module này giúp người dùng dễ dàng tự thay thế các cổng kết nối (USB-C, HDMI, đầu đọc thẻ), nâng cấp RAM, ổ cứng hoặc sửa chữa bàn phím khi hỏng hóc mà không cần vứt bỏ toàn bộ máy, góp phần giảm thiểu đáng kể lượng rác thải điện tử ra môi trường. Giá bán khởi điểm của thiết bị là 749 USD.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072405.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072407.jpg)

7、[Phát hiện mẩu thiên thạch 4,6 tỷ năm tuổi rơi tại Anh](https://www.facebook.com/eaaro.org.uk/posts/1907081252785935)

Sau khi ghi nhận một vệt sao băng màu xanh lục sáng rực bay qua bầu trời nước Anh vào đêm ngày 28/2, các nhà thiên văn học đã tổ chức tìm kiếm và phát hiện được một mẩu đá đen nặng khoảng 300 gram nằm sâu dưới lớp bùn đất tại hạt Gloucestershire một tháng sau đó.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072301.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072302.jpg)

Kết quả phân tích địa chất cho thấy mẩu đá này có tuổi đời khoảng 4,6 tỷ năm (tương đương với tuổi của Trái Đất và hệ Mặt Trời). Đây là phát hiện vô cùng quý giá giúp các nhà khoa học nghiên cứu thành phần vật chất nguyên thủy cấu thành nên các hành tinh từ buổi sơ khai.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072303.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072304.jpg)

## 文章

1、[Tại sao chuẩn kết nối USB-C hiện nay lại vô cùng hỗn loạn?](https://www.ifanr.com/1374936)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081223.jpg)

Bài viết phân tích thực trạng tuy cổng cắm vật lý USB-C đã trở thành tiêu chuẩn chung cho hầu hết thiết bị di động, nhưng các thông số kỹ thuật bên trong (chuẩn truyền dữ liệu USB 2.0/3.0/4.0, chuẩn sạc nhanh PD, giao thức truyền hình ảnh Alt Mode) lại vô cùng hỗn loạn khiến người dùng khó phân biệt sợi cáp chất lượng.

2、[Hướng dẫn cơ bản về xử lý và trực quan hóa âm thanh](https://cjting.me/2021/08/07/fourier-transform-and-audio-visualization/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081002.jpg)

Tác giả giải thích các kiến thức cơ bản về tần số âm thanh, cách thức lấy mẫu tín hiệu số và ứng dụng toán học biến đổi nhanh Fourier (FFT) để tách dải tần nhằm lập trình hiệu ứng cột sóng âm nhảy theo nhịp nhạc trên nền web. (Đóng góp của [@cj1128](https://github.com/ruanyf/weekly/issues/1880))

3、[Cẩm nang trực quan hóa các kiểu liên kết bảng SQL Join](https://dataschool.com/how-to-teach-people-sql/sql-join-types-explained-visually/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070801.jpg)

Bài hướng dẫn kinh điển sử dụng sơ đồ vòng tròn Venn để mô tả trực quan sự khác biệt giữa các lệnh liên kết bảng dữ liệu SQL (Inner Join, Left Join, Right Join, Full Outer Join) giúp người mới bắt đầu dễ dàng hình dung logic truy vấn.

4、[Hướng dẫn lập trình ứng dụng nghe nhạc sử dụng React Hooks](https://letsbuildui.dev/articles/building-an-audio-player-with-react-hooks)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061803.jpg)

Bài viết hướng dẫn chi tiết từng bước xây dựng một ứng dụng trình phát nhạc trực tuyến đẹp mắt chạy trên trình duyệt sử dụng các React Hooks cơ bản để quản lý trạng thái phát nhạc.

5、[Tìm hiểu nguyên lý vận hành vật lý của tàu thủy](https://ciechanow.ski/naval-architecture/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072806.jpg)

Bài phân tích chi tiết giải thích lực nâng của nước giúp các con tàu thép khổng lồ nổi trên mặt nước, cấu tạo bánh lái cân bằng lực cản và cơ chế tạo lực đẩy của chân vịt tàu biển thông qua các mô hình tương tác 3D sinh động trên trang web.

6、[Hướng dẫn cài đặt tính năng tìm kiếm văn bản đầy đủ trong PostgreSQL](https://blog.crunchydata.com/blog/postgres-full-text-search-a-search-engine-in-a-database)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072804.jpg)

Hệ quản trị cơ sở dữ liệu PostgreSQL tích hợp sẵn công cụ hỗ trợ tìm kiếm văn bản (Full-Text Search). Bài viết giới thiệu cách cấu hình thiết lập tính năng tìm kiếm ngôn ngữ tự nhiên tối giản mà không cần cài đặt thêm Elasticsearch.

7、[Tại sao Safari lại trở thành trình duyệt gây phiền toái nhất cho lập trình viên?](https://blog.perrysun.com/2021/07/15/for-developers-safari-is-crap-and-outdated/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072708.jpg)

Tác giả chia sẻ quan điểm cá nhân chỉ trích Apple chậm trễ cập nhật các API chuẩn Web mới cho trình duyệt Safari, khiến nó trở thành một "Internet Explorer thế hệ mới" gây nhiều khó khăn cho lập trình viên khi tối ưu hóa giao diện web.

8、[Tìm hiểu cơ chế biểu diễn số thực dấu phẩy động trong JavaScript](https://github.com/trekhleb/javascript-algorithms/tree/master/src/algorithms/math/binary-floating-point)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072702.jpg)

Bài viết giải thích tiêu chuẩn IEEE 754 mô tả cách thức công cụ JavaScript Engine biên dịch và lưu trữ các con số thực dưới dạng nhị phân trong bộ nhớ máy tính để người dùng thấu hiểu bản chất của các phép tính sai số (như `0.1 + 0.2 !== 0.3`).

9、[Tại sao tôi quyết định khai tử thư viện mã nguồn mở đạt 25.000 sao?](https://marmelab.com/blog/2020/10/21/sunsetting-faker.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072501.jpg)

Tác giả chia sẻ câu chuyện thực tế về áp lực tinh thần và tài chính sau 10 năm tự nguyện duy trì thư viện mã nguồn mở Faker.js nổi tiếng trước khi quyết định dừng phát triển dự án.

10、[Lịch sử hình thành và phát triển của Pixar](https://spectrum.ieee.org/the-real-story-of-pixar)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080502.jpg)

Bài hồi ký của người sáng lập Pixar chia sẻ về giai đoạn khó khăn ban đầu khi công ty hoạt động như một đơn vị bán phần cứng đồ họa máy tính thất bại, đứng trước bờ vực phá sản trước khi được Steve Jobs rót vốn đầu tư cứu vãn và chuyển hướng thành công sang sản xuất phim hoạt hình 3D.

## 工具

1、[Muboard](https://github.com/susam/muboard)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080301.jpg)

Thư viện JavaScript gọn nhẹ hỗ trợ dựng một chiếc bảng đen viết phấn tương tác hiển thị trực quan các công thức toán học TeX trên trang web.

2、[Muse VR Site Builder](https://www.muse.place/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080404.jpg)

Công cụ no-code hỗ trợ người dùng thiết kế và xây dựng các trang web tương tác không gian 3D tương thích tốt với các thiết bị kính thực tế ảo VR.

3、[MacType](https://mactype.net/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080212.jpg)

Tiện ích hệ thống nguồn mở nổi tiếng hỗ trợ mang cơ chế khử răng cưa và render phông chữ mượt mà của hệ điều hành macOS sang Windows.

4、[gosec (Golang Security Checker)](https://github.com/securego/gosec)

Công cụ phân tích mã nguồn tĩnh (static analysis) chuyên dụng rà soát các lỗi bảo mật và cấu hình yếu trong các dự án lập trình viết bằng Go.

5、[interview-schedule Calendar Sync](https://github.com/Mayandev/interview-schedule/issues/19)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080916.jpg)

Tiện ích tự động hóa sử dụng GitHub Actions quét thông tin lịch hẹn từ Google Calendar để cập nhật thành danh sách ghi chú công việc trực quan trên file README của GitHub repository. (Đóng góp của [@Mayandev](https://github.com/ruanyf/weekly/issues/1879))

6、[Web3.Storage](https://web3.storage/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080915.jpg)

Dịch vụ đám mây hỗ trợ lập trình viên nhanh chóng upload và lưu trữ dữ liệu tệp tin lên mạng lưới lưu trữ phi tập trung IPFS/Filecoin thông qua các API đơn giản. (Đóng góp của [@lgE-1](https://github.com/ruanyf/weekly/issues/1877))

7、[Hora Search Library](https://horasearch.com/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081005.jpg)

Thư viện tìm kiếm điểm dữ liệu lân cận gần nhất (Approximate Nearest Neighbor - ANN) tốc độ cao viết bằng Rust hỗ trợ đa nền tảng Python/JS phục vụ các ứng dụng tìm kiếm ảnh tương đồng hoặc xử lý ngôn ngữ tự nhiên. (Đóng góp của [@salamer](https://github.com/ruanyf/weekly/issues/1883))

8、[SRPC: C++ RPC Framework](https://github.com/sogou/srpc/blob/master/README_cn.md)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081004.jpg)

Dự án framework gọi hàm từ xa RPC hiệu năng cao viết bằng C++ được Sogou phát hành nguồn mở, hỗ trợ nhiều định dạng dữ liệu (Protobuf, JSON) và giao thức mạng. (Đóng góp của [@holmes1412](https://github.com/ruanyf/weekly/issues/1882))

9、[Pushpin Reverse Proxy](https://github.com/fanout/pushpin)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080510.jpg)

Máy chủ proxy ngược (reverse proxy) chuyên dụng quản lý kết nối thời gian thực WebSocket, hỗ trợ các cơ chế truyền tải HTTP streaming và long polling hiệu quả.

10、[js-cookie](https://github.com/js-cookie/js-cookie)

Thư viện JavaScript siêu nhỏ gọn (dung lượng sau nén dưới 1 KB) hỗ trợ thao tác đọc, ghi và xóa cookie trên trình duyệt đơn giản, đạt hơn 18.000 sao trên GitHub.

## Tài nguyên

1、[JetBrains Developer Ecosystem Survey 2021](https://www.jetbrains.com/lp/devecosystem-2021/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081001.jpg)

Báo cáo khảo sát thường niên của JetBrains tổng hợp ý kiến đóng góp của hơn 31.000 nhà phát triển phần mềm toàn cầu phản ánh xu hướng phát triển công cụ lập trình, hệ điều hành phát triển và mức độ phổ biến của các ngôn ngữ.

2、[Cẩm nang hướng dẫn bán hàng phần mềm doanh nghiệp B2B](https://read.douban.com/ebook/322579268/)

Một cuốn sách nhỏ tiếng Trung chia sẻ các kinh nghiệm thực tế về cách tiếp cận khách hàng doanh nghiệp, đàm phán hợp đồng thương mại cho các startup phần mềm. (Đóng góp của [@jiezhao9](https://github.com/ruanyf/weekly/issues/1881))

3、[Candide Plant Identification](https://candidegardening.com/GB/identify-plants)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072709.jpg)

Trang web trực tuyến hỗ trợ người dùng upload ảnh chụp cây cối hoa lá để nhận diện tên loài thực vật nhanh chóng thông qua thuật toán AI.

4、[Coding with Character: Tổng hợp phông chữ gõ code đẹp mắt](https://realdougwilson.com/writing/coding-with-character)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072813.jpg)

Tác giả chia sẻ và đánh giá trực quan hơn 10 phông chữ chuyên dụng viết mã nguồn đẹp mắt giúp lập trình viên tăng cảm hứng gõ code hàng ngày (như phông Input Narrow Mono hiển thị ở ảnh trên).

5、[FastAI Deep Learning Course Book](https://github.com/fastai/fastbook)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072807.jpg)

Cuốn sách giáo khoa nguồn mở đi kèm thư viện học sâu FastAI hướng dẫn chi tiết lý thuyết mạng nơ-ron nhân tạo và cách triển khai các mô hình AI nhận diện hình ảnh, văn bản.

## Steve Jobs ở Kyoto

*Lược dịch theo bài viết ký sự phát hành trên trang tin NHK World ngày 1/7/2021:*

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070507.jpg)

Steve Jobs có một tình yêu đặc biệt dành cho đất nước Nhật Bản, và trong số các thành phố tại đây, cố đô Kyoto là nơi ông yêu thích nhất. Ông đã ghé thăm Kyoto 4 lần trong suốt 25 năm cuộc đời, chuyến đi cuối cùng là vào năm 2010 - chỉ một năm trước khi ông qua đời.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081212.jpg)

Trong cả 4 chuyến đi đó, người tài xế kiêm hướng dẫn viên du lịch tin cậy của ông là ông Oshima Hiroshi. Jobs luôn giao toàn bộ việc lập chi tiết lịch trình tham quan cho Oshima tự sắp đặt.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070508.jpg)

Oshima kể lại địa điểm yêu thích nhất của Steve Jobs tại Kyoto là chùa Ryoanji (Long An Tự). Ngôi chùa thiền tông 500 năm tuổi nổi tiếng với khu vườn khô sơn thủy (Karesansui) xếp đá độc đáo. Jobs đã ghé thăm nơi này tới 3 lần.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081213.jpg)

*"Trong lần đầu tiên dẫn ông ấy tới đây, tôi giải thích khu vườn này có 15 viên đá lớn nhỏ đặt trên nền sỏi trắng, nhưng thiết kế đặc biệt khiến người xem đứng ở bất kỳ góc độ nào trên hành lang cũng không thể nhìn thấy đủ cả 15 viên đá cùng lúc"*, Oshima kể.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070509.jpg)

Steve Jobs lập tức đi vòng quanh hành lang ngôi chùa để tìm kiếm một góc nhìn có thể thu vào toàn cảnh 15 viên đá, nhưng cuối cùng ông chấp nhận thực tế không thể tìm ra góc nhìn đó.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081214.jpg)

Oshima giải thích cho ông hiểu con số 15 trong văn hóa phương Đông tượng trưng cho sự hoàn mỹ trọn vẹn (như đêm trăng rằm ngày 15 âm lịch). Thiết kế cố tình giấu đi 1 viên đá của khu vườn mang triết lý thiền tông nhắc nhở con người rằng sự hoàn mỹ thực chất không tồn tại, và hành trình kiếm tìm sự thấu hiểu nội tâm vẫn luôn phải tiếp diễn. Steve Jobs im lặng ngắm nhìn khu vườn rất lâu. Nhiều năm sau, khi dẫn các con của mình tới đây, ông đã tự tay chỉ và giảng giải lại triết lý này cho các con nghe.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081215.jpg)

Trong cuốn tự truyện *Steve Jobs*, ông từng chia sẻ: *"Tôi nhận ra bản thân bị cuốn hút sâu sắc bởi triết lý Phật giáo, đặc biệt là thiền tông Nhật Bản. Vẻ đẹp hư vô cao viễn của những khu vườn đá khô tại Kyoto đã chạm đến tâm hồn tôi, đó chính là biểu hiện đỉnh cao của văn hóa thiền"*.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081216.jpg)

Tháng 7/2010, Oshima chở Steve Jobs đi qua khu biệt thự cổ kính gần chùa Nanzenji. Một ngôi biệt thự xinh đẹp của nhà sáng lập Nomura Securities được xây dựng từ năm 1928 với khu vườn tuyệt đẹp lọt vào mắt Jobs. Ngôi biệt thự này là di sản văn hóa quốc gia của Nhật Bản và chỉ mở cửa cho công chúng vào những dịp lễ lớn giới hạn.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070510.jpg)

*"Tôi nói với ông ấy rằng khu vườn này hiện đang đóng cửa không tiếp khách, nhưng Jobs nói ông sẽ có cách"*, Oshima nhớ lại. *"Jobs gọi điện cho thư ký riêng tại Mỹ. 10 phút sau, tôi nhận được điện thoại trực tiếp từ văn phòng đại diện Nomura Securities thông báo lịch hẹn tiếp đón Steve Jobs tham quan vào ngày hôm sau"*. Sau một giờ tham quan biệt thự, Jobs trở ra xe và nói với Oshima: *"Tôi muốn xây dựng một khu vườn giống hệt như thế này ở Mỹ"*.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081217.jpg)

Mỗi lần đến Kyoto, Steve Jobs chỉ ở duy nhất tại nhà trọ ryokan truyền thống **Tawaraya**. Nhà trọ cổ kính chỉ có 18 phòng nghỉ nhỏ với diện tích mỗi phòng dưới 15 m2 nhưng Jobs cực kỳ hài lòng với dịch vụ tinh tế tại đây.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070513.jpg)

Nhìn từ bên ngoài, nhà trọ trông không khác gì một ngôi nhà gỗ bình dân giản dị.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070512.jpg)

Bên trong phòng trải chiếu tatami mộc mạc làm nơi ăn ngủ sinh hoạt của khách.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070511.jpg)

Jobs cũng thích ăn mì soba lạnh kèm tempura tại một quán mì bình dân bên cạnh nhà trọ.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070514.jpg)

Trong ngày cuối cùng của chuyến thăm Kyoto cuối cùng vào năm 2010, ông đã dẫn vợ và con gái đến một quán sushi nổi tiếng để dùng bữa trưa.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081218.jpg)

Ông ngồi ở dãy bàn sát tường hướng về phía đầu bếp chế biến. Khi được đầu bếp hỏi muốn dùng món gì, Jobs yêu cầu đầu bếp tự chuẩn bị các món sushi ngon nhất.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081219.jpg)

Người đầu bếp lần lượt dâng lên món sushi cá bơn, sushi mực, sushi tôm tươi và sushi cá ngừ. Sau khi thưởng thức miếng cá ngừ, Jobs yêu cầu đầu bếp dừng lại: *"Hãy tiếp tục phục vụ tôi món sushi cá ngừ này cho đến khi tôi nói dừng lại"*.

Đầu bếp đã phục vụ liên tục 6 phần sushi cá ngừ cho Steve Jobs. Ông chia sẻ: *"Tôi chưa từng được ăn món sushi cá ngừ nào ngon đến thế trong đời"*.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081220.jpg)

Sau bữa ăn ngon miệng, con gái của chủ quán sushi đã xin chữ ký lưu niệm của Steve Jobs. Vốn nổi tiếng là người rất ít khi ký tặng cá nhân, nhưng tâm trạng vui vẻ sau bữa ăn ngon đã khiến ông vui lòng đồng ý.

Bức thư ký tặng của ông hiện được lồng khung kính treo trang trọng trên bức tường của quán sushi:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070516.jpg)

Trên giấy ông viết vỏn vẹn ba từ: *"All good things"* (Mọi điều tốt đẹp). Đây là ba từ mở đầu của câu tục ngữ tiếng Anh nổi tiếng: *"All good things must come to an end"* (Mọi điều tốt đẹp rồi cũng có ngày kết thúc).

*"Có lẽ ông ấy đã cảm nhận được tình trạng sức khỏe suy yếu của mình và biết ngày ra đi không còn xa, nên chỉ viết lửng ba từ đầu tiên của câu"*, người chủ quán sushi chia sẻ. Khi tiễn Jobs ra cửa, chủ quán hẹn sớm gặp lại ông ở Kyoto vào lần tới, Jobs đáp nhẹ nhàng: *"Tôi đang mắc bệnh nặng, đây có lẽ là lần cuối cùng tôi có thể đến thăm Kyoto"*.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081221.jpg)

Năm 2016 - 5 năm sau khi Steve Jobs qua đời, cựu CEO John Sculley của Apple (người từng có cuộc đối đầu quyền lực gay gắt dẫn tới việc trục xuất Jobs khỏi Apple vào năm 1985) đã ghé quán sushi này dùng bữa. Nhìn thấy bức chữ ký của Jobs treo trên tường quán, Sculley đã không kìm được nước mắt. Ông chia sẻ với chủ quán rằng ông vẫn luôn hy vọng có một ngày sau khi nghỉ hưu có thể ngồi lại trò chuyện để hóa giải những bất đồng xưa cũ với Jobs, nhưng sự ra đi của Jobs đã khiến mong ước đó mãi mãi không thể thực hiện được nữa.

## 言论

1、

Thuật toán đề xuất của TikTok sở hữu một lợi thế vượt trội về mặt dữ liệu: nội dung video quá ngắn nên lịch sử xem của người dùng được tính bằng giây. Một giờ lướt ứng dụng sinh ra hàng trăm bản ghi hành vi xem. Netflix phải mất cả tháng trời mới thu được lượng dữ liệu hành vi tương đương của một người dùng.

-- Thảo luận trên Hacker News

2、

Hệ thống phần mềm có một điểm khác biệt cốt lõi so với các công trình kỹ thuật truyền thống: tính biến động yêu cầu cực lớn trong quá trình thực thi. Ví dụ, nếu bạn đang chế tạo một chiếc máy bay dân dụng, không khách hàng nào yêu cầu khi máy bay đang chế tạo dở phải sửa lại để nó bay được ra ngoài vũ trụ. Nhưng trong dự án phần mềm, khách hàng luôn nghĩ rằng chỉ cần code của bạn chạy được, nó phải bay được tới bất kỳ tính năng nào họ muốn.

-- Trích bài viết "Dealing with Complex Projects"

3、

Mọi người thường hỏi tôi: *"Trong 10 năm tới thế giới sẽ thay đổi thế nào?"*. Nhưng hiếm có ai hỏi tôi câu ngược lại: *"Trong 10 năm tới điều gì sẽ KHÔNG thay đổi?"*. Thực tế câu hỏi thứ hai mới là quan trọng nhất, vì doanh nghiệp chỉ có thể xây dựng chiến lược phát triển bền vững dựa trên những giá trị cốt lõi không bao giờ thay đổi theo thời gian.

-- Jeff Bezos

4、

Tôi lo ngại công nghệ số tương lai sẽ quét bắt cử động võ thuật của tôi để ghép vào khuôn mặt của bất kỳ diễn viên nào khác rồi biến nó thành tài sản trí tuệ độc quyền của họ mãi mãi, trong khi những võ sư bằng xương bằng thịt như chúng tôi thì ngày một già đi. Đó là lý do tôi từ chối tham gia đóng các phần tiếp theo của phim Matrix.

-- Lý Liên Kiệt chia sẻ lý do từ chối vai diễn trong Matrix 2 & 3

## 历史上的本周

- 2020年（第 120 期）：[Tại sao chỉ có tư duy mở cửa công nghệ mới có thể phá vỡ các lệnh cấm vận](https://www.ruanyifeng.com/blog/2020/08/weekly-issue-120.html)
- 2019年（第 68 期）：[Hãy tập trung vào sự phát triển năng lực bản thân thay vì quá cân nhắc chế độ đãi ngộ thời trẻ](https://www.ruanyifeng.com/blog/2019/08/weekly-issue-68.html)
- 2018年（第 17 期）：[Thực trạng báo động của xu hướng nóng lên toàn cầu hiện nay](https://www.ruanyifeng.com/blog/2018/08/weekly-issue-17.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
