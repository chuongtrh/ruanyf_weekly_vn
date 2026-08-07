# 科技爱好者周刊（第 182 期）：新人优惠的风险

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2032) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110101.jpg)

Hình ảnh chụp trung tâm thương mại Raffles City Trùng Khánh lọt vào vòng chung kết Giải thưởng Nhiếp ảnh Kiến trúc Thế giới 2021. (Nguồn: [CNN](https://edition.cnn.com/style/article/architectural-photography-awards-2021-shortlist/))

## 主带话题：Rủi ro pháp lý từ lỗ hổng chương trình ưu đãi người dùng mới

Rất nhiều ứng dụng (App) hiện nay triển khai các chương trình "Ưu đãi khách hàng mới" hoặc "Đơn hàng đầu tiên miễn phí" với các phần quà hấp dẫn nhằm thu hút người dùng đăng ký.

Gần đây, một vụ án hình sự liên quan đến việc lạm dụng kẽ hở của chương trình khuyến mại này tại Thượng Hải là bài học cảnh tỉnh sâu sắc cho giới lập trình viên và người tiêu dùng.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110501.jpg)

Tóm tắt vụ việc như sau: Cuối năm 2019, một trung tâm thương mại tại quận Dương Phố, Thượng Hải triển khai chương trình khuyến mại: Mọi khách hàng mới đăng ký tài khoản app của trung tâm sẽ nhận được 500 điểm tích lũy dùng để quy đổi sang 1 giờ đỗ xe miễn phí (trị giá 10 NDT).

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110302.jpg)

Tận dụng cơ hội này, hơn 120 nhân viên văn phòng tại các tòa nhà lân cận đã sử dụng "接码平台" (nền tảng cung cấp số điện thoại ảo trực tuyến để nhận mã xác thực OTP) đăng ký hàng vạn tài khoản mới liên tục để trừ điểm đỗ xe miễn phí hàng ngày. Hành vi này gây thiệt hại cho trung tâm thương mại hơn 370.000 NDT (trong đó có chiếc xe đỗ miễn phí quy đổi tới hơn 10.000 NDT tiền gửi xe).

Sau khi nhận tin báo án, cơ quan cảnh sát đã nhanh chóng định vị nhóm nhân viên văn phòng trên, buộc truy thu lại toàn bộ số tiền trốn phí đỗ xe và ra quyết định khởi tố hình sự 20 đối tượng có hành vi trục lợi lớn về tội danh Lừa đảo chiếm đoạt tài sản. Hiện tại đã có 2 bị án phải nhận hình phạt tù.

Vụ án chỉ ra việc lạm dụng quá đà các kẽ hở khuyến mại có thể bị khép vào khung hình phạt tội lừa đảo chiếm đoạt tài sản.

Tuy nhiên, tôi có một vài góc nhìn khác về vụ việc này. Việc nhân viên văn phòng tham lam trục lợi nhỏ là sai trái, nhưng ban quản lý trung tâm thương mại cũng phải chịu một phần trách nhiệm lớn vì thiết kế chương trình quá lỏng lẻo. Họ hoàn toàn không xây dựng bất kỳ cơ chế kiểm soát kỹ thuật nào (ví dụ đơn giản: khống chế một biển số xe chỉ được áp dụng mã giảm giá khách hàng mới duy nhất 1 lần). Việc buông lỏng quản lý và kiểm soát rủi ro của doanh nghiệp đã vô tình tạo điều kiện thử thách lòng tham của con người. Nếu tòa án phán quyết doanh nghiệp tự gánh chịu phần lớn thiệt hại tài chính thì cũng hoàn toàn hợp lý để làm bài học cho các đơn vị vận hành app khác.

Đáng chú ý, cơ quan cảnh sát cũng tiến hành bắt giữ 4 đối tượng lập trình và vận hành nền tảng số điện thoại ảo nhận OTP nói trên.

