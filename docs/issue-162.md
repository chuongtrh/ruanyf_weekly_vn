# 科技爱好者周刊（第 162 期）：生活就像《吃豆人》游戏

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1652) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060914.jpg)

Triển lãm Thế giới Dubai 2020 (trì hoãn đến năm nay) dự kiến sẽ chính thức khai mạc vào ngày 1 tháng 10. Hình ảnh trên là "Tòa nhà Phát triển Bền vững" - một trong ba công trình trung tâm của triển lãm. Công trình được thiết kế để tự cung tự cấp hoàn toàn năng lượng và nước sạch bằng cách sử dụng các tấm pin mặt trời khổng lồ để phát điện và hệ thống ngưng tụ hơi ẩm từ không khí sa mạc để tạo nước ngọt.

## 主带话题：Cuộc sống giống như trò chơi Pac-Man

Có một trò chơi điện tử cổ điển vô cùng nổi tiếng mang tên *Pac-Man* (Ăn đậu). Trò chơi này phát hành lần đầu từ năm 1980, và cho tới tận ngày nay vẫn có rất nhiều người yêu thích chơi.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060615.jpg)

Cách chơi vô cùng đơn giản: Bạn điều khiển nhân vật ăn hết các hạt đậu trong mê cung để vượt qua màn chơi mới, đồng thời phải tìm cách né tránh sự truy đuổi của bốn con ma. Bốn con ma này sở hữu các chiến thuật di chuyển rất khác biệt: con màu đỏ chuyên đuổi theo từ phía sau, con màu hồng di chuyển chặn đầu, con màu xanh lam phục kích ở các ngã rẽ và con màu cam di chuyển trôi nổi ngẫu nhiên. Trong mê cung cũng có bốn hạt đậu năng lượng lớn, giúp bạn có khả năng phản công tiêu diệt tạm thời các con ma sau khi ăn.

Bạn có thể chơi thử phiên bản web do Google phát triển tại [đây](https://www.google.com/search?q=pac-man).

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060901.jpg)

Tôi muốn nói về trò chơi này vì gần đây có đọc được một bài viết của một lập trình viên trẻ người nước ngoài chia sẻ góc nhìn: anh cảm thấy cuộc sống của mình giống hệt như một ván game *Pac-Man*:

> *"Sau khi tốt nghiệp đại học, tôi rơi vào trạng thái mơ hồ không rõ nên làm gì tiếp theo. Đi học thạc sĩ hay tìm một công việc văn phòng ổn định? Cuối cùng, giống như đa số mọi người, tôi lựa chọn những công việc trông có vẻ hào nhoáng dù không mấy tương thích với sở thích cá nhân. Tôi hoàn toàn không có kế hoạch rõ ràng cho tương lai."*
> 
> *"Tôi nhận ra cuộc sống của mình có quá nhiều nét tương đồng với trò chơi Pac-Man. Tôi đang bị mắc kẹt trong một mê cung cuộc đời, phải liên tục di chuyển để tích lũy điểm số và vượt qua các thử thách. Những con ma đại diện cho các cuộc khủng hoảng tài chính, áp lực công việc và biến cố sức khỏe luôn lảng vảng xung quanh chực chờ đánh gục bạn. Chỉ cần sẩy chân một nhịp, bạn có thể mất đi một lượt mạng và phải bắt đầu lại từ con số không."*
> 
> *"Tôi thực sự không biết mình nên đi về hướng nào, làm sao để thăng tiến và khi nào các biến cố khó khăn sẽ bất ngờ ập đến."*

Lập luận này khiến tôi nhận thấy *Pac-Man* thực sự là một hình ảnh ẩn dụ tuyệt vời cho cuộc sống hiện đại. Hàng ngày chúng ta đều đang phải tự mò mẫm tìm đường đi trong các mê cung cuộc đời của mình. Các khó khăn trở ngại luôn xuất hiện ở những ngóc ngách không lường trước. Và cách duy nhất để sinh tồn là phải liên tục di chuyển né tránh rủi ro, tận dụng các cơ hội năng lượng ngắn ngủi để gia tăng sức mạnh nội tại và bước sang màn chơi tiếp theo.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060617.jpg)

