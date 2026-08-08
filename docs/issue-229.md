# 科技爱好者周刊（第 229 期）：手机充电问题的解决

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần。

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn。

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2715) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập。

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110203.webp)

Mới đây, "Thiết bị bay mô phỏng chim vỗ cánh khớp kép cỡ lớn" do Đại học Hàng không Vũ trụ Bắc Kinh nghiên cứu phát triển đã thiết lập kỷ lục Guinness thế giới mới về thời gian bay liên tục của thiết bị bay cơ học vỗ cánh, đạt thành tích 1 giờ 31 phút 04 giây 98. (Nguồn: [Huanqiu](https://uav.huanqiu.com/article/4ADEZRT9pu6))

## 本周话题：手机充电问题的解决

Mỗi ngày, bạn phải dành bao nhiêu thời gian để sạc pin cho chiếc điện thoại di động của mình? Liệu việc phải chờ đợi pin sạc đầy có khiến bạn cảm thấy phiền toái?

Tuy nhiên, bài toán sạc pin dường như đã được giải quyết triệt để bởi những cải tiến công nghệ gần đây.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102911.webp)

Xiaomi vừa qua đã chính thức [công bố sản phẩm](https://m.21jingji.com/article/20221027/herald/c4b4fa8fa8962a50fa416fccf43dacaf.html) điện thoại thông minh Redmi Note 12 Explorer Edition.

Điểm nhấn công nghệ ấn tượng nhất của thiết bị này là việc trang bị công nghệ sạc nhanh thương mại nhanh nhất thế giới hiện nay, cho phép sạc đầy 100% viên pin dung lượng 4300mAh từ mức 0% chỉ trong vòng vỏn vẹn **9 phút**.

Bạn không hề đọc nhầm, thực sự chỉ mất 9 phút – tương đương thời gian uống một tách trà – để nạp đầy năng lượng cho thiết bị.

Với tốc độ này, thói quen sạc pin sẽ thay đổi hoàn toàn. Bạn chỉ cần cắm sạc tranh thủ lúc thức dậy vệ sinh cá nhân vào buổi sáng là thiết bị đã đủ dung lượng pin để sử dụng thoải mái cho đến khi trở về nhà vào tối muộn.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102906.webp)

Bí quyết giúp thiết bị đạt tốc độ sạc ấn tượng này nằm ở củ sạc đi kèm có công suất cực khủng lên tới **210W**.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102905.webp)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102908.webp)

Đây thực sự là một bước nhảy vọt công nghệ đáng kinh ngạc. Tôi nhớ cách đây không lâu, công suất sạc của các hãng mới chỉ vượt mốc 100W, mà nay đã nhanh chóng chạm ngưỡng 210W.

Để hiểu tại sao mức công suất này lại giải quyết được bài toán sạc pin, chúng ta có thể thực hiện một phép tính vật lý đơn giản:

Tốc độ sạc pin phụ thuộc cốt lõi vào thông số điện áp (Voltage) và cường độ dòng điện (Current) ngõ ra tối đa của bộ sạc.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102909.webp)

Các thông số này luôn được in ở mặt sau của củ sạc. Với bộ sạc 210W của Xiaomi, thông số ngõ ra tối đa đạt mức 20V / 10.5A. Phép nhân hai giá trị này (20V * 10.5A) cho ra mức công suất tối đa tương ứng là 210W.

Để so sánh, các bộ sạc thường cũ chỉ có thông số 5V/2A (10W) hoặc thậm chí 5V/1A (5W).

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110101.webp)

Tiếp theo, hãy xem xét dung lượng pin của máy là 4300mAh. Thông số này nghĩa là viên pin có khả năng cung cấp dòng điện liên tục 4300mA trong vòng 1 giờ đồng hồ.

Với điện áp định danh chuẩn của các cell pin Lithium hiện nay là 3.7V, tổng năng lượng dự trữ của viên pin sẽ là:

> 4300mAh * 3.7V = 15910mWh = 15.91 Wh

Từ đó, thời gian sạc đầy viên pin về mặt lý thuyết với công suất sạc 210W sẽ là:

