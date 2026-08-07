# 科技爱好者周刊（第 174 期）：全能程序员 vs 特长程序员

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1913) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090117.jpg)

Nhà ga của Trung tâm vận chuyển hành khách Phổ Đà Sơn, tỉnh Chiết Giang mới đây đã vinh dự giành giải thưởng kiến trúc Versailles 2021 (Prix Versailles). (Nguồn: [Zshid](http://www.zshid.com/?c=building&a=view&id=4499))

## 主带话题：Lập trình viên đa năng (Full-stack) vs Lập trình viên chuyên sâu (Specialist)

Tôi từng đọc một số báo cáo thể thao về bóng rổ, trong đó viết rằng các đội bóng tại giải nhà nghề Mỹ NBA không thực sự mặn mà với các "cầu thủ đa năng", thay vào đó họ ưa chuộng những "cầu thủ có sở trường đặc biệt" (specialist).

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090115.jpg)

Khái niệm "cầu thủ sở trường" ám chỉ những người có thể chơi mờ nhạt ở nhiều khía cạnh khác, nhưng lại có một kỹ năng cực kỳ xuất sắc vượt trội, chẳng hạn phòng ngự siêu việt, ném 3 điểm cực kỳ chuẩn xác, hoặc tranh chấp bóng bật bảng (rebounds) rất mạnh. Ban huấn luyện luôn muốn sở hữu những cầu thủ này để tung vào sân ở các thời điểm quyết định của trận đấu nhằm tạo nên bước ngoặt đột phá.

Ngược lại, các "cầu thủ đa năng" có bộ chỉ số kỹ thuật rất cân bằng: phòng ngự tốt, tấn công ổn, ném bóng khá, đạt mức trung bình chung của giải nhưng không sở hữu bất kỳ kỹ năng nào đạt tới mức kiệt xuất vượt trội. Các đội bóng lớn ít khi đánh giá cao nhóm này do cảm thấy họ không đủ sắc bén để tự xoay chuyển trận đấu giành chiến thắng.

Tôi lập tức liên tưởng đến thực tế của ngành phát triển phần mềm: **Cơ hội thăng tiến của các lập trình viên đa năng thực tế lại kém xa so với các lập trình viên đi sâu chuyên môn hóa.**

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090116.jpg)

Nếu bạn là người cái gì cũng biết làm một chút, từ Front-end, Back-end, quản trị cơ sở dữ liệu đến quản lý server, bạn sẽ là người được chỉ định đắp vào bất kỳ khoảng trống nhân sự nào khi dự án thiếu người. Tuy nhiên, khi hệ thống gặp các lỗi nghiêm trọng (deep technical bugs), ban giám đốc lại không thể trông cậy vào bạn do bạn không phải là chuyên gia đi sâu lĩnh vực đó để giải quyết triệt để vấn đề.

Ngược lại, nếu bạn cực kỳ tinh thông một mảng công nghệ chuyên sâu và hoàn toàn không quan tâm đến các mảng khác, doanh nghiệp lại đánh giá bạn có giá trị cốt lõi rất lớn. Bởi vì bạn có khả năng giải quyết các bài toán hóc búa nhất của mảng đó, tạo lợi thế cạnh tranh cho sản phẩm của công ty, nhờ đó lộ trình thăng tiến của bạn diễn ra nhanh hơn nhiều.

Tôi từng đọc được nhận định thế này:

> *"Hầu hết lập trình viên chuyên nghiệp có thâm niên đều lựa chọn đi sâu chuyên môn hóa một stack công nghệ cụ thể do việc này giúp họ dễ tìm được công việc thu nhập cao. Một số chuyên gia tuyển dụng thậm chí còn coi việc liên tục nhảy qua nhảy lại giữa các stack công nghệ khác nhau là một điểm trừ lớn trong CV."*

Do đó, khi viết CV xin việc, bạn không nên nhồi nhét toàn bộ các từ khóa công nghệ mình từng nghe qua vào bản lý lịch, điều đó chỉ khiến CV của bạn trông giống một người nghiệp dư biết mỗi thứ một ít. Thay vào đó, hãy làm nổi bật mảng công nghệ bạn làm sâu sắc nhất cùng các dự án thực tế tương ứng.

