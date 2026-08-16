# Bản tin chia sẻ công nghệ (Số 298): Thời của các kỹ sư phần cứng lên ngôi

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần. (**[Thông báo] Thứ Sáu tuần sau nghỉ lễ 1/5, bản tin sẽ tạm dừng một số.**)

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/4204) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041903.webp)

Đây là địa điểm check-in cực hot gần đây - thang cuốn thời gian tại Vườn Bách thảo Thái Nguyên. Nơi này vốn là một khu mỏ khai thác than cũ, sau đó đã được chính quyền cải tạo xây dựng thành công công viên sinh thái đẹp mắt. (Nguồn: [QQ News](https://new.qq.com/rain/a/20240414A04RNY00))

## 轮到硬件工程师吃香了

Tuần này, tôi xin chia sẻ tới các bạn một [số liệu thống kê tuyển dụng tại Mỹ](https://twitter.com/aznweng/status/1780594562597081362) khá thú vị.

**Nhu cầu tuyển dụng kỹ sư phần cứng tại đây vừa thiết lập mức kỷ lục lịch sử mới.**

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042301.webp)

Theo báo cáo thống kê, trong tổng số các vị trí tuyển dụng của các tập đoàn công nghệ Internet tại Mỹ, nhóm ngành phần cứng chỉ chiếm khoảng 6% vào năm 2022, nhưng hiện nay tỷ lệ này đã tăng vọt lên tới 16%.

Đây là một hiện tượng chưa từng có tiền lệ. Điều này đồng nghĩa với việc cứ mỗi 5 kỹ sư phần mềm được tuyển dụng thì doanh nghiệp lại tuyển thêm 1 kỹ sư phần cứng - tỷ lệ cao kỷ lục chưa từng ghi nhận trước đây.

Cục diện hiện tại cho thấy các công ty công nghệ lớn nhỏ tại Mỹ đều đang khát nhân sự phần cứng. Các ông lớn như Google, Microsoft, Meta, Apple... lại càng ráo riết săn lùng nhân tài trong lĩnh vực này.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042302.webp)

Mặc dù thị trường Việt Nam không có các báo cáo thống kê chi tiết tương tự, nhưng xu hướng thực tế cũng diễn ra tương đối đồng điệu. Bạn chỉ cần truy cập các trang tin tuyển dụng công nghệ lớn và tìm kiếm từ khóa "kỹ sư phần cứng", hệ thống sẽ trả về rất nhiều kết quả tuyển dụng đi kèm mức lương vô cùng hấp dẫn. **Cơ hội việc làm cho mảng phần cứng đang gia tăng mạnh mẽ hơn bao giờ hết.**

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042303.webp)

Nguyên nhân nào dẫn đến sự lên ngôi đột ngột này của các kỹ sư phần cứng?

**Khởi nguồn gần như chắc chắn là AI**. Toàn bộ ngành công nghiệp Internet đang ồ ạt khởi động các dự án AI, các doanh nghiệp đều vội vã triển khai để tránh bị tụt lại phía sau trong làn sóng công nghệ mới này.

Đối với phần mềm AI, sự xuất hiện của nhiều mô hình nguồn mở chất lượng giúp các lập trình viên dễ dàng tự chạy thử nghiệm dựa trên tài liệu hướng dẫn. Do đó bất kỳ lập trình viên nào, kể cả các lập trình viên Frontend, cũng có thể nhanh chóng học hỏi và chuyển hướng sang phát triển ứng dụng AI.

Tuy nhiên, phần cứng hạ tầng lại là một bài toán hoàn toàn khác, bắt buộc phải có sự tham gia của các chuyên gia phần cứng có chuyên môn sâu. Công nghệ AI không thể vận hành nếu thiếu năng lực tính toán phần cứng - một yếu tố vật lý 100% mà phần mềm không thể tự sản sinh.

