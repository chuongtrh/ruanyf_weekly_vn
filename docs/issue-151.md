# 科技爱好者周刊（第 151 期）：NFT 是什么，听说能赚钱

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1652) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032509.jpg)

Một thương hiệu thiết kế nội thất tại Ý đã cho ra mắt dòng sản phẩm ghế sofa độc đáo được khoác tất và mang giày da ở bốn chân ghế. Thật kỳ lạ, chỉ bằng cách bổ sung thêm chi tiết giày tất đơn giản này, chiếc ghế trông như có hồn và sinh động hẳn lên. (Nguồn: [Instagram](https://www.instagram.com/p/CLWmhSpl5Rq/))

## 主带话题：NFT là gì, nghe nói kiếm được nhiều tiền lắm?

Gần đây, tại Mỹ và trên toàn cầu có một khái niệm cực kỳ sốt dẻo mang tên NFT (Non-Fungible Token), với mức giá giao dịch tăng vọt tới mức khó tin.

Hãy điểm qua một tin tức chấn động gần đây: Một nghệ sĩ kỹ thuật số có nghệ danh Beeple đã kiên trì thực hiện dự án đăng tải một bức vẽ đồ họa mỗi ngày lên Instagram liên tục từ ngày 1 tháng 5 năm 2007.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032311.jpg)

Đến năm nay, anh đã hoàn thành chặng đường liên tục 5.000 ngày. Để kỷ niệm cột mốc này, anh đã ghép toàn bộ 5.000 bức vẽ nhỏ đó thành một file ảnh siêu lớn định dạng JPG và gửi cho nhà đấu giá danh tiếng Christie's để tổ chức đấu giá trực tuyến.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032312.jpg)

**Câu hỏi đặt ra là: Làm sao có thể đấu giá một file ảnh JPG?** Đó suy cho cùng chỉ là một chuỗi các mã nhị phân. Nếu có ai đó copy lưu lại file ảnh đó về máy, thì đâu là bản gốc chính chủ và đâu là bản sao chép?

Giải pháp của Beeple là: Thứ được đem ra đấu giá không phải là bản thân file ảnh JPG đó, mà chính là token NFT đại diện cho tác phẩm nghệ thuật này. Kết quả thật kinh ngạc, tác phẩm đã được gõ búa chốt hạ với mức giá không tưởng: **69,34 triệu USD**!

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032313.jpg)

NFT rốt cuộc là cái gì mà lại có thể khiến một file ảnh kỹ thuật số có giá trị khổng lồ đến như vậy? Để thỏa mãn trí tò mò, tôi đã đọc nhiều tài liệu nghiên cứu và xin tóm lược lại cách hiểu của mình dưới đây.

**Nói một cách đơn giản nhất: NFT là một ứng dụng của công nghệ blockchain, với đặc tính cốt lõi là ghi nhận một liên kết URL cố định vào bên trong sổ cái blockchain.** Như bạn đã biết, một khi dữ liệu đã được ghi vào blockchain thì hoàn toàn không thể sửa đổi hay xóa bỏ. Do đó, liên kết URL chứa trong NFT là cố định vĩnh viễn, và thông qua cơ chế giao dịch của blockchain, liên kết này sẽ được gắn chặt với địa chỉ một ví tiền mã hóa cụ thể của chủ sở hữu.

Điều này đồng nghĩa với việc nếu khối block đó thuộc về ví của bạn, bạn sẽ có quyền sở hữu hợp pháp đối với liên kết URL chứa trong khối đó. Vì thế, **NFT cực kỳ phù hợp để đóng vai trò như một chứng nhận quyền sở hữu đối với các liên kết số.** Quay lại ví dụ trên, thứ mà nhà đấu giá Christie's bán cho người mua thực chất là quyền sở hữu được ghi nhận trên blockchain của liên kết dẫn tới file ảnh JPG gốc kia.

Người mua chốt được đấu giá sẽ nhận lại một khối block chứa địa chỉ liên kết đó, bản chất là một dòng bản ghi dữ liệu trên blockchain để chứng minh mình sở hữu "bản gốc duy nhất". **Bất kỳ thứ gì có thể đại diện bằng một đường link URL (một bài báo, một đoạn video, một dòng tweet...) đều có thể được mã hóa thành NFT để giao dịch.** Đó là lý do nhiều người kỳ vọng NFT sẽ là giải pháp tối ưu cho việc mua bán quyền sở hữu tài sản số.

