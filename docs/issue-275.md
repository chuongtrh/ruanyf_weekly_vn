# Bản tin chia sẻ công nghệ (Số 275): Thử nghiệm của Peter Thiel

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3529) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102101.webp)

Thật khó tin khi công trình kiến trúc có thiết kế vô cùng hiện đại và thời thượng trên đây lại chính là trạm nghiên cứu Nam Cực thứ ba của Ấn Độ mang tên Bharathi, được xây dựng hoàn thành vào năm 2012. (Nguồn: [Inhabitat](https://inhabitat.com/photos-self-sufficient-antarctic-indian-research-station-in-134-shipping-containers/))

## 彼得·蒂尔的实验

Peter Thiel (sinh năm 1967) là một trong những nhà đầu tư mạo hiểm nổi tiếng nhất tại Thung lũng Silicon.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102005.webp)

Ông được biết đến rộng rãi nhờ hai thương vụ đầu tư kinh điển: Thứ nhất, ông đồng sáng lập cổng thanh toán PayPal vào năm 1998, bốn năm sau dự án được eBay mua lại với giá 1,5 tỷ USD giúp ông thu về khoản lợi nhuận 55 triệu USD.

Thứ hai, ông chính là nhà đầu tư bên ngoài đầu tiên rót vốn vào Facebook. Năm 2004, khi Facebook thậm chí còn chưa chính thức thành lập công ty, ông đã cấp cho Mark Zuckerberg khoản vay chuyển đổi trị giá 500.000 USD. Tám năm sau, khi Facebook lên sàn, khoản đầu tư này đạt giá trị lên tới 2 tỷ USD.

Ông cũng là tác giả của cuốn sách kinh doanh nổi tiếng *“Từ không đến một”* (Zero to One), được biên soạn từ các bài giảng khóa học khởi nghiệp của ông tại Đại học Stanford vào năm 2012.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102006.webp)

Tuy nhiên, hôm nay tôi không muốn bàn về những thành tựu kinh doanh lớn này, mà muốn chia sẻ cùng bạn đọc về một dự án thử nghiệm xã hội đầy táo bạo và đi ngược lại các quy chuẩn thông thường của ông, một thử nghiệm khiến tôi vô cùng đồng cảm.

Thử nghiệm này nhằm tìm câu trả lời cho câu hỏi: Liệu các bạn trẻ muốn khởi nghiệp có thực sự bắt buộc phải hoàn thành chương trình học đại học hay không?

Peter Thiel luôn giữ quan điểm cho rằng: **rất nhiều bạn trẻ có tài năng xuất chúng đang bị hệ thống giáo dục đại học làm lãng phí thời gian và kìm hãm năng lực sáng tạo.** Bản thân ông tuy sở hữu cả bằng Cử nhân Văn học lẫn bằng Tiến sĩ Luật của Đại học Stanford danh giá, nhưng ông thẳng thắn thừa nhận việc mình cố gắng học hết các cấp học chủ yếu vì lúc đó ông hoang mang không biết mình có thể làm gì khác:

> *“Tôi cảm thấy ái ngại khi nhìn thấy những bạn trẻ ngày nay cũng đang rơi vào lối mòn giống hệt tôi năm xưa.”*
>
> *“Khi bạn chưa định hình được mình muốn làm gì với cuộc đời mình, bạn chọn đi học đại học để lấy bằng Cử nhân. Khi nhận bằng Cử nhân xong và vẫn chưa biết làm gì tiếp theo, bạn lại chọn học lên Thạc sĩ hoặc Tiến sĩ.”*
>
> *“Bản thân tôi năm xưa lựa chọn trường Luật cũng chỉ bởi đó là phương án an toàn nhất khi tôi không biết làm gì khác. Tôi không hối hận về quãng đời sinh viên của mình, nhưng nếu được làm lại từ đầu, tôi chắc chắn sẽ dành thời gian suy nghĩ để đưa ra nhiều lựa chọn đột phá hơn.”*

Ý của ông là nếu năm xưa có người định hướng và hỗ trợ phương pháp khởi nghiệp, ông rất có thể cũng đã lựa chọn bảo lưu hoặc bỏ học giữa chừng.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102208.webp)

Vào năm 2010, ông đã đưa ra một quyết định táo bạo chưa từng có: thành lập chương trình học bổng mang tên **“Thiel Fellowship”** (Học bổng Thiel). Mỗi năm, quỹ của ông sẽ tuyển chọn ra khoảng 20 sinh viên đại học xuất sắc, trao tặng cho mỗi người khoản hỗ trợ tài chính **100.000 USD** tiền mặt với một điều kiện bắt buộc duy nhất: **bạn phải lập tức bảo lưu hoặc bỏ học đại học để bắt tay vào khởi nghiệp.**

