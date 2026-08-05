# 科技爱好者周刊：第 73 期 (Bản tin chia sẻ công nghệ số 73)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091206.jpg)

Ảnh bìa: Thượng Hải, 2019.

## 刊首语 (Lời tựa)

Nhiều người mua máy chạy bộ về nhà, tập luyện hào hứng được một thời gian rồi dần dần bỏ xó, để máy bám đầy bụi bẩn trong góc nhà. Nhà tôi cũng rơi vào hoàn cảnh y hệt như vậy.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091205.jpg)

Khi các ứng dụng chạy bộ trên điện thoại ra đời, họ cũng phải đối mặt với bài toán hóc búa này: Làm sao để giúp những người dùng chỉ có "nhiệt huyết ba phút" kiên trì tập luyện mà không bỏ cuộc giữa chừng?

Họ đã áp dụng rất nhiều giải pháp, nhưng **tôi cho rằng chiêu thức hiệu quả nhất chính là ghi chép dữ liệu (Data Logging).** Hôm qua chạy được mấy km, hôm nay chạy được mấy km, mỗi ngày đều được hệ thống ghi lại chi tiết. Bạn có thể nhìn thấy sự tiến bộ trực quan của bản thân qua từng con số, từ đó nảy sinh động lực tự nhiên muốn liên tục thử thách và vượt qua giới hạn của chính mình.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091204.jpg)

Để củng cố thêm động lực này, các ứng dụng còn tung ra các chương trình điểm danh chạy bộ liên tục để nhận huy chương ảo, đồng thời xây dựng các cộng đồng chạy bộ nhóm để người dùng theo dõi xem trong số bạn bè của mình ai đang dẫn đầu, ai đang tụt lại phía sau. Nhờ những cơ chế này, rất nhiều người đã thực sự kiên trì luyện tập thành công. Việc chạy bộ từ một hoạt động thể chất đơn thuần đã chuyển hóa thành một dạng rèn luyện ý chí và tương tác xã hội thú vị.

Đó chính là sức mạnh kỳ diệu của dữ liệu. Chỉ riêng việc ghi lại dữ liệu một cách trực quan, thậm chí chỉ là những số thứ tự tăng dần đơn giản, cũng hoàn toàn có khả năng thay đổi hành vi của một con người. Tôi từng nghe có người chia sẻ: "Ban đầu tôi chỉ hy vọng kiên trì chạy được liên tục 100 ngày, thế mà cuối cùng không ngờ mình lại có thể kiên trì chạy tới hơn 800 ngày."

Một ví dụ tương tự là cột lịch đóng góp (contribution graph) trên trang cá nhân GitHub của lập trình viên. Chỉ cần ngày hôm đó bạn có commit đẩy code lên hệ thống, ô vuông nhỏ của ngày đó sẽ chuyển sang màu xanh lục. Nếu trong suốt cả năm bạn coding đều đặn mỗi ngày, cả bảng lịch đóng góp sẽ được phủ kín một màu xanh lục mướt mắt, ngược lại sẽ xuất hiện những ô vuông màu trắng nhạt nhẽo. Bất kỳ ai ghé thăm trang cá nhân của bạn cũng đều nhìn thấy "bản đồ cống hiến" này.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091203.jpg)

Rất nhiều lập trình viên, chỉ để giữ cho chuỗi ngày xanh lục không bị đứt quãng, đã cố gắng duy trì thói quen viết code và commit đều đặn mỗi ngày. Qua thời gian dài tích lũy, họ thực sự đã hoàn thành được rất nhiều dự án giá trị.

Bài học rút ra ở đây là: Dù bạn đang làm bất kỳ công việc gì, việc ghi chép và phân tích dữ liệu liên tục đều đóng vai trò cực kỳ quan trọng. Đối với cá nhân, nó giúp bạn bứt phá từ một người chơi nghiệp dư trở thành một chuyên gia thực thụ; đối với sản phẩm công nghệ, nó giúp nâng tầm một ứng dụng thông thường trở thành một sản phẩm vận hành bằng dữ liệu (data product) mạnh mẽ.

