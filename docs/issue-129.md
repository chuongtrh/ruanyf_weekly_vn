# 科技爱好者周刊（第 129 期）：Hàm lồi và hàm lõm trong khởi nghiệp

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1392) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100716.jpg)

Tác phẩm nghệ thuật sắp đặt "Trứng ốp la trên phố" của nghệ sĩ người Hà Lan Henk Hofstra tại thành phố São Paulo, Brazil. ([Nguồn](https://www.instagram.com/p/CFWQkdOBulW/))

## Chủ đề tuần này: Hàm lồi và hàm lõm trong khởi nghiệp

Nassim Taleb, tác giả của cuốn sách bán chạy nổi tiếng [《Thiên Nga Đen》](https://book.douban.com/subject/6854525/), cựu giáo sư toán học tại Đại học New York, sau đó hoạt động trong ngành tài chính toán học và quản lý rủi ro. Ông đã viết rất nhiều bài viết phổ biến kiến thức, sử dụng các khái niệm toán học để phân tích các hiện tượng trong đời sống.

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100903.jpg)

Ông có một [quan điểm](https://www.indiehackers.com/post/bootstrapping-and-convexity-fb3b2da7c9) mà tôi thấy rất mới mẻ: **Khi khởi nghiệp, bạn cần cân nhắc hướng đi đó là hàm lồi hay hàm lõm.**

Hiểu một cách đơn giản, hàm lồi (*convex function*) có đường cong mở hướng lên (hình bên trái dưới), còn hàm lõm (*concave function*) có đường cong mở hướng xuống (hình bên phải dưới).

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100904.jpg)

Taleb nói rằng hướng đi khởi nghiệp tốt nhất là đường cong dưới đây:

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100905.jpg)

Trục đứng là lợi nhuận (phần dương là lãi, phần âm là lỗ), trục ngang đại diện cho các biến số ngoại cảnh (phần dương là các yếu tố thuận lợi, phần âm là bất lợi). Khi mới bắt đầu, lợi nhuận của bạn là 0 (giao điểm của đường cong với trục ngang), bạn chưa biết tương lai sẽ thế nào.

Một mô hình khởi nghiệp tốt sẽ hoạt động theo đường cong này: Khi môi trường bên ngoài thuận lợi, lợi nhuận của bạn tăng trưởng phi mã và không gian tăng trưởng gần như là khổng lồ; ngược lại khi gặp bất lợi, thua lỗ tích lũy một cách chậm rãi và mức thiệt hại tối đa được giới hạn rõ ràng. Đường cong này chính là hàm lồi. 

Ngược lại nếu khởi nghiệp của bạn thuộc kiểu hàm lõm thì rất nguy hiểm: cơ hội sinh lời bị giới hạn bởi một trần doanh thu cố định và tăng trưởng chậm, nhưng thua lỗ lại có thể tăng nhanh chóng và không có giới hạn.

Ví dụ, dự án khởi nghiệp của bạn là một phần mềm mã nguồn mở chưa có mô hình kinh doanh rõ ràng và bạn còn từ bỏ công việc hiện tại để làm toàn thời gian, thì đó là khởi nghiệp kiểu hàm lõm. Bạn sẽ phải làm việc rất vất vả, và nếu thất bại thì hậu quả sẽ rất thê thảm.

Một số bạn trẻ nghỉ việc khi chưa tìm được công việc mới (*naked resignation*), hành vi này cũng thuộc kiểu hàm lõm. Nếu công việc tiếp theo cũng chỉ tương tự, lương của bạn tăng được bao nhiêu? Nhưng nếu không tìm được việc, bạn sẽ rơi vào cảnh thất nghiệp dài hạn và bị động hoàn toàn.

Việc sử dụng các khái niệm toán học để phân tích các hành vi thường nhật như thế này thật sự rất thú vị. Đây cũng là điểm tôi khâm phục các học giả phương Tây, họ có khả năng mô hình hóa (*modelization*) và khái niệm hóa (*conceptualization*) những hiện tượng quen thuộc để suy nghĩ từ góc nhìn hoàn toàn mới. **Đây gọi là "năng lực trừu tượng hóa", rất đáng để học hỏi: biến những thứ cụ thể thành trừu tượng, và ngược lại, biến những thứ trừu tượng thành cụ thể.**

## Dịch vụ Identity Cloud (IDaaS) - Authing

Tuần này, tôi xin giới thiệu một dịch vụ đám mây nội địa: [Authing](https://authing.cn/).

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101004.png)

Bước đầu tiên khi sử dụng bất kỳ ứng dụng Internet nào luôn là đăng ký hoặc đăng nhập. Xu hướng hiện nay là sử dụng đăng nhập thông qua bên thứ ba (Single Sign-On qua Google, Facebook, GitHub) để xác thực danh tính người dùng.

Phương pháp này mang lại sự tiện lợi cho cả hai bên: Người dùng không cần đăng ký tài khoản mới; nhà phát triển không cần tốn công quản lý cơ sở dữ liệu danh tính mà có thể tập trung vào logic cốt lõi của sản phẩm. Tuy nhiên, việc hỗ trợ nhiều chuẩn kết nối từ các nhà cung cấp khác nhau thường tốn nhiều công sức bảo trì và phát triển.

**[Authing](https://authing.cn/) chính là dịch vụ Identity Cloud (IDaaS) giải quyết tất cả các khâu xác thực và quản lý tài khoản cho ứng dụng doanh nghiệp.** 

Mặc định, nhà phát triển chỉ cần nhúng một đoạn [script](https://github.com/Authing/Guard), biểu mẫu đăng nhập dưới đây sẽ tự động hiển thị để xử lý toàn bộ quy trình:

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101005.png)

Trong trang quản trị, bạn có thể cấu hình hỗ trợ đăng nhập qua các nhà cung cấp phổ biến tại Trung Quốc như WeChat, QQ, Alipay, Weibo, DingTalk... Hỗ trợ tích hợp mượt mà cho cả Web, Mobile App và Mini Program.

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101006.png)

Dịch vụ cũng cung cấp các tính năng nâng cao như SSO đơn điểm, xác thực đa yếu tố (MFA), xác thực OTP qua tin nhắn SMS cùng bộ SDK hỗ trợ hầu hết các ngôn ngữ lập trình phổ biến để tích hợp vào hệ thống hiện có.

Authing cam kết về an toàn thông tin khi không lưu trữ dữ liệu người dùng trực tiếp mà để doanh nghiệp toàn quyền kiểm soát dữ liệu, đồng thời áp dụng nhiều lớp bảo mật để tránh rò rỉ thông tin trong khâu đăng nhập.

Hiện nay, nhiều tập đoàn lớn như PetroChina, China Merchants Bank đã sử dụng Authing làm giải pháp xác thực nội bộ. Authing vừa nâng cấp lên phiên bản 2.0 chuyển sang kiến trúc đám mây đa khách thuê (*multi-tenant*) giúp tối ưu hiệu năng và tốc độ truy cập.

Bạn có thể đăng ký dùng thử miễn phí Authing tại [đây](https://docs.authing.cn/quickstart/create-authing-account.html). Gói miễn phí hỗ trợ 3.000 lượt xác thực mỗi tháng và chỉ tính phí dựa trên số lượng người dùng hoạt động.

## Tin tức

1、[Bao lì xì Nhân dân tệ kỹ thuật số](https://finance.sina.com.cn/china/gncj/2020-10-10/doc-iivhuipp8791865.shtml)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101001.jpg)

Thâm Quyến bắt đầu thử nghiệm đồng Nhân dân tệ kỹ thuật số (e-CNY) bằng cách quay số ngẫu nhiên chọn ra 50.000 người dân, mỗi người nhận một bao lì xì trị giá 200 tệ (tổng trị giá 10 triệu tệ). Số tiền này có thể dùng để mua sắm tại các cửa hàng được chỉ định tại quận La Hồ.

Để nhận tiền, người trúng thưởng phải tải ứng dụng "e-CNY", mở ví kỹ thuật số cá nhân. Khoản tiền này có giá trị tương đương tiền mặt và có thể chi tiêu trực tiếp không cần liên kết với thẻ ngân hàng.

Đồng e-CNY cũng hỗ trợ tính năng thanh toán ngoại tuyến (offline), chỉ cần hai điện thoại chạm nhẹ vào nhau là có thể chuyển tiền từ ví này sang ví khác ngay cả khi không có kết nối mạng mạng di động.

2、[Ảnh tự chụp của Tianwen-1](https://www.sohu.com/a/422325427_338398)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100712.jpg)

Tianwen-1 là tàu thăm dò sao Hỏa đầu tiên của Trung Quốc, được phóng lên vào ngày 23 tháng 7 năm 2020. Vào ngày 1 tháng 10, trên đường bay tới sao Hỏa, Tianwen-1 đã thực hiện một bức ảnh tự chụp gửi về Trái Đất.

Để chụp được toàn cảnh con tàu mà không gặp rủi ro an toàn từ gậy selfie dài 15 mét, các kỹ sư đã thiết kế một camera nhỏ dùng một lần. Khi phóng camera ra không gian với tốc độ 0,2 m/s, nó chụp ảnh rồi truyền dữ liệu về tàu thông qua kết nối Wi-Fi phạm vi 400 mét. Camera hỗ trợ độ phân giải tối đa 1600×1200 và pin chạy được khoảng 1 giờ.

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100713.jpg)

3、[Kho ứng dụng quốc doanh của Ấn Độ](https://www.deccanherald.com/specials/aatmanirbhar-bharat-modi-govt-to-set-up-app-store-alternative-to-google-play-apple-app-store-895755.html)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100406.jpg)

Việc Google bắt đầu thu 30% phí hoa hồng đối với các giao dịch mua hàng trong ứng dụng đã ảnh hưởng rất lớn đến các nhà phát triển Ấn Độ. Theo báo cáo, Thủ tướng Ấn Độ Narendra Modi đã yêu cầu Bộ Điện tử và CNTT xây dựng một cửa hàng ứng dụng di động của quốc gia để giúp lập trình viên tránh khoản phí thu này từ Google.

Tại Ấn Độ, Android chiếm 97% thị phần hệ điều hành trong khi iOS chỉ chiếm 2%, vì vậy một kho ứng dụng Android thay thế có thể tiếp cận hầu hết người dùng di động tại nước này.

4、[Bộ nhận diện thương hiệu mới của Google Workspace](https://9to5google.com/2020/10/06/new-gmail-icon/)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100703.jpg)

Google tiến hành hợp nhất các công cụ gửi thư, lịch, văn phòng và gọi video thành Google Workspace (thay thế cho thương hiệu G Suite cũ). Để đồng bộ hóa, các biểu tượng dịch vụ đã được thiết kế lại theo tông màu chủ đạo thống nhất.

Dưới đây là các biểu tượng mới của Gmail, Lịch, Tài liệu, Meet và Chat:

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100704.jpg)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100705.jpg)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100706.jpg)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100707.jpg)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100708.jpg)

