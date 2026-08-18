# Bản tin chia sẻ công nghệ (Số 362): Kỹ sư GitHub chia sẻ về thiết kế hệ thống

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/7408) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082101.webp)

Tàu thu hồi tên lửa đầu tiên của Trung Quốc mang tên "Tinh Tế Quy Hàng" (星际归航) đã hạ thủy thành công trong tháng này. Sàn boong 40m x 60m của con tàu sẽ được dùng làm bãi đáp cho tên lửa hạ cánh ngoài biển. Con tàu thuộc sở hữu của công ty hàng không vũ trụ tư nhân "iSpace" (星际荣耀). (Nguồn: [geekpark.net](https://www.geekpark.net/news/352799))

## GitHub 工程师谈系统设计

Tuần trước tôi đọc được một bài viết của kỹ sư cấp cao GitHub, [Sean Goedecke](https://www.seangoedecke.com/).

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081814.webp)

Tựa đề bài viết là [《Những gì tôi biết về thiết kế hệ thống tốt》](https://www.seangoedecke.com/good-system-design/).

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081818.webp)

Đọc xong, tôi thấy đây là bài viết rất chất lượng. Một kỹ sư GitHub thực chiến tổng kết kinh nghiệm, hướng dẫn cách thiết kế hệ thống tốt — không phải lý thuyết chung chung mà có nội dung cụ thể, thực tiễn. Dưới đây là một số trích dẫn đáng chú ý.

**1.**

Thiết kế chương trình (program design) là lắp ráp mã nguồn; thiết kế hệ thống (system design) là lắp ráp các dịch vụ.

Các thành phần trong thiết kế chương trình là biến, hàm, lớp... Các thành phần trong thiết kế hệ thống là máy chủ, cơ sở dữ liệu, cache, queue, event bus, proxy...

**2.**

Nếu một hệ thống hoạt động ổn định trong thời gian dài mà không xảy ra lỗi, thiết kế của nó là tốt.

Nếu bạn xem thêm vào mã nguồn và thốt ra: "Ồ, đơn giản hơn tôi tưởng" hoặc "Phần này không cần lo, dù có lỗi cũng dễ sửa" — thì thiết kế của nó là xuất sắc.

**3.**

Thiết kế hệ thống tốt luôn phát triển từ một hệ thống đơn giản đang hoạt động được. Tuyệt đối không cố gắng thiết kế một hệ thống phức tạp từ đầu từ con số không.

**4.**

Điểm khó nhất trong thiết kế hệ thống là **trạng thái (state)**. Hãy ưu tiên các thành phần không lưu trạng thái (stateless), và tối thiểu hóa số lượng "thành phần có trạng thái" (stateful components).

Sự phức tạp của trạng thái nằm ở chỗ bạn không thể đơn giản là khởi động lại dịch vụ. Khi có lỗi xảy ra, thường phải sửa trạng thái thủ công.

**5.**

Trạng thái cần được lưu trong cơ sở dữ liệu. Database là thành phần quan trọng nhất trong hệ thống, đóng vai trò quản lý trạng thái.

Mục tiêu thiết kế database là mỗi bảng phải dễ hiểu: Nhìn vào cấu trúc bảng là có thể hiểu ngay dữ liệu gì đang được lưu và tại sao.

Tuyệt đối tránh các cấu trúc bảng phức tạp — điều này sẽ mang lại vô vàn phức tạp về mặt code và giới hạn về hiệu suất.

**6.**

Database thường là nút thắt cổ chai (bottleneck) của hệ thống, vì mỗi request trang web có thể phải gọi database hàng chục, thậm chí hàng trăm lần theo thứ tự tuần tự.

Để tránh bottleneck, database có thể được cấu hình thành một node ghi (write node) và nhiều bản sao chỉ đọc (read replicas). Tất cả query đều gửi đến read replica; ghi dữ liệu mới gửi đến write node.

Giữa write node và read replica luôn có độ trễ nhân bản dữ liệu (replication lag). Nếu sau khi cập nhật một record bạn cần đọc lại ngay lập tức, hãy lưu dữ liệu đó vào bộ nhớ (memory) và đọc từ đó sau khi ghi database thành công.

**7.**

Các thao tác tốn thời gian cần được tách ra, đặt vào các background job (dịch vụ độc lập bên ngoài hệ thống chính), và xử lý theo hàng đợi.

Background job chủ yếu gồm hai thành phần: Một dịch vụ hàng đợi (queue service) và một trình thực thi job (job runner — lấy task từ queue và thực thi).

Phần mềm cho hàng đợi task có thể dùng Redis (cho các task cần thực thi nhanh) hoặc database thông thường (cho task không cần gấp).

**8.**

Khi tốc độ tạo ra dữ liệu và tốc độ đọc dữ liệu không khớp nhau, giải pháp kinh điển là **caching (bộ đệm)**.

Cách đơn giản nhất là lưu dữ liệu vào RAM; ngoài ra có thể dùng phần mềm lưu trữ key-value chuyên dụng như Redis hay Memcached — lợi thế là nhiều server có thể chia sẻ chung cache.

Kỹ sư junior muốn cache tất cả mọi thứ; kỹ sư senior muốn hạn chế dùng cache tối đa có thể. Lý do: Cache là nguồn gốc của trạng thái, không tránh khỏi phải xử lý kiểm tra tính nhất quán của trạng thái và xử lý cache hết hạn.

**9.**

Ngoài cache và background job, các hệ thống lớn thường có thêm **event bus (trung tâm sự kiện)**, phổ biến nhất là Kafka.

Event bus cũng là một hàng đợi, lưu trữ các thông báo dạng "một sự kiện nào đó đã xảy ra". Ví dụ: Người dùng đăng ký kích hoạt sự kiện "Tài khoản mới được tạo", sự kiện này được đặt vào event bus, sau đó event bus thông báo cho nhiều dịch vụ đăng ký nhận sự kiện đó: Gửi email chào mừng, tạo không gian cá nhân...

Event bus phù hợp khi mã nguồn phát sự kiện không cần biết các dịch vụ khác xử lý sự kiện đó như thế nào, hoặc khi lượng sự kiện rất lớn và không nhạy cảm về thời gian phản hồi.

Đừng lạm dụng event — thường thì cách đơn giản hơn là cho một dịch vụ gọi trực tiếp API của dịch vụ kia. Để dễ debug, tốt nhất là tập trung tất cả log vào một nơi, để có thể xem ngay phản hồi của dịch vụ khác.

**10. Kéo và Đẩy**

Khi dữ liệu cần được phân phối đến nhiều nơi, có hai lựa chọn: Kéo (pull) và đẩy (push).

Nhìn chung, kéo đơn giản hơn (hầu hết website dùng polling — kéo định kỳ); đẩy tiết kiệm tài nguyên hơn vì client không cần chủ động yêu cầu — khi dữ liệu backend thay đổi, server chủ động đẩy đến từng client.

Nếu bạn thực sự cần cung cấp dữ liệu mới nhất cho 1 triệu client (giống như Gmail), nên dùng đẩy hay kéo? Tùy tình huống. Nếu dùng đẩy, hãy đưa mỗi lần đẩy vào event queue và dùng một đội event handler lấy từ queue để đẩy. Nếu dùng kéo, hãy triển khai một đội (ví dụ 100 máy) cache server chỉ đọc tốc độ cao để xử lý toàn bộ lưu lượng đọc.

## 谷歌的两个 AI 新产品

Google tuần này công bố hai sản phẩm AI mới.

**1. [Imagen 4](https://aistudio.google.com/prompts/new_image)**

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081708.webp)

Đây là mô hình tạo ảnh từ văn bản (text-to-image) mới nhất của Google, có thể [sử dụng miễn phí](https://aistudio.google.com/prompts/new_image) trên trang chính thức. Xem thêm [bài giới thiệu chi tiết](https://developers.googleblog.com/en/announcing-imagen-4-fast-and-imagen-4-family-generally-available-in-the-gemini-api/).

Tôi thấy tốc độ tạo ảnh rất nhanh và chất lượng khá tốt (ví dụ như hình ảnh "robot cầm ván trượt đỏ" bên dưới).

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081707.webp)

**2. [Learning About](https://learning.google.com/experiments/learn-about/signup)**

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081805.webp)

Learning About là [nền tảng học tập mới](https://learning.google.com/experiments/learn-about?src=signup) của Google, sử dụng AI để tạo nội dung hướng dẫn học tập theo yêu cầu.

Chỉ cần nhập chủ đề bạn muốn học, ví dụ "Ngôn ngữ lập trình Java":

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081806.webp)

Hệ thống sẽ trả về một bài hướng dẫn tổng quan dễ hiểu:

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081807.webp)

Ngoài phần giới thiệu tổng quát, nó còn liệt kê các chủ đề học tập con để bạn có thể đi sâu hơn:

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081808.webp)

