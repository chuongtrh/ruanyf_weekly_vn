# 科技爱好者周刊（第 184 期）：政府的存储需求有多大？

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2032) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111401.jpg)

Rạng sáng ngày 19/11, tên lửa đẩy Falcon 9 của hãng SpaceX rời bệ phóng tại bờ biển Đại Tây Dương trong điều kiện sương mù sáng sớm bao phủ dày đặc, tạo nên vầng sáng kỳ ảo như cảnh quay trong phim khoa học viễn tưởng. (Nguồn: [SpaceX Twitter](https://twitter.com/SpaceX/status/1459518399373922304))

## 主带话题：Quy mô lưu trữ dữ liệu số của các cơ quan chính phủ khổng lồ ra sao?

Mới đây, một bản tin công nghệ Mỹ đã thu hút sự chú ý của tôi:

> Sở Cảnh sát Dallas (Mỹ) trong quá trình di trú cơ sở dữ liệu nội bộ đã vô tình xóa nhầm 22TB dữ liệu. Mặc dù sau đó đã khôi phục lại được 14TB, 8TB dữ liệu còn lại đã hoàn toàn bị mất.
> 
> Đáng ngại hơn, phần dữ liệu bị mất vĩnh viễn này chứa toàn bộ tài liệu hồ sơ chứng cứ, hình ảnh và video của một vụ án giết người nghiêm trọng đang thụ lý. Sự biến mất của các bằng chứng cốt lõi khiến viện kiểm sát không thể tiếp tục truy tố nghi phạm, và cảnh sát đang phải bàn bạc phương án phóng thích do không đủ chứng cứ buộc tội.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081801.jpg)

Điểm đáng lưu ý ở đây không chỉ là sự cố xóa nhầm dữ liệu (vốn xảy ra hàng ngày ở khắp mọi nơi), mà là dung lượng lưu trữ của một sở cảnh sát cấp thành phố đã vượt ngưỡng 22TB. Điều đó cho thấy khối lượng thông tin cần lưu trữ của các cơ quan hành chính lớn thế nào, đòi hỏi các hệ thống lưu trữ chuyên dụng riêng biệt.

Dallas có dân số khoảng 1,3 triệu người với sở cảnh sát lưu trữ hàng chục TB. Nếu tính quy mô toàn bộ hệ thống cơ quan hành chính của nước Mỹ với dân số hơn 300 triệu dân, tổng dung lượng lưu trữ của tất cả các cơ quan thực thi pháp luật và an ninh quốc gia (như FBI, CIA, Bộ Quốc phòng, Bộ Tài chính) chắc chắn là một con số khổng lồ vô tiền khoáng hậu.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110722.jpg)

Tương tự, nhu cầu lưu trữ dữ liệu của các cơ quan hành chính công tại Trung Quốc cũng vô cùng lớn. Điều này có thể kiểm chứng gián tiếp thông qua các thông báo mời thầu dự án công nghệ trên Cổng thông tin mua sắm công chính phủ:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110908.jpg)

Chỉ tính riêng từ khóa tìm kiếm "lưu trữ" trong vòng 6 tháng qua đã trả về tới 11.431 thông báo thầu mua sắm của các đơn vị công lập khắp các tỉnh thành, với giá trị thầu từ vài trăm nghìn đến hàng triệu NDT. Ví dụ:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110724.jpg)

> - **Công ty Xuất nhập khẩu Sách Giáo dục Trung Quốc:** nâng cấp hệ thống đám mây dùng riêng (Private Cloud Storage) trị giá 2,3 triệu NDT.
> - **Đại học Trùng Khánh:** thầu mua sắm hệ thống máy chủ và lưu trữ All-Flash trị giá 2,43 triệu NDT.
> - **Đài Truyền hình Trung ương Trung Quốc:** thầu dịch vụ bảo trì trọn gói thiết bị lưu trữ đám mây dùng riêng trị giá 1,5 triệu NDT.
> - **Bệnh viện số 1 thuộc Đại học Tôn Trung Sơn (Quảng Châu):** nâng cấp trung tâm dữ liệu và lưu trữ trị giá 6,01 triệu NDT.
> - **Trường Cao đẳng Nghề Công Thương Quảng Đông:** mở rộng dung lượng thiết bị lưu trữ trị giá 300.000 NDT.

