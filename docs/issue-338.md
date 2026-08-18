# Bản tin chia sẻ công nghệ (Số 338): Suy nghĩ lại về 6G

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/6012) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 图片

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021919.webp)

Một góc sau vườn của một homestay độc đáo nằm cheo leo bên vách đá tại huyện Vu Sơn, Trùng Khánh, cung cấp góc nhìn toàn cảnh hùng vĩ xuống khu vực Tam Hiệp sông Trường Giang. (Nguồn: [qq.com](https://news.qq.com/rain/a/20231001A03MJW00))

## 重新思考 6G

Tuần trước, tạp chí khoa học của Viện Kỹ nghệ Điện và Điện tử Quốc tế (IEEE) mang tên *IEEE Spectrum* đã đăng tải bài viết phân tích sâu sắc mang tựa đề [《Suy nghĩ lại về 6G》](https://spectrum.ieee.org/5g-bandwidth).

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021901.webp)

Bài phân tích đưa ra một quan điểm vô cùng đáng suy ngẫm: **Nhu cầu về băng thông mạng của người dùng có thể đã chính thức bão hòa**.

Nội dung cốt lõi chỉ ra rằng, đối với đại đa số người dùng phổ thông, tốc độ đường truyền mạng hiện tại đã hoàn toàn đáp ứng tốt nhu cầu sinh hoạt hằng ngày. Ngay cả khi tốc độ Internet tiếp tục được nâng cấp cao hơn nữa, người tiêu dùng hầu như sẽ không cảm nhận được sự khác biệt thực tế nào.

Luận điểm này được chứng minh qua thực tế: Mạng di động 5G đã bắt đầu được triển khai thương mại từ năm 2018. Trải qua chặng đường hơn 6 năm phát triển, thế giới vẫn chưa ghi nhận sự xuất hiện của bất kỳ ứng dụng mang tính cách mạng (killer app) nào yêu cầu bắt buộc phải có 5G. **Hầu hết các ứng dụng phổ biến hiện nay đều có thể vận hành hoàn hảo ngay trên nền tảng mạng 4G**.

Để các bạn dễ hình dung, tôi xin tổng hợp sơ lược về mặt thứ tự độ lớn của tốc độ đường truyền: Tốc độ mạng 4G đạt mức 100 Mb/s (Megabits mỗi giây), mạng 5G đạt mức 1 Gb/s (1 Gb tương đương 1.000 Mb) và mạng 6G dự kiến trong tương lai sẽ đạt mức 10 Gb/s.

Lưu ý rằng ký tự "b" viết thường đại diện cho đơn vị bit. Trong khi đơn vị đo dung lượng tệp tin chúng ta thường thấy là MB và GB viết hoa đại diện cho Byte (1 Byte = 8 bits).

Các bạn có biết dòng ứng dụng tiêu tốn băng thông mạng nhất hiện nay yêu cầu tốc độ đường truyền tối thiểu là bao nhiêu không?

Các ứng dụng phát video chất lượng cao chính là dòng phần mềm ngốn băng thông nhất. Để xem mượt mà một bộ phim độ phân giải 4K trên nền tảng Netflix, tốc độ đường truyền yêu cầu chỉ là 15 Mb/s. Điều này đồng nghĩa với việc ngay cả dưới đường truyền 4G tiêu chuẩn, bạn hoàn toàn có thể mở đồng thời 3 đến 4 cửa sổ phát video 4K cùng lúc.

Chỉ có một số lượng vô cùng nhỏ các ứng dụng đặc thù mới có yêu cầu băng thông chạm đến ngưỡng tốc độ của 5G. Tiêu biểu như tựa game mô phỏng lái máy bay Microsoft Flight Simulator 2024 — một trong những phần mềm yêu cầu tốc độ đường truyền cao nhất hiện nay — cũng chỉ yêu cầu tốc độ 180 Mb/s.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021902.webp)

Như vậy, ở giai đoạn phát triển hiện tại, thế giới hoàn toàn chưa xuất hiện nhu cầu bắt buộc phải sử dụng tốc độ mạng 1 Gb/s. Đại đa số người dùng khi chuyển đổi từ mạng 4G lên 5G hầu như không cảm nhận thấy sự nâng cấp rõ rệt nào về mặt trải nghiệm, và kịch bản này chắc chắn sẽ lặp lại khi nâng cấp từ 5G lên 6G trong tương lai.

<u>Kết luận rút ra là: Đối với nhóm người dùng phổ thông, giới hạn về băng thông mạng thực tế đã chạm trần, tốc độ mạng 5G hiện tại hoàn toàn đủ khả năng đáp ứng tốt nhu cầu của đại đa số công chúng</u>.

Thực tế này khá tương đồng với lịch sử phát triển của ngành hàng không dân dụng. Trong suốt 50 năm qua, tốc độ bay của các dòng máy bay phản lực cỡ lớn hầu như không có sự thay đổi đáng kể nào, luôn được duy trì ổn định ở mức khoảng 900 km/h. Nguyên nhân hoàn toàn không phải do rào cản kỹ thuật khiến con người không thể chế tạo được những chiếc máy bay nhanh hơn, mà bởi mức tốc độ này chính là điểm cân bằng tối ưu nhất: hành khách cảm thấy thoải mái và chi phí vận hành bay không bị đẩy lên quá cao.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021903.webp)

