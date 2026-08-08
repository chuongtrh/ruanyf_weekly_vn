# 科技爱好者周刊（第 230 期）：电子产品的用电量

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần。

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn。

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2715) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập。

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110906.webp)

Hệ thống máy phát thuốc tự động lắp đặt tại Bệnh viện số 1 thuộc Đại học Chiết Giang. Ngay khi bác sĩ hoàn tất kê đơn trên hệ thống, cánh tay robot cơ khí sẽ tự động lấy các loại thuốc tương ứng từ tủ lưu trữ và chuyển phát nhanh qua hệ thống đường ống khí nén tới quầy cấp phát cho bệnh nhân nhận thuốc. (Nguồn: [CN-Healthcare](https://www.cn-healthcare.com/articlewm/20221101/wap-content-1459477.html))

## 本周话题：电子产品的用电量

Trong số bản tin [tuần trước](https://www.ruanyifeng.com/blog/2022/11/weekly-issue-229.html), chúng ta đã đề cập đến việc công suất của các củ sạc điện thoại di động thế hệ mới hiện nay đã chính thức vượt mốc 200W.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102908.webp)

Đây là một mức công suất tiêu thụ điện năng cực kỳ lớn. Nhiều người có thể không biết rằng con số này thậm chí đã vượt qua mức tiêu thụ điện năng trung bình của chiếc tủ lạnh gia đình bạn (thường dao động trong khoảng từ 100W đến 200W).

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110823.webp)

*(Tủ lạnh gia đình dung tích 200 lít thường có công suất hoạt động khoảng 140W, tiêu thụ xấp xỉ 1 số điện mỗi ngày).*

Sự kiện này phản ánh rõ nét một xu hướng phát triển công nghệ gần đây: **Công suất tiêu thụ điện của các thiết bị công nghệ số đang gia tăng phi mã, tiệm cận hoặc vượt mặt các thiết bị gia dụng truyền thống.** Tôi xin chia sẻ hai câu chuyện thực tế:

**Câu chuyện thứ nhất**: Gần đây tôi có mua một chiếc ổ cắm điện thông minh có tính năng theo dõi và hiển thị công suất tiêu thụ điện thời gian thực trên điện thoại.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110824.webp)

Tôi đã cắm thử nghiệm chiếc màn hình máy tính 27-inch độ phân giải 4K của mình vào ổ cắm này. Bảng thống kê lượng điện tiêu thụ hàng tháng của thiết bị cho thấy chiếc màn hình có công suất ghi danh 30W này đã ngốn hết **13,8 số điện (kWh)** trong tháng qua:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110825.webp)

Con số này thực sự khiến tôi ngỡ ngàng. Màn hình 4K tiêu tốn nhiều điện năng hơn tôi tưởng. Trên bàn làm việc của tôi hiện lắp đặt đồng thời 3 màn hình tương tự, nghĩa là riêng hệ thống hiển thị này đã ngốn khoảng 40 số điện mỗi tháng.

**Câu chuyện thứ hai**: Gần đây xuất hiện nhiều [tin tức báo chí](https://www.igorslab.de/en/adapter-of-the-gray-analyzed-nvidias-brand-hot-12vhpwr-adapter-with-built-in-breakpoint/) phản ánh hiện tượng cháy hỏng cổng cấp nguồn trên dòng card đồ họa cao cấp mới nhất NVIDIA RTX 4090 của người dùng.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102808.webp)

Nếu tìm hiểu kỹ thông số phần cứng, sự cố này là điều hoàn toàn dễ hiểu. Dòng card đồ họa này là một "quái vật" ngốn điện thực sự với công suất đỉnh đạt tới **600W**. Trong khi đó, điện áp cấp nguồn tiêu chuẩn bên trong thùng máy tính PC chỉ là 12V, đồng nghĩa cường độ dòng điện đi qua dây nguồn đạt mức cực cao lên tới **50A** (600W / 12V).

Để phân tán cường độ dòng điện khổng lồ này, hãng sản xuất phải sử dụng cổng cắm 12 chân nối song song. Dù vậy, chỉ cần chân cắm tiếp xúc không hoàn toàn khít hoặc bị lỏng nhẹ, nhiệt lượng sinh ra tại điểm tiếp xúc sẽ tăng vọt dẫn tới nóng chảy cổng cắm nhựa:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102806.webp)

