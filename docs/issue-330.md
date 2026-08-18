# Bản tin chia sẻ công nghệ (Số 330): Lý Khai Phục hệ thống hóa kiến thức Trí tuệ nhân tạo

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/5610) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121703.webp)

Công viên ngọc hồ Lương Chử tại Hàng Châu chính thức mở cửa đón du khách vào tháng trước. Ngôn ngữ thiết kế của công viên mang tính biểu tượng sâu sắc, biểu trưng cho sự kết nối giao thoa giữa văn hóa Lương Chử cổ xưa và văn hóa dòng sông Kinh Hàng Vận Hà lịch sử. (Nguồn: [163.com](https://www.163.com/dy/article/JJI2MD7C0514ETGI.html))

## 李开复梳理人工智能

Thời gian vừa qua, tôi có đọc hai cuốn sách rất nổi tiếng của Tiến sĩ Lý Khai Phục (Kai-Fu Lee): *《AI · Tương lai》* (Nhà xuất bản Nhân dân Chiết Giang, 2018) và *《AI · 10 viễn cảnh cho tương lai chúng ta》* (Nhà xuất bản Nhân dân Chiết Giang, 2022).

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121701.webp)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121702.webp)

Cả hai cuốn sách này đều được biên soạn hướng đến đối tượng độc giả phổ thông nhằm giải thích bức tranh toàn cảnh về công nghệ trí tuệ nhân tạo (AI). Đây không phải là những tài liệu kỹ thuật chuyên sâu, tuy nhiên có nhiều chương mục phân tích và làm sáng tỏ các khái niệm nền tảng của AI rất sâu sắc.

Tác giả đã ứng dụng những thuật ngữ vô cùng phổ thông và trực quan để làm sáng tỏ các khái niệm: Trí tuệ nhân tạo (AI), Học máy (Machine Learning), Mạng thần kinh nhân tạo (Neural Networks), Học sâu (Deep Learning)... **Những khái niệm này thực chất có ý nghĩa gì và mối quan hệ biện chứng giữa chúng ra sao?**

Tôi nhận thấy những đúc kết này rất hữu ích đối với những ai muốn xây dựng một hệ thống kiến thức nền tảng vững chắc về AI. Các nội dung này nằm rải rác ở nhiều chương mục khác nhau, dưới đây tôi xin phép tổng hợp và hệ thống lại.

Để bảo đảm tính mạch lạc cho văn bản tiếng Việt, tôi không dịch thô từng từ mà chủ động biên soạn lại theo văn phong của mình, mọi sai sót về mặt học thuật nếu có xin quy thuộc trách nhiệm của người dịch.

**(1) Trí tuệ nhân tạo (Artificial Intelligence - AI)**

Mùa hè năm 1956, nhà khoa học máy tính John McCarthy lần đầu tiên đề xuất thuật ngữ "Trí tuệ nhân tạo" (AI) trước giới học thuật.

<u>Trí tuệ nhân tạo là thuật ngữ rộng nhất, chỉ việc ứng dụng các giải pháp phần cứng kết hợp phần mềm nhằm mục đích thực thi các tác vụ mà thông thường đòi hỏi phải có sự tham gia của trí tuệ con người mới có thể hoàn thành.</u> Đối tượng nghiên cứu cốt lõi của ngành là mô phỏng lại các năng lực tư duy của bộ não con người trên môi trường máy móc.

**(2) Học máy (Machine Learning - ML)**

Ở giai đoạn sơ khai, các nghiên cứu về trí tuệ nhân tạo được chia thành hai trường phái học thuật độc lập:

Trường phái thứ nhất ứng dụng phương pháp tiếp cận dựa trên luật lệ (Rule-based), thường được gọi là hệ thống chuyên gia (Expert systems). Triết lý của phương pháp này là con người sẽ chủ động viết ra một hệ thống các quy tắc logic chi tiết để hướng dẫn máy tính cách thức suy nghĩ và ra quyết định.

Tuy nhiên trên thực tế, đứng trước các bài toán thực tiễn phức tạp và có quy mô lớn, con người hầu như không thể biên soạn được một hệ thống luật lệ đầy đủ và chuẩn xác. Do đó, trường phái này nhanh chóng gặp phải các giới hạn kỹ thuật và không thể phát triển sâu hơn。

Trường phái thứ hai chính là **Học máy (Machine Learning)**. Triết lý của học máy là **tuyệt đối không thiết lập sẵn các quy tắc logic**, mà chỉ cung cấp một khối lượng lớn dữ liệu đầu vào cho máy tính, để máy tự học tập, tự tìm kiếm quy luật ẩn sâu trong dữ liệu và đưa ra kết quả dự báo.

**(3) Mạng thần kinh nhân tạo (Neural Network)**

Mạng thần kinh nhân tạo là một trong những dạng biểu diễn và triển khai quan trọng nhất của Học máy.

