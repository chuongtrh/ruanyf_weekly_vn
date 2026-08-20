# Bản tin chia sẻ công nghệ (Số 372): Thiết kế giao diện phần mềm thế nào cho đúng

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/8003) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110503.webp)

Không gian tự học tại Thư viện Quốc gia Trung Quốc ở Bắc Kinh vào một ngày mùa đông. ([via](https://www.xinhuanet.com/photo/20251103/d338bbe8a8104730816261a553dd7b9a/c.html))

## 软件界面如何设计

（1）

Giao diện người dùng (UI) của phần mềm là một lĩnh vực chuyên sâu. Có cả một ngành công nghiệp chuyên nghiên cứu về nó, gọi là "Thiết kế UI".

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110511.webp)

Tôi cảm giác nhiều lập trình viên phát triển phần mềm không có nhiều nhạy cảm đối với thiết kế UI, họ không biết thế nào là một giao diện vừa đẹp mắt vừa dễ sử dụng.

Khi tự tay làm giao diện đồ họa, họ chỉ đơn giản là nhồi nhét tất cả các tính năng hiện có lên màn hình và coi như đã hoàn thành công việc, bất chấp việc người dùng có hiểu cách vận hành hay không.

Những ví dụ kiểu này rất nhiều, tôi xin nêu ra một trường hợp vừa bắt gặp gần đây.

（2）

Có một phần mềm rất nổi tiếng là [Handbrake](https://handbrake.fr/) hỗ trợ chuyển đổi định dạng video.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103103.webp)

Tính năng của nó cực kỳ mạnh mẽ, hỗ trợ hầu hết mọi định dạng video đầu vào, đáp ứng đầy đủ mọi nhu cầu nâng cao, lại hoàn toàn miễn phí và chạy đa nền tảng.

Thế nhưng, khi mở phần mềm này lên và nhìn vào giao diện của nó, bạn sẽ lập tức có cảm giác e ngại, trừ khi bạn là một người dùng chuyên nghiệp.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103104.webp)

Bức ảnh trên là giao diện chính của phần mềm, với hàng loạt tùy chọn cài đặt nằm san sát nhau kèm các thuật ngữ giải thích khiến người ngoài ngành hoàn toàn bối rối.

Nếu không phải là chuyên gia, người dùng sẽ tự hỏi: "Tôi nên bắt đầu từ đâu? Liệu tôi có bấm nhầm nút nào không? Để đọc tài liệu hướng dẫn thì có mất quá nhiều thời gian không?"

Và nếu người dùng kiên nhẫn bấm vào menu "Cài đặt" để tìm kiếm thêm gợi ý, họ sẽ nhận thêm một gáo nước lạnh:

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103105.webp)

Giao diện dày đặc các thuật ngữ chuyên môn sâu này dễ khiến người dùng phổ thông cảm thấy trình độ bản thân quá thấp và không đủ khả năng sử dụng công cụ.

Hãy hình dung: người dùng chỉ muốn tìm một công cụ nhỏ để chuyển đổi định dạng video nhanh chóng, nhưng giao diện của công cụ lại liên tục đưa ra thông điệp "bạn không đủ trình độ".

Đây chính là ví dụ điển hình của một giao diện tồi tệ, không chỉ khó dùng mà còn gây ức chế cho người dùng.

（3）

[Một lập trình viên nước ngoài](https://danieldelaney.net/normal/) đã không thể kiên nhẫn thêm được nữa và tự hỏi: "Liệu giao diện của một phần mềm phổ thông có thực sự cần thiết phải phức tạp đến vậy?"

Anh ấy đã tự tay thiết kế lại một giao diện UI hoàn toàn mới:

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103106.webp)

Trông giao diện mới này rõ ràng là trực quan hơn rất nhiều đúng không?

Bất cứ ai nhìn vào giao diện này đều hiểu ngay cách vận hành mà không có chút áp lực tâm lý nào. Thao tác duy nhất cần làm là tải tệp video lên. Người dùng không thể làm sai được, vì ngoài nút tải tệp lên thì giao diện không còn nút bấm nào khác. Chỉ sau khi bạn thêm tệp video thành công, nút bấm duy nhất tiếp theo mới sáng lên để cho phép click.

Bạn có tin được rằng giao diện tối giản này và giao diện phức tạp ban đầu là cùng một phần mềm và thực thi cùng một tác vụ không?

