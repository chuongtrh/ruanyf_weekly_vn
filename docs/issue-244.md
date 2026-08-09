# Bản tin chia sẻ công nghệ (Số 244): Dữ liệu lớn (Big Data) đã chết

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2960) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022804.webp)

Tại thị trấn nhỏ Tirau, New Zealand, người dân đã dựng lên rất nhiều công trình kiến trúc độc đáo bằng tôn lượn sóng dọc theo các tuyến đường quốc lộ. Hình ảnh chú chó dễ thương ở trên thực chất là một nhà vệ sinh công cộng dành cho du khách. (Nguồn: [NewZealand.com](https://www.newzealand.com/us/tirau/))

## 本周话题：大数据已死

Thuật ngữ "Dữ liệu lớn" (Big Data) chắc hẳn là một từ khóa vô cùng quen thuộc với tất cả chúng ta. Đây từng là một trong những từ khóa công nghệ phổ biến nhất được toàn xã hội nhiệt tình săn đón.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022203.webp)

Theo dữ liệu từ [Baidu Index](https://index.baidu.com/v2/main/index.html#/trend/%E5%A4%A7%E6%95%B0%E6%8D%AE?words=%E5%A4%A7%E6%95%B0%E6%8D%AE), từ khóa "Big Data" bắt đầu xuất hiện trên các công cụ tìm kiếm từ năm 2011, sau đó nhanh chóng lan rộng và đạt đỉnh điểm trong giai đoạn từ năm 2017 đến năm 2019.

Vào thời điểm đó, giới công nghệ đều tin rằng lượng dữ liệu toàn cầu sẽ tăng trưởng theo cấp số nhân trong tương lai và nhân loại sẽ bị nhấn chìm trong biển dữ liệu khổng lồ. Việc xử lý hiệu quả lượng dữ liệu lớn này được coi là chìa khóa vàng quyết định năng lực cạnh tranh của mỗi doanh nghiệp và thậm chí là của mỗi quốc gia trong kỷ nguyên thông tin.

Vì lẽ đó, các doanh nghiệp đổ xô đi tìm kiếm các giải pháp xử lý dữ liệu lớn, tạo ra làn sóng tuyển dụng kỹ sư Big Data với mức lương cực kỳ hấp dẫn. Các trường đại học cũng nhanh chóng bắt kịp xu hướng: số liệu thống kê cho thấy có hơn 600 trường đại học tại Trung Quốc đã thành lập chuyên ngành hoặc khoa đào tạo chuyên sâu về "Dữ liệu lớn", bao gồm cả các trường đại học danh tiếng hàng đầu như Đại học Bắc Kinh hay Đại học Phục Đán.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022204.webp)

Thế nhưng, mười năm trôi qua, dữ liệu lớn chưa bao giờ thực sự trở thành nút thắt cổ chai cản trở sự phát triển của công nghệ. Năng lực xử lý của máy tính hiện tại hoàn toàn đủ sức giải quyết gọn gàng mọi lượng dữ liệu phát sinh hàng ngày, và dự kiến điều này vẫn sẽ tiếp tục đúng trong tương lai gần.

**Kỷ nguyên dữ liệu lớn được dự báo trước đây dường như không những không đến, mà ngày càng trở nên xa vời.** Độ nóng của thuật ngữ "Big Data" liên tục giảm nhiệt, tần suất được nhắc đến ít đi và các vị trí tuyển dụng liên quan cũng thưa thớt dần.

Đồng thời, bản thân mảng công nghệ Big Data cũng rơi vào trạng thái phát triển chậm chạp, không có thêm các khái niệm hay lý thuyết đột phá mới ra đời và nhiều hướng nghiên cứu kỹ thuật rơi vào bế tắc.

Ví dụ điển hình là các hệ cơ sở dữ liệu NoSQL (được thiết kế riêng để xử lý lượng dữ liệu lớn) đang ngày càng hạ nhiệt và chững lại. Ngược lại, các hệ cơ sở dữ liệu quan hệ truyền thống như SQLite, PostgreSQL và MySQL lại đang trỗi dậy mạnh mẽ và ngày càng được cộng đồng lập trình viên ưa chuộng.

Tại sao lại có hiện tượng ngược dòng này xảy ra?

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022808.webp)

Jordan Tigani, một cựu kỹ sư dữ liệu lớn của Google, mới đây đã thẳng thắn tuyên bố trong một bài viết gây chú ý: "[Dữ liệu lớn đã chết](https://motherduck.com/blog/big-data-is-dead/)".

