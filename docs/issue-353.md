# Bản tin chia sẻ công nghệ (Số 353): Phong cách thiết kế "Kính lỏng" của Apple hướng tới kỷ nguyên AR

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/6965) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061804.webp)

Vào tối ngày 17 tháng 6 vừa qua, thành phố Trùng Khánh đã tổ chức một buổi biểu diễn máy bay không người lái quy mô cực lớn với sự tham gia của 11.787 chiếc drone. Bức ảnh phía trên ghi lại khoảnh khắc tạo hình nghệ thuật mang tên "Trùng Khánh trên bầu trời". (Nguồn: [xinhuanet.com](https://www.xinhuanet.com/photo/20250618/803d7411ae6041f3981ae375d5ac1bff/c.html))

## 苹果的“液态玻璃”是为了 AR

Tuần trước, tập đoàn Apple đã chính thức công bố ngôn ngữ thiết kế giao diện thế hệ mới của hãng mang tên "Kính lỏng" (Liquid Glass).

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061401.webp)

Phong cách thiết kế mới này ứng dụng chất liệu mô phỏng thủy tinh lỏng để chế tác các nút bấm và bảng điều khiển (hình trên). Phong cách thiết kế phẳng (Flat Design) thống trị trong nhiều năm qua đã bị loại bỏ hoàn toàn.

Hình bên dưới so sánh giao diện thiết kế phẳng truyền thống trên iPhone (bên trái) với phong cách thiết kế kính lỏng mới ở phiên bản thử nghiệm (bên phải):

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061402.webp)

Hầu hết mọi người khi tiếp xúc với phong cách thiết kế mới này đều đưa ra các phản hồi tương đối tiêu cực và cho rằng giao diện này trông không được đẹp mắt. Mọi người đều cảm thấy khó hiểu tại sao Apple lại cố tình chèn thêm một lớp chất liệu kính bán trong suốt lên trên các biểu tượng màn hình.

Nhiều người dùng thậm chí còn [đưa ra bình luận hài hước](https://x.com/greggertruck/status/1932173476879888556) rằng nếu cố chủ tịch Steve Jobs còn sống và nhìn thấy giao diện iPhone biến đổi thế này, ông có thể sẽ sa thải toàn bộ đội ngũ thiết kế của hãng (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061901.webp)

Vậy đâu là động cơ thực sự đằng sau việc Apple đột ngột thay đổi toàn diện giao diện người dùng vốn đang hoạt động rất tốt?

Phía Apple hoàn toàn né tránh đưa ra câu trả lời trực tiếp cho câu hỏi này, nhưng mới đây tôi đã đọc được [một bài phân tích sâu](https://omc345.substack.com/p/from-skeuomorphic-to-liquid-glass) đưa ra một dự báo rất thực tế và sắc bén.

Tác giả bài viết cho rằng **quyết định thay đổi này của Apple hoàn toàn không phải vì mục đích thẩm mỹ đơn thuần, mà là bước đi chiến lược chuẩn bị cho kỷ nguyên điện toán không gian (Spatial Computing) tiếp theo — tức là công nghệ AR**.

Toàn bộ các thiết bị điện toán chúng ta đang sử dụng hiện nay đều vận hành dựa trên các tương tác mặt phẳng hai chiều, người dùng hướng mắt nhìn vào một màn hình phẳng, do đó phong cách thiết kế phẳng hai chiều là hoàn toàn phù hợp.

Tuy nhiên đối với các thiết bị AR tương lai, người dùng sẽ bước vào một không gian 3D lập thể, mọi đối tượng tiếp xúc đều hiển thị dưới dạng hình khối ba chiều, đòi hỏi giao diện tương tác cũng phải được thiết kế dạng hình khối lập thể.

**Các thiết bị AR sẽ không còn màn hình vật lý nữa mà chỉ có không gian xung quanh bạn. Màn hình không còn quan trọng, không gian mới là yếu tố quyết định**.

Phong cách kính lỏng thực chất là một thiết kế hướng tới không gian, nhằm mục đích tạo cho giao diện người dùng cảm giác như một thực thể vật lý có thể chạm vào, giúp người dùng cảm nhận mỗi nút bấm đều có thể tích và khối lượng thực tế. Đồng thời đặc tính bán trong suốt của kính giúp không che khuất các đối tượng cảnh quan phía sau, tạo nên chiều sâu không gian đa tầng rõ rệt.

Dưới lăng kính phân tích này, những lời giới thiệu của ông Alan Dye — Phó chủ tịch phụ trách thiết kế giao diện của Apple — về ngôn ngữ kính lỏng trở nên rất dễ hiểu:

> Mỗi phần tử giao diện đều được chúng tôi thiết kế kỹ lưỡng để mang lại cảm nhận vật lý thực tế: Chúng sở hữu chiều không gian cụ thể, có khả năng phản chiếu ánh sáng động thời gian thực và tự đổ bóng xuống các bề mặt xung quanh.

Về thiết bị AR, hiện tại danh mục sản phẩm của Apple mới chỉ ghi nhận dòng kính thông minh Vision Pro.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061902.webp)

Giao diện kính lỏng ban đầu nhiều khả năng được thiết kế riêng phục vụ cho dòng kính thông minh này. Trong không gian AR, việc giao diện điều khiển hiển thị dưới dạng một tấm kính lơ lửng giữa không trung là vô cùng tự nhiên và hợp lý.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061404.webp)

