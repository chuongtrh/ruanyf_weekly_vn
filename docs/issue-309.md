# Bản tin chia sẻ công nghệ (Số 309): Con dao hai lưỡi của xe taxi không người lái

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/4743) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071817.webp)

Tại thôn Tân Xuân, thành phố Tất Tiết, tỉnh Quý Châu, một sân bóng rổ lung linh ánh đèn đã được xây dựng ngay bên trong một hang động tự nhiên. Giải pháp này vừa giúp tiết kiệm đất canh tác, vừa có thể che mưa che gió, mùa đông ấm áp, mùa hè mát mẻ. (Nguồn: [163.com](https://www.163.com/dy/article/HSDF54N90553BF7G.html))

## 无人驾驶出租车的双面刃

Dịch vụ [xe taxi không người lái tại Vũ Hán](https://finance.sina.cn/chanjing/gdxw/2024-07-08/detail-inccpaqm8845132.d.html) đang là một chủ đề tin tức vô cùng nóng hổi thời gian gần đây.

Hàng trăm chiếc xe taxi của công ty "Apollo Go" (萝卜快跑) hoàn toàn không có tài xế ngồi sau vô lăng đang ngày đêm đưa đón hành khách trên các đường phố Vũ Hán (chủ yếu tập trung tại Khu phát triển công nghệ mới Đông Hồ).

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071414.webp)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071413.webp)

Tất cả chúng ta đều từng nghĩ rằng, một ngày nào đó công nghệ tự lái sẽ trở thành hiện thực và thay thế hoàn toàn tài xế con người, nhưng không ai ngờ rằng ngày đó lại đến nhanh như vậy.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071415.webp)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071416.webp)

Tuy nhiên, ở thời điểm hiện tại, đây chưa phải là công nghệ tự lái hoàn toàn độc lập tuyệt đối. Nhiều hình ảnh chia sẻ trên mạng cho thấy, mỗi chiếc xe đều được giám sát thời gian thực bởi các kỹ thuật viên thông qua hệ thống đám mây, sẵn sàng tiếp quản quyền điều khiển từ xa trong các tình huống khẩn cấp.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071417.webp)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071703.webp)

