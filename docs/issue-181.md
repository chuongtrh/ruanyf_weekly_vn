# 科技爱好者周刊（第 181 期）：移动支付应该怎么设计？

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1980) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102402.jpg)

Tại Tokyo, Nhật Bản có một nhà máy chuyên sản xuất nút bấm thang máy đã thiết lập một bức tường trưng bày khổng lồ gắn hơn 1.000 loại nút bấm thang máy khác nhau do hãng chế tạo qua các thời kỳ. Toàn bộ các nút bấm đều được cấp điện để phát sáng khi nhấn vào, thu hút rất đông trẻ em và người lớn tới tham quan trải nghiệm. (Nguồn: [Oddity Central](https://www.odditycentral.com/travel/pressing-1000-buttons-is-the-perfect-way-to-complete-an-elevator-button-factory-tour.html))

## 主带话题：移动支付应该怎么设计？

Alpay và WeChat Pay gần như độc quyền hoàn toàn thị trường thanh toán di động tại Trung Quốc với tổng thị phần nắm giữ vượt mức 90%.

Mặc dù hai công cụ mang lại sự tiện lợi cực lớn cho đời sống thường nhật, xét ở khía cạnh thiết kế kiến trúc hạ tầng thanh toán di động cấp quốc gia, mô hình hiện tại vẫn tồn tại nhiều rào cản bất cập.

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102803.jpg)

**Điểm hạn chế lớn nhất của Alipay và WeChat Pay là mô hình đóng (Walled Garden) khóa chặt người dùng trong hệ sinh thái của họ.** Một hạ tầng thanh toán công cộng đúng nghĩa cần mở rộng tự do cho bất kỳ ai sở hữu thiết bị di động, nhưng hiện tại bạn bắt buộc phải đăng ký thành viên và cài đặt ứng dụng của hai hãng này mới có thể thanh toán.

Để liên kết tài khoản ngân hàng thực tế, người dùng bắt buộc phải trải qua bước trung gian liên kết tài khoản với Alipay hoặc WeChat Pay chứ không thể dùng tài khoản ngân hàng thanh toán trực tiếp.

Ngoài ra còn có 3 nhược điểm lớn:

1. **Mã QR không đồng nhất:** mã QR của đơn vị này không thể quét đọc bằng ứng dụng của đơn vị kia, buộc các cửa hàng bán lẻ phải dán đồng thời nhiều mã QR khác nhau của từng hãng.
2. **Không thể chuyển tiền liên thông:** người dùng không thể chuyển khoản trực tiếp từ ví Alipay sang ví WeChat Pay và ngược lại, đồng thời không thể chuyển thẳng tới tài khoản ngân hàng của người khác mà phải thực hiện thao tác rút về ngân hàng của mình trước.
3. **Phí rút tiền về tài khoản ngân hàng bị thu phí** (dù rào cản này có thể xuất phát từ quy định chung để giữ dòng tiền trong ví).

Vậy đâu là một giải pháp thanh toán di động thông minh hơn? Câu trả lời nằm ở hệ thống quốc gia mà Brazil đã triển khai thành công.

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102906.jpg)

Mới đây tôi có đọc một bài báo của Bloomberg giới thiệu về hệ thống thanh toán di động **Pix** do Ngân hàng Trung ương Brazil ra mắt vào tháng 11/2020.

Nguyên lý hoạt động của Pix cực kỳ đơn giản: Khi mở tài khoản tại bất kỳ ngân hàng nào, người dùng chỉ cần đăng ký một hoặc nhiều thông tin định danh cá nhân độc nhất (chỉ số định danh như số điện thoại, email, số căn cước, hoặc mã định danh ngẫu nhiên). Sau đó, bạn sử dụng ứng dụng thanh toán Pix của chính phủ cung cấp để sinh mã QR thanh toán. Hệ thống Pix quốc gia sẽ tự động điều phối giao dịch chuyển tiền trực tiếp giữa các tài khoản ngân hàng đích của người bán và người mua.

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102805.jpg)

