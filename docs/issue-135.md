# 科技爱好者周刊（第 135 期）：Ngành nào phù hợp để khởi nghiệp?

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1520) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112601.jpg)

Bãi đỗ xe đa sắc màu mới được xây dựng tại quận Bắc Bối, Trùng Khánh, sử dụng lớp phủ hạt gốm màu đỏ, vàng, xanh trên bề mặt. Phương pháp này ngoài tăng tính thẩm mỹ thị giác, còn giúp bảo vệ nền đường tốt hơn, tăng ma sát chống trượt và nâng cao độ an toàn khi đỗ xe. (Nguồn: [Tân Hoa Xã](http://www.cq.xinhuanet.com/2020-11/25/c_1126780141.htm))

## 主带话题：Ngành nào phù hợp để khởi nghiệp?

Một nhà đầu tư mạo hiểm người Mỹ chia sẻ cách ông lựa chọn các dự án đầu tư dựa trên một hệ tọa độ rất thú vị.

Ông vẽ một hệ trục tọa độ để định vị các ngành công nghiệp trong đó:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111409.jpg)

Trong hệ tọa độ trên:
- Trục tung thể hiện **quy mô giao dịch** (giá trị đơn hàng càng lên cao càng lớn);
- Trục hoành thể hiện **tần suất giao dịch** (tần suất mua hàng càng sang phải càng nhiều).

Dựa trên hai trục này, tất cả các ngành nghề có thể chia làm 4 nhóm chính:
1. **Giá giao dịch cao, tần suất giao dịch thấp** (Ô tô, bất động sản, chụp ảnh cưới, khám sức khỏe cao cấp).
2. **Giá giao dịch thấp, tần suất giao dịch thấp** (Thợ sửa ống nước, thợ khóa, dụng cụ thể thao, quần áo chuyên dụng).
3. **Giá giao dịch thấp, tần suất giao dịch cao** (Taxi, ăn uống nhanh, nhu yếu phẩm).
4. **Giá giao dịch cao, tần suất giao dịch cao** (Hầu như không tồn tại ngành nào có đặc tính này).

Ví dụ: Giá nhà đất rất đắt, người bình thường vài chục năm mới mua một căn, nên bất động sản nằm ở góc trên bên trái; Đồ ăn quán nhỏ giá rẻ, bạn ghé ăn thường xuyên, nên ăn uống nằm ở góc dưới bên phải.

**Nhà đầu tư mạo hiểm này khuyên: Các dự án đầu tư nên tập trung vào góc trên bên trái (Giá cao, tần suất thấp) hoặc góc dưới bên phải (Giá thấp, tần suất cao), tuyệt đối đừng đụng vào góc dưới bên trái (Giá thấp, tần suất thấp).** Lý do rất đơn giản: Một ngành mà giá trị sản phẩm đã rẻ lại còn rất ít khi phát sinh giao dịch thì làm sao có thể tạo ra doanh thu đột phá để doanh nghiệp sống khỏe?

Ví dụ: Nền tảng gọi xe trực tuyến (như Uber, Didi) có thể thành công lớn vì đây là hành vi "giá thấp, tần suất cao"; trong khi nền tảng gọi thợ mở khóa rất khó thành công vì đây là hành vi "giá thấp, tần suất thấp" (hiếm khi có ai bị khóa cửa liên tục).

Ông phân tích thêm: 
- Các ngành thuộc nhóm **"Giá cao, tần suất thấp"** thích hợp sử dụng mô hình trang web/ứng dụng dọc (Vertical Portal), vì đơn giá cao nên có thể tích hợp sâu chuỗi cung ứng thượng nguồn và hạ nguồn để tối ưu hóa biên lợi nhuận; 
- Các ngành **"Giá thấp, tần suất cao"** lại phù hợp với mô hình nền tảng ngang (Horizontal Platform) để bao phủ thị trường rộng lớn, lấy số lượng giao dịch khổng lồ bù đắp chi phí vận hành.

Điều này hoàn toàn trùng khớp với thực tế tại Trung Quốc. Các nền tảng dịch vụ ngang như Taobao, Meituan, Didi phục vụ các ngành "giá thấp, tần suất cao". Các trang web chuyên sâu theo ngành dọc như Beike (bất động sản), Autohome (ô tô) phục vụ các ngành "giá cao, tần suất thấp".

## Khóa học "Front-end và Đồ họa máy tính"

Đồ họa máy tính (Computer Graphics) là một trong những mảng chuyên sâu nhất của phát triển Front-end. Kiến thức và kỹ năng yêu cầu ở mảng này rất khác biệt so với các hướng đi thông thường, thuộc nhóm vị trí kỹ sư Front-end độc lập.

Mảng này đang ngày càng trở nên quan trọng khi nhiều nội dung, dữ liệu trực quan và tương tác người dùng phức tạp bắt buộc phải sử dụng các công nghệ đồ họa mới đem lại hiệu ứng tốt.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112518.jpg)

