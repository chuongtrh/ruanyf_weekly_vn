# Bản tin chia sẻ công nghệ (Số 381): Các nhà lãnh đạo mô hình AI Trung Quốc đang nghĩ gì

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/8591) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011024.webp)

Ga Thông Châu Bắc Kinh mới đi vào hoạt động được thiết kế nằm hoàn toàn dưới lòng đất. Để tận dụng tối đa nguồn ánh sáng tự nhiên, phần mái vòm của nhà ga sử dụng cấu trúc màng căng xuyên sáng đặc biệt, phía trên được trang bị thêm một khung bảo vệ hình cánh buồm độc đáo. ([via](https://news.cnr.cn/native/gd/kx/20251226/t20251226_527472908.shtml))

## 中国 AI 大模型领导者在想什么

Thứ Bảy tuần trước (ngày 10 tháng 1), tại Bắc Kinh đã diễn ra hội nghị thượng đỉnh công nghệ mang tên "AGI-Next Frontier Summit" do Phòng thí nghiệm Mô hình Cơ sở của Đại học Thanh Hoa chủ trì tổ chức.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011406.webp)

Hội nghị quy tụ sự tham gia của đông đảo những gương mặt đứng đầu đại diện cho thế hệ lãnh đạo AI của Trung Quốc hiện nay:

> - Đường Kiệt (Tang Jie): Giáo sư Đại học Thanh Hoa, nhà sáng lập Zhipu AI.
> - Dương Thực Lân (Yang Zhilin): Nhà sáng lập Moonshot AI (đơn vị phát triển trợ lý Kimi).
> - Lâm Tuấn Dương (Lin Junyang): Trưởng nhóm công nghệ mô hình Tongyi Qianwen (Qwen) của tập đoàn Alibaba.
> - Đào Thuận Vũ (Yao Shunyu): Cựu nghiên cứu viên cốt cán tại OpenAI, hiện là trưởng bộ phận AI mới của tập đoàn Tencent.

Các diễn giả đã chia sẻ những góc nhìn sâu sắc về tương lai của các mô hình AI lớn và chiến lược phát triển AI của Trung Quốc. [Nội dung chi tiết các bài phát biểu](https://www.53ai.com/news/LargeLanguageModel/2026011069524.html) đã được công bố trực tuyến.

Hội nghị ghi nhận rất nhiều phần phát biểu giá trị và thú vị, dưới đây là phần lược ghi và trích lục của tôi về các nội dung nổi bật:

## 一、唐杰的发言

### 1. Nguồn gốc của Zhipu AI

Vào năm 2019, chúng tôi bắt đầu đặt câu hỏi nghiên cứu: Liệu có thể chế tạo ra một cỗ máy có khả năng tư duy giống như con người hay không? Xuất phát từ việc chuyển giao các kết quả nghiên cứu khoa học của Đại học Thanh Hoa, dưới sự hỗ trợ mạnh mẽ của nhà trường, công ty Zhipu AI đã chính thức được thành lập. Hiện tôi đang đảm nhận vai trò Nhà khoa học trưởng tại đây.

Vào thời điểm đó, phòng tĩnh nghiệm của chúng tôi đang nghiên cứu khá tốt ở cấp độ quốc tế trong lĩnh vực mạng thần kinh đồ thị (Graph Neural Networks) và thực thể tri thức (Knowledge Graphs). Tuy nhiên, chúng tôi đã kiên quyết tạm dừng cả hai hướng nghiên cứu này, dồn toàn bộ nguồn nhân lực chuyển sang nghiên cứu mô hình AI lớn.

### 2. Khả năng tổng quát hóa và Mở rộng quy mô (Scaling)

Chúng tôi kỳ vọng mô hình AI sở hữu khả năng tổng quát hóa (generalization) cao, chỉ cần hướng dẫn một phần nhỏ là hệ thống có thể tự suy luận mở rộng ra các phần còn lại. Tương tự như quá trình giáo dục trẻ em: khi dạy cho đứa trẻ 3 bài toán, chúng ta luôn mong muốn đứa trẻ có thể tự giải được bài thứ 4, thứ 10, thậm chí cả những dạng bài chưa từng được dạy trước đó. Làm thế nào để AI đạt được năng lực này?

Cho đến nay, phương án chủ yếu để hiện thực hóa mục tiêu này vẫn dựa vào quy luật mở rộng quy mô (Scaling Laws) để nâng cao khả năng tổng quát hóa ở các tầng cấp độ khác nhau:

（1）Giai đoạn sơ khai, chúng tôi áp dụng kiến trúc Transformer để huấn luyện mô hình ghi nhớ toàn bộ lượng kiến thức đầu vào. Quy mô dữ liệu huấn luyện và năng lực toán lực đầu tư càng lớn thì khả năng ghi nhớ của mô hình càng mạnh. Điều này đồng nghĩa với việc mô hình đã học thuộc lòng toàn bộ tri thức của nhân loại, từ đó sở hữu khả năng tổng quát hóa ở mức cơ bản để thực hiện các tác vụ trừu tượng hóa và suy luận đơn giản. Ví dụ: khi hỏi về thủ đô của Trung Quốc, mô hình chỉ cần truy xuất trực tiếp từ kho tri thức ghi nhớ mà không cần chạy tiến trình suy luận phức tạp.

（2）Cấp độ thứ hai là thực hiện căn chỉnh (alignment) và huấn luyện suy luận cho mô hình, giúp AI sở hữu năng lực suy luận phức tạp hơn và hiểu rõ ý định của người dùng. Quá trình này đòi hỏi việc liên tục Scaling SFT (Supervised Fine-Tuning - Tinh chỉnh có giám sát) và áp dụng học tăng cường (reinforcement learning). Việc liên tục mở rộng quy mô dữ liệu phản hồi từ con người giúp mô hình ngày càng trở nên thông minh và đưa ra câu trả lời chính xác hơn.

（3）Năm nay sẽ chứng kiến sự bùng nổ của công nghệ RLVR (Reinforcement Learning with Verifiable Rewards - Học tăng cường với phần thưởng có thể kiểm chứng). Khái niệm "có thể kiểm chứng" ở đây được hiểu thế nào? Ví dụ: các bài toán toán học hay các đoạn mã lập trình là những thứ có thể chạy kiểm chứng đúng/sai rõ ràng bằng máy. Nhưng mở rộng ra các khía cạnh đời sống, chẳng hạn như đánh giá thiết kế một trang web có đẹp mắt hay không là thứ rất khó kiểm chứng bằng máy mà hoàn toàn phụ thuộc vào cảm quan của con người.

Đây chính là rào cản kỹ thuật rất lớn. Trước đây chúng tôi chỉ có thể tối ưu dựa trên dữ liệu phản hồi thủ công từ con người, nhưng nguồn dữ liệu này thường chứa rất nhiều nhiễu (noise) và kịch bản ứng dụng cũng vô cùng đơn điệu.

Nếu chúng ta xây dựng được một môi trường có khả năng tự động kiểm chứng, chúng ta có thể để AI tự do khám phá, tự tìm kiếm dữ liệu phản hồi và tự tối ưu để trưởng thành. Đây chính là thách thức lớn nhất mà chúng tôi đang đối mặt.

### 3. Từ Chat sang hành động: Sự khởi đầu của một mô hình tư duy mới

Mọi người thường đặt câu hỏi: Phải chăng chỉ cần liên tục nâng quy mô huấn luyện là trí thông minh của AI sẽ tăng lên vô hạn? Thực tế không hoàn toàn như vậy.

Đầu năm 2025, DeepSeek ra đời như một hiện tượng đột ngột bước ra ánh sáng. Cả giới học thuật lẫn giới công nghiệp trước đó đều không ngờ tới sự xuất hiện của DeepSeek với hiệu năng cực kỳ mạnh mẽ, khiến rất nhiều người vô cùng kinh ngạc.

Khi đó chúng tôi đã tự suy ngẫm một vấn đề: với sự xuất hiện của mô hình tư duy (paradigm) dạng DeepSeek, bài toán trò chuyện (Chat) coi như đã được giải quyết căn bản. Nghĩa là dù chúng tôi có nỗ lực tối ưu đến đâu thì trải nghiệm Chat cuối cùng cũng chỉ tương đương với DeepSeek. Chúng ta có thể bổ sung thêm yếu tố cá nhân hóa, tích hợp cảm xúc hay tăng độ phức tạp của cuộc hội thoại, nhưng nhìn chung mô hình tư duy Chat đã đi tới giới hạn cuối cùng, phần việc còn lại chủ yếu là các bài toán tối ưu kỹ thuật và công trình.

Vậy bước đi tiếp theo của AI sẽ hướng về đâu? Ý tưởng của chúng tôi lúc đó là làm sao để mỗi người dùng có thể thực sự dùng AI hoàn thành một công việc cụ thể. Đây có thể là mô hình tư duy tiếp theo: trước đây là trò chuyện (Chat), còn bây giờ là thực sự hành động và giải quyết công việc (做事).

Lộ trình phát triển gồm hai hướng chính: một là mảng lập trình (Coding) và xây dựng các AI Agents; hai là sử dụng AI để hỗ trợ nghiên cứu khoa học (tương tự DeepResearch) hay tự soạn thảo các báo cáo nghiên cứu phức tạp. Lựa chọn hiện tại của chúng tôi là tích hợp đồng bộ cả ba năng lực: Lập trình (Coding), Vận hành tác vụ (Agentic) và Suy luận sâu (Reasoning) lại với nhau.

## 二、林俊旸的发言

### 4. Qwen đã mở nguồn mở như thế nào

Nhiều người thường thắc mắc tại sao dòng mô hình Qwen lại phát hành nhiều phiên bản mở nguồn mở đến vậy?

Câu chuyện bắt đầu từ ngày 3 tháng 8 năm 2023, khi chúng tôi quyết định mở nguồn mở một mô hình siêu nhỏ với quy mô 1.8B chỉ được dùng làm môi trường thử nghiệm nội bộ. Khi chạy huấn luyện thử nghiệm, do nguồn tài nguyên toán lực giới hạn nên chúng tôi không thể dùng mô hình lớn 7B để chạy test liên tục mà phải dùng bản 1.8B làm môi trường kiểm chứng nhanh.

Thời điểm đó, người em khóa dưới trong nhóm đã đề xuất mang bản 1.8B này mở nguồn mở cho cộng đồng. Tôi đã rất phản đối vì cho rằng ở thời điểm năm 2023, bản 1.8B hoạt động rất tệ và hầu như không thể ứng dụng thực tế được thì mở nguồn mở để làm gì? Cậu ấy bảo với tôi rằng bản 7B tiêu tốn quá nhiều tài nguyên máy tính, nhiều học viên cao học và nghiên cứu sinh không có đủ tài nguyên để làm thí nghiệm. Nếu chúng ta mở nguồn mở bản 1.8B, rất nhiều bạn sinh viên sẽ có cơ hội hoàn thành nghiên cứu để tốt nghiệp. Đó là một ý định ban đầu vô cùng nhân văn.

Trong quá trình vận hành sau đó, các nhà sản xuất điện thoại di động tìm đến chia sẻ rằng bản 7B quá nặng để chạy local trên điện thoại còn bản 1.8B lại quá yếu, họ mong muốn có phiên bản quy mô khoảng 3B hoặc 4B. Việc tùy chỉnh này khá đơn giản đối với chúng tôi. Cứ như thế, số lượng phiên bản Qwen ngày một tăng lên nhằm đáp ứng tối đa nhu cầu đa dạng của cộng đồng.

### 5. Mục tiêu chúng tôi hướng tới là mô hình đa phương thức (multimodal)

Khát vọng cốt lõi của chúng tôi không chỉ dừng lại ở việc cung cấp công cụ phục vụ giới lập trình viên hay nhà nghiên cứu, mà là hướng tới xây dựng một Mô hình đa phương thức nền tảng (Multimodal Foundation Agent).

Tôi cực kỳ tin tưởng vào lộ trình này. Vào năm 2023, khi mô hình AI lớn vẫn là thứ bị nhiều người hoài nghi và hoạt động nghiên cứu có phần phong trào, chúng tôi đã kiên định xác định đa phương thức chính là hướng đi bắt buộc phải làm.

Tại sao vậy? Bởi nếu muốn kiến tạo một trí thông minh thực thụ, nó tự nhiên phải sở hữu khả năng đa phương thức (Multimodal). Mặc dù giới học thuật vẫn còn nhiều tranh luận trái chiều về việc liệu đa phương thức có thực sự giúp nâng cao trí thông minh hay không, nhưng tôi không muốn tốn thời gian vào các cuộc tranh luận đó. Con người sở hữu mắt và tai để tiếp nhận thông tin và xử lý được nhiều việc hơn. Góc nhìn của tôi là một Agent nền tảng (Foundation Agent) cần phải tạo ra nhiều năng suất lao động thực tế hơn để hỗ trợ con người, do đó việc tích hợp năng lực xử lý hình ảnh và âm thanh là điều hiển nhiên phải thực hiện.

Xa hơn nữa, mục tiêu của chúng tôi là gì? Một mô hình toàn năng (Omni model) không chỉ dừng lại ở việc đọc hiểu văn bản, hình ảnh, âm thanh đầu vào, mà còn phải sở hữu khả năng tự sinh ra các định dạng văn bản hay âm thanh tương ứng. Hiện tại chúng tôi đã hiện thực hóa được điều này, chỉ còn thiếu mảnh ghép tự sinh hình ảnh đồng bộ. Một khi hoàn thiện được cơ chế xử lý đồng thời cả đầu vào và đầu ra cho cả 3 định dạng dữ liệu (text/audio/video), đó sẽ là cột mốc công nghệ vô cùng tuyệt vời.

## 三、姚顺雨的发言

### 6. Sự khác biệt giữa To C và To B

Quan sát đầu tiên của tôi là sự phân hóa ngày càng rõ rệt giữa hai phân khúc mô hình dành cho khách hàng cá nhân (To C) và khách hàng doanh nghiệp (To B).

Khi nhắc tới AI, mọi người thường nghĩ ngay đến hai đại diện tiêu biểu: một là ChatGPT và hai là Claude Code. Đây chính là những ví dụ điển hình cho định hướng To C và To B.

Đối với người dùng cá nhân (To C), phần lớn thời gian họ không thực sự cần tới một mức độ trí thông minh quá siêu việt. Phiên bản ChatGPT hiện tại so với một năm trước rõ ràng đã nâng cấp mạnh mẽ năng lực phân tích nghiên cứu, nhưng phần lớn người dùng cá nhân trong các tác vụ hàng ngày rất khó cảm nhận rõ sự khác biệt đó. Họ chủ yếu sử dụng AI như một công cụ tìm kiếm nâng cao và nhiều khi không biết cách đưa ra câu lệnh (prompt) tối ưu để kích hoạt tối đa trí thông minh của mô hình.

Nhưng đối với khách hàng doanh nghiệp (To B), trí thông minh của mô hình càng cao đồng nghĩa với việc năng suất lao động tạo ra càng lớn, và giá trị kinh tế mang lại càng cao. Do đó, doanh nghiệp luôn sẵn sàng chi tiền để sử dụng dòng mô hình mạnh mẽ nhất. Một mô hình tốt nhất có mức giá 200 USD/tháng, còn các dòng mô hình hạng hai có giá chỉ 20 USD hay 50 USD/tháng, nhưng thực tế cho thấy các doanh nghiệp Mỹ vẫn luôn ưu tiên chi trả mức giá cao để dùng bản tốt nhất.

Ví dụ một nhân sự có mức lương 200.000 USD/năm, mỗi ngày cần xử lý 10 tác vụ công việc. Một mô hình AI cực mạnh có thể xử lý chính xác 9 trên 10 tác vụ đó, còn mô hình yếu hơn chỉ làm đúng được 5 tác vụ. Vấn đề là nếu không biết rõ 5 tác vụ bị sai nằm ở đâu, bạn sẽ phải tốn thêm rất nhiều thời gian và nhân lực để kiểm tra rà soát lại toàn bộ công việc.

Do đó trên thị trường doanh nghiệp (To B), sự phân hóa khoảng cách giữa mô hình dẫn đầu và mô hình hạng hai sẽ ngày càng trở nên sâu sắc.

### 7. Tích hợp dọc và Phân lớp ứng dụng mô hình

Quan sát thứ hai của tôi là sự phân hóa giữa hai triết lý phát triển sản phẩm: Tích hợp dọc (Vertical Integration) và Phân lớp ứng dụng mô hình (Model-App Decoupling).

Ví dụ: hệ sinh thái ChatGPT Agent đi theo hướng tích hợp dọc, còn mô hình phối hợp Claude (hoặc Gemini) chạy kèm Manus đi theo hướng phân lớp ứng dụng. Trước đây, mọi người thường tin rằng năng lực tích hợp dọc từ gốc đến ngọn sẽ luôn mang lại hiệu quả sản phẩm tốt nhất, nhưng thực tế hiện nay cho thấy điều đó không còn hoàn toàn đúng nữa.

Trước hết, năng lực cần có ở tầng mô hình nền tảng và tầng ứng dụng là rất khác nhau. Đặc biệt đối với các kịch bản doanh nghiệp To B hướng tới năng suất lao động, việc huấn luyện mô hình nền tảng quy mô lớn vẫn là yếu tố mang tính quyết định, và đây là phần việc cực kỳ khó khăn đối với các công ty chỉ chuyên làm sản phẩm ứng dụng. Tuy nhiên, để khai thác và ứng dụng hiệu quả một mô hình nền tảng tốt vào thực tế công việc lại đòi hỏi sự tối ưu hóa rất lớn ở tầng ứng dụng và cấu hình môi trường vận hành bên ngoài.

Thực tế chỉ ra rằng đối với các ứng dụng khách hàng cá nhân To C (như ChatGPT hay Doubao), triết lý tích hợp dọc vẫn phát huy hiệu quả rất tốt khi mô hình và sản phẩm ứng dụng được liên kết chặt chẽ và cập nhật liên tục cùng nhau. Nhưng đối với phân khúc doanh nghiệp To B, xu hướng lại đi theo chiều ngược lại: mô hình nền tảng ngày càng phát triển mạnh mẽ và độc lập, đồng thời xuất hiện hàng loạt ứng dụng bên thứ ba đóng vai trò trung gian để đưa mô hình đó tối ưu vào từng quy trình sản xuất cụ thể của doanh nghiệp.

### 8. Nhu cầu mở rộng ngữ cảnh (Context) lớn hơn

Làm thế nào để các mô hình AI hiện nay tạo ra nhiều giá trị thực tế hơn cho người dùng? Chúng tôi nhận thấy chìa khóa nằm ở việc bổ sung thêm các thông tin ngữ cảnh (Context) đầu vào bên ngoài.

Ví dụ khi hỏi AI: "Hôm nay nên ăn gì?". Thực tế câu trả lời của ChatGPT ở các thời điểm hôm nay, năm ngoái hay ngày mai đáng lẽ phải rất khác nhau. Để đưa ra câu trả lời thực sự chất lượng, hệ thống không chỉ cần một mô hình lớn hơn hay thuật toán học tăng cường mạnh mẽ hơn, mà cái nó cần là các thông tin ngữ cảnh đầu vào chi tiết: ví dụ hôm nay thời tiết lạnh nên cần ăn món ấm nóng, vị trí di chuyển hiện tại của tôi ở đâu, hay vợ tôi hôm nay đang đi ăn món gì ở địa điểm khác...

Việc tối ưu hóa và tận dụng hiệu quả các thông tin ngữ cảnh đầu vào (chẳng hạn như việc người dùng chuyển tiếp lịch sử trò chuyện với vợ cho trợ lý Yuanbao phân tích) sẽ giúp mang lại những giá trị ứng dụng vô cùng lớn và thực tế. Đây chính là định hướng tư duy phát triển sản phẩm To C của chúng tôi.

## 四、圆桌对话：中国 AI 的未来

**Lý Quảng Mật (Người điều phối)**: Tôi muốn đặt một câu hỏi chung cho các diễn giả: Theo các bạn, sau 3 đến 5 năm nữa, xác suất để công ty AI dẫn đầu thế giới là một doanh nghiệp Trung Quốc là bao nhiêu phần trăm? Để chuyển dịch vị thế từ người đi sau hiện nay vươn lên thành người dẫn đầu tương lai, chúng ta cần phải tập trung hoàn thiện những yếu tố nào?

### 9. Câu trả lời của Đào Thuận Vũ

Tôi đánh giá xác suất này là tương đối cao và bản thân tôi giữ thái độ khá lạc quan. Thực tế chứng minh bất kỳ đột phá công nghệ mới nào được thế giới phát hiện thì các kỹ sư Trung Quốc đều có khả năng nhanh chóng tái hiện lại và tối ưu hóa cực kỳ tốt ở nhiều khía cạnh cụ thể, tương tự như những gì đã diễn ra trong ngành sản xuất công nghiệp và xe điện trước đây.

Để hiện thực hóa mục tiêu này, tôi nghĩ có một số nút thắt cốt lõi cần phải giải quyết:

（1）Năng lực tự chủ sản xuất máy quang khắc của Trung Quốc có đạt được đột phá hay không. Nếu toán lực trở thành nút thắt cổ chai bị nghẽn, chúng ta có phương án nào để tự giải quyết bài toán toán lực này hay không.

（2）Có xây dựng được một thị trường doanh nghiệp To B trưởng thành hay không. Hiện tại phần lớn các mô hình và ứng dụng hướng tới năng suất lao động doanh nghiệp chất lượng vẫn ra đời tại Mỹ, bởi các doanh nghiệp ở đó có thói quen chi trả dịch vụ tốt hơn và văn hóa cởi mở hơn. Việc phát triển mảng này tại thị trường trong nước hiện vẫn gặp nhiều khó khăn, buộc các startup phải lựa chọn con đường xuất khẩu công nghệ (outbound) ra thị trường quốc tế. Đây là yếu tố khách quan lớn bên cạnh bài toán toán lực.

（3）Nhưng quan trọng hơn cả vẫn là yếu tố chủ quan: Tôi cảm thấy số lượng nhân sự tại Trung Quốc sẵn sàng dũng cảm thử nghiệm các mô hình tư duy mới hoặc chấp nhận dấn thân mạo hiểm vẫn còn tương đối mỏng. Nói cách khác, chúng ta có đủ những nhà khởi nghiệp sở hữu tinh thần phiêu lưu dũng cảm đứng ra tiên phong khai phá những con đường mới hay không. Khả năng dẫn dắt thiết lập các mô hình tư duy mới chính là bài toán duy nhất Trung Quốc cần tìm lời giải, bởi ở các mảng việc còn lại như vận hành thương mại, thiết kế sản phẩm hay tối ưu hóa kỹ thuật công trình thì chúng ta thực tế đã làm tốt hơn người Mỹ ở nhiều khía cạnh.

### 10. Câu trả lời của Lâm Tuấn Dương

Đây là một câu hỏi tương đối nhạy cảm, trên lý thuyết ở những diễn đàn thế này thì không nên đưa ra những nhận định bi quan. Tuy nhiên nếu xét trên khía cạnh xác suất thực tế, tôi xin chia sẻ một vài điểm khác biệt cốt lõi mà tôi cảm nhận được giữa môi trường Trung Quốc và Mỹ.

Ví dụ về tài nguyên toán lực (Compute): quy mô toán lực tổng thể của Mỹ hiện vượt trội hơn chúng ta từ 1 đến 2 cỡ đại lượng (orders of magnitude). Thêm vào đó, tôi quan sát thấy các tổ chức như OpenAI dồn một lượng toán lực khổng lồ cho các nghiên cứu đón đầu tương lai; trong khi tài nguyên của chúng ta hiện tại tương đối eo hẹp, việc bảo đảm hạ tầng vận hành phục vụ các dịch vụ thương mại hiện tại gần như đã ngốn sạch phần lớn năng lực toán lực của các doanh nghiệp trong nước. Đây là một khoảng cách rất lớn.

Đây là bài toán lịch sử luôn tồn tại: hoạt động đổi mới sáng tạo sẽ diễn ra ở nhóm những người giàu có dư dả tài nguyên hay ở nhóm những người nghèo thiếu hụt tài nguyên? Nhóm đi sau không phải là không có cơ hội. Chúng tôi nhận thấy các doanh nghiệp lớn của Mỹ đôi khi chi tiêu toán lực khá lãng phí khi chạy huấn luyện rất nhiều thứ không thực sự mang lại hiệu quả thực tế. Còn khi bạn ở thế thiếu hụt tài nguyên, bạn sẽ có động lực cực lớn để tập trung tối ưu hóa đồng thời cả thuật toán lẫn hạ tầng cơ sở (Infra joint optimization) – điều mà các doanh nghiệp dư dả tài nguyên hầu như không có nhiều động lực để làm.

Một yếu tố cốt lõi nữa trong tương lai là liệu chúng ta có khả năng tự chủ phát triển sự kết hợp đồng bộ giữa mô hình AI thế hệ mới và vi xử lý phần cứng tự chủ trong nước hay không?

Vào năm 2021 khi tôi bắt đầu nghiên cứu mô hình lớn, các kỹ sư mảng chip của Alibaba có tìm đến hỏi tôi liệu có thể đưa ra dự đoán sau 3 năm nữa cấu trúc mô hình chủ lưu có còn là Transformer và đi theo hướng đa phương thức nữa hay không? Sở dĩ họ hỏi mốc 3 năm bởi đó là chu kỳ tối thiểu cần thiết để thiết kế và sản xuất thử nghiệm (tape-out) một dòng chip mới. Câu trả lời của tôi lúc đó là: sau 3 năm nữa liệu tôi có còn làm việc ở Alibaba hay không tôi còn chưa rõ! Nhưng hiện tại tôi vẫn đang làm việc tại Alibaba, và cấu trúc chủ lưu quả thực vẫn là Transformer và đi theo hướng đa phương thức. Tôi vô cùng hối hận vì thời điểm đó đã không thúc giục họ quyết liệt triển khai dự án chip đó sớm. Buổi thảo luận lúc đó giống như hai người nói hai ngôn ngữ khác nhau khi họ không hiểu việc chúng tôi đang làm và ngược lại, dẫn đến việc bỏ lỡ một cơ hội công nghệ quý giá. Liệu cơ hội đó có xuất hiện lại một lần nữa hay không? Và liệu tinh thần vượt khó tìm kiếm giải pháp sáng tạo trong nghịch cảnh của chúng ta có giúp tạo nên đột phá?

Hiện nay chất lượng giáo dục trong nước đang ngày một nâng cao. Tôi thuộc thế hệ đầu 90, anh Thuận Vũ thuộc thế hệ cuối 90, còn trong đội ngũ của chúng tôi hiện nay có rất nhiều bạn trẻ thế hệ 10x (00s) sở hữu tinh thần dấn thân mạo hiểm vô cùng mạnh mẽ. Người Mỹ tự nhiên có tinh thần phiêu lưu rất lớn, tiêu biểu như việc khi các dòng xe điện đầu tiên ra đời dù tính an toàn chưa cao và từng xảy ra tai nạn nhưng giới nhà giàu Mỹ vẫn sẵn sàng chi tiền mua trải nghiệm và đầu tư phát triển; còn ở Trung Quốc trước đây giới nhà giàu hầu như sẽ không bao giờ mạo hiểm làm những việc như vậy mà chỉ lựa chọn những phương án an toàn. Hiện nay tinh thần dấn thân mạo hiểm của giới trẻ trong nước đã được cải thiện rất nhiều cùng với môi trường kinh doanh ngày một hoàn thiện, tôi tin điều này hoàn toàn có thể mang lại những đột phá mới. Xác suất không quá lớn, nhưng hoàn toàn có cơ hội xảy ra.

Dự báo sau 3 đến 5 năm nữa, xác suất để công ty AI dẫn đầu thế giới là một doanh nghiệp Trung Quốc, tôi đánh giá rơi vào khoảng 20%. Con số 20% đã là cực kỳ lạc quan rồi, bởi vì có rất nhiều yếu tố tích lũy lịch sử nằm ở đây.

### 11. Câu trả lời của Đường Kiệt

Trước hết, chúng ta phải thẳng thắn thừa nhận một thực tế là các phòng nghiên cứu AI của doanh nghiệp (AI Labs) trong nước vẫn tồn tại một khoảng cách phát triển nhất định so với các đối thủ Mỹ.

Việc chúng ta công bố một số mô hình mở nguồn mở chất lượng có thể khiến cộng đồng phấn khích và lầm tưởng rằng trình độ mô hình lớn của Trung Quốc đã vượt qua Mỹ. Nhưng thực tế đáng buồn là khoảng cách có thể vẫn đang bị nới rộng, bởi các tập đoàn Mỹ đang giữ kín các mô hình tiên tiến nhất dưới dạng đóng nguồn (closed-source), còn chúng ta chỉ đang tối ưu và tự hài lòng trên các phiên bản mở nguồn mở (open-source). Khoảng cách thực tế không hề thu hẹp nhanh chóng như nhiều người vẫn tưởng tượng. Chúng ta có những điểm sáng nhất định nhưng vẫn phải tỉnh táo nhìn nhận các thách thức và khoảng cách phát triển.

Tuy nhiên tôi tin tưởng mọi việc đang dịch chuyển theo hướng ngày một tốt hơn:

（1）Thế hệ trẻ 9x và 10x hiện nay sở hữu năng lực vượt trội hơn hẳn thế hệ trước. Chúng ta đang có những bộ óc thông minh xuất chúng sẵn sàng dấn thân mạo hiểm dẹp bỏ vùng an toàn để khai phá những hướng đi mới, tiêu biểu như tinh thần của các bạn trẻ như Lâm Tuấn Dương, Dương Thực Lân hay Đào Thuận Vũ.

（2）Môi trường phát triển trong nước đang ngày một tốt hơn, từ các chính sách vĩ mô hỗ trợ quốc gia cho tới cơ chế cạnh tranh bình đẳng giữa doanh nghiệp lớn và nhỏ, tạo không gian sinh tồn tốt cho các startup công nghệ.

（3）Yếu tố quyết định sau cùng nằm ở chính sự kiên trì của mỗi cá nhân chúng ta. Liệu chúng ta có đủ bền bỉ dấn bước trên con đường đã chọn, dám nghĩ dám làm và chấp nhận mạo hiểm hay không. Nếu chúng ta kiên trì theo đuổi mục tiêu một cách bền bỉ nhất, chiến thắng sau cùng chắc chắn sẽ gọi tên chúng ta.

## 科技动态

1. **Tàu khí cầu chở khách đầu tiên đi vào vận hành thương mại**

Vào ngày 9 tháng 1, tàu khí cầu chở khách Xiangyun AS700 do tỉnh Hồ Bắc sản xuất đã hoàn thành chuyến bay khứ hồi từ Kinh Môn đến Vũ Hán. Đây là chuyến bay thương mại bằng tàu khí cầu chở khách đầu tiên tại Trung Quốc, và cũng có thể là tàu khí cầu thương mại chở khách duy nhất đang hoạt động trên thế giới hiện nay.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011101.webp)

Tàu khí cầu có tổng chiều dài 50 mét, sức chứa tối đa 9 hành khách. Do sức chứa quá nhỏ nên nó không thể đóng vai trò như một phương tiện giao thông thông thường mà chỉ phục vụ các chuyến bay ngắm cảnh du lịch.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011102.webp)

