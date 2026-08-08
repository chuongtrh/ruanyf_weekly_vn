# 科技爱好者周刊（第 224 期）：Figma 为什么赢了 Sketch

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần。

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn。

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2599) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập。

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081107.webp)

Làm thế nào để thu hồi vỏ tên lửa đẩy khi rơi tự do? Công nghệ của SpaceX sử dụng hai con tàu chuyên dụng được trang bị một hệ thống lưới thu gom khổng lồ di chuyển trên biển để hứng trọn các mảnh vỏ tên lửa đang rơi xuống từ không trung. (Nguồn: [NASASpaceFlight](https://www.nasaspaceflight.com/2022/08/spacex-fairing-recovery/))

## 本周话题：Figma 为什么赢了 Sketch

Tuần trước, tập đoàn Adobe đã chính thức [công bố thương vụ](https://36kr.com/p/1917326805803014) mua lại phần mềm thiết kế đồ họa Figma với mức giá kỷ lục lên tới 20 tỷ USD.

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092001.webp)

Đây là một mức giá thâu tóm cực kỳ đắt đỏ. Doanh thu năm ngoái của Figma đạt khoảng 50 triệu USD và dự kiến đạt mốc 400 triệu USD trong năm nay. Ngay cả khi con số dự báo 400 triệu USD là chính xác, giá trị thương vụ vẫn gấp tới 50 lần doanh thu năm của công ty.

Để dễ so sánh, thương vụ Microsoft mua lại GitHub vào năm 2018 chỉ có giá 7,5 tỷ USD khi doanh thu năm của GitHub khi đó đã đạt khoảng 300 triệu USD.

**Tại sao một phần mềm thiết kế chuyên dụng chỉ mới ra mắt chính thức vào năm 2016 lại có giá trị lớn đến vậy?**

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092002.webp)

Figma sở hữu một đối thủ cạnh tranh trực tiếp là [Sketch](https://www.sketch.com/) với tính năng tương đương. Cho đến tận năm 2019, định giá thị trường của Sketch vẫn vượt trội so với Figma. Nhiều người thậm chí đã dự đoán về viễn cảnh Sketch sẽ thâu tóm Figma, nhưng thực tế Figma đã bứt phá ngoạn mục và bỏ xa đối thủ.

Dưới góc độ kỹ thuật phần mềm, sự khác biệt cốt lõi quyết định thắng bại của hai sản phẩm nằm ở lựa chọn nền tảng:

Sketch được thiết kế là một ứng dụng bản xứ (Native App) dành riêng cho hệ điều hành macOS, yêu cầu tải về cài đặt trên máy Mac và chỉ cung cấp phiên bản trả phí. **Trong khi đó, Figma được phát triển là một ứng dụng chạy trực tiếp trên nền tảng Web (Web App), hỗ trợ sử dụng miễn phí trên mọi thiết bị có trình duyệt internet.**

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092004.webp)

Một bên yêu cầu người dùng phải có máy Mac và trả phí bản quyền, một bên chỉ cần mở trình duyệt là có thể làm việc ngay lập tức. Ưu thế tiếp cận người dùng của Figma là quá rõ ràng.

Tuy nhiên, bài toán kỹ thuật không hề đơn giản. Ứng dụng native có khả năng can thiệp sâu vào API hệ thống để tối ưu hiệu năng đồ họa, còn ứng dụng web thường bị giới hạn bởi năng lực xử lý của trình duyệt. 

Để giải quyết triệt để rào cản hiệu năng này, Figma đã lựa chọn [ngôn ngữ lập trình Rust](https://www.figma.com/blog/rust-in-production-at-figma/). Toàn bộ logic xử lý đồ họa cốt lõi của Figma không viết bằng JavaScript mà viết bằng Rust, sau đó được biên dịch sang định dạng WebAssembly để thực thi trực tiếp trên trình duyệt với tốc độ xử lý đồ họa tiệm cận ứng dụng native.

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092006.webp)

**Figma hiện là một trong những doanh nghiệp đi đầu thế giới về ứng dụng công nghệ WebAssembly.** CTO của Figma, Evan Wallace (hình dưới, bên phải), vì không hài lòng với tốc độ đóng gói chậm chạp của JavaScript đã tự phát triển công cụ đóng gói thế hệ mới [ESbuild](https://esbuild.github.io/faq/#benchmark-details) viết bằng Go, mang lại tốc độ xử lý nhanh hơn 100 lần so với Webpack (0,33 giây so với 41,53 giây).

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092007.webp)

Khi nút thắt hiệu năng của trình duyệt được tháo gỡ mang lại trải nghiệm mượt mà không thua kém phần mềm cài đặt, Figma đã nhanh chóng giành chiến thắng tuyệt đối trước Sketch.

Những năm gần đây, giới phát triển phần mềm thường có xu hướng coi ứng dụng native là tiêu chuẩn bắt buộc và chỉ coi ứng dụng Web là phương án phụ. Nhiều sản phẩm dù có phiên bản Web rất tốt vẫn cố gắng sử dụng Electron để đóng gói thành phiên bản desktop cài đặt cho người dùng. Thương vụ 20 tỷ USD của Figma đã chứng minh điều ngược lại: **Một ứng dụng Web thuần túy được đầu tư bài bản về công nghệ hoàn toàn có thể tạo nên thành công vang dội.**

Bên cạnh đó, đối với tập đoàn Adobe vốn đi lên từ các phần mềm native cài đặt trên máy tính, chiến lược chuyển dịch dịch vụ lên đám mây (Cloud) đang được đẩy mạnh thông qua hệ thống [Adobe Creative Cloud](https://creativecloud.adobe.com/zh-Hans) và việc miễn phí hóa phiên bản Web của Photoshop. Thương vụ thâu tóm Figma không chỉ nhằm loại bỏ một đối thủ cạnh tranh lớn mà còn giúp Adobe tiếp cận được các công nghệ WebAssembly và kinh nghiệm phát triển Web App đỉnh cao để phục vụ cho hành trình đám mây hóa toàn bộ hệ sinh thái phần mềm của mình.

## 科技动态

1、[Ý tưởng sử dụng máy gia tốc hạt phục vụ khoan giếng địa nhiệt siêu sâu](https://news.mit.edu/2022/quaise-energy-geothermal-0628)

Một nhà vật lý học tại MIT chuyên nghiên cứu về máy gia tốc hạt đã đề xuất ý tưởng độc đáo: sử dụng các chùm hạt năng lượng cao được gia tốc để bắn phá nung chảy đất đá phục vụ khoan giếng sâu trong lòng đất:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080502.webp)

Các thử nghiệm ban đầu chứng minh tính khả thi của giải pháp. Dự án đang được MIT tài trợ nghiên cứu để thiết lập mũi khoan năng lượng có khả năng khoan sâu tới 20 km xuống lòng đất nhằm dẫn nguồn nhiệt lượng 500°C phục vụ sản xuất điện địa nhiệt sạch thay thế than đá. Khó khăn lớn nhất hiện nay là giải pháp xử lý lượng hơi bốc lên từ đá bị nung chảy trong lòng giếng sâu.

2、[Thiết bị mô phỏng đĩa than phát nhạc cho điện thoại của Yamaha](https://www.yamaha-smartphone-turntable)

Hãng Yamaha giới thiệu sản phẩm đồ chơi công nghệ độc đáo dành cho những người yêu thích trải nghiệm nghe nhạc đĩa than cổ điển trên điện thoại di động:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080604.webp)

Người dùng đặt điện thoại lên thiết bị và khởi động ứng dụng đi kèm mô phỏng đĩa nhạc đang quay. Khi hạ kim đọc nhạc (thực chất là một đầu bút cảm ứng) lên màn hình điện thoại, nhạc sẽ bắt đầu phát. Việc di chuyển kim đọc nhạc cũng mang lại các hiệu ứng âm thanh chà đĩa (scratching) tương tự đầu đĩa than thực tế.

3、[Mô hình nông nghiệp trồng lúa không người lái đạt năng suất cao tại Quý Châu](http://www.gz.chinanews.com.cn/dcsj/2022-09-16/doc-ihcearke9348308.shtml)

Mô hình thí điểm "Nông trường trồng lúa không người lái" đầu tiên tại tỉnh Quý Châu đã hoàn thành vụ thu hoạch đầu tiên với sản lượng tốt:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092105.webp)

Toàn bộ quy trình canh tác từ gieo hạt, cấy lúa cho đến thu hoạch đều được vận hành hoàn toàn tự động bằng máy móc cơ giới hóa không người lái:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092103.webp)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092104.webp)

