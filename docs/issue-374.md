# Bản tin chia sẻ công nghệ (Số 374): Rắc rối của băng tần 6GHz

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/8003) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111209.webp)

Khu vui chơi giải trí và thể thao dưới nước mới khánh thành tại vịnh Loan Tử, Hồng Kông. Đây là đoạn bờ kè đầu tiên tại cảng Victoria được thiết kế không có hàng rào chắn, cho phép người dân và du khách tự do tản bộ xuống các bậc thềm sát mép nước. ([via](https://www.hfc.org.hk/tc/hss/water-sports-and-recreation-precinct-wan-chai))

## 6GHz 的问题

Theo [tin tức](https://www.lightreading.com/wifi/mobile-operators-beat-wi-fi-for-upper-6ghz-in-europe) tuần này, Liên minh châu Âu đã chính thức đưa ra quyết định về phương án phân bổ băng tần 6GHz.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111502.webp)

Châu Âu quyết định chia đôi băng tần 6GHz: phần tần số thấp hơn cấp cho WiFi sử dụng, phần tần số cao hơn dành riêng cho thông tin di động.

Phương án này hoàn toàn khác biệt so với Mỹ và Trung Quốc. Trong khi Mỹ cấp toàn bộ băng tần 6GHz cho WiFi, thì Trung Quốc lại phân bổ toàn bộ cho thông tin di động.

Dưới đây là một vài suy nghĩ và phân tích của tôi về sự kiện này.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111503.webp)

Để các bạn dễ hình dung, tôi xin giải thích ngắn gọn băng tần 6GHz là gì.

Mạng không dây gia đình (WiFi) bắt buộc phải sử dụng các tín hiệu tần số cố định. Tần số sơ khai nhất là 2.4GHz. Việc mọi thiết bị không dây đều truy cập vào tần số này đã dẫn đến tình trạng nghẽn mạng và tín hiệu kém ổn định.

Về sau, tần số 5GHz được bổ sung. Tuy nhiên, tần số này hiện tại cũng bắt đầu rơi vào tình trạng quá tải. Tại các căn hộ chung cư cao tầng ở các đô thị lớn, khi mở điện thoại lên bạn có thể dò quét thấy hàng chục mạng WiFi xung quanh. Việc quá nhiều thiết bị cùng chen chúc truyền dữ liệu trên tần số 5GHz khiến kết nối mạng bị chậm và nghẽn.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111504.webp)

Do đó, người ta nghĩ đến việc cấp thêm một băng tần mới cho WiFi, và đích ngắm chính là băng tần 6GHz – dải tần số vốn chưa được quy hoạch cho bất kỳ mục đích sử dụng cụ thể nào trước đó.

Nếu băng tần 6GHz được cấp cho WiFi, lợi ích lớn nhất mang lại là hiện tượng nghẽn mạng sẽ hoàn toàn biến mất. Do có bước sóng ngắn, khả năng xuyên tường của sóng 6GHz cực kỳ kém và hầu như không thể xuyên qua các bức tường bê tông. Điều này đồng nghĩa với việc khi ở trong nhà, bạn chỉ kết nối được với sóng 6GHz từ bộ định tuyến của chính mình, các nguồn sóng nhiễu từ nhà hàng xóm xung quanh không thể lọt vào được.

Đồng thời, băng tần này sở hữu băng thông cực kỳ rộng lớn cho tốc độ truyền tải siêu tốc, tạo điều kiện xây dựng hệ thống WiFi tốc độ cao đáp ứng tốt cho các thiết bị ngốn băng thông lớn như kính thực tế ảo VR.

Thế nhưng, rắc rối phát sinh khi băng tần 6GHz bên cạnh việc cấp cho WiFi còn có thể quy hoạch phục vụ cho thông tin di động (sóng điện thoại di động). Băng tần di động hỗ trợ kết nối đồng thời cho số lượng người dùng lớn hơn rất nhiều so với WiFi vốn chỉ phục vụ quy mô hộ gia đình, do đó mang lại hiệu suất khai thác băng tần cao hơn và lợi ích công cộng lớn hơn.

Như đã đề cập ở trên, quyết định của Trung Quốc là dành toàn bộ băng tần 6GHz cho thông tin di động, đồng nghĩa với việc thiết bị WiFi tại nước này không được phép sử dụng dải tần số này.

Vì vậy, một số người dùng đam mê công nghệ tốc độ cao trong nước thường tìm mua các bộ định tuyến không dây xách tay từ nước ngoài, đi kèm các thiết bị phần cứng hỗ trợ sóng 6GHz (như [các dòng thiết bị của Apple](https://support.apple.com/zh-cn/102285)) để tự thiết lập mạng WiFi tốc độ cao trong gia đình.

Quan điểm của tôi là hệ thống WiFi hiện nay nếu chỉ dừng lại ở hai băng tần 2.4GHz và 5GHz thì thực sự chưa đủ đáp ứng nhu cầu. Việc bổ sung thêm một dải tần số tốc độ cao là vô cùng cần thiết, vừa đáp ứng nhu cầu truyền tải dữ liệu băng thông lớn, vừa thúc đẩy chu kỳ nâng cấp thiết bị và kích cầu tiêu dùng công nghệ.

Dải tần số đầy đủ của 6GHz kéo dài từ 5925MHz đến 7125MHz. Được biết dải tần số mà Trung Quốc phân bổ rõ ràng cho mạng di động là đoạn từ 6425MHz đến 7125MHz, còn phương án phân bổ cho đoạn tần số từ 5925MHz đến 6425MHz còn lại hiện vẫn chưa có quy định văn bản chính thức (theo nguồn tin Bách khoa Baidu).

Nếu thông tin này là chính xác, thiết nghĩ các cơ quan quản lý có thể cân nhắc mở cửa dải tần số từ 5925MHz đến 6425MHz cho WiFi sử dụng tự do mà không cần xin phép, tương tự như chính sách của Mỹ. Giải pháp này sẽ giúp người dân và doanh nghiệp sở hữu thêm một dải tần số kết nối tốc độ cao miễn phí, tạo bệ phóng thúc đẩy nhiều giải pháp công nghệ sáng tạo đột phá ra đời.

## 科技动态

1. **Một ngày ánh sáng**

Vào ngày 5 tháng 9 năm 1977, Mỹ đã phóng tàu vũ trụ Voyager 1. Đây hiện là thiết bị nhân tạo bay xa nhất của loài người và đã chính thức rời khỏi hệ Mặt Trời.

Theo các phép tính toán học, vào ngày 13 tháng 11 năm 2026, Voyager 1 sẽ đạt khoảng cách đúng "1 ngày ánh sáng" (quãng đường ánh sáng di chuyển trong vòng 1 ngày) so với Trái Đất, trở thành thiết bị nhân tạo đầu tiên chạm tới cột mốc vĩ đại này.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111303.webp)

Vào thời điểm đó, Voyager 1 sẽ cách Trái Đất khoảng 25,9 tỷ km. Khoảng cách này ánh sáng chỉ mất đúng 1 ngày để đi hết, nhưng con tàu vũ trụ đã phải mất tới gần 50 năm ròng rã di chuyển.

Ở vị trí hiện tại, các lệnh truyền từ Trái Đất mất tới 23 giờ 29 phút 27 giây để đến được con tàu, và khi vượt qua mốc 1 ngày ánh sáng, phải sang ngày hôm sau con tàu mới nhận được lệnh hồi đáp.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111304.webp)

Các nhà khoa học dự báo phải mất thêm 300 năm nữa Voyager 1 mới tiếp cận đám mây Oort ở rìa hệ Mặt Trời, và sẽ cần khoảng 30.000 năm để bay xuyên qua đám mây bụi khổng lồ này.

2. **Tháp truyền tải điện**

Nước Áo đang tiến hành cải tạo các tháp truyền tải điện cao thế để biến chúng thành những công trình mang tính thẩm mỹ cao, hòa mình vào cảnh quan thiên nhiên.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110204.webp)

