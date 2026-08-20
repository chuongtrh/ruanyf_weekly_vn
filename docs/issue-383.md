# Bản tin chia sẻ công nghệ (Số 383): Bạn đang ở cấp độ nào trong lập trình AI

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/8591) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012103.webp)

Khu đô thị cửa ngõ nhà ga đường sắt cao tốc Nghi Tân, tỉnh Tứ Xuyên vừa hoàn thành xây dựng. Dự án lấy nhà ga cao tốc làm hạt nhân phát triển trung tâm, bao gồm tổ hợp 8 tòa tháp cao tầng, công viên trung tâm, trung tâm nghệ thuật kỹ thuật số và phân khu phố đi bộ văn hóa thương mại. ([via](http://www.archina.com/index.php?g=works&m=index&a=show&id=159920))

## 你是第几级 AI 编程

Steve Yegge là một lập trình viên người Mỹ vô cùng nổi tiếng trong cộng đồng công nghệ.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012408.webp)

Ông từng có thời gian dài công tác tại cả hai tập đoàn công nghệ hàng đầu là Amazon và Google. Tuy nhiên, điều khiến tên tuổi của ông được đông đảo giới lập trình viên biết đến rộng rãi lại không phải là các phần mềm do ông viết, mà là các bài viết blog cá nhân của ông.

Ông sở hữu thói quen đăng tải những bài viết phân tích cực kỳ dài trên trang web cá nhân để thảo luận thẳng thắn, bộc lộ quan điểm cá nhân một cách trực diện mà không hề né tránh các vấn đề nhạy cảm của ngành. Rất nhiều bài viết của ông đã tạo nên những làn sóng thảo luận vô cùng sôi nổi và có sức ảnh hưởng lớn trong giới công nghệ.

Các bài viết nổi bật của ông sau đó đã được tổng hợp lại để xuất bản thành sách và được dịch sang nhiều ngôn ngữ, tiêu biểu là cuốn sách dịch mang tên [《Tiếng thét của lập trình viên (The Programmer's Rant)》](https://book.douban.com/subject/25852508/) (phiên bản tiếng Trung do Nhà xuất bản Bưu điện Nhân dân phát hành năm 2014).

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012409.webp)

Tên tiếng Anh gốc của cuốn sách có chứa từ "ranting" (nghĩa gốc là gào thét,咆哮), mô tả cực kỳ chính xác phong cách hành văn đặc trưng của tác giả.

Tháng này, ông vừa cho xuất bản [bài viết mới nhất](https://steve-yegge.medium.com/welcome-to-gas-town-4f25ee16dd04) chia sẻ những góc nhìn cá nhân của mình về trào lưu lập trình bằng công nghệ AI.

**Ông chia sẻ rằng quy trình lập trình bằng AI được chia thành 8 cấp độ phát triển rõ rệt, và bản thân ông hiện đã tiến tới cấp độ 8** – tức cấp độ cao nhất.

Cấp độ 1: Lập trình viên hoàn toàn chưa tiếp cận với các công cụ AI hỗ trợ viết code, giao diện trình soạn thảo IDE vẫn giữ nguyên cấu trúc truyền thống như dưới đây.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012410.webp)

Cấp độ 2: Bạn bắt đầu cài đặt các plugin trợ lý AI cho IDE của mình, kích hoạt thanh sidebar phụ cạnh màn hình để AI liên tục đưa ra các gợi ý dòng code tự động viết tiếp và bạn lựa chọn chấp nhận hay từ chối (Yes or No).

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012411.webp)

Cấp độ 3: Bạn bắt đầu thiết lập sự tin tưởng tuyệt đối vào khả năng viết code của AI, chuyển sang trạng thái làm việc YOLO (triết lý "You Only Live Once" - Bạn chỉ sống một lần). Để tối ưu hóa thời gian và năng lượng làm việc, bạn dẹp bỏ bước duyệt rà soát từng gợi ý của AI mà liên tục bấm phím xác nhận (Yes) để chấp nhận mọi đoạn code do máy tự sinh ra.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012412.webp)

