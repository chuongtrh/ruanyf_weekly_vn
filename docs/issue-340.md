# Bản tin chia sẻ công nghệ (Số 340): Ba mươi năm thổi phồng công nghệ

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/6189) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030508.webp)

Kiến trúc sư Lưu Gia Côn (Liu Jiakun) đến từ Thành Đô tuần này đã chính thức vinh dự nhận giải thưởng Pritzker — giải thưởng danh giá được ví như "Giải Nobel của ngành kiến trúc". Bức ảnh phía trên giới thiệu tác phẩm Bảo tàng Gạch ngự triều ngự dao Tô Châu do ông thiết kế. (Nguồn: [npr.org](https://www.npr.org/2025/03/04/nx-s1-5304312/pritzker-architecture-prize-liu-jiakun))

## 技术炒作三十年

Các bạn có nhận thấy một quy luật trong đời sống công nghệ: Cứ sau một khoảng thời gian nhất định, giới truyền thông lại bắt đầu rầm rộ thổi phồng về một làn sóng công nghệ mới, tuyên bố rằng nó sẽ thay đổi hoàn toàn tương lai nhân loại, khiến cả xã hội dồn sự chú ý và mọi người đi đâu cũng bàn tán xôn xao.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022505.webp)

Làn sóng thổi phồng này chính là khái niệm "phong khẩu" (hướng gió/trend) mà mọi người thường nhắc tới. Hướng gió nổi lên bất ngờ, và như câu nói nổi tiếng: "Khi đứng đúng ngay hướng gió lớn, ngay cả chú heo cũng có thể bay lên cao".

Các bạn có thể liệt kê được bao nhiêu làn sóng thổi phồng công nghệ như vậy trong quá khứ?

Một [lập trình viên nước ngoài](https://wiki.alopex.li/HypeCycles) đã tổng hợp lại các dấu mốc của các chu kỳ thổi phồng công nghệ lớn nhất ghi nhận trong suốt 30 năm qua:

> - Giai đoạn 1998 - 2001: Mạng thông tin toàn cầu WWW (World Wide Web)
> - Giai đoạn 1999 - 2006: Ngôn ngữ lập trình Java
> - Giai đoạn 2004 - 2007: Xu thế Web 2.0
> - Giai đoạn 2007 - 2010: Điện toán đám mây (Cloud Computing)
> - Giai đoạn 2010 - 2015: Mạng xã hội (Social Media)
> - Giai đoạn 2012 - 2015: Internet vạn vật (IoT)
> - Giai đoạn 2013 - 2015: Dữ liệu lớn (Big Data)
> - Giai đoạn 2017 - 2021: Công nghệ chuỗi khối (Blockchain)
> - Giai đoạn 2021 - nay: Trí tuệ nhân tạo (AI)

Các bạn đánh giá dòng danh sách mốc thời gian này có phản ánh chính xác thực tế hay không?

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030501.webp)

Trải nghiệm thực tế của bản thân tôi thấy bảng thống kê này khá tương thích với thực tế. Đây đều là những làn sóng thổi phồng công nghệ cốt lõi và các công nghệ này sau đó đều chứng minh được giá trị thực tế của mình để đi vào đời sống, đó là lý do chu kỳ thổi phồng của chúng kéo dài tương đối lâu từ 2 đến 5 năm trước khi bị thay thế bởi một xu hướng mới.

Bên cạnh đó, thị trường cũng ghi nhận nhiều chu kỳ thổi phồng công nghệ nhỏ hơn nhưng không đạt được thành công tương tự và nhanh chóng hạ nhiệt như: Vũ trụ ảo Metaverse, Web3, kính thực tế ảo tăng cường AR/VR, công nghệ in 3D, xe tự lái...

Để một công nghệ mới có khả năng tạo ra một làn sóng thổi phồng quy mô lớn và kéo dài dài hạn, điều kiện tiên quyết bắt buộc là **nó phải sở hữu giá trị cốt lõi thực tế và có năng lực mang lại những thay đổi rõ rệt cho nền kinh tế xã hội**.

Toàn bộ danh sách công nghệ kể trên thực tế đều đại diện cho các bước tiến đột phá lớn làm thay đổi hoàn toàn bản đồ công nghệ thế giới, hoàn toàn không phải là những bánh vẽ trống rỗng. Nếu bổ sung thêm các dấu mốc của **điện thoại thông minh, video ngắn và tiền mã hóa**, chúng ta sẽ có được bức tranh toàn cảnh về các hướng gió công nghệ lớn nhất trong suốt ba thập kỷ qua.

Trước đây tôi từng mắc một sai lầm trong nhận thức khi luôn tỏ ra coi thường các làn sóng thổi phồng công nghệ, cho rằng đó chỉ là những đợt sóng truyền thông ồn ào mang tính bầy đàn không khác gì các sự kiện tạo scandal của giới giải trí.

Chỉ đến khi bước vào độ tuổi trung niên, tôi mới thấu suốt rằng quan điểm đó là hoàn toàn sai lầm, và là một kỹ sư công nghệ, bạn tuyệt đối không được phép duy trì tư duy đó. **Mỗi một làn sóng thổi phồng công nghệ không đơn thuần là tiếng ồn truyền thông, mà chính là cơ hội vàng**. Nó mang đến sự tập trung cao độ của toàn xã hội, dòng vốn đầu tư khổng lồ đổ về một cách điên cuồng và các nhu cầu tuyển dụng thực tế vô cùng lớn. Làn sóng thổi phồng càng lớn bao nhiêu, dòng vốn đầu tư và cơ hội đi kèm càng khổng lồ bấy nhiêu.

Sau mỗi chu kỳ thổi phồng công nghệ quy mô lớn, thị trường luôn ghi nhận sự ra đời của các doanh nghiệp biểu tượng đạt tốc độ tăng trưởng thần tốc, kiến tạo nên những hiệu ứng tài sản khổng lồ. Nếu bạn may mắn đứng trong làn sóng đó, sự nghiệp và tài chính cá nhân của bạn sẽ tự động bay cao theo xu hướng.

Chúng ta hãy cùng nhìn nhận thực tế: Quỹ thời gian sung sức nhất của một kỹ sư phần mềm về cả năng lực lập trình, sức sáng tạo và cơ hội phát triển sự nghiệp chỉ kéo dài trong khoảng vài năm ngắn ngủi. Để tạo bước đột phá lớn cho sự nghiệp và xây dựng bệ phóng vững chắc cho tương lai, chỉ có năng lực chuyên môn thuần túy là hoàn toàn chưa đủ, **bạn bắt buộc phải đón đầu được ít nhất một làn sóng công nghệ lớn** nhằm tận dụng nguồn lực tài chính và nhu cầu khổng lồ từ bên ngoài để phóng đại nỗ lực cá nhân của mình.

Nếu không, chỉ dựa vào việc tích lũy nỗ lực tự thân đơn lẻ, tiến trình sẽ diễn ra vô cùng chậm chạp và khó lòng đạt tới những vị trí cao hơn. Rất có thể bạn sẽ phải làm việc vô cùng vất vả suốt 20 năm nhưng vẫn chỉ quanh quẩn xử lý các tác vụ cơ bản. Đến khi có một đợt nâng cấp công nghệ lớn xảy ra khiến kỹ năng cũ của bạn bị đào thải, con đường sự nghiệp phía trước sẽ vô cùng chật vật. Đón đầu hướng gió công nghệ thực chất chính là con đường thực tế nhất giúp bạn hiện thực hóa sự thay đổi tầng lớp xã hội và xoay chuyển cuộc đời.

Do đó, mỗi làn sóng công nghệ lớn nổi lên hoàn toàn không đơn thuần là sự thổi phồng bầy đàn vô nghĩa, nó luôn ẩn chứa những cơ hội phát triển thực tế rất đáng để chúng ta quan tâm và theo sát. Đây cũng chính là lý do tại sao bản tin chia sẻ công nghệ hằng tuần luôn dành sự quan tâm đặc biệt và đưa ra các đánh giá tích cực trước các công nghệ mới xuất hiện.

Tất nhiên, điều kiện tiên quyết để bạn có thể đón đầu được hướng gió công nghệ **vẫn là năng lực thực tế của bản thân** để xây dựng nên những sản phẩm chất lượng. Nếu không, ngay cả khi hướng gió lớn xuất hiện trước mắt, bạn cũng không có đủ khả năng để nắm bắt và tận dụng được phần lợi ích từ làn sóng thổi phồng đó mang lại.

## [活动] AI FOR CODE 创意挑战赛

Các bạn còn nhớ thông tin về cuộc thi lập trình ứng dụng AI cấp quốc gia được giới thiệu trong số bản tin tuần trước hay không?

Để tạo điều kiện cho đông đảo mọi người cùng tham gia thử sức, bên cạnh bảng đấu "Phát triển Ứng dụng" truyền thống, ban tổ chức đã mở rộng thêm bảng đấu "Đề xuất Ý tưởng".

**Chỉ cần bạn sở hữu các ý tưởng sáng tạo độc đáo là đã hoàn toàn có thể đăng ký tham gia**, không yêu cầu năng lực viết code thực tế, tác vụ lập trình sẽ được giao phó hoàn toàn cho các trợ lý AI đảm nhận.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030619.webp)

