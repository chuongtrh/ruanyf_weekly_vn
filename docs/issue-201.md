# 科技爱好者周刊（第 201 期）：中国需要成立半导体部

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2309) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033001.webp)

Tại Thượng Hải, các lực lượng phòng chống dịch đã sử dụng robot bốn chân (robot dog) đi dọc các con phố không một bóng người để phát loa tuyên truyền chính sách phòng dịch, tạo nên một khung cảnh viễn tưởng ấn tượng. (Nguồn: [Xinmin](http://news.xinmin.cn/2022/03/29/32137444.html))

## 主带话题：Trung Quốc cần thành lập Bộ Bán dẫn

Tháng trước, Cục Thống kê Quốc gia đã công bố [《中国2021年统计公报》](http://www.stats.gov.cn/tjsj/zxfb/202202/t20220227_1827960.html) (Báo cáo Thống kê Quốc gia năm 2021).

Báo cáo ghi nhận: ba mặt hàng Trung Quốc nhập khẩu nhiều nhất lần lượt là vi mạch tích hợp (chip bán dẫn), dầu mỏ và quặng sắt.

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032502.webp)

Vi mạch tích hợp chiếm tới 16% tổng kim ngạch nhập khẩu của cả nước, xấp xỉ bằng tổng giá trị của dầu mỏ và quặng sắt cộng lại. Điều này cho thấy **nền kinh tế trong nước đang phụ thuộc vào nguồn chip bán dẫn nhập khẩu còn lớn hơn cả dầu mỏ.** Cần biết rằng Trung Quốc là quốc gia nhập khẩu dầu mỏ lớn nhất thế giới, qua đó có thể hình dung quy mô nhập khẩu chip bán dẫn khổng lồ đến nhường nào.

Nguyên nhân cốt lõi dẫn tới việc nhập khẩu lượng chip khổng lồ này rất đơn giản: chúng ta chưa thể tự chủ sản xuất các dòng vi mạch máy tính cao cấp trong nước.

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032813.webp)

Hiện nay, công nghệ sản xuất bán dẫn tiên tiến nhất thế giới đã đạt tới tiến trình 5nm của TSMC (đã đi vào sản xuất đại trà), và dự kiến tiến trình 3nm sẽ bắt đầu chạy thử trong năm nay, hướng tới mục tiêu 1nm trong vài năm tới. Để so sánh, tiến trình sản xuất tốt nhất trong nước mới đạt tới mức 14nm của SMIC với sản lượng còn hạn chế, đồng thời các thiết bị máy quang khắc lõi vẫn phải phụ thuộc vào công nghệ nước ngoài. Hầu như toàn bộ chip xử lý CPU cho máy tính cá nhân và điện thoại thông minh trong nước hiện nay đều phải nhập khẩu.

Mục tiêu trước mắt của chính phủ là nhanh chóng tự chủ hoàn toàn quy trình sản xuất tiến trình 28nm, sau đó là 14nm nhưng thời gian hoàn thành cụ thể vẫn chưa chắc chắn.

Mục tiêu cốt lõi trong các lệnh cấm vận công nghệ của Mỹ là ngăn chặn Trung Quốc tiếp cận và tự chủ chuỗi công nghệ bán dẫn để sản xuất chip cao cấp. Sự cố trừng phạt ZTE năm 2018 (buộc doanh nghiệp này phải nộp phạt 14,7 tỷ NDT để duy trì hoạt động) và lệnh cấm vận Huawei năm 2020 (khiến mảng smartphone của hãng sụt giảm mạnh và doanh thu toàn tập đoàn sụt giảm 28,9% vào năm 2021 - lần đầu tiên sụt giảm doanh thu sau 20 năm) là minh chứng rõ nhất cho mức độ ảnh hưởng của cấm vận công nghệ chip đối với các doanh nghiệp lớn.

 chip bán dẫn là trái tim cốt lõi của các thiết bị điện tử. Xu hướng hiện nay là các hãng công nghệ lớn đều tự thiết kế chip riêng. Việc Apple phát triển dòng chip M1 từ năm 2020 đã giúp dòng máy Mac lột xác hoàn toàn nâng cao vị thế cạnh tranh vượt trội:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032503.webp)

*(Hình ảnh chip M1 Ultra khổng lồ của Apple bên phải so sánh với chip x86 CPU thông thường bên trái)*