Thông thường, chúng ta chỉ gọi các thư viện đồ họa đã đóng gói sẵn mà ít khi chú ý đến các kỹ nghệ đồ họa bên dưới, chưa nói đến việc hiểu tường tận lý thuyết toán học và vật lý đằng sau nó.

Tuy nhiên, trước các yêu cầu tùy biến cao, tối ưu hiệu năng render và thiết kế giao diện mang hơi thở hiện đại, đồ họa máy tính là lĩnh vực mà một kỹ sư Front-end xuất sắc bắt buộc phải chạm tới. **Kỹ sư đồ họa là nhóm nhân sự Front-end được săn đón nhiều nhất và luôn nằm trong tình trạng khan hiếm tại các tập đoàn lớn.**

Hiện các khóa học đồ họa chất lượng trên thị trường là rất hiếm. Tuần này, chúng tôi giới thiệu khóa học **《Kỹ sư Front-end và Đồ họa máy tính》** do Kaikeba sản xuất. Khóa học được giảng dạy bởi Winter, cựu chuyên gia công nghệ Alibaba P8. Khóa học trị giá 199 tệ hiện được **chia sẻ miễn phí (0 tệ)** cho độc giả bản tin!

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112517.jpg)

Nội dung khóa học kéo dài 120 phút tập trung vào:
1. Mối liên hệ giữa Front-end và đồ họa máy tính, triển vọng nghề nghiệp của kỹ sư đồ họa.
2. Cách áp dụng kiến thức đồ họa vào dự án thực tế để tạo ra giá trị kinh doanh.
3. Hướng dẫn xây dựng hạ tầng kỹ thuật đồ họa phục vụ nâng cao trình độ chuyên môn.

Bạn có thể quét mã QR dưới đây để nhận khóa học hoàn toàn miễn phí (không yêu cầu chia sẻ hay giới thiệu):

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112516.jpg)

## Tin tức

1、[Hộp văn phòng làm việc tại nhà di động](https://www.oriliving.com/products/pocket-office)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111508.jpg)

Trong mùa dịch, nhiều người phải làm việc tại nhà nhưng không gian gia đình thường thiếu yên tĩnh hoặc không đủ chỗ bố trí phòng làm việc riêng. Để giải quyết vấn đề này, một startup Mỹ đã ra mắt hệ thống nội thất văn phòng di động thông minh.

Bình thường, hệ thống này đóng vai trò như hai chiếc tủ áp sát nhau để tiết kiệm diện tích phòng khách (hình trên). Khi cần làm việc, bạn chỉ cần điều khiển trượt mở tủ ra để tạo thành một không gian làm việc chuyên nghiệp biệt lập bên trong (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111509.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111510.jpg)

2、[Cầu Như Ý lơ lửng giữa không trung](https://www.twoeggz.com/info/845009.html)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111820.jpg)

Cuối tháng 9 vừa qua, cây cầu bộ hành Như Ý tại khu danh thắng Thần Tiên Cư, Thai Châu, Chiết Giang đã chính thức đón khách tham quan và nhanh chóng thu hút hơn 200.000 lượt khách trải nghiệm. Cầu dài 100 mét, bắc qua vách núi ở độ cao hơn 140 mét, có thiết kế uốn lượn uốn khúc gồm hai tầng đi bộ đan xen với các đoạn lát kính trong suốt chịu lực.

Nhìn từ trên cao xuống, cây cầu trông giống như một chiếc vương trượng như ý bằng ngọc bích khổng lồ nằm vắt ngang khe núi:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111818.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111821.jpg)

Nhìn từ phía bên hông, cầu lại mềm mại tựa như một dải lụa màu sắc mềm mại đung đưa giữa mây trời:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111822.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111819.jpg)

