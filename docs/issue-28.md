# 每周分享第 28 期 (Bản tin chia sẻ hàng tuần số 28)

Ghi lại những điều thú vị đáng chia sẻ tôi bắt gặp trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Chào mừng mọi người gửi bài đóng góp thông qua mục [issue](https://github.com/ruanyf/weekly/issues) tại kho lưu trữ GitHub [ruanyf/weekly](https://github.com/ruanyf/weekly).

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102601.jpg)

Trong [số chia sẻ thứ 24](issue-24.md), tôi có trích dẫn lời khuyên của một kỹ sư đi trước dành cho các lập trình viên trẻ:

> "Trong ngành phát triển phần mềm, công nghệ thay đổi quá nhanh. Nếu bạn dành quá nhiều thời gian chỉ để học cách sử dụng các công nghệ và công cụ thời thượng, một khi chúng bị thay thế, khối lượng kiến thức đó sẽ trở nên vô giá trị vì chúng chỉ là chi tiết triển khai bề nổi."

Gần đây tôi liên tục suy ngẫm về câu nói này, tự hỏi: Liệu các kỹ năng phát triển phần mềm có thực sự được coi là tri thức đích thực (knowledge) hay không?

Nếu nó là một loại tri thức đích thực, thì về mặt lý thuyết, phần lớn những gì chúng ta học được sẽ không bị lỗi thời theo thời gian, giống như các nguyên lý của môn Giải tích vậy. Tuy nhiên thực tế lại cho thấy các kỹ năng lập trình có hạn sử dụng rất ngắn. Những kiến thức công nghệ bạn học cách đây mười năm gần như không thể áp dụng trực tiếp vào môi trường sản xuất ngày nay. Dưới góc nhìn đó, kỹ năng lập trình chỉ là các chi tiết triển khai tạm thời (implementation details) chứ chưa đạt tới tầm tri thức đích thực.

Cạnh văn phòng tôi có một chi nhánh của chi cục thuế, ngày nào cũng có hàng dài người xếp hàng nộp thuế. Nếu là lần đầu tiên đi nộp thuế, bạn chắc chắn sẽ lúng túng vì không biết quy trình. Việc nộp thuế giống như một thứ kỹ năng thủ tục: bạn phải được hướng dẫn mang theo những giấy tờ gì, điền vào những mẫu đơn nào và xếp hàng ở cửa quầy nào.

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102602.jpg)

**Hiện tại tôi cho rằng việc học lập trình công cụ cũng tương tự như việc học quy trình nộp thuế ở trên: đều là việc ghi nhớ các chi tiết triển khai tạm thời. Một khi môi trường bên ngoài thay đổi, toàn bộ quy trình cũ sẽ trở nên vô dụng.** Do sự xuất hiện của các tầng lớp đóng gói và trừu tượng hóa liên tục trong phát triển phần mềm hiện đại, lập trình viên thông thường gần như không còn phải tiếp xúc với các tri thức phổ quát ở tầng đáy của máy tính. Hầu hết thời gian viết code thực chất là chúng ta đang viết cấu hình (configuration) cho một tầng trừu tượng nào đó. Ví dụ, thiết kế giao diện web thực chất là viết các thuộc tính cấu hình CSS, thật khó để khẳng định đây là tri thức đích thực hay chỉ là các bước thao tác thủ tục tương tự cuốn "Hướng dẫn nộp thuế".

