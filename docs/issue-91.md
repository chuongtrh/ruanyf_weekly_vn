# 科技爱好者周刊：第 91 期 (Bản tin chia sẻ công nghệ số 91)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

[Thông báo] **Thứ Sáu tuần tới (24/1) là đêm Giao thừa, bản tin xin phép tạm dừng phát hành một tuần. Kính chúc quý độc giả một năm mới vạn sự như ý.**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120910.jpg)

Ảnh bìa: Khoảnh khắc hy hữu nhiếp ảnh gia chụp lại được hình ảnh cá voi xanh thải chất thải ra biển làm nước biển đổi sang màu xanh lục nhạt. Ảnh từ [Daily Mail](https://www.dailymail.co.uk/news/article-7696669/Incredible-moment-whale-poos-ocean-turning-water-mysterious-bright-green.html) (Vương quốc Anh).

## 刊首语 (Lời tựa)

Gần đây, tôi vừa đọc xong cuốn sách [《701 ngày của tôi ở Ấn Độ》](https://book.douban.com/subject/30177716/), tác giả là một giảng viên tiếng Trung được Viện Khổng Tử phái cử sang giảng dạy tại Viện Công nghệ Ấn Độ (IIT).

Mã nguồn của tác phẩm vốn là một chuỗi bài viết chia sẻ thực tế nhận được lượng tương tác khổng lồ trên diễn đàn Tianya, sau đó được biên tập xuất bản thành sách. Nếu bạn muốn tìm hiểu các góc nhìn quan sát trực tiếp, chân thực nhất về đời sống xã hội Ấn Độ đương đại dưới lăng kính của một người Trung Quốc, tôi nồng nhiệt giới thiệu cuốn sách này.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011511.jpg)

Trong sách có thảo luận một câu hỏi thú vị: Môn thể thao phổ biến thứ hai thế giới là gì?

> Mọi người đều biết môn thể thao vua có lượng người hâm mộ lớn nhất hành tinh là bóng đá. Nhưng môn thể thao có quy mô thị trường lớn thứ hai thế giới là gì?
> 
> Có thể có nhiều câu trả lời khác nhau, nhưng câu trả lời chính xác là: Bóng chày (Cricket).
> 
> Trong khi bóng đá thu hút khoảng 3.3 đến 3.5 tỷ người hâm mộ toàn cầu, bóng chày cricket đứng ngay sau với lượng người hâm mộ đạt từ 2 đến 3 tỷ người, trong đó riêng đất nước Ấn Độ đã đóng góp không dưới 1 tỷ người hâm mộ cuồng nhiệt. Giải vô địch thế giới Cricket World Cup cũng là ngày hội thể thao lớn thứ ba hành tinh (chỉ đứng sau World Cup bóng đá và Thế vận hội Olympic).

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011512.jpg)

Để minh chứng cho quy mô thị trường khổng lồ này, tác giả đưa ra số liệu thực tế: Thu nhập bình quân năm của các cầu thủ thi đấu chính thức tại Giải ngoại hạng cricket Ấn Độ (IPL) vượt ngưỡng 2.5 triệu USD, và đội trưởng đội tuyển quốc gia Ấn Độ MS Dhoni sở hữu mức thu nhập hàng năm lên tới 31 triệu USD! Để so sánh, thu nhập năm 2016 của huyền thoại bóng rổ Kobe Bryant là 21 triệu USD và siêu sao bóng đá Lionel Messi là 25 triệu Euro.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011513.jpg)

Đây là những con số vô cùng kinh ngạc đối với một quốc gia có mức thu nhập bình quân đầu người còn rất thấp như Ấn Độ. GDP bình quân đầu người của Ấn Độ hiện chỉ bằng 1/4 so với Trung Quốc, và mức thu nhập hàng tháng của phần lớn người dân lao động phổ thông chỉ dao động từ 1.000 đến 2.000 Nhân dân tệ. Tuy nhiên, mức thu nhập của giới siêu giàu và các ngành công nghiệp ngôi sao tại Ấn Độ không hề thua kém bất kỳ quốc gia phát triển nào trên thế giới.

Đọc cuốn sách tôi mới biết giá nhà đất tại các thành phố lớn như Mumbai hay Delhi đắt đỏ ngang ngửa, thậm chí vượt cả Bắc Kinh. Một người dân lao động phổ thông nhận lương cơ bản tại Ấn Độ nếu muốn mua một căn hộ tại Mumbai sẽ phải tích lũy không ăn không tiêu liên tục trong vòng 300 năm.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011514.jpg)

