# 科技爱好者周刊（第 208 期）：晋升制度的问题

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần. (**[Thông báo] Thứ Sáu tuần tới trùng vào ngày Tết Đoan Ngọ nên bản tin sẽ tạm dừng phát hành một kỳ.**)

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2356) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050920.webp)

Vào tháng 4 năm nay, một cặp vợ chồng yêu thích nhiếp ảnh tại Thạch Gia Trang đã phát hiện một chú chim ưng bụng trắng đang bay một cách khó khăn với một mũi tên cắm sâu ở chân trái. Họ đã gọi điện báo cảnh sát, và sau hơn một tuần kiên trì theo dõi, các nhân viên cứu hộ động vật hoang dã đã bắt được chú chim để tiến hành phẫu thuật điều trị vết thương. (Nguồn: [CDSB](https://static.cdsb.com/micropub/Articles/202204/5d2f9fe9cf8a9a3b9a45943767d30ab1.html))

## 本周话题：晋升制度的问题

Gần đây tôi có đọc được [một bài viết](https://www.warp.dev/blog/problems-with-promotion-oriented-cultures) rất hay của Zach Lloyd, cựu trưởng nhóm phát triển Google Sheets (hiện đã rời Google để tự khởi nghiệp). Ông chia sẻ về sự ngán ngẩm của mình đối với hệ thống đánh giá thăng tiến (promotion system) của Google.

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052405.jpg)

Đọc xong bài viết, tôi nhận thấy hệ thống thăng tiến của Google có nhiều điểm tương đồng với cơ chế vận hành của các tập đoàn công nghệ lớn trong nước. Hành vi của nhân viên phần lớn đều bị định hướng theo tiêu chí thăng tiến và kéo theo những bất cập tương tự.

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052210.webp)

Hiện tại đang là mùa đánh giá thăng tiến - thời điểm được nhiều nhân sự công nghệ mong chờ nhất năm. Thông thường, sau khi năm tài chính kết thúc vào cuối tháng 3, quản lý trực tiếp sẽ đề xuất danh sách nhân sự tiềm năng, và hội đồng phản biện thăng tiến sẽ diễn ra vào tháng 4 và tháng 5. Nếu vượt qua kỳ đánh giá, nhân viên sẽ được tăng cấp bậc (level), tăng lương, thưởng cổ phiếu và khẳng định được vị thế trong công ty. Ngược lại, nếu nhiều năm liền không được thăng tiến, đó là tín hiệu cảnh báo vị thế của bạn đang gặp nguy hiểm.

Vì vậy, không có gì ngạc nhiên khi **hành vi của nhân viên tại các công ty lớn đều bị định hướng theo tiêu chí thăng tiến (promotion-oriented)**. Trước khi bắt tay làm bất kỳ việc gì, câu hỏi đầu tiên họ cân nhắc luôn là liệu việc này có giúp ích cho hồ sơ thăng tiến của mình hay không.

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052211.webp)

Zach Lloyd chỉ ra rằng hệ thống thăng tiến định hướng này dẫn tới 4 vấn đề lớn sau:

**1. Tiêu chí thăng tiến không đồng nhất với lợi ích thực tế của doanh nghiệp:** Nhân viên tập trung vào các kết quả thăng tiến ngắn hạn hơn là giá trị dài hạn cho sản phẩm. 

Ví dụ giữa 2 kỹ sư: kỹ sư A chuyên phát triển tính năng mới hoành tráng, kỹ sư B chuyên thầm lặng bảo trì, sửa lỗi và tối ưu hóa hệ thống cũ. Thường kỹ sư A sẽ được thăng tiến nhanh, còn kỹ sư B gặp bất lợi lớn do đóng góp bảo trì khó định lượng bằng số liệu tăng trưởng trực quan. 

Điều này khuyến khích mọi người thích tự tạo ra các dự án mới (vẽ thêm bánh/造轮子) thay vì làm sạch và tối ưu các dự án cũ đã chạy lâu năm. Đó là lý do tại sao phần mềm của các hãng lớn thường cồng kềnh, nhiều tính năng trùng lặp trong khi các dịch vụ cũ lại thiếu người bảo trì.

**2. Làm gia tăng tính phân cấp hành chính:** Hệ thống tạo ra quá nhiều cấp bậc quản lý trung gian, khiến cấu trúc tổ chức phình to và việc phối hợp giữa các phòng ban trở nên cồng kềnh, quan liêu.