2. **Dụng cụ bút cảm ứng điều khiển bằng mũi**

Một nhà phát minh người Anh muốn sử dụng điện thoại khi đang tắm, nhưng các ngón tay dính nước nên không thể thao tác cảm ứng.

Trong lúc cấp bách, ông đã nảy ra ý tưởng phát minh ra một chiếc bút cảm ứng đeo trên mũi.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011014.webp)

Cấu tạo của nó rất đơn giản: gồm một ống bọc mũi bằng thạch cao sợi, bên trong cắm một chiếc bút cảm ứng.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011015.webp)

Phát minh này trông có vẻ rất hữu ích, giúp giải phóng đôi tay và cũng phù hợp cho những trường hợp phải đeo găng tay hoặc người khuyết tật.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011016.webp)

3. **Việt Nam ban hành quy định cấm các quảng cáo không thể bỏ qua**

Chính phủ Việt Nam gần đây đã ban hành Nghị định số 342 cấm các quảng cáo không thể bỏ qua, quy định mới này sẽ chính thức có hiệu lực thi hành từ ngày 15 tháng 2 năm 2026.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011013.webp)

Nghị định quy định thời gian chờ của quảng cáo video phải dưới 5 giây, sau đó người xem có quyền lựa chọn bỏ qua (skip). Đồng thời, nút tắt quảng cáo phải hiển thị rõ ràng, dễ thao tác, cấm sử dụng các ký hiệu giả mạo hoặc mờ nhạt để gây nhầm lẫn cho người dùng.

