# Bản tin chia sẻ công nghệ (Số 386): Khi shipper giao đồ ăn kết nối với AI

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/8882) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026020702.webp)

Tác phẩm nghệ thuật sắp đặt mang tên 《Bánh lái》 nằm bên bờ sông Hoàng Phố, Thượng Hải. Khu vực này vốn là phế tích của một xưởng đóng tàu cũ có xây một bức tường ngăn lũ lớn. Để thu hút người dân đến tham quan dạo bộ và tái hiện lại chủ đề đóng tàu lịch sử, các kiến trúc sư đã thiết kế nên công trình độc đáo này. ([via](https://www.gooood.cn/shanghai-urban-space-art-season-susas-2025-by-shanghai-summits-architecture.htm))

## 当外卖员接入 AI

Gần đây, một [tin tức về mảng xe tự hành](https://www.cnbc.com/2026/02/12/waymo-is-paying-doordash-gig-workers-to-close-its-robotaxi-doors.html) tại Mỹ đã tạo nên những làn sóng thảo luận vô cùng sôi nổi.

Waymo là một công ty xe tự hành hiện đang vận hành dịch vụ taxi tự lái (Robotaxi) tại nhiều thành phố lớn của Mỹ.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021608.webp)

Khó khăn lớn nhất mà hãng gặp phải là sau khi hành khách xuống xe, họ thường quên không đóng chặt cửa xe hoặc cửa cốp sau, khiến xe không thể tự rời đi.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021610.webp)

Điều kỳ lạ là một công ty công nghệ cao như vậy lại không thiết kế tính năng đóng cửa xe từ xa, mà thay vào đó họ đã nghĩ ra một giải pháp vô cùng độc lạ: Lên đơn hàng trên app DoorDash, trả tiền thuê các shipper giao đồ ăn đến hiện trường để... đóng hộ cửa xe.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021609.webp)

Một shipper đã chia sẻ bức ảnh chụp đơn hàng kỳ lạ mà anh nhận được trên app: đơn hàng trị giá 6,25 USD yêu cầu anh di chuyển quãng đường 1 km đến địa điểm chỉ định để tìm một chiếc xe taxi tự lái Waymo và đóng hộ cửa xe lại. Sau khi hoàn thành, anh còn nhận được khoản thưởng thêm trị giá 5 USD từ hệ thống.

Vì thấy sự việc quá thú vị nên anh đã chụp màn hình đăng lên mạng xã hội, và chủ đề này lập tức nhanh chóng trở thành tiêu điểm tin tức công nghệ.

Điểm đắt giá của tin tức này thực chất không nằm ở việc shipper đi đóng hộ cửa xe, mà là ở chỗ: **Chương trình máy tính đang chủ động điều động nhân lực con người để hoàn thiện một quy trình tự động hóa**.

Từ trước đến nay, các chương trình máy tính chỉ có khả năng điều động tài nguyên phần cứng máy tính. Nhưng hiện nay, nó đã có thể trực tiếp điều động sức lao động của con người: khi gặp một mắt xích vật lý ngoài đời thực mà máy móc chưa thể hoàn thành, hệ thống sẽ tự động tìm kiếm con người phù hợp để giải quyết. Đây mới là bản chất của sự thay đổi.

Giải pháp này sở hữu khả năng vận hành thành công hoàn toàn nhờ thực tế: **các shipper giao đồ ăn là một lực lượng lao động được tích hợp sẵn các API kết nối**. Họ đã gia nhập vào hệ thống phần mềm, trở thành một lực lượng lao động tự động hóa mà các chương trình máy tính có thể gọi và điều động dễ dàng thông qua các cổng giao tiếp kết nối.

Nếu phân tích kỹ hiện tượng này, bạn sẽ nhận ra trong kỷ nguyên của trí tuệ nhân tạo và robot, nghề shipper giao đồ ăn sở hữu một giá trị vô cùng đặc biệt và là một công việc đầy tiềm năng. **Vai trò của họ không còn giới hạn ở việc giao nhận đồ ăn, mà hoàn toàn có thể nâng cấp thành một lực lượng lao động vật lý được điều khiển và gọi từ xa qua phần mềm**, đóng vai trò là một mắt xích trung gian kết nối giữa thế giới số và thế giới vật lý của quy trình tự động hóa "Máy móc + Con người".

