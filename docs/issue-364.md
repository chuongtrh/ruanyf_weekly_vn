# Bản tin chia sẻ công nghệ (Số 364): Khối Rubik khó giải nhất thế giới

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/7674) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025083002.webp)

Dưa hấu thái lát tại một siêu thị ở Hạ Môn. (Nguồn: [Facebook](https://www.facebook.com/hxdb1234/posts/pfbid0z2PutGZHD3tWu9BDMTmYP8fqFcySML1K8PRvURUvj8QzpPN1zCtEDwrw9e5yhQnCl))

## 最难还原的魔方

Thật kỳ lạ, nhiều lập trình viên tôi quen biết trông có vẻ không có điểm chung gì, nhưng khi hỏi ra thì hóa ra ai cũng thích Rubik.

Và trình độ đều rất cao, thường không quá 3 phút là giải xong.

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025090405.webp)

Một thời gian, trong văn phòng chúng tôi có vài chiếc Rubik, lúc rảnh mọi người cứ lấy ra xoay.

Tôi từng tự hỏi: **Loại Rubik nào khó giải nhất?**

Những trạng thái Rubik khác nhau chắc chắn có độ khó khác nhau, nhưng làm sao đo lường độ khó?

Gần đây tôi tình cờ phát hiện người nước ngoài đã [nghiên cứu](https://www.solutionslookingforproblems.com/post/the-rubik-s-cube-perfect-scramble) vấn đề này từ lâu.

Họ đề xuất bộ tiêu chí định lượng: Khối Rubik khó giải nhất phải đồng thời thỏa mãn 6 điều kiện sau:

> 1. Mỗi mặt chứa đủ cả 6 màu.
> 2. Trên mỗi mặt, không màu nào xuất hiện quá 2 ô.
> 3. Trên mỗi mặt, không có 2 ô cùng màu nằm liền kề nhau.
> 4. Trên mỗi mặt, không có 2 ô cùng màu nằm trên đường chéo.
> 5. 8 ô góc không có 2 ô nào cùng màu.
> 6. Hoa văn (pattern) của mỗi mặt phải khác nhau hoàn toàn.

Điều đáng khâm phục hơn là tác giả đã viết một [chương trình C++](https://github.com/telemath/PerfectScramble) để tìm ra trạng thái Rubik khó giải nhất đó.

Rubik có tổng cộng 43.252.003.274.489.856.000 cách sắp xếp. Máy tính cá nhân của tác giả mất 5 ngày chạy mới tính xong toàn bộ.

Kết quả: **Chỉ có duy nhất một sắp xếp thỏa mãn cả 6 tiêu chí trên**.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025080310.webp)

Hình ảnh trên là trạng thái Rubik khó giải nhất thế giới.

Hình ảnh này thể hiện cả 6 mặt của khối Rubik. Vì 6 mặt có thể kết hợp ngẫu nhiên với nhau theo nhiều cách, nên tổng cộng có 48 dạng bố cục khác nhau.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025080311.webp)

## 科技动态

（1）Hàn Quốc đã triển khai **cảnh sát hologram** trong các công viên Seoul vào ban đêm.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025083011.webp)

Người đi dạo sẽ thấy một hình ảnh cảnh sát to bằng người thật đứng giữa bụi cây trong công viên, còn có thể nói chuyện và thực hiện các cử động. Từ xa, gần như không phân biệt được đây là hình chiếu.

Cảnh sát cho biết trong thời gian thiết bị hoạt động, tỷ lệ tội phạm trong công viên giảm khoảng 22%.

（2）Một lập trình viên người Mỹ đã cải tạo một chiếc máy pha cà phê cũ thành **"máy tính kiêm máy pha cà phê"** (coffee maker PC).

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025080201.webp)

Thiết bị này vừa có thể dùng như máy tính, vừa có thể dùng như máy pha cà phê — tất cả chức năng của cả hai đều hoạt động đầy đủ.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025080202.webp)

Thách thức lớn nhất là máy pha cà phê sản sinh hơi nước nhiệt độ cao, trong khi máy tính không thể tiếp xúc nước và cần tản nhiệt. Hai thứ đặt cạnh nhau khiến máy tính rất khó hoạt động ổn định.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025080203.webp)

