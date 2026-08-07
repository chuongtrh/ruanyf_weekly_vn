# 科技爱好者周刊（第 185 期）：美国宪法拍卖，一个区块链案例

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2032) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112501.jpg)

Tại triển lãm thế giới Expo Dubai đang diễn ra, hàng ngày đều có 4 buổi biểu diễn "độc tấu dương cầm trên không". Cả người nghệ sĩ và cây đàn piano đều được treo lơ lửng giữa không trung tạo nên trải nghiệm thưởng thức âm nhạc vô cùng kỳ ảo. (Nguồn: [Expo Dubai Instagram](https://www.instagram.com/p/CWoB7c3PUPu/))

## 主带话题：Đấu giá Hiến pháp Mỹ - Bài học thực tế đột phá của Web3 và Blockchain

Thứ Năm tuần trước (18/11), tại New York đã diễn ra một phiên đấu giá đặc biệt: bán đấu giá bản in đầu tiên cực hiếm của Hiến pháp Hoa Kỳ. Vụ việc thu hút sự quan tâm lớn của thế giới công nghệ do sự can thiệp của một dự án blockchain.

Hơn 200 năm trước, sau khi chiến thắng trong cuộc chiến giành độc lập, đại diện của 13 thuộc địa đã họp để soạn thảo bản Hiến pháp lập quốc.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112118.jpg)

Khi được thông qua, hiến pháp đã được in 500 bản để các đại diện mang về các bang. Hiện nay chỉ còn 13 bản lưu giữ được, và chỉ duy nhất 1 bản thuộc sở hữu tư nhân, chính là bản được mang ra đấu giá lần này.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112119.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112121.jpg)

Một nhóm những người đam mê blockchain khi tán gẫu trên mạng đã nảy ra ý tưởng táo bạo: "Hãy cùng nhau góp tiền để đấu thầu và sở hữu cổ vật này!".

Ý tưởng nhanh chóng được hiện thực hóa thông qua việc thành lập một tổ chức tự trị phi tập trung trên mạng lưới blockchain gọi là **ConstitutionDAO** (DAO Hiến pháp).

Họ đăng ký tên miền [ConstitutionDAO.com](https://www.constitutiondao.com/) với giao diện tối giản để giải thích mục tiêu của chiến dịch:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112122.jpg)

Điểm mấu chốt là làm sao thu thập tiền từ hàng nghìn người lạ trên mạng một cách an toàn và minh bạch?

Thật bất ngờ, việc này trở nên rất dễ dàng nhờ các công cụ blockchain có sẵn:

- **Juicebox:** Nền tảng gây quỹ trực tuyến trên blockchain. Nó ghi các điều khoản hợp đồng thông minh của dự án trực tiếp lên blockchain, cung cấp ví nhận tiền. Những người gửi tiền sẽ nhận lại token đại diện của dự án làm minh chứng đóng góp.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112502.webp)

- **Gnosis Safe:** "Két sắt đa chữ ký" (Multisig) bảo mật trên blockchain. Tiền sau khi chuyển vào đây sẽ không thể bị rút ra bởi một cá nhân đơn lẻ. Để rút tiền, hệ thống yêu cầu sự đồng thuận kỹ thuật số của một nhóm quản trị (ví dụ: tối thiểu 5 trên 10 quản trị viên phải ký duyệt). Việc này giúp ngăn chặn hoàn toàn rủi ro người sáng lập ôm tiền biến mất.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112503.webp)

Kết quả gây quỹ thật kinh ngạc:

Mục tiêu ban đầu là 20 triệu USD, sau đó nâng lên 35 triệu USD. Vào thời điểm phiên đấu giá bắt đầu, họ đã huy động được tổng cộng 11.601 Ethereum (tương đương khoảng 47 triệu USD tại thời điểm đó) từ hàng vạn người đóng góp ẩn danh khắp thế giới.

Trong phiên đấu giá nghẹt thở, ConstitutionDAO đã cạnh tranh trực tiếp với một tỷ phú truyền thống. Khi mức giá chạm mốc 40 triệu USD, nhóm DAO quyết định dừng lại để bảo đảm số tiền còn lại đủ trang trải cho các chi phí bảo quản và vận chuyển cổ vật sau khi thắng thầu.

