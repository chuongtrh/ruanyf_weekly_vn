# Bản tin chia sẻ công nghệ (Số 324): Số nguyên tố lớn nhất loài người từng biết

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/5445) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110209.webp)

Bảo tàng Louvre — một trong những bảo tàng nghệ thuật lớn nhất thế giới — có một phân nhánh nổi tiếng tại Abu Dhabi, Các Tiểu vương quốc Ả Rập Thống nhất. Phân nhánh này được xây dựng trên một hòn đảo nhân tạo xinh đẹp, nơi du khách có thể chèo thuyền kayak để đi tham quan xung quanh bảo tàng. (Nguồn: [Visit Abu Dhabi](https://visitabudhabi.ae/zh/what-to-see/historical-and-cultural-attractions/louvre-abu-dhabi))

## 人类已知的最大质数

Tháng trước, có một phát hiện khoa học ít được chú ý nhưng rất đặc biệt: **Số nguyên tố lớn nhất mà nhân loại từng biết đến đã chính thức lộ diện**.

Ngoại trừ các nhà toán học, có lẽ hầu hết mọi người đều không mặn mà với tin tức này bởi nó dường như nằm quá xa rời cuộc sống sinh hoạt hằng ngày.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110708.webp)

Thế nhưng mới đây, tờ *The Washington Post* đã đăng tải [một phóng sự](https://www.washingtonpost.com/science/2024/10/23/nvidia-prime-mersenne-gpu-cloud/) kéo gần khoảng cách của phát hiện toán học khô khan này đến gần hơn với độc giả phổ thông.

Điều bất ngờ lớn nhất là: **Người phát hiện ra con số kỷ lục này không phải là một giáo sư toán học chuyên nghiệp, mà là một kỹ sư lập trình**. Tờ *The Washington Post* đã khai thác câu chuyện hậu trường vô cùng kịch tính và hấp dẫn này. Bản thân tôi khi đọc cũng thấy vô cùng phấn khích. Dưới đây tôi xin chia sẻ lại nội dung câu chuyện với các bạn.

---

Vào ngày 10 tháng 10 năm 2024, một lập trình viên người Mỹ tên là Luke Durant đã tìm ra số nguyên tố lớn nhất từng được biết đến trong lịch sử loài người.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110703.webp)

Tối hôm đó, anh đang thu xếp hành lý cá nhân để chuẩn bị cho chuyến bay từ bang California trở về quê nhà Alabama. Trước khi khóa cửa ra đi, anh quyết định thực hiện truy cập từ xa vào máy chủ để kiểm tra tình trạng hoạt động của các tập lệnh (script) tính toán đang chạy ngầm.

Anh cứ ngỡ kết quả lần này cũng sẽ giống hệt như hàng vạn lần kiểm tra trước đó trong suốt một năm qua: hoặc là hệ thống chưa chạy xong, hoặc là phát sinh các lỗi kết nối. Nhưng lần này đã khác, màn hình máy tính hiển thị dòng trạng thái tính toán thành công.

Durant lập tức nhận ra mình vừa chạm tay vào một cột mốc lịch sử khi tìm ra số nguyên tố lớn nhất thế giới mới. Anh lập tức gửi tin nhắn thông báo cho các cộng sự của mình, quyết định hủy bỏ chuyến bay về quê và lập tức ngồi xuống đối chiếu chi tiết các dữ liệu đầu ra của máy chủ.

Số nguyên tố kỷ lục mà anh tìm thấy sau đó được cộng đồng đặt tên mã hiệu là **M136279841**. Độ lớn của con số này vượt xa mọi trí tưởng tượng thông thường khi sở hữu tới **41.024.320 chữ số** ở hệ thập phân. Nếu bạn thực hiện đọc to từng chữ số của nó liên tục với tốc độ 1 chữ số mỗi giây, bạn sẽ phải mất tới 475 ngày ròng rã mới có thể đọc hết con số này. Nó có giá trị toán học bằng: 2<sup>136.279.841</sup> - 1.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110704.webp)

Để tìm ra con số lịch sử này, Durant đã phải làm việc ròng rã suốt một năm trời, đồng thời tự bỏ tiền túi lên tới khoảng **2 triệu USD** để thuê dịch vụ tính toán đám mây GPU nhằm chạy các thuật toán tìm kiếm.

Luke Durant năm nay 36 tuổi, từng có thời gian dài làm kỹ sư phần mềm tại tập đoàn công nghệ Nvidia. Làn sóng tăng giá cổ phiếu phi mã của Nvidia đã giúp anh tích lũy được một khoản tài chính lớn, giúp anh có thể tự tin xin nghỉ việc vào năm 2021 để tập trung toàn lực nghiên cứu các dự án cá nhân yêu thích.

Và dự án mà anh lựa chọn dấn thân chính là tìm kiếm các số nguyên tố Mersenne. Kinh nghiệm nhiều năm làm việc tại Nvidia đã giúp anh làm chủ kỹ thuật lập trình song song tối ưu hóa hiệu năng tính toán trên GPU để giải các bài toán tốc độ cao.