Bảng đấu "Đề xuất Ý tưởng" chính thức mở cổng nhận bài thi từ ngày hôm nay (7 tháng 3) và sẽ đóng cổng nhận bài vào ngày 27 tháng 3 tới.

Nếu bạn sở hữu bất kỳ ý tưởng sáng tạo nào mong muốn AI hỗ trợ hiện thực hóa, hãy nhanh chóng gửi bài thi về khu vực nhận bài của cuộc thi. Nội dung bài thi cần được biên soạn theo đúng [mẫu cấu trúc yêu cầu](https://bytedance.larkoffice.com/docx/RooLdy1Q7oXVzXx9MJMcWfNcnCe) từ ban tổ chức.

Lưu ý rằng toàn bộ các ý tưởng dự thi sẽ được hiển thị công khai trên hệ thống để cộng đồng tham gia bình chọn. **Những ý tưởng xuất sắc nhận được lượt bình chọn cao nhất từ cộng đồng sẽ nhận được các phần quà vô cùng giá trị**.

Mỗi thí sinh được phép gửi tối đa 5 ý tưởng dự thi. Đặc biệt, nếu có đội thi khác lựa chọn khai thác ý tưởng của bạn để phát triển thành sản phẩm thực tế cho cuộc thi, bạn sẽ nhận được một phần quà tri ân đặc biệt từ ban tổ chức!

Đừng bỏ lỡ cơ hội tham gia sân chơi sáng tạo này, chỉ cần bạn dám nghĩ là đã có cơ hội giành giải thưởng. Để biết thêm thông tin chi tiết về thể lệ gửi bài và quy chế bình chọn, các bạn có thể [click vào đây](https://sourl.co/5thdnz) hoặc quét mã QR trên poster giới thiệu.

## 修复壁画的新方法

Tại nhà thờ Padua (Ý) từng sở hữu một bức bích họa khổng lồ từ thời Trung cổ vô cùng tinh xảo và có giá trị nghệ thuật lớn.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021806.webp)

Tuy nhiên, công trình nghệ thuật này đã bị bom đạn chiến tranh phá hủy hoàn toàn trong một đợt không kích vào năm 1944 của Thế chiến thứ hai.

Bức ảnh phía dưới giới thiệu hình ảnh phục dựng kỹ thuật số một phần của bức bích họa trước khi bị phá hủy.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021807.webp)

