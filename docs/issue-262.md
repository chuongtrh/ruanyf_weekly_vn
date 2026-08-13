# Bản tin chia sẻ công nghệ (Số 262): Tạm biệt mật khẩu

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3222) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071309.webp)

Nếu thoạt nhìn, bạn có thể lầm tưởng đây là một đàn cừu đang lững thững gặm cỏ trên thảo nguyên rộng lớn. Tuy nhiên, thực chất đây là hệ thống kính thiên văn vô tuyến khổng lồ đặt tại sa mạc Atacama, Chile với tổng cộng 66 đĩa anten thu phát tín hiệu lớn, phần lớn trong số đó sở hữu đường kính 12 mét và chiều cao lên tới 15 mét. (Nguồn: [ESO](https://eso.org/public/images/potw2328a/))

## 告别密码

Trải nghiệm tồi tệ nhất khi chúng ta sử dụng mạng Internet hàng ngày chắc chắn chính là việc quản lý và gõ mật khẩu.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071203.webp)

Trải qua hơn 20 năm phát triển vũ bão của mạng Internet, hầu hết mọi quy trình và giao diện người dùng đều được nâng cấp cải thiện vượt bậc, ngoại trừ cơ chế mật khẩu bảo mật vẫn giữ nguyên phương thức hoạt động thô sơ của hai thập kỷ trước.

Nói một cách chính xác, trải nghiệm người dùng với mật khẩu thậm chí còn ngày một đi xuống. Yêu cầu về độ phức tạp và độ dài mật khẩu ngày càng tăng cao, thường bắt buộc không dưới 8 ký tự đi kèm chữ hoa, chữ thường và các ký tự đặc biệt. Thêm vào đó, để bảo mật tài khoản, người dùng thường xuyên phải thực hiện thêm các bước xác thực phụ phiền phức như nhập mã gửi qua tin nhắn SMS, nhận diện hình ảnh captcha hay nhập mã OTP thời gian thực.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071204.webp)

Điều đáng nói là dù quy trình có trở nên rắc rối đến mấy, nguy cơ tài khoản bị đánh cắp do lộ mật khẩu, bị hacker dò khóa hay bị tấn công giả mạo (phishing) vẫn luôn hiện hữu và không thể triệt tiêu hoàn toàn.

Suốt nhiều năm qua, giới công nghệ luôn nỗ lực tìm kiếm giải pháp tối ưu thay thế mật khẩu. Cho đến gần đây, một bước ngoặt lớn đã xuất hiện khi các tập đoàn công nghệ hàng đầu thế giới thống nhất được chuẩn xác thực chung thế hệ mới: **Đăng nhập bằng mã khóa truy cập, tên tiếng Anh gọi là Passkey**.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071205.webp)

Giải pháp Passkey cho phép người dùng đăng nhập tài khoản một cách an toàn mà không cần thiết lập hay ghi nhớ bất kỳ dòng mật khẩu nào, giải quyết triệt để các rủi ro bảo mật nêu trên với thao tác vô cùng dễ dàng và hiện đã nhận được sự hỗ trợ toàn diện từ các nền tảng hệ điều hành lớn.

