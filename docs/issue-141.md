# 科技爱好者周刊（第 141 期）：封闭系统的胜利

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1580) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010101.jpg)

Vào ngày 21 tháng 7 năm 2020, tên lửa Falcon 9 của SpaceX chuẩn bị cất cánh đưa vệ tinh quân sự lên quỹ đạo. Ngay phía trên tên lửa, sao chổi NEOWISE đang vạch một đường sáng rực rỡ qua bầu trời đêm. Bức ảnh này đã được nhiều tạp chí bình chọn là tác phẩm nhiếp ảnh vũ trụ xuất sắc nhất trong năm. (Nguồn: [Twitter của SpaceX](https://twitter.com/spacex/status/1285264295417110528))

## 主带话题：Sự trỗi dậy của các hệ thống đóng

Một trong những sự kiện công nghệ nổi bật nhất năm ngoái là việc Apple chính thức ra mắt chip M1 tự phát triển.

Hiệu năng của M1 thực sự xuất sắc ngoài mong đợi: tốc độ xử lý nhanh hơn, tiết kiệm điện năng vượt trội và chi phí rẻ hơn đáng kể so với dòng chip Intel mà Apple sử dụng trước đó.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010501.jpg)

Tại sao chip M1 lại có hiệu năng vượt trội như vậy?

**Một [nguyên nhân cốt lõi](https://debugger.medium.com/why-is-apples-m1-chip-so-fast-3262b158cba2) là M1 không đơn thuần là một CPU truyền thống mà là một hệ thống trên một vi mạch** (System on a Chip - SoC). Nó tích hợp toàn bộ CPU, GPU, NPU (xử lý trí tuệ nhân tạo), chip bảo mật Secure Enclave và bộ nhớ RAM vào chung một tấm silicon duy nhất.

Công nghệ chế tạo bán dẫn hiện đại đã đạt đến mức độ phi thường, cho phép tích hợp hàng chục tỷ bóng bán dẫn vào một diện tích nhỏ bằng móng tay. Trước đây, các bộ phận này cần các con chip riêng biệt kết nối qua bo mạch chủ, nay đã được tích hợp làm một.

Nhờ đặt tất cả linh kiện cạnh nhau trên một đế chip duy nhất, Apple có thể tối ưu hóa thiết kế đường chạy tín hiệu ở mức tối đa, tăng tốc độ trao đổi dữ liệu giữa các bộ phận lên cực nhanh và giảm hao phí điện năng do truyền dẫn. Hơn nữa, do Apple tự kiểm soát cả hệ điều hành, họ có thể chỉnh sửa sâu ở tầng nhân (kernel) để tối ưu hoàn hảo cho cấu trúc phần cứng mới này.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010502.jpg)

Câu hỏi đặt ra là: Khi M1 gặt hái thành công lớn, các công ty đối thủ sẽ phản ứng ra sao?

Câu trả lời rất rõ ràng: Họ bắt buộc phải chạy theo. Intel, AMD, Samsung, Huawei... sẽ không thể tiếp tục chỉ bán các CPU đơn lẻ cho các hãng lắp ráp mà buộc phải tự thiết kế các SoC tích hợp riêng của mình để tối ưu hóa hiệu năng thiết bị.

Việc Nvidia nỗ lực thâu tóm ARM gần đây cũng nằm trong toan tính này nhằm tích hợp sâu GPU của họ với kiến trúc CPU của ARM để đối phó với Apple. Có [tin tức](https://www.tomshardware.com/news/google-developing-own-processors-for-smartphones-and-chromebooks) cho biết Google cũng đang tự thiết kế SoC riêng để trang bị cho dòng điện thoại Pixel và máy tính Chromebook.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010503.jpg)

Sự phổ cập của SoC sẽ dẫn đến một hệ quả tất yếu: Vì nó tích hợp quá nhiều chức năng với các giao thức kết nối tự tùy biến khép kín như một "hộp đen", nên **phần cứng máy tính cá nhân sẽ chuyển dịch hoàn toàn từ hệ thống mở sang các hệ thống đóng專有 (proprietary).** Điều này tương tự như thực trạng của thế giới smartphone hiện nay.

Không ai có thể tự sửa hay nâng cấp phần cứng Apple, các giao thức kết nối và thông số kỹ thuật đều được giữ kín. Tương lai phần cứng máy tính của các hãng khác cũng sẽ trở thành các hộp đen khép kín tương tự.

Kỷ nguyên tự ráp PC cá nhân (compatible PC) sẽ dần đi đến hồi kết. Người dùng sẽ không thể tự mua card đồ họa rời về nâng cấp vì nó đã được đúc thẳng vào SoC của nhà sản xuất. Đối với hệ điều hành mở như Linux, việc viết driver hỗ trợ các dòng SoC khép kín và không mã nguồn mở này sẽ ngày càng khó khăn hơn.

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010504.jpg)

Không chỉ phần cứng, thế giới phần mềm từ lâu đã chuyển dịch sang mô hình đóng. Trước đây, chỉ cần một trình duyệt web là bạn có thể tiếp cận mọi dịch vụ mạng. Nhưng hiện nay WeChat, Toutiao, Douyin/TikTok... đều khóa nội dung trong ứng dụng riêng của họ, bắt buộc bạn phải cài app mới xem được nội dung và không hề hỗ trợ xem trên web. Và thực tế là họ đều đã thành công rực rỡ với mô hình đóng này.

Xu hướng này đang lan rộng, biến Internet từ một mạng lưới kết nối mở, tự do thành các "hòn đảo thông tin" biệt lập. Giấc mơ về một thế giới số tự do, kết nối thông suốt đang trở nên xa vời hơn bao giờ hết dưới sự chi phối của các tập đoàn khổng lồ kiểm soát toàn bộ hệ sinh thái khép kín.

## Cẩm nang phỏng vấn dành cho lập trình viên

Phỏng vấn ứng tuyển luôn là bước ngoặt quyết định để bạn có được công việc mơ ước.

Nhiều bạn lập trình viên trẻ thường mong muốn có một chương trình định hướng chia sẻ chi tiết từ chính các nhà quản lý, các trưởng nhóm công nghệ về tiêu chí chấm điểm ứng viên, những lỗi cần tránh khi làm bài test kỹ thuật và cách thức chuẩn bị cho các vòng phỏng vấn thực tế.

Tuần này, chúng tôi giới thiệu chuyên đề **《Cẩm nang phỏng vấn Big Tech dành cho lập trình viên》** được chia sẻ bởi 4 chuyên gia công nghệ và cũng là các nhà tuyển dụng lâu năm:
- **Kiều Tân Lượng** (Cựu Phó chủ tịch Suning Technology Group)
- **Tả Nhĩ Thính Hử / Chen Hao** (Lập trình viên nổi tiếng tại Trung Quốc)
- **Bạch Hải Phi** (Trưởng bộ phận thương mại phần mềm IBM)
- **Tang Man** (Trưởng nhóm xử lý dữ liệu PayPal)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010624.jpg)

