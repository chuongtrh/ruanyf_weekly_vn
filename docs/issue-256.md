# Bản tin chia sẻ công nghệ (Số 256): Tác phẩm Lego ấn tượng nhất

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3091) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052522.webp)

Vào ngày kỷ niệm tình yêu "520" vừa qua, tại khu công viên cây xanh thuộc quận Tây Hồ, Hàng Châu đã xuất hiện một mô hình hoa hồng khổng lồ được tạo nên bằng công nghệ in 3D với đường kính bông hoa lên tới 2,4 mét. (Nguồn: [Weibo](https://weibo.com/2097152664/N1jdzBewt))

## 最酷的乐高作品

Có lẽ tất cả chúng ta đều đã quá quen thuộc với cái tên Lego – tập đoàn đồ chơi nổi tiếng thế giới chuyên sản xuất các viên gạch lắp ráp bằng nhựa.

Từ một túi linh kiện nhựa thô sơ mua về, người chơi có thể tỉ mỉ lắp ráp theo sách hướng dẫn đi kèm, hoặc tự do sáng tạo thành bất kỳ mô hình hình học nào theo trí tưởng tượng của mình.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052219.webp)

Mới đây, một nhà sáng chế nước ngoài đã sử dụng các linh kiện Lego kỹ thuật để lắp ráp nên một cỗ máy độc đáo vượt xa tưởng tượng của mọi người: [Hộp giảm tốc Google](https://brickexperimentchannel.wordpress.com/2023/04/29/lego-googol-machine/) (Googol Machine).

Tôi thấy ý tưởng này vô cùng thú vị nên muốn chia sẻ chi tiết cùng các bạn hôm nay.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052210.webp)

Nguồn động lực chính của cỗ máy đến từ một động cơ điện mini xoay liên tục với tốc độ 375 vòng mỗi phút:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052404.webp)

Dòng truyền động này sau đó được dẫn qua một chuỗi các bánh răng giảm tốc cơ học liên hoàn, cuối cùng kết nối để làm xoay một búp bê nhựa đặt ở đầu ra.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052211.webp)

Điểm đáng kinh ngạc nhất của cỗ máy Lego này là tỷ số truyền giảm tốc tổng thể đạt tới con số không tưởng: **10^100 : 1** (một Googol)!

Điều này có nghĩa là động cơ điện ban đầu phải xoay đủ 10^100 vòng thì búp bê Lego ở đầu ra mới có thể hoàn thành đúng 1 vòng quay. Để dễ hình dung về độ lớn của con số này: tổng số lượng nguyên tử cấu thành nên toàn bộ vũ trụ quan sát được của chúng ta ước tính chỉ vào khoảng 10^80. Điều này đồng nghĩa với việc ngay cả khi chúng ta cắm điện cho cỗ máy chạy liên tục từ nay cho đến tận ngày vũ trụ lụi tàn, búp bê Lego kia thậm chí vẫn chưa thể di chuyển nổi một milimet.

Nguyên lý cơ học đứng sau hệ thống giảm tốc kỳ diệu này thực chất rất đơn giản: sử dụng cơ chế bánh răng nhỏ dẫn động bánh răng lớn.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052212.webp)

Như hình ảnh trên, một bánh răng nhỏ có 8 răng được gắn vào trục động cơ để dẫn động một bánh răng lớn có 24 răng. Do bánh răng lớn có kích thước gấp 3 lần bánh răng nhỏ, tốc độ quay của nó sẽ bị giảm đi đúng 3 lần.

Tiếp theo, trên trục của bánh răng lớn này lại được cố định thêm một bánh răng nhỏ 8 răng để tiếp tục dẫn động một bánh răng lớn hơn nữa có 40 răng:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052213.webp)

Theo cách đó, tốc độ quay của bánh răng thứ ba sẽ tiếp tục chậm đi 5 lần (40 / 8) so với bánh răng thứ hai, tương đương với việc chậm đi tới 15 lần (3 x 5) so với tốc độ quay ban đầu của động cơ.

Bằng cách liên tục lặp lại và ghép nối nối tiếp các cặp bánh răng giảm tốc này, tốc độ quay ở các trục sau sẽ ngày càng chậm đi theo cấp số nhân:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052214.webp)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052215.webp)

Để tăng hiệu quả giảm tốc, tác giả thậm chí đã đưa vào sử dụng các bánh răng siêu lớn có tới 168 răng:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052216.webp)

Cùng việc kết hợp đa dạng các tổ hợp bánh răng cơ học phức tạp khác:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052217.webp)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052218.webp)

Kết quả cuối cùng là tạo nên một cỗ máy Lego nhỏ gọn sở hữu tỷ số truyền động giảm tốc đạt mốc kỷ lục 10^100:1.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052220.webp)

Tôi chưa bao giờ nghĩ rằng những viên gạch đồ chơi Lego bằng nhựa lại có thể tạo nên một cỗ máy chạm tới các đại lượng số học ở cấp độ vũ trụ như vậy, đây quả thực là một thực nghiệm vật lý tuyệt vời.

## 腾讯 PAG 动效组件

Tuần trước, tôi có dịp gặp gỡ một kỹ sư làm việc tại tập đoàn Tencent.