Quyết định này ngay lập tức vấp phải làn sóng chỉ trích dữ dội từ giới học thuật và truyền thông. Họ cáo buộc ông vô trách nhiệm, đưa ra những định hướng sai lệch làm hỏng tương lai của thế hệ trẻ. Hiệu trưởng Đại học Harvard thời điểm đó đã phát biểu công khai: *“Đây là dự án từ thiện mang tính định hướng sai lầm nhất, về bản chất ông ấy đang dùng tiền để dụ dỗ sinh viên bỏ học.”*

Bất chấp những lời chỉ trích, Peter Thiel vẫn kiên trì duy trì quỹ học bổng. Ông muốn hỗ trợ những bạn trẻ thực sự có khát vọng và năng lực tự chủ, đồng thời coi đây là một thử nghiệm thực tế để chứng minh những giới hạn của hệ thống giáo dục đại học đối với năng lực sáng tạo.

Đến nay, sau 13 năm triển khai, kết quả của cuộc thử nghiệm này ra sao?

Vừa qua, hãng tin Bloomberg đã thực hiện một bài thống kê chi tiết về số phận của những cựu sinh viên nhận học bổng Thiel, và **kết quả thu được khiến giới học thuật phải ngỡ ngàng**. Trong suốt thời gian qua, đã có tổng cộng 271 sinh viên nhận học bổng này, đồng nghĩa với việc Peter Thiel đã thuyết phục 271 tài năng trẻ rời giảng đường để ra đời lập nghiệp.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102209.webp)

Trong số các công ty khởi nghiệp do nhóm cựu sinh viên này thành lập, tính đến nay đã có tới **11 doanh nghiệp đạt trạng thái "Kỳ lân" (Unicorn)** – tức là được định giá trên 1 tỷ USD, trong đó có không ít doanh nghiệp công nghệ đình đám toàn cầu.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102411.webp)

Tỷ lệ 11 doanh nghiệp kỳ lân trên tổng số 271 dự án khởi nghiệp là một con số thành công cao đến kinh ngạc trong giới đầu tư mạo hiểm. Liệu những bạn trẻ này có đạt được những thành tựu vượt bậc như vậy nếu họ chọn con đường an toàn là tiếp tục ngồi trên ghế nhà trường để nhận tấm bằng tốt nghiệp?

Kết quả thực tế đã chứng minh luận điểm của Peter Thiel: đối với những cá nhân thực sự có năng lực tự chủ và khát vọng khởi nghiệp rõ ràng, giá trị mà giảng đường đại học mang lại cho họ là không nhiều, việc dấn thân sớm để hiện thực hóa ý tưởng là lựa chọn tối ưu hơn.

Bên cạnh việc làm mất đi những năm tháng thanh xuân sung sức nhất cho các thủ tục học thuật, **môi trường đại học đôi khi còn vô tình làm mài mòn ý chí dấn thân khởi nghiệp của con người.** Sau khi đã bỏ ra nhiều năm trời cùng lượng tiền bạc lớn để có được tấm bằng đại học, tâm lý chung của hầu hết mọi người là muốn tìm kiếm các công việc ổn định, thu nhập tốt và ít rủi ro tại các tập đoàn lớn để nhanh chóng thu hồi vốn, đó là lý do các ngành như tài chính, tư vấn quản trị hay công chức luôn thu hút lượng lớn nhân sự chất lượng cao.

Thử nghiệm của Peter Thiel hoàn toàn không nhằm mục đích phủ nhận giá trị của giáo dục đại học, hay cổ xúy phong trào bỏ học khởi nghiệp mù quáng. Mục tiêu của ông là chứng minh cho xã hội thấy cần thiết phải xây dựng một cơ chế phát hiện sớm những cá nhân có tố chất doanh nhân xuất sắc, hỗ trợ họ bắt tay vào sáng tạo nên những giá trị mới cho xã hội thay vì bắt buộc họ phải tuân theo lộ trình bằng cấp truyền thống.

Đối với số đông học sinh chưa xác định được đam mê và định hướng cuộc đời của mình, việc hoàn thành chương trình đại học vẫn là sự lựa chọn tốt nhất. Tuy nhiên, thay vì chỉ thụ động tiếp thu những kiến thức được nhà trường sắp đặt sẵn, bạn hãy chủ động tìm kiếm những giá trị thực tế mà bản thân mong muốn đóng góp cho xã hội.

## 科技动态

1、[Mỹ thử nghiệm tích hợp vũ khí chống tăng điều khiển từ xa lên lưng robot chó](https://www.dvidshub.net/news/456001/marines-test-emerging-technologies-combat-center)

Lực lượng Thủy quân lục chiến Hoa Kỳ mới đây đã công bố bức ảnh ghi lại cuộc thử nghiệm tích hợp hệ thống ống phóng tên lửa chống tăng điều khiển từ xa lên lưng của dòng robot chó bốn chân:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102001.webp)

