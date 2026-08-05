# 每周分享第 47 期 (Bản tin chia sẻ hàng tuần số 47)

Ghi lại những điều thú vị đáng chia sẻ tôi bắt gặp trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Chào mừng mọi người gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục [issue](https://github.com/ruanyf/weekly/issues) tại kho lưu trữ GitHub [ruanyf/weekly](https://github.com/ruanyf/weekly).

![](https://cdn.beekka.com/blogimg/asset/201903/bg2019031501.jpg)

Nếu bạn đọc bản tin này lâu dài, có thể biết quan điểm của tôi: AI sẽ dẫn đến thất nghiệp hàng loạt, vì thuật toán sẽ thay thế phần lớn [công việc cổ cồn trắng](http://www.ruanyifeng.com/blog/2016/01/white-collar.html).

Nhiều người không đồng ý, cho rằng tương lai sẽ có đủ việc làm mới để hấp thụ. Nhưng cụ thể những công việc đó là gì? Không ai trả lời được. Một điều hiển nhiên: những công việc đó không thể là lập trình viên hay chuyên gia thuật toán - vì đại đa số người không đáp ứng được yêu cầu, cũng giống như không thể bắt tất cả mọi người học thành thạo Giải tích.

Gần đây tôi đọc cuốn *WTF? What's the Future and Why It's Up to Us* của Tim O'Reilly - ông cũng đồng ý AI sẽ khiến nhiều người mất việc, nhưng nói không lo vì mọi người sẽ tìm việc khác. Ông ví dụ: tương lai mọi người quay video cho nhau xem - vô số người trở thành "YouTuber", "streamer", kiếm sống bằng việc quay video. Điều đó nghe có vẻ hợp lý - hiện nay đã có nhiều người livestream ăn uống kiếm tiền từ tip/donation. Tiếng Anh có từ riêng [Mukbang](https://en.wikipedia.org/wiki/Mukbang) (音译từ tiếng Hàn) để chỉ loại livestream này.

![](https://cdn.beekka.com/blogimg/asset/201903/bg2019031502.jpg)

Nhưng tôi vẫn hoài nghi: nếu công việc tương lai là quay những video như vậy, thì có ý nghĩa gì không? [Kaczynski](http://www.ruanyifeng.com/blog/2017/09/unabomber.html) từng mô tả tình huống này: khi năng suất sản xuất phát triển vượt bậc, con người không còn việc gì làm, chỉ có thể "dùng thời gian đánh giày cho nhau, chở nhau đi khắp nơi bằng xe taxi, làm đồ thủ công cho nhau, bưng bê đồ ăn cho nhau." Thành thật mà nói, tôi không thấy sự khác biệt về bản chất giữa mọi người quay video cho nhau xem với đánh giày cho nhau.

## 新闻 (Tin tức)

1、[Airbus A380 ngừng sản xuất năm 2021 - Máy bay lớn nhất thế giới thất bại thương mại](https://www.cnn.com/2019/02/14/business/a380-airbus-news-emirates/index.html)

![](https://cdn.beekka.com/blogimg/asset/201903/bg2019031503.jpg)

Airbus thông báo sẽ ngừng sản xuất A380 vào năm 2021. A380 là máy bay thương mại lớn nhất thế giới, chở tối đa 853 hành khách, bay lần đầu năm 2005. Airbus dự báo sẽ bán được 1.200 chiếc nhưng thực tế chỉ bán được 234 - vì các hãng hàng không chuyển sang ưa chuộng máy bay nhẹ hơn, tiết kiệm nhiên liệu hơn.

2、[JPMorgan Chase ra mắt đồng tiền kỹ thuật số JPM Coin cho thanh toán doanh nghiệp](https://decryptmedia.com/5173/jp-morgan-coin-cryptocurrency)

Ngân hàng đầu tư JPMorgan Chase ra mắt đồng kỹ thuật số "JPM Coin" được bảo đảm 1:1 bằng USD. Đây không phải tiền tệ công khai - chỉ dành cho các doanh nghiệp lớn, thanh toán trên blockchain Quorum do JPMorgan tự phát triển. Lợi ích chính: cho phép chuyển tiền gần như tức thì, thay vì 3-5 ngày làm việc như chuyển khoản truyền thống.

3、[Quân đội Đức trong tình trạng tồi tệ: Tiêm kích không bay được, tàu ngầm không chạy được](https://www.politico.eu/article/germany-biggest-enemy-threadbare-army-bundeswehr/)

![](https://cdn.beekka.com/blogimg/asset/201903/bg2019031505.jpg)

Quân đội Đức từng là một trong những lực lượng thiện chiến nhất thế giới. Sau WWII, Đồng minh giải giáp Đức và chỉ cho phép giữ lực lượng phòng thủ. Báo chí Đức gần đây tiết lộ: thiếu người, thiếu thiết bị, tiêm kích hầu hết không thể bay, tàu ngầm không thể ra khơi. Trong 68 trực thăng và 136 máy bay chiến đấu, chỉ dưới 30% sẵn sàng hoạt động. Tháng trước, quân đội phải đi xúc tuyết trên mái nhà ở Bavaria. Trong một nhiệm vụ NATO, 450 binh sĩ Đức phải dùng điện thoại dân sự liên lạc vì thiếu thiết bị vô tuyến.

4、[Firefox Send ra mắt - Chia sẻ file mã hóa đầu cuối, tự hủy sau 7 ngày](https://blog.mozilla.org/blog/2019/03/12/introducing-firefox-send-providing-free-file-transfers-while-keeping-your-personal-information-private/)

Mozilla ra mắt Firefox Send - dịch vụ chia sẻ file mã hóa đầu cuối miễn phí, file tự hủy sau tối đa 7 ngày hoặc sau một số lần tải xuống định trước. Không cần tài khoản, bảo mật hơn email.

5、[Tòa nhà gỗ 18 tầng cao 80m - Tòa nhà gỗ cao nhất thế giới hoàn thành tại Na Uy](http://news.cision.com/metsa-wood/r/metsa-wood--at-18-storeys--mjosa-tower-in-brumunddal-to-take-title-of-world-s-tallest-wooden-buildin,c2325089)

![](https://cdn.beekka.com/blogimg/asset/201903/bg2019031511.jpg)

Tháng 3/2019, tòa nhà Mjøstårnet 18 tầng, cao hơn 80m hoàn thành tại Brumunddal (Na Uy), trở thành tòa nhà gỗ cao nhất thế giới. Tòa nhà dùng ván ép (CLT - Cross-Laminated Timber) với kỹ thuật đặc biệt đảm bảo khả năng chịu lực. So với bê tông đổ tại chỗ, gỗ rút ngắn thời gian thi công một nửa và nhẹ hơn nhiều, giảm yêu cầu về móng.

6、[Robot chép chữ theo nét tay - Học sinh lớp 9 Trung Quốc bị mẹ phát hiện](https://www.thepaper.cn/newsDetail_forward_2998361)

![](https://cdn.beekka.com/blogimg/asset/201903/bg2019031509.jpg)

Theo báo Tiền Giang, một học sinh lớp 9 ở Cáp Nhĩ Tân đặt mua "robot chép chữ" trên mạng - thiết bị có thể nhận dạng chữ viết tay của chủ nhân rồi tự động chép bài tập với tốc độ ~40 chữ/phút. Bà mẹ phát hiện ra, đập vỡ thiết bị và mắng con. Robot thực ra là bộ thanh kim loại điện tử có thể lắp ráp đơn giản.

## 文章 (Bài viết)

1、[Bài viết] [Bạn có thực sự cần Single Page Application không?](https://journal.plausible.io/you-probably-dont-need-a-single-page-app) (Tiếng Anh)

Tác giả lập luận xu hướng làm tất cả mọi thứ thành SPA đang bị lạm dụng. Hầu hết các trường hợp nên dùng web truyền thống; chỉ nên dùng SPA khi thực sự cần real-time, rich interaction hoặc chia sẻ trạng thái phức tạp.

2、[Bài viết] [Lịch sử AltaVista - Công cụ tìm kiếm lớn nhất trước khi Google xuất hiện](https://digital.com/about/altavista/) (Tiếng Anh)

AltaVista từng là công cụ tìm kiếm thống trị internet trước Google. Bài viết kể lại lịch sử ra đời, thống trị và sụp đổ của AltaVista - bài học về cách mất thị phần vào tay đối thủ được thiết kế đơn giản hơn.

3、[Bài viết] [Windows 10 phiên bản 1903 cho phép Windows Explorer truy cập file Linux trong WSL](https://blogs.msdn.microsoft.com/commandline/2019/02/15/whats-new-for-wsl-in-windows-10-version-1903/) (Tiếng Anh)

Bản cập nhật Windows 10 mùa xuân 2019 cho phép File Explorer của Windows trực tiếp truy cập và chỉnh sửa file trong WSL (Windows Subsystem for Linux) - không còn cần phải thao tác trong terminal.

4、[Bài viết] [Làm thế nào để biết vị trí thời gian thực của tất cả chuyến bay trên thế giới?](https://habr.com/en/post/440596/) (Tiếng Anh)

Mỗi máy bay dân dụng đều trang bị thiết bị ADS-B phát tín hiệu vô tuyến 1090MHz không mã hóa, chứa vị trí GPS, tốc độ, độ cao và ID máy bay. Bất kỳ ai có thiết bị nhận sóng đơn giản cũng có thể thu được dữ liệu này.

5、[Bài viết] [Tự học Khoa học Máy tính - Danh sách sách và lộ trình toàn diện](https://teachyourselfcs.com/#programming) (Tiếng Anh)

Lộ trình và danh sách sách kinh điển để tự học đầy đủ các môn CS cơ bản: lập trình, thuật toán, kiến trúc máy tính, hệ điều hành, mạng, cơ sở dữ liệu, ngôn ngữ lập trình và toán học. Có [bản dịch tiếng Trung](http://blog.jobbole.com/114573/).

## 工具 (Công cụ)

1、[Mermaid Live Editor — Vẽ biểu đồ flowchart, sequence diagram... bằng text, xem preview trực tiếp](https://mermaidjs.github.io/mermaid-live-editor/)

![](https://cdn.beekka.com/blogimg/asset/201903/bg2019031516.jpg)

Công cụ online soạn và xem trước biểu đồ Mermaid theo thời gian thực. Mermaid cho phép tạo flowchart, sequence diagram, Gantt chart, class diagram... chỉ bằng text syntax đơn giản.

2、[gita — Quản lý nhiều git repository cùng lúc bằng một lệnh](https://github.com/nosarthur/gita)

Công cụ cho phép chạy git command trên nhiều repo cùng lúc (git pull, git status...), hiển thị tổng quan trạng thái của tất cả repo trong một màn hình, rất hữu ích khi làm việc với monorepo hoặc nhiều dự án liên quan.

3、[FlightGear — Phần mềm giả lập bay mã nguồn mở, miễn phí, đa nền tảng](https://opensource.com/article/19/1/flightgear)

![](https://cdn.beekka.com/blogimg/asset/201903/bg2019031517.jpg)

Giả lập bay mã nguồn mở chạy trên Linux, macOS và Windows. Hỗ trợ hàng trăm loại máy bay, hàng nghìn sân bay và điều kiện thời tiết thực tế. Thay thế miễn phí cho Microsoft Flight Simulator.

4、[Mozilla Send — Chia sẻ file mã hóa đầu cuối, tự hủy sau 7 ngày - Mã nguồn mở](https://github.com/mozilla/send)

Mã nguồn mở của dịch vụ Firefox Send, có thể tự host. File được mã hóa trước khi upload, server không có khả năng đọc nội dung. Link tự hủy sau thời gian hoặc số lần tải được cấu hình trước.

## 资源 (Tài nguyên)

1、[Sách] [Go by Example — Học lập trình Go qua ví dụ thực tế, từng bước](https://gobyexample.com/)

Hướng dẫn Go thực hành với các ví dụ chạy được theo từng tính năng: hello world, goroutines, channels, interfaces, error handling... Mỗi ví dụ đi kèm giải thích ngắn gọn.

2、[Sách] [sicp-py-zh — Bản dịch tiếng Trung của SICP phiên bản Python từ UC Berkeley](https://github.com/wizardforcel/sicp-py-zh)

Bản dịch tiếng Trung của *Composing Programs* - phiên bản SICP dùng Python 3 của UC Berkeley. Dạy tư duy lập trình hệ thống: abstraction, recursion, data structures, OOP.

3、[Trang web] [GitNews — Tổng hợp repo GitHub đang trending từ HackerNews và Reddit theo thời gian thực](https://git.news/)

Công cụ tổng hợp các kho lưu trữ GitHub được nhắc đến nhiều nhất trên Hacker News và Reddit, hiển thị theo thời gian thực với filter theo ngôn ngữ lập trình.

## 文摘 (Văn trích)

1. **Tháp bồ câu Ba Tư - Nhà máy phân bón tự nhiên 1000 năm tuổi**

Nông nghiệp cần đạm (nitơ) và lân (phospho). Người cổ đại giải quyết bằng hai cách: luân canh cây trồng, hoặc dùng phân chim. Ba Tư cổ đại (Iran ngày nay) có giải pháp thanh lịch: xây tháp cho hàng nghìn con bồ câu hoang dã sống giữa đồng ruộng. Phân bồ câu tích lũy dưới đáy tháp, chủ tháp thu gom mỗi năm một lần bán cho nông dân.

![](https://cdn.beekka.com/blogimg/asset/201903/bg2019031530.jpg)

Thiết kế cơ bản rất đơn giản: hình nón, xây bằng gạch bùn, chứa tới 10.000 con bồ câu. Đỉnh tháp có lỗ cho bồ câu ra vào tự do, được thiết kế để rắn không chui vào được. Bồ câu khác gà hay vịt ở chỗ gần như không cần chăm sóc - chỉ cần cung cấp nước và nơi ở, chúng tự đến. Công nghệ cực kỳ thấp: chỉ cần gạch và xẻng để thu phân, vài trăm năm mới cần bảo trì một lần.

2. **Tập gym thôi chưa đủ - Cần vận động liên tục trong ngày, không phải vận động cường độ cao ngắt quãng**

Con người đang ngồi ngày càng nhiều. Hàng trăm nghìn năm trước, người nguyên thủy vận động liên tục để kiếm ăn, săn bắt, xây nhà. Một thế kỷ trước, mua sắm, lau nhà, giặt tay vẫn đòi hỏi vận động. Ngày nay, robot hút bụi, máy rửa bát, mua sắm online, điều khiển giọng nói khiến chúng ta hầu như không cần cử động. Điều tra Mỹ ước tính 86% lao động ngồi làm việc.

Vấn đề: dù bạn đi gym mỗi ngày, nhưng nếu thời gian còn lại vẫn ngồi thì vẫn có hại. Cơ thể cần **vận động liên tục, cường độ thấp đến trung bình suốt ngày** - không phải bùng phát ngắn dù cường độ cao. Những vùng có người sống thọ nhất thế giới không ai đi gym - họ đi bộ nhiều dặm mỗi ngày như một phần của cuộc sống.

Đứng làm việc tốt hơn ngồi một chút, nhưng không nhiều. Thực ra, một chiếc ghế hơi khó chịu có thể hiệu quả hơn - khiến bạn khó ngồi yên quá lâu.

## 本周图片 (Hình ảnh tuần này)

1. **Hạng nhất Singapore Airlines A380 - Vé 18.400 USD với phòng riêng và giường đôi trên máy bay**

![](https://cdn.beekka.com/blogimg/asset/201903/bg2019031520.jpg)

Vé hạng nhất Singapore-New York trên A380 là một trong những vé máy bay đắt nhất thế giới (~18.400 USD). Không chỉ có giường nằm phẳng mà còn là cabin riêng có cửa trượt. Điều đặc biệt nhất: hai cabin kề nhau có thể gộp lại tạo thành giường đôi - Singapore Airlines là hãng hàng không thương mại duy nhất có giường đôi.

2. **Bánh xe sách thế kỷ 17 - "Tablet" đa cửa sổ của thời trung cổ**

![](https://cdn.beekka.com/blogimg/asset/201903/bg2019031528.jpg)

Thời trung cổ, sách châu Âu làm từ da cừu nên rất nặng. Một người thợ sáng tạo ra "bánh xe sách" (bookwheel): máy gỗ hình bánh xe có thể xếp nhiều cuốn sách, muốn đổi sách chỉ cần quay tay cầm. Toàn thế giới hiện còn 14 chiếc. Chiếc trong ảnh được làm năm 1625 tại Đức.

## 本周金句 (Kim ngôn tuần này)

1、

> "Nếu bạn không hoàn thành dự án, dù bận đến đâu cũng không thể che giấu sự thiếu hiệu quả."
>
> -- Jack Bruce Simpson

2、

> "Chỉ có một trường hợp blockchain là giải pháp tốt và duy nhất: khi các bên giao dịch không tin tưởng nhau và không thể dùng hợp đồng hay hệ thống pháp luật. Nói cách khác, là những việc bất hợp pháp. Các trường hợp khác, cơ sở dữ liệu và hợp đồng giữa các bên là giải pháp tốt hơn."
>
> -- [*Các use case phổ biến của blockchain và tại sao chúng không hiệu quả*](https://news.ycombinator.com/item?id=19225857)

3、

> "Tự động hóa và dịch vụ đám mây đã thay đổi backend development: RDS khiến DBA gần như thừa, ảo hóa thay thế server admin, TDD và CI/CD thay thế QA. Các công ty lớn dùng cloud đang chuyển đổi backend engineer thành cloud architect hoặc kỹ sư mở rộng dịch vụ."
>
> -- James Beswick

(Hết)