Một khi mô hình AI lớn được kết hợp chặt chẽ với sức lao động của con người, phạm vi ứng dụng của AI sẽ được mở rộng cực kỳ mạnh mẽ. Hệ thống OpenClaw hiện nay mới chỉ hỗ trợ thao tác trên máy tính, nhưng **các trợ lý AI trong tương lai sẽ phát triển thành các bộ máy điều phối và phân bổ sức lao động của con người**.

Lấy ví dụ khi bạn có nhu cầu sửa sang lại căn nhà: AI sẽ tự động lên phương án thiết kế chi tiết, sau đó tự động phân rã dự án thành các tác vụ nhỏ đăng lên mạng để tìm thợ điện, thợ ống nước nhận việc. Khi các thợ kỹ thuật hoàn thành công việc và được kỹ sư giám sát độc lập xác nhận đạt yêu cầu, AI sẽ tự động thanh toán chi phí và tiếp tục phân bổ việc cho thợ nề, thợ mộc... cho đến khi căn nhà hoàn thiện.

Đến thời điểm đó, chỉ với một câu lệnh đơn giản: "Tôi muốn sửa nhà", toàn bộ quy trình thiết kế và thi công thực tế ngoài đời thực sẽ được AI tự động vận hành hoàn thành cho bạn.

Các nền tảng AI khi đó sẽ chuyển dịch thành các cổng môi giới lao động khổng lồ. Con người có thể tìm kiếm việc làm trực tiếp qua AI, nhận các nhiệm vụ thực tế do AI phân bổ và nhận về các khoản thù lao tương xứng.

Tóm lại, một khi sức lao động của con người được tích hợp và điều phối bởi AI, công nghệ này sẽ không chỉ dừng lại ở một cuộc cách mạng máy tính thông thường, mà toàn bộ cấu trúc kinh tế xã hội của loài người sẽ được định hình và tái cấu trúc xoay quanh nó.

## [本周软件] PinMe：去中心化托管服务

Khi các liên kết trang web bị hỏng, website bị đóng cửa hay tên miền bị hủy bỏ, làm thế nào để chúng ta có thể lưu trữ nội dung **vĩnh viễn** trên môi trường Internet?

Một giải pháp công nghệ hiện nay là ứng dụng giao thức IPFS (InterPlanetary File System - Hệ thống tệp liên hành tinh): thông qua giao thức phân tán để chia sẻ nội dung trên toàn bộ các nút mạng, với địa chỉ truy cập chính là mã băm (hash) của nội dung tệp tin.

Do đó, một khi tệp tin đã được tải lên mạng IPFS, không một ai có thể sửa đổi nội dung tệp (vì bất kỳ thay đổi nào cũng làm thay đổi mã băm) và cũng không thể xóa bỏ tệp tin (vì nội dung luôn được lưu trữ dự phòng ở các nút mạng khác).

Công cụ [PinMe](https://pinme.eth.limo/) được giới thiệu tuần này chính là một giải pháp quản lý lưu trữ IPFS tiện lợi như vậy.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022202.webp)

Bạn có thể sử dụng công cụ để tải bất kỳ tệp tin nào lên mạng lưới IPFS. Khi bạn tải lên một trang web tĩnh, trang web đó trên lý thuyết sẽ tồn tại vĩnh viễn và không một ai (kể cả bạn) có khả năng sửa đổi hay đóng cửa trang web, người dùng có thể truy cập trang web thông qua bất kỳ cổng trung chuyển IPFS nào.

PinMe hỗ trợ cấp một tên miền ENS trỏ trực tiếp đến nội dung tải lên. Tên miền này được ghi trực tiếp vào chuỗi khối Ethereum nên cũng sở hữu đặc tính vĩnh viễn không thể bị xóa bỏ.

Dịch vụ cung cấp hạn ngạch lưu trữ miễn phí lên tới 1 GB, người dùng có nhu cầu sử dụng dung lượng lớn hơn hoặc cấu hình tên miền cá nhân có thể tùy chọn nâng cấp trả phí.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022203.webp)

