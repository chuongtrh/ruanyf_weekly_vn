# 每周分享第 11 期 (Bản tin chia sẻ hàng tuần số 11)

Ghi lại những điều thú vị đáng chia sẻ tôi bắt gặp trong tuần qua, phát hành vào thứ Sáu hàng tuần.

![](https://cdn.beekka.com/blogimg/asset/201806/bg2018062901.jpg)

(Ảnh bìa: Phía sau núi Hổ Bào, Hàng Châu, 2016. Nhiều người đến suối Hổ Bào du lịch nhưng ít ai biết ngọn núi phía sau suối có thể leo lên được, từ đỉnh núi có tầm nhìn vô cùng thoáng đãng. Vượt qua ngọn núi này sẽ dẫn tới Cửu Khê, đi tiếp có thể tới làng Long Tỉnh hoặc Dương Mai Lĩnh.)

Ngày 27/6, Ủy ban TC39 đã chính thức phê duyệt tiêu chuẩn [《ECMAScript 2018 (ES2018)》](https://medium.com/front-end-hacking/javascript-whats-new-in-ecmascript-2018-es2018-17ede97f36d5), bổ sung 4 cú pháp lớn cùng một số cải tiến cú pháp nhỏ khác. Tôi xem qua danh sách đề xuất và thấy còn khoảng hơn 50 đề xuất khác đang xếp hàng chờ duyệt. Nếu tính cả các đề xuất ở Stage 0, JavaScript trong tương lai có thể bổ sung thêm hơn 100 cú pháp mới.

Chỉ 2 tháng nữa, cuộc họp tiếp theo của Ủy ban TC39 sẽ khởi động quy trình xây dựng tiêu chuẩn mới ES2019 để tích hợp thêm các cú pháp tiếp theo. Trước đây tôi cứ nghĩ các thư viện bên ngoài thay đổi nhanh, nay mới nhận ra chính bản thân ngôn ngữ lập trình cũng đang biến đổi với tốc độ chóng mặt.

Không chỉ riêng JS, hầu như tất cả các ngôn ngữ主流 hiện nay đều có xu hướng tăng tốc cập nhật. JS cập nhật cú pháp mới sau mỗi vài tháng, Java phát hành phiên bản mới mỗi nửa năm, C/C++ cập nhật sau vài năm. Bên cạnh đó, mỗi hệ điều hành lớn lại thúc đẩy ngôn ngữ độc quyền của riêng mình: Android thúc đẩy Kotlin, iOS dùng Swift, Fuchsia dùng Dart, cộng thêm Python, Go, Rust, WebAssembly... Các ngôn ngữ mới liên tục ra đời và mỗi ngôn ngữ đều nhanh chóng lặp đi lặp lại để thêm các tính năng cú pháp phức tạp.

Tôi dự đoán trong tương lai, số lượng kỹ sư tinh thông đồng thời nhiều ngôn ngữ lập trình sẽ trở nên rất ít. Bởi vì mỗi ngôn ngữ đều chứa đựng lượng kiến thức khổng lồ, việc học nhập môn thì đơn giản nhưng để đạt tới mức độ tinh thông là cực kỳ khó khăn. Mỗi lập trình viên có xu hướng chỉ chuyên sâu vào một hoặc hai hệ sinh thái ngôn ngữ cụ thể, điều này mang lại rủi ro rất lớn nếu hệ sinh thái bạn chuyên sâu gặp thoái trào và buộc phải chuyển đổi sang lĩnh vực hoàn toàn mới.

## 新闻 (Tin tức)

1、[Ứng dụng trình chiếu Keynote của Apple hỗ trợ định dạng toán học LaTeX](https://support.apple.com/en-sg/HT202501)

![](https://cdn.beekka.com/blogimg/asset/201806/bg2018062902.jpg)

Phần mềm thiết kế bài thuyết trình Keynote của Apple chính thức hỗ trợ trực tiếp cú pháp viết công thức toán học LaTeX nguyên bản từ hệ thống, mang lại trải nghiệm tuyệt vời cho giới khoa học và học thuật.

2、[Google Cloud Platform hỗ trợ môi trường chạy ứng dụng Node.js](https://cloudplatform.googleblog.com/2018/06/Now-you-can-deploy-your-Node-js-app-to-App-Engine-standard-environment.html?m=1)

Google Cloud Platform thông báo hỗ trợ chạy trực tiếp các ứng dụng Node.js trên môi trường tiêu chuẩn App Engine đi kèm chính sách miễn phí cho các ứng dụng quy mô nhỏ, giúp việc triển khai các dịch vụ web trở nên vô cùng đơn giản.

3、[CTO kiêm nhà sáng lập hệ điều hành Deepin Linux Vương Dũng tuyên bố từ chức](https://www.linuxidc.com/Linux/2018-06/152866.htm)

![](https://cdn.beekka.com/blogimg/asset/201806/bg2018062904.jpg)

Deepin là bản phân phối Linux nội địa của Trung Quốc nhận được rất nhiều sự quan tâm của cộng đồng. Nhà sáng lập kiêm CTO Vương Dũng đã đăng thông báo từ chức trên diễn đàn chính thức của hãng vì lý do cá nhân. Trong tâm thư, ông chia sẻ những áp lực và khó khăn khủng khiếp trong suốt 8 năm xây dựng hệ điều hành:

* Làm việc kiệt sức đến mức tối về phải truyền dịch y tế để hôm sau có sức tiếp tục đến công ty làm việc.
* Thường xuyên phải tiếp khách uống rượu liên tục 3 chặng mỗi tối, nôn mửa nhiều lần vẫn phải uống cạn ly.
* Tăng ca triền miên ngủ tại văn phòng công ty, vợ phải bế con nhỏ đến tận dưới sảnh công ty để ép ông phải về nhà nghỉ ngơi.
* Trải qua nhiều cú sốc tinh thần lớn trong cuộc sống khiến ông kiệt sức.

4、[Sức làm việc đáng nể ngoài tuổi 90 của các nhà lãnh đạo](https://cdn.beekka.com/blogimg/asset/201806/bg2018062905.jpg)

Thủ tướng Malaysia Mahathir Mohamad ở tuổi 92 vẫn duy trì cường độ làm việc tranh cử và diễn thuyết dày đặc trước công chúng; Chủ tịch Ủy ban Thường vụ Hội nghị Nhân dân Tối cao Triều Tiên Kim Yong-nam ở tuổi 90 đại diện tham dự khai mạc World Cup và hội kiến Tổng thống Nga Putin. Họ đã định nghĩa lại khả năng làm việc phi thường của con người ngoài 90 tuổi, báo hiệu trong tương lai xã hội hoàn toàn có thể xuất hiện thế hệ lao động trăm tuổi.

5、[Airbnb công bố lộ trình dừng sử dụng React Native để quay lại công nghệ Native](https://medium.com/airbnb-engineering/sunsetting-react-native-1868ba28e30a)

![](https://cdn.beekka.com/blogimg/asset/201806/bg2018062907.jpg)

Airbnb — một trong những thương hiệu tiên phong ứng dụng React Native từ thời kỳ đầu — chính thức thông báo dừng dự án React Native sau hơn 2 năm vận hành thực tế để chuyển đổi quay lại phát triển ứng dụng di động bằng công nghệ Native truyền thống.

Nguyên nhân cốt lõi do React Native không thể giải quyết triệt để khâu trừu tượng hóa đa nền tảng 100%. Lập trình viên vẫn buộc phải viết các đoạn code native riêng biệt để xử lý các tính năng đặc thù của từng hệ điều hành. Điều này dẫn tới yêu cầu kỹ sư phần mềm phải nắm vững cả ba nền tảng (React Native, Android và iOS) để làm chủ hệ thống, một yêu cầu quá cao so với mặt bằng nhân sự thực tế gây phát sinh hàng loạt lỗi vận hành chi tiết.

6、[Hải Nam thử nghiệm thiết lập khu vực mở mạng xã hội quốc tế Facebook và Twitter](http://news.sina.com.cn/o/2018-06-21/doc-ihefphqm2432435.shtml)

Chính quyền tỉnh Hải Nam công bố kế hoạch hành động 3 năm nâng cao quốc tế hóa du lịch địa phương. Mục tiêu đến năm 2020 thu hút 2 triệu lượt khách du lịch quốc tế và 50.000 lao động nước ngoài. Tỉnh lên kế hoạch thiết lập các khu dịch vụ quốc tế đặc thù tại Hải Khẩu và Tam Á cho phép người nước ngoài truy cập bình thường các mạng xã hội phổ biến toàn cầu như Facebook, Twitter và YouTube.

7、[Định dạng video VR180 thế hệ mới của Google](https://itsfoss.com/vr180-creator/)

![](https://cdn.beekka.com/blogimg/asset/201806/bg2018062908.jpg)

Bên cạnh định dạng video toàn cảnh 360 độ cồng kềnh cho kính VR, Google giới thiệu định dạng video VR180 chỉ quay quét không gian 180 độ phía trước sử dụng camera hai ống kính mô phỏng chính xác đôi mắt người để mang lại hiệu ứng lập thể 3D trực quan khi xem, đồng thời ra mắt công cụ biên tập video VR180 miễn phí giúp tối ưu hóa dung lượng truyền tải.

8、[YouTube ra mắt tính năng hội viên trả phí tài trợ cho kênh](https://techcrunch.com/2018/06/21/youtube-introduces-channel-memberships-merchandise-and-premieres/)

YouTube thông báo cho phép các nhà sáng tạo nội dung sở hữu trên 100.000 người đăng ký được phép kích hoạt tính năng hội viên trả phí với mức phí 4,99 USD/tháng để fan hâm mộ ủng hộ tài chính, đổi lại hội viên sẽ nhận được huy hiệu nổi bật và bộ emoji độc quyền của kênh.

9、[Tin tức vắn](https://electronjs.org/releases#3.0.0-beta.1)

* Liên minh Wi-Fi Alliance chính thức công bố chuẩn bảo mật Wi-Fi thế hệ mới WPA3 thay thế cho WPA2 giúp tăng cường khả năng mã hóa đường truyền.
* Electron ra mắt phiên bản 3.0 nâng cấp sâu các nhân Chromium, Node.js và V8.
* MongoDB 4.0 chính thức hỗ trợ tính năng giao dịch ACID (Database Transactions) đa tài liệu.

## 教程 (Hướng dẫn)

1、[Bài viết] [Kinh nghiệm sử dụng tùy chọn an toàn git push --force-with-lease](https://blog.csdn.net/wpwalter/article/details/80371264) (Tiếng Trung)

Khuyên lập trình viên nên dừng thói quen dùng lệnh đè `git push --force` nguy hiểm, thay vào đó hãy chuyển sang dùng lệnh `git push --force-with-lease`. Lệnh này sẽ tự động từ chối đẩy đè code lên nhánh nếu phát hiện có commit mới của lập trình viên khác đẩy lên trước đó mà local chưa đồng bộ.

2、[Bài viết] [Tại sao người dùng Linux luôn ưu tiên sử dụng dòng lệnh Terminal?](https://www.fossmint.com/why-linux-users-prefer-the-commandline-to-a-gui/) (Tiếng Anh)

Phân tích các ưu thế vượt trội của giao diện dòng lệnh (CLI) so với giao diện đồ họa (GUI) trong lập trình về mặt tốc độ xử lý, khả năng tự động hóa bằng script và hiệu năng tiêu thụ tài nguyên phần cứng.

3、[Tài liệu] [Hướng dẫn nhập môn hệ thống lưu trữ phân tán IPFS](https://github.com/miaoski/ipfs-tutorial) (Tiếng Trung)

IPFS (InterPlanetary File System) là giao thức truyền tải tệp tin phân tán P2P kết hợp công nghệ blockchain giúp lưu trữ dữ liệu phi tập trung không thể bị xóa hay chặn bởi bất kỳ thực thể trung gian nào. Tài liệu hướng dẫn cách cài đặt và chia sẻ tệp tin qua mã băm IPFS.

4、[Bài viết] [Các kinh nghiệm thực hành tốt nhất khi tự động hóa trình duyệt bằng thư viện Puppeteer của Google](https://docs.browserless.io/blog/2018/06/04/puppeteer-best-practices.html) (Tiếng Anh)

Tổng hợp các kinh nghiệm thực tế của chuyên gia khi viết script crawl dữ liệu và tự động hóa thao tác trình duyệt bằng Puppeteer headless Chrome để đạt hiệu năng tối ưu và tránh rò rỉ bộ nhớ.

5、[Bài viết] [Tìm hiểu thuật toán nhận diện chữ viết tay GRAIL của RAND](https://jackschaedler.github.io/handwriting-recognition/) (Tiếng Anh)

Tài liệu trực quan giới thiệu chi tiết thuật toán nhận dạng chữ viết tay kinh điển GRAIL thông qua các mô hình tương tác hoạt họa HTML5 dễ hiểu mà không sử dụng các công thức toán phức tạp.

6、[Video] [Hướng dẫn tối ưu hóa thiết kế giao diện web tương thích hệ điều hành WatchOS 5 trên Apple Watch](https://developer.apple.com/videos/play/wwdc2018/239/) (Tiếng Anh)

Bộ video bài giảng của Apple tại hội nghị WWDC hướng dẫn chi tiết các tiêu chuẩn thiết kế CSS và cấu trúc HTML giúp nội dung trang web hiển thị rõ nét trên màn hình siêu nhỏ của Apple Watch.

## 资源 (Tài nguyên)

1、[Tài liệu] [50 bộ dữ liệu mở miễn phí chất lượng cao phục vụ huấn luyện mô hình Machine Learning](https://gengo.ai/articles/the-50-best-free-datasets-for-machine-learning/) (Tiếng Anh)

Danh sách tổng hợp 50 nguồn dữ liệu mở lớn đa lĩnh vực được chọn lọc phục vụ nghiên cứu và huấn luyện AI.

2、[Dữ liệu] [Cổng API cung cấp dữ liệu trực tuyến World Cup 2018](http://worldcup.sfg.io/)

Cung cấp cổng API trả về dữ liệu định dạng JSON cập nhật liên tục theo từng phút về kết quả, thẻ phạt, cầu thủ ghi bàn của tất cả các trận đấu tại giải vô địch bóng đá thế giới.

## 工具 (Công cụ)

1、[GitTorrent](https://blog.printf.net/articles/2015/05/29/announcing-gittorrent-a-decentralized-github/)

Ý tưởng thiết kế hệ thống Git lưu trữ phi tập trung hoàn toàn không cần máy chủ trung gian dựa trên giao thức chia sẻ ngang hàng BitTorrent.

2、[neofetch](https://github.com/dylanaraps/neofetch)

![](https://cdn.beekka.com/blogimg/asset/201806/bg2018062917.jpg)

Công cụ dòng lệnh phổ biến giúp hiển thị logo hệ điều hành cách điệu bằng mã ASCII kèm theo thông tin cấu hình phần cứng CPU, RAM, OS trực tiếp trên terminal.

3、[vivid.js](https://webkul.github.io/vivid/)

Bộ sưu tập icon định dạng hình ảnh vector SVG siêu nhẹ hỗ trợ tùy biến linh hoạt kích thước và màu sắc qua code JS.

4、[Devuan](https://devuan.org/)

Bản phân phối Linux Debian đặc biệt được xây dựng để duy trì hệ thống quản lý khởi động dịch vụ `init.d` truyền thống, dành cho các kỹ sư không muốn chuyển dịch sang SystemD.

5、[usql](https://github.com/xo/usql)

Công cụ dòng lệnh universal viết bằng Go hỗ trợ kết nối và chạy truy vấn SQL đồng nhất cho hầu hết các hệ quản trị cơ sở dữ liệu phổ biến (MySQL, PostgreSQL, SQLite, MSSQL...).

6、[faceai](https://github.com/vipstone/faceai)

Dự án Python mã nguồn mở nhập môn cung cấp các đoạn code mẫu nhận diện khuôn mặt, phát hiện biểu cảm, nhận diện chữ viết OCR và phân tích video.

7、[docz](https://www.docz.site/)

Công cụ hỗ trợ tạo tài liệu hướng dẫn kỹ thuật chuyên nghiệp viết bằng MDX (Markdown kết hợp component React) giúp hiển thị trực quan demo code chạy thực tế.

## 文摘 (Văn trích)

1、[Tại sao nền nông nghiệp Trung Hoa cổ đại lại phát triển vượt bậc so với Tây Âu?](https://cdn.beekka.com/blogimg/asset/201806/bg2018062919.jpg)

Cuốn sách *Lịch sử thế giới* của L.S. Stavrianos lý giải sự vượt trội về sản lượng nông nghiệp và mật độ dân số của Trung Quốc cổ đại so với châu Âu nhờ yếu tố địa lý và khí hậu: Gió mùa mang lại lượng mưa dồi dào vào mùa hè tạo điều kiện canh tác nông nghiệp thuận lợi (canh tác 2 vụ/năm ở vĩ độ thấp), kết hợp loại cây trồng chủ đạo là lúa nước có hàm lượng calo trên đơn vị diện tích đất cao gấp 5 lần so với lúa mì, lúa mạch của châu Âu. Ưu thế về sản lượng lương thực và dân số đông giúp các triều đại Trung Quốc duy trì tốt bộ máy quan lại và quân đội hùng mạnh để bảo vệ và đồng hóa các bộ tộc xâm lược ngoài biên ải, cho đến trước khi cuộc cách mạng công nghiệp nổ ra giúp Tây Âu vượt lên nhờ khoa học kỹ thuật.

2、[Sự dịch chuyển từ giới công nghệ sang cộng đồng cuồng tín của Bitcoin](https://adamcaudill.com/2018/06/21/bitcoin-is-a-cult/)

Nhà nghiên cứu bảo mật nhận định cộng đồng Bitcoin đang dịch chuyển từ nhóm kỹ sư công nghệ ban đầu hiểu rõ bản chất toán học sang nhóm đầu cơ tài chính ngắn hạn, và hiện tại là một nhóm người cuồng tín mất đi góc nhìn khách quan, tin tưởng cực đoan rằng hệ thống tiền tệ truyền thống USD/Euro sắp sụp đổ hoàn toàn để nhường chỗ cho tiền mã hóa thống trị thế giới.

## 本周图片 (Hình ảnh tuần này)

1、[Hình ảnh cuộc sống thường nhật tại Nam Cương](http://news.migage.com/articles/%E6%88%91%E5%9C%A8%E5%8D%97%E7%96%86%E7%9A%8410%E5%A4%A9_1161211_9.html#p=1)

![](https://cdn.beekka.com/blogimg/asset/201806/bg2018062920.jpg)

Hình ảnh ghi lại khoảnh khắc ấm áp của một gia đình người Duy Ngô Nhĩ vui chơi tại công viên nhân dân thành phố Kashgar trong chuyến du hành 10 ngày khám phá nét đẹp văn hóa và cảnh quan thiên nhiên vùng đất Nam Cương.

2、[Lịch sử thâu tóm các công ty công nghệ lớn của Microsoft](https://twitter.com/netlookers/status/1004284958167486464)

![](https://cdn.beekka.com/blogimg/asset/201806/bg2018062921.jpg)

Hình ảnh trào phúng mô tả chuỗi thâu tóm đình đám của Microsoft gồm Nokia, LinkedIn, Skype, Minecraft, GitHub và đặt dấu hỏi về mục tiêu tiếp theo.

3、[Sự khác biệt trong thiết kế biểu tượng vịt Emoji của các hãng công nghệ](https://emojiratings.tumblr.com/post/173579088393/duck-emoji-rates)

![](https://cdn.beekka.com/blogimg/asset/201806/bg2018062922.jpg)

Hình ảnh so sánh thiết kế hình vẽ chú vịt Emoji giữa Apple, Google, Samsung, Twitter... Đặt ra câu hỏi thú vị tại sao ngoại trừ Google vẽ chú vịt màu vàng, các hãng công nghệ khác đều vẽ chú vịt cổ xanh (vịt uyên ương).

## 本周金句 (Kim ngôn tuần này)

1、

> "Tại sao các startup khởi nghiệp thành công? Đây là câu hỏi khó nhất. Phần lớn mọi người chỉ đưa ra những lý do hiển nhiên như: nhà sáng lập tài giỏi chăm chỉ, văn hóa công ty xuất sắc. Vấn đề là 5.000 startup thất bại khác ngoài kia thực tế cũng sở hữu những điều tương tự."
> 
> -- Trích bài viết *Thiên kiến kẻ sống sót* (Survivorship Bias)

2、

> "Tôi luôn yêu thích những thị trấn nhỏ có quy mô thế này: Vừa đủ lớn để xây dựng một rạp chiếu phim và một hiệu sách, nhưng cũng vừa đủ nhỏ để mang lại cảm giác thân thiện ấm áp, thích hợp để sinh sống lâu dài."
> 
> -- Bill Bryson

(Hết)