## 资讯 (Tin tức)

1. **Iceland tổ chức lễ tưởng niệm chính thức cho Okjökull - sông băng đầu tiên biến mất do biến đổi khí hậu**

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082412.jpg)

Ngày 18/8, đất nước Iceland đã tổ chức một lễ tang đặc biệt để tiễn biệt dòng sông băng đầu tiên của quốc gia bị biến mất hoàn toàn, với sự tham dự trực tiếp của Thủ tướng Iceland. Đỉnh núi lửa Okjökull từng được bao phủ bởi một sông băng khổng lồ có diện tích lên tới 16 km². Tuy nhiên, đến năm 2014, dòng sông băng này đã gần như tan chảy hoàn toàn (ảnh trên). Ảnh chụp vệ tinh so sánh rõ rệt lớp tuyết phủ trắng xóa năm 1986 giờ chỉ còn lại một vệt băng mỏng nhỏ quanh miệng núi lửa vào năm nay (ảnh dưới).

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082411.jpg)

Hơn 200 người tham gia đã trèo lên đỉnh núi lửa để dựng một tấm bia tưởng niệm bằng đồng. Nội dung bia khắc lời cảnh báo đanh thép gửi tới thế hệ mai sau: Nếu loài người tiếp tục để khí hậu toàn cầu diễn biến xấu đi, trong vòng 200 năm tới, toàn bộ 400 dòng sông băng trên đảo quốc này sẽ chịu chung số phận tan biến vào hư vô.

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082413.jpg)

2. **Vụ án cáo buộc xâm nhập tài khoản ngân hàng trái phép từ không gian vũ trụ đầu tiên trong lịch sử**

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082508.jpg)

Anne Charlotte McClain - nữ phi hành gia người Mỹ tham gia nhiệm vụ trên Trạm Vũ trụ Quốc tế ISS từ tháng 12/2018 đến tháng 6/2019 - vừa bị cáo buộc đã bí mật truy cập vào tài khoản ngân hàng cá nhân của người vợ cũ (hai người đang thực hiện thủ tục ly hôn) bằng hệ thống mạng máy tính của trạm vũ trụ ISS.

Người vợ cũ đã nộp đơn tố cáo McClain lên Ủy ban Thương mại Liên bang (FTC) với cáo buộc xâm phạm tài khoản tài chính trái phép. Đây được ghi nhận là vụ án tranh chấp pháp lý đầu tiên trong lịch sử loài người liên quan đến một hành vi phạm pháp được thực hiện từ ngoài không gian vũ trụ.

3. **Thuế quan thương mại Mỹ - Trung đe dọa tăng chi phí nghiên cứu y học sinh học tại Hoa Kỳ**

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082512.jpg)

Giới nghiên cứu y sinh học Mỹ bày tỏ lo ngại sâu sắc trước việc chính quyền Trump áp thuế quan cao lên hàng hóa nhập khẩu từ Trung Quốc, do có tới 80% lượng linh trưởng phi nhân (chủ yếu là khỉ) phục vụ thí nghiệm y học tại các phòng lab Mỹ được nhập khẩu trực tiếp từ Trung Quốc. Đây là nguồn động vật thí nghiệm cốt lõi để nghiên cứu vắc-xin và thuốc điều trị các bệnh hiểm nghèo như AIDS, Ebola và Parkinson.

Theo Viện Y tế Quốc gia Mỹ (NIH), nhu cầu sử dụng khỉ thí nghiệm liên tục tăng cao trong khi ngân sách tài trợ nghiên cứu không đổi. Việc áp thuế quan làm tăng chi phí nhập khẩu khỉ thêm từ 5% đến 25% sẽ buộc các phòng lab phải thu hẹp quy mô dự án, hoặc chuyển dịch toàn bộ cơ sở nghiên cứu sang Trung Quốc. Chi phí thực hiện một ca thí nghiệm lâm sàng trên linh trưởng tại Trung Quốc ước tính chỉ khoảng 1.500 USD, trong khi con số này tại Mỹ lên tới hơn 6.000 USD.