Người dùng có thể tải tệp lên trực tiếp qua giao diện web hoặc sử dụng [công cụ dòng lệnh mã nguồn mở](https://github.com/glitternetwork/pinme) của dự án để upload nhanh chỉ với một dòng lệnh duy nhất. Dự án hiện đã nhận được hơn 2.800 lượt yêu thích trên GitHub. Nếu bạn có nhu cầu lưu trữ dữ liệu vĩnh viễn, hãy [trải nghiệm thử dịch vụ](https://pinme.eth.limo/).

## 科技动态

1. **Thí nghiệm thú vị về dây dẫn tín hiệu âm thanh**

Dây truyền dẫn tín hiệu âm thanh có chất liệu càng tốt thì giá thành càng đắt đỏ, nhưng liệu tai con người có thực sự phân biệt được sự khác biệt đó không?

Một người đam mê âm thanh tại Mỹ đã thực hiện cuộc thử nghiệm thú vị: lần lượt sử dụng dây đồng chuyên dụng, một quả chuối và một miếng bùn ướt để làm vật dẫn truyền tín hiệu âm thanh.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021605.webp)

Ông cho nhiều người nghe thử ở chế độ giấu thông tin (blind test), kết quả thật kinh ngạc khi không một ai có thể phân biệt được sự khác biệt về chất lượng âm thanh giữa các vật dẫn này.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021606.webp)

Điều này vô cùng bất ngờ. Theo lý thuyết vật lý, quả chuối và miếng bùn ướt hoàn toàn không phải là những chất dẫn điện tốt, nhưng cuộc thí nghiệm đã chứng minh chúng chỉ làm tăng thêm một chút điện trở để làm giảm cường độ tín hiệu chứ hoàn toàn không hề gây nên hiện tượng méo tiếng hay sụt giảm chất lượng âm thanh đáng kể.

2. **Ứng dụng AI bảo trì mã nguồn COBOL**

COBOL là ngôn ngữ lập trình của thế kỷ trước và hiện nay hầu như không còn lập trình viên nào mặn mà sử dụng nữa.

Tuy nhiên, rất nhiều hệ thống lõi quan trọng của các tập đoàn tài chính lớn tại Mỹ vẫn đang vận hành bằng mã nguồn COBOL. Do không có lập trình viên am hiểu nên các doanh nghiệp bắt buộc phải ký kết các hợp đồng bảo trì với mức giá cực kỳ đắt đỏ với tập đoàn IBM – đơn vị duy nhất có khả năng bảo trì hệ thống này.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022404.webp)

Thứ Hai vừa qua (ngày 23 tháng 2), hãng Anthropic đã bất ngờ công bố một nghiên cứu trên trang chủ (hình trên), tuyên bố mô hình Claude của họ đã sở hữu năng lực tự động phân tích và chuyển đổi mã nguồn COBOL sang các ngôn ngữ lập trình hiện đại.

Thông tin này lập tức khiến giá cổ phiếu của tập đoàn IBM ghi nhận mức sụt giảm mạnh.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022405.webp)

Nếu AI thực sự làm chủ được khả năng bảo trì mã nguồn COBOL, liệu điều này có đồng nghĩa với việc các bài toán bảo trì mã nguồn cũ (legacy code) trong tương lai sẽ không còn là gánh nặng kỹ thuật nữa? Và lập trình viên chúng ta sẽ không còn phải ngao ngán mỗi khi phải tiếp nhận các dự án cũ từ thế hệ trước?

3. **Vấn đề bản quyền đối với các đoạn code do AI viết**

Theo các quy định pháp luật hiện hành của Mỹ, quyền bảo hộ tác giả (copyright) chỉ được cấp cho các sản phẩm sáng tạo từ trí tuệ của con người, còn các kết quả do AI sinh ra hoàn toàn không được thừa nhận quyền bảo quyền tác giả.

Điều này đồng nghĩa với việc các đoạn mã nguồn do AI tự động viết ra (tại Mỹ) hoàn toàn không có bản quyền, và bất kỳ ai cũng có quyền tự do sao chép và sử dụng vào mục đích cá nhân.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021415.webp)

Đây là điểm lưu ý vô cùng quan trọng đối với các dự án lập trình bằng AI được chia sẻ trên GitHub. Thực chất chúng hoàn toàn không có bản quyền bảo hộ, ngay cả khi nhà phát triển có đính kèm tuyên bố bản quyền hay cấp các giấy phép sử dụng (licenses) thì các tuyên bố đó vẫn vô hiệu trước pháp luật. Bởi GitHub là doanh nghiệp đăng ký tại Mỹ và bắt buộc phải tuân thủ nghiêm ngặt luật pháp nước sở tại.

