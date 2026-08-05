# 科技爱好者周刊：第 103 期 (Bản tin chia sẻ công nghệ số 103)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1148) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## Ảnh bìa

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041604.jpg)

Nhân viên công viên quốc gia Utah, Mỹ vào hang để lắp vòng theo dõi cho một con gấu đang ngủ đông. Không ngờ con gấu chưa ngủ, trợn tròn mắt nhìn họ. May mắn thay nó không tấn công nhân viên, thuốc mê cũng nhanh chóng phát huy tác dụng. ([Nguồn](https://www.natgeomedia.com/explore/article/content-9781.html))

## Chủ đề tuần này: Chu kỳ bán rã của thông tin

Chu kỳ bán rã là một khái niệm vật lý, chỉ thời gian cần thiết để chất phóng xạ giảm đi một nửa khối lượng (suy yếu bức xạ).

Khái niệm này thực ra rất dễ hiểu. Theo công thức năng lượng - khối lượng nổi tiếng nhất của Einstein E=mc², năng lượng tức là khối lượng, bất kỳ vật thể nào giải phóng năng lượng đều nhất thiết sẽ giảm nhẹ khối lượng.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041605.jpg)

Gần đây, tôi thấy [có người](https://www.remote.tools/newsletter/knowledge-decay-and-half-life-of-information) đề xuất một khái niệm mới, họ nói thông tin cũng có chu kỳ bán rã. **Chu kỳ bán rã của thông tin chỉ thời gian cần thiết để một nửa lượng thông tin trở nên không còn liên quan hoặc hoàn toàn lỗi thời.**

Lấy báo làm ví dụ, giá trị lớn nhất vào ngày xuất bản, hôm sau nhìn lại, giá trị ít nhất giảm đi một nửa, vì vậy chu kỳ bán rã của báo là một đến vài ngày. Chu kỳ bán rã của WeChat và Weibo cũng tương tự, bài đăng bạn đăng buổi sáng, buổi tối cũng ít ai xem nữa. Còn chu kỳ bán rã của tin nhắn tức thời hoặc chat lại còn ngắn hơn, chỉ vài giờ.

Xu hướng của xã hội hiện đại là chu kỳ bán rã của thông tin ngày càng ngắn, có một từ gọi là "văn hóa fast food". Trước đây, một cuốn sách mới có thể bán vài năm trong hiệu sách, bây giờ bán vài tháng là xuống kệ rồi, bị các ấn phẩm mới thay thế. Chu kỳ bán rã của phần lớn sách là vài tháng đến một năm.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041606.jpg)

Nếu bạn đã từng viết tài liệu phần mềm, sẽ có cảm nhận sâu sắc về chu kỳ bán rã. Một khi phiên bản phần mềm nâng cấp, giá trị của tài liệu cũ lập tức giảm mạnh. Tôi đã viết tutorial cho React phiên bản 0.14, chỉ trong vài năm, API của nó thay đổi ít nhất ba lần, mỗi lần thay đổi, giá trị của tutorial gốc lại giảm một nửa. Tính ra là biết, trải qua ba chu kỳ bán rã, tài liệu chỉ còn lại một phần tám giá trị.

**Lời khuyên của tôi là, dù bạn viết gì, hãy cố gắng viết những nội dung có chu kỳ bán rã tương đối dài**, điều này có lợi cho việc nâng cao giá trị sử dụng của nội dung (cũng là nâng cao giá trị lao động của bạn). Một số bạn thích đăng WeChat Moments và mạng xã hội, tốn nhiều thời gian, nhưng nội dung ngay lập tức lỗi thời, cũng không thể tái sử dụng.

Nhân tiện, chu kỳ bán rã của bản tin này rất ngắn, qua một tuần là rất ít người xem. Tôi cũng đang nghĩ, làm sao mới có thể kéo dài chu kỳ bán rã của bản tin, để nó có nhiều cơ hội được dùng đến hơn.

## Thuật toán và cấu trúc dữ liệu thiết yếu cho front-end

Kỹ sư front-end cần biết bao nhiêu kiến thức về thuật toán?

Trước đây, kỹ sư front-end được gọi đùa là "kỹ sư cắt hình", tất cả công việc chỉ là trung thực tái hiện bản thiết kế đồ họa, lúc đó thực sự không cần thuật toán nhiều.

Nhưng kể từ khi ứng dụng một trang SPA và phát triển full-stack xuất hiện, tất cả đã thay đổi. Ngày nay nếu bạn không hiểu thuật toán, sẽ chỉ có thể dừng lại ở mức tái hiện giao diện, không thể đảm nhận một số nhiệm vụ phát triển cấp cao. Ví dụ, tối ưu hiệu năng render Virtual DOM, hoặc quản lý cache Node.js. Thực tế, phỏng vấn front-end của các công ty lớn hiện nay, nội dung thuật toán cũng chiếm tỷ trọng không nhỏ.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041408.jpg)

