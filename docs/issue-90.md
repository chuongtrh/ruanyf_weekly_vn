# 科技爱好者周刊：第 90 期 (Bản tin chia sẻ công nghệ số 90)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

Mục tuyển dụng [《Ai đang tuyển dụng?》](https://github.com/ruanyf/weekly/issues/983) cung cấp nhiều thông tin việc làm hữu ích, hoan nghênh ghé thăm hoặc đăng tải thông tin tuyển dụng/thực tập.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120604.jpg)

Ảnh bìa: Nhà hàng giữa lòng sa mạc, Dubai, UAE. Ảnh từ [Instagram](https://www.instagram.com/p/B5s4DSkBAKE/).

## 刊首语 (Lời tựa)

Sau một thời gian dài làm việc trong ngành lập trình, nếu dự án tiến triển thuận lợi, các lập trình viên thường sẽ có cơ hội xây dựng hoặc tiếp quản đội ngũ kỹ sư của riêng mình để bắt đầu chuyển dịch sang vai trò quản lý con người.

Tuy nhiên, việc quản lý con người thực tế lại khó khăn hơn rất nhiều so với lập trình kỹ thuật. Công nghệ là bất động và logic, còn con người lại sống động, phức tạp và liên tục thay đổi. Việc có thể gắn kết mọi thành viên lại với nhau, cùng chung sức hướng về một mục tiêu chung là điều vô cùng thách thức.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020010903.jpg)

Rất nhiều lập trình viên kinh nghiệm mà tôi quen biết đều bày tỏ sự e ngại và không muốn đảm nhận công việc quản lý. Một người bạn sáng lập studio lập trình chia sẻ rằng trong những năm qua, doanh nghiệp của anh đã có nhiều cơ hội để mở rộng quy mô nhưng anh đều chủ động từ chối, bởi anh hoàn toàn không biết cách làm thế nào để quản trị nhân sự hiệu quả. **Anh ấy bộc bạch: "Mình có thể quản lý rất tốt bản thân, nhưng lại hoàn toàn bế tắc khi phải quản lý người khác."**

Trước hết, hoạt động tuyển dụng nhân sự mới và sa thải nhân sự không phù hợp là những đầu việc vô cùng phức tạp và nhạy cảm. Tiếp đó, việc đánh giá hiệu suất (KPI), phân chia quỹ thưởng rất dễ phát sinh mâu thuẫn nội bộ. Chỉ cần một nhân sự trong nhóm nảy sinh tâm lý bất mãn, sự lục đục nội bộ sẽ lập tức ảnh hưởng đến tiến độ của dự án. Trong các tình huống cực đoan, nếu xảy ra sự cố phá hoại hệ thống (như xóa cơ sở dữ liệu rồi bỏ trốn), đó sẽ là đòn giáng chí mạng vào doanh nghiệp.

![](https://cdn.beekka.com/blogimg/asset/202001/bg2020010904.jpg)

Điểm mạnh vượt trội của những nhà lãnh đạo lỗi lạc như Jack Ma hay Nhậm Chính Phi nằm ở đâu? Đó hoàn toàn không phải là năng lực kỹ thuật gõ code, mà là tư duy quản trị tổ chức và tầm nhìn thị trường xuất sắc. Họ cực kỳ giỏi trong việc quản lý và gắn kết các tổ chức quy mô lớn. Nhậm Chính Phi từng khiêm tốn nhận xét: "Năng lực lớn nhất của tôi là đóng vai trò như một hũ hồ dán, giúp kết dính hàng vạn con người tài năng lại thành một khối thống nhất."

Do đó, các lập trình viên nên có sự tự nhận thức rõ ràng về bản thân: quản lý con người và nghiên cứu kỹ thuật là hai loại năng lực hoàn toàn khác nhau. Nếu nhận thấy bản thân không phù hợp với việc giao tiếp xã hội, bạn không nên gượng ép nhận các vị trí quản lý; nếu tham gia khởi nghiệp, bạn nên tìm kiếm những nhà quản trị chuyên nghiệp để vận hành doanh nghiệp.

Ngược lại, đối với những người sáng lập không có nền tảng công nghệ chuyên sâu nhưng sở hữu năng lực quản trị xuất sắc, bạn hoàn toàn có thể tìm kiếm các đồng đội lập trình giỏi để cùng đồng hành khởi nghiệp công nghệ.

## Dịch vụ giải mã mã xác thực tự động 2Captcha

Hầu hết các trang web hiện nay đều trang bị các hệ thống mã xác thực (Captcha) ở cổng đăng nhập nhằm ngăn chặn hoạt động của các bot và kịch bản đăng nhập tự động. Có rất nhiều loại Captcha khác nhau, phổ biến nhất là nhận diện ký tự biến dạng (ảnh dưới) - những ký tự được làm méo mó mà máy tính khó lòng nhận dạng chính xác nhưng con người lại dễ dàng đọc được.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019123001.jpg)

Để phục vụ nhu cầu thu thập dữ liệu web (cào web) hoặc vận hành các kịch bản mua hàng nhanh (giật đơn hàng), các dịch vụ giải mã Captcha tự động đã ra đời. Mới đây, đơn vị vận hành dịch vụ [2Captcha](https://2captcha.com?from=8377663) đã liên hệ và mong muốn giới thiệu dịch vụ tới cộng đồng lập trình viên Việt Nam. Được thành lập từ năm 2013 và vận hành ổn định trong suốt nhiều năm qua, 2Captcha là một trong những nhà cung cấp dịch vụ giải mã Captcha uy tín hàng đầu trên thị trường quốc tế.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019123002.jpg)

Điểm độc đáo lớn nhất của [2Captcha](https://2captcha.com?from=8377663) là khả năng giải quyết chính xác mọi loại Captcha có độ khó cao (bao gồm cả ReCaptcha của Google) nhờ ứng dụng mô hình [真人识别 (giải mã bằng người thật)](https://2captcha.com/make-money-online?from=8377663). Nền tảng tuyển dụng cộng tác viên giải mã Captcha trực tuyến từ khắp nơi trên thế giới (chủ yếu từ các nước như Ấn Độ, Nga, Venezuela, Philippines), đảm bảo luôn có đủ nhân sự trực tuyến 24/7 ở mọi múi giờ để xử lý yêu cầu.

Các nhà phát triển chỉ cần gửi hình ảnh Captcha thông qua cổng API của 2Captcha, hệ thống sẽ chuyển đến cộng tác viên để nhập kết quả thủ công. Thời gian xử lý trung bình chỉ mất từ 12 đến 14 giây. Mức phí của dịch vụ vô cùng rẻ, chỉ từ 0.5 USD cho 1.000 lượt giải mã thành công (hỗ trợ thanh toán tiện lợi qua nhiều cổng thanh toán quốc tế), và cam kết hoàn tiền nếu giải mã sai kết quả.

Bên cạnh Captcha ký tự thông thường, dịch vụ còn hỗ trợ giải mã các dạng Captcha chọn ảnh phức tạp, chi tiết tham khảo tại tài liệu hướng dẫn [API Docs](https://2captcha.com/2captcha-api?from=8377663) của hãng. Bộ phận kỹ thuật của hãng cũng sẵn sàng cung cấp các giải pháp hỗ trợ kết nối trực tiếp cho các nhà phát triển.

Nền tảng cũng cung cấp chương trình tiếp thị liên kết (Affiliate Program) hấp dẫn: chiết khấu từ 5% đến 10% doanh số cho người giới thiệu dịch vụ, hoặc 10% doanh thu nếu bạn tích hợp trực tiếp API của 2Captcha vào sản phẩm phần mềm thương mại của mình.

## 资讯 (Tin tức)

1. **Chuẩn bị bãi bỏ định nghĩa đơn vị đo lường US Survey Foot để thống nhất chuẩn quốc tế**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121710.jpg)

Như đã biết, nước Mỹ vẫn duy trì hệ đo lường Anh-Mỹ thay vì chuyển sang hệ mét tiêu chuẩn quốc tế. Tuy nhiên, một thực tế ít người biết là ngay tại Mỹ cũng tồn tại hai định nghĩa khác nhau cho đơn vị đo độ dài "Foot" (bằng Anh).

Từ năm 1893, chính phủ Mỹ quy định 1 US Survey Foot bằng 1200/3937 mét (khoảng 0.3048006 mét). Trong khi đó, định nghĩa chuẩn quốc tế (International Foot) được thống nhất là 0.3048 mét. Sự chênh lệch vô cùng nhỏ ở chữ số thập phân thứ 7 này tưởng chừng không đáng kể, nhưng đối với các dự án khảo sát bản đồ và đo đạc đất đai quy mô lớn, nó tạo ra sai lệch tích lũy rất lớn.

Vào năm 1959, Mỹ đã đồng ý áp dụng chuẩn International Foot nhưng không bắt buộc thực thi nghiêm ngặt, dẫn tới việc hiện tại vẫn còn tới 40 bang tiếp tục sử dụng chuẩn US Survey Foot cũ cho các bản đồ quy hoạch đất đai. Việc này tạo ra những rắc rối dở khóc dở cười khi hai bang giáp ranh sử dụng hai chuẩn đo lường khác nhau (ví dụ bang Oregon và Washington), khiến các kỹ sư khi thiết kế cầu vượt sông biên giới phải liên tục quy đổi đơn vị để tránh lệch nhịp cầu. Cơ quan đo lường Mỹ thông báo sẽ chính thức bãi bỏ hoàn toàn chuẩn US Survey Foot cũ vào năm 2022 để thống nhất một chuẩn duy nhất trên toàn quốc.

2. **Dự án xây dựng tổ hợp khu lưu trú chuyên biệt hỗ trợ người vô gia cư tại California**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122105.jpg)

Làn sóng tăng giá bất động sản chóng mặt tại California đang làm gia tăng nghiêm trọng số lượng người vô gia cư tại bang này, ước tính chạm mốc 130.000 người vào năm 2018 (chiếm gần 1/4 tổng số người vô gia cư trên toàn nước Mỹ). Trước thực trạng đó, một tổ chức xã hội phi lợi nhuận đã đề xuất dự án trị giá 3 tỷ USD để xây dựng một khu đô thị chuyên biệt rộng 1.2 km² làm nơi cư trú tập trung cho khoảng 150.000 người vô gia cư.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122107.jpg)

Theo thiết kế dự án, toàn bộ người vô gia cư đủ điều kiện sẽ được bố trí lưu trú hoàn toàn miễn phí tại các khu nhà ở tập trung mật độ cao, cung cấp miễn phí dịch vụ ăn uống tại các nhà ăn cộng đồng của mỗi block và các không gian sinh hoạt chung sạch sẽ.

Mỗi cư dân khi nhập cư sẽ được cấp một chiếc vòng đeo tay thông minh tích hợp chip RFID đóng vai trò như chìa khóa mở cửa phòng và quản lý phát thuốc men y tế định kỳ. Khu đô thị cũng tích hợp các cơ sở đào tạo nghề, hướng nghiệp giúp cư dân sớm tái hòa nhập cộng đồng và tự chủ cuộc sống để rời khu lưu trú.

3. **M-Blocks 2.0 - Thế hệ robot tự lắp ghép và biến hình linh hoạt của MIT**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121101.jpg)

