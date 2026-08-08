# 科技爱好者周刊（第 214 期）：你的地图是错的

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần。

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn。

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2483) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập。

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070401.webp)

Công trường xây dựng khu nhà ở bằng công nghệ in 3D quy mô lớn tại bang Texas, Mỹ. Tại công trường hầu như có rất ít công nhân, quy trình xây dựng không cần sử dụng hệ thống giàn giáo truyền thống mà thay bằng máy in 3D khổng lồ di chuyển dọc theo hệ thống滑 ray để phun hỗn hợp bê tông tạo vách tường tăng dần từng centimet. Một ngôi nhà hoàn chỉnh có thể được in hoàn tất chỉ trong vòng 1 đến 2 ngày. (Nguồn: [Lennar](https://www.lennar.com/new-homes/texas/austin/promo/auslen_3d_homes))

## 本周话题：你的地图是错的

Vào năm 2010, tại hội nghị Web 2.0 Summit diễn ra ở San Francisco, Mỹ:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070913.webp)

Ban tổ chức đã công bố một tấm bản đồ mang tên [《Internet Map》](https://www.blendinteractive.com/work/web-2.0-summit-interactive-map/) để mô tả cục diện thế giới số:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070914.webp)

Tấm bản đồ này phân chia Internet thành các vương quốc của các ông lớn thời bấy giờ: Google thống trị mảng tìm kiếm, Facebook nắm giữ mảng mạng xã hội, còn mảng thương mại điện tử là sự song hành của Amazon và eBay.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070915.webp)

Khi đó, nhà sáng lập Facebook Mark Zuckerberg đang ngồi trên sân khấu. Vừa nhìn thấy tấm bản đồ này, ông đã lập tức nói với người dẫn chương trình: *"Tấm bản đồ của anh sai rồi"*.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070916.webp)

Ông lý giải:

> *"Phần lớn nhất trên bản đồ chắc chắn phải là những vùng đất chưa được khai phá. Tấm bản đồ này khiến thế giới Internet trông giống như một trò chơi có tổng bằng không (zero-sum game), nhưng thực tế không phải vậy. Chúng ta đang khai phá các ranh giới mới và tạo ra các giá trị mới, chứ không phải đi tranh giành giật lấy chúng từ tay kẻ khác."*

Tôi cho rằng nhận định này vô cùng sâu sắc. Bản đồ mô tả thế giới đã biết, nhưng **cơ hội lớn nhất lại nằm ở những phần chưa được vẽ ra trên bản đồ**, đó mới là nơi chứa đựng các cơ hội lớn nhất.

Nếu bạn chỉ tập trung vào các mảng thị trường đã định hình trên bản đồ, sự phát triển của bạn chắc chắn sẽ xâm lấn vào ranh giới của các ông lớn hiện hữu, và họ sẽ phản kháng quyết liệt.

Ngược lại, nếu bạn hướng tầm mắt ra ngoài ranh giới bản đồ, bạn sẽ thấy một thế giới rộng lớn hơn với nhiều cơ hội để tự xây dựng một đế chế mới từ con số không. Thời gian và năng lượng của bạn sẽ được dành để giải quyết các bài toán chưa ai giải, thay vì phí hoài vào cuộc chiến zero-sum hao tổn lực lượng với các đối thủ cũ.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071301.webp)

Nhìn lại lịch sử phát triển của các gã khổng lồ Internet, hầu như không có doanh nghiệp nào vươn lên bằng cách chiếm đất của đối thủ cũ. Họ đều phát triển vượt bậc nhờ khai mở các mảng thị trường hoàn toàn mới: Microsoft mở ra kỷ nguyên hệ điều hành máy tính cá nhân, Amazon tiên phong khai phá điện toán đám mây AWS, YouTube tạo ra nền tảng chia sẻ video trực tuyến, Netflix mở đầu dịch vụ xem phim theo yêu cầu, và gần đây nhất là ByteDance bùng nổ với video ngắn định dạng dọc.

