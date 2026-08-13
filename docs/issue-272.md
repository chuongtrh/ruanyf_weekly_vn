# Bản tin chia sẻ công nghệ (Số 272): Phí cài đặt của Unity - hình bóng thu nhỏ của ngành game

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần. (Thông báo: Bản tin sẽ tạm nghỉ trong kỳ nghỉ lễ sắp tới, xin hẹn gặp lại bạn đọc sau kỳ nghỉ lễ).

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3425) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091706.webp)

Nghệ sĩ điêu khắc nổi tiếng nhất của Colombia, Fernando Botero, đã qua đời vào tháng này ở tuổi 91. Ông được biết đến rộng rãi trên toàn cầu nhờ phong cách nghệ thuật độc đáo chuyên tạo hình những nhân vật và loài động vật có tỷ lệ cơ thể mập mạp, mang lại cảm giác hài hước và ngộ nghĩnh. Bức ảnh trên chụp tác phẩm điêu khắc nổi tiếng *“Chú Mèo”* của ông. Vào năm 2016, khi ông tổ chức triển lãm tác phẩm cá nhân tại Trung Quốc, tôi cũng đã có dịp đến thưởng lãm trực tiếp các tác phẩm này. (Nguồn: [France24](https://www.france24.com/en/americas/20230915-colombia-s-most-famous-artist-fernando-botero-passes-away-at-91))

## Unity 的安装费，游戏业的缩影

[Unity](https://unity.com) là một trong những game engine hàng đầu thế giới hiện nay. Rất nhiều tựa game di động và game web đình đám đang làm mưa làm gió trên thị trường đều được xây dựng trên nền tảng này, tiêu biểu như *Vương Giả Vinh Diệu* hay *Genshin Impact*.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091902.webp)

Trang web chính thức của hãng tự hào công bố: *“Trong số 1.000 tựa game di động có doanh thu hàng đầu trên thị trường hiện nay, có tới 70% nhà phát triển lựa chọn sử dụng engine Unity.”*

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091903.webp)

Trước đây, mô hình thương mại của Unity dựa trên việc thu phí dịch vụ hàng tháng đối với các nhà phát triển. Điều kiện bắt buộc là khi tựa game đạt mức doanh thu tích lũy vượt mốc 200.000 USD/năm, nhà phát triển sẽ phải mua các gói bản quyền trả phí của hãng, mức doanh thu game càng cao thì phí dịch vụ phải trả càng lớn.

Tuy nhiên vào ngày 12 tháng 9 vừa qua, Unity đã [bất ngờ ra thông báo](https://blog.unity.com/news/plan-pricing-and-packaging-updates) về việc thay đổi toàn diện chính sách thu phí. **Kể từ ngày 1 tháng 1 năm sau, bên cạnh các khoản phí bản quyền định kỳ sẵn có, hãng sẽ áp dụng thêm một khoản phí hoàn toàn mới gọi là: Phí cài đặt (Runtime Fee).**

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091904.webp)

Theo chính sách mới, đối với các tựa game có doanh thu hàng năm vượt mốc 200.000 USD và đạt lượng cài đặt tích lũy trên 200.000 lượt, kể từ lượt tải về tiếp theo, nhà phát triển sẽ phải chi trả cho Unity mức phí **0,20 USD cho mỗi lượt cài đặt mới**.

Hãy thử làm một phép tính đơn giản để thấy chính sách này sẽ làm gia tăng gánh nặng tài chính khổng lồ thế nào cho các studio game: Giả sử một tựa game có lượng tải về đạt 1 triệu lượt mỗi năm, sau khi trừ đi hạn mức miễn phí 200.000 lượt đầu, nhà phát triển sẽ phải trả thêm cho Unity khoản phí cài đặt lên tới 160.000 USD. Nếu tổng doanh thu của tựa game đó trong năm chỉ đạt khoảng 300.000 USD, thì hơn một nửa số tiền kiếm được đã lập tức biến mất vào túi của Unity.

Khoản phí này được ví như đòn chí mạng giáng trực tiếp vào các nhà phát triển game độc lập quy mô nhỏ. Nhóm này thường lựa chọn mô hình phát hành game miễn phí kiếm tiền bằng quảng cáo (Free-to-Play). Theo các báo cáo [thống kê doanh thu ngành quảng cáo](https://www.is.com/glossary/ad-revenue/), doanh thu trung bình mang lại từ mỗi lượt hiển thị quảng cáo trong game chỉ đạt khoảng 0,02 USD. Để có đủ tiền chi trả khoản phí cài đặt 0,20 USD của Unity, nhà phát triển buộc phải bắt mỗi người chơi xem thêm ít nhất 10 lần quảng cáo nữa.

Chính vì vậy ngay khi chính sách giá mới được công bố, làn sóng giận dữ đã bùng lên mạnh mẽ trong cộng đồng các nhà phát triển game toàn cầu. Nhiều studio đã lên tiếng chỉ trích Unity có hành vi "ăn cháo đá bát", tận thu quá mức và bắt đầu lên kế hoạch chuyển dịch mã nguồn dự án sang các game engine thay thế khác như Godot hay Unreal.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091905.webp)

Trong số rất nhiều bài viết thảo luận về chủ đề này, tôi có đọc được [một bài phân tích độc lập khá sâu sắc](https://www.gamesindustry.biz/unitys-pricing-is-a-symptom-not-the-cause-of-tougher-times-ahead-for-the-games-industry-opinion) đưa ra góc nhìn khách quan bênh vực cho Unity (hình dưới). Tác giả cho rằng Unity thực chất cũng đang rơi vào tình thế tiến thoái lưỡng nan buộc phải tăng phí để sinh tồn, bởi vì **bối cảnh chung của toàn ngành công nghiệp game đã thay đổi sâu sắc**. Tôi nghĩ đây là một góc nhìn rất đáng chia sẻ cùng bạn đọc:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091906.webp)

Tình hình tài chính thực tế của bản thân tập đoàn Unity đang gặp rất nhiều khó khăn. Mặc dù là một công ty đại chúng đã niêm yết trên thị trường chứng khoán từ năm 2020, Unity chưa từng ghi nhận một năm tài chính nào có lãi. Chỉ tính riêng trong nửa đầu năm nay, khoản lỗ lũy kế của hãng đã lên tới 440 triệu USD.

Đây thực sự là một thực trạng trớ trêu: ngành công nghiệp trò chơi điện tử vốn nổi tiếng là mỏ vàng hái ra tiền, nhưng bản thân doanh nghiệp cung cấp công cụ cốt lõi xây dựng nên các tựa game đó lại liên tục thua lỗ.

Trước đây, ban lãnh đạo Unity tập trung ưu tiên cho mục tiêu tăng trưởng thị phần và chấp nhận hy sinh biên lợi nhuận. Đến hiện tại, việc ban điều hành mới quyết định thắt chặt chính sách thu phí để cải thiện bảng cân đối kế toán là điều có thể hiểu được về mặt kinh doanh.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091907.webp)

Vậy tại sao Unity lại quyết định thay đổi chiến lược vào thời điểm này? Nguyên nhân chính là tốc độ tăng trưởng thần tốc của ngành game toàn cầu đã chính thức khép lại. Báo cáo tài chính năm 2022 ghi nhận **lần đầu tiên doanh thu ngành game toàn cầu sụt giảm sau nhiều năm tăng trưởng liên tục**, và số liệu của năm nay vẫn chưa cho thấy dấu hiệu khởi sắc trở lại.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091908.webp)

Đáng ngại hơn là **quy mô lượng người chơi game trên thế giới dường như đã chạm trần**. Tình trạng già hóa dân số và sụt giảm tỷ lệ sinh tại các nền kinh tế lớn khiến lượng game thủ mới gia nhập thị trường ngày một ít đi.

Điều này tác động mạnh mẽ tới mô hình kinh doanh của các hãng game. Hiện nay, nguồn thu chính không còn đến từ việc bán đứt đĩa game mà phụ thuộc vào việc gia tăng số lượng người chơi tương tác hàng ngày và kéo dài tổng thời gian chơi game trong ứng dụng. Một khi lượng người chơi ngừng tăng trưởng, doanh thu của hãng cũng sẽ nhanh chóng đi vào ngõ cụt.

Quỹ thời gian trong ngày của mỗi người chơi chỉ giới hạn ở mức 24 giờ và sự chú ý là có hạn. **Ngành game từ nay sẽ phải bước vào cuộc chiến khốc liệt cạnh tranh trực tiếp với hàng loạt hình thức giải trí khác (như xem tivi, lướt video ngắn, ăn uống hay tập gym) để giành giật thời gian của người dùng.**

Thêm vào đó, bối cảnh lạm phát và lãi suất neo cao tại các quốc gia Âu Mỹ trong năm nay đã làm gia tăng đáng kể chi phí vốn đầu tư và rủi ro tài chính cho các dự án phát triển game mới.

Tổng hợp các yếu tố trên, ban lãnh đạo Unity nhận định kỷ nguyên tăng trưởng nóng của ngành game đã chính thức khép lại. Nhận định này không có nghĩa là ngành game sẽ suy thoái ngay lập tức, mà ám chỉ thị trường đã chuyển sang giai đoạn bão hòa ổn định.

Đồng thời, biên lợi nhuận của việc phát triển và phát hành game ngày càng bị thu hẹp, dẫn đến xu hướng thị trường sẽ dần tập trung vào tay một số ít ông lớn có tiềm lực tài chính mạnh, việc các studio game nhỏ bị thâu tóm hoặc sáp nhập là điều tất yếu sẽ diễn ra.

Do đó, tác giả bài viết muốn nhắn nhủ rằng: chính sách thu phí cài đặt mới của Unity không đơn thuần là hành vi bóc lột nhà phát triển, mà là một nỗ lực tự cứu lấy mình để chuẩn bị cho giai đoạn khó khăn sắp tới của thị trường. Điểm trừ lớn nhất là chính sách này đã trực tiếp hy sinh lợi ích của các nhà phát triển game quy mô nhỏ.

> *“Các nhà phát triển đang phẫn nộ với Unity nên nhận ra rằng chính sách tăng giá mới không phải là nguyên nhân gây ra vấn đề, mà nó là biểu hiện rõ nét của một thời kỳ đầy thử thách và khó khăn sắp tới của toàn ngành game.”*
>
> *“Unity đã nhận diện được xu hướng này và đang chủ động tìm kiếm các giải pháp quản trị tài chính để giảm thiểu rủi ro cho mình trước làn sóng tái cơ cấu của ngành game.”*

## 科技动态

1、[Mỹ thử nghiệm trồng dây leo phủ xanh tường nhà để hạ nhiệt đô thị](https://www.ucdavis.edu/climate/what-can-i-do/blog/can-vines-speed-urban-cooling)

Một nhóm nghiên cứu tại Đại học California đang thực hiện dự án trồng thử nghiệm các loài dây leo phủ kín bề mặt ngoài của các tòa nhà cao tầng nhằm kiểm nghiệm hiệu quả hạ nhiệt tự nhiên cho các đô thị:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082801.webp)

Mục tiêu của nghiên cứu là tìm kiếm và lai tạo dòng thực vật dây leo tối ưu nhất: sở hữu tốc độ sinh trưởng nhanh, độ phủ lá rộng giúp che chắn ánh nắng hiệu quả nhưng yêu cầu lượng nước tưới tối thiểu để tiết kiệm tài nguyên.

Trong bối cảnh ấm lên toàn cầu, việc tăng diện tích mảng xanh là phương án tối ưu để giảm hiệu ứng đảo nhiệt đô thị. So với việc trồng cây xanh đô thị truyền thống, việc trồng dây leo bám tường sở hữu các ưu điểm lớn như: (1) thời gian phủ xanh nhanh hơn rất nhiều; (2) chi phí đầu tư ban đầu cực kỳ rẻ; (3) cây tự bám phủ theo hình dáng cấu trúc của tòa nhà mà không cần cắt tỉa.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082802.webp)