Quan điểm của ông là **kỷ nguyên dữ liệu lớn đã kết thúc vì các vấn đề về lưu trữ và phân tích dữ liệu quy mô lớn về mặt kỹ thuật cơ bản đã được giải quyết triệt để.** Người dùng không còn phải lo lắng quá nhiều về kích thước dữ liệu nữa, mọi khối lượng dữ liệu phát sinh hiện nay đều không còn là rào cản quá lớn.

Jordan Tigani đã đưa ra 6 luận điểm rất thuyết phục để chứng minh cho nhận định này của mình:

1. **Hầu hết các doanh nghiệp không có dữ liệu thực sự lớn**: Lượng dữ liệu tích lũy thực tế của đại đa số doanh nghiệp hiện nay thường nhỏ hơn 1 TB, thậm chí có rất nhiều doanh nghiệp chỉ sở hữu dưới 100 GB dữ liệu. Giả sử một doanh nghiệp sản xuất quy mô trung bình có 1.000 khách hàng hoạt động, mỗi khách hàng phát sinh 1 đơn hàng/ngày và mỗi đơn hàng chứa 100 sản phẩm. Lượng dữ liệu phát sinh mỗi ngày của doanh nghiệp này vẫn nhỏ hơn 1 MB rất nhiều. Sau 3 năm hoạt động, tổng lượng dữ liệu thu được chỉ khoảng 1 GB, và họ sẽ cần tới hàng ngàn năm để tích lũy được 1 TB dữ liệu. Ngay cả các tập đoàn internet lớn khi chạy các chiến dịch marketing cho hàng triệu người dùng tham gia đồng thời thì lượng dữ liệu thô phát sinh hàng ngày cũng khó vượt quá vài GB, khoảng cách còn rất xa so với định nghĩa dữ liệu lớn.
2. **Sự tách biệt hoàn toàn giữa lưu trữ và tính toán**: Khái niệm dữ liệu lớn bao gồm hai khía cạnh độc lập: "Lưu trữ dữ liệu" (Storage) và "Tính toán xử lý dữ liệu" (Compute). Việc xử lý chung hai tác vụ này trên cùng một hệ thống vật lý trước đây là rất khó khăn. Tuy nhiên, kiến trúc đám mây hiện đại đã tách biệt hoàn toàn hai mảng này thành hai hệ thống độc lập hoạt động riêng rẽ và có thể mở rộng quy mô (scale) một cách độc lập. Do đó bài toán dữ liệu lớn đã được chia nhỏ thành hai bài toán đơn giản hơn: lưu trữ dung lượng lớn và năng lực tính toán hiệu năng cao.
3. **Nếu không phát sinh mảng kinh doanh mới, dữ liệu chỉ tăng trưởng tuyến tính**: Tốc độ tăng dữ liệu hàng ngày thường có cấu trúc ổn định tương đương các ngày trước đó. Dữ liệu cũ sau khi ghi vào cơ sở dữ liệu hầu như không bao giờ thay đổi và các tác vụ tính toán phân tích liên quan đến nó cũng đã được hoàn thành trước đó. Hệ thống chỉ cần chạy các truy vấn tính toán riêng biệt cho phần dữ liệu mới phát sinh hàng ngày rồi lưu lại kết quả. Rất hiếm khi một doanh nghiệp cần quét và tính toán lại toàn bộ dữ liệu lịch sử hàng ngày: những dữ liệu đó là cố định, tại sao lại phải lãng phí tài nguyên tính toán lặp đi lặp lại chúng?
4. **Người ta thường chỉ quan tâm đến dữ liệu phát sinh gần nhất**: Hầu hết các truy vấn phân tích của doanh nghiệp đều tập trung vào lượng dữ liệu phát sinh trong vòng 24 giờ qua. Tần suất truy vấn đối với dữ liệu từ một tuần trước thấp hơn tới 20 lần, và dữ liệu lịch sử từ một tháng trước hầu như chỉ được truy cập rất hạn chế. Điều này đồng nghĩa với việc dữ liệu lớn hoạt động như dữ liệu tĩnh nhiều hơn là động. Vì dữ liệu cũ ít khi sử dụng đến, chúng ta có thể nén chúng lại để lưu trữ lâu dài. Một bảng dữ liệu tích lũy 10 năm của doanh nghiệp có thể nặng tới cấp độ PB, nhưng nếu tiến hành nén dữ liệu lịch sử thì dung lượng thực tế lưu trên đĩa cứng có thể giảm xuống dưới 50 GB.
5. **Các doanh nghiệp sở hữu dữ liệu lớn thực sự cũng rất hiếm khi truy vấn toàn bộ dữ liệu**: Hơn 90% các câu lệnh truy vấn phân tích chỉ chạy trên các phân vùng dữ liệu có dung lượng nhỏ hơn 100 MB. Các truy vấn chạy trên toàn bộ tập dữ liệu cấp độ TB là cực kỳ hiếm hoi. Việc chạy truy vấn trên toàn bộ tập dữ liệu khổng lồ cũng vô cùng đắt đỏ: ví dụ dịch vụ BigQuery của Google tính phí tới 5.000 USD cho một câu lệnh quét dữ liệu cấp độ PB, ngay cả các doanh nghiệp lớn cũng sẽ cân nhắc kỹ tần suất thực hiện các tác vụ này.
6. **Sự phát triển vượt bậc của phần cứng máy tính đơn lẻ**: Vào năm 2004 khi Google công bố bài báo khoa học về giải thuật MapReduce, năng lực tính toán của một máy chủ đơn lẻ lúc đó còn rất yếu nên bắt buộc phải chia nhỏ tác vụ để chạy phân tán trên hàng ngàn máy tính. Vào năm 2006 khi AWS ra mắt dịch vụ đám mây EC2, cấu hình máy ảo cơ bản chỉ có 1 core CPU và 2 GB RAM. Ngày nay, cấu hình máy chủ tiêu chuẩn của AWS đã lên tới 64 cores và 256 GB RAM. Nếu chấp nhận chi phí cao, doanh nghiệp có thể thuê các máy chủ khủng sở hữu tới 445 cores và hơn 24 TB RAM. Năng lực xử lý cực mạnh của một máy chủ đơn lẻ giúp giải quyết phần lớn các tác vụ xử lý dữ liệu lớn mà không cần đến các hệ thống tính toán phân tán phức tạp khó vận hành.

