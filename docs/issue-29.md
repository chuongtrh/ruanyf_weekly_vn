# 每周分享第 29 期 (Bản tin chia sẻ hàng tuần số 29)

Ghi lại những điều thú vị đáng chia sẻ tôi bắt gặp trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Chào mừng mọi người gửi bài đóng góp thông qua mục [issue](https://github.com/ruanyf/weekly/issues) tại kho lưu trữ GitHub [ruanyf/weekly](https://github.com/ruanyf/weekly).

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110201.jpg)

Năm 1968, nhà khoa học máy tính Melvin E. Conway đã công bố một bài [báo cáo nghiên cứu](http://www.melconway.com/Home/Committees_Paper.html) nổi tiếng, sau này được giới công nghệ đúc kết thành **Conway's Law** (Định luật Conway).

> "Kiến trúc hệ thống phần mềm phản chiếu chính cấu trúc tổ chức của doanh nghiệp thiết kế ra nó."

Định luật này chỉ ra rằng cơ cấu phòng ban hành chính của một doanh nghiệp sẽ được thể hiện một cách trung thực trên cấu trúc sản phẩm phần mềm của họ. Ví dụ, nếu một hãng chia làm bốn nhóm kỹ sư độc lập để cùng viết một bộ trình biên dịch, thì cấu trúc bên trong của bộ trình biên dịch đó chắc chắn sẽ được phân tách thành bốn phân hệ tương ứng. Rất nhiều nghiên cứu thực tế sau đó đã chứng minh tính đúng đắn của định luật này.

Tại sao lại có hiện tượng này? Nguyên nhân là ở các tập đoàn lớn, vị thế của một nhà quản lý phần lớn được quyết định bởi quy mô nhân sự và ngân sách của phòng ban mà họ kiểm soát. Đội ngũ càng đông, ngân sách càng lớn thì tầm ảnh hưởng của người quản lý trong doanh nghiệp càng cao. Đó là lý do các sếp luôn tìm cách tuyển dụng thêm nhân sự và xin thêm ngân sách. Khi đội ngũ phình to, người quản lý bắt buộc phải vẽ ra thêm nhiều đầu việc để đảm bảo mọi nhân viên đều có việc làm. Do đó, khi cả đội ngũ cùng phát triển một dự án, cấu trúc phần mềm bắt buộc phải được thiết kế phức tạp lên để phân chia công việc cho toàn bộ nhân sự tham gia.

Theo định luật Conway, các dự án lớn của các tập đoàn lớn chắc chắn sẽ sở hữu những cấu trúc vô cùng phức tạp, bất kể sự phức tạp đó có thực sự cần thiết hay không. Mặt khác, rất nhiều lập trình viên có tâm lý sùng bái sự phức tạp (worship complexity), coi các phần mềm có cấu trúc đồ sộ rắc rối mới thể hiện được trình độ cao của người viết. Điều này dẫn đến thực tế: các tập đoàn lớn do cấu trúc nhân sự cồng kềnh đã tạo ra những phần mềm phức tạp, và cộng đồng bên ngoài mặc định coi đó là tiêu chuẩn kỹ thuật bắt buộc phải noi theo cho các dự án nhỏ của mình. Đây là lối tư duy sai lầm: việc các tập đoàn lớn buộc phải sống chung với sự phức tạp không đồng nghĩa với việc dự án của bạn cũng cần đến sự phức tạp cồng kềnh đó.

## 新闻 (Tin tức)

1、[Mô phỏng vật lý giải mã triết lý phân nhánh cây xanh của Leonardo da Vinci](https://phys.org/news/2012-01-leonardo-da-vinci-tree.html)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110202.jpg)

Từ 500 năm trước, danh họa Leonardo da Vinci đã quan sát và phát hiện ra một quy luật tự nhiên: tổng diện tích mặt cắt của các cành cây ở một độ cao bất kỳ luôn bằng diện tích mặt cắt của thân cây chính phía dưới. Tuy nhiên ông không đưa ra được lời giải thích cơ học cho hiện tượng này.

Nghiên cứu mới của các nhà vật lý thuộc Đại học Aix-Marseille (Pháp) đã làm sáng tỏ hiện tượng: cấu trúc phân nhánh đặc biệt này là mô hình tối ưu nhất giúp cây xanh phân tán lực cản và chống chọi lại sức gió lớn mà không bị gãy đổ.

2、[Cảnh sát Mỹ được khuyến cáo hạn chế nhìn vào màn hình khóa iPhone X của nghi phạm](https://www.engadget.com/2018/10/13/police-told-to-avoid-looking-at-iphone-x/)

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018101902.jpg)

Dòng iPhone thế hệ mới của Apple sử dụng công nghệ mở khóa bằng nhận diện khuôn mặt FaceID. Nếu camera quét khuôn mặt không khớp quá 5 lần liên tiếp, thiết bị sẽ tự động khóa hoàn toàn và yêu cầu mật mã số (passcode) để kích hoạt lại.

Nhằm bảo toàn cơ hội mở khóa điện thoại thu thập chứng cứ, cảnh sát Mỹ đã đưa ra khuyến cáo đối với các điều tra viên: không được tự ý nhìn vào màn hình khóa iPhone X của nghi phạm trong quá trình bắt giữ để tránh kích hoạt tính năng tự động khóa bảo mật này.

3. **Robot Atlas của Boston Dynamics biểu diễn khả năng nhảy chạy vượt chướng ngại vật**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110204.jpg)

Boston Dynamics công bố video mới nhất trình diễn khả năng giữ thăng bằng xuất sắc của robot nhân hình Atlas khi thực hiện các động tác chạy bộ và nhảy bật qua các khúc gỗ lớn cản đường một cách vô cùng mượt mà. Robot cao 1.45 mét, nặng 74.8 kg được trang bị cảm biến LiDAR và camera lập thể để tự động dựng bản đồ địa hình di chuyển thời gian thực.

4. **Sự thật đằng sau vụ án nhà báo mất tích được hé lộ qua đồng hồ Apple Watch**

Vụ án nhà báo Jamal Khashoggi bị ám sát bí mật tại Lãnh sự quán Saudi Arabia ở Thổ Nhĩ Kỳ đã được điều tra làm rõ nhờ dữ liệu thu âm từ chiếc đồng hồ Apple Watch ông đeo trên tay. Trước khi bước vào lãnh sự quán, nhà báo đã bật tính năng ghi âm của đồng hồ kết nối đồng bộ trực tiếp lên tài khoản iCloud thông qua kết nối mạng di động. Toàn bộ âm thanh hiện trường vụ án đã được đồng bộ về điện thoại iPhone ông để lại cho vị hôn thê đứng chờ bên ngoài, trở thành bằng chứng quan trọng giúp cảnh sát Thổ Nhĩ Kỳ phá án.

5、[Google hạn chế nhắc đến thương hiệu Android trên các thiết bị mới](https://9to5google.com/2018/10/11/the-dirty-word-android-dead-made-by-google/)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110206.jpg)

Tại sự kiện ra mắt sản phẩm phần cứng mới, Google hầu như không hề đề cập đến tên gọi hệ điều hành Android mà tập trung quảng bá thương hiệu dòng điện thoại Pixel 3 và thiết bị chạy ChromeOS. Thậm chí hệ điều hành cho đồng hồ thông minh Android Wear cũng được đổi tên thành Wear OS.

Giới phân tích nhận định Google đang muốn giảm sự hiện diện thương hiệu Android đối với người dùng cuối do tên gọi này thường bị liên tưởng tới các dòng máy giá rẻ của các đối tác sản xuất, đồng thời tập trung định vị dòng sản phẩm Pixel ở phân khúc cao cấp để đối đầu trực tiếp với Apple.

6、[Hãng bia Carlsberg ra mắt giải pháp kết dính lon bia bằng keo sinh học thay thế màng nhựa](https://www.telegraph.co.uk/news/2018/09/07/carlsberg-glues-beer-cans-together-becoming-first-brewery-abandon/)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110207.jpg)

Để giảm thiểu lượng rác thải nhựa khổng lồ từ các màng bọc plastic kết nối các lốc lon bia thông thường, hãng bia Carlsberg đã áp dụng công nghệ bao bì mới mang tên Snap Pack: sử dụng các giọt keo sinh học có độ kết dính cao để dán trực tiếp các lon bia lại với nhau. Người dùng chỉ cần bẻ nhẹ là có thể tách lon bia ra sử dụng dễ dàng.

7、[Thử nghiệm máy bay hybrid chạy bằng động cơ điện chở khách Zunum Aero](https://www.bloomberg.com/hyperdrive)

Dự án máy bay chở khách hybrid Zunum Aero do Boeing tài trợ dự kiến sẽ bàn giao phiên bản thương mại đầu tiên vào năm 2022. Máy bay có sức chứa 12 hành khách, vận hành chủ yếu bằng động cơ điện đặt ở cánh để loại bỏ tiếng ồn động cơ phản lực truyền thống, và trang bị hệ thống động cơ xăng dự phòng hỗ trợ hành trình bay lên tới 1.100 km.

8. **Phát hiện hệ thống hang động cổ đại đục khoét bằng móng vuốt thú khổng lồ tại Brazil**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110209.jpg)

Các nhà khoa học phát hiện nhiều đường hầm hình tròn có kích thước khổng lồ sâu trong lòng đất Brazil với vách hang chằng chịt các vết cào sâu. Nghiên cứu địa chất khẳng định đây không phải là hang động tự nhiên hay do con người cổ đại đào bới, mà chính là các hang trú ẩn (paleoburrows) do loài lười đất khổng lồ (Megatherium) đã tuyệt chủng đào bằng móng vuốt sắc nhọn từ hàng chục ngàn năm trước.

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110210.jpg)

## 教程 (Hướng dẫn)

1、[Bài viết] [Phương pháp đọc hiểu và nghiên cứu các tài liệu tiêu chuẩn kỹ thuật RFC](https://web.archive.org/web/20180916071340/https://www.mnot.net/blog/2018/07/31/read_rfc) (Tiếng Anh)

Tài liệu RFC là chuẩn chung cho hầu hết các giao thức internet (như HTTP, TCP) nhưng thường rất dài và khô khan. Tác giả chia sẻ kinh nghiệm cách đọc quét lấy thông tin cốt lõi và tra cứu các cập nhật bổ sung hiệu quả.

2、[Bài viết] [Hướng dẫn xây dựng ứng dụng giả lập máy tính bỏ túi iPhone bằng Flutter](https://hackernoon.com/how-to-build-iphone-calculator-using-flutter-fe934ce78d7e) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110229.jpg)

Tài liệu thực hành cơ bản hướng dẫn cách thiết kế layout nút bấm tròn và xử lý phép tính số học cho ứng dụng iOS/Android bằng framework Flutter.

3、[Bài viết] [Giải mã hiện tượng cơ học vận chuyển nước lên ngọn các loài cây gỗ cao trăm mét](http://www.science4all.org/article/the-amazing-physics-of-water-in-trees/) (Tiếng Anh)

Dưới góc độ áp suất khí quyển, lực hút chân không thông thường chỉ có thể kéo cột nước lên độ cao tối đa 10 mét. Bài viết giải thích cơ chế thoát hơi nước ở lá cây kết hợp lực mao dẫn và sức căng liên kết của phân tử nước giúp cây Sequoia khổng lồ có thể vận chuyển nước lên ngọn cao hơn 100 mét một cách kỳ diệu.

4、[Bài viết] [Phương pháp mã hóa lưu trữ dữ liệu text ẩn bên trong hình ảnh Canvas PNG](https://www.igorkromin.net/index.php/2018/09/06/hijacking-html-canvas-and-png-images-to-store-arbitrary-text-data/) (Tiếng Anh)

Hướng dẫn giải pháp kỹ thuật sử dụng API Canvas của HTML5 để mã hóa các chuỗi dữ liệu text thành các giá trị màu sắc điểm ảnh RGBA của file ảnh PNG, giúp lưu trữ dữ liệu phía Client tránh bị quét bởi các công cụ kiểm tra cookie thông thường.

## 资源 (Tài nguyên)

1、[Thư viện] [Awesome Lite Websites — Tổng hợp các phiên bản website siêu nhẹ của các trang tin lớn](https://github.com/mdibaiee/awesome-lite-websites)

Kho lưu trữ tổng hợp đường dẫn truy cập phiên bản rút gọn (lite/minimalist version) của các trang web lớn giúp tiết kiệm tối đa dung lượng băng thông di động cho người dùng.

2、[Giáo trình] [Computer Networks: Principles, Protocols and Practice](http://cnp3book.info.ucl.ac.be/#)

Sách giáo khoa điện tử nguồn mở chất lượng cao giới thiệu chi tiết các nguyên lý mạng máy tính và cơ chế vận hành của các giao thức internet cốt lõi.

## 工具 (Công cụ)

1、[Colorblindly Chrome Extension — Trình giả lập hiển thị hình ảnh cho người mù màu](https://github.com/oftheheadland/Colorblindly)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110216.jpg)

Tiện ích mở rộng hỗ trợ lập trình viên kiểm tra độ tương phản thiết kế web bằng cách chuyển đổi toàn bộ màu sắc hiển thị trên trình duyệt sang các dạng mù màu khác nhau (mù màu đỏ, xanh lá, xanh dương).

2、[AdGuard Home](https://adguard.com/en/blog/introducing-adguard-home/)

Giải pháp phần mềm nguồn mở giúp tự thiết lập máy chủ DNS riêng cho gia đình (chạy trên Raspberry Pi), hỗ trợ tự động chặn toàn bộ tên miền quảng cáo và mã theo dõi từ tầng mạng cho mọi thiết bị kết nối.

## 文摘 (Văn trích)

1. **Xu thế chia sẻ hệ thống nhà bếp trung tâm (Cloud Kitchen) của ngành dịch vụ ăn uống**

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102611.jpg)

Mô hình nhà bếp đám mây (Cloud Kitchen) đang phát triển mạnh mẽ tại Mỹ: các thương hiệu nhà hàng không cần đầu tư thuê mặt bằng và trang bị bếp riêng mà cùng thuê chung một khu bếp công nghiệp trung tâm. Khách đặt món qua ứng dụng, món ăn được chế biến tại bếp chung và giao trực tiếp đến tay người dùng, giúp tối ưu hóa chi phí vận hành và mở ra thế hệ chuỗi nhà hàng không sở hữu nhà bếp tương tự Uber không sở hữu xe taxi.

2. **Tương lai giao thông đô thị và sự dịch chuyển từ việc sở hữu phương tiện sang dịch vụ**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110220.jpg)

Kịch bản phổ cập xe tự lái chạy điện sẽ làm thay đổi hoàn toàn thói quen sở hữu xe hơi cá nhân. Minh chứng lịch sử cho thấy tốc độ thay thế của phương tiện diễn ra rất nhanh: năm 1900 đại lộ số 5 New York ngập tràn xe ngựa kéo, nhưng chỉ 13 năm sau (1913) sau khi dòng xe Ford Model T giá rẻ ra mắt, xe ngựa đã hoàn toàn biến mất khỏi đường phố. Khi dịch vụ taxi tự hành chạy điện phổ biến với chi phí rẻ chỉ bằng 1/10 chi phí tự nuôi xe hơi, người dân sẽ từ bỏ sở hữu xe để chuyển sang thuê bao dịch vụ di chuyển.

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110221.jpg)

3. **Nghiên cứu ứng dụng công nghệ biến đổi gene tạo ra hạt bông vải có thể ăn được**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110222.jpg)

Hạt của cây bông vải chứa hàm lượng protein và chất béo rất cao nhưng con người không thể ăn được do chứa độc tố gossypol tự nhiên giúp cây chống sâu bệnh. Các nhà khoa học Mỹ đã ứng dụng công nghệ can thiệp gene để khóa gene sản sinh gossypol trong hạt bông nhưng vẫn giữ nguyên độc tố này ở thân lá để chống sâu hại. Phát hiện giúp biến hàng triệu tấn hạt bông phụ phẩm thu hoạch hàng năm thành nguồn dinh dưỡng protein an toàn cho con người và thức ăn chăn nuôi.

## 新奇 (Sự độc đáo)

1. **Bộ JS vẽ tranh kỹ thuật số dựa trên mô tả ngôn ngữ của Sol LeWitt**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110227.jpg)

Nghệ sĩ Sol LeWitt nổi tiếng với phong cách vẽ tranh ý niệm: ông không trực tiếp vẽ mà chỉ viết các mô tả chi tiết bằng chữ về hướng đi của các nét vẽ và màu sắc để người khác thực hiện. Một lập trình viên đã viết thư viện JS để tự động render các nét vẽ hình học nghệ thuật trực quan trên Canvas dựa trên các đoạn văn mô tả ý niệm gốc của Sol LeWitt.

## 本周金句 (Kim ngôn tuần này)

1、

> "Là một nhà tư bản thành công, tôi rất dị ứng khi nghe các đồng nghiệp tuyên bố rằng những người giàu có như chúng tôi đang tạo ra công ăn việc làm cho xã hội. Thực chất, thực thể duy nhất tạo ra việc làm chính là khách hàng tiêu dùng. Việc các tập đoàn liên tục chèn ép cắt giảm thu nhập của người lao động đang làm suy kiệt sức mua của chính những khách hàng tương lai của họ."
> 
> -- Nick Hanauer

2、

> "Năm 2017 tại quán Starbucks, một phụ nữ trung niên bước đến tặng tôi cuốn sách nhỏ 'Bitcoin: Con đường tự do tài chính nghỉ hưu sớm'. Tôi hỏi bà vài câu hỏi cơ bản về blockchain và bà hoàn toàn không biết gì. Khi một người lao động bình thường đang nhiệt tình giới thiệu cho bạn về một xu hướng công nghệ làm giàu mới, đó chính là thời điểm bong bóng tài chính đã đạt đỉnh điểm. Tôi đã quyết định bán sạch số Bitcoin mình sở hữu ngay trong ngày hôm đó."
> 
> -- Jeremie Harris

(Hết)
