# 科技爱好者周刊（第 170 期）：软件订阅制的胜利

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1870) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080408.jpg)

Một nhiếp ảnh gia tại Hà Lan đã chụp được khoảnh khắc vô cùng độc đáo của một chú ngỗng đang bay trong tư thế lộn ngược thân mình. Các chuyên gia điểu học giải thích đây là hành vi biểu diễn kỹ thuật bay (whiffling) thường dùng để giảm tốc độ nhanh chóng khi hạ cánh. (Nguồn: [WGME](https://wgme.com/news/offbeat/goose-flying-upside-down-is-simply-showing-off-say-experts))

## 主带话题：Sự trỗi dậy và chiến thắng của mô hình phần mềm trả phí đăng ký (Subscription)

Tuần trước, báo cáo tài chính quý mới nhất của Apple công bố một con số thống kê ấn tượng: hãng hiện sở hữu **700 triệu** người dùng trả phí đăng ký (paid subscriptions).

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080103.jpg)

Con số này thực sự rất lớn. Quy mô dân số thế giới hiện nay vào khoảng 7,8 tỷ người (bao gồm cả trẻ em, người già, người dân vùng sâu). Điều này có nghĩa là trung bình cứ 11 người trên Trái Đất thì có 1 người đang trả tiền thuê bao định kỳ cho các dịch vụ phần mềm của Apple. Liệu có mô hình kinh doanh phần mềm nào đạt được quy mô tài chính lớn hơn thế hay không?

Lưu ý đây hoàn toàn là lượng người dùng trả phí thực tế chứ không phải tài khoản miễn phí. Để so sánh, tập đoàn Alibaba mới đây công bố đạt mốc 1 tỷ người dùng hoạt động, nhưng đó là các tài khoản đăng ký miễn phí để mua sắm. Nếu mỗi tháng người dùng phải đóng một khoản phí thuê bao định kỳ để được quyền truy cập vào Taobao, không rõ số lượng người dùng trung thành còn lại sẽ là bao nhiêu.

Hệ sinh thái dịch vụ trả phí đăng ký của Apple hiện tại tập trung vào 6 dịch vụ cốt lõi:

- iCloud: Dịch vụ lưu trữ đám mây.
- Apple Music: Dịch vụ nghe nhạc trực tuyến.
- Apple TV+: Dịch vụ xem video điện ảnh trực tuyến.
- Apple News+: Dịch vụ đọc tin tức báo chí.
- Apple Fitness+: Dịch vụ hướng dẫn tập luyện sức khỏe.
- Apple Arcade: Kho trò chơi điện tử độc quyền.

Apple đã thông minh đóng gói tất cả các dịch vụ này vào một gói thuê bao chung mang tên Apple One. Doanh thu từ dịch vụ bảo hành phần cứng AppleCare không được tính vào số liệu này do được hạch toán vào doanh thu bán thiết bị phần cứng.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080104.jpg)

Điều tôi muốn nhấn mạnh ở đây không phải là chi tiết các gói dịch vụ này, mà là một xu hướng lớn đang định hình lại ngành phần mềm: **Các tập đoàn phần mềm lớn nhất thế giới đang dần khai tử mô hình bán đứt bản quyền phần mềm một lần để chuyển dịch hoàn toàn sang mô hình thu phí thuê bao đăng ký định kỳ (Software-as-a-Service - SaaS).** Apple chính là một đại diện tiêu biểu nhất cho xu hướng này.

Bên cạnh Apple, gã khổng lồ phần mềm máy tính cá nhân Microsoft cũng đang tiến hành các bước dịch chuyển tương tự. Bộ ứng dụng văn phòng Office truyền thống đã được nâng cấp thành dịch vụ đám mây Microsoft 365 thu phí thuê bao hàng năm (mức phí khoảng 398 NDT/năm tại Trung Quốc). Đồng thời, hãng chuẩn bị ra mắt dịch vụ Windows 365 để đưa toàn bộ hệ điều hành Windows lên đám mây và thu phí thuê bao sử dụng theo tháng.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080401.jpg)

Hãng Adobe từ vài năm trước cũng đã khai tử bộ cài Creative Suite bán đứt để chuyển sang Creative Cloud thu phí đăng ký thuê bao hàng năm. Gói phần mềm Photoshop chuyên nghiệp hiện có mức phí đăng ký hàng năm khá cao.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080402.jpg)

