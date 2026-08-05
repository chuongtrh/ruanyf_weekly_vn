# 科技爱好者周刊：第 80 期 (Bản tin chia sẻ công nghệ số 80)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019103101.jpg)

Ảnh bìa: Bến tàu du thuyền Hậu灘 (Houtan), Thượng Hải, 2019.

## 刊首语 (Lời tựa)

Rất nhiều lập trình viên khi khởi nghiệp thường lựa chọn xây dựng các công cụ phát triển phần mềm (Developer Tools) dành cho các lập trình viên khác, tập trung khai thác thị trường B2B (Doanh nghiệp) cho giới công nghệ.

Tư duy đằng sau hướng đi này khá đơn giản: "Tôi là lập trình viên nên tôi hiểu rõ giới lập trình đang cần những công cụ gì. Tôi tự tay phát triển nó và nếu bạn thấy hữu ích, bạn sẽ đề xuất doanh nghiệp của mình chi tiền mua bản quyền sử dụng". Mô hình này có thể vận hành tốt tại thị trường nước ngoài nhưng tôi cho rằng nó sẽ gặp vô vàn thách thức tại thị trường Trung Quốc. **Khởi nghiệp phát triển công cụ phát triển phần mềm cho doanh nghiệp cực kỳ khó sống sót tại Việt Nam và Trung Quốc.**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019103102.jpg)

Nguyên nhân cốt lõi là do ngân sách và ý chí chi tiền mua các công cụ phần mềm quản lý, phát triển của các doanh nghiệp trong nước còn rất hạn chế, đặc biệt là đối với sản phẩm từ các công ty startup non trẻ. Phần lớn các doanh nghiệp trong nước không hoạt động theo mô hình định hướng công nghệ thuần túy, những người đứng đầu ban quản trị thường không xuất thân từ kỹ thuật nên họ không thấu hiểu sâu sắc nhu cầu thực tế của các kỹ sư. Người đứng đầu bộ phận công nghệ (CTO/IT Director) trong doanh nghiệp thường không đóng vai trò quyết định tối cao trong việc phê duyệt ngân sách. Dù toàn bộ lập trình viên trong phòng ban đều thấy công cụ này cực tốt, họ cũng không có đủ tầm ảnh hưởng để thuyết phục ban lãnh đạo ký duyệt chi tiền.

Vậy tại sao vị thế của các kỹ sư công nghệ trong cấu trúc doanh nghiệp trong nước thường không chiếm vai trò chủ đạo và thiếu tiếng nói quyết định trước ban lãnh đạo?

**Bởi vì đối với đa số doanh nghiệp trong nước, công nghệ cốt lõi chưa phải là yếu tố tiên quyết quyết định sự sống còn của doanh nghiệp, mà các yếu tố phi công nghệ (như năng lực gọi vốn, quan hệ khách hàng) lại có tầm ảnh hưởng lớn hơn rất nhiều.** Lấy ví dụ về khởi nghiệp công nghệ: chỉ cần có công nghệ tốt là có thể khởi nghiệp thành công? Chưa chắc. Mô hình phổ biến nhất hiện nay là: tìm kiếm một cơ hội thị trường đang nóng, soạn thảo một bản kế hoạch kinh doanh và chuẩn bị slide PPT ấn tượng để đi gặp các quỹ đầu tư mạo hiểm. Một khi dòng tiền đầu tư đã đổ về, doanh nghiệp sẽ dùng tiền đó để thuê các lập trình viên giỏi về hiện thực hóa sản phẩm.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019103103.jpg)

Hệ quả là, người sáng lập và cổ đông lớn nhất của công ty thường không phải là người có trình độ kỹ thuật giỏi nhất, mà là người có năng lực tìm kiếm dòng vốn tốt nhất. **Đây chính là lý do tại sao người đại diện pháp luật hay cổ đông lớn của các startup công nghệ trong nước thường không xuất thân từ lập trình viên.** Lập trình viên bản chất vẫn là lực lượng lao động trí óc cao cấp được thuê về và có rất ít tiếng nói quyết định đối với chiến lược cấp cao của doanh nghiệp.

Tóm lại, nếu bạn có ý định khởi nghiệp công nghệ trong nước, lời khuyên chân thành là hãy cân nhắc kỹ trước khi chọn hướng đi phát triển công cụ kỹ thuật dành cho doanh nghiệp. Việc này không chỉ gặp khó khăn ở khâu gọi vốn đầu tư mà khâu bán hàng thương mại (Sales) còn gian nan hơn rất nhiều. Thay vào đó, việc phát triển một sản phẩm hướng tới đại chúng (To-C), tích lũy được lượng người dùng thực tế ban đầu rồi mới đi gọi vốn sẽ là con đường có tỷ lệ thành công cao hơn hẳn.

