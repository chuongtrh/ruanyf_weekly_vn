# 科技爱好者周刊（第 219 期）：如何防止帐号被黑

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần。

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn。

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2542) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập。

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081706.webp)

"Trung tâm Siêu máy tính Vũ Hán" được xây dựng bằng cách lắp ghép các container đúc sẵn, là trung tâm siêu máy tính dạng container có quy mô lớn nhất cả nước hiện nay. Dự án đã chính thức kết nối vào "Mạng lưới Điện toán Trung Quốc" vào ngày 15 tháng 8 để cung cấp năng lực tính toán hiệu năng cao. (Nguồn: [CNHubei](http://www.cnhubei.com/content/2022-08/16/content_14982905.html))

## 本周话题：如何防止帐号被黑

Tuần trước đã xảy ra một sự cố bảo mật nghiêm trọng. Hai doanh nghiệp công nghệ lớn của Mỹ là [Twilio](https://www.twilio.com/blog/august-2022-social-engineering-attack) và [Cloudflare](https://blog.cloudflare.com/2022-07-sms-phishing-attacks/) đã bị tấn công mạng, trong đó Twilio đã bị hacker xâm nhập thành công vào hệ thống.

Cả hai đều là những công ty có năng lực kỹ thuật hàng đầu và đã kích hoạt bảo mật xác thực hai lớp (2FA), nhưng vẫn bị tấn công hiệu quả. Những thông tin chi tiết được họ công bố sau sự cố là bài học đắt giá về an toàn thông tin tài khoản:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081711.webp)

Đầu tiên, chúng ta cần thống nhất một nguyên lý: **Chỉ sử dụng mật khẩu đăng nhập thông thường là cực kỳ không an toàn, bắt buộc phải bật xác thực hai lớp.**

Hầu hết cơ sở dữ liệu mật khẩu người dùng trên Internet đều đã bị rò rỉ và rao bán trên các chợ đen trực tuyến. Bạn nên mặc định rằng mật khẩu cá nhân của mình đã bị lộ. Việc sử dụng các mật khẩu khác nhau cho từng trang web giúp giảm thiểu rủi ro, nhưng không thể đảm bảo an toàn tuyệt đối nếu thiếu đi lớp bảo vệ thứ hai.

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081116.webp)

Bất kỳ tài khoản quan trọng nào cũng cần được kích hoạt bảo mật xác thực hai lớp (2FA). Tuy nhiên, người dùng vẫn phải hết sức cảnh giác vì **xác thực hai lớp hoàn toàn có thể bị bẻ khóa bằng các phương thức tinh vi.**

Phương thức 2FA phổ biến nhất là mật khẩu kết hợp mã OTP gửi qua tin nhắn SMS. Rủi ro của phương thức này nằm ở chỗ tin nhắn SMS không được mã hóa đầu cuối khi truyền tải. Kẻ xấu thậm chí có thể làm giả giấy tờ tùy thân của nạn nhân để yêu cầu nhà mạng cấp lại thẻ SIM (tấn công SIM swap) nhằm đánh cắp mã OTP SMS.

Một giải pháp 2FA khác đang được nhiều ngân hàng áp dụng là mật khẩu kết hợp nhận diện khuôn mặt. Tuy nhiên, cơ chế so khớp ảnh selfie trực tiếp với ảnh căn cước công dân lưu trữ của hệ thống đã bị tội phạm công nghệ vượt qua dễ dàng trong nhiều vụ án lừa đảo tài chính gần đây.

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081119.webp)

Phương thức 2FA được đánh giá là an toàn hơn cả là mật khẩu kết hợp mã thời gian thực [TOTP](https://en.wikipedia.org/wiki/Time-based_one-time_password). Người dùng cài đặt ứng dụng sinh mã (như Google Authenticator hoặc Authy), hệ thống sẽ dựa trên khóa bí mật để sinh ra mã xác thực 6 chữ số thay đổi liên tục mỗi 30 giây.

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081118.webp)