> 15.91 Wh / 210 W = 0.076 giờ ≈ 4 phút 33 giây

Trong điều kiện sạc thực tế, do có hao hụt năng lượng tỏa nhiệt và cơ chế sạc nhỏ giọt (trickle charge) tự động giảm dòng để bảo vệ tuổi thọ cell pin ở giai đoạn cuối, tổng thời gian sạc thực tế kéo dài lên mức 9 phút là hoàn toàn chính xác và đáng tin cậy.

Trong khi đó, nếu sử dụng củ sạc 5V/2A (10W) truyền thống, thời gian sạc lý thuyết cho viên pin này phải mất tới gần 1.6 giờ:

> 15.91 Wh / 10 W = 1.591 giờ

Sự nâng cấp công suất sạc lên mức 210W đã rút ngắn thời gian sạc từ hàng tiếng đồng hồ xuống chỉ còn vài phút ngắn ngủi.

Nhiều người sẽ tự hỏi liệu trong tương lai công suất sạc có thể tiếp tục nâng cao hơn nữa để rút ngắn thời gian sạc xuống vài giây?

Câu trả lời là rất khó. Mức công suất hơn 200W gần như đã chạm ngưỡng giới hạn an toàn kỹ thuật đối với mạng điện dân dụng thông thường. Quy định an toàn điện gia đình yêu cầu điện áp tiếp xúc trực tiếp không được vượt quá 24V để phòng tránh giật điện nguy hiểm cho con người. Đồng thời, tiêu chuẩn thiết bị điện gia dụng công suất nhỏ giới hạn cường độ dòng điện ngõ vào dưới mức 10A. Phép nhân hai giới hạn này (24V * 10A) cho thấy ngưỡng công suất sạc an toàn tối đa cho thiết bị gia đình chỉ xoay quanh mức hơn 200W.

## 抖音 iOS 客户端开发技术分享会

Ứng dụng Douyin (phiên bản TikTok nội địa Trung Quốc) chạy trên nền tảng iOS hiện là một trong những ứng dụng di động có lượng người dùng thường xuyên lớn nhất.

Mặc dù quy mô hệ thống cực kỳ đồ sộ, lịch sử phát triển của Douyin lại rất ngắn khi phiên bản đầu tiên chỉ mới được phát hành vào tháng 9 năm 2016.

Sự tăng trưởng thần tốc của lượng người dùng đặt ra những thách thức công nghệ khổng lồ cho đội ngũ kỹ sư iOS của hãng trong việc bảo đảm chất lượng mã nguồn và vận hành các tính năng phức tạp như livestream, thuật toán gợi ý dữ liệu thời gian thực...

Vào chiều thứ Bảy tuần tới (ngày 12 tháng 11), **đội ngũ kỹ thuật iOS của Douyin sẽ tổ chức một buổi hội thảo chia sẻ công nghệ trực tuyến miễn phí** chia sẻ về các giải pháp kỹ thuật thực tế của họ:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022103010.webp)

Chương trình hội thảo gồm 5 bài thuyết trình chuyên sâu do các kỹ sư trưởng trực tiếp trình bày:

1. **Phát hiện lỗi sớm**: Cách thức ứng dụng phân tích mã nguồn tĩnh (Static Analysis) để kiểm soát chất lượng code Swift/Objective-C của dự án.
2. **Quy trình DevOps**: Giải pháp kiểm thử tự động và thiết lập hệ thống tích hợp liên tục (CI/CD) quy mô lớn của Douyin iOS App.
3. **Tối ưu hóa đa phương tiện**: Các giải pháp kỹ thuật tối ưu hóa luồng tải và chất lượng hiển thị video mượt mà trên iOS.
4. **Tái cấu trúc luồng nạp Feed**: Kinh nghiệm thực tế tái cấu trúc mã nguồn dòng cấp dữ liệu video (video feed) trang chủ.
5. **Trí tuệ nhân tạo trên thiết bị**: Cách thức vận hành các mô hình học máy (Machine Learning) chạy trực tiếp trên thiết bị iOS (On-device ML).

