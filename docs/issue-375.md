# Bản tin chia sẻ công nghệ (Số 375): Lỗi bug kinh điển của một cánh cửa

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/8003) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112516.webp)

Bảo tàng Nghệ thuật Đương đại Tô Châu sắp sửa mở cửa đón khách tham quan. Thiết kế phần mái của 10 phòng triển lãm được kết nối liền mạch với nhau, lấy cảm hứng từ cấu trúc mái ngói lượn sóng đặc trưng của các ngôi nhà truyền thống vùng Giang Nam. ([via](https://www.archiposition.com/items/29335ee2bf))

## 一扇门的 Bug

Bạn đã từng nghe nói về những lỗi phần mềm (bug) kỳ lạ nhất trong lịch sử chưa?

[Trường hợp dưới đây](https://mastodon.gamedev.place/@TomF/115589875974658415) là lỗi tôi vừa bắt gặp tuần này, và nó hoàn toàn xứng đáng xếp vào danh sách top 10 lỗi kinh điển nhất mọi thời đại.

Tôi xin dịch lại câu chuyện dưới ngôi kể thứ nhất để chia sẻ cùng các bạn:

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112518.webp)

Vào năm 2013, tôi đang làm nhà phát triển game tại công ty Valve.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112201.webp)

Thời điểm đó, chiếc kính thực tế ảo VR thế hệ đầu tiên là Oculus DK1 vừa mới chính thức mở bán. Ban lãnh đạo công ty đã quyết định thử nghiệm đưa các tựa game sẵn có lên nền tảng VR này, và giao cho tôi nhiệm vụ nghiên cứu môi trường lập trình game VR.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112202.webp)

Tôi quyết định lựa chọn tựa game bắn súng kinh điển do chính Valve phát triển vào năm 2004 là 《Half-Life 2》 để tiến hành chuyển đổi.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112203.webp)

Sau khi chạy thử nghiệm thành công một phân đoạn nhỏ với hiệu ứng hình ảnh vô cùng ấn tượng, chúng tôi quyết định chuyển đổi toàn bộ trò chơi và đăng tải trailer giới thiệu dự án.

Trong suốt quá trình phát triển, tôi đã chạy thử rất nhiều phân cảnh riêng lẻ nhưng chưa từng chơi liền mạch toàn bộ tựa game từ đầu đến cuối một lần nào.

Trước ngày phát hành chính thức, tôi quyết định tự mình trải nghiệm toàn bộ trò chơi một lượt để kiểm tra xem còn vấn đề gì tồn đọng và ghi chú lại trong phần Release Notes.

Tôi tự nhủ thầm chắc chắn sẽ không có vấn đề gì lớn xảy ra, bởi đây là tựa game đã ra mắt được 10 năm với hàng triệu game thủ trải nghiệm và nhận được phản hồi cực kỳ tốt.

Thế nhưng, tôi hoàn toàn không thể ngờ rằng mình lại vấp phải một lỗi nghiêm trọng khiến game không thể chơi tiếp.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112205.webp)

Lỗi xuất hiện ngay ở phân cảnh mở đầu game: người chơi di chuyển tới ga tàu hỏa, và được một tên lính canh hướng dẫn đi vào căn phòng phía trước. Nhưng kỳ lạ thay, cánh cửa căn phòng lại đóng chặt. Nhân vật của bạn không thể bước vào trong và bị mắc kẹt hoàn toàn tại đây.

Bạn không bị chết, nhưng cũng không thể di chuyển đi đâu được. Cánh cửa phía trước khóa chặt, còn cánh cửa lớn phía sau lưng bạn cũng tự động đóng sập lại ngay khi bạn bước vào hành lang. Bạn bị nhốt trong một hành lang hẹp cùng một tên lính canh mà không có lối thoát. Thật sự vô cùng khó hiểu.