Chỉ trong vòng 11 tháng đi vào vận hành, Pix đã gặt hái thành công vang dội với hơn 110 triệu người dùng (chiếm hơn nửa dân số 210 triệu người của Brazil). Riêng trong tháng 9, tổng giá trị giao dịch qua Pix đạt 89 tỷ USD, trung bình mỗi người dùng giao dịch 800 USD, lượng giao dịch đỉnh điểm đạt hơn 40 triệu lượt mỗi ngày.

Hệ thống Pix sở hữu các ưu điểm tuyệt đối:

- **Tính mở hoàn toàn:** Mọi ngân hàng và tổ chức tài chính trung gian đều có thể tích hợp vào hệ thống thay vì bị thao túng bởi một vài tập đoàn công nghệ lớn.
- **Liên thông tài chính:** Mọi ví điện tử và tài khoản ngân hàng trong hệ thống có thể chuyển tiền qua lại trực tiếp cho nhau không giới hạn.
- **Đồng nhất mã QR:** Mã QR thanh toán tuân thủ quy chuẩn kỹ thuật quốc gia thống nhất, cho phép bất kỳ ứng dụng ngân hàng nào cũng có thể quét đọc và xử lý được.
- **Miễn phí giao dịch hoàn toàn cho người dân:** Chính phủ duy trì vận hành hệ thống bằng cách thu phí thường niên từ các tổ chức tài chính tham gia kết nối.

Đây là mô hình hạ tầng tài chính công cộng lý tưởng mà chính phủ các quốc gia nên học hỏi để thúc đẩy dòng lưu chuyển tiền tệ tự do, tạo động lực phát triển kinh tế bền vững cho toàn xã hội.

## KubeSphere 介绍

Xu hướng lớn nhất của ngành phát triển phần mềm thập kỷ qua chính là sự trỗi dậy của công nghệ container Docker giúp chuẩn hóa đóng gói và scale ứng dụng nhanh chóng.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092101.jpg)

Đi kèm với đó là Kubernetes (K8s) - công cụ điều phối container nguồn mở của Google đóng vai trò như bánh lái chỉ huy hàng nghìn container phân tán. Rào cản lớn nhất của K8s là cấu hình cực kỳ phức tạp và đòi hỏi kỹ sư chuyên môn cao để vận hành.

Để đơn giản hóa K8s cho các doanh nghiệp vừa và nhỏ, nền tảng nguồn mở **KubeSphere** đã ra đời đóng vai trò tương tự như hệ điều hành Ubuntu bao quanh nhân Linux kernel.

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102302.webp)

KubeSphere cung cấp bảng điều khiển đồ họa (GUI Dashboard) trực quan hướng dẫn người dùng cấu hình DevOps, triển khai microservices, quản lý chu kỳ ứng dụng và giám sát cảnh báo tài nguyên hệ thống K8s chỉ bằng vài click chuột mà không cần gõ câu lệnh phức tạp.

Dưới đây là video giới thiệu ngắn gọn trong 2 phút về giao diện bảng điều khiển trực quan và các tính năng quản lý mượt mà của KubeSphere:

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=h3303juxyex" allowFullScreen="true" width="600" height="400"></iframe>

Về mặt định vị thương mại, KubeSphere hướng tới các dịch vụ cấp doanh nghiệp yêu cầu cao về tính ổn định và bảo mật: tích hợp sẵn hệ thống thu thập log, giám sát tài nguyên phần cứng chi tiết, đo đạc lưu lượng mạng và tính năng chia hóa đơn tài nguyên sử dụng cho từng phòng ban.

Nền tảng cũng hỗ trợ quản lý đa đám mây (Multi-Cloud) và thiết lập môi trường HA giúp hệ thống vận hành tự động mượt mà.

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102304.webp)

Đối với các lập trình viên Front-end hay DevOps, KubeSphere tích hợp sẵn các template chạy ứng dụng cho Node.js, Java và các framework phổ biến giúp tự động hóa hoàn toàn quy trình đóng gói CI/CD: bạn chỉ cần push code lên Git, hệ thống sẽ tự động build image Docker và deploy lên cụm K8s tương ứng.

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102303.webp)

