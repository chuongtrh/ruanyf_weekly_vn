# 科技爱好者周刊：第 92 期 (Bản tin chia sẻ công nghệ số 92)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

Mục tuyển dụng [《Ai đang tuyển dụng?》](https://github.com/ruanyf/weekly/issues/983) cung cấp nhiều thông tin việc làm hữu ích, hoan nghênh ghé thăm hoặc đăng tải thông tin tuyển dụng/thực tập.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121006.jpg)

Ảnh bìa: Vệ tinh Enceladus (Thổ Vệ Hai) của Sao Thổ, bề mặt được bao phủ bởi một lớp băng dày và các nhà khoa học đã xác nhận sự tồn tại của một đại dương nước lỏng khổng lồ nằm sâu dưới lớp băng này.

## 刊首语 (Lời tựa)

Gần đây, tôi có một giả thuyết thú vị.

Chúng ta đều biết mắt người có hiện tượng ["lưu ảnh" (visual persistence)](https://baike.baidu.com/item/%E8%A7%86%E8%A7%89%E6%9A%82%E7%95%99): sau khi hình ảnh biến mất, võng mạc vẫn lưu lại tín hiệu hình ảnh trong khoảng từ 100 đến 400 mili giây. Đây chính là nguyên lý vận hành của phim ảnh điện ảnh, chỉ cần phát liên tục 24 khung hình mỗi giây là mắt người sẽ tự động cảm nhận hình ảnh chuyển động mượt mà.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020012902.jpg)

Vậy tôi tự hỏi: liệu có tồn tại hiện tượng "lưu âm" (auditory persistence) tương tự hay không? Âm thanh chúng ta nghe được là liên tục, nhưng liệu có phải thực chất nó cũng được ghép nối từ các lát cắt âm thanh rời rạc hay không?

Tìm hiểu kỹ tài liệu y khoa, hiện tượng này hoàn toàn tồn tại và được gọi là ["Hiệu ứng Haas" (Haas Effect)](https://baike.baidu.com/item/%E5%93%88%E6%96%AF%E6%95%88%E5%BA%94). Nếu hai âm thanh tương tự nhau phát ra cách nhau từ 5 đến 35 mili giây, hệ thần kinh thính giác của người sẽ tự động gộp chúng lại và cảm nhận như là một âm thanh duy nhất.

So với thời gian lưu ảnh của thị giác (tối thiểu 100 mili giây), thời gian lưu âm của thính giác ngắn hơn rất nhiều (tối thiểu chỉ 5 mili giây, chênh lệch tới 20 lần).

Tôi giả thuyết rằng điều này có liên quan trực tiếp đến tốc độ truyền tải thông tin của hệ thần kinh con người. Lượng thông tin của dữ liệu hình ảnh (video) lớn hơn rất nhiều so với dữ liệu âm thanh (audio). Nếu tốc độ truyền dẫn tín hiệu của hệ thần kinh là không đổi, việc truyền tải dữ liệu hình ảnh sẽ tiêu tốn nhiều thời gian hơn. Để đảm bảo não bộ thu nhận đầy đủ thông tin hình ảnh, võng mạc bắt buộc phải duy trì thời gian lưu ảnh dài hơn.

Một thực tế kỹ thuật tương tự hỗ trợ cho giả thuyết này: một tệp tin nhạc MP3 dài 4 phút (tần số lấy mẫu 44.1kHz) có dung lượng khoảng 4MB, trong khi một tệp tin video độ phân giải 1080P dài 4 phút (mã hóa H.264) có dung lượng khoảng 80MB, mức chênh lệch cũng xấp xỉ đúng 20 lần.

## 资讯 (Tin tức)

1. **Nguy cơ bùng phát trở lại dịch bệnh bại liệt do biến thể virus từ vắc-xin**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019123112.jpg)

Vào năm 1988, Tổ chức Y tế Thế giới (WHO) đã khởi động chiến dịch quy mô lớn chưa từng có nhằm xóa sổ hoàn toàn bệnh bại liệt (polio) trên toàn cầu. Trải qua hơn 30 năm nỗ lực kiên trì, đến năm 2016 toàn thế giới chỉ còn ghi nhận ca bệnh bại liệt tại 3 quốc gia: Nigeria, Afghanistan và Pakistan.

Tuy nhiên, số liệu năm 2019 đang gióng lên hồi chuông cảnh báo lớn. Riêng tại Afghanistan và Pakistan đã ghi nhận 116 ca bệnh bại liệt mới, tăng gấp 4 lần so với năm 2018. Nghiêm trọng hơn, tại 12 quốc gia Châu Phi ghi nhận tới 196 ca bệnh bại liệt bùng phát không phải do virus bại liệt hoang dã tự nhiên gây ra, mà bắt nguồn từ biến thể đột biến của chính virus sống giảm độc lực có trong vắc-xin uống (OPV). Biến thể này đã khôi phục lại độc lực và khả năng lây truyền trong cộng đồng.

Thực tế này buộc WHO phải nhanh chóng triển khai các chiến dịch uống bổ sung dòng vắc-xin bại liệt mới cho hàng triệu trẻ em tại các khu vực này để ngăn chặn nguy cơ bùng phát đại dịch bại liệt diện rộng làm đổ sông đổ bể thành quả chống bại liệt suốt 30 năm qua.

2. **Nike công bố ngừng bán hàng trực tiếp trên sàn thương mại điện tử Amazon**

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020010215.jpg)

Vào tháng 11/2019, tập đoàn sản xuất đồ thể thao hàng đầu thế giới Nike chính thức thông báo rút toàn bộ các dòng sản phẩm của hãng ra khỏi hệ thống bán lẻ trực tuyến của Amazon để tập trung tối đa nguồn lực phát triển kênh bán hàng trực tiếp chính hãng (D2C) qua ứng dụng di động và website chính thức của mình. Đây là thương hiệu bán lẻ lớn nhất tính đến nay quyết định rời bỏ Amazon để tự chủ hoạt động kinh doanh trực tuyến, tiếp bước các thương hiệu xa xỉ như Rolex hay Louis Vuitton.

Sự phát triển mạnh mẽ của hệ thống dịch vụ SaaS hỗ trợ thương mại điện tử đang giúp các doanh nghiệp dễ dàng tự vận hành website bán hàng riêng biệt thay vì phụ thuộc vào các chợ điện tử lớn. Tại Mỹ, doanh nghiệp có thể sử dụng Shopify để dựng website, tiếp cận khách hàng qua mạng xã hội, xử lý thanh toán qua Stripe, quản lý kho bãi vận chuyển qua ShipBob, quản lý trả hàng qua Returnly và giao hàng nhanh trong ngày qua dịch vụ DarkStore. Chi phí vận hành các dịch vụ này chỉ tiêu tốn vài trăm USD mỗi tháng nhưng mang lại chất lượng dịch vụ chuyên nghiệp tương đương với Amazon.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020010216.jpg)

