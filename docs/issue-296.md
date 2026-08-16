# Bản tin chia sẻ công nghệ (Số 296): Tác giả đứng sau cửa sau xz - Jia Tan là ai?

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/4204) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040706.webp)

Ga Nam Xương Đông hoàn thành xây dựng vào cuối năm ngoái. Công trình lấy cảm hứng từ tác phẩm "Đằng Vương Các Tự" với câu thơ "Lạc hà dữ cô vụ tề phi, thu thủy cộng trường thiên nhất sắc" (Bóng chiều cùng cánh cò cô độc bay liệng, nước thu cùng bầu trời một màu). Thiết kế mái vòm như đôi cánh đang dang rộng tự do bay lượn, tượng trưng cho sự trỗi dậy mạnh mẽ của thành phố. (Nguồn: [Sohu](https://www.sohu.com/a/747607834_791225))

## xz 后门的作者 Jia Tan 是谁？

Sự kiện thu hút sự quan tâm lớn nhất của ngành công nghiệp Internet gần đây chắc chắn là vụ [cài cắm cửa sau (backdoor) trong gói phần mềm xz](https://boehs.org/node/everything-i-know-about-the-xz-backdoor).

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040903.webp)

xz là một công cụ nén dữ liệu phổ biến được sử dụng rộng rãi trên các hệ thống Linux, ví dụ như trình quản lý hệ thống systemd sử dụng nó để nén các tệp tin nhật ký nhật trình (logs). Nó là một thành phần cốt lõi của hệ điều hành Linux và hầu như máy chủ nào cũng được cài đặt sẵn.

Vào cuối tháng 3 năm nay, một kỹ sư phát hiện phiên bản mới nhất của gói thư viện này có biểu hiện bất thường, khiến thời gian khởi động dịch vụ bảo mật SSH bị chậm đi khoảng 500 mili giây. Quá trình điều tra sâu sau đó đã phát hiện ra sự tồn tại của một backdoor vô cùng tinh vi.

Vụ việc này đã gây rúng động toàn bộ cộng đồng bảo mật thông tin trên thế giới. Nguyên nhân do phiên bản bị cài cắm mã độc này chuẩn bị được tích hợp trực tiếp vào các bản phân phối Linux phổ biến (như Debian và Fedora) chỉ trong vòng vài ngày nữa. Nếu điều đó xảy ra, hàng triệu máy chủ trên thế giới sẽ tự động tích hợp sẵn backdoor này, hậu quả để lại sẽ vô cùng khủng khiếp.

Hơn nữa, **toàn bộ kế hoạch cài cắm này đã được chuẩn bị vô cùng tỉ mỉ và kiên trì trong suốt nhiều năm trời mà không hề để lộ bất kỳ sơ hở nào**. Kế hoạch chi tiết, tính kiên nhẫn cao và năng lực kỹ thuật xuất sắc của nhóm tin tặc khiến bất kỳ ai cũng phải rùng mình.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040902.webp)

Sự kiện bắt đầu từ tháng 4 năm 2021, khi một tài khoản GitHub có tên Jia Tan thực hiện gửi bản vá (patch) sửa lỗi bình thường đầu tiên cho dự án xz và được chấp thuận tích hợp thành công.

Trong các tháng 11 năm 2021 và tháng 4 năm 2022, tài khoản này tiếp tục đóng góp thêm hai bản vá sửa lỗi hữu ích khác và đều được tích hợp thành công vào mã nguồn dự án.

Sau đó, một nhóm tài khoản người dùng bất ngờ xuất hiện trên diễn đàn trao đổi (mailing list) của dự án để gửi phản hồi tới nhà phát triển chính của dự án rằng dự án xz hiện đang quá thiếu nhân sự duy trì dẫn đến tốc độ phản hồi chậm, và đề xuất nên cấp quyền quản trị viên (maintainer) cho tài khoản Jia Tan để cùng hỗ trợ phát triển. Đề xuất này sau đó đã được chấp thuận. Tuy nhiên hiện nay các kỹ sư phát hiện ra toàn bộ nhóm tài khoản gửi phản hồi năm xưa đều sử dụng các địa chỉ email ảo và hoàn toàn không có bất kỳ dấu vết hoạt động nào khác trên internet.

Bằng phương pháp này, Jia Tan đã chính thức trở thành một trong các quản trị viên của dự án, sở hữu quyền hạn phát hành và xuất bản trực tiếp các phiên bản mới của gói phần mềm. Ban đầu, các đoạn mã đóng góp của tài khoản này có vẻ vô hại nhưng thực chất được thiết kế để mở rộng tính năng làm nền tảng cho việc cài cắm mã độc sau này.

Vào tháng 2 năm 2024, tài khoản này chính thức chèn mã độc backdoor vào dự án. Đoạn mã đã được làm rối (obfuscated) kỹ lưỡng, đồng thời tệp tin backdoor không nằm trực tiếp trong kho mã nguồn chính mà chỉ được tự động tạo ra trong quá trình biên dịch (build phase) khiến việc phát hiện bằng mắt thường cực kỳ khó khăn. Ngay sau khi phát hành phiên bản mới, tài khoản này liên tục gửi thư hối thúc các nhóm phát triển bản phân phối Linux lớn sớm cập nhật phiên bản mới này.

**Ngay sau khi thông tin backdoor bị phơi bày ra ánh sáng, tài khoản Jia Tan đã lập tức biến mất hoàn toàn** mà không để lại bất kỳ thông tin nhận dạng cá nhân hay dấu vết hoạt động nào khác trên mạng. Cộng đồng bảo mật hiện đang nỗ lực thu thập các manh mối để tìm ra danh tính thực sự đứng sau tài khoản này.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040904.webp)

