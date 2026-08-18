# Bản tin chia sẻ công nghệ (Số 349): Những nhà phát minh của thuật toán mạng thần kinh

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/6771) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052105.webp)

Một đoạn đường xanh đi bộ công cộng dọc bờ sông hộ thành tại Bắc Kinh, tọa lạc gần khu vực Cổ Lâu. (Nguồn: [visuals_china@instagram](https://www.instagram.com/p/DJi3qkuOTZ5/))

## 神经网络算法的发明者

Tiếp nối nội dung từ bài chia sẻ [《Đọc hồi ký của Giáo sư Li Fei-Fei》](https://www.ruanyifeng.com/blog/2025/05/weekly-issue-348.html) của tuần trước, câu chuyện này vẫn còn những diễn biến thú vị phía sau.

Bài viết trước đã kết thúc ở sự kiện mùa giải ILSVRC năm 2012 khi một đội ngũ nghiên cứu đến từ Canada đã ứng dụng thuật toán mạng thần kinh nhân tạo để bất ngờ giành chức vô địch giải đấu ImageNet một cách thuyết phục.

Hôm nay tôi muốn kể chi tiết hơn về câu chuyện của đội ngũ nghiên cứu đến từ Canada này.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052104.webp)

Qua câu chuyện, các bạn sẽ hiểu sâu sắc hơn về hành trình ra đời của thuật toán mạng thần kinh nhân tạo và những bộ óc vĩ đại đứng sau thúc đẩy sự phát triển của nó.

### （1）Geoffrey Hinton (Sinh năm 1947)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051807.webp)

Giáo sư Hinton sinh ra tại Anh, sau đó chuyển dịch sang sinh sống và giảng dạy tại Canada. Ông được tôn vinh là người đặt nền móng và là nhà phát minh nòng cốt của thuật toán mạng thần kinh nhân tạo.

Về lịch sử, ý tưởng sơ khởi về mạng thần kinh nhân tạo thực tế đã được giới khoa học đề xuất từ cuối những năm 1940 (không phải do Hinton đề xuất). Lập luận lúc bấy giờ vô cùng đơn giản: Nếu bộ não con người tư duy dựa trên mạng lưới các tế bào thần kinh sinh học, thì chỉ cần xây dựng máy tính mô phỏng lại cấu trúc mạng lưới đó là máy móc có thể tự học cách tư duy.

Tuy nhiên, ý tưởng đó chỉ dừng lại ở mức độ lý thuyết trừu tượng mà hoàn toàn thiếu vắng đi các thuật toán thực thi cụ thể. Làm thế nào để lập trình cho máy tính mô phỏng được quy trình tư duy đó là bài toán chưa có lời giải suốt nhiều thập kỷ.

Năm 1984, trong thời gian làm nghiên cứu sinh sau tiến sĩ tại Đại học California, giáo sư Hinton cùng hai đồng nghiệp đã chính thức công bố thuật toán lan truyền ngược (Backpropagation).

Thuật toán này cho phép xây dựng cấu trúc mạng lưới tính toán gồm nhiều tầng sâu (multi-layer network) để xử lý dữ liệu và kết xuất kết quả đầu ra chuẩn xác, đưa lý thuyết mạng thần kinh chính thức bước vào ứng dụng thực tế và đặt bệ phóng cho toàn bộ các thuật toán nâng cao sau này.

Do mô hình đòi hỏi quy trình tính toán đa tầng sâu, nơi tầng tính toán phía sau sẽ liên tục học tập và tối ưu hóa dựa trên kết quả xử lý của tầng phía trước, công nghệ này được đặt tên là "Học sâu" (Deep Learning), và giáo sư Hinton được tôn vinh là "Cha đẻ của Học sâu".

Nhờ những cống hiến vĩ đại này cho nhân loại, giáo sư Hinton đã vinh dự được trao tặng giải thưởng Turing (năm 2018) và giải thưởng Nobel Vật lý (năm 2024).

### （2）Yann LeCun (Sinh năm 1960)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051808.webp)

Yann André LeCun (thường được gọi bằng tên tiếng Trung là Dương Lập Côn) là một nhà khoa học người Pháp. Vào những năm 1980, ông tham gia nghiên cứu sau tiến sĩ tại Đại học Toronto.

Trong giai đoạn này, giáo sư Hinton cũng chuyển về giảng dạy tại Đại học Toronto và trực tiếp đảm nhận vai trò giảng viên hướng dẫn nghiên cứu cho Yann LeCun.

Do đó, Yann LeCun chính là học trò xuất sắc thế hệ đầu tiên của Hinton, chịu trách nhiệm kế thừa và phát triển sâu hơn các thuật toán của người thầy. Cống hiến kỹ thuật lớn nhất của ông là việc tích hợp thuật toán tích chập (convolution) vào cấu trúc mạng thần kinh để kiến tạo nên mô hình mạng thần kinh tích chập (Convolutional Neural Networks - CNN), và tự tay phát triển ứng dụng mạng thần kinh thương mại đầu tiên trong lịch sử.

Vào những năm 1990, ông đã ứng dụng mạng thần kinh tích chập để nhận diện các chữ số viết tay trên séc ngân hàng và được các tổ chức tài chính đưa vào vận hành thực tế thành công.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051809.webp)

Tuy nhiên, ứng dụng thực tế này cũng vô tình phơi bày điểm yếu chí tử của mô hình CNN lúc bấy giờ: Mô hình đòi hỏi quy trình huấn luyện trên lượng mẫu thử cực kỳ khổng lồ, ngốn năng lực tính toán vượt xa giới hạn phần cứng thời kỳ đó. Bài toán nhận diện séc ngân hàng thực chất chỉ yêu cầu nhận diện 10 chữ số Ả Rập cơ bản, nếu chuyển dịch sang các kịch bản nhận diện hình ảnh đa dạng ngoài đời thực, năng lực máy tính thời kỳ đó hoàn toàn không thể xử lý nổi.

Hệ quả là giới khoa học máy tính đồng loạt đưa ra nhận định mô hình CNN chỉ phù hợp xử lý các tác vụ chuyên biệt có quy mô tính toán nhỏ, hoàn toàn thiếu đi giá trị ứng dụng thực tiễn rộng rãi. Nhận định bi quan này đã đẩy thuật toán CNN, cùng hai nhà khoa học Hinton và Yann LeCun vào thời kỳ bị cộng đồng học thuật ghẻ lạnh kéo dài suốt hai thập kỷ.

Trong suốt 20 năm trầm lặng đó, Yann LeCun vẫn kiên trì nghiên cứu tại các phòng thí nghiệm của doanh nghiệp và giảng dạy tại các giảng đường đại học. Chỉ đến khi thế giới công nghệ tái phát hiện ra sức mạnh vĩ đại của CNN, ông đã vinh dự cùng người thầy Hinton nhận giải thưởng Turing vào năm 2018. Hiện tại, ông đang đảm nhận vai trò Phó chủ tịch kiêm Kỹ sư trưởng khoa học AI tại tập đoàn Meta.

### （3）Alex Krizhevsky (Sinh năm 1986)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051810.webp)

Alex Krizhevsky sinh ra tại Ukraine, sau đó cùng gia đình di cư sang Canada từ thuở nhỏ. Năm 2007, anh theo học nghiên cứu sinh tại Đại học Toronto và trở thành học trò trực tiếp của giáo sư Hinton.

Thời điểm này đã cách cột mốc Yann LeCun đề xuất mô hình CNN gần 20 năm. Giáo sư Hinton chưa bao giờ từ bỏ niềm tin vào thuật toán này. Ông đã động viên Alex cùng một người bạn học khác là Ilya Sutskever (sẽ được giới thiệu ở phần sau) thử nghiệm ứng dụng thuật toán CNN để tham gia thách thức giải đấu ImageNet của cô Li Fei-Fei.

Alex đã thiết lập một chương trình phần mềm ứng dụng mô hình CNN để huấn luyện trên kho dữ liệu 15 triệu bức ảnh của ImageNet. Tuy nhiên khối lượng phép tính khổng lồ vượt quá năng lực xử lý của chiếc máy tính cá nhân thông thường của anh. Để giải quyết, Alex đã chi tiền mua 2 chiếc card đồ họa Nvidia chuyên dụng và cấu hình cho chúng chạy tính toán liên tục 24/7 không ngừng nghỉ.

Kết quả thực tế chứng minh sự kết hợp hoàn hảo giữa cấu trúc mạng thần kinh tích chập + kho dữ liệu huấn luyện khổng lồ + phần cứng tính toán tốc độ cao (GPU) đã tạo ra sức mạnh vượt trội đè bẹp toàn bộ các thuật toán lập trình truyền thống khác trên thị trường. Chung cuộc, đội ngũ 3 thành viên của họ đã giành chiến thắng áp đảo tại giải đấu ImageNet năm 2012.

Sự kiện đã tạo nên tiếng vang khổng lồ trong giới công nghệ, khiến các tập đoàn công nghệ lớn liên tục gửi lời mời hợp tác đến giáo sư Hinton và các học trò. Tập đoàn Baidu của Trung Quốc đã đưa ra đề nghị rất hấp dẫn mời Hinton đảm nhận vai trò Kỹ sư trưởng khoa học, nhưng cuối cùng đã bị Google vượt qua.

Năm 2013, Google đã chi tới 44 triệu USD để mua lại công ty start-up của Hinton (thực chất chỉ là một công ty vỏ bọc chưa có sản phẩm thương mại) để tuyển dụng cả 3 thành viên Hinton, Alex và Ilya về đầu quân cho hãng.

Đến năm 2017, Alex quyết định từ chức tại Google để chuyển sang làm nghiên cứu công nghệ AI tại một doanh nghiệp khởi nghiệp độc lập.

### （4）Ilya Sutskever (Sinh năm 1986)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051811.webp)

Ilya Sutskever sinh ra tại Liên Xô cũ, sau đó cùng gia đình chuyển sang Israel và cuối cùng định cư tại Canada. Anh là bạn học nghiên cứu sinh cùng khóa với Alex Krizhevsky tại Đại học Toronto dưới sự hướng dẫn của giáo sư Hinton.

Anh đã cùng Alex thiết lập đội ngũ kỹ thuật xuất sắc giành chức vô địch giải đấu ImageNet năm 2012 (với giáo sư Hinton tham gia với vai trò cố vấn định hướng).

Năm 2013, anh cùng người thầy đầu quân cho Google, sau đó từ chức vào năm 2015 để trở thành nhà đồng sáng lập kiêm Kỹ sư trưởng khoa học tại OpenAI, và là một trong những tác giả nòng cốt đặt nền móng cho sự ra đời của ChatGPT. Năm 2024, anh quyết định rời OpenAI để tự thành lập một công ty AI độc lập cho riêng mình.

### （5）Andrej Karpathy (Sinh năm 1986)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051812.webp)

Andrej Karpathy sinh ra tại Slovakia, cùng gia đình di cư sang Canada năm 15 tuổi và hoàn thành chương trình cử nhân tại Đại học Toronto.

Anh và Ilya Sutskever nhiều khả năng đã quen biết nhau từ những năm học đại học tại Toronto. Tuy nhiên, anh quyết định không học tiếp tiến sĩ tại Toronto mà chuyển sang Stanford dưới sự hướng dẫn của cô Li Fei-Fei.

Lĩnh vực nghiên cứu sâu của anh cũng tập trung vào mô hình mạng CNN. Trong thời gian học tiến sĩ tại Stanford, anh chính là người trực tiếp biên soạn giáo trình và đứng lớp giảng dạy khóa học chuyên đề về Học sâu đầu tiên của trường.

Năm 2015, anh cùng Ilya gia nhập OpenAI thời kỳ đầu và là nhân sự nghiên cứu nòng cốt của hãng.

Đến năm 2017, anh rời OpenAI để đầu quân cho hãng xe điện Tesla đảm nhận vai trò Giám đốc bộ phận AI, phụ trách phát triển hệ thống tự lái Autopilot, trước khi chính thức từ chức vào năm 2022.

### （6）Tổng kết

5 gương mặt giới thiệu ở trên chính là những bộ óc vĩ đại đã đặt nền móng và thúc đẩy sự phát triển của thuật toán mạng thần kinh nhân tạo. Thiếu đi sự cống hiến của họ, thế giới công nghệ ngày nay sẽ không có sự xuất hiện của các mô hình ngôn ngữ lớn AI.

Tuy nhiên, nếu chỉ dựa vào các thuật toán toán học của họ, làn sóng AI cũng khó có thể đi đến thành công. Bởi lẽ thuật toán bắt buộc phải được huấn luyện trên nguồn dữ liệu khổng lồ, và quy trình huấn luyện đòi hỏi hạ tầng phần cứng xử lý tốc độ cao. Đây là mối quan hệ kiềng ba chân không thể tách rời.

Chỉ đến mốc lịch sử năm 2012, cả 3 điều kiện cốt lõi này mới cùng hội tụ đầy đủ: Thuật toán mạng thần kinh tích chập của Hinton + kho dữ liệu huấn luyện ImageNet của Li Fei-Fei + hạ tầng card đồ họa GPU tốc độ cao của Nvidia.

Lịch sử công nghệ thế giới chính thức lật sang trang mới, mở ra kỷ nguyên AI bùng nổ của nhân loại.

## 科技动态

（1）Một doanh nghiệp tại Thâm Quyến vừa giới thiệu dòng sản phẩm vỏ case máy tính dành cho Raspberry Pi 5 với phong cách vô cùng hầm hố.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051009.webp)

