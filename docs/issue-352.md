# Bản tin chia sẻ công nghệ (Số 352): Bộ mặt chuẩn mực của một hệ thống theo dõi lỗi (Bug Tracking)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/6965) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060801.webp)

Vào rạng sáng ngày 6 tháng 6 vừa qua, tên lửa đẩy Trường Chinh 6 được phóng đi từ Trung tâm phóng vệ tinh Thái Nguyên đã tạo nên một vệt sáng ấn tượng bay qua bầu trời phía trên khu di tích Tường thành cổ Tây An. (Nguồn: [news.cnwest.com](http://news.cnwest.com/bwyc/a/2025/06/06/23130650.html))

## Bug 追踪系统的正确样子

Chủ đề của tuần trước xoay quanh công cụ [GitHub Issues](https://github.com/features/issues), một giải pháp ghi chú cá nhân vô cùng mạnh mẽ.

Tuy nhiên, vẫn còn những khía cạnh mà tôi chưa kịp đề cập tới. **Xét về mặt nhiệm vụ cốt lõi gốc của nó — làm một hệ thống theo dõi lỗi (Bug Tracking System) — công cụ này thực tế hoạt động không hề hiệu quả**.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060805.webp)

Nếu bạn cố gắng ứng dụng nó để quản lý các lỗi lập trình của dự án, bạn sẽ nhanh chóng phát hiện ra những thiếu sót trong thiết kế khiến quy trình vận hành trở nên rất gượng gạo.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060806.webp)

Hệ thống quản lý lỗi lâu đời nhất vẫn đang hoạt động ổn định và phát triển cho đến ngày nay là [Bugzilla](https://www.bugzilla.org/).

Gần đây, một kỹ sư từng tham gia phát triển Bugzilla thời kỳ đầu đã chia sẻ [một bài viết phân tích](https://www.bozemanpass.com/everythings-a-bug-or-an-issue/) giới thiệu về 4 nguyên tắc thiết kế cốt lõi của Bugzilla.

Tác giả chỉ ra rằng chỉ khi đáp ứng đầy đủ cả 4 tiêu chí này thì một công cụ mới được coi là một hệ thống theo dõi lỗi đạt chuẩn. Phân tích này mang lại cho tôi nhiều chiêm nghiệm thực tế rất giá trị.

**（1）Mọi nhiệm vụ phát triển đều phải được đưa vào danh mục theo dõi lỗi**: Không chỉ dừng lại ở các lỗi mã nguồn (Code Bugs), danh sách cần bao quát cả các đầu việc phát triển tính năng mới, bổ sung tài liệu kỹ thuật còn thiếu, cải thiện các trải nghiệm người dùng chưa tối ưu, giải quyết các vấn đề nghẽn hiệu năng...

Nói cách khác, bản chất của một hệ thống theo dõi lỗi chính là quản lý tác vụ (Task Management) và nó cần được vận hành như một hệ thống quản lý dự án (Project Management) toàn diện.

**（2）Trạng thái của lỗi cần đa dạng, không chỉ giới hạn ở hai nút "Mở" (Open) và "Đóng" (Closed)**:

Quy trình xử lý và phê duyệt lỗi tại các doanh nghiệp công nghệ lớn thường rất phức tạp. Dưới đây là sơ đồ chu trình xử lý lỗi được trích dẫn trực tiếp từ tài liệu kỹ thuật của [Bugzilla Documentation](https://www.bugzilla.org/docs/3.6/en/html/lifecycle.html):

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060807.webp)

Hệ thống theo dõi lỗi bắt buộc phải cung cấp khả năng tùy biến linh hoạt, cho phép thiết lập chi tiết về mức độ ưu tiên (priority), mức độ nghiêm trọng (severity), trạng thái phân bổ nhân sự (assigned), mối quan hệ phụ thuộc chéo giữa các lỗi (dependencies)... để tương thích tốt với quy trình riêng biệt của từng doanh nghiệp.

**（3）Mỗi lỗi chỉ được phân bổ cho một nhân sự chịu trách nhiệm duy nhất**:

Nguyên tắc này giúp phân định rõ ràng trách nhiệm của từng cá nhân, hỗ trợ người quản lý dễ dàng nắm bắt chi tiết từng kỹ sư đang xử lý việc gì, kế hoạch tiếp theo là gì và các kết quả hoàn thành gần nhất. Chi tiết này cũng góp phần nâng cao tinh thần tự chủ và niềm tự hào của kỹ sư đối với phần việc mình phụ trách.

**（4）Hỗ trợ thiết lập các chế độ hiển thị tùy biến (Custom Views)**:

Do các lỗi tồn tại dưới rất nhiều trạng thái khác nhau, hệ thống theo dõi lỗi bắt buộc phải hỗ trợ các bộ lọc hiển thị tùy biến linh hoạt đi kèm công cụ truy vấn dữ liệu mạnh mẽ.

*   *Chế độ hiển thị mặc định của dự án*: Liệt kê toàn bộ các lỗi chưa đóng của phiên bản hiện tại, được sắp xếp thứ tự theo mức độ ưu tiên xử lý.
*   *Chế độ hiển thị cá nhân của kỹ sư*: Chỉ hiển thị các lỗi được phân bổ trực tiếp cho cá nhân họ, cũng được sắp xếp theo mức độ ưu tiên xử lý. Đồng thời, hệ thống cần cho phép người dùng lưu lại cấu hình bộ lọc ưa thích của mình cho các lần truy cập sau.

Đối chiếu 4 tiêu chí chuẩn mực trên với công cụ GitHub Issues, chúng ta thấy một thực tế đáng tiếc là GitHub Issues không đáp ứng tốt bất kỳ một tiêu chí nào:

1.  Tính năng quản lý dự án cực kỳ sơ sài.
2.  Trạng thái tác vụ chỉ có thể phân biệt thủ công qua hệ thống nhãn dán (labels).
3.  Một tác vụ có thể phân bổ vô tội vạ cho nhiều người cùng xử lý.
4.  Giao diện mặc định sắp xếp danh sách theo thời gian khởi tạo và bộ lọc hiển thị chỉ có thể chuyển đổi thô sơ qua nhãn dán.

Ở khía cạnh này, trải nghiệm quản lý lỗi của GitHub thậm chí còn thua kém cả công cụ mã nguồn mở Gitea.

Ví dụ cụ thể là trên GitHub, chúng ta hoàn toàn không có cách nào cấu hình để các lỗi nghiêm trọng nhất (mức ưu tiên P0) tự động hiển thị ở vị trí đầu tiên của danh sách (hình dưới), ngoại trừ việc người quản lý phải thao tác ghim thủ công từng lỗi một lên đầu trang.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060809.webp)

Trong khi đó, Gitea (bao gồm cả nhánh rẽ Forgejo) cung cấp sẵn tính năng cấu hình "[Label Sets](https://docs.gitea.com/administration/customizing-gitea#labels)" rất thông minh, cho phép một nhãn dán chứa nhiều giá trị phân cấp khác nhau và hỗ trợ sắp xếp danh sách tự động theo thứ tự các giá trị này.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060810.webp)

Trong minh họa trên, nhãn dán "Priority" (Mức độ ưu tiên) được cấu hình chứa nhiều mức giá trị phân cấp, và hệ thống cho phép người dùng sắp xếp toàn bộ danh sách lỗi tự động theo thứ tự phân cấp của nhãn này.

## [本周软件] 开源知识库 PandaWiki

Đối với các đội ngũ phát triển nhỏ hoặc cá nhân, làm thế nào để quản lý hiệu quả kho tài liệu đồ sộ và tự xây dựng một hệ thống cơ sở tri thức (Knowledge Base) chuyên nghiệp cho mình?

Tuần này, tôi xin giới thiệu một hệ thống quản lý tri thức mã nguồn mở mới được công bố mang tên [PandaWiki](https://github.com/chaitin/PandaWiki).

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060601.webp)

Hệ thống hoạt động theo mô hình wiki, cho phép người dùng tự do biên soạn và liên kết các trang tài liệu kỹ thuật, rất phù hợp để xây dựng các trang hướng dẫn sử dụng sản phẩm, trang giải đáp thắc mắc FAQ hoặc làm blog cá nhân.

**Điểm nổi bật của PandaWiki là việc tích hợp sẵn các tính năng AI sáng tạo, AI giải đáp và AI tìm kiếm**. Người dùng có thể trực tiếp đối thoại bằng ngôn ngữ tự nhiên với kho tài liệu để tìm kiếm kiến thức, hoặc khai thác các mô hình nhúng (Embedding Models) để tự động quét tìm các tài liệu có nội dung liên quan mật thiết nhất.

Các bạn có thể tham gia trải nghiệm giao diện thực tế tại [Trang Demo](http://47.96.9.75/) của dự án và tham khảo hướng dẫn sử dụng chi tiết tại [Trang tài liệu chính thức](https://pandawiki.docs.baizhi.cloud/).

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060602.webp)

Mã nguồn backend của hệ thống được phát triển trên ngôn ngữ Go mang lại tốc độ phản hồi cực kỳ nhanh nhạy. Quy trình cài đặt vận hành cũng rất tối giản qua Docker chỉ với một dòng lệnh duy nhất.

Dự án hiện đang được chia sẻ công khai tại [Kho mã nguồn GitHub](https://github.com/chaitin/PandaWiki) và đã nhanh chóng nhận được hơn 600 lượt yêu thích (stars) từ cộng đồng.

## 任正非专访

Tuần này, trang nhất của tờ báo chính thống *Nhân dân Nhật báo* đã đăng tải bài viết [phỏng vấn chuyên sâu với ông Nhậm Chính Phi](https://finance.sina.com.cn/roll/2025-06-10/doc-inezpuqu9256330.shtml), người sáng lập tập đoàn công nghệ Huawei.

Dưới đây là một số chia sẻ cốt lõi được trích dẫn:

(1) Về bài toán chip bán dẫn, thực tế chúng ta không cần quá lo lắng hay bi quan. Hiện tại chất lượng chip đơn của chúng ta vẫn đi sau Mỹ khoảng một thế hệ công nghệ. Tuy nhiên chúng ta có thể ứng dụng các giải pháp toán học để bù đắp các hạn chế vật lý, khai thác các công nghệ phi Moore để bù đắp cho Moore, và vận hành hệ thống tính toán cụm (cluster computing) để bù đắp hiệu năng cho chip đơn. Kết quả thực tế hoàn toàn đáp ứng tốt các nhu cầu vận hành thực tiễn.

(2) Mảng phần mềm thực chất là lĩnh vực không thể bị cản trở hay phong tỏa dễ dàng. Bản chất của phần mềm là các ký hiệu toán học, mã nguồn logic và được xây dựng nên bởi các thuật toán và toán tử phức tạp, hoàn toàn không có rào cản vật lý nào ngăn chặn được. Khó khăn thực sự nằm ở việc đổi mới giáo dục và xây dựng được đội ngũ nhân tài kế thừa chất lượng.

(3) Khi quốc gia đã tích lũy được tiềm lực kinh tế nhất định, chúng ta bắt buộc phải dành sự quan tâm lớn cho các nghiên cứu lý thuyết, đặc biệt là nghiên cứu khoa học cơ bản. Thiếu đi nghiên cứu cơ bản, mọi công nghệ phát triển lên đều như cây không rễ. Dù cành lá bên ngoài có vẻ xum xuê, tươi tốt đến đâu thì chỉ cần một cơn gió lớn thổi qua là có thể đổ sụp hoàn toàn.

(4) Xã hội cần thấu hiểu và dành sự hỗ trợ thiết thực cho những người làm công tác nghiên cứu lý thuyết. Các nhà khoa học lý thuyết thường rất cô độc trong hành trình của mình, chúng ta cần kiên nhẫn chiến lược và thấu hiểu họ. Những công thức, ký hiệu toán học và tư duy trừu tượng trong bộ óc của họ thường chỉ có một vài người trên thế giới có khả năng đối thoại chia sẻ được. Chúng ta phải dành sự tôn trọng lớn cho họ, dù bản thân xã hội có thể chưa hiểu hết nội dung văn hóa nghiên cứu đó. Xã hội cần bao dung và quốc gia bắt buộc phải tài trợ kinh phí hoạt động.

(5) Việc mua sắm các thiết bị công nghệ nước ngoài thường có chi phí rất đắt đỏ, bởi giá thành sản phẩm đã bao gồm cả phần chi phí hoàn trả cho các khoản đầu tư nghiên cứu cơ bản trước đó của họ. Dù Việt Nam hay Trung Quốc có tự nghiên cứu cơ bản hay không, chúng ta vẫn phải chi trả khoản tiền này cho thế giới, vậy tại sao chúng ta không đầu tư nguồn kinh phí đó trực tiếp cho các nhà khoa học cơ bản trong nước nghiên cứu?

(6) Hằng năm Huawei chi tới 180 tỷ Nhân dân tệ cho hoạt động nghiên cứu và phát triển (R&D). Trong đó khoảng 60 tỷ Nhân dân tệ được rót trực tiếp cho các nghiên cứu lý thuyết cơ bản và hoàn toàn không áp đặt các chỉ tiêu đánh giá KPIs ngắn hạn. Khoảng 120 tỷ Nhân dân tệ còn lại được đầu tư cho phát triển sản phẩm thương mại và có áp chỉ tiêu nghiệm thu rõ ràng. Không có lý thuyết dẫn đường sẽ không thể có các phát kiến đột phá công nghệ, và chúng ta sẽ mãi đi sau Mỹ.

(7) Trí tuệ nhân tạo (AI) có thể là cuộc cách mạng công nghệ cuối cùng của lịch sử nhân loại, bên cạnh cơ hội về năng lượng phản ứng hạt nhân nhiệt hạch. Để phát triển mạnh mẽ AI bắt buộc phải bảo đảm tốt nguồn năng lượng điện cung cấp. Về khía cạnh này, năng lực phát điện và truyền tải của lưới điện Trung Quốc đang vận hành cực kỳ tốt, đi kèm hạ tầng mạng viễn thông phát triển hàng đầu thế giới, giúp hiện thực hóa tầm nhìn chiến lược điều phối dữ liệu "Đông số Tây toán" (xử lý dữ liệu miền Đông tại các máy chủ miền Tây).

(8) Dù nhận được những lời tán dương hay những lời chỉ trích từ dư luận, chúng ta đều không cần quá để tâm. Điều quan trọng duy nhất là tập trung làm thật tốt phần việc của bản thân mình. Chỉ cần bạn hoàn thiện tốt chính mình thì mọi khó khăn đều sẽ được giải quyết.

## 科技动态

（1）Đại học Khoa học và Công nghệ Trung Quốc đề xuất giải pháp thiết lập cấu trúc "**Pin Hỏa tinh**" (Mars Battery) phục vụ cho các sứ mệnh khám phá vũ trụ tương lai.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060705.webp)

Hệ thống pin này được thiết kế để tích trữ nguồn năng lượng mặt trời thu thập được vào ban ngày trên Sao Hỏa và giải phóng nguồn điện năng phục vụ sinh hoạt cho các thiết bị vào ban đêm.

Cơ chế vận hành của pin dựa trên việc điện phân khí CO2 dồi dào trong bầu khí quyển Sao Hỏa để chuyển hóa thành khí oxy và các nhiên liệu khí như metan, sau đó thực hiện đốt cháy các khí này để phát điện vào ban đêm khi nhiệt độ xuống thấp.

（2）Công ty Công nghệ Ô tô Shenzhen Yinwang (thuộc tập đoàn Huawei) vừa đăng ký thành công bằng sáng chế về thiết kế "**Vô lăng có khả năng thu gọn tiện lợi**".

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061003.webp)

Theo mô tả kỹ thuật, bằng sáng chế cho phép vô lăng điều khiển của xe hơi có thể gấp gọn và thu giấu hoàn toàn vào bên trong bảng điều khiển trung tâm khi xe kích hoạt chế độ tự lái hoàn toàn.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061004.webp)