（3）**Meta** vừa phát minh một **vòng đeo tay điều khiển máy tính**.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025072802.webp)

Chiếc vòng tay có kích thước như đồng hồ, được cho là có thể thay thế chuột và thậm chí cả bút cảm ứng để điều khiển máy tính.

Nguyên lý hoạt động rất mới lạ: Khi ngón tay và lòng bàn tay cử động, cơ bắp tạo ra tín hiệu điện. Vòng tay đọc được tín hiệu điện đó và nhận diện ý định của cử chỉ.

（4）**Lưu trữ năng lượng trong mỏ khai thác**

Phần Lan có một mỏ khai thác bỏ hoang sâu 1.400 mét. Một công ty Anh đang lên kế hoạch biến nó thành pin lưu trữ năng lượng.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021102.webp)

Ý tưởng rất đơn giản: Lắp đặt hệ thống cần cẩu treo vật nặng trong mỏ. Điện dư thừa được dùng để kéo vật nặng lên cao; khi cần điện, vật nặng được thả chậm xuống, giải phóng thế năng trọng lực để kéo máy phát điện tuabin.

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021103.webp)

Nếu phương pháp này khả thi, các mỏ khai thác bỏ hoang có thể được tái sử dụng làm kho lưu trữ năng lượng.

（5）**Quảng cáo trên bản đồ**

Google Maps gần đây xuất hiện một hình thức quảng cáo mới.

Khi bạn đang dùng chức năng dẫn đường, bỗng nhiên một cửa sổ bật lên (hình dưới) gợi ý bạn có thể dừng lại ở một địa điểm nào đó trên đường.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024070902.webp)

Hãy thử tưởng tượng: Trong tương lai, tuyến đường dẫn đường có thể xuất hiện hàng loạt "điểm check-in" — chỉ cần bạn vào cửa hàng và check-in bằng điện thoại là nhận được phần thưởng hoặc mã giảm giá.

## 文章