Bộ tài liệu gồm 12 bài giảng chuyên sâu xoay quanh các chủ đề thiết thực: Cách đánh giá khi chuyển đổi môi trường làm việc, sự khác biệt giữa công ty lớn và startup, quy trình chuẩn bị CV và kỹ năng giao tiếp trong phỏng vấn kỹ thuật.

Ngoài ra, chương trình còn tổ chức các buổi livestream định kỳ trao đổi trực tiếp giải đáp thắc mắc cho học viên. Khóa học được chia sẻ với mức phí tượng trưng **0.99 NDT** dành riêng cho 100 học viên đăng ký đầu tiên qua việc quét mã QR trên ảnh:

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010625.jpg)

## Tin tức

1、[Thiết bị gối tựa đầu chống ồn chủ động](https://spectrum.ieee.org/tech-talk/consumer-electronics/audiovideo/active-noise-cancellation-using-ldvs)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122802.jpg)

Nguyên lý của tai nghe chống ồn chủ động (ANC) là phát ra sóng âm cùng tần số nhưng ngược pha để triệt tiêu tiếng ồn bên ngoài. Các nhà nghiên cứu tại Đại học Công nghệ Sydney đã ứng dụng nguyên lý này để chế tạo một chiếc gối tựa đầu chống ồn lắp sau ghế ngồi, giúp người dùng không cần đeo tai nghe vẫn có được không gian yên tĩnh.

Gối tựa đầu tích hợp các loa phát siêu nhỏ hướng thẳng vào tai người ngồi để phát sóng âm khử ồn, giúp giảm tiếng ồn xung quanh từ 10 đến 20 decibel. Điểm hạn chế hiện tại là người dùng phải tựa đầu cố định vào gối; nếu quay đầu đi hướng khác, chùm sóng âm sẽ lệch khỏi tai. Nhóm nghiên cứu đang phát triển hệ thống camera theo dõi chuyển động đầu để điều chỉnh hướng sóng âm tự động.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122803.jpg)

