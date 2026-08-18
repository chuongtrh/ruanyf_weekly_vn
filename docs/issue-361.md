# Bản tin chia sẻ công nghệ (Số 361): Mạng ẩn danh Tor có thực sự an toàn không?

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/7408) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081404.webp)

Tháp Thời Gian Yên Đài (烟台时光塔) khánh thành vào năm ngoái là một công trình văn hóa bên bờ biển ấn tượng: Tầng dưới là nhà hát mở, tầng giữa là nền tảng ngắm biển và tầng trên cùng là thư viện, phòng triển lãm và quán cà phê. (Nguồn: [archiposition.com](https://www.archiposition.com/items/20241105014028))

## 暗网 Tor 安全吗？

### 1. Tor Browser là gì?

Chắc hẳn nhiều bạn đã biết về [trình duyệt Tor](https://www.torproject.org/) — đây là công cụ chủ yếu để truy cập vào **dark web (mạng tối)**.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081008.webp)

Dark web (mạng tối) là phần của internet không thể truy cập bằng các trình duyệt thông thường mà bắt buộc phải dùng các công cụ chuyên dụng.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081007.webp)

Lý do dark web cần công cụ chuyên dụng là vì nó sử dụng một kiến trúc đặc biệt được thiết kế để **đảm bảo người truy cập có mức độ ẩn danh cao, cực kỳ khó truy vết**.

Nếu bạn muốn thực hiện các hoạt động internet bí mật, bạn có thể sử dụng dark web. Tương tự, các trang web ngầm muốn giấu kín hoạt động của mình khỏi sự phát hiện của cơ quan chức năng có thể tạo phiên bản dark web, không thể truy cập từ internet thông thường.

Dark web có tên miền riêng là `.onion` — các website với tên miền này đều phải truy cập thông qua trình duyệt Tor.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081310.webp)

### 2. Nguyên lý hoạt động của Tor

Trước đây tôi luôn tin rằng Tor/dark web rất an toàn, có thể đảm bảo ẩn danh tuyệt đối cho người dùng và không thể truy vết ra người thật.

Lý do là vì kiến trúc của nó được thiết kế để chống truy vết: **Thay vì kết nối trực tiếp đến địa chỉ đích, Tor tìm một nút trung chuyển (relay node) ngẫu nhiên** để đi qua.

Quy định bắt buộc là phải đi qua đúng 3 nút trung chuyển mới có thể kết nối được trang web đích. Mỗi nút trung chuyển chỉ biết nút trước và nút sau nó, do đó **dù một nút bị tấn công chiếm quyền, kẻ tấn công cũng không thể thấy toàn bộ đường truyền thông tin**.

Về lý thuyết, chỉ khi cả ba nút trung chuyển đều bị phá vỡ thì mới có thể truy vết được người dùng. Nhưng vì các nút này được chọn ngẫu nhiên từ khắp nơi trên thế giới, xác suất tất cả đều bị phá vỡ cùng lúc là cực kỳ thấp.

Thiết kế này được gọi là "định tuyến hành tây" (onion routing) — giống như bóc củ hành, phải lột từng lớp nút trung chuyển mới có thể hiểu được toàn bộ đường truyền. Thực ra, từ "Tor" chính là viết tắt của **The Onion Router** (Bộ định tuyến hành tây).

### 3. Sự thật bất ngờ về Tor

Tuần trước, tôi đọc được [một bài viết](https://thereader.mitpress.mit.edu/the-secret-history-of-tor-how-a-military-project-became-a-lifeline-for-privacy/) đã hoàn toàn làm lung lay niềm tin của tôi vào Tor.

Tôi vô cùng bất ngờ khi phát hiện ra: **Tor là do chính phủ Mỹ phát triển**.

Năm 1997, **Phòng thí nghiệm Nghiên cứu Hải quân Mỹ (NRL)** đã phát minh ra Tor. Động cơ ban đầu là **ngăn chặn chính phủ nước ngoài truy vết các thông tin liên lạc mật của Mỹ**.

Bài toán đặt ra là: Các nhân viên tình báo Mỹ ở nước ngoài cần gửi thông tin bí mật về máy chủ của CIA mà không để chính phủ sở tại phát hiện và truy vết, nhưng lại buộc phải sử dụng đường truyền dân sự của nước ngoài. Giải pháp chính là Tor — thông qua định tuyến hành tây, Tor cho phép che giấu vị trí người gửi và địa chỉ đích trước con mắt của nhà cung cấp internet nước ngoài.

Năm 2004, chính phủ Mỹ công bố mã nguồn của dự án này. Tổ chức Electronic Frontier Foundation (EFF) tiếp nhận và tiếp tục phát triển, dần biến thành Tor ngày nay, nhưng thiết kế nền tảng về cơ bản không có thay đổi lớn.

Sau khi công bố mã nguồn mở, chính phủ Mỹ không buông tay dự án này mà tiếp tục tài trợ mạnh mẽ nhiều năm. Năm 2012, ngân sách hàng năm của dự án Tor là 2 triệu đô la, trong đó [80% đến từ chính phủ Mỹ](https://en.wikipedia.org/wiki/The_Tor_Project#Funding).

Tôi đã tra cứu [báo cáo tài chính](https://www.torproject.org/static/findoc/2023-2024-The_Tor_Project-AuditedFinancialStatements.pdf) mới nhất năm 2023-2024: Trong tổng doanh thu hơn 7,9 triệu đô la, vẫn có hơn 2 triệu đô la đến từ chính phủ.

Chính phủ Mỹ tài trợ mạnh cho Tor vì dự án này có giá trị sử dụng với họ.

Tôi tin mã nguồn Tor là đáng tin cậy và không có cửa hậu (backdoor) được cài cắm — xét cho cùng đây là phần mềm mã nguồn mở, phải chịu sự kiểm tra của lập trình viên khắp thế giới. Nhưng chính phủ Mỹ chắc chắn nắm rõ mọi chi tiết của mã nguồn và rất có thể đang triển khai các phiên bản đã được tùy chỉnh của họ với một số thay đổi không được công bố.

Theo các thông tin từng rò rỉ trước đây, nhiều nút trung chuyển của Tor là do chính phủ Mỹ thiết lập (tỷ lệ cụ thể không thể xác minh). Vì vậy, tôi cho rằng **không thể giả định Tor là an toàn tuyệt đối — chính phủ Mỹ rất có thể đang giám sát các luồng thông tin qua Tor**.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081009.webp)

Chợ đen dark web đình đám một thời "Silk Road" (hình trên) vận hành hoàn toàn dựa trên Tor. Tuy nhiên năm 2013 nó đã bị chính phủ Mỹ đóng cửa và người sáng lập bị bắt. Đây cũng là bằng chứng gián tiếp cho thấy Tor không hoàn toàn an toàn như người ta nghĩ.

## 科技动态

（1）Tuần trước, module **hạ cánh lên Mặt Trăng có người lái "Lãm Nguyệt"** (揽月) của Trung Quốc đã thực hiện thử nghiệm hạ cánh và cất cánh tại huyện Hoài Lai, tỉnh Hà Bắc.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081401.webp)

Module được treo bên dưới một đĩa thép lớn, và đĩa thép được kéo lên xuống bằng cáp thép để mô phỏng lực hấp dẫn thấp trên Mặt Trăng.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081402.webp)

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081403.webp)

