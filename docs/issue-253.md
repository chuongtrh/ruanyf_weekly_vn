# Bản tin chia sẻ công nghệ (Số 253): Ngày cạn kiệt tài liệu huấn luyện AI

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3091) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050201.webp)

Đây không phải là một bảo tàng nghệ thuật kiến trúc, mà là những mái nhà kính chuyên trồng thanh mai xếp lớp dọc theo triền đồi dốc tại thôn Tam Khẩu, Lâm An, Hàng Châu. (Nguồn: [Weibo](https://weibo.com/6385067105/MEmohsdZe))

## 本周话题：训练材料用完之日

Trong các bản tin thời sự công nghệ hiện nay, tin tức về Trí tuệ nhân tạo (AI) xuất hiện với tần suất dày đặc mỗi ngày, đi kèm việc giới thiệu hàng loạt mô hình ngôn ngữ lớn khác nhau.

Để đánh giá và phân biệt năng lực mạnh yếu giữa các mô hình AI này, một trong những chỉ số kỹ thuật then chốt nhất chính là số lượng tham số (parameters) của chúng. Theo nguyên lý chung, mô hình nào sở hữu số lượng tham số lớn hơn thì năng lực xử lý và tư duy sẽ mạnh mẽ hơn.

Mô hình GPT-2 thời kỳ đầu sở hữu 1,5 tỷ tham số, trong khi thế hệ GPT-3 và ChatGPT đã được nâng cấp lên quy mô [175 tỷ tham số](https://developer.nvidia.com/zh-cn/blog/openai-presents-gpt-3-a-175-billion-parameters-language-model/). Đối với phiên bản GPT-4 thế hệ mới nhất, OpenAI lựa chọn giữ bí mật chỉ số này, nhưng giới phân tích đồn đoán quy mô của nó lớn gấp ít nhất 5 lần so với thế hệ tiền nhiệm.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050303.webp)

Vậy tham số thực chất là gì?

Theo một cách hiểu đơn giản nhất, tham số đại diện cho số lượng các nút liên kết mạng thần kinh nhân tạo được mô hình sử dụng làm căn cứ để đưa ra các dự đoán. **Số lượng tham số càng lớn đồng nghĩa với việc mô hình có thể cân nhắc và xử lý được nhiều khả năng và tình huống phức tạp hơn, từ đó mang lại kết quả đầu ra chính xác và tự nhiên hơn, dù đi kèm chi phí tính toán cực kỳ lớn.**

Một khi số lượng tham số càng lớn càng tốt, câu hỏi đặt ra là: liệu quy mô tham số của các mô hình AI có thể tăng trưởng vô hạn hay không?

Câu trả lời chắc chắn là không, bởi quy mô tham số bị giới hạn trực tiếp bởi khối lượng dữ liệu tài liệu dùng để huấn luyện mô hình. Chúng ta bắt buộc phải có đủ lượng dữ liệu huấn luyện đầu vào tương ứng mới có thể tính toán và thiết lập được các tham số này. **Nếu số lượng tham số tăng lên vô hạn, khối lượng dữ liệu huấn luyện bắt buộc cũng phải tăng lên tương ứng.**

Một nguyên lý phổ biến trong ngành học máy chỉ ra rằng: khối lượng dữ liệu huấn luyện cần thiết tối thiểu phải lớn gấp 10 lần quy mô tham số của mô hình.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050305.webp)

Lấy ví dụ với ChatGPT sở hữu 175 tỷ tham số, khối lượng dữ liệu huấn luyện tối ưu cần thiết sẽ không được thấp hơn 1.750 tỷ token (từ vựng và ký hiệu ngôn ngữ). Để dễ hình dung, cuốn tiểu thuyết kinh điển *Hồng Lâu Mộng* có độ dài khoảng 780.000 chữ (tương đương khoảng 1 triệu token). Như vậy, lượng dữ liệu huấn luyện nạp vào ChatGPT tương đương với nội dung của khoảng 1,75 triệu cuốn tiểu thuyết *Hồng Lâu Mộng* gộp lại.

Theo các [báo cáo kỹ thuật](https://www.sciencefocus.com/future-technology/gpt-3/), OpenAI đã sử dụng khoảng 570 GB dữ liệu văn bản thô để huấn luyện ChatGPT, được thu thập từ toàn bộ kho lưu trữ Wikipedia tiếng Anh, các thư viện sách trực tuyến, diễn đàn Reddit, mạng xã hội Twitter cùng hàng tỷ trang web khác trên internet.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050306.webp)

Các thế hệ AI mạnh mẽ hơn trong tương lai chắc chắn sẽ đòi hỏi lượng dữ liệu huấn luyện khổng lồ hơn nữa. **Nhưng vấn đề cốt lõi là: liệu chúng ta có thể tìm kiếm đâu ra nguồn dữ liệu khổng lồ như vậy trên Trái Đất, và liệu có ngày kho dữ liệu này sẽ cạn kiệt?**

Thực tế, đã có những nghiên cứu khoa học chuyên sâu được công bố trong các [bài báo cáo khoa học](https://epochai.org/blog/will-we-run-out-of-ml-data-evidence-from-projecting-dataset) để đi tìm lời giải cho câu hỏi này.

Dữ liệu thống kê trong vòng 10 năm qua cho thấy: tốc độ tăng trưởng quy mô của các tập dữ liệu huấn luyện AI đang nhanh hơn rất nhiều so với tốc độ tích lũy dữ liệu số thực tế của toàn nhân loại. Nếu xu hướng này tiếp tục tiếp diễn, việc cạn kiệt kho dữ liệu số của thế giới là điều không thể tránh khỏi.

Nghiên cứu đã đưa ra dự báo về 3 mốc thời gian cạn kiệt nguồn dữ liệu:

* **Năm 2026**: Cạn kiệt toàn bộ nguồn dữ liệu ngôn ngữ chất lượng cao (high-quality language data) thông thường trên internet.
* **Giai đoạn 2030 - 2050**: Cạn kiệt hoàn toàn toàn bộ các nguồn dữ liệu văn bản và ngôn ngữ của nhân loại.
* **Giai đoạn 2030 - 2060**: Cạn kiệt toàn bộ các nguồn dữ liệu hình ảnh và video (visual data).

Điều này có nghĩa là theo dự báo, **chỉ trong vòng 3 đến 4 năm tới, các công ty công nghệ sẽ gặp rất nhiều khó khăn trong việc tìm kiếm thêm nguồn dữ liệu ngôn ngữ mới chất lượng cao để huấn luyện AI**. Và muộn nhất là trong vòng 30 năm nữa, toàn bộ kho tàng tri thức dạng chữ viết và hình ảnh tích lũy của nhân loại sẽ không còn đủ để đáp ứng nhu cầu huấn luyện của các mô hình AI thế hệ mới.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050307.webp)

Biểu đồ xu hướng phía trên mô tả thực trạng này: đường nét đứt biểu thị tốc độ tăng trưởng của dữ liệu tích lũy toàn cầu, các đường màu đỏ và xanh biểu thị dự báo tốc độ tăng trưởng nhu cầu dữ liệu của các mô hình AI. Từ sau năm 2035, các đường này sẽ giao nhau và đường cong tăng trưởng bắt đầu đi ngang.

Nhóm nghiên cứu nhận định từ thời điểm đó trở đi, do thiếu hụt nghiêm trọng nguồn dữ liệu huấn luyện mới, tốc độ phát triển năng lực của các mô hình AI sẽ bị chững lại rõ rệt.

Nếu dự báo này là chính xác, nó cho thấy một thực tế hoàn toàn trái ngược với suy nghĩ của số đông: **Kỷ nguyên bùng nổ vũ bão của AI sẽ không kéo dài mãi mãi. Giai đoạn hiện tại rất có thể chính là thời kỳ AI phát triển với tốc độ nhanh nhất**, trước khi bắt đầu chững lại và dần rơi vào trạng thái bão hòa tiệm cận停滞 vào giữa thế kỷ này, tương tự như thực trạng nghiên cứu của vật lý lượng tử hiện nay.

## 科技动态

1、[Hyundai giới thiệu công nghệ bánh xe xoay độc lập hỗ trợ di chuyển ngang](https://topcarnews.net/hyundais-new-steering-system-may-make-parking-jobs-way-easier-s237901.html)

Tập đoàn ô tô Hyundai của Hàn Quốc mới đây đã công bố thử nghiệm công nghệ hệ thống lái mới cho phép cả 4 bánh xe của ô tô có thể xoay độc lập một góc lên tới 90 độ:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042801.webp)

Trong đoạn video trình diễn, mẫu xe điện thử nghiệm có thể dễ dàng di chuyển ngang như loài cua để ghép xe vào chuồng hẹp, hoặc tự xoay tròn 360 độ ngay tại chỗ để quay đầu xe trong không gian chật hẹp.

Mặc dù có tính ứng dụng thực tế rất cao hỗ trợ người lái trong đô thị, công nghệ này làm tăng đáng kể độ phức tạp trong kết cấu hệ thống treo và đẩy chi phí sản xuất xe lên rất cao. Hyundai hiện chưa công bố kế hoạch đưa hệ thống lái này vào sản xuất thương mại hàng loạt.

2、[Nhiễu tĩnh điện từ ghế ngồi máy tính làm tắt màn hình hiển thị](https://mastodon.social/@haeckerfelix/110272427676278609)

Một người dùng mạng xã hội nước ngoài đã chia sẻ một sự cố kỳ lạ: màn hình máy tính của anh thường xuyên đột ngột bị tối đen trong vài giây rồi tự động hiển thị lại bình thường mà không rõ nguyên nhân.

Ban đầu anh cho rằng lỗi nằm ở bản thân chiếc màn hình hoặc cáp kết nối, nhưng sau nhiều ngày theo dõi, anh phát hiện hiện tượng này chỉ xảy ra mỗi khi anh dịch chuyển chiếc ghế xoay làm việc, hoặc khi anh ngồi xuống và đứng lên khỏi ghế:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042901.webp)

Chiếc ghế anh sử dụng là mẫu ghế văn phòng MARKUS nổi tiếng của IKEA. Dưới bài đăng, nhiều lập trình viên khác cũng xác nhận họ gặp phải sự cố tương tự với đúng mẫu ghế này:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042902.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042903.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042904.webp)

Nguyên nhân được xác định là do sự ma sát giữa sợi vải bọc ghế với quần áo hoặc trục piston kim loại bên dưới dễ tích tụ một lượng tĩnh điện lớn. Khi người dùng di chuyển hoặc đứng lên, luồng tĩnh điện này phóng ra không khí xung quanh, gây nhiễu điện từ (EMI) tác động trực tiếp lên mạch điều khiển của các màn hình máy tính đặt gần đó làm chúng tạm thời bị ngắt tín hiệu. Cách xử lý đơn giản nhất là đổi sang mẫu ghế khác, hoặc tự chế một sợi dây cáp tiếp địa nối từ khung kim loại của ghế xuống mặt sàn để triệt tiêu dòng tĩnh điện.

3、[Nghiên cứu ứng dụng tai nghe không dây hỗ trợ người suy giảm thính lực](https://www.cnbeta.com.tw/articles/tech/1337127.htm)

Một nghiên cứu y khoa mới đây công bố khả năng tận dụng các thiết bị tai nghe không dây thông thường để hỗ trợ cải thiện khả năng nghe cho những người bị suy giảm thính lực nhẹ:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010505.webp)

Dòng tai nghe AirPods của Apple được trang bị tính năng "Nghe trực tiếp" (Live Listen) có khả năng thu âm thanh từ môi trường xung quanh qua micrô của điện thoại iPhone và phóng đại âm thanh truyền trực tiếp vào tai người đeo. Kết quả thực nghiệm cho thấy hiệu quả khuếch tán âm thanh của tính năng này hoạt động tốt không kém các thiết bị trợ thính chuyên dụng.

Các dòng máy trợ thính chuyên dụng trên thị trường hiện có giá bán rất đắt đỏ, dao động từ vài triệu cho tới hàng chục triệu đồng. Việc tận dụng tai nghe không dây phổ thông làm máy trợ thính hứa hẹn sẽ giúp tiết kiệm chi phí rất lớn cho người bệnh.

4、[Hàn Quốc xây dựng đập tích nước bằng cát đá chống hạn hán vùng cao](https://techxplore.com/news/2023-04-advanced-sand-drought.html)

Để giải quyết tình trạng thiếu hụt nước sinh hoạt trầm trọng cho người dân vùng núi cao vào mùa khô hạn, chính quyền Hàn Quốc đã hoàn thành đập chứa nước bằng cát đá đầu tiên của quốc gia:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023043001.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023043002.webp)

Khác với các đập bê tông hở thông thường, cấu trúc đập chứa này bao gồm một bể chứa khổng lồ chứa đầy cát và sỏi nằm sâu dưới lòng đất để giữ nước mưa chảy tràn:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023043003.webp)

Thiết kế này mang lại ba ưu điểm vượt trội: ngăn chặn gần như hoàn toàn tình trạng thất thoát nước do bay hơi dưới ánh nắng; nguồn nước được lọc sạch tự nhiên khi len lỏi qua các tầng cát sỏi; và lớp cát bảo vệ bên trên giúp nguồn nước không bị đóng băng vào mùa đông lạnh giá.

5、[Mẫu nhẫn cưới thông minh hiển thị nhịp tim của bạn đời](https://language.chinadaily.com.cn/2016-08/22/content_26508362.htm)

Một doanh nghiệp công nghệ tại Cộng hòa Séc đã ra mắt dòng sản phẩm "nhẫn cưới thông minh" được tích hợp cảm biến đo nhịp tim và dải đèn LED hiển thị chạy quanh thân nhẫn:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042405.webp)

Điểm độc đáo của sản phẩm này là chiếc nhẫn sẽ không hiển thị nhịp tim của chính người đeo, mà hiển thị nhịp tim thời gian thực của người bạn đời đang đeo chiếc nhẫn còn lại:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042406.webp)