Việc mỗi cơ quan ban ngành tự xây dựng và vận hành một hệ thống lưu trữ dữ liệu hoặc đám mây dùng riêng (Private Cloud) bộc lộ nhiều điểm hạn chế:

1. **Không tối ưu hóa chi phí:** mỗi đơn vị phải tự trang bị phòng máy, máy chủ vật lý và đội ngũ kỹ thuật viên quản trị riêng biệt gây lãng phí nguồn lực xã hội.
2. **Thiếu hụt nhân sự trình độ cao:** các cơ quan công lập rất khó tuyển dụng và giữ chân các kỹ sư IT giỏi để chuẩn hóa quy trình vận hành bảo mật, dẫn tới nguy cơ xảy ra các sự cố rò rỉ dữ liệu hoặc xóa nhầm dữ liệu như vụ việc của Sở Cảnh sát Dallas.
3. **Phân mảnh dữ liệu:** việc mỗi đơn vị tự sử dụng định dạng lưu trữ và phần mềm quản trị khác nhau gây cản trở cho tiến trình liên thông và mở dữ liệu công.

Giải pháp tối ưu nhất là chính phủ thiết lập một hạ tầng "Đám mây Chính phủ" (Government Cloud) dùng chung thống nhất ở cấp quốc gia. Tất cả các cơ quan ban ngành địa phương sẽ thực hiện lưu trữ dữ liệu thông qua các cổng API chuẩn hóa của đám mây dùng chung này. Mô hình này giúp tiết kiệm ngân sách, bảo đảm an toàn dữ liệu qua cơ chế sao lưu tự động và thúc đẩy kết nối dữ liệu liên thông hiệu quả.

## Vue 3.x 训练营

Nhiều bạn mới tự học Front-end thường phân vân lựa chọn: *"Nên học React hay Vue trước?"*.

Cả hai framework đều rất phổ biến và hỗ trợ tốt cho công việc, nhưng số đông đánh giá Vue thân thiện và dễ tiếp cận hơn cho người mới bắt đầu.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111701.jpg)

Phiên bản Vue 3 ra mắt hỗ trợ tối ưu ngôn ngữ TypeScript và tái cấu trúc Composition API giúp quản lý code dự án lớn hiệu quả hơn, thúc đẩy tỷ lệ ứng dụng của doanh nghiệp tăng mạnh.

Tuần này, chúng tôi giới thiệu chương trình huấn luyện ngắn hạn **《Vue 3.x Front-end & Back-end Separation: Scaffold Architecture Development Practice》** giúp bạn làm chủ framework này:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111702.webp)

Khóa học gồm 3 buổi livestream liên tục từ ngày 22/11 đến 24/11 do nền tảng giáo dục công nghệ **Naixue Education** tổ chức. Chương trình giảng dạy tập trung thực chiến phát triển ứng dụng thông qua bộ khung Vite hiện đại.

Nội dung học chi tiết bao gồm:

> **Ngày 1: Cơ bản cho người mới bắt đầu**  
> Giới thiệu tổng quan hệ sinh thái Vue 3, thiết lập dự án và cú pháp cơ bản.
> 
> **Ngày 2: Tính năng cốt lõi nâng cao**  
> Tìm hiểu Composition API, các hàm reactivity (`ref`, `reactive`), quản lý state và cơ chế watch.
> 
> **Ngày 3: Thực chiến dự án**  
> Xây dựng cấu trúc dự án thực tế bằng scaffold Vite, đóng gói và tối ưu hóa component.

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111703.jpg)

