# 科技爱好者周刊（第 398 期）：Token 费用难以负担 (Bản tin công nghệ hàng tuần số 398: Chi phí Token quá đắt đỏ)

Ghi lại nội dung công nghệ đáng chia sẻ hàng tuần, phát hành vào thứ Sáu.

Bản tin này [mã nguồn mở](https://github.com/ruanyf/weekly), hoan nghênh bạn [đóng góp](https://github.com/ruanyf/weekly/issues). Ngoài ra còn có dịch vụ [《Ai đang tuyển dụng》](https://github.com/ruanyf/weekly/issues/9815) đăng tải thông tin tuyển dụng lập trình viên. Hợp tác vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图 (Ảnh bìa)

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026052803.webp)

Trung tâm Văn hóa Nghệ thuật An Cát tại huyện An Cát, tỉnh Chiết Giang mới mở cửa năm ngoái. Nơi đây nổi tiếng với tre trúc nên mái nhà được thiết kế theo hình dáng lá tre độc đáo. ([daemin_kg@ig](https://www.instagram.com/p/DYKVQBKiBG1/?img_index=1))

## Token 费用难以负担 (Chi phí Token quá đắt đỏ)

Tuần trước, Peter Steinberger — người sáng lập OpenClaw — đã chia sẻ hình ảnh thống kê [lượng Token tiêu thụ](https://x.com/steipete/status/2055346265869721905) của mình.

Anh ấy không phải cố ý khoe khoang mình đã dùng hết bao nhiêu Token, mà là để giới thiệu một tiện ích nhỏ trên thanh menu macOS mang tên [CodexBar](https://codexbar.app/). Tiện ích này giúp thống kê lượng Token sử dụng và quy đổi ra chi phí thực tế.

Mọi người thử đoán xem anh ấy đã dùng hết bao nhiêu Token?

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051701.webp)

Theo ảnh chụp màn hình, chỉ trong một tháng anh ấy đã gửi đi 7,6 triệu lượt yêu cầu (requests), tiêu tốn 603 tỷ Token. Tính theo biểu giá thông thường, lượng Token này trị giá tới 1,3 triệu USD!

Nghĩa là, **chi phí lập trình bằng AI trung bình của anh ấy tốn tới hơn 40.000 USD mỗi ngày**.

Tất nhiên, con số này không phải là chi phí thực trả của cá nhân anh ấy. Do Peter là nhân viên của OpenAI nên anh ấy được cấp quyền sử dụng miễn phí không giới hạn Token từ hệ thống của công ty.

Tuy nhiên, lượng Token anh ấy tiêu thụ là con số thực tế. Hầu hết các công ty bên ngoài đều phải mua Token thương mại. Chúng ta có thể lấy ví dụ này để tính toán: Nếu một lập trình viên tiêu tốn hàng trăm tỷ hoặc thậm chí cả nghìn tỷ Token mỗi tháng, công ty sẽ phải chi trả bao nhiêu?

Một người tốn 1,3 triệu USD một tháng (tương đương gần 9 triệu Nhân dân tệ), **tính ra một năm sẽ ngốn hơn 100 triệu Nhân dân tệ (khoảng 14 triệu USD)!** Đó chính là cái giá mà doanh nghiệp phải trả nếu cho phép nhân viên sử dụng mô hình flagship hàng đầu một cách thả ga.

Nếu chuyển sang dùng các mô hình giá rẻ, chẳng hạn các mô hình nguồn mở trong nước có giá chỉ bằng 1/30 đến 1/50 so với mô hình flagship nước ngoài, thì chi phí hàng năm cho một người vẫn nằm ở mức 2 đến 3 triệu Nhân dân tệ (khoảng 280.000 - 420.000 USD).

Kết quả là: **Nếu cho phép sử dụng không giới hạn, một lập trình viên sẽ tiêu tốn tối thiểu 2 đến 3 triệu Nhân dân tệ tiền Token mỗi năm**. Còn nếu dùng các mô hình cao cấp nhất của Mỹ, chi phí sẽ lập tức tăng vọt lên hàng chục triệu hoặc cả trăm triệu Nhân dân tệ.

Để cắt giảm chi phí này, doanh nghiệp chỉ có hai lựa chọn: Một là mua các gói thuê bao tháng cố định (nhưng dung lượng thường không đủ cho các dự án lớn); hai là tự dựng và chạy các mô hình nguồn mở trên hạ tầng của mình để tiết kiệm phí API (nhưng chi phí phần cứng ban đầu rất đắt đỏ, và các mô hình mạnh nhất hiện tại đều đóng nguồn).

Sau khi cân nhắc kỹ, tôi dự đoán **hầu hết các công ty chắc chắn sẽ áp đặt giới hạn sử dụng, không cho phép lập trình viên tự do gọi các mô hình bên ngoài một cách vô hạn**. Chi phí Token khổng lồ đó vượt quá khả năng chi trả của doanh nghiệp. Lương lập trình viên vốn đã cao, nay cộng thêm vài triệu Nhân dân tệ tiền Token cho mỗi người mỗi năm thì chi phí phát triển dự án sẽ bùng nổ mất kiểm soát.

Các bạn có thể chia sẻ xem có công ty nào đang cấp quyền gọi API không giới hạn các mô hình bên ngoài cho lập trình viên hay không? Cá nhân tôi chưa từng nghe nói.

Trái lại, tôi đã biết đến vài trường hợp các công ty phải thắt chặt chính sách lập trình bằng AI do chi phí Token quá cao.

Ví dụ, hãng gọi xe công nghệ [Uber](https://www.forbes.com/sites/janakirammsv/2026/05/17/uber-burns-its-2026-ai-budget-in-four-months-on-claude-code/) chỉ trong 4 tháng đầu năm đã đốt sạch toàn bộ ngân sách AI trị giá 3,4 tỷ USD của cả năm 2026 cho công cụ Claude Code, buộc họ phải ban hành lệnh hạn chế sử dụng AI.

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026052405.webp)

Hay như [Microsoft](https://aiweekly.co/alerts/microsoft-drops-claude-code-after-budget-overrun) cũng vì chi phí vượt ngân sách nên đã dừng sử dụng Claude Code và chuyển sang sử dụng mô hình OpenAI do chính họ tự host.

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026052406.webp)

Nếu ngay cả các gã khổng lồ như Uber hay Microsoft cũng không chịu nổi chi phí Token khổng lồ này, thì có lẽ không công ty nào trên thế giới có thể gánh nổi.

Tóm lại, mặc dù lập trình bằng AI nghe rất hứa hẹn, nhưng khi nhìn vào hóa đơn thanh toán, các công ty sẽ lập tức tỉnh ngộ: **Lập trình bằng AI tốn kém hơn lập trình viên con người rất nhiều**.

Vì vậy, liệu AI có thay thế lập trình viên không? Đối với các công ty có dự án phần mềm lớn, tôi tin là họ sẽ không thay thế quy mô lớn vì rào cản chi phí. Ít nhất là ở giai đoạn hiện tại, còn tương lai nếu chi phí Token giảm mạnh thì chưa biết thế nào.

## 漏洞赏金计划的终结 (Sự kết thúc của các chương trình săn tiền thưởng lỗi)

[Turso](https://turso.tech) là dịch vụ cơ sở dữ liệu đám mây nguồn mở có mã nguồn đặt trên GitHub.

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026052804.webp)

Họ từng duy trì một chương trình Bug Bounty rất thành công, tặng 1.000 USD cho bất kỳ ai phát hiện ra lỗ hổng bảo mật. Mọi việc diễn ra suôn sẻ cho đến khi các mô hình ngôn ngữ lớn xuất hiện và có thể dùng để quét tìm lỗ hổng tự động.

Trang PR (Pull Request) của dự án này trên GitHub giờ đây đã biến thành như thế này:

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051606.webp)

Lượng người gửi báo cáo lỗi đổ về như lũ quét, tất cả đều nhắm vào giải thưởng tiền mặt. Các "lỗ hổng" họ báo cáo thực chất chỉ là chèn các ký tự rác vào code một cách cố ý hoặc cấu hình sai khiến code không thể chạy được.

Đội ngũ phát triển rơi vào trạng thái kiệt sức vì phải lọc rác. Tệ hơn nữa, khi bị từ chối PR, những người gửi lại sử dụng AI để tạo ra các [đoạn văn giải thích dài dòng](https://github.com/tursodatabase/turso/pull/6257#issuecomment-4216531987) nhằm tranh cãi với đội ngũ kỹ sư: "Tôi không sai, các bạn mới sai", cực kỳ phiền toái.

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051607.webp)

Cuối cùng, đội ngũ phát triển buộc phải công bố [chấm dứt chương trình Bug Bounty](https://turso.tech/blog/the-wonders-of-ai), mọi báo cáo lỗi và PR gửi lên từ nay sẽ không còn tiền thưởng.

> "Những kẻ tạo nội dung rác chỉ mất 1 phút để bấm nút gửi, nhưng chúng tôi phải mất hàng giờ đồng hồ để đọc, tìm hiểu và phản hồi lại. Và tốc độ tạo rác của AI là vô hạn."
> 
> "Dù có thể dùng script tự động để lọc PR, nhưng do có yếu tố tiền thưởng thúc đẩy nên động lực gửi code AI là quá lớn, họ sẽ tìm mọi cách tranh cãi không ngừng nghỉ."

Sự việc này cho thấy mô hình săn tiền thưởng lỗi truyền thống gần như không thể tồn tại trong kỷ nguyên AI. Trong tương lai, việc phát hiện lỗi bảo mật có lẽ sẽ không còn tiền thưởng nữa, điều này có thể dẫn đến việc gia tăng các vụ tấn công mạng thực tế.

## 科技动态 (Tin tức Công nghệ)

1. [Cân nặng và nhiệt độ](https://news.yale.edu/2026/05/20/warmer-temps-heavier-owl-monkeys-climate-linked-weight-gain-primates): Một đội khảo sát từ Đại học Yale phát hiện loài khỉ đêm (owl monkey) tại Argentina hiện tại nặng hơn so với 25 năm trước. Cân nặng trung bình năm 2023 của chúng tăng 50 gram (khoảng 4%) so với năm 1999. Các nhà khoa học tin rằng điều này liên quan đến hiện tượng nóng lên toàn cầu, khiến khỉ tiêu tốn ít năng lượng hơn cho việc duy trì thân nhiệt, do đó có lượng calo dư thừa để tích mỡ. Lý thuyết này có vẻ cũng đúng với con người: Trái Đất ấm lên có thể khiến số lượng người béo phì gia tăng.

2. [Vỏ trứng nhân tạo](https://www.nationalgeographic.com/science/article/artificial-egg-colossal-chickens-moa-dodo): Công ty công nghệ sinh học Colossal của Mỹ đã chế tạo thành công "vỏ trứng nhân tạo" và孵化 ra 26 chú gà con. Vỏ trứng có cấu trúc dạng cốc lục giác chịu lực vững chắc bên ngoài và màng bán thấm bên trong giúp oxy đi qua đồng thời giữ lại độ ẩm. Thiết bị này được thiết kế nhằm mục đích hồi sinh loài chim dodo đã tuyệt chủng, giúp ấp phôi nhân bản của chim dodo mà không cần cấy vào cơ thể các loài động vật khác như đà điểu.

3. [Nghệ thuật phản kháng](https://p26.bg/news/dupkite-po-ul-chiprovci-v-sofiya-se-prevarnaha-v-ulichna-galeriya-snimki-4310news.html): Tại thủ đô Sofia của Bulgaria, có một chiếc hố ga bị sụt lún trên đường phố nhưng chính quyền trì hoãn sửa chữa trong thời gian dài. Hai nghệ sĩ đã vẽ một gương mặt quỷ giận dữ xung quanh chiếc hố đó. Hình ảnh bắt mắt giúp người đi đường dễ quan sát để tránh tai nạn, đồng thời thu hút sự chú ý của truyền thông giúp chiếc hố nhanh chóng được sửa xong. Bài học rút ra là việc phản kháng bằng nghệ thuật thường đem lại hiệu quả cao và dễ được tiếp nhận.

## 文章 (Bài viết)

1、[Nguyên nhân khiến bộ nhớ tăng giá](https://davidoks.blog/p/ai-is-killing-the-cheap-smartphone) (Tiếng Anh)

Các hãng sản xuất bộ nhớ tập trung sản lượng vào dòng chip HBM (bộ nhớ băng thông cao dùng cho server AI) vốn đem lại lợi nhuận khổng lồ, làm giảm sản lượng của dòng chip DDR (PC) và LPDDR (smartphone) dẫn đến tình trạng khan hiếm và đẩy giá thiết bị tiêu dùng tăng cao.

2、[Nghiên cứu dự án Reticulum](https://www.jonaharagon.com/posts/im-getting-into-mesh-networks-meshtastic-meshcore-and-reticulum/) (Tiếng Anh)

Giới thiệu về Reticulum — dự án cho phép tự thiết lập mạng lưới ảo (mesh network) chạy trên nhiều giao thức vật lý khác nhau (WiFi, dây cáp, sóng radio, LoRa, v.v.).

3、[Làm ấm chiếc MacBook của bạn](https://z3ugma.github.io/2019/11/18/warm-up-your-macbook/) (Tiếng Anh)

Bài viết chia sẻ mẹo nhỏ sử dụng lệnh `stress` trên macOS buộc CPU chạy hết công suất nhằm tỏa nhiệt làm ấm lớp vỏ nhôm lạnh giá của MacBook vào mùa đông.

4、[Tại sao tôi phản đối logic Boolean](https://abuseofnotation.github.io/boolean-thinking/) (Tiếng Anh)

Một bài viết triết học lập luận rằng logic Boolean nhị phân (Đúng/Sai) dễ dẫn con người đến lối tư duy nhị nguyên phiến diện, trong khi thế giới thực tế đầy rẫy những biến số không chắc chắn và không có câu trả lời duy nhất.

5、[Tại sao Định lý giới hạn trung tâm lại phổ biến khắp nơi?](https://www.quantamagazine.org/the-math-that-explains-why-bell-curves-are-everywhere-20260316/) (Tiếng Anh)

Giới thiệu lịch sử và ý nghĩa của Định lý giới hạn trung tâm (Central Limit Theorem) nhằm giải thích tại sao phân phối của các giá trị trung bình mẫu luôn tuân theo phân phối chuẩn (hình chuông úp).

## 工具 (Công cụ)

1、[DOCX Editor](https://github.com/eigenpal/docx-editor)

Trình chỉnh sửa tệp docx WYSIWYG nguồn mở chạy trực tiếp trên trình duyệt.

2、[DynIP](https://dynip.dev/)

Dịch vụ cung cấp IP động miễn phí cho người dùng cá nhân.

3、[Graphite](https://editor.graphite.rs/)

Ứng dụng vẽ đồ họa vector nguồn mở chạy trên nền tảng web.

4、[Hindsight](https://github.com/chaosprint/hindsight)

Công cụ dòng lệnh quét các kho lưu trữ git nội bộ để tự động tạo ra biểu đồ đóng góp (contribution heatmap) tương tự phong cách của GitHub.

5、[NyaTerm](https://github.com/nyakang/nyaterm)

Ứng dụng desktop đa nền tảng kết hợp các tính năng SSH, terminal session, quản lý file từ xa, quản lý chứng thực, port forwarding và sao lưu cấu hình trong một giao diện duy nhất. (Đóng góp từ [@nyakang](https://github.com/ruanyf/weekly/issues/10021))

6、[diving-rs](https://github.com/wagoodman/dive)

Công cụ dòng lệnh giúp trực quan hóa và kiểm tra chi tiết các lớp file (layers) bên trong một Docker image. (Đóng góp từ [@vicanso](https://github.com/ruanyf/weekly/issues/10037))

7、[CanvasCast](https://github.com/nine19een/CanvasCast)

Ứng dụng vẽ bảng trắng nguồn mở trên trình duyệt hỗ trợ ghi lại video thuyết trình. (Đóng góp từ [@Hao4Wang](https://github.com/ruanyf/weekly/issues/10055))

8、[Echo Loop](https://github.com/echo-loop/Echo-Loop)

Ứng dụng di động nguồn mở hỗ trợ luyện nghe nói tiếng Anh. (Đóng góp từ [@echo-loop](https://github.com/ruanyf/weekly/issues/10082))

9、[Vue TUI](https://github.com/Simon-He95/vue-tui)

Thư viện UI component viết bằng Vue dùng để xây dựng các giao diện chạy trên terminal, thích hợp phát triển agent. (Đóng góp từ [@Simon-He95](https://github.com/ruanyf/weekly/issues/10083))

10、[witr](https://github.com/pranshuparmar/witr)

Công cụ dòng lệnh hỗ trợ tra cứu xem các cổng mạng (ports) hoặc tên ứng dụng cụ thể đang thuộc về tiến trình (process) nào.

## AI 相关 (AI Liên quan)

1、[DeepSeek Reasonix](https://github.com/esengine/DeepSeek-Reasonix)

AI coding agent chạy trên terminal được thiết kế tối ưu riêng cho DeepSeek, tận dụng tối đa cơ chế cache nhằm giảm thiểu phí API.

2、[FunASR](https://github.com/modelscope/FunASR)

Bộ công cụ nhận diện giọng nói nguồn mở của phòng thí nghiệm Alibaba Tongyi, hỗ trợ nhập liệu bằng giọng nói trên máy tính. (Đóng góp từ [@LauraGPT](https://github.com/ruanyf/weekly/issues/10056)). Các dự án đi kèm: [FunClip](https://github.com/modelscope/FunClip) (cắt video tự động theo từ khóa phụ đề) và [SenseVoice](https://github.com/FunAudioLLM/SenseVoice) (nhận diện cảm xúc, ngôn ngữ, âm thanh sự kiện từ file tiếng).

3、[Codex Mate](https://github.com/SakuraByteCore/codexmate)

Bảng quản lý tập trung các AI coding agent chạy offline hoặc online như Codex, Claude Code, Gemini CLI, CodeBuddy, OpenClaw. (Đóng góp từ [@ymkiux](https://github.com/ruanyf/weekly/issues/10088))

## 资源 (Tài nguyên)

1、[Vi tích phân thực ra rất dễ](https://github.com/KeyAI/calculusmadeeasy-zh)

Bản dịch tiếng Trung phi chính thức của cuốn sách giáo khoa kinh điển *Calculus Made Easy*, giúp người mới dễ dàng tiếp cận môn vi tích phân. (Đóng góp từ [@KeyAI](https://github.com/ruanyf/weekly/issues/10065))

2、[Toàn cảnh 3D Tiểu Tây Thiên](https://funes.world/apps/the-hanging-sculptures-of-the-xiaoxitian)

Bản đồ ảo và thuyết minh 3D các kiến trúc điêu khắc treo tường độc đáo tại chùa Tiểu Tây Thiên, tỉnh Sơn Tây.

3、[C 语言小测验 (C Quiz)](https://stefansf.de/c-quiz/)

Bộ câu hỏi trắc nghiệm kiểm tra kiến thức và ngữ pháp ngôn ngữ C.

## 图片 (Hình ảnh)

1、[Phép chiếu hình trụ (圆柱投影)](https://liorsinai.github.io/mathematics/2020/08/27/secant-mercator.html)

Minh họa phương pháp Mercator chiếu tọa độ mặt cầu Trái Đất lên một ống giấy hình trụ bao quanh để vẽ bản đồ thế giới dạng phẳng.

## 文摘 (Văn trích)

1、[Khi nào lập trình viên nên nghỉ hưu](https://thecodist.com/how-to-know-when-its-time-to-go/)

Sau một năm cân nhắc, tôi quyết định nghỉ hưu và rời bỏ công việc lập trình. Lý do không phải vì tôi không đủ năng lực mà vì tôi nhận thấy mình không còn muốn tiếp tục làm việc này nữa. Ai rồi cũng đến thời điểm không thể làm công việc mình đã gắn bó cả đời. Nó không liên quan đến tuổi tác, tôi từng chứng kiến nhiều lập trình viên trẻ tuổi hơn tôi rất nhiều cũng đã bỏ nghề.

Các nguyên nhân nghỉ hưu phổ biến: (1) Năng lực sa sút; (2) Mất đi niềm đam mê với công việc; (3) Thị trường việc làm khó khăn hoặc công ty đóng cửa; (4) Kỹ năng lỗi thời; (5) Tìm thấy định hướng mới; (6) Đã tích lũy đủ tài chính và cảm thấy kiệt sức.

Quyết định chủ động nghỉ hưu một cách sáng suốt khi nhận thấy mình bắt đầu tụt lại phía sau tốt hơn nhiều so với việc bị đào thải bắt buộc.

## 言论 (Phát ngôn)

1、

> "Nhiều người không nhận ra tiềm năng thay đổi thế giới của AI bởi vì họ không hiểu rằng bản chất của mọi tổ chức xã hội và công ty thực chất chỉ là một biểu đồ tập hợp của các thuật toán vận hành."
> 
> -- 《Công ty chỉ là một biểu đồ thuật toán》

2、

> "Để chống lại tấn công đầu độc thư viện gói phần mềm, giải pháp hiện nay là áp dụng thời gian làm nguội (cooling period) cho các gói phần mềm mới phát hành, người dùng thông thường chỉ nên tải sau khi gói đó đã qua thời gian này. Tuy nhiên, nó lại phụ thuộc vào việc phải có người tải trước đó để kiểm chứng."
> 
> -- 《Gói phần mềm nên được phát hành theo giai đoạn》

3、

> "AI có thể mang lại mô hình giáo dục cá nhân hóa 1-1 với hiệu quả vượt trội, điều này sẽ khiến mô hình đại học truyền thống mất đi giá trị đối với nhiều người."
> 
> -- Sam Altman, CEO của OpenAI.

4、

> "Những người quản lý cấp trung không biết viết code đang cảm thấy rào cản lớn nhất đối với thành công của họ đã biến mất. Họ không cần lập trình viên vẫn có thể tự sửa giao diện web, tự dựng các tính năng nhỏ bằng AI mà AI thì không phàn nàn, không đình công, chỉ biết phục tùng."
> 
> -- 《AI đang dẫn chúng ta đi về đâu》

5、

> "Lý do tôi yêu thích PHP là vì các biến số của nó luôn đi kèm ký hiệu đô la ($) ở đầu, điều này luôn nhắc nhở bạn rằng bạn đang viết code vì mục đích gì."
> 
> -- 《Sự kỳ lạ của PHP》

## 往年回顾 (Nhìn lại các năm trước)

[GitHub Issues gần như là ứng dụng ghi chú tốt nhất](https://www.ruanyifeng.com/blog/2025/06/weekly-issue-351.html)（#351）

[Góc thư viện của OpenAI](https://www.ruanyifeng.com/blog/2024/05/weekly-issue-301.html)（#301）

[Máy tính đơn mạch (SBC) trong nước rất đáng khuyên dùng](https://www.ruanyifeng.com/blog/2023/04/weekly-issue-251.html)（#251）

[Trung Quốc cần thành lập Bộ Bán dẫn](https://www.ruanyifeng.com/blog/2022/04/weekly-issue-201.html)（#201）

(Hết)