Đây có một tài liệu video miễn phí do **Kaikeba** đặc biệt cung cấp 《Thuật toán và cấu trúc dữ liệu thiết yếu cho front-end》. Tập trung giảng về phân loại học tư duy thuật toán, bao gồm đệ quy, quay lui, tham lam, quy hoạch động, v.v.

Các bạn quan tâm, nhấn giữ mã QR bên dưới hai lần, có thể **nhận miễn phí** những video tutorial này ngay bây giờ.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041405.jpg)

Lưu ý: số lượng tài liệu có hạn, chỉ cung cấp 259 suất.

## Tin tức

1、[Bí ẩn về chuyến bay im lặng của cú mèo](https://www.knowablemagazine.org/article/technology/2020/how-owls-fly-without-making-a-sound)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040909.jpg)

Cú mèo là loài chim lớn, khi giang cánh, sải cánh có thể đạt một đến hai mét. Nhưng, nó bay rất êm, bay đến cách bạn ba mét, bạn sẽ không hề hay biết. Điều này là do rung động không khí do cú mèo bay gây ra, tần số rất thấp, dưới ngưỡng thính giác của con người. Từ lâu, các nhà sinh vật học và kỹ sư đều muốn giải mã bí ẩn bay im lặng của cú mèo, thiết kế ra quạt, cánh tua-bin và cánh máy bay yên tĩnh hơn.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040908.jpg)

Trước đây có người đề xuất, cánh cú mèo có ba điểm đặc biệt: lông ở cạnh trên nhô ra phía trước như lược, cánh hoàn toàn được bao phủ bởi một lớp lông mịn như nhung, lông ở cạnh dưới tạo thành những tua rua lởm chởm (hình trên). Gần đây, các nhà khoa học Mỹ công bố bài báo, đề xuất học hỏi từ cánh cú mèo, giảm độ cứng của cạnh sau cánh máy bay, đồng thời áp dụng cấu trúc có lỗ hổng, làm cho nó linh hoạt hơn. Qua thử nghiệm của họ, có thể giảm tiếng ồn khoảng 10 decibel.

