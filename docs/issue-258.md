# Bản tin chia sẻ công nghệ (Số 258): Chú mèo của Carmack

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3157) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060502.webp)

Mẫu đĩa bay chở người đầu tiên trên thế giới đã thực hiện chuyến bay thử nghiệm cất cánh thành công tại thành phố Thâm Quyến vào ngày 3 tháng 6. Thiết bị bay này vận hành hoàn toàn bằng động cơ điện, đạt độ cao bay tối đa khoảng 200m với thời lượng pin duy trì hành trình liên tục trong vòng 15 phút. (Nguồn: [Sohu](https://www.sohu.com/a/681963859_121384220))

## 卡马克的猫

Tôi xin giới thiệu với các bạn cuốn sách nổi tiếng trong ngành công nghiệp game mang tên *“DOOM Khải Huyền”* (Masters of Doom), xuất bản tại Mỹ năm 2003 và nhanh chóng được chuyển ngữ phát hành rộng rãi.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060709.webp)

Cuốn sách ghi lại chi tiết câu chuyện hậu trường phát triển dòng game bắn súng kinh điển *DOOM*, khắc họa chặng đường từ những ngày đầu khởi nghiệp tay trắng của hai chàng trai trẻ mang hoài bão lớn cho đến khi họ định hình lại toàn bộ ngành công nghiệp trò chơi điện tử toàn cầu.

Tác phẩm được biên soạn vô cùng cuốn hút, giúp người đọc thấu hiểu sâu sắc những quy luật ngầm của ngành công nghiệp game cũng như cuộc đời thăng trầm của một lập trình viên.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060710.webp)

Một trong hai nhân vật chính của tác phẩm là kỹ sư lập trình huyền thoại John D. Carmack (sinh năm 1970) – người chịu trách nhiệm viết toàn bộ phần mã nguồn cốt lõi của game *DOOM*. Xuất thân từ một sinh viên bỏ học giữa chừng, anh đã tự học và vươn lên thành một trong những lập trình viên có sức ảnh hưởng lớn nhất thế giới.

Trong sách có ghi lại một câu chuyện nhỏ thú vị về cuộc sống cá nhân của anh:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060711.webp)

Thuở nhỏ, Carmack là một cậu bé cực kỳ say mê máy tính, tính cách lập dị khiến anh sống cô lập và xa lánh cả người thân lẫn bạn bè cùng lớp. Người bạn duy nhất bầu bạn cùng anh trong những năm tháng tuổi thơ là chú mèo cưng mang tên Mitzi. Mỗi khi anh cắm cúi lập trình viết code, chú mèo lại nằm yên vị trên nóc màn hình máy tính để quan sát anh làm việc.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060402.webp)

Năm 19 tuổi khi quyết định dọn ra riêng để sang bang khác lập nghiệp, anh ra đi tay trắng và tài sản gia đình duy nhất anh mang theo chính là chú mèo Mitzi. Nó tiếp tục đồng hành cùng anh trong căn phòng trọ thuê chật hẹp, thậm chí trong bảng danh sách nhân sự chính thức của công ty game do anh sáng lập, Carmack cũng trân trọng điền tên chú mèo cưng này vào danh sách.

Tuy nhiên vào giai đoạn phát triển nước rút của dự án game *DOOM*, do áp lực công việc và không gian sống thay đổi, chú mèo Mitzi trở nên cáu kỉnh, thường xuyên đi vệ sinh bừa bãi và đã cào rách nát bộ ghế sofa da đắt tiền mới mua của anh.

Đứng trước sự việc này, Carmack đã đưa ra quyết định vô cùng dứt khoát: bất chấp tình cảm gắn bó suốt nhiều năm trời, anh mang chú mèo Mitzi gửi vào trại thu nhận động vật vô chủ của thành phố và hoàn toàn không bận tâm đến nó nữa.