Cấp độ 4: Giao diện hiển thị của trợ lý AI ngày càng phình to và chiếm phần lớn không gian màn hình của bạn, khu vực soạn thảo code thủ công chỉ còn được giữ lại một góc nhỏ chủ yếu dùng để so sánh các thay đổi (git diff).

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012413.webp)

Cấp độ 5: Bạn quyết định loại bỏ hoàn toàn giao diện soạn thảo code truyền thống mà chuyển sang sử dụng hoàn toàn cửa sổ dòng lệnh (chẳng hạn như Claude Code), dồn toàn bộ không gian màn hình hiển thị cho AI chạy. Ở cấp độ này, bạn thậm chí không cần quan tâm đến mã nguồn AI sinh ra nữa mà chỉ tập trung theo dõi thanh tiến trình hoàn thành công việc của hệ thống.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012414.webp)

Cấp độ 6: Bạn cảm thấy tốc độ xử lý của một luồng AI là quá chậm, do đó quyết định mở đồng thời từ 3 đến 5 cửa sổ terminal để chạy song song nhiều luồng AI cùng lúc nhằm đẩy nhanh tối đa tiến độ dự án.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012415.webp)

Cấp độ 7: Số lượng cửa sổ chạy song song AI tăng lên trên mốc 10 luồng – đây đã chạm tới giới hạn tối đa mà một bộ óc con người có khả năng tự quản lý thủ công cùng một lúc.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012416.webp)

Cấp độ 8: Bạn chuyển sang sử dụng các bộ lập lịch và điều phối tác vụ AI (AI task orchestrator) để máy tính tự động hóa việc phân bổ và giám sát hoạt động của hàng chục luồng AI lập trình chạy song song cùng lúc.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012417.webp)

Trên đây chính là 8 cấp độ phát triển của quy trình lập trình bằng AI, hãy thử tự đánh giá xem bản thân bạn hiện đang nằm ở cấp độ nào?

Câu chuyện chưa dừng lại ở đó. Như đã đề cập, Steve Yegge hiện đã nâng tầm bản thân lên cấp độ thứ 8. Ông có nhu cầu tìm kiếm một công cụ hỗ trợ điều phối tự động các luồng lập trình AI chạy song song nhưng không tìm thấy sản phẩm nào đáp ứng tốt yêu cầu trên thị trường.

Do đó, ông đã trực tiếp ra lệnh cho AI tự viết nên một công cụ điều phối chuyên dụng của riêng mình và đặt tên dự án là "**Gas Town**" (Thị trấn khí gas). Cái tên này lấy cảm hứng từ căn cứ địa của gã phản diện Immortan Joe trong bộ phim hành động bom tấn 《Mad Max: Fury Road》. Nơi đây ngập tràn các động cơ khí đốt cũ kỹ được độ chế chắp vá từ các linh kiện phế thải, trông vô cùng tạm bợ rách nát nhưng vẫn vận hành hiệu quả.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012418.webp)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012419.webp)

Ông chia sẻ thành thật rằng quá trình phát triển Gas Town hoàn toàn là sự chắp vá, gom nhặt mọi linh kiện tính năng mà không cần quan tâm đến cấu trúc thiết kế khoa học, chỉ cần chạy thử không báo lỗi là ông bấm xác nhận chấp nhận đoạn code. "Dự án hiện chứa tới 225.000 dòng mã nguồn viết bằng ngôn ngữ Go, nhưng tôi chưa từng trực tiếp đọc qua dòng code nào của nó và cũng không bao giờ có ý định xem thử."

Ông thẳng thắn đưa ra lời khuyên mọi người không nên cố gắng sử dụng công cụ này, bởi việc vận hành nó yêu cầu bạn phải đặt niềm tin tuyệt đối và mù quáng vào khả năng của AI. Và ngay cả khi bạn tin tưởng nó, nó vẫn có khả năng làm mọi thứ rối tung lên ngoài tầm kiểm soát. Thêm vào đó việc chạy đồng thời hàng chục luồng AI song song sẽ ngốn một khoản chi phí API khổng lồ của bạn.

