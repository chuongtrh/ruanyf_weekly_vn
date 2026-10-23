# Bản tin công nghệ hàng tuần (Số 413): Tạm biệt React Native

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần. (**[Thông báo] Kỳ tuần san tuần tới sẽ tạm nghỉ dịp nghỉ lễ Trung thu và Quốc khánh.**)

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/11434) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091701.webp)

Cổng Tây mới khánh thành của cơ sở Mẫn Hàng thuộc Đại học Sư phạm Hoa Đông, mô phỏng lại cổng trường Đại học Quang Hoa — một trong những tiền thân của trường. ([via](https://www.ecnu.edu.cn/info/1426/73055.htm))

## 再见了，React Native

Shopify vừa chính thức [tuyên bố](https://shopify.engineering/back-to-native) từ bỏ React Native, quay lại sử dụng Swift và Kotlin để phát triển các ứng dụng di động của hãng.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091307.webp)

Nói cách khác, họ quyết định quay về với ngôn ngữ gốc (native), phát triển client riêng biệt cho iOS và Android, chấm dứt việc dùng công nghệ Web để phát triển một phiên bản trung gian rồi biên dịch ra các nền tảng.

Điều này khiến chúng ta nhớ lại 6 năm trước, vào năm 2020, Shopify cũng từng đăng [một bài viết gây xôn xao](https://shopify.engineering/react-native-future-mobile-shopify), tuyên bố từ bỏ ngôn ngữ native để chuyển toàn diện sang React Native và đón nhận công nghệ Web.

Thời điểm đó đây là tin chấn động, rất nhiều người đồng tình với 3 lý do mà Shopify đưa ra:

> - Không cần viết lặp đi lặp lại cùng một tính năng cho từng nền tảng riêng biệt.
> - Cho phép các lập trình viên làm việc linh hoạt trên nhiều công nghệ khác nhau.
> - Thời gian và công sức dôi dư ra có thể dùng để sáng tạo nên nhiều giá trị hơn.

Thành thật mà nói, ba lý do trên chỉ là lời hoa mỹ bề ngoài, lý do duy nhất có trọng lượng thực tế chính là: tiết kiệm tiền.

Năm xưa vì muốn tiết kiệm chi phí, họ chọn React Native để chỉ cần nuôi một đội ngũ kỹ sư duy nhất, thay vì phải duy trì hai đội Android và iOS tốn kém gấp đôi.

Ngày nay từ bỏ React Native, bản chất cũng là để tiết kiệm tiền. Giờ đây khi đã có AI, lập trình viên sử dụng ngôn ngữ nào không còn là rào cản quá lớn nữa. AI có thể dịch chuyển mã nguồn giữa các ngôn ngữ một cách dễ dàng, vậy thì tội gì không dùng luôn ngôn ngữ native có hiệu năng vượt trội và bỏ qua hoàn toàn tầng trung gian?

Tất nhiên, bản thân React Native cũng chưa thực sự đáp ứng kỳ vọng. Kể từ khi ra mắt vào năm 2015 đến nay đã hơn 10 năm, nhiều vấn đề kỹ thuật cơ bản vẫn chưa được giải quyết triệt để, việc làm quen và sử dụng cũng không mấy thuận tiện. Nó bị thay thế âu cũng là điều hợp lý, không có gì oan ức cả.

Tóm lại, AI giống như một cỗ máy biên dịch vạn năng; một khi nó xuất hiện, những ngôn ngữ trung gian hay các tầng chuyển đổi như React Native coi như đã nhận án tử, việc chúng bắt đầu rút lui khỏi vũ đài lịch sử trở thành kết cục tất yếu.

## 世界地图的新投影方法

Tuần trước vừa diễn ra một sự kiện quan trọng: Liên Hợp Quốc đã bỏ phiếu quyết định [bãi bỏ](https://www.not-ship.com/united-nations-map/) phép chiếu Mercator.

Quyết định này tuy không mang tính ràng buộc pháp lý đối với các quốc gia, nhưng là một cột mốc biểu tượng chỉ ra rằng phép chiếu Mercator đã thực sự lỗi thời và cần phải được thay thế.

Chúng ta đều biết Trái Đất hình cầu, trong khi bản đồ lại là mặt phẳng. Điều này đồng nghĩa với việc bắt buộc phải dùng một phép biến đổi nào đó để chiếu địa hình hình cầu lên một tấm bản đồ phẳng. Điều này cũng gián tiếp khẳng định rằng bất kỳ bản đồ phẳng nào cũng đều tồn tại độ méo mó (sai số).

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091702.webp)

Bức ảnh trên là bản đồ thế giới quen thuộc hiện nay, sử dụng phép chiếu Mercator.

Phép chiếu này tương đương với việc kéo dãn quả địa cầu trực tiếp thành hình chữ nhật, hậu quả là các khu vực ở vĩ độ cao sẽ bị kéo dãn cực mạnh, khiến diện tích trông to hơn rất nhiều so với thực tế.

Trong bản đồ trên, châu Phi ở xích đạo trông có vẻ bằng kích thước đảo Greenland ở vĩ độ cao. Nhưng trên thực tế, diện tích châu Phi gấp tới 14 lần diện tích Greenland.

Liên Hợp Quốc khuyến nghị nên bãi bỏ phép chiếu Mercator và **áp dụng phép chiếu Trái Đất Bình Đẳng (Equal Earth Projection) để vẽ bản đồ thế giới**.

Nguyên tắc cốt lõi của phép chiếu Equal Earth là bảo toàn đúng tỷ lệ diện tích: nếu một vùng đất chiếm 1% diện tích Trái Đất thì trên bản đồ nó cũng phải chiếm đúng 1% diện tích, do đó tỷ lệ diện tích tuyệt đối không bị bóp méo.

Cái giá phải trả là hình dạng địa lý sẽ bị kéo dãn: ở khu vực xích đạo và vĩ độ thấp, bản đồ kéo dãn nhẹ theo chiều dọc bắc-nam và co nhẹ theo chiều đông-tây; ở hai cực và vĩ độ cao, bản đồ nở rộng sang hai bên đông-tây và dẹt mạnh theo chiều bắc-nam.

Vì vậy, phép chiếu này sẽ làm biến dạng hình dạng thực tế của các vùng đất, cả chiều dài lẫn chiều rộng đều có thể bị méo mó, không thể dùng loại bản đồ này cho việc dẫn đường chính xác.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091305.webp)

Hình trên là bản đồ thế giới theo phép chiếu Equal Earth, châu Phi trông to lớn hơn rất nhiều.

Dưới đây là hình ảnh so sánh châu Âu và châu Phi giữa phép chiếu Mercator và Equal Earth, các bạn có thể thấy rõ sự khác biệt:

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091306.webp)

## 科技动态

1. [Thiết bị phát hiện camera giấu kín](https://www.chosun.com/english/industry-en/2026/08/30/SBFXUIJQYZEARKP5T4FBAY25HQ/)

Bạn có từng lo sợ xung quanh mình có camera ngụy trang đang lén lút quay trộm?

Các nhà khoa học Hàn Quốc vừa phát minh một thiết bị nhỏ gọn giúp phát hiện nhanh chóng camera quay lén trong phòng.

Thiết bị thực chất là một bảng mạch nhỏ gắn nhiều bóng đèn LED chớp sáng tuần tự, chỉ cần cắm vào điện thoại là hoạt động, chi phí sản xuất rất rẻ.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090101.webp)

Nguyên lý hoạt động: chùm sáng từ đèn LED phát ra sẽ bị thấu kính của camera phản chiếu lại. Chỉ cần tách được ánh sáng phản xạ của camera ra khỏi các bề mặt phản chiếu bình thường (như gương, kính) là sẽ định vị được vị trí camera.

Làm thế nào để loại bỏ các bề mặt phản xạ thông thường? Thiết bị dùng mẹo rất thông minh: lần lượt thắp sáng các bóng đèn LED ở những góc khác nhau.

Các bề mặt phản chiếu bình thường đều là mặt phẳng, trong khi thấu kính camera là thấu kính lồi hình cầu nên ánh sáng phản xạ sẽ bị lệch góc vị trí. Nhờ việc đổi vị trí nguồn sáng chớp liên tục, thuật toán sẽ nhận diện được điểm phản xạ nào bị dịch chuyển vị trí, từ đó khóa chính xác vị trí ống kính camera quay lén.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090102.webp)

2. **Tin vắn công nghệ**

（1）[Lực lượng Houthi](https://news.ycombinator.com/item?id=49660072) gần đây giành được một thắng lợi lớn bằng một chiến thuật kỳ lạ chưa từng có trong lịch sử:
Họ dùng AI giả mạo một đoạn ghi âm mệnh lệnh rút quân của chỉ huy đối phương, rồi nhờ một tài khoản mạng xã hội có tiếng lan truyền đoạn audio giả mạo này trên Twitter (X). Kết quả là quân đội đối phương rơi vào hỗn loạn, giúp họ dễ dàng tiến quân và kiểm soát cứ điểm với tổn thất tối thiểu.

（2）Laptop bắt đầu áp dụng công nghệ tản nhiệt thể rắn (solid-state cooling), không còn cần quạt cơ học mà làm mát thông qua các tấm màng tản nhiệt graphene/lá đồng siêu mỏng.
Nhờ đó laptop có thể làm siêu mỏng nhẹ: [Lenovo](https://www.notebookcheck.net/Lenovo-unveils-ThinkBook-AeroBlade-14-inch-laptop-that-weighs-under-830-grams.1388619.0.html) vừa giới thiệu mẫu concept ThinkBook AeroBlade 14 inch chỉ nặng vỏn vẹn 830g; trong khi mẫu MateBook Pro S 14 inch của Huawei thậm chí chỉ nhẹ 798g.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091201.webp)

（3）Thành phố Thành Đô (Trung Quốc) dự kiến phát hành "[Voucher Token](https://finance.sina.cn/2026-09-11/detail-inirnhrv2204082.d.html?vt=4)", cho phép các doanh nghiệp và cơ quan đăng ký nhận miễn phí: chính quyền sẽ trợ cấp tới 30% chi phí tiêu thụ Token AI.
Ngoài ra Thành Đô còn dự kiến triển khai gói "Vay Token", cho phép doanh nghiệp vay vốn ngân hàng để chi trả tiền Token cho AI.

## 文章

1. [Bộ khung HTML template chuẩn cho năm 2026](https://vale.rocks/posts/html-boilerplate) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091303.webp)

Tác giả phân tích chi tiết một file HTML template chuẩn năm 2026 nên được viết như thế nào và tác dụng thực tế của từng dòng mã.

2. [Cách dùng JavaScript gỡ bỏ hoàn toàn CSS](https://css-tricks.com/that-time-i-tried-browsing-the-web-without-css/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025062102.webp)

Bài hướng dẫn nhập môn chỉ cách dùng JavaScript để vô hiệu hóa toàn bộ stylesheet CSS trên trang web.

3. [Công cụ quản lý container và reverse proxy tự lưu trữ](https://web.archive.org/web/20250401115923/https://kiranet.org/posts/self-hosting-like-its-2025/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025040105.webp)

Tác giả chia sẻ cách anh dùng công nghệ container để dựng hệ thống server cá nhân kèm danh sách tech stack và các công cụ thực tế.

4. [Những điểm kỳ quặc khó đỡ của JavaScript](https://stack-auth.com/blog/on-javascripts-weirdness) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025040501.webp)

Bài viết thú vị điểm lại những hành vi cú pháp kỳ lạ ít người để ý trong thế giới JavaScript.

5. [Tham số udm trong tìm kiếm Google](https://serpapi.com/blog/every-google-udm-in-the-world/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025062107.webp)

URL tìm kiếm của Google có thể thêm tham số `udm` để truy cập trực tiếp vào các định dạng kết quả nhất định, ví dụ `udm=2` trả về kết quả tìm kiếm hình ảnh thuần túy.

6. [Giải thích trực quan về Entropy qua đàn cừu](https://www.engineersedge.com/thermodynamics/entropy_explained_with_sheep_15961.htm) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024101406.webp)

Bài viết dài giải thích khái niệm nhiệt động lực học "Entropy" bằng hình ảnh ẩn dụ đàn cừu bình dị, dễ hiểu kèm nhiều hình minh họa.

## 工具

1. [Great Tables](https://github.com/posit-dev/great-tables)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040402.webp)

Thư viện Python mạnh mẽ giúp tạo ra các bảng biểu dữ liệu phức tạp và đẹp mắt.

2. [ghostty-web](https://github.com/coder/ghostty-web)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120214.webp)

Dự án biên dịch trình giả lập terminal [Ghostty](https://ghostty.org/) sang WebAssembly (WASM), cho phép trải nghiệm một terminal đầy đủ tính năng ngay trong trình duyệt.

3. [Infat](https://github.com/philocalyst/infat)

Công cụ dòng lệnh trên Mac giúp cài đặt ứng dụng mặc định để mở các định dạng file khác nhau.

4. [mini-img-editor](https://github.com/xdadda/mini-photo-editor)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025042901.webp)

Trình chỉnh sửa ảnh online chạy bằng WebGL, giao diện tối giản thích hợp làm bản mẫu tham khảo.

5. [CryptPad](https://cryptpad.fr/)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025050101.webp)

Bộ công cụ văn phòng trực tuyến miễn phí hỗ trợ mã hóa đầu cuối (end-to-end), xem thêm [bài viết giới thiệu](https://www.xda-developers.com/reasons-why-use-cryptpad-instead-google-docs/).

6. [Lyrimuse](https://github.com/Yudaotor/lyrimuse)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091308.webp)

Công cụ hiển thị lời bài hát trên thanh menu desktop macOS thời gian thực theo bài hát đang phát. (Đóng góp từ [@Yudaotor](https://github.com/ruanyf/weekly/issues/11551))

7. [capcut-cli](https://github.com/renezander030/capcut-cli)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091619.webp)

Công cụ dòng lệnh không chính thức của CapCut, giúp tạo và chỉnh sửa video ngay trong terminal. (Đóng góp từ [@renezander030](https://github.com/ruanyf/weekly/issues/11634))

8. [mailez](https://github.com/mailez-hq/mailez)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091621.webp)

File nhị phân duy nhất viết bằng Go giúp tự triển khai hệ thống máy chủ email cá nhân, gửi nhận mail qua web, hỗ trợ 4 giao thức SMTP / IMAP / POP3 / ManageSieve. (Đóng góp từ [@lianguan](https://github.com/ruanyf/weekly/issues/11680))

9. [Status Trio](https://github.com/lingyired/status-trio)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091622.webp)

Icon thanh trạng thái Mac 3-trong-1 học hỏi phong cách thiết kế Dynamic Island của iPhone, tích hợp gọn gàng Wi-Fi, pin và âm lượng. (Đóng góp từ [@lingyired](https://github.com/ruanyf/weekly/issues/11670))

10. [Polycompiler](https://github.com/EvanZhouDev/polycompiler)

Dự án thú vị cho phép đóng gói tập lệnh JavaScript và Python thành một file duy nhất, có thể chạy song song mượt mà trong cả môi trường JS lẫn Python.

## 资源

1. [gpcb.net](https://gpcb.net/net/)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091620.webp)

Công cụ nền web giúp thiết kế sơ đồ topo mạng và thiết bị hạ tầng. (Đóng góp từ [@abpyu](https://github.com/ruanyf/weekly/issues/11622))

2. [Cẩm nang phong cách thị giác (Visual Styles)](https://visualstyles.jerrymakes.com/)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091309.webp)

Dùng hình ảnh một quả táo để minh họa hơn 100 phong cách thiết kế thị giác khác nhau, hình trên là quả táo phong cách Neon rực rỡ. (Đóng góp từ [@jerrymakes](https://github.com/ruanyf/weekly/issues/11555))

3. [Kiểm tra IP kết nối dịch vụ AI](https://store.xiu.ai/zh/ai-ip/)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091407.webp)

Website hiển thị địa chỉ IP thực tế mà máy bạn kết nối tới khi truy cập Claude, ChatGPT, Grok, Perplexity, Cloudflare. (Đóng góp từ [@MuduiClaw](https://github.com/ruanyf/weekly/issues/11571))

4. [Lực hấp dẫn (Gravity)](https://qunabu.github.io/Gravity/#what-is-gravity)

![](https://cdn.beekka.com/blogimg/asset/202606/bg2026062007.webp)

Trang web tương tác đa phương tiện giúp người xem tìm hiểu tường tận các kiến thức vật lý về định luật vạn vật hấp dẫn.

## 图片

1. [Mũ bảo hiểm chiến đấu cơ F-35](https://www.instagram.com/p/DJPerYryd3P/)

Chiếc mũ bảo hiểm đắt đỏ nhất thế giới là mũ bảo hiểm của phi công tiêm kích F-35 Mỹ, trị giá lên tới 400.000 USD (khoảng gần 10 tỷ đồng).

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025050905.webp)

Sở dĩ nó đắt như vậy vì nó kết nối trực tiếp với toàn bộ cảm biến của máy bay để tiếp nhận và xử lý dòng dữ liệu chiến trường.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025050906.webp)

Mũ tích hợp màn hình hiển thị 360 độ cung cấp cho phi công tầm nhìn ban đêm và các thông số bay trực quan (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025050907.webp)

Mỗi chiếc mũ đều được quét 3D theo đúng kích cỡ đầu phi công, chế tạo từ sợi carbon, sợi Kevlar và vô số linh kiện quang học tinh xảo.

2. [Trực thăng chở khách khổng lồ Mi-6 của Liên Xô](https://www.twz.com/news-features/the-story-of-the-monster-mi-6-helicopter-airliner)

Hãng hàng không Liên Xô từng nảy ra ý tưởng táo bạo: dùng trực thăng khổng lồ để vận chuyển hành khách thường xuyên.

Vào thập niên 1960, họ chế tạo Mi-6 — mẫu trực thăng lớn nhất thế giới thời điểm đó, có sức chứa lên tới 80 hành khách.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071115.webp)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071116.webp)

Máy bay dài khoảng 33m, cao 10m. Khoang bên trong bố trí mỗi hàng 5 ghế ngồi, thậm chí có cả nhà vệ sinh riêng.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071117.webp)

Mẫu trực thăng này chỉ duy nhất một chiếc được hoàn thiện, dùng để đưa đón công nhân đến các vùng khai thác dầu mỏ và khí đốt ở miền Đông Liên Xô.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071118.webp)

## 文摘

1. [Món bánh lasagna nhão (Slop Lasagna)](https://underreacted.leaflet.pub/3mdjygm2p5s2c)

Thành thật mà nói, ngoài đời thực mã nguồn của đa số lập trình viên đều viết rất dở.

Tuy nhiên rác rưởi cũng có đẳng cấp của rác rưởi. Một trường hợp tệ hại là mã nguồn giống hệt như đĩa mỳ spaghetti (spaghetti code): xoắn tít bùi nhùi vào nhau, không tài nào lần ra mối gỡ.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090704.webp)

Một tình huống khá khẩm hơn là "[bánh lasagna nhão](https://underreacted.leaflet.pub/3mdjygm2p5s2c)" (slop lasagna). Loại code này tuy chất lượng cũng nhão nhoét, nhưng ít ra nó được phân tách thành nhiều tầng lớp rõ ràng, ít nhất bạn có thể tách rời từng lớp bánh ra để xử lý.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090703.webp)

Ngay cả khi không thể viết ra những dòng code kiệt xuất, **bạn cũng nên tránh xa code kiểu mỳ spaghetti và cố gắng viết code kiểu bánh lasagna**.

Một ví dụ điển hình là framework React: nó chia tách code thành từng component độc lập. Cái hay của cách tiếp cận này là dù cho mỗi component đều chứa code dở tệ, ít nhất bạn vẫn có thể cô lập và thay thế riêng rẽ từng component đó.

Xóa component, copy component, inline component hay viết lại toàn bộ một component đều là những thao tác rất dễ dàng. Nhờ sự phân tách độc lập giữa các component, bạn chỉ cần bận tâm đến mã nguồn bên trong **duy nhất component đó**.

Chỉ cần thiết kế cây component (component tree) hợp lý, mã nguồn chi tiết bên trong từng component viết dở cũng không phải vấn đề chí mạng. Ai đó viết một component rác dài 10.000 dòng thì đã sao, cuối cùng cũng sẽ có người đập đi viết lại, nó tuyệt đối không thể làm lây lan vấy bẩn phần còn lại của codebase.

**Chỉ cần mã nguồn có cấu trúc lasagna phân lớp, thì việc một lớp cụ thể bị dở cũng không làm hỏng toàn cục**.

Những điều thực sự quan trọng là:

（1）Dữ liệu luân chuyển trong hệ thống như thế nào: luồng dữ liệu hiện tại nạp vào từ đâu, xuất ra cái gì và bạn lưu trữ những dữ liệu nào.

（2）Trải nghiệm người dùng ra sao: có lỗ hổng bảo mật hiển nhiên nào không, hiệu năng có giật lag không, hành vi ứng dụng có bị tiền hậu bất nhất không.

（3）Các khái niệm trừu tượng nền tảng có chuẩn xác không, có bị lạm dụng sai ngữ cảnh không.

**Chỉ cần 3 điểm cốt lõi trên ổn định, và mã nguồn có cấu trúc module tách lớp có thể tháo lắp thay thế, thì chương trình coi như không có vấn đề gì lớn**. Khi đó, một component cụ thể viết dài dòng, chưa tối ưu, kém thanh thoát hay còn vài bug vặt vãnh thực ra cũng chẳng ảnh hưởng tới đại cục.

## 言论

1.

Vệ tinh quay quanh hành tinh sẽ làm tiêu hao dần năng lượng tự quay của hành tinh đó, từ đó đẩy nhanh quá trình diệt vong của hành tinh.

-- [《Sao Kim đã tự nuốt chửng mặt trăng của mình?》](https://www.space.com/astronomy/venus/did-venus-eat-its-own-moon)

2.

Hãy tưởng tượng hai công ty phần mềm có quy mô doanh thu và sản phẩm tương tự nhau. Điểm khác biệt duy nhất là công ty A cần tới 1 triệu dòng code, trong khi công ty B chỉ cần 100.000 dòng code. Công ty nào sẽ vận hành tốt hơn?
Rõ ràng công ty có số dòng code chỉ bằng 1/10 sẽ vượt trội hơn hẳn. Càng ít dòng code, bạn càng đọc hiểu nhanh và sửa đổi kịp thời hơn.

-- [《Mã nguồn chính là món nợ kỹ thuật》](https://tornikeo.com/code-is-debt/)

3.

Mô hình lớn sẽ biến bạn từ một lập trình viên chuyên gõ code thành một kỹ sư chuyên quản trị ngữ cảnh (context), loại bỏ các thông tin rác và chấp bút những câu lệnh prompt tỉ mỉ.

-- [Liz Fong-Jones](https://simonwillison.net/2025/Dec/30/liz-fong-jones/)

4.

Một nhà sáng lập nếu vào năm 2024 xây dựng được đội ngũ chuẩn mực nhưng lại làm sai sản phẩm, thì chỉ cần kiên trì trụ đến năm 2027, đội ngũ đó sẽ trở thành một tập thể dạn dày sương gió qua bao trận mạc và khả năng rất cao sẽ tạo nên sản phẩm đúng đắn.
Kinh nghiệm đúc rút từ những thất bại giống như chất dinh dưỡng tích tụ trong bộ rễ cây, âm thầm chuẩn bị cho mùa xuân tiếp theo chứ không hề mất đi vô ích.

-- [《AI không sụp đổ, mà sẽ đón một cơn bão táp》](https://ceodinner.substack.com/p/the-ai-wildfire-is-coming-its-going)

5.

Nhiều công nghệ gặp lỗi thực ra không phải vấn đề quá lớn: GPS chỉ sai đường thì tôi sẽ nhanh chóng nhận ra vị trí bất thường; Netflix gợi ý phim dở thì tôi tắt đi không xem nữa.
Thế nhưng với AI thì hoàn toàn khác: nó càng tiên tiến thì chúng ta càng khó phát hiện ra nó có bị sai hay không, bởi chúng ta thường giao cho AI những bài toán mà bản thân không thể tự làm và cũng không đủ năng lực thẩm định.
Một khi AI phạm sai lầm, chúng ta chỉ còn biết liên tục triệu hồi những mô hình AI hùng mạnh hơn, hy vọng câu thần chú sẽ phát huy hiệu nghiệm. Chào mừng bạn bước vào kỷ nguyên của những phù thủy.

-- [《Làm việc cùng AI là cộng tác với những phù thủy》](https://www.oneusefulthing.org/p/on-working-with-wizards)

## 往年回顾

[Quảng cáo AI điên cuồng ở San Francisco](https://www.ruanyifeng.com/blog/2025/09/weekly-issue-366.html) (#366)

[Câu chuyện cuộc đời bạn](https://www.ruanyifeng.com/blog/2024/09/weekly-issue-316.html) (#316)

[Tự làm sách điện tử EPUB song ngữ](https://www.ruanyifeng.com/blog/2023/08/weekly-issue-266.html) (#266)

[Chiến thắng của chủ nghĩa tối giản](https://www.ruanyifeng.com/blog/2022/07/weekly-issue-216.html) (#216)

(Hết)
