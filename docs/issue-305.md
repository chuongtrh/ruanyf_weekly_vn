# Bản tin chia sẻ công nghệ (Số 305): Số ngẫu nhiên, đó là cả một vấn đề

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/4550) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061403.webp)

Trạm xe buýt "Duyệt Lai Giang Vịnh" tại Trùng Khánh. Trạm được xây dựng từ một vài khối đá khổng lồ, mô phỏng hình ảnh những viên đá cuội ven sông của địa phương. (Nguồn: [Yuelai](http://www.cqyuelai.com/yuelai_content/2023-09/21/content_10592221.htm))

## 随机数，这是一个问题

Hôm nay, chúng ta cùng bàn về phương pháp khởi tạo một số ngẫu nhiên thực sự.

Đây là một bài toán vô cùng phức tạp, nhưng ẩn chứa nhiều câu chuyện công nghệ thú vị.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061814.webp)

Trước hết, các số ngẫu nhiên được sinh ra bởi các ngôn ngữ lập trình thông dụng thực chất chỉ là số giả ngẫu nhiên (pseudo-random numbers).

Trang chủ của V8 Engine có [một bài phân tích](https://v8.dev/blog/math-random) (hình dưới) đặc biệt lưu ý người dùng về thực tế này: hàm sinh số ngẫu nhiên mặc định bên trong công cụ không phải là ngẫu nhiên thực sự mà là giả ngẫu nhiên.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061606.webp)

Khái niệm giả ngẫu nhiên có nghĩa là chúng không xuất hiện ngẫu nhiên một cách tự nhiên mà được tạo ra thông qua các thuật toán toán học chạy trên máy tính. Chỉ cần giá trị khởi tạo (seed - hạt giống) ban đầu giống nhau, thuật toán sẽ luôn trả về một dãy kết quả hoàn toàn trùng khớp.

Ngôn ngữ JavaScript và nhiều ngôn ngữ lập trình khác đều hoạt động theo cơ chế này. Do đó, đối với các hệ thống yêu cầu độ bảo mật và tính ngẫu nhiên cực cao, lập trình viên tuyệt đối không được sử dụng các hàm sinh số ngẫu nhiên mặc định tích hợp sẵn.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061815.webp)

Một số ngẫu nhiên thực sự (true random number) bắt buộc phải đáp ứng đồng thời 3 tiêu chuẩn sau:

> **（1）Không thể dự đoán trước.** Dãy số sinh ra không thể bị suy đoán trước bằng bất kỳ quy luật nào, do đó nó phải đủ lớn để chống lại các cuộc tấn công brute-force.
> 
> **（2）Không lặp lại.** Mỗi lần khởi tạo, dãy số sinh ra bắt buộc phải có sự khác biệt, không được trùng lặp với kết quả trước đó.
> 
> **（3）Phân phối đồng đều.** Dãy số ngẫu nhiên phải được rải đều trên toàn bộ không gian số, không được tập trung hay thiên lệch về một vài vùng cụ thể.

**Nhìn chung, máy tính chỉ có thể tạo ra số ngẫu nhiên thực sự thông qua việc ghi nhận các tín hiệu vật lý từ phần cứng**, các thuật toán phần mềm đơn thuần hoàn toàn bất khả thi.

Giới khoa học đã dày công nghiên cứu nhiều phương pháp khai thác phần cứng để thu thập dữ liệu ngẫu nhiên từ tự nhiên.

Chuyên trang [Random.org](https://www.random.org/) là một dịch vụ nổi tiếng chuyên cung cấp các số ngẫu nhiên thực sự.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061816.webp)

Họ thiết lập một mạng lưới các đầu thu sóng vô tuyến đặt ở nhiều nơi trên thế giới để liên tục ghi nhận các nhiễu động sóng vô tuyến trong bầu khí quyển (nhiễu khí quyển, bản chất tương tự chuyển động Brown của các phân tử khí). Các tín hiệu nhiễu ngẫu nhiên này sau đó được chuyển đổi thành số ngẫu nhiên. Dưới đây là hình ảnh thiết bị phần cứng thời kỳ đầu của họ.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061817.webp)

Do phải gánh chịu chi phí vận hành và bảo trì thiết bị phần cứng, người dùng muốn sử dụng dịch vụ số ngẫu nhiên thực sự của Random.org bắt buộc phải trả phí. Điều này cho thấy số ngẫu nhiên thực sự có chi phí rõ ràng chứ không đơn giản chỉ là chạy một dòng lệnh lập trình.

Để sở hữu nguồn số ngẫu nhiên thực sự cho dịch vụ bảo mật của mình, tập đoàn Cloudflare thậm chí còn triển khai giải pháp độc đáo hơn.

Tại ba văn phòng đại diện lớn của hãng, họ lắp đặt ba hệ thống thiết bị tạo số ngẫu nhiên vật lý [hoàn toàn khác biệt](https://blog.cloudflare.com/harnessing-office-chaos).

**（1）Trụ sở chính tại San Francisco**. Ngay tại sảnh vào của tòa nhà được trang bị một bức tường trưng bày hàng chục chiếc đèn dung nham (lava lamps).

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031204.webp)

Chất sáp nóng chảy bên trong các bóng đèn dung nham liên tục chuyển động và thay đổi hình dạng ngẫu nhiên không ngừng nghỉ.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061818.webp)