Lấy ví dụ về giới lập trình viên: Khi bạn tốt nghiệp và bước chân vào các tập đoàn công nghệ lớn, đó là lúc trò chơi chính thức bắt đầu. Bạn buộc phải liên tục nâng cấp kỹ năng, vượt qua các kỳ đánh giá hiệu suất để thăng tiến từ Intern lên Junior, Senior, rồi Team Leader hay Tech Lead. Nếu bị kẹt lại ở một vị trí quá lâu, bạn sẽ rơi vào vùng nguy hiểm khi tuổi tác tăng lên nhưng giá trị kỹ thuật đóng góp không tương xứng, nguy cơ bị đào thải (Game Over) bởi các thế hệ trẻ hơn là rất lớn. Thời gian vàng để bạn leo lên các nấc thang quản lý hoặc chuyên gia cốt cán chỉ gói gọn trong khoảng 10 đến 15 năm đầu sự nghiệp.

**Không chỉ lập trình viên, mọi ngành nghề có tính cạnh tranh cao đều vận hành theo quy luật sinh tồn này.** Nhiều người nghĩ làm giảng viên đại học là công việc nhàn hạ, tự do giờ giấc và có kỳ nghỉ hè dài. Nhưng thực tế các trường đại học lớn hiện nay đều áp dụng chính sách quản lý nhân sự theo mô hình Tenure Track (ở Trung Quốc gọi là chính sách "Không thăng tiến thì rời đi" - 非升即走): các tiến sĩ trẻ khi được nhận vào trường ở vị trí giảng viên sẽ có thời hạn 6 năm để nghiên cứu và công bố các bài báo khoa học chuẩn quốc tế. Nếu sau 6 năm không đạt chuẩn thăng tiến lên phó giáo sư, họ bắt buộc phải nộp đơn nghỉ việc để nhường vị trí cho nhân sự mới. Quy luật này có khác gì trò chơi sinh tồn *Pac-Man* phiên bản thực tế đâu cơ chứ.

Rộng hơn nữa, mỗi buổi sáng giờ cao điểm trên các chuyến tàu điện ngầm đông nghẹt, hàng vạn người trẻ đang tham gia vào một ván game lớn tại các siêu đô thị. Nếu sau nhiều năm bám trụ mà không thể đạt được các cột mốc tài chính ổn định (như mua nhà, định cư), họ cũng sẽ phải rời đi để quay về các đô thị nhỏ hơn.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060903.jpg)

Tất nhiên, bạn hoàn toàn có thể lựa chọn đứng ngoài ván game này bằng cách giảm thiểu các nhu cầu vật chất để sống một cuộc đời an nhiên không tranh giành. Nhưng nếu đã lựa chọn hoặc bắt buộc phải tham gia trò chơi, bạn có thể tham khảo một số chiến thuật sinh tồn trong game *Pac-Man*:

- **Tuyệt đối không được đứng yên tại chỗ quá lâu, vì các khó khăn (những con ma) sẽ tự động dò tìm và tiếp cận vị trí của bạn.**
- **Phải luôn giữ trạng thái chuyển động tiến lên phía trước.**
- **Khi phát hiện chướng ngại vật xuất hiện phía trước, phải nhanh chóng chủ động thay đổi lộ trình.**
- **Tập trung thu hoạch các cơ hội tích lũy gần nhất để tạo dựng các cột mốc thành tựu ngắn hạn.**

## Khóa học so sánh các công cụ đóng gói Front-end

Như mọi lập trình viên Front-end đều biết, Webpack là công cụ build tool thống trị tuyệt đối mảng phát triển ứng dụng web trong suốt gần một thập kỷ qua. Dù bạn sử dụng Vue, React hay Angular thì mã nguồn cuối cùng đều được biên dịch đóng gói thông qua Webpack.

Tuy nhiên kể từ năm 2020, sự phổ biến của tiêu chuẩn ESModule đã thúc đẩy sự ra đời của các công cụ đóng gói thế hệ mới như Vite (dựa trên ESbuild viết bằng Go) và Rollup. Các công cụ mới sở hữu tốc độ biên dịch cực nhanh, cấu hình tối giản giúp tối ưu hiệu năng phát triển. Ngay cả cha đẻ Vue -尤雨溪 cũng tuyên bố "không thể quay lại sử dụng Webpack".

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061006.jpg)

