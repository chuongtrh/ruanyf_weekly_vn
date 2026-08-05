# 科技爱好者周刊（第 390 期）：没有语料，大模型就是智障 (Bản tin công nghệ hàng tuần số 390: Không có kho ngữ liệu, mô hình lớn chỉ là kẻ khờ)

Ghi lại nội dung công nghệ đáng chia sẻ hàng tuần, phát hành vào thứ Sáu.

Bản tin này [mã nguồn mở](https://github.com/ruanyf/weekly), hoan nghênh bạn [đóng góp](https://github.com/ruanyf/weekly/issues). Ngoài ra còn có dịch vụ [《Ai đang tuyển dụng》](https://github.com/ruanyf/weekly/issues/9088) đăng tải thông tin tuyển dụng lập trình viên. Hợp tác vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图 (Ảnh bìa)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026032201.webp)

Hành lang mái che rực rỡ sắc màu trong một khu dân cư ở Nhật Chiếu, Sơn Đông. Ở lối vào có trồng nhiều cây xanh và bố trí một quán cà phê nhỏ. ([via](https://mooool.com/coffee-tree-canopy-by-selgascano.html))

## 没有语料，大模型就是智障 (Không có kho ngữ liệu, mô hình lớn chỉ là kẻ khờ)

Nếu bây giờ làm một cuộc khảo sát và hỏi mọi người: "Bạn có nghĩ mô hình lớn (LLM) thực sự có trí thông minh không?"

Tôi tin rằng đa số câu trả lời sẽ là có.

Dù hiện tại mới chỉ là giai đoạn sơ khởi của công nghệ AI, các mô hình lớn đã có khả năng thay thế rất nhiều công việc lao động trí óc của con người, thực sự vô cùng kỳ diệu.

Tuy nhiên, chúng ta đừng quên bản chất thực tế: **Mô hình lớn không phải phép thuật, càng không phải là các sinh thể trí tuệ silicon tự chủ (autonomous agents), mà là các mô hình ngôn ngữ được xây dựng trên các quy luật thống kê toán học**. Mọi hành vi đầu ra của chúng đều dựa trên các phép tính toán học xác suất.

Minh chứng rõ ràng nhất là: Nếu yêu cầu mô hình giải quyết các bài toán chưa từng được đưa vào tập huấn luyện — nghĩa là không tồn tại quy luật thống kê có sẵn — nó sẽ hoàn toàn bó tay.

Đó chính là nội dung của một [thử nghiệm thú vị](https://esolang-bench.vercel.app/) tôi muốn chia sẻ hôm nay.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026032008.webp)

Hai nhà nghiên cứu nước ngoài đã thử nghiệm năm mô hình lớn phổ biến: GPT-5.2, o4-mini, Gemini 3 Pro, Qwen3-235B và Kimi K2.

Họ yêu cầu các mô hình này sử dụng năm ngôn ngữ lập trình cực kỳ hiếm gặp và lập dị (esoteric programming languages) — Brainfuck, Befunge-98, Whitespace, Unlambda và Shakespeare — để viết code giải quyết các bài toán chỉ định.

Đặc trưng chung của các ngôn ngữ lập trình lập dị này là trên mạng có rất ít mã nguồn và tài liệu về chúng, đồng nghĩa với việc chúng không xuất hiện trong tập dữ liệu huấn luyện của các mô hình lớn. Các bạn đoán xem kết quả thế nào?

Có thể tóm gọn kết quả thử nghiệm trong một câu: Hiệu năng của các mô hình lớn cực kỳ tệ hại.

Tỷ lệ trả lời chính xác trung bình của cả năm mô hình chỉ đạt vỏn vẹn 3,8% — nghĩa là **trên 100 câu hỏi thì chỉ trả lời đúng được 3,8 câu**. Để so sánh, tỷ lệ trả lời đúng các bài toán viết bằng Python của các mô hình này đạt tới hơn 90%.

Đáng xấu hổ hơn là vài câu hỏi trả lời đúng hiếm hoi kia đều thuộc cấp độ vỡ lòng (entry-level). Còn đối với các cấp độ khó hơn (sơ cấp, trung cấp, cao cấp), tỷ lệ chính xác của cả năm mô hình đều bằng 0.

Thử nghiệm này chứng minh một sự thật: **Hiệu năng (độ thông minh) của mô hình lớn trước hết do tài liệu huấn luyện quyết định**. Kho ngữ liệu (corpus) huấn luyện càng nhiều thì mô hình hoạt động càng tốt. Ví dụ dữ liệu Python tràn ngập khắp nơi nên AI cực kỳ giỏi giải quyết các bài toán Python; còn dữ liệu càng ít, AI hoạt động càng kém và ngây ngô như một kẻ khờ.

Từ đó đặt ra một câu hỏi thú vị: Nếu một ngôn ngữ lập trình hiếm gặp hoàn toàn không có mã nguồn mẫu trên mạng, nhưng lại có một cuốn "Sách hướng dẫn sử dụng" cực kỳ chi tiết, liệu khi chúng ta nạp cuốn sách này cho AI đọc, nó có thể tự học cách lập trình bằng ngôn ngữ đó hay không?

## MAI-Image-2

Tuần này, Microsoft công bố mô hình sinh ảnh mới **MAI-Image-2** với chất lượng hình ảnh sinh ra cực kỳ cao, được đánh giá là chỉ đứng sau Nano Banana 2 của Google ở thời điểm hiện tại.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026032009.webp)

Microsoft cung cấp giao diện trải nghiệm miễn phí tại trang web [MAI Playground](https://playground.microsoft.ai/chat). Trải nghiệm thực tế cho thấy chất lượng ảnh rất chân thực (hình minh họa chú chó đạp xe dưới biển ở trên). Tuy nhiên, mô hình có nhiều giới hạn: Từ chối sinh các ảnh nhạy cảm; giới hạn miễn phí 15 ảnh/ngày và khoảng cách giữa các lần sinh tối thiểu 30 giây; chỉ hỗ trợ tỷ lệ ảnh 1:1; và không hỗ trợ edit ảnh mà chỉ chạy text-to-image thuần túy.

## 科技动态 (Tin tức Công nghệ)

1. [Bìa tạp chí chơi được game](https://www.yankodesign.com/2026/03/16/red-bull-just-put-a-playable-tetris-game-on-a-magazine-cover/): Red Bull phát hành số tạp chí game *GamePop* đặc biệt với trang bìa tích hợp một trò chơi xếp hình Tetris có thể chơi trực tiếp. Bí mật nằm ở việc tích hợp một tấm bảng mạch dẻo siêu mỏng phía dưới bìa sách, trang bị 180 đèn LED RGB, 7 phím cảm ứng điện dung, một chip vi xử lý ARM 32-bit và pin sạc tích hợp cổng Type-C. Cuốn sách được Tetris ủy quyền chính thức và chỉ phát hành giới hạn 150 bản trên toàn cầu.

2. [HP trì hoãn thời gian gọi của khách hàng](https://arstechnica.com/gadgets/2025/02/misguided-hp-customer-support-approach-included-forced-15-minute-call-wait-times/): Nhằm cắt giảm chi phí vận hành tổng đài viên là người thật, HP áp dụng cơ chế buộc khách hàng gọi điện hỗ trợ kỹ thuật phải nghe thông báo tự động hướng dẫn tự lên web tìm câu trả lời. Nếu khách hàng kiên quyết yêu cầu gặp tổng đài viên người thật, hệ thống sẽ bắt buộc họ phải chờ máy đúng 15 phút. Nếu khách hàng cúp máy giữa chừng và gọi lại, thời gian chờ 15 phút sẽ được tính lại từ đầu. Đây có thể là xu hướng tương lai của các hãng: Dịch vụ miễn phí chỉ có AI bot hỗ trợ, muốn gặp người thật phải trả phí dịch vụ riêng.

3. [Cách ném đĩa bay hiệu quả](https://arstechnica.com/science/2024/10/how-physics-can-improve-your-disc-golf-game/): Một nhà vật lý học Mỹ đã đo đạc các thông số tốc độ bay và mô-men xoắn của đĩa bay từ các thử nghiệm ném của học sinh để tìm ra cách ném đĩa bay đi nhanh và xa nhất. Ông phát hiện việc đặt ngón tay cái cách mép ngoài của đĩa bay khoảng 3cm mang lại tốc độ quay và vận tốc ban đầu tối ưu nhất. Tốc độ xoay của đĩa bay có quan hệ tuyến tính với vận tốc ban đầu, đĩa xoay càng nhanh bay càng xa.

## 文章 (Bài viết)

1、[Sự chia rẽ của dự án MkDocs](https://fpgmaas.com/blog/collapse-of-mkdocs/) (Tiếng Anh)

Phân tích cuộc khủng hoảng và mâu thuẫn nội bộ giữa các nhà duy trì chính của công cụ tạo tài liệu nổi tiếng MkDocs, khiến dự án bị chia rẽ.

2、[Dùng AI dự đoán thời gian nguội của cà phê](https://dynomight.net/coffee/) (Tiếng Anh)

Tác giả yêu cầu các mô hình AI khác nhau đưa ra công thức tính thời gian nguội đi của một tách cà phê, sau đó tiến hành đo đạc thực tế để lập bảng xếp hạng độ chính xác của các mô hình.

3、[Ứng dụng di động tiếp theo có thể là Headless App](https://tuananh.net/2026/03/18/why-your-next-mobile-app-is-probably-headless/) (Tiếng Anh)

Lập luận nếu trong tương lai con người giao tiếp với điện thoại chủ yếu qua trợ lý ảo AI, các ứng dụng di động sẽ không còn cần thiết kế giao diện UI nữa mà chỉ cần cung cấp các cổng API truyền nhận dữ liệu cho AI gọi.

4、[Phương pháp nén dữ liệu ở frontend bằng Canvas](https://jstrieb.github.io/posts/canvas-compress/) (Tiếng Anh)

Hướng dẫn cách sử dụng thẻ canvas của HTML5 để thực hiện nén dữ liệu trực tiếp ở phía client thành một định dạng ảnh.

5、[Ruby là ngôn ngữ tốt nhất để viết ứng dụng AI Agent](https://paolino.me/ruby-is-the-best-language-for-ai-apps/) (Tiếng Anh)

So sánh trải nghiệm viết một AI Agent bằng Python, JS và Ruby, tác giả cho rằng cú pháp linh hoạt của Ruby mang lại sự tiện lợi nhất cho việc xây dựng ứng dụng AI.

6、[Công nghệ bê tông của La Mã cổ đại](https://unchartedterritories.tomaspueyo.com/p/how-roman-technology-drove-its-architecture) (Tiếng Anh)

Người La Mã cổ đại đã phát minh và làm chủ công nghệ đúc bê tông, giúp họ xây dựng được các công trình có không gian trong nhà lớn nhất thời cổ đại với độ bền vững trường tồn đến tận ngày nay.

## 工具 (Công cụ)

1、[proxychains-rs](https://github.com/tianrking/proxychains-rs)

Triển khai lại công cụ proxychains4 bằng ngôn ngữ Rust, giúp ép một tiến trình chỉ định chạy qua chuỗi proxy cấu hình. (Đóng góp từ [@tianrking](https://github.com/ruanyf/weekly/issues/9316))

2、[Flare Stack Blog](https://github.com/du2333/flare-stack-blog)

Hệ thống blog nguồn mở chạy trên Cloudflare Workers kết hợp các dịch vụ D1 Database, R2 Storage, KV và Workflow. (Đóng góp từ [@du2333](https://github.com/ruanyf/weekly/issues/9312))

3、[Tunelo](https://github.com/jiweiyuan/tunelo)

Công cụ chia sẻ cổng dịch vụ nội bộ ra internet chỉ bằng một file chạy duy nhất nặng 4MB sử dụng giao thức QUIC tốc độ cao. (Đóng góp từ [@jiweiyuan](https://github.com/ruanyf/weekly/issues/9328))

4、[ReadAny](https://github.com/codedogQBY/ReadAny)

Trình đọc sách điện tử đa nền tảng cho máy tính và Android, tích hợp tính năng đọc thành tiếng, hỗ trợ đồng bộ dữ liệu đọc và tích hợp trợ lý AI. (Đóng góp từ [@codedogQBY](https://github.com/ruanyf/weekly/issues/9342))

5、[RaTeX](https://github.com/erweixin/RaTeX)

Bộ engine render công thức toán học KaTeX viết thuần bằng Rust, hỗ trợ phân tích và hiển thị nhanh công thức LaTeX. (Đóng góp từ [@erweixin](https://github.com/ruanyf/weekly/issues/9350))

6、[Work Review](https://github.com/wm94i/Work_Review)

Ứng dụng ghi nhận hoạt động nền cho Windows và macOS, tự động lưu lại danh sách ứng dụng và trang web người dùng truy cập trong ngày để giúp tự tổng hợp báo cáo công việc. (Đóng góp từ [@wm94i](https://github.com/ruanyf/weekly/issues/9382))

7、[Valdi](https://github.com/Snapchat/Valdi)

UI framework do SnapChat phát hành cho phép viết code giao diện dạng declarative tương tự React rồi biên dịch trực tiếp ra ứng dụng native chạy trên iOS, Android và macOS.

8、[Npflared](https://npflared.thomas-cogez.fr/index.html)

Công cụ thiết lập máy chủ mirror NPM nội bộ dành cho doanh nghiệp để quản lý và chia sẻ các gói thư viện JS dùng chung.

9、[Chokidar](https://github.com/paulmillr/chokidar)

Module Node.js tối ưu chuyên dùng để giám sát mọi thay đổi (thêm, sửa, xóa) của hệ thống tệp tin, hoạt động ổn định hơn thư viện watch mặc định của Node.js.

## AI 相关 (AI Liên quan)

1、**Cổng kết nối WeChat cho AI Agent**

WeChat tuần này đã công bố mở cổng kết nối API chính thức, cho phép các robot AI gửi tin nhắn trực tiếp vào WeChat. Nhiều thư viện mã nguồn mở đã được phát hành để tận dụng cổng kết nối này giúp tích hợp các AI Agent:
* [wechat-rs-sdk](https://github.com/tianrking/weixin-agent-rs) (Đóng góp từ [@tianrking](https://github.com/ruanyf/weekly/issues/9343))
* [WeChatBot](https://github.com/corespeed-io/wechatbot) (Đóng góp từ [@jiweiyuan](https://github.com/ruanyf/weekly/issues/9369))
* [WeClaw](https://github.com/fastclaw-ai/weclaw) (Đóng góp từ [@idoubi](https://github.com/ruanyf/weekly/issues/9347))
* [WeChat-Channel](https://github.com/nanbingxyz/wechat-channel) (Đóng góp từ [@nanbingxyz](https://github.com/ruanyf/weekly/issues/9357))

2、[AI CLI Complete Notify](https://github.com/ZekerTop/ai-cli-complete-notify)

Ứng dụng nhỏ hỗ trợ gửi thông báo (qua Telegram, Email, Webhook...) báo hiệu khi các tác vụ AI chạy trên terminal hoàn thành. (Đóng góp từ [@ZekerTop](https://github.com/ruanyf/weekly/issues/9348))

3、[Claude Config Manager](https://github.com/Daydayoneup/ccm)

Giao diện quản lý đồ họa cho các tài nguyên AI (Skills, MCP, Agent) của Claude trên macOS. (Đóng góp từ [@Daydayoneup](https://github.com/ruanyf/weekly/issues/9370))

4、[TrustClaw](https://www.trustclaw.app/)

Bản tùy biến của OpenClaw nhằm lược bỏ các rủi ro bảo mật hệ thống khi AI thực thi code.

## 资源 (Tài nguyên)

1、[Project N.O.M.A.D.](https://github.com/Crosstalk-Solutions/project-nomad): Ứng dụng Linux tích hợp sẵn kho tri thức ngoại tuyến khổng lồ (Wikipedia, bản đồ thế giới, các khóa học học tập, AI chatbot chạy offline) chuyên dùng để tra cứu cứu sinh khi xảy ra sự cố mất mạng internet diện rộng. (Đóng góp từ [@15x3](https://github.com/ruanyf/weekly/issues/9345))

2、[Tài liệu đào tạo AI Coding Agent của Simon Willison](https://simonw.github.io/nicar-2026-coding-agents/index.html): Hướng dẫn từng bước cách sử dụng các AI Agent để phân tích dữ liệu hiệu quả.

3、[Cuốn sách ngắn gọn về TypeScript](https://gibbok.github.io/typescript-book/zh-cn/book/the-concise-typescript-book/): Giáo trình giới thiệu và học nhanh ngôn ngữ TypeScript nguồn mở.

## 图片 (Hình ảnh)

1. [Ảnh ẩn trên hình nền Apple](https://www.macworld.com/article/3079526/easter-egg-hiding-in-macbook-neos-wallpaper.html): Khám phá chi tiết ẩn thú vị trên hình nền mặc định của dòng MacBook Neo mới ra mắt và các dòng sản phẩm trước đó như iMac, iPad Pro, MacBook Air (tên sản phẩm được vẽ cách điệu ẩn khéo léo trong các nét vẽ của hình nền).

2. [Tỷ lệ tử vong ở trẻ em](https://kottke.org/25/12/an-astonishing-graph): Biểu đồ thống kê lịch sử chỉ ra trong suốt phần lớn lịch sử loài người trước thế kỷ 19, tỷ lệ tử vong ở trẻ sơ sinh và trẻ em trước tuổi trưởng thành luôn nằm ở mức cao kỷ lục khoảng 50%. Chỉ từ cuối thế kỷ 19 y học phát triển mới giúp con số này giảm mạnh xuống mức trung bình toàn cầu 4.3% vào năm 2020.

## 文摘 (Văn trích)

1、[Đừng tự biến mình thành máy móc](https://blog.armeet.ca/becoming-the-machine/)

Tôi đọc được một câu nói sâu sắc: "Chỉ có nô lệ mới dùng hiệu suất công việc (productivity) để chứng minh giá trị tồn tại của bản thân". Đúng vậy, hiệu suất làm việc của nô lệ càng cao thì họ càng có giá trị đối với chủ nhân. Điều này khiến tôi suy nghĩ về trào lưu cổ xúy văn hóa cống hiến, tăng hiệu suất cá nhân ngập tràn trên mạng xã hội hiện nay (phải dậy từ 5 giờ sáng, là người đến đầu tiên và về sau cùng...). Việc này thực chất là con người đang tự so sánh mình với máy móc. Máy móc hoạt động rất nhanh và tuyến tính theo chu trình định sẵn nhưng chúng không có khả năng thích ứng linh hoạt. Bạn là con người, thế mạnh của bạn nằm ở khả năng thích ứng linh hoạt nhanh chóng để tìm ra giải pháp tối ưu nhất cho bài toán chứ không phải chìm đắm trong các công việc chân tay lặp đi lặp lại tẻ nhạt.

## 言论 (Phát ngôn)

1、

> "Chúng ta xây dựng nên một nền văn minh mà các yếu tố cốt lõi của nó phụ thuộc sâu sắc vào khoa học công nghệ, nhưng lại để cho khoa học công nghệ trở nên quá khó hiểu đối với đại đa số công chúng. Sự kết hợp giữa quyền lực và sự thiếu hiểu biết này là một hỗn hợp cực kỳ dễ cháy nổ trong tương lai."
> 
> -- Carl Sagan, nhà thiên văn học lỗi lạc.

2、

> "Thành phố Paris trước đây luôn chịu cảnh tắc đường nghiêm trọng. Thị trưởng đã áp dụng giải pháp quyết liệt cắt giảm phần lớn các chỗ đỗ xe trong nội đô, và kết quả là lượng người lái xe ô tô vào thành phố đã giảm đi rõ rệt."
> 
> -- CNN

3`

> "AI rất giỏi trong việc chuyển dịch một ý tưởng rõ ràng thành mã nguồn có thể chạy được. Phần việc thực sự tốn thời gian và khó khăn nhất là làm sao làm rõ được bản thân tôi thực chất đang muốn xây dựng cái gì."
> 
> -- lustin.fr

## 往年回顾 (Nhìn lại các năm trước)

[Làm thế nào để chặn các bot cào dữ liệu của AI](https://www.ruanyifeng.com/blog/2025/03/weekly-issue-343.html)（#343）

[Một tuần chiếm 2% của một năm](https://www.ruanyifeng.com/blog/2024/03/weekly-issue-293.html)（#293）

[Chatbot AI mô phỏng Khổng Tử](https://www.ruanyifeng.com/blog/2023/02/weekly-issue-243.html)（#243）

[Lập trình frontend hay backend khó hơn?](https://www.ruanyifeng.com/blog/2022/01/weekly-issue-193.html)（#193）

(Hết)