Mỗi khi hệ thống cần khởi tạo số ngẫu nhiên, một camera sẽ chụp lại bức ảnh của bức tường đèn này. Do trạng thái sáp liên tục biến đổi, mỗi bức ảnh chụp được sẽ là duy nhất. Thuật toán sẽ tính toán giá trị băm (hash) của bức ảnh đó để làm seed khởi tạo số ngẫu nhiên.

**（2）Văn phòng London.** Nơi đây được trang bị một bức tường lắp đặt các hệ thống con lắc đơn chuyển động tự do.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031205.webp)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031206.webp)

Chuyển động của các con lắc cùng bóng đổ của chúng thay đổi liên tục theo thời gian. Hình ảnh ghi nhận từ camera tại đây cũng được băm để tạo seed số ngẫu nhiên.

**（3）Văn phòng Austin.** Trên trần nhà của văn phòng được treo rất nhiều tấm thẻ phản quang nhiều màu sắc.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031207.webp)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031208.webp)

Các tấm thẻ phản quang này chuyển động cực kỳ nhạy cảm trước luồng không khí lưu thông trong phòng (do gió điều hòa, người qua lại đóng mở cửa, thay đổi nhiệt độ, độ ẩm). Sự xoay chuyển của chúng tạo nên các phản xạ màu sắc khác nhau, cung cấp nguồn dữ liệu ngẫu nhiên hoàn hảo cho thuật toán băm.

## 下周五，稀土开发者大会

Trong suốt một tháng qua, bản tin liên tục chia sẻ thông tin cập nhật về sự kiện "Đại hội Lập trình viên Xitu" năm nay.

Sự kiện sẽ chính thức khai mạc vào thứ Sáu tuần tới (ngày 28 tháng 6).

Là một sự kiện công nghệ quy mô lớn trong năm, toàn bộ lịch trình chi tiết đã được ban tổ chức công bố. Dưới đây là **danh sách hơn 70 chủ đề tham luận tại diễn đàn chính và 10 phân hội chuyên đề**.

