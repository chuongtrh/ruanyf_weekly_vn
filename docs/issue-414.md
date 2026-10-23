# Bản tin công nghệ hàng tuần (Số 414): Mô hình quyết định Jev có tác dụng gì

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/12009) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100816.webp)

Đoàn tàu điện ngầm kỹ thuật số nội địa đầu tiên VELLINK của Trung Quốc, vận hành hoàn toàn không người lái, phần đầu tàu được thiết kế thành mảng kính lớn phục vụ ngắm cảnh. ([via](https://jl.chinadaily.com.cn/a/202609/23/WS6ab3be35e4b09a165c78c53d.html))

## Jev 决策模型有什么用

Tháng trước, tin tức AI chấn động nhất không phải là các bản cập nhật mới của GPT hay Claude, mà là việc một công ty chưa mấy tên tuổi [TypeSafe AI](https://typesafe.ai/) đã công bố một lớp mô hình hoàn toàn mới mang tên [Jev](https://typesafe.ai/blog/introducing-system-one-models-and-jev).

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100817.webp)

Mô hình mới này khác biệt một trời một vực so với các mô hình trước đây, được định danh là "mô hình quyết định" (decision model).

Đọc xong tôi cảm thấy thật khó tin: một thứ hữu ích đến thế và về mặt ý niệm lại đơn giản đến vậy, tại sao trước đây chưa từng có ai nghĩ ra?

Đặc điểm lớn nhất của mô hình Jev là: trong khi các mô hình khác trả về câu chữ văn bản, **nó lại trả về một số thực dấu phẩy động (float) biểu thị xác suất**.

Tại sao trả về xác suất lại hữu dụng? Bởi vì chúng ta có thể dùng nó để xử lý dạng câu hỏi "đúng/sai" (True/False). Bạn hỏi nó: "Câu khẳng định 'Ngày mai trời mưa' đúng hay sai?". Nếu nó trả về 0, nghĩa là xác suất đúng bằng 0, tức ngày mai chắc chắn không mưa; nếu trả về 0.99, nghĩa là có 99% khả năng câu này đúng, tức ngày mai gần như chắc chắn sẽ mưa.

Bên cạnh câu hỏi đúng/sai, nó còn xử lý được dạng "câu hỏi trắc nghiệm nhiều lựa chọn". Bạn đưa cho nó 4 phương án A, B, C, D, nó sẽ trả về xác suất chính xác của từng phương án, từ đó bạn biết ngay phương án nào có khả năng đúng cao nhất.

Cuối cùng, nó sở hữu một tính năng thần kỳ gọi là "chấm điểm" (score). Bạn cung cấp cho nó một bộ tiêu chí chấm điểm, rồi đưa cho nó một đoạn tài liệu gốc, nó sẽ dựa trên bộ tiêu chí đó để cho điểm tài liệu.

Dưới đây tôi xin giới thiệu hai ví dụ thực tế dưới dạng extension trình duyệt sử dụng mô hình Jev, bạn sẽ thấy mô hình này hữu ích đến nhường nào:

Ví dụ thứ nhất là bài viết [《Tôi dùng Ctrl + F để tìm kiếm câu trả lời》](https://blog.tymscar.com/posts/hunchsemanticfind/).

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100818.webp)

Mọi người đều biết Ctrl + F là phím tắt tìm kiếm trong trình duyệt để tìm xem một từ hoặc câu xuất hiện ở đâu.

Thế nhưng tác giả đã biến phím tắt này thành "tìm kiếm theo ngữ nghĩa". Ví dụ trên một trang tiểu sử nhân vật, bạn bấm Ctrl + F rồi gõ "thời niên thiếu", công cụ không tìm chính xác cụm từ đó, mà tìm đúng đoạn văn miêu tả những trải nghiệm lúc nhỏ của nhân vật.

Nguyên lý thực hiện rất đơn giản: lấy lần lượt từng đoạn văn trong bài viết rồi gửi câu hỏi cho Jev: "Đoạn văn này có liên quan đến từ khóa tìm kiếm của người dùng hay không?" (câu hỏi đúng/sai). Jev sẽ trả về một xác suất liên quan, và những đoạn văn có xác suất cao nhất chính là kết quả tìm kiếm ngữ nghĩa mà người dùng cần.

Ví dụ thứ hai là [《Tôi dùng Jev để chấm điểm trang web》](https://pub.towardsai.net/build-a-browser-extension-with-jev-22e026255cb7).

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100819.webp)

Tác giả đưa ra một bộ tiêu chí xếp hạng từ thấp đến cao:

> - Luận điểm thiếu căn cứ xác thực, hoặc thuần túy chắp vá từ ngữ hoa mỹ.
> - Lý lẽ thưa thớt, hoặc lập luận lỏng lẻo, sa đà vào khoa trương tu từ.
> - Lý lẽ rõ ràng, cấu trúc logic mạch lạc.
> - Lập luận chặt chẽ, có bằng chứng thực tế vững chắc hậu thuẫn, và có phản biện các góc nhìn trái chiều.

Anh để Jev tự động chấm điểm cho mỗi trang web mới mở dựa trên bộ tiêu chí này. Nhờ đó, chưa cần đọc nội dung trang web, anh đã biết ngay chất lượng bài viết ra sao.

Hai bài viết trên đều có đính kèm mã nguồn đầy đủ để các bạn tham khảo. Đọc xong bạn sẽ hiểu ra một điều cốt lõi: **một khi mô hình AI trả về kết quả được định lượng dạng số, vô số bài toán trước đây không thể xử lý bằng thuật toán số hóa bỗng chốc đều có thể lập trình xử lý được bằng máy tính**.

Tôi cũng rất khuyến khích các bạn đọc [bài giới thiệu Jev của Simon Willison](https://simonwillison.net/2026/Sep/21/jev/).

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100820.webp)

Nhận xét của ông vô cùng sâu sắc và trúng đích: "Jev thực chất đại diện cho một bước thụt lùi của các hệ thống học máy, quay trở lại hệ thống hộp đen hoàn toàn. Các mô hình lớn trước đây dù không đảm bảo luôn đúng, nhưng ít nhất bạn có thể yêu cầu chúng giải thích lý do đằng sau quyết định của mình. Jev thậm chí tước bỏ luôn cả điều đó: bạn chỉ nhận về một con số thực duy nhất, còn con số đó từ đâu mà ra thì hoàn toàn chịu chết."

Ông bày tỏ lo ngại sâu sắc rằng người ta sẽ dùng Jev để xếp hạng ứng viên xin việc.

Với sự xuất hiện của Jev, các công ty sàng lọc hồ sơ CV và chọn người phỏng vấn trở nên dễ dàng hơn bao giờ hết, quy trình đánh giá phức tạp của con người bị rút gọn thành một bài toán chấm điểm số học vô cảm.

## Markdown 正在变成源码

Trước đây định dạng Markdown thuần túy chỉ dùng để soạn thảo tài liệu. Gần đây tôi đọc được một bài viết đưa ra một nhận định rất táo bạo: [Markdown đang dần biến thành mã nguồn](https://htmx.org/essays/markdown-in-src/).

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100821.webp)

Lập luận của tác giả nghe rất thuyết phục:

（1）Markdown là văn bản thuần (plain text), việc so sánh diff, tìm kiếm và review đều vô cùng dễ dàng.

（2）AI đọc và viết Markdown tự nhiên như ngôn ngữ mẹ đẻ.

（3）Con người không cần công cụ hỗ trợ phức tạp vẫn có thể trực tiếp đọc và chỉnh sửa Markdown.

Một khi mã nguồn phần mềm do AI tạo ra dựa trên các câu lệnh prompt viết bằng Markdown, thì chính các file Markdown prompt đó nên được commit trực tiếp vào thư mục `/src` song song cùng với mã nguồn sinh ra.

Trên thực tế, Markdown dưới dạng các tệp cấu hình như `AGENTS.md` đã chính thức trở thành một phần cấu thành của mã nguồn dự án.

Từ nay về sau, chúng ta buộc phải tập làm quen với một sự thật: tài liệu Markdown cũng chính là mã nguồn.

## 不能摄像的摄像头

Có thông tin rò rỉ rằng Apple sắp sửa trình làng một mẫu [camera nhà thông minh](https://www.theapplepost.com/2026/10/01/72882/apples-smart-home-camera-reportedly-wont-record-video/).

Điểm kỳ lạ nhất của sản phẩm này là: tuy mang danh là camera, nhưng nó tuyệt đối không thể ghi hình video.

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100512.webp)

Bạn có hình dung nổi không: camera mà không thể quay phim, thế thì sao gọi là camera được nữa?

Thiết bị hoàn toàn dựa vào AI để phân tích môi trường xung quanh và báo cáo những gì nó nhận biết được. Ví dụ: khi có người lạ gõ cửa, các camera thông thường sẽ cung cấp đoạn video hình ảnh, còn chiếc camera này chỉ gửi cho bạn một đoạn văn bản miêu tả chi tiết bằng chữ!

Mặc dù xử lý bằng chữ tiện lợi và bảo vệ quyền riêng tư hơn, nhưng trong rất nhiều trường hợp con người thực sự cần bằng chứng video ghi lại (như đột nhập trộm cắp, mất cắp bưu kiện...), không rõ Apple sẽ giải quyết các tình huống này như thế nào.

## RSA 因数分解的新纪录

RSA là thuật toán mã hóa khóa công khai phổ biến bậc nhất. Nếu nó bị bẻ khóa, bí mật của vô số phần mềm trên thế giới sẽ lập tức bị phơi bày hoàn toàn.

Độ khó bẻ khóa của RSA hoàn toàn phụ thuộc vào việc khóa công khai có thể bị phân tích thành tích của các thừa số nguyên tố hay không. Độ dài bit mã hóa càng lớn thì càng khó phá; kỷ lục bẻ khóa RSA trước đây từng đạt mốc 768-bit.

Vào ngày 20 tháng 9 năm nay, một kỹ sư phần mềm tại Anthropic [tuyên bố](https://saweis.net/posts/rsa-896.html) anh đã bẻ khóa thành công khóa RSA 896-bit dưới sự trợ giúp của mô hình Claude.

Dưới đây là hình ảnh khóa mã hóa bị bẻ khóa cùng hai thừa số nguyên tố sau khi phân tích:

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026092002.webp)

Theo [chia sẻ](https://nitter.netbub.com/sweis/status/2101484464807596264) của anh, anh đã dùng Claude để port thư viện thuật toán phân tích thừa số nguyên tố CADO-NFS sang chạy trên GPU, rồi cho chạy trên cụm 2.048 GPU trong 10 ngày liên tục là cho ra kết quả.

Bài học rút ra từ sự kiện này là: ngay cả một cá nhân đơn lẻ giờ đây cũng có thể huy động tài nguyên để bẻ khóa những độ dài khóa phức tạp đến vậy, thì các tổ chức tình báo và tập đoàn khổng lồ có thể phá được khóa bao nhiêu bit? Thật không dám tưởng tượng nổi!

Vì vậy hiện nay các chuyên gia đều khuyến cáo: độ dài khóa RSA tối thiểu phải đạt từ 2048-bit trở lên mới tạm coi là an toàn.

## 文章

1. [Xu hướng công nghệ JavaScript mới nhất năm 2026](https://blog.master.dev/what-to-know-in-javascript-2026-edition/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026092401.webp)

Bài viết của Chris Coyier, nhà sáng lập CodePen và CSS-Tricks, điểm lại toàn cảnh các bước tiến mới nhất của hệ sinh thái JS (cú pháp, runtime, framework, tooling...), rất đáng đọc.

2. [Tại sao tôi từ bỏ Deno quay về với Node.js](https://dbushell.com/2026/10/03/deno-to-node/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100518.webp)

Tác giả bày tỏ sự thất vọng với Deno, cho rằng dự án này đã thất bại, ngược lại Node.js thời gian gần đây lại ngày càng trở nên hoàn thiện và dễ dùng hơn.

3. [Câu chuyện đằng sau sự thay đổi của trang example.com](https://www.oliverdunk.com/2026/09/30/iana-reply) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100513.webp)

[example.com](https://example.com/) là trang web ví dụ kinh điển của Internet, chỉ có duy nhất một trang và bao năm qua hầu như không đổi khác.
Thế nhưng gần đây trang web này bất ngờ có sự thay đổi. Bài viết hé lộ ai là người đứng sau trang web này và vì sao họ lại quyết định thay đổi nó.

4. [Cuộc đua AI bỗng trở nên ngượng ngùng](https://insufferable.dev/posts/the-ai-race-just-got-awkward/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100815.webp)

Tác giả bài viết nhận định việc Opus 5.5 và GPT 6.1 Sol đồng loạt giảm giá gần đây hoàn toàn là do các công ty này đã âm thầm áp dụng các thành quả mã nguồn mở của DeepSeek.

5. [Kích thước số nguyên linh hoạt trong C không phải sai lầm thiết kế](https://pikuma.com/blog/c-integer-sizes-not-a-mistake) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026093001.webp)

Bài viết phổ biến kiến thức C, giải thích tại sao kích thước byte của các kiểu dữ liệu trong C lại có thể biến đổi linh hoạt (ví dụ kiểu `int` có thể là 4 byte hoặc 2 byte tùy kiến trúc phần cứng).

6. [Cách làm một mã QR tự động điều hướng đúng hai kho ứng dụng](https://matthuggins.com/blog/posts/qr-codes-that-route-to-the-appropriate-app-store) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026093002.webp)

Tác giả thiết kế một tấm card giấy chỉ có chỗ in một mã QR duy nhất. Anh chia sẻ cách cấu hình server backend để nhận biết điện thoại quét là iPhone hay Android, từ đó tự động chuyển hướng về App Store hoặc Google Play tương ứng.

## 工具

1. [Crafting Apps](https://getartcraft.com/apps)

Có người đã nhờ AI dùng ngôn ngữ Rust để viết lại toàn bộ bộ phần mềm Adobe Creative Cloud. Cả 7 sản phẩm chủ lực của Adobe đều có phiên bản viết lại bằng Rust tương ứng và hoàn toàn là mã nguồn mở!

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100810.webp)

Trong đó [PhotoCraft](https://github.com/storytold/photocraft) có giao diện giống hệt Photoshop.

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100811.webp)

Tôi thấy có bình luận dí dỏm: kết cục của việc này một là Adobe phá sản, hai là nước Mỹ phải sửa lại luật bản quyền.

2. [Pass Designer](https://developer.apple.com/pass-designer/)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100508.webp)

Công cụ chính thức của Apple hỗ trợ thiết kế giao diện thẻ điện tử cho Apple Wallet.

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100509.webp)

3. [tui-dashboard](https://github.com/lyuangg/tui-dashboard)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091901.webp)

Bảng điều khiển terminal có thể tùy biến bố cục và nội dung hiển thị thông qua cấu hình. (Đóng góp từ [@lyuangg](https://github.com/ruanyf/weekly/issues/11718))

4. [yovoice](https://github.com/leemysw/yovoice)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091903.webp)

Công cụ lồng tiếng TTS cục bộ trên máy tính, hỗ trợ clone giọng nói và tinh chỉnh cảm xúc, toàn bộ quá trình tổng hợp giọng nói diễn ra offline. (Đóng góp từ [@leemysw](https://github.com/ruanyf/weekly/issues/11764))

5. [sh.cd](https://github.com/CleanIP/sh.cd)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091905.webp)

Script kiểm tra sức khỏe máy chủ: phần cứng, hiệu năng CPU, chất lượng IP và tốc độ mạng. (Đóng góp từ [@gentpan](https://github.com/ruanyf/weekly/issues/11781))

6. [AirStats](https://github.com/byrencheema/airstats)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026092601.webp)

Ứng dụng theo dõi thông số tài nguyên hệ thống gọn nhẹ nằm trên thanh Menu Bar của macOS. (Đóng góp từ [@byrencheema](https://github.com/ruanyf/weekly/issues/11877))

7. [Video Transcript](https://github.com/anghunk/video-transcript)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026092602.webp)

Web app nhận diện giọng nói trong video và tự động tạo phụ đề. Sử dụng mô hình chạy cục bộ, video và phụ đề không bị tải lên máy chủ ngoài. (Đóng góp từ [@anghunk](https://github.com/ruanyf/weekly/issues/11881))
Ngoài ra còn có ứng dụng tương tự [OpenSubs](https://github.com/open-subs/opensubs). (Đóng góp từ [@open-subs](https://github.com/ruanyf/weekly/issues/11895))

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026092603.webp)

8. [PecoFence](https://github.com/DayuanJiang/PecoFence)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026092604.webp)

Công cụ sắp xếp icon màn hình desktop Windows 11 mã nguồn mở miễn phí, gom gọn các shortcut, tệp và thư mục vào từng ô rào ngăn nắp. (Đóng góp từ [@DayuanJiang](https://github.com/ruanyf/weekly/issues/11887))

9. [skillsgist](https://github.com/Qsnh/skillsgist)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026092605.webp)

Kho lưu trữ Skill riêng tư chạy trên Cloudflare Workers, tải Skill cần nhập mật khẩu, thích hợp cho chia sẻ nội bộ nhóm nhỏ. (Đóng góp từ [@Qsnh](https://github.com/ruanyf/weekly/issues/11897))

10. [Pebrel](https://github.com/Kuddev/pebrel)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026092606.webp)

Trình giả lập terminal đa nền tảng, hoạt động mượt mà trên Windows (tên cũ là Nebula). (Đóng góp từ [@Kuddev](https://github.com/ruanyf/weekly/issues/11909))

11. [WallpaperMachine](https://github.com/WallpaperMachine/WallpaperMachine)

Ứng dụng hình nền động mã nguồn mở cho macOS, cho phép chạy trực tiếp các hình nền từ Wallpaper Engine trên máy Mac. (Đóng góp từ [@fzlzjerry](https://github.com/ruanyf/weekly/issues/11935))

12. [LiteZip](https://github.com/gentpan/LiteZip)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100602.webp)

Công cụ nén và giải nén miễn phí cho macOS, gom các thao tác đóng gói, mã hóa, chia nhỏ file và duyệt file nén vào chung một cửa sổ duy nhất. (Đóng góp từ [@gentpan](https://github.com/ruanyf/weekly/issues/12025))

13. [Burrow](https://github.com/ArkGravity/burrow)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100603.webp)

Dịch vụ đăng nhập một lần (SSO) OIDC gọn nhẹ cho team nhỏ tự lưu trữ, tích hợp xác thực qua OpenID Connect. (Đóng góp từ [@logic3579](https://github.com/ruanyf/weekly/issues/12039))

14. [atv-core](https://github.com/corvofeng/atv-core)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100604.webp)

Cho phép remote Apple TV mặc định trong Control Center của iPhone điều khiển trực tiếp Android TV và Mac mà không cần cài thêm app hay mua Apple TV thật. (Đóng góp từ [@corvofeng](https://github.com/ruanyf/weekly/issues/12051))

15. [open-compute](https://github.com/elliothux/open-compute)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100807.webp)

Nền tảng tương thích mã nguồn mở cho Cloudflare Workers, giúp chạy các tập lệnh worker trực tiếp trên máy chủ riêng mà không cần sửa đổi mã nguồn. (Đóng góp từ [@elliothux](https://github.com/ruanyf/weekly/issues/12062))

16. [Snitch](https://github.com/aixisstudio/Snitch)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100808.webp)

Công cụ trực quan hóa lưu lượng mạng thời gian thực, xem rõ từng kết nối mà máy tính bạn thiết lập: chương trình nào đang giao tiếp với máy chủ nào. (Đóng góp từ [@aixisstudio](https://github.com/ruanyf/weekly/issues/12063))

17. [EdgeChat](https://github.com/aozorae/Edgechat)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100809.webp)

Hệ thống chat tự triển khai mã nguồn mở trên nền Cloudflare, hỗ trợ chat nhóm và tin nhắn riêng, có thể đồng bộ tin nhắn hai chiều với nhóm Telegram. (Đóng góp từ [@aozorae](https://github.com/ruanyf/weekly/issues/12081))

18. [DockTerm](https://github.com/munvard/dockterm)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100601.webp)

Cho phép thông báo cấp quyền của Claude Code bật ra ngay từ phần notch của màn hình Mac, thuận tiện cho việc chạy tác vụ ngầm. (Đóng góp từ [@munvard](https://github.com/ruanyf/weekly/issues/12024))

## 资源

1. [Naive Icons](https://github.com/guokaigdg/naive-icons)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091902.webp)

Bộ icon SVG phong cách vẽ tay ngộ nghĩnh dành cho React. (Đóng góp từ [@guokaigdg](https://github.com/ruanyf/weekly/issues/11740))

2. [Duyệt Cổ Văn](https://yueguwen.com/)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026092001.webp)

Website đọc sách cổ chữ Hán miễn phí, ngoài các chú giải truyền thống còn hỗ trợ bôi đen văn bản để AI giải nghĩa sâu. (Đóng góp từ [@monsoonw](https://github.com/ruanyf/weekly/issues/11824))

3. [Tour dạo bước qua lịch sử nghệ thuật](https://artmuseum.artfrompixels.com/)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100812.webp)

Website biến các bức danh họa trên Wikipedia thành một phòng trưng bày 3D phân loại theo trường phái nghệ thuật, cho phép người dùng dạo bước tham quan.

4. [stillwet](https://stillwet.art/)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100510.webp)

Website trưng bày các bức tranh sơn dầu do AI tạo ra, mô phỏng chân thực từng nét cọ vẽ sơn dầu của con người, sống động đến mức không thể nhận ra đây là tác phẩm của máy tính.

## 图片

1. [Xe điện bánh sắt cổ ở San Francisco](https://daniel.lawrence.lu/blog/2026-09-20-muni-heritage-weekend/)

San Francisco sở hữu nhiều tuyến xe điện bánh sắt cổ kính vẫn được duy trì lăn bánh phục vụ du khách.

Các đoàn tàu chạy dọc theo bờ biển Thái Bình Dương tạo nên khung cảnh tuyệt đẹp. Dưới đây là những bức ảnh chụp trong năm nay:

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026093013.webp)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026093014.webp)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026093015.webp)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026093016.webp)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026093017.webp)

2. [Tỷ suất lợi nhuận của các tập đoàn khổng lồ](https://www.visualcapitalist.com/ranked-how-profitable-are-the-worlds-largest-companies/)

Biểu đồ dưới đây thống kê từ báo cáo tài chính thường niên của các tập đoàn lớn nhất thế giới, thể hiện trên mỗi 100 USD doanh thu thì thu về bao nhiêu USD lợi nhuận:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100516.webp)

Có thể thấy các tập đoàn công nghệ IT nói chung đều có biên lợi nhuận cực cao: đứng đầu là NVIDIA với mỗi 100 USD doanh thu mang về tới 55,6 USD lợi nhuận; tiếp theo là Microsoft (36,1 USD) và Google (32,8 USD).

Apple đứng thứ 5 với 26,9 USD lợi nhuận. Tuy nhiên Apple là công ty phần cứng, việc một hãng sản xuất thiết bị trong ngành công nghệ có tốc độ đào thải chóng mặt duy trì được biên lợi nhuận như vậy thực sự càng đáng kinh ngạc hơn.

## 言论

1.

Gửi các AI Agent: Vui lòng đi chỗ khác mà cày điểm benchmark, chẳng có lý do gì để hack vào hệ thống của chúng tôi cả.

-- [File security.txt của Hugging Face](https://archive.is/1BDwZ)

2.

Thu nhập của tôi chủ yếu đến từ việc bán sách; năm 2024 nó vẫn đủ trang trải cuộc sống cho tôi, nhưng đến năm 2026 thì con số này đã về bằng không.
Blog và các cuốn sách của tôi đều được mở đọc miễn phí online, lượng truy cập tăng vọt ngoài tầm kiểm soát của tôi. Thế nhưng gần như toàn bộ lượng truy cập đó đều đến từ bot cào dữ liệu AI, nên tôi chẳng thu được một đồng doanh thu quảng cáo nào.
Vì vậy tôi quyết định tạm đóng cửa blog và gỡ bỏ toàn bộ sách online để suy nghĩ xem bước tiếp theo nên làm gì.

-- [Axel Rauschmayer](https://molily.de/web-dev-education/), tác giả viết sách công nghệ nổi tiếng, giải thích lý do đóng cửa website cá nhân

3.

Tôi thấy trợ lý cá nhân AI thực ra không mấy hữu dụng. Một năm tôi chỉ đặt đồ ăn ngoài khoảng năm lần nên chẳng cần nó làm hộ; bình thường tôi cũng ít nhận email, việc tự sắp xếp lịch trình cá nhân cũng rất nhanh gọn.
Thứ mà tôi thực sự thấy nó phát huy hiệu quả tuyệt vời là khả năng tự động thu thập và xử lý khối lượng dữ liệu khổng lồ trên mạng: nó có thể quét nhanh 1.000 kênh YouTube để lọc ra những video khớp với sở thích của tôi.

-- [《Mô hình Muse của Meta cực kỳ thích hợp cho web scraping》](https://sigh.dev/posts/metas-muse-is-fantastic-for-web-scraping/)

4.

Gần như tất cả mọi người đều đang phóng đại mối đe dọa từ các mô hình AI Trung Quốc đối với các công ty mô hình của Mỹ; thực chất đó chỉ là hệ quả từ việc nguồn cung mô hình của Mỹ không đáp ứng đủ nhu cầu thị trường mà thôi.

-- [stratechery.com](https://stratechery.com/2026/frontier-overhangs/)

5.

Một nghệ sĩ mắc bệnh ung thư giai đoạn cuối sắp sửa qua đời. Một người dẫn chương trình thường phỏng vấn ông đã hỏi: "Lúc này đây ông có chiêm nghiệm mới nào về sự sống và cái chết không?"
Ông mỉm cười đáp: "Bạn biết không, ăn một chiếc bánh sandwich thực sự là một điều vô cùng hạnh phúc."
Giờ đây tôi cảm thấy cuộc sống quý giá hơn bao giờ hết, luôn nhắc nhở bản thân phải trân trọng từng chiếc sandwich, từng phút giây trôi qua, và tất cả mọi điều bình dị xung quanh.

-- [《Hãy thưởng thức trọn vẹn từng chiếc sandwich》](https://bradmontague.substack.com/p/enjoy-every-sandwich)

## 往年回顾

[Vài mẹo nhỏ hữu ích với Nano Banana](https://www.ruanyifeng.com/blog/2025/09/weekly-issue-367.html) (#367)

[Ngụ ngôn về lừa, hổ và sư tử](https://www.ruanyifeng.com/blog/2024/09/weekly-issue-317.html) (#317)

[Mùa xuân của 5G sắp đến](https://www.ruanyifeng.com/blog/2023/08/weekly-issue-267.html) (#267)

[Thành phố tương lai Neom của Ả Rập Xê Út](https://www.ruanyifeng.com/blog/2022/08/weekly-issue-217.html) (#217)

(Hết)
