# 科技爱好者周刊：第 94 期 (Bản tin chia sẻ công nghệ số 94)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

Mục tuyển dụng [《Ai đang tuyển dụng?》](https://github.com/ruanyf/weekly/issues/983) cung cấp nhiều thông tin việc làm hữu ích, hoan nghênh ghé thăm hoặc đăng tải thông tin tuyển dụng/thực tập.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019113001.jpg)

Ảnh bìa: Thùng rác hút chân không tự động nén đóng gói rác và vận chuyển qua đường ống ngầm dưới lòng đất về trạm thu gom tập trung. Ảnh từ [Wikipedia](https://en.wikipedia.org/wiki/Automated_vacuum_collection).

## 刊首语 (Lời tựa)

Nhà đầu tư mạo hiểm nổi tiếng vùng Silicon Valley [Naval](https://nav.al/build-sell) vừa đăng tải một câu nói kinh điển trên mạng xã hội thu hút hàng vạn lượt tương tác.

**Anh viết: "Nếu bạn vừa am hiểu quy trình sản xuất (build) lại vừa thành thạo kỹ năng bán hàng (sell), bạn sẽ là người bất khả chiến bại."**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121301.jpg)

Ý của Naval là một doanh nghiệp muốn gặt hái thành công vượt bậc bắt buộc phải đồng thời sở hữu hai năng lực cốt lõi: năng lực sản xuất xuất sắc và năng lực bán hàng xuất sắc. Một doanh nghiệp giỏi không chỉ dừng lại ở việc tạo ra các sản phẩm công nghệ tuyệt vời, mà còn phải biết cách đưa sản phẩm đó tiếp cận và thuyết phục người tiêu dùng chi tiền.

Đây cũng là lý do vì sao trong sơ đồ tổ chức của các công ty công nghệ luôn song hành hai vai trò CEO và CTO. Thông thường, CEO sẽ chịu trách nhiệm chính về mảng kinh doanh bán hàng (bao gồm cả gọi vốn đầu tư) và quản trị vận hành, còn CTO sẽ tập trung tối đa vào mảng thiết kế sản phẩm và kỹ thuật sản xuất. Chỉ cần một trong hai vai trò này làm không tốt, doanh nghiệp rất khó có thể đi tới thành công cuối cùng.

Naval chia sẻ thêm: **Trên thế giới này, những cá nhân kiệt xuất nhất chính là những người vừa có thể tự tay viết code chế tạo sản phẩm, vừa có thể đứng ra thuyết phục khách hàng mua sản phẩm đó.** Những con người này có đủ năng lực để tự định hình nên một ngành công nghiệp mới. Tiêu biểu là tỷ phú Elon Musk - người vừa hiểu biết sâu sắc về kỹ thuật cơ khí vũ trụ để định hướng các kỹ sư chế tạo tên lửa và xe điện Tesla, vừa sở hữu tài năng bán hàng thiên bẩm khiến cả thế giới phát cuồng vì thương hiệu của mình. Hay huyền thoại Steve Jobs, người thấu hiểu sâu sắc mong muốn ẩn giấu của khách hàng để dẫn dắt Apple chế tạo nên những thiết bị làm thay đổi lịch sử công nghệ.

Nếu chúng ta coi cuộc đời của chính mình là một dự án khởi nghiệp độc lập, thì công thức thành công cũng tương tự như vậy: bạn vừa phải rèn luyện năng lực chuyên môn thực chất (make), vừa phải học cách tiếp thị và định vị bản thân hiệu quả trước xã hội (sell).

Naval nhận định rằng thông thường các nhà chế tạo (Maker) học kỹ năng bán hàng sẽ dễ dàng hơn nhiều so với việc một nhân viên bán hàng (Sales) bắt đầu học kỹ năng lập trình hay chế tạo kỹ thuật. Do đó, lời khuyên dành cho các bạn trẻ là khi học đại học, tốt nhất nên chọn các ngành học chuyên sâu về chế tạo kỹ thuật (như khoa học máy tính) làm chuyên ngành chính, và học thêm các môn học về kinh tế thương mại làm ngành phụ trợ. Sự kết hợp này sẽ tạo ra bệ phóng sự nghiệp vô cùng vững chắc.

## Khóa học chuyên đề phỏng vấn: "Làm chủ nguyên lý trình duyệt qua 3 bước"

Năm 2020 sẽ là một năm đầy thách thức cho hoạt động tuyển dụng ngành công nghệ. Nhằm giúp các bạn tự học phát triển Frontend chuẩn bị tốt nhất cho các kỳ phỏng vấn tuyển dụng sau mùa dịch, bản tin giới thiệu khóa học chuyên đề: **《Bí quyết phỏng vấn: Làm chủ nguyên lý hoạt động của trình duyệt web qua 3 bước》**.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021202.jpg)

Trình duyệt là môi trường chạy (runtime) cốt lõi của mọi ứng dụng Frontend. Chỉ khi thấu hiểu tường tận cấu trúc cơ học bên dưới và nguyên lý hiển thị của trình duyệt, lập trình viên mới có thể tối ưu hóa hiệu năng hiển thị trang web tốt nhất. Nội dung khóa học tập trung làm rõ:

> (1) Cấu trúc hệ thống và nguyên lý trình duyệt: Kiến trúc đa tiến trình (multi-process), quy trình xử lý giao thức TCP/UDP, chu kỳ yêu cầu HTTP và quy trình dựng trang Render Pipeline.
> 
> (2) Cơ chế thực thi JavaScript và động cơ V8: Variable Hoisting, Call Stack, Prototype Chain, quy trình biên dịch và thông dịch, cơ chế dọn rác bộ nhớ (Garbage Collection), Event Loop, Promise, Async/Await.
> 
> (3) Tối ưu hóa trang web và an ninh bảo mật: Khái niệm Virtual DOM, tối ưu hiệu năng hiển thị, chính sách đồng nguồn gốc (Same-Origin Policy), phòng chống tấn công XSS và XSRF.

Giảng viên trực tiếp đứng lớp là thầy Đổng - hiện là kỹ sư Frontend cấp cao tại tập đoàn công nghệ lớn và cũng là người trực tiếp tham gia chấm điểm phỏng vấn ứng viên. Thầy sẽ chia sẻ các bộ câu hỏi phỏng vấn thực tế từ các doanh nghiệp lớn và kinh nghiệm ứng tuyển thực chiến.

Chương trình được tổ chức bởi trung tâm đào tạo công nghệ Jingcheng Yideng tại Bắc Kinh - đơn vị liên kết chất lượng cao cùng Tencent Classroom.

Khóa học chuyên đề chính thức khai giảng vào thứ Ba tuần tới (18/2). Độc giả bản tin quét mã QR dưới đây để nhận mã ưu đãi, **giảm giá học phí cho 88 học viên đăng ký sớm nhất chỉ còn 1 Nhân dân tệ**:

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021201.jpg)

