# Bản tin chia sẻ công nghệ (Số 367): Một vài công dụng thú vị của Nano Banana

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần. (**[Thông báo] Tuần tới nghỉ lễ Quốc khánh (1/10), bản tin sẽ tạm ngưng phát hành.**)

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/7674) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092501.webp)

Hong Kong tổ chức lễ hội "Đại tuần hành trên vịnh Victoria" (Victoria Harbour Maritime Parade), trưng bày bốn bức tượng bơm hơi khổng lồ dọc bờ vịnh. Bức ảnh chụp lại quá trình vận chuyển các bức tượng bơm hơi này. ([via](https://ztylez.com/life/play/2025/09/23/331873/))

## Nano Banana 的几个妙用

Tháng trước, Google đã phát hành mô hình tạo ảnh Gemini 2.5 Flash Image (tên dự án là [Nano Banana](https://aistudio.google.com/models/gemini-2-5-flash-image)).

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091305.webp)

Google tuyên bố đây là "**mô hình sinh và chỉnh sửa hình ảnh tiên tiến nhất**" hiện nay.

Sau khi dùng thử, tôi thấy mô hình này thực sự rất mạnh mẽ, lại còn cho phép sử dụng miễn phí trực tiếp trên [trang web chính thức](https://aistudio.google.com/prompts/new_chat?model=gemini-2.5-flash-image-preview) (như hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092111.webp)

*(Lưu ý: Nếu bạn không truy cập được trang web chính thức, trong phần thảo luận của bản tin cũng có chia sẻ một số [trang web bên thứ ba](https://github.com/search?q=repo%3Aruanyf%2Fweekly+nano+banana&type=issues) kết nối qua API chính thức, tuy nhiên hầu hết các trang này đều thu phí).*

Nhiều cư dân mạng đã phát hiện ra hàng loạt cách ứng dụng thú vị của mô hình này, thậm chí có người còn tổng hợp chúng thành một [kho lưu trữ Awesome](https://github.com/PicoTrex/Awesome-Nano-Banana-images).

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092113.webp)

Tôi đã chọn ra một vài ví dụ rất thiết thực từ kho lưu trữ này để chia sẻ cùng các bạn. Cần lưu ý rằng các mô hình tạo ảnh khác có lẽ cũng làm được những điều tương tự, các bạn có thể tự mình thử nghiệm.

### （1）人像处理

Tác vụ phổ biến nhất của các mô hình tạo ảnh chắc chắn là xử lý ảnh chân dung. Đầu tiên, chúng ta tải lên một bức ảnh đời thường.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091308.webp)

Sau đó, yêu cầu mô hình chuyển đổi nó thành một bức ảnh thẻ chân dung với câu lệnh (prompt) sau:

> Hãy tạo một bức ảnh thẻ chân dung từ người trong ảnh, yêu cầu nền trắng, mặc trang phục công sở lịch sự, mắt mở và mỉm cười.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091309.webp)

Kết quả thật sự rất đáng kinh ngạc. Điều này đồng nghĩa với việc chúng ta có thể thay đổi hoàn toàn biểu cảm, kiểu tóc, cách trang điểm, trang phục và tư thế của nhân vật.

Dưới đây là ví dụ thay đổi biểu cảm nhân vật, yêu cầu nhân vật quay nghiêng mặt và mỉm cười trước ống kính.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091319.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091320.webp)

Thay đổi tư thế của nhân vật: "Hãy đổi tư thế của người trong bức ảnh thứ hai dưới đây giống với tư thế của người trong bức ảnh thứ nhất."

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091316.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091317.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091318.webp)

Các tiệm chụp ảnh truyền thống trong tương lai có lẽ sẽ gặp khó khăn lớn, khi mà ảnh chân dung, ảnh du lịch hay cả ảnh tập thể đều có thể giao cho AI xử lý.

### （2）建筑处理

Một ứng dụng phổ biến khác của mô hình tạo ảnh là thiết kế nội thất. Nếu muốn xem trước phối cảnh trang trí nhà cửa, bạn chỉ cần để AI tự động dựng hình, việc thay đổi tông màu hay đổi mới đồ nội thất đều chỉ là chuyện nhỏ.

Dưới đây là một ví dụ có độ khó cao hơn: tải lên một bản vẽ mặt bằng căn hộ (floor plan) và yêu cầu AI dựng thành bản render mô hình 3D trực quan.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091310.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091311.webp)

Khả năng trích xuất mô hình kiến trúc 3D trực tiếp từ một bức ảnh chụp thực tế cũng vô cùng ấn tượng.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091323.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091324.webp)