Vỏ case được thiết kế tích hợp sẵn một màn hình hiển thị trạng thái mini, hệ thống đèn LED trang trí RGB bắt mắt, quạt tản nhiệt hiệu năng cao cùng bo mạch mở rộng hỗ trợ lắp đặt hai ổ cứng SSD NVMe, rất thích hợp cho nhu cầu tự dựng máy chủ NAS gia đình hoặc hệ thống tính toán AI biên (Edge Computing).

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051010.webp)

（2）Chính quyền Phần Lan đang triển khai chương trình phun sơn phản quang lên phần sừng của đàn tuần lộc hoang dã.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025042409.webp)

Giải pháp nhằm mục đích giúp các tài xế dễ dàng nhận diện đàn tuần lộc từ xa khi di chuyển trên đường vào ban đêm, giúp giảm thiểu con số thống kê trung bình khoảng 4.000 con tuần lộc bị ô tô đâm chết hằng năm tại quốc gia này.

（3）Dịch vụ họp trực tuyến Google Meet công bố tính năng mới hỗ trợ **dịch thuật giọng nói thời gian thực**, bước đầu tiên hỗ trợ chuyển dịch từ tiếng Tây Ban Nha.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052203.webp)

Trong cuộc họp trực tuyến, khi đối tác phát ngôn bằng tiếng Tây Ban Nha, hệ thống sẽ tự động dịch và phát ra tiếng Anh cho bạn nghe, đồng thời bảo đảm giữ nguyên tông giọng, ngữ điệu và cảm xúc của người nói gốc.

