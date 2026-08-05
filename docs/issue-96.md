# 科技爱好者周刊：第 96 期 (Bản tin chia sẻ công nghệ số 96)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

Mục tuyển dụng [《Ai đang tuyển dụng?》](https://github.com/ruanyf/weekly/issues/1106) cung cấp nhiều thông tin việc làm hữu ích, hoan nghênh ghé thăm hoặc đăng tải thông tin tuyển dụng/thực tập.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011804.jpg)

Ảnh bìa: Nạn dịch châu chấu bùng phát tại Đông Phi, hình ảnh một chiếc Boeing 737-700 của hãng hàng không Ethiopia va chạm với đàn châu chấu khổng lồ khi đang hạ cánh ngày 9/1/2020.

## 刊首语 (Lời tựa)

Sở Giáo dục Thượng Hải vừa ban hành thông báo chính thức: Toàn bộ học sinh tiểu học, trung học cơ sở và trung học phổ thông trên địa bàn thành phố sẽ bắt đầu học kỳ mới từ ngày 2/3 bằng hình thức học tập trực tuyến tại nhà thay vì đến trường học tập trung.

Các bài giảng được xây dựng theo hình thức [ghi hình tập trung](https://mp.weixin.qq.com/s/DegoMgMA6AEenxC9yY4y3Q) với sự tham gia biên soạn của hơn 1.000 giáo viên cốt cán xuất sắc cấp thành phố, phát sóng đồng bộ trên 12 kênh truyền hình chuyên biệt cho từng cấp lớp từ lớp 1 đến lớp 12.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020022613.jpg)

Nhìn vào những bức ảnh ghi lại hậu trường phòng ghi hình bài giảng, tôi nhận thấy phương pháp giảng dạy không có nhiều khác biệt so với các giờ học truyền thống trên lớp, bản chất vẫn chỉ là việc đặt máy quay ghi lại bài giảng đứng lớp thông thường. Liệu phương pháp này có mang lại hiệu quả tiếp thu tốt cho học sinh?

Thực tế, ngay cả khi học sinh ngồi nghe giảng trực tiếp tại lớp học còn khó duy trì sự tập trung cao độ, phương pháp xem ghi hình bài giảng tĩnh tại nhà chắc chắn sẽ còn mang lại hiệu quả kém hơn nữa.

Các video giáo dục trực tuyến muốn đạt hiệu quả cao bắt buộc phải tích hợp các yếu tố trực quan sinh động: lồng ghép các hoạt cảnh đồ họa hoạt hình, sơ đồ tư duy trực quan hoặc các đoạn video ngắn minh họa để thu hút sự chú ý của người xem. Việc giảng dạy chay dựa vào slide chữ khô khan ngay cả người lớn cũng khó lòng duy trì sự tập trung quá 15 phút, chứ chưa nói đến đối tượng học sinh nhỏ tuổi.

Tôi tin rằng học tập trực tuyến chắc chắn là xu hướng không thể đảo ngược của tương lai, giúp học sinh tiếp cận tri thức mọi lúc mọi nơi với chi phí tối ưu nhất. Tuy nhiên, điều kiện tiên quyết để mô hình này thành công là **chúng ta không thể bê nguyên xi video ghi hình lớp học truyền thống lên mạng, mà bắt buộc phải kết hợp nhuần nhuyễn tính giáo dục cùng tính giải trí tương tác trực quan.**

Hai hình mẫu tiêu biểu làm rất tốt triết lý này trên thế giới mà các nhà giáo dục nên tham khảo là kênh toán học trực quan [3Blue1Brown](https://www.3blue1brown.com/) và kênh khoa học thường thức [Kurzgesagt](https://www.youtube.com/user/Kurzgesagt/). Họ xây dựng các video hoạt họa vô cùng tinh xảo để giải thích các khái niệm khoa học phức tạp một cách cuốn hút nhất. Tham khảo thử một video của Kurzgesagt dưới đây để thấy phong cách thiết kế bài giảng lôi cuốn:

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=b06577jvtnj" allowFullScreen="true" width="100%" height="500px"></iframe>

## Khóa học chuyên đề phỏng vấn Frontend

Do ảnh hưởng của dịch bệnh Corona, mùa tuyển dụng Frontend cao điểm đầu năm bị ảnh hưởng nhẹ. Nhiều bạn lầm tưởng các doanh nghiệp đang tạm dừng tuyển dụng, nhưng thực tế phần lớn các công ty công nghệ lớn đã nhanh chóng chuyển dịch hoàn toàn sang quy trình phỏng vấn từ xa (remote interview).

Nếu bạn vẫn đang chờ đợi dịch bệnh kết thúc hoàn toàn mới bắt đầu chuẩn bị ôn luyện kiến thức, bạn sẽ đánh mất rất nhiều cơ hội việc làm tốt. Hãy tận dụng khoảng thời gian này để củng cố hệ thống kiến thức Frontend và làm chủ các case phỏng vấn kỹ thuật chuyên sâu.

Nền tảng Tencent Classroom ra mắt chương trình ôn luyện phỏng vấn Frontend chuyên sâu hướng tới mục tiêu vượt qua 3 vòng thử thách chính của các doanh nghiệp lớn:

> **Vòng 1: Làm chủ kiến thức nền tảng vững chắc**
> 
> Hệ thống lại các câu hỏi phỏng vấn thường gặp về lõi JavaScript và CSS; Phân tích sâu cơ chế hoạt động bên dưới của các giao thức truyền thông HTTP/HTTPS; Nắm vững nguyên lý biên dịch mã nguồn của trình duyệt để sẵn sàng vượt qua vòng phỏng vấn đầu tiên.
> 
> **Vòng 2: Phân tích sâu kiến trúc các Framework phổ biến**
> 
> Giải mã chi tiết mã nguồn Vue 2 và cách xử lý các tính năng cốt lõi; Tìm hiểu cơ chế liên kết dữ liệu hai chiều (data-binding) thế hệ mới trên Vue 3 bằng Proxy và siêu lập trình (metaprogramming); Làm chủ cơ chế hoạt động của React Hooks, Provider và các câu hỏi phỏng vấn React nâng cao.
> 
> **Vòng 3: Tối ưu hóa hiệu năng và quy trình đóng gói dự án**
> 
> Hướng dẫn thiết lập các chỉ số đo lường hiệu năng trang web thực tế và các giải pháp tối ưu; Tìm hiểu nguyên lý hoạt động của Babel trong việc phân tích cú pháp AST, phân tích từ vựng và cú pháp; Đi sâu phân tích cơ chế đóng gói tài nguyên hệ thống của Webpack để giải quyết triệt để các nút thắt hiệu năng.

Khóa học được dẫn dắt bởi thầy Trần - cựu kỹ sư kiến trúc Frontend tại Tencent với nhiều năm kinh nghiệm làm người chấm điểm phỏng vấn trực tiếp cho doanh nghiệp.

Khóa học chính thức khai giảng vào thứ Hai tới (2/3). Độc giả bản tin quét mã QR dưới đây để tham gia nhóm nhận ưu đãi học phí sớm **chỉ còn 1 Nhân dân tệ cho 100 học viên đầu tiên**:

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020022601.jpg)

## 资讯 (Tin tức)

1. **Bosch ra mắt kính thông minh AR hiển thị bằng công nghệ chiếu laser võng mạc**

Tập đoàn công nghệ Bosch (Đức) vừa giới thiệu sản phẩm kính thông minh thế hệ mới có khả năng hiển thị các giao diện phần mềm trực quan đè lên trường nhìn tự nhiên của mắt thông qua thấu kính hoàn toàn trong suốt.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020704.jpg)

Điểm độc đáo cốt lõi của công nghệ này là không sử dụng màn hình hiển thị LCD hay máy chiếu mini truyền thống. Thay vào đó, thiết bị tích hợp một cụm vi gương quét siêu nhỏ để dẫn hướng 3 luồng tia laser (Đỏ, Xanh lục, Xanh lam) công suất cực nhỏ chiếu trực tiếp qua lớp kính全息 phản xạ vào võng mạc của mắt người đeo để tự động vẽ nên hình ảnh sắc nét.

Phương pháp này giúp hình ảnh hiển thị rõ nét ngay cả ngoài nắng gắt và hoàn toàn không bị người xung quanh phát hiện thông tin trên kính. Tuy nhiên, mỗi cặp kính bắt buộc phải được hiệu chỉnh cơ học chính xác theo cấu trúc khuôn mặt của từng cá nhân để đảm bảo tia laser chiếu đúng tâm đồng tử.

2. **SpaceX ra mắt dịch vụ đăng ký phóng vệ tinh nhỏ trực tuyến giá từ 1 triệu USD**

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020703.jpg)

