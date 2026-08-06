# 科技爱好者周刊（第 125 期）：Đồng Nhân dân tệ kỹ thuật số muốn thay thế ai?

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1392) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## Ảnh bìa

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091705.jpg)

Người dân trên đảo Canary, Tây Ban Nha đào hố trồng nho trên tro núi lửa. Tro núi lửa thoát nước nhanh, nho trồng ở đây rất thích hợp để làm rượu vang. ([Nguồn](https://www.instagram.com/p/CFMtHr3jOtR/))

## Chủ đề tuần này: Đồng Nhân dân tệ kỹ thuật số muốn thay thế ai?

Nhân dân tệ kỹ thuật số (e-CNY) đã được đồn đại từ lâu, nhưng truyền thông không nói rõ nó thực chất là gì.

Tuần này, Phó Thống đốc Ngân hàng Nhân dân Trung Quốc viết một [bài viết](https://www.financialnews.com.cn/ll/gdsj/202009/t20200914_200849.html) trả lời ngay dòng đầu tiên:

> "Đồng Nhân dân tệ kỹ thuật số chủ yếu được định vị là tiền mặt đang lưu thông (M0). ... Nhà nước cần sử dụng công nghệ mới để số hóa tiền mặt, cung cấp tiền cơ sở đa dụng cho sự phát triển của nền kinh tế số."

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091414.jpg)

Bây giờ đã rõ, Nhân dân tệ kỹ thuật số không phải là tiền mã hóa (cryptocurrency), mà là hình thức số hóa của tiền mặt Nhân dân tệ, chủ yếu dùng cho thanh toán trực tuyến.

Nhưng thanh toán trực tuyến từ lâu đã không còn là vấn đề nữa, Alipay và WeChat Pay vẫn đang chạy rất tốt, tại sao Ngân hàng Trung ương phải thúc đẩy Nhân dân tệ kỹ thuật số? Bài viết trên giải thích mô hình vận hành của nó:

> **"Ngân hàng Trung ương giữ vị trí trung tâm trong hệ thống Nhân dân tệ kỹ thuật số, chịu trách nhiệm bán buôn Nhân dân tệ kỹ thuật số cho các ngân hàng thương mại được chỉ định và quản lý toàn bộ vòng đời, các ngân hàng thương mại và tổ chức khác chịu trách nhiệm cung cấp dịch vụ đổi và lưu thông Nhân dân tệ kỹ thuật số cho công chúng."**

Bạn thấy đấy, Ngân hàng Trung ương quản lý, chỉ có các ngân hàng thương mại được chỉ định mới được cung cấp dịch vụ cho công chúng. Nghĩa là sau này khi thanh toán trực tuyến, bạn không chỉ dùng WeChat Pay hay Alipay mà còn có thể dùng ứng dụng của ngân hàng thương mại. Nói cách khác, **Nhân dân tệ kỹ thuật số chính là dịch vụ thanh toán trực tuyến của các ngân hàng thương mại.**

Cách đây không lâu, client Nhân dân tệ kỹ thuật số của China Construction Bank bị rò rỉ. Bốn nút chức năng chính trên cùng là Thanh toán, Thu tiền, Quét mã và Chuyển khoản, trùng khớp với tuyên bố của Ngân hàng Trung ương.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091413.jpg)

Tôi nghĩ đó là lý do chính Ngân hàng Trung ương muốn thúc đẩy Nhân dân tệ kỹ thuật số. Cục diện hiện tại là hai gã khổng lồ Internet (Tencent và Alibaba) nắm giữ toàn bộ thanh toán số của cả nước, và họ đều là các công ty tư nhân. Các ngân hàng thương mại quốc doanh hay UnionPay Cloud QuickPass không thể giành nổi thị phần. Ngân hàng Trung ương lo ngại việc thanh toán số bị độc quyền nên muốn các ngân hàng thương mại tham gia vào.

Điều này có lợi cho người tiêu dùng. Hai gã khổng lồ hiện đang chia cắt thị trường, hệ sinh thái Alibaba không hỗ trợ WeChat Pay và ngược lại. Khi Nhân dân tệ kỹ thuật số ra đời, mọi nền tảng bắt buộc phải hỗ trợ (vì nó là tiền tệ pháp định). Tôi đoán tương lai chỉ có một mã QR thống nhất, bất kể bạn quét bằng WeChat, Alipay hay App ngân hàng đều thanh toán được. Không như hiện tại các cửa hàng phải dán hai mã QR xanh và xanh lá.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091703.jpg)