Đáng tiếc, vụ tấn công tuần trước lại bẻ khóa thành công chính cơ chế xác thực TOTP này. Dưới đây là cách thức hacker thực hiện:

Ban đầu, nhân viên của Twilio và Cloudflare nhận được tin nhắn SMS giả mạo vào ngày nghỉ hoặc ngoài giờ làm việc với nội dung thông báo lịch làm việc thay đổi hoặc phiên đăng nhập tài khoản sắp hết hạn, yêu cầu truy cập đường dẫn đính kèm để cập nhật:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081204.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081205.webp)

Tin nhắn chứa các đường dẫn lừa đảo sử dụng các tên miền giả mạo chứa các từ khóa quen thuộc của doanh nghiệp như "sso" hoặc "okta". Hacker thu thập số điện thoại của các kỹ sư thông qua dữ liệu công khai trên mạng xã hội nghề nghiệp LinkedIn.

Khi nhân viên thiếu cảnh giác bấm vào đường link, họ sẽ được dẫn tới một trang đăng nhập giả mạo có giao diện giống hệt trang đăng nhập nội bộ của công ty. Ngay khi họ điền tên đăng nhập và mật khẩu, dữ liệu này sẽ lập tức được gửi về máy chủ của hacker:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081206.webp)

Do hệ thống của hai công ty yêu cầu xác thực hai lớp, trang web giả mạo tiếp tục chuyển hướng yêu cầu người dùng nhập mã xác thực TOTP 6 số.

Lúc này, hacker thực hiện tấn công theo thời gian thực (real-time attack): ngay khi nhân viên điền mã 6 số vào trang giả mạo, hệ thống của hacker sẽ tự động sao chép mã này và điền vào trang đăng nhập thật của doanh nghiệp trước khi mã hết hiệu lực trong vòng 30 giây để chiếm quyền truy cập.

Hầu hết hệ thống bảo mật của các doanh nghiệp sử dụng TOTP đều sẽ bị khuất phục trước phương thức tấn công trung gian (Man-in-the-Middle) này. Tuy nhiên, hệ thống của Cloudflare đã chặn đứng cuộc tấn công nhờ việc yêu cầu nhân viên xác thực bằng **Khóa bảo mật vật lý (YubiKey)** thay vì dùng mã TOTP:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081207.webp)

Khóa vật lý yêu cầu người dùng phải cắm trực tiếp thiết bị vào cổng USB máy tính để xác thực phần cứng. Do hacker không thể chiếm đoạt thiết bị vật lý từ xa, cuộc tấn công của chúng hoàn toàn thất bại.

Bài học rút ra từ sự cố là: **Phương pháp xác thực an toàn nhất hiện nay là mật khẩu kết hợp khóa bảo mật vật lý phần cứng.** Hiện nay nhiều dịch vụ lớn như GitHub đã hỗ trợ phương thức này:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081801.webp)

Do giá thành của các khóa bảo mật vật lý còn khá cao, công nghệ Web Authentication đang được thúc đẩy phát triển để biến chính chiếc điện thoại thông minh hoặc cảm biến vân tay/khuôn mặt tích hợp trên máy tính của người dùng thành một khóa bảo mật vật lý tương đương.

Với đa số người dùng phổ thông, giải pháp tối ưu để bảo vệ tài khoản hiện nay là: kiên trì bật bảo mật hai lớp 2FA, sử dụng các mật khẩu phức tạp và khác nhau cho từng dịch vụ, và tuyệt đối không điền mật khẩu vào các đường dẫn lạ chưa được kiểm chứng.

## 微服务框架 CloudWeGo

Có thể bạn chưa biết, các cấu phần kiến trúc backend vận hành hệ sinh thái ứng dụng của ByteDance (TikTok) đều sử dụng các mã nguồn mở. Vào tháng 9 năm ngoái, ByteDance đã chính thức mở mã nguồn của microservices framework **[CloudWeGo](https://www.cloudwego.io/zh/)** bao gồm các công cụ tự phát triển tối ưu cho việc xây dựng hạ tầng云原生 (Cloud Native).

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081701.webp)

