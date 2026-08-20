# Bản tin chia sẻ công nghệ (Số 387): Bạn đang đi trước thế giới

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/9088) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030503.webp)

Lồng đèn hình Cá May Mắn khổng lồ dài 25 mét được điều khiển bằng hệ thống cơ khí bay lượn trên bầu trời trong sự kiện lễ hội đèn lồng Tết Nguyên tiêu tại thành phố Phúc Châu. ([via](http://fj.people.com.cn/n2/2026/0304/c181466-41515232.html))

## 你是领先的

Dân số thế giới hiện nay đã chạm mốc 8,1 tỷ người. Nếu chúng ta trực quan hóa con số này dưới dạng một biểu đồ ô vuông (hình dưới), với mỗi ô vuông đại diện cho 3,2 triệu người:

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022615.webp)

- Có tới 6,88 tỷ người (chiếm 84% dân số) chưa từng tiếp xúc hay sử dụng bất kỳ công cụ AI nào (thể hiện bằng các ô vuông màu xám).
- Khoảng 1,38 tỷ người (chiếm 16%) từng thực hiện tương tác trò chuyện với AI (các ô màu xanh).
- Khoảng 15 đến 25 triệu người (chiếm 0,3%) có đăng ký sử dụng các dịch vụ AI trả phí (các ô màu vàng).
- Chỉ có khoảng 2 đến 5 triệu người thực sự sử dụng AI để tự tạo các dự án lập trình của riêng mình (khối màu đỏ), chiếm 0,04%.

Do đó, nếu bạn đang đọc bản tin này, thường xuyên theo dõi các tin tức cập nhật về AI và từng sử dụng AI để tự viết code, bạn đã chính thức đi trước và vượt trội hơn 99% dân số trên thế giới.

## OpenClaw 的安全

Sản phẩm phần mềm tạo nên sức hút nóng nhất trên thế giới hiện nay chắc chắn phải kể đến trợ lý AI cá nhân mang tên [OpenClaw](https://openclaw.ai/).

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030302.webp)

Sức hút của nó lớn đến mức nào?

Chỉ trong vòng vỏn vẹn 4 tháng ra mắt, dự án đã thu về tới 250.000 lượt yêu thích (stars) trên GitHub, chính thức vượt qua thư viện React để trở thành dự án phần mềm có số lượng star lớn nhất trong lịch sử.

Cần lưu ý để đạt được cột mốc số lượng star khổng lồ này, React đã phải mất tới 13 năm phát triển, trong khi OpenClaw chỉ cần đúng 4 tháng.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030303.webp)

Trong biểu đồ trên, đường màu đỏ dựng đứng thẳng tắp biểu thị tốc độ tăng trưởng sao kỷ lục của OpenClaw – một con số thực sự điên rồ.

Tính năng cốt lõi của OpenClaw là hỗ trợ người dùng sử dụng mô tả bằng ngôn ngữ tự nhiên để điều khiển máy tính tự động hóa mọi tác vụ. Trước đây, bạn phải cài đặt rất nhiều phần mềm chuyên dụng và trang bị kỹ năng chuyên môn tốt mới đạt được hiệu quả tương ứng. Còn hiện nay, bạn chỉ cần gõ chữ hoặc ra lệnh bằng giọng nói, trải nghiệm vừa hữu ích lại vừa thú vị.

Đây chính là diện mạo lý tưởng mà trợ lý ảo Siri của Apple đáng lẽ phải sở hữu từ lâu. Đối với người dùng phổ thông, đây mới là phương thức tương tác tự nhiên nhất với máy tính. Có thể dự báo trong vòng vài năm tới, các ứng dụng dạng này sẽ nhanh chóng được tích hợp phổ cập trên hệ điều hành di động của mọi người.

Tuy nhiên, dự án đang vấp phải một vấn đề lớn: rủi ro bảo mật an toàn thông tin.

Mã nguồn của OpenClaw chứa tới hơn 400.000 dòng code, 53 tệp tin cấu hình và hơn 70 thư viện phụ thuộc, tất cả được tự động sinh ra bởi AI chỉ trong vòng vài tuần ngắn ngủi mà hoàn toàn không trải qua bất kỳ quy trình kiểm duyệt chất lượng hay review mã nguồn chính quy nào.