<u>Triết lý của mạng thần kinh nhân tạo là thiết lập một hệ thống tính toán mô phỏng lại cấu trúc vật lý của bộ não con người, liên kết các nút tính toán mô phỏng tế bào thần kinh sinh học (neurons) để xử lý thông tin.</u>

Mỗi nút tính toán độc lập đóng vai trò là một neuron, hàng triệu nút liên kết chặt chẽ với nhau tạo thành một mạng lưới tính toán song song quy mô lớn.

Mạng thần kinh nhân tạo yêu cầu năng lực tính toán cực lớn của phần cứng và nguồn dữ liệu huấn luyện khổng lồ. Ở những thập kỷ trước, đây là những rào cản vật lý không thể vượt qua, dẫn đến việc nghiên cứu mạng thần kinh nhân tạo bị rơi vào trạng thái đóng băng suốt từ những năm 70 của thế kỷ trước.

**(4) Học sâu (Deep Learning)**

Học sâu thực chất là một phương pháp triển khai cụ thể của Mạng thần kinh nhân tạo, được nhà khoa học Geoffrey Hinton đề xuất vào những năm 1980. Phát kiến này đã giúp hồi sinh mạnh mẽ các nghiên cứu về mạng thần kinh nhân tạo.

<u>Học sâu là phương pháp thiết lập hệ thống giúp các mạng thần kinh nhân tạo nhiều lớp (multi-layered) có thể tính toán hiệu quả, nâng hiệu năng xử lý lên một tầm cao mới. Từ "sâu" (deep) trong tên gọi phản ánh cấu trúc gồm rất nhiều lớp neuron hoạt động tự học song song.</u>

Cấu trúc mạng bao gồm một lớp nhận dữ liệu đầu vào (Input layer), một lớp xuất kết quả đầu ra (Output layer), và rất nhiều lớp xử lý trung gian ở giữa (được gọi là các lớp ẩn - Hidden layers). Trước đây, do giới hạn năng lực máy tính, các nhà khoa học chỉ có thể cấu hình được 1 đến 2 lớp ẩn. Sự ra đời của Học sâu kết hợp sức mạnh phần cứng hiện đại cho phép chúng ta xây dựng hệ thống mạng sở hữu hàng ngàn lớp ẩn trung gian, tạo nên một độ "sâu" vô cùng khủng khiếp.

**(5) Kiến trúc Transformer**

Trong những năm đầu phát triển của Học sâu, hai kiến trúc phổ biến nhất được ứng dụng rộng rãi là Mạng thần kinh tích chập (CNN - tối ưu cho xử lý hình ảnh) và Mạng thần kinh hồi quy (RNN - tối ưu cho xử lý ngôn ngữ).

Đến năm 2017, các nhà nghiên cứu của Google đã giới thiệu một kiến trúc mạng học sâu hoàn toàn mới mang tên Transformer (Bộ chuyển đổi).

<u>Điểm khác biệt mang tính cách mạng của Transformer so với các kiến trúc đi trước là khả năng xử lý đồng thời toàn bộ chuỗi văn bản đầu vào thay vì phải xử lý tuần tự từng từ một, đồng thời ứng dụng cơ chế tự chú ý (Self-Attention) để tự động gán các trọng số ý nghĩa khác nhau cho từng từ trong câu.</u>

Sự ra đời của Transformer chính là bệ phóng trực tiếp dẫn đến sự bùng nổ của siêu trợ lý ChatGPT vào năm 2022 và hàng loạt các mô hình AI tạo sinh (Generative AI) khổng lồ hiện nay, giữ vững vị thế là kiến trúc công nghệ thống trị tuyệt đối của ngành.

Due to các mô hình dựa trên Transformer bắt buộc phải nạp và xử lý toàn bộ dữ liệu đầu vào trong một chu kỳ tính toán, các mô hình này luôn đi kèm thông số kỹ thuật quan trọng là **Kích thước cửa sổ ngữ cảnh (Context Window Size)**, thể hiện khối lượng dữ liệu tối đa mà mô hình có thể tiếp nhận trong một lượt truy vấn.

Ví dụ, mô hình GPT-4 Turbo sở hữu cửa sổ ngữ cảnh lên tới 128.000 Tokens, tương đương với khả năng đọc hiểu đồng thời một tập tài liệu dài hơn 300 trang sách trong một lượt hỏi. Cửa sổ ngữ cảnh càng lớn giúp AI có khả năng liên kết thông tin càng sâu sắc, đưa ra câu trả lời có độ chính xác và tính mạch lạc cao hơn, đồng thời đòi hỏi phần cứng máy chủ phải có năng lực tính toán cực kỳ khủng khiếp.

## 豆包 MarsCode 动手实验室（杭州站）

Trước hết, xin phép được nhắc lại thông tin về giải đấu lập trình quốc gia **AI Lập Trình Điên Phong Khiêu Chiến Sài** đã được giới thiệu ở số tuần trước.