Tại sao một quốc gia còn nhiều hộ nghèo lại có thể vận hành một ngành công nghiệp thể thao tỷ đô và thị trường bất động sản đắt đỏ đến vậy?

Theo tôi, mức giá siêu cao của các ngành này thực chất được thúc đẩy bởi bài toán cung cầu của quy mô dân số khổng lồ, không phụ thuộc nhiều vào mức thu nhập bình quân. Dân số Ấn Độ sắp sửa chạm mốc 1.4 tỷ người, chuẩn bị vượt qua Trung Quốc để trở thành quốc gia đông dân nhất thế giới. Chính sự cuồng nhiệt của hàng tỷ người hâm mộ cricket và nhu cầu nhà ở đô thị khổng lồ của tầng lớp trung lưu đã nâng đỡ các mức giá kỷ lục này.

Tốc độ tăng trưởng dân số của Trung Quốc hiện đã rơi vào trạng thái bão hòa, và thu nhập bình quân đầu người khó lòng duy trì tốc độ tăng trưởng phi mã như trước. Do đó, tôi cho rằng trong giai đoạn tiếp theo, thị trường Ấn Độ sẽ mở ra nhiều cơ hội tăng trưởng lớn cho các doanh nghiệp công nghệ hơn so với thị trường nội địa.

## Tài liệu học tập Frontend miễn phí từ đối tác

Kỳ nghỉ Tết Nguyên Đán sắp sửa bắt đầu, đây cũng là khoảng thời gian thích hợp để các bạn lập kế hoạch phát triển bản thân và chuẩn bị cho các đợt tuyển dụng sau Tết. Đối tác đào tạo **Zhizuobiao** gửi tặng độc giả bản tin các khóa học lập trình frontend hoàn toàn miễn phí:

Trong suốt thập kỷ qua, lập trình frontend luôn nằm trong danh sách các ngành nghề khát nhân lực với nhu cầu tuyển dụng vô cùng lớn. Hơn nữa, frontend sở hữu rào cản nhập môn thấp hơn so với backend, luôn là lựa chọn hàng đầu cho các bạn muốn chuyển ngành hoặc bắt đầu học lập trình từ con số 0. Đi kèm với đó là mức thu nhập rất hấp dẫn cho các kỹ sư có năng lực thực chiến.

Khóa học **《Lập trình viên Frontend Full-stack: 165 ngày làm chủ kỹ thuật Web cho người mới bắt đầu》** là chuỗi bài giảng chi tiết từ kiến thức cơ bản cho đến thực chiến 3 hệ sinh thái framework lớn (React, Vue, Angular), phù hợp cho học viên tự học nâng cao kỹ năng.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011601.jpg)

Bên cạnh mảng phát triển ứng dụng Web truyền thống, các bạn muốn đón đầu xu hướng lập trình ứng dụng di động dạng Mini-App có thể tham khảo hai khóa học: **《Nhập môn lập trình Mini-App》** và **《Cập nhật cú pháp lập trình Mini-App mới nhất》**.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011602.jpg)

Chương trình được phát triển bởi Zhizuobiao - đơn vị đào tạo uy tín đạt chứng nhận chất lượng của Tencent Classroom với đội ngũ giảng viên giàu kinh nghiệm hỗ trợ học viên định hướng nghề nghiệp.

Độc giả quan tâm có thể quét mã QR dưới đây để tham gia nhóm học tập frontend và nhận 200 bộ tài liệu học tập miễn phí:

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011603.jpg)

## 资讯 (Tin tức)

1. **Thanh Hoa ra mắt ban nhạc robot biểu diễn nhạc cụ cổ truyền Trung Hoa Moja**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122603.jpg)

Truyền thông đưa tin, Đại học Thanh Hoa (Bắc Kinh) vừa công bố dự án ban nhạc robot biểu diễn nhạc cụ truyền thống Trung Quốc đầu tiên trên thế giới mang tên "Moja" (Mặc Giáp). Ban nhạc gồm 3 thành viên robot độc đáo: robot "Kaiyang" chịu trách nhiệm chơi trống, robot "Yuheng" biểu diễn sáo trúc và robot "Yaoguang" gảy đàn Không Hầu (một loại đàn hạc cổ). Dự án là kết quả hợp tác nghiên cứu giữa Học viện Mỹ thuật và Phòng thí nghiệm Tương lai thuộc Đại học Thanh Hoa.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122604.jpg)

