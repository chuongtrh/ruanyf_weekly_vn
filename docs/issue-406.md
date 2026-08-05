# Bản tin công nghệ hàng tuần (Số 406): Đạo khả đạo, phi thường đạo

Ghi lại nội dung công nghệ đáng chia sẻ hàng tuần, phát hành vào thứ Sáu.

Bản tin này [mã nguồn mở](https://github.com/ruanyf/weekly), hoan nghênh bạn [đóng góp](https://github.com/ruanyf/weekly/issues). Ngoài ra còn có dịch vụ [《Ai đang tuyển dụng》](https://github.com/ruanyf/weekly/issues/10950) đăng tải thông tin tuyển dụng lập trình viên. Hợp tác vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## Ảnh bìa

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072904.webp)

Trung tâm văn hóa khoa học nghệ thuật Khanh Tử (Kengzi) ở quận Bình Sơn, Thâm Quyến, vốn chỉ là một tòa nhà ba tầng bình thường, nhưng kiến trúc sư đã khéo léo thêm ba tầng hành lang cuốn, ngay lập tức biến tòa nhà này đầy cảm giác phân tầng hiện đại. ([via](https://tanghuaarchitects.com/project/%E5%9D%91%E6%A2%93%E6%96%87%E5%8C%96%E7%A7%91%E6%8A%80%E4%B8%AD%E5%BF%83/))

## Đạo khả đạo, phi thường đạo

Tuần trước (ngày 22 tháng 7), diễn đàn Xinsheng Community của tập đoàn Huawei đã chia sẻ lại bài [phỏng vấn độc quyền của Nhân Dân Nhật Báo với bà Hà Đình Ba (He Tingbo)](http://finance.people.com.cn/n1/2026/0528/c1004-40728832.html).

Bà Hà Đình Ba là Chủ tịch mảng kinh doanh bán dẫn của Huawei (HiSilicon), gần đây thu hút nhiều sự chú ý khi đề xuất định luật "Tào (τ)".

Khi chia sẻ lại bài phỏng vấn này, Huawei đã đính kèm một lời tựa do ông Nhậm Chính Phi viết, với tiêu đề [《Đạo khả đạo, phi thường đạo》](https://www.163.com/dy/article/L2IH62SK0556LMBK.html). Đoạn lời tựa này rất ngắn, chỉ có vài câu.

> Định luật τ là con đường đột phá duy nhất mà Huawei có thể lựa chọn.
> 
> Các nhà sản xuất khác có nhiều con đường để lựa chọn. Huawei, để thoát hiểm, để sinh tồn, để tiếp tục sống sót và sống tốt, hàng vạn nhân viên trong suốt 6 năm qua đã liên tục cải tiến và đi ra một con đường đã trưởng thành.
>
> Không phải để lật đổ hay thay thế bất kỳ điều gì, mà là đã tìm thấy một con đường có thể lựa chọn. Chúng tôi chọn "chỉ trình bày, không tranh luận" khi giao lưu với các đối tác cấp cao.

Ý nghĩa của đoạn này rất rõ ràng, con đường mà người khác đã đi thông, Huawei hiện tại không thể đi được, chỉ có thể tự mình nghĩ cách tìm một con đường khác, vừa dò dẫm vừa bước tiếp.

Việc con đường này đúng hay sai, khó đi hay dễ đi, đều không còn quan trọng nữa. Không đi con đường này thì chỉ có chờ chết. Một khi đã lên đường thì không cần bận tâm đến những lời bàn tán bên ngoài nữa, cứ cắm đầu tiến về phía trước, bước chân chính là câu trả lời.

Điều thú vị là tiêu đề của Nhậm Chính Phi "Đạo khả đạo, phi thường đạo" chính là câu đầu tiên trong cuốn "Đạo Đức Kinh" của Lão Tử.

Như các bạn đã biết, sách của người cổ đại không có dấu câu, nguyên văn câu này là "Đạo khả đạo phi thường đạo".

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072702.webp)

Từ xưa đến nay, cách ngắt câu được thừa nhận rộng rãi là "Đạo khả đạo, phi thường đạo", nghĩa là "Đạo mà có thể gọi được thì không phải là Đạo vĩnh cửu".

Trong thời hiện đại, có người đề xuất một cách ngắt câu khác, đó là "Đạo khả, đạo phi, thường đạo". Ngắt câu như thế này thì ý nghĩa thay đổi hoàn toàn: "Đi con đường đúng, đi con đường sai, đó mới là con đường vĩnh cửu."

Đây có lẽ chính là ý của Nhậm Chính Phi, Huawei đã thử nghiệm đủ mọi con đường, đi đúng cũng tốt (đạo khả), đi sai cũng được (đạo phi), chỉ để tìm lấy một con đường sống, đây mới là con đường không thay đổi (thường đạo).

## [Phần mềm tuần này] OpenConnector

Hôm nay tôi xin giới thiệu một cổng kết nối bảo mật mã nguồn mở [OpenConnector](https://github.com/oomol-lab/open-connector).

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072801.webp)

Nó được sử dụng đi kèm với AI Agent, chủ yếu giải quyết vấn đề ủy quyền của các công cụ tự động hóa AI (như OpenClaw).

Ví dụ, giao mật khẩu hộp thư cho công cụ AI, bạn có yên tâm không, ai có thể đảm bảo nó sẽ không làm rò rỉ mật khẩu vào ngữ cảnh? OpenConnector được sinh ra để giải quyết vấn đề này.

Nó lưu trữ nghiêm ngặt mật khẩu/thông tin xác thực ủy quyền, chịu trách nhiệm quản lý thống nhất các kết nối với các ứng dụng bên ngoài. Agent chỉ có thể lấy được nhãn tài khoản (account labels), siêu dữ liệu (metadata) và kết quả thực thi, không xảy ra rò rỉ mật khẩu, đồng thời rất thuận tiện cho việc quản lý tập trung.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072802.webp)

Người dùng chỉ cần kết nối với ứng dụng bên ngoài qua nó một lần, nó sẽ tự động lưu thông tin kết nối. Hiện tại nó đã hỗ trợ hơn 1.000 nhà cung cấp danh tính (identity providers) và hơn 10.000 dịch vụ ứng dụng.

Nó có thể được triển khai trên Cloudflare Workers hoặc Fly.io + SQLite, cũng như hỗ trợ triển khai cục bộ Node.js / Docker. Nếu thấy phiền phức, bạn có thể sử dụng trực tiếp dịch vụ đám mây SaaS của nó là [OOMOL](https://oomol.com/apps).

Nó cung cấp trang quản trị Web để xem trạng thái chạy theo thời gian thực và lịch sử gọi API. Phiên bản dành cho đội ngũ còn đi kèm quản lý quyền hạn, hỗ trợ nhóm sử dụng, một thành viên thiết lập kết nối có thể chia sẻ cho các thành viên khác.

## 科技动态 (Tin tức Công nghệ)

1、[Tên lửa bị sét đánh](https://www.163.com/dy/article/L2RLM65G0556BW7G.html)

Vào lúc 8 giờ tối ngày 23 tháng 7, Trung tâm Phóng Vệ tinh Tây Xương đã phóng tên lửa đẩy Trường Chinh 3B (Long March 3B).

47 giây sau khi cất cánh, tên lửa đã bị sét đánh trúng một cách hy hữu.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072905.webp)

Tuy nhiên, tia sét này không ảnh hưởng đến hoạt động của tên lửa, vệ tinh Thiên Liên 2 (Tianlian II) được mang theo trên tên lửa cũng được đưa vào không gian thuận lợi.

Bản thân tên lửa là một thiết bị dễ bị sét đánh, tên lửa Trường Chinh 3B được thiết kế chống sét đặc biệt, vỏ kim loại bên ngoài hoạt động như một "lồng Faraday". Cụ thể hơn, vỏ tên lửa là vật dẫn điện tốt, khi sét đánh, dòng điện sẽ chỉ chạy dọc theo bề mặt vỏ ngoài mà không xâm nhập vào các khoang bên trong.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072906.webp)

Ngoài ra, luồng lửa nhiệt độ cao ở đuôi tên lửa tương đương với một "dây tiếp đất của cột thu lôi" giúp xả dòng điện ra ngoài. Các thiết bị cơ điện bên trong tên lửa cũng được bọc trong các lớp bảo vệ chống nhiễu điện từ chuyên dụng, đảm bảo lõi thiết bị không bị cháy hỏng ngay cả khi có một lượng dòng điện nhất định xâm nhập.

Vì sét đánh là hiện tượng khí quyển, trên thực tế chỉ cần bay thêm hơn mười giây nữa, tên lửa sẽ đạt tới đỉnh của tầng khí quyển và sẽ không gặp phải sét đánh.

2、[Xe đạp trẻ em của Tesla](https://shop.tesla.com/product/balance-bike-for-kids)

Tesla đã ra mắt một mẫu xe đạp trẻ em trên trang web chính thức của mình với giá 225 USD.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072901.webp)

Thiết kế xe rất độc đáo, không có bàn đạp, và được cho là có thể tự giữ thăng bằng.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072902.webp)

Nó trông có vẻ không chứa pin, nếu như vậy, chẳng lẽ hoàn toàn phụ thuộc vào việc dùng hai chân đẩy để di chuyển, hay đây chỉ là một món đồ trưng bày không thể đạp?

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072903.webp)