Tên tài khoản sử dụng cách viết phiên âm Pinyin của tiếng Trung, địa chỉ email đăng ký ghi đầy đủ họ tên là Jia Cheong Tan (trong đó chữ Cheong dường như là cách viết phiên âm theo tiếng Quảng Đông). Các mốc thời gian commit mã nguồn trên GitHub chủ yếu tập trung vào múi giờ Đông 8 (GMT+8). Địa chỉ IP kết nối được xác định tại Singapore.

**Mọi manh mối ban đầu đều hướng tới giả thuyết đây là một lập trình viên gốc Hoa sinh sống tại Singapore. Tuy nhiên thực tế có phải như vậy?**

Tên tài khoản hiển thị chắc chắn là giả, mốc thời gian commit hoàn toàn có thể được điều chỉnh bằng các dòng lệnh Git cấu hình, và địa chỉ IP kết nối đã được xác định là địa chỉ VPN giả lập.

**Liệu có khả năng kẻ tấn công cố tình giả mạo danh tính người gốc Hoa để đổ lỗi cho Trung Quốc?**

Một số chuyên gia bảo mật đã thực hiện [phân tích chi tiết](https://rheaeve.substack.com/p/xz-backdoor-times-damned-times-and) toàn bộ lịch sử commit mã nguồn của tài khoản này trên GitHub. Dù thời gian commit có thể chỉnh sửa giả lập, nhưng kẻ tấn công khó có thể ngụy tạo hoàn hảo toàn bộ tiến trình commit liên tục trong nhiều năm mà vẫn đảm bảo tính logic và tốc độ phản hồi tự nhiên, nên từ đó vẫn hé lộ ra một số manh mối quan trọng.

Phần lớn các commit sử dụng mốc giờ của múi giờ Đông 8, tuy nhiên có một số lượng commit lại vô tình ghi nhận mốc giờ thuộc múi giờ Đông 2 và Đông 3.

Các nhà nghiên cứu tin rằng **kẻ tấn công thực tế là một lập trình viên người châu Âu sinh sống tại khu vực múi giờ Đông 2, cố tình ngụy trang thành người gốc Hoa ở múi giờ Đông 8**. Người này đã thay đổi cài đặt múi giờ trên máy tính cá nhân nhưng đôi khi sơ suất quên không cấu hình lại trước khi commit.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040905.webp)

Các quốc gia thuộc múi giờ Đông 2 (vùng màu xanh trên bản đồ) chủ yếu tập trung tại khu vực Đông Âu, một số quốc gia Bắc Âu (như Phần Lan, Thụy Điển) và một số nước Trung Đông (như Israel, Ai Cập).

Có ba luận điểm chính ủng hộ giả thuyết tài khoản này hoạt động tại khu vực múi giờ Đông 2:

（1）Các commit ghi nhận múi giờ Đông 2 chủ yếu diễn ra vào mùa đông, trong khi các commit ghi nhận múi giờ Đông 3 lại diễn ra vào mùa hè. Quy luật này hoàn toàn trùng khớp với lịch chuyển đổi giờ mùa hè (Daylight Saving Time - DST) của các quốc gia châu Âu và Israel.

（2）Kẻ tấn công rõ ràng thực hiện thay đổi múi giờ thủ công. Ví dụ vào ngày 6 tháng 10 năm 2022, tài khoản này thực hiện một commit lúc 17:00:38 theo múi giờ Đông 8, sau đó lại thực hiện commit tiếp theo lúc 21:53:09 theo múi giờ Đông 3. Hai commit chỉ cách nhau chưa đầy 10 tiếng đồng hồ, rất khó tin lập trình viên có thể di chuyển từ Trung Quốc sang châu Âu trong khoảng thời gian ngắn đó chỉ để tiếp tục viết code.