Dự án hiện đạt hơn 7.000 sao trên GitHub với cộng đồng hơn 250 lập trình viên đóng góp mã nguồn trên toàn cầu. Hơn một nửa số người dùng của KubeSphere đến từ thị trường quốc tế, trong khi các khách hàng lớn tại Trung Quốc bao gồm Trung tâm ngân hàng số Trung Quốc, ngân hàng WeBank, hãng vận chuyển ZTO Express.

Độc giả có thể tìm hiểu thêm tài liệu hướng dẫn và video bài giảng K8s tại website chính thức và trải nghiệm trực tiếp qua trang Demo trực tuyến của dự án.

## 科技动态

1、[Mỹ chế tạo thành công thiết bị cảm biến bay nhỏ bằng hạt cát](https://www.sciencealert.com/the-smallest-flying-device-ever-made-by-humans-is-like-a-grain-of-sand)

Các nhà khoa học tại Đại học Northwestern đã phát triển thành công dòng cảm biến cơ học trôi nổi (Microflyer) có kích thước tương đương một hạt cát nhỏ:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092406.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092407.jpg)

Thiết bị không trang bị động cơ chủ động mà hoạt động dựa trên nguyên lý cánh quạt xoay tự do đón gió. Toàn bộ cấu trúc bo mạch siêu nhỏ tích hợp sẵn cảm biến đo lường chất lượng không khí, pin mặt trời tích điện, ăng-ten phát sóng RF và bộ nhớ flash giúp chính phủ thả bay hàng loạt để phát hiện sớm các sự cố rò rỉ khí độc đô thị.

2、[Sáng chế cụm bàn phím phụ độc đáo dán sau điện thoại](https://ianthehenry.com/posts/peggi/)

Một nhà sáng chế phần cứng cá nhân đã phát triển mẫu bàn phím cơ mini gồm 8 nút bấm để dán cố định vào mặt lưng của điện thoại di động:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092410.jpg)

Bằng cách thiết lập các tổ hợp phím gõ dựa trên trí nhớ cơ bắp (tương tự mã Morse), người dùng có thể gõ nhanh toàn bộ bảng chữ cái và chữ số mà hoàn toàn không cần nhìn vào màn hình điện thoại. Nhược điểm lớn của thiết kế là chỉ tối ưu khi cầm điện thoại nằm ngang để gõ bằng ngón tay trỏ và ngón giữa:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092411.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092412.jpg)

3、[Trang trại sản xuất trứng gà quy mô lớn nhất châu Á đi vào hoạt động](https://finance.sina.com.cn/jjxw/2021-09-23/doc-iktzscyx5863357.shtml)

Trang trại chăn nuôi gà đẻ trứng tự động quy mô lớn nhất châu Á vừa chính thức đi vào vận hành tại đảo Sùng Minh, Thượng Hải:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092419.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092420.jpg)

Dự án có quy mô nuôi dưỡng thường trực 3 triệu gà mái đẻ với chu trình chăm sóc khép kín tự động. Hệ thống dự kiến cung cấp sản lượng trứng kỷ lục 800 triệu quả mỗi năm (trung bình 2 triệu quả trứng xuất xưởng mỗi ngày). Gà mái sau khi nuôi dưỡng 105 ngày ở trại giống sẽ được chuyển sang dây chuyền đẻ trứng trong vòng 72 tuần trước khi đào thải thay thế lứa mới:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092421.jpg)

4、[Hyundai ứng dụng robot bốn chân Boston Dynamics Spot tuần tra nhà máy](https://www.cnet.com/roadshow/news/boston-dynamics-spot-robotic-watchdog-hyundai/)

Tập đoàn sản xuất ô tô Hyundai mới đây đã đặt mua loạt robot chó bốn chân Spot của hãng Boston Dynamics để đưa vào vận hành tuần tra tự động tại các xưởng lắp ráp:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092417.jpg)