## 资讯 (Tin tức)

1. **Thử nghiệm cấy hạt nano hỗ trợ thị giác đêm trực tiếp vào võng mạc mắt**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100303.jpg)

Các nhà khoa học Mỹ đang tiến hành nghiên cứu phương pháp cấy thiết bị nano hỗ trợ thị giác trực tiếp vào mắt người, giúp mắt thường có khả năng quan sát rõ vật thể trong bóng tối mà không cần đeo kính hồng ngoại.

Công nghệ này đã được thử nghiệm thành công trên chuột trong phòng thí nghiệm. Các nhà nghiên cứu đã tiêm các hạt nano đặc biệt có khả năng chuyển đổi ánh sáng hồng ngoại thành ánh sáng khả kiến vào võng mạc chuột. Các hạt nano này liên kết chặt chẽ với tế bào cảm quang trong mắt chuột, mang lại khả năng nhìn đêm ổn định trong suốt 10 tuần liên tục mà hoàn toàn không gây tác dụng phụ. Những chú chuột thử nghiệm dễ dàng định vị tìm đường thoát khỏi mê cung tối đen hoàn toàn.

Các dòng kính nhìn đêm quân sự truyền thống hoạt động dựa trên cảm biến bức xạ nhiệt từ môi trường xung quanh, có nhược điểm là cồng kềnh, nặng nề, góc nhìn hẹp và bắt buộc phải dùng nguồn pin đi kèm. Nếu giải pháp công nghệ sinh học mới này được chứng minh an toàn trên người, nó sẽ giúp loại bỏ hoàn toàn gánh nặng pin nguồn cho binh sĩ trên chiến trường và nâng cao khả năng cơ động phản ứng nhanh.

2. **Old Tjikko - Cây vân sam cổ xưa nhất thế giới với hệ rễ sống sót hơn 9.500 năm tại Thụy Điển**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019101501.jpg)

Cây cổ thụ lâu đời nhất thế giới được ghi nhận là một cây vân sam mang tên Old Tjikko, cao 4.8 mét tại Thụy Điển. Phân tích phóng xạ carbon-14 cho thấy hệ rễ của cây đã tồn tại ổn định suốt 9.500 năm qua.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019101502.jpg)

Điểm độc đáo gây [tranh luận](https://allthatsinteresting.com/old-tjikko) nằm ở chỗ chỉ có hệ rễ dưới lòng đất đạt tuổi thọ 9.500 năm, còn phần thân cây gỗ bên trên thực chất là chồi mới sinh trưởng chỉ vài trăm năm tuổi. Giống cây này có khả năng tự nhân bản vô tính: khi thân cây cũ già cỗi bị tuyết phủ gãy đổ, hệ rễ bên dưới vẫn tiếp tục sống sót và tự sinh chồi phát triển thành thân cây mới. Mỗi chu kỳ sống của phần thân gỗ kéo dài khoảng 600 năm.

Nếu chỉ tính riêng tuổi thọ của phần thân gỗ đơn lẻ liên tục trên mặt đất, kỷ lục thế giới thuộc về cây thông Methuselah tại bang California (Mỹ) với tuổi thọ đạt 4.768 năm.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019101503.jpg)

3. **Phát hiện nhiều báo cáo nhìn thấy loài Hổ Tasmania tưởng chừng đã tuyệt chủng ngoài tự nhiên**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019101702.jpg)

Hổ Tasmania (còn gọi là chó sói có túi Thylacine) từng là loài thú ăn thịt có túi phân bố rộng khắp châu Úc. Do các hoạt động săn bắn của con người, loài này dần co cụm và biến mất hoàn toàn. Điểm đặc trưng của chúng là có các sọc vằn trên lưng giống hổ và sở hữu chiếc túi trước bụng để nuôi con non tương tự như loài chuột túi.

