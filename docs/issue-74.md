# 科技爱好者周刊：第 74 期 (Bản tin chia sẻ công nghệ số 74)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091910.jpg)

Ảnh bìa: Giải vô địch bóng rổ thế giới FIBA, Trung tâm Thể thao Phương Đông Thượng Hải, 2019.

## 刊首语 (Lời tựa)

Mọi người có nhận thấy rằng các tài nguyên miễn phí trên mạng internet ngày càng trở nên khan hiếm hay không?

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091908.jpg)

Khi mở rất nhiều trang web hay ứng dụng di động, hệ thống đều yêu cầu bạn phải trả phí: nghe nhạc mất tiền, xem video mất tiền, tải tài liệu mất tiền và đọc một bài viết chuyên sâu cũng mất tiền. Điều này đương nhiên là hợp lý để bảo vệ bản quyền, nhưng tôi luôn cho rằng **mô hình thu phí thuần túy dựa trên nội dung thông tin (information paywall) không phải là một mô hình kinh doanh bền vững, trừ khi nó đi kèm các dịch vụ giá trị gia tăng.** Có hai lý do lớn cho nhận định này.

Lý do thứ nhất là thông tin mang bản chất khác biệt hoàn toàn so với hàng hóa vật lý. Hàng hóa vật lý có tính chất loại trừ (excludability) - nếu tôi ăn quả táo này thì người khác sẽ không thể ăn nó được nữa, nhưng thông tin thì có thể được tiêu dùng vô số lần bởi vô số người mà không bị hao mòn.

Hơn thế nữa, thông tin sở hữu một đặc tính rất kỳ lạ: càng có nhiều người tiếp cận và tiêu dùng, giá trị của nó lại càng tăng cao. Một bài viết chỉ có vài chục người đọc sẽ nhanh chóng bị lãng quên; nhưng nếu có hàng triệu người cùng đọc, nó sẽ lập tức biến thành chủ đề thảo luận nóng hổi của cả quốc gia. **Việc dựng rào cản thu phí vô hình trung sẽ ngăn chặn quá trình tự tăng trưởng giá trị với chi phí bằng không này của thông tin.**

Lý do thứ hai là mô hình thu phí thông tin rất khó mở rộng quy mô. Khoảng 80% người dùng ghé thăm một trang web chỉ đọc lướt qua rồi rời đi ngay, **rào cản thu phí sẽ chặn đứng nhóm người dùng phổ thông này.** Ví dụ, trang tin của tờ *The New York Times* áp dụng mô hình thu phí đọc bài, nhưng do tôi chỉ có nhu cầu đọc vài bài viết ngẫu nhiên mỗi tháng nên khả năng tôi đăng ký gói thuê bao tháng của họ là cực kỳ thấp. Mô hình thu phí đọc tin chỉ hoạt động hiệu quả khi người dùng có nhu cầu sử dụng dịch vụ sâu sắc và lâu dài - nhóm khách hàng trung thành này rất khó tìm kiếm, do đó mô hình kinh doanh này rất khó tăng trưởng quy mô.

Vì vậy, tôi cho rằng **mô hình kinh doanh thông tin tối ưu không phải là dựng rào thu phí, mà là khuyến khích càng nhiều người tiếp cận tiêu dùng nó càng tốt.** Càng nhiều người đọc, giá trị lan tỏa của thông tin càng lớn, và đây chính là tiền đề để doanh nghiệp phát triển các dịch vụ giá trị gia tăng để tạo ra doanh thu từ dịch vụ đi kèm.

Phần mềm mã nguồn mở là minh chứng rõ nét nhất. Hệ điều hành Linux ban đầu chỉ là một dự án cá nhân phi lợi nhuận của một sinh viên đại học cho phép tải về sử dụng tự do, nhưng kết quả đã phát triển trở thành tiêu chuẩn vận hành của toàn bộ ngành công nghệ thế giới. Tập đoàn Red Hat phát triển các giải pháp dựa trên Linux, cung cấp toàn bộ sản phẩm ở dạng mã nguồn mở miễn phí và chỉ thu phí dịch vụ hỗ trợ kỹ thuật, cuối cùng đã được tập đoàn IBM thâu tóm với mức giá kỷ lục lên tới 34 tỷ USD.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091909.jpg)

