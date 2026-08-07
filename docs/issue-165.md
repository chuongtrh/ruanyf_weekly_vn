# 科技爱好者周刊（第 165 期）：全端 App 的时代

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1826) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062410.jpg)

Một công viên nước tại thành phố Phù Lăng, Trùng Khánh đã tự chế tạo những cây kem que (kem que que kem) khổng lồ độc đáo để phát miễn phí giải nhiệt cho các du khách tham gia vui chơi ngày hè. (Nguồn: [Sohu](https://www.sohu.com/a/473039755_120388781))

## 主带话题：Kỷ nguyên của ứng dụng toàn nền tảng (All-platform Apps)

Tuần trước, Microsoft chính thức giới thiệu hệ điều hành Windows 11. Điểm bất ngờ và đột phá nhất chính là việc Windows 11 sẽ hỗ trợ chạy trực tiếp các ứng dụng Android (Android Apps)!

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062703.jpg)

Nghĩ kỹ thì điều này cũng không có gì quá ngạc nhiên. Kể từ khi Apple ra mắt dòng chip xử lý cấu trúc ARM M1 vào năm ngoái, tất cả các ứng dụng iPhone và iPad đã có thể chạy trực tiếp, mượt mà trên các máy tính macOS.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062704.jpg)

Microsoft chắc chắn không thể ngồi yên nhìn Apple định hình lại trải nghiệm hệ sinh thái mà buộc phải gấp rút đưa tính năng chạy ứng dụng di động Android lên Windows để cạnh tranh sòng phẳng.

Sự vội vàng của Microsoft thể hiện rõ ở việc họ thậm chí chưa kịp xây dựng một kho ứng dụng Android của riêng mình trên Windows, mà buộc phải hợp tác và hướng người dùng cài đặt kho ứng dụng Amazon Appstore để tìm và chạy các app này. Chấp nhận dẫn luồng người dùng khổng lồ sang cho đối thủ đã phản ánh sự sốt sắng của Microsoft đối với tính năng này.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062705.jpg)

Vậy xu hướng chạy ứng dụng di động trực tiếp trên máy tính để bàn (PC/Desktop) sẽ mang lại tác động gì cho thế giới phát triển phần mềm?

Tác động rõ ràng nhất là: **Liệu trong tương lai chúng ta có còn cần phát triển các phiên bản phần mềm chuyên biệt cho máy tính để bàn nữa hay không?** Ngoại trừ một số ứng dụng đặc thù đòi hỏi tài nguyên xử lý cực cao của máy tính (như phần mềm đồ họa 3D, dựng video chuyên nghiệp), các phần mềm thông thường khác chỉ cần tối ưu hóa giao diện ứng dụng di động cho vừa vặn với kích thước màn hình PC là đã có thể thay thế hoàn toàn cho các phiên bản Windows hay macOS chuyên biệt.

Ví dụ thực tế: Để sử dụng WeChat trên Windows hiện nay, người dùng bắt buộc phải cài đặt một phiên bản WeChat dành riêng cho Windows khá nặng nề. Trong tương lai, bạn hoàn toàn có thể chạy trực tiếp phiên bản WeChat di động ngay trên Windows. Đối với người dùng, trải nghiệm tính năng sẽ đầy đủ và đồng bộ hoàn toàn với điện thoại; đối với nhà phát triển Tencent, họ có thể giải tán bớt một đội ngũ lập trình viên chuyên trách phiên bản desktop và giảm thiểu tối đa sự phức tạp của việc kiểm thử mã nguồn đa nền tảng.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062706.jpg)

Trước đây, cái gọi là phần mềm đa nền tảng (cross-platform) có nghĩa là lập trình viên viết một bộ mã nguồn (codebase) chung nhưng vẫn bắt buộc phải biên dịch (compile) riêng biệt ra các tệp thực thi cho từng hệ điều hành khác nhau (như cơ chế của Java, Go hay Electron). Hiện nay, ngay cả bước biên dịch riêng biệt này cũng có thể lược bỏ: cùng một file đóng gói ứng dụng di động duy nhất có thể chạy trực tiếp không sửa đổi trên điện thoại, máy tính bảng và máy tính để bàn. Đây chính là giấc mơ và là món quà tuyệt vời dành cho các nhà phát triển phần mềm.