Steve Jobs từng nói một câu nổi tiếng: việc hỏi khách hàng họ muốn gì là vô nghĩa, bởi họ không biết điều đó cho đến khi bạn mang sản phẩm đặt trước mặt họ. Khai phá vùng đất mới và dẫn dắt người tiêu dùng vào đó chính là cách để trở thành kẻ thống trị. 

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071302.webp)

Elon Musk trở thành người giàu nhất thế giới cũng nhờ tiên phong trong các mảng hoàn toàn mới: sản xuất xe điện hàng loạt, thu hồi tên lửa tái sử dụng, phủ sóng internet vệ tinh tầm thấp Starlink và mục tiêu định cư Hỏa tinh. Mỗi lĩnh vực mới của ông đều có không gian phát triển khổng lồ và ông độc chiếm những diện tích mới này khi gặt hái thành công.

**Lần tới khi bạn nhìn vào tấm bản đồ công nghệ, hãy tìm kiếm những khoảng trống chưa được vẽ ra ngoài ranh giới bản đồ.** Đó mới thực sự là nơi để xây dựng sự nghiệp và phát triển vượt bậc. Đừng tự giới hạn bản thân trong thế giới hiện hữu và phí hoài năng lượng đấu đá giành giật từng chút không gian trong trò chơi zero-sum.

## 活动

1、[Diễn đàn chuyên đề Thiết kế và Thực tiễn Cơ sở dữ liệu Cloud Native](https://conf.juejin.cn/xdc2022/wap/?utm_source=ruanyfblogjiangshi)

Điện toán đám mây đang thúc đẩy sự chuyển dịch mạnh mẽ của hạ tầng cơ sở dữ liệu: từ mô hình đưa cơ sở dữ liệu lên đám mây (On Cloud) chuyển sang kiến trúc cơ sở dữ liệu Cloud Native thực thụ (In Cloud).

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071306.webp)

Tại Hội nghị nhà phát triển稀土开发者大会 diễn ra vào ngày 22 tháng 7 tới, ban tổ chức thiết lập chuyên đề công nghệ **《New Generation Cloud Native Database》** dưới sự chủ trì của chuyên gia dữ liệu Trương Lôi (ByteDance):

Các kỹ sư hàng đầu từ ByteDance, Intel, Meituan và Google Cloud sẽ chia sẻ các case study triển khai cơ sở dữ liệu đám mây thực tế tại doanh nghiệp của họ. Bạn đọc quan tâm có thể đăng ký tham gia trực tuyến miễn phí thông qua đường dẫn phía dưới:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070610.webp)

## 科技动态

1、[Thí nghiệm chỉnh sửa gen lỗi tạo ra thế hệ chuột hamster hung hãn](https://www.dailymail.co.uk/news/article-10884147/Vicious-hamsters-bred-lab-accident.html)

Công nghệ chỉnh sửa gen mang lại nhiều kỳ vọng nhưng cũng ẩn chứa các rủi ro khó lường nếu phát sinh sai lệch ngoài ý muốn. Các nhà khoa học tại Đại học Bang Georgia, Mỹ tiến hành chỉnh sửa gen của loài chuột hamster với mục tiêu tăng cường tính hòa đồng xã hội để chúng dễ chung sống với nhau hơn:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060502.webp)

Tuy nhiên, kết quả thu được hoàn toàn ngược lại mong đợi. Thế hệ chuột hamster bị chỉnh sửa gen trở nên cực kỳ hung hãn và có hành vi bạo lực bất thường. Chúng liên tục cắn xé, rượt đuổi đồng loại khi nhốt chung chuồng:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060503.webp)

Các nhà khoa học hiện vẫn chưa thể giải thích nguyên nhân dẫn tới sự thay đổi hành vi tiêu cực này. Thử nghiệm thất bại là lời cảnh tỉnh lớn về mức độ nguy hiểm của công nghệ chỉnh sửa gen nếu ứng dụng thiếu kiểm soát trên con người.

2、[Khoảnh khắc 99% nhân loại đón nhận ánh sáng Mặt Trời cùng lúc](https://www.timeanddate.com/news/astronomy/99-percent-sunlight-july-8)

Một câu hỏi thú vị trên mạng: Liệu có khoảnh khắc nào trong năm mà ánh sáng mặt trời chiếu tới nhiều người nhất cùng lúc? Các nhà thiên văn học đã tính toán và xác định được thời điểm đặc biệt này:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070904.webp)

