# Bản tin chia sẻ công nghệ (Số 267): Mùa xuân của 5G sắp đến

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3324) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081702.webp)

Khu phức hợp Sân vận động Cù Châu vừa được khánh thành năm ngoái tại tỉnh Chiết Giang sở hữu phong cách kiến trúc vô cùng độc đáo. Toàn bộ công trình được thiết kế mô phỏng theo địa hình đồi núi nhấp nhô của địa phương với lớp phủ đất và thảm cỏ xanh bên ngoài, tạo thành một hệ thống kiến trúc覆土 (覆土 - bao phủ bởi đất) lớn nhất thế giới. Công trình do công ty kiến trúc MAD Bắc Kinh của kiến trúc sư Mã Nham Tùng thiết kế. (Nguồn: [Sohu](https://www.sohu.com/a/579507996_440222))

## 5G 的春天要来了

Vào đầu tháng này, Tổng cục Phát thanh Truyền hình Quốc gia Trung Quốc đã công bố một [thông báo quan trọng](http://www.nrta.gov.cn/art/2023/8/3/art_114_65077.html) trên trang web chính thức của mình, một tin tức hầu như trôi qua trong im lặng mà ít người chú ý tới.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081207.webp)

**Thành phố Thành Đô đã chính thức khởi động chương trình thử nghiệm phát sóng truyền hình quảng bá trên mạng 5G**. Điều này có nghĩa là cơ quan quản lý phát thanh truyền hình sẽ bắt đầu truyền tải trực tiếp tín hiệu truyền hình quảng bá thông qua hạ tầng mạng 5G.

Nhiều người có thể cảm thấy thắc mắc: việc xem truyền hình hay xem video trực tuyến thông qua kết nối mạng 5G di động chẳng phải là tính năng đã quá quen thuộc từ lâu rồi sao, tại sao giờ lại cần phải thực hiện thử nghiệm?

Tôi xin giải thích ngắn gọn về sự khác biệt bản chất trong cơ chế hoạt động kỹ thuật ở đây:

Các ứng dụng xem truyền hình hay xem video qua Internet hiện nay đều vận hành theo **mô hình kết nối "một-đối-một" (Unicast)**. Cụ thể, mỗi thiết bị của người dùng khi truy cập sẽ thiết lập một luồng truyền nhận tín hiệu độc lập với máy chủ. Nếu có 100 người dùng cùng xem một chương trình, máy chủ sẽ phải thực hiện truyền tải tín hiệu 100 lần, gây hao tốn một lượng băng thông cực kỳ lớn của hệ thống mạng.

Trong khi đó, chương trình thử nghiệm mới áp dụng cơ chế **"Phát sóng quảng bá" (Broadcast) trên mạng 5G. Đây là mô hình kết nối "một-đối-nhiều" (one-to-many)**. Một luồng tín hiệu duy nhất sẽ được phát ra không gian và vô số thiết bị khách xung quanh có thể tự động thu nhận trực tiếp mà không cần thiết lập bất kỳ kết nối phản hồi nào tới máy chủ.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081208.webp)

Với cơ chế phát sóng quảng bá này, thiết bị của người dùng thậm chí không cần được cấp phát địa chỉ IP hay lắp thẻ SIM đăng ký mạng vẫn có thể thu nhận tín hiệu bình thường. Cơ chế này tương tự như cách thức hoạt động của sóng phát thanh Radio truyền thống hoặc hệ thống định vị GPS toàn cầu: tín hiệu truyền đi một chiều và số lượng thiết bị thu nhận tăng lên bao nhiêu cũng hoàn toàn không làm tiêu tốn thêm băng thông truyền tải của trạm phát. Đương nhiên, do là truyền dẫn một chiều, người dùng cũng sẽ không thể thực hiện gửi dữ liệu ngược lại lên hệ thống.

Mô hình phát sóng quảng bá này mang lại rất nhiều ưu điểm thực tế vượt trội:

**1. Phổ cập ngay lập tức chất lượng video siêu nét 4K**

Người dùng khi bật tivi lên sẽ có thể xem ngay các kênh truyền hình độ phân giải cao 4K mượt mà mà không gặp tình trạng giật lag do nghẽn mạng cục bộ.

**2. Thúc đẩy xu hướng xem truyền hình miễn phí trên thiết bị di động**

Trước đây, việc xem truyền hình trực tuyến chất lượng cao trên điện thoại thường tiêu tốn lượng dung lượng data 4G/5G rất lớn với chi phí cước đắt đỏ, cản trở việc tiếp cận của người dùng. Khi áp dụng mô hình phát sóng quảng bá, việc thu nhận tín hiệu hoàn toàn miễn phí và không tiêu tốn dung lượng gói cước data của người dùng, giúp dịch vụ truyền hình di động dễ dàng tiếp cận đại chúng.

**3. Kích cầu nâng cấp phần cứng thiết bị**

Để thu nhận được tín hiệu truyền hình 5G đặc thù này, các dòng tivi thế hệ mới sẽ cần được tích hợp thêm chip giải mã và bộ thu sóng 5G Broadcast chuyên dụng. Đồng thời, để tận hưởng chất lượng hình ảnh sắc nét, người dùng cũng sẽ có nhu cầu nâng cấp lên các dòng tivi màn hình 4K thế hệ mới.

**4. Tiết kiệm tài nguyên băng thông mạng xã hội**

Khi diễn ra các sự kiện thể thao hay giải đấu lớn thu hút lượng người xem khổng lồ cùng lúc (như các trận chung kết World Cup), việc chuyển tải luồng trực tiếp qua sóng phát sóng quảng bá 5G giúp giải phóng phần lớn băng thông mạng Internet di động thông thường, bảo đảm cho các kết nối liên lạc thiết yếu khác tại các khu vực đông người (như ga tàu, công viên) luôn được thông suốt và không bị nghẽn mạng.

**5. Tạo ra "ứng dụng sát thủ" chứng minh ưu thế vượt trội của 5G**

Kể từ khi được triển khai thương mại, mạng 5G vẫn chưa thực sự tạo nên sự bứt phá và thiếu đi các ứng dụng thực tế độc quyền (killer apps) có khả năng chứng minh vị thế vượt trội so với mạng 4G hiện tại (vốn vẫn đang đáp ứng tốt hầu hết các nhu cầu duyệt web, xem phim thông thường).

Sự xuất hiện của công nghệ truyền hình phát sóng quảng bá 5G sẽ thay đổi hoàn toàn điều đó: đây là tính năng độc quyền mà hạ tầng mạng 4G cũ không thể đáp ứng. **Đây hứa hẹn sẽ là một bước ngoặt lịch sử giúp mạng di động 5G bùng nổ mạnh mẽ trong tương lai.**

Nhờ sở hữu nhiều ưu điểm lớn, cả [Mỹ](https://spectrum.ieee.org/5g-tv) và các quốc gia [Châu Âu](https://www.ibc.org/trends/5g-in-broadcast-5g-tv-online/5969.article) hiện đều đang tích cực triển khai các chương trình thử nghiệm công nghệ 5G Broadcast này. Điển hình như lễ đăng quang của Vua Charles III tại Anh vào tháng 5 vừa qua đã được phát sóng truyền hình trực tiếp đồng thời thông qua chuẩn 5G Broadcast.

Dưới đây là một số hình ảnh thực tế ghi lại quá trình thử nghiệm thu nhận tín hiệu truyền hình 5G Broadcast trên màn hình điện thoại di động và tivi tại nước ngoài:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081209.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081210.webp)

Về mặt giải pháp kỹ thuật, công nghệ phát sóng 5G Broadcast có hai phương án triển khai: Phương án thứ nhất là truyền tải tín hiệu thông qua mạng lưới các trạm thu phát sóng di động BTS 5G hiện có của các nhà mạng viễn thông (gọi là phương án "Tháp nhỏ"); phương án thứ hai là truyền tải trực tiếp từ các tháp phát sóng truyền hình công suất lớn sẵn có của hệ thống đài truyền hình quốc gia (gọi là phương án "Tháp lớn").

Trong đợt thử nghiệm tại Thành Đô lần này, Trung Quốc đã lựa chọn áp dụng giải pháp "Tháp lớn". Lý do chính là tại Trung Quốc, hệ thống trạm BTS di động thuộc quyền quản lý của các tập đoàn viễn thông (như China Mobile, China Telecom), trong khi hệ thống tháp truyền hình thuộc về hệ thống phát thanh truyền hình (廣電), và dự án thử nghiệm này do Tổng cục Phát thanh Truyền hình Quốc gia trực tiếp chủ trì thúc đẩy.

Hiện tại các thông tin chi tiết về mặt kỹ thuật và cách thức cụ thể để người dân tại Thành Đô có thể thu sóng trải nghiệm dịch vụ vẫn chưa được công bố rộng rãi. Bạn đọc nào nắm được thông tin chi tiết xin hoan nghênh chia sẻ thêm.

## 科技动态

1、[Mỹ cân nhắc lệnh cấm sử dụng bếp gas trong gia đình do lo ngại ảnh hưởng sức khỏe](https://www.bloomberg.com/news/articles/2023-01-09/us-safety-agency-to-consider-ban-on-gas-stoves-amid-health-fears)

Theo báo cáo từ hãng tin Bloomberg, Ủy ban An toàn Sản phẩm Tiêu dùng Mỹ đang xem xét kế hoạch đưa ra các quy định hạn chế hoặc cấm sử dụng bếp gas tại các hộ gia đình ở nước này:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011003.webp)

Lý do chính được đưa ra là quá trình đốt cháy khí tự nhiên của bếp gas giải phóng ra môi trường trong nhà các chất khí độc hại như nitơ dioxide (NO2), carbon monoxide (CO) và các hạt bụi mịn. Trong môi trường nhà ở đóng kín không có hệ thống hút mùi thông gió tốt, các chất khí này tích tụ lâu ngày sẽ gây ra các bệnh nguy hiểm về đường hô hấp, tim mạch và ung thư cho người sử dụng. Báo cáo thống kê chỉ ra có tới 12% ca hen suyễn ở trẻ em tại Mỹ có nguyên nhân liên quan đến việc tiếp xúc lâu ngày với bếp gas.

Các tổ chức bảo vệ sức khỏe khuyên người dân nên chuyển sang sử dụng bếp từ để bảo vệ sức khỏe. Tuy nhiên, khuyến nghị này vấp phải phản ứng từ các hiệp hội ẩm thực Á Đông, do các món ăn Trung Hoa đặc thù luôn yêu cầu kỹ thuật xào nấu trên ngọn lửa lớn trực tiếp (hơi lửa - wok hei), việc cấm bếp gas sẽ khiến các nhà hàng món Á gặp khó khăn lớn để duy trì hoạt động.

2、[Hành trình vượt biên trốn trên bánh lái tàu dầu vượt Đại Tây Dương của nhóm người di cư](https://www.bbc.com/news/world-latin-america-66450500)

Hãng tin BBC đã đưa tin về một sự việc vượt biên vô cùng hy hữu diễn ra vào tháng 6 vừa qua: bốn người đàn ông Nigeria vì muốn tìm đường rời khỏi đất nước đã liều lĩnh trèo lên trốn phía trên phần bánh lái sát chân vịt của một tàu chở dầu khổng lồ đang neo đậu ngoài khơi:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081305.webp)

Họ lầm tưởng chiếc tàu dầu này đang chuẩn bị di chuyển tới các cảng biển ở Châu Âu nên đã chuẩn bị một ít lương khô và nước ngọt trốn tại đây – khu vực duy nhất họ có thể tiếp cận bằng thuyền đánh cá nhỏ để trèo lên tàu.

Tuy nhiên, hải trình thực tế của con tàu lại là hướng tới Brazil. Nhóm người di cư đã phải trải qua hành trình vượt biển Đại Tây Dương dài tới 5.600 km kéo dài liên tục suốt 14 ngày đêm trong điều kiện vô cùng khắc nghiệt:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081306.webp)

Họ phải bám chặt lấy phần bánh lái chật hẹp, chịu đựng tiếng ồn lớn của động cơ, sóng biển tạt liên tục và chia nhau từng ngụm nước ngọt ít ỏi. Cả bốn người đã sống sót thần kỳ cho đến khi tàu cập cảng Brazil và được lực lượng an ninh cảng phát hiện trong tình trạng kiệt sức hoàn toàn do mất nước.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081307.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081308.webp)