Trừ trường hợp nhà phát triển chứng minh và phân tách rõ ràng phần mã nguồn nào do con người tự viết và phần nào do AI sinh ra để đăng ký bảo hộ riêng cho phần nội dung do con người sáng tạo.

4. **Robot nhà sư tại Nhật Bản**

Đại học Kyoto của Nhật Bản vừa giới thiệu một mẫu robot nhà sư độc đáo, phần cứng được phát triển dựa trên robot của hãng Unitree, còn phần mềm là mô hình ChatGPT được huấn luyện chuyên sâu bằng kinh Phật.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022603.webp)

Robot có nhịp bước di chuyển chậm rãi, có khả năng thực hiện các cử chỉ chắp tay, cúi chào, hỗ trợ đàm đạo Phật pháp, tư vấn giải đáp các thắc mắc cuộc sống cho Phật tử và thậm chí có thể chủ trì các nghi thức cầu an đơn giản.

Khi được hỏi về "khó khăn khi nghiện rượu", robot trả lời: "Hãy tránh xa những thứ gây hại cho thân tâm, giữ gìn giới không uống rượu, chăm chỉ hành thiện mới đạt được sự an lạc thực sự". Khi được hỏi về giải pháp cho "tính khí nóng nảy, khó tập trung", robot khuyên: "Chớ cầu thành công nhanh chóng, hãy an trú ở hiện tại, quán chiếu từng sự việc gặp phải, thấu hiểu nhu cầu thực sự của tâm mình, từ từ xử lý thì tâm trí tự khắc sẽ sáng rõ".

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022602.webp)

Đại học Kyoto chia sẻ trong tuyên bố rằng mẫu robot này trong tương lai có thể hỗ trợ hoặc thay thế con người thực hiện một số nghi thức tôn giáo cơ bản, giải quyết bài toán thiếu hụt nhân sự nhà sư do tình trạng già hóa dân số và sụt giảm lực lượng lao động tại Nhật Bản.

Thiết bị sẽ được đưa vào chạy thử nghiệm thực tế trong vòng 6 tháng bắt đầu từ tháng 3 tại chùa Shoren-in Temple ở Kyoto. Nếu kết quả khả quan, phiên bản thương mại dự kiến sẽ ra mắt vào năm 2027 để cung cấp dịch vụ thuê robot cho các ngôi chùa nhỏ để duy trì hoạt động.

## 文章

