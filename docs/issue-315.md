# Bản tin chia sẻ công nghệ (Số 315): Một báo cáo nghỉ việc tại Google

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/4911) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082605.webp)

Khi màn đêm buông xuống, vô số ngọn đèn dụ cá (ngư đăng) được thắp sáng lung linh trên hồ Nhĩ Hải ở Đại Lý để thu hút cá nổi lên mặt nước. Các ngư dân nhân cơ hội này để đánh bắt nhằm tiêu diệt loài cá trắng nhỏ Tây Thái Bình Dương (Hemiculter leucisculus) xâm hại. (Nguồn: [Haiwainet](https://news.haiwainet.cn/n/2024/0820/c3541083-32782962.html))

## 一份谷歌离职报告

Tuần trước, tôi tình cờ đọc được một [bài viết rất thú vị](https://tinystruggles.com/posts/google_postmortem/). Một kỹ sư SRE của Google đã xin nghỉ việc.

Công việc của cô ấy là vận hành và bảo trì máy chủ, thường xuyên phải viết báo cáo phân tích nguyên nhân (postmortem) mỗi khi hệ thống gặp sự cố. Lần này nghỉ việc, cô ấy tự viết cho mình một bản báo cáo phân tích nghỉ việc theo đúng phong cách đó.

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082015.webp)

Bài viết được viết vô cùng thẳng thắn, chia sẻ những suy nghĩ thực chất từ đáy lòng và tiết lộ rất nhiều thông tin nội bộ của Google. Lượng thông tin khá lớn, dưới đây tôi xin chia sẻ lại bản lược dịch (có cắt giảm một số phần để đảm bảo độ dài hợp lý).

**(1) Thông tin cơ bản của tôi.** Năm 2015, sau khi tốt nghiệp một trường đại học ở Ba Lan, tôi gia nhập Google và chuyển đến làm việc tại chi nhánh Ireland với vai trò kỹ sư SRE.

Khi mới vào làm, cấp bậc (level) của tôi là L3. Trong vòng 9 tháng, tôi được thăng lên L4. Một năm sau đó, tôi thăng lên L5 và hiện tại đang ở cấp bậc L6.

**(2) Tôi nhận được những gì từ Google.** Tôi chính thức nghỉ việc vào tuần này sau 9 năm gắn bó tại Google. Nhìn lại chặng đường đã qua, tôi đã tích lũy được rất nhiều giá trị.

Đầu tiên là tiền, tôi đã kiếm được một khoản tiền lớn.

Thứ hai, tôi có được các kỹ năng kỹ thuật phần mềm vững vàng, hiểu sâu sắc về kiến trúc hệ thống web quy mô lớn và phức tạp. Đồng thời, tôi cũng sở hữu những kỹ năng xử lý sự cố môi trường production và gỡ lỗi (debug) hệ thống máy chủ thuộc hàng top đầu thế giới.

Thứ ba, tôi học được các kỹ năng lãnh đạo và quản lý đội ngũ, đi kèm với đó là cảm giác tự hào khi là một phần của một tập đoàn công nghệ khổng lồ.

Cuối cùng là các chế độ phúc lợi tuyệt vời, từ văn phòng làm việc tiện nghi, bể bơi, phòng gym, các khóa học thể thao, dịch vụ mát-xa hằng tuần, cho đến các bữa ăn ngon miệng và lành mạnh, dịch vụ chăm sóc y tế cao cấp, cũng như các cơ hội đi công tác nước ngoài vô cùng thoải mái và thú vị.

**(3) Những thay đổi của Google.** Google ở thời điểm hiện tại đã thay đổi rất nhiều so với thời điểm tôi mới gia nhập, không còn giữ được sự thú vị và cá tính công nghệ độc đáo như xưa nữa.

Trước đây, công nghệ của Google luôn ở vị thế dẫn đầu tuyệt đối. Hiện tại, trình độ công nghệ của các công ty khác đang dần bắt kịp và thu hẹp khoảng cách với Google.

Ngân sách nội bộ của Google cũng liên tục bị cắt giảm, các chuyến đi công tác giảm đi đáng kể và làn sóng sa thải nhân sự diễn ra liên tục. Công ty cũng chuyển hướng tuyển dụng sang các khu vực có chi phí nhân công rẻ hơn. Điều này ảnh hưởng trực tiếp đến tôi khi tôi không được phép tuyển thêm người cho đội ngũ của mình nữa.

Nhiều năm qua, các quy định và hệ thống bảo mật nội bộ của Google liên tục gia tăng và ngày một trở nên rườm rào. Hệ thống hạ tầng nội bộ cũng như mối quan hệ phối hợp giữa các nhóm trở nên vô cùng phức tạp. Điều này làm chậm đáng kể tốc độ phát triển phần mềm và tạo ra nhiều thách thức kỹ thuật rất mệt mỏi.

Đối với chúng tôi, việc hiểu và nắm bắt toàn bộ hệ thống nội bộ của công ty đã trở thành một gánh nặng ngày một lớn. Bạn bắt buộc phải ghi nhớ vô số chi tiết kỹ thuật và hệ thống phức tạp, vì bất kỳ chi tiết nhỏ nào cũng có thể gây ảnh hưởng đến công việc của bạn (đặc biệt là với kỹ sư SRE). Một nhân sự mới vào phải mất tới cả năm trời mới có thể hiểu được hết những thứ này, thật là điên rồ.

Rất nhiều lúc, tôi cảm thấy bản thân bị ngộp thở bởi những cuộc họp triền miên, các công việc lặp đi lặp lại vô nghĩa, sự thiếu hụt nguồn lực của đội ngũ, trong khi lại không tìm thấy cơ hội phát triển bản thân rõ ràng.

Công ty từng hai lần hứa hẹn sẽ cho phép tôi mở rộng quy mô đội ngũ dưới quyền, nhưng cả hai lần quyết định đều bị hủy bỏ vào phút chót. Tôi cảm thấy công việc hiện tại không khai thác hết năng lực của mình, nhưng trong nội bộ công ty lại không tìm thấy vị trí nào phù hợp hơn để cống hiến.

Trong khi đó, các nhà quản lý cấp cao của Google không đưa ra sự hỗ trợ hay phản hồi định hướng nào, và hầu như thiếu sự giám sát sâu sát. Khi bạn hỏi họ về kế hoạch triển khai công việc tiếp theo, họ thường tỏ ra lúng túng và yêu cầu bạn tự tìm cách giải quyết.

**(4) Sự thay đổi trong tư duy của tôi.** Những thứ từng có sức hút rất lớn với tôi trước đây giờ đã không còn nhiều sức hấp dẫn nữa.

Tôi đã đạt và vượt các mục tiêu tài chính cá nhân tự đặt ra cho mình.

Sự đam mê của tôi đối với công nghệ của Google cũng nhạt dần. Các vấn đề kỹ thuật gặp phải trong công việc hằng ngày không còn mang lại cảm giác phấn khích như trước.

Sự quan tâm của tôi đã dịch chuyển sang các lĩnh vực khác. Vai trò kỹ sư SRE thực tế không thực sự phù hợp với sở thích và tính cách của tôi. Tôi là một người hướng đến sự lạc quan và sáng tạo, trong khi vị trí SRE lại yêu cầu tính cẩn trọng, bảo thủ và ổn định tuyệt đối. Ngoài ra, việc phải trực ca đêm liên tục trong thời gian dài đã hủy hoại giấc ngủ của tôi, và yêu cầu "on-call 24/7" khiến tôi rất khó để thực sự thả lỏng tâm trí sau giờ làm việc.

Tôi muốn luân chuyển khỏi bộ phận SRE để sang một vai trò khác, nhưng tại văn phòng Ireland lại không có nhiều vị trí khác để lựa chọn. Do tâm lý trì hoãn và các lý do cá nhân, tôi cũng không nộp đơn chuyển vùng sang các chi nhánh nước ngoài khác. Thành thật mà nói, Google là một công ty lấy nước Mỹ làm trung tâm. Chỉ cần bạn không làm việc tại trụ sở chính ở Mỹ, việc thúc đẩy bất kỳ kế hoạch nào cũng gặp nhiều khó khăn, và bạn rất dễ rơi vào cảm giác bị cô lập và bên lề hóa.

Tôi không nhìn thấy cơ hội thăng tiến lớn nào tại Google nữa. Tôi đã là kỹ sư cấp L6 — mức trần về mặt kỹ thuật chuyên môn thuần túy. Tôi không hào hứng với cấp L7 vì vị trí này thiên về vai trò chính trị và quản lý ngoại giao hơn là kỹ thuật thực chất, và cũng rất khó nói trước bạn sẽ quản lý bao nhiêu nhân sự dưới quyền. Nếu có cơ hội tự mình dẫn dắt một đội ngũ lớn, tôi có thể cân nhắc ở lại, còn không thì tôi khát khao tự mình khởi nghiệp hơn.

**(5) Những suy nghĩ khác.** Nhìn lại 9 năm qua, tôi vẫn cảm thấy bản thân vô cùng may mắn.

Giá cổ phiếu của Google tăng trưởng rất tốt, cộng thêm việc tôi thăng tiến nhanh và đạt hiệu suất công việc cao đã giúp tôi có được mức thu nhập rất tốt. Các quyết định tài chính cá nhân của tôi dựa trên nguồn thu nhập này cũng rất đúng đắn, mang lại nhiều quả ngọt về mặt đầu tư.

Tôi đã quen biết và xây dựng được mối quan hệ với rất nhiều đồng nghiệp giỏi tại Google. Những nhân sự do tôi tuyển dụng đều là những người rất đáng tin cậy.

Tất nhiên, tôi cũng có những điều tiếc nuối vì đã không thực hiện sớm hơn. Điều hối tiếc lớn nhất là đáng lẽ tôi nên rời khỏi bộ phận SRE và nộp đơn chuyển vùng sớm hơn. Ngay từ đầu tôi đã biết SRE không phải là công việc mình thực sự mong muốn, nhưng tôi chỉ thụ động ngồi chờ hoàn cảnh tự thay đổi. Kết quả là mọi thứ không như ý muốn. Giờ đây tôi đã hiểu ra bài học: bản thân phải chủ động tìm kiếm sự thay đổi.

## 微软工程师的薪资

Tuần trước, một [tờ báo Mỹ](https://www.businessinsider.com/microsoft-spreadsheet-shows-pay-engineers-2024-8) đã thu thập được một bảng tính điện tử ghi nhận dữ liệu lương thưởng do hơn 500 nhân viên Microsoft tự nguyện chia sẻ.

Tờ báo này đã tiến hành thống kê mức thu nhập trung bình của các kỹ sư Microsoft theo từng cấp bậc.

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082301.webp)

Bảng số liệu trên cho thấy bức tranh thu nhập thực tế của lập trình viên tại các tập đoàn công nghệ lớn của Mỹ trong năm 2024. Tại Microsoft, kỹ sư cấp bậc thấp nhất (Level 59) cũng có mức lương cơ bản vượt quá 120.000 USD hằng năm. Đây là mức thu nhập rất cao, tương đương với mức lương của một giáo sư thực thụ tại các trường đại học Mỹ.

Mức thu nhập của lập trình viên chủ yếu được quyết định bởi cấp bậc công việc (level), cấp bậc càng cao thì thu nhập càng lớn. Đó là lý do tại sao các kỹ sư tại các hãng công nghệ lớn luôn đặt mục tiêu thăng tiến lên hàng đầu.

Tuy nhiên, mức lương cơ bản giữa các cấp bậc không có sự chênh lệch quá lớn. Sự khác biệt chủ yếu nằm ở khoản tiền thưởng và cổ phiếu thưởng (RSU). Ở các cấp bậc cao, phần thu nhập biến động theo hiệu suất công việc này vượt xa so với mức lương cơ bản.

Tất nhiên, do quy mô mẫu khảo sát tương đối nhỏ nên bảng số liệu trên chắc chắn không phản ánh chính xác 100% thực tế, nhưng nó vẫn là một nguồn tham khảo rất có giá trị.

## [活动通知] 动手练习 AI 编程

Công cụ lập trình hỗ trợ bởi AI đang là xu hướng nóng hổi hiện nay, mọi người đều đang tìm cách ứng dụng AI vào quy trình viết mã nguồn.

Vào chiều mai (ngày 31 tháng 8), sẽ diễn ra một buổi workshop thực hành lập trình với AI do đội ngũ phát triển Doubao MarsCode chính thức tổ chức.

Doubao MarsCode là công cụ hỗ trợ lập trình AI của ByteDance với các tính năng thông minh như tự động tạo mã, hoàn thành mã và dự đoán thông minh. Tại sự kiện, **các kỹ sư ByteDance sẽ trực tiếp hướng dẫn 1-kèm-1** giúp các bạn thực hành hoàn thiện ý tưởng phát triển phần mềm của mình bằng AI.

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082807.webp)

Bạn có thể đăng ký tham gia theo nhóm (tối đa 3 người/nhóm) hoặc đăng ký cá nhân để cùng thiết kế và hoàn thiện một tựa game nhỏ ngay tại sự kiện với sự trợ giúp của AI.

Các kỹ sư sẽ túc trực để hướng dẫn và giải đáp mọi thắc mắc. Cuối buổi, **các nhóm sẽ trình bày sản phẩm của mình để ban giám khảo chấm điểm, trao giải và nhận những phần quà hấp dẫn**.

Đây là cơ hội thực hành tuyệt vời hoàn toàn miễn phí cho các bạn muốn trải nghiệm công nghệ lập trình AI. Sự kiện được tổ chức trực tiếp tại văn phòng TikTok Bắc Kinh.

Các bạn có thể click vào [liên kết này](https://www.bagevent.com/event/8901648?bag_track=ryf) hoặc quét mã QR trên poster để xem chi tiết và đăng ký tham gia. Nếu không ở Bắc Kinh, bạn vẫn có thể tham gia [chiến dịch viết bài chia sẻ](https://sourl.co/ZHGytq) về trải nghiệm sử dụng MarsCode với nhiều phần quà phong phú.

## 科技动态

1、[Tàu khí cầu chở khách AS700](https://www.sohu.com/a/802511112_121873449)

Vào lúc 6 giờ sáng ngày 20 tháng 8, chiếc tàu khí cầu chở khách AS700 của Trung Quốc đã cất cánh từ Kinh Môn, Hồ Bắc và thực hiện hành trình bay gần 1.000 km, tiếp đất an toàn tại Quế Lâm, Quảng Tây vào lúc 12 giờ trưa ngày hôm sau.

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082606.webp)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082607.webp)

Do có chặng dừng nghỉ trung gian để đội ngũ nghỉ ngơi, tổng thời gian bay thực tế trên không là 12 giờ 44 phút.

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082608.webp)