Tuy nhiên, có một kịch bản rủi ro hiển nhiên: Nếu liên kết URL đó bị thay đổi nội dung, tên miền hết hạn hoặc máy chủ chứa file bị sập ngoại tuyến thì sao? Khi đó mã NFT ghi trên blockchain vẫn tồn tại nhưng liên kết bên trong đã trỏ vào hư vô và không thể sửa lại được. Theo các tài liệu hiện tại, mâu thuẫn này vẫn chưa có giải pháp kỹ thuật triệt để (một số người đề xuất giải pháp trỏ link qua mạng lưu trữ phân tán IPFS).

Nếu bạn hỏi tôi NFT có giá trị đầu tư thực sự hay không, hay chỉ là một bong bóng đầu cơ như Bitcoin? Quan điểm của tôi là giá trị của nó phụ thuộc hoàn toàn vào quy mô thực tế của thị trường giao dịch quyền sở hữu tài sản số. Bản chất của file số là khả năng sao chép vô hạn một cách dễ dàng, và NFT cố gắng tạo ra một sự khan hiếm nhân tạo bằng cách gán chứng nhận sở hữu để phân biệt giữa bản sao và bản gốc. Ngoài mục đích đấu giá nghệ thuật hoặc đầu cơ thổi giá, tôi thực sự chưa nghĩ ra được kịch bản ứng dụng thực tế nào khác tốt hơn các giải pháp quản lý truyền thống.

## Khóa học phân tích nguyên lý Vue 3

Vào tháng 9 năm 2020, Vue.js chính thức phát hành phiên bản 3.0 với việc viết lại mã nguồn tối ưu hóa hiệu năng và cung cấp Composition API. Các dự án Front-end hiện nay tại các doanh nghiệp đã dần chuyển dịch sang phiên bản mới này và đây trở thành chủ đề phỏng vấn bắt buộc tại các tập đoàn lớn.

Để chuẩn bị tốt cho các đợt phỏng vấn và chứng minh năng lực tự học công nghệ mới, việc nắm vững bản chất nguyên lý hoạt động của Vue 3 là cực kỳ quan trọng đối với các kỹ sư Front-end.

Tuần này, chúng tôi giới thiệu khóa học **《Vue 3 Principle Analysis》** hỗ trợ bạn tiếp cận mảng kiến thức này:

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032517.jpg)

Giảng viên của khóa học là thầy **Thôi Hiệu Thụy** - một nhà phát triển đóng góp mã nguồn (code contributor) trực tiếp cho dự án Vue 3. Khóa học sẽ hướng dẫn học viên các bước rà soát mã nguồn lõi của Vue 3, cách thức hoạt động của hệ thống phản ứng (reactivity) và tự tay code một phiên bản nhân Vue 3 tối giản từ số không.

Khóa học trị giá 199 tệ hiện được mở **miễn phí** dành riêng cho độc giả bản tin. Bạn có thể quét mã QR dưới đây để đăng ký tham gia:

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032516.jpg)

Đặc biệt, 100 học viên đăng ký sớm nhất sẽ được tặng thêm bộ bài giảng chuyên đề nâng cao về ngôn ngữ ES6.

## 科技动态

1、[Tính năng tự động phát hiện tai nạn giao thông trên Android cứu mạng tài xế Mỹ](https://www.reddit.com/r/GooglePixel/comments/lq3k0a/car_crash_detection_saved_me_hours_of_suffering/)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030801.jpg)

Một tài xế vận hành máy xúc tại Mỹ trong khi làm việc tại khu vực đồi núi hẻo lánh đã gặp tai nạn nghiêm trọng khiến chiếc máy xúc bị lật nhào rơi xuống thung lũng sâu. Người lái bị mắc kẹt cứng trong cabin biến dạng, chấn thương lồng ngực gây khó thở và xung quanh hoàn toàn không có người qua lại.

Rất may mắn, chiếc điện thoại Google Pixel chạy hệ điều hành Android 10 của anh có kích hoạt tính năng tự động phát hiện tai nạn giao thông. Cảm biến gia tốc trên máy đã nhận diện lực va đập cực mạnh và tự động gọi điện đến đầu số khẩn cấp 911 sau vài phút không thấy phản hồi từ người dùng, đồng thời gửi trực tiếp tọa độ định vị GPS cho cơ quan chức năng. Đội cứu hỏa đã tiếp cận hiện trường giải cứu anh kịp thời sau đó ít phút với chấn thương gãy 7 xương sườn và 4 đốt sống ngực.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030802.jpg)