Đối với các lập trình viên mới vào nghề muốn phát triển sự nghiệp lâu dài, lời khuyên là hãy lựa chọn một đến hai hướng công nghệ để đào sâu nghiên cứu trở thành chuyên gia, thay vì cố gắng học mỗi thứ một ít mà không có mảng nào thực sự nổi bật.

Tất nhiên lựa chọn đi sâu chuyên môn hóa cũng đi kèm rủi ro nếu stack công nghệ bạn chọn rơi vào chu kỳ thoái trào (như PHP) hoặc thậm chí bị khai tử hoàn toàn (như công nghệ Flash trước đây). Lúc đó bạn bắt buộc phải chuyển đổi sang stack công nghệ khác từ đầu.

Giải pháp an toàn nhất là lựa chọn chuyên sâu các mảng công nghệ được hậu thuẫn bởi các tập đoàn lớn toàn cầu. Đó là lý do thị trường luôn sở hữu lượng lớn chuyên gia Java hay .NET.

Tóm lại, các lập trình viên đa năng thường ít được ưu tiên thăng tiến chuyên môn sâu tại các doanh nghiệp lớn và thường bị xem là người "vạn năng nhưng không tinh thông". Nếu bạn đang thuộc nhóm này, ngoài việc tranh thủ thời gian bồi đắp một kỹ năng sở trường sâu sắc, bạn cũng không nên quá lo lắng. Ở bản tin số tiếp theo, chúng ta sẽ cùng thảo luận về những giá trị và lợi thế độc đáo mà chỉ các lập trình viên đa năng mới sở hữu.

## Chương trình tư vấn và lập kế hoạch tài chính lương hưu gia đình

Tuần này chúng tôi giới thiệu chương trình tư vấn quản lý tài chính cá nhân xoay quanh chủ đề **hoạch định sớm lương hưu gia đình**.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082915.jpg)

Lập trình viên thường là nhóm lao động trẻ tuổi nên rất ít người chú trọng đến kế hoạch lương hưu dài hạn. Khác với suy nghĩ sai lầm của nhiều người rằng doanh nghiệp sẽ chịu trách nhiệm hoàn toàn cho lương hưu của bạn khi bạn cống hiến đủ lâu, lương hưu thực chất được chi trả từ quỹ bảo hiểm xã hội đóng góp định kỳ. Chỉ cần đóng đủ bảo hiểm xã hội tối thiểu 15 năm và đạt độ tuổi nghỉ hưu theo luật định, bạn sẽ được nhận lương hưu hàng tháng từ ngân sách nhà nước.

Đối với nghề có tính luân chuyển nhân sự cao và nhạy cảm tuổi tác như lập trình viên, việc hoạch định sớm tài chính cá nhân mang ý nghĩa bảo đảm an sinh cực lớn. Dưới đây là các câu hỏi thường gặp:

1. Nếu nghỉ hưu sớm hoặc tạm thời dừng công tác tự do một thời gian, bảo hiểm xã hội sẽ được xử lý ra sao để không bị ngắt quãng?
2. Cách tính toán chi tiết số tiền lương hưu nhận được sau này thế nào? Làm sao để tối ưu hóa mức hưởng cao nhất?
3. Lập trình viên tự do (freelancer) có thể tham gia đóng và nhận lương hưu tự nguyện được không?
4. Ngoài lương hưu nhà nước, có nên mua thêm các gói bảo hiểm hưu trí thương mại bổ trợ?

Mọi thắc mắc trên đều sẽ được giải đáp chi tiết trong chương trình tư vấn tài chính chuyên sâu.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082916.jpg)

Chương trình được phối hợp tổ chức bởi chuyên gia tài chính **Tôn Minh Triển** (nhà sáng lập Trussan - đơn vị tư vấn tài chính doanh nghiệp lớn). Khóa học được thiết kế dành riêng cho độc giả bản tin với **200 suất đăng ký hoàn toàn miễn phí**. Đội ngũ chuyên gia tài chính sẽ hỗ trợ bạn:

- Xác định mục tiêu tích lũy lương hưu dài hạn.
- Đánh giá tổng quan năng lực tài chính và trách nhiệm bảo hiểm của các thành viên gia đình.
- Phân tích hiệu quả chi phí của các gói bảo hiểm thương mại hiện có.
- Hoạch định danh mục đầu tư an toàn tài chính hưu trí gia đình chi tiết, cam kết không quảng cáo bán sản phẩm.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082914.jpg)

