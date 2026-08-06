# 科技爱好者周刊（第 139 期）：Bước tiến đáng kinh ngạc của công nghệ sinh học

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần. ( **Thông báo: Thứ Sáu tuần sau là kỳ nghỉ Tết Dương lịch, bản tin sẽ được phát hành sớm hơn vào thứ Năm ngày 31 tháng 12.** )

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1520) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122303.jpg)

Một khu cắm trại ngắm cực quang tại Phần Lan, du khách lưu trú trong các cabin kính hình vòm đặc biệt giữa tuyết trắng để chiêm ngưỡng vẻ đẹp kỳ ảo của cực quang về đêm. (Nguồn: [Instagram](https://www.instagram.com/p/CJENLJPK0A9/))

## 主带话题：Bước tiến đáng kinh ngạc của công nghệ sinh học

Tuần trước, tôi đọc được một bài viết về vắc-xin mRNA trên một trang web của Mỹ và thực sự cảm thấy vô cùng kinh ngạc.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122105.jpg)

Vắc-xin mRNA là một công nghệ hoàn toàn mới lần đầu tiên được đưa vào ứng dụng thực tế trên người. Mọi người thử đoán xem thời gian nghiên cứu và phát triển nó mất bao lâu?

Câu trả lời chắc chắn sẽ làm bạn ngỡ ngàng. **Vắc-xin mRNA chống dịch của tập đoàn Moderna bắt đầu được nghiên cứu vào ngày 11 tháng 1 năm 2020 và hoàn thành chỉ sau hai ngày vào ngày 13 tháng 1 năm 2020.**

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122301.jpg)

Mốc thời gian này không chỉ sớm hơn ngày phong tỏa Vũ Hán (23 tháng 1) mà còn trước cả ca nhiễm COVID-19 đầu tiên được ghi nhận tại Mỹ (20 tháng 1). Có nghĩa là Moderna đã phát triển thành công vắc-xin mà chưa cần nhìn thấy ca bệnh thực tế hay có mẫu virus sống trong tay - một điều chưa từng có tiền lệ.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122106.jpg)

Sự tình diễn ra như sau: Vào ngày 11 tháng 1 năm 2020, nhóm nghiên cứu của giáo sư Trương Vĩnh Chấn tại Đại học Phục Đán đã chia sẻ trình tự gene DNA của virus Corona lên mạng internet. Ngay chiều hôm đó, các nhà khoa học của Moderna đã tải về và tiến hành phân tích trình tự này trong phòng thí nghiệm để thiết lập cấu trúc vắc-xin và hoàn thành ngay trong hai ngày cuối tuần. Vì ngày 11 tháng 1 năm 2020 là thứ Bảy, nên nếu làm việc khẩn trương tăng ca thì họ hoàn toàn có thể làm xong chỉ trong vòng một ngày.

Lộ trình diễn ra tiếp theo như sau:
- **13 tháng 1**: Hoàn thành thiết kế vắc-xin.
- **7 tháng 2**: Hoàn thành lô sản xuất thử nghiệm lâm sàng đầu tiên.
- **4 tháng 3**: FDA phê duyệt thử nghiệm lâm sàng giai đoạn 1.
- **16 tháng 3**: Tiêm thử nghiệm trên tình nguyện viên đầu tiên.
- **23 tháng 3**: Moderna bắt đầu mở rộng quy mô sản xuất.
- **27 tháng 4**: FDA phê duyệt thử nghiệm lâm sàng giai đoạn 2.
- **27 tháng 7**: Bắt đầu thử nghiệm lâm sàng giai đoạn 3.
- **16 tháng 11**: Kết quả thử nghiệm giai đoạn 3 công bố vắc-xin đạt hiệu quả phòng ngừa 94.5%.
- **11 tháng 12**: FDA cấp phép sử dụng khẩn cấp.

Các bạn có thể thấy, cả một năm sau đó chủ yếu tiêu tốn cho việc thử nghiệm lâm sàng diện rộng và xin cấp phép hành chính. Bản chất cấu trúc của vắc-xin không hề thay đổi so với thành quả nghiên cứu trong hai ngày đầu tiên.