2、[Mẫu cabin du lịch tự cấp sinh thái tuần hoàn độc lập](https://www.163.com/dy/article/FV151NN2051492T3.html)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032505.jpg)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032506.jpg)

Một doanh nghiệp Trung Quốc vừa ra mắt mẫu cabin di động sinh thái hướng tới nhu cầu cắm trại dã ngoại ở các vùng hoang dã. Cabin có thiết kế hình kén khép kín, trang bị bình chứa nước sạch dung tích từ 800 đến 1.600 lít, tấm pin mặt trời công suất 5 kW trên mái và hệ thống xử lý nước thải sinh hoạt khép kín tự tuần hoàn độc lập.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032507.jpg)

Nhà sản xuất cho biết cabin sử dụng vật liệu composite sợi thủy tinh siêu bền nhẹ và chống ăn mòn tốt, cho phép lắp đặt nhanh chóng tại nhiều địa hình phức tạp mà không cần làm móng hay xây dựng bể tự hoại. Tuy nhiên trong điều kiện vận hành thương mại lâu dài, cabin vẫn cần kết nối với hệ thống điện nước cơ sở.

3、[Sono Motors ra mắt mẫu ô tô điện chạy bằng năng lượng mặt trời](https://sonomotors.com/)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031608.jpg)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031609.jpg)

Một startup công nghệ của Đức công bố đã chế tạo thành công mẫu ô tô điện Sion thương mại đầu tiên hoạt động nhờ năng lượng mặt trời tích hợp. Toàn bộ vỏ xe và nắp capo được phủ kín bởi 248 tấm pin mặt trời thay thế cho lớp sơn ngoại thất thông thường.

Do hiệu suất chuyển đổi của pin mặt trời có giới hạn, năng lượng thu được từ ánh sáng tự nhiên hàng tuần chỉ đủ cung cấp cho xe di chuyển quãng đường từ 112 km đến 245 km tùy thuộc vào điều kiện thời tiết, phần năng lượng còn lại vẫn phải sạc qua các trụ sạc điện thông thường. Mẫu xe có tầm hoạt động 250 km cho mỗi lần sạc đầy pin và có mức giá bán khoảng 25.000 Euro.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031611.jpg)

4、[Công bố các phát hiện khảo cổ học mới chấn động tại di chỉ Tam Tinh Đôi](https://weibo.com/6755715468/K754l8FUu)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032011.jpg)

Vào ngày 20 tháng 3, Cục Di sản Văn hóa Trung Quốc đã công bố các phát hiện khảo cổ học mới tại di chỉ văn hóa Tam Tinh Đôi (Tứ Xuyên). Đợt khai quật quy mô lớn trước đó diễn ra từ những năm 1980 mới chỉ khai quật được 2 hố tế thần lớn. Từ năm 2019 đến nay, các nhà khảo cổ đã tiến hành mở thêm 6 hố tế thần mới, phát hiện được mặt nạ vàng ròng nguyên khối cực kỳ tinh xảo và nhiều hiện vật bằng đồng có hình dáng độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032012.jpg)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032206.jpg)

Quy trình khảo cổ hiện đại ứng dụng nhiều trang thiết bị công nghệ cao: xây dựng nhà kính kiểm soát nhiệt độ ẩm trực tiếp trên hố đào, sử dụng cánh tay robot và công nghệ quét 3D để tạo vỏ bảo vệ cho các hiện vật dễ vỡ khi đưa lên mặt đất. Nguồn gốc của nền văn minh cổ phát triển rực rỡ cách đây 4.000 năm này hiện vẫn là một bí ẩn lớn do không có bất kỳ thư tịch cổ nào ghi nhận.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032013.jpg)

