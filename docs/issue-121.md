# 科技爱好者周刊（第 121 期）：Tại sao loài người không ngày càng rảnh rỗi hơn?

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1315) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## Ảnh bìa

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081305.jpg)

Ngày 12 tháng 8 là "Ngày Voi Thế giới", khu du lịch Thung lũng Voi hoang dã Tây Song Bản Nạp đã chuẩn bị một bữa tiệc trái cây thịnh soạn cho những chú voi. ([Nguồn](http://big5.xinhuanet.com/gate/big5/www.xinhuanet.com/photo/2020-08/12/c_1126359736.htm))

## Chủ đề tuần này: Tại sao loài người không ngày càng rảnh rỗi hơn?

Nhiều người tin rằng cùng với sự phát triển của công nghệ, con người trong tương lai sẽ có nhiều thời gian rảnh rỗi hơn vì máy móc sẽ làm hết mọi việc.

Quan điểm này là không đúng. Ngay cả khi có máy móc thông minh cao độ, công nhân trong tương lai cũng không rảnh rỗi, thậm chí có thể còn bận rộn hơn, ít nhất là trong chế độ tư bản chủ nghĩa.

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081908.jpg)

Gần 100 năm trước vào năm 1930, nhà kinh tế học Keynes [dự ngôn](https://www.newstatesman.com/2020/08/why-bertrand-russells-argument-idleness-more-relevant-ever) rằng trong vòng một thế kỷ, sự nâng cao của năng suất lao động sẽ giúp cư dân các nước phát triển chỉ cần làm việc 15 giờ mỗi tuần mà vẫn duy trì được mức sống đàng hoàng.

Dự báo của ông hoàn toàn sai lầm. Ngày nay, không có quốc gia nào thực hiện chế độ làm việc 15 giờ một tuần, thậm chí không có nước nào đạt gần mức đó, ngược lại còn xuất hiện các chế độ làm việc như 996 (9h sáng đến 9h tối, 6 ngày/tuần). Tôi tin rằng, 100 năm nữa cũng sẽ không có chế độ làm việc 15 giờ một tuần.

Hãy tưởng tượng một kịch bản giả định. Một nhà máy trước đây mỗi ngày sản xuất 100 sản phẩm, nhờ tiến bộ công nghệ, nay mỗi ngày có thể sản xuất 200 sản phẩm. Nếu có thể bán hết toàn bộ, thì thời gian lao động của công nhân sẽ không hề giảm đi.

Nếu thị trường vẫn như cũ, chỉ bán được 100 sản phẩm, thì nhà máy sẽ thừa ra 50% năng lực sản xuất. Lúc này, ban quản lý có hai lựa chọn.

Lựa chọn 1: Công nhân chỉ làm việc nửa ngày, giữ nguyên tiền lương.

Lựa chọn 2: Giữ lại một nửa số công nhân, sa thải số còn lại.

Trong thực tế, chắc chắn sẽ là lựa chọn thứ hai, bởi vì điều này có lợi cho việc tăng lợi nhuận. Vì vậy, **lợi ích do tiến bộ công nghệ mang lại sẽ không biến thành thời gian rảnh rỗi của công nhân, mà biến thành việc một số công nhân bận rộn hơn, số khác thì thất nghiệp**, người chiến thắng thực sự là các nhà tư bản, lợi nhuận gia tăng đều thuộc về họ.

Đó chính là điều đang diễn ra trên thế giới hiện nay, những công nhân dư thừa cuối cùng sẽ bị sa thải. Ngành IT là rõ ràng nhất, bởi vì tiến bộ công nghệ có ảnh hưởng lớn nhất đến ngành này.

Chủ nghĩa tư bản theo đuổi tối đa hóa lợi nhuận, một khi doanh số bán hàng không thể mở rộng đồng bộ, tiến bộ công nghệ tất yếu dẫn đến sa thải nhân sự. Những người thất nghiệp nếu không kịp thời tìm được công việc mới sẽ ngày càng nghèo đi. Những người còn lại ở vị trí làm việc thì do phải gánh vác nhiều năng suất hơn mà ngày càng bận rộn hơn.

## Giáo trình Webpack miễn phí

Phát triển front-end hiện nay, công cụ đóng gói hầu hết đều chọn Webpack, giúp gộp các module khác nhau thành một script duy nhất.

Ai dùng qua đều biết Webpack không phải phần mềm dễ dùng, người mới bắt đầu tiếp cận và hiểu nó không hề dễ dàng. Hơn nữa, nó còn liên tục ra phiên bản mới và thêm tính năng mới.

Phiên bản Webpack 5.0 đã được phát triển gần hai năm, hiện tại đã ra tới bản beta 27 nhưng ngày phát hành chính thức vẫn còn rất xa vời. Tại sao phiên bản 5.0 lại khó sinh đến vậy? Nguyên nhân là nó đưa vào hai khái niệm mới là "micro front-end" và "module federation", [tài liệu chính thức](https://webpack.js.org/concepts/module-federation/) viết rất trừu tượng. Sau khi các tính năng này ra mắt, độ khó học có lẽ sẽ lại tăng lên.

Hôm nay nói đến Webpack vì tài liệu khóa học tuần này là 《Giáo trình Webpack》 từ **Kaikeba**. Giáo trình mới ra lò, miễn phí, giảng giải nguyên lý xây dựng và đóng gói - vốn là nền tảng để hiểu Webpack, và hướng dẫn mọi người tự triển khai một Webpack đơn giản.

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020082101.jpg)

Giáo trình này đúc kết ưu điểm của các giáo trình khác, cố gắng giải thích nguyên lý một cách đơn giản nhất, bạn nào quan tâm có thể nghe thử.

Click vào [liên kết](https://wx.kaikeba.com/vip_course/oruqbzt28r/74wti6v05e?tenant=wx5046bc7413796142) hoặc quét mã QR bên dưới để nhận.

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020082003.jpg)

## Tin tức

1、[Nước mắt của chim và bò sát giống con người](https://phys.org/news/2020-08-bird-reptile-human.html)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081307.jpg)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081308.jpg)

Để nghiên cứu sự tiến hóa của nước mắt, các nhà khoa học Brazil đã kiểm tra nước mắt của 7 loài chim và bò sát gồm vẹt, đại bàng, cú, rùa, cá sấu v.v. Hình trên là việc thu thập nước mắt từ đại bàng và cá sấu.

Kết quả phát hiện nước mắt của chim và bò sát rất giống con người, đều chứa lượng chất điện giải tương tự (natri và clorua), tuy nhiên nước mắt của cú và rùa biển chứa lượng urê và protein cao hơn. Điều này cho thấy nước mắt về cơ bản không tiến hóa nhiều.

2、[Máy tính xách tay lắp Raspberry Pi](https://www.tomshardware.com/news/raspberry-pi-zero-replaces-broken-laptop-optical-drive)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020080801.jpg)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020080802.jpg)

Máy tính xách tay cũ thường có ổ đĩa quang nay đã ít dùng. Một người đam mê máy tính đã tháo ổ đĩa quang ra và độ vào đó một chiếc Raspberry Pi (phiên bản Zero W), khay đựng cũng do anh tự in 3D.

Việc này tương đương với việc laptop chứa hai máy tính bên trong. Raspberry Pi lấy nguồn từ laptop, laptop bật thì Raspberry Pi cũng chạy. Màn hình, chuột và bàn phím của laptop có thể dùng để điều khiển Raspberry Pi qua giao thức VNC để remote vào hệ thống.

3、[Màn hình OLED trong suốt](https://oled.com/oleds/transparent-oleds-toleds/)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081403.jpg)

Xiaomi tuần này công bố tivi trong suốt (hình trên), khi tắt máy trông giống một tấm kính trong suốt, khi bật máy biến thành màn hình hiển thị. Nguyên lý rất đơn giản, kẹp một tấm OLED giữa hai lớp kính, điốt phát quang áp dụng công nghệ điện cực trong suốt đã chín muồi để tạo ra màn hình trong suốt, nhưng độ trong suốt chắc chắn không bằng kính thường.

Ứng dụng lớn nhất của công nghệ này là lắp trên cửa sổ xe ô tô (hình dưới). Cửa sổ tàu điện ngầm Bắc Kinh qua máy chiếu cũng cho hiệu quả hiển thị trong suốt rất炫, xem [video dưới đây](https://v.qq.com/x/page/r3135dmqctc.html).

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081404.jpg)

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=r3135dmqctc" allowFullScreen="true" width="600px" height="400px"></iframe>

4、[Pin gạch đỏ](https://arstechnica.com/science/2020/08/how-to-turn-regular-bricks-into-electricity-storying-supercapacitors/)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081501.jpg)

Đội ngũ nghiên cứu của Đại học Washington tại Mỹ thử nghiệm một phát minh rất sáng tạo: biến gạch đỏ thông thường thành pin dựa trên nguyên lý tích năng lượng của tụ điện. Do gạch đỏ chứa sắt và cấu trúc nhiều lỗ xốp bên trong có diện tích bề mặt lớn, sau khi phủ lớp sơn đặc biệt vào các lỗ xốp, sự tương tác giữa lớp phủ và nguyên tố sắt giúp nó tích trữ năng lượng như một siêu tụ điện.

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081502.jpg)

Một viên gạch có thể sạc đầy trong 15 giây và thắp sáng bóng LED trong 11 phút. Tuy nhiên dung lượng điện khá nhỏ, mỗi mét vuông tường tích được khoảng 1.6 Wh, nghĩa là một bức tường 3x6m tích được khoảng 20 Wh, chưa có giá trị thực tiễn.

5、[Nhiệt độ cao nhất trên bề mặt Trái đất](https://bnonews.com/index.php/2020/08/temperature-at-californias-death-valley-reaches-130f/)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081801.jpg)

Ngày 16 tháng 8, nhiệt độ tại Thung lũng Chết (Death Valley), California đạt 54.4 độ C, là mức nhiệt độ cao thứ ba từng được ghi nhận trên bề mặt Trái đất.

Hơn 100 năm trước vào ngày 10/7/1913 cũng tại đây đã ghi nhận nhiệt độ kỷ lục 56.7 độ C chưa bị phá vỡ. Tại sao nơi này lại nóng kỷ lục thế giới là điều kỳ lạ. Thung lũng Chết nằm ở vĩ độ 36.5 độ Bắc, cùng vĩ độ với thành phố Tế Nam, Sơn Đông, cũng không phải vùng sâu trong nội địa và chỉ cách bờ biển hơn 200 km.

6、**Tin tức một câu**

> - [Tòa án Mỹ](https://techcrunch.com/2020/08/07/goodbye-paramount-consent-decrees/) bãi bỏ lệnh cấm kéo dài 70 năm, cho phép các hãng sản xuất phim sở hữu rạp chiếu phim. Nguyên nhân là sự trỗi dậy của các hãng streaming như Netflix khiến quy định này trở nên vô nghĩa.

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020080805.jpg)

> - [Apple](https://www.iphoneincanada.ca/news/apple-legal-action-pear-logo/) kiện một ứng dụng mua sắm gia đình yêu cầu đổi Logo vì quá giống quả táo của hãng. Nhưng xem hình bên dưới thì chả giống chút nào.

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020080901.jpg)

> - [Hiệp hội Bầu trời Tối quốc tế](https://www.atlasobscura.com/articles/dark-sky-photographs) tổ chức cuộc thi ảnh thường niên cho mọi người nộp ảnh dải Ngân hà hay ô nhiễm ánh sáng. Trong số ảnh đoạt giải có một bức ảnh chụp Vạn Lý Trường Thành cho thấy ô nhiễm ánh sáng rất nghiêm trọng.

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081104.jpg)

> - [Tại Triển lãm Môi trường Thượng Hải](https://www.instagram.com/p/CD8MbPuhpbn/?igshid=y7htfs2hn65), hãng trưng bày xe quét dọn tự động có thể tự nhặt chai nước, giấy vụn, đầu thuốc lá trên đường.

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081803.jpg)

> - [Các nhà thiên văn học](https://phys.org/news/2020-08-fastest-star.html) phát hiện ngôi sao di chuyển nhanh nhất vũ trụ với tốc độ đạt 8% tốc độ ánh sáng.

> - [Microsoft](https://www.theverge.com/2020/8/17/21372487/microsoft-internet-explorer-11-support-end-365-legacy-edge) thông báo năm sau sẽ chấm dứt hỗ trợ cho trình duyệt IE 11 và Edge phiên bản cũ.

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081903.jpg)

## Bài viết

1、[Nghệ thuật tạo hình bằng CSS](https://generative-art-with-css.commons.host/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081203.jpg)

Tác giả giới thiệu cách dùng CSS để tạo ra các hình dạng đồ họa khác nhau.

2、[Cách dùng Rust phát triển Single Page Application](http://www.sheshbabu.com/posts/rust-wasm-yew-single-page-application/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081204.jpg)

Single Page App thường viết bằng JavaScript, nhưng nhờ WebAssembly nên các ngôn ngữ khác cũng có thể compile thành JavaScript. Bài viết hướng dẫn dùng Rust viết SPA giúp nhà phát triển backend viết được front-end.

3、[Sự khác biệt giữa Manjaro và Arch Linux](https://itsfoss.com/manjaro-vs-arch-linux/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081401.jpg)

Manjaro và Arch đều là bản phân phối Linux phổ biến, Manjaro dựa trên Arch nhưng có đặc điểm nổi bật riêng.

4、[Công ty có một nhà sáng lập hoạt động tốt hơn](https://www.growthclub.online/post/research-says-solo-founders-perform-better-here-is-why)（Tiếng Anh）

Lời khuyên thông thường là bạn nên lập team trước khi khởi nghiệp. Nhưng thống kê cho thấy công ty có một nhà sáng lập dễ sinh lời hơn, bài viết phân tích nguyên nhân.

5、[Giải thích entropy bằng đàn cừu](https://aatishb.com/entropy/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081504.jpg)

Bài viết dùng đàn cừu làm ví dụ giải thích entropy vật lý là do xác suất dẫn đến.

6、[Thuật toán CRDT có phù hợp cho chỉnh sửa tài liệu thời gian thực nhiều người không?](https://blog.kevinjahns.de/are-crdts-suitable-for-shared-editing/)（Tiếng Anh）

Thuật toán CRDT dùng đồng bộ dữ liệu phân tán, ví dụ cùng chỉnh sửa tài liệu. [Yjs](https://github.com/yjs/yjs) là một thư viện triển khai CRDT, tác giả giải thích sâu về thuật toán này.

7、[Giới thiệu sơ lược TypeScript](https://www.warambil.com/typescript-why-is-so-important)（Tiếng Anh）

Bài viết giới thiệu TypeScript cho người mới bắt đầu rất ngắn gọn.

8、[Giải thích về HTML smuggling](https://outflank.nl/blog/2018/08/14/html-smuggling-explained/)（Tiếng Anh）

Nhiều người không biết JavaScript có thể dùng script để tạo ra file exe cho người dùng tải về. Bài viết giải thích cách nhúng file thực thi độc hại vào trang web.

9、[Sự thật đằng sau tin nhắn quảng cáo hủy đăng ký](https://daily.zhihu.com/story/9726870)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081909.jpg)

Nhiều tin nhắn quảng cáo bảo soạn tin T để hủy đăng ký, nhưng sau khi soạn tin T thì chuyện gì xảy ra? ([@9527q](https://github.com/ruanyf/weekly/issues/1378) đóng góp)

10、[Trải nghiệm đầu tiên về WeChat Minishop](https://juemuren4449.com/archives/wechat-minishop)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081910.jpg)

Ngày 14/7 WeChat mở thử nghiệm tính năng mở cửa hàng chính thức WeChat Minishop khác với các dịch vụ bên thứ ba. Bài viết giới thiệu quy trình đăng ký và trải nghiệm. ([@juemuren4449](https://github.com/ruanyf/weekly/issues/1380) đóng góp)

## Công cụ

1、[QRpicture](https://www.qrpicture.com/)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081503.jpg)

Một công cụ trực tuyến biến hình ảnh thành mã QR có thể quét được.

2、[isoflow](https://isoflow.io/)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081601.jpg)

Công cụ vẽ sơ đồ khối, sơ đồ hệ thống trực tuyến.

3、[ScreenplaySubs](https://screenplaysubs.com/)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081702.jpg)

Plugin trình duyệt đồng bộ hiển thị kịch bản chữ khi xem phim trên Netflix.

4、[Quarantines Sites](https://quarantines.site/)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081704.jpg)

Công cụ trực tuyến giúp duyệt web qua nó để tránh bị theo dõi.

5、[umami](https://umami.is/)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081901.jpg)

Dịch vụ phân tích thống kê truy cập web mã nguồn mở.

6、[ts-migrate](https://github.com/airbnb/ts-migrate)

Dự án nguồn mở mới của Airbnb giúp tự động chuyển đổi code JavaScript sang TypeScript.

7、[js.cool](https://github.com/js-cool/js.cool)

Cung cấp tên miền con miễn phí `js.cool` cho các dự án nguồn mở, tương tự như `js.org`. ([@willin](https://github.com/ruanyf/weekly/issues/1379) đóng góp)

8、[Screen Share Party](https://ba.net/screen-share-party)

Trang web chia sẻ màn hình qua WebRTC, tạo link gửi cho người khác xem trực tiếp màn hình của bạn.

9、[maza](https://github.com/tanrax/maza-ad-blocking)

Một bộ chặn quảng cáo local thông qua việc chặn DNS. Nó cực kỳ đơn giản vì chỉ là một Bash script, rất tốt để làm ví dụ học viết script.

## Tài nguyên

1、[统计学习导论](http://faculty.marshall.usc.edu/gareth-james/ISL/)（An Introduction to Statistical Learning）

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020080508.jpg)

Sách điện tử tiếng Anh miễn phí cho sinh viên không chuyên toán, tập trung vào cơ sở thống kê của Machine Learning với ví dụ bằng ngôn ngữ R.

2、[rms.sexy](https://rms.sexy/)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081001.jpg)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081002.jpg)

Trang web chuyên thu thập hình ảnh Richard Stallman sử dụng laptop.

3、[Bản đồ lịch sử New York năm 1940](https://1940s.nyc/map/)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081402.jpg)

Bản đồ online cho phép xem không gian New York thập niên 1940 và các ảnh lịch sử tương ứng của từng địa điểm.

4、[AI phục dựng hoàng đế La Mã](https://voshart.com/ROMAN-EMPEROR-PROJECT)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081602.jpg)

Dự án dùng AI phục dựng tượng hoàng đế La Mã thành ảnh chân dung sắc nét như người thật.

5、[Danh mục sách Vật lý](https://www.susanjfowler.com/blog/2016/8/13/so-you-want-to-learn-physics)

Tác giả liệt kê một danh sách sách tiếng Anh tự học vật lý đạt trình độ đại học và sau đại học.

6、[Trực quan hóa dư luận báo chí dịch COVID-19](https://pearmini.gitee.io/ncovis-2020/#/)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081911.jpg)

Dự án trực quan hóa phân tích ảnh hưởng của dịch bệnh tới dư luận và tin tức của VisLab đại học Sơn Đông. ([@pearmini](https://github.com/ruanyf/weekly/issues/1382) đóng góp)

## Hình ảnh

1、[Logo NeXT](https://www.logodesignlove.com/next-logo-paul-rand)

Năm 1986 Steve Jobs chi 10 vạn USD thuê nhà thiết kế Paul Rand thiết kế Logo cho công ty máy tính NeXT.

10 vạn USD thời đó giá trị hơn 1 triệu USD bây giờ. Và đây là thành phẩm:

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081606.jpg)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081605.jpg)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081604.jpg)

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081603.jpg)

## Bài đọc thêm

1、[Hiện tượng Mpemba](https://en.wikipedia.org/wiki/Mpemba_effect)

Năm 1963, một học sinh trung học ở Tanzania tên là Mpemba phát hiện nước nóng 100 độ đóng băng nhanh hơn nước ấm 35 độ khi cùng cho vào tủ lạnh khi làm kem.

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081507.jpg)

Giáo viên vật lý cũng không giải thích nổi nên đã công bố hiện tượng này và giới vật lý gọi nó là "hiện tượng Mpemba".

![](https://cdn.beekka.com/blogimg/asset/202008/bg2020081506.jpg)

Năm 2012, Hiệp hội Hóa học Hoàng gia Anh tổ chức cuộc thi giải thích hiện tượng này, thu hút 22.000 bài viết và đưa ra hai lời giải thích được công nhận nhiều nhất:

(1) Quá lạnh (Supercooling): Nước lạnh duy trì thể lỏng dưới điểm đóng băng một thời gian lâu hơn nước nóng.

(2) Đối lưu: Nước nóng có sự đối lưu mạnh hơn giúp tản nhiệt nhanh hơn.

2、[Tại sao ngành tư vấn không hợp với tôi?](https://medium.com/@karti/why-consulting-is-not-for-me-ffdbe09bb3c1)

6 tháng trước tôi mở công ty tư vấn IT nhưng nay nhận ra ngành này không phù hợp với tôi.

Là nhà tư vấn, tôi chỉ tiếp cận một phần nhỏ bài toán của khách hàng chứ không được tham gia chiến lược toàn cục. Tôi muốn chế tạo ô tô nhưng họ chỉ thuê tôi làm vô lăng.

Khách hàng chỉ coi tôi là bên cung cấp dịch vụ chứ không phải đối tác. Tôi thích mối quan hệ sâu sắc trong công việc nhưng ở đây chỉ có những mối quan hệ hời hợt với nhiều người.

Tư vấn tiếp cận nhiều dự án vụn vặt làm mài mòn kỹ năng kỹ thuật cốt lõi. Mỗi dự án lại lặp đi lặp lại quy trình chào hàng, hợp đồng, thanh toán rất nhàm chán chứ không thể phát triển sâu dài hạn.

Tôi cần một mục tiêu chung cùng nhau tạo ra thứ gì đó lớn lao, ngành tư vấn không đem lại điều đó.

## Danh ngôn

1、

Web và trình duyệt đã phát triển đến quy mô công nghệ đáng sợ. Microsoft đã bỏ cuộc, Mozilla đang chật vật sinh tồn, Safari không đáng kể, chỉ còn duy nhất Google độc diễn.

Tôi kêu gọi Google dừng vô thời hạn việc thêm API mới vào Web và trình duyệt, nên tập trung tinh giảm tính năng, chú trọng hiệu năng, độ tin cậy và bảo mật.

-- [《Web cần dừng lại》](https://drewdevault.com/2020/08/13/Web-browsers-need-to-stop.html)

2、

Chrome 86 ẩn địa chỉ URL đầy đủ vì Google muốn thúc đẩy công nghệ AMP để giữ nội dung trên server của họ. Không có địa chỉ URL rõ ràng, người dùng không nhận ra họ đang đọc trên web Google hay web gốc.

-- Độc giả Hacker News

3、

Hậu quả cấp một của sự vô tri là đưa ra quyết định sai lầm, hậu quả cấp hai là không hiểu nổi tại sao quyết định đó lại sai.

-- [unintended consequences](https://unintendedconsequenc.es/tiktok-ban-openness-trap/)

4、

Ở Mỹ ai cũng nói về TikTok, sao không ai nói về AirDroid? Nó cũng từ Trung Quốc, hơn 100 triệu lượt tải và có quyền truy cập sâu vào thiết bị Android, lượng dữ liệu thu thập được còn nhiều hơn cả TikTok.

-- Độc giả Hacker News

5、

Năm ngoái doanh số App Store của Apple là 519 tỷ USD (gồm cả phần cứng liên quan), còn Amazon là 328 tỷ USD. Apple mới là nhà bán lẻ trực tuyến lớn nhất nước Mỹ.

-- [《Amazon không phải nhà bán lẻ trực tuyến lớn nhất》](https://www.forbes.com/sites/danrunkevicius/2020/08/17/apple-not-amazon-is-the-largest-online-retail-force/#43ce5d8764cb)

6、

Chỉ riêng việc cho tựa game Fortnite lên App Store, Apple đã bỏ túi 360 triệu USD lợi nhuận thuần trong 3 năm nhờ ăn chia 30% doanh thu.

-- [《Apple bỏ túi 360 triệu USD từ Fortnite》](https://www.businessinsider.com/apple-made-360-million-from-fortnite-in-app-purchases-2020-8)

## Nhìn lại

Tuần này năm 2019 (số 70): [Thế giới bước vào kỷ nguyên lãi suất âm nghĩa là gì](http://www.ruanyifeng.com/blog/2019/08/weekly-issue-70.html)

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082201.jpg)

Tuần này năm 2018 (số 18): [Tấn công bằng drone, rất khó phòng bị](http://www.ruanyifeng.com/blog/2018/08/weekly-issue-18.html)

![](https://cdn.beekka.com/blogimg/asset/201808/bg2018081701.jpg)

## Đăng ký

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97).

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