Hạ tầng mạng viễn thông thế giới dường như cũng đang bước vào một chu kỳ tương tự. Mạng 5G đã hoàn toàn đáp ứng tốt nhu cầu, việc nâng cấp lên 6G không còn là một mục tiêu cấp bách và nhiều khả năng sẽ trì hoãn trong một thời gian dài sắp tới. Một mặt do nhu cầu thị trường không đủ lớn, mặt khác do chi phí đầu tư thiết bị và cước phí dữ liệu của công nghệ 6G sẽ vô cùng đắt đỏ, khiến người tiêu dùng hầu như không có động lực để chi trả.

Hệ quả kéo theo là thị trường sản xuất thiết bị viễn thông — nơi từng ghi nhận những khoản đầu tư khổng lồ và cạnh tranh khốc liệt suốt nhiều thập kỷ qua — sẽ bắt đầu bước vào giai đoạn tăng trưởng chậm lại. Các khoản ngân sách đầu tư xây dựng hạ tầng mạng của các nhà mạng viễn thông lớn sẽ sụt giảm mạnh.

Một khi các doanh nghiệp viễn thông không còn khả năng thu hút thêm khách hàng mới thông qua việc chạy đua nâng cấp tốc độ mạng, họ buộc phải thay đổi chiến lược kinh doanh tập trung vào các giải pháp khác như: (1) Cắt giảm giá cước dữ liệu; (2) Mở rộng vùng phủ sóng chất lượng cao đến các khu vực sóng yếu; (3) Tối ưu hóa chất lượng dịch vụ chăm sóc khách hàng.

Tương tự như việc các hãng hàng không giá rẻ bùng nổ khi tốc độ bay của máy bay dân dụng đạt ngưỡng bão hòa, chúng ta hoàn toàn có thể kỳ vọng vào sự xuất hiện của các nhà mạng giá rẻ cung cấp các gói cước dữ liệu siêu tiết kiệm trong tương lai.

## AI 动态（两则）

### AI 的研究模式

Bước sang năm 2025, đâu là xu hướng phát triển đột phá nhất của các mô hình ngôn ngữ lớn AI?

**Câu trả lời chắc chắn chính là "Chế độ nghiên cứu chuyên sâu" (Research Mode)**. Phương thức tương tác hỏi đáp ngắn gọn trước đây đã chính thức được nâng cấp lên khả năng phân tích lập luận sâu sắc (Reasoning).

Đối với các câu hỏi phức tạp đòi hỏi sự nghiên cứu chuyên sâu, hệ thống AI sẽ tự động thiết lập khung tư duy, phân tách vấn đề thành các bước xử lý nhỏ, tiến hành truy quét và đọc hiểu lượng lớn tài liệu học thuật trên mạng, sau đó tổng hợp thông tin để kết xuất câu trả lời hoàn chỉnh với các bước lập luận vô cùng chặt chẽ.

Trên thị trường quốc tế, các ông lớn như Google, OpenAI hay Perplexity đã liên tục giới thiệu tính năng Deep Research. Tại thị trường nội địa Trung Quốc, công cụ tìm kiếm thông minh đối đầu trực tiếp với Perplexity là **MiTa AI (秘塔 AI)** cũng đã chính thức cập nhật chế độ nghiên cứu chuyên sâu mới.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022004.webp)

Giải pháp kỹ thuật phía sau công cụ này là "Cấu trúc mô hình kép": Đối với các tác vụ yêu cầu phân tích lập luận sâu, hệ thống sẽ sử dụng phiên bản đầy đủ (full-blood version) của mô hình DeepSeek R1; trong khi các tác vụ tìm kiếm thông tin và tổng hợp tài liệu nhanh sẽ được giao phó cho mô hình tự phát triển của MiTa đảm nhận.