Để tự xây dựng năng lực tính toán độc lập, các doanh nghiệp Internet cần đầu tư thiết kế chip AI chuyên dụng và hệ thống máy chủ AI tối ưu. Nhiều doanh nghiệp thậm chí tự nghiên cứu thiết kế các chip tích hợp chuyên dụng ASIC hoặc FPGA, và các dự án này đều phụ thuộc hoàn toàn vào năng lực của các kỹ sư phần cứng. **Việc đầu tư nguồn tiền khổng lồ vào AI bắt buộc phải đi kèm tuyển dụng đội ngũ kỹ sư phần cứng tương xứng để xây dựng năng lực tính toán hạ tầng.**

Ngược lại, nguồn cung kỹ sư phần cứng trên thị trường lại vô cùng khan hiếm do quy trình đào tạo ngành này rất phức tạp. Một kỹ sư phần cứng giỏi đòi hỏi kiến thức nền tảng vững vàng về mạch điện tử, hiểu biết sâu về kiến trúc máy tính đi kèm nhiều năm kinh nghiệm thực hành thực tế. Do đó các doanh nghiệp thường gặp rất nhiều khó khăn để tìm kiếm ứng viên phù hợp, khiến các tin tuyển dụng phải treo tuyển trong thời gian dài và làm gia tăng sự mất cân bằng cung cầu trên thị trường.

Trái ngược với sự bùng nổ của mảng phần cứng, thị trường tuyển dụng kỹ sư phần mềm lại có phần ảm đạm hơn.

Dù tổng số lượng vị trí tuyển dụng phần mềm vẫn vượt trội so với phần cứng, nhưng tốc độ tăng trưởng đã chậm lại rõ rệt, đặc biệt là ở nhóm các vị trí dành cho sinh viên mới ra trường hoặc lập trình viên ít kinh nghiệm (Junior). So với giai đoạn đỉnh cao của những năm trước, nhu cầu tuyển dụng đã sụt giảm rất nhiều.

Có nhiều nguyên nhân lý giải cho sự suy giảm nhu cầu đối với các kỹ sư phần mềm (Junior):

> （1）Sự phát triển mạnh mẽ của mô hình SaaS và dịch vụ điện toán đám mây cho phép doanh nghiệp mua sẵn các giải pháp phần mềm hoàn thiện thay vì tự xây dựng mã nguồn từ đầu.
> 
> （2）Thị trường điện thoại thông minh dần bão hòa dẫn đến nhu cầu phát triển ứng dụng di động mới giảm sút.
> 
> （3）Các trung tâm đào tạo ngắn hạn liên tục cung cấp lượng lớn lập trình viên Junior ra thị trường gây nên tình trạng thừa nguồn cung.
> 
> （4）Sự hỗ trợ đắc lực từ các công cụ AI trong việc viết mã nguồn cơ bản giúp giảm nhu cầu tuyển dụng lập trình viên ít kinh nghiệm.

Trong tương lai, nếu năng lực lập trình của các công cụ AI tiếp tục được nâng cấp để xử lý tốt các tác vụ logic phức tạp hơn, xu hướng này dự báo sẽ tiếp tục kéo dài: nhu cầu kỹ sư phần cứng duy trì ở mức cao trong khi mảng phần mềm dần đi vào quỹ đạo bình ổn.

Điều đáng ngại là các cơ hội việc làm cho lập trình viên Junior sẽ ngày càng thu hẹp, nhu cầu tuyển dụng chủ yếu tập trung vào phân khúc nhân sự có kinh nghiệm từ trung đến cao cấp. Thực trạng này đặt ra bài toán khó cho việc đào tạo thế hệ lập trình viên kế cận khi họ thiếu đi môi trường thực hành thực tế tại doanh nghiệp để tự nâng cấp năng lực bản thân lên các cấp độ cao hơn.

## 科技动态

1、[Hạt gạo hương vị thịt bò nuôi cấy tế bào của các nhà khoa học Hàn Quốc](https://www.nature.com/articles/d41586-024-00398-w)

Các nhà nghiên cứu Hàn Quốc đã nuôi cấy thành công tế bào cơ thịt bò trực tiếp trên các hạt gạo, tạo ra loại gạo độc đáo mang hương vị thịt bò.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021903.webp)

Quy trình thực hiện bằng cách phủ một lớp dung dịch dinh dưỡng lên hạt gạo, sau đó cấy tế bào cơ và mỡ bò lên bề mặt và để chúng phát triển tự nhiên trong khoảng một tuần để hình thành hạt gạo thịt bò.