Tập đoàn hàng không vũ trụ SpaceX chính thức cung cấp dịch vụ đặt chỗ cất cánh phóng vệ tinh trực tuyến trực tiếp trên trang chủ của hãng. Gói cước cơ bản có mức phí từ 1 triệu USD dành cho các dòng vệ tinh có trọng lượng dưới 200 kg, mỗi kg tải trọng phát sinh sẽ tính thêm phí 5.000 USD.

Khách hàng chỉ cần nhập thông số quỹ đạo mong muốn và đặt cọc trước 5.000 USD để đăng ký chỗ. SpaceX sẽ tận dụng khoảng trống tải trọng dư thừa trên các chuyến bay phóng tên lửa Falcon 9 định kỳ của dự án Starlink để ghép tải đưa các vệ tinh của khách hàng lên quỹ đạo. Đây được xem là mức chi phí cất cánh rẻ nhất và quy trình đơn giản nhất từ trước tới nay cho các dự án vệ tinh nghiên cứu quy mô nhỏ.

3. **Rough Guides xuất bản sách hướng dẫn du lịch tham quan phong cảnh trong thế giới game Xbox**

Nhà xuất bản sách du lịch nổi tiếng thế giới Rough Guides vừa cho ra mắt cuốn sách độc đáo mang tên *Xbox Beauty Guide*, chuyên tổng hợp và giới thiệu các địa điểm phong cảnh tuyệt đẹp được xây dựng chân thực bên trong các tựa game nổi tiếng trên hệ máy Xbox.

