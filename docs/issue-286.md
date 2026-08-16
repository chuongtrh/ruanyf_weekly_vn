# Bản tin chia sẻ công nghệ (Số 286): Giải pháp cho đèn chỉ thị màu xanh dương

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3814) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010607.webp)

Tháng trước, Thư viện Thành phố Bắc Kinh đã chính thức mở cửa đón khách. Công trình này còn có tên gọi khác là "Rừng Sách", với hệ thống cột chống màu trắng mô phỏng những thân cây cổ thụ, lối đi uốn lượn ở giữa tượng trưng cho thung lũng, tạo cho độc giả cảm giác như đang được đọc sách giữa thiên nhiên hoang dã. (Nguồn: [iarch](http://www.iarch.cn/thread-45324-1-1.html))

## 蓝色指示灯的解决方案

Bạn có bao giờ chú ý đến màu sắc của đèn chỉ thị trên các thiết bị điện tử trong nhà mình không?

Thông thường, các đèn chỉ thị màu vàng hoặc xanh lá cây mang lại cảm giác dễ chịu, dịu mắt và thân thiện hơn cho người dùng.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010705.webp)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010914.webp)

Đáng sợ nhất chính là các đèn chỉ thị màu xanh dương (xanh nước biển).

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010915.webp)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010706.webp)

Các nghiên cứu khoa học [từ lâu đã chứng minh](https://wjw.beijing.gov.cn/bmfw_20143/jkzs/jksh/202201/t20220105_2582843.html) việc **tiếp xúc lâu ngày với nguồn ánh sáng xanh dương gây hại nghiêm trọng cho sức khỏe con người**.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011201.webp)

Dưới đây là một số thông tin trích dẫn khoa học:

> "Dải ánh sáng xanh năng lượng cao bước sóng ngắn từ 400nm đến 460nm mới là tác nhân chính ảnh hưởng trực tiếp đến sức khỏe.
> 
> Tác hại lớn nhất của ánh sáng xanh là gây ra các tổn thương quang học cho võng mạc, đẩy nhanh quá trình thoái hóa oxy hóa của tế bào vùng hoàng điểm mắt. Đồng thời, ánh sáng xanh còn làm gia tăng tình trạng mỏi mắt, khô mắt và làm suy giảm màng nước mắt."

Nói một cách ngắn gọn, ánh sáng xanh dương gây hại cho mắt và đẩy nhanh tiến trình lão hóa của tế bào thị lực.

Không dừng lại ở đó, ánh sáng xanh dương còn gây ức chế sản sinh hormone melatonin gây mất ngủ. Nếu trong phòng ngủ có đặt thiết bị phát ra ánh sáng xanh dương rực rỡ, giấc ngủ của bạn chắc chắn sẽ bị ảnh hưởng tiêu cực. Ngoài ra, loại ánh sáng này còn tác động không tốt đến sự phát triển bình thường của trẻ nhỏ.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010918.webp)

Đó là nguyên nhân giải thích vì sao thị trường hiện nay xuất hiện rất nhiều sản phẩm "chống ánh sáng xanh", và khi bạn đi cắt kính thuốc, cửa hàng luôn tư vấn xem bạn có nhu cầu làm thêm [lớp phủ chống ánh sáng xanh](https://jres2023.xhby.net/index/201910/t20191031_6387055.shtml) hay không (dù trên thực tế hiệu quả bảo vệ thực tế của nó vẫn còn tranh cãi).

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010919.webp)

Tác hại của ánh sáng xanh dương xuất phát từ mức năng lượng cực cao của bước sóng này. Trong dải ánh sáng khả kiến (đỏ, cam, vàng, lục, lam, chàm, tím), bước sóng càng lùi về sau thì tần số càng cao và năng lượng càng lớn. Trong ba màu sắc cơ bản (đỏ, xanh lá, xanh dương), màu xanh dương sở hữu mức năng lượng lớn nhất.

Mặc dù vậy, không hiểu vì lý do gì, rất nhiều nhà sản xuất thiết bị điện tử - đặc biệt là các hãng phần cứng Trung Quốc - lại rất ưa chuộng việc sử dụng đèn chỉ thị màu xanh dương. Họ dường như cho rằng ánh đèn màu xanh dương mang lại vẻ hiện đại và đậm chất công nghệ hơn cho sản phẩm.