Xu hướng này mở rộng quy mô thị trường của các ứng dụng di động lên hàng tỷ máy tính để bàn trên thế giới, đặc biệt mở ra cơ hội lớn cho các đội ngũ phát triển tinh gọn và các startup nhỏ.

Vì vậy, kết luận của tôi là: **Thế giới phát triển ứng dụng sẽ dịch chuyển từ giai đoạn "đa nền tảng độc lập" sang "toàn nền tảng đồng nhất".** Ứng dụng di động sẽ dần nuốt chửng các phân khúc khách hàng của các client khác và trở thành lõi trung tâm; trong khi các ứng dụng desktop thuần túy sẽ dần thoái trào và thu hẹp nhu cầu phát triển.

Tuy nhiên, đây là một lộ trình dài hạn và còn nhiều rào cản kỹ thuật cần hoàn thiện. Để làm được điều này trên Windows 11, Microsoft đã tích hợp công nghệ Intel Bridge nhằm giúp các CPU cấu trúc x86 có thể thông dịch trực tiếp các tập lệnh ARM của ứng dụng Android thời gian thực. Nhưng vấn đề đặt ra là các ứng dụng phụ thuộc chặt chẽ vào Dịch vụ Di động của Google (GMS) sẽ được xử lý ra sao? Mặt khác, trước đây Google cũng đã tích hợp khả năng chạy app Android lên hệ điều hành ChromeOS (qua một lớp ảo hóa) nhưng hiệu năng thực tế khá hạn chế và trải nghiệm chuột, bàn phím chưa thực sự tối ưu.

Nhưng dù thế nào đi nữa, ứng dụng toàn nền tảng chắc chắn là tương lai không thể đảo ngược của ngành công nghệ. Các rào cản trên sẽ dần được giải quyết bằng các cải tiến phần cứng và phần mềm, đặc biệt là trong hệ sinh thái khép kín của Apple - nơi sự tương thích phần cứng ARM đã được giải quyết triệt để.

Tôi khuyến nghị các lập trình viên nên chú ý nghiên cứu hướng đi này, đặc biệt là kỹ thuật tối ưu hóa thiết kế giao diện ứng dụng di động thích ứng linh hoạt (responsive layout) trên màn hình máy tính lớn - đây có thể sẽ là một xu hướng tuyển dụng hot trong thời gian tới.

## Khóa học thực hành xây dựng môi trường chạy Mini Program trên trình duyệt

Mini Program (tiểu ứng dụng) là một mô hình ứng dụng vô cùng thành công của ngành công nghệ phần mềm Trung Quốc.

Kể từ khi WeChat phát minh ra mô hình này vào năm 2017, các ông lớn công nghệ khác (Alipay, Baidu, ByteDance, v.v.) đều nhanh chóng hỗ trợ. Hiện nay phát triển Mini Program đã trở thành một nhánh độc lập vô cùng quan trọng bên cạnh Web và App di động truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070105.jpg)

**Về bản chất kỹ thuật, Mini Program là việc dịch chuyển các công nghệ Web chạy trong một container đóng gói bên trong ứng dụng di động.** Nó hoàn toàn sử dụng công nghệ Web để phát triển, chỉ là chuyển engine kết xuất trang web vào một container điều hướng của ứng dụng. Do đó, làm chủ cơ chế kết xuất của trình duyệt là chìa khóa để tối ưu hóa hiệu năng Mini Program.

Khóa học chuyên đề **《Building Mini Program Running Environment in Browser》** do học viện **Jingcheng Yideng** biên soạn sẽ hướng dẫn bạn tự xây dựng một môi trường chạy Mini Program trực tiếp trên nhân trình duyệt để hiểu sâu về cơ chế hoạt động của nó:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070107.jpg)

