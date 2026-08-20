# Bản tin chia sẻ công nghệ (Số 373): Mô hình dữ liệu chính là cốt lõi của sản phẩm mới

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/8003) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111108.webp)

Khu di tích lịch sử trạm dịch Huyền Tuyền Trí ở thành phố Tửu Tuyền, tỉnh Cam Túc vừa khai trương đón khách tham quan từ năm nay. Đây vốn là một trạm dịch phục vụ du khách nghỉ chân trên con đường tơ lụa cổ đại thời nhà Hán. Trong số hơn 80.000 thẻ tre, thẻ gỗ thời Hán được tìm thấy tại Trung Quốc, có tới hơn 30.000 thẻ được phát hiện ngay tại trạm dịch này. ([via](https://www.news.cn/culture/20250430/2dfefaf471ca46f48e70d1ab669ef6e9/c.html?page=5))

## 数据模型是新产品的核心

（1）

Nhà khoa học máy tính lỗi lạc, cha đẻ của ngôn ngữ lập trình Pascal – [Niklaus Wirth](https://en.wikipedia.org/wiki/Niklaus_Wirth) từng đưa ra một luận điểm kinh điển:

> Thuật toán + Cấu trúc dữ liệu = Chương trình (Algorithms + Data Structures = Programs)

Ông thậm chí đã xuất bản một cuốn sách chuyên ngành lấy chính câu nói này làm tựa đề.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110804.webp)

Theo quan điểm của ông, **cấu trúc dữ liệu cũng quan trọng tương đương với thuật toán**, và là những thành phần cốt lõi nhất của chương trình, trong khi ngôn ngữ lập trình chỉ đóng vai trò thứ yếu.

Nếu thiết kế cấu trúc dữ liệu sai, chương trình trước sau gì cũng sẽ phát sinh lỗi; ngược lại, nếu cấu trúc dữ liệu được thiết kế chuẩn xác, phương án giải quyết bài toán thường sẽ tự động hiển lộ một cách dễ dàng.

（2）

Gần đây tôi có đọc [một bài viết](https://notes.mtb.xyz/p/your-data-model-is-your-destiny) chia sẻ cùng quan điểm này, thậm chí tác giả còn nâng tầm luận điểm lên khi cho rằng: **Mô hình dữ liệu (data model) không chỉ là cốt lõi của chương trình, mà còn là cốt lõi của một sản phẩm mới**.

Tác giả lập luận rằng cấu trúc dữ liệu sẽ định hình hình thái của sản phẩm. Chỉ cần thay đổi nhẹ mô hình dữ liệu bên dưới, bạn hoàn toàn có thể kiến tạo nên một dòng sản phẩm hoàn toàn mới.

Bài viết chia sẻ nhiều ví dụ thực tế vô cùng gợi mở mà tôi muốn giới thiệu lại với các bạn.

（3）

Thuở sơ khai, các phần mềm trò chuyện (chat) truyền thống đều được thiết kế lấy con người làm trung tâm: hai hoặc nhiều người kết nối với nhau để tạo thành một cuộc hội thoại.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110807.webp)

Mô hình dữ liệu của hệ thống xoay quanh thực thể con người. Nếu tất cả thành viên thoát ra khỏi nhóm, cuộc hội thoại đó cũng sẽ chính thức khép lại.

Về sau, ứng dụng chat nhóm thế hệ mới [Slack](https://slack.com/intl/zh-cn/) ra đời và thay đổi cuộc chơi.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110805.webp)

Mô hình dữ liệu của Slack đã thay đổi: cốt lõi của hệ thống không phải là con người, mà là chủ đề thảo luận. Mỗi chủ đề đóng vai trò như một chiếc hộp chứa tất cả các nội dung trò chuyện liên quan, gọi là kênh (channel).

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110806.webp)

Ngay cả khi tất cả thành viên rời khỏi kênh và không còn ai trò chuyện, kênh đó vẫn tiếp tục tồn tại, và toàn bộ ngữ cảnh lịch sử thảo luận của chủ đề không hề bị mất đi. Khi một thành viên mới gia nhập kênh sau này, họ vẫn có thể dễ dàng đọc lại toàn bộ lịch sử thảo luận trước đó.

Nhờ đặc tính ưu việt này, Slack đã nhanh chóng chinh phục thị trường doanh nghiệp và trở thành lựa chọn hàng đầu cho các hệ thống trò chuyện và cộng tác nội bộ hiện nay.

Có thể thấy, chỉ bằng việc thay đổi mô hình dữ liệu, ngay cả khi các tính năng chat cơ bản giữ nguyên, Slack đã biến đổi thành một sản phẩm hoàn toàn khác biệt, vượt qua các đối thủ cạnh tranh để thống trị phân khúc doanh nghiệp.

（4）

Hãy cùng nhìn thêm hai ví dụ tương tự khác: Notion và Google Docs đều là các phần mềm soạn thảo tài liệu, nhưng mô hình dữ liệu bên dưới của chúng lại hoàn toàn khác nhau.

Google Docs áp dụng mô hình truyền thống, lấy từng tài liệu đơn lẻ làm trung tâm để quản lý.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110808.webp)

Trong khi đó, cốt lõi của mô hình Notion không phải là tài liệu mà là trang (page). Mỗi trang đóng vai trò như một không gian chứa cho phép bạn lồng ghép, tổ chức nhiều tài liệu khác nhau để hiển thị cùng một nơi.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110809.webp)