**3. Tạo áp lực căng thẳng và lãng phí thời gian:** Mùa thăng tiến làm nảy sinh các cuộc tranh giành nội bộ và buộc nhân sự phải tiêu tốn hàng tuần thiết kế các trang slide thuyết trình bóng bẩy thay vì tập trung code thực tế, gây hao tổn nguồn lực doanh nghiệp.

**4. Hủy hoại văn hóa cống hiến vì sản phẩm:** Khiến những kỹ sư thực sự quan tâm đến sức khỏe mã nguồn và trải nghiệm người dùng bị mất động lực khi phải lựa chọn giữa "điều tốt cho người dùng" và "điều có ích cho thăng tiến".

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052406.jpg)

Mặc dù vậy, Zach Lloyd thừa nhận đây vẫn là công cụ kích thích hiệu suất nhân viên tốt nhất hiện có. Để khắc phục, ông đề xuất ưu tiên các giá trị lấy người dùng làm trung tâm và tuyển dụng các kỹ sư có triết lý làm việc cống hiến.

Tuy nhiên, tôi cho rằng các giải pháp đó khá mơ hồ. Phương án thực tế hơn là khi quy mô công ty phình to đến mức độ nhất định, doanh nghiệp nên tách nhỏ các phòng ban thành các công ty khởi nghiệp hoạt động độc lập để kích thích tính tự chủ và cạnh tranh lành mạnh. Ở các công ty quy mô nhỏ, lợi ích của cá nhân luôn gắn chặt với sự sinh tồn của công ty, giúp mọi người tập trung vào chất lượng sản phẩm hơn là cấp bậc chức danh.

## 工具软件 FlowUs 体验报告

Tuần này, bản tin xin giới thiệu tới bạn đọc một công cụ quản lý năng suất mới ra mắt mang tên **[FlowUs](https://flowus.cn/login?code=FLOWUS&promotionChannel=WX_RYF_01)** (tên tiếng Trung là "息流").

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051502.webp)

**FlowUs tích hợp 3 tính năng cốt lõi: Soạn thảo văn bản + Bảng dữ liệu + Lưu trữ đám mây.** Dựa trên cấu trúc biên tập dạng khối (block editor), người dùng có thể tự do kéo thả, sắp xếp nội dung để viết ghi chú, quản lý dự án hoặc xây dựng trang wiki chia sẻ thông tin.

FlowUs được thiết kế tối ưu cho thói quen sử dụng của người dùng trong nước với tốc độ tải trang nhanh nhờ hệ thống máy chủ nội địa, hỗ trợ đầy đủ các block liên kết các dịch vụ thông dụng (như video Bilibili, nhạc NetEase Music) và khả năng đồng bộ dữ liệu tức thì giữa các thiết bị:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051620.webp)

FlowUs cung cấp hơn 80 mẫu giao diện (templates) dựng sẵn cho các nhu cầu ghi chép cá nhân hay quản lý công việc. Hệ thống cơ sở dữ liệu bảng hỗ trợ hiển thị dưới nhiều dạng trực quan như Kanban, Calendar, Timeline:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052614.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051903.webp)

Bên cạnh đó, dịch vụ lưu trữ đám mây tích hợp trên FlowUs cho phép tải lên file dung lượng lớn không bị giới hạn tốc độ băng thông, hỗ trợ xem trước trực tiếp các file văn bản Office và file video. Tài khoản miễn phí được cung cấp 2GB dung lượng lưu trữ đĩa.

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052613.webp)

*(Giao diện mẫu trang quản lý file tải về tích hợp trên FlowUs)*

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051816.webp)

FlowUs hiện hỗ trợ đầy đủ phiên bản giao diện Web và ứng dụng di động. Gói tài khoản miễn phí hầu như không giới hạn tính năng (ngoại trừ dung lượng lưu trữ đám mây).

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051814.webp)

