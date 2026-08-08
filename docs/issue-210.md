# 科技爱好者周刊（第 210 期）：为什么软件变得复杂

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2426) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061615.webp)

Các nhà khoa học Trung Quốc đã công bố bản đồ địa chất Mặt Trăng chi tiết nhất thế giới với tỷ lệ 1:2,5 triệu. Bản đồ thống kê chi tiết bề mặt Mặt Trăng bao gồm 12.341 hố va chạm, 17 loại đá và 14 loại cấu trúc địa chất khác nhau. (Nguồn: [CNSA](http://www.cnsa.gov.cn/n6758823/n6758838/c6840495/content.html))

## 本周话题：为什么软件变得复杂

Tôi luôn tin rằng mục tiêu cốt lõi của việc phát triển phần mềm là tránh sự phức tạp. Thiết kế phần mềm càng đơn giản càng tốt, nhưng nhiều lập trình viên lại lấy làm tự hào khi xây dựng được các giải pháp phức tạp.

Tuy nhiên, một bài viết tuần này đã khiến tôi phải suy nghĩ lại và nhận thấy quan điểm tránh phức tạp đôi khi không thực tế: **Phần mềm chắc chắn sẽ ngày càng trở nên phức tạp hơn.**

### （一）

Tác giả của bài viết này là Nolan Lawson, kỹ sư Front-end tại Salesforce. Bài viết có tiêu đề là [《Sự sụp đổ của phần mềm phức tạp》](https://nolanlawson.com/2022/06/09/the-collapse-of-complex-software/) (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061407.webp)

Như các bạn đã biết, Salesforce là một tập đoàn công nghệ lớn chuyên phát triển các phần mềm quản lý doanh nghiệp và nổi tiếng với các sản phẩm vô cùng cồng kềnh, phức tạp.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061406.webp)

Vì vậy, thật trớ trêu khi một kỹ sư hàng đầu của một công ty chuyên sản xuất phần mềm phức tạp lại công khai viết rằng: phần mềm phức tạp cuối cùng sẽ sụp đổ.

Mặc dù tác giả không trực tiếp nhắc đến tên Salesforce trong bài viết, nhưng những chia sẻ của ông rất giống như trải nghiệm thực tế tại đây:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061408.webp)

> *"Bất kỳ ai làm việc trong ngành công nghệ đủ lâu, đặc biệt là tại các tập đoàn lớn, đều từng chứng kiến cảnh tượng này:*
> 
> *Có một hệ thống legacy cũ khổng lồ và phức tạp, không một ai trong công ty thực sự hiểu hết cách nó vận hành.*
> 
> *Khi các kiến trúc sư được yêu cầu 'sửa chữa' hoặc nâng cấp hệ thống, họ sẽ đứng trước một tấm bảng trắng lớn, vẽ sơ đồ phân rã hệ thống thành hàng loạt hộp chức năng và các đường mũi tên liên kết. Và giải pháp của họ để giải quyết các vấn đề phát sinh là... vẽ thêm nhiều hộp và mũi tên hơn nữa. Không ai dám xóa bỏ bất kỳ cấu phần nào hiện có, mỗi người chỉ âm thầm bổ sung phần việc của riêng mình vào bức tranh chung."*

Mô tả này vô cùng chân thực và phản ánh đúng thực trạng vận hành dự án tại các doanh nghiệp lớn hiện nay:

1. **Yêu cầu của khách hàng ngày càng phức tạp:** Để đáp ứng các nhu cầu đa dạng này, phần mềm buộc phải phình to và trở nên phức tạp.
2. **Ban lãnh đạo quan tâm đến lợi nhuận hơn là cấu trúc mã nguồn:** Chỉ cần phần mềm còn mang lại doanh thu, họ sẽ chấp nhận việc hệ thống ngày càng rối rắm.
3. **Sự phức tạp đè nặng lên vai các kỹ sư cấp cao:** Mỗi kỹ sư chỉ cố gắng chắp vá giải pháp của mình (thêm hộp và mũi tên) để giải quyết vấn đề trước mắt. Sau một thời gian chịu đựng áp lực quá tải, họ thường lựa chọn rời bỏ công ty.
4. **Hệ thống cũ trở nên bất khả thi để bảo trì:** Cách duy nhất để giải quyết triệt để là đập bỏ hệ thống cũ và xây dựng lại một hệ thống mới từ đầu.

Vì vậy, Nolan Lawson đưa ra kết luận khá bi quan: **Không có giải pháp nào để giải quyết triệt để sự phức tạp của phần mềm. Kết cục thông thường là bạn sẽ rời đi, và công ty sẽ phải đập bỏ phần mềm đó để viết lại từ đầu.**

Góc nhìn này hoàn toàn trùng khớp với thực trạng vận hành các hệ thống legacy cồng kềnh tại các tập đoàn công nghệ lớn hiện nay.

### （二）

Nolan Lawson còn đưa ra một quan điểm đáng chú ý khác. Mọi người thường nghĩ các hệ thống phức tạp dễ sụp đổ trong giai đoạn kinh tế phát triển nóng do lượng giao dịch quá tải. Tuy nhiên, ông cho rằng **sự sụp đổ của hệ thống thường xảy ra trong giai đoạn kinh tế suy thoái.**

Trong thời kỳ kinh tế tăng trưởng tốt, các công ty công nghệ có đủ ngân sách để tuyển thêm nhân sự và đổ thêm tài nguyên để gánh vác, duy trì hệ thống phức tạp. Nhưng khi kinh tế bước vào giai đoạn suy thoái, các doanh nghiệp bắt đầu cắt giảm chi phí, đóng băng tuyển dụng hoặc sa thải nhân sự. Lúc này, các hệ thống phức tạp sẽ lập tức bộc lộ điểm yếu và gặp sự cố nghiêm trọng do thiếu hụt đội ngũ bảo trì có chuyên môn.

Trong bối cảnh nền kinh tế toàn cầu đang có xu hướng thắt chặt hiện nay, liệu chúng ta có sắp sửa chứng kiến một làn sóng sự cố và sụp đổ của các hệ thống phần mềm lớn do thiếu nhân lực bảo trì?

## 前端高频面试题（2022版）

Thực tế hiện nay cho thấy sức nóng của ngành phát triển Front-end đã có phần hạ nhiệt do các thư viện công nghệ dần đi vào giai đoạn ổn định và lượng người dùng smartphone đã đạt ngưỡng bão hòa.

Dù vậy, Front-end vẫn là một trong những nhánh hoạt động sôi nổi nhất của ngành CNTT. Theo khảo sát hàng năm của [GitHub Octoverse](https://octoverse.github.com/), JavaScript vẫn giữ vững vị trí ngôn ngữ phổ biến nhất, trong khi TypeScript đã vươn lên mạnh mẽ đạt vị trí thứ tư, xếp ngay sau Python và Java:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061616.webp)

Sự ổn định của công nghệ đồng nghĩa với việc có ít framework hay công cụ mới ra đời hơn. Cộng đồng tập trung nhiều hơn vào việc tối ưu hóa và nâng cấp các công cụ sẵn có.

Các đội ngũ Front-end tại các doanh nghiệp lớn chuyển hướng sang tối ưu hóa chuyên sâu các mảng kỹ thuật cụ thể (như tối ưu hóa hiệu năng render, đóng gói build tool). Do đó, yêu cầu tuyển dụng của doanh nghiệp cũng khắt khe hơn: họ cần những kỹ sư hiểu sâu về bản chất hệ thống thay vì chỉ biết sử dụng framework ở mức cơ bản.

Nhìn chung, độ khó trong công việc của lập trình viên Front-end hiện nay đã dịch chuyển sang phía bên phải của biểu đồ, đòi hỏi chuyên môn sâu hơn trước:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061617.webp)

Nếu bạn đã có nền tảng phát triển Web cơ bản và đang có kế hoạch phỏng vấn tuyển dụng, bộ tài liệu dưới đây sẽ là nguồn tham khảo hữu ích:

Tài liệu **《Cẩm nang câu hỏi phỏng vấn Front-end đại học và doanh nghiệp lớn (2022)》** dài 174 trang tổng hợp các câu hỏi phỏng vấn thực tế mới nhất do nền tảng đào tạo lập trình Geek Time biên soạn:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061620.webp)