Bộ framework này hiện đang chịu tải cho hơn 100.000 microservices nội bộ và quản lý khoảng 10 triệu container của tập đoàn ByteDance. Bản phân phối nguồn mở sử dụng chung bộ mã nguồn cốt lõi với hệ thống nội bộ của doanh nghiệp và đã nhận được hơn 9.000 sao trên GitHub.

Nhân dịp kỷ niệm 1 năm ra mắt dự án, đội ngũ CloudWeGo sẽ tổ chức sự kiện chuyên đề trực tuyến chia sẻ sâu về cấu trúc hệ thống backend của ByteDance (như kiến trúc của ứng dụng Lark/Feishu) và hướng dẫn phương pháp xây dựng hệ thống microservices cho doanh nghiệp:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081608.webp)

Sự kiện diễn ra vào chiều thứ Bảy (ngày 27 tháng 8) tuần tới dưới dạng phát sóng trực tiếp. Bạn đọc quan tâm có thể đăng ký tham gia thông qua đường dẫn hoặc quét mã QR trong bài viết.

## 科技动态

1、[Mô hình robot phẫu thuật Da Vinci phổ cập tại các bệnh viện lớn của Mỹ](https://spectrum.ieee.org/robotic-surgery)

Hệ thống robot hỗ trợ phẫu thuật Da Vinci do công ty Intuitive Surgical phát triển hiện đã đi vào vận hành tại hầu hết các bệnh viện hàng đầu tại Mỹ:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070602.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070603.webp)

Robot được trang bị 4 cánh tay cơ khí phối hợp nhịp nhàng thực hiện ca phẫu thuật: các tay lái giữ nhiệm vụ mổ xẻ vách cơ, khâu vết thương, di chuyển dụng cụ nội soi và 1 tay chuyên dụng giữ camera siêu nét truyền hình ảnh thời gian thực. Bác sĩ phẫu thuật chính sẽ điều khiển thiết bị thông qua cabin giám sát trực quan bên cạnh.

2、[Sự xuất hiện của các thiết bị khóa hẹn giờ giúp người dùng tự cai nghiện điện thoại](https://www.163.com/dy/article/H62O5V64053469LG.html)

Sự phổ biến của điện thoại thông minh làm suy giảm khả năng tập trung của người dùng. Để giải quyết thực trạng này, thị trường xuất hiện các sản phẩm hộp đựng điện thoại hẹn giờ khóa tự động:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081401.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081402.webp)

Được mệnh danh là "Công cụ tự kỷ luật", người dùng đặt điện thoại vào bên trong hộp và thiết lập thời gian khóa. Hộp khóa sẽ không thể mở ra bằng bất kỳ cách nào cho đến khi hết thời gian đếm ngược.

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081403.webp)

Nhiều người cho rằng thiết bị chỉ mang tính chất giải tỏa tâm lý, nhưng nhiều học sinh ghi nhận thiết bị thực sự giúp họ tập trung học tập tốt hơn và giảm thời gian lướt mạng vô bổ.

3、[Thử nghiệm cấy ghép giác mạc nhân tạo sản xuất từ da heo thành công](https://www.8world.com/world/bioengineered-cornea-can-restore-sight-to-the-blind-and-visually-impaired-1888616)

Bệnh lý giác mạc là nguyên nhân gây mù lòa cho khoảng 5% bệnh nhân khiếm thị trên thế giới. Phương pháp điều trị duy nhất là cấy ghép giác mạc hiến tặng từ người quá cố, vốn luôn trong tình trạng khan hiếm nghiêm trọng.

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081601.webp)

Mới đây, nhóm nghiên cứu tại Đại học Linköping, Thụy Điển công bố thành tựu chế tạo giác mạc nhân tạo sinh học từ collagen chiết xuất từ da heo phế thải. Thiết bị đã được cấy ghép thành công cho 20 bệnh nhân khiếm thị tại Iran và Ấn Độ:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081602.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081603.webp)