（4）Tổ chức phần cứng mã nguồn mở Arduino giới thiệu nguyên mẫu bo mạch mạch in (PCB) sử dụng vật liệu sinh học dễ phân hủy nhằm giảm thiểu ô nhiễm rác thải điện tử ra môi trường.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051201.webp)

Thay vì sử dụng các sợi thủy tinh và nhựa tổng hợp truyền thống khó phân hủy, bo mạch mới ứng dụng các sợi亞麻 (sợi lanh) tự nhiên làm đế để in các đường mạch dẫn điện.

Tuy nhiên, phần kim loại đồng trên mạch vẫn chưa thể tự phân hủy, đòi hỏi người dùng thực hiện tách lọc thu hồi kim loại trước khi thải bỏ bo mạch ra môi trường.

（5）Một doanh nghiệp khởi nghiệp tại Mỹ đề xuất dự án độc đáo nhằm phóng các vệ tinh chuyên dụng để **xây dựng hệ thống máy chủ AI trực tiếp ngoài không gian vũ trụ** (Starcloud).

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051403.webp)

Hệ thống máy chủ sẽ tận dụng nguồn năng lượng mặt trời dồi dào sẵn có 24/7 ngoài không gian để vận hành, đồng thời giải quyết triệt để bài toán tản nhiệt nhờ nhiệt độ cực lạnh của vũ trụ.