Tại sự kiện WWDC 2022, [Apple chính thức công bố](https://developer.apple.com/passkeys/) hỗ trợ chuẩn Passkey trên hệ sinh thái của mình.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070801.webp)

Đến tháng 5 năm 2023, cả [Google](https://blog.google/technology/safety-security/the-beginning-of-the-end-of-the-password/) và [Microsoft](https://www.microsoft.com/en-us/security/blog/2023/05/04/how-microsoft-can-help-you-go-passwordless-this-world-password-day/) đều đồng loạt thông báo chính thức hỗ trợ và tích hợp toàn diện chuẩn Passkey vào các dịch vụ trực tuyến của mình.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071206.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070803.webp)

Hôm nay, tôi xin giải thích ngắn gọn về cơ chế hoạt động thực tế của giải pháp Passkey này:

Trên thực tế, các ứng dụng di động từ lâu đã triển khai phương thức "đăng nhập không mật khẩu" bằng cách cho phép người dùng chạm cảm biến vân tay hoặc quét khuôn mặt FaceID để truy cập nhanh tài khoản mà không cần gõ mật khẩu.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071207.webp)

Ý tưởng của Passkey là mở rộng cơ chế xác thực sinh trắc học tiện lợi này lên môi trường web: xây dựng một giao thức chuẩn hóa cho phép các trang web gọi trực tiếp phần cứng bảo mật sinh trắc học tích hợp trên thiết bị của người dùng để xác nhận danh tính, loại bỏ hoàn toàn mật khẩu.

Về mặt kỹ thuật, Passkey vận hành dựa trên cơ chế mã hóa bất đối xứng. **Trang web máy chủ không lưu trữ mật khẩu của người dùng nữa mà chỉ lưu giữ khóa công khai (Public Key)**. Khi người dùng thực hiện đăng nhập, hệ thống sẽ gửi một mã ngẫu nhiên yêu cầu người dùng sử dụng khóa riêng tư (Private Key) lưu trên thiết bị của mình để giải mã xác thực danh tính.

Cơ chế này đòi hỏi người dùng phải tự bảo quản khóa riêng tư của mình. Để đơn giản hóa tối đa quy trình cho người dùng phổ thông, giao thức Passkey yêu cầu sự tham gia của một **“Trình quản lý danh tính”** (thường do chính hệ điều hành như iOS, Android hoặc macOS cung cấp sẵn). Trình quản lý này sẽ tự động tạo và lưu trữ an toàn khóa riêng tư trong vùng nhớ bảo mật phần cứng của thiết bị.

Khi bạn đăng nhập vào một website yêu cầu xác thực bằng Passkey, trang web sẽ gửi yêu cầu tới Trình quản lý danh tính trên máy. Lúc này hệ thống sẽ hiển thị yêu cầu quét vân tay hoặc quét khuôn mặt trên điện thoại/máy tính của bạn để cấp quyền sử dụng khóa riêng tư hoàn tất đăng nhập. Đối với các dòng máy tính để bàn không tích hợp sẵn camera quét khuôn mặt hay cảm biến vân tay, trình duyệt sẽ tự động hiển thị mã QR để người dùng dùng điện thoại quét và xác thực qua kết nối Bluetooth.

Trình quản lý danh tính cũng có thể được lưu trữ trên các thiết bị phần cứng chuyên dụng độc lập kết nối qua cổng USB (như dòng khóa Yubikey), tuy nhiên phương án này đòi hỏi người dùng phải bỏ chi phí mua thêm phần cứng.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071208.webp)

Giao thức Passkey thực tế chứa đựng cấu trúc kỹ thuật mật mã khá phức tạp, nhưng đối với trải nghiệm thực tế của người dùng cuối, **nó vô cùng đơn giản và trực quan**: bạn chỉ cần chạm nhẹ vân tay hoặc nhìn vào camera thiết bị là tài khoản web đã được đăng nhập thành công. Bạn hoàn toàn có thể quên đi sự tồn tại của những dãy mật khẩu phức tạp trước đây.

Tôi dự báo chỉ trong vòng 1-2 năm tới, đi kèm sự ra đời của các thư viện mã nguồn mở và bộ khung phát triển đóng gói sẵn hỗ trợ tích hợp nhanh, chuẩn xác thực Passkey sẽ nhanh chóng phủ sóng rộng rãi và đẩy lùi kỷ nguyên sử dụng mật khẩu truyền thống.

Hiện tại bạn đọc có thể truy cập trang trải nghiệm [Passkeys.io](https://passkeys.io) để trực tiếp dùng thử quy trình đăng nhập không mật khẩu, hoặc tìm hiểu sâu hơn về mặt kỹ thuật thông qua các tài liệu tham khảo chất lượng sau: [SlashID Passkeys Security](https://www.slashid.dev/blog/passkeys-security-implementation/), [CSS-Tricks Passkeys Overview](https://css-tricks.com/passkeys-what-the-heck-and-why/), [Clearing up Passkeys Misconceptions](https://www.stavros.io/posts/clearing-up-some-passkeys-misconceptions/).

## 科技动态

1、[Phần Lan ra mắt dòng sản phẩm bồn cầu độc đáo chế tạo hoàn toàn từ mùn cưa](https://www.dezeen.com/2023/03/22/woodio-wood-composite-toilet/)

Một doanh nghiệp thiết kế thiết bị vệ sinh tại Phần Lan vừa qua đã công bố dòng sản phẩm bồn cầu thế hệ mới với toàn bộ cấu trúc từ bệ ngồi cho đến phần chân đế đều được sản xuất từ nguyên liệu mùn cưa ép:

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032910.webp)

Hãng đã nghiên cứu pha trộn mùn cưa gỗ tự nhiên cùng chất kết dính nhựa resin đặc biệt để tạo ra loại vật liệu composite siêu bền, chịu lực tốt và có khả năng chống thấm nước tuyệt đối. So với quy trình nung sứ truyền thống vốn tiêu thụ lượng nhiệt năng cực lớn, việc sản xuất bồn cầu từ mùn cưa giúp cắt giảm phần lớn lượng khí thải CO2 ra môi trường, đồng thời mang lại trọng lượng siêu nhẹ cho sản phẩm.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032909.webp)

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032911.webp)

