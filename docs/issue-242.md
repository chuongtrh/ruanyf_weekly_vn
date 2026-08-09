# Bản tin chia sẻ công nghệ (Số 242): Một lần bị hacker tấn công máy chủ đầy bối rối

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021201.webp)

Bức ảnh trên đã đoạt giải nhất tại Cuộc thi Nhiếp ảnh gia Du lịch Thế giới năm 2022. Nhân vật trong ảnh là Najin – một trong hai cá thể tê giác trắng phương bắc cuối cùng còn sót lại trên Trái Đất, hiện đã 33 tuổi. Để bảo vệ Najin khỏi sự săn lùng tàn bạo của những kẻ trộm sừng, chính phủ Kenya đã bố trí một đội tuần tra bảo vệ riêng biệt. Họ gắn bó với Najin như hình với bóng, và trong bức ảnh là khoảnh khắc người lính bảo vệ đang cùng nghỉ ngơi với Najin vào buổi trưa trên thảo nguyên châu Phi rộng lớn. (Nguồn: [TPOTY](https://www.tpoty.com/galleries/2022-winners/))

## 本周话题：一次尴尬的服务器被黑

Vào rạng sáng thứ Hai tuần này (ngày 13 tháng 2), máy chủ trang web cá nhân của tôi đã bị hacker tấn công xâm nhập.

Do cuộc tấn công này không kích hoạt các cơ chế cảnh báo tự động của hệ thống, tôi hoàn toàn không hay biết gì. Cho đến sáng khi thức dậy, tôi nhận được hàng loạt email từ các độc giả báo rằng trang web đang gặp sự cố: cứ nhấp vào bất kỳ liên kết bài viết nào trên trang của tôi là trình duyệt lại tự động chuyển hướng sang một địa chỉ cá cược trực tuyến lạ. Thực sự là một tình huống vô cùng bối rối.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021505.webp)

Tôi lập tức truy cập máy chủ để kiểm tra tình hình. Sự việc diễn ra khá nghiêm trọng: **kẻ tấn công đã chiếm được quyền ghi (write permission) vào thư mục chứa mã nguồn web**, từ đó xóa sạch nội dung của toàn bộ các trang HTML tĩnh và thay vào đó bằng đoạn mã chuyển hướng script dạng `window.onload="..."`.

Tuy nhiên, hệ cơ sở dữ liệu của máy chủ không có dấu hiệu bị can thiệp và hệ thống ghi nhật ký đăng nhập SSH không ghi nhận bất kỳ địa chỉ IP lạ nào truy cập vào hệ điều hành. Từ đó, tôi nhận định hacker chỉ khai thác được lỗ hổng bảo mật ứng dụng web của tôi để ghi đè tệp tin chứ chưa chiếm được quyền kiểm soát hoàn toàn hệ điều hành máy chủ.

Lúc đó, cảm giác của tôi không phải là hoảng sợ hay tức giận mà là một sự bất lực. Điều tôi lo sợ bấy lâu nay cuối cùng cũng đã xảy ra.

Nhiều độc giả thân thiết đều biết giao diện và cấu trúc trang web cá nhân của tôi đã giữ nguyên thiết kế lỗi thời này suốt hơn 10 năm qua. Không phải tôi không muốn tối ưu hóa giao diện, mà thực sự việc sửa đổi mã nguồn vô cùng phức tạp.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021506.webp)

Nguyên nhân là hệ thống quản trị nội dung (CMS) chạy ngầm phía sau của trang web được xây dựng dựa trên MovableType – một nền tảng quản trị blog cổ xưa thậm chí còn ra đời trước cả WordPress.

MovableType từ lâu đã ngừng cung cấp các bản cập nhật mã nguồn mở miễn phí và chuyển giao bản quyền cho một doanh nghiệp Nhật Bản. Nếu muốn nhận được các bản vá bảo mật và nâng cấp hệ thống, người dùng phải đóng một khoản phí duy trì định kỳ. Vì tôi không đóng phí, hệ thống quản trị trang web của tôi đã bị bỏ rơi và lão hóa theo năm tháng.