Hình ảnh trên là tháp hình chú chim cò, và một thiết kế tháp hình chú nai sừng tấm khác vừa được khánh thành (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110205.webp)

Công ty lưới điện Áo dự kiến sẽ thiết kế tổng cộng 9 mô hình tháp điện mang hình dáng các loài động vật khác nhau, tượng trưng cho 9 bang của nước Áo, hiện tại đã hoàn thành 2 mô hình đầu tiên.

Nhiều người dân thường phản đối việc xây dựng các cột điện cao thế ngay cạnh khu dân cư của họ. Công ty lưới điện hy vọng việc biến các tháp điện thành các tác phẩm nghệ thuật trực quan sinh động sẽ giúp người dân dễ dàng chấp nhận sự hiện diện của chúng hơn.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110206.webp)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110207.webp)

3. **Tính năng trang điểm bằng AI khi họp trực tuyến**

Google Meet vừa bổ sung tính năng hỗ trợ người dùng "trang điểm ảo" ngay trong phòng họp trực tuyến.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101410.webp)

Hình ảnh bên phải cung cấp 12 phong cách trang điểm khác nhau để người dùng lựa chọn, khung hình bên trái là màn hình xem trước (preview) – hiển thị diện mạo lung linh mà mọi người trong cuộc họp sẽ nhìn thấy ở bạn. Tính năng trang điểm kỹ thuật số này đảm bảo giúp bạn luôn xuất hiện với vẻ ngoài rạng rỡ nhất.

