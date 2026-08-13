# Bản tin chia sẻ công nghệ (Số 259): Cách sử dụng ChatGPT miễn phí

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần. (**[Thông báo] Tuần tới nghỉ lễ Đoan Ngọ, bản tin tạm ngưng một kỳ.**)

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3157) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061302.webp)

Tại khu du lịch Vân Môn Sơn ở Thiệu Quan, Quảng Đông có một thác nước nhân tạo cao tới 168 mét đổ xuống vách núi. Nếu dòng nước này được dẫn trực tiếp từ mạch nước ngầm tự nhiên trên núi thì rất tuyệt, nhưng nếu phải sử dụng hệ thống máy bơm công suất lớn để bơm nước ngược từ chân núi lên đỉnh thì quả thực là một sự lãng phí năng lượng không cần thiết. (Nguồn: [Sina](https://k.sina.cn/article_1789187543_p6aa4d5d702700vwsr.html))

## 如何免费使用 ChatGPT

Các phương tiện truyền thông trong nước hàng ngày đưa rất nhiều tin tức sốt dẻo về ChatGPT, nhưng hầu như không bao giờ đề cập trực tiếp đến một sự thật: dịch vụ này không chính thức mở cửa cho người dùng tại Trung Quốc Đại Lục.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061401.webp)

Hệ thống của OpenAI yêu cầu người dùng phải xác thực số điện thoại di động khi đăng ký, và tất cả các đầu số điện thoại di động trong nước đều bị hệ thống từ chối. Nói cách khác, OpenAI chủ động không muốn người dùng trong nước tiếp cận dịch vụ của họ.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061303.webp)

Chúng ta không cần suy đoán sâu xa về lý do đằng sau chính sách này của hãng. Tuy nhiên, tôi tin rằng báo chí không nên cố tình che giấu thực trạng này hay tự huyễn hoặc bản thân, mà cần nói thẳng thắn: **ChatGPT không chào đón người dùng tại Trung Quốc Đại Lục**.

Tất nhiên việc không chào đón không có nghĩa là chúng ta không thể sử dụng. Lập trình viên chỉ cần nhờ người quen ở nước ngoài kích hoạt hộ sim, hoặc đơn giản là mua lại một tài khoản đăng ký sẵn là có thể trải nghiệm bình thường.

Thực tế quy trình cũng không cần phức tạp đến vậy. Có rất nhiều giải pháp thay thế đơn giản và nhanh chóng hơn nhiều. **Quan điểm nhất quán của tôi là chủ nghĩa thực dụng**: chúng ta không cần quá bận tâm đến các rào cản chính sách của OpenAI; chỉ cần công cụ đó mang lại giá trị, chúng ta hãy tìm cách tiếp cận để học hỏi các xu hướng công nghệ mới nhất của thế giới và phá vỡ các rào cản hạn chế kỹ thuật.

Có lẽ rất nhiều lập trình viên cũng chia sẻ chung tư duy này, nhờ đó các trang web proxy và giải pháp truy cập ChatGPT trung gian đã mọc lên như nấm sau mưa. Dưới đây tôi xin tổng hợp lại các phương án phổ biến nhất để bạn đọc tiện tham khảo:

**1. Sử dụng các trang web proxy trung gian miễn phí**