> *"Sử (25 tuổi), học viên cao học ngành phần mềm tại một trường đại học lớn đã tự lập trình phát triển và vận hành phần mềm chuyên cung cấp dịch vụ số điện thoại ảo nhận OTP. Dù nhận thức rõ người dùng mua dịch vụ này để trục lợi khuyến mại của các nền tảng thương mại điện tử, Sử vẫn tiếp tục cung cấp và thu lời bất chính hơn 100.000 NDT.*
> 
> *Mới đây, Tòa án Nhân dân quận Dương Phố đã tuyên phạt bị cáo Sử 6 tháng tù giam và phạt hành chính 10.000 NDT về tội danh 'Giúp đỡ hoạt động tội phạm mạng' (帮助信息网络犯罪活动罪)."*

Giai thoại cảnh tỉnh giới lập trình viên: Việc phát triển các công cụ tự động hóa gửi nhận tin nhắn thuần túy không vi phạm pháp luật, nhưng nếu bạn cung cấp dịch vụ phụ trợ hỗ trợ cho các hành vi gian lận trục lợi thương mại của người dùng, bạn hoàn toàn có thể đối mặt với trách nhiệm hình sự liên đới. Lập trình viên cần chú ý tìm hiểu rõ mục đích sử dụng phần mềm của khách hàng.

## Khóa học thuật toán Core-logic dành cho kỹ sư chuyên nghiệp (P6)

Trong cấu trúc nhân sự của các tập đoàn công nghệ lớn như Alibaba, cấp độ P6 (Senior Engineer - Kỹ sư dày dặn kinh nghiệm) là vị trí tuyển dụng chủ lực đòi hỏi năng lực tự lập trình dự án độc lập mượt mà.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110405.jpg)

Thị trường tuyển dụng kỹ sư phần mềm hiện nay luôn săn đón nhân sự đạt chuẩn P6. Với các lập trình viên muốn ứng tuyển vào các tập đoàn lớn, việc chuẩn bị kiến thức giải thuật cấu trúc dữ liệu nâng cao là yêu cầu bắt buộc.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110406.jpg)

Các vòng phỏng vấn P6 đặc biệt chú trọng sát hạch tư duy giải thuật nâng cao (chẳng hạn cơ chế hoạt động của thuật toán DOM Diff trong core Vue và React).

Tuần này, chúng tôi giới thiệu khóa học chuyên đề **《Algorithm Principles for P6 Engineers》** dành cho các kỹ sư Front-end:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110407.jpg)

Chương trình học gồm 2 buổi livestream hướng dẫn chi tiết về các giải thuật lõi trong thiết kế giao diện web, cách thức giải đề thuật toán LeetCode tối ưu và chia sẻ kinh nghiệm phỏng vấn.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110408.jpg)

Độc giả bản tin có thể quét mã QR trên đây để đăng ký tham gia khóa học với mức phí ưu đãi chỉ **0.99 NDT**.

## 科技动态

1、[Trung Quốc thử nghiệm thành công giống lúa khổng lồ cao 2 mét](https://news.mydrivers.com/1/779/779562.htm)

Giống lúa khổng lồ thế hệ mới do các nhà khoa học nông nghiệp phát triển đã được gieo trồng thử nghiệm thành công tại thành phố Trùng Khánh.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082911.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082912.jpg)

Giống lúa này có chiều cao trung bình đạt 1,8m (cá biệt có cây vượt 2m), gấp đôi giống lúa thông thường. Nhờ sải thân cây cao lớn và bộ rễ cắm sâu, giống lúa này cho năng suất hạt rất tốt trên mỗi bông. Ưu điểm lớn nhất là ruộng lúa có thể tích nước ngập sâu tới 80cm, tạo điều kiện thuận lợi để triển khai mô hình cộng sinh lúa - cá - tôm giúp tăng thu nhập cho nông dân và hạn chế tối đa việc sử dụng hóa chất bảo vệ thực vật:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082913.jpg)

2、[Na Uy giới thiệu ý tưởng "Bức tường điện gió" khổng lồ ngoài khơi](https://www.dezeen.com/2021/08/26/wind-catching-systems-floating-offshore-farm/)

Thông thường các trạm điện gió ngoài khơi sử dụng các cột tuabin đơn độc có cánh quạt xoay lớn. Một hãng năng lượng Na Uy đã đề xuất thiết kế đột phá mang tên Windcatching wall:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090108.jpg)

Hệ thống sử dụng một khung giàn thép khổng lồ có chiều cao hơn 300 mét (tương đương tháp Eiffel). Trên mặt lưới thép được lắp đặt tích hợp hơn 100 tuabin gió cỡ nhỏ độc lập:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090109.jpg)