Bạn đọc quan tâm có thể quét mã QR phía trên hoặc truy cập [Liên kết đăng ký FlowUs](https://flowus.cn/login?code=FLOWUS&promotionChannel=WX_RYF_01) để trải nghiệm. FlowUs dành tặng 10 tài khoản chuyên nghiệp (Professional Edition) thời hạn 1 năm cho các bạn đọc may mắn tương tác trên kênh công bố bản tin tuần này.

## 科技动态

1、[Mẫu xe thể thao điện tích hợp thiết bị bay không người lái tự động](https://www.theverge.com/2022/3/2/22956775/polestar-o2-electric-roadster-concept-drone)

Hãng xe điện Polestar vừa giới thiệu nguyên mẫu xe thể thao tích hợp thiết bị bay drone độc đáo:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030510.webp)

Khi xe đang di chuyển, người lái chỉ cần nhấn nút kích hoạt để phần cốp sau xe tự động mở rộng, giải phóng một chiếc máy bay không người lái nhỏ tự động cất cánh bay bám theo ghi hình chiếc xe trên hành trình:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030511.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030512.webp)

Sau khi hoàn thành ghi hình, drone sẽ tự động quay trở về khoang chứa phía sau xe. Ý tưởng giúp người dùng dễ dàng ghi lại các thước phim hành trình cá nhân một cách tự động và an toàn:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030513.webp)

2、[Khánh thành tháp truyền tải điện cao thế lớn nhất thế giới vượt sông Trường Giang](https://j.eastday.com/p/1652785311033170)

Dự án xây dựng cặp tháp truyền tải điện cao thế cao nhất thế giới bắc qua sông Trường Giang vừa chính thức hoàn thành kéo cáp tại tỉnh Giang Tô:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051810.webp)

Hai tòa tháp thép được xây dựng ở hai bên bờ sông thuộc địa phận Vô Tích và Thái Châu với chiều cao đạt tới 385 mét (vượt qua chiều cao của tháp Eiffel 61 mét):

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051811.webp)

Cấu trúc tháp được thiết kế siêu cao nhằm đảm bảo các đường dây truyền tải điện vắt qua sông đạt độ cao an toàn tuyệt đối, không gây ảnh hưởng tới luồng di chuyển của các tàu vận tải container tải trọng lớn lưu thông phía dưới sông Trường Giang:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051812.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051813.webp)

3、[Ốp lưng tích hợp vi xử lý hỗ trợ sóng 5G cho điện thoại di động](https://www.ithome.com/0/618/805.htm)

Thị trường trong nước vừa xuất hiện dòng sản phẩm ốp lưng thông minh hỗ trợ kết nối mạng 5G có giá bán 799 NDT:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052307.webp)

Sản phẩm được thiết kế chuyên dụng dành cho các dòng điện thoại 4G của Huawei (vốn bị cấm vận không thể tiếp cận chip thu phát sóng 5G). Ốp lưng nặng khoảng 52g, được trang bị chip xử lý thu phát sóng riêng và kết nối với điện thoại qua cổng giao tiếp vật lý, hỗ trợ đồng bộ sóng 5G thông qua dịch vụ eSIM của nhà mạng:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052308.webp)

4、[Dự án xây dựng nhà để xe tự động dạng tháp ngầm dưới lòng đất](https://www.163.com/dy/article/H5QOEJPF0514ETGI.html)

Thành phố Hàng Châu chuẩn bị đưa vào vận hành khu nhà để xe tự động thông minh có kiến trúc độc đáo tích hợp dưới một công viên công cộng:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052309.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052310.webp)

Khu đỗ xe bao gồm hệ thống 10 tháp để xe hình trụ tròn xây dựng chìm dưới lòng đất. Người lái chỉ cần đỗ xe tại các khu vực cổng vào ở tầng hầm, hệ thống robot tự động sẽ di chuyển và phân bổ xe vào các khoang chứa bên trong tháp một cách tối ưu diện tích:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052314.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052313.webp)

Giải pháp giúp giải quyết bài toán thiếu hụt chỗ đỗ xe tại các khu đô thị đông dân cư mà không làm ảnh hưởng tới không gian xanh cảnh quan phía trên mặt đất:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052316.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052317.webp)

5、[Mẫu xe đạp chống trộm thiết kế khung xe gập làm khóa bảo vệ](https://robbreport.com/motors/motorcycles/yerka-v3-theft-proof-bike-integrated-lock-1234665378/)

Nhu cầu sử dụng xe đạp tăng cao đi kèm với rủi ro mất trộm xe gia tăng khi kẻ trộm dễ dàng dùng kìm cộng lực cắt đứt các xích khóa thông thường. Hãng Yerka (Mỹ) đã giới thiệu dòng xe đạp chống trộm Yerka V3:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030802.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030803.webp)

