# Bản tin chia sẻ công nghệ (Số 389): Phương thức tuyển dụng lập trình viên trong tương lai

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/9088) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022807.webp)

Đoàn tàu chạy trên đường ray trên cao mang phong cách cổ trang mang tên "Đại Đường Vân Xa" tại khu di sản phố cổ Hà Đầu, thành phố Đường Sơn. ([via](https://view.inews.qq.com/k/20260204A01P0P00))

## 未来如何招聘程序员

Cách đây vài ngày, tại khu vực thảo luận của bản tin có một [chủ đề đăng tải](https://github.com/ruanyf/weekly/issues/9238) đặt ra một câu hỏi vô cùng thực tế:

Nếu trong tương lai mọi dòng code đều do AI tự động viết ra, chúng ta sẽ tuyển dụng lập trình viên bằng cách nào?

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031406.webp)

Kỹ sư phần mềm là người chịu trách nhiệm về mã nguồn, nhưng mã nguồn lại do AI viết chứ không phải do kỹ sư tự tay gõ, vậy chúng ta nên thiết kế quy trình phỏng vấn kiểm tra ứng viên thế nào?

Nếu suy ngẫm kỹ, bạn sẽ thấy bài toán này khó hơn rất nhiều so với những hình dung ban đầu.

**Trước tiên, việc đánh giá năng lực tự viết code của ứng viên sẽ không còn là yếu tố quan trọng (vì code không phải do họ viết nữa), mà thay vào đó, điều cốt lõi là kiểm tra xem họ có kỹ năng sử dụng AI tốt hay không**. Chỉ cần ứng viên thành thạo việc khai thác AI để tạo ra các dòng code đạt yêu cầu, họ đã là một nhân sự chất lượng đối với doanh nghiệp.

Thế nhưng những câu hỏi phỏng vấn thế nào mới đủ sức đánh giá năng lực làm việc với AI của một lập trình viên? Dưới đây là một số ý tưởng câu hỏi mà tôi nghĩ ra:

- Hãy chuyển đổi một yêu cầu tính năng phức tạp của dự án thành một câu lệnh prompt chất lượng: yêu cầu cấu trúc rõ ràng, logic chặt chẽ và tập trung đúng vào các nút thắt kỹ thuật.
- Hãy mô tả một tình huống thực tế mà bạn đánh giá bắt buộc phải xây dựng các cấu phần Skill và tích hợp máy chủ dịch vụ MCP, đồng thời giải thích rõ nguyên lý hoạt động và phương pháp xây dựng các cấu phần đó.
- Làm thế nào để phân rã một dự án phần mềm quy mô lớn và thiết kế nên một cơ chế phối hợp hoạt động hiệu quả giữa nhiều AI Agents (multi-agent orchestration)?
- ...

Liệu các câu hỏi dạng này có thực sự giúp chúng ta sàng lọc ra các chuyên gia lập trình bằng AI giỏi hay không? Thực sự tôi hoàn toàn không dám chắc chắn.

**Thứ hai, bên cạnh kỹ năng sử dụng AI, nhà tuyển dụng cần đánh giá thêm những năng lực gì nữa?** Đây cũng là câu hỏi rất khó trả lời.

Có lẽ tôi vẫn sẽ hỏi thêm các câu hỏi về mặt kiến trúc hệ thống: ứng viên có thể không cần tự tay viết code, nhưng bắt buộc phải thấu hiểu phương pháp tổ chức cấu trúc mã nguồn để thiết kế nên một hệ thống phần mềm hoàn chỉnh. Tuy nhiên tôi cũng không chắc đây có phải là kỹ năng bắt buộc hay không, bởi các hệ thống phần mềm quy mô lớn do AI tự sinh ra sớm muộn cũng sẽ trở thành các hộp đen công nghệ (black boxes), và khi đó nhu cầu về kiến thức kiến trúc hệ thống của con người có thể cũng sẽ sụt giảm mạnh.

**Ngoài ra, tôi cũng sẽ yêu cầu ứng viên chia sẻ về các dự án thực tế họ từng làm trước đây**. Nếu ứng viên từng sử dụng AI để phát triển thành công các sản phẩm có tính năng tương tự, đó là một điểm cộng lớn. Tuy nhiên giải pháp đánh giá này cũng không hoàn toàn đáng tin cậy: số lượng các dự án có tính chất tương đồng hoàn toàn là cực kỳ ít, và với tốc độ tiến hóa thần tốc của AI hiện nay, các kinh nghiệm tích lũy từ hai năm trước có thể đã hoàn toàn lỗi thời ở thời điểm hiện tại.

Tóm lại, tôi nhận ra rất khó để xác định một bộ câu hỏi phỏng vấn nào là thực sự hiệu quả và đủ tin cậy để sàng lọc ra các ứng viên chất lượng. AI không chỉ tái định hình quy trình phát triển phần mềm, mà còn làm thay đổi hoàn toàn cách thức phỏng vấn lập trình viên. Các bạn có ý tưởng nào về các câu hỏi phỏng vấn hay hay không?

Có một thực tế chắc chắn là: **việc phỏng vấn kiểm tra các chi tiết cú pháp lập trình sẽ không còn nhiều giá trị nữa**, bởi lập trình viên không còn cần phải ghi nhớ máy móc các chi tiết cú pháp đó nữa mà hoàn toàn có thể tra cứu nhanh chóng qua các mô hình AI lớn.

## 科技动态

1. **Mascot chú bé Finder (Lil Finder Guy) độc đáo của Apple**

Hãng Apple vừa cho ra mắt dòng máy tính Macbook Neo, và nhiều người tinh ý đã phát hiện ra sự xuất hiện của một nhân vật biểu tượng (mascot) hoàn toàn mới trong các chiến dịch quảng cáo chính thức trên mạng xã hội TikTok của hãng (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031208.webp)

Ở góc trên bên trái của bức ảnh quảng cáo có xuất hiện hình ảnh một chú gấu bông đồ chơi có tạo hình rất lạ mắt chưa từng thấy trước đây.

Tạo hình của chú gấu bông này mô phỏng chân thực biểu tượng của công cụ quản lý tệp tin Finder trên hệ điều hành Mac, do đó cộng đồng mạng nhanh chóng đặt tên cho chú là "Chú bé Finder" (Lil Finder Guy).

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031209.webp)

Vài ngày sau đó, Apple tiếp tục sử dụng rộng rãi hình ảnh biểu tượng này trong một buổi phát sóng trực tiếp của hãng.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031210.webp)

