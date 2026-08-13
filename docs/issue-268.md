# Bản tin chia sẻ công nghệ (Số 268): "Năng suất" là để mô tả máy móc, không phải con người

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3324) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081801.webp)

Tại khu vực sa mạc Gobi thuộc huyện Qua Châu, tỉnh Cam Túc, có một bức tượng chân dung khổng lồ mang tên "Hán Vũ Đại Đế". Cách đây hơn hai ngàn năm, vị hoàng đế Hán Vũ Đế đã từng phái binh sĩ chinh phạt và đánh bại quân Hung Nô ngay tại mảnh đất này. Bức tượng cao 12,5 mét này được chế tác hoàn toàn từ đá sa thạch đỏ, ứng dụng công nghệ khắc 3D và ghép nối tỉ mỉ từ nhiều khối đá độc lập. (Nguồn: [Sohu](https://www.sohu.com/a/542903530_120615216))

## 生产力是形容机器，不是形容人

Trong giới công nghệ, việc các lập trình viên sau khi khởi nghiệp thành công vẫn duy trì niềm đam mê viết sách chia sẻ kiến thức là điều vô cùng hiếm hoi. Bản thân tôi chỉ biết đến một trường hợp duy nhất:

Jason Fried và David Heinemeier Hansson (thường gọi là DHH) là những người sáng lập cốt lõi của công ty Internet nổi tiếng [37signals](https://37signals.com/) (đơn vị đứng sau Basecamp và dịch vụ email HEY). Bên cạnh công việc viết mã lập trình, họ có sở thích đặc biệt là viết sách.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081906.webp)

Đến nay, họ đã cùng nhau xuất bản 4 cuốn sách nổi tiếng và đều đã được dịch sang nhiều ngôn ngữ trên thế giới:

* *Getting Real* (Thực tế), 2006
* *Rework* (Khác biệt để thành công), 2010
* *Remote* (Làm việc từ xa), 2013
* *It Doesn't Have to Be Crazy at Work* (Không cần phải điên cuồng vì công việc), 2018

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081907.webp)

Tôi đã đọc toàn bộ 4 tác phẩm này. Chúng đều là những cuốn sách mỏng, tập hợp các bài viết ngắn gọn phác họa sâu sắc tư duy và triết lý kinh doanh độc đáo của hai tác giả.

Chủ đề xuyên suốt các bài viết của họ tựu trung lại trong một câu hỏi cốt lõi: **Làm thế nào để xây dựng và vận hành một doanh nghiệp Internet theo mô hình "nhỏ mà đẹp"**?

Doanh nghiệp của họ chỉ duy trì quy mô vài chục nhân sự, chưa từng tiếp nhận bất kỳ nguồn vốn đầu tư mạo hiểm nào từ bên ngoài nhưng vẫn hoạt động cực kỳ hiệu quả với doanh thu hàng chục triệu USD mỗi năm. Các cuốn sách của họ chính là lời giải thích tường tận cho triết lý kinh doanh đó.

Gần đây tôi đã đọc xong cuốn sách thứ tư của họ, bản dịch tiếng Trung mang tên *Rework 3: Thoát khỏi sự bận rộn điên cuồng* (It Doesn't Have to Be Crazy at Work).

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081908.webp)

Trong đó, [có một bài viết](https://world.hey.com/jason/effective-productive-acfa210d) đặc biệt sâu sắc mang lại cho tôi một góc nhìn hoàn toàn mới mẻ muốn chia sẻ cùng bạn đọc:

Tác giả lập luận rằng: **Chúng ta tuyệt đối không nên sử dụng khái niệm "năng suất" (productivity) để đánh giá năng lực của một lập trình viên, bởi vì đây là thuật ngữ được sinh ra để đo lường hiệu suất của máy móc chứ không phải con người.**

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081909.webp)

Khái niệm "năng suất" (tiếng Anh: *productive*) bản chất được đo lường bằng số lượng sản phẩm đầu ra (output) tạo ra trong một đơn vị thời gian. Người có năng suất cao là người làm được nhiều việc hơn trong cùng một quỹ thời gian, hoặc hoàn thành cùng một đầu việc với thời gian ngắn hơn.

Nếu một doanh nghiệp lựa chọn "năng suất" làm thước đo chính để đánh giá giá trị của nhân sự, hệ quả tất yếu là mọi người sẽ bị cuốn vào vòng xoáy chạy theo số lượng sản lượng không bao giờ có điểm dừng. Máy móc có thể vận hành liên tục 24/7 không nghỉ, nhưng con người thì không thể làm vậy.

Trong ngành công nghiệp phần mềm từ lâu vẫn lưu truyền giai thoại về việc săn tìm các "lập trình viên 10x" – những người được cho là có năng suất cao gấp 10 lần bình thường. Bản chất của mục tiêu này là tìm kiếm những nhân sự tạo ra sản lượng code khổng lồ, một tư duy quản trị không thực sự lành mạnh.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082309.webp)

**Khi bạn đặt nặng yếu tố năng suất, bạn vô tình áp đặt một tư duy rằng con người bắt buộc phải luôn ở trong trạng thái bận rộn. Mỗi giây phút trôi qua đều phải có việc để làm, và luôn có vô số việc mới đang chờ đón!** Hệ quả là bạn sẽ đối mặt với núi công việc không bao giờ cạn, quỹ thời gian cá nhân ngày càng thu hẹp và áp lực công việc ngày một đè nặng.

**Mục tiêu thực sự mà một lập trình viên nên hướng tới phải là "tính hiệu quả" (effective)**. Nghĩa là sức lao động của bạn mang lại kết quả thực chất, giải quyết được bài toán cốt lõi và giúp dự án hoàn thành đúng mục tiêu.

Khi bạn lấy "tính hiệu quả" làm kim chỉ nam, ngay khi dự án được hoàn thành tốt, bạn có thể tự tin dừng lại để nghỉ ngơi. Nhờ vậy, bạn có thể chủ động tìm kiếm các giải pháp tối ưu để làm ít việc hơn, tốn ít thời gian hơn mà vẫn đạt được kết quả mong muốn, giúp công việc được duy trì một cách bền vững lâu dài.

Mục tiêu chạy theo năng suất (*productive*) sẽ chiếm đoạt toàn bộ quỹ thời gian trống và nhét kín lịch làm việc của bạn để tạo ra nhiều sản lượng nhất có thể.

Ngược lại, mục tiêu hướng tới tính hiệu quả (*effective*) không tìm cách nhét thêm các nhiệm vụ mới, mà tập trung loại bỏ những việc dư thừa không đáng làm để tối ưu hóa nguồn lực.

Nếu trong công việc, có ai đó tán dương bạn là một người có năng suất làm việc cực cao, hoặc công ty của bạn đang áp dụng KPI đo lường năng suất, hãy hết sức cảnh giác: bạn đang đối mặt với rủi ro bị biến thành một cỗ máy thuần túy. Lời khen ngợi ý nghĩa và nhân văn hơn nên là: phương pháp làm việc của bạn rất hiệu quả và chất lượng.

37signals chính là doanh nghiệp tiên phong vận hành theo triết lý này và các cuốn sách của họ luôn nỗ lực truyền tải thông điệp: từ bỏ tư duy cuồng công việc, hướng tới việc đạt kết quả tối ưu với chi phí nguồn lực tối thiểu.

Chuyên mục "Bài đọc thêm" ở cuối bản tin tuần này sẽ trích dẫn một bài viết thú vị khác từ cuốn sách này.

## 云原生深圳沙龙

Mô hình kiến trúc phần mềm phổ biến nhất hiện nay chắc chắn là **Vân Nguyên Sinh (Cloud Native) – phương thức xây dựng và vận hành ứng dụng được thiết kế tối ưu ngay từ đầu cho môi trường điện toán đám mây**. Hầu hết các tập đoàn công nghệ lớn đều đang chuyển dịch hệ thống theo mô hình này.

Vào chiều thứ Bảy tuần này (ngày 26 tháng 8), tại Thâm Quyến sẽ diễn ra một buổi hội thảo kỹ thuật chuyên đề chia sẻ về cách thức ứng dụng Cloud Native giúp doanh nghiệp tối ưu hóa quy trình triển khai, tiết kiệm tài nguyên phần cứng và hạ thấp chi phí vận hành.

Sự kiện do cộng đồng Juejin phối hợp cùng Volcengine Cloud Native tổ chức, với sự tham gia chia sẻ kinh nghiệm thực chiến từ các kỹ sư Frontline của ByteDance về quá trình phát triển ứng dụng trên mây.

Bạn đọc quan tâm có thể truy cập [Trang thông tin chính thức của sự kiện](https://mp.weixin.qq.com/s/qoM5zBC9JmVfgCn1gVxkHA) để xem chi tiết lịch trình:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082106.webp)

Địa điểm tổ chức sự kiện tại **Trung tâm Khoa học Công nghệ Sáng tạo Vịnh Thâm Quyến** (văn phòng làm việc của ByteDance Thâm Quyến). Sự kiện hoàn toàn miễn phí tham dự và có hỗ trợ phát sóng trực tiếp online cho các khán giả ở xa.

Đăng ký tham gia sự kiện [tại đây](https://www.bagevent.com/event/8659508?bag_track=ryf) hoặc quét mã QR trong ảnh. Ban tổ chức có chuẩn bị nhiều phần quà bốc thăm may mắn hấp dẫn như loa thông minh Huawei AI, quà tặng lưu niệm Juejin dành cho khách tham dự.

## 科技动态

1、[Mỹ thử nghiệm ghép thận heo biến đổi gen hoạt động thành công trên cơ thể người](https://nyulangone.org/news/pig-kidney-xenotransplantation-performing-optimally-after-32-days-human-body)

Các bác sĩ ngoại khoa tại Đại học New York công bố đã thực hiện thành công ca phẫu thuật ghép thử nghiệm một quả thận heo vào cơ thể người, quả thận đã duy trì hoạt động bài tiết bình thường liên tục trong 32 ngày:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081905.webp)

Đây là lần thử nghiệm thứ ba của đội ngũ y khoa. Khác với hai lần trước thực hiện trên cơ thể người đã qua đời, ca phẫu thuật lần này được tiến hành trên cơ thể của một bệnh nhân đã được xác định chết não và đang duy trì nhịp tim sinh lý nhờ hệ thống máy thở nhân tạo.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081904.webp)

Thử thách lớn nhất của kỹ thuật ghép tạng động vật (Xenotransplantation) là phản ứng đào thải tự nhiên của hệ miễn dịch người khiến tạng ghép ngừng hoạt động. Ở thử nghiệm lần này, quả thận heo đã được tiến hành chỉnh sửa gen cấu trúc trước khi ghép nhằm ức chế phản ứng đào thải của cơ thể nhận. Vào năm ngoái, y học Mỹ cũng từng thực hiện ca ghép tim heo đầu tiên trên thế giới nhưng bệnh nhân đã qua đời sau hai tháng điều trị.

2、[Bí ẩn ngôi nhà gỗ sống sót kỳ diệu giữa tâm điểm vụ cháy rừng lịch sử tại Hawaii](https://www.civilbeat.org/2023/08/what-saved-the-miracle-house-in-lahaina/)

Đợt cháy rừng nghiêm trọng vừa qua tại đảo Maui, Hawaii đã gây nên thảm họa cháy lớn nhất trong vòng hơn một thế kỷ tại Mỹ, phá hủy gần như toàn bộ thị trấn lịch sử Lahaina:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082001.webp)

Gần như toàn bộ các dãy phố đều bị thiêu rụi hoàn toàn thành tro bụi, tuy nhiên hình ảnh vệ tinh và báo chí ghi nhận có một ngôi nhà gỗ sơn đỏ vẫn đứng vững nguyên vẹn giữa đống đổ nát xung quanh:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082002.webp)

Thời điểm xảy ra cháy rừng, chủ nhân ngôi nhà đang đi du lịch ngoài đảo và đã chuẩn bị tinh thần ngôi nhà của mình bị thiêu rụi. Khi nhìn thấy bức ảnh chụp hiện trạng, chính họ cũng vô cùng kinh ngạc và không hiểu vì sao ngôi nhà có thể sống sót.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082003.webp)