Thời điểm đó rơi vào lúc 11:15 UTC ngày 8 tháng 7 hàng năm (khoảng 18:15 giờ Việt Nam). Khi đó, phần lớn các lục địa châu Mỹ, châu Âu, châu Phi và châu Á đều đang là ban ngày hoặc hoàng hôn, chỉ có châu Đại Dương nằm hoàn toàn trong bóng tối ban đêm.

Tổng số người có thể nhìn thấy ánh sáng mặt trời (trực tiếp hoặc ánh sáng hoàng hôn) tại thời điểm này đạt khoảng 7,7 tỷ người, chiếm tới 99% dân số thế giới. Chỉ có chưa đầy 80 triệu người đang trải qua ban đêm.

3、[Starlink ra mắt dịch vụ Internet vệ tinh hàng hải chuyên dụng](https://www.starlink.com/maritime)

Dự án internet vệ tinh Starlink của Elon Musk chính thức ra mắt gói dịch vụ Starlink Maritime dành cho tàu thuyền đi biển:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070803.webp)

Người dùng cần lắp đặt hệ thống ăng-ten chuyên dụng (ảnh dưới) để có thể truy cập mạng internet băng thông rộng ở giữa đại dương với tốc độ tải về lên tới 350 Mbps:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070804.webp)

Trước đây, liên lạc hàng hải chủ yếu phụ thuộc vào dịch vụ vệ tinh truyền thống có tốc độ rất chậm và cước phí vô cùng đắt đỏ. Dịch vụ mới của Starlink giúp giải quyết triệt để bài toán kết nối internet trên biển.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070805.webp)

Do giai đoạn đầu cần kết nối qua các trạm mặt đất trung chuyển, dịch vụ hiện tại mới phủ sóng các vùng cận hải của khu vực Âu Mỹ (phần màu xanh nhạt). Hệ thống liên lạc trực tiếp giữa các vệ tinh dự kiến hoàn thiện vào cuối năm để phủ sóng toàn bộ các đại dương trên Trái Đất. Chi phí dịch vụ khá đắt với 10.000 USD mua thiết bị ăng-ten và 5.000 USD cước thuê bao hàng tháng.

4、[Thử nghiệm cấy ghép tim lợn biến đổi gen trên bệnh nhân hiến xác](https://www.usatoday.com/story/news/health/2022/03/09/human-pig-heart-transplant-patient-dies/9437650002/)

Vào tháng 1 năm nay, các bác sĩ Mỹ đã thực hiện ca cấy ghép tim lợn biến đổi gen đầu tiên trên thế giới cho một bệnh nhân suy tim nặng. Ban đầu bệnh nhân tiến triển tốt nhưng đã qua đời sau hai tháng do biến chứng suy tim đột ngột:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071414.webp)

*(Hình ảnh bác sĩ vận chuyển tim lợn vào phòng mổ)*

Kết quả giải phẫu phát hiện sự hiện diện của một loại virus cự bào trong quả tim lợn hiến tặng, đây được dự đoán là nguyên nhân gây suy tim của bệnh nhân.

Để kiểm chứng giả thuyết, tuần này các bác sĩ đã thực hiện cấy ghép tim lợn biến đổi gen trên hai bệnh nhân chết não tự nguyện hiến xác để nghiên cứu y học. Quá trình theo dõi liên tục trong 72 giờ cho thấy các quả tim ghép hoạt động hoàn toàn bình thường và không xuất hiện hiện tượng thải ghép cấp tính, đánh dấu bước tiến mới cho công nghệ cấy ghép nội tạng động vật.

5、[Mercedes-Benz cam kết chịu trách nhiệm pháp lý nếu hệ thống lái tự động gây tai nạn](https://www.roadandtrack.com/news/a39481699/what-happens-if-mercedes-drivepilot-causes-a-crash/)

Hãng xe Mercedes-Benz tuyên bố sẽ chịu hoàn toàn trách nhiệm pháp lý trước pháp luật nếu hệ thống hỗ trợ lái tự động Drive Pilot của hãng gây ra tai nạn giao thông trên đường:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032303.webp)

