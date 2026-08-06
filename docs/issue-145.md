# 科技爱好者周刊（第 145 期）：大家不出门，经济怎么办？

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần. ( **[Thông báo] Tuần sau là kỳ nghỉ Tết Nguyên Đán, bản tin sẽ tạm nghỉ một số.** )

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1629) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020303.jpg)

Vào ngày 24 tháng 1 năm 2021, ba chú rùa biển bị sóng đánh dạt vào một bờ biển của Israel sau trận bão lớn. Hình ảnh ghi lại cảnh các bác sĩ thú y đang tiến hành quét CT cắt lớp cho một chú rùa biển bị chấn thương để xác định vết thương trong cơ thể. (Nguồn: [ECNS](http://www.ecns.cn/hd/2021-01-27/detail-ihafywhr7620341.shtml#3))

## 主带话题：Khi mọi người không ra khỏi cửa, nền kinh tế sẽ thế nào?

Gần đây, tôi có trò chuyện với một người bạn. Anh ấy đã chia sẻ một quan điểm khiến tôi rất ấn tượng.

Anh ấy cho rằng mọi người đang đánh giá thấp tác động sâu sắc của ngành dịch vụ giao hàng (gọi tắt là "ship"). Sự trỗi dậy của ngành giao đồ ăn, mua thuốc hộ và đi chợ hộ thực sự là một cột mốc có ý nghĩa lịch sử lớn.

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020301.jpg)

Lý do anh ấy đưa ra là: Trước đây, nền kinh tế Internet chỉ đóng vai trò hỗ trợ, bổ sung cho cuộc sống thường nhật. Ví dụ, mua sắm trực tuyến là để mua những món đồ mà cửa hàng gần nhà không có sẵn; chơi game online chỉ hoạt động khi có mạng. Chúng không thay thế các hoạt động cơ bản của đời sống truyền thống mà chỉ là phần bổ trợ.

**Nhưng dịch vụ giao hàng (ship) thì khác, nó trực tiếp thay thế một phần hoạt động sinh hoạt cơ bản của đời sống thường nhật.** Trong vòng bán kính 3km, bất cứ thứ gì bạn cần (từ đồ ăn, mua thuốc, mua rau củ...) đều có người giao đến tận cửa. Điểm mấu chốt ở đây là: Lẽ ra bạn phải tự mình di chuyển đến các địa điểm đó, nhưng nay bạn không cần phải ra khỏi cửa nữa.

Nói cách khác, sự xuất hiện của dịch vụ giao hàng đã thay đổi thói quen sinh hoạt cơ bản của con người. Nó biến những việc vốn bắt buộc phải ra khỏi nhà thành những việc có thể hoàn thành ngay tại chỗ. **Có thể nói, dịch vụ ship đã cắt giảm đáng kể nhu cầu ra khỏi cửa của người dân, tăng thời gian họ ở nhà hoặc văn phòng.**

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020302.jpg)

Nhờ có Internet, việc học tập, làm việc, mua sắm, giải trí và giao tiếp đều có thể thực hiện trực tuyến. Dịch vụ ship đã đẩy mạnh tác động này lên mức tối đa khi giải quyết luôn cả nhu cầu ăn uống và đi chợ hàng ngày. Sự phụ thuộc vào việc ra ngoài đang giảm dần, thậm chí việc tụ tập ăn uống đông người hiện tại cũng có thể chuyển sang hình thức trực tuyến.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021013004.jpg)

Tôi đặt ra một câu hỏi: **Nếu mọi người giảm một nửa tần suất ra khỏi nhà, nền kinh tế xã hội sẽ bị ảnh hưởng thế nào?**

Trước hết, nền kinh tế dịch vụ thực thể (các cửa hàng truyền thống) sẽ lụi tàn nhanh hơn do họ phụ thuộc hoàn toàn vào lưu lượng khách ghé thăm trực tiếp. Thứ hai, bất động sản thương mại sẽ rơi vào khủng hoảng khi không có người thuê mặt bằng, dẫn đến hàng loạt trung tâm thương mại đóng cửa. Cuối cùng, mối liên kết trực tiếp giữa người với người sẽ bị suy yếu, vì không ra ngoài đồng nghĩa với việc ít tiếp xúc trực tiếp, trong khi Internet rất khó xây dựng các mối quan hệ sâu sắc thực chất.

