# 科技爱好者周刊：第 75 期 (Bản tin chia sẻ công nghệ số 75)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019092604.jpg)

Ảnh bìa: Tiền灘 (Qiantan), Thượng Hải, 2019.

## 刊首语 (Lời tựa)

Trong bối cảnh cả thế giới đang đẩy mạnh sản xuất xe điện, một hãng truyền thông Mỹ đưa ra [nhận định](https://www.detroitnews.com/story/business/autos/2019/09/05/shift-electric-vehicles-radically-change-auto-factories/2208961001/) rằng làn sóng này sẽ dẫn tới tình trạng sa thải công nhân cơ khí ngành ô tô quy mô lớn, và tôi thấy điều này cực kỳ có cơ sở.

Xe hơi truyền thống bản chất là một hệ thống cơ khí phức tạp cấu thành từ hàng vạn chi tiết, chỉ riêng hệ thống truyền động động cơ (powertrain) đã cấu thành từ hơn 2.000 linh kiện cơ học khác nhau.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019092601.jpg)

(Ảnh: Cấu trúc cơ khí vô cùng phức tạp của động cơ xăng truyền thống).

Tuy nhiên, **xe điện bản chất lại là một thiết bị điện tử, với trái tim cốt lõi chỉ gồm động cơ điện và khối pin lưu trữ, số lượng linh kiện cơ học được cắt giảm tối đa.** Hộp số phức tạp, bộ tản nhiệt làm mát, kim phun nhiên liệu, bình xăng, hệ thống ống xả - tất cả đều không còn cần thiết. Thêm vào đó, động cơ điện và các cell pin hoàn toàn có thể mua sẵn từ các nhà cung cấp chuyên biệt bên ngoài, hãng xe không cần duy trì quá nhiều công nhân sản xuất cơ khí.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019092602.jpg)

(Ảnh: Động cơ điện và cấu trúc khối pin dưới sàn xe Tesla Model 3).

Các hãng xe hơi tương lai sẽ có mô hình hoạt động tương tự như các hãng sản xuất máy tính hay điện thoại ngày nay: mua linh kiện cốt lõi từ bên ngoài, chỉ tập trung vào khâu thiết kế thương hiệu, viết phần mềm điều khiển và lắp ráp thành phẩm. Thậm chí, việc lắp ráp hoàn toàn có thể thuê ngoài (outsourcing) cho các đơn vị gia công chuyên nghiệp.

Theo mô hình này, số lượng nhân sự trực tiếp của hãng xe sẽ rất tinh gọn, và hầu hết các vị trí công việc liên quan đến cơ khí chế tạo truyền thống sẽ biến mất.

Mở rộng tư duy này, **trong tương lai, có thể mọi đồ vật xung quanh ta đều sẽ biến đổi thành các thiết bị điện tử**, bởi vì chúng đều sẽ được tích hợp mạch điều khiển, chip vi xử lý và khả năng kết nối mạng. Ví dụ như nồi cơm điện, ổ khóa cửa, giày thể thao, bồn cầu thông minh - những đồ vật trước đây hoàn toàn không liên quan đến máy tính, nay đều đang chuyển mình thành các thiết bị điện tử thông minh.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019092603.jpg)

(Ảnh: Giày thể thao thông minh của Nike tích hợp tính năng tự động thắt dây giày qua ứng dụng).

Xu thế này chỉ ra 3 nhóm ngành công nghiệp sẽ có tiềm năng tăng trưởng vượt trội trong tương lai:
1. **Năng lượng và công nghệ Pin**: cung cấp nguồn năng lượng duy trì hoạt động cho thế giới thiết bị điện tử.
2. **Điện tử và Viễn thông**: đóng vai trò là nền tảng phần cứng và hạ tầng truyền tải kết nối của các thiết bị.
3. **Phần mềm**: hệ thống điều hành và giao diện tương tác trực tiếp của thiết bị với con người.

## Các khóa học miễn phí chất lượng cao trên Udacity

Udacity là một trong những nền tảng giáo dục trực tuyến công nghệ lớn và uy tín nhất của Mỹ mà nhiều người đã biết tới. Bên cạnh các chương trình đào tạo cấp chứng chỉ Nanodegree có thu phí, nền tảng này thực chất sở hữu một kho tài nguyên khóa học hoàn toàn miễn phí cực kỳ đồ sộ.