Chi tiết triển khai không phải là tri thức cốt lõi, nó chỉ là các bước thao tác nghiệp vụ. Khi tech stack thay đổi, các chi tiết này sẽ biến mất không còn giá trị. Tuy nhiên, bạn lại không thể không học chúng vì nếu không làm chủ chi tiết triển khai, bạn sẽ không thể hoàn thành dự án thực tế. Tôi nghĩ lập trình viên cần tỉnh táo để không rơi vào cái bẫy của chi tiết triển khai: đừng dành toàn bộ thời gian và sức lực chỉ để học cách cấu hình các công cụ thời thượng rồi lầm tưởng mình đã làm chủ được tri thức đích thực của ngành khoa học máy tính. Đối với mọi ngôn ngữ và công cụ lập trình, thái độ đúng đắn nên là "dễ dàng đi vào, và dễ dàng đi ra": vừa có khả năng đào sâu chi tiết kỹ thuật khi cần thiết, vừa duy trì được tầm nhìn vĩ mô để hiểu rõ bản chất cơ chế vận hành tầng dưới của chúng.

## 新闻 (Tin tức)

1、[Mỹ nghiên cứu dự án sử dụng côn trùng làm vũ khí sinh học phát tán virus](https://www.newsweek.com/darpa-biological-weapons-insects-scientists-warn-1152834)

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102603.jpg)

Nhóm các nhà nghiên cứu cảnh báo dự án "Insect Allies" của Cơ quan DARPA thuộc Bộ Quốc phòng Mỹ đang nghiên cứu sử dụng các loài côn trùng phổ biến (như rầy lá, rệp, ruồi trắng) làm vector truyền nhiễm để phát tán các dòng virus biến đổi gene có khả năng chỉnh sửa nhiễm sắc thể của cây trồng ngay trên đồng ruộng. Dự án hướng tới mục tiêu bảo vệ mùa màng trước thiên tai nhưng giới khoa học lo ngại công nghệ có thể bị lạm dụng để phá hoại mùa màng của đối phương làm giảm sản lượng lương thực.

2、[Nhà hát Quốc gia London đưa vào sử dụng kính thông minh hiển thị phụ đề tự động](https://www.nytimes.com/2018/10/03/theater/uk-national-theatre-smart-glasses.html)

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102604.jpg)

Nhà hát Quốc gia Anh bắt đầu cung cấp thiết bị kính thông minh cho khán giả. Phụ đề lời thoại của vở kịch sẽ được truyền qua sóng Wi-Fi và hiển thị trực quan ngay trên mắt kính theo thời gian thực. Thiết bị hỗ trợ đắc lực cho những khán giả khiếm thính và cho phép khán giả tùy chọn hiển thị các ngôn ngữ phụ đề khác nhau. Hiện rào cản lớn nhất của thiết bị là mức chi phí sản xuất khá đắt đỏ, khoảng 1.050 USD cho mỗi chiếc kính.

3、[Phát triển miếng dán da co giãn đo huyết áp động mạch sâu trong cơ thể](https://www.technologyreview.com/s/612148/stretchy-stick-on-patch-can-take-blood-pressure-readings-from-deep-inside-your-body/)

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102605.jpg)

Các nhà nghiên cứu tại Đại học California San Diego chế tạo thành công mẫu miếng dán dẻo dán trên da có khả năng đo huyết áp liên tục. Khác với các thiết bị đeo thông thường chỉ đo nhịp tim, miếng dán này sử dụng sóng siêu âm xuyên sâu qua lớp da để đo trực tiếp đường kính và áp lực của các mạch máu sâu trong cơ thể, giúp theo dõi huyết áp liên tục cho bệnh nhân tim mạch một cách dễ dàng không cần dùng đến băng quấn cánh tay truyền thống.

4、[Facebook phát triển hệ thống dịch thuật AI không cần ngữ liệu đối chiếu](https://www.forbes.com/sites/williamfalcon/2018/09/01/facebook-ai-just-set-a-new-record-in-translation-and-why-it-matters/#6e934aa43124)

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102606.jpg)

Các hệ thống dịch thuật máy học thông thường (như Google Translate) hoạt động dựa trên mô hình thống kê phân tích hàng triệu văn bản song ngữ đối chiếu của các ngôn ngữ phổ biến. Đối với các ngôn ngữ ít phổ biến (như tiếng Urdu) vốn rất thiếu tài liệu dịch thuật song ngữ, Facebook đã phát triển hệ thống dịch thuật AI mới có khả năng tự động phân tích cấu trúc ngữ pháp và tách nghĩa từ gốc để tự động dịch chính xác mà không cần nguồn dữ liệu đối chiếu từ trước.