3、[Nghiên cứu hiện tượng đồng bộ sóng não giữa giáo viên và học sinh trong lớp học](https://www.nyu.edu/about/news-publications/news/2023/april/in-sync-brainwaves-predict-learning--study-shows-.html)

Các nhà khoa học tại Đại học New York mới đây đã công bố kết quả nghiên cứu hành vi học đường độc đáo: hiệu quả học tập và tiếp thu kiến thức của học sinh trong giờ học đạt mức tối ưu khi biểu đồ sóng não của giáo viên giảng bài và học sinh thu nhận có xu hướng chuyển dịch đồng điệu tương đồng với nhau:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051808.webp)

Nghiên cứu đề xuất có thể ứng dụng các thiết bị đo điện não đồ để đánh giá khách quan chất lượng của các phương pháp giảng dạy trong thực tế. Tuy nhiên hạn chế lớn nhất là phương pháp này yêu cầu cả giáo viên lẫn học sinh phải liên tục đội mũ đo sóng não cồng kềnh trong suốt tiết học để ghi nhận dữ liệu:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051807.webp)

4、[Trung Quốc thiết kế thử nghiệm tấm pin năng lượng phát điện từ nước mưa](https://thedebrief.org/forget-solar-panels-here-come-rain-panels/)

Các tấm pin năng lượng mặt trời truyền thống chỉ có thể hoạt động hiệu quả tại những khu vực có nhiều ánh nắng ấm áp, hoàn toàn không phát huy được hiệu năng tại những vùng khí hậu nhiều mây mưa kéo dài.

Để giải quyết bài toán này, nhóm nghiên cứu thuộc Đại học Thanh Hoa và Viện Khoa học Trung Quốc đã thiết kế thử nghiệm dòng pin năng lượng thế hệ mới lắp đặt trên mái nhà có khả năng phát sinh dòng điện từ các giọt nước mưa rơi xuống:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072901.webp)