Quan sát từ bức ảnh, mẫu robot chó được sử dụng trong thử nghiệm là dòng Unitree Go1 do Trung Quốc sản xuất, có mức giá bán lẻ trên thị trường dao động từ 16.000 đến 20.000 Nhân dân tệ (khoảng 55 đến 70 triệu đồng).

Thiết bị được lắp đặt thêm hệ thống ăng-ten thu phát sóng Wi-Fi công suất lớn để truyền hình ảnh camera thời gian thực về trung tâm chỉ huy. Khi người vận hành xác định chính xác mục tiêu trên màn hình, họ sẽ kích hoạt lệnh bắn tên lửa chống tăng từ xa:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102002.webp)

Trong khi chi phí chế tạo một chiếc xe tăng chiến đấu hiện đại lên tới hàng chục triệu USD, việc sử dụng các robot chó giá rẻ để tiêu diệt xe tăng là phương án tác chiến vô cùng hiệu quả về mặt chi phí, đồng thời bảo đảm an toàn tuyệt đối cho tính mạng của binh sĩ trên chiến trường. Xu hướng này cho thấy chiến tranh trong tương lai sẽ là cuộc đối đầu trực tiếp giữa các thiết bị tự hành và robot thông minh.

2、[Úc khai trương công viên động vật ảnh ảo Hologram tái hiện sinh động thế giới tự nhiên](https://www.news.com.au/travel/travel-ideas/weird-and-wonderful/hologram-zoo-opens-in-brisbane-australia/news-story/e0a3597cbf577b214df9cf720613eb51)

Tại thành phố Brisbane, Úc vừa qua đã khánh thành một công viên động vật ảnh ảo độc đáo, trưng bày hình ảnh trình chiếu của hơn 50 loài động vật hoang dã khác nhau:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102003.webp)

Khi đến tham quan, du khách sẽ được quan sát các hình ảnh lập thể 3D (Hologram) sinh động của các loài động vật chuyển động tự do trong không gian và có khả năng tương tác trực tiếp với người xem.

Công viên mang lại những trải nghiệm độc đáo mà các sở thú truyền thống không thể thực hiện được, ví dụ như hình ảnh một chú cá voi xanh khổng lồ dài 30 mét từ từ bơi lướt qua ngay trước mặt du khách trong không gian:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102004.webp)

So với mô hình sở thú truyền thống, công viên ảnh ảo sở hữu ưu điểm vượt trội về chi phí vận hành, đồng thời loại bỏ hoàn toàn việc giam cầm động vật hoang dã. Tuy nhiên, tính hấp dẫn lâu dài của mô hình này đối với du khách vẫn cần thời gian để kiểm chứng.

3、[Mẫu xe hơi SUV chạy bằng năng lượng mặt trời hoàn thành hành trình 1.000 km xuyên Maroc](https://www.cnn.com/travel/stella-terra-off-road-solar-powered-suv-morocco-hnk-spc/index.html)

Nhóm nghiên cứu tại Đại học Công nghệ Eindhoven, Hà Lan mới đây đã công bố chế tạo thành công mẫu xe ô tô SUV chạy hoàn toàn bằng năng lượng mặt trời mang tên Stella Terra, thực hiện thành công hành trình thử nghiệm vượt địa hình dài hơn 1.000 km xuyên qua Maroc:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102202.webp)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102205.webp)

Về mặt kỹ thuật, việc vận hành một chiếc xe SUV cỡ lớn hoàn toàn bằng các tấm pin mặt trời trên nóc xe là điều vô cùng khó khả thi do diện tích bề mặt pin giới hạn không thể cung cấp đủ năng lượng cho động cơ hoạt động liên tục.

Để giải quyết bài toán này, nhóm phát triển đã tập trung tối ưu giảm thiểu tối đa khối lượng của xe. Trọng lượng tổng thể của chiếc xe chỉ ở mức 1,2 tấn – nhẹ hơn khoảng 25% so với các dòng xe SUV thông thường cùng kích thước:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102204.webp)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102206.webp)

Đồng thời, xe được thiết kế kiểu dáng khí động học tối ưu để giảm lực cản của gió khi di chuyển. Khi xe dừng đỗ, phần mui phía sau có thể nâng cao và mở rộng cánh ra hai bên để tăng gấp đôi diện tích tiếp nhận ánh sáng của các tấm pin mặt trời, giúp sạc đầy pin nhanh chóng.

