# Bản tin chia sẻ công nghệ (Số 345): HDMI 2.2 có thể đã chạm tới giới hạn nghe nhìn

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/6443) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041104.webp)

Hoạt động du thuyền bằng bè tre ngắm cảnh đêm lung linh sắc màu dọc bờ sông tại huyện Tuyên Ân, tỉnh Hồ Bắc. (Nguồn: [estv.com.cn](https://estv.com.cn/tt/3015235.htm))

## HDMI 2.2 影音可能到头了

Vào tháng 1 đầu năm nay, có một tin tức công nghệ nổi bật mà nhiều người có thể đã bỏ qua: Hiệp hội HDMI chính thức công bố [chuẩn kết nối HDMI phiên bản 2.2](https://finance.sina.com.cn/tech/roll/2025-01-07/doc-ineeeanv7947700.shtml).

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041201.webp)

Hôm nay tôi muốn bàn luận sâu hơn về sự kiện này. Tôi xin phép đưa ra một dự đoán mang tính táo bạo: Chuẩn kết nối phần cứng này nhiều khả năng đã chạm tới giới hạn tối đa của nhu cầu thực tế và sẽ khó có thêm các bước nhảy vọt đáng kể nào nữa về sau.

Cổng kết nối HDMI là chuẩn giao tiếp truyền dẫn hình ảnh và âm thanh phổ biến nhất hiện nay trên thế giới. Hầu như mọi người dùng công nghệ đều đã từng tiếp xúc qua cổng này khi kết nối các thiết bị phát như máy tính, đầu thu kỹ thuật số với màn hình tivi hay màn hình máy tính.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041202.webp)

Chuẩn kết nối này liên tục được nâng cấp định kỳ theo thời gian, với mục tiêu cốt lõi qua mỗi phiên bản là gia tăng đáng kể băng thông tốc độ truyền tải tín hiệu:

*   HDMI 1.0 - 1.2 (Năm 2002): Tốc độ truyền tải 4.9 Gbps
*   HDMI 1.3 - 1.4 (Năm 2006): Tốc độ truyền tải 10.2 Gbps
*   HDMI 2.0 (Năm 2013): Tốc độ truyền tải 18 Gbps
*   HDMI 2.1 (Năm 2017): Tốc độ truyền tải 48 Gbps
*   HDMI 2.2 (Năm 2025): Tốc độ truyền tải 96 Gbps

Quan sát danh sách trên, có thể thấy băng thông truyền tải tín hiệu của HDMI qua mỗi lần nâng cấp lớn đều ghi nhận mức tăng trưởng gấp đôi để đáp ứng xu thế phát triển của các định dạng video chất lượng cao với dung lượng dữ liệu ngày một khổng lồ.

Ở phiên bản nâng cấp từ HDMI 2.1 lên HDMI 2.2 lần này, băng thông truyền dữ liệu đã được đẩy vọt từ mốc 48 Gbps lên đến 96 Gbps.

**Mốc băng thông tốc độ truyền tải 96 Gbps thực sự là một con số khổng lồ kinh ngạc**.

Chúng ta hãy cùng làm một so sánh trực quan: Hạ tầng mạng internet gia đình tốc độ cao nhất hiện nay thường đạt mốc 10 Gbps (vốn đã vượt quá nhu cầu sử dụng thực tế của đại đa số người dùng phổ thông), trong khi chuẩn kết nối HDMI 2.2 sở hữu tốc độ truyền tải nhanh gấp 10 lần con số đó!

Đây hiện là chuẩn giao tiếp truyền dẫn nghe nhìn có tốc độ nhanh nhất thế giới. Ngay cả khi truyền tải đồng thời nhiều luồng video có độ phân giải cao nhất hiện nay, sợi cáp HDMI 2.2 vẫn dư sức đáp ứng mà vẫn còn thừa rất nhiều băng thông trống.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041401.webp)

Vấn đề cốt lõi nằm ở chỗ: Người dùng phổ thông hầu như không thể khai thác hết năng lượng của chuẩn kết nối này. Để truyền tải một luồng video chất lượng cao định dạng 4K ở tốc độ khung hình 60fps đi kèm các tiêu chuẩn HDR10 hoặc Dolby Vision thời gian thực, chúng ta thực tế chỉ cần đến sợi cáp đạt chuẩn HDMI 2.0 là đã hoàn toàn đáp ứng tốt.

