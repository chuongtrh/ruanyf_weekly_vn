# Bản tin chia sẻ công nghệ (Số 370): Tô sáng cú pháp (syntax highlighting) chuẩn xác

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/7832) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102301.webp)

Ngôi cổ tự nghìn năm Linh Nhạc Tự ở quận Môn Đầu Câu, Bắc Kinh, vốn đóng cửa từ năm 1979, nay đã hoàn thành đợt trùng tu và chính thức mở cửa đón khách tham quan từ tháng này. Trong quá trình sửa sang, người ta đã giữ lại một ô kính quan sát trên tường để hiển thị các lớp gạch nung nguyên bản từ thời nhà Đường và nhà Liêu. ([visuals_china@instagram](https://www.instagram.com/p/DQEjgx-EUNN/?img_index=6))

## 正确的代码高亮

Lập trình viên thường sử dụng các công cụ tô sáng cú pháp (syntax highlighting) để hiển thị mã nguồn dưới nhiều màu sắc khác nhau (như hình dưới) nhằm dễ dàng đọc hiểu.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102304.webp)

Câu hỏi đặt ra là: **Bảng phối màu như thế nào sẽ tối ưu nhất cho việc đọc hiểu mã nguồn?**

Hầu hết mọi người (trong đó có tôi) thường chọn màu sắc theo sở thích cá nhân. Ví dụ như bảng phối màu sặc sỡ dưới đây trông vô cùng bắt mắt:

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101704.webp)

Cách đây không lâu, tôi có đọc [một bài viết](https://tonsky.me/blog/syntax-highlighting/), trong đó tác giả lập luận rằng: các bảng màu trông đẹp mắt chưa chắc đã phù hợp cho việc đọc hiểu mã nguồn.

Một hệ thống tô sáng cú pháp chuẩn xác phải giúp người đọc nắm bắt được những thông tin cốt lõi nhất ngay từ cái nhìn đầu tiên. Việc lạm dụng quá nhiều màu sắc chỉ gây rối mắt và làm phân tán sự tập trung.

Tác giả đề xuất 5 nguyên tắc thiết kế tô màu code:

（1）**Chỉ sử dụng tối đa 4 màu sắc khác nhau**, việc dùng nhiều màu hơn sẽ làm loãng sự tập trung.

（2）**Việc định nghĩa biến, hàm và lớp là quan trọng nhất**. Thông thường, đây là những phần cốt lõi của mã nguồn, do đó tên biến, tên hàm và tên lớp khi định nghĩa cần được tô màu nổi bật.

（3）**Các chú thích (comments) cũng vô cùng quan trọng**, vì chúng thường chứa đựng những thông tin giải thích then chốt hoặc thông điệp mà tác giả muốn gửi gắm tới người đọc sau này. Do đó, chú thích cần được tô màu rõ ràng. Việc nhiều bảng phối màu làm mờ (gray out) phần chú thích là không hợp lý.

（4）**Hằng số và các dấu ngoặc lồng nhau cũng là thông tin quan trọng** cần được tô màu nổi bật.

（5）**Các phần mã nguồn khác không cần thiết phải tô màu**, bao gồm việc gọi biến, gọi hàm và các từ khóa khai báo (như `class`, `function`, `if`, `else`, v.v.). Bởi vì chúng xuất hiện ở khắp mọi nơi, và lập trình viên hiếm khi phải chủ động tìm kiếm chúng.

Bạn có đồng ý với 5 nguyên tắc này không?

Nếu thấy hợp lý, bạn có thể trải nghiệm thử bảng phối màu [Alabaster](https://github.com/tonsky/sublime-scheme-alabaster#variations-1) do chính tác giả bài viết thiết kế.

Hình dưới đây là hiệu ứng tô màu của bảng phối màu Alabaster:

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101706.webp)

Để so sánh, hãy nhìn lại hiệu ứng của bảng phối màu sặc sỡ ban đầu:

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101705.webp)

Theo bạn, phương án nào cho hiệu ứng tốt hơn và làm nổi bật các thông tin quan trọng của mã nguồn hơn?

## 大模型 API 怎么买

Nếu cần sử dụng đồng thời mô hình AI của nhiều nhà cung cấp khác nhau, bạn sẽ giải quyết thế nào, mua tài khoản API của từng bên một?