## 资讯 (Tin tức)

1. **MBC Hàn Quốc sản xuất phim tài liệu ứng dụng VR tái dựng hình ảnh con gái đã khuất**

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021115.jpg)

Đài truyền hình MBC của Hàn Quốc vừa phát sóng bộ phim tài liệu đầy xúc động mang tên *Gặp lại con*, ghi lại hành trình một đội ngũ kỹ sư công nghệ phối hợp cùng người mẹ mất con để tái dựng hình ảnh cô con gái nhỏ đã qua đời thông qua công nghệ thực tế ảo VR.

3 năm trước, bé Nayeon (7 tuổi) qua đời đột ngột vì căn bệnh ung thư máu để lại nỗi đau vô hạn cho người mẹ Jang Ji-sung. Một công ty phát triển VR tại Hàn Quốc đã dành hơn 8 tháng nghiên cứu, thu thập hình ảnh, giọng nói của bé để dựng lại mô hình 3D tương tác. Người mẹ đeo thiết bị kính VR để gặp lại con gái trong không gian công viên ảo, trò chuyện trực tiếp và cùng tổ chức một bữa tiệc sinh nhật muộn đầy nước mắt cho con trước khi tiễn bé hóa thành những đốm sáng bay đi.

2. **Các nhà nghiên cứu Anh ứng dụng công nghệ in 3D tái tạo giọng nói của xác ướp Ai Cập cổ đại**

