# Bản tin chia sẻ công nghệ (Số 290): Vấn đề lớn nhất của kính thực tế ảo Apple Vision Pro

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/4002) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024020902.webp)

Bức ảnh đoạt giải nhất trong cuộc thi Nhiếp ảnh gia Động vật hoang dã Quốc tế (năm 2023): một chú gấu Bắc Cực nhỏ trên tảng băng trôi gần quần đảo Svalbard, Na Uy, đã dùng móng vuốt đào ra một chỗ ngủ rồi cuộn tròn ngủ thiếp đi. (Nguồn: [Live Science](https://www.livescience.com/animals/polar-bears/polar-bear-sleeping-on-tiny-iceberg-drifting-in-arctic-sea-captured-in-heartbreaking-photo))

## 苹果头盔的最大问题

Trước Tết Nguyên Đán, kính thực tế ảo Apple Vision Pro của Apple đã chính thức được mở bán.

Đây là thiết bị phần cứng đột phá nhất trong những năm gần đây, với đợt mở bán đầu tiên gồm 200.000 máy nhanh chóng cháy hàng.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021801.webp)

Thiết bị hiện chỉ được bán tại Mỹ và chưa có tên gọi tiếng Việt chính thức. Để thuận tiện cho việc trình bày, tôi sẽ tạm gọi nó là "kính thực tế ảo Apple".

Dù gọi như vậy, nhưng Apple không định vị thiết bị này là một kính thực tế ảo VR thông thường, mà gọi nó là một "máy tính không gian" (spatial computer).

Tên gọi này mang hàm ý rất lớn, thể hiện tầm nhìn dài hạn của Apple: **đây là một thiết bị máy tính cá nhân đa năng giống như laptop hay điện thoại thông minh**, thuộc nhóm thiết bị tính toán phục vụ người dùng cá nhân.

Trong mắt Apple, ba thiết bị này - Mac, iPhone và kính thực tế ảo Apple - đều giải quyết được các nhu cầu công việc tương đồng nhau, điểm khác biệt duy nhất là không gian sử dụng. Mac là máy tính để bàn, iPhone là máy tính di động và kính thực tế ảo Apple là máy tính đeo được.

Trang tin chuyên tháo dỡ thiết bị iFixit [đã mổ xẻ kính thực tế ảo Apple](https://zh.ifixit.com/News/90137/vision-pro-teardown-why-those-fake-eyes-look-so-weird) và xác nhận **CPU của máy sử dụng chip M2 tương tự như trên dòng laptop MacBook**. Do đó về mặt lý thuyết, bất kỳ phần mềm nào chạy được trên MacBook đều có thể hoạt động mượt mà trên kính thực tế ảo Apple.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021802.webp)

Vấn đề đặt ra là: **Liệu kính thực tế ảo Apple có thể thực sự thay thế cho một chiếc máy tính làm việc đa năng thông thường?**

Một số chuyên gia bày tỏ quan điểm vô cùng lạc quan, cho rằng không gian ảo của thiết bị mang lại trải nghiệm chưa từng có, biến các màn hình vật lý truyền thống thành các màn hình ảo sinh động giúp người dùng hoàn toàn có thể đeo kính để làm việc văn phòng. Số khác lại nhận định thiết bị vẫn tồn tại những điểm nghẽn kỹ thuật chưa thể khắc phục để phục vụ công việc thực tế.

Nhà phân tích công nghệ nổi tiếng Ben Thompson đã chia sẻ chi tiết về [trải nghiệm sử dụng thực tế của mình](https://stratechery.com/2024/the-apple-vision-pro/). Tôi thấy những nhận định của ông rất sâu sắc và đáng để tham khảo.

Ông chia sẻ, ấn tượng đầu tiên khi đeo kính là thiết bị mang lại trải nghiệm xem phim giải trí vô cùng tuyệt vời và chân thực. Vợ ông thậm chí đã thốt lên: "Có thiết bị này rồi thì cần gì phải ra rạp chiếu phim nữa?"

Nhưng, khi ông thử nghiệm sử dụng kính để soạn thảo bài viết, ông đã ngay lập tức phát hiện ra một điểm nghẽn lớn khiến thiết bị chưa thể đáp ứng tốt cho các nhu cầu công việc thực thụ.

**Vấn đề cốt lõi đó là: cơ chế quản lý đa cửa sổ (multitasking) trên kính thực tế ảo Apple hoạt động khá tệ**. Nếu bạn chỉ thao tác trên một cửa sổ duy nhất, mọi thứ diễn ra rất mượt mà; nhưng khi mở đồng thời nhiều cửa sổ công việc, sự bất tiện sẽ xuất hiện.

"Nếu các cửa sổ được sắp xếp chồng chéo lên nhau theo trục Z (ở các khoảng cách xa gần khác nhau trước mắt người nhìn), giao diện người dùng sẽ cực kỳ khó thao tác (hình dưới). Do thiết bị áp dụng công nghệ theo dõi chuyển động mắt (eye tracking), độ chính xác của nó chưa đủ nhạy để phân biệt giữa các cửa sổ xếp chồng. Bạn sẽ gặp rất nhiều khó khăn để chọn trúng cửa sổ mong muốn."

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024022107.webp)

*(Chú thích ảnh: Khi nhiều cửa sổ xếp chồng trước sau, việc chọn trúng cửa sổ mong muốn chỉ bằng ánh nhìn là một thử thách khó khăn).*

"Trong trường hợp bạn sắp xếp các cửa sổ dàn trải (xếp cạnh nhau) trên không gian bàn làm việc ảo (hình dưới), bạn sẽ nhận thấy góc nhìn (Field of View - FOV) của kính thực tế ảo Apple tương đối hẹp (Apple chưa công bố thông số chính thức này nhưng cảm giác thực tế nhỏ hơn mức 110° của Quest 3), bạn không thể quan sát trọn vẹn nội dung của hai cửa sổ đặt cạnh nhau cùng một lúc."

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024022108.webp)

*(Chú thích ảnh: Góc nhìn của kính thực tế ảo Apple tương đối hẹp, không thể hiển thị song song trọn vẹn hai cửa sổ lớn).*

"Điều này đồng nghĩa với việc cứ mỗi khi muốn xem nội dung đầy đủ của cửa sổ bên cạnh, bạn buộc phải xoay đầu hoặc di chuyển cơ thể một cách cơ học."

Tóm lại, **trải nghiệm đa cửa sổ trên kính thực tế ảo Apple hiện tại khá tệ**, sự bất tiện này tương tự như cơ chế chia màn hình trên iPad.

Do không thể giải quyết triệt để bài toán đa cửa sổ, iPad đến nay vẫn chỉ được coi là một thiết bị giải trí thuần túy hơn là một công cụ làm việc hiệu suất cao. Kính thực tế ảo Apple cũng đang gặp phải vấn đề tương tự: nó chưa thần kỳ như những gì Apple quảng cáo, chưa thể trở thành một máy tính không gian thực thụ để thay thế laptop phục vụ công việc hàng ngày.

**Điều người dùng thực sự cần trong công việc là một không gian hiển thị khổng lồ có thể chứa đồng thời và trọn vẹn nhiều cửa sổ**, đó là lý do vì sao hầu hết các lập trình viên thường trang bị thêm nhiều màn hình ngoài kết nối với laptop (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021803.webp)

Nếu kính thực tế ảo Apple có thể giải quyết tốt trải nghiệm đa cửa sổ này, nó sẽ trở thành thiết bị khai tử cho các dòng laptop truyền thống và mở ra tiềm năng thị trường vô cùng lớn, nhưng tiếc là hiện tại nó vẫn chưa làm được.

Do đó, nếu bạn mua kính thực tế ảo Apple thuần túy cho mục đích giải trí, đây là một lựa chọn đáng giá; nhưng nếu muốn ứng dụng nó vào công việc hay học tập, lời khuyên là hãy kiên nhẫn chờ đợi các phiên bản nâng cấp hoàn thiện hơn tính năng đa cửa sổ trong tương lai.

Nhận định này cũng hoàn toàn trùng khớp với đánh giá ngắn gọn của tờ [The New York Times](https://www.nytimes.com/2024/02/07/technology/personaltech/apple-vision-pro-review.html): "**Ngoại trừ chức năng như một chiếc TV cá nhân sang trọng, thiết bị này hiện vẫn thiếu các tính năng ứng dụng thực tế.**"

## 科技动态

1、[Cảnh báo nguy cơ bảo mật của hệ thống camera an ninh không dây](https://www.tomshardware.com/networking/wi-fi-jamming-to-knock-out-cameras-suspected-in-nine-minnesota-burglaries-smart-security-systems-vulnerable-as-tech-becomes-cheaper-and-easier-to-acquire)

Cảnh sát bang Minnesota, Mỹ gần đây đã bắt giữ một kẻ trộm công nghệ cao chịu trách nhiệm cho chuỗi 9 vụ đột nhập trộm cắp tài sản liên tiếp.

Điểm chung của các ngôi nhà bị đột nhập là đều lắp đặt hệ thống camera an ninh không dây, và tên trộm đã tìm cách vô hiệu hóa hoàn toàn camera trước khi ra tay.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021501.webp)

Thủ đoạn của tên trộm thực chất rất đơn giản: sử dụng một thiết bị phá sóng WiFi (WiFi jammer).

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021502.webp)

Các dòng camera không dây phụ thuộc hoàn toàn vào sóng WiFi để truyền và lưu trữ hình ảnh về ổ cứng đám mây hoặc máy chủ từ xa. Khi bị thiết bị phá sóng gây nghẽn tín hiệu WiFi, dù camera vẫn ghi nhận được hình ảnh nhưng dữ liệu không thể lưu trữ hay phát đi cảnh báo, giúp tên trộm dễ dàng đột nhập trộm cắp.

Mối đe dọa bảo mật này đã được cảnh báo từ lâu nhưng chưa có giải pháp khắc phục triệt để. Do đó đối với các vị trí giám sát trọng yếu, người dùng nên ưu tiên sử dụng kết nối dây mạng vật lý truyền thống.

2、[Phương pháp cai nghiện điện thoại thông minh hiệu quả](https://www.nytimes.com/2024/02/01/technology/iphone-mental-health-flip-phone.html)

Một doanh nghiệp tại New York mong muốn các nhân viên của mình tập trung làm việc và giảm thiểu thời gian sử dụng điện thoại cá nhân trong giờ làm.

Để thực hiện mục tiêu này, công ty đưa ra quy định yêu cầu toàn bộ nhân viên phải đặt điện thoại lên hệ thống kệ đựng chuyên dụng (device shelf) bố trí ngoài cửa phòng họp trước khi vào họp.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024020501.webp)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024020502.webp)