Trước bối cảnh đó, tôi có một ý tưởng: **Trung Quốc nên thành lập một Bộ Bán dẫn chuyên biệt.** Bộ này sẽ tập hợp các phòng ban quản lý bán dẫn đang phân tán tại Bộ Công nghiệp và Công nghệ thông tin, Bộ Khoa học và Công nghệ, Ủy ban Phát triển và Cải cách Quốc gia để quy về một mối, tập trung nguồn lực quốc gia đột phá công nghệ và phá vỡ thế bao vây của Mỹ.

Ngành bán dẫn có chuỗi cung ứng cực kỳ rộng từ vật liệu hóa chất, thiết bị quang khắc đến phần mềm thiết kế cần sự điều phối tầm quốc gia của chính phủ. Trong lịch sử, Trung Quốc từng có Bộ Than, Bộ Dầu mỏ, Bộ Công nghiệp Điện tử, và hiện tại hoàn toàn là thời điểm thích hợp để thành lập một Bộ Bán dẫn.

## Authing 永久免费版

Năm ngoái, bản tin đã giới thiệu tới các bạn nền tảng quản lý định danh SaaS trong nước mang tên **[Authing](https://www.authing.cn/)**. Mới đây, họ đã chính thức ra mắt gói dịch vụ vĩnh viễn miễn phí nhằm hỗ trợ các nhà phát triển và doanh nghiệp vừa và nhỏ.

Authing cung cấp giải pháp quản lý tài khoản và định danh người dùng (IDaaS) toàn diện, tích hợp các tính năng xác thực, phân quyền và bảo mật tài khoản cho cả ứng dụng Web, mobile hay Desktop với hơn 1.000 API mở:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030601.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033127.webp)

Ví dụ như tính năng tích hợp đăng nhập nhanh qua quét mã QR WeChat (hình trên) có thể dễ dàng thiết lập thông qua 3 bước đơn giản hầu như không cần viết code:
1. Đăng ký ứng dụng trên WeChat Open Platform.
2. Điền thông tin App ID và App Secret vào trang quản trị Authing.
3. Trỏ đường dẫn đăng nhập về trang đăng nhập do Authing host sẵn.

Người dùng quan tâm có thể tham khảo [Tài liệu hướng dẫn](https://docs.authing.cn/v2/guides/wechat-ecosystem/wechat-pc/) và [Kho code mẫu GitHub](https://github.com/Authing/wechat-eco-solution). Các phương thức đăng nhập qua tài khoản mạng xã hội khác (Weibo, DingTalk, Feishu, QQ) cũng được tích hợp tương tự.

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033004.webp)

Authing cũng hỗ trợ giải pháp đăng nhập một lần (Single Sign-On - SSO) liên kết tài khoản nội bộ với hơn 120 công cụ làm việc thông dụng hiện nay như AWS, GitLab, Jira, Notion, Teambition, Feishu:

Chính sách gói vĩnh viễn miễn phí của Authing được chia làm 3 nhóm:
- **Gói B2C:** Hỗ trợ tối đa 8.000 người dùng hoạt động hàng tháng (MAU).
- **Gói B2B:** Hỗ trợ tối đa 200 người dùng hoạt động hàng tháng.
- **Gói B2E (quản lý nhân sự nội bộ):** Hỗ trợ tối đa 10 nhân viên.

Quy mô 8.000 MAU hoàn toàn đủ dùng cho các ứng dụng vừa và nhỏ của cá nhân do hệ thống chỉ tính phí dựa trên số lượng tài khoản đăng nhập thực tế trong tháng. Các bạn có thể đăng ký tài khoản trải nghiệm miễn phí trên [Trang chủ Authing](https://www.authing.cn/) và tham khảo ý kiến tại [Diễn đàn Authing](https://forum.authing.cn/).

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033002.webp)

Vào ngày 15/5 tới tại Bắc Kinh, Authing sẽ tổ chức Hội nghị các nhà phát triển thường niên **Authing Connect** chia sẻ các chủ đề Cloud Native, Serverless và No-code. Bạn đọc quan tâm có thể quét mã QR trên đây để đăng ký tham gia.

## 科技动态

1、[Hội thi xếp đá nghệ thuật thường niên tại bờ biển Scotland](https://hakaimagazine.com/article-short/stones-as-medium-beach-as-canvas/)

Ý tưởng tổ chức cuộc thi xếp đá thăng bằng nghệ thuật được một nghệ sĩ Anh khởi xướng từ năm 2015, thu hút hàng chục nghệ sĩ quốc tế tham dự hàng năm tại bãi biển Scotland:

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020106.webp)

