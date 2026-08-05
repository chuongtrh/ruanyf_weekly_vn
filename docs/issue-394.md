# 科技爱好者周刊（第 394 期）：第二次 API 开放浪潮 (Bản tin công nghệ hàng tuần số 394: Làn sóng mở rộng API lần thứ hai)

Ghi lại nội dung công nghệ đáng chia sẻ hàng tuần, phát hành vào thứ Sáu. (**Thông báo: Tuần sau là kỳ nghỉ lễ 1/5, bản tin sẽ tạm nghỉ một số.**)

Bản tin này [mã nguồn mở](https://github.com/ruanyf/weekly), hoan nghênh bạn [đóng góp](https://github.com/ruanyf/weekly/issues). Ngoài ra còn có dịch vụ [《Ai đang tuyển dụng》](https://github.com/ruanyf/weekly/issues/9454) đăng tải thông tin tuyển dụng lập trình viên. Hợp tác vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图 (Ảnh bìa)

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026042008.webp)

Tấm biển quảng cáo ấn tượng nhất tôi từng thấy, chỉ hiển thị đúng một dòng lệnh để quảng bá một bộ công cụ AI. Người bình thường không đọc hiểu được cũng không sao, vì nó vốn dĩ không dành cho họ. ([via](https://x.com/steventey/status/1689986179746197504))

## 第二次 API 开放浪潮 (Làn sóng mở rộng API lần thứ hai)

Nếu bạn làm việc trong ngành Internet đủ lâu, có lẽ bạn vẫn nhớ trước đây từng có một làn sóng mở rộng API đầu tiên.

Đó là thời điểm cách đây 15 năm (năm 2011), khi các dịch vụ đám mây (cloud services) vừa mới trỗi dậy, các nền tảng công nghệ lớn nhỏ thi nhau mở cổng kết nối API của mình.

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026042102.webp)

Lúc bấy giờ, cả Facebook và Twitter đều công bố API riêng để chia sẻ dữ liệu nền tảng. Thiết kế API của GitHub khi đó đẹp đẽ như một tác phẩm nghệ thuật, cho phép lập trình viên truy cập hầu như mọi tính năng mong muốn.

Ý tưởng của các nền tảng lúc đó là: Cung cấp API mở sẽ giúp thu hút người dùng và các bên thứ ba xây dựng các plugin, ứng dụng mở rộng (extension) phong phú, từ đó thúc đẩy sự phát triển của chính hệ sinh thái nền tảng, nâng cao tỷ lệ giữ chân và mức độ hài lòng của người dùng.

Thời kỳ đó còn có một trang web rất nổi tiếng mang tên [ProgrammableWeb](https://en.wikipedia.org/wiki/ProgrammableWeb) (nay đã đóng cửa). Bản thân cái tên của trang web đã đại diện cho đức tin lúc bấy giờ: Internet có thể lập trình được qua API để kết nối dữ liệu của mọi nền tảng lại với nhau.

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026042103.webp)

Tuy nhiên, mọi việc sau đó diễn ra hoàn toàn ngược lại.

Các nền tảng nhận thấy việc mở cổng API rất khó kiếm tiền do không thể chèn quảng cáo vào dữ liệu thô, đồng thời việc chia sẻ dữ liệu lại vô tình tiếp tay cho hoạt động kinh doanh của các đối thủ, dẫn đến chảy máu người dùng.

Thế là họ đồng loạt quay xe, thắt chặt và đóng cửa API, ngừng chia sẻ dữ liệu để giam lỏng người dùng bên trong "bức tường vườn nhà" của mình.

Ngày nay, API của Facebook và Twitter gần như chỉ còn là hình thức, và mọi ứng dụng client của bên thứ ba đều bị cấm triệt để. GitHub tuy vẫn duy trì API mở nhưng cũng áp dụng các biện pháp kiểm soát gắt gao, tăng cường xác thực và giới hạn tần suất gọi (rate limiting) khiến việc xây dựng một ứng dụng đầy đủ tính năng của bên thứ ba trở nên vô cùng khó khăn.

Đúng lúc mọi người tin rằng tình trạng đóng cửa này sẽ là trạng thái bình thường vĩnh viễn, thì một [bước ngoặt](https://brandur.org/second-wave-api-first) đã xuất hiện.

Vào nửa sau năm 2025, các mô hình ngôn ngữ lớn đã đạt đến điểm bùng nổ công nghệ, trở nên thực sự mạnh mẽ và có thể ứng dụng trực tiếp vào môi trường sản xuất thực tế.

Mọi người nhanh chóng nhận ra rằng, nếu mô hình AI chỉ biết tư duy mà không thể trực tiếp thực thi code thì giá trị mang lại không lớn. **Giá trị lớn nhất của AI không nằm ở việc tạo ra nội dung, mà nằm ở: Tạo nội dung + Tự động hóa**, chỉ có như vậy mới giải phóng tối đa sức lao động và tạo ra giá trị đột phá. Đại diện tiêu biểu cho xu hướng AI tự động hóa và tự thực thi code chính là công cụ "Long Lộ" (OpenClaw).

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026042104.webp)

Khả năng tự động hóa đồng nghĩa với việc AI bắt buộc phải gọi được dịch vụ từ các nền tảng khác, và điều đó lại dẫn tới việc các nền tảng khác bắt buộc phải mở cổng API của mình trước tiên.

Đột nhiên, API không còn là gánh nặng chi phí nữa, mà trở thành điều kiện tiên quyết để kết nối vào hệ sinh thái AI. Không có API, nền tảng của bạn sẽ bị gạt ra ngoài các luồng công việc của AI, và các AI Agent sẽ không thể thay mặt người dùng thực hiện thao tác trên nền tảng của bạn.

Giữa hai nền tảng có tính năng tương đương, bên nào có API mở sẽ được ưu tiên, còn bên đóng cửa sẽ sớm bị thị trường đào thải do AI không thể kết nối và tự động hóa công việc, buộc người dùng AI phải chuyển sang sử dụng sản phẩm đối thủ.

Các nền tảng lập tức nhận ra điều này: Bên nào mở cổng API trước sẽ giành được thế thượng phong. Vì thế, ngay cả ông lớn có hệ sinh thái đóng như Tencent cũng đã lập tức mở cổng kết nối WeChat ngay sau khi OpenClaw bùng nổ, cho phép Agent gửi tin nhắn trực tiếp vào WeChat.

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026042315.webp)