Đây chính là bí quyết của một thiết kế UI xuất sắc: **Tránh việc cung cấp nhiều lối vào cho các thao tác, tránh bắt người dùng phải đưa ra lựa chọn, cung cấp giá trị mặc định tối đa cho tất cả các cài đặt**. Chỉ có như vậy mới giúp người dùng không bị bối rối và có thể hoàn thành công việc chỉ với phím Enter.

Tất nhiên, nhiều người dùng chuyên nghiệp sẽ không đồng tình và đưa ra hàng loạt thắc mắc:

> - Tại sao lại lược bỏ các tính năng mạnh mẽ ban đầu của Handbrake?
> - Nếu có người dùng muốn tùy chỉnh các thông số khác thì sao?
> - Bạn đã tính đến các nhu cầu đặc biệt và trường hợp biên (edge cases) chưa?

Giải pháp thực tế rất đơn giản: chỉ cần thiết kế thêm một giao diện "Chế độ chuyên nghiệp" (Professional Mode) – chính là giao diện hiện tại của Handbrake. Người dùng nào có nhu cầu tinh chỉnh chuyên sâu có thể chủ động chuyển sang giao diện đó để sử dụng.

（4）

Rất nhiều vật dụng trong đời sống hàng ngày của chúng ta cũng gặp phải tình trạng giao diện thiết kế quá phức tạp một cách không cần thiết.

Hãy lấy chiếc điều khiển từ xa (remote) của tivi làm ví dụ, nó được bố trí dày đặc các nút bấm.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103107.webp)

Đến mức nhiều người dùng đã phải dùng băng keo để dán che bớt những nút bấm không bao giờ dùng đến:

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103108.webp)

Thực chất, sau khi dán băng keo che bớt, chiếc remote mới trở về đúng thiết kế giao diện cần có của nó: chỉ giữ lại những nút bấm thực sự thiết yếu nhất.

Những nút bấm ít khi dùng đến hoàn toàn có thể được giấu bên dưới một nắp trượt, để những ai thực sự cần tinh chỉnh nâng cao có thể tự trượt nắp ra để tìm kiếm.

## [本周软件] NocoBase

Làm thế nào để phát triển nhanh một hệ thống quản lý vận hành doanh nghiệp?

Bên cạnh việc giao cho các mô hình AI lớn, có một giải pháp đơn giản và đáng tin cậy hơn là sử dụng [NocoBase](https://github.com/nocobase/nocobase).

![AI-Employees](https://cdn.beekka.com/blogimg/asset/202511/bg2025110603.webp)

Đây là một nền tảng phát triển low-code/no-code mã nguồn mở, hiện đã nhận được hơn 17.000 sao trên GitHub.

Ý tưởng thiết kế của NocoBase rất trực quan: (1) Kết nối vào cơ sở dữ liệu của bạn, (2) Thiết kế giao diện kéo thả trực quan dạng WYSIWYG, (3) Cấu hình các mô-đun plugin cần thiết (như plugin phân quyền, SSO đăng nhập, in ấn, quản lý tài liệu, v.v.).

![AI-Employees](https://cdn.beekka.com/blogimg/asset/202511/bg2025110604.webp)

Phiên bản 2.x mới nhất còn tích hợp tính năng Nhân viên AI (AI Employees), giúp đưa năng lực của các mô hình AI lớn vào hệ thống vận hành doanh nghiệp một cách mượt mà, ví dụ như tự động tìm hiểu thông tin khách hàng, phân tích số liệu hay cào bảng báo giá từ các nền tảng nhà cung cấp.

Sau hơn 4 năm ra mắt, phiên bản thương mại của dự án đã có lượng khách hàng từ hơn 50 quốc gia và vùng lãnh thổ, mang lại doanh thu hàng chục triệu nhân dân tệ mỗi năm.

Bạn có thể đăng ký tài khoản dùng thử bản demo trên [trang chủ](https://www.nocobase.com/cn/) để thử nghiệm tính năng tạo giao diện thao tác cho cơ sở dữ liệu của mình, hoặc tải mã nguồn từ [GitHub](https://github.com/nocobase/nocobase) để tự triển khai.

## 科技动态

1. Một nhà khởi nghiệp nước ngoài vì gặp khó khăn tài chính cho chi phí tổ chức đám cưới của mình đã đăng bài lên mạng xã hội để tìm kiếm nhà tài trợ. Đổi lại, anh sẽ treo biển quảng bá tên của các nhãn hàng tài trợ trong lễ cưới.

Kết quả bất ngờ khi có tới 26 công ty đồng ý tài trợ cho anh. Dưới đây là những bức ảnh chụp lại lễ cưới đặc biệt tràn ngập logo thương hiệu đó.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103005.webp)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103006.webp)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103007.webp)

2. Vụ kiện tranh chấp bản quyền tác giả đối với prompt AI đầu tiên tại Thượng Hải vừa được tuyên án.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110607.webp)