Cam kết này đi ngược lại hoàn toàn với lập trường của Tesla khi hãng này luôn yêu cầu người lái chịu trách nhiệm chính do hệ thống FSD chỉ mang tính chất hỗ trợ lái.

Tuy nhiên, cam kết chịu trách nhiệm của Mercedes-Benz đi kèm các điều kiện ràng buộc ngặt nghèo bao gồm: xe di chuyển dưới vận tốc 60km/h; chạy trên các cung đường cao tốc được hệ thống Mercedes phê duyệt; vận hành vào ban ngày điều kiện thời tiết nắng ráo (không chạy trong đường hầm hoặc trời mưa); và người lái bắt buộc phải ngồi ở ghế lái theo dõi lộ trình (không được ngủ hoặc nhắm mắt).

## 文章

1、[Báo động vụ án lừa đảo vượt qua bảo mật xác thực khuôn mặt của ngân hàng](https://finance.sina.com.cn/money/bank/gsdt/2022-07-06/doc-imizmscv0377623.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071424.webp)

Bài viết đưa tin về vụ án lừa đảo công nghệ cao: tội phạm đã bẻ khóa thành công cơ chế xác thực khuôn mặt sinh trắc học kết hợp mã OTP gửi qua SMS của một ngân hàng lớn để chuyển trót lọt hàng triệu NDT của khách hàng khỏi tài khoản.

2、[Hành trình khám phá kiến trúc Hy Lạp cổ đại qua tựa game Assassin's Creed](https://web.archive.org/web/20211010121826/https://www.douban.com/note/814326492/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070708.webp)

Tựa game bom tấn *Assassin's Creed: Odyssey* nổi tiếng với việc phục dựng chi tiết và chân thực các công trình kiến trúc thời kỳ Hy Lạp cổ đại. Bài viết tiến hành so sánh, đối chiếu hình ảnh các đền đài cổ kính trong game so với các di tích lịch sử Athens thực tế ngày nay:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070709.webp)

3、[Trang web so sánh chất lượng ảnh chụp vũ trụ giữa kính James Webb và kính Hubble](https://johnedchristensen.github.io/WebbCompare/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071304.jpg)

NASA vừa công bố loạt ảnh chụp vũ trụ sâu đầu tiên từ kính viễn vọng không gian thế hệ mới James Webb. Tác giả đã xây dựng một trang web tương tác so sánh chi tiết độ nét và dải màu của các bức ảnh này so với ảnh chụp của kính tiền nhiệm Hubble phóng lên từ 30 năm trước.

4、[Hướng dẫn tự viết một component định tuyến Router trong React dưới 100 dòng code](https://github.com/ashok-khanna/react-snippets/blob/main/Router.js)（Tiếng Anh）

Bài viết chia sẻ mã nguồn kèm chú thích chi tiết giải thích cơ chế hoạt động của một bộ định tuyến (Router component) tối giản tự viết giúp lập trình viên hiểu sâu bản chất cơ chế chuyển trang trong ứng dụng React.

5、[Làm rõ 6 định kiến sai lầm phổ biến của lập trình viên về công nghệ .NET](https://blog.devgenius.io/6-net-myths-dispelled-celebrating-21-years-of-net-652795c2ea27)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031006.webp)

Bài viết phân tích và bác bỏ 6 định kiến lỗi thời của giới lập trình về hệ sinh thái .NET của Microsoft, tiêu biểu là quan điểm cho rằng .NET cồng kềnh và chỉ chạy được trên hệ điều hành Windows.

6、[Giải pháp cấu hình đăng nhập OAuth cho các trang web tĩnh dùng Cloudflare Workers](https://abyteofcoding.com/blog/oauth-with-cloudflare-workers-on-a-statically-generated-site/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120809.webp)

Hướng dẫn chi tiết cách thiết lập quy trình xác thực đăng nhập OAuth (như đăng nhập qua GitHub/Google) cho các trang web tĩnh (static sites) mà không cần xây dựng máy chủ backend chuyên dụng nhờ tận dụng serverless functions của Cloudflare Workers.

7、[Cẩm nang hướng dẫn nhập môn thiết lập chỉ mục index trong PostgreSQL](https://blog.crunchydata.com/blog/postgres-indexes-for-newbies)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012008.webp)

Bài viết giới thiệu cơ bản về các cấu trúc dữ liệu chỉ mục (như B-Tree, Hash, GIN) trong PostgreSQL và cách áp dụng chúng để tối ưu hóa tốc độ truy vấn cơ sở dữ liệu.

8、[Khám phá cơ chế quản lý gói ứng dụng độc đáo của hệ điều hành NixOS](https://blog.wesleyac.com/posts/the-curse-of-nixos)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012507.webp)

NixOS là một phân phối Linux có triết lý thiết kế hệ thống độc đáo. Bài viết phân tích cơ chế quản lý gói Nix giúp loại bỏ hoàn toàn tình trạng xung đột thư viện liên kết và hỗ trợ tính năng rollback hệ thống về trạng thái cũ an toàn.

## 工具

1、[Bud: Framework web full-stack hiệu năng cao viết bằng ngôn ngữ Go](https://github.com/livebud/bud)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051406.webp)

Bộ công cụ hỗ trợ lập trình viên xây dựng toàn bộ mã nguồn giao diện frontend và xử lý backend bằng Go, sau đó biên dịch tất cả thành một tệp tin nhị phân duy nhất để chạy trực tiếp trên máy chủ.

2、[Aspect: Tiện ích tạo nhanh component React bằng công cụ trực quan](https://dev.aspect.app/)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022051407.webp)

Ứng dụng hỗ trợ thiết kế giao diện web thông qua các công cụ kéo thả trực quan và tự động xuất ra mã nguồn React component tương ứng sạch đẹp.

3、[Vexip UI: Thư viện các component UI chất lượng cao cho Vue 3](https://www.vexipui.com/zh-CN)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071415.webp)

Bộ thư viện mã nguồn mở cá nhân thiết kế chứa hơn 70 thành phần giao diện UI tương tác mượt mà hỗ trợ đầy đủ TypeScript cho lập trình viên Vue 3. (Đóng góp của [@qmhc](https://github.com/ruanyf/weekly/issues/2493))

4、[gacm: Tiện ích dòng lệnh hỗ trợ quản lý tài khoản Git di động](https://github.com/alqmc/gacm)

Công cụ dòng lệnh nhỏ gọn hỗ trợ nhà phát triển dễ dàng cấu hình và chuyển đổi nhanh giữa các tài khoản người dùng Git (như tài khoản công ty và tài khoản cá nhân) trên máy tính. (Đóng góp của [@alqmc](https://github.com/ruanyf/weekly/issues/2496))

5、[DBER: Công cụ thiết kế trực quan sơ đồ thực thể mối quan hệ ERD](https://dber.tech/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071417.webp)

Ứng dụng web hỗ trợ thiết kế cơ sở dữ liệu trực quan: người dùng kéo thả các bảng dữ liệu để thiết lập liên kết quan hệ và xuất ra các câu lệnh SQL tương ứng để khởi tạo cơ sở dữ liệu. (Đóng góp của [@findyourmagic](https://github.com/ruanyf/weekly/issues/2501))

6、[EnvKey: Giải pháp bảo mật quản lý và phân phối biến môi trường cấu hình](https://envkey.com/)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033118.webp)

Hệ thống hỗ trợ quản lý tập trung và phân phối mã hóa các biến môi trường cấu hình (config/API keys) an toàn cho các cụm máy chủ ứng dụng mà không cần lưu trữ trực tiếp trên code.

7、[Bing Wallpaper: Tự động cào và cập nhật ảnh nền trang chủ Bing hàng ngày](https://github.com/niumoo/bing-wallpaper)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022013102.webp)

Kho lưu trữ sử dụng quy trình chạy tự động GitHub Actions để định kỳ tải về và lưu trữ các bức ảnh nền chất lượng cao trên trang chủ tìm kiếm của Bing hàng ngày.

8、[C2Rust: Công cụ hỗ trợ dịch mã nguồn viết bằng C/C++ sang Rust](https://c2rust.com/)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020310.webp)

Dự án mã nguồn mở cung cấp công cụ dịch thuật và giao diện web hỗ trợ chuyển đổi nhanh các đoạn mã C/C++ sang mã nguồn tương đương trong Rust để tối ưu hóa an toàn bộ nhớ.

9、[Paperless-ngx: Trình quản lý và lưu trữ tài liệu cá nhân nguồn mở tự host](https://github.com/paperless-ngx/paperless-ngx)

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040102.webp)

Hệ thống quản lý tài liệu wiki hỗ trợ quét ảnh văn bản, tự động nhận diện chữ viết OCR đối với các tệp tin PDF, Office và lưu trữ tập trung trên máy chủ riêng.

## 资源

1、[Bash-Oneliner: Thư mục tổng hợp các câu lệnh Bash một dòng hữu ích](https://github.com/onceupon/Bash-Oneliner)

Repo GitHub chia sẻ kho kiến thức dòng lệnh tổng hợp các câu lệnh Bash ngắn gọn, hiệu quả để xử lý dữ liệu văn bản, quản trị hệ thống và mạng.

2、[Dracula Theme: Bộ sưu tập giao diện tối Dracula đồng bộ cho các ứng dụng](https://draculatheme.com/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071416.webp)

Trang web chia sẻ giao diện tối màu Dracula kinh điển được thiết kế tương thích đồng bộ cho hơn 266 ứng dụng, trình soạn thảo mã nguồn (VS Code, Vim, Xcode) và Terminal. (Đóng góp của [@fish-404](https://github.com/ruanyf/weekly/issues/2495))

3、[Tiny Python Projects: Giáo trình PDF thực hành 22 dự án lập trình Python nhỏ](http://tinypythonprojects.com/Tiny_Python_Projects.pdf)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071006.webp)

Cuốn sách giáo trình chia sẻ bản PDF miễn phí hướng dẫn người học lập trình Python thông qua việc viết mã hoàn chỉnh cho 22 chương trình thực tế có đầy đủ test suite kiểm thử đi kèm.

4、[The Art of Assembly Language Programming: Giáo trình học lập trình hợp ngữ trực tuyến](http://www.phatcode.net/res/223/files/html/toc.html)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030806.webp)

Tác phẩm giáo trình kinh điển giới thiệu các kiến thức cơ bản về hợp ngữ (Assembly), kiến trúc CPU x86 và cơ chế hoạt động mức thấp của máy tính dành cho người mới bắt đầu.

5、[place.dog: Dịch vụ cung cấp ảnh cún con làm ảnh placeholder cho lập trình viên](https://place.dog/)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031004.webp)

Dịch vụ web hỗ trợ tạo nhanh các đường dẫn ảnh placeholder hình cún con đáng yêu với kích thước tùy chỉnh phục vụ thiết kế giao diện web Front-end.

## 图片

1\. [Tranh cãi xung quanh việc lắp đặt camera giám sát chi tiết tại bàn làm việc](https://www.qbitai.com/2022/07/36029.html)

Hình ảnh lan truyền trên mạng xã hội ghi nhận không gian làm việc của một doanh nghiệp công nghệ tại Thâm Quyến, nơi quản lý lắp đặt hệ thống camera giám sát tầm gần ngay phía trên đỉnh đầu của mỗi nhân viên:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071411.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071413.webp)

Góc quay của camera có thể thu lại chi tiết toàn bộ các thao tác và nội dung hiển thị trên màn hình máy tính của nhân viên trong giờ làm việc, dấy lên lo ngại về quyền riêng tư.

2\. [Biểu đồ dự báo quy mô dân số Ấn Độ so với Trung Quốc](https://ourworldindata.org/world-population-update-2022)

Báo cáo Dân số Thế giới của Liên Hợp Quốc dự báo dân số Ấn Độ sẽ vượt Trung Quốc vào năm tới để trở thành quốc gia đông dân nhất hành tinh, đồng thời dự báo đến cuối thế kỷ này quy mô dân số Ấn Độ sẽ lớn gấp đôi Trung Quốc (1,53 tỷ so với 767 triệu người):

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071307.webp)

3\. [Sáng kiến in ấn tờ tiền mệnh giá 0 rupee tại Ấn Độ](https://karthika2006.wordpress.com/2015/05/13/zero-rupee-note/)

Vào năm 2015, một tổ chức phi chính phủ tại Ấn Độ đã in ấn các tờ tiền có thiết kế giống hệt tờ tiền 50 rupee pháp định nhưng mang mệnh giá 0 rupee:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030805.webp)

Trên tờ tiền có in thông điệp *"Tôi cam kết không nhận hối lộ và không đưa hối lộ"*. Mục tiêu của sáng kiến là hỗ trợ người dân phản kháng nạn vòi vĩnh tiền hối lộ của các nhân viên hành chính bằng cách đưa cho họ tờ tiền 0 rupee này như một lời cảnh báo bảo vệ quyền lợi hợp pháp của công dân.

## ✍️ Bài đọc thêm

### Tổng hợp 9 vấn đề sức khỏe nghề nghiệp phổ biến của lập trình viên

Lập trình viên là công việc đòi hỏi thời gian ngồi cố định trước máy tính kéo dài nhiều giờ liên tục, dễ phát sinh các tổn hại sức khỏe nếu thiếu sự đề phòng chủ động:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071412.webp)

1. **Hội chứng ống cổ tay (RSI):** Tình trạng đau mỏi xương khớp cổ tay do các thao tác gõ phím và di chuột cường độ cao liên tục.
2. **Khô mắt và suy giảm thị lực:** Do tập trung nhìn màn hình máy tính quá lâu ở cự ly gần.
3. **Đau mỏi vai gáy và cột sống:** Phát sinh từ các thói quen ngồi sai tư thế, cúi đầu gập cổ về phía trước.
4. **Các bệnh về đường ruột và tiết niệu:** Do thói quen ngồi lì làm việc và nhịn tiểu khi bận rộn.
5. **Bệnh trĩ và các vấn đề tuyến tiền liệt:** Hệ quả trực tiếp của việc ngồi cố định trên ghế làm việc liên tục trong thời gian dài.
6. **Mất nước và khô da:** Do uống quá nhiều cà phê kích thích lợi tiểu nhưng thiếu bổ sung nước lọc.
7. **Rối loạn giấc ngủ:** Tác động của chất kích thích trong cà phê và việc thức khuya chạy tiến độ dự án.
8. **Thiếu hụt Vitamin D:** Do làm việc trong phòng kín cả ngày và ít tiếp xúc với ánh sáng mặt trời tự nhiên.
9. **Đau mỏi cơ bắp toàn thân:** Hệ quả của việc lười vận động thể chất.

## 历史上的本周

- 2021年（第 166 期）：[Thảo luận phương pháp học tập: So sánh hiệu quả tiếp thu tri thức giữa việc xem video bài giảng trực tuyến và đọc sách giấy](https://www.ruanyifeng.com/blog/2021/05/weekly-issue-166.html)
- 2020年（第 115 期）：[Bảo mật thông tin: Khuyến cáo bảo vệ và ngăn chặn rò rỉ thông tin dữ liệu bản đồ gen DNA cá nhân](https://www.ruanyifeng.com/blog/2020/07/weekly-issue-115.html)
- 2019年（第 64 期）：[Lời khuyên nghề nghiệp: Các bước định hướng và chuẩn bị kiến thức cho người mới muốn gia nhập ngành công nghệ Internet](https://www.ruanyifeng.com/blog/2019/07/weekly-issue-64.html)
- 2018年（第 13 期）：[Nhìn nhận thực tế: Tại sao bản tin công nghệ tuần này chỉ tập trung chia sẻ các chủ đề thuần túy về kỹ thuật](https://www.ruanyifeng.com/blog/2018/07/weekly-issue-13.html)

## 鸣谢

Nền tảng quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071305.webp)

（Hết）