Anh chia sẻ rằng Tencent đang sở hữu một giải pháp công nghệ hoạt họa rất chất lượng nhưng chưa được nhiều lập trình viên bên ngoài biết đến rộng rãi, đó chính là **Bộ linh kiện xử lý hoạt ảnh PAG** ([PAG Art](https://pag.art/)).

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052201.webp)

Phản ứng ban đầu của tôi là hoài nghi: một công cụ xử lý hiệu ứng ảnh động thông thường thì có gì quá đặc biệt để nghiên cứu? Nhưng sau khi trực tiếp tìm hiểu các thông số kỹ thuật, tôi nhận thấy đây thực sự là một giải pháp rất đột phá.

Về mặt tính năng, ưu điểm nổi bật nhất của PAG là khả năng hỗ trợ đa nền tảng tuyệt đối. Lập trình viên chỉ cần thiết kế hiệu ứng hoạt ảnh đúng một lần duy nhất là có thể triển khai chạy mượt mà trên **mọi nền tảng phần mềm** từ ứng dụng di động (iOS/Android), ứng dụng web, mini program của WeChat cho đến các hệ điều hành máy tính (Windows, macOS, Linux). Bản thân tên gọi PAG chính là viết tắt của cụm từ *Portable Animated Graphics* (Đồ họa hoạt ảnh di động).

Làm thế nào hệ thống có thể bảo đảm một tệp tin hoạt ảnh động hiển thị đồng bộ và mượt mà trên nhiều hệ điều hành có cấu trúc nhân đồ họa hoàn toàn khác biệt như vậy?

Giải pháp của Tencent là tự phát triển một nhân kết xuất đồ họa độc lập viết hoàn toàn bằng ngôn ngữ C++, sau đó xây dựng các lớp giao tiếp thích ứng riêng cho từng hệ điều hành.

Do đó, cơ chế hoạt động của PAG khác biệt hoàn toàn so với các công cụ tạo ảnh động thông thường; hệ thống không phụ thuộc vào bộ thư viện đồ họa tích hợp sẵn của hệ điều hành máy khách mà hoạt động như **một giải pháp kết xuất đồ họa độc lập hoàn chỉnh**:

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=n3515fscu2f" allowFullScreen="true" width="600" height="400"></iframe>

Nhờ sở hữu nhân đồ họa độc lập, PAG mang lại nhiều ưu điểm vượt trội cho các dự án phần mềm:

1. **Tiết kiệm tối đa chi phí phát triển**: Chỉ cần thiết lập hiệu ứng một lần duy nhất, giảm thiểu công sức viết mã giao diện riêng cho từng nền tảng mà vẫn bảo đảm trải nghiệm hiển thị đồng bộ.
2. **Tối ưu hóa quy trình cộng tác giữa thiết kế và lập trình**: Trước đây, việc đưa các hiệu ứng chuyển động phức tạp vào ứng dụng là quy trình rất tốn thời gian. Nhà thiết kế phải dựng hoạt ảnh trên phần mềm chuyên dụng After Effects (AE), sau đó xuất ra video hoặc ảnh để lập trình viên xem và cố gắng viết mã mô phỏng lại. Quy trình này đòi hỏi hai bên phải liên tục chỉnh sửa và kiểm thử nhiều lần mới đạt yêu cầu. Với PAG, quy trình được rút gọn tối đa: Lập trình viên chỉ cần nhúng bộ thư viện SDK của PAG vào ứng dụng; nhà thiết kế sử dụng plugin PAG chuyên dụng cài trực tiếp trên phần mềm AE để xuất thẳng ra file định dạng nhị phân `.pag` và đưa vào ứng dụng chạy trực tiếp mà không cần lập trình viên viết thêm dòng code giao diện nào.
3. **Hỗ trợ toàn diện các tính năng của After Effects**: Hầu như mọi hiệu ứng chuyển động, mặt nạ, hạt hay vector dựng được trên phần mềm AE chuyên nghiệp đều được nhân đồ họa của PAG phân tích và tái hiện hoàn hảo.
4. **Dung lượng tệp tin siêu nhẹ**: Tệp tin hoạt ảnh của PAG được lưu trữ dưới dạng nhị phân tối ưu. So với định dạng file JSON/SVG của thư viện Lottie nổi tiếng trước đây, tệp PAG có dung lượng nhỏ hơn nhiều lần và tốc độ phân tích cú pháp để hiển thị nhanh hơn vượt trội. Nhiều hoạt ảnh chuyển động phức tạp chỉ có dung lượng vỏn vẹn khoảng 2 KB. Định dạng nhị phân này cũng hỗ trợ đóng gói kèm theo các tệp hình ảnh bitmap, âm thanh và video trực tiếp vào trong một file duy nhất để phân phối tiện lợi.
5. **Cung cấp bộ công cụ xem trước trực quan [PAG Viewer](https://pag.art/docs/pag-viewer.html)**: Phần mềm hỗ trợ xem trước hiệu ứng trực quan, cho phép chỉnh sửa nhanh các đoạn văn bản hoặc thay đổi hình ảnh trực tiếp bên trong tệp nhị phân trước khi đóng gói phát hành.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052203.webp)

Để xây dựng được bộ công cụ hoạt họa chất lượng này, Tencent đã liên tục đầu tư nghiên cứu và phát triển suốt từ năm 2017. Hiện tại hệ thống đã được ứng dụng rộng rãi trên hàng ngàn sản phẩm lớn của tập đoàn như ứng dụng WeChat, QQ, game Vương Giả Vinh Diệu cũng như các đối tác lớn như Xiaohongshu hay Zhihu. Toàn bộ các hiệu ứng quà tặng chuyển động 3D khi xem livestream trên WeChat hay các khung vinh danh chiến báo trong game đều được kết xuất bằng công cụ này.

Bạn đọc có thể truy cập [Thư viện dự án thực tế](https://pag.art/case.html) hoặc trang chia sẻ tài nguyên hoạt ảnh [动池](https://animate.art/) để xem các sản phẩm chuyển động thực tế.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052204.webp)

Năm ngoái, Tencent đã chính thức **mở mã nguồn mở hoàn toàn cho dự án PAG** trên GitHub tại địa chỉ [libpag GitHub](https://github.com/tencent/libpag) và hiện đã thu hút được hơn 3.000 lượt yêu thích từ cộng đồng phát triển. Bạn đọc có thể truy cập trang chủ [pag.art](https://pag.art/) để tìm hiểu tài liệu kỹ thuật và tải về sử dụng thử nghiệm cho các dự án của mình.

## 科技动态

1、[Humane giới thiệu thiết bị công nghệ điều khiển bằng giọng nói hướng tới thay thế điện thoại](https://interestingengineering.com/innovation/humane-ai-wearable-potential-iphone-killer)

Một startup công nghệ tại Mỹ mới đây đã công bố dòng sản phẩm thiết bị đeo thông minh nhỏ gọn điều khiển bằng giọng nói tích hợp AI, được giới truyền thông đánh giá là có tiềm năng thay thế điện thoại thông minh:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052205.webp)

Điểm đặc biệt nhất của thiết bị này là loại bỏ hoàn toàn màn hình kính truyền thống. Khi cần hiển thị thông tin, thiết bị sẽ sử dụng một máy chiếu laser siêu nhỏ để chiếu hình ảnh trực tiếp lên lòng bàn tay của người dùng hoặc lên bề mặt phẳng bất kỳ. Nhờ tích hợp AI thấu hiểu giọng nói tốt, người dùng có thể thực hiện mọi thao tác gọi điện, nhắn tin hay tra cứu thông tin bằng khẩu lệnh một cách dễ dàng, giúp giảm thiểu đáng kể hội chứng nghiện màn hình điện thoại của giới trẻ.

2、[Họa sĩ Mỹ thử nghiệm xuất bản cuốn truyện tranh đầu tiên được vẽ hoàn toàn bằng AI](https://the-decoder.com/the-last-stargazer-is-a-comic-created-with-ai-art/)

Một tác giả truyện tranh người Mỹ đã ứng dụng các công cụ vẽ tranh AI để hoàn thiện và xuất bản thành công cuốn truyện tranh mang tên *“The Last Stargazer”* trên cửa hàng sách Amazon:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112704.webp)

Tác giả chia sẻ khó khăn kỹ thuật lớn nhất khi vẽ truyện tranh bằng AI là việc duy trì sự đồng bộ về nét vẽ và khuôn mặt của nhân vật chính xuyên suốt các khung hình khác nhau. Để giải quyết, ông đã phải cắt riêng khuôn mặt chuẩn của nhân vật (ảnh giữa dưới) để nạp làm dữ liệu tham chiếu đầu vào cho AI trong mọi câu lệnh Prompt:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112702.webp)

Bên cạnh đó, các bức ảnh do AI sinh ra thường xuyên gặp lỗi cấu trúc giải phẫu học (như vẽ thiếu chi hoặc thừa ngón tay), buộc tác giả phải tiến hành chỉnh sửa thủ công bằng phần mềm đồ họa. Dẫu vậy, chất lượng hình ảnh cuối cùng của tác phẩm vẫn rất ấn tượng:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112703.webp)

Cuốn sách được hoàn thành chỉ trong vòng một tháng và đang ghi nhận doanh số bán rất khả quan. Trong tương lai, các tác phẩm nghệ thuật sáng tạo sẽ ngày càng có sự tham gia sâu sắc của các công cụ AI hỗ trợ.

3、[Mẫu thiết bị nhà chờ xe buýt siêu nhỏ gây tranh cãi tại Los Angeles](https://walkingtheworld.substack.com/p/why-the-us-cant-have-nice-things)

Chính quyền thành phố Los Angeles vừa qua đã tổ chức lễ ra mắt dòng sản phẩm nhà chờ xe buýt thế hệ mới được tích hợp tấm che nắng ban ngày và hệ thống đèn đường chiếu sáng ban đêm:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052511.webp)

Tuy nhiên thiết kế thực tế của thiết bị này nhanh chóng nhận về làn sóng chỉ trích lớn từ dư luận do kích thước quá nhỏ hẹp, hầu như chỉ đủ che nắng cho đúng một người đứng thẳng và không có ghế ngồi:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052512.webp)

Truyền thông địa phương lên tiếng nghi ngờ về tính thực tiễn của thiết kế này khi mỗi cột chờ xe buýt như vậy có chi phí lắp đặt lên tới 10.000 USD. Trên thực tế, Los Angeles sở hữu nhiều nhà chờ xe buýt lớn hiện đại (hình dưới) nhưng các địa điểm này thường xuyên bị lạm dụng làm nơi cư trú của người vô gia cư. Thiết kế cột chờ siêu nhỏ mới này là giải pháp nhằm hạn chế tình trạng trên tại các điểm dừng vùng ngoại ô, nhưng thiết kế quá tối giản của nó khiến nhiều người cho rằng thà lắp đặt một cột đèn đường thông thường còn hiệu quả hơn.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052513.webp)