## 科技动态

（1）Bộ Nội vụ Anh thông báo sẽ trang bị **hệ thống nhận diện khuôn mặt** cho các xe cảnh sát trên toàn quốc.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081815.webp)

Xe cảnh sát sẽ quét khuôn mặt người đi đường trong khi di chuyển và đối chiếu với cơ sở dữ liệu của cảnh sát. Nếu phát hiện nghi phạm, hệ thống sẽ phát cảnh báo ngay.

Theo thông tin công bố, trong 12 tháng thử nghiệm tại London, công nghệ này đã giúp bắt giữ 580 nghi phạm.

（2）Nhiều người thích gửi bưu thiếp khi đi du lịch như một kỷ niệm đặc biệt.

Nhưng bưu thiếp truyền thống phải viết tay và chỉ truyền tải được văn bản — điều này trở nên lỗi thời trong thời đại smartphone.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081302.webp)

Một công ty Mỹ vừa ra mắt dịch vụ **Keeps** (hình trên). Người dùng lên website, tải ảnh lên và để lại một đoạn giọng nói (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081303.webp)

Dịch vụ sẽ in ảnh thành bưu thiếp với mã QR ở mặt sau, rồi gửi bưu thiếp đến địa chỉ người nhận bạn chỉ định. Khi nhận được, người nhận quét mã QR bằng điện thoại là có thể nghe lại giọng nói bạn đã để lại.