1. [Khuyến nghị nên thay thế kiểm thử bằng SWE-bench Verified](https://openai.com/index/why-we-no-longer-evaluate-swe-bench-verified/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022617.webp)

Bộ công cụ kiểm thử SWE-bench Verified do OpenAI xây dựng hiện là thước đo phổ biến nhất để đánh giá năng lực lập trình của các mô hình AI.

Tuy nhiên tuần này, chính OpenAI đã lên tiếng đề xuất cộng đồng nên ngừng sử dụng bộ kiểm thử này do phát hiện nhiều lỗi thiết kế không thể khắc phục làm sai lệch kết quả đánh giá, đồng thời khuyến nghị chuyển sang sử dụng bộ kiểm thử SWE-Bench Pro do ScaleAI phát triển.

2. [Quản lý công việc tối giản bằng các tệp tin dạng `.plan`](https://matteolandi.net/plan-files.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021613.webp)

Tác giả bài viết chia sẻ quan điểm cho rằng việc sử dụng các tệp tin văn bản thuần túy `.plan` kết hợp lưu trữ đám mây là giải pháp quản lý công việc tối ưu và tiện lợi nhất, giúp người dùng dễ dàng truy cập và biên tập ghi chú trên mọi thiết bị.

3. [Hiện tượng "Kình lạc" (Whale Fall) trong thế giới mã nguồn](https://nesbitt.io/2026/02/21/whale-fall.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022616.webp)

Hiện tượng tự nhiên "Một con cá voi nằm xuống, vạn sinh vật đại dương được hồi sinh". Tác giả mượn hình ảnh này để phân tích về thế giới phần mềm: khi một dự án lớn bị dừng hoạt động, dữ liệu và mã nguồn của nó không hề biến mất mà sẽ nhanh chóng được cộng đồng tái sử dụng để phát triển thành hàng loạt dự án nhỏ hữu ích khác.

4. [Hướng dẫn xây dựng dịch vụ OCR không máy chủ chỉ với 40 dòng code](https://christopherkrapu.com/blog/2026/ocr-textbooks-modal-deepseek/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021701.webp)

Bài viết hướng dẫn lập trình viên sử dụng các hàm đám mây kết nối tới mô hình DeepSeek OCR để tự động quét chuyển đổi các tài liệu toán học định dạng PDF sang định dạng văn bản Markdown một cách nhanh chóng.

5. [Giải pháp thiết lập chuyển vùng mạng nội bộ (roaming) chỉ với 2 router](https://popring.cn/blog/home-network-issues) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022001.webp)

Trong trường hợp 2 thiết bị router trong nhà không hỗ trợ công nghệ Mesh, tác giả hướng dẫn cách thức cấu hình đưa chúng về cùng một mạng nội bộ để thiết bị di động có thể tự động chuyển kết nối mượt mà khi di chuyển. (Đóng góp từ [@popring](https://github.com/ruanyf/weekly/issues/9042))

6. [Giải pháp thiết kế ẩn phần tử giao diện mới nhất bằng CSS](https://dbushell.com/2026/02/20/visually-hidden/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022103.webp)

Kỹ thuật ẩn giao diện (visually hidden) giúp ẩn hoàn toàn một phần tử trên màn hình thiết bị nhưng vẫn bảo đảm các trình đọc màn hình chuyên dụng (screen readers) quét đọc được dữ liệu. Bài viết giới thiệu các cú pháp CSS mới nhất để thiết lập tính năng này.

7. [Tìm hiểu về động cụ Pi chạy dưới hệ thống OpenClaw](https://www.onuruzunismail.com/blog/the-engine-behind-the-hype) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022407.webp)

Sự bùng nổ của dự án OpenClaw kéo theo sự quan tâm lớn của cộng đồng dành cho động cơ chạy ngầm của nó mang tên Pi. Đây là một Coding Agent có tính năng tương tự Claude Code nhưng được tối ưu hóa gọn nhẹ và linh hoạt hơn.

## 工具

1. [Oat](https://github.com/knadh/oat)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021601.webp)

Thư viện giao diện (UI kit) mã nguồn mở siêu nhẹ kết hợp giữa HTML, CSS và các cú pháp JavaScript tối giản hướng tới trải nghiệm thiết kế giao diện chuẩn ngữ nghĩa.

2. [jsonriver](https://github.com/rictic/jsonriver)

Thư viện JavaScript hỗ trợ bóc tách và phân tích cú pháp các luồng dữ liệu ký tự JSON, giải pháp thay thế rất tốt cho hàm mặc định `JSON.parse()` vốn không hỗ trợ cơ chế xử lý luồng dữ liệu (streaming).

3. [Arcmark](https://github.com/Geek-1001/arcmark)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021607.webp)

Ứng dụng quản lý dấu trang (bookmarks) dành cho hệ điều hành macOS, hỗ trợ tự động gắn chặt vào cạnh màn hình cửa sổ trình duyệt web để tiện thao tác.

4. [Systemd manager tui](https://github.com/matheus-git/systemd-manager-tui)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021611.webp)

Công cụ hỗ trợ quản trị viên dễ dàng quản lý và giám sát các dịch vụ Systemd trực tiếp trên giao diện dòng lệnh terminal.

5. [weathr](https://github.com/Veirt/weathr)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022104.webp)

Ứng dụng dòng lệnh hỗ trợ tra cứu thông tin thời tiết tại địa điểm chỉ định hiển thị kèm các hiệu ứng đồ họa hoạt họa sinh động.

6. [CursorLens](https://github.com/blueberrycongee/CursorLens)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021603.webp)

Phần mềm quay video màn hình máy tính chuyên dụng hỗ trợ các tính năng phóng to thu nhỏ con trỏ chuột phục vụ việc thiết kế các video hướng dẫn sử dụng sản phẩm. (Đóng góp từ [@blueberrycongee](https://github.com/ruanyf/weekly/issues/9019))

7. [Ketsuin (结印)](https://github.com/huanglizhuo/Ketsuin)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021502.webp)

Ứng dụng web giải trí độc đáo sử dụng camera thiết bị để nhận diện các động tác kết thủ ấn trong bộ truyện tranh nổi tiếng Naruto và chuyển đổi chúng thành các ký tự nhập liệu tương ứng. (Đóng góp từ [@huanglizhuo](https://github.com/ruanyf/weekly/issues/9018))

8. [Puter](https://github.com/HeyPuter/puter)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061105.webp)

Hệ điều hành đám mây (cloud OS) mã nguồn mở chạy trực tiếp trên trình duyệt hỗ trợ người dùng tự triển khai lưu trữ riêng. Tham khảo thêm [bài viết giới thiệu chi tiết](https://www.xda-developers.com/this-cracking-cloud-computer-can-be-anything/). (Đóng góp từ [@cosmicqbit](https://github.com/ruanyf/weekly/issues/9043))

9. [Penio](https://github.com/game1024/Penio)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022102.webp)

Ứng dụng hỗ trợ giảng dạy trực quan, giúp hiển thị phóng to và làm nổi bật các thao tác nhấp chuột và gõ phím trên màn hình máy tính của giáo viên. (Đóng góp từ [@game1024](https://github.com/ruanyf/weekly/issues/9046))

10. [openhare](https://github.com/sjjian/openhare)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022401.webp)

Công cụ truy vấn SQL đa cơ sở dữ liệu phát triển bằng Flutter hỗ trợ chạy đa nền tảng, tích hợp sẵn các tính năng AI giúp tự động sinh các câu lệnh truy vấn SQL và phân tích nhanh dữ liệu. (Đóng góp từ [@sjjian](https://github.com/ruanyf/weekly/issues/9056))

## AI 相关

1. [BitFun](https://github.com/GCWing/BitFun)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021501.webp)

Trình soạn thảo mã nguồn tích hợp trợ lý AI lập trình mã nguồn mở, giao diện và tính năng được định vị cạnh tranh trực tiếp với Cursor. (Đóng góp từ [@GCWing](https://github.com/ruanyf/weekly/issues/9004))

2. [Xcode Proxy](https://github.com/tianrking/xcode-proxy)

Dịch vụ chạy local viết bằng Python đóng vai trò làm cổng trung chuyển giúp trình biên dịch Xcode dễ dàng kết nối và gọi các dịch vụ AI từ các nhà cung cấp bên thứ ba. (Đóng góp từ [@tianrking](https://github.com/ruanyf/weekly/issues/9024))

3. [openapi-to-skills](https://neutree.ai/projects/openapi-to-skills)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021901.webp)

Công cụ hỗ trợ phân tách các tài liệu OpenAPI kích thước lớn thành các cấu trúc Skills nhỏ gọn hỗ trợ nạp theo nhu cầu, giúp mô hình AI gọi chính xác các endpoint cần thiết và hạn chế tối đa hiện tượng hao phí Token và lỗi ảo giác. (Đóng góp từ [@Yuyz0112](https://github.com/ruanyf/weekly/issues/9036))

4. [Trending AI](https://github.com/HarlonWang/TrendingAI)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022201.webp)

Ứng dụng di động mã nguồn mở sử dụng trí tuệ nhân tạo để tự động tóm tắt thông tin tính năng của các dự án đang lọt top GitHub Trending hàng ngày. (Đóng góp từ [@HarlonWang](https://github.com/ruanyf/weekly/issues/9047))

5. [Horizon](https://github.com/Thysrael/Horizon)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022302.webp)

Dự án Python hỗ trợ người dùng quét thông tin từ các nguồn tin cấu hình sẵn, tự động lọc nội dung quan trọng và tóm tắt để kết xuất thành một bản tin tổng hợp hàng ngày. (Đóng góp từ [@Thysrael](https://github.com/ruanyf/weekly/issues/9055))

6. [JadeAI](https://github.com/twwch/JadeAI)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022402.webp)

Ứng dụng thiết kế sơ yếu lý lịch thông minh viết bằng Next.js, hỗ trợ giao diện kéo thả trực quan và tích hợp AI giúp tối ưu hóa nội dung CV từ 50 mẫu chuyên nghiệp có sẵn. (Đóng góp từ [@twwch](https://github.com/ruanyf/weekly/issues/9058))

## 资源

1. [Kho lưu trữ game và hoạt hình flash cổ (Flashpoint Database)](https://flashpointproject.github.io/flashpoint-database/)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021602.webp)

Dự án cộng đồng khổng lồ chuyên sưu tầm và lưu trữ các tựa game và hoạt hình chạy trên nền tảng Flash cổ xưa. Kho lưu trữ hiện lưu giữ hơn 180.000 trò chơi và 30.000 tệp hoạt hình khác nhau.

2. [Kho tài liệu tự học Claude Code bằng tiếng Trung](https://github.com/KimYx0207/Claude-Code-Guide-Zh)

Kho lưu trữ chia sẻ tài liệu hướng dẫn sử dụng công cụ Claude Code được biên soạn chi tiết qua 10 chương chuyên đề. (Đóng góp từ [@KimYx0207](https://github.com/ruanyf/weekly/issues/9022))

3. [Bản đồ mô phỏng mực nước biển dâng](https://www.runcell.dev/tool/true-size-map/sea-level-rise-simulator)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022614.webp)

Công cụ trực tuyến hỗ trợ người dùng tùy chỉnh độ cao của mực nước biển dâng lên để theo dõi trực quan các thay đổi trên bản đồ vệ tinh xem những khu vực địa hình nào sẽ bị nhấn chìm. (Đóng góp từ [@ObservedObserver](https://github.com/ruanyf/weekly/issues/9070))

4. [Công cụ mô phỏng bảng mạch điện tử Diode](https://www.withdiode.com/)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022408.webp)

Trang web hỗ trợ người dùng thiết kế và chạy thử nghiệm các sơ đồ mạch điện tử trên bảng mạch thử (breadboard) trực quan bằng việc kéo thả các linh kiện và theo dõi kết quả vận hành thực tế.

## 图片

1. **Trải nghiệm trình duyệt web đầu tiên của nhân loại**

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022101.webp)

Vào năm 1990, nhà nghiên cứu Tim Berners-Lee công tác tại Tổ chức Nghiên cứu Hạt nhân Châu Âu (CERN) đã phát minh ra mạng lưới WWW (World Wide Web) mở ra kỷ nguyên duyệt web của nhân loại.

Hiện tại trên trang chủ của CERN đã cung cấp một phiên bản mô phỏng trực tuyến trình duyệt web đầu tiên này (hình trên) để người dùng thế hệ sau có cơ hội trải nghiệm lịch sử.

Đồng thời trang web cũng cho phép người dùng truy cập trải nghiệm [trang web đầu tiên của thế giới](https://info.cern.ch/) dưới đây:

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022601.webp)

2. **Cách thức bố trí màn hình làm việc của lập trình viên**

Bàn làm việc của một kỹ sư lập trình thường được trang bị từ một cho tới rất nhiều màn hình hiển thị khác nhau phục vụ công việc.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022410.webp)

Cộng đồng mạng đã tổng hợp các sơ đồ bố trí màn hình phổ biến nhất dưới đây, hãy thử xem góc làm việc của bạn hiện đang thuộc phong cách nào?

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022409.webp)

## 文摘

1. **Mối cơ duyên bất ngờ của nghiên cứu khí động học xe tải**

Vào năm 1973, một kỹ sư công tác tại NASA trên đường đạp xe đi làm đã bị luồng khí mạnh từ một chiếc xe tải lớn phóng nhanh qua người đẩy văng cả người và xe vào lề đường.

Trong khi phần lớn mọi người sẽ chỉ cảm thấy hoảng sợ, người kỹ sư này lập tức suy ngẫm: sức gió đẩy mạnh chứng tỏ lực cản không khí của chiếc xe tải là vô cùng khổng lồ.

Ngay khi về đến phòng thí nghiệm, anh đã tập hợp các đồng nghiệp và mượn một chiếc xe tải Ford cũ để tiến hành các cuộc thí nghiệm khí động học nhằm tìm giải pháp tối ưu hóa lực cản để tiết kiệm nhiên liệu cho xe tải.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022307.webp)

Ban đầu họ ốp các tấm nhôm phẳng bao quanh cabin xe (hình trên) để đo các thông số lực cản không khí tiêu chuẩn làm hệ quy chiếu.

Sau đó họ thử nghiệm mài tròn các góc vuông ở đầu xe (hình dưới) để đo đạc các thay đổi của lực cản.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022308.webp)

Tiếp theo họ thực hiện việc ốp kín phần gầm xe để luồng không khí lưu chuyển mượt mà hơn dưới thân xe.

Kết quả đo đạc thực tế chỉ ra: việc mài bo tròn các góc vuông phía trước giúp giảm tới 52% lực cản không khí; việc ốp kín gầm xe giúp giảm thêm 7% lực cản. Nhóm nghiên cứu ước tính các cải tiến này sẽ giúp tiết kiệm từ 15% đến 25% lượng nhiên liệu tiêu thụ của xe tải khi chạy trên đường cao tốc.

Cuối cùng họ tiến hành lắp thêm các tấm chắn gió (整流罩) phía trên cabin và đầu xe kết hợp cánh lướt gió phía sau để giảm thêm 15% lực cản.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022309.webp)

Diện mạo chiếc xe độ thử nghiệm của họ thời kỳ đó sở hữu rất nhiều nét tương đồng với thiết kế của dòng xe tải điện Tesla Semi ra mắt vào năm 2017 sau này.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022310.webp)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022311.webp)

## 言论

1.

Vườn ươm startup lớn nhất nước Mỹ Y Combinator (YC) hiện nay hầu như chỉ tập trung rót vốn cho các dự án liên quan đến AI. Trong danh mục đầu tư mới nhất của họ, tỷ lệ các doanh nghiệp hoạt động trên nền tảng AI chiếm tới 88%.

Định hướng đầu tư này hoàn toàn đi ngược lại với triết lý khuyến khích tư duy ngược (contrarian thinking) mà YC luôn tự hào trước đây, và đang biến tổ chức thành một đơn vị chạy theo đám đông an toàn.

-- Trích bài viết châm biếm [《Có phải YC hiện nay là nơi dung túng cho những kẻ hèn nhát?》](https://stanfordreview.org/is-yc-for-cowards/)

2.

Chúng ta cần có những chính sách hỗ trợ để các cửa hàng bán lẻ truyền thống (brick-and-mortar stores) có cơ hội sống sót. Sự xuất hiện của một cửa hàng truyền thống mang lại nhiều giá trị vô hình cho cộng đồng xung quanh: giúp thu hút cư dân và khách hàng tiềm năng đến khu phố, từ đó kiến tạo sức sống và tăng mức độ đáng sống cho cả khu vực.

-- Trích bài viết [《Ngành bán lẻ giúp nâng cao giá trị bất động sản khu phố thế nào》](https://worksinprogress.co/issue/fixing-retail-with-land-value-capture/)

3.

Nếu công nghệ AI chiếm vị trí chủ đạo trong mọi hoạt động xã hội, những giá trị nhân văn mà AI không thể số hóa hay định lượng được sẽ không thể duy trì vị thế độc bản của mình, mà cuối cùng sẽ bị đào thải khỏi xã hội.

-- Ben Thompson – nhà phân tích công nghệ Mỹ nổi tiếng chia sẻ quan điểm

4.

Một điểm rất đáng nể ở các doanh nghiệp Mỹ là họ không bao giờ lãng phí thời gian và nguồn lực cho những mảng việc mà bản thân không có thế mạnh, ngược lại họ sẽ dồn toàn bộ nguồn lực đầu tư gấp đôi cho những lĩnh vực cốt lõi mà họ làm tốt nhất.

Mục tiêu cốt lõi của họ luôn hướng tới việc tối đa hóa lợi nhuận đầu ra chứ không đơn thuần chỉ là tìm cách tối thiểu hóa chi phí đầu vào.

-- Ben Thompson – nhà phân tích công nghệ Mỹ nổi tiếng chia sẻ quan điểm

5.

Năng lực sáng tạo đòi hỏi con người phải có đủ dũng khí để từ bỏ những cảm giác an toàn của sự chắc chắn sẵn có.

-- Erich Fromm – nhà triết học lỗi lạc người Đức chia sẻ chiêm nghiệm

## 往年回顾

[Tìm hiểu về bản chất của Token kỹ thuật số](https://www.ruanyifeng.com/blog/2025/02/weekly-issue-339.html) (#339)

[Nguồn gốc sâu xa của sự khoan dung trong xã hội](https://www.ruanyifeng.com/blog/2024/02/weekly-issue-289.html) (#289)

[Hai nhóm nhân sự sẽ gia tăng mạnh mẽ trong tương lai](https://www.ruanyifeng.com/blog/2023/01/weekly-issue-239.html) (#239)

[Dự báo về ngành công nghiệp tiếp theo sẽ đối mặt với sự cạnh tranh khốc liệt](https://www.ruanyifeng.com/blog/2021/12/weekly-issue-189.html) (#189)

(Hết)