Dù thế nào đi nữa, ngoại hình của chiếc xe khiến người ta phải trầm trồ, mang lại cảm giác rất giống thời kỳ đầu của Tesla.

3、[Sự phát triển của cây](https://www.instagram.com/p/DN3btHw0MKn/)

Nếu tay của bạn cứ nắm chặt một cái cây thì chuyện gì sẽ xảy ra?

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026010301.webp)

Một nghệ sĩ người Ý đã làm một thí nghiệm. Năm 2004, ông đúc một mô hình bàn tay bằng đồng và đặt nó nắm lấy một thân cây.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026010302.webp)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026010303.webp)

Kết quả là, cả cái cây vẫn tiếp tục lớn lên, ngoại trừ phần bị bàn tay nắm giữ.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026010304.webp)

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026010305.webp)

Đến năm 2018, bàn tay đã lún sâu vào bên trong thân cây, và thân cây tiếp tục phát triển bao bọc xung quanh bàn tay đó.

![](https://cdn.beekka.com/blogimg/asset/202601/bg2026010306.webp)

4、[Điều kiện xin vay vốn sinh viên](https://www.npr.org/2026/06/30/nx-s1-5835631/turner-camhi-do-no-harm-college-loans)

Hiện nay việc vào đại học ngày càng dễ dàng, và sinh viên đều có thể nộp đơn xin vay vốn sinh viên (Student Loans), dẫn đến số lượng tốt nghiệp đại học ngày càng nhiều, tìm việc làm ngày càng khó khăn.

Bộ Giáo dục Hoa Kỳ mới đây quy định, nếu sinh viên tốt nghiệp của một ngành học cụ thể có thu nhập thấp hơn người lao động cùng vị trí nhưng chưa từng học đại học, thì sinh viên học ngành đó sẽ không thể nộp đơn xin vay vốn sinh viên.

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073006.webp)

Tôi nghĩ quy định này rất có lý. Giáo dục đại học nên làm cho vị thế của người tốt nghiệp tốt lên, nếu không đạt được điều đó, thì chỉ trong trường hợp thực lực tài chính của sinh viên đủ mạnh mới nên chọn ngành đó. Điều này cũng có nghĩa là sinh viên đó không cần đến khoản vay hỗ trợ học tập.

## 文章 (Bài viết)

1、["Vẽ" Mona Lisa bằng cách sử dụng GPT-5.6, Claude, Gemini và Grok](https://www.tryai.dev/blog/ai-drawing-arena-colored-pencils-claude-gpt-grok) (Tiếng Anh)

Tác giả đã yêu cầu bốn mô hình flagship có khả năng thị giác — GPT-5.6 Sol, Claude Fable 5, Grok 4.5 và Gemini 3.6 Flash — vẽ lại bức họa nổi tiếng thế giới Mona Lisa từng nét một trên trang web.

Bản gốc

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073012.webp)

GPT-5.6 Sol

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073013.webp)

