# Bản tin chia sẻ công nghệ (Số 339): Token là gì

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/6189) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022708.webp)

Bên trong nhà ga hành khách T5 mới khánh thành của Sân bay Quốc tế Hàm Dương Tây An có thiết kế một khu vực bảo tàng đặc biệt để trưng bày các cổ vật lịch sử được khai quật ngay trong quá trình thi công xây dựng sân bay. (Nguồn: [chinadaily.com.cn](https://cn.chinadaily.com.cn/a/202502/27/WS67c024ffa310510f19ee8fab.html))

## 代币是什么

Hiện nay trên các phương tiện truyền thông xuất hiện rất nhiều thuật ngữ "Token" (thường được dịch là tiền mã hóa/token). Hôm nay chúng ta hãy cùng thảo luận sâu hơn xem khái niệm này thực chất đại diện cho điều gì?

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022304.webp)

Đầu tiên cần khẳng định rằng tiền mã hóa (crypto tokens) thuộc mảng tài sản mã hóa và có thị trường giao dịch riêng. Tôi hoàn toàn không muốn đi sâu thảo luận về khía cạnh đầu cơ tài chính, mà chỉ muốn tập trung phân tích về mặt nguyên lý công nghệ phía sau của nó.

Sau khi đọc xong bài viết này, các bạn sẽ hiểu rõ nguyên nhân tại sao chúng lại có thể được phát hành và giao dịch tự do. Dưới góc nhìn thực nghiệm công nghệ, đây là một mô hình vô cùng thú vị.

Tôi muốn thảo luận chủ đề này xuất phát từ việc gần đây có đọc được một bài phân tích rất hay mang tựa đề [《Definancialization and Hyperfinancialization》 (Phi tài chính hóa và Siêu tài chính hóa)](https://mylessnider.com/articles/definancialization-hyperfinancialization), giúp tôi thấu suốt mối liên kết bản chất giữa token và thị trường tài chính.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022507.webp)

Sự ra đời của tiền mã hóa bắt nguồn từ những nhược điểm cố hữu của tiền giấy truyền thống (tiền pháp định). Tiền giấy (ví dụ như đồng USD) luôn có xu hướng được in ra ngày càng nhiều qua thời gian, dẫn đến lạm phát, mất giá dài hạn và làm suy giảm liên tục sức mua thực tế của người dân.

Hệ quả là người ta không còn muốn tích trữ tiền mặt, mà tìm mọi cách để đầu tư giữ giá trị tài sản, **từ đó hình thành nên các hoạt động "tài chính"** như gửi tiết kiệm, đầu tư chứng khoán, mua bất động sản...

Như vậy, tài chính thực chất chính là mặt đối lập của tiền mặt. Tiền tệ được phát hành càng nhiều, người dân càng không muốn giữ tiền mặt, khiến các hoạt động tài chính phái sinh diễn ra ngày một sôi động hơn.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022508.webp)

**Động lực sơ khai của đồng Bitcoin là tạo dựng một cơ chế tiền tệ không thể bị phát hành vô tội vạ**. Do tổng cung Bitcoin được giới hạn cứng từ đầu, việc ứng dụng nó làm tiền tệ giao dịch chắc chắn sẽ loại bỏ hoàn toàn nguy cơ lạm phát mất giá.

Do đó, người dùng sẽ có xu hướng muốn nắm giữ Bitcoin như một dạng tiền mặt lưu trữ tài sản thay vì vội vàng chi tiêu hoặc mang đi đầu tư. Theo suy luận logic này, thế giới tiền mã hóa ban đầu được kỳ vọng sẽ hạn chế tối đa các hoạt động tài chính phức tạp, hướng tới mục tiêu **"phi tài chính hóa"** và thu hẹp quy mô của các hoạt động đầu tư tài chính phái sinh.

Tuy nhiên, một bước ngoặt lịch sử ngoài dự kiến đã xuất hiện khi mạng lưới **Ethereum** ra đời.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022509.webp)

Ethereum có cùng nền tảng công nghệ blockchain tương tự như Bitcoin, với bản chất là một cuốn sổ cái công khai được phân tán rộng khắp và không thể bị sửa đổi sau khi ghi dữ liệu. Tuy nhiên, nó sở hữu một tính năng vô cùng mạnh mẽ mà Bitcoin không có: **Hợp đồng thông minh (Smart Contracts)**. Tính năng này cho phép lập trình viên biên soạn các kịch bản chương trình riêng biệt và tải lên mạng lưới để blockchain tự động thực thi.

Điều này đồng nghĩa với việc **bất kỳ ai cũng có thể tự phát hành các dòng token riêng của mình dựa trên hợp đồng thông minh**. Ví dụ, bạn chỉ cần ghi nhận một thông tin bất kỳ lên sổ cái blockchain, sau đó dùng mã hợp đồng thông minh quy định quyền sở hữu đối với thông tin này được phân chia thành 10.000 phần bằng nhau (tương ứng với 10.000 khóa định danh con), và cho phép chuyển nhượng, giao dịch tự do từng phần một.

Như vậy, bạn đã tự khởi tạo thành công một loại token của riêng mình với tổng cung cố định là 10.000 đơn vị. Chỉ cần có đủ số lượng người dùng tin tưởng và sẵn sàng chi tiền sở hữu, thị trường giao dịch cho dòng token mới của bạn sẽ chính thức được hình thành.