Dưới đây là [một ví dụ thực tế](https://metaso.cn/s/tfrWtdF): Khi bạn cần viết một bài luận chuyên ngành với tiêu đề "Hệ thống giao dịch tín chỉ carbon dựa trên công nghệ Blockchain", chế độ nghiên cứu sẽ hiển thị chi tiết sơ đồ tư duy phân tích vấn đề và tự động xây dựng nên một khung đề cương nghiên cứu khoa học hoàn chỉnh.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022003.webp)

Kết hợp cùng cơ sở dữ liệu học thuật riêng biệt của MiTa, hệ thống bảo đảm tính xác thực cao cho các nguồn tài liệu tham khảo trích dẫn. Trải nghiệm thực tế cho thấy chất lượng phản hồi đối với một số chủ đề học thuật của công cụ này thậm chí còn vượt trội hơn so với trang web chính thức của DeepSeek.

Tính năng đột phá này hiện đang được cung cấp **hoàn toàn miễn phí** với thao tác sử dụng vô cùng đơn giản. Các bạn có nhu cầu làm báo cáo hoặc phân tích dữ liệu có thể truy cập [trang web để trải nghiệm thử](https://metaso.cn/).

### VS Code 使用 DeepSeek 的方法

Làm thế nào để tích hợp và khai thác sức mạnh của mô hình DeepSeek trực tiếp bên trong trình soạn thảo mã nguồn VS Code?

Đối với các lập trình viên tại Trung Quốc, giải pháp đơn giản và tiện lợi nhất chính là sử dụng công cụ trợ lý lập trình **MarsCode** (Đậu Bao MarsCode).

Bản cập nhật mới nhất của tiện ích mở rộng này trên VS Code (phiên bản 1.1.62) và trên hệ sinh thái JetBrains (phiên bản 1.2.1.15) đều đã chính thức hỗ trợ kết nối với DeepSeek. Những bạn đã cài đặt trước đó chỉ cần tiến hành cập nhật trực tiếp trên IDE, còn người dùng mới có thể tải về từ [trang chủ của hãng](https://zjsms.com/iPg5wXhX/).

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021906.webp)

Trong quá trình viết code, bạn chỉ cần click chọn nút chuyển đổi mô hình ở góc dưới khung chat AI. Hệ thống hiện cung cấp 3 tùy chọn mô hình: doubao-1.5-pro, DeepSeek R1 và DeepSeek V3 (phiên bản đầy đủ). Toàn bộ dịch vụ đều được cung cấp **hoàn toàn miễn phí**.

Cả ba mô hình kể trên đều sở hữu năng lực xử lý vô cùng xuất sắc, giúp nâng cao đáng kể chất lượng các tính năng hỗ trợ như giải thích mã nguồn, chèn chú thích, sửa lỗi code, tối ưu hóa và giải đáp thắc mắc theo ngữ cảnh. Trong đó, mô hình DeepSeek R1 được vận hành trên hạ tầng đám mây Volcengine của ByteDance. Theo các kết quả đo đạc từ bên thứ ba, tốc độ kết xuất token đầu tiên (TTFT) và tốc độ tạo token (TPS) của giải pháp này đạt hiệu năng vô cùng ấn tượng.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021907.webp)

Hiện tại, đội ngũ phát triển MarsCode đang tổ chức chương trình trải nghiệm nhận quà: Người dùng chỉ cần chụp lại giao diện sử dụng thực tế kèm theo một đoạn chia sẻ trải nghiệm tối thiểu 30 chữ trên các nền tảng mạng xã hội (như Xiaohongshu, CSDN, Juejin), tag tài khoản chính thức "@豆包MarsCode" là sẽ có cơ hội tham gia chương trình bốc thăm trúng thưởng với tỷ lệ trúng rất cao thông qua tài khoản WeChat của hãng.

Ngoài ra, nhóm phát triển MarsCode vào tháng trước cũng đã ra mắt dòng IDE chuyên biệt cho AI mang tên **Trae** (sourl.cn/6P5AGW) tập trung tối ưu hóa trải nghiệm lập trình tương tác cùng trí tuệ nhân tạo, các bạn cũng có thể tải về trải nghiệm thử.

## 科技动态

1、[Kỳ thi cuối cùng của nhân loại (Humanity's Last Exam)](https://agi.safe.ai/)

Vào tháng 1 năm nay, hai doanh nghiệp AI tại Mỹ đã hợp tác công bố một bộ dữ liệu kiểm thử năng lực tư duy khoa học gồm tổng cộng 3.000 câu hỏi chuyên sâu thuộc nhiều lĩnh vực học thuật khác nhau.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025020701.webp)

Nhóm nghiên cứu công bố rằng một khi xuất hiện mô hình AI có khả năng vượt qua kỳ thi sát hạch này, điều đó sẽ là minh chứng khoa học khẳng định trí tuệ của máy tính đã chính thức vượt trội hơn trí tuệ của con người, đánh dấu cột mốc đạt tới cấp độ trí tuệ nhân tạo tổng hợp (AGI). Do đó, bộ đề thi này được đặt tên là "Kỳ thi cuối cùng của nhân loại".

Tính đến thời điểm ngày 3 tháng 2 vừa qua, điểm số kỷ lục cao nhất mà các mô hình AI hàng đầu thế giới đạt được mới chỉ dừng lại ở tỷ lệ trả lời chính xác 26,6%.

Theo nhận định của giới chuyên gia, việc AI vượt qua trí tuệ con người chỉ còn là vấn đề thời gian. Sự xuất hiện của bộ đề thi "Kỳ thi cuối cùng của nhân loại" giúp cộng đồng khoa học có được một thước đo định lượng cụ thể để theo dõi tiến trình lịch sử này.

2、[Ghế xoay thực tế ảo tương tác (VR Roto Chair)](https://skarredghost.com/2025/01/20/roto-vr-hands-on-impressions/)

Một doanh nghiệp khởi nghiệp tại Anh vừa giới thiệu dòng ghế xoay chuyên dụng dành cho trải nghiệm thực tế ảo VR, hỗ trợ người chơi tự động xoay chuyển cơ thể đồng bộ theo góc nhìn chuyển động trong thế giới ảo.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025012506.webp)

Hệ thống trang bị một bộ cảm biến gắn trực tiếp trên đỉnh kính thực tế ảo VR (hình trên) chịu trách nhiệm ghi nhận các chuyển động quay đầu của người dùng để truyền lệnh điều khiển đến động cơ xoay của ghế.

Khi bạn ngồi trên ghế và thực hiện thao tác quay đầu sang trái hoặc phải, chiếc ghế sẽ tự động xoay theo góc tương ứng. Ví dụ nếu bạn quay đầu sang trái một góc 45 độ, chiếc ghế cũng sẽ tự động xoay nhẹ sang trái đúng 45 độ.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025012507.webp)

Thiết bị mang lại trải nghiệm tương tác vô cùng chân thực trong không gian ảo, đồng thời giúp loại bỏ hoàn toàn cảm giác chóng mặt, buồn nôn thường gặp do sự bất đồng bộ giữa chuyển động của mắt và cơ thể khi trải nghiệm VR.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025012508.webp)