Cuối cùng, bản Hiến pháp đã thuộc về vị tỷ phú với giá gõ búa là 43 triệu USD. Mặc dù không đấu thầu thành công, ConstitutionDAO đã tạo nên lịch sử: chứng minh năng lực gây quỹ phi tập trung nhanh chóng của blockchain từ những người xa lạ trên internet. Sau khi thất bại, toàn bộ số tiền gây quỹ đã được tự động hoàn trả lại cho các ví gửi ban đầu (chỉ khấu trừ phí giao dịch gas fee của mạng lưới).

Sự kiện này chứng minh sức mạnh của các công cụ tài chính phi tập trung (DeFi) cho phép bất kỳ ai cũng có thể huy động vốn toàn cầu cho dự án của mình với chi phí tối thiểu mà không cần thông qua các định chế tài chính truyền thống.

## 大厂算法题模拟笔试

Vòng thi thuật toán (Coding Interview) luôn là rào cản lớn nhất đối với các lập trình viên khi ứng tuyển vào các tập đoàn công nghệ lớn. Việc chuẩn bị kiến thức giải thuật tốt sẽ là bệ đỡ giúp bạn vượt qua các vòng sát hạch của doanh nghiệp.

Vào lúc 20:00 tối thứ Hai (29/11) tới đây sẽ diễn ra buổi **Thi thử thuật toán chuẩn doanh nghiệp lớn**, giúp các lập trình viên Front-end và Web ôn luyện và cọ xát thực tế:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112518.webp)

Chương trình thi thử gồm 2 phần:

- **Phần 1 (20:00 - 21:00):** Làm bài thi trực tuyến giải quyết các câu hỏi thuật toán Front-end chọn lọc thường gặp ở các kỳ phỏng vấn thực tế của các tập đoàn lớn.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112521.webp)

- **Phần 2 (21:00 - 22:00):** Buổi livestream phân tích đề và hướng dẫn giải thuật chi tiết của chuyên gia **Winter** (cựu chuyên gia công nghệ P8 của Alibaba, cựu trưởng nhóm Front-end Taobao di động).

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112520.webp)

Đây là cơ hội tốt để các bạn Front-end tích lũy kinh nghiệm phỏng vấn và hoàn thiện kỹ năng giải thuật. Những học viên có kết quả thi thử xuất sắc sẽ nhận được cơ hội tư vấn hồ sơ và hướng dẫn phỏng vấn 1-1 trực tiếp từ chuyên gia Winter.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112520.jpg)

Độc giả bản tin có thể quét mã QR trên đây hoặc truy cập [liên kết đăng ký](https://wx.kaikeba.com/xiaoke/market/landing-page/v2/5Npu7PL4AcHvHVf2zWj?kol_ad_code=hSR3JHKqg6n2HDYZwe6) để tham gia thi thử hoàn toàn **miễn phí**.

## 科技动态

1、[Cựu thiết kế trưởng Apple Jony Ive công bố tác phẩm thiết kế mới](https://www.fastcompany.com/90693444/jony-ives-first-major-design-since-leaving-apple-isnt-what-youd-expect)

Jony Ive - người đứng sau hàng loạt thiết kế huyền thoại của Apple như iPhone, sau khi rời hãng năm 2019 để thành lập công ty thiết kế riêng LoveFrom mới đây đã công bố tác phẩm thiết kế công cộng đầu tiên:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110701.jpg)

Đây là mẫu con dấu giấy tinh xảo thiết kế riêng cho quỹ bảo trợ môi trường Terra Carta của Hoàng gia Anh:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110702.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110703.jpg)

Họa tiết con dấu được dập nổi tỉ mỉ hình ảnh chim muông, hoa cỏ đan xen tượng trưng cho sức sống thiên nhiên tươi đẹp. Điểm đặc biệt của thiết kế là để đảm bảo tiêu chuẩn bảo vệ môi trường, con dấu hoàn toàn không sử dụng các chi tiết viền kim loại quý mà được gia công 100% bằng giấy ép sợi tự nhiên cao cấp:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110704.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110705.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110706.jpg)

2、[Startup Mỹ thử nghiệm thành công mô hình phóng tên lửa bằng động năng ly tâm](https://www.odditycentral.com/news/innovative-company-uses-kinetic-energy-to-throw-rockets-into-space.html)

Thay vì chỉ sử dụng phản lực đốt cháy nhiên liệu truyền thống, startup SpinLaunch đã phát triển công nghệ phóng tên lửa bằng động năng ly tâm đột phá:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112402.jpg)

