# Bản tin công nghệ hàng tuần (Số 411): OpenClaw 2.0 là một bức tranh thu nhỏ

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/11434) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082702.webp)

Tại Tây Hạ Lăng ở Ninh Hạ, người ta sử dụng lưới kim loại để phục dựng các mảnh vỡ tàn tích thành tượng đá bảo vệ lăng mộ (thạch tượng sinh). ([via](https://news.ifeng.com/c/8vTLFjHaN2k))

## OpenClaw 2.0 是一个缩影

Tuần này, OpenClaw vừa phát hành [phiên bản 2.0](https://openclaw.ai/blog/openclaw-2-accidentally).

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026083101.webp)

Có phải đã rất lâu rồi bạn không nghe thấy cái tên này? Hiện tại rất hiếm người nhắc tới nó, dù thực tế mới chỉ trôi qua nửa năm.

Nhớ lại dịp Tết Nguyên Đán năm nay, dự án nổi đình nổi đám chỉ sau một đêm, trở thành tâm điểm bàn tán của toàn dân. Vào thời điểm đó, dịch vụ "đến tận nhà cài đặt Tôm Hùm (OpenClaw)" trở thành dịch vụ thịnh hành, và thực sự có không ít người đã chi tiền trả phí.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026083102.webp)

Chỉ mới qua nửa năm ngắn ngủi, nó đã trở thành bông hoa tàn ngày hôm qua, gần như bị lãng quên. Kỷ nguyên AI chính là như vậy, cái mới xuất hiện dồn dập không ngừng, cơn sốt dù có bùng nổ đến đâu cũng chỉ giữ được độ nóng trong vài ngày.

Mất nửa năm, cuối cùng dự án cũng nâng cấp từ bản 1.0 lên 2.0.

Như mọi người đều biết, mã nguồn của OpenClaw gần như 100% là do AI tạo ra; giai đoạn đầu mỗi ngày họ đều đặn phát hành một phiên bản. Về sau nhận thấy làm như vậy không ổn, người dùng sẽ mệt mỏi kiệt sức vì cập nhật liên tục, nên từ tháng 7 họ đã đổi sang **mỗi tháng phát hành một phiên bản**.

Lấy tháng 8 làm ví dụ: đầu tháng họ tung ra bản thử nghiệm [2026.8.1-beta1](https://github.com/openclaw/openclaw/releases/tag/v2026.8.1-beta.1), giữa tháng tiếp tục ra beta2 và beta3, đến cuối tháng thì ra mắt [bản chính thức tháng 8](https://github.com/openclaw/openclaw/releases/tag/v2026.8.1). Đồng thời, họ cũng phát hành luôn bản thử nghiệm tháng 9 [2026.9.1.beta1](https://github.com/openclaw/openclaw/releases#release-v2026.9.1-beta.1).

Nhịp điệu phát hành này tạo cảm giác dễ chịu hơn cho người dùng, mỗi tháng nâng cấp một lần là vừa vặn.

Vì bản tháng 8 có quá nhiều thay đổi lớn nên phiên bản này được đánh dấu là bản 2.0. Theo [thông báo phát hành](https://openclaw.ai/blog/openclaw-2-accidentally), bản cập nhật có tổng cộng 933 người đóng góp và đã hợp nhất tới 16.000 Pull Request (PR).

Con số này thực sự gây choáng ngợp. Theo website chính thức, đội ngũ phát triển của OpenClaw gồm 9 người [toàn thời gian](https://www.openclaw.org/people) và 26 người bán thời gian. Cho dù toàn bộ những người này cùng tham gia thì tôi nghĩ cũng không thể nào trong vòng một tháng rà soát và hợp nhất nổi 16.000 PR.

Mỗi sớm mở mắt ra là có hơn 500 PR đang nằm chờ duyệt, làm sao con người có thể đọc xuể?

Kết luận duy nhất chỉ có thể là: **những PR này không hề qua khâu code review thủ công của con người, mà hoàn toàn do AI tự động merge!**

Tôi phỏng đoán rằng, chỉ cần admin thấy PR đó có vẻ hợp lý, vượt qua khâu kiểm tra tự động của AI và các bộ test, thì sẽ lập tức được merge vào kho mã nguồn.

Cách làm này thực ra cũng chẳng có gì lạ, lập trình cảm tính quy mô lớn (large-scale Vibe Coding) chỉ có thể dẫn đến kết quả này. Vấn đề là công cụ OpenClaw có chức năng chính là tự động kích hoạt và điều phối các công cụ bên ngoài, các test case rất khó bao quát toàn bộ các tình huống trên mọi nền tảng, chắc chắn sẽ có rất nhiều góc khuất chưa từng được kiểm thử tới.

Do đó, 16.000 PR đó rốt cuộc đã đưa vào bao nhiêu lỗi tiềm ẩn (bug), bao nhiêu rủi ro bảo mật khôn lường, thật khó để khiến người dùng yên tâm tin tưởng.

Cũng như trước đây, tôi vẫn đưa ra lời khuyên chân thành: **tuyệt đối không chạy OpenClaw trực tiếp trên máy tính làm việc cá nhân của bạn**, mà hãy cho chạy trên máy vật lý độc lập, máy ảo cách ly hoặc trên môi trường đám mây.

Mô hình phát triển của OpenClaw chính là bức tranh thu nhỏ của phát triển phần mềm thời AI. Hàng loạt phần mềm đang nhanh chóng đi theo con đường này: do AI trực tiếp viết code hoặc merge PR.

Tôi đồ rằng, các phần mềm ứng dụng trong tương lai có lẽ đều không nên chạy trực tiếp trên hệ thống máy chủ/máy trạm bản địa nữa. Máy cá nhân chỉ nên chạy hệ điều hành cơ bản, còn ứng dụng thì cô lập hoàn toàn trên máy ảo hoặc đám mây.

Nhìn theo hướng này, mô hình "Trác Dịch Thông" (môi trường tương thích chạy app Android trên HarmonyOS) hóa ra lại rất phù hợp với xu thế phát triển của kỷ nguyên AI.

## 没人为你的堆栈辩护

Ryan Carniato, nhà sáng lập framework JavaScript frontend SolidJS, gần đây đã đăng một bài viết gây nhiều chú ý [《Không ai đứng ra bảo vệ tech stack của bạn》](https://dev.to/playfulprogramming/nobody-argued-for-your-stack-51fj).

Anh cảm thán (hoặc có thể nói là than phiền) rằng từ khi có AI, mọi người đua nhau di chuyển sang các công nghệ dòng chính (mainstream stack).

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082902.webp)

Trang chủ của Cursor và trang tài liệu của Anthropic đều đã chuyển từ SolidJS sang React. Là cha đẻ của SolidJS, trong lòng anh cảm thấy vô cùng chua xót:

> Phản ứng đầu tiên của tôi không hề dễ chịu chút nào, tâm huyết bao năm của tôi bỗng trở thành trường hợp điển hình bị người ta vội vã rũ bỏ. Trớ trêu thay, ngay trong tuần đó, chúng tôi vừa phát hành phiên bản mới với quy mô lớn nhất trong lịch sử dự án. Điều đó thực sự khiến tôi đau đớn, tôi không thể phủ nhận điều đó.

Anh chỉ ra rằng trước đây, việc di chuyển cả một bộ tech stack là quyết định tốn kém chi phí cực lớn và rủi ro khổng lồ, hiếm ai dám liều lĩnh làm. Nhưng giờ đây, AI có khả năng viết lại toàn bộ mã nguồn dễ như trở bàn tay, khiến việc di chuyển trở nên quá đỗi nhẹ nhàng. Thế là ban lãnh đạo các công ty liên tục đề xuất chuyển dịch về các tech stack thịnh hành nhất.

Những ví dụ khác có thể kể đến như: website marketing của công ty Cognition chuyển từ Astro sang Next.js; runtime Bun chuyển từ Zig sang Rust.

Không cần những buổi tranh luận phản biện nhiều vòng, không cần hàng năm trời đánh giá cẩn trọng, đôi khi chỉ qua một cuộc họp nội bộ ngắn là công ty đã quyết định khai tử tech stack hiện tại để nhảy sang công nghệ phổ biến hơn.

Hoàn toàn không có ai đứng ra bảo vệ stack đang sử dụng, tất cả đều tranh nhau chen chân ôm lấy cái gọi là "best practices".

Kết luận của anh là: "Cứ theo đà này, ngoại trừ một số trường hợp ngoại lệ hiếm hoi, **mỗi tầng kiến trúc cuối cùng đều sẽ quy tụ về giải pháp phổ biến nhất tại thời điểm đó**. Frontend đổ dồn về React, hệ thống đổ dồn về Rust, script đổ dồn về Python, thậm chí bản thân các trang web đều đổ dồn về Next.js, hoàn toàn phớt lờ độ tương thích và tính phù hợp thực tế."

Anh nhận định rằng AI luôn ưu tiên sử dụng những công nghệ thịnh hành nhất, khiến các công nghệ ngách ít người biết đến càng trở nên hoang phế không ai đoái hoài. Cứ kéo dài tình trạng này, hệ sinh thái phần mềm sẽ bị đồng nhất hóa nghèo nàn, sự đa dạng phong phú sẽ không còn tồn tại nữa.

Thế thì chúng ta không khỏi tự hỏi: nếu mảnh đất thiếu đi tính đa dạng, không còn những thử nghiệm táo bạo và cơ hội sửa sai, **thì ý tưởng sáng tạo đột phá tiếp theo của hệ sinh thái phần mềm sẽ đến từ đâu?** Hay là việc lập trình bằng AI vốn dĩ chẳng cần bận tâm đến đổi mới, code sinh ra cứ chạy được là xong?

## 科技动态

1. [Truyền thông laser hai chiều giữa Trái Đất và Mặt Trăng](https://www.guancha.cn/politics/2026_08_29_829154.shtml)

Viện Hàn lâm Khoa học Trung Quốc gần đây đã thực hiện thành công thử nghiệm truyền thông laser tốc độ cao hai chiều giữa Trái Đất và Mặt Trăng.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026083001.webp)

Truyền thông laser ngoài không gian có ba bài toán hóc búa: (1) Đầu phát và đầu thu cách nhau hàng trăm nghìn kilomet, chùm tia sáng rất khó căn chỉnh chuẩn xác; (2) Tín hiệu khi chạm tới mặt đất đã suy hao cực yếu gần như không thu được; (3) Tốc độ truyền tải rất khó nâng cao. Lần này cả ba thách thức trên đều được giải quyết thành công.

Tốc độ truyền thông trong thử nghiệm đạt mức tải lên (uplink) 1,25 Mbps và tải xuống (downlink) 100 Mbps, tương đương ngưỡng tối thiểu của mạng băng thông rộng mặt đất, là con số rất đáng nể.

Trong tương lai việc lướt mạng tốc độ cao ngay trên Mặt Trăng hoàn toàn có thể trở thành hiện thực.

2. [Hàn Quốc cấp Token không giới hạn miễn phí cho mọi công dân](https://decrypt.co/376929/south-korea-will-give-every-citizen-free-ai-access-with-unlimited-tokens)

Nhằm thúc đẩy phổ cập AI, chính phủ Hàn Quốc dự kiến cấp miễn phí Token không giới hạn cho toàn thể người dân, đồng nghĩa với việc người dân được dùng AI thỏa thích.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090104.webp)

Có ba đơn vị chịu trách nhiệm triển khai: hai nhà mạng viễn thông lớn nhất Hàn Quốc và Kakao (ứng dụng nhắn tin quốc dân). Họ sẽ ra mắt các ứng dụng AI riêng để phục vụ người dân miễn phí. Chính phủ dự kiến cấp cho mỗi bên 512 chip NVIDIA B200.

Chính phủ Hàn Quốc cũng quy định ít nhất 80% lưu lượng sử dụng phải hướng về các mô hình lớn nội địa của Hàn Quốc, chỉ khi cần thiết mới được gọi mô hình nước ngoài.

Hiện vẫn chưa rõ dịch vụ này có cung cấp cổng API cho người dân tự do tích hợp hay không. Khả năng cao là không, vì chi phí sẽ vô cùng khủng khiếp. Nhưng nếu chỉ là chat AI miễn phí thì ý nghĩa thực tế không quá lớn, bởi hiện nay việc chat với AI vốn đã gần như miễn phí hoàn toàn rồi.

3. [Nhận nuôi điểm ảnh vũ trụ (Adopt a Pixel)](https://science.nasa.gov/mission/roman-space-telescope/adopt-a-pixel/)

Cơ quan Hàng không Vũ trụ Mỹ (NASA) tuần này đã phóng kính viễn vọng không gian Nancy Grace Roman.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090201.webp)

Đường kính gương chính của kính là 2,4 mét, sở hữu trường nhìn lớn nhất trong các kính viễn vọng không gian hiện nay, hứa hẹn mở ra những khung cảnh vũ trụ chưa từng được khám phá.

NASA đang tổ chức chiến dịch "Nhận nuôi điểm ảnh": chỉ cần đăng ký họ tên và email tại [địa chỉ này](https://science.nasa.gov/mission/roman-space-telescope/adopt-a-pixel/), bạn sẽ được nhận quyền sở hữu danh nghĩa một pixel trong đợt ảnh chụp đầu tiên của kính viễn vọng.

Người đăng ký sẽ nhận được chứng nhận kỹ thuật số (hình dưới) có thể in ra, trên đó ghi rõ mã số pixel của bạn.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090202.webp)

4. [Xe bus Sushi](https://www.engadget.com/2241785/tokyos-sushi-bus-combines-conveyor-belt-dining-with-open-air-sightseeing/)

Xe bus hai tầng ngắm cảnh ở Tokyo, Nhật Bản vừa đưa vào phục vụ món sushi. Du khách vừa có thể ngắm cảnh phố phường vừa thưởng thức sushi băng chuyền ngay trên xe.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026083002.webp)

Tầng một của xe là khu vực bếp chế biến, tầng hai có dải băng chuyền chạy dọc theo cửa sổ, liên tục đưa các đĩa sushi đến trước mặt thực khách.

Sau hai năm thử nghiệm, dịch vụ mới chính thức lăn bánh. Khó khăn lớn nhất trong quá trình thử nghiệm là tài xế tuyệt đối không được phanh gấp, nếu không sushi sẽ bị văng khỏi băng chuyền.

Dịch vụ này thực sự biến khái niệm "nhà hàng di động" thành hiện thực. Tuy nhiên mức giá 16.000 yên/người (khoảng gần 2,5 triệu đồng) không hề rẻ chút nào.

## 文章

1. [Tại sao gói quota Claude của tôi bị cạn sạch chỉ trong 10 phút](https://www.kelviq.com/blog/claude-code-usage-limits-where-tokens-go/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082904.webp)

Tài khoản Claude Max của tác giả bất ngờ bị ngốn lưu lượng đột biến. Trước đây quota dùng được 5 đến 6 ngày mỗi tuần, nay chỉ được 2 ngày, thậm chí có hôm toàn bộ hạn mức 5 giờ bị nuốt chửng chỉ trong 10 phút.

Sau khi điều tra, anh phát hiện có một chương trình đang chạy Claude Code theo dạng cụm (cluster), trên máy tính cùng lúc chạy tới 1.555 phiên hội thoại song song!

Bài viết tổng kết quá trình điều tra và chia sẻ công cụ [tare](https://github.com/kelviq/tare) do anh tự viết, có thể phân tích log cục bộ của Claude Code và xuất báo cáo trực quan (hình dưới), nhìn vào là thấy ngay token bị tiêu hao ở đâu.

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082903.webp)

2. [Giới thiệu WebMCP](https://sreenathmenon.com/blog/2026-08-04-webmcp-teaching-websites-to-talk-to-ai-agents/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082905.webp)

Hiện tại nếu muốn để AI thao tác trên trang web, chúng ta phải chụp màn hình hoặc cào mã nguồn HTML, bắt AI "mò mẫm tìm chiếc nút bấm giữa hàng chục thẻ `<div>` lộn xộn".

Trình duyệt Chrome bắt đầu cung cấp giao diện WebMCP nhằm giải quyết vấn đề này. Cụ thể, các trang web có thể dùng mã JavaScript định nghĩa sẵn các interface MCP cho trang của mình để AI trực tiếp gọi hàm.

3. [Tại sao ở tiền tuyến, bận rộn nhất lại là các lập trình viên Ukraine?](https://mp.weixin.qq.com/s/KyRAvnPNanwy4K1lXzWgXA?poc_token=HC2Wl2qjmcy25tD071C9Vda3QpchiZpdVnqvBGi7) (tiếng Anh)

Khi bạn tiếp nhận đủ loại vũ khí khác nhau từ nhiều quốc gia, việc làm sao tích hợp đồng bộ chúng vào chung một hệ sinh thái tác chiến duy nhất trở thành bài toán công nghệ vô cùng đau đầu. (Đóng góp từ [@zuzuAndroid](https://github.com/ruanyf/weekly/issues/11443))

4. [Chạy OpenBSD trên DigitalOcean chỉ với 4 USD/tháng](https://nil.wallyjones.com/run-openbsd-on-digitalocean-for-4month/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082604.webp)

OpenBSD là hệ điều hành máy chủ cực kỳ xuất sắc và bảo mật. Bài viết hướng dẫn chi tiết cách khởi tạo một máy ảo giá rẻ để vọc vạch và học tập.

5. [Cách sắp xếp nhánh git theo thứ tự thời gian commit giảm dần](https://ryangreenberg.com/til/git-branches-by-commit-date/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090103.webp)

Lệnh `git branch` hiển thị danh sách các nhánh trong kho, mặc định xếp theo thứ tự bảng chữ cái. Chỉ cần cấu hình đơn giản tham số `branch.sort`, bạn có thể cho danh sách sắp xếp theo thời gian commit mới nhất.

6. [Cách tự động format nội dung JSON trong clipboard](https://chris48s.github.io/blogmarks/posts/2021/jsontidy/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090303.webp)

Bài viết hướng dẫn mẹo đơn giản để thay thế nội dung clipboard, ví dụ như tự động format làm đẹp chuỗi JSON vừa copy.

## 工具

1. [OpenCode Mobile](https://github.com/learning233/opencode_mobile)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082908.webp)

Ứng dụng client Android không chính thức dành cho OpenCode. (Đóng góp từ [@learning233](https://github.com/ruanyf/weekly/issues/11381))

2. [Blob Downloader](https://github.com/aeroxy/blob-downloader)

Extension trình duyệt Chrome dùng để tải video và file ẩn sau các liên kết blob trên web. (Đóng góp từ [@aeroxy](https://github.com/ruanyf/weekly/issues/11392))

3. [zlib](https://github.com/heartleo/zlib)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082909.webp)

Công cụ dòng lệnh viết bằng Go dành cho thư viện sách Z-Library. (Đóng góp từ [@heartleo](https://github.com/ruanyf/weekly/issues/11405))

4. [ATBClone](https://github.com/aitobox/ATBClone)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026083107.webp)

Ứng dụng macOS mã nguồn mở cho phép nhân bản chạy nhiều phiên bản ứng dụng cùng lúc và quản lý tài khoản riêng biệt. (Đóng góp từ [@aitoboxinc](https://github.com/ruanyf/weekly/issues/11432))

5. [Orange Cloud](https://github.com/chen2he/orange-cloud)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026083105.webp)

Ứng dụng iOS mã nguồn mở để quản lý tài nguyên Cloudflare. (Đóng góp từ [@chen2he](https://github.com/ruanyf/weekly/issues/11428))

6. [Apolu](https://apolu.app/zh-Hans)

Ứng dụng trên các thiết bị Apple, theo dõi miễn phí thứ hạng và đánh giá review của một app bất kỳ trên các kho App Store khắp thế giới. (Đóng góp từ [@chen2he](https://github.com/ruanyf/weekly/issues/11429))

7. [DanKS](https://github.com/Calix-L/DanKS)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026083103.webp)

Agent AI mã nguồn mở chơi bài Quan Đán (GuanDan) do Kingsoft AI Product Center phát hành. (Đóng góp từ [@Calix-L](https://github.com/ruanyf/weekly/issues/11422))

8. [video-ai-talking](https://github.com/yizhi-chengzi/video-ai-talking)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090212.webp)

Web app mã nguồn mở, chỉ cần nhập văn bản là sinh ra video người thật đọc thuyết trình. (Đóng góp từ [@yizhi-chengzi](https://github.com/ruanyf/weekly/issues/11449))

9. [Git Agent](https://github.com/adoin/git-Agent)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090301.webp)

Client Git desktop đa nền tảng mã nguồn mở, tích hợp khu vực làm việc, lịch sử commit, so sánh diff và xử lý xung đột 3-way merge trong cùng một cửa sổ, hỗ trợ các tính năng AI. (Đóng góp từ [@adoin](https://github.com/ruanyf/weekly/issues/11464))

10. [Subtitle Scout](https://github.com/fancydirty/subtitle-scout)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090302.webp)

Ứng dụng tìm phụ đề tự lưu trữ (self-hosted), tự động tìm kiếm trên 5 nguồn phụ đề dựa trên video của bạn và dùng AI để chọn ra phụ đề chuẩn khớp nhất. (Đóng góp từ [@fancydirty](https://github.com/ruanyf/weekly/issues/11468))

## 资源

1. [Ad Astra](https://github.com/gunerguner/AdAstra)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082907.webp)

Web app bầu trời sao thời gian thực, có thể tương tác và dùng offline, tái hiện bầu trời tại bất kỳ tọa độ và thời điểm nào, mô phỏng chuyển động của các vì sao theo thời gian. (Đóng góp từ [@gunerguner](https://github.com/ruanyf/weekly/issues/11360))

2. [Đàn piano 3D](https://autopiano.cn/3d)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026083106.webp)

Trực quan hóa vị trí các phím đàn trên cây đàn piano 3D khi phát một bản nhạc hoặc khi bạn bấm trên bàn phím MIDI. (Đóng góp từ [@WarpPrism](https://github.com/ruanyf/weekly/issues/11431))

3. [ScriptSpool](https://scriptspool.pixzens.com/zh/editor)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026083108.webp)

Website biến đoạn code của bạn thành video hoạt họa gõ từng phím như người thật gõ máy. (Đóng góp từ [@liyuouyu](https://github.com/ruanyf/weekly/issues/11433))

4. [Mô hình hóa 3D phòng vệ sinh](https://restroomarchive.com/r/2024-10-16-commonwealth-bar-some-restroom)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090206.webp)

Website quét 3D nhiều phòng vệ sinh công cộng thực tế tại Mỹ, cho phép người dùng xoay xem 360 độ các góc trong phòng vệ sinh ngay trên trình duyệt.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090207.webp)

## 图片

1. [Thiết bị đo độ xanh của trời (Cyanometer)](https://byopiapress.wordpress.com/2024/05/19/a-cyanometer-and-a-cloud-colourimeter/)

Năm 2016, một nghệ sĩ đã đặt 4 tác phẩm nghệ thuật tại quảng trường của 4 thành phố châu Âu.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090203.webp)

Thiết bị phản chiếu màu sắc của bầu trời, phía trên có một thang đo màu xanh (cyanometer) giúp người xem xác định sắc xanh của bầu trời hiện tại đang ở mức độ nào.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090204.webp)

Thiết bị còn định kỳ chụp ảnh bầu trời gửi về máy chủ để hiển thị bầu trời của cả 4 thành phố cùng lúc trên website.

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026090205.webp)

2. [Điêu khắc từ dầu ô liu](https://kottke.org/26/01/olive-oil-sculptures)

Một nhiếp ảnh gia người Mỹ chuyên ghi lại khoảnh khắc giọt dầu ô liu bắn tung tóe. Anh xem đó là những tác phẩm điêu khắc tràn đầy sức sống.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011707.webp)

Anh cho rằng mọi người chưa nhận ra rằng những giọt dầu bắn lên thực ra mang tính thẩm mỹ nghệ thuật rất cao.

## 文摘

1. [Tại sao phần mềm tự do nguồn mở thường có trải nghiệm người dùng tệ hại](https://web.archive.org/web/20030201183139/http://mpt.phrasewise.com/discuss/msgReader$173)

![](https://cdn.beekka.com/blogimg/asset/202608/bg2026082906.webp)

Khi dùng phần mềm tự do, chúng ta thường nhận thấy giao diện (UI) của chúng rất không thân thiện và khó sử dụng.

Vấn đề này cực kỳ phổ biến, phần mềm tự do có giao diện đẹp mắt chỉ đếm trên đầu ngón tay, và điều này hoàn toàn có nguyên nhân sâu xa.

Lý do gốc rễ là hầu hết các dự án nguồn mở đều vận hành dựa trên tình nguyện viên, và **việc phụ thuộc vào tình nguyện viên gần như tất yếu sẽ dẫn đến thiết kế giao diện tệ hại**:

（1）Đa số tình nguyện viên trong các dự án nguồn mở là lập trình viên, rất hiếm nhà thiết kế chuyên nghiệp. Do đó, giao diện thường do chính lập trình viên tự tay thiết kế.

（2）Dù dự án có nhà thiết kế giao diện chuyên trách, những đề xuất của họ cũng khó nhận được sự coi trọng từ lập trình viên như trong các dự án thương mại.

（3）Nhiều lập trình viên mặc định cho rằng thiết kế của Microsoft hay Apple là chuẩn mực nên cứ bắt chước rập khuôn, nhưng thực tế không phải lúc nào cũng phù hợp.

（4）Tình nguyện viên thường chỉ phát triển những gì họ thấy hứng thú, tức là công cụ phục vụ cho chính họ. Vì họ là người dùng chuyên sâu (power user), giao diện họ thấy tiện lợi thường quá phức tạp và khó dùng với người bình thường.

（5）Nhiều chi tiết nhỏ tinh tế giúp nâng cao trải nghiệm người dùng thường rất tẻ nhạt khi code và không thú vị, nên tình nguyện viên thường lảng tránh không làm.

（6）Phần mềm nguồn mở có nhiều người đóng góp, ai cũng muốn can thiệp vào thiết kế giao diện dù hiểu biết nông sâu thế nào. Một khi có nhiều hơn một người làm thiết kế, sự thiếu nhất quán sẽ lập tức xuất hiện. Chất lượng thiết kế giao diện tỷ lệ nghịch với số lượng người tham gia thiết kế.

（7）Để khích lệ người đóng góp, quản trị viên dự án thường dễ dãi cho phép mỗi người tự thêm mục cài đặt cho tính năng của mình vào giao diện. Điều này khiến bảng cài đặt trở nên cồng kềnh, vụn vặt, khó hiểu, thiếu kiểm thử và khiến người dùng thông thường hoàn toàn bối rối.

## 言论

1.

Cấm xuất khẩu GPU sang Trung Quốc sẽ chỉ thúc đẩy họ tự lực phát triển công nghệ riêng. Đúng là việc này sẽ khiến họ mất nhiều thời gian hơn, nhưng về lâu dài, việc tự chủ phát triển công nghệ GPU sẽ giúp Trung Quốc gặt hái thành công lớn hơn nhiều.

-- [Cư dân mạng trên Hacker News](https://news.ycombinator.com/item?id=49487064)

2.

Khi bạn đọc một cuốn tiểu thuyết hay và đắm chìm vào đó, tác giả như thể đã nắm giữ tâm trí bạn — bạn mường tượng ra thế giới của họ, và câu chữ của họ dần biến thành dòng suy nghĩ của chính bạn.

-- [《Về việc không trở thành cyborg》](https://nolanlawson.com/2026/08/31/on-not-becoming-a-cyborg/)

3.

Gần đây tôi tham gia một diễn đàn mở; trong phần hỏi đáp, tôi và các diễn giả khác ngồi trên sân khấu đón nhận câu hỏi từ khán giả.

Điều khiến tôi sốc là trong lúc tôi trả lời trên bục, tất cả những người khác đều mở laptop dùng AI để tra câu trả lời cho câu hỏi đó. Nếu tất cả chúng ta đều dùng AI để chuẩn bị bài phát biểu, slide và giải đáp thắc mắc, thì những diễn đàn mở kiểu này cuối cùng chỉ còn giữ lại mỗi mục đích giao lưu xã giao mà thôi.

-- [Độc giả Lobste.rs](https://lobste.rs/s/qn7jtv/i_attended_conference_recently_ai_use_by)

4.

Đừng nhầm lẫn giữa chuyển động và sự tiến bộ, chú ngựa gỗ bập bênh liên tục lắc lư nhưng chẳng hề tiến thêm được bước nào.

-- [Alfred A. Montapert](https://graybeard.ing/the-religion-of-speed/), nhà văn người Mỹ

## 往年回顾

[Khối Rubik khó giải nhất](https://www.ruanyifeng.com/blog/2025/09/weekly-issue-364.html) (#364)

[《Hắc Thần Thoại: Ngộ Không》 có thể công nghiệp hóa không?](https://www.ruanyifeng.com/blog/2024/08/weekly-issue-314.html) (#314)

[Bài học từ Elasticsearch](https://www.ruanyifeng.com/blog/2023/07/weekly-issue-264.html) (#264)

[Bản đồ của bạn bị vẽ sai](https://www.ruanyifeng.com/blog/2022/07/weekly-issue-214.html) (#214)

(Hết)
