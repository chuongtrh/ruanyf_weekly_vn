# 科技爱好者周刊（第 404 期）：你需要知道的 AI 内存知识 (Bản tin công nghệ hàng tuần số 404: Những điều bạn cần biết về bộ nhớ AI)

Ghi lại nội dung công nghệ đáng chia sẻ hàng tuần, phát hành vào thứ Sáu.

Bản tin này [mã nguồn mở](https://github.com/ruanyf/weekly), hoan nghênh bạn [đóng góp](https://github.com/ruanyf/weekly/issues). Ngoài ra còn có dịch vụ [《Ai đang tuyển dụng》](https://github.com/ruanyf/weekly/issues/10517) đăng tải thông tin tuyển dụng lập trình viên. Hợp tác vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## Ảnh bìa

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071603.webp)

Triển lãm "SpongeBob SquarePants" (Hải miên bảo bảo) đang diễn ra tại một trung tâm thương mại ở Thượng Hải. ([via](https://m.thepaper.cn/newsDetail_forward_33450995))

## 你需要知道的 AI 内存知识 (Những điều bạn cần biết về bộ nhớ AI)

Để tự chạy các mô hình AI tại nhà, bạn có hai lựa chọn phần cứng.

Một là card màn hình rời (dedicated graphics card). Hiện tại, card đồ họa tiêu dùng hàng đầu là Nvidia RTX 5090, sở hữu 32GB VRAM (bộ nhớ đồ họa), với mức giá khoảng 30.000 Nhân dân tệ.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071511.webp)

Hai là máy tính gia đình sử dụng chipset tích hợp (gồm CPU + card đồ họa onboard + RAM onboard), chẳng hạn như Mini PC sử dụng chipset Strix Halo của AMD (model cụ thể là Ryzen AI Max+ 395), tích hợp sẵn 128GB RAM, với mức giá khoảng 20.000 Nhân dân tệ.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071512.webp)

Tôi hỏi các bạn, phần cứng nào tốt hơn?

Hầu hết mọi người có lẽ sẽ chọn ngay card đồ họa rời không cần suy nghĩ, vì hiệu năng tính toán của card rời lớn hơn nhiều so với chipset onboard.

Theo tài liệu tôi tìm hiểu, dưới đây là hiệu năng tính toán số thực đơn độ chính xác 32-bit (FP32) của cả hai:

> - Card đồ họa rời (RTX 5090): **104.8 TFLOPS**
> - Chipset onboard (AMD Ryzen AI Max+ 395): **14.8 TFLOPS**

Có thể thấy, hiệu năng tính toán của card rời cao gấp 7 lần so với chipset onboard. Nếu thực hiện các phép tính số thực dấu phẩy động với số bit nhỏ hơn (như FP16 và FP4), khoảng cách hiệu năng thậm chí còn lớn hơn nữa.

Tuy nhiên, tôi muốn nói với bạn rằng câu trả lời chính xác thực ra là "Chưa chắc". Trong nhiều trường hợp, một chiếc Mini PC sử dụng chipset onboard mới là giải pháp chạy mô hình AI cục bộ tốt hơn.

Vấn đề nằm ở chỗ bộ nhớ đồ họa VRAM 32GB của nó thực sự quá ít. Một mô hình với tham số quy mô 70B (70 tỷ), nếu mỗi tham số sử dụng độ chính xác 4-bit, thì việc nạp tất cả trọng số tham số vào bộ nhớ cần khoảng 32.6GB dung lượng. Con số này vượt quá giới hạn VRAM của RTX 5090, khiến nó hoàn toàn không thể khởi chạy.

Ngược lại, chiếc Mini PC của AMD sở hữu 128GB RAM onboard, giúp việc nạp mô hình trở nên vô cùng dễ dàng. **Bộ nhớ của chipset onboard được chia sẻ dùng chung giữa card đồ họa onboard và CPU, do đó được gọi là "Bộ nhớ thống nhất" (Unified Memory)**. Ưu điểm của nó là có thể phân bổ nhiều bộ nhớ nhất có thể cho một bộ xử lý đơn lẻ, nhờ vậy xử lý được các mô hình AI tiêu tốn dung lượng bộ nhớ lớn.