Tencent lo sợ rằng trong thế giới vận hành bởi OpenClaw sẽ không có chỗ đứng cho mình. Các nền tảng khác cũng không ngoại lệ, họ tranh nhau mở cổng kết nối thông qua giao thức MCP và Skill của AI.

Điều này chứng minh **làn sóng mở rộng API lần thứ hai đang ập đến**. Lần này, sự mở cửa sẽ triệt để hơn và dễ sử dụng hơn rất nhiều so với lần trước.

(1) Lần mở rộng này không chỉ giới hạn ở các dịch vụ đám mây, mà bao phủ mọi dịch vụ đời sống hàng ngày: Gọi đồ ăn, thương mại điện tử, dịch vụ ngân hàng... thậm chí cả các mảng trước đây không ai nghĩ tới API như đặt bàn nhà hàng hay đặt sân thể thao.

(2) Các API lần này không cần lập trình viên viết code thủ công để gọi, mà do chính mô hình lớn tự biên dịch từ ngôn ngữ tự nhiên của người dùng sang mã lệnh gọi.

(3) Khách hàng gọi API lần này là người tiêu dùng cá nhân thông qua AI, với mục đích đại diện cho người dùng thực hiện hành vi. Trong khi trước đây API do các ứng dụng gọi nhằm mục đích thu thập và đồng bộ dữ liệu.

## 机器人半马 (Robot chạy bán marathon)

Cuối tuần trước tại Bắc Kinh đã diễn ra cuộc thi chạy bán marathon (Half Marathon) dành riêng cho robot hình người (humanoid robots).

Hơn 100 robot hình người đã tham gia tranh tài xem ai hoàn thành quãng đường 21,0975km nhanh nhất. Kết quả chung cuộc, nhà vô địch đạt thành tích 50 phút 26 giây, vượt qua kỷ lục chạy bán marathon nhanh nhất của con người (kỷ lục thế giới của con người hiện tại là 1 giờ 02 phút 52 giây).

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026042005.webp)

