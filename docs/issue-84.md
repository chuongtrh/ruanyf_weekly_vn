# 科技爱好者周刊：第 84 期 (Bản tin chia sẻ công nghệ số 84)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

Mục tuyển dụng [《Ai đang tuyển dụng?》](https://github.com/ruanyf/weekly/issues/983) cung cấp nhiều thông tin việc làm hữu ích, hoan nghênh ghé thăm hoặc đăng tải thông tin tuyển dụng/thực tập.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111702.jpg)

Ảnh bìa: Tổ hợp căn hộ làm từ container, Johannesburg, Nam Phi. Ảnh từ [Reddit](https://www.reddit.com/r/UrbanHell/comments/dsbd0l/container_flats_joburg/).

## 刊首语 (Lời tựa)

Mỗi khi quan sát các tin tuyển dụng của các công ty công nghệ IT, tôi thường có cảm giác rằng rất nhiều vị trí công việc thực chất chỉ mang tính chất ngắn hạn dùng một lần. Nghĩa là doanh nghiệp tuyển dụng bạn về để giải quyết một bài toán cụ thể và khi dự án hoàn thành hoặc thất bại, họ sẽ sẵn sàng thực hiện các đợt cắt giảm nhân sự tương tự như việc thải bỏ một đôi đũa dùng một lần.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112714.jpg)

Thị trường công nghệ IT cạnh tranh cực kỳ khốc liệt, thị hiếu và công nghệ thay đổi chóng mặt hàng ngày. Các doanh nghiệp buộc phải áp dụng quy trình phát triển tinh gọn (Agile), yêu cầu dự án phải nhanh chóng chứng minh hiệu quả thực tế và hoạt động tuyển dụng luôn phục vụ trực tiếp cho tiến độ dự án. Nếu như các đợt tuyển dụng sinh viên mới tốt nghiệp (Campus Recruitment) còn có mục tiêu tích lũy nhân sự dự phòng cho tương lai, thì tuyển dụng nhân sự có kinh nghiệm (Social Recruitment) hoàn toàn mang tính định hướng dự án thực tế: hoặc là để bổ sung nhân lực cho dự án hiện có, hoặc là để xây dựng đội ngũ mới cho một sản phẩm mới.

Vì phần lớn các dự án khởi nghiệp công nghệ cuối cùng đều đi đến thất bại, nên trường hợp dự án tăng trưởng và liên tục bổ sung nhân sự là rất hiếm. Phần lớn các đợt tuyển dụng quy mô lớn thực chất là để chuẩn bị cho một sản phẩm mới hoặc một định hướng kinh doanh chưa rõ kết quả. Tại thời điểm đó, chính ban lãnh đạo doanh nghiệp cũng không chắc chắn liệu sản phẩm mới này có thể sống sót trên thị trường hay không và sẽ tồn tại được bao lâu. Mục tiêu hàng đầu của việc tuyển dụng là nhanh chóng xây dựng sản phẩm thô để đưa ra thị trường kiểm chứng. Nếu dự án may mắn sống sót, vị trí công việc của bạn sẽ trở thành dài hạn; còn nếu dự án thất bại, đó sẽ là một công việc ngắn hạn.

Khi dự án bị hủy bỏ, đội ngũ nhân sự được tuyển về cho dự án đó tự nhiên sẽ trở nên dư thừa. Doanh nghiệp sẽ tiến hành luân chuyển nội bộ hoặc trực tiếp sa thải. Lập trình viên cần có nhận thức thực tế rằng: các doanh nghiệp hiện nay khi tuyển dụng hầu như sẽ không xây dựng cho bạn một lộ trình đào tạo phát triển dài hạn từ 3 đến 5 năm. Việc bạn có thể tiếp tục đồng hành cùng doanh nghiệp hay không phụ thuộc lớn vào hai yếu tố: một là bạn có chứng minh được năng lực thực chiến ngay lập tức hay không, và hai là thị trường có đón nhận dự án mà bạn đang tham gia hay không. Chỉ cần một trong hai điều kiện này không được đáp ứng, vị trí công việc của bạn sẽ lập tức lung lay.

Theo quan sát của tôi, chiến lược tuyển dụng của nhiều doanh nghiệp hiện nay hoàn toàn mang tính chất dùng một lần. Khi dự án cần người, tôi sẽ đẩy mạnh tuyển dụng ồ ạt để hoàn thiện sản phẩm trong thời gian ngắn nhất. Sau đó, nếu phản hồi từ thị trường không tốt và dự án không thể duy trì, chúng tôi sẽ nhanh chóng chuyển sang dự án tiếp theo. Những nhân sự không phù hợp để luân chuyển sẽ phải rời đi để nhường chỗ cho các đợt tuyển dụng mới.

Về điểm này, các tập đoàn công nghệ lớn (như BAT) cũng không hề tốt hơn các startup nhỏ là bao. Bạn nên hiểu rằng tại các tập đoàn lớn, mọi vị trí công việc ổn định đều đã có người đảm nhiệm. Khi họ đăng tin tuyển dụng mới, mục tiêu chắc chắn là tìm người để giải quyết những công việc khó khăn, vất vả hoặc quá tải mà nhân sự nội bộ hiện tại không muốn nhận. Đi cùng với hệ thống đánh giá hiệu suất (KPI) cực kỳ khắt khe, khả năng bạn gặp phải một vị trí công việc mang tính chất ngắn hạn tại các tập đoàn lớn thậm chí còn cao hơn so với các công ty quy mô nhỏ.

## Tài liệu học tập Frontend miễn phí

Năm cũ sắp sửa khép lại và làn sóng nhảy việc sau Tết Nguyên Đán đang cận kề. Các bạn có kế hoạch tìm kiếm cơ hội công việc mới có thể bắt đầu chủ động ôn tập các kiến thức kỹ thuật trọng tâm thường xuất hiện trong các vòng phỏng vấn ngay từ bây giờ.

Lập trình giao diện Frontend vẫn là mảng tuyển dụng chiếm tỷ trọng lớn của ngành IT. Dưới đây là hai bộ tài liệu học tập frontend thực chiến hoàn toàn miễn phí được đối tác đào tạo Kaikeba gửi tặng độc giả của bản tin:

Bộ tài liệu thứ nhất là **《Bộ câu hỏi phỏng vấn Web 2019: Chuyên đề ES6》**. Đây là chuỗi video bài giảng phân tích chuyên sâu về lập trình hướng đối tượng trong ES6, cơ chế kế thừa Class và các phương thức ứng dụng nâng cao thường gặp trong các vòng phỏng vấn kỹ thuật.

Bộ tài liệu thứ hai là **《Lập trình thực chiến ngôn ngữ TypeScript》**. Hiện nay, hầu hết các dự án quy mô lớn đều ưu tiên lựa chọn TS để đảm bảo chất lượng mã nguồn thông qua cơ chế kiểm tra kiểu tĩnh (Static Typing). Tài liệu sẽ hướng dẫn chi tiết từng bước xây dựng một dự án từ đầu: cài đặt cấu hình TS, các kiểu dữ liệu, Interface, Generic và kết thúc bằng việc ứng dụng TS để xây dựng một dự án Vue.js hoàn chỉnh.

Chương trình quà tặng giới hạn **499 suất đăng ký miễn phí**, độc giả quan tâm có thể quét mã QR dưới đây để nhận tài liệu học tập:

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112809.jpg)