Để trình chiếu các nội dung video siêu nét định dạng 8K ở tốc độ 60fps, hệ thống mới cần huy động đến chuẩn HDMI 2.1. Trong khi đó, **chuẩn kết nối HDMI 2.2 mới ra mắt được thiết kế để hỗ trợ truyền tải video đạt độ phân giải kỷ lục lên tới 12K ở tốc độ 60fps**.

Nhưng liệu người dùng có thực sự phát sinh nhu cầu xem các nội dung video đạt độ phân giải siêu nét lên tới 12K trên tivi tại gia đình hay không?

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041609.webp)

Giới công nghệ thường nhắc tới khái niệm "[Độ phân giải Retina](https://vi.wikipedia.org/wiki/M%C3%A0n_h%C3%ACnh_Retina)" (Retina Display), dùng để chỉ ngưỡng mật độ điểm ảnh tối đa mà mắt người có khả năng phân biệt được ở một khoảng cách quan sát thông thường.

Một khi mật độ điểm ảnh của màn hình vượt qua ngưỡng giới hạn sinh học này, mắt người hoàn toàn không thể nhận biết thêm bất kỳ sự gia tăng độ sắc nét nào nữa. Việc tiếp tục nâng cao độ phân giải khi đó sẽ trở nên hoàn toàn vô nghĩa về mặt trải nghiệm thị giác.

Vào năm 2010, tỷ phú Steve Jobs lần đầu tiên giới thiệu khái niệm này tại sự kiện ra mắt điện thoại iPhone 4. Ông tuyên bố ở khoảng cách sử dụng thông thường từ 25 đến 30 cm, mắt người hoàn toàn không thể phát hiện ra các điểm ảnh riêng lẻ hiển thị trên màn hình của iPhone 4.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041610.webp)

Độ phân giải Retina phụ thuộc trực tiếp vào hai biến số cốt lõi: Khoảng cách từ mắt đến màn hình, và kích thước vật lý của màn hình đó.

Kích thước màn hình càng lớn và khoảng cách quan sát càng gần đòi hỏi độ phân giải màn hình phải càng cao; ngược lại nếu kích thước màn hình nhỏ và khoảng cách quan sát xa, độ phân giải yêu cầu sẽ giảm đi đáng kể.

Một chuyên gia nước ngoài đã [tiến hành các phép tính toán học](https://archimago.blogspot.com/2025/03/hdmi-musings-high-speed-cables-data.html) thực tế: Trong một không gian phòng chiếu phim gia đình thông thường, **nếu người xem ngồi ở khoảng cách 3,6 mét để thưởng thức video 12K, kích thước màn hình phải lớn tới 550 inch thì mắt người mới bắt đầu chạm tới ngưỡng giới hạn phân biệt Retina**.

Một màn hình kích thước 550 inch tương đương với chiều rộng khoảng 12 mét và chiều cao 6,8 mét — ngang ngửa với kích thước của một tấm biển quảng cáo ngoài trời cỡ lớn!

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041611.webp)

Nói cách khác, **đối với tất cả các màn hình có kích thước nhỏ hơn 550 inch, việc trang bị độ phân giải 12K là hoàn toàn dư thừa và lãng phí**, vì mắt người bình thường không thể phân biệt được sự khác biệt về độ sắc nét so với các độ phân giải thấp hơn.

Do đó, không gian gia đình thông thường hoàn toàn không phát sinh nhu cầu thực tế cho độ phân giải 12K. Ngay tại phòng khách gia đình, một chiếc tivi độ phân giải 4K đã là quá đủ để đáp ứng hoàn hảo tiêu chuẩn hiển thị Retina cho mắt người.

Ở giai đoạn phát triển hiện tại, việc nâng cấp chất lượng hiển thị của hình ảnh chủ yếu được tập trung vào các chỉ số kỹ thuật khác như độ chính xác của màu sắc, độ tương phản động (HDR) chứ không còn phụ thuộc nhiều vào việc tăng mật độ điểm ảnh nữa.

Câu chuyện tương tự cũng diễn ra trong lĩnh vực âm thanh. Đối với tai người nghe thông thường, chất lượng âm thanh định dạng CD chuẩn đã đạt tới giới hạn cảm nhận âm thanh nổi của con người. Việc tiếp tục nâng cao tần số lấy mẫu hay độ sâu bit âm thanh hầu như không mang lại sự khác biệt có thể nhận biết được. Tín hiệu âm thanh chất lượng cao này thực tế chỉ cần băng thông của chuẩn USB 2.0 (480 Mbps) là đã thừa sức truyền tải thời gian thực.