Để đồng bộ hóa ngôn ngữ thiết kế chung trên toàn hệ sinh thái sản phẩm, Apple đã quyết định áp dụng chung phong cách này lên cả iPhone và Mac. Giải pháp này giúp các nhà phát triển phần mềm chỉ cần thiết kế giao diện một lần duy nhất là có thể tương thích tốt với mọi thiết bị của hãng.

Cơ chế đồng bộ này mang lại lợi thế lớn cho việc phổ cập AR trong tương lai. Khi người dùng đã quá quen thuộc với phong cách kính lỏng hằng ngày trên điện thoại và máy tính, thời điểm họ đeo chiếc kính AR lên, họ sẽ hoàn toàn không có cảm giác bỡ ngỡ với giao diện tương tác mới, cảm giác như thiết bị AR chỉ là một phần kéo dài tự nhiên của chiếc iPhone quen thuộc.

Nếu quả thực đây là toan tính chiến lược của Apple, chúng ta có thể tin tưởng rằng **tập đoàn này sẽ dành sự tập trung rất lớn để thúc đẩy mảng điện toán không gian thời gian tới**.

Mặc dù doanh số bán hàng của dòng Vision Pro hiện tại không được như kỳ vọng, Apple chắc chắn sẽ không từ bỏ dự án này mà sẽ tiếp tục tăng cường nguồn lực đầu tư, và nhiều khả năng sẽ sớm cho ra mắt các dòng kính AR gọn nhẹ hơn trong tương lai gần.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061405.webp)

AR rất có thể sẽ trở thành làn sóng bùng nổ tiếp theo của toàn ngành công nghiệp máy tính thế giới, và Apple đã đi trước một bước để thiết lập thế trận cho mình.

Đồng thời, giao diện kính lỏng đòi hỏi thiết bị phải thực hiện các tác vụ làm mờ thời gian thực, xử lý độ trong suốt động và chiếu sáng theo ngữ cảnh. Các tác vụ đồ họa phức tạp này đòi hỏi năng lực xử lý phần cứng đồ họa (GPU) cực kỳ mạnh mẽ — vốn là ưu thế vượt trội của các dòng chip tự chủ của Apple, giúp gia tăng khoảng cách cạnh tranh với các đối thủ trên thị trường.

## 科技动态

（1）Tập đoàn Meta giới thiệu tính năng mới hỗ trợ **tự động thiết kế video quảng cáo bằng AI** (AI Ads). Người dùng chỉ cần tải ảnh chụp sản phẩm thô lên, hệ thống AI sẽ tự động sinh dựng thành một video quảng cáo hoàn chỉnh đi kèm phần nhạc nền và nội dung văn bản quảng cáo phù hợp.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061802.webp)