Giống như thông điệp trong bức ảnh trên: **"Open is smart. Smart is open"** (Mở là thông minh. Thông minh là phải mở). Chúng ta không nên xây dựng các sản phẩm đóng khép kín (closed), hãy tập trung tạo ra những sản phẩm mở (open). Bản chất "Mở" chắc chắn sẽ mang lại những giá trị thặng dư to lớn hơn rất nhiều.

## Khóa học 60 ngày chinh phục Cấu trúc dữ liệu và Thuật toán

Thuật toán và cấu trúc dữ liệu chính là nền tảng nội công thâm hậu của mỗi lập trình viên, đóng vai trò quyết định cho việc nâng cao tư duy lập trình và thăng tiến sự nghiệp lâu dài, giúp việc tiếp cận các ngôn ngữ hay framework mới trở nên dễ dàng hơn. Đồng thời, đây cũng là phần nội dung thi bắt buộc trong các vòng phỏng vấn kỹ thuật của các tập đoàn công nghệ lớn.

Nhiều bạn tự học thuật toán thường gặp tình trạng thiếu hệ thống bài bản, học trước quên sau, thiếu sự rà soát kết quả trực quan nên rất khó duy trì thói quen luyện đề thi hàng ngày, dẫn tới việc bế tắc khi gặp các câu hỏi thực tế từ nhà tuyển dụng.

**Nền tảng Geektime phối hợp cùng cựu kỹ sư Facebook Đàm Siêu ra mắt khóa học chuyên sâu "Trại huấn luyện Thuật toán"** kéo dài 60 ngày cường độ cao giúp bạn làm chủ cấu trúc dữ liệu và thuật toán cơ bản đến nâng cao (hiện đã tuyển sinh khóa thứ 4).

Khóa học kết hợp giữa các video bài giảng lý thuyết, các buổi livestream giải bài trực tiếp, hoạt động thảo luận nhóm và dịch vụ hỗ trợ học tập toàn diện từ đội ngũ trợ giảng (chấm bài tập, rà soát mã nguồn, tổ chức thi giữa kỳ, cuối kỳ và cấp chứng nhận tốt nghiệp).

Nội dung học đi từ căn bản đến chuyên sâu: từ cấu trúc mảng, danh sách liên kết đến quy hoạch động, cấu trúc Disjoint Set (Union-Find), Trie (cây từ điển), Red-Black Tree (cây đỏ đen), AVL Tree, thuật toán xử lý bit (Bitwise), Bloom Filter và bộ nhớ đệm LRU Cache. Dưới đây là khung chương trình học chi tiết:

> - Tuần khởi động: Tổng quan về cấu trúc dữ liệu và thuật toán
> - Tuần 1: Mảng (Arrays), Danh sách liên kết (Linked Lists), Ngăn xếp (Stacks) và Hàng đợi (Queues)
> - Tuần 2: Bảng băm (Hash Tables), Ánh xạ (Maps), Tập hợp (Sets)
> - Tuần 2: Cấu trúc Cây (Trees), Cây nhị phân (Binary Trees) và Đồ thị (Graphs)
> - Tuần 3: Đệ quy (Recursion), Chia để trị (Divide and Conquer) và Quay lui (Backtracking)
> - Tuần 4: Thuật toán tìm kiếm DFS, BFS và kỹ thuật cắt tỉa nhánh (Pruning)
> - Tuần 4: Thuật toán Tham lam (Greedy Algorithms) và Tìm kiếm nhị phân (Binary Search)
> - Tuần 5: Quy hoạch động (Dynamic Programming)
> - Tuần 6: Disjoint Set (Union-Find), Trie, Red-Black Tree và AVL Tree
> - Tuần 7: Phép toán xử lý bit, Bloom Filter và LRU Cache
> - Tuần 7: Các thuật toán Sắp xếp (Sorting) và xử lý Chuỗi ký tự (String)
> - Tuần tốt nghiệp: Tổng kết toàn bộ hệ thống tri thức

Học phí gốc 2.499 nhân dân tệ, giá ưu đãi hiện tại là 1.499 nhân dân tệ. Độc giả sử dụng mã giảm giá đặc biệt **RUANYFENG** sẽ được giảm thêm 100 nhân dân tệ. Quét mã QR dưới đây để xem chi tiết chương trình học và đăng ký tham gia.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091808.jpg)