Nhiều người bắt đầu đưa ra các dự đoán liệu đây chỉ là một hành động ngẫu hứng hay thực sự Apple đang lên kế hoạch chính thức ra mắt nhân vật này làm linh vật đại diện mới của hãng.

Cộng đồng mạng yêu công nghệ cũng nhanh chóng sử dụng AI để vẽ phác họa nên diện mạo hoàn chỉnh của "Chú bé Finder".

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031211.webp)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031212.webp)

Tạo hình của chú trông vô cùng đáng yêu và ngộ nghĩnh, rất có nét tương đồng với nhân vật đồ chơi nổi tiếng Labubu, hứa hẹn sẽ nhanh chóng tạo nên một cơn sốt yêu thích mới của giới công nghệ.

2. **Công nghệ truyền tin dữ liệu qua tia hồng ngoại**

Các nhà khoa học Anh vừa phát minh ra một giải pháp truyền thông tin hoàn toàn mới: sử dụng các điốt phát nhiệt bức xạ để truyền tải các tín hiệu số dưới dạng năng lượng nhiệt.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031401.webp)

Mắt thường của con người hoàn toàn không thể quan sát được tín hiệu này (bởi nó thuộc phổ tia hồng ngoại) và các thiết bị dò sóng vô tuyến thông thường cũng hoàn toàn bất lực trong việc phát hiện, tuy nhiên lượng nhiệt tỏa ra của chùm tia được mã hóa có thể được nhận diện rõ nét qua các thiết bị camera nhiệt hồng ngoại chuyên dụng (hình trên).