Giới chuyên gia phân tích có hai nguyên nhân chính giúp ngôi nhà thoát nạn: Thứ nhất, hướng gió đưa ngọn lửa lan từ phía đông sang, và khu đất phía đông ngôi nhà là một khoảng sân cỏ rộng được dọn dẹp sạch sẽ đóng vai trò như một vành đai ngăn lửa tự nhiên. Thứ hai, vào năm 2021, chủ nhà đã tiến hành cải tạo nâng cấp ngôi nhà (ảnh trên là hiện trạng trước khi sửa), thay thế phần mái lá cũ bằng hệ thống mái tôn thép sơn tĩnh điện chịu nhiệt tốt, giúp ngăn chặn các tàn lửa bay theo gió bám vào mái nhà gây bắt cháy.

3、[SpaceX công bố hình ảnh quá trình gia cố nâng cấp cấu trúc tên lửa đẩy Starship](https://twitter.com/SpaceX/status/1692610662604702138)

Tập đoàn công nghệ SpaceX đã chia sẻ hình ảnh ghi lại cận cảnh quá trình thi công nâng cấp tên lửa đẩy khổng lồ Starship, với hình ảnh hai công nhân đang làm việc trên đỉnh tên lửa phác họa chân thực quy mô khổng lồ của dòng tên lửa mạnh nhất thế giới này:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082202.webp)