Bản thân phần mềm quản trị cũ kỹ không phải là vấn đề quá lớn nếu nó vẫn chạy ổn định và bạn không cần thêm tính năng mới. Vấn đề thực sự nằm ở chỗ toàn bộ hệ điều hành và các thư viện liên quan của máy chủ cũng phải giữ nguyên phiên bản cũ để bảo đảm tính tương thích cho MovableType. Tôi từng thử chuyển hệ thống sang chạy trên một OS đời mới hơn, nhưng hàng loạt lỗi xung đột thư viện phát sinh khiến tôi đành từ bỏ và chấp nhận duy trì máy chủ chạy trên một hệ điều hành đã hết hạn hỗ trợ bảo mật.

Tôi luôn biết việc chạy một hệ điều hành máy chủ lỗi thời là cực kỳ mất an toàn, nhưng vì ngại sửa lỗi tương thích nên cứ chần chừ không nâng cấp. Và hậu quả cuối cùng đã đến.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021507.webp)

Cách đây hai năm, trang web từng bị tấn công một lần. Khi đó, tôi đã chủ quan tự vá lỗi thủ công và gia cố bảo mật máy chủ thay vì nâng cấp toàn bộ hệ thống.

Lần này, tôi cũng định làm tương tự. Máy chủ của tôi có cơ chế sao lưu định kỳ (snapshots). Sau khi phát hiện bị hack, tôi thực hiện khôi phục dữ liệu về bản sao lưu an toàn gần nhất, thay đổi một số cấu hình phân quyền thư mục và đưa trang web hoạt động trở lại vào trưa thứ Hai, hy vọng giải pháp tạm thời này sẽ tiếp tục giúp trang web bình yên.

Tuy nhiên, kẻ tấn công dường như đã thiết lập công cụ quét tự động túc trực trực tuyến. Chưa đầy một tiếng sau khi tôi đưa trang web hoạt động trở lại, toàn bộ các tệp tin lại bị ghi đè và chuyển hướng y hệt như cũ.

Lúc này, tôi hiểu rằng lỗ hổng bảo mật nằm sâu trong lõi phần mềm MovableType đã bị hacker khai thác triệt để. Tôi bắt buộc phải ngắt kết nối trang web hoàn toàn và chuyển hướng tên miền trỏ về một trang thông báo tạm dừng hoạt động.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021508.webp)

Suốt một ngày sau đó, tôi rơi vào trạng thái bế tắc và đã chuẩn bị cho kịch bản xấu nhất là trang web cá nhân sẽ phải ngừng hoạt động trong một thời gian dài để thiết kế lại.

Đến chiều thứ Ba, tôi quyết định thực hiện một thử nghiệm mang tính may rủi: tiến hành nâng cấp toàn bộ hệ điều hành máy chủ và các thư viện phụ thuộc lên phiên bản mới nhất.

Tôi tiến hành cập nhật hệ thống và cài đặt các phiên bản môi trường mới, quá trình cài đặt kéo dài liên tục hơn một tiếng đồng hồ. Thật kỳ diệu là sau khi nâng cấp xong, trang web khởi chạy lại hoàn toàn bình thường mà không gặp phải bất kỳ lỗi tương thích nghiêm trọng nào của hệ thống cũ. Tôi lập tức mở lại trang web và hệ thống hoạt động ổn định cho đến nay.

Mặc dù vậy, tôi vẫn không thể khẳng định chắc chắn rằng mọi lỗ hổng bảo mật của MovableType đã được khắc phục hoàn toàn. Nếu trang web tiếp tục bị tấn công lần nữa, tôi sẽ buộc phải đóng trang web lâu dài để tập trung hoàn thiện dự án mà tôi đã lên kế hoạch cho năm nay: Tự viết lại toàn bộ cấu trúc blog của mình thành một trang web tĩnh (static website) hoàn toàn để loại bỏ hoàn toàn các nguy cơ tấn công máy chủ.

