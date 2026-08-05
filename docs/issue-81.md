# 科技爱好者周刊：第 81 期 (Bản tin chia sẻ công nghệ số 81)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

Mục tuyển dụng [《Ai đang tuyển dụng?》](https://github.com/ruanyf/weekly/issues/798) cung cấp nhiều thông tin việc làm hữu ích, hoan nghênh ghé thăm hoặc đăng tải thông tin tuyển dụng/thực tập.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110707.jpg)

Ảnh bìa: Màn hình ghép LCD.

## 刊首语 (Lời tựa)

Gần đây, tôi có đọc được một dòng chia sẻ của một người dùng trên [Twitter](https://twitter.com/cwh_tw/status/1179743496594317313) thế này:

> Khi còn trẻ, tôi luôn nghĩ rằng thế hệ đi trước trong gia đình là những tấm gương phản chiếu để mình rút kinh nghiệm, để tránh đi vào vết xe đổ từ lối sống, tính cách, công việc cho đến cách đối nhân xử thế của họ.
> 
> Cho đến khi chạm đến độ tuổi này, tôi mới nhận ra mình ngày càng giống họ. Hóa ra, quỹ đạo cuộc đời phần lớn đã được định đoạt bởi bộ gen gia đình. Nếu không có những đột biến gen đặc biệt, cuộc đời của một người cơ bản chỉ là mức trung bình cộng từ bộ gen hai bên nội ngoại cộng trừ thêm khoảng 20% mà thôi. Ít nhất là tôi cảm thấy bản thân mình đúng là như vậy.

Ý của anh ấy là, **cho dù bạn có nỗ lực đến đâu đi chăng nữa, trong hầu hết các trường hợp, hoàn cảnh sống của bạn tối đa cũng chỉ tốt hơn thế hệ cha mẹ khoảng 20%.** Tôi cũng có cảm nhận tương tự: thế hệ con cái rất khó để tạo ra sự bứt phá vượt bậc so với thế hệ cha mẹ, đặc biệt là trong bối cảnh tốc độ tăng trưởng kinh tế chung đang có xu hướng chậm lại.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110704.jpg)

Đại văn hào Balzac từng nói một câu đại ý: "Để nuôi dưỡng một người thượng lưu ở Paris, cần có sự tích lũy nỗ lực của ba thế hệ". Trước đây tôi thấy câu nói này quá cường điệu, nhưng giờ đây tôi nhận ra đó chính là thực tế cuộc sống. Trong số những người tôi quen biết, số ví dụ về việc thế hệ con cái vượt trội hoàn toàn so với cha mẹ là không nhiều, **phần lớn mọi người vẫn duy trì cuộc sống, tầng lớp xã hội và vị thế kinh tế tương đồng với thế hệ đi trước.**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110705.jpg)

Làm một phép tính đơn giản: nếu mỗi thế hệ cải thiện cuộc sống được 20% so với thế hệ trước, thì đúng là phải mất ba thế hệ để vị thế kinh tế của gia đình tăng gấp đôi (1.2 lũy thừa 4 bằng 2.07), tức hoàn cảnh sống của bạn sẽ tốt hơn gấp đôi so với thời ông cố. Đây là kịch bản lý tưởng nhất với điều kiện mọi thế hệ đều làm việc chăm chỉ. Nếu trong chuỗi đó xuất hiện một người lười biếng, tốc độ cải thiện sẽ chậm lại rõ rệt; còn nếu xuất hiện một kẻ phá gia chi tử, gia cảnh sẽ lập tức thụt lùi.

Tóm lại, trong điều kiện thông thường, việc thay đổi hoàn cảnh sống của một dòng họ là một tiến trình chậm rãi, đòi hỏi sự tích lũy bền bỉ qua nhiều thế hệ. Chỉ khi có được sự may mắn đặc biệt, bạn mới có cơ hội tạo ra một cuộc đời bứt phá vượt bậc so với xuất phát điểm của cha mẹ. Nếu không gặp may, cuộc sống của bạn thậm chí có thể không bằng thế hệ đi trước.