Tuy nhiên, phương pháp này cũng có nhược điểm là đòi hỏi mặt tường ngoài của tòa nhà phải được thi công lắp đặt thêm hệ thống dây cáp treo hoặc lưới thép chịu lực để cây có thể bám leo. Ngoài ra, việc bao phủ một lớp thực vật khô quanh nhà cũng tiềm ẩn nguy cơ mất an toàn phòng cháy chữa cháy nếu xảy ra hỏa hoạn.

2、[Framework ra mắt dòng hộp mica biến mainboard laptop cũ thành máy tính mini để bàn](https://arstechnica.com/gadgets/2023/08/turning-my-framework-laptop-into-a-tiny-desktop-was-fun-now-it-needs-a-job/)

Thương hiệu máy tính Framework nổi tiếng với triết lý thiết kế phần cứng mô-đun cho phép người dùng tự do tháo lắp, thay thế nâng cấp từng linh kiện riêng lẻ của máy tính để giảm thiểu rác thải điện tử.

Mới đây, hãng đã hợp tác cùng Cooler Master để cho ra mắt một sản phẩm phụ kiện rất độc đáo: hộp đựng mainboard chuyên dụng.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080801.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080802.webp)

Sản phẩm cho phép người dùng tháo rời bo mạch chủ (mainboard) từ chiếc laptop Framework cũ đã nâng cấp của mình để lắp gọn vào bên trong chiếc hộp nhựa mica trong suốt nhỏ gọn này, biến nó lập tức thành một thùng máy tính để bàn mini (Mini PC) độc đáo hoạt động hoàn hảo. Chiếc hộp được thiết kế sẵn các cổng kết nối ngoại vi, nút nguồn tiện lợi và quạt tản nhiệt độc lập:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080804.webp)