Tóm lại, mặc dù các tiêu chuẩn công nghệ nghe nhìn hoàn toàn có thể tiếp tục được nâng cao hơn nữa về mặt lý thuyết, **giới hạn cảm nhận sinh học của con người là có hạn. Các công nghệ hiện tại đã chạm tới ngưỡng giới hạn cảm quan này**, việc tiếp tục đầu tư nâng cao băng thông truyền tải sẽ mang lại những giá trị thặng dư ngày một ít đi.

Bản thân tôi thực sự chưa thể hình dung ra trong tương lai, nếu các nhà sản xuất tiếp tục công bố chuẩn kết nối HDMI 2.3 hoặc 3.0 với băng thông truyền tải lớn hơn nữa thì chúng sẽ phục vụ cho kịch bản ứng dụng thực tế nào của đời sống?

## 科技动态

1、[Bang California chính thức ban hành luật cấm sử dụng cụm từ "Hạn bán" trên bao bì thực phẩm](https://www.foodandwine.com/california-bans-sell-by-dates-8723111)

Chính quyền bang California (Mỹ) vừa thông qua một đạo luật mới quy định kể từ tháng 7 năm 2026, các doanh nghiệp sản xuất thực phẩm sẽ bị cấm in cụm từ "Hạn bán" (Sell-By) lên bao bì sản phẩm, mà bắt buộc phải thay thế bằng cụm từ "Sử dụng tốt nhất trước ngày" (Best Before).

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024101101.webp)

Nguyên nhân do người tiêu dùng thường hiểu lầm mốc "Hạn bán" chính là thời hạn cuối cùng thực phẩm còn an toàn để ăn. Hệ quả là ngay khi vừa bước qua mốc này, lượng lớn thực phẩm chất lượng tốt lập tức bị tiêu hủy gây lãng phí nghiêm trọng.

Trên thực tế, mốc thời gian này chỉ mang ý nghĩa là khoảng thời gian thực phẩm đạt hương vị thơm ngon nhất.

Các báo cáo thống kê chỉ ra sự hiểu lầm về hạn sử dụng này là nguyên nhân làm thất thoát tới 33% lượng thực phẩm tại Mỹ hằng năm. Đạo luật mới cho phép các thực phẩm quá hạn khuyến nghị vẫn được tiếp tục trưng bày trên kệ hàng nếu bảo đảm chất lượng, ước tính giúp bang California giảm thiểu khoảng 70.000 tấn thực phẩm bị lãng phí và tiết kiệm khoảng 300 triệu USD mỗi năm.

2、Sự kiện Triển lãm Thế giới Osaka Expo 2025 vừa chính thức khai mạc ghi nhận công trình kiến trúc bằng gỗ có quy mô lớn nhất thế giới hiện nay.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025040907.webp)

Đó là một cấu trúc vòng tròn khổng lồ bằng gỗ với chu vi kéo dài tới 2 km, mang ý nghĩa biểu tượng cho tinh thần đoàn kết và gắn kết giữa các quốc gia tham gia triển lãm.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025040908.webp)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041702.webp)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025040909.webp)

3、[Robot hình người hỗ trợ bảo trì trên cao](https://www.facebook.com/moneysaveJP/posts/507308291818047/)

Công ty Đường sắt Tây Nhật Bản (JR West) sở hữu hệ thống đường dây điện trên cao vô cùng đồ sộ, trong khi doanh nghiệp luôn đối mặt với tình trạng thiếu hụt nhân sự bảo trì lành nghề, đồng thời các tác vụ làm việc trên cao luôn tiềm ẩn nhiều rủi ro mất an toàn.

Để giải quyết bài toán này, hãng đã đưa ra một giải pháp độc đáo khi lắp đặt một robot hình người trực tiếp trên cabin của xe nâng chuyên dụng.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072407.webp)

Ngoại hình của robot được thiết kế lấy cảm hứng từ nhân vật người máy trong bộ truyện tranh nổi tiếng *Mobile Suit Gundam*, với hệ thống camera quan sát được tạo hình giống như hai mắt của robot.

Robot được điều khiển trực tiếp bởi một nhân viên kỹ thuật ngồi ở cabin điều khiển phía dưới xe nâng để đưa robot lên cao thực hiện các thao tác sửa chữa. Về bản chất, robot này chưa sở hữu các thuật toán tự chủ thông minh mà hoạt động tương tự như một con rối cơ học dưới sự điều khiển của con người.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072408.webp)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072409.webp)

4、**Các tin tức khác**

(1) Giao diện màn hình báo lỗi chết chóc màu xanh lam (BSOD) truyền thống của hệ điều hành Windows nhiều khả năng sẽ được Microsoft thay đổi trong thời gian tới.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025040407.webp)