Mỗi robot được thiết kế cơ học chuyên biệt để thực hiện chính xác các kỹ thuật diễn tấu đặc thù của nhạc cụ: thổi hơi, gảy dây và gõ nhịp. Toàn bộ các bản nhạc biểu diễn đều được các nhạc sĩ sáng tác riêng cho ban nhạc để tối ưu hóa khả năng của robot. Các nhà thiết kế chia sẻ, robot sở hữu những ưu thế vượt trội so với con người khi biểu diễn: đối với sáo trúc, robot có thể kiểm soát và duy trì luồng hơi thổi ổn định với thời gian kéo dài hơn rất nhiều so với hơi thở của nghệ sĩ; đối với phần trống, robot được trang bị tới 4 cánh tay cơ học cho phép gõ đồng thời trên 4 trống có cao độ khác nhau một cách hoàn hảo.

2. **Dự án lưu trữ năng lượng xanh bằng phương pháp Mountain Gravity Energy Storage**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122608.jpg)

Thách thức lớn nhất đối với các nguồn năng lượng tái tạo như điện mặt trời và điện gió là tính chập chờn, không thể liên tục cung cấp điện lên lưới nên bắt buộc phải có các hệ thống lưu trữ năng lượng phụ trợ. Do giá thành các hệ pin Lithium quy mô lớn vẫn còn rất đắt đỏ, các nhà nghiên cứu Áo đề xuất giải pháp lưu trữ năng lượng bằng trọng lực vùng núi (MGES). Hệ thống hoạt động trên nguyên lý: tận dụng lượng điện dư thừa vào giờ thấp điểm để vận chuyển đất cát lên đỉnh núi cao; vào giờ cao điểm, đất cát sẽ được thả rơi tự do xuống dưới theo hệ thống ròng rọc để làm quay tuabin phát điện, tương tự cơ chế hoạt động của các nhà máy thủy điện tích năng.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122609.jpg)

Ưu điểm lớn nhất của giải pháp này là không yêu cầu quỹ đất và nguồn nước lớn như thủy điện, không cần xây dựng đập nước lớn gây ảnh hưởng sinh thái. Đất cát là vật liệu rẻ tiền, không bị bốc hơi theo thời gian nên có thể tuần hoàn sử dụng vô hạn. Nhược điểm nằm ở hiệu suất chuyển đổi năng lượng cơ học còn thấp và thất thoát ma sát lớn. Giải pháp đặc biệt phù hợp cho các đảo cô lập có địa hình đồi núi dốc như quần đảo Hawaii để lưu trữ điện năng theo mùa du lịch.

3. **Máy bay hành khách cỡ lớn C919 hoàn thành giai đoạn bay thử nghiệm mẫu thử cuối cùng**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122703.jpg)

Ngày 27/12/2019, mẫu thử thứ 6 của dòng máy bay hành khách thân rộng do Trung Quốc tự phát triển C919 đã hoàn thành chuyến bay thử nghiệm kéo dài 2 giờ 5 phút tại sân bay quốc tế Phố Đông (Thượng Hải), thực hiện thành công hơn 30 nội dung kiểm thử kỹ thuật an toàn. Đây là mẫu thử cuối cùng của dự án, đánh dấu việc hoàn thành toàn bộ giai đoạn phát triển mẫu thử nghiệm để bước sang giai đoạn bay kiểm thử cường độ cao phục vụ cấp chứng chỉ bay.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122704.jpg)

Hiện tại, cả 6 mẫu thử đang được phân bổ bay thử nghiệm tại các trung tâm thử nghiệm hàng không lớn trên cả nước. Song song đó, dây chuyền sản xuất các linh kiện thương mại đầu tiên cũng đã được khởi động nhằm hướng tới mục tiêu hoàn thành cấp chứng chỉ bay quốc gia và bàn giao những chiếc máy bay đầu tiên cho khách hàng vào năm 2021.

4. **Volkswagen ra mắt bộ nhận diện thương hiệu phẳng 2D tối giản**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122804.jpg)

Hãng xe Đức Volkswagen chính thức công bố thiết kế logo mới tối giản dưới dạng đồ họa phẳng 2D, lược bỏ các đường đổ bóng và chi tiết 3D giả kim loại trước đây để hướng tới sự thanh mảnh, tương phản cao. Thiết kế mới cho phép ứng dụng linh hoạt trên các giao diện kỹ thuật số và phát sáng trên các dòng xe điện tương lai. Trong lịch sử phát triển, hãng đã có 11 lần thay đổi thiết kế logo.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122803.jpg)