Dự báo trong tương lai chi phí sản xuất quảng cáo sẽ giảm về mức cực thấp, quảng cáo xuất hiện ở khắp mọi nơi và được AI tự động tối ưu hóa cá nhân hóa theo sở thích của từng người xem cụ thể.

（2）Một chú rùa hoang dã tại Canada bị mất một phần chân sau do tai nạn đã được nhân viên bảo tàng hỗ trợ chế tạo một **thiết bị trợ xe lăn bằng gạch Lego**.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025050121.webp)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025050122.webp)

Hành động nhân văn này mang ý nghĩa lớn bởi rùa hoang dã sở hữu tuổi thọ rất cao (từ 50 đến 80 năm), và chiếc xe lăn Lego nhỏ này sẽ giúp nâng cao đáng kể chất lượng cuộc sống của chú rùa trong nhiều thập kỷ tới.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025050123.webp)

（3）Cục Dự án Nghiên cứu Quốc phòng Tiên tiến Mỹ (DARPA) công bố thiết lập kỷ lục thế giới mới về khoảng cách **truyền tải điện năng không dây**.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061702.webp)

Nhóm nghiên cứu đã ứng dụng các luồng tia laser chuyên dụng để truyền tải thành công năng lượng điện tới bộ thu cách xa 8,6 km, duy trì liên tục trong vòng 30 giây với công suất truyền tải đạt mốc hơn 800 Watt/giây. Đây là khoảng cách truyền tải điện không dây xa nhất được ghi nhận từ trước đến nay.

Bức ảnh phía trên minh họa thiết bị thu nhận tia laser: Khi luồng tia laser đi vào lỗ tâm của thiết bị sẽ được hệ thống gương phản chiếu tới hàng chục tấm pin quang điện bố trí xung quanh để chuyển hóa năng lượng ánh sáng ngược trở lại thành điện năng sinh hoạt.

（4）Bên cạnh làn sóng phát triển robot hình người sinh học, các viện nghiên cứu cũng đang dành sự quan tâm cho các dòng **robot mô phỏng hình dáng côn trùng** (Robot Insects).

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052501.webp)

Một doanh nghiệp tại Mỹ vừa giới thiệu mẫu robot có hình dáng tương tự như loài rết nhiều chân, có khả năng bò di chuyển linh hoạt trên các địa hình đồi núi mấp mô phức tạp, hiện đang được cấu hình thử nghiệm phục vụ cho các tác vụ nhổ cỏ dại nông nghiệp tự động.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052502.webp)

（5）Một công bố nghiên cứu khoa học mới đây chỉ ra rằng hoạt động **viết tay bằng bút vẽ** giúp gia tăng đáng kể mức độ hoạt động và khả năng kích thích của tế bào não bộ so với thao tác gõ bàn phím máy tính thông thường, hỗ trợ tốt hơn cho năng lực ghi nhớ và tiếp thu kiến thức. Vì vậy khi cần học tập các nội dung quan trọng, các bạn nên ưu tiên sử dụng phương án ghi chép tay truyền thống.

## 文章