Nguyên lý hoạt động của thiết bị dựa trên việc thu nhận ma sát: khi hạt nước mưa rơi xuống va chạm mạnh vào bề mặt phủ lớp màng polymer đặc biệt của tấm pin, ma sát vật lý sẽ làm hạt mưa tích tụ các hạt điện tích dương. Tấm pin được thiết kế để gom các hạt điện tích này lại để chuyển đổi thành dòng điện sử dụng:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072902.webp)

Báo cáo cho biết công suất phát điện thử nghiệm của hệ thống có thể đạt tới 200 Watt trên mỗi mét vuông diện tích lắp đặt – mức hiệu suất tương đương với các tấm pin mặt trời chất lượng tốt hiện nay trong cùng một diện tích.

## Bài viết

1\. [Tài liệu hướng dẫn sử dụng dịch vụ mạng WiFi trên các chuyến bay nội địa tại Trung Quốc](https://www.36kr.com/p/2383422584255753)（Tiếng Trung）

Bài viết tổng hợp và giới thiệu chi tiết thực trạng triển khai dịch vụ kết nối mạng Internet không dây (In-flight WiFi) của các hãng hàng không nội địa Trung Quốc hiện nay: hướng dẫn các dòng máy bay có hỗ trợ thiết bị vệ tinh kết nối, mức chi phí cước dịch vụ và tốc độ đường truyền thực tế trên khoang khách.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081301.webp)