Dự báo trong tương lai gần, các bộ lọc làm đẹp (beauty filters) sẽ trở thành tính năng tiêu chuẩn bắt buộc phải có trên mọi phần mềm gọi video.

4. **Máy ảnh móc khóa**

Kodak vừa cho mắt dòng sản phẩm máy ảnh mini siêu nhỏ được thiết kế làm móc khóa với diện mạo vô cùng hoài cổ.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091802.webp)

Chiếc máy ảnh có kích thước cực kỳ nhỏ gọn và trọng lượng chỉ nhẹ vỏn vẹn 30 gram, nhưng được trang bị đầy đủ các tính năng cơ bản như ống ngắm (viewfinder), màn hình hiển thị LCD, cổng kết nối Type-C, đèn flash, khe cắm thẻ nhớ microSD.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091803.webp)

Chất lượng ảnh chụp của máy ở mức khá khiêm tốn do chỉ sử dụng cảm biến kích thước 1/4 inch, xuất ra tệp ảnh định dạng JPEG độ phân giải 1440 x 1440 pixel.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091804.webp)

Tuy nhiên, nhờ mức giá cực rẻ chỉ 30 USD đi kèm diện mạo hoài cổ vô cùng độc đáo, sản phẩm nhận được sự chào đón rất lớn của thị trường. Hiện tại sản phẩm đăng bán trên trang chủ của Kodak luôn trong tình trạng cháy hàng.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091805.webp)

## 文章