Robot được trang bị camera hồng ngoại tầm nhiệt và cảm biến quét LiDAR 3D hỗ trợ tự di chuyển ban đêm để phát hiện các khu vực máy móc tỏa nhiệt quá mức quy định hoặc phát hiện các cửa phòng không được khóa chốt để gửi cảnh báo an ninh về trung tâm. Hệ thống chỉ lập trình để phát hiện sự cố chứ không có tính năng tấn công hay truy đuổi kẻ đột nhập:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092418.jpg)

5、[Phát hiện dấu tay chân trẻ em cổ đại có niên đại 200.000 năm tại Tây Tạng](http://www.uua.cn/show-7-12334-1.html)

Các nhà khảo cổ học công bố kết quả giám định vết hóa thạch dấu tay và dấu chân trẻ em in trên đá travertine tại khu vực suối nước nóng cổ Qiusang, ngoại ô Lhasa:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092422.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092423.jpg)

Bản in đá được xác định hình thành từ khoảng 169.000 đến 226.000 năm trước. Các nhà khoa học phán đoán thời kỳ đó hai đứa trẻ cổ đại khi chơi đùa quanh các mạch bùn suối nước nóng chứa nhiều muối canxi cacbonat đã ấn tay chân của mình tạo hình nghệ thuật. Bùn sau đó nhanh chóng khô cứng và hóa đá theo thời gian để giữ nguyên vẹn dấu vết cho tới ngày nay:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092424.jpg)

6、[Nhân viên khiếu nại yêu cầu lắp camera AI giám sát khi làm việc tại nhà](https://9to5mac.com/2021/08/09/apple-call-center-workers-surveillance/)

Đội ngũ nhân sự hỗ trợ khách hàng của một tập đoàn dịch vụ đa quốc gia đã gửi đơn khiếu nại tập thể về quy định giám sát mới của hãng.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081101.jpg)

Theo đó, để được phê duyệt chế độ làm việc từ xa (work from home), nhân viên bắt buộc phải đồng ý lắp đặt hệ thống camera giám sát thông minh do hãng cung cấp tại phòng làm việc riêng để AI tự động quét nhận diện hành vi lơ là và ghi âm toàn bộ cuộc đối thoại trong giờ làm việc. Đây là xu hướng quản lý nhân sự từ xa khắc nghiệt đang gây nhiều tranh cãi.

## 文章