2\. [Tìm hiểu nguyên lý hoạt động của bộ phân tích cú pháp Pratt Parser trong trình biên dịch](https://engineering.desmos.com/articles/pratt-parser/)（Tiếng Anh）

Bài viết kỹ thuật giới thiệu cơ chế hoạt động của thuật toán phân tích cú pháp Pratt Parser (phương pháp phân tích độ ưu tiên toán tử) thông qua các ví dụ lập trình trực quan, giải thích cách thức trình biên dịch thực hiện chuyển đổi các đoạn mã nguồn chữ viết thô thành cấu trúc cây cú pháp trừu tượng AST (Abstract Syntax Tree) phục vụ biên dịch.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060901.webp)

3\. [Bài viết tương tác trực quan giới thiệu các kiến thức cơ bản về sóng vật lý](https://pudding.cool/2018/02/waveforms/)（Tiếng Anh）

Một trang web giáo khoa tương tác tuyệt đẹp sử dụng nhiều hình ảnh động mô phỏng trực quan để giải thích các thuộc tính vật lý cơ bản của sóng (như biên độ, tần số, bước sóng) và nguyên lý cộng gộp bước sóng để tạo nên âm thanh trong tự nhiên.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061201.webp)

4\. [Tìm hiểu sức mạnh của hàm ẩn danh Lambda trong ngôn ngữ lập trình Ruby](https://scoutapm.com/blog/power-of-lambdas-in-ruby)（Tiếng Anh）

Bài viết hướng dẫn nhập môn chi tiết dành cho các lập trình viên tìm hiểu về cách thức định nghĩa và ứng dụng các khối mã hàm ẩn danh (Lambda) trong ngôn ngữ Ruby, phân tích sự khác biệt của Lambda so với các khối mã Proc thông thường.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052701.webp)

5\. [Mối quan hệ mật thiết giữa cấu trúc ma trận toán học và đồ thị tin học](https://thepalindrome.org/p/matrices-and-graphs)（Tiếng Anh）

Bài viết toán học giới thiệu mối quan hệ tương hỗ chặt chẽ giữa các cấu trúc Ma trận (Matrix) và cấu trúc Đồ thị (Graph) trong khoa học máy tính: hướng dẫn cách thức sử dụng ma trận kề (adjacency matrix) để biểu diễn và tính toán các liên kết phức tạp của đồ thị mạng lưới.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071503.webp)