Tại sao vắc-xin công nghệ mRNA có thể phát triển nhanh đến vậy mà không cần mẫu virus sống?

Theo thông tin từ CDC Mỹ, vắc-xin mRNA hoạt động như một công cụ gửi "thông báo" hướng dẫn tế bào miễn dịch tự tạo ra gai protein nhận diện đặc trưng của virus. Do đó, chỉ cần giải mã được trình tự gene để xác định các đặc trưng này là các nhà khoa học có thể nhanh chóng thiết kế ra vắc-xin, quy trình tương tự như việc giải một bài toán.

Ý nghĩa của cột mốc này là nếu vắc-xin mRNA chứng minh hiệu quả cao trong thực tế, các đợt phát triển vắc-xin tương lai sẽ diễn ra cực kỳ nhanh chóng. Quy trình thử nghiệm và cấp phép sau này cũng có thể được tối giản vì cơ chế nền tảng là tương đương nhau. Công nghệ sinh học hiện đại đã phát triển vượt bậc ngoài sức tưởng tượng của chúng ta, đưa việc phân tích và thiết lập gene trở thành công việc cơ bản.

## Khóa học phát triển Web Component

Component hóa là xu hướng phát triển web hiện đại được mọi lập trình viên công nhận. Tuy nhiên từ trước đến nay, trình duyệt chưa hề hỗ trợ khai báo component nguyên bản, dẫn đến sự trỗi dậy của các thư viện và framework bên thứ ba như React và Vue.

Công nghệ Web Component do Google (chủ yếu là đội ngũ Chrome) đề xuất nhằm giải quyết bài toán này, giúp trình duyệt tự render component native:

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122404.jpg)

Điểm ưu việt nhất của Web Component là tính mỏng nhẹ, dung lượng code tối giản và hoàn toàn không cần tải thêm bất kỳ thư viện JS ngoài nào để chạy component. Nền tảng chia sẻ video Youtube hiện nay cũng được xây dựng dựa trên công nghệ này.

Tuần này, chúng tôi chia sẻ khóa học video **《Web Component Componentized Development》** kéo dài 90 phút do Kaikeba sản xuất dành cho các lập trình viên muốn đón đầu công nghệ mới.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122405.jpg)

Nội dung chính của khóa học:
- Triết lý cốt lõi của phát triển theo hướng Component.
- Cấu trúc kỹ thuật cấu thành Web Component:
  1. Custom Elements (Tùy biến phần tử HTML).
  2. Thẻ HTML `<template>`.
  3. Mở rộng các component sẵn có của trình duyệt.
- Hướng dẫn thực hành viết mã nguồn hoàn chỉnh cho một component.

Khóa học đi kèm mã nguồn mẫu để học viên thực hành tải về. Bộ tài liệu trị giá 399 tệ hiện dành tặng **200 suất học miễn phí (0 tệ)** cho độc giả bản tin:

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122403.jpg)

## Tin tức