Theo các video ghi nhận tại hiện trường, robot sau khi chạy được một quãng đường nhất định bắt buộc phải ghé vào trạm tiếp tế để kỹ thuật viên thay pin mới và bỏ thêm đá lạnh (hoặc đá khô) để giải nhiệt cho động cơ tránh quá nhiệt.

Điều này đồng nghĩa với việc dung lượng pin tích hợp của robot hiện tại không đủ để duy trì hoạt động cường độ cao suốt 1 giờ đồng hồ.

Mẫu robot hình người H2 thương mại của hãng Unitree có thời gian chạy định mức là 3 giờ trong điều kiện hoạt động bình thường, nhưng khi chạy bộ cường độ cao, thời lượng pin sẽ giảm đi rất nhiều. Hơn nữa, để đạt tốc độ cao, robot cần giảm trọng lượng cơ thể, nghĩa là không thể mang theo quá nhiều pin dự phòng nặng nề.

Do đó, tính thực dụng của robot hình người ở giai đoạn hiện tại vẫn còn khá hạn chế. Nếu hoạt động không cắm điện, chúng cần sạc lại sau mỗi 1-2 tiếng, giới hạn khả năng ứng dụng thực tế.

## GPT Images 2.0

Tuần này, OpenAI phát hành mô hình sinh ảnh mới **GPT Image 2.0**, được đánh giá là mô hình mạnh mẽ nhất hiện nay vượt qua cả Nano Banana 2 Pro của Google.

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026042304.webp)

Theo công bố, mô hình cải tiến lớn khả năng render chữ viết, hỗ trợ tốt chữ Hán và có thể tạo ra các sơ đồ minh họa kỹ thuật phức tạp. Người dùng có thể trải nghiệm miễn phí tại [ChatGPT.com/images](https://chatgpt.com/images).

Dưới đây là hình ảnh so sánh sinh ảnh với prompt "chú chó nhỏ ngủ trưa dưới hiên nhà cổ". Đây là kết quả của GPT Image phiên bản 1:

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026042306.webp)

Và đây là kết quả của GPT Image 2.0:

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026042305.webp)