Theo đúng cốt truyện của game, bạn bắt buộc phải đi vào căn phòng này mới có thể kích hoạt các phân cảnh tiếp theo. Khi bạn quay lại nói chuyện với tên lính canh, hắn chỉ đơn thuần chỉ tay về phía cánh cửa đang khóa chặt mà không làm gì thêm.

Tôi lên mạng tìm các video gameplay của Half-Life 2 để xem lại vì sợ trí nhớ của mình bị nhầm lẫn. Kết quả hiển thị rõ ràng: cánh cửa đó đáng lẽ phải tự động mở ra khi bạn bước tới để bạn đi qua, nhưng hiện tại nó lại đóng chặt!

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112206.webp)

Tôi nghĩ thầm quả này hỏng rồi, dự án phát hành game VR coi như phải hoãn lại.

Tôi lập tức liên hệ với các đồng nghiệp khác, bao gồm cả những kỹ sư kỳ cựu từng tham gia phát triển tựa game này từ 10 năm trước. Họ tiến hành chạy thử nghiệm và xác nhận lỗi này thực sự tồn tại, thậm chí lỗi xuất hiện trên cả phiên bản chạy chế độ thường (không phải VR), cánh cửa vẫn đóng chặt. Do đó lỗi này chắc chắn không phải do quá trình chuyển đổi VR của tôi làm hỏng. Nhưng ngặt nỗi không ai biết nguyên nhân vì sao, bởi mã nguồn của game đã không hề bị chỉnh sửa suốt nhiều năm qua.

Một kỹ sư thậm chí đã tìm lại mã nguồn gốc của game từ 10 năm trước, tiến hành compile (biên dịch) lại nguyên bản game thời điểm phát hành năm 2004 – kết quả thật bất ngờ: phiên bản gốc đó hiện tại cũng bị lỗi tương tự và cánh cửa vẫn đóng chặt.

Làm sao chuyện này có thể xảy ra được? Mọi người bắt đầu hoang mang. Điều này đồng nghĩa với việc lỗi này thực chất đã nằm sẵn trong game từ 10 năm trước, nhưng tại sao khi compile thời điểm đó game lại chạy bình thường, còn hiện tại compile lại thì lỗi lại xuất hiện? Rốt cuộc chuyện gì đang diễn ra?

Sau gần một ngày ròng rã sử dụng lại các công cụ debug và giả lập hệ thống từ thời kỳ đó, một đồng nghiệp đã tìm ra câu trả lời.

Khi quan sát kỹ chuyển động trong game, chúng tôi phát hiện ra cánh cửa này thực chất đã tự động mở ra trong một khoảnh khắc cực ngắn. Tuy nhiên, ngay phía sau cánh cửa có một tên lính canh thứ hai đang đứng gác. Tên lính này đứng quá sát cánh cửa, khiến cánh cửa khi vừa mở ra đã chạm nhẹ vào ngón chân của hắn và lực va chạm khiến cánh cửa bật ngược trở lại, tự động đóng sập và khóa chặt lại. Do trò chơi không được thiết kế kịch bản xử lý mở lại cửa cho tình huống va chạm này, người chơi sẽ bị kẹt lại vĩnh viễn ngoài hành lang.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112207.webp)

Sau khi hiểu rõ nguyên lý lỗi, giải pháp khắc phục cực kỳ đơn giản: chúng tôi chỉ cần chỉnh sửa dịch chuyển vị trí đứng của tên lính canh lùi lại phía sau khoảng 1 milimét, cánh cửa lập tức tự động mở ra trơn tru.

Mọi việc coi như đã được giải quyết để chuẩn bị phát hành. Nhưng câu hỏi lớn nhất vẫn chưa có lời đáp: Tại sao 10 năm trước tựa game gốc lại không bị lỗi này, dù ngón chân của tên lính canh vẫn đứng ở vị trí đó? Tại sao compile lại sau 10 năm thì lỗi mới bộc phát? Nói cách khác, lỗi vốn luôn nằm sẵn ở đó, nhưng điều gì đã giúp cánh cửa không bị đóng sập vào 10 năm trước?