Đây mới chỉ là lượng điện tiêu thụ của riêng card đồ họa. Nếu kết hợp với bộ vi xử lý trung tâm Intel Core i9-13900K (công suất khoảng 360W) và các linh kiện ổ cứng, quạt tản nhiệt đi kèm, tổng công suất của một thùng máy tính PC cấu hình cao để chơi game đã chạm mốc **1000W** (tương đương công suất của một chiếc máy điều hòa nhiệt độ).

Hai câu chuyện trên minh chứng rõ nét: **Cùng với sự gia tăng của năng lực tính toán, máy tính đang trở thành một thiết bị tiêu tốn điện năng khổng lồ.**

Hiện nay, các mô hình trí tuệ nhân tạo (AI) thông minh nhất thế giới đều được xây dựng trên nền tảng năng lực tính toán cực lớn. Khái niệm "thông minh" thực chất đang được đánh đổi bằng lượng tiêu thụ điện năng khổng lồ. Các [nghiên cứu khoa học](https://www.infoq.cn/article/kyspl1wjruoxqtufgodx) chỉ ra rằng *"năng lượng tiêu thụ để huấn luyện hoàn chỉnh một mô hình AI lớn tương đương với lượng khí thải carbon của 5 chiếc ô tô hoạt động suốt vòng đời"*. Nhiều mô hình AI phức tạp thậm chí đòi hỏi lượng điện năng cung cấp từ cả một nhà máy thủy điện nhỏ để vận hành.

Trong tương lai, khi mọi thiết bị xung quanh chúng ta đều kết nối Internet (IoT) và được tích hợp các bộ xử lý AI thông minh chạy ngầm, nhu cầu điện năng của nhân loại sẽ đạt tới những con số thiên văn.

Chúng ta có thể khẳng định rằng: **Kỷ nguyên số hóa thông tin thực chất là một kỷ nguyên vô cùng đói khát năng lượng điện.** Khi xã hội loài người tiến tới tự động hóa hoàn toàn, lượng nhà máy điện cần xây dựng thêm để duy trì hệ thống chắc chắn sẽ là một bài toán lớn.

## 小程序容器 FinClip

Các ứng dụng di động (App) hiện nay thường có dung lượng cài đặt lên tới hàng chục hay hàng trăm MB, tạo gánh nặng lớn cho cả lập trình viên khi bảo trì và người dùng khi tải về.

Giới công nghệ vẫn luôn tìm kiếm các giải pháp xây dựng ứng dụng siêu nhẹ (Light App) tiêu biểu như công nghệ PWA (Progressive Web Apps), Apple App Clips hay Google Instant Apps. Nhưng giải pháp thành công và phổ biến nhất tại thị trường trong nước chính là mô hình **Tiểu chương trình (Mini-Program)**.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110401.webp)

Về bản chất kỹ thuật, **Mini-Program là một công nghệ phát triển ứng dụng phổ quát**:

*Nói một cách đơn giản, Mini-Program là các trang giao diện xây dựng trên nền tảng HTML/CSS/JS chạy bên trong một bộ chứa bảo mật (App chủ quản), có khả năng gọi các API hệ thống của thiết bị như đọc tệp, camera, bluetooth... thông qua cầu nối trung gian (JSBridge).*

Bên cạnh WeChat Mini-Program quen thuộc, nhiều nền tảng lớn như Alipay, Baidu, Meituan, JD, Kuaishou đều tự phát triển các bộ chứa ứng dụng nhỏ riêng của mình:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110402.webp)

Để giúp các ứng dụng di động của các doanh nghiệp khác dễ dàng tích hợp và vận hành các ứng dụng nhỏ này, công nghệ "Bộ chứa ứng dụng nhỏ" (Mini-Program Container) đã ra đời.

**Mini-Program Container thực chất là một môi trường thực thi gọn nhẹ.** Khi nhà phát triển tích hợp bộ SDK này vào mã nguồn App của mình, App đó lập tức có năng lực khởi chạy các ứng dụng nhỏ tương tự như cách WeChat vận hành hệ sinh thái của họ.