Để vận hành, ứng dụng yêu cầu người dùng cung cấp các khóa bảo mật cá nhân (API keys) cùng các quyền hạn truy cập hệ thống cực kỳ lớn để chạy tự động hoàn toàn. Thậm chí nhiều người dùng đã mạo hiểm cấp quyền truy cập tài khoản Apple ID hay Gmail cá nhân cho AI – một kịch bản vô cùng nguy hiểm nếu hệ thống phát sinh lỗi ngoài ý muốn.

Khả năng bảo mật phòng vệ của phần mềm trong thiết kế ban đầu hầu như bằng không, khiến hệ thống rất dễ bị rò rỉ công khai trên mạng Internet.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030301.webp)

Một lập trình viên đã thiết kế trang web [OpenClaw Exposure Watchboard](https://openclaw.allegro.earth/) (Bảng giám sát rò rỉ OpenClaw) để thống kê toàn bộ các máy chủ chạy OpenClaw đang bị lộ thông tin công khai trên Internet (hình trên). Tính đến ngày hôm qua, số lượng máy chủ bị rò rỉ đã chạm mốc 258.305 thiết bị.

Bạn có thể ngẫu nhiên click chọn một thiết bị bất kỳ trong danh sách là đã có thể truy cập thẳng vào bảng điều khiển quản trị OpenClaw của người dùng đó (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030304.webp)

Chủ nhân của các máy tính này vẫn đang đinh ninh rằng mình đang tự động hóa công việc cá nhân an toàn, mà không hề hay biết cánh cửa kết nối máy tính của họ đang mở toang cho cả thế giới dạo chơi.

Nếu bạn có ý định sử dụng OpenClaw, tối thiểu hãy cài đặt nó bên trong một máy ảo (virtual machine) hoặc chạy trên một thiết bị phần cứng chuyên dụng độc lập, còn không thì hãy tự cầu nguyện cho sự an toàn của mình.

## 科技动态

1. **Ý tưởng lưu trữ âm thanh trên dải băng giấy mã QR**

Một nhà phát minh ở nước ngoài vừa nảy ra ý tưởng độc lạ: Liệu có thể lưu trữ âm thanh trực tiếp trên những dải băng giấy thông thường không?

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022303.webp)

Ông đã thực hiện việc mã hóa dữ liệu âm thanh của mỗi giây thành một hình mã QR, sau đó in chuỗi mã QR này liên tiếp dọc theo dải băng giấy.

Tiếp theo, ông chế tạo một thiết bị phát nhạc đặc biệt (hình dưới) với lớp vỏ bên ngoài bằng giấy cứng, bên trong trang bị cụm bánh răng truyền động kết hợp camera quét.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022304.webp)

Thiết bị phát nhạc sẽ tự động kéo dải băng giấy dịch chuyển 1 ô sau mỗi giây, camera sẽ nhận diện dữ liệu từ mã QR và chuyển đổi phát lại thành âm thanh thực tế qua loa.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022305.webp)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022306.webp)

2. **Cơ quan Thuế Hàn Quốc rò rỉ mã bảo mật ví tiền mã hóa**

Cục Thuế Quốc gia Hàn Quốc vừa thực hiện đợt truy quét các tài khoản trốn thuế và tịch thu một lượng lớn tiền mã hóa của các đối tượng vi phạm.

Cơ quan thực thi pháp luật sau đó đã tự hào đăng tải bức ảnh chụp tang vật thu giữ được lên mạng (hình dưới) như chiến tích của chiến dịch.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030202.webp)

Bức ảnh được chụp ở độ phân giải cực cao, hiển thị rõ nét một chiếc ví cứng lưu trữ tiền mã hóa kèm theo một mảnh giấy ghi tay cụm từ khôi phục mật khẩu (seed phrase) của ví đặt ngay bên cạnh.

Hậu quả lập tức diễn ra sau đó: toàn bộ số tiền mã hóa bên trong chiếc ví trị giá khoảng 4,4 triệu USD đã nhanh chóng bị rút sạch và gần như không có khả năng truy vết thu hồi.

Sự cố hy hữu này cho thấy rủi ro cực lớn trong việc quản lý tài sản mã hóa của các cơ quan chính phủ, khi chỉ cần một mắt xích nhỏ bất cẩn làm rò rỉ mật khẩu là toàn bộ tài sản sẽ bốc hơi ngay lập tức.