Khóa học gồm 3 buổi học đi sâu vào nguyên lý hoạt động của nhân trình duyệt để giúp lập trình viên viết được các trang web tối ưu hóa hiệu năng render mượt mà nhất trên thiết bị di động.

Khóa học trị giá 98 tệ hiện được mở đăng ký cho độc giả bản tin qua mã QR dưới đây với mức phí ghi danh tượng trưng chỉ **0.02 NDT**:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070106.jpg)

Học viên đăng ký thành công sẽ được tặng kèm khóa học thực hành code phỏng vấn Front-end nâng cao.

## 科技动态

1、[Xe tải tự hành hoàn thành chuyến giao hàng dài 1.500 km](https://interestingengineering.com/self-driving-truck-completes-950-mile-trip-10-hours-faster-than-human-driver)

Một hãng công nghệ phát triển xe tự hành của Mỹ thông báo đã thực hiện thành công chuyến vận chuyển hàng hóa thử nghiệm bằng xe tải hạng nặng tự lái hoàn toàn trên lộ trình dài 1.500 km chỉ trong vòng 14 giờ. Con số này nhanh hơn 10 giờ so với thời gian vận chuyển của tài xế con người.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060505.jpg)

Do tốc độ di chuyển của xe tải hạng nặng thường chậm và luật giao thông Mỹ quy định tài xế xe tải không được phép lái xe liên tục quá 11 giờ để đảm bảo an toàn, công nghệ tự hành cho xe tải hạng nặng mang lại hiệu ích kinh tế cực kỳ lớn cho các doanh nghiệp logistics và dự kiến sẽ sớm được thương mại hóa trên quy mô lớn.

2、[Ứng dụng di động thay thế phương pháp đếm ngọc trai thủ công](https://countthings.com/case-studies/0001)

Một doanh nghiệp xuất khẩu ngọc trai tại Nhật Bản đã tìm ra giải pháp thay thế cho phương pháp thanh điểm ngọc trai thủ công truyền thống vốn mất rất nhiều thời gian và công sức của nhân viên.

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052417.jpg)

Bằng cách sử dụng ứng dụng di động "CountThings from Photos", nhân viên chỉ cần đặt ngọc trai lên khay phẳng và chụp một bức ảnh. Ứng dụng tích hợp công nghệ thị giác máy tính sẽ tự động đếm chính xác số lượng ngọc trai trên khay chỉ trong vòng 30 phút thay vì mất 2 ngày công đếm tay như trước đây.

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052418.jpg)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052419.jpg)

3、[Cảnh sát bắt giữ tội phạm lẩn trốn từ bức ảnh chụp vân tay cầm phô mai](https://www.bbc.com/news/uk-england-merseyside-57226165)

Kênh tin tức BBC đưa tin lực lượng cảnh sát Anh đã bắt giữ thành công một đối tượng buôn bán ma túy bỏ trốn lâu năm nhờ một sai lầm ngớ ngẩn của đối tượng trên mạng xã hội.

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052416.jpg)

Đối tượng đã đăng tải một bức ảnh chụp bàn tay đang cầm một miếng phô mai lên tài khoản mạng xã hội cá nhân. Cơ quan điều tra đã sử dụng các phần mềm quét ảnh độ phân giải cao để trích xuất dữ liệu đường vân tay và vân lòng bàn tay hiển thị trong bức ảnh, đối chiếu dữ liệu vân tay của các tội phạm truy nã để xác định danh tính và bắt giữ đối tượng. Đối tượng đã bị tuyên án 13 năm 6 tháng tù giam.

