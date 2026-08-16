# Bản tin chia sẻ công nghệ (Số 282): Hệ thống điện 48V trên xe bán tải Cybertruck

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3684) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120511.webp)

Ga tàu điện ngầm Dự Viên trên Tuyến số 14 ở Thượng Hải, nằm ngay bên cạnh sông Hoàng Phố. Thiết kế mái vòm sử dụng hàng chục nghìn tấm nhôm, mô phỏng những vòng sóng nước lăn tăn cùng mái hiên cong truyền thống của Dự Viên, kết hợp với ánh sáng để tạo nên một bầu trời nghệ thuật rực rỡ. (Nguồn: [Archiposition](https://www.archiposition.com/items/20220224043158))

## 电动皮卡 Cybertruck 的 48V 供电

Trong tháng này, dòng xe bán tải điện Cybertruck của Tesla đã chính thức bắt đầu được bàn giao đến tay khách hàng tại Mỹ.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120808.webp)

Đây là một chiếc xe bán tải có kiểu dáng vô cùng độc lạ, thùng xe phía sau có một tấm chắn bảo vệ có thể mở ra để chất hàng hóa.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120809.webp)

Dòng xe này đã thiết lập rất nhiều cột mốc đầu tiên trên thế giới:

> 1. Chiếc xe thương mại đầu tiên trên thế giới sử dụng thân vỏ thép không gỉ.
> 2. Lớp vỏ thép được giới thiệu là có khả năng chống đạn, và với thiết kế góc cạnh sắc nhọn, bất kỳ chiếc xe thông thường nào va chạm với nó sẽ gặp tổn thất vô cùng lớn.
> 3. Là chiếc bán tải nặng nhất với trọng lượng tự thân lên tới 3,5 tons, khi chở thêm hành khách và hàng hóa có thể vượt quá 4 tons, gấp đôi trọng lượng của các dòng xe bán tải thông thường.

Tuy nhiên, có một cột mốc đầu tiên trên thế giới cực kỳ quan trọng nhưng lại rất ít người nhắc đến: **Đây là chiếc xe đầu tiên trên thế giới chuyển đổi hoàn toàn hệ thống điện cabin sang điện áp 48V**.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120810.webp)

Như chúng ta đã biết, bên trong một chiếc xe hơi có rất nhiều thiết bị điện tử tiêu thụ năng lượng như cửa sổ điện, điều hòa, hệ thống đèn chiếu sáng, tẩu sạc... Tất cả các thiết bị này đều phụ thuộc vào nguồn điện áp cabin.

Trước đây, thời đại xe chạy xăng truyền thống vốn không có quá nhiều thiết bị điện tử phức tạp, công suất yêu cầu thấp nên điện áp cabin được thiết lập ở mức khá thấp. Ban đầu là dòng điện một chiều 6V, sau đó nâng lên chuẩn 12V.

Hiện nay, hầu như tất cả các xe thương mại trên thị trường đều sử dụng hệ thống điện cabin 12V. Tương ứng, các thiết bị điện tử phụ trợ trong xe cũng được thiết kế để tương thích với mức điện áp 12V này.

Cybertruck là chiếc xe thương mại đầu tiên trên thế giới loại bỏ hoàn toàn hệ thống điện 12V truyền thống và chuyển sang sử dụng điện áp 48V. Điều này đồng nghĩa với việc toàn bộ linh kiện điện tử phụ trợ trên chiếc xe này đều phải được đặt hàng thiết kế riêng biệt.

Tại sao Cybertruck lại quyết định từ bỏ tiêu chuẩn 12V?

Lý do rất đơn giản: lượng điện năng tiêu thụ của nó quá lớn, mức điện áp 12V sẽ khiến hệ thống dây dẫn bên trong quá tải nghiêm trọng.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120811.webp)

Một số báo cáo kỹ thuật tiết lộ rằng, chỉ riêng chiếc cần gạt nước khổng lồ dài tới 1,2 mét của Cybertruck (hình trên) đã yêu cầu công suất khởi động lên tới 3600W. Nếu chạy ở mức điện áp 12V, cường độ dòng điện sẽ lên tới 300A, đòi hỏi hệ thống dây dẫn phải có đường kính cực kỳ lớn.