### （3）包装处理

Tiếp theo, hãy yêu cầu mô hình thay đổi bao bì của sản phẩm: "Hãy dán hình vẽ nhân vật hoạt hình ở ảnh thứ hai lên hộp bao bì ở ảnh thứ nhất, rồi tạo ra một bức ảnh chụp sản phẩm chuyên nghiệp."

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091313.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091314.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091315.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092112.webp)

Thiết kế bìa sách hay vỏ hộp phần mềm cũng có thể được thực hiện theo cách tương tự.

### （4）地图处理

Một thị trường tiềm năng khác của các mô hình tạo ảnh là ứng dụng bản đồ (thông tin địa lý), tuy nhiên hiện tại vẫn chưa có nhiều mô hình kinh doanh thu phí rõ ràng. Dưới đây là một cách ứng dụng rất sáng tạo:

Tải lên một bản đồ có vẽ mũi tên chỉ hướng tại một địa điểm tùy chọn, rồi yêu cầu mô hình: "Hãy tạo ra khung cảnh nhìn theo hướng của mũi tên màu đỏ."

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092114.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092115.webp)

Nó thậm chí có thể dựa trên bản đồ đường đồng mức địa hình để dựng nên bức ảnh phong cảnh thực tế tại vị trí mũi tên đỏ.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091326.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091327.webp)

## 科技动态

1. [Dao bếp siêu âm](https://seattleultrasonics.com/products/c-200-ultrasonic-8-chefs-knife)

Một công ty của Mỹ đã giới thiệu loại dao làm bếp hoạt động bằng công nghệ siêu âm.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092107.webp)

Trên cán dao được tích hợp một nút bấm, khi nhấn vào, lưỡi dao sẽ chuyển sang chế độ rung siêu âm.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092108.webp)

Theo giới thiệu, khi kích hoạt chế độ siêu âm, lưỡi dao sẽ dao động với tần số hơn 40.000 lần mỗi giây, giúp dao sắc bén hơn rất nhiều so với bình thường và tiết kiệm tới 50% sức lực khi cắt thái.

Trong một số trường hợp, chỉ cần đặt nhẹ dao lên thực phẩm, dao sẽ tự động cắt đứt nhờ vào năng lượng của sóng siêu âm phát ra.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092109.webp)

Sản phẩm này được tích hợp pin bên trong cán dao và đi kèm một bộ sạc chuyên dụng.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092110.webp)

2. [Bo mạch đất sét](https://feministhackerspaces.cargo.site/Clay-PCB-Tutorial)

Bo mạch in (PCB) là nền tảng cốt lõi của mọi sản phẩm điện tử.

Một cư dân mạng nước ngoài, để chứng minh bo mạch không phải là một sản phẩm công nghệ quá xa vời, đã tự tay chế tạo một bo mạch bằng đất sét nung.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091901.webp)

Anh ấy đã chia sẻ toàn bộ ảnh chụp quá trình thực hiện lên mạng: đầu tiên là thu gom bùn đất tự nhiên, sau đó cán mỏng và phẳng.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091902.webp)

Tiếp theo là khắc các đường mạch dẫn điện lên bề mặt rồi đem nung cứng trong lò.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091903.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091904.webp)

Cuối cùng, lắp thêm dây đồng dẫn điện cùng các linh kiện điện tử cơ bản lên bo mạch.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091905.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091906.webp)

3. [Cơ cấu việc làm trong ngành IT](https://www.derekthompson.org/p/the-25-most-interesting-ideas-ive)

Theo báo cáo AI của nhà phân tích nổi tiếng Mary Meeker, nếu loại bỏ các vị trí công việc liên quan đến AI ra khỏi ngành CNTT, số lượng nhân sự có việc làm trong ngành IT tại Mỹ hầu như đi ngang hoặc có xu hướng giảm trong nhiều năm qua.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092303.webp)

Trong biểu đồ trên, đường màu xanh lam biểu diễn tổng số lượng việc làm trong toàn ngành IT, đường màu xanh lá cây đại diện cho số lượng việc làm sau khi đã loại bỏ các vị trí liên quan đến AI, và phần đỉnh nhọn tăng vọt ở giữa trùng vào giai đoạn đại dịch COVID-19.

Điều này cho thấy mặc dù bản thân ngành IT vẫn đang không ngừng mở rộng quy mô, nhưng hầu như toàn bộ phần tăng trưởng việc làm mới đều chỉ tập trung ở lĩnh vực AI.