5、[Hệ thống camera kết hợp radar quét 3D không gian OS-1](https://www.ouster.io/blog-posts/2018/8/31/the-camera-is-in-the-lidar)

Một startup công nghệ giới thiệu thiết bị quét OS-1 tích hợp đồng thời camera kỹ thuật số thông thường và hệ thống cảm biến LiDAR đo khoảng cách bằng laser. Thiết bị hỗ trợ tự động chụp ảnh và dựng mô hình 3D đo đạc khoảng cách thực tế của toàn bộ vật thể trong phòng ngay trong quá trình bấm máy chụp ảnh.

6. **Tác phẩm hội họa của Banksy tự hủy bằng máy hủy tài liệu giấu trong khung tranh**

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102608.jpg)

Tại buổi đấu giá của Sotheby's London, ngay sau khi bức tranh "Girl with Balloon" của nghệ sĩ đường phố nổi tiếng Banksy được gõ búa chốt giá bán kỷ lục, một bộ phận hủy giấy giấu kín bên trong khung tranh đã tự động kích hoạt cắt nửa dưới bức tranh thành các sợi nhỏ trước sự ngỡ ngàng của toàn bộ khách mời tham dự.

7、[Thành phố Paris thử nghiệm lắp đặt hệ thống bồn tiểu lộ thiên thân thiện môi trường](https://edition.cnn.com/2018/08/14/europe/paris-urinal-intl/index.html)

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102609.jpg)

Nhằm giải quyết tình trạng phóng uế bừa bãi trên đường phố, thủ đô Paris đã lắp đặt các hộp bồn tiểu lộ thiên (Uritrottoir) sơn màu đỏ nổi bật dọc theo bờ sông Seine. Bên trong bồn tiểu chứa rơm khô giúp khử mùi hôi hiệu quả và lượng nước tiểu thu thập được sẽ được ủ men tự nhiên làm phân bón hữu cơ cho hệ thống cây hoa trồng ngay phía trên nắp bồn.

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102610.jpg)

8、[Châu Âu phóng thành công hai vệ tinh thăm dò Sao Thủy BepiColombo](https://arstechnica.com/science/2018/10/two-orbiters-begin-their-long-journey-to-mercury-friday-night/)

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102612.jpg)

Cơ quan Vũ trụ Châu Âu (ESA) phối hợp cùng JAXA Nhật Bản phóng thành công tàu vũ trụ mang theo hai vệ tinh thăm dò tiến về Sao Thủy. Chuyến hải trình dự kiến kéo dài 7 năm do Sao Thủy nằm rất gần Mặt Trời, đòi hỏi tàu phải thực hiện nhiều vòng bay quanh các hành tinh để giảm tốc độ tránh bị lực hấp dẫn cực lớn của Mặt Trời hút vào tiêu hủy.

