# 每周分享第 30 期 (Bản tin chia sẻ hàng tuần số 30)

Ghi lại những điều thú vị đáng chia sẻ tôi bắt gặp trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Chào mừng mọi người gửi bài đóng góp thông qua mục [issue](https://github.com/ruanyf/weekly/issues) tại kho lưu trữ GitHub [ruanyf/weekly](https://github.com/ruanyf/weekly).

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110901.jpg)

Tháng trước, tập đoàn Google đã [chính thức thông báo](https://www.blog.google/technology/safety-security/project-strobe/) sẽ đóng cửa mạng xã hội Google Plus (G+) sau 10 tháng nữa.

Có hai nguyên nhân cốt lõi dẫn đến quyết định này. Thứ nhất là do sự thiếu hụt trầm trọng người dùng thực tế: thống kê cho thấy hơn 90% số lượt truy cập của người dùng trên G+ kéo dài chưa đầy 5 giây. Thứ hai là sự phát hiện của một lỗ hổng bảo mật nghiêm trọng liên quan đến API có nguy cơ làm rò rỉ dữ liệu cá nhân của hơn 500.000 tài khoản, mặc dù chưa có bằng chứng thực tế cho thấy tin tặc đã khai thác lỗ hổng này.

Là công ty internet lớn nhất thế giới sở hữu tiềm lực tài chính khổng lồ cùng đội ngũ kỹ sư hàng đầu, các sản phẩm hạ tầng của Google gần như thống trị tuyệt đối: từ AI, bộ máy tìm kiếm, email, bản đồ, kho ảnh cho đến điện toán đám mây... Về mặt lý thuyết, một mạng xã hội do Google hậu thuẫn không có lý do gì để thất bại khi hãng hoàn toàn có thể tích hợp sâu toàn bộ hệ sinh thái của mình vào đó. Nhưng G+ vẫn thất bại thảm hại. Đây là dự án mạng xã hội thứ tư của Google bị khai tử. Tại sao ông lớn này lại vô duyên với mảng mạng xã hội đến vậy?

Cách đây vài năm, từng có đề xuất tích hợp sâu tài khoản Gmail vào G+ để kích cầu lượng truy cập, nhưng dự án đã không thể triển khai. Điều này phản ánh G+ chưa bao giờ là ưu tiên cốt lõi trong DNA phát triển của Google. Mối quan tâm cốt lõi của hãng luôn hướng về các hạ tầng dịch vụ cơ bản, các thuật toán tìm kiếm tối ưu ở tầng sâu và hệ điều hành hệ thống. Các kỹ sư và nhà khoa học hàng đầu tại Google thường coi các mạng xã hội như một thứ đồ chơi công nghệ đơn giản và thiếu tính thử thách học thuật để họ tập trung cống hiến. Lãnh đạo cấp cao cho đến kỹ sư của Google hầu như không ai đam mê tham gia tương tác trên mạng xã hội. Sự thiếu hụt đam mê thực tế từ chính nội bộ là nguyên nhân sâu xa dẫn đến cái chết được báo trước của G+.

Câu chuyện này là minh chứng thực tế: doanh nghiệp cũng giống như con người, đều sở hữu những thế mạnh và sở thích đam mê cốt lõi riêng. Nếu cố ép bản thân làm những việc mình không hề đam mê, kết quả nhận lại thường chỉ là sự lãng phí nguồn lực khổng lồ trước khi chấp nhận thất bại và rời bỏ cuộc chơi.

## 新闻 (Tin tức)

1、[Mô hình nhà máy nhiệt điện hội tụ năng lượng mặt trời công suất lớn](https://arstechnica.com/science/2018/10/new-material-could-up-efficiency-of-concentrated-solar-power/)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110902.jpg)

Hiện nay, sản xuất điện mặt trời chủ yếu sử dụng công nghệ quang điện (photovoltaic) chuyển đổi trực tiếp ánh sáng thành dòng điện. Nhược điểm lớn của phương pháp này là tính bất ổn định của thời tiết dẫn đến việc lưu trữ điện năng vô cùng khó khăn và tốn kém.

Một giải pháp thay thế là xây dựng các nhà máy hội tụ năng lượng mặt trời (CSP) sử dụng hệ thống gương khổng lồ tập trung ánh sáng để tạo ra nguồn nhiệt lượng cực lớn nung nóng các dung dịch muối lỏng đặc biệt. Nguồn nhiệt năng tích lũy này sau đó được sử dụng để chạy tuabin phát điện liên tục bất kể ngày đêm. Phương pháp lưu trữ nhiệt lượng này hiệu quả và rẻ hơn nhiều so với lưu trữ điện bằng pin truyền thống. (Hình trên là nhà máy điện mặt trời CSP công suất 110 MW tại sa mạc Negev, Israel).

2、[Bitmovin ra mắt trình phát video thông minh tự động nhận diện tương tác của người xem](https://bitmovin.com/user-aware-video-player/)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110903.jpg)

Trình phát video thông dụng Bitmovin đã cập nhật tính năng nhận diện người xem thông minh qua camera thiết bị. Khi phát hiện người xem di chuyển ra xa màn hình, hệ thống sẽ tự động giảm bitrate (chất lượng hình ảnh) để tiết kiệm băng thông và tự động tăng chất lượng khi họ tiến lại gần. Nếu người xem rời khỏi vị trí, video sẽ tự động tạm dừng (pause) và tự động phát tiếp (resume) ngay khi họ quay trở lại.

3. **Thuật toán giao tiếp chéo giữa các xe tự hành hứa hẹn thay thế hệ thống đèn tín hiệu giao thông**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110904.jpg)

Đại học Carnegie Mellon phát triển thành công thuật toán giao tiếp giữa các phương tiện tự hành (V2V communication) tại các giao lộ. Khi tiến gần ngã tư, các xe tự lái sẽ tự động trao đổi dữ liệu tốc độ và hướng đi để tự thỏa thuận thứ tự xe nào vượt qua trước một cách an toàn mà không cần đến sự hỗ trợ của đèn xanh đèn đỏ truyền thống. Mô phỏng thực tế cho thấy giải pháp giúp cắt giảm 1/3 thời gian di chuyển trong đô thị.

4、[MongoDB thay đổi giấy phép bản quyền sang SSPL bắt buộc các hãng đám mây phải开源](https://www.mongodb.com/press/mongodb-issues-new-server-side-public-license-for-mongodb-community-server)

Giấy phép mã nguồn mở GPL truyền thống quy định nếu một bên sửa đổi mã nguồn phần mềm và phát tán (redistribute) tệp tin cài đặt thì bắt buộc phải mở nguồn phần mềm đó. Tuy nhiên, các nhà cung cấp dịch vụ đám mây lớn (như AWS) đã lách luật bằng cách đóng gói MongoDB thành dịch vụ đám mây cho thuê trực tiếp mà không cần phân phối tệp tin cài đặt cho người dùng, từ đó tránh được việc phải mở nguồn phần mềm chỉnh sửa của họ. MongoDB công bố chuyển sang giấy phép mới SSPL quy định rõ: bất kỳ hãng nào thương mại hóa dịch vụ MongoDB trên đám mây bắt buộc phải mở nguồn toàn bộ hệ thống quản lý dịch vụ liên quan của họ.

5、[Công nghệ in 3D nhà đất bằng chất liệu đất bùn sinh học giá rẻ tại Ý](https://newatlas.com/wasp-gaia-3d-printed-mud-hut/56777/)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110906.jpg)

Một doanh nghiệp in 3D của Ý đã giới thiệu dự án xây nhà bằng chất liệu bùn đất tự nhiên kết hợp sợi rơm khô. Đầu phun robot sẽ phun từng lớp bùn đất đắp thành bức tường bao che vững chắc cho căn nhà nhỏ với chi phí vật liệu siêu rẻ chỉ khoảng 1.000 euro cho mỗi căn nhà.

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110907.jpg)

6、[Thành phố Istanbul thử nghiệm máy đổi vỏ chai nước lấy điểm vé tàu điện ngầm](https://www.nytimes.com/2018/10/17/world/europe/istanbul-vending-machines-recycling-subway.html)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110908.jpg)

Nhằm nâng cao ý thức tái chế rác thải nhựa, hệ thống tàu điện ngầm Istanbul đã lắp đặt các máy thu hồi rác tự động. Khách đi tàu chỉ cần bỏ các vỏ chai nhựa hoặc lon nước ngọt vào máy để tích lũy điểm thưởng nạp trực tiếp vào thẻ đi tàu điện ngầm.

7. **Báo cáo nghiên cứu khoa học ước tính tổng sinh khối carbon của sinh vật trên Trái Đất**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110909.jpg)

Nghiên cứu của Viện Khoa học Quốc gia Mỹ ước tính tổng khối lượng carbon sinh học trên Trái Đất đạt khoảng 550 tỷ tấn. Trong đó, giới thực vật chiếm tỷ trọng tuyệt đối với 450 tỷ tấn, tiếp theo là vi khuẩn (70 tỷ tấn) và nấm (12 tỷ tấn). Toàn bộ giới động vật chỉ chiếm vỏn vẹn 2 tỷ tấn carbon, và tổng sinh khối của toàn bộ loài người chỉ chiếm khoảng 0.06 tỷ tấn.

8、[Phát hiện xác tàu cổ đại nguyên vẹn nhất lịch sử dưới đáy Biển Đen](https://www.theguardian.com/science/2018/oct/23/oldest-intact-shipwreck-thought-to-be-ancient-greek-discovered-at-bottom-of-black-sea)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110910.jpg)

Các nhà khảo cổ học đại dương phát hiện xác một con tàu buôn cổ đại của Hy Lạp dài 23 mét nằm im lìm dưới độ sâu hơn 2.000 mét ở Biển Đen. Do môi trường nước sâu thiếu oxy tuyệt đối giúp ngăn chặn quá trình phân hủy gỗ, con tàu 2.700 năm tuổi vẫn giữ được cấu trúc cột buồm, bánh lái và các băng ghế chèo thuyền nguyên vẹn hoàn hảo như lúc mới chìm.

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110911.jpg)

9. **Nghị viện Châu Âu thông qua dự luật cấm sử dụng đồ nhựa dùng một lần từ năm 2021**

Để giảm thiểu thảm họa ô nhiễm rác thải nhựa đại dương, EU đã bỏ phiếu thông qua luật cấm hoàn toàn việc sản xuất và tiêu dùng các sản phẩm nhựa dùng một lần như ống hút nhựa, tăm bông, đĩa và thìa dĩa nhựa trên toàn bộ lãnh thổ từ năm 2021.

## 教程 (Hướng dẫn)

1、[Bài viết] [Tìm hiểu về vẻ đẹp toán học của các thuật toán nén dữ liệu Deflate](http://www.codersnotes.com/notes/elegance-of-deflate/) (Tiếng Anh)

Phân tích nguyên lý của hai phương pháp nén dữ liệu kinh điển: nén dựa trên lý thuyết entropy (mã hóa Huffman) và nén dựa trên từ khóa lặp lại (LZ77), giải thích cách thuật toán Deflate kết hợp hai phương pháp này để tối ưu hóa nén tệp tin zip.

2、[Bài viết] [Trải nghiệm hệ điều hành Manjaro Linux giao diện tối giản Deepin](https://hackernoon.com/manjaro-deepin-review-a-clean-minimal-and-powerful-linux-distro-6c0ccac04cd8) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110914.jpg)

Giới thiệu các tính năng nổi bật của bản phân phối Manjaro Linux chạy trên nhân Arch Linux ổn định kết hợp giao diện máy tính để bàn (DE) Deepin trực quan đẹp mắt.

3、[Bài viết] [Lý do các website nên cân nhắc hạn chế sử dụng tính năng cuộn vô hạn (Infinite Scroll)](https://logrocket.com/blog/infinite-scroll/) (Tiếng Anh)

Phân tích các bất cập về mặt trải nghiệm người dùng (UX) và hiệu năng của tính năng infinite scroll: gây khó khăn cho việc định vị chân trang (footer), làm tăng đột biến lượng sử dụng bộ nhớ của trình duyệt và ảnh hưởng đến SEO do khó thu thập dữ liệu nội dung ở sâu phía dưới.

4、[Bài viết] [Tìm hiểu các đề xuất cải tiến kỹ thuật tương lai của WebAssembly](https://hacks.mozilla.org/2018/10/webassemblys-post-mvp-future/) (Tiếng Anh)

Giới thiệu lộ trình phát triển của WebAssembly hỗ trợ các tính năng đa luồng (threads), Garbage Collection và tích hợp module trực tiếp vào ES6 để hỗ trợ chạy các chương trình hiệu năng cao trên web.

## 资源 (Tài nguyên)

1、[Học tập] [Giáo trình toán học lý thuyết căn bản nguồn mở (Infinite Descent)](https://infinitedescent.xyz/)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110916.jpg)

Sách giáo khoa điện tử giới thiệu các khái niệm toán học nền tảng từ tập hợp số tự nhiên, đại số học, lý thuyết số cho đến xác suất thống kê dành cho người học khoa học máy tính.

2、[Thư viện] [Tổng hợp các mẫu thiết kế giao diện máy tính tương lai trong phim khoa học viễn tưởng](http://sciencefictioninterfaces.tumblr.com/)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110918.jpg)

Trang web tổng hợp và phân tích các giao diện hiển thị đồ họa (FUI) độc đáo xuất hiện trong các bộ phim sci-fi nổi tiếng để các nhà thiết kế tìm kiếm ý tưởng giao diện người dùng.

## 工具 (Công cụ)

1、[arwes — Bộ thư viện component React phong cách khoa học viễn tưởng](https://github.com/arwesjs/arwes)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110921.jpg)

Một bộ UI kit độc đáo dành cho React hỗ trợ tạo các hiệu ứng âm thanh nút bấm và khung viền neon phát sáng mang đậm hơi hướng thiết kế phim viễn tưởng cyber.

2、[irondb — Thư viện đóng gói cơ chế lưu trữ dữ liệu phía Client redundancy](https://github.com/gruns/irondb)

Thư viện JavaScript hỗ trợ hợp nhất các API lưu trữ Cookies, IndexedDB, LocalStorage và SessionStorage trên trình duyệt thành một giao diện duy nhất, tự động sao lưu chéo dữ liệu để đảm bảo thông tin không bị mất khi người dùng xóa cache trình duyệt.

3、[Sketch2Code — Công cụ AI chuyển đổi bản vẽ phác thảo tay thành code HTML của Microsoft](https://sketch2code.azurewebsites.net/)

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110924.jpg)

Dịch vụ đám mây ứng dụng thị giác máy tính của Microsoft hỗ trợ nhận diện các nét vẽ nút bấm, ô nhập liệu vẽ tay trên giấy và tự động sinh ra mã nguồn giao diện HTML tương ứng mượt mà.

## 文摘 (Văn trích)

1. **Ý tưởng táo bạo về dự án xây dựng thuộc địa lơ lửng trên tầng khí quyển Sao Kim**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110926.jpg)

Mặc dù bề mặt Sao Kim có nhiệt độ cực cao (460 độ C làm nóng chảy cả kim loại) và áp suất khí quyển khổng lồ 93 atm, cơ quan NASA đang nghiên cứu dự án HAVOC hướng tới xây dựng căn cứ lơ lửng ở độ cao 50 km trong bầu khí quyển của hành tinh này. Ở độ cao này, nhiệt độ duy trì ở mức lý tưởng 20-30 độ C và áp suất tương đương Trái Đất. Các phi hành gia có thể sinh sống trong các khinh khí cầu khổng lồ chứa hỗn hợp khí oxy và nitơ thông thường (do hỗn hợp này nhẹ hơn khí CO2 của khí quyển Sao Kim nên tự tạo lực nâng lớn), giúp tránh được bức xạ vũ trụ và khai thác hiệu quả năng lượng mặt trời.

2. **So sánh ba mô hình quản lý quyền sở hữu mã nguồn trong doanh nghiệp**

Nhà nghiên cứu Martin Fowler phân loại ba cơ chế quản lý code phổ biến:
* **Quyền sở hữu mạnh (Strong Code Ownership):** Mỗi module do một kỹ sư làm chủ, người khác muốn sửa phải gửi yêu cầu hoặc viết patch để chủ module phê duyệt. Giúp bảo vệ chất lượng code tốt nhất.
* **Quyền sở hữu yếu (Weak Code Ownership):** Có người chịu trách nhiệm chính nhưng các lập trình viên khác vẫn có thể chủ động sửa code sau khi thảo luận.
* **Quyền sở hữu tập thể (Collective Code Ownership):** Toàn bộ nhóm làm chủ code, ai cũng có quyền sửa mọi vị trí. Đây là mô hình phổ biến hiện nay nhưng dễ dẫn đến tình trạng cha chung không ai khóc làm giảm sút chất lượng mã nguồn.

## 本周图片 (Hình ảnh tuần này)

1. **Hệ thống bảo tàng lưu trữ các sự cố tai nạn đường sắt của hãng JR Nhật Bản**

![](https://cdn.beekka.com/blogimg/asset/201811/bg2018110934.jpg)

Hãng đường sắt quốc gia Nhật Bản duy trì một trung tâm lưu trữ hình ảnh hiện trường các vụ tai nạn tàu hỏa lịch sử. Trung tâm hoạt động như một cơ sở giáo dục nội bộ bắt buộc đối với toàn bộ nhân viên mới để nhắc nhở họ luôn ghi nhớ bài học quá khứ, đề cao tinh thần cảnh giác và trách nhiệm an toàn trong vận hành đường sắt.

## 本周金句 (Kim ngôn tuần này)

1、

> "Do lực hấp dẫn trên Mặt Trăng chỉ bằng 1/6 Trái Đất, đây sẽ là thiên đường nghỉ dưỡng và chăm sóc y tế tuyệt vời cho người cao tuổi vào cuối thế kỷ này. Hệ tim mạch của người già sẽ hoạt động êm ái hơn do không phải chịu áp lực tuần hoàn lớn, và hệ xương khớp yếu của họ cũng giảm bớt được phần lớn tải trọng nâng đỡ cơ thể."
> 
> -- Robert A. Heinlein (Nhà viết tiểu thuyết khoa học viễn tưởng, chia sẻ năm 1969)

2、

> "Điểm cộng lớn của JavaScript là bạn có thể dùng nó để lập trình ra bất kỳ thứ gì trên đời, nhưng điểm trừ lớn nhất lại là việc các lập trình viên thực sự đi dùng nó để viết ra tất cả những thứ kỳ quặc đó."
> 
> -- Reg Braithwaite

(Hết)
