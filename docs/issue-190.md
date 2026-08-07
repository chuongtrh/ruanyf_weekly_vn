# 科技爱好者周刊（第 190 期）：产品化思维

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2139) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122913.webp)

Trong suốt năm 2021, chỉ có duy nhất một lần nhật thực toàn phần diễn ra vào ngày 4/12 tại khu vực Nam Cực. Khoảnh khắc này đã được vệ tinh của NASA chụp lại từ không gian: vùng bóng tối bao trùm hoàn toàn Nam Cực khi Mặt Trăng nằm thẳng hàng giữa Trái Đất và Mặt Trời. Hiện tượng thiên văn kỳ thú này kéo dài trong vòng 2 phút. (Nguồn: [NASA Earth Observatory](https://earthobservatory.nasa.gov/images/149174/antarctica-eclipsed))

## 主带话题：Tư duy sản phẩm hóa

Tuần trước, Huawei vừa cho ra mắt một mẫu đồng hồ đo huyết áp mang tên **Watch D** có khả năng đo huyết áp trực tiếp trên cổ tay người dùng.

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122506.webp)

Thiết kế của sản phẩm này khá độc đáo, có thể là chiếc đồng hồ thông minh đầu tiên áp dụng thiết kế này.

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122508.webp)

Như hình ảnh trên, phía bên dưới dây đeo được trang bị một lớp đệm dạng túi khí siêu nhỏ.

Khi đo huyết áp, đồng hồ sẽ bơm khí làm túi căng lên ép chặt vào cổ tay (hình dưới) để đo nhịp tim và huyết áp dựa trên dao động mạch.

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122509.webp)

Thiết kế này trông rất quen thuộc, thực chất nó hoạt động tương tự như một chiếc máy đo huyết áp cổ tay truyền thống thường thấy trong các gia đình:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122510.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122804.webp)

Sản phẩm đồng hồ của Huawei thực chất chính là một phiên bản thu nhỏ của máy đo huyết áp cổ tay. Tuy nhiên, sự khác biệt lớn nằm ở giá cả: chiếc smartwatch của Huawei có giá chính thức là 2.988 NDT (khoảng 10,7 triệu VND), trong khi một chiếc máy đo huyết áp cổ tay thông dụng chỉ có giá hơn 100 NDT (khoảng 350.000 VND).

Tất nhiên, đồng hồ thông minh có nhiều chức năng nâng cao khác, nhưng điểm bán hàng chính của nó là đo huyết áp. Ở khía cạnh này, nó không quá vượt trội so với máy đo huyết áp cổ tay thông thường. Nhưng bạn chỉ cần bỏ ra 5% số tiền là đã có được một thiết bị có độ tiện lợi tương đương và kết quả đo đạc thực tế có khi còn chính xác hơn.

Điều này gợi lên một câu hỏi: **Tại sao các nhà sản xuất máy đo huyết áp truyền thống trước đây chưa từng nghĩ tới việc biến sản phẩm của họ thành một chiếc đồng hồ đeo tay thời thượng?**

Sở dĩ họ không nghĩ tới là do thiếu **"Tư duy sản phẩm hóa"** (Productization thinking) - tức là khả năng đóng gói một tính năng cơ bản thành một sản phẩm thương mại hấp dẫn và giới thiệu ra thị trường. Nếu các hãng máy đo huyết áp có tư duy này, họ đã có thể thâm nhập vào thị trường thiết bị đeo. Ngược lại, Huawei đã nhìn thấy cơ hội từ chiếc máy đo huyết áp truyền thống: bằng cách tích hợp túi khí mini vào dây đeo, chiếc smartwatch thông thường đã biến thành một thiết bị y tế cao cấp bán được giá cao hơn rất nhiều.

Một ví dụ tương tự là máy lọc không khí. Nguyên lý cốt lõi của nó cực kỳ đơn giản: chỉ là một chiếc quạt kết hợp với màng lọc HEPA để giữ bụi mịn. Người đầu tiên nghĩ ra việc đóng gói cụm quạt lọc này thành một thiết bị trang nhã mang tên "máy lọc không khí" rõ ràng là người có tư duy sản phẩm hóa xuất sắc, bởi vì giá của máy lọc không khí đắt hơn quạt thường rất nhiều.

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122511.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122512.webp)