## Chuỗi khóa học Zhizhaobiao trên Tencent Classroom

Như các bạn đã biết, [Tencent Classroom](https://ke.qq.com/?utm=ruanyifeng) - một trong những nền tảng giáo dục trực tuyến lớn nhất Trung Quốc - đang là đơn vị tài trợ đồng hành cùng trang blog cá nhân của tôi. Gần đây, họ khởi động chương trình **"Kế hoạch Tencent Classroom 101"** nhằm thúc đẩy các tài nguyên giáo dục công nghệ chất lượng cao. Hôm nay, tôi xin giới thiệu tới các bạn ba khóa học lập trình tiêu biểu của đối tác Zhizhaobiao:

Khóa học thứ nhất là **《Lập trình viên Frontend Full-stack: 165 ngày bứt phá thành kỹ sư Web Full-stack thực chiến》** giúp bạn làm chủ toàn diện các kiến thức, công cụ lập trình giao diện và hệ thống để nâng cao năng lực cạnh tranh khi tìm việc.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110307.jpg)

Hai khóa học tiếp theo tập trung chuyên sâu vào mảng ứng dụng nhỏ WeChat Mini Program, gồm **《Khóa học nhập môn Mini Program》** và **《Khóa học cú pháp mới Mini Program 2019》**, rất phù hợp cho các bạn đang muốn tiếp cận hệ sinh thái này.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110308.jpg)

Đơn vị xây dựng nội dung là học viện Zhizhaobiao - tổ chức đào tạo frontend uy tín nhận chứng chỉ kép (Khóa học tuyển chọn và Đối tác chính thức) trên Tencent Classroom với đội ngũ giảng viên CNTT giàu kinh nghiệm thực chiến.

Độc giả quan tâm có thể quét mã QR WeChat dưới đây để tham gia nhóm học tập của Zhizhaobiao để nhận **kho tài liệu miễn phí gồm 200 cuốn sách điện tử mảng lập trình Web Frontend**, đồng thời nhận ngay **mã ưu đãi giảm 50% cho khóa học "7 ngày nhập môn phát triển ứng dụng WeChat Mini Program"**.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110610.jpg)

Bên cạnh các khóa học chuyên sâu, họ cũng cung cấp nhiều video học thử miễn phí về CSS, HTML5 và Node.js rất đáng để tham khảo.

## 资讯 (Tin tức)

1. **Ứng dụng drone tích hợp camera nhiệt tìm kiếm thành công bé trai 6 tuổi đi lạc trong rừng sâu**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102505.jpg)

Một cậu bé 6 tuổi không may đi lạc vào khu rừng rậm tại bang Minnesota (Mỹ) lúc trời đã tối và nhiệt độ ngoài trời giảm xuống dưới 0 độ C. Lực lượng cảnh sát địa phương đã huy động hơn 600 người tìm kiếm suốt nhiều giờ nhưng không có kết quả.

Đến 8 giờ tối, một nhiếp ảnh gia tự do nghe tin đã lập tức mang thiết bị bay không người lái DJI M210RTK V2 chuyên dụng có tích hợp camera cảm biến nhiệt hồng ngoại đến hiện trường hỗ trợ. Ông mang theo khoảng 12 bộ pin dự phòng để duy trì drone bay quét tầm nhiệt liên tục trên mặt đất từ trên cao.

Sau khi lọc bỏ các tín hiệu nhiệt gây nhầm lẫn từ các loài động vật hoang dã như rái cá, hươu và gấu, đến 1 giờ 40 sáng, chiếc drone đã xác định chính xác vị trí phát nhiệt của cậu bé nằm giữa hai nhóm tìm kiếm mặt đất (ảnh trên). Đội cứu hộ lập tức tiếp cận tọa độ và đưa cậu bé ra ngoài an toàn. Ảnh dưới là hình ảnh tầm nhiệt của đội cứu hộ đang di chuyển tiếp cận vị trí cậu bé.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102506.jpg)