Mấu chốt công nghệ ở đây là phần nội dung gốc bạn ghi nhận lên blockchain có thể là **bất kỳ nội dung nào**. Điều này dẫn tới hệ quả: **Mọi thứ trên đời đều có thể được token hóa (tokenization)**. Từ một dòng ghi chú cá nhân, một tệp ghi âm, cho đến một chiếc áo ngoài đời thực đều có thể được đại diện dưới dạng token, miễn là bạn bảo đảm được mối liên kết logic chứng minh nội dung ghi nhận trên blockchain đại diện chuẩn xác cho tài sản vật lý tương ứng.

Dựa trên nguyên lý vận hành đơn giản này, vô số các loại token với những ý tưởng [vô cùng kỳ lạ](https://zhuanlan.zhihu.com/p/480224017) đã liên tục được phát hành ra thị trường, tiêu biểu như Dogecoin, Catcoin, Mooncoin, Marscoin, Garliccoin... Chúng được gọi chung bằng thuật ngữ **Meme Coins** (tiền mã hóa迷 nhân).

Token có thể được phân loại thành hai dạng: Token đồng nhất (Fungible Token - các đơn vị có giá trị tương đương và có thể thay thế hoàn hảo cho nhau) và Token không đồng nhất (Non-Fungible Token - mỗi đơn vị sở hữu một mã định danh duy nhất, tương tự như một chứng thư số độc nhất vô nhị). Dạng thứ hai chính là công nghệ **NFT** (Non-fungible token) từng tạo nên làn sóng sốt khổng lồ trên thị trường toàn cầu.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022510.webp)

Vào năm 2022, bức ảnh đại diện chú khỉ kỹ thuật số thuộc bộ sưu tập nổi tiếng "[Bored Ape Yacht Club](https://36kr.com/p/1754971959967751)" từng ghi nhận mức giá chuyển nhượng kỷ lục lên tới 147 đồng ETH (tương đương khoảng 420.000 USD tại thời điểm đó). Về bản chất kỹ thuật, khoản tiền khổng lồ bạn chi ra chỉ để đổi lấy quyền sở hữu duy nhất đối với một dòng ghi chú định danh đứng tên bạn trên sổ cái blockchain, đi kèm quyền hạn được chuyển nhượng dòng ghi chú đó cho người khác về sau, hoàn toàn không có thêm bất kỳ giá trị vật lý nào khác.

Bởi lẽ mọi thứ giờ đây đều dễ dàng biến thành một tài sản kỹ thuật số có khả năng giao dịch tự do, công nghệ token vô hình trung đã kiến tạo nên một trạng thái **"Siêu tài chính hóa" (Hyperfinancialization)**, biến mọi khía cạnh sinh hoạt thông thường của con người thành các tài sản tài chính phái sinh để đầu cơ kiếm lời.

Sự phát triển này mang tính châm biếm sâu sắc: Mục tiêu sơ khởi của sự ra đời tiền mã hóa là hướng tới "Phi tài chính hóa" để tạo dựng một đồng tiền có sức mua ổn định, nhưng kết quả thực tế thu về lại là một trạng thái "Siêu tài chính hóa" cực đoan, biến vô số các nội dung vốn không liên quan đến thương mại thành tài sản tài chính để đầu cơ với mức biến động giá vô cùng khủng khiếp.

## GeeLark 云手机

Hiện nay, lượng cá nhân và doanh nghiệp Việt Nam tham gia vào mảng thương mại điện tử xuyên biên giới đang ngày một tăng cao, đòi hỏi nhu cầu lớn về các công cụ quản lý tài khoản mạng xã hội nước ngoài an toàn và hiệu quả.

Hôm nay, tôi xin giới thiệu một giải pháp chuyên dụng hỗ trợ đắc lực cho nhu cầu này mang tên **GeeLark**.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022601.webp)

Sản phẩm được định vị là "Nền tảng vận hành tiếp thị xuyên biên giới một điểm dừng", hỗ trợ hiệu quả cho các thương hiệu Việt Nam vươn ra thị trường quốc tế.

Về mặt công năng, đây là giải pháp **điện thoại đám mây (Cloud Phone), cho phép người dùng điều khiển và vận hành trực tiếp các ứng dụng di động thông qua máy tính** (như TikTok, Instagram, YouTube, Facebook, WhatsApp...) (hình trên).

Phần lớn các nhà bán hàng hiện nay vẫn đang phải duy trì các dàn điện thoại vật lý cồng kềnh để quản lý hàng loạt tài khoản TikTok. Cloud Phone ra đời để giải quyết triệt để sự rườm rà này:

(1) Mỗi thiết bị Cloud Phone hoạt động như một môi trường phần cứng độc lập và biệt lập hoàn toàn. Giao diện và thao tác sử dụng tương tự như thiết bị vật lý thông thường giúp người dùng không mất thời gian làm quen. Hệ thống hỗ trợ đa dạng phiên bản hệ điều hành Android từ phiên bản 10 đến 14.

(2) Quản lý tập trung tiện lợi: Người dùng chỉ cần sử dụng một chiếc máy tính duy nhất để quản lý toàn bộ hệ thống điện thoại ảo và tài khoản tương ứng.

