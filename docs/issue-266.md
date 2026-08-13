# Bản tin chia sẻ công nghệ (Số 266): Tự tạo sách điện tử EPUB song ngữ

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3324) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081010.webp)

Tại thành phố Đức Dương, tỉnh Tứ Xuyên, người ta đã sử dụng các tấm thép không gỉ để dựng nên một công viên cảnh quan độc đáo mang tên “Vườn Bánh Răng”. Mỗi khu vực tiểu cảnh được tạo hình theo khối lục giác đều tượng trưng cho một chiếc bánh răng cơ khí, ẩn dụ cho quá trình chuyển đổi xanh của thành phố công nghiệp lâu đời này. (Nguồn: [Lingganlb](https://lingganlb.com/index/index/detail.html?code=A7883509524180829270))

## 自己做双语 EPUB 电子书

Trong chuyên mục "Công cụ" hàng tuần của bản tin, tôi thường xuyên giới thiệu các phần mềm hữu ích và có nhiều công cụ đã hỗ trợ đắc lực cho công việc hàng ngày của tôi.

Trong số đó, công cụ tiện ích mở rộng “[Immersive Translate](https://immersivetranslate.com/)” (Dịch thuật đắm chìm) do một lập trình viên tự ứng cử giới thiệu trong [Bản tin số 254](https://www.ruanyifeng.com/blog/2023/05/weekly-issue-254.html) là một công cụ đặc biệt hữu ích.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080602.webp)

Đây là một tiện ích mở rộng trình duyệt chuyên dụng phục vụ dịch thuật trang web trực tiếp, hỗ trợ người dùng tùy chỉnh lựa chọn nhiều dịch vụ dịch thuật API khác nhau.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080603.webp)

Tuy nhiên, tính năng mà tôi yêu thích và sử dụng nhiều nhất trên công cụ này lại là tính năng hỗ trợ tự sản xuất sách điện tử song ngữ định dạng EPUB. Hôm nay tôi xin giới thiệu chi tiết cách thức ứng dụng tính năng này.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080604.webp)

Rất nhiều cuốn sách và tài liệu công nghệ nước ngoài chất lượng cao mà tôi muốn nghiên cứu hiện chưa được dịch và xuất bản tại thị trường trong nước. Nếu cố gắng đọc trực tiếp phiên bản tiếng Anh gốc, tốc độ đọc hiểu sẽ rất chậm và dễ gây mệt mỏi. Trong tình huống này, giải pháp tối ưu là **tự tay biên dịch một phiên bản song ngữ đối chiếu bằng máy**. Chúng ta sẽ ưu tiên đọc lướt phần nội dung đã dịch bằng tiếng Việt ở phía dưới, và khi gặp những câu chữ chưa rõ nghĩa, ta có thể đối chiếu trực tiếp với câu tiếng Anh gốc ngay phía trên.

Ví dụ vừa qua, cuốn tự truyện của lập trình viên huyền thoại John Romero mang tên *DOOM Guy* đã được xuất bản tại thị trường Mỹ:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080910.webp)

John Romero được biết đến là một trong những bộ óc vĩ đại sáng tạo nên dòng trò chơi bắn súng kinh điển *DOOM* (毁灭战士). Kể từ sau khi đọc cuốn sách *Cuộc đời lập trình của Carmack*, tôi vô cùng tò mò muốn tìm hiểu sâu hơn về cuộc đời của Romero.

Do cuốn sách chưa được dịch sang tiếng Trung, tôi đã sử dụng tiện ích Immersive Translate để tự tạo cho mình một bản sách điện tử song ngữ đối chiếu định dạng EPUB để đọc trên máy đọc sách.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080605.webp)

Quy trình thực hiện vô cùng đơn giản: bạn chỉ cần tải tệp tin EPUB gốc của cuốn sách lên giao diện công cụ, bấm kích hoạt dịch trang và lựa chọn xuất ra tệp tin EPUB mới. Toàn bộ quá trình chỉ diễn ra trong vòng vài phút.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080606.webp)

So với các giải pháp phần mềm dịch thuật sách điện tử khác trên thị trường, công cụ này sở hữu giao diện trực quan, thao tác đơn giản hơn hẳn và hoàn toàn miễn phí sử dụng.

