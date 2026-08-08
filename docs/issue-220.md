# 科技爱好者周刊（第 220 期）：人工智能的机会在哪里

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần。

Bản tin này is mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn。

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2542) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập。

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082517.webp)

Nắng nóng gay gắt kéo dài tại Trùng Khánh khiến mực nước sông Gia Lăng giảm sâu kỷ lục, làm lộ ra lòng sông cát sỏi khô cằn. Trụ móng của cây cầu Thiên Ty Môn vốn ngập sâu dưới nước nay hoàn toàn trơ trọi trên cạn. (Nguồn: [Tân Hoa Xã](http://www.news.cn/local/2022-08/17/c_1128922377.htm))

## 本周话题：人工智能的机会在哪里

Mô hình trí tuệ nhân tạo tạo ảnh từ văn bản nổi tiếng [DALL·E 2](https://openai.com/dall-e-2/) của [OpenAI](https://openai.com/blog/dall-e-now-available-in-beta/) vừa chính thức mở giai đoạn thử nghiệm rộng rãi cho công chúng.

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082004.webp)

Người dùng có thể gõ các mô tả văn bản để yêu cầu hệ thống tự động vẽ tranh tương ứng, tương tự như chiếc gương thần trong truyện cổ tích. Mức chi phí dịch vụ hiện tại khá rẻ với 15 USD cho 460 lượt sinh ảnh (trung bình khoảng 0,03 USD hay 700 VNĐ cho mỗi bức ảnh).

Ngay lập tức, giới công nghệ đã tìm ra các ứng dụng thực tế hiệu quả của công cụ này:

Tác giả của dự án phần mềm truy vấn dữ liệu [OctoSQL](https://github.com/cube2222/octosql) đang thiếu một logo đại diện. Anh đã mô tả ý tưởng cho DALL·E 2:

> *"Một chú bạch tuộc nhỏ dễ thương đội mũ bảo hộ màu vàng đang đùa nghịch với các hạt ngọc trai sắc màu đầy sức sống trên nền màu đen."*

Hệ thống DALL·E 2 đã trả về cho anh bức ảnh dưới đây:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082403.webp)

Bức ảnh này hiện đã được anh chọn làm logo chính thức hiển thị trên trang chủ dự án sau một vài chỉnh sửa nhỏ (chi tiết xem tại [Bài chia sẻ của tác giả](https://jacobmartins.com/posts/how-i-used-dalle2-to-generate-the-logo-for-octosql/)).

Một nhà phát triển khác thử dùng công cụ để sinh ảnh đại diện [minh họa bài viết kỹ thuật](https://deephaven.io/blog/2022/08/08/AI-generated-blog-thumbnails/). Cho bài giới thiệu về Docker Container, anh gõ mô tả *"Một chú cá voi xanh khổng lồ chở các thùng hàng container trên lưng"*, và AI cho ra bức ảnh:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082404.webp)

Hay bài viết về lập trình đồng thời trong ngôn ngữ Go với mô tả *"Một chú gopher màu xanh nhiều lông đang gõ code lập trình trước nhiều màn hình máy tính"*:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082405.webp)

Các ví dụ trên chứng minh: **Đối với các nhà phát triển độc lập và doanh nghiệp nhỏ, công cụ AI này giống như một nhà thiết kế đồ họa chất lượng cao miễn phí.**

Ngay cả với các tập đoàn lớn sở hữu sẵn đội ngũ thiết kế chuyên nghiệp, công cụ cũng mang lại giá trị to lớn. Thử nghiệm đưa bức vẽ *"Phi hành gia cưỡi ngựa trên Mặt Trăng"* cho các nghệ sĩ đồ họa chuyên nghiệp và đặt câu hỏi: **"Nếu để vẽ bức tranh này thủ công, bạn cần mất bao lâu?"**

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082005.webp)

Thời gian ước tính trung bình nhận được là 5,25 giờ làm việc liên tục. Trong khi đó, DALL·E 2 chỉ mất đúng 22 giây để kết xuất ra hình ảnh tương đương. **Hệ thống giúp tối ưu hóa tới 99,9% thời gian phác thảo ý tưởng của nhà thiết kế.**

Mô hình làm việc tối ưu nhất hiện nay là: nhà thiết kế chịu trách nhiệm trao đổi lấy yêu cầu cụ thể từ khách hàng, sau đó chuyển đổi yêu cầu thành các câu lệnh (prompts) tối ưu để AI sinh ảnh, rồi chỉnh sửa hậu kỳ thủ công để cho ra sản phẩm cuối cùng.

Rõ ràng, các công cụ như DALL·E 2 đang thay thế một phần công việc của các họa sĩ đồ họa thông thường do tốc độ xử lý siêu tốc và chi phí rẻ. Điều này có thể làm giảm bớt nhu cầu tuyển dụng các vị trí vẽ minh họa đơn giản và ảnh hưởng tới mặt bằng thu nhập chung của ngành đồ họa.

Tuy nhiên, thay vì nhìn nhận tiêu cực dưới góc độ AI cướp đi việc làm, hãy nhìn nhận đây là **cơ hội nâng cao năng lực cho tất cả mọi người.**

Những dự án cá nhân vốn trước đây không đủ ngân sách thuê họa sĩ thiết kế nay đã có thể tiếp cận nguồn tài nguyên hình ảnh chất lượng. Thay vì cố gắng cạnh tranh với AI, lựa chọn khôn ngoan nhất là học cách thích nghi và biến chúng thành công cụ đắc lực phóng đại năng suất lao động cá nhân.

Làn sóng AI đang bùng nổ trên mọi lĩnh vực: GitHub Copilot hỗ trợ tự động sinh mã nguồn (thay thế coder), GPT-3 sinh văn bản tự nhiên (thay thế nhà văn), AlphaFold dự đoán cấu trúc protein (thay thế nhà sinh hóa)... Việc chủ động tìm hiểu, thích nghi và làm chủ các công cụ AI mới chính là cách để nâng cao năng lực cạnh tranh cốt lõi của mỗi lập trình viên trong kỷ nguyên mới.

## 稀土开发者大会资料

Cuối tháng trước, cộng đồng [Juejin](https://juejin.cn/?utm_source=ryfzk) đã tổ chức thành công [Hội thảo nhà phát triển lần thứ hai](https://conf.juejin.cn/xdc2022/?utm_source=ryfzk):

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081506.webp)

Sự kiện quy tụ hàng chục chuyên gia công nghệ từ các doanh nghiệp lớn với 18 chuyên đề công nghệ chuyên sâu. Dưới đây là một số bài chia sẻ nổi bật đã được ban tổ chức công bố tài liệu trình bày (PPT) và video xem lại:

### 1\. Xu hướng phát triển của Front-end 2022 - Tác giả Vue Evan You

Evan You chia sẻ về hai khía cạnh chính: các nhược điểm của React Hooks và giải pháp khắc phục trên các framework khác (bao gồm Vue); đồng thời đưa ra nhận định **Front-end framework đang dần dịch chuyển thành một "Lớp trung gian" (Middle Layer)**:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081407.webp)

Phía trên framework là các full-stack framework (như Next.js hay Nuxt) xử lý kết nối server-client, phía dưới là các công cụ biên dịch nhị phân hệ thống (như Rust/Go build tools) thay thế cho JS truyền thống.

### 2\. Java Cloud Native Challenges - Chuyên gia Ao Xiao-jiang (Microsoft Dapr Maintainer)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081502.webp)

Bài viết phân tích bài toán thực tế của các nhà phát triển Java khi xu hướng Cloud Native, Microservices và Serverless đang thu hẹp dần đất diễn của các kiến trúc Spring Cloud cồng kềnh, đề xuất các giải pháp tối ưu hóa bộ nhớ cho Java.

Ban tổ chức đã tổng hợp toàn bộ 78 slide bài trình bày (PPT) chất lượng của hội thảo thành một tập tài liệu Juejin Book trực quan:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082406.webp)

Độc giả quan tâm có thể [Bấm vào đây](https://juejin.cn/book/7127092198096502822?utm_source=ryfzk) hoặc quét mã QR trong bài để đăng ký tài khoản đọc tài liệu miễn phí và tham gia chương trình bốc thăm trúng thưởng từ ban tổ chức.

## 科技动态

1、[重庆 tắt đèn ga tàu điện ngầm để đối phó tình trạng thiếu điện](https://www.cnbeta.com/articles/tech/1307717.htm)

Do đợt nắng nóng kéo dài gây quá tải và thiếu hụt nguồn cung điện lưới nghiêm trọng, hệ thống tàu điện ngầm Trùng Khánh đã tiến hành tắt bớt thiết bị chiếu sáng tại các nhà ga và khoang tàu để tiết kiệm năng lượng:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082518.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082519.webp)

Cảnh tượng hành khách đi lại trong không gian ánh sáng mờ ảo của các ga tàu ngầm. Riêng trong các toa tàu tối om, màn hình LED hiển thị thông tin lộ trình màu đỏ sáng rực tạo nên khung cảnh mang đậm phong cách viễn tưởng cyberpunk:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082513.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082520.webp)

2、[Công nghệ truyền dữ liệu bằng ánh sáng khả kiến cho thiết bị gia dụng thông minh](https://kiwink.io/)

Để kết nối các thiết bị gia dụng thông minh IoT vào mạng di động mà không cần tích hợp module Wi-Fi hay Bluetooth đắt đỏ, một startup tại Anh đề xuất giải pháp truyền dẫn bằng ánh sáng khả kiến (Visible Light Communication):

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032005.webp)

Thiết bị gia dụng được trang bị một bóng đèn LED siêu nhỏ nhấp nháy phát tín hiệu ở tần số cực cao. Camera điện thoại ở khoảng cách 5cm sẽ thu nhận và giải mã luồng sáng này với tốc độ đạt khoảng 1,5 kb/s:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032006.webp)