(3) Tự động hóa các tác vụ lặp đi lặp lại: Hỗ trợ tự động đăng tải video hàng loạt, tự động đăng bộ sưu tập ảnh, tự động tối ưu hóa nội dung mô tả, tương tác bình luận tự động bằng AI...

(4) Phân quyền quản trị khoa học: Doanh nghiệp có thể phân quyền truy cập chi tiết cho từng nhân sự theo nhóm công việc. Nhân viên có thể trực tiếp vận hành tài khoản trên Cloud Phone mà hoàn toàn không biết thông tin mật khẩu gốc của tài khoản, giúp bảo đảm an toàn dữ liệu tối đa cho doanh nghiệp.

(5) Tích hợp sâu các tính năng chuyên dụng cho TikTok: Hỗ trợ quy trình xây dựng, quản lý và tự động hóa vận hành tài khoản một điểm dừng, hỗ trợ tốt tính năng phát sóng trực tiếp (livestream).

(6) Cung cấp kết nối [API](https://open.geelark.cn/web/#/602813388/101527801): Lập trình viên có thể viết các kịch bản phần mềm riêng để điều khiển hệ thống Cloud Phone thực hiện các tác vụ tự động hóa nâng cao, hỗ trợ mở cổng ADB điều khiển từ xa.

(7) Trợ lý AI GeeLark: Phiên bản mới nhất đã chính thức tích hợp các tính năng thông minh **kết nối trực tiếp với mô hình DeepSeek R1**. Hệ thống Cloud Phone có khả năng tự động lướt và tương tác trên TikTok mô phỏng hành vi của người dùng thật dựa trên các từ khóa chỉ định, giúp xây dựng các thẻ định danh tài khoản chuẩn xác cho thuật toán TikTok phân phối nội dung.

AI còn hỗ trợ đắc lực trong việc biên soạn các đoạn mô tả sản phẩm hấp dẫn và tự động tạo ra nhiều phiên bản video khác nhau để thử nghiệm hiệu quả phân phối.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022709.webp)

GeeLark hỗ trợ chính sách trải nghiệm miễn phí: **Người dùng mới đăng ký tài khoản sẽ được cấp ngay 2 thiết bị Cloud Phone dùng thử với tổng quỹ thời gian trải nghiệm là 60 phút**. Nếu có nhu cầu khai thác dài hạn với số lượng thiết bị lớn hơn, người dùng có thể lựa chọn nâng cấp các gói trả phí phù hợp.

Các bạn quan tâm có thể truy cập trang chủ [geelark.cn để tải và trải nghiệm thử](https://www.geelark.cn/download-center/?utm_source=ruanyifeng.com&utm_medium=post&utm_campaign=campaign20250228) mà hoàn toàn không yêu cầu liên kết thẻ tín dụng. Tham khảo thêm bài viết hướng dẫn chi tiết dành cho người mới bắt đầu tại [đây](https://www.geelark.cn/blog/beginner-s-guide-how-to-run-a-tiktok-account-efficiently/?utm_source=ruanyifeng.com&utm_medium=post&utm_campaign=campaign20250228).

## [活动] AI FOR CODE 创意挑战赛

Nhằm thúc đẩy phong trào ứng dụng AI vào lập trình và tìm kiếm các phát kiến công nghệ đột phá mới, cuộc thi cấp quốc gia **"AI FOR CODE Creative Challenge"** chuẩn bị được khởi tranh.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022707.webp)

Để khuyến khích đông đảo lập trình viên và học sinh sinh viên tham gia, bên cạnh bảng đấu "Phát triển Ứng dụng" truyền thống, ban tổ chức đã đặc biệt mở rộng thêm bảng đấu "Đề xuất Ý tưởng".

**Chỉ cần bạn sở hữu các ý tưởng sáng tạo độc đáo, ngay cả khi không có năng lực tự tay lập trình phát triển mã nguồn, bạn vẫn hoàn toàn có thể tham gia tranh tài**. Ý tưởng của bạn sẽ là nguồn cảm hứng cho các đội thi khác hiện thực hóa thông qua các công cụ AI. Đây là cơ hội tuyệt vời để biến các ý tưởng sáng tạo của bản thân thành sản phẩm thực tế và giành được các giải thưởng giá trị từ ban tổ chức.

Lễ khai mạc và công bố thể lệ cuộc thi sẽ chính thức được phát sóng trực tiếp vào **18h00 tối thứ Hai tuần tới (ngày 3 tháng 3)**. Chương trình cũng sẽ giới thiệu chi tiết về công cụ lập trình AI **Trae** — môi trường phát triển chính thức được chỉ định cho các đội thi năm nay.

Trong suốt buổi phát sóng trực tiếp, ban tổ chức sẽ tổ chức nhiều đợt **bốc thăm trúng thưởng** với lượng quà tặng vô cùng hấp dẫn. Bên cạnh đó, hoạt động chia sẻ poster giới thiệu cuộc thi đến bạn bè xung quanh cũng đi kèm các phần quà giá trị.