Đồng thời, công ty cũng cam kết chi trả toàn bộ chi phí mua sắm thiết bị nếu nhân viên đồng ý từ bỏ điện thoại thông minh để chuyển sang sử dụng các dòng điện thoại nắp gập cơ bản.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024020503.webp)

Kết quả thử nghiệm thực tế cho thấy giải pháp chuyển sang điện thoại nắp gập mang lại hiệu quả rất tốt trong việc giúp nhân viên từ bỏ thói quen nghiện điện thoại.

3、[Tranh luận xoay quanh dự án trùng tu Kim tự tháp Ai Cập](https://www.timesofisrael.com/egyptian-pyramid-undergoes-renovation-drawing-criticism/)

Chính phủ Ai Cập mới đây đã khởi động dự án trùng tu các công trình Kim tự tháp bằng cách ốp thêm một lớp đá hoa cương bên ngoài thân tháp.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024020701.webp)

Theo các tài liệu khảo cổ học, khi mới được xây dựng, bề mặt bên ngoài của Kim tự tháp được bao phủ bảo vệ bởi một lớp đá hoa cương mịn màng, nhưng lớp đá này đã bị phong hóa sụt lún và biến mất theo thời gian.

Phía chính phủ Ai Cập nhận định việc trùng tu sẽ giúp du khách có cơ hội trải nghiệm diện mạo nguyên bản nhất của Kim tự tháp cổ đại, đồng thời giúp bảo vệ cấu trúc đá lõi bên trong tháp.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024020702.webp)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024020703.webp)