5、[Dịch vụ taxi không người lái Waymo One](https://auto-time.36kr.com/p/916577169093378)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101003.jpg)

Ngày 9 tháng 10, Waymo (công ty con mảng tự hành của Alphabet) thông báo mở cửa dịch vụ taxi không người lái hoàn toàn cho công chúng tại khu vực Phoenix với đội xe ban đầu khoảng 3.000 chiếc. Đây là dịch vụ taxi tự hành thương mại đầu tiên trên thế giới vận hành mà không cần nhân viên an toàn ngồi trên xe.

Mặc dù không có tài xế trực tiếp, nhân viên của Waymo vẫn theo dõi tình trạng xe từ xa qua hệ thống camera và hỗ trợ hành khách khi có yêu cầu.

Một người dùng Reddit đã chia sẻ video hành trình dài 4 phút đi taxi tự hành vào ban đêm. Xe di chuyển mượt mà, dừng đèn đỏ chuẩn xác và tự động đỗ xe. Nhiều người nhận xét điều đáng sợ nhất không phải là độ an toàn của chiếc xe, mà là những tài xế đi đường xung quanh khi nhìn vào cabin trống không của xe Waymo sẽ bị giật mình.

6、**Tin tức một câu**

> - [Các nhà nghiên cứu Đức](https://www.bbc.com/news/science-environment-54515518) hoàn thành chuyến khảo sát Bắc Cực kéo dài 1 năm, cảnh báo về tốc độ tan băng kỷ lục tại đây. Dưới đây là bản đồ so sánh diện tích băng Bắc Cực năm 2020 (trái) so với năm 1980 (phải), màu xanh là băng, màu trắng là đại dương.

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101501.jpg)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101502.jpg)