Điều này gây ra không ít băn khoăn cho lập trình viên:
- Liệu Webpack có bị khai tử sớm và có cần học Webpack nữa không?
- Chưa học xong Webpack lại phải học thêm các công cụ mới?
- Nên chọn công cụ nào cho dự án tiếp theo?

Thực tế, cả ba công cụ trên đều có những phân khúc và ưu thế ứng dụng riêng biệt. Khóa học chuyên đề **《Front-end Build Tools PK: Deep Analysis of Webpack, Vite, Rollup Principles》** sẽ giúp bạn gỡ rối các thắc mắc này:

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061008.jpg)

Nội dung khóa học sẽ dẫn dắt học viên thực hành cấu hình dự án trên cả ba công cụ, phân tích chuyên sâu các cơ chế nạp module bên dưới của chúng để giúp lập trình viên lựa chọn công cụ tối ưu cho dự án.

Khóa học được thiết kế tương thích cho cả lập trình viên sơ cấp lẫn trung cấp muốn tìm hiểu sâu về kiến trúc đóng gói mã nguồn Front-end.

Độc giả có thể đăng ký tham gia khóa học qua mã QR dưới đây với mức phí ghi danh tượng trưng chỉ **0.99 NDT**:

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061007.jpg)

Chương trình học sẽ phát sóng trực tiếp từ ngày 15 tháng 6 đến ngày 17 tháng 6 vào lúc 20:00 mỗi tối.

## 科技动态

1、[Tỷ phú Jeff Bezos công bố kế hoạch bay lên không gian vũ trụ](https://www.cnbc.com/2021/06/07/jeff-bezos-to-fly-on-blue-origin-first-passenger-flight-in-july.html)

Nhà sáng lập tập đoàn Amazon - tỷ phú Jeff Bezos thông báo ông sẽ tham gia chuyến bay thử nghiệm chở người đầu tiên lên không gian vũ trụ của hãng hàng không vũ trụ do ông sáng lập - Blue Origin vào tháng 7 tới.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060801.jpg)

Chuyến bay sử dụng tên lửa đẩy phóng khoang cabin chứa khách lên độ cao hơn 100 km cách mặt đất (vùng ranh giới Karman được coi là rìa vũ trụ). Khoang cabin được thiết kế cho 6 hành khách với hệ thống cửa kính siêu lớn giúp hành khách chiêm ngưỡng toàn cảnh Trái Đất và trải nghiệm trạng thái không trọng lực trong vài phút trước khi hạ cánh an toàn xuống mặt đất bằng dù cứu hộ.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060802.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060803.jpg)

2、[Công viên đảo nhân tạo độc đáo Little Island trên sông Hudson](https://mp.weixin.qq.com/s/rf0U7OjeGHBvKGpfECMVhA)

Một quỹ từ thiện tại Mỹ đã đầu tư 260 triệu USD để xây dựng một công viên đảo nhân tạo nổi độc đáo mang tên Little Island nằm trên sông Hudson, New York.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060915.jpg)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052502.jpg)

Công trình được xây dựng trên nền một cầu cảng cũ đã bỏ hoang bằng cách dựng hệ thống cột bê tông đúc ly tâm tạo hình bông hoa tulip nâng đỡ các thảm cỏ, vườn hoa uốn lượn ven sông và một nhà hát ngoài trời có quy mô 687 chỗ ngồi phục vụ các buổi biểu diễn nghệ thuật công cộng cho người dân thành phố.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060916.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060917.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060918.jpg)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052505.jpg)

3、[Làn đường cầu vượt treo hình chữ U giúp xe quay đầu trên cao tốc Quý Châu](https://www.chinatimes.com/realtimenews/20210510002190-260402)

Một tuyến đường cao tốc chạy qua địa phận đồi núi Quý Châu vừa đưa vào vận hành một thiết kế cầu vượt treo hình chữ U (U-turn flyover) vô cùng độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021051807.jpg)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021051808.jpg)