Sự cố lần này mang lại nhiều bài học đắt giá. Nếu các bạn lập trình viên cũng có ý định tự vận hành một trang blog cá nhân độc lập, tôi xin chia sẻ hai lời khuyên thực tế:

1. **Đừng tự mình quản trị máy chủ vật lý**: Công tác vận hành và bảo mật máy chủ (SysAdmin/DevOps) là một lĩnh vực chuyên môn rất phức tạp đòi hỏi nhiều thời gian bảo trì. Ngay cả khi bạn có kiến thức chuyên môn, việc tiêu tốn quá nhiều thời gian để theo dõi và vá lỗi bảo mật cho một trang blog cá nhân là điều không đáng. Internet là một môi trường đầy rẫy các bot quét lỗi tự động hoạt động liên tục, rất khó để bạn có thể phòng thủ thủ công mãi mãi.
2. **Nên sử dụng các dịch vụ lưu trữ đám mây chuyên nghiệp**: Hiện nay, hầu hết các nhà cung cấp dịch vụ đám mây lớn đều cung cấp các giải pháp lưu trữ trang web tĩnh (Static Web Hosting) cực kỳ an toàn và miễn phí. Bạn chỉ cần biên dịch mã nguồn thành các file HTML/CSS tĩnh và đẩy lên đó, hệ thống sẽ tự động phân phối qua mạng CDN mà không cần lo lắng về việc máy chủ bị tấn công. Nếu cần xử lý các logic động, hãy tận dụng các dịch vụ Serverless (FaaS) như Cloud Functions để hệ thống tự động xử lý và co giãn tính toán an toàn.

## Tin tức công nghệ

1、[Trò chơi mô phỏng bay tái hiện các mẫu máy bay cổ trong bảo tàng](https://www.yystv.cn/p/10140)

Tựa game nổi tiếng *《Microsoft Flight Simulator》* (Mô phỏng bay của Microsoft) cung cấp cho game thủ trải nghiệm điều khiển các mẫu máy bay bay qua các không gian thực tế trên thế giới với độ chân thực cực cao:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120103.webp)

Đội ngũ phát triển game vừa thực hiện một dự án độc đáo: số hóa các mẫu máy bay cổ quý hiếm đang được lưu giữ trong các bảo tàng hàng không quốc tế để đưa vào game, trong đó có chiếc thủy phi cơ khổng lồ Hughes H-4 Hercules:

Đây là chiếc máy bay thân rộng có kích thước lớn nhất trong lịch sử hàng không với sải cánh ngang một sân bóng đá. Thiết bị chỉ cất cánh thử nghiệm duy nhất một lần vào năm 1947, bay lướt trên mặt nước trong vài chục giây trước khi được đưa vào lưu trữ trong kho và sau đó chuyển vào bảo tàng:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120104.webp)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120105.webp)

Nhờ nỗ lực số hóa, game thủ hiện nay đã có thể trực tiếp ngồi vào buồng lái giả lập để trải nghiệm cảm giác điều khiển chiếc thủy phi cơ huyền thoại này cất cánh trên bầu trời ảo:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120106.webp)

Đội ngũ phát triển dự kiến sẽ tiếp tục thực hiện quét 3D hơn 300 mẫu máy bay cổ khác để giúp bảo tồn và "phục sinh" những cỗ máy hàng không lịch sử không còn khả năng cất cánh trên thực tế.

2、[Disney công bố thuật toán tự động điều chỉnh tuổi tác của diễn viên](https://gizmodo.com/whats-next-arecibo-observatory-collapse-2-years-later-1849836610)

Tập đoàn giải trí Disney vừa công bố một công nghệ AI chuyên dụng cho ngành điện ảnh cho phép tự động điều chỉnh độ tuổi (trẻ hóa hoặc làm già đi) của diễn viên trên phim:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120205.webp)

Thuật toán hỗ trợ xử lý hình ảnh trực tiếp trên các khung hình video chuyển động, cho phép các diễn viên lớn tuổi tự đóng các phân cảnh thời trẻ của chính mình một cách tự nhiên mà không cần đến các chuyên gia đồ họa CGI xử lý thủ công đắt đỏ:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120206.webp)