Các chip dòng M của Apple luôn áp dụng kiến trúc "Bộ nhớ thống nhất" này, và các nhà sản xuất khác hiện nay cũng đã bắt kịp. Strix Halo của AMD, DGX Spark của NVIDIA, Core Ultra của Intel và Snapdragon X của Qualcomm đều sử dụng kiến trúc này. Ngoài dung lượng bộ nhớ lớn, giá thành của nó cũng thấp hơn so với card đồ họa rời.

Đọc đến đây, có thể bạn sẽ hỏi: Với những ưu điểm như vậy của chipset onboard, liệu có cần thiết phải mua card đồ họa rời nữa không?

Câu trả lời là bộ nhớ có hai chỉ số quan trọng, ngoài dung lượng lưu trữ, còn có một chỉ số khác là "băng thông bộ nhớ" (memory bandwidth). **Điểm yếu của chipset onboard lại chính là băng thông bộ nhớ.**

Khái niệm "băng thông bộ nhớ" chỉ tốc độ truyền dữ liệu từ bộ nhớ đến bộ xử lý. Mặc dù RTX 5090 không có nhiều dung lượng VRAM, nhưng băng thông của nó cực kỳ lớn, đạt tới 1792GB/s, trong khi băng thông của AMD chỉ có 256GB/s.

Mỗi khi mô hình AI tạo ra một Token, bộ xử lý cần đọc toàn bộ mô hình từ bộ nhớ để thực hiện tính toán. Nếu băng thông bộ nhớ là 256GB/s, thì với một mô hình có dung lượng 40GB, bộ xử lý chỉ có thể đọc 6 lần mỗi giây (256 chia cho 40), nghĩa là chỉ tạo ra được 6 Token mỗi giây (đây là giá trị lý thuyết, thực tế có thể không đạt được). Tốc độ chậm chạp như rùa bò này thì ai chịu nổi?

Ngay cả chip Apple M3 Ultra có băng thông bộ nhớ lớn nhất ở mức 819GB/s thì cũng chỉ tạo ra khoảng 20 Token mỗi giây, kém xa mức 1792GB/s của RTX 5090.

Vì thế, cả dung lượng bộ nhớ và băng thông bộ nhớ đều là những nút thắt cổ chai (bottlenecks) của mô hình AI. Đây cũng là lý do tại sao giá của bộ nhớ băng thông cao (HBM) tăng phi mã.

Nếu bạn chọn Mini PC chạy chipset onboard, bạn phải chuẩn bị tâm lý chấp nhận tốc độ tạo Token cực kỳ chậm.

May thay, để tiết kiệm lượng tính toán, kiến trúc "Mô hình hỗn hợp chuyên gia" (MoE - Mixture of Experts) đã ra đời. **Khi tính toán Token, nó không cần đọc toàn bộ tham số mà chỉ cần kích hoạt một phần tham số.**

Lấy mô hình Qwen3-30B-A3B làm ví dụ, nó chứa 30 tỷ tham số nhưng mỗi lần chỉ kích hoạt 3 tỷ tham số. Do đó, lượng dữ liệu cần đọc cho mỗi Token không phải là 20GB mà chỉ là 2GB. Như vậy trên Mini PC của AMD, tốc độ lý thuyết có thể đạt hơn 100 Token mỗi giây, một tốc độ khá tốt.

Vì vậy, nếu bạn dùng Mini PC có chế độ "Bộ nhớ thống nhất", hãy ưu tiên chọn mô hình MoE.

Ngoài ra, Mini PC còn có một nhược điểm lớn khác không liên quan đến bộ nhớ, mà liên quan đến hiệu năng tính toán chậm.

Chúng ta biết rằng mô hình phải xử lý các từ gợi ý (prompts) của người dùng trước khi có thể tạo ra Token. Vì hiệu năng tính toán của Mini PC chậm nên tốc độ xử lý prompt cũng rất chậm.

Theo đo lường thực tế, Mini PC của AMD chạy mô hình 70B có tốc độ xử lý prompt là 95 Token mỗi giây. Như vậy, nếu người dùng gửi một tài liệu dài 4.000 Token, máy sẽ mất khoảng 40 giây để xử lý xong trước khi xuất ra Token đầu tiên.