Các bạn quan tâm đến mảng lập trình ứng dụng AI có thể [click vào đây](https://sourl.co/XYmPA8) hoặc quét mã QR trên poster để **đăng ký đặt lịch xem trực tiếp chương trình**.

## 科技动态

**1、Dự án thử nghiệm trạm máy chủ trên Mặt Trăng**

Tuần này, tên lửa Falcon 9 của SpaceX đã phóng thành công một thiết bị đổ bộ lên bề mặt Mặt Trăng.

Thiết bị đổ bộ mang theo một hộp máy chủ mini chuyên dụng (hình dưới) với trọng lượng khoảng 1kg và được tích hợp ổ cứng dung lượng lưu trữ lên tới 8TB.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022710.webp)

Mục tiêu của thử nghiệm này là đánh giá tính khả thi thực tế của việc xây dựng các trung tâm lưu trữ dữ liệu (Data Center) trực tiếp trên bề mặt Mặt Trăng.

So với Trái Đất, Mặt Trăng hoàn toàn không tồn tại các hiện tượng thiên tai tự nhiên, không có mưa gió, không có độ ẩm hay dưỡng khí gây oxy hóa thiết bị, và đặc biệt là không có nguy cơ từ chiến tranh hay các hoạt động phá hoại của con người. Về mặt vật lý, ngoại trừ nguy cơ nhỏ từ việc bị thiên thạch va chạm, cấu trúc địa lý bề mặt Mặt Trăng hầu như không ghi nhận sự thay đổi nào trong suốt hàng vạn năm qua.

Do đó, các nhà khoa học đã đề xuất giải pháp đưa các dữ liệu tri thức quan trọng của nhân loại lên lưu trữ tại Mặt Trăng nhằm bảo đảm khả năng tồn tại vĩnh cửu của dữ liệu.

Thử nghiệm lần này tập trung đánh giá xem hệ thống máy chủ mini có thể vận hành ổn định bằng nguồn điện năng mặt trời trong điều kiện chênh lệch nhiệt độ cực hạn giữa ngày và đêm trên Mặt Trăng hay không.

**2、Thử nghiệm nguyên mẫu xe ô tô bay**

Mẫu xe ô tô bay do doanh nghiệp được tỷ phú Elon Musk đầu tư phát triển mới đây đã tiến hành các bước bay thử nghiệm thực tế đầu tiên.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022208.webp)

Điểm đặc biệt nhất của mẫu phương tiện này là việc sở hữu kiểu dáng tương tự như một chiếc ô tô thông thường và hoàn toàn không để lộ hệ thống cánh quạt nâng bên ngoài. Các cánh quạt nâng được hãng thiết kế ẩn hoàn toàn bên trong thân xe.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022209.webp)

Trong đợt thử nghiệm thực tế, phương tiện chỉ thực hiện bay ở độ cao giới hạn dưới 5 mét so với mặt đất, duy trì độ cao này di chuyển về phía trước một khoảng ngắn trước khi đáp xuống.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022210.webp)

Nhà sản xuất chia sẻ hai kịch bản ứng dụng thực tế lớn nhất của dòng xe này là: Hỗ trợ người lái bay vượt qua các chướng ngại vật ùn tắc giao thông do tai nạn phía trước, hoặc di chuyển bay vượt qua các vùng lòng sông, mặt nước nhỏ.

Sản phẩm được định giá bán dự kiến khoảng 300.000 USD (tương đương hơn 7 tỷ VNĐ) và kế hoạch bàn giao những chiếc xe đầu tiên vào cuối năm nay, trở thành mẫu xe ô tô bay thương mại đầu tiên được mở bán chính thức trên thế giới.

**3、Hạ tầng phát điện năng lượng mặt trời trên quỹ đạo không gian**

Mặc dù ngành công nghiệp năng lượng mặt trời đang ghi nhận tốc độ tăng trưởng vượt trội, nó vẫn đối mặt với một hạn chế vật lý lớn là không thể phát điện liên tục suốt 24 giờ do chu kỳ ngày đêm và ảnh hưởng của thời tiết mây mưa.

Để khắc phục rào cản này, các nhà khoa học đã đề xuất giải pháp đưa toàn bộ các tấm pin quang năng lên hoạt động trên không gian vũ trụ để đón ánh nắng mặt trời liên tục 24/7, sau đó truyền tải nguồn năng lượng thu được về Trái Đất.

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024102405.webp)

Một doanh nghiệp khởi nghiệp tại Mỹ đang tích cực triển khai dự án thương mại hóa ý tưởng này với kế hoạch phóng vệ tinh thử nghiệm đầu tiên vào năm 2026.

Thiết kế hệ thống tương tự cấu trúc chùm vệ tinh Starlink: Hàng loạt vệ tinh quang năng sẽ được xếp thành một hàng dọc trên quỹ đạo để hấp thụ ánh sáng mặt trời chuyển hóa thành điện năng, sau đó truyền dẫn năng lượng về Trái Đất thông qua hệ thống chùm tia laser hồng ngoại công suất lớn.

Tại mặt đất sẽ xây dựng các trạm tiếp nhận năng lượng phân tán. Mỗi trạm sẽ đảm nhận nhiệm vụ thu nhận năng lượng từ vệ tinh đang bay qua đỉnh đầu, và khi vệ tinh đó di chuyển qua vùng khuất sẽ tiếp tục đón nhận luồng năng lượng từ vệ tinh tiếp theo trong chùm.

**4、Các tin tức khác**