Claude Fable 5

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073014.webp)

Grok 4.5

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073015.webp)

Gemini 3.6 Flash

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073016.webp)

Đánh giá của tác giả là, GPT-5.6 Sol dẫn đầu vượt trội, Grok 4.5 đơn giản là một đống rác rưởi, hiếm khi tạo ra được bất cứ thứ gì dùng được, và Gemini 3.6 Flash chỉ tốt hơn Grok một chút.

Claude Fable 5 đứng thứ hai về mặt chất lượng, nhưng lại xếp bét về chi phí và thời gian tiêu tốn, với chi phí đắt gấp gần 20 lần so với ba mô hình còn lại.

2、[Câu chuyện về giao thức BitTorrent](https://www.xda-developers.com/the-story-of-bram-cohen-and-the-bittorrent-protocol/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025101405.webp)

Bài viết này giới thiệu câu chuyện lập trình viên người Mỹ Bram Cohen phát minh ra giao thức BitTorrent dựa trên P2P vào năm 2001.

3、[Tại sao Emoji đến từ Nhật Bản?](https://mp.weixin.qq.com/s/TyVxvHtTyDjmR2L8IXZCdw) (Tiếng Trung)

Sự ra đời của Emoji hoàn toàn là vì cước phí mạng di động cực kỳ đắt đỏ của Nhật Bản vào cuối những năm 90, cũng như tiếng Nhật có đủ loại kính ngữ, cần có cách biểu đạt tiết kiệm ký tự. (Đóng góp từ [@zuzuAndroid](https://github.com/ruanyf/weekly/issues/10931))

4、[Tôi đã làm tranh mosaic hồ cá koi từ phế thải in 3D như thế nào](https://www.instructables.com/A-Koi-Pond-Mosaic-Made-From-10-Pounds-of-3D-Printe/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073017.webp)

Quá trình in 3D tạo ra một lượng lớn rác thải nhựa, tác giả đã dùng lượng rác thải này để tạo nên một bức tranh mosaic ghép mảnh nghệ thuật.

5、[Cách thiết lập Tổ chức cấp chứng chỉ (Certificate Authority) của riêng bạn trên Linux](https://previnder.com/tls-ca-linux/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025021804.webp)

Bài viết này là một tài liệu hướng dẫn, chỉ cách thiết lập Tổ chức cấp chứng chỉ (CA) của riêng bạn trên Linux, và thêm chứng chỉ gốc (root certificate) của nó vào danh sách chứng chỉ đáng tin cậy của hệ điều hành.

## 工具 (Công cụ)

1、[Orion](https://orionbrowser.com/)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072701.webp)

Trình duyệt do công ty Kagi ra mắt, hỗ trợ máy tính và điện thoại di động, sử dụng nhân WebKit, hỗ trợ đồng thời các tiện ích mở rộng của Safari, Chrome và Firefox, cam kết bảo vệ quyền riêng tư, không thu thập dữ liệu từ xa (zero telemetry) và tích hợp sẵn trình chặn quảng cáo.

2、[Chirp](https://github.com/solst-ice/chirp)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025030503.webp)

Một công cụ mã nguồn mở dùng để gửi và nhận dữ liệu thông qua âm thanh (loa và micro).

3、[Bento Slides](https://bento.page/slides/)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073005.webp)

Trình chỉnh sửa/trình chiếu slide PowerPoint chỉ yêu cầu [một tệp HTML duy nhất](https://bento.page/).

4、[lazyrsync](https://github.com/westpoint-io/lazyrsync)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072622.webp)

Giao diện terminal bổ sung cho công cụ đồng bộ hóa file rsync. (Đóng góp từ [@pobin6](https://github.com/ruanyf/weekly/issues/10830))

5、[Birth](https://github.com/iAmCorey/birth)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072623.webp)

Công cụ quản lý các mục khởi động mã nguồn mở dành cho macOS, gộp mọi tiến trình chạy ngầm (background items), daemon và mục đăng nhập (login items) vào chung một cửa sổ, cho phép vô hiệu hóa hoặc gỡ bỏ chỉ với một cú nhấp chuột. (Đóng góp từ [@iAmCorey](https://github.com/ruanyf/weekly/issues/10842))

6、[Linux Router](https://github.com/Jaksay/Linux-Router)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072624.webp)

Biến một thiết bị chạy Debian hoặc Armbian thành một bộ định tuyến (router) và cung cấp một bảng điều khiển Web rõ ràng. (Đóng góp từ [@Jaksay](https://github.com/ruanyf/weekly/issues/10847))

7、[RepoMirror](https://github.com/wutongyuonce/RepoMirror)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072626.webp)

Một ứng dụng desktop dành cho macOS, giúp tạo bản sao mirror của các kho lưu trữ GitHub hoặc các thư mục cụ thể về máy cục bộ, giúp bạn không cần phải kiểm tra thủ công xem hàng chục dự án GitHub có bản cập nhật mới hay không. (Đóng góp từ [@wutongyuonce](https://github.com/ruanyf/weekly/issues/10851))

8、[FluxDown](https://github.com/zerx-lab/FluxDown)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072704.webp)

Trình tải xuống đa giao thức mã nguồn mở, tích hợp sẵn máy chủ MCP, có thể được gọi bởi AI Agent. (Đóng góp từ [@zerx-lab](https://github.com/ruanyf/weekly/issues/10901))

9、[米饭云盘 (Mifun Storage)](https://github.com/AndySkaura/mifun-storage)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073003.webp)

Hệ thống lưu trữ tệp tin nhỏ mã nguồn mở dựa trên Telegram Channel, thích hợp triển khai làm kho lưu trữ ảnh cá nhân / kho ảnh phục vụ viết bài Markdown. (Đóng góp từ [@AndySkaura](https://github.com/ruanyf/weekly/issues/10936#issuecomment-5115313857))

10、[StaticShield](https://github.com/wangshengithub/staticshield)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073004.webp)

Thư viện JS dùng để thêm tính năng bảo vệ bằng mật khẩu cho trang web, mã hóa trang web và yêu cầu nhập mật khẩu để truy cập. (Đóng góp từ [@wangshengithub](https://github.com/ruanyf/weekly/issues/10940#issuecomment-5117097770))

## AI 相关 (AI Liên quan)

1、[ai-disk-cleaner](https://github.com/vudsen/ai-disk-cleaner)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072703.webp)

Công cụ dọn dẹp ổ đĩa mã nguồn mở trên Windows, sử dụng AI để phân tích và xác định các file rác. (Đóng góp từ [@vudsen](https://github.com/ruanyf/weekly/issues/10900))

2、[PhysiClaw](https://github.com/physiclaw/PhysiClaw)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072627.webp)

Một hệ thống AI mã nguồn mở, người dùng cần tự mua phần cứng, có thể thao tác iPhone giống như con người bằng cách dùng camera quan sát màn hình và cánh tay robot điều khiển điện thoại. (Đóng góp từ [@physiclaw](https://github.com/ruanyf/weekly/issues/10893))

3、[Figwright](https://github.com/awdr74100/figwright)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026072625.webp)

Một máy chủ MCP giúp các AI Agent như Claude Code, Cursor, Codex thao tác trực tiếp trên Figma, có thể đọc và vẽ trực tiếp các bản thiết kế. (Đóng góp từ [@awdr74100](https://github.com/ruanyf/weekly/issues/10850))

## 资源 (Tài nguyên)

1、[How to Draw](https://www.howtodraw.ai/)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073002.webp)

Trang web cung cấp hướng dẫn vẽ từng bước cho nhiều loại động vật nhỏ khác nhau, rất thích hợp cho trẻ em sử dụng. (Đóng góp từ [@Etshop-AI](https://github.com/ruanyf/weekly/issues/10934))

2、[Hiệu ứng hoạt động cuộn trang web](https://scroll-driven-animations.style/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202607/bg2026073001.webp)

Trang web này tổng hợp nhiều hiệu ứng hoạt động cuộn trang web khác nhau, được triển khai bằng Web Animations API (WAAPI) và CSS Animations API.

3、[Học chơi cờ vây](https://online-go.com/learn-to-play-go)

![](https://cdn.beekka.com/blogimg/asset/202509/bg2025092903.webp)

Tài liệu hướng dẫn chơi cờ vây tương tác trực tuyến, giải thích chi tiết từng bài học từ cơ bản đến nâng cao.

## 图片 (Hình ảnh)

1、[Đèn chai nước](https://www.bbc.co.uk/news/magazine-23536914)

2002 năm, một kỹ sư người Brazil bị mất điện tại nhà, cả căn phòng tối đen như mực giữa ban ngày.

Anh ấy nghĩ ra một cách, tìm một chai nhựa PET đựng đồ uống trong suốt, đổ đầy nước vào bên trong.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024073005.webp)

Sau đó, anh ta khoan một cái lỗ trên mái ngói và cắm chai nhựa vào đó.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024073006.webp)

Ánh sáng mặt trời đi qua nước trong chai, khúc xạ vào trong nhà và trở thành một chiếc đèn chiếu sáng đơn giản.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024073007.webp)

Phát minh này nhanh chóng trở nên phổ biến và được nhiều người áp dụng.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024073008.webp)

Hiện tại, nó đã được sử dụng rộng rãi tại 15 quốc gia bao gồm Brazil, Philippines, Ấn Độ, Bangladesh, Tanzania, Argentina và Fiji.

## 文摘 (Văn trích)

1、[Lập trình viên giỏi nhất nhưng ít được biết đến nhất trên thế giới](https://x.com/bigaiguy/status/2063903532575752211)

Một lập trình viên người Pháp sống ẩn dật tại Paris, trong suốt 30 năm qua, chỉ tập trung viết phần mềm. Toàn bộ mạng Internet ngày nay đều phụ thuộc vào các sản phẩm của ông, nhưng rất ít người biết đến tên ông.

Mã nguồn do ông viết hỗ trợ đắc lực cho các dịch vụ video của YouTube, Netflix và TikTok, đồng thời cũng là nền tảng cho các máy chủ ảo của AWS, Google Cloud và Microsoft Azure. Ông cũng từng tạo ra kỷ lục thế giới về việc tính toán số chữ số của số Pi.

Ông không có tài khoản Twitter, cũng không thực hiện bất kỳ hoạt động marketing nào, chỉ lặng lẽ phát hành sản phẩm.

Tên của ông là Fabrice Bellard.

![](https://cdn.beekka.com/blogimg/asset/202606/bg2026062004.webp)

Ngoài lĩnh vực lập trình, hầu như không ai biết đến những kỳ tích mà ông đã tạo ra.

Ông sinh năm 1972 tại Grenoble, Pháp, tốt nghiệp trường kỹ thuật hàng đầu của Pháp — École Polytechnique (Đại học Bách khoa Paris).

Ông chưa từng đến Thung lũng Silicon, chỉ vùi đầu vào viết mã nguồn.

Năm 2000, ở tuổi 28, ông khởi động một dự án có tên FFmpeg, một framework đa phương tiện nguồn mở dùng để mã hóa, giải mã video và truyền tải luồng media. Dự án này hoàn thành một nhiệm vụ mà chưa nhà phát triển nào làm tốt trước đó. Nó xử lý tất cả các định dạng video và âm thanh hiện có trong một thư viện duy nhất và hỗ trợ mọi hệ điều hành.

Ông đã một mình dẫn dắt dự án này trong nhiều năm. Ngày nay, FFmpeg đã trở thành nền tảng của video trên internet. YouTube sử dụng nó, Netflix sử dụng nó, VLC sử dụng nó, Chrome và Firefox cũng sử dụng một phần mã nguồn của nó. Mỗi chiếc điện thoại Android, iPhone, mỗi chiếc smart TV và mọi công cụ chỉnh sửa video bạn từng chạm vào, đều có FFmpeg chạy ngầm ở tầng dưới cùng. Nếu bạn từng xem bất kỳ video nào trong 20 năm qua, thì FFmpeg chắc chắn đã xử lý nó.

Nhưng ông không dừng lại ở đó. Năm 2003, ông tạo ra QEMU, một trình mô phỏng và ảo hóa hệ điều hành. Ông đã tự mình viết QEMU cho đến phiên bản 0.7.1 năm 2005. QEMU cho phép bạn chạy bất kỳ hệ điều hành nào trên bất kỳ hệ điều hành khác.

Nó trở thành nền tảng của ảo hóa hiện đại. Trình ảo hóa nhân Linux KVM chạy trực tiếp trên QEMU. Tất cả các nhà cung cấp dịch vụ đám mây lớn như AWS, Google Cloud, Microsoft Azure và IBM Cloud đều chạy các máy ảo trên cơ sở hạ tầng được xây dựng dựa trên QEMU. QEMU là mã nguồn cơ sở hạ tầng đám mây được trích dẫn nhiều nhất trên Trái Đất.

Năm 2001, ông đã giành chiến thắng trong Cuộc thi viết code C khó hiểu quốc tế (IOCCC) nhờ một trình biên dịch C siêu nhỏ, sau này phát triển thành TCC (Tiny C Compiler). TCC có thể tự biên dịch từ mã nguồn và khởi động nhân Linux chỉ trong chưa đầy 15 giây.

Năm 2004, ông sử dụng một máy tính để bàn cá nhân và thuật toán do tự mình phát triển — công thức Bellard, để tính ra số lượng chữ số của số Pi nhiều nhất tại thời điểm đó.

Năm 2011, ông sử dụng hoàn toàn JavaScript thuần để viết một trình mô phỏng PC hoàn chỉnh, có thể chạy hệ điều hành Linux trực tiếp trong trình duyệt. Dự án này mang tên JSLinux, cho đến nay vẫn làm cho các kỹ sư kinh ngạc.

Năm 2019, ông phát hành QuickJS, một công cụ JavaScript nhỏ gọn nhưng đầy đủ tính năng, có thể đảm nhiệm những công việc mà V8 engine không làm nổi.

Năm 2021, ông phát hành NNCP, một công cụ nén dữ liệu không mất dữ liệu (lossless data compression) dựa trên mạng nơ-ron, ngay lập tức đứng đầu trong các bài kiểm tra nén văn bản quy mô lớn.

Sau đó, ông chuyển sự chú ý của mình sang các mô hình ngôn ngữ lớn (LLM). Ông đã xây dựng TextSynth Server, một máy chủ Web cung cấp REST API để chạy cục bộ các LLM.

Ông cũng phát hành ts_zip và ts_sms, các công cụ sử dụng mô hình lớn để nén văn bản, với tỷ lệ nén vượt trội so với các thuật toán truyền thống. Ông cũng phát hành TSAC, một hệ thống nén âm thanh với tốc độ bit cực thấp.

Vào tháng 12 năm 2025, ông phát hành Micro QuickJS, một JavaScript micro-engine hoàn toàn mới tách biệt với QuickJS, được thiết kế đặc biệt cho các môi trường có dung lượng bộ nhớ cực kỳ hạn chế.

Fabrice Bellard gia nhập công ty viễn thông Amarisoft vào năm 2012 và giữ chức Giám đốc Công nghệ (CTO). Công ty này phát triển phần mềm trạm phát sóng 4G và 5G cho các nhà mạng và phòng thí nghiệm trên toàn thế giới sử dụng. Ông đã vận hành công ty này trong hơn một thập kỷ, đồng thời vẫn liên tục đăng tải các dự án cá nhân trên trang chủ của mình: bellard.org.

![](https://cdn.beekka.com/blogimg/asset/202606/bg2026062005.webp)

Ông không có tài khoản Twitter, cũng không có Instagram và hầu như không nhận phỏng vấn. Trang web cá nhân của ông chỉ đơn thuần là một danh sách dự án, không có bất kỳ style thiết kế, font chữ hay bài viết marketing nào, chỉ có tiêu đề và liên kết.

Người kỹ sư Pháp kín tiếng chưa từng chuyển đến Thung lũng Silicon này đã viết nên những dòng code âm thầm vận hành mạng Internet toàn cầu. Và ông ấy vẫn đang tiếp tục phát hành sản phẩm mới.

## 言论 (Phát ngôn)

1、

> Có một số trang web thiết kế nút "Đăng nhập" (Login) nhỏ hơn nút "Đăng ký" (Register), hoặc mặc định chỉ hiển thị nút "Đăng ký".
> 
> Tôi rất ghét loại trang web như vậy, điều đó cho thấy họ ưu tiên người dùng mới hơn là làm hài lòng người dùng cũ.
> 
> -- [Độc giả Hacker News](https://news.ycombinator.com/item?id=48971030)

2、

> Nhiệm vụ của một lập trình viên con người chưa bao giờ chỉ là viết code đơn thuần, mà là giảm thiểu rủi ro cho mã nguồn khi đối mặt với sự mơ hồ, các hạn chế và thay đổi. Trước đây là như vậy, và trong thời đại AI không tự viết code này lại càng đúng như vậy.
> 
> -- [《Mã nguồn không ai đọc》](https://www.heavybit.com/library/article/write-only-code)

3、

> Tôi biết nhiều người rất thành công đã nghỉ hưu, nhưng gần đây đã quay trở lại thị trường làm việc vì những thách thức và cơ hội mà AI mang lại có sức hút không thể cưỡng lại đối với họ.
> 
> Trong vài thập kỷ qua, những ý tưởng dự án phụ rải rác của họ giờ đây bỗng nhiên trở nên hoàn toàn khả thi, có quá nhiều thứ mới mẻ đáng để khám phá và sáng tạo.
> 
> -- [Simon Willison](https://news.ycombinator.com/item?id=47152086), nhà phát triển nổi tiếng

4、

> Có người cho rằng CSS hiện tại là một đống hỗn độn vô cùng phình to. Ý kiến của tôi hoàn toàn ngược lại, CSS đang cố gắng hết sức để thể hiện đầy đủ trải nghiệm thị giác, thiết kế bố cục, dàn trang, hoạt ảnh, tương tác kỹ thuật số và một số nội dung khác dưới dạng văn bản dễ đọc đối với con người. Nó không phải phình to, mà là cực kỳ tham vọng.
> 
> -- [Eric A. Meyer](https://mastodon.social/@Meyerweb/116065151451468199), nhà phát triển web nổi tiếng

## 往年回顾 (Nhìn lại các năm trước)

[Palantir rất đáng chú ý](https://www.ruanyifeng.com/blog/2025/08/weekly-issue-359.html)（#359）

[Con dao hai lưỡi của taxi tự lái](https://www.ruanyifeng.com/blog/2024/07/weekly-issue-309.html)（#309）

[Cách sử dụng ChatGPT miễn phí](https://www.ruanyifeng.com/blog/2023/06/weekly-issue-259.html)（#259）

[Lập trình viên là những người thế nào](https://www.ruanyifeng.com/blog/2022/06/weekly-issue-209.html)（#209）

(Hết)