Đi kèm sản phẩm là tài liệu hướng dẫn trực quan chi tiết chỉ dẫn người dùng các bước tháo lắp bo mạch chủ từ laptop sang hộp đựng một cách an toàn.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080803.webp)

Đây là một sáng kiến công nghệ rất có ý nghĩa thực tế, giúp tận dụng tối đa vòng đời của các bo mạch chủ cũ để làm máy chủ gia đình hoặc máy tính văn phòng nhỏ, tránh lãng phí linh kiện điện tử. Hy vọng các hãng máy tính lớn khác cũng sớm học tập triển khai giải pháp này.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080805.webp)

3、[Mỹ phát minh dòng robot đa hình thái có thể bay, chạy và leo trèo linh hoạt](https://www.caltech.edu/about/news/new-bioinspired-robot-flies-rolls-walks-and-more)

Các nhà khoa học tại Viện Công nghệ California (Caltech) vừa qua đã công bố chế tạo thành công mẫu robot di động đa hình thái có khả năng tự động thay đổi phương thức di chuyển tùy thuộc vào địa hình:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062809.webp)

Robot được trang bị hệ thống 4 bánh xe cho phép di chuyển nhanh chóng trên địa hình bằng phẳng tương tự như một chiếc ô tô điều khiển (hình trên).

