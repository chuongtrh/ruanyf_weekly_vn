# 科技爱好者周刊：第 93 期 (Bản tin chia sẻ công nghệ số 93)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121509.jpg)

Ảnh bìa: Các đụn cát khổng lồ trên bề mặt Sao Hỏa. Ảnh từ [NASA](https://www.jpl.nasa.gov/spaceimages/details.php?id=PIA20755).

## 刊首语 (Lời tựa)

Trong kỳ nghỉ lễ vừa qua, tôi dành khá nhiều thời gian rảnh rỗi để chơi trò chơi điện tử tại nhà.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020509.jpg)

Có nhà phê bình từng nhận định rằng, thế giới trò chơi điện tử được chia thành hai trường phái chính: Một là dòng game định hướng mục tiêu rõ ràng - người chơi phải tìm cách đánh bại mọi đối thủ, vượt qua các thử thách kỹ năng để giành chiến thắng cuối cùng; Hai là dòng game phi mục tiêu - trò chơi được thiết kế chỉ để kể một câu chuyện nghệ thuật hoặc mang lại trải nghiệm phiêu lưu, dạo chơi tự do trong một không gian ảo tuyệt đẹp.

Tôi nhận ra bản thân ngày càng trở nên thờ ơ với dòng game thứ nhất, hoàn toàn mất đi hứng thú với các mô hình lặp đi lặp lại dạng "diệt quái vật, thăng cấp, làm nhiệm vụ tuyến tính và thu thập trang bị". Ngược lại, tôi đặc biệt yêu thích cảm giác được thong thả dạo chơi và khám phá thế giới ảo trong game, tương tự như chuyến tham quan ngắm cảnh tại một thành phố xa lạ: không có nhiệm vụ bắt buộc phải làm, không có chướng ngại vật buộc phải vượt qua, không cần thu thập vật phẩm, không chiến đấu với ai và cũng không lo sợ kẻ địch bất ngờ xuất hiện từ các góc khuất. Hễ bắt gặp một phong cảnh hay kiến trúc đẹp mắt, tôi sẽ dừng lại và thư thái thưởng thức.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020503.jpg)

Một tựa game kinh điển thuộc dòng này là [《Dear Esther》](https://www.douban.com/game/19974701/) (Thư gửi Esther), được đánh giá là một trong những tác phẩm game mang đậm tính văn học nghệ thuật nhất lịch sử. Giới phê bình thậm chí nhận xét đây không phải là một trò chơi thông thường mà là một cuốn tiểu thuyết tương tác trực quan: "Một bức di chúc đầy chất thơ về sự u sầu, cô độc và tĩnh lặng". Người chơi được đưa lên một hòn đảo hoang vắng, phong cảnh thiên nhiên hoang sơ hùng vĩ kết hợp cùng những bản nhạc không lời da diết vang lên theo tiếng sóng biển. Bạn chỉ việc thong thả dạo bước trên đảo, lắng nghe giọng đọc truyền cảm của một người đàn ông vô danh gửi cho người vợ đã khuất của mình. Dựa trên nội dung các bức thư và các dấu vết khảo sát trên đảo, bạn sẽ tự mình xâu chuỗi để phác họa lại câu chuyện đã xảy ra. Lối chơi này vô cùng phù hợp với gu thưởng thức của tôi.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020504.jpg)

Trong tâm trí tôi, một tựa game tuyệt vời cần mang lại trải nghiệm: người chơi được đắm chìm vào trong một cốt truyện sâu sắc, được hỗ trợ bởi một thế giới ảo mỹ thuật lộng lẫy và sống động để kích thích khát vọng khám phá mọi ngóc ngách của câu chuyện. Quá trình trải nghiệm game giống như một chuyến du lịch thư giãn, nơi bạn thong thả tương tác với môi trường xung quanh và kiên nhẫn chờ đợi các tình tiết truyện tự nhiên mở ra.

Tôi tin rằng trong tương lai, xu hướng phát triển các dòng game dạng "tiểu thuyết số thực tế ảo" này sẽ ngày càng phát triển mạnh mẽ. Về bề nổi, bạn đang chơi game, nhưng về bản chất, bạn đang trực tiếp bước vào trang sách, hóa thân thành nhân vật để trải nghiệm và định hình thế giới của cuốn tiểu thuyết đó.

## Khóa học Python thực chiến 50 ngày cùng chuyên gia

Kỳ nghỉ lễ kéo dài là thời điểm vô cùng thích hợp để các nhà phát triển tranh thủ nâng cao trình độ chuyên môn qua các khóa học trực tuyến chất lượng cao.

Ngôn ngữ Python là công cụ cơ bản gần như bắt buộc phải có của mọi kỹ sư phần mềm, được ứng dụng rộng rãi từ mảng web cho đến xử lý dữ liệu. Tuy nhiên, nếu bạn nhận thấy việc tự học Python qua các tài liệu rời rạc trên mạng thiếu đi tính hệ thống và không có chuyên gia hỗ trợ giải đáp thắc mắc khi gặp lỗi code khó, hãy tham khảo khóa học chuyên sâu của nền tảng Geekbang.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020508.jpg)