Nesyamun là một vị tư tế và người chép kinh nổi tiếng sống dưới thời Ai Cập cổ đại (khoảng năm 1100 trước Công nguyên). Mẫu xác ướp của ông được tìm thấy từ thế kỷ 19 và đang được bảo tồn tại bảo tàng nước Anh.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020012604.jpg)

Mới đây, các nhà nghiên cứu đã tiến hành chụp cắt lớp vi tính CT toàn bộ vùng cổ họng của xác ướp để dựng lại mô hình 3D cấu trúc thanh quản, sau đó tiến hành in 3D thanh quản nhân tạo này. Khi kết hợp cùng hệ thống tổng hợp âm thanh điện tử, các chuyên gia đã có thể phát ra âm thanh giọng nói của vị tư tế này sau hơn 3.000 năm yên nghỉ.

Công nghệ này vốn được nghiên cứu phát triển để tái tạo giọng nói cho các bệnh nhân bị tổn thương thanh quản nặng sau tai nạn hoặc phẫu thuật ung thư vòm họng.

3. **Lốp xe không hơi (Airless Tires) sắp sửa đưa vào ứng dụng thực tế trên xe đạp**

Hãng sản xuất lốp xe hàng đầu Nhật Bản Bridgestone giới thiệu công nghệ lốp xe không cần bơm hơi. Cấu trúc bên trong lốp được dệt bằng các sợi polymer nhựa nhiệt dẻo có khả năng chịu lực nén cực tốt lên tới 2.2 tấn, đáp ứng được nhu cầu tải trọng của xe tải.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020012406.jpg)

Lốp xe không hơi loại bỏ hoàn toàn rủi ro xẹp lốp, nổ lốp hay đinh cắm khi di chuyển. Nhược điểm lớn nhất là độ đàn hồi hấp thụ xung lực kém hơn lốp khí nén thông thường, tạo cảm giác xóc hơn khi đi qua đường xấu. Bridgestone tuyên bố sẽ sớm bán thương mại các dòng xe đạp trang bị loại lốp không hơi thế hệ mới này.

4. **Hãng Airbus thử nghiệm thành công máy bay hành khách A350 cất cánh tự động không người lái**

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011904.jpg)

Vào tháng 12/2019, tập đoàn hàng không Airbus đã thực hiện thành công chuyến bay thử nghiệm cất cánh tự động trên dòng máy bay thân rộng A350 tại sân bay Toulouse (Pháp). Khi máy bay di chuyển vào đường băng cất cánh, hệ thống lái tự động sẽ tiếp quản toàn bộ quá trình tăng tốc, tự động điều chỉnh hướng di chuyển thẳng theo vạch sơn trung tâm nhờ hệ thống camera nhận diện gắn trên thân và nâng mũi máy bay cất cánh.

Phi công lái chính vẫn ngồi trong cabin giám sát nhưng hoàn toàn không chạm vào cần điều khiển, chỉ đóng vai trò quan sát đề phòng sự cố kỹ thuật xảy ra để tiếp quản thủ công. Vì công nghệ bay tự động trên không và hạ cánh tự động (Autoland) vốn đã rất hoàn thiện, việc làm chủ quy trình cất cánh tự động sẽ mở đường cho các dòng máy bay chở khách tự hành hoàn toàn trong tương lai gần.

5. **Thiết bị khóa kính chắn gió phạt đỗ xe trái phép Barnacle của Mỹ**

Hệ thống bãi đỗ xe của Đại học Oklahoma bắt đầu thử nghiệm thiết bị phạt đỗ xe trái phép mang tên Barnacle (Con Hà biển). Đây là sản phẩm thiết kế thông minh của một startup để thay thế cho việc khóa bánh xe hay cẩu xe truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020011801.jpg)

Khi phát hiện phương tiện vi phạm đỗ quá giờ hoặc không nộp phí, nhân viên quản lý sẽ đặt tấm nhựa màu vàng lớn này lên kính chắn gió trước của xe. Hệ thống giác hút chân không cực mạnh bên trong sẽ bám chặt vào kính với lực hút khổng lồ không thể gỡ ra bằng tay. Tài xế bắt buộc phải quét mã QR trên tấm nhựa để nộp tiền phạt trực tuyến, sau đó hệ thống sẽ cấp mã số để mở khóa gỡ thiết bị. Nếu cố tình lái xe đi khi tầm nhìn bị che khuất, thiết bị tích hợp cảm biến gia tốc sẽ liên tục rú còi báo động.