（3）Thụy Sĩ vừa hoàn thành xây dựng **tòa tháp in 3D cao nhất thế giới** với chiều cao đạt mốc 30 mét, phục vụ mục đích ngắm cảnh cho du khách, với thiết kế ngoại hình mô phỏng theo một loại kẹo truyền thống nổi tiếng của địa phương.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052704.webp)

Để bảo đảm khả năng chịu lực chịu tải an toàn cho tòa tháp cao tầng, đơn vị thi công đã ứng dụng một dòng bê tông chuyên dụng đặc biệt, đồng thời bố trí robot in thứ hai thực hiện việc đặt bổ sung các thanh cốt thép gia cố sau mỗi 20 cm bê tông được in ra.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060104.webp)

（4）Bản cập nhật hệ điều hành macOS mới được Apple công bố tuần này ghi nhận một chỉnh sửa giao diện rất nhỏ nhưng làm xôn xao cộng đồng thiết kế.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061104.webp)

Biểu tượng ứng dụng quản lý tệp tin Finder quen thuộc đã được **lật ngược chiều từ trái sang phải** (hình bên trái là biểu tượng truyền thống lâu năm, hình bên phải là biểu tượng mới). Hiện tại phía Apple vẫn chưa đưa ra lời giải thích chính thức nào về lý do thực hiện cú lật ngược lịch sử này.