**Sau khi nâng lên chuẩn 48V, điện áp tăng lên 4 lần, cường độ dòng điện yêu cầu sẽ giảm xuống chỉ còn 1/4 so với trước đây**.

Nhu cầu công suất điện cabin ngày càng lớn không chỉ là bài toán riêng của Cybertruck, mà tất cả các hãng xe điện hiện nay đều đang đối mặt. Tiêu chuẩn điện áp 12V từ lâu đã trở thành rào cản hạn chế sự phát triển của công nghệ ô tô.

Việc chuyển đổi sang hệ thống điện 48V mang lại rất nhiều lợi ích kỹ thuật vượt trội:

(1) Cường độ dòng điện giảm xuống còn 1/4 giúp giảm đường kính dây dẫn đi rất nhiều, tiết kiệm lượng lớn kim loại đồng sử dụng, từ đó tối ưu hóa chi phí sản xuất đồng thời giảm đáng kể trọng lượng của toàn bộ chiếc xe.

(2) Dòng điện nhỏ hơn cũng giúp giảm lượng nhiệt tỏa ra trên đường truyền, giảm thiểu đáng kể hao phí năng lượng.

(3) Điện áp 48V đạt chuẩn tương thích với công nghệ cấp nguồn qua dây mạng Power over Ethernet (PoE), cho phép truyền tải cả dữ liệu và nguồn điện trên cùng một sợi cáp mạng đến một số thiết bị. Hơn nữa, việc sử dụng cáp mạng Ethernet mang lại tốc độ truyền dữ liệu cao và tín hiệu ổn định hơn hẳn so với hệ thống dây xoắn đôi truyền thống.

Tất nhiên, tiêu chuẩn 48V cũng có những nhược điểm riêng, lớn nhất là chuỗi cung ứng linh kiện phụ trợ tương thích còn rất hạn chế và giá thành cao. Bên cạnh đó, toàn bộ kiến trúc điện của chiếc xe bắt buộc phải được thiết kế lại từ đầu.

Một điểm đáng mừng là Tesla đã công khai toàn bộ tài liệu thiết kế kiến trúc điện 48V của Cybertruck và [chủ động gửi tặng cho các hãng xe đối thủ](https://electrek.co/2023/12/07/tesla-shares-48v-architecture-with-other-automakers-to-move-the-industry/). CEO của Ford Motor đã đăng trên X rằng ông rất bất ngờ khi thực sự nhận được tập tài liệu bản vẽ kỹ thuật chi tiết từ phía Tesla, và Elon Musk đã phản hồi thân thiện: "Không có chi" (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121203.webp)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121204.webp)

Hệ thống điện 48V chắc chắn là xu thế tất yếu của tương lai. Hy vọng các doanh nghiệp sản xuất ô tô và linh kiện phụ tùng trong nước sẽ nhanh chóng bắt kịp xu hướng để nâng cấp hệ thống điện áp cabin trên các dòng xe thế hệ mới.

## [活动] 人工智能线下沙龙（深圳站）

Trí tuệ nhân tạo (AI) hiện đang là tâm điểm chú ý của toàn ngành công nghệ, đồng thời cũng là lĩnh vực thu hút dòng vốn đầu tư và nhu cầu tuyển dụng lớn nhất.

Cộng đồng Juejin (掘金), một trong những cộng đồng nhà phát triển nổi tiếng tại Trung Quốc, sẽ **tổ chức một buổi giao lưu trực tiếp (offline) tại Thâm Quyến vào Chủ Nhật tuần này**, nhằm tạo cơ hội cho mọi người cùng gặp gỡ, giao lưu và thảo luận sâu về chủ đề AI.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121309.webp)

Chủ đề của sự kiện lần này là **《Khám phá công nghệ mô hình lớn và đổi mới ứng dụng AIGC》**. Ban tổ chức đã mời 4 chuyên gia kỹ thuật hàng đầu từ Alibaba, NVIDIA... đến chia sẻ về các chủ đề chuyên sâu như tối ưu hóa Transformer và các giải pháp thực tế để ứng dụng mô hình AIGC vào hoạt động kinh doanh thực tế.