Sản phẩm thu được có màu hồng nhạt đặc trưng của dung dịch dinh dưỡng nuôi cấy tế bào, do bản chất tế bào cơ bò nuôi cấy vốn không có màu.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021904.webp)

Loại gạo này giúp bổ sung hàm lượng dinh dưỡng cao cho hạt gạo thông thường. Người dùng chỉ cần ăn một bát cơm là đã được bổ sung đầy đủ cả tinh bột và protein động vật, rất phù hợp làm khẩu phần ăn dã chiến cho quân đội hoặc giúp giảm thiểu tác động tiêu cực của ngành chăn nuôi gia súc truyền thống đến môi trường.

2、[Thiết kế thiết bị bay dạng vòng tròn độc đáo của startup Pháp](https://aeronde.com/index_en.html)

Một công ty khởi nghiệp của Pháp đã chế tạo thành công mẫu thiết bị bay cá nhân có hình dạng vòng tròn khổng lồ độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042408.webp)

Cấu trúc chính của thiết bị là một vòng tròn bơm căng khí Heli màu trắng lớn để tạo lực nâng, xung quanh vòng được bố trí các cánh quạt điều khiển bằng động cơ điện.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042409.webp)

Thiết bị có tải trọng thiết kế khoảng 200 kg, đủ không gian cho hai người ngồi. Tuy nhiên khoang hành khách thực chất chỉ là một chiếc ghế băng dài treo lơ lửng phía dưới vòng tròn khí, đòi hỏi hành khách phải thực sự dũng cảm khi trải nghiệm.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042410.webp)

3、[Giải pháp xử lý các vệt ố màu đen trên tường nhà ga tàu điện ngầm London](https://www.ianvisits.co.uk/articles/elizabeth-line-testing-ways-of-banishing-its-ghosts-in-the-walls-68642/)

Hệ thống ghế chờ tại các ga tàu điện ngầm London chủ yếu là các băng ghế inox không gỉ lắp đặt áp sát trực tiếp vào mảng tường bê tông phía sau.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010304.webp)

Do tần suất hành khách ngồi chờ lớn, sau một thời gian dài sử dụng, mảng tường phía sau ghế bị ố đen tạo thành các vệt bóng lưng người trông rất kém thẩm mỹ và không đảm bảo vệ sinh.

Để khắc phục tình trạng này, ban quản lý ga đã thử nghiệm nhiều giải pháp. Việc thay thế toàn bộ hệ thống ghế có tựa lưng đòi hỏi chi phí đầu tư rất lớn và phức tạp. Cuối cùng, họ đã chọn giải pháp đơn giản và tiết kiệm nhất: dán các tấm decal bảo vệ đè lên khu vực vệt ố.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010305.webp)

Các tấm dán bảo vệ có chi phí rẻ, dễ thi công và được thiết kế in ấn nhiều hoa văn họa tiết đẹp mắt trang trí cho nhà ga. Khi các tấm dán bị cũ hoặc bong tróc, nhân viên chỉ cần lột ra và thay thế bằng tấm dán mới.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010306.webp)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010307.webp)

## Bài viết