Sự phát triển của công nghệ hình ảnh hiện nay khiến ranh giới giữa hình ảnh thực tế và kỹ thuật số trên phim ảnh ngày càng mờ nhạt: từ việc làm đẹp da mặt, thay đổi tuổi tác cho đến việc dựng toàn bộ bối cảnh bằng kỹ thuật màn hình xanh.

3、[Thiết kế sân chơi trẻ em mô phỏng địa hình dốc đá hoang dã](https://www.core77.com/posts/117655/Artist-and-Structural-Engineer-Designs-Risky-Playground)

Các sân chơi trẻ em thông thường thường được trang bị các thiết bị tiêu chuẩn quen thuộc như cầu trượt, xích đu hay bập bênh.

Một kiến trúc sư người New Zealand cho rằng các thiết bị chuẩn hóa này thiếu đi tính thử thách phiêu lưu và đề xuất ý tưởng xây dựng sân chơi mô phỏng địa hình thiên nhiên dốc đá:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120207.webp)

Sân chơi được thiết kế bằng các khối đá tự nhiên lớn xếp chồng lên nhau:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120208.webp)

Tuy trông có vẻ nguy hiểm, toàn bộ các khối đá lớn đều được khoan neo giữ cố định chắc chắn bằng các trục thép chịu lực cắm sâu xuống đất, và bề mặt sân chơi được phủ một lớp cao su đàn hồi giảm chấn để bảo đảm an toàn tuyệt đối cho trẻ em khi leo trèo:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120209.webp)

Sau một tháng đưa vào vận hành thử nghiệm, sân chơi thu hút đông đảo trẻ em tới tham gia vui chơi trải nghiệm leo trèo tự nhiên và chưa ghi nhận bất kỳ sự cố chấn thương nào xảy ra:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120210.webp)

4、[Công nghệ băng gạc y tế thông minh tự động theo dõi vết thương](https://www.inverse.com/innovation/self-healing-bandage-wireless)

Các loại băng gạc thông thường không thể giúp bác sĩ biết được tiến trình phục hồi bên trong vết thương, đôi khi chỉ khi tháo băng ra mới phát hiện vết thương bị nhiễm trùng nghiêm trọng do thuốc không phát huy tác dụng.

Để khắc phục hạn chế này, một nhóm nghiên cứu quốc tế đã phát triển mẫu băng gạc y tế thông minh tích hợp cảm biến:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120803.webp)

Mẫu băng gạc sử dụng một bảng mạch in siêu mỏng co giãn linh hoạt có khả năng tự động đo nồng độ vi khuẩn xung quanh vết thương, từ đó tự động điều tiết lượng thuốc kháng sinh phóng thích qua da cho phù hợp.

Thiết bị tích hợp module truyền tải dữ liệu không dây và sử dụng công nghệ thu năng lượng sóng vô tuyến qua ăng-ten để hoạt động mà không cần tích hợp pin cồng kềnh:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120802.webp)

## Bài viết