Geekbang là một trong những nền tảng đào tạo công nghệ uy tín hàng đầu hiện nay. Khóa học **《Python Bootcamp: 50 ngày nâng cao năng lực lập trình thực chiến》** được thiết kế bài bản bởi chuyên gia Doãn Hội Sinh, hướng tới mục tiêu giúp các lập trình viên đã nắm vững cú pháp cơ bản nhanh chóng nâng cao trình độ thực chiến qua các dự án thực tế.

Chương trình áp dụng mô hình giảng dạy tương tác trực tuyến, kết hợp cùng các bài tập thực hành hàng tuần, có trợ giảng hỗ trợ giải đáp lỗi code 24/7 và giảng viên theo sát tiến độ.

Nội dung khóa học đi từ việc xây dựng một hệ thống cào dữ liệu (crawler) đơn luồng đơn giản, nâng cấp lên đa luồng tối ưu hiệu năng, tiếp theo là các công đoạn lưu trữ cơ sở dữ liệu, làm sạch dữ liệu thô, phân tích từ vựng và phân tích cảm xúc (Sentiment Analysis), và kết thúc bằng việc xây dựng giao diện Web trực quan hóa số liệu đã xử lý. Đây là nền tảng vô cùng vững chắc cho các bạn muốn chuyển dịch sang mảng phát triển Web, xử lý dữ liệu lớn, xử lý ngôn ngữ tự nhiên NLP hay AI.

[![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020506.jpg)](https://cdn.beekka.com/blogimg/asset/202002/bg2020020505.jpg)

Học viên hoàn thành khóa học sẽ nhận được đặc quyền **giới thiệu ứng tuyển trực tiếp 2 lần trong năm vào các tập đoàn công nghệ lớn** và mạng lưới hơn 600 doanh nghiệp liên kết của TGO.

Khóa học đang áp dụng mức giá ưu đãi từ 3.600 Nhân dân tệ giảm còn 1.999 Nhân dân tệ. Độc giả bản tin có thể sử dụng mã giảm giá độc quyền: **PYRUANYFE** để được giảm thêm 200 Nhân dân tệ, mức học phí cuối cùng chỉ còn **1.799 Nhân dân tệ**. Quét mã QR dưới đây để tìm hiểu chi tiết:

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020507.jpg)

## 资讯 (Tin tức)

1. **Tòa án Thâm Quyến ra phán quyết khẳng định tác phẩm do AI tạo ra vẫn được bảo hộ bản quyền**