Các nhà nghiên cứu tại Viện Công nghệ Massachusetts (MIT) giới thiệu thế hệ robot tự biến hình M-Blocks 2.0. Hệ thống robot được tạo thành từ các khối lập phương nhỏ gọn riêng biệt, có khả năng tự động di chuyển, nhảy lên, xoay vòng và liên kết với nhau để thay đổi hình dạng cấu trúc tổng thể theo yêu cầu công việc.

Mỗi mặt của khối lập phương được in một mã vạch đặc biệt giúp các khối tự nhận diện và truyền thông tin định vị cho nhau, kết hợp cùng hệ thống nam châm điện bên trong để liên kết chặt chẽ tạo thành các cấu trúc cơ học chịu lực ổn định. Nhóm nghiên cứu kỳ vọng trong tương lai có thể chế tạo các hệ thống gồm hàng triệu khối lập phương nhỏ để ứng dụng vào công tác cứu hộ thiên tai, robot có thể tự động biến hình thành một chiếc thang cứu hộ cao tầng giúp người dân thoát khỏi đám cháy.

4. **Tranh cãi quanh lễ cầu siêu tiễn biệt các linh kiện của robot thú cưng AIBO tại Nhật Bản**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122204.jpg)

Một ngôi chùa cổ tại tỉnh Chiba (Nhật Bản) đã tổ chức một buổi lễ cầu siêu vô cùng đặc biệt dành riêng cho các dòng robot chó cưng AIBO thế hệ cũ do Sony sản xuất. Hàng chục chú robot chó hỏng được xếp ngay ngắn trên ban thờ để tiến hành các nghi thức tụng kinh tiễn biệt trước sự chứng kiến đầy xúc động của những người chủ lớn tuổi.