Các đồng nghiệp tại văn phòng vô cùng ngạc nhiên và lên tiếng chất vấn: *"Nếu gửi vào trại, chú mèo đó rất có thể sẽ bị tiêm mũi tiêm nhân đạo nếu không có người nhận nuôi đấy"*. Nhưng Carmack lạnh lùng trả lời: *"Sự hiện diện của Mitzi đang gây ra những tác động tiêu cực đến hiệu suất cuộc sống và công việc của tôi"*, rồi lập tức quay lưng tiếp tục cặm cụi gõ phím viết code.

Tác giả cuốn sách nhận định câu chuyện nhỏ này phản ánh chân thực nét tính cách đặc trưng của John Carmack: **Anh chỉ dành sự quan tâm và tập trung tuyệt đối cho những dòng mã nguồn của mình. Đối với anh, mọi khía cạnh khác của cuộc sống đều là thứ yếu, và bất kỳ nhân tố nào gây ảnh hưởng tiêu cực đến tiến trình lập trình của anh đều bắt buộc phải bị loại bỏ thẳng tay.**

Sự lạnh lùng và lý trí thái quá này không chỉ áp dụng với thú cưng mà còn được anh áp dụng với cả bạn bè đồng hành và chính bản thân mình. Carmack hầu như không lưu giữ bất kỳ bức ảnh cá nhân nào, không giữ lại các tài liệu kỷ niệm hay các sản phẩm phần mềm thời kỳ đầu của mình vì coi chúng là vô giá trị. Trong công việc, nếu anh nhận thấy một nhân sự không mang lại giá trị gia tăng thực tế cho sản phẩm phần mềm, anh sẽ yêu cầu sa thải ngay lập tức. Hai trong số các nhà đồng sáng lập ban đầu của *DOOM* đã bị sa thải trực tiếp dưới bàn tay sắt của anh.

Nét tính cách lạnh lùng, có phần tàn nhẫn này khiến anh rất khó hòa đồng với mọi người xung quanh, không khí văn phòng luôn trở nên căng thẳng và ngột ngạt mỗi khi có sự xuất hiện của anh.

Tuy nhiên, tác giả cuốn sách nhận định: **Chính nét tính cách lý trí cực đoan đó đã làm nên sự vĩ đại của John Carmack.** Nhờ khả năng tập trung tinh thần tuyệt đối và loại bỏ hoàn toàn các yếu tố xao nhãng xung quanh, anh đã sáng tạo nên những thuật toán đồ họa 3D mang tính cách mạng đầu tiên trên thế giới chạy mượt mà trên nền tảng phần cứng máy tính vô cùng yếu kém thời bấy giờ. Mọi đoạn mã nguồn không đóng góp trực tiếp vào hiệu năng hệ thống đều bị anh lược bỏ không thương tiếc để tạo nên cấu trúc code tối giản và hiệu quả nhất.

Lấy ví dụ, phần cứng thời kỳ đó không đủ sức mạnh tính toán để dựng toàn bộ không gian 3D hoàn chỉnh. Carmack đã đưa ra ý tưởng táo bạo: loại bỏ hoàn toàn việc kết xuất trần nhà và sàn nhà, chỉ tập trung tính toán dựng các mảng tường dọc ở hai bên để tạo ảo giác chiều sâu 3D cho người chơi (hình dưới). Giải pháp tối giản này có mối liên hệ mật thiết với tư duy lược bỏ mọi chi tiết thừa trong tính cách của anh:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060403.webp)

Nhiều lập trình viên xuất sắc hàng đầu thế giới cũng sở hữu những nét tính cách lập dị và rất khó giao tiếp. Ví dụ như Richard Stallman với tinh thần cực đoan tuyệt đối dành cho phần mềm tự do, hay Linus Torvalds với thói quen thẳng thừng chế giễu các lập trình viên nộp những đoạn code ngớ ngẩn trên cộng đồng. Có lẽ tư duy ưu tiên tối đa cho chất lượng mã nguồn (code-first) luôn có xu hướng đối nghịch với các quy chuẩn giao tiếp xã giao thông thường, và những người có tính cách quá hiền hòa, hòa đồng đôi khi lại khó đạt tới đỉnh cao trong lĩnh vực lập trình chuyên sâu.

## 活动消息