Các câu hỏi được phân loại theo từng chuyên đề từ cơ bản đến nâng cao, đi kèm đáp án phân tích chi tiết giúp học viên dễ dàng hệ thống hóa kiến thức:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061618.webp)

Đồng thời, bộ tài liệu cũng chia sẻ kinh nghiệm chuẩn bị hồ sơ CV, kỹ năng đàm phán lương và ứng phó các tình huống phỏng vấn thực tế từ các kỹ sư công nghệ đi trước:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061619.webp)

Bạn đọc có thể quét mã QR phía trên để nhận **miễn phí** bộ tài liệu ôn tập Front-end này từ ban tổ chức.

*Lưu ý: Bộ tài liệu được thiết kế chuyên sâu, phù hợp với các lập trình viên đã có kinh nghiệm làm việc thực tế hơn là các bạn sinh viên mới bắt đầu học lập trình web.*

## 科技动态

1、[Thiết kế giải pháp mô phỏng nụ hôn ảo trong môi trường VR](https://gizmodo.com/vr-researches-simulate-kisses-with-ultrasonic-transduce-1848849489)

Các nhà nghiên cứu tại Đại học Carnegie Mellon vừa phát triển một công nghệ mới giúp người đeo kính thực tế ảo VR có thể cảm nhận được các kích thích xúc giác như nụ hôn ảo:

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022043003.webp)