So với các khóa học trả phí, các khóa học miễn phí chỉ thiếu phần chấm bài tập thực hành lớn và dịch vụ cố vấn học tập 1-1, còn lại toàn bộ nội dung video bài giảng gốc của chuyên gia vẫn được giữ nguyên vẹn, và rất nhiều bài giảng đã có phụ đề tiếng Trung/tiếng Anh đầy đủ. Bạn chỉ cần đăng ký tài khoản là có thể học ngay mà không tốn bất kỳ chi phí nào.

Hầu hết các khóa học miễn phí này tập trung vào mảng lập trình thực chiến cho người mới bắt đầu: từ lập trình web, phát triển ứng dụng di động đến quản trị hệ thống. Trong đó, các khóa học về Flutter và Kotlin được thiết kế phối hợp trực tiếp cùng đội ngũ kỹ sư của Google.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019092606.jpg)

Chất lượng bài giảng của Udacity luôn nhận được đánh giá rất cao từ cộng đồng công nghệ. Nếu bạn đang muốn học lập trình hoặc muốn trải nghiệm thử phương pháp giảng dạy hiện đại của Thung lũng Silicon, hãy tận dụng kỳ nghỉ để tham gia các khóa học miễn phí hữu ích dưới đây:

> - Khóa học: [《Nhập môn HTML and CSS》](https://cn.udacity.com/course/html-and-css-syntax--ud001/?utm_source=wechat-kol-ruanyf&utm_medium=kol&utm_campaign=freecourse) (Có phụ đề tiếng Trung)
> - Khóa học: [《Nhập môn JavaScript》](https://cn.udacity.com/course/intro-to-javascript--ud803/?utm_source=wechat-kol-ruanyf&utm_medium=kol&utm_campaign=freecourse) (Có phụ đề tiếng Trung)
> - Khóa học: [《Làm chủ Git và Quản lý phiên bản》](https://cn.udacity.com/course/version-control-with-git--ud123/?utm_source=wechat-kol-ruanyf&utm_medium=kol&utm_campaign=freecourse) (Có phụ đề tiếng Trung)
> - Khóa học: [《Phát triển ứng dụng di động với Flutter》](https://cn.udacity.com/course/build-native-mobile-apps-with-flutter--ud905/?utm_source=wechat-kol-ruanyf&utm_medium=kol&utm_campaign=freecourse) (Tiếng Anh)
> - Khóa học: [《Nhập môn ngôn ngữ Kotlin》](https://cn.udacity.com/course/kotlin-bootcamp-for-programmers--ud9011/?utm_source=wechat-kol-ruanyf&utm_medium=kol&utm_campaign=freecourse) (Tiếng Anh)
> - Khóa học: [《Lớp học thực hành Shell Unix》](https://cn.udacity.com/course/shell-workshop--ud206/?utm_source=wechat-kol-ruanyf&utm_medium=kol&utm_campaign=freecourse) (Có phụ đề tiếng Trung)
> - Khóa học: [《Hướng dẫn viết tệp README chuẩn mực cho dự án》](https://cn.udacity.com/course/writing-readmes--ud777?utm_source=wechat-kol-ruanyf&utm_medium=kol&utm_campaign=freecourse) (Có phụ đề tiếng Trung)

## 资讯 (Tin tức)

1. **Siêu xe Bugatti Chiron lập kỷ lục tốc độ thế giới mới vượt ngưỡng 300 mph**

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090202.jpg)

Mẫu siêu xe thể thao Chiron do hãng Bugatti (Pháp) chế tạo đã thiết lập kỷ lục tốc độ thế giới mới vào ngày 2/8 khi chạm mốc vận tốc tối đa 304.77 mph (tương đương 490.5 km/h), trở thành siêu xe thương mại đầu tiên vượt qua giới hạn 300 mph. Kỷ lục trước đó thuộc về dòng xe Koenigsegg lập năm 2017 với vận tốc 284.55 mph.

Ở vận tốc khủng khiếp này, chiếc xe về bản chất tương tự như đang bay sát mặt đất, đòi hỏi thiết kế khí động học cực kỳ phức tạp để đảm bảo lực ép xuống mặt đường (downforce) giữ cho xe không bị nhấc bổng khỏi đường ray chạy thử. Bugatti Chiron được trang bị động cơ 16 xi-lanh, 4 bộ tăng áp kép cho công suất tối đa 1.500 mã lực, với mức giá bán thương mại lên tới hơn 3 triệu USD.

2. **Bài toán phân rã số 42 thành tổng ba lũy thừa bậc ba chính thức được các nhà toán học giải quyết**

42 = (-80.538.738.812.075.974)³ + 80.435.758.145.817.515³ + 12.602.123.297.335.631³

Giới toán học từ lâu đã đưa ra giả thuyết rằng mọi số nguyên không thuộc dạng `9n ± 4` đều có thể phân tích được thành tổng của ba số nguyên lũy thừa bậc ba: n = x³ + y³ + z³. Tính đến đầu năm 2019, trong số các số tự nhiên nhỏ hơn 100, chỉ còn duy nhất hai số là `33` và `42` là chưa tìm được đáp án phân rã phù hợp.

Tháng 2/2019, bài toán cho số `33` đã được giải quyết. Và đến đầu tháng 9, các nhà toán học sử dụng mạng lưới siêu máy tính phân tán tiếp tục công bố đáp án phân tích cho số `42` (công thức trên). Hiện tại, trong nhóm các số tự nhiên nhỏ hơn 1.000, vẫn còn 10 số chưa tìm ra lời giải phân rã gồm: 114, 165, 390, 579, 627, 633, 732, 906, 921 và 975.

3. **Doanh thu từ đĩa than (Vinyl) dự báo vượt doanh số đĩa CD tại Mỹ lần đầu tiên kể từ năm 1986**

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090803.jpg)

Hiệp hội Công nghiệp Ghi âm Hoa Kỳ (RIAA) dự báo doanh thu bán đĩa than sẽ chính thức vượt qua doanh thu đĩa CD truyền thống vào cuối năm nay - cột mốc lần đầu tiên xuất hiện sau hơn 3 thập kỷ kể từ năm 1986. Thống kê nửa đầu năm cho thấy đĩa than bán được 8.6 triệu bản đem về 224.1 triệu USD, trong khi CD bán được 18.6 triệu bản thu về 247.9 triệu USD.

Dù số lượng đĩa CD bán ra nhiều hơn nhưng do giá trị sưu tầm của đĩa than lớn nên doanh thu từ đĩa than liên tục tăng trưởng mạnh mẽ (tăng 12% so với cùng kỳ), ngược lại doanh số CD liên tục sụt giảm sâu. Hiện tại, doanh thu từ các định dạng vật lý (đĩa than + CD) chỉ chiếm khoảng 4% tổng doanh thu ngành âm nhạc Mỹ, trong khi doanh thu từ các dịch vụ phát nhạc số trực tuyến như Spotify hay Apple Music chiếm tới 62%.

4. **Thử nghiệm thả muỗi biến đổi gen埃及伊蚊 nhằm kiểm soát dịch bệnh tại Brazil thất bại ngoài thực địa**

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091501.jpg)

Nhằm đẩy lùi bệnh sốt xuất huyết và sốt vàng da, trong giai đoạn 2013-2015, giới khoa học đã liên tục thả khoảng 450.000 con muỗi vằn đực biến đổi gen ra môi trường hàng tháng tại một khu vực của Brazil. Các muỗi đực này mang gen khiếm khuyết khiến đời con sinh ra bị chết trước khi trưởng thành.

Ban đầu, cơ quan y tế kỳ vọng giải pháp sinh học này sẽ giúp cắt giảm 90% quần thể muỗi truyền bệnh tại địa phương. Tuy nhiên, các khảo sát mới nhất cho thấy số lượng muỗi đã phục hồi hoàn toàn về mức cũ, đánh dấu thử nghiệm thất bại. Dù lý thuyết dự tính khoảng 3% đến 4% muỗi con mang gen lỗi vẫn có thể sống sót trưởng thành và con số này là quá nhỏ để phục hồi đàn, nhưng thực tế tiến hóa tự nhiên đã giúp muỗi nhanh chóng thích nghi vượt qua khiếm khuyết di truyền này.

5. **Mackmyra Intelligens - Dòng rượu Single Malt Whisky đầu tiên được phát triển bởi trí tuệ nhân tạo**

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091602.jpg)

Hãng rượu Thụy Điển Mackmyra ra mắt dòng sản phẩm Whisky Intelligens được phát triển hoàn toàn bởi thuật toán AI của Microsoft. AI đã phân tích cơ sở dữ liệu gồm hơn 70 triệu công thức phối trộn rượu hiện có, kết hợp dữ liệu phản hồi của khách hàng và doanh số bán hàng để tự động thiết kế ra một công thức ủ rượu mạch nha đơn cất mới. Dòng rượu thành phẩm mang màu vàng óng ánh với hương vị phức hợp hòa quyện của kẹo bơ cứng, vani kem, lê, táo, tiêu trắng và hương gỗ sồi nướng ấm áp.

6. **Tin vắn**

- Thống kê dân số quốc gia Hàn Quốc năm 2018 ghi nhận tỷ suất sinh (fertility rate) giảm xuống mức kỷ lục 0.98 - trung bình một phụ nữ Hàn Quốc sinh chưa đầy 1 con trong cả cuộc đời, biến Hàn Quốc thành quốc gia duy nhất trên thế giới có tỷ suất sinh tụt dưới mốc 1.

- Trình duyệt bảo mật Brave tích hợp nút thưởng tiền mã hóa BAT ngay trên thanh công cụ, cho phép người dùng lướt web gửi trực tiếp tiền ủng hộ cho các nhà sáng tạo nội dung của các trang web đã xác thực.

- Sau 360 năm lệch hướng do dịch chuyển địa từ, kim指南 châm tại Anh lần đầu tiên chỉ hướng Bắc từ tính trùng khớp hoàn hảo với hướng Bắc địa lý (True North) do đường kinh tuyến không từ tính đi qua đúng trạm thiên văn Greenwich.

- Hệ thống tàu điện ngầm New York bị người dân chỉ trích khi thay thế các bản đồ giấy truyền thống bằng màn hình LCD hiển thị bản đồ số có độ phân giải quá thấp, khiến người đi tàu rất khó nhìn rõ các chi tiết nhỏ của ga chuyển tuyến.

- Hãng đồ ăn nhanh KFC tiến hành thử nghiệm bán các dòng gà viên làm hoàn toàn từ protein thực vật (plant-based chicken nuggets) liên kết cùng hãng Beyond Meat tại thị trường Mỹ.

- Kính viễn vọng không gian Hubble công bố bức ảnh chụp土 tinh (Saturn) với độ nét cực cao vào ngày 20/6, hiển thị rõ ràng cấu trúc các vành đai băng đá xung quanh hành tinh.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091603.jpg)

- Apple chính thức phát hành hệ điều hành chuyên biệt iPadOS cho các dòng máy tính bảng iPad, tích hợp thanh dock ứng dụng mới và hỗ trợ đọc dữ liệu trực tiếp từ USB cắm ngoài.

- Stack Overflow chính thức bổ nhiệm Prashanth Chandrasekar làm CEO mới của nền tảng, tiếp tục khẳng định ưu thế quản trị của nhân sự gốc Ấn Độ trong ban lãnh đạo các tập đoàn công nghệ lớn tại Thung lũng Silicon.

## 文章 (Bài viết)

1、[Bài viết] [Hướng dẫn tối ưu hóa tài nguyên máy chủ bằng cách kích hoạt cơ chế đa tiến trình clustering trong Node.js](https://www.jsmonday.dev/articles/24/how-to-scale-your-node-js-server-using-clustering) (Tiếng Anh)

Mặc định ứng dụng Node.js chạy trên mô hình đơn luồng đơn tiến trình (single-process). Tác giả hướng dẫn sử dụng thư viện tích hợp `cluster` của Node.js để tự động nhân bản tiến trình chạy trên nhiều nhân CPU vật lý giúp tối ưu hiệu suất xử lý tải của máy chủ.

2、[Bài viết] [Tìm hiểu về cấu trúc hoạt động và các thuật toán định tuyến của giao thức chia sẻ file ngang hàng BitTorrent](https://skerritt.blog/bit-torrent/) (Tiếng Anh)

Bài viết giải thích trực quan cơ chế hoạt động của giao thức Torrent: từ cách chia nhỏ tệp tin thành các mảnh (pieces), cơ chế tìm kiếm bạn đồng hành (peers) qua Tracker, thuật toán ưu tiên tải mảnh hiếm (rarest-first) đến nguyên lý hoạt động của mã liên kết từ tính Magnet link.

3、[Bài viết] [Hành trình tự lập trình trình biên dịch self-hosting viết bằng C trong vòng 40 ngày](https://www.sigbus.info/how-i-wrote-a-self-hosting-c-compiler-in-40-days) (Tiếng Anh)

Nhật ký lập trình chi tiết của tác giả ghi lại quá trình tự viết một trình biên dịch ngôn ngữ C có khả năng tự biên dịch chính nó (self-hosting): đi từ 20 dòng code đơn giản ban đầu vào ngày thứ nhất đến khi hoàn thiện hơn 4.000 dòng mã nguồn giải quyết các bài toán parse cú pháp phức tạp.

## 软件 (Phần mềm)

1、[chart.xkcd — Thư viện vẽ biểu đồ số liệu theo phong cách truyện tranh vẽ tay XKCD ngộ nghĩnh](https://github.com/timqian/chart.xkcd)

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019081909.jpg)

Thư viện JavaScript hỗ trợ vẽ các dạng biểu đồ thông dụng (đường, cột, bánh) với hiệu ứng nét vẽ nguệch ngoạc vẽ tay cá tính.

2、[K2pdfopt — Công cụ tối ưu hóa giao diện file PDF hiển thị vừa vặn trên màn hình Kindle và điện thoại](https://www.willus.com/k2pdfopt/)

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082011.jpg)

Tự động quét cấu trúc trang PDF, căn lề và co giãn phông chữ tự động để dàn trang lại thành tệp PDF mới hiển thị sắc nét trên các máy đọc sách màn hình nhỏ mà không cần zoom thủ công.

3、[ShowMeBug — Nền tảng hỗ trợ phỏng vấn viết code trực tuyến theo thời gian thực dành cho nhà tuyển dụng](https://www.showmebug.com/)

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091005.png)

Cung cấp giao diện IDE trực tuyến hỗ trợ đồng bộ thao tác gõ chữ và chạy thử mã nguồn giữa ứng viên phỏng vấn và chuyên gia tuyển dụng từ xa, đi kèm tính năng gọi video trao đổi trực tiếp.

4、[Sổ tay màu sắc truyền thống Trung Hoa — Trang tra cứu mã màu古典 cổ điển trực quan trên nền web](https://works.yangerxiao.com/chinese-colors/)

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019092007.jpg)

Cung cấp bảng phối màu mỹ thuật cổ điển độc đáo kèm tên gọi thơ ca truyền thống và mã màu Hex/RGB tương ứng phục vụ các nhà thiết kế đồ họa.

## 资源 (Tài nguyên)

1、[Tài liệu] [Docker Curriculum - Giáo trình thực hành Docker căn bản dành cho lập trình viên](https://docker-curriculum.com/)

Tài liệu hướng dẫn trực quan giới thiệu các khái niệm container, image, cách viết Dockerfile đóng gói ứng dụng Node.js/Python và triển khai container lên các nền tảng đám mây AWS/DigitalOcean.

2、[Trang web] [justDelete.me - Danh mục tra cứu độ khó khi muốn thực hiện xóa vĩnh viễn tài khoản trên các dịch vụ web](https://backgroundchecks.org/justdeleteme/)

Tổng hợp đường link trực tiếp đến trang xóa tài khoản của hàng trăm dịch vụ internet thông dụng, kèm đánh giá xếp hạng độ khó (Dễ, Trung bình, Khó, Không thể) do nhà cung cấp cố tình gây cản trở.

## 图片 (Hình ảnh)

1. **Tháp điện thoại Stockholm - Chứng tích công nghệ viễn thông khổng lồ thời kỳ sơ khai**

Cách đây hơn 100 năm, hệ thống điện thoại hoạt động hoàn toàn bằng tổng đài chuyển mạch thủ công, đòi hỏi mỗi máy điện thoại gia đình phải có một sợi dây cáp đồng kết nối trực tiếp về bưu điện trung tâm.

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019081102.jpg)

Bức ảnh chụp tòa tháp tổng đài điện thoại khổng lồ tại thủ đô Stockholm (Thụy Điển) hoạt động trong giai đoạn 1887-1913. Tòa tháp là nơi tập hợp của hơn 5.000 sợi dây cáp đồng giăng kín bầu trời thành phố trước khi công nghệ cáp ngầm dưới lòng đất ra đời. Tòa tháp bị tháo dỡ vào năm 1953 sau một vụ hỏa hoạn nghiêm trọng.

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019081103.jpg)

2. **Ảnh tư liệu qua các thời kỳ của Guido van Rossum - cha đẻ ngôn ngữ Python**

Năm 1990, lập trình viên người Hà Lan Guido van Rossum (lúc đó 34 tuổi) bắt đầu viết dự án mã nguồn mở cá nhân trong kỳ nghỉ đông mang tên Python.

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019081207.jpg)

(Ảnh: Guido van Rossum tham dự hội thảo thảo luận Python tổ chức năm 1994).

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019081205.jpg)

(Ảnh: Guido làm việc tại văn phòng Dropbox năm 2014 trước khi chính thức nghỉ hưu).

## 言论 (Danh ngôn)

1、

> "Thực tế, triết lý thiết kế của các sản phẩm vĩ đại không nằm ở việc cố gắng nhồi nhét thật nhiều tính năng phức tạp để gây ấn tượng, mà là tập trung tối giản hóa sản phẩm để giúp cho người dùng của bạn tự động trở nên vĩ đại hơn khi sử dụng nó."
> 
> -- Kathy Sierra

(Hết)