Tuy nhiên, mảng thanh toán số thực chất không mang lại lợi nhuận trực tiếp. Nó không như thẻ tín dụng, bên cung cấp không thu phí dịch vụ mà còn phải bù tiền vận hành. Việc duy trì phần cứng và phát triển phần mềm đòi hỏi đầu tư khổng lồ, yêu cầu độ tin cậy cực cao, không được gián đoạn hay sai sót. WeChat và Alipay chỉ coi thanh toán quét mã là lối vào lưu lượng người dùng chứ không phải nguồn lợi nhuận chính.

Tôi rất tò mò máy chủ Nhân dân tệ kỹ thuật số sau này do ai duy trì? Liệu Ngân hàng Trung ương sẽ lập một bộ phận DevOps chuyên trách không? Nhưng một mảng không kiếm ra tiền, độ khó công nghệ cao, lương kỹ sư cực khủng như vậy thì đơn vị quốc doanh liệu có làm tốt nổi không?

## Khóa học thực chiến phân tích dữ liệu lớn

Ngày nay thế giới đã bước vào kỷ nguyên dữ liệu, ngành dữ liệu phát triển nhanh chóng, nhân sự thiếu hụt hơn 1.5 triệu người, mức lương vượt trội so với các ngành truyền thống. Ước tính 10 năm tới các vị trí liên quan sẽ tăng gấp 5 lần.

Nhiều người muốn vào ngành nhưng gặp khó khăn: không biết học công cụ nào (Excel, SQL, Python...), thiếu kinh nghiệm thực chiến, lo lắng khi phỏng vấn.

Tài liệu khóa học tuần này chính là **《Khóa học thực chiến phân tích dữ liệu lớn》** của **Kaikeba**, với 4 dự án thực chiến giúp bạn tích lũy kinh nghiệm nhanh chóng từ các tình huống thực tế:

- Dự án 1: Dùng Python tự động hóa văn phòng.
- Dự án 2: Trực quan hóa dữ liệu khổng lồ bằng đồ họa.
- Dự án 3: Phân tích dữ liệu thương mại điện tử và hiển thị trực quan.
- Dự án 4: Khám phá phân tích văn bản độ chính xác cao.

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081102.jpg)

Giảng dạy bởi chuyên gia Big Data thầy Phan Hải Siêu. Khóa học trị giá 599 tệ hiện **ưu đãi giá 0 tệ**. Quét mã QR dưới đây để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091604.jpg)

## Tin tức

1、[Máy bay chạy bằng gió ion](https://buzzorange.com/techorange/2018/11/23/plane-with-no-moving-parts/)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020090408.jpg)

Máy bay thường dùng động cơ cánh quạt hoặc phản lực. Gần đây MIT nghiên cứu thành công máy bay dùng dòng điện tạo ra gió ion làm lực đẩy. Từ những năm 1960 người ta đã biết dòng điện chạy giữa các điện cực tạo ra gió ion (hình dưới). Đây là lần đầu tiên hiện tượng này được ứng dụng làm lực đẩy cho máy bay.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020090409.jpg)

Điểm lợi là động cơ không có bộ phận chuyển động cơ khí nên không ồn, giảm chi phí bảo trì và ô nhiễm. Điểm yếu là lực đẩy yếu, hiện mới bay được mô hình nhỏ dưới 10kg, chưa thể chở người.

2、[Bút thử thai điện tử chứa que thử giấy bên trong](https://threadreaderapp.com/thread/1301708467925741568.html)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020090503.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020090504.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020090505.jpg)

Một người dùng Twitter gần đây đã mua bút thử thai điện tử của hãng chẩn đoán Thụy Sĩ. Sau khi tháo ra, anh ngỡ ngàng phát hiện bên trong thực chất là một que thử giấy thông thường. Phần thử nghiệm thực tế là que thử giấy đó chứ không phải mạch điện.

Phần điện tử chỉ gồm các cảm biến quang học đọc vạch trên giấy rồi hiển thị kết quả lên màn hình LCD. Việc này giúp kết quả dễ đọc hơn nhưng làm tăng độ phức tạp và giá bán đắt gấp 25 lần que thử thường.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020090506.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020090507.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020090508.jpg)

