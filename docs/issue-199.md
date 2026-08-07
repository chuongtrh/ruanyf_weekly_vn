# 科技爱好者周刊（第 199 期）：俄罗斯的 HTTPS 证书问题

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2234) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031406.webp)

Một trường tiểu học tại Chiết Giang đã đưa vào sử dụng loại bàn ghế học sinh thông minh có thể ngả phẳng thành giường ngủ trưa nhỏ, giải quyết triệt để bài toán ngủ trưa tại lớp của học sinh. Các lập trình viên thường xuyên làm việc muộn cũng rất cần một chiếc ghế ngả phẳng tiện lợi như thế này tại văn phòng. (Nguồn: [WeChat](https://mp.weixin.qq.com/s/d8GSJYSnUyMn6aXzQwUU_Q))

## 主带话题：Sự cố chứng chỉ HTTPS tại Nga

Tuần trước, cộng đồng công nghệ quốc tế [phát hiện](https://twitter.com/Scott_Helme/status/1502204103132393472) một tổ chức phát hành chứng chỉ HTTPS (CA) của phương Tây đã từ chối gia hạn, thậm chí chủ động thu hồi các chứng chỉ bảo mật HTTPS đang hoạt động của các trang web và tên miền thuộc Nga:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031105.webp)

Mặc dù chính phủ Mỹ chưa ban hành bất kỳ lệnh cấm chính thức nào đối với dịch vụ kỹ thuật này, nhưng nhà phát hành chứng chỉ đã tự phát thực hiện hành vi trừng phạt. Nếu toàn bộ các tổ chức CA phương Tây đồng loạt làm theo, các trang web của Nga sẽ hoàn toàn mất khả năng mã hóa kết nối bảo mật HTTPS, làm tê liệt hệ thống thanh toán trực tuyến và ảnh hưởng nghiêm trọng tới các dịch vụ số thiết yếu của người dân.

Để phòng ngừa rủi ro này, chính phủ Nga đã khẩn trương thiết lập một trung tâm phát hành chứng chỉ bảo mật quốc gia riêng. Các doanh nghiệp và cá nhân trong nước có thể đăng ký chứng chỉ do nhà nước cấp trực tiếp tại trang web [gosuslugi.ru/tls](https://www.gosuslugi.ru/tls):

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031106.webp)

Tuy nhiên, điểm mấu chốt là chứng chỉ số tự phát hành của Nga không nằm trong danh sách tổ chức chứng chỉ tin cậy (Root CA) mặc định của các hệ điều hành phổ biến (Windows, macOS, iOS, Android) và các trình duyệt lớn (Chrome, Safari, Firefox). Khi người dùng truy cập, trình duyệt sẽ lập tức hiển thị cảnh báo đỏ nguy hiểm, cảnh báo kết nối không an toàn:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031107.webp)

Trong bối cảnh căng thẳng chính trị hiện nay, việc thuyết phục các hãng công nghệ lớn của phương Tây cập nhật tin cậy chứng chỉ của Nga vào hệ thống là điều không thể. Để xử lý, Nga khuyến cáo người dân chuyển sang sử dụng trình duyệt nội địa **Yandex Browser** (đã tích hợp sẵn Root CA của Nga) hoặc hướng dẫn người dùng tự tải và cài đặt thủ công chứng chỉ của chính phủ vào hệ thống máy tính cá nhân.

**Sự kiện này rất có thể sẽ dẫn tới việc thế giới Internet bị phân tách thành hai nửa chứng chỉ số độc lập.** Xu hướng này thậm chí đang lan rộng sang các khía cạnh khác như tạm dừng định tuyến mạng quốc tế, ngừng cung cấp đăng ký tên miền quốc tế và chặn phân giải hệ thống DNS đối với Nga. Nếu đi đến bước này, mạng Internet của Nga sẽ hoàn toàn bị cô lập thành một ốc đảo tách biệt với phần còn lại của thế giới.

Điều này gợi nhớ đến một câu nói nổi tiếng trong bài cổ văn 《Phong Phú》:

> *"Phu phong giả, thiên địa chi khí, phổ sướng nhi chí, bất trạch quý tiện cao hạ nhi gia yên."*
> 
> (Dịch nghĩa: Gió là linh khí của đất trời, thổi đi khắp nơi, không phân biệt sang hèn cao thấp).

Tôi luôn tin rằng Internet là một cơ sở hạ tầng kỹ thuật trung lập, giống như ngọn gió mát lành của tự nhiên thổi đồng đều tới tất cả mọi người, không phân biệt giàu nghèo, tốt xấu, biên giới quốc gia, và bất kỳ ai cũng có quyền sử dụng nó.

**Việc vũ khí hóa hạ tầng Internet bằng cách đơn phương thu hồi chứng chỉ số hay ngắt kết nối mạng quốc gia sẽ triệt tiêu hoàn toàn tính trung lập của Internet.** Một tiền lệ nguy hiểm được thiết lập sẽ biến Internet từ một không gian mở, tự do chia sẻ toàn cầu thành các khu vực biên giới phòng ngự nghiêm ngặt với hệ thống chứng chỉ, DNS và cổng mạng riêng của từng nước. Giấc mơ ban đầu của những người sáng lập Internet về một thế giới kết nối phẳng và đoàn kết nhân loại sẽ chính thức tan vỡ. Và những người phải gánh chịu thiệt hại lớn nhất chính là những người dân thường và các doanh nghiệp nhỏ.

## 计算机考研基础课训练营

Tháng này, các thông tin liên quan đến kỳ thi tuyển sinh thạc sĩ nhận được sự quan tâm lớn do điểm thi quốc gia vừa được công bố và các trường đang chuẩn bị xét tuyển lại.

Với số lượng thí sinh đăng ký dự thi tăng vọt hàng năm kéo theo điểm chuẩn nâng cao, các thí sinh có mục tiêu thi thạc sĩ năm tới đã bắt đầu ôn tập từ bây giờ để chuẩn bị cho đợt đăng ký vào tháng 9.

Khóa học giới thiệu tuần này tập trung vào cẩm nang ôn tập các môn thi đại cương: **《Computer Master Entrance Exam Foundation Bootcamp》**:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031712.webp)

Lịch học kéo dài 4 buổi tối liên tục từ thứ Hai đến thứ Năm tuần tới (19:20 - 21:30):
- **Buổi 1 - Bản đồ ôn thi:** Cựu học viên Thanh Hoa hướng dẫn phân tích giá trị của học vị thạc sĩ CNTT, đánh giá độ khó của đề thi và triển khai lộ trình ôn tập tối ưu.
- **Buổi 2 - Môn chuyên ngành:** Kỹ sư công nghệ (cựu chuyên gia Alibaba) hướng dẫn phương pháp làm chủ bài thi chuyên ngành 408 từ con số 0, vượt qua các dạng bài tập giải thuật hóc búa.
- **Buổi 3 - Môn Chính trị:** Hệ thống hóa các kiến thức trọng tâm môn Chính trị và chia sẻ mẹo làm bài trắc nghiệm nhanh.
- **Buổi 4 - Môn Tiếng Anh:** Phân tích quy luật ra đề đọc hiểu tiếng Anh thi thạc sĩ, đúc kết các phương pháp làm bài đạt điểm cao.

Đội ngũ giảng viên tốt nghiệp từ các trường đại học hàng đầu 985/211 trực tiếp hướng dẫn phương pháp ghi nhớ khoa học giúp học viên nhanh chóng làm chủ kiến thức. Hệ thống AI của ban tổ chức cũng hỗ trợ chấm điểm thử dựa trên dữ liệu thi các năm để tư vấn chọn trường thi có tỷ lệ đỗ cao nhất:

Khóa học phù hợp cho 3 nhóm đối tượng:
- Sinh viên chuẩn bị tốt nghiệp muốn thi thạc sĩ trái ngành sang CNTT để tìm cơ hội việc làm tốt hơn.
- Người đã đi làm muốn nâng cao học vị để mở rộng cơ hội thăng tiến sự nghiệp.
- Người muốn chuyển hướng nghề nghiệp tìm kiếm sự ổn định trong các cơ quan nhà nước.

Khóa học được thiết kế dễ tiếp cận cho cả học viên chưa từng học lập trình, toàn bộ mã nguồn bài tập sẽ được chia sẻ miễn phí để học viên tự luyện tập nâng cao kỹ năng thực chiến.

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031713.webp)