2. **Các nhà khoa học đau đầu vì hóa đơn cước SMS roaming tăng vọt của những chú đại bàng Nga**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102601.jpg)

Một nhóm nhà nghiên cứu Nga chuyên theo dõi quỹ đạo di cư của loài đại bàng thảo nguyên đang đối mặt nguy cơ tuyệt chủng đã gắn các thiết bị định vị GPS đặc biệt lên lưng chim. Thiết bị được gắn SIM di động để tự động gửi tin nhắn SMS báo tọa độ về máy chủ định kỳ.

Đầu tháng 10, hành trình di trú của đàn chim vượt ra ngoài vùng thảo nguyên Kazakhstan để tiến vào không phận Iran và Pakistan. Việc này khiến các nhà khoa học hốt hoảng do thiết bị tự động chuyển sang chế độ chuyển vùng quốc tế (roaming), đẩy cước phí gửi mỗi tin nhắn SMS từ mức 2-15 Rúp vọt lên tới 49 Rúp. Hóa đơn tiền điện thoại gửi về vượt quá toàn bộ ngân sách nghiên cứu của dự án.

Nhóm nghiên cứu buộc phải khởi xướng chiến dịch quyên góp trực tuyến mang tên "Nạp tiền điện thoại cho đại bàng" kêu gọi cộng đồng chung tay giúp đỡ. Chiến dịch nhận được sự ủng hộ nhiệt tình từ những người yêu động vật hoang dã, số tiền quyên góp hiện đã đủ để chi trả cước phí SMS roaming cho đàn chim trong suốt một năm tới. Dưới đây là sơ đồ hành trình di cư của 17 chú đại bàng:

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102602.jpg)

3. **WHO tuyên bố xóa sổ hoàn toàn chủng virus bại liệt hoang dã Tuýp 3 trên toàn cầu**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102603.jpg)

Nhân ngày Thế giới phòng chống bệnh bại liệt (24/10), [Tổ chức Y tế Thế giới (WHO)](https://www.who.int/news-room/feature-stories/detail/two-out-of-three-wild-poliovirus-strains-eradicated) đưa ra tuyên bố lịch sử về việc根 trừ hoàn toàn chủng virus bại liệt hoang dã tuýp 3 (WPV3) trên quy mô toàn cầu.

Virus bại liệt hoang dã gây bệnh bại liệt ở trẻ em gồm 3 tuýp sinh học khác nhau (Tuýp 1, 2 và 3). Trong đó tuýp 2 đã được công bố xóa sổ hoàn toàn vào năm 2015. Ca bệnh nhiễm virus bại liệt tuýp 3 cuối cùng được ghi nhận tại Nigeria vào năm 2012 và suốt nhiều năm qua không phát hiện thêm bất kỳ ca bệnh mới nào, đủ cơ sở khoa học để tuyên bố xóa sổ hoàn toàn chủng này.

Hiện nay, thế giới chỉ còn duy nhất chủng virus bại liệt tuýp 1 tồn tại dai dẳng tại hai quốc gia Afghanistan và Pakistan với 94 ca nhiễm được ghi nhận trong năm nay. Một khi dập tắt hoàn toàn dịch bệnh tại hai điểm nóng này, bại liệt sẽ trở thành căn bệnh truyền nhiễm thứ hai trong lịch sử y học loài người bị xóa sổ hoàn toàn sau bệnh đậu mùa.

4. **Google triển khai thuật toán tìm kiếm BERT chú trọng ngữ cảnh và trật tự từ**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102705.jpg)

