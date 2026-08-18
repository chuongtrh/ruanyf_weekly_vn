# Bản tin chia sẻ công nghệ (Số 336): Đối diện với AI, Internet truyền thống đang suy tàn

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/6012) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025013001.webp)

Hệ thống đèn lồng trang trí rực rỡ sắc xuân đón Tết Nguyên Đán trên cây cổ thụ ở đường Chung Pháp, Chương Châu. (Nguồn: [Facebook](https://www.facebook.com/watch/?v=3865521307053699))

## 面对 AI，互联网正在衰落

Suốt những ngày qua, tâm điểm chú ý của giới truyền thông toàn cầu đều đổ dồn vào DeepSeek, khiến các sự kiện công nghệ quan trọng khác phần nào bị lu mờ.

Một trong những sự kiện vô cùng quan trọng mà tôi muốn nhắc đến là vào ngày 23 tháng 1, chỉ đúng 3 ngày sau khi DeepSeek công bố dòng mô hình R1, OpenAI đã chính thức ra mắt một công cụ AI hoàn toàn mới mang tên **Operator** (Trợ lý vận hành).

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025013006.webp)

Dưới góc nhìn của tôi, **sự ra đời của công cụ này rất có thể là hồi chuông báo hiệu cho sự suy tàn không thể tránh khỏi của thế giới Internet truyền thống**.

Operator sở hữu triết lý thiết kế khác biệt hoàn toàn so với các sản phẩm AI tạo sinh trước đó. Đây không đơn thuần là một công cụ tạo nội dung, mà là một đại lý tự động hóa (Computer-using Agent) có khả năng trực tiếp thao tác trên các giao diện trang web thay cho con người.

Bản demo giới thiệu của OpenAI cho thấy một kịch bản: Khi người dùng đưa ra yêu cầu: "Hãy vào trang web du lịch TripAdvisor để đặt tour du lịch Rome một ngày có lượt đánh giá tốt nhất giúp tôi", hệ thống AI sẽ tự động điều khiển trình duyệt truy cập và hoàn tất các thủ tục đặt chỗ mà người dùng hoàn toàn không cần phải mở hay chuyển dịch sang bất kỳ tab cửa sổ nào khác (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020201.webp)

Chúng ta hãy cùng suy ngẫm xem sự thay đổi này sẽ dẫn tới hệ quả gì?

Trước đây, khi có nhu cầu đặt một dịch vụ du lịch, quy trình thông thường của người dùng sẽ là: Truy cập Google gõ tìm kiếm địa chỉ TripAdvisor, truy cập vào trang web, tìm kiếm các gói tour Rome, đọc đối chiếu đánh giá của các công ty lữ hành và cuối cùng đưa ra quyết định đặt gói tour tối ưu nhất.

Đến nay, **toàn bộ các bước trung gian kể trên đã bị AI thay thế hoàn toàn**. Bạn không còn cần thiết phải trực tiếp truy cập Google, TripAdvisor hay trang web của các công ty lữ hành nữa, bởi AI đã đảm nhận thay thế quy trình đó.

Trải nghiệm thực tế của người dùng sẽ dần dịch chuyển sang trạng thái: Tôi không còn cần quan tâm đến sự tồn tại của các website nguồn nữa, chỉ cần tương tác với AI là đã hoàn toàn đủ.

Năng lực xử lý của các hệ thống AI càng mạnh mẽ bao nhiêu thì vai trò hiển thị trực tiếp của các website nguồn sẽ ngày một mờ nhạt bấy nhiêu.

If các thế hệ AI tương lai đạt tới năng lực xử lý vạn năng, người dùng rất có thể sẽ không bao giờ cần phải trực tiếp lướt web nữa. Mọi yêu cầu mua sắm, đặt đồ ăn, đầu tư chứng khoán hay giải trí video đều có thể được ủy quyền trực tiếp cho AI thao tác từ đầu đến cuối.

Hệ quả tất yếu là: **Mô hình Internet hoạt động dựa trên sự hiển thị trực tiếp của các website truyền thống sẽ dần đi đến hồi kết**.

Tôi có đọc [một bài phân tích](https://brids.bearblog.dev/openai-just-put-the-final-nail-in-the-coffin-of-the-open-world-wide-web/) dự báo mô hình kinh doanh tương lai nhiều khả năng sẽ chuyển dịch sang trạng thái: Các nhà cung cấp dịch vụ sẽ không còn chú trọng đầu tư xây dựng các website đẹp mắt để trực tiếp tiếp cận người dùng nữa. Thay vào đó, họ sẽ chọn giải pháp bán dịch vụ của mình trực tiếp cho các hãng phát triển AI hoặc cung cấp các cổng kết nối API để hệ thống AI trả phí truy cập dữ liệu.

Thế giới Internet tương lai sẽ không còn được thiết kế để phục vụ trải nghiệm trực quan của con người, mà chuyển sang phục vụ khả năng đọc hiểu dữ liệu của AI. Rất có thể một tầng cấu trúc dữ liệu chuẩn hóa mới (structured data layer) sẽ ra đời để thay thế hoàn toàn cho các giao diện web hiện nay, được thiết kế chuyên biệt để các hệ thống AI truy xuất thông tin tối ưu nhất.

## 科技动态

**1、Biểu đồ nhiệt độ toàn cầu năm 2025**

Viện Nghiên cứu Biến đổi Khí hậu thuộc Đại học Maine (Mỹ) vận hành một chuyên trang trực tuyến hiển thị biểu đồ nhiệt độ trung bình toàn cầu được tích lũy trong suốt 50 năm qua.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025012204.webp)

Quan sát biểu đồ, đường cong màu cam nằm ở vị trí cao nhất chính là đường biểu diễn nhiệt độ trung bình toàn cầu ghi nhận trong năm 2024 vừa qua.

Năm 2024 đã được khoa học ghi nhận là năm nóng kỷ lục nhất trong lịch sử quan trắc khí tượng của nhân loại, do đó đường biểu diễn của nó luôn nằm tách biệt ở phía trên tất cả các năm trước đó.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025012205.webp)