4. **Nga vận hành nhà máy điện hạt nhân nổi đầu tiên trên thế giới tại khu vực Bắc Cực**

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082513.jpg)

Nga đã chính thức đưa vào vận hành Akademik Lomonosov - nhà máy điện hạt nhân nổi đầu tiên trên thế giới. Đây thực chất là một sà lan khổng lồ dài 144m, rộng 30m được trang bị hai lò phản ứng hạt nhân công suất lớn. Sà lan không tự di chuyển mà được các tàu kéo dắt dọc theo bờ biển Bắc Cực để di chuyển về cảng Pewek thuộc vùng Siberia lạnh giá.

Tổ chức bảo vệ môi trường Greenpeace lên tiếng phản đối gay gắt dự án này do lo ngại nguy cơ xảy ra thảm họa hạt nhân đe dọa trực tiếp hệ sinh thái mong manh vùng Bắc Cực. Tuy nhiên, giới chức Nga khẳng định sà lan hạt nhân này là giải pháp an toàn tối ưu để thay thế cho một nhà máy điện hạt nhân cũ kỹ xây dựng trên nền đất đóng băng vĩnh cửu (permafrost) đang bị sụt lún nghiêm trọng do hiện tượng nóng lên toàn cầu tại địa phương.

5. **Dự án đóng tàu robot tự hành Maxlimer chuẩn bị thực hiện hành trình vượt Đại Tây Dương**

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082702.jpg)

Mẫu tàu robot tự hành Maxlimer dài 11m do một công ty khởi nghiệp công nghệ Anh chế tạo đang hoàn tất các bước chuẩn bị cuối cùng cho chuyến hải trình tự lái vượt Đại Tây Dương. Do thiết kế tàu hoàn toàn không có thủy thủ đoàn nên khoang tàu tối ưu hóa được tối đa diện tích chứa hàng hóa vận tải. Khi di chuyển qua các vùng nước cảng biển đông đúc, tàu sẽ được điều khiển từ xa bởi các kỹ sư đất liền qua sóng vô lăng; khi ra biển khơi rộng lớn, tàu sẽ tự động chạy theo hệ dẫn đường định vị GPS.

Tàu đã hoàn thành nhiều đợt chạy thử nghiệm vận chuyển hàng hóa thành công giữa Anh và Bỉ từ khi ra mắt năm 2017. Theo kế hoạch, Maxlimer sẽ thực hiện hải trình nối giữa Anh và Na Uy trước khi tiến hành hành trình vượt Đại Tây Dương vào đầu năm 2020. Nếu thử nghiệm thành công, nó sẽ mở ra một chương mới cho ngành vận tải biển toàn cầu.

6. **Facebook chính thức ra mắt tính năng hẹn hò Facebook Dating tại nhiều thị trường**

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090601.jpg)

Facebook chính thức triển khai rộng rãi tính năng hẹn hò Facebook Dating tích hợp trực tiếp trên ứng dụng di động. Người dùng kích hoạt tính năng sẽ tạo một trang cá nhân hẹn hò riêng biệt tách hoàn toàn khỏi tài khoản cá nhân thông thường để chia sẻ hình ảnh và sở thích. Khi duyệt các hồ sơ khác, nếu có cảm tình bạn có thể bấm thả tim để gửi tín hiệu kết đôi.

Điểm thú vị là thuật toán AI của Facebook sẽ tự động phân tích hành vi và sở thích để gợi ý ghép cặp phù hợp từ danh sách những người dùng khác trong khu vực, bao gồm cả những người lạ có chung mối quan tâm và những người trong danh sách bạn bè (thông qua tính năng Secret Crush - Bạn thầm thương trộm nhớ).

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090602.jpg)