Quy định này rõ ràng nhắm vào các quảng cáo đầu video trên các nền tảng lớn như YouTube. Điều này khiến cộng đồng mạng lần đầu tiên cảm thấy Internet Việt Nam đáng được biểu dương.

## 文章

1. [Quyết định đóng toàn bộ mã nguồn của các dự án phần mềm mới](https://x.com/MarcJSchmidt/status/2009688028931875156) (tiếng Anh)

Chia sẻ của một lập trình viên có nhiều đóng góp cho cộng đồng mã nguồn mở. Anh bày tỏ sự thất vọng khi các đoạn mã nguồn mở của mình liên tục bị các mô hình AI lớn tự động quét thu thập dữ liệu, dẫn đến lượt truy cập trực tiếp vào dự án sụt giảm mạnh và bản thân không thể tìm kiếm nguồn thu nhập duy trì. Do đó anh quyết định toàn bộ các dự án lập trình mới trong tương lai sẽ chuyển hoàn toàn sang mô hình đóng nguồn (closed-source).

2. [Phương pháp chạy kiểm thử hồi quy trực quan cho trang web](https://marending.dev/notes/visual-testing/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011201.webp)

Bài viết hướng dẫn cách thức sử dụng thư viện tự động hóa Playwright để thực hiện quy trình kiểm tra so sánh giao diện đồ họa của trang web nhằm phát hiện nhanh các lỗi hiển thị phát sinh sau khi cập nhật code.

3. [Thay thế Redis bằng cơ sở dữ liệu PostgreSQL cho hiệu năng tối ưu](https://dev.to/polliog/i-replaced-redis-with-postgresql-and-its-faster-4942) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011202.webp)

Redis vốn là lựa chọn quen thuộc nhất cho các tác vụ lưu trữ bộ nhớ đệm (caching). Tác giả bài viết phân tích những điểm hạn chế của Redis trong thực tế vận hành và hướng dẫn giải pháp chuyển đổi sang sử dụng PostgreSQL làm bộ nhớ đệm với hiệu suất xử lý thậm chí còn tốt hơn.

4. [Các giải pháp xử lý triệt để lỗi xuất hiện thanh cuộn ngang bằng CSS](https://aartaka.me/easy-fixes.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011008.webp)

Tài liệu CSS cơ bản giới thiệu 4 mẹo xử lý giao diện cực kỳ đơn giản để bảo đảm trang web không phát sinh lỗi tràn khung hiển thị tạo nên thanh cuộn ngang gây mất thẩm mỹ.

5. [Tìm hiểu các nguyên lý hoạt động của hệ thống hàng đợi tin nhắn (Message Queue)](https://www.cloudamqp.com/blog/message-queues-exaplined-with-analogies.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011403.webp)

Bài viết vỡ lòng sử dụng các hình ảnh so sánh thực tế đời sống để giải thích trực quan về khái niệm và tầm quan trọng của hệ thống hàng đợi tin nhắn trong kiến trúc phần mềm hiện đại.

6. [Các rắc rối liên quan đến góc bo tròn trên giao diện macOS Tahoe](https://noheger.at/blog/2026/01/11/the-struggle-of-resizing-windows-on-macos-tahoe/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011207.webp)

Phiên bản hệ điều hành macOS Tahoe mới nhất của Apple đã tăng đáng kể bán kính bo tròn góc của các cửa sổ ứng dụng. Thay đổi này vô tình gây nên lỗi khiến người dùng thường xuyên rê chuột kéo thay đổi kích thước cửa sổ thất bại. Tác giả phân tích và đưa ra kiến nghị tối ưu hóa thiết kế giao diện bo góc để bảo đảm hiệu quả tương tác tốt nhất.

## 工具

1. [whenwords](https://github.com/dbreunig/whenwords)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011105.webp)

Tuần này trên GitHub xuất hiện một kho lưu trữ vô cùng độc đáo: dự án hoàn toàn không chứa bất kỳ một dòng code lập trình nào mà chỉ cung cấp duy nhất một tệp tin tài liệu mô tả chi tiết giao diện kết nối (API document).

Người dùng có nhu cầu sử dụng sẽ tự copy phần mô tả tài liệu này đưa vào mô hình AI lớn, chỉ định ngôn ngữ lập trình mong muốn để AI tự sinh ra mã nguồn thư viện tương ứng rồi nhúng vào dự án.

Liệu đây có phải là xu hướng phát triển phần mềm trong tương lai: các thư viện mã nguồn sẽ không còn tồn tại các đoạn code thô mà chỉ cung cấp các tài liệu mô tả giao diện kết nối?

2. [Hongdown](https://github.com/dahlia/hongdown)

Công cụ hỗ trợ tự động căn chỉnh và làm đẹp định dạng cho các tệp tin văn bản Markdown dựa trên các bộ quy tắc cấu hình thiết lập sẵn.

3. [VAM Seek](https://github.com/unhaya/vam-seek)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011204.webp)

Trình phát video trực tuyến mã nguồn mở tự động trích xuất và hiển thị các hình ảnh thu nhỏ (thumbnails) tại nhiều mốc thời gian dọc thanh tiến trình, giúp người xem dễ dàng click chuyển nhanh đến phân đoạn cần xem.

4. [kodbox](https://github.com/kalcaddle/kodbox)

Hệ thống quản lý tệp tin dựa trên giao diện web mã nguồn mở chất lượng.

5. [Nigate](https://github.com/hoochanlon/Free-NTFS-for-Mac)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011103.webp)

Công cụ mã nguồn mở hỗ trợ hệ điều hành macOS dễ dàng đọc ghi dữ liệu trên các ổ đĩa định dạng NTFS. (Đóng góp từ [@hoochanlon](https://github.com/ruanyf/weekly/issues/8672))

6. [Flippy Lid](https://github.com/huanglizhuo/Flappy.Lid)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011206.webp)

Phần mềm thử nghiệm độc đáo biến hành vi đóng/mở bản lề của máy tính MacBook thành tín hiệu đầu vào để điều khiển chơi game hoặc dùng làm cơ chế mở khóa mật khẩu máy tính. (Đóng góp từ [@huanglizhuo](https://github.com/ruanyf/weekly/issues/8683))

7. [Jumble](https://github.com/CodyTseng/jumble)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011301.webp)

Trình duyệt web mã nguồn mở chuyên dụng kết nối vào mạng xã hội phân tán Nostr, được thiết kế tối ưu để theo dõi các nội dung bảng tin (feed) từ các nút relay. (Đóng góp từ [@CodyTseng](https://github.com/ruanyf/weekly/issues/8692))

8. [Clash Kit](https://github.com/wangrongding/clash-kit)

Bộ công cụ dòng lệnh hỗ trợ quản lý và cấu hình dịch vụ Clash phát triển dựa trên môi trường Node.js. (Đóng góp từ [@wangrongding](https://github.com/ruanyf/weekly/issues/8703))

9. [SlideNote](https://github.com/maoruibin/SlideNote)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011501.webp)

Plugin trình duyệt Chrome hỗ trợ mở thanh ghi chú nhanh ở cạnh màn hình, tự động đồng bộ dữ liệu ghi chú của người dùng trên các thiết bị khác nhau. (Đóng góp từ [@maoruibin](https://github.com/ruanyf/weekly/issues/8715))

10. [NginxPulse](https://github.com/likaia/nginxpulse)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011502.webp)

Bảng quản trị hiển thị và phân tích dữ liệu nhật ký truy cập (access log) của máy chủ Nginx mã nguồn mở, cung cấp các thông số thống kê thời gian thực, bộ lọc PV, thông tin địa chỉ IP truy cập và phân tích trình duyệt sử dụng của khách hàng. (Đóng góp từ [@likaia](https://github.com/ruanyf/weekly/issues/8696))

## AI 相关

1. **Auto Paper Digest (APD)**

Ứng dụng AI hỗ trợ tự động quét thu thập các bài báo khoa học về công nghệ AI nổi bật hàng tuần trên arXiv, kết nối tới NotebookLM để tự động sinh video thuyết trình giới thiệu nội dung và xuất bản trực tiếp lên Douyin (TikTok Trung Quốc). (Đóng góp từ [@brianxiadong](https://github.com/brianxiadong/auto-paper-digest))

2. **CC Switch**

Ứng dụng desktop đa nền tảng hỗ trợ lập trình viên chuyển đổi nhanh các khóa API và mô hình AI nền tảng chạy ngầm cho các công cụ như Claude Code, Codex hay Gemini CLI chỉ với một cú click chuột. (Đóng góp từ [@farion1231](https://github.com/ruanyf/weekly/issues/8674))

3. **Công cụ AI phân tích danh sách nhạc NetEase Cloud Music**

Dịch vụ web miễn phí sử dụng trí tuệ nhân tạo để phân tích sâu gu âm nhạc và đưa ra các đánh giá tóm tắt về danh sách phát nhạc (playlist) cá nhân của người dùng trên nền tảng NetEase Cloud Music. (Đóng góp từ [@immotal](https://github.com/ruanyf/weekly/issues/8706))

## 资源

1. [Tra cứu thông điệp ghi trên chuỗi khối Bitcoin (EverMsg)](https://www.evermsg.com/zh)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026010902.webp)

Trang web hỗ trợ người dùng tìm kiếm và đọc các nội dung thông điệp dạng văn bản được ghi trực tiếp vào trường dữ liệu `OP_RETURN` của các khối giao dịch Bitcoin. Các thông tin này một khi đã được xác nhận ghi vào blockchain sẽ tồn tại vĩnh viễn và không thể bị sửa xóa. (Đóng góp từ [@blueslmj](https://www.evermsg.com/zh))

2. [Cây thư mục tiến hóa của động vật có vú (DeepTime Mammalia)](https://github.com/SeanWong17/Mammalia-tree)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011208.webp)

Dự án trực quan hóa giao diện web 2D/3D tương tác sinh động, giúp người xem dễ dàng tìm hiểu và khám phá chi tiết cây tiến hóa lịch sử kéo dài 200 triệu năm của lớp động vật có vú (Mammalia). (Đóng góp từ [@SeanWong17](https://github.com/ruanyf/weekly/issues/8688))

## 图片

1. **Quy trình sửa chữa vỏ tàu dưới lớp băng dày**

Tại vùng Yakutsk của Nga có một xưởng đóng tàu nằm sát vòng Cực Bắc. Vào mùa đông hàng năm, toàn bộ mặt nước sông khu vực bến tàu đều đóng băng hoàn toàn.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011001.webp)

Để có thể tiến hành sửa chữa bảo dưỡng vỏ tàu trong điều kiện mùa đông giá rét, các công nhân phải thực hiện việc đục khoét lớp băng để làm lộ ra phần đáy tàu cần sửa.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011002.webp)

Độ dày của lớp băng tự nhiên thường không đủ dày để chạm tới đáy tàu, do đó quy trình đục băng phải được tiến hành theo từng lớp: công nhân sử dụng máy cưa xích cắt bỏ lớp băng trên cùng, đợi dòng nước bên dưới tiếp tục đóng băng dày lên rồi tiếp tục cưa xuống lớp tiếp theo, lặp lại quy trình nhiều lần cho đến khi tiếp cận được đáy tàu.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011003.webp)

Có những trường hợp xưởng tàu yêu cầu đục những rãnh băng kéo dài dọc thân tàu.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011004.webp)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011005.webp)

Bức ảnh dưới đây chụp cận cảnh người thợ sửa chữa chui xuống phía dưới lớp băng để tiến hành hàn sửa vỏ tàu. Do điều kiện làm việc dưới hầm băng vô cùng khắc nghiệt và tiềm ẩn nhiều rủi ro nguy hiểm, mức lương chi trả cho các công nhân này thường rất cao.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011006.webp)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011007.webp)

## 言论

1.

Cảm xúc của tôi thế nào khi mã nguồn của mình bị các mô hình AI lớn tự động quét thu thập dữ liệu?

Tôi thực sự cảm thấy rất vui và chào đón điều đó. Tôi xem đây là sự tiếp nối lý tưởng cho sứ mệnh cả đời của mình: phổ cập hóa mã nguồn, hệ thống phần mềm và tri thức nhân loại.

Mô hình AI lớn giúp lập trình viên viết phần mềm nhanh hơn, tốt hơn và hiệu quả hơn, đồng thời mang lại cơ hội cạnh tranh công bằng cho các nhóm nhỏ trước các tập đoàn khổng lồ. Đây chính là những gì phong trào phần mềm mã nguồn mở đã làm được ở thập niên 90. Một công nghệ quan trọng như AI tuyệt đối không nên chỉ bị độc quyền nắm giữ trong tay một số ít tập đoàn công nghệ lớn.

-- Salvatore Sanfilippo (Antirez) – cha đẻ của dự án Redis chia sẻ quan điểm

2.

Ngay cả khi bạn là người hoài nghi và không tin tưởng vào công nghệ AI, việc trốn tránh hay bỏ qua nó hoàn toàn không mang lại bất kỳ lợi ích nào cho sự nghiệp của bạn.

Trước đây khi bạn thức đêm lập trình và nhìn thấy dự án vận hành trơn tru, cảm giác phấn khích tột độ dâng trào trong lồng ngực. Giờ đây, nếu biết cách khai thác hiệu quả công cụ AI, bạn sẽ có khả năng xây dựng được nhiều dự án lớn hơn với chất lượng tốt hơn. Niềm vui tự tay sáng tạo ra sản phẩm vẫn luôn được giữ nguyên vẹn và không hề bị suy giảm.

-- Salvatore Sanfilippo (Antirez) – cha đẻ của dự án Redis chia sẻ quan điểm

3.

Nếu bạn không viết lách, bạn chỉ tương đương với một máy trạng thái hữu hạn (finite state machine). Còn khi đặt bút viết, bạn sẽ sở hữu sức mạnh phi thường của một máy Turing (Turing machine).

-- Manuel Blum – nhà khoa học đoạt giải thưởng Turing danh giá

4.

Con người thường rơi vào trạng thái bế tắc trong cuộc sống vì 3 nguyên nhân chủ chốt: (1) thiếu hụt năng lực hành động thực tế, (2) hành động sai hướng đi, và (3) tâm lý ngồi chờ sung rụng (ảo tưởng khó khăn sẽ tự biến mất mà không chịu chủ động tìm giải pháp xử lý).

-- [《Khi bạn muốn tự kéo mình ra khỏi vũng lầy bế tắc》](https://www.experimental-history.com/p/so-you-wanna-de-bog-yourself)

## 往年回顾

[Bốn ghi chép chiêm nghiệm thời điểm cuối năm](https://www.ruanyifeng.com/blog/2025/01/weekly-issue-334.html) (#334)

[Nền tảng YouTube hiện lưu trữ tổng cộng bao nhiêu video?](https://www.ruanyifeng.com/blog/2023/12/weekly-issue-284.html) (#284)

[Năng lực tương tác trò chuyện của AI thực tế mạnh đến mức nào?](https://www.ruanyifeng.com/blog/2022/12/weekly-issue-234.html) (#234)

[Quy mô nhu cầu lưu trữ dữ liệu của các cơ quan chính phủ lớn cỡ nào?](https://www.ruanyifeng.com/blog/2021/11/weekly-issue-184.html) (#184)

(Hết)