Độc giả bản tin đăng ký tham gia khóa học sẽ được nhận mức học phí ưu đãi chỉ **1 NDT**. Bạn đọc quan tâm có thể quét mã QR phía trên để đăng ký và kết nối với trợ lý nhận bộ tài liệu đề thi thử các năm.

## 科技动态

1、[Nintendo Switch phủ chất cực đắng lên thẻ game ngăn trẻ em nuốt](https://www.polygon.com/2017/3/1/14784140/nintendo-switch-cartridges-taste-awful-psa)

Trào lưu các streamer thử nghiệm liếm thẻ game Nintendo Switch và lập tức phải nhổ ra vì vị quá đắng đã thu hút sự chú ý lớn của cộng đồng mạng:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012603.webp)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020103.webp)

Đại diện Nintendo xác nhận hãng đã chủ động phủ một lớp chất tạo đắng an toàn và không độc hại mang tên **Denatonium Benzoate** lên vỏ nhựa ngoài của thẻ game. Đây là hợp chất đắng nhất mà con người từng biết đến, được phủ lên thẻ game kích thước nhỏ để ngăn chặn trẻ em vô tình ngậm hoặc nuốt phải thẻ game gây nguy hiểm.

2、[Nghiên cứu y sinh đạt bước tiến mới: Thực hiện thành công sinh sản đơn tính ở chuột](https://news.bioon.com/article/6796589.html)

Quy luật sinh sản của động vật có vú bậc cao luôn yêu cầu sự kết hợp giữa tinh trùng và trứng để thụ tinh. Nhóm nghiên cứu thuộc Đại học Y khoa Giao thông Thượng Hải vừa công bố đã phá vỡ giới hạn này:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031404.webp)

