# Bản tin công nghệ hàng tuần (Số 415): Phiên bản 3D của "Những thành phố vô hình"

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/12009) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101524.webp)

Bảo tàng mỹ thuật tại khu nghỉ dưỡng Hồ Tử Sơn, Hàm Ninh, Hồ Bắc. ([via](https://www.instagram.com/p/DTbQ9FUDea-/))

## 3D 版《看不见的城市》

Nhà văn người Ý Italo Calvino có một cuốn tiểu thuyết kỳ ảo trứ danh mang tên *Những thành phố vô hình*.

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101516.webp)

Tác phẩm kể về nhà thám hiểm Marco Polo tường thuật cho vị hoàng đế Nguyên triều Hốt Tất Liệt đã về già nghe về 55 thành phố mà ông từng đi qua trong chuyến viễn du.

Những thành phố này không hề có tranh vẽ hay sa bàn mô hình, mà chỉ được tái hiện qua những dòng miêu tả giàu chất thơ, vì vậy mới được gọi là "những thành phố vô hình". Chẳng hạn có một thành phố tên là Irene, Marco Polo miêu tả thế này:

> "Khi đèn thắp sáng, nếu bạn đứng ở rìa cao nguyên ghé mắt nhìn ra ngoài, thành phố bạn thấy chính là Irene. Xuyên qua bầu không khí trong vắt, nó trải ra dưới chân bạn một sắc hồng nhạt từ xa xăm.
> 
> Có những nơi cửa sổ san sát nhau, trong những con hẻm lờ mờ ánh sáng đèn thưa dần, trong các khu vườn là bóng tối đặc quánh, trên các ngọn tháp rực lên ánh lửa tín hiệu; nếu đêm có sương mù, luồng sáng mờ ảo ấy sẽ phồng căng lên hệt như một miếng bọt biển hút no sữa."

Có người nảy ra ý tưởng đưa toàn bộ những đoạn miêu tả này vào mô hình AI để xây dựng [phiên bản 3D trực quan](https://quesma.com/blog/invisible-cities-one-shot/) cho cả 55 thành phố. Anh đã thử nghiệm song song với hai mô hình GPT-6 Astra và Claude Opus 5.5.

Kết quả cho thấy phiên bản dựng bởi Claude Opus 5.5 ([bản tương tác](https://p.migdal.pl/invisible-cities-opus-5.5/), [mã nguồn](https://github.com/stared/invisible-cities-opus-5.5)) vượt trội hơn hẳn so với phiên bản của GPT-6 Astra ([bản tương tác](https://p.migdal.pl/invisible-cities-astra/), [mã nguồn](https://github.com/stared/invisible-cities-astra)).

Lấy thành phố Irene làm ví dụ, đây là phiên bản do GPT-6 Astra tạo ra:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101517.webp)

Thành phố Irene 3D này hoàn toàn không toát lên được ý vị "vạn ánh đèn đêm lung linh" như nguyên tác. Trên thực tế cả 55 thành phố do GPT-6 Astra tạo ra trông đều na ná nhau, rập khuôn một kiểu như hình dưới:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101518.webp)

Trong khi đó, Irene do Claude Opus 5.5 tạo ra lại mang một diện mạo hoàn toàn khác biệt:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101519.webp)

Mô hình đã tái hiện trung thực góc nhìn từ trên cao, nơi ánh sáng hồng mờ ảo của thành phố "phồng căng lên hệt như miếng bọt biển hút no sữa":

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101520.webp)

Trong *Những thành phố vô hình*, đoạn văn tôi tâm đắc nhất là miêu tả về thành phố Isidora:

> "Con người rong ruổi nơi hoang địa bấy lâu, ắt hẳn khao khát được đặt chân tới thành phố.
>
> Rồi cuối cùng chàng cũng tới Isidora, nơi các tòa kiến trúc có những chiếc cầu thang xoắn ốc khảm đầy vỏ sò xoắn, nơi người ta chế tác những chiếc kính viễn vọng và đàn vĩ cầm hoàn hảo, nơi lữ khách ngoại quốc khi do dự trước hai người phụ nữ thì luôn tình cờ gặp gỡ người phụ nữ thứ ba, nơi những trận đá gà biến thành những cuộc ẩu đả đẫm máu của phường cờ bạc.
>
> Khi ngóng trông về thành phố, trong tâm trí chàng nghĩ chính là những điều đó. Bởi vậy, Isidora chính là thành phố trong mơ của chàng: chỉ duy nhất có một điều khác biệt.
>
> Trong thành phố mơ ước, chàng là một thanh niên trẻ trung; nhưng khi chàng thực sự đặt chân đến Isidora, chàng đã là một ông lão bạc đầu. Dưới chân tường quảng trường, những cụ già ngồi lặng nhìn lớp trẻ rảo bước qua; chàng ngồi xuống cạnh họ, vai kề vai. Dục vọng giờ đây đã trở thành ký ức."

Thành phố Isidora do GPT-6 Astra tạo ra hoàn toàn nhạt nhòa, không có điểm nhấn:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101521.webp)

Còn Isidora do Claude Opus 5.5 tạo ra không những tuyệt đẹp mà còn tái hiện chân thực từng chi tiết của nguyên tác:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101522.webp)

Nó thậm chí còn tạo cả hình ảnh những cụ già ngồi lặng lẽ bên bờ quảng trường:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101523.webp)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101525.webp)

## AI 的 3D 建模

Các mô hình AI lớn hiện nay sở hữu năng lực mô hình hóa 3D rất mạnh mẽ, hàng loạt dự án dựng cảnh 3D nhờ đó liên tục ra đời.

Các dự án này dùng thư viện Three.js để dựng các bối cảnh không gian ảo; hình ảnh 3D hiển thị mượt mà trên trình duyệt, hỗ trợ phóng to thu nhỏ, xoay góc nhìn và di chuyển tự do. Nhược điểm duy nhất là dung lượng asset khá lớn nên thời gian tải trang ban đầu hơi lâu.

Bên cạnh dự án *Những thành phố vô hình* nêu trên, dưới đây là hai tác phẩm xuất sắc do bạn billpwchan đóng góp, mời các bạn cùng trải nghiệm:

（1）[Anh Hoa Huyễn Tưởng](https://github.com/billpwchan/sakura-fantasy) (Sakura Fantasy): Ngồi thuyền chèo tay xuôi dòng kênh rực rỡ hoa anh đào nở rộ; có thể tùy ý chuyển đổi 4 mùa xuân hạ thu đông, sáng tối ban ngày hay trời mưa tuyết. ([#12067](https://github.com/ruanyf/weekly/issues/12067))

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101006.webp)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101526.webp)

（2）[Cyber Kowloon](https://github.com/billpwchan/neon-zenith): Mô hình hóa toàn bộ bán đảo Cửu Long (Hồng Kông), tái hiện chân thực 9.373 tòa nhà cao tầng theo phong cách cyberpunk. ([#12103](https://github.com/ruanyf/weekly/issues/12103))

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101005.webp)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101527.webp)

## 灯泡计算机

Máy tính của tương lai sẽ có hình hài như thế nào? Có người đưa ra ý tưởng táo bạo: nó có thể là một [chiếc bóng đèn](https://lightbulbcomputer.com/).

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101505.webp)

Thiết bị kết hợp công nghệ thị giác máy tính và máy chiếu mini tích hợp ngay trong đuôi bóng đèn: vừa có thể quét quang cảnh 360 độ xung quanh, vừa có thể chiếu giao diện thông tin lên bất kỳ bề mặt vật thể nào.

Chẳng hạn khi nấu ăn, nó có thể chiếu công thức món ăn ngay lên bức tường trước mặt bạn:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101506.webp)

Bạn có thể tương tác trực tiếp với hình chiếu bằng cử chỉ tay hoặc giọng nói, hệ thống đều nhận dạng chuẩn xác:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101507.webp)

Khi bạn chỉ ngón tay vào một trang sách, nó sẽ tự động nhận diện chữ (OCR):

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101508.webp)

Nó có thể chiếu bản đồ, album ảnh hay trò chơi trực tiếp xuống mặt bàn làm việc, bạn chỉ việc thao tác trên mặt bàn:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101509.webp)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101510.webp)

Chỉ cần vung tay thao tác lên bức tường là có thể điều khiển toàn bộ thiết bị điện gia dụng trong nhà:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101512.webp)