Tương tự đối với Figma và Photoshop trong mảng phần mềm thiết kế đồ họa:

Trọng tâm mô hình của Photoshop là bức ảnh/hình ảnh đơn lẻ, mọi thao tác chỉnh sửa đều phải quy về và nằm trong phạm vi bức ảnh đó.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110810.webp)

Còn đối với Figma, cốt lõi của mô hình chính là không gian làm việc (workspace). Mỗi dự án thiết kế là một không gian làm việc chung, trong đó chứa nhiều hình ảnh, thiết kế khác nhau và hỗ trợ nhiều người cùng tham gia thao tác, để lại bình luận tương tác trực tiếp.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110811.webp)

（5）

Tóm lại, chỉ một thay đổi nhỏ trong thiết kế mô hình dữ liệu có thể khai sinh ra một sản phẩm hoàn toàn mới, tạo ra sự khác biệt độc đáo so với các giải pháp sẵn có trên thị trường và mở ra những cơ hội kinh doanh mới.

Đây là một gợi ý tuyệt vời cho chúng ta: nếu sản phẩm của bạn đang gặp tình trạng bão hòa hoặc tương đồng với các đối thủ, hãy thử suy nghĩ xem liệu có thể thay đổi thiết kế mô hình dữ liệu bên dưới hay không.

## 科技动态

1. Nước Úc hiện đã lắp đặt một khối lượng khổng lồ các tấm pin năng lượng mặt trời, dẫn đến một rắc rối hoàn toàn mới.

Đó là lượng điện phát ra quá nhiều vào ban ngày và không thể tiêu thụ hết. Chính phủ nước này đang lên kế hoạch triển khai chương trình miễn phí tiền điện vào buổi trưa – thời điểm bức xạ mặt trời mạnh nhất trong ngày.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110902.webp)

Chính phủ yêu cầu các công ty điện lực phải cung cấp ít nhất 3 giờ sử dụng điện miễn phí mỗi ngày cho người dân. Nếu người dân tự trang bị hệ thống pin lưu trữ điện năng, họ thậm chí có thể sử dụng điện miễn phí cả ngày.

Cùng với sự phát triển của năng lượng mặt trời, nhân loại đang đứng trước cơ hội bước vào kỷ nguyên giá điện cực rẻ hoặc thậm chí bằng không (ít nhất là vào ban ngày).

2. Gần đây, tại các ga tàu điện ngầm ở thành phố New York xuất hiện đồng loạt một loại quảng cáo AI độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101402.webp)

Đó là một thiết bị AI đeo cổ dạng mặt dây chuyền (AI pendant), cho phép người đeo trò chuyện trực tiếp với nó, sản phẩm có giá bán 129 USD.

Biển quảng cáo cho sản phẩm này xuất hiện ở khắp mọi nơi: từ các bức tường, thân tàu cho đến bên trong các toa tàu điện ngầm.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101403.webp)

CEO của công ty chia sẻ khi biết chi phí thuê trọn gói quảng cáo tại hệ thống tàu điện ngầm New York chỉ tốn chưa đầy 1 triệu USD mỗi tháng, anh thấy mức giá này quá rẻ nên đã quyết định chi tiền ngay lập tức.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111305.webp)