Sau khi đáp xuống Quế Lâm, tàu khí cầu bắt đầu chuỗi hoạt động bay trình diễn kéo dài 20 ngày kể từ ngày 23 tháng 8. Nếu du lịch Dương Sóc trong khoảng thời gian này, bạn sẽ thường xuyên bắt gặp chiếc tàu bay lơ lửng trên bầu trời vào mỗi buổi trưa.

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082609.webp)

Thiết bị có sức chứa tối đa 10 người (bao gồm 1 phi công), độ cao hành trình dao động từ 500m đến 2.000m, thời gian bay liên tục tối đa 10 giờ với tầm bay đạt 700 km.

Tàu bay chủ yếu phục vụ nhu cầu du lịch ngắm cảnh trên không, thậm chí hỗ trợ tổ chức các sự kiện độc đáo như "đám cưới trên mây". Do được bơm khí heli bên trong nên độ an toàn của thiết bị là rất cao.

2、[Kiểu mì Ý mới thiết kế bằng máy tính](https://kottke.org/21/03/the-invention-of-a-new-pasta-shape)

Để món mì Ý đạt hương vị ngon nhất, nước sốt bắt buộc phải bám dính đều trên sợi mì khi thưởng thức.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072612.webp)

Một người có tầm ảnh hưởng trên mạng xã hội tại Mỹ đã nảy ra ý tưởng thiết kế một hình dáng sợi mì Ý hoàn toàn mới nhờ sự trợ giúp của máy tính.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072613.webp)