1. [Trải nghiệm chạy ứng dụng Android trên hệ điều hành Windows 11](https://sspai.com/post/69446)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102203.jpg)

Bài hướng dẫn chi tiết các bước thiết lập môi trường giả lập Windows Subsystem for Android (WSA) mới ra mắt trên Windows 11, đồng thời chia sẻ đánh giá thực tế về hiệu năng chơi game và khả năng tương thích app di động.

2. [Giải pháp quy hoạch kiến trúc đường ray trên cao độc đáo của nhà ga Tây Hàng Châu](https://mp.weixin.qq.com/s/jSeAG_YoTEJshhTQZLHf1Q)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102401.jpg)

Nhà ga tàu cao tốc Tây Hàng Châu phục vụ thế vận hội ASIAD 2022 sở hữu kiến trúc đột phá: đưa toàn bộ hệ thống đường ray và sân ga lên tầng cao của tòa nhà, giải phóng không gian mặt đất bên dưới cho mạng lưới giao thông công cộng đô thị, tránh việc đường ray chia cắt thành phố làm đôi.

3. [Đánh giá kế hoạch xây dựng siêu nhà máy đúc chip GigaFab của SMIC](https://www.anandtech.com/show/16931/china-smic-build-gigafab)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092111.jpg)

Bài phân tích chuyên sâu về kế hoạch đầu tư xây dựng cơ sở sản xuất chip bán dẫn quy mô lớn GigaFab (công suất thiết kế vượt 100.000 tấm wafer/tháng) tại khu thương mại tự do Lâm Cảng, Thượng Hải của tập đoàn SMIC.

4. [Microsoft chính thức ra mắt trình soạn thảo VS Code phiên bản web](https://code.visualstudio.com/blogs/2021/10/20/vscode-dev)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102909.jpg)

Microsoft công bố phát hành tên miền chính thức `vscode.dev` cho phép lập trình viên chạy trực tiếp trình soạn thảo VS Code trên mọi trình duyệt web di động và máy tính mà không cần cài đặt node hay thư viện hỗ trợ. (Đóng góp của [@StevenNin](https://github.com/ruanyf/weekly/issues/2012))

5. [Hướng dẫn đăng ký mã chỉ số tạp chí ISSN cho trang web cá nhân](https://shkspr.mobi/blog/2021/09/how-to-add-issn-metadata-to-a-web-page/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092006.jpg)

Tác giả chia sẻ kinh nghiệm chuẩn bị hồ sơ và đăng ký thành công mã chỉ số ISSN quốc tế cho trang blog cá nhân của mình giúp chuẩn hóa siêu dữ liệu phục vụ các trích dẫn nghiên cứu khoa học.

6. [Tại sao doanh nghiệp nên cấu hình tệp tin Security.txt trên server?](https://krebsonsecurity.com/2021/09/does-your-organization-have-a-security-txt-file/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092213.jpg)

Giới thiệu tiêu chuẩn bảo mật mới đề xuất việc cấu hình tệp tin cấu trúc `security.txt` đặt tại thư mục gốc `.well-known/` của website giúp các chuyên gia bảo mật mũ trắng dễ dàng tìm thấy thông tin liên hệ báo cáo lỗ hổng an ninh.

7. [Phát triển giao diện web theo cơ chế Server-Informed UI](https://max.engineer/server-informed-ui)（Tiếng Anh）

Tác giả đề xuất phương án tối ưu thiết kế API Backend: thay vì chỉ xây dựng một hệ thống API chung cho mọi tác vụ, hãy tách biệt thành một cổng API dữ liệu chung và một cổng API chuyên biệt định hình giao diện (Server-Informed UI) giúp client render trang nhanh hơn.

8. [Nhật ký tự lắp ráp và cấu hình case máy tính chơi game chạy hệ điều hành Linux](https://boilingsteam.com/how-i-built-my-new-linux-gaming-desktop-in-2021-with-amd-cpugpu-and-gnu-guix/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092408.jpg)

Tác giả chia sẻ kinh nghiệm lựa chọn linh kiện phần cứng (CPU AMD, card đồ họa Radeon) và cài đặt phân phối hệ điều hành GNU Guix để tự dựng một cỗ máy PC chuyên dụng chơi game mượt mà trên nền tảng Linux:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092409.jpg)

9. [Tìm hiểu API phát hiện trạng thái rảnh Idle Detection API của Chrome](https://web.dev/idle-detection/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092414.jpg)

Hướng dẫn sử dụng đối tượng `IdleDetector` mới được tích hợp sẵn trên Chrome hỗ trợ website phát hiện hành vi người dùng không hoạt động (không gõ phím, di chuột hoặc màn hình bị khóa) để tự động lưu dữ liệu hoặc tắt các tác vụ nặng.

## 工具

1、[EBS Design: Thư viện components React hiện đại](https://github.com/ebs-integrator/ebs-design)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092112.jpg)

Bộ component UI mã nguồn mở được thiết kế theo phong cách tối giản hiện đại (Neumorphism kết hợp Flat Design) đang được phát triển tích cực cho các ứng dụng React.

2、[bunny.net: Dịch vụ CDN hiệu năng cao](https://bunny.net/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091812.jpg)

Một nhà cung cấp dịch vụ mạng truyền tải nội dung CDN có tính phí được đánh giá cao nhờ tốc độ phân phối dữ liệu nhanh và chi phí hợp lý, thích hợp làm giải pháp dự phòng cho Cloudflare.

3、[context-note: Extension ghi chú tài liệu trực tiếp trên website](https://github.com/betterRunner/context-note)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082304.jpg)

Extension Chrome hỗ trợ người dùng quét chọn văn bản và tạo ghi chú trực tiếp trên trang web, tự động lưu trữ hiển thị lại ghi chú đó ở đúng vị trí cũ trong lần truy cập sau. (Đóng góp của [@betterRunner](https://github.com/ruanyf/weekly/issues/2013))

4、[APIAuto: Hệ thống tự động hóa kiểm thử API của Tencent](https://github.com/TommyLemon/APIAuto)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102404.jpg)

Dự án nguồn mở của Tencent hỗ trợ quét cấu trúc API, tự động sinh các test-cases và thực hiện kiểm thử tự động dựa trên phân tích thuật toán học máy thông minh. (Đóng góp của [@TommyLemon](https://github.com/ruanyf/weekly/issues/2010))

5、[3D pipes Screen Saver in HTML5 Canvas](https://1j01.github.io/pipes/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092004.jpg)

Dự án mã nguồn mở thú vị sử dụng thư viện đồ họa để tái hiện lại hoàn hảo màn hình chờ 3D Pipes (đường ống dẫn nước 3D) huyền thoại của Windows 95/98 ngay trên trang web.

6、[Composable: Trình vẽ đồ họa vector trực tuyến](https://www.composable.art/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092107.jpg)

Công cụ trực tuyến gọn nhẹ hỗ trợ người dùng vẽ, chỉnh sửa và xuất các file đồ họa vector dạng SVG trực tiếp trên trình duyệt web.

7、[lists.sr.ht: Dịch vụ mailing list nguồn mở](https://lists.sr.ht/)

Nền tảng hỗ trợ các nhà phát triển thiết lập và quản lý hệ thống hòm thư chung (mailing list) phục vụ thảo luận đóng góp mã nguồn cho dự án công nghệ.

8、[Kill the Newsletter! (Chuyển đổi email newsletter sang RSS)](https://github.com/leafac/kill-the-newsletter)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091814.jpg)

Công cụ nguồn mở hỗ trợ chuyển đổi toàn bộ các email bản tin nhận qua hòm thư thành đường dẫn cập nhật luồng RSS feed giúp quản lý thông tin tập trung trên các ứng dụng đọc tin.

9、[AirGuard: Phát hiện AirTag lạ theo dõi xung quanh](https://github.com/seemoo-lab/AirGuard)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091917.jpg)

Ứng dụng nguồn mở dành riêng cho điện thoại Android hỗ trợ quét tìm nhanh sự hiện diện của các thiết bị định vị Bluetooth lạ (như AirTag) đang di chuyển theo lộ trình của bạn để cảnh báo nguy cơ bị bám đuôi.

10、[Black: Trình format code Python chuẩn hóa](https://black.vercel.app/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092215.jpg)

Thư viện định dạng mã nguồn Python tự động (code formatter) được cộng đồng tin dùng nhất nhờ khả năng dọn dẹp các khoảng trống dư thừa và căn lề code chuẩn hóa.

## Tài nguyên

1、[10 công cụ trực tuyến kiểm thử giao diện responsive của website](https://www.webfx.com/blog/web-design/responsive-design-testing-tools/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080508.jpg)

Giới thiệu danh sách 10 công cụ web tiện ích hỗ trợ nhà phát triển Front-end giả lập hiển thị và kiểm tra lỗi vỡ khung giao diện web trên nhiều độ phân giải màn hình di động khác nhau.

2、[pi (zhaoolee): Hướng dẫn biến Raspberry Pi thành máy chủ cloud](https://github.com/zhaoolee/pi)

Cẩm nang hướng dẫn chi tiết cách cấu hình máy tính nhúng mini Raspberry Pi 4B kết hợp công cụ nội soi mạng frp để thiết lập một server đám mây cá nhân có IP tĩnh truy cập từ xa. (Đóng góp của [@zhaoolee](https://github.com/ruanyf/weekly/issues/2008))

3、[CPU Museum: Bảo tàng chip xử lý Intel trực tuyến](https://www.mynikko.com/CPU/)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102403.jpg)

Trang web chia sẻ thông tin hình ảnh chi tiết giới thiệu bộ sưu tập các thế hệ chip xử lý của Intel từ thời kỳ sơ khai 3101 cho đến dòng Pentium M của tác giả. (Đóng góp của [@TransparentLC](https://github.com/ruanyf/weekly/issues/2009))

4、[Git Flight Rules: Cẩm nang xử lý nhanh các sự cố Git](https://github.com/k88hudson/git-flight-rules/blob/master/README_zh-CN.md)

Bản dịch tiếng Trung tổng hợp các câu hỏi thường gặp và cẩm nang câu lệnh Git tương ứng để giải quyết nhanh các tình huống gộp nhánh lỗi, sửa tin nhắn commit sai hoặc khôi phục file bị xóa. (Đóng góp của [@xcuYao](https://github.com/ruanyf/weekly/issues/2015))

5、[Decentralized Library: Thư viện Libgen chuyển dịch lên IPFS](https://libgen.fun/dweb.html)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092005.jpg)

Dự án thư viện sách điện tử khổng lồ Libgen công bố hoàn thành việc chuyển đổi toàn bộ cơ sở dữ liệu và trang hiển thị sang giao thức lưu trữ phân tán IPFS giúp hạn chế rủi ro bị khóa máy chủ.

## 图片

1、[Mẫu cầu vượt bộ hành nhẹ lắp đặt nhanh tại Anh](https://www.railadvent.co.uk/2021/06/groundbreaking-new-bridge-design-could-transform-rail-crossings-across-the-uk.html)

Lực lượng kỹ sư đường sắt Anh đang tiến hành lắp đặt thử nghiệm dòng cầu vượt bộ hành chế tạo từ vật liệu polymer siêu nhẹ gia cường sợi thủy tinh:

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062904.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062905.jpg)

Cấu trúc cầu được tính toán tối ưu giúp giảm trọng lượng khung sắt truyền thống xuống 50%, cho phép vận chuyển và cẩu lắp ráp hoàn thiện bắc ngang đường sắt chỉ trong vòng một đêm để tiết kiệm chi phí thi công.

2、[Mẫu font chữ giải phẫu độc đáo Dissection Font](http://erikdemaine.org/fonts/dissect/)

Giáo sư khoa học máy tính huyền thoại Donald Knuth đồng phát triển bộ font chữ giải phẫu độc đáo: toàn bộ các chữ cái Latin đều được thiết kế để có thể cắt nhỏ ra và ghép khít lại thành một hình vuông kích thước 6x6 pixel:

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062808.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062809.jpg)

3][Bản đồ giả lập thế giới khi mực nước biển dâng cao](https://ahstat.github.io/Topography/)

Sơ đồ mô phỏng địa lý thế giới khi mực nước biển dâng cao thêm 100m do hiện tượng biến đổi khí hậu làm tan băng hai cực:

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021100318.jpg)

Bản đồ thế giới khi mực nước biển dâng cao kỷ lục thêm 1.000m:

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021100319.jpg)

## Bài đọc thêm

### Xu hướng quay trở lại của hệ thống dòng điện một chiều DC hạ thế

**1. Tại sao dòng điện xoay chiều AC giành chiến thắng lịch sử?**

Vào cuối thế kỷ 19, cuộc chiến dòng điện nổ ra giữa Thomas Edison (ủng hộ dòng DC) và Nikola Tesla (ủng hộ dòng AC). Chung cuộc, dòng điện AC giành chiến thắng tuyệt đối nhờ khả năng nâng điện áp lên rất cao thông qua máy biến áp, giúp truyền tải điện năng đi xa hàng nghìn cây số mà không bị hao hụt nhiệt lượng trên đường dây (do dòng điện nhỏ). Thời điểm đó hệ thống DC không có công nghệ nâng áp nên dòng điện lớn gây nóng chảy đường dây nếu truyền đi xa hơn 1 km:

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102801.jpg)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102908.jpg)

**2. Hai xu thế mới châm ngòi cho sự hồi sinh của dòng DC**

Tuy nhiên sự bùng nổ của hai yếu tố công nghệ mới đang khiến dòng DC trở lại:
- **Điện mặt trời áp mái và pin lưu trữ:** các tấm pin mặt trời và pin lithium đều phát và lưu trữ năng lượng dưới dạng dòng điện một chiều DC ngay tại chỗ (mô hình phân tán), không cần truyền tải đi xa.
- **Thiết bị điện tử tiêu dùng chạy nguồn DC:** hầu hết các thiết bị hiện đại như máy tính, smartphone, tivi LED, lò vi sóng đều vận hành bằng dòng điện DC.

**3. Sự lãng phí năng lượng của quá trình chuyển đổi dòng điện**

Thông thường trong các hộ gia đình lắp điện mặt trời, dòng điện DC từ tấm pin phải đi qua bộ kích biến đổi thành dòng AC để truyền vào lưới điện gia đình, sau đó khi cắm sạc laptop hay tivi, dòng AC này lại đi qua củ sạc chuyển đổi ngược lại thành dòng DC. Quá trình chuyển đổi kép này gây tổn hao tới 20% - 30% lượng điện năng dưới dạng nhiệt lượng tỏa ra.

**4. Lợi ích khi thiết lập mạng điện DC trực tiếp cho tòa nhà**

- Loại bỏ hoàn toàn năng lượng thất thoát do chuyển đổi dòng điện.
- Tiết kiệm chi phí mua bộ nghịch lưu (inverter) đắt tiền và có tuổi thọ ngắn hơn tấm pin mặt trời.
- Đơn giản hóa cấu trúc bo mạch nguồn của các thiết bị điện tử, giúp chúng bền và rẻ hơn.
- An toàn tuyệt đối: dòng DC hạ thế thường dưới 24V không gây nguy cơ điện giật hay chập cháy nổ lớn.

**5. Rào cản lớn nhất của dòng DC hạ thế**

Hao hụt truyền dẫn trên đường dây DC hạ thế rất lớn khi khoảng cách tăng lên: một dây đồng truyền điện 12V cấp điện cho lò vi sóng công suất 1.000W sẽ bị thất thoát tới 47% điện năng chỉ trên chiều dài dây 3m. Do đó dòng DC chỉ phù hợp cấp điện cho các thiết bị công suất thấp như đèn LED, laptop và yêu cầu bố trí thiết bị ở vị trí gần nhất dưới tấm pin mặt trời.

## 言论

1、

Khi tôi chạm ngưỡng 80 tuổi, tôi sẽ không bao giờ hối tiếc vì những dự án khởi nghiệp thất bại mà tôi đã dũng cảm dấn thân thử nghiệm thời trẻ. Tôi chỉ hối tiếc về những ý tưởng hay ho mà tôi đã chần chừ không dám làm, chúng sẽ luôn là nỗi trăn trở ám ảnh tâm trí tôi.

-- Trích bài viết "Regret Minimization Framework" của Jeff Bezos

2、

Một dự án phần mềm nguồn mở thành công thường vận hành theo mô hình "dự án anh hùng" (hero project): nơi có tới hơn 80% lượng code đóng góp cốt lõi đến từ vỏn vẹn 20% số lượng lập trình viên chủ lực của dự án.

-- Trích nghiên cứu về hoạt động mã nguồn mở trên GitHub

## 历史上的本周

- 2020年（第 130 期）：[Phân tích xu hướng trẻ hóa và giảm độ tuổi trung bình của người dùng internet toàn cầu](https://www.ruanyifeng.com/blog/2020/10/weekly-issue-130.html)
- 2019年（第 78 期）：[Khảo sát các mảng công nghiệp và dịch vụ mới được dự báo sẽ trở thành xu hướng đón đầu dòng vốn đầu tư](https://www.ruanyifeng.com/blog/2019/10/weekly-issue-78.html)
- 2018年（第 27 期）：[Thảo luận về tính đúng đắn của giả thuyết "Làm việc vì đam mê" của Steve Jobs đối với giới trẻ lập nghiệp](https://www.ruanyifeng.com/blog/2018/10/weekly-issue-27.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
