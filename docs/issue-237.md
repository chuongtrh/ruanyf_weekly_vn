# 科技爱好者周刊（第 237 期）：真实方位是如何暴露的？

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần。

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn。

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2771) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập。

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122705.jpg)

Ngày 23 tháng 12, sân bay nằm ở cực Tây của Trung Quốc - sân bay Tashkurgan tại Tân Cương đã chính thức khánh thành và đón chuyến bay đầu tiên. Đây là sân bay đầu tiên được xây dựng trên cao nguyên Pamir (người xưa gọi là "thung lũng hành"), nằm ngay dưới chân một ngọn núi băng vĩnh cửu. (Nguồn: [Sina](https://news.sina.com.cn/o/2022-12-23/doc-imxxrpwa1056172.shtml))

## 本周话题：真实方位是如何暴露的？

Trong quá trình phát triển ứng dụng, các lập trình viên thường xuyên cần xác định vị trí địa lý của người dùng để cung cấp dịch vụ phù hợp.

Giải pháp đơn giản nhất là dựa vào địa chỉ IP truy cập của người dùng để đối chiếu khu vực địa lý.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122706.webp)

Nếu bạn không muốn lộ vị trí thực tế của mình, bạn có thể sử dụng các giải pháp kỹ thuật như VPN để giả lập địa chỉ IP ở một quốc gia khác.

Tuy nhiên, câu chuyện thực tế không hề đơn giản như vậy, **vị trí thực tế của bạn cực kỳ khó che giấu hoàn toàn.**

Tuần trước, trên diễn đàn công nghệ Hacker News xuất hiện [một bài thảo luận](https://news.ycombinator.com/item?id=34032484) của một thành viên chia sẻ thắc mắc về việc làm thế nào Google vẫn định vị chính xác vị trí của anh:

Anh đi công tác từ Mỹ sang Mexico. Để truy cập các dịch vụ ngân hàng trực tuyến của Mỹ, anh luôn kết nối VPN để giả lập địa chỉ IP của mình tại bang Washington (Mỹ) trong suốt chuyến đi. Về mặt lý thuyết, máy chủ ngân hàng chỉ ghi nhận anh đang truy cập từ Mỹ.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122707.webp)

Tuy nhiên, sau khi kết thúc chuyến công tác và quay trở lại Mỹ, anh mở máy tính để bàn ở nhà lên (chiếc máy tính này đặt cố định tại nhà và chưa từng mang đi đâu). Trình duyệt của anh lập tức định vị vị trí của anh tại Mexico và liên tục hiển thị các nội dung quảng cáo bằng tiếng Tây Ban Nha.

Anh vô cùng bối rối: Làm thế nào Google có thể biết được việc anh từng ở Mexico khi máy tính ở nhà của anh không hề di chuyển và máy tính xách tay đi công tác luôn được che giấu bằng VPN?

Bên dưới bài đăng, nhiều chuyên gia bảo mật đã giải thích cơ chế định vị của Google: Để xác định vị trí địa lý của thiết bị, các tập đoàn công nghệ không chỉ nhìn vào địa chỉ IP, mà tham số quan trọng hơn họ sử dụng là **địa chỉ MAC của các router Wi-Fi xung quanh bạn.**

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122708.webp)

Thông thường, các router Wi-Fi là thiết bị cố định tại nhà hoặc văn phòng và hầu như không bao giờ di chuyển vị trí địa lý. Rất hiếm ai mang theo router Wi-Fi khi đi du lịch.

Do đó, chỉ cần xác định được thiết bị của bạn đang kết nối vào router Wi-Fi nào, hệ thống có thể suy ra vị trí địa lý chính xác của bạn dựa trên vị trí cố định của router đó.

Địa chỉ MAC của mỗi router Wi-Fi là duy nhất trên toàn cầu và không thay đổi. Các tập đoàn công nghệ lớn như Google hay Apple đã xây dựng một cơ sở dữ liệu khổng lồ liên kết địa chỉ MAC của hàng triệu router Wi-Fi với tọa độ GPS thực tế.