Trong số các giải pháp trên thị trường hiện nay, [FinClip](https://www.finclip.com/) là một trong những công nghệ nổi bật và đi đầu:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110821.webp)

FinClip cung cấp bộ SDK hỗ trợ đa nền tảng từ di động (iOS/Android) đến máy tính để bàn (Windows/Linux/macOS), các thiết bị thông minh trên xe hơi hay đồng hồ thông minh. **Chỉ cần ứng dụng tích hợp bộ SDK của FinClip (làm tăng kích thước bộ cài đặt thêm khoảng 3MB), App của bạn đã có thể chạy trực tiếp các ứng dụng nhỏ WeChat Mini-Program mà không cần sửa đổi bất kỳ dòng code nào.**

Sản phẩm tương thích hoàn toàn với cú pháp WXML của WeChat, giúp nhà phát triển có thể phân phối ứng dụng của mình đồng thời trên cả WeChat và App riêng của doanh nghiệp một cách đồng bộ.

Ngoài ra, FinClip cũng cung cấp môi trường IDE chuyên dụng hỗ trợ biên dịch và xuất gói mã nguồn Mini-Program thành các tệp cài đặt App độc lập (.apk hoặc .ipa) để đưa lên các chợ ứng dụng di động một cách nhanh chóng.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110404.webp)

Công nghệ của FinClip đã được triển khai thực tế và chứng minh độ ổn định trên hệ thống của nhiều ngân hàng, công ty chứng khoán và hãng hàng không lớn, chịu tải lượng truy cập đồng thời khổng lồ của hơn 25 triệu người dùng.

Dịch vụ được cung cấp miễn phí cho các lập trình viên cá nhân và dự án nhỏ. Nhà phát triển quan tâm có thể đăng ký tài khoản trải nghiệm tại [Trang chủ FinClip](https://www.finclip.com/login/?type=register&from=home).

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110803.webp)

## 科技动态

1、[Hệ thống tủ kính trồng rau xanh trang trí sảnh của khách sạn JW Marriott](https://www.fastcompany.com/90740481/why-jw-marriott-is-planting-edible-gardens-is-every-one-of-its-hotels)

Chuỗi khách sạn JW Marriott đã triển khai lắp đặt các tủ kính nông nghiệp công nghệ cao tại sảnh chờ của 25 khách sạn thành viên:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051609.webp)

Tủ kính có chiều cao 2,1m tích hợp hệ thống đèn tia cực tím giả lập ánh sáng mặt trời để gieo trồng các loại rau xanh, rau thơm thảo mộc và quả nhỏ:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051610.webp)

Mặc dù sản lượng rau thu hoạch được từ hệ thống đèn nhân tạo này khá thấp và tốn chi phí điện, thiết bị đóng vai trò như một tác phẩm nghệ thuật xanh trang trí sảnh ấn tượng thay thế cho hoa tươi truyền thống. Lượng rau thơm sau khi thu hoạch được chuyển trực tiếp cho nhà bếp chế biến món ăn phục vụ thực khách.

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051611.webp)

2、[Ý tưởng thiết kế hệ thống thu hồi nhiệt lượng từ nước thải phòng tắm](https://dynomight.net/hot-water/)

Trong bối cảnh chi phí năng lượng sưởi ấm gia tăng tại Anh, một cư dân mạng đã đề xuất giải pháp kỹ thuật nhằm tái tận dụng nhiệt lượng từ nước tắm ấm trước khi xả ra cống:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110315.webp)

Phần lớn lượng nhiệt dùng để đun nước tắm bị lãng phí khi nước nóng trôi tuột xuống ống thoát nước. Tác giả đề xuất lắp đặt một cuộn ống trao đổi nhiệt bằng đồng bọc quanh ống thoát nước thải, dùng lượng nhiệt dư này để làm ấm sơ bộ luồng nước lạnh ngõ vào nhà trước khi đưa vào bình đun. Dù ý tưởng mang tính sáng tạo về mặt vật lý, việc thi công thực tế gặp nhiều rào cản về chi phí lắp đặt và bảo trì đường ống thoát nước.