1、[Phân tích các giải pháp thay thế tối ưu cho thuộc tính class trong CSS](https://www.keithcirkel.co.uk/css-classes-considered-harmful/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061703.webp)

Tác giả chia sẻ quan điểm phân tích những hạn chế về mặt cấu trúc khi lạm dụng thuộc tính class của phần tử web, đồng thời giới thiệu các giải pháp viết CSS thay thế thông minh mang lại nhiều tư duy lập trình mới mẻ cho lập trình viên frontend.

2、[Hướng dẫn xây dựng hệ thống tự động gửi tin nhắn SMS dự báo thời tiết hằng ngày](https://bensilverman.co.uk/posts/daily-weather-sms/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061504.webp)

Bài hướng dẫn lập trình chi tiết các bước kết nối dịch vụ để tự động gửi thông tin cập nhật thời tiết mỗi sáng về số điện thoại cá nhân thông qua giao thức tin nhắn SMS.

3、[Giải pháp tối ưu hóa tính năng tìm kiếm lịch sử câu lệnh trên terminal](https://tratt.net/laurie/blog/2025/better_shell_history_search.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032608.webp)

Bài hướng dẫn cấu hình giúp lập trình viên tối ưu hóa tính năng tìm kiếm lịch sử các câu lệnh (Shell History Search) trên cửa sổ dòng lệnh terminal nhanh chóng và tiện lợi hơn.

4、[Giới thiệu 3 tiện ích mở rộng giúp nâng cao hiệu quả sử dụng NotebookLM](https://www.xda-developers.com/notebooklm-chrome-extensions/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061502.webp)

Ứng dụng ghi chú thông minh NotebookLM của Google đang nhận được sự quan tâm lớn. Bài viết giới thiệu 3 tiện ích mở rộng chất lượng trên Chrome giúp người dùng tối ưu hóa quy trình nhập dữ liệu và khai thác tính năng của công cụ này tốt hơn.

5、[Lịch sử đằng sau quyết định đổi tên từ giao thức bảo mật SSL sang TLS](https://tim.dierks.org/2014/05/security-standards-and-name-changes-in.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061602.webp)

Giao thức mã hóa bảo mật đường truyền HTTP vốn quen thuộc với tên gọi SSL sau đó đã được chuẩn hóa đổi tên thành TLS. Tác giả bài viết chia sẻ những câu chuyện hậu trường thú vị chỉ ra nguyên nhân đổi tên thực chất là kết quả của cuộc chiến tranh giành ảnh hưởng thương hiệu giữa các tập đoàn công nghệ lớn thời kỳ đó.

6、[Cách thức khai thác thuộc tính viewport chuẩn xác cho thiết kế web thích ứng (Responsive Web Design)](https://lukeplant.me.uk/blog/posts/you-can-stop-using-user-scalable-no-and-maximum-scale-1-in-viewport-meta-tags-now/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024101509.webp)

Để trang web hiển thị tối ưu trên màn hình di động, lập trình viên thường chèn các câu lệnh viewport trong thẻ head. Bài viết phân tích các lỗi thông dụng và hướng dẫn cách thức viết câu lệnh viewport chuẩn xác nhất hiện nay để bảo đảm trải nghiệm cho người dùng.

## 工具

1、[Cap.js](https://github.com/tiagorangel1/cap)

Công cụ nhận diện bot truy cập trang web mã nguồn mở hoạt động như một giải pháp thay thế CAPTCHA, vận hành dựa trên thuật toán SHA-256 Proof-of-Work chạy trực tiếp trên trình duyệt máy khách.

2、[Quartz](https://github.com/jackyzha0/quartz)

Trình biên dịch và xuất bản kho ghi chú Markdown cá nhân thành trang web tĩnh (Static Site Generator), được đánh giá là giải pháp thay thế tự chủ hoàn hảo cho dịch vụ trả phí Obsidian Publish.

3、[somo](https://github.com/theopfr/somo)

Công cụ dòng lệnh gọn nhẹ dành cho hệ điều hành Linux hỗ trợ kiểm tra nhanh các tiến trình phần mềm đang chiếm dụng các cổng kết nối mạng (ports).

4、[OOMOL Studio](https://github.com/ruanyf/weekly/issues/7029)

Môi trường phát triển tích hợp (IDE) sáng tạo dành cho máy tính để bàn, cho phép người dùng đóng gói các đoạn code chức năng tự viết thành các nút khối trực quan, sau đó sử dụng giao diện kéo thả đồ họa để kết nối các nút này thành một quy trình xử lý công việc tự động (workflows). (Đóng góp từ [@BlackHole1](https://github.com/ruanyf/weekly/issues/7029))

5、[Cực Trắc (极测)](https://www.jicesys.com/)

Bộ công cụ hỗ trợ kiểm thử giao tiếp mạng miễn phí hỗ trợ các kỹ sư mô phỏng và kiểm tra kết nối truyền nhận dữ liệu trên nhiều giao thức thông dụng như UDP, TCP, Serial Port, WebSocket, ZeroMQ... (Đóng góp từ [@seasonlaw](https://github.com/ruanyf/weekly/issues/7032))

6、[container](https://github.com/apple/container)

Công cụ dòng lệnh chính thức do Apple phát hành hỗ trợ người dùng macOS khởi chạy trực tiếp các container Linux gốc mà hoàn toàn không bắt buộc phải cài đặt ứng dụng Docker Desktop cồng kềnh.

7、[DarkFlare](https://github.com/doxx/darkflare)

Công cụ dòng lệnh giúp mã hóa và ngụy trang toàn bộ các luồng dữ liệu truyền nhận dạng TCP thành các gói tin HTTPS thông dụng khi đi qua mạng CDN nhằm tăng cường tính bảo mật thông tin.

8、[JDownloader](https://jdownloader.org/)

Trình quản lý tải tệp tin đa nền tảng mã nguồn mở mạnh mẽ. Tham khảo thêm [bài hướng dẫn chi tiết](https://www.xda-developers.com/raspberry-pi-downloading-device-entire-network/) để biến chiếc máy tính nhúng Raspberry Pi thành một máy chủ tải tệp tự động hoạt động 24/7 cho cả gia đình.

9、[Pydoll](https://github.com/autoscrape-labs/pydoll)

Thư viện Python chuyên dụng hỗ trợ lập trình điều khiển tự động trình duyệt Chrome thông qua giao thức Chrome DevTools Protocol trực tiếp trên máy tính cục bộ.

10、[Chili3D](https://github.com/xiangechen/chili3d)

Dự án phần mềm hỗ trợ vẽ kỹ thuật thiết kế 3D CAD hoạt động mượt mà ngay trên giao diện trình duyệt web được chia sẻ mã nguồn mở hoàn toàn.

## 资源

1、[Daily arXiv AI Enhanced](https://github.com/dw-dengwei/daily-arXiv-ai-enhanced)

Hệ thống tự động quét các bài báo khoa học mới công bố hằng ngày trên chuyên trang arXiv, sử dụng AI để tự động tóm tắt nội dung cốt lõi và xuất bản lên trang giao diện GitHub Pages trực quan cho người đọc. (Đóng góp từ [@dw-dengwei](https://github.com/ruanyf/weekly/issues/7052))

2、[Bản đồ trực quan mạng lưới tàu điện ngầm các thành phố Trung Quốc](https://subway.cuvii.dev)

Trang web bản đồ tương tác hiển thị chi tiết mạng lưới các tuyến tàu điện ngầm tại các đô thị lớn của Trung Quốc, dự án [chia sẻ mã nguồn mở tại GitHub](https://github.com/thecuvii/subway). (Đóng góp từ [@thecuvii](https://github.com/ruanyf/weekly/issues/7064))

3][Thiings](https://www.thiings.co)

Trang thư viện hỗ trợ tìm kiếm và tải về hơn 3.000 mẫu biểu tượng thiết kế định dạng 3D (3D Icons) hoàn toàn miễn phí phục vụ công tác thiết kế giao diện.

4、[Chứng minh không lời (Proofs without words)](https://artofproblemsolving.com/wiki/index.php/Proofs_without_words)

Trang thư viện tổng hợp các hình vẽ minh họa toán học giúp chứng minh các định lý, công thức toán học một cách trực quan sinh động mà không cần dùng đến các dòng chữ giải thích rườm rà. Hình ảnh phía trên là minh họa trực quan chứng minh công thức: Tổng của n số lẻ đầu tiên luôn bằng n bình phương.

## 图片

1、[Bảng xếp hạng quy mô thành viên của các subreddits lớn trên Reddit](https://www.visualcapitalist.com/ranked-largest-communities-on-reddit/)

Diễn đàn Reddit là cộng đồng trực tuyến lớn nhất tại Mỹ, được phân chia thành hàng vạn các kênh thảo luận chuyên đề nhỏ (subreddits) hoạt động tương tự như mô hình các bang hội trên các diễn đàn trực tuyến lớn.

Bảng thống kê phía dưới ghi nhận quy mô thành viên của các subreddits lớn nhất trên hệ thống:

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061803.webp)

Nếu mới tiếp cận diễn đàn và chưa rõ nên theo dõi kênh nào, các bạn có thể bắt đầu khám phá từ các subreddits dẫn đầu này, tiêu biểu như kênh giải trí hài hước [r/funny](https://www.reddit.com/r/funny/) đang đứng ở vị trí số một.

2、[Thương vụ đầu tư kỳ lạ trị giá 14,3 tỷ USD của tập đoàn Meta](https://www.facebook.com/groups/gaitech/permalink/1415307136320164/)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061806.webp)

Biểu đồ phía trên liệt kê 5 thương vụ thâu tóm và đầu tư có quy mô lớn nhất lịch sử của tập đoàn Meta (Facebook trước đây).

Trong đó, thương vụ lớn thứ hai vừa được hoàn tất tuần trước ghi nhận một cấu trúc giao dịch vô cùng kỳ lạ và hiếm thấy trong giới công nghệ.

Meta đã chi tới 14,3 tỷ USD đầu tư vào công ty AI Scale AI để sở hữu một lượng nhỏ cổ phần của doanh nghiệp này, đồng thời đưa ra điều kiện yêu cầu nhà sáng lập kiêm CEO 28 tuổi của Scale AI là Alexandr Wang từ chức để đầu quân trực tiếp cho Meta dẫn dắt bộ phận nghiên cứu AI của hãng.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061807.webp)

Nói cách khác, Meta thực chất đã chấp nhận chi ra khoản tiền khổng lồ 14,3 tỷ USD chỉ để chiêu mộ duy nhất một nhân tài kiệt xuất là Alexandr Wang về làm việc cho mình. Mức giá chi trả cho các nhân sự đỉnh cao trong cuộc đua AI hiện nay thực sự làm chấn động giới công nghệ.

## 文摘

1、[Tầm quan trọng của những "công việc chất keo" (Glue Work) trong tổ chức](https://www.seangoedecke.com/glue-work-considered-harmful/)

Khái niệm "công việc chất keo" (Glue Work) được dùng để chỉ toàn bộ các đầu việc phụ trợ giúp kết nối các thành viên, tối ưu hóa quy trình làm việc và hỗ trợ gián tiếp để tạo nên sản phẩm hoàn thiện.

Các ví dụ điển hình của công việc chất keo bao gồm: Cập nhật và bổ sung tài liệu kỹ thuật, xử lý các khoản nợ kỹ thuật (Technical Debt) tồn đọng, đào tạo và hướng dẫn nhân sự mới gia nhập, duy trì và cải thiện luồng thông tin giao tiếp giữa các phòng ban... Mọi đội ngũ kỹ thuật đều đòi hỏi phải có một lượng lớn các đầu việc này để vận hành trơn tru.

Dưới góc nhìn cá nhân, **tôi đánh giá các công việc chất keo này đóng vai trò vô cùng quan trọng. Thiếu đi chất keo kết dính này, một tập thể rất khó có thể hoàn thiện được các sản phẩm phần mềm quy mô lớn, và không thể giảm thiểu các ma sát vận hành trong một tổ chức lớn**.

Tuy nhiên nhiều kỹ sư trẻ thường có cái nhìn khá ngây thơ khi dành phần lớn thời gian và tâm huyết của mình để cống hiến cho các công việc chất keo này. Đến thời điểm đánh giá thăng tiến hay xem xét tăng lương thưởng hằng năm, họ lại thường bị ban lãnh đạo ngó lơ do công ty có xu hướng ưu tiên ghi nhận các kỹ sư trực tiếp tạo ra các tính năng thương mại mang lại doanh thu rõ rệt cho sản phẩm (như phát triển tính năng mới).

Tại sao những cống hiến cho công việc chất keo lại không giúp bạn được thăng tiến trong sự nghiệp?

Liệu có phải do ban quản trị công ty quá yếu kém nên không nhận thức được giá trị thực tế của các công việc này mang lại? Tôi không nghĩ vậy.

**Lý do thực sự là doanh nghiệp cố tình không khen thưởng lớn cho công việc chất keo vì họ không muốn bạn ưu tiên nguồn lực cho nó, họ muốn bạn tập trung tối đa cho nhiệm vụ ra mắt sản phẩm**. Việc dọn dẹp các ma sát hệ thống rất vất vả. Nếu bạn là một nhân sự có năng lực giải quyết tốt các ma sát đó, công ty muốn bạn dành năng lực đó để thúc đẩy sản phẩm ra mắt nhanh hơn là việc ngồi tối ưu hóa quy trình nội bộ của đội ngũ.

Bạn bắt buộc phải nhận thức rõ ràng: **Giúp cho đội ngũ vận hành mượt mà hơn không phải là nhiệm vụ cốt lõi của bạn, nhiệm vụ thực sự của bạn là thực thi và hoàn thành các mục tiêu chiến lược do ban lãnh đạo áp xuống**.

Một thực tế vận hành ít được chia sẻ rộng rãi là: Thay vì nỗ lực duy trì hiệu suất hoạt động của đội ngũ ở mốc 100%, việc để đội ngũ vận hành ổn định ở mức hiệu suất khoảng 60% đôi khi lại là giải pháp tối ưu hơn cho tổ chức.

Điều này xuất phát từ hai nguyên nhân cốt lõi sau:

（1）Nếu liên tục duy trì hiệu suất hoạt động ở mốc 100%, các thành viên trong đội ngũ chắc chắn sẽ sớm rơi vào trạng thái kiệt sức (burnout), gây ảnh hưởng tiêu cực lâu dài cho toàn bộ tập thể.

（2）Giải pháp tốt nhất là để các thành viên quen với việc vận hành ở mức hiệu suất nền tảng cơ bản của doanh nghiệp thay vì tìm cách loại bỏ hoàn toàn các ma sát hệ thống trong ngắn hạn. Bởi trạng thái vận hành không ma sát đòi hỏi nguồn đầu tư tài nguyên cực kỳ lớn và không thể duy trì ổn định được lâu dài.

Hầu hết các tập đoàn công nghệ lớn hiện nay đều chỉ vận hành với hiệu suất thực tế dao động từ 20% đến 60% (quy mô doanh nghiệp càng lớn thì hiệu suất vận hành thực tế càng thấp). Động lực tăng trưởng của các tập thể lớn chủ yếu nằm ở việc mở rộng chiếm lĩnh thị phần chứ không nằm ở việc tối ưu hóa hiệu suất nội bộ, do đó ban lãnh đạo không quá bận tâm đến việc đẩy hiệu suất đội ngũ lên mốc tối đa. Ngược lại nếu có cá nhân kỹ sư nào tự nguyện cống hiến thời gian để kéo hiệu suất đội ngũ lên mốc 80% hay 90%, công ty sẽ vui vẻ tiếp nhận giá trị miễn phí đó nhưng sẽ không thiết lập các cơ chế để ghi nhận lâu dài vì họ biết sự cống hiến tự nguyện của cá nhân là không bền vững.

Do đó, kết luận rút ra là: Doanh nghiệp luôn cần một lượng công việc chất keo nhất định để gắn kết nhưng hoàn toàn không cần quá nhiều.

Là một nhà phát triển phần mềm thông minh, **bạn chỉ nên tham gia giải quyết các công việc chất keo ở mức độ chiến thuật ngắn hạn chứ tuyệt đối không được biến nó thành mục tiêu chiến lược dài hạn của sự nghiệp**.

Nghĩa là bạn nên coi các công việc chất keo là phần việc hỗ trợ thêm ngoài giờ, và mục tiêu tập trung cao nhất của bạn phải luôn là sự thành công thương mại của dự án. Bạn sẽ không nhận được phần thưởng thăng tiến lớn chỉ nhờ việc chăm chỉ dán keo cho đội ngũ, nhưng bạn chắc chắn sẽ được ghi nhận lớn khi dự án chung đi đến thành công.

## 言论

1、

Quy trình mua sắm phần mềm của các cơ quan chính phủ thường có chung một kịch bản: Chi ra những khoản ngân sách khổng lồ, thu hút vô số các bài viết đưa tin rầm rộ trên truyền thông, huy động lực lượng nhân sự tham gia đông đảo, nhưng cuối cùng hầu như không có một phần mềm nào thực sự đi vào vận hành hiệu quả. Người dùng cuối tại các cơ quan vẫn tiếp tục sử dụng Excel để xử lý mọi đầu việc hằng ngày và dùng PowerPoint để soạn thảo các tài liệu báo cáo.

-- *Bình luận của một độc giả trên Hacker News liên quan đến thương vụ Bộ Quốc phòng Mỹ chi 200 triệu USD mua sắm các mô hình AI của OpenAI*

2、

Dưới kỷ nguyên AI, bạn vẫn cần phải học lập trình nghiêm túc. Bởi để có được kết quả mong muốn, bạn bắt buộc phải có khả năng mô tả và ra lệnh chính xác cho AI, và việc thấu hiểu tường tận nguyên lý vận hành của máy tính sẽ là nền tảng giúp bạn viết ra các câu lệnh nhắc (prompts) chuẩn xác và tối ưu nhất.

-- *Andrew Ng (Ngô Ân Đạt), chuyên gia AI nổi tiếng thế giới, giáo sư Đại học Stanford chia sẻ*

3、

Liệu các phi hành gia có thực hiện việc giặt quần áo khi làm việc ngoài không gian vũ trụ hay không? Câu trả lời là hoàn toàn không.

Nguồn nước cung cấp trên Trạm Vũ trụ Quốc tế (ISS) là cực kỳ hạn chế và hệ thống hoàn toàn không được thiết kế tính năng giặt giũ. Trang phục của phi hành gia sau khi bị bẩn chỉ có hai lựa chọn: Hoặc là tiếp tục mặc, hoặc là thải bỏ trực tiếp. Toàn bộ lượng quần áo bẩn thải ra sẽ được gom lại và thiêu rụi hoàn toàn khi tàu chở rác đi vào bầu khí quyển Trái Đất.

-- *Trích bài viết 《Phi hành gia giặt đồ thế nào ngoài vũ trụ》*

4、

Tôi vô cùng lo ngại trong tương lai các nội dung báo chí chuyên sâu chất lượng sẽ dần bị suy tàn trên các phương tiện truyền thông chính thống. Thay vào đó các đoạn video ngắn 30 giây nông cạn sẽ lên ngôi thống trị, các chương trình chỉ hướng tới việc đáp ứng thị hiếu chung thấp nhất của đại chúng, ngập tràn các nội dung cổ xúy cho ngụy khoa học và mê tín dị đoan, và đặc biệt là sự trỗi dậy của một tư duy cổ vũ cho sự thiếu hiểu biết.

-- *Carl Sagan, nhà văn khoa học vũ trụ lỗi lạc người Mỹ chia sẻ (đoạn văn được ông biên soạn từ năm 1994)*

## 往年回顾

- Số #306: [Thảo luận về cơ chế tâm lý: Tại sao thông tin trực tuyến lại dễ gây nghiện như chất đường](https://www.ruanyifeng.com/blog/2024/06/weekly-issue-306.html)
- Số #256: [Khám phá bộ sưu tập những tác phẩm sáng tạo Lego độc đáo nhất thế giới](https://www.ruanyifeng.com/blog/2023/05/weekly-issue-256.html)
- Số #206: [Chia sẻ các giải pháp tâm lý giúp vượt qua các giai đoạn thất vọng và hoài nghi bản thân](https://www.ruanyifeng.com/blog/2022/05/weekly-issue-206.html)
- Số #156: [Thảo luận về bài toán khủng hoảng thiếu hụt card đồ họa và sự cạnh tranh chéo giữa các ngành công nghiệp](https://www.ruanyifeng.com/blog/2021/04/weekly-issue-156.html)

(Hết)