Tôi đã áp dụng phương pháp này để đọc liên tục vài cuốn sách ngoại văn nguyên bản và nhận thấy hiệu quả mang lại rất tốt, đáp ứng hoàn hảo nhu cầu tự học tập.

Lưu ý nhỏ là công cụ này yêu cầu tệp tin đầu vào bắt buộc phải ở định dạng EPUB tiêu chuẩn. Nếu tài liệu nghiên cứu của bạn đang ở các định dạng khác, bạn có thể sử dụng phần mềm quản lý sách miễn phí [Calibre](https://calibre-ebook.com/) để thực hiện chuyển đổi định dạng trước:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080607.webp)

Các tệp tài liệu định dạng HTML, TXT hay Markdown đều có thể dễ dàng nhập vào Calibre thông qua nút "Add books" ở góc trên bên trái, sau đó nhấn nút "Convert books" để xuất ra định dạng EPUB chuẩn chỉnh.

Calibre hỗ trợ nhập từng tệp tin riêng lẻ. Trong trường hợp bạn có một thư mục chứa nhiều tệp tin HTML độc lập muốn gộp lại thành một cuốn sách điện tử theo thứ tự chương hồi nhất định, bạn cần thiết lập thêm một tệp tin mục lục index theo hướng dẫn chi tiết tại trang [Tài liệu hướng dẫn Calibre](https://manual.calibre-ebook.com/faq.html#how-do-i-convert-a-collection-of-html-files-in-a-specific-order).

Trên đây là phương pháp tự học và đọc tài liệu ngoại văn hàng ngày của tôi, xin được chia sẻ để bạn đọc cùng tham khảo ứng dụng.

## 科技动态

1、[Mỹ thử nghiệm thay thế người dẫn chương trình radio bằng trí tuệ nhân tạo](https://techcrunch.com/2023/06/14/radio-station-gets-part-time-ai-dj-based-on-its-midday-host/)

Một đài phát thanh tại bang Oregon, Mỹ vừa qua đã công bố thử nghiệm chương trình phát thanh hàng ngày từ 10 giờ sáng đến 3 giờ chiều của MC Ashley sẽ do hệ thống AI đảm nhận hoàn toàn:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062405.webp)

Hệ thống AI sẽ tự động thu thập các tin tức nóng hổi trong ngày để tự động soạn thảo kịch bản phát sóng, sau đó sử dụng công nghệ mô phỏng giọng nói sinh trắc học để phát ra giọng đọc của MC Ashley đi kèm nhạc đệm. Giải pháp này giúp đài tiết kiệm tối đa chi phí vận hành so với việc MC Ashley phải trực tiếp ngồi trong phòng thu. MC Ashley từ nay sẽ chuyển sang đảm nhận các công việc biên tập nội dung ở hậu trường.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062406.webp)

Nhiều đài phát thanh địa phương quy mô nhỏ tại Mỹ cho biết đang cân nhắc học tập mô hình này. Trong tương lai, lượng thông tin truyền thông mà con người tiếp cận hàng ngày có thể tăng lên gấp hàng chục lần nhưng phần lớn trong số đó sẽ được biên tập sản xuất bởi AI.

2、[Sự thật hài hước đằng sau miếng dán cấm cổng kết nối USB trên máy in HP](https://www.theverge.com/2023/8/4/23820710/pay-no-attention-to-the-usb-port-behind-the-no-usb-sticker)

Một người dùng mạng xã hội đã chia sẻ hình ảnh dở khóc dở cười khi chọn mua một dòng máy in văn phòng phân khúc giá rẻ của hãng HP:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080501.webp)

Trên vỏ hộp và tờ hướng dẫn đi kèm, hãng in dòng chữ cảnh báo lớn khẳng định thiết bị này chỉ hỗ trợ kết nối in ấn qua WiFi và hoàn toàn không hỗ trợ cổng USB. Phía sau thân máy in cũng được dán đè một miếng decal cảnh báo cấm bóc che đi vị trí cổng kết nối:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080502.webp)