Một công ty vào năm 2022 đã soạn thảo 6 bộ từ khóa gợi ý (prompt) để sinh các tác phẩm hội họa trên nền tảng Midjourney, sau đó đăng tải lên mạng xã hội Xiaohongshu (Tiểu Hồng Thư).

Về sau, công ty phát hiện ra hai bị đơn đã copy nguyên các prompt này để sinh tranh rồi công bố rộng rãi, nên đã khởi kiện yêu cầu hai bị đơn chấm dứt hành vi vi phạm và bồi thường 9.900 nhân dân tệ.

Tòa án phán quyết rằng các prompt này chỉ là sự liệt kê đơn giản các yếu tố hình ảnh, thiếu tính liên kết ngữ pháp logic và chưa thể hiện được sự đầu tư trí tuệ mang tính cá nhân hóa của tác giả, do đó không được công nhận là một tác phẩm. Vì vậy, tòa bác đơn kiện và tuyên bố nguyên cáo không có quyền tác giả đối với các prompt này.

3. Một công ty Mỹ vừa chính thức mở bán dòng robot làm việc nhà đầu tiên trên thế giới với mức giá 20.000 USD.

Ngoại hình của chú robot này trông có phần hơi kỳ dị.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110608.webp)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110609.webp)

Mặc dù mức giá không phải là quá đắt đỏ so với các dòng robot công nghệ cao, tuy nhiên các tác vụ tự động mà nó có thể thực hiện là vô cùng hạn chế. Phần lớn các động tác vẫn cần con người điều khiển từ xa, và tốc độ làm việc của nó cũng cực kỳ chậm chạp, mất tới 1 phút chỉ để lấy một chai nước.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110610.webp)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110611.webp)

4. Trong menu tắt máy của hệ điều hành Windows có tùy chọn "Cập nhật và tắt máy" (Update and shut down) mà chắc hẳn mọi người đều đã từng sử dụng qua.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110402.webp)

Tuy nhiên, tùy chọn này tồn tại một lỗi (bug) kinh điển: hệ thống sau khi cập nhật xong thực chất không hề tắt máy mà lại tự khởi động lại và đứng chờ thao tác của bạn, tên gọi chính xác của nó đáng lẽ phải là "Cập nhật và khởi động lại".

Microsoft đã để mặc lỗi này mà không sửa trong suốt khoảng 20 năm qua. Mãi đến bản cập nhật Windows 11 phiên bản 25H2 mới nhất, hành vi này mới chính thức được khắc phục để hệ thống tự động tắt máy hoàn toàn sau khi cập nhật.

5. Công ty công nghệ quốc phòng Mỹ Anduril Industries vừa ra mắt sản phẩm kính thông minh tích hợp trên mũ bảo hiểm mang tên "EagleEye" (Mắt đại bàng).

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103008.webp)

Khi sử dụng, người lính có thể hạ tấm kính chắn gió xuống để bao bọc kín phần đầu.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103009.webp)

Chiếc mũ bảo hiểm này tích hợp một màn hình hiển thị ngay trước mắt người lính, cho phép lồng ghép hình ảnh thực tế với bản đồ, luồng dữ liệu từ drone (UAV) và các cảm biến khác, giúp người lính nắm bắt toàn diện tình hình chiến trường.

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103010.webp)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103011.webp)

Sản phẩm dự kiến sẽ được bàn giao cho quân đội Mỹ vào năm sau. Trông chiếc mũ này rất giống với những chiếc kính thực tế ảo metaverse trong tương lai.

## 文章