4、[Mỹ thử nghiệm mô hình tử cung nhân tạo ngoài cơ thể hỗ trợ nuôi dưỡng trẻ sinh non](https://www.nature.com/articles/d41586-023-02901-1)

Trẻ sinh non thường có thể trạng vô cùng yếu ớt và cần chế độ chăm sóc y tế đặc biệt. Bệnh viện Nhi Philadelphia (Mỹ) hiện đang tiến hành các bước thử nghiệm lâm sàng hệ thống tử cung nhân tạo ngoài cơ thể nhằm hỗ trợ trẻ sinh non tiếp tục phát triển hoàn thiện các cơ quan trong môi trường tối ưu:

Các nhà khoa học đã thực hiện thử nghiệm trên các chú cừu non sinh non bằng cách đặt chúng vào bên trong một chiếc túi nhựa trong suốt chứa đầy dung dịch dinh dưỡng mô phỏng chính xác môi trường nước ối bên trong tử cung mẹ:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091506.webp)

Hệ thống được trang bị một thiết bị bơm máu ngoài cơ thể kết nối trực tiếp với hệ thống động mạch và tĩnh mạch của cừu non, đảm nhận nhiệm vụ liên tục cung cấp oxy và lọc bỏ các chất thải chuyển hóa. Toàn bộ quy trình được giám sát chặt chẽ bởi hệ thống máy đo thông số sinh học:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091507.webp)

Dự án thử nghiệm này đã được triển khai từ năm 2017 và trải qua nhiều vòng cải tiến kỹ thuật. Hiện tại, Cục Quản lý Thực phẩm và Dược phẩm Hoa Kỳ (FDA) đang tiến hành đánh giá các chỉ số an toàn của dự án để xem xét cấp phép cho giai đoạn thử nghiệm lâm sàng trực tiếp trên cơ thể người.

## 机房的中间人攻击

Dịch vụ nhắn tin mã nguồn mở Jabber.ru của Nga vừa qua đã công bố một báo cáo chi tiết về một [sự cố an toàn thông tin nghiêm trọng](http://notes.valdikss.org.ru/jabber.ru-mitm/) xảy ra trên hệ thống của họ:

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102102.webp)

Hệ thống máy chủ của dịch vụ được thuê đặt tại các phòng máy lớn của Hetzner (Đức) và Linode. Tuy nhiên, các kỹ sư phát hiện ra khi người dùng kết nối tới dịch vụ, chứng chỉ SSL bảo mật trả về cho máy khách đã bị giả mạo.

Điều này đồng nghĩa với việc đã có một thực thể thực hiện cuộc tấn công trung gian (Man-in-the-Middle) ngay bên trong hạ tầng mạng của phòng máy nhằm giải mã và ghi lại toàn bộ nội dung trò chuyện của người dùng Nga trước khi chuyển tiếp dữ liệu về máy chủ gốc. Cuộc tấn công này bắt buộc phải có sự đồng thuận hoặc can thiệp kỹ thuật trực tiếp từ đội ngũ quản trị hạ tầng mạng của phòng máy.

Vẫn chưa rõ nguyên nhân tại sao các nhà cung cấp dịch vụ máy chủ uy tín như Hetzner và Linode lại cho phép hành vi can thiệp dữ liệu khách hàng này diễn ra trên hệ thống của họ, nhiều khả năng do yêu cầu pháp lý từ phía cơ quan an ninh chính phủ sở tại.

Sự cố là lời nhắc nhở quan trọng đối với người dùng: khi truyền tải các thông tin nhạy cảm, chúng ta bắt buộc phải ưu tiên lựa chọn các ứng dụng hỗ trợ cơ chế mã hóa đầu cuối (End-to-End Encryption) thực sự, nơi khóa giải mã chỉ được lưu trữ trên thiết bị cá nhân của người dùng nhằm bảo đảm an toàn dữ liệu ngay cả khi máy chủ trung gian bị thỏa hiệp.

## Bài viết

1\. [Hướng dẫn cấu hình duy trì kết nối SSH Client hoạt động liên tục không bị ngắt](https://linuxiac.com/how-to-keep-ssh-session-alive/)（Tiếng Anh）

Khi quản trị hệ thống qua giao thức SSH, kết nối thường tự động bị ngắt (timeout) nếu người dùng không gõ lệnh trong một khoảng thời gian. Bài viết hướng dẫn các phương pháp cấu hình tham số phía Client hoặc Server để định kỳ gửi gói tin kiểm tra kết nối, giúp giữ cho phiên làm việc SSH luôn hoạt động thông suốt.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081102.webp)

2\. [Hướng dẫn phương pháp kết nối Remote Desktop tới Raspberry Pi trong mạng nội bộ](https://pinggy.io/blog/iot_remote_desktop_raspberry_pi/)（Tiếng Anh）

Bài viết hướng dẫn kỹ thuật chi tiết chỉ dẫn cách thức cấu hình dịch vụ thiết lập cổng kết nối (tunneling) để giúp người dùng dễ dàng truy cập và điều khiển giao diện màn hình máy tính Raspberry Pi từ xa khi thiết bị đang đặt phía sau NAT của mạng nội bộ.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081315.webp)