> - [Một startup của Mỹ](https://peripherii.com/) thiết kế tai nghe Bluetooth dưới hình dạng khuyên tai thời trang, truyền âm thanh trực tiếp thông qua lỗ xỏ khuyên.

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101504.jpg)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101505.jpg)

> - [Nghiên cứu của Mỹ](https://spectrum.ieee.org/energywise/green-tech/fuel-cells/spinach-gives-fuel-cells-a-power-up) phát hiện rau chân vịt (cải bó xôi) có thể làm chất xúc tác giá rẻ cho pin nhiên liệu nhờ chứa hàm lượng sắt và nitơ dồi dào, giảm phụ thuộc vào các chất xúc tác kim loại quý hiếm.

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101503.jpg)

> - [Amazon](http://www.southgatearc.org/news/2020/october/sale-of-amateur-radio-amprnet-tcp-ip-addresses.htm) đã bỏ ra 108 triệu USD mua lại 4 triệu địa chỉ IPv4 từ Hiệp hội vô tuyến nghiệp dư toàn cầu do cạn kiệt tài nguyên địa chỉ IPv4.

> - [Mức tiêu thụ dữ liệu SIM di động trung bình ở Phần Lan](https://twitter.com/mikko/status/1315178802356649986) đạt 17.3 GB/tháng, cao nhất thế giới, cho thấy sự phổ biến vượt trội của các dịch vụ di động không dây tại đây.

## Bài viết

1、[Bố cục bài viết toàn màn hình (full-bleed) với CSS Grid](https://joshwcomeau.com/css/full-bleed/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100601.jpg)

Hướng dẫn dùng CSS Grid để căn lề bố cục bài viết để ảnh hoặc bảng biểu có thể tràn viền hai bên (full-bleed) đẹp mắt. Xem thêm phương pháp truyền thống tại [đây](https://uglyduck.ca/poor-mans-full-bleed/).

2、[Hướng dẫn sử dụng extension Vimium](https://codefaster.substack.com/p/look-ma-no-mouse-vimium)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100701.jpg)

Vimium là tiện ích mở rộng trên Chrome giúp người dùng duyệt web nhanh chóng bằng các phím tắt của trình biên dịch Vim mà không cần chạm vào chuột.

3、[Các khái niệm cơ bản trong phát triển game với Unity](https://blog.eyas.sh/2020/10/unity-for-engineers-pt1-basic-concepts/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101201.jpg)

Bài viết giới thiệu các thuật ngữ nền tảng trong Unity dành cho lập trình viên mới bắt đầu tiếp cận mảng game dev.

4、[Tùy biến ký hiệu đầu dòng danh sách bằng CSS `::marker`](https://web.dev/css-marker-pseudo-element/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100804.jpg)

Từ phiên bản Chrome 86, lập trình viên có thể dùng pseudo-element `::marker` để tùy biến các ký tự hay số đầu dòng trong thẻ `<ul>` và `<ol>`.

5、[Hãy quên các dự án cá nhân đi và tập trung vào công việc chính](https://manuel.darcemont.fr/posts/focus-on-jour-job/)（Tiếng Anh）

Lời khuyên cho các lập trình viên trẻ: Đừng làm các side project một cách lan man thiếu định hướng, hãy làm những dự án cá nhân có tính liên kết trực tiếp giúp bổ trợ kiến thức cho công việc hàng ngày của bạn.

6、[Chrome thay đổi cơ chế phân vùng bộ nhớ đệm HTTP](https://developers.google.com/web/updates/2020/10/http-cache-partitioning)（Tiếng Anh）

Để tránh việc các bên thứ ba lợi dụng bộ nhớ cache của trình duyệt để theo dõi lịch sử duyệt web của người dùng, Chrome 86 bắt đầu phân vùng bộ nhớ đệm HTTP (HTTP Cache Partitioning) dựa trên tên miền của trang web truy cập.

7、[Tại sao sử dụng chung CDN cho thư viện JS không còn là ý tưởng hay](https://shkspr.mobi/blog/2020/10/please-stop-using-cdns-for-external-javascript-libraries/)（Tiếng Anh）

Phân tích ảnh hưởng của cơ chế phân vùng cache mới trên Chrome 86: Việc tải các thư viện JS dùng chung qua CDN (như jQuery, React) sẽ không còn giúp trang web load nhanh hơn do trình duyệt không dùng lại cache từ trang web khác nữa.

8、[Cách viết bộ ứng dụng văn phòng tối giản nhất](https://zserge.com/posts/awfice/)（Tiếng Anh）

Cách tận dụng các tính năng sẵn có trên trình duyệt để tạo ra trình soạn thảo văn bản, bảng tính spreadsheet và slide trình chiếu siêu nhỏ gọn.

9、[Tự viết một phiên bản React tối giản dưới 1KB](https://zserge.com/posts/worst-react-ever/)（Tiếng Anh）

Hướng dẫn xây dựng một thư viện lõi tương tự React hỗ trợ cú pháp JSX và các API cơ bản để hiểu sâu cơ chế hoạt động bên dưới của React.

10、[Tình trạng hỗn loạn mua bán Star trên GitHub](https://www.pingwest.com/a/177413)（Tiếng Trung）

Bài viết phản ánh thực trạng một bộ phận lập trình viên Trung Quốc đang tìm cách mua bán Star để lọt vào bảng xếp hạng GitHub Trending.

## Công cụ

1、[playwright-python](https://github.com/microsoft/playwright-python)

Thư viện tự động hóa trình duyệt web của Microsoft hỗ trợ viết kịch bản điều khiển bằng ngôn ngữ Python.

2、[Anbox](https://anbox.io/)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100508.jpg)

Dự án mã nguồn mở chạy hệ điều hành Android trong container trên các bản phân phối Linux.

3、[Diagram Maker](https://github.com/awslabs/diagram-maker)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100602.jpg)

Thư viện JavaScript do AWS phát triển giúp vẽ sơ đồ luồng (flowchart) tương tác trên web.

4、[DigitalOcean App Platform](https://www.digitalocean.com/blog/introducing-digitalocean-app-platform-reimagining-paas-to-make-it-simpler-for-you-to-build-deploy-and-scale-apps)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100702.jpg)

Nền tảng PaaS mới của DigitalOcean cho phép deploy và mở rộng quy mô ứng dụng tự động trực tiếp từ kho lưu trữ GitHub.

5、[Apache JMeter](https://www.2n.pl/blog/apache-jmeter)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100711.jpg)

Công cụ mã nguồn mở quen thuộc dùng để chạy thử nghiệm hiệu năng và tải của hệ thống.

6、[nb](https://github.com/xwmx/nb)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100803.jpg)

Công cụ ghi chú trên dòng lệnh CLI hỗ trợ định dạng Markdown và mã hóa dữ liệu.

7、[Frame](https://framevr.io/)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100815.jpg)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100814.jpg)

Không gian họp ảo 3D trực quan chạy trực tiếp trên trình duyệt, hỗ trợ tương tác kính VR.

8、[optimizt](https://github.com/funbox/optimizt)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100901.jpg)

Công cụ nén ảnh CLI hỗ trợ định dạng PNG, JPEG, GIF, SVG và có tùy chọn chuyển đổi sang định dạng WebP.

9、[Calligrapher.ai](https://www.calligrapher.ai/)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100902.jpg)

Công cụ AI biến chữ gõ tiếng Anh thành chữ viết tay động dạng hình ảnh vector SVG.

10、[github-daily](https://github.com/headllines/github-daily)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020101603.jpg)

Công cụ dùng GitHub Actions tự động ghi nhận danh sách Top 10 dự án GitHub Trending mỗi ngày lưu vào issue để người dùng theo dõi. ([@timqian](https://github.com/ruanyf/weekly/issues/1440) đóng góp)

## Tài nguyên

1、[CSS 3D 示例](https://polypane.app/css-3d-transform-examples/)

Bộ sưu tập các ví dụ trực quan sử dụng thuộc tính 3D transform trong CSS.

2、[漫游者的压缩知识指南](https://go-compression.github.io/)

Tài liệu tiếng Anh giới thiệu căn bản về các thuật toán nén dữ liệu cho người mới bắt đầu.

3、[Mô hình 100,000 Stars](http://stars.chromeexperiments.com/)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100710.jpg)

Dự án tương tác 3D trên trình duyệt hiển thị vị trí của hơn 100.000 ngôi sao trong thiên hà.

4、[names.io](https://github.com/Debdut/names.io)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100802.jpg)

Dataset lưu trữ kho tên tiếng Anh được tổng hợp chia theo tệp tin Họ và Tên riêng.

## Hình ảnh

1、[Nhà máy gốm sứ hiện đại](https://www.archdaily.cn/cn/918363/jing-de-zhen-bing-ding-chai-yao-zhang-lei-lian-he-jian-zhu-shi-wu-suo)

Một lò nung gốm truyền thống tại làng Tiền Trình, Cảnh Đức Trấn được các kiến trúc sư cải tạo thành một công trình kiến trúc bê tông hiện đại ấn tượng.

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100810.jpg)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100813.jpg)

Công trình hòa quyện giữa nét hiện đại công nghiệp và khung cảnh núi rừng thiên nhiên bao quanh.

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100812.jpg)

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100811.jpg)

2、[Màu sắc bầu trời ở độ cao 7.000 mét](https://www.dcfever.com/news/readnews.php?id=28338)

Màu của bầu trời khi nhìn từ mặt đất là màu xanh lam, nhưng ở độ cao 7.000 mét liệu nó có còn màu xanh?

Nhiếp ảnh gia người Nhật Ueda Yuki chia sẻ những bức ảnh chụp trên dãy Himalaya: "Càng lên cao, màu sắc bầu trời càng đậm dần. Khi vượt qua độ cao 7.000 mét, bầu trời chuyển sang màu xanh thẫm gần như đen thẳm của vũ trụ."

![](https://cdn.beekka.com/blogimg/asset/202007/bg2020071401.jpg)

![](https://cdn.beekka.com/blogimg/asset/202007/bg2020071402.jpg)

![](https://cdn.beekka.com/blogimg/asset/202007/bg2020071403.jpg)

Nguyên nhân chính là ở độ cao lớn, mật độ không khí loãng và ít hạt bụi lơ lửng khiến hiện tượng tán xạ ánh sáng xanh giảm đi đáng kể.

## Bài đọc thêm

### 1. Rủi ro công việc và rủi ro sự nghiệp

Có quan điểm cho rằng trước khi khởi nghiệp, bạn nên làm việc ở các tập đoàn lớn để tích lũy quan hệ, kỹ năng và thương hiệu cá nhân.

Tôi không đồng ý với quan điểm này. Việc làm ở công ty lớn chỉ giúp bạn học được cách vận hành trong môi trường tập đoàn lớn. Trong khi khởi nghiệp đòi hỏi đi từ 0 đến 1, một bộ kỹ năng hoàn toàn khác biệt.

Chúng ta có thể phân loại rủi ro thành hai loại:
- **Rủi ro công việc**: Khả năng công việc hiện tại của bạn biến mất.
- **Rủi ro sự nghiệp**: Khả năng sự nghiệp dài hạn bị ảnh hưởng tiêu cực.

Khởi nghiệp có rủi ro công việc cực kỳ cao (dễ mất việc nếu công ty đóng cửa), nhưng lại giúp giảm thiểu rủi ro sự nghiệp dài hạn. Việc khởi nghiệp thất bại không làm hồ sơ của bạn xấu đi. Ngược lại, trong mắt nhiều nhà tuyển dụng, đó là minh chứng cho việc bạn đã dấn thân và có trải nghiệm thực chiến.

Nếu bạn thực sự muốn lập công ty riêng, hãy bắt đầu sớm nhất có thể thay vì nghĩ mình phải tích lũy kinh nghiệm làm thuê trước.

### 2. Sự ra đời của ca ghép tim đầu tiên

*Tác giả: Bill Bryson*

Ghép tim từng là giấc mơ y học đối mặt với rào cản pháp lý lớn: Bác sĩ chỉ được tuyên bố người hiến tặng tử vong khi tim ngừng đập, nhưng khi tim ngừng đập thì nó sẽ không còn khả năng cấy ghép nữa.

![](https://cdn.beekka.com/blogimg/asset/202010/bg2020100801.jpg)

Năm 1967, tại Nam Phi (nơi không áp dụng điều luật này), bác sĩ Christiaan Barnard đã ghép tim của một phụ nữ trẻ qua đời vì tai nạn giao thông vào lồng ngực bệnh nhân Louis Washkansky 54 tuổi. Ca ghép thành công vang dội dù bệnh nhân qua đời sau đó 18 ngày do nhiễm trùng. Ca ghép thứ hai của ông giúp bệnh nhân sống thêm được 19 tháng.

Sự kiện này thúc đẩy các quốc gia thay đổi định nghĩa y học sang "chết não" để tạo điều kiện ghép tạng. Trở ngại lớn tiếp theo là hiện tượng thải ghép tạng. Năm 1969, một nhân viên hãng dược Sandoz đi nghỉ mát tại Na Uy đã mang một mẫu đất về phòng thí nghiệm. Mẫu đất chứa loài nấm *Tolypocladium inflatum* tuy không có tính kháng sinh nhưng lại giúp ức chế miễn dịch cực tốt, mở đường chế tạo thuốc chống thải ghép Cyclosporine đưa tỷ lệ ghép tim thành công lên 80% vào thập niên 80.

## Danh ngôn

1、

Hơn một trăm năm trước, nhà vật lý học người Mỹ Henry Rowland đã phát biểu rằng nếu chúng ta chỉ chăm chăm ứng dụng khoa học mà ngừng phát triển khoa học cơ bản, chúng ta sẽ sớm tụt hậu. Người Trung Quốc cổ xưa có rất ít tiến bộ khoa học dài hạn vì họ chỉ thỏa mãn với việc ứng dụng thực tế mà không bao giờ truy vấn đến tận cùng nguyên lý của tự nhiên.

-- [《Mỹ chưa từng từ bỏ ngành sản xuất chế tạo》](https://finance.sina.com.cn/china/2020-09-18/doc-iivhuipp5079056.shtml)

2、

Trong suốt 500 năm từ năm 1320 đến năm 1820, nước Anh không thành lập thêm bất kỳ một trường đại học mới nào do đại học Oxford và Cambridge đã kiến nghị Vua Edward III cấm thành lập trường mới để duy trì vị thế độc quyền của mình.

-- [《Trường đại học cổ đại》](https://viaappia.substack.com/p/the-ancient-universities)

3、

Để có được những phần mềm mã nguồn mở xuất sắc như Calibre, xã hội cần những nhà phát triển có phần lập dị sẵn sàng cống hiến thời gian cá nhân của mình để tạo ra sản phẩm hoàn toàn miễn phí cho cộng đồng.

-- Độc giả Hacker News

4、

Nếu bạn bắt buộc phải duy trì công việc hiện tại chỉ để chi trả hóa đơn hàng tháng và không có sự tự tin hay cơ hội nào để tìm một công việc khác tốt hơn, thì tức là bạn đang bị mắc kẹt.

-- Độc giả Hacker News

5、

Trí tuệ nhân tạo không cần phải thù ghét chúng ta để tiêu diệt chúng ta. Giống như con người không ghét kiến, nhưng nếu cần xây một đường cao tốc đi qua tổ kiến, chúng ta sẽ san phẳng nó. AI cũng sẽ làm điều tương tự nếu con người cản đường nó.

-– Elon Musk

6、

Đầu óc tôi luôn có quá nhiều suy nghĩ cùng lúc, cảm giác như đang mở quá nhiều tab trình duyệt vậy.

-– Elon Musk

## Nhìn lại

Tuần này năm 2019 (số 78): [Ngành nào sẽ là xu hướng tiếp theo?](http://www.ruanyifeng.com/blog/2019/10/weekly-issue-78.html)

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019101707.jpg)

Tuần này năm 2018 (số 26): [Cuốn sách mới của DHH: Làm việc đâu cần phải điên cuồng](http://www.ruanyifeng.com/blog/2018/10/weekly-issue-26.html)

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018101201.jpg)

## Đăng ký

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97).

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