Tòa án Nhân dân Quận Nam Sơn (Thâm Quyến) mới đây đã đưa ra một phán quyết mang tính lịch sử đối với ngành luật sở hữu trí tuệ: Thừa nhận các bài viết báo chí do hệ thống trí tuệ nhân tạo tự động viết ra vẫn được bảo hộ quyền tác giả. Vụ kiện do tập đoàn Tencent khởi kiện một công ty dịch vụ thông tin tại Thượng Hải vì hành vi tự ý sao chép lại bài viết phân tích tài chính do robot viết báo Dreamwriter của Tencent tự động biên soạn đăng trên cổng thông tin tài chính của hãng. Tòa án tuyên án Tencent thắng kiện, yêu cầu bị đơn gỡ bỏ toàn bộ bài viết vi phạm và bồi thường thiệt hại.

Dreamwriter là hệ thống robot viết báo tự động được Tencent phát triển từ năm 2015, chuyên tự động phân tích dữ liệu thị trường chứng khoán, báo cáo tài chính doanh nghiệp để sinh ra các bài viết tin tức tài chính nhanh chóng trong vài giây.

Việc tác phẩm do AI tạo ra có được bảo hộ quyền tác giả hay không luôn là chủ đề tranh cãi lớn của luật pháp quốc tế. Luật bản quyền của Mỹ hiện nay quy định rõ ràng luật chỉ bảo hộ cho các thành quả lao động sáng tạo trực tiếp từ trí tuệ của con người, các tác phẩm do máy tính tự sinh không được bảo hộ. Một tòa án tại Úc vào năm 2012 cũng đưa ra phán quyết tương tự đối với các tác phẩm có sự can thiệp tự động hóa của máy tính. Phán quyết mới của tòa án Thâm Quyến mở ra một tiền lệ pháp lý mới rất đáng quan tâm.

2. **Hệ thống thông tin vệ sinh di động vệ tinh đầu tiên do Trung Quốc tự xây dựng đi vào thương mại**

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011304.jpg)

Hệ thống thông tin di động vệ tinh tự chủ đầu tiên của Trung Quốc - hệ thống Thiên Thông chính thức đi vào hoạt động thương mại thông qua sự vận hành của nhà mạng China Telecom. Dịch vụ sử dụng đầu số chuyên dụng 1740, cung cấp cả các dòng thiết bị cầm tay chạy hệ điều hành Android và thiết bị lắp trên xe ô tô chuyên dụng. Người dùng cũng có thể kết nối điện thoại thông minh cá nhân với thiết bị đầu cuối thông qua ứng dụng di động để gọi điện vệ tinh.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011305.jpg)

Hệ thống đã chạy thử nghiệm từ tháng 3/2018 và thu hút khoảng 30.000 khách hàng tham gia trải nghiệm. Gói cước thương mại có mức giá khoảng 1.000 Nhân dân tệ/năm, bao gồm 750 phút gọi thoại vệ tinh.

Hệ thống liên lạc vệ tinh đóng vai trò vô cùng quan trọng đảm bảo duy trì kết nối thông tin liên lạc tại các vùng biển xa, sa mạc hay khu vực thiên tai mất sóng viễn thông mặt đất. Hiện tại hệ thống Thiên Thông mới chỉ vận hành với 1 vệ tinh Thiên Thông 1 (phóng tháng 8/2016) nên phạm vi phủ sóng mới chỉ bao trùm toàn bộ lãnh thổ Trung Quốc, chưa thể phủ sóng toàn cầu như hệ thống vệ tinh Iridium.

3. **Làn sóng mở các trung tâm luyện thi phỏng vấn bằng AI bùng nổ tại Hàn Quốc**

Do nhiều tập đoàn kinh tế lớn tại Hàn Quốc bắt đầu áp dụng các hệ thống lọc hồ sơ và phỏng vấn tự động bằng trí tuệ nhân tạo (AI Hiring Bots) để đánh giá ứng viên, thị trường giáo dục nước này đã nhanh chóng xuất hiện các trung tâm ôn luyện phỏng vấn AI chuyên biệt. Các trung tâm cung cấp hệ thống phần mềm phỏng vấn giả định giúp ứng viên rèn luyện biểu cảm khuôn mặt trước camera để đạt điểm số tối ưu từ thuật toán nhận diện. Ví dụ: khi mỉm cười trước camera, ứng viên được khuyên không nên há miệng quá to mà nên mỉm cười bằng ánh mắt để tạo cảm giác tự nhiên cho thuật toán.