Tuy nhiên, sau hơn một tháng chạy quảng cáo rầm rộ, sản phẩm mới chỉ bán ra được 3.100 chiếc, thu về tổng doanh thu chưa đầy 400.000 USD. Đây rõ ràng là một thương vụ đầu tư lỗ nặng.

Mặc dù vậy, vị CEO vẫn tỏ ra rất lạc quan và tin tưởng rằng doanh số sẽ tăng trưởng nhanh chóng sau khi sản phẩm được đưa lên kệ tại chuỗi siêu thị Walmart. Anh tin người dùng sẽ cần đến chiếc mặt đeo cổ này như một người bạn đồng hành AI giúp "nâng cao trí tuệ cảm xúc (EQ) và định nghĩa lại khái niệm bạn bè". Để hiện thực hóa mục tiêu này, anh thậm chí đang chuẩn bị chi thêm các khoản ngân sách khổng lồ để chạy quảng cáo tại Los Angeles và Chicago.

Đây là thực trạng chung của các thiết bị phần cứng và ứng dụng AI hiện nay: doanh số bán ra thực tế rất khiêm tốn nhưng lại cần những khoản chi phí tiếp thị và quảng cáo khổng lồ, và các công ty AI vẫn sẵn sàng đốt tiền không chút phàn nàn.

3. Thiết bị "dù bắt gió" (wind-catching umbrella) khổng lồ nhất thế giới vừa thực hiện thành công thử nghiệm bung dù và thu dù tại bãi thử nghiệm kỳ thuộc minh Alxa Tả, khu tự trị Nội Mông.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111211.webp)

Diện tích bao phủ của chiếc dù khi bung ra đạt tới 5.000 mét vuông, được thiết kế để thu giữ năng lượng gió ở tầng cao phục vụ phát điện.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111212.webp)

Gió mạnh chủ yếu tập trung ở tầng khí quyển trên cao. Các nhà khoa học đã sớm phát triển mô hình dù bắt gió hoạt động tương tự như một chiếc diều khổng lồ được thả lên độ cao trên 300 mét để đón gió, sau đó truyền động năng thông qua dây cáp kéo để làm quay máy phát điện ở mặt đất.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111213.webp)

4. Bản cập nhật hệ điều hành visionOS mới nhất dành cho kính thực tế ảo Apple Vision Pro vừa bổ sung tính năng tạo "Avatar không gian" (Spatial Persona).

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110508.webp)

Tính năng này sử dụng hệ thống camera bên trong kính để quét và ghi hình khuôn mặt người dùng, sau đó áp dụng thuật toán Gaussian Splatting để chuyển đổi hình ảnh chân dung 2D thông thường thành một avatar 3D không gian sống động như thật.

Khi thực hiện cuộc gọi, người dùng sẽ thấy hình ảnh avatar 3D của đối phương hiển thị lơ lửng ngay trong không gian thực trước mắt và tương tác thời gian thực theo từng biểu cảm, cử chỉ của họ. Điều kiện là cả hai bên tham gia cuộc gọi đều phải đeo kính Vision Pro.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110509.webp)

Tính năng hỗ trợ kết nối đồng thời lên tới 5 người trong một cuộc gọi không gian.

Trải nghiệm này mở ra nhiều hứa hẹn thú vị: nếu trong tương lai hệ thống hỗ trợ dựng thêm cả phần cơ thể ảo thì người dùng hoàn toàn có thể nhìn thấy các chuyển động cơ thể của nhau trực quan trong không gian.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110510.webp)

## 文章

