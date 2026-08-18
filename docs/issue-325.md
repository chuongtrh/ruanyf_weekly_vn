# Bản tin chia sẻ công nghệ (Số 325): Trình soạn thảo Zed sẽ là điểm dừng chân tiếp theo sau VS Code?

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/5445) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110513.webp)

Đảo Giang Tâm thuộc Ôn Châu là một hòn đảo nhỏ nằm giữa dòng sông Âu Giang, gần đây đã hoàn thành toàn bộ dự án nâng cấp và cải tạo cảnh quan. (Nguồn: [66wz](http://4g.66wz.com/xw/system/2024/05/31/105637714.shtml))

## VS Code 编辑器的下一站是 Zed？

Lập trình viên không thể thiếu trình soạn thảo mã nguồn (editor), và công cụ phổ biến nhất hiện nay chắc chắn là VS Code.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110601.webp)

VS Code sở hữu nhiều ưu điểm vượt trội, nhưng lại tồn tại một điểm trừ rất lớn liên quan đến: **Hiệu năng**.

Do vận hành bên trong môi trường hộp cát (sandbox) của Electron, VS Code tiêu tốn rất nhiều tài nguyên phần cứng hệ thống và cho tốc độ phản hồi khá chậm. Hiện tại khi tôi thực hiện gọi một số plugin bổ sung, độ trễ hiển thị có thể cảm nhận được rất rõ ràng.

Ngoài ra, ứng dụng cũng đang ngày càng trở nên cồng kềnh hơn khi tệp cài đặt ban đầu đã nặng tới 100MB và yêu cầu khoảng không gian đĩa trống lên tới 500MB sau khi cài đặt.

Chính vì thế, ngay sau khi nghe tin về một trình soạn thảo mã nguồn thế hệ mới mang tên [Zed](https://zed.dev/) với hiệu năng xử lý vượt trội cùng bộ tính năng mạnh mẽ, tôi đã lập tức tải về cài đặt để trải nghiệm thử. Dưới đây là những đánh giá chi tiết của tôi.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110602.webp)

Đầu tiên, lý do gì đã giúp Zed thu hút sự chú ý của tôi?

(1) Tác giả sáng lập của dự án cũng chính là người đã thiết kế nên trình soạn thảo Atom danh tiếng năm xưa, đồng thời cũng là cha đẻ của thư viện phân tích cú pháp Tree-sitter được ứng dụng rộng rãi.

(2) Dự án được phát triển hoàn toàn bằng ngôn ngữ Rust, cho phép tận dụng tối đa sức mạnh xử lý đa nhân của CPU và GPU nhằm hướng tới việc tối ưu hóa hiệu năng và tốc độ xử lý nhanh nhất.

(3) Hệ thống được tích hợp sẵn rất nhiều tính năng bổ trợ của VS Code như Giao thức máy chủ ngôn ngữ (LSP), tính năng tự động gợi ý hoàn thành mã nguồn, tính năng cộng tác chỉnh sửa mã nguồn thời gian thực giữa nhiều người và tích hợp trợ lý AI thông minh.

(4) Tốc độ phát triển dự án vô cùng ấn tượng khi kho mã nguồn GitHub của Zed hiện đã cán mốc hơn 49.000 lượt yêu thích (Stars).

Sau khi cài đặt xong, giao diện đầu tiên hiện lên mang phong cách tối giản vô cùng sạch sẽ và thoáng đãng. Bố cục giao diện có nhiều nét tương đồng với VS Code nên tôi hầu như không mất thời gian học cách làm quen, có thể bắt tay viết code ngay lập tức.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110603.webp)

Tốc độ phản hồi của Zed thực sự rất đáng kinh ngạc, mọi thao tác từ mở tệp cho đến chuyển đổi tab đều diễn ra tức thì không có chút độ trễ nào. Sau một thời gian trải nghiệm Zed, khi quay trở lại sử dụng VS Code, tôi thực sự cảm thấy không còn quen với độ trễ của nó nữa.

Đại bộ phận các tính năng phục vụ lập trình cơ bản đều đã được tích hợp sẵn để dùng ngay. Nếu có nhu cầu mở rộng thêm, người dùng hoàn toàn có thể tìm kiếm tại [Cửa hàng tiện ích (Extensions Market)](https://zed.dev/extensions) của hệ thống.

Một số tính năng tích hợp sẵn được tôi đánh giá rất cao. Ví dụ như bảng quản lý cấu trúc mã nguồn (Outline Panel) ở khung bên trái (hình dưới), hỗ trợ liệt kê toàn bộ các hàm có trong tệp hiện tại để người dùng có thể nhấp chuột và di chuyển nhanh đến vị trí định nghĩa hàm đó.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110604.webp)

Ứng dụng còn hỗ trợ tính năng mời thêm cộng sự tham gia viết mã nguồn (yêu cầu tài khoản GitHub) để cùng thực hiện chỉnh sửa và trao đổi trực tuyến thời gian thực ngay trên giao diện code.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110605.webp)

