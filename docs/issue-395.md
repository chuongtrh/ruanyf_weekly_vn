# 科技爱好者周刊（第 395 期）：软件开发的第三种方式 (Bản tin công nghệ hàng tuần số 395: Phương thức thứ ba của phát triển phần mềm)

Ghi lại nội dung công nghệ đáng chia sẻ hàng tuần, phát hành vào thứ Sáu.

Bản tin này [mã nguồn mở](https://github.com/ruanyf/weekly), hoan nghênh bạn [đóng góp](https://github.com/ruanyf/weekly/issues). Ngoài ra còn có dịch vụ [《Ai đang tuyển dụng》](https://github.com/ruanyf/weekly/issues/9815) đăng tải thông tin tuyển dụng lập trình viên. Hợp tác vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图 (Ảnh bìa)

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026050602.webp)

Bảo tàng Tự nhiên Thâm Quyến dự kiến hoàn thành trong năm nay, với thiết kế mô phỏng hình dáng một dòng sông uốn lượn mềm mại. ([via](https://baike.baidu.com/item/%E6%B7%B1%E5%9C%B3%E8%87%AA%E7%84%B6%E5%8D%9A%E7%89%A9%E9%A6%86/22596523))

## 软件开发的第三种方式 (Phương thức thứ ba của phát triển phần mềm)

Có một cuốn sách kinh điển nổi tiếng trong ngành phát triển phần mềm mang tên *Nhà thờ lớn và Chợ phi tập trung* (The Cathedral and the Bazaar), mọi người có biết không?

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026050712.webp)

Cuốn sách chỉ ra hai phương thức phát triển phần mềm chính:

Một là **Nhà thờ lớn** (Cathedral): Phần mềm được lập kế hoạch tỉ mỉ, do một đội ngũ chuyên gia đóng cửa tự nghiên cứu phát triển, toàn bộ quá trình tuân thủ các quy trình và kiểm soát nghiêm ngặt, mã nguồn thường đóng.

Hai là **Chợ phi tập trung** (Bazaar): Quy trình phát triển mở rộng hoàn toàn, bất kỳ ai cũng có thể tham gia đóng góp, quá trình đưa ra quyết định minh bạch do cộng đồng dẫn dắt, mã nguồn mở.

Cách so sánh này đã phân chia ngành công nghiệp phần mềm làm đôi một cách sâu sắc. Kể từ khi được đưa ra cách đây gần 30 năm, nó vẫn nhận được sự đồng thuận rộng rãi từ giới công nghệ.

Thế nhưng gần đây, có người lập luận rằng hai mô hình này đã không còn đủ để khái quát thực tế, và trong ngành phát triển phần mềm hiện tại đã xuất hiện một phương thức thứ ba: **Ngôi nhà bí ẩn** (Winchester Mystery House).

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026040502.webp)

"Ngôi nhà bí ẩn" là một dinh thự có thật nằm ở bang California (Mỹ), do một góa phụ giàu có xây dựng vào cuối thế kỷ 19.

Người phụ nữ này cực kỳ giàu có và sở hữu sở thích duy nhất là kiến trúc. Bà coi chính ngôi nhà của mình làm nơi thử nghiệm, xây dựng hết phòng này đến phòng khác hoàn toàn theo ý thích cá nhân của bà, tự tay thiết kế và giám sát thi công.

Ngôi nhà hoàn toàn không có bản quy hoạch tổng thể, thích xây thế nào thì xây thế đó: Phòng A theo phong cách Victoria, phòng B theo phong cách La Mã, phòng C theo phong cách Gothic... Nếu xây được một nửa mà bà không hài lòng, bà sẽ lập tức cho phá dỡ để xây lại từ đầu.

Hậu quả là toàn bộ dinh thự giống như một mê cung khổng lồ chằng chịt, phong cách mỗi phòng một kiểu. Theo hồ sơ ghi chép, căn phòng được xây đi xây lại nhiều nhất lên tới 16 lần. Để tiết kiệm công sức, nhiều cánh cửa ra vào và cửa sổ của phòng cũ không được tháo dỡ mà bị xây tường gạch bịt kín lại luôn.