Google chính thức áp dụng thuật toán tìm kiếm thế hệ mới mang tên BERT vào hệ thống tìm kiếm thực tế của hãng. Cải tiến lớn nhất của BERT là khả năng hiểu được ngữ nghĩa thông qua trật tự từ và các giới từ đi kèm trong câu lệnh tìm kiếm của người dùng. Các thuật toán cũ thường bỏ qua các từ nối hoặc giới từ đơn giản, dẫn đến việc tìm kiếm cụm từ `hello world` hay `world hello` cho ra kết quả tương tự nhau.

Tuy nhiên, giới từ và trật tự từ thường là chìa khóa quyết định ý đồ tìm kiếm của con người. Ví dụ trong ảnh trên, khi người dùng tìm kiếm cụm từ "visa du lịch từ Brazil đến Mỹ" (brazilian traveler to usa), giới từ `to` đóng vai trò định hướng cực kỳ quan trọng. Thuật toán tìm kiếm cũ không hiểu được giới từ này nên hiển thị kết quả đầu tiên là thông tin miễn thị thực cho công dân Mỹ đi du lịch Brazil, trong khi thuật toán BERT mới đã hiểu đúng ngữ cảnh và trả về trang xin visa của Đại sứ quán Mỹ.

Hiện tại thuật toán BERT mới được áp dụng cho các tìm kiếm bằng tiếng Anh và sẽ sớm được mở rộng ra các ngôn ngữ khác.

5. **Nghiên cứu phả hệ di truyền xác định博茨瓦纳 (Botswana) là cái nôi khởi nguồn của loài người hiện đại**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102904.jpg)

Hầu hết các nhà nhân chủng học đều đồng thuận với giả thuyết loài người hiện đại có nguồn gốc từ châu Phi. Mới đây, một nhóm nghiên cứu di truyền học công bố kết quả phân tích DNA xác định chính xác khu vực Botswana thuộc miền trung nam châu Phi chính là nơi tổ tiên loài người xuất hiện đầu tiên vào khoảng 200.000 năm trước.

Loài người đã sinh sống tại khu vực này khoảng 70.000 năm trước khi bắt đầu dịch chuyển di cư theo hướng đông bắc hướng về phía Ai Cập ngày nay vào khoảng 130.000 năm trước, và bắt đầu di cư tỏa ra khắp các châu lục trên thế giới vào khoảng 80.000 năm trước.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102905.jpg)

6. **Tàu vũ trụ quân sự không người lái X-37B của Mỹ lập kỷ lục hoạt động 780 ngày liên tục trên quỹ đạo**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102909.jpg)

Mẫu máy bay vũ trụ không người lái tuyệt mật X-37B của quân đội Mỹ đã hạ cánh an toàn xuống Trạm vũ trụ Kennedy vào ngày 27/10, kết thúc sứ mệnh bay liên tục kỷ lục kéo dài 780 ngày trong không gian. Thiết bị có kích thước tương đương một chiếc xe bus nhỏ, sở hữu nhiều đường nét kiến trúc của tàu con thoi truyền thống nhưng hoạt động hoàn toàn tự động không cần phi hành đoàn. Đây là sứ mệnh thử nghiệm quỹ đạo lần thứ 5 của dòng máy bay này kể từ khi được phóng lên vào năm 2017.

7. **Tin vắn**

- Báo cáo thống kê của một đơn vị nghiên cứu nhân sự công nghệ cho biết tổng số lượng kỹ sư phần mềm trên thế giới năm 2018 đạt khoảng 22.3 triệu người, trong đó Trung Quốc sở hữu khoảng 1.9 triệu kỹ sư.

- Tập đoàn Khoa học và Công nghệ Hàng không Vũ trụ Trung Quốc công bố tầm nhìn xây dựng "Khu kinh tế Địa - Nguyệt" (Earth-Moon Economic Zone) vào năm 2050 với dự báo quy mô giá trị sản lượng các ngành dịch vụ, khai khoáng liên quan đến mặt trăng đạt trên 10.000 tỷ USD.