2、[Cơ chế đánh giá chất lượng sản phẩm định kỳ dài hạn](https://www.buyforlife.com/blog/4kpaLtbnG6MkseMj44niVV/recurring-reviews-to-track-the-whole-lifecycle-of-a-product)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122905.jpg)

Các đánh giá sản phẩm trên các trang thương mại điện tử thường chỉ phản ứng cảm xúc ban đầu của khách hàng ngay khi mở hộp và chưa phản ánh được độ bền thực tế của sản phẩm. Một trang bán hàng trực tuyến của Mỹ đã đưa vào thử nghiệm tính năng "Đánh giá định kỳ" (Recurring Reviews).

Sau khi khách hàng mua một sản phẩm bền (như ba lô, nồi chảo, giày dép), hệ thống sẽ gửi email tự động hàng năm để nhờ khách hàng chụp ảnh tình trạng sử dụng hiện tại và viết cảm nhận sau 1 năm, 2 năm hoặc 5 năm sử dụng. Hình ảnh trên là trạng thái sản phẩm sau 2 tháng, 2 năm và 5 năm sử dụng thực tế của một khách hàng, giúp người mua sau có cái nhìn trực quan nhất về tuổi thọ sản phẩm.

3、[Dự án chế tạo vệ tinh bằng gỗ thân thiện môi trường](https://www.bbc.com/news/business-55463366)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122909.jpg)

Lượng vệ tinh nhân tạo được phóng lên quỹ đạo ngày một nhiều và khi hết hạn sử dụng, phần lớn chúng sẽ rơi lại và bốc cháy trong bầu khí quyển Trái Đất. Quá trình bốc cháy của các vật liệu kim loại và composite sinh ra các hạt bụi nhôm siêu mịn lơ lửng ở tầng thượng quyển gây ảnh hưởng xấu đến môi trường.

Để giải quyết vấn đề này, Đại học Kyoto đã hợp tác với một doanh nghiệp lâm nghiệp Nhật Bản để nghiên cứu phát triển vỏ vệ tinh bằng gỗ đặc biệt chịu nhiệt. Mục tiêu của dự án là phóng vệ tinh vỏ gỗ đầu tiên vào năm 2023. Khi kết thúc nhiệm vụ rơi lại bầu khí quyển, toàn bộ vỏ gỗ sẽ cháy sạch hoàn toàn không để lại tàn dư kim loại gây hại.

4、[Người liệt điều khiển đồng thời hai cánh tay giả bằng sóng não](https://neurosciencenews.com/bci-prosthetic-limb-movement-17423/)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122203.jpg)

Đầu năm 2019, các nhà khoa học tại Đại học Johns Hopkins đã tiến hành cấy ghép 6 cảm biến điện cực siêu nhỏ vào vùng vỏ não vận động của một bệnh nhân bị liệt tứ chi suốt 30 năm.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122202.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122201.jpg)

Sau hai năm kiên trì tập luyện tương tác với máy tính, bệnh nhân này đã có thể sử dụng ý nghĩ điều khiển đồng thời cả hai cánh tay robot phối hợp thực hiện các động tác khéo léo cơ bản như cầm dao dĩa tự cắt thức ăn và đưa vào miệng của mình. Mục tiêu tiếp theo của dự án là giúp bệnh nhân thực hiện các nhiệm vụ không cần nhìn bằng mắt (như tự buộc dây giày).

5、[Ba Lan sử dụng loài trai sông để giám sát nước sạch tự nhiên](https://www.polishnews.co.uk/poznan-the-clams-filter-the-water-they-check-whether-the-water-is-polluted-or-clean/)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020123107.jpg)

Nhiều năm qua, thành phố Poznań của Ba Lan vẫn duy trì một phương pháp kiểm tra nước sinh hoạt độc đáo bằng cách sử dụng các chú trai sông làm "lính gác". Phương pháp sinh học này rẻ hơn rất nhiều so với dùng máy đo hóa chất mà độ nhạy bén rất cao. Loài trai sông nhạy cảm với kim loại nặng và hóa chất độc hại, chúng sẽ khép chặt vỏ ngay khi phát hiện nguồn nước bị ô nhiễm.

Nhà máy nước bố trí 3 trạm giám sát, mỗi trạm thả 8 con trai sông được gắn các cảm biến nam châm siêu nhẹ trên vỏ để ghi nhận trạng thái đóng mở vỏ. Nếu chỉ 1-2 con khép vỏ thì có thể là hành vi tự nhiên, nhưng nếu cả 8 con đồng loạt đóng vỏ thì hệ thống sẽ tự động ngắt van cấp nước chính và phát cảnh báo nguy hiểm khẩn cấp. Mỗi năm nhà máy sử dụng khoảng 200 chú trai sông luân phiên làm nhiệm vụ.

6、**Tin tức một câu**

> - Fujifilm công bố công nghệ sản xuất băng từ lưu trữ thế hệ mới đạt dung lượng kỷ lục 580 TB trên một cuộn băng dệt từ hạt Barium Ferrite, gấp 50 lần dung lượng băng từ lưu trữ thương mại hiện nay.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122902.jpg)

> - Cơ quan JAXA của Nhật Bản công bố hình ảnh thực tế những hạt cát đen đầu tiên thu gom từ bề mặt tiểu hành tinh Ryugu cách Trái Đất 300 triệu km mang về bởi tàu Hayabusa-2.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122903.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122904.jpg)

> - Một doanh nghiệp Mỹ giới thiệu dòng máy kéo chạy điện thông minh Monarch Tractor giá 50.000 USD có khả năng tự động cày ruộng không cần người lái liên tục trong 10 tiếng, hướng tới giải pháp nông nghiệp sạch không khí thải dầu diesel có hại cho cây trồng.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121710.jpg)