[![](https://cdn.beekka.com/blogimg/asset/202406/bg2024062004.webp)](https://cdn.beekka.com/blogimg/asset/202406/bg2024062005.webp)

Bạn đọc có thể click để xem [ảnh độ phân giải cao](https://cdn.beekka.com/blogimg/asset/202406/bg2024062005.webp), nội dung tập trung vào các xu hướng công nghệ nổi bật và lĩnh vực tiên phong hiện nay. Dàn diễn giả quy tụ nhiều chuyên gia công nghệ và kỹ sư nòng cốt hàng đầu trên thế giới.

Ngoài ra, sự kiện tích hợp khu trải nghiệm AI ngoài sảnh với 4 khu vực hoạt động độc đáo, mang lại cơ hội giao lưu trực tiếp với các hãng công nghệ AI lớn trong nước và tham gia minigame nhận quà lưu niệm. Khu vực triển lãm này mở cửa hoàn toàn miễn phí.

Thông tin chi tiết về đại hội và đăng ký vé tham dự (vé nghe tham luận trong hội trường hoặc vé tham quan tự do ngoài sảnh) xin vui lòng truy cập [Website chính thức của sự kiện](https://conf.juejin.cn/xdc2024/?utm_source=ryf) hoặc quét mã QR trên poster.

## 科技动态

1、[Sự cố kỹ thuật của tàu vũ trụ Boeing Starliner](https://www.wsj.com/science/space-astronomy/boeing-sent-two-astronauts-into-space-now-it-needs-to-get-them-home-99d96633)

Cơ quan Hàng không Vũ trụ Mỹ (NASA) đang phải đối mặt với một tình huống tiến thoái lưỡng nan đầy thách thức.

Tàu vũ trụ Starliner của hãng Boeing (hình dưới) sau khi hoàn thành nhiệm vụ đưa hai phi hành gia lên Trạm Vũ trụ Quốc tế (ISS) hiện đang gặp sự cố và chưa thể đưa họ trở lại Trái Đất.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061906.webp)

Sau khi phóng, tàu vũ trụ được phát hiện gặp hiện tượng rò rỉ khí heli và lỗi hệ thống động cơ đẩy. Do chưa xác định được chính xác nguyên nhân gốc rễ, NASA chưa cho phép sử dụng con tàu này để thực hiện hành trình trở về nhằm đảm bảo an toàn tối đa cho phi hành đoàn.

Sứ mệnh ban đầu dự kiến kéo dài 8 ngày, hiện tại đã bước sang ngày thứ 20. Lịch trình trở về hiện được dời sang ngày 26 tháng 6 nhưng có khả năng sẽ tiếp tục bị hoãn.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061907.webp)

Rất may là trạm ISS luôn chuẩn bị sẵn lượng lương thực dự phòng đủ dùng cho 4 tháng nên sinh hoạt của các phi hành gia hoàn toàn không bị ảnh hưởng.

Đây là chuyến bay thử nghiệm chở người đầu tiên của dự án Starliner và đã gặp phải sự cố nghiêm trọng. Trong trường hợp xấu nhất, NASA sẽ phải điều động một tàu vũ trụ khác lên trạm để đón các phi hành gia trở về.

2、[Phát hiện khảo cổ về loài ngỗng khổng lồ đã tuyệt chủng tại Úc](https://www.nhm.ac.uk/discover/news/2024/june/face-ancient-australian-giga-goose-revealed-after-fossil-skull-found.html)

Do đặc thù địa lý biệt lập với các châu lục khác, nước Úc là ngôi nhà của nhiều loài động vật độc đáo.

Các nhà khoa học từ lâu đã biết đến sự tồn tại của một loài ngỗng khổng lồ cổ đại tại Úc (hình ngoài cùng bên phải), sở hữu kích thước tương đương chim đà điểu với chiều cao hơn 2 mét và trọng lượng đạt 240 kg, nhưng đã bị tuyệt chủng khoảng 45.000 năm trước.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061501.webp)

Mốc thời gian tuyệt chủng của chúng trùng khớp với thời điểm những nhóm người đầu tiên di cư đến định cư tại Úc, khiến các nhà khoa học suy đoán hoạt động săn bắt của con người là nguyên nhân chính dẫn đến sự biến mất của loài chim khổng lồ không biết bay và di chuyển chậm chạp này.

Trước đây, giới khảo cổ chỉ tìm thấy một vài mảnh xương hóa thạch rời rạc của loài ngỗng này, nhưng gần đây họ đã khai quật được mẫu hộp sọ hóa thạch hoàn chỉnh đầu tiên.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061502.webp)

Dựa trên hộp sọ này, các nhà nghiên cứu đã phục dựng lại hình ảnh chân thực của loài ngỗng khổng lồ cổ đại này.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061503.webp)

3、[Xu hướng theo dõi ánh mắt người dùng để ép xem quảng cáo trên thiết bị di động](https://x.com/soren_iverson/status/1801253187602788424)

Một người dùng mạng xã hội đã chia sẻ hình ảnh gây chú ý trên Twitter.

Khi đang xem video trên ứng dụng di động YouTube, màn hình bất ngờ hiển thị một thông báo cảnh báo.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061506.webp)

Nội dung thông báo chỉ ra hệ thống phát hiện mắt của người dùng không chú ý nhìn vào màn hình quảng cáo, do đó quảng cáo sẽ được tự động phát lại từ đầu.

Mặc dù bức ảnh chia sẻ này có thể chỉ là một tác phẩm thiết kế giả định, nhưng xét về mặt kỹ thuật, việc triển khai tính năng này hoàn toàn khả thi. Hệ thống chỉ cần kích hoạt camera trước khi phát quảng cáo để nhận diện sự hiện diện của khuôn mặt và hướng nhìn của ánh mắt người dùng.

Tôi lo ngại kịch bản này có thể trở thành sự thật trong tương lai gần. Khi đó, người dùng trả phí được trải nghiệm bình thường, còn người dùng miễn phí sẽ bị giám sát ánh mắt để đảm bảo họ thực sự xem hết nội dung quảng cáo.

4、[Giải pháp kết nối Internet sáng tạo bằng eSIM và giỏ treo tại dải Gaza](https://globalvoices.org/2024/06/13/the-ingenious-network-tree-defying-gazas-connectivity-blockade/)

Do ảnh hưởng trực tiếp từ chiến sự, toàn bộ hạ tầng mạng internet tại dải Gaza hiện đã bị phá hủy và ngắt kết nối hoàn toàn.

Một tổ chức nhân đạo quốc tế đã đề xuất một giải pháp sáng tạo giúp người dân tại đây kết nối với thế giới bên ngoài.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061504.webp)

Đầu tiên, họ thu mua một lượng lớn thẻ eSIM từ các quốc gia lân cận và gửi thông số kích hoạt kỹ thuật số cho người dân trong khu vực. Do eSIM là thẻ ảo, người dùng chỉ cần quét cấu hình là có thể kích hoạt dịch vụ rất dễ dàng.

Tiếp theo, người dân địa phương kết nối điện thoại với pin sạc dự phòng, đặt thiết bị vào một chiếc giỏ và treo lên các vị trí cao như ngọn cây gần khu vực biên giới.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061505.webp)