Tôi đặc biệt quan tâm tới bài chia sẻ thứ 4 về tái cấu trúc luồng nạp video Feed trang chủ. Đây là tính năng cốt lõi quyết định video nào được hiển thị ưu tiên cho người dùng, đồng thời cũng là luồng xử lý phức tạp nhất. Theo chia sẻ của kỹ sư, tính đến đầu năm 2020, riêng mã nguồn quản lý luồng dữ liệu Feed đã vượt mốc 300.000 dòng code với nhiều tệp tin chứa hơn 10.000 dòng lệnh phức tạp.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022103011.webp)

Buổi chia sẻ do cộng đồng công nghệ ByteTech của ByteDance bảo trợ tổ chức, đi kèm các phiên thảo luận hỏi đáp trực tiếp (Q&A) với các lập trình viên bên ngoài.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022103012.webp)

Hội thảo diễn ra dưới hình thức livestream trực tuyến miễn phí. Độc giả quan tâm có thể click vào [Đường dẫn đăng ký tham gia hội thảo](https://www.bagevent.com/event/8325585?bag_track=001) hoặc quét mã QR trong hình để đặt chỗ trước.

## 科技动态

1、[Thiết bị công nghệ hỗ trợ radar nhìn xuyên qua tường](https://www.businessinsider.com/new-israeli-military-technology-allows-operators-to-see-through-walls-2022-6)

Một doanh nghiệp quốc phòng của Israel giới thiệu thiết bị chuyên dụng cầm tay cho phép người vận hành quan sát được các mục tiêu chuyển động phía sau bức tường gạch:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062701.webp)

Thiết bị ứng dụng sóng radar vi sóng có khả năng xuyên qua các lớp vật liệu xây dựng dày, sau đó thu nhận các sóng phản xạ từ chuyển động vật thể để dựng lại hình ảnh 3D thời gian thực:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062702.webp)

Hệ thống hỗ trợ đắc lực cho lực lượng đặc nhiệm hoặc cứu hộ xác định nhanh số lượng người trong phòng kín, tư thế đứng/ngồi/nằm và bố cục không gian bên trong ngôi nhà bị sập đổ để lên phương án tiếp cận.

2、[Adobe Photoshop chính thức loại bỏ thư viện màu chuẩn Pantone](https://kotaku.com/photoshop-pantone-color-plugin-adobe-creative-cloud-1849714742)

Công ty Pantone của Mỹ nổi tiếng với việc sáng chế ra hệ thống so khớp màu sắc tiêu chuẩn Pantone Matching System (PMS) giúp đồng bộ hóa hiển thị màu sắc chính xác trên mọi chất liệu và thiết bị in ấn khác nhau. Hệ màu này được bảo hộ bản quyền thương mại rất nghiêm ngặt.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102902.webp)

Trước đây, Adobe trả phí bản quyền cho Pantone để tích hợp sẵn bảng màu này trong Photoshop. Do bất đồng về chi phí nhượng quyền, hai bên đã ngừng hợp tác và Adobe đã chính thức gỡ bỏ thư viện màu Pantone khỏi bản cập nhật Photoshop tháng này:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102903.webp)

Sự thay đổi này khiến toàn bộ các vùng màu Pantone trên các tệp thiết kế cũ (.psd) của người dùng tự động chuyển thành màu đen. Để khôi phục hiển thị màu sắc, thiết kế viên buộc phải mua thêm gói plugin dịch vụ bổ sung trực tiếp từ Pantone với giá 15 USD/tháng. Việc này gây ra làn sóng phản đối lớn trong giới thiết kế đồ họa toàn cầu khi lần đầu tiên họ nhận thức được việc phải trả tiền thuê bao tháng để được sử dụng màu sắc.