7. **FogCam - Hệ thống webcam phát trực tuyến lâu đời nhất thế giới tuyên bố dừng hoạt động sau 25 năm**

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019083008.jpg)

FogCam - hệ thống webcam truyền hình trực tuyến qua internet lâu đời nhất lịch sử công nghệ đặt tại Đại học Bang San Francisco - đã chính thức dừng hoạt động vào ngày 30/8 sau tròn 25 năm hoạt động liên tục từ năm 1994.

Hệ thống do hai sinh viên công nghệ thiết lập, hoạt động bằng cách chụp ảnh quang cảnh khuôn viên trường sau mỗi 1 phút rồi tự động tải ảnh lên trang web. Tên gọi "FogCam" xuất phát từ đặc trưng thời tiết nhiều sương mù của thành phố San Francisco. Lý do dừng hoạt động được ban quản trị chia sẻ là do nhà trường không còn bố trí được không gian đặt camera thích hợp và khó khăn trong việc duy trì hạ tầng máy chủ cũ kỹ. FogCam cũng được ghi nhận là một trong những trang web hoạt động liên tục lâu nhất trong lịch sử Internet.

8. **Tin vắn**

- Công ty bán dẫn Cerebras Systems của Mỹ công bố mẫu vi mạch tích hợp xử lý AI lớn nhất thế giới Wafer Scale Engine chứa tới 1.200 tỷ bóng bán dẫn (transitors), so với chỉ 2.300 bóng bán dẫn của vi xử lý Intel 4004 năm 1971.

- Twitter tuyên bố tạm khóa tính năng đăng tweet qua tin nhắn SMS sau khi tài khoản cá nhân của CEO Jack Dorsey bị hacker tấn công chiếm quyền kiểm soát bằng phương pháp tráo SIM (SIM swap) để đăng loạt nội dung nhạy cảm qua SMS.

- Quỹ Mozilla công bố dự án thử nghiệm Firefox Private Network cung cấp dịch vụ mạng proxy mã hóa HTTPS mặc định tích hợp sẵn trong trình duyệt cho người dùng Mỹ nhằm tăng cường bảo mật thông tin lướt web.

- Giao dịch chuyển khoản Bitcoin có trị giá tương đương 1 tỷ USD được ghi nhận thành công trên mạng blockchain với mức phí giao dịch cực thấp chỉ khoảng 600 USD - con số tối ưu không tưởng đối với hệ thống ngân hàng truyền thống.

- Tàu đổ bộ mặt trăng Vikram của Ấn Độ bị mất tín hiệu liên lạc hoàn toàn khi chỉ còn cách bề mặt Mặt Trăng khoảng 2 km trong quá trình hạ cánh tự động, đánh dấu thử nghiệm đổ bộ mặt trăng thất bại đầy tiếc nuối của nước này (ảnh dưới).

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090703.jpg)

## 文章 (Bài viết)