1. [Các mô hình AI của Trung Quốc chỉ là "hổ giấy"?](https://www.gleech.org/paper) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111801.webp)

Bài viết của một tác giả người Mỹ đưa ra những nhận định chỉ trích rằng năng lực thực tế của các mô hình AI lớn do Trung Quốc phát triển không mạnh mẽ như những gì họ đang quảng bá.

Quan điểm cá nhân của tôi là bài viết này có phần thiên lệch, nhiều luận điểm đưa ra thiếu tính thuyết phục vững chắc và giọng văn có phần đố kỵ, tuy nhiên đây vẫn là một góc nhìn để chúng ta tham khảo.

2. [Ứng dụng WhatsApp trên Windows chính thức chuyển sang chạy WebView](https://www.windowslatest.com/2025/11/12/meta-just-killed-native-whatsapp-on-windows-11-now-it-opens-webview-uses-1gb-ram-all-the-time/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111309.webp)

Phiên bản WhatsApp chạy trên hệ điều hành Windows trước nay vốn là một ứng dụng máy tính dạng Native (ứng dụng gốc viết riêng cho nền tảng).

Tác giả bài viết đã vô cùng bất ngờ khi phát hiện ra bản cập nhật mới nhất của ứng dụng thực chất đã bị hạ cấp xuống dạng chạy WebView (chạy trên nhân trình duyệt web). Sự thay đổi này khiến hiệu năng ứng dụng sụt giảm nghiêm trọng và liên tục ngốn tới hơn 1GB dung lượng bộ nhớ RAM của hệ thống. Nguyên nhân sâu xa được cho là do tập đoàn Meta đã tiến hành cắt giảm toàn bộ đội ngũ kỹ sư phụ trách phát triển phiên bản Windows Native trước đó.

3. [Đánh giá thực tế về hình thức phỏng vấn lập trình bằng AI (Vibe Coding Interview)](https://mp.weixin.qq.com/s/roURrNNBJ2J5ZqdFuU1tkA) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112003.webp)

Bài viết chia sẻ từ một trưởng nhóm phát triển phần mềm về việc áp dụng hình thức phỏng vấn mới: yêu cầu ứng viên trực tiếp sử dụng các công cụ AI để hoàn thành một tính năng lập trình thực tế, đi kèm những cảm nhận và đánh giá chi tiết về hiệu quả của phương pháp này. (Đóng góp từ [@thuwyh](https://github.com/ruanyf/weekly/issues/8254))

4. [Hướng dẫn các phương pháp chạy mô hình AI trực tiếp trên máy tính cá nhân](https://decrypt.co/348129/running-your-own-local-open-source-ai-model-easy-heres-how) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111808.webp)

Bài viết giới thiệu và hướng dẫn chi tiết một số giải pháp giúp người dùng dễ dàng cài đặt và chạy các mô hình AI mã nguồn mở ngay trên máy tính của mình thông qua các công cụ như [LM Studio](https://lmstudio.ai/) hay [Ollama](https://ollama.com/).

5. [Chúng tôi sử dụng trình soạn thảo Zed làm văn phòng làm việc chung](https://zed.dev/blog/zed-is-our-office) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111402.webp)

Zed là một trình soạn thảo mã nguồn thế hệ mới đang được phát triển tích cực. Bên cạnh tính năng viết code thông thường, đội ngũ kỹ sư của Zed còn tận dụng chính công cụ này để tổ chức họp hành và trao đổi công việc hàng ngày nhờ tích hợp sẵn tính năng kênh thảo luận nội bộ và cộng tác viết code thời gian thực.

6. [Các cột mốc định nghĩa một lập trình viên cấp trung (Intermediate Developer)](https://dawranliou.com/blog/intermediate-dev/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111308.webp)

Đánh dấu cột mốc 10 năm hoạt động trong ngành lập trình chuyên nghiệp, tác giả tự định vị bản thân ở cấp độ lập trình viên trung cấp và tổng hợp lại những bài học kinh nghiệm, nội dung công việc thực tế của mình.

Anh chia sẻ nếu bạn có khả năng xử lý tốt các nhóm công việc được liệt kê trong bài viết, bạn đã hoàn toàn đạt chuẩn của một lập trình viên cấp trung.

## 工具

1. [LibrePods](https://github.com/kavishdevar/librepods)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111806.webp)

Công cụ hỗ trợ quản lý và sử dụng tai nghe AirPods của Apple trên các thiết bị không thuộc hệ sinh thái Apple (chẳng hạn như chạy hệ điều hành Android hay Linux).

2. [IDEmacs](https://codeberg.org/IDEmacs/IDEmacs)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111807.webp)

Bộ cấu hình (config) giúp biến đổi trình soạn thảo cổ điển Emacs sở hữu giao diện và các tính năng tương tự như VS Code.

3. [Kratos](https://github.com/ory/kratos)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111310.webp)

Máy chủ quản lý danh tính và xác thực mã nguồn mở, hỗ trợ nhiều hình thức xác thực bảo mật khác nhau, được định vị là giải pháp thay thế tự lưu trữ cho Auth0 và Okta.

4. [Biu](https://github.com/wood3n/biu)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111307.webp)

Ứng dụng máy tính mã nguồn mở đa nền tảng, hỗ trợ tìm kiếm và phát nhạc trực tiếp từ nền tảng Bilibili thông qua API, hỗ trợ đăng nhập tài khoản để đồng bộ hóa danh sách nhạc yêu thích. (Đóng góp từ [@wood3n](https://github.com/ruanyf/weekly/issues/8202))

5. [Enjoy Git](https://enjoygit.com/)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111401.webp)

Ứng dụng quản trị Git bằng giao diện đồ họa (GUI client) hỗ trợ tiếng Trung, hiện tại mới chỉ phát hành phiên bản dành cho hệ điều hành Windows. (Đóng góp từ [@huangcs427](https://github.com/ruanyf/weekly/issues/8207))

6. [Readdig](https://github.com/readdig/readdig)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111705.webp)

Trang web mã nguồn mở hỗ trợ đọc tin tức RSS và nghe các chương trình âm thanh Podcasts trực tuyến trên một giao diện thống nhất. (Đóng góp từ [@copilot-is](https://github.com/ruanyf/weekly/issues/8223))

7. [Tiny SVG](https://github.com/hehehai/tiny-svg)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111706.webp)

Công cụ trực tuyến mã nguồn mở hỗ trợ tối ưu hóa và nén dung lượng các tệp đồ họa vector SVG. [Trang chạy thử trực tuyến](https://tiny-svg.actnow.dev/). (Đóng góp từ [@mutou981](https://github.com/ruanyf/weekly/issues/8225))

8. [fssh](https://github.com/Mister-leo/fssh)

Công cụ hỗ trợ quản lý khóa bảo mật SSH cá nhân dành cho máy tính MacBook, cho phép xác thực vân tay Touch ID trực tiếp khi thực hiện kết nối máy chủ từ xa. (Đóng góp từ [@Mister-leo](https://github.com/ruanyf/weekly/issues/8226))

9. [CrossDesk](https://www.crossdesk.cn/)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112001.webp)

Phần mềm điều khiển máy tính từ xa mã nguồn mở đa nền tảng, hỗ trợ tăng tốc phần cứng và truy cập điều khiển trực tiếp trên trình duyệt web. (Đóng góp từ [@kunkundi](https://github.com/ruanyf/weekly/issues/8251))

10. [Git PR AI](https://github.com/leochiu-a/git-pr-ai)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112002.webp)

Công cụ dòng lệnh hỗ trợ kết nối trực tiếp với hệ thống quản lý công việc JIRA để tự động tạo nhánh Git từ thông tin JIRA Ticket tích hợp các tính năng tự động hóa bằng AI. (Đóng góp từ [@leochiu-a](https://github.com/ruanyf/weekly/issues/8252))

## AI 相关

1. [Antigravity](https://antigravity.google)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111901.webp)

Môi trường phát triển tích hợp (IDE) chuyên dụng hỗ trợ lập trình bằng AI do Google phát hành tuần này, được xây dựng dựa trên nền tảng của VS Code.

2. [Code Wiki](https://codewiki.google/)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111805.webp)

Dịch vụ mới do Google giới thiệu sử dụng sức mạnh của mô hình Gemini để tự động quét và sinh tài liệu giải thích chi tiết cho toàn bộ kho lưu trữ mã nguồn của bạn.

3. [Open CoreUI](https://github.com/xxnuo/open-coreui)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111704.webp)

Dự án viết lại giao diện Open WebUI bằng ngôn ngữ Rust giúp tối ưu hóa hiệu năng, giảm thiểu đáng kể tài nguyên CPU và bộ nhớ RAM tiêu thụ, phát hành đầy đủ phiên bản chạy trên máy chủ và ứng dụng máy tính. (Đóng góp từ [@xxnuo](https://github.com/ruanyf/weekly/issues/8222))

4. [Continuous Claude](https://github.com/AnandChowdhary/continuous-claude)

Công cụ dòng lệnh hỗ trợ tự động chạy lặp đi lặp lại công cụ lập trình Claude Code cho cùng một tác vụ được chỉ định trước với số lần lặp tùy cấu hình của người dùng.

## 资源

1. [Hướng dẫn kiểm tra tính ngẫu nhiên (random.tastemaker.design)](https://random.tastemaker.design/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111311.webp)

Trang web giới thiệu hàng loạt phương pháp giúp kiểm tra xem một bộ sinh số ngẫu nhiên có thực sự đạt độ ngẫu nhiên chuẩn xác hay không. Các phương pháp kiểm thử đều đi kèm lời giải thích khoa học dễ hiểu, tài liệu tham khảo tốt để học bộ môn thống kê.

2. [Cơ sở toán học của học tăng cường](https://github.com/MathFoundationRL/Book-Mathematical-Foundation-of-Reinforcement-Learning) (tiếng Anh)

Sách điện tử mã nguồn mở cung cấp các kiến thức toán học nền tảng phục vụ cho việc nghiên cứu và phát triển các thuật toán học tăng cường (Reinforcement Learning) trong AI.

3. [Tài liệu học ngôn ngữ Erlang dành cho người mới bắt đầu](https://learnyousomeerlang.com/content) (tiếng Anh)

Erlang là ngôn ngữ lập trình hàm (functional language) đặc biệt mạnh mẽ khi xây dựng các hệ thống phân tán yêu cầu tính sẵn sàng cao. Trang web cung cấp khóa học hướng dẫn trực quan dành riêng cho người mới tiếp cận ngôn ngữ này.

## 图片

1. Một tờ báo của Pakistan đã vô tình in kèm cả đoạn hội thoại hướng dẫn của họ với trợ lý AI ngay dưới bài viết được xuất bản trên báo giấy.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111214.webp)

Trong khung đỏ ở cuối bài viết có dòng chữ: "Nếu bạn muốn, tôi cũng có thể tạo ra một phiên bản mang phong cách 'Trang nhất' lôi cuốn hơn nữa, đi kèm số liệu thống kê một dòng cô đọng và bố cục dạng infographic trực quan – cực kỳ phù hợp để thu hút tối đa độc giả. Bạn có muốn tôi tạo tiếp bản đó không?" (If you want, I can also create an even snappier “front-page style” version with punchy one-line stats and a bold, infographic-ready layout — perfect for maximum reader impact. Do you want me to do that next?)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112004.webp)

Nếu các cơ quan báo chí đều chuyển sang sử dụng AI để viết bài hoàn toàn, liệu độc giả có còn lý do để chi tiền mua báo nữa hay không?

2. **Dải hố đất kỳ bí tại dãy núi Andes**

Tại một thung lũng ở miền nam Peru tồn tại một dải hố đất kéo dài xếp hàng ngay ngắn với hơn 5.000 hố sâu kỳ bí.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111903.webp)

Công trình này rõ ràng là sản phẩm nhân tạo, tuy nhiên lịch sử địa phương hoàn toàn không có bất kỳ ghi chép nào về việc ai đã đào chúng và dùng để làm gì.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111904.webp)

Vệt màu xám chạy dọc sườn núi ở bức ảnh trên chính là dải hố đất kéo dài.

Các nhà khảo cổ học khi tiến hành khai quật lòng hố đã phát hiện ra dấu vết phấn hoa ngô cùng nhiều sợi cỏ sậy. Ngô là nguồn lương thực chính của khu vực này thời cổ đại, còn cỏ sậy thường dùng để đan lát giỏ chứa.

Do đó, người ta đưa ra giả thuyết rằng vị trí này từng là một khu chợ giao thương tập trung quy mô lớn của Đế chế Inca cổ đại, và các hố đất sâu đóng vai trò như các ô chứa và bảo quản hàng hóa cho thương nhân.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025111905.webp)

## 文摘

1. [Cửa hàng ứng dụng (App Store) đầu tiên trên thế giới](https://one-from-nippon.ghost.io/worlds-first-app-store/)

Cửa hàng ứng dụng đầu tiên trên thế giới xuất hiện tại Nhật Bản vào những năm 1980 để giúp người dùng mua bản quyền phần mềm máy tính.

Nó được thiết kế dưới hình dạng một chiếc máy bán hàng tự động, và cũng được ghi nhận là chiếc máy bán hàng tự động phân phối phần mềm kỹ thuật số đầu tiên trong lịch sử nhân loại.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110403.webp)

Vào năm 1986, phần mềm máy tính hầu hết được phân phối và bán thông qua đĩa mềm. Dung lượng của một ứng dụng thời kỳ đó thường chỉ nặng vài trăm KB, vừa vặn lưu trữ trong một chiếc đĩa mềm duy nhất.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110501.webp)

Góc dưới bên trái hình trên là hình ảnh đĩa mềm thời kỳ đó.

Mỗi khi cần cài đặt phần mềm mới, người dùng có xu hướng xóa sạch dữ liệu cũ trong đĩa mềm mang đi sao chép. Một công ty Nhật Bản đã nảy ra ý tưởng chế tạo một chiếc máy tự động cho phép người dùng đút đĩa mềm vào đầu đọc để sao chép phần mềm họ lựa chọn trực tiếp tại chỗ.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110502.webp)

Bức ảnh trên mô tả chiếc máy bán phần mềm tự động độc đáo đó.

Người dùng chỉ cần đưa đĩa mềm của mình vào máy, sử dụng màn hình để lựa chọn phần mềm muốn mua, tiến hành thanh toán tiền và hệ thống sẽ tự động ghi dữ liệu phần mềm vào đĩa mềm cho bạn mang về nhà sử dụng.

Nếu phần mềm đi kèm tài liệu hướng dẫn sử dụng, chiếc máy cũng sẽ tự động in tài liệu ra giấy cho bạn.

Đây được coi là phát minh mang tính cách mạng thời bấy giờ và nhanh chóng tạo nên cơn sốt trên thị trường. Khi mạng Internet còn chưa xuất hiện, việc mua phần mềm bắt buộc phải tìm đến các cửa hàng chuyên doanh lớn, sự ra đời của chiếc máy này giúp người dùng dễ dàng mua phần mềm ngay tại các góc phố.

Tuy nhiên điểm hạn chế chí mạng của hệ thống nằm ở dung lượng ổ cứng bên trong máy rất giới hạn, chỉ đủ chứa một số phần mềm phổ biến nhất (chủ yếu là trò chơi điện tử). Nếu khách hàng muốn tìm mua các phần mềm ít phổ biến hơn, chiếc máy buộc phải thực hiện tải xuống từ xa thông qua kết nối mạng.

Thời kỳ đó sử dụng kết nối quay số qua đường dây điện thoại với tốc độ truyền tải cực kỳ chậm chỉ khoảng 1.2 KB/s, khiến thời gian tải xuống một tựa game đôi khi kéo dài tới 20 phút. Trong khoảng thời gian này, khách hàng buộc phải đứng chờ cạnh máy và không ai khác có thể sử dụng hệ thống. Nếu đường truyền mạng bất ngờ bị đứt giữa chừng, quá trình tải xuống sẽ phải thực hiện lại từ đầu.

Để khắc phục điểm yếu này, công ty đã lập trình cho máy tự động chạy tải xuống các tựa game mới nhất vào ban đêm. Tuy nhiên, giải pháp vẫn không thể giải quyết triệt để sự chờ đợi của khách hàng.

Vào thời kỳ hoàng kim nhất, hệ thống máy tự động này đã được lắp đặt rộng khắp trên toàn nước Nhật với hơn 300 máy hoạt động, trước khi chính thức rút khỏi thị trường vào năm 1997.

## 言论

1.

Tôi muốn hướng tới việc để robot Optimus trực tiếp ngồi trong các xe taxi tự lái Waymo để đi giao hàng cho khách.

Sau khi taxi tự lái di chuyển tới đúng địa chỉ giao hàng, robot sẽ chịu trách nhiệm bốc dỡ và mang kiện hàng đặt trước cửa nhà khách hàng.

-- [Elon Musk](https://stratechery.com/2025/robotaxis-and-suburbia/) chia sẻ về tầm nhìn phát triển dòng robot nhân hình Optimus của Tesla

2.

Một hình thức lừa đảo qua mạng cực kỳ phổ biến tại châu Á hiện nay là kẻ gian gọi điện trực tiếp cho nạn nhân, mạo danh nhân viên ngân hàng để cảnh báo tài khoản của họ đang gặp rủi ro bảo mật và hướng dẫn họ cài đặt một ứng dụng bảo vệ tài khoản.

Kẻ lừa đảo sẽ dẫn dụ nạn nhân bỏ qua mọi cảnh báo an ninh hiển thị trong quá trình cài đặt ứng dụng. Ứng dụng này thực chất là một mã độc được ngụy trang dưới vỏ bọc phần mềm hợp pháp, có khả năng đánh cắp thông tin đăng nhập và chặn các mã xác thực hai lớp (OTP) gửi về máy điện thoại của nạn nhân để chiếm đoạt tài khoản ngân hàng.

-- [Google](https://www.engadget.com/apps/google-will-allow-experienced-users-to-sideload-unverified-android-apps-130000130.html) chia sẻ ví dụ thực tế giải thích tầm quan trọng của việc triển khai "Chương trình chứng nhận nhà phát triển Android"

3.

Một khi trợ lý AI có khả năng tự viết ra các đoạn code thực thi chính xác tính năng bạn yêu cầu trong nháy mắt, liệu bạn có cần phải gánh chịu rủi ro bảo mật chuỗi cung ứng bằng việc nhập thêm các thư viện dependency bên thứ ba vào dự án nữa không?

Do đó các thư viện dependency quy mô nhỏ và ít giá trị sẽ dần biến mất trong tương lai gần.

-- [《Số phận của các phần mềm nguồn mở quy mô nhỏ》](https://simonwillison.net/2025/Nov/17/the-fate-of-small-open-source/)

4.

Liệu pháp gen có thể giúp chữa khỏi hoàn toàn bệnh tật cho bệnh nhân chỉ sau một lần điều trị duy nhất, điều này thực tế lại là một tin xấu đối với việc duy trì nguồn doanh thu ổn định lâu dài cho các hãng dược phẩm.

So với việc duy trì các liệu trình điều trị bệnh mãn tính kéo dài liên tục, liệu việc chữa khỏi hoàn toàn bệnh cho bệnh nhân có được coi là một mô hình kinh doanh bền vững cho doanh nghiệp hay không?

-- Báo cáo nghiên cứu kinh tế của tập đoàn tài chính [Goldman Sachs](https://www.cnbc.com/2018/04/11/goldman-asks-is-curing-patients-a-sustainable-business-model.html)

5.

Năm ngoái đánh dấu cột mốc lần đầu tiên trong lịch sử Internet ghi nhận lượng lưu lượng truy cập từ bot tự động vượt qua lượng truy cập từ con người. Một báo cáo chỉ ra rằng các hệ thống bot tự động chiếm tới 51% tổng lưu lượng web năm 2024, và số lượng các bài viết do AI tự động tạo lập trên mạng cũng chính thức vượt mốc bài viết do con người tự viết vào cuối năm 2024.

-- [《Thuyết Internet đã chết (Dead Internet Theory)》](https://decrypt.co/348837/dead-internet-theory-gains-traction-ai-content-surges-online)

## 往年回顾

[Internet không có liên kết](https://www.ruanyifeng.com/blog/2024/11/weekly-issue-327.html) (#327)

[Lựa chọn màn hình phụ tối ưu cho góc làm việc](https://www.ruanyifeng.com/blog/2023/11/weekly-issue-277.html) (#277)

[Chương trình đào tạo nhân sự mới của Facebook](https://www.ruanyifeng.com/blog/2022/10/weekly-issue-227.html) (#227)

[Công dụng thực sự của máy tính bảng iPad](https://www.ruanyifeng.com/blog/2021/09/weekly-issue-177.html) (#177)

(Hết)