Cuốn sách được bán thương mại với mức giá 20 bảng Anh. Với sự phát triển vượt bậc của đồ họa 3D hiện nay, thế giới ảo trong các trò chơi điện tử (như quần thể kim tự tháp Giza trong *Assassin's Creed: Odyssey*) được xây dựng vô cùng sống động và hùng vĩ, xứng đáng là điểm đến cho các du khách thích du lịch ảo khám phá thế giới ngay tại nhà qua màn hình máy game.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020702.jpg)

4. **Ứng dụng thuật toán AI phục dựng bộ phim lịch sử "Tàu hỏa vào ga" năm 1895 lên chuẩn 4K**

Bộ phim ngắn kéo dài 50 giây *L'Arrivée d'un train en gare de La Ciotat* (Tàu hỏa vào ga) do anh em nhà Lumière thực hiện năm 1895 được coi là tác phẩm điện ảnh đầu tiên trong lịch sử nhân loại, ghi lại hình ảnh đầu tàu hơi nước kéo đoàn tàu vào sân ga ven biển nước Pháp.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020501.jpg)

Mẫu phim gốc hiện bị nhòe mờ, xước và có độ phân giải rất thấp. Mới đây, một nhà phát triển đã ứng dụng các mô hình mạng nơ-ron chuyên sâu để tự động nâng cấp độ phân giải đoạn phim lên chuẩn 4K sắc nét kết hợp bù đắp khung hình lên 60fps. Phiên bản phục dựng hiển thị rõ nét từng chi tiết trang phục, biểu cảm khuôn mặt của hành khách và chuyển động của đầu tàu hơi nước sau hơn 120 năm.

5. **Tai nạn thương tâm của nhà phiêu lưu tự chế tên lửa hơi nước bay lên bầu trời**

Nhà phiêu lưu người Mỹ Mike Hughes (biệt danh Mad Mike) đã tử nạn ở tuổi 64 trong một vụ thử nghiệm phóng tên lửa tự chế chạy bằng hơi nước tại khu vực sa mạc bang California ngày 22/2/2020. Sự việc xảy ra trực tiếp trước sự chứng kiến của đoàn làm phim tài liệu thuộc kênh Science Channel.