Theo các nguồn tin [báo chí](https://www.sohu.com/a/792584536_120046696), Apollo Go hiện đang vận hành tại 12 thành phố (Thượng Hải, Phúc Châu, Gia Hưng, Dương Tuyền, Trùng Khánh, Thành Đô, Bắc Kinh, Hợp Phì, Quảng Châu, Trường Sa, Vũ Hán và Thâm Quyến). Trong đó, có 4 thành phố cho phép xe hoàn toàn không có người bên trong (Bắc Kinh, Thượng Hải, Thâm Quyến, Vũ Hán), các thành phố còn lại vẫn yêu cầu có nhân viên an toàn ngồi ở ghế lái.

Tuy nhiên, Vũ Hán là thành phố duy nhất cho phép vận hành không người lái trên toàn phạm vi thành phố 24/7, trong khi các thành phố khác chỉ giới hạn hoạt động trong các khu vực và khung giờ quy định.

Đó là lý do vì sao làn sóng xe tự lái lại bùng nổ mạnh mẽ đầu tiên tại Vũ Hán. Bởi vì **đây là đô thị duy nhất tại Trung Quốc thực sự đưa công nghệ tự lái vào đời sống một cách toàn diện ở thời điểm hiện tại.**

Chính sách của thành phố Vũ Hán là cởi mở nhất. Ngay từ năm 2022, chính quyền đã ban hành quy định "Ba cho phép": Cho phép không cần nhân viên an toàn trong xe, cho phép chạy trên các tuyến đường giao thông công cộng, và cho phép thương mại hóa dịch vụ. Diện tích khu vực mở cửa cho xe tự lái tại Vũ Hán được cho là lớn nhất thế giới.

Tuy nhiên, lợi thế đi đầu này có lẽ sẽ không kéo dài được lâu. Sau thành công vang dội của Apollo Go tại Vũ Hán, các thành phố khác đang nhanh chóng nhập cuộc. Vào ngày 8 tháng 7, [Thượng Hải](https://www.sohu.com/a/792024596_121124483) đã lập tức tuyên bố cho phép xe tự lái không cần nhân viên an toàn, và dự kiến sẽ mở cửa thử nghiệm dịch vụ taxi tự lái cho công chúng trong vòng một tuần.

Chính phủ Trung Quốc cũng thể hiện sự ủng hộ rõ ràng đối với hướng đi này, và thúc đẩy chiến lược [“Tích hợp Xe - Đường - Đám mây”](https://app.xinhuanet.com/news/article.html?articleId=7fc13d1cf5732d55fce0836701d02a90) làm định hướng phát triển quốc gia. Chính quyền thành phố Bắc Kinh thậm chí đã [ban hành văn bản quy định](https://new.qq.com/rain/a/20240630A06XHY00): Từ nay về sau, các dự án xây mới, cải tạo, mở rộng đường bộ đều phải chừa không gian hai bên đường để lắp đặt hạ tầng thông minh.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071418.webp)

Tóm lại: **Công nghệ tự lái không còn là nghiên cứu trong phòng thí nghiệm nữa, kỷ nguyên thử nghiệm diện rộng và ứng dụng quy mô lớn trên toàn quốc đang chuẩn bị gõ cửa.**

Xét trên góc độ tích cực, tôi tin rằng đây là một bước đi đúng đắn: (1) Xe tự lái thúc đẩy quá trình nâng cấp và chuyển dịch cơ cấu ngành công nghiệp; (2) Nâng cao năng lực cạnh tranh quốc gia, bảo toàn lợi thế cạnh tranh của đất nước trong các ngành chế tạo ô tô, vận tải và phần mềm; (3) Mang lại nhiều lợi ích thiết thực cho người tiêu dùng.

Tuy nhiên, công nghệ tự lái cũng mang lại những tác động tiêu cực, gây tổn thương cho xã hội. Đó là **nó sẽ thay thế tài xế con người, dẫn đến làn sóng thất nghiệp**. Đây là một thực tế không thể phớt lờ.

Xe tự lái có giá cước vô cùng rẻ, hoạt động liên tục 24 giờ không nghỉ, tài xế truyền thống hoàn toàn không có cửa cạnh tranh. Dịch vụ Apollo Go tại Vũ Hán có giá cước chưa đầy 1 tệ cho mỗi km, thấp hơn nhiều so với xe công nghệ (ride-hailing) truyền thống, và càng rẻ hơn so với xe taxi truyền thống. (Tại Vũ Hán, giá mở cửa xe taxi là 10 tệ cho 3 km đầu tiên, sau đó là 1.8 tệ/km).

Các hãng xe taxi tại Vũ Hán hiện đã rơi vào tình cảnh kiệt quệ. Trên mạng xã hội đang lan truyền một bức [thư ngỏ](https://h5.ifeng.com/c/vivoArticle/v002lY-_1e8oWIXJ92Qtx7OqvmieIzXPWmvUapr5VFNKP82U__?isNews=1&showComments=0) kêu cứu của Công ty Vận tải Hành khách Ô tô Vũ Hán:

"Hiện tại, thu nhập gộp hàng ngày của mỗi tài xế trong công ty chúng tôi chỉ dao động từ 200 đến 300 tệ, thực sự là muối bỏ bể, không thể duy trì cuộc sống.

由此引发驾驶员与公司之间的矛盾，司机群里每天抱怨公司和管理部门不作为。

特别是在这一段无人驾驶网络车的流行，**科技垄断资源，抢夺底层人的饭碗**，许多巡游出租车养家糊口困难，被逼退出这个行业。"

Thất nghiệp là một vấn đề xã hội vô cùng nghiêm trọng. Nếu xe taxi tự lái thay thế tài xế con người trên quy mô lớn, sinh kế của rất nhiều gia đình sẽ bị lung lay. Để đảm bảo ổn định xã hội, **chính phủ cần phải áp đặt các biện pháp kiểm soát và hạn chế đối với dịch vụ xe tự lái**.

Tôi xin đưa ra một vài kiến nghị như sau:

（1）Ưu tiên vận tải hàng hóa hơn vận tải hành khách. Các tuyến vận tải hàng hóa đường dài vô cùng gian khổ, phù hợp hơn cho công nghệ tự lái đảm nhận.

（2）Ưu tiên xe buýt công cộng hơn xe taxi. Ngành xe buýt vốn luôn đối mặt với tình trạng thiếu hụt tài xế, xe buýt tự lái có thể giúp tăng tần suất chuyến, thúc đẩy xu hướng di chuyển xanh.

（3）Ưu tiên khu vực ngoại thành và nông thôn hơn khu vực nội đô. Những vùng này vốn khó gọi xe truyền thống, nhu cầu sử dụng xe tự lái là thiết thực hơn.

（4）Đối với dịch vụ taxi tự lái trong nội đô, chính phủ nên thu phí quản lý để đưa mức giá cước tương đương với tài xế con người. Nguồn thu này sẽ được dùng để hỗ trợ chuyển đổi nghề nghiệp cho các tài xế taxi truyền thống.

## 科技动态

1、[Vỏ ốp biến Apple Watch thành máy nghe nhạc di động](https://thetinypod.com/)

Ngoài việc đeo trên cổ tay, đồng hồ thông minh còn có thể làm được gì khác?

Một công ty khởi nghiệp của Mỹ đã nảy ra ý tưởng vô cùng độc đáo khi thiết kế chiếc vỏ ốp chuyên dụng dành riêng cho Apple Watch.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071807.webp)

Chiếc vỏ ốp này mô phỏng thiết kế huyền thoại của máy nghe nhạc iPod, tích hợp hệ thống phím bấm vật lý và vòng xoay điều khiển.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071810.webp)

Nó đã biến chiếc đồng hồ thông minh thành một thiết bị cầm tay nhỏ gọn vô cùng tiện lợi.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071808.webp)

Nhiều người dùng thường xuyên phàn nàn rằng điện thoại thông minh ngày nay quá cồng kềnh, họ chỉ muốn một thiết bị phụ trợ nhỏ gọn để xem giờ, nghe nhạc, kiểm tra thời tiết, nhận cuộc gọi và tin nhắn nhanh. Sản phẩm này rõ ràng đã đáp ứng hoàn hảo nhu cầu đó.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071809.webp)

2、[Hệ thống tuabin gió hai đầu cánh quạt thế hệ mới](https://new.qq.com/rain/a/20240716A02WBD00)

Trong tháng này, Quảng Châu đã hoàn thành xây dựng tuabin gió hai đầu cánh quạt đầu tiên trên thế giới.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071811.webp)

Khác biệt hoàn toàn với các tuabin gió truyền thống chỉ sở hữu một cụm cánh quạt quay, thiết kế mới này tích hợp hai cụm cánh quạt đặt đối xứng.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071812.webp)