（3）Các bài viết trên Wikipedia tồn tại ở nhiều phiên bản ngôn ngữ khác nhau. Bạn có biết bài nào có nhiều phiên bản ngôn ngữ nhất không?

Thật bất ngờ, đó lại là trang về một nghệ sĩ gần như vô danh tên [David Woodard](https://en.wikipedia.org/wiki/Wikipedia:Wikipedia_Signpost/2025-08-09/Disinformation_report).

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081304.webp)

Trang về ông này có tới 335 phiên bản ngôn ngữ — nhiều hơn bất kỳ bài viết nào khác trên toàn bộ Wikipedia.

Hầu hết các phiên bản ngôn ngữ đó đều do một tài khoản tên Swmmng tạo ra, với cùng một địa chỉ IP, trong suốt hơn một thập kỷ.

Rõ ràng đây là hành vi tự quảng bá: Nghệ sĩ này đã cố tình tạo các trang Wikipedia về mình bằng hàng trăm ngôn ngữ để nổi tiếng. Hiện nay phần lớn các phiên bản đó đã bị xóa, chỉ còn lại 20 ngôn ngữ.

## 文章

1、[Dịch vụ AI miễn phí từ GitHub Models](https://github.blog/ai-and-ml/llms/solving-the-inference-problem-for-open-source-ai-projects-with-github-models/) (tiếng Anh)

Tôi vừa biết rằng GitHub cung cấp khả năng gọi API các mô hình AI hoàn toàn miễn phí, bao gồm GPT-4o, DeepSeek-R1, Llama 3 và nhiều mô hình khác, tuy có giới hạn về lượng sử dụng.

2、[Tạo mê cung bằng JavaScript](https://jrsinclair.com/articles/2025/joy-of-immutable-data-recursion-pure-functions-javascript-mazes/) (tiếng Anh)

Bài viết giải thích bằng ngôn ngữ thông thường một thuật toán đơn giản để sinh mê cung ngẫu nhiên và cung cấp cài đặt bằng JavaScript.

3、[Cloudflare không phải CDN thông thường](https://magecdn.com/blog/2025/08/11/cloudflare-not-a-cdn/) (tiếng Anh)

Cloudflare cung cấp CDN miễn phí với băng thông không giới hạn, vậy tại sao họ vẫn có gói CDN tính phí? Bài viết giải thích rằng ngoài băng thông, còn nhiều chỉ số hiệu suất CDN khác quan trọng không kém.

4、[Git xử lý file lớn như thế nào](https://tylercipriani.com/blog/2025/08/15/git-lfs/) (tiếng Anh)

Các file lớn vài chục MB không phù hợp để đưa vào repository Git. Nếu bắt buộc phải đưa vào, cần dùng extension Git LFS. Bài viết phân tích hạn chế của Git LFS và đề xuất hướng cải tiến.

5、[10 plugin VS Code không thể thiếu](https://www.xda-developers.com/vs-code-extensions-i-cant-live-without/) (tiếng Anh)

Tác giả giới thiệu 10 plugin VS Code mà ông đã sử dụng thường xuyên đến mức không thể làm việc thiếu chúng.

6、[Vấn đề với cửa sổ tắc nghẽn khởi đầu của TCP](https://jeclark.net/articles/tcp-initcwnd/?tag=performance) (tiếng Anh)

Giao thức TCP có cơ chế "cửa sổ tắc nghẽn" (congestion window) tự động điều chỉnh số lượng gói tin gửi đi dựa trên trạng thái mạng. Bài viết giải thích khái niệm này một cách dễ hiểu và đề xuất hướng cải tiến.

## 工具

1、[doxx](https://github.com/bgreenwell/doxx)

Công cụ dòng lệnh cho phép xem trực tiếp nội dung các file `.docx` ngay trong terminal mà không cần mở Word.

2、[IntraScribe](https://github.com/weynechen/intrascribe)

Nền tảng quản lý và cộng tác chuyển đổi giọng nói thành văn bản được thiết kế dành riêng cho môi trường mạng nội bộ (intranet) của doanh nghiệp và tổ chức. (Đóng góp từ [@weynechen](https://github.com/ruanyf/weekly/issues/7542))

3、[P2P Remote Desktop](https://github.com/miroslavpejic85/p2p)

Công cụ remote desktop Windows mã nguồn mở, chạy thẳng file thực thi là có thể kết nối điều khiển máy từ xa, không cần cài đặt hay cấu hình phức tạp. (Đóng góp từ [@miroslavpejic85](https://github.com/ruanyf/weekly/issues/7547))

4、[CuteClock](https://github.com/AkenClub/CuteClock)

Dự án phần cứng mã nguồn mở: Đồng hồ thông minh dựa trên chip ESP8266 hiển thị thời gian và thời tiết, hỗ trợ điều khiển bằng giọng nói qua trợ lý Xiaoai, kèm client Web và mini-program. (Đóng góp từ [@AkenClub](https://github.com/ruanyf/weekly/issues/7553))

5、[CleanYourMac](https://github.com/GitDzreal93/clean-your-mac)

Ứng dụng Mac mã nguồn mở hỗ trợ dọn dẹp hệ thống thông minh, sử dụng AI để phân tích và gợi ý các file nên xóa. (Đóng góp từ [@GitDzreal93](https://github.com/ruanyf/weekly/issues/7555))

6、[Next QR Code Generator](https://github.com/chromium-style-qrcode/next-qrcode-generator)

Tiện ích mở rộng mã nguồn mở cho Firefox tạo mã QR cho trang hiện tại theo phong cách tương tự Chrome. (Đóng góp từ [@liuliangsir](https://github.com/ruanyf/weekly/issues/7563))

7、[Translator 快速翻译](https://github.com/AnYi-0/Translator)

Plugin dịch thuật ngoại tuyến (offline) cho Chrome, dựa trên Translator API và Language Detector API mới của trình duyệt, không cần kết nối mạng để dịch. (Đóng góp từ [@AnYi-0](https://github.com/ruanyf/weekly/issues/7562))

8、[Jupyter Notebook to PDF](https://ipynbtopdf.net/)

Trang web chuyển đổi file `.ipynb` (Jupyter Notebook) sang các định dạng PDF, HTML và Python. (Đóng góp từ [@CurioChen77](https://github.com/ruanyf/weekly/issues/7587))

9、[Docker Pull Script](https://github.com/luckfu/docker_pull)

Script Python hỗ trợ tải Docker image từ nguồn mirror tùy chỉnh, hỗ trợ tải song song và cache thông minh (cập nhật tăng dần theo layer). (Đóng góp từ [@luckfu](https://github.com/ruanyf/weekly/issues/5931#issuecomment-3205330268))

10、[Make Graph](https://makegraph.app/editor)

Công cụ vẽ biểu đồ trực tuyến hỗ trợ nhiều loại biểu đồ phổ biến, có thể xuất ra định dạng SVG. (Đóng góp từ [@bimohxh](https://github.com/ruanyf/weekly/issues/7597))

Tham khảo thêm công cụ tương tự: [ChartFromText](https://chartfromtext.com/) — nhập dữ liệu dạng text, tự động sinh biểu đồ trực quan. (Đóng góp từ [@StevenWuHao](https://github.com/ruanyf/weekly/issues/7601))

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082104.webp)

## AI 相关

1、[OpenAI Progress](https://progress.openai.com/)

Dự án chính thức của OpenAI ghi lại hành trình phát triển AI: Cùng một câu lệnh nhắc, xem đầu ra thay đổi như thế nào qua từng năm.

2、[MCP Playground](https://mcpso.cc/kchat/index.html)

Ứng dụng web hoạt động như MCP client: Chỉ cần chỉ định mô hình AI và MCP server là có thể sử dụng trực tuyến ngay. (Đóng góp từ [@mcpexplorer](https://github.com/ruanyf/weekly/issues/7550))

3、[Coro Code](https://github.com/Blushyes/coro-code)

AI coding agent chạy trên terminal, là giải pháp mã nguồn mở thay thế cho Claude Code. (Đóng góp từ [@Blushyes](https://github.com/ruanyf/weekly/issues/7561))

4、[Claude Code Status Bar Monitor](https://github.com/leeguooooo/claude-code-usage-bar)

Plugin cho Claude Code hiển thị real-time lượng sử dụng còn lại và thời gian reset của các giới hạn. (Đóng góp từ [@leeguooooo](https://github.com/ruanyf/weekly/issues/7588))

## 资源

1、[Thư viện đọc diễn cảm ngữ văn tiểu/trung học](https://zedex.github.io/mandarin-reading-resource/)

Giao diện web tái tạo lại [Thư viện đọc diễn cảm ngữ văn tiểu/trung học của Đài Phát thanh Trung ương Trung Quốc](https://edu.cnr.cn/eduzt/ywkwsfsd/), phân loại bài đọc theo lớp và học kỳ. (Đóng góp từ [@ZedeX](https://github.com/ruanyf/weekly/issues/7556))

2、[Nền tảng kiểm tra phần cứng trực tuyến](https://volumeshader.org/zh)

Trang web kiểm tra nhiều loại phần cứng máy tính trực tiếp qua trình duyệt: GPU, màn hình, mạng, camera, âm thanh, chuột, bàn phím. (Đóng góp từ [@linhuaqian](https://github.com/ruanyf/weekly/issues/7552))

3、[Thi thử chứng chỉ vô tuyến nghiệp dư (2025)](https://github.com/AlliotTech/ham-exam-web)

Ứng dụng web thi thử và luyện tập trực tuyến dựa trên ngân hàng câu hỏi chính thức mới nhất dành cho kỳ thi lấy chứng chỉ vô tuyến nghiệp dư (ham radio). (Đóng góp từ [@AlliotTech](https://github.com/ruanyf/weekly/issues/7585))

4、[Citywalki](https://www.citywalki.com)

Trải nghiệm đi bộ, lái xe hoặc bay bằng drone ảo qua hơn 200 thành phố trên khắp thế giới. Sau khi chọn thành phố và phương thức di chuyển, nó sẽ phát video YouTube toàn màn hình tương ứng — trải nghiệm khá thú vị.

## 图片

1、[Chiếc lốp xe lăn lâu nhất thế giới](https://kottke.org/25/08/roll-on-you-crazy-tire)

Gợi ý xem [một video trên YouTube](https://www.youtube.com/watch?v=tLpQ5bcxouw).

Một nhóm nghệ sĩ leo lên một trong những đồi cát cao nhất ở Chile, thả lăn một chiếc lốp xe xuống từ đỉnh và quay toàn bộ hành trình bằng drone.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081710.webp)

Chiếc lốp xe lăn trên sa mạc gần như ba phút liên tục. Video ghi lại toàn bộ quá trình đó — vô cùng ngoạn mục và có tác dụng giải tỏa căng thẳng đặc biệt.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081711.webp)

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025081712.webp)

## 文摘

1、**Câu chuyện về Wozniak**

Ngày 11 tháng 8 năm nay là sinh nhật lần thứ 75 của Steve Wozniak, đồng sáng lập Apple.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082103.webp)

Diễn đàn Slashdot đăng lại tin tức về sinh nhật của ông. Có người bình luận, tiếc rằng nếu ông không bán cổ phần Apple, chắc chắn đã là một trong những người giàu nhất thế giới.

Chính Wozniak đọc được bình luận đó và đã trả lời trực tiếp:

> "Tôi đã bán và hiến tặng tất cả cổ phần Apple, vì tài sản và quyền lực không phải là mục tiêu sống của tôi.
>
> Tôi muốn có hạnh phúc và niềm vui. Tôi đã tài trợ cho nhiều bảo tàng và tổ chức nghệ thuật ở San Jose — nơi tôi sinh ra, họ còn đặt tên một con đường theo tên tôi.
>
> Hai mươi năm diễn thuyết công khai, thu nhập có thể đạt 10 triệu đô la. Như vậy là đủ với tôi."

Những lời này khiến người ta nhớ lại một cuốn sách về lịch sử Apple từng kể về Wozniak.

Từ thời còn đi học, ông đã không bao giờ để ý đến tiền bạc của mình. Sau khi giàu có, ông vẫn vậy.

Ông không bao giờ theo dõi chi tiêu của mình, cũng lười nghe lời khuyên về tài chính. Khi ai đó cần giúp đỡ, ông thường ký séc ngay tại chỗ.

Khác với Jobs giữ chặt cổ phần Apple, Wozniak đã tặng cổ phần trị giá 4 triệu đô la cho bố mẹ, chị và em trai, tặng thêm 2 triệu đô la cho bạn bè. Người cha một lần tìm thấy tờ séc 250.000 đô la chưa đổi tiền trong xe Wozniak, thở dài: "Một người như vậy không nên có nhiều tiền đến thế."

Có lần ông vào trụ sở Apple và tuyên bố lớn: "Luật sư của tôi khuyên đa dạng hóa đầu tư, vì vậy tôi vừa mua một rạp chiếu phim." Nhưng chuyện này gây ra ít rắc rối. Rạp nằm ở khu nghèo phía đông San Jose, chiếu một bộ phim băng đảng và bị cộng đồng phản đối. Ông tham dự vài buổi họp cộng đồng, lắng nghe cư dân địa phương, hứa rạp sẽ không chiếu phim bạo lực hay khiêu dâm. Sau đó ông ngồi một mình trong rạp tối vắng người, liên tục xem phim để làm kiểm duyệt viên.

## 言论

1、

Tôi dự định viết một cuốn sách về ngôn ngữ lập trình Gleam. Nhưng AI đã có thể giải thích Gleam cực kỳ rõ ràng, và còn có thể đáp ứng mọi yêu cầu của người đọc.

Dù tôi tự tin bản thân viết tốt hơn AI hiện tại, nhưng thực sự không có lý do gì để thuyết phục bản thân làm việc đó. Bạn bỏ ra hàng trăm giờ viết sách, số tiền kiếm được không xứng đáng với công sức đó.

Với AI, tôi không biết sau này động lực để người ta viết sách là gì nữa — có lẽ chỉ còn viết vì niềm vui thuần túy.

-- *Trích bài viết 《Cuộc khủng hoảng danh tính do AI gây ra》*

2、

Điều tôi không thể cưỡng lại là: Làm việc với Trung Quốc dễ hơn nhiều so với bất kỳ nơi nào khác trên thế giới. Tôi gửi email cho một người Trung Quốc, chắc chắn sẽ nhận được phản hồi trong vòng 24 giờ, thường là trong vòng 4 giờ.

Gửi email cho một công ty EU hay Mỹ, thường phải chờ nhiều ngày mới có hồi âm. Trong quá trình làm việc với các công ty Trung Quốc, tôi chưa bao giờ gặp tình trạng đó, dù chỉ một lần. Và hầu như các nền tảng thương mại điện tử B2B lớn của họ luôn cung cấp hỗ trợ khách hàng trực tuyến 24/7.

-- *Độc giả Hacker News*

3、

AI không làm giảm bớt nỗ lực bạn cần bỏ ra để thực sự nắm vững một kỹ năng mới — nó chỉ tạo ra ảo tưởng rằng bạn đã học được mà chẳng cần học.

-- *Trích bài viết 《AI tạo ra ảo giác kiểm soát》*

4、

Những chương trình đáng tin cậy và minh bạch thường không phục vụ lợi ích của người thiết kế chúng.

-- *Niklaus Wirth, nhà khoa học máy tính, người đoạt giải Turing*

## 往年回顾

- Số #315: [Bản tâm thư chia sẻ kinh nghiệm sau khi rời Google](https://www.ruanyifeng.com/blog/2024/08/weekly-issue-315.html)
- Số #265: [Công nghệ tiếp theo sau WiFi — LiFi truyền dữ liệu bằng ánh sáng](https://www.ruanyifeng.com/blog/2023/08/weekly-issue-265.html)
- Số #215: [Mô hình hành vi yêu thích nhất của internet](https://www.ruanyifeng.com/blog/2022/07/weekly-issue-215.html)
- Số #165: [Kỷ nguyên ứng dụng toàn ngăn xếp (Full-stack App)](https://www.ruanyifeng.com/blog/2021/07/weekly-issue-165.html)

(Hết)