Thông tin chi tiết về sự kiện và đăng ký tham dự miễn phí, quý độc giả có thể truy cập tại [trang chủ chính thức của sự kiện](https://www.bagevent.com/event/8756156?bag_track=ruanyifeng) hoặc quét mã QR ở hình trên.

Các bạn quan tâm khu vực lân cận Thâm Quyến nếu có thời gian rảnh vào chiều Chủ Nhật này (17/12) có thể đến tham gia giao lưu tại văn phòng ByteDance ở khu vực vịnh Thâm Quyến. Bên cạnh việc tương tác trực tiếp với các chuyên gia, sự kiện còn có tiệc trà nhẹ và nhiều phần quà tặng lưu niệm như sổ tay, huy hiệu và sticker cho người tham gia.

## 科技动态

1、[Bảo tàng nghệ thuật dành riêng cho người khiếm thị](https://www.thrillist.com/travel/nation/envision-arts-gallery-wichita-kansas)

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023063004.webp)

Làm thế nào để người khiếm thị có thể trải nghiệm nghệ thuật tại bảo tàng? Một bảo tàng nghệ thuật đặc biệt dành riêng cho người khiếm thị vừa được khai trương tại bang Kansas, Mỹ.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023063005.webp)

Tất cả tác phẩm nghệ thuật trưng bày tại đây đều cho phép khách tham quan chạm trực tiếp bằng tay. Để giúp người khiếm thị dễ dàng hình dung cấu trúc, các tác phẩm đều được thiết kế lại với bề mặt in nổi rõ nét.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023063006.webp)

Bản thuyết minh thông tin tác phẩm cũng được viết bằng chữ nổi Braille. Ngoài ra, khách tham quan sẽ được trang bị một thiết bị thuyết minh tự động phát tiếng giới thiệu khi họ đứng trước mỗi tác phẩm.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023063007.webp)

2、[Chiếc Tesla chạy nhiều km nhất thế giới](https://insideevs.com/news/699413/highest-mileage-tesla-model-s-3-batteries-14-motors/)

Chiếc xe Tesla ghi nhận quãng đường di chuyển lớn nhất thế giới hiện nay là một chiếc Model S P85 phiên bản năm 2014.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120702.webp)

Chiếc xe đã hoàn thành tổng quãng đường di chuyển lên tới 1,9 triệu km, tương đương trung bình 210.000 km mỗi năm. Điều này đồng nghĩa với việc dù không nghỉ ngày nào, chiếc xe này vẫn phải duy trì chạy ít nhất 577 km mỗi ngày trong suốt nhiều năm qua.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120703.webp)

Lý do cụ thể vì sao chiếc xe lại di chuyển nhiều đến vậy vẫn chưa được tiết lộ chi tiết. Chủ nhân của chiếc xe chỉ chia sẻ rằng anh đã sử dụng nó để thực hiện rất nhiều chuyến hành trình dài ra nước ngoài, đi qua các nước châu Phi, Morocco, Thụy Điển, Áo và cả Trung Quốc.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120704.webp)

Việc một chiếc xe thuần điện có thể duy trì hoạt động bền bỉ qua quãng đường kỷ lục như vậy là điều vô cùng đáng nể. Tất nhiên, các bộ phận cốt lõi của xe đã được thay thế nhiều lần trong quá trình sử dụng, bao gồm 13 lần thay động cơ và 3 lần thay thế cụm pin.

3、[Ý tưởng sản xuất điện từ chuyển động lắc lư của tàu biển](https://newatlas.com/marine/heave-oscillators-wave-energy-ship/)

Nhiều người có lẽ đã quen thuộc với khái niệm "Điện sóng biển" - đặt các máy phát điện dưới biển để tận dụng cơ năng từ sóng vỗ tạo ra điện.

Một viện nghiên cứu tại Thượng Hải đã đưa ra ý tưởng: bản thân các con tàu khi di chuyển trên biển cũng liên tục bị lắc lư do sóng vỗ, vậy tại sao không tận dụng ngay chuyển động này để biến con tàu thành một máy phát điện.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120708.webp)