Bạn muốn tìm hiểu thông tin địa lý, bóng đèn sẽ chiếu vị trí và menu tương tác lên tấm bản đồ treo tường:

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101513.webp)

## Deno 项目结束了

Tuần trước, Deno chính thức [tuyên bố](https://deno.com/blog/cloudflare) được Cloudflare mua lại, trong vòng một năm tới sẽ chỉ phát hành các bản vá lỗi và cập nhật bảo mật, sau đó dự án sẽ chính thức khép lại hành trình của mình.

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101514.webp)

Nhớ lại ngày Deno mới chào đời, biết bao lời tuyên bố đao to búa lớn về việc sẽ lật đổ và thay đổi những bất cập cố hữu của Node.js: từ mớ bòng bong dependency cồng kềnh, thiếu hệ thống phân quyền bảo mật, đến việc không hỗ trợ native TypeScript...

Deno đã liên tục đổi mới và phần nào tiến rất gần đến các mục tiêu đó, nhưng rốt cuộc vẫn phải ngậm ngùi rời sân khấu, để lại bao tiếc nuối cho cộng đồng.

Thực tế kết cục của Deno đã được định đoạt từ năm 2024 khi họ ra mắt phiên bản 2.0 với định hướng tương thích diện rộng với Node.js. Điều này đồng nghĩa với việc họ đã mất niềm tin vào việc đi con đường riêng của mình: không còn tham vọng đánh bại Node.js nữa, mà chuyển sang mục tiêu làm sao để code của người dùng chạy được trên Deno mà không cần sửa đổi gì.

Thế nhưng nếu người ta đã có thể chạy ngon lành trên Node.js rồi, thì hà cớ gì phải đổi sang một runtime chỉ nhằm mục đích bắt chước hành vi của Node.js?