Tuy nhiên khi tò mò bóc miếng dán cảnh báo ra, người dùng phát hiện phía sau miếng dán vẫn là một cổng kết nối USB tiêu chuẩn:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080503.webp)

Và khi cắm cáp kết nối trực tiếp cổng USB này vào máy tính, máy in vẫn nhận driver và thực hiện in ấn tài liệu hoàn toàn bình thường:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080504.webp)

Rất khó lý giải tại sao HP lại phải tốn công dán decal để che giấu một tính năng phần cứng cơ bản. Nếu thực sự muốn loại bỏ cổng USB, hãng hoàn toàn có thể tinh chỉnh thiết kế khuôn đúc nhựa hoặc khóa cổng ở tầng firmware, nhưng họ chỉ dùng duy nhất một miếng dán che đi. Giới phân tích nhận định HP làm vậy để ép người dùng kết nối máy in vào mạng WiFi gia đình, từ đó hãng có thể liên tục thu thập dữ liệu hành vi sử dụng và lượng mực in tiêu thụ của người dùng để phục vụ mục đích thương mại.

3、[Nam bán cầu hứng chịu đợt nắng nóng kỷ lục bất thường ngay trong mùa đông](https://www.sohu.com/a/708607595_116237)

Trong khi Bắc bán cầu đang ở giai đoạn đỉnh điểm của mùa hè, Nam bán cầu theo quy luật thời tiết lẽ ra phải ở thời kỳ mùa đông lạnh giá. Tuy nhiên thực tế Nam bán cầu đang hứng chịu một đợt nắng nóng cực đoan chưa từng có:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080509.webp)

Bước vào tháng 8, nhiệt độ tại nhiều khu vực thuộc智利 (Chile) đã vượt mốc 37.8 độ C, thiết lập kỷ lục nắng nóng mùa đông mới. Tại thủ đô Buenos Aires của Argentina, nhiệt độ trung bình ngày cũng vượt mốc 30 độ C (trong khi nhiệt độ trung bình mùa đông các năm trước chỉ dao động quanh mức 14.4 độ C). Tình trạng biến đổi khí hậu đang làm biến mất dần mùa đông tại Nam bán cầu.

4、[Nga phóng thành công tàu vũ trụ Luna 25 sau hàng thập kỷ trì hoãn](https://aviationweek.com/defense-space/space/russias-luna-25-lunar-lander-arrives-vostochny-spaceport)

Vào thứ Năm tuần này, tàu đổ bộ mặt trăng Luna 25 của Nga đã được phóng thành công vào không gian:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080911.webp)

Đây được xem là dự án thám hiểm không gian bị trì hoãn lâu nhất trong lịch sử nước Nga. Con tàu tiền nhiệm Luna 24 đã được phóng từ năm 1976 – tức là cách đây tròn 47 năm. Suốt gần nửa thế kỷ qua, Nga chưa thực hiện thêm bất kỳ dự án đổ bộ mặt trăng nào.

Dự án Luna 25 vốn được lên kế hoạch sơ bộ từ những năm 1990, chính thức khởi động chế tạo vào những năm 2010, hoàn thành lắp ráp thử nghiệm vào năm 2021 và liên tục lùi lịch phóng từ 2022 sang năm nay. Nhiều kỹ sư tham gia thiết kế bản vẽ dự án thời kỳ đầu có lẽ nay đều đã nghỉ hưu.

## Bài viết

1\. [Trung Quốc ban hành quy định bắt buộc khai báo thông tin đối với tất cả ứng dụng di động](https://news.cnstock.com/news,bwkx-202308-5103126.htm)（Tiếng Trung）

Bộ Công nghiệp và Công nghệ thông tin Trung Quốc vừa ban hành thông tư yêu cầu tất cả các ứng dụng di động (bao gồm App và các chương trình mini program chạy trên nền tảng mạng xã hội) hoạt động tại thị trường trong nước bắt buộc phải thực hiện đăng ký khai báo thông tin quản lý (ICP) tương tự như quy định quản lý trang web từ tháng 9 năm nay. Kể từ tháng 4 năm 2024, các ứng dụng không hoàn tất thủ tục khai báo sẽ bị chặn cung cấp dịch vụ mạng.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080907.webp)