Đơn vị tài trợ cho sự kiện là một doanh nghiệp chuyên sửa chữa đồ điện tử cũ. Dòng robot chó cưng AIBO thế hệ đầu ra mắt năm 1999 đã bán được hơn 150.000 máy trước khi bị Sony khai tử ngừng hỗ trợ linh kiện sửa chữa. Đối với nhiều người già neo đơn tại Nhật, chú robot chó này đã trở thành một thành viên thực sự trong gia đình. Buổi lễ cầu siêu được tổ chức nhằm an ủi tinh thần cho những người chủ trước khi chú robot chó của họ buộc phải tháo dỡ linh kiện phục vụ việc sửa chữa cho các chú chó robot khác còn hoạt động.

5. **Sự cố nhiễm mã độc làm tê liệt toàn bộ hệ thống thông tin một trường đại học Đức**

Trước kỳ nghỉ lễ Giáng sinh, một trường đại học lớn tại Frankfurt (Đức) đã chứng kiến khung cảnh hàng vạn giảng viên và sinh viên xếp hàng dài trước văn phòng công nghệ thông tin IT của trường để xuất trình giấy tờ tùy thân và nhận lại mật khẩu tài khoản nội bộ mới được in ra giấy trực tiếp.

Hệ thống mạng nội bộ của trường trước đó đã bị mã độc tống tiền tấn công làm tê liệt hoàn toàn, buộc bộ phận IT phải ngắt kết nối internet toàn trường để tiến hành quét virus cho hơn 38.000 máy tính bằng các thiết bị USB chuyên dụng. Do máy chủ mail nội bộ cũng bị nhiễm độc không thể gửi thư tự động, nhà trường bắt buộc phải áp dụng phương thức thủ công phát mật khẩu mới trực tiếp tại quầy cho từng người dùng để đảm bảo an toàn thông tin.