Doanh nghiệp cho biết đang tiếp tục phát triển và sớm đưa ra thị trường các dòng sản phẩm bồn rửa mặt và bồn tắm làm từ chất liệu gỗ composite thân thiện với môi trường này.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032908.webp)

2、[Trò đùa đặt chóp nón giao thông làm tê liệt hoạt động của các xe taxi tự lái](https://www.thedrive.com/news/rebels-are-disabling-waymo-cruise-robotaxi-with-traffic-cones)

Sau khi chính quyền thành phố San Francisco cấp phép cho các hãng xe tự lái (như Cruise hay Waymo) triển khai dịch vụ taxi không người lái thương mại trên đường phố, một số người dân phản đối đã phát hiện ra một lỗ hổng thiết kế hài hước của hệ thống:

Theo các video chia sẻ trên mạng xã hội, chỉ cần người đi đường đặt một chiếc chóp nón cảnh báo giao thông bằng nhựa lên trên nắp capo của xe tự lái (hình dưới), cảm biến LiDAR của xe sẽ lập tức nhận diện đây là chướng ngại vật khẩn cấp sát thân xe và ra lệnh cho xe dừng hoạt động ngay lập tức kể cả khi đang đỗ giữa ngã tư đông đúc:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070704.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070703.webp)

Lỗi logic này hiện được cho là rất khó khắc phục triệt để bằng phần mềm vì xe bắt buộc phải ưu tiên dừng lại để bảo đảm an toàn khi phát hiện vật cản che khuất tầm nhìn cảm biến. Sự việc cho thấy những thách thức lớn mà xe tự lái phải đối mặt khi xử lý các hành vi cố tình phá hoại từ con người ngoài đời thực.

3、[Ghi nhận những ngày có nhiệt độ trung bình toàn cầu cao nhất trong lịch sử khí tượng](https://apnews.com/article/global-record-breaking-heat-july-27069b5380117534d78f1f40a6edc7a0)

Mô hình phân tích khí hậu toàn cầu của Đại học Maine, Mỹ thu thập dữ liệu thời gian thực từ các trạm khí tượng mặt đất kết hợp ảnh vệ tinh đã đưa ra báo cáo đáng lo ngại về tình hình ấm lên của Trái Đất:

Theo đó, ngày 6 tháng 7 vừa qua đã được xác nhận là ngày có nhiệt độ trung bình toàn cầu cao nhất từng được ghi nhận trong lịch sử khí tượng với mức nhiệt đạt **17,23 độ C**. Đáng ngại hơn, các vị trí xếp thứ hai và thứ ba về nắng nóng kỷ lục cũng vừa được thiết lập ngay trước đó vào ngày 5 và ngày 4 tháng 7.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071105.webp)

Biểu đồ nhiệt độ lịch sử (hình trên) cho thấy đường biểu diễn nhiệt độ của năm 2023 (đường màu đen đậm) đã có sự bứt phá vượt hẳn lên so với tất cả các năm trước đó ngay từ đầu tháng 6.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071106.webp)

Bản đồ phân bổ nhiệt độ bề mặt Trái Đất (hình trên) cho thấy hầu hết các khu vực thuộc vĩ độ thấp và trung bình đều đang bị bao trùm bởi sắc đỏ nhiệt độ cao cực đoan, ngoại trừ các khu vực cao nguyên có địa hình cao.

4、[Las Vegas khánh thành công trình kiến trúc hình cầu tích hợp màn hình LED khổng lồ nhất thế giới](https://edition.cnn.com/2023/07/05/travel/msg-sphere-las-vegas-venue-cec/index.html)

Tại khu resort khách sạn Venetian ở Las Vegas mới đây đã khánh thành một khu nhà hát biểu diễn nghệ thuật vô cùng độc đáo mang tên MSG Sphere:

Đây được ghi nhận là công trình kiến trúc hình cầu có quy mô lớn nhất thế giới với chiều cao 111 mét và chiều rộng lên tới 516 mét:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071107.webp)