Tuy nhiên, dự án gặp phải sự phản đối gay gắt từ giới khảo cổ học quốc tế. Nhiều chuyên gia cho rằng hành động này đang phá hoại nghiêm trọng di tích lịch sử, thậm chí có ý kiến châm biếm: "Tại sao không dán luôn gạch men lên Kim tự tháp cho nhanh?"

Dự án phản ánh bài toán nan giải trong công tác bảo tồn di sản: liệu có nên trùng tu phục dựng lại các kiến trúc cổ và phương án trùng tu như thế nào để không làm mất đi giá trị lịch sử nguyên bản.

4、[Cảnh báo nguy cơ rác thải vệ tinh làm suy giảm từ trường Trái Đất](spaceweatherarchive.com/2024/02/01/will-satellite-megaconstellations-weaken-earths-magnetic-field/)

Dự án phủ mạng Internet vệ tinh Starlink của SpaceX lên kế hoạch phóng tới 12.000 vệ tinh nhỏ lên quỹ đạo tầm thấp, và hiện đã phóng thành công hơn 5.000 thiết bị.

Rất nhiều tập đoàn công nghệ khác cũng công bố kế hoạch xây dựng hệ thống mạng vệ tinh tương tự. Giới khoa học bày tỏ sự lo ngại sâu sắc về các tác động tiêu cực chưa thể kiểm soát khi có quá nhiều vệ tinh nhỏ quay quanh Trái Đất.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024020704.webp)

