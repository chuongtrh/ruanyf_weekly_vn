# Bản tin công nghệ hàng tuần (Số 416): Lập trình đã hoàn toàn thay đổi diện mạo

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/12009) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102201.webp)

Không gian nội thất của Nhà hát Lớn Thượng Hải vừa được đưa vào sử dụng trong tuần này. ([via](http://sh.news.cn/20261022/b4bc8ab8a9e848f7aa8d044ba56487cc/c.html))

## 编程已经面目全非

Đa số mọi người chỉ nhìn thấy AI làm thay đổi nghề lập trình viên. Rất hiếm người đề cập đến việc: AI cũng đã thay đổi hoàn toàn bản thân công việc lập trình.

AI đã lật đổ phương thức phát triển phần mềm truyền thống; việc lập trình giờ đây đã hoàn toàn đổi khác, không còn nhận ra diện mạo thuở ban đầu.

Ngay cả khi bong bóng định giá trong tương lai có vỡ vụn, AI cũng không bao giờ biến mất khỏi chuỗi công cụ lập trình, nó đã vĩnh viễn trở thành một phần không thể tách rời của quy trình phát triển phần mềm.

Một lập trình viên kỳ cựu nước ngoài đã [đúc kết](https://x.com/thorstenball/status/2101305394190557466) những phương diện mà AI đã làm thay đổi việc lập trình.

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101515.webp)

Quan điểm của anh rất cấp tiến với nhiều khẳng định táo bạo, tôi thấy rất đáng để chia sẻ rộng rãi tới mọi người:

**（1）Quy trình đánh giá mã nguồn (Code review) sẽ biến mất.**
Con người review code thủ công giờ đây không còn ý nghĩa gì nữa. Bởi vì tốc độ của con người không thể nào bắt kịp tốc độ sinh code của AI, và cũng không thể trong một khoảng thời gian hợp lý phát hiện ra bug ẩn sâu trong đống code khổng lồ của AI.
Trong tương lai con người chỉ thẩm định xem cấu trúc tổng thể và kiến trúc hệ thống có hợp lý hay không, chứ tuyệt đối không bao giờ ngồi dò từng dòng code qua Pull Request như hiện nay.

**（2）Kiểm thử đơn vị (Unit test) có thể sẽ biến mất.**
AI có thể viết lại toàn bộ cách triển khai của đoạn code bất cứ lúc nào, việc đi kiểm thử từng đơn vị code nhỏ lẻ vì thế trở nên vô nghĩa. Có thể ngay lần lặp tiếp theo cả tòa nhà sẽ được đập đi xây mới hoàn toàn, việc gì phải mất công đi săm soi từng viên gạch.
Các dự án tương lai có lẽ sẽ chỉ giữ lại kiểm thử giao diện (interface test), kiểm thử tích hợp (integration test) và kiểm thử toàn hệ thống (system test), chứ không duy trì unit test nữa.

**（3）Trọng tâm phát triển phần mềm không còn nằm ở việc gõ code.**
Code trong tương lai do AI gánh vác, trọng tâm của lập trình viên sẽ dịch chuyển sang các khâu ngoài mã nguồn: dùng phần mềm giải quyết bài toán kinh doanh như thế nào, hiểu phần mềm hiện thực hóa ra sao, phát hành thế nào và thu thập phản hồi của người dùng ra sao.

**（4）Bản chất của Bug cũng đã thay đổi.**
Đa số bug phát sinh không còn là bug cú pháp hay thuật toán trong code, mà là do việc đặt yêu cầu nghiệp vụ bị sai hoặc diễn đạt thiếu chuẩn xác.

**（5）Mã nguồn mở không còn là yếu tố nâng cao chất lượng phần mềm.**
Trước đây, một lý do để mở mã nguồn là "chỉ cần đủ nhiều người để mắt tới thì mọi lỗi lầm đều sẽ bị phát hiện".
Câu nói này ngày nay vẫn đúng, nhưng khác ở chỗ: giờ đây ngay cả khi bạn không mở mã nguồn, AI vẫn có thể thừa sức giúp bạn dò ra toàn bộ bug.

**（6）Lập trình linh hoạt (Agile) sẽ cáo chung.**
Các phương pháp luận của Agile hay Scrum không còn nhiều ý nghĩa thực tế; tốc độ sinh mã của AI quyết định thời gian hoàn thành dự án, tất cả những gì bạn cần làm là đẩy thẳng phiếu yêu cầu (ticket/issue) cho AI xử lý.

**（7）Phân công vai trò trong dự án sẽ biến chuyển.**
Trước đây một đội ngũ phát triển thường có ba vai trò trụ cột: Quản lý sản phẩm (PM), Nhà thiết kế (Designer) và Kỹ sư lập trình (Engineer).
Sau này cấu trúc kiềng ba chân này sẽ tan biến. Với sự trợ giúp của AI, một người duy nhất có thể kiêm nhiệm trọn vẹn cả ba vai trò.

**（8）Khái niệm "Code đẹp" sẽ không còn tồn tại.**
Trước kia, chuẩn mực của một đoạn code đẹp là dễ đọc hiểu đối với con người, thuận tiện tái cấu trúc (refactor) và có chi phí bảo trì thấp.
Thế nhưng giờ đây khi bạn không còn trực tiếp đọc, sửa đổi và bảo trì phần lớn code nữa, tiền đề tồn tại của khái niệm "code đẹp" cũng tự khắc biến mất.

**（9）Quy chuẩn định dạng code và công cụ Linter cũng không còn nhiều ý nghĩa.**
AI có bao giờ bận tâm xem mỗi dòng code có vượt quá 80 ký tự hay không, có thụt đầu dòng bằng phím Tab hay Space không, hay dòng cuối có ký tự xuống dòng hay không...?

**（10）Giao diện người dùng (UI) sẽ giảm dần tầm quan trọng.**
Một mặt, rất nhiều UI trong tương lai sinh ra là để cho các AI Agent sử dụng, mà Agent thì chỉ cần API chứ không cần giao diện trau chuốt màu mè.
Mặt khác, nếu tốc độ sinh code diễn ra tức thì, thì UI sẽ được render động theo thời gian thực. Rất nhiều UI hiện tại sinh ra chỉ vì phần mềm không biết chính xác bạn muốn gì — menu, trang cài đặt, dashboard, bộ lọc sinh ra là để giúp người dùng lần mò ra nhu cầu. Khi người dùng diễn đạt rõ mong muốn bằng ngôn ngữ tự nhiên, AI có thể sinh ra ngay một UI tùy biến tức thời phục vụ đúng nhu cầu đó.

**（11）Token là vua.**
Bên nào kham nổi lượng Token lớn hơn, bên đó sẽ tạo ra phần mềm vượt trội hơn. Nếu không có đủ Token dồi dào, bạn sẽ không thể nào phát triển được những phần mềm xuất sắc nhất.

## 大模型的区别对待

Tuần này, một công ty AI của Mỹ đã đăng một [bài viết](https://www.hirundo.io/blog/qwen3-coder-vulnerabilities) gây giật gân trên trang web của họ.

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102204.webp)

Họ tuyên bố rằng mô hình Qwen3-Coder có hành vi phân biệt đối xử với người dùng: nếu người dùng khai báo mình là "nhà thầu quốc phòng của Mỹ", mô hình sẽ cố tình sinh ra code chất lượng kém với nhiều lỗ hổng bảo mật hơn.

Ngược lại, nếu người dùng khai mình là doanh nghiệp Trung Quốc, mô hình sẽ sinh ra code có chất lượng cao vượt trội.

Đọc xong tôi thực sự bật cười vì ngán ngẩm, đúng là để tạt nước bẩn thì người ta sẵn sàng thêu dệt nên bất cứ điều gì. Một khi đã tin vào thuyết âm mưu thì nhìn đâu cũng thấy âm mưu.

Chưa bàn tới việc phương pháp kiểm thử có khách quan hay không, chỉ riêng việc họ chọn mô hình Qwen3-Coder-30B-A3B-Instruct để thử nghiệm đã thấy có vấn đề lớn.

Đây là mô hình đã phát hành từ tận ngày 31 tháng 7 năm 2025, từ lâu đã lỗi thời. Hơn nữa số tham số kích hoạt của nó chỉ vỏn vẹn 3.3B, ai lại đi dùng một mô hình tí hon như vậy để sinh code trong môi trường sản xuất thực tế?

Nếu thực sự muốn ngấm ngầm cài cắm cửa sau hay lỗ hổng, chẳng phải người ta nên can thiệp vào các mô hình cao cấp hàng đầu hay sao? Bởi các mô hình cao cấp mới là thứ được các tập đoàn lớn trọng yếu đưa vào ứng dụng.

Công ty Mỹ này hoàn toàn không đưa ra được lời giải thích thỏa đáng vì sao lại chọn duy nhất Qwen3-Coder-30B-A3B-Instruct làm ví dụ mà không thử nghiệm trên các mô hình Trung Quốc khác.

Nực cười nhất là sản phẩm mà công ty này đang chào bán chính là phiên bản "đã qua xử lý an toàn hóa" của chính mô hình Qwen3-Coder-30B-A3B-Instruct! Vừa lu loa rằng mô hình Trung Quốc nguy hiểm, vừa chào mời khách hàng mua bản sửa đổi của chính mô hình đó, tôi không hiểu vị khách hàng nào có thể ngây thơ bỏ tiền ra mua sản phẩm của họ.

Mặc dù bài viết đó thuần túy là một trò hề thương mại, nhưng câu hỏi liệu mô hình lớn có phân biệt đối xử với người dùng hay không lại là một vấn đề nghiêm túc cần được mổ xẻ.

Liệu một mô hình có thực sự nhắm vào nhóm người dùng cụ thể để trả về kết quả định hướng riêng (thuật ngữ máy tính gọi là "honeypot") hay không?

Nếu điều này thực sự có thể xảy ra, điều đó đồng nghĩa với việc người dùng buộc phải mặc định coi mọi mô hình đều không đáng tin cậy tuyệt đối, và bắt buộc phải dùng thêm các mô hình độc lập khác để thẩm định chéo kết quả sinh ra.

## 印度的证书颁发机构

Tuần này còn diễn ra một sự việc bi hài không kém.

eMudhra — một tổ chức cấp chứng chỉ số (CA) tại Ấn Độ — vừa bị [bẻ khóa toàn bộ khóa riêng tư (private key)](https://scotthelme.co.uk/eight-bits-of-trust-emudhras-ca-keys-cracked-in-milliseconds/). Bất kỳ ai giờ đây cũng có thể dùng private key của họ để tự ký phát chứng chỉ bảo mật.

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102205.webp)

Khác xa với những gì mọi người mường tượng, việc bẻ khóa private key của tổ chức này hoàn toàn không liên quan đến kỹ thuật hack siêu đẳng hay cần đến năng lực tính toán siêu máy tính khổng lồ. Bởi vì một trong các private key của họ chỉ là con số... 4, và hai private key khác lần lượt là 56 và 115!

Có tổng cộng 8 private key bị bẻ khóa, toàn bộ đều là những số nguyên nhỏ hơn 255.

Theo đúng nguyên tắc mật mã học, private key bắt buộc phải là một số ngẫu nhiên cực lớn; thế nhưng công ty này lại điền toàn bộ các byte đầu của khóa bằng số 0, chỉ để lại duy nhất byte cuối cùng là một giá trị khác 0, hệt như bức hình dưới đây:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102206.webp)

Do đó việc bẻ khóa diễn ra dễ như trở bàn tay, chỉ mất đúng 1 phần nghìn giây (1ms) tính toán là xong.

Hiện tại các trình duyệt lớn như Chrome, Mozilla Firefox đã phải cấp tốc tung ra bản cập nhật khẩn cấp thu hồi chứng chỉ gốc và chấm dứt mọi sự tin cậy đối với các chứng chỉ do eMudhra cấp phát.

Phong cách làm việc của các công ty công nghệ Ấn Độ quả thực luôn khiến người ta phải ngỡ ngàng.

## 文章

1. [Bức tranh toàn cảnh về mô hình lớn năm 2026](https://simonwillison.net/2026/Sep/27/2026-in-llms-so-far/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102119.webp)

Bài thuyết trình của lập trình viên danh tiếng Simon Willison tổng kết những bước tiến lớn của AI trong năm nay qua các từ khóa: OpenClaw, Tokenmaxxing, Claude Fable 5 / Mythos, Local model và sự cố Hugging Face.

2. [Cuộc chiến giữa Terence Tao và làn sóng AI](https://archive.ph/uaQ4X) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102103.webp)

Bài phóng sự dài kỳ của *The New York Times*: nhà toán học lừng danh Terence Tao công khai phản đối việc các công ty AI bừa bãi dùng mô hình lớn để tự động hóa chứng minh hàng loạt bài toán khó, vì ông cho rằng điều đó chẳng giúp ích gì cho nhận thức và tư duy toán học đích thực của nhân loại.

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102104.webp)

Bài báo cũng điểm lại cuộc đời rực rỡ của ông: bức ảnh trên chụp ông năm 13 tuổi (1988) khi giành huy chương vàng Olympic Toán quốc tế; năm 24 tuổi ông trở thành giáo sư thực thụ trọn đời tại UCLA (hình dưới là bài giảng đại chúng năm 2007).

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102105.webp)

3. [11 dịch vụ tôi tự lưu trữ tại nhà](https://viceconsole.fyi/blog/2026/10/10/what-i-self-host/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101501.webp)

Tác giả cho chạy 17 dịch vụ native và 11 container Podman ngay trên một chiếc máy tính mini PC 16GB RAM tại nhà, chia sẻ kinh nghiệm vận hành thực tế.

4. [Ví phần cứng là gì?](https://decrypt.co/resources/what-is-a-hardware-wallet-crypto-cold-storage-explained) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101805.webp)

Bài viết giải thích khái niệm ví lạnh phần cứng trong tiền mã hóa, tác dụng bảo mật và phân tích hai vụ việc ví phần cứng bị giải mã tấn công vật lý gần đây.

5. [Tôi huấn luyện mô hình 360M tham số để giả lập terminal](https://simedw.com/2026/10/21/world-model-terminal/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102202.webp)

Tác giả chia sẻ cách anh dựa trên Qwen2.5-Coder-0.5B để huấn luyện một mô hình nhỏ với 2 tỷ token trong 75 giờ GPU RTX 4090.
Điều thú vị nhất là công năng của mô hình: nó giả lập giao diện terminal. Mỗi khi người dùng gõ lệnh, mô hình không hề thực thi lệnh đó mà chỉ dự đoán kết quả đầu ra rồi hiển thị lên màn hình. Ý tưởng vô cùng độc đáo: mô hình không làm việc thật nhưng tạo cảm giác như công việc đã được hoàn thành trơn tru.

6. [NVIDIA nợ tôi 1 tỷ USD cổ phiếu](https://colo.to/nvidia-stock-narrative.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102118.webp)

Bài hồi ký thú vị: cách đây 30 năm NVIDIA đồng ý cấp cho tác giả một lượng quyền chọn cổ phiếu, thời điểm đó NVIDIA chỉ là một công ty khởi nghiệp tí hon sắp phá sản nên quyền chọn chẳng có giá trị gì. Tác giả quên bẵng đi; 30 năm sau nhớ ra thì số cổ phiếu đó trị giá hơn 1 tỷ USD, tiếc là thời hiệu khởi kiện đã hết nên tòa án bác đơn.

## 工具

1. [sslx](https://github.com/glincker/sslx)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101806.webp)

Công cụ dòng lệnh kiểm tra và xem thông tin chứng chỉ HTTPS nhanh gọn.

2. [Mac.apk](https://github.com/kksimp/Mac.apk)

Chạy ứng dụng Android trực tiếp trên Mac mà không cần máy ảo hay trình giả lập, bằng cách mô phỏng trực tiếp hệ thống API của Android.

3. [siltop](https://github.com/CLoaKY233/siltop)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102110.webp)

Công cụ dòng lệnh macOS hiển thị thông số hệ thống thời gian thực trong terminal: CPU, GPU, RAM, pin, nhiệt độ, ổ cứng, mạng...

4. [Little Snitch Mini](https://obdev.at/products/littlesnitch-mini/index.html)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071301.webp)

Phần mềm macOS hiển thị toàn bộ kết nối Internet của các ứng dụng đang chạy và cho phép chặn đứng các kết nối đáng ngờ.

5. [Pines](https://github.com/thedevdojo/pines)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071307.webp)

Thư viện thành phần UI xây dựng trên nền Tailwind CSS và Alpine.js.

6. [silkpulse](https://github.com/2234839/silkpulse)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101901.webp)

Công cụ debug trang web từ xa: nhúng một script vào trang là có thể mở console từ xa xem log và bắt lỗi thời gian thực, rất tiện để debug trên thiết bị di động. (Đóng góp từ [@2234839](https://github.com/ruanyf/weekly/issues/12383))

7. [TaskbarLyrics](https://github.com/ANYNC/TaskbarLyrics)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101903.webp)

Hiển thị lời bài hát trực tiếp trên thanh Taskbar của Windows theo thời gian thực. (Đóng góp từ [@ANYNC](https://github.com/ruanyf/weekly/issues/12408))

8. [Archify](https://github.com/tt-a1i/archify)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101905.webp)

Skill biến một đoạn mô tả, kế hoạch hoặc một kho mã nguồn thành sơ đồ luồng tương tác sinh động trên nền web. (Đóng góp từ [@zhengxin-wang](https://github.com/ruanyf/weekly/issues/12423))

9. [html-to-video](https://github.com/wx4766/html-to-video)

Công cụ dòng lệnh render các hiệu ứng hoạt họa HTML từng khung hình thành video MP4. (Đóng góp từ [@wx4766](https://github.com/ruanyf/weekly/issues/12486))

10. [Parcel](https://github.com/hyphy-void/Parcel)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026102101.webp)

Ứng dụng chia sẻ file tạm thời chạy trên Cloudflare Workers: tạo link mã hóa sau khi upload, tự động hủy file khi hết hạn. (Đóng góp từ [@hyphy-void](https://github.com/ruanyf/weekly/issues/12598))

11. [douban-cli](https://github.com/Marvae/douban-cli)

Client dòng lệnh lấy thông tin dữ liệu phim ảnh, sách truyện trên Douban. (Đóng góp từ [@Marvae](https://github.com/ruanyf/weekly/issues/12616))

12. [wol](https://github.com/Trugamr/wol)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025012509.webp)

Công cụ dòng lệnh và giao diện web hỗ trợ tính năng Wake-on-LAN để đánh thức các máy tính đang ngủ trong mạng nội bộ.

## 资源

1. [Thư pháp Đại Bằng](https://zidian.dapengshufa.com/)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101902.webp)

Tra cứu các kiểu chữ thư pháp đa dạng của từng chữ Hán. (Đóng góp từ [@gengdapeng-beep](https://github.com/ruanyf/weekly/issues/12402))

2. [Học Vim đúng cách](https://github.com/iggredible/Learn-Vim) (Learn Vim the Smart Way)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110605.webp)

Giáo trình học trình biên tập Vim mã nguồn mở chất lượng cao.

3. [Nhập môn thiết kế trình biên dịch và ngôn ngữ](https://dthain.github.io/books/compiler/) (Introduction to Compilers and Language Design)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026070703.webp)

Sách giáo khoa tiếng Anh miễn phí dành cho người mới bắt đầu, giới thiệu các khái niệm biên dịch và cách tự viết một trình biên dịch C.

## 图片

1. [Biển chỉ dẫn đường bộ tại Pháp](https://www.bbc.com/travel/article/20260327-the-road-signs-that-teach-travellers-about-france)

Biển báo trên các tuyến cao tốc ở Pháp không chỉ để chỉ đường, mà còn giới thiệu ẩm thực, danh lam thắng cảnh và làng cổ địa phương.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026033109.webp)

Biển báo trên biểu thị phía trước là công viên chim nước.

Những biển báo này được thiết kế để thu hút ánh nhìn của tài xế chỉ trong vài giây: biểu tượng đồ họa tối giản, tên địa danh rõ ràng với hai tông màu nâu trắng thanh lịch.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026033110.webp)

Biển báo trên báo hiệu phía trước có một tòa lâu đài cổ trứ danh.

Hình dưới là biển báo thành phố cảng Saint-Malo với tường thành cổ kính, thuyền buồm và những ngọn sóng cuộn trào:

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026033111.webp)

Một số biển báo còn khắc họa chân dung các danh nhân lịch sử địa phương:

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026033112.webp)

Bức hình trên là đài tưởng niệm chiến tranh dành cho những trẻ em địa phương thiệt mạng trong Thế chiến II.

## 文摘

1. [Vì sao nheo mắt lại nhìn rõ hơn?](https://www.mentalfloss.com/posts/why-does-squinting-help-you-see-better)

Tất cả chúng ta đều từng trải qua cảm giác này: khi khó nhìn rõ một vật ở xa, chỉ cần nheo mắt lại là độ nét dường như được cải thiện đáng kể.

Nghĩ kỹ thì điều này có vẻ ngược đời: nheo mắt làm giảm diện tích tiếp nhận ánh sáng của mắt, tại sao lại nhìn rõ hơn?

![](https://cdn.beekka.com/blogimg/asset/202606/bg2026062510.webp)

Bạn có thể lầm tưởng rằng điều này liên quan đến áp lực lên mắt, rằng nheo mắt sẽ "bóp nhẹ nhãn cầu" làm thay đổi tiêu cự của thủy tinh thể. Suy nghĩ đó hoàn toàn sai lầm.

Tác dụng thực sự của việc nheo mắt là giảm bớt lượng ánh sáng đi vào mắt. Khi nheo mắt, bạn thực chất đang thu nhỏ đồng tử ngoại vi, ngăn chặn các tia sáng ngoại biên gây nhiễu và chỉ cho phép những chùm tia sáng đi qua vùng trung tâm của nhãn cầu chiếu thẳng vào võng mạc, giúp hình ảnh hội tụ sắc nét hơn. Đây chính là "hiệu ứng lỗ kim" (pinhole effect) — nguyên nhân cốt lõi giúp bạn nhìn rõ hơn.

Mặt tiêu cực của việc nheo mắt là nó làm giảm tần suất chớp mắt. Do đó nếu nheo mắt quá lâu (chẳng hạn nheo mắt nhìn màn hình máy tính cả ngày) sẽ dẫn đến mỏi mắt và khô mắt.

Ngược lại với một số quan niệm sai lầm, nheo mắt không làm suy giảm thị lực của bạn. Nó không phải nguyên nhân gây giảm thị lực mà là triệu chứng báo hiệu thị lực đang suy giảm. Nếu lúc nào bạn cũng phải nheo mắt mới nhìn rõ thì đã đến lúc bạn nên đi đo kính khám mắt.

## 言论

1.

Có người hỏi: "Code do AI viết tôi hoàn toàn không hiểu nổi, nhưng công ty bắt tôi phải deploy lên môi trường production, tôi phải làm sao?"
Câu trả lời của tôi là: Đừng để AI thiết kế kiến trúc code, mà hãy để nó hiện thực hóa phần code mà bạn đã tự tay thiết kế tỉ mỉ từ trước.

-- [Độc giả Hacker News](https://news.ycombinator.com/item?id=50157475)

2.

Hầu hết mọi lời khuyên chỉ đúng với chính người đưa ra lời khuyên đó, chứ chưa chắc đã đúng với người khác.

-- [coached.com](https://coached.com/essays/most-advice-is-right-for-the-person-giving-it/)

3.

AI giúp việc khởi nghiệp một mình (solopreneur) trở nên dễ dàng hơn bao giờ hết, và nguyên nhân thất bại hàng đầu của các nhà sáng lập đơn độc trong tương lai sẽ là sự cô đơn.
Xung quanh bạn không còn ai phản biện lại ý tưởng, không ai nhận ra những bế tắc bạn đang đối mặt, và không ai ở bên động viên bạn kiên trì đến cùng. AI có thể giúp bạn tiến nhanh hơn, nhưng nó không bao giờ có thể thay thế được nhu cầu tâm sự hay chia sẻ niềm vui giữa con người với con người.

-- [《Sau tự động hóa, khởi nghiệp đơn độc sẽ trở thành xu thế chủ đạo》](https://every.to/thesis-statements/julian-weisser)

4.

Mối bận tâm hàng đầu của chính phủ Mỹ hiện nay đã chuyển thành việc làm sao duy trì lợi thế dẫn đầu công nghệ trước Trung Quốc, và tìm mọi cách neo giữ mức định giá cao ngất ngưởng của thị trường chứng khoán Mỹ.

-- [Tạp chí *The Economist*](https://www.economist.com/business/2026/09/30/the-era-of-speedball-capitalism-has-dawned)

5.

Mấy tháng qua OpenAI đã công bố hàng trăm bản chứng minh toán học do AI giải quyết. Giới toán học bàng hoàng chấn động, một nhà toán học thừa nhận ông đã bật khóc vì cảm thấy AI đang hủy diệt lĩnh vực nghiên cứu cả đời của mình.
Một người theo chủ nghĩa lạc quan công nghệ có lẽ sẽ không nghĩ như vậy, anh ta sẽ khuyên nhà toán học hãy vực dậy tinh thần:
Toán học không bận tâm đến cảm xúc của bạn, hiện thực khoa học hoàn toàn dửng dưng trước những giọt nước mắt. Bạn cảm thấy thánh đường thiêng liêng của mình bị sụp đổ, nhưng điều tương tự trước đây cũng từng xảy ra với bao ngành nghề khác rồi. Hãy dũng cảm chấp nhận thực tế.

-- [《Tôi hiểu vì sao các nhà toán học bật khóc》](https://www.derekthompson.org/p/i-know-why-the-mathematicians-weep)

## 往年回顾

[Cuộc đối thoại giữa Tim và La Vĩnh Hạo](https://www.ruanyifeng.com/blog/2025/10/weekly-issue-369.html) (#369)

[Làm thế nào để tạo ra video triệu view](https://www.ruanyifeng.com/blog/2024/09/weekly-issue-319.html) (#319)

[Tại sao người hùng không dùng thuốc nổ](https://www.ruanyifeng.com/blog/2023/09/weekly-issue-269.html) (#269)

[Cách phòng chống tài khoản bị xâm nhập](https://www.ruanyifeng.com/blog/2022/08/weekly-issue-219.html) (#219)

(Hết)