Toàn bộ bề mặt cong bên ngoài của khối cầu được phủ kín bởi hàng triệu bóng đèn LED tạo thành một màn hình hiển thị khổng lồ, cho phép trình chiếu các hoạt ảnh chuyển động 3D sống động vào ban đêm thu hút sự chú ý cực lớn của du khách:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071108.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071109.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071110.webp)

Phía trong công trình là một khán đài hình vòm hiện đại sức chứa hàng vạn chỗ ngồi phục vụ tổ chức các giải đấu thể thao và các show diễn âm nhạc đỉnh cao:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071111.webp)

Mặc dù nhanh chóng trở thành biểu tượng du lịch mới của thành phố, công trình khổng lồ này cũng nhận về những phản hồi trái chiều từ các nhà bảo vệ môi trường do mức tiêu thụ năng lượng điện cực lớn và nguy cơ gây ô nhiễm ánh sáng nghiêm trọng cho khu vực dân cư xung quanh vào ban đêm.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071112.webp)

## Bài viết

1\. [Thảo luận về tính chính xác của thuật ngữ dịch nghĩa từ “Tiến hóa”](https://mp.weixin.qq.com/s/5fF7o8EePoIhqZ4x0KrTaQ)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070511.webp)

Bài phân tích ngôn ngữ học và sinh học thảo luận về việc thuật ngữ khoa học "Evolution" trong tiếng Trung có nên được dịch thống nhất là "Diễn hóa" thay vì "Tiến hóa" như trước đây hay không. Dưới góc nhìn sinh học hiện đại, các sinh vật biến đổi cấu trúc gen chủ yếu nhằm mục đích thích nghi với sự thay đổi của môi trường sống xung quanh (diễn hóa) chứ không nhất thiết là sự phát triển tiến bộ đi lên (tiến hóa).

2\. [Chia sẻ kinh nghiệm tự khởi nghiệp và vận hành công ty SaaS một thành viên hướng ra thị trường quốc tế](https://mp.weixin.qq.com/s/x6PLSIMn_1qcKnXWPT-J-Q)（Tiếng Trung）

Tác giả chia sẻ chi tiết chặng đường thực tế của một lập trình viên tự mình nghiên cứu sản phẩm, hoàn thiện các thủ tục pháp lý để đăng ký thành lập doanh nghiệp công nghệ dạng SaaS một thành viên hướng tới tệp khách hàng quốc tế để tối ưu hóa nguồn thu cá nhân.

3\. [Cảnh báo tình trạng ứng dụng tivi thông minh chạy ngầm chiếm dụng băng thông của người dùng](https://news.mydrivers.com/1/922/922097.htm)（Tiếng Trung）

Nhiều người dùng phát hiện ra ứng dụng xem video iQiyi phiên bản dành cho tivi thông minh (TV App) dù đã được tắt màn hình vẫn âm thầm chạy ngầm liên tục tải dữ liệu lên (upload) với tốc độ cao, chỉ dừng lại khi rút nguồn điện tivi. Phần mềm đã tự ý cấu hình biến thiết bị của khách hàng thành một nút CDN đệm để tiết kiệm chi phí băng thông đường truyền cho hãng.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071201.webp)

4\. [Bài viết phân tích so sánh chi tiết giữa hai cơ sở dữ liệu PostgreSQL và MySQL phiên bản năm 2023](https://mp.weixin.qq.com/s/xf7qb4oAVHyi4_U32FSKPA)（Tiếng Trung）

PostgreSQL và MySQL hiện là hai hệ quản trị cơ sở dữ liệu quan hệ nguồn mở phổ biến nhất thế giới. Bài viết so sánh chi tiết các tính năng tối ưu hóa truy vấn, cấu trúc chỉ mục, khả năng mở rộng hệ thống và độ tin cậy dữ liệu của hai cơ sở dữ liệu này trong bối cảnh phát triển hiện nay. (Đóng góp của [@milasuperstar](https://github.com/ruanyf/weekly/issues/3269))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071318.webp)

5\. [Hướng dẫn phân tích nguyên lý và giải thuật tự động vượt qua ảnh trượt xác thực](https://mp.weixin.qq.com/s/iK_JkVRrh5vIRBjnQbDOyw)（Tiếng Trung）

Bài viết giới thiệu cơ chế lập trình và các bước xử lý hình ảnh của hệ thống mã xác thực dạng trượt (Slider Captcha), đồng thời hướng dẫn cách ứng dụng các thuật toán nhận diện hình ảnh để tính toán khoảng cách trượt tự động nhằm tối ưu hóa quy trình kiểm thử phần mềm. (Đóng góp của [@niumoo](https://github.com/ruanyf/weekly/issues/3266))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071316.webp)

6\. [Hướng dẫn tối ưu hóa chất lượng hình ảnh mã QR nghệ thuật được sinh bởi AI](https://antfu.me/posts/ai-qrcode-refine)（Tiếng Anh）

Nhà phát triển nổi tiếng Anthony Fu chia sẻ quy trình tinh chỉnh kỹ thuật để nhúng mã QR vào bên trong các bức tranh nghệ thuật do AI sinh ra, sao cho bức tranh trông tự nhiên và có thẩm mỹ tốt đối với người xem nhưng vẫn bảo đảm cấu trúc tương phản giúp các ứng dụng quét mã nhận diện nhanh chóng. (Đóng góp của [@POKEZHANG](https://github.com/ruanyf/weekly/issues/3247))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071313.webp)

7\. [Những quan ngại kỹ thuật xoay quanh cơ chế React Server Components mới](https://marmelab.com/blog/2023/06/05/react-angularjs-moment.html)（Tiếng Anh）

React đang tích cực thúc đẩy việc áp dụng mô hình kết xuất linh kiện phía máy chủ (React Server Components - RSC). Tác giả bài viết bày tỏ những lo ngại về việc thay đổi kiến trúc lớn này sẽ làm vô hiệu hóa nhiều thư viện bổ trợ và phương thức viết code React truyền thống của các lập trình viên Front-end.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060701.webp)

8\. [Các trình duyệt hiện đại chính thức hỗ trợ cơ chế ánh xạ module Import Maps](https://web.dev/import-maps-in-all-modern-browsers/)（Tiếng Anh）

Trước đây khi nạp các module JS trực tiếp trên trình duyệt, lập trình viên bắt buộc phải điền đường dẫn URL đầy đủ. Bài viết giới thiệu tính năng Import Maps hiện đã được hỗ trợ đồng loạt trên các trình duyệt lớn, cho phép trình duyệt tự động phân giải và nạp module trực tiếp từ tên gọi tương tự như môi trường Node.js.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050302.webp)

9\. [Phân tích thế cuộc cạnh tranh dịch vụ điện toán đám mây toàn cầu giữa Mỹ và Trung Quốc](https://interconnected.blog/us-vs-china-a-cloud-proxy-war/)（Tiếng Anh）

Trong bối cảnh chính phủ Mỹ xem xét các biện pháp hạn chế các nhà cung cấp đám mây Trung Quốc hoạt động tại thị trường nội địa, bài viết phân tích chi tiết chiến lược cạnh tranh giành thị phần hạ tầng đám mây đang diễn ra gay gắt giữa hai bên tại các khu vực đang phát triển như Đông Nam Á, Trung Đông và Mỹ Latinh.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070510.webp)

## 工具

1、[Connect-Web: Thư viện TypeScript gọi RPC trực tiếp từ trình duyệt](https://connect.build/)

Một thư viện TypeScript tiện lợi cho phép lập trình viên Front-end gọi trực tiếp các dịch vụ chạy giao thức gRPC hoặc Protocol Buffers từ trình duyệt web mà không cần cấu hình thêm lớp trung gian phức tạp. (Xem thêm [Bài viết giới thiệu chi tiết](https://buf.build/blog/connect-web-protobuf-grpc-in-the-browser)).

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080504.webp)

2、[xBrowserSync: Tiện ích đồng bộ hóa dấu trang trình duyệt mã nguồn mở bảo mật](https://www.xbrowsersync.org/)

Extension trình duyệt hỗ trợ đồng bộ hóa bookmark (dấu trang) cá nhân giữa nhiều trình duyệt khác nhau (ví dụ đồng bộ giữa Chrome trên điện thoại Android và Firefox trên máy tính) với cơ chế mã hóa dữ liệu đầu cuối bảo mật tuyệt đối.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122212.webp)

3、[I Don't Care About Commit Message: Extension VS Code tự động tạo mô tả commit](https://github.com/mefengl/vscode-i-dont-care-about-commit-message)

Tiện ích mở rộng dành cho VS Code kết nối với API của OpenAI để tự động phân tích những thay đổi trong mã nguồn vừa sửa đổi và tự động soạn thảo nội dung commit ngắn gọn, giúp lập trình viên tiết kiệm thời gian viết log. (Đóng góp của [@mefengl](https://github.com/ruanyf/weekly/issues/3248))

4、[React1s: Tiện ích hỗ trợ nhảy nhanh đến dòng code định nghĩa linh kiện React từ web](https://github.com/aaamoon/react1s)

Extension hữu ích dành cho lập trình viên phát triển React chạy local: người dùng chỉ cần nhấp chuột vào một phần tử giao diện bất kỳ trên trình duyệt, công cụ sẽ tự động kích hoạt IDE để mở đúng tệp mã nguồn và di chuyển con trỏ tới dòng code định nghĩa phần tử đó. (Đóng góp của [@aaamoon](https://github.com/ruanyf/weekly/issues/3268))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071317.webp)

5、[TGSCAN: Công cụ tìm kiếm dữ liệu nguồn mở dành riêng cho Telegram](https://github.com/tgscan-dev/tgscan)

Dự án phát triển công cụ tìm kiếm dữ liệu mã nguồn mở hỗ trợ thu thập và lập chỉ mục tìm kiếm thông tin các kênh chat công khai trên ứng dụng Telegram. (Đóng góp của [@HandelDev](https://github.com/ruanyf/weekly/issues/3263))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071314.webp)

6、[LeaferJS: Engine kết xuất đồ họa Canvas 2D siêu nhẹ hiệu năng cao](https://www.leaferjs.com/)

Một thư viện kết xuất đồ họa Canvas 2D do các kỹ sư trong nước tự phát triển, hướng tới mục tiêu tối ưu hóa tốc độ vẽ đồ họa vector mượt mà và tiết kiệm tối đa dung lượng bộ nhớ. (Đóng góp của [@leaferjs](https://github.com/ruanyf/weekly/issues/3246))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071312.webp)

7、[AltTab: Mang tính năng chuyển đổi cửa sổ Alt+Tab của Windows lên macOS](https://github.com/lwouis/alt-tab-macos)

Ứng dụng nhỏ gọn dành cho người dùng hệ điều hành macOS, giả lập hoàn hảo tính năng và giao diện xem trước hình thu nhỏ khi chuyển đổi nhanh các cửa sổ ứng dụng bằng phím tắt Alt + Tab của hệ điều hành Windows.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051203.webp)

8、[rsync-time-backup: Công cụ sao lưu dữ liệu gia tăng theo thời gian qua dòng lệnh](https://github.com/laurent22/rsync-time-backup)

Một tập lệnh Shell tiện lợi hỗ trợ lập trình viên thực hiện sao lưu gia tăng (incremental backup) các thư mục dữ liệu trên máy tính tương tự như công cụ Time Machine của Apple, hỗ trợ khôi phục thư mục về trạng thái tại bất kỳ mốc thời gian nào trong quá khứ.

9、[XState: Thư viện quản lý trạng thái dựa trên mô hình máy trạng thái hữu hạn](https://xstate.js.org/)

Thư viện JavaScript mạnh mẽ giúp lập trình viên quản lý trạng thái của ứng dụng phức tạp một cách khoa học bằng cách áp dụng mô hình toán học Máy trạng thái hữu hạn (Finite State Machine).

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051501.webp)

10、[hat-syslog: Ứng dụng giao diện đồ họa quản trị log hệ thống Linux Syslog](https://github.com/hat-open/hat-syslog)

Phần mềm mã nguồn mở cung cấp giao diện đồ họa trực quan hỗ trợ các kỹ sư quản trị hệ thống Linux dễ dàng theo dõi, lọc tìm kiếm và phân tích các tệp tin nhật ký hệ thống Syslog.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051602.webp)

## 资源

1、[US Radio Spectrum Allocation Chart: Sơ đồ phân phối tần số vô tuyến tại Mỹ](https://www.beautifulpublicdata.com/the-united-states-radio-frequency-allocation-chart/)

Trang web giới thiệu và cung cấp liên kết tải về tệp tin [Bản đồ PDF chất lượng cao](https://ntia.gov/sites/default/files/publications/january_2016_spectrum_wall_chart_0.pdf) trực quan hóa toàn bộ việc phân bổ tần số sóng vô tuyến từ tần số thấp đến siêu cao phục vụ các mục đích viễn thông, hàng hải, hàng không và quân sự của chính phủ Mỹ.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020809.webp)

2、[Oak BYO: Giáo trình tự học cách tự viết lại các thư viện React và Redux](https://nytimes.github.io/oak-byo-react-prosemirror-redux/)

Bộ giáo trình huấn luyện kỹ thuật nội bộ của tòa soạn báo *The New York Times*, hướng dẫn chi tiết từng bước cho các lập trình viên mới cách thức tự viết mã xây dựng lại các phiên bản thu nhỏ của thư viện React, ProseMirror và Redux từ con số không để thấu hiểu sâu sắc nguyên lý hoạt động của chúng.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020811.webp)

3、[StockAI.Trade: Công cụ AI hỗ trợ phân tích lọc cổ phiếu thị trường A-share](https://stockai.trade/)

Ứng dụng web tích hợp API của ChatGPT hỗ trợ các nhà đầu tư phân tích nhanh báo cáo tài chính và đưa ra các đánh giá phân tích kỹ thuật lọc mã cổ phiếu trên thị trường chứng khoán Trung Quốc. (Đóng góp của [@yvonuk](https://github.com/ruanyf/weekly/issues/3265))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071315.webp)

4、[GifCities: Thư viện công cụ tìm kiếm và lưu trữ kho ảnh GIF động cổ](https://gifcities.org/)

Dự án lưu trữ phi lợi nhuận Internet Archive đã tiến hành thu thập và bảo tồn toàn bộ kho hình ảnh động GIF dạng pixel cổ từ thời kỳ sơ khai của mạng Internet trên nền tảng GeoCities huyền thoại, cung cấp công cụ tìm kiếm tiện lợi cho người dùng.

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082303.webp)

5、[FlagWaver: Trang web giả lập hiệu ứng lá cờ bay trong gió trực quan](https://krikienoid.github.io/flagwaver/)

Ứng dụng Web sử dụng thư viện đồ họa 3D để mô phỏng chân thực chuyển động của một lá cờ đang bay trong gió. Người dùng có thể tải lên bức ảnh bất kỳ của mình làm hình ảnh lá cờ và tùy chỉnh các thông số sức gió, hướng gió.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111201.webp)

## 图片

1、**Hồi cứu sự cố tai nạn hàng không thoát hiểm kỳ diệu của chuyến bay United Airlines 811**

Vào ngày 24 tháng 2 năm 1989, chiếc máy bay Boeing 747 thực hiện chuyến bay mang số hiệu UA811 di chuyển từ Los Angeles đi Sydney, Úc đã gặp sự cố nghiêm trọng sau khi vừa cất cánh từ điểm dừng chân trung chuyển tại Hawaii được 17 phút:

Một tiếng nổ lớn vang lên từ phần thân dưới do cánh cửa khoang hành lý phía trước bị bung ra hoàn toàn dưới áp suất chênh lệch ở độ cao lớn:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011710.webp)

Sức ép chênh lệch áp suất cực lớn đã lập tức giật bay một mảng lớn thân máy bay, cuốn trôi 5 hàng ghế khoang hành khách và hút thẳng 9 hành khách đang ngồi tại khu vực đó ra ngoài không trung:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011711.webp)

Cả 9 hành khách trên đều tử nạn. Báo cáo điều tra chỉ ra có một hành khách (mũi tên ngoài cùng bên trái hình trên) ngồi ở vị trí dãy ghế phía bên kia lối đi không thuộc khu vực vỡ thân máy, nhưng do anh không thắt dây an toàn nên đã bị luồng khí mạnh hút bay ra ngoài, nếu thắt dây an toàn thì cơ hội sống sót của anh là rất lớn.

Hình ảnh dưới đây ghi lại khoảnh khắc hỗn loạn bên trong khoang hành khách ngay sau sự cố: mặt nạ dưỡng khí rơi xuống nhưng hoàn toàn không có khí oxy do đường ống dẫn khí đã bị đứt nát, tiếng gió rít gào lùa qua lỗ hổng thân máy bay tạo ra tiếng ồn cực lớn:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011712.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011713.webp)

Dù hai động cơ một bên cánh đã hỏng hoàn toàn do hút phải các mảnh vỡ thân máy, cơ trưởng và tổ lái đã vô cùng bình tĩnh điều phối thiết bị bay vòng trở lại hạ cánh khẩn cấp an toàn xuống sân bay Hawaii, cứu sống toàn bộ các hành khách còn lại:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011714.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011715.webp)

Kết quả điều tra xác định nguyên nhân tai nạn do lỗi thiết kế của hệ thống khóa cửa điện trên dòng máy bay Boeing 747 thời kỳ đó, khiến mô tơ khóa tự động kích hoạt mở chốt do rò rỉ điện trong lúc bay.

Sau sự cố thảm khốc này, toàn bộ thiết kế khóa cửa khoang hành lý của dòng Boeing 747 đã được cải tiến thay thế từ dạng mở quay ra ngoài sang cơ chế mở trượt vào trong. Với thiết kế mở vào trong, khi máy bay lên cao, chênh lệch áp suất lớn trong khoang sẽ tự động ép chặt cánh cửa vào khung và ngăn không cho cửa có thể tự mở ra, loại bỏ hoàn toàn nguy cơ xảy ra tai nạn tương tự sau này.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011716.webp)

## ✍️ Bài đọc thêm

### Ba nguyên tắc cốt lõi để xây dựng hệ thống ghi chép ghi chú hiệu quả

Để xây dựng một hệ thống lưu trữ kiến thức cá nhân thực sự mang lại hiệu quả lâu dài, bạn nên tuân thủ 3 nguyên tắc nền tảng sau:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071319.webp)

**1. Ghi chép phải tương thích với cấu trúc tư duy tự nhiên của bạn**

Khi thực hiện ghi chép một kiến thức mới, bạn bắt buộc phải biên soạn lại thông tin theo đúng cách suy nghĩ và liên kết logic của cá nhân mình, tuyệt đối không được chép nguyên văn cách trình bày của giáo viên hay sách giáo khoa. Cách làm này giúp bạn viết thông tin thoải mái hơn, và quan trọng nhất là khi mở ra đọc lại sau này, bạn dễ dàng bắt nhịp lại mạch suy nghĩ của mình lúc đó.

**2. Ghi chú phải đại diện cho vốn tri thức thực tế của bạn**

Hãy từ bỏ thói quen copy-paste hàng loạt các đoạn văn bản dài của người khác vào sổ ghi chép. Hãy tập diễn đạt lại kiến thức đó bằng chính ngôn ngữ viết của mình. Đồng thời, bạn nên đánh dấu rõ ràng những phần bản thân đã thấu hiểu hoàn toàn, và những điểm còn mơ hồ cần nghiên cứu thêm để tiện theo dõi tiến độ học tập.

**3. Hệ thống ghi chú phải dễ dàng tra cứu nhanh khi cần**

Để tối ưu hóa giá trị của kho tri thức cá nhân và tiết kiệm thời gian, bạn bắt buộc phải tổ chức lưu trữ sao cho việc tìm kiếm thông tin diễn ra nhanh nhất. Hãy luôn đặt tiêu đề rõ ràng, mạch lạc cho từng phần ghi chép nhỏ và duy trì thói quen định kỳ tổng hợp xây dựng một trang mục lục liên kết để tiện tra cứu.

## Lịch sử tuần này

- 2022年（第 215 期）：[Lối sống số: Phân tích các mô hình hành vi tương tác được ưa chuộng nhất trên môi trường Internet](http://www.ruanyifeng.com/blog/2022/07/weekly-issue-215.html)
- 2021年（第 165 期）：[Xu hướng ứng dụng: Kỷ nguyên trỗi dậy của các dòng ứng dụng chạy mượt mà trên đa nền tảng phần cứng](http://www.ruanyifeng.com/blog/2021/07/weekly-issue-165.html)
- 2020年（第 115 期）：[Bảo mật thông tin: Cảnh báo tầm quan trọng của việc bảo vệ dữ liệu giải mã gen DNA cá nhân](http://www.ruanyifeng.com/blog/2020/07/weekly-issue-115.html)
- 2019年（第 65 期）：[Thông tin dịch vụ: Bản tin chính thức thử nghiệm chuyên mục hỗ trợ tuyển dụng nhân sự công nghệ](http://www.ruanyifeng.com/blog/2019/07/weekly-issue-65.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes organizing and collaborative work seamless.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