Dinh thự được xây chồng thêm nhiều tầng qua các thời kỳ, cao nhất đạt tới 5 tầng, gồm khoảng 160 phòng nghỉ, 2.000 cánh cửa đi, 10.000 cửa sổ, 47 cầu thang, 47 lò sưởi, 13 phòng tắm và 6 phòng bếp. Sau khi bà qua đời vào năm 1922, nó được mở cửa cho công chúng tham quan và được mệnh danh là "Ngôi nhà bí ẩn".

Ngày nay, rất nhiều lập trình viên đang hành động giống như người phụ nữ giàu có đó.

Họ dùng AI để phát triển phần mềm, tự mình đưa ra các yêu cầu (prompts) và để AI viết code theo mọi ý thích phát sinh nhất thời, hoàn toàn không có khâu kiểm duyệt yêu cầu sản phẩm hay viết test kiểm thử mã nguồn.

Phần mềm cuối cùng được tạo ra có tính cá nhân hóa cực kỳ cao, quy mô đồ sộ, liên tục phình to, mã nguồn chồng chéo nhiều tầng mà không hề được tinh giản hay tối ưu hóa, chắp vá chằng chịt các bản vá lỗi (bug fixes). Hơn thế nữa, chúng thường không có tài liệu hướng dẫn và cực kỳ khó hiểu đối với người ngoài, hệt như "Ngôi nhà bí ẩn" vậy.

Tuy nhiên, quá trình phát triển này lại mang lại niềm vui lớn, khiến lập trình viên cảm thấy vô cùng thỏa mãn và chìm đắm trong thế giới riêng của mình.

Dưới sự trợ giúp của các mô hình AI ngày càng mạnh mẽ, các phần mềm kiểu "Ngôi nhà bí ẩn" đang bùng nổ hàng loạt, và rất có thể sẽ trở thành xu hướng chủ đạo trong tương lai, thay thế cả mô hình Nhà thờ lớn lẫn Chợ phi tập trung. Phần lớn phần mềm, đặc biệt là các dự án cá nhân hoặc của nhóm nhỏ, trong tương lai có lẽ đều sẽ được xây dựng theo cách này.

## 大模型流行度排行榜 (Bảng xếp hạng mức độ phổ biến của mô hình lớn)

Hầu hết bảng xếp hạng hiện nay đều dùng để đánh giá năng lực kỹ thuật của mô hình lớn. Tuy nhiên, có người đã thiết kế một phương pháp độc đáo để đo lường độ phổ biến (sự yêu thích) của các mô hình.

Cụ thể, hệ thống sẽ tự động quét 200 chủ đề hot nhất mỗi ngày trên cộng đồng [Hacker News](https://news.ycombinator.com/), lọc ra các chủ đề liên quan đến lập trình và AI, sau đó phân tích các bình luận phía dưới để thống kê xem mô hình nào được thảo luận nhiều nhất và nhận được nhiều đánh giá tích cực nhất.

Hacker News là cộng đồng lập trình viên danh tiếng với lượng truy cập và bình luận khổng lồ hàng ngày từ các kỹ sư công nghệ. Do đó, kết quả thống kê từ đây phản ánh rất chính xác mức độ phổ biến thực tế của các mô hình trong giới lập trình.

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026050405.webp)

