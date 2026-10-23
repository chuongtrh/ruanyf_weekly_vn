# Bản tin công nghệ hàng tuần (Số 410): Ba cơ chế AI bạn cần biết

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/10950) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082701.webp)

Bức điêu khắc bịt mắt khổng lồ tại khu thắng cảnh Sa Pha Đầu, Ninh Hạ. ([via](https://www.4anet.com/p/01kzzn7qc04ts41frfk4zqjkc0))

## 你需要知道的 AI 三种机制

Đây là bài viết thứ ba trong loạt bài "Kiến thức nhập môn AI", hai bài trước lần lượt là [《Mô hình lớn cần bao nhiêu bộ nhớ RAM》](https://www.ruanyifeng.com/blog/2026/07/weekly-issue-404.html) và [《Bộ nhớ đệm AI là gì》](https://www.ruanyifeng.com/blog/2026/08/weekly-issue-408.html).

Tôi xin chia sẻ một vài ghi chép học tập cá nhân nhằm hệ thống hóa lại hiểu biết về công nghệ AI. Tôi cố gắng diễn đạt thật bình dị, dễ hiểu, hy vọng sẽ hữu ích với mọi người.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082703.webp)

Hôm nay chúng ta bàn về một câu hỏi cơ bản: **Tại sao AI có thể trả lời các câu hỏi của chúng ta, làm sao nó biết được câu trả lời?**

Bạn có thể tìm thấy rất nhiều luận văn và sách vở về chủ đề này, giải thích cặn kẽ cách vận hành của mô hình lớn, nhưng thường rất khó hiểu. Tuy nhiên, đối với người không chuyên, chỉ cần hiểu một cách đơn giản [ba cơ chế của AI](https://w4g1.dev/blog/models-are-getting-dumber-on-purpose) là đủ:

**（1）Cơ chế tham số (Parameter mechanism)**

Ở tầng vĩ mô, **mọi mô hình ngôn ngữ lớn đều là sự mô hình hóa tri thức nhân loại**. Nó xây dựng một mô hình toán học dùng để mô tả toàn bộ tri thức của loài người.

Mô tả bằng cách nào? Nó sử dụng cơ chế tham số: phân rã tri thức thành từng "token" (từ nguyên/mảnh từ), sau đó tính toán mối quan hệ toán học giữa tất cả các token với nhau. Quá trình này được gọi là "huấn luyện" (training).

Mối quan hệ toán học này được biểu diễn bằng vô số tham số. Ví dụ, mô hình lớn GLM 5.3 có tới 744 tỷ tham số, những tham số này dùng để kiến tạo mối quan hệ (tức trọng số) giữa tất cả các token. Cái gọi là "huấn luyện" thực chất là tìm ra 744 tỷ trọng số đó nhằm mô tả cấu trúc tri thức của nhân loại, tức là mối liên kết giữa các token.

Một khi đã huấn luyện xong, khi chúng ta đặt câu hỏi cho mô hình lớn, nó sẽ dựa trên những trọng số này để tìm ra các token có khả năng xuất hiện cao nhất, từ đó sinh ra câu trả lời phù hợp nhất theo xác suất.

Vì vậy, **bản chất của mô hình lớn là cơ chế "nén - sinh" (compression-generation)**, trừu tượng hóa tri thức loài người vào vô số tham số, rồi sau đó tái tạo sinh ra nội dung.

**（2）Cơ chế suy luận (Reasoning mechanism)**

Không khó để hiểu rằng tham số càng nhiều thì hiệu quả mô hình càng tốt. Bởi nhiều tham số hơn đồng nghĩa với việc có thể mô tả chính xác hơn các loại tri thức khác nhau, từ đó khôi phục lại chuẩn xác hơn.

Tuy nhiên, một mặt tham số không thể tăng lên vô hạn vì chi phí huấn luyện và chi phí vận hành sẽ tăng phi mã, thời gian tính toán khi sử dụng cũng kéo dài.

Mặt khác, cũng không cần thiết phải nạp toàn bộ mọi tri thức vào tham số, có rất nhiều tri thức không cần lưu sẵn trong tham số mà **hoàn toàn có thể suy luận logic ra được**.

Ví dụ, chỉ cần biết tỷ lệ sinh và tỷ lệ tử của một thành phố là có thể biết ngay tỷ lệ tăng trưởng dân số tự nhiên. Điều này không cần phải ghi nhớ cứng, mà có thể tính ra bằng suy luận.

Mô hình lớn dựa vào cơ chế suy luận, xuất phát từ các quy tắc logic kết hợp với tri thức chứa trong tham số để suy ra những tri thức mà nó chưa từng được ghi nhớ sẵn.

**（3）Cơ chế kết nối mạng (Web retrieval mechanism)**

Dù mô hình có nhiều tham số đến đâu, năng lực suy luận mạnh đến mức nào, nó cũng không thể bao quát toàn bộ tri thức thế giới, luôn có những câu hỏi nó không thể tự trả lời.

Ví dụ, nếu bạn hỏi mô hình lớn chỉ số đóng cửa của thị trường chứng khoán hôm nay là bao nhiêu, nó sẽ chịu thua. Tham số không chứa tri thức này, và suy luận cũng không thể đoán ra.

Khi đó, mô hình phải dựa vào cơ chế kết nối Internet do Agent hoặc khung ứng dụng cung cấp, tự động lên mạng tìm kiếm những thông tin mà nó chưa biết.

**（4）Tổng kết**

Chính nhờ có ba cơ chế trên mà AI mới có thể trả lời chính xác các câu hỏi của chúng ta:

Trước hết, cơ chế tham số cung cấp nền tảng tri thức cơ bản của mô hình; kế đến, cơ chế suy luận tạo ra các tri thức mới thông qua suy diễn logic; cuối cùng, cơ chế kết nối mạng giúp thu thập những tri thức mà hai cơ chế đầu không thể có được.

## 公开演讲的窍门

Nhiều bạn khi phải bước lên sân khấu trước đám đông để thuyết trình thường cảm thấy rất run và căng thẳng.

Thực ra chỉ cần nắm vững [vài mẹo nhỏ](https://blog.guillheu.dev/articles/first-time-speaker/) và thiết lập tư duy đúng đắn là bạn hoàn toàn có thể có một buổi diễn thuyết trước công chúng thành công:

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082404.webp)

（1）Một bài thuyết trình thành công thì nội dung chỉ chiếm 30%, kỹ năng trình diễn chiếm tới 70%.
Bạn cần hiểu rằng thuyết trình là một màn trình diễn (show diễn). Bạn phải tận dụng tối đa giọng điệu, cử chỉ, biểu cảm khuôn mặt và động tác tay để thu hút sự chú ý của thính giả, nội dung thực ra không mang tính quyết định tuyệt đối.

（2）Chuẩn bị kỹ lưỡng từ trước.
Bài phát biểu, slide, các mẩu chuyện cười, ngữ điệu, nhịp điệu... tốt nhất mọi chi tiết đều được luyện tập nhiều lần. Bạn không thể đoán trước điều gì sẽ xảy ra khi lên sân khấu, việc luyện tập kỹ càng sẽ giúp bạn bám chắc lộ trình đã định sẵn và hoàn thành suôn sẻ.

（3）Nếu bài nói liên quan đến chi tiết kỹ thuật cụ thể, bạn nên nói nhiều về "Tại sao" (Why) để người nghe hiểu lý do họ nên quan tâm đến điều đó.
Còn về "Làm thế nào" (How), chỉ cần trình bày sơ lược ý tưởng chính và khái niệm chung là đủ, có thể bỏ qua toàn bộ các bước thao tác triển khai tỉ mỉ, vì chẳng ai muốn nghe bạn đọc thuộc lòng tài liệu hướng dẫn cả.

（4）Căng thẳng là chuyện hoàn toàn bình thường.
Nhưng nếu bạn đã chuẩn bị chu đáo và thuộc làu bài thuyết trình thì khi bước lên sân khấu và bắt nhịp được, bạn sẽ nhanh chóng quên đi cảm giác căng thẳng.

（5）Dù nói hay hay dở, bạn nhất định phải tự tin. Nếu ngay cả bản thân bạn còn do dự về những gì mình đang nói thì rất khó để thuyết phục người nghe.
Những người diễn thuyết thành công trước công chúng đều là những người tự tin, chứ chưa chắc đã là người có năng lực chuyên môn giỏi nhất. Rất nhiều nhà quản lý tồi hay thậm chí những kẻ lừa đảo từng có những bài thuyết trình rất thành công, điều đó chứng minh nội dung tuyệt đối không phải điều kiện tiên quyết duy nhất để bước lên bục giảng.

（6）Chỉ cần bạn có khao khát chia sẻ về một chủ đề nào đó, bạn chắc chắn đã đủ tư cách để bước lên sân khấu.

## 科技动态

1. [Chiếc ghế dạng phẳng xếp gọn](https://www.toxel.com/tech/2026/08/07/flat-chair-by-sara-paculdo/)

Một nhà thiết kế người Mỹ đã sáng tạo ra chiếc ghế bằng sợi thủy tinh, khi nhận hàng người dùng chỉ cầm trên tay một tấm phẳng duy nhất.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082405.webp)

Chỉ mất vài phút tách các bộ phận ra và lắp ghép lại là bạn đã có một chiếc ghế hoàn chỉnh.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082406.webp)

Thiết kế dạng phẳng này giúp giảm đáng kể thể tích vận chuyển, không gian lưu trữ và chi phí giao hàng.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082407.webp)

Ghế dựa vào sức căng của các đường cong và các khớp nối cài vào nhau để tạo nên độ vững chắc chịu lực tốt.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082408.webp)