## 资讯 (Tin tức)

1. **Hiện tượng sông băng vùng Bắc Cực cạn nước nghiêm trọng chưa từng có trong lịch sử**

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019083012.jpg)

Mùa hè năm nay ghi nhận đợt nắng nóng cực đoan tại vòng Bắc Cực khiến mực nước của sông Lena - một trong những hệ thống sông lớn nhất chảy qua vùng đất đóng băng vĩnh cửu của vùng Siberia thuộc Nga - bị sụt giảm tới 2.5 mét, đẩy lòng sông rơi vào tình trạng cạn trơ đáy nghiêm trọng (ảnh trên). Việc giao thông đường thủy bị tê liệt hoàn toàn gây ảnh hưởng nặng nề đến đời sống của nhiều khu dân cư hẻo lánh ven sông do đây là tuyến đường vận tải hậu cần tiếp tế độc đạo của vùng không có đường bộ kết nối.

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019083013.jpg)

2. **Nữ tay đua tốc độ huyền thoại Jessi Combs tử nạn ở tuổi 39 khi cố gắng phá kỷ lục thế giới**

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090102.jpg)

Jessi Combs - nữ tay đua xe chuyên nghiệp nổi tiếng người Mỹ - vừa qua đời trong một tai nạn thảm khốc tại vùng hoang mạc bang Oregon khi đang thực hiện thử nghiệm phá kỷ lục tốc độ thế giới của dòng xe 4 bánh, hưởng dương 39 tuổi.

Năm 2013, cô từng thiết lập kỷ lục thế giới về tốc độ lái xe 4 bánh của nữ giới với vận tốc trung bình đạt 632 km/h và tốc độ tối đa chạm mốc 709 km/h. Năm 2016, cô tiếp tục tự vượt qua giới hạn của mình với vận tốc tối đa đạt tới 768.61 km/h. Chiếc xe cô lái sử dụng động cơ phản lực đặc biệt có tên "North American Eagle" (Đại bàng Bắc Mỹ), và đây cũng chính là chiếc xe gặp sự cố mất kiểm soát trong đợt thử nghiệm định mệnh này.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090104.jpg)

3. **Hãng xe BMW ra mắt mẫu SUV X6 sử dụng chất liệu sơn hấp thụ ánh sáng Vantablack tối nhất thế giới**

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090105.jpg)

Hãng xe Đức giới thiệu phiên bản đặc biệt của dòng xe BMW X6 phủ lớp sơn Vantablack. Vantablack là vật liệu nhân tạo tối nhất thế giới có khả năng hấp thụ tới hơn 99% ánh sáng chiếu vào bề mặt. Lớp phủ này khiến chiếc BMW VBX6 gần như loại bỏ hoàn toàn mọi góc phản chiếu ánh sáng tự nhiên. Về mặt vật lý học thị giác, nếu một vật thể hoàn toàn không phản chiếu bất kỳ photon ánh sáng nào phản hồi về mắt người, cấu trúc 3D của nó sẽ biến mất và trông như một "hố đen" phẳng lơ lửng trong không gian.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090106.jpg)

4. **Kỷ niệm 10 năm thành lập trường học sinh thái Green School hoàn toàn bằng tre tại Bali**

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090301.jpg)

Trường học sinh thái Green School nổi tiếng tại đảo Bali (Indonesia) vừa tổ chức lễ kỷ niệm 10 năm thành lập. Toàn bộ khuôn viên và kiến trúc mái vòm của trường được xây dựng hoàn toàn bằng thân cây tre tự nhiên mang lại kiến trúc vô cùng độc đáo thu hút sự chú ý của giới kiến trúc thế giới. Thông thường, tre chỉ được dùng cho các công trình tạm bợ, hàng rào do tre chứa nhiều tinh bột dễ bị mối mọt, nấm mốc tàn phá và rất dễ cháy. Các kiến trúc sư đã ứng dụng phương pháp xử lý ngâm tẩm hóa chất sinh học tự nhiên giúp tăng tuổi thọ và độ chịu lực của tre lên hàng chục năm.

