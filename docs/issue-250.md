# Bản tin chia sẻ công nghệ (Số 250): Rủi ro lớn nhất của công nghệ mới

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3022) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041207.webp)

Cửa hàng bán lẻ chính thức đầu tiên của Apple tại Ấn Độ đã khai trương vào ngày 18 tháng 4 tại thành phố Mumbai. Các báo cáo phân tích cho thấy Apple đang đặt kỳ vọng rất lớn vào việc biến Ấn Độ thành thị trường quốc tế lớn thứ hai của hãng, đồng thời lên kế hoạch chuyển dịch sản xuất để quốc gia này đảm nhận việc lắp ráp khoảng 25% lượng iPhone toàn cầu trong tương lai gần. (Nguồn: [IndianExpress](https://indianexpress.com/article/technology/tech-news-technology/apple-mumbai-delhi-stores-india-opening-8549861/))

## 本周话题：新技术的最大风险

Gần đây, tôi vô tình đọc được ba bài viết kỹ thuật khác nhau, nhưng tất cả đều chia sẻ chung một chủ đề: **sự hối hận của các kỹ sư sau một thời gian đưa các công nghệ mới vào dự án thực tế.**

* Bài viết thứ nhất: [《Tại sao chúng tôi quyết định từ bỏ ngôn ngữ Elm tại Culture Amp》](https://kevinyank.com/posts/on-endings-why-how-we-retired-elm-at-culture-amp/)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041003.webp)

* Bài viết thứ hai: [《GraphQL: Chặng đường từ sự hào hứng ban đầu đến nỗi thất vọng thực tế》](https://betterprogramming.pub/graphql-from-excitement-to-deception-f81f7c95b7cf)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041004.webp)

* Bài viết thứ ba: [《Tại sao tôi hối hận vì đã lựa chọn Ionic để phát triển ứng dụng di động》](https://mhamri.com/why-i-regret-using-ionic-for-app-development-c8b21b88d83a)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041002.webp)

Cả ba giải pháp công nghệ mới nêu trên đều ra đời trong khoảng 10 năm trở lại đây. **Vào thời điểm xuất hiện, chúng đều được quảng bá rộng rãi như những giải pháp đột phá giải quyết triệt để các khó khăn lớn của lập trình viên.** Nhờ tính năng hấp dẫn và độ phủ sóng truyền thông lớn, các kỹ sư trên đã nhanh chóng quyết định đưa chúng vào ứng dụng cho dự án của mình.

Chúng ta hãy cùng nhìn lại những ưu điểm nổi bật được hứa hẹn ban đầu của các công nghệ này:

* **Ngôn ngữ Elm**: Cam kết giúp mã nguồn script chạy trên trình duyệt web hoạt động hoàn hảo và không bao giờ phát sinh lỗi crash (runtime exceptions).
* **GraphQL**: Chỉ cần gửi một yêu cầu truy vấn API duy nhất từ phía client là có thể lấy về toàn bộ cấu trúc dữ liệu phức tạp mà giao diện frontend yêu cầu.
* **Ionic**: Hỗ trợ lập trình viên xây dựng ứng dụng di động chạy đồng thời trên cả Android và iOS bằng cách tận dụng bất kỳ framework JavaScript quen thuộc nào (như Angular, React, Vue).

Đối với một kỹ sư frontend, những tính năng kỹ thuật này thực sự vô cùng hấp dẫn và dễ dàng thuyết phục họ đưa vào sử dụng.

Thế nhưng, khi chính thức đưa các công nghệ này vào vận hành thực tế trong môi trường sản xuất (production) lâu dài, hàng loạt vấn đề ngầm bắt đầu phát sinh. Sau vài năm, các lập trình viên mới nhận ra những hệ lụy giống như chia sẻ trong các bài viết trên:

* **Elm**: Bản cập nhật phiên bản mới nhất đã dừng lại từ năm 2019, khiến ngôn ngữ này ngày càng bị cô lập và khó khăn trong việc tích hợp với hệ sinh thái JavaScript hiện đại đang thay đổi từng ngày.
* **GraphQL**: Hiệu năng tải trang thực tế không được cải thiện rõ rệt, ngược lại còn khiến kiến trúc hệ thống backend trở nên vô cùng phức tạp. Các bài toán kinh điển như phân trang (pagination) hay lưu bộ nhớ đệm (caching) trở thành những bài toán kỹ thuật cực kỳ nan giải.
* **Ionic**: Tài liệu hướng dẫn lập trình thiếu thốn và lộn xộn, cộng đồng nhà phát triển quá nhỏ bé dẫn đến việc thiếu các thư viện sinh thái bổ trợ khi dự án phát triển chuyên sâu.

Đến khi các kỹ sư nhận ra sai lầm và muốn thay đổi cấu trúc công nghệ thì mọi chuyện đã quá muộn. Việc lên xe thì dễ nhưng xuống xe lại cực kỳ gian nan; dự án đã được đầu tư phát triển liên tục trong nhiều năm, việc đập đi xây lại toàn bộ kiến trúc là điều vô cùng tốn kém và khó khả thi.

Bài học xương máu rút ra ở đây là: **Chúng ta cần cực kỳ thận trọng khi quyết định đưa các công nghệ mới vào các dự án dài hạn.** Rủi ro lớn nhất của các công nghệ mới – điều mà các lập trình viên thường vô tình bỏ qua – **chính là việc chúng chưa trải qua đủ thời gian kiểm nghiệm thực tế trên quy mô lớn, khiến các lỗi thiết kế ẩn giấu chưa có cơ hội bộc lộ ra ngoài.**

Một nghiên cứu về chi phí phần mềm doanh nghiệp chỉ ra rằng: chi phí viết mã phát triển ban đầu chỉ chiếm khoảng 20% tổng ngân sách dự án, 80% chi phí còn lại thực chất nằm ở khâu bảo trì, cập nhật và sửa lỗi vận hành dài hạn sau này.

Nhiều giải pháp công nghệ mới quảng cáo giúp tiết kiệm rất nhiều công sức cho 20% khâu phát triển ban đầu, nhưng lại vô tình làm phình to chi phí và độ phức tạp cho 80% khâu bảo trì dài hạn sau này.

Đây chính là lý do tại sao tuyệt đại đa số các tập đoàn lớn hiện nay vẫn ưu tiên lựa chọn Java hoặc các hệ thống công nghệ được coi là cũ kỹ cho các dự án cốt lõi của họ thay vì chạy theo các xu hướng công nghệ thời thượng. Java đã được kiểm chứng tính ổn định qua nhiều thập kỷ hoạt động thực tế, hệ sinh thái hỗ trợ cực kỳ phong phú giúp giảm thiểu rủi ro vận hành dài hạn cho doanh nghiệp xuống mức thấp nhất.

Nếu một lập trình viên muốn thiết kế một hệ thống hoạt động ổn định lâu dài, giúp bản thân không phải đau đầu xử lý các lỗi kỹ thuật kỳ lạ phát sinh mỗi ngày, giải pháp tối ưu là hãy ưu tiên lựa chọn các công nghệ cũ nhưng đáng tin cậy cho các dự án dài hạn của mình.

**Nhược điểm duy nhất của các công nghệ cũ là chúng khá tẻ nhạt**: Toàn bộ các giải pháp và tính năng đều đã được khai phá trọn vẹn, không còn nhiều không gian cho sự sáng tạo hay trải nghiệm mới mẻ. Đây là lý do nhiều lập trình viên (đặc biệt là các lập trình viên trẻ tuổi) thường cảm thấy các công nghệ cũ không giúp họ thể hiện năng lực cá nhân và thiếu tính trải nghiệm thú vị như các công nghệ mới.

Tư duy muốn thử nghiệm cái mới này hoàn toàn không sai, nhưng nó chỉ phù hợp với các dự án ngắn hạn hoặc các sản phẩm thử nghiệm nhanh. Đối với các dự án lớn đòi hỏi vận hành ổn định lâu dài, việc lạm dụng các công nghệ mới chưa được kiểm chứng luôn là một canh bạc vô cùng rủi ro.

## 暑期实习申请

Chương trình tuyển dụng thực tập sinh mùa hè dành cho sinh viên đã chính thức khởi động. Hôm nay tuần báo xin giới thiệu cơ hội thực tập hấp dẫn tại tập đoàn **ByteDance**.

ByteDance đang mở đợt tuyển dụng quy mô lớn với hàng ngàn vị trí thực tập tại hơn 10 thành phố khác nhau, thời gian thực tập tiêu chuẩn kéo dài từ 3 tháng trở lên, cho phép ứng viên nộp hồ sơ đồng thời vào nhiều vị trí phù hợp:

[![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041303.webp)](https://mp.weixin.qq.com/s/7stXftKlm1LdBOw_v6KFUw)

Đây là cơ hội thực tập rất chất lượng cho các bạn sinh viên. Năm nay, ByteDance chính thức triển khai chương trình ByteIntern chuyên biệt, bảo đảm các vị trí thực tập đều đi kèm chỉ tiêu chuyển thẳng thành nhân viên chính thức sau kỳ thực tập với tỷ lệ giữ lại rất cao.

Để giúp các bạn hình dung rõ hơn về công việc thực tế, dưới đây là bài chia sẻ trải nghiệm tự sự của 4 bạn sinh viên đang tham gia thực tập các vị trí kỹ thuật tại tập đoàn. **Các bạn có thể nhấp vào hình ảnh phía dưới, kéo xuống cuối bài viết để truy cập cổng nộp hồ sơ và xem các lưu ý quan trọng khi ứng tuyển:**

[![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041304.webp)](https://mp.weixin.qq.com/s/7stXftKlm1LdBOw_v6KFUw)

Trong các số phát hành tới, tuần báo sẽ tiếp tục cập nhật thêm thông tin tuyển dụng thực tập và việc làm công nghệ chất lượng. Chúc các bạn sinh viên tìm kiếm được công việc thực tập ưng ý!

## 科技动态

1、[Hàn Quốc lên kế hoạch xây dựng vòng quay mặt trời không trục lớn nhất thế giới](https://mymodernmet.com/seoul-ring-hubless-ferris-wheel/)

Chính quyền thành phố Seoul mới đây đã công bố dự án xây dựng một vòng quay mặt trời không trục (hubless Ferris wheel) có quy mô lớn nhất thế giới tại thủ đô:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041105.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041108.webp)

Cấu trúc vòng quay không trục loại bỏ hoàn toàn phần trục quay và hệ thống căm xe truyền thống ở giữa, tạo nên một vòng tròn thép khổng lồ rỗng bên trong. Bản thân vòng tròn lớn này sẽ đứng yên cố định, các cabin chở khách sẽ tự di chuyển dọc theo hệ thống đường ray bám quanh chu vi vòng tròn:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041106.webp)

Theo thiết kế, vòng quay khổng lồ này có đường kính lên tới 180m, trang bị 36 cabin chở khách hiện đại với sức chứa tối đa 25 người trong mỗi cabin cho một lượt tham quan.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041107.webp)

2、[Bộ ảnh chân dung tập thể hoàn hảo được dựng hoàn toàn bằng AI](https://medium.com/@socialcreature/ai-and-the-american-smile-76d23a0fbfaf)

Một nghệ sĩ người Mỹ đã ứng dụng công nghệ mô phỏng hình ảnh AI để tạo nên bộ ảnh chân dung tập thể của nhiều nhóm người từ các thời kỳ lịch sử và nền văn hóa khác nhau trên thế giới:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041109.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041110.webp)

Các nhân vật giả lập trong ảnh đều hướng về ống kính với những nụ cười rạng rỡ và tự nhiên như thật:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041111.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041112.webp)

Dù các nhân vật này hoàn toàn không tồn tại ngoài đời thực, thực nghiệm này cho thấy một ứng dụng thực tiễn rất cao của AI: hỗ trợ chỉnh sửa ảnh tập thể. Chúng ta hoàn toàn có thể nạp các bức ảnh chụp tập thể của gia đình hay công ty vào AI để hệ thống tự động chỉnh sửa biểu cảm nụ cười của từng thành viên sao cho sống động và đẹp nhất.

3、[Trung Quốc thử nghiệm thành công trạm phát điện mặt trời nổi trên biển](https://sz.oeeee.com/html/202304/06/1356839.html)

Hệ thống giàn phát điện năng lượng mặt trời dạng bán chìm nổi trên biển đầu tiên của Trung Quốc đã chính thức được bàn giao đưa vào vận hành tại vùng biển Yên Đài:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040620.webp)

Cấu trúc giàn phát điện nổi này bao gồm 4 mảng pin quang điện khổng lồ ghép lại với nhau. Diện tích mỗi mảng pin tương đương kích thước một sân bóng rổ tiêu chuẩn, nâng tổng diện tích bề mặt tiếp nhận ánh sáng lên tới 1.900 mét vuông với công suất phát điện cực đại đạt 400 kW.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040621.webp)

Hệ thống được thiết kế neo nổi vững vàng trên mặt nước để hấp thụ ánh nắng mặt trời. Trong bối cảnh quỹ đất trống trên đất liền thích hợp để lắp đặt các tấm pin mặt trời ngày càng thu hẹp, mô hình phát điện quang điện nổi trên mặt biển này hứa hẹn sẽ trở thành xu hướng phát triển mạnh mẽ trong tương lai.

4、[Nghiên cứu ứng dụng giống lúa trồng một lần thu hoạch nhiều năm](https://www.npr.org/2023/03/23/1165680024/perennial-rice-plant-once-harvest-again-and-again)

Lúa nước là cây lương thực cốt lõi nuôi sống hơn một nửa dân số toàn cầu.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040801.webp)

Tuy nhiên, quy trình canh tác truyền thống có một nhược điểm lớn là yêu cầu người nông dân phải tiến hành gieo mạ và cấy lúa lại từ đầu sau mỗi mùa thu hoạch. Việc cày bừa đất và cấy lúa lặp đi lặp lại hàng năm gây tốn rất nhiều công sức lao động và làm suy kiệt chất dinh dưỡng của đất trồng.

Trong nhiều năm qua, các nhà khoa học trên thế giới đã tập trung nghiên cứu giống "lúa lâu năm" (perennial rice) – loại lúa chỉ cần gieo cấy một lần duy nhất nhưng cây lúa có thể tiếp tục sinh trưởng tự động phục hồi đâm chồi kết hạt mới sau mỗi vụ thu hoạch trong nhiều năm tiếp theo.

Báo chí quốc tế đưa tin các nhà khoa học Mỹ đã thực hiện lai tạo giống lúa thơm Thái Lan với một giống lúa hoang dã có sức sống cực kỳ bền bỉ tại châu Phi và đã chọn lọc ra được 3 giống lúa lâu năm tiềm năng. Hiện tại các giống lúa thử nghiệm này đã bước sang năm sinh trưởng thứ 4 liên tiếp và cho sản lượng hạt rất khả quan, mở ra triển vọng thay đổi hoàn toàn phương thức canh tác lúa nước truyền thống.

## Bài viết

1\. [Cẩm nang hướng dẫn chi tiết phương pháp viết Prompt cho công cụ vẽ tranh AI](https://boostpixels.com/guide)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040903.webp)

Làm thế nào để viết các câu lệnh Prompt mô tả hình ảnh chính xác giúp các mô hình Generative AI vẽ tranh đúng ý muốn? Bài viết hướng dẫn chi tiết từng bước cách xây dựng cấu trúc Prompt tối ưu từ cơ bản đến nâng cao. Tuy viết riêng cho công cụ vẽ tranh BoostPixels, bài viết chứa đựng nhiều nguyên lý thiết lập Prompt rất đáng để tham khảo. Bạn đọc có thể xem thêm phiên bản [tóm tắt nhanh](https://boostpixels.com/short-guide).

2\. [Hướng dẫn nhanh cách ứng dụng mô hình ngôn ngữ lớn LLM vào công việc](https://www.ruxu.dev/articles/ai/maximizing-the-potential-of-llms/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041102.webp)

Bài viết chia sẻ các ví dụ thực hành trực quan hướng dẫn lập trình viên tận dụng sức mạnh của các mô hình LLM để nhanh chóng tự động hóa các tác vụ lặp đi lặp lại hàng ngày như tóm tắt tài liệu, phân loại văn bản hay viết code mẫu.

3\. [Giải pháp chèn hiển thị các trang web bên ngoài an toàn bằng iframe](https://making.close.com/posts/rendering-untrusted-html-email-safely)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032806.webp)

Khi xây dựng trang web cho phép người dùng chèn hiển thị nội dung của các trang web bên ngoài không rõ nguồn gốc (untrusted HTML) thông qua thẻ `<iframe>`, nguy cơ bị tấn công bảo mật XSS là rất lớn. Bài viết chia sẻ các thiết lập thuộc tính bảo mật Sandbox của thẻ iframe để bảo đảm an toàn cho hệ thống.

4\. [Kỷ nguyên thiết kế HTML Email hiện đại không còn phụ thuộc vào thẻ table](https://fullystacked.net/posts/modern-html-email/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040904.webp)

Trước đây khi viết mã HTML cho email, lập trình viên buộc phải lạm dụng thẻ `<table>` để bảo đảm bố cục hiển thị đồng bộ trên ứng dụng Microsoft Outlook (vốn sử dụng nhân MS Word cũ để kết xuất HTML). Bài viết chỉ ra rằng với việc các phiên bản Outlook mới đã chuyển sang sử dụng nhân Microsoft Edge hiện đại, lập trình viên hoàn toàn có thể sử dụng Flexbox và Grid CSS thông thường để thiết kế email.

5\. [Bài viết phân tích so sánh định dạng tài liệu Asciidoc và Markdown](https://pdx.su/blog/2023-02-05-asciidoc-and-markdown/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020808.webp)

Asciidoc là định dạng tài liệu viết bằng văn bản thô (plain text) được thiết kế chuyên dụng cho việc viết sách kỹ thuật và tài liệu lập trình quy mô lớn. Tác giả thực hiện so sánh chi tiết các ưu nhược điểm của Asciidoc so với Markdown trong việc quản lý cấu trúc chương mục và xuất bản tài liệu.

6\. [Khảo sát khả năng truyền tham số trong dòng khai báo Shebang của lệnh Bash](https://linuskarlsson.se/blog/shebang-shenanigans/)（Tiếng Anh）

Dòng đầu tiên của các tệp tin script Linux thường bắt đầu bằng ký tự `#!` (gọi là Shebang) để chỉ định trình biên dịch chạy script. Bài viết phân tích sâu cơ chế hoạt động của nhân hệ điều hành Linux khi xử lý dòng Shebang này và hướng dẫn cách truyền thêm tham số cấu hình một cách an toàn.

7\. [Nhìn lại chặng đường tiến hóa kiến trúc hạ tầng hệ thống của Twitter](https://iosifache.me/twitter-architecture-trends)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020810.webp)

Bài viết tổng hợp và sơ đồ hóa quá trình thay đổi kiến trúc hệ thống backend của mạng xã hội Twitter qua các năm, từ mô hình Ruby on Rails nguyên khối ban đầu chuyển dịch sang kiến trúc microservices viết bằng Scala và Java để chịu tải hàng tỷ lượt truy cập.

8\. [Khám phá 18 câu hỏi vật lý học cơ bản hiện chưa có lời giải đáp](https://www.livescience.com/34052-unsolved-mysteries-physics.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032807.webp)

Bài viết khoa học phổ thông giới thiệu tóm tắt về 18 bài toán vật lý lý thuyết nền tảng mà giới khoa học hiện đại vẫn chưa thể đưa ra câu trả lời chắc chắn, bao gồm bản chất của vật chất tối, năng lượng tối và nguồn gốc của vũ trụ.

## Công cụ

1、[Alfred Home Security: Ứng dụng biến điện thoại cũ thành camera giám sát](https://alfred.camera/)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011602.webp)

Ứng dụng di động hữu ích giúp người dùng tận dụng các điện thoại cũ không dùng đến làm camera giám sát an ninh gia đình có hỗ trợ phát hiện chuyển động (dịch vụ trả phí). Một số phần mềm tương tự hoàn toàn miễn phí bạn có thể tham khảo là [Live-Reporter](https://apps.apple.com/us/app/live-reporter-live-camera/id996017825) hoặc dự án mã nguồn mở [Haven](https://guardianproject.github.io/haven/).

2、[OpenPromptStudio: Công cụ Web quản lý và tối ưu hóa Prompt vẽ tranh AI](https://moonvy.com/apps/ops/)

Công cụ web nguồn mở hỗ trợ quản lý trực quan các câu lệnh Prompt cho các mô hình AI vẽ tranh như Midjourney, hỗ trợ tự động dịch mô tả từ tiếng Trung sang tiếng Anh và phân loại prompt theo các thẻ phong cách để lập trình viên dễ dàng lựa chọn. (Đóng góp của [@xcuyao](https://github.com/ruanyf/weekly/issues/3044))

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041202.webp)

3、[Anonymous Chat Room: Ứng dụng phòng chat ẩn danh đa năng nguồn mở](https://github.com/velor2012/anonymous-chat-room)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041203.webp)

Mã nguồn mở xây dựng ứng dụng phòng trò chuyện trực tuyến ẩn danh, hỗ trợ người dùng trao đổi tin nhắn văn bản, thực hiện cuộc gọi thoại trực tiếp trên trình duyệt và tích hợp tính năng quay video màn hình cuộc trò chuyện. (Đóng góp của [@velor2012](https://github.com/ruanyf/weekly/issues/3045))

4、[SQLkiller: Công cụ AI hỗ trợ sinh tự động câu lệnh truy vấn SQL](https://www.sqlkiller.com/)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041205.webp)

Ứng dụng web tích hợp mô hình AI giúp lập trình viên viết nhanh câu lệnh SQL: người dùng chỉ cần dán cấu trúc bảng cơ sở dữ liệu (schema) lên hệ thống và mô tả yêu cầu truy vấn bằng ngôn ngữ tự nhiên, AI sẽ tự động sinh câu lệnh SQL tương ứng. (Đóng góp của [@Benxzz](https://github.com/ruanyf/weekly/issues/3047))

5、[PyGWalker: Thư viện chuyển dữ liệu Pandas sang giao diện tương tác](https://github.com/Kanaries/pygwalker)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041206.webp)

Thư viện Python mạnh mẽ hỗ trợ chuyển đổi nhanh các cấu trúc bảng dữ liệu Pandas DataFrame thành một giao diện đồ họa phân tích dữ liệu trực quan kéo thả tương tự như phần mềm Tableau để phân tích nhanh số liệu. (Đóng góp của [@jojocys](https://github.com/ruanyf/weekly/issues/3050))

6、[Domain Admin: Nền tảng nguồn mở theo dõi thời hạn chứng chỉ SSL](https://github.com/mouday/domain-admin)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041204.webp)

Hệ thống quản trị nguồn mở hỗ trợ giám sát thời hạn hoạt động của hàng loạt tên miền và chứng chỉ bảo mật SSL/TLS, tự động gửi thông báo nhắc nhở gia hạn qua email hoặc webhook khi chứng chỉ sắp hết hạn. (Đóng góp của [@mouday](https://github.com/ruanyf/weekly/issues/3038))

7、[x-crawl: Thư viện cào dữ liệu web mạnh mẽ chạy trên Node.js](https://github.com/coder-hxl/x-crawl)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041201.webp)

Thư viện viết crawler cào dữ liệu linh hoạt trên Node.js, tích hợp sẵn nhân trình duyệt Puppeteer để xử lý các trang SPA tải dữ liệu bằng JavaScript và hỗ trợ cơ chế tự động xoay vòng proxy bypass Cloudflare. (Đóng góp của [@coder-hxl](https://github.com/ruanyf/weekly/issues/3040))

8、[unblob: Tiện ích CLI giải nén và phân tích cấu trúc file container](https://unblob.org/)

Công cụ dòng lệnh hiệu năng cao giúp nhà phát triển nhanh chóng giải nén, trích xuất dữ liệu và phân tích cấu trúc nội bộ của hơn 30 định dạng file nén và tệp container hệ thống khác nhau (như firmware, file ảnh đĩa).

9、[YakGPT: Giao diện web UI tối giản hỗ trợ nhập giọng nói cho ChatGPT](https://yakgpt.vercel.app/)

Giao diện frontend thay thế cho ChatGPT được tối ưu hóa tốc độ tải trang, bổ sung tính năng độc đáo cho phép người dùng trực tiếp sử dụng micro điện thoại/máy tính để nhập câu hỏi bằng giọng nói thay vì gõ phím.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040109.webp)

10、[CLI Co-Pilot: Trợ lý sinh lệnh terminal bằng trí tuệ nhân tạo](https://github.com/AntonOsika/CLI-Co-Pilot)

Công cụ CLI nhỏ gọn: người dùng chỉ cần mô tả thao tác muốn thực hiện trên máy tính bằng tiếng Anh, công cụ sẽ gọi API OpenAI để sinh câu lệnh shell tương ứng và hỏi xác nhận thực thi trực tiếp trên terminal. Một công cụ tương tự là [AI Shell](https://github.com/BuilderIO/ai-shell).

11、[Cheetah: Công cụ hỗ trợ trả lời phỏng vấn từ xa bằng AI](https://github.com/leetcode-mafia/cheetah)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040614.webp)

Dự án mã nguồn mở thiết kế tiện ích hỗ trợ phỏng vấn tuyển dụng từ xa: công cụ sẽ tự động thu âm câu hỏi của người phỏng vấn qua cuộc gọi, dùng mô hình Whisper chuyển thành chữ gửi tới OpenAI và hiển thị nhanh câu trả lời gợi ý lên màn hình của ứng viên.

## 资源

1、[Java Programming Tutorial: Giáo trình thực hành lập trình Java chất lượng](https://www3.ntu.edu.sg/home/ehchua/programming/index.html)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011504.webp)

Trang web lưu trữ toàn bộ tài liệu giảng dạy và bài tập thực hành lập trình ngôn ngữ Java (viết bằng tiếng Anh) của một giảng viên thuộc Đại học Công nghệ Nanyang (Singapore), rất thích hợp làm tài liệu tự học.

2、[offsec.tools: Thư viện tổng hợp công cụ và phần mềm bảo mật thông tin](https://offsec.tools/)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012101.webp)

Trang web chuyên cập nhật và phân loại thông tin của hơn 600 công cụ, phần mềm mã nguồn mở chuyên dụng phục vụ công tác kiểm thử xâm nhập (pentesting) và bảo mật an toàn thông tin.

3、[Wonders of Street View: Kho ảnh chụp những khoảnh khắc kỳ thú trên Google Maps](https://neal.fun/wonders-of-street-view/?v=b2wMrU)

Trang web thú vị tự động lựa chọn và hiển thị ngẫu nhiên các bức ảnh chụp ghi lại những tình huống hài hước hoặc kỳ lạ vô tình lọt vào ống kính của xe chụp ảnh bản đồ đường phố Google Street View.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012501.jpg)

4、[nosignup.tools: Danh tuyển chọn các ứng dụng web dùng ngay không cần đăng ký](https://www.nosignup.tools/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081705.webp)

Thư mục tổng hợp các dịch vụ trực tuyến hữu ích (như chuyển đổi định dạng ảnh, chỉnh sửa văn bản, vẽ sơ đồ) hỗ trợ người dùng truy cập và sử dụng được ngay lập tức mà không yêu cầu bước đăng ký tài khoản phiền phức.

5、[DNS0.EU: Dịch vụ DNS công cộng bảo mật dành riêng cho cư dân châu Âu](https://www.dns0.eu/)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020805.webp)

Trang chủ giới thiệu và hướng dẫn cấu hình dịch vụ phân giải tên miền DNS công cộng mới của Liên minh châu Âu, tập trung vào việc tăng tốc độ truy cập internet và bảo vệ người dùng trước các tên miền độc hại.

## 图片

1、**So sánh hiệu quả tiết kiệm điện giữa tủ lạnh đứng và tủ đông nằm ngang**

Tủ lạnh thông thường của gia đình được thiết kế dạng cửa mở dọc đứng:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110507.webp)

Tủ đông chuyên dụng thường được thiết kế dạng cửa mở nằm ngang phía trên:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110508.webp)

Thiết kế nào mang lại hiệu năng tiết kiệm năng lượng tốt hơn?

Câu trả lời là các tủ đông nằm ngang. Nguyên lý vật lý cho thấy không khí lạnh có khối lượng riêng lớn hơn nên luôn chìm xuống dưới đáy khoang chứa. Khi bạn mở cửa tủ lạnh đứng thông thường, lượng không khí lạnh sẽ lập tức ùa thoát ra ngoài, buộc block máy phải khởi động lại để làm lạnh không khí mới. Ngược lại khi mở cửa tủ đông nằm ngang từ phía trên, lượng khí lạnh nặng vẫn nằm nguyên bên trong lòng tủ, giúp tiết kiệm lượng điện năng tiêu thụ từ 10 đến 20 lần so với tủ đứng.

2、**Bộ ảnh chân dung giả lập các tỷ phú công nghệ nếu sinh ra ở khu ổ chuột**

Môi trường sinh trưởng ban đầu quyết định rất lớn tới chặng đường thành công sau này của mỗi con người.

Liệu các tỷ phú công nghệ hàng đầu thế giới như Bill Gates hay Elon Musk có thể gặt hái được những thành tựu như hiện tại nếu họ không may mắn được sinh ra trong các gia đình có điều kiện kinh tế tốt?

Một nghệ sĩ người Ấn Độ đã sử dụng công nghệ AI để phác họa lại chân dung của các tỷ phú giàu nhất hành tinh trong bối cảnh giả định họ sinh ra và lớn lên trong các khu ổ chuột nghèo khó:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041208.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041209.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041210.webp)

## ✍️ Bài đọc thêm

### Phương pháp phát triển sản phẩm độc đáo của thương hiệu Nest

Vào năm 2014, tập đoàn Google đã chi ra tới 3,2 tỷ USD để mua lại Nest – một startup nổi tiếng chuyên sản xuất các thiết bị gia dụng thông minh (như máy điều nhiệt, chuông cửa thông minh).

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061607.webp)

Quy trình nghiên cứu và phát triển sản phẩm của Nest có một triết lý rất khác biệt so với số đông các công ty công nghệ: **Họ luôn hoàn thiện bản dự thảo thông cáo báo chí và thiết kế vỏ hộp sản phẩm trước khi tiến hành viết dòng code đầu tiên.**

Nhà sáng lập Tony Fadell chia sẻ về triết lý này:

> “Khi bạn ép bản thân phải viết ra một bản thông cáo báo chí giới thiệu sản phẩm trước, bạn sẽ buộc phải trả lời câu hỏi: Tính năng cụ thể nào của thiết bị này thực sự mang lại giá trị truyền thông và thu hút sự chú ý của người tiêu dùng?”

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041301.webp)

Bởi lẽ thông thường, một người đọc lướt qua một bản tin giới thiệu sản phẩm mới chỉ dành tối đa khoảng 30 giây. Nếu trong 30 giây ngắn ngủi đó sản phẩm không khơi gợi được sự tò mò, họ sẽ lập tức bỏ qua nó. Do đó, bạn bắt buộc phải chắt lọc và trình bày được tính năng độc đáo, giá trị nhất của sản phẩm ngay trong trang viết giới thiệu ban đầu. Điều này tương tự như việc bạn có cơ hội đi chung thang máy với một nhà đầu tư từ tầng 1 lên tầng 14; bạn chỉ có khoảng thời gian rất ngắn ngủi đó để thuyết phục họ, từng câu chữ nói ra đều phải được chắt lọc kỹ lưỡng.

Một khi đã hoàn thiện được một bản thông cáo báo chí hấp dẫn, đội ngũ kỹ sư sẽ hiểu rất rõ đâu là các tính năng cốt lõi cần ưu tiên tập trung nguồn lực để phát triển.

Sau khi hoàn thành thông cáo báo chí, Tony Fadell tiếp tục bắt tay vào khâu thiết kế vỏ hộp sản phẩm trên giấy. Ông chia sẻ:

> “Quy cách đóng gói vỏ hộp sẽ quyết định hình hài của sản phẩm. Những giới hạn vật lý về kích thước và hình dáng của chiếc hộp giấy sẽ buộc bạn phải suy nghĩ xem sản phẩm bên trong cần có cấu trúc và thiết kế tối ưu ra sao để nằm vừa vặn và hiển thị các tính năng bắt mắt nhất.”

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041302.webp)

Trong suốt quy trình thiết kế ngược đó, đội ngũ phát triển liên tục tinh chỉnh và hoàn thiện các ý tưởng của mình, cho đến khi cốt lõi tinh túy nhất của sản phẩm được hiện thực hóa thành một món hàng hoàn thiện bắt mắt nằm sẵn trên kệ để người tiêu dùng có thể cầm lên và thanh toán.

Chỉ sau khi đã xác định rõ ràng tính năng và kiểu dáng thiết kế hộp ngoài, Nest mới chính thức bắt tay vào quy trình lập trình và chế tạo phần cứng sản phẩm thực tế.

## Lịch sử tuần này

- 2022年（第 203 期）：[Giáo dục: Nhìn nhận thực tế giá trị của tấm bằng danh giá tại Anh và chương trình dạy CNTT tại Berkeley](http://www.ruanyifeng.com/blog/2022/04/weekly-issue-203.html)
- 2021年（第 153 期）：[Dịch thuật: Liệu sự phát triển của dịch thuật máy có phải là một sự xúc phạm đối với biên dịch viên](http://www.ruanyifeng.com/blog/2021/04/weekly-issue-153.html)
- 2020年（第 103 期）：[Lý thuyết thông tin: Tìm hiểu về khái niệm chu kỳ bán rã của thông tin trong thế giới số](http://www.ruanyifeng.com/blog/2020/04/weekly-issue-103.html)
- 2019年（第 53 期）：[Xã hội: Trải nghiệm thú vị về phương pháp tổ chức các buổi hẹn hò ghép đôi dựa theo dữ liệu DNA](http://www.ruanyifeng.com/blog/2019/04/weekly-issue-53.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