（3）Tài khoản này ghi nhận lịch commit liên tục vào các ngày nghỉ lễ truyền thống của Trung Quốc (như Tết Trung thu, Thanh minh, Tết Nguyên đán). Đặc biệt trong kỳ nghỉ Tết Nguyên đán năm 2023 (từ ngày 21 đến ngày 27 tháng 1), tài khoản này ghi nhận hoạt động commit liên tục trong 5 ngày (các ngày 22, 23, 24, 26 và 27), chứng tỏ lập trình viên này hoàn toàn không ăn Tết theo phong tục Á Đông. Ngược lại, tài khoản này hoàn toàn không có hoạt động commit nào vào các ngày lễ lớn của phương Tây như Giáng sinh và Năm mới.

Tóm lại, nhiều khả năng tài khoản Jia Tan đứng sau cuộc tấn công này hoạt động tại khu vực múi giờ Đông 2. Tuy nhiên, do cá nhân hoặc tổ chức đứng sau chiến dịch này hoạt động vô cùng cẩn mật và sở hữu trình độ công nghệ thông tin xuất sắc, danh tính thực sự của họ có thể sẽ mãi mãi nằm trong bóng tối.

Sự kiện này là lời cảnh báo sâu sắc cho cộng đồng mã nguồn mở rằng không phải tất cả những người tham gia đóng góp đều mang mục đích tốt đẹp. Có những thế lực vô cùng thâm độc sẵn sàng lên kế hoạch dài hạn cài cắm mã độc và ngụy tạo danh tính để đổ lỗi cho người khác. Do đó, bên cạnh việc duy trì tinh thần cởi mở, chúng ta cũng cần nâng cao cảnh giác. Đã có đề xuất rằng các dự án mã nguồn mở quan trọng cần từ chối tiếp nhận đóng góp mã nguồn từ các tài khoản ẩn danh hoặc không xác thực được danh tính thực tế.

## 科技动态

1、[Cảnh báo về xu hướng đồng nhất hóa họ của người dân Nhật Bản](https://www.spoon-tamago.com/2531-sato-surname-problem/)

Một giáo sư đại học Nhật Bản đưa ra cảnh báo rằng nếu xu hướng suy giảm dân số hiện tại tiếp tục kéo dài, đến năm 2531 toàn bộ người dân Nhật Bản có thể sẽ mang chung một họ là Sato (佐藤).

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040206.webp)

Họ Sato hiện là họ phổ biến nhất tại Nhật Bản, chiếm khoảng 1,5% tổng dân số. Do dân số Nhật Bản đang có xu hướng giảm nhanh, các dòng họ hiếm gặp dần biến mất khiến cấu trúc họ của người dân có xu hướng tập trung vào các họ lớn.

Đồng thời, quy định pháp luật hiện hành của Nhật Bản bắt buộc phụ nữ sau khi kết hôn phải đổi sang họ của gia đình chồng cũng là nguyên nhân khiến các họ nhỏ khó duy trì.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040205.webp)

*(Chú thích ảnh: Đội hình thi đấu của một câu lạc bộ bóng đá nơi tất cả các cầu thủ đều mang họ Sato).*

Các số liệu thống kê cho thấy trong giai đoạn 2022-2023, tỷ lệ người mang họ Sato tăng trưởng tới 0,83%. Nghĩa là trong khi tổng dân số quốc gia giảm đi thì số lượng người mang họ Sato lại có xu hướng tăng lên.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040207.webp)

Dựa trên thuật toán tính toán của giáo sư, nếu giữ nguyên tốc độ tăng trưởng này, đến năm 2531 Nhật Bản sẽ không còn họ thứ hai và tất cả người dân đều mang họ Sato.