Tuy nhiên, nếu phóng to khu vực góc dưới cùng bên trái của biểu đồ (hình trên), bạn sẽ nhận thấy có một đường biểu diễn ngắn màu nâu cà phê đang có xu hướng nằm ở vị trí cao hơn hẳn so với đường màu cam. Đó chính là số liệu nhiệt độ thực tế ghi nhận trong những ngày đầu năm 2025.

Điều này đồng nghĩa với việc nhiệt độ trung bình toàn cầu ghi nhận trong tháng 1 năm 2025 đã chính thức vượt qua mức kỷ lục của tháng 1 năm 2024, dự báo năm 2025 nhiều khả năng sẽ tiếp tục là một năm nắng nóng khắc nghiệt hơn nữa.

**2、Sự cố nhầm lẫn tên miền quốc gia**

Cơ quan thuế thành phố Basel (Thụy Sĩ) trong quá trình gửi thư thông báo khai thuế định kỳ đến người dân đã vô tình viết nhầm địa chỉ trang web khai thuế từ `esteuern.bs.ch` thành `esteuern.bs` (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020102.webp)

Nhân viên kỹ thuật đã bỏ sót hậu tố tên miền quốc gia Thụy Sĩ là `.ch`, vô tình biến địa chỉ cổng thông tin thành phố từ phân vùng `bs.ch` thành tên miền quốc gia của quốc đảo Bahamas ở vùng biển Caribe là `.bs`.

Tại thời điểm phát hiện ra sai sót, toàn bộ thư giấy thông báo đã được gửi đi đến tay người dân. Nhận thấy chi phí để in ấn và gửi lại thư đính chính là quá tốn kém, chính quyền thành phố đã quyết định giải pháp nhanh gọn hơn: Chi tiền mua đứt chính tên miền `.bs` của Bahamas đó.

Hệ quả là năm nay, toàn bộ người dân thành phố Basel sẽ thực hiện thủ tục khai thuế trên một địa chỉ tên miền thuộc quốc gia Bahamas.

**3、Hệ thống tản nhiệt card màn hình bằng dàn nóng điều hòa**

Cộng đồng công nghệ Trung Quốc tuần này đang chia sẻ rộng rãi một đoạn video ghi lại thử nghiệm độc đáo của một lập trình viên khi ứng dụng dàn nóng điều hòa gia đình để làm mát cho dòng card đồ họa cao cấp RTX 5090 vừa ra mắt.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020603.webp)

Thử nghiệm hoàn toàn không sử dụng đến block nén ga của điều hòa mà chỉ khai thác hệ thống quạt gió công suất lớn cùng các đường ống dẫn nhiệt bằng đồng của dàn nóng để làm bộ tản nhiệt cỡ lớn bên ngoài cho máy tính.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020604.webp)