Tóm lại, thông điệp cốt lõi là: **Dung lượng dữ liệu không còn là vấn đề đau đầu đối với các nhà phát triển nữa, việc xử lý lượng dữ liệu khổng lồ đã không còn là rào cản kỹ thuật khó vượt qua.** Big Data với tư cách là một bài toán công nghệ thách thức cơ bản đã được giải quyết trọn vẹn.

## Tin tức công nghệ

1、[Show diễn thời trang độc đáo dành cho người cao tuổi được dựng hoàn toàn bằng AI](https://mymodernmet.com/malik-afegbua-fashion-show-for-elders/)

Một nghệ sĩ người châu Phi đã ứng dụng công nghệ AI để tạo ra hình ảnh một buổi trình diễn thời trang vô cùng ấn tượng:

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022601.webp)

Anh đã gửi các mô tả chi tiết yêu cầu AI vẽ hình ảnh các cụ ông, cụ bà người châu Phi mặc các bộ trang phục truyền thống rực rỡ tự tin sải bước trên sàn catwalk. Sau nhiều lần tinh chỉnh từ khóa, kết quả thu được vô cùng hoàn hảo và chân thực:

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022602.webp)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022603.webp)

Thực tế đời sống cho thấy việc quy tụ được dàn người mẫu lớn tuổi và chuẩn bị các bộ trang phục thiết kế kỳ công như thế này ngoài đời thực là cực kỳ khó khăn với chi phí vô cùng đắt đỏ. Show diễn thời trang ảo bằng AI này hứa hẹn sẽ mang lại những thay đổi lớn cho ngành công nghiệp thời trang tương lai, tác động trực tiếp tới công việc của giới người mẫu truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022604.webp)

2、[Nghiên cứu về tốc độ phát tán sol khí của bồn cầu khi xả nước](https://www.colorado.edu/today/2022/12/08/cu-scientists-shine-light-what-comes-when-you-flush)

Các chuyên gia y tế công cộng từ lâu đã cảnh báo việc xả nước bồn cầu không đậy nắp sẽ tạo ra các hạt sol khí (aerosol) li ti phát tán mầm bệnh vào không khí, nhưng chưa có nghiên cứu trực quan nào ghi nhận được tốc độ và phạm vi phát tán cụ thể của chúng.

Đội ngũ kỹ sư tại Đại học Colorado đã sử dụng hệ thống tia laser xanh công suất lớn kết hợp cùng camera quay tốc độ cao để ghi hình lại quá trình xả nước bồn cầu:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120821.webp)