Nội dung đợt nâng cấp kỹ thuật này nhằm chuyển đổi cơ chế phân tách giữa tầng đẩy thứ nhất (Super Heavy) và tầng tàu thứ hai (Starship) sang cơ chế tách tầng nóng (Hot-Staging) – tức là động cơ của tầng thứ hai sẽ được kích hoạt đánh lửa trực tiếp trước khi tách rời hoàn toàn khỏi tầng đẩy thứ nhất. Thiết kế này đòi hỏi SpaceX phải gia cố mạnh mẽ cấu trúc chịu lực và chịu nhiệt ở phần đỉnh của tầng đẩy Super Heavy.

Hình ảnh trên mô tả khu vực đỉnh của tầng đẩy thứ nhất sau khi được lắp đặt thêm một vòng đệm lá chắn nhiệt bằng thép có thiết kế các khe thoát khí (hình dưới) để thoát luồng lửa từ động cơ tầng hai:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082203.webp)

4、[Doanh nghiệp Đức trình chiếu tia laser xanh lục công suất lớn nhất thế giới mừng sinh nhật](https://www.swr.de/swraktuell/baden-wuerttemberg/stuttgart/laserstrahl-ueber-ditzingen-102.html)

Để kỷ niệm cột mốc 100 năm ngày thành lập doanh nghiệp, một tập đoàn công nghệ của Đức mới đây đã thực hiện chiếu một luồng tia laser màu xanh lục công suất lớn thẳng lên bầu trời đêm từ trụ sở chính của hãng như một ngọn nến mừng sinh nhật:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082306.webp)