Sau khi sự cố xảy ra, người dân và các nhà bảo tồn đã thu gom toàn bộ các mảnh vỡ của bức tường bích họa với tổng số lượng lên tới hơn 88.000 mảnh và lưu giữ cẩn thận trong bảo tàng.

Bức ảnh dưới đây chụp lại các mảnh vỡ được lưu giữ, toàn bộ số mảnh vỡ này thực chất mới chỉ chiếm khoảng 10% diện tích của bức bích họa gốc.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021808.webp)

Do số lượng mảnh vỡ quá khổng lồ đi kèm tỷ lệ thất thoát quá lớn, trong suốt nhiều thập kỷ qua, hầu như không một nhà bảo tồn nào dám nghĩ đến việc khôi phục lại tác phẩm nghệ thuật này theo phương pháp thủ công.

Tuy nhiên vào năm 1992, bảo tàng đã tiến hành chụp ảnh kỹ thuật số toàn bộ các mảnh vỡ này để lưu kho tư liệu.

Biết được thông tin này, giáo sư toán học Massimo Fornasier đến từ Đại học Kỹ thuật Munich (Đức) đã quyết định thử nghiệm giải pháp ứng dụng thuật toán máy tính để tiến hành ghép nối các mảnh vỡ dựa trên kho ảnh kỹ thuật số.

Để làm căn cứ đối chiếu cho thuật toán, nhóm nghiên cứu đã sử dụng một bức ảnh đen trắng duy nhất của bức bích họa được chụp từ trước chiến tranh (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021809.webp)

Bước đầu tiên của giáo sư Massimo và cộng sự là ứng dụng AI để phục dựng màu sắc cho bức ảnh đen trắng gốc thành ảnh màu.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021810.webp)

Sau đó, hệ thống sẽ thực hiện phân tích và so khớp hình ảnh của từng mảnh vỡ để định vị chính xác vị trí ban đầu của nó trên bức bích họa (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021811.webp)

Dưới đây là hình ảnh các mảnh vỡ sau khi được định vị thành công lên khung tường.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021814.webp)

Đối với những mảng tường bị mất mảnh vỡ, đội ngũ thiết kế lựa chọn giải pháp bù đắp bằng các mảng màu xám trắng trung tính để làm nổi bật các mảnh vỡ gốc.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021812.webp)

Hình ảnh kết quả phục dựng kỹ thuật số toàn phần của tác phẩm:

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021815.webp)

## 科技动态

1、Thiết bị đổ bộ **"Blue Ghost"** (Lục Hồn) do doanh nghiệp hàng không vũ trụ Firefly Aerospace (Mỹ) chế tạo đã thực hiện hạ cánh thành công xuống bề mặt Mặt Trăng, đánh dấu cột mốc lần đầu tiên một doanh nghiệp tư nhân tự chủ thực hiện thành công sứ mệnh đổ bộ Mặt Trăng trong lịch sử.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030401.webp)

2、Một doanh nghiệp công nghệ sinh học Mỹ công bố đã can thiệp thành công vào mã gen quy định lông của loài chuột, nuôi cấy thành công giống chuột có lớp lông dày ấm áp giống như loài voi ma mút cổ xưa (woolly mouse).

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030509.webp)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030510.webp)

Mục tiêu nghiên cứu tiếp theo của dự án là hướng tới việc hồi sinh loài voi ma mút lông xoăn đã tuyệt chủng.

3、Hãng xe Honda vừa giới thiệu nguyên mẫu xe máy điện mang phong cách thiết kế độc đáo lấy cảm hứng từ nhân vật Koraidon trong tựa game Pokemon nổi tiếng.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030511.webp)