Tôi tin rằng **mô hình trả phí đăng ký (subscription) chính là tương lai không thể đảo ngược của thương mại số.** Đối với các doanh nghiệp phần mềm, mô hình này mang lại nguồn doanh thu định kỳ lặp lại (Recurring Revenue) vô cùng ổn định thay vì phụ thuộc vào doanh số bán đứt bấp bênh theo từng phiên bản. Nó giúp doanh nghiệp có dòng tiền mặt dự báo trước tốt để tái đầu tư. Thêm vào đó, việc người dùng luôn sử dụng phiên bản cập nhật mới nhất trên đám mây giúp đội ngũ kỹ sư không còn phải tốn tài nguyên bảo trì các phiên bản cũ lạc hậu.

Ngược lại, đối với người dùng phổ thông, mô hình này có phần kém tối ưu hơn. Trước đây, khi mua một bản quyền phần mềm, bạn có thể cài đặt và sử dụng nó ổn định suốt 5-10 năm mà không phát sinh thêm chi phí. Hiện nay, bạn bắt buộc phải chi trả hàng tháng/hàng năm. Nếu dừng đóng phí, bạn lập tức mất quyền truy cập vào phần mềm và thậm chí không thể mở các file định dạng đặc thù lưu trữ công việc cũ của mình (ví dụ như các tệp PSD của Photoshop).

Không chỉ phần mềm, xu hướng này đang mở rộng sang mọi hàng hóa dịch vụ số có tính tiêu dùng lâu dài. Mới đây, gã khổng lồ giáo dục Pearson đã ra mắt dịch vụ Pearson+ cho phép sinh viên Mỹ trả phí thuê bao 14,99 USD/tháng để được toàn quyền truy cập, tra cứu, ghi chú và nghe sách nói của hơn 1,500 đầu giáo trình đại học của hãng:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080403.jpg)

Tóm lại: **Mọi sản phẩm có thể số hóa được trong tương lai đều sẽ chuyển dịch sang mô hình thu phí đăng ký thuê bao định kỳ.** Người tiêu dùng sẽ dần quen với việc thanh toán hóa đơn thuê bao phần mềm hàng tháng tương tự như hóa đơn tiền điện, tiền nước sinh hoạt.

## Công cụ quản lý tài liệu ShowDoc

Tuần này chúng tôi giới thiệu đến các bạn một công cụ quản lý tài liệu chất lượng cao do các lập trình viên trong nước phát triển mang tên **ShowDoc**. Bản tin thường xuyên hỗ trợ giới thiệu các sản phẩm phần mềm nguồn mở hữu ích, các tác giả có nhu cầu kết nối xin liên hệ (Email: yifeng.ruan@gmail.com).

Giới công nghệ thường chia sẻ câu nói vui về tầm quan trọng của tài liệu hướng dẫn phát triển phần mềm:

> *Lập trình viên ghét hai việc: viết tài liệu hướng dẫn và việc dự án không có tài liệu hướng dẫn.*

Một công cụ viết tài liệu tốt sẽ giúp giảm thiểu tối đa gánh nặng ghi chép mã nguồn cho các kỹ sư và nâng cao hiệu quả làm việc nhóm. **ShowDoc** chính là giải pháp được thiết kế tối ưu cho nhu cầu này. Hiện tại công cụ đã thu hút hơn 100.000 đội ngũ lập trình viên trong nước tin dùng (bao gồm cả các team dự án nội bộ của Tencent, Huawei, Baidu, ByteDance).

ShowDoc giải quyết triệt để bài toán của các nhóm phát triển tinh gọn hoặc cá nhân: Cung cấp một trung tâm lưu trữ tài liệu trực quan, dễ dàng tạo mới, tìm kiếm phân loại tài liệu nhanh chóng bằng Markdown, phân quyền biên soạn rõ ràng và hỗ trợ ứng dụng đa nền tảng (desktop, mobile):

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070603.jpg)

Mã nguồn của ShowDoc được công bố hoàn toàn miễn phí trên [GitHub](https://github.com/star7th/showdoc) và đã đạt mốc hơn 9.000 sao, khẳng định độ uy tín tin cậy của sản phẩm:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070605.jpg)

Nếu sở hữu máy chủ riêng, bạn có thể dễ dàng deploy ShowDoc chỉ bằng một dòng lệnh Docker tự động cài đặt. Hệ thống cũng hỗ trợ chạy trên môi trường Windows. Sau khi khởi chạy, bạn chỉ cần truy cập địa chỉ `localhost:4999` trên trình duyệt là đã sở hữu một wiki tài liệu hoàn chỉnh:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070604.jpg)