## 资讯 (Tin tức)

1. **Tổ chức quản lý RIPE thông báo chính thức phân bổ hết toàn bộ địa chỉ IPv4 tại khu vực Châu Âu**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112602.jpg)

Ngày 25/11, Tổ chức đăng ký địa chỉ IP khu vực Châu Âu (RIPE NCC) chính thức công bố kho địa chỉ IPv4 dự phòng của họ đã hoàn toàn cạn kiệt, không còn bất kỳ địa chỉ IPv4 mới nào để phân bổ cho các nhà mạng di động hay doanh nghiệp tại khu vực. Để ghi dấu sự kiện lịch sử này, toàn thể đội ngũ kỹ sư của tổ chức đã cùng chụp ảnh lưu niệm (ảnh trên).

Kể từ thời điểm này, RIPE NCC chỉ có thể cấp phát địa chỉ IPv4 mới bằng cách thu hồi lại các dải IP từ các tổ chức giải thể hoặc tuyên bố phá sản để tái phân bổ. Giải pháp căn cơ duy nhất cho vấn đề cạn kiệt IP toàn cầu là đẩy nhanh tiến trình chuyển dịch hạ tầng mạng sang giao thức IPv6 thế hệ mới. RIPE chịu trách nhiệm quản lý phân bổ IP cho khu vực màu vàng trên bản đồ dưới đây:

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112603.jpg)