Sau 24 tháng theo dõi, 14 bệnh nhân mù lòa đã khôi phục lại thị lực hoàn toàn, 6 bệnh nhân còn lại cải thiện đáng kể từ thị lực yếu sang mức trung bình. Đội ngũ y tế đang tiến hành thủ tục xin cấp phép thử nghiệm lâm sàng quy mô lớn 100 người tại khu vực Âu Mỹ.

4、[Thử nghiệm giải pháp làm mát tập trung đô thị tại Quảng Châu](https://www.time-weekly.com/post/294534)

Trái ngược với hệ thống sưởi ấm tập trung mùa đông ở miền Bắc, khu đô thị mới Zhujiang New Town tại Quảng Châu đang thí điểm mô hình làm mát tập trung (district cooling) cho các tòa nhà:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081709.webp)

Các căn hộ trong khu vực không cần lắp cục nóng điều hòa riêng lẻ. Trạm làm mát trung tâm sử dụng hệ thống tích trữ đá lạnh quy mô lớn vào ban đêm (khi giá điện rẻ) để cấp năng lượng, ban ngày đá lạnh được làm tan chảy thành nước lạnh và dẫn qua mạng lưới đường ống ngầm đến từng tòa nhà để làm mát không khí.

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081710.webp)

Giải pháp giúp tiết kiệm đáng kể điện năng tiêu thụ và giảm hiệu ứng đảo nhiệt đô thị, tuy nhiên chi phí đầu tư quỹ đất xây dựng trạm trung tâm giữa lòng thành phố lớn là rào cản lớn nhất cho việc phổ cập mô hình này.

5、[Hệ thống pin nhiệt năng từ cát đầu tiên đi vào vận hành tại Phần Lan](https://www.energy-storage.news/worlds-first-large-scale-sand-battery-goes-online-in-finland/)

Phần Lan khánh thành trạm lưu trữ nhiệt năng bằng cát khô thương mại đầu tiên trên thế giới, được ví như một quả "pin cát" khổng lồ:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070704.webp)

Hệ thống là một bồn chứa bằng thép cao 7m rộng 4m chứa hàng trăm tấn cát khô. Nguồn điện năng dư thừa từ các tua-bin gió được sử dụng để nung nóng cát bên trong bồn chứa lên tới nhiệt độ 500 - 600°C và giữ nhiệt trong nhiều tháng. Khi mùa đông đến, lượng nhiệt lưu trữ trong cát được truyền dẫn phục vụ sưởi ấm cho hệ thống nhà dân của khu vực với giá thành cực kỳ rẻ.

## 文章