Bộ định tuyến WiFi và đầu thu TV box ở nhà tôi không may đều trang bị đèn chỉ thị nguồn màu xanh dương. Chỉ cần bật thiết bị, ánh đèn xanh dương lại phát ra rực rỡ. Bộ định tuyến đặt trong góc phòng thì có thể khuất tầm nhìn, nhưng đầu thu TV box lại luôn đặt đối diện trực diện với người xem do khu vực nhận tín hiệu hồng ngoại của điều khiển từ xa được thiết kế tích hợp ngay cạnh đèn chỉ thị. Cứ mỗi khi bật TV lên, ánh đèn xanh dương lại rọi thẳng vào mắt khiến tôi vô cùng khó chịu.

Tuần trước, trên diễn đàn Hacker News xuất hiện [một bài chia sẻ kỹ thuật](https://www.fullcircuit.com/blog/fixing-annoying-blue-standby-lights) của một lập trình viên phàn nàn về đúng chủ đề này, thu hút rất nhiều lượt thảo luận và chia sẻ từ những người cùng chung cảnh ngộ.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010920.webp)

Họ đã đề xuất rất nhiều giải pháp thủ công để xử lý vấn đề đèn chỉ thị màu xanh dương này. Cách thức đơn giản nhất chính là sử dụng một miếng băng keo điện màu đen để dán đè lên phần đèn.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010921.webp)

Băng keo điện màu đen có đặc tính cản sáng hoàn hảo, ngăn hoàn toàn ánh sáng xanh lọt ra ngoài. Hơn nữa, chất liệu băng keo điện chịu được nhiệt độ cao và có độ bền bám dính tốt, rất thích hợp sử dụng trên vỏ các thiết bị điện tử tỏa nhiệt.

Trong trường hợp bạn vẫn muốn giữ lại một phần ánh sáng mờ để tiện theo dõi trạng thái hoạt động của thiết bị, giải pháp dán băng keo đen sẽ không phù hợp. Thay vào đó, bạn có thể sử dụng sơn móng tay màu đen để phủ lên bề mặt đèn.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010922.webp)

Ưu điểm của sơn móng tay màu đen là người dùng có thể chủ động điều chỉnh độ dày của lớp sơn phủ: phủ dày để cản sáng hoàn toàn hoặc phủ mỏng để ánh sáng mờ lọt qua tùy ý. Tuy nhiên, cả hai phương án trên đều không phù hợp cho TV box, bởi khi che hoàn toàn ánh sáng xanh thì cũng đồng thời chặn luôn đường truyền tín hiệu hồng ngoại của điều khiển từ xa.

Tác giả bài viết đã đề xuất một giải pháp xử lý cực kỳ thông minh: sử dụng giấy gói kẹo màu đỏ trong suốt.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010923.webp)

Khi bạn dán một lớp giấy kẹo màu đỏ trong suốt đè lên đèn xanh dương, ánh sáng xanh sẽ được lọc và chuyển sang sắc độ rất dịu mắt, đồng thời lớp giấy này vẫn cho phép tia hồng ngoại của điều khiển đi qua bình thường mà không gây ảnh hưởng đến hoạt động của thiết bị.

Thử nghiệm thực tế của tác giả cho thấy, ngay cả khi dán chồng 2 lớp giấy kẹo màu đỏ, điều khiển từ xa vẫn hoạt động nhạy bén trong khi ánh sáng xanh độc hại đã được triệt tiêu gần như hoàn toàn. Nếu các thiết bị điện tử trong nhà bạn cũng đang gặp sự cố tương tự với đèn chỉ thị xanh dương, hãy thử áp dụng mẹo nhỏ hữu ích này.

## [详细日程] 掘金年度技术演讲

Tuần trước, bản tin đã đăng tải thông tin giới thiệu về sự kiện công nghệ quy mô "Diễn thuyết Công nghệ Thường niên Juejin", diễn ra vào ngày 20 tháng 1 tại Khách sạn Renaissance Thâm Quyến, mọi người còn nhớ chứ?

Đây là hoạt động thường niên trọng điểm của cộng đồng Xitu Juejin nên ban tổ chức đầu tư rất nhiều nguồn lực chuẩn bị và mời nhiều diễn giả uy tín trong ngành tham gia. Hiện tại, ban tổ chức đã công bố lịch trình chi tiết các phiên phát biểu. Quý độc giả có thể tham khảo lịch trình dưới đây để lựa chọn chủ đề quan tâm:

**Phiên toàn thể chính (9:30-12:30)**

Diễn ra vào sáng ngày 20 tháng 1 với các bài phát biểu của các chuyên gia công nghệ hàng đầu đến từ ByteDance, NVIDIA, Datastrato, Huawei Noah's Ark Lab, Jina AI xoay quanh các chủ đề nóng như Frontend, AI và Cloud Native. Chi tiết xem hình minh họa dưới đây:

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011104.webp)

**Phiên chuyên đề: Hệ sinh thái nhà phát triển (14:00-17:00)**