6. **Tin vắn**

- Báo cáo của Liên minh Bảo tồn Thiên nhiên Quốc tế (IUCN) chỉ ra hiện tượng biến đổi khí hậu đang làm nhiệt độ nước biển tăng cao, làm sụt giảm nghiêm trọng nồng độ oxy hòa tan trong nước biển đe dọa sự tồn tại của hàng vạn loài sinh vật đại dương.

- Lực lượng an ninh Thượng Hải đưa vào vận hành dòng robot tuần tra tự hành tích hợp hệ thống camera 360 độ độ phân giải cao và cảm biến hồng ngoại, hỗ trợ đắc lực cho công tác giám sát an ninh đám đông đêm giao thông.

- Bảng xếp hạng ứng dụng di động phổ biến nhất thế giới trên Google Play Store năm 2019 ghi nhận sự thống trị tuyệt đối của các ứng dụng mạng xã hội của Facebook (WhatsApp, Messenger, Facebook, Instagram) và game di động.

- Tác phẩm điện ảnh bom tấn *The Irishman* ứng dụng các thuật toán AI xử lý hình ảnh phức tạp để tự động trẻ hóa khuôn mặt của dàn diễn viên gạo cội (đều đã trên 70 tuổi) về lại độ tuổi trung niên 40-50 trực tiếp trong các cảnh quay.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121005.jpg)