Độc giả có thể quét mã QR trên đây để đăng ký tham gia chương trình tư vấn tài chính hưu trí miễn phí.

## 科技动态

1、[Mức phí đăng ký tên miền .com chính thức tăng giá](https://domainnamewire.com/2021/02/11/breaking-verisign-announces-com-price-hike-to-8-39/)

Kể từ ngày 1/9, mức phí đăng ký gốc của tên miền .com do tổ chức quản lý độc quyền VeriSign thu từ các nhà bán lẻ chính thức điều chỉnh tăng từ 7,85 USD lên 8,39 USD mỗi năm (mức tăng khoảng 54 cent Mỹ).

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021083111.jpg)

Hệ thống tên miền toàn cầu được quản lý bởi tổ chức ICANN, tổ chức này đã ủy quyền quyền khai thác thương mại đuôi tên miền phổ biến nhất thế giới .com cho công ty VeriSign. Do tính chất độc quyền và áp lực tăng trưởng của một doanh nghiệp niêm yết, VeriSign dự kiến sẽ tiếp tục tăng phí đăng ký tên miền .com trong các năm tới theo lộ trình đã được phê duyệt.

2、[Thiết bị điện kích thích thần kinh thay thế cà phê chống buồn ngủ](https://www.scientificamerican.com/article/neck-zapping-gadget-reduced-all-nighter-fatigue-in-new-study/)

Để giúp nhân viên văn phòng và các kỹ sư làm việc đêm tỉnh táo tức thì mà không cần lạm dụng cà phê, một startup công nghệ tại Mỹ đã phát triển dòng thiết bị mát-xa điện cực nhỏ gọn:

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062203.jpg)

Người dùng chỉ cần áp thiết bị vào vùng da cổ gần động mạch cảnh và bật công tắc. Thiết bị sẽ phát ra các xung điện áp thấp cực ngắn (chỉ khoảng 1 mili giây) tác động kích thích nhẹ lên dây thần kinh phế vị, thúc đẩy cơ thể tự sản sinh adrenaline tự nhiên để loại bỏ cảm giác mệt mỏi tức thì. Giá bán hiện tại của sản phẩm khá đắt đỏ, ở mức 1.250 USD mỗi thiết bị.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062204.jpg)

3、[Triển lãm ảo kỷ niệm bài phát biểu của Martin Luther King trên game Fortnite](https://www.yystv.cn/p/8306)

Nhân ngày kỷ niệm danh nhân Martin Luther King phát biểu bài chính luận kinh điển *"Tôi có một ước mơ"* (28/8), tựa game trực tuyến Fortnite đã thiết lập một phân khu không gian triển lãm ảo 3D đặc biệt bên trong bản đồ game:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090102.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090103.jpg)

Người chơi khi điều khiển nhân vật chạy qua khu vực này có thể dừng lại xem các đoạn phim tư liệu lịch sử trình chiếu trực tiếp trên màn hình ảo lớn, hoặc bước vào bảo tàng ảo để đọc các thông tin sự kiện lịch sử chi tiết. Đây là hướng đi mới của ngành giáo dục tương tác số đang được nhiều hãng công nghệ áp dụng.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090104.jpg)

4、[Michelin thử nghiệm cánh buồm hơi tự động trên tàu biển vận tải](https://spectrum.ieee.org/energywise/green-tech/wind/michelin-puffy-sails-cargo-ships-improve-fuel-economy)

Tập đoàn lốp xe Michelin đang tiến hành thử nghiệm dự án lắp đặt hệ thống cánh buồm khí nén tự động dạng module trên các tàu chở hàng đại dương cỡ lớn:

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062701.jpg)

Cánh buồm có khả năng tự động bơm căng hơi và điều chỉnh góc đón gió tối ưu nhờ hệ thống cảm biến thông minh giúp tận dụng tối đa động lực gió trên biển, tiết kiệm tới 20% lượng dầu diesel tiêu thụ và giảm đáng kể lượng khí thải carbon phát sinh.