Các nhà khoa học hiện đang đẩy mạnh nghiên cứu các dòng ván tre ép kết hợp nhựa sinh học chống cháy để nhân rộng mô hình xây dựng thân thiện môi trường này ra thế giới.

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090303.jpg)

5. **Bức ảnh chụp vệ tinh vô tình hé lộ năng lực giám sát tầm cực cao của vệ tinh do thám Mỹ USA-224**

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019090503.jpg)

Ngày 29/8, một vụ nổ bệ phóng tên lửa đẩy Safir của Iran đã diễn ra thất bại tại trung tâm vũ trụ địa phương. Ngay hôm sau, Tổng thống Mỹ Donald Trump đã chia sẻ trên Twitter một bức ảnh chụp bệ phóng bị cháy đen từ trên không với độ sắc nét cực cao để khẳng định Mỹ không liên quan đến sự cố (ảnh trên).

Các nhà thiên văn học quốc tế đã nhanh chóng phân tích góc đổ bóng của các cột tháp trên ảnh để tính toán chính xác thời điểm chụp. Kết quả cho thấy tại thời điểm đó, chỉ có duy nhất vệ tinh do thám tuyệt mật mang mã hiệu USA-224 của quân đội Mỹ bay qua bầu trời Iran. Bức ảnh Trump chia sẻ vô tình trở thành tài liệu rò rỉ đầu tiên chứng minh năng lực chụp ảnh tầm xa cực kỳ sắc nét của các vệ tinh do thám quân sự Mỹ, vốn là thông tin bảo mật quốc gia không được phép công bố rộng rãi.

6. **Phát minh bê tông sinh học tự vá lành vết nứt nhờ vi khuẩn của nhà khoa học Hà Lan**

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082707.jpg)

Các vết nứt chân chim trên cấu trúc bê tông xây dựng là hiện tượng vật lý phổ biến gây xuống cấp công trình theo thời gian. Một giáo sư vi sinh học tại Hà Lan đã phát minh ra loại bê tông sinh học (bio-concrete) bằng cách trộn thêm các bào tử vi khuẩn đặc biệt cùng thức ăn lactat canxi vào hỗn hợp xi măng.

Khi bê tông xuất hiện vết nứt, nước và oxy từ môi trường ngoài lọt vào sẽ kích hoạt bào tử vi khuẩn thức dậy sau giấc ngủ đông. Vi khuẩn tiêu thụ lactat canxi và tiết ra đá vôi (canxi cacbonat) lấp đầy các khe nứt một cách tự nhiên. Hiện tại, công nghệ có thể vá lành các vết nứt có chiều rộng lên tới 0.8mm, tuy nhiên chi phí sản xuất loại bê tông này cao gấp đôi so với xi măng thông thường. (Ảnh dưới: Tiến trình vá lành vết nứt của bê tông sinh học sau 28 ngày và 56 ngày).

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082710.jpg)

7. **Hình ảnh vệ tinh cho thấy vụ tấn công chính xác bằng drone vào nhà máy lọc dầu Saudi Aramco**