（2）Nhóm nghiên cứu của Đại học Pennsylvania (Mỹ) vừa công bố một kỹ thuật mới có thể **tái tạo lại nội dung cuộc gọi điện thoại bằng cách theo dõi rung động siêu nhỏ** của thiết bị.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081102.webp)

Khi điện thoại đang phát âm thanh trong cuộc gọi, loa của máy sẽ tạo ra các rung động vi mô. Bằng cách sử dụng radar laser (LiDAR) theo dõi từ khoảng cách 3 mét, có thể cảm nhận được các rung động này và từ đó tái tạo lại tín hiệu âm thanh.

Kết hợp thêm với mô hình chuyển đổi giọng nói sang văn bản Whisper, nội dung cuộc gọi có thể được trích xuất ra dạng văn bản với độ chính xác khoảng 60%.

（3）Một lập trình viên người Mỹ đã tự chế tạo ra một **màn hình pixel bằng gỗ** độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081115.webp)

Mỗi pixel trên màn hình là một khối gỗ nhỏ, một mặt được sơn đen.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081116.webp)

Bộ điều khiển màn hình là một chiếc Raspberry Pi: Sau khi nhận lệnh hiển thị hình ảnh, nó tính toán xem khối gỗ nào cần xoay, rồi điều khiển cánh tay robot xoay từng khối một.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081118.webp)