> - Các nhà nghiên cứu tại Đại học Oxford sử dụng mô hình học máy phân tích ảnh chụp vệ tinh có độ phân giải cao để nhận diện và thống kê số lượng đàn voi trên các cánh đồng cỏ châu Phi nhằm phục vụ công tác bảo tồn động vật hoang dã. Vệt khung xanh là AI nhận diện và khung đỏ là kết quả đối chiếu thực tế.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122503.jpg)

> - Hàn Quốc công bố số liệu năm 2020 ghi nhận lần đầu tiên quốc gia này có tỷ lệ tăng trưởng dân số tự nhiên ở mức âm, gia nhập nhóm các nước có tốc độ già hóa dân số nhanh nhất thế giới cùng Nhật Bản.

## Bài viết

1、[Nhìn lại hành trình đo đạc chiều cao thực tế của đỉnh Everest](https://mp.weixin.qq.com/s/r5kOO48Ow19uhUFDpk6iPQ)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122608.jpg)

Hình ảnh tư liệu chi tiết về hành trình của đội leo núi và các thiết bị đo đạc định vị GNSS tiên tiến được đưa lên đỉnh Everest để xác định lại chiều cao chuẩn xác của đỉnh núi vào tháng 5 năm 2020.

2、[Sử dụng ứng dụng SunCalc để định vị hình ảnh dựa vào hướng nắng](https://technews.tw/2020/12/15/the-angle-of-sunlight-and-shadow-can-reveal-where-the-photo-was-taken/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122610.jpg)

Hướng dẫn cách sử dụng công cụ tính toán SunCalc để phân tích chiều dài bóng đổ và góc chiếu của ánh sáng mặt trời trên một bức ảnh chụp, giúp suy đoán ra thời gian chụp ảnh hoặc thu hẹp vị trí chụp thực tế của bức ảnh.

3、[Cơ cấu phân bổ lại băng tần tần số vô tuyến mạng 5G tại Trung Quốc](https://www.tmtpost.com/4912205.html)（Tiếng Trung）

Bài viết phân tích thực trạng điều chỉnh băng tần số sóng vô tuyến của các nhà mạng viễn thông trong nước, tiến hành thu hồi một số băng tần 2G/3G cũ để tái sử dụng nâng cấp năng lượng phủ sóng cho mạng 5G.

4、[Khảo sát các mối nguy sinh sinh thái từ động vật hoang dã và chó mèo hoang](https://mp.weixin.qq.com/s/FZAHxaxdSBHN4XGov9QjXQ)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020123103.jpg)

Số liệu khảo sát giật mình về số lượng động vật nhỏ (chuột, chim, thằn lằn) bị săn bắt hàng năm bởi một chú mèo hoang đô thị, nhấn mạnh sự mất cân bằng sinh thái do việc bỏ rơi thú cưng ra môi trường tự nhiên.

5、[Mối tương quan cấu trúc giữa Máy trạng thái hữu hạn (FSM) và Biểu thức chính quy](https://qntm.org/plants)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122611.jpg)

Bài viết toán học trực quan giải thích sự tương đương và cách chuyển đổi qua lại giữa cấu trúc đồ thị của máy trạng thái hữu hạn và các chuỗi biểu thức chính quy (Regex).

6、[Hướng dẫn thiết lập đồng hồ số chạy trực tiếp trên Google Sheets](https://www.therobinlord.com/making-a-digital-clock-in-google-sheets/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122612.jpg)

Mẹo sử dụng các hàm công thức bảng tính và script trigger thời gian để tạo một giao diện đồng hồ hiển thị giờ phút giây tự nhảy số trực tiếp trên ô tính Google Sheets.

7、[Lập trình viên cần trang bị lượng kiến thức toán học bao nhiêu là đủ?](https://lispmachine.wordpress.com/2014/12/05/how-much-math-you-need-for-programming/)（Tiếng Anh）

Chia sẻ của một kỹ sư kỳ cựu: Bạn hoàn toàn có thể trở thành một lập trình viên giỏi làm ra sản phẩm chạy tốt mà không cần giỏi toán cao cấp, nhưng kiến thức toán học tốt sẽ mở ra cho bạn những tư duy giải quyết thuật toán thông minh và tối ưu hơn nhiều.

8、[Tại sao triết lý thiết kế "Mobile First" đôi khi chưa hẳn là giải pháp tốt nhất](https://web.archive.org/web/20201228005247if_/https://planflow.dev/blog/why-mobile-first-is-a-bad-idea)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122808.jpg)

Tác giả phản biện quan điểm thiết kế giao diện ưu tiên hiển thị di động trước rồi mới scale lên desktop, cho rằng nên thiết kế bố cục desktop hoàn chỉnh để bao quát hết thông tin rồi mới viết CSS media query co gọn lại cho di động sẽ dễ kiểm soát layout hơn.

9、[Ba trường phái tư duy triết học cốt lõi trong lập trình](https://josephg.com/blog/3-tribes/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122901.jpg)

Phân tích 3 quan điểm lập trình của cộng đồng dev: Nhóm coi viết code như một tác phẩm nghệ thuật cần sự hoàn mỹ; Nhóm coi code là công cụ điều khiển phần cứng tối ưu hiệu năng; Nhóm coi code đơn thuần là phương tiện để nhanh chóng làm ra sản phẩm giải quyết bài toán thực tế.

10、[Tự dựng máy chủ cân bằng tải (load balancer) qua Cloudflare Workers](https://justyy.com/archives/44793)（Tiếng Trung）

Hướng dẫn chi tiết viết mã nguồn JS chạy trên nền tảng Serverless Cloudflare Workers để phân phối lưu lượng truy cập qua các máy chủ đích khác nhau hoàn toàn miễn phí (giới hạn 100.000 request/tháng). ([@DoctorLai](https://github.com/ruanyf/weekly/issues/1576) đóng góp)

## 工具

1、[best-resume-ever](https://github.com/salomonelli/best-resume-ever)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020123011.jpg)

Công cụ mã nguồn mở dựa trên Vue giúp lập trình viên thiết kế CV cá nhân đẹp mắt từ các template sẵn có và xuất ra file PDF chất lượng cao qua tính năng in của trình duyệt.

2、[librephotos](https://github.com/LibrePhotos/librephotos)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020123108.jpg)

Dự án tự host lưu trữ và quản lý album ảnh gia đình mã nguồn mở, backend viết bằng Django kết hợp frontend React, hỗ trợ nhận diện khuôn mặt và phân loại địa điểm thông minh.

3、[ArtLine](https://github.com/vijishmadhavan/ArtLine)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010102.jpg)

Dự án Deep Learning xử lý hình ảnh giúp tự động chuyển đổi các bức ảnh chụp người hoặc phong cảnh thành các nét vẽ phác họa bút chì nghệ thuật. ([Demo web Flask](https://github.com/jwenjian/artline-demo) đóng góp bởi [@jwenjian](https://github.com/ruanyf/weekly/issues/1571))

4、[ssdt](https://github.com/62726164/a-survey-of-security-dot-txt)

Công cụ thu thập và thống kê thông tin liên hệ bảo mật từ tệp tin `security.txt` của top 1 triệu website lớn nhất thế giới để đánh giá mức độ tuân thủ tiêu chuẩn bảo mật.

5、[pure CSS digital clock](https://www.quaxio.com/pure_css_digital_clock.html)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010410.jpg)

Một thử nghiệm lập trình đồng hồ số đếm giờ chạy hoàn toàn bằng hiệu ứng động CSS mà không sử dụng bất kỳ dòng code JavaScript nào. Do không đọc được giờ hệ thống, đồng hồ chỉ đếm giây bắt đầu từ mốc 12 giờ mặc định.

6、[Pipedream](https://pipedream.com/)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010413.jpg)

Nền tảng tích hợp tự động hóa quy trình làm việc (workflow) kết nối các dịch vụ web qua API tương tự như Zapier hay IFTTT dành riêng cho lập trình viên.

7、[Scrollama.js](https://github.com/russellgoldenberg/scrollama)

Thư viện JavaScript gọn nhẹ dựa trên API `IntersectionObserver` hỗ trợ tạo các hiệu ứng chuyển động, hiển thị nội dung theo bước cuộn trang (scrollytelling) mượt mà.

8、[DALL-E](https://openai.com/blog/dall-e/)

OpenAI ra mắt mô hình AI thế hệ mới DALL-E có khả năng tự động sinh ra các bức ảnh vẽ chân thực, chi tiết dựa trên mô tả văn bản của người dùng:
- *Ví dụ: "Một chiếc ghế có hình quả bơ"*

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010610.jpg)

- *Ví dụ: "Mặt tiền một cửa hàng có chữ OpenAI"*

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010609.jpg)

- *Ví dụ: "Phòng ngủ áp mái có giường ngủ cạnh bể cá"*

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010611.jpg)

9、[My Icon](https://myicon.io/)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010705.jpg)

Bộ sưu tập hàng nghìn biểu tượng icon miễn phí chất lượng cao hỗ trợ người dùng tùy biến thay thế giao diện icon ứng dụng trên màn hình chính của iOS 14.

## Tài nguyên

1、[Thiết bị PCIe tương thích với Raspberry Pi 4](https://pipci.jeffgeerling.com/)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122815.jpg)

Trang web tổng hợp danh sách các thiết bị ngoại vi giao tiếp qua cổng PCI Express 1x tương thích tốt với bo mạch máy tính nhúng Raspberry Pi 4.

2、[iMac G3 và 20 sản phẩm mang tính bước ngoặt của Apple](https://sixcolors.com/post/2020/12/20-macs-for-2020-1-imac-g3/)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122908.jpg)

Chuỗi 20 bài viết tiếng Anh ôn lại lịch sử phát triển các dòng sản phẩm máy tính iMac huyền thoại của Apple kể từ ngày Steve Jobs quay lại vực dậy công ty vào năm 1998 với chiếc iMac G3 nhiều màu sắc.

3、[Linux Hardening Guide](https://madaidans-insecurities.github.io/guides/linux-hardening.html)

Tài liệu chi tiết hướng dẫn các bước tối ưu hóa cấu hình hệ thống, quản lý quyền hạn và bảo mật nhân kernel cho hệ điều hành Linux. ([@alaskasquirrel](https://github.com/ruanyf/weekly/issues/1582) đóng góp)

4、[bigdata_analyse](https://github.com/TurboWay/bigdata_analyse)

Kho lưu trữ chia sẻ các bài tập phân tích dữ liệu lớn thực tế (như xử lý hơn 100 triệu dòng log hành vi người dùng Taobao, phân tích 7.000 tin thuê nhà...). ([@TurboWay](https://github.com/ruanyf/weekly/issues/1577) đóng góp)

5、[Cẩm nang tối ưu hóa hiệu năng lập trình Go](https://github.com/geektutu/high-performance-go)

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010103.jpg)

Cuốn sách điện tử tiếng Trung miễn phí chia sẻ các mẹo tối ưu hóa bộ nhớ, quản lý goroutine để tăng hiệu năng xử lý cho ứng dụng Go. ([@geektutu](https://github.com/ruanyf/weekly/issues/1575) đóng góp)

## Hình ảnh

1、[Cùng một góc chụp qua 100 năm lịch sử tại Trung Quốc](https://petapixel.com/2016/04/09/reshot-old-photos-see-china-changed-100-years/)

Nhiếp ảnh gia Mỹ Dheera Venkatraman thực hiện hành trình tìm lại các góc chụp của các bức ảnh tư liệu cũ cách đây gần một thế kỷ để chụp lại cảnh quan hiện tại làm phép đối chiếu:

Cầu sắt Trung Sơn bắc qua sông Hoàng Hà tại Lan Châu:

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010307.jpg)

Nhà thờ Công giáo Bắc Quý Dương:

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010308.jpg)

Đê Tô Châu tại Tây Hồ, Hàng Châu:

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010309.jpg)

Ngã ba sông Nghi Tân Tam Giang:

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010310.jpg)

2、[Thiết kế bãi đỗ xe và giao thông trong các tựa game xây dựng thành phố](https://mobile.twitter.com/alfred_twu/status/1345959947452911616)

Các tựa game mô phỏng xây dựng đô thị phản ánh các tư duy quy hoạch giao thông khác nhau:

Trong *SimCity*, người chơi thường xây dựng trung tâm tài chính dày đặc cao ốc. Game mặc định giả định toàn bộ bãi đỗ xe ô tô được đưa xuống lòng đất để tiết kiệm không gian bề mặt:

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010604.jpg)

Trong *Cities Skylines*, game khuyến khích người chơi hạn chế xe cá nhân để chuyển sang dùng giao thông công cộng tàu điện, xe buýt tương tự như quy hoạch thực tế của các thành phố Bắc Âu:

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010607.jpg)

Trong tựa game *Workers & Resources: Soviet Republic*, nếu bạn cho phép người dân mua xe hơi cá nhân, bạn bắt buộc phải xây dựng các bãi đỗ xe mặt đất chiếm dụng diện tích lớn:

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010605.jpg)

Nếu không cấp xe cá nhân, khu dân cư phải được xây dựng cực kỳ nhỏ gọn để người dân đi bộ đi làm và dùng xe lửa đưa đón công nhân đến các khu công nghiệp nằm xa khu dân cư để tránh ô nhiễm:

![](https://cdn.beekka.com/blogimg/asset/202101/bg2021010606.jpg)

## Bài đọc thêm

### 1. Hành trình đổi một chiếc ghim giấy màu đỏ lấy một căn nhà

Năm 2006, chàng trai người Canada Kyle MacDonald đã thực hiện một thử nghiệm trao đổi vật phẩm trực tuyến nổi tiếng. Bắt đầu chỉ với một chiếc ghim giấy màu đỏ kẹp tài liệu, qua 14 lần giao dịch trung gian trực tuyến bằng phương thức trao đổi vật ngang giá, anh đã đổi được một căn nhà hai tầng hoàn chỉnh:

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122603.jpg)

1. 14/07/2005: Đổi chiếc ghim giấy đỏ lấy một chiếc bút hình con cá.
2. Cùng ngày: Đổi chiếc bút hình cá lấy một tay nắm cửa điêu khắc thủ công.
3. 25/07/2005: Đổi tay nắm cửa lấy một chiếc bếp du lịch kèm bình ga.
4. 24/09/2005: Đổi bếp du lịch lấy một máy phát điện Honda cũ.
5. 16/11/2005: Đổi máy phát điện lấy một thùng bia trống kèm cam kết rót đầy bia và một bảng đèn neon Budweiser.
6. 08/12/2005: Đổi bộ đèn và bia lấy một chiếc xe trượt tuyết Ski-Doo.
7. Đổi xe trượt tuyết lấy một chuyến du lịch hai người đến British Columbia.
8. 07/01/2006: Đổi chuyến du lịch lấy một chiếc xe tải chở hàng thùng kín.
9. 22/02/2006: Đổi xe tải lấy một hợp đồng thu âm của hãng đĩa.
10. 11/04/2006: Đổi hợp đồng lấy quyền thuê miễn phí 1 năm một căn hộ ở Phoenix, Arizona.
11. 26/04/2006: Đổi quyền thuê nhà lấy một buổi chiều giao lưu cùng rocker Alice Cooper.
12. 26/05/2006: Đổi buổi giao lưu lấy một quả cầu tuyết trang trí của ban nhạc Kiss.
13. 02/06/2006: Đổi quả cầu tuyết lấy một vai diễn định sẵn trong bộ phim của đạo diễn Corbin Bernsen.
14. 05/07/2006: Đổi vai diễn lấy một căn nhà hai tầng tại Saskatchewan.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122604.jpg)

Một công viên tại Saskatchewan đã dựng một bức tượng ghim giấy đỏ khổng lồ để ghi dấu sự kiện thú vị này, đồng thời xác lập kỷ lục chiếc ghim giấy lớn nhất thế giới.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020122605.jpg)

### 2. Vấn đề bán kèm tính năng sản phẩm (Bundling) của các hệ điều hành

Vào những năm 1950, một chiếc ô tô mới xuất xưởng thường chưa được trang bị đèn xi-nhan báo rẽ. Đó là một linh kiện phụ trợ mà khách hàng phải tự mua ngoài và lắp thêm sau đó.

Năm 1960 khi Ford quyết định tích hợp sẵn đài radio vào bảng táp-lô của xe, một số nhà sản xuất radio đã đâm đơn kiện Ford ra tòa, buộc tòa án phải phân xử xem đài radio là bộ phận thiết yếu cấu thành nên xe hay chỉ là linh kiện tùy chọn để tránh cạnh tranh không lành mạnh.

Tương tự vào những năm 1980, các phần mềm soạn thảo văn bản thô sơ không hề tích hợp tính năng đếm từ, tạo footnote hay in khổ ngang. Khách hàng phải mua thêm các module phụ trợ của bên thứ ba với giá từ 50-100 USD. Sau đó các nhà phát triển lớn dần tích hợp sẵn toàn bộ các tính năng này vào phần mềm chính, bóp nghẹt thị trường của các công ty con.

Ngày nay, ranh giới giữa việc hệ điều hành di động được phép tích hợp sẵn các tính năng gì (như trình duyệt, ứng dụng nghe nhạc) và quyền tự do lựa chọn của người tiêu dùng vẫn là tâm điểm tranh cãi. Phần lớn người dùng phổ thông thường giữ nguyên các thiết lập mặc định của trình duyệt và ứng dụng hệ thống mà không có nhu cầu hoặc kỹ năng để tìm hiểu cài đặt các giải pháp thay thế của bên thứ ba. Quy mô và giới hạn của một hệ điều hành tích hợp hiện nay hoàn toàn phụ thuộc vào ý chí chủ quan của các gã khổng lồ công nghệ.

## 言论

1、

Một người biết cách thực hiện công việc (know-how) sẽ luôn tìm được một công việc ổn định, nhưng người hiểu rõ tại sao phải thực hiện công việc đó (know-why) sẽ trở thành sếp của người đó.

-- John Maxwell

2、

Trào lưu thời trang nhanh thay đổi liên tục và quần áo mới ngày càng rẻ như quần áo cũ, khiến số lần mặc trung bình của một bộ đồ trước khi bị vứt bỏ giảm mạnh. Trên toàn cầu số lần mặc giảm 36%, riêng tại Trung Quốc con số này giảm tới 70%.

-- Bloomberg

3、

Nếu công nghệ tiếp tục phát triển nhanh như hiện nay, các quốc gia phát triển có dân số ít và công nghệ cao sẽ được hưởng lợi lớn. Do dân số ít, họ dễ dàng chi trả các gói an sinh xã hội cho người thất nghiệp để tập trung nguồn lực xây dựng hạ tầng cho nền kinh tế robot hóa. Ngược lại, các nước đang phát triển có dân số đông và trình độ công nghệ thấp sẽ chịu ảnh hưởng nặng nề nhất do áp lực thất nghiệp.

-- Thảo luận trên Hacker News

4、

Tôi từng rời bỏ một công ty kỳ lân công nghệ lớn để đầu quân cho một startup nhỏ. Ngay ngày đi làm đầu tiên tôi đã cảm nhận sự thụt lùi: từ một văn phòng làm việc lung linh sang một căn phòng tối tăm bừa bộn đầy linh kiện phần cứng để nghiên cứu một sản phẩm chưa rõ tương lai thương mại và phải mất nhiều năm sửa lỗi mới mong tiếp cận được thị trường.

-- Bài viết 《Từ chức sau hai tháng nhận việc》

## Nhìn lại

Tuần này năm 2020 (số 90): [Quản trị con người và quản trị công nghệ là hai năng lực hoàn toàn khác nhau](http://www.ruanyifeng.com/blog/2020/01/weekly-issue-90.html)

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120604.jpg)

Tuần này năm 2019 (số 38): [Trải nghiệm sử dụng càng đơn giản thì cấu trúc kỹ thuật bên dưới càng phức tạp](http://www.ruanyifeng.com/blog/2019/01/weekly-issue-38.html)

![](https://cdn.beekka.com/blogimg/asset/201901/bg2019010401.jpg)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