Cơ sở dữ liệu này được thu thập tự động thông qua hàng triệu thiết bị chạy Android hoặc trình duyệt Chrome bật định vị GPS di chuyển hàng ngày: mỗi khi điện thoại của ai đó bật GPS và quét thấy một mạng Wi-Fi xung quanh, hệ thống sẽ gửi cặp dữ liệu (địa chỉ MAC của Wi-Fi + tọa độ GPS hiện tại) về máy chủ Google để cập nhật bản đồ vị trí. Nếu thiết bị của bạn không có chip GPS (như máy tính để bàn), Google sẽ quét danh sách các địa chỉ MAC Wi-Fi xung quanh để đối chiếu vị trí trên bản đồ.

Do cơ chế đồng bộ dữ liệu này có độ trễ thời gian nhất định chứ không cập nhật thời gian thực, khi bạn đi công tác và kết nối thiết bị của mình vào wifi tại Mexico, hệ thống của Google ghi nhận tài khoản của bạn đang liên kết với router đó. Khi bạn quay về Mỹ, hệ thống vẫn lưu vết khu vực Mexico này một thời gian trước khi tự động cập nhật lại vị trí mới cho tài khoản của bạn.

Nếu bạn thực sự muốn bảo vệ vị trí cá nhân tối đa, giải pháp khả thi duy nhất là sử dụng các hệ điều hành di động mã nguồn mở đã loại bỏ hoàn toàn các dịch vụ ngầm của Google (như [GrapheneOS](https://grapheneos.org/)) hoặc sử dụng các trình duyệt Chromium độc lập.

Tuy nhiên, hầu hết các ứng dụng di động hiện nay đều tích hợp âm thầm các bộ SDK thu thập dữ liệu vị trí này. Với sự liên thông dữ liệu giữa nhà mạng, hệ điều hành và các ứng dụng chạy ngầm, việc che giấu hoàn toàn vị trí thực tế trên Internet hiện nay gần như là nhiệm vụ bất khả thi.

## 活动

1、[Hội thảo kỹ thuật chia sẻ kinh nghiệm phát triển Flutter của ByteDance](https://www.bagevent.com/event/8366150?bag_track=001)

Trong số các giải pháp phát triển ứng dụng đa nền tảng hiện nay, Flutter của Google đang là công nghệ thu hút sự quan tâm lớn nhất nhờ khả năng đóng gói bộ thư viện đồ họa trực tiếp vào ứng dụng giúp mang lại trải nghiệm mượt mà, đồng nhất trên mọi nền tảng.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122803.webp)

Với phiên bản Flutter 3.0 ra mắt vào tháng 5 vừa qua, công nghệ này đã hỗ trợ xuất bản ứng dụng đồng thời trên cả 6 nền tảng lớn gồm iOS, Android, Web, Windows, macOS và Linux từ một bộ mã nguồn duy nhất.

Vào chiều thứ Bảy (ngày 14 tháng 1 năm 2023) lúc 14 giờ, **đội ngũ kỹ sư của ByteDance sẽ tổ chức buổi hội thảo trực tuyến chia sẻ các kinh nghiệm thực tế khi ứng dụng Flutter ở quy mô lớn:**

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122804.webp)

Tại ByteDance, hiện có hơn 70 ứng dụng di động được phát triển dựa trên Flutter với đội ngũ lập trình viên nội bộ lên tới hơn 600 kỹ sư. Họ đã đóng góp rất nhiều bản vá PR quan trọng cho kho chứa mã nguồn mở của Flutter.

Hội thảo chuyên đề **《Phân tích chuyên sâu về khám phá và thực tiễn công nghệ Flutter》** sẽ gồm 4 bài phát biểu chia sẻ về cấu trúc kiến trúc dự án, kinh nghiệm tối ưu hóa hiệu năng render đồ họa và quy trình CI/CD cho các dự án Flutter lớn. Độc giả quan tâm có thể đăng ký tham gia giao lưu trực tuyến và bốc thăm trúng thưởng tại [Trang đăng ký hội thảo Flutter của ByteDance](https://www.bagevent.com/event/8366150?bag_track=001).

## 科技动态

1、[Ý tưởng thành phố nổi turtle-shape khổng lồ trên đại dương](https://www.pangeosyacht.com/projects)

Một hãng thiết kế du thuyền quốc tế vừa công bố bản phác thảo ý tưởng táo bạo về một tổ hợp thành phố nổi khổng lồ trên đại dương mang tên Pangeos với tạo hình giống một chú rùa biển lớn:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111704.webp)

Công trình thực chất là một siêu du thuyền có chiều dài 550m và chiều rộng lên tới 600m. Trên mai rùa khổng lồ này là một thị trấn hoàn chỉnh với các tòa nhà căn hộ, trung tâm thương mại và công viên cây xanh:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111705.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111706.webp)

Hãng thiết kế kỳ vọng sẽ huy động vốn bằng cách bán trước các căn hộ trên tàu. Con tàu dự kiến sẽ di chuyển liên tục quanh các đại dương và neo đậu gần cảng biển của các quốc gia để du khách trên tàu có thể chu du khắp thế giới.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111707.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111708.webp)