Hôm nay tôi xin giới thiệu một dịch vụ "AI Gateway" mà tôi đang sử dụng, hỗ trợ **gọi hơn 50 dòng mô hình AI phổ biến thông qua một cổng kết nối duy nhất**. Đó chính là [Nền tảng suy luận mô hình AI của Qiniu Cloud](https://s.qiniu.com/JrUbmm).

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102313.webp)

Họ cung cấp hầu hết các mô hình phổ biến hiện nay (như mô hình nước ngoài của OpenAI, Gemini, Claude và mô hình nội địa Trung Quốc như DeepSeek, Qwen, Doubao, Zhipu, Kimi). Mục [Model Plaza](https://t.wangbase.com/AR4lw) (hình trên) liệt kê một số mô hình tiêu biểu, và bạn có thể [tra cứu danh sách API đầy đủ](https://developer.qiniu.com/aitokenapi/13000/claude-inference-api#3).

Qiniu Cloud (七牛云) là nhà cung cấp dịch vụ đám mây lâu đời của Trung Quốc với 15 năm hoạt động và đã niêm yết trên thị trường chứng khoán, do đó dịch vụ rất đáng tin cậy. Bạn hoàn toàn có thể yên tâm về tính ổn định cũng như chất lượng dịch vụ chăm sóc khách hàng ở đây.

Việc sử dụng "cổng kết nối hợp nhất" này mang lại một số ưu điểm vượt trội: (1) **Sử dụng thuận tiện**, đăng ký và thanh toán trực tiếp bằng Nhân dân tệ, không yêu cầu thẻ tín dụng quốc tế; (2) **Tích hợp dễ dàng**, hỗ trợ kết nối nhanh vào các ứng dụng khách AI, IDE, công cụ dòng lệnh hay MCP, tương thích tốt với cả cấu trúc API của OpenAI và Claude; (3) **Độ trễ thấp + Băng thông cao**, kết quả đo lường bằng [AIPerf](https://www.aiperf.top/test) khi gọi mô hình của Google cho thời gian phản hồi trung bình chỉ hơn 700 ms và tốc độ đạt 184.6 Token/s; (4) **Giới hạn băng thông (Rate limit) cao**, tài khoản thông thường được hỗ trợ tối đa 500 yêu cầu/phút và 5 triệu token/phút, hoàn toàn đáp ứng tốt nhu cầu sử dụng thông thường.

Hiện tại, chương trình khuyến mãi dành cho người dùng mới của họ vẫn đang diễn ra. <u>Người dùng mới đăng ký sẽ nhận miễn phí 3 triệu Token, và nếu mời thêm bạn bè sử dụng, bạn sẽ nhận thêm 5 triệu Token, đồng thời người được mời cũng nhận được 10 triệu Token</u>.

Tóm lại, nếu bạn đăng ký qua [liên kết giới thiệu của tôi](https://s.qiniu.com/JrUbmm) (hình dưới), bạn sẽ nhận ngay 3 triệu + 10 triệu Token miễn phí. Sau đó, bạn có thể tạo mã giới thiệu của riêng mình để tiếp tục nhận thêm 5 triệu Token cho mỗi lượt mời thành công.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102402.webp)

## 科技动态

1. Tuần này, một chiếc máy bay hành khách Boeing 737 Max của Mỹ khi đang bay ở độ cao 11.000 mét đã bị [một vật thể lạ va trúng](https://economictimes.indiatimes.com/news/international/us/united-airlines-737-max-carrying-140-passengers-to-lax-diverts-after-mysterious-object-cracks-cockpit-windshield-midair-pilot-injured/articleshow/124683266.cms), làm vỡ kính chắn gió phía trước cabin phi công và khiến phi công trưởng bị thương nhẹ do nhiều mảnh kính nhỏ cứa vào tay.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102008.webp)

Ở độ cao lớn như vậy, thủ phạm không thể là chim, và dựa trên các vết cháy xém do nhiệt độ cao trên kính chắn gió, nguyên nhân cũng được loại trừ là do mưa đá. Khả năng cao nhất chỉ có thể là thiên thạch nhỏ hoặc rác vũ trụ (rác không gian).

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102009.webp)

Nếu được xác định là do rác vũ trụ, đây sẽ là trường hợp máy bay đầu tiên trong lịch sử bị va chạm bởi rác không gian.

*(Cập nhật: Thông tin mới nhất cho biết chiếc máy bay rất có thể đã va chạm với một khinh khí cầu thời tiết ở tầng cao. Đây cũng sẽ là trường hợp va chạm đầu tiên ghi nhận trong lịch sử giữa máy bay và khinh khí cầu).*

2. Một công ty lốp xe của Trung Quốc tại thành phố Trường Xuân, tỉnh Cát Lâm, đã chế tạo thành công [chiếc lốp xe lớn nhất thế giới](https://finance.sina.cn/tech/2025-10-19/detail-infumsek4716883.d.html).

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102002.webp)

Lốp xe này sở hữu đường kính vượt quá 4 mét và có trọng lượng nặng hơn 6 tấn, được thiết kế chuyên biệt dành cho các dòng xe ben khai mỏ khổng lồ hoạt động tại các mỏ lộ thiên.

3. Quốc gia nào trên thế giới không có muỗi?

Trước đây, quốc gia duy nhất được ghi nhận hoàn toàn không có muỗi là Iceland. Tuy nhiên tuần này, một nông dân Iceland đã phát hiện ra 3 con [muỗi còn sống](https://www.npr.org/2025/10/22/nx-s1-5582748/iceland-mosquitoes-first-time) tại trang trại của gia đình mình.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102305.webp)

Từ nay, mọi quốc gia trên hành tinh đều đã xuất hiện loài muỗi.

Chính phủ Iceland nhận định những con muỗi này có thể đã theo các chuyến bay hoặc tàu biển du lịch du nhập vào nước này. Nhưng nguyên nhân sâu xa là hiện tượng ấm lên toàn cầu đã tạo điều kiện khí hậu phù hợp cho loài muỗi có thể sinh sống và sinh sản tại các khu vực vĩ độ cao.

4. Nghiên cứu của Đại học Mie (三重大学) Nhật Bản chỉ ra rằng [mùa hè tại Nhật Bản](https://english.kyodonews.net/articles/-/62626) hiện đã kéo dài hơn 3 tuần so với thời điểm 42 năm trước (năm 1982).

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101201.webp)

Đây là biểu hiện rõ nét của biến đổi khí hậu: mùa hè ngày càng kéo dài và nóng bức hơn, thời gian mùa đông hầu như giữ nguyên, trong khi mùa xuân và mùa thu bị thu hẹp đáng kể, chỉ còn kéo dài khoảng 1 đến 2 tuần.

5. Công ty X (trước đây là Twitter) chính thức ra mắt [thị trường mua bán tên người dùng (username/handle marketplace)](https://www.engadget.com/social-media/xs-handle-marketplace-will-sell-some-rare-usernames-for-millions-of-dollars-224852740.html), cho phép người dùng đấu giá mua lại các tên tài khoản đã bị thu hồi.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102110.webp)

Chính sách của nền tảng quy định nếu tài khoản không đăng nhập trong một khoảng thời gian nhất định (ví dụ 6 tháng), tên người dùng sẽ bị thu hồi. Tuy nhiên, cách xử lý các tên tài khoản này ở mỗi mạng xã hội là khác nhau.

X là nền tảng lớn đầu tiên công khai bán đấu giá các tên tài khoản đã thu hồi. Một số tên tài khoản hiếm (ví dụ như @one, @fly, @compute) có mức giá khởi điểm từ 2.500 USD và có thể lên tới 1 triệu USD.

Sự việc này một lần nữa nhắc nhở chúng ta rằng tên tài khoản không thực sự thuộc quyền sở hữu của bạn mà thuộc về nền tảng. Nền tảng chỉ tạm thời cho bạn mượn và họ có thể thu hồi bất cứ lúc nào.

## 文章

1. [TypeScript rất giống với C#](https://typescript-is-like-csharp.chrlschn.dev/pages/intro-and-motivation.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025100916.webp)

Bài viết phân tích sự tương đồng lớn trong cú pháp giữa hai ngôn ngữ TypeScript và C#, một điều dễ hiểu khi cả hai đều được thiết kế bởi cùng một kiến trúc sư ngôn ngữ (Anders Hejlsberg).

Do đó, khi cần tối ưu hóa hiệu năng chuyên sâu cho mã nguồn TypeScript, nhà phát triển có thể cân nhắc chuyển đổi mã nguồn sang C# (ngôn ngữ hiện đã hỗ trợ chạy đa nền tảng rất tốt).

2. [Cách tối ưu hóa hoạt họa trang web đạt tốc độ render 16.67 ms mỗi khung hình](https://koolcodez.com/blog/inside-the-frame/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101002.webp)

Màn hình máy tính thông thường có tần số quét 60Hz. Để hoạt họa hiển thị mượt mà nhất, thời gian render cho mỗi khung hình (frame) không nên vượt quá 16.67 ms. Bài viết chia sẻ một số kiến thức kỹ thuật CSS giúp tăng tốc hiệu năng render hoạt họa của trang web.

3. [Từ cơ chế HTTP Polling chuyển sang MQTT: Hành trình cải tiến kiến trúc hệ thống của chúng tôi trên AWS IoT Core](https://mp.weixin.qq.com/s/3wyrIFf3pQh5EJ0NWbHOjA) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101902.webp)

Bài viết chia sẻ từ một lập trình viên về dự án IoT của công ty, ban đầu sử dụng cơ chế HTTP Polling để cập nhật dữ liệu, sau đó đã chuyển đổi sang giao thức MQTT thông qua dịch vụ AWS IoT Core của Amazon. (Đóng góp từ [@Konata9](https://github.com/ruanyf/weekly/issues/7943))

4. [Tại sao NetNewsWire không được phát triển dưới dạng ứng dụng Web](https://inessential.com/2025/10/04/why-netnewswire-is-not-web-app.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101407.webp)

NetNewsWire là một ứng dụng đọc tin RSS dạng cài đặt trên máy tính (desktop client) rất nổi tiếng. Có nhiều ý kiến đề xuất tác giả nên chuyển đổi ứng dụng này thành phiên bản Web chạy trên trình duyệt. Bài viết là những chia sẻ thẳng thắn và lập luận thuyết phục của tác giả giải thích lý do tại sao ông từ chối phát triển phiên bản Web.

5. [Phép biến đổi Burrows-Wheeler](https://sandbox.bio/concepts/bwt) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101001.webp)

Bài viết giới thiệu về thuật toán biến đổi Burrows-Wheeler (BWT) độc đáo. Thuật toán này xáo trộn thứ tự các ký tự trong chuỗi văn bản sao cho các ký tự giống nhau có xu hướng đứng cạnh nhau.

Điểm kỳ diệu của thuật toán là sau khi xáo trộn, nó vẫn cho phép thực hiện phép biến đổi ngược để khôi phục chuỗi văn bản ban đầu một cách hoàn hảo, làm cho nó trở thành bước đệm lý tưởng cho các thuật toán nén dữ liệu văn bản.

6. [Tấn công tiêm lệnh ẩn qua ảnh chụp màn hình](https://simonwillison.net/2025/Oct/21/unseeable-prompt-injections/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102307.webp)

Ngày càng nhiều hãng phát triển trình duyệt tích hợp trợ lý AI có khả năng đọc hiểu nội dung hiển thị trên màn hình qua hình ảnh chụp màn hình tự động. Gần đây đã xuất hiện kỹ thuật tấn công tiêm lệnh (prompt injection) bằng cách chèn các đoạn văn bản ẩn mà mắt người không nhìn thấy được nhưng mô hình AI vẫn đọc được, từ đó lừa AI thực thi các tác vụ độc hại (như hình trên).

7. [Mã độc sử dụng ký tự Unicode ẩn trên Open VSX Marketplace](https://www.koi.ai/blog/glassworm-first-self-propagating-worm-using-invisible-code-hits-openvsx-marketplace) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102308.webp)

Bài viết giới thiệu một trường hợp mã độc JavaScript vô cùng tinh vi: các đoạn mã độc được viết hoàn toàn bằng các ký tự ẩn (invisible characters) thuộc bảng mã Unicode. Mắt người chỉ thấy các khoảng trắng trống trơn (như hình trên), nhưng các bộ thông dịch lệnh của máy tính vẫn đọc và thực thi các dòng lệnh độc hại đó bình thường.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102309.webp)

## 工具

1. [OpenZL](https://github.com/facebook/openzl)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101008.webp)

Một công cụ nén dữ liệu mã nguồn mở mới do Meta phát hành, được thiết kế chuyên biệt để nén các dữ liệu có cấu trúc (như cơ sở dữ liệu) với tỷ lệ nén cao hơn và tốc độ nhanh hơn. Tham khảo thêm [bài viết giới thiệu](https://linuxiac.com/meta-unveils-openzl-a-new-open-source-data-compression-framework/).

2. [Handy](https://github.com/cjpais/Handy)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092905.webp)

Ứng dụng máy tính đa nền tảng hoàn toàn miễn phí và mã nguồn mở, hỗ trợ chuyển đổi giọng nói thành văn bản.

3. [Feed me up, Scotty!](https://feed-me-up-scotty.vincenttunru.com/)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102111.webp)

Một dịch vụ web tự lưu trữ, người dùng chỉ cần nhập URL trang web và chỉ định bộ chọn CSS (CSS Selector) tương ứng, công cụ sẽ tự động cào dữ liệu và tạo nguồn cấp tin RSS cho trang đó. [Mã nguồn dự án](https://gitlab.com/vincenttunru/feed-me-up-scotty).

4. [Judo](https://judojj.com/releases/)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102306.webp)

Giao diện đồ họa (GUI client) đa nền tảng hỗ trợ quản lý mã nguồn qua Git và Jujutsu (JJ).

5. [htmldocs](https://github.com/htmldocs-js/htmldocs)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101701.webp)

Một thành phần React (React component) hỗ trợ soạn thảo, chỉnh sửa và xem trước tài liệu PDF trực tiếp trên trang web. (Đóng góp từ [@Haopeng138](https://github.com/ruanyf/weekly/issues/7925))

6. [Cent](http://github.com/glink25/Cent)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101703.webp)

Ứng dụng web mã nguồn mở hỗ trợ nhiều người cùng quản lý chi tiêu chung, toàn bộ dữ liệu được lưu trữ an toàn trong kho lưu trữ GitHub cá nhân của bạn. (Đóng góp từ [@glink25](https://github.com/ruanyf/weekly/issues/7929))

7. [Shell360](https://github.com/nashaofu/shell360)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101901.webp)

Ứng dụng kết nối SSH mã nguồn mở hỗ trợ chạy đa nền tảng Windows, macOS, Linux, Android và iOS. (Đóng góp từ [@nashaofu](https://github.com/ruanyf/weekly/issues/7942))

8. [015](https://github.com/keven1024/015)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102003.webp)

Nền tảng chia sẻ tệp tin tạm thời tự lưu trữ (self-hosted). (Đóng góp từ [@keven1024](https://github.com/ruanyf/weekly/issues/7952))

9. [MHtool](https://github.com/sudo1123/MHtool)

Bộ công cụ toán học viết bằng Python chạy trên dòng lệnh, tích hợp các tính năng tính toán toán học, xử lý dữ liệu và vẽ biểu đồ trực quan. (Đóng góp từ [@sudo1123](https://github.com/ruanyf/weekly/issues/7965))

10. [TextGO](https://github.com/C5H12O5/TextGO)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102204.webp)

Ứng dụng máy tính đa nền tảng cho phép người dùng gán các phím tắt chung để thực thi nhanh các tác vụ xử lý văn bản khác nhau dựa trên nội dung đang được bôi đen lựa chọn. (Đóng góp từ [@C5H12O5](https://github.com/ruanyf/weekly/issues/7970))

## AI 相关

1. [AICrop](https://aicrop.app/#upload)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101702.webp)

Dịch vụ web miễn phí sử dụng mô hình AI hỗ trợ cắt cúp hình ảnh đạt chuẩn hiển thị trên nhiều mạng xã hội khác nhau như Instagram, X/Twitter, TikTok. (Đóng góp từ [@indielucas](https://github.com/ruanyf/weekly/issues/7927))

2. [Trình tạo ảnh AI miễn phí](https://freeaiimage.net/zh/)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102203.webp)

Trang web chuyển đổi văn bản thành hình ảnh (text-to-image) hoàn toàn miễn phí và không cần đăng ký tài khoản. Theo chia sẻ, tác giả đã tự thiết lập dịch vụ này trên hệ thống máy chủ cá nhân trang bị card đồ họa RTX 4090 và chạy mô hình Qwen. (Đóng góp từ [@rustflare](https://github.com/ruanyf/weekly/issues/7968))

3. [XCodeReviewer](https://github.com/lintsinghua/XCodeReviewer)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102302.webp)

Nền tảng kiểm tra và đánh giá chất lượng mã nguồn tự động vận hành bằng các mô hình ngôn ngữ lớn (LLM). (Đóng góp từ [@lintsinghua](https://github.com/ruanyf/weekly/issues/7975))

4. [SLOCCount](https://tools.simonwillison.net/sloccount)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102303.webp)

Trang web thống kê số lượng dòng mã (SLOC) do lập trình viên nổi tiếng Simon Willison phát triển với sự hỗ trợ của AI, giúp phân tích quy mô mã nguồn dự án để ước tính thời gian phát triển cần thiết. Tham khảo thêm [bài viết giới thiệu](https://simonwillison.net/2025/Oct/22/sloccount-in-webassembly/).

5. [Podcast Generator](https://github.com/justlovemaki/Podcast-Generator)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102113.webp)

Công cụ mã nguồn mở giúp chuyển đổi nội dung văn bản thành tệp âm thanh podcast, yêu cầu người dùng cấu hình khóa API OpenAI của riêng mình. (Đóng góp từ [@justlovemaki](https://github.com/ruanyf/weekly/issues/7967))

6. [MuseBot](https://github.com/yincongcyincong/MuseBot/blob/main/README_ZH.md)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102205.webp)

Robot trò chuyện thông minh tích hợp trên các phần mềm giao tiếp trực tuyến, hỗ trợ trả lời tự động bằng nhiều dòng mô hình lớn khác nhau, tương thích tốt với Telegram, Feishu, DingTalk và WeChat. (Đóng góp từ [@yincongcyincong](https://github.com/ruanyf/weekly/issues/7972))

## 资源

1. [EndlessWiki](https://www.endlesswiki.com)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092704.webp)

Trang bách khoa toàn thư đầu tiên trên thế giới được vận hành và sinh nội dung hoàn toàn bằng trí tuệ nhân tạo (AI), các bài viết sẽ được AI tự động tạo lập thời gian thực dựa trên nội dung tìm kiếm của người dùng.

2. [ISBN Visualization](https://phiresky.github.io/isbn-visualization/)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102101.webp)

Trang web trực quan hóa mã số sách tiêu chuẩn quốc tế (ISBN) của toàn bộ các đầu sách trên thế giới thành một thư viện sách trực quan. Khi tìm kiếm một cuốn sách, hệ thống sẽ hiển thị vị trí của cuốn sách đó trên kệ sách. [Mã nguồn dự án](https://github.com/phiresky/isbn-visualization/). (Đóng góp từ [@kohunglee](https://github.com/ruanyf/weekly/issues/7957))

3. [Clone Wars](https://github.com/GorvGoyl/Clone-Wars)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101605.webp)

Kho lưu trữ tổng hợp các dự án mã nguồn mở tái dựng (clone) giao diện và tính năng của nhiều trang web nổi tiếng (như Airbnb, Amazon, Instagram, Netflix, TikTok, v.v.), hiện số lượng dự án được sưu tầm đã vượt quá mốc 100 trang web.

## 图片

1. [Trạm quan sát Neutrino ngầm Giang Môn](https://www.cnrs.fr/en/press/juno-giant-detector-unravel-mysteries-neutrinos)

Vào tháng 8 năm 2025, Trạm quan sát hạt Neutrino ngầm Giang Môn (JUNO) tại Quảng Đông đã chính thức đi vào hoạt động.

Trạm được xây dựng tại vị trí trung điểm giữa hai nhà máy điện hạt nhân Dương Giang và Đài Sơn để tiếp nhận và đo lường lượng neutrino sinh ra từ quá trình vận hành của các nhà máy điện hạt nhân này.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025100910.webp)

Thiết bị cốt lõi của trạm là một bộ phát hiện hình quả cầu trong suốt khổng lồ có đường kính lên tới 35,4 mét, được đặt sâu dưới lòng đất 700 mét để dò tìm các hạt neutrino siêu nhỏ.

Bên trong quả cầu trong suốt chứa đầy 20.000 tấn chất nhấp nháy lỏng (liquid scintillator) cực kỳ nhạy, mọi tương tác giữa hạt neutrino và chất lỏng này đều sẽ tạo ra những tia chớp sáng siêu nhỏ.

Xung quanh quả cầu được lắp đặt khoảng 43.212 đầu dò quang học (PMT), liên tục giám sát và sẵn sàng ghi nhận bất kỳ tia chớp sáng nào phát sinh.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025100911.webp)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025100912.webp)

Dựa trên việc đo lường các tia chớp sáng này, các nhà khoa học mới có thể xác định chính xác đặc tính của hạt neutrino.

Toàn bộ hệ thống được đặt ngập trong một bể nước siêu sạch đường kính 44 mét, phía trên đỉnh bể được bố trí một thiết bị phát hiện lớn khác gọi là Top Tracker (hình dưới) nhằm xác định các hạt tia vũ trụ lọt vào, tránh gây nhiễu và sai lệch kết quả đo lường hạt neutrino từ nhà máy điện hạt nhân.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025100913.webp)

2. [Cầu Choluteca](https://zhuanlan.zhihu.com/p/346564115)

Từ năm 1996 đến năm 1998, một công ty Nhật Bản đã thi công và bàn giao cây cầu Choluteca dài nhất tại quốc gia Trung Mỹ Honduras, với tổng chiều dài đạt 484 mét.

Ngay sau khi hoàn thành, khu vực này đã phải hứng chịu một siêu bão kỷ lục. Bản thân thân cầu chính đứng vững và không bị hư hại, tuy nhiên toàn bộ phần đường dẫn hai đầu cầu đều bị lũ cuốn trôi hoàn toàn (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102311.webp)

Khi chính phủ Honduras còn chưa kịp lên kế hoạch sửa chữa phần đường dẫn, điều tồi tệ hơn đã xảy ra: dòng chảy của sông Choluteca do ảnh hưởng của lũ quét lớn đã chuyển hướng hoàn toàn sang một lối đi khác.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025102312.webp)

Bức ảnh trên mô tả thực trạng của cầu Choluteca hiện tại, chỉ còn là một dải cầu chính cô độc đứng trơ trọi bên cạnh dòng sông đã đổi dòng.

## 文摘

1. [Làm thế nào để phát triển dự án mã nguồn mở bền vững?](https://byroot.github.io/opensource/ruby/2025/10/09/dear-rubyists.html)

Một chủ đề cũ nhưng luôn mang tính thời sự: làm thế nào để duy trì sự phát triển khỏe mạnh và lâu dài của một dự án mã nguồn mở?

Nhiều người sẽ lập tức trả lời rằng: cần có các doanh nghiệp chi tiền tài trợ để trả lương cho thời gian làm việc của các lập trình viên.

Điều đó quả thực không sai, tuy nhiên **phương án hỗ trợ tối ưu hơn không phải là bơm tiền tài trợ, mà là cử nhân sự tham gia**. Ví dụ điển hình nhất chính là nhân phát triển Linux Kernel, hầu như mọi đóng góp mã nguồn lớn đều đến từ đội ngũ kỹ sư thuộc các tập đoàn được hưởng lợi từ việc vận hành hệ thống Linux.

Nếu các doanh nghiệp đó chỉ quyên góp tiền mặt cho dự án và để đội ngũ nòng cốt tự xoay xở viết mã, Linux Kernel chắc chắn không thể phát triển mạnh mẽ và nhanh chóng như ngày nay.

Một ví dụ tuyệt vời khác là ngôn ngữ lập trình Ruby. Vào năm 2019, một kỹ sư của công ty Shopify đã có cơ hội gặp mặt cha đẻ của ngôn ngữ Ruby là Matz.

Khi được hỏi ông đang cần hỗ trợ điều gì nhất, Matz đã trả lời: "Tôi đang thiếu nhân lực."

Sau khi người kỹ sư quay lại bàn bạc với công ty, Shopify đã quyết định cử hẳn một đội ngũ phát triển Ruby tham gia đóng góp mã nguồn trực tiếp vào ngôn ngữ Ruby, kết quả là mang lại rất nhiều đóng góp chất lượng và bổ sung thêm hơn chục nhà phát triển nòng cốt (core committers) cho ngôn ngữ này.

Nếu ngày hôm đó Matz trả lời "Tôi đang thiếu tiền", và Shopify quyên góp hàng trăm nghìn hay hàng triệu USD, điều đó chưa chắc đã mang lại lợi ích tốt nhất cho Ruby.

Đầu tiên, ai dám đảm bảo định hướng phát triển và các quyết định kỹ thuật của ngôn ngữ Ruby sau này sẽ không bị chi phối bởi lợi ích của Shopify? Một tính năng mới được chấp nhận là vì nó thực sự ưu việt hay vì nó đến từ nhà tài trợ lớn nhất? Liệu ban quản trị Ruby có đủ dũng khí từ chối các đề xuất từ Shopify? Thị hiếu của nhà tài trợ lớn hoàn toàn có thể bóp méo hướng đi của dự án.

Thứ hai, tiền bạc là thứ một khi đã có, bạn dễ sinh ra tâm lý ỷ lại và phụ thuộc. Nếu sau này nhà tài trợ rút vốn, bạn sẽ buộc phải cắt giảm nhân sự, dừng các dự án đang triển khai, v.v. Vì vậy, các tổ chức hay cá nhân nhận tài trợ thường có xu hướng hành xử theo mong muốn của nhà tài trợ để giữ vững dòng tiền đổ về.

Tôi không có ý nói rằng các dự án mã nguồn mở nên từ chối mọi khoản quyên góp, mà là các khoản tài trợ tiền mặt lớn luôn đi kèm với những tác dụng phụ nhất định.

Lần tới, nếu bạn có ý định hỗ trợ một dự án mã nguồn mở, bên cạnh việc gửi tiền quyên góp, hãy cân nhắc đóng góp trực tiếp công sức và thời gian phát triển để san sẻ gánh nặng công việc cùng các nhà sáng lập.

## 言论

1.

Chúng ta phải dần quen với một thế hệ học sinh được đào tạo bởi AI: màn hình của các em ngập tràn chữ nghĩa, nhưng đầu óc lại trống rỗng không có lấy một tư duy.

-- [《Rủi ro từ "chế độ học tập" của OpenAI》](https://resobscura.substack.com/p/openais-new-study-mode-and-the-risks)

2.

Quyết định sáng suốt nhất không phải là chạy theo các trào lưu thời thượng, mà là trồng một cái cây và để cho thời gian làm việc của nó. Cây cối không mang lại quả ngọt vào ngày mai, chúng cần 10 năm để sinh hoa trái. Chúng âm thầm lớn lên và làm đẹp cho mọi thứ xung quanh: từ bóng mát, giá trị kinh tế, tính thẩm mỹ cho đến tuổi thọ.

-- [《Lãi kép của thiết kế》](https://designobserver.com/the-compound-interest-of-design-what-not-to-build/)

3.

OpenAI đã giới thiệu công cụ tìm kiếm Atlas của riêng mình, nhưng thực chất nó là một "trình duyệt ngược", tìm mọi cách hạn chế tối đa việc người dùng truy cập trực tiếp vào các trang web trên internet. Ví dụ khi tìm kiếm từ khóa "Taylor Swift", nó sẽ giải thích chi tiết cô ấy là ai nhưng tuyệt nhiên không trả về bất kỳ đường dẫn liên kết nào dẫn tới trang web cá nhân của cô.

-- [《Atlas của ChatGPT: Trình duyệt ngược lại thế giới Web》](https://www.anildash.com/2025/10/22/atlas-anti-web-browser/)

4.

Một kỹ sư không chỉ cần rèn luyện các kỹ năng chuyên môn kỹ thuật, mà còn phải trau dồi các kỹ năng mềm, cụ thể là kỹ năng giao tiếp và ứng xử giữa người với người.

Nếu không thấu hiểu tính phức tạp của xã hội loài người, bạn sẽ không thể hiểu được cách thức vận hành và hợp tác trong một công ty hay đội ngũ, điều này cuối cùng sẽ cản trở hiệu suất làm việc và khả năng tạo tầm ảnh hưởng của chính bạn.

-- [《Những kỹ năng mềm bị đánh giá thấp》](https://utopianengineeringsociety.substack.com/p/new-series-underrated-soft-skills)

## 往年回顾

[Cuộc so tài slogan của các công ty công nghệ](https://www.ruanyifeng.com/blog/2024/11/weekly-issue-323.html) (#323)

[Ba bài phát biểu mới nhất của Nhậm Chính Phi](https://www.ruanyifeng.com/blog/2023/10/weekly-issue-273.html) (#273)

[Lập trình viên có cần lo lắng về làn sóng sa thải?](https://www.ruanyifeng.com/blog/2022/09/weekly-issue-223.html) (#223)

[Thiết kế của dòng máy thu thanh Internet](https://www.ruanyifeng.com/blog/2021/08/weekly-issue-173.html) (#173)

(Hết)