6\. [Giới thiệu giải pháp sử dụng công cụ Taskfile thay thế cho Makefile truyền thống](https://cloudnativeengineer.substack.com/p/ep-5-taskfile-a-modern-alternative)（Tiếng Anh）

Tác giả chia sẻ kinh nghiệm sử dụng công cụ Taskfile – một trình quản lý và chạy tác vụ tự động hóa viết bằng cú pháp YAML hiện đại, dễ đọc và dễ bảo trì hơn so với việc viết các file cấu hình Makefile truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071604.webp)

7\. [Giới thiệu cấu trúc dữ liệu bảng băm ánh xạ mảng HAMT](https://photonlines.substack.com/p/grokking-hash-array-mapped-tries)（Tiếng Anh）

Bài viết kỹ thuật giải thích nguyên lý cấu tạo và ưu điểm vận hành của cấu trúc dữ liệu HAMT (Hash Array Mapped Trie) – một dạng cấu trúc cây tìm kiếm tối ưu giúp hệ thống thực hiện truy vấn và so khớp nhanh các khóa dữ liệu trong bộ nhớ.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071605.webp)

8\. [Tận dụng thuộc tính CSS đặc thù của trình duyệt Firefox để lấy ảnh chụp màn hình](https://www.stefanjudis.com/a-firefox-only-minimap/)（Tiếng Anh）

Bài viết giới thiệu một thuộc tính CSS đặc biệt hiện chỉ được hỗ trợ thử nghiệm duy nhất trên trình duyệt Firefox (như thuộc tính `-moz-element`), cho phép lập trình viên Front-end lấy ảnh chụp hiển thị trực tiếp của một phần tử DOM bất kỳ trên trang để làm hình ảnh hiển thị cho một phần tử khác (ví dụ làm bản đồ thu nhỏ minimap của trang web).

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071802.webp)

## 工具

1、[Novel: Trình soạn thảo văn bản WYSIWYG trên web hỗ trợ viết bài bằng AI](https://github.com/steven-tey/novel)

Một công cụ soạn thảo văn bản theo thời gian thực (WYSIWYG) dành cho web sở hữu phong cách thiết kế giao diện tối giản tương tự Notion, tích hợp sẵn các API kết nối trí tuệ nhân tạo hỗ trợ soạn thảo nội dung nhanh chóng.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061701.webp)