Do địa hình rừng núi hiểm trở, khoảng cách giữa các nút giao exit trên cao tốc Quý Châu thường rất xa (có thể lên tới hàng chục km). Cầu vượt hình chữ U được thiết kế bắc qua dải phân cách giúp các tài xế lỡ đi quá lối rẽ có thể quay đầu xe nhanh chóng và an toàn mà không cần phải di chuyển quá xa.

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021051809.jpg)

4、[Tên lửa Falcon 9 của SpaceX đạt cột mốc phóng thành công 100 lần liên tiếp](https://arstechnica.com/science/2021/05/is-spacex-reliable-company-goes-for-100th-successful-flight-in-a-row-today/)

Dòng tên lửa đẩy Falcon 9 của hãng SpaceX đã thiết lập cột mốc ấn tượng khi thực hiện thành công liên tiếp 100 chuyến phóng vũ trụ an toàn tính đến cuối tháng 5. Tần suất phóng của hãng đang tăng nhanh chóng mặt: đạt trung bình 9 ngày một chuyến phóng từ đầu năm và tăng lên mức 5 ngày một chuyến trong tháng 5.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060301.jpg)

Ưu thế vượt trội giúp SpaceX duy trì tần suất phóng kỷ lục này là nhờ công nghệ tự động thu hồi và tái sử dụng nhanh chóng tầng đẩy thứ nhất (booster) của tên lửa sau khi phóng - một công nghệ hiện tại chỉ có SpaceX làm chủ thành thục trên quy mô thương mại.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060303.jpg)

5、[Hisense ra mắt dòng tivi màn hình laser cuộn độc đáo](https://ggjd.cnstock.com/company/scp_ggjd/tjd_bbdj/202106/4713062.htm)

Hãng điện tử Hisense công bố sẽ mở bán các dòng tivi sử dụng công nghệ màn hình laser cuộn (rollable screen) trong nửa cuối năm nay. Sản phẩm tích hợp một hệ máy chiếu laser tầm siêu ngắn đi kèm một tấm màn chiếu đặc biệt có khả năng tự động cuộn gọn lại vào trong kệ tủ khi không sử dụng để tiết kiệm tối đa không gian phòng khách.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060606.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060607.jpg)

6、[Liên Hợp Quốc công bố mục tiêu chấm dứt dịch bệnh AIDS vào năm 2030](https://news.un.org/zh/story/2021/06/1085332)

Chương trình Phối hợp của Liên Hợp Quốc về HIV/AIDS (UNAIDS) công bố báo cáo khả quan về khả năng chấm dứt dịch bệnh thế kỷ AIDS vào năm 2030. Số lượng người nhiễm mới HIV toàn cầu năm qua đạt 37,6 triệu người và số ca tử vong đạt 690.000 người - giảm lần lượt 30% và 43% so với năm 2010. Liên Hợp Quốc tin rằng nếu nâng tỷ lệ người nhiễm tiếp cận thuốc điều trị ức chế virus ARV từ 73% hiện tại lên mức 95% vào năm 2025, thế giới hoàn toàn có thể loại bỏ dịch bệnh này vào năm 2030.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060407.jpg)

7、[United Airlines đặt mua 15 máy bay thương mại siêu thanh Overture](https://boomsupersonic.com/united)

Hãng hàng không United Airlines thông báo đã ký thỏa thuận đặt mua 15 chiếc máy bay thương mại siêu thanh Overture do hãng Boom Supersonic phát triển với mục tiêu đưa vào vận hành thương mại từ năm 2029.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060404.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060405.jpg)

Dòng máy bay siêu thanh thế hệ mới được thiết kế với sức chứa 55 hành khách, đạt tốc độ bay Mach 1.7 giúp rút ngắn một nửa thời gian bay của các chặng bay xuyên đại dương truyền thống. Boom Supersonic tuyên bố dòng máy bay này sẽ sử dụng 100% nhiên liệu sinh học hàng không để đạt mức phát thải carbon ròng bằng không.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060406.jpg)