2. [Concert avatar ảo](https://www.billboard.com/music/country/dolly-parton-health-update-1236322526/)

Tuần này, nữ ca sĩ huyền thoại người Mỹ Dolly Parton qua đời ở tuổi 80. Tin tức này rất bất ngờ, bởi cách đó không lâu bà vừa thông báo sẽ tổ chức concert.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082502.webp)

Tuy nhiên bà không trực tiếp lên sân khấu biểu diễn mà ủy quyền tạo một "avatar ảo" để avatar này thay bà hát trên sân khấu.

Bà không tiết lộ chi tiết cụ thể, nhưng về mặt công nghệ hiện nay điều này hoàn toàn khả thi. AI ngày nay không chỉ hát giống như thật mà còn có thể render hình ảnh theo thời gian thực và tương tác với người hâm mộ.

Những buổi concert dùng avatar ảo này có rất nhiều lợi thế: có thể tổ chức với số lượng lớn, một ngày diễn vài buổi đều được, giá vé rẻ, và đặc biệt là làm được những việc mà ca sĩ người thật không thể làm, chẳng hạn như ca sĩ đã khuất vẫn có thể tiếp tục mở concert. Tin rằng sau lần tiên phong này, thị trường sẽ xuất hiện hàng loạt mô hình tương tự tạo thành một ngành kinh doanh riêng biệt.