Bằng cách sử dụng công cụ chỉnh sửa gen chuẩn xác để tác động trực tiếp vào các gen kiểm soát sự phát triển của trứng chưa thụ tinh (mô phỏng lại trạng thái gen của tinh trùng sau khi thụ tinh), nhóm nghiên cứu đã kích thích trứng tự phân chia phát triển thành phôi và hạ sinh thành công những chú chuột con khỏe mạnh, có khả năng sinh sản bình thường khi trưởng thành.

3、[Intel đặt mua máy quang khắc EUV hiện đại nhất thế giới của ASML với giá kỷ lục](https://www.eet-china.com/news/202201210103.html)

Tập đoàn ASML (Hà Lan) - nhà sản xuất độc quyền máy quang khắc tia cực tím cực đoan (EUV) phục vụ sản xuất chip bán dẫn cao cấp - công bố đã nhận đơn đặt hàng phiên bản máy quang khắc High-NA EUV thế hệ mới nhất từ Intel:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012104.webp)

Mỗi máy quang khắc thế hệ mới có giá bán lên tới 340 triệu USD (khoảng 2,2 tỷ NDT), dự kiến bắt đầu bàn giao từ năm 2024. Một nhà máy sản xuất chip bán dẫn hiện đại thường cần trang bị từ 9 đến 18 thiết bị quang khắc EUV, đưa tổng vốn đầu tư thiết bị lên tới 10 đến 20 tỷ USD:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012105.webp)

Hiện tại thế giới chỉ có 3 khách hàng lớn đủ khả năng tài chính đặt mua dòng máy này là TSMC, Samsung và Intel. Do năng lực sản xuất của ASML có giới hạn nên các hãng bắt buộc phải xếp hàng đặt trước nhiều năm để nhận máy.

4、[Microsoft Windows 11 loại bỏ ký tự ổ đĩa A: mặc định khi cài driver](https://www.windowslatest.com/2022/01/10/windows-11s-device-manager-finally-uses-os-path-instead-of-a-floppy-disks/)

Lịch sử hệ điều hành Windows từ trước đến nay khi người dùng tải và cài đặt driver thiết bị thủ công trong Device Manager luôn gợi ý đường dẫn bắt đầu từ ổ đĩa A:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012009.webp)

Ký tự ổ A: và B: vốn đại diện cho ổ đĩa mềm (floppy disk) từ những thập niên trước nay đã hoàn toàn tuyệt chủng. Bắt đầu từ bản cập nhật Windows 11 Build 22000, Microsoft đã chính thức thay đổi cài đặt này để gợi ý đường dẫn bắt đầu trực tiếp từ phân vùng ổ C: chứa hệ điều hành:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012010.webp)

Tuy nhiên, mã nguồn cốt lõi của Windows 11 vẫn được thiết kế tương thích ngược để hỗ trợ nhận dạng ổ đĩa mềm nếu máy tính của người dùng có trang bị phần cứng cổ điển này:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012011.webp)

5、[Thượng viện Mỹ thông qua dự luật áp dụng vĩnh viễn giờ mùa hè](https://www.reuters.com/world/us/us-senate-approves-bill-that-would-make-daylight-savings-time-permanent-2023-2022-03-15/)

Thượng viện Mỹ vừa bỏ phiếu thông qua dự luật chuyển dịch giờ quốc gia sang áp dụng vĩnh viễn giờ mùa hè (Daylight Saving Time - DST) bắt đầu từ năm 2023:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031601.webp)