2\. [Giới thiệu bản phân phối hệ điều hành Rhino Linux thế hệ mới](https://linuxiac.com/rhino-linux-unveil-its-first-stable-2023-1-release/)（Tiếng Anh）

Bài viết giới thiệu bản phân phối hệ điều hành Rhino Linux mới ra mắt bản ổn định đầu tiên. Hệ điều hành được phát triển dựa trên nền tảng Ubuntu ổn định nhưng áp dụng mô hình cập nhật liên tục (Rolling Release), là sự lựa chọn phù hợp cho nhóm lập trình viên yêu thích sự ổn định của Ubuntu nhưng muốn liên tục trải nghiệm các bản vá phần mềm mới nhất.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080908.webp)

3\. [Tận dụng mạng xã hội phân tán Mastodon để xây dựng hệ thống bình luận blog](https://cassidyjames.com/blog/fediverse-blog-comments-mastodon/)（Tiếng Anh）

Tác giả giới thiệu giải pháp kỹ thuật độc đáo: sử dụng API của mạng xã hội phi tập trung Mastodon để làm hệ thống bình luận tích hợp dưới chân bài viết blog cá nhân. Ưu điểm lớn nhất của giải pháp là dữ liệu bình luận được mở và hoàn toàn phi tập trung, giúp chủ nhân blog tránh được sự kiểm soát thông tin từ các tập đoàn công nghệ lớn.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070701.webp)

4\. [Khóa bảo mật RSA 2048-bit liệu có nguy cơ bị bẻ khóa hoàn toàn vào năm 2030?](https://articles.59.ca/doku.php?id=em:20482030)（Tiếng Anh）

Trong giới mật mã học xuất hiện những lo ngại cho rằng sự gia tăng sức mạnh xử lý của các siêu máy tính và sự phát triển của máy tính lượng tử có thể giúp bẻ khóa hoàn toàn các mã khóa bảo mật RSA 2048-bit vào năm 2030. Tác giả bài viết phân tích chi tiết cơ sở toán học và độ tin cậy của nhận định này.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071102.webp)

5\. [Lịch sử ra đời và chặng đường phát triển của công cụ quản lý Docker Compose](https://brianchristner.io/4000-stars-and-counting-a-trip-down-memory-lane/)（Tiếng Anh）

Tác giả – một trong những người đầu tiên tiếp cận và viết tài liệu hướng dẫn sử dụng Docker – chia sẻ những hồi ức thú vị về giai đoạn phát triển sơ khai của Docker và câu chuyện ra đời của công cụ quản lý đa container Docker Compose từ một dự án nguồn mở nhỏ của cộng đồng.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071103.webp)

6\. [Cẩm nang thiết lập và khai báo tệp tin biểu tượng Favicon phiên bản năm 2023](https://evilmartians.com/chronicles/how-to-favicon-in-2021-six-files-that-fit-most-needs)（Tiếng Anh）

Bài viết kỹ thuật hướng dẫn lập trình viên thiết kế và khai báo các file biểu tượng Favicon cho trang web một cách gọn nhẹ nhất hiện nay, chỉ với tối thiểu 6 file hình ảnh cơ bản là đã đủ đáp ứng tốt yêu cầu hiển thị của hầu hết các dòng trình duyệt và hệ điều hành di động.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071304.webp)

7\. [Hướng dẫn xây dựng tính năng tìm kiếm toàn văn sử dụng cơ sở dữ liệu PostgreSQL](https://xata.io/blog/postgres-full-text-search-engine)（Tiếng Anh）

Tài liệu kỹ thuật hướng dẫn lập trình viên khai thác các tính năng tìm kiếm văn bản nâng cao (Full-text Search) được tích hợp sẵn bên trong hệ quản trị cơ sở dữ liệu PostgreSQL mà không cần thiết lập thêm các bộ công cụ tìm kiếm bên ngoài.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071308.webp)