Trong bản cập nhật thử nghiệm mới nhất dành cho người dùng Windows Insider, giao diện báo lỗi sập hệ thống đã được chuyển đổi sang tông nền màu đen tối giản (hình dưới) tương tự như giao diện cập nhật hệ thống thông thường.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025040408.webp)

(2) Nền tảng ghi chú Notion giới thiệu dịch vụ hộp thư điện tử mới mang tên **Notion Mail**, ở giai đoạn thử nghiệm đầu tiên dịch vụ mới chỉ hỗ trợ liên kết đồng bộ hóa dữ liệu từ tài khoản Gmail.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041601.webp)

(3) Thời hạn hiệu lực tối đa của các chứng chỉ bảo mật TLS (SSL) dành cho website sẽ được rút ngắn xuống chỉ còn 47 ngày, quy định mới sẽ chính thức có hiệu lực áp dụng kể từ năm 2026.

## 文章

1、[Chúng ta đang chính thức bước vào kỷ nguyên của các dòng chip tích hợp quy mô lớn (Big Chip Era)](https://www.xda-developers.com/were-entering-the-big-chip-era-and-i-couldnt-be-more-excited/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041109.webp)

Khái niệm chip lớn ở đây dùng để chỉ cấu trúc thiết kế tích hợp chung cả bộ vi xử lý CPU, nhân đồ họa GPU và bộ nhớ RAM vào bên trong một đế chip duy nhất (System-on-Chip - SoC), với đại diện tiêu biểu là dòng chip M-series của Apple.

Kiến trúc thiết kế này giúp CPU và GPU chia sẻ trực tiếp chung một vùng nhớ RAM với băng thông bộ nhớ cực lớn, giải thích lý do tại sao các máy tính chạy chip Apple hoàn toàn đủ năng lực vận hành mượt mà các mô hình AI lớn mà không bắt buộc phải trang bị card đồ họa rời chuyên dụng của Nvidia.

2、[Trải nghiệm thực tế khi quyết định từ bỏ laptop để chuyển sang sử dụng máy tính mini bỏ túi kết hợp kính AR](https://www.tomsguide.com/computing/i-ditched-my-laptop-for-a-pocketable-mini-pc-and-a-pair-of-ar-glasses-heres-what-happened) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041604.webp)

Tác giả giới thiệu bộ thiết bị làm việc di động gọn nhẹ khi đi ra ngoài của mình bao gồm: một máy tính mini bỏ túi, một viên pin sạc dự phòng hiệu năng cao, một chiếc kính thực tế ảo tăng cường AR thay thế màn hình hiển thị cùng bộ bàn phím chuột không dây siêu mỏng.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041605.webp)

3、[Tại sao mã QR sinh ra từ liên kết viết hoa toàn bộ lại có kích thước hiển thị nhỏ hơn viết thường?](https://shkspr.mobi/blog/2025/02/why-are-qr-codes-with-capital-letters-smaller-than-qr-codes-with-lower-case-letters/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030617.webp)

Tác giả chia sẻ một phát hiện thú vị: Nếu chúng ta tiến hành chuyển đổi toàn bộ các ký tự của đường link URL sang định dạng viết hoa trước khi tạo mã QR, hình ảnh mã QR kết xuất ra sẽ có kích thước nhỏ gọn và các điểm ảnh hiển thị thưa hơn nhiều so với việc giữ nguyên định dạng chữ viết thường.

4、[Một mẹo nhỏ giúp đo đạc chính xác hiệu năng chạy mã nguồn JavaScript](https://ates.dev/posts/2025-01-12-accurate-benchmarking/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025011911.webp)

Thông thường khi đo đạc hiệu năng chạy của một đoạn code JS, lập trình viên hay sử dụng các vòng lặp lớn, nhưng bản thân việc duy trì vòng lặp cũng tiêu tốn tài nguyên hệ thống. Tác giả giới thiệu giải pháp loại bỏ sai số này bằng cách thiết lập hai vòng lặp: vòng lặp thứ nhất chạy thực thi code 1 lần, vòng lặp thứ hai chạy thực thi code 2 lần, sau đó lấy kết quả thời gian của vòng lặp thứ hai trừ đi vòng lặp thứ nhất để ra thời gian chạy thuần túy của code.

5、[Hướng dẫn làm đẹp định dạng hiển thị cho tệp tin RSS/Atom feeds](https://taxodium.ink/pretty-feed.html) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041501.webp)

Bài hướng dẫn kỹ thuật cơ bản giới thiệu phương pháp nhúng các định dạng giao diện (CSS/XSLT) vào tệp tin XML của RSS giúp giao diện đọc feed hiển thị trực quan và thân thiện hơn với người dùng. (Đóng góp từ [@Spike-Leung](https://github.com/ruanyf/weekly/issues/6576))

6、[Tìm hiểu các thuộc tính định dạng text-wrap mới trong CSS](https://webkit.org/blog/16547/better-typography-with-text-wrap-pretty/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041108.webp)

Thuộc tính `text-wrap` trong CSS được khai thác để kiểm soát quy tắc xuống dòng của văn bản. Bài viết giới thiệu tính năng của hai giá trị khai báo mới là `text-wrap: pretty` (giúp tối ưu hóa khoảng cách xuống dòng đẹp mắt hơn) và `text-wrap: balance` (giúp cân bằng số lượng chữ đồng đều giữa các dòng).

## 工具

1、[yabs.sh](https://github.com/masonr/yet-another-bench-script)

Bộ mã kịch bản Bash shell chuyên dụng để đo đạc và kiểm tra hiệu năng (benchmark) của máy chủ Linux. Tham khảo thêm [bài viết hướng dẫn cài đặt sử dụng](https://blog.aawadia.dev/2023/08/26/yabs-august-2023/).

2、[Pākiki Proxy](https://pakikiproxy.com/)

Ứng dụng máy tính đa nền tảng hỗ trợ nhà phát triển dễ dàng theo dõi, kiểm soát và chỉnh sửa các luồng dữ liệu truyền tải qua giao thức bảo mật HTTPS và WebSocket chạy cục bộ trên máy tính.

3、[Giant Log Viewer](https://github.com/sunny-chung/giant-log-viewer)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041602.webp)

Ứng dụng máy tính hỗ trợ người dùng dễ dàng mở và đọc mượt mà các tệp tin dữ liệu ghi chép (log files) có dung lượng cực lớn lên tới hàng TB mà không làm sập bộ nhớ máy tính.

4、[OpenAPI DevTools](https://github.com/AndrewWalsh/openapi-devtools)

Tiện ích mở rộng trên Chrome hỗ trợ tự động phân tích các luồng yêu cầu mạng thời gian thực để tự động sinh ra tệp cấu hình mô tả API chuẩn hóa theo định dạng OpenAPI.

5、[Online 3D Viewer](https://3dviewer.net)

Dự án thư viện mã nguồn mở hỗ trợ kết xuất và hiển thị trực tiếp các tệp tin đồ họa 3D đa định dạng ngay trên giao diện trình duyệt web.

6、[Tirreno](https://github.com/TirrenoTechnologies/tirreno)

Hệ thống phân tích thống kê lượng truy cập người dùng (Analytics) mã nguồn mở phát triển trên nền tảng ngôn ngữ PHP.

7、[EaseVoice Trainer](https://github.com/megaease/easevoice-trainer)

Ứng dụng mã nguồn mở chạy cục bộ trên máy tính hỗ trợ người dùng tự huấn luyện và克隆 (cloning) giọng nói cá nhân bằng AI. (Đóng góp từ [@xxx7xxxx](https://github.com/ruanyf/weekly/issues/6569))

8、[Lexe](https://github.com/Ray-D-Song/lexe)

Công cụ hỗ trợ đóng gói các ứng dụng viết bằng Node.js thành một tệp tin thực thi duy nhất chạy trực tiếp dựa trên lõi chạy JS tối giản LLRT, giúp giảm thiểu tối đa dung lượng tệp tin sau đóng gói. (Đóng góp từ [@Ray-D-Song](https://github.com/ruanyf/weekly/issues/6597))

9、[Treex](https://github.com/shiquda/treex)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041504.webp)

Công cụ dòng lệnh mã nguồn mở hỗ trợ hiển thị cấu trúc sơ đồ cây của thư mục máy tính đi kèm nhiều bộ lọc hiển thị và tùy biến định dạng xuất ra. (Đóng góp từ [@shiquda](https://github.com/ruanyf/weekly/issues/6591))

10、[py-xiaozhi](https://github.com/huangjunsen0406/py-xiaozhi)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041701.webp)

Dự án ứng dụng ngôn ngữ Python tái dựng lại trợ lý giọng nói thông minh Xiaozhi, hỗ trợ đầy đủ các tính năng tương tác giọng nói, điều khiển thiết bị thông minh IoT và phát nhạc trực tuyến mà không đòi hỏi trang bị phần cứng chuyên dụng. (Đóng góp từ [@huangjunsen0406](https://github.com/ruanyf/weekly/issues/6643))

## AI 相关

1、[PureChat](https://github.com/Hyk260/PureChat)

Giao diện quản trị trò chuyện AI mã nguồn mở hỗ trợ kết nối linh hoạt với nhiều dịch vụ API mô hình lớn phổ biến như OpenAI, Ollama hay DeepSeek, phát triển trên Vue 3 và Vite 5. (Đóng góp từ [@Hyk260](https://github.com/ruanyf/weekly/issues/6567))

2、[Vanna](https://github.com/vanna-ai/vanna)

Dự án AI hỗ trợ phân tích dữ liệu cơ sở dữ liệu mã nguồn mở: Cho phép người dùng đưa ra câu hỏi bằng ngôn ngữ tự nhiên, hệ thống sẽ tự động phân tích sinh ra câu lệnh SQL chuẩn xác và thực thi để hiển thị kết quả cho người dùng. (Đóng góp từ [@904192063](https://github.com/ruanyf/weekly/issues/6573))

3、[AI 视频图文创作助手 (AI-Media2Doc)](https://github.com/hanshuaikang/AI-Media2Doc)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041503.webp)

Bộ công cụ hỗ trợ người dùng chuyển đổi các nội dung video hoặc tệp tin âm thanh thành các bài viết văn bản theo nhiều phong cách biên soạn khác nhau, hỗ trợ cài đặt chạy hoàn toàn cục bộ trên máy tính cá nhân. (Đóng góp từ [@hanshuaikang](https://github.com/ruanyf/weekly/issues/6584))

## 资源

1、[Flight Track in 3D Earth](https://flight.is26.com/)

Dịch vụ web hỗ trợ hiển thị mô phỏng 3D đường bay thực tế của một chuyến bay bất kỳ trên mô hình quả địa cầu tương tác trực quan. (Đóng góp từ [@foru17](https://github.com/ruanyf/weekly/issues/6583))

2、[Bản đồ hệ thống tàu hỏa chạy đêm tại Châu Âu (European Night Train Map)](https://back-on-track.eu/night-train-map/)

Một trang web sở hữu thiết kế đồ họa vô cùng ấn tượng và giàu tính tương tác rất đáng để tham khảo học hỏi: Cho phép người dùng click chọn trực tiếp vào từng tuyến đường tàu chạy để hiển thị cửa sổ thông tin chi tiết về hành trình.

3、[Sách hướng dẫn cấu trúc thị trường chứng khoán (Market Structure Primer)](https://primer.prooftrading.com/)

Cuốn sách điện tử tiếng Anh cung cấp các kiến thức cơ bản hệ thống về cấu trúc vận hành của thị trường chứng khoán Mỹ, rất hữu ích cho các nhà đầu tư cá nhân có kế hoạch tham gia giao dịch cổ phiếu Mỹ.

## 生成随机数的波浪机

Tập đoàn dịch vụ bảo mật internet Cloudflare sở hữu một nét văn hóa độc đáo khi lắp đặt tại các văn phòng chi nhánh của hãng trên thế giới các hệ thống thiết bị vật lý cơ học kỳ lạ.

Mục tiêu của các hệ thống này là tạo ra các nguồn dữ liệu biến động tự nhiên hoàn toàn không thể dự đoán trước để phục vụ việc sinh các mã khóa số ngẫu nhiên cho thuật toán mã hóa dữ liệu.

Ví dụ tiêu biểu nhất là hệ thống đèn dung nham (Lava Lamps) được bố trí tại văn phòng trụ sở San Francisco:

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031204.webp)

Sự chuyển động và biến đổi hình dáng liên tục của chất lỏng bên trong các bóng đèn được camera ghi nhận lại, sau đó máy tính sẽ phân tích các pixel ảnh để tạo thành các số ngẫu nhiên bảo mật.

Tại văn phòng London, hãng thiết lập một "Bức tường con lắc đơn" với hàng loạt con lắc liên tục chuyển động độc lập:

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031205.webp)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031206.webp)

Tại văn phòng Austin là hệ thống trần nhà được bao phủ bởi các tấm phản quang siêu mỏng dễ dàng xoay chuyển trước bất kỳ luồng chuyển động không khí nhỏ nào trong phòng:

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031207.webp)

Độc giả có thể tìm đọc chi tiết về cơ chế vận hành của các thiết bị này tại bài viết giới thiệu trong [Bản tin số 305](https://www.ruanyifeng.com/blog/2024/06/weekly-issue-305.html).

Tháng trước, nhân dịp khai trương văn phòng chi nhánh mới tại Lisbon (Bồ Đào Nha), Cloudflare đã tiếp tục công bố một thiết bị vật lý sinh số ngẫu nhiên mới độc đáo.

Đó là một bức tường lớn được cấu thành từ 50 chiếc máy tạo sóng cơ học độc lập:

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032005.webp)

Mỗi chiếc máy tạo sóng là một ống nghiệm thủy tinh nằm ngang chứa các dung dịch có màu sắc nổi bật như xanh lam, xanh lá hoặc màu cam.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032006.webp)

Hệ thống mô tơ điện điều khiển các ống nghiệm xoay chuyển liên tục khoảng 14 lần mỗi phút (hơn 20.000 lần mỗi ngày). Chất lỏng di chuyển liên tục bên trong ống nghiệm theo chu kỳ xoay tạo nên các chuyển động sóng nước ngẫu nhiên:

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032007.webp)

Hệ thống gương phản quang bố trí phía sau sẽ phóng đại các hiệu ứng khúc xạ ánh sáng đi qua làn nước chuyển động, tạo thành nguồn dữ liệu hình ảnh ngẫu nhiên chất lượng cao phục vụ quy trình mã hóa bảo mật của máy chủ.

## 文摘

1、[Văn hóa "Đáng yêu" tại Hàn Quốc](https://walkingtheworld.substack.com/p/the-unbearable-lightness-of-korean)

Tôi là người đặc biệt yêu thích thành phố Seoul của Hàn Quốc, và trong vòng 4 năm qua tôi đã thực hiện tổng cộng 7 chuyến du lịch đến đây.

Trong các chuyến đi, tôi quan sát thấy một hiện tượng nổi bật: Toàn bộ không gian thành phố Seoul được bao phủ bởi vô số các họa tiết trang trí mang phong cách dễ thương (Cute Culture) ở khắp mọi nơi mà người đi đường hoàn toàn không thể né tránh. Hầu như mọi vật dụng công cộng hay thương mại đều được tạo hình theo phong cách các nhân vật hoạt hình.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041606.webp)

Người dân địa phương ở mọi lứa tuổi đều hào hứng chi tiền mua sắm các loại thú bông mềm mại.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041607.webp)

Ngay tại các quán ăn hải sản, hình ảnh quảng cáo vẽ chú bạch tuộc hoạt hình dễ thương được tô son môi điệu đà — mặc dù đó chính là loài vật mà thực khách sẽ gọi món để nhà bếp chế biến và ăn thịt sau đó.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025041608.webp)

Dưới góc nhìn cá nhân, tôi cảm giác thế hệ trẻ tại Hàn Quốc đang tìm cách拥抱 (chìm đắm vào) các biểu tượng dễ thương này như một cơ chế tâm lý tự vệ để đối phó với áp lực khủng khiếp của xã hội tiêu dùng, chủ nghĩa vật chất và sự trống rỗng tinh thần đi kèm.

Việc cố gắng biến mọi khía cạnh của đời sống xã hội trở nên đáng yêu giúp làm giảm bớt cảm giác ngột ngạt và sự tẻ nhạt của nhịp sống hằng ngày, giúp né tránh các câu hỏi nghiêm túc về giá trị cuộc sống và làm cho hành vi tiêu dùng bớt đi cảm giác vô nghĩa.

Bản thân tôi hoàn toàn ủng hộ việc nhân cách hóa các con vật hay đồ vật để tạo sự thân thiện. Tuy nhiên khi văn hóa đáng yêu này bị đẩy lên thành một hệ thế giới quan chi phối toàn xã hội thì lại mang đến một cảm giác tương đối đáng buồn.

Tại Seoul, văn hóa đáng yêu dường như đã trở thành một hệ thế giới quan chủ đạo của thế hệ trẻ để đối phó với một tương lai thiếu vắng đi các giá trị tinh thần chiều sâu.

Mặc dù văn hóa này tương đối nông cạn, nó lại vận hành vô cùng khớp với cơ chế của một xã hội tiêu dùng: Việc mua sắm nhiều thú bông đáng yêu hơn giúp kích thích sinh ra nhiều niềm vui ngắn hạn hơn, thôi thúc người dùng tiếp tục chi tiêu mua sắm nhiều hơn nữa.

Một xã hội thực sự hạnh phúc và vận hành bền vững đòi hỏi phải được định hình bởi các hệ giá trị niềm tin và tiêu chuẩn thẩm mỹ có chiều sâu để giúp con người vượt lên trên các nhu cầu vật chất thuần túy.

Việc cố gắng sử dụng sự đáng yêu nông cạn để lấp đầy khoảng trống tinh thần đó thực chất chỉ là một giải pháp tự lừa dối bản thân.

## 言论

1、

Nội dung của loạt phim khoa học viễn tưởng nổi tiếng *Black Mirror* (Gương đen) mang đậm tư duy bi quan công nghệ cực đoan khi chỉ tập trung khai thác và thổi phồng các rủi ro của sự phát triển kỹ thuật, hoàn toàn ngó lơ các giá trị thực tế của công nghệ giúp cải thiện chất lượng sống của nhân loại vượt trội so với quá khứ. Lối làm phim này gieo rắc nỗi sợ hãi mơ hồ về tương lai vào tâm trí công chúng.

Tuy nhiên thực tế đã chứng minh, nếu nhân loại mong muốn hướng tới một tương lai tốt đẹp và thịnh vượng hơn, công nghệ chính là con đường khả thi duy nhất.

-- *Trích bài phân tích đăng tải trên tờ The Guardian của Anh*

2、

Triết lý viết code cốt lõi của bản thân tôi đi theo hướng tiếp cận "Lập trình hướng đau khổ" (Suffering-Oriented Programming). Cụ thể, khi phát sinh một vấn đề kỹ thuật nào thực sự gây ra sự phiền toái và đau khổ lớn cho quy trình làm việc của mình, tôi sẽ lập tức tập trung giải quyết nó triệt để; vấn đề nào gây đau khổ lớn nhất sẽ được ưu tiên xử lý trước tiên; những vấn đề nhỏ chưa gây ảnh hưởng lớn sẽ tạm thời được bỏ qua.

Phương pháp lập trình này bảo đảm bạn luôn tập trung 100% nguồn lực vào các tác vụ thực sự quan trọng và có giá trị thực tế cao nhất, từ đó giảm thiểu tối đa các rủi ro lãng phí thời gian phát triển dự án.

-- *Trích bài chia sẻ 《Lập trình hướng đau khổ》*

3、

Thuật toán phân phối của các mạng xã hội hiện nay hoàn toàn không ưu tiên cho các nội dung có chất lượng chuyên môn sâu, mà chỉ tập trung tối đa vào các chỉ số tương tác bề nổi và các giải pháp AI nhằm mục đích thu hút tối đa lưu lượng truy cập để thương mại hóa quảng cáo.

Thực tế này dẫn đến việc người dùng liên tục bị dẫn dụ và thao túng cảm xúc bởi các nội dung gây tranh cãi, trong khi khó lòng tiếp cận được các tác phẩm sáng tạo có chiều sâu và giàu tính chân thực của các tác giả.

-- *Trích bài viết 《Không ai nên tự định danh bản thân là một nhà sáng tạo nội dung (Content Creator)》*

4、

Quy trình tự học lập trình cốt lõi của một hacker luôn đi theo chu kỳ lặp: Bắt đầu bằng việc tự tay nghịch và phá phách thử nghiệm một công cụ bất kỳ, sau đó quay lại đọc tài liệu hướng dẫn kỹ thuật để hiểu cơ chế, tiếp tục quay lại nghịch sâu hơn, lại tiếp tục đọc tài liệu để gỡ lỗi... Chu trình này được lặp đi lặp lại liên tục cho đến khi hoàn toàn thấu suốt bản chất của hệ thống.

-- *Trích nội dung cuốn Sách tay của Hacker (Hacker's Handbook)*

## 往年回顾

- Số #298: [Nhận định về xu hướng: Thời đại hoàng kim của các kỹ sư phần cứng đã chính thức quay trở lại](https://www.ruanyifeng.com/blog/2024/04/weekly-issue-298.html)
- Số #248: [Thảo luận về luận điểm: Chúng ta không nên thần thánh hóa và phóng đại quá mức năng lực của ChatGPT](https://www.ruanyifeng.com/blog/2023/03/weekly-issue-248.html)
- Số #198: [Phân tích về tính khả thi của chiến lược khôi phục lại ngành công nghiệp sản xuất ngay tại nước Mỹ](https://www.ruanyifeng.com/blog/2022/03/weekly-issue-198.html)
- Số #148: [Chiêm nghiệm về giai đoạn chuyển dịch sang thời kỳ tăng trưởng kinh tế ở mức độ thấp (Vi tăng trưởng)](https://www.ruanyifeng.com/blog/2021/03/weekly-issue-148.html)

(Hết)