Mặc dù vậy, ông vẫn quyết định mở nguồn mở [dự án này trên GitHub](https://github.com/steveyegge/gastown) vì tính giải trí và thú vị của nó. Tính đến tuần trước, dự án đã nhanh chóng nhận được hơn 6.000 lượt yêu thích (stars) từ cộng đồng lập trình viên toàn cầu.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012420.webp)

## 科技动态

1. **Trí thông minh bất ngờ của loài bò**

Một nông dân người Áo vô cùng kinh ngạc khi phát hiện ra một chú bò trong trang trại của mình biết cách dùng miệng ngậm một cành củi khô để tự gãi ngứa trên lưng.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012406.webp)

Phát hiện này đã gây kinh ngạc lớn cho giới nghiên cứu, bởi nó chứng minh loài bò sở hữu khả năng tự biết cách sử dụng các công cụ – một tập tính trước đây chưa từng được ghi nhận ở loài động vật này.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012407.webp)

Hiện nay ngoài con người, khoa học mới chỉ ghi nhận hành vi biết sử dụng công cụ ở loài tinh tinh. Các nhà khoa học cho biết điều này đòi hỏi chúng ta phải đánh giá lại toàn bộ mức độ thông minh của loài bò.

2. **Hệ thống tích trữ năng lượng đường ray**

Một công ty Mỹ đã thiết kế hệ thống tích năng đường ray (ARES - Advanced Rail Energy Storage) tận dụng các đường ray chạy dọc theo địa hình đồi núi để tích trữ năng lượng.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011017.webp)

Khi nguồn cung lưới điện dư thừa, hệ thống sẽ sử dụng động cơ điện kéo các toa tàu chở nặng từ chân núi di chuyển lên đỉnh núi để tích năng.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011018.webp)

Khi lưới điện thiếu hụt năng lượng, hệ thống sẽ thả cho các toa tàu nặng tự trượt dốc theo quán tính trọng lực từ đỉnh núi xuống chân núi, từ đó kéo căng các sợi cáp xích để kích hoạt máy phát điện tạo ra dòng điện cung cấp ngược lại cho lưới.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011019.webp)

Ưu điểm lớn nhất của hệ thống này là cấu tạo cơ khí đơn giản, độ tin cậy cao, chi phí vận hành thấp và có khả năng hoạt động liên tục nhiều năm mà không hề phát sinh hiện tượng hao mòn hay suy giảm hiệu năng lưu trữ như các hệ thống pin hóa học.

3. **Miếng dán hỗ trợ phát âm vùng cổ họng**

Nối tiếp thiết bị vòng cổ thông minh giới thiệu ở số trước, số này tiếp tục giới thiệu một phát minh có tính năng tương tự. Đội ngũ nghiên cứu thuộc Đại học California, Los Angeles (UCLA) đã thiết kế một miếng dán đeo vùng cổ họng hỗ trợ các bệnh nhân mất khả năng ngôn ngữ tự phục hồi giọng nói nhân tạo.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031903.webp)

Nhiều bệnh nhân do mắc các bệnh lý nghiêm trọng về thanh quản dẫn đến mất đi dây thanh âm và không thể tự phát âm thành tiếng, nhưng các nhóm cơ vùng cổ họng của họ vẫn có khả năng vận động bình thường.

Miếng dán đặc biệt này khi được dán lên cổ họng sẽ cảm nhận chính xác các rung động chuyển động của nhóm cơ cổ, chuyển đổi chúng thành các tín hiệu điện sinh học để gửi đi.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031904.webp)

Hệ thống máy tính sau khi nhận được tín hiệu điện sẽ tự động dịch nghĩa và phát ra giọng nói tương ứng với nội dung người dùng muốn diễn đạt.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031905.webp)

Để thiết lập mối tương quan chính xác giữa chuyển động cơ cổ và giọng nói, nhóm nghiên cứu đã áp dụng các thuật toán máy học (machine learning) để xây dựng bộ liên kết ngữ nghĩa giữa tín hiệu điện và từ vựng.

## 文章