8\. [Phương pháp tối ưu hóa hiệu năng ứng dụng Node.js tận dụng CPU nhiều nhân](https://www.digitalocean.com/community/tutorials/how-to-scale-node-js-applications-with-clustering)（Tiếng Anh）

Mặc định ứng dụng Node.js hoạt động dưới dạng đơn luồng (single-thread) nên chỉ tận dụng được hiệu năng của một nhân CPU đơn lẻ. Bài viết hướng dẫn cách thức sử dụng thư viện cluster mặc định hoặc công cụ PM2 để phân phối tải ứng dụng chạy song song trên tất cả các nhân CPU của máy chủ.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051902.webp)

## 工具

1、[TypeCell: Môi trường viết mã TypeScript tương tác trực tiếp trên web](https://www.typecell.org/)

Một công cụ tạo tài liệu tương tác trực quan dành cho lập trình viên TypeScript, cho phép người dùng viết và xem kết quả chạy code trực tiếp trên trình duyệt tương tự như mô hình hoạt động của Jupyter Notebook.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061501.webp)

2、[小抽屉 (Pandora): Ứng dụng dịch thuật nội dung màn hình dành cho Android](https://play.google.com/store/apps/details?id=com.mydobby.pandora)

Một ứng dụng tiện ích dành cho điện thoại Android, hỗ trợ quét và dịch trực tiếp các đoạn văn bản hiển thị trên màn hình ứng dụng sang ngôn ngữ đích, giúp người dùng dễ dàng trải nghiệm các app nước ngoài. (Đóng góp của [@tuesda](https://github.com/ruanyf/weekly/issues/3328))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080601.webp)

3、[FoodCa: Tiện ích iOS ghi nhận nhanh lượng calo nạp vào cơ thể qua giọng nói](https://apps.apple.com/cn/app/foodca-ai%E5%8A%A0%E6%8C%81%E7%9A%84%E9%A3%9F%E7%89%A9%E7%83%AD%E9%87%8F%E9%80%9F%E6%9F%A5%E4%B8%8E%E8%AE%B0%E5%BD%95%E5%B7%A5%E5%85%B7/id6451112435)

Ứng dụng di động trên iOS tích hợp API của ChatGPT, cho phép người dùng ghi nhật ký ăn uống hàng ngày bằng cách nói tự nhiên (ví dụ nói "tôi vừa ăn ba quả nho"), hệ thống sẽ tự động phân tích và tính toán lượng calo nạp vào. (Đóng góp của [@wdkwdkwdk](https://github.com/ruanyf/weekly/issues/3330))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080905.webp)

4、[Douyin Chat: Ứng dụng nhắn tin trao đổi của Douyin dành cho máy tính](https://imdesktop.douyin.com/)

Hãng phát triển Douyin (phiên bản TikTok nội địa) vừa qua đã chính thức phát hành phiên bản phần mềm nhắn tin chat độc lập dành cho máy tính PC giúp người dùng dễ dàng trao đổi thông tin. (Đóng góp của [@stefanJi](https://github.com/ruanyf/weekly/issues/3329))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080904.webp)

5、[usememos: Ứng dụng ghi chú cá nhân dạng web tự lưu trữ bảo mật](https://github.com/usememos/memos)

Mã nguồn mở xây dựng ứng dụng lưu trữ ghi chú cá nhân gọn nhẹ hoạt động trên nền web, hỗ trợ người dùng tự triển khai (self-hosted) trên máy chủ cá nhân để bảo vệ quyền riêng tư dữ liệu. (Đóng góp của [@pmxiao](https://github.com/ruanyf/weekly/issues/3349))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081003.webp)

6、[mdBook: Bộ công cụ dòng lệnh đóng gói sách điện tử viết bằng Rust](https://github.com/rust-lang/mdBook)

Công cụ dòng lệnh mạnh mẽ viết bằng Rust hỗ trợ lập trình viên nhanh chóng đóng gói toàn bộ các file tài liệu Markdown thô thành các định dạng sách điện tử PDF hoặc EPUB chuyên nghiệp. (Xem thêm [Tài liệu hướng dẫn sử dụng](https://mp.weixin.qq.com/s?__biz=MzIyNDQ2MTQwOQ==&mid=2247493433&idx=1&sn=8a6f2c9975f34b9e2e7be62479f24478&chksm=e80c3037df7bb9212d320ca3fff025a81347fbc163add2a0456ea5a522ab6a836755af84ccb6&token=1949573976&lang=zh_CN#rd)). (Đóng góp của [@mzhren](https://github.com/ruanyf/weekly/issues/3350))

7、[PDDON: Ứng dụng vẽ sơ đồ tư duy và biểu đồ trực tuyến tích hợp AI](https://pddon.com/)

Trình vẽ biểu đồ thiết kế hệ thống trực tuyến, tích hợp sẵn các tính năng low-code và trợ lý trí tuệ nhân tạo AI giúp người dùng nhanh chóng hoàn thiện các sơ đồ quy trình công việc. (Đóng góp của [@pddon](https://github.com/ruanyf/weekly/issues/3351))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081005.webp)

8、[Ruff: Công cụ kiểm tra lỗi cú pháp Python viết bằng Rust với tốc độ siêu nhanh](https://github.com/astral-sh/ruff)

Trình phân tích và kiểm tra lỗi cú pháp (Linter) dành riêng cho ngôn ngữ Python, được viết hoàn toàn bằng Rust giúp mang lại hiệu năng xử lý và tốc độ quét code nhanh vượt trội so với các công cụ cũ.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061510.webp)

9、[ReactPy: Thư viện hỗ trợ viết giao diện web động bằng mã Python](https://reactpy.dev/docs/index.html)

Một dự án phát triển thư viện Front-end độc đáo cho phép lập trình viên sử dụng trực tiếp các cú pháp và tư duy thiết kế component của React trong Python để xây dựng giao diện trang web động.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061511.webp)

10、[Wasmer: Công cụ dòng lệnh chạy trực tiếp mã WebAssembly trên terminal](https://wasmer.io/)

Trình chạy mã nguồn WebAssembly (Wasm) gọn nhẹ cho phép lập trình viên thực thi trực tiếp các tệp tin wasm từ dòng lệnh mà không cần phụ thuộc vào trình duyệt web. (Xem thêm [Tài liệu giới thiệu phiên bản Wasmer 3.0](https://wasmer.io/posts/announcing-wasmer-3.0)).

11、[GoodbyeDPI: Công cụ hỗ trợ vượt qua bộ lọc DPI của mạng trên Windows](https://github.com/ValdikSS/GoodbyeDPI)

Tiện ích nguồn mở do kỹ sư người Nga phát triển dành riêng cho hệ điều hành Windows, giúp người dùng thay đổi cấu trúc gói tin mạng để vượt qua các bộ lọc kiểm soát gói tin chuyên sâu (DPI) của nhà mạng.

## 资源

1、[Claude 2: Trang web giao diện trải nghiệm Claude 2 miễn phí](https://www.claudeai.ai/)

Trang web cung cấp cổng giao diện kết nối không chính thức với mô hình ngôn ngữ lớn Claude 2 của công ty Anthropic, hỗ trợ người dùng trong nước trải nghiệm đầy đủ các tính năng trò chuyện hoàn toàn miễn phí. (Đóng góp của [@zengdamo](https://github.com/ruanyf/weekly/issues/3338))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081004.webp)

2、[AI Navigation: Thư mục danh bạ tổng hợp các trang web ứng dụng AI](https://ai.dreamthere.cn/)

Trang web chuyên tổng hợp, phân loại và cập nhật liên kết truy cập của hàng trăm dịch vụ ứng dụng trí tuệ nhân tạo đang hoạt động trên Internet. (Đóng góp của [@zllz5230](https://github.com/ruanyf/weekly/issues/3352))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081006.webp)

3、[Video bài giảng giới thiệu sơ đồ kiến trúc các module của thư viện LangChain](https://www.bilibili.com/read/cv25333824)

Video bài giảng kỹ thuật trực quan giới thiệu chi tiết kiến trúc hoạt động của LangChain – framework lập trình ứng dụng LLM phổ biến nhất hiện nay – thông qua một sơ đồ cấu trúc trực quan dễ hiểu. (Đóng góp của [@webup](https://github.com/ruanyf/weekly/issues/3332))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080906.webp)

4\. [Charles Dickens Illustrated Gallery: Kho lưu trữ tranh minh họa cổ các tác phẩm của Charles Dickens](https://www.charlesdickensillustration.org/)

Trang web phi lợi nhuận lưu trữ hàng ngàn bức tranh vẽ minh họa cổ được in kèm trong các tác phẩm tiểu thuyết nổi tiếng của nhà văn Charles Dickens vào thế kỷ 19.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062001.webp)

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062002.webp)

5\. [React Graph Gallery: Thư viện biểu đồ giao diện lập trình bằng React và D3](https://www.react-graph-gallery.com/)

Trang web tổng hợp và cung cấp mã nguồn mẫu của nhiều dạng biểu đồ dữ liệu khác nhau (biểu đồ cột, biểu đồ đường, biểu đồ phân tán) được xây dựng tối ưu bằng sự kết hợp giữa React và thư viện đồ họa D3.js.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062404.webp)

## 图片

1、**Hình ảnh hệ thống lưu trữ hồ sơ cơ khí khổng lồ từ thế kỷ trước**

Các bức ảnh lịch sử dưới đây chụp lại không gian làm việc bên trong kho lưu trữ hồ sơ của Cục Xã hội Tiệp Khắc cũ vào năm 1937. Hệ thống tủ hồ sơ cao tới 5 mét phủ kín các bức tường với tổng cộng hơn 3.000 ngăn kéo lưu trữ lớn:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053002.webp)

Để thao tác tìm kiếm hồ sơ, nhân viên văn phòng sử dụng các bàn làm việc cơ điện đặc biệt chạy trên ray trượt. Bàn làm việc có thể tự động di chuyển ngang dọc và nâng hạ chiều cao đưa kỹ sư lên sát trần nhà để rút ngăn kéo hồ sơ cần tìm:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053007.webp)

Ý tưởng thiết kế hệ thống văn phòng bán tự động này mang đậm sắc màu khoa học viễn tưởng dù được chế tạo từ cách đây gần một thế kỷ:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053004.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053005.webp)

2、**Khám phá mũi tên ẩn giấu tinh tế bên trong Logo thương hiệu FedEx**

FedEx là một trong những tập đoàn chuyển phát nhanh lớn nhất của Mỹ. Logo thương hiệu của hãng thoạt nhìn qua có vẻ rất đơn giản và bình thường:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081001.webp)

Tuy nhiên nếu quan sát kỹ khoảng trống giữa chữ cái E và chữ x, người xem sẽ nhận ra một mũi tên hướng về phía bên phải được tạo hình rất khéo léo, ẩn dụ cho tốc độ giao hàng nhanh chóng và sự chính xác của dịch vụ vận chuyển.

## ✍️ Bài đọc thêm

### Câu chuyện vượt qua nỗi sợ hãi để thành lập nên tập đoàn Nike của Phil Knight

Vào đầu những năm 1960, chàng thanh niên 22 tuổi Phil Knight vừa hoàn thành chương trình tốt nghiệp đại học.

Thời sinh viên, ông vốn là một vận động viên chạy cự ly ngắn trong đội tuyển điền kinh của trường và có sự hiểu biết sâu sắc về các dòng giày chạy. Sau khi tốt nghiệp, ông quyết định khởi nghiệp bằng việc nhập khẩu các mẫu giày chạy giá rẻ của Nhật Bản về bán lại tại thị trường Mỹ.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081007.webp)

Ông phát hiện dòng giày chạy Tiger của Nhật Bản có trọng lượng siêu nhẹ và thiết kế đế bám đường tốt hơn hẳn các thương hiệu giày thể thao nội địa thời bấy giờ, giúp các vận động viên điền kinh cải thiện đáng kể thành tích chạy. Ông quyết định dồn vốn nhập khẩu dòng giày này.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081008.webp)

Thế nhưng chỉ một thời gian ngắn sau, ông nhận được một thư cảnh báo pháp lý từ một công ty lớn. Công ty này tuyên bố họ là đơn vị sở hữu quyền phân phối độc quyền dòng giày Tiger tại thị trường Mỹ và ra lệnh yêu cầu Knight phải dừng ngay việc bán giày nếu không muốn đối mặt với một vụ kiện bản quyền lớn tại tòa án.

Lúc đó Phil Knight vẫn còn là một chàng thanh niên có tính cách khá nhút nhát và gầy gò, tin tức này lập tức dội một gáo nước lạnh vào tinh thần của ông.

Ông nhớ lại: *“Sự việc khiến tôi rơi vào trạng thái sợ hãi tột cùng. Mỗi tối, tôi ngồi ăn cơm cùng gia đình nhưng đầu óc hoàn toàn trống rỗng, sau đó tôi lầm lũi ngồi ở góc phòng khách và chăm chăm nhìn vào màn hình tivi với sự chán nản”*.

Ông đã cân nhắc nghiêm túc việc từ bỏ kinh doanh và tìm một công việc văn phòng bình thường. Tuy nhiên trước khi buông xuôi, ông muốn thử nỗ lực thêm một lần cuối cùng.

Ông viết thư gửi trực tiếp cho tổng công ty sản xuất giày Onitsuka tại Nhật Bản, tha thiết đề xuất họ xem xét lại điều khoản độc quyền và cấp phép cho ông quyền bán lẻ giày tại khu vực bờ Tây nước Mỹ.

Nhưng lá thư gửi đi hoàn toàn không nhận được phản hồi. Sau nhiều tháng im lặng, ông gần như đã chấp nhận thất bại.

Trải qua một thời gian chán nản, khát khao kinh doanh trong ông lại trỗi dậy. Ông nhớ lại: *“Tôi vô cùng lo lắng và sợ hãi về tương lai của mình. Nhưng không hiểu sao, trong đầu tôi lại nảy ra một ý tưởng điên rồ và tôi quyết định phải thực hiện nó bằng được. Tôi không muốn đầu hàng”*.

Ý tưởng điên rồ của ông là tự mình mua vé máy bay bay thẳng sang Nhật Bản, tìm đến trụ sở chính của công ty Onitsuka để xin một cuộc hẹn gặp mặt trực tiếp thuyết phục ban lãnh đạo công ty trao cho ông quyền phân phối dòng giày Tiger tại Mỹ.

Và sự dũng cảm đó đã mang lại quả ngọt: đại diện công ty Nhật Bản sau khi nghe ông trình bày nhiệt huyết đã đồng ý cấp phép cho ông bán giày.

Phil Knight trở về Mỹ mở lại cửa hàng giày chạy của mình, đặt những viên gạch nền móng đầu tiên cho sự phát triển của tập đoàn Nike khổng lồ ngày nay.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081009.webp)

Nếu trong giây phút khủng hoảng đối mặt với thư kiện cáo ngày đó, Phil Knight lựa chọn đầu hàng nỗi sợ hãi để từ bỏ kinh doanh giày, tập đoàn Nike chắc chắn sẽ không bao giờ xuất hiện trên thế giới.

## Lịch sử tuần này

- 2022年（第 219 期）：[Bảo mật số: Hướng dẫn các phương pháp cơ bản giúp người dùng bảo vệ tài khoản cá nhân khỏi nguy cơ bị hack](http://www.ruanyifeng.com/blog/2022/08/weekly-issue-219.html)
- 2021年（第 169 期）：[Thiết kế sản phẩm: Phân tích tư duy thiết kế sản phẩm xe hơi tối giản thực dụng của hãng Wuling](http://www.ruanyifeng.com/blog/2021/07/weekly-issue-169.html)
- 2020年（第 119 期）：[Xã hội học: Mối liên hệ giữa lượng mưa dự báo thực tế và lý thuyết trò chơi trong ngành bảo hiểm nông nghiệp](http://www.ruanyifeng.com/blog/2020/08/weekly-issue-119.html)
- 2019年（第 69 期）：[Hiệu suất công việc: Thảo luận về việc ưu tiên làm tốt chất lượng sản phẩm hay ưu tiên tốc độ hoàn thành dự án](http://www.ruanyifeng.com/blog/2019/08/weekly-issue-69.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes team coordination and knowledge sharing smooth and efficient.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