Phiên thảo luận được chia làm hai phần: Chia sẻ chuyên đề và Thảo luận nhóm. Phần chia sẻ chuyên đề gồm 4 bài phát biểu ngắn gọn và cô đọng từ các chuyên gia:

> - Thành Thần (ModelScope): Thảo luận về việc xây dựng hệ sinh thái nhà phát triển trong lòng các tập đoàn lớn.
> - Lâm Lữ Cường (01.AI): Chia sẻ các góc nhìn thực tế về xu hướng mô hình lớn dưới góc độ doanh nghiệp.
> - Trương Chí Bình (Chuyên gia công nghệ Alibaba, thành viên ủy ban DB-GPT): Chia sẻ kinh nghiệm thực chiến từ các dự án lớn.
> - Tô Bằng (Datawhale): Thảo luận về phương pháp xây dựng cộng đồng lập trình viên và tác động của LLM đến cấu trúc cộng đồng.

Phần thảo luận nhóm sẽ là không gian để các kỹ sư tham gia cùng trao đổi quan điểm sâu về xu hướng LLM.

**Phiên chuyên đề: Cơ hội dành cho nhà phát triển (14:00-17:00)**

Gồm 3 phần: Chia sẻ chuyên đề, Thảo luận nhóm và Hỏi đáp tổng kết. Phần phát biểu gồm 4 chủ đề chính:

> - Địch Giai: 《Góc nhìn về thương mại hóa phần mềm mã nguồn mở Trung - Mỹ qua case-study Pulsar》
> - Quách Vĩ: 《Ứng dụng mã nguồn mở làm đòn bẩy thúc đẩy SaaS toàn cầu》
> - Tôn Dục Hạo: 《Tính khả thi của mô hình OpenChat và giải pháp triển khai LLM chi phí thấp》
> - Nghi Bác: 《Tìm kiếm cơ hội khởi nghiệp kỷ nguyên AGI dựa trên nguyên lý triết học AI First》

Phần thảo luận nhóm sẽ chia thành các bàn tròn do chính các chuyên gia dẫn dắt để thảo luận sâu về cơ hội vươn ra thị trường quốc tế, thương mại hóa mô hình lớn và cách tối ưu công nghệ bổ trợ cho hoạt động kinh doanh.

Phần Hỏi đáp cuối buổi là cơ hội để mọi người trực tiếp chất vấn các chuyên gia và tổng kết hoạt động.

**Phiên chuyên đề: Trà đàm Juejin (14:00-17:00)**

Tổ chức dưới dạng bàn tròn thảo luận xoay quanh 3 chủ đề lớn:

> - Chủ đề 1: Những thay đổi lớn nào sẽ diễn ra dưới làn sóng mô hình lớn?
> - Chủ đề 2: Lập trình viên cần làm gì để đón đầu và làm chủ làn sóng AI mới?
> - Chủ đề 3: Bị thay thế hay làm chủ công nghệ, định hướng lộ trình nghề nghiệp cho kỹ sư phần mềm?

Mỗi chủ đề đều có đầy đủ các bước giới thiệu, chia sẻ quan điểm, thảo luận bàn tròn và đúc kết nội dung.

**Phúc lợi đặc biệt**

Sự kiện lần này hoàn toàn miễn phí tham gia, các bạn đừng quên đăng ký nhé. Bạn có thể nhấp vào [liên kết này](https://www.bagevent.com/event/8758229?bag_track=ryf0112), hoặc quét mã QR trên poster ở trên.

Ban tổ chức cũng cung cấp một lượng lớn quà tặng tinh tế, bao gồm túi DuPont "who cares" của Juejin, hộp cơm hai lớp di động đồng thương hiệu Xitu Juejin X A-SOUL, bao thẻ dệt "warm tu you", v.v. (hình dưới). **Chỉ cần chia sẻ poster (liên kết nằm trong thể lệ rút thưởng) là có thể tham gia rút thăm trúng thưởng**, tỷ lệ trúng khoảng 10%, xem chi tiết [Thể lệ rút thăm trúng thưởng](https://bytedance.larkoffice.com/share/base/form/shrcn13nhTRvSG2dPwjOH5zVV4f).

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011105.webp)

## 科技动态

1、[Kỷ lục mới về độ cao rơi tự do của điện thoại di động](https://twitter.com/SeanSafyre/status/1744138937239822685)

Vào ngày 5 tháng 1, một chiếc máy bay Boeing 737 Max 9 của hãng hàng không Alaska Airlines khi đang bay ở độ cao khoảng 5000 mét thì bất ngờ gặp sự cố nổ bung cửa thoát hiểm khỏi thân máy bay.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010801.webp)

Đây là một sự cố cực kỳ kinh hoàng khi thân máy bay xuất hiện một lỗ thủng lớn giữa không trung. Rất may mắn là không có hành khách nào bị hút ra ngoài và chiếc máy bay đã thực hiện hạ cánh khẩn cấp an toàn.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010802.webp)