1\. [Phân biệt sự khác nhau giữa Next.js, Nuxt và NestJS](https://www.twilio.com/blog/comparing-nextjs-nestjs-nuxt-gatsby)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121802.webp)

Bài viết so sánh chi tiết về kiến trúc, ngôn ngữ sử dụng và mục đích phát triển của ba framework JavaScript lớn phổ biến hiện nay: Next.js (cho React), Nuxt (cho Vue) và NestJS (cho ứng dụng Backend Node.js).

2\. [Tại sao ngành công nghiệp phần mềm chuyển dịch sang ngôn ngữ an toàn bộ nhớ?](https://www.darkreading.com/application-security/shift-memory-safe-languages-gains-momentum)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121002.webp)

Bài phân tích về xu hướng các tập đoàn công nghệ lớn (như Microsoft, Google) đẩy mạnh việc chuyển đổi mã nguồn hệ thống sang các ngôn ngữ an toàn bộ nhớ (Memory-safe languages) như Rust, Go hay Java để triệt tiêu các lỗi rò rỉ hoặc tràn bộ đệm của C/C++.

3\. [Hướng dẫn tạo bản đồ không ảnh 3D từ video camera 360 độ](https://jakecoppinger.com/2022/12/creating-aerial-imagery-with-a-bike-helmet-camera-and-opendronemap/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121201.webp)

Tác giả chia sẻ quy trình sử dụng phần mềm mã nguồn mở OpenDroneMap để dựng mô hình bản đồ hình ảnh 3D từ trên cao bằng cách xử lý luồng video ghi hình từ camera 360 độ gắn trên mũ bảo hiểm khi đạp xe quanh khu vực.

4\. [Chia sẻ kinh nghiệm thiết lập góc làm việc Home Office thoải mái](https://arun.is/blog/desk-setup/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022103007.webp)

Bài viết chia sẻ chi tiết sơ đồ bố trí bàn làm việc công thái học, cách đi dây cáp tối giản, lựa chọn màn hình và ghế ngồi để tạo không gian làm việc tại nhà thoải mái và tăng năng suất viết code cho lập trình viên.

5\. [Tôi kiếm sống bằng việc phát triển hệ điều hành SerenityOS như thế nào?](https://awesomekling.github.io/How-I-make-a-living-working-on-SerenityOS/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022103102.webp)

Tác giả của dự án hệ điều hành mã nguồn mở độc đáo SerenityOS chia sẻ hành trình từ bỏ công việc văn phòng để chuyển sang phát triển mã nguồn mở toàn thời gian từ năm 2021 dựa trên nguồn tài trợ đóng góp từ cộng đồng.

6\. [Hệ thống hạ tầng CNTT cá nhân phục vụ làm việc tại nhà của tôi](https://writings.stephenwolfram.com/2019/02/seeking-the-productive-life-some-details-of-my-personal-infrastructure/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110301.webp)

Stephen Wolfram – nhà sáng lập phần mềm tính toán nổi tiếng Mathematica – chia sẻ chi tiết về hệ thống mạng, thiết bị sao lưu dữ liệu tại nhà và mẫu bàn máy tính di động đặc biệt giúp ông có thể làm việc khi đang đi bộ thể dục.

7\. [Cách cấu hình Playwright tự động vượt qua xác thực hai yếu tố (2FA)](https://blog.checklyhq.com/how-to-bypass-totp-based-2fa-login-flows-with-playwright/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121604.webp)

Bài viết kỹ thuật hướng dẫn lập trình viên kiểm thử tự động sử dụng Playwright để tự sinh mã OTP dựa trên thuật toán TOTP để tự động điền vào ô xác thực bảo mật 2 lớp khi chạy test login.

8\. [Mô phỏng và tìm hiểu các giao thức mạng bằng ngôn ngữ Ruby](https://medium.com/geckoboard-under-the-hood/how-to-build-a-network-stack-in-ruby-f73aeb1b661b)（Tiếng Anh）

Bài viết hướng dẫn xây dựng một ngăn xếp kết nối mạng cơ bản từ đầu bằng ngôn ngữ Ruby để giải thích trực quan cơ chế đóng gói gói tin và hoạt động của giao thức truyền tải UDP.

## Công cụ

1、[Convex: Dịch vụ đám mây quản lý trạng thái thời gian thực cho ứng dụng](https://www.convex.dev/)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062210.webp)

Dịch vụ Backend-as-a-Service (tương tự Firebase) hỗ trợ lập trình viên lưu trữ và đồng bộ hóa trạng thái dữ liệu thời gian thực giữa máy chủ và các thiết bị khách kết nối một cách mượt mà.

2、[Công cụ tự tạo ảnh đại diện Tết Quý Mão độc đáo](https://www.xiaoli.vip/rabbit/)

Ứng dụng web nguồn mở cho phép người dùng tải ảnh chân dung cá nhân lên để tự động lồng ghép vào nhiều khung hình viền trang trí hình chú thỏ Tết Quý Mão đẹp mắt. Mã nguồn dự án được chia sẻ công khai trên [GitHub](https://github.com/xiaoli1999/custom-rabbitImage). (Đóng góp của [@xiaoli1999](https://github.com/ruanyf/weekly/issues/2898))

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021101.webp)

3、[ElasticView: Ứng dụng desktop quản lý cơ sở dữ liệu ElasticSearch](https://github.com/1340691923/ElasticView)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021202.webp)

Công cụ giao diện đồ họa (GUI client) dành cho hệ điều hành Windows/macOS hỗ trợ quản trị viên giám sát trạng thái sức khỏe các node và thực hiện nhanh các truy vấn dữ liệu trên cụm ElasticSearch. (Đóng góp của [@lin2415016](https://github.com/ruanyf/weekly/issues/2887))

4、[RATH: Công cụ phân tích và trực quan hóa dữ liệu tự động bằng AI](https://github.com/Kanaries/Rath)

Công cụ nguồn mở hỗ trợ nhà phân tích dữ liệu: chỉ cần tải tệp tin dữ liệu (CSV/JSON) lên, hệ thống sẽ tự động quét, tìm kiếm mối tương quan giữa các trường thông tin và tự động sinh các biểu đồ trực quan hóa dữ liệu phù hợp. (Đóng góp của [@AntoineYANG](https://github.com/ruanyf/weekly/issues/2892))

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021204.webp)

5、[tl-rtc-file-tool: Công cụ chia sẻ file trực tiếp bằng WebRTC](https://im.iamtsm.cn/)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021205.webp)

Dự án web [mã nguồn mở](https://github.com/iamtsm/tl-rtc-file) ứng dụng giao thức WebRTC hỗ trợ người dùng truyền tải dữ liệu, gửi tệp tin trực tiếp giữa các trình duyệt (P2P) với tốc độ cao không qua máy chủ trung gian. (Đóng góp của [@iamtsm](https://github.com/ruanyf/weekly/issues/2893))

6、[EasyNode: Bảng điều khiển quản trị máy chủ Linux bằng Node.js](https://github.com/chaos-zhu/easynode)

Mã nguồn mở xây dựng trang quản trị máy chủ Linux gọn nhẹ viết bằng Node.js hỗ trợ giám sát thông số CPU, RAM, lưu lượng mạng và quản lý tệp tin trực quan qua giao diện web. (Đóng góp của [@chaos-zhu](https://github.com/ruanyf/weekly/issues/2897))

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021206.webp)

7、[vscode-gptcommit: Plugin tự động viết Git commit message trên VS Code](https://github.com/pwwang/vscode-gptcommit)

Extension dành cho trình soạn thảo VS Code tích hợp mô hình ngôn ngữ lớn để tự động phân tích các dòng code thay đổi trong git diff và tự động sinh nội dung commit message phù hợp. (Đóng góp của [@pwwang](https://github.com/ruanyf/weekly/issues/2890))

8、[Tweek Calendar: Ứng dụng lịch quản lý công việc tối giản](https://tweek.so/)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111904.webp)

Ứng dụng web hỗ trợ lên kế hoạch công việc hàng tuần với giao diện thiết kế tối giản, trực quan tương tự như một cuốn sổ tay lịch giấy truyền thống.

9、[BetterDisplay: Công cụ tinh chỉnh thông số hiển thị màn hình trên macOS](https://github.com/waydabber/BetterDisplay)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111905.webp)

Phần mềm mã nguồn mở dành cho máy tính Mac hỗ trợ người dùng tạo màn hình ảo (virtual screens), tinh chỉnh độ phân giải HiDPI và quản lý độ sáng của các màn hình ngoài kết nối.

10、[berty: Ứng dụng chat bảo mật ngang hàng qua kết nối Bluetooth](https://berty.tech/)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112201.webp)

Ứng dụng nhắn tin nhóm phi tập trung bảo mật cao, điểm đặc biệt là khả năng kết nối trò chuyện trực tiếp giữa các thiết bị thông qua sóng Bluetooth năng lượng thấp (BLE) khi khu vực không có sóng di động hay internet.

## Tài nguyên

1、[Mastering Bitcoin: Sách hướng dẫn chuyên sâu về kỹ thuật Bitcoin](https://github.com/bitcoinbook/bitcoinbook)

Tài liệu điện tử tiếng Anh chất lượng cao (phiên bản thứ hai) được chia sẻ miễn phí trên GitHub giải thích chi tiết cấu trúc mật mã học và cơ chế đồng thuận ngang hàng của mạng lưới Bitcoin.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062303.webp)

2、[satellite-track: Bản đồ trực quan hóa quỹ đạo bay của các vệ tinh](https://jiangteng2019.github.io/satellite-track/)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021203.webp)

Ứng dụng web trực quan hóa vị trí thời gian thực và đường bay quỹ đạo của hàng ngàn vệ tinh nhân tạo quanh Trái Đất dạng 3D. Mã nguồn mở trên [GitHub](https://github.com/jiangteng2019/satellite-track). (Đóng góp của [@jiangteng2019](https://github.com/ruanyf/weekly/issues/2888))

3、[tabler-icons: Kho thư viện biểu tượng SVG đồng bộ cho lập trình viên](https://tabler-icons.io/)

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022042302.webp)

Trang web cung cấp miễn phí hơn 1.900 biểu tượng đồ họa vector định dạng SVG được thiết kế theo phong cách tối giản đồng bộ nét vẽ giúp làm đẹp giao diện ứng dụng.

4、[Some Assembly Required (Cẩm nang học hợp ngữ Assembly nhập môn)](https://github.com/hackclub/some-assembly-required)

Bộ tài liệu hướng dẫn cơ bản về hợp ngữ Assembly được biên soạn trực quan kèm nhiều hình minh họa sinh động dành riêng cho học sinh sinh viên chưa có nền tảng lập trình máy tính.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022062905.webp)

5、[Quick, Draw!: Trò chơi phác họa nét vẽ kiểm thử AI của Google](https://quickdraw.withgoogle.com/)

Trò chơi trực tuyến vui nhộn của Google yêu cầu người dùng vẽ phác thảo nhanh một đồ vật theo yêu cầu trong vòng 20 giây để hệ thống mạng nơ-ron AI phán đoán nhận dạng hình vẽ.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022063003.webp)

## Hình ảnh

1\. **Phát hiện những bức tượng đầu đá Olmec khổng lồ cổ đại**

Vào thập niên 1930, các nhà khảo cổ học đã phát hiện ra nhiều bức tượng đầu người bằng đá khổng lồ chôn sâu dưới lòng đất tại Guatemala với chiều cao dao động từ 2m đến 3m:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090505.webp)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090506.webp)

Các nghiên cứu khảo cổ nhận định các bức tượng đá này do người Olmec cổ đại điêu khắc từ khoảng 3.000 đến 5.000 năm trước:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090507.webp)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090508.webp)

Hiện nay, tổng cộng có 17 bức tượng đầu đá khổng lồ Olmec đã được khai quật và trưng bày bảo tồn trong các bảo tàng khảo cổ quốc gia.

## ✍️ Bài đọc thêm

### Ký ức về thương vụ Apple mua lại NeXT cách đây 25 năm

Hai mươi nhăm năm trước, vào ngày 20 tháng 12 năm 1996, tôi đang làm việc với tư cách là kỹ sư hệ thống tại NeXT – công ty máy tính do Steve Jobs thành lập vào năm 1985 sau khi rời Apple. Tôi là một trong ba nhân viên duy nhất của hãng làm việc tại thị trường Canada.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021501.webp)

Thời kỳ đó điện thoại di động chưa phổ biến, mọi thông báo quan trọng của ban giám đốc NeXT đều được truyền tải qua hệ thống thư thoại Audix. Chúng tôi kiểm tra thông tin bằng cách gọi điện về tổng đài số 1-800-345-5588 và nhập mã hộp thư thoại của mình.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021502.webp)

Hôm đó, tôi nhận được tin nhắn khẩn thông báo tất cả nhân viên phải gọi về tổng đài vào đúng 14 giờ chiều để nghe thông báo một sự kiện đặc biệt. Khi đó tôi đang di chuyển trên phố và phải chạy khắp nơi tìm kiếm một bốt điện thoại công cộng đáng tin cậy bên trong một viện bảo tàng để gọi điện.

Đúng 14 giờ, thông tin được công bố khiến toàn bộ nhân viên chấn động: Apple đã đồng ý mua lại NeXT với giá 400 triệu USD. (Nhiều năm sau nhìn lại, giới công nghệ đùa rằng thực chất đây là việc Apple chi ra 400 triệu USD để NeXT thâu tóm lại chính mình, vì sau đó hầu hết các lãnh đạo cấp cao của Apple mới đều là người cũ từ NeXT chuyển sang).

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122204.webp)

Thời điểm trước sáp nhập, tình hình kinh doanh của NeXT thực sự gặp rất nhiều khó khăn. Steve Jobs dành phần lớn thời gian tập trung cho hãng phim hoạt hình Pixar. Lợi nhuận của NeXT chủ yếu đến từ việc bán phần mềm máy chủ WebObjects (viết bằng Java). Ý tưởng về dòng máy trạm và hệ điều hành cách mạng của hãng không đạt được doanh số kỳ vọng và Steve Jobs phải duy trì công ty bằng cách bán các phần mềm máy chủ doanh nghiệp đắt đỏ.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021503.webp)

Apple khi đó cũng đang rơi vào vòng xoáy khủng hoảng trầm trọng và đứng trước nguy cơ cạn kiệt dòng tiền mặt hoạt động.

Apple quyết định mua lại NeXT chủ yếu để sở hữu hệ điều hành NeXTSTEP (đã được cấu hình tương thích với vi xử lý Intel). Ngay sau khi thương vụ hoàn tất và Steve Jobs quay trở lại nắm quyền điều hành Apple, một chặng đường tái cấu trúc công nghệ ngoạn mục đã bắt đầu diễn ra:

Hệ điều hành NeXTSTEP đã trở thành nền móng để phát triển hệ điều hành Mac OS X sau này; công cụ phát triển phần mềm Project Builder và Interface Builder của NeXT đã được phát triển thành bộ công cụ Xcode quen thuộc ngày nay; và định hướng ngôn ngữ lập trình Objective-C của NeXT chính là tiền đề dẫn lối cho sự ra đời của ngôn ngữ lập trình Swift sau này.

Khi sáp nhập diễn ra, NeXT chỉ có vỏn vẹn khoảng 400 nhân sự so với quy mô hàng ngàn người của Apple. Ngày nay, Apple đã lớn mạnh thành tập đoàn với hơn 160.000 nhân viên trên toàn cầu.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021504.webp)

## Lịch sử tuần này

- 2022年（第 195 期）：[Triết lý công việc: Giá trị tinh thần của việc thực hiện các dự án cá nhân không mưu cầu kết quả thương mại](https://www.ruanyifeng.com/blog/2022/02/weekly-issue-195.html)
- 2021年（第 145 期）：[Kinh tế học: Thảo luận thực trạng biến động kinh tế khi hành vi đi lại giao thương của người dân bị hạn chế](https://www.ruanyifeng.com/blog/2021/02/weekly-issue-145.html)
- 2020年（第 93 期）：[Xu hướng game: Tại sao thể loại trò chơi phiêu lưu khám phá bản đồ tự do sẽ ngày càng phổ biến](https://www.ruanyifeng.com/blog/2020/02/weekly-issue-93.html)
- 2019年（第 43 期）：[Chia sẻ khoa học: Giới thiệu một bài báo cáo khoa học nghiên cứu có đề tài thú vị và hài hước](https://www.ruanyifeng.com/blog/2019/02/weekly-issue-43.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072108.webp)

（Hết）