Các kỹ sư và lập trình viên thường tập trung giải quyết các bài toán kỹ thuật mà bỏ quên tư duy sản phẩm hóa này. Điều này hạn chế khả năng phát triển sự nghiệp kinh doanh riêng. Bởi vì chỉ có tạo ra sản phẩm hoàn chỉnh mới có thể mang đi bán, và bán tốt sản phẩm của chính mình mới giúp chúng ta tự làm chủ cuộc đời thay vì đi làm thuê suốt đời.

Hàng chục năm trước, kỹ sư Steve Wozniak của HP đã tự thiết kế một bảng mạch máy tính cực kỳ mạnh mẽ để tự chơi trong thời gian rảnh. Cho đến khi Steve Jobs nhìn thấy và kiên quyết thuyết phục Wozniak lắp thêm vỏ hộp, bàn phím để biến nó thành một chiếc máy tính hoàn chỉnh mang đi bán. Đó là sự ra đời của Apple I và tập đoàn Apple danh tiếng. Chúng ta cần học hỏi tư duy sản phẩm hóa đó của Steve Jobs: biến bảng mạch thô thành máy tính cá nhân, và biến máy đo huyết áp thô thành đồng hồ đeo tay thời thượng.

## 飞连

Gần đây, bài viết **[《ByteDance không cần tòa nhà trụ sở》](https://mp.weixin.qq.com/s/nPChaKQcotEzttnSysom5w)** gây xôn xao dư luận. Với quy mô hơn 11 vạn nhân viên làm việc từ xa tại 150 quốc gia, làm thế nào ByteDance quản lý được hiệu suất và đặc biệt là vấn đề an toàn thông tin mạng nội bộ khi làm việc từ xa?

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122906.webp)

*(Chỉ tính riêng tại Bắc Kinh, ByteDance đã có gần 20 địa điểm văn phòng khác nhau)*

Bên cạnh ứng dụng văn phòng Lark (飛書), ByteDance dựa vào một công cụ bảo mật nội bộ cốt lõi mang tên **[Feilian (飞连)](https://www.volcengine.com/products/feilian/?utm_source=outsidemedia&utm_medium=ruanyifeng&utm_term=wx_readmore&utm_campaign=20211231&utm_content=feilian)**:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021123009.webp)

Được phát triển và kiểm chứng thực tế trong nội bộ ByteDance, Feilian là cổng kết nối an toàn tích hợp các tính năng:
- **Quản lý danh tính tập trung:** Đồng bộ hóa dữ liệu nhân sự trên toàn hệ thống, tự động phân quyền truy cập theo vai trò.
- **Quản lý truy cập mạng và VPN:** Kiểm soát kết nối Wi-Fi, mạng có dây và kết nối VPN an toàn cho cả máy tính công ty, thiết bị cá nhân (BYOD), máy in và camera.
- **Bảo mật thiết bị đầu cuối:** Quét mã độc, phòng chống rò rỉ dữ liệu (DLP) và chẩn đoán lỗi mạng tự động giúp giảm tải cho bộ phận IT.

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021123011.webp)

Hiện tại, giải pháp bảo mật cao cấp này đã được thương mại hóa qua nền tảng đám mây **Volcengine** của hãng. Doanh nghiệp có nhu cầu trải nghiệm có thể truy cập [trang chủ Volcengine](https://www.volcengine.com/products/feilian/?utm_source=outsidemedia&utm_medium=ruanyifeng&utm_term=wx_readmore&utm_campaign=20211231&utm_content=feilian) hoặc quét mã QR dưới đây để đăng ký dùng thử:

<a href="https://cdn.beekka.com/blogimg/asset/202112/bg2021123016.webp" target="_blank"><img src="https://cdn.beekka.com/blogimg/asset/202112/bg2021123016.webp" width="800"></a>

## 科技动态

1、[NASA thử nghiệm trồng ớt chuông thành công trên Trạm vũ trụ quốc tế](https://edition.cnn.com/2021/12/01/world/nasa-space-chile-harvest-scn/index.html)

Tháng 7 vừa qua, các phi hành gia trên trạm vũ trụ ISS đã gieo những hạt giống ớt chuông trong môi trường vô trọng lực:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120903.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120904.webp)

Đến tháng 11, họ đã thu hoạch được 26 quả ớt phát triển khỏe mạnh. 12 quả được gửi về Trái Đất phục vụ phân tích sinh học, số còn lại được các phi hành gia chế biến thành món Taco vũ trụ với hương vị rất thơm ngon:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120905.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120906.webp)