5、[Mẫu nhà lắp ghép Boxabl Casita giá rẻ thu hút sự quan tâm của Elon Musk](https://www.businessinsider.com/elon-musk-tiny-home-prefab-boxabl-casita-50000-person-waitlist-2021-8#tiny-homes-have-become-an-undeniably-popular-alternative-to-the-classic-family-home-or-apartment-1)

Hãng công nghệ nhà lắp ghép tiền chế Boxabl tại Las Vegas đã phát triển mẫu nhà di động Casita rộng 35m2 với giá bán chỉ 49.500 USD:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081021.jpg)

Ngôi nhà được đóng gói gọn gàng như một thùng container lớn, khi vận chuyển đến địa điểm lắp đặt chỉ mất vài giờ để mở rộng cấu trúc vách tường hoàn thiện đầy đủ phòng ngủ, phòng khách, bếp và nhà tắm đã lắp sẵn các thiết bị nội thất cơ bản:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081022.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081023.jpg)

Sản phẩm gây chú ý lớn khi chính tỷ phú Elon Musk đã đặt mua một ngôi nhà Casita để lắp đặt sử dụng ngay tại bãi thử tên lửa Starbase của SpaceX ở Texas. Thông tin này lập tức tạo nên cơn sốt mua hàng tại Mỹ với danh sách chờ đăng ký mua hiện đã vượt quá 50.000 khách hàng.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081024.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081025.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081027.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081026.jpg)

6、[Hải quân Mỹ nghiên cứu máy bay năng lượng mặt trời bay 90 ngày liên tục](https://uk.news.yahoo.com/us-navy-developing-solar-powered-193723844.html)

Lực lượng Hải quân Mỹ đang đặt hàng phát triển dòng máy bay không người lái trinh sát chạy bằng năng lượng mặt trời Skydweller có khả năng bay liên tục trên không trung suốt 90 ngày đêm không cần hạ cánh tiếp nhiên liệu.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081009.jpg)

Máy bay sở hữu sải cánh siêu rộng lên tới 72 mét được phủ kín hoàn toàn bằng các tấm pin mặt trời hiệu suất cao, tích hợp hệ thống pin lưu trữ lithium lớn để duy trì nguồn điện cho động cơ hoạt động ổn định vào ban đêm. Phiên bản thử nghiệm trước đó của dòng máy bay này đã lập kỷ lục thế giới khi thực hiện hành trình bay liên tục suốt 117 giờ không nghỉ.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081010.jpg)

7、[Doanh nghiệp gây tranh cãi khi sa thải nhân viên bằng thuật toán phân tích dữ liệu](https://www.gamasutra.com/view/news/386534/Xsolla_lays_off_150_after_an_algorithm_ruled_staff_unengaged_and_unproductive.php)

Tập đoàn cung cấp dịch vụ thanh toán trò chơi trực tuyến Xsolla (Mỹ) công bố quyết định sa thải đồng loạt 150 nhân sự (chiếm khoảng 1/3 quy mô công ty) do lợi nhuận sụt giảm. Chi tiết gây tranh cãi lớn là ban giám đốc đã sử dụng một thuật toán AI phân tích dữ liệu lớn để chỉ định danh sách nhân sự bị sa thải.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081301.jpg)

Email thông báo của CEO gửi đến các nhân sự bị cắt giảm viết rõ: *"Hệ thống phân tích dữ liệu lớn của chúng tôi đã theo dõi và đánh giá toàn bộ hoạt động tương tác của các bạn trên các nền tảng Jira, Confluence, Gmail, các cuộc trò chuyện nhóm và chỉnh sửa tài liệu nội bộ. Kết quả phân tích chỉ ra mức độ tương tác và hiệu quả đóng góp công việc của bạn khi làm việc từ xa (remote work) không đạt yêu cầu. Chúng tôi tin rằng môi trường làm việc năng động của Xsolla không còn phù hợp với bạn nữa."*

## 文章