Một dự án thú vị khác đi kèm là [Flipbook](https://flipbook.page/) — trình duyệt ảnh minh họa kỹ thuật. Khi người dùng nhập một chủ đề, hệ thống sẽ tự động vẽ sơ đồ giải thích chi tiết, click vào từng bộ phận trên sơ đồ sẽ tiếp tục vẽ thêm các hình ảnh giải thích sâu hơn (hình minh họa cấu tạo nước ngọt có ga ở trên).

Cộng đồng cũng đã lập các kho lưu trữ [Awesome GPT Image 2](https://github.com/YouMind-OpenLab/awesome-gpt-image-2) để tổng hợp các prompt sinh ảnh đẹp.

## AI 是扩展神器 (AI là công cụ mở rộng thông tin cực mạnh)

**Một đặc trưng lớn của AI là không chỉ biết tóm tắt nén thông tin, mà còn cực kỳ giỏi trong việc mở rộng phình to thông tin**. Nó tự động suy luận ra các phần mơ hồ, tạo ra các phần bị khuyết thiếu và bổ sung thêm các chi tiết nghe rất hợp lý.

Do đó, AI là một công cụ mở rộng thông tin cực mạnh. Kịch bản ứng dụng trong doanh nghiệp có thể diễn ra như sau:
* CEO họp và nói ra một ý tưởng sơ khai.
* AI tự động viết mở rộng ý tưởng đó thành một tài liệu chiến lược dài hạn.
* AI dịch tài liệu chiến lược thành bảng mô tả thông số kỹ thuật sản phẩm chi tiết.
* AI dùng cơ chế viết code theo cảm hứng (vibe coding) để sinh ra bản mẫu prototype chạy thử.
* AI dựa trên prototype để viết bài thông cáo báo chí giới thiệu sản phẩm.

AI có thể biến một ý nghĩ nhỏ trong đầu thành cả một hệ thống tài liệu, mã nguồn, sản phẩm và chiến dịch truyền thông hoàn chỉnh. Điều này có nghĩa là trong tương lai, mọi sản phẩm tạo ra từ thông tin (như code, văn bản, ảnh, video) sẽ bùng nổ về mặt số lượng nhờ các công cụ AI.

## 小轿车的车载厕所 (Thiết kế nhà vệ sinh trên xe ô tô con)

Hãng xe Seres (Sài Lực Tư) đã nộp bằng sáng chế thiết kế "nhà vệ sinh trên xe ô tô con". Ghế ngồi của xe được đặt trên một hệ thống ray trượt, khi trượt lùi về phía sau sẽ để lộ ra một bồn vệ sinh tích hợp phía dưới sàn xe. Bồn vệ sinh được trang bị thanh nhiệt để làm bay hơi chất lỏng và sấy khô chất thải rắn, tuy nhiên người dùng vẫn cần dọn dẹp thủ công định kỳ. Xe cũng trang bị hệ thống quạt thông gió và ống xả riêng để khử mùi. Thiết kế này có tính ứng dụng hạn chế trên xe con (chỉ dùng khi tắc đường kéo dài trên cao tốc), nhưng hứa hẹn rất hữu ích cho các xe tải chạy đường dài.

## 文章 (Bài viết)

1、[Hãy ngừng sử dụng Ollama](https://sleepingrobots.com/dreams/stop-using-ollama/) (Tiếng Anh)

Phân tích các nhược điểm của công cụ chạy mô hình cục bộ Ollama và khuyên người dùng nên chuyển sang dùng [llama.cpp](https://github.com/ggml-org/llama.cpp) hoặc [LM Studio](https://lmstudio.ai/) để đạt hiệu năng tốt hơn.

2、[Các tính năng đáng học hỏi của npmx](https://nesbitt.io/2026/04/16/features-everyone-should-steal-from-npmx.html) (Tiếng Anh)

Giới thiệu dự án frontend mới [npmx.dev](https://npmx.dev/package/egg) cho trang thư viện npmjs.com, giúp giải quyết nhiều tính năng hữu ích mà giới lập trình viên mong chờ từ lâu.

3、[Tránh lạm dụng liên kết chuỗi (chaining) quá dài](https://allthingssmitty.com/2026/04/20/why-i-dont-chain-everything-in-javascript-anymore/) (Tiếng Anh)

Trong JavaScript, lập trình viên có thể viết các câu lệnh gọi hàm liên tiếp dạng chuỗi rất dài (method chaining). Bài viết phân tích các nhược điểm của phong cách viết này và khuyên không nên lạm dụng chuỗi quá dài vì sẽ gây khó khăn cho việc debug và bảo trì code.

4、[Sự phát triển của lập trình bất đồng bộ](https://causality.blog/essays/what-async-promised/) (Tiếng Anh)

Bài viết phân tích sâu về lịch sử ra đời của lập trình bất đồng bộ (asynchronous programming), cách phát triển ra cú pháp `async/await` đang được áp dụng phổ biến ngày nay và các vấn đề kỹ thuật còn tồn tại.

5、[Cơ chế hoạt động của Radar thụ động](https://www.passiveradar.com/how-passive-radar-works/) (Tiếng Anh)

Khác với radar chủ động phát sóng điện từ để dò tìm vật thể, radar thụ động không phát sóng mà chỉ chẩn đoán sự thay đổi của các sóng điện từ có sẵn trong môi trường (như sóng radio, sóng TV) để phát hiện máy bay.

## 工具 (Công cụ)

1、[Little Snitch cho Linux](https://obdev.at/products/littlesnitch-linux/index.html)

Phần mềm giám sát kết nối mạng nổi tiếng trên macOS Little Snitch đã chính thức phát hành phiên bản dành cho Linux, giúp người dùng kiểm soát chính xác mọi kết nối ra internet của từng ứng dụng.

2、[quien](https://github.com/retlehs/quien/)

Công cụ dòng lệnh tra cứu nhanh thông tin tên miền (Whois) với giao diện hiển thị trực quan và dễ sử dụng.

3、[ggsql](https://ggsql.org/)

Công cụ truy vấn cơ sở dữ liệu bằng SQL hỗ trợ xuất trực tiếp kết quả truy vấn thành các biểu đồ đồ họa trực quan.

4、[Himi Recorder](https://github.com/jrainlau/himi-recorder)

Ứng dụng quay màn hình nguồn mở cho macOS, có khả năng vượt qua các cơ chế phát hiện quay màn hình (screen recording detection) của các ứng dụng khác. (Đóng góp từ [@jrainlau](https://github.com/ruanyf/weekly/issues/9663))

5、[Tab Harbor](https://github.com/V-IOLE-T/tab-harbor)

Plugin Chrome nguồn mở biến trang tab mới thành một giao diện quản lý và sắp xếp các tab đang mở tiện lợi. (Đóng góp từ [@V-IOLE-T](https://github.com/ruanyf/weekly/issues/9665)). Một dự án tương tự là [Tab Out](https://github.com/zarazhangrui/tab-out) (Đóng góp từ [@Acorn2](https://github.com/ruanyf/weekly/issues/9687)).

6、[animal-island-ui](https://github.com/guokaigdg/animal-island-ui)

Thư viện React UI component mang phong cách thiết kế của trò chơi nổi tiếng *Animal Crossing* (Animal Island). (Đóng góp từ [@guokaigdg](https://github.com/ruanyf/weekly/issues/9668))

7、[CUPS Web](https://github.com/hanxi/cups-web)

Trình quản lý máy in giao diện web, giúp điều khiển máy in từ xa qua trình duyệt hỗ trợ quản lý phân quyền người dùng và theo dõi lịch sử in ấn. (Đóng góp từ [@hanxi](https://github.com/ruanyf/weekly/issues/8587))

8、[Blog Helper](https://github.com/thinkycx/blog-helper)

Dịch vụ thống kê lượng truy cập PV/UV nguồn mở cho trang web cá nhân, hỗ trợ hiển thị các bài viết hot và biểu đồ xu hướng. (Đóng góp từ [@thinkycx](https://github.com/ruanyf/weekly/issues/9677))

9、[HiKid](https://github.com/xiaochong/hi-kid)

Ứng dụng desktop miễn phí giúp trẻ em luyện nghe nói tiếng Anh, hiện tại mới chỉ hỗ trợ phiên bản cho hệ điều hành macOS. (Đóng góp từ [@Hao4Wang](https://github.com/ruanyf/weekly/issues/9689))

10、[Kite Desktop](https://github.com/eryajf/kite-desktop)

Công cụ giao diện đồ họa cho máy tính dùng để quản lý đồng thời nhiều cụm máy chủ Kubernetes (K8s). (Đóng góp từ [@eryajf](https://github.com/ruanyf/weekly/issues/9719))

11、[Project River](https://github.com/Lionad-Morotar/project-river)

Trực quan hóa lịch sử commit của kho lưu trữ Git dưới dạng sơ đồ dòng sông (river diagram), hỗ trợ so sánh dữ liệu giữa nhiều dự án. (Đóng góp từ [@Lionad-Morotar](https://github.com/ruanyf/weekly/issues/9722))

## AI 相关 (AI Liên quan)

1、[OpenAI Privacy Filter](https://github.com/openai/privacy-filter)

Bộ lọc bảo mật chạy offline tại máy cục bộ do OpenAI giới thiệu nhằm tự động quét bỏ các thông tin cá nhân nhạy cảm (như email, số điện thoại, mật khẩu) trước khi gửi yêu cầu lên các mô hình ngôn ngữ trực tuyến.

2、[LinkAI Gateway](https://github.com/ruanyf/weekly/issues/9657)

Cổng kết nối AI gateway nguồn mở hỗ trợ cấu hình nhiều loại mô hình lớn và cung cấp một cổng API chung tương thích cấu trúc của OpenAI để các ứng dụng khác gọi. (Đóng góp từ [@star7th](https://github.com/ruanyf/weekly/issues/9657))

3、[Nezha (哪吒)](https://github.com/hanshuaikang/nezha)

Trình quản lý tác vụ lập trình AI gọn nhẹ dưới 10MB tích hợp sẵn cửa sổ terminal, quản lý phiên làm việc, trình chỉnh sửa code và Git. (Đóng góp từ [@hanshuaikang](https://github.com/ruanyf/weekly/issues/9714))

4、[WatermarkZero](https://watermarkzero.org/)

Công cụ chạy ở frontend hỗ trợ xóa các hình mờ watermark ẩn hoặc hiện của Gemini trên ảnh, xử lý trực tiếp trên trình duyệt mà không cần tải ảnh lên server. (Đóng góp từ [@liuyan-wjy](https://github.com/ruanyf/weekly/issues/9664))

5、[mini-cc](https://github.com/you-want/mini-cc)

AI coding agent nguồn mở hoạt động tương tự như Claude Code, hiện tại đã hoàn thành phiên bản viết bằng TypeScript. (Đóng góp từ [@RainyNight9](https://github.com/ruanyf/weekly/issues/9681))

## 资源 (Tài nguyên)

1、[Bảo tàng Âm thanh (The Listening Museum)](https://sheets.works/data-viz/keyboard-sounds): Trang web tổng hợp các đoạn thu âm tiếng gõ phím của nhiều loại bàn phím cơ và bàn phím thông dụng giúp người dùng nghe thử trước khi mua.

2、[Các định luật kỹ nghệ phần mềm](https://lawsofsoftwareengineering.com/): Kho lưu trữ tổng hợp 56 định luật và kinh nghiệm trong phát triển phần mềm như Định luật Parkinson: Công việc luôn tự phình to ra để chiếm hết khoảng thời gian được ấn định cho nó.

## 图片 (Hình ảnh)

1. [Phông chữ tiếng Anh kích thước 5x5](https://maurycyz.com/projects/mcufont/): Phân tích thiết kế phông chữ tiếng Anh siêu nhỏ có kích thước 5x5 pixel, chỉ chiếm dụng 350 byte bộ nhớ giúp render văn bản dễ dàng trên các bộ vi điều khiển 8-bit cũ có dung lượng RAM chỉ 16KB.

2. [Thành phố dầu khí trên biển Caspi](https://www.cnn.com/2024/11/06/climate/oil-rocks-neft-daslari-caspian-sea-city/index.html): Câu chuyện về thành phố dầu khí trên mặt nước Neft Daslari do Liên Xô xây dựng từ giữa thế kỷ 20 trên hồ Caspi, từng là nơi sinh sống của hơn 5.000 công nhân với hệ thống cầu nối dài hàng trăm dặm nối liền 320 giếng dầu.

## 言论 (Phát ngôn)

1、

> "Hãng giày Allbirds công bố chuyển hướng chiến lược thành công ty AI, giúp giá cổ phiếu tăng vọt gấp 5 lần chỉ trong một ngày. Việc này gợi nhớ năm 2017 khi một hãng giải khát công bố đổi tên sang công ty Blockchain để bán trà chanh kèm đầu tư coin, giúp cổ phiếu tăng mạnh trước khi phá sản do dự án blockchain đổ vỡ."
> 
> -- Yahoo News

2、

> "Figma sở hữu gần 2.000 nhân viên để phát triển sản phẩm, trong khi đội ngũ phát triển tính năng Claude Design mới của Anthropic tôi nghi ngờ không quá 10 người. Trước tốc độ phát triển và chi phí cực rẻ của AI, các phần mềm truyền thống trở nên vô cùng yếu ớt."
> 
> -- 《Tình thế khó khăn của Figma》

3、

> "Tôi mong muốn thế giới tương lai thay vì tràn ngập các thiết bị công nghệ viễn tưởng thì sẽ mang tính田 viên nhiều hơn, con người có thể quay lại lối sống truyền thống mà không mất đi các tiện ích công nghệ mang lại, gần như không còn phải nhìn hay chạm vào màn hình thiết bị nữa."
> 
> -- jsomers.net

4、

> "Thung lũng Silicon luôn bị ám ảnh bởi sự giảm tốc tăng trưởng và việc không tạo ra được sản phẩm bùng nổ mới, do đó họ tôn sùng hình tượng các 'kỹ sư anh hùng' — những người thức thâu đêm viết tính năng mới và biến các bản vẽ nguệch ngoạc trên bảng trắng thành các startup tỷ đô."
> 
> -- 《Bài ca của những lập trình viên duy trì cổ điển》

## 往年回顾 (Nhìn lại các năm trước)

[Giải pháp phá vỡ bài toán khởi động lạnh (Cold Start)](https://www.ruanyifeng.com/blog/2025/05/weekly-issue-347.html)（#347）

[Đồ chơi chim uống nước](https://www.ruanyifeng.com/blog/2024/04/weekly-issue-297.html)（#297）

[Thư sa thải nhân viên của Mark Zuckerberg](https://www.ruanyifeng.com/blog/2023/03/weekly-issue-247.html)（#247）

[Nếu thế giới này thực sự có máy tạo niềm vui](https://www.ruanyifeng.com/blog/2022/03/weekly-issue-197.html)（#197）

(Hết)