Trước đây, cơ hội kinh doanh của Internet chủ yếu nằm ở việc "làm sao để mọi người không cần ra ngoài vẫn hoàn thành được công việc". Tôi đoán rằng cơ hội kinh doanh trong tương lai có thể sẽ chuyển dịch ngược lại: "làm sao để thu hút mọi người ra ngoài và tăng cường kết nối trực tiếp giữa người với người".

## Khóa học phân tích mã nguồn Vue 3.0

Phiên bản chính thức của Vue 3.0 đã ra mắt được hơn 4 tháng kể từ ngày 18 tháng 9 năm ngoái. Quá trình học tập công nghệ mới của bạn đến đâu rồi?

Mặc dù hệ sinh thái xung quanh Vue 3.0 hiện tại chưa thể phong phú như bản Vue 2 cũ, nhưng hầu hết các dự án mới khởi chạy tại các doanh nghiệp hiện nay đã chuyển dịch sang bản này. Đồng thời, các câu hỏi phỏng vấn tuyển dụng Front-end hiện tại cũng tập trung xoay quanh các tính năng và nguyên lý của Vue 3.

Để giúp các nhà phát triển làm chủ các tính năng và đi sâu vào bản chất của công nghệ mới, tuần này chúng tôi chia sẻ khóa học **《Vue 3.0: From Practice to Source Code Analysis》**:

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020406.jpg)

Giảng viên của khóa học là thầy Dương Đào - một nhà phát triển đóng góp mã nguồn (code contributor) trực tiếp cho dự án Vue 3.0. Khóa học kéo dài trong 3 ngày sẽ không đi vào phân tích lý thuyết khô khan mà hướng dẫn học viên tự tay viết lại các module lõi của Vue 3.0 để hiểu rõ cơ chế phản ứng (reactivity) bên dưới.

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020407.jpg)

Chương trình học diễn ra vào các buổi tối ngày 5, 6 và 7 tháng 2 lúc 8 giờ tối. Khóa học được hỗ trợ mức phí ưu đãi dành riêng cho độc giả bản tin chỉ còn **0.99 NDT** (giá gốc 388 tệ) cho 200 học viên đăng ký sớm qua mã QR:

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020408.jpg)

## 科技动态

1、[Bắt giữ các nghi phạm dùng thiết bị camera dò cá trái phép](https://sichuan.scol.com.cn/sczh/202101/58037620.html)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012809.jpg)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012810.jpg)

Lực lượng công an thành phố Xạ Hồng, Tứ Xuyên đã bắt giữ hai nghi phạm có hành vi sử dụng thiết bị câu cá bằng móc chùm kết hợp camera truyền hình ảnh dưới nước (可视锚鱼 - Visual Anchoring Fish).

Thiết bị câu cá thế hệ mới này gồm một camera chống nước thả sâu dưới lòng sông để truyền hình ảnh trực tiếp lên màn hình LCD cầm tay của người câu. Khi phát hiện thấy các loại cá lớn bơi ngang qua cụm móc câu, người câu sẽ giật mạnh cần để các móc chùm lớn (thường to gấp hàng chục lần lưỡi câu thông thường) cắm rách thân cá để kéo lên bờ. Cảnh sát xác định đây là hình thức đánh bắt hủy diệt do móc câu cào rách nghiêm trọng thân cá khiến cá chết ngay cả khi được thả lại môi trường nước.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012812.jpg)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012811.jpg)