3、[Thiết kế hồ nước nhân tạo giúp du khách chụp ảnh động vật hoang dã cận cảnh](https://mymodernmet.com/shompole-hide-will-burrard-lucas/)

Một nhiếp ảnh gia động vật hoang dã người Anh khi tác nghiệp tại Kenya nhận thấy ban ngày thời tiết quá nắng nóng khiến thú rừng ẩn nấp kỹ, chỉ tập trung đi uống nước vào ban đêm. Anh đã phối hợp cùng người dân bản địa xây dựng một hồ nước nhân tạo đặc biệt:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110813.webp)

Hồ nước sử dụng hệ thống bơm chạy bằng năng lượng mặt trời để lấy nước ngầm từ khoảng cách 3 km, bảo đảm nguồn nước luôn dồi dào. Ngay bên cạnh hồ, anh cho xây dựng một căn hầm bê tông kiên cố ngụy trang dưới lòng đất có khe kính quan sát:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110814.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110815.webp)

Giải pháp giúp nhiếp ảnh gia và du khách có thể ngồi an toàn bên trong hầm chụp được những bức ảnh tuyệt đẹp ở cự ly cực gần của các loài thú lớn như sư tử, báo, voi rừng đến uống nước ban đêm, tạo thêm nguồn thu nhập dịch vụ bền vững cho người dân địa phương.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110816.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110817.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110818.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111101.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110820.webp)

4、[Xác nhận sự tồn tại của cả 5 loại bazơ nitơ cấu thành sự sống trên mẫu thiên thạch](https://www.sciencenews.org/article/all-of-the-bases-in-dna-and-rna-have-now-been-found-in-meteorites)

Các nhà khoa học Mỹ công bố kết quả phân tích mẫu thiên thạch Murchison rơi xuống Australia vào năm 1969, xác nhận đã tìm thấy đầy đủ cả 5 loại bazơ nitơ hình thành nên chuỗi xoắn kép DNA và RNA:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110801.webp)

Năm khối cơ bản của sự sống bao gồm: Adenine (A), Guanine (G), Cytosine (C), Thymine (T) và Uracil (U). Thành tựu phân tích này củng cố thêm độ tin cậy cho giả thuyết khoa học cho rằng các hợp chất hữu cơ tiền đề của sự sống trên Trái Đất nguyên thủy vốn được mang tới từ các vụ va chạm thiên thạch ngoài không gian.

## 文章