Cổng nhận sản phẩm dự thi của Nhánh Ứng dụng sáng tạo đã chính thức mở từ ngày 16 tháng 12, các bạn thí sinh đã có thể tải sản phẩm ứng dụng tự phát triển bằng AI của mình lên hệ thống.

Nhánh Thuật toán hiện vẫn đang tiếp tục nhận hồ sơ đăng ký. **Chỉ cần bạn có niềm đam mê và tự tin làm chủ các công cụ AI để giải quyết các bài toán thuật toán, hãy nhanh tay đăng ký tham gia** để trải nghiệm và cọ xát năng lực lập trình của bản thân.

[![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121908.webp)](https://cdn.beekka.com/blogimg/asset/202412/bg2024122001.webp)

Chi tiết về thể lệ thi đấu và cổng đăng ký tham gia sự kiện có thể truy cập trực tiếp tại [liên kết này](http://zjsms.com/iUNhdBEk/).

---

Sự kiện công nghệ tiếp theo được giới thiệu tuần này là chương trình offline **Doubao MarsCode Hands-on Lab** sẽ được tổ chức vào chiều thứ Bảy ngày 28 tháng 12 tới tại văn phòng ByteDance Hàng Châu.

Tham gia sự kiện, các bạn lập trình viên sẽ có cơ hội trải nghiệm sâu sắc năng lực hỗ trợ viết mã của trợ lý AI Doubao MarsCode, đồng thời giao lưu trực tiếp với đội ngũ kỹ sư phát triển sản phẩm của ByteDance. Trong phần thực hành, bạn sẽ được tự tay lập trình ứng dụng để hiện thực hóa ý tưởng của mình dưới sự hướng dẫn của AI. Những sản phẩm xuất sắc nhất tại sự kiện sẽ nhận được tấm vé đặc cách đi thẳng vào vòng chung kết của giải đấu AI Lập Trình Điên Phong Khiêu Chiến Sài.

Thông tin chi tiết về nội dung chương trình và cổng đăng ký tham dự sự kiện offline có thể tra cứu tại [liên kết sự kiện](https://www.bagevent.com/event/8960133?bag_track=ryf).

## 科技动态

1、[Thiết bị đột phá phá hủy vật lý ổ cứng máy tính](https://www.tomshardware.com/pc-components/storage/hard-drive-ssd-puncher-puts-four-holes-through-your-drives-puncher-p30-destroys-physical-media-with-12-tons-of-pressure)

Khi tiến hành thanh lý hoặc tiêu hủy các ổ cứng máy tính cũ, quy trình quan trọng nhất là phải bảo đảm dữ liệu lưu trữ đã được xóa sạch hoàn toàn. Giải pháp an toàn và triệt để nhất chính là phá hủy vật lý cấu trúc ổ cứng.

Tuy nhiên, việc này thủ công thường khá vất vả khi bạn phải dùng búa đập vỡ từng chiếc ổ cứng một.

Để đơn giản hóa quy trình này, một doanh nghiệp Nhật Bản đã giới thiệu dòng sản phẩm máy đột dập phá hủy ổ cứng chuyên dụng. Thiết bị có khả năng dập thủng 4 lỗ sâu xuyên qua ổ cứng chỉ trong tích tắc, bảo đảm phá hủy hoàn toàn mọi đĩa từ lưu trữ dữ liệu bên trong.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024070507.webp)

Thiết bị ứng dụng hệ thống bơm thủy lực chạy điện mạnh mẽ, tạo ra lực ép cực lớn lên tới 12 tấn, dễ dàng xuyên thủng bất kỳ loại vỏ ổ cứng kim loại dày nào.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024070508.webp)

Kích thước của máy là 410 x 289 x 187 mm, chỉ tương đương với một thùng máy tính để bàn thông thường, nhưng có trọng lượng lên tới 18kg. Thiết bị là giải pháp lý tưởng cho các doanh nghiệp và tập đoàn lớn có nhu cầu thanh lý định kỳ hàng ngàn ổ cứng lưu trữ thông tin nhạy cảm.

2、[Bộ cờ vua chế tác từ cát in 3D](https://parametric-architecture.com/3d-printed-dune-chess-set-by-rory-noble-turner/)

Một nhà thiết kế người Anh đã ứng dụng công nghệ in 3D để tạo nên một bộ cờ vua vô cùng độc đáo với vật liệu chế tác hoàn toàn từ cát mịn.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121811.webp)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121812.webp)

Nhà thiết kế chia sẻ ý tưởng của anh xuất phát từ mong muốn tìm kiếm một trải nghiệm cảm giác mới lạ. Cát vốn là một vật liệu dạng hạt rời rạc, vô hình và dễ dàng trôi chảy, việc định hình nó thành các quân cờ kiên cố vững chãi mang lại một cảm giác nghệ thuật về sự vô thường và biến đổi không ngừng của vạn vật.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121813.webp)