Hình ảnh đại diện của các cộng sự đang cùng tham gia viết mã sẽ được hiển thị trực quan ở góc trên bên phải cửa sổ làm việc.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110606.webp)

Sở hữu những ưu điểm vượt trội kể trên, nhưng hiện tại Zed vẫn tồn tại một số hạn chế rất khó để bỏ qua:

(1) Ứng dụng chưa thực sự hỗ trợ đa nền tảng hoàn hảo. Hiện tại chỉ có phiên bản dành cho macOS là hoạt động ổn định nhất, phiên bản dành cho Linux vẫn còn phát sinh tương đối nhiều lỗi trong khi phiên bản dành cho Windows vẫn chưa được phát hành chính thức.

(2) Nhiều tính năng nhỏ vẫn chưa được hoàn thiện, người dùng thường xuyên gặp phải tình trạng thiếu hụt một vài tùy chỉnh nhỏ quen thuộc và rất khó tìm kiếm giải pháp khắc phục.

(3) Toàn bộ cấu hình cài đặt của hệ thống đều được lưu trữ dưới dạng một tệp JSON lớn và không có giao diện đồ họa điều chỉnh trực quan, buộc người dùng phải thường xuyên tra cứu tài liệu hướng dẫn mỗi khi muốn thay đổi cài đặt.

(4) Trợ lý AI tích hợp sẵn hiện tại mới chỉ hỗ trợ kết nối API với các mô hình của OpenAI, Claude hoặc mô hình chạy cục bộ thông qua Ollama.

Đánh giá tổng quan của tôi là: **Zed là một trình soạn thảo mã nguồn có chất lượng rất xuất sắc, nhưng chưa thực sự sẵn sàng cho mọi người dùng**. Ứng dụng hiện chỉ thực sự phù hợp cho những lập trình viên yêu cầu hiệu năng tốc độ xử lý cao và sẵn sàng tự mình mày mò cấu hình giải quyết các lỗi nhỏ phát sinh.

Tóm lại, **Zed là một giải pháp thay thế rất tiềm năng cho VS Code nhờ triết lý thiết kế tối giản, gọn nhẹ và tích hợp sẵn đầy đủ các tính năng cốt lõi**. Vào thời điểm này năm sau, rất có thể Zed sẽ làm cho sức hút của VS Code giảm đi đáng kể.

## ［本周软件］302.AI

Đứng trước sự ra đời của vô số các mô hình trí tuệ nhân tạo lớn nhỏ hiện nay, đã bao giờ bạn nảy ra ý tưởng: Sẽ thật tuyệt vời nếu chúng ta có **một cổng kết nối sử dụng chung duy nhất** hay không?