## 文章

1、[Tổng kết toàn cảnh về sự phát triển của các mô hình ngôn ngữ lớn LLM trong nửa năm qua](https://simonwillison.net/2025/Jun/6/six-months-in-llms/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060804.webp)

Nhà phát triển Simon Willison chia sẻ bài viết tổng hợp chi tiết các sự kiện và bước tiến công nghệ nổi bật của mảng AI trong nửa năm qua, rất thích hợp để làm tư liệu tham khảo lịch sử.

Tốc độ tiến hóa của AI hiện nay diễn ra nhanh đến mức kinh ngạc, các mô hình ngôn ngữ được coi là đỉnh cao công nghệ vào thời điểm cuối năm ngoái giờ đây đã nhanh chóng bị xếp vào nhóm công nghệ thế hệ cũ.

2、[Chia sẻ trải nghiệm thực tế sau khi nâng cấp sử dụng dịch vụ Claude Code Max](https://steipete.me/posts/2025/claude-code-is-my-computer) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060405.webp)

Tác giả chia sẻ đánh giá chi tiết sau khi chi trả mức phí 200 USD/tháng để trải nghiệm gói dịch vụ cao cấp Claude Code Max, đưa ra nhận xét công cụ này hoàn toàn xứng đáng với từng đồng chi phí bỏ ra nhờ năng lực hỗ trợ lập trình vượt trội.

3、[Hướng dẫn trực quan sinh động về các giải pháp giới hạn tần suất truy cập (Rate Limiting)](https://blog.sagyamthapa.com.np/interactive-guide-to-rate-limiting) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060701.webp)

Làm thế nào để thiết lập giới hạn tần suất truy cập hiệu quả cho hệ thống API? Bài viết giới thiệu chi tiết nguyên lý vận hành của 4 thuật toán thông dụng nhất hiện nay: Token Bucket, Leaky Bucket, Fixed Window và Sliding Window.

4、[Tìm hiểu cấu trúc mạng riêng ảo Amazon VPC qua hình vẽ minh họa](https://www.ducktyped.org/p/why-is-it-called-a-cloud-if-its-not) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060903.webp)

Bài viết sử dụng các hình vẽ thiết kế trực quan dễ hiểu để giải thích bản chất kỹ thuật của khái niệm mạng riêng ảo (VPC - Virtual Private Cloud) trên hạ tầng máy chủ đám mây của Amazon.

5、[Giới thiệu 5 dịch vụ quản lý dấu trang (Bookmarks) tự lưu trữ mã nguồn mở chất lượng](https://www.xda-developers.com/replacements-for-pocket-that-are-self-hosted/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061002.webp)

Tổng hợp và đánh giá nhanh 5 dự án phần mềm mã nguồn mở cho phép người dùng tự dựng máy chủ cá nhân để lưu trữ và quản lý các liên kết trang web yêu thích thay thế cho dịch vụ Pocket.

6、[Trải nghiệm thực tế về cuộc sống cắm trại tự do tại bờ biển Hồng Kông](https://corentin.trebaol.com/Blog/8.+The+Homelessness+Experiment) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060802.webp)

Câu chuyện trải nghiệm thú vị của một sinh viên nước ngoài học tập tại Hồng Kông vào năm 2016. Do nguồn học bổng hạn chế không đủ chi trả chi phí thuê nhà đắt đỏ, anh đã quyết định dựng帐篷 (lều) sinh sống tự do ngay tại khu vực bờ biển suốt học kỳ. Bài viết ghi lại những kỷ niệm và bài học cuộc sống đáng quý từ trải nghiệm độc đáo này.

## 工具

1、[Cap.js](https://github.com/tiagorangel1/cap)

Công cụ nhận diện robot truy cập trang web mã nguồn mở được phát triển như một giải pháp thay thế cho CAPTCHA truyền thống, vận hành dựa trên cơ chế thuật toán chứng minh công việc (Proof-of-Work) SHA-256 chạy trên trình duyệt máy khách.

2、[Quartz](https://github.com/jackyzha0/quartz)

Bộ công cụ hỗ trợ người dùng chuyển đổi kho ghi chú Markdown cá nhân thành trang web tĩnh (static website) đẹp mắt và nhanh chóng, được đánh giá là giải pháp thay thế tự chủ hoàn hảo cho dịch vụ trả phí Obsidian Publish.

3、[somo](https://github.com/theopfr/somo)

Công cụ dòng lệnh gọn nhẹ dành cho hệ điều hành Linux hỗ trợ kỹ sư nhanh chóng kiểm tra và phát hiện chi tiết các tiến trình đang chiếm dụng các cổng kết nối mạng (ports).

4、[OOMOL Studio](https://github.com/ruanyf/weekly/issues/7029)

Môi trường phát triển tích hợp (IDE) máy tính độc đáo, cho phép lập trình viên đóng gói các hàm xử lý cá nhân thành các nút trực quan (nodes), sau đó sử dụng giao diện kéo thả để liên kết các nút này thành một quy trình làm việc tự động (workflows). (Đóng góp từ [@BlackHole1](https://github.com/ruanyf/weekly/issues/7029))

5、[Cực Trắc (极测)](https://www.jicesys.com/)

Bộ công cụ hỗ trợ kiểm thử giao tiếp mạng miễn phí, cho phép kỹ sư dễ dàng mô phỏng và gửi nhận các gói tin thử nghiệm trên nhiều giao thức phổ biến như UDP, TCP, Serial Port, WebSocket, ZeroMQ... (Đóng góp từ [@seasonlaw](https://github.com/ruanyf/weekly/issues/7032))

6、[container](https://github.com/apple/container)

Công cụ dòng lệnh chính thức do Apple phát hành hỗ trợ người dùng macOS khởi chạy trực tiếp các container Linux gốc mà hoàn toàn không bắt buộc phải cài đặt ứng dụng Docker Desktop cồng kềnh.

7、[DarkFlare](https://github.com/doxx/darkflare)

Công cụ dòng lệnh độc đáo giúp bảo mật thông tin bằng cách mã hóa và ngụy trang toàn bộ các luồng dữ liệu truyền nhận dạng TCP thành các gói tin HTTPS thông dụng khi đi qua mạng CDN.

8、[JDownloader](https://jdownloader.org/)

Trình quản lý tải tệp tin đa nền tảng mã nguồn mở mạnh mẽ. Tham khảo thêm [bài hướng dẫn chi tiết](https://www.xda-developers.com/raspberry-pi-downloading-device-entire-network/) để biến chiếc máy tính nhúng Raspberry Pi thành một máy chủ tải tệp tự động hoạt động 24/7 cho cả gia đình.

9、[Pydoll](https://github.com/autoscrape-labs/pydoll)

Thư viện Python chuyên dụng hỗ trợ lập trình điều khiển tự động trình duyệt Chrome thông qua giao thức Chrome DevTools Protocol trực tiếp trên máy tính cục bộ.

10、[Chili3D](https://github.com/xiangechen/chili3d)

Dự án phần mềm hỗ trợ vẽ kỹ thuật thiết kế 3D CAD hoạt động mượt mà ngay trên giao diện trình duyệt web được chia sẻ mã nguồn mở hoàn toàn.

## AI 相关

1、[Page Magic](https://github.com/khaledh/pagemagic)

Tiện ích mở rộng AI dành cho trình duyệt Chrome: Người dùng chỉ cần nhập mô tả yêu cầu chỉnh sửa giao diện trang web bằng ngôn ngữ tự nhiên, công cụ sẽ tự động chỉnh sửa trực tiếp mã nguồn HTML/CSS để hiển thị kết quả thay đổi ngay trên màn hình (yêu cầu kết nối khóa API của Anthropic).

2、[Bích Hưởng (壁响 - WallEcho)](https://wallecho.com/)

Dịch vụ trực tuyến miễn phí ứng dụng AI hỗ trợ người dùng nhanh chóng sinh và tải về các hình ảnh hình nền (wallpapers) nghệ thuật chất lượng cao cho điện thoại và máy tính dựa trên mô tả văn bản đầu vào. (Đóng góp từ [@twjiem](https://github.com/ruanyf/weekly/issues/6999))

3、[AI Động Sát Nhật Báo (AI 洞察日报)](https://github.com/justlovemaki/CloudFlare-AI-Insight-Daily)

Dự án mã nguồn mở xây dựng hệ thống tự động quét và thu thập thông tin công nghệ từ các nguồn chỉ định thông qua dịch vụ Cloudflare Workers, tự động biên tập và xuất bản bản tin AI tổng hợp hằng ngày. Tham khảo [giao diện hiển thị mẫu](https://justlovemaki.github.io/CloudFlare-AI-Insight-Daily/today/book/). (Đóng góp từ [@justlovemaki](https://github.com/ruanyf/weekly/issues/7009))

4、[zenfeed](https://github.com/glidea/zenfeed)

Trợ lý thông tin thông minh ứng dụng AI để tự động theo dõi, thu thập lọc và tóm tắt nội dung cốt lõi của các bài viết tin tức thuộc các chủ đề quan tâm của người dùng từ các nguồn RSS. (Đóng góp từ [@glidea](https://github.com/ruanyf/weekly/issues/7012))

5、[Văn Nhan MCP Server (文颜 MCP Server)](https://github.com/caol64/wenyan-mcp)

Dự án xây dựng cổng kết nối giao thức MCP hỗ trợ các mô hình AI tự động định dạng bố cục thẩm mỹ bài viết và thực hiện đăng tải trực tiếp lên các kênh truyền thông chính thức của WeChat. Xem thêm [bài viết giới thiệu chi tiết](https://babyno.top/posts/2025/06/let-ai-help-you-manage-your-gzh-layout-and-publishing/). (Đóng góp từ [@caol64](https://github.com/ruanyf/weekly/issues/7048))

## 资源

1、[Danh sách toàn thư hơn 3.000 trường đại học và học viện tại Trung Quốc](https://laosheng.top/fuwu/yuanxiao)

Trang web tổng hợp và cung cấp đầy đủ liên kết trang chủ chính thức của toàn bộ các cơ sở giáo dục đại học tại Trung Quốc. (Đóng góp từ [@DiamonWoo](https://github.com/ruanyf/weekly/issues/7047))

2、[Mullvad Leta](https://leta.mullvad.net/)

Dịch vụ công cụ tìm kiếm trực tuyến được công bố bởi hãng bảo mật Mullvad. Công cụ tiến hành thu thập kết quả tìm kiếm từ Google và Brave, đồng thời lọc sạch toàn bộ các thông tin định danh thiết bị của người dùng để bảo vệ quyền riêng tư tuyệt đối khi tìm kiếm.

Trải nghiệm thực tế cho thấy tốc độ truy vấn của công cụ rất nhanh nhạy và hoàn toàn sạch bóng các quảng cáo thương mại gây phiền nhiễu.

3、[DNS4EU](https://www.joindns4.eu/)

Dịch vụ máy chủ phân giải tên miền công cộng (Public DNS) chính thức được Liên minh Châu Âu công bố, tích hợp sẵn các tính năng lọc quảng cáo và chặn các trang web lừa đảo độc hại.

## 图片

1、[Mức phóng xạ tồn dư trên tay nắm cửa tại ngôi nhà cũ của nhà bác học Marie Curie](https://www.bbc.com/future/article/20250605-the-hunt-for-marie-curies-radioactive-fingerprints-in-paris)

Nhà vật lý học lỗi lạc Marie Curie do đặc thù công việc nghiên cứu tiếp xúc liên tục với các nguyên tố phóng xạ trong thời gian dài khiến các hạt bụi phóng xạ radium siêu nhỏ bám dính sâu vào da tay.

Tại ngôi nhà cũ của bà ở thủ đô Paris (Pháp), dù đã trôi qua gần một thế kỷ, các thiết bị đo chuyên dụng ngày nay vẫn dễ dàng phát hiện mức độ phóng xạ nhẹ tồn dư ngay trên tay nắm cửa ra vào.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061106.webp)

Vào năm 1934, bà đã qua đời do chứng thiếu máu suy tủy nghiêm trọng — hệ quả trực tiếp của việc cơ thể bị phơi nhiễm phóng xạ quá liều lượng an toàn trong quá trình nghiên cứu khoa học.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025061107.webp)

2、[Hệ thống bãi đỗ xe ngầm khổng lồ trong lòng hang đá](https://www.hagerty.com/media/automotive-history/since-the-60s-ford-has-stored-cars-underground-in-a-kansas-city-cave/)

Tại bang Missouri (Mỹ) vốn có hoạt động khai thác đá vôi nhộn nhịp từ thế kỷ trước, để lại hệ thống các khoảng không gian hang động ngầm khổng lồ bên dưới lòng đất sau khi dừng khai thác.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024111103.webp)

Các hang động ngầm này đã bị bỏ hoang trong thời gian dài cho đến khi tập đoàn sản xuất xe hơi Ford quyết định thuê lại toàn bộ không gian này vào thập niên 1950.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024111104.webp)

Không gian hang động ngầm sở hữu ưu thế lớn về mặt diện tích chứa khi có thể đỗ cùng lúc hơn 5.000 chiếc xe hơi mới sản xuất, bảo đảm xe hoàn toàn tránh được các tác động thời tiết khắc nghiệt như mưa bão hay tuyết rơi, đồng thời độ ẩm khô ráo và nhiệt độ mát mẻ luôn duy trì ổn định quanh năm.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024111105.webp)

Hệ thống bãi đỗ xe ngầm độc đáo này vẫn tiếp tục được vận hành hiệu quả cho đến ngày nay, được ghi nhận là một trong những hạ tầng thương mại ngầm có quy mô lớn nhất lịch sử nhân loại.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024111106.webp)

## 文摘

1、[Xu thế chuyển dịch định nghĩa về khái niệm "Mô hình ngôn ngữ nhỏ" (SLMs)](https://jigsawstack.com/blog/what-even-is-a-small-language-model-now--ai)

Trong giai đoạn sơ khai của công nghệ học máy, thuật ngữ "Mô hình nhỏ" (Small Models) thường được dùng để chỉ các cấu trúc mạng thần kinh cơ bản có khả năng chạy trực tiếp trên bộ xử lý CPU của máy tính gia đình thông thường.

Đến mốc thời gian năm 2018, nếu bạn đặt câu hỏi về định nghĩa mô hình nhỏ, câu trả lời nhận được thường là các mô hình xử lý có quy mô chỉ khoảng vài triệu tham số có khả năng vận hành trơn tru trên các bo mạch Raspberry Pi hoặc trên điện thoại di động.

Tuy nhiên, sự bùng nổ của cấu trúc Transformer và các mô hình ngôn ngữ lớn (LLMs) sau đó đã nhanh chóng làm thay đổi hoàn toàn định nghĩa này khi quy mô tham số của các mô hình liên tục phình to ra.

Ngày nay, bất kỳ mô hình AI nào có khả năng vận hành độc lập mà hoàn toàn không đòi hỏi phải kết nối vào các cụm siêu máy chủ card đồ họa A100 chuyên dụng của các tập đoàn công nghệ đều có thể được xếp vào danh mục mô hình nhỏ.

Giờ đây giới công nghệ gọi các mô hình có quy mô 30 tỷ tham số (30B) là mô hình nhỏ, bởi chúng có khả năng chạy mượt mà chỉ với tài nguyên của một chiếc card đồ họa đơn lẻ.

Định nghĩa về mô hình nhỏ hiện nay tập trung nhiều vào năng lực triển khai độc lập (deployability) của mô hình thay vì chỉ đo đạc thô sơ dựa trên số lượng tham số bên trong.

Chỉ cần một mô hình có khả năng cài đặt chạy cục bộ trên thiết bị cá nhân của người dùng cuối, nó sẽ được coi là mô hình nhỏ. Chúng ta có thể chia chúng làm hai nhóm cụ thể:

*   *Nhóm 1*: Các mô hình siêu nhỏ có khả năng chạy trực tiếp trên thiết bị di động hoặc phần cứng nhúng biên phục vụ cho các tác vụ trợ lý giọng nói offline, dịch thuật nhanh không cần mạng, tóm tắt văn bản cục bộ hay chatbot nhúng.
*   *Nhóm 2*: Các mô hình có quy mô lớn hơn từ 30B đến 70B tham số nhưng có thể vận hành ổn định trên tài nguyên của một chiếc card đồ họa đơn lẻ (như dòng GPU Nvidia RTX 4090). Việc có thể tự chạy một mô hình 70B cục bộ tại nhà với tốc độ phản hồi nhanh nhạy là điều chỉ xuất hiện trong các câu chuyện khoa học viễn tưởng cách đây vài năm.

Mặc dù năng lực tổng quát của mô hình nhỏ khó có thể sánh được với các siêu mô hình đám mây, chúng lại sở hữu những ưu thế vượt trội ở các bài toán chuyên biệt: Vận hành tối ưu cho các tác vụ hẹp, độ chính xác cao khi được huấn luyện sâu trong một lĩnh vực cụ thể, dễ dàng tinh chỉnh (fine-tuning) và thời gian triển khai cập nhật cực nhanh.

Đồng thời chi phí vận hành của mô hình nhỏ cực kỳ tiết kiệm, giúp các cá nhân và doanh nghiệp khởi nghiệp dễ dàng triển khai bảo mật ngay trên hạ tầng máy chủ cục bộ của mình.

Đây chính là lý do các mô hình ngôn ngữ nhỏ đang nhận được sự quan tâm rất lớn của giới công nghệ, mở ra cơ hội cho phép mọi người tự chạy các trợ lý AI chất lượng cao tương đương GPT-3.5 ngay tại nhà với nguồn tài nguyên phần cứng vô cùng tiết kiệm.

## 言论

1、

Rất nhiều người thường rơi vào trạng thái trì hoãn công việc và đưa ra lời biện bạch rằng bản thân chưa có đủ động lực để bắt tay vào hành động. Tuy nhiên thực tế tâm lý học cho thấy động lực chỉ thực sự được sinh ra sau khi bạn đã hành động. Chỉ cần bạn chịu bắt tay vào thực hiện những bước đi đầu tiên hướng về mục tiêu, bạn sẽ tự động thấy tinh thần hăng say và động lực làm việc xuất hiện.

Vì vậy mỗi khi đối mặt với một tác vụ lớn và phức tạp, tôi thường chia nhỏ vấn đề thành các bước thực thi cực kỳ đơn giản. Mục tiêu lúc này không phải là hoàn thành toàn bộ công việc đồ sộ đó mà chỉ đơn giản là kích hoạt hành động của bản thân để bước tiếp một bước đi nhỏ phía trước.

-- *Trích bài phân tích 《Giải pháp khoa học giúp vượt qua hội chứng trì hoãn công việc》*

2、

Mã nguồn an toàn và ổn định nhất của hệ thống hoàn toàn không phải là những dòng code được viết tinh xảo, hoa mỹ hay sử dụng các kỹ thuật phức tạp, mà chính là những dòng code có phần tẻ nhạt và đơn điệu nhất.

Ngôn ngữ Go chính là minh chứng tiêu biểu cho triết lý thiết kế này khi ban quản trị cố tình loại bỏ toàn bộ các cú pháp viết code bóng bẩy hay các cách viết quá linh hoạt, chỉ giữ lại các cú pháp tối giản và dễ đọc hiểu nhất. Chi tiết này giúp mã nguồn dự án cực kỳ dễ dàng cho công tác kiểm tra chéo (code review), ngăn chặn các hành vi lạm dụng kỹ thuật và giảm thiểu tối đa nguy cơ phát sinh các lỗ hổng bảo mật hệ thống.

-- *Trích bài viết 《Sự đơn giản vượt trội vẻ đẹp cú pháp: Tại sao chất lượng mã nguồn quyết định tính an toàn hệ thống》*

3、

Thị hiếu của người dùng đại chúng luôn có xu hướng ưu ái các sản phẩm mới: Đọc sách mới xuất bản, nghe các ca khúc mới phát hành.

Số liệu thống kê lượng phát nhạc trực tuyến tại Mỹ năm 2024 đạt mốc kỷ lục 1,4 nghìn tỷ lượt, tuy nhiên có tới gần 50% thời lượng phát thuộc về các ca khúc được phát hành mới trong giai đoạn từ năm 2020 đến 2024, và gần 80% lượt phát tập trung vào các ca khúc ra đời từ sau năm 2010. Ca khúc có tuổi đời càng lâu thì lượng người nghe càng sụt giảm nghiêm trọng.

-- *Theo báo cáo thống kê của Hãng tin AP*

4、

Tốc độ tiếp nhận các cổng kết nối API thế hệ mới của cộng đồng nhà phát triển dự báo sẽ bị chậm lại đáng kể dưới kỷ nguyên AI. Nguyên nhân do các mô hình ngôn ngữ lớn AI chỉ có khả năng học tập dựa trên kho dữ liệu tri thức sẵn có trong quá khứ, nên khi một API mới được công bố, lượng tài liệu mẫu trực tuyến để AI học tập chắc chắn là cực kỳ khan hiếm.

Đồng thời, những lập trình viên quen phụ thuộc vào AI cũng sẽ tỏ ra e ngại khi chuyển sang sử dụng các API mới này, bởi họ biết rõ AI có khả năng viết code nhanh và chuẩn xác hơn nhiều khi khai thác các thư viện API thế hệ cũ đã có sẵn nhiều tài liệu mẫu.

-- *Chia sẻ của một độc giả trên diễn đàn Hacker News*

## 往年回顾

- Số #305: [Tìm hiểu bản chất toán học của các thuật toán sinh số ngẫu nhiên trong máy tính](https://www.ruanyifeng.com/blog/2024/06/weekly-issue-305.html)
- Số #255: [Thảo luận về tư duy và thái độ ứng xử chuẩn mực của con người trước làn sóng bùng nổ của AI](https://www.ruanyifeng.com/blog/2023/05/weekly-issue-255.html)
- Số #205: [Phân tích về xu thế phát triển: Liệu thời kỳ hoàng kim của làn sóng khởi nghiệp Internet đã chính thức đi qua?](https://www.ruanyifeng.com/blog/2022/05/weekly-issue-205.html)
- Số #155: [Thảo luận chuyên đề: Liệu tiền kỹ thuật số có thể trở thành vũ khí phá vỡ thế độc tôn của đồng USD?](https://www.ruanyifeng.com/blog/2021/04/weekly-issue-155.html)

(Hết)