6. **Tin vắn**

- Cơ quan Cấp bằng Sáng chế Châu Âu (EPO) bác bỏ đơn đăng ký bằng sáng chế cho một thiết kế hộp nhựa do thuật toán trí tuệ nhân tạo tự động thiết kế, khẳng định chủ thể nộp bằng sáng chế bắt buộc phải là con người.

- Steve Wozniak - nhà đồng sáng lập huyền thoại của Apple - gây chú ý khi đeo chiếc đồng hồ hiển thị bằng bóng đèn chân không cổ độc đáo. Thiết bị tiêu thụ điện năng cực lớn nên chỉ sáng đèn khi nâng cổ tay xem giờ.

- Na Uy ghi nhận năm 2019 thủ đô Oslo không có bất kỳ người đi bộ hay đi xe đạp nào tử vong vì tai nạn giao thông, nhờ chính sách cấm xe cơ giới vào trung tâm và giới hạn tốc độ tối đa 30 km/h ở các khu vực khác.

## 文章 (Bài viết)

1、[Bài viết] [Tìm hiểu về phong trào nghỉ hưu sớm FIRE (Financial Independence, Retire Early)](https://en.wikipedia.org/wiki/FIRE_movement) (Tiếng Anh)

Trang tổng hợp thông tin về trào lưu sống tiết kiệm tối đa để tự chủ tài chính và nghỉ hưu sớm: phương pháp cốt lõi là nỗ lực tiết kiệm trên 50% tổng thu nhập hàng tháng và đầu tư tích lũy tài sản cho tới khi đạt mốc quy tắc 4% (quỹ đầu tư bằng 25 lần chi tiêu năm).

2、[Bài viết] [Giải pháp quét mã QR kết nối nhanh mạng WiFi tự động trên thiết bị di động](https://feeding.cloud.geek.nz/posts/encoding-wifi-access-point-passwords-qr-code/) (Tiếng Anh)

Hướng dẫn cách mã hóa thông tin tên mạng SSID, mật khẩu và giao thức bảo mật của bộ phát WiFi thành định dạng mã QR tiêu chuẩn bằng công cụ dòng lệnh `qrencode` của Linux để người dùng quét kết nối nhanh không cần nhập tay mật khẩu.

3、[Bài viết] [Chia sẻ về mô hình dịch vụ in 3D công nghiệp giá siêu rẻ tại Đông Quan](https://www.zhihu.com/question/50594957/answer/949100875) (Tiếng Trung)

Bài viết phân tích thực trạng chuỗi cung ứng in 3D công nghiệp tại khu vực Thâm Quyến/Đông Quan: lý giải nguyên nhân vì sao các xưởng gia công lớn tại đây có thể cung cấp dịch vụ in 3D với giá thành rẻ đến mức kinh ngạc (chỉ từ 1 Tệ/gram sản phẩm) nhờ tối ưu hóa công suất chạy máy 24/7 liên tục và chia sẻ hao mòn khuôn dùng chung.

## 软件 (Phần mềm)

1、[age — Công cụ dòng lệnh hỗ trợ mã hóa và giải mã tệp tin an toàn tốc độ cao](https://github.com/FiloSottile/age)

Thiết kế tối giản thay thế cho hệ thống GPG phức tạp, hỗ trợ các nhà phát triển mã hóa tệp tin nhanh chóng bằng các cặp khóa public/private key hoặc mật khẩu thông thường với thuật toán mã hóa hiện đại.

2、[tauri — Thư viện hỗ trợ đóng gói ứng dụng desktop đa nền tảng bằng Rust và Webview](https://github.com/tauri-apps/tauri)

Giải pháp thay thế cho Electron siêu nhẹ: sử dụng ngôn ngữ Rust cho phần lõi logic hệ thống và tận dụng trực tiếp bộ dựng Webview có sẵn của hệ điều hành (WebKit trên macOS, WebView2 trên Windows) giúp file cài đặt siêu nhỏ gọn (chỉ vài MB) và tiết kiệm RAM tối đa.

## 资源 (Tài nguyên)

1、[Tài liệu] [Waking-Up - Tổng hợp tài liệu chuẩn bị phỏng vấn kỹ thuật Backend dành cho sinh viên](https://github.com/wolverinn/Waking-Up)

Kho lưu trữ GitHub tổng hợp chi tiết các kiến thức cốt lõi phục vụ phỏng vấn kỹ sư Backend: từ kiến thức mạng máy tính, hệ điều hành, cơ sở dữ liệu cho tới cấu trúc dữ liệu và thuật toán thực chiến.

## 图片 (Hình ảnh)

1. **Bản dịch lịch sử giải mã cuộn kinh Phật Gandhara mỏng manh nhất thế giới**

Hình ảnh ghi lại quy trình nghiệp vụ phục dựng và số hóa cuộn kinh Phật viết trên vỏ cây bạch dương niên đại hơn 2.000 năm được phát hiện nguyên vẹn trong một陶 hũ cổ tại Afghanistan của các chuyên gia Thư viện Quốc hội Mỹ.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121319.jpg)

Do vỏ cây cực kỳ giòn và dễ vỡ vụn trước hơi thở của con người, các chuyên gia phải tiến hành dưỡng ẩm làm mềm trong phòng thí nghiệm chuyên dụng suốt nhiều tuần, sử dụng các dụng cụ vi phẫu tinh xảo để trải phẳng từng lớp vỏ cây trước khi tiến hành dịch nghĩa thành công hơn 80% văn bản cổ.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121320.jpg)

## 文摘 (Văn trích)

1. **Giả thuyết về sự tuyệt chủng của 8 loài người cổ đại khi chạm trán tổ tiên Homo Sapiens**

Khoảng 30 vạn năm trước, trái đất là ngôi nhà chung của ít nhất 9 loài người cổ đại sinh sống rải rác: người Neanderthal ở Châu Âu, người Denisovan ở Châu Á, người Homo Erectus ở Indonesia, người Homo Sapiens ở Nam Phi, và một số loài người lùn khác trên các đảo biệt lập.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021204.jpg)

Thế nhưng đến mốc 1 vạn năm trước, ngoại trừ tổ tiên loài người hiện đại Homo Sapiens chúng ta, toàn bộ 8 loài người cổ đại còn lại đều hoàn toàn biến mất khỏi bản đồ sinh học thế giới. Đáng lưu ý là giai đoạn này không hề ghi nhận các thảm họa thiên thạch hay núi lửa phun trào quy mô lớn toàn cầu. Tác nhân lớn nhất dẫn tới sự tuyệt chủng hàng loạt này chính là làn sóng di cư mở rộng địa bàn hoạt động ra khỏi Châu Phi của người Homo Sapiens.

Nhờ sở hữu năng lực ngôn ngữ phức tạp và tư duy hợp tác cộng đồng quy mô lớn vượt trội, người Homo Sapiens nhanh chóng trở thành loài săn mồi đỉnh bảng không có thiên địch. Làn sóng dân số bùng nổ thúc đẩy nhu cầu chiếm lĩnh đất đai canh tác và nguồn thức ăn, dẫn tới các cuộc đụng độ sinh tồn không thể tránh khỏi giữa các bộ tộc. Các loài người cổ khác dần bị đẩy vào thế yếu, mất nguồn thức ăn và dần bị xóa sổ hoàn toàn khỏi lịch sử tiến hóa.

## 言论 (Danh ngôn)

1、

> "Mã nguồn của hệ cơ sở dữ liệu SQLite được quản lý hoàn toàn trên hệ thống Fossil và chúng tôi cam kết sẽ không bao giờ chuyển dịch sang Git. Fossil được thiết kế chuyên biệt để phục vụ hoàn hảo cho quy trình phát triển của SQLite, hướng tới một phân khúc thị trường công cụ quản lý phiên bản hoàn toàn khác biệt so với Git hay GitHub."
> 
> -- Chia sẻ của D. Richard Hipp - cha đẻ của SQLite và Fossil

(Hết)