1、[Lắp đặt đồng hồ nước thông minh hỗ trợ người già neo đơn](https://finance.sina.com.cn/tech/2020-12-13/doc-iiznctke6317394.shtml)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121408.jpg)

Chính quyền phường Giang Tô thuộc quận Trường Ninh, Thượng Hải đã triển khai lắp đặt hệ thống đồng hồ nước thông minh cho các hộ gia đình người già neo đơn sống một mình.

Nếu trong vòng 12 tiếng liên tục lượng nước sinh hoạt tiêu thụ của căn hộ dưới mức 0.01 m3, hệ thống sẽ tự động gửi cảnh báo về ban quản lý tổ dân phố để cử nhân viên y tế đến kiểm tra sức khỏe của cụ già kịp thời. Đồng thời, hệ thống cảm biến cửa thông minh cũng được lắp đặt để phát cảnh báo nếu cửa ra vào không mở trong suốt 24 giờ.

2、[Dịch vụ du lịch VR 360 độ trực tiếp](https://www.vpark.io/travel)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120916.jpg)

Một startup tại San Francisco vừa ra mắt dịch vụ du lịch trải nghiệm qua kính VR thực tế ảo. Hướng dẫn viên du lịch sẽ cầm camera 360 độ đi tham quan trực tiếp các địa danh nổi tiếng của San Francisco và livestream trực tiếp qua Youtube 360 theo khung giờ đăng ký.

Khách hàng ngồi tại nhà đeo kính VR sẽ nhận được hình ảnh 360 độ thời gian thực sinh động, nghe thuyết minh và có thể đàm thoại trực tiếp với hướng dẫn viên tại hiện trường. Chi phí cho mỗi giờ trải nghiệm dao động từ 39 đến 59 USD.

3、[Cáp quang lõi rỗng (Hollow-core fiber) tăng tốc độ mạng của các quỹ đầu tư tài chính](https://www.wsj.com/articles/high-frequency-traders-push-closer-to-light-speed-with-cutting-edge-cables-11608028200)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121602.jpg)

Các công ty giao dịch tần suất cao (High-Frequency Trading) tại phố Wall đang tiến hành lắp đặt cáp quang lõi rỗng để giúp truyền các lệnh giao dịch tài chính nhanh hơn đối thủ. Khác với cáp quang thủy tinh đặc truyền thống, cáp quang thế hệ mới thiết kế phần ruột rỗng chứa không khí siêu nhỏ.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121603.jpg)

Do tốc độ truyền ánh sáng trong không khí nhanh hơn khoảng 50% so với trong môi trường thủy tinh đặc, cáp quang lõi rỗng giúp rút ngắn độ trễ truyền dữ liệu đi vài trăm nanosecond (1 phần tỷ giây). Trước đây các quỹ đầu tư từng chi hàng trăm triệu USD chỉ để đào đường cáp quang chạy thẳng tắp hoặc chuyển sang dùng sóng viba vĩ ba để giảm trễ vài mili giây.

4、[Em bé sinh ra từ phôi đông lạnh lâu nhất lịch sử](https://www.bbc.com/news/world-us-canada-55164607)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120407.jpg)

Tháng 10 năm 2020, bé gái Molly Gibson đã chào đời khỏe mạnh tại Mỹ từ một phôi thai được hiến tặng đông lạnh từ tháng 10 năm 1992 (tức là phôi đã được đông lạnh suốt 27 năm). Về mặt sinh học, cô bé có cùng độ tuổi với người mẹ mang thai hộ của mình.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120408.jpg)

Hiện tại trung tâm NEDC của Mỹ đang lưu trữ khoảng 1 triệu phôi thai đông lạnh do các cặp vợ chồng hiến tặng nhằm hỗ trợ các gia đình mắc chứng vô sinh nhận nuôi phôi. Công nghệ đông lạnh phôi xuất hiện lần đầu vào năm 1984 tại Úc và có thời hạn bảo quản gần như vô hạn.

5、[Chủ tịch Toyota cảnh báo việc ép buộc chuyển dịch hoàn toàn sang xe điện](http://www.nbd.com.cn/articles/2020-12-23/1579335.html)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122307.jpg)

Chủ tịch tập đoàn Toyota Akio Toyoda nhận định làn sóng truyền thông và chính sách ép buộc loại bỏ hoàn toàn xe xăng sang xe điện là quá cường điệu và phi thực tế.

Ông phân tích tại Nhật Bản, phần lớn sản lượng điện năng quốc gia vẫn đến từ nhiệt điện than và khí đốt, do đó xe điện chỉ giúp chuyển dịch ô nhiễm từ ống xả xe sang các nhà máy điện. Hơn nữa, việc sạc xe điện đồng loạt vào giờ cao điểm mùa hè sẽ gây quá tải nghiêm trọng cho lưới điện quốc gia và chi phí nâng cấp trạm sạc là một con số khổng lồ. Một trụ sạc nhanh Supercharger của Tesla có công suất lên tới 250 kW (tương đương lượng điện tiêu thụ của hàng chục máy điều hòa công suất lớn).

6、**Tin tức một câu**

> - Thư mời họp báo ra mắt điện thoại Xiaomi 11 gây sốt khi đính kèm một con chip Snapdragon 888 thật (mẫu chip flagship cao cấp nhất của Qualcomm trị giá khoảng 200 USD) làm quà lưu niệm.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122406.jpg)

> - Các trình duyệt lớn Safari, Chrome, Edge và Firefox đồng loạt phát hành bản vá chặn hoàn toàn một chứng chỉ gốc do chính phủ Kazakhstan bắt buộc người dân cài đặt lên máy tính để giám sát dữ liệu mạng internet.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121801.jpg)

> - Cơ quan quản lý Pháp tuyên phạt Google 100 triệu euro và Amazon 35 triệu euro vì hành vi tự động ghi cookie quảng cáo lên trình duyệt khi chưa có sự đồng ý của người dùng.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121101.jpg)