(1) Chính quyền tỉnh Hồ Nam (Trung Quốc) ban hành quy định nghiêm cấm các cơ sở y tế ứng dụng các công cụ AI tự động kê đơn thuốc trực tiếp cho bệnh nhân.

(2) Các nhà khảo cổ học tại Ai Cập mới đây đã phát hiện thêm một lăng mộ pharaoh cổ đại với lối vào được ngụy trang vô cùng kín kẽ dưới đáy thung lũng (hình dưới). Đây là cột mốc phát hiện lăng mộ pharaoh đầu tiên sau hơn 100 năm kể từ sự kiện tìm thấy lăng mộ của pharaoh Tutankhamun vào năm 1922.

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022204.webp)

## 文章

1][Cẩm nang hướng dẫn tự triển khai mô hình DeepSeek chạy cục bộ trên máy tính cá nhân](https://blog.lovefc.cn/archives/start.html) (tiếng Trung)

Bài hướng dẫn chi tiết các bước giúp người dùng cấu hình và vận hành các phiên bản mô hình nhỏ của DeepSeek trực tiếp trên phần cứng máy tính gia đình thông thường một cách đơn giản. (Đóng góp từ [@lovefc](https://github.com/ruanyf/weekly/issues/6150))

2、[Hướng dẫn từng bước tự lập trình xây dựng một mô hình ngôn ngữ lớn từ con số không](https://brettgfitzgerald.com/posts/build-a-large-language-model/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022207.webp)

Tác giả chia sẻ kinh nghiệm thực tế khi tự học và xây dựng một mô hình ngôn ngữ lớn dựa trên giáo trình học thuật chuyên ngành (hình trên), đồng thời giải thích một cách dễ hiểu về các nguyên lý thuật toán AI cốt lõi phía sau.

3、[Góc nhìn: Phiên bản Svelte 5 không thực sự là JavaScript](https://hodlbod.npub.pro/post/1739830562159/) (tiếng Anh)

Svelte là một trong những bộ khung phát triển frontend được yêu thích nhất hiện nay. Tác giả sau một thời gian trải nghiệm phiên bản Svelte 5.0 mới phát hành chia sẻ nhận định rằng do mức độ trừu tượng hóa của thư viện quá cao, cú pháp lập trình của nó hiện tại giống như một ngôn ngữ lập trình hoàn toàn mới hơn là cú pháp JavaScript thông thường.

4、[Nhật ký hành trình phỏng vấn vào vị trí kỹ sư phần mềm tại Google London](https://justyy.com/archives/68019) (tiếng Trung)

Tác giả chia sẻ chi tiết toàn bộ quá trình nộp hồ sơ, trải qua các vòng phỏng vấn kỹ thuật căng thẳng và cuối cùng nhận được thư từ chối từ văn phòng Google tại London. (Đóng góp từ [@DoctorLai](https://github.com/ruanyf/weekly/issues/6151))

5、[10 ý tưởng khai thác hệ thống máy ảo Proxmox cho phòng thí nghiệm tại gia](https://www.xda-developers.com/projects-i-host-on-my-proxmox-home-lab/) (tiếng Anh)

Proxmox hiện giữ vị thế là một trong những phần mềm quản lý máy ảo hypervisor phổ biến nhất hiện nay. Bài viết gợi ý 10 dự án thực tiễn giúp người dùng tối ưu hóa hạ tầng máy ảo phục vụ nhu cầu nghiên cứu cá nhân.

6、[Kinh nghiệm lập trình tính năng điều khiển chuột máy tính bằng nhận diện cử chỉ tay](https://chernando.com/blog/2023/07/23/hand-tracking-for-mouse-input.html) (tiếng Anh)

Bài viết hướng dẫn kỹ thuật chi tiết cách phối hợp thư viện nhận diện hình ảnh MediaPipe của Google và thư viện OpenCV để chuyển đổi các cử chỉ tay thu nhận từ camera máy tính thành các lệnh điều khiển chuột mượt mà.

7、[Hướng dẫn thiết kế hiệu ứng kính mờ (Frosted Glass) cho giao diện trang web](https://www.tyleo.com/html-glass.html) (tiếng Anh)

Bài hướng dẫn chi tiết các bước thiết lập mã nguồn HTML và CSS để tạo nên các khối hộp giao diện có hiệu ứng làm mờ và trong suốt sang trọng cho trang web.

8、[Tìm hiểu cú pháp phạm vi ảnh hưởng cục bộ @scope trong CSS](https://picostitch.com/tidbits/2024/10/inline-scope-for-css/) (tiếng Anh)

Bài viết giới thiệu về cú pháp `@scope` mới được hỗ trợ trên trình duyệt Chrome, giúp định nghĩa các quy tắc định dạng CSS chỉ có hiệu lực cục bộ bên trong một phân vùng chỉ định mà hoàn toàn không ảnh hưởng đến toàn bộ trang web.

## 工具

1、[digiKam](https://www.digikam.org/)

Phần mềm quản lý và biên tập bộ sưu tập hình ảnh cá nhân mã nguồn mở và chuyên nghiệp chạy trực tiếp trên máy tính.

2、[Web Awesome](https://backers.webawesome.com/)

Bộ thư viện các thành phần giao diện Web Components chất lượng cao và dễ tùy biến dành cho lập trình viên.

3、[WhiteSur](https://github.com/vinceliuice/WhiteSur-gtk-theme)

Dự án cung cấp bộ giao diện thiết kế (theme) theo phong cách macOS sang trọng dành cho các bản phân phối hệ điều hành Linux sử dụng môi trường GTK.

4、[mdq](https://github.com/yshavit/mdq)

Công cụ dòng lệnh hỗ trợ truy vấn và trích xuất nhanh các thông tin cấu trúc từ tệp tin định dạng Markdown, với cơ chế hoạt động tương tự công cụ jq xử lý tệp tin JSON.

5、[Electro](https://github.com/pTinosq/Electro)

Ứng dụng xem hình ảnh siêu tốc thông qua môi trường dòng lệnh được phát triển bằng ngôn ngữ Rust tối ưu hiệu năng.

6、[Liên Đồ (Link to Image)](https://Wind-liang.github.io/link-to-image/)

Dự án trực tuyến mã nguồn mở hỗ trợ người dùng nhanh chóng chuyển đổi một liên kết trang web bất kỳ thành một bức ảnh poster giới thiệu đẹp mắt tích hợp mã QR truy cập nhanh. (Đóng góp từ [@wind-liang](https://github.com/ruanyf/weekly/issues/6162))

7、[MinMail.app](https://minmail.app/cn)

Dịch vụ web hỗ trợ tạo các hòm thư điện tử tạm thời (disposable email) hoàn toàn miễn phí giúp bảo vệ thông tin cá nhân khi đăng ký dịch vụ. (Đóng góp từ [@withoctober](https://github.com/ruanyf/weekly/issues/6179))

8、[MoePush](https://github.com/beilunyang/moepush)

Dịch vụ thông báo đẩy (push notifications) mã nguồn mở phát triển trên Next.js và Cloudflare, hỗ trợ đồng bộ gửi thông báo qua nhiều kênh liên lạc như DingTalk, WeChat Enterprise, Telegram... (Đóng góp từ [@beilunyang](https://github.com/ruanyf/weekly/issues/6180))

9、[Ant Design X Vue](https://github.com/wzc520pyfm/ant-design-x-vue)

Dự án biên dịch bộ thư viện thiết kế chuyên biệt cho các giao diện ứng dụng AI Ant Design X sang phiên bản hỗ trợ framework Vue. (Đóng góp từ [@wzc520pyfm](https://github.com/ruanyf/weekly/issues/6184))

10、[New SVG Viewer](https://github.com/liujuntao123/new-svg-viewer)

Dịch vụ trực tuyến mã nguồn mở hỗ trợ người dùng nhanh chóng xem trước và tối ưu hóa các tệp tin đồ họa định dạng SVG. (Đóng góp từ [@liujuntao123](https://github.com/ruanyf/weekly/issues/6185))

11、[Statusnook](https://github.com/goksan/Statusnook)

Bộ mã nguồn cho phép người dùng tự triển khai một trang giám sát trạng thái hoạt động (Status Page) tối giản để theo dõi độ ổn định của các dịch vụ web.

12、[llm-commit](https://github.com/GNtousakis/llm-commit)

Công cụ dòng lệnh gọn nhẹ hỗ trợ ứng dụng mô hình ngôn ngữ lớn để tự động phân tích các thay đổi mã nguồn và biên soạn các nội dung thông điệp commit (commit messages) chuẩn xác cho Git.

## 资源

1、[Dịch thuật Trung - Nhật trực quan](https://zh2ja.whoops.space/)

Trang web hỗ trợ dịch thuật nhanh từ tiếng Trung sang tiếng Nhật đi kèm hiển thị phiên âm chữ Kana và phiên âm Romaji giúp hỗ trợ đắc lực cho người học ngoại ngữ. (Đóng góp từ [@zhanghuid](https://github.com/ruanyf/weekly/issues/6181))

2、[Trải nghiệm làm gốm 3D tương tác](https://artsandculture.google.com/experiment/3d-pottery/nwHg1D0riJ1ltA)

Một ứng dụng web nhỏ thú vị do Google phát triển, cho phép người dùng trải nghiệm các thao tác nhào nặn và tạo hình các sản phẩm gốm sứ nghệ thuật dưới dạng không gian 3D tương tác trực tiếp trên trình duyệt.

3、[Mô hình 3D tương tác tháp truyền hình Sutro Tower](https://vincentwoo.com/3d/sutro_tower/)

Tháp truyền hình Sutro Tower là công trình biểu tượng cao 298 mét tại thành phố San Francisco. Tác giả đã xử lý ghép nối hàng nghìn bức ảnh chụp từ thiết bị bay không người lái để tái dựng nên mô hình 3D tương tác của ngọn tháp với độ chi tiết cực cao. (Đóng góp từ [@YuJianrong](https://github.com/ruanyf/weekly/issues/6161))

4、[Tổng hợp các phương thức tấn công mã hóa đường cong elip (ECC)](https://github.com/elikaski/ECC_Attacks)

Kho chứa mã nguồn mở chia sẻ các tài liệu nghiên cứu và mã nguồn minh họa về các lỗ hổng và phương thức tấn công bảo mật nhắm vào hệ thống mật mã hóa đường cong elip.

## 图片

1、[Thiết kế mỏ kẹp phân hình (Fractal Vise)](https://airgraver.com/fractal-vise.htm)

Ê tô (mỏ kẹp) là dụng cụ cơ khí vô cùng quen thuộc được ứng dụng để kẹp chặt các chi tiết phôi trong quá trình gia công cơ khí.

Các thiết kế ê tô truyền thống thông thường sở hữu hai má kẹp phẳng cố định, do đó chúng chỉ hoạt động hiệu quả khi kẹp các chi tiết phôi có hình khối hình học phẳng và đối xứng.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071001.webp)

Để kẹp chặt các chi tiết có biên dạng hình học phức tạp và không quy luật, các kỹ sư đã chế tạo ra dòng ê tô phân hình độc đáo sử dụng hệ thống các má kẹp nhỏ có khả năng tự động xoay chuyển góc độ để ôm khít vào bề mặt phôi.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071002.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071003.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071004.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071006.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071005.webp)

## 文摘

1、[Nếu không có ai đọc bài viết của bạn, việc duy trì viết blog còn mang lại ý nghĩa gì?](https://andysblog.uk/why-blog-if-nobody-reads-it/)

Chúng ta hãy cùng thẳng thắn nhìn nhận thực tế này: Khi bạn viết xong và xuất bản một bài chia sẻ lên blog cá nhân, hầu như sẽ không có ai tìm đọc nó cả.

Hoặc ít nhất, lượng người đọc sẽ ít hơn rất nhiều so với kỳ vọng của bạn. Bạn đã dành nhiều tâm huyết để đúc rút suy nghĩ thành câu chữ, trau chuốt từng đoạn văn, lựa chọn hình ảnh minh họa kỹ lưỡng — để rồi sau khi đăng tải chỉ nhận lại sự im lặng tuyệt đối, không lượt thích, không lượt chia sẻ hay bình luận tương tác nào.

Vậy việc duy trì viết blog cá nhân trong bối cảnh đó thực chất mang lại giá trị gì?

Đầu tiên, tồn tại hai quan điểm sai lầm phổ biến về việc viết blog. Quan điểm thứ nhất là: Chỉ cần tôi viết được bài viết chất lượng tốt, độc giả tự khắc sẽ tìm đến. Thực tế hoàn toàn không như vậy. Giữa không gian Internet khổng lồ với hàng tỷ bài viết mới được xuất bản mỗi ngày như một cơn bão lớn, trang blog nhỏ của bạn chỉ giống như một chiếc lá mỏng rơi giữa bão, hầu như không ai có thể chú ý tới.

Quan điểm sai lầm thứ hai là: Nếu bài viết không có ai đọc, việc viết lách chỉ là một hoạt động lãng phí thời gian vô ích.

Thực tế, viết blog sở hữu những giá trị ẩn sâu bên trong. Bạn đặt bút viết hoàn toàn không phải để tìm kiếm những tràng pháo tay tán thưởng từ số đông bên ngoài, mà vì nhu cầu phát triển của chính bản thân bạn.

Quy trình viết blog giúp rèn luyện khả năng tư duy mạch lạc cho bộ não. Việc cố gắng diễn đạt suy nghĩ thành câu chữ rõ ràng buộc bạn phải sắp xếp lại các luồng suy nghĩ lộn xộn trong đầu, từ đó giúp nâng cao năng lực phân tích vấn đề. Khi bạn có được tư duy logic tốt hơn, bạn sẽ đạt được các kết quả làm việc xuất sắc hơn.

**Đối tượng độc giả quan trọng nhất của các bài viết trên blog thực chất không phải là cộng đồng mạng, mà chính là bản thân bạn trong tương lai**. Những bài viết cũ sẽ là tấm gương phản chiếu rõ nét chặng đường phát triển tư duy của chính bạn qua các thời kỳ.

Bên cạnh đó, vào một thời điểm nào đó trong tương lai, một người thực sự cần đến những kiến thức chia sẻ của bạn chắc chắn sẽ tìm ra bài viết của bạn thông qua các công cụ tìm kiếm. Giá trị ảnh hưởng dài hạn của một bài viết chia sẻ sâu sắc luôn bền vững hơn nhiều so với những thông tin giật gân có tốc độ lan truyền nhanh nhưng sớm bị lãng quên.

Hoạt động viết blog có nhiều nét tương đồng với nghệ thuật nhiếp ảnh đường phố. Bạn cầm chiếc máy ảnh đi dạo quanh các góc phố đô thị. Khi bắt gặp một khung cảnh ánh sáng đẹp mắt, một khoảnh khắc tương tác giàu tính nhân văn, bạn bấm máy lưu lại khoảnh khắc đó.

Hầu như không ai quan tâm hay biết đến bức ảnh bạn vừa chụp. Nhưng đó hoàn toàn không phải là mục tiêu khiến bạn bấm máy. **Bạn chụp ảnh đơn giản bởi vì mắt bạn đã quan sát và cảm nhận được vẻ đẹp của khoảnh khắc đó**.

Viết blog cũng tương tự như vậy. **Bạn viết bởi vì bộ não của bạn đang không ngừng tư duy, bởi vì bạn đang tích cực quan sát cuộc sống xung quanh, và bạn mong muốn lưu lại những chiêm nghiệm đó tại một không gian kỷ niệm**.

Nếu bài viết may mắn nhận được sự quan tâm từ độc giả, đó là một niềm vui lớn đi kèm. Còn nếu không, quy trình tự học tập và rèn luyện tư duy thông qua viết lách của bản thân bạn cũng đã được hoàn thành một cách trọn vẹn.

Đó mới chính là giá trị cốt lõi nhất của việc viết blog.

## 言论

1、

Một số tập đoàn công nghệ lớn hiện nay thiết lập chính sách chỉ tuyển dụng các kỹ sư phần mềm cấp trung và cấp cao, hoàn toàn từ chối các lập trình viên mới vào nghề (junior). Tôi cho rằng đây là một tư duy quản trị sai lầm.

Bởi lẽ các doanh nghiệp công nghệ hiện đại hoạt động dựa trên nền tảng tích lũy tri thức. Sự xuất hiện của các nhân sự trẻ trong đội ngũ sẽ tạo ra một áp lực tích cực buộc các nhân sự kỳ cựu phải thực hiện việc đào tạo, chuyển giao kiến thức và hợp tác, từ đó giúp doanh nghiệp không ngừng tái tạo và phát triển kho tàng tri thức nội bộ.

-- *Trích bài phân tích 《Tại sao doanh nghiệp của bạn luôn cần các lập trình viên trẻ》*

2、

Các cấp quản lý tại công ty tôi (những người hoàn toàn không có chuyên môn về kỹ thuật) hiện đang bị cuốn vào làn sóng truyền thông tin tưởng tuyệt đối rằng công cụ AI có thể thay thế hoàn toàn lập trình viên. Giám đốc công nghệ (CTO) của chúng tôi thậm chí từng phát biểu: "Việc ứng dụng GPT để tự động viết mã nguồn là tác vụ vô cùng đơn giản có thể hoàn thiện ngay trong ngày".

Họ thực sự tin rằng AI có thể thay thế hoàn toàn các lập trình viên lành nghề chỉ sau một đêm. Trong khi bản thân họ chưa từng tự tay viết hay triển khai bất kỳ một dòng code chạy thực tế nào bằng GPT, mà chỉ đơn thuần đọc các bài viết quảng cáo PR của các hãng công nghệ để rồi thần thánh hóa sức mạnh của AI.

-- *Trích chia sẻ 《Làm thế nào để ứng phó với văn hóa phát triển phần mềm đang bị bóp méo hiện nay》*

3、

Mục tiêu tối thượng mà tôi kỳ vọng ở robot là chúng có thể đảm nhận thay con người các tác vụ lao động chân tay mệt mỏi hằng ngày như rửa bát, giặt quần áo. Tôi hoàn toàn không mong muốn chúng thay thế con người ở các hoạt động sáng tạo nghệ thuật như chơi nhạc, lập trình viết code hay sáng tác văn học.

-- *Trích bài phân tích 《Liệu tôi có đang vi phạm các quy chuẩn đạo đức khi ứng dụng mô hình lớn?》*

4、

Các doanh nghiệp đường sắt Nhật Bản thường sở hữu quỹ đất khổng lồ xung quanh khu vực các nhà ga. Để tối ưu hóa lượng hành khách đi tàu, họ chủ động đầu tư xây dựng các khu đô thị phức hợp, trung tâm thương mại và khách sạn ngay cạnh nhà ga để thu hút người dân đến sinh hoạt.

Thậm chí họ còn tự thành lập các đoàn nghệ thuật biểu diễn riêng, tiêu biểu như đoàn ca múa nhạc nổi tiếng Takarazuka Revue do chính công ty đường sắt Hankyu sáng lập nhằm mục đích kích cầu người dân mua vé tàu đi xem biểu diễn nghệ thuật.

-- *Ý kiến chia sẻ của độc giả trên diễn đàn Hacker News*

5、

Tiến trình phát triển xã hội của con người thường tuân theo quy luật: Đầu tiên tập trung giải quyết nhu cầu sinh tồn cơ bản, tiếp theo hướng tới tính tiện dụng thực tế, sau đó theo đuổi sự tiện nghi thoải mái, rồi chuyển sang hưởng thụ các khoái cảm giải trí dẫn đến lối sống xa xỉ phù phiếm, và cuối cùng rơi vào trạng thái điên cuồng lãng phí vật chất xã hội.

-- *Giambattista Vico, nhà triết học người Ý nổi tiếng chia sẻ*

## 往年回顾

- Số #292: [Thảo luận sâu về luận điểm: Mọi dòng mã nguồn được viết ra thực chất đều là một khoản nợ kỹ thuật](https://www.ruanyifeng.com/blog/2024/03/weekly-issue-292.html)
- Số #242: [Chia sẻ bài học kinh nghiệm từ một sự cố bị tấn công xâm nhập máy chủ đáng xấu hổ](https://www.ruanyifeng.com/blog/2023/02/weekly-issue-242.html)
- Số #192: [Phân tích luận điểm: Những cơ hội phát triển lớn nhất luôn xuất hiện đi kèm với các công nghệ mới](https://www.ruanyifeng.com/blog/2022/01/weekly-issue-192.html)
- Số #142: [Lập luận chứng minh năm 2020 mới thực sự là năm khởi đầu của thế kỷ 21](https://www.ruanyifeng.com/blog/2021/01/weekly-issue-142.html)

(Hết)