8、[Công bố bản đồ mô phỏng mạng lưới phân bổ vật chất tối kết nối vũ trụ](https://www.vice.com/en/article/n7be77/scientists-discover-huge-voids-in-the-cosmic-web-connecting-the-universe)

Một nhóm nghiên cứu thiên văn quốc tế đã công bố mô hình bản đồ 3D mô phỏng mạng lưới phân bổ vật chất tối (dark matter web) khổng lồ kết nối vũ trụ. Các nhà khoa học tin rằng vũ trụ được liên kết với nhau bằng một mạng lưới trọng lực vô hình cấu thành từ vật chất tối, và toàn bộ các thiên thể, thiên hà sáng mà chúng ta quan sát được đều phân bổ bám dọc theo các sợi tơ của mạng lưới vô hình này.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060315.jpg)

## 文章

1、[Phỏng vấn chuyên gia về đàn voi hoang dã di chuyển bất thường tại Vân Nam](http://wap.xinmin.cn/content/31969939.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060913.jpg)

Bài trao đổi cùng chuyên gia bảo tồn động vật hoang dã tại vườn quốc gia Tây Song Bản Nạp lý giải các nguyên nhân đàn voi châu Á di chuyển liên tục hàng trăm km lên phía Bắc - một hành vi bất thường chưa từng được ghi nhận trong lịch sử tập tính của loài voi tại khu vực.

2、[Dự án ứng dụng công nghệ VR phục dựng kinh đô Trường An thời Đường](https://www.gcores.com/articles/137634)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060105.jpg)

Tác giả chia sẻ chi tiết các tài liệu khảo cổ cổ và các công cụ đồ họa 3D được ứng dụng để phục dựng lại cấu trúc quy hoạch đô thị, các phường xã của kinh thành Trường An thời nhà Đường phục vụ phát triển game thế giới mở trên nền tảng Steam.

3、[Lần theo định vị Find My để bắt giữ kẻ trộm Macbook](https://www.douban.com/note/803274306/)（Tiếng Trung）

Một bài viết chia sẻ kinh nghiệm thực tế sinh động của tác giả khi bị trộm mất máy tính Macbook, đã tận dụng hệ thống định vị Find My để lần theo dấu vết di chuyển của thiết bị và báo cảnh sát bắt giữ thành công đối tượng tiêu thụ đồ gian.

4、[Đánh giá trải nghiệm thực tế dịch vụ Internet vệ tinh Starlink](https://www.theverge.com/22435030/starlink-satellite-internet-spacex-review)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060304.jpg)

Tác giả chia sẻ chi tiết các bước lắp đặt chảo thu sóng vệ tinh Starlink tại nhà và đánh giá hiệu năng thực tế. Kết luận là tốc độ download khá cao nhưng kết nối rất dễ bị gián đoạn ngắn (micro-disconnect) khi có mây dày hoặc gió lớn lay động chảo thu, không phù hợp cho các tác vụ thời gian thực như chơi game online hay họp video.

5][Claude Shannon: Cha đẻ của Thuyết thông tin](https://spectrum.ieee.org/tech-history/cyberspace/claude-shannon-tinkerer-prankster-and-father-of-information-theory)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052415.jpg)

Bài viết chia sẻ các giai thoại thú vị về nhà khoa học Claude Shannon. Bài viết tiết lộ câu chuyện ông chọn thuật ngữ "entropy" để mô tả đại lượng đo lường độ hỗn loạn của thông tin đơn giản vì đây là từ có định nghĩa toán học mơ hồ nên ít bị các nhà khoa học khác phản bác.

6、[UC Browser tự ý thu thập dữ liệu người dùng ở chế độ ẩn danh](https://hookgab.medium.com/ucbrowser-privacy-study-ecff96fbcee4)（Tiếng Anh）

Một chuyên gia bảo mật phân tích luồng dữ liệu mạng của trình duyệt di động UC Browser và phát hiện phần mềm vẫn tự động gửi các dữ liệu định danh thiết bị và lịch sử truy cập web lên máy chủ quảng cáo ngay cả khi người dùng đang bật chế độ duyệt web ẩn danh (incognito mode).

7、[Giới thiệu công nghệ chạy Node.js native trên trình duyệt WebContainers](https://blog.stackblitz.com/posts/introducing-webcontainers/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052102.jpg)

StackBlitz giới thiệu công nghệ đột phá WebContainers sử dụng WebAssembly hỗ trợ khởi tạo và chạy trực tiếp môi trường Node.js đầy đủ ngay trên trình duyệt web Front-end, giúp lập trình viên có thể code và chạy thử các framework backend không cần cài đặt node cục bộ trên máy.

8、[Tại sao lập trình viên máy tính lại vô cùng yêu thích cà phê?](https://nerdlettering.com/blogs/articles/why-do-programmers-love-coffee)（Tiếng Anh）

Tổng hợp các phân tích về sinh lý học và văn hóa làm việc của ngành công nghệ giải thích lý do tại sao chất caffeine trong cà phê lại trở thành "nguyên liệu vận hành" không thể thiếu giúp các coder duy trì sự tập trung cao độ khi gõ code.

## 工具

1、[WireGuard Easy](https://github.com/WeeJeWel/wg-easy)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052401.jpg)

Bộ công cụ hỗ trợ cài đặt và quản lý giao thức mạng riêng ảo WireGuard trên hệ điều hành Linux một cách nhanh chóng, đi kèm giao diện quản trị Web UI trực quan để cấp phát và quản lý các file cấu hình client.

2、[Vosk](https://alphacephei.com/vosk/index.zh)

Thư viện nhận diện giọng nói ngoại tuyến (offline speech recognition) gọn nhẹ hỗ trợ hơn 18 ngôn ngữ khác nhau (bao gồm cả tiếng Trung) với dung lượng chỉ khoảng 50MB, dễ dàng tích hợp vào các script điều khiển hoặc bot chat.

3、[PINTR](https://javier.xyz/pintr/)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052103.jpg)

Một công cụ trực tuyến giúp chuyển đổi các bức ảnh chụp thông thường sang phong cách tranh vẽ nét mực vector tối giản (line art) rất nghệ thuật.

4、[Grafar](https://thoughtspile.github.io/grafar)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021050406.jpg)

Thư viện JavaScript chuyên dụng hỗ trợ vẽ và trực quan hóa các phương trình, hàm số và sơ đồ toán học phức tạp dưới dạng đồ thị 3D tương tác tốt trên trình duyệt.

5、[Mockoon](https://mockoon.com/)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021050401.jpg)

Phần mềm máy tính nguồn mở giúp lập trình viên dễ dàng thiết lập các mock server API chạy local phục vụ quá trình phát triển và kiểm thử Front-end nhanh chóng.

6、[Kakoune](http://kakoune.org/)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060204.jpg)

Trình soạn thảo văn bản chạy trên terminal sở hữu cú pháp điều khiển ngắn gọn, hỗ trợ tính năng chọn nhiều con trỏ cùng lúc (multiple selections) và hướng phím thuận tiện tương tự như Vim.

7、[GitHubPoster](https://github.com/yihong0618/GitHubPoster)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060912.jpg)

Công cụ đắc lực hỗ trợ tự động quét và thu thập lịch sử hoạt động của người dùng trên nhiều nền tảng dịch vụ web khác nhau để sinh ra biểu đồ đóng góp dạng ô vuông heatmap tương tự như GitHub. (Đóng góp của [@yihong0618](https://github.com/ruanyf/weekly/issues/1790))

8、[Apitest](https://github.com/sigoden/apitest/blob/master/README.zh-CN.md)

Tiện ích dòng lệnh CLI hỗ trợ chạy tự động hóa các kịch bản kiểm thử API thông qua tệp cấu hình JSON/YAML. (Đóng góp của [@sigoden](https://github.com/ruanyf/weekly/issues/1788))

9、[hacker-feeds-cli](https://github.com/Mayandev/hacker-feeds-cli)

Trình đọc tin tổng hợp thông tin từ các trang tin công nghệ phổ biến như Hacker News, Reddit, V2EX hiển thị trực tiếp trên màn hình dòng lệnh terminal. (Đóng góp của [@Mayandev](https://github.com/ruanyf/weekly/issues/1787))

## Tài nguyên

1、[freesound.org: Kho chia sẻ âm thanh môi trường xung quanh](https://freesound.org/)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052409.jpg)

Nền tảng cộng đồng chia sẻ hơn 500.000 tệp tin ghi âm âm thanh môi trường thực tế (ambient sound) từ khắp nơi trên thế giới do người dùng tự nguyện đóng góp (như tiếng xe buýt Bắc Kinh, tiếng tàu hỏa qua rào chắn đường sắt).

2、[Can I email](https://www.caniemail.com/)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021051107.jpg)

Trang web hữu ích giúp các lập trình viên Front-end tra cứu nhanh khả năng hỗ trợ các thuộc tính HTML/CSS khi thiết kế các mẫu email template hiển thị trên các trình đọc thư.

3、[Battlesnake](https://play.battlesnake.com/)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060308.jpg)

Một trò chơi lập trình trực tuyến thú vị: người chơi sẽ viết các thuật toán điều hướng di chuyển cho chú rắn của mình thông qua API để thi đấu trực tiếp cùng các thuật toán của người chơi khác.

4、[How to set up data science development environment](https://whiteboxml.com/blog/the-definitive-data-scientist-environment-setup)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060307.jpg)

Cẩm nang hướng dẫn chi tiết từng bước thiết lập môi trường lập trình Python, Anaconda và Jupyter Notebook phục vụ nghiên cứu khoa học dữ liệu.

## 图片和视频

1、[Ảnh đạt giải cuộc thi Nhiếp ảnh Trái Đất từ không trung của NASA](https://earthobservatory.nasa.gov/tournament-earth/results)

Tác phẩm ghi lại hình ảnh hồ nước kiềm lớn nhất thế giới - hồ Van (Thổ Nhĩ Kỳ) nhìn từ Trạm Vũ trụ Quốc tế (ISS) hiển thị rõ nét các xoáy nước trầm tích cacbonat tuyệt đẹp:

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021051405.jpg)

2、[Loa từ tính ferrofluid nhảy theo nhạc](https://hackaday.io/project/179136-ferrofluid-display-cell-bluetooth-speaker)

Một dự án chế tạo loa Bluetooth độc đáo của một nhà sáng chế người Hàn Quốc: bên trong loa tích hợp một khoang chứa chất lỏng từ tính (ferrofluid) tự động biến đổi hình học chuyển động nhảy múa theo nhịp điệu âm nhạc dưới sự điều khiển của từ trường biến thiên.

3、[Tác phẩm ảnh siêu thực Escher-style của Erik Johansson](https://www.facebook.com/photo/?fbid=311674710320284)

Nhiếp ảnh gia người Thụy Điển Erik Johansson chia sẻ tác phẩm ảnh siêu thực mới nhất của mình, ghép nối các góc sàn gỗ gác mái của gia đình thành một cấu trúc không gian đa chiều không tưởng nhưng hiển thị vô cùng tự nhiên:

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021051810.jpg)

## Bài đọc thêm

### Bức thư email lịch sử năm 2007 mở đường cho sự ra đời của App Store

*Vụ kiện pháp lý căng thẳng giữa Apple và hãng Epic Games đã làm hé lộ nhiều tệp tin email nội bộ chưa từng công bố trước đây của Apple, tiêu biểu là bức thư của phó chủ tịch Bertrand Serlet gửi Steve Jobs vào tháng 10 năm 2007:*

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061001.jpg)

iPhone thế hệ đầu tiên ra mắt tháng 1 năm 2007 được Steve Jobs thiết kế theo mô hình phần cứng và phần mềm khép kín hoàn toàn, máy chỉ chạy được 16 ứng dụng cài sẵn của hệ điều hành.

Steve Jobs ban đầu cực kỳ phản đối việc cho phép các ứng dụng từ bên thứ ba chạy native trên iOS. Ông đề xuất các lập trình viên muốn viết ứng dụng cho iPhone nên phát triển các Web App chạy trực tiếp trên trình duyệt Safari:

> *"Chúng tôi không có kế hoạch cung cấp SDK cho các bạn. Nếu các bạn làm chủ các tiêu chuẩn Web hiện đại, các bạn hoàn toàn có thể viết ra các ứng dụng tuyệt vời chạy tốt trên Safari của iPhone ngay lập tức."*

Tuy nhiên giới phát triển phần mềm không đồng ý với lập luận đó của Jobs. Phong trào bẻ khóa (jailbreak) iPhone rầm rộ nổ ra nhằm cài đặt các ứng dụng native từ bên ngoài. Cách duy nhất để Apple kiểm soát tình hình là phải chính thức phát hành bộ công cụ SDK phát triển ứng dụng chính quy.

Để thuyết phục Steve Jobs thay đổi tư duy khép kín này, phó chủ tịch phụ trách công nghệ phần mềm lúc bấy giờ là Bertrand Serlet đã viết một email gửi Jobs đề xuất thiết lập hệ thống SDK chính quy cho iPhone dựa trên bốn tiêu chí bảo mật cốt lõi:

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060701.jpg)

1. Chỉ cho phép các ứng dụng được cấp phép chính thức chạy trên máy để bảo vệ an toàn cho người dùng.
2. Phân quyền truy cập tài nguyên hệ thống nghiêm ngặt cho ứng dụng (sandbox) để bảo vệ hệ điều hành.
3. Cung cấp bộ công cụ phát triển phần mềm chuẩn hóa (SDK) trên hệ điều hành macOS đi kèm giả lập (simulator) và gỡ lỗi (debugger).
4. Thiết lập hệ thống API ổn định lâu dài.

Steve Jobs đã phản hồi email này ngắn gọn: *"Đồng ý, miễn là toàn bộ các nội dung này phải sẵn sàng để ra mắt tại sự kiện Macworld vào ngày 15 tháng 1 năm 2008."*

Quyết định đồng ý lịch sử này đã mở đường cho bộ SDK chính thức ra mắt vào tháng 3 năm 2008 và kho ứng dụng App Store đi vào vận hành từ tháng 7 năm 2008. Sự thành công vượt bậc của App Store không chỉ thúc đẩy giá trị vốn hóa của Apple tăng trưởng gấp hàng chục lần mà còn khai sinh ra cả một nền công nghiệp ứng dụng di động khổng lồ với sự ra đời của các kỳ lân công nghệ như Instagram, Uber, Spotify...

## 言论

1、

Vào năm 1919, nhà thiên văn học Arthur Eddington đã sử dụng dữ liệu quan sát hiện tượng nhật thực toàn phần để lần đầu tiên chứng minh bằng thực nghiệm tính đúng đắn của thuyết tương đối tổng quát của Albert Einstein. Thời bấy giờ rất ít người có thể hiểu được thuyết tương đối. Một nhà vật lý học đã nói đùa với Eddington: *"Thưa giáo sư, ngài chắc hẳn là một trong ba người duy nhất trên thế giới hiểu được thuyết tương đối"*. Eddington đã hóm hỉnh đáp lại: *"Tôi cũng đang tự hỏi không biết người thứ ba kia là ai đây"*.

-- Trích giai thoại vật lý

2、

Dữ liệu thống kê của Cloudflare chỉ ra rằng người dùng Internet trung bình mất khoảng 32 giây để hoàn thành một mã xác thực hình ảnh CAPTCHA chống bot. Nếu giả định trung bình một người gặp mã CAPTCHA một lần sau mỗi 10 ngày, thì với quy mô hơn 4,6 tỷ người dùng Internet toàn cầu hiện nay, nhân loại đang tiêu tốn tổng cộng khoảng **500 năm tuổi thọ mỗi ngày** chỉ để thực hiện việc bấm chọn các hình ảnh CAPTCHA phiền phức trên các website.

-- Trích bài phân tích về việc thay thế mã CAPTCHA

## 历史上的本周

- 2020年（第 111 期）：[Tìm hiểu các sai lầm phổ biến khi chọn mua Smart TV](http://www.ruanyifeng.com/blog/2020/06/weekly-issue-111.html)
- 2019年（第 59 期）：[Tại sao kỷ nguyên Internet lại khiến việc kết giao bạn bè trở nên khó khăn?](http://www.ruanyifeng.com/blog/2019/06/weekly-issue-59.html)
- 2018年（第 8 期）：[Liệu các phòng thí nghiệm trong tương lai có thể tự nhân bản con người?](http://www.ruanyifeng.com/blog/2018/06/weekly-issue-8.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