2、[trurl: Công cụ dòng lệnh hỗ trợ phân tích cấu trúc và xử lý địa chỉ URL](https://github.com/curl/trurl)

Một công cụ dòng lệnh gọn nhẹ do chính tác giả của công cụ curl nổi tiếng Daniel Stenberg phát triển, chuyên phục vụ việc phân tích cấu trúc, trích xuất thông số và chuẩn hóa định dạng các địa chỉ URL một cách chính xác.

3、[WingetUI: Giao diện đồ họa trực quan cho công cụ quản lý gói Winget trên Windows](http://www.marticliment.com/wingetui/)

Phần mềm mã nguồn mở cung cấp giao diện đồ họa (GUI) trực quan giúp người dùng hệ điều hành Windows dễ dàng tìm kiếm, cài đặt và cập nhật các phần mềm hệ thống thông qua bộ quản lý gói dòng lệnh Winget mặc định mà không cần gõ lệnh.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061903.webp)

4、[Bytebase: Hệ thống quản trị và kiểm soát cấu trúc cơ sở dữ liệu trên nền Web](https://www.oschina.net/p/bytebase)

Một giải pháp quản trị cấu trúc cơ sở dữ liệu (Database Schema Management) nguồn mở do các kỹ sư trong nước phát triển, hỗ trợ quy trình kiểm soát thay đổi dữ liệu theo chuẩn GitOps và hỗ trợ hầu hết các hệ CSDL phổ biến. (Đóng góp của [@shandbb](https://github.com/ruanyf/weekly/issues/3367))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081607.webp)

5、[DevPod: Công cụ hỗ trợ đồng bộ hóa môi trường lập trình local lên máy chủ đám mây](https://devpod.sh/)

Ứng dụng máy tính giúp lập trình viên thiết lập môi trường phát triển đồng bộ: tự động ánh xạ và lưu kết quả viết mã từ các IDE cài đặt cục bộ trên máy khách lên các container chạy trên máy chủ đám mây từ xa, hoạt động tương tự như mô hình GitHub Codespaces.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062102.webp)

6、[Anime.js: Thư viện JavaScript hỗ trợ tạo hiệu ứng chuyển động animation](https://animejs.com/)

Một thư viện JS nhỏ gọn nhưng mạnh mẽ giúp các nhà phát triển Front-end xây dựng các hiệu ứng chuyển động đồ họa (CSS properties, SVG, DOM attributes) mượt mà trên giao diện web thông qua hệ thống API trực quan.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062301.webp)

7、[Mailpit: Công cụ kiểm thử và giả lập dịch vụ gửi email dành cho nhà phát triển](https://github.com/axllent/mailpit)

Ứng dụng nhỏ gọn giúp giả lập một máy chủ gửi thư điện tử SMTP nội bộ phục vụ quá trình chạy thử phần mềm: tự động chặn thu toàn bộ các email do hệ thống gửi ra để hiển thị trên giao diện web giúp lập trình viên kiểm tra cấu trúc thư.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062402.webp)

8、[OpenResume: Công cụ thiết kế và xuất bản sơ yếu lý lịch CV mã nguồn mở](https://github.com/xitanggg/open-resume)

Dự án cung cấp công cụ thiết kế hồ sơ năng lực cá nhân (Resume/CV) trực tuyến mã nguồn mở, hỗ trợ xuất file PDF định dạng chuẩn ATS và cho phép import dữ liệu từ các file PDF sẵn có của người dùng.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062601.webp)

9、[Glitch Text Generator: Tiện ích web tạo hiệu ứng chữ nhiễu độc đáo](https://glitchtext.net/)

Một trang web tiện ích đơn giản giúp người dùng tự động chuyển đổi các đoạn chữ viết thông thường thành các định dạng ký tự unicode có hiệu ứng nhiễu sóng (glitch text) lạ mắt để trang trí trang cá nhân. (Đóng góp của [@maojindao55](https://github.com/ruanyf/weekly/issues/3373))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081703.webp)

10、[Fresns: Bộ mã nguồn xây dựng diễn đàn thảo luận và mạng xã hội viết bằng PHP](https://fresns.cn)

Một giải pháp phần mềm nguồn mở viết bằng PHP với cấu trúc module linh hoạt, cho phép người dùng tùy biến thiết lập làm hệ thống diễn đàn, trang tin tức hoặc mạng xã hội nội bộ tùy theo nhu cầu. (Đóng góp của [@jevantang](https://github.com/ruanyf/weekly/issues/3374))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081704.webp)

## 资源

1、[高校校徽字体图标库: Thư viện SVG logo huy hiệu các trường đại học tại Trung Quốc](https://github.com/lovefc/china_school_badge)

Dự án mã nguồn mở thu thập và vẽ lại dưới dạng vector SVG logo huy hiệu chính thức của hơn 200 trường đại học lớn tại Trung Quốc, đóng gói thành bộ font biểu tượng tiện lợi để lập trình viên nhúng vào website sử dụng. (Đóng góp của [@lovefc](https://github.com/lovefc))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081206.webp)

2、[The Concise TypeScript Book: Giáo trình tóm tắt kiến thức lập trình TypeScript ngắn gọn](https://github.com/gibbok/typescript-book)

Cuốn sách hướng dẫn kỹ thuật viết bằng tiếng Anh tóm tắt súc tích toàn bộ các kiến thức cốt lõi và các cú pháp nâng cao của ngôn ngữ TypeScript dành cho lập trình viên tra cứu nhanh.

3、[Workout.lol: Trang web gợi ý tư thế và bài tập gym trực quan](https://workout.lol/)

Một tiện ích web hữu ích dành cho người tập thể hình: người dùng chỉ cần lựa chọn các dụng cụ tập luyện có sẵn tại nhà/phòng gym và nhấp chuột chọn nhóm cơ muốn rèn luyện, hệ thống sẽ tự động hiển thị video hướng dẫn các động tác tập luyện chuẩn xác.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071007.webp)

4、[Name by AI: Ứng dụng hỗ trợ đặt tên tiếng Anh cá nhân bằng AI](https://www.namedbyai.com/)

Công cụ web ứng dụng trí tuệ nhân tạo: dựa trên các câu trả lời khảo sát ngắn về sở thích, tính cách và mong muốn của người dùng để gợi ý danh sách các tên gọi tiếng Anh ý nghĩa phù hợp nhất.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071302.webp)

## 图片

1、**Nghiên cứu vai trò sinh thái bất ngờ của loài lừa hoang trên sa mạc Úc**

Các loài ngựa và lừa hoang dã nhập khẩu tại các vùng hoang mạc nước Úc vốn bị coi là loài gây hại cho hệ sinh thái bản địa do chúng ăn sạch thảm thực vật thấp khan hiếm. Tuy nhiên, nghiên cứu thực địa mới của các nhà khoa học Úc đã ghi nhận một hành vi sinh thái rất thú vị của chúng: lừa hoang có khả năng tự đào giếng nước ngọt trên cát:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081201.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081202.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081203.webp)

Tại các vùng lòng sông khô cạn, lừa hoang sử dụng móng guốc để đào các hố cát sâu xuống mạch nước ngầm. Những giếng nước tự chế này trở thành nguồn cấp nước ngọt duy nhất giúp duy trì sự sống cho hàng loạt loài động vật hoang dã khác trong vùng (như các loài chim, hoẵng và cả thú săn mồi) vượt qua mùa khô hạn:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081204.webp)

Kể cả sau khi giếng nước rút cạn cát bồi, khu vực đất ẩm này vẫn giữ vai trò là những ốc đảo nhỏ giúp các hạt giống thực vật nảy mầm sinh trưởng tạo mảng xanh cho sa mạc:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081205.webp)

2、**Ngắm nhìn kiến trúc uốn lượn toán học độc đáo của Integral House**

Nhà toán học người Canada James Stewart được biết đến là tác giả của bộ giáo trình giảng dạy vi tích phân (Calculus) kinh điển cực kỳ ăn khách tại khu vực Bắc Mỹ, mang lại cho ông nguồn thu nhập tác quyền khổng lồ. Vào năm 2003, ông đã đầu tư xây dựng một dinh thự độc đáo tại khu phố thượng lưu ở Toronto:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081309.webp)

Ông đặt hàng kiến trúc sư phải thiết kế ngôi nhà dựa trên các đường cong mềm mại và thể hiện được vẻ đẹp trừu tượng của các tích phân toán học:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081310.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081311.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081312.webp)

Công trình sau khi hoàn thành đã trở thành một biểu tượng kiến trúc nhà ở nổi tiếng thế giới. Sau khi nhà toán học qua đời vào năm 2014, căn biệt thự độc đáo này đã được giao dịch thành công trên thị trường với mức giá chuyển nhượng lên tới 105 triệu Nhân dân tệ:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081313.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081314.webp)

## ✍️ Bài đọc thêm

### 13 đúc kết quý báu tôi rút ra sau chặng đường 20 năm làm kỹ sư phần mềm

**1. Kỹ sư giỏi không chỉ viết code**

Một kỹ sư phần mềm xuất sắc không đơn thuần chỉ tập trung hoàn thiện các dòng mã lệnh. Họ luôn dành thời gian suy nghĩ về đối tượng người dùng cuối: ai sẽ sử dụng tính năng này, họ sử dụng vì mục đích gì và thao tác như thế nào. Việc luôn đặt nhu cầu người dùng làm trọng tâm là chìa khóa tạo nên trải nghiệm sản phẩm tốt.

**2. Tiết chế tối đa lượng mã nguồn cần viết**

Dù là lập trình viên có trình độ cao đến đâu cũng luôn có xác suất mắc sai lầm trong mã nguồn của mình. Hãy luôn khắc ghi nguyên lý: đoạn code tốt nhất và an toàn nhất chính là đoạn code không cần phải viết ra, hoặc hệ thống đơn giản đến mức không cần tốn công sức bảo trì.

**3. Phần mềm chỉ là phương tiện truyền tải giá trị**

Nhiệm vụ cốt lõi hàng đầu của mọi kỹ sư phần mềm là chuyển giao giá trị thực tế cho doanh nghiệp và khách hàng. Phần mềm hay công nghệ suy cho cùng chỉ là phương tiện kỹ thuật để đạt được mục tiêu đó.

**4. Cảnh giác với những kiến trúc sư xa rời thực tế viết code**

Hãy luôn thận trọng trước những bản thiết kế hệ thống phức tạp được đề xuất bởi những người đã từ rất lâu không trực tiếp tham gia viết mã nguồn thực tế.

**5. Chấp nhận sự bất hoàn hảo của các hệ thống lớn**

Tác giả ngôn ngữ C++ Bjarne Stroustrup có câu nói nổi tiếng: *“Trên đời chỉ có hai loại ngôn ngữ lập trình: loại bị mọi người phàn nàn và loại không có ai thèm dùng”*. Điều này cũng hoàn toàn đúng đối với các hệ thống phần mềm lớn: mọi hệ thống khi quy mô phình to đều sẽ bộc lộ những điểm yếu kém. Do đó, thay vì ám ảnh bởi việc viết code thanh lịch hoàn hảo, hãy tập trung xây dựng một hệ thống hoạt động ổn định, dễ dàng cải tiến liên tục để mang lại giá trị nhanh nhất.

**6. Sự hoang đường của huyền thoại lập trình viên 10x**

Tôi chưa từng gặp một lập trình viên siêu cấp nào có khả năng tạo ra giá trị thực tế gấp 10 lần đồng nghiệp. Tôi chỉ thường thấy những người viết ra lượng code phình to gấp 10 lần bình thường để rồi cả đội ngũ phải tốn công sức sửa lượng bug phát sinh lớn gấp 10 lần. Mục tiêu thực tế của quản lý đội ngũ là làm sao tránh tuyển dụng phải những lập trình viên "0.1x" – những người lười giao tiếp, viết code không chịu chạy test và thường xuyên bỏ qua các kịch bản biên quan trọng.

**7. Bản chất thực sự của sự đổi mới công nghệ**

Mọi người thường nói họ thích sự đổi mới đột phá, nhưng thực chất thứ họ tìm kiếm chỉ là sự thành công thương mại đi kèm một chút mới mẻ. Nếu sự đổi mới của bạn làm thay đổi thói quen làm việc lâu năm của mọi người, bạn sẽ phải chuẩn bị tinh thần nhận về những phản hồi tiêu cực trong giai đoạn đầu. Hãy kiên trì nếu bạn thực tin vào giá trị thực tế của giải pháp.

**8. Dữ liệu là tài sản quan trọng nhất**

Mã nguồn phần mềm có thể bị thay thế viết lại sau vài năm, nhưng dữ liệu hệ thống sẽ tồn tại lâu dài cùng doanh nghiệp. Việc duy trì cấu trúc dữ liệu ngăn nắp, sạch sẽ ngay từ đầu sẽ mang lại thành quả rất lớn cho hệ thống về lâu dài.

**9. Công nghệ cũ ổn định giống như loài cá mập**

Những công nghệ cũ đã tồn tại lâu năm không phải là những con khủng long lỗi thời, mà chúng giống như loài cá mập dưới đại dương: cấu trúc của chúng đã được tối ưu hoàn hảo để giải quyết tốt bài toán thực tế nên chúng không bị đào thải qua các làn sóng công nghệ mới. Đừng vội vàng thay thế một công nghệ cũ đang vận hành ổn định chỉ vì muốn chạy theo những xu hướng công nghệ mới mẻ chưa được kiểm chứng.

**10. Lắng nghe những tiếng nói thầm lặng trong nhóm**

Nhiều kỹ sư phần mềm giỏi có tính cách khá trầm lặng và chỉ đưa ra ý kiến khi được hỏi trực tiếp. Đừng bỏ qua họ. Trong nhiều cuộc họp, những người phát biểu to tiếng nhất lại là những người đưa ra ít giá trị nhất.

**11. Trao quyền chủ động cho kỹ sư**

Nếu bạn tách rời người lập trình ra khỏi thành quả sản phẩm của họ, họ sẽ dần mất đi sự nhiệt huyết công việc. Kỹ sư cần cảm giác làm chủ (ownership) toàn bộ quy trình phát triển sản phẩm để cảm nhận được giá trị mình đóng góp.

**12. Hạn chế tối đa độ phức tạp khi thiết kế hệ thống**

Luôn có vô số lý do (từ yêu cầu tính năng của kinh doanh đến sở thích kỹ thuật của kỹ sư) thúc đẩy hệ thống phình to hơn thiết kế ban đầu. Hãy kiên quyết từ chối những tính năng chưa thực sự cần thiết, luôn cố gắng xây dựng hệ thống với quy mô nhỏ gọn nhất có thể để bảo đảm khả năng vận hành trơn tru.

## Lịch sử tuần này

- 2022年（第 220 期）：[Trí tuệ nhân tạo: Đâu là những cơ hội khởi nghiệp thực tế dành cho các công nghệ AI thế hệ mới](https://www.ruanyifeng.com/blog/2022/08/weekly-issue-220.html)
- 2021年（第 170 期）：[Mô hình kinh doanh: Sự lên ngôi và chiến thắng của mô hình phần mềm dạng đăng ký thuê bao (Subscription)](https://www.ruanyifeng.com/blog/2021/08/weekly-issue-170.html)
- 2020年（第 120 期）：[Phát triển phần mềm: Tại sao chỉ có tư duy mở rộng mã nguồn mới giúp doanh nghiệp vượt qua các rào cản phong tỏa](https://www.ruanyifeng.com/blog/2020/08/weekly-issue-120.html)
- 2019年（第 70 期）：[Kinh tế học: Thế giới bắt đầu bước vào kỷ nguyên lãi suất âm và những tác động tới đời sống](https://www.ruanyifeng.com/blog/2019/08/weekly-issue-70.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes team communication and document management seamless.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