Vào thế kỷ 17, tu sĩ người Pháp Marin Mersenne đã đưa ra giả thuyết rằng tồn tại vô số các số nguyên tố có cấu trúc biểu diễn dưới dạng 2<sup>n</sup> - 1 (ví dụ như: 3 = 2<sup>2</sup> - 1, hay 7 = 2<sup>3</sup> - 1).

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110705.webp)

Tính đến nay, nhân loại mới chỉ tìm thấy tổng cộng 52 số nguyên tố Mersenne (bao gồm cả số nguyên tố kỷ lục mà Durant vừa tìm ra). Việc tìm kiếm các số nguyên tố Mersenne thế hệ mới từ lâu đã trở thành một trò chơi trí tuệ đầy lôi cuốn của cộng đồng yêu toán học toàn cầu.

Vào những năm 90 của thế kỷ trước, cùng với sự phổ cập của mạng Internet, lập trình viên người Mỹ George Woltman đã đứng ra khởi xướng dự án tìm kiếm số nguyên tố Mersenne quy mô toàn cầu mang tên GIMPS (Great Internet Mersenne Prime Search).

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110706.webp)

Mục tiêu của dự án GIMPS là phát triển các phần mềm mã nguồn mở để tận dụng sức mạnh máy tính tìm kiếm số nguyên tố Mersenne. Trang web chính thức của dự án ([mersenne.org](http://www.mersenne.org/)) cung cấp các phần mềm miễn phí để mọi người tải về cài đặt lên máy tính cá nhân. Phần mềm sẽ tự động tận dụng các khoảng thời gian nhàn rỗi của bộ vi xử lý máy tính để thực hiện các phép toán tìm kiếm.

Hiện nay, mạng lưới GIMPS thu hút khoảng 3.000 đến 5.000 tình nguyện viên toàn cầu tham gia chạy phần mềm thường trực. Tuy nhiên, do các phép toán tìm kiếm số nguyên tố Mersenne có độ phức tạp lũy thừa cực kỳ khủng khiếp, trong suốt 28 năm hoạt động vừa qua, toàn bộ mạng lưới GIMPS cũng chỉ mới tìm ra vỏn vẹn 18 số nguyên tố mới.

Số nguyên tố gần đây nhất được tìm thấy vào năm 2018, và nó có độ dài ngắn hơn số nguyên tố thứ 52 của Durant tới 16 triệu chữ số thập phân.

Điểm khác biệt mang tính đột phá của Luke Durant so với tất cả các tình nguyện viên đi trước là: Trong khi toàn bộ mạng lưới từ trước đến nay đều sử dụng CPU để tính toán, thì anh là người duy nhất chuyển đổi thành công thuật toán sang chạy trên GPU. Hiệu năng vượt trội của GPU giúp xử lý khối lượng công việc tính toán của CPU trong một đến hai tuần chỉ trong vòng vỏn vẹn một đến hai ngày.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110709.webp)

Để tìm ra con số kỷ lục này, Durant đã huy động và cấu hình chạy song song hệ thống máy chủ đặt tại 24 trung tâm dữ liệu thuộc 17 quốc gia/vùng lãnh thổ khác nhau thông qua hai nhà cung cấp dịch vụ đám mây lớn.

Anh chia sẻ: "Trong kỷ nguyên hiện nay, năng lực hành động của một cá nhân đã được phóng đại mạnh mẽ hơn bao giờ hết nhờ công nghệ. Quy mô hạ tầng điện toán đám mây mà bạn có thể thuê và vận hành là vô cùng khủng khiếp. Chúng ta đang sở hữu những công cụ công nghệ mạnh mẽ chưa từng có trong lịch sử, vì vậy điều tốt nhất là hãy tìm cách khai thác chúng phục vụ sự phát triển tri thức."

Thực tế, việc tìm ra các số nguyên tố Mersenne khổng lồ không mang lại giá trị ứng dụng thực tiễn trực tiếp nào cho đời sống. Các nhà khoa học dấn thân tìm kiếm chúng đơn giản chỉ vì niềm vui chinh phục thử thách và khát vọng mở rộng biên giới tri thức của nhân loại.

Nhờ phát hiện lịch sử này, Durant đã nhận được khoản tiền thưởng trị giá 3.000 USD từ dự án GIMPS. Anh đã quyết định quyên tặng toàn bộ số tiền này cho trường trung học nội trú công lập Alabama — ngôi trường cũ của anh trước khi anh thi đỗ vào Viện Công nghệ California (Caltech).

Dù số nguyên tố mới của Durant đã đạt độ dài tới 41 triệu chữ số, dự án GIMPS hiện vẫn đang treo giải thưởng lớn dành cho người đầu tiên tìm ra số nguyên tố Mersenne có độ dài đạt mốc 1 tỷ chữ số thập phân.

## 活动

Tuần này có hai hoạt động rất thú vị dành cho các bạn đam mê công nghệ.

## 豆包 MarsCode 校园发布会

Các bạn sinh viên nên học tập và ứng dụng AI như thế nào để nâng cao năng lực cạnh tranh cá nhân? Khi gặp khó khăn trong quá trình học tập lập trình thì giải quyết ra sao? Và làm thế nào để có thể tìm kiếm được cơ hội việc làm tốt trong ngành công nghệ sau khi ra trường?

Đây đều là những nỗi băn khoăn rất lớn của phần lớn các bạn học sinh, sinh viên hiện nay.

Thấu hiểu điều đó, trợ lý lập trình thông minh [Doubao MarsCode](https://www.marscode.cn/) của tập đoàn ByteDance đã chính thức khởi động chương trình đồng hành cùng giảng đường đại học với [chuỗi sự kiện hấp dẫn](https://www.marscode.cn/events/campus). Chương trình cung cấp các khóa học miễn phí, các cuộc thi lập trình thực tế, và chương trình tìm kiếm gương mặt đại sứ công nghệ (MVP) nhằm hỗ trợ các bạn trẻ định hình hướng đi tương lai.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110712.webp)

Vào chiều thứ Bảy tuần tới (ngày 16 tháng 11), chương trình sẽ tổ chức buổi livestream ra mắt chính thức. Bên cạnh việc giới thiệu các hoạt động hỗ trợ sinh viên, buổi phát sóng còn có sự góp mặt chia sẻ kinh nghiệm thực tế từ các anh chị khóa trên xuất sắc của các trường đại học lớn, cùng các buổi tọa đàm với chuyên gia công nghệ của Doubao MarsCode về định hướng nghề nghiệp trong kỷ nguyên AI.

Cổng đăng ký tham gia sự kiện đã chính thức mở từ hôm nay. Ban tổ chức đã chuẩn bị rất nhiều chương trình tương tác hấp dẫn: **các giải thưởng tương tác hằng ngày, bốc thăm may mắn trong nhóm chat, và chương trình quay số trúng thưởng lớn trực tiếp trong buổi livestream** với các phần quà công nghệ giá trị.

Các bạn quan tâm có thể quét mã QR trên poster hoặc truy cập vào [liên kết này](https://live.marscode.cn/7116/campus?ch=ryf) để xem chi tiết thể lệ và đăng ký tham gia.

## [竞赛] 扣子 AI 挑战赛

Nền tảng tạo chatbot AI chuyên nghiệp Coze (扣子) của ByteDance đang tổ chức cuộc thi [Thử thách thiết kế Mẫu Template thông minh (扣子模板挑战赛)](https://mp.weixin.qq.com/s/CRxT9UTuD1dH53ePwi-_Zw).

Trước ngày 22 tháng 11, bạn chỉ cần thiết kế và xây dựng một ứng dụng AI trên Coze và xuất bản thành công lên [Cửa hàng ứng dụng thông minh (Coze Store)](https://www.coze.cn/store/agent?cate_type=recommend) là đã đủ điều kiện tham gia cuộc thi.

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024102812.webp)

Quét mã QR trên poster hoặc [click vào đây](https://www.coze.cn/s/iANJPSxo/) để xem chi tiết thể lệ cuộc thi.

Các bạn không cần quá lo lắng về rào cản kỹ thuật. Nền tảng Coze hoạt động trên cơ chế lập trình dạng luồng công việc (Workflow) trực quan (bạn có thể tham khảo [bài viết giới thiệu của tôi](http://www.ruanyifeng.com/blog/2024/10/coze.html) hoặc [tài liệu hướng dẫn chính thức](https://www.coze.cn/docs/guides/quickstart)). Với giao diện kéo thả đồ họa, người dùng hoàn toàn có thể tự liên kết các khối tính năng để tạo ra ứng dụng AI cho riêng mình mà không cần biết viết code.

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024102708.webp)

Đặc biệt, Coze tuần này đã chính thức ra mắt tính năng thương mại hóa Mẫu Template trả phí. Bạn hoàn toàn có thể đặt giá bán cho các mẫu ứng dụng do mình thiết kế. Những người dùng khác muốn sao chép và chỉnh sửa ứng dụng dựa trên mẫu của bạn sẽ phải trả phí mua template, tạo ra nguồn thu nhập thụ động trực tiếp cho bạn.

**Ban tổ chức cuộc thi sẽ dựa trên số lượng lượt sao chép sử dụng của template để trao các giải thưởng tiền mặt trị giá từ 1.000 đến 10.000 nhân dân tệ**. Việc xây dựng ứng dụng trên Coze là hoàn toàn miễn phí, các bạn hãy thử ghé thăm cửa hàng ứng dụng tìm kiếm ý tưởng và trải nghiệm xây dựng ứng dụng AI bằng giải pháp low-code đầy thú vị này.

## 科技动态

1、[Hộp ngủ胶囊 tại San Francisco](https://www.theguardian.com/society/2024/oct/31/san-francisco-sleeping-pods-affordable-housing-crisis)

Một khu nhà trọ dạng hộp ngủ (sleeping pods) cho thuê theo tháng tại trung tâm thành phố San Francisco đang trở nên cực kỳ đắt khách. Do nhu cầu thuê quá lớn, người thuê bắt buộc phải đăng ký trực tuyến trước để tham gia vòng quay số may mắn.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110201.webp)

Thống kê cho thấy đã có tới hơn 300 hồ sơ đăng ký cạnh tranh cho vỏn vẹn 17 vị trí giường ngủ trống của cơ sở.

Mỗi chiếc giường ngủ dạng hộp xếp tầng này có mức giá thuê hằng tháng là 700 USD (khoảng 17 triệu VNĐ), đã bao gồm toàn bộ chi phí điện nước, internet tốc độ cao, quyền sử dụng nhà tắm công cộng, nhà vệ sinh, một tủ đồ khóa riêng và khu bếp chung của tòa nhà.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110202.webp)

Sở dĩ một không gian sống chật hẹp và đắt đỏ như vậy vẫn luôn trong tình trạng cháy phòng là bởi vì tại San Francisco, bạn hầu như không thể tìm kiếm được bất kỳ địa điểm lưu trú nào có mức giá rẻ hơn như vậy.

Sự bùng nổ của Thung lũng Silicon đã đẩy giá bất động sản tại San Francisco lên mức đắt đỏ bậc nhất nước Mỹ. Giá thuê một phòng đơn合租 trong căn hộ thông thường tại đây đã dao động ở mức từ 3.000 đến 3.500 USD/tháng, vượt quá khả năng tài chính của đại bộ phận người lao động phổ thông Mỹ.

2、[Sự cố triển khai hệ thống Oracle tại Birmingham](https://www.theregister.com/2024/08/20/birmingham_oracle_cost/)

Vào năm 2022, chính quyền thành phố Birmingham (Anh) đã quyết định thực hiện nâng cấp toàn bộ hệ thống quản trị doanh nghiệp (ERP) của thành phố, lựa chọn giải pháp của hãng Oracle để thay thế cho hệ thống cũ của SAP đã vận hành ổn định suốt hơn 20 năm qua.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110501.webp)

Tuy nhiên, ngay sau khi đưa hệ thống mới vào vận hành, ban quản lý mới tá hỏa phát hiện phần mềm Oracle không có năng lực tự động kết xuất các báo cáo kiểm toán dòng tiền mặt của thành phố. Tình thế bắt buộc chính quyền thành phố phải huy động nhân sự thực hiện kiểm toán thủ công bằng tay.

Chi phí triển khai nâng cấp hệ thống Oracle từ mức dự toán ban đầu là 19 triệu bảng Anh (khoảng 600 tỷ VNĐ) nay đã đội vốn lên tới 131 triệu bảng Anh (khoảng 4.200 tỷ VNĐ).

Hiện tại vẫn chưa có mốc thời gian cụ thể khi nào sự cố phần mềm này mới được khắc phục triệt để, đồng nghĩa với việc chi phí thiệt hại của dự án sẽ còn tiếp tục tăng cao. Sự kiện này là một bài học đắt giá cảnh báo về mức độ rủi ro cực lớn khi thực hiện nâng cấp và thay thế các hệ thống phần mềm nghiệp vụ cốt lõi quy mô lớn.

3、[Sự cố đám đông tụ tập vì thông tin lễ hội ma Halloween giả tạo bằng AI](https://www.irishtimes.com/ireland/2024/11/01/we-are-highly-embarrassed-website-creator-behind-non-existent-dublin-halloween-parade-says-it-was-a-mistake/)

Cuối tháng trước nhân sự kiện lễ hội Halloween, hai bạn trẻ người Pakistan đã thiết lập một [trang web thông tin](https://myspirithalloween.com/) chuyên tổng hợp các hoạt động vui chơi giải trí trên toàn thế giới.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110507.webp)

Thế nhưng, họ đã giấu kín một sự thật là: Để tiết kiệm chi phí và thời gian thu thập dữ liệu thủ công, toàn bộ thông tin các sự kiện trên trang web đều được tạo tự động bằng AI và hoàn toàn không có thật trên thực tế.

Một cư dân mạng Ireland do không biết sự thật đã vô tình chia sẻ thông tin về một lễ hội hóa trang Halloween tại Dublin lên mạng xã hội. Thông tin sau đó nhanh chóng lan truyền chóng mặt trên các nền tảng TikTok và Instagram.

Kết quả là vào đúng đêm Halloween, hàng ngàn người dân đã đổ xô về một con phố lớn ở thủ đô Dublin, Ireland để xếp hàng chờ đợi tham gia lễ diễu hành hóa trang.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110508.webp)

Mọi người đứng chờ đợi mỏi mòn giữa phố suốt nhiều giờ đồng hồ và sau đó mới ngỡ ngàng nhận ra mình đã bị lừa khi không có bất kỳ lễ hội nào diễn ra. Để tránh tình trạng hỗn loạn và mất an ninh trật tự do đám đông tiếp tục đổ về, lực lượng cảnh sát Dublin đã phải khẩn cấp phát đi thông báo giải tán đám đông.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110509.webp)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110512.webp)

Sự việc hy hữu này ngay ngày hôm sau đã tràn ngập trên khắp các trang báo quốc tế, buộc hai bạn trẻ quản trị trang web phải lên tiếng xin lỗi công khai. Sự cố này là một minh chứng rõ nét cho thấy tính cấp thiết của việc phải gắn nhãn hiển thị rõ ràng đối với các nội dung được tạo tự động bằng AI (AI-generated content).

4、**Các tin tức khác**

(1) Trung Quốc đang chính thức phát động chiến dịch kêu gọi người dân [đặt tên cho xe tự hành Mặt Trăng](https://www.cmse.gov.cn/xwzx/202410/t20241028_55835.html) thế hệ mới của quốc gia, đồng thời công bố hai phương án thiết kế nguyên mẫu xe tự hành đầu tiên.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110701.webp)

(2) Công ty công nghệ Etched vừa chính thức giới thiệu [*Oasis*](https://www.etched.com/blog-posts/oasis) — tựa game AI hoạt động theo thời gian thực đầu tiên trên thế giới. Game được huấn luyện dựa trên mã nguồn và dữ liệu của trò chơi Minecraft, với toàn bộ đồ họa và khung hình hiển thị trong game đều do AI tự động tạo ra theo thời gian thực (tham khảo thêm [trang web giới thiệu chi tiết](https://oasisaiminecraft.com/) của một lập trình viên).

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110208.webp)

(3) Tập đoàn OpenAI vừa chính thức mua lại và kích hoạt tên miền [chat.com](https://chat.com/), tự động chuyển hướng người dùng trực tiếp về trang chủ chatgpt.com.

## 文章

1、[So sánh năng lực công cụ tìm kiếm ChatGPT Search và Google Search](https://www.tomsguide.com/ai/i-just-tested-google-vs-chatgpt-search-and-im-shocked-by-the-results) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110207.webp)

Tuần trước, OpenAI đã chính thức tích hợp tính năng tìm kiếm trực tiếp ChatGPT Search, đối đầu trực diện với gã khổng lồ Google. Bài viết đối chiếu kết quả tìm kiếm thực tế của hai bên và đưa ra nhận định ngắn gọn: Google thực sự đang đứng trước một thử thách lớn.

2、[Hướng dẫn thiết lập các phím tắt lệnh (alias) cho Git](https://tutorialedge.net/tips/aliasing-your-git-commands/) (tiếng Anh)

Tác giả giới thiệu cách cấu hình và thiết lập các phím tắt dòng lệnh tiện lợi cho Git, giúp rút ngắn thời gian gõ lệnh hằng ngày (ví dụ chuyển đổi lệnh `git add -A` thành phím tắt ngắn gọn `git a`).

3、[Hướng dẫn thiết kế trang web hồ sơ cá nhân (Resume Web)](https://michaelengen.com/posts/my-eleventy-resume/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110402.webp)

Tác giả chia sẻ cách ứng dụng trình tạo trang web tĩnh Eleventy (viết bằng JavaScript) để tự xây dựng một trang web hồ sơ cá nhân đẹp mắt (hình trên), hỗ trợ xuất bản và in ấn trực tiếp ra định dạng tệp tin PDF chuẩn xác.

4、[Câu chuyện đóng góp mã nguồn vá lỗi cho dự án VS Code của tôi](https://imbant.github.io/blog/2024/10/29/VS-Code-Thankyou/) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110504.webp)

Chia sẻ của tác giả về quá trình phát hiện, tìm nguyên nhân và gửi bản vá sửa một lỗi (bug) bảo mật liên quan đến trình quản lý ngôn ngữ TypeScript được tích hợp sẵn bên trong VS Code. (Đóng góp từ [@imbant](https://github.com/ruanyf/weekly/issues/5478))

5、[Cách ứng dụng công cụ Makefile cho các dự án Node.js](https://rosszurowski.com/log/2022/makefiles) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082401.webp)

Bài viết hướng dẫn chi tiết cách viết tệp Makefile để quản lý và tự động hóa các tác vụ chạy thử, đóng gói và kiểm thử trong các dự án JavaScript/Node.js.

6、[Hướng dẫn xây dựng Web Components bằng thư viện Lit](https://pwp.stevecassidy.net/javascript/lit/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024082505.webp)

Bài hướng dẫn cơ bản từng bước giúp lập trình viên nhanh chóng tiếp cận và ứng dụng thư viện Lit để thiết kế các thành phần Web Components tùy biến độc lập.

7、[Tìm hiểu cơ chế nạp mô-đun thư viện của ngôn ngữ Ruby](https://www.railsexplained.com/pages/hunting-for-gems/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024093005.webp)

Bài viết cơ bản dành cho lập trình viên mới bắt đầu tìm hiểu về lịch sử phát triển và các cơ chế gọi nạp thư viện (require/load gems) của ngôn ngữ Ruby.

## 工具

1、[flyscrape](https://flyscrape.com/)

Công cụ cào và trích xuất dữ liệu trang web đa nền tảng chạy trên dòng lệnh, được viết bằng Go nhưng hỗ trợ viết tập lệnh điều khiển bằng JavaScript giúp lập trình viên dễ dàng thao tác.

2、[uv](https://github.com/astral-sh/uv)

Công cụ quản lý và cài đặt thư viện Python cực nhanh được phát triển bằng ngôn ngữ Rust, hoạt động như một giải pháp thay thế hiệu năng cao cho công cụ `pip` truyền thống.

3、[ChatTCP](https://chattcp.com)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110212.webp)

Ứng dụng phân tích gói tin mạng TCP chuyên nghiệp dành cho hệ điều hành macOS, hỗ trợ đơn giản hóa quy trình giám sát mạng, cung cấp miễn phí các tính năng cốt lõi. (Đóng góp từ [@wujiuye](https://github.com/ruanyf/weekly/issues/5454))

4、[typing-practice](https://github.com/wincatcher/typing-practice.toolsnav.top)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110211.webp)

Ứng dụng web luyện gõ phím tiếng Anh mã nguồn mở trực quan. (Đóng góp từ [@wincatcher](https://github.com/ruanyf/weekly/issues/5451))

5、[Vân Đáp (云搭)](https://github.com/wangyuan389/yunda)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110502.webp)

Nền tảng xây dựng ứng dụng low-code mã nguồn mở, hỗ trợ tạo nhanh các ứng dụng mini-programs, trang H5, bảng khảo sát và bài viết đồ họa. Trải nghiệm thử bản [Demo](https://www.sunmao-design.top/sunmao/admin). (Đóng góp từ [@wangyuan389](https://github.com/ruanyf/weekly/issues/5473))

6、[NextTalk](https://github.com/Mebius1916/NextTalk_web)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110213.webp)

Hệ thống phòng chat trực tuyến thời gian thực được xây dựng trên nền tảng Next.js, tài liệu cấu hình chi tiết có thể tham khảo tại phiên bản [Desktop App](https://github.com/Mebius1916/NextTalk). (Đóng góp từ [@Mebius1916](https://github.com/ruanyf/weekly/issues/5457))

7、[dazhengTools](https://github.com/dazhengs/tools)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110306.webp)

Hộp công cụ mã hóa và giải mã dữ liệu trực tuyến hoạt động hoàn toàn ở phía client, hỗ trợ chạy offline bảo mật dữ liệu. (Đóng góp từ [@dazhengs](https://github.com/ruanyf/weekly/issues/5460))

8、[TempMail](https://tempmail100.com/)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110308.webp)

Dịch vụ hộp thư điện tử tạm thời (Temporary Email) hỗ trợ tốt cho cả trình duyệt web và ứng dụng di động iOS. (Đóng góp từ [@houzhongjian](https://github.com/ruanyf/weekly/issues/5455))

9、[Hệ thống tự động tuần tra giám sát website](https://github.com/TheCoolQATeam/online-inspection-tracker)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110702.webp)

Công cụ mã nguồn mở hỗ trợ cấu hình kiểm tra định kỳ trạng thái hoạt động của các liên kết web, giúp kịp thời phát hiện sự cố lỗi trang trắng (white screen) hoặc máy chủ không phản hồi, tự động gửi cảnh báo về DingTalk, Lark, WeChat. Trải nghiệm bản [Demo](https://check.itest.ren/). (Đóng góp từ [@zdx0122](https://github.com/ruanyf/weekly/issues/5486))

10、[Magika](https://google.github.io/magika/)

Công cụ dòng lệnh do Google phát triển ứng dụng mô hình AI Học sâu để tự động nhận dạng và phân tích định dạng tệp tin (ví dụ xác định chính xác tệp là ảnh hay text), có cung cấp phiên bản JavaScript chạy trên web.

## AI 相关

1、[AI Hear](https://hear.thucydides.net/zh-cn/)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110305.webp)

Phần mềm máy tính chạy offline hỗ trợ nhận diện và chuyển đổi giọng nói thành văn bản theo thời gian thực, hỗ trợ dịch thuật trực tiếp và xuất tệp phụ đề, tương thích với cả Windows và macOS. (Đóng góp từ [@phonechan](https://github.com/ruanyf/weekly/issues/5458))

2、[5ire](https://5ire.app/)

Trình quản lý và tương tác với các mô hình ngôn ngữ lớn LLM mã nguồn mở dành cho máy tính (Windows và macOS). (Đóng góp từ [@nanbingxyz](https://github.com/ruanyf/weekly/issues/5461))

3、[CR-Mentor](https://github.com/Gijela/CR-Mentor)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110503.webp)

Dự án mã nguồn mở hỗ trợ tự thiết lập dịch vụ AI kết nối với kho chứa GitHub để tự động thực hiện quy trình đánh giá chất lượng mã nguồn (Code Review) mỗi khi có Pull Request mới. (Đóng góp từ [@Gijela](https://github.com/ruanyf/weekly/issues/5476))

4、[APIPark](https://github.com/APIParkLab/APIPark)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110518.webp)

Nền tảng quản lý cổng kết nối AI (AI Gateway) mã nguồn mở, giúp doanh nghiệp dễ dàng thiết lập hệ thống quản lý tập trung việc gọi API và tích hợp đồng thời nhiều mô hình AI khác nhau. (Đóng góp từ [@Frey2024](https://github.com/ruanyf/weekly/issues/5481))

5、[Srcbook](https://github.com/srcbookdev/srcbook)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110514.webp)

Môi trường phát triển ứng dụng mã nguồn mở cho phép người dùng mô tả yêu cầu bằng văn bản để AI tự động thiết kế và tạo nhanh các ứng dụng full-stack hoàn chỉnh viết bằng JavaScript.

6、[Claude Artifacts giới thiệu](https://simonwillison.net/2024/Oct/21/claude-artifacts/)

Tính năng hiển thị kết quả trực tiếp Artifacts của mô hình Claude có tính năng hoạt động tương tự như công cụ trên, hỗ trợ dựng nhanh các ứng dụng web một trang (SPA) trực quan. Bài viết giới thiệu sâu về cơ chế hoạt động của tính năng này.

7、[Browser-Use](https://github.com/gregpr07/browser-use)

Thư viện Python mã nguồn mở hỗ trợ lập trình viên ứng dụng mô hình trí tuệ nhân tạo để thiết lập quy trình tự động hóa tương tác trình duyệt web (Web Automation).

## 资源

1、[Unfaked](https://www.gounfaked.com/)

Thư viện lưu trữ hình ảnh chất lượng cao miễn phí, chuyên thu thập và cung cấp các bức ảnh chân thực được tạo hoàn toàn bằng AI để phục vụ thiết kế.

2、[Bản dịch cuốn sách: Phỏng vấn thiết kế hệ thống](https://learning-guide.gitbook.io/system-design-interview)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110210.webp)

Bản dịch tiếng Trung đầy đủ của cuốn sách cẩm nang nổi tiếng *System Design Interview: An Insider's Guide*, cung cấp các kiến thức cốt lõi về cách thức thiết kế và xây dựng các hệ thống phần mềm quy mô lớn phục vụ các kỳ thi tuyển dụng. (Đóng góp từ [@Admol](https://github.com/ruanyf/weekly/issues/5448))

3、[Auth Wiki](https://auth.wiki/)

Trang bách khoa toàn thư trực tuyến chuyên tổng hợp và giải thích chi tiết các thuật ngữ, khái niệm liên quan đến lĩnh vực xác thực (Authentication), phân quyền (Authorization) và quản lý danh tính (Identity Management) trong công nghệ thông tin.

4、[Bản đồ theo dõi vệ tinh 3D thời gian thực](https://app.keeptrack.space/)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024100304.webp)

Ứng dụng web hiển thị mô phỏng 3D thời gian thực vị trí của toàn bộ các vệ tinh nhân tạo đang quay quanh Trái Đất. Người dùng có thể chọn một tọa độ bất kỳ để xem danh sách các vệ tinh đang bay qua bầu trời khu vực đó.

## 图片

1、[Xu hướng ứng dụng tấm pin năng lượng mặt trời](https://x.com/jessepeltan/status/1836523494840111613)

Giá thành sản xuất các tấm pin năng lượng mặt trời hiện nay đang giảm mạnh với tốc độ chóng mặt, tiệm cận hoặc thậm chí rẻ hơn giá của các vật liệu tấm ốp mặt dựng tòa nhà thông thường.

Trong tương lai không xa, chúng ta rất có thể sẽ chứng kiến phần lớn các tòa nhà cao tầng đều sử dụng pin mặt trời để làm vật liệu ốp bao phủ toàn bộ mặt ngoài ngoại thất.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110301.webp)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110302.webp)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110303.webp)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110304.webp)

## 文摘

1、[Tại sao các bệnh viện tại Mỹ vẫn tin dùng máy nhắn tin (pager)?](https://healthtechmagazine.net/article/2019/06/why-hospital-pager-withstood-test-time)

Máy nhắn tin (hay máy tìm tin) là thiết bị liên lạc vô cùng phổ biến của những năm 90 thế kỷ trước, nay đã bị khai tử hoàn toàn trong đời sống xã hội.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110713.webp)

Tuy nhiên, có một thực tế kinh ngạc là hiện nay có tới gần 80% số bệnh viện tại Mỹ vẫn duy trì sử dụng hệ thống máy nhắn tin trong hoạt động hằng ngày. Lý do đằng sau là gì?

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110714.webp)

Giải pháp này vẫn được ưu tiên lựa chọn nhờ một số ưu thế công nghệ vượt trội:

**(1) Chất lượng phủ sóng tín hiệu mạng cực tốt.**

Hệ thống máy nhắn tin hoạt động trên băng tần sóng vô tuyến tương tự như sóng phát thanh FM, hoàn toàn độc lập với mạng viễn thông di động 3G/4G/5G hay Wi-Fi. Băng tần sóng này có năng lực xuyên thấu vật cản bê tông cực mạnh và phạm vi phủ sóng rất rộng. Tại các khu vực phòng kín, tầng hầm hay góc khuất của bệnh viện nơi điện thoại hoàn toàn mất sóng di động, máy nhắn tin vẫn có thể nhận tín hiệu thông suốt.

Điều này giúp hệ thống liên lạc qua máy nhắn tin đạt độ tin cậy an toàn gần như tuyệt đối, đặc biệt là khi xảy ra các thảm họa thiên tai gây sập mạng viễn thông công cộng.

**(2) Thời lượng pin bền bỉ vượt trội.**

Thiết bị máy nhắn tin tiêu hao cực kỳ ít năng lượng. Chỉ với một viên pin nhỏ, thiết bị có thể duy trì hoạt động liên tục suốt 2 tuần liền mà không cần sạc, vượt trội hoàn toàn so với yêu cầu phải sạc pin hằng ngày của điện thoại thông minh.

**(3) Tính bảo mật và tối giản.**

Cơ chế vận hành của máy nhắn tin rất đơn giản, không chạy hệ điều hành phức tạp nên hầu như không thể bị tấn công mạng hay cài mã độc. Ngay cả khi thiết bị vô tình rơi vào tay người lạ, lượng thông tin y tế rò rỉ ra ngoài cũng là cực kỳ hạn chế và an toàn.

## 言论

1、

Một cuộc khảo sát thực tế tại Mỹ cho thấy có tới 81% số doanh nghiệp thừa nhận từng đăng tải các thông tin tuyển dụng giả tạo (ghost jobs). Mục tiêu của hành vi này bao gồm: (1) Duy trì sự hiện diện liên tục của thương hiệu trên các trang tuyển dụng, (2) Thu thập dữ liệu để xây dựng kho lưu trữ hồ sơ nhân tài dự phòng, và (3) Tạo áp lực tâm lý cho nhân viên hiện tại hiểu rằng họ hoàn toàn có thể bị thay thế bất kỳ lúc nào để họ không dám lơ là công việc.

-- [《Tác hại của các tin tuyển dụng ma đối với nhân sự ngành công nghệ》](https://www.sfgate.com/tech/article/ghost-jobs-california-tech-industry-19871249.php)

2、

Hiệu năng của phần cứng máy tính ngày nay đã đạt tốc độ nhanh đến kinh ngạc: Bộ vi xử lý Apple M1 Max chạy ở xung nhịp 3.2GHz, tương đương với 3,2 tỷ chu kỳ xử lý mỗi giây.

Thế nhưng, tôi vẫn mất tới 3 giây ròng rã chỉ để mở ứng dụng Microsoft Teams trên máy. Tôi hoàn toàn không tin nổi việc mở một phần mềm văn phòng lại tiêu tốn của hệ thống tới 9,6 tỷ chu kỳ xử lý. Tôi biết so sánh này có phần đơn giản hóa vấn đề, nhưng thực trạng rõ ràng là: Phần cứng ngày một nhanh hơn, nhưng các ứng dụng chúng ta dùng hằng ngày lại ngày một chậm đi. Rốt cuộc chuyện gì đang xảy ra vậy?

-- [preyneyv.dev](https://blog.preyneyv.dev/doing-less-with-more)

3、

Một nghiên cứu phân tích văn bản cho thấy tần suất xuất hiện của các từ ngữ thể hiện tính không chắc chắn như "might" (có thể) hay "probably" (nhiều khả năng) trong các bài báo cáo nghiên cứu khoa học đã sụt giảm nghiêm trọng tới 40% trong vòng 20 năm qua.

Điều này cảnh báo một thực trạng đáng lo ngại rằng các bài báo khoa học ngày nay đang có xu hướng phóng đại kết quả và đưa ra các khẳng định mang tính chủ quan thiếu độ tin cậy khoa học cao.

-- [Tạp chí Science](https://www.science.org/content/article/some-scientific-papers-words-expressing-uncertainty-have-decreased)

4、

Khái niệm "tầng lớp trung lưu" tại Mỹ đang có sự thay đổi căn bản về mặt bản chất. Trước đây, tầng lớp trung lưu dùng để chỉ những người có nguồn tài chính dư dả để đầu tư, sở hữu công việc ổn định, có nhà riêng, xe hơi, gia đình hạnh phúc và có quỹ lương hưu an nhàn.

Nhưng ngày nay, tầng lớp trung lưu lại đang dần biến thành "tầng lớp bấp bênh" (precariat). Bạn vẫn có một công việc để làm, nhưng có thể bị sa thải bất kỳ lúc nào. Bạn hoàn toàn không có khả năng mua nhà riêng, không thể tích lũy tài chính cho tương lai hưu trí và luôn chật vật xoay xở chi trả các hóa đơn sinh hoạt hằng tháng.

Đây là thực trạng bình thường mới tại nước Mỹ. Một người bạn làm việc trong ngành ngân hàng chia sẻ với tôi rằng phần lớn các tài khoản khách hàng của anh ấy sau khi trừ đi chi phí thanh toán tiền thuê nhà chỉ còn lại số dư vỏn vẹn vài trăm USD.

-- [Ý kiến độc giả trên diễn đàn Hacker News](https://news.ycombinator.com/item?id=42066439)

5、

Nghiên cứu của Hiệp hội Tâm lý học Hoa Kỳ chỉ ra rằng việc tập trung tư duy suy nghĩ quá sâu sẽ trực tiếp gây ra các cảm xúc bực bội, chán nản hoặc các trạng thái tâm lý tiêu cực khác. Vì vậy, nhận định vui rằng "suy nghĩ nhiều không tốt cho sức khỏe" xét ở góc độ khoa học là hoàn toàn có cơ sở.

-- [Hãng tin UPI](https://www.upi.com/Health_News/2024/08/05/netherlands-mental-exertion-thinking/2701722810331/)

## 往年回顾

[Đánh giá và lựa chọn màn hình phụ tối ưu cho góc làm việc](https://www.ruanyifeng.com/blog/2023/10/weekly-issue-277.html) (2023 #277)

[Tìm hiểu chương trình đào tạo hội nhập nhân sự mới của Meta (Facebook)](https://www.ruanyifeng.com/blog/2022/10/weekly-issue-227.html) (2022 #227)

[Bàn về công năng sử dụng thực tế và giá trị của chiếc iPad](https://www.ruanyifeng.com/blog/2021/09/weekly-issue-177.html) (2021 #177)

[Tương lai: Mọi người đều có thể làm phần mềm, rất ít người viết code](https://www.ruanyifeng.com/blog/2020/09/weekly-issue-127.html) (2020 #127)

(Hết)