Thiết bị kết nối với điện thoại thông minh qua Bluetooth. Mỗi khi người đeo chạm nhẹ vào mặt nhẫn, chiếc nhẫn sẽ gửi tín hiệu kích hoạt đo nhịp tim của đối phương và truyền dải nhịp tim hiển thị rực sáng trên chiếc nhẫn của bạn:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042407.webp)

Nhà sản xuất chia sẻ sản phẩm này giúp các cặp đôi luôn cảm nhận được sự hiện diện và nhịp đập tình yêu của đối phương mọi lúc mọi nơi. Mẫu nhẫn được chế tác bằng chất liệu vàng hồng cao cấp với giá bán khoảng 3.000 USD cho một cặp.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042408.webp)

## 文章

1\. [Lập trình viên chia sẻ câu chuyện tự phát triển công cụ chỉnh sửa ảnh nguồn mở](https://www.v2ex.com/t/934564)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050401.webp)

Tác giả chia sẻ chi tiết hành trình cá nhân từ khâu lên ý tưởng thiết kế, lựa chọn thư viện công nghệ cho đến quy trình tối ưu hóa trải nghiệm người dùng khi tự tay lập trình xây dựng một ứng dụng web chỉnh sửa hình ảnh mã nguồn mở hoàn toàn miễn phí. (Đóng góp của [@nihaojob](https://github.com/ruanyf/weekly/issues/3081))

2\. [Hướng dẫn tự lập trình ứng dụng chỉnh sửa code trực quan tương tự CodePen](https://decode.sh/building-a-code-pen-type-editor-from-scratch)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041602.webp)

CodePen là một ứng dụng web vô cùng quen thuộc cho phép lập trình viên viết mã HTML/CSS/JS và xem kết quả hiển thị trực tiếp. Bài viết hướng dẫn chi tiết cách tự xây dựng các tính năng cốt lõi của một ứng dụng biên dịch code trực tiếp tương tự bằng JavaScript thuần rất đơn giản.

3\. [Cẩm nang hướng dẫn nhanh cách sử dụng công cụ giám sát mạng tcpdump](https://jvns.ca/blog/2016/03/16/tcpdump-is-amazing/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020818.webp)

Bài hướng dẫn thực hành trực quan giúp quản trị viên hệ thống nhanh chóng làm quen với cách sử dụng lệnh `tcpdump` trong Linux để theo dõi, lọc và phân tích các gói tin truyền tải qua giao thức TCP của một trang web cụ thể.

4\. [Phân tích vai trò và tầm quan trọng của tiêu chuẩn đồ họa WebGPU mới](https://cohost.org/mcc/post/1406157-i-want-to-talk-about-webgpu)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050301.webp)

Hiện nay các hệ điều hành lớn đều sử dụng các thư viện đồ họa độc quyền khác nhau (Windows dùng DirectX, macOS dùng Metal, Linux dùng Vulkan). Bài viết phân tích cách thức WebGPU đóng vai trò như một lớp giao tiếp đồ họa thống nhất hỗ trợ chạy các tác vụ đồ họa 3D hiệu năng cao trực tiếp trên mọi trình duyệt web.

5\. [Nhìn lại chặng đường 30 năm phát triển ứng dụng máy tính PCalc của tác giả](https://pcalc.com/mac/thirty.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122402.webp)

Tác giả chia sẻ câu chuyện hồi ký đầy cảm xúc về hành trình tự tay viết phần mềm máy tính PCalc cho hệ máy Macintosh từ năm 1992 và kiên trì duy trì, nâng cấp, chuyển đổi mã nguồn của ứng dụng này suốt 30 năm qua để tương thích với các thiết bị thế hệ mới của Apple như iPhone và Apple Watch:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122403.webp)

6\. [Tự động hóa quy trình kiểm thử API HTTP bằng tiện ích dòng lệnh Hurl](https://brie.dev/2022-http-testing-hurl/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122701.webp)

Bài viết hướng dẫn cách sử dụng công cụ dòng lệnh Hurl để viết các kịch bản kiểm thử tự động gửi các yêu cầu HTTP tới API của hệ thống và kiểm tra các phản hồi đầu ra (status code, nội dung JSON) để bảo đảm hệ thống vận hành đúng đặc tả.

7\. [Phân tích so sánh các mô hình xử lý lỗi của các ngôn ngữ lập trình](https://www.amazingcto.com/best-way-to-handle-errors-for-a-programming-language/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041305.webp)

Bài viết so sánh ưu nhược điểm của các tư duy thiết kế xử lý lỗi khác nhau giữa các ngôn ngữ lập trình phổ biến (như cơ chế ném ngoại lệ Exception của Java, C# so với phương án trả về mã lỗi trực tiếp trong kết quả hàm của Go, Rust). Bạn đọc có thể xem thêm [bài viết cùng chủ đề](https://andreabergia.com/blog/2023/05/error-handling-patterns/).

8\. [Những điểm phức tạp và rắc rối khi xử lý chuỗi ký tự trong ngôn ngữ C](https://www.deusinmachina.net/p/c-strings-and-my-slow-descent-to)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040702.webp)

Bài viết phân tích sâu các vấn đề quản lý bộ nhớ của chuỗi ký tự trong ngôn ngữ C, từ ký tự kết thúc chuỗi null-terminator `\0` cho tới các khó khăn khi xử lý mã hóa đa ngôn ngữ Unicode, giúp người đọc hình dung được sự phức tạp của việc lập trình hệ thống cấp thấp.

## Công cụ

1、[stagit: Công cụ tự động chuyển đổi kho Git thành trang web tĩnh hiển thị](https://git.codemadness.org/stagit/)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121903.webp)

Một tiện ích dòng lệnh nhỏ gọn hỗ trợ lập trình viên tạo nhanh một trang web tĩnh hiển thị toàn bộ lịch sử commit, danh sách tệp tin và các thay đổi mã nguồn của một kho chứa Git để duyệt trực tuyến.

2、[Website Meta Tags Generator: Công cụ tạo các thẻ Meta hiển thị mạng xã hội](https://websitemetadata.com/meta-tags-generator)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101001.webp)

Khi chia sẻ đường dẫn trang web lên các mạng xã hội (như Facebook, Twitter), hệ thống sẽ tự động hiển thị một thẻ xem trước (preview card). Công cụ này hỗ trợ người dùng sinh nhanh các thẻ HTML Meta Tags (Open Graph) chính xác để trang web hiển thị đẹp nhất.

3、[CJK Font Detection: Công cụ nguồn mở nhận diện phông chữ Đông Á qua ảnh](https://github.com/JeffersonQin/YuzuMarker.FontDetection)

Ứng dụng nguồn mở hữu ích: người dùng chỉ cần tải lên một bức ảnh chụp có chứa các ký tự chữ viết Đông Á (Trung - Nhật - Hàn), hệ thống AI sẽ tự động phân tích nét chữ để nhận diện xem đoạn văn bản đó đang sử dụng phông chữ cụ thể nào. (Đóng góp của [@JeffersonQin](https://github.com/ruanyf/weekly/issues/3090))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050402.webp)

4、[microblog.pub: Giải pháp tự dựng trang mạng xã hội cá nhân nguồn mở](https://microblog.pub/)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101007.webp)

Mã nguồn mở hỗ trợ thiết lập một trang mạng xã hội dạng tin nhắn ngắn (microblog) cá nhân độc lập dành riêng cho một người sử dụng, có hỗ trợ kết nối chia sẻ dữ liệu với mạng lưới Fediverse thông qua giao thức ActivityPub.

5、[Textual Markdown Browser: Trình hiển thị và đọc file Markdown trong terminal](https://github.com/willmcgugan/textual-markdown)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121804.webp)

Một thư viện viết bằng Python hỗ trợ kết xuất và hiển thị các tệp tin tài liệu Markdown trực quan, giữ nguyên định dạng bảng biểu và màu sắc cú pháp ngay trong cửa sổ dòng lệnh terminal.

6、[HorusPass: Tiện ích chia sẻ văn bản bảo mật tự hủy sau một lần đọc](https://horuspass.com/send)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022501.webp)

Dịch vụ chia sẻ thông tin nhạy cảm bảo mật: người dùng nhập nội dung văn bản (như mật khẩu, khóa API), hệ thống sẽ cấp một đường dẫn URL chia sẻ. Đường dẫn này chỉ có thể truy cập để đọc duy nhất một lần, toàn bộ dữ liệu sẽ lập tức bị xóa sạch khỏi máy chủ sau đó.

7、[Progress-up: Thư viện JavaScript hỗ trợ tải tệp tin kèm thanh tiến độ](https://progress-up.live/)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022701.webp)

Một thư viện JS gọn nhẹ hỗ trợ lập trình viên tích hợp nhanh tính năng tải nhiều tệp tin lên máy chủ cùng lúc, hỗ trợ hiển thị tiến trình tải lên (progress bar) trực quan cho người dùng.

8、[snappify: Tiện ích tạo ảnh chụp màn hình mã nguồn chuyên nghiệp](https://snappify.com/editor)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120903.webp)

Ứng dụng web hỗ trợ các nhà phát triển tạo ra các bức ảnh chụp mã nguồn (code snippets) đẹp mắt với nhiều tùy chọn hình nền gradient, khung cửa sổ hệ điều hành để chia sẻ lên mạng xã hội hoặc chèn vào bài viết.

9、[RustDesk: Phần mềm điều khiển máy tính từ xa nguồn mở viết bằng Rust](https://rustdesk.com/)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121003.webp)

Giải pháp kết nối và điều khiển màn hình máy tính từ xa nguồn mở chất lượng cao thay thế cho các phần mềm trả phí thương mại (như TeamViewer, AnyDesk), hỗ trợ cài đặt ứng dụng khách trên mọi hệ điều hành.

10、[LosslessCut: Phần mềm cắt ghép video siêu tốc không cần giải mã lại](https://mifi.no/losslesscut/)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121403.webp)

Ứng dụng biên tập video chuyên dụng hỗ trợ cắt, ghép và chia nhỏ các tệp video mà không thực hiện quá trình render mã hóa lại dữ liệu (lossless), giúp xuất video đầu ra gần như ngay lập tức và giữ nguyên chất lượng gốc.

## 资源

1\. [ChatGPT Prompt Engineering for Developers: Khóa học viết Prompt chuyên nghiệp](https://www.deeplearning.ai/short-courses/chatgpt-prompt-engineering-for-developers/)

Khóa học trực tuyến miễn phí (bằng tiếng Anh) do giáo sư Andrew Ng phối hợp cùng các kỹ sư OpenAI xây dựng, hướng dẫn lập trình viên các kỹ thuật viết Prompt tối ưu để gọi API xây dựng các ứng dụng chatbot:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023043004.webp)

2\. [React & Next.js Complete Guide: Giáo trình học Next.js kèm phụ đề tiếng Trung](https://www.bilibili.com/read/cv20992052)

Chia sẻ bản dịch phụ đề tiếng Trung của khóa học lập trình React và Next.js được đánh giá cao trên nền tảng Udemy, hỗ trợ các lập trình viên frontend tự học. (Đóng góp của [@lyf61](https://github.com/ruanyf/weekly/issues/3093))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050403.webp)

3\. [QUIC Connection Illustrated: Bản dịch tài liệu trực quan hóa kết nối QUIC](https://cangsdarm.github.io/illustrate/quic)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050404.webp)

Bản dịch tiếng Trung của tài liệu giải thích chi tiết ý nghĩa kỹ thuật của từng byte dữ liệu truyền tải trong quá trình thiết lập kết nối của giao thức mạng thế hệ mới QUIC (HTTP/3). Bạn đọc có thể xem thêm [phiên bản gốc tiếng Anh](https://quic.xargs.org/). (Đóng góp của [@cangSDARM](https://github.com/ruanyf/weekly/issues/3094))

4、[Musico: Nền tảng nghe nhạc được soạn tự động bằng trí tuệ nhân tạo AI](https://www.musi-co.com/listen/streams)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022093004.webp)

Trang web giới thiệu năng lực của mô hình AI chuyên dụng cho mảng sáng tác âm nhạc, cho phép người dùng truy cập để nghe trực tiếp các bản nhạc không bản quyền được AI tự động sinh ra liên tục.

## 图片

1、**Bộ ảnh vẽ thêm biểu cảm ngộ nghĩnh biến những đám mây thành nhân vật hoạt hình**

Một nghệ sĩ người Mỹ đã thực hiện dự án nghệ thuật đáng yêu: chụp ảnh các đám mây trên bầu trời mỗi ngày và vẽ thêm các đường nét biểu cảm đơn giản để biến chúng thành những nhân vật hoạt hình sống động:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111716.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111717.webp)

Dự án ban đầu được thực hiện ngẫu hứng lúc rảnh rỗi, nhưng sau khi đăng tải lên mạng xã hội đã nhận được sự hưởng ứng rất lớn của cộng đồng người dùng:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111718.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111719.webp)

Nghệ sĩ chia sẻ: *"Chỉ cần bạn ngước mắt nhìn lên bầu trời xanh và ngắm nhìn những đám mây trôi, bạn sẽ nhận về nguồn cảm hứng sáng tạo vô tận"*. Hiện tại dự án đang được mở rộng với các bức ảnh đóng góp của người đọc từ khắp nơi trên thế giới:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111720.webp)

## ✍️ Bài đọc thêm

### Sơ đồ phân loại 7 cấp độ bận rộn trong cuộc sống thường nhật

Cuộc sống bận rộn của mỗi con người có thể được chia thành 7 cấp độ tăng dần. Hãy cùng tự đối chiếu xem bản thân bạn đang nằm ở cấp độ nào:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050405.webp)

* **Cấp độ 1: Hoàn toàn thong thả.** Bạn có toàn quyền quyết định quỹ thời gian của mình, không có bất kỳ đầu việc bắt buộc nào cần hoàn thành, ngày cuối tuần có thể ngủ nướng tùy thích.
* **Cấp độ 2: Có vài việc lặt vặt.** Bạn nhớ ra mình có một vài việc nhỏ cần giải quyết. Các công việc này hoàn toàn không có giới hạn thời gian (deadline) áp lực, nhưng bạn biết sớm muộn cũng phải hoàn thành chúng.
* **Cấp độ 3: Có các nhiệm vụ quan trọng.** Bạn bắt đầu có các công việc quan trọng bắt buộc phải hoàn thành đúng hạn, đòi hỏi phải theo sát tiến độ và không được phép trì hoãn. Bạn luôn phải tự nhắc nhở bản thân về chúng.
* **Cấp độ 4: Lịch biểu lấp đầy.** Lịch làm việc trong ngày của bạn đã kín chỗ. Bạn liên tục phải tự đặt câu hỏi *"Việc nào quan trọng hơn?"* để sắp xếp thứ tự ưu tiên xử lý trước sau. Bạn gần như không còn thời gian dự phòng ngoài kế hoạch nhưng vẫn kiểm soát tốt công việc.
* **Cấp độ 5: Bắt đầu rơi vào trạng thái quá tải.** Khối lượng công việc phát sinh không thể giải quyết hết trong giờ hành chính buộc bạn phải làm thêm giờ (OT). Bạn bắt đầu phải gửi lời xin lỗi tới mọi người xung quanh vì trễ hẹn. Một số công việc bắt đầu bị xử lý vội vàng, qua loa.
* **Cấp độ 6: Khối lượng công việc vượt ngoài tầm kiểm soát.** Số lượng đầu việc cần làm vượt quá khả năng tự sắp xếp lịch biểu của bạn. Ngay cả khi đã chủ động gạch bỏ một số việc phụ, bạn vẫn không thể hoàn thành phần việc còn lại. Thời gian làm việc kéo dài làm suy giảm nghiêm trọng sức khỏe và bạn luôn cảm thấy mệt mỏi, kiệt sức.
* **Cấp độ 7: Cuộc sống bế tắc.** Các nhiệm vụ đè nặng và chiếm trọn từng phút giây khi bạn thức giấc. Các hoạt động thiết yếu như ăn uống, ngủ nghỉ chỉ được thực hiện tranh thủ, thậm chí nhiều bữa bạn không có cả thời gian để ăn. Bạn không còn viết lịch biểu nữa vì tình thế thay đổi liên tục theo từng giờ, tâm trí luôn trong trạng thái lo âu và tiệm cận mức sụp đổ.

## Lịch sử tuần này

- 2022年（第 206 期）：[Tâm lý học: Lời khuyên giúp bản thân tự bước ra khỏi những nghi ngờ và thất vọng](http://www.ruanyifeng.com/blog/2022/05/weekly-issue-206.html)
- 2021年（第 156 期）：[Kinh tế số: Thảo luận về hiện trạng khan hiếm card đồ họa và sự cạnh tranh chéo ngành](http://www.ruanyifeng.com/blog/2021/04/weekly-issue-156.html)
- 2020年（第 106 期）：[Xu hướng xã hội: Tìm hiểu về phong cách sống và làm việc của cộng đồng Du mục kỹ thuật số](http://www.ruanyifeng.com/blog/2020/05/weekly-issue-106.html)
- 2019年（第 56 期）：[Xã hội học: Phân tích nguyên nhân tại sao sinh viên các ngành xã hội gặp khó khăn khi tìm kiếm việc làm](http://www.ruanyifeng.com/blog/2019/05/weekly-issue-56.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes team work easy.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