Dự án kỳ vọng sẽ giải quyết triệt để bài toán khủng hoảng năng lượng tiêu thụ điện và chi phí làm mát khổng lồ của các trung tâm dữ liệu AI dưới mặt đất hiện nay.

## 文章

1、[Hướng dẫn thiết lập môi trường chạy Linux Desktop trực tiếp trên điện thoại di động kết hợp cùng kính AR](https://holdtherobot.com/blog/2025/05/11/linux-on-android-with-ar-glasses/) (tiếng Anh)

Tác giả chia sẻ giải pháp làm việc di động tối giản khi đi công tác mà không mang theo máy tính xách tay, chỉ sử dụng một chiếc điện thoại di động kết hợp cùng bàn phím bluetooth và kính AR thông minh.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051903.webp)

Chiếc điện thoại Android sau khi được can thiệp quyền hệ thống (Root) đã được thiết lập cài đặt một bản phân phối Linux hoàn chỉnh thông qua cơ chế chroot, cho phép kết xuất giao diện làm việc desktop mượt mà lên kính AR.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051904.webp)

2、[Phân tích logic vận hành cốt lõi của các ứng dụng AI Agent](https://sketch.dev/blog/agent-loop) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051905.webp)

Tác giả bài viết chia sẻ quan điểm cho rằng cấu trúc logic vận hành cốt lõi bên dưới của các ứng dụng tác vụ AI (AI Agent) thực chất chỉ cần gói gọn trong vòng 9 dòng code cơ bản.

3、[Tổng hợp danh sách các cổng kết nối (Ports) bị trình duyệt web mặc định chặn truy cập](https://www.keenformatics.com/ports-that-are-blocked-by-browsers) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025051906.webp)

Nhiều nhà phát triển có thể chưa biết lý do tại sao trình duyệt web mặc định từ chối kết nối đến địa chỉ chạy thử nghiệm cục bộ dạng `localhost:6000`. Bài viết giải thích chi tiết về quy chuẩn bảo mật quy định các cổng kết nối bị trình duyệt tự động chặn lọc để phòng tránh các đợt tấn công chéo.

4、[Đánh giá và đề xuất ứng dụng truy cập máy tính từ xa mã nguồn mở RustDesk](https://www.xda-developers.com/i-tried-every-method-to-remotely-access-my-pc-this-method-is-the-best/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025040506.webp)

Tác giả chia sẻ kinh nghiệm sử dụng các giải pháp kết nối điều khiển máy tính Windows từ xa trên máy Mac, đưa ra các nhận xét đánh giá cao về hiệu năng vận hành mượt mà và tính an toàn của công cụ mã nguồn mở RustDesk.

5、[Các mẹo định dạng CSS chuyên dụng cho phần tử `<dialog>` trong HTML](https://cassidoo.co/post/css-for-dialogs/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025011910.webp)

Ngôn ngữ HTML cung cấp sẵn một phần tử hiển thị hộp thoại pop-up mặc định là `<dialog>`. Bài viết hướng dẫn hai mẹo định dạng CSS hữu ích để tùy biến giao diện hiển thị của hộp thoại này đẹp mắt hơn.

6、[Tìm hiểu chi tiết về các câu lệnh cấu hình Git của các nhà phát triển lõi](https://blog.gitbutler.com/how-git-core-devs-configure-git/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022504.webp)

Bài viết giải thích cặn kẽ ý nghĩa kỹ thuật và hướng dẫn cấu hình các tùy biến thông dụng nhất của câu lệnh `git config` giúp tối ưu hóa quy trình làm việc với kho chứa Git.

## 工具

1、[Pyrefly](https://github.com/facebook/pyrefly/)

Công cụ kiểm tra kiểu dữ liệu (static type checker) chuyên dụng cho mã nguồn Python do tập đoàn Meta nghiên cứu phát triển và chia sẻ mã nguồn mở. Xem thêm bài viết [giới thiệu chi tiết từ hãng](https://engineering.fb.com/2025/05/15/developer-tools/introducing-pyrefly-a-new-type-checker-and-ide-experience-for-python/).

2、[Zen Browser](https://github.com/zen-browser/desktop)

Dòng trình duyệt web mã nguồn mở mới phát triển dựa trên nhân Firefox, nhận được nhiều đánh giá tích cực từ cộng đồng công nghệ quốc tế nhờ giao diện tối giản hiện đại và tốc độ tải trang nhanh. Xem thêm bài viết [đánh giá chi tiết](https://www.xda-developers.com/zen-browser-better-brave-arc-chrome/).

3、[xtool](https://github.com/xtool-org/xtool)

Công cụ thay thế cho bộ IDE Xcode truyền thống, cho phép lập trình viên phát triển và biên dịch các ứng dụng iOS trực tiếp trên các hệ điều hành Linux hoặc Windows.

4、[Zero Convert](https://nextbconvert.com/)

Dịch vụ web hỗ trợ chuyển đổi định dạng tệp tin hàng loạt trực tuyến, vận hành dựa trên lõi công nghệ WebAssembly giúp xử lý dữ liệu hoàn toàn cục bộ ngay trên trình duyệt máy khách mà không cần tải tệp tin lên máy chủ, hỗ trợ thêm các tính năng chỉnh sửa ảnh cơ bản. (Đóng góp từ [@xiaoshangmin](https://github.com/ruanyf/weekly/issues/6864))

5、[Háo Tử Diện Bản (耗子面板)](https://github.com/tnb-labs/panel)

Dự án xây dựng hệ thống bảng điều khiển quản trị máy chủ (Server Management Panel) mã nguồn mở phát triển trên ngôn ngữ Go. (Đóng góp từ [@devhaozi](https://github.com/ruanyf/weekly/issues/6881))

6、[Goravel](https://github.com/goravel/goravel)

Bộ khung phát triển ứng dụng Web (Web Framework) trên ngôn ngữ Go, được thiết kế mô phỏng chuẩn xác theo triết lý cấu trúc của framework Laravel nổi tiếng trong PHP giúp lập trình viên Laravel dễ dàng tiếp cận. (Đóng góp từ [@devhaozi](https://github.com/ruanyf/weekly/issues/6882))

7、[OpenSpeedy](https://github.com/game1024/OpenSpeedy)

Công cụ mã nguồn mở hỗ trợ điều chỉnh tốc độ vận hành của các tựa game chạy trên Windows thông qua việc can thiệp thay đổi các hàm đếm thời gian hệ thống. (Đóng góp từ [@game1024](https://github.com/ruanyf/weekly/issues/6884))

8、[SimonAKing-Gallery](https://github.com/SimonAKing/AnimatedGallery)

Ứng dụng album ảnh web mã nguồn mở phát triển trên Node.js, hỗ trợ hiển thị kho ảnh cá nhân dưới dạng bố cục thác nước (waterfall layout) trực quan, chỉ cần cấu hình đường dẫn thư mục ảnh là ứng dụng có thể tự động quét và chạy ngay. (Đóng góp từ [@SimonAKing](https://github.com/ruanyf/weekly/issues/6886))

9、[Jwno](https://github.com/agent-kilo/jwno)

Dự án mã nguồn mở xây dựng trình quản lý sắp xếp cửa sổ dạng gạch (Tiling Window Manager) dành cho Windows 10/11, hỗ trợ điều khiển hoàn toàn bằng phím tắt bàn phím tiện lợi. (Đóng góp từ [@agent-kilo](https://github.com/ruanyf/weekly/issues/6891))

10、[Tinh Hà Tiểu Trình Tự (星河小程序 - Dimina)](https://github.com/didi/dimina)

Bộ khung phát triển đa nền tảng do tập đoàn Didi chia sẻ mã nguồn mở, hỗ trợ đóng gói mã nguồn của ứng dụng nhỏ (Mini Program) thành các ứng dụng chạy native trên cả 4 nền tảng di động lớn là Android, iOS, HarmonyOS và Web. (Đóng góp từ [@dos1in](https://github.com/ruanyf/weekly/issues/6912))

## AI 相关

1、[aTrain](https://github.com/JuergenFleiss/aTrain)

Ứng dụng máy tính mã nguồn mở hỗ trợ nhận diện và chuyển đổi giọng nói thành văn bản trực quan, hoạt động dựa trên mô hình Whisper của OpenAI và hỗ trợ nhận diện hơn 50 ngôn ngữ khác nhau. Xem thêm bài viết [giới thiệu chi tiết trải nghiệm](https://www.xda-developers.com/i-switched-from-otter-to-this-self-hosted-audio-transcription-app/).

2、[AI Image Editor](https://aiimageeditor.me/)

Dịch vụ trực tuyến miễn phí cung cấp bộ công cụ chỉnh sửa hình ảnh đa dạng tích hợp AI, hỗ trợ các tính năng tăng cường chất lượng ảnh, xóa logo chìm, chuyển đổi phong cách tranh vẽ... (Đóng góp từ [@worminone](https://github.com/ruanyf/weekly/issues/6883))

## 资源

1、[Vạn Vật Bác Vật Quán (Museum of All Things)](https://mayeclair.itch.io/museum-of-all-things)

Ứng dụng máy tính độc đáo hỗ trợ người dùng khám phá kho tàng kiến thức của Wikipedia dưới dạng một không gian bảo tàng ảo 3D tương tác sinh động.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031008.webp)

Mỗi gian trưng bày tương ứng với một bài viết trên Wikipedia, các bức tranh treo tường hiển thị hình ảnh minh họa và bảng thông tin ghi chú hiển thị nội dung tóm tắt của bài viết.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031009.webp)

Các lối đi hành lang sẽ dẫn người dùng chuyển tiếp sang các phòng trưng bày của các bài viết có liên kết tương ứng, mở ra một hành trình khám phá bảo tàng vô tận.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025031010.webp)

## 图片

1、[Góc khuất hậu trường của nhân vật người máy R2-D2 trong phim Star Wars](https://www.facebook.com/groups/1740302472949408/permalink/3918177945161839)

Tập đầu tiên của loạt phim điện ảnh bom tấn *Star Wars* được khởi quay từ năm 1976. Trong phim xuất hiện nhân vật người máy R2-D2 có khả năng di chuyển linh hoạt, thực hiện các tương tác cơ học và phát ra âm thanh nói chuyện độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052106.webp)

Trên thực tế thời kỳ đó chưa hề có công nghệ robot cao siêu nào đáp ứng được yêu cầu này. Để thực hiện cảnh quay, đoàn làm phim đã bố trí một diễn viên người thật có vóc dáng nhỏ nhắn ngồi ẩn nấp bên trong thân vỏ của robot để điều khiển các chuyển động thủ công.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052107.webp)

2、[Giải mã nguyên nhân vật lý khiến thể tích của nước đá lớn hơn nước lỏng](https://nautil.us/five-things-we-still-dont-know-about-water-3383/)

Nước sau khi bị đóng băng thành đá sẽ ghi nhận mức tăng thể tích khoảng 10%, dẫn đến việc khối lượng riêng của nước đá nhỏ hơn nước lỏng và giúp các tảng băng có thể nổi trên mặt nước.

Vậy nguyên nhân cấu trúc nào dẫn đến việc phình to thể tích này?

Câu trả lời nằm ở sự khác biệt rõ rệt về cấu trúc liên kết phân tử giữa hai trạng thái của nước.

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031408.webp)

Hình bên trái minh họa cấu trúc liên kết phân tử của nước lỏng thông thường, và hình bên phải minh họa cấu trúc của nước đá. Trong sơ đồ, các điểm tròn màu trắng đại diện cho nguyên tử Hydro và các điểm màu đỏ đại diện cho nguyên tử Oxy.

Có thể thấy cấu trúc của nước lỏng là các liên kết đan xen tương đối khít và dày đặc, trong khi nước đá khi đóng băng lại định hình thành các cấu trúc mạng lưới hình học rỗng với nhiều không gian trống ở giữa các phân tử. Sự xuất hiện của các khoảng trống này chính là nguyên nhân làm thể tích của khối nước đá phình to ra.

## 文摘

1、[Chiêm nghiệm từ cách đặt tên đường dẫn URL độc đáo của tập đoàn Slack](https://blog.jim-nielsen.com/2023/examples-of-great-urls/)

Slack là doanh nghiệp phát triển phần mềm giao tiếp doanh nghiệp nổi tiếng. Trên trang chủ của hãng có thiết lập trang giới thiệu thông tin doanh nghiệp. Thông thường các website hay đặt đường dẫn mặc định cho trang này là `slack.com/about`, tuy nhiên Slack đã lựa chọn một giải pháp đặt tên thú vị hơn nhiều.

Họ đặt tên thư mục gốc của trang giới thiệu là `is` (có nghĩa là "là"), và chia nhỏ các nội dung giới thiệu thành các trang con tương ứng.

Hệ quả là đường link giới thiệu chung của hãng hiển thị rất gọn gàng: `slack.com/is`.

Và đường dẫn của các trang giới thiệu chi tiết hiển thị dưới dạng các câu khẳng định trực quan:

*   `slack.com/is/team-communication` (Slack là công cụ giao tiếp đội ngũ)
*   `slack.com/is/everything-in-one-place` (Slack là nơi hội tụ mọi thông tin)
*   `slack.com/is/wherever-you-are` (Slack luôn đồng hành cùng bạn mọi nơi)

Giải pháp thông minh này giúp người dùng chỉ cần quan sát đường dẫn URL là đã thấu hiểu ngay các thông điệp cốt lõi doanh nghiệp muốn truyền tải, biến bản thân URL thành một công cụ quảng bá thương hiệu tự nhiên hiệu quả.

Ý tưởng đặt tên với từ khóa `is` này sau đó đã được rất nhiều thương hiệu công nghệ học hỏi áp dụng. Trùng hợp hơn nữa, ký tự `is` cũng chính là tên miền quốc gia cao cấp (ccTLD) của Iceland. Nhiều nhân vật nổi tiếng đã đăng ký tên miền này để làm trang cá nhân độc đáo cho mình.

Ví dụ như trang web của nữ nghệ sĩ thiết kế Jessica Hische sử dụng tên miền `jessicahische.is`, giúp cô dễ dàng thiết lập các trang giới thiệu cá nhân có dạng câu khẳng định như `jessicahische.is/xxx` vô cùng tự nhiên.

## 言论

1、

Chúng tôi dự kiến sẽ sớm chia sẻ đến các bạn một kết quả nghiên cứu công nghệ mới được hoàn thiện một cách âm thầm. Chúng tôi sẽ đặt cho nó một cái tên ít nổi bật hơn so với chatGPT để phòng tránh việc nó nhanh chóng tạo nên một cơn sốt quá lớn trên thị trường.

-- *Sam Altman, CEO của OpenAI chia sẻ*

2、

Định luật Gall thường xuyên được giới công nghệ trích dẫn: "Mọi hệ thống phức tạp hoạt động hiệu quả trong thực tế luôn được phát triển đi lên từ một hệ thống đơn giản hoạt động tốt trước đó."

Tuy nhiên, phần hệ quả của định luật này lại ít khi được mọi người nhắc tới: "Một hệ thống phức tạp được thiết kế đồ sộ ngay từ đầu mà không đi qua bước tối giản sẽ không bao giờ có thể hoạt động ổn định được. Bạn bắt buộc phải bắt đầu bằng việc xây dựng một hệ thống đơn giản chạy được trước tiên."

-- *Trích chia sẻ của nhà nghiên cứu Stack Staves*

3、

Chỉ có hai kịch bản khả thi tồn tại trong vũ trụ: Hoặc là chúng ta là sinh vật thông minh duy nhất tồn tại cô độc trong vũ trụ, hoặc là ngoài kia còn có những nền văn minh khác đồng hành cùng chúng ta. Cả hai kịch bản này đều mang lại một cảm giác đáng sợ như nhau cho nhân loại.

-- *Arthur C. Clarke, nhà văn khoa học viễn tưởng lỗi lạc người Anh chia sẻ*

4、

Hệ Mặt Trời cần tới khoảng 230 triệu năm mới hoàn thành một vòng quỹ đạo quay quanh trung tâm Dải Ngân Hà. Ở thời điểm Mặt Trời của chúng ta hoàn thành vòng quay trước đó, loài khủng long vẫn đang là sinh vật thống trị tối cao trên Trái Đất.

-- *Chia sẻ của một độc giả trên diễn đàn Reddit*

5、

Tôi đã có cơ hội trao đổi với nhiều nhà giáo dục đang giảng dạy thực tế và họ đều chia sẻ chung một nỗi lo ngại lớn: Học sinh của họ hiện nay lạm dụng ChatGPT để xử lý mọi bài tập được giao, và hệ quả là các em hầu như không tích lũy được bất kỳ kiến thức thực tế nào cho bản thân.

Xu thế này có thể dẫn tới sự ra đời của một thế hệ mới suy giảm năng lực tự chủ tư duy, phụ thuộc hoàn toàn vào những công nghệ mà bản thân họ không hề thấu hiểu cơ chế vận hành. Một khi hệ thống công nghệ đó gặp sự cố sụp đổ, thế hệ này sẽ hoàn toàn bất lực và không bao giờ có khả năng tự tái dựng lại cuộc sống từ con số không.

-- *Neal Stephenson, nhà văn khoa học viễn tưởng Mỹ (người đầu tiên sáng tạo ra khái niệm "Metaverse") chia sẻ*

## 往年回顾

- Số #302: [Chiêm nghiệm cuộc sống: Khởi nghiệp dù mang lại nhiều trải nghiệm tốt nhưng tôi không còn dám khuyến khích mọi người dấn thân nữa](https://www.ruanyifeng.com/blog/2024/05/weekly-issue-302.html)
- Số #252: [Phân tích về những nguyên nhân khiến hoạt động khởi nghiệp Internet ngày một trở nên khó khăn hơn trước](https://www.ruanyifeng.com/blog/2023/04/weekly-issue-252.html)
- Số #202: [Giới thiệu 3 phương pháp học tập hiệu quả giúp tiếp thu kiến thức nhanh chóng](https://www.ruanyifeng.com/blog/2022/04/weekly-issue-202.html)
- Số #152: [Câu chuyện thực tế đầy suy ngẫm về hành trình rẽ hướng sự nghiệp từ sinh viên tốt nghiệp Đại học Bắc Kinh sang trường nghề](https://www.ruanyifeng.com/blog/2021/04/weekly-issue-152.html)

(Hết)