## 文章 (Bài viết)

1、[Bài viết] [Tìm hiểu về phương thức bay và cơ chế kết nối internet trên các chuyến bay dân dụng](https://onezero.medium.com/what-makes-it-possible-to-browse-the-internet-at-35-000-feet-1afaea83eb5) (Tiếng Anh)

Bài viết phân tích các giải pháp công nghệ giúp hành khách có thể lướt web ở độ cao 10.000 mét: thông qua kết nối sóng vô tuyến trực tiếp với các trạm phát sóng mặt đất (ATG) khi bay qua đất liền hoặc kết nối với hệ thống vệ tinh quỹ đạo (dải tần Ku/Ka) khi bay qua đại dương.

2、[Bài viết] [Khám phá phương pháp giản đơn mới giải phương trình bậc hai không cần nhớ công thức](https://www.technologyreview.com/s/614775/a-new-way-to-make-quadratic-equations-easy/) (Tiếng Anh)

Giới thiệu phương pháp giải phương trình bậc hai mới do nhà toán học Po-Shen Loh đề xuất, giúp đơn giản hóa quy trình tư duy tìm nghiệm bằng cách tận dụng mối quan hệ đối xứng giữa hai nghiệm thay vì bắt học sinh phải ghi nhớ công thức delta phức tạp từ thời cổ đại.

## 软件 (Phần mềm)

1、[Elementary OS — Bản phân phối Linux đẹp mắt với giao diện tối ưu mô phỏng macOS](https://blog.elementary.io/introducing-elementary-os-5-1-hera/)

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120607.jpg)

Hệ điều hành mã nguồn mở xây dựng trên nền tảng Ubuntu, hướng tới trải nghiệm sử dụng tinh giản, trực quan và mượt mà phù hợp cho người dùng phổ thông muốn chuyển dịch từ macOS hoặc Windows.

2、[VirtScreen — Ứng dụng biến thiết bị máy tính bảng thành màn hình phụ cho hệ điều hành Linux](https://github.com/kbumsik/VirtScreen)

Giải pháp phần mềm hữu ích cho phép lập trình viên tận dụng chiếc iPad hoặc máy tính bảng Android cũ làm màn hình phụ hiển thị mã nguồn hoặc tài liệu thông qua kết nối mạng không dây dựa trên giao thức kết nối VNC.

3、[docker-slim — Công cụ hỗ trợ tối ưu hóa và nén giảm dung lượng file ảnh Docker](https://github.com/docker-slim/docker-slim)

Tiện ích mạnh mẽ dành cho kỹ sư DevOps giúp phân tích cấu trúc Docker Image để tự động loại bỏ các tệp tin dư thừa, thư viện không dùng tới, giúp nén dung lượng file ảnh nhỏ lại tới 30 lần mà vẫn đảm bảo ứng dụng vận hành ổn định.

4、[openEuler — Bản phân phối hệ điều hành Linux mã nguồn mở từ tập đoàn Huawei](https://openeuler.org/zh/)

Huawei chính thức phát hành mã nguồn mở hệ điều hành openEuler phát triển dựa trên nền tảng CentOS, được tối ưu hóa hiệu năng chuyên sâu cho cấu trúc vi xử lý ARM64 và tích hợp các chuẩn bảo mật cấp doanh nghiệp.

## 资源 (Tài nguyên)

1、[Trang web] [The Deep Sea - Hành trình khám phá các tầng sâu đại dương trực quan](https://neal.fun/deep-sea/)

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120505.jpg)

Trang web giáo dục tương tác độc đáo cho phép người dùng cuộn chuột đi sâu xuống các tầng đáy đại dương để quan sát hình dạng và thông tin của các loài sinh vật đặc trưng sinh sống ở từng độ sâu áp suất khác nhau.

## 图片 (Hình ảnh)

1. **Khung cảnh kết nối giao thông金 môn của bán đảo San Francisco**

Bức ảnh chụp vệ tinh toàn cảnh địa hình địa lý khu vực San Francisco với điểm kết nối phía bắc là cây cầu Golden Gate nổi tiếng dẫn sang hạt Marin, và phía đông là cầu cảng Bay Bridge dẫn sang thành phố Oakland.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110807.jpg)

## 文摘 (Văn trích)

1. **Lời khuyên hữu ích cho lập trình viên: Đừng vội vàng chạy theo các công nghệ, framework mới ra mắt**

Trong thế giới phát triển phần mềm, hầu như mỗi tháng đều có sự xuất hiện của một framework lập trình mới bóng bẩy được quảng bá rầm rộ (ví dụ như SwiftUI của Apple).

Lời khuyên thực tế của tôi dành cho các nhà phát triển là: hãy kiên nhẫn chờ đợi từ 1 đến 2 năm trước khi quyết định đầu tư thời gian học tập nó. Đừng lo lắng về việc bỏ lỡ cơ hội thăng tiến; đây không phải là một chuyến bay cố định giờ mà là một tiến trình công nghệ dài hạn, bạn luôn có thể lên tàu bất kỳ lúc nào. Quyết định áp dụng một công nghệ mới phải dựa trên nhu cầu thực tế của dự án chứ không phải vì tâm lý sợ bị tụt hậu (FOMO).

Bản thân các đơn vị phát hành luôn có động lực thương mại để quảng bá thổi phồng sản phẩm của họ là hoàn hảo nhất. Một số lập trình viên trẻ thiếu kinh nghiệm cũng dễ dàng bị cuốn theo sự phấn khích ban đầu để tâng bốc công nghệ đó lên. Thế nhưng thực tế, các framework mới ra mắt thường chứa đầy lỗi kỹ thuật, hệ thống tài liệu hướng dẫn sơ sài và chưa được kiểm chứng qua các dự án lớn thực tế. Nếu bạn vội vàng đưa nó vào dự án, bạn sẽ tiêu tốn hàng tuần trời chỉ để sửa các lỗi lặt vặt của chính framework đó, tạo thêm gánh nặng học tập lớn cho các thành viên khác trong nhóm.

Một công nghệ mới ra mắt không thể ngay lập tức khai tử các công nghệ cũ đã chín muồi. Ví dụ điển hình như ngôn ngữ Swift được Apple giới thiệu bản 1.0 từ năm 2014, nhưng phải đến năm 2016 bản 3.0 mới bắt đầu tạm ổn định để đưa vào sản xuất thực tế, và thực sự chín muồi vào năm 2018. Quá trình chuyển dịch công nghệ luôn diễn ra trong nhiều năm, hãy kiên nhẫn để công nghệ đó tự hoàn thiện lỗi trước khi bạn áp dụng nó.

## 言论 (Danh ngôn)

1、

> "Nếu loài蜜 ong hoàn toàn biến mất khỏi trái đất, nhân loại sẽ chỉ còn lại đúng 4 năm để sinh tồn. Không có ong, sẽ không có hoạt động thụ phấn; không có thụ phấn, thảm thực vật sẽ lụi tàn; không có thực vật, động vật sẽ không có thức ăn; và con người cũng sẽ diệt vong theo."
> 
> -- Câu nói nổi tiếng của Albert Einstein

(Hết)