Để truyền tín hiệu ngược lại từ điện thoại về thiết bị, hệ thống sử dụng ánh sáng nhấp nháy từ đèn flash của camera điện thoại kết hợp đầu thu hồng ngoại đơn giản trên thiết bị gia dụng để nhận lệnh:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032007.webp)

3、[Ra mắt mẫu đồng hồ cơ học mỏng nhất thế giới](https://www.hodinkee.com/articles/richard-mille-sets-a-new-record-for-the-worlds-thinnest-watch-with-the-rm-up-01-ferrari)

Hãng đồng hồ xa xỉ Richard Mille vừa công bố tuyệt tác cơ khí RM UP-01 Ferrari với độ dày kỷ lục chỉ 1,75 mm:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070906.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070909.webp)

Đây là một kỳ tích kỹ nghệ cơ khí khi toàn bộ bánh răng, dây cót và vỏ đồng hồ bằng titan kết hợp mặt kính sapphire được thu gọn tối đa trong bề dày chưa đầy 2mm:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070907.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070908.webp)

Không gian hiển thị thời gian kim chỉ giờ được thu gọn tối đa chiếm khoảng 1/6 diện tích mặt trước nằm ở trung tâm phía trên:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070910.webp)

Thiết bị có giá bán siêu đắt đỏ lên tới 1,88 triệu USD và chỉ sản xuất giới hạn 150 chiếc trên toàn thế giới.