Thiết kế này giúp tận dụng tối đa dòng gió đại dương đi qua khung. Hãng tuyên bố sản lượng phát điện của một bức tường tương đương với công suất của 5 cột tuabin gió đơn lớn nhất hiện nay cộng lại với chi phí phát điện giảm một nửa. Nguyên mẫu dự kiến sẽ được triển khai lắp đặt trong 3 năm tới.

3、[Căn hộ mẫu "Near-zero energy building" đầu tiên ra mắt tại Bắc Kinh](http://www.bj.xinhuanet.com/2021-08/11/c_1127749972.htm)

Cơ sở văn phòng mẫu ứng dụng tiêu chuẩn tiết kiệm năng lượng tối đa "Near-zero energy" vừa được đưa vào vận hành tại quận Thông Châu, Bắc Kinh:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081104.jpg)

Tòa nhà tự cấp 100% điện năng hoạt động điều hòa, chiếu sáng và sưởi ấm duy trì nhiệt độ ổn định ở mức 20 độ C quanh năm nhờ tích hợp bơm nhiệt địa nhiệt sâu dưới lòng đất, bơm nhiệt không khí và các tấm pin mặt trời áp mái kết hợp hệ thống 5 bể trữ năng lượng lớn dưới hầm tòa nhà.

4、[Zeit Medical ra mắt băng đeo trán phát hiện sớm tai biến đột quỵ](https://www.zeitmedical.com/)

Tai biến mạch máu não (đột quỵ) là bệnh lý cực kỳ nguy hiểm và khó dự báo trước. Bệnh nhân sau khi phát bệnh bắt buộc phải được đưa đến bệnh viện cấp cứu trong khung giờ vàng để hạn chế tối đa di chứng bại não:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081307.jpg)

Startup Zeit Medical (Mỹ) đã chế tạo mẫu băng đeo trán thông minh tích hợp điện cực giám sát sóng não liên tục khi ngủ. Khi phát hiện các bước sóng não bất thường trùng khớp dấu hiệu đột quỵ, thiết bị sẽ phát tín hiệu cảnh báo về điện thoại và tự động kích hoạt gọi xe cứu thương gửi kèm tọa độ định vị của người dùng:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081308.jpg)

5、[Tây Ban Nha phát triển công nghệ thu điện sinh học từ vi sinh vật đất](https://sifted.eu/articles/bioo-batteries-electricity-soil/)

Tập đoàn công nghệ Bioo (Tây Ban Nha) công bố thử nghiệm thành công giải pháp thu điện năng trực tiếp từ đất trồng trọt:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090507.jpg)

Khi các vi sinh vật trong đất phân giải các chất hữu cơ tự nhiên, chúng sẽ giải phóng ra các electron tự do. Bằng cách cắm điện cực âm và dương sâu xuống lòng đất, hệ thống có thể thu thập dòng điện này. Hiệu năng thu được khoảng 200 Wh điện năng mỗi năm trên 1 mét vuông đất màu mỡ. Lượng điện nhỏ này rất tối ưu để cấp nguồn hoạt động liên tục cho các cảm biến đo độ ẩm, pH đất nông nghiệp mà không cần pin sạc:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090508.jpg)

6\. [Sinh viên Na Uy thử nghiệm theo dõi lộ trình người dùng qua địa chỉ Bluetooth](https://www.theregister.com/2021/09/04/bluetooth_headphones_tracking_oslo/)

Mỗi thiết bị Bluetooth (như tai nghe không dây, vòng đeo tay thông minh) đều có một địa chỉ MAC cố định phát ra khi kết nối.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090601.jpg)

Một sinh viên đại học Na Uy đã thực hiện dự án nghiên cứu thực địa để kiểm tra nguy cơ lộ lọt thông tin riêng tư này. Anh đã đạp xe liên tục trong 12 ngày qua quãng đường 300 km ở thủ đô Oslo để thu thập sóng Bluetooth phát ra xung quanh:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110502.jpg)