Do đó, giải pháp truyền tin này đòi hỏi máy thu phải trang bị camera nhiệt và kết nối với bộ giải mã tín hiệu trên máy tính. Công nghệ hứa hẹn sẽ mang lại nhiều giá trị ứng dụng thực tế trong các lĩnh vực công nghiệp chuyên dụng và quân sự quốc phòng.

3. **Tận dụng tủ rack máy chủ để trồng cây thủy canh**

Làm thế nào để tận dụng hiệu quả các thùng tủ rack máy chủ (server rack) cũ trong nhà khi không có nhu cầu sử dụng?

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031504.webp)

Một lập trình viên nước ngoài đã nảy ra ý tưởng độc đáo: tận dụng hệ thống cổng nguồn điện, các đường đi dây cáp và hệ thống kệ khay sẵn có trong tủ rack để thiết kế một hệ thống trồng cây thủy canh trong nhà.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031505.webp)

Anh đã mua thêm các dải đèn LED chuyên dụng để giả lập ánh sáng mặt trời chiếu sáng cho cây, đồng thời lắp đặt các bơm nước mini ở mỗi tầng khay để thiết lập hệ thống tự động cấp thoát nước nuôi cây.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031506.webp)

Nếu bạn có sở thích trồng cây cảnh trang trí trong nhà hoặc các loại thực vật đòi hỏi điều kiện chiếu sáng liên tục trong thời gian dài, giải pháp tận dụng các tủ rack máy chủ cũ thực sự là một phương án sáng tạo rất đáng để trải nghiệm.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031507.webp)

## 文章