3、[Bàn phím giấy](https://www.smithsonianmag.com/smart-news/your-next-digital-tablet-could-be-made-paper-180975727/)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020090603.jpg)

Các kỹ sư Đại học Purdue phát minh công nghệ biến giấy thường (báo cũ hay giấy in) thành bàn phím máy tính. Họ phủ một lớp mực đặc biệt lên giấy rồi đặt mạch điện lên trên. Sự ma sát khi gõ phím tạo ra điện năng tự cấp nguồn cho bàn phím, kết nối Bluetooth với máy tính/điện thoại. Công nghệ này có thể dùng trên bao bì để kiểm tra hạn sử dụng hay hàng thật giả.

4、[Chung cư vườn rừng đô thị](https://sichuan.scol.com.cn/cddt/202007/57855226.html)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091706.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091707.jpg)

Thành phố Thành Đô có dự án chung cư gồm 8 tòa nhà 30 tầng mà mỗi hộ dân đều có sân vườn rộng 40-100 m2 để trồng cây nuôi hoa trông giống như một khu rừng dựng đứng.

Đất vườn dày 60cm, chỗ sát tường có hồ trồng cây sâu hơn 1m để trồng cây cao 4-5m cố định vào tường tránh gió bão, khu vực khác trồng hoa cỏ bụi thấp. Ban quản lý tòa nhà lắp đặt hệ thống tưới nước tự động cho từng nhà.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091708.jpg)

5、[Máy ảnh số lớn nhất thế giới](https://www.bbc.com/news/science-environment-54066586)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091103.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091105.jpg)

Đài thiên văn Vera C. Rubin tại Chile lắp đặt máy ảnh số lớn nhất thế giới độ phân giải 3.2 tỷ pixel (3200 megapixel) để chụp bản đồ sao toàn bầu trời. Cảm biến ảnh gồm 189 chip CCD ghép lại, đang được thử nghiệm lắp ráp tại California.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091104.jpg)

Để thử nghiệm tính năng của nó, các kỹ sư đã dùng nó chụp một bông súp lơ xanh. Dự kiến máy ảnh hoạt động chính thức từ cuối năm 2022.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091102.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091106.jpg)

6、**Tin tức một câu**