Kết quả ghi nhận 9.149 địa chỉ Bluetooth độc nhất, trong đó có 129 tai nghe không dây bị bắt tín hiệu liên tục nhiều lần ở các vị trí khác nhau giúp phác họa chính xác lộ trình di chuyển thường nhật của chủ nhân tai nghe. Thí nghiệm cảnh báo nguy cơ bị theo dõi hành trình nếu các trạm thu phát Bluetooth công cộng được triển khai thu thập thông tin.

## 文章

1、[Trải nghiệm cài đặt và chạy ứng dụng Android trên Windows 11](https://sspai.com/post/69446)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102203.jpg)

Bài hướng dẫn chi tiết các bước thiết lập môi trường giả lập Windows Subsystem for Android (WSA) mới ra mắt trên Windows 11, đồng thời chia sẻ đánh giá thực tế về hiệu năng chơi game và khả năng tương thích app di động.

2、[Ý tưởng thiết kế đưa đường ray lên cao của nhà ga cao tốc Tây Hàng Châu](https://mp.weixin.qq.com/s/jSeAG_YoTEJshhTQZLHf1Q)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102401.jpg)

Bài viết phân tích thiết kế của ga tàu cao tốc Tây Hàng Châu phục vụ thế vận hội ASIAD 2022: đưa hệ thống đường ray và sân ga lên tầng cao của tòa nhà, giải phóng không gian mặt đất bên dưới cho mạng lưới giao thông công cộng đô thị, tránh việc đường ray chia cắt thành phố làm đôi.

3、[Đánh giá kế hoạch xây dựng siêu nhà máy đúc chip GigaFab của SMIC](https://www.anandtech.com/show/16931/china-smic-build-gigafab)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092111.jpg)

Bài phân tích chuyên sâu về kế hoạch đầu tư xây dựng cơ sở sản xuất chip bán dẫn quy mô lớn GigaFab (công suất thiết kế vượt 100.000 tấm wafer/tháng) tại khu thương mại tự do Lâm Cảng, Thượng Hải của tập đoàn SMIC.

4、[Microsoft chính thức ra mắt trang web vscode.dev hỗ trợ lập trình viên](https://code.visualstudio.com/blogs/2021/10/20/vscode-dev)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102909.jpg)

Microsoft công bố phát hành tên miền chính thức `vscode.dev` cho phép lập trình viên chạy trực tiếp trình soạn thảo VS Code trên mọi trình duyệt web di động và máy tính mà không cần cài đặt node hay thư viện hỗ trợ. (Đóng góp của [@StevenNin](https://github.com/ruanyf/weekly/issues/2012))

5、[Hướng dẫn đăng ký mã chỉ số tạp chí ISSN cho trang blog cá nhân](https://shkspr.mobi/blog/2021/09/how-to-add-issn-metadata-to-a-web-page/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092006.jpg)

Tác giả chia sẻ kinh nghiệm chuẩn bị hồ sơ và đăng ký thành công mã chỉ số ISSN quốc tế cho trang blog cá nhân của mình giúp chuẩn hóa siêu dữ liệu phục vụ các trích dẫn nghiên cứu khoa học.

6、[Tại sao doanh nghiệp nên cấu hình tệp tin Security.txt trên server?](https://krebsonsecurity.com/2021/09/does-your-organization-have-a-security-txt-file/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092213.jpg)

Giới thiệu tiêu chuẩn bảo mật mới đề xuất việc cấu hình tệp tin cấu trúc `security.txt` đặt tại thư mục gốc `.well-known/` của website giúp các chuyên gia bảo mật mũ trắng dễ dàng tìm thấy thông tin liên hệ báo cáo lỗ hổng an ninh.

7、[Phát triển giao diện web theo cơ chế Server-Informed UI](https://max.engineer/server-informed-ui)（Tiếng Anh）

Tác giả đề xuất phương án tối ưu thiết kế API Backend: thay vì chỉ xây dựng một hệ thống API chung cho mọi tác vụ, hãy tách biệt thành một cổng API dữ liệu chung và một cổng API chuyên biệt định hình giao diện (Server-Informed UI) giúp client render trang nhanh hơn.

8、[Nhật ký tự lắp ráp và cấu hình case máy tính chơi game chạy hệ điều hành Linux](https://boilingsteam.com/how-i-built-my-new-linux-gaming-desktop-in-2021-with-amd-cpugpu-and-gnu-guix/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092408.jpg)

Tác giả chia sẻ kinh nghiệm lựa chọn linh kiện phần cứng (CPU AMD, card đồ họa Radeon) và cài đặt phân phối hệ điều hành GNU Guix để tự dựng một cỗ máy PC chuyên dụng chơi game mượt mà trên nền tảng Linux:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092409.jpg)

9、[Tìm hiểu API phát hiện trạng thái rảnh Idle Detection API của Chrome](https://web.dev/idle-detection/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092414.jpg)

Hướng dẫn sử dụng đối tượng `IdleDetector` mới được tích hợp sẵn trên Chrome hỗ trợ website phát hiện hành vi người dùng không hoạt động (không gõ phím, di chuột hoặc màn hình bị khóa) để tự động lưu dữ liệu hoặc tắt các tác vụ nặng.

## 工具

1、[EBS Design: Thư viện components React hiện đại](https://github.com/ebs-integrator/ebs-design)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092112.jpg)

Bộ component UI mã nguồn mở được thiết kế theo phong cách tối giản hiện đại (Neumorphism kết hợp Flat Design) đang được phát triển tích cực cho các ứng dụng React.

2、[bunny.net: Dịch vụ CDN hiệu năng cao](https://bunny.net/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091812.jpg)

Một nhà cung cấp dịch vụ mạng truyền tải nội dung CDN có tính phí được đánh giá cao nhờ tốc độ phân phối dữ liệu nhanh và chi phí hợp lý, thích hợp làm giải pháp dự phòng cho Cloudflare.

3、[context-note: Extension ghi chú tài liệu trực tiếp trên website](https://github.com/betterRunner/context-note)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102406.jpg)

Extension Chrome hỗ trợ người dùng quét chọn văn bản và tạo ghi chú trực tiếp trên trang web, tự động lưu trữ hiển thị lại ghi chú đó ở đúng vị trí cũ trong lần truy cập sau. (Đóng góp của [@betterRunner](https://github.com/ruanyf/weekly/issues/2013))

4、[APIAuto: Hệ thống tự động hóa kiểm thử API của Tencent](https://github.com/TommyLemon/APIAuto)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102404.jpg)

Dự án nguồn mở của Tencent hỗ trợ quét cấu trúc API, tự động sinh các test-cases và thực hiện kiểm thử tự động dựa trên phân tích thuật toán học máy thông minh. (Đóng góp của [@TommyLemon](https://github.com/ruanyf/weekly/issues/2010))

5、[3D pipes Screen Saver in HTML5 Canvas](https://1j01.github.io/pipes/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092004.jpg)

Dự án mã nguồn mở thú vị sử dụng thư viện đồ họa để tái hiện lại hoàn hảo màn hình chờ 3D Pipes (đường ống dẫn nước 3D) huyền thoại của Windows 95/98 ngay trên trang web.

6、[Composable: Trình vẽ đồ họa vector trực tuyến](https://www.composable.art/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092107.jpg)

Công cụ trực tuyến gọn nhẹ hỗ trợ người dùng vẽ, chỉnh sửa và xuất các file đồ họa vector dạng SVG trực tiếp trên trình duyệt web.

7、[lists.sr.ht: Dịch vụ mailing list nguồn mở](https://lists.sr.ht/)

Nền tảng hỗ trợ các nhà phát triển thiết lập và quản lý hệ thống hòm thư chung (mailing list) phục vụ thảo luận đóng góp mã nguồn cho dự án công nghệ.

8、[Kill the Newsletter! (Chuyển đổi email newsletter sang RSS)](https://github.com/leafac/kill-the-newsletter)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091814.jpg)

Công cụ nguồn mở hỗ trợ chuyển đổi toàn bộ các email bản tin nhận qua hòm thư thành đường dẫn cập nhật luồng RSS feed giúp quản lý thông tin tập trung trên các ứng dụng đọc tin. (Demo: [kill-the-newsletter.com](https://kill-the-newsletter.com/))

9、[AirGuard: Phát hiện AirTag lạ theo dõi xung quanh](https://github.com/seemoo-lab/AirGuard)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091917.jpg)

Ứng dụng nguồn mở dành riêng cho điện thoại Android hỗ trợ quét tìm nhanh sự hiện diện của các thiết bị định vị Bluetooth lạ (như AirTag) đang di chuyển theo lộ trình của bạn để cảnh báo nguy cơ bị bám đuôi.

10、[Black: Trình format code Python chuẩn hóa](https://black.vercel.app/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092215.jpg)

Thư viện định dạng mã nguồn Python tự động (code formatter) được cộng đồng tin dùng nhất nhờ khả năng dọn dẹp các khoảng trống dư thừa và căn lề code chuẩn hóa.

## Tài nguyên

1、[10 công cụ trực tuyến kiểm thử giao diện responsive của website](https://www.webfx.com/blog/web-design/responsive-design-testing-tools/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080508.jpg)

Giới thiệu danh sách 10 công cụ web tiện ích hỗ trợ nhà phát triển Front-end giả lập hiển thị và kiểm tra lỗi vỡ khung giao diện web trên nhiều độ phân giải màn hình di động khác nhau.

2、[pi (zhaoolee): Hướng dẫn biến Raspberry Pi thành máy chủ cloud](https://github.com/zhaoolee/pi)

Cẩm nang hướng dẫn chi tiết cách cấu hình máy tính nhúng mini Raspberry Pi 4B kết hợp công cụ nội soi mạng frp để thiết lập một server đám mây cá nhân có IP tĩnh truy cập từ xa. (Đóng góp của [@zhaoolee](https://github.com/ruanyf/weekly/issues/2008))

3、[CPU Museum: Bảo tàng chip xử lý Intel trực tuyến](https://www.mynikko.com/CPU/)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102403.jpg)

Trang web chia sẻ thông tin hình ảnh chi tiết giới thiệu bộ sưu tập các thế hệ chip xử lý của Intel từ thời kỳ sơ khai 3101 cho đến dòng Pentium M của tác giả. (Đóng góp của [@TransparentLC](https://github.com/ruanyf/weekly/issues/2009))

4、[Git Flight Rules: Cẩm nang xử lý nhanh các sự cố Git](https://github.com/k88hudson/git-flight-rules/blob/master/README_zh-CN.md)

Bản dịch tiếng Trung tổng hợp các câu hỏi thường gặp và cẩm nang câu lệnh Git tương ứng để giải quyết nhanh các tình huống gộp nhánh lỗi, sửa tin nhắn commit sai hoặc khôi phục file bị xóa. (Đóng góp của [@xcuYao](https://github.com/ruanyf/weekly/issues/2015))

5、[Decentralized Library: Thư viện Libgen chuyển dịch lên IPFS](https://libgen.fun/dweb.html)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092005.jpg)

Dự án thư viện sách điện tử khổng lồ Libgen công bố hoàn thành việc chuyển đổi toàn bộ cơ sở dữ liệu và trang hiển thị sang giao thức lưu trữ phân tán IPFS giúp hạn chế rủi ro bị khóa máy chủ.

## 图片

1、[Hình ảnh hoang phế tại trụ sở cũ của tập đoàn Motorola](https://www.abandonedspaces.com/industry/motorola.html)

Được thành lập và đặt đại bản doanh từ năm 1976 tại ngoại ô Chicago, đây là nơi chứng kiến chiếc điện thoại di động đầu tiên của nhân loại được phát minh:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081417.jpg)

Sau đợt chia tách doanh nghiệp do thua lỗ giai đoạn 2007-2009, hãng đã quyết định di dời trụ sở về trung tâm thành phố Chicago, bỏ lại khu tổ hợp văn phòng rộng lớn dần rơi vào hoang phế trước khi chính thức bị tháo dỡ vào năm 2017:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081418.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081419.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081420.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081421.jpg)

2\. [Thuật toán phục dựng thành công bức tranh dang dở của họa sĩ M. C. Escher](https://www.universiteitleiden.nl/en/news/2020/04/how-mathematician-hendrik-lenstra-completed-an-unfinished-artwork-by-escher)

Họa sĩ người Hà Lan M. C. Escher nổi tiếng với các bức vẽ gây ảo giác không gian 3 chiều. Tác phẩm cuối đời của ông vẽ cảnh một người đang xem tranh trong phòng triển lãm có các cửa sổ lồng ghép kỳ lạ vào khu phố bên ngoài:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081504.jpg)

Tác giả đã để trống một vòng tròn lớn ở khu vực tâm bức tranh kèm chữ ký của mình. Năm 2000, một giáo sư toán học người Mỹ đã phát hiện ra quy luật tỷ lệ co giãn xoắn ốc (droste effect) của tranh và viết thuật toán máy tính để phục dựng thành công phần khuyết thiếu này:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081503.jpg)

## Bài đọc thêm

### Triết lý phát triển năng lực: Tầm quan trọng của độ dốc (Slope) so với điểm chặn (Intercept)

*Tại sao trong dài hạn, gia tốc thích ứng học hỏi của cá nhân lại quan trọng hơn điểm xuất phát của họ:*

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081907.jpg)

Nếu vẽ lộ trình phát triển sự nghiệp của bạn lên hệ trục tọa độ với trục hoành là thời gian và trục tung là mức độ tích lũy kỹ năng, lộ trình đó sẽ là một đường thẳng đi lên được định hình bởi hai biến số: điểm chặn trục tung y-intercept (điểm xuất phát nền tảng ban đầu của bạn) và độ dốc slope (gia tốc thích ứng học hỏi và nỗ lực bền bỉ của bạn theo thời gian).

Thực tế chứng minh: Ngay cả khi một người có điểm xuất phát ban đầu (y-intercept) thấp hơn rất nhiều so với các đồng nghiệp khác, chỉ cần họ duy trì được một độ dốc học hỏi (slope) lớn hơn, họ chắc chắn sẽ bứt phá và vượt xa các đối thủ trong dài hạn.

Việc rèn luyện kỹ năng mới mỗi ngày thường khó duy trì do trong ngắn hạn bạn hầu như không thấy sự thay đổi rõ rệt nào trên biểu đồ. Nhưng hãy tin tưởng vào định luật tích lũy: mọi nỗ lực nhỏ hàng ngày sẽ cộng dồn theo thời gian để tạo nên sự bứt phá vượt bậc. Tương tự trong tuyển dụng nhân sự, một ứng viên có tinh thần ham học hỏi tiềm năng lớn về lâu dài sẽ mang lại nhiều giá trị đột phá cho doanh nghiệp hơn là một ứng viên có sẵn nhiều kinh nghiệm cũ nhưng thiếu khả năng thích ứng.

## 言论

1\.

Tôi rất ghét xu hướng các dự án phần mềm hiện nay chuyển toàn bộ khu vực thảo luận kỹ thuật sang nền tảng Discord. Việc này làm đứt gãy khả năng tìm kiếm index của các bộ máy tìm kiếm (như Google) đối với các lỗi hệ thống cũ, đồng thời gây phiền toái cho người dùng khi phải quản lý quá nhiều tài khoản định danh trên cùng một nền tảng.

-- Thảo luận trên Hacker News

2\.

Một trong những bài học quản lý tài chính cá nhân cốt lõi là: *"Gia tăng thu nhập và Cắt giảm chi phí"*. Tuy nhiên hai mục tiêu này đòi hỏi hai trạng thái tư duy hoàn toàn trái ngược nhau: việc gia tăng thu nhập đòi hỏi bạn phải sẵn sàng đầu tư mạo hiểm học hỏi kỹ năng mới, trong khi việc cắt giảm chi phí đòi hỏi bạn phải có tư duy cực kỳ bảo thủ phòng thủ tài chính.

-- Trích bài viết "My Top 10 Money Rules"

## 历史上的本周

- 2020年（第 131 期）：[Thảo luận về mô hình tư duy logic nhị phân (Binary) và logic tam phân (Ternary) của bộ não con người](https://www.ruanyifeng.com/blog/2020/10/weekly-issue-131.html)
- 2019年（第 79 期）：[Phân tích sự phụ thuộc ngày càng lớn của hoạt động sinh hoạt thường nhật của con người vào hệ thống máy móc tự động](https://www.ruanyifeng.com/blog/2019/10/weekly-issue-79.html)
- 2018年（第 28 期）：[Thảo luận triết học về bản chất của kiến thức và quy trình tích lũy tri thức trong lập trình phần mềm](https://www.ruanyifeng.com/blog/2018/10/weekly-issue-28.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