Mặc dù không có thiệt hại về người, một số thiết bị điện thoại của hành khách đã bị hút bay ra ngoài lỗ thủng, thiết lập kỷ lục về độ cao rơi tự do lớn nhất của thiết bị di động.

Đến nay, hai chiếc điện thoại rơi từ máy bay đã được người dân tìm thấy dưới mặt đất.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010803.webp)

Trong đó, một chiếc iPhone được tìm thấy trong tình trạng hoàn hảo không một vết xước và vẫn đang hoạt động bình thường, nhiều khả năng do rơi trúng thảm cỏ rậm rạp trong rừng. Đây quả thực là một quảng cáo thực tế vô giá cho độ bền của iPhone.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010804.webp)

2、[Cuộc khủng hoảng hạn hán tại kênh đào Panama](https://www.bloomberg.com/news/features/2024-01-03/-270-billion-in-trade-rests-on-finding-a-fix-to-the-panama-canal)

Như chúng ta đã biết, lục địa Nam Mỹ và Bắc Mỹ được kết nối liền mạch với nhau. Để tối ưu hóa tuyến đường vận tải biển giữa bờ Tây và bờ Đông nước Mỹ, từ đầu thế kỷ 20 người Mỹ đã tiến hành xây dựng kênh đào Panama cắt qua eo đất Trung Mỹ (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010608.webp)

Kênh đào Panama là tuyến đường biển ngắn nhất kết nối Thái Bình Dương và Đại Tây Dương, luôn tấp nập các tàu hàng qua lại quanh năm.

Tuy nhiên, kể từ nửa cuối năm ngoái, khu vực kênh đào Panama đã phải đối mặt với đợt hạn hán nghiêm trọng chưa từng có. Tác động của biến đổi khí hậu khiến mực nước kênh đào sụt giảm nghiêm trọng, buộc ban quản lý phải cấm các tàu container tải trọng lớn lưu thông qua kênh và chỉ có thể chờ đợi mực nước dâng lên khi có mưa.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010609.webp)

Bức ảnh trên cho thấy lòng kênh đã cạn nước đến mức trơ cả các nhánh cây dưới đáy. Phía xa là một tàu container cỡ lớn đang bị mắc kẹt không thể di chuyển.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010611.webp)

Phía ngoài cửa âu tàu, mực nước hệ thống cũng đã cạn kiệt trơ đáy.

Thời kỳ đầu xây dựng, các kỹ sư lựa chọn Panama làm vị trí đào kênh không chỉ vì đây là dải đất hẹp nhất Trung Mỹ, mà còn nhờ hệ thống hồ nước tự nhiên sẵn có tại đây giúp giảm thiểu đáng kể khối lượng đất đá cần đào bới (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010610.webp)

Tuy nhiên hiện nay, nguồn nước ngọt cấp vào các hồ tự nhiên này sụt giảm nghiêm trọng khiến mực nước hồ ngày một đi xuống. Tình trạng này gây nên sự tắc nghẽn giao thông nghiêm trọng tại kênh đào, hàng dài tàu bè phải xếp hàng nhiều ngày chờ đợi để được qua kênh.

Sự cố ảnh hưởng lớn đến hoạt động lưu thông hàng hóa của Mỹ. Chính phủ Mỹ đang đánh giá tính khả thi của dự án đào đường hầm dẫn nước ngọt từ các vùng lân cận vào hệ thống hồ để nâng mực nước, nhưng đây là giải pháp dài hạn mất nhiều năm thực hiện. Trước mắt, hoạt động vận tải qua kênh đào Panama sẽ ngày một gặp nhiều khó khăn.

3、[Bàn phím vật lý độc đáo dành cho iPhone](https://www.clicks.tech/)

Một công ty khởi nghiệp tại Anh đã nghiên cứu chế tạo bộ ốp lưng tích hợp bàn phím vật lý dành riêng cho điện thoại iPhone.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010612.webp)

Thiết bị này khiến chiếc điện thoại trông dài hơn đáng kể, nhưng bù lại giao diện màn hình sẽ không bị chiếm dụng bởi bàn phím ảo, giúp tối ưu hóa không gian hiển thị thông tin.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010613.webp)

Đối với những người dùng có nhu cầu soạn thảo văn bản tốc độ cao trên điện thoại, đây hứa hẹn là một công cụ hỗ trợ đắc lực.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010614.webp)