4、[Nghiên cứu sóng não của cầu thủ khi thực hiện sút phạt đền](https://www.cbc.ca/radio/quirks/may-15-california-condor-genetics-a-strange-star-goes-supernova-don-t-think-just-kick-and-more-1.6025290/for-soccer-players-the-less-brain-they-use-the-better-for-penalty-kicks-1.6025297)

Một nghiên cứu sinh ngành thần kinh học tại Hà Lan đã tiến hành đo đạc hoạt động sóng não của các cầu thủ bóng đá chuyên nghiệp khi thực hiện sút phạt đền bằng cách cho họ đeo mũ cảm biến điện não đồ.

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052402.jpg)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021052403.jpg)

Kết quả nghiên cứu chỉ ra rằng các cầu thủ thực hiện loạt sút phạt đền nhanh chóng và ít suy nghĩ phân tích nhất có tỷ lệ sút bóng trúng đích cao nhất. Trái lại, những cầu thủ có hoạt động sóng não vùng vỏ não lập kế hoạch hoạt động quá mạnh (biểu hiện của sự lo lắng và suy nghĩ quá nhiều) thường có tỷ lệ sút hỏng cao hơn.

5、[Xe tự hành Curiosity chụp ảnh các đám mây mỏng trên Sao Hỏa](https://petapixel.com/2021/06/02/nasas-mars-curiosity-rover-captures-rare-photos-of-shimmering-clouds/)

Xe tự hành Curiosity của NASA hoạt động trên Sao Hỏa đã gửi về những hình ảnh cận cảnh tuyệt đẹp về các đám mây trên bầu khí quyển Hỏa Tinh.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060316.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060317.jpg)

Do bầu khí quyển của Sao Hỏa cực kỳ mỏng và khô cằn, các đám mây tại đây không dày đặc như Trái Đất mà chỉ xuất hiện dưới dạng các sợi tơ mây mỏng nhẹ, lung linh phản chiếu ánh sáng mặt trời hoàng hôn ở độ cao lớn.

6、[Hãng Unitree ra mắt robot bốn chân Go1 giá rẻ](https://spectrum.ieee.org/automaton/robotics/robotics-hardware/unitrees-go1-robot-dog-looks-pretty-great-costs-just-usd-2700)

Hãng phát triển robot Unitree của Trung Quốc công bố dòng robot bốn chân (机器狗) Go1 hướng tới phân khúc người dùng cá nhân phổ thông với mức giá bán cực kỳ dễ tiếp cận chỉ từ 2.700 USD (khoảng 16.000 ~ 20.000 NDT).

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062102.jpg)

Go1 được trang bị hệ thống cảm biến thông minh tự động bám sát chủ đi bộ và tránh các chướng ngại vật trên đường đi với khả năng thăng bằng cực tốt khi bị xô đẩy và tự đứng dậy khi ngã. Robot có tải trọng 5 kg và thời lượng pin hoạt động liên tục 1 giờ, mức giá này rẻ bằng một phần mười so với sản phẩm của Boston Dynamics.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062103.jpg)

7、[Bàn giao tàu nghiên cứu khoa học biển lớn nhất Trung Quốc "Sun Yat-sen University"](https://china.huanqiu.com/article/43h6gCmStZe)

Tàu nghiên cứu khoa học hải dương và giáo dục thực địa có tải trọng lớn nhất Trung Quốc mang tên "Sun Yat-sen University" đã chính thức được bàn giao cho Đại học Tôn Trung Sơn tại Thượng Hải. Tàu có lượng giãn nước 6.880 tấn và tầm hoạt động tối đa lên tới 15.000 hải lý, được trang bị nhiều phòng thí nghiệm hiện đại phục vụ nghiên cứu biển sâu.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062606.jpg)

8、[Thiết bị hỗ trợ con người nghe được các tần số siêu âm](https://www.aalto.fi/en/news/anyone-can-get-super-hearing)

Tai người bình thường chỉ nghe được âm thanh trong dải tần số từ 20 Hz đến 20.000 Hz. Các nhà nghiên cứu tại Đại học Aalto, Phần Lan đã phát triển một thiết bị hỗ trợ tai nghe giúp con người nghe được các tần số siêu âm trên 20.000 Hz.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061002.jpg)