Kết quả thực nghiệm cho thấy ngay khi nhấn nút xả nước, các hạt nước li ti lập tức bắn ra ngoài với vận tốc lên tới 2 m/s và bay cao tới 1,5m phía trên bồn cầu. Các hạt nước lớn sẽ nhanh chóng rơi xuống bám vào các bề mặt xung quanh chỉ sau vài giây, nhưng các hạt bụi nước li ti (sol khí) siêu nhỏ có thể tiếp tục lơ lửng trong không khí nhà vệ sinh suốt nhiều phút hoặc lâu hơn.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120822.webp)

3、[Tác phẩm nghệ thuật vẽ tranh bằng GPS lớn nhất thế giới trên bản đồ](https://interestingengineering.com/culture/man-travels-4000-miles-marriage)

Nhiều người có sở thích di chuyển tạo ra các đường vẽ lộ trình chạy ngầm trên bản đồ Google Maps dựa theo tín hiệu định vị GPS, loại hình này được gọi là nghệ thuật GPS.

Một người đàn ông Nhật Bản đã quyết định thực hiện một lộ trình di chuyển đặc biệt trên bản đồ nước Nhật để cầu hôn bạn gái của mình:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120901.webp)

Anh đã tự lái xe liên tục suốt 6 tháng, đi qua hành trình dài tổng cộng 7.163 km kéo dài từ hòn đảo Hokkaido phía bắc tới tận tỉnh Kagoshima ở cực nam nước Nhật để vẽ nên dòng chữ "Marry Me" khổng lồ kèm hình trái tim bị mũi tên tình yêu xuyên qua. Tác phẩm đã được kỷ lục Guinness ghi nhận là tác phẩm nghệ thuật GPS có kích thước lớn nhất thế giới.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120902.webp)

4、[Trình diễn dòng chảy dung nham núi lửa nhân tạo độc đáo tại Iceland](https://phys.org/news/2022-12-lava-iceland-volcano.html)

Một nhà hát tại thủ đô Reykjavik, Iceland đã tổ chức một chương trình biểu diễn đặc biệt cho phép du khách ngắm nhìn trực tiếp dòng dung nham núi lửa nóng chảy ngay trong khán phòng:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120904.webp)

Ban tổ chức đã thu gom hơn 600 kg dung nham tự nhiên nguội lạnh từ vụ phun trào núi lửa năm 1918 để làm nguyên liệu. Khối dung nham này được nung nóng lại đến điểm nóng chảy ở nhiệt độ 1.100 độ C để hóa lỏng thành dòng magma đỏ rực chảy dọc theo máng trượt kim loại trước sự chứng kiến của du khách.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120905.webp)

Dung nham núi lửa tự nhiên thường chứa nhiều khí lưu huỳnh có độc tính cao, nhưng do khối dung nham này đã trải qua quá trình nguội lạnh và nung nóng lại nhiều lần nên toàn bộ lượng khí độc đã bay hơi hết, bảo đảm an toàn tuyệt đối cho người xem trong phòng kín.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120906.webp)

## Bài viết