*(Tác phẩm đoạt giải quán quân năm 2019)*

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020107.webp)

Cuộc thi diễn ra trong vòng nửa ngày khi thủy triều rút xuống. Các nghệ sĩ phải tranh thủ tìm kiếm các khối đá tự nhiên trên bãi biển để tạo dựng tác phẩm thăng bằng nghệ thuật trước khi thủy triều dâng lên cuốn trôi mọi thứ:

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020108.webp)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020109.webp)

2、[Apple Maps và Google Maps thiết lập bức tường kỹ thuật số che mờ nhà CEO Tim Cook](https://www.cultofmac.com/764740/apple-maps-hides-tim-cook-house/)

Hình ảnh ngôi biệt thự riêng của CEO Apple Tim Cook tại California mới đây đã được che mờ hoàn toàn trên các dịch vụ bản đồ đường phố của Apple và Google:

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020111.webp)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020112.webp)

Quyết định được đưa ra sau khi tòa án ban hành lệnh cấm đối với một đối tượng có hành vi theo dõi và đe dọa đột nhập vào nhà riêng của ông. Thực tế, bất kỳ người dùng cá nhân nào cũng có thể gửi đơn yêu cầu Apple và Google che mờ hình ảnh ngôi nhà của mình trên bản đồ để bảo vệ quyền riêng tư.

3、[Nhật Bản thử nghiệm máy tính tiền toàn ảnh không tiếp xúc tại cửa hàng tiện lợi](https://japantoday.com/category/tech/floating-hologram-registers-coming-to-japanese-convenience-stores-1)

Chuỗi cửa hàng tiện lợi 7-Eleven tại Nhật Bản đang chạy thử nghiệm hệ thống máy tính tiền tự động không tiếp xúc ứng dụng công nghệ trình chiếu hình ảnh lơ lửng trong không khí:

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020306.webp)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020307.webp)

Hệ thống sử dụng gương phản chiếu đặc biệt để trình chiếu giao diện thanh toán lơ lửng trước mặt khách hàng (chỉ người đứng trực diện mới quan sát thấy màn hình). Khách hàng thực hiện thao tác chạm ngón tay vào khoảng không để chọn phương thức thanh toán mà không cần chạm trực tiếp vào màn hình cơ học, giúp tăng tính vệ sinh phòng dịch:

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020308.webp)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020309.webp)

4、[Tuần lễ thời trang Metaverse đầu tiên được tổ chức](https://mashable.com/article/metaverse-fashion-week)

Nền tảng thực tế ảo Decentraland đã tổ chức sự kiện tuần lễ thời trang ảo thường niên từ ngày 24 đến 27 tháng 3 với sự tham gia của nhiều thương hiệu danh tiếng như Dolce & Gabbana, Estée Lauder, Forever 21:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033109.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033110.webp)

Các thương hiệu lớn đã thiết lập các cửa hàng flagship ảo để người dùng điều khiển nhân vật vào tham quan mua sắm các trang phục ảo dưới dạng NFT hoặc mua các sản phẩm thời trang thật ngoài đời:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033111.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033112.webp)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033113.webp)

5、[Nghiên cứu khoa học về sự tập trung của người dùng trong các cuộc họp trực tuyến](https://www.news.iastate.edu/news/2022/02/07/zoom-eye-tracking)

Một nhóm nghiên cứu tại Mỹ đã sử dụng camera theo dõi cử động mắt (eye-tracking) của các thành viên tham gia họp trực tuyến qua Zoom để đánh giá mức độ tập trung:

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021002.webp)

Kết quả cho thấy trong các cuộc họp quy mô nhỏ, người dùng dành tới 1/3 thời gian để nhìn ra ngoài màn hình máy tính (mỗi lần nhìn lệch khoảng vài giây trước khi quay lại màn hình). Trong các cuộc họp lớn, tỷ lệ này thấp hơn do người dùng có tâm lý sợ bị phát hiện lơ là. Nghiên cứu cũng chỉ ra người dùng nữ dành nhiều thời gian để quan sát hình ảnh chân dung của chính mình trên màn hình họp hơn so với nam giới.

## 文章