Có thể hình dung, một khi người dùng đưa lượng lớn nội dung vào cửa sổ ngữ cảnh (context window), việc chỉ xử lý prompt thôi cũng có thể tốn từ vài phút đến vài chục phút.

Tóm lại, ở giai đoạn hiện tại, việc muốn chạy mô hình lớn trên máy tính cục bộ dù là card đồ họa rời hay chipset onboard đều có những khuyết điểm. Bạn chỉ có thể chạy tốt một số mô hình MoE quy mô trung bình và từ gợi ý không được quá dài.

## 布尔变量如何起名 (Cách đặt tên cho biến Boolean)

Trong giới lập trình lưu truyền một câu chuyện về hai bài toán khó nhất: một là vô hiệu hóa bộ nhớ đệm (cache invalidation), và hai là đặt tên biến.

Trong đó, biến Boolean đặc biệt khó đặt tên. Làm thế nào để diễn đạt một cách chính xác rằng biến này biểu thị giá trị đúng (true) hoặc sai (false)?

Gần đây tôi đọc được một bài viết [《Nghệ thuật đặt tên biến Boolean》](https://thatamazingprogrammer.com/posts/stop-naming-your-variables-flag-the-art-of-boolean-prefixes/), đề xuất sử dụng bốn tiền tố để đặt tên biến Boolean đúng cách, tôi thấy rất có gợi mở.

1. **is-**: mô tả trạng thái của sự vật, phía sau là tính từ, ví dụ: isActive, isDeleted, isEmpty.
2. **has-**: mô tả quyền sở hữu hoặc quan hệ chứa đựng của sự vật, phía sau là danh từ, ví dụ: hasAccess, hasChildren, hasValidationErrors.
3. **can-**: mô tả khả năng hoặc quyền hạn của sự vật, ví dụ: canEdit, canDelete, canRetry.
4. **should-**: mô tả ý định hoặc logic của sự vật, ví dụ: shouldRetry, shouldCacheResponse.

Bên cạnh bốn tiền tố này, còn có một quy tắc đặt tên khác: Không bao giờ sử dụng từ phủ định trong tên biến Boolean.

Ví dụ, không sử dụng isDisabled, mà hãy dùng `isEnabled = false`.

## 科技动态 (Tin tức Công nghệ)

1、[Bàn phím OpenAI](https://openai.com/zh-Hans-CN/supply/co-lab/work-louder/)

Công ty OpenAI vừa ra mắt một mẫu bàn phím tiện lợi giúp thao tác dễ dàng hơn với các AI Agent.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071601.webp)

Phía dưới bàn phím là một dãy phím tắt dùng để phê duyệt (approve), bác bỏ (deny), nhập liệu bằng giọng nói, v.v. Phía trên là một dải đèn RGB hiển thị trạng thái hiện tại của AI Agent (đang suy nghĩ, đang chạy, đang đợi, hoàn thành).

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071602.webp)

Sản phẩm này có giá 230 USD, trông không có gì mới mẻ và chưa chắc đã tiện dụng hơn bàn phím thông thường.

Nhà thiết kế nổi tiếng Jony Ive sau khi rời Apple hiện đang chịu trách nhiệm thiết kế phần cứng cho OpenAI. Mọi người đều hy vọng ông có thể mang lại một thiết bị thông minh đột phá, nhưng mẫu bàn phím nhỏ ra mắt đầu tiên này thực sự gây thất vọng.

2、[Tiểu hành tinh 2016HO3](https://www.cnsa.gov.cn/n6758823/n6758838/c10760422/content.html)

Tàu thăm dò Thiên Vấn 2 (Tianwen-2) được phóng vào tháng 5 năm 2025, sau khoảng 400 ngày bay, cuối cùng đã tiếp cận mục tiêu — tiểu hành tinh 2016HO3 và gửi ảnh về.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071501.webp)

Tiểu hành tinh này có chiều dài khoảng 20 mét, chỉ lớn hơn một chút so với nửa sân bóng rổ tiêu chuẩn, hình dạng không đều và có các góc nhọn, chứng tỏ đây là mảnh vỡ sau một vụ va chạm chứ không phải do dung nham nguội đi hình thành.