Bên cạnh các tính năng soạn thảo văn bản và bảng tính thông thường, ShowDoc cung cấp hai công cụ tự động hóa vô cùng đắt giá cho dân kỹ thuật:
1. **Tự động sinh tài liệu API:** Hỗ trợ quét các comment chú thích trong mã nguồn để tự động biên dịch thành tài liệu API chi tiết.
2. **Tự động xuất sơ đồ cơ sở dữ liệu:** Hỗ trợ kết nối database để tự cấu hình hiển thị sơ đồ các bảng dữ liệu (data dictionary).

Để tối ưu hóa luồng làm việc với API, đội ngũ phát triển còn cung cấp ứng dụng khách **RunApi** miễn phí hỗ trợ gửi test request và sinh Mock dữ liệu tương tự Postman, tự động đồng bộ kết quả kiểm thử thành tài liệu trên ShowDoc:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071313.jpg)

ShowDoc hỗ trợ xuất dữ liệu ra định dạng Word hoặc Markdown. Nếu không muốn tự host vận hành máy chủ, bạn có thể đăng ký sử dụng phiên bản Cloud trực tuyến miễn phí của hãng dành cho các nhóm dưới 5 thành viên.

## 科技动态

1、[Tháp quạt lọc không khí khổng lồ tại New Delhi](https://techxplore.com/news/2021-07-smog-tower-delhi-experts-sceptical.html)

Thủ đô New Delhi của Ấn Độ thường xuyên xếp hàng đầu thế giới về ô nhiễm không khí. Mới đây, ban quản lý khu mua sắm sầm uất tại trung tâm thành phố đã đầu tư 2 triệu USD để xây dựng một tháp lọc không khí cao 25 mét:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072210.jpg)

Hệ thống tích hợp 40 cánh quạt hút khổng lồ đặt trên đỉnh tháp hoạt động liên tục để hút và lọc bụi mịn trong không khí, hướng tới mục tiêu cung cấp vùng không khí sạch trong phạm vi bán kính 1 km2 cho khu thương mại xung quanh. Tuy nhiên nhiều chuyên gia môi trường hoài nghi về hiệu quả thực tế của phương án tốn kém này.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072211.jpg)