Dự án mang tên [HN SOTA](https://hnup.date/hn-sota) và cập nhật bảng xếp hạng hàng ngày. Ba vị trí dẫn đầu tuần này lần lượt thuộc về: Claude Opus 4.7, GPT 5.5 và Claude Sonnet.

Các mô hình nội địa Trung Quốc như Kimi K2.6, DeepSeek V4, Qwen 3.6 và GLM 5.1 đều thành công lọt vào top 10.

## 科技动态 (Tin tức Công nghệ)

1. [Robot chó bầu bạn](https://www.wsj.com/tech/ai/familiar-machines-and-magic-robot-c8711e45): Colin Angle — nhà sáng lập hãng robot hút bụi nổi tiếng iRobot, sau khi nghỉ hưu đã tiếp tục nghiên cứu và cho ra mắt dòng robot chó chuyên phục vụ mục đích bầu bạn. Robot có vẻ ngoài thân thiện giống thú nhồi bông bằng lông mịn, có khả năng đi theo chủ và tương tác tự nhiên. Với công nghệ hiện tại, robot hoàn toàn có thể thay thế chó thật để làm bạn với con người mà không lo nguy cơ cắn người, sủa bậy hay mất công dắt đi dạo hàng ngày.

2. [Đèn pha ô tô tích hợp máy chiếu](https://insideevs.com/news/794295/chinese-ev-headlight-movie-projectors/): Huawei giới thiệu công nghệ tích hợp máy chiếu trực tiếp vào cụm đèn pha phía trước của ô tô. Khi đỗ xe, người dùng có thể bật đèn pha để chiếu video lên bức tường hoặc màn chắn phía trước để thưởng thức. Tính năng này rất thực dụng cho việc đi dã ngoại bằng xe hơi hoặc xem phim trong nhà xe. Để đảm bảo an toàn, máy chiếu có độ sáng rất cao này chỉ được phép kích hoạt khi xe đã đỗ hẳn để tránh gây chói mắt cho các xe đi ngược chiều.

3. [AI hỗ trợ phân loại bệnh nhân](https://www.theguardian.com/technology/2026/apr/30/ai-outperforms-doctors-in-harvard-trial-of-emergency-triage-diagnoses): Việc dùng AI thay thế bác sĩ khám bệnh vẫn đang gây nhiều tranh cãi. Tuy nhiên, Đại học Harvard đã thử nghiệm thành công việc đưa AI vào làm nhiệm vụ phân loại bệnh nhân ban đầu tại cửa phòng khám. AI dựa trên mô tả triệu chứng của bệnh nhân để đưa ra chẩn đoán sơ bộ và phân bổ vào chuyên khoa tương ứng với độ chính xác đạt 67%, vượt trội so với tỷ lệ 50-55% của các bác sĩ là con người.

4. [Tấn công chèn mã lệnh trên xe tự lái](https://www.theregister.com/2026/01/30/road_sign_hijack_ai/): Tương tự như các vụ tấn công chèn mã lệnh (prompt injection) trên mô hình ngôn ngữ lớn, các nhà nghiên cứu tại Đại học California phát hiện xe tự lái cũng có nguy cơ bị tấn công tương tự. Bằng việc giơ các tấm biển ghi chữ "Tiến lên" ở giữa đường, xe tự lái trong một số thử nghiệm thay vì dừng lại khi thấy người cản đường đã tiếp tục di chuyển theo mệnh lệnh ghi trên biển hiệu. Điều này cho thấy hệ thống tự lái cần có khả năng phân biệt biển báo giao thông hợp chuẩn và biển báo độc hại.

## 文章 (Bài viết)

1、[Tôi viết ứng dụng bản đồ cho Apple Watch](https://david-smith.org/blog/2026/04/29/maps-on-watchos/) (Tiếng Anh)

Tác giả chia sẻ lại hành trình thiết kế và phát triển ứng dụng bản đồ cho watchOS, đặc biệt là các khó khăn trong việc thiết kế giao diện UI tương thích với màn hình siêu nhỏ của đồng hồ.

2、[So sánh GPT Image 2 và Google Nano Banana 2](https://decrypt.co/366408/openai-gpt-image-2-vs-google-nano-banana-2-review) (Tiếng Anh)

Bài viết đánh giá và so sánh chất lượng hình ảnh tạo ra từ hai mô hình sinh ảnh mạnh mẽ nhất hiện nay của OpenAI và Google.

3、[Chrome tự động tải ngầm mô hình AI dung lượng 4GB](https://www.thatprivacyguy.com/blog/chrome-silent-nano-install/) (Tiếng Anh)

Phát hiện ra trình duyệt Chrome tự động tải xuống tệp tin mô hình AI `weights.bin` nặng tới 4GB về máy người dùng mà không hề thông báo. Nếu người dùng xóa đi, trình duyệt sẽ tự động tải lại trong các phiên tiếp theo.

4、[Phân tích chi tiết MacBook Neo](https://www.jdhodges.com/blog/macbook-neo-benchmarks-analysis/) (Tiếng Anh)

Phân tích hiệu năng dòng MacBook Neo giá rẻ ra mắt năm 2026 của Apple, dù chỉ trang bị dung lượng RAM 8GB nhưng vẫn được đánh giá là một sản phẩm rất xuất sắc trong tầm giá.

5、[CSS Animation dựa trên khung nhìn (Viewport)](https://www.joshwcomeau.com/animation/scroll-driven-animations/) (Tiếng Anh)

Thay vì chạy hoạt họa dựa trên thời gian truyền thống, API Animation Timeline mới hỗ trợ kích hoạt chuyển động dựa trên tỷ lệ phần trăm hiển thị và dịch chuyển của phần tử bên trong khung nhìn của trình duyệt.

6、[Tại sao bầu trời có màu xanh](https://explainers.blog/posts/why-is-the-sky-blue/) (Tiếng Anh)

Giải thích dễ hiểu các hiện tượng quang học liên quan đến màu sắc bầu trời: Tại sao ban ngày trời xanh, lúc hoàng hôn lại đỏ, tại sao mây có màu trắng, và tại sao bầu trời Sao Hỏa lại có màu đỏ còn hoàng hôn trên Sao Hỏa lại có màu xanh.

## 工具 (Công cụ)

1、[auge](https://auge.franzai.com)

Công cụ dòng lệnh cho macOS tận dụng framework thị giác máy tính Apple Vision tích hợp sẵn trong hệ thống để thực hiện phân tích và nhận diện hình ảnh trực tiếp từ terminal.

2、[BleachBit](https://github.com/bleachbit/bleachbit)

Phần mềm dọn rác hệ thống và xóa bộ nhớ đệm trình duyệt đa nền tảng nổi tiếng.

3、[Cicada](https://asong56.github.io/Cicada)

Ứng dụng bảng trắng viết tay chạy thuần trên trình duyệt chỉ với một tệp tin HTML duy nhất nặng 13KB không chứa bất kỳ dependency nào, toàn bộ dữ liệu vẽ được mã hóa lưu trữ trực tiếp trên đường dẫn URL. (Đóng góp từ [@Bennet7291](https://github.com/ruanyf/weekly/issues/9737))

4、[ASS Subsetter](https://subs.js.org/ass-subset/)

Công cụ web giúp nhúng phông chữ trực tiếp vào tệp phụ đề định dạng ASS để giảm dung lượng file phụ đề khi chia sẻ. (Đóng góp từ [@mtsubs](https://github.com/ruanyf/weekly/issues/9739))

5、[Infinitum](https://github.com/shawnxie94/infinitum)

Dịch vụ đọc tin RSS tự host nguồn mở tích hợp tính năng tự động lấy nội dung bài viết đầy đủ, phân tích nội dung bằng AI và tự động nhóm các sự kiện liên quan. (Đóng góp từ [@shawnxie94](https://github.com/ruanyf/weekly/issues/9773))

6、[tunnix](https://github.com/aeroxy/tunnix)

Giải pháp thiết lập đường truyền mã hóa SOCKS5/HTTP tunnel gồm ứng dụng cài trên server và client dòng lệnh. (Đóng góp từ [@aeroxy](https://github.com/ruanyf/weekly/issues/9779))

7、[curve-arrow](https://github.com/YYsuni/curve-arrow)

Công cụ web hỗ trợ thiết kế và xuất nhanh các hình mũi tên dạng đường cong định dạng SVG. (Đóng góp từ [@YYsuni](https://github.com/ruanyf/weekly/issues/9801))

8、[LynxDB](https://github.com/lynxbase/lynxdb)

Công cụ phân tích tệp nhật ký (log) hệ thống dưới dạng một file chạy duy nhất, hỗ trợ lọc thông tin từ nhiều nguồn log server khác nhau. (Đóng góp từ [@OrlovEvgeny](https://github.com/ruanyf/weekly/issues/9821))

9、[Chrome DevTools CLI](https://github.com/aeroxy/chrome-devtools-cli)

Công cụ dòng lệnh viết bằng Rust kết nối với Chrome thông qua giao thức DevTools để thực hiện các thao tác trên web tự động, thích hợp cho AI Agent gọi. (Đóng góp từ [@aeroxy](https://github.com/ruanyf/weekly/issues/9833))

10、[LaunchNext](https://github.com/RoversX/LaunchNext)

Ứng dụng nguồn mở thay thế cho giao diện Launchpad của macOS sau khi phiên bản mới của hệ điều hành lược bỏ hoặc thay đổi tính năng này gây khó dùng. (Đóng góp từ [@meichiny](https://github.com/ruanyf/weekly/issues/9862))

## AI 相关 (AI Liên quan)

1、[SpineDigest](https://github.com/oomol-lab/spinedigest)

Công cụ dòng lệnh hỗ trợ tóm tắt các tệp sách điện tử (ebook) dung lượng lớn thành sách tóm tắt ngắn gọn hơn bằng AI. (Đóng góp từ [@BlackHole1](https://github.com/ruanyf/weekly/issues/9813))

2、[Privacy Filter Online](https://privacyfilter.app/zh-hans/)

Dịch vụ web hỗ trợ kiểm tra và lọc bỏ các thông tin nhạy cảm cá nhân trong văn bản chạy hoàn toàn offline trên trình duyệt. (Đóng góp từ [@airyland](https://github.com/ruanyf/weekly/issues/9753))

3、[OpenClip](https://github.com/linzzzzzz/openclip)

Dịch vụ web hỗ trợ tự động tải video từ YouTube/Bilibili và dùng AI để tự động cắt trích xuất các phân cảnh nổi bật nhất của video. (Đóng góp từ [@linzzzzzz](https://github.com/ruanyf/weekly/issues/9780))

## 资源 (Tài nguyên)

1、[Nguyên lý hoạt động của mô hình ngôn ngữ lớn](https://ynarwal.github.io/how-llms-work/) (Tiếng Anh)

Tài liệu chi tiết đi kèm các sơ đồ tương tác giải thích trực quan về cơ chế vận hành của LLM cho người mới bắt đầu.

2、[Giáo trình C++ hiện đại](https://github.com/federico-busato/Modern-CPP-Programming) (Modern C++ Programming)

Bộ slide bài giảng chi tiết giúp các lập trình viên đã biết ngôn ngữ C nhanh chóng làm quen và làm chủ C++ hiện đại.

## 图片 (Hình ảnh)

1. [Bộ ảnh tàu Artemis II](https://artemistimeline.com): Trang web tổng hợp hơn 300 bức ảnh chất lượng cao ghi lại quá trình chuẩn bị và phóng tàu vũ trụ Artemis II đưa 4 phi hành gia thực hiện chuyến bay vòng quanh Mặt Trăng vào tháng 4 năm nay.

2. [Tem kỷ niệm Tuyến đường 66](https://apnews.com/article/route-66-potage-stamps-centennial-road-trip-84815c35b1f1536176d5040615c5e5c2): Bộ 8 mẫu tem đặc biệt do Bưu điện Mỹ phát hành nhằm kỷ niệm 100 năm ngày khai thông Tuyến đường 66 (Route 66) lịch sử nổi tiếng đi qua 16 bang.

## 文摘 (Văn trích)

1、[Bảo vệ ngôi nhà nhỏ của bạn](https://dylanbutler.dev/blog/protect-your-shed/)

Các dự án ở công ty giống như tòa nhà chọc trời, còn dự án cá nhân theo sở thích của bạn chính là ngôi nhà nhỏ. Những kỹ sư chỉ biết xây tòa nhà chọc trời ở công ty lâu dần sẽ rơi vào trạng thái kiệt quệ sức sáng tạo do công việc lặp đi lặp lại và bị gò bó bởi các yêu cầu thương mại. Hãy bảo vệ tốt các dự án cá nhân của mình, đó mới là nơi nuôi dưỡng trí tò mò, là nơi bạn thử nghiệm những điều mới lạ và giúp bạn giữ vững ngọn lửa đam mê với lập trình thay vì chỉ coi mình là một công nhân gõ code thuê.

2、[Mở cánh cửa xưởng gỗ khi làm việc](https://notes.andymatuschak.org/Work_with_the_garage_door_up)

Trên đường đi làm, tôi luôn đi qua một xưởng đồ gỗ luôn mở toang cánh cửa lớn. Việc nhìn vào bên trong thấy các công cụ xếp đặt gọn gàng và đống gỗ nguyên liệu mang lại cảm giác dễ chịu và phát đi tín hiệu: Nơi này đang hoạt động rất tốt. Trên internet cũng vậy, nếu bạn không lên tiếng chia sẻ công việc của mình thì cũng giống như xưởng gỗ đóng kín cửa, không ai biết bạn có tồn tại hay không. Việc liên tục lên tiếng chia sẻ chính là cách mở toang cánh cửa xưởng gỗ để mọi người biết bạn vẫn đang hoạt động tích cực.

## 言论 (Phát ngôn)

1、

> "Cơ chế khai thác của Monero (XMR) hoàn toàn khác với Bitcoin. Thiết kế của nó cố gắng giúp mọi máy tính cá nhân đều có thể tham gia đào và ngăn chặn lợi thế độc quyền của các máy đào chuyên dụng (ASIC). Thuật toán đào của Monero sẽ mô phỏng một CPU thông thường để khiến các chip ASIC chuyên dụng mất đi ưu thế vượt trội."
> 
> -- 《Cơ chế Proof of Work của Monero》

2、

> "Trong tương lai sẽ không còn vị trí kỹ sư junior (cấp thấp) nữa vì máy móc sẽ làm thay công việc của họ với chi phí rẻ hơn nhiều. Nhưng giá trị thực sự của junior không nằm ở những việc họ đang làm mà ở tiềm năng phát triển của họ trong tương lai. Có lẽ vài năm nữa chúng ta sẽ phải tự hỏi các kỹ sư senior (cấp cao) đã đi đâu hết rồi?"
> 
> -- stvn.sh

3、

> "Tốc độ viết code của AI quá nhanh khiến rào cản lớn nhất của các startup hiện tại chuyển sang khâu quản lý sản phẩm (Product Management). Khi việc dựng bản demo chỉ mất 1 ngày còn việc lấy feedback của người dùng mất cả tuần, đội ngũ buộc phải dựa vào trực giác nhiều hơn để ra quyết định nhanh."
> 
> -- Andrew Ng (Ngô Ân Đạt), chuyên gia AI nổi tiếng.

4、

> "Kế hoạch phát triển sự nghiệp của bạn thực ra chỉ gồm 3 bước: (1) Rèn luyện để bản thân cực kỳ giỏi ở một mảng nào đó, (2) Tìm cách kiếm tiền từ thế mạnh đó, và (3) Duy trì công việc đó lâu nhất có thể."
> 
> -- 《Làm thế nào để tôi gia nhập ngành công nghiệp game》

## 往年回顾 (Nhìn lại các năm trước)

[Li Fei-Fei (Lý Phi Phi): Từ người nhập cư đến ngôi sao AI](https://www.ruanyifeng.com/blog/2025/05/weekly-issue-348.html)（#348）

[Đã đến lượt kỹ sư phần cứng lên ngôi](https://www.ruanyifeng.com/blog/2024/04/weekly-issue-298.html)（#298）

[Đừng thổi phồng quá mức về ChatGPT](https://www.ruanyifeng.com/blog/2023/03/weekly-issue-248.html)（#248）

[Liệu việc khôi phục sản xuất tại Mỹ có khả thi?](https://www.ruanyifeng.com/blog/2022/03/weekly-issue-198.html)（#198）

(Hết)