3、[Sự việc in mã nguồn ra giấy A4 gây xôn xao tại văn phòng Twitter](https://twitter.com/goldman/status/1586128703259521024)

Vào ngày đầu tiên tiếp quản mạng xã hội Twitter, tỷ phú Elon Musk đã bất ngờ gửi thông báo yêu cầu toàn bộ các kỹ sư phần mềm của hãng phải tiến hành in toàn bộ các đoạn mã nguồn do họ tự viết trong vòng 30 đến 60 ngày gần nhất ra giấy A4 để chuẩn bị duyệt trực tiếp.

Yêu cầu đột ngột này khiến hệ thống máy in tại văn phòng Twitter hoạt động quá tải và nhanh chóng rơi vào tình trạng hết sạch giấy in A4.

Một kỹ sư iOS của Twitter đã đăng tải hình ảnh chồng mã nguồn in giấy dày cộp của mình lên mạng xã hội:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102904.webp)

Tuy nhiên đến buổi trưa cùng ngày, ban quản lý mới lại gửi thông báo yêu cầu dừng ngay việc in ấn, đồng thời yêu cầu các kỹ sư phải bỏ toàn bộ số mã nguồn giấy đã in vào máy hủy tài liệu để bảo mật thông tin và chuyển sang chuẩn bị mã nguồn trực tiếp trên máy tính cá nhân.

4、[DPreview đề xuất thay đổi cách ghi kích thước cảm biến ảnh điện thoại](https://www.dpreview.com/articles/4159871805/making-sensor-sizes-less-misleading)

Trang tin nhiếp ảnh uy tín DPreview đề xuất các hãng công nghệ nên từ bỏ cách ghi kích thước cảm biến camera điện thoại bằng đơn vị inch phân số truyền thống vì nó dễ gây hiểu nhầm cho khách hàng:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022073102.webp)

Ví dụ cảm biến của iPhone 13 Pro Max ghi là 1/1.65 inch còn cảm biến của Xiaomi 12 Ultra ghi là 1 inch. Khách hàng thông thường khó hình dung được sự chênh lệch thực tế giữa hai con số này:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022073103.webp)

Thực tế diện tích cảm biến của iPhone chỉ là 44 mm², còn cảm biến 1 inch của Xiaomi có diện tích thực tế lên tới 128 mm² (lớn gấp gần 3 lần). DPreview đề xuất các hãng nên ghi trực tiếp thông số diện tích cảm biến bằng đơn vị mm² để đảm bảo tính minh bạch.

5、[Triển lãm văn cụ bút mực quốc tế Tokyo thu hút đông đảo giới trẻ](https://tokyo-international-penshow.com/)

Triển lãm bút mực quốc tế Tokyo thường niên vừa khai mạc đã ghi nhận lượng vé tham quan bán hết sạch từ sớm với tỷ lệ người tham gia đa số là các bạn trẻ:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110311.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110312.webp)

Sự kiện quy tụ hàng trăm gian hàng trưng bày các mẫu bút máy, các loại giấy viết tay mỹ thuật và các dòng mực viết thư pháp đa màu sắc:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110313.webp)

Trong thời đại số hóa hiện nay, dù giá trị sử dụng thực tế của các loại văn phòng phẩm truyền thống đang giảm dần, chúng lại đang chuyển dịch mạnh mẽ thành những món đồ sưu tầm nghệ thuật có giá trị tinh thần cao.

## 文章