3. [Bộ trợ lực xe đạp thông minh](https://www.asus.com/accessories/bike-booster/asus-oxiis/oxiis-intelligent-bike-booster/)

ASUS vừa ra mắt một "bộ trợ lực xe đạp", có thể gắn vào bất kỳ chiếc xe đạp nào để biến xe đạp cơ thông thường thành xe đạp trợ lực điện.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082704.webp)

Nguyên lý rất đơn giản: một khối pin dẫn động một bánh lăn nhỏ.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082705.webp)

Bạn gắn nó lên phía trên bánh sau, bánh lăn sẽ tự tì vào lốp và kéo bánh sau quay, từ đó tạo ra lực trợ lực đẩy xe đi.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082707.webp)

Thiết bị này rất hữu ích khi leo dốc hoặc chở hàng nặng, rất đáng được nhân rộng.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082708.webp)

## 文章

1. [Kỷ nguyên AI đầy biến động đã tới](https://www.gatesnotes.com/home/home-page-topic/reader/a-turbulent-ai-era-and-critical-choices-to-make) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082709.webp)

Bill Gates tuần này đăng một bài viết cho rằng AI tiềm ẩn nhiều rủi ro và nên làm chậm lại tốc độ phát triển.

Tuy nhiên năm 2023 ông từng đăng một bài viết với quan điểm hoàn toàn trái ngược [《Rủi ro của AI là có thật, nhưng hoàn toàn có thể kiểm soát》](https://www.gatesnotes.com/work/make-ai-work-for-everyone/reader/the-risks-of-ai-are-real-but-manageable).

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082710.webp)

Điều gì trong suốt 3 năm qua đã khiến ông đổi ý? Nhưng bất kể ông nghĩ gì, tốc độ phát triển của AI chỉ có thể ngày càng nhanh hơn chứ không thể chậm lại được nữa.

2. [Ox Alpha chính là mô hình GLM](https://dejan.ai/blog/ox-alpha/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082504.webp)

Mấy hôm trước trên mạng xuất hiện một mô hình ẩn danh tên Ox Alpha với hiệu năng vô cùng xuất sắc, khiến cộng đồng thi nhau phỏng đoán xem công ty nào đứng sau. Cuối cùng Zhipu AI (Trí Phổ) thừa nhận đó chính là GLM 5.3 Flash.

Tuy nhiên trước đó đã có người dựa trên bằng chứng kỹ thuật để suy đoán ra đơn vị đứng sau là Zhipu. Bài viết chia sẻ cách lần ra danh tính tác giả của mô hình.

Nhân tiện, điểm Artificial Analysis của mô hình này đạt 57 điểm, cao hơn DeepSeek V4 Pro (53 điểm). Điều này thực sự ấn tượng vì số tham số kích hoạt của nó chỉ là 18B, nhỏ hơn mức 49B của DeepSeek. Và với số lượng tham số nhỏ như vậy, nó hoàn toàn có thể chạy mượt mà trên máy tính cá nhân.

3. [Hướng dẫn chi tiết sử dụng Git worktree](https://barrd.dev/article/parallel-development-without-the-headaches-using-git-worktree/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082402.webp)

Kho Git thông thường chỉ có một thư mục làm việc, nếu phát triển đồng thời hai hoặc ba tính năng thì việc chuyển đổi nhánh qua lại rất bất tiện.

Lệnh `git worktree` cho phép tạo nhiều thư mục làm việc độc lập song song; bài viết hướng dẫn chi tiết cách sử dụng.

4. [Trang web AliExpress dùng kỹ thuật nhận dạng dấu vân tay âm thanh WebAudio](https://blog.laserphile.com/2026/08/aliexpress-webpage-keeping-multipoint.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082003.webp)

Một lập trình viên nước ngoài tình cờ phát hiện trang chủ AliExpress có đoạn code sử dụng WebAudio API, khiến mỗi lần mở trang này thì tai nghe Bluetooth của anh đều bị ngắt kết nối. Kiểm tra kỹ mã nguồn, anh phát hiện ra mục đích của đoạn mã là để định danh thiết bị người dùng (device fingerprinting).

5. [Lỗi kiểm tra tên miền ngớ ngẩn của Google Workspace](https://blog.elis.cc/articles/google-workspace-thinks-my-domain-is-an-email-provider/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082403.webp)

Dịch vụ doanh nghiệp Google Workspace yêu cầu liên kết tên miền của người dùng, nhưng tên miền của tác giả liên tục bị hệ thống từ chối.

Tác giả liên hệ với đội hỗ trợ khách hàng thì chỉ nhận lại những câu trả lời sáo rỗng vô dụng. Cuối cùng, chịu không nổi, anh tự kiểm tra mã nguồn frontend và phát hiện nguyên nhân chỉ là do một hàm JavaScript phía client kiểm tra tên miền; chỉ cần vô hiệu hóa hàm này là tên miền được thêm thành công. Tình trạng chất lượng dịch vụ của Google hiện nay thực sự khiến người ta cạn lời.

6. [Thuật toán sinh số ngẫu nhiên Xorshift](https://www.alanzucconi.com/2026/08/15/xorshift-generators/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082409.webp)

Có thể nhiều người chưa biết, hầu hết các số ngẫu nhiên trong tính toán thường ngày đều do thuật toán Xorshift sinh ra: thông qua các phép toán XOR và dịch bit (shift) trên giá trị seed ban đầu. Bài viết giới thiệu chi tiết cách triển khai thuật toán này.

## 工具

1. [Vanilla OS 3](https://vanillaos.org)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082601.webp)

Bản phân phối Linux dựa trên Debian hiện thực hóa hệ điều hành bất biến (immutable), nơi mọi thao tác hệ thống đều mang tính nguyên tử (atomic). (Đóng góp từ [@NN708](https://github.com/ruanyf/weekly/issues/11356))

2. [stock-tui](https://github.com/Folgerjun/stock-tui)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082602.webp)

Công cụ dòng lệnh TUI xem biểu đồ nến K-line, tỷ số P/E và khối lượng giao dịch cổ phiếu hạng A. (Đóng góp từ [@Folgerjun](https://github.com/ruanyf/weekly/issues/11354))

3. [Dark mode PDFs](https://veil.simoneamico.com/)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026032702.webp)

Trang web nhỏ thú vị giúp đảo ngược màu sắc file PDF tải lên, biến chữ đen nền trắng thành chữ trắng nền đen để đọc trong bóng tối.

4. [Termio](https://github.com/termio-sh/termio)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082410.webp)

Môi trường phát triển lập trình AI (ADE) dành cho Mac, có phiên bản đồng bộ đi kèm trên iPhone. (Đóng góp từ [@jiweiyuan](https://github.com/ruanyf/weekly/issues/11273))

5. [PicLite](https://github.com/amiaoapp/PicLite) (Đồ Khinh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082411.webp)

Công cụ nén ảnh đa nền tảng, hỗ trợ theo dõi thư mục cục bộ, chuyển đổi định dạng ảnh, nén hàng loạt, chèn watermark và tải ảnh lên hosting. (Đóng góp từ [@amiaoapp](https://github.com/ruanyf/weekly/issues/11290))

6. [Multi-Row Tabs](https://github.com/hezhizheng/multi-row-tabs)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082412.webp)

Extension Chrome hiển thị toàn bộ các tab đang mở của cửa sổ trình duyệt dưới dạng nhiều hàng xếp chồng lên nhau. (Đóng góp từ [@hezhizheng](https://github.com/ruanyf/weekly/issues/11310))

7. [InvoiceFlowAI](https://github.com/EthanYoQ/Invoice-Downloader)

Công cụ desktop mã nguồn mở giúp quản lý và thanh toán hóa đơn điện tử: kết nối hòm thư QQ hoặc 163 của người dùng, tự động thu thập hóa đơn đính kèm trong email, nhận dạng OCR, phân loại lưu trữ và xuất bảng tổng hợp Excel. (Đóng góp từ [@EthanYoQ](https://github.com/ruanyf/weekly/issues/11327))

8. [CozyClay](https://github.com/NomaDamas/CozyClay)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082501.webp)

Dựng khung cảnh, tạo tư thế cho nhân vật, thiết lập chuyển động camera và cắt ghép ngay trong trình duyệt, sau đó chuyển cho mô hình AI video để sinh ra video với độ chính xác cao hơn. (Đóng góp từ [@HaD0Yun](https://github.com/ruanyf/weekly/issues/11329))

9. [Email.md](https://www.emailmd.dev/templates)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026032801.webp)

Trang web cung cấp các mẫu email, người dùng chỉ cần viết nội dung bằng Markdown là hệ thống sẽ tự động tạo email đã được format chỉn chu đẹp mắt.

10. [Minimalytics](https://github.com/nafey/minimalytics)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032101.webp)

Máy chủ thống kê gọn nhẹ ghi nhận và theo dõi các sự kiện, viết bằng ngôn ngữ Go và cơ sở dữ liệu SQLite, tích hợp sẵn giao diện Web.

## 资源

1. [Starbase SpaceX](https://www.spacex.com/sites/starbase-la)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082603.webp)

SpaceX chuẩn bị xây dựng một "Starbase" mới tại bang Louisiana; trang web chính thức của căn cứ trông hệt như trong phim khoa học viễn tưởng.

2. [Dạo quanh San Francisco](https://sf.thijs.gg/)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082503.webp)

Game nền web cho phép người chơi lang thang trên bản đồ đường phố San Francisco thực tế, có thể chọn địa điểm cụ thể, trải nghiệm rất thú vị.

3. [Bản đồ mạng lưới đường phố đô thị](https://anvaka.github.io/city-roads/) (city-roads)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122612.webp)

Trang web biến toàn bộ mạng lưới đường phố của một thành phố bất kỳ thành một bức tranh vẽ đường nét tối giản, hỗ trợ phóng to thu nhỏ.

## 图片

1. [Những bức tượng điêu khắc nhỏ nhất London](https://lookup.london/londons-smallest-public-sculptures/)

London có một số bức điêu khắc công cộng tí hon ẩn chứa những câu chuyện rất bất ngờ.

Trên đỉnh mặt tiền tầng một của một con phố sầm uất có bức điêu khắc hai chú chuột đang ăn trộm phô mai.

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051704.webp)

Tương truyền bức tượng này được dựng để tưởng nhớ một câu chuyện bi kịch.

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051705.webp)

Vào thế kỷ 19, hai người công nhân xây dựng tại đây đã ẩu đả kịch liệt vì một miếng phô mai bị biến mất, dẫn đến chết người; về sau người ta mới phát hiện miếng phô mai thực ra là do lũ chuột tha đi mất.

Ở London còn có một bức điêu khắc "ngôi nhà của chuột".

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051706.webp)

Chủ cửa hàng tại đây phát hiện dãy số nhà trên phố bị thiếu mất một số, nên ông đã làm bức điêu khắc này và gán số nhà bị thiếu cho ngôi nhà của chú chuột.

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051707.webp)

Dưới đây là một số tác phẩm điêu khắc siêu nhỏ khác:

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051708.webp)

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051709.webp)

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051710.webp)

## 文摘

1. [Mạng lưới tính đồng nhất](https://www.science.org/doi/10.1126/science.aei2409)

Một đặc tính căn bản của mạng xã hội là chúng thúc đẩy các mạng lưới mang tính "đồng nhất" (homophily).

Tính đồng nhất ám chỉ việc người dùng sẽ dễ dàng bắt gặp những người có nét tương đồng với mình. Chẳng hạn người thích ngắm chim sẽ tham gia nhóm ngắm chim online, người chơi bowling sẽ tụ họp với những người chơi bowling khác.

Hệ quả là mạng Internet sẽ kéo những người có quan điểm thiểu số, bên lề lại với nhau. Những người tin rằng Trái Đất phẳng có thể dễ dàng kết nối với nhau trên mạng — điều mà ngoài đời thực gần như bất khả thi vì số người tin vào Trái Đất phẳng quá ít ỏi và khó lòng gặp được nhau.

Mạng lưới đồng nhất sẽ làm sai lệch nhận thức của con người về sự phân bố quan điểm trong xã hội. Những người có quan điểm rõ ràng là thiểu số, khi ở lâu trong các mạng lưới đồng nhất, có thể lầm tưởng rằng quan điểm của họ đại diện cho sự đồng thuận của đa số — hiện tượng này gọi là "hiệu ứng đồng thuận giả" (false consensus effect).

Hiệu ứng đồng thuận giả gây ra một số hệ lụy: (1) Nó có thể củng cố niềm tin mù quáng của các cá nhân vào quan điểm thiểu số; (2) Khi một người lầm tưởng quan điểm thiểu số được xã hội đón nhận rộng rãi, họ sẽ nảy sinh bất mãn với các thể chế và quyết định vận hành theo ý chí của số đông, từ đó sinh ra cảm giác bản thân đang bị xã hội bài xích, cô lập.

## 言论

1.

Biểu hiện của một người có tu dưỡng là họ có thể tận hưởng những thứ tốt đẹp nhất, đồng thời cũng có thể chịu đựng được những hoàn cảnh tồi tệ nhất.

-- [Đường Sư Tăng](https://news.pku.edu.cn/xwzh/129-116805.htm), nhà báo nổi tiếng vừa qua đời tuần này

2.

Thế giới của chúng ta không phải lúc nào cũng là nơi mọi người biết đặt mình vào vị trí của người khác. Nhưng nếu bạn có thể giải thích thế giới cho một đứa trẻ 10 tuổi hiểu, hoặc thiết kế một chiếc nắp lọ mà một cụ già 80 tuổi cũng có thể dễ dàng mở được, đôi khi điều đó sẽ giúp bạn hoàn thành tốt hơn mục tiêu ban đầu mình muốn hướng tới.

-- [《Xin hãy giải thích cho tôi như thể tôi là đứa trẻ 10 tuổi》](https://timharford.com/2026/08/explain-it-to-me-like-im-ten/)

3.

Có người viết bài "Trực ca đã là chuyện dĩ vãng", đề xuất nên để AI đảm nhiệm việc trực ca hệ thống. Chỉ khi AI không giải quyết được vấn đề thì mới bàn giao cho con người, và nên để AI chủ động gọi điện báo cho kỹ sư.

-- [《Những sự cố độ tin cậy liên quan đến AI sắp sửa xảy ra》](https://surfingcomplexity.blog/2026/08/22/wild-ai-related-reliability-incidents-are-coming/)

4.

Mọi người dần nhận ra rằng nếu dùng AI để học kiến thức mới, tốc độ học nhanh hơn rất nhiều so với phương pháp truyền thống, vì AI cực kỳ giỏi trong việc khái quát hóa lượng lớn thông tin phân tán.

Tuy nhiên, học qua AI thì bộ não không chủ động tham gia sâu vào quá trình học tập, dẫn đến việc hiểu và ghi nhớ kiến thức không sâu sắc bằng cách truyền thống. Cách thức hoạt động của não bộ quyết định rằng học theo đường xoắn ốc (lặp lại ngắt quãng và đào sâu) là phương pháp tốt nhất để ghi nhớ tri thức. AI đưa thẳng ra kết quả, khiến chúng ta bỏ qua các bước tư duy, trăn trở qua lại ở giữa.

-- [《AI và kiến thức kiểu tài xế》](https://www.aaron-gray.com/ai-and-chauffeur-knowledge/)

5.

Nếu giá nhà lao dốc, tài sản của tôi sẽ bị thiệt hại, nhưng điều đó cũng mang lại điểm tích cực: con cái tôi sẽ được ở trong những căn nhà rẻ hơn. Đúng vậy, phần thừa kế chúng nhận được sẽ ít đi, nhưng đổi lại chúng sẽ được hưởng chi phí nhà ở rẻ hơn trong suốt cả cuộc đời.

-- [《Chứng chỉ tiền gửi và tâm lý NIMBY》](https://www.betonit.ai/p/cds-vs-nimby)

## 往年回顾

[Giải thích mạng nơ-ron dễ hiểu nhất](https://www.ruanyifeng.com/blog/2025/08/weekly-issue-363.html) (#363)

[Nếu Singapore không có điều hòa](https://www.ruanyifeng.com/blog/2024/08/weekly-issue-313.html) (#313)

[Phần mềm mã nguồn mở kiếm tiền như thế nào?](https://www.ruanyifeng.com/blog/2023/07/weekly-issue-263.html) (#263)

[Ốc đảo tri thức và phần mềm tri thức](https://www.ruanyifeng.com/blog/2022/07/weekly-issue-213.html) (#213)

(Hết)