Kết quả hiển thị cuối cùng trông như sau:

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081117.webp)

（4）Google tiết lộ hệ thống Android đã tích hợp sẵn **hệ thống cảnh báo động đất toàn cầu** có khả năng gửi cảnh báo động đất đến người dùng trên khắp thế giới.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025072804.webp)

Điện thoại Android đều được trang bị cảm biến gia tốc (accelerometer) — loại cảm biến giúp màn hình tự động xoay khi điện thoại được đặt ngang. Cảm biến này cũng có khả năng phát hiện mọi chuyển động của thiết bị.

Nếu hệ thống phát hiện nhiều điện thoại trong cùng một khu vực địa lý đột ngột rung cùng lúc, đó là dấu hiệu của động đất. Google sẽ lập tức gửi cảnh báo động đất đến người dùng trong khu vực đó.

Hệ thống này được triển khai lần đầu tại New Zealand và Hy Lạp vào tháng 4/2021 và hiện đã phủ sóng tới 98 quốc gia và vùng lãnh thổ. Hệ thống đã gửi cảnh báo thành công cho trận động đất 6,7 độ Richter tại Philippines tháng 11/2023 và trận 5,7 độ tại Nepal cùng tháng.

（5）Tại sao con người cần ngủ? Một nghiên cứu mới đây chỉ ra mối liên hệ giữa giấc ngủ và **ty thể (mitochondria) trong tế bào**.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025073012.webp)

Trong môi trường có oxy, hoạt động liên tục của ty thể dần dẫn đến phân rã cấu trúc của chúng, do đó cần có một giai đoạn nghỉ ngơi (giấc ngủ) để tái tạo và nạp lại năng lượng.

Kết luận rút ra là: Bất kỳ sinh vật nào cần oxy để tồn tại thì đều cần ngủ, vì hoạt động hiếu khí liên tục sẽ tiêu hao ty thể.

## 文章