2、[Giải mã hiện tượng sét xanh (Blue Jet) kỳ bí ở tầng bình lưu](https://www.sciencenews.org/article/space-station-detectors-found-source-weird-blue-jet-lightning)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012202.jpg)

Năm 2019, các phi hành gia trên Trạm Vũ trụ Quốc gia ISS đã ghi nhận được những luồng sét màu xanh lam kỳ lạ phát ra từ các đám mây dông phóng ngược lên tầng bình lưu của Trái Đất. Bài viết công bố trên tạp chí *Nature* mới đây đã giải mã chi tiết cơ chế vật lý của hiện tượng này.

Thông thường, sét xuất hiện sát mặt đất có màu trắng do dòng điện tích ion hóa hỗn hợp nhiều chất khí khác nhau trong khí quyển. Nhưng ở tầng cao bình lưu, luồng điện tích từ các đám mây dông tương tác ion hóa trực tiếp với khí Nitơ (vốn chiếm tỷ lệ tuyệt đối tại đây) tạo ra bức xạ ánh sáng màu xanh lam đặc trưng.

3、[Mô hình giày thể thao tích hợp card đồ họa RTX 3080 của NZXT](https://www.rockpapershotgun.com/2021/01/21/my-sole-weeps-for-these-rtx-3080-shoes/)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012205.jpg)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012206.jpg)

Hãng sản xuất thiết bị tản nhiệt và vỏ máy tính NZXT phối hợp với thương hiệu thời trang Artifact Studios giới thiệu mô hình đôi giày thể thao tích hợp nguyên một dàn máy tính PC mini bên trong. Đôi giày trang bị cụm tản nhiệt nước, bo mạch chủ, quạt thông gió có đèn LED RGB và phần gót giày mô phỏng hình dáng chiếc card đồ họa cao cấp RTX 3080. Mặc dù là sản phẩm quảng bá thương hiệu độc đáo nhưng thiết kế cồng kềnh khiến đôi giày không thể sử dụng để đi lại thông thường.

4、[Nhà xuất bản ra mắt phiên bản in 14 màu của cuốn tiểu thuyết của William Faulkner](https://latimesblogs.latimes.com/jacketcopy/2012/07/the-sound-and-the-fury-as-william-faulkner-imagined-in-color.html)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012210.jpg)

Tác phẩm kinh điển *Âm thanh và cuồng nộ* (The Sound and the Fury) của nhà văn đoạt giải Nobel William Faulkner xuất bản năm 1929 nổi tiếng là một trong những cuốn sách khó đọc nhất lịch sử văn học Mỹ. Sách được viết theo lối độc thoại dòng tâm thức kéo dài liên tục, các mốc thời gian và góc nhìn nhân vật nhảy cóc đột ngột mà không có bất kỳ dấu câu nào ngăn cách để biểu thị tâm trí hỗn loạn của nhân vật.

Sinh thời, Faulkner từng mong muốn in cuốn sách bằng nhiều màu mực khác nhau để giúp người đọc dễ phân định các mốc thời gian nhảy cóc nhưng kỹ thuật in ấn thời đó chưa đáp ứng được. Mới đây, một nhà xuất bản đã hiện thực hóa ý tưởng này bằng cách xuất bản phiên bản in giới hạn 1.480 cuốn sử dụng 14 màu mực khác nhau đại diện cho các mốc thời gian nhảy cóc với mức giá 345 USD/cuốn.

5、[Thương mại hóa chất màu xanh lam YInMn Blue sau hơn 200 năm](https://www.smithsonianmag.com/smart-news/first-blue-pigment-discovered-200-years-finally-sale-180976769/)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012507.jpg)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021013001.jpg)

Do các khoáng chất màu xanh lam trong tự nhiên cực kỳ hiếm, các chất màu xanh dùng trong hội họa phần lớn đều phải tổng hợp hóa học. Năm 2009, các nhà khoa học tại Đại học Oregon đã tình cờ phát hiện ra hợp chất màu xanh mới gồm Yttrium, Indium và Mangan (được đặt tên là YInMn Blue).

Đây là phương thức tổng hợp màu xanh lam mới đầu tiên sau hơn 200 năm kể từ khi màu xanh Cobalt được phát minh vào năm 1807. YInMn Blue có khả năng phản xạ bước sóng hồng ngoại tốt giúp giữ bề mặt mát hơn và mang lại sắc xanh thuần khiết, tươi sáng bền bỉ. Sản phẩm hiện được bán thương mại với giá khá đắt: 179.4 USD cho tuýp màu nhỏ 37 gram.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012508.jpg)

6、**Tin tức một câu**

> - Nắng nóng kỷ lục mùa hè tại Sydney, Úc đẩy nhiệt độ đo được trên mặt đất đô thị lên sát mức 50 độ C, các nhà khí hậu học cảnh báo một số khu vực có thể trở nên không phù hợp để sinh sống vào mùa hè nếu không cải thiện quy hoạch cây xanh.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012501.jpg)

> - Nhà máy thủy điện tích năng Fengning tại Thừa Đức, Hà Bắc - dự án thủy điện tích năng lớn nhất thế giới - đã hoàn tất lắp đặt thiết bị và chuẩn bị hòa lưới phát điện vào cuối năm nay. Dự án hoạt động bằng cách dùng điện thừa ban đêm để bơm nước lên hồ đỉnh núi và xả nước phát điện vào ban ngày.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021013104.jpg)

> - Tỷ phú Elon Musk tuyên bố tự tin SpaceX sẽ thực hiện sứ mệnh đưa con người đầu tiên hạ cánh xuống Sao Hỏa vào năm 2026, hoặc sớm nhất là vào năm 2024 nếu gặp các điều kiện quỹ đạo thuận lợi.

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020209.jpg)