Độc giả bản tin có thể quét mã QR trên đây hoặc bấm vào [liên kết đăng ký](https://j.naixuejiaoyu.com/1J6ZZgZlLm8?putcode=20211119KOLGZH-RYF) để tham gia khóa học với mức phí ưu đãi chỉ **0.99 NDT**.

## 科技动态

1、[Phi thuyền helium khinh khí cầu lớn nhất thế giới chuẩn bị chở khách](https://www.businessinsider.com/photos-see-the-flying-bum-airlander-10-2021-9)

Dòng khinh khí cầu helium lai ghép Airlander 10 do một hãng công nghệ Anh chế tạo có chiều dài thân lên tới 91 mét (lớn hơn chiều dài 80 mét của siêu máy bay chở khách Airbus A380):

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091805.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091806.jpg)

Thiết kế ban đầu của khinh khí cầu phục vụ đơn đặt hàng quân sự của Bộ Quốc phòng Mỹ năm 2013 nhưng sau đó bị hủy bỏ. Hãng sản xuất đã quyết định hoán cải thiết bị sang mục đích dân dụng:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091807.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091810.jpg)

Phần khoang cabin bên dưới khí cầu được thiết kế sang trọng với sức chứa 100 hành khách, trang bị các cửa sổ kính sát đất lớn phục vụ du lịch ngắm cảnh trên không. Thiết bị có tốc độ di chuyển chậm khoảng 100 km/h và dự kiến đi vào phục vụ thương mại từ năm 2025:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091808.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091809.jpg)

2、[Doanh số bán xe hơi động cơ đốt trong tại Na Uy giảm mạnh](https://electrek.co/2021/09/23/norway-bans-gas-cars-in-2025-but-trends-point-toward-100-ev-sales-as-early-as-april/)

Chính phủ Na Uy đã công bố lộ trình cấm bán toàn bộ xe chạy xăng và dầu vào năm 2025 (sớm nhất thế giới).

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021092404.jpg)

Thực tế tốc độ dịch chuyển sang xe điện tại đây diễn ra nhanh hơn dự kiến: thị phần xe chạy xăng dầu truyền thống đã giảm từ 21% năm ngoái xuống chỉ còn 10% vào tháng 9 vừa qua. Trong số 15 mẫu xe bán chạy nhất nước này, có tới 14 mẫu là xe điện và 1 mẫu là hybrid. Các chuyên gia dự báo doanh số bán xe mới có thể đạt tỷ lệ 100% xe điện ngay trong đầu năm sau, bất chấp thời tiết lạnh giá Bắc Âu làm giảm hiệu năng pin.

3、[Phát triển thiết bị vòng đeo tay phát điện từ thân nhiệt](https://www.newscientist.com/article/2276215-wristband-that-turns-body-heat-into-electricity-can-power-an-led/)

Các nhà khoa học tại Viện Công nghệ Cáp Nhĩ Tân đã chế tạo mẫu vòng đeo tay độc đáo có khả năng thu năng lượng từ nhiệt độ cơ thể người:

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102901.jpg)

Thiết bị sử dụng các điện cực linh hoạt tích hợp hợp chất Magnesium và Bismuth dán áp sát vào da cổ tay để khai thác sự chênh lệch nhiệt độ giữa da người và môi trường không khí bên ngoài làm nguồn phát điện. Dòng điện tuy nhỏ nhưng đủ để duy trì hoạt động phát sáng của hệ thống đèn LED cảnh báo thể thao ban đêm:

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021102902.jpg)

4、[Đính chính thông tin nhiễu sóng vô tuyến ngoài trái đất](https://www.nature.com/articles/d41586-021-02931-7)

Vào năm 2019, đài thiên văn Úc công bố thu nhận được luồng sóng vô tuyến định kỳ hướng phát từ chòm sao Alpha Centauri (hệ sao gần mặt trời nhất có hành tinh chứa nước lỏng), làm dấy lên giả thuyết về sự tồn tại của nền văn minh ngoài trái đất:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110105.jpg)