1\. [Hướng dẫn chi tiết quy trình tự thiết lập trang blog cá nhân của tôi](https://www.joshwcomeau.com/blog/how-i-built-my-blog/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122702.webp)

Tác giả chia sẻ chi tiết về kiến trúc mã nguồn trang blog cá nhân của mình sử dụng framework Next.js kết hợp cùng các công cụ React, hướng dẫn cách thức sử dụng định dạng MDX để chèn các component React động vào bên trong các bài viết viết bằng Markdown.

2\. [Đánh giá chặng đường một năm ra mắt của máy chơi game cầm tay Steam Deck](https://boilingsteam.com/steam-deck-first-anniversary-of-the-ultimate-gaming-platform/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022801.webp)

Bài viết nhìn lại chặng đường phát triển sau một năm chính thức mở bán dòng máy chơi game cầm tay Steam Deck của Valve, phân tích các cải tiến quan trọng về mặt tối ưu hóa hệ điều hành SteamOS giúp nâng cao hiệu năng trải nghiệm game.

3\. [Hướng dẫn cấu hình trình soạn thảo nano trên máy chủ Linux](https://ariadne.space/2021/08/13/gnu-nano-is-my-editor-of-choice/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122805.webp)

Mặc dù trình soạn thảo nano thường bị đánh giá là có tính năng đơn giản so với Vim, tác giả hướng dẫn cách thức cấu hình tệp tin `.nanorc` để bổ sung tính năng highlight cú pháp, tự động thụt lề và hiển thị số dòng giúp nano trở nên tiện dụng hơn.

4\. [Stripe ứng dụng định dạng Markdoc để xây dựng tài liệu tương tác](https://stripe.com/blog/markdoc)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022091603.webp)

Bài viết từ đội ngũ phát triển Stripe giới thiệu về Markdoc – một phần mở rộng cú pháp của Markdown do họ tự phát triển cho phép tích hợp trực tiếp các components giao diện tương tác vào tài liệu kỹ thuật của lập trình viên.

5\. [Tìm hiểu chi tiết các định dạng biểu diễn màu sắc trong CSS](https://www.joshwcomeau.com/css/color-formats/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022123102.webp)

Bài phân tích chi tiết của Josh W. Comeau giải thích sự khác biệt giữa các định dạng màu sắc thông dụng trong CSS như Hex, RGB, HSL và định dạng LCH/OKLCH mới, giúp lập trình viên hiểu sâu cách trình duyệt xử lý không gian màu sắc.

6\. [Sử dụng ClickHouse để truy vấn phân tích dữ liệu lịch sử GitHub](https://til.simonwillison.net/clickhouse/github-explorer)（Tiếng Anh）

Hướng dẫn kết nối và thực hiện các câu lệnh truy vấn phân tích SQL tốc độ cao trên trang chạy thử trực tuyến của ClickHouse để khai thác kho dữ liệu lịch sử chứa hơn 3,1 tỷ bản ghi sự kiện hoạt động của lập trình viên trên GitHub từ năm 2011 đến nay.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010201.webp)

7\. [Giải thích cơ chế hoạt động của giao thức HTTPS qua hình ảnh bồ câu đưa thư](https://baida.dev/articles/https-explained-with-carrier-pigeons)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010303.webp)

Bài viết phổ biến kiến thức mạng máy tính cực kỳ sáng tạo: sử dụng hình ảnh ẩn dụ về việc gửi thư bằng bồ câu để giải thích rõ ràng các khái niệm phức tạp của giao thức mã hóa HTTPS như khóa công khai, khóa bí mật và chứng chỉ số CA.

8\. [Windows 11 lưu giữ bao nhiêu thế hệ giao diện người dùng cũ?](https://ntdotdev.wordpress.com/2023/01/01/state-of-the-windows-how-many-layers-of-ui-inconsistencies-are-in-windows-11/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010302.webp)

Tác giả thực hiện khảo sát sâu bên trong các cửa sổ cấu hình của hệ điều hành Windows 11 và vạch trần sự bất nhất về mặt thiết kế giao diện khi hệ thống vẫn lưu giữ nguyên vẹn nhiều cửa sổ cài đặt kế thừa từ thời Windows XP, Windows 2000 và thậm chí là Windows 3.1.

## Công cụ

1、[kill-sticky: Script bookmarklet xóa nhanh các thành phần sticky che khuất màn hình](https://github.com/t-mart/kill-sticky)

Đoạn mã JavaScript nhỏ lưu dưới dạng bookmarklet trình duyệt giúp người dùng nhấp nhanh để loại bỏ các thanh menu cố định (sticky headers), banner quảng cáo bám đuổi màn hình gây khó chịu khi đọc báo. (Xem thêm công cụ tương tự là [unsticky](https://github.com/nothingless/unsticky)).

2、[MuJing (幕境): Phần mềm hỗ trợ học tiếng Anh qua phụ đề video](https://github.com/tangshimin/MuJing)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022806.webp)

Ứng dụng hỗ trợ người học tiếng Anh bằng cách phân tích tệp video và file phụ đề đi kèm để tự động trích xuất từ vựng mới. Khi xem phim, các từ vựng này sẽ tự động xuất hiện định nghĩa tiếng Trung dưới dạng phụ đề chạy (danmaku) để người dùng ghi nhớ. (Đóng góp của [@tangshimin](https://github.com/ruanyf/weekly/issues/2936))

3、[Quickly Picture Bed: Hệ thống quản lý kho lưu trữ ảnh trực tuyến gọn nhẹ](https://github.com/ischenliang/quickly-picture-bed)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022805.webp)

Mã nguồn mở xây dựng ứng dụng quản trị hình ảnh (圖床) chạy trên nền tảng web hỗ trợ kéo thả tải ảnh nhanh và sinh liên kết Markdown chèn vào bài viết. (Đóng góp của [@it-chenliang](https://github.com/ruanyf/weekly/issues/2937))

4、[Datasette: Công cụ trực quan hóa và khai thác cơ sở dữ liệu SQLite](https://datasette.io/)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022807.webp)

Công cụ nguồn mở hữu ích cho phép người dùng nhanh chóng nạp các tệp tin cơ sở dữ liệu SQLite lên giao diện web để thực hiện các truy vấn dữ liệu, sinh biểu đồ thống kê trực quan hoặc kết xuất dữ liệu qua API. (Đóng góp của [@jerrylususu](https://github.com/ruanyf/weekly/issues/2950))

5、[DrissionPage: Thư viện Python hỗ trợ tự động hóa trình duyệt tinh gọn](https://github.com/g1879/DrissionPage)

Thư viện Python hỗ trợ viết kịch bản tự động hóa thao tác trên trang web, tích hợp cả cơ chế request HTTP tốc độ cao và cơ chế điều khiển trình duyệt Chromium giúp tăng hiệu suất cào dữ liệu (crawling) so với Selenium. (Đóng góp của [@g1879](https://github.com/ruanyf/weekly/issues/2946))

6、[git-hours: Công cụ dòng lệnh ước tính tổng thời gian phát triển dự án Git](https://github.com/kimmobrunfeldt/git-hours)

Tiện ích Node.js dòng lệnh giúp quét lịch sử commit của kho chứa Git để tự động phân tích khoảng thời gian giữa các commit và đưa ra con số ước tính tổng số giờ code mà các kỹ sư đã đầu tư cho dự án.

7、[Manticore Search: Hệ thống tìm kiếm toàn văn nguồn mở tốc độ cao](https://github.com/manticoresoftware/manticoresearch)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072904.webp)

Hệ thống cơ sở dữ liệu tìm kiếm toàn văn (full-text search engine) nguồn mở tốc độ cao, hỗ trợ tốt các ngôn ngữ đa phân đoạn như tiếng Trung, được thiết kế nhằm thay thế cho Elasticsearch với mức tiêu thụ tài nguyên phần cứng thấp hơn.

8、[Unsilence: Tiện ích CLI tự động lọc bỏ các đoạn im lặng trong video](https://github.com/lagmoellertim/unsilence)

Công cụ dòng lệnh hỗ trợ người biên tập video tự động quét file âm thanh và cắt bỏ các phân đoạn im lặng không có tiếng nói trong các video ghi hình bài giảng hoặc thuyết trình để video trở nên liền mạch hơn.

9、[Tabler: Framework UI xây dựng giao diện Dashboard dựa trên Bootstrap](https://github.com/tabler/tabler)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072905.webp)

Bộ mã nguồn cung cấp các thành phần giao diện (UI components) được thiết kế hiện đại, đồng bộ chạy trên nền tảng Bootstrap giúp lập trình viên nhanh chóng xây dựng các trang quản trị Admin Dashboard chuyên nghiệp.

10、[Code Language Converter: Tiện ích chuyển đổi mã nguồn giữa các ngôn ngữ lập trình](https://codelanguageconverter.com/)

Ứng dụng web trực tuyến hỗ trợ chuyển đổi cú pháp mã nguồn tự động từ ngôn ngữ này sang ngôn ngữ khác (ví dụ chuyển đổi JavaScript sang PHP hoặc Python) (dịch vụ trả phí kèm gói dùng thử miễn phí).

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022093005.webp)

11、[VueTube: Ứng dụng khách xem Youtube nguồn mở dành cho di động](https://github.com/VueTubeApp/VueTube)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100102.webp)

Dự án phát triển ứng dụng khách (client app) thay thế cho trình xem Youtube chính thức trên hệ điều hành Android và iOS, được viết bằng Vue.js chú trọng bảo mật quyền riêng tư.

## 资源

1、[CSS Bed: Kho tổng hợp các CSS frameworks tối giản không dùng class](https://www.cssbed.com/)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022091111.webp)

Trang web tổng hợp và chạy thử trực quan hàng chục thư viện Classless CSS frameworks tối giản (như Water.css, Sakura.css) hỗ trợ lập trình viên nhanh chóng làm đẹp trang HTML gốc mà không cần viết class.

2、[Sách hướng dẫn lập trình ngôn ngữ C chính thức của dự án GNU](https://lists.gnu.org/archive/html/info-gnu/2022-09/msg00005.html)

Tài liệu hướng dẫn học lập trình ngôn ngữ C do huyền thoại Richard Stallman biên soạn chính thức được phát hành. Người dùng có thể tải phiên bản PDF được chuyển đổi sẵn tại [Kho chứa GitHub GNU C Manual](https://github.com/VernonGrant/gnu-c-language-manual).

3、[Atkinson Hyperlegible: Bộ phông chữ tiếng Anh tăng khả năng đọc hiểu](https://brailleinstitute.org/freefont)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022091201.webp)

Bộ phông chữ tiếng Anh được thiết kế bởi Viện chữ nổi Braille dành cho những người có thị lực kém, tập trung làm rõ nét các ký tự dễ gây nhầm lẫn như chữ số `1` với chữ `I` in hoa, hay chữ `l` viết thường với chữ `i`.

4、[Practical Python: Giáo trình học lập trình Python thực hành tinh gọn](https://dabeaz-course.github.io/practical-python/Notes/Contents.html)

Khóa học trực tuyến chất lượng cao được thiết kế theo dạng các bài thực hành ngắn giúp lập trình viên nhanh chóng nắm bắt các kiến thức cốt lõi của ngôn ngữ Python.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121001.webp)

## 图片

1\. **Bộ ảnh chân dung phong cách hoạt hình Pixar của các vị tổng thống Mỹ**

Một nhà báo Mỹ đã chia sẻ bộ ảnh chân dung độc đáo của các vị tổng thống Mỹ trong lịch sử được vẽ lại theo phong cách hoạt hình 3D của hãng Pixar bằng công nghệ AI:

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022502.webp)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022503.webp)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022504.webp)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022505.webp)

2\. **Hiện trạng quy hoạch chắp vá "Brussels hóa" trong kiến trúc đô thị**

Vào thập niên 1960 và 1970, thủ đô Brussels của Bỉ đã áp dụng chính sách quy hoạch đô thị tự do thiếu kiểm soát, cho phép xây dựng tràn lan các tòa tháp cao tầng hiện đại xen kẽ ngay trong các khu phố cổ truyền thống:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022091102.webp)

Cảnh tượng các tòa nhà kính chọc trời mọc lên hoàn toàn ngẫu nhiên phá vỡ cảnh quan kiến trúc lịch sử đồng bộ của khu phố cổ. Sau này trong ngành kiến trúc, thuật ngữ "Brusselization" (Brussels hóa) đã được sử dụng rộng rãi để chỉ những sai lầm trong công tác quy hoạch đô thị chắp vá làm hỏng cảnh quan.

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022091103.webp)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022091104.webp)

## ✍️ Bài đọc thêm

### Nhật ký anh hùng tắt lò phản ứng hạt nhân trên tàu ngầm K-219 của Liên Xô

Tàu ngầm K-219 là một trong những tàu ngầm hạt nhân chiến lược của Hải quân Liên Xô có khả năng mang theo 16 tên lửa đạn đạo tầm xa trang bị từ 32 đến 48 đầu đạn hạt nhân.

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022091105.webp)

Vào thứ Sáu ngày 3 tháng 10 năm 1986, khi tàu ngầm đang di chuyển tuần tra trên Đại Tây Dương, một ống phóng tên lửa bất ngờ gặp sự cố rò rỉ nhiên liệu dẫn đến một vụ nổ lớn và hỏa hoạn bùng lên. Phía Liên Xô sau đó tuyên bố vụ tai nạn xảy ra do va chạm ngầm với một tàu ngầm của Mỹ, tuy nhiên phía Hải quân Mỹ đã bác bỏ thông tin này.

Vụ nổ ban đầu đã cướp đi sinh mạng của hai thủy thủ ngay tại chỗ và một thủy thủ khác tử vong sau đó do hít phải khí độc từ đám cháy. Nghiêm trọng hơn, vụ nổ làm thủng vỏ tàu khiến nước biển tràn vào khoang làm tàu ngầm mất kiểm soát, rơi tự do từ độ sâu 40m xuống 300m dưới lòng biển.

Để ngăn chặn nước tiếp tục tràn sang các khu vực khác, thuyền trưởng buộc phải ra lệnh đóng chặt toàn bộ các cửa ngăn nước giữa các khoang cách ly. Hành động này khiến 25 thủy thủ bị mắc kẹt hoàn toàn bên trong một khoang kín chứa đầy khí độc. Sau cuộc họp khẩn cấp, thuyền trưởng quyết định mạo hiểm mở cửa khoang cách ly để giải cứu họ ra ngoài.

Tuy nhiên mối nguy hiểm lớn nhất lúc này là lò phản ứng hạt nhân của tàu ngầm không thể tự động ngắt hoạt động do hệ thống điều khiển bị phá hủy sau vụ nổ. Nếu lò phản ứng tiếp tục hoạt động quá nhiệt không có nước làm mát, một thảm họa hạt nhân hủy diệt sẽ xảy ra ngay trên biển. Nhiệt độ bên trong khoang lò phản ứng lúc đó đã vượt quá 60 độ C và chứa đầy khói axit nitric cực độc. Bắt buộc phải có người tình nguyện đi vào bên trong khoang lò để hạ các thanh điều khiển hấp thụ nơ-ron bằng tay nhằm đóng lò phản ứng khẩn cấp.

Người lính đầu tiên đi vào khoang lò phản ứng chỉ mới hạ được một thanh điều khiển (trong tổng số 4 thanh) thì bình dưỡng khí đã cạn kiệt, anh phải lết ra ngoài và ngất lịm ngay tại cửa khoang.

Lúc này, Sergey Preminin – một người lính trẻ mới 20 tuổi – đã tình nguyện đi vào để hoàn thành nhiệm vụ còn dang dở. Khoác lên mình bộ đồ phòng hóa dày cộp, anh dũng cảm bước vào khoang lò nóng rực và thực hiện hạ thành công toàn bộ các thanh điều khiển còn lại để đóng cửa lò phản ứng an toàn.

Thế nhưng, nhiệt độ quá cao bên trong phòng lò đã làm tăng áp suất không khí chênh lệch lớn giữa hai bên cửa khoang cách ly. Áp suất khí nén khổng lồ khiến Sergey Preminin không thể dùng sức đẩy cánh cửa thép để trở ra ngoài, và anh đã hy sinh vì ngạt khí ngay bên trong khoang lò phản ứng sau khi cứu sống toàn bộ đồng đội. Anh đã được truy phong danh hiệu Anh hùng Liên bang Nga vì hành động quả cảm này.

Sau khi đóng lò phản ứng hạt nhân thành công, tàu ngầm K-219 mất hoàn toàn động lực và phải nổi lên mặt nước bằng nguồn điện ắc quy dự phòng. Phía Liên Xô đã điều động một tàu chở hàng đến để lai dắt chiếc tàu ngầm gặp nạn về cảng. Tuy nhiên do lượng nước tràn vào quá lớn không thể khắc phục, vào ngày 6 tháng 10 năm 1986, toàn bộ thủy thủ đoàn được lệnh di tản khẩn cấp trước khi con tàu cùng toàn bộ vũ khí hạt nhân chìm sâu xuống đáy biển Đại Tây Dương ở độ sâu 6.000m.

## Lịch sử tuần này

- 2022年（第 197 期）：[Triết lý cuộc sống: Thảo luận giả định về chiếc máy tạo cảm giác hạnh phúc nhân tạo cho con người](http://www.ruanyifeng.com/blog/2022/03/weekly-issue-197.html)
- 2021年（第 147 期）：[Định hướng cuộc sống: Lời khuyên về việc chủ động tìm kiếm những thử thách khó khăn mà bạn sẵn sàng chấp nhận](http://www.ruanyifeng.com/blog/2021/02/weekly-issue-147.html)
- 2020年（第 95 期）：[Văn hóa doanh nghiệp: Phân tích thực tế của việc làm việc từ xa giúp ban quản lý nhận diện các vị trí thừa thãi](http://www.ruanyifeng.com/blog/2020/02/weekly-issue-95.html)
- 2019年（第 45 期）：[Giới thiệu tác phẩm: Trích dẫn và cảm nhận từ cuốn hồi ký tự truyện *Con đường cuộc sống* của nhà văn Isaac Asimov](http://www.ruanyifeng.com/blog/2019/03/weekly-issue-45.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