Cùng xu hướng tối giản hóa, hãng xe Audi cũng đã đăng ký bảo quyền cho hai thiết kế logo 4 vòng tròn lồng nhau dạng phẳng 2D đơn giản hơn, được dự báo sẽ ứng dụng riêng cho các dòng xe điện thế hệ mới của hãng.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122805.jpg)

5. **Giải mã bí ẩn về các chấm vàng li ti định danh của các dòng máy in màu**

Vào năm 2017, một tài liệu tuyệt mật của chính phủ Mỹ bị rò rỉ ra ngoài và cơ quan điều tra FBI đã nhanh chóng xác định chính xác danh tính của người đã in và mang tài liệu đó ra khỏi văn phòng. Sau khi tài liệu được công bố, các chuyên gia bảo mật phát hiện trên bề mặt giấy in xuất hiện hàng loạt chấm màu vàng nhỏ li ti được sắp xếp theo quy luật toán học đặc biệt, mắt thường hầu như không thể phát hiện nhưng hiển thị rõ dưới ánh sáng xanh chuyên dụng (ảnh dưới).

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122906.jpg)

Phân tích quy luật sắp xếp các chấm vàng, chuyên gia xác định đây là một hệ thống mã hóa ghi lại chính xác ngày, giờ in tài liệu (6 giờ 20 phút ngày 9/5/2017) cùng số seri định danh của chính máy in đã thực hiện lệnh in (ảnh dưới). Sự việc xác nhận một bí mật công nghệ lâu năm: các nhà sản xuất máy in màu lớn đều âm thầm cài đặt thuật toán tự động in kèm mã định danh ẩn này lên mọi trang giấy in mà không công bố rộng rãi cho khách hàng.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122907.jpg)

6. **Trung Quốc công bố bộ ảnh bề mặt mặt trăng độ phân giải cao kỷ niệm một năm tàu Hằng Nga 4 đổ bộ**

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011509.jpg)

Kỷ niệm một năm ngày tàu thăm dò Hằng Nga 4 đổ bộ thành công lên vùng tối của mặt trăng vào ngày 3/1/2019, Cơ quan vũ trụ quốc gia Trung Quốc đã công bố rộng rãi bộ dữ liệu hình ảnh độ phân giải cao về bề mặt mặt trăng do tàu đổ bộ và xe tự hành Ngọc Thỏ 2 chụp lại. Bộ dữ liệu gồm hơn 17.000 tệp tin với dung lượng tổng cộng đạt 20.9 GB cho phép các nhà khoa học toàn cầu tải về nghiên cứu địa chất.

7. **Tin vắn**

- Mạng xã hội Facebook tài trợ cuộc thi phát triển các công cụ ứng dụng trí tuệ nhân tạo nhằm phát hiện và cảnh báo các video giả mạo sử dụng công nghệ Deepfake trước khi người dùng đăng tải lên hệ thống.

- Nhóm nghiên cứu sinh vật học chỉ ra loài quạ có khả năng tư duy logic và sử dụng công cụ thông minh vượt trội, được đánh giá là loài động vật thông minh nhất hành tinh ngoài nhóm động vật linh trưởng.

- Báo cáo xu hướng tìm kiếm nổi bật của Google tại Úc ghi nhận từ khóa "Bản đồ cháy rừng xung quanh tôi" (Fires near me) dẫn đầu lượng tìm kiếm trong suốt năm 2019 do thảm họa cháy rừng lịch sử đe dọa các khu dân cư.

- Tập đoàn Huawei chính thức nâng cấp mảng kinh doanh Cloud và AI thành nhóm ngành kinh doanh chiến lược lớn thứ 4 của tập đoàn (bên cạnh mảng viễn thông Carrier, mảng doanh nghiệp Enterprise và mảng tiêu dùng Consumer).

- Hãng điện thoại OnePlus thu hút sự chú ý tại triển lãm CES khi lắp ráp một chiếc đàn piano độc đáo sử dụng màn hình của 17 chiếc điện thoại OnePlus 7T làm phím bấm tương tác.

## 文章 (Bài viết)