Khi gặp chướng ngại vật lớn hoặc khe nứt sâu, các khớp nối sẽ tự động lật ngang bánh xe ra, lúc này các cánh quạt ẩn bên trong bánh xe sẽ hoạt động như cánh quạt trực thăng biến robot thành một thiết bị bay không người lái để vượt qua chướng ngại vật:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062810.webp)

Bên cạnh đó, nhờ cơ chế điều khiển độc lập của mỗi bánh xe, robot cũng có khả năng dựng đứng thân mình để di chuyển bằng hai bánh hoặc bò leo qua các bậc thang cao một cách linh hoạt.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062811.webp)

4、[Ả Rập Xê Út công bố dự án xây dựng tòa nhà chọc trời hình khối lập phương khổng lồ Mukaab](https://www.dezeen.com/2023/02/17/cube-skyscraper-riyadh-saudi-arabia-mukaab-murabba/)

Chính phủ Ả Rập Xê Út vừa qua đã công bố bản thiết kế cho dự án xây dựng một tòa nhà chọc trời có dạng hình lập phương khổng lồ mang tên "Mukaab" đặt tại khu đô thị mới của thủ đô Riyadh:

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022605.webp)

Tòa nhà được thiết kế dưới dạng khối lập phương hoàn hảo với chiều dài mỗi cạnh lên tới 400 mét, hứa hẹn sẽ trở thành công trình biểu tượng có chiều cao vượt trội tại thủ đô.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022606.webp)

Toàn bộ phần lõi bên trong của khối lập phương được thiết kế rỗng để bố trí một tòa tháp xoắn ốc khổng lồ mang phong cách kiến trúc nghệ thuật truyền thống của quốc gia.

Xung quanh tòa tháp trung tâm là hệ thống các khu căn hộ cao cấp, trung tâm thương mại và khách sạn sang trọng bám dọc theo thành trong của tòa nhà.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022607.webp)

Theo thiết kế chi tiết, siêu dự án này sẽ cung cấp không gian sinh sống cho 100.000 căn hộ dân cư, 9.000 phòng khách sạn, hơn 980.000 mét vuông khu mua sắm thương mại, 1,4 triệu mét vuông văn phòng làm việc đi kèm 80 khu vui chơi giải trí văn hóa, một trường đại học quốc tế và hệ thống bảo tàng nghệ thuật lớn. Chính phủ Ả Rập Xê Út đặt mục tiêu hoàn thành toàn bộ công trình vào năm 2030.

## Bài viết