1、[Trải nghiệm một ngày làm việc của nhân viên giám sát an toàn xe tự lái Baidu](https://oversea.huanqiu.com/article/4909nNA0m09)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081605.webp)

Bài viết ghi chép lại trải nghiệm thực tế của một nhân viên giám sát an toàn ngồi ở ghế lái phụ trên dòng xe robotaxi tự lái chạy thử nghiệm của Baidu tại khu công nghiệp Shougang (Bắc Kinh), chia sẻ về thói quen vận hành của xe tự lái và cảm giác khi giao phó tính mạng cho AI điều khiển.

2、[Khám phá kiến trúc cầu vòm gỗ cổ đại độc đáo của Trung Quốc](https://mp.weixin.qq.com/s/Zc47jf3OCYjjdgJ2qpu1rg)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081707.webp)

Bên cạnh cầu vòm đá, kiến trúc cầu vòm gỗ ghép chịu lực là một trong những thành tựu kỹ thuật xây dựng độc đáo thời cổ đại. Bài viết phân tích cấu trúc kết cấu dầm đan xen chịu lực của các cây cầu gỗ cổ xưa sau vụ việc cháy rụi đáng tiếc của cây cầu vạn an lịch sử tại Phúc Kiến.

3、[Dự án xây dựng hệ thống quản trị thông minh tại chùa Linh Ẩn, Hàng Châu](https://mp.weixin.qq.com/s/xeNhTRQIY_EQheJyRVTr6Q)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081816.webp)

Hình ảnh ghi nhận buổi lễ ra mắt chính thức hệ thống "Quản trị chùa chiền thông minh" ứng dụng CNTT quản lý dữ liệu, camera an ninh và lưu lượng khách tham quan tại ngôi chùa Linh Ẩn cổ kính.

4、[Đánh giá hiệu năng của JavaScript Runtime thế hệ mới Bun so với Node.js](https://semaphoreci.com/blog/javascript-bun#what-is-bun)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081504.webp)

Bun là môi trường runtime chạy JS/TS được viết bằng ngôn ngữ Zig định hướng thay thế cho Node.js tích hợp sẵn trình đóng gói (bundler) và quản lý gói (package manager). Bài viết thực hiện các bài benchmark đánh giá tốc độ khởi động và thực thi vượt trội của Bun.

5、[Khuyến nghị ngừng sử dụng nhãn chú thích TODO chung chung trong mã nguồn](https://goldin.io/blog/stop-using-todo)（Tiếng Anh）

Tác giả đề xuất các lập trình viên thay đổi thói quen viết các ghi chú `// TODO` chung chung vốn dễ bị lãng quên trong dự án, thay bằng các nhãn mô tả cụ thể công việc cần xử lý như `// DOCME` (cần bổ sung tài liệu hướng dẫn) hoặc `// TESTME` (cần viết test cases).

6、[So sánh chi tiết chất lượng cảm biến camera của Xiaomi 12s Ultra và iPhone 13 Pro Max](https://www.xda-developers.com/xiaomi-12s-ultra-vs-apple-iphone-13-pro-max-camera-shootout-comparison/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081404.webp)

Mẫu điện thoại Xiaomi 12s Ultra trang bị cảm biến ảnh kích thước lớn tới 1 inch hợp tác cùng Leica. Trang tin công nghệ XDA tiến hành chụp thực tế so sánh chi tiết dải động, độ chi tiết và khả năng khử nhiễu của cảm biến này so với iPhone 13 Pro Max.

7、[Phân biệt cơ chế hoạt động và vai trò của thư viện OpenSSL và OpenSSH](https://www.cnblogs.com/foohack/p/4103212.html)（Tiếng Trung）

Bài viết phân tích sự khác biệt cốt lõi: OpenSSL là thư viện hàm lập trình viết bằng C cung cấp các giao thức mã hóa dữ liệu bảo mật SSL/TLS; trong khi OpenSSH là bộ công cụ cung cấp dịch vụ đăng nhập shell mã hóa bảo mật từ xa dựa trên nền tảng mật mã của OpenSSL.

8、[Sử dụng trí tuệ nhân tạo giải thích cơ chế hoạt động của các đoạn code phức tạp](https://simonwillison.net/2022/Jul/9/gpt-3-explain-code/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070917.webp)

Tác giả chia sẻ trải nghiệm thực tế khi đưa các đoạn mã nguồn lập trình tối giản khó hiểu cho mô hình AI GPT-3 của OpenAI phân tích và viết lại lời giải thích logic hoạt động chi tiết bằng ngôn ngữ tự nhiên.

## 工具

1、[Maccy: Tiện ích quản lý lịch sử sao chép clipboard nguồn mở cho macOS](https://maccy.app/)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062406.webp)

Công cụ nhỏ gọn hỗ trợ lưu giữ lịch sử các đoạn văn bản, hình ảnh người dùng đã copy vào bộ nhớ đệm clipboard hệ thống để tra cứu sử dụng lại nhanh chóng.

2、[Nude UI: Thư viện Web Component biểu mẫu siêu nhẹ do Lea Verou thiết kế](https://nudeui.com/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081301.webp)

Bộ công cụ thiết kế chứa các thành phần form nhập liệu tối giản dễ sử dụng được phát triển trực tiếp trên chuẩn Web Component giúp tăng tốc độ tải trang Front-end.

3、[Cartoon Cat Generator: Trang web trực tuyến tự thiết kế ảnh mèo hoạt hình](https://uchinoko-maker.jp/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081309.webp)

Tiện ích giải trí hỗ trợ người dùng tùy chọn màu lông, hình dáng đuôi và mắt để tự tạo hình ảnh minh họa chú mèo cưng của mình dưới dạng phong cách hoạt hình dễ thương.

4、[Glances: Công cụ giám sát tài nguyên hệ thống đa nền tảng viết bằng Python](https://nicolargo.github.io/glances/)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062601.webp)

Ứng dụng CLI hỗ trợ theo dõi thông số CPU, RAM, ổ cứng và băng thông mạng hoạt động ổn định trên cả hệ điều hành Linux, Windows và macOS.

5、[XLite: Công cụ hỗ trợ nhập dữ liệu Excel vào SQLite nhanh chóng](https://github.com/x2bool/xlite)

Tiện ích cho phép nhà phát triển chuyển nhanh các tệp dữ liệu bảng tính Excel thành cơ sở dữ liệu SQLite cục bộ để thực hiện các truy vấn dữ liệu phức tạp bằng ngôn ngữ SQL.

6、[Jina: Framework Python hỗ trợ xây dựng hệ thống tìm kiếm neural search](https://github.com/jina-ai/jina)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081812.webp)

Bộ khung lập trình hỗ trợ thiết kế các tính năng tìm kiếm thông tin phi cấu trúc bằng công nghệ học sâu đối với hình ảnh, video, âm thanh (ví dụ: tìm kiếm màu son môi phù hợp dựa trên ảnh chụp khuôn mặt). (Đóng góp của [@Guanngxu](https://github.com/ruanyf/weekly/issues/2565))

7、[ITraffic-monitor-for-mac: Tiện ích giám sát lưu lượng mạng từng tiến trình trên macOS](https://github.com/foamzou/ITraffic-monitor-for-mac)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081813.webp)

Công cụ hỗ trợ đo đạc tốc độ tải lên/tải xuống thời gian thực của từng ứng dụng đang chạy trên máy Mac trực quan trên thanh Menu Bar. (Đóng góp của [@foamzou](https://github.com/foamzou))

8、[diskusage: Công cụ dòng lệnh phân tích dung lượng ổ đĩa đa nền tảng viết bằng Go](https://github.com/chenquan/diskusage)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081814.webp)

Tiện ích hỗ trợ quét hệ thống tập tin và biểu diễn dung lượng chiếm dụng của các thư mục dưới dạng đồ họa trực quan trên dòng lệnh. (Đóng góp của [@chenquan](https://github.com/chenquan))

9、[GitJournal: Ứng dụng ghi chú Markdown tự động đồng bộ lên Git từ xa](https://gitjournal.io/)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062906.webp)

Trình soạn thảo văn bản ghi chú định dạng Markdown trên điện thoại di động hỗ trợ tự động commit và push dữ liệu nhật ký trực tiếp lên repository cá nhân trên GitHub.

10、[Unpaywall: Extension Chrome tìm kiếm phiên bản PDF miễn phí của bài báo khoa học](https://unpaywall.org/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050706.webp)

Tiện ích mở rộng trình duyệt hỗ trợ phát hiện và hiển thị nút tải về tệp tin PDF mở (Open Access) của các bài báo khoa học trên các trang lưu trữ thu phí. (Bạn đọc cũng có thể tra cứu trực tiếp qua cơ sở dữ liệu [OA.mg](https://oa.mg/)).

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050705.webp)

## 活动

1、[Chương trình ưu đãi thẻ thành viên Juejin VIP](https://juejin.cn/vip?utm_source=ruanyifeng0819&utm_medium=gzh&utm_campaign=202207vip)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081811.webp)

Cộng đồng công nghệ稀土掘金 là diễn đàn chia sẻ kiến thức CNTT chất lượng trong nước. Ban quản trị vừa ra mắt gói thành viên "Juejin VIP" hỗ trợ mở khóa 90% các khóa học lập trình Front-end và cẩm nang phỏng vấn thực chiến chuyên sâu. Chương trình hiện đang áp dụng ưu đãi giảm giá 50% cho thành viên đăng ký sớm.

## 资源

1、[Learn Haskell by Building a Blog Generator (Học Haskell qua dự án tạo blog)](https://lhbg-book.link/)

Giáo trình trực tuyến tiếng Anh hướng dẫn chi tiết cú pháp và triết lý lập trình hàm của ngôn ngữ Haskell thông qua việc tự xây dựng một công cụ sinh trang web tĩnh.

2、[oPhysics: Trang web mô phỏng trực quan các thí nghiệm vật lý tương tác](https://ophysics.com/index.html)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081815.webp)

Thư viện sơ đồ thí nghiệm vật lý cho phép học sinh tương tác trực tiếp, thay đổi thông số lực, vận tốc để quan sát kết quả chuyển động mô phỏng trực quan. (Đóng góp của [@meq1986](https://github.com/ruanyf/weekly/issues/2570))

3、[treevis.net: Thư viện tổng hợp các giải pháp thiết kế trực quan hóa dữ liệu](https://treevis.net/)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060911.webp)

Trang web tổng hợp và phân loại hơn 300 mô hình trực quan hóa cấu trúc cây dữ liệu (tree data) phục vụ thiết kế sơ đồ quan hệ của dự án phần mềm.

4、[Unix Window Managers: Danh sách các bộ quản lý cửa sổ hiển thị cho Unix/Linux](https://www.gilesorr.com/wm/table.html)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061101.webp)

Trang web tổng hợp so sánh tính năng và dung lượng bộ nhớ của hơn 200 trình quản lý cửa sổ hiển thị (Window Manager) gọn nhẹ thay thế cho môi trường desktop mặc định của Linux.

5、[Understanding Quantum Technologies: Giáo trình nhập môn công nghệ điện toán lượng tử](https://www.oezratty.net/wordpress/2021/understanding-quantum-technologies-2021/)

Tài liệu điện tử tiếng Anh giới thiệu kiến thức vật lý lượng tử cơ bản, cấu trúc bóng bán dẫn lượng tử và hướng phát triển máy tính lượng tử dày hơn 800 trang có hình minh họa màu sắc.

## 图片

1\. [Khối đá đói cảnh báo nạn hạn hán lịch sử lộ diện tại sông Elbe](https://en.wikipedia.org/wiki/Hunger_stone)

Đợt nắng nóng kỷ lục mùa hè năm nay tại châu Âu làm suy giảm nghiêm trọng mực nước sông ngòi, làm lộ ra các khối "Đá đói" dưới lòng sông Elbe chảy qua Đức và Cộng hòa Séc:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081604.webp)

"Đá đói" (Hunger Stones) là các khối đá được tổ tiên khắc các thông điệp và dấu mốc thời gian cảnh báo nạn đói khi hạn hán xảy ra từ thế kỷ 15 đến 19, với lời nhắn gửi: *"Nếu bạn nhìn thấy khối đá này lộ diện, hãy khóc đi vì nạn đói sắp quay lại"*.

2\. [Các tác phẩm vẽ tranh động vật dạng điểm ảnh pixel của nghệ sĩ Nhật](https://kottke.org/22/03/pixel-birds-and-other-animals)

Tuyển tập các hình vẽ minh họa các loài chim và động vật dưới dạng pixel art phối màu độc đáo:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033105.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033106.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033107.webp)

3\. [Hình ảnh chú sóc New York giãn mình trên đất ẩm để giải nhiệt](https://www.washingtonpost.com/science/2022/08/12/splooting-squirrel-meaning-definition-new-york/)

Du khách tại công viên Trung tâm New York ghi lại hình ảnh những chú sóc nằm áp bụng áp sát cơ thể xuống mặt đất ẩm dưới bóng râm cồn cát:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081302.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081303.webp)

Ban quản lý công viên giải thích đây là tập tính sinh học bình thường (splooting) của loài sóc khi thời tiết quá nóng: chúng cố gắng kéo giãn tối đa thân người áp vào bề mặt đất mát lạnh để tăng diện tích tỏa nhiệt đối phó nắng nóng.

## 🏢 Tòa nhà không cửa sổ số 33 Thomas Street, New York

Vào thập niên 1960 của thời kỳ Chiến tranh Lạnh, Bộ Quốc phòng và hãng viễn thông AT&T quyết định xây dựng một tòa nhà chọc trời đặc biệt ngay giữa lòng thành phố New York với khả năng chống chịu sóng xung kích của một vụ nổ bom nguyên tử:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122205.webp)

Công trình cao 170 mét gồm 29 tầng nổi và 3 tầng hầm, được xây dựng hoàn toàn bằng các bức tường bê tông xám trần và không trang bị bất kỳ một cánh cửa sổ kính nào. Nếu xảy ra thảm họa hạt nhân, tòa nhà có đủ kho dự trữ lương thực và nhiên liệu phát điện độc lập để duy trì sự sống cho 1.500 người trong vòng hai tuần.

Mục tiêu cốt lõi của công trình không phải làm hầm trú ẩn cho người dân, mà là bảo vệ an toàn cho hệ thống máy tính điều phối và mạng lưới viễn thông quốc gia hoạt động liên tục sau vụ nổ hạt nhân.

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122207.webp)

Khởi công năm 1969 và hoàn thành năm 1974 tại địa chỉ số 33 phố Thomas,曼哈顿, tòa nhà là một khối bê tông xám khổng lồ sừng sững giữa phố phường nhộn nhịp. Khi màn đêm buông xuống, công trình trở thành một khối đen sẫm im lìm đặc biệt, chỉ có tiếng kêu rầm rì trầm đục từ hệ thống quạt thông gió vuông khổng lồ lắp đặt xung quanh vách tháp.

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122206.webp)

*(Tòa tháp bê tông không ánh sáng sừng sững giữa曼哈顿 về đêm)*

Ngoài các cửa thoát khí thông gió, lối ra vào duy nhất của tòa nhà là cổng kiểm soát an ninh nghiêm ngặt ở tầng trệt. 

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122208.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122209.webp)

Dựa trên các tài liệu rò rỉ của Edward Snowden, giới điều tra báo chí quốc tế đưa ra các phân tích chỉ ra tòa nhà số 33 Thomas Street thực chất là trung tâm nghe lén và thu thập thông tin viễn thông toàn cầu tuyệt mật mang bí danh TITANPOINTE do Cơ quan An ninh Quốc gia Mỹ (NSA) vận hành núp bóng trạm trung chuyển điện thoại đường dài của AT&T.

## 历史上的本周

- 2021年（第 171 期）：[Hạ tầng mạng: Phân tích cơ cấu và so sánh chi phí truyền tải băng thông (bandwidth fees) đắt đỏ của các nhà cung cấp dịch vụ đám mây](https://www.ruanyifeng.com/blog/2021/08/weekly-issue-171.html)
- 2020年（第 120 期）：[Tư duy công nghệ: Tại sao chỉ có tinh thần mở rộng hợp tác nguồn mở mới giúp phá bỏ hoàn toàn các rào cản cấm vận công nghệ](https://www.ruanyifeng.com/blog/2020/08/weekly-issue-120.html)
- 2019年（第 69 期）：[Thảo luận quản lý: Phân tích sự đánh đổi và lựa chọn ưu tiên giữa chất lượng hoàn thiện (Do it well) và tốc độ giao hàng (Do it fast) trong dự án phần mềm](https://www.ruanyifeng.com/blog/2019/08/weekly-issue-69.html)
- 2018年（第 18 期）：[An ninh quốc phòng: Những thách thức và giải pháp kỹ thuật phòng chống các cuộc tấn công khủng bố bằng thiết bị bay không người lái (UAV)](https://www.ruanyifeng.com/blog/2018/08/weekly-issue-18.html)

## 鸣谢

Nền tảng quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072108.webp)

（Hết）