Toàn bộ lượng nhiệt năng tỏa ra từ thùng máy sẽ được dẫn qua đường ống nước chảy về phía dàn nóng điều hòa ngoài trời để làm mát, sau đó dòng nước mát được bơm tuần hoàn quay trở lại máy tính.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020605.webp)

Các số liệu kiểm thử thực tế cho thấy hiệu năng tản nhiệt của giải pháp này đạt mức kinh ngạc.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020606.webp)

Ở trạng thái không tải trước khi kiểm thử, nhiệt độ bộ nhớ video (VRAM) chỉ ở mức 2 độ C và nhiệt độ nhân GPU ở mức 4 độ C. Khi tiến hành ép tải tối đa (stress test) đẩy công suất tiêu thụ lên tới 1000W liên tục trong suốt 40 phút, nhiệt độ của nhân GPU vẫn được duy trì ổn định ở mức dưới 30 độ C.

**4、Các tin tức khác**

(1) Nguyên mẫu máy bay chở khách siêu thanh thương mại đầu tiên do một doanh nghiệp tư nhân chế tạo đã thực hiện bay thử nghiệm thành công và chính thức vượt qua bức tường âm thanh (phá vỡ rào cản âm thanh).

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025012905.webp)

(2) Tập đoàn Google công bố nhờ ứng dụng các mô hình lọc thông minh bằng AI, trong năm qua hãng đã gỡ bỏ thành công hơn 2,36 triệu ứng dụng vi phạm chính sách khỏi kho ứng dụng Google Play và tiến hành khóa vĩnh viễn hơn 158.000 tài khoản nhà phát triển vi phạm. Xu hướng kiểm duyệt nội dung tương lai hứa hẹn sẽ được giao phó hoàn toàn cho AI đảm nhận tự động.

(3) Trình duyệt **Opera Air** vừa được phát hành chính thức, tích hợp tính năng tự động phát nhạc nền thư giãn theo hành vi lướt web của người dùng và đưa ra các gợi ý hướng dẫn vận động cơ thể định kỳ. Động thái phản ánh một thực tế rằng bản thân mảng công nghệ trình duyệt hiện đã bão hòa và rất khó để tạo nên các đột phá công nghệ cốt lõi mới.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020602.webp)

## 文章

