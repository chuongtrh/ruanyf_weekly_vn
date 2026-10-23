# Bản tin công nghệ hàng tuần (Số 412): Cấm issue, chỉ nhận PR

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/11434) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090901.webp)

Triển lãm "Kỷ niệm 15 năm Liên Minh Huyền Thoại" tổ chức tại Taikoo Li Tiền Than, Thượng Hải. ([via](https://weibo.com/5720474518/RgUnYmL0t))

## 禁止 issue，只用 PR

Tuần trước, framework PHP nổi tiếng Laravel đã ban hành [một quy định mới](https://x.com/taylorotwell/status/2095516796748996843): cấm mở issue, chỉ cho phép gửi Pull Request.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091017.webp)

Thoạt nhìn, quy định này có vẻ quá mức vô lý. Người dùng không được tạo issue thì báo cáo lỗi kiểu gì? Chẳng lẽ bắt ai cũng phải đọc hiểu mã nguồn rồi tự tay sửa lỗi hay sao!

Thế nhưng suy nghĩ kỹ lại, bạn sẽ thấy biện pháp này [rất hợp lý](https://stitcher.io/blog/no-more-issues), thậm chí rất đáng được nhân rộng:

（1）Triệt tiêu hoàn toàn issue rác.
Nếu một người dùng sẵn lòng bỏ thời gian tạo PR, điều đó chứng tỏ họ thực sự quan tâm đến vấn đề. Những con bot hay những kẻ quấy rối chỉ biết mở issue rác chứ tuyệt đối không bao giờ chịu bỏ công sức đóng góp cho dự án.

（2）Thuận tiện hơn cho người bảo trì dự án (maintainer).
Lượng thông tin mà maintainer nhận được từ PR nhiều hơn hẳn so với một issue mơ hồ, giúp họ dễ hiểu bản chất vấn đề và giải quyết nhanh hơn, tốn ít thời gian công sức hơn.

（3）Không làm tăng độ khó đóng góp của người dùng.
Người dùng ngay cả khi không hiểu mã nguồn vẫn có thể tạo PR. Họ có thể mô tả bài toán cho AI để AI tự viết mã tạo PR. Trong kỷ nguyên AI, việc tạo một PR thực ra cũng đơn giản chẳng kém gì việc mở một issue.

（4）Nguyên nhân gốc rễ của việc cấm issue là các dự án nguồn mở luôn thiếu thốn nguồn lực bảo trì, không thể kham nổi lượng issue bùng nổ quá nhanh.
Trong thời đại AI, dự án không nên khuyến khích người dùng chỉ việc ném vấn đề ra đó rồi khoanh tay chờ người khác giải quyết giúp, mà nên khuyến khích mọi người cùng bắt tay đóng góp sức mình cho dự án.

## 史上最长的数学程序

Tuần trước, công ty Anthropic sử dụng mô hình Claude AI đã hoàn thành chương trình toán học dài nhất trong lịch sử nhân loại: chứng minh định lý lớn Fermat bằng mã lập trình hình thức.

Vào thế kỷ 17, nhà toán học người Pháp Pierre de Fermat đã đưa ra một giả thuyết trứ danh: không tồn tại các số nguyên dương $x, y, z$ thỏa mãn phương trình dưới đây khi số mũ lớn hơn 2.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090502.webp)

Các thế hệ nhà toán học đời sau nhận thấy giả thuyết này hóc búa ngoài sức tưởng tượng, gần như không thể chứng minh. Mãi hơn 300 năm sau, vào năm 1995, nhà toán học người Anh Andrew Wiles mới hoàn thành bản chứng minh khẳng định định lý lớn Fermat là hoàn toàn chính xác.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090503.webp)

Bản chứng minh của Andrew Wiles dài tới 129 trang, ngay cả những nhà toán học chuyên nghiệp cũng phải mất nhiều tháng mới đọc hiểu tường tận.

Kể từ khi bản chứng minh ra đời, giới toán học luôn khao khát dịch nó sang ngôn ngữ máy tính nhằm thực hiện chứng minh bằng máy (machine-checked proof), từ đó tự động hóa việc xác minh toàn bộ quá trình suy luận logic.

Dự án dịch từ chứng minh thủ công của con người sang chứng minh bằng máy này cũng khó khăn và có khối lượng công việc khổng lồ, bao năm qua vẫn dang dở. Cho đến tuần trước, một nhóm nghiên cứu công bố [Claude AI](https://www.anthropic.com/research/formalizing-fermats-last-theorem) sau 11 ngày miệt mài cuối cùng đã hoàn tất: chuyển toàn bộ bản chứng minh của Andrew Wiles thành chương trình viết bằng ngôn ngữ Lean.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090504.webp)

Ngôn ngữ Lean do Microsoft Research giới thiệu năm 2013, là ngôn ngữ lập trình chuyên dụng phục vụ việc chứng minh các định lý toán học hình thức.

Ban đầu các nhà nghiên cứu chỉ muốn thử nghiệm năng lực nghiên cứu toán học của Claude AI, không ngờ nó thực sự giải quyết trọn vẹn dự án siêu khó mà trước nay chưa ai làm nổi.

Trước khi đi đến kết quả chứng minh cuối cùng, Claude đã tự chứng minh hơn 30.000 định lý bổ trợ (lemma), sử dụng hơn 29.000 định lý trong số đó, tiêu tốn hàng tỷ token, và tạo ra lượng mã nguồn cuối cùng dài tới 13 triệu dòng code!

Đây là chương trình toán học dài nhất từng được tạo ra trong lịch sử; thật khó tưởng tượng nếu để một nhóm các nhà toán học con người tự viết thì sẽ mất bao nhiêu năm tháng? Toàn bộ mã nguồn hiện đã được công khai trên [GitHub](https://github.com/anthropics/fermats-last-theorem).

Ý nghĩa sâu sắc của sự kiện này là: hiện nay có vô số bản chứng minh toán học phức tạp mà con người chưa thể thẩm định tính đúng đắn, ngay cả các chuyên gia cũng mất rất nhiều thời gian mới đọc hiểu. Giờ đây thực tế đã chứng minh AI hoàn toàn có thể đảm đương trọng trách thẩm định tính chính xác của các công trình toán học này.

Cuối cùng, xin gửi tới các bạn một [bài phỏng vấn Andrew Wiles](https://www.pbs.org/wgbh/nova/proof/wiles.html) kể về hành trình cuộc đời ông.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026080302.webp)

Người phỏng vấn hỏi ông: "Ông đã dày công theo đuổi định lý Fermat suốt bao nhiêu năm ròng. Giờ đây cuộc hành trình đã khép lại, chắc hẳn ông sẽ cảm thấy có chút bùi ngùi tiếc nuối?"

Andrew Wiles trả lời rằng cảm giác giống như vừa bước ra khỏi một trận đại chiến, cảm thấy được giải thoát hoàn toàn:

> "Quả thực có chút bùi ngùi, nhưng đồng thời là một cảm giác thành tựu lớn lao, và cảm giác cuối cùng đã được tự do. Tôi từng say mê bài toán này đến mức mất ăn mất ngủ, mọi lúc mọi nơi đều nghĩ về nó — sáng mở mắt ra nghĩ, tối đi ngủ cũng nghĩ — tình trạng đó kéo dài suốt tám năm trời. Đăm chiêu nghĩ về một việc duy nhất trong ngần ấy năm quả thực không hề dễ dàng. Giờ đây hành trình đặc biệt này cuối cùng đã kết thúc, tâm hồn tôi cuối cùng đã tìm lại được sự thanh thản bình yên."

## 科技动态

1. [Tesla mở bán xe Cybercab](https://electrek.co/2026/09/07/tesla-cybercab-fleet-profitable-wouldnt-sell/)

Tesla ra mắt dòng taxi tự hành Cybercab tại Mỹ. Theo lời Elon Musk, mảng kinh doanh cốt lõi của Tesla trong tương lai sẽ không còn là sản xuất ô tô mà là vận hành mạng lưới taxi không người lái.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090908.webp)

Tuần này, Tesla bất ngờ tuyên bố dòng taxi tự hành này sẽ được bán ra cho công chúng.

Bạn mua chiếc xe taxi tự hành này không phải để phục vụ việc đi lại cá nhân, mà là để đầu tư. Mỗi chuyến chở khách có doanh thu phát sinh, bạn và Tesla sẽ chia đôi 50-50.

Vì xe hoạt động liên tục 24/7, Musk luôn quảng bá rằng chỉ cần mua xe, ngay cả trong lúc bạn ngủ thì chiếc xe vẫn đang miệt mài kiếm tiền cho bạn.

Vấn đề là, khi mua chiếc xe này, bạn phải tự gánh chịu toàn bộ chi phí khấu hao hao mòn và mất giá xe, đồng thời phải chi thêm 15.000 USD để mua gói tính năng tự lái hoàn toàn (FSD). Rất khó hình dung một chiếc xe chạy cày ải suốt ngày đêm như vậy có thể trụ được bao nhiêu năm.

Bằng cách bán xe cho bạn, Tesla không còn phải nắm giữ phần cứng, chuyển sang đóng vai trò đơn vị vận hành xe của bạn — biến từ một mô hình kinh doanh thâm dụng tài sản nặng (heavy-asset) sang mô hình tài sản nhẹ (light-asset). Trong lúc bạn ngủ, xe của bạn không chỉ kiếm tiền cho bạn mà thực chất còn đang cày tiền cho chính Tesla.

2. [Bàn chải đánh răng điện Dyson](https://www.dyson.com/oral-care/electric-toothbrush/camerajet/ceramic-ultra-blue)

Dyson — hãng chuyên sản xuất máy hút bụi và máy sấy tóc cao cấp — vừa chính thức lấn sân sang mảng chăm sóc răng miệng với bàn chải đánh răng điện.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090909.webp)

Điểm độc đáo của chiếc bàn chải này là trên đầu bàn chải được trang bị một camera siêu nhỏ cùng đèn chiếu sáng.

Nó không chỉ cho phép bạn theo dõi tình trạng khoang miệng trực tiếp qua điện thoại, mà quan trọng hơn, thiết bị sẽ dựa vào hình ảnh camera ghi nhận để tự động nhận biết vị trí nào bám bẩn, từ đó tự động phun tia nước áp lực cao để tăng cường hiệu quả làm sạch.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090910.webp)

Tôi thấy nếu đã làm đến mức này rồi thì sao không làm hẳn một chiếc máy đánh răng tự động: bạn chỉ việc há miệng ra là máy tự động chải sạch bong từ A đến Z.

3. [Gậy chống thông minh AI](https://seas.harvard.edu/news/smartphone-navigation-app-people-blindness-and-low-vision)

Các kỹ sư tại Trường Kỹ thuật Harvard vừa phát minh ra một chiếc gậy chống AI hỗ trợ người khiếm thị và người thị lực kém.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090912.webp)

Chiếc gậy cần kết hợp sử dụng cùng điện thoại thông minh. Điện thoại dùng camera, GPS và các cảm biến chuyển động, phương hướng để thu thập dữ liệu không gian thời gian thực, kết hợp thuật toán điều hướng tự động tìm ra hướng đi tiếp theo rồi truyền tín hiệu đến gậy.

Chiếc gậy sẽ phát ra các âm thanh bíp bíp khác nhau để hướng dẫn người dùng đi thẳng, rẽ trái hay rẽ phải. Nếu người dùng đi chệch hướng, nó sẽ lập tức phát tiếng còi cảnh báo.

Tôi nhận thấy phát minh này thực sự rất hữu ích cho người khiếm thị, nhưng việc bắt điện thoại phải mở liên tục và camera phải luôn hướng ra mặt đường khá bất tiện. Sẽ tốt hơn nếu họ tích hợp thẳng phần cứng của điện thoại vào thân gậy để tạo thành một chiếc gậy thông minh độc lập hoàn chỉnh.

## 文章

1. [Câu chuyện bi kịch của Lee Holloway](https://note.com/masakazu_urabe/n/n7815f5b64fab?hl=en) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090902.webp)

Sinh năm 1981, Lee Holloway là kỹ sư sáng lập chủ chốt của Cloudflare và được mọi người công nhận là một thiên tài công nghệ hiếm có. Bức ảnh trên là 3 nhà sáng lập Cloudflare, anh đứng ở vị trí chính giữa.

Thế nhưng ở tuổi 36, anh mắc phải chứng sa sút trí tuệ khởi phát sớm (frontotemporal dementia), não bộ dần teo lại, đến mức về sau ngay cả việc nói tròn câu anh cũng không còn khả năng.

2. [Tổng kết tình hình mô hình mở mùa hè 2026](https://huggingface.co/blog/state-of-open-models-summer-2026) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090911.webp)

Hugging Face phân tích những bước tiến mới nhất của các mô hình mở (open-weight models), giúp độc giả nắm bắt vị thế hiện tại của các mô hình AI Trung Quốc trên bản đồ AI toàn cầu.

3. [Tôi đã bẻ khóa khóa RSA từ thập niên 90 như thế nào](https://mcpherrin.ca/2026/09/07/rsa.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090907.webp)

An toàn của truyền thông Internet hoàn toàn phụ thuộc vào việc khóa mã hóa có bị giải mã hay không. Tác giả đã thử phá khóa RSA 512-bit được cấp từ năm 1999 (hiện nay tiêu chuẩn tối thiểu là 2048-bit).

Kết quả là chiếc máy tính để bàn thông thường của anh chỉ mất 32 giờ là phá khóa thành công. Nếu dùng cụm tính toán GPU, thời gian chỉ mất khoảng 1 giờ.

Do đó, tiền điện tử (crypto) xét về lâu dài cũng tiềm ẩn rủi ro, định kỳ bắt buộc phải nâng cấp các thuật toán mã hóa.

4. [HTML không còn cần thuộc tính initial-scale](https://vale.rocks/micros/20260902-1350) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090401.webp)

Để trang web tự thích ứng viewport trên di động, hiện nay không cần thiết phải chỉ định `initial-scale=1.0` nữa, chỉ cần khai báo `width=device-width` là đủ.

Ở các dòng iPhone đời đầu, khi xoay ngang màn hình trang web không tự co giãn độ rộng, để [khắc phục lỗi này](https://quirksmode.org/quirksblog/2026/0902-initial.html) người ta mới khai sinh ra thuộc tính initial-scale.

5. [Cách xử lý đệ quy trong JavaScript](https://blog.gaborkoos.com/posts/2026-05-09-Your-Recursion-Is-Lying-to-You/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026080407.webp)

Khi dùng đệ quy, nếu stack lồng nhau quá sâu sẽ gây tràn bộ nhớ (stack overflow), đệ quy đuôi (tail recursion) có thể giải quyết bài toán này. Tuy nhiên các JavaScript runtime hiện tại không hỗ trợ tối ưu đệ quy đuôi (TCO); bài viết hướng dẫn bạn cách xử lý triệt để.

6. [Tôi tự dựng một phòng làm việc ngoài sân sau](https://www.imkylelambert.com/articles/building-a-backyard-office-the-build-and-cost-breakdown) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082606.webp)

Một lập trình viên người Mỹ tự tay dựng một studio làm việc tiện nghi ngay trong sân sau nhà mình. Anh ghi lại chi tiết từng bước xây dựng kèm bảng phân tích chi phí và hình ảnh trực quan.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082605.webp)

## 工具

1. [FlyonUI](https://flyonui.com/)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024100504.webp)

Thư viện component giao diện xây dựng trên nền Tailwind CSS.

2. [endlessh-go](https://github.com/shizunge/endlessh-go)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032905.webp)

Công cụ phòng thủ chống lại các cuộc tấn công dò quét SSH: thay vì ngắt kết nối, nó giữ cho các kết nối độc hại luôn rơi vào trạng thái chờ vô tận, từ đó làm cạn kiệt tài nguyên của kẻ tấn công. Hỗ trợ dashboard Grafana.

3. [PuTTYgen](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024033001.webp)

Công cụ tạo cặp khóa SSH trên nền tảng Windows.

4. [gh gfm-preview](https://github.com/thiagokokada/gh-gfm-preview)

Chương trình viết bằng Go dùng để khởi tạo một server cục bộ xem trước kết quả hiển thị Markdown theo đúng chuẩn GitHub Flavored Markdown.

5. [caddy-waf](https://github.com/fabriziosalmi/caddy-waf)

Plugin tường lửa ứng dụng web (WAF) cho máy chủ Caddy, hỗ trợ các quy tắc regex và danh sách đen IP/DNS/ASN/quốc gia để chặn đứng các request độc hại. (Đóng góp từ [@abriziosalmi](https://github.com/ruanyf/weekly/issues/11486))

6. [Nhất Tức (Yixi)](https://github.com/Defiabell/yixi)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090501.webp)

Web app triển khai trên Cloudflare Workers kết hợp cùng tính năng "Shortcuts" trên iOS: trước khi mở một app gây nghiện nào đó, hệ thống tự động chuyển hướng sang trang này và bắt bạn dừng lại hít thở 10 giây trước khi quyết định có mở tiếp hay không. (Đóng góp từ [@Defiabell](https://github.com/ruanyf/weekly/issues/11509))

7. [ctty](https://github.com/zsuroy/ctty)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026091001.webp)

Ứng dụng terminal mã nguồn mở giúp quản lý trực quan các kết nối SSH, Serial Port, Telnet... ngay trong giao diện đồ họa dòng lệnh. (Đóng góp từ [@zsuroy](https://github.com/ruanyf/weekly/issues/11522))

8. [vet](https://github.com/vet-run/vet)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025072420.webp)

Công cụ kiểm tra độ an toàn của tập lệnh Bash tải từ trên mạng về: nó phân tích những thay đổi mà script chuẩn bị thực hiện trên máy bạn và chỉ chạy khi được bạn phê duyệt.

9. [Krep](https://github.com/davidesantangelo/krep)

Công cụ thay thế cho lệnh `grep` để tìm kiếm chuỗi văn bản, được giới thiệu là có tốc độ nhanh hơn `grep` gấp 50 lần.

10. [Inbucket](https://inbucket.org/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024070709.webp)

Ứng dụng kiểm thử chức năng gửi nhận email dành cho nhà phát triển, có thể nhúng vào dự án để test email với giao diện quản trị Web tích hợp sẵn.

## 资源

1. [Kiến thức Linux căn bản cho Hacker](https://github.com/ahegazy0/linux-basics-for-hackers-notes) (Linux Basics for Hackers)

Tài liệu tiếng Anh giải thích các khái niệm căn bản của hệ điều hành Linux bằng ngôn ngữ bình dị, rất thích hợp làm giáo trình nhập môn.

2. [Nguyên lý hoạt động của DNSSEC](https://howdnssec.works/)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025062508.webp)

Website tiếng Anh sử dụng hình thức truyện tranh vui nhộn để giải thích cơ chế mở rộng bảo mật DNS (DNSSEC) giúp chống lại hình thức đầu độc bộ nhớ đệm DNS.

3. [Gorgeous GRUB](https://github.com/Jacksaur/Gorgeous-GRUB)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025050406.webp)

Kho lưu trữ tổng hợp các bộ theme giao diện khởi động cực đẹp dành cho bootloader GRUB.

## 图片

1. [Những công trình kiến trúc độc lạ ven đường cao tốc Mỹ](https://publicdomainreview.org/collection/john-margolies-photographs-of-roadside-america/)

Nước Mỹ được mệnh danh là quốc gia sống trên bánh xe, không có ô tô thì gần như không thể di chuyển.

Ven các tuyến đường cao tốc thường xuất hiện những ngôi nhà có hình thù kỳ dị nhằm thu hút ánh nhìn tò mò của khách vãng lai:

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090903.webp)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090904.webp)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090905.webp)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090906.webp)

Thư viện Quốc hội Mỹ hiện lưu giữ một [bộ sưu tập ảnh](https://www.loc.gov/pictures/search/?q=mrg&sp=1&st=gallery) gồm 11.710 bức ảnh màu chụp những ngôi nhà độc đáo ven đường như thế này.

## 文摘

1. [Trước khi bắt tay xây dựng bất cứ thứ gì, hãy tự hỏi bản thân ba câu hỏi](https://jordanlord.co.uk/blog/3-constraints/)

Tôi làm việc trong mảng phát triển sản phẩm đã được 10 năm, từng chứng kiến và trực tiếp tạo ra những sản phẩm thất bại — hoặc vì chúng quá phức tạp, hoặc vì thiếu đi một nét cá tính rõ ràng. Sau những vấp ngã đó, tôi đúc rút ra ba điều kiện giới hạn.

Về sau, trước khi bắt tay xây dựng bất cứ thứ gì, tôi đều tự vấn bản thân ba câu hỏi. Chỉ khi cả ba câu hỏi đều nhận được câu trả lời khẳng định chắc nịch, tôi mới tiến hành phát triển:

（1）Bạn có thể gói gọn phần giới thiệu sản phẩm vào đúng một trang giấy tóm tắt không?
Nếu một dự án cần nhiều hơn một trang giấy để diễn giải thì điều đó chứng tỏ nó đã quá phức tạp, tốt nhất đừng làm.

（2）Công nghệ cốt lõi có thể tách rời khỏi sản phẩm hay không?
Sản phẩm có thể liên tục phải chuyển hướng (pivot), nhưng công nghệ cốt lõi thì vẫn luôn bất biến và tiếp tục phát triển. Việc tách rời công nghệ cốt lõi khỏi hình hài sản phẩm sẽ buộc bạn phải tư duy vượt ra ngoài những giới hạn hạn hẹp của bản thân sản phẩm đó. Ví dụ: công nghệ cốt lõi của điện thoại di động là viễn thông di động. Một mẫu điện thoại cụ thể có thể thất bại, nhưng công nghệ viễn thông thì không.

（3）Sản phẩm có sở hữu một đặc trưng cốt lõi mang tính định hình không?
Đặc trưng này phải rõ ràng, sắc nét và ban tặng cho sản phẩm một cá tính độc nhất vô nhị. Chẳng hạn tựa game Minecraft hoàn toàn được tạo nên từ các khối lập phương vuông vức; IKEA mang đến những món đồ nội thất đóng gói dạng phẳng mà người dùng tự tay lắp ráp. Đặc trưng cốt lõi mà bạn lựa chọn sẽ thu hẹp không gian ra quyết định, giúp bạn tập trung vào những bài toán thực sự quan trọng. Nếu sản phẩm thiếu đi đặc trưng, hoặc chọn sai đặc trưng, bạn sẽ tạo ra một sản phẩm cồng kềnh, chắp vá với tham vọng làm hài lòng tất cả mọi thứ.

## 言论

1.

Khi AI thay thế nhà văn, tôi im lặng vì tôi không phải là nhà văn.
Khi AI thay thế họa sĩ, tôi im lặng vì tôi không phải là họa sĩ.
Bây giờ khi AI thay thế lập trình viên, thì đã chẳng còn ai có thể lên tiếng bênh vực cho tôi nữa rồi.

-- [《Và rồi AI đã thay thế lập trình viên》](https://medium.com/@sebastiancarlos/the-tech-market-situation-is-crazy-ec49ea772903)

2.

Hiện tại, cứ mỗi 5 tên miền cấp cao nhất mới được đăng ký thì có tới 1 tên miền là website lừa đảo.

-- [《Vấn nạn đăng ký tên miền độc hại》](https://simonwillison.net/2026/Sep/6/the-purpose-of-dns-is-to-spread-scams/)

3.

Người ta đang thi nhau để AI giải quyết hàng loạt bài toán khó, nhưng những bài toán toán học hay thì không thể tự tái sinh vô tận; ngày nay những câu hỏi hay đã trở nên vô cùng khan hiếm.
Việc dùng công cụ tự động hóa để giải bài không hề làm gia tăng tư duy toán học của nhân loại, trái lại đang làm tổn hại đến sự phát triển toán học trong tương lai.

-- [Terence Tao (Đào Triết Hiên)](https://mathstodon.xyz/@tao/117237320796901560), nhà toán học lỗi lạc

4.

Thế giới đang được "điện khí hóa", pin và động cơ điện đang tạo thành nền móng của đời sống; kết hợp với sự bùng nổ của AI, điều này đồng nghĩa với việc nhiều "vật vô tri vô giác" xung quanh chúng ta sẽ trở nên thông minh, có khả năng tự tư duy và tự di chuyển.

-- [Noah Smith](https://www.noahpinion.blog/p/at-least-five-interesting-things-304), chuyên gia phân tích kinh tế Mỹ

5.

Khoa học được chia thành hai nhánh. "Khoa học 1" là sự theo đuổi chân lý một cách lý tưởng hóa. "Khoa học 2" là thực hành khoa học ngoài đời thực, mang nhiều tính chất của hoạt động giao tiếp xã hội, đòi hỏi phải cân nhắc đến các thực tế xã hội và chính trị.
Nếu bạn là một nghiên cứu sinh tiến sĩ, bạn bắt buộc phải hiểu rằng bạn chủ yếu đang tham gia vào Khoa học 2 chứ không phải Khoa học 1.

-- [《Nghiên cứu sinh đừng cố gắng cải cách khoa học》](https://maxwellforbes.com/posts/dont-try-to-reform-science/)

## 往年回顾

[Kiếm tiền từ lưu lượng truy cập đang sụp đổ](https://www.ruanyifeng.com/blog/2025/09/weekly-issue-365.html) (#365)

[Bản báo cáo thôi việc ở Google](https://www.ruanyifeng.com/blog/2024/08/weekly-issue-315.html) (#315)

[Sau WiFi sẽ là LiFi](https://www.ruanyifeng.com/blog/2023/08/weekly-issue-265.html) (#265)

[Khuôn mẫu hành vi mà Internet ưa chuộng nhất](https://www.ruanyifeng.com/blog/2022/07/weekly-issue-215.html) (#215)

(Hết)