1. [Lý do tôi chuyển đổi từ Elasticsearch sang Meilisearch](https://www.anisafifi.com/en/blog/i-ditched-elasticsearch-for-meilisearch-heres-what-nobody-tells-you/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031303.webp)

Bài viết giới thiệu về Meilisearch – một giải pháp tìm kiếm dữ liệu mã nguồn mở gọn nhẹ và tối ưu, đồng thời hướng dẫn phương pháp chuyển đổi thay thế cho hệ thống Elasticsearch cồng kềnh.

2. [Hồi ký về dự án khởi nghiệp AI viết code từ năm 2016](https://blog.youxu.info/2026/01/14/ai-codes-retrospective/) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031918.webp)

Tác giả Từ Hựu (Eric Xu) chia sẻ những hồi ức về dự án khởi nghiệp mảng AI viết code từ thời điểm năm 2016. Khi đó, nhóm của anh dự kiến cần khoản kinh phí 250.000 USD để huấn luyện mô hình AI lớn nhưng hoàn toàn bất lực trong việc tìm kiếm các nhà đầu tư mạo hiểm tin tưởng vào công nghệ này. (Đóng góp từ [@gengxiuli](https://github.com/ruanyf/weekly/issues/9296))

3. [Giải pháp thiết lập quy trình đọc phễu lọc thông tin trong kỷ nguyên quá tải dữ liệu](https://shawnxie.top/blogs/tools/read-flow-2026.html) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031914.webp)

Trước lượng thông tin khổng lồ cần tiếp cận hàng ngày, tác giả giới thiệu chi tiết quy trình xử lý thông tin cá nhân của mình, sử dụng AI làm màng lọc thông minh để trích xuất ra những nội dung thực sự giá trị đáng đọc nhất. (Đóng góp từ [@shawnxie94](https://github.com/ruanyf/weekly/issues/9282))

4. [Tìm hiểu về cấu trúc Front-end và Back-end của trình biên dịch](https://medium.com/packt-hub/the-world-of-compiler-backends-9b27a3e37866) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025050118.webp)

Bài viết khoa học phổ thông giới thiệu chi tiết các khái niệm và vai trò phân tách của cấu phần Front-end và Back-end bên trong các trình biên dịch mã nguồn hiện đại (như LLVM).

5. [Tìm hiểu về đơn vị kích thước chữ `lh` trong CSS](https://webkit.org/blog/16831/line-height-units/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025050125.webp)

Thông tin giới thiệu về đơn vị kích thước font chữ mới `lh` trong CSS, đại diện cho giá trị chiều cao dòng (line-height) của phần tử hiện tại phục vụ việc căn chỉnh giao diện chính xác hơn.

6. [Hành trình tìm kiếm loài hoa Đỗ Quyên Vương](https://blog.sciencenet.cn/home.php?mod=space&uid=52727&do=blog&id=1525508) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031302.webp)

Đỗ Quyên Cổ Thụ là giống đỗ quyên có kích thước thân gỗ cao lớn nhất thế giới, được một nhà thực vật học người Anh phát hiện lần đầu tiên tại tỉnh Vân Nam vào năm 1919.

Sau khi nhà thực vật học này qua đời tại Vân Nam, thông tin về vị trí phân bổ của loài cây quý này hoàn toàn bị thất lạc, và phải mãi đến tận năm 1982 các nhà nghiên cứu mới tìm thấy lại chúng tại khu bảo tồn núi Cao Lê Cống. Bài viết chia sẻ câu chuyện lịch sử thú vị về loài cây độc đáo này.

## 工具

1. [APTUI](https://github.com/mexirica/aptui)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031301.webp)

Ứng dụng giao diện terminal dành cho hệ điều hành Linux hỗ trợ quản trị viên quản lý và cài đặt các gói phần mềm APT trên Debian/Ubuntu trực quan.

2. [my.WordPress.net](https://my.wordpress.net/)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031502.webp)

Nếu bạn muốn trải nghiệm nhanh mã nguồn WordPress mà không muốn tốn chi phí thuê máy chủ, dịch vụ trực tuyến mới của WordPress chính là giải pháp tối ưu.

Hệ thống đã biên dịch toàn bộ mã nguồn PHP sang JavaScript để chạy native hoàn toàn phía client ngay trên trình duyệt web của bạn, bảo đảm an toàn dữ liệu cá nhân. Tham khảo thêm [bài viết giới thiệu chi tiết](https://wordpress.org/news/2026/03/announcing-my-wordpress/).

3. [GrobPaint](https://github.com/groverburger/grobpaint)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031503.webp)

Phần mềm chỉnh sửa hình ảnh mã nguồn mở đa nền tảng siêu nhẹ, hỗ trợ chạy mượt mà ngay trên trình duyệt hoặc biên dịch thành file thực thi nhị phân độc lập.

4. [Apple Matting](https://matting.lingxiangtools.top)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031407.webp)

Ứng dụng tách nền hình ảnh (tách vật thể/người) chuyên dụng cực nhẹ dành cho macOS với dung lượng cài đặt chỉ khoảng 8 MB. (Đóng góp từ [@pangxiaobin](https://github.com/ruanyf/weekly/issues/9241))

5. [HealthTick](https://github.com/lifedever/health-tick-release)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031409.webp)

Ứng dụng nhỏ chạy trên thanh menu bar của macOS có tính năng nhắc nhở người dùng đứng dậy vận động tránh ngồi làm việc quá lâu có hại cho sức khỏe. (Đóng góp từ [@lifedever](https://github.com/ruanyf/weekly/issues/9242))

6. [CheatReader](https://github.com/yaoyao2mm/cheatreader)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031501.webp)

Ứng dụng đọc sách đa nền tảng hỗ trợ chế độ cửa sổ nổi thu nhỏ dạng dòng đơn cực kỳ độc đáo, giải pháp tuyệt vời cho những ai có nhu cầu "đọc sách giải trí bí mật" ngay trong giờ làm việc. (Đóng góp từ [@yaoyao2mm](https://github.com/ruanyf/weekly/issues/9247))

7. [Thước kẻ di động (Web Note)](https://github.com/zhaoolee/notes)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031702.webp)

Giao diện ghi chú tối giản chạy web mô phỏng phong cách ứng dụng ghi chú nổi tiếng của hãng Smartisan, hỗ trợ gọi trực tiếp như một cấu phần Skill. (Đóng góp từ [@zhaoolee](https://github.com/ruanyf/weekly/issues/9274))

8. [WeChat Download API](https://github.com/tmwgsicp/wechat-download-api)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031917.webp)

Bộ công cụ mã nguồn mở hỗ trợ chuyển đổi các bài đăng từ WeChat Official Accounts sang định dạng dữ liệu cấp tin RSS tiện lợi. (Đóng góp từ [@tmwgsicp](https://github.com/ruanyf/weekly/issues/9295))

9. [Speech Speed](https://github.com/ywong137/speech-speed)

Tiện ích mở rộng Chrome độc đáo hỗ trợ tự động điều chỉnh tốc độ phát video dựa trên tốc độ nói của nhân vật: hệ thống tự động tăng tốc độ phát khi nhân vật nói chậm và giảm tốc độ khi nhân vật nói nhanh.

## AI 相关

1. [VibeGo](https://github.com/xxnuo/VibeGo)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031913.webp)

Trình soạn thảo mã nguồn tích hợp (Web IDE) mã nguồn mở hỗ trợ phong cách lập trình Vibe Coding, tích hợp sẵn các cổng kết nối đến Claude Code, Gemini CLI, CodeX và OpenCode. (Đóng góp từ [@xxnuo](https://github.com/ruanyf/weekly/issues/9281))

2. [Mimic Them](https://github.com/zhanchey/MimicThem)

Ứng dụng mã nguồn mở tận dụng mô hình hình ảnh Seedream của ByteDance để tự động tái tạo và sinh các bài đăng hình ảnh kèm chữ mô phỏng theo phong cách của mạng xã hội Xiaohongshu từ các bài đăng mẫu có sẵn. (Đóng góp từ [@zhanchey](https://github.com/ruanyf/weekly/issues/9215))

3. [AICheck](https://github.com/MatrixA/aicheck)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031305.webp)

Công cụ dòng lệnh viết bằng ngôn ngữ Rust hỗ trợ quét kiểm tra ngoại tuyến (offline) để phát hiện xem các tệp tin hình ảnh, video, âm thanh hay tài liệu văn bản có phải do AI tự động sinh ra hay không. (Đóng góp từ [@MatrixA](https://github.com/ruanyf/weekly/issues/9219))

4. [AionUi](https://github.com/iOfficeAI/AionUi)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031405.webp)

Dự án mã nguồn mở hỗ trợ tự động hóa các thao tác điều khiển trên máy tính, giải pháp thay thế rất tốt cho Cowork và OpenClaw. (Đóng góp từ [@cdxiaodong](https://github.com/ruanyf/weekly/issues/9236))

5. [Lumo](https://github.com/zhnd/lumo)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031408.webp)

Bảng quản trị hiển thị dữ liệu cục bộ dành cho công cụ Claude Code, hỗ trợ theo dõi chi tiết lượng tiêu thụ token, lịch sử phiên trò chuyện và thống kê các khung giờ lập trình trong ngày. (Đóng góp từ [@zhnd](https://github.com/ruanyf/weekly/issues/9239))

6. [AIComicBuilder](https://github.com/twwch/AIComicBuilder)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031704.webp)

Hệ thống tự động biên tập và dựng video anime bằng AI mã nguồn mở. Người dùng chỉ cần nhập kịch bản văn bản phân cảnh, hệ thống sẽ tự động thực hiện nhận diện nhân vật, thiết kế phân cảnh, sinh hình ảnh các khung hình khóa và tổng hợp xuất ra tệp video hoàn chỉnh. (Đóng góp từ [@twwch](https://github.com/ruanyf/weekly/issues/9275))

## 资源

1. [canirun.ai](https://www.canirun.ai/)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031402.webp)

Trang web hỗ trợ quét kiểm tra cấu hình thiết bị phần cứng máy tính của bạn để đưa ra danh sách các mô hình AI chạy local nào mà máy tính có khả năng vận hành được tốt.

2. [Sổ tay tìm hiểu về trí tuệ nhân tạo (whats_ai)](https://wmyskxz.cn/wiki/whats_ai/)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031304.webp)

Tài liệu hướng dẫn trực quan giới thiệu các nguyên lý hoạt động cốt lõi của công nghệ AI biên soạn bằng ngôn từ phổ thông dễ hiểu dành cho mọi đối tượng độc giả. (Đóng góp từ [@wmyskxz](https://github.com/ruanyf/weekly/issues/9218))

3. [Giáo trình cấu trúc dữ liệu và giải thuật bằng TypeScript](https://amoilanen.github.io/Algorithms-with-Typescript/preface.html)

Sách giáo khoa điện tử tiếng Anh chất lượng cao hướng dẫn người học thấu hiểu các kiến thức về cấu trúc dữ liệu và giải thuật trong lập trình thông qua việc minh họa bằng ngôn ngữ TypeScript.

4. [Giao diện xem tivi hoài cổ Channel Surfer](https://channelsurfer.tv)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031404.webp)

Trang web độc đáo giúp biến đổi giao diện xem video YouTube thành phong cách xem các kênh truyền hình tivi truyền thống đi kèm lịch phát sóng chi tiết cho từng kênh. Giải pháp tuyệt vời cho những ai đang băn khoăn không biết chọn xem gì trên YouTube.

## 图片

1. **Những巧思 kiến trúc trong các công trình cổ đại**

Do hạn chế về mặt máy móc cơ khí và nguồn động lực năng lượng, các kỹ sư thời kỳ cổ đại thường lồng ghép rất nhiều giải pháp thiết kế vô cùng thông minh vào các công trình:

（1）Vào thế kỷ 19 tại kênh đào Macclesfield của Anh, do thiết kế luồng nước không có độ dốc tạo dòng chảy tự nhiên, các tàu vận chuyển bắt buộc phải nhờ sức ngựa kéo dọc bờ để di chuyển.

Tại những đoạn đường đường dẫn ngựa kéo bắt buộc phải chuyển làn sang bờ đối diện sông, ngựa sẽ phải đi qua cầu vượt sông.

Để ngựa có thể đi qua cầu mà không cần phải thực hiện tháo dây cáp kéo tàu phức tạp, các kỹ sư đã thiết kế nên mẫu "Cầu rắn" (Snake Bridge) độc đáo, cho phép ngựa đi lên cầu và có khe rãnh chạy xuyên suốt dọc thân cầu để dây kéo đi qua thuận lợi:

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120205.webp)

（2）Hệ thống cối xay nước Barbegal tại miền Nam nước Pháp được xây dựng từ thế kỷ thứ 2 sau Công Nguyên.

Công trình được xây dựng men theo sườn dốc đồi núi, bao gồm chuỗi 16 bánh xe nước liên kết tuần hoàn để tận dụng triệt để động năng dòng nước đổ xuống. Hệ thống có công suất sản xuất lên tới 25 tấn bột mì mỗi ngày, được coi là khu xưởng sản xuất công nghiệp quy mô lớn đầu tiên của lịch sử Châu Âu.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120206.webp)

（3）Hệ thống cối xay gió cổ đại Nashtifan tại Iran được xây dựng liên hoàn trên các mái nhà. Trục gỗ trung tâm được gắn các lá buồm làm từ đất sét, rơm và gỗ định vị theo trục đứng. Sức gió mạnh của vùng sa mạc sẽ làm quay trục gỗ để vận hành cối xay nghiền ngũ cốc đặt ở các gian phòng phía dưới.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120208.webp)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120207.webp)

（4）Hệ thống đường ống dẫn nước bằng gốm từ thời kỳ Chiến Quốc được phát hiện tại di chỉ Thượng Lâm Uyển thuộc thời nhà Tần tại thành phố Tây An, hiện đang được lưu giữ trưng bày tại Bảo tàng Tây An.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120209.webp)

## 文摘

1. **Lời khuyên nên tránh tự xây dựng các "定制框架" (mini-frameworks) nội bộ**

Nhiều đội nhóm kỹ thuật quy mô nhỏ trong quá trình làm việc thường có xu hướng tự phát minh ra các "khung phát triển tùy chỉnh" (mini-frameworks) của riêng họ.

Họ xuất phát từ việc sử dụng các framework phổ biến trên thị trường nhưng cảm thấy có một vài điểm chưa thực sự tối ưu, từ đó đi đến quyết định tự xây dựng một phiên bản framework tùy chỉnh dựa trên nền tảng của framework cũ.

Các dòng framework tùy chỉnh nội bộ này thường sở hữu một số đặc điểm chung:

> （1）Được phát triển bởi các đội nhóm nhỏ nhằm giải quyết các bài toán cục bộ của họ;
>
> （2）Vẫn vận hành dựa trên nền tảng công nghệ của một framework phổ biến bên dưới;
>
> （3）Tự ý đưa vào nhiều khái niệm thuật ngữ kỹ thuật mới hoàn toàn chưa từng có trong framework cũ;
>
> （4）Nhóm phát triển luôn quảng cáo rằng framework tùy chỉnh này đã giải quyết một cách "kỳ diệu" rất nhiều vấn đề kỹ thuật và ra sức thuyết phục mọi người trong công ty sử dụng.

Từ kinh nghiệm thực tế của bản thân, tôi nhận thấy các framework tùy chỉnh nội bộ này thường cực kỳ khó sử dụng, do chúng bắt buộc phải nạp thêm hàng loạt khái niệm phức tạp mới để che đậy đi các gánh nặng kỹ thuật phát sinh bên dưới.

Tôi khuyên các lập trình viên nên tránh việc tự thiết kế các framework tùy chỉnh nội bộ vì các lý do sau:

（1）Các framework tùy chỉnh thường quảng cáo chúng giúp ẩn đi hoặc loại bỏ các "độ phức tạp không cần thiết" của framework cũ, nhưng thực tế hoàn toàn không làm được. Ngay cả khi framework tùy chỉnh xử lý rất tốt 80% các bài toán lập trình thông thường, thì do áp đặt các cú pháp thiết kế mới, 20% các tình huống đặc thù còn lại sẽ cực kỳ khó xử lý do mất đi tính linh hoạt và các tính năng mặc định của framework gốc.

（2）Khung phát triển tùy chỉnh cực kỳ khó thay đổi. Do thiết kế ban đầu chỉ hướng tới giải quyết các bài toán cụ thể của đội nhóm tại thời điểm đó, nên khi yêu cầu nghiệp vụ thay đổi trong tương lai, framework thường không kịp thích ứng. Thêm vào đó, framework tùy chỉnh thường can thiệp sâu vào các chi tiết cấu trúc bên trong của framework gốc, trong khi bản thân framework gốc luôn cập nhật thay đổi liên tục, việc can thiệp quá sâu sẽ khiến bạn gặp rất nhiều khó khăn trong việc cập nhật nâng cấp phiên bản framework gốc sau này.

（3）Framework tùy chỉnh mang đậm dấu ấn tư duy cá nhân của nhóm phát triển. Việc đội nhóm thấu hiểu sâu bài toán của mình là tốt, nhưng điều này vô hình trung làm cho triết lý thiết kế của framework không tương thích với mô hình tư duy của các lập trình viên khác khi tiếp cận hệ thống.

（4）Gây nên sự phân mảnh trong hệ thống công nghệ của doanh nghiệp. Bạn chỉ thay đổi được một phần nhỏ cấu trúc công nghệ liên quan trực tiếp đến mình, trong khi các mảng việc khác vẫn giữ nguyên. Cùng với thời gian và các lớp công nghệ mới đắp lên, hệ thống sẽ ngày càng cồng kềnh và cực kỳ khó khăn nếu có nhu cầu chuyển dịch toàn bộ hạ tầng công nghệ sau này.

（5）Thiếu sự bảo trì lâu dài. Các công nghệ phổ biến luôn được bảo trì bởi các tổ chức hoặc tập đoàn công nghệ chuyên nghiệp, trong khi các framework tùy chỉnh nội bộ thường chỉ được duy trì bởi một hoặc hai nhân sự sáng lập. Một khi những nhân sự này rời bỏ doanh nghiệp, hệ thống sẽ lập tức rơi vào trạng thái không có người tiếp quản bảo trì và nhanh chóng bị đào thải.

Tôi không có ý khuyên bạn tuyệt đối không nên tự viết framework của riêng mình, mà khuyến nghị nếu làm thì nên tuân thủ 3 nguyên tắc cốt lõi: (1) Cố gắng hạn chế tối đa việc đưa vào các khái niệm thuật ngữ mới, (2) Ưu tiên đóng gói mã nguồn dưới dạng thư viện (library) thay vì xây dựng framework, (3) Tuyệt đối không viết wrapper bọc ngoài các framework sẵn có, hãy tự xây dựng từ đầu nếu thực sự cần thiết.

## 言论

1.

Thế giới Internet lý tưởng mà tôi mong muốn hướng tới là một không gian số mà ở đó mọi thứ đều có tính linh hoạt cao, kích thích bản năng sáng tạo tự nhiên của mỗi người dùng để họ trở thành những nhà kiến tạo thực thụ.

-- David Miranda chia sẻ quan điểm

2.

Làn sóng công nghệ AI đang làm dịch chuyển các chi phí phát triển phần mềm từ mảng viết mã nguồn sang mảng xây dựng kịch bản kiểm thử và hoàn thiện tài liệu hướng dẫn. Giá trị thực tế của một bộ kịch bản kiểm thử chất lượng cao hiện nay thậm chí vượt trội hơn nhiều so với bản thân việc viết mã nguồn chương trình.

-- Trích chia sẻ trên trang blog lucumr.pocoo.org

3.

Bản chất cốt lõi của lập trình nằm ở năng lực trừu tượng hóa (abstraction) – tức khả năng tư duy logic và cấu trúc mã nguồn ở một cấp độ cao hơn hoàn toàn so với các lớp công nghệ phần cứng bên dưới.

-- Trích bài viết [《Góc nhìn về các lập trình viên đang sống trong thế giới phẳng Flatland》](https://blog.redplanetlabs.com/2025/11/24/the-programmers-who-live-in-flatland/)

4.

Nghệ thuật lãnh đạo thực chất là khả năng định hướng và thuyết phục người khác tự nguyện cống hiến hoàn thành công việc mà bạn mong muốn họ làm.

-- Tổng thống Mỹ Dwight D. Eisenhower chia sẻ chiêm nghiệm

## 往年回顾

[Phương thức gian lận phỏng vấn lập trình bằng công nghệ nhân vật số AI](https://www.ruanyifeng.com/blog/2025/03/weekly-issue-342.html) (#342)

[Mọi dòng code viết ra thực chất đều là một khoản nợ kỹ thuật (technical debt)](https://www.ruanyifeng.com/blog/2024/03/weekly-issue-292.html) (#292)

[Bài học đắt giá từ một sự cố máy chủ bị hacker xâm nhập](https://www.ruanyifeng.com/blog/2023/02/weekly-issue-242.html) (#242)

[Cơ hội phát triển lớn nhất luôn xuất phát từ các làn sóng công nghệ mới](http://www.ruanyifeng.com/blog/2022/01/weekly-issue-192.html) (#192)

(Hết)