1. [Tổng hợp các trình phát nhạc phổ biến trên hệ điều hành Linux năm 2026](https://crescentro.se/posts/linux-music-players-2026/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012701.webp)

Bài viết điểm lại và giới thiệu các dòng phần mềm nghe nhạc chất lượng cao phổ biến nhất dành cho cộng đồng người dùng Linux hiện nay.

2. [Giải pháp cấu hình chặn truy cập giao thức cũ HTTP/1.0 và HTTP/1.1 trên máy chủ](https://markmcb.com/web/selectively_disabling_http_1/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012301.webp)

Hướng dẫn phương pháp thiết lập máy chủ Nginx để vô hiệu hóa quyền truy cập qua các giao thức mạng cũ đã lỗi thời là HTTP/1.0 và HTTP/1.1, ngoại trừ một số địa chỉ nằm trong danh sách trắng (whitelist). Giải pháp hiệu quả để loại bỏ phần lớn các cuộc tấn công mạng và bot cào dữ liệu tự động.

3. [Cách thức tôi quét tìm mật khẩu rò rỉ từ các commit lỗi đã bị xóa trên GitHub](https://trufflesecurity.com/blog/guest-post-how-i-scanned-all-of-github-s-oops-commits-for-leaked-secrets/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070316.webp)

Nếu bạn vô tình submit nhầm mật khẩu lên GitHub, giải pháp của bạn là gì? Đa số lập trình viên sẽ lập tức sửa code và thực hiện lệnh force push để ghi đè lịch sử commit trước đó.

Bài viết cảnh báo giải pháp này hoàn toàn không an toàn. Thực chất GitHub không hề xóa bỏ hoàn toàn dữ liệu của commit cũ mà chỉ ẩn chúng đi dưới dạng các commit mồ côi (orphan commits). Tác giả đã thử nghiệm quét toàn bộ dữ liệu lịch sử force push của GitHub và phát hiện ra một lượng lớn mật khẩu cùng khóa bảo mật quan trọng vẫn đang bị rò rỉ công khai.

4. [Hướng dẫn thiết kế các bộ đếm số chuyển động bằng CSS](https://css-tricks.com/animating-number-counters/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070317.webp)

Bài viết tổng hợp các phương pháp lập trình hiệu ứng chuyển động tăng giảm số lượng (number counters) sinh động trên trang web chỉ bằng việc áp dụng các cú pháp CSS thuần túy.

5. [Những kịch bản ứng dụng thực tế của công cụ tự động hóa n8n](https://www.xda-developers.com/built-expense-tracker-using-n8n/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060406.webp)

n8n là một công cụ hỗ trợ thiết lập quy trình tự động hóa công việc trực quan bằng giao diện đồ họa. Tác giả giới thiệu cách tự xây dựng hệ thống theo dõi chi tiêu cá nhân: gửi thông tin chi phí qua app chat tới máy chủ n8n local, AI sẽ tự động phân tích phân loại chi phí và ghi nhận dữ liệu vào Google Sheets.

6. [Những tính năng mới của HTML lập trình viên cần cập nhật trong năm 2025](https://frontendmasters.com/blog/bone-up-html-2025/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025011921.webp)

Bài viết tổng hợp các thuộc tính và tính năng mới được cập nhật trong đặc tả HTML mà lập trình viên nên nắm vững để tối ưu hóa mã nguồn.

7. [Gợi ý danh sách các ứng dụng tự lưu trữ (Self-hosted) chất lượng mới ra mắt](https://selfh.st/2024-favorite-new-apps/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025011922.webp)

Tác giả tổng hợp và chia sẻ danh sách các ứng dụng self-hosted yêu thích cá nhân có giao diện đẹp và tính năng rất hữu ích cho các dự án homelab.

## 工具

1. [teemux](https://github.com/gajus/teemux)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012503.webp)

Công cụ dòng lệnh phát triển bằng JavaScript hỗ trợ lập trình viên gộp và hiển thị tập trung toàn bộ dữ liệu log đầu ra của nhiều tiến trình đang chạy tại một giao diện duy nhất, hỗ trợ xem qua terminal hoặc qua trình duyệt web.

2. [daedalOS](https://github.com/DustinBrett/daedalOS)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052602.webp)

Môi trường desktop ảo mã nguồn mở chạy trực tiếp trên trình duyệt web với thiết kế giao diện mô phỏng tương tự hệ điều hành Windows.

3. [Dendron](https://www.dendron.so/)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052633.webp)

Plugin hỗ trợ ghi chú chất lượng cao dành cho VS Code, giúp quản lý ghi chú dưới dạng thư mục phân cấp trực quan, hỗ trợ vẽ sơ đồ liên kết giữa các ghi chú. Tham khảo thêm [bài viết giới thiệu chi tiết](https://www.xda-developers.com/how-i-use-dendron-to-organize-project-documentation-across-devices/).

4. [CWD](https://github.com/anghunk/cwd) (Cloudflare Workers Discuss)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012307.webp)

Giải pháp xây dựng hệ thống bình luận (comment system) cho trang web vận hành hoàn toàn trên nền tảng Cloudflare Workers. (Đóng góp từ [@anghunk](https://github.com/ruanyf/weekly/issues/8801))

5. [Mouse Gestures](https://github.com/Chance-fyi/mouse-gestures)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012304.webp)

Plugin mã nguồn mở dành cho trình duyệt Chrome hỗ trợ người dùng thực hiện nhanh các tác vụ duyệt web (back, forward, reload...) thông qua cử chỉ vẽ đường đi của chuột trên màn hình. (Đóng góp từ [@Chance-fyi](https://github.com/ruanyf/weekly/issues/8779))

6. [relationship-ts](https://github.com/ExploringTheCodeWorld/relationship-ts)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012306.webp)

Thư viện JavaScript/TypeScript chuyên dụng để tính toán nhanh cách xưng hô các mối quan hệ họ hàng của người Trung Quốc. Các bạn có thể trải nghiệm [bản demo trực tuyến](https://example.qinyimo.cn/). (Đóng góp từ [@ExploringTheCodeWorld](https://github.com/ruanyf/weekly/issues/8792))

7. [Deck](https://github.com/yuzeguitarist/Deck)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012403.webp)

Ứng dụng desktop mã nguồn mở quản lý clipboard dành riêng cho hệ điều hành macOS, hỗ trợ bảo mật mở khóa bằng Touch ID và mã hóa đầu cuối dữ liệu. (Đóng góp từ [@yuzeguitarist](https://github.com/ruanyf/weekly/issues/8809))

8. [EdgeTunnel](https://github.com/tianrking/Re_edgetunnel) (Refactored)

Giải pháp thiết lập đường truyền đường hầm (tunnel) mã nguồn mở chạy trên nền tảng Cloudflare Workers, mã nguồn phiên bản mới đã được tái cấu trúc sạch sẽ và tối ưu hơn. (Đóng góp từ [@tianrking](https://github.com/ruanyf/weekly/issues/8828))

9. [Mail Studio](https://github.com/wzc520pyfm/mail-studio)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012816.webp)

Trình biên tập email trực quan mã nguồn mở, hỗ trợ người dùng kéo thả các khối thành phần để tự động xuất bản các mẫu email tương thích tốt với nhiều thiết bị (responsive). Trải nghiệm [bản demo trực tuyến](https://mail-studio-black.vercel.app/). (Đóng góp từ [@wzc520pyfm](https://github.com/ruanyf/weekly/issues/8851))

10. [TermClean](https://github.com/daijinhai/TermClean)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012815.webp)

Ứng dụng mã nguồn mở dành cho macOS, giúp quét hiển thị dung lượng ổ cứng bị chiếm dụng bởi các gói phần mềm cài đặt qua terminal và cung cấp tính năng gỡ bỏ dọn dẹp bộ nhớ nhanh. (Đóng góp từ [@daijinhai](https://github.com/ruanyf/weekly/issues/8852))

## AI 相关

1. **Bộ chuyển đổi định dạng tài liệu sang có dạng sách nói (ebook2audiobook)**

Công cụ mã nguồn mở hỗ trợ người dùng tự động chuyển đổi các định dạng tệp tin sách điện tử (ebook) thông dụng sang định dạng sách nói (audiobook) bằng AI.

2. [WorkAny](https://github.com/workany-ai/workany)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012308.webp)

Trình khách chạy desktop mã nguồn mở cho phép thiết lập và quản lý các AI Agents để tự động thực thi các tác vụ xử lý tệp tin và công việc trên máy tính, tính năng tương tự như bản thử nghiệm Claude Cowork của Anthropic. (Đóng góp từ [@idoubi](https://github.com/ruanyf/weekly/issues/8805))

3. [Voice Key](https://github.com/BuildWithAIs/voicekey)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012305.webp)

Công cụ mã nguồn mở chạy trên máy tính hỗ trợ nhận diện và chuyển đổi nhanh giọng nói trực tiếp sang định dạng văn bản bằng công nghệ AI. (Đóng góp từ [@yexia553](https://github.com/ruanyf/weekly/issues/8780))

4. [Phân cảnh video tự động bằng AI (分镜大师)](https://github.com/BroderQi/Storyboard)

Ứng dụng mã nguồn mở chạy trên hệ điều hành Windows hỗ trợ người dùng tự động phân tách các cảnh quay trong video (storyboard) bằng công nghệ trí tuệ nhân tạo. (Đóng góp từ [@BroderQi](https://github.com/ruanyf/weekly/issues/8819))

## 资源

1. [Khóa học thực chiến Claude Code (Claude Code in Action)](https://anthropic.skilljar.com/claude-code-in-action)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012401.webp)

Chương trình đào tạo hướng dẫn sử dụng công cụ Claude Code chính thức và hoàn toàn miễn phí do Anthropic phát hành, bao gồm 15 bài học dạng video ngắn với tổng thời lượng khoảng 1 giờ.

2. [Tự thiết kế chứng nhận hoạt động đóng góp GitHub cá nhân](https://certificate.brendonmatos.com/)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012303.webp)

Dịch vụ web hỗ trợ người dùng tự động kết xuất toàn bộ dữ liệu hoạt động đóng góp (contributions) của tài khoản GitHub trong năm 2025 thành một bức ảnh chứng chỉ danh dự đẹp mắt.

3. [Nhận diện phông chữ tự động (Fontsniff)](https://fontsniff.com/zh/font-identification)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012502.webp)

Công cụ trực tuyến hỗ trợ người dùng tải lên hình ảnh chứa văn bản để hệ thống tự động quét và phân tích chính xác tên phông chữ (font) đang được sử dụng. (Đóng góp từ [@cosmicqbit](https://github.com/ruanyf/weekly/issues/8822))

4. [Bảng tuần hoàn hóa học tương tác sinh động (Future Style Periodic Table)](https://github.com/SeanWong17/Future-Style-Periodic-Table)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012405.webp)

Dự án bảng tuần hoàn các nguyên tố hóa học mã nguồn mở được thiết kế theo phong cách hiện đại, hiển thị chi tiết cấu hình phân bố electron lớp ngoài cùng của từng nguyên tố. (Đóng góp từ [@SeanWong17](https://github.com/ruanyf/weekly/issues/8816))

5. [Học tiếng Nhật miễn phí (nihongo)](https://yarn.gonomad.cn/assets/word.html)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012404.webp)

Nền tảng hỗ trợ tự học tiếng Nhật trực tuyến miễn phí cung cấp đầy đủ các bài học từ vựng, luyện nghe và các bài đọc hiểu phong phú. (Đóng góp từ [@FrankZhai367](https://github.com/ruanyf/weekly/issues/8811))

## 图片

1. **Tôi không còn trực tiếp viết code nữa, tôi chuyển sang điêu khắc mã nguồn**

Phương thức lập trình dự án của tôi đã hoàn toàn thay đổi. Hiện tại tôi hầu như rất ít khi tự tay gõ từng dòng code nữa mà giao phó toàn bộ công việc cho công cụ Claude Code tự động hoàn thành.

Phần việc cốt lõi còn lại của tôi hiện nay là đóng vai trò như một người thợ điêu khắc, mài giũa và hoàn thiện các kết quả đầu ra của AI để biến chúng thành những sản phẩm ổn định và có giá trị sử dụng lâu dài.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012504.webp)

Trợ lý AI hầu như không bao giờ chủ động xóa bỏ những đoạn mã thừa thãi trong dự án. Nếu thiếu đi vai trò gọt giũa của người thợ điêu khắc con người, sản phẩm sau cùng của bạn sẽ chỉ là một khối mã nguồn cồng kềnh, thiếu bản sắc, nặng nề đến mức không thể vận hành ổn định và không truyền tải được bất kỳ giá trị cốt lõi nào.

2. **Dự án tranh tường hình bướm nghệ thuật**

Một nghệ sĩ người Pháp đã thực hiện việc vẽ các bức tranh tường khổng lồ mô tả các tiêu bản cánh bướm sống động như thật trên các bức tường tòa nhà lớn ở khắp nơi trên thế giới nhằm kêu gọi cộng đồng chung tay bảo vệ sự đa dạng sinh học của Trái Đất.

Dưới đây là các bức ảnh chụp thực tế công trình nghệ thuật của anh chứ hoàn toàn không phải là các bức ảnh do AI dựng nên:

Tác phẩm tại Miami, Mỹ:

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070509.webp)

Tác phẩm tại Houston, Mỹ:

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070511.webp)

Tác phẩm tại Tây Ban Nha:

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070512.webp)

Tác phẩm tại New York, Mỹ:

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070513.webp)

Tác phẩm tại Pháp:

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070514.webp)

## 文摘

1. **Tại sao một số công ty chấp nhận áp dụng mô hình "lập trình hộp đen"**

Trên thị trường hiện nay, có một số doanh nghiệp nhỏ đã chuyển giao toàn bộ quy trình lập trình phần mềm cho AI vận hành, họ hầu như không bao giờ đọc rà soát lại mã nguồn mà trực tiếp đưa code do AI viết ra vào vận hành ở môi trường thực tế.

Tôi gọi mô hình này là "**lập trình hộp đen (black-box programming)**". Toàn bộ tiến trình phát triển phần mềm được ẩn kín bên trong một chiếc hộp đen mà hoàn toàn không cần, thậm chí không hoan nghênh sự can thiệp thủ công của con người. Nhiệm vụ của hệ thống là tự động chuyển đổi các yêu cầu thông số kỹ thuật đầu vào thành một sản phẩm phần mềm hoàn chỉnh chạy được.

Tôi biết có một số startup nhỏ quy mô nhân sự dưới 5 người đang vận hành hoàn toàn theo mô hình này. Dù nghe có vẻ khó tin ở thời điểm hiện tại nhưng rất có thể đây chính là tương lai phát triển chung của ngành phần mềm.

Tôi đã thử liên hệ hỏi một nhà quản lý của startup đó lý do tại sao họ lại quyết định lựa chọn mô hình mạo hiểm như vậy?

Anh ấy giải thích rằng đối với một startup quy mô siêu nhỏ, mục tiêu tối thượng hàng đầu của đội ngũ là nhanh chóng chứng minh được tính hiệu quả thực tế của sản phẩm trên thị trường (MVP).

Vai trò của con người lúc này là tập trung thiết kế kiến trúc hệ thống: tìm kiếm các mô hình hoạt động tối ưu, hỗ trợ AI vận hành hiệu quả nhất để bảo đảm sản phẩm phần mềm xây dựng nên chạy ổn định. Toàn bộ các phần việc viết mã nguồn còn lại được giao khoán hoàn toàn cho AI để đạt được hiệu suất công việc cao nhất.

Dưới góc nhìn của tôi, lời giải thích này là hoàn toàn thuyết phục.

Mặc dù quy mô nhân sự rất nhỏ nhưng họ chỉ mất vỏn vẹn vài tháng để phát hành một sản phẩm vận hành tốt ra thị trường. Đặc biệt trong đội ngũ của họ có những nhân sự sở hữu hơn 20 năm kinh nghiệm phát triển các hệ thống có yêu cầu độ tin cậy và an toàn cực cao, điều đó chứng minh quyết định lựa chọn mô hình "lập trình hộp đen" của họ hoàn toàn là một chiến lược có tính toán kỹ lưỡng chứ không phải là sự liều lĩnh do thiếu kiến thức chuyên môn.

Tôi rất mong chờ được chứng kiến thời điểm sản phẩm hoàn thiện sau cùng của họ chính thức ra mắt thị trường.

## 言论

1.

Đa số các tổ chức công nghệ hiện nay luôn duy trì một phản xạ tự nhiên: ngay khi hệ thống phát sinh cảnh báo lỗi (alert), câu hỏi đầu tiên họ đưa ra luôn là: "Ai vừa mới thực hiện deploy bản cập nhật code?". Người ta mặc định rằng kỹ sư nhấn nút merge code bắt buộc phải thấu hiểu nguyên lý vận hành của đoạn code đó và sở hữu khả năng sửa lỗi nhanh chóng.

Thế nhưng kịch bản sẽ ra sao nếu đoạn code bạn vừa deploy lên môi trường production hoàn toàn không phải do con người viết ra và cũng không có bất kỳ nhân sự nào trong team thực sự hiểu rõ nguyên lý hoạt động của nó?

-- Trích đoạn bài viết [《Hai mươi năm thực hành DevOps》](https://www.honeycomb.io/blog/you-had-one-job-why-twenty-years-of-devops-has-failed-to-do-it)

2.

Các công cụ như JavaDoc có khả năng tự động trích xuất mã nguồn để sinh tài liệu kỹ thuật. Tuy nhiên theo đánh giá cá nhân tôi, những tài liệu tự sinh tự động này không mang lại nhiều giá trị thực tế, và việc đọc chúng đôi khi còn khó hiểu hơn là trực tiếp đọc mã nguồn dự án.

Không có bất kỳ công cụ tự động nào có khả năng thay thế được giá trị của những tài liệu kỹ thuật được biên soạn thủ công, có cấu trúc khoa học và được biên tập chu đáo bởi con người.

-- Trích đoạn bài viết [《Thế nào là một tài liệu chất lượng và hướng dẫn biên soạn》](https://stevelosh.com/blog/2013/09/teach-dont-tell/)

3.

Mỗi ngôn ngữ lập trình và công nghệ bạn từng dành thời gian học hỏi và sử dụng trong đời, ngay cả khi chúng đã bị thị trường đào thải và lỗi thời, vẫn luôn mang lại những giá trị vô hình to lớn. Chúng giúp củng cố tư duy và giúp việc tiếp cận ngôn ngữ hay công nghệ tiếp theo của bạn trở nên dễ dàng hơn nhiều.

-- [《Họ đã lừa bạn đấy, phát triển phần mềm thực sự là công việc rất khó khăn》](https://toddle.dev/blog/they-lied-to-you-building-software-is-really-hard)

4.

Sau một thời gian dài quen thuộc với việc lập trình bằng AI, một ngày nọ tôi bỗng bàng hoàng nhận ra bản thân đã rơi vào một cái bẫy vô cùng nguy hiểm.

Tôi phát hiện ra mình đã trở nên hoàn toàn xa lạ với chính kho mã nguồn dự án của mình và mất đi sự kiên nhẫn để tự tìm lỗi sửa code. Chỉ cần có sự đồng hành của trợ lý AI, tôi luôn có cảm giác phấn chấn, ngỡ rằng bản thân đang trở nên thông minh hơn, làm việc hiệu quả hơn và làm chủ mọi thứ. Nhưng ngay khi ngắt kết nối với AI, tôi mới bừng tỉnh phát hiện ra tất cả những cảm giác đó thực chất chỉ là một bức màn ảo ảnh do công nghệ tạo nên.

-- [《Có sự hỗ trợ của AI, tôi bỗng trở nên lười biếng và khờ khạo hơn》](https://thomasorus.com/i-tried-coding-with-ai-i-became-lazy-and-stupid)

## 往年回顾

[Trước làn sóng AI, mạng Internet truyền thống đang dần suy tàn](https://www.ruanyifeng.com/blog/2025/02/weekly-issue-336.html) (#336)

[Giải pháp xử lý ô nhiễm ánh sáng từ đèn LED chỉ thị màu xanh](https://www.ruanyifeng.com/blog/2024/01/weekly-issue-286.html) (#286)

[Những vùng đất ngập tràn ánh nắng ấm áp tại Trung Quốc](https://www.ruanyifeng.com/blog/2022/12/weekly-issue-236.html) (#236)

[Lợi thế khí hậu của các vùng vĩ độ thấp đi kèm cao độ lớn](https://www.ruanyifeng.com/blog/2021/12/weekly-issue-186.html) (#186)

(Hết)