- Tập đoàn dầu khí quốc gia Saudi Arabia Saudi Aramco - doanh nghiệp có lợi nhuận lớn nhất thế giới với sản lượng chiếm 10% toàn cầu - thông báo chính thức khởi động tiến trình phát hành cổ phiếu lần đầu ra công chúng (IPO) với định giá mục tiêu có thể lên tới 2.000 tỷ USD.

- Các nhà tâm lý học Mỹ thực hiện lại nghiên cứu về "Quy tắc 10.000 giờ" nổi tiếng và chỉ ra rằng việc kiên trì luyện tập 10.000 giờ giúp bạn cải thiện chuyên môn xuất sắc hơn chính mình trước đây, nhưng hoàn toàn không đảm bảo bạn chắc chắn sẽ vượt qua tài năng thiên bẩm của những người khác.

- Không quân Mỹ thử nghiệm mời 7 hacker chuyên nghiệp tìm cách tấn công vào hệ thống điện tử của máy bay chiến đấu F-16 và phát hiện ra nhiều lỗ hổng bảo mật nghiêm trọng. Sang năm, lực lượng này dự kiến sẽ tổ chức giải đấu tấn công thử nghiệm vào các vệ tinh quân sự đang hoạt động trên quỹ đạo.

- Trình duyệt Firefox công bố kế hoạch mặc định ẩn tất cả các hộp thoại yêu cầu hiển thị thông báo (Notification popups) kể từ năm sau, người dùng muốn nhận thông báo bắt buộc phải chủ động click vào biểu tượng chuông trên thanh địa chỉ. Hộp thoại thông báo phiền toái này cùng với các hộp thoại xác nhận Cookie từ lâu đã được coi là những yếu tố gây ức chế nhất khi duyệt web.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110301.jpg)

## 文章 (Bài viết)