Hai cụm cánh quạt này quay theo hai chiều ngược nhau, giúp triệt tiêu momen xoắn tác động lên cột trụ, mang lại độ ổn định kết cấu vượt trội.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071813.webp)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071814.webp)

Ưu điểm trực tiếp của thiết kế này là giúp tuabin chống chịu được các cơn bão cấp 5 (sức gió lên tới 260 km/h) và những cột sóng biển cao tới 30 mét. Đồng thời, sản lượng điện năng tạo ra cũng vượt trội hơn rõ rệt.

3、[Ứng dụng mới đầy tính nhân văn của công nghệ giọng nói AI](https://people.com/congresswoman-shares-new-ai-voice-that-mimics-her-speech-8676408)

Một nữ nghị sĩ Mỹ không may mắc chứng bệnh thần kinh não bộ dẫn đến mất hoàn toàn khả năng nói.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071411.webp)

Bà đã nghĩ ra giải pháp thu thập toàn bộ các file ghi âm giọng nói trước đây của mình để huấn luyện một mô hình AI, giúp tái tạo lại giọng nói cá nhân.

Gần đây, bà đã chia sẻ một đoạn video trên mạng xã hội. Mặc dù bản thân bà không thể phát ra tiếng nói, nhưng mô hình AI đã sử dụng chính chất giọng quen thuộc của bà để phát biểu gửi lời cảm ơn đến những người ủng hộ.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071412.webp)

Đối với những người không may bị mất đi giọng nói, công nghệ sao chép giọng nói bằng AI là một giải pháp vô cùng tuyệt vời, giúp họ tiếp tục giao tiếp với thế giới bằng chính chất giọng của mình.

Điểm hạn chế duy nhất hiện tại là mô hình bắt buộc phải xử lý dữ liệu từ văn bản chuẩn bị trước, chưa thể hỗ trợ giao tiếp tương tác thời gian thực.