Sợi mì mới được tính toán để tối đa hóa các nếp gấp lượn sóng trên bề mặt, giúp giữ được lượng nước sốt nhiều nhất có thể khi trộn, đồng thời vẫn bảo đảm độ dai giòn tối ưu để mang lại cảm giác ngon miệng nhất khi nhai.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072614.webp)

Mỗi gói mì Ý độc đáo này có giá bán khá đắt, lên tới hơn 200 nhân dân tệ nhưng đã nhanh chóng cháy hàng ngay khi vừa mở bán.

3、[Máy tính xách tay màn hình gập đôi](https://arstechnica.com/gadgets/2024/08/acemagics-x1-is-a-clever-but-delicate-approach-to-dual-screen-laptops/)

Một công ty công nghệ tại Thâm Quyến đã giới thiệu dòng máy tính xách tay màn hình gập độc đáo tích hợp hai màn hình ghép nối trực tiếp.

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082501.webp)

Các dòng máy tính hai màn hình trước đây hầu hết đều loại bỏ bàn phím vật lý, bắt buộc người dùng phải gõ trên màn hình cảm ứng phụ hoặc sử dụng bàn phím rời bên ngoài.

Tuy nhiên, chiếc máy tính này đã giải quyết bài toán bằng cách thiết kế hệ thống bản lề gập mở linh hoạt nối hai màn hình lại với nhau.

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082502.webp)