1. [Cách thiết lập một trang web chạy trên mạng ẩn danh Tor (Dark Web)](https://flower.codes/2025/10/23/onion-mirror.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103015.webp)

Các trang web chạy trên mạng ẩn danh Dark Web (sở hữu tên miền có hậu tố `.onion`) chỉ cho phép truy cập thông qua trình duyệt Tor. Tác giả ghi lại toàn bộ quy trình thiết lập trang web ẩn danh cá nhân, các bước triển khai nhìn chung không quá phức tạp.

2. [Phương pháp đơn giản giúp chặn và lọc bot cào dữ liệu](https://fxgn.dev/blog/anubis/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110403.webp)

Tác giả đề xuất một giải pháp gọn nhẹ giúp máy chủ web chủ động từ chối và chặn đứng các yêu cầu cào dữ liệu từ bot tự động, không yêu cầu thiết lập hệ thống tường lửa phức tạp mà chỉ cần cấu hình ngay trên máy chủ web (tác giả sử dụng máy chủ web Caddy).

3. [Bạn có biết đến các API xử lý bảng HTML (HTML Table API) không?](https://christianheilmann.com/2025/10/08/abandonware-of-the-web-do-you-know-that-there-is-an-html-tables-api/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110404.webp)

Có một bộ API trình duyệt cổ xưa hỗ trợ thao tác trực tiếp với bảng HTML bằng JavaScript. Mặc dù nhiều năm qua rất ít lập trình viên sử dụng bộ API này nhưng các trình duyệt hiện nay vẫn tiếp tục duy trì hỗ trợ bình thường.

4. [Báo cáo tổng quan về sự phát triển của công cụ biên dịch (Compiler Backend)](https://abhinavsarkar.net/notes/2025-compiler-backend-survey/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110612.webp)

Bài viết tổng hợp và đánh giá tổng quan về thực trạng phát triển hiện tại của các công cụ và trình biên dịch mã nguồn.

5. [Khởi động Raspberry Pi thông qua kết nối mạng (Network Booting) là phương án tối ưu nhất](https://www.xda-developers.com/booting-raspberry-pi-network-huge-performance-difference/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202510/bg2025103101.webp)

Thông thường, thiết bị Raspberry Pi sẽ khởi động hệ điều hành thông qua thẻ nhớ SD. Tác giả khuyên bạn nên chuyển đổi sang hình thức mạng khởi động (Network Booting). Giải pháp này cực kỳ tiện lợi đối với những ai cần liên tục thay đổi hệ điều hành hoặc phải quản lý cùng lúc nhiều thiết bị Raspberry Pi.

6. [Nhìn lại loạt phim hoạt hình Flash "Xiao Xiao" (小小作品)](https://animationobsessive.substack.com/p/when-stick-figures-fought) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110401.webp)

Trong giai đoạn từ năm 1999 đến 2006, loạt phim hoạt hình Flash "Xiao Xiao" (thường gọi là loạt phim "người que" đấu võ) do họa sĩ hoạt hình Chu Chí Cường sáng tạo đã gây sốt trên khắp không gian mạng Trung Quốc. Bài viết nhìn lại lịch sử và những câu chuyện thú vị về loạt phim kinh điển này, thứ mà ngày nay ít người còn nhớ tới.

## 工具

1. [Zensical](https://github.com/zensical/zensical)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110613.webp)

Phiên bản nâng cấp do tác giả của công cụ tạo trang tài liệu tĩnh nổi tiếng [Material for MkDocs](https://github.com/squidfunk/mkdocs-material/) phát triển. Dự án tương thích tốt với các cấu hình MkDocs sẵn có nhưng xử lý triệt để nhiều điểm hạn chế của phiên bản cũ.

2. [Affinity](https://www.affinity.studio/)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110203.webp)

Bộ công cụ thiết kế đồ họa chất lượng cao chạy trên máy tính, được định vị là giải pháp thay thế cho phần mềm Photoshop. Sau khi được Canva mua lại, hiện tại hãng đang cho phép tải về và sử dụng hoàn toàn miễn phí.

3. [FileBrowser Quantum](https://github.com/gtsteffaniak/filebrowser)

Trình quản lý tệp tin dựa trên giao diện web tự lưu trữ (self-hosted). Tham khảo thêm [bài viết giới thiệu](https://www.xda-developers.com/self-hosted-free-open-source-web-based-file-browser/).

4. [Texo](https://github.com/alephpi/Texo)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110202.webp)

Công cụ nhận diện ký tự quang học (OCR) mã nguồn mở dành cho công thức toán học, thực thi nhận diện trực tiếp ở phía client để chuyển đổi ảnh chụp công thức sang cấu trúc cú pháp LaTeX. [Trang chạy thử trực tuyến](https://texocr.netlify.app/ocr). (Đóng góp từ [@alephpi](https://github.com/ruanyf/weekly/issues/8026))

5. [TDesign uniapp](https://github.com/novlan1/tdesign-uniapp)

Thư viện adapter uniapp không chính thức cho bộ thành phần giao diện TDesign của Tencent, hỗ trợ chạy trên H5, mini program WeChat, mini program Alipay và ứng dụng di động App. (Đóng góp từ [@novlan1](https://github.com/ruanyf/weekly/issues/8022))

6. [GreenWall](https://github.com/zmrlft/GreenWall)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110201.webp)

Công cụ hỗ trợ tự động vẽ các hình ảnh, ký tự tùy biến lên bảng đóng góp (contribution calendar) màu xanh lá trên trang cá nhân GitHub của bạn. (Đóng góp từ [@zmrlft](https://github.com/ruanyf/weekly/issues/8024))

7. [BakLab](https://github.com/biliqiqi/baklab-web)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110502.webp)

Nền tảng cộng đồng mã nguồn mở, kết hợp hài hòa giữa tính năng diễn đàn thảo luận truyền thống và giao diện chat trò chuyện thời gian thực. Link tiêu đề dẫn tới repo frontend, tham khảo thêm [trang chủ dự án](https://baklab.app). (Đóng góp từ [@oodzchen](https://github.com/ruanyf/weekly/issues/8050))

8. [Tra cứu ngày lễ Trung Quốc (chinese-days)](https://github.com/vsme/chinese-days)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110512.webp)

Thư viện cung cấp các hàm hỗ trợ tra cứu lịch nghỉ lễ, ngày tiết khí của Trung Quốc, dữ liệu được cập nhật tự động hàng ngày thông qua GitHub Action, hỗ trợ đăng ký nhận lịch định dạng iCal. (Đóng góp từ [@vsme](https://github.com/ruanyf/weekly/issues/8059))

Ngoài ra còn có [một dự án tương tự](https://github.com/tomandjerry136/hodiday) cung cấp dữ liệu ngày lễ Trung Quốc định dạng tệp JSON. (Đóng góp từ [@tomandjerry136](https://github.com/ruanyf/weekly/issues/8062))

9. [QiLuo (祺洛)](https://github.com/chelunfu/qiluo_admin)

Giao diện quản trị hệ thống web phát triển hoàn toàn trên tech stack của Rust, sử dụng framework Axum kết hợp thư viện Sea ORM. (Đóng góp từ [@chelunfu](https://github.com/ruanyf/weekly/issues/8106))

10. [navsite](https://github.com/wubh2012/navsite)

Công cụ hỗ trợ tự động chuyển đổi bảng dữ liệu nhiều chiều của Feishu (Lark) thành một trang web danh bạ, điều hướng trực quan. (Đóng góp từ [@wubh2012](https://github.com/ruanyf/weekly/issues/8109))

## AI 相关

1. [Jta](https://github.com/hikanner/jta)

Công cụ dòng lệnh mã nguồn mở sử dụng mô hình AI để dịch thuật tự động các tệp JSON ngôn ngữ, hỗ trợ dịch thuật đa ngôn ngữ lên tới 27 ngôn ngữ khác nhau với nhiều tùy chọn cấu hình. (Đóng góp từ [@hikanner](https://github.com/ruanyf/weekly/issues/8014))

2. [Smart Excalidraw](https://github.com/liujuntao123/smart-excalidraw-next)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110405.webp)

Phiên bản tích hợp AI của công cụ vẽ tay Excalidraw, cho phép người dùng sử dụng mô tả ngôn ngữ tự nhiên để AI tự động vẽ ra các sơ đồ theo phong cách vẽ phác thảo bằng tay. [Trang chạy thử trực tuyến](https://smart-excalidraw.aizhi.site/). (Đóng góp từ [@liujuntao123](https://github.com/ruanyf/weekly/issues/8029))

3. [VibeVoiceFusion](https://github.com/zhao-kun/VibeVoiceFusion)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110406.webp)

Ứng dụng web mã nguồn mở hỗ trợ tổng hợp giọng nói đa âm sắc, tích hợp sẵn các thuật toán nhân bản giọng nói (voice cloning) chất lượng cao. (Đóng góp từ [@zhao-kun](https://github.com/ruanyf/weekly/issues/8030))

4. [Mini-Kode](https://github.com/minmaxflow/mini-kode)

Dự án trợ lý lập trình AI mã nguồn mở được thiết kế cho mục đích học tập và giảng dạy, giúp lập trình viên hiểu rõ cách thức phát triển và vận hành của các công cụ hỗ trợ viết mã bằng AI. (Đóng góp từ [@minmaxflow](https://github.com/ruanyf/weekly/issues/8035))

5. [SQLBot](https://github.com/dataease/SQLBot)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110407.webp)

Dịch vụ web mã nguồn mở hỗ trợ kết nối trực tiếp mô hình AI lớn với cơ sở dữ liệu của bạn, cho phép người dùng truy vấn dữ liệu bằng ngôn ngữ tự nhiên (công nghệ text-to-SQL). (Đóng góp từ [@maninhill](https://github.com/ruanyf/weekly/issues/8039))

6. [Docutranslate](https://github.com/xunbu/docutranslate)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110408.webp)

Công cụ dịch thuật tài liệu đa định dạng viết bằng Python, sử dụng các mô hình AI để xử lý bản dịch trực tiếp trên cấu trúc tệp tài liệu. (Đóng góp từ [@xunbu](https://github.com/ruanyf/weekly/issues/8042))

7. [Paper Burner X](https://github.com/Feather-2/paper-burner-x)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110501.webp)

Ứng dụng web mã nguồn mở hỗ trợ xử lý và đọc hiểu các bài báo khoa học, tài liệu nghiên cứu, tích hợp các tính năng dịch thuật tài liệu, hỏi đáp thông minh với nội dung tài liệu. (Đóng góp từ [@Feather-2](https://github.com/ruanyf/weekly/issues/8049))

## 资源

1. [Cửa hàng ứng dụng App Store phiên bản Web](https://apps.apple.com/)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110504.webp)

Apple tuần này đã chính thức ra mắt trang web App Store chạy trên trình duyệt tại địa chỉ `apps.apple.com`. Mặc dù người dùng không thể trực tiếp cài đặt ứng dụng từ trình duyệt web vào thiết bị, nhưng trang web cung cấp một cổng tìm kiếm và khám phá ứng dụng trực quan trên môi trường web.

Nhiều lập trình viên đã phân tích [mã nguồn frontend](https://github.com/rxliuli/apps.apple.com) của trang web và phát hiện ra Apple đã sử dụng framework Svelte để phát triển dự án này.

2. [ASCIIMoon](https://asciimoon.com/)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070313.webp)

Trang web đơn giản hiển thị hình dạng của mặt trăng (trăng non, trăng khuyết, trăng tròn) theo thời gian thực của ngày hiện tại được vẽ hoàn toàn bằng các ký tự nghệ thuật ASCII.

## 图片

1. [Tàu khí cầu Hindenburg](https://rarehistoricalphotos.com/hindenburg-interior-photos/)

Tàu khí cầu Hindenburg là một khinh khí cầu chở khách khổng lồ do Đức chế tạo vào những năm 1930, từng thực hiện các chuyến bay thương mại chở khách vượt Đại Tây Dương từ châu Âu sang Mỹ.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110614.webp)

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024090801.webp)

Với chiều dài lên tới 245 mét, nó được ví như một tàu sân bay khổng lồ di chuyển trên bầu trời, với sức chứa từ 50 đến 70 hành khách.

Không gian nội thất bên trong tàu khí cầu được thiết kế vô cùng sang trọng và xa hoa, trang bị đầy đủ các phòng ngủ cá nhân riêng biệt cùng nhà hàng ăn uống cao cấp. Người thời nay thật khó có thể hình dung các chuyến bay xuyên lục địa thời kỳ đó lại sở hữu mức độ tiện nghi và thoải mái cao đến vậy.

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024090802.webp)

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024090803.webp)

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024090804.webp)

Tuy nhiên, do túi khí của tàu sử dụng khí Hydro để bay nên tiềm ẩn nguy cơ cháy nổ cực kỳ cao. Vào tháng 5 năm 1937, một vụ cháy lớn bất ngờ bộc phát trên tàu đã cướp đi sinh mạng của hơn 30 người, và kể từ sau thảm kịch đó, kỷ nguyên sử dụng khinh khí cầu làm phương tiện giao thông vận tải hành khách cũng chính thức khép lại.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110615.webp)

## 文摘

1. [Các tập đoàn công nghệ sa thải hàng loạt nhân sự để "rót tiền đầu tư AI"](https://www.reddit.com/r/ArtificialInteligence/comments/1oj52xx/tech_companies_are_firing_everyone_to_fund_ai_but/)

Tháng trước, Amazon công bố đợt cắt giảm nhân sự lên tới 30.000 người, đánh dấu đợt sa thải có quy mô lớn nhất trong lịch sử hoạt động của hãng. Trước đó, Microsoft cũng đã cắt giảm 15.000 nhân sự, Meta sa thải 3.600 người, và Google cũng cắt giảm hàng trăm nhân viên trong năm nay. Tính riêng trong năm 2025, đã có hơn 180.000 nhân sự hoạt động trong ngành công nghệ Internet bị mất việc làm.

Ở chiều ngược lại, các tập đoàn lớn này đã rót tới hơn 300 tỷ USD vào lĩnh vực AI trong năm nay. Rõ ràng, hành động sa thải hàng loạt là nhằm "tối ưu chi phí và giải phóng nguồn vốn để tập trung đầu tư cho AI".

Tuy nhiên, vấn đề cốt lõi là họ không thực sự tiết kiệm được tiền. Chi phí đầu tư khổng lồ cho AI vượt xa số tiền họ tiết kiệm được từ việc cắt giảm nhân sự. Thêm vào đó, nguồn vốn khổng lồ đổ vào AI hiện tại chưa hề mang lại doanh thu bù đắp, khoản phí thu về từ người dùng dịch vụ AI chỉ là muối bỏ bể so với chi phí vận hành khổng lồ đã bỏ ra.

Vậy dòng tiền khổng lồ đầu tư cho AI của các ông lớn công nghệ rốt cuộc đã trôi về đâu? Câu trả lời là dòng tiền thực chất chỉ xoay vòng mua bán lẫn nhau giữa các hãng: Apple trả tiền cho Google, Google chi tiền cho Nvidia, và Nvidia lại trả tiền cho TSMC để đặt hàng sản xuất chip.

Hoạt động mua bán qua lại này giúp đẩy doanh số bán hàng của các công ty lên mức cao kỷ lục, từ đó trực tiếp thúc đẩy giá cổ phiếu của họ tăng vọt trên thị trường chứng khoán.

Công chúng thấy giá cổ phiếu tăng liên tục liền đổ xô vào mua cổ phiếu của các tập đoàn này, tiếp tục thổi bùng cơn sốt giá cổ phiếu.

Nhóm 7 ông lớn công nghệ (Magnificent Seven) – gồm Apple, Microsoft, Nvidia, Amazon, Alphabet, Meta và Tesla – hiện sở hữu tổng giá trị vốn hóa thị trường khổng lồ lên tới 17 nghìn tỷ USD, với chỉ số P/E trung bình đạt mức cao ngất ngưỡng 35 lần. Để so sánh, nếu loại bỏ 7 tập đoàn này ra, chỉ số P/E trung bình của nhóm S&P 500 chỉ dừng lại ở mức 15,5 lần.

Tại sao các tập đoàn này lại được thị trường định giá cao với mức chiết khấu lớn đến vậy? Bởi tất cả mọi người đều tin tưởng rằng AI chắc chắn sẽ mang lại nguồn lợi nhuận khổng lồ cho họ trong tương lai.

Nhưng thực tế hiện tại là các hãng này chưa hề kiếm được tiền từ AI, họ mới chỉ đang đốt tiền cho AI và chủ yếu là tiêu tiền qua lại lẫn nhau để kiến tạo nên một bức tranh tăng trưởng ảo.

Tệ hơn nữa là giờ đây họ không thể dừng lại. Bởi chỉ cần bất kỳ một ông lớn nào công bố cắt giảm hay dừng đầu tư cho AI, giá cổ phiếu của họ lập tức sẽ lao dốc không phanh do giới đầu tư tháo chạy. Do đó, ngay cả khi các khoản đầu tư khổng lồ cho AI chưa mang lại quả ngọt, họ vẫn phải tiếp tục đốt tiền để duy trì niềm tin và giữ giá cổ phiếu.

Đây chính là thực trạng hiện tại: sự hưng thịnh của AI đang được xây dựng hoàn toàn trên nguồn vốn đầu tư khổng lồ của các tập đoàn lớn. Để có tiền đầu tư, các tập đoàn buộc phải cắt giảm các mảng hoạt động khác (bao gồm sa thải nhân sự), trong khi dòng tiền đầu tư thực chất chỉ là dòng tiền chạy vòng quanh giữa các hãng. Tất cả dường như đều đang đặt cược vào việc dòng tiền đầu tư này sẽ không bao giờ đứt gãy, và sẽ có ngày họ thu hồi lại được toàn bộ vốn liếng đã bỏ ra.

## 言论

1.

Tôi từng tuyên bố htmx sẽ không bao giờ có phiên bản thứ 3, nhưng tôi chưa bao giờ nói rằng nó sẽ không có phiên bản thứ 4.

-- [Carson Gross](https://htmx.org/essays/the-fetchening/), nhà sáng lập dự án htmx, người từng tuyên bố sẽ không phát triển htmx 3.0 nhưng tuần này đã bất ngờ công bố phát hành thẳng phiên bản htmx 4.0.

2.

Chúng tôi nhận được thông báo từ phía Google cho biết họ đã quét và phát hiện ra một lỗ hổng bảo mật trong mã nguồn của chúng tôi.

Chúng tôi rất coi trọng vấn đề bảo mật. Tuy nhiên, việc các tập đoàn công nghệ khổng lồ sử dụng AI để tự động quét mã nguồn của các dự án do cộng đồng tình nguyện viên bảo trì, rồi gửi thông báo yêu cầu các tình nguyện viên phải sửa lỗi miễn phí cho họ, liệu điều đó có thực sự công bằng hay không?

-- [Đội ngũ phát triển dự án FFmpeg](https://x.com/FFmpeg/status/1984178359354483058)

3.

Trong vòng 10 năm tới, hơn 70 nghìn tỷ USD tài sản thừa kế trên toàn cầu sẽ được chuyển giao trực tiếp cho các thế hệ kế cận, điều này dự báo sẽ càng làm trầm trọng thêm tình trạng bất bình đẳng xã hội.

-- [Báo The Guardian của Anh](https://www.theguardian.com/inequality/2025/nov/03/more-than-70tn-of-inherited-wealth-over-next-decade-will-widen-inequality-economists-warn)

4.

Tại sao yếu tố may mắn lại vô cùng quan trọng trong đời người? Bởi vì may mắn sẽ giúp bạn rút ngắn đáng kể thời gian tích lũy ban đầu, từ đó giúp bạn tiếp cận được với những cơ hội lớn hơn sớm hơn. Điều này tương tự như việc một khi bạn đã có tiền, việc kiếm thêm nhiều tiền hơn nữa sẽ trở nên dễ dàng hơn rất nhiều.

-- [《Cuộc đời là một trò chơi xác suất》](https://zachholman.com/posts/money-off-the-table)

5.

Kể từ sau sự xuất hiện của AI, lộ trình phát triển kỹ năng của lập trình viên đã hoàn toàn thay đổi.

Bạn bắt buộc phải chuyển đổi trọng tâm từ việc thấu hiểu cú pháp ngôn ngữ sang thấu hiểu kiến trúc hệ thống, và năng lực cốt lõi của bạn phải dịch chuyển từ việc viết mã đơn thuần sang thiết kế kiến trúc, bảo mật và khả năng tương tác, cộng tác hiệu quả giữa người và máy.

Tương lai của ngành phần mềm sẽ thuộc về những ai sở hữu năng lực hình dung, xây dựng và bảo trì các hệ thống phức tạp quy mô lớn.

-- [《Sự tiến hóa của phát triển phần mềm》](https://guptadeepak.com/the-evolution-of-software-development-from-machine-code-to-ai-orchestration/)

## 往年回顾

[Next.js đã đi đến điểm cuối và Zed sẽ thay thế VS Code?](https://www.ruanyifeng.com/blog/2024/11/weekly-issue-325.html) (#325)

[Thí nghiệm của Peter Thiel](https://www.ruanyifeng.com/blog/2023/10/weekly-issue-275.html) (#275)

[Diễn viên quần chúng NPC cũng là một nghề nghiệp thực thụ](https://www.ruanyifeng.com/blog/2022/09/weekly-issue-225.html) (#225)

[Độ rộng kiến thức vs Độ sâu kiến thức](https://www.ruanyifeng.com/blog/2021/09/weekly-issue-175.html) (#175)

(Hết)