Hơn nữa, bề mặt của các quân cờ in từ cát giữ lại độ nhám tự nhiên đặc trưng, mang lại một trải nghiệm xúc giác vô cùng chân thực và khác biệt cho các kỳ thủ khi trực tiếp cầm nắm quân cờ thi đấu.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121814.webp)

3、[Gạch kính xây dựng chịu lực trong suốt](https://news.mit.edu/2024/engineers-3d-print-sturdy-glass-bricks-building-structures-0920)

Đã bao giờ bạn tự hỏi tại sao các ngôi nhà luôn cần đến những bức tường gạch kiên cố? Liệu chúng ta có thể xây dựng một ngôi nhà hoàn toàn không có tường mà chỉ bao quanh bằng những ô cửa kính lớn ngập tràn ánh sáng hay không?

Câu trả lời thực tế là không thể, bởi toàn bộ tải trọng của ngôi nhà đều được truyền trực tiếp xuống hệ thống tường chịu lực, trong khi các khung cửa kính thông thường không có khả năng chịu tải. Nếu thay thế toàn bộ tường bằng kính thường, ngôi nhà sẽ lập tức bị sụp đổ.

Vậy giải pháp thay thế là gì? Liệu có thể chế tạo ra một loại vật liệu thủy tinh vừa có khả năng truyền sáng tối ưu như cửa kính, vừa có năng lực chịu lực kiên cố giống như gạch xây dựng thông thường hay không?

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024101804.webp)

Các nhà khoa học tại Viện Công nghệ Massachusetts (MIT) mới đây đã nghiên cứu chế tạo thành công mẫu gạch kính xây dựng hoàn toàn trong suốt (hình trên). Các bài kiểm định vật lý cho thấy mẫu gạch kính này sở hữu năng lực chịu tải trọng tương đương với các loại gạch đất sét nung thông thường.

Bên cạnh khả năng truyền sáng tuyệt vời, gạch kính còn sở hữu một ưu điểm lớn liên quan đến khả năng tái chế bảo vệ môi trường. Chỉ cần được gia nhiệt ở nhiệt độ cao thích hợp, các viên gạch kính cũ sẽ nóng chảy hoàn toàn để tái chế đúc thành các viên gạch mới hoặc ứng dụng công nghệ in 3D tạo hình các kết cấu kiến trúc khác. Tuy nhiên, đặc tính nóng chảy này cũng vô tình khiến loại vật liệu này có khả năng chống hỏa hoạn kém hơn gạch nung.

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024101805.webp)

Nhìn chung, gạch kính trong suốt sở hữu các đặc tính thân thiện với môi trường tốt hơn nhiều so với gạch đỏ truyền thống và hứa hẹn sẽ được ứng dụng rộng rãi trong các công trình kiến trúc hiện đại tương lai.

4、**Các tin tức khác**