Khi Thiên Vấn 2 chụp ảnh, nó cách tiểu hành tinh này 20 km. Bước tiếp theo theo kế hoạch sẽ là lấy mẫu đất đá từ tiểu hành tinh này để mang về Trái Đất.

Cái khó của nhiệm vụ này là sải cánh của Thiên Vấn 2 đạt tới 15 mét, chỉ nhỏ hơn một chút so với tiểu hành tinh này, quá trình lấy mẫu có thể làm thay đổi quỹ đạo của tiểu hành tinh.

3、[Máy dệt sức gió](https://www.merelkarhof.nl/work/wind-knitting-factory)

Một nhà thiết kế người Hà Lan đã phát minh ra máy dệt len chạy bằng sức gió dùng cho hộ gia đình, có thể lắp đặt ở ban công hoặc sân thượng.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070405.webp)

Sức gió làm quay các cánh quạt, vận hành một bàn xoay dệt tròn để dệt len thành những chiếc khăn quàng cổ.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070406.webp)

Khi gió lớn, tốc độ dệt cực kỳ nhanh. Nó trông giống như một thiết bị thuần cơ khí, không sử dụng điện gió.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070407.webp)

Ý định ban đầu của nhà thiết kế là cho mọi người thấy rằng, ngay cả trong các tòa nhà đô thị cũng có thể tận dụng sức gió.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070408.webp)

## 文章 (Bài viết)