3、[Vụ kiện bắt buộc quét nhận diện khuôn mặt đầu tiên tại Trung Quốc](http://www.xinhuanet.com/2020-11/21/c_1126767913.htm)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112207.jpg)

Năm 2019, Công viên động vật hoang dã Hàng Châu đã nâng cấp hệ thống thẻ năm của khách hàng từ xác thực vân tay sang nhận diện khuôn mặt, yêu cầu tất cả hội viên phải quét mặt để vào cửa, nếu không thẻ sẽ bị khóa. Một khách hàng không đồng ý cung cấp dữ liệu sinh trắc học khuôn mặt và đã khởi kiện công viên ra tòa sau khi thương lượng bất thành.

Mới đây, tòa án nhân dân quận Phú Dương, Hàng Châu tuyên án sơ thẩm phần thắng thuộc về người tiêu dùng. Tuy nhiên, tòa án chỉ tuyên phạt công viên vi phạm hợp đồng dịch vụ đã ký trước đó chứ không phán quyết cấm các cơ sở kinh doanh bắt buộc thu thập thông tin khuôn mặt của khách hàng, gây nhiều thất vọng cho giới bảo vệ quyền riêng tư cá nhân.

4、[Kính thiên văn vô tuyến Arecibo huyền thoại chính thức bị tháo dỡ](https://www.sciencemag.org/news/2020/11/famed-arecibo-telescope-brink-collapse-will-be-dismantled)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112001.jpg)

Quỹ Khoa học Quốc gia Mỹ (NSF) thông báo sẽ tiến hành tháo dỡ kính thiên văn vô tuyến Arecibo tại Puerto Rico do công trình đã quá xuống cấp và việc sửa chữa tiềm ẩn nhiều rủi ro sập đổ nguy hiểm. Được khánh thành từ năm 1963, đây từng là kính thiên văn vô tuyến đơn đĩa lớn nhất thế giới trong suốt hơn nửa thế kỷ trước khi bị kính thiên văn FAST của Trung Quốc vượt qua vào năm 2016.

Cấu trúc của Arecibo gồm cụm thiết bị thu phát nặng 900 tấn treo lơ lửng ở độ cao 137 mét phía trên đĩa phản xạ rộng 305 mét. Do ảnh hưởng của bão nhiệt đới và động đất liên tục tại vùng biển Caribe, các sợi cáp thép gánh cụm thiết bị đã bị đứt gãy nghiêm trọng và cấu trúc tháp đỡ có nguy cơ đổ sập bất cứ lúc nào.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112002.jpg)

5、[Cơn khát đá khô toàn cầu phục vụ vận chuyển vaccine Covid-19](https://edition.cnn.com/2020/11/21/world/coronavirus-vaccine-dry-ice-intl/index.html)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112104.jpg)

Vaccine phòng Covid-19 của tập đoàn Pfizer sắp sửa được phân phối quy mô lớn trên toàn cầu. Tuy nhiên dòng vaccine này yêu cầu nhiệt độ bảo quản cực lạnh ở mức âm 70°C. Phương pháp làm lạnh kinh tế và dễ triển khai nhất là sử dụng đá khô (giúp duy trì nhiệt độ âm 78.5°C).

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112105.jpg)

Nhu cầu thu mua gom đá khô khẩn cấp tại nhiều quốc gia đang dẫn đến tình trạng khan hiếm nguồn cung. Đá khô vốn là phụ phẩm của quá trình sản xuất cồn ethanol công nghiệp, tuy nhiên do ảnh hưởng của dịch bệnh khiến sản lượng ethanol sụt giảm mạnh, gián tiếp bóp nghẹt nguồn cung đá khô của thị trường.

6、**Tin tức một câu**

> - [Quân đội Mỹ](https://www.bbc.com/news/technology-54465361) thử nghiệm trang bị kính thực tế ảo tăng cường AR chuyên dụng cho quân khuyển để người điều khiển từ xa có thể quan sát góc nhìn của chó và gửi các lệnh định hướng trực tiếp lên kính.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111908.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111909.jpg)

> - [Khu công nghệ cao Trương Giang, Thượng Hải](https://www.soyacincau.com/2020/11/18/kfc-autonomous-5g-restaurant-on-wheels-china/) đưa vào hoạt động các xe bán thức ăn tự hành 5G của KFC, khách hàng quét mã QR mở cửa tủ chọn đồ ăn và hệ thống tự động trừ tiền qua ví điện tử dựa trên trọng lượng hàng lấy ra.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111903.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111904.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111901.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111902.jpg)

> - [NASA](https://www.cnbc.com/2020/11/15/why-nasa-wants-to-put-a-nuclear-power-plant-on-the-moon.html) công bố kế hoạch hợp tác xây dựng một lò phản ứng hạt nhân nhỏ phát điện trên Mặt Trăng vào năm 2026.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112101.jpg)

> - [Tập đoàn Volvo](https://www.media.volvocars.com/global/en-gb/media/pressreleases/274379/watch-how-volvo-cars-drops-new-cars-from-30-metres-to-help-rescue-services-save-lives) thực hiện thử nghiệm thả rơi tự do 10 chiếc xe hơi mới từ độ cao 30 mét bằng cần cẩu để giả lập và đánh giá độ biến dạng khung gầm trong các va chạm giao thông cực đoan giúp đội cứu hộ huấn luyện kỹ năng cắt dỡ xe cứu người.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112006.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112007.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112008.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112009.jpg)

## Bài viết

1、[Các công cụ và dịch vụ tôi dùng để vận hành SaaS](https://jake.nyc/words/tools-and-services-i-use-to-run-my-saas/)（Tiếng Anh）

Tác giả chia sẻ chi tiết danh sách toàn bộ các dịch vụ cloud, framework frontend/backend và công cụ phân tích dữ liệu phục vụ vận hành sản phẩm SaaS cá nhân hiệu quả nhất.

2、[9 giai đoạn phát triển của một nhà duy trì dự án mã nguồn mở](https://nibblestew.blogspot.com/2020/11/the-nine-phases-of-open-source-project.html)（Tiếng Anh）

Một góc nhìn thực tế về hành trình tâm lý và công việc của lập trình viên duy trì dự án open-source lớn, trải qua 9 giai đoạn từ nhà phát minh ban đầu đầy hào hứng đến lúc chuyển giao dự án và nghỉ hưu trong danh dự.

3、[Trải nghiệm thực tế tham quan phòng thí nghiệm tiến trình chế tạo chip bán dẫn](https://www.coolapk.com/feed/22961813?shareKey=ZmFlODJiZmI1YzRhNWZjMmZhNGU)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112510.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112511.jpg)

Nhật ký của một sinh viên năm nhất ghi lại trải nghiệm chi tiết khi tham quan phòng sạch chế tạo bán dẫn, các thiết bị quang khắc và quy trình gia công wafer tại trường đại học.

4、[Cải tạo khu nhà cổ Tứ Hợp Viện Bắc Kinh thành trường mầm non độc đáo](https://www.gooood.cn/le-cheng-kindergarten-completed-mad.htm)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112512.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112513.jpg)

Văn phòng kiến trúc danh tiếng MAD thực hiện dự án cải tạo khu Tứ Hợp Viện cổ kính tại Bắc Kinh thành trường mầm non hiện đại cho 390 trẻ em với điểm nhấn là lối đi lợp thảm đỏ uốn lượn trên mái nhà nối liền cổ kính và hiện đại.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112514.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112515.jpg)

5、[Cách viết file Makefile dễ đọc và dễ bảo trì](https://www.thapaliya.com/en/writings/well-documented-makefiles/)（Tiếng Anh）

Hướng dẫn chi tiết các quy tắc thực hành tốt nhất để viết Makefile chuẩn hóa, dễ tra cứu và tự động hóa các tác vụ build dự án phần mềm một cách chuyên nghiệp.

6、[Tổng hợp các tính năng cú pháp mới của Java từ phiên bản 9 đến 15](https://advancedweb.hu/new-language-features-since-java-8-to-15/)（Tiếng Anh）

Bài viết tổng hợp các cải tiến cú pháp quan trọng nhất của Java qua các phiên bản phát hành từ Java 9 đến Java 15 giúp lập trình viên cập nhật kiến thức mới.

7、[Cách phát hiện hành vi chụp ảnh màn hình trong ứng dụng Android](https://proandroiddev.com/detect-screenshots-in-android-7bc4343ddce1)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111606.jpg)

Phương pháp và đoạn mã code đơn giản giúp các ứng dụng Android bảo mật ngăn chặn hoặc phát hiện khi người dùng thực hiện thao tác chụp màn hình điện thoại thông qua cơ chế lắng nghe thay đổi trong thư mục hình ảnh của hệ thống.

8、[Hướng dẫn chuyển đổi từ Docker sang sử dụng Podman](https://developers.redhat.com/blog/2020/11/19/transitioning-from-docker-to-podman/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112102.jpg)

Podman là công cụ quản lý container không cần daemon do RedHat phát triển nhằm thay thế Docker. Bài viết hướng dẫn cấu hình và chuyển đổi các câu lệnh quen thuộc sang công cụ mới.

9、[Tự viết trình thông dịch JavaScript bằng JavaScript](https://juejin.cn/post/6898093501376905230)（Tiếng Trung）

Giải thích chi tiết quy trình trình thông dịch phân tích mã nguồn JS thành cây cú pháp trừu tượng AST và thực thi mã nguồn đi kèm dự án ví dụ viết bằng JavaScript. ([@webfansplz](https://github.com/ruanyf/weekly/issues/1516) đóng góp)

## 工具

1、[Your First GitHub Commit](https://www.amitmerchant.com/your-first-commit-ever/)

Trang web thú vị giúp bạn tìm lại commit đầu tiên trong lịch sử sử dụng tài khoản GitHub cá nhân của mình.

2、[Perfect Dark Mode](https://perfect-dark-mode.netlify.app/)

Thư viện JavaScript gọn nhẹ giúp dễ dàng phát triển nút chuyển đổi qua lại chế độ giao diện sáng/tối (Dark Mode) cho trang web.

3、[rector](https://github.com/rectorphp/rector/)

Công cụ chuyển dịch mã nguồn PHP, hỗ trợ tự động convert code PHP phiên bản mới 8.x về dạng tương thích chạy được trên PHP 7.x tương tự vai trò của Babel đối với JavaScript.

4、[gping](https://github.com/orf/gping)

Công cụ thay thế lệnh ping truyền thống hiển thị kết quả phản hồi trễ mạng dưới dạng biểu đồ đồ họa trực quan ngay trên cửa sổ terminal.

5、[Edit CSV Online](https://www.editcsvonline.com/)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111403.jpg)

Trình chỉnh sửa trực tuyến các tệp tin dữ liệu định dạng CSV đơn giản, nhanh chóng.

6、[Logseq](https://github.com/logseq/logseq)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111407.jpg)

Ứng dụng ghi chú cá nhân nguồn mở bảo mật cao, hỗ trợ liên kết các ý tưởng dạng sơ đồ tri thức. Điểm cộng là toàn bộ dữ liệu ghi chú được lưu trữ trên kho chứa GitHub cá nhân của bạn, trang web không lưu bất kỳ thông tin nào của người dùng.

7、[Drumbit](https://drumbit.app/)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111601.jpg)

Ứng dụng trực tuyến giả lập bộ gõ trống giúp tạo các đoạn beat nhạc điện tử nhanh chóng.

8、[GitHub Pages URL Shortener](https://github.com/nelsontky/gh-pages-url-shortener)

Một ý tưởng độc đáo giúp bạn tự thiết lập một hệ thống rút gọn link tĩnh chạy hoàn toàn trên GitHub Pages mà không cần thuê máy chủ backend hay cơ sở dữ liệu.

9、[SVGOMG](https://jakearchibald.github.io/svgomg/)

Trình tối ưu hóa và nén dung lượng các tệp tin ảnh vector đồ họa SVG trực tuyến hiệu quả.

10、[Code with me](https://plugins.jetbrains.com/plugin/14896-code-with-me)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112501.jpg)

Plugin chính thức của JetBrains hỗ trợ tính năng làm việc nhóm code chung thời gian thực (collaborative programming) trực tiếp trên các IDE của hãng như IntelliJ IDEA. ([@dengshenkk](https://github.com/ruanyf/weekly/issues/1508) đóng góp)

## Tài nguyên

1、[Docker 指南](https://www.robertcooper.me/docker-guide)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111301.jpg)

Tài liệu hướng dẫn sử dụng Docker chi tiết cho người mới bắt đầu, giải thích rõ các khái niệm Container, Image, Volume, Network:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111302.jpg)

2、[Bảo tàng thiết bị lưu trữ dữ liệu lỗi thời](https://obsoletemedia.org/identify/)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111402.jpg)

Trang web tổng hợp và phân loại hình ảnh các phương tiện lưu trữ thông tin đã bị đào thải trong lịch sử phát triển máy tính như băng giấy đục lỗ, đĩa mềm các kích thước, băng từ cổ...

3、[Play with Go](https://play-with-go.dev/guides.html)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111404.jpg)

Trang web cung cấp chuỗi bài giảng tự học lập trình ngôn ngữ Go thông qua các bài tập thực hành gõ code chạy thử trực tiếp trên trình duyệt.

4、[互联网围棋数据库](http://iwdb.cn/)

Cơ sở dữ liệu lưu trữ phong phú các kỳ phổ cờ vây trực tuyến, hỗ trợ tìm kiếm theo tên kỳ thủ và tải tệp tin định dạng SGF về máy. ([@yujiff](https://github.com/ruanyf/weekly/issues/1223) đóng góp)

5、[Linux 命令大全](https://www.yuque.com/books/share/742ca8f6-34f3-41ef-b239-be00aaf0df31)

Tài liệu tra cứu tiếng Trung chi tiết tổng hợp các dòng lệnh Linux đi kèm ví dụ cú pháp cụ thể. ([@1228857713](https://github.com/ruanyf/weekly/issues/1225) đóng góp)

6、[《编程之道》中英双语版](https://github.com/yikeke/tao-of-programming)

Bản dịch song ngữ Anh-Trung tác phẩm kinh điển "The Tao of Programming" xuất bản năm 1987 của tác giả Geoffrey James, chứa đựng nhiều câu chuyện ngụ ngôn hài hước châm biếm về triết lý viết code của lập trình viên. ([@yikeke](https://github.com/ruanyf/weekly/issues/1513) đóng góp)

## Hình ảnh

1、**Tác phẩm ảnh chụp xuất sắc năm 2020**

Bức ảnh đạt giải cuộc thi ảnh chụp cận cảnh [Close-up Photographer of the Year](https://www.theatlantic.com/photo/2020/11/winners-close-up-photographer-year/617070/): Frost phủ trắng trên mũ nấm trong buổi sớm mùa đông:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111303.jpg)

Chú kiến đen đang nỗ lực vận chuyển các kén trứng của loài bướm đêm:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111304.jpg)

Tác phẩm tham gia giải ảnh thời tiết [Weather Photographer of the Year](https://www.rmets.org/wpoty-2020-shortlist): Cảnh hạn hán nghiêm trọng tại Bangladesh:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111305.jpg)

Mặt băng hồ Baikal ánh lên sắc xanh ngọc bích dưới ánh mặt trời mùa đông:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111306.jpg)

Hiện tượng mây thềm lớn cuộn tròn như một chiếc nồi úp khổng lồ trên bầu trời Croatia:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111308.jpg)

2、[Sự tiến hóa đồ họa game bóng rổ NBA 2K14 và NBA 2K21](https://twitter.com/BleacherReport/status/1327119782815129601/)

Sự thay đổi về độ chi tiết khuôn mặt và đổ bóng vật lý của các cầu thủ sau 7 năm phát triển công nghệ đồ họa game:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111602.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111603.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111604.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111605.jpg)

3、[Xu hướng tỷ lệ sinh con toàn cầu sụt giảm](https://www.reddit.com/r/dataisbeautiful/comments/gl6f35/oc_falling_fertility_around_the_world_100_years/fqvir2k/)

Biểu đồ thống kê tỷ lệ sinh con của các quốc gia từ năm 1900 đến 2016. Đường kẻ ngang ở giữa đại diện cho mức sinh thay thế (2.05) để duy trì quy mô dân số. Số liệu cho thấy tỷ lệ sinh toàn cầu liên tục giảm sâu trong 100 năm qua, đồng nghĩa dân số thế giới có thể sẽ đi vào giai đoạn thu hẹp trong tương lai chứ không bùng nổ vô hạn.

1900:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112003.jpg)

2016:

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112004.jpg)

## Bài đọc thêm

### 1. Hormone Leptin và tuổi dậy thì

*Tác giả: Bill Bryson (Trích cuốn sách 《Cơ thể: Hướng dẫn cho người sử dụng》)*

Trong suốt quá trình tiến hóa lâu dài của nhân loại, cơ thể chúng ta luôn quen với trạng thái thiếu thốn thực phẩm và nạn đói rình rập, lịch sử chưa bao giờ có giai đoạn dư thừa thức ăn kéo dài. Do đó, cơ thể con người không hề tiến hóa ra bất kỳ cơ chế sinh học nào để nhắc nhở chúng ta khi nào nên chủ động ngừng ăn.

Đó là lý do chúng ta có xu hướng thèm ăn và ăn quá mức cần thiết một khi có sẵn thức ăn ngon, vì cơ thể luôn muốn tích trữ năng lượng dự phòng cho những lúc đói kém.

Năm 1995, các nhà khoa học đã phát hiện ra hormone **Leptin** có vai trò kích hoạt quá trình giải phóng và tiêu thụ mỡ thừa của cơ thể.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112502.jpg)

Cụ thể hơn, Leptin làm nhiệm vụ báo hiệu cho não bộ biết cơ thể đã tích lũy đủ nguồn năng lượng dự trữ để sẵn sàng bước vào các giai đoạn thay đổi sinh học quan trọng và tiêu tốn năng lượng như mang thai hoặc bắt đầu bước vào tuổi dậy thì. Nếu thiếu hụt lượng Leptin cần thiết, các quá trình này sẽ bị trì hoãn khởi động. Đây là nguyên nhân vì sao những thanh thiếu niên mắc chứng biếng ăn/suy dinh dưỡng thường có tuổi dậy thì đến rất muộn.

Trong các thế kỷ trước, con người thường bước vào tuổi dậy thì ở độ tuổi 16-17. Ngày nay thì khác, tuổi dậy thì bắt đầu sớm hơn bất kỳ giai đoạn nào trong lịch sử, thường là từ năm 11 tuổi. Nguyên nhân chủ chốt chắc chắn là do điều kiện dinh dưỡng được cải thiện vượt bậc, lượng mỡ cơ thể tăng giúp hormone Leptin tiết ra sớm hơn, phát tín hiệu cho não bộ kích hoạt tuổi dậy thì từ rất sớm.

### 2. Thuế Apple Tax 30% trên App Store

*Tác giả: John Luxford*

Kể từ khi máy tính cá nhân ra đời, các lập trình viên luôn có quyền tự do phân phối phần mềm trực tiếp tới tay người dùng. Chưa bao giờ có một tổ chức trung gian nào đứng ra phán quyết phần mềm nào được phân phối, phần mềm nào bị cấm; và càng không có việc bắt ép lập trình viên phải cắt nộp một phần lớn doanh thu cho họ.

Dòng máy chơi game console (như PlayStation, Xbox) là một ngoại lệ do các hãng sản xuất thiết bị đóng vai trò kiểm soát nội dung đưa lên máy, nhưng đó là các thiết bị phần cứng chuyên dụng chạy hệ sinh thái đóng. Máy tính cá nhân thì khác, nó luôn là một hệ sinh thái mở hỗ trợ tối đa cho sự sáng tạo công nghệ.

Tuy nhiên từ khi chợ ứng dụng iPhone App Store xuất hiện, mọi thứ đã thay đổi. Phần mềm chỉ được phép phân phối trên iPhone nếu được Apple phê duyệt, đi kèm khoản phí duy trì nhà phát triển 99 USD/năm và Apple sẽ tự động thu chiết khấu 30% trên mọi doanh thu phát sinh của ứng dụng. Để so sánh, phí giao dịch thẻ tín dụng thông thường tại Mỹ chỉ khoảng 2.9% + 0.30 USD cho mỗi giao dịch.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112304.jpg)

Mức thuế 30% này thực chất được Apple sao chép từ mô hình ăn chia của các hãng máy console. Apple lập luận rằng iPhone là thiết bị đóng chuyên dụng để nghe gọi nên cần kiểm soát chặt chẽ để bảo vệ an toàn cho người dùng trước các mã độc hại. Do đó mức phí 30% là hợp lý để trang trải chi phí kiểm duyệt ứng dụng.

Sau đó, Google cũng áp dụng mức phí tương tự cho kho ứng dụng Play Store của Android và mô hình này nhanh chóng được nhân rộng ra từ Steam đến các kho ứng dụng của Samsung.

Hiện nay, hệ điều hành máy tính như Windows và macOS cũng đang dần tích hợp các chợ ứng dụng riêng, tiến tới kiểm soát và cảnh báo người dùng khi cài đặt các phần mềm tải từ nguồn ngoài không qua kiểm duyệt của hãng, đe dọa nghiêm trọng đến quyền tự do phân phối mã nguồn của nhà phát triển.

Chúng ta cần có các biện pháp pháp lý mạnh mẽ từ chính phủ để bảo vệ thị trường mở trước các hành vi độc quyền của các tập đoàn công nghệ lớn. Điện thoại thông minh ngày nay thực chất là những chiếc máy tính cá nhân bỏ túi, nó là thiết bị tính toán đa dụng chứ không phải là thiết bị nghe gọi chuyên dụng đóng kín. Việc đóng kín hệ sinh thái này chỉ mang lại lợi nhuận khổng lồ cho nhà sản xuất thiết bị chứ không mang lại lợi ích thực chất cho người dùng và các nhà phát triển.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112305.jpg)

Năm 2019, App Store mang về doanh thu khoảng 50 tỷ USD và Apple đút túi khoảng 15 tỷ USD tiền phí chiết khấu. Chúng ta cần đặt câu hỏi liệu chi phí vận hành và kiểm duyệt một kho ứng dụng có thực sự tốn kém đến mức đó hay đây chỉ là một khoản thuế độc quyền áp lên người dùng?

## 言论

1、

Mô hình cất cánh kinh tế của Trung Quốc thực chất kế thừa từ mô hình phát triển của Mỹ, vốn đã được Nhật Bản và bốn con rồng châu Á áp dụng thành công đi trước, và Trung Quốc đã học hỏi, điều chỉnh lại cho phù hợp với quy mô của mình.

-- Độc giả Hacker News

2、

Trình duyệt web ban đầu được thiết kế chỉ để xem tài liệu tĩnh từ xa, nhưng sau đó bị ép phải gánh vác vai trò làm nền tảng chạy các ứng dụng web phức tạp. Do cấu trúc ban đầu không được thiết kế cho mục đích này nên phần lớn các vấn đề lỗi bảo mật và hiệu năng trên Internet hiện nay đều bắt nguồn từ sự thiếu đồng bộ đó.

-- Báo cáo Xu hướng công nghệ ThoughtWorks (10/2020)

3、

Sau khi hoàn thành công việc chính tại công ty, mỗi tối tôi đều dành thêm 4 đến 5 tiếng để viết code phát triển Bootstrap. Tôi không dám nhận lời đi ăn tối với bạn bè vì luôn có cảm giác tội lỗi rằng mình đang làm người dùng thất vọng: Thay vì ra ngoài đi chơi, đáng lẽ ra tôi phải ngồi gõ code cống hiến cho dự án Bootstrap!

-- Jacob Thornton, một trong hai nhà sáng lập của CSS framework Bootstrap chia sẻ về áp lực tâm lý của người duy trì dự án mã nguồn mở suốt 9 năm.

4、

Chúng tôi quyết định tự bỏ vốn nghiên cứu vaccine phòng Covid-19 mà không nhận tiền tài trợ từ chính phủ. Bởi vì các khoản tiền đó luôn đi kèm các điều khoản báo cáo tiến độ phiền hà làm phân tán sự tập trung. Tôi muốn các nhà khoa học của mình dồn 100% tâm trí vào chuyên môn sản xuất vaccine thay vì lo lắng viết các báo cáo tiến độ.

-- CEO tập đoàn dược phẩm Pfizer

5、

Để mắt người không cảm nhận được các hạt pixel li ti trên màn hình khi nhìn ở cự ly gần, mật độ điểm ảnh của màn hình bắt buộc phải vượt quá giới hạn phân giải của mắt người, tức là lớn hơn 285 PPI (pixel per inch). Màn hình 4K thông thường không đạt mức này (một màn hình 27 inch 4K chỉ đạt 163 PPI). Trên thị trường hiện nay chỉ có dòng màn hình 5K của máy iMac 27 inch là tiệm cận giới hạn này với mật độ điểm ảnh đạt 220 PPI.

-- Bài viết 《Cách tự chế khung ảnh kỹ thuật số độ phân giải siêu cao》

6、

Rất nhiều người coi tranh luận là một cuộc chiến phân định thắng thua để thỏa mãn cái tôi cá nhân. Thực chất, tranh luận nên được coi là một hành vi hợp tác giữa hai bên để cùng nhau tìm ra chân lý của vấn đề.

-- Sách 《Cẩm nang tranh luận mang tính xây dựng》

## Nhìn lại

Tuần này năm 2019 (số 84): [Mô hình tuyển dụng một lần: dùng xong là bỏ](http://www.ruanyifeng.com/blog/2019/11/weekly-issue-84.html)

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111702.jpg)

Tuần này năm 2018 (số 32): [Ba góc nhìn của người thợ xây gạch](http://www.ruanyifeng.com/blog/2018/11/weekly-issue-32.html)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018112301.jpg)

## Đăng ký

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97).

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