## 文章

1. [Vượt ra ngoài hộp cát](https://bughunters.google.com/blog/6715529872080896/beyond-sandbox-domains-rendering-untrusted-web-content-with-safecontentframe) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092116.webp)

Làm thế nào để chạy mã nguồn của bên thứ ba một cách an toàn trên trang web? Google đã đề xuất một giải pháp kiến trúc hoàn toàn mới mang tên SafeContentFrame.

Đây là một thư viện JS giúp tải mã nguồn bên thứ ba lên một tên miền riêng biệt (`googleusercontent.com`), rồi dùng `iframe` để nhúng vào trang web hiện tại, từ đó mang lại khả năng cô lập tối đa.

2. [Tại sao các ứng dụng ưu tiên chạy offline (Local-first) vẫn chưa phổ biến?](https://marcobambini.substack.com/p/why-local-first-apps-havent-become) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092301.webp)

Tính năng sử dụng offline vẫn chưa thực sự trở nên phổ biến. Tác giả cho rằng, việc phát triển ứng dụng offline cũng tương tự như xây dựng một hệ thống phân tán phức tạp, phải đối mặt với các bài toán đồng bộ hóa dữ liệu rất khó để giải quyết triệt để.

3. [Elasticsearch không phù hợp để dùng làm cơ sở dữ liệu](https://www.paradedb.com/blog/elasticsearch-was-never-a-database) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092007.webp)

Elasticsearch hiện đang là dịch vụ tìm kiếm phổ biến nhất, liệu có thể sử dụng nó làm cơ sở dữ liệu chính không? Bài viết này chỉ ra lý do tại sao không nên làm vậy, bởi nó vốn không được thiết kế cho mục đích này.

4. [Cách sử dụng Python để chuyển đổi âm thanh thành văn bản](https://www.pavlinbg.com/posts/python-speech-to-text-guide) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092302.webp)

Một bài hướng dẫn đơn giản giúp bạn tự viết kịch bản Python để trích xuất văn bản từ tệp âm thanh bằng mô hình Whisper.

5. [Tránh sử dụng @ts-ignore](https://evanhahn.com/ts-ignore-is-almost-always-the-worst-option/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092406.webp)

Chú thích `@ts-ignore` trong TypeScript được sử dụng để tắt toàn bộ cảnh báo lỗi ở dòng tiếp theo. Tác giả khuyên không nên lạm dụng nó, thay vào đó hãy dùng `@ts-expect-error` hoặc kiểu `any`.

6. [Thuộc tính CSS nội bộ của Apple giúp tạo hiệu ứng "kính lỏng" cho trang web](https://alastair.is/apple-has-a-private-css-property-to-add-liquid-glass-effects-to-web-content/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092010.webp)

Tác giả phát hiện ra Apple đã âm thầm thêm một thuộc tính CSS chưa được công bố vào trình duyệt Safari, giúp các thành phần trên trang web hiển thị hiệu ứng "kính lỏng" độc đáo.

7. [Cách tinh chỉnh systemd giúp tăng tốc độ khởi động](https://www.xda-developers.com/systemd-tweaks-boost-boot-time/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092403.webp)

Một bài hướng dẫn cho người mới bắt đầu với 5 mẹo điều chỉnh cài đặt systemd nhằm rút ngắn thời gian khởi động hệ thống.

## 工具

1. [gpu-kill](https://github.com/kagehq/gpu-kill)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092201.webp)

Công cụ hiển thị thông tin vận hành của GPU, đi kèm bảng điều khiển quản trị web trực quan, hỗ trợ nhiều dòng card đồ họa của Nvidia/AMD/Intel/Apple.

Ngoài ra còn có một trang web kiểm tra hiệu năng GPU trực tuyến mang tên [Volume Shader BM](https://www.volumeshader.dev/). (Đóng góp từ [@BOS1980](https://github.com/ruanyf/weekly/issues/7804))

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092410.webp)

2. [RustNet](https://github.com/domcyrus/rustnet)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092011.webp)

Công cụ dòng lệnh đa nền tảng giúp giám sát lưu lượng mạng và hiển thị chi tiết thông tin các kết nối hiện tại.

3. [PortNote](https://github.com/crocofied/PortNote)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060114.webp)

Bảng điều khiển tự lưu trữ (self-hosted) hiển thị danh sách các cổng cục bộ đang bị chiếm dụng bởi các dịch vụ khác nhau. Khi kết hợp với tệp Compose, nó có thể dùng để khởi chạy hoặc dừng các container Docker. Tham khảo thêm [bài viết giới thiệu](https://www.xda-developers.com/reasons-why-portnote-port-of-call-on-every-server/).

4. [Atlas](https://github.com/karam-ajaj/atlas)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092407.webp)

Một container Docker giúp quét mạng hiện tại và hiển thị trực quan thông tin các nút mạng dưới dạng đồ họa.

5. [Midnight Commander](https://github.com/MidnightCommander/mc)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060107.webp)

Trình quản lý tệp tin dựa trên giao diện dòng lệnh cổ điển, hỗ trợ cả Linux và macOS.

Ngoài ra còn có một trình quản lý tệp tin dòng lệnh tương tự viết bằng Rust là [Yazi](https://github.com/sxyazi/yazi).

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092408.webp)

6. [frp-tunnel-cli](https://github.com/openapphub/frpc-cli)

Kịch bản Bash hỗ trợ cho công cụ chuyển tiếp cổng (intranet penetration) [frp](https://gofrp.org/zh-cn/docs/overview/), giúp đơn giản hóa việc tạo lập và quản lý các đường hầm kết nối. (Đóng góp từ [@openapphub](https://github.com/ruanyf/weekly/issues/7785))

7. [Hamsterbase Tasks](https://github.com/hamsterbase/tasks)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092101.webp)

Phần mềm quản lý tác vụ mã nguồn mở hỗ trợ đa nền tảng Web, điện thoại, máy tính để bàn và có thể triển khai dễ dàng qua Docker. (Đóng góp từ [@CaryTrivett](https://github.com/ruanyf/weekly/issues/7792))

8. [db-back-tool](https://github.com/iKeepLearn/db-back-tool)

Công cụ sao lưu cơ sở dữ liệu PostgreSQL/MySQL do một lập trình viên tự phát triển, hỗ trợ tự động sao lưu, mã hóa, nén dữ liệu và tải tệp tin sao lưu lên dịch vụ đám mây Tencent Cloud COS hoặc Alibaba Cloud OSS. (Đóng góp từ [@iKeepLearn](https://github.com/ruanyf/weekly/issues/7798))

9. [X-CMD](https://github.com/x-cmd/x-cmd)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092412.webp)

Bộ công cụ dòng lệnh đa nền tảng hỗ trợ kích hoạt nhanh hơn 1000 công cụ CLI và tích hợp sẵn các tính năng AI. (Đóng góp từ [@Zhengqbbb](https://github.com/ruanyf/weekly/issues/7806))

## AI 相关

1. [Huxe](https://www.huxe.com/)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092404.webp)

Trợ lý giọng nói cá nhân giúp tạo các bản tin "tóm tắt hàng ngày" dạng podcast để bạn lắng nghe, bao gồm tin tức trong ngày, sở thích cá nhân, lịch trình và email.

Đây là sản phẩm khởi nghiệp đầu tay của đội ngũ phát triển chính đứng sau NotebookLM sau khi rời khỏi Google. Hiện tại dịch vụ đang được cung cấp miễn phí, tham khảo thêm [bài viết giới thiệu](https://www.xda-developers.com/huxe-app-official-launch/).

2. [AIPex](https://github.com/AIPexStudio/AIPex)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091908.webp)

Một tiện ích mở rộng mã nguồn mở dành cho Chrome từng được giới thiệu trước đây, nay đã nâng cấp tính năng hỗ trợ tự động hóa các thao tác trên trình duyệt bằng AI. (Đóng góp từ [@buttercannfly](https://github.com/ruanyf/weekly/issues/7783))

3. [binglish](https://github.com/klemperer/binglish)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092401.webp)

Script Python tự động tải và thay đổi hình nền Bing hàng ngày cho Windows, đồng thời chèn thêm "từ vựng của ngày" kèm giải nghĩa và câu ví dụ do AI tự động tạo ra. (Đóng góp từ [@klemperer](https://github.com/ruanyf/weekly/issues/7800))

4. [index-tts-lora](https://github.com/asr-pub/index-tts-lora)

Mô hình tinh chỉnh (fine-tuned) dựa trên mô hình tổng hợp giọng nói nguồn mở Index-TTS của Bilibili, giúp cải thiện ngữ điệu và độ tự nhiên của giọng nói được tạo ra. (Đóng góp từ [@asr-pub](https://github.com/ruanyf/weekly/issues/7789))

5. [Neovate](https://github.com/neovateai/neovate-code)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092411.webp)

Trợ lý lập trình thông minh chạy ngay trên terminal (Code Agent), có thể coi là một phiên bản mã nguồn mở của Claude Code. (Đóng góp từ [@xierenyuan](https://github.com/ruanyf/weekly/issues/7805))

6. [FlyCut Caption](https://github.com/x007xyz/flycut-caption)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092402.webp)

Công cụ chỉnh sửa phụ đề video bằng AI hoạt động trên trình duyệt web, hỗ trợ nhận dạng giọng nói trong video để tự động tạo phụ đề. Bản thử nghiệm trực tuyến: [Demo](https://caption.flycut.co/en/tool). (Đóng góp từ [@x007xyz](https://github.com/ruanyf/weekly/issues/7801))

7. [mcpstore](https://github.com/whillhill/mcpstore)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092005.webp)

Công cụ quản lý các dịch vụ MCP (Model Context Protocol), giúp kết nối nhiều máy chủ MCP khác nhau thông qua một giao diện web trực quan. (Đóng góp từ [@whillhill](https://github.com/ruanyf/weekly/issues/7790))

## 资源

1. [99 thí nghiệm vật lý nhỏ](https://interactivetextbooks.tudelft.nl/showthephysics/Introduction/About.html)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092003.webp)

Cuốn sách trực tuyến bằng tiếng Anh chọn lọc 99 thí nghiệm vật lý nhỏ trong chương trình trung học của Hà Lan, bao gồm nhiều lĩnh vực (lực, ánh sáng, từ trường, sóng, v.v.).

2. [NPM bảo mật tốt nhất](https://github.com/bodadotsh/npm-security-best-practices)

Trước hàng loạt vụ việc mã độc chèn vào các gói thư viện npm gần đây, kho lưu trữ này tổng hợp các biện pháp bảo mật npm hữu ích dành cho cả người dùng lẫn người phát hành gói thư viện.

## 图片

1. **Nguyên lý xe điện**

Bức ảnh hài hước lan truyền trên mạng giải thích nguyên lý hoạt động của xe điện.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025091907.webp)

2. [Một bài toán hình học](https://samjshah.com/2025/08/05/sangaku-puzzle-i-cant-solve/)

Có một hình vuông chứa một hình tròn nhỏ bên trong. Hãy tìm mối liên hệ giữa bán kính hình tròn nhỏ và chiều dài cạnh hình vuông?

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092001.webp)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092002.webp)

Bài toán này có vẻ không hề đơn giản, và đáp án là bán kính hình tròn bằng 4/33 chiều dài cạnh hình vuông.

## 文摘

1. [Lập trình bằng AI chỉ giải quyết được 70% vấn đề](https://addyo.substack.com/p/the-70-problem-hard-truths-about)

Theo quan sát của tôi, cách lập trình viên cấp cao và lập trình viên cấp thấp sử dụng AI là hoàn toàn khác nhau.

**Lập trình viên cấp cao không hoàn toàn tin tưởng vào kết quả do AI tạo ra, họ chỉ dùng AI để tăng tốc dự án**. Họ thường xem xét kỹ lưỡng và tái cấu trúc (refactor) đoạn mã do AI sinh ra, đồng thời luôn đặt nghi vấn trước các quyết định về cấu trúc hệ thống của AI.

Ngược lại, lập trình viên cấp thấp có xu hướng bỏ qua việc xem xét và tái cấu trúc, chấp nhận toàn bộ mã do AI cung cấp. Điều này dễ dẫn đến những đoạn mã kiểu "lâu đài cát": trông có vẻ hoạt động được nhưng sẽ lập tức đổ vỡ khi đưa vào vận hành thực tế.

Tôi không chắc liệu AI có thay thế lập trình viên trong tương lai hay không, nhưng ở giai đoạn hiện tại, lập trình bằng AI chưa thể giải quyết 100% bài toán phần mềm, mà mới chỉ dừng lại ở mức 70%. Điều này đồng nghĩa với việc **AI có thể giảm bớt 70% khối lượng công việc của một lập trình viên cấp cao**.

30% còn lại vẫn phải phụ thuộc hoàn toàn vào kinh nghiệm và kiến thức chuyên môn của lập trình viên, và đây chính xác là những gì **lập trình viên cấp thấp còn thiếu**.

Vì vậy, dù nghe có vẻ ngược đời: AI thực chất mang lại nhiều lợi ích và dễ tạo ra kết quả công việc tốt hơn cho lập trình viên cấp cao hơn là lập trình viên cấp thấp.

Ở giai đoạn hiện nay, AI giống như một lập trình viên cấp thấp cực kỳ năng nổ trong nhóm, có thể viết mã rất nhanh nhưng cần có sự giám sát và sửa lỗi liên tục từ người có kinh nghiệm. **Bạn càng hiểu biết nhiều, bạn càng có khả năng hướng dẫn và làm chủ nó tốt hơn.**

Do đó, cách sử dụng AI đúng đắn là: lập trình viên cấp cao dùng nó để tăng tốc những việc họ đã biết cách làm, còn lập trình viên cấp thấp dùng nó để học hỏi xem mình nên làm những gì.

## 言论

1.

AI sẽ tiếp tục mở rộng quy mô, cho đến khi phần lớn năng lượng của Mặt Trời được dùng cho hoạt động tính toán.

-- [Bài phỏng vấn mới nhất của Elon Musk](https://t.wangbase.com/0ZKey)

2.

Tôi tin rằng con người có thể tự cung tự cấp trên Sao Hỏa trong vòng 30 năm nữa. Cứ mỗi hai năm, các hành tinh sẽ thẳng hàng và bạn có thể khởi hành đến Sao Hỏa. Vì thế, trong 30 năm tới sẽ có khoảng 10 đến 15 cơ hội phóng tàu.

Mỗi lần khởi hành, khối lượng hàng hóa vận chuyển đến Sao Hỏa sẽ tăng theo cấp số nhân, do đó trong vòng 30 năm, chúng ta hoàn toàn có thể xây dựng một Sao Hỏa tự cung tự cấp.

-- [Bài phỏng vấn mới nhất của Elon Musk](https://t.wangbase.com/0ZKey)

3.

Ngành phần mềm đang âm thầm xuất hiện một công việc mới gọi là "Dọn dẹp Vibe Coding" (Vibe Coding cleanup), chuyên giải quyết các sự cố phát sinh do lập trình tùy hứng bằng AI gây ra. Đây thực sự là điều trớ trêu lớn nhất của thời đại AI: con người được thuê để dọn dẹp đống rác do AI để lại.

-- [《Dịch vụ dọn dẹp Vibe Coding》](https://donado.co/en/articles/2025-09-16-vibe-coding-cleanup-as-a-service/)

4.

Một bong bóng AI hoàn toàn có thể xảy ra, nhưng đối với các công ty như Meta, rủi ro lớn hơn lại là sự do dự.

Nếu cuối cùng chúng tôi lãng phí hàng trăm tỷ USD cho AI, đó rõ ràng là một điều không may, nhưng tôi tin rằng rủi ro của việc bỏ lỡ làn sóng AI còn cao hơn nhiều. Đối với chúng tôi, rủi ro không phải là quá激 tiến, mà là chưa đủ激 tiến.

-- [Mark Zuckerberg](https://finance.sina.cn/7x24/2025-09-19/detail-infqzkhk9726343.d.html)

5.

Máy tính ngày nay đóng vai trò là bên phản hồi (responder): bạn yêu cầu nó làm gì, nó sẽ làm nấy. Giai đoạn tiếp theo của máy tính sẽ là "agent" (tác nhân), nó giống như một người tí hon nằm trong hộp bắt đầu dự đoán những gì bạn muốn. Nó không chỉ đơn thuần là giúp đỡ, mà sẽ dẫn dắt bạn xử lý một lượng thông tin khổng lồ, giống như việc bạn có một người bạn đồng hành nhỏ bé bên trong chiếc hộp vậy.

-- [Steve Jobs](https://simonwillison.net/2025/Sep/18/steve-jobs/), bài phỏng vấn năm 1984

## 往年回顾

[Bàn bóng bàn kiêm giường ngủ](https://www.ruanyifeng.com/blog/2024/10/weekly-issue-320.html) (#320)

["Phát triển tinh gọn" (Lean Development) thực chất là gì?](https://www.ruanyifeng.com/blog/2023/09/weekly-issue-270.html) (#270)

[Cơ hội của trí tuệ nhân tạo nằm ở đâu](https://www.ruanyifeng.com/blog/2022/08/weekly-issue-220.html) (#220)

[Chiến thắng của mô hình phần mềm trả phí định kỳ (Subscription)](https://www.ruanyifeng.com/blog/2021/08/weekly-issue-170.html) (#170)

(Hết)