9、[Tin tức vắn](https://www.nextplatform.com/2018/10/04/in-a-parallel-universe-data-warehouses-run-on-gpus/)

* Nhiều doanh nghiệp công nghệ đang tập trung phát triển các dòng cơ sở dữ liệu xử lý bằng GPU thay vì CPU, giúp giảm đáng kể thời gian truy vấn dữ liệu cho các hệ thống Data Warehouse khổng lồ.
* Phát hiện lỗ hổng zero-day nguy hiểm cho phép hacker tải file thực thi độc hại lên máy chủ web PHP thông qua thư viện upload file jQuery File Upload phổ biến.

## 教程 (Hướng dẫn)

1、[Bài viết] [Sự khác biệt cốt lõi về cơ chế quản lý Thread giữa Java và Go](https://rcoh.me/posts/why-you-can-have-a-million-go-routines-but-only-1000-java-threads/) (Tiếng Anh)

Giải thích nguyên nhân tại sao một máy chủ thông thường chỉ chạy được tối đa vài ngàn thread trong Java nhưng có thể khởi chạy đồng thời hàng triệu goroutine trong Go, liên quan đến kích thước bộ nhớ stack mặc định (mỗi thread Java chiếm tới 1MB trong khi goroutine Go chỉ tốn 4KB bộ nhớ khởi tạo ban đầu).

2、[Bài viết] [Hướng dẫn lập trình Web Server bằng ngôn ngữ C++](https://blog.sourcerer.io/building-a-website-with-c-db942c801aee) (Tiếng Anh)

Tài liệu hướng dẫn cách viết mã nguồn C++ biên dịch ra tệp tin thực thi binary liên kết với cổng CGI của máy chủ web Apache để phản hồi nội dung HTML cho trình duyệt, giúp hiểu rõ bản chất hoạt động của các hệ thống Backend.

3、[Bài viết] [Tìm hiểu chi tiết về giao thức mạng cấu hình động DHCP](https://www.benburwell.com/posts/how-does-dhcp-work/) (Tiếng Anh)

Giải thích quy trình 4 bước bắt tay (Discovery, Offer, Request, Acknowledge - DORA) của giao thức DHCP giúp các thiết bị mới kết nối vào mạng LAN tự động nhận địa chỉ IP từ router.

4、[Tài liệu] [Bản đồ tương tác mô tả chi tiết từng byte dữ liệu của quá trình kết nối bảo mật TLS Handshake](https://tls.ulfheim.net/) (Tiếng Anh)

Trang web trực quan hóa giải thích ý nghĩa chi tiết của từng byte dữ liệu trao đổi trong gói tin Client Hello và Server Hello của giao thức bảo mật HTTPS/TLS.

## 资源 (Tài nguyên)

1、[Sách] [Cryptography: An Introduction — Giáo trình nhập môn mật mã học](https://intensecrypto.org/public/) (Tiếng Anh)

Cuốn sách giáo trình nguồn mở của Đại học Harvard giới thiệu chi tiết các cơ sở toán học (lý thuyết số, độ phức tạp thuật toán) đằng sau các hệ thống mã hóa bảo mật hiện đại.

2、[Học tập] [Best YouTube Channels — Trang web tổng hợp các kênh YouTube giáo dục học thuật uy tín](https://www.bestyoutubechannels.info/)

Trang web tổng hợp và phân loại các kênh YouTube chất lượng nhất chia sẻ kiến thức về lập trình, khoa học tự nhiên, kinh tế học và triết học giúp người tự học dễ dàng tìm kiếm.

## 工具 (Công cụ)

1、[walt](https://github.com/ballercat/walt)

Một cú pháp ngôn ngữ viết code kiểu JavaScript nhưng được biên dịch trực tiếp ra định dạng file WebAssembly (WASM) giúp lập trình viên Frontend dễ dàng tiếp cận công nghệ WASM mà không cần học C/C++ hay Rust.

2、[the-great-suspender](https://github.com/deanoemcke/thegreatsuspender)

Tiện ích mở rộng Chrome hỗ trợ tự động giải phóng bộ nhớ RAM bằng cách tạm thời "đóng băng" (suspend) các tab trình duyệt đã lâu không active, giúp trình duyệt chạy mượt mà hơn.

3、[AutoMono](https://github.com/0matgal0/AutoMono)

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102613.jpg)

Một bộ phông chữ等宽 Monospace mã nguồn mở được thiết kế tối ưu hóa độ tương phản và hình dạng ký tự giúp lập trình viên dễ dàng đọc code và hạn chế mỏi mắt.

## 文摘 (Văn trích)

1. **Khủng hoảng thiếu hụt lập trình viên ngôn ngữ COBOL tại các ngân hàng Mỹ**

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102614.jpg)

Cụ ông Bill Hinshaw 75 tuổi vẫn phải tiếp tục điều hành công ty tư vấn để hỗ trợ các ngân hàng lớn tại Mỹ duy trì hệ thống máy chủ cổ xưa. Ngôn ngữ lập trình COBOL ra đời từ 60 năm trước hiện không còn được giảng dạy tại các trường đại học, nhưng nó vẫn đang gánh vác toàn bộ hệ thống xử lý giao dịch tiền gửi, thanh toán thẻ tín dụng và mạng lưới ATM trị giá hàng ngàn tỷ USD xây dựng từ những năm 1970-1980 của hệ thống tài chính Mỹ. Việc thay thế hoàn toàn hệ thống lõi (core banking) chạy COBOL sang các ngôn ngữ hiện đại gặp rủi ro hệ thống cực lớn và tốn kém hàng tỷ USD, buộc các ngân hàng phải chi trả mức thù lao đắt đỏ để mời các lập trình viên COBOL đã nghỉ hưu (hầu hết đều trên 50-70 tuổi) tiếp tục bảo trì hệ thống.

2. **Khảo sát thống kê về mức độ cảm nhận xác suất qua ngôn ngữ nói của con người**

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102616.jpg)

Nghiên cứu khoa học thống kê mức độ tương đồng trong cách hiểu các từ chỉ xác suất trong giao tiếp hàng ngày (như "có thể", "rất có thể", "khó xảy ra"). Kết quả khảo sát được trực quan hóa bằng biểu đồ hộp (box plot) của ggplot2 cho thấy phần lớn mọi người ngầm định nghĩa từ "probably/likely" tương ứng với khoảng 60-85% cơ hội xảy ra, trong khi từ "unlikely" tương ứng với khoảng 10-20% xác suất.

## 本周图片 (Hình ảnh tuần này)

1. **Phương pháp đánh dấu theo dõi đường di cư của loài bướm vua**

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102623.jpg)

Để nghiên cứu chi tiết đường bay di cư tránh rét dài hàng ngàn km của loài bướm vua (Monarch butterfly), các nhà khoa học đã bắt giữ và dán các mảnh nhãn dán siêu nhẹ có in mã số lên góc cánh bướm, hy vọng người dân ở các địa phương dọc đường bay khi bắt được sẽ gửi thông tin mã số về để hoàn thiện bản đồ di cư.

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102624.jpg)

2. **Cách thức các nhà nghiên cứu giám sát mật độ hoạt động của đàn ong mật**

![](https://cdn.beekka.com/blogimg/asset/201810/bg2018102625.jpg)

Các nhà khoa học thuộc Đại học Missouri đã lắp đặt các đầu thu âm thanh siêu nhạy ngoài đồng cỏ để tự động ghi lại tần số tiếng vo ve phát ra từ cánh ong, giúp thống kê chính xác mật độ và thời gian ong đi hút mật mà không làm xáo trộn sinh hoạt tự nhiên của bầy ong.

## 本周金句 (Kim ngôn tuần này)

1、

> "Để giải quyết vấn đề biến đổi khí hậu toàn cầu, nhân loại cần thay đổi thói quen sinh hoạt: ưu tiên sử dụng các dòng xe hơi cỡ nhỏ, tích cực đi bộ hoặc đi xe đạp, cắt giảm các chuyến bay đường dài, hạn chế mua sắm các sản phẩm thời trang nhanh dễ vứt bỏ và giảm tỷ trọng tiêu thụ thịt động vật hàng ngày."
> 
> -- Trích báo cáo khí hậu của BBC.

2、

> "Đầu tiên hãy tập trung xây dựng sản phẩm làm công cụ hữu ích (tool), sau khi có được lượng người dùng trung thành đủ lớn mới bắt đầu phát triển các tính năng kết nối mạng xã hội và cộng đồng (network)."
> 
> -- Chris Dixon

(Hết)