Loài động vật này được coi là đã tuyệt chủng hoàn toàn sau khi cá thể cuối cùng chết tại vườn thú Hobart vào ngày 7/9/1936 (ảnh dưới). Tuy nhiên, báo cáo mới nhất của cơ quan quản lý động vật bang Tasmania tiết lộ trong 3 năm qua đã ghi nhận 8 báo cáo nhìn thấy loài thú này ngoài tự nhiên từ người dân địa phương. Các nhân chứng đều khẳng định đã quan sát thấy một loài động vật lớn giống mèo có sọc vằn đặc trưng trên lưng. Hiện nay, các nhà khoa học Úc vẫn duy trì dự án nghiên cứu hồi sinh loài hổ này thông qua công nghệ nhân bản vô tính DNA.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019101703.jpg)

4. **Chính phủ Singapore ban hành lệnh cấm quảng cáo đối với tất cả các dòng nước ngọt含糖饮料**

Singapore thông báo chính thức ban hành lệnh cấm quảng cáo trên mọi phương tiện truyền thông đối với các sản phẩm nước ngọt chứa lượng đường cao, trở thành quốc gia đầu tiên trên thế giới thực hiện biện pháp mạnh tay này. Lệnh cấm áp dụng cho tất cả các dòng sản phẩm nước ngọt đóng chai, nước trái cây, sữa chua uống và cà phê hòa tan.

Quyết định này nhằm ngăn chặn tình trạng gia tăng bệnh nhân tiểu đường trong nước. Việc tiêu thụ quá nhiều nước ngọt là nguyên nhân chính dẫn tới béo phì, làm tăng nguy cơ mắc các bệnh tim mạch và tiểu đường mãn tính. Thống kê cho thấy tỷ lệ béo phì tại Singapore liên tục tăng và hiện cứ 7 người trưởng thành thì có 1 người mắc bệnh tiểu đường.

Khảo sát dân ý cho thấy hơn 70% người dân Singapore ủng hộ quyết định này. Bên cạnh lệnh cấm quảng cáo, chính phủ cũng yêu cầu các nhãn hàng nước ngọt bắt buộc phải dán nhãn cảnh báo đỏ và ghi rõ hàm lượng đường ở vị trí nổi bật mặt trước bao bì sản phẩm.

5. **Giải pháp lắp đặt hệ thống dây treo ngăn ngừa chim va đập vào các tòa nhà kính**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019103003.jpg)

Các tòa nhà cao tầng sử dụng vách kính gương lớn phản chiếu mây trời thường khiến các loài chim mất phương hướng thị giác, dẫn tới hàng triệu vụ tai nạn va chạm làm chim chết hàng năm. Một nghiên cứu sinh tại Đại học Queensland (Úc) sau khi chứng kiến nhiều loài vẹt quý hiếm va vào tường kính của viện nghiên cứu đã đề xuất giải pháp bảo vệ chim tự nhiên.

Nhà trường đã cho lắp đặt một hệ thống dây treo song song chắn dọc mặt ngoài của tường kính để tạo ra các vạch kẻ sọc trực quan giúp chim nhận biết được có vật cản. Theo Hiệp hội Bảo vệ Chim Hoa Kỳ, việc sử dụng các họa tiết sọc, decal dán kính hoặc lưới mờ là giải pháp đơn giản và hiệu quả nhất giúp ngăn ngừa tai nạn va đập cho chim.

6. **Tin vắn**

- Chính quyền bang New York chính thức tuyên bố đại dịch HIV/AIDS đã không còn ở trạng thái dịch bệnh lây lan mất kiểm soát tại bang này sau khi số ca nhiễm mới năm 2018 giảm xuống mức thấp kỷ lục 248 ca, giảm 11% so với năm trước nhờ các biện pháp điều trị dự phòng PREP và ARV phát huy hiệu quả toàn diện.

- Huyện đảo Nam Cực ghi nhận sự bùng nổ của hoạt động du lịch trải nghiệm với hơn 51.000 lượt khách ghé thăm vào năm ngoái (tăng 16%), trong đó lượng du khách Mỹ đông nhất (17.000 người), tiếp theo là du khách Trung Quốc (8.200 người).

- Hãng tin lớn BBC chính thức ra mắt phiên bản trang tin chạy trên mạng ẩn danh Tor (Dark Web) qua địa chỉ tên miền onion `bbcnewsv2vjtpsuy.onion` nhằm hỗ trợ người dùng tại các quốc gia bị chặn truy cập internet vẫn có thể cập nhật tin tức an toàn.

- Tổ chức OpenJS Foundation thông báo ra mắt 2 chứng chỉ chuyên nghiệp dành cho lập trình viên phát triển ứng dụng Node.js, đánh dấu việc chuẩn hóa chứng chỉ nghề nghiệp chính thức cho cộng đồng JavaScript toàn cầu.