Đây là cuộc thử nghiệm nuôi cấy thực vật kéo dài nhất (hơn 4 tháng) trong không gian của NASA, mở ra hướng đi tự cung cấp thực phẩm tươi sống cho các phi hành trình dài ngày trong tương lai.

2、[Năm bùng nổ của thị trường thiết bị thực tế ảo VR](https://twitter.com/JackSoslow/status/1471549480595955716)

Năm 2021 đánh dấu sự cất cánh mạnh mẽ của các thiết bị thực tế ảo cá nhân. Dòng kính VR Quest 2 của hãng Oculus (thuộc Meta) đã đạt doanh số bán ra kỷ lục 8,1 triệu máy trên toàn cầu, vượt qua cả doanh số máy chơi game Xbox của Microsoft (8 triệu máy):

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122706.webp)

Đặc biệt trong kỳ nghỉ Giáng sinh, ứng dụng Oculus đã vươn lên dẫn đầu bảng xếp hạng ứng dụng miễn phí tải nhiều nhất trên App Store Mỹ, chứng tỏ kính VR đã trở thành món quà công nghệ được yêu thích nhất của các gia đình:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122707.webp)

Trải nghiệm thực tế ảo hiện đã tiệm cận độ trưởng thành cao, không chỉ phục vụ chơi game mà còn ứng dụng rộng rãi vào các chương trình tập thể thao tại nhà:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122708.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122709.webp)

3、[Citroen giới thiệu mẫu xe điện ý tưởng trang bị bánh xe dạng cầu](https://www.byri.net/2021/09/29/citroen-an-urban-autonomous-and-interchangeable-vehicle-concept/)

Nhân kỷ niệm 100 năm thành lập, hãng xe Pháp Citroen đã công bố mẫu xe điện đô thị tương lai với thiết kế đột phá:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122908.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122909.webp)

Xe sử dụng 4 bánh xe dạng quả cầu lăn cho phép di chuyển linh hoạt theo mọi hướng mà không cần cua góc. Đồng thời, phần khung gầm tự hành có thể tách rời để lắp ghép với các kiểu dáng thân xe khác nhau tùy mục đích sử dụng:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122910.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122911.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122912.webp)

4、[Nhà xuất bản Springer Nature thu hồi 44 bài báo khoa học vô nghĩa](https://retractionwatch.com/2021/11/04/springer-nature-geosciences-journal-retracts-44-articles-filled-with-gibberish/)

Nhà xuất bản học thuật danh tiếng Springer Nature vừa thông báo thu hồi 44 bài báo khoa học đã đăng trên tạp chí *Arabian Journal of Geosciences* do nội dung hoàn toàn vô nghĩa và phi logic. Một số tiêu đề bài báo bao gồm:

> - *Giám sát và cảnh báo sạt lở đất dựa trên môi trường phân tán và tính toán hiệu quả rèn luyện thể chất.*
> - *Dự báo xu hướng lượng mưa đô thị và quản lý lo âu ở thanh thiếu niên dựa trên mạng thần kinh.*
> - *Phân tích lượng mưa vùng ven biển và hệ thống gợi ý sách thư viện thông minh hướng tới Internet vạn vật.*

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112505.webp)

Nội dung bên trong các bài báo cũng hoàn toàn là những từ ngữ được chắp vá vô căn cứ:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112504.webp)

Hầu hết các bài báo này đều đứng tên bởi các tác giả từ Trung Quốc. Ban biên tập giải thích nguyên nhân sự cố do tài khoản email của các biên tập viên bình duyệt đã bị tin tặc tấn công để tự động phê duyệt và đẩy bài lên hệ thống xuất bản tự động.

## 文章