Nguy cơ lớn nhất được cảnh báo là việc làm biến dạng và suy giảm cường độ từ trường Trái Đất.

Trong vài thập kỷ tới, các thế hệ vệ tinh này sẽ dần hết hạn sử dụng, phân rã và rơi trở lại bầu khí quyển. Quá trình đó sẽ giải phóng một lượng khổng lồ các hạt và mảnh vụn kim loại lơ lửng trong không gian vũ trụ. Khi mật độ hạt đạt đến giới hạn, chúng sẽ tạo thành một lớp hạt điện tích khổng lồ bao quanh bầu khí quyển.

Lớp hạt điện tích nhân tạo này hoạt động giống như một lớp vỏ dẫn điện bao bọc Trái Đất, gây ra hiện tượng lồng Faraday ngăn cản từ trường Trái Đất tương tác ra bên ngoài vũ trụ.

Từ trường Trái Đất đóng vai trò lá chắn bảo vệ sự sống khỏi tác động của các tia vũ trụ độc hại và các đợt bão Mặt Trời mạnh mẽ. Việc lá chắn này bị vô hiệu hóa sẽ dẫn đến những hậu quả thảm khốc chưa thể dự đoán trước.

5、[Ảnh chụp cận cảnh núi lửa trên vệ tinh Io của Sao Mộc](science.nasa.gov/get-involved/citizen-science/for-your-processing-pleasure-the-sharpest-pictures-of-jupiters-volcanic-moon-io-in-a-generation/)

Trong tháng này, tàu vũ trụ Juno của NASA đã thực hiện chặng bay tiếp cận cực gần vệ tinh Io của Sao Mộc ở khoảng cách chưa đầy 1500 km.

Tàu thăm dò đã truyền về những hình ảnh có độ phân giải cao nhất từ trước đến nay của vệ tinh Io, hiển thị chi tiết bề mặt địa hình.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021001.webp)

Trong hệ Mặt Trời, Io là thiên thể có núi lửa hoạt động mạnh nhất. Do Io ở quá gần Sao Mộc nên chịu lực hấp dẫn cực kỳ mạnh mẽ, khiến địa hình bên trong luôn thay đổi dữ dội và tạo nên vô số ngọn núi lửa đang phun trào liên tiếp.

## Bài viết