4、[Tư thế vỗ tay cho âm thanh lớn nhất](https://physicsworld.com/a/the-physics-of-hand-clapping-heres-how-to-do-it-best/)

Vỗ tay là hành động quen thuộc của tất cả mọi người, nhưng liệu các tư thế vỗ tay khác nhau có mang lại sự khác biệt nào không?

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090107.webp)

Các nhà nghiên cứu tại Đại học Kỹ thuật Crete, Hy Lạp đã tiến hành phân tích các tư thế vỗ tay khác nhau (hình trên). Họ phát hiện ra rằng, khi hai bàn tay đặt lệch nhau một góc 45 độ và lòng bàn tay chồng lên nhau một phần (tư thế A2 trong hình), âm thanh phát ra sẽ có cường độ lớn nhất, đạt mức 85,2 dB.

Ngoài ra, nếu hai bàn tay đặt lệch 45 độ nhưng lòng bàn tay khum lại tạo thành một khoảng trống nhỏ ở giữa (tư thế A1+), âm thanh phát ra sẽ có tần số trầm nhất.

## Bài viết

1\. [Xây dựng trang web loại bỏ hoàn toàn thông báo lỗi 404](https://pillser.com/engineering/2024-06-10-website-without-404s)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061507.webp)

Bài viết chia sẻ một thủ thuật lập trình đơn giản giúp truy vấn cơ sở dữ liệu để tìm ra đường dẫn gần giống nhất với địa chỉ người dùng nhập sai, từ đó tự động chuyển hướng và xóa bỏ hoàn toàn lỗi 404.

2\. [Ứng dụng JavaScript để phát hiện trạng thái phím Caps Lock](https://davidwalsh.name/detect-caps-lock)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061510.webp)

Rất nhiều người dùng gặp lỗi nhập sai mật khẩu do vô tình bật phím Caps Lock. Bài viết hướng dẫn cách viết mã JavaScript đơn giản để cảnh báo người dùng khi phím này đang được bật.

3\. [Kiến trúc hạ tầng vận hành dịch vụ SaaS cho mô hình công ty một thành viên](https://anthonynsimon.com/blog/one-man-saas-architecture/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061701.webp)

Bài viết chi tiết từ năm 2021 chia sẻ kinh nghiệm của tác giả trong việc thiết lập và vận hành hệ thống hạ tầng kỹ thuật để một lập trình viên duy nhất có thể duy trì dịch vụ SaaS ổn định.

4\. [Hướng dẫn thiết lập hệ thống bẫy bảo mật SSH Honeypot](https://blog.sofiane.cc/setup_ssh_honeypot/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061801.webp)

Bài viết hướng dẫn cách triển khai công cụ bẫy bảo mật Cowrie để ghi lại các hành vi xâm nhập trái phép của hacker qua cổng SSH, các phương pháp phân tích sâu hơn được trình bày trong [bài viết tiếp theo](https://blog.sofiane.cc/ssh_honeypot/).

5\. [Nhận định kỹ thuật: Mock Testing thực chất là một phản mẫu thiết kế](https://www.amazingcto.com/mocking-is-an-antipattern-how-to-test-without-mocking/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061802.webp)

Tác giả đưa ra góc nhìn phản đối việc lạm dụng cơ chế mock để giả lập các điều kiện ngoại cảnh trong quy trình kiểm thử phần mềm, đồng thời đề xuất các giải pháp thay thế hiệu quả hơn.

## 工具

1\. [Floating Whiteboard (Bảng vẽ tương tác trực tuyến trực quan)](https://floating-hands-whiteboard.vercel.app/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071301.webp)

Một công cụ bảng vẽ whiteboard trực tuyến chạy trực tiếp trên trình duyệt.

2\. [Ditto (Hệ thống mạng xã hội phi tập trung xây dựng trên Nostr)](https://soapbox.pub/ditto/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071407.webp)

Dự án mã nguồn mở hỗ trợ người dùng tự triển khai mạng xã hội tương tự Twitter dựa trên giao thức Nostr. Điểm ưu việt là tài khoản người dùng được định danh bằng cặp khóa mật mã độc quyền, không chịu sự kiểm soát của bất kỳ máy chủ trung tâm nào.

3\. [MathLive (Thành phần giao diện hỗ trợ nhập công thức toán học trên web)](https://github.com/arnog/mathlive)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071409.webp)

Một thư viện Web Component chuyên dụng hỗ trợ người dùng soạn thảo công thức toán học trực quan trên trang web. (Đóng góp của [@shlroland](https://github.com/ruanyf/weekly/issues/4814))

4\. [fideo (Công cụ hỗ trợ tự động ghi hình luồng livestream đa nền tảng)](https://github.com/chenfan0/fideo-live-record/blob/main/README-CN.md)

Ứng dụng máy tính đa nền tảng hỗ trợ tự động ghi lại nội dung các phòng livestream của nhiều nền tảng lớn trong và ngoài nước. (Đóng góp của [@chenfan0](https://github.com/ruanyf/weekly/issues/4827))

5\. [Oceanbase (Hệ quản trị cơ sở dữ liệu quan hệ mã nguồn mở của Ant Group)](https://github.com/oceanbase/oceanbase/blob/develop/README_CN.md)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071802.webp)

Dự án cơ sở dữ liệu quan hệ mã nguồn mở do Ant Group tự phát triển, định hướng làm giải pháp thay thế mạnh mẽ cho MySQL. (Đóng góp của [@liboyang0730](https://github.com/ruanyf/weekly/issues/4836))

6\. [Shell360 (Ứng dụng quản lý kết nối SSH đa nền tảng)](https://github.com/shell360/release)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071806.webp)

Ứng dụng khách SSH đa nền tảng hỗ trợ chạy trên Windows, Linux, macOS, iOS và Android. (Đóng góp của [@nashaofu](https://github.com/ruanyf/weekly/issues/4847))

7\. [Simple Pastebin (Mẫu thiết kế trang lưu trữ văn bản nhanh tối giản)](https://github.com/yuxiaoy1/simple-pastebin)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071801.webp)

Một dự án trang pastebin đơn giản xây dựng trên nền tảng Flask phục vụ mục đích học tập. (Đóng góp của [@yuxiaoy1](https://github.com/ruanyf/weekly/issues/4828))

8\. [Lima (Hệ thống máy ảo Linux gọn nhẹ dành cho macOS)](https://lima-vm.io/)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071101.webp)

Giải pháp tạo máy ảo Linux tối giản trên macOS giúp chạy các ứng dụng Linux mượt mà. Bạn đọc có thể tham khảo thêm [Colima](https://github.com/abiosoft/colima) - một dự án phát triển dựa trên Lima chuyên dùng để chạy Docker trên Mac.

9\. [progress (Công cụ hiển thị thanh tiến trình cho các lệnh dòng lệnh Linux)](https://github.com/Xfennec/progress)

Tiện ích terminal giúp hiển thị thanh tiến trình trực quan khi người dùng thực thi các lệnh sao chép hay di chuyển dữ liệu lớn như `cp`, `mv`, `dd`...

10\. [yt-fts (Công cụ tìm kiếm thông tin trong phụ đề kênh YouTube)](https://github.com/NotJoeMartinez/yt-fts)

Thư viện viết bằng Python hỗ trợ tải toàn bộ tệp phụ đề của một kênh YouTube chỉ định để xây dựng công cụ tìm kiếm toàn văn (full-text search).

11\. [VanJS (Thư viện JavaScript xây dựng giao diện tối giản tối đa)](https://vanjs.org/)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052003.webp)

Thư viện JavaScript có tư tưởng thiết kế tương tự React nhưng được rút gọn tối đa, tổng dung lượng file nén chỉ nặng vỏn vẹn 1.2 KB.

## AI 相关

1\. [WordSea (Trang từ điển tiếng Anh minh họa bằng hình ảnh AI)](https://wordsea.xyz/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071502.webp)

Dịch vụ từ điển tiếng Anh trực tuyến hỗ trợ hiển thị hình ảnh minh họa do AI tạo ra tương ứng với ngữ nghĩa của từ vựng để người học dễ dàng ghi nhớ.

2\. [EasyVideoTrans (Công cụ hỗ trợ tự động dịch thuật và lồng tiếng video)](https://easyvideotrans.com/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071410.webp)

Mã nguồn mở hỗ trợ tự động biên dịch và tạo file lồng tiếng tiếng Trung cho các video tiếng Anh gốc. (Đóng góp của [@kitety](https://github.com/ruanyf/weekly/issues/4821))

3\. [AIEntries (WordPress plugin hỗ trợ tự động tạo nội dung bằng AI)](https://github.com/berchj/AIEntries)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071702.webp)

Plugin dành cho WordPress hỗ trợ tự động tạo lập bài viết và thiết kế ảnh minh họa tương ứng dựa trên chủ đề yêu cầu bằng AI.

## 资源

1\. [Free Font (Kho lưu trữ phông chữ chữ Hán miễn phí cho mục đích thương mại)](https://github.com/jaywcjlove/free-font)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071803.webp)

Dự án tổng hợp danh sách các phông chữ chữ Hán được phép sử dụng thương mại miễn phí với hơn 199 lựa chọn. (Đóng góp của [@jaywcjlove](https://github.com/ruanyf/weekly/issues/4839))

2\. [Daily Blog (Kênh tổng hợp các bài viết kỹ thuật tiếng Trung nổi bật)](https://daily-blog.chlinlearn.top/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071804.webp)

Trang tin chuyên cập nhật các chia sẻ blog công nghệ tiếng Trung hàng ngày. (Đóng góp của [@chlinlearn](https://github.com/ruanyf/weekly/issues/4831))

3\. [SaltyLeo Book DB API (Cổng truy xuất thông tin sách tiếng Trung)](https://book-db-v1.saltyleo.com/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071805.webp)

Dịch vụ cung cấp thông tin metadata của các đầu sách tiếng Trung bao gồm tên sách, tác giả, nhà xuất bản, tóm tắt nội dung, ảnh bìa, giá bán... (Đóng góp của [@SaltyLeo](https://github.com/ruanyf/weekly/issues/4841))

4\. [Movie Posters Perfected (Kho lưu trữ ảnh poster phim chất lượng 4K)](https://www.moviepostersperfected.com/quick-setup)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032111.webp)

Bộ sưu tập ảnh poster phim khổng lồ với hơn 3.500 ảnh chất lượng cao 4K đi kèm API kết nối hỗ trợ làm trình bảo vệ màn hình trên Smart TV.

## 图片

1\. [Những tác phẩm điêu khắc nghệ thuật lấy cảm hứng từ cấu trúc toán học](http://zacharyabel.com/sculpture/)

Một giảng viên công nghệ thông tin tại MIT chia sẻ niềm đam mê chế tác các mô hình cấu trúc toán học từ những vật dụng văn phòng quen thuộc.

Dưới đây là mô hình xoắn ốc hình sao được ghép hoàn toàn từ các ghim kẹp giấy.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071401.webp)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071402.webp)

Mô hình Borromean Rings độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071403.webp)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071404.webp)

Và một vài tác phẩm nghệ thuật toán học khác.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071405.webp)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071406.webp)

2\. [Biểu đồ tương quan giữa sản lượng thuốc lá tiêu thụ và tỷ lệ tử vong do ung thư phổi](https://commons.wikimedia.org/wiki/File:Smoking-and-lung-cancer-mortality-US-only_3048.png)

Biểu đồ so sánh hai xu hướng: đường màu tím hiển thị sản lượng thuốc lá tiêu thụ tại Mỹ qua các năm và đường màu đỏ hiển thị tỷ lệ tử vong do bệnh ung thư phổi.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071501.webp)

Có thể thấy hai đường đồ thị có hình dáng tương đồng gần như tuyệt đối, cho thấy mối liên hệ nhân quả cực kỳ mạnh mẽ. Tỷ lệ tử vong do ung thư phổi phản ánh độ trễ khoảng 25 đến 30 năm so với sản lượng tiêu thụ thuốc lá.

Năm 1964, sản lượng tiêu thụ thuốc lá tại Mỹ đạt đỉnh và bắt đầu giảm dần; đến đầu thập niên 1990, tỷ lệ tử vong do ung thư phổi cũng chạm đỉnh và bước vào xu hướng giảm tương ứng.

## ✍️ Bài đọc thêm

### Gửi AWS: Xin hãy để tôi làm một kỹ sư đám mây thuần túy một lần nữa

Tôi là một kỹ sư chịu trách nhiệm quản lý và vận hành hệ thống đám mây Amazon Web Services (AWS) cho doanh nghiệp.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071818.webp)

Tôi yêu thích các dịch vụ của AWS và luôn tham gia sự kiện thường niên re:Invent của họ. Sự kiện năm 2022 thực sự tuyệt vời với rất nhiều cập nhật kỹ thuật giá trị về hạ tầng đám mây.

Tuy nhiên đến năm 2023, làn sóng Generative AI bắt đầu xâm chiếm sự kiện, từ các giải pháp tương tác khách hàng đến tạo nội dung, cấu trúc vận hành... Tất cả đều xoay quanh AI. Mặc dù tôi coi đó là một làn sóng thổi phồng, nhưng cũng phải thừa nhận bản thân có phần hào hứng trước những cơ hội công nghệ mới này mang lại.

Nhưng đến sự kiện năm 2024, bằng cách nào đó, sự tập trung của AWS dành cho Generative AI đã trở nên thái quá. Phải đến hơn 80% thời lượng và nội dung chia sẻ chỉ xoay quanh AI, hầu như không còn chỗ cho các chủ đề hạ tầng truyền thống.

Điều này vô hình trung gửi đi một thông điệp đến giới lập trình viên rằng AWS hiện nay chỉ tập trung cho AI và không còn mặn mà với các dịch vụ cốt lõi khác nữa.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071408.webp)

Tôi cảm thấy định hướng của AWS và nhu cầu thực tế của chúng tôi đang ngày một xa nhau. Những giá trị cốt lõi chúng tôi trân trọng dường như không còn được họ ưu tiên. Họ càng nói nhiều về AI thì càng ngầm khẳng định rằng trong mắt họ, cơ sở dữ liệu không còn quan trọng, hạ tầng mở rộng linh hoạt hay khả năng duy trì mã nguồn hệ thống cũng không còn là ưu tiên hàng đầu, tất cả chỉ có AI mới là tương lai.

Hệ quả là ngân sách dành cho các sản phẩm hạ tầng truyền thống yêu thích của chúng tôi sẽ bị cắt giảm, các tính năng mới sẽ bị chậm trễ cập nhật hoặc thậm chí bị ngưng phát triển.

Tóm lại, AWS đang ngầm khuyên các nhà phát triển ngừng quan tâm đến hạ tầng cốt lõi để dồn toàn lực cho AI. Tôi tin rằng đây là một tư duy sai lầm. Bởi vì chỉ khi hệ thống hạ tầng bên dưới vận hành ổn định thì các ứng dụng AI mới có đất diễn. Chúng tôi sử dụng dịch vụ đám mây của AWS là để xây dựng nền tảng cho hoạt động kinh doanh thực tế của mình chứ không phải để ngồi chờ đợi AI giải quyết hộ mọi vấn đề trong tương lai - điều mà ai cũng biết là bất khả thi.

Tôi hy vọng AWS sẽ không quên đi gốc gác phát triển của mình, tiếp tục tôn trọng và hỗ trợ các nhóm sản phẩm cốt lõi đã làm nên thương hiệu của họ. Xin hãy lắng nghe và giải quyết các bài toán thực tế của lập trình viên để giúp họ xây dựng các hệ thống ngày một tốt hơn.

Với tư cách là một khách hàng trung thành, tôi khẩn cầu AWS: Xin hãy để tôi làm một kỹ sư đám mây thuần túy một lần nữa.

## Lịch sử tuần này

- 2023年（第 262 期）：[Xu hướng bảo mật: Phân tích về tương lai của các giải pháp xác thực không mật khẩu (passwordless)](https://www.ruanyifeng.com/blog/2023/07/weekly-issue-262.html)
- 2022年（第 212 期）：[Triết lý cuộc sống: Suy ngẫm về giá trị thời gian và cách tận hưởng cuộc đời ý nghĩa](https://www.ruanyifeng.com/blog/2022/07/weekly-issue-212.html)
- 2021年（第 162 期）：[Trải nghiệm cuộc sống: Lăng kính cuộc đời thông qua trò chơi kinh điển Pac-Man](http://www.ruanyifeng.com/blog/2021/06/weekly-issue-162.html)
- 2020年（第 112 期）：[Kinh nghiệm quản lý: Các phương pháp rèn luyện và nâng cao năng lực lãnh đạo thực chiến](https://www.ruanyifeng.com/blog/2020/06/weekly-issue-112.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