**1、[Hội thảo kỹ thuật Cloud Native & Cơ sở hạ tầng của ByteDance (Kỳ 2)](https://www.bagevent.com/event/sales/zzze3q8v8uvz6ff7fjpwe4wx9jt5rvrj)**

Tiếp nối hội thảo tuần trước, vào chiều thứ Bảy tuần này (ngày 10 tháng 6), đội ngũ hạ tầng của ByteDance tiếp tục phối hợp cùng cộng đồng Juejin tổ chức buổi giao lưu kỹ thuật kỳ 2.

Chủ đề xuyên suốt của chuỗi hội thảo là chia sẻ các kinh nghiệm thực tế của ByteDance trong việc chuyển đổi các kiến trúc phần mềm từ dạng tự lưu trữ (Self-hosted) truyền thống sang mô hình hạ tầng đám mây (Cloud-native).

Nếu như kỳ 1 tập trung vào Serverless, nội dung kỳ này sẽ đi sâu vào việc triển khai và tối ưu hóa các phần mềm cơ sở hạ tầng lớn trong doanh nghiệp, bao gồm 4 bài chia sẻ chuyên sâu từ các kỹ sư trưởng của ByteDance:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060801.webp)

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060803.webp)

Địa điểm tổ chức hội thảo trực tiếp lần này được đặt tại Trung tâm Cao Hà Kính, số 1520 đường Cổ Mỹ, quận Từ Hối, Thượng Hải (đây chính là khu văn phòng làm việc lớn của ByteDance tại Thượng Hải). Bạn đọc tại Thượng Hải có thể đăng ký tham gia trực tiếp để kết hợp tham quan văn phòng hãng, hoặc đăng ký theo dõi buổi phát sóng trực tuyến miễn phí tại [Đăng ký hội thảo ByteDance](https://www.bagevent.com/event/sales/zzze3q8v8uvz6ff7fjpwe4wx9jt5rvrj) để nhận nhiều phần quà lưu niệm hấp dẫn từ ban tổ chức.

## 科技动态

1、[Mẫu đồng hồ đeo tay độc đáo chế tạo từ bo mạch thử nghiệm breadboard](https://ingep.net/breadboardwatch/)

Một lập trình viên đam mê điện tử đã thiết kế thành công mẫu đồng hồ đeo tay độc đáo sử dụng tấm breadboard (bo mạch thử nghiệm nhanh mạch điện) làm khung máy:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052801.webp)

Anh đã trực tiếp cắm các linh kiện bao gồm pin nguồn, IC định thời, mạch vi xử lý và màn hình hiển thị LED lên các lỗ cắm của tấm breadboard và cố định nó vào dây đeo đồng hồ. Mã nguồn firmware vận hành đồng hồ được chia sẻ công khai tại [Breadboardwatch GitHub](https://github.com/ingepnet/breadboardwatch):

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052802.webp)

2、[Mỹ xem xét quy định bắt buộc trang bị phanh khẩn cấp tự động cho ô tô con](https://arstechnica.com/cars/2023/05/automatic-emergency-braking-should-become-mandatory-feds-say/)

Bộ Giao thông Vận tải Mỹ đang lấy ý kiến dự thảo quy định bắt buộc tất cả các dòng xe ô tô con mới bán ra tại thị trường nước này phải được trang bị hệ thống phanh khẩn cấp tự động (AEB):

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060202.webp)

Hệ thống sử dụng cảm biến radar hoặc camera đặt phía trước xe để liên tục giám sát chướng ngại vật; khi phát hiện phương tiện phía trước phanh gấp hoặc có người đi bộ băng qua đường đột ngột, hệ thống sẽ phát âm thanh cảnh báo và chủ động kích hoạt lực phanh khẩn cấp để tránh va chạm. Dự thảo hướng tới việc biến hệ thống AEB thành trang bị an toàn bắt buộc tương tự như dây đai an toàn hay túi khí. Các số liệu nghiên cứu ước tính quy định này sẽ giúp ngăn ngừa khoảng 24.000 vụ tai nạn giao thông và giảm thiểu 360 ca tử vong mỗi năm tại Mỹ.

3、[Mẫu máy ảnh Paragraphica không sử dụng ống kính quang học](https://bjoernkarmann.dk/project/paragraphica)

Một nhà thiết kế người Hà Lan đã ra mắt một thiết bị ghi hình độc đáo: máy ảnh hoàn toàn không có ống kính:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060203.webp)

Phần trước của máy ảnh được bịt kín hoàn toàn bằng một tấm kim loại màu đỏ mô phỏng vòi của loài mũi sao. Khi người dùng bấm nút chụp, thiết bị sẽ tự động thu thập tọa độ vị trí GPS hiện tại, phân tích thời gian trong ngày và phác họa thô bố cục cảnh quan xung quanh để gửi tới máy chủ AI.

Hệ thống AI sẽ tự động biên soạn một đoạn văn bản mô tả chi tiết về cảnh quan thực tế tại địa điểm đó:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060204.webp)