1\. [Tài liệu hồi ký của em gái nhà toán học Trương Ích Đường về gia đình](https://mp.weixin.qq.com/s/oEMUWTmUZNYRU8hYFNih6A)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110822.webp)

Bài viết hồi ký đầy cảm xúc của bà Trương Doanh Đường chia sẻ về chặng đường học tập gian nan và cuộc sống cô độc nơi xứ người của anh trai mình - nhà toán học lỗi lạc Trương Ích Đường (Zhang Yitang) tại Mỹ trước khi công bố công trình chứng minh toán học chấn động về thuyết số nguyên tố sinh đôi năm 2013.

2\. [Bản tiếng Trung tóm tắt nội dung cuộc phỏng vấn mới nhất của Elon Musk](https://finance.sina.com.cn/tech/it/2022-11-09/doc-imqmmthc3912903.shtml)（Tiếng Trung）

Tổng hợp các chia sẻ của tỷ phú Elon Musk về tiến trình cải tổ cấu trúc nhân sự tại Twitter, các mục tiêu tích hợp thanh toán số và định hướng phát triển công nghệ tự lái của hãng xe điện Tesla thời gian tới.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110908.webp)

3\. [Khám phá quy trình vận hành tòa nhà nuôi heo công nghiệp cao 26 tầng tại Hồ Bắc](https://www.jiemian.com/article/8327167.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110804.webp)

Tìm hiểu thiết kế xây dựng và quy trình xử lý chất thải, cấp thức ăn tự động của khu tổ hợp chuồng nuôi heo dạng nhà cao tầng hiện đại quy mô 26 tầng khép kín tại thành phố Ngạc Châu, tỉnh Hồ Bắc. (Đọc thêm [bài viết chi tiết bổ sung](http://hb.sina.com.cn/news/j/2022-10-21/detail-imqmmthc1616038.shtml)).

4\. [Hành trình tự nghiên cứu và phục chế mô hình thuyền buồm gỗ cổ đại](https://mp.weixin.qq.com/s/6kOdAljOqSe1dQP73c4TBQ)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022103008.webp)

Tác giả chia sẻ chi tiết hành trình sưu tầm tư liệu cổ và tìm kiếm những nghệ nhân mộc lão luyện còn sót lại để phục dựng nguyên bản một chiếc thuyền buồm gỗ đi biển truyền thống Trung Hoa cổ đại vốn đã bị thất truyền kỹ thuật chế tác từ lâu.

5\. [Phương pháp thiết lập cache cho các yêu cầu CORS HTTP Requests](https://httptoolkit.tech/blog/cache-your-cors/)（Tiếng Anh）

Yêu cầu跨 miền CORS thường buộc trình duyệt phát đi đồng thời hai truy vấn (Preflight request + Actual request) lên server. Bài viết hướng dẫn lập trình viên Front-end cách thiết lập header phản hồi thích hợp để cache các yêu cầu này ở trình duyệt client nhằm giảm lượng tải và tiết kiệm chi phí băng thông máy chủ cloud.

6\. [Quy trình phát triển tính năng tốc độ cao dành cho các nhà sáng lập startup](https://growing-products.paralect.com/a-development-process-startup-founders-should-use-to-ship-features-weirdly-fast)（Tiếng Anh）

Tác giả chia sẻ các kinh nghiệm quản trị dự án phần mềm và tổ chức luồng code tinh gọn giúp các đội ngũ lập trình nhỏ của startup có thể kiểm thử và phát hành tính năng mới ra thị trường với tốc độ nhanh chóng.

7\. [Đánh giá chi tiết thiết bị phần cứng máy chủ ARM Windows Dev Kit 2023](https://www.jeffgeerling.com/blog/2022/testing-microsofts-windows-dev-kit-2023)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110511.webp)

Đánh giá chi tiết về cấu hình phần cứng, hiệu năng đo đạc thực tế của mẫu máy tính nhỏ chạy chip ARM do Microsoft phát hành với mức giá 599 USD nhằm hỗ trợ các lập trình viên biên dịch và kiểm thử phần mềm tối ưu cho hệ điều hành Windows trên nền tảng chip ARM. (Xem thêm [bản đánh giá tiếng Trung](https://zhuanlan.zhihu.com/p/580147966)).

8\. [Phương pháp trừng phạt spammers bằng công cụ Cloudflare Workers và Power Automate](https://www.troyhunt.com/sending-spammers-to-password-purgatory-with-microsoft-power-automate-and-cloudflare-workers-kv/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080404.webp)

Chuyên gia bảo mật Troy Hunt chia sẻ một trò đùa kỹ thuật thú vị: anh thiết lập một luồng xử lý tự động sử dụng Cloudflare Workers để chuyển hướng các email gửi thư rác đến một trang đăng ký giả lập, trang này yêu cầu người gửi thiết lập mật khẩu bảo mật rất ngặt nghèo nhưng thực chất được lập trình để liên tục báo lỗi thất bại nhằm làm mất thời gian của spammers.

## 工具

1、[Upscayl: Ứng dụng trí tuệ nhân tạo nguồn mở hỗ trợ làm sắc nét hình ảnh](https://github.com/upscayl/upscayl)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082909.webp)

Phần mềm máy tính nguồn mở sử dụng mô hình AI hỗ trợ phóng to độ phân giải hình ảnh chất lượng thấp thành ảnh độ nét cao mà không làm nhòe thớ ảnh.

2、[CodeGeeX: Mô hình trí tuệ nhân tạo hỗ trợ sinh mã nguồn tự động của Trung Quốc](https://keg.cs.tsinghua.edu.cn/codegeex/index_zh.html)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111006.webp)

Công cụ hỗ trợ viết code tự động tương tự GitHub Copilot do các viện nghiên cứu Trung Quốc phát triển, hỗ trợ dịch chuyển mã nguồn qua lại giữa các ngôn ngữ lập trình khác nhau, cung cấp extension tương thích tốt trên VS Code. (Đóng góp của [@jues](https://github.com/ruanyf/weekly/issues/2717))

3、[Lama Cleaner: Tiện ích web hỗ trợ xóa bỏ nhanh các vật thể thừa khỏi bức ảnh](https://github.com/Sanster/lama-cleaner)

Công cụ AI nguồn mở chạy trực tiếp trên web cho phép người dùng bôi chọn và xóa bỏ lập tức các chi tiết thừa, chữ chèn hoặc người trong ảnh một cách tự nhiên. (Đóng góp của [@willshion](https://github.com/ruanyf/weekly/issues/2721))

4、[vtui-npm: Tiện ích dòng lệnh CLI tìm kiếm và cài đặt module npm tương tác](https://github.com/webfansplz/vtui-npm)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111009.webp)

Công cụ CLI hỗ trợ lập trình viên JavaScript tìm kiếm trực quan và cài đặt nhanh các package npm trực tiếp trên màn hình Terminal. (Đóng góp của [@webfansplz](https://github.com/ruanyf/weekly/issues/2731))

5、[watching-you: Thư viện JavaScript tạo hiệu ứng nhân vật hướng mắt theo trỏ chuột](https://github.com/jj811208/watching-you)

Thư viện tạo hiệu ứng CSS/JS tương tác vui nhộn cho website: các hình ảnh nhân vật đồ họa trên trang sẽ tự động xoay hướng mắt dõi theo tọa độ di chuyển của con trỏ chuột của người dùng. (Đóng góp của [@jj811208](https://github.com/ruanyf/weekly/issues/2729))

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111010.webp)

6、[Sonic: Nền tảng quản lý trang blog cá nhân viết bằng Go gọn nhẹ](https://github.com/go-sonic/sonic/blob/master/doc/README_ZH.md)

Mã nguồn mở xây dựng trang blog cá nhân viết bằng Go hỗ trợ đầy đủ trang Dashboard quản trị nội dung, tiêu thụ tài nguyên hệ thống cực nhỏ và dễ dàng deploy. (Đóng góp của [@1379](https://github.com/ruanyf/weekly/issues/2736))

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111011.webp)

7、[Netease Recent Profile: Tiện ích kết xuất danh sách nghe nhạc thành ảnh SVG](https://github.com/zonemeen/netease-recent-profile)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111012.webp)

Công cụ hỗ trợ tự động đồng bộ lịch sử nghe nhạc trên NetEase Cloud Music thành một tệp hình ảnh SVG động để người dùng nhúng trang trí vào trang profile cá nhân trên GitHub. (Đóng góp của [@zonemeen](https://github.com/ruanyf/weekly/issues/2735))

8、[Bun: Môi trường thực thi JavaScript thế hệ mới tốc độ cao](https://bun.sh/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070604.webp)

Bộ công cụ biên dịch và runtime JS/TS viết bằng Zig từ đầu nhằm tương thích và thay thế Node.js, cung cấp tốc độ cài đặt package và thực thi mã nguồn vượt trội hơn hẳn Node.js hay Deno.

9、[IPFS Cloud: Cổng lưu trữ dữ liệu miễn phí lên mạng phi tập trung IPFS](https://ipfs-gateway.cloud/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070701.webp)

Dịch vụ web hỗ trợ người dùng tải tệp tin nhanh chóng lên giao thức lưu trữ phân tán IPFS. Các tệp tin sau khi được tải lên sẽ được cấp địa chỉ hash duy nhất để truy cập vĩnh viễn không thể sửa đổi hay xóa bỏ.

10、[LocalStack: Môi trường giả lập ngoại tuyến các dịch vụ đám mây AWS](https://github.com/localstack/localstack)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070706.webp)

Dự án nguồn mở hữu ích cho phép lập trình viên chạy giả lập toàn bộ các dịch vụ cloud của Amazon (S3, Lambda, DynamoDB) cục bộ trên máy tính cá nhân để phục vụ công tác viết code test ngoại tuyến (offline).

## 资源

1、[Postgres Playground: Môi trường thực hành cơ sở dữ liệu PostgreSQL trực tuyến](https://www.crunchydata.com/developers/tutorials)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081802.webp)

Trang web học tập SQL tương tác trực quan: hệ thống tạo nhanh một database PostgreSQL ảo trực tiếp trên trình duyệt để người dùng gõ câu lệnh SQL thực hành theo giáo trình đi kèm. (Xem thêm [bài viết giới thiệu](https://www.crunchydata.com/blog/learn-postgres-at-the-playground)).

2、[IconGo: Công cụ tìm kiếm thư viện icon đồ họa nguồn mở phong phú](https://icongo.github.io/)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111007.webp)

Trang web tổng hợp và hỗ trợ nhà phát triển Front-end tìm kiếm, copy nhanh mã SVG của hàng ngàn biểu tượng icon thiết kế từ các bộ nguồn mở nổi tiếng. (Đóng góp của [@jaywcjlove](https://github.com/ruanyf/weekly/issues/2724))

3、[SadServers: Bộ bài tập thực hành gỡ lỗi sự cố máy chủ Linux thực tế](https://sadservers.com/)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111008.webp)

Trang web học tập quản trị hệ thống Linux thú vị: hệ thống khởi tạo một máy ảo Linux chứa sẵn một số lỗi cấu hình cụ thể, yêu cầu người dùng phải gõ lệnh Terminal trực tuyến để tự debug giải bài tập. (Đóng góp của [@jerrylususu](https://github.com/ruanyf/weekly/issues/2726))

4、[Full Stack Python: Giáo trình hướng dẫn phát triển phần mềm bằng Python](https://www.fullstackpython.com/)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061606.webp)

Sách hướng dẫn tiếng Anh miễn phí chất lượng cao dành cho người đã nắm vững cú pháp Python cơ bản muốn học cách triển khai dự án thực tế: thiết lập web server, kết nối DB, cấu hình bảo mật và deploy.

5、[Unicode Confusables: Công cụ đối chiếu các ký tự Unicode dễ gây nhầm lẫn](https://util.unicode.org/UnicodeJsps/confusables.jsp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082102.webp)

Do nhiều ký tự trong bảng mã Unicode ở các ngôn ngữ khác nhau có hình dáng thiết kế giống hệt nhau (như ký tự `c` trong các bảng chữ cái khác nhau), công cụ này giúp các chuyên gia bảo mật tra cứu các ký tự tương đồng để phòng chống lỗ hổng giả mạo tên miền quốc tế (IDN homograph attack).

## 图片和视频

1、[Dự án tự chế thấu kính hội tụ năng lượng mặt trời phục vụ luyện kim sạch](https://jelleseegers.com/)

Một kỹ sư đã tự chế tạo một khung thấu kính hội tụ ánh sáng mặt trời cực lớn nhằm nung chảy kim loại trong nồi đất nung trực quan mà không cần dùng than hay điện, nhằm hướng tới giải pháp luyện kim xanh không phát thải carbon:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102704.webp)

2、[Khám phá kiến trúc độc đáo của tòa nhà trụ sở "Sky City" của hãng DJI](https://dji-skycity)

Vào tháng 9 vừa qua, DJI đã chính thức khánh thành tổ hợp tòa nhà văn phòng trụ sở mới mang tên "Sky City" (Thành phố trên trời) tại quận Nam Sơn, Thâm Quyến:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110505.webp)

Công trình do văn phòng kiến trúc danh tiếng Foster + Partners thiết kế với tổng kinh phí xây dựng hơn 1,6 tỷ Nhân dân tệ. Điểm nhấn kiến trúc là cấu trúc tháp đôi được kết nối bằng cầu treo dây văng thép, mỗi tòa tháp thiết kế các khối kính lớn nhô ra lơ lửng giữa không trung:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110503.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110502.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110504.webp)

Độc giả có thể theo dõi [Video cận cảnh nội thất bên trong tòa nhà](https://v.qq.com/x/page/g3362le7ktg.html) (hoặc xem bản [Youtube](https://www.youtube.com/watch?v=RGsa_bpkVpU)).

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=g3362le7ktg" allowFullScreen="true" width="600" height="400"></iframe>

3、[Bộ sưu tập các bức poster văn hóa doanh nghiệp cũ tại văn phòng Facebook](https://bytepawn.com/culture-docs-facebook-netflix-and-valve.html)

Một số thông điệp thiết kế tối giản, đầy sức sống dán trên tường văn phòng làm việc cũ của Facebook:

* *"Bạn sẽ hành động như thế nào nếu bản thân không còn cảm thấy sợ hãi?"*

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062108.webp)

* *"Thử nghiệm và thất bại một cách mạnh mẽ hơn nữa."*

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062109.webp)

* *"Ý kiến phản hồi từ người dùng chính là món quà quý giá nhất."*

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102703.webp)

## ✍️ Bài đọc thêm

### Tại sao các kỹ sư dữ liệu của Google không quá chú trọng việc tối ưu hóa câu lệnh SQL?

Tôi từng làm việc với tư cách là đối tác cung cấp dịch vụ bên ngoài của Google. Trong quá trình cộng tác, tôi nhận thấy một thực tế khá lạ lùng: Nhiều kỹ sư dữ liệu của Google viết các câu lệnh truy vấn SQL với cấu trúc rất cồng kềnh và kém hiệu quả về mặt tài nguyên hệ thống.

Các câu lệnh này định kỳ 10 phút lại quét toàn bộ và chụp ảnh lưu lại (snapshot) bảng dữ liệu khổng lồ, tiêu tốn hàng TB không gian đệm lưu trữ. Tại sao một công ty công nghệ hàng đầu thế giới lại không tối ưu hóa các dòng code này để tiết kiệm chi phí?

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111013.webp)

Sau này, tôi đã hiểu ra nguyên nhân sâu xa đằng sau:

1. **Sự phát triển của bộ tối ưu hóa tự động (Optimizer)**: Các hệ quản trị cơ sở dữ liệu lớn hiện đại (như Google BigQuery) được tích hợp sẵn các thuật toán tự động phân tích và tối ưu hóa đường đi của câu lệnh SQL ở tầng dưới, giúp giảm đáng kể vai trò tối ưu hóa thủ công của con người.
2. **Bài toán chi phí nhân sự (Cost/Benefit)**: Theo thống kê lương, mức thu nhập trung bình của một kỹ sư dữ liệu lớn tại Mỹ dao động quanh mốc 112.500 USD/năm (lương tại Google còn cao hơn). Trong khi đó, chi phí lưu trữ đám mây hiện nay đã cực kỳ rẻ (chỉ khoảng 20 USD/năm cho 1TB dữ liệu lưu trữ trên Google Cloud Platform - GCP).
3. **Phép tính toán kinh tế cụ thể**: Lương trung bình theo giờ của kỹ sư dữ liệu khoảng 54 USD. Nếu yêu cầu kỹ sư dành 8 giờ làm việc (tương đương 1 ngày lương khoảng 432 USD) để tối ưu hóa một câu lệnh SQL, viết các pipeline gom dữ liệu phức tạp, gửi code review và theo dõi bảo trì lâu dài... chi phí nhân công bỏ ra này tương đương với chi phí lưu trữ tệp dữ liệu không tối ưu đó trong suốt **21 năm**.

Vì chi phí phần cứng và lưu trữ ngày càng tiệm cận mốc 0, thời gian làm việc của kỹ sư được định hướng tập trung hoàn toàn vào việc phát triển nhanh các tính năng mang lại giá trị trực tiếp cho hoạt động kinh doanh của doanh nghiệp, thay vì lãng phí tài nguyên chất xám đi tinh chỉnh các chi tiết tối ưu hóa nhỏ nhặt vốn có thể dễ dàng giải quyết bằng hạ tầng.

## 历史上的本周

- 2021年（第 182 期）：[Thảo luận kinh doanh: Những rủi ro tiềm ẩn đối với doanh nghiệp khi triển khai các chương trình khuyến mãi ưu đãi cực lớn cho khách hàng mới](https://www.ruanyifeng.com/blog/2021/11/weekly-issue-182.html)
- 2020年（第 132 期）：[Định hướng bản thân: Phân tích sự bổ trợ giữa năng lực hành động nhanh nhạy và năng lực tư duy chiều sâu](https://www.ruanyifeng.com/blog/2020/11/weekly-issue-132.html)
- 2019年（第 80 期）：[Kinh doanh phần mềm: Tại sao thị trường phát triển phần mềm quản trị doanh nghiệp (SaaS) lại gặp nhiều khó khăn tại thị trường trong nước](https://www.ruanyifeng.com/blog/2019/11/weekly-issue-80.html)
- 2018年（第 29 期）：[Kiến trúc hệ thống: Định luật Conway - Cách thức tổ chức bộ máy nhân sự quyết định độ phức tạp của mã nguồn phần mềm](https://www.ruanyifeng.com/blog/2018/11/weekly-issue-29.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2715) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## 鸣谢

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072108.webp)

（Hết）