Hệ thống sử dụng các cảm biến siêu âm (ultrasonic transducers) gắn ở viền dưới kính VR để bắn chùm sóng siêu âm định hướng vào vùng môi và miệng người dùng, tạo ra các xung lực nhỏ mô phỏng chân thực cảm giác chạm lên môi, răng hoặc lưỡi:

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022043004.webp)

Bên cạnh mô phỏng nụ hôn, công nghệ này còn được ứng dụng trong game để tạo ra các hiệu ứng môi trường chân thực như cảm giác gió thổi qua mặt, mạng nhện quẹt vào má hoặc cảm giác uống nước ảo.

2、[Hội đồng Bóng rổ Quốc tế cho phép sử dụng sân đấu kính LED trong các giải lớn](http://www.lanxiongsports.com/posts/view/id/22687.html)

Liên đoàn Bóng rổ Quốc tế (FIBA) chính thức ra thông báo cho phép áp dụng hệ thống sàn thi đấu bằng kính LED (LED glass floor) tại các giải đấu thế giới cấp cao nhất:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060807.webp)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060808.webp)

Trước đây sàn đấu bắt buộc phải làm bằng gỗ tự nhiên để đảm bảo độ đàn hồi giảm chấn cho vận động viên. Hiện tại, công nghệ vật liệu kính cường lực LED thế hệ mới đã đáp ứng đầy đủ tiêu chuẩn giảm chấn tương đương gỗ.

Sử dụng sàn đấu LED giúp đơn giản hóa việc kẻ vạch sân, dễ dàng chuyển đổi nhanh giữa sân bóng rổ, bóng chuyền, cầu lông và cho phép hiển thị trực quan các thông số kỹ thuật trận đấu trực tiếp trên mặt sân:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060809.webp)

3、[Dự án sáng tạo phông chữ biến dạng tự nhiên theo sự sinh trưởng của thân cây](https://bjoernkarmann.dk/occlusion-grotesque)

Một nghệ sĩ người Đan Mạch đã thực hiện một thử nghiệm nghệ thuật độc đáo: khắc các chữ cái lên thân một cây xanh trong rừng để theo dõi sự biến đổi của phông chữ theo sự lớn lên của cây:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050302.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050306.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050307.webp)

*(Quá trình biến đổi của các ký tự chữ cái a và o khắc trên thân cây sau 5 năm)*

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050303.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050304.webp)

Các chữ cái sau khi được số hóa thành phông chữ máy tính hiển thị trên các ấn phẩm in ấn:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050305.webp)

Nghiên cứu cho thấy các vết khắc chữ chủ yếu bị kéo giãn theo chiều ngang thân cây (làm chữ béo và dày hơn) trong khi chiều cao chữ hầu như không thay đổi. Điều này chứng minh sinh học thân cây sau khi định hình chiều cao chỉ phát triển mở rộng chu vi vòng thân.

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050308.webp)