5、**Tin tức một câu**

> - Tuyến đường hàng hải huyết mạch qua Kênh đào Suez lần đầu tiên trong lịch sử bị tê liệt hoàn toàn do siêu tàu container Ever Given dài 400 mét bị gió lớn thổi xoay ngang mắc cạn vào bờ kênh (vốn chỉ rộng 200 mét), khiến hàng trăm tàu chở hàng ùn tắc nghiêm trọng ở cả hai đầu運河.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032401.jpg)

> - Báo cáo của BBC chỉ ra ngày càng có nhiều tập đoàn lớn tại Âu Mỹ ứng dụng hệ thống trí tuệ nhân tạo (AI) để phỏng vấn và sàng lọc hồ sơ ứng viên thông qua việc yêu cầu ứng viên chơi trò chơi test tư duy hoặc trả lời câu hỏi trước camera để AI phân tích nét mặt, dấy lên tranh cãi lớn về tính công bằng của thuật toán tuyển dụng.

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021020911.jpg)

> - Các nhà khoa học Mỹ công bố thực hiện thành công ca nhân bản vô tính đầu tiên một cá thể chồn chân đen (loài động vật đang đứng trước nguy cơ tuyệt chủng cao tại Bắc Mỹ) sử dụng mẫu tế bào DNA lưu giữ đông lạnh từ năm 1988 và mang thai hộ bởi chồn nhà thông thường.

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021022201.jpg)

> - Dòng điện thoại cao cấp Oppo Find X3 Pro gây chú ý với truyền thông công nghệ khi trang bị camera hiển thị kính hiển vi native hỗ trợ độ phóng đại lên tới 60x, cho phép chụp rõ nét các cấu trúc sợi vải dệt và tế bào rêu nhỏ:

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031203.jpg)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031204.jpg)

> - Nhà sản xuất bộ phim truyền hình Hàn Quốc *Vincenzo* tiết lộ toàn bộ các phân cảnh hoành tráng diễn ra tại Ý trong phim thực chất đều được thực hiện hoàn toàn trong studio phông xanh trong nước và dựng cảnh nền 3D bằng đồ họa máy tính, cho thấy trình độ kỹ xảo hình ảnh rất ấn tượng.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031706.jpg)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031708.jpg)

## 文章