4、[Sự bùng nổ của thiết kế màn hình máy tính tỷ lệ正 vuông 16:18](https://www.lg.com/us/monitors/lg-28mq780-b)

Hãng LG giới thiệu mẫu màn hình độc đáo LG DualUp Monitor sở hữu tỷ lệ khung hình đặc biệt 16:18:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071002.webp)

Với tỷ lệ này, màn hình tương đương việc ghép chồng hai màn hình tỷ lệ 16:9 thông thường lên nhau theo chiều dọc. Thiết kế giúp mở rộng không gian hiển thị cho lập trình viên khi đọc mã nguồn dài và hỗ trợ xử lý song song các định dạng video dọc và ngang tiện lợi:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071003.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071004.webp)

## 文章

1\. [Bài phỏng vấn độc quyền ghi nhận cuộc đời bán dẫn của ông Giang Thượng Nghĩa](https://mp.weixin.qq.com/s/Y22nMfoIh1h3J6cLaNii2w)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082006.webp)

Nội dung buổi trò chuyện chi tiết với ông Giang Thượng Nghĩa (sinh năm 1946, cựu Giám đốc vận hành TSMC và cựu Phó Chủ tịch SMIC) được lưu giữ tại Bảo tàng Lịch sử Máy tính Mỹ, cung cấp bức tranh toàn cảnh về lịch sử phát triển của ngành công nghiệp đúc chip bán dẫn toàn cầu và sự trỗi dậy của TSMC.

2\. [DuckDuckGo chính thức cung cấp dịch vụ email bảo mật miễn phí `@duck.com`](https://www.cnbeta.com/articles/tech/1308699.htm)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082516.webp)

DuckDuckGo mở cổng đăng ký miễn phí hòm thư điện tử bảo mật `@duck.com` cho tất cả mọi người. Dịch vụ đóng vai trò bộ lọc trung gian: tự động bóc tách toàn bộ các đoạn mã theo dõi (tracking pixels) bên trong email trước khi chuyển tiếp nội dung sạch về hòm thư chính chủ của người dùng.

3\. [Thảo luận về giải pháp thay thế ghế công thái học văn phòng bằng xe lăn điện](https://mp.weixin.qq.com/s/hxmC3wHTw4g_JvcRCoqPDQ)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082003.webp)

Tác giả bài viết phân tích các ưu điểm về đệm ngồi êm ái hỗ trợ cột sống nâng đỡ cơ thể và tính cơ động di chuyển của các dòng xe lăn điện cao cấp khi ứng dụng làm ghế làm việc trước máy tính cho lập trình viên.

4\. [Nhìn lại bài phân tích lịch sử năm 2014 dự đoán việc Apple chuyển dịch máy tính Mac sang chip ARM](https://www.mattrichman.net/why-apple-will-switch-to-arm-based-macs/)（Tiếng Anh）

Bài viết phân tích kỹ thuật xuất sắc từ 8 năm trước chỉ ra các rào cản về hiệu năng nhiệt lượng của chip Intel và dự đoán chính xác chiến lược thiết kế chip xử lý tự chủ dựa trên kiến trúc ARM (Apple Silicon) của Apple.

5\. [Hướng dẫn chi tiết quy trình xây dựng trang blog cá nhân sử dụng Next.js](https://www.joshwcomeau.com/blog/how-i-built-my-blog/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071103.webp)

Bài viết cẩm nang hướng dẫn lập trình viên xây dựng hệ thống blog cá nhân mượt mà bằng Next.js kết hợp MDX để viết bài và deploy trực tiếp trên hạ tầng Vercel miễn phí.

6\. [Tranh cãi hiệu năng xử lý module CommonJS và ES Modules trên Node.js](https://github.com/nodejs/node/issues/44186)（Tiếng Anh）

Thảo luận kỹ thuật trên kho lưu trữ mã nguồn của Node.js ghi nhận phản hồi của lập trình viên về việc cơ chế tải module CommonJS (CJS) truyền thống của Node.js hiện đang hoạt động nhanh gấp 10 lần so với tiêu chuẩn ES Modules (ESM) mới và hiệu năng Node.js 18 bị sụt giảm so với Node.js 16.

7\. [Đánh giá thực tế hiệu năng phát triển ứng dụng giữa Tauri và Electron](https://www.levminer.com/blog/tauri-vs-electron)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082304.webp)

Electron hiện đang là framework hàng đầu để viết ứng dụng desktop đa nền tảng nhưng gặp nhược điểm tốn tài nguyên RAM và file cài đặt nặng nề. Tác giả thực hiện viết thử nghiệm dự án bằng Tauri (viết bằng Rust) và so sánh dung lượng, hiệu năng xử lý của hai giải pháp.

8\. [Tìm hiểu mã trạng thái HTTP Early Hints 103 giúp tăng tốc độ tải trang](https://developer.chrome.com/blog/early-hints/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082002.webp)

Chrome hỗ trợ mã trạng thái HTTP Early Hints 103 cho phép máy chủ gửi sớm danh sách các tài nguyên tĩnh (CSS, JS) cần tải trước cho trình duyệt trong thời gian máy chủ đang xử lý dữ liệu trang web, thay thế cho cơ chế HTTP/2 Server Push cũ.

## 工具

1、[mjml: Cú pháp thẻ hỗ trợ thiết kế email HTML hiển thị responsive đa thiết bị](https://mjml.io/)

Bộ công cụ cung cấp cú pháp thẻ XML tối giản giúp tự động biên dịch thành mã nguồn HTML email tương thích tốt với mọi ứng dụng đọc thư (Gmail, Outlook) mà không cần cấu hình CSS bảng phức tạp.

2、[Upptime: Hệ thống giám sát trạng thái uptime website chạy bằng GitHub Actions](https://github.com/upptime/upptime)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070110.webp)

Tiện ích chạy tự động qua GitHub Actions định kỳ 5 phút kiểm tra trạng thái hoạt động của website, tự động tạo issue thông báo lỗi và commit lịch sử phản hồi trực tiếp lên repo Git để tạo trang trạng thái trực quan.

3、[Vanblog: Hệ thống quản trị blog cá nhân gọn nhẹ đóng gói bằng Docker](https://vanblog.mereith.com/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082503.webp)

Mã nguồn mở xây dựng blog cá nhân tích hợp sẵn trang quản trị, tối ưu SEO, hỗ trợ viết bài bằng Markdown và tự động gia hạn chứng chỉ bảo mật SSL HTTPS. (Đóng góp của [@Mereithhh](https://github.com/ruanyf/weekly/issues/2576))

4、[SvnAdmin: Giao diện Web quản trị tài khoản và phân quyền cho máy chủ SVN](https://github.com/witersen/SvnAdminV2.0)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082505.webp)

Phần mềm PHP hỗ trợ các quản trị viên dễ dàng tạo kho chứa, phân quyền truy cập và quản lý người dùng cho hệ thống kiểm soát mã nguồn Subversion (SVN). (Đóng góp của [@witersen](https://github.com/ruanyf/weekly/issues/2578))

5、[gossip: Tiện ích chuyển đổi GitHub Issues thành trang blog tĩnh chạy Next.js](https://github.com/qianxi0410/gossip)

Công cụ hỗ trợ nhà phát triển viết bài đăng trực tiếp trên mục GitHub Issues của dự án để hệ thống tự động đồng bộ và kết xuất thành blog tĩnh triển khai trên Vercel hoặc GitHub Pages. (Đóng góp của [@qianxi0410](https://github.com/ruanyf/weekly/issues/2581))

6、[BgSub: Công cụ tự động xóa nền ảnh AI chạy trực tiếp trên trình duyệt client](https://bgsub.cn/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082509.webp)

Ứng dụng web hỗ trợ tự động tách nền hình ảnh bằng thuật toán AI xử lý hoàn toàn cục bộ trên máy tính của người dùng, không truyền ảnh lên máy chủ giúp bảo vệ quyền riêng tư. (Đóng góp của [@PearOCR](https://github.com/ruanyf/weekly/issues/2582))

7、[Podcast Together: Tiện ích nghe chung podcast trực tuyến cùng bạn bè](https://github.com/yenche123/podcast-together)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082506.webp)

Mã nguồn mở hỗ trợ thiết lập phòng nghe chung đồng bộ âm thanh các tập podcast từ nguồn Apple Podcast hoặc Xiaoyuzhou cho nhóm người dùng. (Đóng góp của [@yenche123](https://github.com/ruanyf/weekly/issues/2579))

8、[MiraPlayer: Component phát và chỉnh sửa biên tập video dựa trên FFCreator](https://github.com/miravideo/FFCreator)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082504.webp)

Thư viện Front-end hỗ trợ nhà phát triển tích hợp trình phát và công cụ cắt ghép chỉnh sửa video mượt mà trên nền tảng web tận dụng thư viện đồ họa FFCreator của Tencent. (Đóng góp của [@milkliker](https://github.com/ruanyf/weekly/issues/2577))

9、[Solon: Framework phát triển ứng dụng Java gọn nhẹ và khởi động siêu tốc](https://solon.noear.org/)

Giải pháp thay thế Spring Boot hướng tới sự tối giản: tệp tin đóng gói nhỏ gọn, giảm thiểu thời gian khởi động máy chủ và tiết kiệm tài nguyên RAM đáng kể. (Đóng góp của [@noear](https://github.com/ruanyf/weekly/issues/2590))

10、[Codeberg: Nền tảng hosting mã nguồn Git tự do bảo mật](https://codeberg.org/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070111.webp)

Một sự lựa chọn thay thế cho GitHub/GitLab do cộng đồng phi lợi nhuận vận hành nhằm cung cấp dịch vụ lưu trữ mã nguồn mở an toàn tôn trọng quyền riêng tư.

## 资源

1、[WantQuotes (据意查句): Công cụ tìm kiếm câu thơ văn tương ứng theo ý nghĩa](https://wantquotes.net/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081819.webp)

Dự án do Đại học Thanh Hoa phát triển: người dùng chỉ cần gõ các từ khóa tâm trạng (ví dụ: "buồn bã") để hệ thống AI tự động tìm và gợi ý các câu thơ cổ, ngạn ngữ tương đồng ý nghĩa. Độc giả cũng có thể thử nghiệm công cụ tìm [từ đồng nghĩa WantWords](https://wantwords.net/).

2、[Bing Wallpaper: Trang web tổng hợp ảnh nền Bing hàng ngày](https://bing.wdbyte.com/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082507.webp)

Trang web tổng hợp và cho phép tải miễn phí các ảnh phong cảnh chất lượng cao cập nhật từ trang chủ tìm kiếm của Bing hàng ngày. (Đóng góp của [@niumoo](https://github.com/ruanyf/weekly/issues/2591))

3、[Code Heroes (代码英雄): Bản dịch tiếng Trung loạt podcast âm thanh của Red Hat](https://linux.cn/talk/clh/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082508.webp)

Bản dịch chuyên đề tiếng Trung của loạt podcast âm thanh nổi tiếng do Red Hat phát hành giới thiệu lịch sử phát triển của hệ điều hành Linux và phong trào mã nguồn mở. (Đóng góp của [@CherryLover](https://github.com/ruanyf/weekly/issues/2584))

4、[Bunny Fonts: Thư viện phông chữ web nguồn mở thay thế cho Google Fonts](https://fonts.bunny.net/about)

Thư viện phông chữ web thiết kế tối ưu hóa tốc độ tải trang và cam kết bảo vệ dữ liệu người dùng không theo dõi IP để thay thế cho Google Fonts.

## 图片

1\. [Hình ảnh hiển vi các chi tiết chống giả tinh vi trên tờ tiền 50 USD](https://www.hillelwayne.com/post/microscopy/)

Bức ảnh chụp phóng đại bề mặt tờ tiền 50 USD dưới kính hiển vi điện tử:

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040303.webp)

Hệ thống in tiền tích hợp các sợi nylon màu xanh bảo an siêu mỏng đan xen cấu trúc hình ngôi sao, bên trong ngôi sao có dòng chữ siêu nhỏ *"USA FIFTY"* mắt thường khó phát hiện được.

2\. [Hình ảnh ba lô "Người rao bán chính mình" trên tàu điện ngầm Thượng Hải](https://cdn.beekka.com/blogimg/asset/202208/bg2022082407.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082408.webp)

Bức ảnh chụp một hành khách nam đeo ba lô nhựa trong suốt bên trong có dán dòng chữ hài hước: *"Hàng có thể bán, giá cả thương lượng"* trên một chuyến tàu điện ngầm tại Thượng Hải.

3\. [Hiện tượng bùn tuyết (snezhura) độc đáo trên sông Saint Petersburg](https://englishrussia.com/2022/04/01/rare-natural-phenomenon-observed-in-saint-petersburg/)

Hiện tượng tự nhiên kỳ thú xuất hiện khi tuyết rơi dày vào dòng sông có nhiệt độ cận 0°C nhưng dòng chảy chưa đóng băng hoàn toàn:

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040610.webp)

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040611.webp)

Hỗn hợp nước và tuyết tạo thành một lớp màng bùn tuyết trắng xốp trôi bồng bềnh dập dềnh mượt mà trên mặt nước sông như những tấm thảm lông khổng lồ.

## ✍️ Bài đọc thêm

### Ngành công nghiệp chụp ảnh chân dung đại diện cao cấp trị giá hàng ngàn USD tại Mỹ

Trên các mạng xã hội nghề nghiệp như LinkedIn, một bức ảnh chân dung đại diện (headshot) chuyên nghiệp và thu hút đóng vai trò cực kỳ quan trọng giúp ứng viên nâng cao cơ hội tiếp cận nhà tuyển dụng:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081304.webp)

Nhu cầu này thúc đẩy sự hình thành một ngành dịch vụ chụp ảnh chân dung đại diện cao cấp tại Mỹ. Người dùng sẵn sàng chi trả từ 200 USD cho đến hàng ngàn USD cho một buổi chụp hình chân dung:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081305.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081306.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081307.webp)

Các nhiếp ảnh gia chuyên nghiệp phối hợp cùng thợ làm tóc, chuyên gia trang điểm để tư vấn trang phục, góc mặt tối ưu nhất nhằm tạo ra một bức ảnh thể hiện thần thái tự tin, tin cậy của ứng viên.

Các khảo sát thống kê chỉ ra mức chi phí đắt đỏ này mang lại hiệu quả thực tế: hồ sơ cá nhân sở hữu bức ảnh chân dung chuyên nghiệp nhận được lượng truy cập xem hồ sơ cao gấp 21 lần và số lượng yêu cầu kết nối kết bạn cao gấp 9 lần so với hồ sơ không có ảnh đại diện.

## 历史上的本周

- 2021年（第 172 期）：[Khí hậu học: Liệu nhân loại có khả năng tự cứu mình trước nguy cơ thảm họa biến đổi khí hậu toàn cầu](https://www.ruanyifeng.com/blog/2021/08/weekly-issue-172.html)
- 2020年（第 121 期）：[Thảo luận xã hội học: Tại sao năng suất lao động tăng cao nhưng con người không hề trở nên rảnh rỗi hơn](https://www.ruanyifeng.com/blog/2020/08/weekly-issue-121.html)
- 2019年（第 70 期）：[Kinh tế học: Thế giới bước vào kỷ nguyên lãi suất âm và những tác động tới hoạt động đầu tư tài chính](https://www.ruanyifeng.com/blog/2019/08/weekly-issue-70.html)
- 2018年（第 19 期）：[Trải nghiệm tương lai: Nhìn nhận thế giới trò chơi thực tế ảo VR được mô tả qua tác phẩm điện ảnh Ready Player One](https://www.ruanyifeng.com/blog/2018/08/weekly-issue-19.html)

## 鸣谢

Nền tảng quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072108.webp)

（Hết）