> - NASA công bố danh sách 18 phi hành gia chuẩn bị cho chương trình Artemis đổ bộ Mặt Trăng tương lai, cam kết sẽ đưa nữ phi hành gia đầu tiên đặt chân lên Mặt Trăng.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121406.jpg)

> - Quốc hội Mỹ phê duyệt gói cứu trợ Covid-19 trị giá 900 tỷ USD, bao gồm khoản ngân sách 7 tỷ USD trợ cấp chi phí sử dụng internet băng thông rộng cho các hộ gia đình thu nhập thấp (mức 50 USD/tháng).

## Bài viết

1、[Mẹo sáng tạo giá đỡ điện thoại, hộp bút từ gạch xếp hình Lego](https://www.coolapk.com/feed/23451115?shareKey=ZDY5ODdkNGVmOTg2NWZkNTU2MzI~)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121303.jpg)

Hướng dẫn chi tiết kèm hình ảnh cách tận dụng các viên gạch Lego cũ lắp ráp thành các vật dụng văn phòng tiện ích, sáng tạo phục vụ bàn làm việc.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121304.jpg)

2、[Nature công bố 10 phát kiến khoa học nổi bật nhất năm 2020](https://mp.weixin.qq.com/s/CVzJjOq87FTYjwRSno04yQ)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121705.jpg)

Tổng hợp 10 nghiên cứu khoa học xuất sắc nhất trong năm của tạp chí Nature, bao gồm cơ chế căng thẳng gây bạc tóc nhanh chóng ở động vật, lần đầu thu nhận chớp vô tuyến nhanh (FRB) trong dải Ngân Hà...

3、[Báo cáo khảo sát các công cụ thiết kế UI/UX năm 2020](https://uxtools.co/survey-2020/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121706.jpg)

Kết quả khảo sát từ hàng nghìn nhà thiết kế giao diện toàn cầu chỉ ra Figma tiếp tục dẫn đầu thị phần phần mềm thiết kế UI, xếp sau lần lượt là Sketch, Adobe XD, Illustrator và Photoshop.

4、[Cách xác định địa chỉ IP thật của máy chủ ẩn sau lớp bảo vệ CDN Cloudflare](https://soatok.blog/2020/05/09/how-to-de-anonymize-scam-knock-off-sites-hiding-behind-cloudflare/)（Tiếng Anh）

Phân tích các lỗ hổng cấu hình DNS và cách gửi yêu cầu HTTP để tìm ra IP thực tế của máy chủ gốc (Origin Server) khi website cấu hình chưa chuẩn sau CDN.

5、[Các quy tắc thiết lập thuộc tính noopener, noreferrer và nofollow cho thẻ link](https://blog.bhanuteja.dev/noopener-noreferrer-and-nofollow-when-to-use-them-how-can-these-prevent-phishing-attacks)（Tiếng Anh）

Giải thích chi tiết các nguy cơ bảo mật tấn công giả mạo (phishing) qua thuộc tính `window.opener` và cách sử dụng thuộc tính `rel` của thẻ `<a>` để bảo vệ an toàn cho website của bạn.

6、[Sự bóp nghẹt của các dịch vụ Cloud lớn đối với mô hình kinh doanh mã nguồn mở](https://joemorrison.medium.com/death-of-an-open-source-business-model-62bc227a7e9b)（Tiếng Anh）

Phân tích xu hướng các nhà cung cấp dịch vụ đám mây lớn (như AWS) lấy mã nguồn mở miễn phí của các startup để tự đóng gói thành dịch vụ thương mại Cloud cạnh tranh trực tiếp, phá vỡ mô hình doanh thu truyền thống của các nhà phát triển open-source gốc.

7、[Sử dụng thẻ HTML `<details>` để làm footnote chú thích chân trang](https://shkspr.mobi/blog/2020/12/a-terrible-way-to-do-footnotes-in-html/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121102.jpg)

Một mẹo nhỏ sử dụng thẻ HTML5 native `<details>` và `<summary>` để trình bày phần chú thích footnote thu gọn đẹp mắt ngay dưới chân bài viết.

8、[Mẫu viết file script Bash an toàn và súc tích](https://betterdev.blog/minimal-safe-bash-script-template/)（Tiếng Anh）

Giới thiệu bộ khung khai báo cấu hình đầu file Bash giúp script tự động dừng hoạt động khi gặp lỗi biến số hoặc lệnh lỗi, hỗ trợ viết code an toàn hơn.

9、[Hướng dẫn dùng GitHub Actions deploy trang blog tĩnh lên GitHub Pages](https://itsopensource.com/publish-github-pages-with-github-actions/)（Tiếng Anh）

Các bước cấu hình luồng CI/CD tự động build mã nguồn Markdown thành trang web tĩnh và đẩy lên host GitHub Pages miễn phí thông qua GitHub Actions.

10、[Các thuộc tính thử nghiệm của đối tượng `navigator` trong JavaScript](https://umaar.com/dev-tips/242-considerate-javascript/)（Tiếng Anh）

Giới thiệu cách dùng API trình duyệt để đọc các thông số phần cứng thiết bị của người dùng như dung lượng RAM (`navigator.deviceMemory`), số nhân CPU (`navigator.hardwareConcurrency`) để tối ưu hóa hiệu năng render phù hợp.

## 工具

1、[imgdiff](https://github.com/n7olkachev/imgdiff)

Công cụ dòng lệnh CLI tốc độ cao hỗ trợ so sánh và trực quan hóa điểm khác biệt giữa hai bức ảnh.

2、[BrowserTime](https://github.com/seanmiller802/BrowserTime)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121707.jpg)

Extension dành cho Chrome giúp phân tích lịch sử lướt web hiển thị dưới dạng biểu đồ tròn thống kê các trang web ngốn nhiều thời gian sử dụng nhất của bạn.

3、[AI Picture Restorer](https://hotpot.ai/restore-picture)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121802.jpg)

Công cụ trực tuyến ứng dụng AI giúp tự động xóa bỏ các vết xước, nếp gấp gãy trên các bức ảnh đen trắng cũ để phục chế lại ảnh.

4、[Cloudflare Pages](https://blog.cloudflare.com/cloudflare-pages/)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121901.jpg)

Dịch vụ build và deploy hosting cho trang web tĩnh mới ra mắt của Cloudflare cạnh tranh trực tiếp với Netlify và Vercel. ([@Wazons](https://github.com/ruanyf/weekly/issues/1559) đóng góp)

5、[Geometrize](https://www.geometrize.co.uk/)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122001.jpg)

Công cụ trực tuyến giúp chuyển đổi bức ảnh chụp thông thường thành các bức tranh nghệ thuật được vẽ bằng cách chồng lấp các hình khối hình học phẳng (tam giác, hình tròn) độc đáo:

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122002.jpg)

6、[OwnCast](https://github.com/owncast/owncast)

Giải pháp máy chủ livestream video tự vận hành mã nguồn mở giúp bạn tự phát sóng trực tiếp video cá nhân mà không cần phụ thuộc các nền tảng lớn.

7、[tetris](https://github.com/k-vernooy/tetris)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122104.jpg)

Trò chơi xếp hình Tetris cổ điển chạy trực tiếp ngay trên giao diện dòng lệnh terminal của hệ thống.

8、[Holiday Card Maker](https://photoroom.com/holiday-card-maker/)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122302.jpg)

Công cụ online giúp tự động bóc tách nền chân dung người dùng và ghép vào các khung thiệp chúc mừng Giáng sinh hay Năm mới đẹp mắt.

## Tài nguyên

1、[恐龙的声音](https://www.google.com/search?q=what%20sound%20does%20a%20dinosaur%20make)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122003.jpg)

Tính năng thú vị trên Google Search: Chỉ cần gõ từ khóa "what sound does a dinosaur make", trang kết quả sẽ hiển thị bảng âm thanh mô phỏng tiếng kêu của các loài khủng long cổ xưa để bấm nghe.

2、[Bản dịch tiếng Trung các bài blog kỹ thuật của trường Elixir School](https://github.com/caicaishmily/elixirschool_blogs)

Kho lưu trữ bản dịch tiếng Trung các bài viết chuyên sâu chia sẻ kinh nghiệm lập trình ngôn ngữ Elixir. ([@caicaishmily](https://github.com/ruanyf/weekly/issues/1558) đóng góp)

3、[School of SRE của LinkedIn](https://linkedin.github.io/school-of-sre/)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120902.jpg)

Tài liệu hướng dẫn kỹ năng DevOps và vận hành hệ thống Site Reliability Engineering do đội ngũ kỹ sư LinkedIn biên soạn dành cho nhân viên mới.

4、[Khóa học miễn phí về an ninh bảo mật máy tính](https://opensecuritytraining.info/Training.html)

Tổng hợp 29 bài giảng video chất lượng kèm slide lý thuyết đào tạo về mã độc, dịch ngược mã nguồn và bảo mật hệ thống của OpenSecurityTraining.

5、[Free Python Books List](https://www.pythonkitchen.com/legally-free-python-books-list/)

Danh mục tổng hợp các cuốn sách học lập trình Python được chia sẻ miễn phí hợp pháp trực tuyến.

## 图片

1、[Hệ thống công sự quốc phòng ngụy trang tại Thụy Sĩ](https://www.amusingplanet.com/2015/07/the-camouflaged-military-bunkers-of.html)

Là một quốc gia trung lập nhưng Thụy Sĩ sở hữu hệ thống phòng thủ rất mạnh mẽ. Dọc dãy Alps được bố trí dày đặc các hầm hào, công sự quân sự ngụy trang khéo léo để hòa lẫn vào cảnh quan thiên nhiên xung quanh.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120811.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120812.jpg)

Một số lô cốt được ngụy trang giống hệt khối đá tự nhiên khổng lồ, số khác trông như một căn nhà gỗ nghỉ dưỡng yên bình giữa rừng nhưng thực chất có thiết kế cửa sập mở ra các bệ pháo binh hạng nặng.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120813.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120814.jpg)

Thụy Sĩ xây dựng khoảng 300.000 hầm trú ẩn cá nhân và hơn 5.100 hầm trú ẩn công cộng, đủ sức chứa cho toàn bộ dân số cả nước trong trường hợp xảy ra chiến tranh hủy diệt.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120815.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120816.jpg)

## Bài đọc thêm

### 1. Đồng hồ Ngày tận thế (Doomsday Clock)

Năm 1945 sau khi Mỹ ném hai quả bom nguyên tử xuống Nhật Bản, thế giới bước vào kỷ nguyên lo ngại chiến tranh hạt nhân hủy diệt toàn cầu. Năm 1947, nhóm các nhà vật lý hạt nhân tham gia dự án Manhattan đã xuất bản tạp chí *Bulletin of the Atomic Scientists* với ảnh bìa vẽ một chiếc đồng hồ đếm ngược đến giờ G hủy diệt.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112902.jpg)

Thời điểm nửa đêm 12 giờ đại diện cho thảm họa hủy diệt thế giới, và chiếc kim đồng hồ đầu tiên được đặt ở mức 11 giờ 53 phút (còn 7 phút nữa tới nửa đêm). Chiếc đồng hồ này được gọi là "Đồng hồ Ngày tận thế".

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112904.jpg)

Kể từ đó, vị trí kim đồng hồ liên tục được ban biên tập điều chỉnh dựa trên tình hình căng thẳng địa chính trị và biến đổi khí hậu toàn cầu, tính đến nay đã có 22 lần thay đổi:
- **1949**: Liên Xô thử thành công bom nguyên tử, kim đồng hồ nhích lên mức còn 3 phút.
- **1953**: Mỹ và Liên Xô thử nghiệm bom khinh khí (bom H), kim nhích lên mức còn 2 phút.
- **1991**: Chiến tranh Lạnh kết thúc, hiệp ước giảm vũ khí hạt nhân được ký kết, kim lùi về mức xa nhất lịch sử là còn 17 phút.
- **2020**: Do biến đổi khí hậu nghiêm trọng không thể đảo ngược và căng thẳng leo thang, kim đồng hồ được điều chỉnh về mức sát giờ G nhất lịch sử là **còn 100 giây**.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112903.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112905.jpg)

### 2. Vấn nạn các hội nghị khoa học rác của tổ chức WASET

Nhiều năm qua, một tổ chức của Thổ Nhĩ Kỳ tên là WASET (World Academy of Science, Engineering and Technology) đã liên tục đăng ký và tổ chức hàng chục nghìn hội nghị khoa học giả mạo trên toàn cầu. Các hội nghị này có tên gọi gần như trùng khớp với các hội nghị của các viện nghiên cứu uy tín.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121403.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121404.jpg)

Năm 2018, WASET đã chạy quảng cáo cho 49.844 hội nghị khoa học tự phong, nhiều sự kiện được tổ chức chung địa điểm và thời gian tại các khách sạn để tối ưu chi phí. Ví dụ tháng 2 năm 2016 tại một khách sạn ở Rio de Janeiro ghi nhận có tới 116 hội nghị khoa học diễn ra cùng lúc.

Chất lượng của các hội nghị này cực kỳ tệ, bất kỳ ai nộp tiền đăng ký đều có thể gửi bài báo và được phê duyệt xuất bản. Năm 2013 xảy ra vụ bê bối khi một nhà khoa học Anh cố tình gửi một bài viết giả lập chứa các số liệu ngẫu nhiên vô nghĩa về y học lên tạp chí của WASET và vẫn được duyệt xuất bản dễ dàng. Ước tính doanh thu của WASET riêng trong năm 2017 đạt khoảng 4,5 triệu USD từ việc thu phí của các nghiên cứu sinh cần làm đẹp hồ sơ học thuật của mình.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121405.jpg)

## 言论

1、

Đừng để bản thân bị cuốn vào các mục tiêu tham lam của các tập đoàn tư bản, đừng cống hiến toàn bộ thời gian và năng lượng cuộc sống cho họ. Điều đó chắc chắn sẽ khiến bạn đánh mất cuộc đời mình mà không có bất kỳ lý do chính đáng nào.

-- Jonathan Carter, Trưởng dự án hệ điều hành Debian

2、

Những người có tư duy lớn thường thảo luận về các ý tưởng; những người có tư duy trung bình thảo luận về các sự kiện; còn những người có tư duy hẹp hòi chỉ tập trung bàn tán về con người.

-- Eleanor Roosevelt

3、

Mỗi ngày, cơ thể con người cần tiêu thụ lượng năng lượng sinh học tương đương công suất một bóng đèn 90W để duy trì sự sống. Tuy nhiên, nếu tính cả lượng năng lượng tiêu thụ cho các thiết bị sinh hoạt, xe cộ đi lại... một người bình thường thời nay ngốn khoảng 3.000W mỗi ngày. Nếu bạn là một người Mỹ, con số này vọt lên mức 11.000W - tương đương lượng năng lượng tiêu thụ của một chú cá voi xanh (động vật lớn nhất Trái Đất).

-- Geoffrey West (Nhà vật lý học)

4、

Việc đọc nhiều tài liệu, sách báo chỉ giúp bạn biết thêm thông tin chứ không giúp bạn nâng cao kỹ năng của bản thân. Chỉ có quá trình bắt tay vào thực hành (practice) liên tục mới giúp nâng cao tay nghề. Nếu muốn tiến bộ hơn, hãy bắt tay vào tự làm sản phẩm thực tế.

-- Jason Fried (Nhà sáng lập Basecamp)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121501.jpg)

## 回顾

Tuần này năm 2019 (số 88): [Nếu bạn gặp phải một con rắn](http://www.ruanyifeng.com/blog/2019/12/weekly-issue-88.html)

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019113002.jpg)

Tuần này năm 2018 (số 36): [Lập trình viên tương lai có bị dư thừa?](http://www.ruanyifeng.com/blog/2018/12/weekly-issue-36.html)

![](https://cdn.beekka.com/blogimg/asset/201812/bg2018122129.jpg)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