1、[Tại sao Ấn Độ gặp khó khăn khi phát triển công nghiệp sản xuất chế tạo?](https://www.guancha.cn/moxizhi/2021_02_20_581655.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031709.jpg)

Bài viết phân tích sâu các rào cản về hạ tầng giao thông nghèo nàn, luật đất đai phức tạp, trình độ học vấn của người lao động và sự thiếu hụt các chuỗi cung ứng công nghiệp phụ trợ khiến Ấn Độ chưa thể sao chép thành công mô hình công xưởng thế giới của Trung Quốc. (Ảnh trên là cảnh một giáo viên Ấn Độ dạy học online tự chế giá đỡ điện thoại từ ghế gỗ).

2、[Bí ẩn thương vụ Baidu suýt chiêu mộ được cha đẻ Deep Learning Geoffrey Hinton](https://posts.careerengine.us/p/605412f82e61cf72e86dc02c)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032103.jpg)

Cuốn sách mới xuất bản *Genius Makers* tiết lộ nhiều bí mật hậu trường công nghệ: Vào năm 2012, CEO Baidu Lý Ngạn Hoành đã quyết định ra giá 12 triệu USD để chiêu mộ giáo sư Geoffrey Hinton (người sau này đoạt giải Turing cho Deep Learning) cùng nhóm nghiên cứu của ông, nhưng cuối cùng Google đã nhanh chân nâng giá để đưa ông về thung lũng Silicon.

3、[Vấn đề bảo mật dữ liệu sau sự cố LINE thuê ngoài kỹ sư Trung Quốc](https://mp.weixin.qq.com/s/w6lKuPMwgtGstu978iBU8Q)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032207.jpg)

Tranh cãi nổ ra tại Nhật Bản khi truyền thông khui ra việc ứng dụng nhắn tin quốc dân LINE đã thuê ngoài một số module phát triển phần mềm cho doanh nghiệp Trung Quốc, cho phép các kỹ sư Trung Quốc truy cập hợp pháp vào hệ thống cơ sở dữ liệu chứa tin nhắn và thông tin cá nhân của người dùng Nhật Bản để bảo trì hệ thống.

4、[Kinh nghiệm thực tế của một nhà đầu tư khi mua lại doanh nghiệp SaaS](https://every.to/superorganizers/how-i-bought-a-business-for-0)（Tiếng Anh）

Một nhà đầu tư mạo hiểm chia sẻ chi tiết quy trình tìm kiếm, đàm phán giá trị định giá và các bước vận hành kỹ thuật khi mua lại một phần mềm dịch vụ đám mây (SaaS) quy mô nhỏ đang hoạt động hiệu quả.

5、[Tôi đã kiếm tiền từ việc đăng ký hàng loạt tên miền chứa biểu tượng Emoji như thế nào](https://tinyprojects.dev/projects/mailoji)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031106.jpg)

Tác giả chia sẻ trải nghiệm thú vị khi phát hiện một số nhà đăng ký tên miền quốc gia cho phép đăng ký tên miền chứa ký tự Emoji (như biểu tượng mặt cười). Anh đã đăng ký nhanh hơn 300 tên miền Emoji đẹp và thiết kế dịch vụ email theo tên miền này để thu phí.

6、[Khái niệm cơ bản về lập trình đa luồng (multithreading)](https://www.internalpointers.com/post/gentle-introduction-multithreading)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031105.jpg)

Bài viết nhập môn ngắn gọn và dễ hiểu giải thích cơ chế hoạt động của Thread, sự khác biệt bản chất so với Process, cách thức chia sẻ tài nguyên bộ nhớ và các lỗi deadlock thường gặp.

7、[Bài toán vật lý: Có thể đặt cuộn dây dưới đường dây cao thế để cảm ứng "trộm" điện?](https://users.physics.unc.edu/~deardorf/phys25/rwp/exam1rwpsolution.html)（Tiếng Anh）

Lời giải chi tiết cho một bài toán kiểm tra vật lý đại học phân tích tính khả thi về mặt kỹ thuật, lượng điện năng thu được và các rủi ro pháp lý nếu cố tình đặt cuộn dây đồng lớn dưới hành lang lưới điện cao thế để thu dòng điện cảm ứng điện từ.

8、[Tại sao các website nên loại bỏ menu hiển thị dạng hover di chuột](https://css-tricks.com/in-praise-of-the-unambiguous-click-menu/)（Tiếng Anh）

Tác giả đưa ra các lập luận UI/UX chứng minh việc sử dụng menu dạng hover dễ gây thao tác nhầm trên thiết bị di động cảm ứng, đề xuất chuyển đổi hoàn toàn sang menu kích hoạt dạng click rõ ràng.

## 工具

1、[Gotify](https://gotify.net/)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031001.jpg)

Một máy chủ thông báo tin nhắn tự động (push notification) viết bằng Go sử dụng giao thức WebSockets hỗ trợ lập trình viên tự xây dựng kênh thông báo riêng có ứng dụng Android đi kèm.

2、[UserLAnd](https://github.com/CypherpunkArmory/UserLAnd)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031002.jpg)

Ứng dụng Android mã nguồn mở hỗ trợ người dùng thiết lập và chạy các bản phân phối Linux (Ubuntu, Debian) ngay trên điện thoại di động dưới dạng một ứng dụng thông thường mà không cần root máy.

3、[lint-md](https://github.com/lint-md)

Công cụ dòng lệnh CLI đắc lực giúp rà soát lỗi trình bày văn bản tiếng Trung trong các file Markdown (như bắt buộc chèn khoảng trắng giữa ký tự alphabet và ký tự chữ Hán toàn góc).

4、[FairEmail](https://email.faircode.eu/)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030901.jpg)

Ứng dụng đọc email khách (email client) mã nguồn mở dành cho hệ điều hành Android, được đánh giá cao nhờ cơ chế bảo mật tối đa và bảo vệ quyền riêng tư người dùng.

5、[AR-lab: Công cụ sao chép vật thể AR từ điện thoại lên PC](https://github.com/shadowcz007/AR-lab)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032203.jpg)

Một ứng dụng máy tính thử nghiệm kết hợp framework Electron và mô hình AI PaddlePaddle: Người dùng chỉ cần chĩa camera điện thoại quét chụp một vật thể/người ngoài đời thực, AI sẽ tự động tách nền và dán (paste) trực tiếp hình ảnh đó vào màn hình PC theo thời gian thực. ([@shadowcz007](https://github.com/ruanyf/weekly/issues/1680) đóng góp)

6、[rss_everyday](https://github.com/GuangzheJiang/rss_everyday)

Template cấu hình GitHub Actions giúp thiết lập quy trình tự động cào tin tức từ các nguồn RSS định sẵn và tự động gửi thông báo tổng hợp hàng ngày vào kênh Telegram của bạn. ([@GuangzheJiang](https://github.com/ruanyf/weekly/issues/1682) đóng góp)

7、[mdBook](https://github.com/rust-lang/mdBook)

Một công cụ viết bằng Rust hỗ trợ build các thư mục chứa tệp tin Markdown thành một website đọc sách trực tuyến với giao diện gọn đẹp tương tự như GitBook.

8、[flowchart-fun](https://github.com/tone-row/flowchart-fun)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030201.jpg)

Công cụ thiết kế sơ đồ tư duy và flowchart tối giản nhất: Người dùng chỉ cần nhập dữ liệu dạng text thụt dòng ở khung bên trái, hệ thống sẽ tự động vẽ sơ đồ phân cấp tương ứng ở khung bên phải ngay lập tức.

9、[DarkModeBuddy](https://github.com/insidegui/DarkModeBuddy)

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021022703.jpg)

Ứng dụng macOS nhỏ gọn tự động chuyển đổi giao diện hệ điều hành giữa Light Mode và Dark Mode dựa trên việc đo đạc cường độ ánh sáng môi trường thu được từ cảm biến camera của máy.

10、[Arrow](https://github.com/arrow-py/arrow)

Thư viện xử lý múi giờ và ngày tháng chuyên nghiệp dành cho Python, sở hữu thiết kế API thân thiện dễ sử dụng tương tự như thư viện moment.js của JavaScript.

## Tài nguyên

1、[Clone Wars: Kho dự án clone các website nổi tiếng](https://github.com/GorvGoyl/Clone-Wars)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031003.jpg)

Bộ sưu tập tổng hợp hơn 70 dự án mã nguồn mở tái hiện lại giao diện và tính năng cơ bản của các nền tảng web lớn (Airbnb, Netflix, Spotify, TikTok...) giúp lập trình viên học tập kiến trúc Front-end.

2、[Kênh video khoa học History of the Earth](https://www.youtube.com/c/HistoryoftheEarth/videos)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030805.jpg)

Kênh YouTube chuyên sản xuất các video đồ họa khoa học mô tả chi tiết lịch sử hình thành cấu trúc địa chất và tiến hóa sinh vật trên Trái Đất từ thuở sơ khai.

3、[Real-world Cryptography: Sách giáo khoa mật mã học ứng dụng](https://www.manning.com/books/real-world-cryptography)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030803.jpg)

Cuốn sách chuyên ngành giải thích chi tiết các nguyên lý và ứng dụng thực tế của mật mã học bảo mật thông tin trong đời sống hàng ngày, hỗ trợ đọc trực tuyến miễn phí.

4、[Bộ video bài giảng Cấu trúc dữ liệu và Giải thuật trên Bilibili](https://space.bilibili.com/50003725/video)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032205.jpg)

Tuyển tập các video hoạt họa mô phỏng hoạt động của các thuật toán đồ thị, cây nhị phân, cấu trúc mảng động được dịch phụ đề tiếng Trung chia sẻ trên Bilibili. ([@jizai](https://github.com/ruanyf/weekly/issues/1685) đóng góp)

5、[Live feed núi lửa đang hoạt động tại Iceland](https://www.ruv.is/frett/2021/03/20/live-feed-from-iceland-volcano)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032107.jpg)

Kênh truyền hình Iceland thiết lập camera giám sát túc trực truyền hình trực tiếp 24/7 cảnh tượng dòng dung nham nóng đỏ phun trào từ vết nứt của một ngọn núi lửa đang hoạt động tại địa phương.

## 图片

1、[Bảng phối màu sản phẩm Braun thời Dieter Rams](http://blog.presentandcorrect.com/rams-palettes)

Hãng điện gia dụng Braun của Đức nổi tiếng lịch sử thiết kế với triết lý tối giản của Dieter Rams (nguồn cảm hứng lớn cho thiết kế phần cứng của Apple). Dưới đây là các bảng phối màu nút bấm và vỏ thiết bị cực kỳ tinh tế của hãng:

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030301.jpg)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030302.jpg)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030303.jpg)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030304.jpg)

2、[Cuốn sổ tay Little Red Book của Facebook năm 2012](https://twitter.com/antoniogm/status/1365795467376824320)

Vào năm 2012 khi Facebook tiến hành IPO niêm yết cổ phiếu, mỗi nhân viên công ty đã được phát một cuốn sổ tay nhỏ màu đỏ chứa đựng các châm ngôn hoạt động của hãng.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030311.jpg)

Trang cuối cùng của cuốn sổ tay in dòng chữ cảnh báo đầy ấn tượng:

> *"Nếu chính chúng ta không tự mình tạo ra sản phẩm thay thế tiêu diệt Facebook, đối thủ khác sớm muộn sẽ làm việc đó. ... Mạng Internet không phải là một nơi yên bình để dung dưỡng sự chậm trễ. Những thứ không còn giá trị sẽ nhanh chóng bị đào thải mà không để lại bất kỳ dấu tích lịch sử nào. Chúng sẽ biến mất hoàn toàn."*

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030312.jpg)

## Bài đọc thêm

### 1. Hành trình vượt đại dương trên phao cứu sinh của Alain Bombard

*Tóm tắt câu chuyện sinh tồn phi thường của bác sĩ người Pháp Alain Bombard vào năm 1952:*

Để chứng minh luận điểm khoa học của mình rằng con người khi gặp nạn trên biển hoàn toàn có thể sinh tồn dài ngày bằng việc tận dụng nguồn thức ăn nước uống tự nhiên mà không bị chết khát, bác sĩ Alain Bombard đã thực hiện chuyến hành trình mạo hiểm vượt Đại Tây Dương một mình trên một chiếc phao cứu sinh cao su nhỏ dài 4.3 mét.

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021022305.jpg)

Bắt đầu chuyến đi từ năm 1952 hoàn toàn không mang theo lương thực và nước ngọt dự trữ, ông đã di chuyển chặng đường dài 4.400 km và cập bờ đảo quốc Barbados an toàn vào ngày 23 tháng 12 cùng năm với cơ thể bị sụt mất 25 kg.

![](https://cdn.beekka.com/blogimg/asset/202102/bg2021022306.jpg)

Theo lý thuyết y khoa của Bombard, cơ thể người nếu chưa bị rơi vào trạng thái mất nước nghiêm trọng (dehydration) có thể hấp thụ một lượng nhỏ nước biển hàng ngày mà không gây nguy hiểm cho thận, trái ngược với việc uống nhiều nước biển khi cơ thể đã kiệt quệ. Trong chuyến đi, ông tự săn cá bằng lao tự chế và dùng lưới nhỏ vớt các sinh vật phù du trên mặt nước để cung cấp vitamin chống bệnh scurvy. Mặc dù gặp nhiều hoài nghi về việc ông có thể âm thầm thu gom nước mưa dọc đường, chuyến đi của ông vẫn là một biểu tượng lớn của lòng quả cảm chứng minh giới hạn sinh tồn của con người.

### 2. Sự cố thất lạc thiết bị nghe lén hạt nhân của CIA trên dãy Himalaya

Năm 1964, sau khi Trung Quốc thực hiện thử nghiệm thành công quả bom nguyên tử đầu tiên tại Tân Cương, chính phủ Mỹ đã vô cùng lo ngại và tìm mọi cách thu thập thông tin tình báo về chương trình hạt nhân này.

Cơ quan tình báo CIA đã lập ra một kế hoạch do thám táo bạo: Triển khai một trạm thu phát tín hiệu nghe lén đặt trên đỉnh núi cao thuộc dãy Himalaya giáp biên giới để thu nhận các luồng sóng vô tuyến liên lạc của Trung Quốc. Thiết bị nghe lén là một hộp kim loại nặng hơn 50 kg có cột anten dài 2 mét, hoạt động nhờ nguồn năng lượng phát ra từ một máy phát điện hạt nhân mini tích hợp bên trong để đảm bảo hoạt động liên tục nhiều năm giữa đỉnh núi lạnh giá.

Năm 1965, CIA phối hợp cùng quân đội Ấn Độ thành lập một đoàn leo núi chuyên nghiệp để vận chuyển thiết bị này lên đỉnh núi Nanda Devi cao 7.816 mét thuộc dãy Himalaya.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030203.jpg)

Tuy nhiên khi đoàn leo núi chỉ còn cách đỉnh vài trăm mét, một trận bão tuyết khủng khiếp bất ngờ đổ ập xuống khiến nhiều thành viên thiệt mạng. Trưởng đoàn buộc phải ra lệnh rút lui khẩn cấp và quyết định chốt chặt thiết bị nghe lén hạt nhân vào vách đá ven đường để quay lại thu hồi sau.

Đến mùa xuân năm sau khi quay lại hiện trường, đoàn leo núi kinh ngạc phát hiện toàn bộ mảng đá chứa thiết bị nghe lén hạt nhân đã bị lở tuyết cuốn trôi mất tích hoàn toàn. CIA sau đó đã tổ chức thêm 7 đợt tìm kiếm quy mô lớn dọc các khe nứt băng trôi bên dưới suốt nhiều năm nhưng hoàn toàn không tìm lại được khối phóng xạ này. Khối hạt nhân Plutonium mất tích hiện vẫn đang nằm sâu đâu đó dưới lớp băng tuyết của dãy Himalaya đe dọa ô nhiễm nguồn nước sông Hằng nếu bị rò rỉ.

## 言论

1、

Gần như 1/4 tổng số lượng đồng USD đang lưu hành trên thị trường tài chính thế giới hiện nay được in ra và bơm vào nền kinh tế trong riêng năm 2020.

-- Trích bài viết về sự mất giá của đồng USD

2、

Những cải tiến nhỏ mang tính lũy tiến (incremental innovation) chỉ giúp các doanh nghiệp đang dẫn đầu thị trường duy trì vị thế sẵn có của mình. Nhưng chính những cải tiến mang tính đột phá (radical innovation) mới là đòn bẩy giúp các doanh nghiệp khởi nghiệp non trẻ thực hiện các bước đi "nhảy vọt" (leapfrogging) để vượt qua gã khổng lồ dẫn đầu.

-- Định nghĩa trên Wikipedia

3、

Thuật ngữ "Ứng dụng sát thủ" (killer application) dùng để mô tả một chương trình phần mềm cực kỳ thành công và phổ biến trên thị trường đến mức người tiêu dùng sẵn sàng bỏ tiền mua sắm các thiết bị phần cứng đắt đỏ chỉ để có cơ hội chạy phần mềm đó (ví dụ game hot đẩy doanh số bán console).

-- Định nghĩa trên Wikipedia

4、

Nếu bạn tự mình thành lập và vận hành một doanh nghiệp phần mềm nhưng doanh thu hàng tháng thu về dưới mốc 20.000 USD, thì thực chất đó chưa phải là một doanh nghiệp đúng nghĩa, mà chỉ là bạn đang tự tạo ra một công việc làm thuê cho chính mình.

-- Trích bài viết về khởi nghiệp SaaS

## 历史上的本周

- 2020年（第 100 期）：[Kỷ nguyên lãi suất bằng không](http://www.ruanyifeng.com/blog/2020/03/weekly-issue-100.html)
- 2019年（第 48 期）：[Những bài học cuộc đời từ nhà lập trình huyền thoại Bill Joy](http://www.ruanyifeng.com/blog/2019/03/weekly-issue-48.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