1、[Bài viết] [Chia sẻ kinh nghiệm bán startup nhỏ với giá 22.000 USD của một lập trình viên mới tốt nghiệp](https://mohddanish.me/blog/micro-startup-acquired) (Tiếng Anh)

Một kỹ sư phần mềm trẻ người Ấn Độ chia sẻ về hành trình tìm kiếm ý tưởng sản phẩm ngách, tự tay lập trình phát triển và vận hành sản phẩm tối giản (MVP) để thu hút lượng người dùng trả phí ban đầu trước khi bán lại dự án cho nhà đầu tư để nhận khoản tiền 22.000 USD.

2、[Bài viết] [So sánh hiệu năng thực tế giữa vi xử lý Intel và AMD trên dòng Surface Laptop 3](https://www.anandtech.com/show/15213/the-microsoft-surface-laptop-3-showdown-amd-picasso-vs-intel-ice-lake) (Tiếng Anh)

Chuyên trang công nghệ thực hiện đánh giá hiệu năng chi tiết giữa hai phiên bản cấu hình của Surface Laptop 3 sử dụng vi xử lý Intel Ice Lake và AMD Picasso: kết quả ghi nhận Intel tối ưu thời lượng pin tốt hơn cho các tác vụ văn phòng thông thường, trong khi đồ họa tích hợp của AMD mang lại hiệu năng gaming mượt mà hơn.

3、[Bài viết] [Tổng hợp các nguyên tắc thiết kế RESTful API hiệu quả cho doanh nghiệp](https://www.vinaysahni.com/best-practices-for-a-pragmatic-restful-api) (Tiếng Anh)

Tác giả chia sẻ hơn 20 nguyên tắc thực chiến khi xây dựng API: từ việc thiết kế đường dẫn URL nhất quán, quản lý phiên bản API, xử lý lỗi phản hồi bằng HTTP status codes cho đến cơ chế bảo mật xác thực và giới hạn băng thông (rate limiting).

## 软件 (Phần mềm)

1、[repl.it — Nền tảng lập trình và chạy thử mã nguồn trực tiếp trên trình duyệt web](https://repl.it/site/blog/github)

Cung cấp công cụ khởi tạo môi trường chạy code tức thì cho hơn 50 ngôn ngữ lập trình phổ biến, nay tích hợp tính năng tự động tải và chạy trực tiếp mã nguồn từ bất kỳ kho lưu trữ GitHub nào ngay trên trình duyệt mà không cần cài đặt node_modules hay trình biên dịch cục bộ.

2、[Gitpod — Công cụ khởi tạo môi trường phát triển ứng dụng (IDE) đám mây dựa trên VSCode](https://www.gitpod.io/)

Tích hợp trực tiếp với các nền tảng lưu trữ mã nguồn GitHub, GitLab: chỉ cần thêm tiền tố `gitpod.io/#` trước URL kho lưu trữ để khởi tạo một không gian làm việc VSCode hoàn chỉnh chạy trên container đám mây của hãng để lập trình trực tuyến.

3、[Hidden Bar — Tiện ích tối giản hỗ trợ ẩn bớt các biểu tượng trên thanh Menu Bar của macOS](https://github.com/dwarvesf/hidden)

Công cụ mã nguồn mở viết bởi các kỹ sư Việt Nam giúp người dùng dễ dàng thu gọn màn hình macOS bằng cách ẩn bớt các biểu tượng ứng dụng chạy ngầm trên thanh menu bar, mang lại không gian làm việc sạch sẽ tối giản.

## 资源 (Tài nguyên)

1、[Tài liệu] [Giáo trình tự học cấu trúc dữ liệu và giải thuật bằng phiên bản JavaScript của cuốn SICP kinh điển](https://sicp.comp.nus.edu.sg/)

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121804.jpg)

Giáo trình khoa học máy tính kinh điển *SICP (Structure and Interpretation of Computer Programs)* được biên soạn lại mã nguồn ví dụ hoàn toàn bằng ngôn ngữ JavaScript bởi các giáo sư Đại học Quốc gia Singapore (NUS) giúp sinh viên dễ tiếp cận.

2、[Trang web] [Tổng hợp các sự kiện công nghệ và dự án phát triển thần tốc của thế giới](https://patrickcollison.com/fast)

Trang web cá nhân của CEO Stripe Patrick Collison tổng hợp các cột mốc thi công, nghiên cứu khoa học hoàn thành trong thời gian ngắn nhất của nhân loại: tiêu biểu là tốc độ gia tăng dân số của Thâm Quyến và tốc độ mở 1.000 cửa hàng của Luckin Coffee.

## 图片 (Hình ảnh)

1. **Futuro House - Kiến trúc nhà nghỉ di động hình đĩa bay độc đáo năm 1965**

Vào năm 1965, kiến trúc sư người Phần Lan Matti Suuronen đã thiết kế mẫu cabin nghỉ dưỡng trượt tuyết độc đáo với cấu trúc hình đĩa bay UFO, sử dụng chất liệu nhựa composite siêu nhẹ dễ dàng cẩu vận chuyển lắp đặt ở mọi địa hình hiểm trở và tối ưu hiệu suất sưởi ấm bên trong.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111202.jpg)

Mẫu nhà di động này cao 4 mét, rộng 8 mét với không gian phòng sinh hoạt lớn và nhà tắm khép kín, được bán ra thương mại với mức giá khoảng 12.000 USD thời bấy giờ. Có 96 căn hộ Futuro được chế tạo thương mại và hiện còn 67 căn được lưu giữ bảo tồn trên khắp thế giới.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111204.jpg)

2. **2D Cafe - Quán cà phê mang phong cách bản vẽ tranh vẽ độc đáo tại Tokyo**

Một quán cà phê tại Tokyo thiết kế không gian độc đáo bằng cách sử dụng tông màu trắng đen chủ đạo kết hợp các đường kẻ nét vẽ tay viền xung quanh toàn bộ đồ vật trang trí từ bàn ghế cho tới rèm cửa.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111206.jpg)

Hiệu ứng thị giác tương phản mạnh mẽ khiến du khách khi bước chân vào quán có cảm giác như đang bước vào một thế giới truyện tranh phẳng 2D đầy ảo ảnh.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111207.jpg)

## 文摘 (Văn trích)

1. **Lịch sử phát triển và cấu trúc hóa học của vật liệu xi măng xây dựng**

Các công trình kiến trúc sơ khai của nhân loại sử dụng bùn đất nện để làm tường và lợp mái tranh. Cấu trúc này có độ bền cơ học kém, không thể xây cao tầng và dễ bị nước mưa cuốn trôi khi mưa bão.

Đá tự nhiên là vật liệu lý tưởng hơn nhưng việc đục đẽo định hình lại vô cùng khó khăn và khó liên kết chặt chẽ. Từ xa xưa, nhân loại đã mơ ước về một loại đá lỏng có thể đổ vào khuôn để đông cứng theo hình dạng mong muốn hoặc một loại keo liên kết đá siêu cứng. Giải pháp cho ước mơ đó chính là xi măng - một trong những phát minh cổ xưa nhất của nhân loại.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111812.jpg)

Thành phần nguyên liệu cốt lõi của xi măng là đá vôi (chứa canxi cacbonat). Khi nung đá vôi lên nhiệt độ khoảng 1.000 độ C, khí CO2 thoát ra và thu được bột vôi sống (oxit canxi). Vôi sống có tính ăn mòn da rất mạnh, và sở hữu đặc tính phản ứng nhiệt lượng cực mạnh khi trộn cùng nước làm nước sôi lên, tạo thành vôi tôi (canxi hydroxit).

Khi đổ hỗn hợp vôi tôi tôi vào khuôn gỗ ngoài không khí, vôi tôi sẽ hấp thụ khí CO2 từ không khí để chuyển hóa ngược lại thành canxi cacbonat ban đầu. Bằng phản ứng hóa học đơn giản này, bột đá vôi ban đầu đã đông cứng trở lại thành khối đá bền vững. Để tăng khả năng chịu lực chống nứt, cát đá và sỏi được thêm vào để tạo thành bê tông đổ móng công trình.

Các thế hệ xi măng ban đầu đòi hỏi không khí để khô cứng nên không thể ứng dụng thi công móng cầu dưới nước sâu. Người La Mã cổ đại đã phát hiện ra việc pha trộn bột đá vôi cùng tro núi lửa sẽ tạo ra loại xi măng đặc biệt có khả năng tự đông cứng ngay trong môi trường nước biển, giúp họ xây dựng nên các công trình hải cảng kỳ vĩ vẫn tồn tại vững chãi cho tới ngày nay.

## 言论 (Danh ngôn)

1、

> "Nếu một công nghệ lập trình hay thiết bị gia dụng trở nên đủ phổ biến trên thị trường, chắc chắn sẽ có nhà phát triển nỗ lực tìm cách tích hợp công nghệ đó lên chiếc máy nướng bánh mì."
> 
> -- Nhận xét châm biếm về dự án máy nướng bánh mì thông minh Toasteroid hỗ trợ in thông tin dự báo thời tiết trực tiếp lên lát bánh mì nướng.

(Hết)