Theo quy chế cũ, mỗi năm người dân Mỹ phải chỉnh đồng hồ nhanh lên 1 tiếng vào tháng 3 và chỉnh chậm lại 1 tiếng vào tháng 11 gây nhiều phiền toái. Nếu dự luật được Hạ viện thông qua và Tổng thống ký ban hành, đồng hồ tại Mỹ sẽ được cố định nhanh hơn 1 tiếng quanh năm. Những người ủng hộ chỉ ra việc này giúp kéo dài thời gian có ánh sáng ban ngày vào buổi tối mùa đông muộn hơn, giúp tiết kiệm năng lượng chiếu sáng và thúc đẩy các hoạt động thương mại ngoài trời.

## 文章

1、[Tại sao sản lượng phát điện của Trung Quốc vượt xa Mỹ nhưng GDP quy đổi vẫn thấp hơn?](https://www.sohu.com/a/477247226_100110525)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030504.webp)

Thông thường chỉ số sản lượng điện năng tiêu thụ tỷ lệ thuận với GDP quốc gia. Bài viết phân tích cấu trúc kinh tế của hai nước: Trung Quốc tập trung mạnh vào sản xuất công nghiệp nặng tiêu thụ lượng điện khổng lồ nhưng biên lợi nhuận thấp, trong khi nền kinh tế Mỹ tập trung vào mảng dịch vụ tài chính, công nghệ và sở hữu trí tuệ tạo ra giá trị thặng dư GDP cao nhưng tiêu tốn ít năng lượng hơn.

2、[Trải nghiệm thực tế của nạn nhân bị lừa đảo qua trang web giả mạo](https://mp.weixin.qq.com/s/OrzpD-bVkUpL2mkFqqOCPg)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022030807.webp)

Tác giả chia sẻ câu chuyện cảnh giác khi vô tình điền mã xác thực OTP ngân hàng vào một trang web câu cá (phishing), dẫn tới tài khoản bị kẻ gian liên kết dịch vụ thanh toán rút sạch tiền, và chia sẻ các bước làm việc với ngân hàng và Apple Pay để khiếu nại thu hồi lại được một phần tài sản bị mất.

3、[Phóng sự về thiết bị thông tin liên lạc của lực lượng quân sự trên thực địa](https://mp.weixin.qq.com/s/q8NiQ2MJyRLEOhnX5lAk2g)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031203.webp)

Ghi nhận thực tế một số đơn vị quân sự ngoài chiến trường sử dụng các dòng bộ đàm mô phỏng analog dân dụng giá rẻ mua từ Taobao thay vì hệ thống thông tin mã hóa chuyên dụng. Thiết kế truyền sóng analog không bảo mật trên tần số dân dụng khiến các cuộc trao đổi thông tin dễ dàng bị các無線 điện nghiệp dư trong khu vực bắt sóng và nghe lén.

4、[4 tính năng và cú pháp nên tránh sử dụng trong TypeScript](https://www.executeprogram.com/blog/typescript-features-to-avoid)（Tiếng Anh）

Bài viết chuyên sâu chỉ ra 4 lỗi thiết kế cú pháp thường gặp của lập trình viên TypeScript (như sử dụng enum hay thuộc tính namespace) dễ gây lỗi biên dịch hoặc làm giảm hiệu năng tối ưu hóa của compiler và đề xuất giải pháp thay thế sạch hơn.

5、[Kế hoạch viết lại bộ trình biên dịch TypeScript Compiler bằng ngôn ngữ Rust](https://zackoverflow.dev/writing/tyty)（Tiếng Anh）

Một lập trình viên công bố dự án phát triển trình biên dịch TypeScript phi chính thức viết hoàn toàn bằng Rust nhằm thay thế cho compiler chính thức `tsc` hiện tại (viết bằng JavaScript) vốn có tốc độ biên dịch khá chậm khi chạy các dự án quy mô lớn.

6、[Hướng dẫn bật tính năng phát tiếng ồn trắng hỗ trợ tập trung trên iOS 15](https://support.apple.com/zh-cn/guide/iphone/iphb2cfa052c/ios)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011820.webp)

Apple đã bổ sung tính năng Background Sounds trực tiếp trong phần Cài đặt của iOS 15. Tiện ích hỗ trợ phát các dải âm thanh tự nhiên như tiếng mưa rơi, tiếng sóng biển hay tiếng suối chảy lặp liên tục chạy ngầm để giúp người dùng thư giãn đầu óc khi làm việc.

7、[Hướng dẫn thiết lập interceptor gói tin mitmproxy trên thiết bị iOS 15](https://www.trickster.dev/post/setting-up-mitmproxy-with-ios15/)（Tiếng Anh）

Bài viết hướng dẫn chi tiết các bước cài đặt chứng chỉ bảo mật SSL và cấu hình proxy mạng trên thiết bị iOS 15 để sử dụng công cụ mitmproxy theo dõi các yêu cầu gọi API của ứng dụng di động. Xem thêm [hướng dẫn cho Android](https://www.trickster.dev/post/setting-up-mitmproxy-with-android/).

8、[Sử dụng biểu thức chính quy Regex để giải nhanh ô chữ đoán từ Wordle](https://dov.is/notebooks/solving-wordle-regex.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012601.webp)

Một cách tiếp cận thú vị để đoán từ trong game Wordle: tác giả hướng dẫn cách xây dựng các chuỗi regex so khớp ký tự linh hoạt để lọc nhanh các từ tiếng Anh thỏa mãn điều kiện từ bộ từ điển có sẵn chỉ qua vài bước loại trừ.

9、[Chỉ ra lỗi logic xử lý đầu ra dòng lệnh trong ví dụ Hello World của các ngôn ngữ](https://blog.sunfishcode.online/bugs-in-hello-world/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031005.webp)

Tác giả phân tích sâu về cơ chế gọi hàm hệ thống (system call) trong nhân Linux của chương trình Hello World kinh điển. Ông chỉ ra hầu hết trình biên dịch của các ngôn ngữ (kể cả C) đều bỏ qua việc kiểm tra mã lỗi trả về của luồng đầu ra stdout khi bộ nhớ đệm bị đầy, dẫn tới việc chương trình vẫn báo chạy thành công dù thông điệp chưa được in ra màn hình.

## 工具

1、[jless: Trình xem và tương tác file JSON trên giao diện Command Line](https://pauljuliusmartinez.github.io/)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021203.webp)

Công cụ dòng lệnh hữu ích hỗ trợ hiển thị dữ liệu JSON có cấu trúc màu sắc, cho phép người dùng sử dụng phím tắt để thu gọn hoặc mở rộng từng trường dữ liệu con trực quan.

2、[Terrain2STL: Sinh file mô hình 3D địa hình từ bản đồ vệ tinh](https://jthatch.com/Terrain2STL/)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021304.webp)

Trang web hỗ trợ người dùng quét chọn một tọa độ địa lý bất kỳ trên bản đồ Trái Đất để tự động dựng lưới độ cao và xuất ra file thiết kế định dạng STL phục vụ việc in 3D sa bàn địa hình thực tế.

3、[SikuliX: Bộ công cụ tự động hóa thao tác màn hình bằng nhận diện hình ảnh](https://github.com/RaiMan/SikuliX1)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021305.webp)

Tiện ích tự động hóa hỗ trợ viết kịch bản click chuột, gõ phím dựa trên việc nhận diện ảnh chụp màn hình bằng thư viện OpenCV. Ví dụ khi phát hiện nút bấm chuyển sang màu xanh lá, phần mềm sẽ tự động kích hoạt chuỗi thao tác định nghĩa trước.

4、[jDeploy: Đóng gói và phát hành ứng dụng Java lên NPM dưới dạng file cài đặt](https://www.jdeploy.com/)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021503.webp)

Công cụ hỗ trợ các nhà phát triển Java đóng gói nhanh file Jar thành các gói cài đặt chạy trực tiếp trên Windows, macOS, Linux và đẩy lên kho quản lý gói NPM để người dùng dễ dàng cài đặt nâng cấp qua dòng lệnh.

5、[Ronja: Dự án phần cứng truyền tải mạng LAN bằng ánh sáng khả kiến](http://ronja.twibright.com/about.php)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021406.webp)

Dự án thiết kế thiết bị truyền dẫn mạng không dây tầm ngắn bằng luồng ánh sáng LED hội tụ của máy phát quang học:

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021407.webp)

Thiết bị hỗ trợ kết nối hai mạng nội bộ LAN ở cự ly tối đa 1.4 km với tốc độ truyền tải 10Mbps ổn định không bị ảnh hưởng bởi sóng vô tuyến xung quanh.

6、[AirPods Jump Rope: Ứng dụng đếm số lần nhảy dây qua tai nghe AirPods](https://apps.apple.com/cn/app/id1485959492)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031702.webp)

Ứng dụng tận dụng cảm biến gia tốc chuyển động 3 trục tích hợp trên các thế hệ tai nghe AirPods mới để theo dõi chuyển động nẩy của cơ thể, hỗ trợ đếm số lần nhảy dây chính xác mà không cần đeo vòng tay thông minh. (Đóng góp của [@haozes](https://github.com/ruanyf/weekly/issues/2263))

7、[Regex-Vis: Trình biên soạn và vẽ sơ đồ biểu thức chính quy trực quan](https://github.com/Bowen7/regex-vis)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031703.webp)

Dự án nguồn mở hỗ trợ lập trình viên nhập biểu thức regex để tự động vẽ sơ đồ logic cấu trúc so khớp ký tự, giúp dễ dàng kiểm tra và chỉnh sửa trực quan từng nút điều kiện trên giao diện web. (Đóng góp của [@Bowen7](https://github.com/ruanyf/weekly/issues/2271))

8、[Rubik's Cube 3D: Trò chơi Rubik nhiều tầng trực tuyến](https://github.com/pengfeiw/rubiks-cube)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031701.webp)

Dự án viết bằng thư viện đồ họa 3D Three.js cho phép người chơi giải Rubik trực tiếp trên trình duyệt, hỗ trợ tùy chỉnh số lượng ô của khối Rubik từ 3x3 đến các bậc cao hơn. Bạn có thể chơi thử [bản Demo](https://pengfeiw.github.io/rubiks-cube/). (Đóng góp của [@pengfeiw](https://github.com/ruanyf/weekly/issues/2262))

9、[Process Hacker: Phần mềm giám sát tiến trình hệ thống Windows chuyên sâu](https://processhacker.sourceforge.io/)

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021505.webp)

Tiện ích thay thế Task Manager mặc định của Windows, cung cấp thông tin chi tiết về các tiến trình đang chạy, bộ nhớ RAM sử dụng và các kết nối mạng thời gian thực của từng ứng dụng.

10、[Watchtower: Tự động cập nhật phiên bản mới cho Docker container](https://containrrr.dev/watchtower/)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022010503.webp)

Công cụ chạy dưới dạng một Docker container chuyên giám sát các container khác đang hoạt động trên hệ thống. Khi phát hiện Docker Image trên Docker Hub hoặc registry riêng tư có phiên bản build mới, Watchtower sẽ tự động tải về, dừng container cũ và khởi chạy container mới với cấu hình tương đương.

## 资源

1、[CSS Selector Speedrun: Thử thách kỹ năng viết CSS Selector nhanh](https://css-speedrun.netlify.app/)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011802.webp)

Trang web trắc nghiệm trực tuyến kiểm tra năng lực viết biểu thức chọn thẻ CSS tối ưu để chọn đúng các thành phần UI yêu cầu kèm hệ thống tính giờ thi đấu thú vị.

2、[DI.FM: Trang phát thanh nhạc điện tử trực tuyến phân loại theo thể loại](https://www.di.fm/)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011809.webp)

Website tổng hợp hàng trăm kênh radio chuyên phát nhạc điện tử (ambient, techno, house) chất lượng cao hoàn toàn miễn phí.

3、[OpenInfraMap: Bản đồ số hóa cơ sở hạ tầng năng lượng toàn cầu](https://openinframap.org/)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011810.webp)

Bản đồ trực quan hóa dữ liệu vị trí địa lý của toàn bộ các nhà máy điện, trạm biến áp, đường dây truyền tải điện cao thế và tua-bin gió trên thế giới dựa trên cơ sở dữ liệu OpenStreetMap.

4、[CRDT Wiki: Tổng hợp tài liệu nghiên cứu giải thuật đồng bộ phân tán](https://wiki.nikitavoloboev.xyz/distributed-systems/crdt)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011817.webp)

Trang wiki tổng hợp các công trình nghiên cứu khoa học, thư viện mã nguồn và giải thuật đồng bộ dữ liệu thời gian thực CRDT áp dụng cho các ứng dụng viết tài liệu đồng thời.

5、[Deno Examples: Kho tài liệu ví dụ lập trình Deno thực tế](https://examples.deno.land/)

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031704.webp)

Cổng thông tin hướng dẫn chính thức từ dự án Deno chia sẻ các đoạn code mẫu thực hiện các tác vụ cơ bản (đọc ghi file, gọi mạng, mã hóa dữ liệu).

## 图片

1、[Chiêm ngưỡng nghệ thuật xây dựng mô hình "Nhà giấy" của Bryan Berg](https://www.cardstacker.com/)

Trong tiếng Anh, cụm từ "house of cards" (tòa nhà bằng quân bài) thường dùng để chỉ cấu trúc lỏng lẻo dễ đổ vỡ. Tuy nhiên, kỷ lục gia thế giới Bryan Berg đã nâng bộ môn này lên tầm nghệ thuật kiến trúc:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121102.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121103.webp)

Ông đã xây dựng mô hình tháp bằng quân bài cao nhất thế giới lên tới hơn 7 mét, sử dụng hết 1.700 bộ bài tây với tổng trọng lượng hơn 100 kg. Ông cũng là người dựng mô hình bài tây lớn nhất thế giới phác họa lại khách sạn Venetian Macau tại Trung Quốc từ 218.000 quân bài xếp chồng hoàn toàn tự nhiên không dùng keo dính trong 44 ngày:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121104.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121105.webp)

Một số hình ảnh ghi nhận quá trình làm việc tỉ mỉ đòi hỏi độ tập trung cực cao của tác giả:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121106.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121107.webp)

2、[Bộ sưu tập icon skeuomorphism độc đáo của hệ điều hành NeXTSTEP](http://galgot.free.fr/wordpress/?p=1380)

Năm 1985, sau khi rời khỏi Apple, Steve Jobs đã thành lập công ty máy tính NeXT và phát triển hệ điều hành riêng mang tên NeXTSTEP. Mặc dù không thành công về mặt thương mại, hệ điều hành này sau đó đã được Apple mua lại vào năm 1996 để làm nền tảng phát triển cho hệ điều hành macOS mới, đưa Steve Jobs trở lại Apple:

Bộ thiết kế icon của NeXTSTEP áp dụng phong cách mô phỏng vật thể thực tế (skeuomorphism) cực kỳ tỉ mỉ và sang trọng, trông không hề lỗi thời ngay cả ở thời điểm hiện tại:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121408.webp)

*(Giao diện màn hình chính của hệ điều hành NeXTSTEP)*

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121409.webp)

*(Biểu tượng File Manager)*

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121410.webp)

*(Biểu tượng Home Directory)*

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121411.webp)

*(Biểu tượng Folder)*

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121412.webp)

*(Biểu tượng Library)*

## Bài đọc thêm

### Định luật lặp lại của thông tin sai lệch: Tại sao tin giả vẫn luôn có người tin tưởng?

Một trong những lý do khiến các thông tin sai lệch hay tin đồn thất thiệt vẫn luôn có một lượng người tin tưởng lớn là vì mọi người thường xuyên nghe thấy người xung quanh bàn luận về chúng:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031714.webp)

Cách duy nhất để triệt tiêu một ý tưởng hay thông tin sai lệch là không ai nhắc tới nó nữa. Nếu một tin giả liên tục được lặp đi lặp lại trong cộng đồng, nó sẽ tự động được não bộ ghi nhớ và chấp nhận như một sự thật.

Do đó, việc bạn cố gắng chia sẻ bài viết để chỉ trích, phản bác tin giả vô tình lại chính là hành vi giúp tin giả được lặp lại nhiều lần hơn trên mạng xã hội, khiến nhiều người tiếp cận và ghi nhớ nó hơn.

Hiện tượng này được gọi là **Định luật lặp lại Cleary (Cleary’s Law of Recurrence)**: số lượng người tin vào một ý kiến tỷ lệ thuận với tần suất ý kiến đó được lặp lại trong năm qua, ngay cả khi ý kiến đó rõ ràng là phản khoa học.

Mỗi khi bạn lao vào tấn công một luận điểm sai lầm, bạn đang vô tình tiếp thêm năng lượng cho chính con quái vật mà bạn muốn tiêu diệt. Như một nhân viên Twitter từng nhận xét: *"Mỗi khi bạn chia sẻ hoặc trích dẫn lại một bài viết bạn ghét để phê phán, bạn đang trực tiếp giúp bài viết đó tăng tương tác."*

Giải pháp tối ưu là hãy tập trung quỹ thời gian hạn hẹp để lan tỏa và ủng hộ các ý tưởng tốt đẹp, thay vì tốn công sức đi vạch trần các tin đồn vô căn cứ. Hãy để tin giả tự biến mất bằng cách rơi vào quên lãng do không ai quan tâm. Như học giả Tyler Cowen từng khuyên: *"Hãy dành ít thời gian nhất có thể để bàn luận về những sai lầm của người khác."*

Hãy cùng nhau lan tỏa tri thức hữu ích và để các tin đồn thất thiệt chìm vào im lặng.

### Tại sao trình duyệt Vivaldi từ chối tích hợp tính năng tiền số

CEO của trình duyệt Vivaldi từng chia sẻ thẳng thắn về lý do sản phẩm của họ quyết định đứng ngoài làn sóng tích hợp tiền điện tử (cryptocurrency):

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022031715.webp)

Khi thiết kế trình duyệt, chúng tôi từng cân nhắc việc phát hành một đồng tiền mã hóa riêng hoặc tích hợp các công cụ ví điện tử vào trình duyệt để thu hút người dùng.

Tuy nhiên, chúng tôi nhận thấy việc này không khác gì hành vi khuyến khích người dùng phổ thông tham gia vào một trò chơi cá cược tài chính mạo hiểm, thậm chí dễ vấp phải các bẫy lừa đảo đa cấp. Đó là hành vi thiếu đạo đức kinh doanh.

Thay vì quảng cáo tiền số như một cơ hội làm giàu nhanh chóng, chúng tôi muốn người dùng giữ một thái độ thận trọng và hoài nghi cần thiết trước các bong bóng tài chính công nghệ này. Đối với các nhà đầu tư mạo hiểm và những kẻ đầu cơ giàu có, đây có thể chỉ là một trò chơi giải trí, nhưng đối với những người bình thường đặt cược cả gia tài vào giấc mơ làm giàu nhanh, hậu quả của việc mất tiền có thể gây đổ vỡ cuộc sống gia đình họ.

Chúng tôi sẽ không đánh đổi lòng tin của người dùng để tích hợp một tính năng rủi ro như vậy vào sản phẩm của mình.

## 言论

1\.

Thời kỳ mới gia nhập đội ngũ phát triển máy chơi game Xbox của Microsoft, tôi không được phân công vào nhóm phát triển kiến trúc CPU mà chỉ được cấp quyền đọc tài liệu kỹ thuật của chip. Dù vậy, tôi có niềm đam mê cực kỳ lớn với cấu trúc phần cứng. Một mùa đông năm đó, bão tuyết làm đổ cột điện gây mất điện toàn khu vực nhà tôi. Tôi đã nằm trên sàn phòng khách tối om, bật đèn pin đọc tỉ mỉ từng trang tài liệu cấu tạo CPU cho tới khi hiểu rõ đường đi của từng chân linh kiện. Chính sự kiên trì tự học đó đã đưa tôi trở thành chuyên gia về CPU của cả đội ngũ sau này.

-- Kỹ sư phần mềm Bruce Dawson chia sẻ

2\.

Tài sản số hóa NFT hoàn toàn không cấp cho bạn bản quyền tác giả, quyền sử dụng hay quyền sở hữu hợp pháp đối với tác phẩm nghệ thuật gốc dưới bất kỳ luật pháp quốc gia nào. Khi bạn bỏ tiền mua một NFT, thực tế thứ bạn nhận được chỉ là một mã hóa hóa đơn điện tử xác nhận giao dịch (receipt) lưu trên blockchain ngoài ra không có gì khác. Điểm thú vị là NFT cho phép bạn tìm cách bán lại chính hóa đơn đó cho người khác với giá cao hơn để kiếm lời.

-- Trích bài phân tích về công nghệ NFT

3\.

Sự nỗ lực bền bỉ, kiên trì và có kỷ luật hàng ngày dù rất nhỏ cuối cùng sẽ mang lại những kết quả đột phá đáng kinh ngạc. Mỗi khi cảm thấy mệt mỏi với nhịp sống lặp đi lặp lại thường nhật, tôi luôn tự nhắc nhở bản thân rằng việc kiên trì thực hiện công việc đều đặn mỗi ngày là điều quan trọng nhất. Dù chưa thể nhìn rõ tương lai sẽ ra sao, tôi tin vào sức mạnh tích lũy của sự bền bỉ, đúng như câu tục ngữ cổ: "Hãy tiếp tục làm việc".

-- Trích bài viết "Lessons from the sea"

## 历史上的本周

- 2021年（第 148 期）：[Thảo luận về các giải pháp thích ứng của doanh nghiệp trong kỷ nguyên tăng trưởng chậm (Micro-growth era)](https://www.ruanyifeng.com/blog/2021/03/weekly-issue-148.html)
- 2020年（第 96 期）：[Phân tích thực tế: Lập trình giảng dạy trực tuyến hiệu quả không đơn thuần là việc ghi hình lại bài giảng video sẵn có](https://www.ruanyifeng.com/blog/2020/02/weekly-issue-96.html)
- 2019年（第 45 期）：[Đọc hiểu và chia sẻ cảm nghĩ về cuốn hồi ký cuộc đời 《Sân khấu cuộc đời》 của nhà văn Isaac Asimov](https://www.ruanyifeng.com/blog/2019/03/weekly-issue-45.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