Hệ thống xây dựng một tháp ly tâm hình tròn cao 35 mét. Tên lửa được lắp bên trong và quay với tốc độ cực lớn trước khi được mở chốt quăng thẳng lên tầng bình lưu qua ống dẫn đứng. Thử nghiệm thực tế hồi tháng 10 đã phóng thành công nguyên mẫu tên lửa đạt độ cao hơn 10.000 mét:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112403.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112404.jpg)

Ưu điểm của công nghệ là giảm thiểu đáng kể trọng lượng và chi phí nhiên liệu phóng ở tầng khởi động ban đầu. Tuy nhiên tên lửa vẫn cần trang bị động cơ đốt phụ để đẩy hành trình khi lên tới độ cao lớn, và công nghệ này hiện chưa thể áp dụng cho các dòng tên lửa tải trọng lớn chở người.

3、[Dịch vụ in mã QR thông tin lên bia mộ tại El Salvador](https://www.phnompenhpost.com/lifestyle/salvadoran-resident-replaces-epitaphs-qr-codes)

Một phóng viên ảnh tại El Salvador đã nảy ra ý tưởng thay thế các tấm bia đá khắc chữ truyền thống bằng việc khảm mã QR chống nước lên bia mộ:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110709.jpg)

Người viếng thăm chỉ cần dùng điện thoại quét mã QR để truy cập trang web lưu trữ hình ảnh kỷ niệm, các đoạn video ngắn ghi lại cuộc sống thường nhật và các câu chuyện kể về người quá cố khi còn sống:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110710.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110711.jpg)

4、[Meta giới thiệu nguyên mẫu găng tay phản hồi xúc giác cho không gian VR](https://www.shenzhenware.com/articles/15348)

Tập đoàn Meta (Facebook) vừa giới thiệu nguyên mẫu găng tay thông minh Haptic Gloves hỗ trợ tạo cảm nhận sờ chạm chân thực cho người dùng trong môi trường kính thực tế ảo:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112506.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112507.jpg)

Mặt trong găng tay được bố trí hàng loạt túi khí nén vi mô. Khi người dùng thực hiện thao tác cầm, nắm hoặc sờ vào vật thể ảo trong game VR, hệ thống sẽ tự động bơm xả khí tạo áp lực tương ứng lên da ngón tay để tạo cảm giác về độ cứng, độ mịn hoặc độ rung vật lý của vật thể:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112508.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112509.jpg)

5、[Hệ thống rào chắn nước chiếu đèn STOP độc đáo trong hầm vượt biển Sydney](https://www.laservision.com.au/portfolio/softstop/)

Ban quản lý hầm vượt biển Sydney (Úc) đã triển khai hệ thống rào cản cảnh báo bằng nước Softstop để xử lý các sự cố khẩn cấp trong hầm:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111004.jpg)

Khi xảy ra tai nạn giao thông hoặc cháy nổ phía trước, hệ thống vòi phun trên trần hầm sẽ tự động tạo một bức màn sương nước mỏng phủ kín lối đi, đồng thời máy chiếu công suất lớn sẽ chiếu trực tiếp chữ "STOP" đỏ rực lên màn nước. Biện pháp này giúp cảnh báo trực quan cực kỳ bắt mắt buộc tài xế phanh xe gấp mà không gây hư hại cho phương tiện nếu vô tình đâm qua:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111005.jpg)

## 文章