4、Lenovo giới thiệu nguyên mẫu máy tính xách tay chạy năng lượng mặt trời với phần nắp lưng được bao phủ hoàn toàn bởi các tấm pin năng lượng mặt trời.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030614.webp)

Hãng công bố chỉ cần phơi máy dưới nắng khoảng 20 phút là đủ cấp điện năng cho máy phát video liên tục trong 1 giờ. Tuy nhiên dưới góc nhìn thực tế, giải pháp này có vẻ kém hiệu quả và bất tiện hơn nhiều so với việc sử dụng một tấm pin năng lượng mặt trời di động bên ngoài để sạc cho máy tính.

5、Tập đoàn Microsoft thông báo kế hoạch chính thức khai tử dịch vụ gọi điện và nhắn tin Skype vào tháng 5 năm nay để chuyển dịch toàn bộ người dùng sang ứng dụng Microsoft Teams. Trước kỷ nguyên bùng nổ của điện thoại thông minh, Skype từng là phần mềm gọi điện thoại quốc tế qua Internet phổ biến nhất thế giới.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022801.webp)

## 文章

1、[Tìm hiểu kỹ thuật truyền tải dữ liệu HTML trực tiếp (Streaming HTML)](https://rinici.de/posts/streaming-html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025011908.webp)

Hầu hết các phản hồi hội thoại của chatbot AI hiện nay đều được truyền tải dưới dạng dòng dữ liệu (streaming). Bài viết hướng dẫn một mẹo nhỏ giúp nhà phát triển thiết lập tính năng truyền dữ liệu dạng dòng này trực tiếp bằng HTML mà hoàn toàn không cần viết mã nguồn JavaScript.

2、[Khuyến nghị hạn chế sử dụng cú pháp Enum trong TypeScript](https://blog.disintegrator.dev/posts/ode-to-typescript-enums/) (tiếng Anh)

Tài liệu chính thức của ngôn ngữ TypeScript hiện tại đã không còn khuyến khích lập trình viên khai thác cú pháp `enum` (liệt kê). Tác giả bài viết đề xuất giải pháp thay thế tối ưu hơn bằng việc sử dụng định dạng chuỗi kết hợp (union types).

3、[Kinh nghiệm tự động hóa quy trình chuyển đổi âm thanh podcast thành văn bản bằng AI chạy cục bộ](https://den.dev/blog/how-i-automated-podcast-transcription-with-local-ai/) (tiếng Anh)

Bài hướng dẫn chi tiết các bước thiết lập công cụ mã nguồn mở [roboscribe](https://github.com/dend/roboscribe) để tự động hóa quy trình chuyển dịch các tệp âm thanh podcast dài thành định dạng văn bản đọc một cách tối ưu.

4、[Hướng dẫn thiết lập các kịch bản kiểm thử (Test Cases) cho hệ thống thang máy](http://hanzilu.com/wordpress/?p=239) (tiếng Trung)

Bài viết hướng dẫn phương pháp mô hình hóa hoạt động phức tạp của thang máy thành cấu trúc một "máy trạng thái hữu hạn" (finite state machine) để từ đó thiết kế nên các kịch bản kiểm thử phần mềm khoa học và toàn diện. (Đóng góp từ [@lezhi12](https://github.com/ruanyf/weekly/issues/6207))

5、[Lý do tôi quyết định chuyển sang sử dụng trình duyệt Firefox dài hạn](https://www.howtogeek.com/why-i-switched-to-firefox-and-never-looked-back/) (tiếng Anh)

Tác giả chia sẻ những trải nghiệm thực tế chứng minh những ưu thế vượt trội về mặt bảo mật và các tính năng tiện ích độc đáo của trình duyệt Mozilla Firefox so với Google Chrome.

6、[Giải pháp viết mã kịch bản (Scripts) thay thế cho việc cấu hình Alias trong terminal](https://evanhahn.com/why-alias-is-my-last-resort-for-aliases/) (tiếng Anh)

Việc viết các bí danh (alias) để rút ngắn các câu lệnh terminal dài là giải pháp rất phổ biến của lập trình viên. Tuy nhiên, tác giả đề xuất một phương pháp quản lý khoa học và dễ bảo trì hơn bằng cách viết các tệp kịch bản lệnh ngắn thay thế cho alias.

7、[Những giá trị thực tế của công cụ mạng ảo Tailscale trong công việc](https://blog.6nok.org/tailscale-is-pretty-useful/) (tiếng Anh)

Tác giả hướng dẫn cách thức ứng dụng công cụ mạng ảo Tailscale để kết nối toàn bộ các thiết bị công nghệ cá nhân nằm ở các mạng internet khác nhau thành một mạng cục bộ ảo (VPN) bảo mật và tiện lợi.

## 工具

1、[Yaak](https://github.com/mountain-loop/yaak)

Ứng dụng máy tính mã nguồn mở hỗ trợ lập trình viên gửi yêu cầu và kiểm thử các cổng kết nối API với giao diện quản trị hiện đại và đầy đủ tính năng.

2、[cleanmac](https://github.com/hkdobrev/cleanmac)

Bộ kịch bản lệnh dòng lệnh (shell script) gọn nhẹ hỗ trợ người dùng macOS nhanh chóng dọn dẹp các tệp tin rác hệ thống để giải phóng bộ nhớ.

3、[Lynx](https://lynxjs.org/)

Dự án mã nguồn mở do tập đoàn ByteDance phát triển hỗ trợ xây dựng ứng dụng di động đa nền tảng (cross-platform) sử dụng các cú pháp web tiêu chuẩn nhưng kết xuất ra giao diện ứng dụng native mượt mà tương tự bộ khung React Native.

4、[appstat](https://pragmar.com/appstat/)

Ứng dụng giám sát tài nguyên dành cho hệ điều hành Windows, hỗ trợ hiển thị chi tiết mức độ tiêu thụ bộ nhớ RAM, CPU và băng thông mạng của từng phần mềm đang chạy thời gian thực.

5、[Maestro](https://github.com/mobile-dev-inc/Maestro)

Bộ công cụ hỗ trợ chạy thử nghiệm giao diện tự động (UI Testing) cho cả ứng dụng Web và Di động thông qua việc biên soạn các tệp cấu hình YAML đơn giản.

6、[Git Worktree Manager](https://github.com/jackiotyu/git-worktree-manager)

Tiện ích mở rộng trên VS Code hỗ trợ lập trình viên nhanh chóng quản lý, chuyển đổi qua lại giữa các nhánh và kho chứa code Git khác nhau bằng giao diện trực quan. (Đóng góp từ [@jackiotyu](https://github.com/ruanyf/weekly/issues/6198))

7、[Hugo Translator](https://github.com/Rico00121/hugo-translator)

Bộ kịch bản Python hỗ trợ tự động dịch thuật các bài viết định dạng Markdown của blog tĩnh Hugo từ tiếng Trung sang tiếng Anh thông qua việc kết nối API mô hình dịch thuật. (Đóng góp từ [@Rico00121](https://github.com/ruanyf/weekly/issues/6199))

8、[Page-Spy (O-Spy)](https://github.com/HuolalaTech/page-spy-web/)

Công cụ hỗ trợ ghi nhận và phát lại chi tiết toàn bộ các thao tác tương tác của người dùng trên trang web, hỗ trợ đắc lực cho lập trình viên từ xa trong quá trình gỡ lỗi (debugging). (Đóng góp từ [@wqcstrong](https://github.com/ruanyf/weekly/issues/6202))

9、[MTranServer](https://github.com/xxnuo/MTranServer)

Dự án máy chủ dịch thuật offline mã nguồn mở được thiết kế tối ưu hiệu năng để hoạt động mượt mà ngay trên cấu hình phần cứng tối thiểu chỉ cần 1 nhân CPU và 1GB RAM, hỗ trợ tích hợp trực tiếp vào tiện ích mở rộng Immersive Translate. (Đóng góp từ [@xxnuo](https://github.com/ruanyf/weekly/issues/6208))

10、[Screen Sharing Application](https://github.com/tonghohin/screen-sharing)

Ứng dụng chia sẻ màn hình thời gian thực mã nguồn mở được xây dựng trên nền tảng Next.js, hỗ trợ truyền tải tín hiệu trực tiếp ngang hàng (P2P) thông qua việc sinh mã phòng truy cập nhanh mà không cần cài đặt phần mềm trung gian.

## AI 相关

1、[olmOCR](https://github.com/allenai/olmocr)

Bộ công cụ viết bằng Python hỗ trợ ứng dụng các mô hình AI thị giác chuyên dụng để nhận diện và trích xuất chữ viết từ các tài liệu hình ảnh PDF quét với độ chính xác cao.

2、[Probly](https://github.com/PragmaticMachineLearning/probly)

Ứng dụng quản lý bảng tính thông minh tích hợp trí tuệ nhân tạo, cho phép người dùng viết và chạy các đoạn mã Python để xử lý dữ liệu trực tiếp trên bảng tính ngay trên trình duyệt.

3、[Hacker News Daily Podcast](https://github.com/ccbikai/hacker-news)

Chương trình tự động hóa hằng ngày: Tự động thu thập các bài viết nóng hổi nhất trên diễn đàn Hacker News, sau đó ứng dụng AI dịch nghĩa và sinh nội dung âm thanh podcast tóm tắt tin tức bằng tiếng Trung. (Đóng góp từ [@Y024](https://github.com/ruanyf/weekly/issues/6200))

4、[Ngữ Tích (Yuxi-Know)](https://github.com/xerrors/Yuxi-Know)

Công cụ hỗ trợ quản lý cơ sở tri thức cá nhân và tự động dựng sơ đồ tư duy liên kết tri thức (Knowledge Graph) dựa trên công nghệ AI. (Đóng góp từ [@xerrors](https://github.com/ruanyf/weekly/issues/6215))

5、[DiffRhythm](https://github.com/ASLP-lab/DiffRhythm)

Nguyên mẫu mô hình sinh nhạc bằng trí tuệ nhân tạo do phòng thí nghiệm ASLP thuộc Đại học Kỹ thuật Tây Bắc (Trung Quốc) nghiên cứu phát triển. (Đóng góp từ [@JoeDeanx](https://github.com/ruanyf/weekly/issues/6218))

## 资源

1、[Meta AI Demos](https://aidemos.meta.com/)

Trang web giới thiệu và cho phép người dùng trực tiếp trải nghiệm các mô hình và phát kiến công nghệ AI mới nhất từ phòng thí nghiệm của tập đoàn Meta.

2、[ProWords](https://prowords.zeabur.app)

Nền tảng hỗ trợ học và ghi nhớ từ vựng tiếng Anh thông minh ứng dụng AI để tự động tạo ra các câu ví dụ thực tế tương thích với ngành nghề chuyên môn của người học. Mã nguồn dự án được [chia sẻ công khai tại GitHub](https://github.com/winterfx/ProWords). (Đóng góp từ [@winterfx](https://github.com/ruanyf/weekly/issues/6217))

3、[Trải nghiệm tham quan 3D Vương cung thánh đường Thánh Phêrô](https://virtual.basilicasanpietro.va/en)

Vương cung thánh đường Thánh Phêrô tại Vatican là công trình nhà thờ Thiên Chúa giáo lớn nhất thế giới. Trang web cung cấp trải nghiệm tham quan mô phỏng dưới dạng không gian 3D tương tác với độ chi tiết cực cao.

4、[Shapecatcher](https://shapecatcher.com/)

Dịch vụ tìm kiếm ký tự độc đáo: Người dùng vẽ phác thảo một hình dáng bất kỳ lên khung vẽ, hệ thống sẽ tự động quét đối chiếu để trả về các ký tự Unicode (bao gồm cả ký tự Emoji và hệ chữ tượng hình Đông Á) có hình dáng tương đồng nhất.

## 图片

1、[Giải pháp in ấn mã vạch siêu dài của siêu thị ALDI](https://thehill.com/homenews/nexstar_media_wire/5006900-whats-up-with-aldis-trippy-barcodes/)

Chuỗi siêu thị giá rẻ ALDI của Đức áp dụng một phương thức thiết kế bao bì độc đáo khi in các mã vạch (barcodes) sản phẩm có chiều dài chạy dọc gần như toàn bộ bao bì để giúp nhân viên thu ngân dễ dàng quét mã nhanh nhất ở mọi góc độ.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112508.webp)

Đối với các sản phẩm có kích thước bao bì nhỏ không đủ không gian in mã vạch dài, hãng lựa chọn giải pháp in đồng thời nhiều mã vạch ở các mặt khác nhau của bao bì.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112509.webp)

Bức ảnh phía trên minh họa hộp mì ống phô mai được in mã vạch ở cả mặt bên và mặt đáy của vỏ hộp.

2、[Mô hình hệ Mặt Trời hoạt động bằng gạch Lego (Lego Orrery)](https://marian42.de/article/orrery/)

Một tín đồ Lego đã tự thiết kế và lắp ráp thành công mô hình cơ học chuyển động mô phỏng hoạt động của Trái Đất và Mặt Trăng quay quanh Mặt Trời.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061005.webp)

Khối tròn màu vàng ở trung tâm đại diện cho Mặt Trời, Trái Đất được thiết kế quay xung quanh Mặt Trời với góc nghiêng trục quay mô phỏng thực tế 22,5 độ.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061006.webp)

Bên cạnh Trái Đất cũng được thiết kế mô hình Mặt Trăng chuyển động đồng bộ. Quỹ đạo của Mặt Trăng thực tế có góc nghiêng 5,15 độ nhưng rất khó phát hiện bằng mắt thường trên mô hình.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061007.webp)

Toàn bộ hệ thống cơ học có khả năng chuyển động mượt mà nhờ một cấu trúc bánh răng truyền động vô cùng phức tạp và tinh xảo ở bên trong.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061008.webp)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061009.webp)

## 文摘

1、[Mối quan hệ đứt gãy nhận thức giữa cấp quản lý cao cấp và nhân viên thông thường](https://x.com/EthanEvansVP/status/1895845734177452369)

Tác giả: Ethan Evans (Cựu Phó chủ tịch tập đoàn Amazon)

Tôi đã chính thức nghỉ hưu sau hơn 15 năm cống hiến tại Amazon ở cương vị Phó chủ tịch phụ trách các đội ngũ kỹ sư toàn cầu quy mô hơn 800 nhân sự.

Trong suốt nhiệm kỳ làm việc của tôi, giá trị cổ phiếu của Amazon đã ghi nhận mức tăng trưởng kỷ lục lên tới 9.082%, do đó bản thân tôi hầu như không có cơ hội trải nghiệm hay thấu hiểu được những khó khăn tài chính hằng ngày của một người dân lao động bình thường. Đối với các vị trí quản lý cao hơn như CEO hay các phó chủ tịch khác, khoảng cách nhận thức này lại càng xa vời hơn. Việc thảo luận về khối tài sản cá nhân khổng lồ luôn là một chủ đề cấm kỵ mà hầu hết các lãnh đạo cấp cao đều tìm cách né tránh trước công chúng.

Hôm nay tôi muốn chia sẻ thẳng thắn về chủ đề này thông qua việc tự phác họa chân dung cuộc sống cá nhân của mình ở 4 khía cạnh: 1) Tôi hoàn toàn không có bất kỳ khoản nợ thế chấp mua nhà nào; 2) Định kỳ mỗi hai tuần đều có nhân viên dọn dẹp đến vệ sinh toàn bộ nhà cửa; 3) Tôi chi tiền thuê người cắt cỏ cho khu vườn của mình; 4) Tôi chính thức nghỉ hưu tự do ở độ tuổi 50.

Một gia đình bình dân thông thường, ngay cả đối với các gia đình kỹ sư hay trí thức có thu nhập tốt, hầu như cũng khó có được cuộc sống an nhàn như vậy.

Đối với các vị trí lãnh đạo cấp cao hơn tôi, những đặc quyền họ sở hữu còn vượt trội hơn nhiều, tiêu biểu như: 1) Có các khu biệt thự nghỉ dưỡng riêng được thuê nhân sự trông coi và bảo trì quanh năm; 2) Di chuyển bằng chuyên cơ riêng; 3) Có trợ lý cá nhân lo liệu toàn bộ các tác vụ sinh hoạt hằng ngày như thanh toán hóa đơn, mua sắm nhu yếu phẩm hay đưa đón con cái; 4) Có tài xế riêng; 5) Con cái được học tập tại các trường tư thục đắt đỏ hàng đầu; 6) Có quyền tự do lựa chọn sinh sống tại bất kỳ đâu trên thế giới.

Chi phí tài chính chưa bao giờ là rào cản đối với nhóm người này.

Bây giờ chúng ta hãy cùng phân tích một ví dụ điển hình minh họa cho sự đứt gãy nhận thức giữa cấp quản lý và nhân viên: Quyết định chấm dứt chế độ làm việc từ xa để bắt buộc nhân viên quay trở lại văn phòng làm việc.

Khối tài sản khổng lồ giúp các lãnh đạo cấp cao có những sự lựa chọn khác biệt. Hầu hết các nhà quản lý luôn đặt công việc và sự thành công của sự nghiệp lên ưu tiên hàng đầu trong cuộc sống (nếu không sở hữu tư duy đó, họ rất khó có thể leo lên được các vị trí lãnh đạo). Họ sử dụng tài chính để mua lại thời gian cá nhân. Phần lớn quỹ thời gian trong ngày của họ được dành cho công việc và chỉ một phần nhỏ dành cho gia đình. Khi công việc là trọng tâm duy nhất của cuộc sống, việc yêu cầu quay trở lại văn phòng làm việc đối với họ là một quyết định vô cùng hợp lý và hiển nhiên.

Bạn hãy cùng hình dung ngày làm việc của một phó chủ tịch: Không phải lo lắng về việc chen chúc trên các phương tiện giao thông công cộng vì đã có tài xế đưa đón tận nơi giúp họ tranh thủ làm việc trên xe; không phải vội vã chạy về nhà đón con hay lo lắng việc mua sắm, nấu nướng và dọn dẹp nhà cửa vì đã có hệ thống trợ lý và người giúp việc lo liệu; việc học tập của con cái cũng được giao phó cho các trường tư thục chất lượng cao hỗ trợ. Trong một điều kiện sống lý tưởng như vậy, việc đến văn phòng làm việc mang lại cho họ cảm giác vô cùng năng suất và đáng giá.

Mục tiêu của bài chia sẻ này hoàn toàn không phải là một bài luận chỉ trích khối tài sản của các lãnh đạo cấp cao (bản thân tôi cũng đã phải đánh đổi 25 năm làm việc cật lực để có được khối tài sản hiện tại). Mục tiêu của tôi là giúp các bạn nhân viên thấu hiểu được nguyên nhân sâu xa dẫn đến sự đứt gãy nhận thức này.

Khi bạn cần thuyết phục hoặc gây ảnh hưởng đến các quyết định của cấp quản lý cao cấp — những người vốn có cuộc sống tách biệt hoàn toàn với thực tế sinh hoạt hằng ngày của bạn — đừng chỉ đưa ra những lời than vãn cá nhân. Hãy thuyết phục họ bằng các câu chuyện thực tế sinh động, hình ảnh trực quan và các số liệu thống kê khoa học để giúp họ nhìn nhận rõ thực tế cuộc sống của số đông. Hãy ghi nhớ rằng họ thực sự đang sinh sống ở một thế giới khác. Điều đó không có nghĩa họ là những người xấu xa, đơn giản chỉ là họ đã bị đứt gãy nhận thức thực tế. Bản thân tôi trước đây luôn cố gắng phòng tránh việc rơi vào trạng thái đứt gãy này, nhưng phải thừa nhận rằng đó là một xu thế tất yếu sẽ xảy ra theo thời gian khi địa vị của bạn thay đổi.

## 言论

1、

Khởi nghiệp bán thời gian (Side Project) không phải là giải pháp có thể duy trì được trong dài hạn. Nếu ban ngày bạn phải làm việc căng thẳng 8 tiếng trước màn hình máy tính tại công sở, tối về lại tiếp tục ngồi trước một màn hình máy tính khác để tự phát triển phần mềm cá nhân, bạn sẽ nhanh chóng rơi vào trạng thái kiệt sức.

Bạn có thể duy trì lối sống này trong vòng vài tháng, nhưng vấn đề là các dự án khởi nghiệp thường yêu cầu một khoảng thời gian tương đối dài mới có thể bắt đầu tạo ra doanh thu thực tế, và hầu hết mọi người đều sẽ bỏ cuộc trước khi đạt được cột mốc đó.

-- *Trích bài chia sẻ 《Bàn về hoạt động phát triển độc lập (Indie App)》*

2、

Khi bắt đầu triển khai một dự án mới, sự ngây thơ ở một mức độ nhất định luôn là yếu tố thiết yếu. Nếu ngay từ đầu tôi đã biết rõ con đường phía trước sẽ gian nan và thử thách đến nhường nào, tôi nhiều khả năng sẽ không bao giờ có đủ dũng khí để bắt đầu. Nhưng chính nhờ sự ngây thơ hoàn toàn không biết gì về những khó khăn tương lai, tôi đã dũng cảm dấn thân và tự mày mò tìm kiếm lối đi trong suốt hành trình.

-- *Gints Zilbalodis, đạo diễn người Latvia chia sẻ* (Tác phẩm 《Flow》 của ông đã vinh dự nhận giải Phim hoạt hình xuất sắc nhất tại lễ trao giải Oscar năm nay)

3、

Mỗi một dòng code bạn viết ra đều ẩn chứa nguy cơ phát sinh lỗi (bug) tiềm ẩn. Trừ khi dòng code đó là thực sự bắt buộc và việc thiếu nó sẽ trực tiếp ảnh hưởng đến sự vận hành của chương trình, nếu không thì tốt nhất là bạn đừng viết nó. Tuyệt đối không tự ý xây dựng thêm các tầng trừu tượng hóa khi chưa có nhu cầu thực tế. Nếu việc tối ưu hóa hiệu năng làm tăng độ phức tạp của hệ thống lên, hãy kiên quyết từ bỏ việc tối ưu hóa đó.

-- *Trích bài phân tích 《Mỗi dòng code đều có thể là một lỗi tiềm ẩn》*

4、

Quan điểm của tôi đối với công cụ AI là bản thân nó hoàn toàn không có khả năng tự sáng tạo độc lập, nó đòi hỏi sự cộng tác sáng tạo của con người. Chất lượng kết quả đầu ra tốt hay xấu phụ thuộc trực tiếp vào năng lực tư duy của chính người sử dụng công cụ.

Việc tương tác trò chuyện với AI không giống như việc trò chuyện với một cá nhân cụ thể, mà tương tự như việc bạn đang đối thoại với trí tuệ tập thể của toàn nhân loại. Việc ứng dụng AI hoàn toàn không nhằm mục đích giúp bạn lười suy nghĩ đi, mà là công cụ đắc lực hỗ trợ bạn mở rộng và đào sâu tư duy của mình hơn. AI chính là đòn bẩy giúp bạn bứt phá các giới hạn của bản thân.

-- *Alex Komoroske, lập trình viên người Mỹ chia sẻ*

5、

Một cuộc họp quy mô 10 người hoàn toàn có thể vận hành tốt mà không cần người chủ trì. Một cuộc họp 100 người bắt buộc phải có người chủ trì điều phối. Nhưng một hội nghị quy mô 1.000 người sẽ đòi hỏi sự ra đời của cả một ban tổ chức chuyên nghiệp.

Để mở rộng quy mô lên gấp 10 lần, bạn chỉ cần đẩy các tài nguyên hiện có lên mức giới hạn tối đa. Nhưng để mở rộng quy mô lên gấp 100 lần, bạn bắt buộc phải thoát khỏi hệ tư duy cũ để tái thiết kế và sắp xếp lại toàn bộ hệ thống từ con số không.

-- *Trích bài phân tích 《Hai chữ số 0 tiếp theo của cuộc đời bạn》*

## 往年回顾

- Số #293: [Thảo luận về luận điểm: Một tuần làm việc thực chất chỉ chiếm 2% quỹ thời gian của một năm](https://www.ruanyifeng.com/blog/2024/03/weekly-issue-293.html)
- Số #243: [Trải nghiệm trò chuyện trực tuyến thú vị cùng mô hình AI mô phỏng Khổng Tử](https://www.ruanyifeng.com/blog/2023/02/weekly-issue-243.html)
- Số #193: [Thảo luận về bài toán: Giữa lập trình Frontend và Backend, mảng nào khó hơn?](https://www.ruanyifeng.com/blog/2022/01/weekly-issue-193.html)
- Số #143: [Giới thiệu tác phẩm văn học 《Xứ sở diệu kỳ tàn bạo và chốn tận cùng thế giới》 của Haruki Murakami](https://www.ruanyifeng.com/blog/2021/01/weekly-issue-143.html)

(Hết)