2. **Disney+ nhận phản hồi trái chiều khi tự động cắt xén định dạng phim hoạt hình The Simpsons sang tỷ lệ 16:9**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111603.jpg)

Sau khi dịch vụ xem phim trực tuyến Disney+ ra mắt, nhiều khán giả phát hiện bộ phim hoạt hình kinh điển *The Simpsons* đã bị tự động co giãn hiển thị sang định dạng màn hình rộng 16:9. Thực tế trước mùa 20, bộ phim được sản xuất trên tỷ lệ khung hình gốc là 4:3 (hình trên).

Đội ngũ kỹ thuật của Disney bên cạnh việc nâng cao độ phân giải hình ảnh đã thực hiện cắt xén (crop) bớt phần nội dung hiển thị ở cạnh trên và cạnh dưới của khung hình gốc để ép phim về chuẩn tỷ lệ 16:9 hiện đại (hình dưới). Việc cắt xén này vô tình làm biến mất nhiều chi tiết và trò đùa hình ảnh ẩn giấu trong khung hình gốc. Trước phản ứng của người xem, Disney thông báo sẽ cập nhật thêm tùy chọn cho phép người dùng lựa chọn thưởng thức phim ở đúng tỷ lệ khung hình 4:3 gốc vào năm sau.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111602.jpg)

3. **Xu hướng sở hữu các thiết bị thời trang số (Digital Fashion) độc bản trên mạng xã hội**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111716.jpg)

Bản tin BBC đưa tin về việc Richard Ma, CEO của một doanh nghiệp bảo mật blockchain tại San Francisco, đã chi tới 9.500 USD để mua một bộ váy thiết kế đặc biệt dành tặng vợ. Điểm độc đáo là bộ váy này hoàn toàn không tồn tại ngoài đời thực dưới dạng vải vóc vật lý, mà là một tệp tin đồ họa số 3D được các nhà thiết kế "mặc" ghép nối vào hình ảnh cá nhân của vợ anh để chia sẻ lên các trang mạng xã hội (ảnh trên).

Vị CEO nhận định: "Mặc dù chi phí rất đắt đỏ nhưng đây là một khoản đầu tư giá trị. Trong thập kỷ tới, xu hướng khoác lên mình các trang phục thời trang số độc bản sẽ trở nên phổ biến, là biểu tượng văn hóa đặc trưng của kỷ nguyên số". Các bộ trang phục số cho phép các nhà thiết kế thỏa sức sáng tạo các cấu trúc siêu thực, sử dụng các vật liệu ánh sáng, hiệu ứng động mà công nghệ dệt may truyền thống không thể thực hiện được.

Nhiều hãng thời trang tại Thụy Điển đã bắt đầu ra mắt các dòng sưu tập thời trang số thương mại với mức giá khởi điểm khá tiếp cận chỉ từ 11 USD mỗi bộ trang phục (ảnh dưới):

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111717.jpg)

4. **Hãng hàng không Qantas thử nghiệm chuyến bay thẳng dài nhất thế giới từ London đến Sydney**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111809.jpg)

Do vị trí địa lý nằm ở Nam Bán Cầu, mọi chuyến bay từ Úc đến các trung tâm kinh tế lớn ở Bắc Bán Cầu đều có cự ly cực kỳ dài. Hãng hàng không quốc gia Úc Qantas đang tiến hành chuỗi thử nghiệm bay thẳng phi thương mại để đánh giá sức chịu đựng của phi hành đoàn và hành khách. Ngày 18/10, hãng thực hiện thành công chuyến bay thử nghiệm từ London đến Sydney với thời gian bay liên tục trên không đạt 19 giờ 19 phút.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111808.jpg)