4、[Chính phủ Mỹ ban hành quy định cấm bán bóng đèn sợi đốt](https://www.cnbc.com/2022/04/26/biden-blocks-sales-of-inefficient-lightbulbs-reversing-trump-policy-.html)

Chính phủ Mỹ vừa công bố lộ trình cấm lưu hành đối với các dòng bóng đèn có hiệu suất phát quang thấp dưới 45 lumens/watt, điều này đồng nghĩa với việc khai tử hoàn toàn bóng đèn sợi đốt truyền thống trên thị trường:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050502.webp)

Quy định hướng tới mục tiêu tối ưu hóa tiết kiệm năng lượng điện quốc gia. Trung bình bóng đèn sợi đốt chỉ đạt hiệu suất khoảng 10 lumens/watt trong khi bóng đèn LED hiện đại dễ dàng đạt trên 100 lumens/watt.

## 文章

1、[Chia sẻ của lập trình viên game Nhật Bản về quá trình hợp tác và chia tay nhà phát hành Trung Quốc](https://www.chuapp.com/?a=index&c=Article&id=288712)（Tiếng Trung）

Bài dịch chia sẻ trải nghiệm thực tế của một nhà phát triển game độc lập Nhật Bản về quy trình làm việc, đàm phán hợp đồng phát hành game và những xung đột về mặt bản quyền dẫn tới quyết định hủy bỏ hợp tác với nhà phát hành Trung Quốc.

2、[Intel chính thức công bố thông tin công nghệ tiến trình Intel 4](https://finance.sina.com.cn/tech/2022-06-14/doc-imizirau8363822.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061609.webp)

Intel công bố chi tiết về tiến trình Intel 4, đánh dấu cột mốc lần đầu tiên hãng ứng dụng công nghệ khắc cực tím cực ngắn EUV vào dây chuyền sản xuất vi xử lý thương mại đạt mật độ bóng bán dẫn tương đương tiến trình 7nm để cạnh tranh trực tiếp với TSMC.

3、[Cẩm nang hướng dẫn tự xây dựng hệ thống lưu trữ mạng NAS gia đình](https://icloudnative.io/posts/budget-nas/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060906.webp)

Bài viết chia sẻ chi tiết cẩm nang tự lựa chọn linh kiện phần cứng, cài đặt hệ điều hành và thiết lập máy chủ lưu trữ mạng NAS gia đình dung lượng 22TB với mức ngân sách tối ưu nhất. (Đóng góp của [@yangchuansheng](https://github.com/ruanyf/weekly/issues/2444))

4、[Giới thiệu phương pháp quản lý công việc tối giản dạng thẻ vật lý](https://ugmonk.com/blogs/journal/analog-the-simplest-productivity-system)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021201.webp)

Tác giả chia sẻ giải pháp quản lý công việc hàng ngày mang tên "Analog": thay vì sử dụng các phần mềm todo app, ông ghi tối đa 10 đầu việc cần làm lên một thẻ giấy cứng đặt ngay trên bàn làm việc để dễ dàng theo dõi tập trung.

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021202.webp)

5、[Xây dựng hệ thống CDN hình ảnh miễn phí sử dụng Cloudflare và Backblaze B2](https://www.backblaze.com/blog/free-image-hosting-with-cloudflare-transform-rules-and-backblaze-b2/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021604.webp)

Bài viết hướng dẫn chi tiết các bước thiết lập hosting lưu trữ ảnh trên dịch vụ lưu trữ đám mây Backblaze B2, sau đó cấu hình CDN qua Cloudflare tận dụng gói dịch vụ miễn phí để tối ưu chi phí vận hành cho các website nhỏ.

6、[Ứng dụng phím tắt iOS Shortcuts giúp hạn chế nghiện mạng xã hội](https://nick.comer.io/post/ios-shortcuts)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022010401.webp)

Tác giả chia sẻ cách thiết lập kịch bản tự động hóa trên iOS: mỗi khi người dùng mở các ứng dụng mạng xã hội giải trí, hệ thống sẽ tự động kích hoạt phím tắt hiển thị màn hình thông báo nhắc nhở tập trung vào công việc chính.

7、[Quy trình xử lý hậu kỳ ảnh kỹ thuật số hoàn toàn bằng các phần mềm nguồn mở](https://blog.fidelramos.net/photography/photography-workflow#5-replication-with-syncthing)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040609.webp)

Một nhiếp ảnh gia chuyên nghiệp chia sẻ cẩm nang các công cụ phần mềm miễn phí (như Darktable, GIMP, Syncthing) giúp quản lý và chỉnh sửa ảnh chất lượng cao thay thế cho bộ công cụ Adobe mất phí.

8、[Giải pháp kiến trúc vận hành hàng chục trang web nhỏ trên một VPS duy nhất](https://cprimozic.net/blog/my-selfhosted-websites-architecture/#backup--disaster-recovery)（Tiếng Anh）

Bài viết chia sẻ chi tiết cách thiết lập máy chủ ảo VPS chạy Docker, cấu hình reverse proxy Nginx và hệ thống sao lưu dữ liệu tự động giúp tác giả tự vận hành hàng chục trang web dịch vụ quy mô nhỏ một cách ổn định.

9、[Phương pháp gián tiếp đo lường lượng dòng tiền đổ vào thị trường tiền mã hóa](https://tomtunguz.com/how-much-money-flowing-into-crypto/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020302.webp)

Bài viết đề xuất phương pháp ước lượng dòng vốn đổ vào thị trường crypto thông qua việc theo dõi và thống kê tốc độ tăng trưởng lượng phát hành hàng tháng của các đồng tiền ổn định (stablecoins).

## 工具

1、[CloudMP3.cc: Công cụ chuyển đổi âm thanh từ SoundCloud thành file MP3](https://cloudmp3.cc/en/)

Dịch vụ trực tuyến giúp người dùng tải nhanh các file nhạc, podcast từ nền tảng SoundCloud về máy tính dưới định dạng MP3.

2、[ToolJet: Khung phát triển low-code nguồn mở xây dựng giao diện quản trị](https://github.com/ToolJet/ToolJet)

Bộ công cụ hỗ trợ các nhà phát triển thiết kế nhanh các trang quản trị cơ sở dữ liệu nội bộ thông qua thao tác kéo thả linh hoạt và kết nối trực tiếp với PostgreSQL, MongoDB, Google Sheets.

3、[iWeRead (i 微信读书): Tiện ích mở rộng hỗ trợ đọc sách trên WeChat Read](https://secreter.github.io/ireader/index.html)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061503.webp)

Plugin dành cho trình duyệt Chrome giúp người dùng tối ưu hóa giao diện đọc của trang WeChat Read bản web, hỗ trợ xuất nhanh các ghi chú trích dẫn và thiết kế ảnh trích dẫn đẹp mắt. (Đóng góp của [@secreter](https://github.com/ruanyf/weekly/issues/2439))

4、[Sogou C++ Workflow: Engine máy chủ C++ bất đồng bộ do Sogou phát triển](https://github.com/sogou/workflow)

Bộ thư viện mã nguồn mở C++ hỗ trợ lập trình viên xây dựng hệ thống xử lý tác vụ bất đồng bộ, kết nối cơ sở dữ liệu hiệu năng cao đang vận hành các dịch vụ cốt lõi tại Sogou. (Đóng góp của [@Barenboim](https://github.com/ruanyf/weekly/issues/2446))

5、[FastGit: Dịch vụ proxy tăng tốc độ kết nối GitHub nội địa](https://doc.fastgit.org/zh-cn/guide.html)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061504.webp)

Dịch vụ proxy trung gian giúp các nhà phát triển trong nước tải nhanh các thư viện mã nguồn từ GitHub (lưu ý không nên sử dụng dịch vụ này khi đăng nhập tài khoản cá nhân vì lý do an toàn bảo mật). (Đóng góp của [@dllen](https://github.com/ruanyf/weekly/issues/2448))

6、[Go-Ldap-Admin: Giao diện quản lý dịch vụ OpenLDAP viết bằng Go và Vue](http://ldapdoc.eryajf.net/)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061505.webp)

Hệ thống quản trị tài khoản openLDAP trực quan, hỗ trợ đồng bộ dữ liệu người dùng của doanh nghiệp với các ứng dụng nhắn tin nội bộ như DingTalk, Lark. (Đóng góp của [@eryajf](https://github.com/ruanyf/weekly/issues/2450))

7、[Japa: Thư viện kiểm thử gọn nhẹ dành cho các dự án Node.js](https://japa.dev/)

Framework viết mã test đơn giản, hiệu năng cao chạy trực tiếp không cần cấu hình phức tạp dành riêng cho các ứng dụng viết bằng JavaScript/TypeScript trên môi trường Node.js.

8、[@xata.io/screenshot: Thư viện JS hỗ trợ chụp ảnh màn hình trang web](https://github.com/xataio/screenshot)

Gói thư viện JavaScript nhỏ gọn giúp nhà phát triển dễ dàng tích hợp tính năng tự động chụp ảnh màn hình giao diện hiện tại của trang web và xuất ra file ảnh.

9、[GitLens: Plugin quản lý lịch sử Git cực kỳ mạnh mẽ cho VS Code](https://www.gitkraken.com/gitlens/features)

Extension hỗ trợ hiển thị thông tin tác giả viết từng dòng code (git blame) thời gian thực, so sánh nhanh các nhánh commit trực quan ngay trong trình soạn thảo VS Code.

## Deno 框架

Deno là môi trường chạy mã JavaScript/TypeScript thế hệ mới được thiết kế để cạnh tranh trực tiếp với Node.js. Các bộ khung framework xây dựng trên Deno đang dần hoàn thiện giúp công nghệ này dễ tiếp cận hơn:

1、[Fresh: Framework phát triển Web gọn nhẹ cho Deno](https://fresh.deno.dev/)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061401.webp)

Fresh Framework vừa ra mắt bản thử nghiệm hỗ trợ kết xuất giao diện HTML hoàn toàn từ phía máy chủ (SSR) mà không cần cấu hình hay biên dịch trước, giúp giảm thiểu tối đa dung lượng mã JS tải về trình duyệt người dùng.

2、[Aleph.js: Framework full-stack hỗ trợ React/Vue chạy trên Deno](https://alephjs.org/)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061402.webp)

Dự án phát triển bộ khung full-stack cho Deno hoạt động tương tự Next.js trong hệ sinh thái React, hiện đang ở giai đoạn hoàn thiện các tính năng cốt lõi.

3、[Express 5.0 chuẩn bị phát hành bản chính thức](https://expressjs.com/)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061403.webp)

Bộ thư viện máy chủ NodeJS kinh điển Express chuẩn bị phát hành phiên bản 5.0 chính thức sau hơn 8 năm vận hành phiên bản 4.0. Xem thêm thông tin về các thay đổi cấu trúc và hỗ trợ async handler mới tại bài viết [Điểm mới trên Express 5](https://fusebit.io/blog/new-express-5-features/).

## 可视化作品

1、[Interactive 3D Submarine Cables Map (Bản đồ tương tác cáp quang biển toàn cầu)](http://he.net/3d-map/)

Trang web trực quan hóa quả địa cầu 3D tương tác hiển thị vị trí các tuyến cáp quang biển huyết mạch kết nối mạng Internet toàn cầu và vị trí các trạm máy chủ máy trạm lớn.

2、[Draw Aurora: Trang vẽ tranh tương tác cực quang](https://www.drawaurora.com/)

Trang web tương tác nghệ thuật cho phép người dùng sử dụng chuột để tự tay phác họa và mô phỏng chuyển động của các dải ánh sáng cực quang sắc màu trên bầu trời đêm.

3、[Persepolis 3D: Khám phá kinh đô cổ đại Ba Tư qua phối cảnh 3D](https://persepolis.getty.edu/)

Dự án số hóa của bảo tàng phục dựng lại toàn cảnh kiến trúc kinh đô cổ đại Persepolis (thuộc Iran ngày nay) dưới dạng mô hình 3D tương tác giúp người xem tự do dạo bước khám phá di sản.

## 图片

1\. [Ảnh vệ tinh ghi nhận sự biến mất của hồ muối Aral lớn thứ tư thế giới](https://zh.wikipedia.org/wiki/%E9%B9%B9%E6%B5%B7)

Hồ muối Aral tại Trung Á từng có diện tích lên tới 68.000 km2 (lớn thứ tư thế giới). Tuy nhiên các dự án đào kênh dẫn nước tưới tiêu quy mô lớn của Liên Xô từ thập niên 60 đã khiến hồ bị mất nguồn nước bù đắp và cạn trơ đáy:

*(Hình ảnh chụp hồ Aral năm 1985)*

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022022001.webp)

*(Hình ảnh chụp hồ Aral năm 1997)*

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022022002.webp)

*(Hình ảnh chụp hồ Aral năm 2014 - hồ nước khổng lồ hầu như đã biến mất hoàn toàn)*

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022022003.webp)

2\. [Kiến trúc tòa nhà kiêm bức tường chắn gió Fermont tại Canada](https://www.houseporn.ca/landscape/article/the_wall_housing_structure_in_fermont_quebec)

Tại một thị trấn nhỏ gần cực Bắc thuộc bang Quebec (Canada), người dân thường xuyên phải hứng chịu những luồng gió lạnh bắc cực thổi mạnh buốt giá.

Để chắn gió, kiến trúc sư đã thiết kế tòa nhà phức hợp dịch vụ và nhà ở cao 50 mét, kéo dài 1,3 km đóng vai trò như một bức tường chắn gió kiên cố bảo vệ cho khu dân cư phía sau:

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022022006.webp)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022022007.webp)

Thiết kế giúp tạo ra một vi khí hậu ấm áp, không có gió lớn thổi trực diện cho toàn bộ cư dân sinh sống trong khu vực thị trấn nhỏ phía sau bức tường:

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022022008.webp)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022022009.webp)

## 💡 Bài đọc thêm

### Giai thoại tăng doanh số bán kem đánh răng thêm 40% của chuyên gia tư vấn

Thập niên 50 của thế kỷ trước, một công ty sản xuất kem đánh răng lớn tổ chức chương trình thu thập ý kiến đóng góp từ công chúng để tìm giải pháp đột phá doanh thu bán hàng.

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020805.webp)

Sau đó, một người đàn ông đã đề xuất giải pháp giúp tăng ngay 40% sản lượng bán ra mà không cần thay đổi công nghệ hay tăng ngân sách tiếp thị, ông yêu cầu mức phí bản quyền ý tưởng là 100.000 USD.

Sau nhiều tuần đắn đo, ban giám đốc công ty đã đồng ý ký hợp đồng chi trả số tiền trên. Người đàn ông trao lại một phong bì nhỏ chứa mảnh giấy ghi vỏn vẹn 4 từ:

> *"Make The Hole Bigger"* (Hãy làm miệng vòi to hơn)

Trước đây, đường kính vòi bóp của tuýp kem đánh răng thường được sản xuất ở mức 5mm. Khi nâng đường kính vòi lên 6mm, lượng kem đánh răng bóp ra ngoài trong mỗi lần sử dụng của khách hàng theo thói quen bóp lực cũ sẽ tự động tăng thêm khoảng 44%. 

Sự thay đổi kích thước lỗ nhỏ bé này đã giúp khách hàng tiêu hao tuýp kem nhanh hơn và tăng mạnh sản lượng mua lặp lại của người tiêu dùng, đem lại doanh thu kỷ lục lịch sử cho công ty.

## 历史上的本周

- 2021年（第 162 期）：[Trải nghiệm cuộc sống: Góc nhìn ví von đời người như trò chơi Pac-Man cổ điển](https://www.ruanyifeng.com/blog/2021/06/weekly-issue-162.html)
- 2020年（第 111 期）：[Phân tích sản phẩm: Những sai lầm trong định hướng thiết kế giao diện của TV thông minh](https://www.ruanyifeng.com/blog/2020/06/weekly-issue-111.html)
- 2019年（第 60 期）：[Giới thiệu sách: Cuốn tự truyện của nhà nhân chủng học nghiên cứu về nguồn gốc loài người](https://www.ruanyifeng.com/blog/2019/06/weekly-issue-60.html)
- 2018年（第 9 期）：[Thảo luận tương lai công nghệ: Ý tưởng cấy ghép thẻ căn cước thông minh dưới da người](https://www.ruanyifeng.com/blog/2018/06/weekly-issue-9.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