Luồng tia laser này có khả năng chiếu cao tới 10 km vào không trung và người dân sinh sống trong bán kính 80 km xung quanh đều có thể quan sát rõ bằng mắt thường. Đây được ghi nhận là hệ thống trình chiếu laser xanh lục có quy mô lớn nhất thế giới hiện nay:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082307.webp)

Doanh nghiệp thực hiện dự án chính là đơn vị chuyên nghiên cứu và sản xuất các thiết bị phát laser công nghiệp. Một trong những ứng dụng độc đáo của hệ thống laser công suất lớn này là hoạt động như một hệ thống cột thu lôi chủ động: bằng việc bắn tia laser ion hóa không khí lên cao, hệ thống sẽ chủ động dẫn hướng dòng điện của các tia sét từ đám mây xuống đất an toàn để bảo vệ các công trình lớn xung quanh.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082308.webp)

## 文章

1\. [Năm mẹo nhỏ hữu ích nâng cao hiệu quả lập trình với TypeScript](https://double-trouble.dev/post/typescript-tips/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071803.webp)

Bài viết kỹ thuật chia sẻ một số kinh nghiệm thực chiến và mẹo nhỏ khi khai báo kiểu dữ liệu nâng cao trong TypeScript giúp mã nguồn trở nên gọn gàng, chặt chẽ và dễ bảo trì hơn.

2\. [Tìm hiểu cơ chế tự động sinh tên ngẫu nhiên cho container của Docker](https://pet2cattle.com/2022/08/docker-container-names-generator)（Tiếng Anh）

Khi người dùng khởi chạy một container Docker mới mà không chỉ định tham số đặt tên `--name`, Docker sẽ tự động gán cho container đó một cái tên ghép ngẫu nhiên rất ngộ nghĩnh (ví dụ: *Romantic_shtern*). Bài viết giải thích chi tiết cơ chế hoạt động của bộ sinh tên này trong mã nguồn của Docker.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062403.webp)

3\. [Tại sao TypeScript gặp khó khăn khi xử lý kiểu dữ liệu của phương thức Object.keys()](https://alexharri.com/blog/typescript-structural-typing)（Tiếng Anh）

Bài viết phân tích sâu cơ chế kiểm tra kiểu cấu trúc (structural typing) của TypeScript để lý giải nguyên nhân tại sao phương thức `Object.keys()` mặc định không trả về kiểu mảng các thuộc tính của đối tượng, dẫn đến các lỗi cảnh báo kiểu dữ liệu gây phiền hà cho lập trình viên.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062501.webp)

4\. [Hướng dẫn thiết lập và chạy giả lập máy tính Raspberry Pi trong môi trường QEMU](https://interrupt.memfault.com/blog/emulating-raspberry-pi-in-qemu)（Tiếng Anh）

Tài liệu hướng dẫn kỹ thuật chi tiết dành cho các kỹ sư phát triển nhúng: hướng dẫn cách thức sử dụng công cụ ảo hóa nguồn mở QEMU để khởi tạo và chạy giả lập một môi trường phần cứng máy tính Raspberry Pi ngay trên máy tính cá nhân phục vụ viết và debug code.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062701.webp)

5\. [Một chi tiết kỹ thuật thú vị về cấu trúc định dạng của mã định danh UUID phiên bản 4](https://susam.net/blog/from-uuid-to-infinite-loops.html)（Tiếng Anh）

Mã định danh UUID v4 là chuỗi ký tự ngẫu nhiên biểu diễn dưới dạng hệ thập lục phân gồm 32 ký tự thường dùng để định danh đối tượng duy nhất. Bài viết chia sẻ một chi tiết kỹ thuật nhỏ ít người để ý: ký tự ở vị trí thứ 14 trong chuỗi mã UUID v4 luôn được cố định là chữ số `4` để biểu thị phiên bản của chuẩn mã hóa.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072201.webp)

6\. [Hướng dẫn tạo hiệu ứng gấp giấy lật trang độc đáo chỉ bằng mã CSS thuần](https://thomaspark.co/2020/06/the-mad-magazine-fold-in-effect-in-css/)（Tiếng Anh）

Bài viết hướng dẫn lập trình viên Front-end cách thức kết hợp các thuộc tính biến đổi không gian 3D và hiệu ứng chuyển động trong CSS để tạo nên hiệu ứng lật gấp trang giấy tương tác sinh động trên giao diện web mà không cần dùng đến JavaScript.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072502.webp)

7\. [Hướng dẫn chi tiết về cách sử dụng cấu trúc Struct và cơ chế căn chỉnh bộ nhớ trong C](https://abstractexpr.com/2023/06/29/structures-in-c-from-basics-to-memory-alignment/)（Tiếng Anh）

Tài liệu học tập lập trình C cơ bản, giải thích chi tiết cách khai báo sử dụng cấu trúc dữ liệu Struct và đi sâu phân tích nguyên lý căn chỉnh dữ liệu trên bộ nhớ (Memory Alignment) của trình biên dịch giúp tối ưu hóa tốc độ truy xuất dữ liệu của CPU.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062914.webp)

8\. [Tìm hiểu cú pháp Macro mới hỗ trợ biên dịch mã nguồn trong JavaScript](https://bun.sh/blog/bun-macros)（Tiếng Anh）

Bài viết giới thiệu cú pháp Macro – một tính năng mới hỗ trợ lập trình viên thực hiện chạy các đoạn mã tính toán logic ngay trong quá trình build/biên dịch để nhúng kết quả vào file đích, hiện đã được hỗ trợ chính thức bởi trình đóng gói Bun tốc độ cao.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023063001.webp)

## 工具

1、[Simple Statistics: Thư viện JavaScript cung cấp các hàm thống kê toán học cơ bản](http://simplestatistics.org/)

Một thư viện JS gọn nhẹ, không phụ thuộc thư viện ngoài, cung cấp đầy đủ các hàm tính toán thống kê toán học (như tính trung bình, trung vị, độ lệch chuẩn, phân phối chuẩn) hỗ trợ xử lý dữ liệu Front-end.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062814.webp)

2、[豆包 (Doubao): Chatbot trí tuệ nhân tạo tương tác tự do do ByteDance phát hành](https://www.doubao.com/)

Ứng dụng chatbot AI thế hệ mới dựa trên mô hình ngôn ngữ lớn do tập đoàn ByteDance phát triển và cung cấp miễn phí cho người dùng trải nghiệm viết lách, dịch thuật và hỗ trợ lập trình.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081903.webp)

3、[TrackerControl: Ứng dụng Android giám sát và ngăn chặn hành vi thu thập dữ liệu](https://github.com/TrackerControl/tracker-control-android)

Một công cụ bảo mật mạnh mẽ dành cho hệ điều hành Android, giúp người dùng giám sát thời gian thực các kết nối mạng của toàn bộ app trên máy và chủ động chặn đứng các hành vi âm thầm gửi dữ liệu theo dõi thói quen người dùng lên server quảng cáo. (Đóng góp của [@cheanus](https://github.com/ruanyf/weekly/issues/3381))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082011.webp)

4、[DCNews: Công cụ Go hỗ trợ tự động đồng bộ hóa tin nhắn từ WeChat sang Discord](https://github.com/121812/dcnews)

Ứng dụng viết bằng Go hỗ trợ quản trị viên tự động thu thập và đồng bộ các tin nhắn thảo luận từ các nhóm chat WeChat chỉ định sang kênh Discord của cộng đồng theo thời gian thực. (Đóng góp của [@121812](https://github.com/ruanyf/weekly/issues/3382))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082012.webp)

5、[Walrus: Nền tảng quản lý và triển khai ứng dụng nguồn mở tối giản](https://github.com/seal-io/walrus)

Một nền tảng điều phối ứng dụng (Orchestration) giúp các nhà phát triển dễ dàng cấu hình và triển khai nhanh ứng dụng lên các hạ tầng đám mây mà không cần tốn thời gian nghiên cứu sâu các thiết lập hạ tầng Kubernetes hay Terraform bên dưới. (Đóng góp của [@Aleegra](https://github.com/ruanyf/weekly/issues/3385))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082303.webp)

6、[GFPGAN: Công cụ ứng dụng thuật toán AI hỗ trợ phục hồi chất lượng ảnh chân dung cũ](https://github.com/TencentARC/GFPGAN)

Dự án mã nguồn mở do viện nghiên cứu công nghệ Tencent phát triển, ứng dụng các mô hình học sâu giúp tự động làm nét khuôn mặt, loại bỏ vết xước và khôi phục màu sắc cho các bức ảnh chân dung cũ bị mờ nhòe. Bạn đọc có thể dùng thử bản [Demo trực tuyến](https://replicate.com/tencentarc/gfpgan). (Đóng góp của [@Y024](https://github.com/Y024))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082304.webp)

7、[铜钟 (tonzhon): Ứng dụng web nghe nhạc trực tuyến giao diện tinh tế](https://tonzhon.com/)

Một trình phát nhạc chạy trên nền web sở hữu giao diện tối giản hiện đại, tổng hợp tài nguyên bài hát từ nhiều nguồn nhạc trực tuyến lớn giúp người dùng dễ dàng tìm kiếm và thưởng thức âm nhạc. Dự án được [mở nguồn hoàn toàn trên GitHub](https://github.com/enzeberg/tonzhon-music). (Đóng góp của [@enzeberg](https://github.com/enzeberg))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082305.webp)

8、[AutoAnimate: Thư viện JavaScript hỗ trợ tự động sinh hiệu ứng chuyển động web](https://github.com/formkit/auto-animate)

Một công cụ gọn nhẹ giúp tự động thêm các hiệu ứng chuyển động (transition animation) mượt mà cho các phần tử DOM mỗi khi có sự thay đổi trạng thái cấu trúc trang (như thêm/xóa phần tử danh sách), tương thích tốt với React, Vue, Svelte. (Đóng góp của [@GenerQAQ](https://github.com/ruanyf/weekly/issues/3398))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082402.webp)

9、[background-removal-js: Thư viện JavaScript hỗ trợ tách nền hình ảnh trực tiếp trên trình duyệt](https://github.com/imgly/background-removal-js)

Thư viện mã nguồn mở cho phép tích hợp tính năng tự động nhận diện chủ thể và tách bỏ nền ảnh (Remove Background) chạy trực tiếp trên môi trường trình duyệt máy khách mà không cần gửi dữ liệu ảnh về máy chủ xử lý.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062903.webp)

10、[scrcpy: Ứng dụng hỗ trợ phản chiếu và điều khiển màn hình điện thoại Android từ máy tính](https://github.com/Genymobile/scrcpy)

Một công cụ máy tính mã nguồn mở vô cùng nổi tiếng, hỗ trợ truyền hình ảnh hiển thị độ phân giải cao từ điện thoại Android lên màn hình máy tính qua kết nối USB hoặc WiFi, cho phép dùng chuột và bàn phím điều khiển điện thoại mượt mà với độ trễ siêu thấp.

## 资源

1、[WordPress Playground: Môi trường thử nghiệm chạy WordPress trực tiếp trên trình duyệt](https://developer.wordpress.org/playground/)

Dịch vụ thử nghiệm chính thức do dự án WordPress phát triển ứng dụng công nghệ WebAssembly, cho phép khởi chạy một phiên bản WordPress hoàn chỉnh hoạt động hoàn toàn trong bộ nhớ trình duyệt web giúp lập trình viên test nhanh giao diện, plugin mà không cần cài đặt máy chủ.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071501.webp)

2、[Periodic Table Cli: Tiện ích tra cứu bảng tuần hoàn hóa học trực tiếp bằng dòng lệnh](https://github.com/spirometaxas/periodic-table-cli)

Một công cụ dòng lệnh viết bằng Node.js giúp hiển thị bảng tuần hoàn các nguyên tố hóa học trực quan dạng màu sắc ngay trong màn hình terminal, hỗ trợ tra cứu nhanh các thông số vật lý hóa học của từng nguyên tố.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071701.webp)

3、[SQL for Devs: Cuốn sách điện tử tiếng Anh miễn phí chia sẻ các kỹ năng truy vấn SQL](https://sqlfordevs.com/ebook)

Tài liệu học tập SQL nâng cao định dạng PDF miễn phí dành cho các lập trình viên Backend, giới thiệu các phương pháp viết câu lệnh truy vấn phức tạp, tối ưu hóa chỉ mục và tăng tốc độ xử lý cơ sở dữ liệu.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120303.webp)

4、[面试押题王 (yatiwang): Ứng dụng web hỗ trợ sinh câu hỏi và đáp án phỏng vấn thử bằng AI](https://yatiwang.chat/)

Một ứng dụng web hữu ích dành cho người tìm việc: người dùng chỉ cần dán nội dung mô tả vị trí công việc (JD), hệ thống AI sẽ tự động phân tích để sinh ra bộ câu hỏi phỏng vấn sát thực tế đi kèm gợi ý câu trả lời tối ưu. (Đóng góp của [@vickwv](https://github.com/ruanyf/weekly/issues/3397))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082401.webp)

## 图片

1、**Thiết kế độc đáo của bộ hộp đọc ổ cứng SSD M.2 mô phỏng bóng đèn chân không**

Một doanh nghiệp sản xuất phụ kiện phần cứng máy tính của Đức mới đây đã cho ra mắt dòng sản phẩm hộp đọc ổ cứng di động SSD chuẩn M.2 NVMe sở hữu ngôn ngữ thiết kế vô cùng độc đáo mô phỏng hình dáng của các bóng đèn chân không (vacuum tube) cổ điển:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082109.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082110.webp)

2、**Khám phá thông điệp nhị phân ẩn giấu dưới nền gạch tòa nhà Đại học UCLA**

Vào năm 1969, nhóm nghiên cứu tại Đại học California, Los Angeles (UCLA) đã thực hiện gửi đi thông điệp truyền tải dữ liệu qua mạng Internet sơ khai đầu tiên trong lịch sử nhân loại.

Theo kế hoạch, các kỹ sư dự định gõ từ "LOGIN" để kết nối với máy tính ở viện nghiên cứu Stanford. Tuy nhiên, hệ thống mạng đã bị đổ vỡ ngay sau khi họ mới chỉ gõ gửi đi được hai ký tự đầu tiên là "LO".

Vào năm 2011, nhân dịp cải tạo nâng cấp tòa sảnh Boelter Hall của trường – địa điểm diễn ra sự kiện lịch sử năm xưa, các kiến trúc sư đã sử dụng hai tông màu gạch lát nền để khảm một chuỗi mã nhị phân ẩn dưới sàn nhà làm kỷ niệm:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082006.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082005.webp)

Chuỗi gạch khảm gồm 14 dòng gạch lớn, mỗi dòng gồm 8 ô vuông đại diện cho 1 byte dữ liệu:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082007.webp)

Khi tiến hành chuyển đổi vị trí các viên gạch màu đậm nhạt thành chuỗi mã nhị phân 0 và 1 tương ứng (hình dưới):

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082008.webp)

Và thực hiện tra cứu dịch nghĩa chuỗi mã nhị phân này theo bảng mã chuẩn ASCII, chúng ta sẽ nhận được dòng chữ tiếng Anh: **“lo and behold!”** (Hãy nhìn xem! - một câu cảm thán cổ biểu thị sự ngạc nhiên thú vị, đồng thời chơi chữ ghép từ hai ký tự đầu tiên "LO" lịch sử năm xưa).

## ✍️ Bài đọc thêm

### Triết lý quản trị "Chúng ta không phải là một gia đình" tại doanh nghiệp

*Bài viết được trích dịch từ nội dung cuốn sách Rework 3 của ban lãnh đạo công ty công nghệ 37signals.*

Nhiều doanh nghiệp hiện nay rất thích tuyên truyền và quảng bá khẩu hiệu: *"Ở công ty chúng ta, mọi thành viên đều là người trong một đại gia đình"*. Thực tế phũ phàng là: doanh nghiệp và nhân viên hoàn toàn không phải là người nhà của nhau.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082310.webp)

Tại 37signals, chúng tôi cũng chưa từng coi công ty là một gia đình. Chúng tôi định vị rõ ràng bản thân là những người đồng nghiệp phối hợp công việc. Điều này hoàn toàn không có nghĩa là chúng tôi thờ ơ và không quan tâm đến nhau. Chúng tôi luôn sẵn lòng hỗ trợ, chia sẻ khó khăn cùng đồng nghiệp trong cuộc sống, nhưng chúng tôi không phải là người nhà. Thực tế tại công ty của bạn cũng hoàn toàn tương tự như vậy.

Chúng ta là một tập thể nhân sự tụ họp lại cùng làm việc vì mục tiêu chung là tạo ra những sản phẩm công nghệ chất lượng. Chúng ta cùng nhau cống hiến chất xám để làm ra những sản phẩm hoàn thiện nhất, nhưng chúng ta không có nghĩa vụ phải hy sinh hạnh phúc cá nhân hay sức khỏe vì lợi ích của công ty. Bạn đối với công ty của mình cũng nên có tư duy như vậy.

Chúng tôi tự hào về chất lượng những sản phẩm do mình làm ra. Cảm xúc tự hào nghề nghiệp đó đã là quá đủ để thúc đẩy công việc.

Mỗi khi thấy các nhà quản lý cấp cao ra sức thuyết phục nhân viên rằng công ty là một "đại gia đình hạnh phúc ấm áp", bạn nên hết sức tỉnh táo đề phòng. Thông thường, thông điệp ẩn ý phía sau câu nói đó không phải là công ty sẽ bao dung nâng đỡ bạn vô điều kiện mỗi khi bạn gặp biến cố cuộc đời, mà ý của họ là: **Họ đang yêu cầu một sự hy sinh đơn phương từ phía bạn.**

Bởi vì một khi đã khoác lên mình chiếc áo tình cảm mang tên "gia đình", tâm lý đồng cam cộng khổ sẽ tự động được kích hoạt. Việc bạn tự nguyện làm việc tăng ca đến đêm muộn hay chủ động hủy bỏ kỳ nghỉ cá nhân để hoàn thành công việc sẽ không còn bị coi là việc vắt kiệt sức lao động giúp doanh nghiệp kiếm thêm lợi nhuận nữa, mà sẽ được ca tụng là sự cống hiến cao cả cho "đại gia đình chung".

Thực chất, đây chỉ là một đòn tâm lý vụng về của nhà quản trị nhằm khiến nhân viên tự nguyện từ bỏ các quyền lợi cá nhân hợp pháp của mình vì lợi ích của công ty.

Doanh nghiệp không phải là một tổ chức giang hồ thu nhận các trẻ mồ côi để đào tạo chúng đi tranh giành địa bàn cho gia tộc. Việc công ty cố tình đóng giả làm gia đình thực chất là một chiêu trò tinh quái nhằm đặt lợi ích công việc lên trên lợi ích gia đình thực sự của người lao động.

Những doanh nghiệp nhân văn và xuất sắc nhất không bao giờ tự nhận mình là gia đình của bạn. Họ định vị mình là người đồng minh đáng tin cậy, là hậu thuẫn vững chắc hỗ trợ cho gia đình thực sự của bạn. Họ nỗ lực xây dựng một môi trường làm việc lành mạnh giúp nhân viên có thể thoải mái gập máy tính đúng giờ sau ca làm để trở về nhà làm một người cha, người mẹ, người chồng, người vợ tốt nhất cho tổ ấm thực sự của mình.

## Lịch sử tuần này

- 2022年（第 221 期）：[Ngành dịch vụ: Phân tích chặng đường phát triển và cơ hội của ngành công nghiệp dịch vụ trên thế giới](http://www.ruanyifeng.com/blog/2022/09/weekly-issue-221.html)
- 2021年（第 171 期）：[Hạ tầng mạng: Tìm hiểu chi phí băng thông đắt đỏ của các nhà cung cấp đám mây lớn](http://www.ruanyifeng.com/blog/2021/08/weekly-issue-171.html)
- 2020年（第 121 期）：[Xã hội học: Tại sao năng suất lao động tăng cao nhưng con người ngày càng không có nhiều thời gian rảnh](http://www.ruanyifeng.com/blog/2020/08/weekly-issue-121.html)
- 2019年（第 71 期）：[Khởi nghiệp: Tại sao nhóm sinh viên tốt nghiệp từ các trường danh tiếng lại gặp nhiều khó khăn khi khởi nghiệp](http://www.ruanyifeng.com/blog/2019/08/weekly-issue-71.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes team collaboration and workspace sharing smooth and effective.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