1、[Bài viết] [Tại sao sự phát triển kinh tế xóa đói giảm nghèo tại các vùng sâu vùng xa của Trung Quốc lại diễn ra thành công?](https://finance.sina.cn/china/gncj/2019-05-31/detail-ihvhiqay2662671.d.html) (Tiếng Trung)

Bài viết lược dịch một câu trả lời nhận được lượng bình chọn cao nhất trên Quora giải đáp câu hỏi: Tại sao Trung Quốc chi rất nhiều tiền đầu tư hạ tầng ở nước ngoài nhưng vẫn dành nguồn lực khổng lồ để phát triển các vùng núi nghèo khó nội địa? Bài viết phân tích chi tiết chiến lược xây dựng lưới điện quốc gia, phổ cập đường giao thông nông thôn và hạ tầng viễn thông 4G phủ sóng vùng cao giúp thúc đẩy thương mại điện tử nông thôn phát triển bền vững.

2、[Bài viết] [Những sự kiện lịch sử diễn ra đồng thời cùng thời điểm nhưng mang cảm giác thuộc hai thời đại hoàn toàn khác nhau](https://www.zhihu.com/question/333199024/answer/746004419) (Tiếng Trung)

Tổng hợp các sự kiện lịch sử thú vị trên Zhihu. Ví dụ tiêu biểu nhất: "Vào đúng năm nhà bác học Albert Einstein công bố Thuyết tương đối hẹp (1905), triều đình nhà Thanh tại Trung Quốc mới chính thức tuyên bố bãi bỏ hoàn toàn chế độ thi cử khoa cử phong kiến kéo dài hàng nghìn năm".

3、[Bài viết] [Làm sao để thiết kế hệ thống chạy sandbox mã nguồn JavaScript của bên thứ ba an toàn trên trang web?](https://www.figma.com/blog/how-we-built-the-figma-plugin-system/) (Tiếng Anh)

Figma là ứng dụng thiết kế chạy trực tiếp trên nền web hỗ trợ kho plugin phong phú từ cộng đồng. Bài viết chia sẻ hành trình thiết kế hệ thống sandbox an toàn để cô lập mã nguồn của bên thứ ba không làm ảnh hưởng đến bộ nhớ và bảo mật của trang chính, đi từ việc dùng iframe, worker đến giải pháp tối ưu sử dụng đề xuất tiêu chuẩn Realm API mới.

4、[Bài viết] [Trực quan hóa cấu trúc hình học của hoa hướng dương theo tỷ lệ Vàng toán học](https://card.weibo.com/article/m/show/id/2309404407466321379574) (Tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082303.jpg)

Giải thích chi tiết bằng hình ảnh mô phỏng toán học tại sao cấu trúc sắp xếp hạt trên nhụy hoa hướng dương hay mắt quả thông luôn tuân theo tỷ lệ Vàng 1.618. Tỷ lệ toán học vô tỷ đặc biệt này giúp tối ưu hóa không gian phân bổ hạt đều nhất trên mặt phẳng tròn mà không bị chồng chéo lãng phí diện tích.

## 软件 (Phần mềm)

1、[formik — Thư viện hỗ trợ xây dựng và quản lý trạng thái biểu mẫu (form) tinh gọn trong React](https://github.com/jaredpalmer/formik)

Giúp giảm thiểu tối đa lượng boilerplate code tẻ nhạt khi xử lý dữ liệu form, kiểm thử tính hợp lệ của dữ liệu đầu vào (validation) và quản lý trạng thái submit dữ liệu dễ dàng hơn.

2、[Antmove — Bộ công cụ hỗ trợ chuyển đổi mã nguồn ứng dụng nhỏ Mini Program đa nền tảng](https://github.com/ant-move/antmove)

Hỗ trợ biên dịch nhanh toàn bộ mã nguồn dự án WeChat Mini Program sang định dạng chạy trên Alipay Mini Program chỉ với một dòng lệnh, giúp lập trình viên không phải viết lại code từ đầu.

3、[oktools — Trang web tổng hợp các công cụ trực tuyến tiện lợi dành cho lập trình viên](https://oktools.net/)

Cung cấp nhanh các công cụ thông dụng chạy trực tiếp trên web: định dạng JSON, mã hóa Base64, chuyển đổi mã màu Hex/RGB, nén ảnh, kiểm thử biểu thức chính quy Regex, đổi dấu thời gian Epoch Timestamp và tính toán mã băm Hash.

4、[Tone.js — Thư viện Web Audio framework mạnh mẽ tạo hiệu ứng âm thanh và nhạc cụ trên web](https://github.com/Tonejs/Tone.js)

Cung cấp bộ API hướng đối tượng giúp các nhà phát triển web xây dựng các ứng dụng chơi nhạc, tổng hợp âm thanh (synthesizers), tạo hiệu ứng trễ (delay), méo tiếng (distortion) trực tiếp trên trình duyệt.

## 资源 (Tài nguyên)

1、[Tài liệu] [Deep Learning PM - Cẩm nang hướng dẫn hiểu sâu về học sâu dành cho Product Manager](https://easyai.tech/blog/65pdf-pm-understand-dl/) (PDF)

Tài liệu tiếng Trung dài 65 trang trình bày trực quan bằng hình vẽ các khái niệm cốt lõi của mạng nơ-ron nhân tạo, học sâu và ứng dụng thực tế giúp các quản trị sản phẩm dễ dàng phối hợp làm việc cùng đội ngũ kỹ sư AI.

2、[Bản đồ] [Global Coal Plant Tracker - Bản đồ tương tác hiển thị vị trí các nhà máy nhiệt điện than toàn cầu](https://www.carbonbrief.org/mapped-worlds-coal-power-plants)

Bản đồ trực quan hiển thị vị trí địa lý, công suất hoạt động, lượng phát thải CO₂ và trạng thái vận hành của hàng nghìn nhà máy nhiệt điện than trên khắp thế giới.

## 图片 (Hình ảnh)

1. **Bức ảnh đen trắng đánh lừa thị giác người xem bằng các đường lưới màu sắc**

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019080201.jpg)

Khi nhìn vào bức ảnh trên, bộ não của bạn sẽ tự động điền các mảng màu để cảm nhận đây là một bức ảnh màu sống động. Tuy nhiên thực chất đây hoàn toàn là một bức ảnh đen trắng gốc, chỉ có các đường lưới màu sắc (color grid lines) được vẽ đè lên trên. Hiệu ứng này chứng minh trong hệ thống thị giác của con người, thông tin về độ sáng (luminance) đóng vai trò quyết định hơn thông tin về màu sắc (chrominance) khi não bộ tái tạo hình ảnh.

## 言论 (Danh ngôn)

1、

> "Thói quen tai hại của nhiều lập trình viên, đặc biệt là các bạn trẻ, là họ dành quá nhiều năng lực trí óc chỉ để tìm hiểu sâu về bản thân việc lập trình. Họ say mê học các cú pháp lạ lẫm của ngôn ngữ, các mẹo thiết lập hệ thống kiểu dữ liệu (type system), các chi tiết vận hành sâu của những thư viện UI JavaScript khổng lồ, nhưng lại quên mất việc dành thời gian để thấu hiểu sâu sắc lĩnh vực chuyên môn (domain knowledge) của bài toán thực tế mà họ đang cần viết phần mềm để giải quyết."
> 
> -- Rich Hickey, cha đẻ ngôn ngữ lập trình Clojure

## 招聘信息 (Thông tin tuyển dụng)

Dưới đây là thông tin tuyển dụng từ các doanh nghiệp đối tác tài trợ cho bản tin.

Các vị trí tuyển dụng và thực tập miễn phí khác luôn được cập nhật tại [mục thảo luận tuyển dụng trên GitHub](https://github.com/ruanyf/weekly/issues/798).

1、**Cryptape (Mật Viên Khoa Học)**

Doanh nghiệp khởi nghiệp công nghệ blockchain chuyên phát triển hạ tầng và dịch vụ blockchain cho nền kinh tế mã hóa, các sản phẩm chính gồm Nervos, Huobi Finance Chain, CITA. Địa điểm làm việc: Hàng Châu hoặc làm việc từ xa (remote).

Các vị trí đang tuyển dụng:
- Kỹ sư Blockchain cao cấp (yêu cầu thành thạo Rust)
- Kỹ sư Backend cao cấp (kinh nghiệm phát triển hệ thống phân tán)
- Trưởng phòng An ninh thông tin (CSO) (trên 5 năm kinh nghiệm bảo mật)
- Trưởng phòng Kiểm thử cao cấp (kiểm thử tự động hóa blockchain)

Chi tiết công việc và yêu cầu tuyển dụng xem tại [đây](https://github.com/ruanyf/weekly/issues/798#issuecomment-524289916).

Nộp hồ sơ trực tiếp tới Email: [zhouyun@cryptape.com](mailto:zhouyun@cryptape.com) (phản hồi trong vòng 24h).

(Hết)