Thiết kế đề xuất đặt một bộ dao động ba trục kết nối với một xi-lanh thủy lực và lò xo ở dưới đáy khoang tàu.

Khi thân tàu lắc lư, bộ dao động sẽ rung động theo ba hướng khác nhau, từ đó truyền lực tác động lên xi-lanh thủy lực để nén/kéo lò xo và tạo ra dòng điện.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120709.webp)

Tuy nhiên, nhóm nghiên cứu vẫn chưa đưa ra tính toán cụ thể về lượng điện năng thực tế có thể thu hồi được. Xem xét việc các tàu biển luôn chủ động lựa chọn những tuyến đường biển lặng sóng để di chuyển an toàn, ý tưởng thiết kế này dù có thể chế tạo thành công thì sản lượng điện tạo ra trên thực tế có lẽ cũng rất nhỏ bé.

4、[Mỹ phê duyệt liệu pháp chỉnh sửa gen đầu tiên trong y học](https://finance.sina.com.cn/stock/usstock/c/2023-12-09/doc-imzxkvky9798727.shtml)

Vào ngày 8 tháng 12, Mỹ đã chính thức phê duyệt liệu pháp chỉnh sửa gen đầu tiên để điều trị bệnh hồng cầu hình liềm (hình dưới, do lỗi đột biến gen, các tế bào máu của người bệnh không có hình tròn bình thường mà bị biến dạng thành hình lưỡi liềm).

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121006.webp)

Sự kiện này đánh dấu cột mốc quan trọng khi công nghệ chỉnh sửa gen nổi tiếng CRISPR chính thức được ứng dụng điều trị lâm sàng sau 10 năm phát minh.

Liệu pháp tiến hành tách toàn bộ tế bào gốc tạo máu của người bệnh, thực hiện chỉnh sửa gen để loại bỏ đoạn gen lỗi và sau đó truyền ngược lại tế bào sạch vào cơ thể.

Do đặc thù quy trình phức tạp, liệu pháp chỉnh sửa gen hiện tại chủ yếu chỉ áp dụng hiệu quả cho các bệnh về máu, bởi các cơ quan nội tạng khác rất khó thực hiện chỉnh sửa chi tiết từng tế bào trừ khi được can thiệp từ giai đoạn phôi thai.

Hơn nữa, chi phí điều trị của liệu pháp này cực kỳ đắt đỏ, với mức giá thấp nhất lên tới 2,2 triệu USD (khoảng hơn 50 tỷ đồng), vượt xa khả năng chi trả của đại đa số bệnh nhân thông thường.

## Bài viết