1、[Hướng dẫn tìm việc cho Tiến sĩ Machine Learning](https://silviasapora.github.io/blog/ml-interviews.html) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071509.webp)

Tác giả là một tiến sĩ tốt nghiệp ngành Machine Learning ở Mỹ, hiện đã vào làm việc tại DeepMind. Bài viết này là phần hồi tưởng và tổng kết lại quá trình tìm việc của tác giả.

Ngoài ra còn có một bài viết [tương tự](https://alisawuffles.github.io/blog/job-search/).

2、[Sử dụng DNS để xác thực ACME](https://hsm.tunnel53.net/article/dns-for-acme-challenges/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092405.webp)

Chứng chỉ HTTPS miễn phí cần được cấp thông qua giao thức ACME. Giao thức này yêu cầu xác thực quyền sở hữu tên miền, và một phương pháp xác thực là sử dụng DNS. Bài viết này giải thích nguyên lý hoạt động của nó.

3、[Tình thế tiến thoái lưỡng nan của ngôn ngữ Go](https://www.andrewvittiglio.com/thoughts/go-killed-arenas) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120608.webp)

Bài viết cho rằng ngôn ngữ Go đang ở vị thế ngượng ngùng, tương lai không mấy sáng sủa. "Khi các ngôn ngữ chậm trở nên nhanh hơn, các ngôn ngữ khó trở nên dễ dàng hơn, phân khúc tầm trung mà Go đang chiếm giữ sẽ không còn tồn tại."

4、[So sánh tốc độ các thuật toán băm (hash) trong JavaScript](https://lemire.me/blog/2025/01/11/javascript-hashing-speed-comparison-md5-versus-sha-256/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025011918.webp)

MD5 và SHA256 đều là các thuật toán băm thông dụng. Bài viết tìm hiểu xem trong ngôn ngữ JavaScript, thuật toán băm nào có tốc độ tạo nhanh hơn? Câu trả lời có thể khác với những gì bạn nghĩ.

5、[Bảng tra cứu ký tự điều khiển trong Terminal](https://jvns.ca/blog/2024/10/31/ascii-control-characters/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110405.webp)

Tác giả đã vẽ một biểu đồ (hình trên), liệt kê các phím tắt điều khiển dòng lệnh có thể sử dụng (ví dụ Ctrl-C để chấm dứt lệnh hiện tại), tổng cộng gồm 33 phím tắt.

6、[Richard Feynman gia nhập công ty khởi nghiệp của tôi](https://longnow.org/ideas/richard-feynman-and-the-connection-machine/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071605.webp)

Tác giả hồi tưởng lại nhà vật lý nổi tiếng Richard Feynman từng gia nhập startup của mình để cùng phát triển siêu máy tính, chứa đựng nhiều câu chuyện rất thú vị.

## 工具 (Công cụ)

1、[WhatCable](https://github.com/darrylmorley/whatcable)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071510.webp)

Ứng dụng trên thanh menu của macOS, hiển thị các đặc trưng của cáp USB-C đang cắm vào máy tính.

2、[amber](https://amber-lang.com/)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071401.webp)

Một ngôn ngữ mới giúp đơn giản hóa cú pháp Bash, các script viết bằng ngôn ngữ này có thể được biên dịch thành Bash.

3、[Ant](https://antjs.org)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071402.webp)

Một runtime gọn nhẹ cho JS/TS, có vẻ được tự viết từ đầu, file binary chỉ nặng 8MB.

4、[屏译 (Screen Translator)](https://github.com/ciddwd/overlay-translator)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071404.webp)

Ứng dụng Android mã nguồn mở, hỗ trợ dịch thuật trực tiếp trên màn hình theo thời gian thực. (Đóng góp từ [@ciddwd](https://github.com/ruanyf/weekly/issues/10701))

5、[TurboOCR](https://turboocr.com/)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071406.webp)

Công cụ nhận diện ký tự quang học (OCR) tốc độ cao sử dụng GPU. (Đóng góp từ [@nataell95](https://github.com/ruanyf/weekly/issues/10706))

Ngoài ra còn có thư viện nhận diện chữ cục bộ [light-ocr](https://github.com/arcships/light-ocr) cung cấp API cho JS/C++. (Đóng góp từ [@eric8810](https://github.com/ruanyf/weekly/issues/10714))

6、[Visprex](https://visprex.com/)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024111013.webp)

Trang web cho phép tải lên tệp dữ liệu CSV để tự động tạo biểu đồ trực quan.

7、[Loro](https://www.loro.dev/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111321.webp)

Thư viện thuật toán đồng bộ CRDT mã nguồn mở dùng để đồng bộ hóa trạng thái theo thời gian thực cho nhiều người dùng.

8、[File Wizard](https://github.com/LoredCast/filewizard)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025100202.webp)

Dịch vụ self-hosted chạy trên Web giúp chuyển đổi các định dạng tệp thông dụng, hỗ trợ OCR hình ảnh và chuyển đổi âm thanh thành văn bản.

## AI 相关 (AI Liên quan)

1、[Oh My HuggingFace](https://github.com/oh-my-hf/ohmyhf)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071405.webp)

Ứng dụng khách không chính thức cho Hugging Face, đa nền tảng và mã nguồn mở, dùng để duyệt tìm và tải xuống các mô hình, tập dữ liệu. (Đóng góp từ [@fzlzjerry](https://github.com/ruanyf/weekly/issues/10705))

2、[pi-auto-approval](https://github.com/Europa2061/pi-auto-approval)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071403.webp)

Plugin dành cho lập trình viên AI agent (như Pi agent), tự động phê duyệt các quyền xác nhận có mức rủi ro thấp, trong khi các quyền rủi ro cao vẫn được chuyển đến người dùng để xác nhận. (Đóng góp từ [@Europa2061](https://github.com/ruanyf/weekly/issues/10669))

3、[GPT Crawler](https://github.com/BuilderIO/gpt-crawler)

Công cụ này giúp thu thập nội dung của một trang web được chỉ định thành một tệp JSON, sau đó tải lên ChatGPT để tạo chatbot của riêng trang web đó, cho phép bạn chat trực tiếp với nội dung của trang web.

4、[Tokenwiz](https://github.com/1rgs/tokenwiz)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111305.webp)

Thư viện mã nguồn mở mô phỏng thuật toán phân tách từ khóa (tokenization) của OpenAI.

## 资源 (Tài nguyên)

1、[Goto Onion](https://gotoonion.site/)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071506.webp)

Cổng kết nối vào các trang web Tor (dark web), giúp các trình duyệt thông thường có thể truy cập được các đường link Onion.

2、[Fading Maize](https://www.fadingmaize.com/)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071507.webp)

Một trang web thú vị kể về một ban nhạc đại học Mỹ từng thu âm album vào năm 2001 rồi giải tán. Hiện tại, họ sử dụng AI để chuyển đổi các bản thu âm năm xưa sang phong cách của năm 2026. Trang web cung cấp cả hai bản thu âm để mọi người so sánh.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071508.webp)

Âm nhạc thật kỳ diệu, âm nhạc từ hơn 20 năm trước không hề mang dấu vết thời gian, tiếng guitar vang lên như mới hôm qua.

3、[Maze Algorithms (Thuật toán mê cung)](https://www.jamisbuck.org/mazes/)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026012505.webp)

Trang web này tổng hợp các thuật toán tạo mê cung khác nhau.

## 图片 (Hình ảnh)

1、[海底环岛 (Vòng xuyến dưới đáy biển)](https://visitfaroeislands.com/en/plan-your-stay/getting-around/world-first-under-sea-roundabout)

Vòng xuyến giao thông thường được đặt ở các ngã tư đông đúc, nhưng ở quần đảo Faroe thuộc Đại Tây Dương, có một vòng xuyến dưới đáy biển độc nhất vô nhị trên thế giới.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071502.webp)

Hình trên là sơ đồ đường hầm dưới đáy biển của quần đảo Faroe, tại vị trí khoanh tròn màu vàng, đường hầm chia làm hai ngã đi đến hai hòn đảo khác nhau. Tại đây người ta đã xây dựng một vòng xuyến dưới biển.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071503.webp)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071504.webp)

Để thu hút sự chú ý của các tài xế, chính quyền đã thuê nghệ sĩ trang trí nó thành hình dáng một con sứa.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026071505.webp)

## 文摘 (Văn trích)

1、[AI vốn dĩ để tiết kiệm thời gian, giảm khối lượng công việc](https://decrypt.co/357527/ai-save-time-instead-created-new-kind-burnout)

Mọi người vốn nghĩ AI sẽ giúp tiết kiệm thời gian và giảm khối lượng công việc, nhưng một cuộc khảo sát của Đại học California cho thấy điều ngược lại. AI làm tăng khối lượng công việc, đẩy cao cường độ làm việc, dẫn đến tình trạng kiệt sức nghề nghiệp (burnout).

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026021615.webp)

**Tại sao AI không những không giảm bớt việc mà còn làm tăng việc?** Nguyên nhân có thể do các điểm sau:

**(1) Phạm vi trách nhiệm công việc bị mở rộng**. Các product manager giờ đây bắt đầu viết code, các nhà nghiên cứu bắt đầu bảo trì máy chủ, trách nhiệm công việc không còn rạch ròi mà trở nên mờ nhạt. Nhân viên bắt đầu xử lý các công việc ngoài phạm vi của mình, và AI làm cho sự chuyển dịch này trở nên khả thi.

Điều này tạo ra hiệu ứng dây chuyền. Các kỹ sư đột nhiên phát hiện mình phải kiểm tra, sửa lỗi và hướng dẫn mã nguồn của các đồng nghiệp không chuyên, vì những đồng nghiệp đó đang "vibe coding" (lập trình theo cảm hứng bằng AI).

Những người tự động hóa công việc ngoài chuyên môn của mình thực chất lại đang mang thêm việc cho người khác.

**(2) Ranh giới công việc/cuộc sống bị xóa nhòa**. Giao diện trò chuyện của AI giúp công việc trở nên dễ dàng, không còn cảm giác bất lực trước trang giấy trắng, cũng không có rào cản học tập đáng sợ.

Vì thế, nhân viên bắt đầu gửi các "prompt nhanh" trước khi rời bàn làm việc (ví dụ trước khi đi vệ sinh) để AI xử lý các việc vặt. Nhiều người thậm chí nhập prompt trong thời gian nghỉ ngơi để AI chạy. Việc tích lũy các đầu việc xử lý bằng AI ngoài giờ làm này làm giảm thời gian nghỉ ngơi thực tế và tăng đáng kể giờ làm việc.

**(3) Làm việc đa nhiệm gia tăng**. Vì AI mang lại ảo tưởng rằng các tác vụ có thể chạy ngầm ở chế độ background nên nhân viên bị yêu cầu quản lý nhiều luồng công việc cùng lúc.

Điều này nhìn bề ngoài giúp tăng năng suất, nhưng thực chất lại chuyển thành việc liên tục phân tán sự chú ý và kéo dài danh sách đầu việc cần làm.

**(4) Vòng lặp tự củng cố của các yếu tố trên.** AI giúp mọi việc đơn giản hơn, thế là nhân viên làm nhiều việc hơn, dẫn đến càng phụ thuộc vào AI to simplify those things. Vòng lặp cứ thế tiếp diễn dẫn đến kiệt sức.

Các nhà nghiên cứu chỉ ra: "Một số người tham gia khảo sát cho biết mặc dù cảm thấy hiệu suất công việc cao hơn, nhưng họ không hề thấy thư thả mà ngược lại cảm thấy bận rộn hơn trước."

**(5) Giải pháp**. Nhà nghiên cứu đề xuất để giải quyết tình trạng kiệt sức do AI mang lại, các công ty nên có biện pháp chủ động để quy chuẩn hóa cách nhân viên sử dụng AI:

1. Tạm dừng công việc một lát trước khi đưa ra quyết định quan trọng.
2. Sắp xếp thứ tự công việc để giảm thiểu việc chuyển đổi ngữ cảnh (context switching).
3. Dành thời gian cho giao tiếp thực tế giữa con người với nhau.

## 言论 (Phát ngôn)

1、

> Nếu bạn là mặt trời, tôi chính là hố đen.
> 
> -- [Stephen Hawking](https://geohot.github.io//blog/jekyll/update/2026/05/03/punk-or-why-i-dont-stream.html)

2、

> Thế giới của các mô hình AI giống như một thành phố, trong đó có năm khu vực trụ sở doanh nghiệp lớn và một khu phố Tàu (Chinatown).
> 
> -- [《Kỳ điểm đang ngày càng đến gần hơn》 (The Singularity Is Nearer)](https://geohot.github.io//blog/jekyll/update/2026/05/03/punk-or-why-i-dont-stream.html)

3、

> AI là một chiếc hộp đen hoàn toàn, điều này có nghĩa là cái gọi là "AI engineering" hay "prompt engineering" hoàn toàn là trò lừa bịp. Bất kỳ tuyên bố nào cho rằng có thể thao túng chiếc hộp đen bằng một phương pháp khéo léo nào đó đều là giả tạo.
> 
> Bạn không thể tìm hiểu được logic vận hành của AI, nó chỉ là một kiểu thực thi máy móc mang tính "hãy tin tôi đi, người anh em".
> 
> -- [《AI là một công cụ tồi tệ》](https://bytecode.news/posts/2026/07/user-submission-ai-is-a-bad-tool)

4、

> Tôi có một chiếc máy làm bánh mì, nó tự động lo gần như mọi công đoạn: nhào bột, ủ men, nướng bánh. Tôi đổ nguyên liệu vào, nhấn nút và ba giờ sau là có bánh mì nóng hổi.
> 
> Thế nhưng, trong suốt ba năm qua, tôi chắc chỉ dùng chiếc máy đó đúng hai lần. Thay vào đó, mỗi tuần tôi đều ra siêu thị mua một ổ bánh mì cắt lát sẵn đóng gói.
> 
> Điều này giải thích tại sao ngay cả khi AI có thể dễ dàng tạo ra code, các công ty SaaS vẫn còn lâu mới đi đến chỗ lụi tàn.
> 
> -- [《Tại sao sự tiện lợi luôn thắng cuộc, và tại sao SaaS sẽ không biến mất》](https://www.joanwestenberg.com/p/the-bread-paradox-why-convenience)

## 往年回顾 (Nhìn lại các năm trước)

[Cuộc chơi của stablecoin](https://www.ruanyifeng.com/blog/2025/07/weekly-issue-357.html)（#357）

[Đừng quá coi trọng Product Hunt](https://www.ruanyifeng.com/blog/2024/07/weekly-issue-307.html)（#307）

[Câu chuyện Nvidia của Jensen Huang](https://www.ruanyifeng.com/blog/2023/06/weekly-issue-257.html)（#257）

[Đỉnh cao của ngành công nghiệp ô tô có lẽ đã qua](https://www.ruanyifeng.com/blog/2022/05/weekly-issue-207.html)（#207）

(Hết)