Thiết bị sử dụng một cụm microphone đặt trong một quả cầu nhựa nhỏ để thu nhận các âm thanh tần số siêu âm của môi trường xung quanh, phân tích định vị hướng phát của nguồn âm thanh và hạ tần số của nó về dải nghe được của con người trước khi phát ra tai nghe, mang lại cho con người thính giác siêu phàm tương tự loài dơi.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061003.jpg)

## 文章

1、[Sự trỗi dậy và lụi tàn của trò chơi ảo nuôi thú QQ Pet](https://www.gcores.com/articles/137688)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060305.jpg)

Bài viết nhìn lại lịch sử phát triển của dòng game nuôi thú ảo QQ Pet được Tencent giới thiệu vào năm 2005. Trò chơi đã nhanh chóng thu hút hàng chục triệu người chơi thế hệ 8x, 9x tham gia và đạt mốc 1 triệu người dùng trực tuyến đồng thời trước khi chính thức dừng vận hành vào năm 2018.

2、[Trải nghiệm dòng game tương tác hẹn hò thực cảnh tại Hàn Quốc](https://mp.weixin.qq.com/s/ICeg7ksh3KHbFSj00mbmvg)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061702.jpg)

Giới thiệu xu hướng phát triển dòng game nhập vai hẹn hò sử dụng video quay thực cảnh (FMV) do các diễn viên thật đóng tại Hàn Quốc, mang lại cho người chơi trải nghiệm tương tác trực quan tương tự như đang tham gia một bộ phim truyền hình đa tuyến nhân vật.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061703.jpg)

3、[Hướng dẫn thiết lập cơ sở dữ liệu SQLite chạy trực tiếp trên web tĩnh](https://phiresky.github.io/blog/2021/hosting-sqlite-databases-on-github-pages/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021063012.jpg)

Tác giả hướng dẫn cách cấu hình tệp tin cơ sở dữ liệu SQLite tĩnh chạy trực tiếp trên môi trường GitHub Pages, cho phép trình duyệt Front-end của người dùng thực hiện các truy vấn SQL để lấy dữ liệu về hiển thị mà không cần cài đặt máy chủ cơ sở dữ liệu hay viết mã backend điều hướng. Giải pháp tận dụng cơ chế chia trang dữ liệu 4KB của SQLite kết hợp sql.js chạy trên WebAssembly. (Đóng góp của [@joyc](https://github.com/ruanyf/weekly/issues/1820))

4、[Telegram và đế chế bảo mật của Pavel Durov](https://www.spiegel.de/international/world/the-telegram-billionaire-and-his-dark-empire-a-f27cb79f-86ae-48de-bdbd-8df604d07cc8)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061502.jpg)

Phóng sự chuyên sâu dài kỳ của báo *Spiegel* (Đức) khắc họa chân dung nhà sáng lập ứng dụng nhắn tin bảo mật Telegram Pavel Durov (36 tuổi), từ những mâu thuẫn chính trị với nước Nga cho đến triết lý xây dựng ứng dụng nhắn tin mã hóa hàng đầu thế giới hiện nay.

5、[Cẩm nang hướng dẫn cài đặt Windows 11 trên các dòng máy tính cũ](https://allthings.how/how-to-install-windows-11-on-legacy-bios-without-secure-boot-or-tpm-2-0/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062702.jpg)

Bài viết hướng dẫn chi tiết cách cấu hình sửa đổi bộ cài đặt ISO của Windows 11 để bỏ qua bước kiểm tra yêu cầu phần cứng khắt khe của Microsoft (như yêu cầu chíp bảo mật TPM 2.0 và chế độ Secure Boot của BIOS) giúp cài đặt hệ điều hành mới trên các dòng PC đời cũ.

6、[Phân tích lỗi logic trong đoạn code được copy nhiều nhất trên StackOverflow](https://programming.guide/worlds-most-copied-so-snippet.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061704.jpg)

Một nghiên cứu chỉ ra đoạn mã Java hỗ trợ chuyển đổi kích thước byte sang đơn vị đo lường MB, GB trực quan dễ đọc là đoạn code được lập trình viên sao chép nhiều nhất trên StackOverflow. Tác giả của đoạn code đó đã viết bài viết này để mổ xẻ các lỗi làm tròn số học nhỏ trong đoạn code gốc của mình và cách khắc phục nó.

7、[Hướng dẫn cấu hình proxy native trong trình duyệt để truy cập Sci-Hub](https://fragile-credences.github.io/scihub-proxy/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061004.jpg)

Bài viết hướng dẫn lập trình cấu hình file Proxy Auto-Config (PAC) tích hợp trực tiếp vào trình duyệt để tự động điều hướng truy cập khi người dùng truy cập các liên kết tài liệu nghiên cứu trên thư viện khoa học Sci-Hub bị chặn.

8、[Cẩm nang hướng dẫn nhanh sử dụng Docker Compose](https://linuxhandbook.com/docker-compose-quick-start/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061203.jpg)

Bài viết hướng dẫn nhập môn Docker Compose thông qua việc cấu hình file `yaml` đơn giản để thiết lập và chạy đồng bộ hệ thống ứng dụng web đa container (như WordPress kết hợp cơ sở dữ liệu MySQL).

9、[Tiêu chuẩn HTTP mới loại bỏ hiển thị Cookie Banner phiền phức](https://arstechnica.com/gadgets/2021/06/tired-of-accepting-rejecting-cookies-adpc-wants-to-automate-the-process/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061710.jpg)

Do luật bảo vệ dữ liệu châu Âu (GDPR), mọi trang web nước ngoài đều hiện popup hỏi người dùng có đồng ý lưu Cookie hay không. Một đề xuất kỹ thuật mới mang tên ADPC đề xuất tích hợp cấu hình bảo mật vào header HTTP của trình duyệt để tự động gửi tùy chọn của người dùng đến website mà không cần hiển thị banner hỏi phiền phức.

## 工具

1、[NVIDIA Canvas](https://www.nvidia.com/en-gb/studio/canvas/)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062601.jpg)

Ứng dụng vẽ tranh nghệ thuật ứng dụng AI miễn phí của Nvidia, cho phép người dùng chỉ cần vẽ các nét vẽ phác thảo thô sơ bằng cọ vẽ ảo và chọn chất liệu (như mây, đá, sông, cỏ) để AI tự động render thành bức ảnh phong cảnh siêu thực cực kỳ ấn tượng.

2、[nuoshell](https://www.nuoshell.com/)

Trình quản trị kết nối máy chủ SSH client gọn nhẹ, miễn phí hỗ trợ nhiều tab kết nối dành riêng cho hệ điều hành macOS. (Đóng góp của [@anlityli](https://github.com/ruanyf/weekly/issues/1814))

3、[gum](https://github.com/gauseen/gum)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021063011.jpg)

Tiện ích dòng lệnh hỗ trợ quản lý nhanh nhiều cấu hình định danh tài khoản Git khác nhau phục vụ commit mã nguồn lên các repo riêng biệt thuận tiện. (Đóng góp của [@gauseen](https://github.com/ruanyf/weekly/issues/1816))

4、[BookmarkHub](https://github.com/dudor/BookmarkHub/blob/main/README_cn.md)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021063010.jpg)

Extension trình duyệt hỗ trợ đồng bộ hóa kho dấu trang bookmark giữa các trình duyệt khác nhau thông qua GitHub Gist làm nơi lưu trữ dữ liệu an toàn. (Đóng góp của [@weavers1f](https://github.com/ruanyf/weekly/issues/1815))

5、[EssayKiller](https://github.com/EssayKillerBrain/EssayKiller_V2)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021063009.jpg)

Dự án AI mã nguồn mở hỗ trợ tự động viết các bài văn nghị luận tiếng Trung đạt chất lượng tương đương học sinh trung học phổ thông từ tiêu đề bài viết đầu vào. (Đóng góp của [@dllen](https://github.com/ruanyf/weekly/issues/1818))

6、[T-Rex Runner C Version](https://github.com/shlomnissan/t-rex-runner-c)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060602.jpg)

Dự án chuyển đổi tựa game khủng long nhảy xương rồng huyền thoại khi mất mạng của Chrome viết lại hoàn toàn bằng ngôn ngữ C.

7、[Rustpad](https://rustpad.io/)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060601.jpg)

Trình soạn thảo văn bản cộng tác trực tuyến thời gian thực viết bằng Rust hỗ trợ nhiều người cùng chỉnh sửa văn bản mượt mà thông qua cơ chế Operational Transformation (OT).

8、[Zero-width Short Link Generator](https://zws.im/)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061202.jpg)

Một trình rút gọn link độc đáo tạo ra các đường link rút gọn trông giống hệt nhau nhưng thực chất điều hướng đến các địa chỉ khác nhau nhờ chèn ngầm các ký tự khoảng trắng có độ rộng bằng không (zero-width space).

9、[Ojoy](https://ojoy.zaps.dev/)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061501.jpg)

Công cụ trực tuyến hỗ trợ phóng to kích thước hình ảnh nhưng vẫn giữ được độ sắc nét và chi tiết của ảnh nhờ thuật toán học máy.

## Tài nguyên

1、[Track Awesome List](https://www.trackawesomelist.com/)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021063001.jpg)

Trang web hữu ích tự động quét và cập nhật danh sách các tài nguyên mới được thêm vào các kho "Awesome List" nổi tiếng trên GitHub hàng ngày. (Đóng góp của [@theowenyoung](https://github.com/ruanyf/weekly/issues/1822))

2、[Stanford CS Courses Spreadsheet](https://docs.google.com/spreadsheets/d/1zfw8nPvJeewxcFUBpKUKmAVE8PjnJI7H0CKimdQXxr0/htmlview)

Bảng tính Google Sheets tổng hợp toàn bộ các khóa học giảng dạy chuyên ngành khoa học máy tính bậc cử nhân của Đại học Stanford kèm liên kết trang giáo trình chi tiết.

3、[Computation Structures (Kiến trúc máy tính)](https://computationstructures.org/index.html)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061401.jpg)

Tài liệu giảng dạy môn Kiến trúc máy tính của MIT cung cấp đầy đủ các bài viết lý thuyết, slide bài giảng và video thực hành hữu ích.

4][List of commercial games with available source code](https://en.wikipedia.org/wiki/List_of_commercial_video_games_with_available_source_code)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061403.jpg)

Trang Wikipedia tổng hợp danh sách các tựa game thương mại nổi tiếng đã được nhà phát triển công bố mã nguồn mở để cộng đồng học tập và mod game.

## 图片

1、[Tháp chuông nổi tiếng của ngôi làng cổ Curon chìm dưới lòng hồ nước Ý](https://www.smithsonianmag.com/smart-news/medieval-italian-village-briefly-surfaces-after-70-years-underwater-180977838/)

Năm 1950, chính phủ Ý xây dựng đập thủy điện nhân tạo làm ngập thung lũng sông và nhấn chìm ngôi làng cổ Curon. Tháp chuông nhà thờ thế kỷ 14 do quá cao nên vẫn nổi lên trên mặt nước tạo nên cảnh tượng độc đáo thu hút du khách:

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021053007.jpg)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021053008.jpg)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021053009.jpg)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021053010.jpg)

2、[Lunch atop a Skyscraper (Bữa trưa trên đỉnh tháp chọc trời)](https://historydaily.org/charles-ebbets-lunchtime-atop-a-skyscraper)

Bức ảnh chụp đen trắng nổi tiếng thế giới chụp năm 1932 ghi lại cảnh 11 công nhân xây dựng ngồi ăn trưa vắt vẻo trên thanh dầm thép ở độ cao 256 mét không đai bảo hộ khi xây dựng tòa tháp GE Building tại New York:

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021053001.jpg)

Bức ảnh hậu trường chụp nhiếp ảnh gia tác nghiệp cũng hiểm trở không kém:

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021053002.jpg)

Thực tế bên dưới thanh dầm có dựng một sàn gỗ bảo hộ khá an toàn và đây là bức ảnh摆拍 dàn dựng để làm quảng cáo truyền thông cho tòa nhà. Bức ảnh nổi tiếng đến mức thành phố New York đã đúc tượng đồng để vinh danh các công nhân xây dựng:

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021053003.jpg)

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021053004.jpg)

## Bài đọc thêm

### Tại sao tôi坚持 viết blog cá nhân suốt 8 năm?

*Tác giả chia sẻ các lợi ích thu được sau khi viết hơn 100 bài viết kỹ thuật chia sẻ trên trang cá nhân:*

1. **Hệ thống hóa kiến thức:** Viết blog buộc bạn phải diễn đạt lại kiến thức học được bằng ngôn ngữ cá nhân, giúp ghi nhớ lâu và dễ dàng tra cứu lại khi cần.
2. **Kích thích nghiên cứu sâu:** Để viết một bài viết logic, bạn sẽ tự đặt ra các câu hỏi phản biện và tiến hành các nghiên cứu sâu hơn để kiểm chứng.
3. **Đánh giá giá trị thông tin:** Quá trình chuẩn bị bài viết giúp bạn nhận diện những chủ đề nào thực sự hữu ích và có giá trị chia sẻ cho cộng đồng.
4. **Nhận đóng góp từ độc giả:** Các bình luận đóng góp của độc giả giúp bạn phát hiện các thiếu sót trong bài viết và cập nhật thêm các giải pháp mới.
5. **Cảm giác hỗ trợ cộng đồng:** Việc viết lại giải pháp cho một lỗi lập trình khó bạn đã vượt qua sẽ giúp ích cho hàng nghìn lập trình viên khác gặp lỗi tương tự tiết kiệm thời gian xử lý.

## 言论

1、

Python là ngôn ngữ lập trình tôi yêu thích nhất, nhưng nó không thể thay thế được các câu lệnh Bash. Một dòng lệnh Bash ngắn gọn có thể thay thế cho cả trăm dòng code Python tương đương (ví dụ như lệnh `mv` di chuyển file phức tạp). Bash đã đóng gói và ẩn đi toàn bộ sự phức tạp của tương tác hệ điều hành để lập trình viên sử dụng nhanh chóng.

-- Trích thảo luận trên Hacker News

2、

Trải nghiệm nâng cấp từ Python 2 lên Python 3 quá đau đớn cho cộng đồng phát triển phần mềm toàn cầu suốt nhiều năm qua, có thể đó là lý do thế giới sẽ mãi mãi không có phiên bản Python 4.0.

-- Guido van Rossum, cha đẻ ngôn ngữ Python

3、

Khi các thiết bị gia dụng và đồ dùng cá nhân ngày càng tích hợp kết nối Internet thông minh, trong tương lai nếu muốn mua các sản phẩm không kết nối mạng (offline) bạn sẽ phải trả thêm phí vì nhà sản xuất không thể thu thập dữ liệu hành vi của bạn hoặc hiển thị quảng cáo kiếm lời nữa.

-- Trích thảo luận trên Hacker News

## 历史上的本周

- 2020年（第 114 期）：[Tìm hiểu xu hướng làm việc tự do thời đại số (Gig Economy)](https://www.ruanyifeng.com/blog/2020/07/weekly-issue-114.html)
- 2019年（第 62 期）：[Giới thiệu bộ phim điện ảnh Nhật Bản ý nghĩa "Fune wo Amu" (Đan Tàu)](https://www.ruanyifeng.com/blog/2019/06/weekly-issue-62.html)
- 2018年（第 11 期）：[Phân tích sự tiến hóa ngày càng phức tạp của các ngôn ngữ lập trình hiện đại](https://www.ruanyifeng.com/blog/2018/06/weekly-issue-11.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