1\. [Tác giả Rails framework DHH tuyên bố loại bỏ TypeScript để quay về JavaScript](https://world.hey.com/dhh/turbo-8-is-dropping-typescript-70165c01)（Tiếng Anh）

Nhà lập trình nổi tiếng David Heinemeier Hansson (DHH) – người sáng tạo ra framework Web Ruby on Rails – đã gây xôn xao cộng đồng Front-end khi ra thông báo chính thức loại bỏ hoàn toàn TypeScript khỏi dự án thư viện Turbo 8 của mình để quay lại viết bằng mã nguồn JavaScript thuần túy, bày tỏ quan điểm cá nhân cho rằng sự phức tạp của việc biên dịch kiểu dữ liệu trong TypeScript đang làm giảm tốc độ phát triển dự án.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091806.webp)

2\. [Thống kê các cổng kết nối mạng phổ biến lớn hơn 1024 trong hệ thống Linux](https://matt-rickard.com/de-facto-ports)（Tiếng Anh）

Trong hệ điều hành Linux, các cổng mạng (port) có giá trị nhỏ hơn 1024 được giữ lại mặc định cho các dịch vụ hệ thống cốt lõi sử dụng, các cổng lớn hơn 1024 sẽ do người dùng tự phân bổ. Bài viết tổng hợp danh sách các cổng mạng lớn hơn 1024 đang được các phần mềm dịch vụ phổ biến (như cơ sở dữ liệu, máy chủ web, công cụ cache) chiếm dụng mặc định trong thực tế.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082105.webp)

3\. [Thống kê mức độ phân mảnh kích thước khung hiển thị của trình duyệt web](https://viewports.fyi/)（Tiếng Anh）

Kích thước cửa sổ hiển thị thực tế (Viewport) của các trình duyệt web trong thực tế đa dạng thế nào? Một công ty thiết kế giao diện đã tiến hành thu thập số liệu phân tích và đưa ra kết quả bất ngờ: có tới hơn 2.300 kích thước viewport khác nhau đang được người dùng sử dụng để duyệt web hàng ngày, đòi hỏi các lập trình viên Front-end phải thiết kế giao diện có độ co giãn đáp ứng cực kỳ linh hoạt.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082107.webp)