Đoạn văn bản này sau đó được chuyển tiếp tới công cụ Generative AI vẽ tranh để tự động sinh ra một bức ảnh phong cảnh giả lập tương ứng. Kết quả hình ảnh sinh ra có độ tương đồng đáng kinh ngạc với thực tế, dưới đây là ảnh chụp thực tế của góc phố:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060205.webp)

Và đây là bức ảnh do máy ảnh không ống kính Paragraphica tự động sinh ra dựa trên tọa độ GPS và văn bản mô tả của AI:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060206.webp)

4、[Mô hình nhà máy sản xuất lúa thông minh trong nhà tại An Huy](http://ah.people.com.cn/n2/2023/0606/c227131-40445805-7.html)

Một nhà máy nông nghiệp thông minh tại thành phố Lục An, An Huy đã triển khai mô hình trồng lúa nước hoàn toàn trong nhà kính sử dụng hệ thống khay gieo hạt tiêu chuẩn:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060703.webp)

Nhờ áp dụng quy trình nuôi trồng khép kín, hệ thống máy tính có thể tự động kiểm soát tối ưu các thông số nhiệt độ, độ ẩm của không khí và thực hiện châm chất dinh dưỡng chính xác cho từng khay lúa:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060704.webp)

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060705.webp)

Mặc dù có ưu điểm tiết kiệm tối đa diện tích đất canh tác ngoài tự nhiên và giải phóng sức lao động chân tay, chi phí đầu tư ban đầu cùng lượng điện năng tiêu thụ cho hệ thống đèn chiếu sáng giả lập ánh nắng mặt trời của nhà máy là rất lớn, gây khó khăn cho việc cạnh tranh thương mại với lúa nước canh tác truyền thống nếu không có các giải pháp tối ưu hóa năng lượng. (Đóng góp của [@shencn](https://github.com/ruanyf/weekly/issues/3169))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060706.webp)

## Bài viết

1\. [Lời giải chi tiết bài toán cơ học vật lý trong đề thi đại học Trung Quốc năm nay](https://m.weibo.cn/detail/4910316167105260)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060804.webp)

Bài phân tích lời giải chi tiết cho câu hỏi vật lý lý thuyết hấp dẫn trong đề thi tuyển sinh đại học (Gaokao) toàn quốc vừa qua: *"Giả sử tàu đổ bộ Hằng Nga 5 có khối lượng m đặt trên bề mặt Mặt Trăng có gia tốc trọng trường bằng 1/6g. Biết góc nghiêng của 4 chân đáp của tàu so với phương thẳng đứng là θ, hãy tính lực nén tác động lên bề mặt Mặt Trăng của mỗi chân đáp"*.

2\. [Google DeepMind ứng dụng AI phát hiện các thuật toán sắp xếp mã nguồn mới](https://www.ithome.com/0/698/425.htm)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060805.webp)

Phòng nghiên cứu AI DeepMind của Google công bố dự án AlphaDev ứng dụng phương pháp học máy tăng cường để tự động tìm kiếm và tối ưu hóa các giải thuật sắp xếp dữ liệu (Sorting Algorithms) ở cấp độ mã máy Assembly, giúp tăng tốc độ sắp xếp dữ liệu lên tới 70% so với các thuật toán tối ưu do con người viết trước đây. Nghiên cứu cho thấy trong tương lai AI hoàn toàn có khả năng tự động tối ưu hóa cấu trúc thuật toán nền tảng của hệ thống.

3\. [Bài viết phân tích nguyên nhân tụt hậu của ngành công nghiệp điện tử Liên Xô](https://mp.weixin.qq.com/s/Vqd2tg0Rlx0bSaPxUYc9Cg)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060115.webp)

Trong thời kỳ đầu của kỷ nguyên bóng chân không, ngành công nghiệp điện tử của Liên Xô sở hữu thế mạnh rất lớn. Bài viết phân tích các quyết định sai lầm trong việc định hướng công nghệ và cơ chế quản lý tập trung dẫn đến việc ngành công nghiệp bán dẫn của họ bị tụt hậu xa so với các quốc gia phương Tây sau đó.

4\. [Mẹo cấu hình trình duyệt Firefox trên Android luôn sử dụng giao diện Desktop](https://www.reddit.com/r/firefox/comments/p38p6t/guide_how_to_always_use_desktop_view_in_firefox/)（Tiếng Anh）

Theo mặc định, các trình duyệt di động luôn ưu tiên tải trang giao diện tối giản cho điện thoại. Bài viết hướng dẫn cấu hình chi tiết trong phần cài đặt ẩn của Firefox Android để ép trình duyệt luôn ưu tiên tải giao diện máy tính (Desktop View) cho mọi trang web truy cập.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051804.webp)

5\. [Phương pháp đếm số lượng phần tử con của container bằng thuộc tính CSS mới](https://ishadeed.com/article/conditional-css-has-nth-last-child/)（Tiếng Anh）

Bài viết hướng dẫn lập trình viên tận dụng sức mạnh của các bộ chọn CSS thế hệ mới là `:has()` và `:nth-last-child()` để thiết lập các quy tắc định dạng giao diện động dựa trên việc tính toán chính xác số lượng thẻ con nằm trong một thẻ cha (ví dụ thay đổi bố cục lưới khi danh sách có trên 5 phần tử) mà không cần viết mã JS.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051810.webp)

6\. [Tìm hiểu chi tiết cơ chế hoạt động của hệ thống Index trong PostgreSQL](https://blog.mastermind.dev/indexes-in-postgresql)（Tiếng Anh）

Bài viết khoa học phổ thông giới thiệu chi tiết cấu trúc dữ liệu cây B-Tree và nguyên lý hoạt động của các bộ chỉ mục (Indexes) trong hệ quản trị cơ sở dữ liệu PostgreSQL, giúp lập trình viên tối ưu hóa tốc độ truy vấn cho các bảng dữ liệu lớn.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051812.webp)

7\. [Liệu thuật toán lọc thư rác của Gmail có đang bóp nghẹt các máy chủ email độc lập](https://tutanota.com/blog/posts/gmail-independent-email/)（Tiếng Anh）

Bài viết phân tích thực trạng khó khăn của các lập trình viên khi tự thiết lập máy chủ mail cá nhân (Self-hosted mail server). Các email gửi từ các IP máy chủ độc lập này thường xuyên bị hệ thống bảo mật của Gmail tự động đánh dấu là thư rác (Spam) hoặc áp đặt độ trễ nhận thư rất lớn, gây khó khăn cho việc duy trì sự đa dạng của hệ sinh thái email toàn cầu.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042906.webp)

8\. [Bài viết phân tích so sánh chi tiết giữa hai giao thức REST API và gRPC](https://kreya.app/blog/rest-vs-grpc/)（Tiếng Anh）

REST và gRPC hiện là hai phương thức thiết kế giao tiếp dịch vụ (API) phổ biến nhất trong kiến trúc hệ thống. Bài viết so sánh chi tiết sự khác biệt về hiệu suất truyền tải, định dạng dữ liệu (JSON so với Protocol Buffers) và các tình huống ứng dụng tối ưu cho từng giải pháp.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042910.webp)

## 工具

1、[Docker-OSX: Docker Container hỗ trợ chạy máy ảo macOS](https://github.com/sickcodes/Docker-OSX)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011501.webp)

Dự án mã nguồn mở cung cấp tệp cấu hình Docker giúp nhà phát triển nhanh chóng khởi chạy một hệ điều hành macOS giả lập trong môi trường container phục vụ công tác kiểm thử phần mềm.

2、[Tabby: Trợ lý viết code AI nguồn mở hỗ trợ chạy ngoại tuyến](https://github.com/TabbyML/tabby)

Giải pháp mã nguồn mở thay thế cho GitHub Copilot: hỗ trợ doanh nghiệp tự thiết lập máy chủ AI viết mã riêng trên hạ tầng nội bộ để bảo mật thông tin mã nguồn và cho phép lập trình viên sử dụng ngoại tuyến (offline) hoàn toàn.

3、[undb: Tiện ích cơ sở dữ liệu no-code gọn nhẹ lưu trữ dạng tệp tin](https://github.com/undb-xyz/undb)

Một ứng dụng web cung cấp giao diện quản lý cơ sở dữ liệu dạng kéo thả no-code trực quan, toàn bộ dữ liệu bảng biểu được lưu trữ gọn gàng dưới dạng một tệp tin đơn nhất trên máy tính. (Đóng góp của [@nichenqin](https://github.com/ruanyf/weekly/issues/3172))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060708.webp)

4、[jelBAN.js: Thư viện JavaScript hỗ trợ lọc và kiểm tra định dạng email](https://github.com/Fcmam5/jelban-js)

Thư viện JS nhỏ gọn giúp các nhà phát triển tích hợp nhanh tính năng kiểm tra tính hợp lệ của địa chỉ email khi người dùng đăng ký tài khoản, hỗ trợ tự động phát hiện và chặn các email ảo dùng một lần (disposable emails) hoặc các email alias.

5、[Herowand Editor: Công cụ web trực quan hóa cấu trúc dữ liệu](https://editor.herowand.com/)

Tiện ích web hỗ trợ lập trình viên dán các đoạn dữ liệu thô định dạng JSON, XML, YAML hoặc TOML lên hệ thống để tự động chuyển đổi sang giao diện sơ đồ cây trực quan giúp dễ dàng đọc hiểu cấu trúc dữ liệu.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041703.webp)

6、[sqlite-gui: Trình quản lý cơ sở dữ liệu SQLite siêu nhẹ cho Windows](https://github.com/little-brother/sqlite-gui)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041904.webp)

Phần mềm giao diện đồ họa quản trị CSDL SQLite dành riêng cho Windows, sở hữu dung lượng siêu nhẹ, tốc độ khởi động nhanh và tích hợp đầy đủ tính năng truy vấn.

7、[val town: Nền tảng viết và thực thi Cloud Functions trực tiếp trên Web](https://www.val.town/)

Dịch vụ web miễn phí cung cấp môi trường chạy các đoạn mã script ngắn trực tiếp trên trình duyệt, hỗ trợ người dùng viết nhanh các API nhỏ, lên lịch chạy tác vụ tự động mà không cần cấu hình server.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042004.webp)

8、[stable-diffusion-videos: Công cụ AI sinh video chuyển cảnh mượt mà](https://github.com/nateraw/stable-diffusion-videos)

Tiện ích ứng dụng mô hình Stable Diffusion: người dùng cung cấp hai bức ảnh đầu vào A và B, AI sẽ tính toán và tự động sinh ra một đoạn video ngắn mô tả quá trình biến đổi hình ảnh mượt mà từ bức ảnh A sang bức ảnh B.

9、[Helix: Trình soạn thảo văn bản hiện đại viết bằng Rust](https://helix-editor.com/)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090702.webp)

Trình soạn thảo văn bản dòng lệnh được lập trình hoàn toàn bằng ngôn ngữ Rust. Khác biệt với NeoVim, Helix được tích hợp sẵn toàn bộ các tính năng hỗ trợ lập trình như tự động hoàn thành, định dạng code mà không yêu cầu người dùng phải tự cài đặt thêm các plugin bên ngoài.

10、[Chitchatter: Ứng dụng phòng chat P2P bảo mật trên nền web](https://chitchatter.im/)

Một ứng dụng trò chuyện trực tuyến nguồn mở sử dụng giao thức WebRTC: cho phép người dùng tạo nhanh phòng chat và chia sẻ liên kết cho bạn bè để trò chuyện trực tiếp với nhau theo cơ chế ngang hàng (P2P), không lưu trữ thông tin trò chuyện trên bất kỳ máy chủ trung gian nào.

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090703.webp)

11、[Aether: Ứng dụng xây dựng diễn đàn thảo luận phi tập trung qua P2P](https://getaether.net/)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090806.webp)

Phần mềm cài đặt trên máy tính hỗ trợ người dùng tự thiết lập các mạng lưới diễn đàn thảo luận nội bộ chạy trên mạng ngang hàng P2P: mọi bài đăng và phản hồi sẽ được đồng bộ trực tiếp giữa các máy thành viên trong nhóm mà không cần máy chủ trung tâm.

## 资源

1、[Posters: Thư viện poster minh họa kiến thức khoa học máy tính](https://github.com/corkami/pics/blob/master/binary/README.md)

Kho lưu trữ GitHub tổng hợp hàng trăm mẫu thiết kế poster đồ họa đẹp mắt giải thích trực quan các kiến thức kỹ thuật (như bảng mã ASCII, cấu trúc file nhị phân) do tác giả tự thiết kế.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122703.webp)

2、[Passkeys.io: Trang web trải nghiệm phương thức xác thực không mật khẩu](https://www.passkeys.io/)

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060501.webp)

Trang web thử nghiệm do FIDO Alliance phát triển giúp người dùng trải nghiệm thực tế quy trình đăng nhập tài khoản an toàn sử dụng tính năng sinh trắc học vân tay hoặc khuôn mặt của điện thoại (Passkeys) để thay thế hoàn toàn mật khẩu gõ phím truyền thống.

3、[Trang web tự động cào và tóm tắt tin tức Hacker News bằng AI](https://hackernews.betacat.io/)

Tiện ích tự động cào các bài viết thịnh hành nhất trên trang Hacker News mỗi ngày và gọi API ChatGPT để viết các đoạn tóm tắt nội dung ngắn gọn giúp tiết kiệm thời gian đọc tin của các nhà phát triển. (Đóng góp của [@polyrabbit](https://github.com/ruanyf/weekly/issues/3171) - Xem thêm [bài viết giới thiệu chi tiết](https://blog.betacat.io/post/2023/06/summarize-hacker-news-by-chatgpt/)).

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060707.webp)

4\. [Google Cloud Generative AI: Khóa học AI tạo sinh miễn phí từ Google](https://www.cloudskillsboost.google/paths/118)

Hệ thống các khóa học trực tuyến viết bằng tiếng Anh hoàn toàn miễn phí do Google Cloud thiết lập, giới thiệu các nguyên lý hoạt động của mô hình ngôn ngữ lớn và cách thức ứng dụng Generative AI vào thực tiễn.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060503.webp)

## 图片

1、**YBC 7289: Phiến đất sét Babylon cổ đại chứng minh sự hiểu biết về căn bậc hai**

YBC 7289 là ký hiệu lưu trữ của một phiến đất sét nhỏ có từ thời cổ đại Babylon, được xác định chế tác trong khoảng từ năm 1600 TCN đến 1800 TCN:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022123001.webp)

Phiến đất sét quý hiếm này được nhà tài phiệt J.P. Morgan mua lại và hiến tặng cho Đại học Yale vào năm 1909. Điểm giá trị nhất của cổ vật này là nó chứng minh các nhà toán học Babylon cổ đại đã biết cách tính toán giá trị của căn bậc hai của 2 (√2) với độ chính xác kinh ngạc lên tới 99,9999% từ hơn 3.500 năm trước.

Trên bề mặt phiến đất sét có khắc hình một hình vuông cùng các đường chéo và các ký hiệu số dọc theo đường chéo:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022123002.webp)

Các ký hiệu số này được viết theo hệ chữ tượng hình楔形 (Cuneiform) của Babylon cổ đại, biểu thị 4 nhóm số: 1, 24, 51 và 10:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022123003.webp)

Do người Babylon sử dụng hệ đếm cơ số 60 (sexagesimal), khi chúng ta chuyển đổi 4 nhóm số trên sang hệ cơ số 10 thập phân thông thường sẽ có kết quả phép tính: 1 + 24/60 + 51/3600 + 10/216000 = **1,41421296296**:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022123004.webp)

Kết quả này trùng khớp hoàn hảo với giá trị thực tế của √2 (khoảng 1,41421356...) tới chữ số thập phân thứ 6, đạt độ chính xác gần như tuyệt đối:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022123005.webp)

2、**Hình ảnh hệ thống hàng rào biên giới Mỹ - Mexico đồ sộ**

Bức tường rào biên giới khổng lồ ngăn cách ranh giới địa lý giữa hai quốc gia Mỹ và Mexico nhằm ngăn chặn dòng người nhập cư trái phép:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060806.webp)

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060807.webp)

Tổng chiều dài biên giới giữa hai nước kéo dài khoảng 3.145 km, trong đó hệ thống hàng rào thép kiên cố đã được xây dựng phủ kín hơn 1.000 km và vẫn đang tiếp tục được kéo dài thêm, trở thành một trong những dự án xây dựng hàng rào biên giới quy mô lớn nhất thế giới:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080505.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080507.webp)

## ✍️ Bài đọc thêm

### Định luật Bushnell trong triết lý thiết kế trò chơi điện tử

Nolan Bushnell là nhà khởi nghiệp nổi tiếng – người sáng lập nên tập đoàn Atari danh tiếng thời kỳ đầu của ngành công nghiệp game:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121805.webp)

Trong dự án trò chơi đầu tay của mình, ông thiết kế bảng điều khiển bao gồm 4 nút bấm có ngoại hình giống hệt nhau nhưng đảm nhận các chức năng hoàn toàn khác biệt. Sau khi phát hành, hãng nhận về rất nhiều lời phàn nàn từ người chơi vì cơ chế điều khiển quá phức tạp và dễ gây nhầm lẫn.

Qua sự cố đó, ông đã đúc kết nên một triết lý thiết kế game kinh điển: *“Một trò chơi xuất sắc cần có cơ chế điều khiển đơn giản giúp người chơi làm quen ngay lập tức, nhưng phải giữ được độ khó và tính thử thách tăng dần trong quá trình chơi”*. Triết lý này sau đó được giới công nghệ gọi là **“Định luật Bushnell”** với câu đúc kết nổi tiếng: **“Easy to learn, hard to master”** (Dễ học nhưng khó thành thạo).

Tập đoàn game nổi tiếng Blizzard đã coi định luật này như tôn chỉ vàng trong mọi dự án thiết kế game của họ.

Triết lý này có thể ứng dụng rộng rãi cho mọi sản phẩm hướng tới số đông: sản phẩm ban đầu phải cực kỳ dễ tiếp cận để thu hút lượng lớn người dùng dùng thử, nhưng phải giữ chân họ bằng các tính năng chuyên sâu đầy thử thách phía sau.

## Lịch sử tuần này

- 2022年（第 211 期）：[Kinh tế số: Thảo luận về cách thức các giao dịch vật phẩm ảo đóng góp vào GDP](http://www.ruanyifeng.com/blog/2022/06/weekly-issue-211.html)
- 2021年（第 161 期）：[Giáo dục: Góc nhìn về việc giảm quy mô tuyển sinh các ngành Thạc sĩ học thuật](http://www.ruanyifeng.com/blog/2021/06/weekly-issue-161.html)
- 2020年（第 111 期）：[Sản phẩm: Phân tích các lỗi thiết kế phổ biến của hệ thống Tivi thông minh](http://www.ruanyifeng.com/blog/2020/06/weekly-issue-111.html)
- 2019年（第 61 期）：[Thị trường lao động: Tại sao rào cản chuyển hướng sự nghiệp sang mảng Front-end ngày càng cao](http://www.ruanyifeng.com/blog/2019/06/weekly-issue-61.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes organization and coordination easy.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