1. [Thống kê công suất và mức tiêu thụ điện năng của các trạm phát sóng 5G](http://finance.sina.com.cn/tech/csj/2021-02-26/doc-ikftpnny9891878.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112114.jpg)

Bài phân tích số liệu thực tế về mức tiêu thụ điện của hạ tầng mạng mới: một trạm phát sóng 5G ngoài trời có công suất tiêu thụ trung bình 3.8 kW (gấp 3 lần trạm 4G) với chi phí tiền điện rất lớn. Dự báo đến năm 2026, toàn bộ hệ thống trạm 5G sẽ tiêu thụ tới 2.1% tổng sản lượng điện quốc gia.

2. [Tại sao bản làm lại GTA Trilogy Definitive Edition lại bị đánh giá tệ hại?](https://www.yystv.cn/p/8533)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111902.jpg)

Bài viết phân tích các lỗi đồ họa kỳ dị và sự cẩu thả trong khâu lập trình của studio phát triển đối với tựa game làm lại giá 60 USD của hãng Rockstar, gây ra làn sóng tẩy chay lớn từ cộng đồng game thủ.

3. [Hướng dẫn sử dụng esbuild để biên dịch và đóng gói ứng dụng Node.js Express](https://devtails.medium.com/bundling-your-node-js-express-app-with-esbuild-5aecc36c5047)（Tiếng Anh）

Bài viết hướng dẫn lập trình viên Backend phương pháp sử dụng công cụ đóng gói esbuild để gom toàn bộ các tệp tin script dự án Express thành một tệp tin phân phối duy nhất chạy cực nhanh.

4. [Thủ thuật cài đặt kho ứng dụng Google Play Store lên Windows 11](https://www.windowscentral.com/how-run-google-play-store-android-apps-windows-11)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110201.jpg)

Mặc dù Windows 11 hỗ trợ chạy app Android nhưng bị giới hạn dịch vụ Google Services. Bài viết hướng dẫn cách bypass cài đặt nhân Google Play Store giúp chạy mượt mà mọi ứng dụng Android yêu cầu dịch vụ của Google trên máy tính.

5. [Nâng cao độ rõ nghĩa của code JavaScript bằng mẫu thiết kế RORO Pattern](https://www.tinyblog.dev/blog/2020-07-13-javascript-roro-pattern/)（Tiếng Anh）

Giới thiệu phương pháp thiết kế tham số đầu vào và đầu ra của hàm theo mẫu RORO (Receive Object, Return Object) tận dụng tính năng destructuring của ES6 giúp code JavaScript dễ đọc và bảo trì hơn.

6. [Thủ thuật đo đạc thời gian phản hồi của trang web bằng câu lệnh curl](https://susam.in/maze/timing-with-curl.html)（Tiếng Anh）

Hướng dẫn viết lệnh curl kết hợp định dạng cấu hình đầu ra để đo đạc chính xác thời gian phân giải DNS, thời gian kết nối TCP và thời gian tải trang web trực tiếp từ terminal.

7. [Cẩm nang hướng dẫn sử dụng cơ bản bộ chia màn hình terminal Tmux](https://pragmaticpineapple.com/gentle-guide-to-get-started-with-tmux/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082201.jpg)

Bài hướng dẫn chi tiết kèm ảnh động minh họa trực quan các phím tắt quản lý phiên làm việc, phân chia cửa sổ hiển thị dòng lệnh của công cụ Tmux trên Linux.

8. [Bài học đắt giá 5.000 USD từ việc thiếu một chỉ mục cơ sở dữ liệu SQL](https://briananglin.me/posts/spending-5k-to-learn-how-database-indexes-work/)（Tiếng Anh）

Tác giả chia sẻ trường hợp thực tế khi một câu lệnh truy vấn SQL không được thiết lập Index trên đám mây, dẫn tới việc nhà mạng tính phí quét hàng tỷ dòng dữ liệu dư thừa làm hóa đơn tăng vọt.

## 工具

1、[DuckDuckGo TTY: Trình tìm kiếm giao diện terminal](https://duckduckgo.com/tty/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082302.jpg)

Trang web mô phỏng giao diện dòng lệnh của DuckDuckGo cho phép người dùng thực hiện gõ từ khóa tìm kiếm trực tiếp bằng câu lệnh CLI trên trình duyệt.

2、[CodingFont: Công cụ so sánh font chữ lập trình trực quan](https://www.codingfont.com/)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102903.jpg)

Website hỗ trợ lập trình viên so sánh hiển thị mã nguồn trực quan giữa các font chữ chuyên dụng cho lập trình (như JetBrains Mono, Fira Code) để chọn lựa.

3、[Netlify Drop: Deploy website nhanh bằng kéo thả](https://app.netlify.com/drop)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112510.jpg)

Dịch vụ đám mây của Netlify hỗ trợ kéo thả thư mục chứa code HTML/CSS/JS tĩnh để tự động deploy trang web lên Internet trong vài giây.

4、[CSS Doodle: Thiết kế hình học bằng CSS](https://yuanchuan.dev/polygon-shapes)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110103.jpg)

Thành phần Web Component hỗ trợ lập trình viên Front-end vẽ các cấu trúc đa giác và hoa văn trang trí nghệ thuật trực tiếp bằng cú pháp CSS.

5、[Arco Design: Hệ thống thiết kế UI cấp doanh nghiệp của ByteDance](https://arco.design/)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112203.jpg)

Hệ thống thiết kế giao diện (Design System) chính thức từ TikTok hỗ trợ đầy đủ bộ components giao diện cho cả React và Vue. (Đóng góp của [@PengJiyuan](https://github.com/ruanyf/weekly/issues/2070))

6、[Remix: Framework phát triển web React mới](https://blog.remix.run/p/remix-preview)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112401.jpg)

Framework phát triển ứng dụng React tập trung tối ưu hóa tốc độ tải trang thông qua cơ chế render phía server (SSR) được phát triển bởi đội ngũ React Router.

7、[PianoPlayer: Trình mô phỏng 3D cử động ngón tay chơi đàn](https://github.com/marcomusy/pianoplayer)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110104.jpg)

Tiện ích nguồn mở hỗ trợ sinh các hoạt cảnh 3D mô phỏng vị trí đặt ngón tay gõ phím trên đàn piano dựa trên dữ liệu phân tích từ tệp nhạc MIDI đầu vào.

8、[Google DNS Web Tool](https://dns.google/)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110108.jpg)

Trang web chính thức của Google hỗ trợ tra cứu nhanh các thông số bản ghi phân giải tên miền (DNS records) trực quan.

9、[Tree Generator: Tự sinh cấu trúc sơ đồ hình cây dạng text](https://devtool.tech/tree)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112202.jpg)

Công cụ web giúp sinh nhanh sơ đồ thư mục dạng văn bản phân cấp để chèn vào các file hướng dẫn Markdown README.md. (Đóng góp của [@shfshanyue](https://github.com/ruanyf/weekly/issues/2066))

10、[HTTP Server Online: Trình chạy máy chủ tĩnh Front-end](https://github.com/EtherDream/http-server-online)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110109.jpg)

Công cụ web cho phép tạo lập một server chạy thử tài nguyên tĩnh ngay trên trình duyệt mà không cần cài đặt Node hay Python.

## Tài nguyên

1、[DeepCourse: Bản đồ kiến thức học tập Deep Learning](https://arthurdouillard.com/deepcourse/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090811.jpg)

Chương trình học tập AI và Deep Learning được thiết kế trực quan theo dạng sơ đồ đường đi giúp người học dễ dàng bấm chọn và theo dõi tiến độ tích lũy kiến thức.

2、[OKR.com: Tổng hợp tài liệu quản trị mục tiêu OKR](https://www.okr.com/)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112324.jpg)

Trang tổng hợp các bài viết nghiên cứu và tài liệu thực tế hướng dẫn áp dụng cơ chế đánh giá hiệu năng OKR trong doanh nghiệp. (Đóng góp của [@xcuYao](https://github.com/ruanyf/weekly/issues/2068))

3、[Archive.org Serendipity: Nghe nhạc đĩa nhựa cổ](https://www.locserendipity.com/PushPlay.html)

Dự án hỗ trợ phát ngẫu nhiên các bản nhạc thu âm từ đĩa nhựa cổ từ thế kỷ trước đã hết hạn bản quyền được lưu trữ trên Internet Archive.

4、[Tổng hợp các trang web chia sẻ hình ảnh miễn phí bản quyền](https://admcpr.com/where-to-find-royalty-free-images/)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021101304.jpg)

Bài viết tổng hợp danh sách các nguồn chất lượng cung cấp ảnh chụp phong cảnh, ảnh minh họa vector miễn phí cho các nhà thiết kế web.

5、[Ten Years Ago: Trải nghiệm lướt web 10 năm trước](https://neal.fun/ten-years-ago/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090805.jpg)

Website lưu trữ lịch sử cho phép người dùng xem lại chính xác giao diện hiển thị của các trang web nổi tiếng vào đúng ngày này của 10 năm trước.

## 图片

1、[Chân dung cổ nhân sống ở thời hiện đại](https://mossandfog.com/artist-imagines-what-famous-historical-figures-would-look-like-today/)

Một nghệ sĩ đồ họa đã thực hiện bộ sưu tập tranh chân dung tái hiện diện mạo của các nhân vật lịch sử nổi tiếng nếu họ sống ở thế kỷ 21:

- Leonardo da Vinci:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091201.jpg)

- Thiếu nữ đeo hoa tai ngọc trai:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091202.jpg)

- Mona Lisa:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091203.jpg)

- Tượng Binh mã dũng đất nung:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091204.jpg)

2、[Thiết kế phòng họp đối diện đặc sắc của Nghị viện Anh](https://www.notboring.co/p/the-interface-phase)

Khác với thiết kế dạng rạp hát bán nguyệt của Nghị viện Mỹ:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091406.jpg)

Hạ viện Anh sở hữu bố cục thiết kế hai hàng ghế dài đối diện trực tiếp vào nhau qua lối đi trung tâm:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091407.jpg)

Thiết kế này được Winston Churchill ủng hộ mạnh mẽ sau Thế chiến II nhằm thúc đẩy tranh luận trực tiếp và phân định rõ hai luồng quan điểm đối lập (ủng hộ hoặc phản đối), không để lại bất kỳ vị trí thỏa hiệp trung gian nào:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091408.jpg)

## Bài đọc thêm

### Nguồn gốc lịch sử của tên gọi công nghệ kết nối không dây Bluetooth

Công nghệ kết nối không dây tầm ngắn Bluetooth hiện nay có mặt trên hầu hết các thiết bị điện tử. Tuy nhiên tên gọi *"Răng xanh"* độc đáo này bắt nguồn từ đâu?

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090712.jpg)

Vào năm 1998, khi các công ty viễn thông lớn đang tranh luận tìm giải pháp thiết lập một quy chuẩn sóng không dây thống nhất toàn cầu, hai kỹ sư Sven Mattisson (Ericsson, Thụy Điển) và Jim Kardach (Intel, Mỹ) đã cùng nhau đi uống bia tại Toronto.

Trong cuộc trò chuyện về lịch sử Bắc Âu, kỹ sư người Thụy Điển đã kể về vị vua Viking Đan Mạch thế kỷ thứ 10 tên là Harald Gormsson, người nổi tiếng với biệt danh "Bluetooth" (được cho là do ông có một chiếc răng bị hỏng ngả màu xanh). Vua Harald có công lao to lớn khi thống nhất các bộ tộc Đan Mạch và Na Uy cổ:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112526.jpg)

Nhận thấy sự tương đồng giữa việc vua Harald thống nhất các bộ tộc và mục tiêu thống nhất các chuẩn kết nối không dây của dự án, kỹ sư người Mỹ đã đề xuất lấy "Bluetooth" làm mật danh tạm thời cho dự án. Khi tiêu chuẩn kết nối được chính thức ban hành vào tháng 5/1998, do không tìm được tên gọi thương mại nào phù hợp hơn, mật danh này đã trở thành tên gọi chính thức cho tới ngày nay.

## 言论

1\.

Vào năm 2016, ứng dụng nhắn tin WhatsApp đã cán mốc hơn 1 tỷ người dùng thường xuyên nhưng toàn bộ hệ thống Backend chỉ được vận hành bởi vỏn vẹn 50 kỹ sư, chia thành các nhóm nhỏ độc lập từ 1-3 người có quyền tự quyết rất lớn.

-- Trích bài viết "How WhatsApp Scaled to 1 Billion Users"

2\.

Nếu bạn nhận được email chỉ thị từ tôi, bạn chỉ có 3 lựa chọn phản hồi, nếu không hãy nộp đơn xin từ chức lập tức:
- 1. Phản hồi giải thích rõ ràng tại sao chỉ thị của tôi là sai lầm.
- 2. Yêu cầu tôi giải thích thêm nếu nội dung email chưa rõ nghĩa.
- 3. Thực hiện chính xác theo chỉ thị.

-- Trích email nội bộ của Elon Musk gửi ban quản lý Tesla tháng 10/2021

## 历史上的本周

- 2020年（第 134 期）：[Thảo luận về tiềm năng tăng trưởng quy mô gấp 100 lần của ngành công nghiệp game trong tương lai](https://www.ruanyifeng.com/blog/2020/11/weekly-issue-134.html)
- 2019年（第 82 期）：[Lời khuyên định nghiệp: Nên lựa chọn đầu quân vào các ngành công nghiệp có tốc độ tăng trưởng nhanh nhất](https://www.ruanyifeng.com/blog/2019/11/weekly-issue-82.html)
- 2018年（第 31 期）：[Thảo luận về các dấu hiệu nhận biết thời điểm nghỉ hưu thích hợp đối với lập trình viên](https://www.ruanyifeng.com/blog/2018/11/weekly-issue-31.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