> - Khảo sát sức khỏe giấc ngủ ghi nhận Trung Quốc có tới hơn 300 triệu người gặp các chứng rối loạn giấc ngủ, trong đó hơn 3/4 người có thói quen thức khuya ngủ sau 11 giờ đêm và gần 1/3 thức qua 1 giờ sáng do thói quen lướt điện thoại tại nhà.

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020102.jpg)

> - Bộ Giáo dục ban hành quy chế nghiêm cấm học sinh bậc phổ thông mang điện thoại di động vào khuôn viên trường học khi chưa có đơn xin phép cam kết từ phụ huynh học sinh, các thiết bị mang theo phải được trường thu gom bảo quản tập trung.

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020105.jpg)

## 文章

1、[Bảng mã hiển thị phông chữ 16x16 pixel trên biển điện tử](https://mp.weixin.qq.com/s/iX8inI6kiS5TSqWbwFP7EQ)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012709.jpg)

Bài viết nghiên cứu kỹ thuật hiển thị chữ Hán trên các bảng điện tử LED ma trận kích thước 16x16 pixel gắn trên các xe buýt công cộng, so sánh độ dễ đọc của các font chữ nét thanh, nét đậm khác nhau.

2、[Phân tích cấu trúc thư mục mã nguồn của client Xunlei](https://zhuanlan.zhihu.com/p/337048581)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012702.jpg)

Tác giả thực hiện giải nén gói cài đặt và rà soát cấu trúc thư mục code JavaScript của ứng dụng tải file Xunlei bản desktop (vốn được xây dựng dựa trên Electron framework).

3、[Tìm hiểu nguyên lý chứng chỉ chữ ký số bảo mật của hệ điều hành iOS](http://chuquan.me/2020/03/22/ios-certificate-principle/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021013002.jpg)

Bài viết phân tích chi tiết cơ chế bảo mật xác thực chứng chỉ ký số của Apple đối với các ứng dụng iOS để chạy thử nghiệm (provisioning profile) và đưa lên App Store. ([@baochuquan](https://github.com/ruanyf/weekly/issues/1620) đóng góp)

4、[Kỷ niệm tham gia kỳ thi học sinh giỏi tin học NOIP của tác giả cách đây 20 năm](https://justyy.com/archives/45269)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021013003.jpg)

Tác giả chia sẻ lại những kỷ niệm đáng nhớ khi tham gia kỳ thi lập trình thuật toán NOIP bậc phổ thông vào năm 2001, dấu mốc định hình con đường sự nghiệp lập trình của anh về sau. ([@DoctorLai](https://github.com/ruanyf/weekly/issues/1624) đóng góp)

5、[Tìm hiểu cơ chế công nghệ sạc không dây xuyên không gian Mi Air Charge](https://zhidx.com/p/255150.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021013101.jpg)

Phân tích cấu trúc anten phát chùm sóng mmWave định hướng và cụm anten thu tín hiệu chuyển đổi năng lượng tích hợp trên điện thoại để thực hiện sạc không dây khoảng cách vài mét của Xiaomi.

6、[Tìm hiểu thuộc tính CSS `aspect-ratio` mới trên Chrome 88](https://web.dev/aspect-ratio/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021013103.jpg)

Chrome 88 chính thức hỗ trợ thuộc tính CSS `aspect-ratio` native giúp dễ dàng cố định tỷ lệ khung hình (width/height ratio) cho các phần tử chứa ảnh hoặc video mà không cần dùng các hack CSS cũ.

7、[30 bài học kinh nghiệm đúc rút sau nhiều năm làm phát triển phần mềm](https://chriskiehl.com/article/thoughts-after-6-years)（Tiếng Anh）

Những đúc kết thực tế của tác giả về cách viết code sạch, cách giao tiếp trong nhóm dev, việc lựa chọn công nghệ và tầm quan trọng của việc hiểu rõ yêu cầu nghiệp vụ của dự án.

8、[Hướng dẫn cài đặt biến Raspberry Pi 4 thành máy tính PC thay thế desktop](https://debugger.medium.com/my-impressions-on-using-a-raspberry-pi-4-as-a-desktop-replacement-ff677c885149)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012707.jpg)

Với sức mạnh phần cứng được nâng cấp, tác giả hướng dẫn các bước cài đặt hệ điều hành và so sánh hiệu năng sử dụng thực tế giữa Raspbian OS và Ubuntu khi dùng Pi 4 làm máy làm việc văn phòng hàng ngày.

9、[10 thói quen code TypeScript xấu cần loại bỏ trong năm nay](https://startup-cto.net/10-bad-typescript-habits-to-break-this-year/)（Tiếng Anh）

Tổng hợp 10 lỗi thiết kế code TypeScript không tối ưu (như lạm dụng kiểu dữ liệu `any`, bỏ qua kiểm tra giá trị null) và các giải pháp refactor code tương ứng. ([@naruco](https://github.com/ruanyf/weekly/issues/1631) đóng góp)

10、[Tại sao Go là ngôn ngữ lập trình yêu thích của tác giả](https://michael.stapelberg.ch/posts/2017-08-19-golang_favorite/)（Tiếng Anh）

Liệt kê các ưu điểm nổi bật của Go (Golang) dưới góc nhìn thực tiễn: tốc độ biên dịch cực nhanh, file thực thi độc lập nhỏ gọn, cơ chế concurrency mạnh mẽ và cú pháp tường minh.

## 工具

1、[Ebook Reader](https://www.loudreader.com/)

Trình đọc sách điện tử trực tuyến chạy trực tiếp trên trình duyệt, chỉ cần kéo thả các tệp định dạng azw3, epub, mobi hoặc pdf vào trang để đọc sách ngoại tuyến rất tiện lợi.

2、[Darkwire.io](https://github.com/darkwire/darkwire.io)

Ứng dụng phòng chat nhóm trực tuyến mã nguồn mở chạy trên nền Web, hỗ trợ mã hóa đầu cuối (end-to-end encryption) bảo vệ dữ liệu hội thoại. ([@Dup4](https://github.com/ruanyf/weekly/issues/1619) đóng góp)

3、[Xonsh](https://github.com/xonsh/xonsh)

Một shell dòng lệnh Linux viết bằng Python, cho phép lập trình viên viết lồng ghép cú pháp Python và lệnh Bash ngay trên giao diện terminal. ([@morefreeze](https://github.com/ruanyf/weekly/issues/1621) đóng góp)

4、[Filmulator](https://filmulator.org/)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021013106.jpg)

Phần mềm mã nguồn mở chuyên dụng hỗ trợ chỉnh sửa và xử lý ảnh chụp định dạng thô (Raw) của máy ảnh.

5、[Valetudo](https://github.com/Hypfer/Valetudo)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021013107.jpg)

Bản firmware mã nguồn mở thay thế cho các robot hút bụi Xiaomi và Roborock, cho phép người dùng tự vận hành quản lý robot qua giao diện Web cục bộ không cần thông qua cloud của hãng.

6、[Semgrep](https://github.com/returntocorp/semgrep)

Công cụ phân tích mã nguồn tĩnh (SAST) đa ngôn ngữ tốc độ cao, hỗ trợ lập trình viên tự cấu hình các rule quét bảo mật và lỗi logic code ngay trong CI/CD.

7、[Text to Handwriting](https://saurabhdaware.github.io/text-to-handwriting/)

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020103.jpg)

Công cụ trực tuyến giúp chuyển đổi văn bản đánh máy thành các trang viết tay sinh động, cho phép tải lên phông chữ viết tay cá nhân và tùy biến trang giấy nền.

8、[subaligner](https://github.com/baxtree/subaligner)

Công cụ dòng lệnh sử dụng mô hình học máy để tự động phân tích âm thanh video và căn chỉnh đồng bộ thời gian (sync timeline) cho tệp tin phụ đề.

9、[CSS Stripes Generator](https://stripesgenerator.com/stripe-samples)

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020317.jpg)

Công cụ trực tuyến hỗ trợ thiết kế các dải họa tiết sọc kẻ trang trí bằng CSS thuần và kết xuất code tự động.

10、[Archivy](https://github.com/archivy/archivy/)

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020318.jpg)

Ứng dụng mã nguồn mở hỗ trợ cá nhân tự xây dựng và quản lý bách khoa toàn thư wiki lưu trữ ghi chú cá nhân ngoại tuyến.

## Tài nguyên

1、[MuscleWiki](https://musclewiki.com/)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012110.jpg)

Bản đồ tương tác cơ thể người bằng tiếng Anh: Người dùng chỉ cần click chọn nhóm cơ mong muốn trên sơ đồ, trang web sẽ hiển thị các bài tập thể hình hướng dẫn chi tiết cho nhóm cơ đó.

2、[Rijksstudio của Bảo tàng Quốc gia Hà Lan](https://www.rijksmuseum.nl/en/rijksstudio)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012207.jpg)

Bảo tàng mở cổng số hóa chia sẻ hình ảnh độ phân giải cao của hơn 710.000 tác phẩm nghệ thuật名画 quý giá của các họa sĩ Hà Lan cổ điển cho phép tải về sử dụng tự do.

3、[Practice Python](http://www.practicepython.org/)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012209.jpg)

Trang web tổng hợp hàng chục bài tập lập trình Python từ mức cơ bản nhất có chia mức độ khó kèm lời giải chi tiết cho người tự học.

4、[Classpert](https://classpert.com/)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012807.jpg)

Trình tìm kiếm khóa học trực tuyến tổng hợp thông tin của hơn 240.000 khóa học đa lĩnh vực từ các nền tảng giáo dục lớn.

5、[Trang sưu tập hình ảnh ảo giác thị giác của Giáo sư Akiyoshi](http://www.ritsumei.ac.jp/~akitaoka/index-e.html)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021011516.jpg)

Trang chủ của giáo sư thuộc Đại học Ritsumeikan lưu trữ kho tranh vẽ ảo giác thị giác chuyển động độc đáo khi cuộn trang hoặc đảo mắt.

## 图片

1、[Cầu vượt dành riêng cho cua đỏ di cư tại đảo Giáng Sinh](https://www.theguardian.com/environment/2021/jan/23/how-wildlife-crossings-are-helping-reindeer-bears-and-even-crabs-aoe)

Hàng năm vào mùa mưa, hàng triệu chú cua đỏ từ các cánh rừng trên đảo Giáng Sinh di cư đồng loạt ra biển để sinh sản.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012502.jpg)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012503.jpg)

Để tránh tình trạng cua bị xe cán chết khi bò qua đường lộ, chính quyền địa phương đã thiết kế các cây cầu vượt và rào chắn dẫn hướng dành riêng cho cua đỏ di chuyển an toàn.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012504.jpg)

2、[Quả cầu nước và khí quyển của Trái Đất](https://ourplnt.com/water-air-earth/)

Hình ảnh mô phỏng lượng nước (quả cầu xanh lớn đường kính 1.400 km) và toàn bộ bầu khí quyển (quả cầu xanh nhạt nhỏ hơn) của Trái Đất nếu được thu gom nén lại đặt bên cạnh quả địa cầu đường kính 12.742 km để thấy sự hữu hạn của nguồn sống.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012708.jpg)

3、[Tỷ lệ phân bổ thời gian trong vòng đời phát triển phần mềm](https://blog.feenk.com/developers-spend-most-of-their-time-figuri-7aj1ocjhe765vvlln8qqbuhto/)

Biểu đồ in trong cuốn sách kinh điển *Software Engineering Principles* xuất bản năm 1979 mô tả tỷ lệ thời gian của lập trình viên dành cho một dự án phần mềm quy mô lớn:

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012808.jpg)

- Phân tích yêu cầu: 3%
- Phân tích hệ thống: 3%
- Thiết kế hệ thống: 5%
- Viết code (coding): 7%
- Kiểm thử module: 8%
- Kiểm thử tích hợp: 7%
- **Bảo trì hệ thống (maintenance): 67%**

## Bài đọc thêm

### Lịch sử ra đời của dịch vụ điện toán đám mây AWS

*Chia sẻ của một cựu kỹ sư làm việc tại Amazon vào năm 2000:*

Khi bong bóng internet dot-com đổ vỡ vào năm 2000, Amazon rơi vào tình thế vô cùng hiểm nghèo. Dòng vốn đầu tư cạn kiệt trong khi chi phí vận hành hạ tầng hàng năm lên tới 1 tỷ USD. Chi phí lớn nhất nằm ở các cụm máy chủ Sun Microsystems đắt đỏ vốn là tiêu chuẩn vàng của ngành thời bấy giờ.

Ban lãnh đạo Amazon đưa ra quyết định mạo hiểm: Dừng toàn bộ việc phát triển và bàn giao các tính năng bán hàng mới trong suốt hơn 1 năm trời để tập trung toàn lực cấu hình và viết lại toàn bộ mã nguồn hệ thống chuyển đổi từ máy chủ Sun sang chạy trên cụm máy chủ sử dụng hệ điều hành Linux giá rẻ.

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020305.jpg)

Quyết định chuyển đổi thành công ngoài mong đợi giúp chi phí hạ tầng giảm tới hơn 80% ngay lập tức. Hệ thống mới giúp Amazon tự chủ mở rộng quy mô dễ dàng.

Sau đó, Jeff Bezos nhận thấy một vấn đề: Là một đơn vị bán lẻ, lưu lượng truy cập của Amazon có tính mùa vụ cực kỳ cao, lượng máy chủ chuẩn bị cho mùa mua sắm tháng 11-12 sẽ bị bỏ trống thừa thãi trong suốt 46 tuần còn lại của năm. Ông bắt đầu suy nghĩ về việc đóng gói và cho các doanh nghiệp khác thuê lượng tài nguyên máy chủ thừa thãi này. Đồng thời, kiến trúc hệ thống cũng được thiết kế lại theo dạng tách biệt lỏng (decoupling) để các nhóm dev làm việc độc lập.

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020304.jpg)

Đó chính là bối cảnh ra đời của Amazon Web Services (AWS) thay đổi hoàn toàn bộ mặt của ngành công nghệ. AWS ra đời giúp giảm chi phí khởi nghiệp của các công ty công nghệ đi hàng chục lần, mở ra làn sóng bùng nổ startup toàn cầu. Nếu không có cuộc khủng hoảng tài chính năm 2000 ép buộc Amazon phải thay đổi kiến trúc hạ tầng để sinh tồn, có lẽ AWS đã không bao giờ xuất hiện. Hãy biết tận dụng các cơ hội từ khủng hoảng mang lại!

## 言论

1、

Trong trò chơi mô phỏng cuộc sống nông trại *Stardew Valley*, sau một thời gian chơi tôi luôn ước có tính năng thuê một nhân vật ảo khác đi vắt sữa bò và dê hộ mình mỗi sáng để tôi có thời gian đi làm việc khác. Tôi chọn game này vì muốn trải nghiệm cuộc sống yên bình thoát khỏi áp lực công sở, nhưng cuối cùng tư duy của tôi vẫn muốn thuê người khác làm thuê cho mình để tối ưu hóa thời gian - tựa game này thực sự làm tôi dao động giữa tư duy ủng hộ hay phản đối chủ nghĩa tư bản.

-- Trích bài viết về thiết kế game Stardew Valley

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021012509.jpg)

2、

Vấn đề của các cơ sở dữ liệu NoSQL là mô hình dữ liệu ban đầu trông rất đơn giản nhưng theo thời gian và sự phát triển của dự án, mô hình của bạn bắt buộc phải phình to và trở nên phức tạp đến mức không thể quản lý nổi. Sau 10 năm trải nghiệm thực tế, tôi nhận thấy việc lựa chọn hệ quản trị cơ sở dữ liệu quan hệ RDBMS truyền thống là quyết định đúng đắn trong hầu hết mọi trường hợp.

-- Thảo luận trên Hacker News

3、

Mỗi khi bạn cảm thấy đau đầu hay mệt mỏi khi viết lách, thực chất đó là quá trình bộ não đang phải cật lực hoạt động để sắp xếp, hệ thống hóa lại các luồng tư duy hỗn loạn trong đầu cho mạch lạc.

-- David Perell

## Nhìn lại

Tuần này năm 2020 (số 94): [Người lập trình giỏi cần trang bị cả kỹ năng tạo sản phẩm và kỹ năng bán hàng](http://www.ruanyifeng.com/blog/2020/02/weekly-issue-94.html)

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019113001.jpg)

Tuần này năm 2019 (số 42): [Làm sao để tìm ra lĩnh vực mà bạn có thể làm xuất sắc nhất?](http://www.ruanyifeng.com/blog/2019/02/weekly-issue-42.html)

![](https://cdn.beekka.com/blogimg/asset/201901/bg2019020101.jpg)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