1\. [Khám phá phần cứng máy chủ lưu trữ video 262TB thanh lý của Netflix](https://www.chiphell.com/forum.php?mod=viewthread&tid=2454839&extra=page%3D1&mobile=2)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022103009.webp)

Một thành viên diễn đàn công nghệ chia sẻ trải nghiệm thực tế khi mua lại một thiết bị máy chủ lưu trữ đệm video (cache server) đời 2013 do Netflix thanh lý. Thiết bị có dung lượng lưu trữ lên tới 262TB dùng làm trạm CDN phân phối video cục bộ của hãng.

2\. [Thăm phòng thí nghiệm vật lý đặt sâu nhất thế giới tại Tứ Xuyên](http://sc.sina.com.cn/news/m/2022-10-10/detail-imqqsmrp1980816.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022103001.webp)

Giới thiệu về phòng thí nghiệm lòng đất sâu 2.400m nằm sâu dưới lòng núi Đại Lương thuộc tỉnh Tứ Xuyên. Đây là cơ sở nghiên cứu khoa học sâu nhất hành tinh chuyên phục vụ công tác đo đạc và tìm kiếm sự tồn tại của vật chất tối (dark matter) trong vũ trụ nhờ lớp đất đá dày giúp ngăn nhiễu tia vũ trụ.

3\. [Sự cố xung đột tần số micro không dây của Sony với mạng di động 5G](https://finance.sina.cn/tech/2022-10-26/detail-imqmmthc2126430.d.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102710.webp)

Phân tích nguyên nhân hàng loạt thiết bị micro ghi âm không dây cao cấp của Sony sử dụng băng tần vô tuyến 700MHz gặp hiện tượng mất sóng và rè tiếng ngắt quãng khi sử dụng tại Trung Quốc do trùng với băng tần phát sóng của mạng viễn thông di động 5G quốc gia.

4\. [Tìm hiểu lịch sử phân loại kích thước các dòng pin khô gia dụng](https://finance.sina.com.cn/wm/2022-10-24/doc-imqqsmrp3595606.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102709.webp)

Bài viết khoa học thường thức giới thiệu về lịch sử ra đời và các tiêu chuẩn phân loại kích thước, dung lượng điện áp của các dòng pin khô gia dụng thông dụng hiện nay (như pin tiểu AA - pin số 5, pin đũa AAA - pin số 7).

5\. [Hướng dẫn tùy biến thuộc tính CSS cho thẻ `<details>` trong HTML](https://css-tricks.com/two-issues-styling-the-details-element-and-how-to-solve-them/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090516.webp)

Thẻ `<details>` trong HTML hỗ trợ tạo các khung hiển thị nội dung dạng gập mở tiện lợi không cần dùng JS. Bài viết hướng dẫn chi tiết cách thiết lập CSS để thay đổi biểu tượng mũi tên chỉ hướng mặc định và xử lý lỗi giật khung hình khi mở rộng.

6\. [Tận dụng thuộc tính `capture` của thẻ `<input>` để gọi nhanh camera điện thoại](https://austingil.com/html-capture-attribute/)（Tiếng Anh）

Hướng dẫn lập trình web tận dụng thuộc tính `capture` của thẻ `<input type="file">` trong HTML giúp trình duyệt trên điện thoại di động tự động mở trực tiếp camera hoặc máy ghi âm của thiết bị để thu nhận file mà không cần viết các đoạn mã JavaScript phức tạp.

7\. [Tổng hợp các dịch vụ cloud thay thế miễn phí sau khi Heroku ngừng gói free](https://www.reaktor.com/blog/how-to-deal-with-life-after-heroku/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110310.webp)

Sau khi nền tảng hosting Heroku chính thức chấm dứt chương trình cung cấp máy chủ web và cơ sở dữ liệu miễn phí, tác giả tổng hợp danh sách các dịch vụ cloud thay thế chất lượng tốt (như Render, Fly.io, Supabase) cho lập trình viên.

8\. [Phân tích xu hướng sụt giảm số lượng khe cắm PCIe trên bo mạch chủ mới](https://kerricklong.com/articles/pci-express-slots.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090701.webp)

Bài viết phân tích nguyên nhân tại sao các bo mạch chủ thế hệ mới hiện nay ngày càng cắt giảm số lượng khe cắm mở rộng chuẩn PCIe truyền thống để chuyển sang tích hợp sẵn các cổng cắm ổ cứng M.2 siêu tốc và các cổng kết nối ngoại vi băng thông rộng.

## 工作与开发者工具

1、[SourceHut: Nền tảng hosting mã nguồn uy tín cập nhật điều khoản bảo mật mới](https://sourcehut.org/blog/2022-10-31-tos-update-cryptocurrency/)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022103103.webp)

Dịch vụ lưu trữ mã nguồn độc lập SourceHut công bố cập nhật chính sách dịch vụ quan trọng: (1) Cấm lưu trữ toàn bộ các dự án liên quan đến tiền điện tử và blockchain do lo ngại các hoạt động đầu cơ; (2) Đóng cửa văn phòng đại diện tại Mỹ để tránh nghĩa vụ tuân thủ các sắc lệnh pháp luật đặc thù của Mỹ nhằm bảo vệ quyền riêng tư tuyệt đối cho người dùng quốc tế.

2、[SQLite3 WASM: SQLite chính thức phát hành phiên bản WebAssembly](https://sqlite.org/wasm/doc/ckout/index.md)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110316.webp)

Trang chủ SQLite chính thức công bố bản build WebAssembly hoàn thiện, hỗ trợ đắc lực cho các nhà phát triển web chạy trực tiếp các câu lệnh truy vấn cơ sở dữ liệu SQL ngay trên trình duyệt client mà không cần thông qua kết nối server bên ngoài.

3、[ravynOS: Dự án phát triển hệ điều hành nguồn mở hướng tương thích macOS](https://ravynos.com/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081810.webp)

Do hệ điều hành macOS được xây dựng trên nền tảng nhân Unix tương tự FreeBSD, dự án ravynOS nỗ lực xây dựng một nhánh phân phối FreeBSD nguồn mở có cấu trúc hệ thống và giao diện đồ họa tương đồng và tương thích tốt nhất với các ứng dụng của macOS.

4、[Palette.fm: Ứng dụng trí tuệ nhân tạo hỗ trợ tô màu ảnh đen trắng cổ điển](https://palette.fm/)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102708.webp)

Dịch vụ web cho phép người dùng đăng tải các bức ảnh đen trắng cũ để hệ thống tự động phân tích và tô màu sắc sinh động bằng AI với nhiều phong cách bộ lọc màu sắc khác nhau. (Đọc thêm dự án tương tự mang tên [DeOldify](https://github.com/jantic/DeOldify)).

5、[sttr: Tiện ích dòng lệnh CLI hỗ trợ xử lý chuỗi văn bản đa năng](https://github.com/abhimanyu003/sttr)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081820.webp)

Công cụ CLI đa nền tảng hỗ trợ lập trình viên xử lý nhanh các chuỗi dữ liệu đầu vào như: đếm ký tự, mã hóa/giải mã Base64, tạo mã băm MD5/SHA, lọc trích xuất địa chỉ email hoặc định dạng file JSON.

6、[ntfy: Dịch vụ thông báo pub-sub nguồn mở tự vận hành gọn nhẹ](https://ntfy.sh/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081901.webp)

Giải pháp thiết lập máy chủ notification cá nhân, hỗ trợ gửi tin nhắn đẩy (push notifications) trực tiếp về thiết bị di động hoặc màn hình máy tính thông qua các câu lệnh HTTP POST/PUT đơn giản. (Xem thêm công cụ tương tự [Gotify](https://gotify.net/)).

7、[NeatChart: Tiện ích vẽ biểu đồ dạng cột từ tệp CSV sử dụng Unreal Engine 5](https://neatchart.io/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082001.webp)

Phần mềm đồ họa chạy trên Windows hỗ trợ nhập tệp dữ liệu CSV để kết xuất thành các biểu đồ 3D chuyển động mượt mà nhờ ứng dụng công nghệ đồ họa của Unreal Engine 5.

8、[Crawlee: Thư viện tự động hóa trình duyệt cào dữ liệu web viết bằng Node.js](https://crawlee.dev/)

Thư viện hỗ trợ xây dựng bot cào dữ liệu web thông minh, đóng gói dựa trên nhân無 đầu trình duyệt Playwright giúp xử lý mượt mà các trang web Single Page Application chạy JS phức tạp.

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082305.webp)

9、[Nolibox Creator: Giao diện WebUI nguồn mở cho mô hình Stable Diffusion](https://creator.nolibox.com/guest)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110307.webp)

Dự án [mã nguồn mở](https://github.com/carefree0910/carefree-creator) xây dựng bảng điều khiển WebUI chuyên nghiệp hỗ trợ người dùng tinh chỉnh trực quan các thông số tạo ảnh nghệ thuật của mô hình Stable Diffusion.

## 资源

1、[Chia sẻ kho ảnh tư liệu khảo cổ học khổng lồ của cố tiến sĩ Lưu Thác](https://mp.weixin.qq.com/s/CwJHo3iLOkOwGz--vFxYPg)

Ngày 26 tháng 10 năm 2021, tiến sĩ khảo cổ học trẻ tuổi Lưu Thác (31 tuổi) của Đại học Bắc Kinh đã không may gặp tai nạn rơi xuống vực qua đời khi đang tiến hành khảo sát các bức bích họa trong hang động cổ tại huyện Barkam, tỉnh Tứ Xuyên.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110303.webp)

Lúc sinh thời, anh đã đặt chân khám phá các di tích lịch sử cổ đại tại hơn 30 quốc gia vùng Trung Đông và Trung Á như Iraq, Afghanistan, Syria, Yemen, Sudan... chụp lại hơn 1 triệu bức ảnh khảo cổ quý giá với dung lượng hơn 10 TB chia thành 15.000 danh mục lưu trữ.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110304.webp)

Nhân ngày giỗ đầu của anh, gia đình và bạn bè đã tiến hành phân loại và chia sẻ miễn phí toàn bộ kho tư liệu hình ảnh di tích vô giá này lên các trang lưu trữ đám mây để phục vụ công tác nghiên cứu học thuật cộng đồng.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110305.webp)

2、[Apple cập nhật giao diện thiết kế mới cho dịch vụ đám mây iCloud Web](https://beta.icloud.com/)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102901.webp)

Apple chính thức phát hành phiên bản giao diện web mới của dịch vụ iCloud với các widget tùy biến thông tin trực quan, hỗ trợ tốt cho người dùng truy cập từ các hệ điều hành Windows hoặc Android.

3、[Windows 11 Hardening: Hướng dẫn tăng cường bảo mật cho Windows 11](https://github.com/beerisgood/Windows11_Hardening)

Thư mục mã nguồn mở tổng hợp chi tiết các thiết lập hệ thống, chỉnh sửa Registry và tắt các dịch vụ chạy ngầm không cần thiết để tối ưu hóa khả năng an toàn thông tin trên Windows 11.

4、[The Flask Mega-Tutorial: Giáo trình học lập trình Python Flask từ cơ bản](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053113.webp)

Sách hướng dẫn lập trình web tiếng Anh miễn phí cực kỳ nổi tiếng, hướng dẫn từng bước từ cài đặt Hello World đến xây dựng một ứng dụng mạng xã hội hoàn chỉnh sử dụng Python và Flask.

5、[3D Math Primer for Graphics and Game Development: Sách toán học 3D cho game](https://gamemath.com/book/intro.html)

Giáo trình trực tuyến cung cấp miễn phí các kiến thức toán học cơ bản (vectơ, ma trận, hệ tọa độ 3D) ứng dụng trực tiếp trong lập trình đồ họa 3D và phát triển game.

## 图片

1\. [Bản đồ thống kê cách biểu đạt tiếng cười trên Internet của các quốc gia](https://preply.com/en/d/laughing-around-the-world-map--lp)

Một nghiên cứu thống kê thú vị về cách biểu thị tiếng cười viết bằng ký tự của cư dân mạng ở các quốc gia khác nhau: ví dụ ở Mỹ dùng "haha", ở Anh dùng từ viết tắt "LOL", còn ở Trung Quốc dùng dãy số "23333".

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061601.webp)

2\. [Quỹ di sản Tolkien lần đầu công bố các bức tranh vẽ tay của tác giả J.R.R. Tolkien](https://www.tolkienestate.com/painting/)

Nhân sự kiện ra mắt giao diện trang chủ mới, quỹ quản lý di sản của tác giả bộ tiểu thuyết kinh điển *Chúa tể những chiếc nhẫn* (The Lord of the Rings) đã công bố những bức phác họa vẽ tay do chính tác giả vẽ để minh họa thế giới Trung Địa (Middle-earth) trong trí tưởng tượng của ông:

(1) Tháp Orthanc nơi ngự trị của phù thủy trắng Saruman:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061602.webp)

(2) Pháo đài hắc ám Barad-dûr của chúa tể Sauron tại Mordor:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061603.webp)

(3) Cảnh quan yên bình của ngôi làng xứ Shire nơi người Hobbit sinh sống:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061604.webp)

(4) Hang báu vật chứa đầy vàng bạc của con rồng Smaug khổng lồ dưới lòng Núi Cô Đơn:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061605.webp)

## ✍️ Bài đọc thêm

### Lý giải nguyên nhân nhiều kỹ sư phần mềm thường có xu hướng yêu thích làm mộc thủ công

Nhiều lập trình viên phần mềm sau giờ gõ code căng thẳng thường chọn sở thích tự tay đóng các đồ gỗ nội thất gia đình (Làm mộc - Woodworking):

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110201.webp)

Đây hoàn toàn không phải sự ngẫu nhiên. Môn thủ công mỹ nghệ làm mộc sở hữu những đặc tính tư duy tương đồng sâu sắc với công việc viết code lập trình:

1. **Đều bắt đầu từ việc thiết kế sản phẩm**: Trước khi bắt tay cắt gỗ hay gõ dòng code đầu tiên, bạn bắt buộc phải có một bản vẽ thiết kế chi tiết để hình dung các bộ phận kết nối và tương tác với nhau như thế nào để tránh sai sót hệ thống.
2. **Hệ thống công cụ hỗ trợ phong phú**: Làm mộc yêu cầu sử dụng rất nhiều dụng cụ chuyên dụng như máy khoan, máy cưa, máy bào, đục, dũa, búa... tương tự như bộ công cụ lập trình viên (IDE, Git, libraries, debuggers) và yêu cầu bạn phải tự tìm ra công cụ tối ưu cho từng tác vụ.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110202.webp)

3. **Làm việc trong các giới hạn tài nguyên**: Trong khi lập trình bị giới hạn bởi dung lượng RAM, băng thông và năng lực xử lý của CPU, làm mộc bị ràng buộc trực tiếp bởi kích thước vật lý của thanh gỗ và diện tích không gian của căn phòng.
4. **Quy trình chờ đợi để hoàn thiện**: Lập trình viên phải chờ đợi quá trình build code và chạy thử nghiệm (compiling); thợ làm mộc cũng phải chờ đợi các lớp keo dán gỗ hoặc nước sơn phủ bề mặt khô hoàn toàn mới có thể tiến hành bước tiếp theo.
5. **Đều hướng tới sản phẩm phục vụ người dùng thực tế**: Đồ gỗ đóng xong để gia đình sử dụng cũng giống như phần mềm viết xong để khách hàng trải nghiệm.

Làm mộc mang lại những phản hồi vật lý trực quan tức thì hơn, giúp lập trình viên tạm rời xa màn hình máy tính để rèn luyện thể chất mà vẫn duy trì được tư duy logic sáng tạo tương tự lập trình nên có sức hút rất lớn với giới kỹ sư công nghệ.

## 历史上的本周

- 2021年（第 181 期）：[Giao diện người dùng: Các giải pháp thiết kế luồng thanh toán không chạm trên thiết bị di động tối ưu trải nghiệm](https://www.ruanyifeng.com/blog/2021/10/weekly-issue-181.html)
- 2020年（第 131 期）：[Tư duy logic: Phân tích sự khác biệt giữa mô hình tư duy logic nhị phân (boolean) và logic tam phân](https://www.ruanyifeng.com/blog/2020/10/weekly-issue-131.html)
- 2019年（第 79 期）：[Xã hội học: Nhìn nhận sự phụ thuộc ngày càng lớn của con người hiện đại vào các hệ thống máy móc tự động](https://www.ruanyifeng.com/blog/2019/10/weekly-issue-79.html)
- 2018年（第 28 期）：[Triết học công nghệ: Thảo luận liệu việc phát triển phần mềm có được coi là một dạng tri thức khoa học thực thụ](https://www.ruanyifeng.com/blog/2018/10/weekly-issue-28.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2715) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## 鸣谢

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072108.webp)

（Hết）