Nhà sáng chế công bố thiết bị này còn hỗ trợ đắc lực cho hiệu suất làm việc văn phòng. Nếu bạn thiết lập một hệ thống nhiều màn hình ảo hiển thị xung quanh trong không gian VR, bạn chỉ cần nghiêng nhẹ cổ là toàn bộ cơ thể sẽ tự động được xoay hướng về phía màn hình tương ứng, bảo đảm bàn phím ảo luôn nằm đối diện trực diện với cơ thể.

3、[Dự án xây dựng biệt thự dưới đáy biển](https://www.theguardian.com/environment/2025/feb/03/flooded-quarry-mysterious-millionaire-and-dream-new-atlantis-welsh-border-deep)

Một doanh nghiệp xây dựng tại Anh đang triển khai dự án thử nghiệm độc đáo mang tên "Biệt thự dưới lòng đại dương", nhằm nghiên cứu khả năng sinh sống dài hạn của con người ở độ sâu 80 mét dưới mực nước biển.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021202.webp)

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021203.webp)

Hình ảnh phía trên hiển thị bản vẽ phác thảo thiết kế kiến trúc và hình ảnh phía dưới ghi nhận thực tế quá trình thi công vỏ thép của công trình.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021204.webp)

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021205.webp)

Sau khi hoàn thiện lắp đặt dưới đáy biển, khách lưu trú sẽ di chuyển ra vào công trình thông qua một hệ thống tàu ngầm mini chuyên dụng.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021206.webp)

Quan sát thực tế cho thấy dự án này mang thiên hướng là một dịch vụ du lịch trải nghiệm xa xỉ dành cho giới siêu giàu hơn là một giải pháp định cư thực tiễn cho nhân loại dưới lòng đại dương.

Trên thực tế, việc di cư sinh sống dưới lòng sâu đại dương đối mặt với áp suất nước khổng lồ và thiếu ánh sáng là rất khó khả thi. Giải pháp phát triển các "Thành phố nổi tự chủ" trên mặt biển được đánh giá là có giá trị thực tiễn và tính khả thi cao hơn nhiều.

4、[Công nghệ nung quặng sắt bằng gạch gốm điện nhiệt](https://www.bostonglobe.com/2024/05/25/science/race-clean-up-heavy-industry-heats-up/)

Quy trình luyện kim sản xuất thép đòi hỏi nguồn nhiệt lượng cực cao để nung chảy quặng sắt. Các lò luyện kim truyền thống hiện nay chủ yếu sử dụng nhiên liệu than đá để đốt lò, gây ra các vấn đề ô nhiễm môi trường nghiêm trọng và phát thải lượng lớn khí CO2.

Các nhà máy thép trước đây không thể chuyển dịch sang giải pháp nung bằng điện năng thông thường do các sợi dây mayso nhiệt thông dụng không thể chịu đựng và duy trì được mức nhiệt lượng khổng lồ yêu cầu cho quy trình luyện thép, trong khi các sợi mayso hợp chất đặc chủng lại có giá thành quá đắt đỏ.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024052706.webp)

Để giải quyết bài toán này, một doanh nghiệp khởi nghiệp tại Mỹ đã chế tạo thành công mẫu lò nung không sử dụng than đá (hình trên), ứng dụng các khối gạch gốm chuyên dụng để tích và phát nhiệt lượng cao.

Dòng gạch gốm đặc chủng này (hình dưới) sở hữu khả năng liên tục hấp thụ nhiệt lượng từ nguồn điện năng truyền vào và tích trữ nhiệt ở mức hao hụt cực thấp. Chỉ cần được cấp điện năng liên tục, nhiệt độ bên trong lò nung gạch gốm có thể dễ dàng đạt mốc 1.800 độ C, hoàn toàn đủ năng lực nung chảy quặng sắt.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024052707.webp)