4、[Mỹ thử nghiệm công nghệ máy bay không người lái cất hạ cánh thẳng đứng không cánh quạt](https://interestingengineering.com/transportation/us-startups-bladeless-vtol-can-reach-up-to-08-mach)

Các dòng máy bay cất cánh thẳng đứng (VTOL) truyền thống như trực thăng đều phụ thuộc vào hệ thống cánh quạt lớn để tạo lực nâng. Mới đây, một startup công nghệ tại Mỹ đã công bố thử nghiệm thành công nguyên mẫu máy bay VTOL không sử dụng cánh quạt:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011901.webp)

Cơ chế tạo lực nâng của thiết bị tương tự như nguyên lý hoạt động của các dòng quạt không cánh: nạp khí và nén áp lực cao để phun mạnh ra từ các khe hở của hai khung chữ nhật phía trên máy bay để tạo phản lực đẩy thiết bị bay lên:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011902.webp)

Do giới hạn về hiệu suất luồng khí, công nghệ này hiện mới chỉ tạo ra lực nâng đủ cho các dòng máy bay không người lái cỡ nhỏ, nhưng mở ra hướng đi mới cho thiết kế khí động học yên tĩnh trong tương lai.

## 文章

1\. [Tại sao các mô hình ngôn ngữ lớn nguồn mở thường được đặt tên theo họ lạc đà](https://sspai.com/post/79443)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051819.webp)

Bài viết thú vị giải thích nguồn gốc lịch sử đặt tên của các dòng mô hình AI nguồn mở lớn hiện nay (như LLaMA, Alpaca, Vicuna). Xu hướng này bắt nguồn từ việc Meta đặt tên cho mô hình nền tảng của họ là LLaMA (phát âm giống tên con lạc đà Llama), từ đó các nhà nghiên cứu phát triển các phiên bản tinh chỉnh sau này quyết định lấy tên của các loài động vật họ hàng nhà lạc đà để đặt tên cho sản phẩm của mình.

2\. [Nhìn lại chặng đường lịch sử của dòng tạp chí khoa học cổ viễn tưởng tại Trung Quốc](https://mp.weixin.qq.com/s/x3haEmgZF2qZ4Os4vmixjA)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052509.webp)

Bài viết hồi cứu chặng đường phát triển và sự thoái trào của dòng ấn phẩm *“Khám phá UFO”* – một trong những tạp chí khoa học phổ thông có số lượng phát hành lớn nhất cả nước vào thế kỷ trước, chỉ ra sự suy giảm sức hút của các câu chuyện giả khoa học về đĩa bay là minh chứng cho sự nâng cao dân trí và tư duy khoa học thực nghiệm của người dân.

3\. [Cảnh báo lỗ hổng lừa đảo tự động xác nhận giao dịch trên ví Alipay](https://zhuanlan.zhihu.com/p/625230704)（Tiếng Trung）

Tác giả chia sẻ câu chuyện thực tế khi mua sắm trên ứng dụng đồ cũ Xianyu và thanh toán qua Alipay đã bị đối tượng lừa đảo chiếm đoạt tiền. Kẻ lừa đảo đã lợi dụng sơ hở trong API giao dịch để viết mã lệnh tự động gửi yêu cầu xác nhận "đã nhận hàng" giả mạo lên hệ thống ngay khi người dùng vừa chuyển tiền, qua đó rút tiền ra lập tức trước khi người mua kịp phát hiện. (Đóng góp của [@childrentime](https://github.com/ruanyf/weekly/issues/3141))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052517.webp)

4\. [Chia sẻ trải nghiệm thực tế khi sử dụng hệ thống nộp đơn khởi kiện trực tuyến của tòa án](https://mp.weixin.qq.com/s/yxiKVuSSZD16id698gIvKA)（Tiếng Trung）

Tác giả ghi lại chi tiết các bước trải nghiệm gỡ lỗi giao diện đầy khó khăn khi cố gắng sử dụng hệ thống dịch vụ công nộp đơn khởi kiện dân sự trực tuyến tới tòa án giải quyết tranh chấp với ngân hàng, chỉ ra các lỗi thiết kế giao diện thiếu thân thiện khiến anh phải thực hiện lại tới 4 lần mới nộp đơn thành công. (Đóng góp của [@dingjs](https://github.com/ruanyf/weekly/issues/3138))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052518.webp)

5\. [Intel công bố đề xuất kiến trúc tập lệnh CPU x86S lược bỏ hoàn toàn chế độ 16/32-bit](https://news.mydrivers.com/1/911/911250.htm)（Tiếng Trung）

Intel chính thức công bố tài liệu kỹ thuật giới thiệu kiến trúc tập lệnh CPU thế hệ mới mang tên x86S. Kiến trúc này đề xuất lược bỏ hoàn toàn các chế độ tương thích ngược 16-bit và 32-bit cũ kỹ từ thời sơ khai của máy tính để CPU khởi động trực tiếp ở chế độ 64-bit, giúp đơn giản hóa đáng kể cấu trúc thiết kế bóng bán dẫn phần cứng.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052508.webp)

6\. [Mối lo ngại về an ninh bảo mật trước việc mở bán các đuôi tên miền `.zip`](https://www.bleepingcomputer.com/news/security/new-zip-domains-spark-debate-among-cybersecurity-experts/)（Tiếng Anh）

Việc Google chính thức mở bán các đuôi tên miền cấp cao mới như `.zip` và `.mov` đang dấy lên nhiều tranh luận trong giới bảo mật. Kẻ xấu có thể đăng ký các tên miền trùng tên với các tệp tin nén cài đặt phần mềm phổ biến (ví dụ `setup.zip`) để lừa người dùng nhấp vào liên kết tải về các phần mềm độc hại.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051901.webp)

7\. [Microsoft phát hành tính năng Mouse Without Borders điều khiển nhiều máy tính](https://learn.microsoft.com/en-us/windows/powertoys/mouse-without-borders)（Tiếng Anh）

Microsoft chính thức tích hợp tính năng "Mouse Without Borders" vào bộ công cụ PowerToys. Tiện ích này cho phép người dùng chỉ cần sử dụng một bộ chuột và bàn phím duy nhất là có thể di chuyển con trỏ và điều khiển mượt mà tối đa 4 máy tính Windows khác nhau trong cùng mạng nội bộ.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052401.webp)

8\. [Bài viết phân tích làm rõ sự khác biệt bản chất giữa ngôn ngữ C và C++](https://brycevandegrift.xyz/blog/stop-saying-c-and-c++/)（Tiếng Anh）

Tác giả chỉ ra sai lầm phổ biến khi nhiều người thường gộp chung hai ngôn ngữ này làm một và coi C++ chỉ đơn giản là tập hợp mở rộng có hướng đối tượng của C. Bài viết phân tích sâu sự khác biệt lớn về tư duy quản lý bộ nhớ và giải thuật phát triển của hai ngôn ngữ này. (Đóng góp của [@wrenashe](https://github.com/ruanyf/weekly/issues/3136))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052304.webp)

## 云原生数据仓库 ByConity 开源

Dành cho các lập trình viên quan tâm đến tối ưu hóa truy vấn dữ liệu lớn (Big Data) và công nghệ cơ sở dữ liệu:

Tuần này ghi nhận một sự kiện mã nguồn mở quan trọng: tập đoàn ByteDance (công ty mẹ của TikTok) đã chính thức **mở mã nguồn mở hoàn toàn cho hệ thống kho dữ liệu đám mây ByConity** do hãng tự nghiên cứu phát triển (Xem thêm bài viết công bố tại [ByteDance Open Source](https://mp.weixin.qq.com/s/BQvlOnzD56wacIj2HJgQpA)).

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052515.webp)

Trong các bài toán xử lý dữ liệu quy mô lớn của doanh nghiệp, việc sử dụng các cơ sở dữ liệu quan hệ thông thường rất dễ gặp nghẽn hiệu năng. Giải pháp tối ưu là chuyển sang xây dựng hệ thống kho dữ liệu (Data Warehouse) chuyên dụng.

Đội ngũ kỹ sư dữ liệu của ByteDance đã tiến hành tối ưu hóa và tái cấu trúc sâu rộng trên nền tảng của phần mềm kho dữ liệu nổi tiếng ClickHouse để xây dựng nên [ByConity](https://byconity.github.io/) phù hợp với nhu cầu xử lý lượng dữ liệu khổng lồ của tập đoàn.

Sau một thời gian vận hành phiên bản thương mại dưới tên gọi ByteHouse, ByteDance đã quyết định [mở mã nguồn mở hoàn toàn ByConity trên GitHub](https://github.com/ByConity/ByConity) để cộng đồng phát triển toàn cầu có thể tự do tải về và sử dụng.

ByConity sở hữu nhiều tính năng cao cấp như: cơ chế tách biệt hoàn toàn giữa tài nguyên đọc và ghi, khả năng mở rộng hoặc thu hẹp tài nguyên tính toán đàn hồi theo thời gian thực, cơ chế cô lập tài nguyên giữa các khách hàng (multi-tenancy) và bảo đảm tính nhất quán mạnh mẽ của dữ liệu.

Được biết ban đầu đội ngũ phát triển có ý định đóng góp các cải tiến này ngược lại cho dự án gốc ClickHouse. Tuy nhiên do số lượng dòng code thay đổi quá lớn và bổ sung thêm quá nhiều tính năng kiến trúc mới, ban quản trị ClickHouse đã đề xuất ByteDance nên tách ra thành một dự án mã nguồn mở độc lập.

Bạn đọc quan tâm có thể truy cập trang chủ [byconity.github.io](https://byconity.github.io/) để xem tài liệu hướng dẫn và tải về thử nghiệm. Đồng thời, đội ngũ phát triển dữ liệu của ByteDance tại Singapore và Trung Quốc vẫn đang tích cực tuyển dụng thêm các kỹ sư phát triển công cụ OLAP và kỹ sư kho dữ liệu, ứng viên quan tâm có thể gửi CV trực tiếp tới hòm thư nhân sự: `chenlingwei.0316@bytedance.com`.

## 工具

1、[Convoy: Hệ thống quản lý và phân phối Webhooks nguồn mở](https://github.com/frain-dev/convoy)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040108.webp)

Một giải pháp Webhooks Gateway mạnh mẽ hỗ trợ doanh nghiệp quản lý tập trung luồng gửi webhook, tích hợp sẵn các tính năng tự động gửi lại khi lỗi (retries), giới hạn tần suất gửi (rate limiting) và cơ chế ngắt mạch bảo vệ hệ thống (circuit breaking).

2、[AME Wizard: Tiện ích tùy biến cấu hình hệ điều hành Windows 11](https://ameliorated.io/)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040119.webp)

Phần mềm hỗ trợ người dùng tinh chỉnh sâu các thiết lập hệ thống của Windows 11. Người dùng có thể tải về các tệp tin cấu hình tối ưu dựng sẵn từ cộng đồng để tự động tắt các dịch vụ chạy ngầm không cần thiết và gỡ bỏ phần mềm rác chỉ với một click.

3、[RunApi: Ứng dụng quản lý và kiểm thử API đa nền tảng](https://www.showdoc.com.cn/runapi/30291)

Một ứng dụng máy tính đa nền tảng hỗ trợ lập trình viên thiết lập, quản lý tài liệu và thực hiện kiểm thử nhanh các API dịch vụ tương tự như phần mềm Postman nổi tiếng. (Đóng góp của [@star7th](https://github.com/ruanyf/weekly/issues/3128))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052302.webp)

4、[Shaku: Thư viện làm đẹp giao diện hiển thị codeblock trong Markdown](https://github.com/JSerZANP/shaku)

Công cụ hỗ trợ render các đoạn mã nguồn trong bài viết Markdown đẹp mắt, cho phép lập trình viên chèn các chú thích đặc biệt để tạo hiệu ứng highlight hoặc giải thích dòng code trực quan. (Đóng góp của [@DongHY1](https://github.com/ruanyf/weekly/issues/3133) - Xem thêm [bài viết giới thiệu chi tiết](https://jser.dev/2023-05-14-introducing-shaku/)).

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052303.webp)

5、[eslint-plugin-check-file: Plugin ESLint kiểm tra định dạng tên tệp tin](https://github.com/DukeLuo/eslint-plugin-check-file)

Tiện ích mở rộng dành cho công cụ linter ESLint, giúp tự động kiểm tra xem cấu trúc đặt tên của các file và thư mục trong dự án phần mềm có tuân thủ đúng quy tắc quy chuẩn của nhóm đề ra hay không. (Đóng góp của [@DukeLuo](https://github.com/ruanyf/weekly/issues/3132))

6、[Soft Serve: Giải pháp tự thiết lập máy chủ Git cá nhân siêu nhanh](https://github.com/charmbracelet/soft-serve)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040202.webp)

Tiện ích dòng lệnh gọn nhẹ cho phép lập trình viên nhanh chóng thiết lập một máy chủ quản lý mã nguồn Git cá nhân an toàn mà không cần cấu hình giao diện Web phức tạp, mọi thao tác quản trị được thực hiện qua giao diện SSH terminal.

7、[JShelter: Tiện ích mở rộng bảo vệ quyền riêng tư chống theo dõi dấu vân tay](https://jshelter.org/)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040403.webp)

Extension trình duyệt hỗ trợ người dùng kiểm soát và vô hiệu hóa các API Javascript chuyên dùng để thu thập dấu vân tay trình duyệt (browser fingerprinting) của các mạng lưới quảng cáo nhằm chống theo dõi hành vi lướt web.

8、[Tails: Hệ điều hành bảo mật an toàn chạy trực tiếp từ thẻ nhớ USB](https://tails.boum.org/index.en.html)

Dự án phát triển hệ điều hành Linux bảo mật cao được cấu trúc trên nền tảng Debian, tích hợp sẵn cơ chế mã hóa định tuyến toàn bộ lưu lượng mạng qua mạng ẩn danh Tor giúp người dùng bảo vệ danh tính tuyệt đối khi lướt web:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010701.webp)

9、[Just: Tiện ích hỗ trợ quản lý lệnh chạy dự án viết bằng Rust](https://just.systems/)

Công cụ chạy lệnh dự án tương tự như Make viết bằng Rust nhưng tập trung tối giản hóa cú pháp, hỗ trợ lập trình viên lưu trữ và chạy nhanh toàn bộ các lệnh terminal thường dùng của dự án trên mọi hệ điều hành.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011002.webp)

10、[Dora.ai: Công cụ AI hỗ trợ tự động thiết kế trang web 3D tương tác](https://www.dora.run/)

Ứng dụng web tích hợp trí tuệ nhân tạo thế hệ mới: người dùng chỉ cần nhập mô tả giao diện bằng văn bản, AI sẽ tự động thiết kế và sinh ra trang web có giao diện hoạt họa 3D tương tác bắt mắt. Hiện dự án đang mở đăng ký trải nghiệm phiên bản thử nghiệm Alpha và ghi nhận lượt bình chọn dẫn đầu trên Product Hunt. (Đóng góp của [@CharlesLiuyx](https://github.com/ruanyf/weekly/issues/3144))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052521.webp)

## 稀土开发者大会

Nhiều lập trình viên thường hỏi tôi làm thế nào để mở rộng các mối quan hệ chuyên môn trong ngành?

Nếu bạn kiên trì xây dựng và đóng góp cho một dự án mã nguồn mở hoặc duy trì viết blog chia sẻ kiến thức công nghệ trong nhiều năm, bạn tự khắc sẽ quen biết được rất nhiều đồng nghiệp cùng chí hướng.

Ngoài ra, một phương pháp nhanh chóng và hiệu quả hơn là **tích cực tham gia các hội thảo công nghệ ngoại tuyến (offline)**. Tại đây, bạn có cơ hội trực tiếp lắng nghe các chuyên gia chia sẻ về dự án của họ, giới thiệu về sản phẩm của bản thân và dễ dàng kết nối kết bạn. Rất nhiều nhà sáng lập startup công nghệ đã tìm kiếm được các cộng sự ăn ý của mình từ chính các buổi giao lưu bên lề các hội thảo này.

Hôm nay, tuần báo xin vui mừng thông báo **Bản tin của chúng ta vinh dự được lựa chọn làm đối tác truyền thông đồng hành cùng sự kiện "Hội thảo nhà phát triển Xitu 2023"** diễn ra vào ngày 30 tháng 6 đến ngày 1 tháng 7 tới đây tại Bắc Kinh.

Sự kiện do cộng đồng công nghệ lớn Juejin tổ chức, quy tụ hàng chục diễn giả đến từ các tập đoàn lớn chia sẻ về các xu hướng công nghệ nóng nhất hiện nay (như AI, Cloud Native, Frontend).

Ban tổ chức đang mở bán các hạng vé tham dự với mức giá cực kỳ ưu đãi dành cho học sinh, sinh viên chỉ **99 nhân dân tệ** cho trọn vẹn 2 ngày tham gia hội thảo.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052507.webp)

Đối với các doanh nghiệp mua vé cho kỹ sư tham dự, hãy sử dụng mã giảm giá độc quyền **“ruanyifeng”** khi đặt mua trên trang chủ để được áp dụng mức giá ưu đãi 799 nhân dân tệ cho hạng vé VIP (bao gồm suất ăn trưa tại khách sạn).

Sự kiện sẽ được tổ chức tại Khách sạn Crowne Plaza Sun Palace, Bắc Kinh. Do số lượng ghế ngồi tại hội trường có giới hạn, bạn đọc quan tâm nên truy cập [Trang chủ sự kiện Xitu 2023](https://conf.juejin.cn/xdc2023/?utm_source=0525rrydrz) hoặc quét mã QR phía trên để xem lịch trình chi tiết và đăng ký mua vé sớm.

## 资源

1\. [LangChain & LlamaIndex Book: Tài liệu tự học lập trình kết nối các mô hình AI](https://leanpub.com/langchain/read)

Cuốn sách điện tử viết bằng tiếng Anh cung cấp tài liệu hướng dẫn thực hành chi tiết cách sử dụng hai thư viện nguồn mở thiết yếu là LangChain và LlamaIndex để xây dựng các ứng dụng AI kết nối dữ liệu riêng tư, cho phép đọc trực tuyến miễn phí.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052002.webp)

2、[Bing Wallpaper Database: Cơ sở dữ liệu lưu trữ hình ảnh màn hình khóa của Bing](https://github.com/mouday/wallpaper-database)

Mã nguồn mở hỗ trợ thu thập và lưu trữ toàn bộ các bức ảnh phong cảnh tuyệt đẹp được Microsoft sử dụng làm màn hình khóa hàng ngày trên công cụ tìm kiếm Bing. (Đóng góp của [@mouday](https://github.com/ruanyf/weekly/issues/3126))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052301.webp)

3、[Reinforcement Learning 100: Bộ bài tập 100 câu hỏi tự học học máy tăng cường](https://p100.koki-saitoh.com/zh-CN)

Bản dịch tiếng Trung của bộ bài tập trắc nghiệm và thực hành lập trình 100 câu hỏi chuyên sâu về mảng Học máy tăng cường (Reinforcement Learning) do tác giả sách công nghệ nổi tiếng người Nhật Koki Saitoh biên soạn giúp người học củng cố kiến thức. (Đóng góp của [@RiverTwilight](https://github.com/ruanyf/weekly/issues/3143))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052519.webp)

4、[supes.top: Tiện ích hỗ trợ tự build firmware OpenWrt tùy biến cho router](https://supes.top/)

Một dịch vụ web trực quan hỗ trợ người dùng tự lựa chọn các gói thư viện tính năng mong muốn để hệ thống tự động biên dịch thành tệp tin firmware hệ điều hành OpenWrt tùy biến tương thích riêng với cấu hình phần cứng router của mình.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041908.webp)

## 图片

1、**Trào lưu tạo các video giả lập lịch sử bằng công nghệ AI trên TikTok**

Gần đây trên mạng xã hội TikTok xuất hiện trào lưu sáng tạo nội dung độc đáo: sử dụng hình ảnh AI phác họa lại các kịch bản lịch sử giả tưởng thu hút lượng người xem lớn. Ví dụ như chủ đề giả định *"Nếu Ấn Độ đô hộ nước Anh"* được AI vẽ ra cảnh tượng cảnh sát London cưỡi lạc đà đi tuần tra trên đường phố:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052206.webp)

Các kịch bản giả tưởng thú vị khác bao gồm *"Nếu Mexico giành chiến thắng trong cuộc chiến với Mỹ năm 1848"* hay *"Nếu đế quốc Inca tiếp tục tồn tại và phát triển đến ngày nay"*:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052207.webp)

2、**Bộ sưu tập các mô hình bản đồ địa hình in nổi bằng công nghệ 3D**

Một người đam mê công nghệ in 3D đã sử dụng dữ liệu độ cao vệ tinh để in thành các mô hình bản đồ địa hình dạng 3D nổi trực quan của các quốc gia và bang trên thế giới:

* Bản đồ địa hình nước Thái Lan:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030907.webp)

* Bản đồ địa hình bang California, Mỹ:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030908.webp)

* Bản đồ địa hình nước Tây Ban Nha:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030909.webp)

## ✍️ Bài đọc thêm

### Tìm hiểu về nghịch lý tam đề Munchhausen trong triết học nhận thức

Các nhà triết học Đức đã từng đưa ra một luận điểm gây tranh cãi: **Mọi mệnh đề khoa học được chứng minh hoàn toàn bằng các phương pháp toán học và logic học thuần túy đều không thể coi là chân lý tuyệt đối.**

Hay nói cách khác, một chân lý tuyệt đối không bao giờ có thể được chứng minh chỉ bằng công cụ toán học và logic.

Cơ sở của lập luận này chỉ ra rằng để chứng minh một mệnh đề A là đúng, chúng ta bắt buộc phải dựa vào một tiền đề B làm căn cứ. Tuy nhiên để chứng minh tiền đề B đó là đúng, chúng ta lại cần một tiền đề C khác. Quá trình này suy ra chỉ có 3 kịch bản xảy ra:

1. **Lập luận vòng quanh (Circular reasoning)**: Mệnh đề A dùng tiền đề B để chứng minh, nhưng tiền đề B thực chất lại được chứng minh ngược lại từ mệnh đề A.
2. **Suy luận vô hạn (Infinite regress)**: Quá trình đi tìm tiền đề chứng minh kéo dài mãi mãi không có điểm dừng.
3. **Dừng lập luận tiên đề (Dogmatic interruption)**: Quá trình chứng minh được chủ động dừng lại ở một tiền đề cơ bản được số đông công nhận là hiển nhiên đúng (các tiên đề toán học) mà không cần chứng minh thêm.

Cả ba kịch bản trên đều chứa đựng những thiếu sót về mặt logic học chặt chẽ, và nghịch lý này được gọi là **“Tam đề Munchhausen”** (Munchhausen Trilemma).

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052520.webp)

*Tên gọi lấy cảm hứng từ nhân vật nam tước Munchhausen giả tưởng trong truyện dân gian Đức, người tuyên bố có khả năng tự túm tóc của chính mình để kéo cả người và ngựa thoát khỏi đầm lầy, thường được ví cho các hành động bất khả thi.*

Nghịch lý này chỉ ra giới hạn của toán học và logic: chúng không thể tự đứng độc lập mà bắt buộc phải được xây dựng trên nền tảng của một số tiên đề mặc định được thừa nhận mà không thể chứng minh bằng thực nghiệm.

## Lịch sử tuần này

- 2022年（第 209 期）：[职业生涯: Phân tích thực tế lập trình viên là nhóm người có đặc điểm tính cách như thế nào](http://www.ruanyifeng.com/blog/2022/06/weekly-issue-209.html)
- 2021年（第 159 期）：[Ngành công nghiệp: Khảo sát mức thu nhập bình quân của các nhà phát triển trò chơi](http://www.ruanyifeng.com/blog/2021/05/weekly-issue-159.html)
- 2020年（第 109 期）：[Truyền thông số: Thảo luận về các giá trị thương mại của loại hình phát sóng podcast](http://www.ruanyifeng.com/blog/2020/05/weekly-issue-109.html)
- 2019年（第 59 期）：[Xã hội số: Tại sao việc tìm kiếm và kết bạn trong thời đại Internet lại ngày càng khó khăn](http://www.ruanyifeng.com/blog/2019/06/weekly-issue-59.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs is an amazing workspace platform.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