Hệ thống phun thuốc bảo vệ thực vật và phân bón tự động bằng máy bay không người lái:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092106.webp)

Hệ thống máy gặt đập tự hành hoạt động trên cánh đồng:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092102.webp)

Toàn bộ hoạt động của máy móc nông nghiệp được kỹ sư giám sát và điều khiển trực quan thông qua ứng dụng trên điện thoại di động.

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092107.webp)

4、[Đảng chính trị đầu tiên vận hành dựa trên mô hình trí tuệ nhân tạo](https://www.thelocal.dk/20220804/danish-ai-driven-political-party-eyes-parliament/)

Đan Mạch ghi nhận sự ra đời của một đảng chính trị mới mang tên "Đảng Tổng hợp" (The Synthetic Party) với toàn bộ cương lĩnh và chính sách hành động đều do mô hình AI đề xuất:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080801.webp)

Mục tiêu hoạt động của mô hình AI này là tính toán tối ưu hóa các giải pháp chính trị nhằm đạt mức cao nhất các chỉ tiêu phát triển bền vững của Liên Hợp Quốc. Đảng đang tích cực hoàn thiện các thủ tục tranh cử để tham gia vào kỳ bầu cử quốc hội Đan Mạch vào năm tới.

## 文章

1\. [Triển vọng thương mại hóa công nghệ kết nối vệ tinh trên điện thoại thông minh](https://finance.sina.com.cn/tech/tele/2022-09-19/doc-imqmmtha7923057.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092012.webp)

Bài viết phân tích thực trạng phát triển hạ tầng và công nghệ liên lạc qua vệ tinh của Trung Quốc, giới thiệu dự án phóng vệ tinh viễn thông quỹ đạo thấp của startup GalaxySpace nhằm thiết lập mạng truyền thông băng thông rộng kết nối trực tiếp thiết bị di động.

2\. [Kinh nghiệm thực tế lựa chọn thiết bị máy in 3D cá nhân cho người mới bắt đầu](https://sspai.com/post/75665)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022091506.webp)

Tác giả chia sẻ chi tiết kinh nghiệm đánh giá tính năng, độ phân giải in và ngân sách đầu tư để lựa chọn chiếc máy in 3D cá nhân đầu tiên phục vụ sáng tạo các mô hình đồ chơi tại nhà.

3\. [Tổng hợp 7 công cụ trực quan hóa kiến trúc thư mục mã nguồn dự án](https://lmy.medium.com/7-tools-for-visualizing-a-codebase-41b7cddb1a14)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040301.webp)

Bài viết giới thiệu 7 tiện ích hỗ trợ phân tích và hiển thị trực quan các mối quan hệ phụ thuộc (dependencies) và cấu trúc phân cấp file bên trong một kho chứa mã nguồn lớn để hỗ trợ lập trình viên mới tiếp cận dự án.

4\. [Những trường hợp biên phức tạp khi xây dựng cơ sở dữ liệu thông tin âm nhạc](https://dustri.org/b/horrible-edge-cases-to-consider-when-dealing-with-music.html)（Tiếng Anh）

Tác giả liệt kê các tình huống thực tế khó xử lý khi thiết kế DB âm nhạc: các ban nhạc trùng tên nhau, nghệ sĩ thay đổi nghệ danh qua các thời kỳ, hoặc các ca khúc đồng sáng tác có sự tham gia của hàng trăm nghệ sĩ phối khí.

5\. [Hướng dẫn cấu hình xác thực lệnh `sudo` bằng Touch ID trên máy MacBook](https://sixcolors.com/post/2020/11/quick-tip-enable-touch-id-for-sudo/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061608.webp)

Bài viết hướng dẫn cấu hình hệ thống macOS để cho phép lập trình viên xác thực quyền chạy lệnh quản trị `sudo` trên Terminal bằng vân tay Touch ID tiện lợi thay vì phải gõ mật khẩu thủ công.

6\. [Phân biệt cơ chế hoạt động của toán tử `is` và `==` trong Python](https://anvil.works/articles/pointers-in-my-python-2)（Tiếng Anh）

Bài viết giải thích rõ sự khác biệt bản chất: toán tử `is` dùng so khớp địa chỉ vùng nhớ của hai đối tượng (so sánh con trỏ), còn toán tử `==` dùng so sánh tính tương đương về mặt giá trị lưu trữ của chúng.

7\. [Khám phá nguyên lý đo đạc nồng độ bụi mịn PM 2.5 của máy giám sát không khí](https://woodgears.ca/dust/dylos.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080602.webp)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080603.webp)

Tác giả tiến hành tháo dỡ thiết bị đo bụi mịn gia đình để tìm hiểu nguyên lý hoạt động: cảm biến sử dụng một chùm laser chiếu qua buồng khí để đếm số lượng và cường độ của xung ánh sáng bị tán xạ khi gặp các hạt bụi lơ lửng, từ đó tính toán chỉ số chất lượng không khí tương ứng.

8\. [Khuyến nghị tắt tính năng tự động dọn rác định kỳ của Git](https://donatstudios.com/yagni-git-gc)（Tiếng Anh）

Tác giả phân tích cơ chế dọn rác mặc định của Git (`git gc`) vốn tự động xóa bỏ các commits mồ côi (không thuộc nhánh nào) và khuyên người dùng nên tắt tính năng này để có thể khôi phục lại các đoạn code đã mất khi thao tác sai lệnh.

## 工具

1、[kvass: Công cụ lưu trữ dữ liệu key-value gọn nhẹ hoạt động cục bộ](https://github.com/maxmunzel/kvass)

Tiện ích lưu trữ dữ liệu key-value đơn giản chạy trên máy tính cá nhân, hỗ trợ truy xuất qua dòng lệnh CLI hoặc mở cổng dịch vụ API HTTP để chia sẻ dữ liệu nhanh chóng.

2、[ERNIE-ViLG: Mô hình trí tuệ nhân tạo sinh ảnh từ văn bản tiếng Trung của Baidu](https://wenxin.baidu.com/moduleApi/ernieVilg)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092108.webp)

Mô hình AI tạo ảnh từ văn bản tiếng Trung tương tự DALL-E do Baidu phát triển (bạn đọc cũng có thể tham khảo thêm dịch vụ tạo ảnh tiếng Anh tương tự mang tên [Elbo](https://art.elbo.ai/)).

3、[Simple Admin: Hệ thống quản trị backend dạng microservices viết bằng Go](https://github.com/suyuan32/simple-admin-core)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092109.webp)

Mã nguồn mở xây dựng hệ thống quản trị nội dung backend và phân quyền người dùng dạng microservices gọn nhẹ viết bằng ngôn ngữ Go. (Đóng góp của [@suyuan32](https://github.com/ruanyf/weekly/issues/2632))

4、[text-watermark: Thư viện chèn chữ ký bản quyền ẩn vào văn bản](https://github.com/zengkan0703/text-watermark)

Thư viện npm hỗ trợ lập trình viên nhúng (hoặc giải mã) các thông điệp ẩn vào văn bản thô bằng cách chèn các ký tự có độ rộng bằng không (zero-width characters). (Đóng góp của [@zengkan0703](https://github.com/ruanyf/weekly/issues/2634))

5、[proxy-web-storage: Thư viện JavaScript đóng gói LocalStorage bằng Proxy](https://github.com/KID-joker/proxy-web-storage)

Thư viện hỗ trợ đóng gói LocalStorage và SessionStorage bằng ES6 Proxy, bổ sung các tính năng hữu ích như lắng nghe sự kiện thay đổi dữ liệu và thiết lập hạn sử dụng cho key lưu trữ. (Đóng góp của [@KID-joker](https://github.com/ruanyf/weekly/issues/2643))

6、[TinyTeX: Bản phân phối LaTeX siêu gọn nhẹ dành cho lập trình viên](https://yihui.org/tinytex/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072607.webp)

Phiên bản rút gọn của bộ công cụ soạn thảo tài liệu khoa học TeX Live với dung lượng cài đặt chỉ khoảng 100 MB, hỗ trợ biên dịch tốt các ký tự tiếng Trung.

7、[Keet: Ứng dụng trò chuyện nhắn tin mã hóa bảo mật dạng P2P](https://keet.io/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072615.webp)

Phần mềm hỗ trợ nhắn tin, chia sẻ tệp tin và thực hiện cuộc gọi video trực tiếp mã hóa đầu cuối giữa các thiết bị mà không cần truyền dữ liệu qua máy chủ trung gian.

8、[Phoenix: Môi trường soạn thảo mã nguồn trực tuyến kế thừa từ Brackets](https://phcode.dev/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072701.webp)

Dự án phát triển phiên bản Web cho trình soạn thảo code Brackets nổi tiếng trước đây của Adobe, cung cấp trải nghiệm IDE lập trình trực quan ngay trên trình duyệt.

9、[HypeScript: Thư viện TypeScript hỗ trợ bắt lỗi biên dịch trực tiếp](https://github.com/ronami/HypeScript)

Tiện ích độc đáo cho phép lập trình viên viết code để bắt và xử lý các lỗi biên dịch của TypeScript compiler trực tiếp trong thời gian chạy.

10、[Dragonfly: Hệ quản trị cơ sở dữ liệu key-value hiệu năng cao thay thế Redis](https://github.com/dragonflydb/dragonfly)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053105.webp)

Hệ thống lưu trữ dữ liệu key-value trên bộ nhớ RAM tốc độ cao tương thích với API của Redis và Memcached, được tối ưu hóa kiến trúc đa luồng cho hiệu năng vượt trội.

## 活动

1、[Hội thảo trực tuyến chia sẻ kinh nghiệm vận hành ClickHouse từ ByteDance: ByteHouse](https://www.bagevent.com/event/8303002?bag_track=001)

ClickHouse là hệ quản trị cơ sở dữ liệu dạng cột (Column-oriented) nguồn mở do Yandex phát triển, hiện là giải pháp hàng đầu cho kho dữ liệu và phân tích dữ liệu lớn.

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092203.webp)

Sự kiện diễn ra vào chiều thứ Bảy (ngày 15 tháng 10) tới đây sẽ giới thiệu các chia sẻ từ đội ngũ kỹ sư ByteDance về lý do lựa chọn ClickHouse làm hạ tầng phân tích dữ liệu lớn với hơn 18.000 nodes, kinh nghiệm tối ưu hóa và giới thiệu sản phẩm ByteHouse được tinh chỉnh tối ưu dành cho doanh nghiệp. Độc giả quan tâm có thể đăng ký tham gia thông qua quét mã QR trong bài viết.

## 资源

1、[Life Stats: Trang web thống kê các chỉ số sinh học thú vị về cuộc đời bạn](https://neal.fun/life-stats/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070905.webp)

Người dùng chỉ cần nhập ngày sinh nhật, hệ thống sẽ tính toán hiển thị các thông số thú vị: tổng số ngày bạn đã sống, số nhịp tim đã đập, số lượng dân số Trái Đất tăng thêm tương ứng...

2\. [Bảng xếp hạng các chương trình Podcast tiếng Trung được nghe nhiều nhất](https://xyzrank.com/)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092111.webp)

Nền tảng tổng hợp dữ liệu xếp hạng hàng ngày của các chương trình phát thanh Podcast tiếng Trung dựa trên số liệu thống kê từ Apple Podcast và Xiaoyuzhou. (Đóng góp của [@alaskasquirrel](https://github.com/ruanyf/weekly/issues/2641))

3\. [Cloud Security Resources: Thư viện tổng hợp tài nguyên về bảo mật điện toán đám mây](https://wiki.teamssix.com/cloudsecurityresources/)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092110.webp)

Dự án mã nguồn mở tổng hợp các liên kết bài viết, công cụ và giáo trình học tập chuyên sâu về lĩnh vực an toàn thông tin và bảo mật đám mây. (Đóng góp của [@teamssix](https://github.com/ruanyf/weekly/issues/2635))

4、[Music for Programming: Danh sách nhạc không lời hỗ trợ lập trình viên tập trung](https://musicforprogramming.net/latest/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070912.webp)

Trang web chia sẻ các bản nhạc nền hòa tấu êm dịu giúp tăng hiệu năng làm việc cho lập trình viên, nổi bật với giao diện phong cách Terminal cổ điển.

5、[Programming Fonts: Trang web hỗ trợ so khớp các phông chữ lập trình](https://www.programmingfonts.org/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071013.webp)

Trang web tổng hợp gần 100 mẫu phông chữ lập trình phổ biến, cho phép người dùng thay đổi trực tiếp mẫu code để lựa chọn phông chữ phù hợp nhất cho IDE của mình.

## 图片

1\. [Bức ảnh chụp Trái Đất đầu tiên từ không gian vũ trụ](https://www.vintag.es/2022/02/first-photo-from-space.html)

Bạn có biết bức ảnh đầu tiên ghi lại hình ảnh của Trái Đất được chụp từ ngoài không gian khi nào?

Đáp án là ngày 24 tháng 10 năm 1946:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051506.webp)

Sau khi Chiến tranh Thế giới thứ II kết thúc, quân đội Mỹ đã đưa các tên lửa đẩy V2 thu giữ của Đức về sa mạc New Mexico để phục vụ nghiên cứu khoa học. Các kỹ sư đã tiến hành lắp đặt một máy quay phim 35mm được bảo vệ bên trong hộp thép kiên cố lên đỉnh tên lửa. Tên lửa đạt độ cao hành trình 105 km và thực hiện chụp ảnh Trái Đất mỗi 1,5 giây. Khi rơi tự do xuống đất đá sa mạc, dù máy quay bị hỏng nhưng cuộn phim bên trong hộp bảo vệ vẫn nguyên vẹn giúp nhân loại có được bức ảnh thô sơ đen trắng đầu tiên về hành tinh của mình.

2\. [Khám phá hang Sơn Đoòng - Hang động tự nhiên lớn nhất thế giới tại Việt Nam](https://mossandfog.com/earths-biggest-cave-will-blow-your-mind/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051008.webp)

Hang Sơn Đoòng nằm sâu trong vùng rừng núi tỉnh Quảng Bình, Việt Nam hiện giữ kỷ lục là hang động tự nhiên lớn nhất thế giới. Lối vào hang được một người dân địa phương tình cờ phát hiện vào năm 2009.

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051006.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051009.webp)

Hang động có chiều dài khoảng 9 km, chiều cao vòm hang đạt 200m và chiều rộng 150m. Bên trong hang sở hữu một hệ sinh thái rừng rậm nhiệt đới riêng biệt, các thác nước, sông ngầm chảy xiết và những cột thạch nhũ tự nhiên cao tới 70m. Không gian vòm hang đủ rộng để một chiếc máy bay Boeing 747 có thể di chuyển qua dễ dàng.

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051007.webp)

## ✍️ Bài đọc thêm

### Triết lý kiến trúc phần mềm: "Crash-Only Software" (Phần mềm chỉ có sập)

Một nghiên cứu khoa học công bố năm 2003 đã chỉ ra một thực tế thú vị: tốc độ khởi động lại của nhiều hệ thống phần mềm sau khi bị sập (crash) bất ngờ thường nhanh hơn so với việc thực hiện quy trình tắt hệ thống thông thường (normal exit):

* **Hệ điều hành Redhat 8**: Tắt bình thường rồi bật lại mất 104 giây; khởi động lại sau khi sập chỉ mất 75 giây.
* **Ứng dụng JBoss 3.0**: Tắt bình thường mất 47 giây; khởi động lại sau khi sập chỉ mất 39 giây.
* **Hệ điều hành Windows**: Tắt bình thường mất 61 giây; khởi động lại sau khi sập mất 48 giây.

Hơn nữa, các nhà nghiên cứu ghi nhận các hệ thống hiện đại được thiết kế các cơ chế kiểm tra tính nguyên vẹn dữ liệu rất tốt nên việc sập nguồn đột ngột hầu như không gây mất mát dữ liệu quan trọng.

Từ thực tế này, giới lập trình đưa ra một triết lý thiết kế hệ thống táo bạo mang tên **"Crash-only software" (Phần mềm chỉ có sập)**. Đối với các hệ thống này, lập trình viên hoàn toàn không viết các dòng mã xử lý quy trình tắt dịch vụ thông thường. Khi cần dừng hệ thống, ban quản trị chỉ cần ngắt nguồn hoặc kích hoạt lỗi để phần mềm tự sập. Do toàn bộ quy trình dọn dẹp bộ nhớ và khôi phục trạng thái đã được tối ưu hóa cho kịch bản phục hồi sau sự cố, hệ thống sẽ tự động khôi phục trạng thái hoạt động cực kỳ an toàn và nhanh chóng khi khởi động lại. Hệ thống tập tin phân tán nổi tiếng Google File System (GFS) của Google được ghi nhận là một trong những sản phẩm áp dụng triết lý thiết kế này.

### Câu chuyện về món thịt viên Thụy Điển của thương hiệu nội thất IKEA

IKEA được biết đến là tập đoàn bán lẻ đồ nội thất hàng đầu thế giới, nhưng ít ai biết họ cũng là nhà phân phối món thịt viên Thụy Điển lớn nhất thế giới với sản lượng tiêu thụ hơn 1 tỷ viên mỗi năm tại hệ thống nhà hàng của mình:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050909.webp)

Thời kỳ đầu thành lập, các cửa hàng của IKEA hoàn toàn không có nhà hàng ăn uống mà chỉ phục vụ cà phê và bánh ngọt nhỏ tại quầy. 

Khi quy mô các siêu thị nội thất ngày càng mở rộng như những mê cung khổng lồ, ban quản lý nhận thấy nhiều khách hàng thường có xu hướng rời khỏi siêu thị sớm do cảm thấy đói và mệt mỏi sau hàng giờ đi bộ mua sắm. Để giữ chân khách hàng lâu hơn, việc mở các nhà hàng ăn uống bên trong siêu thị trở thành yêu cầu bắt buộc.

Yêu cầu đặt ra cho thực đơn nhà hàng là phải đảm bảo tính đơn giản, dễ dàng chuẩn bị quy chuẩn hóa số lượng lớn cho hàng ngàn lượt khách mỗi ngày và phù hợp với khẩu vị của thực khách ở mọi quốc gia. Món thịt viên Thụy Điển truyền thống đã được lựa chọn vì đáp ứng tốt các tiêu chí dễ chế biến, dễ đông lạnh bảo quản và vận chuyển toàn cầu.

Nhà hàng IKEA thường được thiết kế bố trí ngay cạnh khu vực lối ra của siêu thị. Đây là một sự sắp đặt có chủ đích: IKEA không muốn khách hàng được ăn no ngay từ đầu. Họ để khách hàng có cảm giác hơi đói trong quá trình đi bộ tham quan chọn mua đồ (giúp kích thích nhu cầu mua sắm tiêu dùng) và phục vụ bữa ăn như một phần thưởng dừng chân hoàn hảo sau khi họ hoàn thành thanh toán giỏ hàng. Các nghiên cứu hành vi chỉ ra những khách hàng mua sắm trong trạng thái đói bụng thường chi tiêu nhiều hơn tới 64% so với những khách hàng đã ăn no.

## 历史上的本周

- 2021年（第 176 期）：[Pháp lý mã nguồn mở: Tòa án Trung Quốc đưa ra các phán quyết công nhận hiệu lực pháp lý của giấy phép GPL như thế nào](https://www.ruanyifeng.com/blog/2021/09/weekly-issue-176.html)
- 2020年（第 125 期）：[Tài chính số: Nhìn nhận mục tiêu và các đối tượng tác động chính của đồng Nhân dân tệ số (e-CNY)](https://www.ruanyifeng.com/blog/2020/09/weekly-issue-125.html)
- 2019年（第 74 期）：[Kinh doanh nội dung: Tại sao mô hình kinh doanh thông tin hiệu quả trên Internet thường là miễn phí quảng cáo thay vì thu phí đọc](https://www.ruanyifeng.com/blog/2019/09/weekly-issue-74.html)
- 2018年（第 23 期）：[Thống kê học: Phân tích các yếu tố quyết định lớn nhất tới sự thành công trong cuộc đời của một con người](https://www.ruanyifeng.com/blog/2018/09/weekly-issue-23.html)

## 鸣谢

Nền tảng quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072108.webp)

（Hết）