1、[Bài viết] [Tại sao việc sử dụng phương thức JSON.stringify lại ảnh hưởng nghiêm trọng đến hiệu năng của máy chủ Node.js?](https://itnext.io/how-json-stringify-killed-my-express-server-d8d0565a1a61) (Tiếng Anh)

Phân tích chuyên sâu về cơ chế đồng bộ (synchronous/blocking) của phương thức `JSON.stringify()` trong JavaScript. Đối với các đối tượng JSON có dung lượng lớn, việc thực hiện tuần tự hóa (serialization) sẽ chiếm dụng tài nguyên CPU liên tục, làm nghẽn Event Loop của Node.js và làm giảm khả năng xử lý yêu cầu đồng thời của máy chủ Express.

2、[Bài viết] [Xu hướng thay đổi hình thức công bố của các bài báo cáo khoa học học thuật trong 200 năm qua](https://thegradient.pub/over-optimization-of-academic-publishing-metrics/) (Tiếng Anh)

Một nhóm nghiên cứu Israel thực hiện phân tích thống kê lịch sử từ hơn 528 triệu tài liệu tham khảo học thuật trong suốt 2 thế kỷ qua. Kết quả chỉ ra xu hướng: nội dung chính của các bài báo cáo khoa học ngày càng ngắn đi, trong khi độ dài của tiêu đề, phần tóm tắt (abstract), danh sách đồng tác giả và lượng tài liệu tham khảo tự trích dẫn ngày càng tăng vọt, phản ánh hệ quả của việc chạy theo các chỉ số KPI đánh giá số lượng bài viết của giới học thuật.

3、[Bài viết] [Hướng dẫn chuyển đổi các hàm Callback truyền thống sang định dạng Promise trong JavaScript](https://zellwk.com/blog/converting-callbacks-to-promises/) (Tiếng Anh)

Bài viết hướng dẫn chi tiết cách viết lại các hàm xử lý bất đồng bộ sử dụng Callback truyền thống sang cấu trúc Promise hiện đại để chuẩn bị cho việc áp dụng cú pháp `async/await` giúp mã nguồn gọn gàng, dễ đọc và dễ bảo trì hơn.

## 软件 (Phần mềm)

1、[crontab guru — Công cụ trực tuyến giúp trực quan hóa và kiểm tra cấu pháp cấu hình hẹn giờ crontab](https://crontab.guru/)

Giúp các quản trị viên hệ thống dễ dàng gõ các chuỗi ký tự hẹn giờ của tiện ích Cron trên Linux (ví dụ `*/5 * * * *`) để xem giải nghĩa thời gian chạy cụ thể bằng ngôn ngữ tự nhiên trực quan, tránh lỗi cấu hình sai giờ chạy của các tác vụ ngầm.

2、[streamlit — Thư viện Python hỗ trợ xây dựng nhanh giao diện ứng dụng cho các mô hình học máy](https://github.com/streamlit/streamlit)

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100603.jpg)

Cho phép các kỹ sư dữ liệu chỉ cần viết vài dòng mã Python đơn giản là có thể dựng ngay một trang web dashboard tương tác trực quan hiển thị kết quả mô hình dữ liệu, tích hợp các bộ kéo trượt (sliders) và biểu đồ cập nhật động mượt mà.

3、[Bitwarden — Phần mềm quản lý thông tin mật khẩu mã nguồn mở đa nền tảng miễn phí uy tín](https://bitwarden.com/)

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100701.jpg)

Giải pháp quản lý thông tin đăng nhập an toàn thay thế cho các phần mềm trả phí thương mại, hỗ trợ đồng bộ dữ liệu mã hóa đầu cuối (end-to-end encryption) trên mọi thiết bị di động, máy tính và trình duyệt web.

4、[imagededup — Thư viện Python hỗ trợ tìm kiếm và loại bỏ các hình ảnh trùng lặp](https://github.com/idealo/imagededup)

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100705.jpg)

Ứng dụng thuật toán so khớp mã băm hình ảnh (Perceptual Hashing) và các mạng nơ-ron tích chập (CNN) để tự động phát hiện các bức ảnh có nội dung tương đồng hoặc trùng lặp trong kho ảnh lớn để dọn dẹp bộ nhớ.

## 资源 (Tài nguyên)

1、[Tài liệu] [Tài liệu dịch thuật tài liệu kỹ thuật phát triển Backend Docs4dev](https://www.docs4dev.com/)

Trang web tổng hợp và dịch thuật tiếng Trung chất lượng cao (có kết hợp hiệu chỉnh máy dịch) cho tài liệu hướng dẫn chính thức của các thư viện và framework phát triển backend phổ biến như Spring Boot, Nginx, các hệ thống Big Data (Hive, HBase, Flume) và các hệ cơ sở dữ liệu thông dụng.

2、[Tài liệu] [Hướng dẫn phong cách lập trình ngôn ngữ Go của tập đoàn Uber (Uber Go Style Guide)](https://github.com/uber-go/guide/blob/master/style.md)

Tài liệu chuẩn hóa phong cách viết code ngôn ngữ Go do đội ngũ kỹ sư của Uber biên soạn và chia sẻ mã nguồn mở, cung cấp các quy chuẩn thiết kế hàm, xử lý lỗi và tối ưu hiệu năng chạy đồng thời (concurrency) thực tế của doanh nghiệp.

## 图片 (Hình ảnh)

1. **Sự khác biệt bản chất giữa: Dữ liệu, Thông tin, Tri thức, Sự thấu suốt và Trí tuệ**

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091004.jpg)

Sơ đồ trực quan nổi tiếng mô tả tiến trình xử lý thông tin của bộ não con người: đi từ các hạt điểm dữ liệu rời rạc (Data), kết nối thành thông tin có nghĩa (Information), xâu chuỗi thành hệ thống tri thức (Knowledge), phát hiện ra các quy luật bản chất (Insight) và sau cùng đạt tới tầm trí tuệ ứng dụng thực tiễn (Wisdom).

2. **Apple I và giải pháp lưu trữ dữ liệu bằng băng từ cassette Panasonic năm 1976**

Năm 1976, nguyên mẫu máy tính thương mại đầu tiên của Apple mang tên Apple I được phát hành.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019092701.jpg)

Thời kỳ đó do ổ đĩa mềm và ổ cứng chưa phổ biến với người dùng cá nhân, toàn bộ dữ liệu lập trình của máy tính Apple I được ghi và đọc trực tiếp thông qua một chiếc máy ghi âm băng cassette Panasonic RQ-2102 thông thường kết nối qua cổng âm thanh (audio interface).

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019092703.jpg)

## 文摘 (Văn trích)

1. **Kiến trúc phần mềm đang bị thần thánh hóa quá mức, trong khi thiết kế đơn giản lại bị xem nhẹ**

- Mục tiêu tối thượng khi thiết kế một hệ thống máy tính luôn phải là **sự đơn giản**. Hệ thống càng đơn giản bao nhiêu thì việc thấu hiểu cấu trúc, tìm kiếm sửa lỗi và lập trình triển khai thực tế sẽ càng dễ dàng bấy nhiêu. Ngôn ngữ mô tả cấu trúc càng tường minh thì thiết kế đó càng dễ đi vào thực tế. Thiết kế hệ thống sạch cũng tương tự như mã nguồn sạch: dễ đọc và dễ hiểu.

- Làm thế nào để viết ra mã nguồn sạch? Có rất nhiều nguyên lý kỹ thuật để hướng tới điều này, nhưng bạn sẽ rất hiếm khi nghe thấy các chuyên gia khuyên bạn phải áp dụng cứng nhắc toàn bộ các mẫu thiết kế (Design Patterns) kinh điển của nhóm "Gang of Four" (GoF) vào dự án của mình. Mã nguồn sạch thực chất chỉ cần tuân thủ tốt nguyên lý đơn nhiệm (Single Responsibility Principle), đặt tên biến/hàm tường minh và thống nhất các quy ước chung của đội ngũ. Những nguyên tắc cơ bản này hoàn toàn tương thích tốt cho việc xây dựng một kiến trúc hệ thống sạch.

- Vậy vai trò thực tế của các mẫu thiết kế (Design Patterns) là gì? Chúng cung cấp cho bạn những gợi ý giải pháp tham khảo để tối ưu hóa mã nguồn hoặc cấu trúc khi gặp bài toán tương tự. Việc thấu hiểu các design patterns thông dụng là điều rất tốt, giúp rút ngắn thời gian thảo luận chuyên môn giữa các kỹ sư thông qua việc sử dụng chung các thuật ngữ kỹ thuật thống nhất. Tuy nhiên, design patterns không phải là cái đích hướng tới và không bao giờ có thể thay thế được sự đơn giản của hệ thống. 

Trong quá trình lập trình, nếu bạn vô tình viết ra một đoạn code tương đồng với một design pattern quen thuộc thì đó là điều rất tốt. Nhưng bạn không nên coi design patterns như những chiếc búa và nhìn đâu cũng thấy hệ thống của mình như những chiếc đinh cần phải đóng búa vào bằng mọi giá. Mục tiêu tối thượng của một kỹ sư là giải quyết bài toán thực tế của hệ thống một cách hiệu quả và học hỏi từ đó, thay vì cố gắng tô vẽ các kiến trúc phức tạp để trông có vẻ chuyên nghiệp.

## 言论 (Danh ngôn)

1、

> "Thực trạng cước phí lãi suất âm đang đặt ra một bài toán hóc búa cho ngành tài chính toàn cầu: hầu hết các mô hình toán học lượng hóa tài chính trị giá hàng nghìn tỷ USD được thiết kế từ trước tới nay đều không hỗ trợ việc tính toán với các tham số là số âm."
> 
> -- Trích bài viết *Lãi suất âm đang phá vỡ các quy tắc tài chính hiện đại*

(Hết)
