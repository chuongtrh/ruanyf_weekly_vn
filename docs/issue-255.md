# Bản tin chia sẻ công nghệ (Số 255): Thái độ đúng đắn đối với AI

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3091) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051818.webp)

Tuyến tàu điện trên cao không người lái (Sky Rail) tại Thung lũng Quang học Vũ Hán đã chính thức đi vào chạy thử nghiệm từ ngày 26 tháng 4 với tổng chiều dài toàn tuyến là 10,5 km. Đây là hệ thống tàu điện trên treo thương mại đầu tiên được triển khai tại nước này. Mặc dù cấu trúc kỹ thuật bảo đảm an toàn tuyệt đối, cảm giác ngồi trên toa tàu treo lơ lửng giữa không trung vẫn mang lại sự hồi hộp cho hành khách. (Nguồn: [Tân Hoa Xã](http://www.news.cn/local/2023-05/11/c_1129607613.htm))

## 本周话题：对待 AI 的正确态度

Thời gian gần đây, tôi nhận được khá nhiều câu hỏi từ độc giả về quan điểm đối với chủ đề đang gây xôn xao dư luận: “[Front-end đã chết](https://www.baidu.com/s?wd=%E5%89%8D%E7%AB%AF%E5%B7%B2%E6%AD%BB)”.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051607.webp)

Phản ứng đầu tiên của tôi là mảng Front-end hoàn toàn không có dấu hiệu lụi tàn, tuyệt đại đa số các doanh nghiệp công nghệ vẫn đang đăng tuyển các vị trí kỹ sư lập trình Front-end mỗi ngày.

Tìm hiểu kỹ hơn, tôi nhận thấy mối lo ngại thực sự của cộng đồng là sự sụt giảm sức hút của ngành: **tốc độ phát triển công nghệ Front-end đang chững lại, thiếu vắng các xu hướng công nghệ mới mang tính đột phá, vai trò chiến lược của giao diện trong doanh nghiệp bị xem nhẹ và cơ hội việc làm cho người mới sụt giảm rõ rệt.**

Đáng lo ngại hơn cả là sự xuất hiện của các công cụ AI có khả năng tự động thiết kế và sinh mã nguồn giao diện hoàn chỉnh, dấy lên nỗi sợ hãi liệu lập trình viên Front-end có bị AI thay thế hoàn toàn trong tương lai gần?

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051303.webp)

Góc nhìn của tôi không quá bi quan như vậy. Giai đoạn khó khăn hiện tại chỉ là chu kỳ suy thoái ngắn hạn của nền kinh tế; một khi thị trường phục hồi, nhu cầu nhân lực lập trình Front-end chất lượng cao chắc chắn sẽ tăng trở lại.

Còn về câu hỏi liệu AI có thể "khai tử" mảng lập trình Front-end hay không thì rất khó nói trước, điều đó phụ thuộc hoàn toàn vào tốc độ tiến hóa của công nghệ AI, dù cá nhân tôi chưa tin rằng AI có thể tự động xây dựng được các hệ thống giao diện có cấu trúc logic và tương tác phức tạp.

Hôm nay, tôi muốn thảo luận về câu hỏi: **Lập trình viên cần làm gì để đối phó với một tương lai đầy biến động hiện nay?** Tiến trình phát triển của AI là điều không thể dự đoán và hoàn toàn nằm ngoài tầm kiểm soát của mỗi cá nhân. Khi sự nghiệp và tương lai của lập trình viên trở nên bấp bênh trước làn sóng AI, chúng ta nên hành động như thế nào?

Tôi vô tình đọc được chia sẻ của [một lập trình viên người Ấn Độ](https://github.com/ixaxaar/VardaGPT/blob/master/STORY.md) xoay quanh chủ đề này. Anh đã quyết định tự mình thử nghiệm thực tế để kiểm chứng giới hạn năng lực viết mã hiện tại của AI.

Anh yêu cầu ChatGPT viết một phần mềm ứng dụng theo thiết kế của mình. Kết quả là anh phải mất trọn vẹn ba ngày cuối tuần liên tục điều chỉnh các câu lệnh Prompt và sửa lỗi hệ thống thì phần mềm mới có thể tạm thời chạy được ổn định.

Dưới đây là những nhận định thực tế của anh về năng lực của AI:

> “Đôi khi tôi thực sự kinh ngạc trước khả năng thấu hiểu yêu cầu của ChatGPT, nhưng phần lớn thời gian tôi phải cật lực tìm cách dẫn dắt và định hướng nó đi đúng quỹ đạo thiết kế mong muốn. Đôi khi AI sinh ra những đoạn mã lỗi rất ngớ ngẩn khiến tôi vô cùng nản lòng.
> 
> Nó giống như một sinh viên mới tốt nghiệp nắm giữ toàn bộ kho tàng tri thức lý thuyết của nhân loại nhưng lại thiếu đi năng lực thực tế để tự xâu chuỗi và liên kết các kiến thức đó lại với nhau để giải quyết một bài toán cụ thể nếu không có sự chỉ dẫn sát sao.
> 
> **Có vẻ như công việc của tôi trong năm nay vẫn hoàn toàn an toàn. Nhưng tôi cần học cách làm chủ và sử dụng thành thạo ChatGPT để bảo đảm công việc của tôi vào năm sau cũng sẽ tiếp tục an toàn.**”

Tôi vô cùng tâm đắc với câu kết luận cuối cùng của anh và tin rằng đây chính là tinh thần và thái độ sống mà mỗi lập trình viên chúng ta cần trang bị trong giai đoạn hiện nay.

Tương lai của AI phát triển ra sao là điều không thể biết trước, nhưng có một sự thật hiển nhiên là năng lực lập trình hiện tại của AI chưa thể đe dọa đến vị trí công việc của các kỹ sư lập trình thực thụ.

Vị trí của bạn trong năm nay vẫn được bảo đảm. Nếu bạn chịu khó nỗ lực, công việc của bạn trong năm sau cũng sẽ an toàn, và nhiều khả năng bạn sẽ luôn giữ được vị thế chủ động. Bởi trong quá trình làm việc cùng AI, bạn sẽ ngày càng thành thạo kỹ năng điều phối công cụ này để phục vụ cho các mục tiêu công việc của mình. Nói cách khác, AI đóng vai trò như một bộ nhân tăng cường đáng kể hiệu suất làm việc cá nhân của bạn.

Đó chính là mấu chốt của vấn đề: **Mối quan hệ giữa con người và AI không phải là sự đối đầu triệt tiêu lẫn nhau. AI không cướp đi công việc của bạn, trái lại nó mở ra nhiều cơ hội phát triển sản phẩm mới.**

Một doanh nhân công nghệ người Anh đã đúc kết [5 nhận định cốt lõi về AI](https://adamcohenhillel.substack.com/p/new-layer-of-abstraction-not-the) mà tôi tin rằng đây chính là thái độ tiếp cận đúng đắn nhất đối với trí tuệ nhân tạo:

1. AI sẽ tăng cường mạnh mẽ năng suất làm việc của lập trình viên, cho phép xây dựng các sản phẩm công nghệ đột phá trước đây chưa từng có.
2. AI bản chất là một công cụ tăng năng suất lao động, tương tự như các tầng phát triển trước đây của ngành công nghệ như sự xuất hiện của các ngôn ngữ lập trình bậc cao, dịch vụ điện toán đám mây hay các thư viện mã nguồn mở.
3. Rào cản tiếp cận lập trình viết mã sẽ được hạ thấp, thu hút thêm nhiều nhân sự tham gia vào ngành CNTT và mở rộng quy mô của thị trường phần mềm toàn cầu.
4. Sự bùng nổ của AI sẽ tạo ra động lực tăng trưởng mới cho nền kinh tế số, mang lại nhiều cơ hội phát triển sản phẩm và việc làm mới cho tất cả mọi người.
5. Việc của chúng ta là chủ động tham gia vào tiến trình này bằng cách tích cực học hỏi, liên tục cập nhật bộ kỹ năng và làm chủ các công cụ hỗ trợ thế hệ mới.

## 科技动态

1、[Mỹ thử nghiệm mô hình phân phối tivi màn hình lớn miễn phí tích hợp quảng cáo](https://www.theverge.com/2023/5/15/23721674/telly-free-tv-streaming-ilya-pozin-ads)

Một doanh nghiệp truyền thông tại Mỹ mới đây đã công bố chương trình tặng tivi màn hình lớn 55 inch hoàn toàn miễn phí cho những người dùng đăng ký thông tin trên [Trang chủ của hãng](https://www.freetelly.com/):

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051603.webp)

Điểm mấu chốt của mô hình kinh doanh miễn phí này nằm ở thiết kế phần cứng: phía dưới màn hình chính của tivi được trang bị thêm một màn hình phụ độc lập chuyên phục vụ hiển thị quảng cáo liên tục không ngừng nghỉ ngay cả khi màn hình chính đang tắt:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051605.webp)

Đồng thời, hệ thống sẽ tiến hành thu thập chi tiết thói quen và thời lượng xem các chương trình truyền hình của gia đình. Nếu người dùng tắt tính năng thu thập dữ liệu này, họ bắt buộc phải trả lại tivi cho hãng. Liệu bạn có sẵn sàng chia sẻ thông tin cá nhân và chấp nhận xem quảng cáo liên tục để đổi lấy một chiếc tivi thông minh miễn phí?

2、[Chính quyền thành phố Baltimore khởi kiện hãng xe Kia vì xe quá dễ bị lấy trộm](https://www.thebaltimorebanner.com/community/criminal-justice/baltimore-lawsuit-hyundai-kia-thefts-WQ74KXUXTBGB3JOTHQHEGIPT6M/)

Chính quyền thành phố Baltimore, Mỹ đã chính thức nộp đơn khởi kiện hãng sản xuất ô tô Kia và Hyundai của Hàn Quốc với lý do thiết kế hệ thống bảo mật của các dòng xe này quá lỏng lẻo dẫn đến tình trạng mất trộm xe tăng vọt:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051301.webp)

Thời gian gần đây, số lượng vụ trộm cắp ô tô tại thành phố tăng đột biến, trong đó tuyệt đại đa số nạn nhân đều sở hữu các dòng xe Kia đời cũ thiếu bộ phận mã hóa động cơ (immobilizer). Do việc bẻ khóa quá dễ dàng, các video hướng dẫn trộm xe Kia bằng cáp USB đã lan truyền chóng mặt trên mạng xã hội TikTok thu hút hàng triệu lượt xem:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051302.webp)

Tình trạng trộm xe tràn lan gây áp lực rất lớn lên lực lượng cảnh sát tuần tra, đồng thời các đối tượng trộm xe thường lái xe lạng lách gây ra nhiều vụ tai nạn giao thông nghiêm trọng trước khi vứt xe bỏ trốn. Vụ việc là lời cảnh báo đắt giá cho các doanh nghiệp sản xuất phần cứng: việc chậm trễ cập nhật công nghệ bảo mật lỗi thời có thể dẫn đến nguy cơ pháp lý rất lớn.

3、[Nhật Bản thử nghiệm mô hình đường bộ tích hợp sạc không dây cho xe điện](http://tech.ce.cn/news/202209/27/t20220927_38129413.shtml)

Báo *Nikkei Asia* đưa tin một doanh nghiệp xây dựng tại Tokyo đang triển khai thử nghiệm mô hình làn đường giao thông thông minh tích hợp công nghệ sạc không dây cho phương tiện giao thông:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092908.webp)

Lớp dưới của mặt đường được lắp đặt hệ thống các cuộn dây điện từ chạy ngầm. Khi các phương tiện xe điện được trang bị cuộn cảm nhận năng lượng di chuyển qua đoạn đường này, dòng điện sẽ được truyền tải không dây trực tiếp vào pin xe thông qua hiện tượng cảm ứng từ trường, giúp kéo dài đáng kể quãng đường di chuyển của xe mà không cần dừng lại cắm sạc. Ý tưởng đặt một lượng lớn cuộn dây từ trường dưới lòng đường nhựa đô thị là một thử nghiệm táo bạo của các kỹ sư xây dựng.

4、[Nữ ca sĩ Grimes công bố chính sách chia sẻ tác quyền giọng hát AI](https://hypebeast.com/2023/5/grimes-ai-software-elf-tech-voice-music)

Trong bối cảnh nhiều nghệ sĩ lớn đang kịch liệt phản đối việc các mô hình AI sao chép và giả mạo giọng hát của mình, nữ ca sĩ nổi tiếng người Canada Grimes đã có một hướng tiếp cận hoàn toàn khác biệt:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051205.webp)

Cô thông báo cho phép cộng đồng tự do sử dụng phiên bản giọng hát giả lập AI của mình để sáng tác các tác phẩm âm nhạc mới, với một điều kiện duy nhất:

Người dùng phải tải bản nhạc tự sáng tác lên trang web công nghệ của cô để hệ thống tự động xử lý chuyển đổi giọng hát sang chất giọng AI của Grimes. Tác giả có toàn quyền phát hành bài hát đó lên các nền tảng âm nhạc, nhưng nếu bài hát phát sinh doanh thu thương mại, họ phải thực hiện chia sẻ 50% lợi nhuận về cho Grimes.

## Bài viết

1\. [Đúc kết nội dung bài phát biểu trực tiếp của kỹ sư kỳ cựu Trần Hạo](https://mp.weixin.qq.com/s/bOnW8gDJ-dXp4KbAjhDw9A)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051803.webp)

Bài viết tổng hợp lại nội dung cuộc phỏng vấn trực tiếp đầy ý nghĩa của kỹ sư phát triển kỳ cựu Trần Hạo (biệt danh Left Ears Mouse - người sáng lập MegaEase) chia sẻ về các quan điểm lập trình hệ thống, định hướng sự nghiệp và kinh nghiệm khởi nghiệp công nghệ, được đăng tải nhằm tưởng nhớ những đóng góp to lớn của ông cho cộng đồng lập trình viên.

2\. [Cẩm nang hướng dẫn sử dụng phiên bản Midjourney chính thức tại Trung Quốc](https://mp.weixin.qq.com/s/4NefHvl7A-o-hVm1PZr5Gw)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051820.webp)

Mô hình AI vẽ tranh hàng đầu thế giới Midjourney mới đây đã chính thức ra mắt phiên bản dịch vụ chuyên biệt dành riêng cho thị trường trong nước. Bài viết hướng dẫn chi tiết cách thức đăng ký tài khoản và trải nghiệm công cụ vẽ tranh này.

3\. [Nhìn lại buổi lên lớp giảng dạy cuối cùng của giáo sư toán học 88 tuổi tại MIT](https://www.jiqizhixin.com/articles/2023-05-16-2)（Tiếng Trung）

Giáo sư Gilbert Strang nổi tiếng thế giới với loạt bài giảng môn Đại số tuyến tính kinh điển tại Viện Công nghệ Massachusetts (MIT). Ở tuổi 88, vào ngày 15 tháng 5 vừa qua, ông đã chính thức thực hiện buổi lên lớp giảng dạy cuối cùng trong sự nghiệp của mình và được phát sóng trực tiếp tới hàng triệu học sinh trên thế giới:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051821.webp)

4\. [Thử nghiệm hiệu năng của công cụ đóng gói mã nguồn tích hợp trên Bun.js](https://shaneosullivan.wordpress.com/2023/05/17/using-bun-js-as-a-bundler/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051811.webp)

Môi trường chạy JavaScript thế hệ mới Bun.js vừa tích hợp thêm tính năng đóng gói mã nguồn (Bundler) mặc định. Bài viết thực nghiệm so sánh tốc độ đóng gói dự án thực tế của Bun.js chỉ ra tốc độ xử lý của nó vượt trội hoàn toàn so với Webpack hay Esbuild.

5\. [Tìm hiểu nguyên lý vận hành cơ bản của kỹ thuật phân mảnh dữ liệu](https://planetscale.com/blog/how-does-database-sharding-work)（Tiếng Anh）

Bài viết cơ bản giải thích cặn kẽ thuật ngữ phân mảnh cơ sở dữ liệu (Database Sharding) – một giải pháp kỹ thuật cốt lõi giúp chia nhỏ các bảng dữ liệu khổng lồ ra nhiều máy chủ vật lý khác nhau để tăng hiệu suất đọc ghi cho các hệ thống lớn.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040703.webp)

6\. [Mẹo nhỏ ngắt các kết nối SSH bị treo không phản hồi trên dòng lệnh](https://davidisaksson.dev/posts/closing-stale-ssh-connections/)（Tiếng Anh）

Khi kết nối với máy chủ qua giao thức SSH, nếu người dùng không tương tác trong thời gian dài, phiên kết nối thường bị treo cứng và terminal không nhận phím bấm. Bài viết hướng dẫn phím tắt thoát nhanh phiên SSH bị treo một cách dễ dàng.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041001.webp)

7\. [Phân tích chi tiết thuật toán xếp hạng tin tức của trang Hacker News](https://vigneshwarar.substack.com/p/hackernews-ranking-algorithm-how)（Tiếng Anh）

Bài phân tích toán học giải thích cách thức trang tin tức công nghệ hàng đầu Hacker News sử dụng số điểm bình chọn (upvotes) kết hợp với trọng số thời gian trôi qua để tính toán vị trí hiển thị của các bài viết trên trang chủ.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041005.webp)

8\. [Khám phá các phương thức viết địa chỉ IP độc đáo trong mạng máy tính](https://ma.ttias.be/theres-more-than-one-way-to-write-an-ip-address/)（Tiếng Anh）

Địa chỉ IP thường được viết dưới dạng chuẩn 4 nhóm số phân cách bằng dấu chấm (ví dụ `127.0.0.1`). Bài viết giới thiệu các định dạng viết địa chỉ IP rút gọn hoặc chuyển đổi hệ cơ số khác (như `127.1`) mà hệ điều hành vẫn nhận diện chính xác.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042905.webp)

## 工具

1、[Astrodon: Bộ công cụ phát triển ứng dụng desktop đa nền tảng bằng Deno](https://github.com/astrodon/astrodon)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081606.webp)

Một framework hỗ trợ lập trình ứng dụng máy tính đa nền tảng sử dụng runtime Deno, hoạt động tương tự Electron nhưng tận dụng nhân Tauri phía dưới để tối ưu hóa dung lượng cài đặt siêu nhẹ.

2、[HuggingChat: Trang chủ trải nghiệm chatbot AI nguồn mở của Hugging Face](https://huggingface.co/chat)

Giao diện trò chuyện trực tuyến hoàn toàn miễn phí do nền tảng AI lớn Hugging Face xây dựng, cho phép người dùng tùy chọn kết nối và hỏi đáp với nhiều mô hình ngôn ngữ lớn nguồn mở khác nhau:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051202.webp)

3、[Chat with any PDF: Công cụ tương tác hỏi đáp thông tin trực tiếp với file PDF](https://damngood.tools/tools/chat-pdf)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051207.webp)

Ứng dụng Web hỗ trợ người dùng tải tài liệu PDF lên hệ thống để AI tự động đọc hiểu, sau đó người dùng có thể gõ câu hỏi bằng tiếng Việt để AI tự tìm kiếm và tóm tắt thông tin trả lời tương ứng. Một dịch vụ tương tự là [ScholarTurbo](https://scholarturbo.com/).

4、[Nature: Ngôn ngữ lập trình thế hệ mới hướng tới cú pháp tự nhiên](https://github.com/nature-lang/nature)

Một ngôn ngữ lập trình mới do lập trình viên trong nước tự thiết kế, hướng tới mục tiêu xây dựng một cấu trúc cú pháp tối giản, tự nhiên, dễ đọc tương tự như ngôn ngữ tự nhiên của con người. (Đóng góp của [@weiwenhao](https://github.com/ruanyf/weekly/issues/3117))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051801.webp)

5、[LaWGPT: Mô hình ngôn ngữ lớn nguồn mở chuyên sâu về luật pháp Trung Quốc](https://github.com/pengxiao-song/LawGPT)

Dự án phát triển mô hình ngôn ngữ lớn được huấn luyện chuyên biệt trên kho dữ liệu hiến pháp, luật và các văn bản tư pháp nhằm phục vụ việc hỗ trợ ôn thi chứng chỉ ngành luật. (Đóng góp của [@pengxiao-song](https://github.com/ruanyf/weekly/issues/3116))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051813.webp)

6、[mblog: Hệ thống mạng xã hội tin nhắn ngắn đa người dùng viết bằng Java](https://github.com/kingwrcy/mblog-backend)

Mã nguồn mở xây dựng ứng dụng mạng xã hội tiểu blog hỗ trợ nhiều tài khoản người dùng đăng tải tin nhắn ngắn, được phát triển trên nền tảng Java kết hợp cơ sở dữ liệu MySQL. (Đóng góp của [@kingwrcy](https://github.com/ruanyf/weekly/issues/3121))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051814.webp)

7、[wallpaper-box: Ứng dụng quản trị và thiết lập hình nền desktop](https://github.com/wangrongding/wallpaper-box)

Ứng dụng cài đặt hình nền máy tính viết bằng Electron, hỗ trợ tải các bộ sưu tập hình nền chất lượng cao, thiết lập hình nền động (video) và tùy biến biểu tượng khay hệ thống. (Đóng góp của [@wangrongding](https://github.com/ruanyf/weekly/issues/3118))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051815.webp)

8、[Pho: Ứng dụng quản lý ảnh Android hỗ trợ đồng bộ dữ liệu lên ổ cứng mạng NAS](https://github.com/fregie/pho)

Một ứng dụng thư viện ảnh nguồn mở dành cho thiết bị Android, hỗ trợ tự động sao lưu và đồng bộ hình ảnh chụp từ điện thoại lên các thiết bị lưu trữ NAS trong gia đình qua các giao thức mạng SMB, WebDAV hoặc NFS. (Đóng góp của [@fregie](https://github.com/ruanyf/weekly/issues/3122))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051816.webp)

9、[Bilibili Subtitle List: Tiện ích xem danh sách phụ đề video trên Bilibili](https://github.com/IndieKKY/bilibili-subtitle)

Extension dành cho trình duyệt hỗ trợ trích xuất toàn bộ nội dung phụ đề của video Bilibili thành một danh sách văn bản có gắn mốc thời gian, cho phép người dùng click chuột vào dòng chữ để tua nhanh tới phân cảnh tương ứng. (Đóng góp của [@IndieKKY](https://github.com/ruanyf/weekly/issues/3123))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051817.webp)

10、[stitching: Thư viện Python hỗ trợ ghép nối hình ảnh Panorama](https://github.com/lukasalexanderweber/stitching)

Bộ thư viện lập trình Python chuyên dụng cung cấp các thuật toán ghép nối tự động nhiều bức ảnh chụp góc hẹp liền kề nhau để tạo thành một bức ảnh phong cảnh góc rộng panorama duy nhất chất lượng cao.

## 资源

1、[Data Viz Project: Thư viện tổng hợp các dạng sơ đồ trực quan hóa dữ liệu](https://datavizproject.com/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053106.webp)

Trang web chuyên cập nhật và giới thiệu chi tiết về hàng trăm định dạng biểu đồ, sơ đồ thống kê số liệu khác nhau cùng các ví dụ thực tế hướng dẫn lập trình viên lựa chọn phương án trực quan hóa dữ liệu tối ưu.

2\. [Awesome ChatGPT: Danh mục tuyển chọn các tài nguyên hữu ích về ChatGPT](https://github.com/sindresorhus/awesome-chatgpt)

Dự án Awesome GitHub do lập trình viên nổi tiếng Sindre Sorhus khởi xướng, chuyên tổng hợp các liên kết ứng dụng, tiện ích mở rộng và tài liệu hướng dẫn phát triển xoay quanh ChatGPT:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051606.webp)

3、[Spring Chinese Document: Thư viện tài liệu kỹ thuật Spring Framework tiếng Việt](https://springdoc.cn/)

Trang web lưu trữ hệ thống tài liệu hướng dẫn lập trình và tra cứu API của hệ sinh thái Spring Framework bằng tiếng Trung được dịch thuật và cập nhật đầy đủ nhất. (Đóng góp của [@KevinBlandy](https://github.com/ruanyf/weekly/issues/3112))

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051802.webp)

4、[Wikiversity: Dự án thư viện khóa học trực tuyến mở của Wikimedia](https://en.wikiversity.org/wiki/Wikiversity:Main_Page)

Một dự án chính thức trực thuộc quỹ Wikimedia, hoạt động tương tự Wikipedia nhưng tập trung vào việc cho phép các tình nguyện viên biên soạn các giáo trình khóa học mở về mọi chủ đề học thuật trên thế giới.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102716.webp)

5、[PrintableSearch: Công cụ tìm kiếm các mẫu thiết kế 3D in ấn miễn phí](https://www.printablesearch.com/)

Công cụ tìm kiếm chuyên dụng giúp người dùng nhanh chóng quét và tải về các tệp tin thiết kế mô hình 3D (STL files) hoàn toàn miễn phí từ các kho chia sẻ lớn để phục vụ việc in 3D.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041704.webp)

## 图片

1、**Mô hình giao nhận đồ ăn xuyên biên giới độc đáo tại biên giới Mỹ - Mexico**

Tại khu vực hàng rào biên giới ngăn cách giữa hai nước Mỹ và Mexico tập trung một lượng lớn người dân tị nạn đang chờ làm thủ tục. Do không muốn rời bỏ vị trí xếp hàng dài trong thời gian lâu, họ đã nghĩ ra một cách độc đáo để giải quyết nhu cầu ăn uống:

Sử dụng điện thoại kết nối mạng di động của Mexico để đặt đồ ăn qua các ứng dụng giao hàng trực tuyến của Mexico, sau đó các shipper từ phía Mexico sẽ vận chuyển đồ ăn tới và đưa qua khe hở của bức tường rào biên giới cho người mua:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051208.webp)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051209.webp)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051210.webp)

2、**Jizai Arms: Thiết bị tăng cường nhiều cánh tay robot đeo lưng của Nhật Bản**

Một doanh nghiệp công nghệ robot của Nhật Bản mới đây đã giới thiệu thiết bị cơ khí sinh học độc đáo mang tên Jizai Arms: cho phép người dùng đeo một balo cơ khí sau lưng để lắp thêm tối đa 6 cánh tay robot hoạt động đồng thời:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051806.webp)

Các cánh tay robot này được điều khiển trực quan dựa trên các chuyển động cơ thể của người đeo, hướng tới việc hỗ trợ người khuyết tật phục hồi vận động hoặc hỗ trợ công nhân tăng cường năng lực khuân vác trong các nhà xưởng.

## ✍️ Bài đọc thêm

### Cơ chế chia sẻ băng thông truyền phát video qua giao thức P2P tại Trung Quốc

Giao thức P2P (Peer-to-Peer - mạng ngang hàng) là phương thức chia sẻ dữ liệu giúp tiết kiệm băng thông máy chủ rất phổ biến trong công nghệ tải file trước đây:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051822.webp)

Tại các quốc gia phương Tây, giao thức P2P hầu như chỉ được ứng dụng cho việc tải tệp tin dung lượng lớn, rất hiếm khi được áp dụng cho truyền phát video trực tuyến (video streaming) do trải nghiệm người dùng kém, thường xuyên phát sinh hiện tượng lag giật chờ load bộ đệm:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051823.webp)

Tuy nhiên, hầu như toàn bộ các tập đoàn video trực tuyến lớn tại Trung Quốc đều lạm dụng triệt để công nghệ P2P này nhằm cắt giảm tối đa chi phí thuê băng thông đường truyền CDN đắt đỏ. Phương pháp này hoạt động hiệu quả nhờ vào quy mô người dùng cực lớn của thị trường:

* **Đối với truyền phát trực tiếp (Livestream)**: Tệp người dùng thường tập trung rất đông vào top 1% các phòng livestream của các streamer nổi tiếng. Khi số lượng người xem đồng thời đạt hàng triệu người, hiệu năng chia sẻ P2P đạt mức tối đa (nguyên lý P2P: số lượng người tải càng nhiều thì tốc độ chia sẻ chéo giữa các máy càng nhanh), giúp nhà đài tiết kiệm được phần lớn chi phí băng thông máy chủ.
* **Đối với truyền phát theo yêu cầu (Video on Demand)**: Đối với các bộ phim có ít người xem đồng thời, hiệu năng P2P truyền thống sẽ rất kém. Để khắc phục, các doanh nghiệp video đã sản xuất và phân phối các thiết bị định tuyến thông minh (thường gọi là "Hộp hạt giống - Seedbox") cho người dùng gia đình. Người dùng mua thiết bị này cắm sạc sử dụng như bộ phát Wifi thông thường, nhưng hệ thống sẽ chạy ngầm để lưu trữ các video phổ biến và biến máy khách thành một nút CDN biên mini chia sẻ băng thông cho những người dùng khác xung quanh. Đổi lại, người dùng chia sẻ băng thông sẽ nhận về các điểm tích lũy số để đổi quà tặng hoặc tiền mặt.

Tuy nhiên đối với các video cũ có lượng người xem cực kỳ ít, hệ thống vẫn bắt buộc phải duy trì hạ tầng CDN truyền thống làm phương án dự phòng tải trang cuối cùng. Thành công của mô hình P2P tại đây phần lớn nhờ vào quy mô dân số số đông đặc thù giúp giảm thiểu tối đa các nhược điểm của công nghệ.

## Lịch sử tuần này

- 2022年（第 208 期）：[Văn hóa doanh nghiệp: Thảo luận về các lỗi thiết kế phổ biến của hệ thống thăng tiến nhân sự](http://www.ruanyifeng.com/blog/2022/05/weekly-issue-208.html)
- 2021年（第 158 期）：[Kinh tế số: Góc nhìn về việc giảm giá trị chiến lược của các kênh phân phối nội dung](http://www.ruanyifeng.com/blog/2021/05/weekly-issue-158.html)
- 2020年（第 108 期）：[Chiến lược kinh doanh: So sánh mô hình phát triển kiểu trận địa chiến và chiến thuật tập kích nhanh](http://www.ruanyifeng.com/blog/2020/05/weekly-issue-108.html)
- 2019年（第 58 期）：[Thảo luận: Liệu chúng ta có thể áp dụng chiến dịch quảng bá phần mềm tương tự như ngành mỹ phẩm](http://www.ruanyifeng.com/blog/2019/05/weekly-issue-58.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs is a comprehensive dynamic workspace.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