1、[Xác thực bot của Cloudflare](https://developers.cloudflare.com/bots/reference/bot-verification/web-bot-auth/) (tiếng Anh)

Cloudflare với tư cách là nhà cung cấp CDN lớn nhất thế giới đã ra mắt hệ thống xác thực bot. Muốn thu thập dữ liệu (crawl) các trang web do Cloudflare lưu trữ, bạn phải đăng ký khóa công khai, sau đó mỗi request phải kèm theo chữ ký số.

2、[Làm kỹ sư tại Anduril](https://joincolossus.com/article/the-amusement-park-for-engineers/) (tiếng Anh)

Anduril là công ty công nghệ quốc phòng mới nổi của Mỹ, chuyên về ứng dụng quân sự của drone. Người sáng lập chính là nhà sáng lập kính AR Oculus, tự tuyên bố sứ mệnh bảo vệ nước Mỹ bằng drone.

Bài viết do kỹ sư của họ giới thiệu về tình hình nghiên cứu phát triển nội bộ với nhiều chi tiết thú vị — đáng đọc.

3、[Khi nào nên dùng database thay vì cache](https://avi.im/blag/2025/db-cache/) (tiếng Anh)

Tác giả chia sẻ quan điểm về khi nào nên truy vấn trực tiếp database, khi nào nên dùng cache, và ưu nhược điểm của cache so với database.

4、[Chúng tôi đặt lập trình AI vào một vòng lặp while](https://github.com/repomirrorhq/repomirror/blob/main/repomirror.md) (tiếng Anh)

Tác giả viết một đoạn lệnh cho AI tự tạo code, tự phát hiện lỗi và tự tạo PR để sửa. Sau đó đặt đoạn lệnh này vào vòng lặp `while` rồi đi ngủ. Sáng hôm sau thức dậy kiểm tra tiến độ của AI. (Spoiler: Một đêm, AI đã tiêu tốn 800 đô la.)

5、[Bộ công cụ Python của tôi](https://www.cesarsotovalero.net/blog/i-am-switching-to-python-and-actually-liking-it.html) (tiếng Anh)

Tác giả là người mới học Python và giới thiệu các công cụ phát triển cơ bản mà họ đang sử dụng như uv, ruff, ty...

6、[Sự khác biệt giữa CPU AMD và Intel](https://www.xda-developers.com/differences-between-amd-and-intel-cpus/) (tiếng Anh)

Cả AMD và Intel đều sản xuất CPU x86, dù là sản phẩm cùng loại nhưng có nhiều điểm khác biệt về kiến trúc. Bài viết phân tích chi tiết những khác biệt đó.

## 工具

1、[sping](https://dseltzer.gitlab.io/sping/)

Phiên bản nâng cấp của lệnh `ping`: Hiển thị độ trễ của từng gói tin dưới dạng đồ thị trực tiếp ngay trên terminal.

2、[Beszel](https://github.com/henrygd/beszel)

Công cụ giám sát máy chủ nhẹ, có giao diện web trực quan. Xem thêm [bài giới thiệu](https://www.xda-developers.com/beszel-feature/).

3、[WinApps](https://github.com/winapps-org/winapps)

Công cụ chạy ứng dụng Windows trên hệ thống Linux bằng cách tự động khởi động một máy ảo để chạy — khác với Wine (mô phỏng Windows API). Có thêm công cụ tương tự là [WinBoat](https://github.com/TibixDev/winboat).

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025090412.webp)

4、[YouTube TUI](https://github.com/Siriusmart/youtube-tui)

Client YouTube chạy trên terminal, cho phép thao tác YouTube hoàn toàn từ dòng lệnh.

5、[LabPlot](https://labplot.org/)

Phần mềm desktop trực quan hóa dữ liệu mạnh mẽ, chuyển đổi dataset thành nhiều loại biểu đồ phong phú.

6、[gitlab-to-github](https://github.com/wuuashen/gitlab-to-github)

Script Python giúp di chuyển toàn bộ repository từ GitLab sang GitHub chỉ với một lệnh. (Đóng góp từ [@wuuashen](https://github.com/wuuashen/gitlab-to-github))

7、[Telegram Ad Blocker Bot (Bot chặn quảng cáo Telegram)](https://github.com/ramsayleung/bayes_spam_sniper)

Bot Telegram mã nguồn mở sử dụng thuật toán Bayes để tự động chặn các bài đăng quảng cáo trong nhóm. Xem thêm [bài giới thiệu của tác giả](https://ramsayleung.github.io/zh/post/2025/%E4%B8%80%E4%B8%AA%E8%87%AA%E5%AD%A6%E4%B9%A0%E7%9A%84telegram%E5%B9%BF%E5%91%8A%E6%8B%A6%E6%88%AA%E6%9C%BA%E5%99%A8%E4%BA%BA/). (Đóng góp từ [@ramsayleung](https://github.com/ruanyf/weekly/issues/7686))

8、[Foxel](https://github.com/DrizzleTime/Foxel)

Ổ đĩa đám mây riêng tư mã nguồn mở, hỗ trợ tìm kiếm ngữ nghĩa bằng AI. (Đóng góp từ [@DrizzleTime](https://github.com/ruanyf/weekly/issues/7687))

9、[StoryMotion](https://storymotion.video/)

Trình biên tập hoạt hình chạy trên web để tạo các animation phong cách vẽ tay Excalidraw nhúng được vào trang web, rất phù hợp cho các bài thuyết trình. (Đóng góp từ [@chunrapeepat](https://github.com/ruanyf/weekly/issues/7695))

10、[Website Screenshot Online](https://websitescreenshot.online/zh-CN)

Dịch vụ chụp ảnh màn hình trang web trực tuyến miễn phí: Nhập URL, nhận về ảnh chụp màn hình trang đó. Cũng cung cấp [công cụ quay video cuộn trang](https://websitescreenshot.online/zh-CN/tools/record-website-video). (Đóng góp từ [@cryptobanksy](https://github.com/ruanyf/weekly/issues/7705))

## AI 相关

1、[Công cụ AI tóm tắt sách theo chương](https://github.com/SSShooter/ebook-to-mindmap)

Ứng dụng web phân tách sách điện tử (EPUB và PDF) theo từng chương, sử dụng AI tạo bản tóm tắt văn bản và sơ đồ tư duy cho mỗi chương. Cần người dùng cung cấp API key của mô hình AI. (Đóng góp từ [@SSShooter](https://github.com/ruanyf/weekly/issues/7660))

2、[VIVY](https://github.com/liriliri/vivy)

Client desktop cho mô hình tạo ảnh từ văn bản Stable Diffusion. (Đóng góp từ [@surunzi](https://github.com/ruanyf/weekly/issues/7673))

3、[ApeRAG](https://github.com/apecloud/ApeRAG)

Nền tảng RAG (Retrieval-Augmented Generation) mã nguồn mở, kết hợp Graph RAG, tìm kiếm vector và tìm kiếm toàn văn bản với AI agent. (Đóng góp từ [@earayu](https://github.com/ruanyf/weekly/issues/7690))

4、[AI Video Transcriber](https://github.com/wendy7756/AI-Video-Transcriber)

Công cụ AI chuyển đổi giọng nói thành văn bản, dịch thuật và tóm tắt video, hỗ trợ hơn 30 nền tảng bao gồm YouTube, TikTok, Bilibili. Mã nguồn mở, cần tự triển khai frontend và backend. (Đóng góp từ [@wendy7756](https://github.com/ruanyf/weekly/issues/7678))

## 资源

1、[OpenAnimation](https://github.com/orispok/OpenAnimationApp)

Kho lưu trữ chuyên tổng hợp các animation dựa trên định dạng Lottie từ nhiều nguồn khác nhau.

2、[Jujutsu Beginner Tutorial (Hướng dẫn Jujutsu cho người mới)](https://jj-for-everyone.github.io/)

Jujutsu là hệ thống quản lý mã nguồn mới nổi, tự nhận là dễ dùng và dễ hiểu hơn Git. Tài liệu hướng dẫn tiếng Anh này được viết dành cho người hoàn toàn chưa biết Git.

3、[50 chiếc bàn phím trong bộ sưu tập của tôi](https://aresluna.org/50-keyboards-from-my-collection/)

Tác giả là một nhà sưu tầm bàn phím nước ngoài, liệt kê 50 chiếc bàn phím kỳ lạ nhất trong bộ sưu tập của mình.

Ví dụ, chiếc bàn phím dưới được thiết kế để dùng theo chiều đứng, có gương đi kèm để bạn nhìn thấy các phím khi gõ:

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025090408.webp)

Hay bàn phím gắn trên găng tay, dùng tay còn lại để gõ:

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025090409.webp)

Và một bàn phím có tất cả keycap có thể thay thế bất cứ lúc nào:

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025090410.webp)

## 图片

1、[Bên trong các nhạc cụ](https://www.dpreview.com/photography/5400934096/probe-lenses-and-focus-stacking-the-secrets-to-incredible-photos-taken-inside-instruments)

Một nhạc sĩ nước ngoài nảy ra ý tưởng: Hằng ngày chúng ta chỉ nhìn bên ngoài nhạc cụ, thế thì bên trong trông ra sao?

Ông chụp một loạt ảnh bên trong các nhạc cụ, mang lại trải nghiệm thị giác hoàn toàn khác lạ — như đang bước vào bên trong những công trình kiến trúc kỳ lạ.

**Đàn organ ống:**

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060110.webp)

**Đàn violin:**

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060111.webp)

**Đàn piano:**

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060112.webp)

**Đàn cello:**

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060113.webp)

## 文摘

1、**Tại sao Facebook không giữ được các nhà khoa học**

Gần đây Facebook đầu tư mạnh tuyển dụng nhiều nhân tài AI, nhưng không ít người chỉ làm một thời gian ngắn rồi xin nghỉ. Tại sao?

Một cựu nhân viên đưa ra lý giải, cho rằng điều này liên quan trực tiếp đến sứ mệnh của công ty.

Sứ mệnh của Facebook là "kết nối mọi người" (connect everyone) — không liên quan trực tiếp đến AI. Dù nội bộ có nhiều nhà nghiên cứu, hướng nghiên cứu chủ yếu là thuật toán xếp hạng và phân tích dữ liệu lớn. Lịch sử công ty không có nền tảng nghiên cứu AI.

Hơn nữa, các nhà nghiên cứu không được coi trọng trong văn hóa nội bộ Facebook.

Nhiều nhà nghiên cứu được tuyển về vốn có không gian tự do khám phá tại học viện hay Google/DeepMind, có thể làm nghiên cứu lâu dài và tiên phong. Khi vào Facebook, nghiên cứu AI của họ bị yêu cầu phục vụ các mục tiêu kinh doanh ngắn hạn như quảng cáo, hệ thống đề xuất và kiểm duyệt nội dung. Các nhà nghiên cứu dễ cảm thấy thiếu tầm nhìn dài hạn hay hướng đột phá thực sự.

Facebook về bản chất là công ty internet tiêu dùng vận hành theo triết lý "di chuyển nhanh" (move fast), nhấn mạnh triển khai nhanh và thúc đẩy kết quả kinh doanh.

Gien đó khiến các nhà nghiên cứu cảm thấy thiếu môi trường học thuật và khó duy trì danh tiếng trong cộng đồng đồng nghiệp.

Đồng thời, bộ phận nghiên cứu và sản phẩm của Facebook tách biệt nghiêm trọng — kết quả nghiên cứu khó trực tiếp ứng dụng vào sản phẩm, và nhóm sản phẩm không hoàn toàn hiểu giá trị của nghiên cứu.

Nhiều nhà khoa học vì vậy cảm thấy không thể tạo ra đổi mới và thành tích thực sự tại Facebook, hằng ngày chỉ bận rộn cho công việc kinh doanh, cuối cùng lựa chọn rời đi.

Điều này cho thấy các công ty lớn chưa hẳn có thể độc quyền nhân tài bằng tiền bạc. Nếu các công ty nhỏ thực sự đang làm sản phẩm mang tính đột phá, họ có cơ hội lớn để thu hút nhân tài tốt.

## 言论

1、

Một nghiên cứu Mỹ phát hiện AI tác động tiêu cực nhất đến cơ hội việc làm của sinh viên tốt nghiệp từ các trường đại học bình thường, trong khi sinh viên các trường danh tiếng như Harvard hay MIT gần như không bị ảnh hưởng.

AI đang đẩy nhanh sự mất giá trị của bằng cấp từ các trường thường.

-- *Trích bài viết 《Tác động của AI lên thị trường lao động》*

2、

Chạy các ứng dụng AI trên máy tính cá nhân của bạn có ba nguy cơ lớn: Chúng có thể truy cập dữ liệu riêng tư của bạn, có thể tải nội dung không đáng tin cậy, và có thể thực hiện giao tiếp với bên ngoài.

-- *Simon Willison*

3、

Trung Quốc có khái niệm "吃苦" (chịu khổ / rèn luyện qua gian khó). Mỹ không có khái niệm tương đương này.

-- *Độc giả Hacker News*

4、

Vibe coding thực sự rất thú vị — bạn chỉ cần suy nghĩ ý tưởng, không cần tự code. Sau khi dùng thử tôi mới nhận ra, đây mới thực sự là điều tôi yêu thích.

-- *Trích bài viết 《Trải nghiệm vibe coding của một nhà đầu tư mạo hiểm》*

5、

Trò chơi SEO (tối ưu hóa công cụ tìm kiếm) đã kết thúc từ lâu.

Đa số mọi người vẫn đang cật lực theo đuổi thứ hạng Google, nhưng người dùng thực tế đã rời khỏi Google từ lâu. Hiện tại chỉ còn 27% lượng tìm kiếm diễn ra ở đó; 73% còn lại xảy ra trên TikTok, Amazon, Reddit, YouTube và thậm chí ChatGPT.

-- *Neil Patel, tác giả bán chạy người Mỹ*

## 往年回顾

- Số #317: [Ngụ ngôn về con lừa, con hổ và con sư tử](https://www.ruanyifeng.com/blog/2024/09/weekly-issue-317.html)
- Số #267: [Mùa xuân của 5G đã đến](https://www.ruanyifeng.com/blog/2023/08/weekly-issue-267.html)
- Số #217: [NEOM — Thành phố tương lai của Saudi Arabia](https://www.ruanyifeng.com/blog/2022/08/weekly-issue-217.html)
- Số #167: [Trình chặn quảng cáo đang đi quá giới hạn](https://www.ruanyifeng.com/blog/2021/07/weekly-issue-167.html)

(Hết)