1\. [Nội dung chi tiết bài phỏng vấn mới nhất của nhà sáng lập Linux Linus Torvalds](https://new.qq.com/rain/a/20240422A04OR300)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042402.webp)

Bản dịch tiếng Trung bài chia sẻ mới nhất của cha đẻ Linux Linus Torvalds, tập trung thảo luận về sự cố cài cắm cửa sau xz gần đây và những nhận định cá nhân của ông về xu hướng phát triển của công nghệ AI.

2\. [Ứng dụng CSS Grid thiết kế bố cục tràn viền full-bleed chuyên nghiệp](https://www.joshwcomeau.com/css/full-bleed/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030606.webp)

Bài viết hướng dẫn chi tiết cách khai thác các thuộc tính CSS Grid để thiết kế giao diện bố cục tràn viền (full-bleed) - cho phép hình ảnh hoặc các khối nội dung đặc biệt tự động căn rộng chiếm trọn chiều rộng của trang màn hình.

3\. [Hướng dẫn đăng ký và cài đặt chứng chỉ bảo mật ZeroSSL miễn phí](https://linuxiac.com/zerossl-how-to-install-ssl-certificate/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122801.webp)

Tương tự như giải pháp Let's Encrypt, dịch vụ ZeroSSL cung cấp chứng chỉ bảo mật SSL/TLS hoàn toàn miễn phí cho trang web. ZeroSSL sở hữu giao diện quản lý web trực quan thân thiện và bổ sung một số tính năng nâng cao có phí. Bài viết hướng dẫn chi tiết các bước đăng ký.

4\. [Kinh nghiệm xây dựng và tối ưu trang web Frontend trong 10 giờ cùng GitHub Copilot](https://ameow.xyz/archives/develop-a-frontend-site-with-copilot)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042413.webp)

Tác giả chia sẻ câu chuyện thực tế dù chỉ có kiến thức cơ bản về Frontend nhưng nhờ ứng dụng hiệu quả công cụ hỗ trợ AI GitHub Copilot đã hoàn thành xuất sắc một dự án React Frontend chỉ trong vòng 10 tiếng, đồng thời tóm tắt các mẹo viết câu lệnh prompts hiệu quả cho Copilot. (Đóng góp của [@LeslieLeung](https://github.com/ruanyf/weekly/issues/4340))

5\. [Chia sẻ chiến lược xây dựng và tăng trưởng người theo dõi trên Twitter hiệu quả](https://mp.weixin.qq.com/s/2y463r9G4hnsIc0c2ig7dA)（Tiếng Trung）

Tác giả chia sẻ kinh nghiệm vận hành tài khoản Twitter cá nhân đạt cột mốc 8.000 người theo dõi chỉ sau vài tháng dù duy trì tần suất đăng bài tương đối thấp, đồng thời đúc kết các quy tắc tối ưu nội dung để thu hút tương tác. (Đóng góp của [@dongan-beta](https://github.com/ruanyf/weekly/issues/4298))

6\. [So sánh các phương pháp quản lý lỗi runtime trong JavaScript, Go và Rust](https://betterprogramming.pub/typescript-with-go-rust-errors-no-try-catch-heresy-da0e43ce5f78)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023123006.webp)

Bài viết thực hiện phân tích và so sánh các triết lý thiết kế cơ chế xử lý lỗi hệ thống khi vận hành của ba ngôn ngữ lập trình JavaScript, Go và Rust, đồng thời đưa ra góc nhìn đề xuất JavaScript nên tham khảo định hướng quản lý lỗi của Go và Rust để tối ưu chất lượng mã nguồn.

7\. [Giới thiệu hai công cụ dòng lệnh thay thế và đổi tên tệp tin hàng loạt rep và ren](https://blog.robenkleene.com/2023/12/26/introducing-rep-ren/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023123007.webp)

Tác giả giới thiệu hai tiện ích CLI do ông phát triển giúp phối hợp nhịp nhàng với các lệnh grep và find để tìm kiếm, thay thế nội dung văn bản và đổi tên file hàng loạt một cách nhanh chóng.

## AI 相关

1\. [Meta AI chính thức ra mắt phiên bản trợ lý AI tích hợp mô hình Llama 3](https://www.meta.ai/)

Meta công bố phát hành dịch vụ trợ lý AI miễn phí xây dựng trên mô hình Llama 3 mới nhất, hỗ trợ tốt các tác vụ trò chuyện và tạo hình ảnh từ văn bản chất lượng cao. Chi tiết xin đọc thêm [báo cáo giới thiệu chính thức từ Meta](https://about.fb.com/news/2024/04/meta-ai-assistant-built-with-llama-3/).

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041901.webp)

Đây được đánh giá là đối thủ cạnh tranh đáng gờm nhất của OpenAI thời điểm hiện tại.

Bên cạnh đó, Meta cũng cung cấp trang web trải nghiệm chatbot Llama chuyên dụng tại địa chỉ [llama3.dev](https://llama3.dev/) cho phép tùy chọn các phiên bản mô hình khác nhau. (Đóng góp của [@AICodeHunt](https://github.com/ruanyf/weekly/issues/4342))

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042206.webp)

2\. [DuckDuckGo AI Chat (Trình duyệt tìm kiếm tích hợp tính năng chat AI bảo mật)](https://duckduckgo.com/?q=DuckDuckGo&ia=chat)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042005.webp)

Trình duyệt bảo mật DuckDuckGo giới thiệu tính năng trò chuyện AI hoàn toàn miễn phí cho người dùng, hỗ trợ bởi các mô hình GPT-3.5 Turbo và Claude 1.2 chạy ngầm.

3\. [LLM Pricing (Trình so sánh giá và thông số các mô hình ngôn ngữ lớn)](https://llmpricecheck.com/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042006.webp)

Trang web hỗ trợ lập trình viên so sánh chi tiết bảng giá API và các thông số kỹ thuật của các mô hình LLM phổ biến hiện nay, đi kèm link dùng thử trực quan. (Đóng góp của [@lvwzhen](https://github.com/ruanyf/weekly/issues/4307))

4\. [Image to Text (Công cụ phân tích mô tả nội dung hình ảnh bằng AI)](https://imagetotext.cfd/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041902.webp)

Dịch vụ trực tuyến cho phép người dùng upload ảnh để AI tự động phân tích và trả về đoạn mô tả nội dung bằng tiếng Anh, đồng thời tích hợp tính năng nhận diện chữ viết OCR trên ảnh.

Một dịch vụ tương tự khác bạn đọc có thể tham khảo là [Image Describer](https://imagedescriber.online/).

5\. [OutfitAnyone AI (Mô hình AI hỗ trợ thử trang phục lên người mẫu)](https://github.com/ihmily/outfit-anyone)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042415.webp)

Mô hình AI hỗ trợ tự động lồng ghép hình ảnh quần áo phẳng lên cơ thể người mẫu ảo để hiển thị kết quả thử đồ trực quan. (Đóng góp của [@ihmily](https://github.com/ruanyf/weekly/issues/4297))

6\. [Lười nhân khách phục (Phần mềm chăm sóc khách hàng tự động bằng AI)](https://github.com/lrhh123/ChatGPT-On-CS)

Giải pháp chatbot tự động phản hồi khách hàng ứng dụng AI dành riêng cho các chủ shop kinh doanh trên các nền tảng WeChat, Taobao (Qianniu), Douyin (Doudian)... (Đóng góp của [@alsritter](https://github.com/ruanyf/weekly/issues/4308))

7\. [Dive Into Knowledge (Trình tổng hợp thông tin tìm kiếm thông minh)](https://openperplex.com/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042207.webp)

Dịch vụ web ứng dụng AI để tự động đọc, phân tích và tóm tắt lại các kết quả tìm kiếm từ internet trả về câu trả lời súc tích nhất cho người dùng.

8\. [Giáo trình lý thuyết và thực hành Đại học mô hình ngôn ngữ lớn LLM](https://llmbook-zh.github.io/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042305.webp)

Cuốn sách điện tử chia sẻ miễn phí cung cấp các kiến thức toàn diện về công nghệ LLM dành cho người mới bắt đầu, được biên soạn bởi chính đội ngũ tác giả của báo cáo khoa học nổi tiếng "A Survey of Large Language Models". (Đóng góp của [@acelit](https://github.com/ruanyf/weekly/issues/4330))

9\. [AI Image Generator (Ứng dụng tạo hình ảnh AI giao diện tối giản)](https://github.com/amin2312/AI-Image-Generator)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042414.webp)

Phần mềm hỗ trợ triển khai cục bộ giao diện tạo ảnh nghệ thuật từ văn bản kết nối tới các dịch vụ API của DALL-E hoặc Stable Diffusion. (Đóng góp của [@amin2312](https://github.com/ruanyf/weekly/issues/4345))

10\. [RMBG (Công cụ mã nguồn mở hỗ trợ xóa nền hình ảnh tự động)](https://github.com/zhbhun/rmbg)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042501.webp)

Dự án mã nguồn mở hỗ trợ tự động tách nền hình ảnh (remove background) hiệu quả bằng AI. (Đóng góp của [@zhbhun](https://github.com/ruanyf/weekly/issues/4347))

Một dịch vụ trực tuyến có tính năng tương đương khác là [công cụ tách nền AI Weidaobang (未道帮 AI 抠图)](https://cutout.aiwave.cc/). (Đóng góp của [@wytxer](https://github.com/ruanyf/weekly/issues/4356))

## 工具

1\. [Lan Mouse (Công cụ chia sẻ chuột và bàn phím trong mạng nội bộ)](https://github.com/feschber/lan-mouse)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010703.webp)

Phần mềm mã nguồn mở cho phép người dùng điều khiển đồng thời nhiều máy tính trong cùng một mạng LAN chỉ bằng một bộ chuột và bàn phím vật lý duy nhất.

2\. [UnoCssUi (Bộ thư viện UI thành phần nguyên tử tối giản)](https://github.com/cherryful/unocss-ui)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041904.webp)

Bộ thư viện giao diện thành phần (component library) phát triển trên nền Vue 3, UnoCSS và Tailwind CSS theo triết lý thiết kế nguyên tử hóa (atomic CSS) mà không phụ thuộc thêm thư viện ngoài nào khác. (Đóng góp của [@szluyu99](https://github.com/ruanyf/weekly/issues/4294))

3\. [drawDB (Trình thiết kế sơ đồ thực thể cơ sở dữ liệu trực tuyến)](https://github.com/drawdb-io/drawdb)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040703.webp)

Công cụ mã nguồn mở hỗ trợ vẽ sơ đồ quan hệ cơ sở dữ liệu (ERD) trực quan trực tiếp trên trình duyệt và tự động xuất file câu lệnh SQL tương ứng. (Đóng góp của [@yingming006](https://github.com/ruanyf/weekly/issues/4314))

4\. [vscode-highlight-text (Tiện ích tùy biến bôi màu hiển thị code trên VS Code)](https://github.com/Simon-He95/vscode-highlight-text)

Extension trên VS Code hỗ trợ lập trình viên tự cấu hình các quy tắc tô màu làm nổi bật (syntax highlighting) các từ khóa hoặc đoạn text đặc thù cho bất kỳ ngôn ngữ hay framework nào. (Đóng góp của [@Simon-He95](https://github.com/ruanyf/weekly/issues/4302))

5\. [Easy GitHub 2FA authentication (Tiện ích hỗ trợ tự động điền mã xác thực GitHub)](https://github.com/Dolov/chrome-github-2fa)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042304.webp)

Tiện ích mở rộng trình duyệt mã nguồn mở hỗ trợ tự động nhận diện và điền nhanh mã xác thực hai yếu tố (2FA) khi đăng nhập tài khoản GitHub. (Đóng góp của [@Dolov](https://github.com/ruanyf/weekly/issues/4328))

6\. [JavaVision (Hệ thống thị giác máy tính phát triển bằng Java)](https://gitee.com/giteeClass/java-vision)

Dự án thị giác máy tính mã nguồn mở viết bằng ngôn ngữ Java, tích hợp các tính năng cốt lõi như nhận diện vật thể, nhận diện khuôn mặt và tìm kiếm ảnh tương tự, hỗ trợ triển khai cục bộ và gọi lệnh qua Web API. (Đóng góp của [@javpower](https://github.com/ruanyf/weekly/issues/4343))

7\. [Shion (Phần mềm ghi nhận và phân tích thời gian làm việc cá nhân)](https://github.com/shion-app/shion)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042502.webp)

Ứng dụng mã nguồn mở trên Windows giúp tự động theo dõi, thống kê thời gian người dùng tương tác với các ứng dụng khác nhau và đồng bộ lịch sử duyệt web để phân tích hiệu suất làm việc cá nhân. (Đóng góp của [@hanaTsuk1](https://github.com/ruanyf/weekly/issues/4350))

8\. [Chat2DB (Công cụ quản lý và tương tác cơ sở dữ liệu thông minh)](https://github.com/chat2db/Chat2DB)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042503.webp)

Trình quản lý cơ sở dữ liệu đa nền tảng mã nguồn mở, cung cấp phiên bản app máy tính và bản web client giúp quản trị viên dễ dàng truy vấn và thao tác trên nhiều hệ quản trị CSDL khác nhau. (Đóng góp của [@JerryFan626](https://github.com/ruanyf/weekly/issues/4349))

9\. [Teable (Giải pháp cơ sở dữ liệu không mã nguồn mở thay thế Airtable)](https://github.com/teableio/teable)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042504.webp)

Dự án mã nguồn mở thay thế cho Airtable, hỗ trợ người dùng xây dựng các ứng dụng quản lý dữ liệu dạng bảng không cần viết code (no-code) phát triển trên nền cơ sở dữ liệu PostgreSQL, mang lại tốc độ phản hồi cực nhanh. (Đóng góp của [@yingming006](https://github.com/ruanyf/weekly/issues/4352))

10\. [main-thread-scheduling (Thư viện tối ưu điều phối luồng xử lý chính trong JS)](https://github.com/astoilkov/main-thread-scheduling)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010602.webp)

Mô-đun JS hỗ trợ tối ưu điều phối các tác vụ tính toán nặng chạy trực tiếp trên main thread mà hoàn toàn không gây tắc nghẽn luồng xử lý chính, giúp giao diện UI của trang web duy trì khả năng tương tác mượt mà với người dùng. Cấu trúc mã nguồn của dự án sở hữu giá trị học tập kỹ thuật rất tốt.

## 资源

1\. [Tìm hiểu trực quan về mô hình nhúng từ Word2vec](https://cloud.tencent.com/developer/article/1430171)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042003.webp)

Một bài phân tích chi tiết giới thiệu cơ chế vận hành của công nghệ nhúng từ Word2vec thông qua các hình vẽ minh họa và ví dụ trực quan dễ hiểu. Bạn đọc có thể tham khảo thêm [phiên bản tiếng Anh gốc tại đây](https://jalammar.github.io/illustrated-word2vec/).

2\. [Cẩm nang thực hành phát triển và thương mại hóa sản phẩm của Hard Hacker](https://github.com/hardhackerlabs/book)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042208.webp)

Cuốn sách điện tử mã nguồn mở chia sẻ chi tiết hành trình phát triển dự án thực tế [Podwise](https://podwise.ai/) từ khâu định hình ý tưởng cho đến khi gặt hái doanh thu ARR 12.000 USD thành công chỉ trong vòng hai tháng. (Đóng góp của [@SaitoWu](https://github.com/ruanyf/weekly/issues/4322))

3\. [Search for John (Trình tìm kiếm thông tin tổng hợp đa nền tảng)](https://www.searchforjohn.com/)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024020301.webp)

Một dịch vụ tìm kiếm thông tin tối giản hỗ trợ tổng hợp và lọc các kết quả trả về từ nhiều công cụ tìm kiếm phổ biến khác nhau, mang lại trải nghiệm tìm kiếm rất tốt.

4\. [Giáo trình nhập môn Mạng máy tính đại học (An Introduction to Computer Networks)](https://intronetworks.cs.luc.edu/)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100518.webp)

Cuốn sách giáo trình đại học giới thiệu các kiến thức cơ bản về mạng máy tính được chia sẻ đọc trực tuyến miễn phí bằng tiếng Anh.

## 图片

1\. [Hình ảnh ấn tượng về khoảnh khắc chim bay ngang qua hiện tượng nhật thực](https://petapixel.com/2024/04/21/how-a-photographer-captured-his-spectacular-dream-eclipse-photo/)

4/8 vừa qua, hiện tượng nhật thực toàn phần kỳ thú đã diễn ra tại khu vực Bắc Mỹ. Nhiều nhiếp ảnh gia chuyên nghiệp trên thế giới đã chuẩn bị kỹ lưỡng thiết bị từ rất sớm để săn tìm khoảnh khắc này.

Một nhiếp ảnh gia chuyên chụp ảnh chim muông đã di chuyển đến một hòn đảo nhỏ hoang vắng tại Mexico.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042403.webp)

Hòn đảo là nơi cư ngụ của loài chim chiến lớn (frigatebirds).

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042404.webp)

Nhiếp ảnh gia muốn ghi lại phản ứng tự nhiên của đàn chim khi bầu trời đột ngột tối sầm do nhật thực toàn phần.

Và vào ngày đặc biệt đó, ông đã xuất sắc chụp lại được những bức ảnh tuyệt đẹp làm say lòng người.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042405.webp)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042406.webp)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042407.webp)

2\. [Tác phẩm điêu khắc nghệ thuật trên lá cây](https://lito-leafart.com/)

Một nghệ sĩ Nhật Bản đã sáng tạo nên bộ sưu tập các tác phẩm nghệ thuật chạm khắc thủ công vô cùng tinh xảo trực tiếp trên bề mặt các lá cây xanh.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111202.webp)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111203.webp)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111204.webp)

## ✍️ Bài đọc thêm

### Phân tích những lợi ích sức khỏe và vận động của tất năm ngón

Tôi đã duy trì thói quen sử dụng tất năm ngón (toe socks) liên tục trong suốt 8 năm qua và muốn chia sẻ tới các bạn những trải nghiệm tuyệt vời của loại tất này.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062816.webp)

（1）Tất năm ngón mang lại cấu trúc thoải mái hơn cho các ngón chân. Khi mang tất này, các ngón chân được tự do co giãn và vận động độc lập thay vì bị bó chặt ép sát vào nhau như khi sử dụng các loại tất thông thường.

（2）Tất năm ngón giúp tăng khả năng thăng bằng. Khi diện tích tiếp xúc của bàn chân với mặt đất được mở rộng tối đa, cơ thể sẽ có khả năng thăng bằng tốt hơn. Ngay cả khi kết hợp với các đôi giày thể thao thông thường, tôi vẫn cảm nhận được độ vững chãi rõ rệt.

（3）Ngăn ngừa hiện tượng ra mồ hôi kẽ chân. Các loại tất truyền thống thường làm tích tụ mồ hôi ẩm ở các khe ngón chân gây cảm giác bí bách khó chịu, trong khi tất năm ngón giải quyết triệt để vấn đề này nhờ lớp vải bao bọc riêng biệt từng ngón.

（4）Hạn chế phồng rộp da chân khi di chuyển đường dài. Đây là ưu điểm cực kỳ quan trọng đối với các vận động viên chạy marathon hoặc người thích đi bộ dã ngoại (trekking). Sự cọ xát trực tiếp giữa da ngón chân với nhau nay được thay thế bằng sự ma sát mềm mại giữa các lớp vải tất.

（5）Độ bám của tất tốt hơn và hạn chế tình trạng tất bị trượt tuột ra khỏi gót chân.

Hiện nay tất năm ngón vẫn chưa thực sự phổ biến do quy trình công nghệ dệt may phức tạp hơn khiến giá thành sản xuất cao hơn và đa số người dùng chưa quen với thiết kế lạ mắt này. Tuy nhiên tôi đã khuyên nhiều người bạn dùng thử và họ đều phản hồi rất tích cực, vì vậy bạn cũng nên thử trải nghiệm một lần.

## Lịch sử tuần này

- 2023年（第 251 期）：[Góc nhìn phần cứng: Đánh giá và giới thiệu các dòng máy tính đơn bản (single-board computers) do Trung Quốc sản xuất](https://www.ruanyifeng.com/blog/2023/04/weekly-issue-251.html)
- 2022年（第 201 期）：[Nhận định chính sách: Khuyến nghị Trung Quốc cần thành lập Bộ phụ trách ngành công nghiệp bán dẫn](https://www.ruanyifeng.com/blog/2022/04/weekly-issue-201.html)
- 2021年（第 151 期）：[Tìm hiểu công nghệ: NFT là gì và liệu có khả năng kiếm tiền từ NFT?](https://www.ruanyifeng.com/blog/2021/03/weekly-issue-151.html)
- 2020年（第 101 期）：[Góc nhìn Internet: Nhận định về thời kỳ kết nối internet đã không còn là tài nguyên khan hiếm](https://www.ruanyifeng.com/blog/2020/04/weekly-issue-101.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