Thực tế ý tưởng này đã được hiện thực hóa. Bản tin trước đây đã từng giới thiệu về trang web [302.AI](https://302.ai) hoạt động theo đúng triết lý thiết kế này.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024111201.webp)

Ứng dụng được định vị là một "siêu thị ứng dụng AI", **hoạt động như một lớp cổng chuyển đổi trung gian kết nối với hàng loạt các mô hình AI khác nhau**, giúp người dùng có thể dễ dàng khai thác mọi mô hình tại một nơi duy nhất.

Bạn có thể tương tác trực tiếp với các mô hình AI thô, hoặc ứng dụng hơn 30 công cụ AI chuyên dụng được thiết lập sẵn tại [Cửa hàng công cụ (Tools Market)](https://302.ai/tools/), ví dụ như công cụ [Tìm kiếm bài báo nghiên cứu khoa học bằng AI](https://302.ai/tools/academic/).

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024111301.webp)

Trang web cũng cung cấp dịch vụ gọi API trung gian, giúp các nhà phát triển có thể gọi API của các mô hình khác nhau thông qua hệ thống máy chủ của 302.AI.

<u>Hệ thống cung cấp một hạn mức dùng thử miễn phí ban đầu, sau đó sẽ thực hiện tính phí dựa trên lượng tài nguyên sử dụng thực tế</u>, thông thường chi phí sử dụng qua đây chỉ bằng khoảng một nửa so với giá gốc của nhà cung cấp mô hình.

Đặc biệt, **tuần này dự án đã chính thức mở mã nguồn toàn bộ các công cụ giao diện của hệ thống**, mã nguồn được chia sẻ công khai tại địa chỉ [github.com/302ai](https://github.com/302ai). Các mã nguồn này được phát triển trên Next.js, rất thích hợp để làm tài liệu tham khảo cho các bạn muốn tự phát triển ứng dụng AI cho riêng mình.

## 科技动态

1、[Mô hình khối Rubik 34 tầng](https://ruwix.com/blog/34x34x34-rubiks-cube-record/)

Các khối Rubik thông thường có cấu trúc 3 tầng (3x3x3), tức mỗi chiều có 3 ô màu, nhưng thực tế cũng có các khối Rubik nhiều tầng hơn.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110203.webp)

Hình ảnh trên là các khối Rubik cấu trúc 2 tầng, 4 tầng và 5 tầng.

Mới đây, một nhà thiết kế đã ứng dụng công nghệ in 3D để chế tạo thành công khối Rubik có số tầng lớn nhất thế giới hiện nay, lên tới 34 tầng (34x34x34).

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110204.webp)

Với kích thước khổng lồ như vậy, việc xoay chuyển các ô màu trên khối Rubik này là cực kỳ khó khăn và bất tiện. Thiết bị hoàn toàn không phù hợp để chơi giải trí thông thường, mà chủ yếu dùng để tạo hình các khối màu nghệ thuật độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110205.webp)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110206.webp)

Cùng với sự phổ cập của công nghệ in 3D, việc chế tạo các khối Rubik có số tầng lớn hơn nữa là hoàn toàn khả thi, nhưng chúng không mang nhiều giá trị thực tiễn. Hiện tại, khối Rubik lớn nhất được sản xuất thương mại đại trà trên thị trường là loại 17 tầng.

2、[Đồng hồ đo độ trễ mạng (Ping Clock)](https://github.com/turingbirds/ping-clock)

`ping` là một công cụ dòng lệnh cơ bản được dùng để đo lường tốc độ phản hồi và thời gian truyền tải gói tin từ máy tính đến máy chủ mạng.

Một lập trình viên nước ngoài đã nảy ra ý tưởng chế tạo một chiếc đồng hồ vật lý hiển thị trực quan thông số ping mạng này trên mặt đồng hồ.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110804.webp)

Mặt đồng hồ được thiết kế với hai kim chỉ thị: Kim dài hiển thị thời gian phản hồi ping theo đơn vị mili giây (ms) hiện tại, trong khi kim ngắn ghi nhận thông số ping cao nhất trong phiên làm việc.

Phía dưới mặt đồng hồ được bố trí một màn hình LCD nhỏ để hiển thị thông tin mạng kết nối hiện tại và địa chỉ máy chủ mục tiêu đang thực hiện đo lường.

Mỗi khi máy tính chạy lệnh ping, kim dài trên mặt đồng hồ sẽ liên tục dao động phản ánh tốc độ mạng theo thời gian thực, giúp người dùng có thể dễ dàng "nhìn thấy" tốc độ mạng của mình.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110805.webp)

Toàn bộ mã nguồn và sơ đồ thiết kế phần cứng của chiếc đồng hồ này đã được chia sẻ công khai. Thiết bị sử dụng vi điều khiển ESP32 kết hợp với một động cơ bước nhỏ và bảng mạch PCB tự thiết kế. Các bạn học sinh có kiến thức cơ bản về điện tử hoàn toàn có thể tự mua linh kiện và lắp ráp cho riêng mình.

3、[Ứng dụng mới từ loài chim sẻ](https://www.abc.net.au/news/science/2024-07-18/sparrows-lead-poisoning-children-blood-levels-health-mining/104075894)

Loài chim sẻ nhỏ bé có thể giúp ích gì cho con người? Các nhà khoa học Australia mới đây đã tìm ra một giải pháp vô cùng độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072113.webp)