Phát minh này giúp các nhà máy thép có thể hoàn toàn loại bỏ than đá ra khỏi quy trình sản xuất, tận dụng nguồn điện năng xanh sạch từ hệ thống điện gió hoặc điện mặt trời để biến ngành luyện kim thành một ngành công nghiệp xanh thân thiện với môi trường.

## 文章

1、[React chính thức công bố ngừng hỗ trợ công cụ Create React App (CRA)](https://react.dev/blog/2025/02/14/sunsetting-create-react-app) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021505.webp)

Đội ngũ phát triển React chính thức thông báo kế hoạch khai tử công cụ khởi tạo dự án CRA quen thuộc. Hãng khuyến nghị lập trình viên nên chuyển sang khởi tạo React thông qua các framework hoàn chỉnh (như Next.js hay Remix) thay vì xây dựng các dự án SPA thuần túy trực tiếp từ thư viện React.

2、[Hướng dẫn tạo biểu đồ cột mini bằng các ký tự Unicode](https://blog.jonudell.net/2021/08/05/the-tao-of-unicode-sparklines/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082702.webp)

Bài viết hướng dẫn một kỹ thuật hiển thị dữ liệu thú vị: Ứng dụng tập hợp các ký tự Unicode đặc biệt để vẽ nên các biểu đồ cột dạng mini (sparklines) hiển thị trực tiếp ngay trong dòng văn bản (hình trên).

3、[Lập luận chứng minh tính hiệu quả của mô hình thiết kế ứng dụng nhiều trang (MPA)](https://htmx.org/essays/you-cant/) (tiếng Anh)

Mặc dù kiến trúc ứng dụng một trang (SPA) đang là tiêu chuẩn của lập trình web hiện đại, bài viết phân tích chỉ ra rằng các hệ thống MPA nếu được tối ưu hóa tốt vẫn hoàn toàn có thể mang lại các trải nghiệm mượt mà tương đương.

4、[Phân biệt cơ chế hoạt động của Hard Link và Soft Link trên hệ điều hành Linux](https://bhoot.dev/2024/on-linux-file-and-links/) (tiếng Anh)

Bài viết phân tích chuyên sâu giúp lập trình viên hiểu rõ sự khác biệt về mặt bản chất cấu trúc dữ liệu và cách thức quản lý tệp tin của hai loại liên kết Hard Link và Soft Link trên Linux.

5、[Khai phá thuộc tính overflow: clip trong thiết kế CSS](https://ishadeed.com/article/overflow-clip/) (tiếng Anh)

Bài viết hướng dẫn chi tiết cách thức ứng dụng giá trị `clip` của thuộc tính `overflow` trong CSS để cắt gọn các phần nội dung bị tràn và tạo ra các hiệu ứng giao diện đẹp mắt cho trang web.

6、[Tìm hiểu vai trò và cách thức khai báo siêu dữ liệu (Metadata) cho trang web](https://www.thisdaysportion.com/posts/dublin-core-what-is-it-good-for) (tiếng Anh)

Bài viết hướng dẫn cách chèn các thẻ thông tin mô tả chuẩn hóa (như tên tác giả, từ khóa chính, tóm tắt nội dung...) vào mã nguồn trang web nhằm tối ưu hóa khả năng đọc hiểu dữ liệu của các công cụ tìm kiếm và hệ thống AI.

7、[Hướng dẫn chi tiết quy trình cài đặt công cụ điều khiển thiết bị Android ADB](https://www.xda-developers.com/install-adb-windows-macos-linux/) (tiếng Anh)

ADB là công cụ dòng lệnh thiết yếu cho việc kết nối và thao tác phần mềm trên điện thoại Android từ máy tính. Bài viết hướng dẫn chi tiết các bước cài đặt và cấu hình công cụ trên các hệ điều hành Windows, macOS và Linux.

## 工具

1、[ElevenReader](https://elevenreader.io/)

Ứng dụng di động (hỗ trợ cả nền tảng iOS và Android) chuyên dụng cho việc chuyển đổi sách điện tử thành sách nói có hỗ trợ tiếng Việt. Tuy nhiên, chất lượng giọng đọc nhân tạo mặc định vẫn còn tương đối thô cứng.

2、[GIXY](https://github.com/dvershinin/gixy)

Công cụ dòng lệnh mã nguồn mở giúp quản trị viên hệ thống nhanh chóng quét và phân tích tệp tin cấu hình máy chủ NGINX để phát hiện các lỗi bảo mật hoặc cấu hình sai sót.

3、[uchū](https://uchu.style/)

Công cụ cung cấp các bộ sưu tập bảng phối màu (palettes) CSS tiện lợi dành cho nhà thiết kế web. Bảng màu ứng dụng khai báo thông số màu sắc theo hàm công nghệ mới `oklch()`. Tham khảo thêm bài viết phân tích [《Tại sao bạn nên từ bỏ hệ màu RGB/HSL để chuyển sang oklch()》](https://evilmartians.com/chronicles/oklch-in-css-why-quit-rgb-hsl).

4、[Bun Shell](https://bun.sh/blog/the-bun-shell)

Môi trường thực thi dòng lệnh tích hợp sẵn trong bộ công cụ Bun, cho phép lập trình viên viết và chạy các tệp kịch bản hệ thống trực tiếp bằng ngôn ngữ JavaScript một cách nhanh chóng.

5、[Spotube](https://github.com/KRTirtho/spotube)

Ứng dụng nghe nhạc đa nền tảng độc đáo: Công cụ đồng bộ hóa dữ liệu danh sách bài hát từ tài khoản Spotify cá nhân nhưng thực hiện phát trực tiếp nguồn âm thanh từ các dịch vụ chia sẻ miễn phí khác (như YouTube), giúp người dùng trải nghiệm nghe nhạc không quảng cáo mà không cần nâng cấp tài khoản Spotify Premium.

6、[Kener](https://github.com/rajnandan1/kener)

Hạ tầng giám sát trạng thái trực tuyến của các website tự triển khai (self-hosted), tự động vẽ biểu đồ thời gian hoạt động (uptime status) và gửi cảnh báo khi phát hiện sự cố mất kết nối. Dòng công cụ tương tự nổi tiếng khác là Uptime Kuma.

7、[gtrash](https://github.com/umlx5h/gtrash)

Công cụ quản lý thùng rác thông minh dành cho môi trường terminal trên Linux và macOS, cho phép người dùng dễ dàng liệt kê và khôi phục các tệp tin đã xóa bằng lệnh trực tiếp. Tham khảo thêm [bài viết giới thiệu chi tiết](https://linuxiac.com/gtrash-linux-command/).

## AI 工具

1、[DeepSRT](https://chromewebstore.google.com/detail/deepsrt-experience-the-fa/mdaaadlpcanoofcoeanghbmpbdbhladd)

Tiện ích mở rộng trên trình duyệt Chrome hỗ trợ tự động trích xuất phụ đề và hiển thị bản tóm tắt nội dung chính của video YouTube đang xem ngay ở thanh công cụ bên hông màn hình. (Đóng góp từ [@tsungmin](https://github.com/ruanyf/weekly/issues/6108))

2、[Deep Research Web UI](https://github.com/AnotiaWang/deep-research-web-ui)

Giao diện web mã nguồn mở hỗ trợ kết nối API với các mô hình ngôn ngữ lớn để tự xây dựng hệ thống nghiên cứu chuyên sâu (Deep Research) tự động quét dữ liệu web và tổng hợp báo cáo. (Đóng góp từ [@AnotiaWang](https://github.com/ruanyf/weekly/issues/6110))

3、[AI 翻译助手](https://github.com/ItusiAI/AI-Translation-Assistant-Pro)

Dự án mã nguồn mở xây dựng trang web dịch thuật tự động ứng dụng các mô hình AI chất lượng cao. (Đóng góp từ [@321208008](https://github.com/ruanyf/weekly/issues/6121))

4、[GitSeek](https://gitseek.dev/)

Dịch vụ tìm kiếm mã nguồn thông minh: Lập trình viên cung cấp đường dẫn kho chứa code, hệ thống sẽ cho phép sử dụng ngôn ngữ tự nhiên để truy vấn và định vị nhanh các đoạn mã nguồn xử lý tác vụ tương ứng. (Đóng góp từ [@i-richardwang](https://github.com/ruanyf/weekly/issues/6132))

5、[AI 多人聊天室](https://github.com/maojindao55/botgroup.chat)

Dự án phòng chat AI mã nguồn mở phát triển trên nền tảng React và dịch vụ Cloudflare Pages, cho phép người dùng trò chuyện và đối chiếu câu trả lời từ nhiều mô hình lớn khác nhau đồng thời trong cùng một giao diện. (Đóng góp từ [@maojindao55](https://github.com/ruanyf/weekly/issues/6133))

## 资源

1、[Sổ tay học từ vựng tiếng Anh CET-4 biên soạn bởi DeepSeek](https://github.com/vxiaozhi/vocabulary-book-by-deepseek)

Bộ tài liệu học từ vựng tiếng Anh ôn thi cấp độ 4 được biên soạn hoàn toàn bằng mô hình DeepSeek, cung cấp chi tiết ngữ nghĩa, từ căn phân tích cấu trúc, câu ví dụ thực tế và các mẹo ghi nhớ kèm hình ảnh trực quan. (Đóng góp từ [@vxiaozhi](https://github.com/ruanyf/weekly/issues/6107))

2、[Đường Vận (唐韵)](https://www.chinesepoems.org/)

Trang web lưu trữ và giới thiệu kho tàng thơ ca cổ Trung Quốc với phong cách thiết kế giao diện vô cùng tối giản và tinh tế. (Đóng góp từ [@LLSean](https://github.com/ruanyf/weekly/issues/6086))

3、[News Digest](https://news-digest-nine.vercel.app/)

Trang tổng hợp thông tin công nghệ: Ứng dụng AI để tự động dịch thuật và viết tóm tắt ngắn gọn các dòng tin tức công nghệ nóng hổi nhất từ các tờ báo lớn của Mỹ và châu Âu, cập nhật liên tục theo thời gian thực.

4、[Discuo](https://discuo.com)

Diễn đàn thảo luận trực tuyến theo phong cách tối giản cho phép người dùng tự do tham gia bình luận chia sẻ thông tin mà hoàn toàn không bắt buộc phải đăng ký tài khoản.

## 图片

1、[So sánh hiệu quả trực quan của biểu đồ tròn (Pie chart) và biểu đồ cột (Bar chart)](https://perthirtysix.com/visualizing-data-is-an-art)

Việc biểu diễn cùng một bộ số liệu phần trăm dưới dạng biểu đồ tròn và biểu đồ cột sẽ mang lại hiệu quả đọc hiểu thông tin rất khác biệt cho người xem.

Đầu tiên là dạng biểu đồ tròn.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021601.webp)

Tiếp theo là dạng biểu đồ cột.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021602.webp)

Theo các bạn, cách biểu diễn nào giúp người xem dễ dàng nắm bắt dữ liệu nhanh hơn?

Nghiên cứu khoa học chỉ ra rằng biểu đồ cột luôn cho khả năng đọc hiểu tốt hơn nhiều so với biểu đồ tròn. Nguyên nhân xuất phát từ việc cấu trúc não bộ của con người có khả năng so sánh tương quan về mặt độ dài tốt hơn nhiều so với khả năng so sánh tương quan về mặt góc độ hình học.

2、[Công nghệ bảo mật trên hộ chiếu mới của Thụy Sĩ](https://www.swissinfo.ch/chi/politics/%E6%96%B0%E7%89%88%E7%91%9E%E5%A3%AB%E6%8A%A4%E7%85%A7%E4%B8%8A%E6%9E%B6/48023134)

Mẫu hộ chiếu mới được phát hành của Thụy Sĩ tích hợp các lớp hình ảnh chìm bảo mật hiển thị dưới ánh sáng tia cực tím (UV) vô cùng độc đáo trên từng trang giấy.

Khi soi dưới đèn cực tím, trang bìa hộ chiếu sẽ hiển thị hình ảnh quốc huy Thụy Sĩ hình chữ thập rực rỡ.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021913.webp)

Các trang nội dung bên trong sẽ hiển thị chi tiết các đường đồng mức địa hình và bản đồ địa lý của quốc gia dưới dạng màu sắc phản quang bắt mắt.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021914.webp)

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021915.webp)

## 文摘

1、[50 năm kinh nghiệm du lịch khám phá thế giới](https://kk.org/thetechnium/50-years-of-travel-tips/)

Tác giả: Kevin Kelly (Nhà đồng sáng lập tạp chí *Wired*)

Tôi đã có hành trình liên tục du lịch khám phá thế giới suốt hơn 50 năm qua và đúc rút ra được nhiều bài học thực tiễn giá trị.

Hoạt động du lịch thông thường có thể được phân tách thành hai trạng thái khác biệt. Trạng thái thứ nhất là "Du lịch nghỉ dưỡng": Người dùng đi du lịch nhằm mục đích thoát khỏi áp lực công việc thường nhật để nghỉ ngơi và tái tạo năng lượng. Với trạng thái này, bạn nên chọn những địa điểm có dịch vụ tiện nghi và thong thả tận hưởng kỳ nghỉ.

Trạng thái thứ hai là "Du lịch trải nghiệm": Bạn đi du lịch để khám phá thế giới xung quanh, tích lũy các trải nghiệm mới, dấn thân vào các cuộc phiêu lưu đầy bất ngờ và tiếp xúc với những nền văn hóa xa lạ. Đây thực chất là một chu trình học tập thực tế, và các kinh nghiệm tôi chia sẻ dưới đây chủ yếu hướng tới trạng thái này.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022005.webp)

Sai lầm phổ biến nhất của nhiều người khi đi du lịch là cố gắng nhồi nhét để đi được nhiều địa điểm nhất có thể. Do tâm lý sợ rằng bản thân sẽ không có cơ hội quay lại nơi này lần thứ hai, họ liên tục tìm cách tối đa hóa hành trình: "Nếu chúng ta đang ở điểm X, mà điểm Y và Z lại nằm khá gần đó, tại sao không tranh thủ ghé qua luôn...".

Thực tế chứng minh việc bạn chọn lưu lại tại ít địa điểm hơn nhưng với thời gian dài hơn sẽ mang lại những trải nghiệm giá trị hơn nhiều so với việc mất phần lớn thời gian di chuyển qua lại giữa một loạt các tọa độ khác nhau. Bạn nên học cách làm chậm tốc độ hành trình và dành nhiều thời gian hơn để nghỉ ngơi tĩnh lặng.

Những khoảnh khắc đáng nhớ nhất của một chuyến đi — như việc tình cờ trò chuyện với một người xa lạ bản địa, được mời đến thăm nhà của họ hay tự mình khám phá ra một góc phố ẩn giấu — thường chỉ xảy ra khi bạn dừng chân đứng lại quan sát xung quanh.

Bên cạnh đó, việc ưu tiên lựa chọn những quốc gia có chi phí sinh hoạt thấp sẽ giúp bạn kéo dài thời gian lưu trú hơn với cùng một mức ngân sách dự chi. Hơn nữa, những điểm đến giá rẻ và ít người biết tới thường ẩn chứa nhiều giá trị văn hóa bản địa vô cùng độc đáo rất đáng để bạn khám phá.

Để thu về một chuyến du lịch trải nghiệm hoàn hảo, bạn bắt buộc phải đầu tư hoặc thật nhiều tiền bạc, hoặc thật nhiều thời gian. Trong hai tùy chọn đó, việc đầu tư thời gian luôn mang lại giá trị tốt hơn nhiều. Tiền bạc có thể giúp bạn mua được các gói dịch vụ tiện lợi, nhưng tiền bạc không bao giờ mua được những trải nghiệm sâu sắc mà chỉ có thời gian và sự tĩnh lặng mới có thể mang lại.

## 言论

1、

Tôi nhận thấy các mô hình lớn AI khi thực hiện sinh mã nguồn luôn có xu hướng ưu tiên khai thác các giải pháp công nghệ phổ biến của giai đoạn trước thời điểm tháng 11 năm 2022 (thời điểm dòng ChatGPT lần đầu ra mắt). Sự ưu ái mang tính thuật toán này của AI vô tình làm kéo dài vòng đời sử dụng và cản trở việc phổ biến các công nghệ lập trình mới hơn trên thị trường.

-- *Trích bài phân tích 《Trí tuệ nhân tạo đang vô tình kìm hãm sự đổi mới công nghệ》*

2、

Tôi cho rằng châu Âu thực sự cần phải có những hành động quyết liệt để bứt phá. Trong suốt 20 năm qua, tốc độ tăng trưởng kinh tế của Mỹ và Trung Quốc đã bỏ xa hoàn toàn khối EU.

Nếu các nhà quản lý tiếp tục duy trì các chính sách kiểm soát và kìm hãm quá mức đối với công nghệ trí tuệ nhân tạo, châu Âu đối mặt với nguy cơ tụt hậu để rồi trở thành một "bảo tàng lịch sử cổ kính" của thế giới.

-- *Ulf Kristersson, Thủ tướng Thụy Điển chia sẻ*

3、

Trong thế giới kinh doanh, lợi thế thuộc về những người tiên phong đi đầu (first-mover advantage). Tuy nhiên trong lĩnh vực nghiên cứu khoa học và học thuật, vinh quang cuối cùng thường không thuộc về người đầu tiên đưa ra phát kiến, mà thuộc về người sở hữu sự thấu hiểu sâu sắc và bản chất nhất về vấn đề đó. Lợi thế cạnh tranh đích thực nằm ở các góc nhìn nền tảng và cốt lõi nhất.

-- *Trích bài viết 《Hồi ký về khoảng thời gian nghiên cứu tại MIT》*

4、

Người đi tiên phong phải bỏ ra nguồn lực khổng lồ để khai phá con đường mới, trong khi những người đi sau chỉ cần sử dụng một lượng tài nguyên tính toán nhỏ hơn nhiều đã có thể nhanh chóng thu hẹp khoảng cách công nghệ. Đây chính là khái niệm về "bất lợi của người đi đầu" (second-mover advantage/pioneer disadvantage) trong phát triển AI.

-- *Ý kiến độc giả trên diễn đàn Hacker News*

5、

Khi bạn tiếp cận công việc bằng một thái độ khiêm nhường và tinh thần tò mò thuần khiết, bạn sẽ học hỏi được nhiều kiến thức hơn và có sự dấn thân trọn vẹn hơn. Duy trì một tư duy của người mới bắt đầu (beginner's mind) luôn là một tài sản vô giá giúp bạn định vị được sứ mệnh đích thực của cuộc đời mình.

-- *Trích bài viết 《Hồi ký về khoảng thời gian nghiên cứu tại MIT》*

## 往年回顾

- Số #291: [Thảo luận về luận điểm: Công nghệ AI thực tế không sở hữu rào cản độc quyền (Moat)](http://www.ruanyifeng.com/blog/2024/03/weekly-issue-291.html)
- Số #241: [Phân tích luận điểm: Động lực tăng trưởng tương lai của Trung Quốc nằm ở các vùng nội địa](http://www.ruanyifeng.com/blog/2023/02/weekly-issue-241.html)
- Số #191: [Chia sẻ hành trình tự do tài chính của một lập trình viên công nghệ](http://www.ruanyifeng.com/blog/2022/01/weekly-issue-191.html)
- Số #141: [Thảo luận về sự chiến thắng của các hệ thống sinh thái khép kín trong công nghệ](http://www.ruanyifeng.com/blog/2021/01/weekly-issue-141.html)

(Hết)