4、[Áo phao bảo vệ chống ngã dành cho người cao tuổi](mymodernmet.com/wearable-airbags-elderly-fall-protection/)

Một doanh nghiệp khởi nghiệp tại Tô Châu mới đây đã giới thiệu sản phẩm "Áo phao chống ngã".

Thiết bị hoạt động dựa trên nguyên lý túi khí an toàn của ô tô để bảo vệ người cao tuổi khi gặp sự cố trượt chân ngã.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011005.webp)

Tận dụng các cảm biến và thuật toán nhận diện hành vi ngã, ngay khi phát hiện người mặc bị mất thăng bằng ngã xuống, hệ thống túi khí sẽ tự động bơm căng chỉ trong vòng 0,18 giây. Thông thường một người ngã xuống đất mất khoảng 0,3 giây, do đó thiết bị hoàn toàn đủ thời gian kích hoạt để bảo vệ cơ thể khỏi chấn thương va đập.

Khi được bơm căng, túi khí sẽ bao bọc toàn bộ các vùng trọng yếu như đầu, vai, lưng và hông. Do chấn thương vùng đầu là nguy hiểm nhất, thiết bị được thiết kế bao bọc đặc biệt dày dặn quanh khu vực này.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011007.webp)

## Bài viết

1\. [Những kỷ niệm tự học lập trình với ngôn ngữ Pascal của tôi](https://justyy.com/archives/64211)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010901.webp)

Niklaus Wirth, cha đẻ của ngôn ngữ lập trình Pascal huyền thoại, đã qua đời trong tuần này. Tác giả chia sẻ lại những kỷ niệm gắn bó của bản thân với ngôn ngữ lập trình Pascal từ những ngày thơ ấu. (Đóng góp của [@DoctorLai](https://github.com/ruanyf/weekly/issues/3851))

2\. [Dự án OpenWrt công bố kế hoạch phát triển mẫu phần cứng router riêng](https://www.landiannews.com/archives/101760.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011108.webp)

Để kỷ niệm 20 năm ngày thành lập dự án hệ điều hành mã nguồn mở cho bộ định tuyến OpenWrt, nhóm phát triển đã công bố kế hoạch sản xuất mẫu phần cứng router do chính họ thiết kế với mức giá dưới 100 USD, đi kèm đặc tính bảo vệ firmware tối ưu giúp tránh sự cố hỏng bộ nhớ khi nạp ROM (brick).

3\. [Tìm hiểu bản chất của công nghệ nhúng văn bản (Embeddings) trong AI](https://simonwillison.net/2023/Oct/23/embeddings/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010708.webp)

Nền tảng của các mô hình ngôn ngữ lớn GPT dựa trên công nghệ embeddings - giải pháp chuyển đổi các đoạn văn bản tự nhiên thành các vectơ số học nhiều chiều, từ đó giúp máy tính dễ dàng tính toán độ tương đồng về mặt ngữ nghĩa giữa các văn bản.

4\. [Giới thiệu thuật toán ước tính số lượng phần tử duy nhất trong chuỗi dữ liệu](https://justinjaffray.com/a-charming-algorithm-for-count-distinct/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112508.webp)

Bài viết giới thiệu một giải pháp thuật toán thú vị giúp ước tính số lượng các phần tử không trùng lặp trong một tập dữ liệu lớn với yêu cầu tối ưu hóa bộ nhớ RAM sử dụng ở mức cố định tối thiểu.

5\. [Giải mã cơ chế hoạt động của tính năng thông báo đẩy trên trình duyệt Web Push](https://pqvst.com/2023/11/21/web-push-notifications/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112706.webp)

Tác giả tự xây dựng một mô hình demo đơn giản để giải thích chi tiết về cơ chế đăng ký và gửi thông báo đẩy (Web Push Notifications) cho các ứng dụng web dạng PWA.

6\. [Giải nghĩa các ký hiệu kỹ thuật trên thân tàu container](https://hakaimagazine.com/videos-visuals/the-secret-language-of-ships/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112402.webp)

Vỏ các tàu vận tải container cỡ lớn thường được sơn rất nhiều ký hiệu và thông số kỹ thuật đặc thù (hình trên). Bài viết giới thiệu ngắn gọn ý nghĩa của từng ký hiệu giúp bạn đọc yêu thích ngành hàng hải dễ dàng tìm hiểu.

## 工具

1\. [VisActor](https://visactor.io/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010604.webp)

Bộ giải pháp trực quan hóa dữ liệu frontend toàn diện do ByteDance phát triển, bao gồm thư viện biểu đồ [VChart](https://visactor.io/vchart) và thư viện bảng dữ liệu lớn [VTable](https://visactor.io/vtable). (Đóng góp của [@airgeek](https://github.com/ruanyf/weekly/issues/3849))

2\. [h5player for tampermonkey](https://github.com/xxxily/h5player)

Một tập lệnh Tampermonkey hữu ích bổ sung nhiều tính năng nâng cao cho các trình phát video HTML5 (điều chỉnh tốc độ phát nhiều mức, chụp màn hình video, chế độ picture-in-picture, hiệu chỉnh độ sáng, độ bão hòa, độ tương phản...), tương thích tốt với hầu hết các trang web chia sẻ video lớn hiện nay. (Đóng góp của [@xxxily](https://github.com/ruanyf/weekly/issues/3852))

3\. [Ảnh phục sửa chữa nhỏ trợ thủ (Inpaint WeChat)](https://github.com/shifu-group/inpaint_wechat)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010605.webp)

Dự án mã nguồn mở xây dựng ứng dụng WeChat Mini Program giúp xóa các vật thể hoặc người không mong muốn ra khỏi bức ảnh, toàn bộ thuật toán xử lý chạy trực tiếp trên thiết bị của người dùng mà không cần gửi dữ liệu về server. (Đóng góp của [@wangqmshf](https://github.com/ruanyf/weekly/issues/3853))

4\. [Pacman (Trò chơi ăn đậu cổ điển phiên bản web)](https://github.com/mumuy/pacman)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010902.webp)

Dự án mã nguồn mở tái hiện lại trò chơi ăn đậu kinh điển Pacman trên nền tảng web. Bạn có thể chơi thử bản [Demo tại đây](https://passer-by.com/pacman/). (Đóng góp của [@mumuy](https://github.com/ruanyf/weekly/issues/3855))

5\. [UShare](https://share.aitimi.cn/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010903.webp)

Công cụ web hỗ trợ tạo ảnh chia sẻ các đoạn code hoặc văn bản mẫu đẹp mắt, cho phép tùy chỉnh phông chữ và kích thước chữ hiển thị. (Đóng góp của [@szmxx](https://github.com/ruanyf/weekly/issues/3856))

6\. [mdcat](https://github.com/swsnr/mdcat)

Công cụ thay thế cho lệnh `cat` truyền thống trên terminal, hỗ trợ hiển thị nội dung tệp tin Markdown đã được định dạng và tô màu cú pháp trực quan trực tiếp trên màn hình console. (Đóng góp của [@lengyijun](https://github.com/ruanyf/weekly/issues/3859))

7\. [SuperCopy (Siêu cấp sao chép)](https://github.com/ruanyf/weekly/issues/3862)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010904.webp)

Tiện ích mở rộng trên trình duyệt giúp mở khóa các trang web chặn tính năng click chuột phải, cho phép người dùng bôi đen sao chép nội dung dễ dàng. (Đóng góp của [@WFANG12719](https://github.com/ruanyf/weekly/issues/3862))

8\. [Vue DevTools Next](https://github.com/vuejs/devtools-next)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010905.webp)

Thế hệ công cụ hỗ trợ gỡ lỗi và phát triển tiếp theo của Vue, mang lại trải nghiệm lập trình vượt trội cho các nhà phát triển Vue. (Đóng góp của [@webfansplz](https://github.com/ruanyf/weekly/issues/3864))

9\. [yft-design](https://yft.design/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010906.webp)

Ứng dụng hỗ trợ thiết kế danh thiếp (business cards) trực quan trên web được phát triển dựa trên thư viện fabric.js. (Đóng góp của [@more-strive](https://github.com/ruanyf/weekly/issues/3865))

10\. [ant-codeAI](https://github.com/sparrow-js/ant-codeAI/blob/main/README-zh_CN.md)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010907.webp)

Công cụ hỗ trợ tạo nhanh các đoạn mã nguồn web (React, Vue, Tailwind CSS) và ứng dụng di động (React Native) qua các API OpenAI, Gemini. (Đóng góp của [@sparrow-js](https://github.com/ruanyf/weekly/issues/3860))

11\. [paint-board](https://github.com/LHRUN/paint-board)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010908.webp)

Dự án bảng vẽ mã nguồn mở tích hợp nhiều loại cọ vẽ nghệ thuật độc đáo. Bạn đọc có thể xem bản [Demo tại đây](https://songlh.top/paint-board/). (Đóng góp của [@LHRUN](https://github.com/ruanyf/weekly/issues/3867))

12\. [Read Copilot](https://apps.apple.com/us/app/read-copilot-beyond-summarizer/id6449242676)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010909.webp)

Ứng dụng đọc tin tức trên iOS/macOS hỗ trợ kết nối RSS và lưu trữ đọc sau (Read It Later), tích hợp AI giúp tự động tạo tóm tắt, dàn ý chính và dịch thuật văn bản. (Đóng góp của [@dongsuo](https://github.com/ruanyf/weekly/issues/3868))

13\. [Hải báo D2C (Seal D2C)](https://music.163.com/st/seal/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010910.webp)

Tiện ích mở rộng trên Figma và MasterGo hỗ trợ xuất trực tiếp bản vẽ thiết kế thành mã nguồn React, Vue, React Native và WeChat Mini Program tương ứng. (Đóng góp của [@Kinasha](https://github.com/ruanyf/weekly/issues/3869))

14\. [vscode-common-intellisense](https://github.com/Simon-He95/vscode-common-intellisense)

Tiện ích mở rộng trên VS Code hỗ trợ tính năng tự động gợi ý mã nguồn (intellisense) cho các thư viện và framework frontend phổ biến hiện nay. (Đóng góp của [@Simon-He95](https://github.com/ruanyf/weekly/issues/3873))

15\. [Screenshot Beautifier (Shot Easy)](https://github.com/CH563/shot-easy-website)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011001.webp)

Dự án mã nguồn mở xây dựng trang web hỗ trợ làm đẹp ảnh chụp màn hình, xem bản dùng thử tại Demo. (Đóng góp của [@CH563](https://github.com/ruanyf/weekly/issues/3876))

16\. [Apache Answer](https://answer.apache.org/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011002.webp)

Nền tảng hỏi đáp mã nguồn mở được phát triển bằng Go và ReactJS, giúp doanh nghiệp nhanh chóng xây dựng hệ thống hỏi đáp nội bộ, diễn đàn hỗ trợ khách hàng hoặc kho lưu trữ tri thức. (Đóng góp của [@PrimmaAnna](https://github.com/ruanyf/weekly/issues/3877))

17\. [Yazi](https://github.com/sxyazi/yazi/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011101.webp)

Trình quản lý tệp tin đa nền tảng chạy ngay trên giao diện terminal, hỗ trợ xem trước file hình ảnh trực quan, được phát triển bằng ngôn ngữ Rust mang lại tốc độ phản hồi cực nhanh. (Đóng góp của [@lengyijun](https://github.com/ruanyf/weekly/issues/3879))

18\. [AI Thay mặt (Change Face)](https://www.changeface.online/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011102.webp)

Ứng dụng web hỗ trợ hoán đổi khuôn mặt của các nhân vật xuất hiện trong các bức ảnh hoặc đoạn video tải lên. (Đóng góp của [@CNHarrySun](https://github.com/ruanyf/weekly/issues/3882))

## 资源

1\. [linkhut](https://ln.ht/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011012.webp)

Dịch vụ lưu trữ và quản lý bookmark liên kết cá nhân tích hợp các tính năng mạng xã hội.

2\. [AI Search (Tìm kiếm thông minh)](https://aoyo.ai/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010603.webp)

Công cụ tìm kiếm thông minh: bên cạnh việc hiển thị danh sách các kết quả tìm kiếm thông thường, hệ thống sẽ tự động tổng hợp thông tin câu trả lời bằng ngôn ngữ tùy chọn của người dùng. (Đóng góp của [@aooyoo](https://github.com/ruanyf/weekly/issues/3848))

3\. [Tề Tư (MiraclePlus Wiki)](https://news.miracleplus.com/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010911.webp)

Trang tin tức công nghệ tổng hợp tiếng Trung hàng ngày, toàn bộ khâu cập nhật và biên tập nội dung được thực hiện tự động bằng hệ thống các tác nhân AI (AI agents). (Đóng góp của [@caoxuwen](https://github.com/ruanyf/weekly/issues/3861))

4\. [Email.ML](https://email.ml/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010912.webp)

Dịch vụ tạo địa chỉ email tạm thời tối giản hỗ trợ nhiều tên miền tùy chọn với thời gian hiệu lực trong vòng một giờ, được phát triển dựa trên Cloudflare Workers kết hợp Nuxt. (Đóng góp của [@ccbikai](https://github.com/ruanyf/weekly/issues/3870))

## 图片

1\. [Tài liệu hình ảnh cấu trúc linh kiện điện tử (Open Circuits)](https://pluralistic.net/2023/08/14/hidden-worlds/#making-the-invisible-visible-and-beautiful)

Năm ngoái, một cuốn sách có tên "Open Circuits: The Inner Beauty of Electronic Components" (Mở mạch: Vẻ đẹp tiềm ẩn của các linh kiện điện tử) đã được xuất bản tại Hoa Kỳ.

Cuốn sách giới thiệu chi tiết về các linh kiện điện tử cơ bản khác nhau, phần đặc biệt nhất là nó có nhiều hình minh họa tuyệt đẹp thể hiện các linh kiện điện tử bị cắt đôi ra. Hình bên dưới là mặt cắt dọc của một tụ điện.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081601.webp)

Bạn đọc có thể thử đoán xem hai bức ảnh dưới đây chụp cấu trúc cắt lớp của loại linh kiện điện tử nào hay không?

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081602.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081603.webp)

## ✍️ Bài đọc thêm

### Trải nghiệm thực tế về sự cần thiết của các thiết kế hỗ trợ người khuyết tật (Accessibility)

Vào tháng 6 năm nay, tôi cùng gia đình đi nghỉ mát tại một bãi biển.

Do một sự cố trượt chân bất cẩn, đầu gối của tôi đã bị chấn thương nghiêm trọng. Tôi lập tức nhận thức được mức độ nghiêm trọng của chấn thương.

Tôi nằm bất động trên bãi cát và hoàn toàn không thể tự đứng dậy nổi mặc cho các con sóng xô vào người. Sau khi uống phải vài ngụm nước biển mặn chát, tôi phải gồng mình dùng hai tay lết cơ thể dần khỏi mép nước để bò lên bờ.

Đến nay đã qua ba tháng điều trị chấn thương, tôi vẫn phải đi lại với dáng vẻ khập khiễng. Dù sức khỏe đang cải thiện dần nhưng tiến trình hồi phục diễn ra rất chậm chạp. Bác sĩ điều trị cho biết: "Có thể sẽ phải mất thêm vài tháng nữa."

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011003.webp)

Trong suốt khoảng thời gian khó khăn này, tôi nhận thấy bản thân phụ thuộc rất nhiều vào các thiết kế hỗ trợ người khuyết tật (Accessibility): từ hệ thống tay vịn cầu thang, các đường dốc lối vào cho đến thang máy công cộng...

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011004.webp)

Những thiết kế hỗ trợ này vốn là những chi tiết tôi hầu như không bao giờ để mắt tới trước đây, nhưng nay lại trở thành những yếu tố sống còn giúp tôi di chuyển hàng ngày.

Trải nghiệm thực tế khiến tôi liên tưởng đến một câu nói từng được nghe trước đây: "**Chúng ta thực chất đều chỉ là những người tạm thời lành lặn mà thôi**."

Bạn có biết rằng, tính trên quy mô toàn cầu hiện nay có tới 1/5 dân số đang phải chung sống với một dạng khuyết tật cơ thể nào đó. Ngay cả đối với những người hoàn toàn lành lặn, trong suốt chặng đường đời của mình, họ chắc chắn sẽ có lúc phải trải qua các giai đoạn chấn thương hạn chế vận động tạm thời hoặc vĩnh viễn do lão hóa.

Bản thân tôi vẫn cảm thấy mình rất may mắn. Đầu gối của tôi đang hồi phục tốt lên mỗi ngày, và đặc thù công việc văn phòng giúp tôi không phải di chuyển quá nhiều.

Tôi thực sự trân trọng những năng lực vận động bình thường mà mình đang sở hữu, đồng thời bày tỏ sự biết ơn đối với những người đã thiết kế nên các công trình hỗ trợ giúp người hạn chế vận động có thể tự lập sinh hoạt - những điều mà trước nay tôi vốn coi là hiển nhiên.

Việc chung tay hỗ trợ và nỗ lực xây dựng một không gian sống thân thiện với người khuyết tật thực chất chính là hành trình chuẩn bị để giúp đỡ chính bản thân chúng ta trong tương lai.

## Lịch sử tuần này

- 2023年（第 239 期）：[Lộ trình nghề nghiệp: Thảo luận về hai nhóm nhân sự có xu hướng gia tăng trong tương lai](http://www.ruanyifeng.com/blog/2023/01/weekly-issue-239.html)
- 2021年（第 189 期）：[Xu hướng thị trường: Dự báo về ngành công nghiệp tiếp theo sẽ rơi vào tình trạng cạnh tranh khốc liệt (nội quyển)](http://www.ruanyifeng.com/blog/2021/12/weekly-issue-189.html)
- 2020年（第 139 期）：[Khoa học công nghệ: Bàn luận về các bước tiến đáng kinh ngạc của ngành sinh học thời gian gần đây](http://www.ruanyifeng.com/blog/2020/12/weekly-issue-139.html)
- 2020年（第 89 期）：[Lời khuyên kinh doanh: Bài học về việc tuyệt đối không mang ô đi bán ở những vùng đất không có mưa](http://www.ruanyifeng.com/blog/2020/01/weekly-issue-89.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