> - [Một người dùng Twitter](https://twitter.com/vidister/status/1304542559210024962) cắt đứt dây đồng cáp mạng rồi cắm hai đầu vào quả táo, tín hiệu vẫn truyền qua bình thường với tốc độ mạng rất tốt.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091201.jpg)

> - [Không quân Mỹ](https://www.cnn.com/2020/09/09/us/robot-dogs-us-air-force-test-intl-hnk-scli-scn/index.html) bắt đầu thử nghiệm dùng chó robot tuần tra cùng binh sĩ. Tên chính thức của chó robot là "Phương tiện mặt đất tự hành không người lái".

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091403.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091404.jpg)

> - [Hong Kong](https://edition.cnn.com/style/article/diamond-auction-hong-kong/index.html) chuẩn bị đấu giá viên kim cương 102.39 carat, là viên kim cương trên 100 carat thứ 8 được đấu giá trong lịch sử.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091306.jpg)

> - [Chính phủ Ai Cập](http://world.people.com.cn/n1/2020/0907/c1002-31852279.html) công bố khai quật 13 cỗ quan tài gỗ cổ 2500 năm tuổi còn nguyên niêm phong chưa từng bị mở ra kể từ khi hạ táng.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091307.jpg)

> - [Tập đoàn dầu khí BP](https://www.theguardian.com/business/2020/sep/14/global-oil-demand-may-have-passed-peak-says-bp-energy-report) phát biểu báo cáo nghiên cứu cho rằng lượng tiêu thụ dầu mỏ toàn cầu đã đạt đỉnh trước đại dịch và sẽ có xu hướng giảm dần sau đó.

## Bài viết

1、[Cách viết tiếng Anh đơn giản](http://www.plainenglish.co.uk/how-to-write-in-plain-english.html)（Tiếng Anh）

Hướng dẫn các quy tắc viết tiếng Anh ngắn gọn, dễ hiểu.

2、[Dùng SQL truy vấn log Git](https://willschenk.com/articles/2020/gitlog_in_sqlite/)（Tiếng Anh）

Cách xuất log Git thành cơ sở dữ liệu SQLite để chạy các câu lệnh SQL truy vấn thông tin commit.

3、[Triển khai micro front-end microcosmos](https://juejin.im/post/6864381092061773831)（Tiếng Trung）

Bài viết thảo luận về khái niệm và cách tự viết một framework micro front-end đơn giản. ([@chuifengji](https://github.com/ruanyf/weekly/issues/1407) đóng góp)

4、[Dùng máy tính bảng Android làm màn hình phụ](https://blog.8bitbuddhism.com/2019/12/01/how-to-use-your-android-tablet-as-second-monitor/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091601.jpg)

Cách tận dụng máy tính bảng Android cũ làm màn hình thứ hai cho máy tính thông qua giao thức VNC để hiển thị màn hình điều khiển từ xa.

5、[Giải thích cú pháp `for await ... of`](https://www.mikealche.com/software-development/a-simple-explanation-of-the-for-await-of-statement-in-node-js)（Tiếng Anh）

Cú pháp ES6 dùng để duyệt qua các async iterator, bài viết giải thích dễ hiểu về nó.

6、[6 lý do dùng React Hooks thay vì Class](https://blog.bitsrc.io/6-reasons-to-use-react-hooks-instead-of-classes-7e3ee745fe04)（Tiếng Anh）

Phân tích các ưu điểm của Hooks như loại bỏ vấn đề con trỏ `this` hay việc phải bind phương thức.

7、[Tìm hiểu định dạng ảnh AVIF](https://jakearchibald.com/2020/avif-has-landed/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091711.jpg)

AVIF là định dạng ảnh mã nguồn mở phát triển từ codec video AV1, bài viết so sánh chất lượng và dung lượng của nó với JPEG và WebP.

8、[Cách download file dạng stream trong Node.js](https://philna.sh/blog/2020/08/06/how-to-stream-file-downloads-in-Node-js-with-got/)（Tiếng Anh）

Hướng dẫn dùng thư viện Got để tải file lớn dưới dạng stream trong Node.js.

9、[Tìm bức ảnh đẹp nhất từ thư viện Apple Photos](https://simonwillison.net/2020/May/21/dogsheep-photos/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020052402.jpg)

Ứng dụng Apple Photos tự động chạy mô hình máy học chấm điểm thẩm mỹ (ZBEHAVIORALSCORE) lưu vào SQLite local. Tác giả dùng SQL để lọc ra những bức ảnh đẹp nhất theo chủ đề.

## Công cụ

1、[Diffchecker](https://www.diffchecker.com/)

Công cụ so sánh trực tuyến tìm điểm khác biệt giữa văn bản, hình ảnh, file PDF.

2、[youtube-dlc](https://github.com/blackjack4494/youtube-dlc)

Một công cụ dòng lệnh, nhánh rẽ (fork) của youtube-dl giúp tải video từ Youtube và nhiều trang web khác.

3、[fastmac](https://github.com/fastai/fastmac/)

Dịch vụ chạy terminal macOS miễn phí dựa trên tài nguyên GitHub Actions, phù hợp khi bạn cần test môi trường Mac mà không có thiết bị.

4、[Screely](https://www.screely.com/)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091323.jpg)

Công cụ tạo ảnh mockup màn hình trình duyệt từ ảnh chụp màn hình thô.

5、[Poolside FM](https://poolside.fm/)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091503.jpg)

Trang web nghe nhạc radio phong cách retro thập niên 80 độc đáo. ([@freezsun](https://github.com/ruanyf/weekly/issues/1406) đóng góp)

6、[Mimestream](https://mimestream.com/)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091504.jpg)

Client email native tuyệt đẹp dành riêng cho Gmail trên macOS viết bởi cựu kỹ sư Apple. ([@dushi792](https://github.com/ruanyf/weekly/issues/1408) đóng góp)

7、[real-live](https://github.com/parzulpan/real-live)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091505.jpg)

Ứng dụng xem tivi truyền hình trực tuyến nguồn mở viết bằng Qt/Python hỗ trợ nhiều kênh. ([@parzulpan](https://github.com/ruanyf/weekly/issues/1409) đóng góp)

8、[kibana-eye](https://github.com/CasterWx/kibana-eye)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091507.jpg)

Công cụ quản lý tác vụ định kỳ cho ES/Kibana để tổng hợp log gửi báo cáo qua Email/DingTalk. ([@CasterWx](https://github.com/ruanyf/weekly/issues/1413) đóng góp)

9、[LofiMusic](https://lofimusic.app)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091509.jpg)

Trang web nghe nhạc nền Lofi thư giãn mã nguồn mở.

10、[BeeWare](https://beeware.org/)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091701.jpg)

Bộ công cụ đóng gói code Python thành ứng dụng GUI chạy đa nền tảng, hỗ trợ build thành app iOS/Android.

## Tài nguyên

1、[Aggregated Awesome](https://aggregatedawesome.com/)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091702.jpg)

Trang tổng hợp danh sách các kho lưu trữ "Awesome" chất lượng trên GitHub theo từng chủ đề.

2、[Fuel Collection](https://app.ignitionrobotics.org/GoogleResearch/fuel/collections/Google%20Scanned%20Objects)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091101.jpg)

Bộ sưu tập quét 3D hàng ngàn vật thể hàng ngày do Google thực hiện và chia sẻ miễn phí.

3、[Prime Curios!](https://primes.utm.edu/curios/)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091301.jpg)

Trang web tổng hợp các con số kỳ thú liên quan đến số nguyên tố.

4、[顶级域名列表](http://data.iana.org/TLD/tlds-alpha-by-domain.txt)

Danh sách tất cả 1508 tên miền cấp cao nhất (TLD) chính thức từ IANA.

5、[如何写一个简单的 C 语言解释器](https://github.com/lotabout/write-a-C-interpreter/tree/master/tutorial/en)

Giáo trình tiếng Anh viết trình thông dịch C đơn giản để hiểu sâu nguyên lý trình biên dịch.

6、[WebRTC 示例仓库](https://webrtc.github.io/samples/)

Kho lưu trữ các ví dụ chính thức sử dụng WebRTC cho giao tiếp P2P trên trình duyệt.

## Hình ảnh

1、[Đường Hu](https://zh.wikipedia.org/wiki/%E9%BB%91%E6%B2%B3-%E8%85%BE%E5%86%B2%E7%BA%BF)

Đường nối Hắc Hà và Đằng Xung chia đôi bản đồ Trung Quốc, phía Đông đường này tập trung 94% dân số cả nước từ nghiên cứu năm 1935 của nhà địa lý học Hồ Hoán Dung.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020090907.jpg)

2、[Núi lửa cao nhất hệ Mặt Trời](https://designyoutrust.com/2020/09/olympus-mons-the-largest-volcano-in-the-solar-system/)

Núi lửa Olympus Mons trên sao Hỏa cao 21km gấp 2.5 lần đỉnh Everest là ngọn núi cao nhất hệ Mặt Trời.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091001.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091002.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091003.jpg)

## Bài đọc thêm

### 1. Hành tinh rác thải nhựa

Ngành nhựa mới phát triển 60 năm nhưng nhân loại đã tạo ra 8.3 tỷ tấn nhựa, phần lớn là đồ dùng một lần.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091606.jpg)

Chỉ 9% được tái chế, 12% bị thiêu hủy, 79% còn lại chôn lấp hoặc xả ra đại dương. Dự báo đến 2050 lượng nhựa dưới biển sẽ nhiều hơn cá. Nhựa mất hơn 400 năm để phân hủy.

### 2. Ngô cố định đạm

Không khí chứa 78% là nitơ nhưng hầu hết thực vật không tự hấp thụ được mà phải bón phân đạm. 

Thập niên 1980 nhà khoa học tìm ra giống ngô đặc biệt ở Mexico cao 5-6m không cần phân đạm vẫn lớn tốt trên đất nghèo nhờ có rễ khí thở tiết chất dịch chứa vi khuẩn cố định đạm từ không khí.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091107.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091108.jpg)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091109.jpg)

Nghiên cứu sinh học phân tử sau đó mở ra cơ hội chuyển gene cố định đạm này sang ngô thường để giảm phụ thuộc phân đạm vốn ngốn nhiều năng lượng sản xuất và gây ô nhiễm môi trường biển.

## Danh ngôn

1、

Năm 2002 tôi phỏng vấn Jensen Huang (NVIDIA) tại một khách sạn bình dân ở Trung Quan Thôn, anh ấy nói khẽ với tôi: "Intel có CPU, chúng tôi có GPU". 

Lúc đó trông anh ấy đầy vẻ không tự tin. Tôi cũng chỉ cười xã giao khi anh ấy đặt NVIDIA ngang hàng với Intel. 18 năm sau, vốn hóa NVIDIA đã chính thức vượt qua Intel.

-- Lưu Nhận

2、

Năm 2005, luận văn tốt nghiệp của tôi chứa 152 liên kết tham chiếu URL. Nhân kỷ niệm 15 năm tốt nghiệp, tôi kiểm tra lại và thấy 82 liên kết đã không còn hoạt động. Do đó tôi rút ra tỷ lệ link die của Internet là khoảng 57% sau 15 năm.

-- [《Đo lường tỷ lệ link die》](https://www.lightbluetouchpaper.org/2020/09/03/a-measurement-of-link-rot-57/)

3、

Sự thành công của Lý Quang Diệu ở Singapore không chỉ nhờ tính độc tài của ông, mà còn nhờ tính thực dụng triệt để của giới tinh hoa đưa ra quyết định. Họ không bị trói buộc bởi hệ tư tưởng cố định nào mà chọn giải pháp thực tiễn nhất.

-- Độc giả Hacker News

4、

Mô hình phát triển của ngành phần mềm Internet đã chuyển dịch từ chu kỳ phát triển dài ngày sang tích hợp và triển khai liên tục (CI/CD) tốc độ nhanh, giúp tăng tốc chu kỳ lặp sản phẩm cực kỳ đáng kể.

-- [《Kiểm thử môi trường production với mô hình Dark Canary》](https://engineering.linkedin.com/blog/2020/production-testing-with-dark-canaries)

5、

Bạn có thể nhanh chóng tìm thấy lá bài 3 Rô trong đống bài dưới đây không? Đó chính là cảm giác của người dùng khi nhìn vào một thanh menu điều hướng khổng lồ.

-- [《Giải quyết bài toán Megaton trong Mega Menu》](https://uxmovement.com/navigation/solving-the-megaton-problem-with-mega-menus/)

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091401.jpg)

6、

Ba năm trước chúng tôi chuyển tới London để dạy học và phải đi thuê nhà, giờ thì có thể tự mua nhà được rồi.

-- Phát biểu nhận giải của Giáo sư toán học người Anh Martin Hairer. Ông nhận giải thưởng Breakthrough Prize năm nay trị giá 3 triệu USD, giải thưởng khoa học có giá trị tiền mặt cao nhất thế giới.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091308.jpg)

7、

Nó chưa chết nhưng thực sự đã viết xong.

-- [Moment.js](https://momentjs.com/docs/#/-project-status/) tuyên bố dừng phát triển, chuyển sang chế độ bảo trì.

![](https://cdn.beekka.com/blogimg/asset/202009/bg2020091508.jpg)

## Nhìn lại

Tuần này năm 2019 (số 74): [Tại sao mô hình thương mại của thông tin không phải là thu phí](http://www.ruanyifeng.com/blog/2019/09/weekly-issue-74.html)

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091910.jpg)

Tuần này năm 2018 (số 22): [Chú khỉ tự sướng, bản quyền thuộc về ai](http://www.ruanyifeng.com/blog/2018/09/weekly-issue-22.html)

![](https://cdn.beekka.com/blogimg/asset/201809/bg2018091401.jpg)

## Đăng ký

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97).

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