1\. [Tổng kết các tính năng mới nổi bật của CSS trong năm 2023](https://developer.chrome.com/blog/css-wrapped-2023?hl=zh-cn)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121202.webp)

Bài tổng hợp chi tiết từ đội ngũ phát triển trình duyệt Chrome giới thiệu những tính năng và thuộc tính CSS mới được bổ sung trong năm 2023.

2\. [Câu chuyện trải nghiệm làm việc tại tập đoàn Alibaba của một lập trình viên người Việt](https://corecursive.com/software-world-tour-with-son-luong-ngoc/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120705.webp)

Tác giả là một kỹ sư phần mềm người Việt Nam, trước đây làm việc tại Lazada. Sau khi Alibaba mua lại Lazada, anh đã chuyển sang làm việc tại văn phòng Alibaba ở Tây Khê, Hàng Châu một thời gian.

Hiện tại anh đã chuyển sang đầu quân cho Booking.com, bài viết là những chia sẻ thú vị của anh về hành trình sự nghiệp cá nhân và những cảm nhận thực tế khi làm việc trong môi trường tập đoàn lớn của Trung Quốc.

3\. [Ký sự ghé thăm văn phòng lưu trữ vật lý của Internet Archive](https://thenewstack.io/a-visit-to-the-physical-internet-archive/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023103001.webp)

Internet Archive là một dự án phi lợi nhuận tuyệt vời với mục tiêu sao lưu và lưu trữ bản chụp của **tất cả các trang web** trên thế giới để người dùng toàn cầu có thể truy cập tra cứu hoàn toàn miễn phí.

Trụ sở chính của tổ chức tại bang California hiện đã mở cửa bán vé cho khách tham quan. Tác giả đã chia sẻ trải nghiệm thực tế chuyến ghé thăm văn phòng của mình và may mắn được trực tiếp nhà sáng lập dự án dẫn đi giới thiệu.

4\. [Hướng dẫn sử dụng công cụ Fail2ban để bảo vệ cổng SSH trên Linux](https://linuxiac.com/how-to-protect-ssh-with-fail2ban/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110106.webp)

Tài liệu hướng dẫn cơ bản cho người mới bắt đầu cách cấu hình Fail2ban trên hệ điều hành Linux để ngăn chặn các cuộc tấn công dò mật khẩu (brute-force) vào cổng kết nối SSH.

5\. [Web Components hứa hẹn sẽ có tuổi thọ lâu bền hơn các JavaScript Frameworks](https://jakelazaroff.com/words/web-components-will-outlive-your-javascript-framework/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110208.webp)

Tác giả phân tích lý do khi cần thiết kế một hiệu ứng giao diện trang web, anh đã lựa chọn giải pháp Web Components tiêu chuẩn để đảm bảo khả năng tương thích lâu dài và độc lập, thay vì phụ thuộc vào một JS framework cụ thể vốn có thể bị lỗi thời nhanh chóng.

6\. [Cách cấu hình HTTP Cache Headers tối ưu cho các tài nguyên tĩnh](https://www.macarthur.me/posts/more-aggressive-cache-headers/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092108.webp)

Các tài nguyên tĩnh (như file hình ảnh, CSS, JS) của website thường rất ít khi thay đổi. Bài viết hướng dẫn chi tiết cách cấu hình tham số HTTP cache headers tối ưu nhất giúp giảm tải cho server và tăng tốc độ tải trang.

7\. [Hướng dẫn chuyển đổi tệp tin âm thanh định dạng MP3 sang chuẩn mới Opus](https://www.worthe-it.co.za/blog/2023-08-20-building-a-digital-music-collection-in-2023.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082108.webp)

Opus là chuẩn mã hóa âm thanh thế hệ mới mang lại chất lượng âm thanh sắc nét vượt trội so với MP3 truyền thống, đồng thời tối ưu hóa dung lượng tệp tin nén nhỏ hơn đáng kể.

8\. [Mẹo thiết lập giảm độ sáng màn hình điện thoại vượt mức giới hạn mặc định](https://practicalbetterments.com/create-a-shortcut-for-even-lower-phone-brightness/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110713.webp)

Trong môi trường đêm tối, đôi khi dù đã điều chỉnh độ sáng màn hình về mức tối thiểu mặc định, điện thoại của bạn trông vẫn rất chói mắt. Bài viết hướng dẫn mẹo cấu hình trên điện thoại iPhone và Android để giảm độ sáng màn hình xuống mức cực tối.

9\. [Ứng dụng mô hình ngôn ngữ lớn GPT-3 để bóc tách và chuẩn hóa dữ liệu phi cấu trúc](https://marcotm.com/articles/information-extraction-with-large-language-models-parsing-unstructured-data-with-gpt/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092401.webp)

Tác giả trình bày ví dụ thực tế cách viết prompt hướng dẫn mô hình GPT-3 tự động phân tích các nội dung tin tuyển dụng viết dạng văn bản tự do để bóc tách thành dữ liệu định dạng JSON chuẩn hóa.

## 工具

1、[Imagine](https://imagine.meta.com/)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120803.webp)

Công cụ tạo ảnh từ văn bản do tập đoàn Meta ra mắt, được huấn luyện dựa trên kho dữ liệu khổng lồ gồm 1,1 tỷ bức ảnh từ Facebook và Instagram, hiện mở cửa cho người dùng trải nghiệm miễn phí.

2、[NotebookLM](https://notebooklm.google.com/)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120902.webp)

Ứng dụng ghi chú thông minh tích hợp AI do Google phát triển. Người dùng có thể tải lên các tài liệu học tập nghiên cứu cá nhân để AI hỗ trợ trả lời câu hỏi và tự động tóm tắt nội dung ghi chú. Hiện tại dịch vụ đang mở cửa miễn phí cho người dùng khu vực Mỹ. Xem thêm bài viết giới thiệu của [Google](https://blog.google/technology/ai/notebooklm-new-features-availability/).

Lưu ý hiện tại ứng dụng chủ yếu hỗ trợ tốt định dạng tệp PDF viết bằng tiếng Anh.

3、[Scalar API Reference](https://github.com/scalar/scalar)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101616.webp)

Dự án mã nguồn mở hỗ trợ tự động chuyển đổi các tài liệu đặc tả Swagger/OpenAPI thành giao diện tài liệu hướng dẫn API tương tác trực quan.

4、[RoomGPT](https://github.com/Nutlope/roomGPT)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101701.webp)

Dự án mã nguồn mở hỗ trợ người dùng thiết kế lại nội dung phòng ốc bằng AI: Bạn chỉ cần tải lên một bức ảnh chụp căn phòng thực tế, hệ thống sẽ tự động vẽ ra các phương án bài trí nội thất mới.

5、[Comments](https://github.com/DongHY1/comments)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121403.webp)

Hệ thống bình luận trang web mã nguồn mở cho phép người dùng bôi đen và kéo khung để để lại phản hồi trực tiếp trên từng vùng nội dung cụ thể của trang web. Dự án tích hợp hệ thống xác thực tài khoản GitHub và lưu trữ cơ sở dữ liệu trên Supabase. (Đóng góp của [@DongHY1](https://github.com/ruanyf/weekly/issues/3743))

6、[GPT Assistant](https://github.com/ruanyf/weekly/issues/3725)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120802.webp)

Ứng dụng Android mã nguồn mở kết nối với GPT hỗ trợ tính năng trò chuyện bằng giọng nói, gửi ảnh phân tích qua mô hình GPT-4V và tích hợp Android WebView giúp AI có thể truy cập đọc thông tin từ các liên kết trang web bên ngoài. (Đóng góp của [@Skythinker616](https://github.com/ruanyf/weekly/issues/3725))

7、[MD Video](https://www.wvovw.com/guide/what-is-wvovw.html)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121301.webp)

Ứng dụng máy tính hỗ trợ tự động chuyển đổi các nội dung ghi chép định dạng Markdown thành các đoạn video ngắn. (Đóng góp của [@lqomg](https://github.com/ruanyf/weekly/issues/3736))

8、[CodeGeeX2](https://github.com/THUDM/CodeGeeX2)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121302.webp)

Trợ lý viết code bằng AI hỗ trợ tích hợp mượt mà dưới dạng extension trên các trình biên dịch phổ biến như VS Code, IntelliJ IDEA, PyCharm, GoLand, WebStorm. Xem thêm [bài viết giới thiệu chi tiết](https://github.com/CatsAndMice/blog/issues/72). (Đóng góp của [@CatsAndMice](https://github.com/ruanyf/weekly/issues/3731))

9、[bproxy](https://github.com/zobor/bproxy)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121004.webp)

Công cụ bắt gói tin (packet capture proxy) gọn nhẹ hỗ trợ can thiệp các yêu cầu HTTP, toàn bộ file cấu hình hoạt động của công cụ được viết bằng cú pháp JavaScript. (Đóng góp của [@zobor](https://github.com/ruanyf/weekly/issues/3728))

10、[Trippy](https://trippy.cli.rs/)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121005.webp)

Công cụ dòng lệnh hiệu năng cao thay thế cho traceroute truyền thống, hỗ trợ hiển thị trực quan lộ trình truyền tải gói tin trên không gian mạng giúp kỹ sư phân tích nhanh sự cố kết nối mạng.

## 资源

1、[Tuyển tập các dòng lệnh Terminal hữu ích trên macOS](https://git.herrbischoff.com/awesome-macos-command-line/about/)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120801.webp)

Trang web tổng hợp và phân loại rất nhiều dòng lệnh terminal hữu dụng dành riêng cho hệ điều hành macOS.

2、[Sách giáo trình Nhập môn Thống kê Hiện đại](https://openintro-ims2.netlify.app/)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101403.webp)

Cuốn sách giáo khoa cơ bản giới thiệu các kiến thức nền tảng về ngành khoa học thống kê dành cho sinh viên đại học năm nhất, mở cửa đọc trực tuyến miễn phí.

3、[Khóa học tự học ngôn ngữ lập trình Python trong 30 ngày](https://github.com/Asabeneh/30-Days-Of-Python)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101618.webp)

Kho lưu trữ mã nguồn cung cấp lộ trình bài giảng và bài tập thực hành Python cơ bản được thiết kế học gọn gàng trong vòng 30 ngày đi kèm video hướng dẫn.

4、[Tổng hợp các tựa game chạy trên trình duyệt web có đồ họa đẹp nhất](https://news.ycombinator.com/item?id=37931804)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101902.webp)

Một chủ đề thảo luận sôi nổi trên diễn đàn Hacker News, nơi các lập trình viên cùng chia sẻ danh sách các tựa game chạy trực tiếp trên trình duyệt sở hữu thiết kế đồ họa nghệ thuật xuất sắc nhất. Ảnh minh họa phía trên được chụp từ tựa game [Short Trip (Chuyến đi ngắn ngày)](https://alexanderperrin.com.au/paper/shorttrip/).

## 图片

1、[Tài liệu hình ảnh lịch sử về lớp tàu ngầm hạt nhân Typhoon khổng lồ của Liên Xô](https://imgur.com/a/xi3P3)

Lớp tàu ngầm hạt nhân chiến lược Typhoon (Dự án 941 Akula) được chế tạo từ những năm 1980, hiện vẫn giữ kỷ lục là lớp tàu ngầm có kích thước lớn nhất từng được chế tạo trong lịch sử nhân loại.

Liên kết bài viết cung cấp bộ sưu tập gồm hơn 100 bức ảnh tư liệu lịch sử chi tiết ghi lại quá trình vận hành của gã khổng lồ biển sâu này.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071305.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071306.webp)

Liên Xô đã hoàn thành chế tạo tổng cộng 6 tàu ngầm thuộc lớp này. Do chi phí vận hành và bảo dưỡng quá đắt đỏ vượt quá khả năng duy trì, hiện nay toàn bộ các tàu ngầm lớp Typhoon đều đã chính thức được cho nghỉ hưu.

2、[Những chiếc tổ chim độc đáo làm từ gai kim loại chống chim](https://www.naturalis.nl/en/about-us/media/press-releases/rebellious-birds-make-nests-out-of-anti-bird-pins)

Các nhà nghiên cứu tại Hà Lan đã công bố một phát hiện thú vị: Nhiều loài chim sống tại đô thị đã chủ động nhổ các thanh gai kim loại chống chim đậu được lắp trên các tòa nhà cao tầng để mang về làm vật liệu xây dựng tổ.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071311.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071702.webp)

Hiện tại giới khoa học vẫn chưa đưa ra lời giải thích chính xác liệu loài chim thực sự ưa thích kết cấu tổ kim loại vững chắc này hay đơn giản vì đây là nguồn vật liệu dễ tìm kiếm nhất trong môi trường đô thị hiện đại.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071703.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071704.webp)

## ✍️ Bài đọc thêm

### Chia sẻ trải nghiệm thực tế với dự án khởi nghiệp Web3 blockchain

Vào năm 2022, tôi đã may mắn nhận được tấm vé tài trợ để một mình bay sang thủ đô Lisbon của Bồ Đào Nha tham dự hội nghị công nghệ NearCon 2022.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121404.webp)

Đây là một sự kiện hội nghị kết hợp cuộc thi hackathon về mảng công nghệ blockchain kéo dài liên tục trong 4 ngày. Trong thời gian diễn ra sự kiện, nhiệm vụ chính của tôi là nỗ lực tìm kiếm và thuyết phục các nhà đầu tư rót vốn cho dự án Web3 cá nhân của mình.

Thực tế, tôi vốn không hề có kinh nghiệm trong hoạt động thuyết trình gọi vốn và bản thân cũng không quá tự tin khi giải thích chi tiết về các cơ chế mã hóa mật mã học phức tạp phía sau dự án, bởi chuyên môn chính của tôi chỉ thuần về lập trình frontend.

Tuy nhiên, tôi vốn là một người có sự tự tin khá cao và không hề e ngại việc phát biểu trước đám đông. Ngay trong ngày đầu tiên của sự kiện, tôi đã chủ động bước lên bục sân khấu chính để thuyết trình giới thiệu dự án.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121405.webp)

Vào thời điểm đó tôi mới tròn 21 tuổi, và sự tự tin cùng độ tuổi trẻ trung của tôi đã để lại ấn tượng mạnh mẽ cho nhiều người tham dự. Tôi là một trong những diễn giả trẻ tuổi nhất sự kiện và theo lời nhận xét của một số người, gương mặt của tôi trông còn trẻ hơn tuổi thực tế khá nhiều.

Lợi thế này đã giúp tôi nhanh chóng kết nối và làm quen với rất nhiều bạn bè trong ngành, từ các kỹ sư phát triển, nhà đầu tư cho đến các nhân sự làm việc trong lĩnh vực tiền mã hóa.

Một điều khiến tôi vô cùng bất ngờ là tổ chức NEAR Foundation đã đổ một khoản ngân sách khổng lồ cho sự kiện này. Xét thực tế NEAR chỉ là một đồng tiền mã hóa tương đối nhỏ và chưa được niêm yết rộng rãi trên hầu hết các sàn giao dịch lớn tại thời điểm đó, quy mô hoành tráng của hội nghị là điều không tưởng.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121406.webp)

Sự kiện chiêu đãi khách tham quan vô cùng xa hoa: Toàn bộ đồ ăn cao cấp đều miễn phí, các đêm tiệc tùng sôi động tại hộp đêm cũng hoàn toàn miễn phí, quỹ tiền thưởng mặt cho giải hackathon vô cùng lớn, các phòng hội thảo lớn được trang bị hệ thống màn hình và camera ghi hình hiện đại đi kèm khâu chuẩn bị tổ chức cực kỳ chuyên nghiệp.

Tôi cảm thấy khá băn khoăn: Tại sao một dự án blockchain chưa được biết đến rộng rãi lại sẵn sàng chi một lượng tiền khổng lồ như vậy cho các hoạt động sự kiện công nghệ ngoài đời thực?

Dường như đối với ban tổ chức, nhiệm vụ tối thượng của họ là phải làm hài lòng các nhà phát triển và giới đầu tư để giữ chân họ ở lại trải nghiệm một kỳ nghỉ cuối tuần vui vẻ tại Lisbon, từ đó nuôi hy vọng thu hút thêm nguồn vốn đầu tư mới và ngăn họ mất đi niềm tin vào các giải pháp công nghệ vốn vẫn chưa chứng minh được tính ứng dụng thực tiễn trong đời sống.

Chính từ trải nghiệm thực tế tại sự kiện ngày ấy, tôi đã bắt đầu giữ thái độ hoài nghi về giá trị thực tiễn lâu dài của toàn bộ hệ sinh thái công nghệ blockchain.

## Lịch sử tuần này

- 2022年（第 235 期）：[Vấn đề xã hội: Thảo luận về tình hình tỷ lệ thất nghiệp trong giới trẻ và xu hướng lựa chọn khởi nghiệp](http://www.ruanyifeng.com/blog/2022/12/weekly-issue-235.html)
- 2021年（第 185 期）：[Ứng dụng blockchain: Phân tích vụ đấu giá bản hiến pháp Mỹ thông qua mô hình DAO](http://www.ruanyifeng.com/blog/2021/11/weekly-issue-185.html)
- 2020年（第 135 期）：[Lựa chọn hướng đi: Lời khuyên phân tích các ngành nghề phù hợp nhất để bắt đầu khởi nghiệp](http://www.ruanyifeng.com/blog/2020/11/weekly-issue-135.html)
- 2019年（第 85 期）：[Góc nhìn xã hội: Bàn luận về các cơ chế giúp duy trì trật tự và ổn định trong xã hội Mỹ](http://www.ruanyifeng.com/blog/2019/12/weekly-issue-85.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