![](https://cdn.beekka.com/blogimg/asset/201909/bg2019091701.jpg)

Ngày 14/9, tổ hợp lọc dầu lớn nhất của tập đoàn Saudi Aramco bị tấn công gây hỏa hoạn nghiêm trọng. Ảnh vệ tinh hiện trường cho thấy độ chính xác tuyệt đối vô tiền khoáng hậu của cuộc tấn công: toàn bộ 17 điểm nổ đều găm trúng hồng tâm các bồn chứa dầu hình tròn mà hoàn toàn không gây tổn hại đến các hạ tầng xung quanh (các ô vuông đỏ trên ảnh). Giới chuyên gia quân sự nhận định cuộc tấn công sử dụng các dòng thiết bị bay không người lái (drone) tự sát có hệ dẫn đường lập trình chính xác cao.

8. **Tin vắn**

- Nghiên cứu công bố trên tạp chí *Nature* cảnh báo tốc độ khai thác cát sông trên thế giới đã vượt quá tốc độ bồi đắp tự nhiên của các dòng chảy, đe dọa trực tiếp đến hệ sinh thái sông ngòi toàn cầu. Cát sa mạc và cát biển quá mịn không thể dùng cho xây dựng, buộc ngành bê tông thế giới phải sử dụng từ 32 đến 50 tỷ tấn cát sông mỗi năm.

- Bang California (Mỹ) thông qua dự luật AB5 quy định các tài xế lái xe công nghệ cho Uber hay Lyft phải được coi là nhân viên chính thức (employees) thay vì nhà thầu độc lập (contractors) để được hưởng lương tối thiểu, bảo hiểm y tế và các phúc lợi lao động.

- Chính phủ Ấn Độ ban hành lệnh cấm sử dụng 6 loại sản phẩm nhựa dùng một lần (túi nilon, cốc, đĩa, chai nhựa nhỏ, ống hút và màng bọc) trên toàn quốc từ ngày 2/10 để hạn chế ô nhiễm môi trường.

- Một startup công nghệ đưa ra thống kê cho thấy việc lưu trữ và gửi nhận 246 tỷ email hàng ngày trên thế giới tiêu thụ lượng điện năng tương đương phát thải 986.000 tấn khí thải carbon, và kêu gọi người dùng hủy đăng ký (unsubscribe) các hòm thư rác không cần thiết để bảo vệ môi trường.

- Du khách tham gia hoạt động tìm kiếm tại Công viên Crater of Diamonds (bang Arkansas, Mỹ) bất ngờ phát hiện một viên kim cương màu vàng thô nặng tới 3.72 carat ngay khi đang xem video hướng dẫn tìm kim cương trên YouTube (ảnh dưới).

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082604.jpg)

## 文章 (Bài viết)