Mức học phí cho một buổi luyện tập phỏng vấn giả lập bằng phần mềm AI kéo dài 3 giờ có chi phí lên tới 100.000 Won (tương đương khoảng 2 triệu VNĐ).

4. **Florida ứng dụng mô hình青 vẹt nhân tạo thay thế cho thí nghiệm giải phẫu sinh học cấp ba**

Các trường trung học phổ thông tại bang Florida (Mỹ) đang thí điểm đưa vào giảng dạy mô hình青 vẹt nhân tạo (Synthetic Frogs) chất lượng cao để thay thế cho việc giải phẫu ếch thật trong các giờ thực hành sinh học nhằm bảo vệ số lượng loài lưỡng cư hoang dã.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020010301.jpg)

Mô hình được chế tác vô cùng tinh xảo từ chất liệu polymer đặc biệt, mang lại cảm giác bề mặt da và độ đàn hồi cơ học tương tự như ếch thật. Khi học sinh dùng dao mổ rạch bụng mô hình, họ sẽ quan sát thấy đầy đủ cấu trúc các lớp cơ, hệ thống các cơ quan nội tạng và trứng ếch mô phỏng chi tiết. Việc sử dụng mô hình giúp loại bỏ hoàn toàn mùi hóa chất bảo quản formalin độc hại tại các phòng thực hành, và mô hình có khả năng tái sử dụng nhiều lần sau khi thực hành xong. Mức giá thương mại cho mỗi mô hình khoảng 150 USD.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020010303.jpg)

5. **Ứng dụng WiFi Master Key bị tòa án bác bỏ yêu cầu đăng ký bảo hộ nhãn hiệu thương mại**

Tòa án Nhân dân Tối cao Bắc Kinh đưa ra phán quyết bác bỏ yêu cầu đăng ký nhãn hiệu thương mại cho ứng dụng "WiFi万能钥匙" (WiFi Master Key) của doanh nghiệp sở hữu. Tòa án nhận định cụm từ "WiFi" đại diện cho công nghệ kết nối không dây phổ biến, còn "万能钥匙" (chìa khóa vạn năng) là cách gọi dân gian chỉ các hành vi bẻ khóa, dò mật khẩu mạng không dây.

Việc đăng ký nhãn hiệu thương mại chứa cụm từ này dễ khiến người tiêu dùng phổ thông hiểu lầm về bản chất và tính hợp pháp của dịch vụ, mang tính chất lừa dối khách hàng nên không được phép đăng ký bảo hộ độc quyền nhãn hiệu.

6. **Tin vắn**

- Cục Hàng không Liên bang Mỹ (FAA) đề xuất quy định bắt buộc mọi dòng thiết bị bay không người lái (UAV) phải được trang bị hệ thống định danh vô tuyến từ xa (Remote ID) để hỗ trợ công tác quản lý an ninh hàng không.

- Khảo sát của Nielsen chỉ ra xu hướng tiêu dùng phương tiện truyền thông mới: có tới 88% người dân Mỹ có thói quen sử dụng điện thoại thông minh song song khi đang bật tivi xem các chương trình giải trí.

- Người dùng công nghệ chia sẻ mẹo tản nhiệt độc đáo cho máy tính nhúng Raspberry Pi 4: chỉ cần đặt một đồng xu kim loại lên trên bề mặt chip CPU có thể giúp giảm nhiệt độ hoạt động của chip xuống 10 độ C tức thì.

## 文章 (Bài viết)