Nhờ đó, màn hình thứ hai có thể gập ngược 360 độ áp sát vào mặt lưng của màn hình chính (ảnh trên), hoặc mở rộng sang bên trái để hoạt động như một màn hình phụ độc lập (ảnh dưới).

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082503.webp)

Theo trải nghiệm thực tế từ người dùng, màn hình phụ bên trái hỗ trợ rất tốt cho công việc đa nhiệm. Tuy nhiên, kết cấu này làm trọng tâm máy hơi mất cân bằng, khiến màn hình phụ có hiện tượng rung nhẹ khi người dùng gõ phím mạnh tay.

Sản phẩm này chứng minh rằng ngay cả với những dòng thiết bị công nghệ đã bão hòa như laptop thì vẫn luôn tồn tại không gian sáng tạo mở cho các kỹ sư.

4、**Các tin tức khác**

(1) Dòng sản phẩm [iPhone 16 Series](https://www.idownloadblog.com/2024/08/22/iphone-16-jpeg-xl-rumor/) được dự báo sẽ hỗ trợ định dạng hình ảnh mới JPEG-XL, giúp tiết kiệm dung lượng lưu trữ xuống chỉ còn 1/3 so với định dạng JPEG truyền thống.

(2) Theo thống kê của [Trung tâm Thông tin Mạng Internet Trung Quốc](https://china.chinadaily.com.cn/a/202408/29/WS66d00abba310b35299d39168.html) (CNNIC), tính đến cuối tháng 6, tổng số tên miền đăng ký tại nước này đạt 31,87 triệu tên miền, trong đó tên miền quốc gia `.cn` chiếm tới 19,56 triệu.

Báo cáo cũng chỉ ra tỷ lệ người dùng internet Trung Quốc xem video ngắn đạt 95,5%, trong khi tỷ lệ xem video dài truyền thống là 65,2%.

## 文章

1、[Hình ảnh giải thích trực quan về giao thức xác thực SAML](https://www.sheshbabu.com/posts/visual-explanation-of-saml-authentication/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072503.webp)

SAML là giao thức xác thực danh tính phổ biến được sử dụng rộng rãi trong các doanh nghiệp lớn phục vụ giải pháp đăng nhập một lần (SSO). Bài viết giải thích chi tiết khái niệm này.

2、[Tùy biến bảng biểu (table) bằng các thuộc tính CSS hiện đại](https://piccalil.li/blog/styling-tables-the-modern-css-way/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072504.webp)

Hướng dẫn cách khai thác các thuộc tính CSS hiện đại để thiết kế kiểu dáng đẹp mắt và chuyên nghiệp cho thẻ `<table>` trên trang web.

3、[Quy trình thiết kế biểu tượng loading dạng chuyển động bằng SVG](https://www.fffuel.co/svg-spinner/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072508.webp)

Bài viết hướng dẫn từng bước viết mã nguồn SVG để tạo nên một biểu tượng vòng quay tải dữ liệu (spinner loading) chuyển động mượt mà.

4、[Tại sao sử dụng ký tự viết thường giúp giảm dung lượng tệp tin nén](https://endtimes.dev/why-lowercase-letters-save-data/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072512.webp)

Bài viết phân tích nguyên lý thuật toán nén dữ liệu để giải thích tại sao việc chuyển đổi toàn bộ ký tự viết hoa sang viết thường lại giúp giảm kích thước tệp tin sau khi nén.

5、[Khám phá cấu trúc bên trong thư mục ẩn `.git`](https://jvns.ca/blog/2024/01/26/inside-git/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072610.webp)

Toàn bộ dữ liệu lịch sử và metadata của dự án Git được lưu trữ trong thư mục ẩn `.git`. Bài viết giải thích chi tiết vai trò và chức năng của từng thư mục con và tệp tin bên trong nó.

6、[Quy ước thiết kế hộp kiểm checkbox hình vuông](https://tonsky.me/blog/checkbox/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072611.webp)

Tác giả lập luận các nhà thiết kế UI/UX cần tuân thủ nghiêm ngặt quy ước giao diện cơ bản: hộp kiểm cho phép chọn nhiều (checkbox) bắt buộc phải là hình vuông, còn nút chọn một (radio button) phải là hình tròn để tránh gây nhầm lẫn cho người dùng.

## 工具

1、[Coolify](https://github.com/coollabsio/coolify)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082701.webp)

Nền tảng hỗ trợ triển khai và vận hành ứng dụng nguồn mở, được đánh giá là giải pháp tự triển khai (self-hosted) thay thế hoàn hảo cho các dịch vụ đám mây trả phí như Heroku, Netlify hay Vercel.

2、[Ente Auth](https://ente.io/auth/)

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024052603.webp)

Ứng dụng quản lý mã xác thực hai lớp (2FA) nguồn mở an toàn.

3、[Marsview](https://github.com/JackySoft/marsview)

Một nền tảng thiết kế giao diện trực quan low-code hỗ trợ xây dựng nhanh các hệ thống quản trị nội bộ (admin dashboard). (Đóng góp từ [@JackySoft](https://github.com/ruanyf/weekly/issues/5060))

4、[Notion Exporter](https://notionexporter.com/)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082808.webp)

Tiện ích mở rộng trình duyệt hỗ trợ xuất nhanh nội dung ghi chú trên Notion thành hình ảnh dài hoặc thẻ card chia sẻ mà vẫn bảo toàn định dạng căn lề ban đầu. (Đóng góp từ [@Shanshi66](https://github.com/ruanyf/weekly/issues/5079))

5、[Battery Indicator](https://deepesh-01.github.io/battery_indicator/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112807.webp)

Trang web ứng dụng một đoạn mã ngắn đơn giản (đọc thêm [mã nguồn](https://deepesh-01.github.io/battery_indicator/app.js)) để hiển thị phần trăm dung lượng pin hiện tại của thiết bị truy cập.

6、[tsimp](https://github.com/tapjs/tsimp)

Thư viện hỗ trợ Node.js chạy và thực thi trực tiếp các tệp tin script viết bằng ngôn ngữ TypeScript mà không cần biên dịch thủ công sang JS trước.

7、[xpano](https://github.com/krupkat/xpano)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112905.webp)

Công cụ nguồn mở hỗ trợ ghép nối tự động nhiều bức ảnh đơn lẻ thành một bức ảnh toàn cảnh (panorama) góc rộng.

8、[concrete.css](https://concrete.style/)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024020806.webp)

Thư viện CSS tối giản không sử dụng class (classless CSS), lấy cảm hứng thiết kế từ hai thư viện Milligram và Skeleton.

9、[Person Diagram](https://peoplegraphmaker.com/)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024020108.webp)

Ứng dụng web giải trí hỗ trợ thiết kế nhanh các biểu đồ tỷ trọng dân số trực quan trực tuyến.

## AI 相关

1、[Mô hình chuyển đổi văn bản bạch thoại sang văn ngôn (chữ Hán cổ)](https://modelscope.cn/studios/chostem/ancient_Chinese_text_generator)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082511.webp)

Nhập các câu tiếng Trung hiện đại để mô hình AI tự động chuyển dịch sang văn phong chữ Hán cổ đại phong cách tao nhã, [mã nguồn mở](https://github.com/JianXiao2021/ancient_text_generation_LLM). (Đóng góp từ [@JianXiao2021](https://github.com/ruanyf/weekly/issues/5057))

2、[Linly-Dubbing](https://github.com/Kedreamix/Linly-Dubbing)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082805.webp)

Công cụ AI nguồn mở hỗ trợ dịch và lồng tiếng tự động cho video, chuyển đổi âm thanh tiếng nước ngoài sang tiếng Trung. (Đóng góp từ [@Y024](https://github.com/ruanyf/weekly/issues/5074))

3、[kotaemon](https://github.com/Cinnamon/kotaemon)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082806.webp)

Giao diện đồ họa cục bộ nguồn mở hỗ trợ người dùng tương tác trò chuyện (chat RAG) trực tiếp trên các tài liệu văn bản cá nhân thông qua các mô hình AI chỉ định. (Đóng góp từ [@Y024](https://github.com/ruanyf/weekly/issues/5075))

4、[Watson AI](https://www.guillaume.sh/watson)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082504.webp)

Phần mềm máy tính nguồn mở hỗ trợ thu âm các buổi họp trực tuyến qua microphone của hệ thống, sau đó ứng dụng AI để tự động biên soạn biên bản cuộc họp và tóm tắt nội dung cốt lõi.

5、[Fluximg.com](https://fluximg.com/)

Dịch vụ tạo ảnh nghệ thuật trực tuyến miễn phí sử dụng mô hình AI tạo ảnh thế hệ mới Flux. (Đóng góp từ [@youyuela](https://github.com/ruanyf/weekly/issues/5055))

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082510.webp)

## 资源

1、[Hồ sơ yêu quái Hắc Thần Thoại: Ngộ Không (妖怪平生录)](https://github.com/meethigher/black-wukong-youji/blob/master/%E9%BB%91%E7%A5%9E%E8%AF%9D%E6%82%9F%E7%A9%BA%E5%A6%96%E6%80%AA%E5%B9%B3%E7%94%9F%E5%BD%95.md)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082705.webp)

Kho lưu trữ hình ảnh minh họa kèm theo các bài thơ giới thiệu và câu chuyện truyền thuyết của toàn bộ 203 loài yêu quái xuất hiện trong trò chơi "Hắc Thần Thoại: Ngộ Không". (Đóng góp từ [@meethigher](https://github.com/ruanyf/weekly/issues/5063))

2、[Emoji Spark](https://emojispark.com/)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082801.webp)

Công cụ trực tuyến hỗ trợ tìm kiếm và đối chiếu nhanh các biểu tượng cảm xúc Emoji phù hợp với ngữ cảnh. (Đóng góp từ [@0xjoanne](https://github.com/ruanyf/weekly/issues/5067))

3、[Sách học vi tích phân bằng ngôn ngữ Julia](https://jverzani.github.io/CalculusWithJuliaNotes.jl/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024060509.webp)

Giáo trình toán học trực tuyến giới thiệu các khái niệm vi tích phân từ cơ bản (giới hạn), tích hợp minh họa tính toán thực tế bằng ngôn ngữ Julia.

4、[Thư viện phim tài liệu miễn phí (ihavenotv.com)](https://ihavenotv.com/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011601.webp)

Trang web hỗ trợ xem trực tuyến miễn phí lượng lớn phim tài liệu khoa học và lịch sử bằng tiếng Anh.

## 图片

1、[Mô phỏng tai nạn thử nghiệm hạt nhân chết người](https://www.bbc.com/future/article/20230725-making-the-blue-flash-how-i-reconstructed-a-fatal-atomic-accident)

Vào năm 1946, một vụ tai nạn phóng xạ nghiêm trọng đã xảy ra tại Phòng thí nghiệm Quốc gia Los Alamos ở Mỹ — nơi nghiên cứu và chế tạo bom nguyên tử.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072903.webp)

Nhà vật lý hạt nhân Louis Slotin khi dẫn các đồng nghiệp đi tham quan phòng thí nghiệm đã quyết định thực hiện một thao tác biểu diễn trực quan để chỉ ra "trạng thái tới hạn" của lõi bom.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072904.webp)

Ông sử dụng một chiếc tua-vít dẹt để kê nghiêng nửa bán cầu bằng kim loại beryli bao quanh lõi plutoni bên trong.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072905.webp)

Tuy nhiên, chiếc tua-vít bất ngờ bị trượt tay, khiến nửa bán cầu beryli sập hoàn toàn chụp lên lõi plutoni, ngay lập tức kích hoạt phản ứng hạt nhân dây chuyền phát ra bức xạ cực mạnh.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072906.webp)

Ông đã phản ứng cực kỳ nhanh khi dùng tay không hất văng bán cầu beryli ra để cứu sống các đồng nghiệp xung quanh. Tuy nhiên bản thân ông đã hấp thụ lượng bức xạ chết người và qua đời chỉ 9 ngày sau đó.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072907.webp)

Dưới đây là mô hình phục dựng lại chi tiết hiện trường vụ tai nạn phóng xạ năm đó do một nghệ sĩ người Anh thiết kế tỉ mỉ.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072908.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072909.webp)

## 文摘

1、[Cả nhân loại xếp vừa một tòa nhà nhỏ](https://waitbutwhy.com/2015/03/7-3-billion-people-one-building.html)

Tổng dân số trên Trái Đất hiện nay đạt khoảng 8,17 tỷ người.

Vào 10 năm trước (năm 2014), tổng dân số thế giới đạt mốc 7,3 tỷ người.

Thời điểm đó, một tác giả đã thực hiện phép tính thú vị để chỉ ra rằng: dù 7,3 tỷ người nghe có vẻ là con số khổng lồ, nhưng quy mô vật lý của nó thực chất nhỏ hơn chúng ta tưởng tượng rất nhiều.

If mỗi con người được đại diện bằng một hạt gạo nhỏ, thì toàn bộ 7,3 tỷ hạt gạo này sẽ xếp vừa vặn trong một khối lập phương có chiều dài cạnh là 6,1 mét — tương đương với thể tích của một căn nhà hai tầng nhỏ.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024052604.webp)

Còn nếu mỗi người được đại diện bằng một hạt cát siêu nhỏ, thì toàn bộ 7,3 tỷ hạt cát này sẽ nằm gọn gàng bên trong một chai nước ngọt dung tích 2 lít.

Dưới góc nhìn của hành tinh Trái Đất, loài người thực chất chỉ nhỏ bé như một hạt gạo hay hạt cát lơ lửng. Xã hội loài người náo nhiệt hằng ngày mà chúng ta luôn coi là trung tâm của vũ trụ, thực chất chỉ tương đương với những gì diễn ra bên trong một căn nhà nhỏ hay một chai nước ngọt mà thôi.

## 言论

1、

Hỏi: Nếu tốc độ kết nối internet tăng lên tới mức 1 Tb/s, mạng lưới internet sẽ thay đổi ra sao?

Đáp: Chúng ta sẽ phải xem nhiều quảng cáo hơn, với kích thước lớn hơn và tốc độ hiển thị nhanh hơn.

-- [Ý kiến độc giả trên diễn đàn Hacker News](https://news.ycombinator.com/item?id=41332413)

2、

Mọi người thường coi Nvidia là một công ty chuyên bán phần cứng GPU (card đồ họa), nhưng thực chất sản phẩm cốt lõi giữ chân khách hàng của họ là thư viện phần mềm tính toán CUDA. GPU thực ra chỉ là phần linh kiện độc quyền đi kèm bắt buộc phải mua với giá đắt đỏ để chạy thư viện đó mà thôi.

-- [Ý kiến độc giả trên diễn đàn Hacker News](https://news.ycombinator.com/item?id=41361597)

3、

Tôi cực kỳ không thích nghe các bài thuyết trình kỹ thuật trực tiếp tại hội thảo, vì 95% trong số đó mang lại rất ít giá trị. Tôi ưu tiên xem video ghi hình lại buổi thuyết trình hơn. Bằng cách đó, tôi có thể dừng lại để suy nghĩ kỹ lưỡng, tăng tốc độ phát lên 1,5x hoặc 2x để tiết kiệm thời gian, hoặc nhanh chóng bỏ qua nếu nội dung không thực sự chất lượng.

-- [《Kinh nghiệm chuẩn bị bài thuyết trình kỹ thuật》](https://chelseatroy.com/2022/08/03/how-i-do-and-dont-prepare-a-talk-for-a-technical-conference/)

4、

Việc hạ cánh thẳng đứng của các thiết bị vũ trụ lên bề mặt Mặt Trăng là vô cùng thách thức. Gần đây, cả tàu đổ bộ của Mỹ và Nhật Bản đều gặp sự cố bị lật nghiêng khi tiếp đất. Nguyên nhân chính là do trọng lực trên Mặt Trăng chỉ bằng 1/6 so với Trái Đất, khiến các thiết bị chỉ cần có trọng tâm hơi lệch một chút là rất dễ bị lật úp.

-- [《Tại sao đổ bộ Mặt Trăng thẳng đứng lại khó khăn đến vậy》](https://www.nytimes.com/2024/03/04/science/moon-landing-sideways-gravity.html)

5、

Tuyên ngôn Agile đề ra 4 tôn chỉ cốt lõi, trong đó có quy định: "Phần mềm chạy tốt quan trọng hơn tài liệu hướng dẫn đầy đủ".

Hệ quả thực tế của tôn chỉ này là các dự án phát triển theo mô hình Agile thường có hệ thống tài liệu hướng dẫn cực kỳ sơ sài. Một nghiên cứu thống kê chỉ ra rằng các dự án áp dụng mô hình Agile có tỷ lệ thất bại cao hơn tới 268% so với các dự án truyền thống không áp dụng Agile.

-- [theregister.com](https://www.theregister.com/2024/06/05/agile_failure_rates/)

## 往年回顾

[Năng suất là từ dùng cho máy móc, không phải cho con người](https://www.ruanyifeng.com/blog/2023/08/weekly-issue-268.html) (2023 #268)

[Rượu vang, hoa anh đào và biến đổi khí hậu](https://www.ruanyifeng.com/blog/2022/08/weekly-issue-218.html) (2022 #218)

[Trải nghiệm tựa game "Detroit: Become Human"](https://www.ruanyifeng.com/blog/2021/07/weekly-issue-168.html) (2021 #168)

[Kinh nghiệm chọn nguyện vọng thi đại học](https://www.ruanyifeng.com/blog/2020/07/weekly-issue-118.html) (2020 #118)

(Hết)