Việc ngồi im liên tục suốt gần 20 giờ bay tiềm ẩn nhiều rủi ro sức khỏe cho hành khách (như hội chứng huyết khối tĩnh mạch sâu). Qantas đã áp dụng nhiều giải pháp khoa học: phục vụ bữa tối giàu carbohydrate ngay sau khi cất cánh và tắt đèn sớm để điều chỉnh nhịp sinh học giúp khách dễ ngủ. Sau khi tỉnh giấc, hành khách được hướng dẫn các bài tập kéo giãn cơ và đi bộ dọc khoang cabin rộng rãi của chiếc Boeing 787 Dreamliner (chuyến bay thử nghiệm chỉ chở 50 người để giảm tải trọng). Khi mặt trời mọc, hành khách được mời di chuyển đến cửa sổ để ngắm bình minh nhằm kích thích thị giác. Qantas sẽ đưa ra quyết định thương mại hóa đường bay thẳng này vào cuối năm nay.

5. **Nhà máy xử lý rác thải phát điện kết hợp khu vui chơi trượt tuyết độc đáo tại Copenhagen**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112111.jpg)

Thành phố Copenhagen (Đan Mạch) đưa vào vận hành nhà máy phát điện đốt rác công nghệ sạch thế hệ mới Amager Bakke. Mặt ngoài công trình được thiết kế ốp các module kính kim loại tạo hiệu ứng như một sườn núi xanh mát. Điểm độc đáo nằm ở phần mái dốc của tòa nhà được cải tạo thành một đường trượt tuyết nhân tạo khổng lồ phục vụ người dân thành phố.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112112.jpg)

Địa hình Đan Mạch chủ yếu là đồng bằng phẳng, người dân muốn chơi trượt tuyết thường phải di chuyển rất xa sang các nước láng giềng. Công trình mới giúp người dân có thể thỏa sức trượt tuyết ngay trong lòng thủ đô với mức phí khoảng 22 USD/giờ. Tòa nhà còn tích hợp các đường đi bộ leo núi nhân tạo trên mái, nhà hàng, quán bar ngắm cảnh và một bức tường leo núi nhân tạo cao nhất thế giới (85 mét) ở mặt bên tòa nhà. Toàn bộ quy trình vận hành nhà máy đốt rác phát điện cho 220.000 hộ gia đình bên trong chỉ cần đúng 2 kỹ sư điều khiển giám sát.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112113.jpg)

6. **Dự án ứng dụng gương hội tụ ánh sáng mặt trời tạo nguồn nhiệt lượng siêu cao của Heliogen**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112114.jpg)

Bên cạnh việc dùng pin mặt trời để phát điện, startup công nghệ Heliogen do tỷ phú Bill Gates tài trợ đã thử nghiệm thành công giải pháp sử dụng phần mềm điều khiển hàng nghìn tấm gương hội tụ ánh sáng mặt trời vào một điểm duy nhất để tạo ra nguồn nhiệt lượng tập trung đạt mức kỷ lục trên 1.000 độ C (nhiệt độ tối đa chạm mốc 1.500 độ C).

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112115.jpg)

Nguồn nhiệt lượng khổng lồ này được định hướng ứng dụng trực tiếp vào các ngành công nghiệp nặng (như sản xuất xi măng, luyện kim) để thay thế hoàn toàn việc đốt than đá và dầu mỏ truyền thống, giúp cắt giảm lượng khí thải nhà kính khổng lồ của ngành sản xuất vật liệu xây dựng toàn cầu.

7. **Tin vắn**

- Nghiên cứu y học công bố trên tạp chí *Nature* chỉ ra việc tiếp xúc kéo dài với các dải ánh sáng xanh phát ra từ hệ thống đèn LED chiếu sáng có thể gây ảnh hưởng xấu làm gia tăng tốc độ lão hóa tế bào và tổn thương hệ thần kinh của các sinh vật thử nghiệm.

- Bang New South Wales (Úc) triển khai hệ thống camera giám sát thông minh tích hợp AI trên các tuyến cao tốc để tự động phát hiện và xử phạt các tài xế có hành vi vừa lái xe vừa sử dụng điện thoại di động.

- Tesla chính thức ra mắt dòng xe bán tải chạy điện đặc sắc mang tên Cybertruck với ngôn ngữ thiết kế góc cạnh, vuông vức sử dụng vỏ thép không gỉ siêu cứng chịu lực, mức giá khởi điểm thương mại từ 40.000 USD.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112204.jpg)