1、[Bài viết] [Khám phá câu chuyện hậu trường thú vị về đội ngũ kỹ sư phát triển thư viện React](https://reactjs.org/community/team.html) (Tiếng Anh)

Trang giới thiệu chính thức về đội ngũ nhân sự phát triển mã nguồn mở React trên trang chủ: giới thiệu hình ảnh chân dung cá nhân và những dòng tự sự ngắn gọn, hài hước về công việc hàng ngày của 10 kỹ sư nòng cốt phát triển dự án.

2、[Bài viết] [Hành trình chuyển dịch toàn bộ hệ thống từ Python sang ngôn ngữ Go của Khan Academy](https://engineering.khanacademy.org/posts/goliath.htm) (Tiếng Anh)

Đội ngũ kỹ sư của nền tảng giáo dục Khan Academy chia sẻ chi tiết về quyết định không nâng cấp hệ thống mã nguồn Python 2 khổng lồ lên Python 3, mà quyết định viết lại toàn bộ kiến trúc backend sang ngôn ngữ Go để tối ưu hóa hiệu năng xử lý đồng thời và giảm chi phí vận hành máy chủ.

3、[Bài viết] [Lịch sử bức ảnh đầu tiên được tải lên mạng xã hội Instagram năm 2010](https://birdeatsbug.com/real-first-post-on-instagram) (Tiếng Anh)

Bằng cách phân tích cấu trúc đánh số ID tuần tự của các tệp tin hình ảnh tải lên máy chủ Instagram, chuyên gia đã tìm ra bức ảnh đầu tiên được nhà sáng lập Kevin Systrom tải lên hệ thống vào ngày 16/7/2010: bức ảnh chụp một chú chó nhỏ bên cạnh đôi dép lê của vợ anh tại một quán ăn ven đường với dòng mô tả đơn giản "Test".

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122405.jpg)

## 软件 (Phần mềm)

1、[kutt — Trình rút gọn liên kết web mã nguồn mở bảo mật viết bằng Node.js](https://github.com/thedevs-network/kutt)

Cung cấp giải pháp tự dựng máy chủ rút ngắn link chuyên nghiệp: hỗ trợ cấu hình tên miền riêng, thiết lập mật khẩu bảo vệ cho liên kết, đặt thời hạn hết hạn link và tích hợp trang quản trị phân tích chi tiết lượng truy cập.

2、[tesseract.js — Thư viện JavaScript hỗ trợ nhận dạng chữ viết hình ảnh (OCR) trực tiếp trên trình duyệt](https://github.com/naptha/tesseract.js)

Giải pháp nhận dạng ký tự quang học OCR mạnh mẽ được biên dịch từ công cụ Tesseract nổi tiếng của Google sang WebAssembly, cho phép chạy trực tiếp trên trình duyệt web của client để nhận dạng hơn 100 ngôn ngữ khác nhau mà không cần gửi hình ảnh lên server.

3、[linkding — Tiện ích tự lưu trữ danh sách bookmark tên miền cá nhân tối giản](https://github.com/sissbruecker/linkding)

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122610.jpg)

Công cụ viết bằng Python/Django hỗ trợ người dùng tự dựng một trang quản lý các đường dẫn website ưa thích gọn nhẹ, hỗ trợ gắn tag phân loại, tìm kiếm nhanh và giao diện tối giản hỗ trợ chế độ tối (dark mode).

## 资源 (Tài nguyên)

1、[Tài liệu] [Tổng hợp 60 xu hướng phát triển công nghệ đột phá của năm 2020](https://danieleckler.com/2020/)

Trang web tổng hợp và phân tích chi tiết về 60 công nghệ ngách đầy tiềm năng được dự báo sẽ bứt phá mạnh mẽ trong năm 2020: từ các giải pháp thịt nhân tạo, mạng 5G cho tới các thiết bị y tế đeo thông minh.

## 图片 (Hình ảnh)

1. **Cầu rễ cây sống (Living Root Bridges) - Kỳ quan kiến trúc xanh độc đáo tại Ấn Độ**

Tại vùng Meghalaya của Ấn Độ, người dân bản địa đã phát triển một phương pháp xây dựng cầu treo tự nhiên vô cùng độc đáo bằng cách tận dụng hệ rễ phụ (rễ khí sinh) của loài cây đa cao su bản địa để dẫn hướng qua các dòng sông lớn.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112307.jpg)

Quy trình xây dựng kéo dài hàng thập kỷ: người dân đặt các thân tre hoặc cây cọ làm khung dẫn hướng bắc ngang sông, sau đó quấn các rễ cây non bò theo khung sang bờ bên kia và cắm xuống đất trồng. Theo thời gian, hệ rễ cây ngày càng phát triển to khỏe, đan xen chặt chẽ tạo thành một cây cầu treo tự nhiên vô cùng vững chãi có chiều dài lên tới 50 mét và tuổi thọ sử dụng kéo dài hàng trăm năm mà không lo bị mục nát trong điều kiện khí hậu mưa nhiều của vùng nhiệt đới.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112306.jpg)

## 文摘 (Văn trích)

1. **Magdeburg Water Bridge - Nguyên lý vật lý thú vị đằng sau cây cầu nước khổng lồ tại Đức**

Cây cầu nước Magdeburg tại Đức là một công trình kiến trúc thủy lợi vĩ đại bắc ngang qua sông Elbe, điểm đặc biệt là cây cầu này không phục vụ cho xe cộ di chuyển mà là một kênh dẫn nước phục vụ cho các tàu bè qua lại giữa hai hệ thống kênh vận tải lớn của khu vực.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112518.jpg)

Dưới góc nhìn vật lý kiến trúc, một câu hỏi thú vị được đặt ra: liệu khi có các tàu tải trọng hàng vạn tấn di chuyển qua cầu, kết cấu của cây cầu có phải chịu thêm một lực đè nặng tương đương trọng lượng của con tàu đó hay không?

Câu trả lời là hoàn toàn không. Bất kể trên cầu có tàu di chuyển hay không, lực đè nặng lên mặt cầu luôn được duy trì ở một mức không đổi.

Theo nguyên lý lực đẩy Archimedes, khi một con tàu di chuyển vào kênh nước trên cầu, nó sẽ chiếm chỗ và đẩy một lượng nước có trọng lượng đúng bằng trọng lượng của con tàu đó ra ngoài. Do hệ thống kênh nước trên cầu được liên thông trực tiếp với hệ thống kênh vận tải dài vô hạn ở hai đầu cầu, lượng nước bị chiếm chỗ này sẽ tự động chảy tản ra toàn bộ hệ thống kênh bên ngoài. Kết quả là, tổng trọng lượng của hệ thống nước và tàu nằm trên cầu luôn bằng đúng trọng lượng của khối nước ban đầu khi chưa có tàu. Cây cầu nước vì thế không phải chịu thêm bất kỳ lực tải trọng phát sinh nào từ các đoàn tàu.

## 言论 (Danh ngôn)

1、

> "Toàn bộ các dự án công nghệ của tỷ phú Elon Musk dường như đều được thiết kế để chuẩn bị cho các kịch bản thất bại lớn của nhân loại trên trái đất:
> 
> Khi hệ thống điện lưới quốc gia tê liệt, hệ thống điện mặt trời SolarCity sẽ phát huy tác dụng. Khi nguồn dầu mỏ khan hiếm, xe điện Tesla sẽ đảm nhận vai trò giao thông. Khi hệ thống internet mặt đất bị cắt đứt, chòm sao vệ tinh Starlink sẽ duy trì kết nối. Và khi trái đất không còn là nơi có thể cư trú, con người sẽ di cư sang Sao Hỏa bằng phi thuyền SpaceX."
> 
> -- Nhận xét của người dùng công nghệ trên mạng xã hội

(Hết)