3. **Tư thế di chuyển của khủng long bạo chúa T-Rex**

Khủng long bạo chúa T-Rex là loài khủng long khổng lồ hung dữ nhất thời kỳ Bạch Diệp, vị vua tuyệt đối của chuỗi thức ăn thời kỳ cổ đại.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022803.webp)

Vẫn còn rất nhiều bí ẩn chưa có lời giải xoay quanh loài T-Rex này, giới khoa học bấy lâu nay vẫn chưa thể lý giải tại sao hai chi trước của loài bò sát khổng lồ này lại tiêu biến ngắn ngủn và nhỏ bé đến vậy.

Gần đây, các nhà khoa học tiếp tục phát hiện ra một tập tính thú vị khác: loài sinh vật khổng lồ nặng hàng chục tấn này thực chất lại có tư thế di chuyển và chạy bằng các đầu ngón chân (kiểu nhón chân).

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022804.webp)

Phát hiện dựa trên việc phân tích các hóa thạch dấu chân của loài T-Rex (hình dưới): phần vết chân in sâu nhất luôn tập trung ở các ngón chân trước, chứng tỏ đây là vùng chịu lực nâng đỡ trọng lượng cơ thể lớn nhất khi di chuyển.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022805.webp)

Tư thế đi nhón chân này có thể là giải pháp sinh học giúp T-Rex tăng tốc độ chạy tốt hơn khi săn mồi.

## 文章