Australia hiện là một trong những quốc gia khai thác và xuất khẩu chì lớn nhất thế giới với 28 mỏ khai thác đang hoạt động. Kim loại chì gây độc hại nghiêm trọng cho sức khỏe con người, đặc biệt là sự phát triển của trẻ nhỏ.

Các nhà khoa học luôn tìm kiếm những giải pháp tối ưu để giám sát mức độ rò rỉ chì ra môi trường xung quanh, và họ đã quyết định thử nghiệm trên loài chim sẻ.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072114.webp)

Chim sẻ có thói quen sinh hoạt gần gũi với con người và có tốc độ hấp thụ các chất hóa học độc hại từ môi trường nhanh hơn. Bằng cách bắt và thực hiện đo lường hàm lượng chì trong máu của chim sẻ, các nhà khoa học có thể nhanh chóng phát hiện các dấu hiệu rò rỉ chì ra môi trường để phát đi các cảnh báo sớm cho cộng đồng (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072115.webp)

4、**Các tin tức khác**

(1) Một nhà vật lý học người Mỹ đã nghiên cứu và công bố [phương trình mô tả hành vi chuyển động của loài mèo](https://phys.org/news/2024-10-physicist-cat-reveal-equation-motion.html). Bằng cách nhập các thông số khối lượng và hệ số mệt mỏi của mèo, công thức cho phép tính toán chính xác quãng đường dịch chuyển của chú mèo từ thời điểm t0 đến t1. Mục tiêu của nghiên cứu vui này là nhằm khơi gợi sự hứng thú của công chúng đối với bộ môn cơ học cổ điển.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110519.webp)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110520.webp)

(2) Nhà cung cấp dịch vụ phân phối nội dung CDN [bunny.net](https://bunny.net/blog/introducing-bunny-edge-scripting-a-better-way-to-build-and-deploy-applications-at-the-edge/) vừa chính thức ra mắt dịch vụ Edge Scripting chạy trên nền tảng Deno, bổ sung thêm một lựa chọn triển khai mã nguồn tại vùng biên mạng cho các nhà phát triển.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110802.webp)

## 文章

1、[Node.js 23 chính thức hỗ trợ require() nạp trực tiếp mô-đun ES6](https://evertpot.com/using-top-level-await-is-bc-break/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024100908.webp)

Phiên bản Node.js 23 mới ra mắt đã hỗ trợ nạp mô-đun ES6 thông qua phương thức `require()`. Bài viết giới thiệu cơ chế này đồng thời đưa ra các góc nhìn phân tích xem liệu đây có phải là một quyết định thực sự hợp lý.

2、[Thư mục AppData trên Windows có công năng gì?](https://www.xda-developers.com/appdata/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024100909.webp)

Bài viết khoa học phổ thông giải thích chi tiết về cấu trúc và công năng lưu trữ dữ liệu của thư mục ẩn AppData mặc định trên hệ điều hành Windows 11.

3、[Lịch sử tiến hóa và sự thay đổi của các phiên bản công nghệ Bluetooth](https://www.androidauthority.com/bluetooth-versions-3488170/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024100910.webp)

Bài viết tổng hợp lịch sử phát triển của giao thức kết nối không dây Bluetooth, phân tích các đặc tính kỹ thuật nổi bật của từng phiên bản công nghệ qua các thời kỳ.

4、[Lập luận: Không nên đưa logic nghiệp vụ (business logic) vào cơ sở dữ liệu](https://www.infoworld.com/article/2269523/put-business-logic-in-the-application-not-the-database.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024100911.webp)

Tác giả đưa ra các lập luận phân tích cho thấy cơ sở dữ liệu chỉ nên làm đúng vai trò lưu trữ thông tin thô, và toàn bộ logic nghiệp vụ của hệ thống nên được xử lý tập trung tại tầng ứng dụng để dễ dàng bảo trì và mở rộng về sau.

5、[Tìm hiểu cơ bản về giao thức đăng nhập một lần SAML](https://ssoready.com/docs/saml/saml-technical-primer) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024092802.webp)

Bài phân tích sâu giới thiệu về giao thức xác thực SAML thường được ứng dụng rộng rãi trong các hệ thống doanh nghiệp lớn. Phần đầu bài viết giới thiệu rất dễ hiểu về khái niệm SAML, phần sau đi sâu vào các chi tiết kỹ thuật phức tạp hơn.

6、[Giải thích trực quan phương trình Einstein E=mc² và vận tốc ánh sáng](https://profmattstrassler.com/2024/10/01/why-is-the-speed-of-light-so-fast-part-1/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024100502.webp)

Bài viết khoa học phổ thông giải thích dễ hiểu về ý nghĩa vật lý của phương trình nổi tiếng E=mc² mà không lạm dụng các công thức toán học phức tạp, phân tích tại sao phương trình lại chứa bình phương vận tốc ánh sáng.

## 工具

1、[PasteBar](https://github.com/PasteBar/PasteBarApp)

Ứng dụng mã nguồn mở dành cho máy tính (Windows và macOS) giúp quản lý lịch sử khay nhớ tạm (clipboard manager), hỗ trợ tìm kiếm nhanh lịch sử copy và thiết lập sẵn các nội dung văn bản thường dùng để dán nhanh khi cần.

2、[FastHTML](https://fastht.ml/)

Nền tảng phát triển ứng dụng web gọn nhẹ dành cho ngôn ngữ Python, hoạt động như một giải pháp thay thế đơn giản và tối giản hơn cho Django framework.

3、[Dịch vụ dịch thuật Kagi Translate](https://translate.kagi.com/)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110803.webp)

Công cụ tìm kiếm Kagi vừa chính thức giới thiệu dịch vụ dịch thuật trực tuyến mới hoạt động tương tự như Google Translate.

4、[Star (Tìm hướng vệ tinh)](https://star.conor.link/)

Ứng dụng web hoạt động trên trình duyệt điện thoại di động, tận dụng cảm biến con quay hồi chuyển của thiết bị để hiển thị và chỉ hướng chính xác vị trí của một vệ tinh nhân tạo chỉ định trên bầu trời so với vị trí của bạn.

5、[kkTerminal](https://github.com/zyyzyykk/kkTerminal)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024111010.webp)

Ứng dụng web terminal mã nguồn mở hỗ trợ kết nối SSH điều khiển các máy chủ từ xa trực tiếp trên giao diện trình duyệt web. (Đóng góp từ [@zyyzyykk](https://github.com/ruanyf/weekly/issues/5503))

6、[ReactPress](https://github.com/fecommunity/reactpress)

Hệ thống quản trị nội dung CMS và trang blog hiện đại được xây dựng dựa trên Next.js. Trải nghiệm bản [Demo](https://blog.gaoredu.com). (Đóng góp từ [@fecommunity](https://github.com/ruanyf/weekly/issues/5524))

7、[PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110909.webp)

Công cụ dòng lệnh mã nguồn mở ứng dụng AI để dịch thuật các tệp PDF tài liệu khoa học, hỗ trợ giữ nguyên hoàn hảo định dạng trang và các công thức toán học phức tạp. (Đóng góp từ [@Byaidu](https://github.com/ruanyf/weekly/issues/5501))

8、[dimmer](https://github.com/slc3a2/dimmer)

Tiện ích mở rộng mã nguồn mở dành cho trình duyệt Chrome hỗ trợ người dùng bật/tắt nhanh chế độ giao diện tối (dark mode) trên mọi trang web chỉ bằng một cú nhấp chuột. (Đóng góp từ [@slc3a2](https://github.com/ruanyf/weekly/issues/5496))

9、[ThriveX](https://github.com/LiuYuYang01/ThriveX-Blog)

Dự án trang blog cá nhân mã nguồn mở xây dựng trên kiến trúc Next.js 14 kết hợp với Spring Boot. Liên kết trên dẫn đến kho chứa mã nguồn frontend, ngoài ra dự án còn có kho chứa [backend](https://github.com/LiuYuYang01/ThriveX-Service) và trang [quản trị admin](https://github.com/LiuYuYang01/ThriveX-Admin) riêng. (Đóng góp từ [@LiuYuYang01](https://github.com/ruanyf/weekly/issues/5491))

10、[Trayce](https://trayce.dev/)

Công cụ hỗ trợ giám sát và bắt các yêu cầu truyền tải HTTP(S) đi và đến của các container Docker hoạt động trong môi trường phát triển cục bộ.

11、[ngtop](https://github.com/facundoolano/ngtop)

Công cụ dòng lệnh gọn nhẹ giúp quản trị viên nhanh chóng phân tích và truy vấn dữ liệu từ tệp nhật ký truy cập (access log) của máy chủ Nginx.

12、[InputShare](https://github.com/BHznJNs/InputShare)

Công cụ nhỏ gọn hỗ trợ chia sẻ chuột, bàn phím và khay nhớ tạm (clipboard) của máy tính Windows sang thiết bị di động Android kết nối cùng hệ thống. (Đóng góp từ [@BHznJNs](https://github.com/ruanyf/weekly/issues/5545))

## 资源

1、[Giáo trình học tập kỹ thuật ngược cho mọi người](https://0xinfection.github.io/reversing/) (Reverse Engineering For Everyone)

Tài liệu điện tử miễn phí bằng tiếng Anh hướng dẫn học tập kỹ thuật ngược (Reverse Engineering) từ cơ bản, hỗ trợ cả hai cấu trúc vi xử lý thông dụng là x86 và ARM.

2、[Công cụ tạo mã iframe trực quan](https://iframegenerator.top/)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110908.webp)

Thẻ HTML iframe sở hữu rất nhiều thuộc tính cấu hình phức tạp. Công cụ web trực quan này giúp người dùng dễ dàng tùy chỉnh các thuộc tính hiển thị và tự động sinh mã nguồn tương ứng. (Đóng góp từ [@wincatcher](https://github.com/ruanyf/weekly/issues/5499))

3、[Danh sách các tham số dòng lệnh (flags) của Chromium](https://peter.sh/experiments/chromium-command-line-switches/)

Trang web tổng hợp chi tiết toàn bộ danh sách các tham số dòng lệnh cấu hình sâu (switches) dành cho trình duyệt Chromium (Chrome) với số lượng lên tới hơn 1.600 tham số.

4、[Giới thiệu công cụ soạn thảo văn bản Typst](https://blog.jreyesr.com/posts/typst/) (tiếng Anh)

Bài viết giới thiệu về Typst — công cụ soạn thảo văn bản khoa học thế hệ mới hoạt động tương tự như LaTeX nhưng sở hữu cú pháp viết giản dị và thân thiện gần giống như Markdown.

## 图片

1、[Hóa thạch loài thú mai tấm khổng lồ (Glyptodon)](https://allthatsinteresting.com/glyptodon-fossils)

Một người nông dân tại Argentina trong lúc đi làm đồng đã vô tình phát hiện ra bốn khối đất tròn lớn có hình thù kỳ dị nằm bên vệ đường.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110901.webp)

Sau khi các nhà khảo cổ học đến giám định, họ đã vô cùng ngạc nhiên khi xác định đây chính là hóa thạch nguyên vẹn của bốn cá thể Glyptodon (thú mai tấm khổng lồ) — loài động vật tiền sử đã bị tuyệt chủng từ cách đây khoảng 10.000 năm.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110902.webp)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110903.webp)

Thú mai tấm khổng lồ có cấu trúc lớp vỏ cứng bảo vệ bên ngoài tương tự như loài rùa hay tê tê ngày nay. Hình ảnh dưới là bức ảnh chụp loài thú mai tấm nhỏ (Armadillo) trong tự nhiên ngày nay.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110904.webp)

Một trong những giả thuyết về nguyên nhân tuyệt chủng của loài Glyptodon khổng lồ có liên quan trực tiếp đến hoạt động săn bắn của con người cổ đại nhằm lấy lớp vỏ mai cứng cáp của chúng để làm khiên che hoặc làm vật liệu dựng lều tạm.

2、[Kính chống tuyết cổ xưa của người Inuit](https://kottke.org/21/11/arctic-snow-goggles)

Bề mặt băng tuyết có năng lực phản xạ ánh sáng mặt trời cực mạnh dễ gây tổn thương thị lực nghiêm trọng cho con người (y học gọi là chứng mù tuyết). Do đó, các hoạt động trên băng tuyết bắt buộc phải đeo kính bảo vệ.

Người Inuit — những cư dân bản địa sinh sống tại vùng Bắc Cực lạnh giá suốt hàng trăm năm qua — đã giải bài toán phòng ngừa chứng mù tuyết như thế nào trong điều kiện nguyên thủy?

Họ đã sáng tạo ra các loại kính bảo vệ mắt từ các vật liệu tự nhiên có sẵn như xương động vật, gỗ hoặc răng cá voi, thiết kế ôm khít khuôn mặt và chỉ chừa lại một khe hở rất nhỏ để quan sát thế giới xung quanh.

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120403.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120404.webp)

Thiết kế khe hở siêu nhỏ này giúp hạn chế tối đa lượng ánh sáng phản xạ đi vào mắt để bảo vệ võng mạc, đồng thời hỗ trợ cải thiện độ sắc nét của hình ảnh quan sát. Cơ chế này hoạt động tương tự như nguyên lý của máy ảnh lỗ kim (pinhole camera), khi khe hẹp giúp tập trung các tia sáng đi thẳng giúp hình ảnh ở xa trở nên rõ ràng và sắc nét hơn.

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120405.webp)

## 文摘

1、[Lập luận: Giao diện giọng nói (Voice UI) thực sự rất tệ](https://shubhamjain.co/2024/04/16/voice-is-bad-ui/)

Sự bùng nổ của công nghệ AI đang thúc đẩy mạnh mẽ xu hướng ứng dụng giọng nói làm giao diện tương tác người dùng (được gọi là Voice UI).

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024111401.webp)

Nhiều người tin rằng Voice UI sẽ là đích đến cuối cùng của trải nghiệm người dùng, bởi lẽ khi bạn có thể điều khiển thiết bị bằng giọng nói thì tại sao lại phải mất thời gian sử dụng bàn phím hay chuột làm gì?

Tuy nhiên, tôi lại hoàn toàn không tin tưởng vào tương lai phổ biến của giao diện giọng nói vì một số lý do cốt lõi sau:

**(1) Ngôn ngữ nói vốn không tối ưu cho việc diễn đạt các ý tưởng trừu tượng.**
Nhiều khi bộ não của chúng ta mới chỉ hình thành những suy nghĩ sơ khai mập mờ, việc tìm kiếm từ ngữ chính xác để diễn đạt suy nghĩ đó thành câu nói mạch lạc là việc tương đối mất thời gian.

**(2) Giọng nói làm phức tạp hóa nhiều tác vụ đơn giản.**
Về lý thuyết, câu lệnh *"gọi một chiếc xe taxi ra sân bay"* nghe có vẻ rất nhanh gọn. Nhưng nếu bạn có thêm các yêu cầu cụ thể như chọn dòng xe tiết kiệm, giới hạn tầm giá và chọn tuyến đường đi tránh kẹt xe... việc diễn đạt tất cả các yêu cầu đó bằng giọng nói sẽ trở nên vô cùng rườm rà.

**(3) Vấn đề bảo mật thông tin riêng tư.**
Khi bạn ra lệnh bằng giọng nói, bạn có thực sự cảm thấy thoải mái khi những người xung quanh đều nghe thấy toàn bộ nội dung bạn nói?

**(4) Giao diện đồ họa (GUI) hiển thị trực quan các giới hạn của phần mềm, còn Voice UI thì không.**
Giao diện đồ họa giúp người dùng nhìn thấy ngay phần mềm có những tính năng gì và không thể làm được việc gì. Nếu không có giao diện trực quan này, bạn sẽ gặp rất nhiều khó khăn để tự mò mẫm xem hệ thống AI có hỗ trợ tính năng mình cần hay không.

**(5) Người dùng không thích nói liên tục.**
Việc ra lệnh bằng giọng nói cho một vài tác vụ đơn giản thì rất tiện lợi, nhưng để giải quyết toàn bộ các công việc phức tạp hằng ngày bằng cách nói liên tục sẽ sớm gây mệt mỏi và phiền toái cho chính bạn.

**(6) Giọng nói không thể giải quyết triệt để các mơ hồ trong giao tiếp.**
Ngôn từ giao tiếp hằng ngày thường chứa đựng rất nhiều sắc thái mơ hồ tùy thuộc ngữ cảnh mà các mô hình AI hiện nay chưa thể hiểu đúng 100%, dễ dẫn đến việc AI thực thi sai lệnh của người dùng.

## 言论

1、

Công ty giáo dục trực tuyến Chegg của Mỹ vốn nổi tiếng với dịch vụ hỗ trợ giải bài tập về nhà cho học sinh. Mô hình hoạt động của họ là nhận câu hỏi của học sinh rồi phân phối cho hàng ngàn cộng tác viên tại Ấn Độ để viết lời giải.

Ngay sau khi ChatGPT ra đời, học sinh đã lập tức từ bỏ dịch vụ này để chuyển sang hỏi trực tiếp AI. Giá cổ phiếu của Chegg hiện tại đã sụt giảm nghiêm trọng tới 99% giá trị.

-- [《Chi tiết cách ChatGPT đánh sập gã khổng lồ công nghệ giáo dục》](https://www.wsj.com/tech/ai/how-chatgpt-brought-down-an-online-education-giant-200b4ff2)

2、

Mục tiêu cốt lõi của phần lớn các học thuyết triết học là giúp rèn luyện và củng cố nội lực tinh thần của bạn, giúp bạn học cách giữ thái độ bình thản và thờ ơ trước những sự việc nằm ngoài tầm kiểm soát của bản thân.

-- [《Chủ nghĩa khắc kỷ trong thế giới Linux》](https://www.rugu.dev/en/blog/linux-asceticism/)

3、

Là một công dân sinh sống tại Đức, mỗi tháng tôi phải đóng khoảng 1.000 Euro tiền bảo hiểm y tế bắt buộc cùng một khoản thuế thu nhập cá nhân tương tự. Thế nhưng, nếu tôi quyết định nghỉ việc ở nhà, lập gia đình và sinh 1 đến 2 con, tổng số tiền trợ cấp thất nghiệp cộng với trợ cấp sinh con hằng tháng mà tôi nhận được từ chính phủ còn cao hơn cả mức thu nhập ròng sau thuế khi tôi đi làm chăm chỉ. Cơ chế phúc lợi xã hội này thực sự là không thể duy trì bền vững lâu dài, nhưng đáng buồn là không một chính trị gia nào dám thẳng thắn nhìn nhận vấn đề này.

-- [Ý kiến độc giả trên diễn đàn Hacker News](https://news.ycombinator.com/item?id=42070430)

4、

Tôi thường xuyên nhận được câu hỏi tại sao vào năm 2019 lại quyết định sáp nhập thư viện Keras vào hệ sinh thái TensorFlow của Google.

Thực tế đó hoàn toàn không phải là quyết định của cá nhân tôi, mà là chỉ thị của trưởng bộ phận TensorFlow lúc đó. Thời điểm ấy tôi mới chỉ là nhân sự cấp bậc L5 tại Google trong khi anh ấy ở cấp bậc L8. Nếu tôi không đồng ý với chỉ thị đó, lựa chọn duy nhất của tôi là phải nộp đơn xin nghỉ việc tại Google.

-- [Francois Chollet](https://news.ycombinator.com/item?id=42130881), *Tác giả thư viện mạng thần kinh Keras nổi tiếng, người vừa chính thức thông báo từ bỏ công việc tại Google tuần này*

5、

Rủi ro lớn nhất của một doanh nghiệp khởi nghiệp (startup) không phải là sự thất bại của dự án, mà là việc hình thành nên một nền văn hóa né tránh thử thách và không dám thử nghiệm những ý tưởng mới.

-- [《Những nhà lãnh đạo có năng lực bao dung thất bại》](https://praachi.work/blog/failure-tolerant-leaders)

## 往年回顾

[Tìm hiểu về các vấn đề tranh chấp bản quyền tác phẩm nghệ thuật tạo bằng AI](https://www.ruanyifeng.com/blog/2023/10/weekly-issue-278.html) (2023 #278)

[Chiêm nghiệm về ý nghĩa thực sự của con người và cuộc sống](https://www.ruanyifeng.com/blog/2022/10/weekly-issue-228.html) (2022 #228)

[Kỷ nguyên bùng nổ của giải pháp điện mặt trời hộ gia đình](https://www.ruanyifeng.com/blog/2021/10/weekly-issue-178.html) (2021 #178)

[Liệu xã hội hiện đại của chúng ta có đang dần chuyển dịch sang mô hình Cyberpunk?](https://www.ruanyifeng.com/blog/2020/10/weekly-issue-128.html) (2020 #128)

(Hết)