3\. [So sánh trải nghiệm phát triển ứng dụng di động giữa Flutter và React Native](https://stackoverflow.blog/2022/10/31/comparing-frameworks-for-cross-platform-apps-flutter-vs-react-native/)（Tiếng Anh）

Bài viết chia sẻ góc nhìn thực tế của một lập trình viên di động khi sử dụng song song hai framework phổ biến là Flutter và React Native để xây dựng ứng dụng đa nền tảng, đưa ra các đánh giá so sánh chi tiết về hiệu năng hiển thị, tốc độ phát triển và độ lớn của cộng đồng hỗ trợ.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081401.webp)

4\. [Các phương pháp tối ưu hóa việc bỏ qua bộ nhớ đệm khi xây dựng Docker Image](https://depot.dev/blog/docker-build-no-cache)（Tiếng Anh）

Mặc định, quy trình build của Docker sẽ tận dụng lại cache của các layer trước đó để tăng tốc độ. Tuy nhiên trong nhiều trường hợp cần cập nhật thư viện mới, việc dùng cache lại gây lỗi. Bài viết hướng dẫn các tham số cấu hình giúp lập trình viên chủ động bỏ qua bộ nhớ đệm cho toàn bộ hoặc một phần cụ thể của Dockerfile khi build.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081011.webp)

5\. [Hướng dẫn ứng dụng công cụ curl để thống kê chi tiết thời gian phản hồi mạng](https://susam.net/blog/timing-with-curl.html)（Tiếng Anh）

Bài viết chia sẻ một mẹo nhỏ hữu ích: tận dụng các tham số định dạng đầu ra của công cụ dòng lệnh `curl` để đo lường và hiển thị chính xác thời gian tiêu tốn cho từng công đoạn kết nối mạng (từ phân giải tên miền DNS, thiết lập TCP Handshake cho đến hoàn tất quá trình bắt tay TLS).

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081605.webp)

6\. [Những ký niệm thời sinh viên của Linus Torvalds và sự ra đời của hệ điều hành Linux](https://lwn.net/SubscriberLink/928581/841b747332791ac4/)（Tiếng Anh）

Bài viết hồi ký đầy thú vị do một người bạn học cùng lớp đại học của Linus Torvalds biên soạn, kể về những thói quen học tập, tính cách cá nhân của Linus và những ngày đầu tiên ông bắt tay vào viết những dòng mã nguồn sơ khai đặt nền móng cho hệ điều hành Linux huyền thoại.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041501.webp)

## 工具

1、[oxc: Bộ công cụ xử lý JavaScript hiệu năng cao viết bằng ngôn ngữ Rust](https://github.com/web-infra-dev/oxc/)

Một dự án phát triển bộ công cụ Front-end (bao gồm parser, linter, formatter, type checker) viết bằng ngôn ngữ Rust, hướng tới mục tiêu tối ưu hóa tốc độ xử lý nhanh gấp hàng chục lần so với các công cụ viết bằng JavaScript truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102201.webp)

2、[TinaCMS: Hệ quản trị nội dung CMS hoạt động trực tiếp dựa trên kho lưu trữ Git](https://tina.io/)

Một giải pháp quản trị nội dung website (CMS) độc đáo: thay vì lưu trữ dữ liệu trong cơ sở dữ liệu truyền thống, hệ thống lưu trữ trực tiếp các bài viết dưới dạng file Markdown ngay trong kho lưu trữ Git của dự án, cung cấp giao diện chỉnh sửa trực quan cho người dùng.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102404.webp)

3、[Writerside: Trình soạn thảo tài liệu kỹ thuật chuyên nghiệp mới của JetBrains](https://www.jetbrains.com/writerside/)

Hãng phần mềm JetBrains giới thiệu công cụ máy tính chuyên dụng hỗ trợ các nhà phát triển viết tài liệu kỹ thuật, hướng dẫn sử dụng cho dự án, hỗ trợ định dạng Markdown và XML, tích hợp khả năng xem trước thời gian thực và đồng bộ Git.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102405.webp)