- Tập đoàn General Electric bắt đầu lắp đặt tuabin gió ngoài khơi lớn nhất thế giới Haliade-X tại Hà Lan với chiều dài mỗi cánh quạt đạt kỷ lục 107 mét.

- Đội ngũ kỹ sư ảnh chụp của Google công bố các bức ảnh chụp dải Ngân Hà sắc nét được chụp trực tiếp từ chế độ chụp đêm (Night Sight) của dòng máy Pixel 4 XL mà hoàn toàn không qua chỉnh sửa hậu kỳ (ảnh dưới).

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112712.jpg)

## 文章 (Bài viết)

1、[Bài viết] [Phỏng vấn chuyên sâu cùng cha đẻ ngôn ngữ C++ Bjarne Stroustrup](https://news.codecademy.com/bjarne-stroustrup-interview/) (Tiếng Anh)

Nhà khoa học máy tính Bjarne Stroustrup chia sẻ về bối cảnh ra đời của ngôn ngữ C++ tại Bell Labs, triết lý thiết kế ngôn ngữ và trực tiếp đưa ra lời giải đáp chuyên môn cho 5 câu hỏi lập trình C++ nhận được lượt bình chọn cao nhất trên hệ thống Stack Overflow.

2、[Bài viết] [Thống kê phân tích các hành vi dò quét cổng SSH trái phép trên môi trường internet](https://bastian.rieck.me/blog/posts/2019/ssh_incidents/) (Tiếng Anh)

Tác giả thực hiện thu thập và phân tích dữ liệu từ hơn 980.000 lượt yêu cầu đăng nhập SSH trái phép (brute-force) vào hệ thống máy chủ cá nhân của mình trong vòng một năm, phác họa chân dung các botnet quét IP, các tài khoản (username) thường bị dò quét nhiều nhất và nguồn gốc địa lý của cuộc tấn công.

3、[Bài viết] [Làm thế nào để xuất địa chỉ IP của người dùng trực tiếp bằng cấu hình Nginx?](https://www.ecalamia.com/blog/show-ip-api-nginx/) (Tiếng Anh)

Chia sẻ mẹo cấu hình Nginx tối giản chỉ với hai dòng lệnh để tự động trả về địa chỉ IP công cộng của client dưới dạng một chuỗi JSON sạch sẽ mà không cần viết thêm mã nguồn PHP hay Node.js ở backend.

## 软件 (Phần mềm)

1、[onefetch — Tiện ích dòng lệnh hiển thị thông tin tổng quan của dự án Git trực quan](https://github.com/o2sh/onefetch)

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102912.jpg)

Công cụ viết bằng Rust giúp quét nhanh thư mục Git để in ra màn hình terminal biểu tượng logo của ngôn ngữ lập trình chủ đạo của dự án kèm theo các thông số: số lượng commit, số tác giả, số dòng code và giấy phép bản quyền của dự án.

2、[leonsans — Thư viện JavaScript hỗ trợ vẽ nét chữ nghệ thuật bằng Canvas và WebGL](https://github.com/cmiscm/leonsans)

Cung cấp công cụ vẽ các nét chữ Latinh dưới dạng các đường vector toán học, giúp các nhà phát triển frontend dễ dàng tạo ra các hiệu ứng hoạt họa chữ chạy, chữ vẽ nét chuyển động mượt mà trên giao diện web.

3、[SearX — Công cụ tìm kiếm siêu dữ liệu (Metasearch Engine) nguồn mở bảo vệ quyền riêng tư](https://github.com/asciimoo/searx)

Cho phép người dùng tự dựng một máy chủ tìm kiếm riêng tư của mình để tự động gom và lọc kết quả tìm kiếm từ hơn 70 dịch vụ lớn (như Google, Bing, Yahoo) mà hoàn toàn không lưu trữ cookie hay theo dõi hành vi lướt web của người dùng.

## 资源 (Tài nguyên)

1、[Tài liệu] [Danh sách các blog cá nhân tiếng Trung chất lượng cao xếp hạng theo lượng người đăng ký RSS](https://github.com/timqian/chinese-independent-blogs)

Kho dữ liệu GitHub tổng hợp thông tin đường dẫn RSS feed của hàng trăm blog cá nhân mảng công nghệ và đời sống chất lượng cao bằng tiếng Trung, được sắp xếp thứ tự theo số lượng độc giả theo dõi thực tế trên hệ thống Feedly.

2、[Tài liệu] [Lịch sử thiết kế và tiến hóa của các thanh cuộn (Scrollbar) trên các hệ điều hành](https://scrollbars.matoseb.com/)

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110302.jpg)

Trang web tổng hợp hình ảnh giao diện thiết kế của thanh cuộn màn hình qua các thế hệ hệ điều hành: từ phiên bản thô sơ của Macintosh System 1 (1984), Windows 95 cho tới giao diện phẳng tối giản của macOS và Windows 10 ngày nay.

## 图片 (Hình ảnh)

1. **Bản đồ phác thảo ý tưởng đào kênh đào Panama của các kỹ sư Pháp năm 1881**

Bức ảnh bản đồ cổ vẽ năm 1881 mô tả phương án đào kênh dẫn nước thẳng nối liền hai đại dương của các kỹ sư người Pháp. Do không lường trước được chênh lệch mực nước và dịch bệnh sốt rét hoành hành làm hàng vạn công nhân tử vong, dự án của Pháp đã thất bại hoàn toàn.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100601.jpg)

Phương án thực tế sau đó được người Mỹ tiếp quản hoàn thiện bằng cách xây dựng hệ thống âu tàu (locks) nâng hạ mực nước nhân tạo qua hồ Gatun như hiện nay.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100602.jpg)

## 文摘 (Văn trích)

1. **Vấn nạn ô nhiễm môi trường và sự trỗi dậy của khái niệm "Thời trang chậm" (Slow Fashion)**

Hoạt động sản xuất và tiêu dùng quần áo thời trang giá rẻ thay đổi mẫu mã liên tục hàng tháng (còn gọi là "Thời trang nhanh" - Fast Fashion) đang tạo ra lượng rác thải dệt may khổng lồ tàn phá môi trường trái đất:

Thống kê cho thấy chỉ riêng tại Mỹ đã phát thải tới 11.9 triệu tấn rác thải dệt may vào năm 2015 - trung bình mỗi người dân thải bỏ khoảng 34 kg quần áo mỗi năm, phần lớn trong số đó kết thúc ở các bãi chôn lấp rác thải. So với năm 1960, lượng rác thải dệt may đã tăng trưởng hơn 750% - tốc độ tăng nhanh gấp 10 lần so với tốc độ gia tăng dân số.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112814.jpg)

Sự bùng nổ của các thương hiệu thời trang nhanh như H&M hay Zara là nguyên nhân chính thúc đẩy xu hướng này. Mô hình kinh doanh của họ dựa trên việc tung ra hàng vạn mẫu thiết kế giá rẻ mới hàng năm để kích thích người tiêu dùng mua sắm liên tục và sẵn sàng vứt bỏ các trang phục cũ sau vài lần mặc để đón đầu các xu hướng mới.

Nhằm cân bằng lại thực trạng này, khái niệm "Thời trang chậm" (Slow Fashion) đang được các nhà hoạt động môi trường tích cực truyền bá trong thập kỷ qua: khuyến khích người tiêu dùng nâng cao nhận thức, mua sắm ít đi, chọn lọc các trang phục bền đẹp có thời gian sử dụng lâu dài để giảm thiểu lượng hóa chất độc hại và khí thải nhà kính sinh ra từ ngành công nghiệp dệt may (vốn chiếm tới 8% tổng lượng phát thải khí nhà kính toàn cầu).

## 言论 (Danh ngôn)

1、

> "Các hệ thống tự lái của xe điện Tesla hoàn toàn có thể giúp bảo vệ tính mạng của hàng triệu người dùng trong tương lai, nhưng để đạt được độ tin cậy tuyệt đối cho mục tiêu đó, hệ thống có thể sẽ phải trải qua những sự cố tai nạn gây tử vong ở giai đoạn thử nghiệm thực tế ban đầu."
> 
> -- Trích bài viết trên hãng tin Bloomberg

(Hết)
