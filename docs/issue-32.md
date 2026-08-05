# 每周分享第 32 期 (Bản tin chia sẻ hàng tuần số 32)

Ghi lại những điều thú vị đáng chia sẻ tôi bắt gặp trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Chào mừng mọi người gửi bài đóng góp thông qua mục [issue](https://github.com/ruanyf/weekly/issues) tại kho lưu trữ GitHub [ruanyf/weekly](https://github.com/ruanyf/weekly).

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112301.jpg)

(Ảnh bìa: Lục Gia Chủy, Thượng Hải, 2018)

Gần đây, tôi có đọc được một [câu chuyện ngụ ngôn nhỏ](http://www.bbc.com/future/story/20160307-why-does-walking-through-doorways-make-us-forget) rất ý nghĩa muốn chia sẻ cùng mọi người.

> Có ba người thợ xây đang cùng xây một bức tường gạch.
> 
> Một người qua đường tiến lại hỏi người thợ thứ nhất: "Anh đang làm gì thế?" Người thợ trả lời: "Tôi đang xếp những viên gạch."
> 
> Người đó quay sang hỏi người thợ thứ hai: "Còn anh đang làm gì?" Người thợ thứ hai đáp: "Tôi đang xây dựng một bức tường."
> 
> Cuối cùng, người đó hỏi người thợ thứ ba: "Anh đang làm gì?" Người thợ thứ ba hào hứng trả lời: "Tôi đang xây dựng một thánh đường lớn!"

Dù cả ba người thợ đều đang thực hiện cùng một công việc vật lý giống nhau, nhưng tầm nhìn và góc độ tiếp cận công việc của họ lại hoàn toàn khác biệt.

Các lập trình viên cũng rất cần rèn luyện năng lực tư duy đa chiều này. Khi thiết kế sản phẩm, bạn cần có **tầm nhìn vĩ mô (macro-thinking)**: tự hỏi tại sao cần phát triển phần mềm này, nó giải quyết bài toán gì và đóng vai trò gì trong hệ sinh thái chung. Khi lựa chọn giải pháp kỹ thuật, bạn cần có **tầm nhìn trung mô (meso-thinking)**: nhìn nhận phần mềm như một tập hợp các module liên kết chặt chẽ và xác định rõ chức năng cốt lõi của từng module. Khi trực tiếp viết code, bạn cần có **tầm nhìn vi mô (micro-thinking)**: tối ưu hóa từng vòng lặp, thiết kế các hàm sạch và xây dựng các bộ test case kiểm thử chất lượng.

Việc có thể linh hoạt chuyển đổi góc nhìn ở các độ cao khác nhau sẽ giúp chúng ta hiểu sâu sắc bản chất công việc mình đang làm. Giống như bản tin tuần này: bề nổi là việc tổng hợp các liên kết hữu ích, nhưng chiều sâu là xây dựng một cộng đồng học thuật kết nối, và xa hơn là sự chuẩn bị năng lực để đón đầu thế giới tương lai.

## 新闻 (Tin tức)

1、[Trung Quốc nuôi cấy thành công chuột con từ hai chuột mẹ đồng tính](https://www.theguardian.com/science/2018/oct/11/mice-same-sex-parents-born-same-sex-reproduction-humans)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112302.jpg)

Đội ngũ nghiên cứu thuộc Viện Khoa học Trung Quốc đã tạo nên bước đột phá y sinh khi nuôi cấy thành công thế hệ chuột con khỏe mạnh phát triển hoàn toàn từ vật liệu di truyền của hai chuột mẹ mà không cần đến tế bào tinh trùng của bố.

Nghiên cứu giải mã cơ chế in vết di truyền (genomic imprinting) ở động vật có vú: có khoảng 100 gene đặc biệt chỉ được kích hoạt nếu nhận từ DNA của bố hoặc mẹ. Các nhà khoa học đã sử dụng công cụ chỉnh sửa gene CRISPR để xóa bỏ các dấu vết in di truyền trên tế bào gốc đơn bội của chuột mẹ thứ nhất, biến đổi cấu trúc của nó tương tự như tế bào di truyền của chuột bố, sau đó tiêm vào trứng của chuột mẹ thứ hai để tạo thành phôi thai phát triển bình thường.

2. **Hội nghị đo lường quốc tế chính thức thay đổi định nghĩa đơn vị Kilogram bằng hằng số Planck**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112303.jpg)

Tại Văn phòng Cân đo Quốc tế đặt ở Paris, trọng lượng tiêu chuẩn 1 kg từ trước đến nay được định nghĩa dựa trên một khối kim loại hình trụ làm bằng hợp kim platinum-iridium nguyên bản gọi là "Le Grand K". Toàn bộ các hệ thống đo lường khối lượng trên thế giới đều phải so chuẩn định kỳ với khối kim loại này. Tuy nhiên, việc phụ thuộc vào một vật thể vật lý duy nhất tiềm ẩn rủi ro hư hại và thay đổi khối lượng vi mô theo thời gian.

Ngày 16/11, Ủy ban Cân đo Quốc tế đã chính thức bỏ phiếu thông qua quyết định lịch sử: loại bỏ khối kim loại nguyên bản này và thay thế định nghĩa 1 kg dựa trên hằng số vật lý Planck bất biến trong tự nhiên.

3、[Raspberry Pi ra mắt phiên bản nhỏ gọn giá rẻ Raspberry Pi 3 Model A+](https://techcrunch.com/2018/11/15/raspberry-pi-3-model-a-is-a-compact-yet-powerful-raspberry-pi/)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112304.jpg)

Hội tổ chức Raspberry Pi chính thức trình làng phiên bản rút gọn Model A+ của dòng mạch Pi 3. Thiết bị có giá bán 25 USD (rẻ hơn 10 USD so với bản B+), được cắt giảm bộ nhớ RAM xuống còn 512MB, chỉ trang bị 1 cổng USB 2.0 và loại bỏ cổng cắm mạng dây Ethernet, rất phù hợp cho các dự án nhúng IoT nhỏ gọn không đòi hỏi xử lý dữ liệu lớn.

4、[Tàu thăm dò địa chất InSight của NASA chuẩn bị đổ bộ xuống bề mặt Sao Hỏa](https://mars.nasa.gov/insight/)

Tàu vũ trụ thăm dò địa chất InSight của cơ quan NASA (phóng đi từ tháng 5) dự kiến sẽ đáp xuống bề mặt Sao Hỏa vào ngày 26/11. Không giống như các robot tự hành như Curiosity, InSight là trạm nghiên cứu tĩnh cố định. Nhiệm vụ chính của trạm là sử dụng các đầu dò địa chấn siêu nhạy cắm sâu xuống lòng đất để đo đạc các rung chấn địa chất (marsquakes), từ đó dựng mô hình cấu trúc các tầng đất đá sâu dưới lòng Sao Hỏa hỗ trợ nghiên cứu quá trình hình thành các hành tinh đá cách đây 4.6 tỷ năm.

5、[Nghiên cứu công nghệ tổng hợp bột protein dinh dưỡng trực tiếp từ khí CO2](http://www.solarfoods.fi/)

Một startup công nghệ tại Phần Lan giới thiệu quy trình sản xuất thực phẩm độc đáo: sử dụng dòng điện phân tách nước thành hydro, sau đó nuôi cấy các chủng vi sinh vật đặc biệt hấp thụ hydro, khí CO2 và nitơ trong không khí để sản xuất ra bột protein dinh dưỡng chất lượng cao. Công nghệ hứa hẹn giúp cơ quan vũ trụ giải quyết bài toán tự sản xuất lương thực cho các phi hành gia trên Sao Hỏa — nơi có bầu khí quyển ngập tràn khí CO2.

6、[Trường đại học Anh thử nghiệm công nghệ giảng dạy từ xa bằng hình ảnh hologram 3D](https://www.bbc.com/news/technology-46060381)

Trường Đại học Imperial College London đã đưa vào chạy thử nghiệm hệ thống máy chiếu hình ảnh toàn ảnh (hologram) tái tạo hình ảnh 3D kích thước thực tế của các giáo sư ở xa đứng giảng bài ngay trên sân khấu giảng đường, mang lại trải nghiệm tương tác trực quan sinh động hơn nhiều so với các phần mềm gọi video 2D thông thường.

7、[Các nước châu Âu thử nghiệm hệ thống kiểm tra nói dối bằng AI tại cửa khẩu biên giới](https://gizmodo.com/an-ai-lie-detector-is-going-to-start-questioning-travel-1830126881)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112308.jpg)

Dự án iBorderCtrl ứng dụng AI bắt đầu được thử nghiệm tại các cửa khẩu của Hungary, Latvia và Hy Lạp. Hệ thống sẽ tự động đưa ra các câu hỏi phỏng vấn du khách ngoài khối EU, camera thông minh phân tích hàng chục chuyển động vi mô trên cơ mặt (micro-expressions) để chấm điểm mức độ trung thực của câu trả lời trước khi chuyển các trường hợp nghi vấn cho nhân viên hải quan xử lý trực tiếp.

8、[Khảo sát tiềm năng kinh tế khổng lồ từ khai thác khoáng sản trên các tiểu hành tinh](https://physicsworld.com/a/the-asteroid-trillionaires/)

Mặc dù NASA đã tạm hoãn ngân sách cho dự án bắt giữ tiểu hành tinh đưa về quỹ đạo Trái Đất, giới khoa học tính toán việc khai thác mỏ vũ trụ có tiềm năng kinh tế cực lớn. Chi phí để tiếp cận và khai thác một tiểu hành tinh cỡ nhỏ ước tính khoảng 2.6 tỷ USD, nhưng lượng kim loại quý nhóm bạch kim thu hoạch được trên đó có giá trị quy đổi lên tới hơn 50 tỷ USD.

9. **Chất lượng không khí tại San Francisco suy giảm nghiêm trọng do cháy rừng**

Do ảnh hưởng từ các vụ cháy rừng lớn kéo dài tại bang California, khói bụi đã bao phủ toàn bộ vùng vịnh. Chỉ số bụi mịn PM2.5 tại thành phố San Francisco đã đo được ở mức kỷ lục 271 AQI — ngưỡng cực kỳ nguy hại cho sức khỏe con người.

## 教程 (Hướng dẫn)

1、[Bài viết] [Tìm hiểu các thuật toán kiểm soát tắc nghẽn đường truyền của giao thức TCP](http://squidarth.com/rc/programming/networking/2018/07/18/intro-congestion.html) (Tiếng Anh)

Giải thích cơ chế hoạt động của cửa sổ kiểm soát tắc nghẽn (Congestion Window) trong giao thức TCP: cách hệ thống tự động tăng giảm số lượng gói tin gửi đi đồng thời dựa trên phản hồi gói tin hao hụt để tối ưu hóa băng thông mà không làm nghẽn đường truyền mạng.

2、[Bài viết] [Hướng dẫn tự xây dựng frontend web framework chạy bằng WebAssembly và Go](https://tutorialedge.net/golang/writing-frontend-web-framework-webassembly-go/) (Tiếng Anh)

Từng bước hướng dẫn cách thiết kế component giao diện và viết logic định tuyến routing trực tiếp bằng ngôn ngữ Go, sau đó biên dịch ra WASM để chạy mượt mà trên trình duyệt, mở ra hướng đi mới không cần dùng đến JavaScript.

3、[Bài viết] [Hướng dẫn sử dụng thư viện Pandas xử lý và phân tích dữ liệu CSV bằng Python](https://jalammar.github.io/gentle-visual-intro-to-data-analysis-python-pandas/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112311.jpg)

Bài viết trực quan sinh động bằng hình vẽ hướng dẫn các thao tác lọc dữ liệu, tính toán thống kê và chuyển đổi định dạng cột điểm dữ liệu bằng thư viện Pandas.

4、[Bài viết] [Hướng dẫn thiết lập môi trường lập trình JavaScript chuyên nghiệp trên Neovim](https://hackernoon.com/using-neovim-for-javascript-development-4f07c289d862) (Tiếng Anh)

Chia sẻ cách cài đặt các plugin quản lý package, tự động gợi ý code (autocompletion) và kiểm tra cú pháp (linter) để biến Neovim thành một IDE lập trình JS mạnh mẽ và siêu nhẹ.

## 资源 (Tài nguyên)

1、[Lịch sử] [Old Internet Files — Lưu trữ tệp tin hosts.txt thời kỳ sơ khai của Internet](https://rscott.org/OldInternetFiles/)

Vào thời kỳ đầu trước khi hệ thống phân giải tên miền DNS ra đời, toàn bộ địa chỉ IP và tên miền của mạng internet sơ khai được quản lý tập trung trong một file text duy nhất có tên `hosts.txt`. Trang web lưu trữ các phiên bản file này qua các mốc lịch sử để tham khảo.

2、[Sách] [C/C++ hướng sang WebAssembly — Sách hướng dẫn thực hành biên dịch Emscripten](https://github.com/3dgen/cppwasm-book)

Cuốn sách điện tử nguồn mở hướng dẫn chi tiết cách biên dịch các dự án C/C++ thành các module WASM chạy hiệu năng cao trên trình duyệt web.

## 工具 (Công cụ)

1、[ml5.js — Thư viện học máy thân thiện dành cho trình duyệt web](https://ml5js.org/)

Một thư viện đóng gói gọn gàng viết trên nền tảng TensorFlow.js, cung cấp các API cực kỳ đơn giản cho lập trình viên web để tích hợp tính năng nhận diện vật thể qua camera, phát hiện dáng người hoặc phân tích cảm xúc văn bản bằng JavaScript.

2、[I Ching Codes — Bộ mã hóa và giải mã dữ liệu QR dựa trên quẻ dịch Kinh Dịch](https://iching.codes/)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112317.jpg)

Một dự án sáng tạo nguồn mở sử dụng hệ thống biểu tượng sáu mươi tư quẻ dịch của Kinh Dịch Trung Hoa cổ đại làm cấu trúc mã hóa thông tin thay thế cho các chấm vuông của mã QR truyền thống.

## 文摘 (Văn trích)

1. **Thực trạng cuộc sống và công việc của các blogger du lịch trên Instagram**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112318.jpg)

Bài viết phân tích mô hình kinh doanh của các influencer du lịch trên Instagram (như Lisa Linh với gần 100.000 người theo dõi). Họ có thể đi du lịch vòng quanh thế giới miễn phí bằng cách gửi đề xuất hợp tác trực tiếp đến các resort cao cấp, đổi lại việc đăng tải các bức ảnh check-in quảng bá thương hiệu cho khách sạn trên trang cá nhân. Tuy nhiên, các resort hiện nay đang siết chặt quy trình duyệt hồ sơ để lọc bỏ các tài khoản mua follower ảo, đồng thời yêu cầu các influencer cung cấp thêm các giá trị gia tăng thực tế như bàn giao bản quyền hình ảnh chất lượng cao hoặc đào tạo kỹ năng marketing mạng xã hội cho nhân viên khách sạn.

2. **Lịch sử tìm ra hoạt chất Morphine và sự ra đời của Heroin**

Cuối thế kỷ 18, nhà hóa học Đức Friedrich Sertürner đã thành công trong việc phân tách tinh thể tinh khiết có tác dụng鎮痛镇痛鎮痛鎮痛 cốt lõi từ cây thuốc phiện thô và đặt tên là Morphine (đặt theo tên thần giấc mơ Morpheus trong thần thoại Hy Lạp).

Đến cuối thế kỷ 19, các nhà hóa học tại hãng dược phẩm Bayer (Đức) đã tiến hành acetyl hóa morphine để tạo ra chất diacetylmorphine nhằm giúp hoạt chất dễ dàng vượt qua hàng rào máu não nhanh hơn. Hoạt chất mới này mang lại cảm giác hưng phấn cực mạnh nên được đặt tên thương mại là **Heroin** (nghĩa là anh hùng) và ban đầu được quảng cáo bán rộng rãi như một loại thuốc giảm ho, giảm đau an toàn cho cả trẻ em. Chỉ 4 năm sau khi tung ra thị trường, trước tình trạng nghiện ngập tàn phá xã hội nghiêm trọng do độc tính gây nghiện của heroin cao hơn morphine gấp nhiều lần, các quốc gia mới bắt đầu ban hành lệnh cấm sản xuất và lưu hành chất này.

## 本周图片 (Hình ảnh tuần này)

1. **Hiện tượng cát sa mạc nuốt chửng các tuyến đường cao tốc tại Dubai**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112321.jpg)

Hình ảnh chụp từ trên cao cho thấy sức mạnh của những cơn gió cát sa mạc tại UAE đang liên tục bồi đắp cát tràn ngập đè lên các tuyến đường nhựa hiện đại, tạo nên cảnh tượng thiên nhiên lấn át công trình nhân tạo vô cùng ấn tượng.

2. **Elliðaey — Ngôi nhà biệt lập cô độc nhất hành tinh tại Iceland**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112325.jpg)

Ngôi nhà gỗ nhỏ nằm đơn độc giữa thảm cỏ xanh mướt của hòn đảo dốc Elliðaey ngoài khơi Iceland. Hòn đảo này từng là nơi sinh sống của 5 gia đình chăn nuôi gia súc trước khi họ chuyển vào đất liền sinh sống từ những năm 1930. Ngôi nhà hiện tại được hiệp hội săn bắn địa phương xây dựng từ năm 1953 làm nơi lưu trú tạm thời cho các thành viên ra đảo săn chim biển vào mùa săn bắn.

## 新奇 (Sự độc đáo)

1. **Ý tưởng tự chế bếp cảm ứng từ chiên trứng bằng nam tơ-bin quay**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112327.jpg)

Một sáng chế DIY độc đáo ứng dụng định luật cảm ứng điện từ Faraday: tác giả gắn 10 khối nam châm vĩnh cửu cực mạnh lên một đĩa xoay và kết nối với động cơ máy chạy bộ cũ để xoay tròn đĩa nam châm với tốc độ cao dưới đáy chảo dẫn điện. Sự thay đổi liên tục của từ trường xuyên qua đáy chảo sinh ra dòng điện xoáy Foucault tự nung nóng đáy chảo làm chín trứng nhanh chóng mà không cần cắm điện trực tiếp vào chảo.

## 本周金句 (Kim ngôn tuần này)

1、

> "Cùng một phần mềm ứng dụng, nếu được thiết kế giao diện bằng thư viện native QT sẽ có mức tiêu thụ bộ nhớ RAM và tài nguyên CPU thấp hơn từ 4 đến 8 lần so với việc dựng giao diện bằng công nghệ HTML5 (Electron). Việc lạm dụng HTML5 cho các ứng dụng desktop đang vô tình ép máy tính của người dùng phải tính toán nhiều hơn, đốt cháy nhiều điện năng hơn và gián tiếp ép họ phải nâng cấp phần cứng liên tục, tạo ra lượng rác thải điện tử khổng lồ cho hành tinh."
> 
> -- Trích cẩm nang "Sinh thái học cho lập trình viên".

2. **Kinh nghiệm viết tiểu thuyết của Stephen King gợi ý cho việc refactor mã nguồn**

> "Bí quyết viết tiểu thuyết của tôi là không ngừng chỉnh sửa cắt gọt bản nháp. Quy tắc bắt buộc là bản thảo sau khi chỉnh sửa lần thứ hai phải ngắn hơn bản thảo đầu tiên ít nhất 10% nhờ loại bỏ toàn bộ các câu chữ thừa thãi rườm rà."
> 
> -- Stephen King

(Hết)