Tuy nhiên sau hơn một năm phân tích dữ liệu, các nhà khoa học xác định đây thực chất chỉ là tín hiệu nhiễu sóng phát ra từ các thiết bị phát sóng liên lạc hàng không trên mặt đất. Phát hiện củng cố quan điểm cho rằng các kính viễn vọng lớn trong tương lai cần được đưa lên quỹ đạo không gian để tránh nhiễu sóng từ mặt đất.

5、[Nhật Bản phê duyệt thương mại hóa cá nóc chỉnh sửa gen](https://news.sina.com.cn/w/2021-10-30/doc-iktzqtyu4375777.shtml)

Bộ Y tế Nhật Bản đã chính thức cấp phép lưu thông thương mại giống cá nóc hổ chỉnh sửa gen mới:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110106.jpg)

Các nhà khoa học đã ứng dụng công nghệ CRISPR để bất hoạt gen ức chế sự thèm ăn của cá nóc, khiến cá liên tục ăn và tăng trưởng trọng lượng gấp 1,9 lần so với giống tự nhiên trong cùng một chu kỳ nuôi dưỡng. Đây là thực phẩm chỉnh sửa gen thứ 3 được cấp phép tại Nhật (sau cà chua hỗ trợ hạ huyết áp và cá tráp tăng cơ):

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021110107.jpg)

## 文章