Một cuộc tìm kiếm nguyên nhân chuyên sâu lại tiếp tục được triển khai.

Cuối cùng, chúng tôi đã phát hiện ra thủ phạm – một chủ đề kinh điển trong khoa học máy tính: **Phép toán số thực dấu phẩy động (floating-point operations)**.

Tựa game Half-Life 2 ra mắt năm 2004 được compile bằng các tập lệnh toán học thế hệ cũ là x87/8087. Độ chính xác của các số thực dấu phẩy động trong tập lệnh này rất không đồng đều: có đoạn mã sử dụng 32-bit, có đoạn dùng 64-bit, có đoạn lại dùng 80-bit. Các phần mã nguồn khác nhau hoạt động trên các độ chính xác khác nhau.

Đến năm 2013, tập lệnh SSE đã trở thành tiêu chuẩn mặc định trên các dòng CPU kiến trúc x86. Trình biên dịch mặc định chuyển sang sử dụng SSE với độ chính xác số thực dấu phẩy động được quy định rõ ràng 32-bit hoặc 64-bit tùy theo mã nguồn, giúp kết quả tính toán có tính nhất quán cao.

Sự thật là: bản game biên dịch 10 năm trước sử dụng độ chính xác số thực dấu phẩy động 32-bit cho phân đoạn đó, còn trình biên dịch mới năm 2013 lại sử dụng 64-bit. Sự sai lệch cực kỳ nhỏ ở phần thập phân đã tạo ra khoảng cách chênh lệch vài milimét trong việc dựng hình không gian, vừa đủ khiến ngón chân của tên lính canh chạm trúng cánh cửa đang mở.

Sau khi sửa lỗi, giờ đây game thủ đã có thể thoải mái bước qua cánh cửa ga tàu hỏa để tiếp tục hành trình khám phá thế giới game.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112208.webp)

## 科技动态

1. **Giảng dạy bằng AI**

Sinh viên tại trường Đại học Staffordshire ở Anh vừa lên tiếng khiếu nại với cơ quan truyền thông.

Trong các buổi lên lớp của họ, hệ thống slide trình chiếu của giảng viên (hình dưới) hoàn toàn được tạo bằng AI, thậm chí giảng viên còn không trực tiếp đứng lớp giảng bài mà chỉ phát các file âm thanh bài giảng do AI tổng hợp giọng nói.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112102.webp)

Các sinh viên vô cùng phẫn nộ bởi theo quy định của nhà trường, nếu sinh viên nộp các bài tập làm bằng AI sẽ lập tức bị đuổi học, nhưng chính các giảng viên lại đang sử dụng AI để dạy học.

Sự việc này một mặt phản ánh chất lượng giáo dục đại học tại Anh đang ngày càng đi xuống, mặt khác cũng khiến dư luận phải suy ngẫm: Nếu các trường đại học lạm dụng AI để dạy học, hoặc chất lượng đứng lớp của giảng viên còn thua kém cả trợ lý AI, liệu sinh viên có còn cần thiết phải đến trường nữa không, tại sao họ không tự học trực tiếp qua AI?

2. **Xe lăn dạng cua**

Toyota vừa giới thiệu mẫu sản phẩm ý tưởng: chiếc xe lăn có khả năng di chuyển linh hoạt như loài cua.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111217.webp)

Bốn chiếc chân của xe có khả năng cử động linh hoạt nhờ hệ thống động cơ điều khiển khớp nối. Người dùng ngồi lên trên và chiếc xe sẽ tự động bước đi, thậm chí có khả năng leo bậc cầu thang dễ dàng.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111219.webp)

Thiết bị còn có thể hạ thấp trọng tâm nằm sát đất hoặc nâng cao thẳng đứng.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111220.webp)

Tôi dự báo các doanh nghiệp sẽ sớm ra mắt các dòng sản phẩm robot di chuyển tương tự. Thị trường dành cho các thiết bị robot hỗ trợ chở người đi lại này hứa hẹn sẽ vô cùng rộng mở.