1、[Giới thiệu về Anchor Positioning — Định vị neo trong CSS](https://webkit.org/blog/17240/a-gentle-introduction-to-anchor-positioning/) (tiếng Anh)

Cú pháp CSS mới "Anchor Positioning" cho phép lập trình viên định vị các menu popup, tooltip hay dropdown tương đối với một phần tử neo (anchor element) bất kỳ hoàn toàn bằng CSS thuần túy mà không cần viết thêm bất kỳ đoạn JavaScript nào.

2、[Hướng dẫn gắn kết dịch vụ lưu trữ đám mây vào thư mục cục bộ bằng Rclone](https://blog.fernvenue.com/archives/mount-cloud-drive-using-rclone/) (tiếng Anh)

Bài hướng dẫn chi tiết cách sử dụng công cụ [Rclone](https://rclone.org/) để gắn kết (mount) các dịch vụ lưu trữ đám mây (như Microsoft OneDrive) thành một thư mục cục bộ trên máy tính, giúp truy cập file đám mây như truy cập ổ đĩa thông thường.

3、[Hướng dẫn lựa chọn font chữ Latin phù hợp](https://imperavi.com/books/ui-typography/basis/choosing-typeface/) (tiếng Anh)

Bài viết phân tích các tiêu chí và lưu ý thực tế khi lựa chọn font chữ Latin phù hợp cho thiết kế giao diện và tài liệu, từ tính dễ đọc đến tính thẩm mỹ và phong cách thương hiệu.

4、[Cách tôi sử dụng NotebookLM để "xem" phim mà không cần xem phim](https://www.xda-developers.com/using-notebooklm-to-watch-a-show/) (tiếng Anh)

NotebookLM hiện được đánh giá là công cụ ghi chú AI tốt nhất hiện nay. Tác giả chia sẻ cách ông dùng nó để "tiêu thụ" nội dung các bộ phim hay series mà không cần dành thời gian xem trực tiếp — một trường hợp sử dụng sáng tạo và đáng tham khảo.

5、[Cách chạy ứng dụng đồ họa GUI trong Docker container](https://github.com/hemashushu/docker-archlinux-gui) (tiếng Anh)

Hướng dẫn sử dụng giao thức Wayland để chạy các ứng dụng có giao diện đồ họa (GUI) bên trong Docker container và hiển thị cửa sổ ra màn hình máy chủ.

6、[Tại sao π² ≈ g? (Pi bình phương xấp xỉ gia tốc trọng trường)](https://roitman.io/blog/91) (tiếng Anh)

π² ≈ 9,86, rất gần với giá trị gia tốc trọng trường g ≈ 9,8 m/s². Bài viết giải thích đây không phải là sự trùng hợp ngẫu nhiên mà có liên quan trực tiếp đến định nghĩa của đơn vị đo lường mét (1 mét = một phần triệu khoảng cách từ Bắc Cực đến xích đạo).

## 工具

1、[Battery](https://github.com/actuallymentor/battery)

Tiện ích nhỏ cho MacBook giúp giới hạn mức sạc tối đa của pin ở 80%, kéo dài tuổi thọ pin theo khuyến cáo của Apple.

2、[Readeck](https://readeck.org)

Ứng dụng web tự triển khai hỗ trợ lưu trữ và đọc sau (read-later) các trang web, tự động tải và lưu nội dung của trang về cục bộ để đọc ngoại tuyến sau này.

3、[missing.css](https://missing.style/)

Thư viện CSS tối giản cung cấp một bộ kiểu dáng (stylesheet) cơ bản, dễ mở rộng làm nền tảng cho việc tùy chỉnh thiết kế.

4、[My idlers](https://github.com/cp6/my-idlers)

Ứng dụng web tự triển khai giúp quản lý tập trung toàn bộ các máy chủ ảo (VPS), hosting chia sẻ và tên miền của bạn trong một giao diện. Xem thêm [bài giới thiệu](https://www.xda-developers.com/use-self-hosted-app-tabs-home-server-vps-domains/).

5、[Kimu](https://trykimu.com/)

Trình biên tập video chạy trực tiếp trên trình duyệt web, hỗ trợ tích hợp AI để hỗ trợ quá trình chỉnh sửa. [Mã nguồn mở](https://github.com/robinroy03/videoeditor).

6、[vYinn (殷人)](https://github.com/shanleiguang/vYinn)

Công cụ tạo và thiết kế các mẫu ấn triện (con dấu) theo phong cách cổ đại Trung Hoa. (Đóng góp từ [@shanleiguang](https://github.com/ruanyf/weekly/issues/7486))

7、[Call-Me](https://github.com/miroslavpejic85/call-me)

Ứng dụng web mã nguồn mở hỗ trợ gọi video 1-1 trực tiếp qua trình duyệt, xem thử tại [Demo](https://cme.mirotalk.com/). (Đóng góp từ [@miroslavpejic85](https://github.com/ruanyf/weekly/issues/7500))

8、[Modern MD Editor](https://github.com/xiaobox/mdeditor)

Trình biên tập Markdown chạy trên trình duyệt, tạo ra mã HTML tương thích với định dạng hiển thị của các nền tảng mạng xã hội Trung Quốc như WeChat Official Account. (Đóng góp từ [@xiaobox](https://github.com/ruanyf/weekly/issues/7506))

Tham khảo thêm trình biên tập Markdown tối ưu cho WeChat sử dụng AI: [md2wechat.cn](https://www.md2wechat.cn/). (Đóng góp từ [@geekjourneyx](https://github.com/ruanyf/weekly/issues/7513))

9、[FluentRead (流畅阅读)](https://github.com/Bistutu/FluentRead)

Tiện ích mở rộng dịch thuật mã nguồn mở cho trình duyệt, được phát triển như một giải pháp thay thế mã nguồn mở cho "Immersive Translation". Hỗ trợ nhiều công cụ dịch và mô hình AI, cung cấp dịch thuật song ngữ và dịch thuật theo từ được tô sáng. (Đóng góp từ [@Bistutu](https://github.com/ruanyf/weekly/issues/7514))

10、[Diff Excel](https://github.com/zbuzhi/diff-excel)

Ứng dụng máy tính đa nền tảng mã nguồn mở viết bằng Go để so sánh trực quan sự khác biệt giữa hai file Excel. (Đóng góp từ [@zbuzhi](https://github.com/ruanyf/weekly/issues/7523))

## AI 相关

1、[LLM from URL](https://818233.xyz/)

Dịch vụ thú vị cho phép đặt câu hỏi cho mô hình AI lớn trực tiếp qua URL — ví dụ: [818233.xyz/你是什么模型](https://818233.xyz/%E4%BD%A0%E6%98%AF%E4%BB%80%E4%B9%88%E6%A8%A1%E5%9E%8B). (Đóng góp từ [@yvonuk](https://github.com/ruanyf/weekly/issues/7517))

2、[AI Short Video Factory (短视频工厂)](https://github.com/YILS-LIN/short-video-factory)

Ứng dụng web mã nguồn mở cho phép người dùng tải video thô lên, cung cấp câu lệnh nhắc và để AI tự động tạo ra video ngắn hoàn chỉnh kèm kịch bản bình luận. (Đóng góp từ [@YILS-LIN](https://github.com/ruanyf/weekly/issues/7518))

3、[Mapedia.cc](https://mapedia.cc/)

Bản đồ AI: Người dùng tìm kiếm một chủ đề, hệ thống sẽ hiển thị bản đồ địa lý liên quan cùng các bài giải thích. Ví dụ như [bản đồ hành trình của Tô Đông Pha (Tô Thức)](https://mapedia.cc/view/22cb103f456b4502dfa7315ebfc3dc83). (Đóng góp từ [@klemperer](https://github.com/ruanyf/weekly/issues/7525))

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081306.webp)

## 资源

1、[One Million Screenshots](https://onemillionscreenshots.com)

Trang web tuyên bố được tạo thành từ một triệu ảnh chụp màn hình các trang web, người dùng có thể phóng to thu nhỏ để xem.

2、[Engineering.fyi](https://engineering.fyi/)

Trang web tổng hợp và lưu trữ các bài viết kỹ thuật từ các công ty công nghệ lớn trên thế giới vào một nơi để dễ tra cứu.

3、[Touch Mapper](https://touch-mapper.org/en/)

Ý tưởng sáng tạo xuất sắc: Nhập địa chỉ đường phố vào, trang web xuất ra file bản đồ 3D của khu vực đó, có thể in 3D ra để người khiếm thị có thể dùng tay cảm nhận bản đồ.

4、[Pricing Pages Design](https://pricingpages.design/)

Thư viện thiết kế tổng hợp nhiều mẫu trang định giá (pricing page) đa dạng từ các sản phẩm phần mềm khác nhau để tham khảo và lấy cảm hứng.

## 图片

1、[Tượng điêu khắc cổ điển kết hợp thời trang đương đại](https://www.itsnicethat.com/articles/leo-caillard-hipster-in-stone)

Một nhiếp ảnh gia người Pháp đã sáng tạo mặc quần áo và phụ kiện thời trang hiện đại lên các bức tượng điêu khắc cổ điển.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081001.webp)

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081002.webp)

Sự kết hợp đối lập này không chỉ tạo ra cảm giác hài hước mà còn khơi gợi một góc nhìn hoàn toàn mới lạ về các tác phẩm nghệ thuật cổ điển.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081003.webp)

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081004.webp)

Điều này nhắc nhở chúng ta rằng ấn tượng của người khác về một con người và khí chất mà họ toát ra phần lớn phụ thuộc vào cách ăn mặc và phong cách thể hiện bản thân.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081005.webp)

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081006.webp)

## 文摘

1、**Kỹ năng kỹ thuật của tôi đã thoái hóa**

Năm năm trước, khi vừa tốt nghiệp đại học, tôi đam mê lập trình và tích cực tham gia vào hàng loạt dự án mã nguồn mở.

Tôi đã đổ vào đó hàng nghìn giờ với toàn bộ tâm huyết. Dù không có thu nhập từ đó, tôi cảm thấy vô cùng thỏa mãn, và người dùng của các dự án đó đánh giá cao công việc của tôi.

Sau tốt nghiệp, tôi bắt đầu tìm việc làm. Tôi tin rằng các công ty sẽ đánh giá cao kinh nghiệm mã nguồn mở của mình. Tôi đã nhầm.

Tôi nộp hơn 600 đơn xin việc, giới thiệu các đóng góp mã nguồn mở của mình, nhưng chỉ nhận được 3 lời mời phỏng vấn. Cuối cùng tôi nhận đề nghị từ một công ty khởi nghiệp.

Ban ngày tôi làm việc cho công ty khởi nghiệp đó 8-9 tiếng. Về nhà, tôi tiếp tục đổ vào dự án mã nguồn mở của mình cho đến tận khuya.

Lương tôi rất thấp, nhưng tôi tìm thấy niềm vui trong đó. Kỹ năng của tôi nâng cao nhanh chóng, và tầm ảnh hưởng trong cộng đồng cũng tăng lên đáng kể.

Cuối cùng, một ngày nào đó, tôi đối mặt với thực tế. Công ty không trân trọng đúng giá trị của tôi, còn những người biết giá trị của tôi thì lại không phải người trả lương cho tôi. Tôi lùi bước và bắt đầu khổ luyện Leetcode.

Tôi không còn đầu tư nhiều thời gian vào mã nguồn mở nữa, và cộng đồng dự án cũng dần mất đi sức sống. Bỏ các dự án mã nguồn mở khiến tôi đau lòng, nhưng nhờ đó tôi vào được một công ty lớn với mức lương tăng 5 lần.

Tôi đổ hết thời gian vào các dự án của công ty, được cấp trên đánh giá tốt. Hộp thư của tôi bắt đầu đầy những email săn đầu người từ các công ty khác.

Nhưng tôi biết mình đang thoái hóa về kỹ thuật. Các dự án công ty nhàm chán, không có thách thức, sử dụng công nghệ nội bộ riêng.

Ngoài ra, tôi cũng không còn hạnh phúc như trước.

Tôi nghĩ mình sẽ tích lũy tiền, vài năm nữa nghỉ hưu sớm, và hy vọng lúc đó thế giới mã nguồn mở vẫn sôi động như xưa.

## 言论

1、

Để thấy cuộc điên rồ gọi vốn của các công ty AI tệ đến mức nào: Cựu Giám đốc Khoa học của OpenAI, Ilya Sutskever, đã huy động được 1 tỷ đô la vào năm 2024 và vài tháng sau lại huy động thêm 2 tỷ đô la, với định giá công ty lên tới 32 tỷ đô la.

Theo tôi biết, sản phẩm duy nhất của họ là 370 từ trên trang web của công ty, tương đương mỗi từ có giá trị 80 triệu đô la, trong đó 148 từ là về việc một đối tác rời khỏi công ty. Dù sao ít nhất họ còn có website — có những nhà sáng lập nhận tiền xong là mất tăm tích luôn.

-- *Trích bản tin Substack*

2、

Các công ty bảo hiểm đang cực kỳ lo ngại: Khi trái đất nóng lên và thiên tai cực đoan ngày một nhiều hơn, rủi ro thiệt hại tài sản tăng mạnh và thế giới đang trở nên không thể bảo hiểm được nữa.

-- *Trích bài viết 《Thế giới sắp không còn thể bảo hiểm》*

3、

Các gói cập nhật Windows 11 trước đây được gọi là "gói Mùa xuân" và "gói Mùa thu". Sau đó, có người phản ánh tên gọi này không phù hợp với người dùng ở Nam Bán cầu (vì ở đó mùa ngược lại), nên Microsoft đổi tên thành gói H1 và gói H2.

-- *Trích bài viết 《Tại sao các gói cập nhật Windows được gọi là H1 và H2》*

4、

Trong hơn một thập kỷ, các khóa học lập trình cấp tốc (bootcamp) là một ngành trụ cột của Silicon Valley. Ngày nay, AI đang khiến các công ty giảm tuyển nhân sự cấp thấp, đồng thời học viên có thể tự học lập trình với sự hỗ trợ của AI. Các bootcamp lập trình đang dần biến mất.

-- *Reuters*

5、

Con người tưởng mình đang suy nghĩ, nhưng thực ra chỉ đang sắp xếp lại những định kiến sẵn có của mình.

-- *William James, triết gia người Mỹ*

## 往年回顾

- Số #314: [Liệu "Black Myth: Wukong" có thể tạo ra một ngành công nghiệp game không?](https://www.ruanyifeng.com/blog/2024/08/weekly-issue-314.html)
- Số #264: [Bài học rút ra từ câu chuyện Elasticsearch về mã nguồn mở và thương mại hóa](https://www.ruanyifeng.com/blog/2023/07/weekly-issue-264.html)
- Số #214: [Bản đồ thế giới mà bạn đang dùng hằng ngày thực ra là sai](https://www.ruanyifeng.com/blog/2022/07/weekly-issue-214.html)
- Số #164: [So sánh thực tế tỷ lệ xin việc thành công giữa học viên bootcamp và sinh viên đại học](https://www.ruanyifeng.com/blog/2021/06/weekly-issue-164.html)

(Hết)