3. **Dân số Trung Quốc chính thức vượt ngưỡng 1.4 tỷ người**

Ngày 17/1/2020, Cục Thống kê Quốc gia Trung Quốc công bố số liệu thống kê dân số chính thức: tính đến cuối năm 2019, tổng dân số đại lục Trung Quốc đã vượt ngưỡng 1.4 tỷ người (đạt 1.400.050.000 người), tăng 4.67 triệu người so với năm trước. Trong đó, dân số khu vực nông thôn đạt 550 triệu người và dân số thành thị đạt 848 triệu người.

Để dễ hình dung về quy mô dân số khổng lồ này: tổng dân số của toàn bộ 28 quốc gia liên minh Châu Âu là 512 triệu người, khu vực Bắc Mỹ (Mỹ và Canada) là 364 triệu người, Nhật Bản là 127 triệu người, Úc và New Zealand là 30 triệu người. Tổng dân số của toàn bộ các quốc gia phát triển kể trên cộng lại chỉ đạt 1.033 tỷ người. Ngay cả khi cộng thêm toàn bộ 90 triệu dân số của 4 con rồng châu Á, tổng dân số giới phát triển toàn cầu vẫn ít hơn dân số Trung Quốc khoảng 200 triệu người.

Mức GDP bình quân đầu người của Trung Quốc trong năm 2019 cũng lần đầu tiên chạm mốc 10.000 USD, xếp ở vị trí khoảng thứ 67 thế giới, tương đương với mức của Mexico và Nga.

4. **S-Pod - Ý tưởng xe điện tự cân bằng dạng ghế ngồi di động độc đáo của Segway**

Hãng sản xuất xe điện tự cân bằng Segway giới thiệu dự án xe điện tự cân bằng dạng ghế ngồi S-Pod. Ghế ngồi được thiết kế di chuyển trên hai bánh lớn sử dụng công nghệ tự động cân bằng con quay hồi chuyển, người dùng ngồi thoải mái điều khiển hướng di chuyển thông qua cần gạt cần joystick bên hông với tốc độ tối đa đạt 40 km/h.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020010401.jpg)

Thiết kế của S-Pod được lấy cảm hứng từ các quả cầu ngắm cảnh trong phim điện ảnh *Jurassic World* và các ghế bay tương lai trong phim hoạt hình *WALL-E*. Thiết bị hiện chỉ hướng tới việc ứng dụng di chuyển trong các không gian đô thị khép kín như sân bay, khu vui chơi chủ đề, trung tâm mua sắm lớn thay vì lưu thông trên đường phố công cộng.