Phần gióng khung dưới của xe được thiết kế khớp nối cho phép tháo rời và gập ngang kết hợp với cọc yên xe để khóa chặt vào cột điện bên đường. Nếu kẻ trộm cố tình cưa cắt gióng khung xe để lấy trộm, kết cấu chịu lực của xe sẽ bị phá hủy hoàn toàn khiến chiếc xe trở nên vô giá trị không thể sử dụng hay bán lại được:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030804.webp)

## 文章

1、[Lập trình viên sử dụng hệ thống 50 card đồ họa 1080Ti hỗ trợ nghiên cứu điều trị ung thư](https://www.toutiao.com/article/7094940100450107935/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052108.webp)

Tác giả chia sẻ câu chuyện ý nghĩa của một lập trình viên tự bỏ tiền túi đầu tư hệ thống 50 card đồ họa cũ để tự huấn luyện các mô hình AI nhận diện tế bào ung thư vú giai đoạn đầu từ ảnh chụp X-quang, và định hướng phát triển mô hình hỗ trợ chẩn đoán u não.

2、[Ký sự hành trình đo đạc chiều cao cây cổ thụ thông Bhutan kỷ lục tại Tây Tạng](https://mp.weixin.qq.com/s/UHAnsrvzu-Hc9orfICwv3Q)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052109.webp)

Bài phóng sự chi tiết ghi lại quá trình đội ngũ khảo sát lâm nghiệp đi sâu vào khu bảo tồn thiên nhiên huyện Mê Thoát để định vị và sử dụng thiết bị quét laser đo đạc chiều cao thực tế của cây bách thông Bhutan đạt chiều cao kỷ lục 76,8 mét.

3、[GitHub chính thức hỗ trợ kết xuất công thức toán học LaTeX trong file Markdown](https://github.blog/changelog/2022-05-19-render-mathematical-expressions-in-markdown/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052105.webp)

GitHub công bố tính năng được nhiều nhà nghiên cứu mong đợi: hỗ trợ kết xuất trực tiếp các công thức toán học viết bằng cú pháp LaTeX bên trong các tệp tin Markdown trên repo thông qua thư viện kết xuất MathJax.

4、[Mẹo tìm kiếm vị trí địa lý chụp ảnh thực tế dựa trên các chi tiết ảnh](https://sspai.com/post/73193)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051703.webp)

Bài viết hướng dẫn các phương pháp phân tích góc bóng đổ Mặt Trời, biển báo giao thông và kiến trúc nhà cửa xung quanh để xác định chính xác tọa độ địa lý chụp của một bức ảnh ngẫu nhiên trên mạng.

5、[Hình ảnh bên trong dự án xây dựng lò phản ứng hạt nhân fusion lớn nhất thế giới](https://www.sciencefocus.com/future-technology/nuclear-fusion-inside-the-construction-of-the-worlds-largest-tokamak/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032901.webp)

Phóng sự ảnh ghi nhận tiến độ thi công thực tế tại miền Nam nước Pháp của lò phản ứng hạt nhân hạt nhân nhiệt hạch Tokamak (dự án ITER) có sự tham gia đóng góp công nghệ của hơn 32 quốc gia hướng tới nguồn năng lượng vô hạn cho tương lai.

6、[Cảnh báo phương thức tấn công giả mạo giao diện đăng nhập popup trình duyệt](https://mrd0x.com/browser-in-the-browser-phishing-attack/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031913.webp)

Bài phân tích kỹ thuật về hình thức tấn công lừa đảo nguy hiểm: trang web độc hại tự dựng một cửa sổ đăng nhập giả lập bằng mã HTML/CSS giống hệt cửa sổ đăng nhập tài khoản Google/Facebook của trình duyệt để đánh cắp thông tin tài khoản của người dùng mất cảnh giác.

7、[Hướng dẫn sử dụng thẻ HTML5 `<dialog>` thay thế các hộp thoại JavaScript](https://css-tricks.com/replace-javascript-dialogs-html-dialog-element/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032201.webp)

Bài viết hướng dẫn lập trình viên Front-end ứng dụng thẻ `<dialog>` mặc định của HTML5 để thiết lập các hộp thoại xác nhận, cảnh báo đẹp mắt thay thế cho các hàm chặn luồng UI truyền thống của trình duyệt như `alert()`, `confirm()`.

8、[Đánh giá sự kiện Google I/O 2022 dưới góc nhìn sản phẩm](https://arstechnica.com/gadgets/2022/05/googles-past-failures-were-on-full-display-at-i-o-2022/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052402.webp)

Bài viết đưa ra góc nhìn phản biện cho rằng sự kiện Google I/O năm nay thiếu đi các đột phá công nghệ mới, chủ yếu tập trung cải tiến lại các dự án phần cứng từng gặp nhiều khó khăn trước đây như kính thông minh Google Glass hay hệ điều hành cho máy tính bảng.

## 工具

1、[Yaade: Công cụ quản lý và kiểm thử API nguồn mở](https://github.com/EsperoTech/yaade)

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040304.webp)

Dự án phát triển công cụ gọi thử nghiệm API tự host (self-hosted API client) gọn nhẹ chạy trên nền tảng web làm giải pháp thay thế mã nguồn mở cho Postman.

2、[Regolith Linux: Bản phân phối Linux tích hợp sẵn i3 window manager](https://regolith-linux.org/)

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040406.webp)

Hệ điều hành xây dựng trên nền tảng Ubuntu kết hợp giao diện quản lý cửa sổ dạng i3 tiling window manager tối giản và tiết kiệm tài nguyên RAM cho các kỹ sư lập trình.

3、[Google Chinese Results Blocklist: Bộ lọc trang web rác tiếng Trung trên kết quả tìm kiếm](https://github.com/cobaltdisco/Google-Chinese-Results-Blocklist)

Danh sách cấu hình mở rộng cho extension uBlacklist giúp tự động lọc bỏ các trang web sao chép nội dung, trang web rác kém chất lượng khỏi kết quả tìm kiếm tiếng Trung trên Google. (Đóng góp của [@52fhy](https://github.com/ruanyf/weekly/issues/2409))

4、[NocoBase: Nền tảng xây dựng ứng dụng cộng tác no-code nguồn mở](https://www.nocobase.com/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052507.webp)

Công cụ hỗ trợ doanh nghiệp tự thiết lập nhanh các trang quản trị dữ liệu, hệ thống CMS nội bộ chỉ thông qua các thao tác kéo thả giao diện trực quan không cần viết code. (Đóng góp của [@zhouyanliang](https://github.com/ruanyf/weekly/issues/2416))

5、[StickyNote: Tiện ích ghi chú dán màn hình cải tiến cho Windows](http://cppdebug.com/archives/286)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052508.webp)

Công cụ ghi chú nhỏ gọn chạy trên Windows bổ sung các tính năng định dạng văn bản, sao lưu dữ liệu đám mây tiện lợi dựa trên app Sticky Notes mặc định của Win10. (Đóng góp của [@KeyboardMan1996](https://github.com/ruanyf/weekly/issues/2417))

6、[pnpm: Bộ quản lý gói Node.js hiệu năng cao tiết kiệm dung lượng đĩa](https://pnpm.io/zh/)

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040604.webp)

Tiện ích quản lý gói npm thế hệ mới sử dụng cơ chế lưu trữ thư viện tập trung và liên kết cứng (hard links) trong dự án giúp tối ưu hóa đáng kể tốc độ cài đặt và tiết kiệm dung lượng đĩa cứng.

7、[CRX Viewer: Xem trực tiếp mã nguồn tiện ích mở rộng Chrome](https://github.com/Rob--W/crxviewer)

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040614.webp)

Extension trình duyệt hỗ trợ nhà phát triển phân tích xem nhanh cấu trúc thư mục và nội dung code JavaScript bên trong của bất kỳ tiện ích mở rộng nào trên cửa hàng Chrome Web Store.

8、[Gephi: Phần mềm trực quan hóa đồ thị mạng lưới dữ liệu chuyên nghiệp](https://gephi.org/)

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040704.webp)

Ứng dụng đa nền tảng hỗ trợ các nhà phân tích dữ liệu vẽ sơ đồ liên kết, biểu diễn mối quan hệ của các thực thể dữ liệu phức tạp dưới dạng đồ thị trực quan.

9、[Rust Coreutils: Viết lại các dòng lệnh cốt lõi của Linux bằng ngôn ngữ Rust](https://github.com/uutils/coreutils)

Dự án nguồn mở hướng tới mục tiêu dùng ngôn ngữ Rust viết lại toàn bộ các công cụ dòng lệnh cơ bản của hệ thống Unix (ls, cp, rm, mv) để thay thế cho bộ GNU Coreutils viết bằng C nhằm tăng độ an toàn bộ nhớ.

## 资源

1、[Cloud Native & DevOps Interview Guide (Bộ câu hỏi phỏng vấn tuyển dụng)](https://geekbang.org/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052612.webp)

Bộ tài liệu cẩm nang ôn tập dày 80 trang tổng hợp hơn 198 câu hỏi phỏng vấn thực tế tại các hãng lớn xoay quanh kiến thức vận hành hệ thống container Docker, Kubernetes và quy trình CI/CD. Độc giả quan tâm có thể quét mã QR phía trên để nhận miễn phí.

2、[Webcamtaxi: Tổng hợp các kênh camera phát trực tuyến công cộng toàn cầu](https://www.webcamtaxi.com/en/)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033115.webp)

Trang web tổng hợp liên kết của hàng ngàn camera giám sát giao thông và cảnh quan thành phố phát trực tuyến 24/7 trên YouTube từ nhiều quốc gia.

3、[Side Project Guide: Cuốn sách chia sẻ kinh nghiệm phát triển sản phẩm cá nhân](https://sideproject.guide/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052503.webp)

Bộ tài liệu chia sẻ kinh nghiệm thực tế về cách tìm kiếm ý tưởng, phát triển tính năng tối giản và tìm kiếm mô hình doanh thu cho các dự án phần mềm cá nhân (side projects). (Đóng góp của [@timqian](https://github.com/ruanyf/weekly/issues/2405))

4、[Jest Tutorial: Giáo trình thực hành viết mã kiểm thử Front-end](http://github.yanhaixiang.com/jest-tutorial/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052504.webp)

Giáo trình tiếng Trung hướng dẫn lập trình viên cách viết mã unit test giao diện UI, chạy mô phỏng hành vi người dùng sử dụng thư viện kiểm thử Jest. (Đóng góp của [@haixiangyan](https://github.com/ruanyf/weekly/issues/2407))

5、[Java Notes for Professionals (Sách học lập trình Java tổng hợp từ StackOverflow)](https://books.goalkicker.com/JavaBook/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052505.webp)

Cuốn sách biên soạn miễn phí hệ thống hóa các chủ đề lập trình Java cơ bản và nâng cao dựa trên các câu hỏi và câu trả lời chất lượng nhất của cộng đồng StackOverflow. (Đóng góp của [@52fhy](https://github.com/ruanyf/weekly/issues/2410))

6、[Intel Virtual Museum: Chuyên trang tham quan bảo tàng công nghệ ảo Intel](https://virtualmuseum.intel.com/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052506.webp)

Trang web tương tác 3D cho phép người dùng tham quan trực tuyến không gian bảo tàng trưng bày lịch sử các thế hệ chip vi xử lý của tập đoàn Intel. (Đóng góp của [@Codeniu](https://github.com/ruanyf/weekly/issues/2411))

## 图片

1\. [Phong cách thiết kế giao diện đồ họa GUI của phần mềm thế kỷ trước](https://twitter.com/Nexuist/status/1486466541491261443)

Hình ảnh minh họa phong cách thiết kế giao diện đồ họa nhồi nhét nhiều thanh công cụ và nút bấm cơ học đặc trưng của các phần mềm máy tính thời kỳ đầu những năm 90:

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020803.webp)

Sự phát triển của tư duy thiết kế UX trong 20 năm qua đã giúp tinh giản hóa giao diện người dùng trở nên trực quan và dễ sử dụng hơn rất nhiều.

2\. **Sự phân chia các dòng thương hiệu dịch vụ tài chính của Apple**

Apple hiện đang vận hành 4 thương hiệu con phục vụ cho mảng thanh toán và ví điện tử:

- **Apple Wallet:** Ứng dụng ví lưu trữ thẻ ngân hàng, vé máy bay.
- **Apple Pay:** Giải pháp bảo mật thanh toán không chạm qua NFC.
- **Apple Card:** Dòng thẻ tín dụng liên kết ngân hàng phát hành cho người dùng.
- **Apple Cash:** Dịch vụ nạp tiền và chuyển tiền nhanh giữa các tài khoản.

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052609.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052608.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052607.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052606.webp)

Việc phân tách một tính năng thanh toán cốt lõi thành 4 thương hiệu độc lập đôi khi gây bối rối cho người dùng phổ thông khi phải phân biệt cách thức hoạt động của từng dịch vụ.

3\. **Thống kê chuỗi cung ứng sản xuất và tinh chế khoáng sản cho pin Lithium**

Biểu đồ thống kê các quốc gia khai thác quặng thô cobalt, lithium chủ chốt trên thế giới (với Cộng hòa Dân chủ Congo chiếm ưu thế về cobalt):

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052604.webp)

Biểu đồ thống kê các quốc gia nắm giữ thị phần tinh chế và gia công thành phẩm kim loại cobalt, lithium phục vụ lắp ráp pin (với Trung Quốc chiếm thị phần áp đảo):

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052605.webp)

## ✍️ Bài đọc thêm

### Giai thoại về góc nhìn đèn giao thông của trẻ nhỏ

Một câu chuyện ngụ ngôn nhỏ mang lại bài học ý nghĩa về kỹ năng quản lý và làm việc nhóm:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052610.webp)

Tôi chở cậu con trai 3 tuổi Ben dừng xe chờ đèn đỏ tại ngã tư. Để thử trí thông minh của con, tôi hỏi: *"Ben, đèn giao thông đang là màu gì thế con?"*. Cậu bé trả lời: *"Màu xanh lá cây bố ạ"*. 

Tôi chỉ tay vào biển dừng và bảo con quan sát kỹ lại xem, nhưng cậu bé vẫn khẳng định là màu xanh. Một lát sau khi đèn tín hiệu chuyển làn, cậu bé lại bảo: *"Đèn đỏ rồi bố ơi, chúng ta đi thôi"*.

Lúc đó tôi vô cùng lo lắng nghĩ con mình bị tật khúc xạ màu sắc. Tuy nhiên khi về nhà kiểm tra bằng bảng màu vẽ, cậu bé phân biệt các màu đỏ, xanh hoàn toàn chính xác.

Ba tuần sau đó trong một chuyến đi chơi gia đình, tôi ngồi ở hàng ghế sau ngay cạnh ghế an toàn của Ben. Khi xe dừng chờ đèn đỏ tại ngã tư, tôi hướng mắt theo góc nhìn của con và lập tức hiểu ra vấn đề: do tầm vóc thấp và bị vướng tựa lưng ghế lái phía trước, Ben hoàn toàn không nhìn thấy cụm đèn tín hiệu chính diện của xe. Cậu bé đang quan sát cụm đèn tín hiệu dành cho làn đường cắt ngang bên cạnh (vốn luôn hiển thị màu sắc ngược lại với làn chính).

Bài học đúc kết từ câu chuyện: **Vị trí đứng của bạn sẽ quyết định góc nhìn và giới hạn tầm quan sát của bạn.** Khi đứng ở vị trí vận hành trực tiếp, bạn sẽ quan sát thấy những thách thức thực tế mà những người đứng ngoài hoặc ngồi ở hàng ghế sau không thể nhận thấy. Hãy kiên định với định hướng thực tế của mình và bỏ qua các ý kiến nhận định thiếu căn cứ thực tiễn từ những người không ở cùng vị trí.

## 历史上的本周

- 2021年（第 160 期）：[Thảo luận thực tế: Góc nhìn về khủng hoảng tuổi trung niên của lập trình viên thế hệ trước](https://www.ruanyifeng.com/blog/2021/05/weekly-issue-160.html)
- 2020年（第 109 期）：[Phân tích xu hướng phát triển và giá trị truyền tải tri thức của định dạng âm thanh Podcast](https://www.ruanyifeng.com/blog/2020/05/weekly-issue-109.html)
- 2019年（第 57 期）：[Thảo luận triết học: Hành vi tự nguyện chia sẻ tri thức miễn phí có trái với bản năng tư lợi của con người?](https://www.ruanyifeng.com/blog/2019/05/weekly-issue-57.html)
- 2018年（第 6 期）：[Nhìn nhận thực tế: Trong kỷ nguyên phát triển của AI dịch thuật, liệu học sinh có cần nỗ lực học ngoại ngữ?](https://www.ruanyifeng.com/blog/2018/05/weekly-issue-6.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
