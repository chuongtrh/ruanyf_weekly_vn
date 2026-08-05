# 每周分享第 55 期 (Bản tin chia sẻ hàng tuần số 55)

Ghi lại những điều thú vị đáng chia sẻ tôi bắt gặp trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Chào mừng mọi người gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục [issue](https://github.com/ruanyf/weekly/issues) tại kho lưu trữ GitHub [ruanyf/weekly](https://github.com/ruanyf/weekly).

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051001.jpg)

(Ảnh bìa: Ga tàu hỏa Côn Sơn, Tô Châu, 2018)

Đã có rất nhiều bình luận và báo cáo về [chế độ làm việc 996](https://996.icu/#/zh_CN), nhưng có một điểm dường như chưa ai nhắc tới: Lập trình viên thực ra không cần thiết phải đến văn phòng.

Phát triển phần mềm chỉ cần máy tính và kết nối internet, làm việc ở đâu không quan trọng, hoàn toàn có thể làm việc tại nhà. Trên thực tế, nhiều công ty phần mềm hoạt động theo mô hình làm việc từ xa (remote work), văn phòng hầu như không có ai đến. Ví dụ, công ty GitLab có 350 nhân viên tính đến cuối năm 2018, phân bố tại 45 quốc gia và vùng lãnh thổ, tất cả đều làm việc tại nhà. Họ thậm chí còn xây dựng một trang web riêng để quảng bá [triết lý làm việc từ xa](https://about.gitlab.com/company/culture/all-remote/) của mình.

Điều tôi không hiểu về chế độ 996 là tại sao nhất thiết phải bắt mọi người ngồi ở văn phòng trong thời gian dài như vậy. Tương tác trực tiếp 8 tiếng không đủ sao? Thời gian còn lại hoàn toàn có thể về nhà để tiếp tục làm việc.

Một số nhà quản lý có triết lý rằng: Tôi phải trực tiếp giám sát thì mới đảm bảo bạn cống hiến và không lười biếng. Nhiều công ty outsource phần mềm là như vậy: chỉ được code bằng máy tính của công ty, không được mang máy về nhà, máy tính không có quyền truy cập internet bên ngoài, cũng không được cài đặt phần mềm chưa phê duyệt, nên muốn làm việc thì bắt buộc phải đến công ty.

Tôi nghĩ, việc lập trình viên nên làm không chỉ là phản đối 996, mà là thúc đẩy xu hướng làm việc từ xa. Đối với các dự án quan trọng, việc cống hiến 12 giờ một ngày, 7 ngày một tuần là khả thi, với điều kiện là được phép làm việc tại nhà.

## 新闻 (Tin tức)

1、[Tranh chấp tên miền cao cấp nhất (TLD) .amazon giữa Amazon và các quốc gia Nam Mỹ](https://www.bbc.com/news/business-47794353)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051002.jpg)

Tập đoàn Amazon nộp đơn đăng ký tên miền TLD `.amazon` nhưng vấp phải sự phản đối gay gắt từ 8 quốc gia Nam Mỹ thuộc lưu vực sông Amazon (Bolivia, Brazil, Colombia, Ecuador, Guyana, Peru, Suriname và Venezuela). Các nước này yêu cầu được đồng sở hữu tên miền `.amazon`. Tập đoàn Amazon không đồng ý, chỉ chấp nhận nhượng bộ các tên miền cấp hai theo mã quốc gia (ví dụ Brazil là `br.amazon`). Tranh chấp kéo dài và vụ việc hiện đã được chuyển giao cho ICANN phán quyết. Các tranh chấp tương tự từng xảy ra trước đây: năm 2013, hãng thời trang Patagonia đã phải rút đơn đăng ký tên miền `.patagonia` sau khi bị Argentina và Chile phản đối.

2、[Nông nghiệp năng lượng mặt trời - Kết hợp trồng trọt, chăn nuôi dưới tấm pin mặt trời nâng hiệu suất sử dụng đất lên 160%](https://cleantechnica.com/2019/04/12/fraunhofer-reports-combining-farming-with-solar-186-more-efficient-in-summer-of-2018/)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051003.jpg)

Đức đang tiến hành thử nghiệm kết hợp sản xuất điện mặt trời với nông nghiệp: lắp đặt các tấm pin mặt trời cách mặt đất 5 mét, phía dưới vẫn trồng trọt và chăn nuôi bình thường. Kết quả thực tế cho thấy mô hình này giúp tăng giá trị sản lượng của đất lên 160%. Mùa hè năm 2018 nắng nóng kỷ lục tại châu Âu gây hại cho mùa màng, nhưng nhờ các tấm pin che chắn bớt 30% bức xạ mặt trời trực tiếp nên sản lượng nông sản lại tăng lên, đồng thời nắng nóng cực độ cũng giúp tối ưu hóa sản lượng điện phát ra.

3、[Hàn Quốc nâng tỷ lệ tái chế rác thải thực phẩm lên mức kinh ngạc 95% nhờ thu phí theo cân nặng](https://www.weforum.org/agenda/2019/04/south-korea-recycling-food-waste/)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051004.jpg)

Sau nhiều năm nỗ lực, Hàn Quốc đã nâng tỷ lệ tái chế rác thải thực phẩm lên mức kỷ lục 95%. Ngay từ năm 2005, nước này đã cấm đổ rác thực phẩm trực tiếp ra các bãi chôn lấp. Đến năm 2013, Hàn Quốc triển khai bắt buộc người dân dùng túi rác sinh học chuyên dụng và mang đến các thùng rác thông minh tự động (ảnh trên). Thùng rác sẽ cân trọng lượng rác thải và trừ tiền trực tiếp của người dân: rác càng nặng, phí càng cao. Việc này thúc đẩy người dân tự vắt kiệt nước khỏi rác trước khi vứt (nước chiếm tới 80% trọng lượng rác thực phẩm). Rác thực phẩm thu gom được đưa về nhà máy xử lý để sản xuất khí sinh học (biogas), dầu sinh học và phân bón.

4、[Tác giả cuốn sách "Sapiens" Yuval Noah Harari đối thoại về tương lai AI với Tiến sĩ Lý Phi Phi](http://tech.sina.com.cn/csj/2019-04-25/doc-ihvhiewr8092203.shtml)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051005.jpg)

Tại giảng đường Đại học Stanford, nhà sử học Yuval Noah Harari và Tiến sĩ Lý Phi Phi (Giám đốc Viện AI Stanford) đã có buổi đối thoại sâu sắc về trí tuệ nhân tạo. Harari bày tỏ những lo ngại sâu sắc về sự phát triển của AI:
- Trước dữ liệu lớn (big data), những khái niệm như tự do ý chí, tư duy độc lập hay quyết định dân chủ đều có thể bị lung lay và biến thành kết quả thao túng của thuật toán.
- Trong mắt AI, tình yêu không có gì khác biệt so với một trận cúm (đều là các phản ứng hóa sinh có thể đo lường).
- AI không minh bạch, nó không chia sẻ thông tin với tôi mà liên kết với các nhà quảng cáo, tập đoàn và chính phủ để khai thác tôi.
- Cuộc đua AI toàn cầu đáng sợ hơn cuộc đua hạt nhân. Vũ khí hạt nhân được chế tạo ra không ai dám tùy tiện sử dụng, nhưng AI thì khác - hễ phát triển được tính năng nào là người ta sẽ lập tức đưa vào sử dụng ngay.

5、[Khám phá loài sinh vật mới ở Panama được đặt tên là "Sâu Donald Trump"](https://en.wikipedia.org/wiki/Dermophis_donaldtrumpi)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051006.jpg)

Một loài sâu không chân mới dài khoảng 10 cm vừa được phát hiện tại rừng rậm Panama. Chúng sống hoàn toàn dưới lòng đất, hầu như không có thị lực và mắt chỉ phân biệt được sáng tối. Chủ một công ty xây dựng đã bỏ ra 25.000 USD trong cuộc đấu giá quyền đặt tên cho loài này và đặt tên là *Dermophis donaldtrumpi*. Lý do là để mỉa mai việc Donald Trump từ chối thừa nhận biến đổi khí hậu, ví như loài sâu này chỉ nhìn thấy hai màu đen trắng và không thể nhìn xa hơn.

6、[Các nhà khoa học Trung Quốc cấy thành công gen não người vào khỉ giúp cải thiện trí nhớ](http://science.caixin.com/2019-04-15/101404121.html)

Viện Khoa học Động vật Côn Minh công bố đã chuyển gen MCPH1 của người (gen liên quan đến sự phát triển não bộ) vào bộ gen của khỉ. Đã có 11 chú khỉ Rhesus mang gen người được sinh ra. Các nhà khoa học cho biết những chú khỉ biến đổi gen này có khả năng ghi nhớ ngắn hạn "cải thiện rõ rệt" so với khỉ hoang dã.

7、[Speedgate - Môn thể thao đầu tiên trên thế giới được thiết kế hoàn toàn bởi AI](https://playspeedgate.org/)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051008.jpg)

Công ty thiết kế AKQA ra mắt môn thể thao mang tên Speedgate được thiết kế hoàn toàn bởi AI sau khi phân tích luật lệ của 400 môn thể thao truyền thống. Mỗi đội gồm 6 cầu thủ (3 tiền đạo, 3 hậu vệ). Sân đấu có 3 cổng dọc, cầu thủ phải đưa bóng qua cổng trung tâm trước khi sút vào cổng đối phương để ghi điểm.

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051009.jpg)

8、**Tin vắn**

- Elon Musk khẳng định công nghệ tự lái của Tesla đang phát triển cực nhanh, trong vòng một năm tới con người sẽ không cần can thiệp vào vô lăng vì sự can thiệp của con người lúc đó thậm chí còn kém an toàn hơn máy tính tự lái.

- Sàn giao dịch tiền mã hóa Binance bị hacker tấn công ngày 7/5, lấy đi 7.000 Bitcoin (tương đương hơn 40 triệu USD thời điểm đó). Binance cam kết sẽ đền bù toàn bộ thiệt hại cho người dùng từ quỹ bảo hiểm khẩn cấp.

- Một công ty Đức tuyên bố đã nghiên cứu thành công loại pin có mật độ năng lượng đạt 1 kWh/kg. Đây là mật độ năng lượng kỷ lục, có thể giúp xe điện chạy được quãng đường hơn 1.000 km cho một lần sạc.

- Trung tâm An ninh mạng Quốc gia Anh phân tích 23 triệu mật khẩu bị rò rỉ và công bố 5 mật khẩu phổ biến nhất thế giới: 123456, 123456789, qwerty, password và 1111111.

- Nghiên cứu mới chỉ ra sự chú ý của công chúng toàn cầu đối với các sự kiện hot ngày càng ngắn lại. Năm 2013, một chủ đề hot trên Twitter duy trì được trung bình 17.5 tiếng, đến năm 2016 con số này giảm xuống còn 11.9 tiếng (chưa đầy nửa ngày).

## 文章 (Bài viết)

1、[Bài viết] [Tại sao ngôn ngữ truy vấn dữ liệu SQL lại trường tồn và thành công như vậy?](https://blog.couchbase.com/unreasonable-effectiveness-of-sql/) (Tiếng Anh)

SQL đã ra đời hàng chục năm nhưng sức sống không hề suy giảm. Ngay cả các cơ sở dữ liệu phi quan hệ (NoSQL) cũng đang tìm cách hỗ trợ cú pháp giống SQL. Bài viết phân tích các nguyên nhân: tính khai báo (declarative), tách biệt dữ liệu với logic tính toán, và giao diện chuẩn hóa dễ học.

2、[Bài viết] [Hướng dẫn tự viết tính năng xác thực bằng JSON Web Token (JWT) trong Node.js](https://guseyn.com/posts/simple-jwt?v=1.0.85) (Tiếng Anh)

JWT là cơ chế tạo token phổ biến dùng trong xác thực và phân quyền trên web. Bài viết hướng dẫn chi tiết cách tự triển khai tạo và verify JWT trong môi trường Node.js mà không cần dùng thư viện bên ngoài.

3、[Bài viết] [Đúc kết kinh nghiệm sau khi migrate hệ thống 50.000 dòng code từ Java sang Go](https://blog.kowalczyk.info/article/19f2fe97f06a47c3b1f118fd06851fad/lessons-learned-porting-50k-loc-from-java-to-go.html) (Tiếng Anh)

Tác giả so sánh chi tiết sự khác biệt về cú pháp, quản lý bộ nhớ, hiệu năng chạy thực tế và độ phức tạp khi chuyển đổi một codebase lớn từ Java sang Golang.

4、[Bài viết] [Phân tích thiết kế ứng dụng báo thức tinh tế trên dòng điện thoại huyền thoại Nokia N9](http://nition.momentstudio.co.nz/2014/08/the-nokia-n9-alarm-clock/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051010.jpg)

Nokia N9 chạy MeeGo tuy ngắn ngủi nhưng sở hữu giao diện đồng hồ báo thức cực kỳ thông minh. Bài viết phân tích trải nghiệm xoay vòng chọn giờ trực quan và các chi tiết micro-interaction xuất sắc của nó.

5、[Bài viết] [Tìm hiểu lịch sử phát triển của các thiết bị lưu trữ dữ liệu máy tính](https://royal.pingdom.com/the-history-of-computer-data-storage-in-pictures/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051012.jpg)

Hình ảnh minh họa lịch sử phát triển bộ nhớ từ băng đục lỗ, băng từ, đĩa mềm đến ổ cứng hiện đại. (Ảnh trên: Ổ cứng IBM 3380 dung lượng 2.52 GB ra mắt năm 1980, nặng 250 kg và có giá từ 80.000 đến 140.000 USD).

6、[Bài viết] [Google công bố Flutter hỗ trợ nền tảng Web - Bước tiến thành bộ công cụ phát triển đa nền tảng](https://developers.googleblog.com/2019/05/Flutter-io19.html) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051013.jpg)

Tại Google I/O 2019, Google chính thức giới thiệu Flutter cho Web, đưa Flutter thành framework hỗ trợ mọi nền tảng từ di động, web, desktop đến các thiết bị nhúng thông minh.

## 软件 (Phần mềm)

1、[fyne — Thư viện lập trình giao diện người dùng (GUI) đa nền tảng bằng ngôn ngữ Go](https://github.com/fyne-io/fyne)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051014.jpg)

Giúp viết ứng dụng desktop và di động có giao diện đồ họa đẹp mắt bằng Golang, render trực tiếp bằng driver đồ họa phần cứng (OpenGL) để đảm bảo hiệu năng mượt mà.

2、[Kroki — Dịch vụ render biểu đồ mã nguồn mở hỗ trợ PlantUML, Mermaid, GraphViz](https://kroki.io/)

Cung cấp API chuyển đổi mã nguồn text thành hình ảnh biểu đồ tương ứng một cách nhanh chóng, hỗ trợ hàng chục định dạng biểu đồ thiết kế phổ biến.

3、[md2pdf — Công cụ chuyển đổi Markdown thành file PDF trực tiếp trên trình duyệt](https://github.com/realdennis/md2pdf)

Chạy offline trên browser giúp render file Markdown thành tài liệu PDF đẹp mắt, hỗ trợ tùy chỉnh CSS layout cho trang in.

4、[asciiflow — Công cụ vẽ sơ đồ bằng ký tự ASCII trực quan ngay trên web](http://asciiflow.com/)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051016.jpg)

Giúp vẽ các sơ đồ khối, đường nối bằng các ký tự text để chèn trực tiếp vào comment source code hoặc file README một cách dễ dàng qua giao diện vẽ chuột.

5、[avataaars generator — Công cụ tạo ảnh đại diện avatar hoạt hình phong cách vector](https://getavataaars.com/)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051017.jpg)

Trang web miễn phí cho phép tùy biến kiểu tóc, quần áo, phụ kiện, biểu cảm khuôn mặt để xuất ra các ảnh đại diện đẹp định dạng SVG/PNG.

6、[Windows Terminal — Trình quản lý dòng lệnh console thế hệ mới của Microsoft](https://github.com/microsoft/Terminal)

Hỗ trợ tab, chia màn hình, bộ ký tự Unicode (emoji), tăng tốc render đồ họa bằng GPU và cho phép tùy biến theme linh hoạt cho PowerShell, CMD và WSL.

## 资源 (Tài nguyên)

1、[Tài liệu] [Tự viết giải mã ảnh JPEG bằng ngôn ngữ Rust](https://github.com/MROS/jpeg_tutorial)

Kho tài liệu hướng dẫn chi tiết lý thuyết nén ảnh JPEG và hướng dẫn từng bước viết trình giải mã ảnh (decoder) bằng Rust.

2、[Sách] [Mạng thần kinh nhân tạo và Học sâu - Giáo trình của Đại học Phúc Đán](https://github.com/nndl/nndl.github.io)

Giáo trình giảng dạy của PGS. Khâu Tích Bằng giới thiệu nền tảng toán học và các mô hình deep learning phổ biến trong Computer Vision và NLP.

## 文摘 (Văn trích)

1. **Hiện tượng "Tỷ lệ không kết hôn trọn đời" tăng mạnh**

Trích cuốn sách phóng sự xã hội *Không có sự gắn kết* (Mạng lưới xã hội vô duyên Nhật Bản):

Xã hội học định nghĩa tỷ lệ những người đến tuổi 50 vẫn chưa từng kết hôn lần nào là "Tỷ lệ không kết hôn trọn đời". Tại Nhật Bản, tỷ lệ này ở nam giới năm 2005 là 16%, dự kiến năm 2030 sẽ tăng lên 33% (cứ 3 người đàn ông thì có 1 người sống độc thân cả đời). Với nữ giới, dự báo năm 2030 là 23%, tăng hơn gấp đôi so với năm 2005.

Các chuyên gia phân tích nguyên nhân của xu hướng này:
- Một là, hạ tầng đô thị phục vụ đời sống độc thân ngày càng hoàn thiện (như sự phổ cập của cửa hàng tiện lợi 24/7), giúp việc sống một mình không còn nhiều bất tiện.
- Hai là, các công việc ổn định trọn đời ngày càng ít đi, thay vào đó là lao động hợp đồng ngắn hạn có thu nhập bấp bênh. Khi đối mặt với chi phí nhà ở và giáo dục con cái đắt đỏ, người có thu nhập không ổn định sẽ chọn cách không kết hôn.
- Ba là, định kiến xã hội về việc bắt buộc phải lập gia đình khi đến tuổi đang dần mờ nhạt.
- Bốn là, phụ nữ độc lập hơn về tài chính nên không còn áp lực phải phụ thuộc vào hôn nhân.

2. **Hội chứng tích lũy các dự án cá nhân (side projects) dở dang của lập trình viên**

Là lập trình viên, tôi có hơn 100 dự án cá nhân chưa từng được phát hành:
- Kịch bản thường thấy: Tôi hào hứng với một ý tưởng mới, nghĩ rằng có thể hoàn thành trong một cuối tuần. Tôi làm việc điên cuồng, code cơ bản đã chạy được và chứng minh được concept hoạt động đúng.
- Nhưng dự án đã sẵn sàng launch chưa? Thường là chưa. Phần thú vị nhất (code tính năng cốt lõi) đã xong, nhưng phần còn lại rất nhàm chán: thiết kế giao diện thô sơ, thiếu trang giới thiệu landing page cho người dùng mới. Tôi lại là người viết lách tệ và ngại bị người khác đánh giá sản phẩm.
- Khâu khó khăn nhất là tiếp thị (marketing). Không gì tệ hơn việc một lập trình viên hướng nội phải tự đi quảng bá sản phẩm của mình. Tôi sợ bị chê cười, sợ phát hiện ra ai đó đã làm sản phẩm tốt hơn, hoặc tệ nhất là sự im lặng thờ ơ của internet.
- Những khâu dở dang này chỉ chiếm 20% khối lượng công việc, nhưng 20% cuối cùng này lại đòi hỏi nỗ lực tinh thần lớn hơn cả 80% thời gian code trước đó. Kết quả là dự án bị bỏ xó để nhường chỗ cho một ý tưởng mới lấp lánh hơn vừa xuất hiện. Chu kỳ này cứ thế lặp đi lặp lại vô tận.

## 图片 (Hình ảnh)

1. **Ký tự mưa mã màu xanh huyền thoại trong phim The Matrix thực chất là công thức làm sushi**

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019051022.jpg)

Dòng ký tự đổ xuống ở đầu phim *Ma Trận* đã trở thành biểu tượng của văn hóa hacker. Nhà thiết kế Simon Whiteley tiết lộ nguồn gốc: khi nhận nhiệm vụ thiết kế hiệu ứng này, ông đã mượn cuốn sách dạy nấu món ăn Nhật của người vợ Nhật Bản, quét các ký tự tiếng Nhật (chữ Hiragana, Katakana và Hán tự) trong trang sách in dọc để tạo nên dòng ký tự chảy từ trên xuống.

## 言论 (Danh ngôn)

1、

> "Áp lực công việc của tôi rất lớn, và cách duy nhất tôi biết để đối phó là làm việc chăm chỉ hơn nữa. Đó là lối thoát duy nhất giúp tôi giải tỏa áp lực."
>
> -- Alan Turing. (Ông hoàn thành cự ly Marathon với thành tích ấn tượng 2 giờ 46 phút 3 giây. Khi được hỏi lý do tập chạy bền khắc nghiệt, ông đã trả lời như trên).

2、

> "Đối với các sản phẩm thử nghiệm hoặc phiên bản đầu tiên (v1), bạn hầu như không cần đến các Web framework thời thượng. Điều bạn cần nhất là tốc độ đưa sản phẩm ra thị trường nhanh nhất để kiểm chứng ý tưởng."
>
> -- [*Bạn có thể không cần Web framework thời thượng*](https://char.gd/blog/2019/you-dont-need-that-hipster-web-framework)

(Hết)