5. **Phát hiện hóa thạch xương hàm của người Denisovan niên đại 160.000 năm tại Cam Túc**

Tạp chí khoa học *Archaeology* bình chọn công trình nghiên cứu hóa thạch người Denisovan của Đại học Lan Châu (Trung Quốc) nằm trong top 5 phát hiện khảo cổ học nổi bật toàn cầu của năm 2019.

Hóa thạch xương hàm dưới của một loài người cổ đại được một nhà sư phát hiện từ năm 1980 bên trong hang động Karst Baishiya tại huyện Hạ Hà, tỉnh Cam Túc. Hóa thạch sau đó được bàn giao cho đại học Lan Châu và bắt đầu nghiên cứu chi tiết từ năm 2010.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020010404.jpg)

Kết quả phân tích protein và đo đạc đồng vị phóng xạ xác định mẫu hóa thạch có tuổi thọ lên tới 160.000 năm và thuộc về loài người Denisovan. Đây là lần đầu tiên phát hiện được hóa thạch của loài người cổ này ở ngoài khu vực hang động Denisova vùng núi Altai (Siberia), đồng thời là dấu vết cư trú cổ xưa nhất của người cổ đại được ghi nhận trên cao nguyên Tây Tạng, chứng minh người Denisovan đã thích nghi với môi trường sống lạnh giá và khắc nghiệt nơi đây từ hàng vạn năm trước.

6. **Tin vắn**

- Mạng xã hội Facebook tuyển dụng đội ngũ cộng tác viên cộng đồng để hỗ trợ xác thực thông tin, lọc bỏ các nội dung tin giả dựa trên danh sách các bài viết bị người dùng báo cáo nghi vấn.

- Báo cáo kinh tế Mỹ chỉ ra giá xe ô tô cũ trung bình tại nước này đã tăng trưởng tới 75% trong vòng 10 năm qua (đạt mức bình quân 8.657 USD/xe), trong khi giá xe mới chỉ tăng 25% làm gia tăng áp lực chi phí đi lại của người nghèo.

- Chính phủ Trung Quốc công bố lộ trình siết chặt quy định cấm sử dụng nhựa: bắt đầu từ cuối năm 2020 sẽ nghiêm cấm sản xuất và lưu hành các loại túi nilon siêu mỏng, màng phủ nông nghiệp PE siêu mỏng, hộp xốp dùng một lần và tăm bông nhựa trên phạm vi toàn quốc.

## 文章 (Bài viết)