Tuy nhiên, hãng thiết kế vẫn chưa đưa ra được các lời giải khả thi về nguồn động lực đẩy khổng lồ để di chuyển cấu trúc này, cách thức tiếp tế thực phẩm nước ngọt cho hàng ngàn cư dân trên tàu, cũng như bến cảng nào đủ quy mô để đón nhận một con tàu khổng lồ như vậy. Nhiều người nhận định đây chỉ là một dự án mang tính quảng bá hình ảnh.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111709.webp)

2、[Sân vận động New York ứng dụng nhận diện khuôn mặt để chặn đối thủ pháp lý](https://www.nytimes.com/2022/12/22/nyregion/madison-square-garden-facial-recognition.html)

Tổ hợp nhà thi đấu và sân vận động nổi tiếng Madison Square Garden (MSG) tại New York thuộc sở hữu của gia tộc tỷ phú James L. Dolan:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122406.webp)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122407.webp)

Năm ngoái, gia tộc Dolan bị vướng vào một vụ kiện tụng pháp lý. Kết quả là ban quản lý MSG đã đưa toàn bộ các luật sư làm việc tại văn phòng luật đang thụ lý vụ kiện đó vào danh sách đen (blacklist) cấm cửa.

Mới đây, một luật sư thuộc văn phòng này khi đến MSG để xem một trận đấu thể thao đã bị hệ thống camera nhận diện khuôn mặt tự động phát hiện ngay tại cửa kiểm soát an ninh. Nhân viên bảo vệ lập tức xuất hiện và mời anh rời khỏi khu vực với lý do thuộc nhóm người bị cấm vào cửa:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122408.webp)

Sự việc đang gây tranh cãi lớn tại New York khi hiệp hội luật sư chuẩn bị khởi kiện MSG vì hành vi lạm dụng công nghệ nhận diện khuôn mặt để phân biệt đối xử. Tuy nhiên, do MSG là khu vực tài sản tư nhân, chủ sở hữu có quyền hợp pháp trong việc từ chối phục vụ khách hàng nên vụ kiện dự kiến sẽ gặp nhiều khó khăn pháp lý.

3、[Thử nghiệm thành công dòng cánh quạt máy bay 11 lá đầu thế giới](https://interestingengineering.com/innovation/worlds-first-propeller-with-11-blades)

Một hãng hàng không của Đức vừa công bố thử nghiệm cất cánh thành công mẫu máy bay trang bị cánh quạt 11 lá đầu tiên trên thế giới:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122806.webp)

Vai trò của cánh quạt máy bay là chuyển đổi năng lượng của động cơ thành lực đẩy khí động học. Thông thường, diện tích bề mặt lá cánh quạt quan trọng hơn số lượng lá, đó là lý do hầu hết máy bay cánh quạt cỡ nhỏ hiện nay chỉ sử dụng cánh quạt 2 lá hoặc 3 lá.

Tuy nhiên, đối với các động cơ phản lực cánh quạt có công suất cực lớn, khi giới hạn vật lý không cho phép tăng thêm chiều dài lá cánh quạt (do va chạm mặt đất hoặc tốc độ đầu cánh quạt vượt vận tốc âm thanh), việc tăng số lượng lá cánh quạt lên 11 lá là giải pháp tối ưu để gia tăng đáng kể lực đẩy cho máy bay.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122807.webp)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122808.webp)

4、[NASA đầu tư nghiên cứu công nghệ in 3D công trình trên Mặt Trăng](https://makerfairerome.eu/en/nasa-advance-lunar-construction-technology-for-moon-missions/)

Cơ quan Hàng không Vũ trụ Mỹ (NASA) vừa công bố khoản tài trợ trị giá 57,2 triệu USD cho một công ty xây dựng công nghệ để phát triển hệ thống thiết bị in 3D có khả năng thi công các công trình trên bề mặt Mặt Trăng:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122409.webp)