1. [Hướng dẫn quy trình đóng gói và xuất bản ứng dụng web PWA lên Apple App Store](https://blog.pwabuilder.com/posts/publish-your-pwa-to-the-ios-app-store/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021103004.jpg)

Bài viết hướng dẫn lập trình viên sử dụng các công cụ đóng gói trung gian để chuyển đổi trang web dạng Progressive Web App (PWA) thành tệp tin ứng dụng tương thích tiêu chuẩn và gửi lên kho ứng dụng App Store dành cho hệ điều hành iOS.

2. [Tổng quan cấu trúc và cơ chế thiết lập chỉ mục trong MySQL](https://blog.csdn.net/wallace_www/article/details/117264149)（Tiếng Trung）

Bài viết phân tích chuyên sâu về cấu trúc dữ liệu B+ Tree dùng để thiết lập Index trong cơ sở dữ liệu MySQL, thảo luận các nguyên tắc lựa chọn trường dữ liệu để thiết lập chỉ mục tối ưu hiệu năng truy vấn. (Đóng góp của [@wallace1995](https://github.com/ruanyf/weekly/issues/2055))

3. [Tìm hiểu các giá trị trả về của hàm printf() trong ngôn ngữ C](https://www.netmeister.org/blog/return-printf.html)（Tiếng Anh）

Phân tích một chi tiết cú pháp ít được chú ý trong lập trình C: tại sao hàm xuất văn bản tiêu chuẩn `printf()` lại trả về giá trị số nguyên biểu thị số lượng ký tự được in ra màn hình hoặc giá trị âm biểu thị lỗi hệ thống.

4. [Các giải pháp ngăn chặn gỡ lỗi ngược và phát hiện Chrome DevTools](https://medium.com/@weizmangal/javascript-anti-debugging-some-next-level-sh-t-part-2-abusing-chromium-devtools-scope-pane-b2796c00331d)（Tiếng Anh）

Giới thiệu một số mẹo nâng cao sử dụng JavaScript để phát hiện nhanh hành vi người dùng mở công cụ Developer Tools trên trình duyệt nhằm bảo vệ mã nguồn Front-end khỏi các công cụ cào dữ liệu.

5. [Hướng dẫn sử dụng Calibre chuyển đổi trang web lưu trữ cục bộ thành Ebook](https://bbs.pediy.com/thread-269615.htm)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021100503.jpg)

Bài hướng dẫn viết các đoạn kịch bản Python kết hợp phần mềm quản lý Calibre để cào và sắp xếp các trang HTML lưu trữ cục bộ thành một cuốn sách điện tử định dạng EPUB/MOBI mượt mà. (Đóng góp của [@evmn](https://github.com/ruanyf/weekly/issues/1987))

6. [Hướng dẫn xây dựng ứng dụng đọc tin tức Android bằng React Native](https://www.freecodecamp.org/news/build-an-android-news-app-with-react-native-and-native-base/)（Tiếng Anh）

Cẩm nang thực chiến hướng dẫn lập trình viên di động từng bước cài đặt môi trường, liên kết API tin tức công cộng và thiết kế giao diện bằng thư viện NativeBase để hoàn thiện app tin tức.

7. [Tại sao website nên ưu tiên ứng dụng kỹ thuật hình ảnh nhiễu sắc (Dithering)?](https://endtimes.dev/why-you-should-dither-images/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021093003.jpg)

Tác giả đề xuất phương án nén ảnh nghệ thuật hiển thị trên web bằng giải pháp chuyển đổi ảnh màu có chiều sâu lớn sang dạng ảnh chấm hạt nhiễu sắc (Dithering) giúp giảm dung lượng file xuống cực nhẹ khi lưu dưới dạng PNG/WebP mà vẫn giữ được phom ảnh gốc.

8. [Hành trình tối ưu hóa thuật toán phân tích dấu ngoặc màu của nhóm phát triển VS Code](https://code.visualstudio.com/blogs/2021/09/29/bracket-pair-colorization)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021093004.jpg)

Nhóm kỹ sư phát triển phần mềm soạn thảo VS Code chia sẻ giải pháp kỹ thuật viết lại bộ phân tích cú pháp ngoặc màu (Bracket pair colorization) từ dạng extension bên thứ ba ngốn tài nguyên thành tính năng tích hợp trực tiếp vào nhân giúp hiển thị ngoặc màu siêu nhanh không gây卡顿.

9. [Trải nghiệm phát triển ứng dụng Full-stack toàn diện trên nền tảng Cloudflare Pages](https://blog.cloudflare.com/building-full-stack-with-pages/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111812.jpg)

Đại diện Cloudflare giới thiệu các nâng cấp mới của dịch vụ Cloudflare Pages cho phép lập trình viên tích hợp các cloud functions (Workers) và cơ sở dữ liệu KV để tạo lập một ứng dụng Web Full-stack hoàn chỉnh trên cùng một hạ tầng.

## 工具

1、[Hurl: Tiện ích kiểm thử API bằng dòng lệnh](https://hurl.dev/)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021100604.jpg)

Công cụ CLI tương tự curl hỗ trợ gửi các yêu cầu HTTP, phân tích phản hồi và tự động đối chiếu kiểm thử (assertion) theo các cấu hình định sẵn, rất phù hợp cho các quy trình test CI/CD.

2、[ColorFu: Tiện ích thiết kế hình nền tối giản trực tuyến](https://colorfu.art/editor)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111308.jpg)

Trình tạo ảnh nền đồ họa trực tuyến hỗ trợ người dùng phối chữ viết nghệ thuật lên các khối màu sắc hoặc chất liệu vân đá tối giản để tải về làm hình nền. (Đóng góp của [@pearmini](https://github.com/ruanyf/weekly/issues/2053))

3、[Xterm.js: Nhúng Terminal trực tiếp lên website](https://xtermjs.org/)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021100902.jpg)

Thư viện JavaScript hỗ trợ lập trình viên tạo lập một cửa sổ dòng lệnh Terminal hoạt động trực quan trên giao diện web giúp tương tác quản trị máy chủ từ xa qua WebSockets.

4、[yabai: Trình quản lý sắp xếp cửa sổ dạng phẳng cho macOS](https://github.com/koekeishiya/yabai/)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021101001.jpg)

Tiện ích mở rộng hỗ trợ người dùng macOS tự động căn chỉnh và phân chia diện tích hiển thị của các cửa sổ ứng dụng đang mở theo dạng phẳng (tiling window) khoa học.

5、[ROAPI: Tự động chuyển đổi tệp tin dữ liệu tĩnh thành API](https://github.com/roapi/roapi)

Giải pháp server API viết bằng Rust hỗ trợ người dùng tự động ánh xạ cấu trúc các file tĩnh JSON, CSV thành cổng API REST hoặc GraphQL tương tác dữ liệu mà không cần viết code.

6、[Unicode Calendar Generator: Tự sinh lịch biểu bằng ký tự Unicode](https://qwerty.dev/calendar-generator/)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021101404.jpg)

Một trang web tiện ích hỗ trợ tự sinh nhanh một bảng hiển thị lịch các tháng trong năm cấu thành hoàn toàn từ các ký tự văn bản Unicode để copy/paste nhanh vào file README.md.

7、[weird json: Thư viện sao chép sâu đối tượng trong JavaScript](https://github.com/i5ik/weird-json)

Thư viện JavaScript hỗ trợ thực hiện nhân bản sâu (deep copy) đối tượng thông qua phương pháp tối ưu chuyển đổi chuỗi JSON độc lập để tránh các lỗi tham chiếu vùng nhớ.

8、[Euterpe: Phần mềm máy chủ phát nhạc trực tuyến cá nhân](https://github.com/ironsmile/euterpe)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111813.webp)

Mã nguồn thiết lập music streaming server cá nhân nguồn mở, hỗ trợ tải lên các tệp tin nhạc lossless và phát nhạc trực tuyến thông qua giao diện web di động khi đi ra ngoài.

9、[Matrix Rain: Hiệu ứng mưa chữ xanh trong The Matrix](https://github.com/nojvek/matrix-rain)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091205.jpg)

Thư viện JavaScript hỗ trợ chạy trình chiếu hiệu ứng các dòng mã chữ xanh rơi uốn lượn phong cách phim Ma Trận ngay trên màn hình terminal của lập trình viên.

10、[gobang: Trình quản lý SQL database bằng dòng lệnh](https://github.com/TaKO8Ki/gobang)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091206.jpg)

Công cụ viết bằng Rust hỗ trợ lập trình viên kết nối và quản trị nhanh các cơ sở dữ liệu MySQL, PostgreSQL và SQLite trực tiếp trong cửa sổ terminal không cần GUI.

## Tài nguyên

1、[deskto.ps: Chuyên trang chia sẻ hình ảnh góc làm việc của lập trình viên](https://deskto.ps/)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021100901.jpg)

Trang web cộng đồng cho phép các chuyên gia công nghệ chia sẻ ảnh chụp màn hình desktop bố trí các widget tiện ích làm việc của mình để học hỏi kinh nghiệm sắp xếp.

2、[Email-newsletter-RSS: Tổng hợp luồng RSS bản tin công nghệ tiếng Trung](https://github.com/alaskasquirrel/Email-newsletter-RSS)

Kho lưu trữ tổng hợp liên kết đăng ký theo dõi các trang bản tin chia sẻ kinh nghiệm công nghệ Front-end, Back-end chất lượng cao qua RSS. (Đóng góp của [@alaskasquirrel](https://github.com/ruanyf/weekly/issues/2054))

3、[Vididoo: Công cụ xử lý video trực tuyến gọn nhẹ](https://vididoo.vercel.app/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090506.jpg)

Website cung cấp các công cụ xử lý tệp tin video cơ bản chạy trực tiếp trên trình duyệt như: nén dung lượng, cắt video, tách xuất file âm thanh MP3 từ video.

4、[oldmouse.com: Bảo tàng lịch sử chuột máy tính trực tuyến](http://oldmouse.com/)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021101102.jpg)

Chuyên trang giới thiệu tư liệu hình ảnh về quá trình phát triển của chuột máy tính từ các nguyên mẫu cơ khí thô sơ bằng gỗ thời kỳ đầu.

5、[GNU Coreutils CLI Text Processing: Giáo trình xử lý văn bản Linux](https://learnbyexample.github.io/cli_text_processing_coreutils/preface.html)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021101301.jpg)

Giáo trình tiếng Anh miễn phí hướng dẫn chi tiết cách sử dụng các dòng lệnh cơ bản trong gói GNU Coreutils (như head, tail, tr, sort) để lọc dữ liệu log hệ thống.

## 图片

1、[Hiện tượng địa chất kỳ lạ "Vết khuyết địa tầng vĩ đại" tại Grand Canyon](https://www.bbc.com/future/article/20210901-the-strange-race-to-track-down-a-missing-billion-years)

Từ thế kỷ 19, các nhà địa chất học đã ghi nhận hiện tượng bất thường khi nghiên cứu cấu trúc đá tại vườn quốc gia Grand Canyon:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090603.jpg)

Quan sát hình ảnh mặt cắt vách đá, tầng đá kết tinh phía dưới được xác định có niên đại hình thành khoảng 1,7 tỷ năm, trong khi lớp cát đá phủ ngay phía trên nó lại có niên đại chỉ 550 triệu năm. Khoảng trống địa tầng chênh lệch tới hơn 1 tỷ năm hoàn toàn biến mất không để lại dấu tích bùn đất trung gian. Hiện tại giả thuyết phổ biến nhất cho rằng thời kỳ đó khu vực này bị các sông băng khổng lồ phủ kín và mài mòn hoàn toàn bề mặt trước khi lớp trầm tích mới hình thành.

2、[Quy hoạch đô thị hướng tới người đi bộ của thành phố Utrecht](https://twitter.com/david_perell/status/1434731477237907460)

Thành phố cổ Utrecht (Hà Lan) sở hữu thiết kế đô thị đặc sắc ưu tiên tuyệt đối không gian công cộng cho người đi bộ và xe đạp thay vì ô tô:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090715.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090716.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090717.jpg)

Toàn bộ hệ thống kè kênh rạch nội đô được thiết kế thấp sát mặt nước tạo lập các tuyến亲水 (親水 -亲 thủy) bộ hành tuyệt đẹp, đem lại chất lượng không khí trong lành cho cư dân.

## Bài đọc thêm

### Giai thoại về tệp tin JSON 74.000 số điện thoại của Barclays Bank

Để phòng tránh vấn nạn giả mạo nhân viên ngân hàng thực hiện các cuộc gọi lừa đảo chiếm đoạt tài sản của khách hàng, ngân hàng Barclays Bank (Anh) đã thiết kế một trang web tra cứu chính chủ số điện thoại来 điện:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111805.jpg)

Tuy nhiên, thay vì gửi yêu cầu truy vấn số điện thoại về cơ sở dữ liệu ở máy chủ Backend để kiểm tra và trả về kết quả, trang web này lại trực tiếp tải một file dữ liệu tĩnh định dạng JSON có dung lượng lên tới 1.3 MB về trình duyệt của khách hàng:

[Tệp tin JSON chứa số điện thoại của Barclays](https://www.barclays.co.uk/content/dam/json-files/TelephoneNumberChecker_26_03_2021.json)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021083104.jpg)

File JSON này chứa danh sách công khai toàn bộ 74.000 số điện thoại nội bộ của ngân hàng. Hơn thế nữa, bộ lọc kiểm tra của website hoạt động rất ngô nghê: nếu người dùng nhập số điện thoại có kèm mã vùng quốc gia `+44` hoặc có dấu gạch ngang phân cách, hệ thống sẽ báo không tìm thấy số do không được cấu hình Regex xử lý chuẩn hóa chuỗi đầu vào ở client.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021083105.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021083106.jpg)

Đây là ví dụ điển hình về việc thiết kế hệ thống cẩu thả và thiếu kiến thức bảo mật cơ bản của đội ngũ phát triển ứng dụng web doanh nghiệp.

### So sánh kỹ thuật giữa tàu ngầm hạt nhân và tàu ngầm động cơ AIP

Tàu ngầm diesel truyền thống bắt buộc phải thường xuyên nổi lên mặt nước hoặc sử dụng ống thông hơi để lấy oxy ngoài không khí chạy động cơ sạc pin, điều này khiến chúng dễ bị radar đối phương phát hiện.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021083108.jpg)

Sự xuất hiện của tàu ngầm hạt nhân thế hệ mới sử dụng lò phản ứng hạt nhân không cần oxy đã giải quyết triệt để vấn đề này, cho phép tàu lặn liên tục vài tháng dưới lòng đại dương với công suất di chuyển rất lớn. Tuy nhiên, chi phí đóng mới và bảo trì một tàu ngầm hạt nhân cực kỳ đắt đỏ (như tàu ngầm lớp Virginia của Mỹ tiêu tốn tới 2,6 tỷ USD).

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111806.jpg)

Do đó, các quốc gia có ngân sách quốc phòng vừa phải đã phát triển dòng tàu ngầm diesel ứng dụng hệ thống động cơ không cần không khí ngoài trời AIP (Air-Independent Propulsion), sử dụng nguồn oxy lỏng dự trữ sẵn trên tàu để sạc pin khi lặn sâu:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111807.jpg)

So sánh thông số kỹ thuật giữa hai dòng tàu:
- **Thời gian lặn liên tục:** Tàu ngầm hạt nhân có thể lặn liên tục 3-4 tháng; tàu ngầm AIP lặn liên tục khoảng 3 tuần (đủ đáp ứng cho các hoạt động phòng thủ vùng biển cận duyên).
- **Tốc độ di chuyển:** Tàu ngầm hạt nhân đạt tốc độ lặn hơn 35 dặm/giờ; tàu ngầm AIP đạt tốc độ khoảng 23 dặm/giờ.
- **Giá thành:** Tàu ngầm hạt nhân có giá từ 2-3 tỷ USD; tàu ngầm AIP có giá mềm hơn khoảng 200 - 600 triệu USD.
- **Quy mô thủy thủ đoàn:** Tàu hạt nhân lớn cần hơn 100 người vận hành; tàu AIP trung bình cần từ 30 - 60 người.

## 言论

1\.

Tôi không bao giờ đầu tư vào các đồng tiền mã hóa (crypto), lý do cốt lõi là tôi không muốn gánh chịu áp lực tâm lý căng thẳng do sự biến động giá cả quá lớn của thị trường này hàng ngày mang lại.

-- Thảo luận trên Hacker News

2\.

Tôi đến chơi và lưu trú tại nhà mẹ đẻ một tuần. Ngay sau khi trở về căn hộ của mình, tôi bắt đầu nhận được hàng loạt quảng cáo về nhãn hiệu kem đánh răng mà mẹ tôi đang dùng trên các mạng xã hội dù tôi chưa bao giờ tìm kiếm thương hiệu đó. 

Sau đó tôi nhận ra: các ứng dụng di động đã thu thập vị trí GPS định vị của tôi và mẹ tôi ở cùng một vị trí trong nhiều ngày, từ đó AI phán đoán mối quan hệ thân cận và thực hiện phân phối chéo các quảng cáo tiêu dùng giữa các tài khoản.

-- Chia sẻ trên Twitter

## 历史上的本周

- 2020年（第 133 期）：[Thảo luận về tiềm năng xây dựng trung tâm dữ liệu xanh của tỉnh Quý Châu tương tự Thụy Sĩ](https://www.ruanyifeng.com/blog/2020/11/weekly-issue-133.html)
- 2019年（第 81 期）：[Thảo luận xã hội học về khả năng bứt phá phát triển vượt bậc của thế hệ con cái so với nền tảng cha mẹ](https://www.ruanyifeng.com/blog/2019/11/weekly-issue-81.html)
- 2018年（第 30 期）：[Phân tích nguyên nhân tại sao tập đoàn Google lại liên tục thất bại khi phát triển các sản phẩm mạng xã hội](https://www.ruanyifeng.com/blog/2018/11/weekly-issue-30.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