1、[Hiện trạng và triển vọng của công nghệ cấy ghép tim lợn trên cơ thể người tại Trung Quốc](https://mp.weixin.qq.com/s/VGi50iOMHH0CermRv8rW2g)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032401.webp)

Sau sự kiện Mỹ thực hiện thành công ca phẫu thuật ghép tim lợn biến đổi gen đầu tiên trên thế giới cho bệnh nhân duy trì sự sống trong 2 tháng, bài viết phân tích các rào cản kỹ thuật chỉnh sửa gen và triển vọng ứng dụng lâm sàng của công nghệ này trong nước.

2、[Người dùng Nhật Bản chia sẻ hành trình gỡ bỏ trình duyệt 360 Safe Browser](https://mp.weixin.qq.com/s/Hdgcp-I0SrZioXnv3mA6-Q)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032402.webp)

Bài đăng hài hước ghi lại hành trình của một blogger công nghệ Nhật Bản tìm cách gỡ bỏ tận gốc trình duyệt 360 Safe Browser vô tình cài đặt trên máy tính Windows sau khi gặp các thông báo nhắc nhở tiếng Trung khó hiểu.

3、[Cảnh báo nguy cơ đổ sập của tháp gỗ cổ nhất thế giới tại Ứng Huyện](https://mp.weixin.qq.com/s/wd2gvWpfg85RZAzNEQTa2Q)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031009.webp)

Tháp gỗ Ứng Huyện tại tỉnh Sơn Tây xây dựng từ thời nhà Liêu là tháp gỗ cổ nhất và cao nhất thế giới còn tồn tại. Tuy nhiên, các kỹ sư cảnh báo hệ thống cột đỡ bằng gỗ tại tầng 2 của tháp hiện đang bị nghiêng lệch nghiêm trọng đứng trước nguy cơ đổ sập nếu không được gia cố kỹ thuật kịp thời:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031010.webp)

4、[Giải thích hiện tượng vật lý học hình thành cột gai băng trong khay đá tủ lạnh](http://www.its.caltech.edu/~atomic/snowcrystals/icespikes/icespikes.htm)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020801.webp)

Bài phân tích hiện tượng khoa học thú vị giải thích lý do tại sao đôi khi các khay nước đông đá trong tủ lạnh lại hình thành những cột gai băng nhọn trồi thẳng lên trên mặt nước khi đông đặc.

5、[Hướng dẫn sử dụng thuộc tính tỷ lệ khung hình aspect-ratio trong CSS](https://css-irl.info/aspect-ratio-is-great/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021007.webp)

Bài viết hướng dẫn cách ứng dụng thuộc tính `aspect-ratio` mới của CSS giúp lập trình viên dễ dàng cố định tỷ lệ hiển thị dài/rộng của các khung ảnh hoặc video khi thiết kế web responsive.

6、[Tổng hợp 10 kiểu layout trang web thông dụng chỉ bằng 1 dòng code CSS](https://1linelayouts.glitch.me/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112410.jpg)

Trang web chia sẻ 10 dòng code CSS Grid và Flexbox thông minh hỗ trợ dựng nhanh các bộ khung căn chỉnh bố cục web phổ biến.

7、[Mẹo lập trình tự động trích xuất nội dung sách điện tử trên điện thoại Android](https://shkspr.mobi/blog/2021/12/quick-and-dirty-way-to-rip-an-ebook-from-android/)（Tiếng Anh）

Tác giả chia sẻ kịch bản script tự động ra lệnh vuốt chuyển trang và chụp ảnh màn hình điện thoại Android kết nối máy tính qua ADB để thu thập dữ liệu ảnh trang sách, sau đó dùng công cụ OCR để trích xuất văn bản sách điện tử bị khóa DRM.

8、[Hoạt họa trực quan giải thích nguyên lý toán học chuỗi Markov](https://setosa.io/blog/2014/07/26/markov-chains/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020710.webp)

Bài viết ứng dụng các sơ đồ hoạt họa tương tác trực quan giúp người học dễ dàng nắm bắt các khái niệm lý thuyết xác suất chuỗi chuyển trạng thái Markov.

## 工具

1、[PeaZip: Trình nén và giải nén tệp tin nguồn mở đa năng](https://peazip.github.io/)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022022602.webp)

Phần mềm nén file có giao diện đồ họa trực quan hỗ trợ xử lý hầu hết định dạng file nén hiện nay và bổ sung hỗ trợ hai định dạng nén hiệu năng cao Zstandard, Brotli.

2、[Speech To Code: Lập trình mã nguồn bằng giọng nói](https://github.com/pedrooaugusto/speech-to-code)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033119.webp)

Dự án thử nghiệm nhận diện khẩu lệnh tiếng Anh để tự động sinh các đoạn mã nguồn HTML/JS tương ứng. Người dùng có thể chạy thử tại [Bản Demo trực tuyến](https://pedrooaugusto.github.io/speech-to-code/webapp/). (Đóng góp của [@ooohmydawn](https://github.com/ruanyf/weekly/issues/2288))

3、[HertzBeat (赫兹跳动): Hệ thống giám sát tài nguyên đám mây nguồn mở](https://hertzbeat.com/)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033120.webp)

Hệ thống giám sát hiệu năng website, kiểm tra ping kết nối, trạng thái cổng mạng, bộ nhớ RAM hệ điều hành và gửi thông báo cảnh báo tức thì qua email, WeChat, DingTalk. (Đóng góp của [@tomsun28](https://github.com/ruanyf/weekly/issues/2298))

4、[stop-mess-around: Extension quản lý thời gian lướt web chống摸 cá](https://github.com/OBKoro1/stop-mess-around)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033122.webp)

Tiện ích mở rộng trình duyệt hỗ trợ người dùng thiết lập danh sách các trang web giải trí tiêu tốn thời gian. Hệ thống sẽ tự động tính giờ truy cập và hiển thị cảnh báo nhắc nhở khi người dùng lướt web quá lâu. (Đóng góp của [@OBKoro1](https://github.com/ruanyf/weekly/issues/2302))

5、[Video PPT Extractor: Công cụ tự động trích xuất slide bài giảng từ video](https://github.com/wudududu/extract-video-ppt)

Công cụ hữu ích hỗ trợ quét khung hình video bài giảng để phát hiện sự thay đổi nội dung trang trình chiếu, tự động chụp lại các trang slide và xuất ra file PDF học tập tiện lợi. (Đóng góp của [@wudududu](https://github.com/ruanyf/weekly/issues/2303))

6、[sqlite-utils: Tiện ích dòng lệnh tương tác dữ liệu SQLite nhanh](https://github.com/simonw/sqlite-utils)

Công cụ hỗ trợ lập trình viên chạy nhanh các truy vấn SQL, thêm/sửa cấu trúc bảng và nhập dữ liệu JSON/CSV trực tiếp vào file SQLite thông qua terminal.

7、[Simple.css: Thư viện CSS tối giản tự động định dạng thẻ HTML](https://github.com/kevquirk/simple.css)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011703.webp)

Bộ khung CSS tối giản thiết kế theo triết lý classless: không cần gán class cho thẻ, thư viện sẽ tự động định dạng hiển thị đẹp mắt cho các thẻ tiêu chuẩn mặc định của HTML. Người dùng có thể tham khảo thêm các thư viện tương tự như [Pico.css](https://picocss.com/), [MVP.css](https://andybrewer.github.io/mvp/), [Water.css](https://github.com/kognise/water.css).

8、[Sci Hub Injector: Tự động nhúng link tải báo Sci-Hub trên các tạp chí khoa học](https://github.com/rickwierenga/sci-hub-injector)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011704.webp)

Extension trình duyệt hỗ trợ tự động phát hiện mã DOI của bài báo trên các trang tạp chí lớn (Nature, PubMed) để nhúng trực tiếp nút tải bài báo miễn phí qua Sci-Hub.

9、[fq: Công cụ dòng lệnh phân tích cấu trúc file nhị phân](https://github.com/wader/fq)

Tiện ích dòng lệnh hỗ trợ lập trình viên kiểm tra cấu trúc trường dữ liệu, byte nhị phân của các file ảnh, video hoặc file thực thi.

10、[Lemmy: Hệ thống diễn đàn liên hợp phi tập trung](https://github.com/LemmyNet/lemmy)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012201.webp)

Mã nguồn mạng xã hội diễn đàn phi tập trung viết bằng Rust tương thích giao thức ActivityPub, hỗ trợ đồng bộ hiển thị bài đăng chéo giữa các máy chủ độc lập trong mạng lưới Fediverse.

## 资源

1、[Disney Animation Process: Khám phá quy trình dựng phim hoạt hình của Disney](https://disneyanimation.com/process/)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021001.webp)

Chuyên trang tương tác chính thức giới thiệu quy trình 10 bước hậu kỳ thiết kế nhân vật, dựng xương đồ họa và render ánh sáng phim hoạt hình 3D của hãng Disney.

2、[PHP The Right Way (Cẩm nang lập trình PHP chuẩn hóa hiện đại)](https://learnku.com/docs/php-the-right-way/PHP8.0)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020707.webp)

Bộ giáo trình tự học lập trình PHP hướng dẫn viết code chuẩn mực, tối ưu hóa bảo mật và cấu hình máy chủ web chạy PHP (bản dịch tiếng Trung - Xem thêm [bản gốc tiếng Anh](https://phptherightway.com/)).

3、[Canteen Weekly: Bản tin công nghệ lập trình Front-end tiếng Trung](https://github.com/Geekhyt/weekly)

Bản tin tổng hợp các bài viết phân tích kỹ thuật và chia sẻ kinh nghiệm phát triển Web Front-end hàng tuần. (Đóng góp của [@Geekhyt](https://github.com/ruanyf/weekly/issues/2290))

4、[LearnGolang: Thư mục tổng hợp tài liệu tự học ngôn ngữ Go của lập trình viên](https://github.com/LearnGolang/LearnGolang)

Kho lưu trữ chia sẻ lộ trình tự học từ cơ bản đến nâng cao, các bài tập code mẫu và câu hỏi phỏng vấn Go phổ biến. (Đóng góp của [@0e0w](https://github.com/ruanyf/weekly/issues/2293))

5、[study-is-wonderful: Thư mục tổng hợp các khóa học trực tuyến hữu ích](https://github.com/xioacd99/study-is-wonderful)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033121.webp)

Thư mục chia sẻ các liên kết bài giảng, khóa học đại cương đại học chất lượng cao bằng tiếng Trung. (Đóng góp của [@xioacd99](https://github.com/ruanyf/weekly/issues/2300))

## 图片

1\. [Tranh cãi thú vị về phương pháp nướng Pizza của Elon Musk](https://twitter.com/elonmusk/status/1505100708256825347)

Elon Musk đăng ảnh trên Twitter đùa rằng việc nướng pizza hình tròn trong khay nướng chữ nhật là lãng phí không gian lò và đề xuất cách cắt ghép để nướng tối ưu:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032009.webp)

Một cư dân mạng lập tức phản hồi bằng hình ảnh cách sắp xếp 4 góc pizza cắt ghép mang lại tỷ lệ tận dụng diện tích khay nướng cao hơn nhiều:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032010.webp)

2、[Beverly Clock: Chiếc đồng hồ cơ khí hoạt động hơn 150 năm không cần lên dây](https://en.wikipedia.org/wiki/Beverly_Clock)

Đặt tại hành lang Khoa Vật lý Đại học Otago, New Zealand là chiếc đồng hồ cơ khí cổ kính do nghệ nhân chế tạo vào năm 1864:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122703.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122704.webp)

Đồng hồ vận hành bền bỉ hơn 1,5 thế kỷ qua mà chưa từng cần tới sự can thiệp lên dây cót thủ công của con người. Bí quyết nằm ở bầu không khí 28 lít đặt trong hộp kính kín bên trong: chỉ cần nhiệt độ môi trường chênh lệch 3.3°C trong ngày, lượng khí co giãn sẽ tạo lực kéo quả nặng dịch chuyển 1 inch để nạp lại thế năng dây cót cho đồng hồ:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122705.webp)

## Bài đọc thêm

### Quy trình phát triển phần mềm nên tương tự như một chiếc bánh ngọt

Chúng ta có thể rút ra nhiều nguyên lý thiết kế phần mềm từ quá trình làm một chiếc bánh ngọt:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033123.webp)

1. **Giới hạn thời gian hoàn thành rõ ràng:** Làm bánh ngọt luôn có mốc thời gian hoàn thành cụ thể. Nếu bạn dự tính làm trong 3 tiếng nhưng kéo dài tới 1 tuần, nguyên liệu bên trong chắc chắn sẽ bị hỏng. Dự án phần mềm cũng vậy, nếu thời gian thực hiện bị kéo dài quá lâu so với ước lượng ban đầu, cấu trúc hệ thống rất dễ phát sinh lỗi nghiêm trọng.
2. **Kích thước dự án nhỏ gọn:** Bánh ngọt có kích thước nhỏ giúp người thợ dễ dàng thử nghiệm điều chỉnh công thức. Quy mô dự án phần mềm nhỏ hỗ trợ đội ngũ nhanh chóng lặp (iterative) để tìm ra giải pháp tối ưu nhất.
3. **Phải có người thưởng thức trực tiếp:** Một chiếc bánh làm ra cần có người ăn thử để cho nhận xét khách quan về hương vị. Phần mềm cũng bắt buộc phải có người dùng trải nghiệm thực tế để thu thập phản hồi cải tiến tính năng, tránh làm ra sản phẩm không ai cần tới.
4. **Quá trình thực hiện mang lại niềm vui:** Việc làm bánh cần đem lại sự thú vị cho người thợ. Việc viết code cũng nên giúp lập trình viên cảm thấy hứng thú sáng tạo khi nhìn thấy sản phẩm dần hình thành.

### Tại sao tôi duy trì phát hành công cụ PuTTY hoàn toàn miễn phí?

Nhiều ý kiến cho rằng các nhà phát triển nên thu phí giấy phép phần mềm nguồn mở đối với các tập đoàn lớn để có kinh phí duy trì dự án lâu dài. Tác giả của công cụ SSH Client huyền thoại **PuTTY** trên Windows đã chia sẻ góc nhìn của mình:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033124.webp)

Ông hoàn toàn vui vẻ khi các doanh nghiệp lớn sử dụng miễn phí phần mềm của mình và không hề cảm thấy công sức bị bóc lột.

Nguyên nhân do PuTTY là phần mềm liên quan tới bảo mật hạ tầng mạng. An ninh của thế giới mạng có tính liên kết chặt chẽ: nếu càng nhiều máy chủ trên Internet có lỗ hổng bảo mật do không trang bị công cụ mã hóa kết nối tốt, nguy cơ các cuộc tấn công phát tán mã độc lây lan sang các trang web cá nhân quan trọng của chính ông sẽ càng cao.

Việc phát hành miễn phí PuTTY giúp mọi quản trị viên hệ thống đều dễ dàng trang bị kết nối bảo mật SSH chất lượng cao. Khi toàn bộ mạng Internet trở nên an toàn và tin cậy hơn, chính bản thân tác giả cũng sẽ được hưởng lợi gián tiếp từ môi trường mạng sạch đó. Nếu ông thu phí phần mềm, rào cản chi phí có thể khiến nhiều công ty hạn chế đầu tư bảo mật, làm tăng nguy cơ mất an toàn chung của toàn hệ thống mạng.

## 言论

1\.

Trong cộng đồng phần mềm tự do luôn tồn tại một tâm lý hoài nghi sâu sắc: không tin cậy các tập đoàn công nghệ lớn, không tin cậy các cơ quan chính phủ và bài trừ phần mềm độc quyền. Nguồn gốc của sự hoài nghi này đến từ việc họ phản đối cấu trúc quản lý tập trung và luôn ưu tiên lựa chọn các thiết kế hệ thống phi tập trung (decentralized).

-- Trích bài viết "The federation fallacy"

2\.

Môi trường phát triển Web hiện nay đã thay đổi bản chất: chúng ta không còn xây dựng nội dung trang web để chia sẻ liên kết bền vững hay lưu trữ lâu dài như trước, mà chủ yếu tạo ra nội dung phục vụ hiển thị quảng cáo kiếm tiền. Thời gian đọc nội dung của người dùng đã sụt giảm từ vài phút xuống còn vài giây, và các thuật toán gây nghiện của Facebook, Instagram hay TikTok đang định hình bộ mặt mới của Internet.

-- Trích bài viết "The Web starts on page four"

## 历史上的本周

- 2021年（第 150 期）：[Thảo luận văn hóa xã hội: Nhìn lại thời kỳ âm nhạc còn là tài nguyên khan hiếm](https://www.ruanyifeng.com/blog/2021/03/weekly-issue-150.html)
- 2020年（第 98 期）：[Chia sẻ các kỹ năng giúp lập trình viên trình bày quan điểm kỹ thuật rõ ràng và thuyết phục](https://www.ruanyifeng.com/blog/2020/03/weekly-issue-98.html)
- 2019年（第 47 期）：[Thảo luận thực tế: Hoạt động livestream mukbang (ăn uống) có được coi là một công việc chính thức?](https://www.ruanyifeng.com/blog/2019/03/weekly-issue-47.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