2、[Robot Toyota trình diễn ném bóng rổ chuẩn xác 100% tại Olympic](https://v.qq.com/x/page/w0039aev369.html)

Trong giờ nghỉ giữa hiệp của trận đấu bóng rổ nam giữa Mỹ và Pháp tại Olympic Tokyo, một chú robot của hãng Toyota đã ra sân trình diễn kỹ thuật ném bóng rổ ở khoảng cách xa với tỷ lệ trúng đích tuyệt đối:

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=w0039aev369" allowFullScreen="true" width="400" height="600"></iframe>

Chú robot cao 2,04m này được nhóm 17 kỹ sư của Toyota nghiên cứu chế tạo trong thời gian rảnh rỗi. Robot sử dụng hệ thống camera quét hồng ngoại xác định cự ly rổ và chạy thuật toán AI điều khiển lực nâng cánh tay cơ khí để ném bóng chuẩn xác ở mọi vị trí trên sân.

3、[Cảnh sát bắt giữ drone vận chuyển ma túy xuyên quốc gia](https://english.elpais.com/spain/2021-07-15/spanish-police-seize-large-drone-used-to-carry-drugs-from-morocco.html)

Cảnh sát Tây Ban Nha công bố thông tin triệt phá một đường dây vận chuyển chất cấm xuyên biên giới từ Maroc sử dụng thiết bị bay không người lái (drone) cỡ lớn:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072206.jpg)

Chiếc drone chạy động cơ xăng có sải cánh rộng tới 4,5 mét, đạt tốc độ bay 170 km/h và tải trọng hữu ích lên tới 150 kg hành lý. Tội phạm đã lập trình cho máy bay bay sát mặt đất để tránh hệ thống radar quét phòng không quốc gia, nhưng cảnh sát đã phát hiện ra đường bay nhờ định vị luồng sóng điều khiển vô tuyến bất thường.

4、[Game thủ rò rỉ bản vẽ xe tăng Challenger 2 lên diễn đàn game](https://ukdefencejournal.org.uk/classified-challenger-tank-specs-leaked-online-for-videogame/)

Một sự việc hy hữu xảy ra trên diễn đàn của tựa game bắn xe tăng trực tuyến *War Thunder*. Một game thủ tự xưng là lính xe tăng thuộc quân đội Anh đã đăng tải các tệp tin chứa bản vẽ thiết kế kỹ thuật chi tiết của dòng xe tăng Challenger 2 lên diễn đàn để chứng minh nhà phát triển game thiết kế sai thông số giáp của xe tăng trong game.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071702.jpg)

Do Challenger 2 vẫn là dòng xe tăng chiến đấu chủ lực đương nhiệm của quân đội Anh, toàn bộ bản vẽ kỹ thuật của xe đều thuộc danh mục bí mật quân sự. Ban quản trị diễn đàn đã lập tức xóa tệp tin và cảnh báo hành vi phát tán tài liệu mật này có thể đối mặt với mức án lên tới 14 năm tù giam theo Luật Bảo mật của Anh.

5、[Ford phát minh dòng nước hoa mùi xăng dầu dành cho chủ xe điện](https://electrek.co/2021/07/15/ford-petrol-scent-for-electric-cars-barrier-ev-adoption/)

Khảo sát khách hàng của Ford chỉ ra một thực tế thú vị: 20% tài xế khi chuyển sang sử dụng xe điện cho biết họ cảm thấy không quen khi khoang cabin thiếu đi mùi xăng dầu đặc trưng, và có tới 70% người dùng thừa nhận họ có phần nhớ mùi động cơ đốt trong truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071701.jpg)

Ford đã quyết định chế tạo dòng nước hoa cao cấp mang tên Mach-Eau mô phỏng mùi hương kết hợp giữa xăng dầu, khói xám nhẹ và mùi cao su lốp xe cháy để phun nhẹ trong cabin xe điện giúp tài xế tìm lại cảm giác lái xe quen thuộc.

6、[Thực trạng lạm dụng nước ngọt có ga thay nước uống tại bang nghèo Mexico](https://mexiconewsdaily.com/news/with-average-daily-consumption-of-2-2-liters-of-coca-cola-chiapas-leads-the-world/)

Bang Chiapas - bang nghèo nhất của Mexico được ghi nhận là khu vực có lượng tiêu thụ nước ngọt có ga (đặc biệt là Coca-Cola) cao nhất thế giới. Trung bình một người dân tại đây tiêu thụ tới 2,2 lít nước ngọt mỗi ngày (821 lít/năm):

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071601.jpg)

Nguyên nhân bắt nguồn từ việc hạ tầng công cộng tại địa phương rất kém, nguồn nước máy bị ô nhiễm nghiêm trọng không thể lọc sạch. Trong khi đó, Coca-Cola có nhà máy đóng chai lớn đặt ngay tại bang và bán nước ngọt với mức giá rẻ hơn cả nước lọc đóng chai thông thường. Nhiều gia đình nghèo dùng Coca-Cola làm nước uống chính hàng ngày cho cả trẻ sơ sinh, dẫn tới tỷ lệ tử vong do tiểu đường và tim mạch cực kỳ cao tại bang.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071602.jpg)

## 文章