1\. [Giới thiệu các kỹ thuật can thiệp và kiểm soát HTTP trên nền tảng Web](https://hughfenghen.github.io/posts/2023/12/23/web-spy/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021006.webp)

Bài viết giới thiệu các phương pháp phổ biến để can thiệp và kiểm soát luồng giao tiếp dữ liệu HTTP trên trình duyệt Web, đồng thời hướng dẫn cách thức chèn mã can thiệp hiệu quả. (Đóng góp của [@hughfenghen](https://github.com/ruanyf/weekly/issues/4014))

2\. [Phân tích chi tiết cấu trúc chứng chỉ SSL/TLS](https://jvns.ca/blog/2017/01/31/whats-tls/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121103.webp)

Bài viết giới thiệu một cách dễ hiểu về phương pháp kiểm tra nội dung chứng chỉ bảo mật HTTPS và giải thích ý nghĩa các thông số cơ bản cấu thành chứng chỉ.

3\. [Tìm hiểu các yêu cầu kết nối tự động của trình duyệt Web](https://sizeof.cat/post/web-browser-telemetry/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121201.webp)

Thống kê chi tiết các yêu cầu HTTP tự động phát đi ngay khi người dùng mở trình duyệt. Ví dụ: Firefox tự động gửi 15 yêu cầu, Chrome gửi 12 yêu cầu và Edge gửi tới 21 yêu cầu kết nối ngầm.

4\. [Hướng dẫn xây dựng thành phần Web Component cho trình phát video responsive](https://calendar.perfplanet.com/2023/extending-responsive-video-with-html-web-components/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121303.webp)

Bài viết hướng dẫn lập trình viên từng bước xây dựng các thành phần Web Components thông qua ví dụ thiết kế một trình phát video có khả năng hiển thị tương thích tốt trên nhiều thiết bị.

5\. [Cảnh báo nguy cơ bảo mật từ việc cài đặt các tiện ích mở rộng Chrome thiếu uy tín](https://mattfrisbie.substack.com/p/spy-chrome-extension)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110712.webp)

Tác giả đưa ra lời cảnh báo sâu sắc về việc các extension trên trình duyệt hoàn toàn có khả năng đọc trộm mọi thông tin nhạy cảm của người dùng và gửi về máy chủ từ xa, đồng thời cung cấp mã nguồn demo minh họa cơ chế hoạt động nguy hại này.

6\. [Tìm hiểu chi tiết về cơ chế mã hóa Base32](https://ptrchm.com/posts/base32-explained/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121801.webp)

Bài viết giải thích chi tiết nguyên lý toán học và cách thức triển khai mã hóa của các định dạng Base64, Base32 và Base8 trong lập trình.

7\. [Hướng dẫn thiết lập tính năng xác thực hai yếu tố cho kết nối SSH](https://linuxiac.com/how-to-set-up-ssh-to-use-two-factor-authentication/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121915.webp)

Bài viết hướng dẫn chi tiết các bước cấu hình để kích hoạt tính năng xác thực hai lớp (2FA) bảo vệ kết nối SSH vào máy chủ Linux.

8\. [Hệ thống kiến thức về kiến trúc GPU dành cho lập trình viên phần mềm](https://journal.hexmos.com/gpu-survival-toolkit/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111306.webp)

Trong bối cảnh công nghệ AI bùng nổ kéo theo nhu cầu tính toán hiệu năng cao trên GPU, bài viết hệ thống lại các khái niệm cơ bản về cấu trúc phần cứng GPU và giới thiệu các phương pháp lập trình GPU chuyên sâu.

## 工具

1\. [Zed (Trình biên tập mã nguồn thế hệ mới)](https://zed.dev/)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021902.webp)

Trình biên tập mã nguồn với tốc độ phản hồi cực nhanh, hỗ trợ đa nền tảng, được phát triển bởi chính đội ngũ kỹ sư từng xây dựng nên trình biên tập Atom nổi tiếng.

Bên cạnh đó, sau khi dự án Atom chính thức đóng cửa, cộng đồng đã tiếp tục phát triển mã nguồn mở này dưới tên gọi mới là [Pulsar](https://optimizedbyotto.com/post/pulsar-best-text-file-and-code-editor/) - một lựa chọn trình biên tập code rất đáng chú ý.

2\. [TCPView](https://learn.microsoft.com/en-us/sysinternals/downloads/tcpview)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021005.webp)

Phần mềm chính thức từ Microsoft hỗ trợ theo dõi trực quan và chi tiết tất cả các kết nối mạng giao thức TCP và UDP đang hoạt động trên hệ thống Windows. (Đóng góp của [@meq1986](https://github.com/ruanyf/weekly/issues/4013))

3\. [EasyDevo](https://easydevo.boringboring.design/)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021008.webp)

Ứng dụng dọn dẹp hệ thống dành riêng cho hệ điều hành macOS, hỗ trợ quét xóa các tệp tin rác và giám sát trực quan các chỉ số hiệu năng (mạng, CPU, RAM và pin). Xem thêm [bài viết giới thiệu công cụ](https://medium.com/@hi_caicai/easydevo-the-developer-tool-you-might-need-a70dfd6ee3e1). (Đóng góp của [@hi-caicai](https://github.com/ruanyf/weekly/issues/4018))

4\. [FontMagic](https://github.com/leibnizli/fontmagic)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021905.webp)

Phần mềm quản lý và xử lý phông chữ nghệ thuật, hỗ trợ trích xuất nhanh các ký tự glyph bất kỳ trong file font thành định dạng ảnh vectơ SVG và chuyển đổi qua lại giữa các định dạng font phổ biến, tương thích macOS và Windows. (Đóng góp của [@leibnizli](https://github.com/ruanyf/weekly/issues/4028))

5\. [uv](https://astral.sh/blog/uv)

Công cụ quản lý gói thư viện Python được viết bằng ngôn ngữ Rust mang lại tốc độ xử lý vượt trội, sẵn sàng thay thế hoàn hảo cho `pip` và `pip-tools`. (Đóng góp của [@qiaouchicago](https://github.com/ruanyf/weekly/issues/4030))

6\. [Keep Screen On](https://www.keepscreenon.com/)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021906.webp)

Dịch vụ web đơn giản giúp ngăn màn hình máy tính hoặc điện thoại tự động tắt ngủ, tương thích tốt trên các nền tảng Windows, macOS, Android và iOS. (Đóng góp của [@tufucheung](https://github.com/ruanyf/weekly/issues/4033))

7\. [background-erase.xyz](https://background-erase.xyz/)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021908.webp)

Dịch vụ trực tuyến hỗ trợ xóa nền ảnh chân dung miễn phí, ứng dụng mô hình AI RMBG-v1.4 hiện đại với toàn bộ tác vụ tính toán chạy trực tiếp trên trình duyệt của người dùng mà không cần upload ảnh lên server. (Đóng góp của [@janily](https://github.com/ruanyf/weekly/issues/4040))

8\. [browserscan.net](https://www.browserscan.net/)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024022202.webp)

Dịch vụ trực tuyến hỗ trợ kiểm tra nhanh các thông số cấu hình vân tay trình duyệt (browser fingerprinting), địa chỉ IP thực tế và phát hiện các rò rỉ bảo mật qua giao thức WebRTC hoặc DNS. (Đóng góp của [@BrowserScan](https://github.com/ruanyf/weekly/issues/4045))

9\. [NPMprune](https://github.com/xthezealot/npmprune)

Kịch bản lệnh Shell hỗ trợ tự động tìm và xóa các tệp tin không cần thiết (như các file tài liệu Markdown) trong thư mục `node_modules`, giúp tối ưu hóa dung lượng gói build khi đóng gói container.

10\. [Localtunnel](https://theboroer.github.io/localtunnel-www/)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023093004.webp)

Công cụ Node.js hỗ trợ gán nhanh một địa chỉ tên miền public trỏ trực tiếp về cổng chạy dịch vụ local trên máy tính cá nhân, giúp kiểm thử nhanh dịch vụ.

11\. [SirTunnel](https://github.com/anderspitman/SirTunnel)

Dự án mã nguồn mở tối giản chỉ với 50 dòng code giúp thiết lập nhanh đường truyền tunnel để kết nối máy tính trong mạng nội bộ ra ngoài mạng Internet public. Xem thêm [bài viết hướng dẫn cài đặt](https://eighty-twenty.org/2023/01/27/sirtunnel-personal-ngrok).

## 资源

1\. **Tổng hợp tài nguyên video minh họa của mô hình Sora**

OpenAI mới đây đã gây xôn xao giới công nghệ khi giới thiệu mô hình tạo video từ mô tả văn bản Sora, có khả năng tạo ra các video chân thực dài tới 60 giây.

Mô hình này hiện chưa chính thức được phát hành cho tất cả mọi người, chỉ hiển thị một số video mẫu. Các trang web sau đây giúp bạn tổng hợp video và xem các câu lệnh (prompts) tương ứng:

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021907.webp)

- [SoraPrompts](https://soraprompts.co/) (Đóng góp của [@GregoryZeng](https://github.com/ruanyf/weekly/issues/4034))
- [SoraHub](https://sorahub.video/zh) (Đóng góp của [@JasonJJLL](https://github.com/ruanyf/weekly/issues/4035))
- [Sora Videos](https://soravideos.media/) (Đóng góp của [@MuYiBo](https://github.com/ruanyf/weekly/issues/4041))

2\. [Ái Phát Âm (Fayin Love)](https://fayin.love/)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024022102.webp)

Trang web hỗ trợ học phát âm bảng ký tự âm tiếng Anh trực quan, cung cấp video và audio hướng dẫn phát âm chi tiết cho từng âm theo chuẩn Anh - Anh và Anh - Mỹ. (Đóng góp của [@Yidoon](https://github.com/ruanyf/weekly/issues/4042))

3\. [Tài liệu học tập toàn diện về thiết kế đồ họa ảnh vectơ SVG](https://svg-tutorial.com/)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120801.webp)

Chuỗi 25 bài học bằng tiếng Anh được thiết kế từ cơ bản đến nâng cao đi kèm các ví dụ thực hành trực quan giúp bạn làm chủ thiết kế đồ họa SVG.

4\. [Tổng hợp các giải pháp khắc phục điểm yếu của hệ thống quản lý mã nguồn Git](https://news.ycombinator.com/item?id=38590080)（Tiếng Anh）

Hệ thống Git vẫn tồn tại một số nhược điểm như chưa hỗ trợ tốt các tệp tin nhị phân dung lượng lớn, gặp khó khăn khi quản lý dự án quy mô siêu lớn, cấu trúc lệnh phức tạp và bất tiện khi quản lý submodule...

Liên kết trên dẫn đến cuộc thảo luận của các kỹ sư trên Hacker News chia sẻ các kinh nghiệm và công cụ bổ trợ giúp khắc phục các nhược điểm này.

## 图片 

1\. [Ảnh chụp vệ tinh khoảnh khắc núi lửa phun trào tại Băng Đảo](https://kottke.org/24/02/incredible-satellite-images-of-the-latest-volcanic-eruption-in-iceland)

Khoảnh khắc núi lửa phun trào được ghi nhận bởi vệ tinh nhân tạo hiển thị một vệt lửa đỏ rực nổi bật giữa thung lũng tuyết trắng xóa tại Iceland.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021007.webp)

2\. [Nguồn gốc lịch sử thói quen sử dụng đơn vị cân đo Kg tại Vân Nam](https://twitter.com/ruanyf/status/1757002038981112152)

Tại hầu hết các tỉnh thành Trung Quốc, người dân thường sử dụng đơn vị cân truyền thống (cân Trung Quốc - 1/2 kg) trong giao dịch hàng ngày. Tuy nhiên tại một số vùng thuộc tỉnh Vân Nam (như Côn Minh), người dân lại quen dùng đơn vị kg (kilogram), nguyên nhân do đâu?

Lịch sử ghi nhận vào đầu thế kỷ trước, chính phủ Pháp đã xây dựng tuyến đường sắt Điền - Việt kết nối Việt Nam và tỉnh Vân Nam.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021201.webp)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024022103.webp)

Nước Pháp là quốc gia phát minh ra hệ đo lường quốc tế mét, nên tất cả các khu vực dọc theo tuyến đường sắt này đều chuyển sang dùng kilogram: từ Hà Khẩu, Bình Biên, Mông Tự, Khai Viễn đến Côn Minh. Thói quen này vẫn được duy trì cho đến ngày nay.

3\. [Tác phẩm nghệ thuật điêu khắc gỗ mô phỏng luồng ánh sáng đèn xe](https://www.thisiscolossal.com/2024/02/kiko-miyares-headlights/)

Một nghệ sĩ điêu khắc người Tây Ban Nha đã tạo nên những tác phẩm điêu khắc gỗ độc đáo, tái hiện sinh động hình ảnh những chiếc ô tô đi kèm luồng ánh sáng đèn pha chiếu ra phía trước.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024022104.webp)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024022105.webp)

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024022106.webp)

## ✍️ Bài đọc thêm

### Bài học thú vị về áp lực cạnh tranh tâm lý từ những làn bơi trong bể bơi

Cách đây vài năm, tôi có cơ hội tham gia một khóa huấn luyện kỹ năng bơi lội.

Toàn bộ học viên được phân chia tập luyện trên các làn bơi khác nhau tùy thuộc vào năng lực cá nhân: làn A (dành cho những người bơi nhanh nhất), làn B (nhóm khá), làn C (nhóm trung bình) và làn D (nhóm bơi chậm nhất).

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024022203.webp)

Tôi bắt đầu hành trình từ làn D và nhận được nhiều sự chỉ dẫn tận tình từ mọi người. Sau khi tiến bộ dần, tôi chuyển sang làn C và tiếp tục nhận được sự chào đón thân thiện của các học viên tại đây.

Tuy nhiên, tôi nhận thấy các học viên ở làn B bên cạnh lại không hề có thái độ cởi mở và thân thiện như nhóm làn C hay làn A. Những học viên xuất sắc nhất ở làn A luôn rất cởi mở, sẵn sàng chia sẻ kinh nghiệm, dành nhiều lời động viên và chỉ dẫn hữu ích cho người khác.

Tôi đoán đây là một hiện tượng phổ biến: những người ở làn A, C và D đều thân thiện và sẵn lòng giúp đỡ người khác; còn những người ở làn B chỉ thân thiện với làn A và những người cùng làn B khác, còn đối với làn C và D thì không.

Bởi vì sau này tôi phát hiện ra điều này cũng đúng ở các môn thể thao khác. Những vận động viên ở nhóm tiệm cận xuất sắc thường rất khắt khe với những người yếu hơn mình, vì lo sợ sẽ bị vượt mặt.

Trong môi trường học thuật cũng tồn tại hiện tượng tương tự. Những giáo sư đầu ngành thực thụ thường rất hào hiệp và sẵn lòng hỗ trợ các nhà nghiên cứu trẻ, và những nghiên cứu viên có năng lực trung bình cũng vậy. Ngược lại, những học giả đã có chút danh tiếng nhưng chưa thể vươn lên tầm đỉnh cao thường có xu hướng khắt khe và thiếu thân thiện với những người có năng lực kém hơn.

Khi bạn ở vị trí số một (nhóm A), bạn rất dễ thể hiện sự rộng lượng vì bạn hoàn toàn tự tin vào vị thế của mình mà không cần lo lắng về sự cạnh tranh.

Khi ở vị trí trung bình hoặc thấp hơn (nhóm C hoặc D), việc duy trì thái độ thân thiện cũng rất dễ dàng do áp lực cạnh tranh không quá lớn, nhịp độ học tập thoải mái giúp bạn giữ được tâm lý nhẹ nhàng.

Nhưng đối với nhóm tiệm cận xuất sắc, áp lực là vô cùng lớn. Họ đã ở rất gần đỉnh cao nhưng chặng đường bứt phá tiếp theo lại vô cùng gian nan, buông bỏ thì tiếc nuối mà cố gắng thì mệt mỏi. Điều đáng buồn là lịch sử thường chỉ nhớ đến người chiến thắng ở vị trí số một, trong khi những người ở nhóm sau vẫn có nguy cơ vượt qua họ bất cứ lúc nào. Các áp lực này gián tiếp tạo nên thái độ khắt khe của họ đối với xung quanh.

## Lịch sử tuần này

- 2023年（第 243 期）：[Trải nghiệm công nghệ: Giai thoại thú vị về cuộc trò chuyện thử nghiệm cùng AI mô phỏng Khổng Tử](https://www.ruanyifeng.com/blog/2023/02/weekly-issue-243.html)
- 2022年（第 193 期）：[Thảo luận nghề nghiệp: Phân tích và so sánh độ khó công việc giữa lập trình viên Frontend và Backend](https://www.ruanyifeng.com/blog/2022/01/weekly-issue-193.html)
- 2021年（第 143 期）：[Thưởng thức nghệ thuật: Giới thiệu tiểu thuyết "Xứ sở diệu kỳ tàn bạo và chốn tận cùng thế giới" của Haruki Murakami](https://www.ruanyifeng.com/blog/2021/01/weekly-issue-143.html)
- 2020年（第 93 期）：[Xu hướng công nghệ: Dự báo về sự bùng nổ của các dòng game thế giới mở (roaming games) tương lai](https://www.ruanyifeng.com/blog/2020/02/weekly-issue-93.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