1、[Danh sách các nhà cung cấp linh kiện Trung Quốc của tập đoàn Apple năm 2020](https://weibo.com/ttarticle/p/show?id=2309404718623225937978)（Tiếng Trung）

Bài phân tích chi tiết về 48 doanh nghiệp Trung Quốc đại lục và Hồng Kông lọt vào danh sách 200 nhà cung cấp linh kiện lớn nhất thế giới của Apple, cùng bài viết phân tích sâu về [sự dịch chuyển địa lý của chuỗi cung ứng](https://weibo.com/ttarticle/p/show?id=2309404720079463121314).

2、[Giáo sư Nhật Bản tiến hành tháo rã mẫu xe điện giá rẻ Wuling Hongguang Mini EV](https://mp.weixin.qq.com/s/OSSXtVc5KcxQjSYS908dtQ)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122603.webp)

Mẫu xe điện mini của Wuling đạt doanh số kỷ lục tại Trung Quốc nhờ mức giá siêu rẻ chỉ từ 28.800 NDT. Một giáo sư cơ khí Nhật Bản đã tiến hành tháo rời toàn bộ chi tiết máy của xe để phân tích giải pháp cắt giảm chi phí linh kiện tối ưu của hãng.

3、[Các nguyên tắc vàng khi thiết kế kiến trúc hệ thống của tôi](https://coolshell.cn/articles/21672.html)（Tiếng Trung）

Bài viết chia sẻ kinh nghiệm quý báu của tác giả Chen Hao (chủ biên trang blog công nghệ CoolShell nổi tiếng) về các nguyên tắc cốt lõi khi thiết kế hệ thống phần mềm quy mô lớn đúc kết sau hơn 20 năm làm việc. (Đóng góp của [@lyf2nb](https://github.com/ruanyf/weekly/issues/2120))

4. [Defensive CSS: Viết mã CSS phòng thủ tránh vỡ giao diện](https://ishadeed.com/article/defensive-css/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121101.webp)

Giới thiệu các mẹo viết CSS thông minh giúp trang web hiển thị ổn định, tự động co giãn nội dung văn bản và hình ảnh mượt mà trên nhiều kích cỡ màn hình khác nhau mà không làm lỗi layout.

5、[Tại sao hiệu năng của cơ sở dữ liệu IndexedDB trên trình duyệt lại chậm?](https://rxdb.info/slow-indexeddb.html)（Tiếng Anh）

IndexedDB là bộ lưu trữ dữ liệu tiêu chuẩn tích hợp trong trình duyệt web nhưng thường gặp phàn nàn về tốc độ. Bài viết phân tích sâu nguyên nhân cơ chế ghi ổ đĩa của trình duyệt và đề xuất các giải pháp tối ưu hóa truy vấn.

6. [Các thiết lập bảo mật cần làm ngay trong 5 phút đầu tiên khi thuê VPS Linux](https://sollove.com/2013/03/03/my-first-5-minutes-on-a-server-or-essential-security-for-linux-servers/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120816.webp)

Hướng dẫn ngắn gọn các thao tác bảo mật cơ bản như đổi cổng SSH mặc định, tắt quyền đăng nhập user root và cấu hình tường lửa UFW để bảo vệ máy chủ Linux mới khởi tạo.

7、[Sử dụng Docker để ảo hóa môi trường chạy ứng dụng cục bộ](https://nystudio107.com/blog/dock-life-using-docker-for-all-the-things)（Tiếng Anh）

Tác giả chia sẻ phương pháp sử dụng các container Docker để chạy các công cụ phát triển (như Node.js, Composer, Python) thay vì cài đặt trực tiếp lên hệ điều hành máy tính, giúp máy sạch sẽ và tránh xung đột phiên bản. (Đóng góp của [@AlexChingEraser](https://github.com/ruanyf/weekly/issues/2122))

8、[Tổng hợp các tính năng hứa hẹn của Apple năm 2021 nhưng vẫn chưa xuất hiện](https://www.macworld.com/article/557089/apple-ios-macos-features-universal-control-xcode.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120809.webp)

Điểm danh các tính năng phần mềm cao cấp (như Universal Control hỗ trợ dùng chung chuột bàn phím Mac/iPad hay Xcode Cloud) vốn được Apple công bố tại WWDC nhưng liên tục bị trì hoãn cập nhật.

## 工具

1、[deeplinks.js: Thư viện JavaScript tạo liên kết neo phân đoạn văn bản](https://github.com/WesleyAC/deeplinks)

Thư viện JavaScript nhỏ gọn giúp tự động tạo ra một liên kết URL chứa mã neo định vị phân đoạn văn bản cụ thể mà người dùng bôi đen, giúp người đọc sau nhảy trực tiếp tới đúng dòng chữ đó.

2、[AltTab: Mang tính năng Alt+Tab của Windows lên macOS](https://alt-tab-macos.netlify.app/)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121110.webp)

Ứng dụng nguồn mở hữu ích mô phỏng chính xác giao diện hiển thị ảnh thu nhỏ của các cửa sổ khi bấm Alt+Tab trên Windows mang lên hệ điều hành macOS.

3、[Xitu Juejin Extension: Tiện ích trang chủ dành cho nhà phát triển](https://juejin.cn/extension)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122905.webp)

Trình tiện ích mở rộng trình duyệt tổng hợp các bài viết công nghệ, xu hướng nổi bật hàng ngày từ các diễn đàn Juejin, GitHub, V2ex, Zhihu về một trang chủ gọn gàng giúp lập trình viên cập nhật tin tức nhanh.

4、[Weekly RSS Push: Tự động gửi số tuần mới về Slack/WeChat](https://github.com/ruanyf/weekly/issues/2132)

Giải pháp ứng dụng GitHub Actions giúp tự động đẩy nội dung bản tin tuần mới xuất bản về hòm thư nhóm trên Slack hoặc doanh nghiệp WeChat. (Đóng góp của [@ronething](https://github.com/ruanyf/weekly/issues/2132))

5、[Online Resume Generator: Trình tạo CV trực tuyến từ kho lưu trữ GitHub](https://github.com/visiky/resume)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021123005.webp)

Trình tạo trang sơ yếu lý lịch trực tuyến đẹp mắt, tự động đồng bộ hóa thông tin cá nhân từ file dữ liệu JSON/YAML được lưu trữ trên kho GitHub của bạn. (Đóng góp của [@visiky](https://github.com/ruanyf/weekly/issues/2131))

6、[SpiderFlow: Nền tảng thiết kế công cụ cào dữ liệu web kéo thả trực quan](https://github.com/ssssssss-team/spider-flow)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021123002.webp)

Hệ thống quản lý công cụ cào web nguồn mở viết trên Java, hỗ trợ lập trình viên xây dựng luồng lấy dữ liệu (crawler) thông qua sơ đồ khối kéo thả mà không cần viết code. (Đóng góp của [@dllen](https://github.com/ruanyf/weekly/issues/2125))

7、[pinyin-pro: Thư viện chuyển đổi chữ Hán sang phiên âm Pinyin](https://github.com/zh-lx/pinyin-pro)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021123001.webp)

Thư viện JavaScript hiệu năng cao hỗ trợ chuyển đổi từ chữ Hán sang dạng ký tự phiên âm Latin Pinyin đầy đủ dấu thanh. (Đóng góp của [@zh-lx](https://github.com/ruanyf/weekly/issues/2121))

8、[DooringX: Khung phát triển low-code kéo thả trang H5](https://github.com/H5-Dooring/dooringx)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021123004.webp)

Bộ mã nguồn mở hỗ trợ các nhà phát triển tự thiết lập và vận hành một nền tảng low-code riêng biệt phục vụ thiết kế nhanh giao diện H5 di động. (Đóng góp của [@MrXujiang](https://github.com/ruanyf/weekly/issues/2128))

9、[LaTeX Editor: Trình soạn thảo văn bản hỗ trợ xuất mã LaTeX](https://github.com/SoftMaple/Editor)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021123007.webp)

Trình soạn thảo trực tuyến mã nguồn mở hỗ trợ định dạng căn lề và xuất nhanh tài liệu sang mã ký tự LaTeX chuyên nghiệp. (Đóng góp của [@007tom](https://github.com/ruanyf/weekly/issues/2136))

10、[wfrest: Thư viện C++ xây dựng dịch vụ Rest API gọn nhẹ](https://github.com/wfrest/wfrest)

Bộ khung lập trình C++ siêu nhỏ gọn hỗ trợ các lập trình viên hệ thống khởi chạy nhanh một máy chủ dịch vụ web Restful API đạt hiệu năng xử lý cao. (Đóng góp của [@chanchann](https://github.com/ruanyf/weekly/issues/2127))

## 资源

1、[Trung Quốc triết học thư điện tử hóa kế hoạch (Ctext.org)](https://ctext.org/zhs)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021123006.webp)

Thư viện số hóa học thuật khổng lồ lưu trữ kho tàng thư tịch, tác phẩm triết học cổ điển Trung Hoa phong phú với hơn 3 vạn đầu sách. (Đóng góp của [@kernelry](https://github.com/ruanyf/weekly/issues/2133))

2、[Shuge (书格): Thư viện mở lưu trữ sách cổ scan màu chất lượng cao](https://new.shuge.org/)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021123003.webp)

Thư viện số phi lợi nhuận cung cấp các bản quét màu chất lượng cao của hàng ngàn cuốn sách cổ quý hiếm định dạng PDF cho phép tải xuống miễn phí. (Đóng góp của [@alaskasquirrel](https://github.com/ruanyf/weekly/issues/2126))

3、[Software Engineering fundamentals checklist: Tiêu chuẩn kiểm tra chất lượng phần mềm của Microsoft](https://microsoft.github.io/code-with-engineering-playbook/ENG-FUNDAMENTALS-CHECKLIST/)

Bộ cẩm nang liệt kê đầy đủ các đầu việc kiểm tra chất lượng mã nguồn, quy trình thử nghiệm và CI/CD do Microsoft phát hành cho các nhóm phát triển.

4、[InterfaceLIFT: Trang tải ảnh nền máy tính chất lượng cao](https://interfacelift.com/wallpaper/downloads/downloads/any/)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112905.jpg)

Website chia sẻ kho hình nền phong cảnh thiên nhiên độ nét cao 4K/8K miễn phí phù hợp cho nhiều kích thước màn hình máy tính và điện thoại.

5、[The Joy of Cryptography: Giáo trình mật mã học cơ bản trực tuyến](https://joyofcryptography.com/)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112515.jpg)

Cuốn sách giáo khoa tiếng Anh trực tuyến giới thiệu các khái niệm lý thuyết mật mã học cơ bản dành cho sinh viên đại học chuyên ngành an toàn thông tin.

## 图片

1、[Chiếc đồng hồ sáu mặt cơ khí phức tạp nhất Nhật Bản thế kỷ 19](https://watchesbysjx.com/2016/09/how-japans-thomas-edison-built-the-nations-most-complicated-clock.html)

Hisashige Tanaka (1799—1881) là một nhà phát minh lỗi lạc được mệnh danh là "Edison của Nhật Bản". Ông là người đã chế tạo đầu máy xe lửa hơi nước đầu tiên của Nhật, đặt nền móng cho tập đoàn công nghệ Toshiba sau này.

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021100201.jpg)

Năm 1851, ông đã hoàn thành chiếc đồng hồ cơ khí sáu mặt kỳ diệu cấu tạo từ hơn 1.000 chi tiết cơ khí tinh xảo:

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021100202.jpg)

Đỉnh đồng hồ là một mô hình渾 thiên nghi có mặt kính đại diện cho Nhật Bản với hai quả cầu Mặt Trời và Mặt Trăng quay quanh biểu thị vị trí thực tế của chúng. Sáu mặt của đồng hồ hiển thị các thông tin đo lường thời gian khác nhau bao gồm: chu kỳ 24 tiết khí địa phương (hình dưới), năm thiên can địa chi và hệ 12 giờ tiêu chuẩn phương Tây. Thiết bị hoạt động hoàn toàn bằng hệ thống dây cót cơ học có thể chạy liên tục suốt một năm sau mỗi lần lên dây.

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021100204.jpg)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021100206.jpg)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021100208.jpg)

2、[Cây thông Noel vẽ theo các trường phái kiến trúc kinh điển](https://www.instagram.com/p/CX84PQ6okFY/)

Một họa sĩ đã đăng tải hình ảnh minh họa thú vị: nếu cây thông Noel được thiết kế bởi các kiến trúc sư thuộc các trường phái nghệ thuật kinh điển, chúng sẽ trông như thế nào?

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122921.webp)

Các mẫu cây thông trên hình đại diện cho các trường phái nghệ thuật (theo thứ tự từ trái qua phải, từ trên xuống dưới) bao gồm: Tối giản (Minimalism), Tân nghệ thuật (Art Nouveau), De Stijl (Hà Lan), Gothic, Giải cấu trúc (Deconstructivism), Hiện đại (Modernism) và Bauhaus.

## Bài đọc thêm

### Tại sao bạn không nên cố gắng cạnh tranh trực tiếp với Roblox?

Tôi nhớ trước năm 2018, hộp thư của tôi tràn ngập email từ các startup công nghệ tuyên bố rằng mục tiêu lớn của họ là đánh bại Steam - nền tảng phân phối game PC khổng lồ của Valve. Số lượng các công ty này nhiều tới mức tôi đã phải viết một bài phân tích dài để khuyên họ từ bỏ ý định điên rồ đó. Cho tới nay, hầu hết các đối thủ thách thức Steam đều đã phá sản hoặc biến mất, chỉ còn Epic Games đang bám đuổi vô cùng chật vật.

Bước sang năm 2021, hộp thư của tôi lại ngập tràn các dự án tuyên bố sẽ tạo lập hệ thống để cạnh tranh trực tiếp với Roblox - nền tảng game sandbox cộng đồng hiện định giá tới 41 tỷ USD:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122907.webp)

Tôi tin lịch sử sẽ lặp lại. Nếu bạn có ý định khởi nghiệp đối đầu trực diện với Roblox, lời khuyên chân thành duy nhất của tôi là: **Tuyệt đối đừng làm vậy!**

Roblox được ra mắt lần đầu tiên vào năm 2006, tức là cách đây đã 15 năm. Họ đã xây dựng được một khoảng cách dẫn đầu quá xa với hệ sinh thái lập trình viên game mini và lượng người dùng trẻ trung khổng lồ gắn kết chặt chẽ. Việc cố gắng tạo dựng một nền tảng tương tự để lôi kéo tệp khách hàng này là nhiệm vụ bất khả thi trong bối cảnh hiện tại. Việc khuyên bạn dừng lại là để tránh lặp lại vết xe đổ của ít nhất 12 startup công nghệ đã phá sản trước đây khi cố gắng lật đổ Steam.

## 言论

1\.

Trước đại dịch, điện thoại iPhone sản xuất tại nhà máy Foxconn Trịnh Châu được bốc thẳng lên các chuyến bay vận tải đi qua Anchorage, Alaska để cung cấp cho thị trường Mỹ. Hiện nay để tránh các quy định cách ly nghiêm ngặt, hầu hết các chuyến bay chở hàng của Trung Quốc đi Mỹ sẽ dừng chuyển tiếp tại Hàn Quốc hoặc Nhật Bản để bốc hàng sang máy bay khác. Tổ bay ban đầu sẽ bay thẳng ngược lại Trung Quốc từ Hàn Quốc/Nhật Bản để tránh tiếp xúc với nhân sự phương Tây, giúp họ không phải cách ly khi về nước.

-- Chia sẻ của một thành viên trên diễn đàn Hacker News

2\.

Năm 2021 là một năm buồn đối với tôi khi cả cha và mẹ tôi đều lần lượt qua đời. Đón Giáng sinh năm nay trong không gian vắng lặng, tôi luôn vô thức muốn gọi điện để kể cho cha nghe về những tin tức công nghệ thú vị gần đây, nhưng ông đã không còn nữa. Tôi chắc chắn rằng nếu ông còn sống, ông sẽ ngồi canh xem buổi phát sóng trực tiếp lễ phóng kính viễn vọng không gian James Webb.

-- Chia sẻ của một thành viên trên diễn đàn Hacker News

3\.

Thời hạn bảo hộ bản quyền tác phẩm tại Mỹ kéo dài tới 95 năm là quá lâu và cản trở sự phát triển văn hóa. Tôi đề xuất một phương án cải cách: miễn phí bảo hộ trong 10 năm đầu tiên, sau đó nếu muốn gia hạn bản quyền mỗi năm tiếp theo, chủ sở hữu phải trả phí lũy tiến theo công thức $10 \times 1.5^{n-1}$ (với $n$ là số năm gia hạn). Theo công thức này, phí duy trì bản quyền năm thứ 20 là 380 USD, năm thứ 30 là 22.000 USD, năm thứ 40 là 1,3 triệu USD và năm thứ 50 vọt lên mốc 75 triệu USD. Mức phí này sẽ buộc các hãng phải cân nhắc giải phóng tác phẩm về miền công cộng sớm nếu không mang lại giá trị lớn.

-- Chia sẻ của một thành viên trên diễn đàn Hacker News

## 历史上的本周

- 2020年（第 139 期）：[Thảo luận về các đột phá sinh học mới gần đây và tiềm năng ứng dụng y tế](https://www.ruanyifeng.com/blog/2020/12/weekly-issue-139.html)
- 2019年（第 87 期）：[Đề xuất giải pháp giúp nhân viên mới hòa nhập nhanh bằng cách giao nhiệm vụ viết tài liệu kỹ thuật cho nhóm](https://www.ruanyifeng.com/blog/2019/12/weekly-issue-87.html)
- 2018年（第 36 期）：[Thảo luận về nhu cầu nhân lực công nghệ tương lai: Liệu lập trình viên có rơi vào tình trạng dư thừa?](https://www.ruanyifeng.com/blog/2018/12/weekly-issue-36.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