1、[Bài viết] [Ứng dụng toán học giải cứu tên miền bị thu hồi trái phép của lập trình viên](https://susam.in/blog/sinkholed/) (Tiếng Anh)

Nhật ký ghi lại quá trình đấu tranh đòi lại quyền sở hữu tên miền cá nhân bị nhà đăng ký thu hồi sai sót kỹ thuật của tác giả bằng các lập luận pháp lý, liên tục gửi các khiếu nại kỹ thuật hệ thống tới cơ quan quản lý ICANN để buộc nhà đăng ký phải trả lại tên miền.

2、[Bài viết] [Tìm hiểu về chuyến hải trình Kon-Tiki huyền thoại vượt Thái Dương bằng bè gỗ năm 1947](https://www.lifeinnorway.net/kon-tiki-voyage/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122116.jpg)

Nhằm chứng minh giả thuyết người da đỏ Nam Mỹ cổ đại hoàn toàn có khả năng di cư sang các hòn đảo Polynesia thuộc Nam Thái Bình Dương bằng bè gỗ thô sơ, nhà thám hiểm người Na Uy Thor Heyerdahl cùng 5 đồng sự đã đóng chiếc bè gỗ mang tên Kon-Tiki và thực hiện hành trình trôi tự do theo hải lưu suốt 97 ngày từ Peru tới đảo Raroia vào năm 1947.

3、[Bài viết] [Tại sao tôi quyết định rời bỏ công việc lập trình viên tại tập đoàn Google?](https://mtlynch.io/why-i-quit-google/) (Tiếng Anh)

Cựu kỹ sư Google chia sẻ câu chuyện chân thực về môi trường làm việc bên trong tập đoàn: quy trình xét duyệt thăng tiến (promotion) quá chú trọng vào các chỉ số đóng góp tính năng hiển thị trực quan thay vì nỗ lực dọn rác code hay bảo trì hệ thống ngầm, dẫn tới việc các kỹ sư buộc phải chạy theo các dự án bóng bẩy bề nổi để được thăng chức.

## 软件 (Phần mềm)

1、[Hammerspoon — Công cụ tự động hóa hệ điều hành macOS bằng lập trình ngôn ngữ Lua](https://www.hammerspoon.org/)

Tiện ích mạnh mẽ hỗ trợ các kỹ sư tự động hóa mọi tác vụ trên máy Mac (như quản lý vị trí các cửa sổ ứng dụng, phím tắt hệ thống, tương tác với các cổng kết nối phần cứng) thông qua các đoạn mã viết bằng ngôn ngữ Lua gọn nhẹ.

2、[playwright — Thư viện tự động hóa trình duyệt web đa nền tảng của Microsoft](https://github.com/microsoft/playwright)

Được phát triển bởi đội ngũ kỹ sư đứng sau Puppeteer, Playwright hỗ trợ các lập trình viên dễ dàng viết kịch bản kiểm thử tự động (e2e testing) chạy đồng thời trên các nhân trình duyệt phổ biến Chromium (Chrome/Edge), WebKit (Safari) và Gecko (Firefox) chỉ với một cổng API duy nhất.

## 资源 (Tài nguyên)

1、[Trang web] [unDraw - Kho thư viện hình ảnh minh họa vector (SVG) bản quyền mở miễn phí](https://undraw.co/illustrations)

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122301.jpg)

Cung cấp hàng nghìn bức hình vẽ minh họa phẳng (flat illustrations) chất lượng cao thuộc nhiều chủ đề công nghệ, đời sống cho phép người dùng tùy chọn màu sắc thương hiệu và tải về định dạng SVG/PNG để sử dụng cho các dự án thương mại hoàn toàn miễn phí.

## 图片 (Hình ảnh)

1. **Quy trình tái chế biến đổi rác thải sinh hoạt thành hạt nhựa nguyên liệu tại Israel**

Hình ảnh ghi lại các công đoạn công nghệ của một nhà máy xử lý rác tại Israel cho phép thu gom rác thải hỗn hợp (thức ăn thừa, túi nilon, chai lọ nhựa) để sấy khô, xay mịn thành bột hữu cơ tổng hợp và nén ép nhiệt tạo thành hạt nhựa tái chế cung cấp cho các xưởng đúc đồ dùng gia dụng.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112109.jpg)

## 文摘 (Văn trích)

1. **So sánh cơ chế hoạt động của mô hình dự báo thời tiết GFS của Mỹ và ECMWF của Châu Âu**

Hoạt động dự báo thời diện rộng hiện nay phụ thuộc lớn vào các mô hình khí tượng toán học. Nhờ sự gia tăng sức mạnh của hệ thống siêu máy tính, độ chính xác của dự báo thời tiết liên tục được cải thiện (dự báo 5 ngày hiện nay có độ chính xác tương đương dự báo 3 ngày của thập niên 1990).

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112301.jpg)

Hiện tại, hai mô hình dự báo thời tiết toàn cầu phổ biến và có sức ảnh hưởng nhất thế giới là mô hình GFS của Mỹ và mô hình ECMWF của Châu Âu:

Mô hình GFS (Global Forecast System) được vận hành bởi Cơ quan Thời tiết Quốc gia Mỹ, thực hiện tính toán 4 lần mỗi ngày để đưa ra dự báo thời tiết trong vòng 16 ngày tới. Hệ thống siêu máy tính chạy mô hình GFS có khả năng xử lý tới 10^15 phép tính mỗi giây, nằm trong danh sách các siêu máy tính nhanh nhất thế giới.

Mô hình ECMWF (European Centre for Medium-Range Weather Forecasts) được hợp tác xây dựng bởi 34 quốc gia Châu Âu. Nhờ việc đầu tư thuật toán mô phỏng chuyển động khí quyển chi tiết và hệ thống siêu máy tính cấu hình mạnh hơn, mô hình ECMWF thường được giới chuyên môn đánh giá có độ tin cậy dự báo cao hơn mô hình GFS của Mỹ (tiêu biểu là việc dự báo chính xác quỹ đạo di chuyển của siêu bão Sandy năm 2012 trước nhiều ngày). Mô hình chỉ tập trung đưa ra dự báo trong cự ly 10 ngày - vốn được coi là giới hạn vật lý tối đa cho một dự báo thời tiết có độ tin cậy cao.

## 言论 (Danh ngôn)

1、

> "Ước mơ lớn nhất đời tôi là sở hữu đủ tiềm lực tài chính để sinh sống tại những đô thị hàng đầu thế giới, trong khi vẫn giữ được quyền kiểm soát tuyệt đối quỹ thời gian cá nhân của mình để làm những việc mình yêu thích."
> 
> -- Trích chia sẻ của một lập trình viên tự khởi nghiệp SaaS thành công

(Hết)