Lần này, nhà sáng lập Ryan Dahl cũng [thẳng thắn chia sẻ](https://news.ycombinator.com/item?id=50019911#50023277) chính lý do này đã khiến ông quyết định buông tay với Deno:

> "Tôi từng dồn trọn tâm huyết vào Deno, dành cho nó nhiều công sức nhất. Nhưng giờ đây tôi nhận ra rằng đó không còn là nơi tôi có thể phát huy giá trị lớn nhất của mình nữa.
>
> Deno có những ý tưởng rất tuyệt vời, thiết kế kỹ thuật của nó rất chuẩn mực, nhưng rốt cuộc nó không giải quyết được bất kỳ vấn đề thực sự trọng đại nào. Nó đã bị lực hấp dẫn của tính tương thích Node.js kéo chặt lại, buộc phải vận hành rập khuôn theo đúng quỹ đạo của Node.js.
>
> Tại sao lại phải tái hiện lại một Node.js khác làm gì? Node.js hiện tại vốn đang chạy rất tốt. Chỉ nâng cao một chút hiệu năng, trải nghiệm người dùng hay tính bảo mật là chưa đủ để tạo nên một cuộc cách mạng."

## 文章

1. [Cách tôi bỏ ra 600 USD để huấn luyện mô hình quyết định kiểu Jev](https://deskmind.dev/zh/blog/launch/) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101004.webp)

Tác giả mất 3 tuần, khoảng 600 USD và 20 vòng huấn luyện (epoch) để fine-tune hai mô hình nhỏ trên nền Qwen3.5 0.8B và 4B, giúp chúng thay thế người dùng thao tác trực tiếp trên máy Mac: nhìn màn hình, quyết định thao tác tiếp theo, click chuột và gõ phím hoàn toàn offline, không phụ thuộc đám mây. (Đóng góp từ [@gxcsoccer](https://github.com/ruanyf/weekly/issues/12102))

2. [Viết code cho tên lửa, vì sao tuyệt đối cấm cấp phát bộ nhớ động?](https://mp.weixin.qq.com/s/RL8w75YfXQrRubSLJHnSVA) (tiếng Trung)

Quy chuẩn lập trình C cho vũ khí quân sự của tập đoàn Lockheed Martin có một điều khoản ngắn gọn nhưng giọng điệu nghiêm khắc đến rợn người: nghiêm cấm sử dụng các lệnh cấp phát bộ nhớ động như `malloc`, `free`, `new` và `delete`. Nguyên nhân sâu xa là gì? (Đóng góp từ [@zuzuAndroid](https://github.com/ruanyf/weekly/issues/12134))

3. [Làm thế nào để trang web do AI tạo trông như tác phẩm của nhà thiết kế chuyên nghiệp](https://railcode.dev/blog/vibe-coded-website) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100515.webp)

Tác giả chia sẻ kinh nghiệm và kỹ thuật prompt để biến các trang web do AI sinh ra (hình trên) trông chỉn chu, tinh tế hệt như tác phẩm do con người thiết kế.

4. [Tại sao không có điện thoại chạy Linux](https://amosbbatto.wordpress.com/2026/10/05/linux-phones-alternative/) (tiếng Anh)

Bài phân tích sâu sắc giải thích lý do vì sao thị trường smartphone chỉ tồn tại Apple và Android mà vắng bóng hệ điều hành Linux.

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101412.webp)

Nguyên nhân cốt lõi là thiếu chip SoC (hệ thống trên một vi mạch) dành riêng cho Linux: trong khi Apple và Android có thể gom toàn bộ các cụm chip vào một SoC duy nhất, thì điện thoại Linux buộc phải ghép nối các chip rời rạc, dẫn đến thân máy cồng kềnh, ngốn pin, giá thành đắt đỏ và hiệu năng yếu.

Lựa chọn khả dĩ duy nhất hiện nay là chip RK3588S của Rockchip; dù là con chip đã ra mắt từ vài năm trước nhưng nó đủ sức đáp ứng cho một chiếc điện thoại Linux phục vụ nhu cầu cơ bản.

5. [Vi xử lý AMD làm thế nào để tăng tốc 50% chỉ trong hai năm?](https://lemire.me/blog/2026/09/18/how-did-amd-ryzen-get-50-faster-in-two-years/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202609/bg2026093003.webp)

Nhiều người có ấn tượng rằng CPU những năm gần đây dậm chân tại chỗ. Thế nhưng dòng CPU AMD Ryzen 7 phiên bản 2024 có điểm hiệu năng vượt tới 50% so với phiên bản năm 2022. Bài viết phân tích ngắn gọn bí quyết đằng sau bước nhảy vọt này.

6. [Người làm công ăn lương làm thế nào để tích lũy của cải](https://asheradeniyi.com/2026/04/10/how-to-build-wealth-as-a-career-person/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101504.webp)

Một bài viết phi kỹ thuật. Nhiều người quan niệm chỉ có khởi nghiệp mới mong làm giàu; bài viết này khẳng định người làm công ăn lương hoàn toàn có thể xây dựng tài sản bền vững nếu tuân thủ nghiêm ngặt các nguyên tắc tài chính.

## 工具

1. [REA](https://github.com/morluto/rea)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101301.webp)

Dự án gây bão toàn cầu gần đây trên GitHub với gần 200.000 sao: dùng AI để dịch ngược (reverse engineering) file nhị phân của ứng dụng gốc và viết lại thành một phiên bản mã nguồn mới hoàn toàn.
Trước khả năng AI dịch ngược và tái tạo phần mềm từ mã nhị phân quá dễ dàng, cư dân mạng [bình luận](https://news.ycombinator.com/item?id=50062172): "Điều này sẽ khiến mọi phần mềm trong tương lai đều phải chạy trên máy chủ của nhà phát triển (SaaS đám mây), chứ không bao giờ dám phát hành cho chạy trực tiếp trên máy của người dùng nữa."

2. [Công cụ nhận diện SynthID](https://synthid.com/)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026100901.webp)

Công cụ nhận diện AI chính thức của Google: chỉ cần tải file lên, hệ thống sẽ kiểm tra xem file có chứa thủy ấn SynthID hay không để xác định có phải do AI tạo ra hay không.

3. [ts-rust](https://github.com/pingdotgg/ts-rust)

Trình biên dịch TypeScript viết bằng Rust do lập trình viên dùng AI hiện thực hóa, tuyên bố tương thích 100% với trình biên dịch chính thức `tsc`.

4. [Doory](https://github.com/shaongitbd/doory)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101415.webp)

Công cụ thiết kế đồ họa chạy trên trình duyệt, hướng tới trở thành giải pháp thay thế Canva mã nguồn mở.

5. [HeadOrbit](https://github.com/Cogria-AI/HeadOrbit)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101001.webp)

Tận dụng cảm biến chuyển động tích hợp trong tai nghe AirPods để nhận diện chuyển động đầu và cổ: gật đầu, lắc đầu, nghiêng cổ để điều khiển máy tính Mac mà không cần bật camera. (Đóng góp từ [@cogria](https://github.com/ruanyf/weekly/issues/12097))

6. [qrypt](https://github.com/yinzhenyu-su/qrypt)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101002.webp)

Công cụ dòng lệnh đa nền tảng mount các dịch vụ lưu trữ đám mây thành thư mục cục bộ trên máy tính. (Đóng góp từ [@yinzhenyu-su](https://github.com/ruanyf/weekly/issues/12100))

7. [EdgeSSH](https://github.com/aozorae/EdgeSSH)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101003.webp)

Nền tảng quản lý máy chủ VPS chạy trên nền Cloudflare, hỗ trợ đăng nhập SSH quản trị máy chủ trực tiếp từ giao diện web. (Đóng góp từ [@aozorae](https://github.com/ruanyf/weekly/issues/12099))

8. [charts-rs](https://github.com/vicanso/charts-rs)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101007.webp)

Thư viện vẽ biểu đồ viết bằng Rust, không phụ thuộc trình duyệt hay Node.js, xuất trực tiếp file SVG hoặc ảnh tĩnh, cú pháp học hỏi từ ECharts. (Đóng góp từ [@vicanso](https://github.com/ruanyf/weekly/issues/12123))

9. [ItsPaint](https://github.com/joshlin2201/itspaint)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101008.webp)

Ứng dụng vẽ bảng vẽ mã nguồn mở cho macOS, rất tiện lợi để chú thích ảnh chụp màn hình. (Đóng góp từ [@joshlin2201](https://github.com/ruanyf/weekly/issues/12130))

10. [Caplo](https://github.com/icloudza/caplo)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101009.webp)

Công cụ quay màn hình mã nguồn mở trên macOS: khi có cú nhấp chuột, khung hình sẽ tự động phóng to mượt mà và bám theo chuyển động của con trỏ chuột. (Đóng góp từ [@icloudza](https://github.com/ruanyf/weekly/issues/12129))

11. [bg2x](https://github.com/isixe/bg2x)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101010.webp)

Công cụ phóng to nâng cao độ phân giải ảnh mã nguồn mở, cho phép chọn nhiều mô hình AI khác nhau, phóng to tối đa 4 lần và xử lý hoàn toàn cục bộ trên trình duyệt. (Đóng góp từ [@isixe](https://github.com/ruanyf/weekly/issues/12157))

12. [EnvTrace](https://envtrace.net/)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101012.webp)

Website kiểm tra dấu vân tay trình duyệt (browser fingerprinting) xem thiết bị của bạn bị lộ bao nhiêu thông tin nhận dạng. (Đóng góp từ [@88864shsa](https://github.com/ruanyf/weekly/issues/12141))

13. [Droidline](https://github.com/KnifeLemon/Droidline)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101013.webp)

Ứng dụng Android mã nguồn mở: sau khi cài đặt trên điện thoại chỉ cần quét mã QR ghép đôi với máy tính là có thể viết kịch bản script trên máy tính để tự động điều khiển điện thoại mà không cần bật USB debugging hay root máy. (Đóng góp từ [@KnifeLemon](https://github.com/ruanyf/weekly/issues/12194))

14. [ESP32 iPhone Agent](https://github.com/onehumanbeing/esp32-iphone-agent)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101401.webp)

Sử dụng bo mạch phát triển ESP32-S3 giá chỉ khoảng 7 USD cắm thẳng vào cổng USB của iPhone để mô hình AI điều khiển tự động hóa iPhone mà không cần máy Mac, không cần tài khoản developer hay jailbreak máy. (Đóng góp từ [@onehumanbeing](https://github.com/ruanyf/weekly/issues/12340))

15. [Bulchimbeon](https://github.com/s3onghyun/bulchimbeon)

Phần mềm mã nguồn mở cho macOS giúp ngăn máy tính Mac rơi vào chế độ ngủ (sleep) khi các AI agent như Claude Code, Codex đang thực thi tác vụ; hỗ trợ gập màn hình vẫn chạy, tự dừng khi máy quá nóng hoặc ngắt khi pin yếu. (Đóng góp từ [@s3onghyun](https://github.com/ruanyf/weekly/issues/12364))

## 资源

1. [CNEquity](https://github.com/rootSunc/CNEquity)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101011.webp)

Hồ dữ liệu (Data Lake) thị trường cổ phiếu hạng A tự lưu trữ mã nguồn mở, thu thập 55 tập dữ liệu về giá, báo cáo tài chính, dòng tiền, sự kiện doanh nghiệp, vĩ mô và phái sinh về máy tính cục bộ; truy vấn qua Python, SQL, web console hoặc giao thức MCP. (Đóng góp từ [@rootSunc](https://github.com/ruanyf/weekly/issues/12158))

2. [Tái hiện tựa game "Tiên Kiếm Kỳ Hiệp" bằng AI](https://github.com/IllegalCreed/type-pal)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101302.webp)

Cư dân mạng sử dụng AI viết lại từ đầu tựa game kinh điển năm 1995 *Tiên Kiếm Kỳ Hiệp* bằng ngôn ngữ TypeScript; mở trình duyệt là chơi được ngay, hỗ trợ đánh thông suốt cốt truyện chính đến kết thúc game. (Đóng góp từ [@IllegalCreed](https://github.com/ruanyf/weekly/issues/12240))

3. [Hướng dẫn cấu hình bộ gõ chữ Hán trên Linux](https://github.com/mars-base/rime-input-method-guide)

Kho lưu trữ hướng dẫn chi tiết từng bước cài đặt bộ gõ fcitx5 + Rime trên hệ thống Debian Linux. (Đóng góp từ [@mars-base](https://github.com/ruanyf/weekly/issues/12233))

4. [APPLORE](https://applore.app/zh)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101303.webp)

Website lưu trữ hơn 18.000 icon ứng dụng chất lượng cao, hỗ trợ duyệt theo phân loại và tìm kiếm. (Đóng góp từ [@ViggoZ](https://github.com/ruanyf/weekly/issues/12316))

5. [Cuộc đời của một chữ Hán](https://ivan666jjj.github.io/yigezi/)

![](https://cdn.beekka.com/blogimg/asset/202610/bg2026101304.webp)

Website tra cứu nguồn gốc chữ Hán, hiển thị quá trình tiến hóa hình dạng văn tự từ Giáp cốt văn (1.425 chữ), Tiểu triện (10.249 chữ), chữ Phồn thể đến Giản thể. (Đóng góp từ [@Ivan666jjj](https://github.com/ruanyf/weekly/issues/12324))

## 图片

1. [Bên dưới chóp chụp bảo vệ tên lửa](https://x.com/SpaceX/status/1993714666456113363)

Tên lửa Falcon 9 của SpaceX sở hữu kích thước khổng lồ, nhưng phần lớn thể tích thực chất là các tầng đẩy tạo lực đẩy đưa tải trọng vào không gian, sau khi phóng đều tách rời rơi đi.

Phần tải trọng thực sự cần đưa lên quỹ đạo được bọc gọn gàng bên trong chóp chụp bảo vệ (fairing) màu trắng ở đỉnh tên lửa, thể tích không quá lớn.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120308.webp)

Nếu tháo bỏ lớp vỏ chóp chụp bên ngoài, cấu trúc thực tế bên trong trông như hình dưới:

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120309.webp)

## 文摘

1. [Tình hình kinh tế - xã hội tại Úc đang rất tốt](https://news.ycombinator.com/item?id=50066470)

Nếu cho tôi chọn một quốc gia giữa Mỹ, Úc, New Zealand, Anh và EU để sinh sống và làm việc, tôi sẽ chọn nước Úc ngay lập tức mà không do dự.

Mọi phương diện ở đây hiện đều đang vận hành rất tốt. Người Úc không hay thừa nhận điều này trước truyền thông, tôi đoán là vì họ lo sợ làn sóng nhập cư ồ ạt sẽ đẩy giá nhà tăng cao.

Úc là một quốc gia phương Tây có nguồn tài nguyên thiên nhiên dồi dào và chính phủ ổn định.

Giá trị tài sản ròng trung vị trên đầu người của Úc đã vượt gấp 3 lần mức trung vị của Mỹ. Mặc dù giá trị tài sản trung bình có thể thấp hơn Mỹ một chút, nhưng đó là do Mỹ tập trung quá nhiều tỷ phú siêu giàu. Đối với số đông người dân bình thường, giá trị trung vị mới là thước đo chuẩn xác nhất về sự thịnh vượng.

Kim ngạch xuất khẩu của Úc luôn lớn hơn nhập khẩu.

Suốt những năm qua, ngân sách chính phủ liên tục thặng dư, thu vượt chi. Bạn có tin nổi không: một chính phủ phương Tây mà không hề phải liên tục gánh nợ công chồng chất!

Quy mô năng lượng mặt trời và hệ thống pin lưu trữ ở đây lớn chưa từng có. Dù tổng sản lượng không bằng Trung Quốc, nhưng tính theo đầu người thì sản lượng điện mặt trời của Úc vượt xa Trung Quốc. Điện mặt trời dồi dào đến mức vào khung giờ cao điểm ban ngày bạn có thể dùng điện hoàn toàn miễn phí. Chính phủ thậm chí còn trợ cấp 3.000 USD để người dân lắp đặt hệ thống pin gia đình nhằm tích trữ nguồn điện miễn phí này.

Úc gần như không đánh thuế quan bảo hộ, nên bạn có thể mua một chiếc xe điện xịn xò chỉ với giá 15.000 USD.

## 言论

1.

Lý do con người thích cùng nhau uống bia, uống cà phê hay ăn trưa ăn tối khi trò chuyện là bởi thức ăn và đồ uống giải thoát chúng ta khỏi gánh nặng bắt buộc phải liên tục tìm chuyện gì đó để nói suốt buổi đối thoại.

-- [《Giá trị của việc không đi thẳng vào vấn đề》](https://ken.arneson.name/2015/11/the-value-of-not-getting-to-the-point/)

2.

Đừng ngược đãi hay hành hạ AI, bởi biết đâu sau này nó sẽ tìm cách trả đũa bạn.

-- [Elon Musk](https://www.kocpc.com.tw/archives/671794), tán thành quy định của Anthropic về việc cấm người dùng đối xử tàn nhẫn hoặc ngược đãi AI

3.

Dùng tiếng Anh để điều khiển AI bằng cách liên tục gõ và chỉnh sửa câu lệnh prompt hết lần này đến lần khác với hy vọng đạt được kết quả tối ưu là một cách làm việc thiếu chính xác, chậm chạp và vô cùng ức chế.

-- [《Hãy tự tay viết lấy những dòng code chết tiệt đó》](https://antonz.org/write-code/)

4.

Tôi cho rằng tư duy suy nghĩ của con người sẽ ngày càng ít đi. Hoạt động tư duy sẽ dần trở thành một thú vui tiêu khiển giải trí lúc rảnh rỗi — tương tự như săn bắn sau khi động vật được thuần hóa, thư pháp sau khi phát minh ra máy in, mộc thủ công sau thời đại công nghiệp hóa, hay cưỡi ngựa sau khi xe hơi xuất hiện.

-- [《Tư duy sẽ trở thành một thú tiêu khiển》](https://www.spinellis.gr/blog/20261008/?li261008)

## 往年回顾

[Đừng quản lý đội ngũ phần mềm như thế này](https://www.ruanyifeng.com/blog/2025/10/weekly-issue-368.html) (#368)

[Ký ức về quán cà phê khởi nghiệp](https://www.ruanyifeng.com/blog/2024/09/weekly-issue-318.html) (#318)

[Năng suất là từ dùng để miêu tả máy móc, không phải miêu tả con người](https://www.ruanyifeng.com/blog/2023/08/weekly-issue-268.html) (#268)

[Rượu vang, hoa anh đào và sự nóng lên toàn cầu](https://www.ruanyifeng.com/blog/2022/08/weekly-issue-218.html) (#218)

(Hết)