1、[Trung Quốc thử nghiệm thành công kỹ thuật lặn sâu bão hòa 500 mét](https://finance.sina.com.cn/tech/2021-09-01/doc-iktzqtyt3389836.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090208.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090209.jpg)

Bài viết tường thuật chi tiết quá trình thử nghiệm của 9 thợ lặn chuyên nghiệp sinh hoạt liên tục trong buồng áp suất khí nén mô phỏng độ sâu 500m dưới lòng đại dương (áp suất lên tới 51 atm) suốt 176 giờ liên tục, mở đường cho việc ra mắt các tàu lặn cứu hộ biển sâu thế hệ mới.

2、[Hành trình gia nhập Viện nghiên cứu Microsoft Cambridge của tôi](https://justyy.com/archives/45631)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090111.jpg)

Tác giả chia sẻ chi tiết kinh nghiệm chuẩn bị hồ sơ ứng tuyển, các vòng phỏng vấn kỹ thuật thuật toán hóc búa để chuyển việc thành công từ tập đoàn Amazon sang làm việc tại Viện nghiên cứu Microsoft Cambridge. (Đóng góp của [@DoctorLai](https://github.com/ruanyf/weekly/issues/1914))

3、[Hướng dẫn theo dõi cập nhật log hệ thống thời gian thực trên Linux](https://linux.cn/article-13733-1.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090114.jpg)

Cẩm nang hướng dẫn sử dụng các tiện ích dòng lệnh như `tail`, `multitail` hoặc `lnav` để gom và theo dõi trực quan toàn bộ các tệp tin nhật ký hoạt động (log files) tại thư mục `/var/log` trong cùng một giao diện dòng lệnh. (Đóng góp của [@jerrylususu](https://github.com/ruanyf/weekly/issues/1915))

4、[Phân tách logic dữ liệu ra khỏi UI bằng React Hooks](https://felixgerschau.com/react-hooks-separation-of-concerns/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081020.jpg)

Một bài viết chất lượng cao hướng dẫn tư duy viết code React hiện đại: Sử dụng custom Hooks làm nơi quản lý toàn bộ các tác vụ gọi API, xử lý biến đổi dữ liệu (logic layer) để giữ cho file code components giao diện (UI layer) luôn sạch sẽ, dễ bảo trì và tối ưu kiểm thử.

5、[Tìm hiểu 4 quy chuẩn thiết kế tương tác UI/UX mới trên hệ điều hành iOS](https://www.nngroup.com/articles/4-ios-rules-break/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081102.jpg)

Bài viết phân tích các thay đổi thiết kế giao diện di động của Apple (như chuyển nút xác nhận Submit lên góc trên bên phải màn hình thay vì đặt dưới biểu mẫu) giúp các nhà thiết kế UI/UX xây dựng ứng dụng di động tối ưu hành vi ngón tay người dùng.

6、[Ứng dụng thuộc tính content trong CSS](https://echeverra.cn/2021/08/06/css-content/)（Tiếng Trung）

Tổng hợp các kỹ thuật thiết kế Front-end ứng dụng thuộc tính `content` kết hợp với các bộ chọn giả `:before` hoặc `:after` trong CSS để tự động thêm chữ, hiển thị số thứ tự tự động hoặc chèn icon động mà không cần can thiệp cấu trúc file HTML.

7、[Tìm hiểu bản chất của hệ điều hành máy tính](https://zhuanlan.zhihu.com/p/403919173)（Tiếng Trung）

Bài viết dịch thuật nhập môn thuộc chuỗi bài giảng thiết kế hệ điều hành, phân tích định nghĩa về kernel OS, cơ chế tương tác phần cứng và quản lý tiến trình cơ bản của hệ thống. (Đóng góp của [@StrokMitream](https://github.com/ruanyf/weekly/issues/1909))

8、[Firefox 91 ra mắt cơ chế nâng cao hỗ trợ xóa sạch cookie của bên thứ ba](https://blog.mozilla.org/security/2021/08/10/firefox-91-introduces-enhanced-cookie-clearing/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081103.jpg)

Thông thường tính năng xóa cookie của trình duyệt chỉ xóa các cookie của chính trang web đó mà bỏ sót các cookie theo dõi do các iframe quảng cáo bên thứ ba nhúng vào. Firefox 91 ra mắt tính năng Enhanced Cookie Clearing hỗ trợ quét và dọn dẹp sạch toàn bộ các cookie theo dõi chéo này.

9、[Hướng dẫn lập trình crawler thu thập dữ liệu web bằng Python từ con số không](https://www.zenrows.com/blog/mastering-web-scraping-in-python-crawling-from-scratch)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081205.jpg)

Cẩm nang hướng dẫn chi tiết cách viết một script cào dữ liệu web bằng Python: sử dụng thư viện Requests và BeautifulSoup để bóc tách thông tin HTML, cấu hình đa luồng tối ưu tốc độ tải và xử lý cơ chế đổi User-Agent để tránh bị máy chủ chặn.

## 工具

1、[FeedAdd: Tạo RSS cho tài khoản công khai WeChat](https://feeddd.org/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090110.jpg)

Một công cụ trực tuyến miễn phí hỗ trợ người dùng nhập tài khoản WeChat công khai bất kỳ để tự động sinh ra một đường dẫn luồng RSS cập nhật bài viết mới tự động. (Đóng góp của [@miscommunication](https://github.com/ruanyf/weekly/issues/1910))

2、[PlayCover: Hỗ trợ chuột và phím cho iOS App trên Mac M1](https://github.com/Letscoder/PlayCover)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081312.jpg)

Dự án mã nguồn mở hỗ trợ gán phím tắt linh hoạt để điều khiển các tựa game và ứng dụng di động iOS chạy trên dòng máy tính MacBook chip M1 bằng chuột và bàn phím máy tính.

3、[Judo: Công cụ thiết kế giao diện không code cho iOS](https://www.judo.app/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081413.jpg)

Ứng dụng thiết kế dành riêng cho macOS hỗ trợ các designer kéo thả trực quan để tự sinh giao diện ứng dụng iOS đạt tiêu chuẩn SwiftUI mà không cần viết code, hỗ trợ kết nối hiển thị kết quả thời gian thực trên điện thoại.

4、[macOS Monterey Web](https://github.com/puruvj/macos-web)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081422.jpg)

Dự án thú vị sử dụng framework Svelte để tái hiện sinh động toàn bộ giao diện desktop, thanh dock, cửa sổ ứng dụng và hình nền động của hệ điều hành macOS Monterey ngay trên nền web.

5、[OneDev Git Server](https://github.com/theonedev/onedev)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081601.jpg)

Hệ thống quản lý kho mã nguồn Git và tích hợp CI/CD tự host nguồn mở gọn nhẹ, tiêu thụ rất ít tài nguyên máy chủ so với các giải pháp nặng nề như GitLab.

6、[BackgroundRemover](https://github.com/nadermx/backgroundremover)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081701.jpg)

Công cụ dòng lệnh sử dụng mô hình học máy thông minh giúp nhanh chóng tách và xóa bỏ nền của ảnh chụp hoặc các phân cảnh video tự động.

7、[js-ziju: Compiler JavaScript tự viết của tác giả](https://github.com/wizardpisces/js-ziju)

Dự án viết trình biên dịch cá nhân của tác giả giúp chuyển đổi trực tiếp mã nguồn JavaScript sang cấu trúc trung gian LLVM IR và mã máy assembly X86. (Đóng góp của [@wizardpisces](https://github.com/ruanyf/weekly/issues/1918))

8、[zx: Thư viện điều khiển dòng lệnh bằng JavaScript của Google](https://github.com/google/zx)

Tiện ích do Google phát triển hỗ trợ lập trình viên viết các kịch bản script tự động hóa hệ thống (thay thế Shell Script truyền thống) bằng cú pháp JavaScript mượt mà thông qua việc đóng gói các hàm thực thi Bash trực quan.

9、[HyperFormula Formula Engine](https://github.com/handsontable/hyperformula)

Thư viện JavaScript hiệu năng cao hỗ trợ xử lý và tính toán hơn 300 công thức toán học, logic và tài chính tương đương bộ công cụ Excel trên trình duyệt web.

## Tài nguyên

1、[Khóa học lập trình Go cơ bản đến thực chiến](https://cdn.beekka.com/blogimg/asset/202109/bg2021090207.jpg)

Chương trình đào tạo Go cơ bản miễn phí trên nền tảng Geekbang do chuyên gia Senior Go giảng dạy, giới thiệu cú pháp cơ bản và thực hành viết ứng dụng máy tính bỏ túi bỏ túi. Đăng ký qua WeChat của trợ lý lớp học trước ngày 6/9.

2、[Bộ hình nền macOS Bliss độc đáo](https://basicappleguy.com/basicappleblog/macosbliss)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081019.jpg)

Tác giả chia sẻ miễn phí bộ hình nền phong cảnh đồi cỏ xanh ngắt lấy cảm hứng từ bức ảnh hình nền Bliss huyền thoại của Windows XP được thiết kế tối ưu hóa độ phân giải cao cho các dòng máy Mac, iPad và iPhone.

3、[Hướng dẫn thiết lập trình giả lập Nintendo Switch trên hệ điều hành Linux](https://boilingsteam.com/emulating-nintendo-switch-games-on-linux-2/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081011.jpg)

Cẩm nang hướng dẫn chi tiết các bước cài đặt và cấu hình trình giả lập Yuzu để trải nghiệm mượt mà các tựa game Nintendo Switch ngay trên máy tính chạy hệ điều hành Linux.

4、[Bảng tra cứu địa chất các loại đá trong game Minecraft ngoài đời thực](https://www.mindat.org/a/minecraft)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081014.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081016.jpg)

Chuyên trang tổng hợp đối chiếu hình ảnh và thông số tinh thể của toàn bộ các loại quặng mỏ ảo xuất hiện trong game Minecraft tương ứng với các mẫu khoáng vật địa chất thực tế ngoài đời thực.

5、[AWS in Plain English (Lược dịch AWS sang tiếng Anh dễ hiểu)](https://expeditedsecurity.com/aws-in-plain-english/)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072703.jpg)

Trang web tổng hợp lược dịch đặc tả kỹ thuật của hơn 50 dịch vụ điện toán đám mây cốt lõi của AWS sang ngôn ngữ tiếng Anh phổ thông dễ hiểu thay cho các tài liệu đặc tả học thuật rườm rà của Amazon.

## 图片

1、[Ý tưởng thiết kế chiếc quần jeans tích hợp sẵn bàn phím độc đáo](https://www.theverge.com/2016/4/21/11476984/keyboard-pants-reconsidered)

Một sinh viên thiết kế người Hà Lan đã phát triển sản phẩm quần jeans bàn phím vô cùng độc đáo. Bàn phím không dây Bluetooth được may cố định ngay trên hai đùi quần jeans, đi kèm một hộc chứa chuột máy tính nhỏ ở túi sau giúp người dùng chỉ cần ngồi xuống là đã có thể gõ máy tính linh hoạt mà không cần nâng cổ tay lên bàn:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071003.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071004.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071005.jpg)

2、[Cận cảnh một chú hải ly gặm đổ thân cây gỗ làm tổ](https://twistedsifter.com/videos/beaver-chewing-through-tree-close-up/)

Hình ảnh cận cảnh chú hải ly dùng bộ răng cửa vô cùng khỏe của mình gặm đổ một gốc cây gỗ lớn để chuẩn bị kéo gỗ về đắp đập ngăn sông làm tổ ấm:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070908.jpg)

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=q3258r13usz" allowFullScreen="true" width="600" height="400"></iframe>

## Bài đọc thêm

### Lời phát biểu của Linus Torvalds nhân dịp ra mắt Linux Kernel 5.14

*Nhân dịp kỷ niệm tròn 30 năm ngày Linus công bố bản Linux Kernel đầu tiên ra thế giới (25/8/1991), ông đã phát hành phiên bản cập nhật 5.14 đúng kế hoạch và gửi kèm thư ngỏ gửi đến các nhà phát triển:*

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021083114.jpg)

*"Tôi biết mọi người đang bận rộn tham gia các bữa tiệc kỷ niệm 30 năm hoành tráng ngoài kia với rượu champagne và pháo hoa. Nhưng nếu một lúc nào đó bạn cảm thấy mệt mỏi với những lễ nghi hào nhoáng và bộ vest gò bó đó, muốn tìm một khoảng lặng tĩnh tâm, tôi đã chuẩn bị sẵn một phiên bản Kernel mới để bạn tải về thử nghiệm.*

*Tất nhiên, những nhà phát triển bảo trì Kernel cần mẫn của chúng ta sẽ không có thời gian dự tiệc đâu, vì đối với họ, ngày hôm nay đồng nghĩa với việc khung thời gian merge code cho phiên bản tiếp theo sẽ mở ra vào ngày mai. Chúng tôi hy vọng sẽ cùng nhau đi tiếp hành trình 30 năm tiếp theo. Nhưng đối với tất cả những người khác, hãy tạm nghỉ một chút, biên dịch phiên bản Kernel mới này, chạy thử nghiệm nó, rồi bạn có thể quay lại bữa tiệc dường như không bao giờ kết thúc ngoài kia."*

### Chia sẻ của chuyên gia Scott Meyers về quyết định rút lui khỏi cộng đồng C++

*Scott Meyers là chuyên gia C++ huyền thoại, tác giả của loạt sách giáo khoa kinh điển Effective C++ gối đầu giường của nhiều thế hệ lập trình viên:*

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090201.jpg)

Sau khi công bố dừng viết sách C++ vào năm 2015, đến năm 2018 ông tiếp tục thông báo sẽ dừng việc cập nhật và đính chính các lỗi kỹ thuật (errata) trong các cuốn sách cũ của mình. Ông chia sẻ chân thành:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090206.jpg)

*"Để sửa lỗi, trước hết tôi phải có khả năng nhận diện và đánh giá chúng. Nhưng tôi nhận ra mình không còn đủ khả năng làm việc đó nữa. Kể từ khi tôi dừng tham gia sâu vào sự phát triển của ngôn ngữ C++ từ cuối năm 2015, tốc độ thay đổi và sự phức tạp của các chuẩn C++ mới (C++11/14/17) đã khiến tôi quên đi rất nhiều chi tiết tinh tế của ngôn ngữ.*

*C++ là một ngôn ngữ vô cùng khổng lồ và phức tạp với hàng loạt cơ chế hoạt động tinh vi, tôi không còn tin bản thân có thể ghi nhớ chính xác toàn bộ chúng trong đầu sau khi nghỉ hưu. Do đó, tôi chân thành cảm ơn các báo cáo lỗi của độc giả nhưng sẽ không tiến hành chỉnh sửa nội dung sách nữa. Đây là giải pháp duy nhất có trách nhiệm mà tôi có thể thực hiện lúc này."*

## 言论

1、

Một trong những bài học lập trình đắt giá nhất tôi học được trên mạng là: Tuyệt đối không bao giờ copy và paste trực tiếp các đoạn code do người khác viết vào dự án của mình. Nếu bạn muốn sử dụng đoạn code đó, hãy tự tay gõ lại từng ký tự. Việc gõ lại từng chữ buộc bộ não của bạn phải suy nghĩ thấu đáo logic thực tế của dòng code đó hoạt động ra sao.

-- Thảo luận trên Hacker News

2、

Mọi người thường nói 996 (làm việc từ 9h sáng đến 9h tối, 6 ngày/tuần) giúp tăng năng suất công nghệ, nhưng tư duy này thực chất bắt nguồn từ thời kỳ sản xuất công nghiệp nhà máy dệt may cổ xưa: muốn tăng sản lượng quần áo cách nhanh nhất là bắt công nhân tăng ca. Lập trình công nghệ hoàn toàn khác, việc lập trình viên ngồi lì trước màn hình máy tính nhiều giờ hơn không đồng nghĩa với việc họ viết ra được những dòng code chất lượng hơn. Thực tế, cách tốt nhất để tìm ra các lỗi logic hóc búa là đứng dậy nghỉ ngơi một chút rồi quay lại đọc code sau đó.

-- Thảo luận trên Hacker News nhân sự kiện Tòa án Tối cao Trung Quốc tuyên bố chế độ làm việc 996 là vi phạm luật lao động

## 历史上的本周

- 2020年（第 123 期）：[Phân tích mô hình tổ chức của các tập đoàn Internet Trung Quốc so sánh với cơ cấu quân đội Tương Quân thời xưa](https://www.ruanyifeng.com/blog/2020/09/weekly-issue-123.html)
- 2019年（第 71 期）：[Tại sao những sinh viên tốt nghiệp các trường đại học danh tiếng hàng đầu lại khó khăn hơn khi bắt đầu khởi nghiệp](https://www.ruanyifeng.com/blog/2019/08/weekly-issue-71.html)
- 2018年（第 20 期）：[Khảo sát các giải pháp học nghề thực tiễn dành cho học sinh không lựa chọn con đường vào đại học](https://www.ruanyifeng.com/blog/2018/08/weekly-issue-20.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