4、[EuBackend: Nền tảng hỗ trợ phát triển web nhanh sử dụng Java SpringBoot + Vue](https://gitee.com/zhaoeryu/eu-backend)

Một bộ khung mã nguồn mở cung cấp sẵn cấu trúc thư mục, hệ thống phân quyền và các module quản trị cơ bản được xây dựng trên nền tảng Java SpringBoot kết hợp Vue ở Front-end giúp lập trình viên nhanh chóng triển khai dự án web. (Đóng góp của [@zhaoeryu](https://github.com/ruanyf/weekly/issues/3579))

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102302.webp)

5、[EmuDeck: Tiện ích cài đặt nhanh trình giả lập game cho hệ máy Steam Deck](https://www.emudeck.com/)

Một công cụ hữu ích dành cho người dùng máy chơi game cầm tay Steam Deck: hỗ trợ tự động tải về, cài đặt và cấu hình tối ưu toàn bộ các trình giả lập của các hệ máy game cổ điển (như PS, Nintendo) để chơi trực tiếp trên máy.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050102.webp)

6、[Secretive: Ứng dụng hỗ trợ quản lý khóa SSH an toàn bằng Touch ID trên macOS](https://github.com/maxgoedjen/secretive)

Phần mềm mã nguồn mở dành cho người dùng máy tính Mac, cho phép lưu trữ bảo mật các khóa SSH cá nhân bên trong chip bảo mật Secure Enclave của máy, yêu cầu người dùng xác thực bằng Touch ID hoặc Apple Watch mỗi khi gọi khóa để kết nối.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031408.webp)

7、[tRPC: Bộ khung giao tiếp RPC hiệu năng cao mã nguồn mở của Tencent](https://github.com/trpc-group/trpc)

Hệ thống khung sườn giao tiếp RPC nội bộ của tập đoàn Tencent chính thức được mở nguồn cho cộng đồng. Dự án hỗ trợ cơ chế giao tiếp đa ngôn ngữ, hiệu năng cao tương tự gRPC, hiện đã công bố trước phiên bản hỗ trợ cho Go và C++. (Đóng góp của [@ryantang1991](https://github.com/ruanyf/weekly/issues/3584))

8、[Atuin: Công cụ hỗ trợ lưu trữ và tra cứu lịch sử dòng lệnh Shell bằng SQLite](https://atuin.sh/)

Một tiện ích dòng lệnh giúp thay thế trình quản lý lịch sử mặc định của Shell: tự động ghi nhận toàn bộ lịch sử gõ lệnh đi kèm thời gian thực thi vào một tệp cơ sở dữ liệu SQLite cục bộ, hỗ trợ tìm kiếm nhanh và đồng bộ hóa mã hóa giữa các máy tính.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050609.webp)

9、[BackgroundRemover: Công cụ dòng lệnh hỗ trợ tách nền ảnh và video tự động](https://github.com/nadermx/backgroundremover)

Một tiện ích dòng lệnh chạy trên máy tính, sử dụng mô hình trí tuệ nhân tạo để tự động nhận diện và tách bỏ phông nền của hình ảnh hoặc tệp video một cách nhanh chóng, rất thích hợp để nhúng vào các tập lệnh xử lý tự động hàng loạt.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050611.webp)

10\. [pear-rec: Ứng dụng mã nguồn mở hỗ trợ chụp ảnh màn hình và ghi âm trên máy tính](https://github.com/027xiguapi/pear-rec/)

Phần mềm viết bằng Electron hỗ trợ đầy đủ các tính năng văn phòng cơ bản như chụp ảnh màn hình, quay video màn hình máy tính, thu âm giọng nói và trích xuất ảnh GIF chuyển động nhanh chóng. (Đóng góp của [@027xiguapi](https://github.com/ruanyf/weekly/issues/3587))

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102607.webp)

11\. [TwitterShots: Dịch vụ web hỗ trợ tạo ảnh chụp bài đăng Twitter đẹp mắt](https://twittershots.com/)

Một công cụ trực tuyến tiện lợi giúp người dùng nhanh chóng tạo ra các bức ảnh chụp màn hình bài đăng trên mạng xã hội Twitter/X với thiết kế đổ bóng, lồng khung hình nền nghệ thuật để chia sẻ lên các nền tảng khác. (Đóng góp của [@0xinhua](https://github.com/ruanyf/weekly/issues/3588))

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102608.webp)

## 资源

1\. [HTTP Headers Hacktricks: Cẩm nang tổng hợp các trường HTTP Header đặc thù](https://book.hacktricks.xyz/network-services-pentesting/pentesting-web/special-http-headers)

Trang tài liệu chuyên sâu dành cho các kỹ sư kiểm thử bảo mật (Pentester), tổng hợp thông tin và cơ chế hoạt động của các trường HTTP Header đặc biệt, ít gặp nhưng thường được khai thác để kiểm tra lỗi bảo mật web.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023073101.webp)

2、[Roblox Ryanair: Trải nghiệm không gian ảo mô phỏng hãng hàng không Ryanair](https://www.robloxryanair.com/)

Một dự án sáng tạo trên nền tảng Roblox tái hiện chi tiết từ thiết kế quầy làm thủ tục, máy bay cho tới quy trình vận hành bay của hãng hàng không giá rẻ Ryanair ngoài thực tế để người chơi trải nghiệm trong thế giới ảo.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102401.webp)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102402.webp)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102403.webp)

3\. [PyFlo: Giáo trình tự học lập trình Python trực quan bằng sơ đồ](https://pyflo.net/)

Một trang web cung cấp khóa học lập trình Python cơ bản miễn phí dành cho người mới bắt đầu, điểm độc đáo là toàn bộ lộ trình bài học được thiết kế trực quan dưới dạng một sơ đồ cây tiến trình, giúp người học dễ dàng theo dõi lộ trình.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023073102.webp)

4\. [BASIC Computer Games: Kho mã nguồn tái phát triển các tựa game BASIC cổ điển](https://github.com/coding-horror/basic-computer-games)

Dự án cộng đồng chuyên thực hiện viết lại mã nguồn của các trò chơi điện tử viết bằng ngôn ngữ BASIC cổ điển từ thế kỷ trước sang các ngôn ngữ lập trình hiện đại (như Python, Go, Rust, JavaScript), một nguồn bài tập thực hành lập trình rất thú vị.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080106.webp)

5\. [CSS Loaders: Kho lưu trữ các hiệu ứng chuyển động tải trang bằng CSS](https://css-loaders.com/)

Trang web tổng hợp hàng trăm mẫu thiết kế hiệu ứng chuyển động chờ tải trang (Loading animation) được xây dựng hoàn toàn bằng mã nguồn CSS tối giản, cho phép người dùng click để sao chép nhanh mã nguồn về dự án.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090701.webp)

## 图片

1\. **Khám phá hang động khảo cổ dưới nước Cosquer độc đáo tại Pháp**

Hang động Cosquer là một di tích khảo cổ nổi tiếng nằm tại vùng biển Marseille, miền nam nước Pháp. Từ hàng chục ngàn năm trước, đây từng là nơi sinh sống của người tiền sử. Trải qua các thời kỳ địa chất biến đổi, mực nước biển dâng cao đã nhấn chìm toàn bộ lối vào của hang động:

Hiện nay, lối vào hang nằm sâu dưới mặt nước biển tới 37 mét:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050603.webp)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050607.webp)

Vào năm 1985, một thợ lặn chuyên nghiệp đã tình cờ phát hiện ra cửa hang và thực hiện lặn thám hiểm sâu vào bên trong:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050608.webp)

Khi di chuyển dọc theo đường hầm dốc hướng lên trên, anh phát hiện ra phần lòng hang phía trong cùng nằm phía trên mực nước tạo thành một hồ nước ngầm lớn có thể lên bờ đi lại được. Đến năm 1991, các thợ lặn đã phát hiện các hình in bàn tay trên vách đá, giúp cơ quan khảo cổ nhận định đây là di tích lịch sử vô giá lưu giữ hàng loạt bức vẽ động vật độc đáo của người tiền sử trên vách hang:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050604.webp)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050605.webp)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050606.webp)

## ✍️ Bài đọc thêm

### Chia sẻ đầy cảm hứng của nữ tác giả đoạt giải Hugo năm 2023: "Luôn có lối thoát ở cuối chặng đường tối tăm"

Tại Hội nghị Khoa học Viễn tưởng Thế giới năm 2023 diễn ra tại Thành Đô vừa qua, ban tổ chức đã công bố danh sách các tác phẩm đoạt giải thưởng Hugo danh giá. Tác phẩm tiểu thuyết kỳ ảo *“Nettle & Bone”* của nữ nhà văn Mỹ Ursula Vernon đã xuất sắc giành giải thưởng “Tiểu thuyết xuất sắc nhất”.

Dưới đây là bài chia sẻ đầy hài hước và ý nghĩa của bà về khoảnh khắc nhận giải:

Múi giờ của Thành Đô đi trước múi giờ của chúng tôi tại Mỹ tới 12 tiếng. Vì vậy, để theo dõi trực tiếp lễ trao giải, chúng tôi đã phải thức dậy từ lúc tảng sáng để thực hiện kết nối video qua Zoom.

Cả nhóm chúng tôi đều mặc đồ ngủ ở nhà, vừa nhâm nhi đồ uống vừa chăm chú nhìn vào màn hình. Do tín hiệu đường truyền video chập chờn liên tục bị ngắt quãng, chúng tôi đành phải tìm trò khác để tự giải trí. Đó là lý do tại sao đúng vào khoảnh khắc ban tổ chức gọi tên tôi đoạt giải, tôi thực chất đang cầm một cuốn tài liệu viết tay thời Trung Cổ mô tả cách dùng phân gà trống để chữa ngộ độc để đọc to cho mọi người nghe.

Đại diện nhà xuất bản tại hiện trường đã thay mặt tôi lên sân khấu đọc bài phát biểu cảm ơn đã chuẩn bị từ trước:

*“Xin chào tất cả mọi người tại Thành Đô! Tôi vô cùng tiếc nuối khi không thể có mặt trực tiếp tại hội trường để nhận giải thưởng danh giá này. Tiếc nuối không chỉ vì giải thưởng Hugo, mà còn vì Trung Quốc sở hữu nền ẩm thực tuyệt vời nhất trong số các quốc gia tôi từng đặt chân tới. Tôi từng được thưởng thức món lẩu xiên que (串串) ngon đến mức có thể khiến những người nghiêm túc nhất cũng phải rơi nước mắt vì hạnh phúc.*

*Tôi hoàn toàn không nghĩ mình sẽ đoạt giải thưởng lớn này, đây là niềm vinh dự lớn trong cuộc đời tôi khi tôi mới chỉ 46 tuổi! Xin gửi lời cảm ơn sâu sắc tới toàn bộ độc giả đã yêu thích và bình chọn cho tác phẩm.*

*Không có cuốn sách nào được hoàn thành chỉ bởi một cá nhân. Xin cảm ơn biên tập viên, nhà xuất bản, người đại diện Helen và Kevin – chồng tôi, người luôn bảo đảm tôi có những bữa ăn ngon và quần áo sạch để tập trung viết lách.*

*Tôi có thể nói nhiều điều nghiêm túc và vĩ đại hơn trong khoảnh khắc này, nhưng có lẽ nhiều diễn giả khác đã diễn đạt điều đó hay hơn tôi rồi. Vì vậy, tôi muốn chia sẻ cùng các bạn một phát hiện khoa học vừa thú vị vừa có phần kỳ lạ của giới sinh học để làm bài học cảm hứng:*

*Vào năm 2020, các nhà khoa học Nhật Bản đã công bố một nghiên cứu về tập tính sinh tồn kỳ lạ của một loài bọ nước. Loài bọ này là món mồi yêu thích của loài ếch và thường xuyên bị ếch nuốt chửng nguyên con vào bụng. Thông thường, một khi đã trôi vào dạ dày ếch, số phận của con mồi coi như đã định đoạt: bạn sẽ nhanh chóng bị dịch vị tiêu hóa hoàn toàn.*

*Nhưng loài bọ nước đặc biệt này lại không chịu khuất phục. Nó đã chủ động bò dọc theo đường tiêu hóa của ếch và chui ra ngoài hoàn toàn khỏe mạnh qua đường hậu môn của ếch.*

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102410.webp)