Cộng đồng nhà phát triển quốc tế đã xây dựng dự án nổi tiếng mang tên [FreeGPT](https://freegpt.one/), mở cửa hoàn toàn miễn phí cho người dùng toàn cầu truy cập trực tiếp để trò chuyện với AI mà không yêu cầu đăng ký tài khoản.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061402.webp)

Một trang web có tính năng tương tự là [Chat GPT Demo](https://chatgptdemo.net/zh-hans). Trong nước cũng có rất nhiều trang web tương tự, bạn chỉ cần gõ từ khóa "nguồn ChatGPT" trên công cụ tìm kiếm là có thể tìm ra. Trên GitHub hiện có một số kho lưu trữ lớn chuyên tổng hợp danh sách hàng trăm liên kết proxy miễn phí đang hoạt động ổn định: [Awesome Free ChatGPT 1](https://github.com/LiLittleCat/awesome-free-chatgpt), [2](https://github.com/lzwme/chatgpt-sites), [3](https://github.com/xxxily/hello-ai/blob/main/home/FreeChatGPTSiteList.md).

**2. Sử dụng công cụ Bing Chat**

Trình duyệt Edge của Microsoft đã tích hợp sẵn tính năng Bing Chat kết nối trực tiếp với mô hình ngôn ngữ lớn của OpenAI, cho phép người dùng trò chuyện và thậm chí là yêu cầu AI vẽ tranh hoàn toàn miễn phí:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061403.webp)

Hạn chế duy nhất là tính năng này hiện ưu tiên cho người dùng khu vực Mỹ. Người dùng trong nước muốn trải nghiệm cần truy cập qua IP của Mỹ, đồng thời đăng ký một tài khoản Microsoft mới theo tài liệu hướng dẫn chi tiết tại [Hướng dẫn cấu hình Bing Chat](https://kerrynotes.com/bing-keeps-prompting-to-login-to-continue-chat/).

Bên cạnh đó, ứng dụng nhắn tin [Skype](https://www.skype.com/en/blogs/2023-02-bing-bot-in-skype/) của Microsoft cũng đã được tích hợp sẵn công cụ Bing Chat này:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061404.webp)

Có lẽ nhiều người đã quên mất sự tồn tại của phần mềm Skype, nhưng nó vẫn hoạt động tốt và hỗ trợ đầy đủ ứng dụng khách cho hầu hết các hệ điều hành di động lẫn máy tính. Người dùng chỉ cần cài đặt ứng dụng và tiến hành kết bạn với tài khoản bot của Bing là có thể bắt đầu trò chuyện trực tiếp (Tham khảo thêm [Hướng dẫn kết nối Bing trên Skype](https://www.gizmochina.com/2023/03/04/how-to-add-bing-chatgpt-in-skype/)).

Cuối cùng, có một câu chuyện hậu trường công nghệ khá hài hước:

Trình duyệt di động bên thứ ba Vivaldi do bị Microsoft chặn quyền truy cập các tính năng AI mới nên đã quyết định thay đổi User Agent của trình duyệt để giả lập bản thân là trình duyệt Edge của Microsoft. Kết quả là hiện tại người dùng cài đặt trình duyệt Vivaldi trên Android bỗng nhiên có thể [sử dụng miễn phí tính năng Bing Chat](https://vivaldi.com/blog/vivaldi-on-android-6-1/) một cách dễ dàng.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061521.webp)

## 稀土开发者大会

Như đã thông tin ở các số trước, sự kiện công nghệ quy mô lớn dành cho cộng đồng phát triển **“Hội thảo nhà phát triển Xitu 2023”** đang cận kề ngày tổ chức. Sự kiện sẽ diễn ra vào hai ngày cuối tuần từ **ngày 30 tháng 6 đến ngày 1 tháng 7** tới đây.

Hội thảo được thiết kế với 12 chuyên đề kỹ thuật chuyên sâu cùng sự góp mặt của hơn 60 diễn giả là các kỹ sư công nghệ hàng đầu (Xem [Danh sách diễn giả đầy đủ](https://mp.weixin.qq.com/s/T-cJh_0bJD8l--WAnfebiw)), tập trung chia sẻ các kinh nghiệm thực tế về Frontend, Low-code, Cloud-native, cơ cấu hệ thống phân tán, thiết kế kiến trúc và công nghệ xử lý âm thanh hình ảnh.

Dưới đây là lịch trình của chuyên đề AIGC (Công nghệ sinh nội dung bằng trí tuệ nhân tạo) – một trong những chủ đề nóng nhất hiện nay:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061518.webp)

Đây chỉ là một phần nhỏ trong lịch trình hoạt động đa dạng của hội thảo. Nếu bạn đọc chưa có kế hoạch gì cho hai ngày cuối tuần đó thì đây là cơ hội rất tốt để tham khảo cách làm của các chuyên gia trong ngành.

Ban tổ chức hỗ trợ phát sóng trực tiếp miễn phí cho các khán giả đăng ký trước. Đối với các bạn có điều kiện tham gia trực tiếp tại Bắc Kinh, giá vé phổ thông tham dự 2 ngày (không bao gồm ăn trưa) là 199 tệ. Với đối tượng doanh nghiệp, việc mua các hạng vé VIP kèm suất ăn trưa tại khách sạn sẽ mang lại nhiều cơ hội trò chuyện sâu hơn với các diễn giả bên lề hội thảo. Nếu có nhu cầu mua vé tập thể cho công ty, vui lòng liên hệ WeChat: `@bigeyehan`.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061523.webp)

Bạn đọc có thể truy cập [Trang chủ sự kiện Xitu 2023](https://conf.juejin.cn/xdc2023/?utm_source=ryf0616) hoặc quét mã QR phía trên để xem lịch trình chi tiết, đăng ký nhận link xem trực tuyến hoặc mua vé tham gia. Khán giả đăng ký cũng có cơ hội tham gia chương trình bốc thăm may mắn nhận tai nghe Sony và máy chiếu cao cấp.

## 科技动态

1、[Thiết kế bồn tiểu nam chống bắn nước dựa trên nghiên cứu thủy động lực học](https://arstechnica.com/science/2022/11/the-angle-at-which-dogs-pee-inspired-optimal-design-for-splash-free-urinal/)

Các nhà khoa học tại Đại học Waterloo, Canada đã tiến hành thu thập và kiểm thử nhiều kiểu dáng bồn tiểu nam khác nhau để tìm ra cấu trúc hình học giúp hạn chế tối đa hiện tượng bắn nước tiểu ra ngoài:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112901.webp)

Thông qua các mô phỏng dòng chảy thủy động lực học trên máy tính, họ chỉ ra rằng thiết kế bồn tiểu tối ưu nhất chính là mẫu thiết kế thứ 2 từ bên phải sang: một cấu trúc bọc cao và thu hẹp dần về phía dưới.

Đồng thời, họ cũng đề xuất giải pháp lót thêm các tấm vật liệu có khả năng hấp thụ lực và thấm hút mạnh ở phần đáy bồn tiểu để tạo hiệu ứng triệt tiêu lực chảy của dòng nước tương tự như "hố đen".

2、[Mỹ chính thức phê duyệt thương mại hóa các sản phẩm thịt nhân tạo nuôi cấy từ tế bào](https://www.npr.org/sections/health-shots/2022/11/14/1136186819/cultivated-cultured-meat-heathy-climate-change)

Cục Quản lý Thực phẩm và Dược phẩm Mỹ (FDA) vừa qua đã chính thức cấp phép cho một sản phẩm thịt gà được sản xuất bằng phương pháp nuôi cấy tế bào động vật được phép bán ra thị trường tiêu dùng:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112902.webp)

Sản phẩm thịt này không được thu hoạch từ quá trình giết mổ gia cầm truyền thống mà được sản xuất khép kín hoàn toàn trong phòng thí nghiệm.

Quy trình sản xuất bắt đầu bằng việc trích xuất các tế bào cơ của gà, đặt vào các bồn nuôi cấy vô trùng và châm thêm các chất dinh dưỡng thiết yếu (bao gồm chất béo, đường, axit amin và vitamin) để tế bào tự động nhân bản và liên kết lại tạo thành các mớ cơ thịt hoàn chỉnh.

Nhà máy trưng bày trong hình có công suất sản xuất khoảng 22 tấn thịt nhân tạo mỗi năm. Toàn bộ nguyên liệu dinh dưỡng được truyền qua hệ thống ống dẫn vào các bồn thép lớn để nuôi cấy tế bào tạo ra thịt tươi thành phẩm:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112903.webp)

Thịt nuôi cấy sở hữu nhiều ưu điểm vượt trội như tiết kiệm diện tích đất chăn nuôi, giảm thiểu ô nhiễm chất thải nông nghiệp và thân thiện với môi trường. Dòng sản phẩm thịt gà nhân tạo đầu tiên này được đánh giá là có hương vị và cấu trúc mô thịt rất giống với thịt gà tự nhiên.

3、[Đức thử nghiệm tổ chức buổi lễ nhà thờ được dẫn dắt hoàn toàn bởi AI](https://apnews.com/article/germany-church-protestants-chatgpt-ai-sermon-651f21c24cfb47e3122e987a7263d348)

Vào ngày 9 tháng 6 vừa qua, tại một nhà thờ ở Đức đã diễn ra một buổi lễ cầu nguyện đặc biệt được điều hành hoàn toàn bởi trí tuệ nhân tạo trước sự chứng kiến của hàng trăm tín đồ:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061202.webp)

Phía trên bục giảng đạo được trang bị một màn hình lớn hiển thị hình ảnh đại diện AI là một người đàn ông da màu có râu. AI đã trực tiếp dẫn dắt buổi lễ và đọc bài giảng đạo dài 40 phút cho hơn 300 tín đồ có mặt tại khán phòng. Toàn bộ nội dung bài giảng, lời cầu nguyện và các đoạn nhạc thánh ca đều do công cụ ChatGPT tự động biên soạn.

Nhiều người tham gia đánh giá buổi lễ diễn ra rất suôn sẻ và mang lại trải nghiệm mới lạ vượt kỳ vọng. Tuy nhiên, một số tín đồ bày tỏ cảm giác không thoải mái khi nghe bài giảng: *"Nội dung bài giảng nghe rất trôi chảy nhưng thiếu đi hoàn toàn cảm xúc và tâm hồn của một người truyền giáo thực thụ"*.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061203.webp)

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061204.webp)

Nếu AI có thể đảm nhận tốt các vai trò nghi lễ tôn giáo phức tạp, nó hoàn toàn có thể được ứng dụng để làm trợ lý tư vấn tâm lý, lắng nghe và trò chuyện giải tỏa căng thẳng cho các bệnh nhân trong tương lai.

4、[Ý tưởng biến cánh cửa cổng gia đình thành một cây đàn phong cầm độc đáo](https://www.windmusik.com/html/turharfe.htm#T)

Một người yêu nhạc tại Đức đã tự tay lắp đặt hệ thống dây đàn lên phần ô thoáng của cánh cửa cổng nhà mình, biến nó thành một nhạc cụ phát nhạc tự nhiên nhờ sức gió:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081803.webp)

Anh đã khoét một khe thông gió lớn trên cánh cửa gỗ để luồng gió tự nhiên có thể thổi qua dễ dàng, sau đó căng các sợi dây đàn kim loại ngang qua khe gió này để khi gió thổi qua sẽ làm rung các dây đàn phát ra âm thanh:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081805.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081804.webp)

Sau quá trình căn chỉnh cao độ tỉ mỉ cho từng sợi dây, tiếng đàn phát ra mỗi khi có gió thổi nghe rất êm dịu, hài hòa như tiếng nhạc của thiên nhiên và không bao giờ bị trùng lặp do cường độ gió luôn thay đổi.

## Bài viết

1\. [Đánh giá kết quả làm bài thi toán THPT quốc gia của ChatGPT](https://mp.weixin.qq.com/s/HG_Axf38ljcaQTfi9pyJvA)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061522.webp)

Bài viết thực nghiệm cho ChatGPT thử sức với đề thi môn Toán trong kỳ thi tốt nghiệp THPT quốc gia năm 2023 của Trung Quốc để xem mô hình AI này đạt được bao nhiêu điểm và gặp khó khăn ở các dạng toán nào.

2\. [Cảnh báo nguy cơ AI suy giảm trí thông minh khi huấn luyện bằng dữ liệu do chính nó tạo ra](https://m.thepaper.cn/newsDetail_forward_23467960)（Tiếng Trung）

Một nhóm nghiên cứu tại Anh chỉ ra rằng việc sử dụng các dữ liệu do AI thế hệ trước sinh ra để làm dữ liệu huấn luyện cho các thế hệ AI tiếp theo sẽ dẫn đến hiện tượng suy thoái mô hình (Model Collapse), khiến AI ngày càng trở nên ngớ ngẩn và mất đi khả năng tư duy đa dạng.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061509.webp)

3\. [Tìm hiểu thuật toán CORDIC giúp tính toán nhanh các giá trị lượng giác](http://www.longluo.me/blog/2023/06/07/CORDIC-algorithm/)（Tiếng Trung）

Bài viết giới thiệu thuật toán CORDIC – một giải pháp toán học giúp máy tính tính toán nhanh các giá trị lượng giác (sin, cos) chỉ bằng các phép toán cộng trừ và dịch bit cơ bản, thay vì phải chạy các phép tính lũy thừa phức tạp của chuỗi Taylor. (Đóng góp của [@longluo](https://github.com/ruanyf/weekly/issues/3183))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061508.webp)

4\. [Hướng dẫn sử dụng Cloudflare Tunnel để kết nối SSH xuyên tường lửa](https://iq.thc.org/tunnel-via-cloudflare-to-any-tcp-service)（Tiếng Anh）

Bài viết hướng dẫn lập trình viên thiết lập cổng kết nối an toàn Cloudflare Tunnel để truy cập từ xa vào các máy chủ nằm sâu trong mạng nội bộ hoặc phía sau tường lửa mà không cần cấu hình mở cổng NAT trên router.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052005.webp)

5\. [Ứng dụng mô hình AI Whisper để tự động tạo phụ đề cho video](https://www.spapas.net/2023/05/22/ai-auto-subtitling/)（Tiếng Anh）

Bài viết hướng dẫn chi tiết cách cài đặt và chạy mô hình nhận dạng giọng nói Whisper của OpenAI để tự động chuyển đổi âm thanh hội thoại trong video thành văn bản và xuất ra tệp phụ đề SRT chuẩn xác.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052208.webp)

6\. [Góc nhìn phản biện: Không phải lúc nào cơ sở dữ liệu cũng cần thiết lập Index](https://www.jefftk.com/p/you-dont-always-need-indexes)（Tiếng Anh）

Các giáo trình luôn khuyên lập trình viên phải tạo bộ chỉ mục (Index) cho các bảng dữ liệu để tối ưu tốc độ truy vấn. Tuy nhiên bài viết chỉ ra với các bảng dữ liệu có dung lượng nhỏ, việc quét toàn bộ bảng (Table Scan) đôi khi lại cho tốc độ nhanh hơn và tiết kiệm dung lượng bộ nhớ hơn so với việc duy trì Index.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052601.webp)

7\. [Hướng dẫn sử dụng Stable Diffusion để biến mã QR thành tác phẩm nghệ thuật](https://stable-diffusion-art.com/qr-code/)（Tiếng Anh）

Bài viết hướng dẫn chi tiết cách thức ứng dụng công cụ Stable Diffusion kết hợp ControlNet để nhúng chìm mã QR vào bên trong các bức tranh vẽ nghệ thuật bắt mắt mà camera điện thoại vẫn có thể nhận diện và quét được liên kết một cách chính xác.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061301.webp)

8\. [Visual Information Theory: Bài viết trực quan hóa lý thuyết thông tin](https://colah.github.io/posts/2015-09-Visual-Information/)（Tiếng Anh）

Một bài viết phân tích khoa học sử dụng rất nhiều biểu đồ trực quan sinh động để giải thích các khái niệm trừu tượng của Lý thuyết thông tin (như entropy, thông tin tương hỗ) giúp người đọc dễ dàng tiếp thu kiến thức.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052501.webp)

9\. [So sánh hiệu năng giữa máy lọc không khí và hệ thống cấp khí tươi áp suất dương](https://www.airgradient.com/open-airgradient/blog/air-purifier-vs-positive-pressure-fresh-air-system-an-unfair-battle/)（Tiếng Anh）

Để duy trì không khí trong lành trong nhà, chúng ta có hai giải pháp: sử dụng máy lọc không khí tuần hoàn trong phòng hoặc lắp đặt hệ thống cấp gió tươi áp suất dương để ép bụi bẩn không thể lọt qua khe cửa vào nhà. Bài viết thực nghiệm so sánh chi tiết hiệu quả của hai phương án này.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060905.webp)

## 工具

1、[Mosh: Công cụ kết nối terminal thay thế SSH cho kết nối mạng không ổn định](https://mosh.org/)

Một giải pháp thay thế SSH xuất sắc dành cho lập trình viên hay di chuyển. Điểm ưu việt của Mosh là khả năng duy trì phiên làm việc terminal liên tục ngay cả khi thiết bị mất mạng tạm thời hoặc thay đổi IP kết nối (như chuyển từ mạng Wifi sang mạng di động 4G).

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042008.webp)

2、[Ezno: Trình biên dịch TypeScript hiệu năng cao viết bằng Rust](https://github.com/kaleidawave/ezno)

Dự án phát triển trình biên dịch TypeScript mới viết hoàn toàn bằng Rust, hướng tới mục tiêu thay thế trình biên dịch `tsc` chính thức của Microsoft nhằm cải thiện tối đa tốc độ biên dịch mã nguồn của dự án.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060906.webp)

3、[Bark: Mô hình AI chuyển đổi văn bản thành giọng nói sinh động](https://github.com/suno-ai/bark)

Công cụ chuyển đổi văn bản thành giọng nói (TTS) thế hệ mới có khả năng mô phỏng giọng đọc tự nhiên của con người, tích hợp các biểu cảm giọng nói như tiếng cười, tiếng thở dài hay tiếng khóc, đồng thời hỗ trợ tự động tạo nhạc nền đi kèm.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042101.webp)

4、[trzsz-ssh: Trình khách SSH viết bằng Go hỗ trợ truyền tải file nhanh](https://github.com/trzsz/trzsz-ssh)

Ứng dụng client SSH viết bằng Go hỗ trợ ghi nhớ danh sách máy chủ đã truy cập, tích hợp sẵn tính năng kéo thả truyền tải tệp tin nhanh chóng giữa máy tính và server. (Đóng góp của [@lonnywong](https://github.com/ruanyf/weekly/issues/3180))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061506.webp)

5、[STDF: Bộ linh kiện giao diện di động dựa trên Svelte và Tailwind](https://github.com/dufu1991/stdf)

Bộ sưu tập các component giao diện tinh tế dành riêng cho ứng dụng di động Web, được xây dựng trên nền tảng framework Svelte kết hợp Tailwind CSS. (Đóng góp của [@dufu1991](https://github.com/ruanyf/weekly/issues/3175))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061503.webp)

6、[code-inspector: Tiện ích hỗ trợ tìm nhanh dòng code từ giao diện Vue](https://github.com/zh-lx/code-inspector)

Công cụ hỗ trợ phát triển dành riêng cho Vue: người dùng chỉ cần nhấp chuột vào một phần tử giao diện bất kỳ trên trình duyệt, hệ thống sẽ tự động gọi IDE mở đúng file mã nguồn và di chuyển con trỏ tới đúng dòng code định nghĩa phần tử đó. (Đóng góp của [@zh-lx](https://github.com/ruanyf/weekly/issues/3178))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061504.webp)

7、[Tiny Player: Trình phát video web tối giản hỗ trợ tùy biến giao diện](https://tiny-player.vercel.app/)

Trình phát video mini chạy trên nền web hỗ trợ tốt cả hai phương thức giải mã cứng và mềm, cho phép lập trình viên tự do thiết kế lại kiểu dáng các nút điều khiển. (Đóng góp của [@wangrongding](https://github.com/ruanyf/weekly/issues/3174))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061505.webp)

8、[BrutalityExtractor: Phần mềm giải nén tối ưu hóa đa nhân cho Windows](https://github.com/hxz393/BrutalityExtractor)

Ứng dụng giải nén dữ liệu nguồn mở trên Windows được tối ưu hóa sâu để tận dụng tối đa sức mạnh của các dòng CPU đa nhân và ổ cứng SSD tốc độ cao bằng cách chia nhỏ tệp tin để chạy giải nén đa tiến trình song song. (Đóng góp của [@hxz393](https://github.com/ruanyf/weekly/issues/3181))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061507.webp)

9、[highlight.io: Nền tảng giám sát lỗi giao diện frontend nguồn mở](https://github.com/highlight/highlight)

Hệ thống ghi nhận và phân tích lỗi giao diện (Frontend Monitoring) tự lưu trữ an toàn, cung cấp đầy đủ các tính năng giám sát lỗi thời gian thực và ghi lại phiên hoạt động của người dùng tương tự như Sentry.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042201.webp)

10、[Keyv: Thư viện quản lý lưu trữ key-value đa cơ sở dữ liệu](https://keyvhq.js.org/)

Thư viện JS cung cấp giao diện lập trình key-value tối giản hỗ trợ kết nối đồng bộ dữ liệu ra nhiều hệ quản trị CSDL backend khác nhau từ SQL (MySQL, PostgreSQL, SQLite) cho đến NoSQL (Redis, Memcached).

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042404.webp)

11、[Jellylade: Tiện ích web hỗ trợ chụp và trang trí ảnh chụp màn hình](https://app.jellylade.com/)

Công cụ web trực tuyến giúp người dùng nhanh chóng tạo ra các bức ảnh chụp màn hình trang web đẹp mắt kèm hiệu ứng đổ bóng và bo góc để chèn vào các bài viết blog.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042602.webp)

## 资源

1\. [China Universities Map: Bản đồ phân cấp danh sách các trường đại học tại Trung Quốc](https://laosheng.top/fuwu/yuanxiao)

Trang web tổng hợp và phân loại chi tiết danh sách kèm liên kết trang chủ của hàng ngàn trường đại học, cao đẳng trên cả nước, được phân chia khoa học theo các cấp quản lý nhà nước từ trung ương đến địa phương. (Đóng góp của [@DiamonWoo](https://github.com/ruanyf/weekly/issues/3173))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061502.webp)

2、[Prompt Engineering Guide: Cẩm nang hướng dẫn viết câu lệnh Prompt cho AI](https://www.promptingguide.ai/)

Cuốn sách điện tử trực tuyến miễn phí cung cấp các kiến thức nền tảng và các mẹo thực hành viết câu lệnh Prompt tối ưu khi làm việc với các mô hình ngôn ngữ lớn.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060301.webp)

3、[GitHub Actions by Example: Giáo trình học GitHub Actions qua ví dụ](https://www.actionsbyexample.com/)

Trang web giới thiệu chi tiết cách thức xây dựng các tệp cấu hình tự động hóa quy trình CI/CD thông qua 10 ví dụ thực tế có kèm chú thích cụ thể cho từng dòng lệnh.

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012504.webp)

4\. [Introduction to Compilers: Giáo trình nhập môn thiết kế trình biên dịch](https://www3.nd.edu/~dthain/compilerbook/)

Cuốn sách giáo trình đại học viết bằng tiếng Anh giới thiệu các nguyên lý thiết kế trình biên dịch và ngôn ngữ lập trình, tài liệu được cập nhật mới nhất vào năm 2021 và hỗ trợ tải về đọc miễn phí.

## 图片

1、**Sự suy giảm màu sắc của môi trường sống xung quanh chúng ta**

Một tài khoản trên mạng xã hội Twitter đã chia sẻ bài phân tích chỉ ra một hiện tượng thú vị: thế giới xung quanh chúng ta dường như đang ngày càng ít màu sắc hơn so với quá khứ.

Đây là hình ảnh bãi đỗ xe ô tô vào những năm trước đây với đa dạng sắc màu xanh, đỏ, vàng:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072811.webp)

Và đây là hình ảnh bãi đỗ xe ngày nay với tông màu chủ đạo chỉ xoay quanh đen, trắng và xám:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072812.webp)

Đây là thiết kế nội thất phòng ngủ cổ điển rực rỡ màu sắc:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072813.webp)

Và đây là thiết kế nội thất căn phòng hiện đại tối giản với tông màu trung tính chủ đạo:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072814.webp)

Tác giả bài viết nhận định xu hướng thiết kế công nghiệp ngày nay đang ngày càng thu hẹp dải màu sử dụng vào một số tông màu cơ bản tối giản, làm mất đi sự sống động của cuộc sống. Bạn có đồng tình với quan điểm này không?

2、**Các mẫu tàu ngầm tự chế độc đáo của các băng nhóm buôn lậu ma túy**

Các băng nhóm tội phạm ma túy tại Colombia đã tự thiết kế các mẫu tàu bán ngầm phục vụ vận chuyển hàng lậu xuyên đại dương:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010601.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010602.webp)

Các dòng tàu này thực chất không lặn sâu hoàn toàn dưới lòng nước mà chỉ mấp mé sát mặt nước để che mắt các hệ thống tuần tra bằng radar của lực lượng cảnh sát biển:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010603.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010604.webp)

Điều đáng kinh ngạc là toàn bộ các tàu ngầm này đều được lắp ráp thủ công tại các nhà xưởng dã chiến ẩn sâu trong rừng rậm nhiệt đới Colombia:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010605.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010606.webp)

Quy mô của các xưởng cơ khí dã chiến này đủ lớn để hoàn thiện các vỏ tàu composite chịu áp lực nước tốt, cho thấy tiềm lực tài chính khổng lồ của các băng nhóm này:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010607.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010608.webp)

## ✍️ Bài đọc thêm

### Trong tương lai, thế hệ sau sẽ lấy gì để hoài niệm về quá khứ của chúng ta?

Ngày xửa ngày xưa, trong mỗi gia đình Thụy Điển bình dân thường chỉ sở hữu một cuốn sách duy nhất, đó là cuốn *Kinh Thánh*. Cuốn sách này được trân trọng truyền qua nhiều thế hệ trong dòng họ.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061512.webp)

Mỗi khi mở trang sách cũ ra, bạn sẽ nhớ rằng ông nội và cha mình cũng từng lật qua trang giấy này. Bên trong cuốn sách thường lưu giữ những kỷ vật nhỏ của gia đình: một bức thư tay, một mẩu tin báo cắt rời hay một bức ảnh cưới đã úa vàng theo thời gian.

Nhiều năm sau đó khi máy tính xuất hiện, mọi người bắt đầu lưu trữ hình ảnh gia đình vào các đĩa mềm và đĩa CD. Trải qua 30 năm, các định dạng file đó hiện vẫn có thể được mở ra đọc dễ dàng trên các máy tính hiện đại:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061513.webp)

Và rồi thời đại điện thoại thông minh cùng công nghệ điện toán đám mây bùng nổ, mọi thói quen lưu giữ ký ức đã thay đổi hoàn toàn.

Hiện nay do chi phí lưu trữ đám mây và băng thông mạng quá rẻ, mọi người bắt đầu có xu hướng ném hàng trăm GB, thậm chí hàng TB hình ảnh chụp hàng ngày lên mây:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061514.webp)

Chúng ta đang ghi lại chi tiết cuộc sống hàng ngày với khối lượng ảnh khổng lồ chưa từng có trong lịch sử nhân loại, tự tin rằng các kho lưu trữ số hóa đó sẽ trường tồn mãi mãi.

Bạn chụp ảnh mọi thứ xung quanh mình: từ món ăn trưa, bộ quần áo mặc hàng ngày, cảnh hoàng hôn, hàng cây ven đường cho đến cốc bia, đôi giày và những góc phố. Tuy nhiên, hầu như bạn không bao giờ dành thời gian mở ra xem lại chúng. Bạn chỉ đơn giản là phó mặc toàn bộ ký ức đó cho các tập đoàn công nghệ quản lý trên các hệ thống máy chủ mà bạn không hề có quyền kiểm soát thực tế. Liệu các dịch vụ lưu trữ này có biến mất vào ngày mai không? Ngay cả khi chúng vẫn hoạt động, 50 năm nữa liệu nền tảng YouTube, Instagram hay Dropbox có còn tồn tại?

**Tôi luôn tự hỏi, thế hệ tương lai sẽ làm thế nào để hoài niệm về quá khứ của cha ông họ?** Ngay cả khi toàn bộ kho ảnh khổng lồ này được bảo toàn nguyên vẹn trên mây, số lượng ảnh quá nhiều sẽ khiến việc tìm kiếm và xem lại trở nên vô cùng loãng, trong khi các kỷ vật vật lý sờ nắm được lại quá khan hiếm.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061516.webp)

Bà ngoại tôi khi về già mắc chứng mất trí nhớ và phải chuyển vào viện dưỡng lão. Phương pháp duy nhất giúp bà cảm thấy thoải mái và gợi lại phần nào ký ức là cùng lật giở những bức ảnh cũ. Những bức ảnh đó được cất giữ cẩn thận trong một hộp gỗ đựng xì gà cũ, nhiều bức ảnh đã bạc màu và sờn góc sau hàng chục năm lưu giữ.

Đến khi thế hệ chúng ta về già, chúng ta sẽ không còn những cuốn album ảnh sờn góc đầy vết mòn thời gian như thế nữa, khi đó chúng ta sẽ lấy gì để hoài niệm về những năm tháng đã qua?

## Lịch sử tuần này

- 2022年（第 212 期）：[Triết lý cuộc sống: Phân tích các luận điểm chứng minh cuộc đời con người thực ra không hề ngắn ngủi](http://www.ruanyifeng.com/blog/2022/07/weekly-issue-212.html)
- 2021年（第 162 期）：[Trải nghiệm: Tại sao cuộc sống của chúng ta có nhiều nét tương đồng với trò chơi Pac-Man](http://www.ruanyifeng.com/blog/2021/06/weekly-issue-162.html)
- 2020年（第 112 期）：[Quản trị: Phương pháp rèn luyện và nâng cao năng lực lãnh đạo cho lập trình viên](http://www.ruanyifeng.com/blog/2020/06/weekly-issue-112.html)
- 2019年（第 62 期）：[Phim hay: Giới thiệu bộ phim điện ảnh Nhật Bản “Fune wo Amu” kể về hành trình biên soạn từ điển đầy ý nghĩa](http://www.ruanyifeng.com/blog/2019/06/weekly-issue-62.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes team collaboration smooth and efficient.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