1、[Phân tích một kịch bản phản hồi tư duy của mô hình DeepSeek R1](https://stephaniekelton.substack.com/p/the-impact-of-25-tariffs-on-canadian) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025012911.webp)

Mô hình DeepSeek R1 hỗ trợ hiển thị chi tiết toàn bộ chuỗi tư duy (reasoning process) trong quá trình xử lý câu hỏi. Tác giả đã đặt câu hỏi kiểm thử: "Việc Mỹ áp thuế quan 25% lên hàng hóa Canada sẽ gây ra những tác động cụ thể nào đến tổng sản phẩm quốc nội (GDP) của Canada?".

Câu trả lời giải thích của DeepSeek R1 được kết xuất mạch lạc như một bài luận chuyên sâu ngành kinh tế học, và mô hình chỉ mất vỏn vẹn 12 giây để hoàn thành toàn bộ chu kỳ "suy nghĩ" của mình.

2、[Phương pháp xây dựng hệ thống tìm kiếm hình ảnh tương đồng của Canva](https://www.canva.dev/blog/engineering/image-replacement-in-canva-designs-using-reverse-image-search/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025012910.webp)

Bài viết chia sẻ về giải pháp kỹ thuật của đội ngũ kỹ sư Canva khi ứng dụng công nghệ vector hóa dữ liệu (vector embeddings) để xây dựng hệ thống tìm kiếm hình ảnh tương đồng hiệu năng cao phục vụ người dùng thiết kế.

Một bài viết chia sẻ về giải pháp kỹ thuật tương đương khác là [《Hướng dẫn xây dựng hệ thống tìm kiếm thông tin phim ảnh theo ngữ nghĩa bằng pgvector và Next.js》](https://blog.6nok.org/building-a-semantic-movie-search-demo-with-pgvector-and-next.js/) cũng ứng dụng công nghệ cơ sở dữ liệu vector.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025013004.webp)

3、[So sánh hai giải pháp lưu trữ OpenMediaVault và TrueNAS Scale](https://www.xda-developers.com/openmediavault-vs-truenas-scale/) (tiếng Anh)

Đây là hai hệ điều hành máy chủ NAS mã nguồn mở phổ biến nhất hiện nay cho phép người dùng tự triển khai tại nhà. Bài viết so sánh chi tiết ưu nhược điểm của từng hệ thống để người dùng lựa chọn giải pháp phù hợp.

4、[Hướng dẫn cấu hình nhiều khóa SSH khác nhau cho cùng một tài khoản GitHub](https://stevenharman.net/configure-ssh-keys-for-multiple-github-accounts) (tiếng Anh)

Trong nhiều trường hợp, lập trình viên cần sử dụng các cặp khóa SSH khác nhau để tương tác bảo mật với các kho chứa (repositories) khác nhau trên GitHub. Bài viết hướng dẫn chi tiết cách biên soạn tệp cấu hình SSH trên máy tính để tự động hóa quy trình này.

5、[Lập luận: Hệ thống dấu trang tích hợp sẵn của trình duyệt vẫn là giải pháp tối ưu nhất](https://afewthingz.com/browserbookmark) (tiếng Anh)

Tác giả chia sẻ quan điểm cá nhân chứng minh tính hiệu quả và sự tiện lợi của hệ thống quản lý dấu trang (bookmarks) mặc định của các trình duyệt so với các ứng dụng quản lý bên thứ ba rườm rà khác.

6、[Tìm hiểu cơ chế hoạt động của quy trình bắt tay 3 bước trong giao thức TCP](https://www.pixelstech.net/article/1727412048-Why-TCP-needs-3-handshakes) (tiếng Anh)

Bài viết phân tích chuyên sâu giải thích chi tiết ý nghĩa kỹ thuật của quy trình 3 lượt truyền nhận tín hiệu (3-way handshake) bắt buộc để thiết lập một kết nối truyền tải dữ liệu an toàn theo giao thức TCP.

7、[Trải nghiệm nhập khẩu máy xúc điện mini từ Trung Quốc về Mỹ kinh doanh](https://electrek.co/2025/02/03/i-bought-a-container-full-of-chinese-electric-excavators-heres-what-showed-up/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020406.webp)

Một nhà kinh doanh người Mỹ chia sẻ câu chuyện thực tế về hoạt động nhập khẩu dòng máy xúc đất chạy điện cỡ nhỏ từ Trung Quốc về phân phối tại thị trường Mỹ. Những chiếc máy xúc mini này sở hữu thiết kế vô cùng nhỏ gọn trông giống như một món đồ chơi cỡ lớn.

## 工具

1、[Lightpanda](https://github.com/lightpanda-io/browser)

Dòng trình duyệt không đầu (headless browser) siêu nhẹ được thiết kế tối ưu cho việc tích hợp vào các bộ khung tự động hóa như Playwright hay Puppeteer. Nhà phát triển công bố công cụ giúp tiết kiệm tới 90% tài nguyên bộ nhớ và đạt tốc độ thực thi nhanh gấp 10 lần so với trình duyệt Chrome không đầu truyền thống.

2、[Dual-Link QR Code Generator](https://dualqrcode.com/)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025012601.webp)

Công cụ trực tuyến độc đáo hỗ trợ tạo mã QR tích hợp đồng thời hai liên kết khác nhau. Tùy thuộc vào góc nghiêng của camera khi quét, hệ thống sẽ trả về các địa chỉ liên kết khác nhau, dự án được [chia sẻ mã nguồn mở tại GitHub](https://github.com/zacharyreese/DualQRCode).

3、[isd](https://github.com/isd-project/isd)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025012909.webp)

Công cụ hỗ trợ quản trị và tương tác hệ thống `systemd` trên Linux trực quan thông qua việc cung cấp giao diện menu lựa chọn dòng lệnh tiện lợi. Xem thêm bài viết [hướng dẫn sử dụng](https://linuxiac.com/isd-is-a-new-tool-offering-a-user-friendly-approach-to-systemd-management/).

4、[changedetection.io](https://github.com/dgtlmoon/changedetection.io)

Hạ tầng dịch vụ mã nguồn mở hỗ trợ theo dõi và giám sát tự động các thay đổi trên một phân vùng chỉ định của trang web bất kỳ (ví dụ: tự động gửi cảnh báo qua email ngay khi phát hiện giá bán sản phẩm trên trang thương mại điện tử thay đổi).

5、[Internet Speed](https://www.internetspeed.my/)

Dịch vụ web hỗ trợ người dùng nhanh chóng đo đạc và kiểm tra tốc độ kết nối băng thông mạng trực tuyến tối giản và tiện lợi.

6、[Mô phỏng pháo hoa trực tuyến (在线焰火模拟器)](https://fireworks.visualized.fun/)

Trang web tương tác mô phỏng sinh động các hiệu ứng ánh sáng pháo hoa nở rộ đẹp mắt trực tiếp trên trình duyệt. (Đóng góp từ [@wincatcher](https://github.com/ruanyf/weekly/issues/5994))

7、[MultiPost](https://github.com/leaper-one/MultiPost-Extension)

Tiện ích mở rộng trình duyệt mã nguồn mở hỗ trợ nhà sáng tạo nội dung nhanh chóng đồng bộ hóa và xuất bản bài viết của mình lên nhiều nền tảng mạng xã hội khác nhau (như Zhihu, Weibo, Xiaohongshu, Douyin, Twitter, Facebook...) chỉ bằng một thao tác duy nhất. (Đóng góp từ [@tymon42](https://github.com/ruanyf/weekly/issues/6015))

8、[Sinh Tài Hữu Tích (Wealth Tracker)](https://github.com/nicejade/wealth-tracker)

Ứng dụng web mã nguồn mở hỗ trợ cá nhân tự phân tích, theo dõi và quản lý dòng tiền tài sản cá nhân một cách khoa học. (Đóng góp từ [@nicejade](https://github.com/ruanyf/weekly/issues/5996))

9、[StayFocused](https://github.com/daijinhai/StayFocused)

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020407.webp)

Ứng dụng cung cấp các âm thanh tiếng ồn trắng và âm thanh thiên nhiên mã nguồn mở giúp tăng cường sự tập trung khi làm việc. (Đóng góp từ [@daijinhai](https://github.com/ruanyf/weekly/issues/6023))

10、[MacVimSwitch](https://github.com/Jackiexiao/macvimswitch/)

Công cụ mã nguồn mở hỗ trợ người dùng macOS tự động cấu hình chuyển đổi bộ gõ ngôn ngữ thông minh theo từng ứng dụng đang làm việc chỉ định. (Đóng góp từ [@Jackiexiao](https://github.com/ruanyf/weekly/issues/6017))

## AI 相关

1、[AI as Workspace](https://github.com/NitroRCr/AIaW)

Bộ phần mềm client mã nguồn mở kết nối với các mô hình ngôn ngữ lớn, cung cấp giao diện quản trị Web UI trực quan và đầy đủ tính năng. (Đóng góp từ [@NitroRCr](https://github.com/ruanyf/weekly/issues/6011))

2、[podscript](https://github.com/deepakjois/podscript)

Chương trình viết bằng ngôn ngữ Go hỗ trợ ứng dụng AI để tự động nhận diện và chuyển đổi các tệp âm thanh giọng nói thành văn bản viết.

3、[Voice-Pro](https://github.com/abus-aikorea/voice-pro/blob/main/docs/README.zh.md)

Ứng dụng web cung cấp giao diện quản trị trực quan cho mô hình nhận diện giọng nói Whisper của OpenAI, hỗ trợ đa dạng các tác vụ như nhận diện tiếng nói, dịch thuật, sao chép giọng nói và chuyển đổi văn bản thành giọng đọc.

4、[Hacker News Wrapped](https://hn-wrapped.kadoa.com/)

Dịch vụ web vui vẻ: Người dùng chỉ cần nhập một tên tài khoản trên diễn đàn công nghệ Hacker News, hệ thống sẽ ứng dụng mô hình DeepSeek để tự động phân tích và viết một đoạn tóm tắt phác họa chân dung cá tính của thành viên đó vô cùng hài hước và chuẩn xác.

5、[GenSFX](https://gensfx.com)

Công cụ trực tuyến ứng dụng trí tuệ nhân tạo hỗ trợ người dùng tự thiết kế và tạo các hiệu ứng âm thanh (sound effects) hoàn toàn miễn phí. (Đóng góp từ [@andylearnai](https://github.com/ruanyf/weekly/issues/6016))

6、[Phúc Kỳ viết câu đối (福琪写春联)](https://cl.aixiaoke.cc/)

Ứng dụng web miễn phí sử dụng trí tuệ nhân tạo hỗ trợ soạn thảo và tạo các cặp câu đối đỏ chúc mừng năm mới ý nghĩa. (Đóng góp từ [@itfoxnet](https://github.com/ruanyf/weekly/issues/6002))

## 资源

1、[Cẩm nang hướng dẫn cấu hình Arch Linux dành cho người mới bắt đầu](https://ejmastnak.com/tutorials/arch/about/)

Chuỗi bài viết hướng dẫn chi tiết cách thức thiết lập và tối ưu hóa hệ điều hành Arch Linux từ các bước cơ bản nhất, được đánh giá là dễ tiếp cận hơn nhiều so với tài liệu Wiki chính thức của hệ điều hành.

2、[Cẩm nang hướng dẫn sử dụng công cụ Git của tác giả Beej](https://beej.us/guide/bggit/html/split/index.html)

Tài liệu hướng dẫn Git chất lượng cao mới nhất do chính nhà sư phạm nổi tiếng Beej biên soạn dựa trên các bài giảng thực tế dành cho sinh viên đại học chuyên ngành khoa học máy tính.

3、[MandoBot (Công cụ hỗ trợ học tiếng Trung trực quan)](https://mandobot.netlify.app/)

Một nhà phát triển nước ngoài đã xây dựng công cụ này giúp tự động phân tách cấu trúc các từ trong câu tiếng Trung và cung cấp phần dịch nghĩa từ vựng tiếng Anh tương ứng đi kèm giúp hỗ trợ đắc lực cho quy trình tự học ngoại ngữ.

## 图片

1、[Tính năng chuyển đổi ảnh không khí Tết bằng AI](https://www.sohu.com/a/849035825_121798711)

Dòng điện thoại thông minh vivo vừa giới thiệu tính năng chụp ảnh tết thông minh, cho phép hệ thống tự động nhận diện và chèn thêm các hoa văn trang trí không khí Tết Nguyên Đán ấm cúng vào bức ảnh chụp thông thường.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020408.webp)

Bức ảnh bên trái hiển thị ảnh chụp gốc và bức ảnh bên phải hiển thị kết quả sau khi được AI xử lý chèn thêm các họa tiết trang trí tết sinh động.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020409.webp)

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020410.webp)

2、[Mô hình trạm phát điện sử dụng ống khói mặt trời](https://hackaday.com/2024/01/15/solar-chimneys-viable-energy-solution-or-a-lot-of-hot-air/)

Hạ tầng phát điện năng lượng mặt trời hiện nay chủ yếu ứng dụng các tấm pin quang năng để chuyển đổi trực tiếp quang năng thành điện năng.

Tuy nhiên trong lịch sử phát triển, các kỹ sư thời kỳ đầu từng thử nghiệm giải pháp phát điện năng lượng mặt trời thông qua các ống khói khổng lồ.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072605.webp)

Cơ chế vật lý dựa trên hiện tượng luồng không khí nóng luôn có xu hướng bốc lên cao. Bằng cách thiết lập nhà kính xung quanh để mặt trời làm nóng không khí, luồng khí nóng sẽ di chuyển với tốc độ cao thoát ra ngoài qua đường ống khói khổng lồ dựng ở trung tâm, tạo lực xoay thúc đẩy tuabin phát điện đặt ở đáy ống khói vận hành.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072606.webp)

Vào năm 1982, Tây Ban Nha đã triển khai vận hành một trạm phát điện thực tế theo mô hình này với tháp ống khói cao tới 194 mét, bao quanh bởi khu nhà kính thu nhiệt có đường kính lên tới 244 mét.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072607.webp)

Tuy nhiên, công suất phát điện thực tế thu về của trạm chỉ đạt khoảng 50 kW. Công trình vận hành trong vòng 7 năm trước khi bị sụp đổ hoàn toàn do một trận bão lớn vào năm 1989.

Hệ quả là do hiệu suất phát điện quá thấp trong khi yêu cầu diện tích mặt bằng xây dựng quá lớn cùng chi phí dựng tháp tốn kém, giải pháp công nghệ này đã nhanh chóng bị khai tử ngay khi các tấm pin quang năng ra đời.

## 文摘

1、[Mối lo ngại về thế hệ lập trình viên bị mù công nghệ do phụ thuộc vào AI](https://nmn.gl/blog/ai-illiterate-programmers)

Tôi đã duy trì thói quen viết code cộng tác cùng AI trong suốt một thời gian dài, và đến thời điểm hiện tại, tôi nhận ra bản thân mình hầu như không thể tự mình giải quyết tốt bất kỳ sự cố lập trình nào nếu thiếu đi sự trợ giúp của AI.

Tôi đã hoàn toàn từ bỏ thói quen đọc các tài liệu hướng dẫn kỹ thuật (documentation). Bởi lẽ chỉ cần hỏi AI là sẽ lập tức nhận được câu trả lời giải thích cặn kẽ, vậy tại sao phải mất công tự mình đi đọc tài liệu?

Năng lực gỡ lỗi (debugging) của tôi đang ngày một mai một nghiêm trọng. Tôi thậm chí không còn thèm đọc nội dung của các thông báo lỗi hiển thị trên màn hình nữa, mà chỉ đơn thuần sao chép toàn bộ chúng dán vào khu vực chat của AI để nhận câu trả lời giải thích cơ chế lỗi.

Tôi dần biến thành một cỗ máy sao chép dán vật lý — một trung gian truyền tải dữ liệu thuần túy giữa mã nguồn và AI.

Trước đây, mỗi một thông báo lỗi gặp phải đều là cơ hội tuyệt vời để tôi tự học tập nâng cao kiến thức hệ thống. Nhưng bối cảnh hiện nay thì sao? AI đưa ra giải pháp sửa lỗi ăn liền, tôi gán vào và hệ thống chạy được, nhưng bản thân tôi hoàn toàn không tích lũy thêm được bất kỳ kiến thức mới nào. Sự kích thích dopamine tức thời do câu trả lời ăn liền mang lại đã thay thế hoàn toàn niềm vui sướng của cảm giác thấu hiểu bản chất vấn đề trước đây.

Mức độ thấu hiểu sâu sắc bản chất hệ thống của tôi cũng bị suy giảm nghiêm trọng. Trước đây, tôi có thể dành hàng giờ liền để nghiên cứu tại sao một giải pháp lập trình lại có thể hoạt động hiệu quả. Hiện nay, tôi chỉ đơn thuần áp dụng rập khuôn theo gợi ý của AI. Nếu gợi ý đó không hoạt động, tôi tiếp tục cung cấp thêm ngữ cảnh để yêu cầu AI đưa ra gợi ý khác. Chu trình này khiến mức độ phụ thuộc của tôi vào AI ngày càng tăng cao theo cấp số nhân.

Trạng thái cảm xúc khi làm việc của tôi cũng bị ảnh hưởng tiêu cực. Trước đây, việc tự mình mày mò giải quyết các bài toán lập trình hóc búa là niềm vui cốt lõi của công việc. Hiện nay, chỉ cần AI không thể kết xuất ra giải pháp sửa lỗi tối ưu trong vòng 5 phút, tôi sẽ lập tức cảm thấy vô cùng ức chế và chán nản.

Tôi nên làm gì để thoát khỏi tình trạng này? Việc quyết định từ bỏ hoàn toàn các công cụ AI là điều hoàn toàn không thực tế trong bối cảnh hiện nay. Tôi quyết định sẽ thiết lập quy tắc tự rèn luyện bản thân bằng cách duy trì định kỳ một ngày "Nói không với AI" hằng tuần.

Chiêm nghiệm thực tế của tôi là: AI không thực sự biến chúng ta thành những siêu lập trình viên có năng suất làm việc gấp 10 lần, mà nó chỉ đơn thuần khiến mức độ phụ thuộc của chúng ta vào nó tăng lên gấp 10 lần mà thôi.

Mỗi khi chúng ta lười biếng giao phó việc giải quyết các bài toán mà bản thân hoàn toàn có khả năng tự giải quyết cho AI, chúng ta đang đánh đổi năng lực hiểu biết sâu sắc dài hạn để lấy hiệu suất làm việc ngắn hạn trước mắt, hay nói cách khác là tự tay triệt tiêu năng lực phát triển của bản thân ngày mai để đổi lấy sự nhàn hạ của ngày hôm nay.

Lời khuyên của tôi hoàn toàn không phải là từ bỏ AI, mà là khuyến nghị các bạn lập trình viên trẻ đừng bao giờ từ bỏ nỗ lực tự mình suy nghĩ giải quyết các bài toán thực tế trước tiên.

Chúng ta đang vô tính đào tạo nên một thế hệ lập trình viên mới chỉ biết cách đặt câu hỏi đúng cho AI nhưng lại hoàn toàn không có khả năng đọc hiểu và đánh giá chất lượng câu trả lời của AI. Để rồi mỗi khi hệ thống AI gặp sự cố mất kết nối, họ sẽ lập tức rơi vào trạng thái hoàn toàn bất lực. Cho đến thời điểm hiện tại, AI vẫn chưa đủ năng lực để thay thế hoàn toàn con người, nhưng nếu xu hướng phụ thuộc này tiếp tục diễn ra, kịch bản đó chắc chắn sẽ ngày một tồi tệ hơn.

## 言论

1、

Chi phí vận hành dịch vụ của DeepSeek hiện đang rẻ hơn gấp 15 lần so với dòng mô hình Claude 3.5 Sonnet. Đối với OpenAI và Microsoft, mục tiêu chiến lược cốt lõi nhất hiện nay của họ là làm sao để ngăn cản việc DeepSeek tiếp tục cung cấp dịch vụ với mức giá hủy diệt như vậy trên thị trường.

Bởi lẽ OpenAI và Anthropic hiện đang phải áp mức phí dịch vụ rất cao nhằm mục đích duy trì các khoản quỹ lương khổng lồ cho nhân sự và chi phí R&D đắt đỏ. Trong khi đó, DeepSeek lựa chọn phát hành mã nguồn mở hoàn toàn miễn phí trọng số mô hình (weights), cho phép bất kỳ doanh nghiệp nào cũng có thể tự tải về để triển khai dịch vụ riêng, với khoản chi phí duy nhất chỉ là tiền điện vận hành phần cứng máy chủ.

-- *Ý kiến độc giả trên diễn đàn Hacker News*

2、

Ngay cả trong kịch bản DeepSeek biến mất khỏi thị trường vào ngày mai, thì do tính chất mã nguồn mở của dự án, các thành tựu của nó đã chính thức hòa chung vào dòng máu công nghệ toàn cầu, xác lập nên một cái neo về mặt chi phí (cost anchor) cho toàn bộ ngành công nghiệp AI.

Kể từ thời điểm này, các ông lớn AI sẽ không còn cơ hội xây dựng các rào cản độc quyền khép kín để thu lợi nhuận siêu ngạch nữa, và các mô hình lớn cũng sẽ mất đi giá trị khan hiếm thương mại vốn có của mình.

-- *Trích bài phân tích 《Làn sóng sốt AI chính thức hạ nhiệt》*

3、

Tôi chưa từng bao giờ nghĩ rằng bản thân mình sẽ bị công ty sa thải, bởi các chỉ số đánh giá hiệu quả công việc hằng năm của tôi luôn vượt qua các kỳ vọng của ban quản trị.

Tuy nhiên sau sự cố bị sa thải vừa qua, tôi đã thấu hiểu bản chất vấn đề. Trong các đợt tái cơ cấu cắt giảm nhân sự quy mô lớn, năng lực thực tế và những đóng góp của bạn cho doanh nghiệp hoàn toàn không phải là yếu tố quyết định. Trong hầu hết các trường hợp, quyết định sa thải được đưa ra hoàn toàn dựa trên các phép tính toán học của những người quản lý cấp cao thậm chí chưa từng biết mặt bạn.

Đối với doanh nghiệp, bản thân tôi chỉ đơn thuần đại diện cho một dòng số liệu vô hồn trên bảng tính Excel.

-- *Trích bài chia sẻ 《Sự cố sa thải đã thay đổi hoàn toàn tư duy của tôi》*

4、

Tập đoàn Apple hiện nay sở hữu năng lực kéo dài vòng đời thương mại của một dòng sản phẩm vô cùng xuất sắc, nhưng họ hầu như không còn trình diễn những ý tưởng điên rồ mang tính cách mạng nữa. Tổn thất lớn nhất kể từ khi Steve Jobs qua đời là việc Apple không còn dám thử nghiệm làm những điều kỳ lạ nữa.

-- *Chia sẻ của nhà phân tích công nghệ nổi tiếng vận hành kênh Asianometry*

5、

Cuộc sống của chúng ta càng bận rộn bao nhiêu thì bản thân chúng ta càng cảm nhận sâu sắc được sự tồn tại của cuộc sống bấy nhiêu, và từ đó hình thành nên nhiều chiêm nghiệm ý nghĩa hơn về cuộc đời.

—— *Immanuel Kant, nhà triết học người Đức nổi tiếng*

## 往年回顾

- Số #289: [Thảo luận về nguồn gốc hình thành tinh thần khoan dung trong lịch sử xã hội](https://www.ruanyifeng.com/blog/2024/02/weekly-issue-289.html)
- Số #239: [Dự báo về xu hướng gia tăng của hai nhóm đối tượng người dùng trong tương lai](https://www.ruanyifeng.com/blog/2023/01/weekly-issue-239.html)
- Số #189: [Phân tích về những ngành công nghiệp đối mặt với nguy cơ cạnh tranh khốc liệt (nội quyển) tiếp theo](https://www.ruanyifeng.com/blog/2021/12/weekly-issue-189.html)
- Số #139: [Đánh giá những bước tiến mang tính đột phá và đáng sợ của ngành sinh học](https://www.ruanyifeng.com/blog/2020/12/weekly-issue-139.html)

(Hết)