Thông qua eSIM, chiếc điện thoại treo cao có thể bắt được sóng mạng 4G từ các trạm phát sóng của quốc gia lân cận, sau đó phát Wi-Fi hotspot để người dân đứng bên dưới có thể truy cập mạng.

## Bài viết

1\. [Phân tích xu hướng phát triển chip AI: Tương lai chưa chắc đã thuộc về GPU](https://www.36kr.com/p/2826590796843272)（Tiếng Trung）

Bài viết phân tích nhận định rằng GPU không phải là giải pháp duy nhất cho nhu cầu tăng tốc điện toán AI, các kiến trúc chip chuyên dụng như FPGA hay ASIC hoàn toàn có thể là những lựa chọn tối ưu hơn ở lớp phần cứng.

2\. [Chia sẻ trải nghiệm 10 năm tự phát triển công cụ blog cá nhân](https://medium.com/@ideatocode/what-i-learned-as-an-artist-writing-my-own-blog-engine-for-10-years-straight-0cb8297e7712)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040801.webp)

Tác giả chia sẻ những bài học kinh nghiệm quý giá và trải nghiệm cá nhân sau chặng đường 10 năm kiên trì tự viết và vận hành công cụ blog engine riêng của mình.

3\. [Hướng dẫn tạo hiệu ứng gập trang 3D bằng CSS](https://www.joshwcomeau.com/react/folding-the-dom/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040601.webp)

Bài viết giới thiệu phương pháp khai thác các thuộc tính CSS nâng cao để tạo hiệu ứng hoạt họa gập trang 3D độc đáo cho giao diện web.

4\. [Tìm hiểu thuật toán tạo danh sách phát nhạc ngẫu nhiên của Spotify](https://pncnmnp.github.io/blogs/fibonacci-hashing.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121001.webp)

Bài viết phân tích chi tiết thuật toán trộn bài hát (shuffle) của Spotify, giải quyết bài toán phân bổ ngẫu nhiên sao cho các ca khúc của cùng một nghệ sĩ không bị phát liên tục.

5\. [Trải nghiệm tham quan trụ sở tập đoàn thiết bị bán dẫn ASML](https://www.asianometry.com/p/whats-next-for-asml)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061702.webp)

Tác giả chia sẻ những ghi nhận thực tế và góc nhìn thú vị khi đến tham quan trụ sở của gã khổng lồ chế tạo máy quang khắc ASML tại ngoại ô thành phố Eindhoven, Hà Lan.

6\. [Hướng dẫn tự viết 200 dòng JavaScript để xây dựng cơ chế Virtual DOM](https://lazamar.github.io/virtual-dom/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024052205.webp)

Virtual DOM là nền tảng cốt lõi của nhiều thư viện JavaScript hiện đại. Bài viết hướng dẫn chi tiết cách tự xây dựng cơ chế này từ con số không.

## 工具

1\. [Postgres.js (Thư viện kết nối cơ sở dữ liệu PostgreSQL tối ưu cho Node.js)](https://github.com/porsager/postgres)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101401.webp)

Bộ mã nguồn thư viện kết nối cơ sở dữ liệu PostgreSQL hiệu năng cao tương thích tốt cho cả môi trường Node.js và Deno. Bạn đọc có thể tham khảo thêm dự án tương tự [Zapatos](https://jawj.github.io/zapatos/).

2\. [OpenccLint (Công cụ hỗ trợ soát lỗi chuyển đổi chữ Hán giản thể và phồn thể)](https://opencclint.vercel.app/)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061601.webp)

Dự án phát triển dựa trên OpenCC giúp dịch và kiểm tra tính đồng bộ khi chuyển đổi văn bản chữ Hán giữa hai hệ Giản thể và Phồn thể, hỗ trợ giao diện web và dòng lệnh. (Đóng góp của [@hddhyq](https://github.com/ruanyf/weekly/issues/4629))

3\. [BiliVideoDown (Ứng dụng hỗ trợ tải video từ Bilibili phát triển bằng Flutter)](https://github.com/kangpeiqin/bilivideo_down)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061604.webp)

Công cụ máy tính mã nguồn mở hỗ trợ người dùng tải video chất lượng cao từ nền tảng Bilibili. (Đóng góp của [@kangpeiqin](https://github.com/ruanyf/weekly/issues/4640))

4\. [AQChat (Dự án xây dựng phòng chat trực tuyến ẩn danh)](https://gitee.com/howcode/aq-chat-server)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061605.webp)

Mã nguồn mở hỗ trợ xây dựng dịch vụ chat ẩn danh trực tuyến, cho phép tạo phòng, trao đổi tin nhắn và truyền tệp tin dễ dàng. Trải nghiệm bản dùng thử [Demo tại đây](https://aqchat.run/). Dự án cung cấp đầy đủ mã nguồn cho [Backend](https://gitee.com/howcode/aq-chat-server), [Web Frontend](https://gitee.com/howcode/aq-chat) và [Mobile Client](https://gitee.com/ghosthhf/aqchat-mobile). (Đóng góp của [@howcodes](https://github.com/ruanyf/weekly/issues/4643))

5\. [Voicer (Tiện ích hỗ trợ đọc thành tiếng nội dung trang web trên Chrome)](https://voicer.hellogeek.work/)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061808.webp)

Plugin trên trình duyệt giúp chuyển đổi văn bản trên trang web thành giọng đọc để người dùng theo dõi tiện lợi. (Đóng góp của [@wang-jianliang](https://github.com/ruanyf/weekly/issues/4647))

6\. [Dịch vụ tạo mã vạch trực tuyến Dịch Điều Hình](https://www.1txm.com/barcode)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061810.webp)

Công cụ web trực quan hỗ trợ người dùng nhanh chóng tạo ra các định dạng mã vạch thông dụng. (Đóng góp của [@FZliweiliang](https://github.com/ruanyf/weekly/issues/4651))

7\. [ScienHub (Trình soạn thảo LaTeX trực tuyến giàu mẫu thiết kế)](https://scienhub.com/templates)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061812.webp)

Dịch vụ web hỗ trợ biên tập mã nguồn tài liệu LaTeX trực tuyến đi kèm kho thư viện template báo cáo khoa học đa dạng. (Đóng góp của [@tc1989tc](https://github.com/ruanyf/weekly/issues/4657))

8\. [trash.sh (Giải pháp thay thế lệnh rm an toàn bằng cơ chế thùng rác)](https://github.com/qqAys/trash.sh)

Công cụ CLI đơn giản thay thế cho lệnh rm mặc định của Linux giúp di chuyển tệp tin cần xóa vào thư mục thùng rác tạm thời để tránh rủi ro mất dữ liệu. (Đóng góp của [@qqAys](https://github.com/ruanyf/weekly/issues/4658))

9\. [Ngã Đích Tự Thể (Công cụ tự thiết kế bộ font chữ viết tay cá nhân)](https://cloud.myfont.bid/)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061813.webp)

Dịch vụ trực tuyến giúp người dùng chuyển đổi các nét chữ viết tay cá nhân thành bộ font chữ kỹ thuật số hoàn chỉnh. (Đóng góp của [@harbor2009](https://github.com/ruanyf/weekly/issues/4659))

10\. [lingo link (Plugin hỗ trợ dịch thuật và đánh dấu từ vựng trực quan)](https://github.com/chengfengfengwang/lingo-link/blob/main/README_ZH-CN.md)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024062001.webp)

Tiện ích mở rộng nguồn mở trên trình duyệt hỗ trợ dịch thuật nhanh đoạn văn, ứng dụng AI giải nghĩa từ và đánh dấu từ mới để học tập. (Đóng góp của [@chengfengfengwang](https://github.com/ruanyf/weekly/issues/4670))

## AI 相关

1\. [Luma AI Video Generator (Trình tạo video nghệ thuật từ văn bản trực tuyến)](https://lunaai.video/)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061602.webp)

Dịch vụ web hỗ trợ trải nghiệm miễn phí công nghệ sinh video nghệ thuật từ câu lệnh mô tả văn bản của Luma AI. (Đóng góp của [@sunnyjingliu](https://github.com/ruanyf/weekly/issues/4628))

2\. [Stable Diffusion 3 AI Image Generator (Dịch vụ tạo ảnh vẽ trực tuyến miễn phí)](https://stablediffusion3.net/zh-CN)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061603.webp)

Trang web hỗ trợ người dùng trải nghiệm mô hình tạo ảnh vẽ nghệ thuật từ văn bản Stable Diffusion 3 miễn phí không cần đăng ký tài khoản. (Đóng góp của [@ddewfrefref](https://github.com/ruanyf/weekly/issues/4637))

3\. [Generative Voice AI (Dịch vụ chuyển đổi văn bản thành giọng nói chất lượng cao)](https://elevenlabs.io/)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101615.webp)

Dịch vụ chuyển đổi văn bản thành giọng nói (TTS) chất lượng cao hỗ trợ tốt tiếng Việt. Tài khoản miễn phí được cung cấp hạn mức 10.000 ký tự mỗi tháng (tương đương khoảng 10 phút âm thanh).

4\. [BrainyAI (Plugin tích hợp đa mô hình AI cho thanh bên trình duyệt)](https://github.com/luyu0279/BrainyAI)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061809.webp)

Plugin trình duyệt mã nguồn mở hỗ trợ gọi nhanh các mô hình AI thông dụng ở thanh bên màn hình, đóng vai trò giải pháp thay thế miễn phí cho các công cụ trả phí như Sider AI, Monica, Merlin hay MaxAI. (Đóng góp của [@luyu0279](https://github.com/ruanyf/weekly/issues/4648))

5\. [Rock AI (Trang chạy thử nghiệm trực tuyến các mô hình AI nguồn mở)](https://www.rockai.online/)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061908.webp)

Nền tảng chia sẻ trực tuyến hỗ trợ chạy thử nghiệm nhanh nhiều mô hình AI nguồn mở hữu ích. (Đóng góp của [@hellokidder](https://github.com/ruanyf/weekly/issues/4668))

6\. [Chrome AI (Ứng dụng chat cục bộ khai thác Gemini Nano tích hợp sẵn)](https://chrome-ai.cc/)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061811.webp)

Công cụ hỗ trợ người dùng trò chuyện trực tiếp với mô hình Gemini Nano chạy ngoại tuyến tích hợp sẵn trên trình duyệt Chrome. (Đóng góp của [@zengkan0703](https://github.com/ruanyf/weekly/issues/4655))

7\. [Giải pháp xây dựng công cụ tóm tắt nội dung trang web cục bộ trên macOS](https://www.sheshbabu.com/posts/system-wide-text-summarization-using-ollama-and-applescript/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061512.webp)

Bài viết hướng dẫn phương pháp cài đặt mô hình ngôn ngữ lớn cục bộ bằng Ollama trên macOS kết hợp AppleScript để tạo phím tắt tự động tóm tắt nội dung của trang web đang mở.

## 资源

1\. [Những kiến thức cơ bản về chuẩn Unicode mà lập trình viên cần nắm vững](https://tonsky.me/blog/unicode/)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100210.webp)

Bài phân tích chi tiết cập nhật các kiến thức quan trạng và nguyên lý hoạt động của chuẩn mã hóa ký tự Unicode thế hệ mới.

2\. [loadership (Thư viện tùy biến hiệu ứng tải trang bằng thuần CSS)](https://www.loadership.com/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024012002.webp)

Trang web cung cấp công cụ trực quan giúp lập trình viên tùy chỉnh cấu hình và tải về các đoạn mã hiệu ứng chuyển động tải trang (loaders) viết hoàn toàn bằng CSS.

3\. [Giáo trình tự học ngôn ngữ lập trình C++ hiện đại Modern C++ Programming](https://github.com/federico-busato/Modern-CPP-Programming)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112902.webp)

Tài liệu học tập mã nguồn mở chia sẻ các kiến thức và kỹ thuật viết code tối ưu bằng ngôn ngữ C++ hiện đại.

## 图片

1\. [Nút giao vòng xuyến giao thông Magic Roundabout độc đáo tại Anh](https://www.snopes.com/fact-check/magic-roundabout-photo/)

Thành phố Swindon của Anh sở hữu một nút giao vòng xuyến vô cùng phức tạp, được phân tách rõ rệt thành vòng xuyến đồng tâm phía trong và vòng xuyến phía ngoài đi kèm 5 vòng xuyến nhỏ vệ tinh xung quanh.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061703.webp)

Cơ chế vận hành quy định luồng phương tiện di chuyển ở vòng xuyến đồng tâm phía trong chạy theo chiều ngược chiều kim đồng hồ, trong khi luồng xe ở vòng xuyến phía ngoài chạy theo chiều thuận chiều kim đồng hồ.

Để di chuyển chuyển đổi qua lại giữa vòng xuyến trong và ngoài, các phương tiện bắt buộc phải đi qua hệ thống 5 vòng xuyến nhỏ vệ tinh.

Dưới đây là hình ảnh biển báo chỉ dẫn giao thông lắp đặt tại thực địa.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024061704.webp)

Nút giao thông đặc biệt này được đưa vào sử dụng từ năm 1972 và số liệu thống kê thực tế cho thấy tỷ lệ xảy ra tai nạn nghiêm trọng tại đây ở mức cực kỳ thấp.

2\. [Công trình đường hầm giao thông dưới lòng sông Elbe cổ đại](https://en.wikipedia.org/wiki/Elbe_Tunnel_(1911))

Dòng sông Elbe chảy qua khu vực trung tâm thành phố Hamburg, Đức.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101409.webp)

Vào năm 1911, chính quyền thành phố Hamburg đã hoàn thành xây dựng đường hầm dài 426 mét chạy dưới lòng sông giúp kết nối giao thương giữa hai bờ.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101410.webp)

Điểm đặc biệt của công trình là đường hầm hoàn toàn không thiết kế lối đường dẫn thoải lên xuống. Người đi bộ và phương tiện giao thông muốn tiếp cận hoặc rời đường hầm bắt buộc phải di chuyển bằng các buồng nâng thang máy khổng lồ đặt thẳng đứng ở hai đầu cầu (vùng màu vàng trên bản vẽ phác thảo).

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101412.webp)

Hình ảnh lối vào hệ thống thang máy chuyên dụng dành cho các phương tiện ô tô.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101411.webp)

Công trình lịch sử này vẫn tiếp tục duy trì hoạt động phục vụ người dân cho đến tận ngày nay, thậm chí thỉnh thoảng lòng đường hầm còn được trưng dụng làm không gian tổ chức các buổi hòa nhạc nghệ thuật. Dưới đây là góc nhìn từ đáy buồng thang máy hướng lên lối ra phía trên.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101413.webp)

## ✍️ Bài đọc thêm

### Quy mô thiết kế tối ưu của một ngôn ngữ lập trình

Quy mô thiết kế của các ngôn ngữ lập trình hiện nay rất đa dạng.

Một số ngôn ngữ ưu tiên sự tối giản tuyệt đối, chỉ cung cấp các cú pháp cốt lõi nhất. Ngược lại, một số ngôn ngữ cố gắng tích hợp toàn bộ các tính năng hỗ trợ đa dạng nhu cầu.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024062002.webp)

Bên cạnh đó, có những ngôn ngữ ban đầu được thiết kế rất tinh gọn nhưng trải qua quá trình phát triển liên tục đắp thêm tính năng mới khiến chúng trở nên cồng kềnh, phức tạp và gây khó khăn cho người học.

Phiên bản đầu tiên của Python được thiết kế rất nhỏ gọn, và định hướng này được duy trì nghiêm túc qua các phiên bản đầu tiên. Ban phát triển ban đầu kiên quyết từ chối nhiều đề xuất bổ sung tính năng mới với lập luận giữ cho ngôn ngữ không bị phình to.

Tuy nhiên tại một thời điểm bước ngoặt (khoảng giữa giai đoạn phát triển từ Python 1.6 lên Python 2.0), định hướng thiết kế đã có sự thay đổi lớn: các đề xuất bổ sung tính năng sẽ không bị loại bỏ chỉ vì lý do làm ngôn ngữ phình to nữa, mà chỉ bị từ chối nếu tính năng đó không thực sự giải quyết được một bài toán kỹ thuật thực tế quan trọng.

Kể từ cột mốc đó, Python chính thức bước vào hành trình trở thành một ngôn ngữ khổng lồ.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024062003.webp)

Theo quan điểm cá nhân tôi, một khi đội ngũ thiết kế không còn đặt rào cản kiểm soát quy mô của ngôn ngữ, sự phình to vô hạn của ngôn ngữ đó là điều tất yếu sẽ xảy ra.

Kịch bản tương tự cũng diễn ra với nhiều ngôn ngữ khác. Mặc dù Java chưa bao giờ được coi là một ngôn ngữ gọn nhẹ, nhưng trước khi tính năng Generic được đưa vào phiên bản Java 1.5, cấu trúc của nó thay đổi khá chậm rãi. Sự ra đời của Generic dường như là điểm khởi đầu cho hành trình phình to quy mô của Java.

Tương tự, JavaScript vốn ban đầu là một ngôn ngữ tối giản được thiết kế thần tốc chỉ trong vòng một tuần, hiện nay cũng đã trở thành một hệ sinh thái ngôn ngữ vô cùng đồ sộ.

Ngôn ngữ Rust dù hiện tại đã sở hữu quy mô rất lớn nhưng các cuộc thảo luận phát triển vẫn đang liên tục cân nhắc bổ sung thêm nhiều tính năng mới.

Tại sao hầu hết các ngôn ngữ lập trình đều không thể tránh khỏi xu hướng ngày càng phình to?

Lý do cốt lõi là không có bất kỳ một ngôn ngữ lập trình nào đạt đến trạng thái hoàn hảo tuyệt đối, luôn tồn tại những kịch bản sử dụng (use cases) mà ngôn ngữ đó chưa thể hỗ trợ tối ưu. Trong nhiều trường hợp, việc bổ sung cú pháp hay tính năng mới là giải pháp trực quan nhất để giải quyết bài toán đó.

Và do các kịch bản ứng dụng trong thực tế phát triển phần mềm là vô hạn, đội ngũ thiết kế sẽ luôn tìm ra lý do để bổ sung thêm tính năng mới nhằm giúp ngôn ngữ "tốt hơn", và hệ quả tất yếu đi kèm là khiến ngôn ngữ ngày một đồ sộ hơn.

## Lịch sử tuần này

- 2023年（第 258 期）：[Góc nhìn công nghệ: Bài học kinh nghiệm và góc nhìn thú vị từ chia sẻ của huyền thoại John Carmack về chú mèo cưng](https://www.ruanyifeng.com/blog/2023/06/weekly-issue-258.html)
- 2022年（第 208 期）：[Tư duy quản trị: Phân tích những mặt trái và hạn chế của cơ chế thăng tiến nhân sự truyền thống trong doanh nghiệp](https://www.ruanyifeng.com/blog/2022/05/weekly-issue-208.html)
- 2021年（第 158 期）：[Xu hướng thị trường: Nhận định về thực trạng mất giá và bão hòa của các kênh phân phối nội dung trực tuyến](https://www.ruanyifeng.com/blog/2021/05/weekly-issue-158.html)
- 2020年（第 108 期）：[Tư duy chiến lược: Phân tích sự khác biệt và nguyên lý áp dụng giữa hai mô hình trận địa chiến và tập kích chiến trong kinh doanh](http://www.ruanyifeng.com/blog/2020/05/weekly-issue-108.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