Tên lửa của ông sử dụng áp suất hơi nước nóng công suất lớn để đẩy thiết bị bay lên không trung. Trong vụ tai nạn, hệ thống dù hãm cứu hộ gặp sự cố kỹ thuật không thể bung ra sau khi cất cánh khiến tên lửa rơi tự do thẳng xuống mặt đất từ độ cao lớn gây tử vong tại chỗ. Trước đó vào năm 2018, ông từng phóng thành công dòng tên lửa này lên độ cao hơn 500 mét.

## 文章 (Bài viết)

1、[Bài viết] [Tìm hiểu phương thức tối ưu hóa tắt ứng dụng Web Node.js an toàn (Graceful Shutdown)](https://yvonnickfrin.dev/shutdown-correctly-nodejs-apps) (Tiếng Anh)

Khi người dùng nhấn tổ hợp phím Ctrl + C để tắt một tiến trình Node.js đang chạy trên server, làm thế nào để lập trình viên bắt được tín hiệu ngắt (SIGINT/SIGTERM) nhằm đóng toàn bộ các cổng kết nối database đang mở và xử lý nốt các request dang dở trước khi cho phép tắt hoàn toàn hệ thống.

2、[Bài viết] [Ứng dụng thư viện lit-html để tối ưu hóa thiết kế giao diện Web Components](https://terodox.tech/handling-web-component-markup-with-lit-html/) (Tiếng Anh)

Bài viết phân tích các ưu điểm vượt trội của thư viện lit-html do Google phát triển: sử dụng các tính năng ES6 Template Literals để xây dựng các cấu trúc HTML động siêu nhẹ ngay trong JavaScript mà không cần thông qua lớp ảo Virtual DOM giúp đạt hiệu năng hiển thị tối ưu nhất.

## 软件 (Phần mềm)

1、[craft.js — Framework hỗ trợ lập trình viên xây dựng tính năng kéo thả giao diện (Drag-and-Drop) trong React](https://github.com/prevwong/craft.js)

Cung cấp bộ công cụ toàn diện giúp các lập trình viên dễ dàng tích hợp tính năng tự kéo thả thiết kế trang web (page builder) vào ứng dụng React của mình: quản lý trạng thái các component kéo thả, hỗ trợ undo/redo và xuất dữ liệu JSON cấu trúc trang.

2、[qier-player — Linh kiện Web Player chơi video H5 chất lượng cao dành riêng cho React](https://github.com/vortesnail/qier-player)

Mã nguồn mở thành phần giao diện trình phát video viết bằng React, hỗ trợ đầy đủ các tính năng hiện đại như điều chỉnh tốc độ phát, chế độ picture-in-picture, hiển thị thanh tiến trình đẹp mắt và hỗ trợ phím tắt tùy chỉnh.

## 资源 (Tài nguyên)

1、[Tài liệu] [Hướng dẫn chi tiết quy trình tự thiết kế và lắp ráp thiết bị lưu trữ dữ liệu NAS từ bo mạch Raspberry Pi](https://www.instructables.com/id/PiNAS-the-Raspberry-Pi-NAS/)

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020604.jpg)

Bài viết hướng dẫn từng bước từ việc lựa chọn bo mạch Raspberry Pi, kết nối ổ cứng HDD qua cổng SATA, cài đặt hệ điều hành OpenMediaVault cho đến việc tự thiết kế in 3D vỏ hộp bảo vệ để tạo nên một máy chủ NAS lưu trữ đám mây gia đình giá rẻ.

## 图片 (Hình ảnh)

1. **Wisdom - Chú chim dã sinh có tuổi thọ cao nhất lịch sử sinh học thế giới**

Vào năm 1956, nhà điểu học Chandler Robbins đã đeo vòng định danh số hiệu cho một cá thể chim hải âu lớn khoảng 5 tuổi tại quần đảo Midway và đặt tên cho nó là "Wisdom" (Trí tuệ).

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122904.jpg)

Hiện tại chú chim này vẫn hoàn toàn khỏe mạnh ở tuổi 69, xác lập kỷ lục là cá thể chim hoang dã có tuổi thọ cao nhất được ghi nhận trong lịch sử khoa học. Chú chim đã bay tổng quãng đường hơn 3 triệu km (tương đương 120 vòng quanh Trái Đất) và vẫn đều đặn quay lại đảo đẻ trứng nuôi con hàng năm.

## 文摘 (Văn trích)

1. **Khái niệm chặng đường phát triển AirPods từ phụ kiện iPhone thành một nền tảng phần cứng độc lập**

Dòng tai nghe không dây AirPods của Apple đang xác lập vị thế thống trị tuyệt đối trên thị trường. Chỉ sau 3 năm ra mắt, AirPods đã bứt phá từ một món phụ kiện đi kèm iPhone để trở thành một hệ sinh thái thiết bị đeo (wearable platform) độc lập mạnh mẽ.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122623.jpg)

Một chi tiết thú vị là cách Apple ra mắt AirPods Pro: không hề có một sự kiện sân khấu hoành tráng nào, hãng chỉ âm thầm đăng tải một thông cáo báo chí ngắn gọn lên trang chủ. Nhưng AirPods Pro đã nhanh chóng trở thành một trong những thiết bị phần cứng bán chạy nhất lịch sử Apple.

Trong năm tài chính 2019, Apple đã phân phối tới 35 triệu cặp tai nghe AirPods mang lại doanh thu hơn 6 tỷ USD (tăng trưởng gấp đôi). Tính lũy kế 3 năm, doanh số AirPods đạt 61 triệu thiết bị - con số vượt cả doanh số iPhone trong 3 năm đầu tiên ra mắt. AirPods đang mở ra một không gian sáng tạo mới cho các nhà phát triển ứng dụng bằng cách kết hợp sâu với cảm biến sinh học trên Apple Watch để tự động điều chỉnh nhịp điệu âm nhạc theo nhịp tim người nghe.

2. **Liệu nguồn tài nguyên khí Heli (Helium) trên Trái Đất có bị khai thác cạn kiệt?**

Heli là nguyên tố hóa học nhẹ thứ hai trong bảng tuần hoàn (chỉ sau hydro). Chính vì sở hữu trọng lượng siêu nhẹ, lực hấp dẫn của Trái Đất không đủ sức giữ khí Heli tự do trong khí quyển khiến chúng liên tục bị thất thoát ra ngoài không gian vũ trụ, tạo nên sự khan hiếm của nguyên tố này trên Trái Đất.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121708.jpg)

Nhờ đặc tính hóa học trơ hoàn toàn, khí Heli đóng vai trò không thể thay thế trong các ngành công nghiệp công nghệ cao: ứng dụng làm chất làm mát siêu lạnh cho hệ thống nam châm siêu dẫn của máy chụp cộng hưởng từ MRI y tế, sản xuất vi mạch silicon và hàn công nghệ cao. Hiện tại toàn bộ lượng khí Heli thương mại đều được trích xuất từ các mỏ khí tự nhiên ngầm sâu dưới lòng đất.

Với tốc độ tiêu thụ hiện nay của nhân loại kết hợp cùng việc chính phủ Mỹ tiến hành tư nhân hóa bán tháo kho dự trữ Heli quốc gia với mức giá quá rẻ, các chuyên gia cảnh báo nguồn tài nguyên khí Heli tự nhiên có khả năng sẽ hoàn toàn cạn kiệt trong vòng 30 năm tới, đẩy giá thành Heli lên mức cực đắt đỏ trong tương lai.

## 言论 (Danh ngôn)

1、

> "Nếu tôi cần gửi đi một tệp tin văn bản thuần túy có định dạng cơ bản, định dạng lựa chọn hàng đầu của tôi luôn là RTF (Rich Text Format). Định dạng này chứa các thẻ siêu dữ liệu cho phép thiết lập in nghiêng, in đậm linh hoạt mà không cho phép đính kèm các mã macro lập trình ẩn bên trong giống như tệp DOCX của Word, loại bỏ hoàn toàn nguy cơ lây nhiễm mã độc máy tính."
> 
> -- Chia sẻ của một thành viên thuộc cộng đồng số hóa sách cổ

(Hết)