2、[Nhà mô-đun hóa](https://www.dwellito.com/modular-homes)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041103.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041102.jpg)

Một công ty khởi nghiệp Mỹ ra mắt nhà mô-đun hóa. Nhà máy làm sẵn các mô-đun nhà khác nhau, trực tiếp dùng xe tải chở đến hiện trường lắp đặt, có thể nhanh chóng vào ở. Giá từ vài nghìn đô la đến vài trăm nghìn đô la.

Nó cung cấp nhiều giao diện năng lượng, có thể kết nối nguồn điện bên ngoài, cũng có thể kết nối máy phát điện hoặc tấm pin mặt trời. Nếu lắp đặt là nhà ở, hiện trường còn phải kết nối đường ống thoát nước. Vì là nhà mô-đun hóa, việc tháo dỡ và thay thế linh kiện rất tiện lợi. Tuy nhiên, loại nhà này không thể xây cao tầng, nên chỉ thích hợp ở nông thôn.

3、[Xe đo thân nhiệt không người lái](https://3g.163.com/tech/article/F9U2QL8O0514R9OJ.html)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041201.jpg)

Đại học Công nghệ Bắc Kinh triển khai một xe đo thân nhiệt không người lái ở cổng trường để đo nhiệt độ người vào trường. Một khi phát hiện ai có thân nhiệt cao, sẽ phát ra âm thanh báo động.

Chức năng ban đầu của xe là xe giao hàng không người lái, có thể vận chuyển kiện hàng đến đích. Sau khi người nhận đến hiện trường, camera trên đỉnh xe sẽ nhận dạng khuôn mặt người nhận. Chỉ khi nhận dạng thành công, người nhận mới có thể mở cửa kho trên xe lấy kiện hàng.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041202.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041203.jpg)

4、[Địa nhiệt phát điện](https://grist.org/energy/as-oil-crashes-americas-untapped-energy-giant-could-rise/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041303.jpg)

Gần đây giá dầu lao dốc, một kết quả bất ngờ là điều này mang đến cơ hội phát triển cho địa nhiệt phát điện của Mỹ. Vì giá dầu quá thấp, công ty dầu mỏ buộc phải ngừng sản xuất, máy móc khai thác nhàn rỗi vừa hay có thể dùng để khoan thăm dò cho địa nhiệt phát điện.

Càng gần tâm Trái đất, nhiệt độ càng cao, vì vậy có thể sử dụng năng lượng từ nhiệt độ cao dưới lòng đất để phát điện. Địa nhiệt phát điện có nhiều ưu điểm, rất đáng tin cậy, không bị gián đoạn, không có bất kỳ ô nhiễm nào. Nhược điểm duy nhất là chi phí xây dựng cao, đắt hơn nhiều so với nhà máy điện mặt trời. Phần lớn chi phí phát sinh ở khoan thăm dò, cần khoan xuống lòng đất hơn 1000 mét mới có thể đạt nhiệt độ cao 150 độ, vì vậy giá khoan giảm là tin tốt lành nhất cho nó.

5、[Theo dõi Bluetooth](https://www.apple.com/newsroom/2020/04/apple-and-google-partner-on-covid-19-contact-tracing-technology/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041101.jpg)

Apple thông báo hợp tác với Google, cung cấp API theo dõi Bluetooth cho điện thoại, dùng để theo dõi người tiếp xúc gần với bệnh nhân nhiễm virus. Đây có lẽ là lần hợp tác đầu tiên giữa iOS và Android.

Nguyên lý của API này là, Bluetooth của điện thoại phát ra ngoài một mã định danh duy nhất, điện thoại khác nhận được mã định danh này sẽ ghi lại, có hiệu lực hai tuần. Nếu bạn phát hiện mình bị nhiễm virus, hãy tải lên mã định danh duy nhất của mình lên đám mây. Các điện thoại khác sẽ đồng bộ danh sách này, một khi phát hiện mã định danh trong danh sách từng xuất hiện trong nhật ký, người đó nên tự cách ly. Giới thiệu chi tiết có thể tham khảo [ở đây](https://joekent.nyc/google-apple-contact-tracing).

6、**Tin tức một câu**

> - [Có người](https://milliondollarmetropolis.com/) đã làm phiên bản WebGL của "trang chủ lưới triệu đô", bán vĩnh viễn quảng cáo tòa nhà ảo trên trang. Tôi thấy khá sáng tạo.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041401.jpg)

> - [GitHub](https://github.blog/2020-04-14-github-is-now-free-for-teams/) tuyên bố, kho riêng tư của nhóm cũng miễn phí rồi. Nghĩa là, về cơ bản nó là một trang web miễn phí, các tính năng cốt lõi gần như đều không mất tiền, chỉ còn phiên bản doanh nghiệp thu phí.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041407.jpg)

> - [Chính phủ Phần Lan](http://demoscene-the-art-of-coding.net/2020/04/15/breakthrough-finland-accepts-demoscene-on-their-national-list-of-intangible-cultural-heritage-of-humanity/) phê duyệt văn hóa số Demoskene trở thành di sản văn hóa nhân loại, đây có thể là di sản văn hóa đầu tiên trên thế giới liên quan đến phần mềm. Hình thức phổ biến nhất của Demoskene là các buổi tụ họp của những người đam mê, trưng bày âm nhạc, đồ họa, video, v.v.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041602.jpg)

> - Doanh thu bán hàng năm 2019 của [Instagram](https://www.bloomberg.com/news/articles/2020-02-04/instagram-generates-more-than-a-quarter-of-facebook-s-sales) là 20 tỷ đô la. So với đó, doanh thu bán hàng của Youtube là 15 tỷ đô la, và phần lớn trong đó vẫn phải chia cho nhà sáng tạo video.

> - [Nhật Bản](https://www.nytimes.com/2020/02/03/climate/japan-coal-fukushima.html) sẽ xây mới tới 22 nhà máy điện than trong năm năm tới. Đây là hậu quả của kế hoạch buộc Nhật Bản đóng cửa gần như tất cả nhà máy điện hạt nhân sau thảm họa Fukushima gần mười năm trước.

> - [Thống kê phát hiện](https://marginalrevolution.com/marginalrevolution/2020/01/ceo-ages-at-hire.html), trong 14 năm qua, tuổi nhậm chức CEO của các công ty trong S&P 500 đã tăng lên 14 tuổi. Điều này cho thấy, các công ty lớn của Mỹ gần đây thích bổ nhiệm CEO nhiều tuổi hơn.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020020101.jpg)

## Bài viết

1、[Tìm hiểu về địa ngục phụ thuộc JavaScript](https://blog.appsignal.com/2020/04/09/ride-down-the-javascript-dependency-hell.html)（Tiếng Anh）

Khi cài đặt Gatsby.js, sẽ tải xuống 19.000 module phụ thuộc. Bài viết này giải thích cách phân tích các phụ thuộc của Node.js.

2、[10 mẹo sử dụng GitHub](https://github.blog/2020-04-09-github-protips-tips-tricks-hacks-and-secrets-from-lee-reilly/)

Chính thức giới thiệu 10 mẹo sử dụng GitHub, rất thực dụng, khuyến nghị đọc.

3、[Nhà tôi lắp điện mặt trời như thế nào](https://www.mobile01.com/topicdetail.php?f=360&t=6065849)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041304.jpg)

Một bài đăng forum của người dùng Đài Loan, có nhiều hình ảnh, giới thiệu cách họ lắp tấm pin mặt trời trên mái nhà, đơn giản đạt được công suất 1000 watt.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041305.jpg)

4、[Dừng dạy Java bằng Eclipse](https://nora.codes/post/stop-making-students-use-eclipse/)（Tiếng Anh）

Bài viết này đề xuất dạy Java cho người mới bắt đầu, không nên dạy qua IDE (ví dụ Eclipse). Như vậy, trọng tâm giảng dạy sẽ trở thành cách sử dụng IDE, chứ không phải bản thân ngôn ngữ.

5、[Lệnh mv không cần gõ tên file hai lần](https://news.ycombinator.com/item?id=22860140)（Tiếng Anh）

Lệnh `mv` dùng để đổi tên file, cần nhập tên file hai lần (tên cũ và tên mới). Nếu bạn chỉ thay đổi một ký tự, mà tên file lại đặc biệt dài, thì rất phiền. Đây có một mẹo Bash, có thể giúp bạn giảm thiểu lượng nhập.

6、[Tại sao tôi chọn NextDNS](https://angristan.xyz/2020/04/nextdns/)（Tiếng Anh）

DNS là một giao thức cần thiết để lên mạng. Hiện nay nhiều nhà cung cấp dịch vụ cung cấp tính năng chặn quảng cáo và chặn theo dõi ở cấp DNS, tác giả bài viết giới thiệu tại sao chọn NextDNS.

7、[Bảng băm phân tán (DHT) và công nghệ P2P](https://luyuhuang.github.io/2020/03/06/dht-and-p2p.html)（Tiếng Trung）

Mạng P2P phân tán thường sử dụng bảng băm phân tán (DHT) để định tuyến, tìm kiếm các nút xung quanh. Bài viết này giới thiệu kiến thức cơ bản về DHT và nguyên lý triển khai thuật toán. (@[luyuhuang](https://github.com/ruanyf/weekly/issues/1178) đóng góp)

8、[Tutorial xây dựng Docker image: Giảm kích thước image](https://fuckcloudnative.io/posts/docker-images-part1-reducing-image-size/)（Tiếng Trung）

File Docker image tự làm thường có kích thước rất lớn. Bài viết này giới thiệu cách từng bước nén kích thước file image, nén "hello world" ngôn ngữ C từ 1 GB ban đầu xuống còn 94 KB. (@[lupus721](https://github.com/ruanyf/weekly/issues/1184) đóng góp)

9、[CTO làm gì？](https://www.hashtagcoder.dev/blog/director-of-engineering)（Tiếng Anh）

Tác giả ban đầu là kỹ sư của một công ty nhỏ 6 người, sau đó vì công việc kinh doanh của công ty mở rộng nhanh chóng, ông được thăng chức làm Giám đốc kỹ thuật (CTO). Ông mất ba năm mới hiểu rõ trách nhiệm của CTO là gì, chia thành ba phần: sản phẩm, quy trình, nhân sự.

## Công cụ

1、[markmap-lib](https://markmap.js.org/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041001.jpg)

Công cụ mã nguồn mở chuyển đổi Markdown thành sơ đồ tư duy.

2、[codefence](https://codefence.io/)

Trình soạn thảo code tương tác có thể nhúng vào trang web, người dùng có thể trực tiếp nhập code trên trang web và chạy, nhận kết quả. Phía server là container Docker, hiện hỗ trợ hàng chục ngôn ngữ máy tính phổ biến.

3、[droppy](https://github.com/silverwind/droppy)

Dịch vụ mạng riêng tư có thể tự dựng, phù hợp triển khai trên mạng nội bộ, tải lên và tải xuống file qua giao diện Web.

4、[aind](https://github.com/aind-containers/aind)

Một trình giả lập Android trong container Docker.

5、[jott.live](https://jott.live/)

Trang web ghi chú Markdown nhẹ, không cần đăng ký, chỉ cần đặt mật khẩu cho tài liệu, thích hợp để nhanh chóng viết gì đó và chia sẻ.

6、[Tablist](https://chrome.google.com/webstore/detail/tablist/eagbohciligljbgpbdbflaloangiodhe)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041302.jpg)

Plugin trình duyệt Chrome, có thể liệt kê URL trang web của tất cả Tab cùng một lúc, tiện để sao chép.

7、[iKeep](https://github.com/brenner8023/iKeep)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041404.jpg)

Mini program WeChat lập kế hoạch thời gian mã nguồn mở. (@[brenner8023](https://github.com/ruanyf/weekly/issues/1185) đóng góp)

8、[Feeds Pub](https://feeds.pub/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041601.jpg)

Trình đọc RSS xã hội hóa, ngoài tính năng tổng hợp RSS thông thường, còn thêm một số thuộc tính xã hội hóa. (@[timqian](https://github.com/ruanyf/weekly/issues/1189) đóng góp)

9、[JSON Generator](https://next.json-generator.com/)

Công cụ trực tuyến tạo dữ liệu JSON ảo, có thể tự động tạo dữ liệu JSON theo schema cho trước.

10、[Branca](https://branca.io/)

Một định dạng dữ liệu token bảo mật, an toàn hơn JWT, dự án cùng loại còn có [Paseto](https://paseto.io/).

## Tài nguyên

1、[NYC Cams](https://jott.live/html/nyc_cams)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041301.jpg)

Xem camera trên đường phố New York theo thời gian thực.

2、[Nhập môn ngôn ngữ Haskell](http://dev.stephendiehl.com/hask/)

Sách điện tử miễn phí tiếng Anh.

3、[Godot 101 – Nền tảng engine game](https://academy.zenva.com/product/godot-101-game-engine-foundations/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041311.jpg)

Tutorial miễn phí về engine game Godot.

4、[RFC1180: Tutorial TCP/IP](https://tools.ietf.org/html/rfc1180)

Một tutorial tiếng Anh đầu tiên về giao thức TCP/IP, được nộp với tư cách là RFC 1180.

5、[《Tự truyện Snowden》](https://a.temporaryrecord.com/)

Tự truyện Snowden 《Hồ sơ vĩnh cửu》, bản PDF tiếng Trung giản thể không bị kiểm duyệt để tải xuống, được tác giả ủy quyền.

6、[Tài nguyên học lập trình hợp ngữ x64](https://news.ycombinator.com/item?id=22279051)（Tiếng Anh）

Đây là bài thảo luận trên Hacker News, liệt kê các tài nguyên học ngôn ngữ hợp ngữ x86 miễn phí trên mạng.

## Hình ảnh

1、[Lâu đài Guédelon](https://en.wikipedia.org/wiki/Gu%C3%A9delon_Castle)

Lâu đài Guédelon là một dự án khảo cổ thực nghiệm của Pháp, sử dụng vật liệu và phương pháp thời Trung cổ để xây dựng một lâu đài từ đầu.

Bắt đầu khởi công năm 1997, do không sử dụng máy móc hiện đại nên xây rất chậm, dự kiến hoàn thành năm 2023.

Năm 2000.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041306.jpg)

Năm 2006.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041307.jpg)

Năm 2009.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041308.jpg)

Năm 2015.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041309.jpg)

Năm 2019.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041310.jpg)

2、[Tải xuống hình minh họa sinh vật](https://www.flickr.com/photos/biodivlibrary/)

Thư viện Di sản Đa dạng sinh học (Biodiversity Heritage Library, BHL) cung cấp hơn 15.000 hình minh họa sinh vật, có thể tải xuống miễn phí, đều đến từ các tài liệu lịch sử khác nhau.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021103.jpg)

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021104.jpg)

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021105.jpg)

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021106.jpg)

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021107.jpg)

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021108.jpg)

## Bài đọc thêm

1、[Vũ khí động năng trên quỹ đạo](https://zh.wikipedia.org/wiki/%E5%A4%A9%E5%9F%BA%E5%8B%95%E8%83%BD%E6%AD%A6%E5%99%A8)

Vũ khí động năng trên quỹ đạo là loại vũ khí hủy diệt hàng loạt ở giai đoạn khái niệm, tất cả công nghệ đã được thực hiện.

Ý tưởng ban đầu đến từ việc triển khai tên lửa hạt nhân trên vệ tinh không gian, trong thời chiến trực tiếp rơi xuống lãnh thổ kẻ thù, điều này sẽ rút ngắn đáng kể thời gian phản ứng của đối phương. Tuy nhiên, không lâu sau có người đề xuất bất kỳ vật thể có khối lượng nào rơi từ độ cao vệ tinh, sức sát thương không khác gì thiên thạch va vào Trái đất, không cần vũ khí hạt nhân cũng có thể đạt hiệu quả tương tự vũ khí hạt nhân.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041002.jpg)

Khái niệm này ngày càng phổ biến, vì ô nhiễm phóng xạ và nhạy cảm chính trị của vũ khí hạt nhân, làm cho tính chính đáng của việc sử dụng vũ khí hạt nhân trước rất khó đứng vững trong cộng đồng quốc tế, chi phí duy trì đầu đạn hạt nhân trong không gian cũng cao kinh khủng. Trong khi đó loại vũ khí quỹ đạo mới này tốc độ phản ứng nhanh, độ chính xác cao, không có phóng xạ, cũng không vi phạm bất kỳ hiệp ước vũ khí hạt nhân quốc tế hiện hành nào, sức mạnh có thể dễ dàng điều chỉnh qua khối lượng đạn.

Về lý thuyết, một thanh đạn kim loại tungsten, titan hoặc uranium rộng 30 cm, dài 6,1 m, nặng vài tấn có thể xuyên qua giai đoạn đốt trong khí quyển, rơi từ không gian cách mặt đất 1000 km với tốc độ hơn 15.000 km/h, tương đương 11,5 tấn thuốc nổ TNT, động năng va chạm tạo ra có thể sánh với vũ khí hạt nhân chiến thuật nhỏ.

2、[Tai nạn Apollo 13](https://baike.baidu.com/item/%E9%98%BF%E6%B3%A2%E7%BD%9713%E5%8F%B7/3965)

50 năm trước vào tuần này, ngày 13 tháng 4 năm 1970, tàu vũ trụ đổ bộ Mặt trăng Apollo 13 của Mỹ gặp tai nạn. Nhưng, ba phi hành gia đã trở về Trái đất thành công, trở thành huyền thoại lịch sử hàng không vũ trụ.

Khi đó, cảm biến của một bình oxy bị trục trặc, khi phi hành gia kiểm tra công tắc, xảy ra vụ nổ, tàu vũ trụ bị hư hại nhất định. Tệ nhất là, oxy trong cả hai bình oxy đều bị mất hoàn toàn, pin nhiên liệu cần oxy để duy trì hoạt động, chỉ còn điện cho 10 giờ.

Để tiết kiệm điện, phi hành gia chỉ có thể tắt hệ thống sưởi, và từ bỏ tàu chính, ngồi mô-đun đổ bộ Mặt trăng trở về Trái đất. Mô-đun đổ bộ ban đầu được thiết kế để hai phi hành gia sử dụng hai ngày, nay lại nhồi thêm ba phi hành gia. Nồng độ CO2 tăng nhanh, trung tâm chỉ huy mặt đất nghĩ ra một cách, hướng dẫn phi hành gia dùng vật liệu còn lại, lắp ráp thành một bộ lọc, thành công giảm nồng độ CO2 trong mô-đun đổ bộ.

Hệ thống đẩy chính của tàu đã không còn đáng tin cậy, họ đành sau khi bay vòng qua phía sau Mặt trăng, phóng một tên lửa để tăng tốc, sau đó tự do rơi về phía Trái đất. Trên đường trở về, ba phi hành gia được thông báo không được xả nước tiểu hoặc chất lỏng khác ra ngoài khoang, vì điều này sẽ ảnh hưởng đến quỹ đạo rơi của mô-đun đổ bộ.

Toàn bộ quá trình kéo dài bốn ngày, ba phi hành gia cuối cùng an toàn trở về Trái đất. Để phân tích nguyên nhân tai nạn, trung tâm chỉ huy yêu cầu phi hành gia chụp ảnh tàu vũ trụ, trở thành tài liệu lịch sử quý giá. Dưới đây là ảnh chụp chung ba người của họ trước khi vào khí quyển Trái đất.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041403.jpg)

Phân tích sau đó, điều may mắn nhất trong toàn bộ tai nạn là, tàu vũ trụ gặp vấn đề trên đường đến Mặt trăng, chứ không phải trên đường về. Nếu tai nạn xảy ra sau khi đổ bộ, do tài nguyên còn lại sẽ giảm nhiều, phi hành gia sẽ khó có thể sống sót. Nếu hoàn thành nhiệm vụ đổ bộ bình thường, mô-đun đổ bộ sẽ bị loại bỏ, ba phi hành gia sẽ không còn khoang cứu sinh.

## Danh ngôn & Con số

1、

Lập trình viên 501 chỉ những lập trình viên, đúng 5 giờ 01 là rời văn phòng về nhà.

-- 《[Tuyên ngôn lập trình viên 501](https://501manifesto.dev/)》

2、

Một trong những vấn đề lớn nhất của ngành phần mềm là phải liên tục tuyển người mới. Vì phần mềm liên tục bị hỏng, luôn cần phải tháo dỡ và xây dựng lại hoàn toàn.

-- 《[Vấn đề lớn nhất của ngành phần mềm](https://www.neilwithdata.com/developer-hiring)》

3、

Ông ấy yêu toán học đến mức không thể hình dung, tại sao học sinh trong lớp ông lại quan tâm đến điểm số của mình.

-- 《[Nhà toán học John Conway qua đời](https://news.ycombinator.com/item?id=22845374)》

4、

Vi sinh vật đã biết có tính gây bệnh cho con người, có khoảng 1.400 loài, trong đó khoảng 500 loài vi khuẩn, khoảng 200 loài virus, phần còn lại là các loại nấm, sán và nguyên sinh động vật khác nhau.

-- [《Mầm bệnh và kỷ nguyên Nhân sinh》](https://inhabitingtheanthropocene.com/2017/10/18/pathogens-and-the-anthropocene-germs-genes-geography-part-1/)

5、

Nếu muốn bảo tồn thứ gì đó lâu dài, đừng dùng thứ không bền để làm nền tảng của nó.

Có một số công nghệ, không phù hợp để xây dựng website lâu dài. Bạn có thể tưởng tượng vận hành một trang web WordPress liên tục 25 năm không? Phiên bản PHP mà nó phụ thuộc sẽ không chạy được từ rất sớm rồi.

-- [Độc giả HN](https://news.ycombinator.com/item?id=22326930), bình luận về một trang web được làm bằng FrontPage, 18 năm sau vẫn đang cập nhật.

6、

Vài năm trước, tôi mở một trang web cộng đồng, thường có người đến phá hoại, thêm vào danh sách đen, chặn địa chỉ IP đều không có tác dụng, họ sẽ thay đổi tên người dùng và địa chỉ IP.

Cuối cùng, tôi nghĩ ra một cách, tăng thời gian render mỗi trang lên 5 đến 25 giây, làm cho trải nghiệm website kém. Sau vài ngày, những người này không còn xuất hiện nữa.

-- [Độc giả HN](https://news.ycombinator.com/item?id=22321023)

## Nhìn lại

Tuần này năm ngoái: [《Bản tin số 52》](http://www.ruanyifeng.com/blog/2019/04/weekly-issue-52.html)

![](https://cdn.beekka.com/blogimg/asset/201904/bg2019041901.jpg)

## Đăng ký

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97).

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