3. **Máy tính lượng tử**

Văn phòng của IBM tại London hiện đang trưng bày một hệ thống máy tính lượng tử thực tế.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112503.webp)

Hệ thống này được chế tạo vào năm 2019 và hiện tại đã lỗi thời. Tuy nhiên, khách tham quan không được phép vào sát bên trong văn phòng mà chỉ có thể đứng quan sát từ xa ở khu vực cửa ra vào.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112506.webp)

Công nghệ này được kỳ vọng là tương lai của ngành máy tính, sở hữu khả năng bẻ khóa cực nhanh các thuật toán mã hóa hiện nay. Tuy nhiên, trong quá trình hoạt động, hệ thống yêu cầu môi trường làm mát siêu lạnh cận kề độ không tuyệt đối, do đó không thể ứng dụng sử dụng trong gia đình.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112504.webp)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112505.webp)

4. **Chi phí xây dựng trang web chính phủ**

Để xây dựng một trang web chính phủ thì cần tiêu tốn bao nhiêu chi phí? Câu trả lời là 96,5 triệu đô la Úc (tương đương khoảng 450 triệu Nhân dân tệ / 1.600 tỷ VNĐ).

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112514.webp)

Trang web mới của Cục Khí tượng Úc có chi phí thiết kế là 4,1 triệu AUD, chi phí phát triển lập trình là 79,8 triệu AUD, và chi phí phát hành kèm thử nghiệm bảo mật là 12,6 triệu AUD, nâng tổng mức đầu tư lên tới 96,5 triệu AUD.

Do vượt quá xa so với mức dự toán ban đầu là 4,1 triệu AUD, thương vụ này sau khi bị báo chí phanh phui đã tạo nên làn sóng phẫn nộ trong công luận.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112515.webp)

Đáng cười hơn nữa là sau khi trang web mới được đưa vào vận hành, nhiều nông dân phản ánh họ không thể tìm thấy số liệu lượng mưa cần thiết, buộc cơ quan này phải mở lại trang web phiên bản cũ để phục vụ người dân.

Việc làm sao để các hệ thống công nghệ thông tin của chính phủ hoạt động hiệu quả, dễ dùng mà không gây lãng phí tiền thuế của người dân thực sự là một bài toán hóc búa.