Để cảnh báo người dân, ông đã thiết lập trang web [Dự án Nghiên cứu Họ Sato](https://think-name.jp/) nhằm kêu gọi chính phủ sớm thay đổi luật bắt buộc đổi họ sau kết hôn.

2、[Kỷ lục thế giới mới về số lượng loài chim quan sát được ngoài tự nhiên](https://www.theguardian.com/environment/2024/mar/24/birding-online-community-10000-species)

Trang web [iGoTerra](https://igoterra.com) là một cộng đồng trực tuyến uy tín dành cho những người yêu thích thiên nhiên hoang dã chia sẻ và ghi chép lại hình ảnh các loài động vật họ quan sát được ngoài tự nhiên.

Hệ thống sở hữu [bảng xếp hạng thành tích](https://igoterra.com/rankings?group=33&rank=8&area=312025&year=-1&observedSeen=1) ghi nhận số lượng loài chim quan sát được của các thành viên. Mới đây, cộng đồng đã chứng kiến cột mốc lịch sử khi lần đầu tiên có một thành viên ghi nhận quan sát được hơn 10.000 loài chim khác nhau.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040303.webp)

Người xác lập kỷ lục này là Peter Kaestner - một cựu ngoại giao người Mỹ 70 tuổi đã nghỉ hưu. Hình ảnh dưới đây chụp loài chim hút mật mà ông chụp được tại Philippines vào ngày 9 tháng 2 năm 2024, đánh dấu loài chim thứ 10.000 trong hành trình của ông.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040304.webp)

Đây là một con số kỷ lục phi thường bởi tổng số loài chim được biết đến trên Trái Đất hiện nay chỉ khoảng 11.000 loài, đồng nghĩa với việc ông đã được nhìn thấy hầu như tất cả các loài chim trên hành tinh.

Sự hỗ trợ của công nghệ hiện đại đóng vai trò quan trọng giúp những người yêu chim đạt được thành tích này. Các thuật toán học máy hiện nay có khả năng tự động nhận diện chính xác loài chim từ hình ảnh chụp được hoặc phân tích từ tiếng hót, kết hợp cùng cộng đồng iGoTerra chia sẻ dữ liệu vị trí xuất hiện của các loài chim quý hiếm.

Bên cạnh đó, nhờ sự phát triển của ngành phân loại học, nhiều loài chim trước đây được gộp chung nay được phân tách thành các loài độc lập, góp phần làm tăng tổng số lượng loài chim được ghi nhận.

Tuy nhiên, cộng đồng iGoTerra chỉ yêu cầu người dùng upload ảnh chụp hoặc tệp ghi âm tiếng hót làm bằng chứng chứ không thực hiện quy trình thẩm định thực tế nghiêm ngặt.

3、[Giai thoại lịch sử về nguồn gốc ra đời của tập đoàn Apple](https://www.vintag.es/2024/04/steve-wozniak-working-in-garage.html)

Trong tháng này, tập đoàn công nghệ Apple đã tổ chức kỷ niệm [48 năm ngày thành lập](https://www.benzinga.com/markets/equities/24/04/38023363/happy-48-apple-if-you-invested-1000-in-apple-when-it-went-public-heres-how-much-youd-have). Doanh nghiệp được thành lập vào ngày 1 tháng 4 năm 1976 bởi Steve Jobs và Steve Wozniak tại bang California, Mỹ.

Thời kỳ đầu thành lập, cả hai đã tận dụng không gian nhà kho để xe chật hẹp của cha mẹ Steve Jobs để làm nơi lắp ráp thủ công các bo mạch máy tính đầu tiên đem bán.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040208.webp)

Không gian nhà kho khi đó vô cùng đơn sơ qua các bức ảnh tư liệu lịch sử dưới đây chụp cảnh Steve Wozniak đang miệt mài làm việc một mình.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040209.webp)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040210.webp)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040211.webp)

Hai nhà sáng lập thời điểm đó chắc chắn khó có thể hình dung doanh nghiệp nhỏ của họ sau này lại phát triển trở thành một đế chế công nghệ khổng lồ hàng đầu thế giới.

## Bài viết

1\. [Giới thiệu giáo sư đầu tiên vinh dự nhận cả hai giải thưởng danh giá Turing và Abel](https://www.163.com/dy/article/IVGAHL7K0511ABV6.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041108.webp)

Giải thưởng Turing danh giá nhất ngành khoa học máy tính vừa chính thức vinh danh giáo sư toán học Avi Wigderson thuộc Viện Nghiên cứu Cao cấp Princeton. Ông cũng là nhà khoa học duy nhất trong lịch sử từng nhận cả giải thưởng Abel - giải thưởng cao quý nhất ngành toán học.

2\. [Đánh giá các thư viện Frontend tiềm năng thay thế cho React](https://joshcollinsworth.com/blog/antiquated-react)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081606.webp)

Bài phân tích chi tiết chỉ ra các điểm hạn chế và các cơ chế thiết kế dần lỗi thời của React framework, đồng thời giới thiệu các giải pháp công nghệ Frontend mới thay thế.

3\. [Hướng dẫn xây dựng hệ thống theo dõi và phân tích lịch sử phím gõ](https://greptime.com/blogs/2024-03-19-keyboard-monitoring)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040306.webp)

Bài viết hướng dẫn lập trình viên viết một đoạn mã Python đơn giản để thống kê và phân tích các phím bấm người dùng thao tác trên máy tính cá nhân. (Đóng góp của [@tisonkun](https://github.com/ruanyf/weekly/issues/4195))

4\. [Khám phá 4 tính năng ưu việt của Claude AI so với ChatGPT](https://www.zdnet.com/article/4-things-claude-ai-can-do-that-chatgpt-cant/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090711.webp)

Claude là mô hình ngôn ngữ lớn mạnh mẽ phát triển bởi công ty Anthropic, cung cấp cả gói miễn phí lẫn gói trả phí [Claude Pro](https://www.zdnet.com/article/anthropic-unveils-claude-pro-a-paid-subscription-plan-for-its-chatgpt-rival/). Bài viết so sánh 4 điểm mạnh vượt trội của Claude khi đặt cạnh ChatGPT.

5\. [Hướng dẫn thiết lập Caddy làm máy chủ Reverse Proxy](https://linuxiac.com/how-to-set-up-caddy-as-reverse-proxy/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032907.webp)

Bài viết hướng dẫn nhập môn chi tiết cách cấu hình máy chủ web Caddy đóng vai trò đại diện ngược (reverse proxy). Caddy sở hữu cơ chế cấu hình đơn giản hơn nhiều so với Nginx và tích hợp tính năng tự động đăng ký và gia hạn chứng chỉ bảo mật HTTPS.

6\. [Góc nhìn lập trình: Sự đánh đổi giữa mã nguồn sạch và khả năng mở rộng](https://overreacted.io/goodbye-clean-code/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120807.webp)

Một bài chia sẻ kinh nghiệm cũ của lập trình viên nổi tiếng Dan Abramov. Ông từng tự ý refactor lại một phần mã nguồn của đồng nghiệp vì cho rằng nó quá dài dòng và dư thừa nhằm biến nó thành "clean code".

Tuy nhiên sau này ông nhận ra những phần code có vẻ dư thừa đó thực chất lại là thiết kế mở giúp hệ thống dễ dàng mở rộng tính năng sau này, trong khi việc đóng gói quá mức đôi khi gây cản trở cho việc bảo trì.

## AI 相关

1\. [ChatGPT mở rộng dịch vụ cho phép trải nghiệm không cần đăng nhập tài khoản](http://chatgpt.com/)

OpenAI thông báo chính thức gỡ bỏ yêu cầu đăng nhập đối với dịch vụ ChatGPT cơ bản, cho phép người dùng lướt web truy cập trực tiếp. Tuy nhiên các tính năng nâng cao (như mô hình GPT-4 hay trình tạo ảnh DALL-E) vẫn yêu cầu tài khoản.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040201.webp)

2\. [Trình duyệt Opera tích hợp sâu tính năng cài đặt mô hình AI chạy cục bộ](https://www.opera.com/zh-cn)

Hãng trình duyệt Opera [công bố](https://press.opera.com/2024/04/03/ai-feature-drops-local-llms/) tích hợp tính năng cho phép người dùng trực tiếp tải và chạy hơn 50 mô hình AI ngôn ngữ lớn ngay trên máy tính cá nhân (mỗi mô hình chiếm dụng khoảng 2GB dung lượng), giúp tối ưu hóa bảo mật dữ liệu.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040401.webp)

3\. [Suno Prompt (Công cụ hỗ trợ tạo câu lệnh viết nhạc cho Suno AI)](https://sunoprompt.com/)

Dịch vụ trực tuyến giúp người dùng thiết kế và tối ưu các câu lệnh (prompts) mô tả âm nhạc để gửi cho Suno AI tạo bài hát. (Đóng góp của [@Lcorinst](https://github.com/ruanyf/weekly/issues/4194))

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040305.webp)

Bên cạnh đó bạn đọc có thể tham khảo thêm [Suno AI Music Downloader](https://sunoaidownload.com/) hỗ trợ tải nhạc. (Đóng góp của [@AICodeHunt](https://github.com/ruanyf/weekly/issues/4250))

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041104.webp)

4\. [Free Prompt Market (Thư viện chia sẻ câu lệnh tạo ảnh AI miễn phí)](https://artiversehub.ai/prompt-marketplace)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040311.webp)

Trang web chia sẻ và tổng hợp các câu lệnh mẫu chất lượng dành cho các mô hình AI tạo ảnh phổ biến hiện nay. (Đóng góp của [@leoli202303](https://github.com/ruanyf/weekly/issues/4209))

## 工具

1\. [DOOM Captcha (Trình xác thực người dùng bằng trò chơi bắn súng DOOM)](https://vivirenremoto.github.io/doomcaptcha/)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032906.webp)

Ý tưởng thiết kế trình captcha độc đáo dựa trên trò chơi huyền thoại DOOM, yêu cầu người dùng phải tiêu diệt đủ số lượng quái vật hiển thị để vượt qua xác thực.

2\. [OneUptime (Giải pháp giám sát trạng thái hệ thống máy chủ)](https://github.com/OneUptime/oneuptime)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040301.webp)

Công cụ mã nguồn mở hỗ trợ theo dõi trạng thái hoạt động (uptime) của hệ thống máy chủ dịch vụ, tự động gửi cảnh báo lập tức nếu dịch vụ gặp sự cố dừng hoạt động, giải pháp thay thế tốt cho StatusPage.io.

3\. [DashPress (Trình tự động tạo giao diện quản trị Admin tự động)](https://github.com/dashpresshq/dashpress)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040302.webp)

Công cụ mã nguồn mở hỗ trợ tự động quét cấu trúc cơ sở dữ liệu để tạo lập nhanh trang quản trị admin mà hoàn toàn không cần viết mã nguồn.

4\. [Landing Page Boilerplate (Bộ mã nguồn mẫu thiết kế trang Landing Page)](https://github.com/weijunext/landing-page-boilerplate)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040307.webp)

Bộ khung mã nguồn mở hỗ trợ lập trình viên xây dựng nhanh giao diện trang giới thiệu sản phẩm (landing page). Tham khảo thêm [bài viết giới thiệu chi tiết](https://juejin.cn/post/7350200488455520267). (Đóng góp của [@weijunext](https://github.com/ruanyf/weekly/issues/4197))

5\. [GitHub Custom Notifier (Tiện ích mở rộng nhận thông báo tùy biến trên GitHub)](https://github.com/qiweiii/github-custom-notifier)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040308.webp)

Tiện ích mở rộng trên trình duyệt hỗ trợ lập trình viên đăng ký theo dõi các sự kiện đặc thù trên kho lưu trữ GitHub (như việc tạo mới nhãn label) vốn không được hệ thống thông báo mặc định của GitHub hỗ trợ. (Đóng góp của [@qiweiii](https://github.com/ruanyf/weekly/issues/4199))

6\. [HeyForm (Trình thiết kế biểu mẫu khảo sát trực tuyến)](https://github.com/heyform/heyform)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040310.webp)

Công cụ mã nguồn mở giúp người dùng nhanh chóng thiết kế các bảng khảo sát, biểu mẫu thu thập ý kiến, bình chọn trực tuyến mà không cần lập trình. (Đóng góp của [@iMuFeng](https://github.com/ruanyf/weekly/issues/4207))

7\. [Youdeyiwu (Mã nguồn diễn đàn thảo luận tối giản)](https://github.com/dafengzhen/youdeyiwu)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040312.webp)

Mã nguồn mở hỗ trợ thiết kế trang diễn đàn thảo luận gọn nhẹ, tối giản giao diện, phát triển phần Backend bằng ngôn ngữ Java và Frontend bằng Next.js. (Đóng góp của [@dafengzhen](https://github.com/ruanyf/weekly/issues/4211))

8\. [Markdown Genji (Plugin nhúng mã chạy trực tiếp vào tệp tài liệu)](https://genji-md.dev/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040313.webp)

Một plugin dành cho trình đóng gói tài liệu VitePress hỗ trợ nhúng các khối code thực thi được trực tiếp vào tệp Markdown để tạo tài liệu hướng dẫn tương tác. (Đóng góp của [@pearmini](https://github.com/ruanyf/weekly/issues/4212))

9\. [Mutative (Thư viện tối ưu hóa xử lý Immutable State)](https://github.com/ruanyf/weekly/issues/4222)

Thư viện JavaScript hỗ trợ cập nhật và quản lý trạng thái không đổi (immutable state) với hiệu năng xử lý cực cao. (Đóng góp của [@unadlib](https://github.com/ruanyf/weekly/issues/4222))

10\. [Fusion (Trình quản lý và đọc tin tức RSS tối giản)](https://github.com/0x2E/fusion)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040501.webp)

Ứng dụng hỗ trợ đăng ký và theo dõi tin tức định dạng RSS gọn nhẹ, phát triển dựa trên ngôn ngữ Go và Svelte. (Đóng góp của [@0x2E](https://github.com/ruanyf/weekly/issues/4223))

11\. [node-screenshots (Thư viện hỗ trợ chụp ảnh và ghi hình màn hình)](https://github.com/nashaofu/node-screenshots)

Mô-đun Node.js gọn nhẹ hỗ trợ lập trình viên xây dựng tính năng chụp ảnh màn hình hoặc ghi hình video màn hình đa nền tảng mà không yêu cầu thêm thư viện đi kèm. (Đóng góp của [@nashaofu](https://github.com/ruanyf/weekly/issues/4224))

12\. [Lưu loát đọc (Tiện ích dịch thuật trang web thông minh)](https://github.com/Bistutu/FluentRead)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040707.webp)

Tiện ích mở rộng dịch thuật trang web trên trình duyệt hỗ trợ kết nối các công cụ dịch thuật AI thông minh. (Đóng góp của [@Bistutu](https://github.com/ruanyf/weekly/issues/4230))

13\. [keynavish (Công cụ hỗ trợ điều khiển chuột bằng bàn phím)](https://github.com/lesderid/keynavish)

Phần mềm chạy trên hệ điều hành Windows hỗ trợ người dùng điều khiển tọa độ chuột thông qua các phím bấm bàn phím. (Đóng góp của [@NomandChan](https://github.com/ruanyf/weekly/issues/55))

14\. [K8Z (Công cụ quản lý hạ tầng Kubernetes tiện lợi)](https://github.com/k8zdev/k8z)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041002.webp)

Công cụ mã nguồn mở hỗ trợ theo dõi và quản lý cụm máy chủ Kubernetes, cung cấp ứng dụng khách đầy đủ cho thiết bị di động và máy tính để bàn. (Đóng góp của [@kofj](https://github.com/ruanyf/weekly/issues/4246))

## 资源

1\. [Giáo trình hướng dẫn tự học Next.js tiếng Trung](https://qufei1993.github.io/nextjs-learn-cn)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040309.webp)

Bản dịch tiếng Trung của tài liệu [Next.js Learn chính thức](https://nextjs.org/learn), hướng dẫn lập trình viên từng bước xây dựng một ứng dụng web full-stack. (Đóng góp của [@qufei1993](https://github.com/ruanyf/weekly/issues/4206))

2\. [3DP.ing (Trình tìm kiếm mô hình in 3D bằng hình ảnh)](https://3dp.ing/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040602.webp)

Công cụ hỗ trợ tìm kiếm các file thiết kế mô hình in 3D, đặc biệt hỗ trợ tìm kiếm bằng cách phân tích hình ảnh đầu vào. (Đóng góp của [@wangasa](https://github.com/ruanyf/weekly/issues/4227))

3\. [1000UserGuide (Danh bạ các kênh truyền thông tiếp thị miễn phí)](https://1000userguide.com)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040901.webp)

Trang web tổng hợp thông tin của hơn 300 kênh truyền thông giới thiệu sản phẩm miễn phí (bao gồm các diễn đàn, danh bạ web...) hỗ trợ các lập trình viên độc lập quảng bá sản phẩm mới ra mắt. (Đóng góp của [@naxiaoduo](https://github.com/ruanyf/weekly/issues/4240))

4\. [Awesome Cloudflare (Tổng hợp các dự án mã nguồn mở phát triển trên Cloudflare)](https://github.com/zhuima/awesome-cloudflare)

Kho lưu trữ chia sẻ danh sách các công cụ mã nguồn mở và giải pháp công nghệ phát triển dựa trên hệ sinh thái dịch vụ của Cloudflare. (Đóng góp của [@zhuima](https://github.com/ruanyf/weekly/issues/4244))

5\. [Tài liệu hướng dẫn mạng máy tính Beej's Guide to Network Concepts bản dịch tiếng Trung](https://github.com/rogerzhu/-bgnet0-cn/tree/main/src)

Bản dịch tiếng Trung do cộng đồng thực hiện cho cuốn sách mạng máy tính nhập môn nổi tiếng [《Beej's Guide to Network Concepts》](https://beej.us/guide/bgnet0/). (Đóng góp của [@rogerzhu](https://github.com/ruanyf/weekly/issues/4248))

## 图片

1\. [Hình ảnh sạt lở địa chất nghiêm trọng trên tuyến đường cao tốc ven biển California Highway 1](https://www.cnn.com/travel/california-highway-1-damage-big-sur/index.html)

Tuyến đường cao tốc ven biển nổi tiếng nối liền San Francisco và Los Angeles được xây dựng dọc theo sườn các dãy núi sát biển Thái Bình Dương mang lại cảnh quan thiên nhiên vô cùng kỳ vĩ.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040203.webp)

Tuy nhiên do địa hình xây dựng sát mép vực biển nên tuyến đường này thường xuyên phải đối mặt với các đợt sạt lở địa chất nguy hiểm. Trong tháng này, một vụ sạt lở lớn đã cuốn trôi một đoạn mặt đường xuống biển Thái Bình Dương buộc chính quyền phải ra lệnh phong tỏa tạm thời.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040202.webp)

2\. [Hố va chạm Plum Crater trên bề mặt Mặt Trăng](https://www.nasa.gov/image-article/craters-edge/)

Plum Crater là một hố va chạm thiên thạch quy mô nhỏ trên bề mặt Mặt Trăng với đường kính khoảng 40 mét và độ sâu lòng hố khoảng 10 mét.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032901.webp)

Hố va chạm này sở hữu giá trị lịch sử đặc biệt do là một trong số ít khu vực từng ghi nhận dấu chân của con người ghé thăm.

Vào ngày 21 tháng 4 năm 1972, tàu vũ trụ Apollo 16 đã lựa chọn bãi hạ cánh gần khu vực hố va chạm này.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032902.webp)

Hình ảnh ghi lại cảnh các phi hành gia đang thực hiện khảo sát địa chất thực địa sát mép hố va chạm.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032904.webp)

Dấu chân lịch sử của phi hành gia lưu lại trên bề mặt bụi Mặt Trăng vẫn được bảo tồn nguyên vẹn rõ nét (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032903.webp)

## ✍️ Bài đọc thêm

### Tìm hiểu về giá trị thiết kế và an toàn giao thông của các bùng binh vòng xuyến

Khi tham gia giao thông trên đường bộ, chắc chắn bạn đã từng đi qua nhiều bùng binh (vòng xuyến).

Có bao giờ bạn tự hỏi vì sao tại các giao lộ lớn người ta lại ưu tiên thiết kế các bùng binh hình tròn thay vì giải phóng không gian để tạo các ngã tư thông thường giúp tăng diện tích mặt đường xe chạy?

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102603.webp)

Về bản chất kỹ thuật, bùng binh là một phương pháp điều tiết giao thông thông minh sở hữu nhiều ưu điểm vượt trội khi so sánh với các ngã tư kiểm soát bằng đèn tín hiệu truyền thống, đặc biệt là khả năng nâng cao an toàn giao thông.

Trước tiên, cấu trúc bùng binh bắt buộc các tài xế phải chủ động giảm tốc độ lái xe để điều khiển đầu xe ôm cua theo vòng tròn.

Thứ hai, bùng binh giúp giảm thiểu đáng kể số lượng điểm xung đột giao thông tiềm ẩn. Điểm xung đột là tọa độ có nguy cơ xảy ra va chạm trực tiếp giữa các phương tiện với nhau hoặc giữa phương tiện với người đi bộ; số lượng điểm này càng lớn thì xác suất xảy ra tai nạn càng cao.

Các nghiên cứu kỹ thuật chỉ ra rằng cấu trúc bùng binh chỉ có 8 điểm xung đột tiềm ẩn, trong khi một ngã tư bốn chiều truyền thống có tới 32 điểm xung đột.

Cuối cùng, các làn xe di chuyển trong bùng binh được thiết kế dạng các đường tròn đồng tâm chật hẹp kết hợp hệ thống đường rẽ hướng ra vào buộc các phương tiện phải giảm tốc nhường đường nhau một cách nhịp nhàng.

Các số liệu thống kê của Cục Quản lý Đường cao tốc Liên bang Mỹ ước tính việc thay thế các giao lộ truyền thống bằng bùng binh giúp kéo giảm tới 80% đến 90% số vụ tai nạn giao thông nghiêm trọng.

Bên cạnh giá trị an toàn, bùng binh còn giúp duy trì trật tự dòng xe lưu thông ổn định, giảm thiểu hiện tượng ùn tắc giao thông hỗn loạn tại giao lộ và hỗ trợ tài xế quay đầu xe (u-turn) dễ dàng hơn.

## Lịch sử tuần này

- 2023年（第 249 期）：[Góc nhìn khởi nghiệp: Giới thiệu hành trình phát triển của các nhà doanh nghiệp phần mềm thành công](https://www.ruanyifeng.com/blog/2023/04/weekly-issue-249.html)
- 2022年（第 199 期）：[Bảo mật mạng: Phân tích sự cố chứng chỉ HTTPS của các dịch vụ internet tại Nga](https://www.ruanyifeng.com/blog/2022/03/weekly-issue-199.html)
- 2021年（第 149 期）：[Nhận định thị trường: Dự báo về các doanh nghiệp dẫn đầu trong cuộc đua xe điện thế hệ mới](https://www.ruanyifeng.com/blog/2021/03/weekly-issue-149.html)
- 2020年（第 99 期）：[Góc nhìn xã hội: Xu hướng mở rộng chỉ tiêu tuyển sinh nghiên cứu sinh do ảnh hưởng của dịch bệnh](https://www.ruanyifeng.com/blog/2020/03/weekly-issue-99.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