(1) Thị trường đầu tư mạo hiểm tuần này ghi nhận [thương vụ đầu tư lớn nhất lịch sử](https://finance.sina.cn/7x24/2024-12-18/detail-inczvnmc5201636.d.html) khi doanh nghiệp công nghệ AI Databricks đã hoàn tất vòng gọi vốn với số tiền đầu tư nhận được lên tới 10 tỷ USD chỉ trong một lần gọi vốn.

(2) GitHub chính thức thông báo trợ lý lập trình thông minh [GitHub Copilot](https://github.com/features/copilot) sẽ được mở quyền sử dụng hoàn toàn miễn phí cho mọi nhóm đối tượng người dùng phổ thông.

(3) OpenAI ra mắt dịch vụ gọi thoại miễn phí mang tên [1-800-ChatGPT](https://help.openai.com/en/articles/10193193-1-800-chatgpt-calling-and-messaging-chatgpt-with-your-phone). Người dùng tại khu vực Bắc Mỹ có thể quay số điện thoại này để thực hiện cuộc gọi thoại trò chuyện trực tiếp với AI, với hạn mức trải nghiệm miễn phí là 15 phút mỗi tháng.

(4) [Xiaomi chính thức công bố](https://github.com/XiaoMi/ha_xiaomi_home/blob/main/doc/README_zh.md) hỗ trợ tích hợp sâu toàn bộ hệ sinh thái thiết bị thông minh IoT của hãng vào nền tảng quản trị nhà thông minh mã nguồn mở Home Assistant.

## 文章

1、[Hướng dẫn cơ bản về ngôn ngữ lập trình hợp ngữ (Assembly)](https://shikaan.github.io/assembly/x86/guide/2024/09/08/x86-64-introduction-hello.html) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024091802.webp)

Bài chia sẻ ngắn gọn giải thích một cách vô cùng dễ hiểu về các khái niệm cơ bản của ngôn ngữ lập trình cấp thấp hợp ngữ (Assembly x86-64).

2、[Hướng dẫn chi tiết về thuộc tính grid-area trong CSS Grid](https://ishadeed.com/article/css-grid-area/#header-layout) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024081701.webp)

Bài viết phân tích chuyên sâu hướng dẫn các nhà phát triển cách thức khai thác tính năng phân vùng layout (template area) của CSS Grid để thiết kế giao diện trang web linh hoạt.

3、[Phương pháp tích hợp dữ liệu ngữ nghĩa định dạng JSON-LD vào trang web](https://csvbase.com/blog/13) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082206.webp)

Bài viết hướng dẫn chi tiết cách nhúng các khối dữ liệu cấu trúc định dạng JSON-LD vào mã nguồn HTML nhằm cung cấp dữ liệu ngữ nghĩa tối ưu cho các công cụ cào dữ liệu và tìm kiếm tự động đọc hiểu cấu trúc trang web.

4、[13 tiện ích mở rộng Chrome hữu dụng dành cho nhà phát triển Frontend](https://jsdevspace.substack.com/p/13-super-useful-chrome-plugins-for) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024092304.webp)

Bài viết tổng hợp và giới thiệu chi tiết về 13 extension trên trình duyệt Chrome giúp hỗ trợ đắc lực cho quy trình thiết kế và kiểm thử giao diện Frontend.

5、[Lập luận: Google đang mất dần vị thế công cụ tìm kiếm tốt nhất](https://www.theregister.com/2024/12/16/opinion_column_perplexity_vs_google/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121902.webp)

Bài phân tích chuyên sâu nhận định năng lực tìm kiếm và tổng hợp thông tin ứng dụng trí tuệ nhân tạo của Perplexity AI hiện đã cho trải nghiệm vượt trội hơn hẳn so với kết quả tìm kiếm truyền thống của Google.

6、[Thủ thuật mang các tính năng tốt nhất của macOS lên Windows](https://www.xda-developers.com/how-i-got-the-best-macos-features-on-windows/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121903.webp)

Bài hướng dẫn chia sẻ một số thủ thuật cài đặt phần mềm bổ trợ giúp người dùng hệ điều hành Windows có thể trải nghiệm các tính năng tiện lợi vốn là thế mạnh của macOS (ví dụ tính năng xem nhanh nội dung tệp bằng phím Space ngay trong File Explorer).

## 工具

1、[Presenterm](https://github.com/mfontanini/presenterm)

Công cụ dòng lệnh mã nguồn mở hỗ trợ lập trình viên nhanh chóng chuyển đổi tệp Markdown thành các trang slide thuyết trình và thực hiện trình chiếu trực tiếp ngay trên giao diện terminal. (Đóng góp từ [@lengyijun](https://github.com/ruanyf/weekly/issues/5706))

2、[Rslib](https://github.com/web-infra-dev/rslib)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121402.webp)

Công cụ đóng gói và xuất bản các thư viện JavaScript chuyên nghiệp, hỗ trợ lập trình viên xây dựng nhanh các bộ thư viện UI components hoặc các tiện ích dòng lệnh (CLI tools). (Đóng góp từ [@fi3ework](https://github.com/ruanyf/weekly/issues/5713))

3、[Midscene.js](https://github.com/web-infra-dev/midscene)

Bộ khung thử nghiệm tự động hóa giao diện trang web bằng AI, cho phép lập trình viên chỉ cần mô tả kịch bản test bằng ngôn ngữ tự nhiên, hệ thống sẽ tự động phân tích và thực thi các bước kiểm thử giao diện trực quan. (Đóng góp từ [@yuyutaotao](https://github.com/ruanyf/weekly/issues/5733))

4、[wechatDataBackup](https://github.com/git-jiadong/wechatDataBackup)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121501.webp)

Tiện ích máy tính hỗ trợ người dùng nhanh chóng kết xuất và sao lưu toàn bộ dữ liệu lịch sử cuộc trò chuyện từ ứng dụng WeChat phiên bản Windows PC chỉ bằng một cú nhấp chuột. (Đóng góp từ [@git-jiadong](https://github.com/ruanyf/weekly/issues/5721))

5、[MoeMail](https://github.com/beilunyang/moemail)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121803.webp)

Dịch vụ tạo hộp thư điện tử tạm thời (Temporary Email) mã nguồn mở được phát triển trên kiến trúc Next.js kết hợp Cloudflare Workers. Trải nghiệm trực tiếp tại [moemail.app](https://moemail.app). (Đóng góp từ [@beilunyang](https://github.com/ruanyf/weekly/issues/5740))

6、[my-github-2024](https://github.com/WCY-dt/my-github-2024)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121502.webp)

Tập lệnh Python hỗ trợ tự động thu thập thông tin và xuất bản các biểu đồ trực quan thống kê toàn bộ hoạt động commit đóng góp mã nguồn của bạn trên GitHub trong năm 2024. (Đóng góp từ [@WCY-dt](https://github.com/ruanyf/weekly/issues/5722))

7、[Vanilla CSS Framework](https://vanillaframework.io/)

Bộ khung định dạng CSS (CSS Framework) chính thức do hãng Canonical thiết kế và ứng dụng cho toàn bộ giao diện trang chủ của hệ điều hành Ubuntu.

8、[OpenAuth](https://github.com/openauthjs/openauth)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121806.webp)

Thư viện tích hợp hỗ trợ các nhà phát triển nhanh chóng thiết lập tính năng đăng nhập trang web thông qua xác thực của các bên thứ ba (OAuth Providers).

9、[Schemio](https://github.com/ishubin/schemio)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121807.webp)

Trình chỉnh sửa và thiết kế trực quan hóa các sơ đồ kỹ thuật hoạt động trực tiếp trên nền tảng trình duyệt Web.

10、[Buzee](https://github.com/gsidhu/buzee-tauri)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121907.webp)

Phần mềm máy tính hỗ trợ người dùng thực hiện tìm kiếm toàn văn (full-text search) nhanh các tệp tin lưu trữ cục bộ, tích hợp tính năng OCR tự động trích xuất và tìm kiếm cả các ký tự xuất hiện trong hình ảnh (hỗ trợ Windows và macOS).

## AI 相关

1、[Hika AI](https://hika.fyi/)

Dịch vụ tìm kiếm thông tin ứng dụng trí tuệ nhân tạo (AI Search Engine) hoàn toàn miễn phí. (Đóng góp từ [@atlas-comstock](https://github.com/ruanyf/weekly/issues/5714))

2、[Slea.ai](https://slea.ai/zh-CN)

Công cụ hỗ trợ tự động thiết kế và tạo logo doanh nghiệp bằng AI miễn phí. (Đóng góp từ [@aaamomo64](https://github.com/ruanyf/weekly/issues/5727))

3、[AI Sound Effect Generator](https://tiktokvoice.net/en/sounds-effect)

Trang web hỗ trợ người dùng tự tạo nhanh các hiệu ứng âm thanh môi trường tự nhiên (như tiếng mưa rơi, tiếng gió rít) bằng AI hoàn toàn miễn phí. (Đóng góp từ [@aurthur](https://github.com/ruanyf/weekly/issues/5729))

## 资源

1、[SQL Style Guide (Cẩm nang chuẩn hóa cách viết câu lệnh SQL)](https://www.sqlstyle.guide)

Tài liệu điện tử tổng hợp toàn bộ các quy chuẩn định dạng và chuẩn hóa phong cách viết câu lệnh SQL giúp mã nguồn trở nên sạch sẽ và dễ đọc hơn.

2、[Màu sắc mã số bảng tra cứu](https://www.ysdaima.com)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121404.webp)

Trang web tổng hợp bộ sưu tập các công cụ hỗ trợ phối màu trực tuyến phục vụ thiết kế giao diện Web. (Đóng góp từ [@nettsz](https://github.com/ruanyf/weekly/issues/5717))

## 图片

1、[Mẫu robot chuồn chuồn gián điệp của CIA](https://www.popularmechanics.com/flight/drones/a30795266/cia-robot-dragonfly/)

Tại khu trưng bày bảo tàng của Cơ quan Tình báo Trung ương Mỹ (CIA) ở Washington có trưng bày một nguyên mẫu robot chuồn chuồn ngụy trang được chế tạo từ những năm 70 của thế kỷ trước.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121808.webp)

Thiết bị thực chất là một chiếc máy bay trực thăng siêu nhỏ ngụy trang, được thiết kế để bay tiếp cận các mục tiêu tình báo nhằm thực hiện nhiệm vụ nghe lén các cuộc trò chuyện.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121809.webp)

Chú chuồn chuồn cơ học này có khả năng bay tự hành trong phạm vi khoảng 200 mét rồi hạ cánh xuống mục tiêu, sau đó sử dụng chùm tia laser ghi nhận các rung động của không khí để giải mã và khôi phục lại âm thanh cuộc trò chuyện.

Tuy nhiên, do thiết kế quá nhỏ nhẹ khiến thiết bị có khả năng chống gió kém và rất khó điều khiển hướng bay chính xác nên dự án chưa từng được đưa vào khai thác thực tế.

2、[Mã bưu chính ghi tay độc đáo của Hà Lan](https://en.wikipedia.org/wiki/Postzegelcode)

Hệ thống bưu chính Hà Lan hỗ trợ dịch vụ gửi thư không cần mua tem giấy truyền thống, thay vào đó người gửi sẽ ghi một dãy mã số bưu chính gồm 9 chữ cái và chữ số lên phong bì.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071110.webp)

Người dùng thực hiện thanh toán trực tuyến để mua một đoạn mã số bưu chính này, sau đó viết đoạn mã lên phong bì thư theo cấu trúc ma trận 3 x 3 thay thế cho con tem giấy làm bằng chứng đã thanh toán phí bưu chính.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071111.webp)

Do đoạn mã bưu chính này chỉ có thời hạn hiệu lực sử dụng trong vòng 5 ngày kể từ khi mua (căn cứ theo dấu bưu điện) nên rủi ro bị kẻ gian đoán mò mã số để sử dụng lậu là cực kỳ thấp.

## 文摘

1、[Triết lý: Không tồn tại khái niệm năng suất viết phần mềm](https://www.benrady.com/2012/11/theres-no-such-thing-as-software-productivity.html)

Giống như nhà thiết kế phần mềm nổi tiếng Martin Fowler từng nhận định: Năng suất viết mã nguồn (productivity) của một lập trình viên thực tế là điều hoàn toàn không thể đo lường một cách chuẩn xác, bởi vì khái niệm này căn bản là không hề tồn tại.

Hoạt động phát triển phần mềm không giống như dây chuyền sản xuất công nghiệp để có thể đo lường sản phẩm đầu ra theo số lượng.

Hãy tưởng tượng bạn có hai kỹ sư phần mềm cùng tham gia phát triển một dự án, và ngẫu nhiên trong cùng một ngày, cả hai được giao thực hiện một nhiệm vụ vá lỗi hệ thống giống hệt nhau.

Kỹ sư Giáp đã thức đêm viết một bộ khung mã nguồn dài tới 1.000 dòng để giải quyết triệt để bài toán. Đoạn code được cấu trúc vô cùng sạch sẽ, viết đầy đủ các test case kiểm thử và biên soạn tài liệu giải thích chi tiết từng bước.

Trong khi đó, kỹ sư Ất dành phần lớn thời gian ban ngày để ra công viên đi dạo ngắm cảnh và suy ngẫm hướng giải quyết bài toán. Cuối ngày, anh trở lại văn phòng, thực hiện xóa bỏ 100 dòng mã nguồn cũ có sẵn của hệ thống, cập nhật cấu hình và triển khai thay đổi... Sự cố lập tức được khắc phục triệt để.

Theo bạn, ai trong hai người sở hữu năng suất làm việc cao hơn?

Thực tế câu trả lời ai năng suất hơn không phải là điều quan trọng nhất. Giá trị cốt lõi là kỹ sư Ất đã giải quyết xong bài toán mà không phát sinh thêm dòng code mới nào, đồng thời giúp giảm thiểu chi phí bảo trì hệ thống dài hạn của cả đội ngũ kỹ sư. Kỹ sư Giáp cũng xử lý xong sự cố, nhưng giải pháp của anh đã chèn thêm 1.000 dòng code mới vào hệ thống, vô tình làm tăng chi phí đọc hiểu và bảo trì mã nguồn về sau, do đó (trong các điều kiện khác tương đương) giải pháp của Giáp được đánh giá là kém tối ưu hơn so với Ất.

Vậy chúng ta có thể khẳng định kỹ sư Ất có năng suất làm việc cao hơn không? Rõ ràng là rất khó để tìm ra một thước đo toán học chuẩn xác phản ánh năng suất lập trình.

Tôi cho rằng **giá trị cốt lõi của một kỹ sư phần mềm xuất sắc là năng lực giải quyết vấn đề**. Và các thước đo sản phẩm đầu ra như số dòng code, số trang tài liệu hướng dẫn hay cơ sở dữ liệu thực chất chỉ là những công cụ hỗ trợ giải quyết vấn đề chứ hoàn toàn không phải là mục tiêu cuối cùng của công việc.

## 言论

1、

Trong suốt quá trình tự tay viết mã nguồn phát triển hệ quản trị cơ sở dữ liệu SQLite, chưa từng có ai dạy tôi về cấu trúc dữ liệu cây B-tree. Khi đứng trước yêu cầu phải triển khai cấu trúc B-tree cho hệ thống, tôi đã tìm đọc chương sách viết về B-tree trong bộ sách kinh điển *The Art of Computer Programming* của giáo sư Donald Knuth. Tôi đọc hiểu các thuật toán mô tả trong sách và tiến hành lập trình theo.

Điều thú vị là trong cuốn sách, giáo sư Knuth hướng dẫn vô cùng chi tiết các thuật toán tìm kiếm và chèn dữ liệu vào cây B-tree, nhưng riêng thuật toán xóa dữ liệu khỏi cây ông lại không viết chi tiết mà chuyển nó thành bài tập thực hành ở cuối chương. Do đó, trước khi có thể tự viết code hoàn thiện cấu trúc B-tree cho SQLite, tôi đã bắt buộc phải tự mình hoàn thành bài tập xóa phần tử đó trước. Xin gửi lời cảm ơn chân thành đến giáo sư Donald Knuth vì bài tập đầy thử thách đó.

-- [Richard Hipp](https://corecursive.com/066-sqlite-with-richard-hipp/), *Cha đẻ của SQLite chia sẻ trong phóng sự "Những câu chuyện chưa kể về SQLite"*

2、

Tại thành phố Malmö ở miền nam Thụy Điển, chi phí tiền điện cho một lượt tắm nước nóng 10 phút của người dân hiện nay đã đội giá lên tới 2,65 Euro (tương đương khoảng 70.000 VNĐ). Nguyên nhân là bởi hệ thống điện của thành phố này được kết nối trực tiếp với lưới điện quốc gia Đức, và tình trạng thiếu hụt năng lượng nghiêm trọng tại Đức đã đẩy giá điện sinh hoạt của khu vực tăng cao.

-- [《Phóng sự: Khủng hoảng năng lượng tại Thụy Điển》](https://www.euractiv.com/section/energy/news/swedish-minister-open-to-new-measures-to-tackle-energy-crisis-blames-german-nuclear-phase-out/)

3、

Bài học quan trọng nhất trong chặng đường phát triển sự nghiệp của mỗi người là bạn cần sớm nhận ra rằng: Mục tiêu cốt lõi trong công việc hằng ngày của bạn không phải là làm hài lòng toàn bộ khách hàng của công ty, mà là phải làm hài lòng chính những người đang trực tiếp quyết định mức lương, tiền thưởng và cơ hội thăng tiến của bạn tại doanh nghiệp.

-- [Ý kiến độc giả trên diễn đàn Hacker News](https://news.ycombinator.com/item?id=42092156)

4、

Các công nghệ tàu lặn không người lái (UUV) đang được nghiên cứu và phát triển mạnh mẽ hiện nay sẽ sớm khiến học thuyết quân sự lấy tàu sân bay làm trung tâm trở nên lỗi thời, giúp các quốc gia cắt giảm đáng kể các khoản ngân sách chi tiêu quân sự khổng lồ.

Ví dụ tiêu biểu là mẫu tàu lặn không người lái khổng lồ Orca XLUUV do Mỹ phát triển, có khả năng mang theo 8 tấn thiết bị, tự hành di chuyển hành trình dài hàng ngàn dặm mà không yêu cầu phải nổi lên mặt nước trong suốt thời gian dài.

-- [Ý kiến độc giả trên diễn đàn Hacker News](https://news.ycombinator.com/item?id=42432129)

5、

Khi lần đầu tiên trải nghiệm các công cụ AI tạo sinh như Midjourney (tạo ảnh) hay Suno (tạo nhạc), tôi từng tự hỏi liệu trong tương lai có phải tất cả mọi người đều sẽ dễ dàng trở thành nghệ sĩ số hay không.

Tuy nhiên, tôi sớm nhận ra bản thân mình hoàn toàn không sở hữu "khát vọng sáng tạo nghệ thuật" (creative drive). Ngay cả khi được chiêm ngưỡng rất nhiều tác phẩm nghệ thuật đẹp mắt của người khác, tôi cũng thường không hình thành nên ý tưởng cụ thể về một tác phẩm mà mình muốn tạo ra.

Do đó, dù các công cụ AI tương lai có sở hữu năng lực vẽ tranh hay phối nhạc mạnh mẽ đến đâu, số lượng họa sĩ và nhạc sĩ thực thụ trong xã hội vẫn sẽ chỉ chiếm một tỷ lệ rất nhỏ. Câu chuyện đối với ngành lập trình cũng hoàn toàn tương tự: Dù AI có khả năng viết code tự động tốt đến đâu, việc tất cả mọi người đều có thể trở thành lập trình viên chuyên nghiệp là điều không bao giờ xảy ra.

-- [《Đánh giá chi tiết sau một thời gian trải nghiệm sâu công cụ Cursor》](https://www.pixelstech.net/article/1734488862-do-not-be-misled-by-‘build-an-app-in-5-minutes’%3a-in-depth-practice-with-cursor)

## 往年回顾

[Bàn về triết lý hành động: Tiến lên phía trước ngay cả khi chưa định hình điểm đến](http://www.ruanyifeng.com/blog/2023/12/weekly-issue-283.html) (2023 #283)

[Chiêm nghiệm: Cuộc sống của con người hiện đại có nét tương đồng với một bể cá cảnh](http://www.ruanyifeng.com/blog/2022/12/weekly-issue-233.html) (2022 #233)

[Tìm hiểu về các chính sách phúc lợi hưu trí dành cho nhân sự của tập đoàn Tencent](http://www.ruanyifeng.com/blog/2021/11/weekly-issue-183.html) (2021 #183)

[Bàn về cơ hội phát triển kinh tế và tiềm năng du lịch của tỉnh Quý Châu](http://www.ruanyifeng.com/blog/2020/11/weekly-issue-133.html) (2020 #133)

(Hết)