Các bạn có thể truy cập trải nghiệm trang web này tại địa chỉ [bom.gov.au](https://www.bom.gov.au/). Ngoài ra trang web phiên bản cũ tại địa chỉ [reg.bom.gov.au](https://reg.bom.gov.au/) hiện vẫn đang tiếp tục duy trì hoạt động trực tuyến.

## 文章

1. [Tại sao các hệ quản trị cơ sở dữ liệu đều sử dụng cấu trúc cây B-Tree](https://mehmetgoekce.substack.com/p/b-trees-why-every-database-uses-them) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112401.webp)

Bài viết phân tích và giải thích chi tiết lý do tại sao cấu trúc dữ liệu cây tìm kiếm B-Tree lại tối ưu cho việc tổ chức và truy vấn cơ sở dữ liệu hơn so với cấu trúc cây nhị phân (Binary Tree) thông thường.

2. [Tại sao việc đánh giá, kiểm thử các mô hình AI mới ngày càng khó khăn](https://simonwillison.net/2025/Nov/24/claude-opus/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112508.webp)

Lập trình viên nổi tiếng Simon Willison chia sẻ góc nhìn về việc anh hầu như không thể tự đánh giá được năng lực của các mô hình ngôn ngữ lớn thế hệ mới hiện nay. Bởi năng lực của các mô hình AI mới đã trở nên quá mạnh mẽ, các bài toán kiểm thử thông thường đều được chúng giải quyết dễ dàng, buộc người kiểm thử phải thiết kế những câu hỏi chuyên sâu và hóc búa hơn rất nhiều.

3. [Ổ cứng SSD sẽ bị mất dữ liệu nếu không được cắm điện trong thời gian dài](https://www.xda-developers.com/your-unpowered-ssd-is-slowly-losing-your-data/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112509.webp)

Bài viết chỉ ra điểm hạn chế vật lý của các dòng ổ cứng thể rắn (SSD) phân khúc phổ thông: nếu để ổ cứng trong tình trạng không được cấp điện quá 1 năm, dữ liệu lưu trữ bên trong sẽ bắt đầu bị rò rỉ và mất mát.

Hiện tại, ngay cả những dòng SSD cao cấp nhất cũng không thể duy trì dữ liệu quá 10 năm nếu hoàn toàn không được cấp điện. Do đó, nếu cần lưu trữ dữ liệu lâu dài dưới dạng lưu trữ lạnh, bạn không nên sử dụng ổ cứng SSD.

4. [Bài test hiệu năng vi xử lý Loongson 3A6000 của Trung Quốc](https://lemire.me/blog/2025/11/23/how-good-are-chinese-cpus-benchmarking-the-loongson-3a6000/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112522.webp)

Một lập trình viên nước ngoài tiến hành các bài kiểm tra hiệu năng thực tế đối với dòng vi xử lý nội địa Loongson 3A6000 của Trung Quốc để so sánh với dòng chip Intel Xeon Gold 6338 ra mắt năm 2021.

5. [Tại sao một đường dẫn URL nằm trong mã nguồn C vẫn có thể compile bình thường?](https://susam.net/url-in-c.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112706.webp)

Bài viết giải thích một hiện tượng thú vị trong lập trình C: khi chèn trực tiếp một đường dẫn URL vào mã nguồn, trình biên dịch vẫn chạy và compile bình thường mà không báo lỗi cú pháp.

6. [Hướng dẫn tự xây dựng một công cụ tìm kiếm đơn giản](https://karboosx.net/post/4eZxhBon/building-a-simple-search-engine-that-actually-works) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112602.webp)

Bài viết giới thiệu nguyên lý hoạt động cơ bản của các công cụ tìm kiếm trực tuyến và hướng dẫn từng bước lập trình để xây dựng một bộ máy tìm kiếm đơn giản của riêng bạn.

7. [Tự lắp ráp hệ thống lưu trữ mạng NAS: Phiên bản 2026](https://blog.briancmoses.com/2025/11/diy-nas-2026-edition.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112708.webp)

Tác giả chia sẻ chi tiết cấu hình phần cứng và quy trình tự xây dựng một hệ thống NAS lưu trữ dữ liệu gia đình chất lượng, tài liệu tham khảo tốt cho những ai có ý định tự lắp đặt.

## 工具

1. [DNS Benchmark Tool](https://github.com/frankovo/dns-benchmark-tool)

Công cụ dòng lệnh hỗ trợ kiểm tra và đo lường hiệu năng của các máy chủ DNS, đo độ trễ kết nối từ máy khách đến DNS server và thời gian thực hiện phân tích cú pháp tên miền ra địa chỉ IP.

2. [iDescriptor](https://github.com/iDescriptor/iDescriptor)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112405.webp)

Ứng dụng quản lý thiết bị đa nền tảng chạy trên máy tính, hỗ trợ kết nối và quản lý dữ liệu trên điện thoại iPhone.

3. [SVG.js](https://svgjs.dev)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112406.webp)

Thư viện JavaScript gọn nhẹ hỗ trợ lập trình viên xây dựng và thao tác trực tiếp với các hình ảnh vector động định dạng SVG trên trang web.

4. [impala](https://github.com/pythops/impala)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112303.webp)

Ứng dụng giao diện dòng lệnh (TUI) hỗ trợ quản lý và kết nối mạng WiFi trên các hệ điều hành Linux.

5. [2025-blog-public](https://github.com/YYsuni/2025-blog-public)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112106.webp)

Mẫu giao diện thiết kế trang blog tĩnh phát triển dựa trên nền tảng Next.js. (Đóng góp từ [@YYsuni](https://github.com/ruanyf/weekly/issues/8262))

6. [pdfpc-ts](https://github.com/Master-Hash/pdfpc-ts)

Dịch vụ web mã nguồn mở hỗ trợ trình diễn slide tài liệu PDF trực tuyến, tích hợp giao diện hiển thị ghi chú riêng cho người thuyết trình tương tự ứng dụng [pdfpc](https://github.com/pdfpc/pdfpc). (Đóng góp từ [@Master-Hash](https://github.com/ruanyf/weekly/issues/8264))

7. [Clip-Save (剪存)](https://github.com/snsogbl/clip-save)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112302.webp)

Phần mềm mã nguồn mở chạy trên máy tính Windows và macOS hỗ trợ ghi lại và quản lý lịch sử sao chép bộ nhớ tạm (clipboard). (Đóng góp từ [@snsogbl](https://github.com/ruanyf/weekly/issues/8269))

8. [Hoa](https://github.com/hoa-js/hoa)

Thư viện framework máy chủ Web JavaScript gọn nhẹ lấy cảm hứng thiết kế từ Koa và Hono, được tối ưu hóa chuyên biệt chạy trên Cloudflare Workers. (Đóng góp từ [@nswbmw](https://github.com/ruanyf/weekly/issues/8289))

9. [NodeBBS](https://github.com/aiprojecthub/nodebbs)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112701.webp)

Hệ thống diễn đàn thảo luận mã nguồn mở hiện đại phát triển hoàn toàn bằng ngôn ngữ JavaScript. (Đóng góp từ [@wengqianshan](https://github.com/ruanyf/weekly/issues/8294))

10. [MyTube](https://github.com/franklioxygen/MyTube)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112704.webp)

Dịch vụ web tự lưu trữ (self-hosted) hỗ trợ tải xuống và quản lý video từ hai nền tảng lớn là YouTube và Bilibili. (Đóng góp từ [@franklioxygen](https://github.com/ruanyf/weekly/issues/8300))

## AI 相关

1. [WeFinance-Copilot](https://github.com/JasonRobertDestiny/WeFinance-Copilot)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112301.webp)

Ứng dụng web mã nguồn mở hỗ trợ tải lên các tệp hóa đơn tiêu dùng để AI tự động nhận diện thông tin và thực hiện phân tích tình hình tài chính cá nhân. (Đóng góp từ [@JasonRobertDestiny](https://github.com/ruanyf/weekly/issues/8270))

2. [KoalaQA](https://github.com/chaitin/KoalaQA)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112502.webp)

Hệ thống chăm sóc khách hàng bằng AI mã nguồn mở, hỗ trợ xây dựng các cổng hỏi đáp thông minh, trang cộng đồng hỗ trợ kỹ thuật cho nhà phát triển và người dùng. (Đóng góp từ [@Trc0g](https://github.com/ruanyf/weekly/issues/8286))

3. [seekdb](https://github.com/oceanbase/seekdb)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112521.webp)

Dòng cơ sở dữ liệu tích hợp trí tuệ nhân tạo (AI Database) mã nguồn mở do đội ngũ OceanBase phát hành, hỗ trợ lưu trữ và tính toán vector tương thích tốt với MySQL. (Đóng góp từ [@liboyang0730](https://github.com/ruanyf/weekly/issues/8288))

4. [OPENUGC](https://chat.openugc.com)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112703.webp)

Ứng dụng khách Web client tích hợp nhiều tính năng AI, hỗ trợ người dùng tự cấu hình kết nối mô hình lớn, Agent và cổng giao tiếp MCP. Dự án cung cấp đầy đủ tính năng nhưng không mở nguồn mở. (Đóng góp từ [@aicu-icu](https://github.com/ruanyf/weekly/issues/8298))

## 资源

1. [Hướng dẫn chi tiết về khung phát triển Agent: LangGraph 1.0](https://www.luochang.ink/dive-into-langgraph/quickstart/)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112501.webp)

LangGraph là khung công nghệ nguồn mở phát triển AI Agent. Tài liệu hướng dẫn được thiết kế trực quan dưới dạng các tệp Jupyter Notebook tương tác thực tế giúp nhà phát triển dễ dàng tiếp cận. (Đóng góp từ [@luochang212](https://github.com/ruanyf/weekly/issues/8283))

2. [Tổng hợp từ khóa gợi ý Nano Banana Pro Prompts](https://github.com/YouMind-OpenLab/awesome-nano-banana-pro-prompts/blob/main/README_zh.md)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112702.webp)

Kho lưu trữ tổng hợp hơn 500 từ khóa gợi ý (prompt) dành riêng cho mô hình Nano Banana Pro. Mỗi từ khóa đều đi kèm hình ảnh minh họa thực tế và hơn một nửa số prompt có đính kèm thông số cấu hình chi tiết. (Đóng góp từ [@DophinL](https://github.com/ruanyf/weekly/issues/8297))

3. [OCR Arena](https://www.ocrarena.ai)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112507.webp)

Trang web xếp hạng đánh giá năng lực nhận diện ký tự quang học (OCR) của các mô hình AI lớn hiện nay theo phương thức đối đầu trực tiếp, hiện dòng mô hình Gemini 3 đang dẫn đầu bảng xếp hạng.

## 图片

1. **Mô hình sa bàn sân bay**

Một cựu phi công người Mỹ sau khi nghỉ hưu đã dành thời gian theo đuổi đam mê chế tác các mô hình sa bàn sân bay.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112510.webp)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112511.webp)

Trang web cá nhân của ông đăng tải rất nhiều hình ảnh về các mô hình sân bay do ông tự tay thiết kế, bạn đọc có thể truy cập để xem chi tiết.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112709.webp)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112710.webp)

Dưới đây là hình ảnh sa bàn sân bay Mumbai do ông chế tác, hỗ trợ hiển thị cả hiệu ứng ánh sáng ban đêm vô cùng lung linh.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112512.webp)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112513.webp)

## 文摘

1. [Nói "Không" với những lời đề nghị xin "một chút" thời gian của bạn](https://thoughtcatalog.com/ryan-holiday/2017/01/to-everyone-who-asks-for-just-a-little-of-your-time/)

Tôi thường xuyên nhận được những lời mời kiểu như:

> - Tôi muốn hẹn gặp trao đổi nhanh với bạn một lát được không?
> - Tuần sau chúng ta cùng đi uống cà phê nhé?
> - Chúng ta cùng ngồi thảo luận một chút về chủ đề này nhé?

Câu trả lời của tôi luôn nhất quán là: Không, Không và Không.

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082212.webp)

Thực tế tôi hoàn toàn có khả năng sắp xếp thời gian để đáp ứng lời mời của bạn, nhưng tôi chọn cách không làm vậy.

Ngay cả khi đó là một cơ hội kinh doanh đầy hứa hẹn, ngay cả khi cuộc gặp chỉ tiêu tốn của tôi vỏn vẹn 15 phút, và ngay cả khi đó là việc mà hầu hết mọi người bình thường khác đều sẽ vui vẻ đồng ý tham gia, tôi vẫn chọn cách từ chối.

Tôi bắt buộc phải giới hạn tối đa khoảng thời gian bị người khác chiếm dụng trong ngày, nếu không tôi sẽ không còn thời gian dành riêng cho chính mình.

Thêm vào đó, ngay cả khi sau cuộc gặp tôi vẫn còn dư lại một chút thời gian rảnh, thì năng lượng tinh thần và sự tập trung của tôi cũng đã bị bào mòn và tôi không còn đủ tỉnh táo để tận dụng tốt khoảng thời gian còn lại đó nữa.

Thời gian là tài sản quý giá và không thể tái tạo nhất của mỗi người – chúng ta không cách nào dùng tiền để mua thêm thời gian. Chúng ta không thể lấy lại dù chỉ 1 giây đã trôi qua. Điều duy nhất có thể làm là cố gắng giảm thiểu tối đa việc lãng phí nó.

Thế nhưng trong đời sống thực tế, không hiểu vì lý do gì, nhiều người lại xem thời gian như một nguồn tài nguyên vô hạn và có khả năng tự tái tạo, tiêu tốn hết thì thôi, trước sau gì cũng sẽ có khoảng thời gian khác thế vào.

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082213.webp)

Vì vậy, nếu bạn ngỏ ý muốn hẹn gặp hay trò chuyện cùng tôi, câu trả lời sẽ là Không. Tôi hy vọng bạn có thể thấu hiểu và chia sẻ lý do đằng sau quyết định này của tôi.

## 言论

1.

Lập trình là liều thuốc hữu hiệu nhất giúp tôi kiềm chế sự kiêu ngạo của bản thân. Nếu bạn thấy ai đó quá kiêu ngạo, hãy bảo anh ta đi học lập trình.

-- Trang web [tratt.net](https://tratt.net/laurie/blog/2020/automatic_syntax_error_recovery.html)

2.

Việc huấn luyện một mô hình AI sở hữu những quan điểm độc lập và khác biệt so với số đông sẽ ngày càng gặp khó khăn. Bởi nếu quan điểm của mô hình đi chệch khỏi các dữ liệu thực tế và thế giới quan đời thực, bạn không thể đơn thuần sử dụng các tài liệu huấn luyện bên ngoài để điều chỉnh mô hình được.

-- Độc giả trên diễn đàn Hacker News

3.

Hiện tại là năm 2025, và AI đang lây lan nhanh chóng như một loại virus. Ngay cả khi bạn vẫn đang kiên trì tạo ra các tác phẩm thủ công chất lượng cao, người ta vẫn rất dễ lầm tưởng những nỗ lực lao động vất vả của bạn là các sản phẩm rác vô hồn do máy móc tự động sinh ra.

-- Trang web [tonsky.me](https://tonsky.me/blog/hiring-ai/)

4.

Cuộc đời con người quá ngắn ngủi, và cái chết có thể ập đến bất cứ lúc nào. Nếu tôi chỉ chọn cách sống buông xuôi và trôi theo dòng đời, chớp mắt một cái tôi đã trở thành một ông lão tóc bạc da mồi.

-- [Goro Obata](https://kottke.org/25/11/my-pace), Youtuber người Nhật Bản

5.

Nếu một vật dụng được thiết kế tối ưu 100% cho mục đích sử dụng thực tế của nó, vật dụng đó chắc chắn sẽ sở hữu vẻ đẹp riêng, ví dụ như chúng ta không bao giờ thấy một cây búa hay một cây đinh có hình thù xấu xí. Ngược lại, có rất nhiều mẫu xe ô tô có ngoại hình khá xấu, bởi không phải bộ phận nào trên chiếc xe cũng được thiết kế hoàn toàn phục vụ công năng thực tế.

-- Dan Gelbart, nhà phát minh công nghiệp

## 往年回顾

[Phát triển mô hình AI không phải là một mô hình kinh doanh tốt](https://www.ruanyifeng.com/blog/2024/12/weekly-issue-328.html) (#328)

[Rắc rối tranh chấp bản quyền nội dung AI](https://www.ruanyifeng.com/blog/2023/11/weekly-issue-278.html) (#278)

[Ý nghĩa của nhân loại và đời người](https://www.ruanyifeng.com/blog/2022/10/weekly-issue-228.html) (#228)

[Thời kỳ hoàng kim của điện năng lượng mặt trời gia đình](https://www.ruanyifeng.com/blog/2021/10/weekly-issue-178.html) (#178)

(Hết)