1、[Bài viết] [Phân tích cấu trúc 3 tầng của hệ điều hành Android và cơ hội của Harmony OS (Hồng Mông)](https://raccoon.onyxbits.de/blog/harmony-os-the-android-killer/) (Tiếng Anh)

Hệ điều hành Android thực chất được cấu thành từ 3 lớp: Nhân Linux kernel ở đáy, lớp trung gian Android Runtime/Framework và lớp Dịch vụ của Google (GMS) ở trên cùng. Tác giả phân tích chiến lược khả thi của Huawei cho hệ điều hành Harmony OS là giữ nguyên hai lớp dưới để đảm bảo tính tương thích với hệ sinh thái ứng dụng Android hiện tại và tập trung tự phát triển lớp dịch vụ thay thế cho GMS.

2、[Bài viết] [Rủi ro bảo mật nghiêm trọng từ việc rò rỉ dữ liệu sinh trắc học của hệ thống BioStar 2](https://www.vpnmentor.com/blog/report-biostar2-leak/) (Tiếng Anh)

Nhóm nghiên cứu bảo mật công bố đã phát hiện lỗ hổng rò rỉ cơ sở dữ liệu của hệ thống kiểm soát an ninh BioStar 2 chứa hơn 1 triệu mẫu vân tay và nhận diện khuôn mặt của người dùng. Bài viết cảnh báo việc sử dụng sinh trắc học làm mật khẩu khóa hệ thống tiềm ẩn rủi ro cực lớn, bởi vì một khi khóa vân tay bị rò rỉ trên mạng, người dùng hoàn toàn không thể thực hiện đổi vân tay như mật khẩu thông thường.

3、[Bài viết] [Hướng dẫn xây dựng hệ thống lưu trữ ảnh (图床) cá nhân miễn phí bằng Backblaze B2 và Cloudflare Workers](https://blog.jross.me/free-personal-image-hosting-with-backblaze-b2-and-cloudflare-workers/) (Tiếng Anh)

Hướng dẫn chi tiết từng bước cấu hình lưu trữ ảnh tĩnh trên kho lưu trữ đám mây Backblaze B2 (miễn phí 10GB đầu), kết hợp viết script định tuyến qua Cloudflare Workers để tạo CDN phân phối ảnh miễn phí tốc độ cao cho blog cá nhân.

4、[Bài viết] [Lịch sử ra đời và các đặc tính vật lý của dòng switch bàn phím cơ Cherry MX](https://www.keymouse.com/cherry-mx-switches) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019082701.jpg)

Giới thiệu các thông số kỹ thuật (lực nhấn, hành trình phím) và chia sẻ các hình vẽ động cắt lớp mô tả cơ chế phản hồi xúc giác bên trong các dòng switch bàn phím cơ nổi tiếng của hãng Cherry (Blue, Red, Brown, Black).

## 软件 (Phần mềm)

1、[Dadroit JSON Viewer — Trình duyệt và phân tích tệp tin dữ liệu JSON dung lượng lớn siêu nhanh](https://viewer.dadroit.com/)

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019081107.jpg)

Giải quyết triệt để tình trạng đơ lag máy khi mở các file JSON nặng hàng trăm MB nhờ cơ chế parse dữ liệu tuần tự trực tiếp trên bộ nhớ và hiển thị cấu trúc dạng cây trực quan.

2、[Anime4K — Thuật toán AI tự động nâng cấp độ phân giải hình ảnh hoạt hình anime theo thời gian thực](https://github.com/bloc97/Anime4K)

Sử dụng thuật toán nội suy hình ảnh tối ưu hóa riêng cho các nét vẽ 2D giúp nâng cấp nhanh các bộ phim anime cũ từ độ phân giải SD/HD lên chuẩn 4K sắc nét mà không bị mờ nhòe.

3、[wallace-cli — Công cụ dòng lệnh CLI phân tích chi tiết cấu trúc tệp tin định dạng CSS](https://github.com/bartveneman/wallace-cli)

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019081404.jpg)

Giúp các kỹ sư frontend kiểm tra số lượng selector, rules, thuộc tính trùng lặp và tính toán hiệu suất tải của file stylesheet trước khi đóng gói production.

4、[Dịch Hiệp (Translate Man) — Công cụ dịch thuật đa ngôn ngữ mượt mà cho trình duyệt](https://github.com/magic-FE/translate-man)

Plugin dịch thuật nguồn mở hỗ trợ Chrome và Firefox, cho phép người dùng bôi đen từ khóa hoặc bấm đúp chuột để tra nhanh nghĩa từ qua Google Translate API trực quan.

## 资源 (Tài nguyên)

1、[Trang web] [Version Museum - Bảo tàng số lưu trữ lịch sử thay đổi giao diện của các ứng dụng công nghệ](https://www.versionmuseum.com/)

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019081801.jpg)

Nơi lưu trữ ảnh chụp màn hình qua các thời kỳ phát triển của các website và phần mềm nổi tiếng (như giao diện Amazon năm 1995, Windows 95, Apple.com thời kỳ đầu) giúp người xem tìm hiểu lịch sử thiết kế giao diện UI/UX thế giới.

2、[Tài liệu] [Algorithms by Jeff Erickson - Giáo trình thuật toán miễn phí chất lượng cao của Đại học Illinois](http://jeffe.cs.illinois.edu/teaching/algorithms/)

Bộ tài liệu giảng dạy khoa học máy tính trình bày cực kỳ chi tiết, khoa học về các cấu trúc giải thuật nền tảng (quy hoạch động, thuật toán đồ thị, độ phức tạp thuật toán) đi kèm hệ thống bài tập thực hành phong phú.

## 图片 (Hình ảnh)

1. **Hostile Architecture - Xu hướng thiết kế kiến trúc đối phó ngăn ngừa lạm dụng không gian công cộng**

Kiến trúc đối phó (hostile architecture) là giải pháp thiết kế được các đô thị ứng dụng để ngăn chặn hành vi vô gia cư nằm ngủ hoặc phá hoại cảnh quan công cộng.

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019080601.jpg)

Ghế băng công cộng được thiết kế uốn lượn gồ ghề hoặc lắp thêm các tay vịn chia nhỏ khoảng ghế để người đi đường không thể nằm dài trên ghế.

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019080602.jpg)

Góc tường được ốp các khối đá nhọn nhô ra để ngăn chặn hành vi phóng uế bừa bãi.

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019080603.jpg)

Thành hoa trượt được lắp thêm các miếng kim loại nhô cao để ngăn các bạn trẻ chơi trượt ván mạo hiểm làm nứt vỡ đá ốp.

## 文摘 (Văn trích)

1. **Dark Matter Developers - Những lập trình viên "Vật chất tối" thầm lặng của thế giới công nghệ**

Trong vật lý thiên văn, vật chất tối (dark matter) chiếm đại đa số khối lượng vũ trụ nhưng hoàn toàn không phát sáng hay phản chiếu ánh sáng, khiến kính viễn vọng không thể quan sát trực tiếp. Chúng ta chỉ biết đến sự tồn tại của nó qua lực hấp dẫn tác động lên các thiên hà xung quanh.

Thực tế trong ngành phần mềm cũng tồn tại một nhóm lập trình viên tương tự, có thể gọi họ là các **Lập trình viên Vật chất tối (Dark Matter Developers)**. Họ chiếm tới 99% lực lượng lao động của ngành nhưng gần như vô hình trên internet: họ không bao giờ viết blog chia sẻ kỹ thuật, không tham gia thảo luận trên Reddit hay Hacker News, không tweet trên Twitter, không đóng góp mã nguồn mở trên GitHub và hầu như không bao giờ xuất hiện tại các hội thảo công nghệ lớn.

Họ thầm lặng làm việc trong các công ty truyền thống, sử dụng các công nghệ cũ kỹ để giải quyết các bài toán vận hành hàng ngày của doanh nghiệp: duy trì hệ thống ASP cũ trong văn phòng nhỏ, viết mã VB6 tại Mexico hay bảo trì ứng dụng PHP quản lý lịch làm việc của một hãng sản xuất chip.

Họ chỉ quan tâm đến các công cụ đã được kiểm chứng lâu năm, ổn định và dễ hiểu để hoàn thành công việc được giao. Họ hoàn toàn không hào hứng với các thư viện beta mới ra mắt hàng tuần của giới frontend. Họ thầm lặng duy trì hệ thống xương sống vận hành xã hội hàng ngày, và đương nhiên, một lập trình viên Vật chất tối thực thụ sẽ không bao giờ đọc bài viết này.

## 言论 (Danh ngôn)

1、

> "Mỗi ngày làm việc trôi qua có thể cho ta cảm giác rất dài, nhưng nhìn lại vài thập kỷ cuộc đời lại trôi qua vô cùng nhanh chóng."
> 
> -- Sam Altman, viết trong bài viết *Trải nghiệm tuổi 30 của tôi*

## 招聘信息 (Thông tin tuyển dụng)

Dưới đây là thông tin tuyển dụng từ các doanh nghiệp đối tác tài trợ cho bản tin.

Các vị trí tuyển dụng và thực tập miễn phí khác luôn được cập nhật tại [mục thảo luận tuyển dụng trên GitHub](https://github.com/ruanyf/weekly/issues/798).

1、**Entropy Reduction Technology (Hành Giản Khoa Học)**

Doanh nghiệp cung cấp giải pháp trung tâm dữ liệu (data mid-end) hàng đầu Trung Quốc phục vụ ngành tài chính đầu tư, đã hoàn thành gọi vốn vòng B. Các khách hàng lớn gồm Harvest Fund, Bosera Funds, Boston Consulting Group. Địa điểm làm việc: Bắc Kinh.

Các vị trí đang tuyển dụng:
- Quản trị sản phẩm cao cấp (Product Manager)
- Kỹ sư thuật toán xử lý ngôn ngữ tự nhiên (NLP Algorithm Engineer)
- Kỹ sư phát triển Backend
- Kỹ sư phát triển Frontend
- Kỹ sư vận hành hệ thống (DevOps)
- Kỹ sư kiểm thử chất lượng (QA)

Chi tiết yêu cầu tuyển dụng xem tại [đây](https://github.com/ruanyf/weekly/issues/798#issuecomment-532968882).

2、**Cryptape (Mật Viên Khoa Học)**

Doanh nghiệp khởi nghiệp công nghệ blockchain chuyên phát triển hạ tầng và dịch vụ blockchain cho nền kinh tế mã hóa, các sản phẩm chính gồm Nervos, Huobi Finance Chain, CITA. Địa điểm làm việc: Hàng Châu hoặc làm việc từ xa (remote).

Các vị trí đang tuyển dụng:
- Kỹ sư Blockchain cao cấp
- Kỹ sư Backend cao cấp
- Kỹ sư An ninh bảo mật và Kiểm thử phần mềm

Chi tiết công việc và yêu cầu tuyển dụng xem tại [đây](https://github.com/ruanyf/weekly/issues/798#issuecomment-524289916).

(Hết)