1. [Một thủ thuật tối ưu hóa chất lượng đầu ra của mô hình AI](https://simonwillison.net/guides/agentic-engineering-patterns/hoard-things-you-know-how-to-do/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022702.webp)

Khi mô hình AI gặp khó khăn hoặc đưa ra câu trả lời kém chất lượng ở một tác vụ chuyên môn cụ thể, giải pháp xử lý là gì?

Lập trình viên nổi tiếng Simon Willison giới thiệu một giải pháp đơn giản: hãy chủ động tìm kiếm các tài liệu lý thuyết chuẩn cùng các ví dụ mã nguồn mẫu đang vận hành tốt của mảng việc đó nạp trực tiếp vào ngữ cảnh (context) đầu vào để AI tham khảo làm mẫu. Mô hình sẽ nhanh chóng học và xử lý cực tốt tác vụ tương ứng.

Do đó, hãy tích lũy và xây dựng một kho lưu trữ các giải pháp mẫu của những việc bạn am hiểu để nạp cho AI khi cần thiết.

2. [Hướng dẫn tự thiết kế một phiên bản AI của chính mình](https://luolei.org/luolei-ai) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030307.webp)

Blogger công nghệ nổi tiếng Lạc Lỗi chia sẻ chi tiết về quy trình thu thập toàn bộ dữ liệu bài viết blog, video và lịch sử bài đăng mạng xã hội suốt hơn 10 năm qua của mình để huấn luyện nên một trợ lý AI đại diện cho cá nhân phục vụ người dùng. Anh đã thử nghiệm huấn luyện trên 6 mô hình AI khác nhau để tạo ra 6 phiên bản AI phân thân độc đáo. (Đóng góp từ [@foru17](https://github.com/ruanyf/weekly/issues/9118))

3. [Những điểm lưu ý quan trọng khi sử dụng câu lệnh `scp`](https://sny.sh/hypha/blog/scp) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022802.webp)

Lệnh `scp` thường được sử dụng để truyền tải nhanh tệp tin lên máy chủ. Bài viết lưu ý cơ chế truyền tải tệp tin của lệnh này có đi kèm cấu hình phân quyền dữ liệu, và trong một số trường hợp cụ thể có thể vô tình vô hiệu hóa tính năng đăng nhập SSH từ xa vào máy chủ của bạn.

4. [Bảng so sánh năng lực hình ảnh giữa Nano Banana 2 và Seedream 5.0 Lite](https://decrypt.co/359700/image-ai-leap-google-bytedances-latest-models) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030405.webp)

Bài viết so sánh và đánh giá chi tiết về chất lượng đồ họa sinh ra từ hai mô hình sinh ảnh hiện đại nhất hiện nay: dòng Nano Banana 2 của Google và dòng Seedream 5.0 Lite của ByteDance.

5. [So sánh hiệu năng của 4 cơ chế duyệt mảng dữ liệu trong JavaScript](https://waspdev.com/articles/2026-01-01/javascript-for-of-loops-are-actually-fast#javascript_s_for_of_loops_are_actually_fast) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026011012.webp)

Bài phân tích so sánh tốc độ xử lý của 4 cú pháp vòng lặp duyệt mảng phổ biến trong JavaScript. Kết quả ghi nhận vòng lặp `for (let i = 0; i < len; i++)` truyền thống đạt tốc độ xử lý nhanh nhất, tiếp theo là vòng lặp `for-of`, cú pháp `forEach` có tốc độ khá chậm và lập trình viên được khuyến nghị nên tránh sử dụng vòng lặp `for-in` cho việc duyệt mảng.

## 工具

1. [yj_nearbyglasses](https://github.com/yjeanrenaud/yj_nearbyglasses)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030402.webp)

Ứng dụng Android mã nguồn mở hỗ trợ người dùng quét và phát hiện xem xung quanh khu vực di chuyển có thiết bị kính thông minh (smart glasses) nào đang hoạt động hay không.

2. [explain-my-curl](https://github.com/akgitrepos/explain-my-curl)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030403.webp)

Giao diện tương tác terminal hỗ trợ hiển thị giải thích chi tiết các tham số và kết quả phản hồi của câu lệnh kết nối `curl`.

3. [Pocket ID](https://github.com/pocket-id/pocket-id)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030501.webp)

Dịch vụ quản lý xác thực danh tính OIDC hỗ trợ người dùng tự triển khai lưu trữ riêng, trang bị tính năng đăng nhập không cần mật khẩu qua bảo mật Passkey. Tham khảo thêm [hướng dẫn thiết lập chi tiết](https://runtimeterror.dev/pocket-id-easy-passkey-authentication/).

4. [R2 Web](https://github.com/vikiboss/r2-web)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022703.webp)

Giao diện quản trị web client dành cho dịch vụ lưu trữ đám mây Cloudflare R2, giúp người dùng dễ dàng upload và quản lý tệp tin trực quan. (Đóng góp từ [@vikiboss](https://github.com/ruanyf/weekly/issues/9081))

5. [Voxt](https://github.com/hehehai/voxt)

Ứng dụng nhỏ dành riêng cho macOS hỗ trợ các tính năng chuyển đổi giọng nói thành văn bản và dịch thuật trực tiếp âm thanh thời gian thực. (Đóng góp từ [@hehehai](https://github.com/ruanyf/weekly/issues/9091))

6. [Cutia](https://github.com/msgbyte/cutia)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030103.webp)

Trình biên tập video chạy trên trình duyệt web mã nguồn mở chất lượng, định vị là giải pháp thay thế chạy web cho CapCut. Trải nghiệm [bản demo trực tuyến](https://cutia.msgbyte.com/). (Đóng góp từ [@moonrailgun](https://github.com/ruanyf/weekly/issues/9092))

7. [Gorse](https://github.com/gorse-io/gorse)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030201.webp)

Bộ động cơ gợi ý nội dung (recommendation engine) mã nguồn mở, hỗ trợ tự động huấn luyện trên nguồn dữ liệu sẵn có để kết xuất các gợi ý cá nhân hóa cho từng tài khoản, dễ dàng tích hợp vào nhiều nền tảng dịch vụ trực tuyến. (Đóng góp từ [@zhenghaoz](https://github.com/ruanyf/weekly/issues/9098))

8. [vscode-stylelint-plus](https://hex-ci.github.io/vscode-stylelint-plus/)

Plugin chất lượng dành cho trình soạn thảo VS Code hỗ trợ tính năng linter kiểm tra lỗi cú pháp cho các tệp tin CSS, SCSS và Less. (Đóng góp từ [@hex-ci](https://github.com/ruanyf/weekly/issues/9111))

9. [OneDroid](https://qingge.tech/onedroid/web/)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030401.webp)

Ứng dụng quản trị hệ thống Android mã nguồn mở, cung cấp đa dạng các công cụ hỗ trợ người dùng quản lý thiết bị di động hiệu quả. (Đóng góp từ [@QingGeTech](https://github.com/ruanyf/weekly/issues/9126))

10. [NoteCalc](https://github.com/2234839/TsFullStack)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030502.webp)

Giao diện ghi chú hỗ trợ tính toán công thức toán học hiển thị kết quả thời gian thực trực quan dạng WYSIWYG. (Đóng góp từ [@2234839](https://github.com/ruanyf/weekly/issues/9139))

## AI 相关

1. **Quy chuẩn AGENTS.md chặn bot AI thu thập dữ liệu (no-agents.md)**

Nếu bạn mong muốn bảo vệ kho mã nguồn repository của mình không bị các bot của các mô hình AI tự động cào dữ liệu huấn luyện, bạn có thể bổ sung các tệp tin khai báo tiêu chuẩn `AGENTS.md` và `CLAUDE.md` do dự án này cung cấp.

2. [Skills Manager](https://github.com/xingkongliang/skills-manager)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030207.webp)

Ứng dụng quản lý tệp tin Skill dành cho macOS, lưu trữ dữ liệu tại thư mục `~/.skills-manager` và hỗ trợ đồng bộ nhanh nội dung đến nhiều công cụ AI lập trình khác nhau. (Đóng góp từ [@xingkongliang](https://github.com/ruanyf/weekly/issues/9109))

Cộng đồng cũng chia sẻ một dự án quản lý tệp Skill có tính năng tương tự mang tên [Skills Manager](https://github.com/Rito-w/skills-manager) (hình dưới). (Đóng góp từ [@Rito-w](https://github.com/ruanyf/weekly/issues/9129))

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030406.webp)

3. [AGI Agent](https://github.com/agi-hub/AGIAgent)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030306.webp)

Dự án trợ lý AI cá nhân mã nguồn mở được thiết kế như giải pháp thay thế cho OpenClaw, đặc biệt được tối ưu hóa khả năng tương thích tốt với các dòng mô hình AI nội địa Trung Quốc. (Đóng góp từ [@agi-hub](https://github.com/ruanyf/weekly/issues/9115))

4. [ArXiv Daily Researcher](https://github.com/yzr278892/arxiv-daily-researcher)

Ứng dụng Python hỗ trợ tự động quét tìm kiếm các bài báo khoa học mới nhất trên ArXiv và các tạp chí khoa học uy tín theo từ khóa cấu hình trước, tự động tổng hợp thông tin để kết xuất thành báo cáo chuyên đề gửi qua nhiều kênh cho người dùng. (Đóng góp từ [@yzr278892](https://github.com/ruanyf/weekly/issues/9119))

5. [Magic Resume (魔方简历)](https://github.com/JOYCEQL/magic-resume)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030206.webp)

Trình biên tập và thiết kế hồ sơ lý lịch (CV) trực tuyến dựa trên giao diện web, hỗ trợ tích hợp sâu các tính năng tối ưu hóa nội dung bằng AI thông qua kết nối API. (Đóng góp từ [@JOYCEQL](https://github.com/ruanyf/weekly/issues/9104))

## 资源

1. [Mô hình trực quan tương tác giải thích nguyên lý MicroGPT](https://growingswe.com/blog/microgpt)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030203.webp)

MicroGPT là một đoạn mã nguồn Python siêu nhỏ chỉ khoảng 200 dòng được viết để giải thích nguyên lý vận hành cơ bản của mô hình ChatGPT. Bài viết sử dụng các hiệu ứng đồ họa hoạt họa tương tác trực quan để phân tích từng dòng code của MicroGPT, tài liệu tuyệt vời cho người mới học thuật toán AI.

2. [Bản đồ dự báo mùa hoa anh đào nở năm 2026 tại Trung Quốc](https://rogerzhu.github.io/yinghua-map/)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030305.webp)

Bản đồ tương tác hiển thị dự báo chi tiết về thời gian hoa anh đào chính thức khai hoa nở rộ tại các vùng miền trên cả nước. (Đóng góp từ [@rogerzhu](https://github.com/ruanyf/weekly/issues/9114))

3. [Dịch vụ tóm tắt bài báo khoa học Now I Get It!](https://nowigetit.us/)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030101.webp)

Người dùng chỉ cần tải lên tệp tin định dạng PDF của bài báo khoa học, hệ thống sẽ tự động chuyển đổi thành giao diện trang web tương tác giải thích toàn bộ nội dung học thuật bằng ngôn từ tiếng Anh phổ thông cực kỳ dễ hiểu. Dịch vụ hiện đang hỗ trợ hoàn toàn miễn phí.

## 图片

1. **Sự thay đổi phong cách quảng cáo của Apple sau 30 năm**

Bức ảnh quảng cáo của Apple năm 1997 với hình ảnh chân dung nhà vật lý lỗi lạc Albert Einstein:

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032011.webp)

Bức ảnh quảng cáo của Apple năm 2025 với hình ảnh chú ếch ngộ nghĩnh:

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032012.webp)

Trải qua hành trình 30 năm phát triển, thật khó để tưởng tượng hãng Apple ngày nay lại tiếp tục lựa chọn hình ảnh vĩ nhân như Einstein để làm đại diện quảng cáo.

Sự tương phản này phản ánh xu thế giải trí hóa mạnh mẽ của xã hội hiện đại, khi mọi thông điệp truyền thông ngày càng hướng tới sự hài hước, nhẹ nhàng thay vì phong cách nghiêm túc, hàn lâm của thế kỷ trước.

## 文摘

1. **Câu chuyện tôi bị sếp sa thải qua tin nhắn WhatsApp khi sếp đang đi nghỉ mát**

Tôi từng làm việc cho một doanh nghiệp tư nhân nhỏ và sếp trực tiếp của tôi cũng chính là nhà sáng lập công ty.

Cách đây một thời gian, tôi đã hoàn thành toàn bộ danh sách công việc được giao và rơi vào trạng thái rảnh rỗi. Tôi chủ động liên hệ hỏi Product Manager về dự án tiếp theo cần làm nhưng suốt hai tuần liên tiếp sau đó anh ấy vẫn không phân bổ bất kỳ đầu việc mới nào cho tôi.

Đây là một tình huống vô cùng kỳ lạ mà tôi chưa từng gặp phải trong đời: đột ngột không có việc gì để làm suốt nửa tháng trời. Tôi cảm giác chắc chắn hệ thống vận hành của công ty đang gặp vấn đề gì đó nghiêm trọng.

Do đó, tôi đã chủ động nhắn tin trực tiếp cho sếp trên Slack để hỏi về kế hoạch phân bổ công việc của mình trong tháng.

Nhiều giờ trôi qua vẫn không có phản hồi. Rồi hai ngày trôi qua, cửa sổ Slack vẫn hoàn toàn im lặng.

Sáng nay, tôi quyết định nhắn lại nội dung đó qua số tài khoản WhatsApp cá nhân của ông ấy.

Lần này ông ấy đã phản hồi nhanh chóng, chia sẻ rằng mình đang đi nghỉ mát cùng gia đình tại Hawaii nên không đăng nhập vào hệ thống Slack công việc.

Nhưng ngay sau đó, ông gửi tiếp một tin nhắn cực dài thông báo chính thức sa thải tôi.

Lý do được đưa ra là bộ phận của tôi hiện có chi phí vận hành đắt đỏ nhất công ty, trong khi tháng vừa qua doanh nghiệp lần đầu tiên ghi nhận kết quả thua lỗ, và bản thân ông đang phải vay tiền để chi trả cho khoản nợ mua nhà cá nhân, do đó việc cắt giảm nhân sự là con đường duy nhất để công ty duy trì sự sống sót.

Tôi hoàn toàn sốc trước những lời chia sẻ đó, đặc biệt khi nghĩ đến cảnh ông ấy viết những dòng tin nhắn cắt giảm chi phí này khi đang tận hưởng kỳ nghỉ dưỡng xa hoa tại Hawaii.

Trước đó, tôi thực sự đã dành nhiều sự cảm thông cho hoàn cảnh khó khăn của sếp khi chứng kiến ông chật vật xoay xở tài chính duy trì công ty. Thậm chí nếu không nghĩ đến việc ông ấy đang đi nghỉ mát tại Hawaii, tôi đã có cảm giác tự trách và ái ngại khi yêu cầu nhận lương, và thậm chí sẵn lòng làm việc không lương một thời gian để giúp công ty vượt qua khó khăn.

Nhưng sau khi đọc xong những dòng tin nhắn sa thải đó, tôi chỉ thấy sự việc thật nực cười, nực cười cho hành động chủ động nhắn tin xin việc của mình trước đó.

Tôi nhận ra mình đã bị sa thải một cách phũ phàng chỉ qua một dòng tin nhắn trên WhatsApp. Tôi đã cống hiến 4 năm thanh xuân cho công ty, nhưng khi sa thải tôi, sếp thậm chí không có đủ dũng khí tối thiểu để thực hiện một cuộc gọi video để trực tiếp nói lời chia tay một cách lịch sự.

Bức tranh thực tế đã hiện rõ: vai trò công việc của tôi bấy lâu nay thực chất chỉ là công cụ giúp ông ấy chi trả các khoản nợ mua nhà và tích lũy thêm sự giàu có. Và một khi giá trị sử dụng không còn, ông ấy không cần phải giữ sự tôn trọng hay dũng khí tối thiểu để nhìn thẳng vào mắt tôi và nói lời sa thải.

## 言论

1.

Một hiện tượng khá thú vị gần đây là các lập trình viên đã bắt đầu chủ động thực hiện những việc đáng lẽ phải làm từ lâu:

- Biên soạn các tài liệu hướng dẫn kỹ thuật ngắn gọn, mạch lạc và lưu trữ trong tệp tin `AGENTS.md`.
- Đóng gói các quy trình làm việc hữu ích dưới dạng các Skills hoặc các dịch vụ MCP.
- Tối ưu hóa định dạng kết xuất dữ liệu của các công cụ dòng lệnh (CLI) và các bài kiểm thử để cung cấp nhiều thông tin giá trị hơn.

-- Trích bài viết [《Sử dụng AI=true là một phản mẫu thiết kế (anti-pattern)》](https://keleshev.com/ai-equals-true-is-an-anti-pattern)

2.

Hệ thống GitHub gần đây thường xuyên ghi nhận các sự cố sập mạng (outages). Tôi tin nguyên nhân cốt lõi không phải do hệ thống của họ bị quá tải bởi việc chạy các đoạn code do AI viết, mà là do lập trình viên đang liên tục submit mã nguồn do AI tự sinh lên hệ thống với tần suất và quy mô vượt trội hoàn toàn so với trước đây, khiến hạ tầng của GitHub không kịp đáp ứng.

-- Chia sẻ của một thành viên trên diễn đàn Hacker News

3.

Số lượng sao yêu thích GitHub Star từng là một chỉ số uy tín để đánh giá chất lượng dự án, cho đến khi mọi người nhận ra nó thực sự là một chỉ số quá tốt (và bắt đầu tìm cách thao túng nó).

-- Chia sẻ của một thành viên trên diễn đàn Hacker News

4.

Sự hỗ trợ của công nghệ AI giúp các kỹ sư dễ dàng hoàn thiện tới 7 tính năng sản phẩm chỉ trong vòng 1 chu kỳ sprint, việc thăng tiến sự nghiệp chưa bao giờ trở nên dễ dàng đến thế.

-- Trích bài viết [《Khi tốc độ sinh code vượt trội hơn khả năng thấu hiểu của con người》](https://www.rockoder.com/beyondthecode/cognitive-debt-when-velocity-exceeds-comprehension/)

5.

Chỉ có một phương án duy nhất để ăn hết một con voi khổng lồ: đó là ăn từng miếng nhỏ một.

-- Lời khuyên nổi tiếng của Giám mục Nam Phi Desmond Tutu

## 往年回顾

[Tìm hiểu về bản chất của Token kỹ thuật số](https://www.ruanyifeng.com/blog/2025/03/weekly-issue-340.html) (#340)

[Điểm hạn chế lớn nhất của thiết bị kính Vision Pro của Apple](https://www.ruanyifeng.com/blog/2024/02/weekly-issue-290.html) (#290)

[Liệu chúng ta có thể rút ngắn chu kỳ giáo dục phổ thông không?](https://www.ruanyifeng.com/blog/2023/02/weekly-issue-240.html) (#240)

[Tầm quan trọng của tư duy đóng gói sản phẩm thương mại](https://www.ruanyifeng.com/blog/2021/12/weekly-issue-190.html) (#190)

(Hết)