*Đây hoàn toàn không phải là câu chuyện do tôi tự nghĩ ra, các bạn có thể tìm đọc bài nghiên cứu khoa học chính thức này. Thống kê chỉ ra có tới 19 trên tổng số 20 chú bọ nước đã thực hiện thoát xác thành công khỏi bụng ếch mà hoàn toàn không gặp bất kỳ tổn thương nào. Quy trình này thường tiêu tốn khoảng một giờ đồng hồ, nhưng có một chú bọ đặc biệt đã bứt tốc thoát ra ngoài chỉ trong vòng 5 phút, tôi tin rằng chú ếch lúc đó chắc hẳn đã cảm thấy vô cùng nhẹ nhõm.*

*Ý nghĩa rút ra từ câu chuyện sinh tồn này là: dù hoàn cảnh xung quanh bạn có tăm tối đến mức nào đi chăng nữa, luôn có một con đường sống dành cho bạn nếu bạn không ngừng nỗ lực hành động. Luôn có ánh sáng đón chờ bạn ở cuối con đường tiêu hóa của chú ếch.”*

## Lịch sử tuần này

- 2022年（第 227 期）：[Văn hóa doanh nghiệp: Tìm hiểu quy trình đào tạo và hòa nhập văn hóa dành cho nhân viên mới tại Facebook](http://www.ruanyifeng.com/blog/2022/10/weekly-issue-227.html)
- 2021年（第 177 期）：[Thiết bị di động: Thảo luận về những vai trò và ứng dụng thực tế phù hợp nhất của máy tính bảng iPad](http://www.ruanyifeng.com/blog/2021/09/weekly-issue-177.html)
- 2020年（第 127 期）：[Xu hướng công nghệ: Dự báo tương lai khi lập trình không code phổ cập giúp ai cũng có thể tạo phần mềm](http://www.ruanyifeng.com/blog/2020/09/weekly-issue-127.html)
- 2019年（第 77 期）：[Giải trí: Giới thiệu và phân tích ý tưởng công nghệ AR độc đáo trong bộ phim truyền hình Hàn Quốc “Ký ức Alhambra”](http://www.ruanyifeng.com/blog/2019/10/weekly-issue-77.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