1、[Dự án cải tạo và thiết kế nhà vệ sinh nông thôn mới](https://mp.weixin.qq.com/s/J0w7_rd40_L9hB6Z1yLmjw)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071907.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071908.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071909.jpg)

Bài viết chia sẻ nỗ lực của một nhóm kiến trúc sư trẻ nhằm thiết kế lại nhà vệ sinh gia đình tại các vùng nông thôn phía Bắc Trung Quốc, giải quyết các bài toán thiếu đường ống thoát nước công cộng, thu gom xử lý chất thải sinh học tự động và giữ nhiệt ấm cho phòng vệ sinh vào mùa đông lạnh giá.

2、[Nghiên cứu khoa học thể thao của vận động viên Tô Bính Thiêm](https://mp.weixin.qq.com/s/ddwBH9lMWDD6NHcAN1zVwA)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080214.jpg)

Tô Bính Thiêm (Su Bingtian) là vận động viên châu Á đầu tiên vượt qua giới hạn chạy 100m dưới 10 giây tại sân chơi Olympic. Bên cạnh tư cách vận động viên, anh còn là phó giáo sư giảng dạy tại Đại học Cự Nam. Bài viết giới thiệu các công trình nghiên cứu khoa học thể thao phân tích kỹ thuật sải bước và tần số guồng chân dựa trên dữ liệu chuyển động của chính anh.

3、[Thuật toán lập trình sinh ra các bảng câu đố Sudoku](https://me.guanghechen.com/post/game/sudoku/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080505.jpg)

Tác giả giới thiệu chi tiết tư duy lập trình và các bước xây dựng thuật toán quay lui (backtracking) để tự động tạo ra các bảng câu đố Sudoku hoàn chỉnh theo nhiều mức độ khó khác nhau. (Đóng góp của [@guanghechen](https://github.com/ruanyf/weekly/issues/1874))

4、[Kỹ thuật nén dung lượng Docker Image cho ứng dụng Node.js](https://juejin.cn/post/6991689670027542564)（Tiếng Trung）

Hướng dẫn từng bước tối ưu hóa cấu hình Dockerfile (sử dụng multi-stage build và alpine base image) để nén dung lượng Docker Image của dự án Node.js từ 1,06 GB xuống còn 73,4 MB, giúp tăng tốc độ build CI/CD của doanh nghiệp. (Đóng góp của [@iamobj](https://github.com/ruanyf/weekly/issues/1873))

5、[Thiết kế database cho mối quan hệ bạn bè hai chiều](https://minimalmodeling.substack.com/p/modeling-mutual-friendship)（Tiếng Anh）

Bài viết phân tích các mô hình thiết kế cơ sở dữ liệu quan hệ tối ưu để quản lý tính năng kết bạn hai chiều (mutual friendship) trong các ứng dụng mạng xã hội, đảm bảo tốc độ truy vấn danh sách bạn chung nhanh chóng.

6、[Thiết kế chế độ tối (dark mode) cho web bằng một dòng CSS](https://davidwalsh.name/dark-mode-invert-filter)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072111.jpg)

Tác giả chia sẻ mẹo nhỏ sử dụng bộ lọc CSS `filter: invert(1) hue-rotate(180deg);` khai báo trên thẻ `html` để đảo ngược màu sắc hiển thị của toàn bộ trang web tạo giao diện dark mode nhanh gọn.

7、[Googlebot có quét nội dung chữ được sinh ra từ CSS?](https://www.searchcandy.uk/seo/technical-seo/css-pseudo-elements/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071901.jpg)

Tác giả thực hiện một thử nghiệm thực tế để kiểm tra xem thuật toán lập chỉ mục SEO của Google có ghi nhận các đoạn text được sinh ra động từ thuộc tính CSS `:before` hoặc `:after` hay không, kết quả cho thấy Google hoàn toàn có thể đọc được luồng text này.

8、[Tại sao mắt người khó lấy nét chính xác đối với vật thể ánh sáng xanh?](https://calebkruse.com/10-projects/seeing-blue/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071703.jpg)

Bài viết phân tích cấu trúc cấu tạo sinh học võng mạc của mắt người giải thích nguyên nhân tại sao mắt người nhạy bén và lấy nét dễ dàng với ánh sáng đỏ, xanh lá hơn là ánh sáng xanh lam (do mật độ tế bào nón cảm nhận xanh lam ở trung tâm hố hoàng điểm rất thưa thớt).

## 工具

1、[Obsidian Mobile](https://obsidian.md/mobile)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071302.jpg)

Phiên bản di động của ứng dụng ghi chép Markdown Obsidian nổi tiếng, hỗ trợ đồng bộ hóa tệp tin markdown cục bộ và quản lý liên kết sơ đồ tri thức hai chiều cực kỳ mạnh mẽ.

2、[Fakeflix](https://github.com/Th3Wall/Fakeflix)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071401.jpg)

Dự án mã nguồn mở tái dựng lại giao diện trang web xem phim Netflix sử dụng React kết hợp Redux, là tài liệu thực hành frontend chất lượng.

3、[PhotoBook VR Album](https://awesomealbum.com/photobook)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072401.jpg)

Ứng dụng web sáng tạo cho phép người dùng upload ảnh chụp cá nhân để tự động dựng thành một cuốn album ảnh 3D xem trong không gian thực tế ảo VR trực quan.

4、[hookdeck](https://hookdeck.com/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080501.jpg)

Tiện ích đám mây hỗ trợ quản lý tập trung, theo dõi luồng request và hỗ trợ gửi lại (retry) các yêu cầu gọi Webhook của hệ thống dịch vụ để tránh mất dữ liệu.

5、[DataEase](https://github.com/dataease/dataease)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080504.jpg)

Công cụ phân tích và trực quan hóa dữ liệu (BI tool) nguồn mở giúp kết nối nhiều nguồn database để thiết kế các dashboard kéo thả trực quan. (Đóng góp của [@chixq](https://github.com/ruanyf/weekly/issues/1872))

6、[Mousai](https://github.com/SeaDve/Mousai)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080503.jpg)

Phần mềm máy tính nguồn mở hỗ trợ nhận diện tên ca khúc đang phát từ âm thanh thu được qua micro tương tự Shazam.

7、[html-to-image](https://github.com/bubkoo/html-to-image)

Thư viện JavaScript hỗ trợ chụp ảnh màn hình và xuất một phần tử DOM thành ảnh PNG/SVG tải về bằng cách render lại thông qua Canvas.

8、[mandodb](https://github.com/chenjiandongx/mandodb)

Dự án lập trình hướng dẫn tự xây dựng một cơ sở dữ liệu dạng chuỗi thời gian (Time Series Database - TSDB) tối giản bằng ngôn ngữ Go. (Đóng góp của [@chenjiandongx](https://github.com/ruanyf/weekly/issues/1876))

## Tài nguyên

1、[SVN Cheatsheet](https://spike-leung.github.io/blog/others/svn-cheatsheet.html)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080507.jpg)

Bảng tra cứu nhanh các dòng lệnh và cú pháp sử dụng hệ thống quản lý phiên bản Subversion (SVN) bằng tiếng Trung. (Đóng góp của [@Spike-Leung](https://github.com/ruanyf/weekly/issues/1875))

2、[Rust and WebAssembly Book](https://rustwasm.github.io/docs/book/introduction.html)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070301.jpg)

Giáo trình trực tuyến hướng dẫn lập trình viên sử dụng ngôn ngữ Rust để biên dịch ra mã WebAssembly tối ưu hiệu năng chạy trên web.

3、[Introduction to Information Retrieval (Môn học tìm kiếm thông tin)](https://nlp.stanford.edu/IR-book/)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071406.jpg)

Sách giáo khoa miễn phí của Đại học Stanford giảng dạy nguyên lý xây dựng công cụ tìm kiếm, thuật toán xếp hạng trang web và lập chỉ mục văn bản.

4、[XPRIZE Carbon Removal (Giải thưởng 100 triệu USD giảm carbon)](https://www.xprize.org/prizes/elonmusk)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071415.jpg)

Dự án thi đua đề xuất giải pháp thu hồi khí thải carbon toàn cầu do quỹ từ thiện của Elon Musk tài trợ giải thưởng trị giá 100 triệu USD.

5、[Public API Lists](https://github.com/public-api-lists/public-api-lists)

Repo GitHub tổng hợp hàng nghìn API dịch vụ miễn phí thuộc nhiều lĩnh vực dành cho lập trình viên phát triển dự án.

## 图片

1、[液晶广告门](https://twitter.com/RunDaltonRun/status/1408566439833788423)

Hãng công nghệ Cooler Screens của Mỹ giới thiệu thiết kế cửa tủ mát siêu thị thế hệ mới tích hợp màn hình LCD hiển thị quảng cáo động và thông tin sản phẩm:

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062602.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062603.jpg)

Thiết kế này giúp siêu thị tăng nguồn thu quảng cáo đồng thời hiển thị thông tin sản phẩm trực quan hơn, khách hàng chỉ cần mở cửa kính ra để lấy đồ bên trong tủ mát thực tế:

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=u3255jduawe" allowFullScreen="true" width="400" height="600"></iframe>

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062604.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062605.jpg)

2、[Nghệ thuật xếp đá cuội độc đáo của Justin Bateman](https://www.odditycentral.com/art/the-awe-inspiring-pebble-mosaics-of-justin-bateman.html)

Nghệ sĩ người Anh Justin Bateman chia sẻ các tác phẩm tranh chân dung siêu thực được anh sắp xếp tỉ mỉ hoàn toàn từ các viên đá cuội tự nhiên có nhiều màu sắc và kích thước khác nhau:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072808.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072809.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072810.jpg)

## Bài đọc thêm

### Tại sao các lập trình viên từ bỏ dự án mã nguồn mở cá nhân?

*Hầu hết các dự án open-source được khởi tạo bởi các cá nhân và chỉ một tỷ lệ rất nhỏ được duy trì lâu dài. Dưới đây là các nguyên nhân hàng đầu khiến tác giả từ bỏ dự án:*

1. **Thiếu động lực tài chính:** Dự án hoàn toàn miễn phí trong khi tác giả phải bỏ nhiều công sức duy trì.
2. **Khó khăn cập nhật công nghệ:** Việc nâng cấp code để tương thích với các thư viện nền tảng mới tốn quá nhiều thời gian.
3. **Mất đi sự hứng thú ban đầu:** Dự án ban đầu chỉ được viết cho vui hoặc phục vụ bài tập đại học.
4. **Mã nguồn phình to quá lớn:** Dự án vượt quá tầm kiểm soát và khả năng bảo trì của một cá nhân.
5. **Áp lực hỗ trợ người dùng:** Tác giả phải đối mặt với hàng chục yêu cầu hỗ trợ, sửa lỗi từ những người dùng phổ thông thiếu kiên nhẫn hàng ngày.
6. **Sự xuất hiện của giải pháp thay thế tốt hơn.**
7. **Bất đồng ý kiến** giữa các thành viên chủ chốt trong nhóm phát triển.
8. **Thay đổi ưu tiên cuộc sống** của tác giả (kết hôn, sinh con).
9. **Chất lượng mã nguồn ban đầu kém** gây khó khăn cho việc refactor.
10. **Tác giả bán lại dự án** cho đơn vị thương mại khác.

## 言论

1、

Huy chương bạc thực sự mang lại cảm giác khá khó chịu. Nếu bạn đạt huy chương vàng, bạn sẽ vô cùng tự hào; nếu đạt huy chương đồng, bạn sẽ an ủi mình ít nhất cũng có giải mang về. Nhưng khi nhận huy chương bạc, cảm giác giống như ai đó nói với bạn: *"Chúc mừng nhé, bạn suýt chút nữa thì thắng, và trong số những người thua cuộc, bạn là người đứng đầu"*.

-- Jerry Seinfeld

2、

Mục tiêu lớn nhất của chúng tôi là lưu trữ và bảo tồn mãi mãi các tác phẩm viết của 1 tỷ người trên Trái Đất.

-- Brewster Kahle, nhà sáng lập Internet Archive phát biểu nhân kỷ niệm 25 năm dự án

3、

Mọi người thường hỏi tôi về sự cân bằng giữa công việc và cuộc sống (work-life balance). Tôi cho rằng thuật ngữ này dễ khiến con người trở nên yếu đuối vì nó hàm ý bạn phải phân định rạch ròi giữa hai bên. Thực tế công việc và cuộc sống hòa quyện chặt chẽ với nhau, nếu một bên gặp bất ổn thì bên còn lại chắc chắn sẽ bị ảnh hưởng tiêu cực theo.

-- Jeff Bezos

4、

Mỗi dòng code viết thêm thực chất là một gánh nặng kỹ thuật. Khi bạn gia tăng số lượng dòng code của dự án, bạn đang trực tiếp gia tăng trách nhiệm bảo trì của mình trong tương lai.

-- Trích cẩm nang khởi nghiệp "Tech Startup Survival Guide"

## 历史上的本周

- 2020年（第 119 期）：[Phân tích mô hình toán học lượng mưa và trò chơi bảo hiểm nông nghiệp](https://www.ruanyifeng.com/blog/2020/08/weekly-issue-119.html)
- 2019年（第 67 期）：[Tại sao các hệ thống kỹ thuật quá phức tạp luôn có nguy cơ sụp đổ](https://www.ruanyifeng.com/blog/2019/08/weekly-issue-67.html)
- 2018年（第 16 期）：[Công nghệ hiện đại đang định hình lại các dịch vụ hậu sự ra sao](https://www.ruanyifeng.com/blog/2018/08/weekly-issue-16.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