1. [Lời kêu cứu của một lập trình viên người Iran](https://gist.github.com/EchenD/8b211ebfa4941d2c5df7b526790b31aa#the-current-situation-being-completely-honest) (tiếng Anh)

Một lập trình viên tại Iran đã phát triển một công cụ sinh avatar ảo bằng AI rất chất lượng, nhưng phát hiện ra rằng dưới lệnh cấm vận của Mỹ, anh không có cách nào bán được sản phẩm ra thị trường quốc tế, nên đã đăng bài kêu cứu trên GitHub:

> Tôi không có khách hàng, không có doanh thu, toàn bộ số tiền tiết kiệm tích lũy đã cạn kiệt, và tôi đã tích cực tìm kiếm việc làm trong suốt 9 tháng qua nhưng vẫn hoàn toàn bế tắc. Vợ tôi là một y tá, cô ấy phải làm việc vất vả từ 5 giờ sáng đến 7 giờ tối hàng ngày, còn tôi thì chỉ biết ngồi trước máy tính phát triển những thứ thậm chí không đủ trả tiền thuê nhà.
> 
> Sống tại Iran, tôi không được phép đăng ký và sử dụng các cổng thanh toán phương Tây như Stripe hay PayPal, cũng không thể sử dụng các dịch vụ đám mây lớn như AWS, GCP hay Azure. Tôi không có tài khoản ngân hàng quốc tế để nhận tiền và cũng không thể chấp nhận thanh toán qua thẻ tín dụng của khách hàng nước ngoài.

2. [Tôi ghét việc gửi ảnh chụp màn hình chứa mã nguồn](https://parkscomputing.com/page/i-hate-screenshots-of-text) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111201.webp)

Một lập trình viên nước ngoài đã lên tiếng kêu gọi khách hàng và đồng nghiệp đừng gửi ảnh chụp màn hình chứa code khi gặp sự cố nữa. Bởi việc này bắt anh phải gõ lại thủ công từng dòng code để debug thay vì copy nhanh từ liên kết dẫn tới dòng mã nguồn đó.

3. [Hình ảnh có giúp tiết kiệm số lượng Token hơn văn bản không?](https://pagewatch.ai/blog/post/llm-text-as-image-tokens/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110802.webp)

Bài viết tiến hành thử nghiệm thực tế xem việc chuyển đổi nội dung prompt từ dạng văn bản thông thường sang định dạng hình ảnh có giúp tiết kiệm chi phí Token khi gọi API của các mô hình LLM hay không.

Kết quả cho thấy bản thân hình ảnh đầu vào giúp tiết kiệm Token cho prompt, tuy nhiên mô hình AI lại cần tiêu tốn nhiều Token đầu ra hơn để giải nghĩa ngữ cảnh hình ảnh đó, do đó tổng chi phí Token thực tế không hề giảm đi.

4. [Hướng dẫn trực quan chi tiết về thuật toán Dijkstra](https://github.com/trekhleb/javascript-algorithms/blob/master/src/algorithms/graph/dijkstra/README.zh-CN.md) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111207.webp)

Dijkstra là thuật toán kinh điển dùng để tìm đường đi ngắn nhất giữa hai điểm trong đồ thị. Bài viết sử dụng các hình vẽ minh họa từng bước vô cùng trực quan để giải thích nguyên lý hoạt động của thuật toán này.

5. [Trải nghiệm sử dụng thử nghiệm Web Monetization API](https://blog.tomayac.com/2025/11/07/using-the-web-monetization-api-for-fun-and-profit/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110803.webp)

Trình duyệt web hiện có một API thử nghiệm hỗ trợ người dùng quyên góp tiền trực tiếp cho chủ sở hữu trang web. Bài viết chia sẻ trải nghiệm thực tế và đánh giá về tính năng này.

6. [So sánh chi phí sử dụng của các plugin hỗ trợ lập trình bằng AI](https://blog.kilocode.ai/p/testing-augment-codes-new-credit) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111306.webp)

Bài viết tiến hành chạy thử nghiệm các tác vụ lập trình thực tế để so sánh chi phí vận hành giữa hai plugin AI nổi tiếng trên VS Code: [Augment Code](https://www.augmentcode.com) và [Kilo Code](https://kilocode.ai/).

Plugin đầu tiên bắt buộc sử dụng mô hình tích hợp sẵn Claude Sonnet 4.5, trong khi plugin thứ hai cho phép người dùng tự cấu hình khóa API mô hình của riêng mình. Bài viết sẽ phân tích xem phương án nào tối ưu chi phí hơn.

## 工具

1. [MagicMirror²](https://github.com/MagicMirrorOrg/MagicMirror)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110901.webp)

Ứng dụng hiển thị thông tin đa nhiệm trên một bảng điều khiển, thường được dùng để thiết lập màn hình hiển thị thông tin gia đình hoặc tích hợp làm gương thông minh (smart mirror).

2. [btop](https://github.com/aristocratos/btop)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111208.webp)

Phiên bản cải tiến vượt trội của lệnh `htop`, hiển thị trực quan và cực kỳ chi tiết các thông số tài nguyên hệ thống ngay trên giao diện terminal.

3. [DroidDock](https://github.com/rajivm1991/DroidDock)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111206.webp)

Ứng dụng dành cho hệ điều hành macOS hỗ trợ kết nối, quản lý và duyệt tệp tin trên điện thoại Android một cách dễ dàng.

4. [RedisFX](https://github.com/tanhuang2016/RedisFX)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110801.webp)

Giao diện quản trị đồ họa gọn nhẹ dành cho cơ sở dữ liệu Redis, phát triển bằng JavaFX và chạy trên máy ảo JVM. (Đóng góp từ [@tanhuang2016](https://github.com/ruanyf/weekly/issues/8120))

5. [Pingap](https://github.com/vicanso/pingap)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111007.webp)

Máy chủ proxy ngược phát triển bằng Rust có tính năng tương tự Nginx, tích hợp sẵn nhiều plugin hữu ích (xác thực danh tính, bảo mật, giới hạn lưu lượng, thay đổi nội dung phản hồi, v.v.). (Đóng góp từ [@vicanso](https://github.com/ruanyf/weekly/issues/8133))

6. [Alle](https://github.com/bestruirui/Alle)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111008.webp)

Hệ thống quản lý và gom hòm thư mã nguồn mở triển khai trên Cloudflare Workers. Cho phép người dùng đọc toàn bộ thư điện tử từ nhiều tài khoản khác nhau trên một giao diện duy nhất, tích hợp sẵn các trợ lý AI xử lý email. (Đóng góp từ [@bestruirui](https://github.com/ruanyf/weekly/issues/8140))

7. [gocron](https://github.com/gocronx-team/gocron)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111010.webp)

Hệ thống quản lý tác vụ định kỳ (cron jobs) viết bằng ngôn ngữ Go, đi kèm giao diện web trực quan để thay thế cho công cụ crontab mặc định của Linux. (Đóng góp từ [@gocronx](https://github.com/ruanyf/weekly/issues/8143))

8. [markdown-it-ts](https://github.com/Simon-He95/markdown-it-ts)

Thư viện parser phân tích cú pháp Markdown nổi tiếng `markdown-it` được viết lại hoàn toàn bằng TypeScript. (Đóng góp từ [@Simon-He95](https://github.com/ruanyf/weekly/issues/8145))

9. [TUIOS](https://github.com/Gaurav-Gosain/tuios)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111109.webp)

Ứng dụng độc đáo đóng vai trò như một trình quản lý cửa sổ ngay bên trong một cửa sổ terminal duy nhất, giúp người dùng quản lý nhiều phiên làm việc dòng lệnh cùng lúc. (Đóng góp từ [@kero990](https://github.com/ruanyf/weekly/issues/8148))

10. [XMSLEEP](https://github.com/Tosencen/XMSLEEP)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111215.webp)

Ứng dụng phát âm thanh tiếng ồn trắng (white noise) mã nguồn mở dành cho hệ điều hành Android. (Đóng góp từ [@Tosencen](https://github.com/ruanyf/weekly/issues/8157))

## AI 相关

1. [Davia](https://github.com/davialabs/davia)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111203.webp)

Công cụ mã nguồn mở sử dụng mô hình AI để tự động phân tích và chuyển đổi toàn bộ cấu trúc mã nguồn dự án thành một trang tài liệu hướng dẫn trực quan.

2. [VoidMuse](https://github.com/voidmuse-dev/voidmuse)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111009.webp)

Plugin hỗ trợ viết mã nguồn tích hợp AI dành cho IntelliJ IDEA và VS Code, dự án được mở nguồn mở để phục vụ mục đích giảng dạy cơ chế phát triển các công cụ lập trình AI. (Đóng góp từ [@voidmuse-dev](https://github.com/ruanyf/weekly/issues/8142))

3. [UPage](https://github.com/halo-dev/upage)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111012.webp)

Nền tảng kéo thả giao diện trang web trực quan sử dụng các mô hình ngôn ngữ lớn, định vị là giải pháp thay thế mã nguồn mở cho Lovable. (Đóng góp từ [@wan92hen](https://github.com/ruanyf/weekly/issues/8147))

4. [Pair Translate](https://github.com/Cookee24/PairTranslate)

Plugin trình duyệt mã nguồn mở hỗ trợ dịch thuật trang web, cho phép người dùng tự cấu hình kết nối tới các nhà cung cấp dịch vụ dịch thuật hoặc mô hình AI tùy chọn. (Đóng góp từ [@Cookee24](https://github.com/ruanyf/weekly/issues/8155))

5. [DatasetLoom](https://github.com/599yongyang/DatasetLoom)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111216.webp)

Ứng dụng web mã nguồn mở hỗ trợ thu thập, xây dựng và chuẩn hóa dữ liệu huấn luyện cho các mô hình lớn đa phương thức (multimodal LLMs). (Đóng góp từ [@599yongyang](https://github.com/ruanyf/weekly/issues/8156))

6. [Cordys CRM](https://github.com/1Panel-dev/CordysCRM)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111011.webp)

Hệ thống quản lý quan hệ khách hàng (CRM) tích hợp trí tuệ nhân tạo (AI CRM) mã nguồn mở. (Đóng góp từ [@maninhill](https://github.com/ruanyf/weekly/issues/8144))

## 资源

1. [stickertop.art](https://stickertop.art/main/)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111204.webp)

Trang web sưu tầm và trưng bày hình ảnh về những chiếc laptop được dán nhiều sticker độc đáo của giới lập trình viên.

2. [Trực quan hóa kiểu dữ liệu TypeScript](https://types.kitlangton.com/)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111301.webp)

Trang web sử dụng các sơ đồ hình họa trực quan để giải thích các khái niệm kiểu dữ liệu phức tạp trong TypeScript.

3. [Tỷ lệ sử dụng tiền mặt của các quốc gia](https://www.voronoiapp.com/economy/Who-Still-Uses-Cash-7090)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111302.webp)

Bảng thống kê tỷ lệ giao dịch bằng tiền mặt của các quốc gia trên thế giới năm 2025, dữ liệu tham khảo hữu ích khi đi du lịch nước ngoài. Tỷ lệ tiêu dùng tiền mặt của Trung Quốc hiện ở mức 10%, thuộc nhóm các quốc gia thấp nhất thế giới.

## 图片

1. [Đề thi đầu vào của Viện Công nghệ Massachusetts (MIT)](https://www.facebook.com/photo/?fbid=1259756362864936&set=a.474859918021255)

Hình dưới đây là phần thi Đại số trong đề thi tuyển sinh đầu vào của MIT vào năm Đồng Trị thứ 8 thời nhà Thanh (năm 1869).

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111210.webp)

2. [Chữ tượng hình Ai Cập cổ đại](https://optional.is/required/2009/12/03/welcome-the-entire-land/)

Một lập trình viên Iceland đã tìm đến các chuyên gia khảo cổ học nhờ dịch câu nói kinh điển "hello world" sang chữ tượng hình Ai Cập cổ đại.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111202.webp)

Do người Ai Cập cổ đại không có khái niệm về "thế giới" (world), câu nói sau khi dịch sát nghĩa sẽ là: "Chào mừng, toàn bộ lục địa".

## 文摘

1. [Quy mô công ty càng lớn, sản phẩm tạo ra càng dễ phức tạp](https://hugo.writizzy.com/being-opinionated/57a0fa35-1afc-4824-8d42-3bce26e94ade)

Các tập đoàn công nghệ lớn thường có xu hướng tạo ra những dòng sản phẩm cồng kềnh và phức tạp, nguyên nhân chủ yếu bắt nguồn từ hai yếu tố sau:

（1）Số lượng nhân sự trong dự án càng đông, sản phẩm càng dễ phức tạp, bởi mỗi cá nhân đều muốn để lại dấu ấn đóng góp của riêng mình.

Quy tắc thăng tiến tại các tập đoàn lớn là bạn sẽ dễ dàng được cất nhắc khi phát triển và đóng góp thành công một tính năng mới nào đó cho hệ thống.

Cho dù tính năng đó có thể dư thừa và nhanh chóng bị bỏ xó sau 10 tháng hoạt động, thì nhà phát triển ra nó vẫn đã nhận được phần thưởng thăng chức, do đó mọi nhân sự đều có xu hướng liên tục đề xuất thêm tính năng mới cho sản phẩm.

（2）Quy mô công ty càng lớn, tệp khách hàng càng đông, đồng nghĩa với việc họ phải đáp ứng vô vàn các yêu cầu tùy biến cụ thể khác nhau.

Đội ngũ bán hàng (sales) sẽ liên tục hối thúc rằng khách hàng lớn A cần tính năng này; trong khi bộ phận hỗ trợ khách hàng (customer support) lại phản ánh rằng nhóm người dùng B đang có nhu cầu kia.

Trừ khi bạn có một tầm nhìn kiến trúc hệ thống đủ sắc bén để kiên quyết từ chối những tính năng đi chệch khỏi triết lý cốt lõi của sản phẩm, nếu không bạn sẽ bị cuốn vào vòng xoáy thêm thắt tính năng theo yêu cầu của số đông.

Trong đời thực, dưới áp lực từ nhiều phòng ban nội bộ, lập trình viên hầu như không có tiếng nói quyết định mà buộc phải tìm cách cân bằng lợi ích và làm hài lòng các cấp quản lý, kết quả là tạo ra những phần mềm có độ phức tạp khổng lồ.

## 言论

1.

Khác với các API truyền thống, việc sử dụng giao thức MCP (Model Context Protocol) làm cổng kết nối mang lại một lợi thế lớn.

Các API truyền thống được coi là một cam kết kỹ thuật của nhà phát triển và không thể tùy ý thay đổi sau khi phát hành để tránh làm gãy ứng dụng gọi nó. Ngược lại, cổng MCP chỉ phục vụ cho việc gọi lệnh của mô hình AI lớn, và mô hình AI sẽ tự động đọc lại tài liệu hướng dẫn sử dụng một cách động sau mỗi lượt gọi, do đó chúng ta có thể thoải mái sửa đổi mã nguồn phía máy chủ MCP bất cứ lúc nào mà không sợ làm gãy hệ thống.

-- [Steve Krouse](https://simonwillison.net/2025/Nov/12/steve-krouse/), lập trình viên người Mỹ

2.

Nếu bạn chỉ ra cho mọi người thấy vấn đề và đồng thời chỉ ra cho họ giải pháp tháo gỡ, mọi người sẽ bị lay động và lập tức bắt tay vào hành động.

-- [Bill Gates](https://www.goodreads.com/quotes/731935-i-believe-that-if-you-show-people-the-problems-and)

3.

Khoảng 25% lớp đá trên bề mặt Trái Đất thuộc nhóm đá cacbonat. Phần lớn lớp đá này được hình thành từ quá trình phân hủy xác của các sinh vật hữu cơ cổ đại. Điều này đồng nghĩa với việc một lượng lớn đá cacbonat trên hành tinh vốn dĩ từng là những cơ thể sống.

-- [《Suy nghĩ của tôi về cái chết》](https://doc.searls.com/2025/10/06/leavings/)

4.

Những người đang tung hô và truyền thông quá mức về lập trình bằng AI liệu có nhận thức được rằng AI chắc chắn sẽ tạo ra một lượng khổng lồ mã nguồn rác và để lại khoản "nợ kỹ thuật về mặt thấu hiểu" (understanding debt)?

-- Độc giả trên diễn đàn Hacker News

5.

Gần đây tôi thường suy ngẫm: nếu trong tương lai AI có thể chuyển đổi ngôn ngữ tự nhiên của chúng ta thành mã nguồn ứng dụng chạy được một cách hoàn hảo, liệu chúng ta có còn cần đến các ngôn ngữ lập trình truyền thống nữa hay không?

-- [《Lập trình độc lập với ngôn ngữ》](https://joaquimrocha.com/2025/08/31/language-agnostic-programming-why-you-may-still-need-code/)

## 往年回顾

[Thế giới không sở hữu nhiều của cải đến thế](https://www.ruanyifeng.com/blog/2024/11/weekly-issue-326.html) (#326)

[Sự suy tàn của ngành công nghiệp nội dung](https://www.ruanyifeng.com/blog/2023/11/weekly-issue-276.html) (#276)

[Google đang gặp phải vấn đề gì?](https://www.ruanyifeng.com/blog/2022/10/weekly-issue-226.html) (#226)

[Tòa án Trung Quốc có công nhận giấy phép GPL không?](https://www.ruanyifeng.com/blog/2021/09/weekly-issue-176.html) (#176)

(Hết)