Mục tiêu của dự án là thiết kế các robot tự động có khả năng tận dụng đất cát trên Mặt Trăng (lunar regolith) làm nguyên liệu thô để in 3D các công trình kiên cố như bãi đáp tàu vũ trụ, đường giao thông và các khu nhà ở bảo vệ phi hành gia khỏi bức xạ vũ trụ và sự va đập của thiên thạch nhỏ. Công nghệ này dự kiến cũng sẽ được nâng cấp thử nghiệm cho các sứ mệnh thám hiểm Sao Hỏa trong tương lai.

## 文章

1\. [Giải thích dễ hiểu về đột phá độ lợi năng lượng hạt nhân nhiệt hạch](https://mp.weixin.qq.com/s/44H689gZQ-26ZbzC9D-RTg)（Tiếng Trung）

Bài viết phổ biến khoa học giải thích chi tiết ý nghĩa sự kiện Bộ Năng lượng Mỹ tuyên bố đạt được bước tiến lớn "net energy gain" (độ lợi năng lượng thuần) trong phản ứng hạt nhân nhiệt hạch kiểm soát bằng hệ thống laser công suất lớn, mở ra hy vọng về nguồn năng lượng sạch không giới hạn. (Đóng góp của [@marmul2](https://github.com/ruanyf/weekly/issues/2811))

2\. [Phân tích các ưu thế địa lý tự nhiên độc nhất vô nhị của nước Mỹ](https://unchartedterritories.tomaspueyo.com/p/world-chessboard)（Tiếng Anh）

Bài phân tích sâu sắc về mặt địa chính trị giải thích các ưu thế địa lý của Mỹ: hai đại dương bao bọc bảo vệ, đồng bằng trung tâm rộng lớn màu mỡ và hệ thống sông ngòi nội địa liên thông có tổng chiều dài vận tải thủy vượt trội hơn hẳn mọi quốc gia khác giúp tối ưu chi phí vận chuyển hàng hóa. Bài viết đính kèm hình vẽ so sánh kích thước thuyền buồm thám hiểm lớn thời Minh của Trịnh Hòa so với chiếc thuyền nhỏ vượt đại dương của Colombo.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122106.webp)

3\. [Hướng dẫn chi tiết về cấu trúc mạng xã hội phi tập trung Mastodon](https://wordsmith.social/elilla/a-futuristic-mastodon-introduction-for-2021)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110306.webp)

Tài liệu giới thiệu chi tiết cho lập trình viên và người dùng về cơ chế hoạt động phi tập trung (decentralized) của hệ thống mạng xã hội Mastodon, cách thức hoạt động của các máy chủ độc lập (instances) liên kết với nhau qua giao thức ActivityPub.

4\. [CDN Bunny.net ứng dụng AI tự động sinh ảnh đại diện hình thỏ độc bản](https://bunny.net/blog/introducing-bunny-optimizer-ai-a-new-way-of-creating-content/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121602.webp)

Hãng dịch vụ CDN Bunny.net giới thiệu giải pháp ứng dụng mô hình AI tạo ảnh tự động vẽ các hình đại diện chú thỏ độc bản riêng biệt cho mỗi khách hàng đăng ký tài khoản mới trên hệ thống để tăng tính cá nhân hóa trải nghiệm.

5\. [Hướng dẫn sử dụng thẻ `<picture>` tối ưu hóa hình ảnh đáp ứng](https://jfhr.me/optimizing-images-with-the-html-picture-tag/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110309.webp)

Bài hướng dẫn cơ bản cho nhà phát triển Front-end cách thức sử dụng thẻ `<picture>` trong HTML5 kết hợp thuộc tính `media` để trình duyệt tự động hiển thị định dạng và kích thước ảnh tối ưu nhất cho từng loại thiết bị.

6\. [Mẹo thiết lập mã HTML ngăn trình duyệt gửi yêu cầu tải favicon](https://tdarb.org/blog/under-1kb.html)（Tiếng Anh）

Tác giả chia sẻ các mẹo định dạng code HTML tối giản để giảm dung lượng trang web xuống dưới 1KB, trong đó có đoạn mã khai báo giúp chặn trình duyệt tự động phát đi yêu cầu tải tệp tin biểu tượng `favicon.ico` gây chậm tốc độ tải trang.

7\. [Lợi thế trường tồn của cơ sở dữ liệu quan hệ so với các giải pháp NoSQL](https://www.simplethread.com/relational-databases-arent-dinosaurs-theyre-sharks/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072613.webp)

Bài viết phân tích các thế mạnh của hệ cơ sở dữ liệu quan hệ truyền thống sử dụng ngôn ngữ SQL (như tính nhất quán ACID, độ tin cậy giao dịch lớn) chứng minh đây vẫn là công cụ cốt lõi của ngành công nghệ thông tin.

8\. [8 quan niệm sai lầm kinh điển về hệ thống mạng phân tán](https://architecturenotes.co/fallacies-of-distributed-systems/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060504.webp)

Bài viết phân tích sâu sắc 8 ngộ nhận phổ biến của lập trình viên khi thiết kế kiến trúc phân tán (như coi mạng luôn thông suốt, băng thông vô hạn, độ trễ bằng không), giúp người đọc nhận thức rõ các rào cản kỹ thuật thực tế.

## 工具

1、[tremor: Thư viện React component UI chuyên dụng cho các trang Dashboard](https://www.tremor.so/)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101103.webp)

Bộ thư viện mã nguồn mở cung cấp các components UI thiết kế hiện đại, tinh giản giúp lập trình viên nhanh chóng xây dựng các giao diện Dashboard hiển thị biểu đồ số liệu trực quan.

2、[GPTAnywhere: Tiện ích tương tác ChatGPT trên thanh công cụ Chrome](https://chrome.google.com/webstore/detail/gptanywhere/pklibapjplkpanekidgnckgjablljhni)

Plugin Chrome cho phép người dùng nhấp nhanh biểu tượng trên thanh công cụ trình duyệt để mở ngay giao diện chat với ChatGPT mà không cần mở tab trang chủ.

3、[Obsidian Canvas: Tính năng thiết lập bản đồ tư duy trên Obsidian](https://obsidian.md/canvas)

Công cụ ghi chú cá nhân Obsidian ra mắt tính năng Canvas cho phép người dùng tạo một trang vẽ vô cực kéo thả tự do để liên kết các ghi chú, hình ảnh thành dạng sơ đồ tư duy trực quan:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122104.webp)

4、[Enhance Speech: Tiện ích lọc nhiễu nâng cao chất lượng giọng nói AI của Adobe](https://podcast.adobe.com/enhance)

Ứng dụng web chạy AI của Adobe hỗ trợ lọc nhiễu âm môi trường, tự động nâng cao chất lượng giọng nói ghi âm thông thường thành chất giọng trong trẻo tương đương thu âm trong phòng thu chuyên nghiệp.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121904.webp)

5、[One Tab Group: Tiện ích mở rộng quản lý và đồng bộ nhóm tab trình duyệt](https://www.onetab.group/)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122111.webp)

Extension Chrome hỗ trợ người dùng gom nhóm các tab đang mở ngăn nắp, quản lý bộ nhớ đệm và hỗ trợ đồng bộ hóa danh sách tab lên đám mây. (Đóng góp của [@xiaoluoboding](https://github.com/ruanyf/weekly/issues/2812))

6、[Forgejo: Dự án git client phi thương mại tách ra từ Gitea](https://forgejo.org/)

Sau khi Gitea thương mại hóa, một nhóm lập trình viên lo ngại mất tính mở đã tách nhánh (fork) mã nguồn để xây dựng dự án Forgejo hoạt động phi lợi nhuận độc lập:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121603.webp)

7、[Satori: Thư viện JavaScript chuyển đổi HTML/CSS sang định dạng SVG](https://github.com/vercel/satori)

Thư viện JS gọn nhẹ của Vercel hỗ trợ biên dịch nhanh các thẻ HTML và thuộc tính định dạng CSS cơ bản thành một tệp hình ảnh đồ họa vector SVG động, rất hữu ích để tự động sinh các ảnh xem trước (OG image).

8、[Agreper: Diễn đàn tối giản viết bằng Python hoàn toàn không dùng JS](https://github.com/Demindiro/agreper)

Dự án mã nguồn xây dựng diễn đàn thảo luận tối giản viết bằng Python, điểm đặc biệt là hệ thống vận hành hoàn toàn dựa trên cơ chế HTTP request truyền thống và không cần tải bất kỳ dòng code JavaScript nào ở trình duyệt client.

9、[Rmt.rs: Tiện ích dòng lệnh CLI thay thế lệnh rm tích hợp thùng rác](https://github.com/AmineZouitine/rmt.rs)

Công cụ dòng lệnh viết bằng Rust hoạt động tương tự lệnh xóa tệp `rm` nhưng chuyển tệp tin vào một thư mục thùng rác (recycle bin) tạm thời để người dùng có thể khôi phục lại khi cần.

## 资源

1、[OpenVerse: Trình tìm kiếm thư viện hình ảnh và âm thanh miễn phí bản quyền](https://wordpress.org/openverse/)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092904.webp)

Công cụ tìm kiếm thông tin của WordPress hỗ trợ tra cứu hơn 600 triệu hình ảnh và âm thanh miễn phí bản quyền cho phép người dùng tự do tải về sử dụng thương mại.

2、[MetroDB: Bản đồ trực quan hóa dữ liệu hệ thống tàu điện ngầm Trung Quốc](https://metrodb.org/index/beijing.html)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122901.webp)

Trang web trực quan hóa dữ liệu mạng lưới đường ray, ga tàu điện ngầm và lưu lượng hành khách đi lại hàng ngày của các đô thị lớn tại Trung Quốc. (Đóng góp của [@xcuYao](https://github.com/ruanyf/weekly/issues/2816))

3、[Green Wall: Công cụ hiển thị lịch sử đóng góp code trên GitHub](https://green-wall.vercel.app/)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122902.webp)

Ứng dụng web hỗ trợ trực quan hóa biểu đồ đóng góp code (contribution graph) của một tài khoản GitHub qua các năm. (Đóng góp của [@Codennnn](https://github.com/ruanyf/weekly/issues/2814) - Mã nguồn mở trên [GitHub](https://github.com/Codennnn/Green-Wall)).

4、[Codenews: Cộng đồng chia sẻ công cụ kỹ thuật dành cho lập trình viên](https://codenews.cc/)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122904.webp)

Trang diễn đàn thảo luận và giới thiệu các công cụ phần mềm, thư viện mã nguồn hữu ích dành cho giới phát triển phần mềm. (Đóng góp của [@jqsl2012](https://github.com/ruanyf/weekly/issues/2824))

5、[ChatBCG: Dịch vụ trực tuyến sinh slide thuyết trình PowerPoint bằng AI](https://www.chatbcg.com/)

Công cụ ứng dụng mô hình AI hỗ trợ người dùng nhập từ khóa để hệ thống tự động soạn thảo bố cục nội dung văn bản và thiết kế slide thuyết trình PowerPoint hoàn chỉnh:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122907.webp)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122906.webp)

## 图片

1\. **Bản đồ lưu vực hệ thống sông Mississippi kỳ vĩ của Mỹ**

Sông Mississippi là con sông dài nhất khu vực Bắc Mỹ với 3 nhánh chính chảy qua địa phận 32 bang của Mỹ và 2 tỉnh của Canada. Tổng diện tích lưu vực sông lên tới 3,2 triệu km²:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072505.webp)

Bản đồ lưu vực sông Mississippi với các nhánh sông được tô đậm màu xanh. Tuy sông có chiều dài ngắn hơn sông Trường Giang đôi chút nhưng diện tích lưu vực của nó rộng lớn gấp 1,8 lần lưu vực sông Trường Giang.

2\. **Bộ tranh sơn dầu nghệ thuật mang chủ đề phim khoa học viễn tưởng Star Wars**

Một nghệ sĩ người Thổ Nhĩ Kỳ đã thực hiện bộ tranh sơn dầu độc đáo tái hiện các nhân vật và bối cảnh viễn tưởng trong vũ trụ điện ảnh Chiến tranh giữa các vì sao:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031906.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031907.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031908.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031909.webp)

## ✍️ Bài đọc thêm

### Phép ẩn dụ thực tế về hoạt động khởi nghiệp kinh doanh

Hoạt động khởi nghiệp kinh doanh thực chất rất giống với trò chơi phi tiêu trúng thưởng tại các hội chợ công viên giải trí:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122908.webp)

* Những đứa trẻ xuất thân từ gia đình nghèo chỉ đủ tiền mua vé ném phi tiêu duy nhất **một lần**. Hầu hết chúng đều ném trượt. Một số ít may mắn ném trúng các vòng ngoài nhận phần quà nhỏ. Cực kỳ hiếm hoi có trường hợp ném trúng hồng tâm nhận giải thưởng lớn, và câu chuyện này thường được ca tụng như một tấm gương vượt khó đại diện cho "Giấc mơ Mỹ".

* Những đứa trẻ sinh ra trong gia đình khá giả có đủ nguồn lực tài chính để mua vé ném phi tiêu **vô số lần**. Chúng có thể liên tục ném thử, rút kinh nghiệm và ném lại cho đến khi trúng đích mới thôi. Một vài đứa trẻ trong số đó sau khi ném trúng đích sẽ đăng bài viết chia sẻ kinh nghiệm khởi nghiệp thành công và thuyết giảng về giá trị của sự kiên trì nỗ lực cá nhân.

* Còn những đứa trẻ thuộc hộ nghèo nhất thì hoàn toàn không có cơ hội bước chân vào công viên giải trí để chơi trò ném phi tiêu. Chúng phải đi làm thuê kiếm sống hàng ngày.

### Những phiền toái chưa được giải quyết của kết nối không dây Bluetooth

Giao thức truyền tải không dây Bluetooth đã ra đời được hơn 20 năm. Từ các thiết bị điện thoại di động, tai nghe không dây cho đến các vật dụng gia dụng như tủ lạnh, bóng đèn thông minh hiện nay đều dựa vào Bluetooth để kết nối.

Tuy nhiên, giao thức này vẫn tồn tại rất nhiều hạn chế cố hữu gây phiền toái cho người sử dụng:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122909.webp)

Ưu điểm lớn nhất của Bluetooth là mức tiêu thụ năng lượng cực kỳ thấp. Tuy nhiên, để đánh đổi lấy ưu điểm này, giao thức phải chấp nhận các giới hạn vật lý nghiêm ngặt: khoảng cách truyền nhận tín hiệu ngắn (thường dưới 15m), băng thông dữ liệu hẹp, dễ bị nhiễu sóng và độ bảo mật kém.

Do Bluetooth sử dụng dải tần số vô tuyến tự do không đăng ký bản quyền (2.4 GHz) để truyền tải, thiết bị của bạn bắt buộc phải chia sẻ dải tần này với hàng loạt thiết bị điện tử gia dụng khác (như lò vi sóng, cục phát Wi-Fi). Điều này gây nhiễu và làm suy giảm chất lượng kết nối không dây.

Vấn đề bảo mật của Bluetooth cũng là một rào cản lớn. Khi bạn kích hoạt một loa Bluetooth ở chế độ chờ kết nối, bất kỳ ai đứng trong bán kính 15m xung quanh đều có thể dò quét và gửi yêu cầu kết nối thiết bị, tiềm ẩn nhiều nguy cơ mất an toàn thông tin.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122910.webp)

Dù vậy, với sự phát triển của hệ sinh thái thiết bị thông minh IoT, nhu cầu kết nối gần giữa các thiết bị ngày càng gia tăng. Bluetooth vẫn là sự lựa chọn kết nối tối ưu nhất hiện nay. Người tiêu dùng trong tương lai sẽ tiếp tục phải học cách chung sống với các nhược điểm này của Bluetooth để tận hưởng sự tiện lợi của công nghệ kết nối không dây.

## 历史上的本周

- 2021年（第 189 期）：[Thảo luận kinh doanh: Nhìn nhận thực tế làn sóng cạnh tranh khốc liệt (nội quyển) tiếp theo trong ngành sản xuất công nghệ](https://www.ruanyifeng.com/blog/2021/12/weekly-issue-189.html)
- 2020年（第 139 期）：[Y học hiện đại: Khám phá những bước tiến công nghệ đột phá trong nghiên cứu sinh học di truyền](https://www.ruanyifeng.com/blog/2020/12/weekly-issue-139.html)
- 2019年（第 87 期）：[Văn hóa công sở: Tầm quan trọng của việc giao nhiệm vụ soạn thảo tài liệu kỹ thuật cho nhân sự mới trong đội ngũ](https://www.ruanyifeng.com/blog/2019/12/weekly-issue-87.html)
- 2018年（第 36 期）：[Thảo luận nghề nghiệp: Phân tích khả năng dư thừa nguồn nhân lực của ngành lập trình phần mềm trong tương lai](https://www.ruanyifeng.com/blog/2018/12/weekly-issue-36.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2771) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## 鸣谢

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072108.webp)

（Hết）