- Thư viện Công cộng New York triển khai dự án đăng tải toàn văn các cuốn tiểu thuyết kinh điển (như *Alice ở xứ sở thần tiên*) dưới dạng các tin ngắn trên mạng xã hội Instagram Stories để khuyến khích giới trẻ đọc sách, dự án thu hút hơn 300.000 lượt đọc sau một năm hoạt động.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100102.jpg)

- Vương quốc Anh phê duyệt siêu dự án xây dựng trang trại điện gió ngoài khơi lớn nhất thế giới tại vùng biển Bắc Hải với các cột tuabin khổng lồ có chiều cao tiệm cận tháp Eiffel (công suất đạt 12 MW mỗi cột).

## 文章 (Bài viết)

1、[Bài viết] [Hướng dẫn xây dựng hệ thống chuyển đổi giao diện Dark Mode tự động cho website](https://www.kooslooijesteijn.net/blog/add-dark-mode-to-website) (Tiếng Anh)

Chia sẻ các kỹ thuật CSS Media Queries `prefers-color-scheme` để tự động nhận biết cấu hình giao diện hệ điều hành của người dùng, kết hợp viết mã JavaScript tự động chuyển đổi bảng màu giao diện sáng/tối theo thời gian thực của môi trường.

2、[Bài viết] [Conventional Commits - Tiêu chuẩn viết nội dung Git commit thống nhất cho dự án](https://www.conventionalcommits.org/zh-hans/v1.0.0) (Tiếng Trung)

Bản dịch tài liệu chuẩn hóa cấu trúc viết thông điệp Git commit (Conventional Commits) giúp cộng đồng lập trình viên và các công cụ tự động hóa CI/CD dễ dàng theo dõi lịch sử thay đổi, tự sinh nhật ký thay đổi (Changelog) của dự án.

3、[Bài viết] [Tìm hiểu về bản chất của cấu trúc dữ liệu S-expression thay thế định dạng XML](https://news.ycombinator.com/item?id=21393705) (Tiếng Anh)

Thảo luận trên Hacker News về việc ứng dụng cấu trúc dữ liệu biểu thức S-expression (S-expression) kinh điển của ngôn ngữ Lisp làm định dạng lưu trữ và truyền tải thông tin gọn nhẹ, trực quan thay thế cho cấu trúc rườm rà của XML.

4、[Bài viết] [Quyết định dừng học nghiên cứu sinh直博 năm thứ 5 chuyên ngành Đồ họa máy tính tại Đại học Bắc Kinh](https://www.zhihu.com/question/27479057/answer/834579040) (Tiếng Trung)

Bài viết chia sẻ tâm sự đầy tính thực tế của một nghiên cứu sinh quyết định rút hồ sơ nghỉ học tiến sĩ vào năm học thứ 5 do áp lực nghiên cứu khoa học nặng nề và mất đi niềm đam mê nghiên cứu ban đầu, đi kèm 5 câu hỏi tự vấn bản thân sâu sắc trước khi đưa ra quyết định lớn của cuộc đời.

## 软件 (Phần mềm)

1、[git-quick-stats — Tiện ích dòng lệnh CLI thống kê chi tiết lịch sử đóng góp code của dự án Git](https://github.com/arzzen/git-quick-stats)

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091703.jpg)

Hỗ trợ phân tích dữ liệu Git của dự án để xuất ra các báo cáo trực quan: số lượng commit theo tác giả, tần suất sửa đổi file, biểu đồ đóng góp theo giờ trong tuần.

2、[Regexper — Công cụ trực quan hóa biểu thức chính quy (Regex) thành sơ đồ trạng thái trực quan](https://regexper.com/#%2F%5B0-9%5D%5Cs%5B0-9%5D%2F)

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091704.jpg)

Giúp lập trình viên dễ dàng hiểu và debug các chuỗi Regex phức tạp bằng cách chuyển dịch chúng thành sơ đồ luồng dữ liệu đồ họa (Railroad diagram) trực quan.

3、[Write With Transformer — Công cụ viết văn bản tiếng Anh tự động bằng mô hình AI GPT-2](https://transformer.huggingface.co/doc/gpt2-large)

Ứng dụng viết văn bản thử nghiệm của Hugging Face sử dụng mô hình học máy GPT-2 để tự động gợi ý và sinh các câu tiếp theo của văn bản tiếng Anh một cách tự nhiên khi người dùng nhấn phím Tab.

4、[folder-explorer — Tiện ích máy tính để bàn hỗ trợ quét và phân tích chi tiết dung lượng thư mục](https://github.com/d2-projects/folder-explorer)

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019092804.jpg)

Hỗ trợ quét nhanh cấu trúc thư mục ổ cứng để xuất ra thống kê dạng cây thư mục kèm thông tin dung lượng chi tiết của từng tệp tin phục vụ dọn dẹp bộ nhớ máy tính.

5、[Hệ thống đối thoại mở WeChat (WeChat OpenAI) — Nền tảng xây dựng chatbot chăm sóc khách hàng tự động](https://openai.weixin.qq.com/)

Giải pháp chatbot AI chính thức từ Tencent giúp các doanh nghiệp dễ dàng thiết lập hệ thống tự động trả lời câu hỏi thông minh tích hợp vào Fanpage WeChat, Mini Program hoặc website riêng.

## 资源 (Tài nguyên)

1、[Tài liệu] [OSSU Computer Science - Lộ trình tự học Khoa học Máy tính bài bản qua các khóa học trực tuyến](https://github.com/ossu/computer-science)

Dự án mã nguồn mở xây dựng khung chương trình đào tạo Khoa học Máy tính tự học chất lượng tương đương chương trình đại học Mỹ, tổng hợp từ các khóa học miễn phí của các trường đại học danh tiếng (MIT, Harvard) kèm theo lộ trình học cụ thể.

2、[Bản đồ] [Mini Tokyo 3D - Bản đồ 3D tương tác mô tả lịch trình di chuyển thời gian thực của tàu điện ngầm Tokyo](https://nagix.github.io/mini-tokyo-3d/)

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100803.jpg)

Ứng dụng trực quan hóa tuyệt đẹp kết nối dữ liệu Open Data của giao thông Tokyo để hiển thị vị trí chạy thực tế của hàng trăm đoàn tàu điện trên bản đồ 3D của thành phố.

## 图片 (Hình ảnh)

1. **SPHINX (Dự án Nhân sư) - Ý tưởng thiết kế máy tính gia đình tích hợp thông minh đi trước thời đại của Liên Xô năm 1986**

Dự án SPHINX là nguyên mẫu máy tính gia đình đa năng được phát triển tại Liên Xô từ năm 1986, hướng tới mục tiêu tích hợp toàn bộ hệ thống giải trí số, viễn thông, làm việc từ xa và điều khiển nhà thông minh (Smart Home) vào một hệ thống máy tính duy nhất.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090901.jpg)

Bộ vi xử lý trung tâm của máy tính được thiết kế để kết nối trực tiếp cùng 3 mô-đun lưu trữ bộ nhớ hình tam giác độc đáo.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090903.jpg)

Thiết bị đi kèm một chiếc tay cầm điều khiển từ xa có tích hợp màn hình LCD nhỏ, microphone và loa thoại giúp người dùng ra lệnh điều khiển từ xa hoặc sử dụng độc lập như một máy tính cầm tay gọn nhẹ. Dự án bị dừng phát triển hoàn toàn vào năm 1991 sau sự kiện Liên Xô tan rã.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090904.jpg)

## 文摘 (Văn trích)

1. **Lịch sử ra đời của trò chơi Rắn săn mồi (Snake) - Tựa game di động huyền thoại khai sinh trên dòng máy Nokia 6110**

Vào năm 1995, kỹ sư phần mềm Taneli Armanto làm việc tại hãng Nokia (Phần Lan) nhận được yêu cầu phát triển "một vài trò chơi nhỏ thú vị" để cài sẵn trên dòng điện thoại Nokia 6110 chuẩn bị ra mắt. Do có chút kinh nghiệm lập trình game trước đó, ông đã được giao phụ trách dự án này.

Thời kỳ đó, điện thoại di động chưa phổ cập toàn cầu, và Nokia đang nỗ lực phát triển dòng 6110 với mục tiêu thiết kế nhỏ gọn hơn, tiết kiệm pin hơn và tích hợp giao diện người dùng mới dễ dàng chuyển đổi nhanh giữa các tính năng.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091308.jpg)

Ban đầu, Taneli muốn đưa trò chơi xếp gạch Tetris lên máy. Tuy nhiên, đơn vị sở hữu bản quyền Tetris yêu cầu mức phí bản quyền quá cao trên mỗi đầu máy bán ra, buộc Nokia phải từ bỏ ý định. Taneli bắt buộc phải tự suy nghĩ thiết kế một trò chơi hoàn toàn mới của riêng mình.

Thiết kế phần cứng của Nokia 6110 lúc đó mang lại rất nhiều hạn chế cho việc lập trình game: màn hình hiển thị đơn sắc cực nhỏ, phím bấm vật lý hạn chế và dung lượng bộ nhớ lưu trữ code vô cùng ít ỏi.

Taneli nhớ lại một trò chơi đơn giản ông từng chơi trên máy tính Apple Macintosh mang tên "Snake" (Rắn), trong đó người chơi điều khiển một đường thẳng di chuyển nhặt mồi trên màn hình. Ông nhận định cơ chế này rất phù hợp với cấu trúc phím bấm và độ phân giải màn hình của điện thoại di động.

Trò chơi Rắn săn mồi chính thức trình làng cùng dòng máy Nokia 6110 vào tháng 12/1997. Với luật chơi đơn giản nhưng cực kỳ cuốn hút, game lập tức tạo nên cơn sốt toàn cầu, mở ra trào lưu chơi game trên điện thoại di động của hàng triệu người. Snake được ghi nhận là tựa game di động quan trọng đầu tiên trong lịch sử công nghệ.

2. **Bài học xương máu trị giá 1 triệu USD chi phí từ cuộc khủng hoảng nguồn cung ổ cứng toàn cầu năm 2011**

Vào năm 1981, chi phí để lưu trữ 1GB dữ liệu tiêu tốn tới hơn 1 triệu USD. Đến năm 2011, con số này giảm xuống chỉ còn chưa đầy 0.05 USD. Tuy nhiên, xu hướng giảm giá liên tục kéo dài 30 năm của ổ cứng máy tính đã bị chặn đứng hoàn toàn vào tháng 10/2011.

Trận lũ lụt lịch sử tại Thái Lan năm đó đã nhấn chìm hàng loạt khu công nghiệp sản xuất linh kiện và lắp ráp ổ cứng lớn của thế giới tại đây. Nguồn cung bị tê liệt khiến giá ổ cứng toàn cầu lập tức tăng phi mã và duy trì ở mức cao suốt gần 2 năm tiếp theo mới phục hồi về mức giá cũ.

Hãng dịch vụ lưu trữ Backblaze chia sẻ: trước khi khủng hoảng nổ ra, họ thường mua số lượng lớn dòng ổ cứng Hitachi 3TB với mức giá ổn định 130 USD/chiếc (tương đương 0.044 USD/GB).

Chỉ 2 tháng sau trận lụt, giá của đúng dòng ổ cứng này vọt lên mức 249 USD/chiếc (khoảng 0.083 USD/GB - tăng 88%), và thậm chí có tiền cũng không mua được do tình trạng khan hàng nghiêm trọng. Hãng buộc phải chuyển sang mua gom mọi dòng ổ cứng khác có trên thị trường với giá đắt đỏ để duy trì hoạt động hệ thống.

Trong suốt 2 năm khủng hoảng đó, chi phí lưu trữ thực tế của hãng bị đội lên mức trung bình 0.064 USD/GB. Dù mức tăng chênh lệch chỉ khoảng 0.02 USD cho mỗi GB, nhưng với quy mô lưu trữ mở rộng thêm tới 50PB (Petabyte) trong giai đoạn này, doanh nghiệp đã phải chi trả thêm tới hơn 1 triệu USD chi phí chênh lệch giá ổ cứng.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091805.jpg)

(Đồ thị: Biến động giá ổ cứng của hãng Backblaze trong cuộc khủng hoảng lụt Thái Lan 2011. Đường nét đứt màu đỏ mô tả xu hướng giảm giá lý thuyết nếu không có thiên tai xảy ra).

## 言论 (Danh ngôn)

1、

> "Hầu hết thời gian sử dụng thực tế, người dùng điện thoại có xu hướng muốn phóng to hình ảnh thu phóng (Zoom) để chụp chi tiết vật thể ở xa hơn là thu nhỏ góc nhìn. Do đó, mặc dù ống kính góc siêu rộng (Ultra-wide) có nhiều điểm thú vị, chúng tôi tin rằng việc trang bị ống kính tele chụp xa (Telephoto) có giá trị thực tế lớn hơn rất nhiều đối với người dùng."
> 
> -- Đại diện Google giải thích lý do dòng máy Pixel 4 chỉ trang bị ống kính tele chụp xa mà không có camera góc rộng.

(Hết)