4\. [Chia sẻ kinh nghiệm gửi thư yêu cầu chuyển đổi tài khoản AWS SES sang chế độ Production](https://tiezhu.wang/posts/aws-ses-production-access/)（Tiếng Trung）

Dịch vụ gửi thư điện tử hàng loạt AWS Simple Email Service (SES) của Amazon mặc định khi khởi tạo sẽ ở chế độ thử nghiệm Sandbox giới hạn tính năng. Để chuyển đổi sang chế độ chạy thực tế (Production), nhà phát triển phải gửi thư giải trình chi tiết mục đích sử dụng. Tác giả bài viết chia sẻ kinh nghiệm viết nội dung thư giải trình giúp tăng tỷ lệ duyệt thành công của Amazon. (Đóng góp của [@tiezhudotwang](https://github.com/ruanyf/weekly/issues/3487))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091512.webp)

5\. [Bài viết phân tích chuyên sâu về kiến trúc kỹ thuật của hệ thống mạng phân tán ZeroNet](https://znano.eu.org/blog/posts/a-very-technical-look-at-zeronet)（Tiếng Anh）

ZeroNet là một mạng lưới phân tán ngang hàng (P2P) cho phép người dùng lưu trữ và duyệt website không cần máy chủ trung tâm. Bài viết đi sâu phân tích cấu trúc kỹ thuật, cách thức đồng bộ hóa dữ liệu giữa các nút mạng và cơ chế bảo mật danh tính của giao thức này dưới góc nhìn dễ hiểu.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071801.webp)

6\. [Hướng dẫn cài đặt và cấu hình ứng dụng phân phối game Steam trên hệ điều hành Arch Linux](https://linuxiac.com/how-to-play-games-on-arch-linux-using-steam/)（Tiếng Anh）

Bài viết hướng dẫn chi tiết từng bước dành cho các game thủ sử dụng hệ điều hành Linux: cách thức kích hoạt các thư viện đồ họa cần thiết, cài đặt bộ driver card màn hình và cấu hình chạy nền tảng Steam để chơi game mượt mà trên hệ điều hành tối giản Arch Linux.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082010.webp)

7\. [Lập trình viên chuyên nghiệp đưa ra so sánh lựa chọn học tập giữa hai ngôn ngữ Rust và Go](https://kerkour.com/should-i-rust-or-should-i-go)（Tiếng Anh）

Tác giả – một chuyên gia có nhiều năm kinh nghiệm lập trình Rust – đã đưa ra nhận định bất ngờ: đối với những người mới bắt đầu học lập trình hệ thống, ngôn ngữ Go là sự lựa chọn phù hợp hơn so với Rust. Một trong những lý do được đưa ra là tốc độ cập nhật phiên bản của Rust quá nhanh (ghi nhận tới 31 bản cập nhật lớn từ năm 2020 đến 2023, trong khi Go chỉ có 8 bản), khiến hệ sinh thái thư viện đi kèm liên tục thay đổi cấu trúc gây khó khăn cho việc học tập lâu dài.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091601.webp)

## 工具

1、[Linkwarden: Công cụ quản lý và lưu trữ dấu trang web nguồn mở tự lưu trữ](https://github.com/linkwarden/linkwarden)

Một phần mềm mã nguồn mở cho phép người dùng tự triển khai một hệ thống quản lý dấu trang (bookmark) cá nhân trên máy chủ của mình, hỗ trợ phân loại thư mục, gắn thẻ tag và tự động lưu lại bản chụp (snapshot) nội dung trang web để xem lại khi link gốc bị lỗi.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080107.webp)

2、[v0: Trình tạo sinh giao diện trang web bằng trí tuệ nhân tạo của Vercel](https://v0.dev/)

Một công cụ thử nghiệm đột phá của hãng Vercel: cho phép người dùng nhập mô tả giao diện mong muốn bằng văn bản, hệ thống AI sẽ tự động thiết kế và sinh ra 3 mẫu giao diện trực quan kèm theo toàn bộ mã nguồn lập trình bằng React và Tailwind CSS tương ứng để tải về. (Đóng góp của [@James-Lam](https://github.com/ruanyf/weekly/issues/3486))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091510.webp)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091511.webp)

3、[Extension Manager: Tiện ích hỗ trợ quản lý nhanh các plugin cài đặt trên trình duyệt](https://github.com/JasonGrass/auto-extension-manager)

Một extension hữu ích giúp người dùng dễ dàng bật, tắt hoặc nhóm lại các tiện ích mở rộng đã cài đặt trên trình duyệt chỉ bằng một cú click chuột từ thanh công cụ, giải quyết các hạn chế hiển thị của trình quản lý mặc định. (Đóng góp của [@JasonGrass](https://github.com/ruanyf/weekly/issues/3500))

4、[讯飞星火 (Xunfei Spark): Mô hình AI hỗ trợ sinh slide trình chiếu và viết CV xin việc](https://passport.xfyun.cn/login)

Mô hình trí tuệ nhân tạo do tập đoàn công nghệ Xunfei phát triển, hỗ trợ người dùng tạo lập nhanh cấu trúc bài trình chiếu slide PPT, tối ưu hóa nội dung CV xin việc và hỗ trợ đọc hiểu phân tích tài liệu văn bản lớn. (Đóng góp của [@huiyanghu12](https://github.com/ruanyf/weekly/issues/3502))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092106.webp)

5、[Subdomain Center: Dịch vụ trực tuyến tìm kiếm toàn bộ tên miền phụ của một website](https://www.subdomain.center/)

Một công cụ web cho phép người dùng nhanh chóng truy vấn và liệt kê toàn bộ các tên miền phụ (subdomains) đang hoạt động của một tên miền bất kỳ phục vụ công tác bảo mật hệ thống. Dự án được [mở nguồn hoàn toàn trên GitHub](https://github.com/ARPSyndicate/puncia).

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091602.webp)

6、[Sqids: Thư viện tạo mã ID rút gọn ngẫu nhiên từ các số nguyên](https://sqids.org/)

Một thư viện mã nguồn mở hữu ích (phát triển thay thế cho thư viện Hashids cũ) hỗ trợ tạo ra các chuỗi ký tự ID rút gọn độc nhất từ các số nguyên (như ID cơ sở dữ liệu) để nhúng vào URL trang web, hỗ trợ hầu hết các ngôn ngữ lập trình phổ biến.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080202.webp)

7、[Webrecorder: Bộ công cụ hỗ trợ tải và lưu trữ tương tác trang web ngoại tuyến](https://webrecorder.net/)

Một giải pháp kỹ thuật giúp người dùng ghi nhận và tải về toàn bộ tài nguyên hiển thị của một trang web động phức tạp để lưu trữ dưới dạng file chuẩn lưu trữ web, giúp tái hiện chính xác giao diện tương tác của trang ngay cả khi thiết bị hoàn toàn không có mạng.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080204.webp)

8、[Reflex: Thư viện lập trình Front-end Web sử dụng hoàn toàn bằng mã Python](https://github.com/reflex-dev/reflex)

Một framework Front-end độc đáo dành riêng cho các lập trình viên Python: cho phép viết mã xây dựng toàn bộ giao diện trang web động và cơ chế tương tác trực tiếp bằng cú pháp Python mà không cần viết bất kỳ dòng mã JavaScript hay HTML nào.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080301.webp)

## IP 地域归属查询

Hai trang web dưới đây cung cấp công cụ trực tuyến tra cứu nhanh thông tin địa lý, nhà mạng và dải IP của một địa chỉ IP bất kỳ:

1、[ipinfo.io](https://ipinfo.io/)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091501.webp)

2、[ipapi.is](https://ipapi.is/)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091502.webp)

Cả hai website này đều hỗ trợ các nhà phát triển tải về phiên bản cơ sở dữ liệu IP địa lý miễn phí để nhúng vào ứng dụng cá nhân chạy offline: [ipinfo database](https://ipinfo.io/developers/ip-to-country-asn-database), [ipapi database](https://ipapi.is/geolocation.html).

## 资源

1、[Ancient Earth: Bản đồ 3D tương tác mô phỏng bề mặt Trái Đất qua các kỷ địa chất](https://dinosaurpictures.org/ancient-earth/)

Một trang web giáo dục khoa học thú vị, cho phép người dùng xoay quả địa cầu 3D để quan sát sự dịch chuyển của các mảng kiến tạo bề mặt Trái Đất qua từng thời kỳ địa chất lịch sử, với dữ liệu nguồn hỗ trợ quay ngược thời gian lên tới 750 triệu năm trước.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050801.webp)

2、[Tài liệu hướng dẫn kỹ thuật chuyển đổi định dạng video từ HDR sang SDR trên Android](https://juejin.cn/post/7205908717886865469)（Tiếng Trung）

Chuỗi bài viết kỹ thuật chia sẻ chi tiết các kiến thức toán học và giải thuật xử lý màu sắc để thực hiện chuyển đổi luồng video dải động cao HDR sang dải động tiêu chuẩn SDR phục vụ phát triển ứng dụng media trên Android. Bạn đọc có thể xem thêm [Mã nguồn thư viện mẫu](https://github.com/JonaNorman/HDRSample). (Đóng góp của [@JonaNorman](https://github.com/ruanyf/weekly/issues/3494))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091805.webp)

3\. [FinChat: Công cụ trí tuệ nhân tạo hỗ trợ phân tích báo cáo tài chính doanh nghiệp](https://finchat.io/)

Ứng dụng web tích hợp mô hình ngôn ngữ lớn hỗ trợ các nhà đầu tư tài chính: tự động thu thập và phân tích nhanh báo cáo tài chính của các công ty niêm yết trên các sàn chứng khoán lớn, hỗ trợ trả lời các câu hỏi so sánh số liệu tài chính trực quan. (Đóng góp của [@Y024](https://github.com/ruanyf/weekly/issues/3495))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092105.webp)

4\. [Pierce through the Laravel: Bộ tài liệu phân tích sâu mã nguồn của Laravel framework](http://www.idocloud.net/pttl/index.html)（Tiếng Trung）

Một bộ tài liệu học tập lập trình web chuyên sâu viết bằng tiếng Trung, đi sâu phân tích cơ chế hoạt động của Service Container, Routing và ORM bên dưới mã nguồn của PHP framework nổi tiếng Laravel. Dự án được [mở nguồn hoàn toàn trên GitHub](https://github.com/youngtrix/pierce_through_the_laravel). (Đóng góp của [@youngtrix](https://github.com/ruanyf/weekly/issues/3504))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092107.webp)

## 图片

1、**Đời sống thực tế bên trong các nhà nhộng ngủ cho thuê giá rẻ tại San Francisco**

Thành phố San Francisco là khu vực có chi phí thuê nhà đắt đỏ bậc nhất nước Mỹ với giá thuê căn hộ một phòng ngủ thông thường dao động từ 3.000 đến 5.000 USD/tháng.

Để tiết kiệm chi phí sinh hoạt khi mới chuyển đến thành phố tìm kiếm cơ hội khởi nghiệp, nhiều lập trình viên trẻ đã lựa chọn giải pháp thuê các buồng ngủ dạng nhộng (capsule) trong một không gian sinh hoạt chung:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091801.webp)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091802.webp)

Mức giá thuê cho một buồng ngủ nhỏ hẹp này là 700 USD/tháng (khoảng 17 triệu đồng). Điểm cộng lớn nhất là khu nhà chung cung cấp không gian phòng khách, bếp ăn và khu làm việc chung rộng rãi, sạch sẽ giúp các nhà phát triển dễ dàng giao lưu kết nối công việc với nhau:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091803.webp)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091804.webp)

2、**Bảng thống kê hình dáng các loại phích cắm và ổ cắm điện chuẩn trên thế giới**

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041901.webp)

## ✍️ Bài đọc thêm

### Phân biệt Quyết định có thể đảo ngược và Quyết định không thể đảo ngược trong cuộc sống

*Bài viết chia sẻ triết lý tư duy ra quyết định của Farnam Street.*

Trong cuộc sống cũng như trong quản trị công việc, các quyết định chúng ta đưa ra hàng ngày thường được chia làm hai nhóm cơ bản:

Nhóm thứ nhất là **Quyết định không thể đảo ngược (Irreversible)**. Những quyết định này giống như một cánh cửa một chiều: một khi bạn đã bước qua thì cánh cửa sẽ khóa lại và bạn hoàn toàn không có cách nào quay trở lại điểm xuất phát được nữa. Chi phí để rút lui hoặc sửa sai của quyết định này là cực kỳ đắt đỏ.

Nhóm thứ hai là **Quyết định có thể đảo ngược (Reversible)**. Những quyết định này hoạt động như một cánh cửa hai chiều: sau khi bước qua, nếu cảm thấy không phù hợp, bạn hoàn toàn có thể dễ dàng bước ngược trở lại. Chi phí để hủy bỏ quyết định là rất thấp.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092109.webp)

Làm thế nào để chúng ta nhận diện nhanh hai nhóm quyết định này?

Điểm mấu chốt nằm ở việc ước tính Chi phí hủy bỏ quyết định. Chi phí hủy bỏ càng cao thì quyết định đó càng thiên về hướng không thể đảo ngược, chi phí càng thấp thì quyết định đó càng dễ dàng đảo ngược.

Bí quyết tư duy được đúc kết là: **Hãy đưa ra quyết định có thể đảo ngược thật nhanh, và đưa ra quyết định không thể đảo ngược thật muộn.**

Đối với các quyết định có thể đảo ngược dễ dàng, rủi ro lớn nhất không phải là quyết định sai mà là sự do dự, kéo dài thời gian làm mất đi thời cơ hành động. Do đó, hãy quyết định thật nhanh chóng.

Đối với các quyết định không thể đảo ngược, rủi ro lớn nhất là đưa ra quyết định sai lầm gây hậu quả nghiêm trọng. Do đó, hãy chủ động làm chậm quy trình ra quyết định lại, dành thêm thời gian để thu thập và phân tích thêm nhiều thông tin hữu ích.

Nhà sáng lập tập đoàn Amazon Jeff Bezos cho rằng: đối với các quyết định không thể đảo ngược, thời điểm thích hợp để bấm nút thực hiện là khi bạn đã nắm chắc khoảng 70% độ tin cậy của kết quả dự báo. Nếu độ tin cậy thấp hơn con số đó, bạn nên tiếp tục kiên nhẫn quan sát và thu thập thêm thông tin.

Tóm lại, sai lầm lớn nhất đối với các quyết định có thể đảo ngược là kéo dài sự do dự cho đến phút cuối cùng, còn sai lầm lớn nhất đối với các quyết định không thể đảo ngược là vội vã đưa ra quyết định trước khi thời khắc bắt buộc ra quyết định thực sự đến.

## Lịch sử tuần này

- 2022年（第 225 期）：[Lối sống số: Thảo luận về việc nghề đóng vai nhân vật phụ (NPC) trong game đang trở thành một nghề nghiệp thực tế](http://www.ruanyifeng.com/blog/2022/09/weekly-issue-225.html)
- 2021年（第 175 期）：[Phát triển cá nhân: Phân tích sự khác biệt và ưu nhược điểm giữa việc tích lũy tri thức rộng và tri thức sâu](http://www.ruanyifeng.com/blog/2021/09/weekly-issue-175.html)
- 2020年（第 125 期）：[Tài chính số: Tìm hiểu mục tiêu thực tế của việc triển khai đồng tiền nhân dân tệ kỹ thuật số](http://www.ruanyifeng.com/blog/2020/09/weekly-issue-125.html)
- 2019年（第 75 期）：[Xã hội học: Quá trình tự động hóa thay thế các thiết bị cơ khí bằng điện tử tác động thế nào tới việc làm](http://www.ruanyifeng.com/blog/2019/09/weekly-issue-75.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge organization and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
