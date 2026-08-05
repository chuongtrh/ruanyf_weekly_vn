# 科技爱好者周刊：第 88 期 (Bản tin chia sẻ công nghệ số 88)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

Mục tuyển dụng [《Ai đang tuyển dụng?》](https://github.com/ruanyf/weekly/issues/983) cung cấp nhiều thông tin việc làm hữu ích, hoan nghênh ghé thăm hoặc đăng tải thông tin tuyển dụng/thực tập.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019113002.jpg)

Ảnh bìa: Chú chuột túi (Kangaroo) bạch tạng, chú chuột túi con trong túi mẹ vẫn mang màu sắc bình thường. Ảnh từ [Instagram chính thức](https://www.instagram.com/p/B5cfkT2oXsq/) của Chính phủ Úc.

## 刊首语 (Lời tựa)

Gần đây, tôi có đọc được hai câu chuyện rất hay, cả hai đều sử dụng hình ảnh con rắn để ẩn dụ về phương thức quản lý doanh nghiệp.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122601.jpg)

Câu chuyện thứ nhất trích từ chia sẻ của James Barksdale, cựu CEO của tập đoàn Netscape:

> Tại Netscape, chúng tôi tuân thủ nghiêm ngặt 3 quy tắc:
> 
> Quy tắc số 1: Nếu bạn phát hiện một con rắn, đừng mất thời gian gọi điện báo cáo cho ban quản trị, đừng gọi điện buôn chuyện với đồng nghiệp, đừng lập một nhóm nghiên cứu, cũng đừng tổ chức một cuộc họp thảo luận. Việc duy nhất bạn phải làm là cầm gậy lên và tiêu diệt con rắn đó ngay lập tức.
> 
> Quy tắc số 2: Đừng bao giờ quay lại nghịch ngợm hay lãng phí thời gian chơi đùa với xác con rắn đã chết. Rất nhiều người đang tiêu tốn quá nhiều thời gian quý báu chỉ để bàn lùi hoặc nghi ngờ những quyết định đã được thống nhất đưa ra trước đó.
> 
> Quy tắc số 3: Mọi cơ hội kinh doanh lúc ban đầu trông đều đáng sợ và đầy rủi ro giống như một con rắn độc vậy, việc của bạn là phải tìm ra và giải quyết các điểm nghẽn của nó.

Hàm ý của ông rất rõ ràng: Người đầu tiên phát hiện ra vấn đề phát sinh trong doanh nghiệp phải chủ động bắt tay vào giải quyết ngay lập tức, tuyệt đối không được đùn đẩy trách nhiệm hay trì hoãn thời gian.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122602.jpg)

Câu chuyện thứ hai là nhận xét của tỷ phú Ross Perot về phong cách quản lý chậm chạp tại tập đoàn ô tô General Motors (GM):

> Tôi đến từ một môi trường làm việc mà ở đó, hễ ai phát hiện ra một con rắn bò vào nhà, họ sẽ lập tức đập chết nó.
> 
> Thế nhưng ở General Motors, nếu bạn phát hiện ra một con rắn, việc đầu tiên bạn làm là chi tiền thuê một chuyên gia tư vấn đến để thảo luận về sự xuất hiện của nó. Tiếp theo, một ban quản trị chuyên trách được thành lập để nghiên cứu các phương án xử lý. Sau vài năm thảo luận liên tục, kết quả khả thi nhất là... không làm gì cả. Bởi vì con rắn đó vẫn chưa cắn bất kỳ ai, nên mọi người vẫn thản nhiên để mặc nó bò lổm ngổm trên sàn nhà xưởng.
> 
> Chúng ta cần xây dựng một văn hóa doanh nghiệp mà ở đó, người đầu tiên phát hiện ra con rắn sẽ chủ động đập chết nó ngay lập tức.

Tôi nghĩ cả hai câu chuyện trên đều mang lại những bài học quản trị vô cùng sâu sắc đáng suy ngẫm.

Tuy nhiên, tiền đề để thực hiện các lời khuyên trên là bạn phải có đủ năng lực và công cụ để "tiêu diệt con rắn". Trên thực tế, đối với các doanh nghiệp nhỏ hoặc trong cuộc sống của mỗi cá nhân, những "con rắn" (khó khăn, khủng hoảng tài chính) ta gặp phải thường là những con mãng xà khổng lồ vượt quá khả năng xử lý của chúng ta tại thời điểm đó. Khi đó, chiến lược khả thi duy nhất có lẽ không phải là lao vào đối đầu trực diện, mà là tạm thời lờ nó đi, tập trung tối đa nguồn lực vào định hướng phát triển cốt lõi, nỗ lực tăng trưởng thật nhanh để bỏ xa mối đe dọa đó ở phía sau.

## Khóa học Vue.js miễn phí từ đối tác

Bản tin tuần này giới thiệu tới độc giả khóa học lập trình frontend hoàn toàn miễn phí được tài trợ bởi đối tác đào tạo **Kaikeba**.

Như các bạn đã biết, Vue.js là một trong những framework lập trình frontend chủ đạo hiện nay với ưu điểm dễ tiếp cận cho người mới bắt đầu, hiệu năng tối ưu và giao diện trực quan, chiếm thị phần tuyển dụng vô cùng lớn tại thị trường trong nước. Khả năng làm chủ Vue.js gần như là kỹ năng bắt buộc phải có khi tham gia các vòng phỏng vấn kỹ sư frontend.

Hiện tại, phiên bản thử nghiệm Vue.js 3.0 đã được công bố rộng rãi và phiên bản chính thức dự kiến sẽ ra mắt vào quý 1 năm sau. Điều này đồng nghĩa với việc rất nhiều tài liệu hướng dẫn và khóa học dựa trên phiên bản cũ Vue 2.x sẽ sớm trở nên lạc hậu.

Khóa học miễn phí **《Giải mã cơ chế phản ứng dữ liệu sinh học của Vue.js 3.0》** sẽ cập nhật hoàn toàn theo mã nguồn mới nhất của Vue 3, phân tích chi tiết cơ chế cập nhật dữ liệu hai chiều giữa UI và Model, so sánh sự khác biệt kiến trúc lõi giữa Vue 2 và Vue 3, đồng thời hướng dẫn học viên tự tay lập trình xây dựng hệ thống phản ứng dữ liệu Vue 3 từ đầu.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122409.jpg)

Độc giả quan tâm có thể quét mã QR dưới đây để liên hệ trợ lý học tập và nhận suất học thử miễn phí:

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122410.jpg)

## 资讯 (Tin tức)

1. **Báo chí kêu gọi di dời bức họa Mona Lisa sang một khu triển lãm riêng biệt để giảm tải cho bảo tàng Louvre**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110805.jpg)

Bức ảnh trên ghi lại khung cảnh chen chúc nghẹt thở trước bức họa kinh điển *Mona Lisa* của danh họa Leonardo da Vinci tại bảo tàng Louvre (Pháp) vào ngày 24/10 vừa qua. Ước tính có tới hơn 30.000 lượt khách đổ dồn về đây mỗi ngày chỉ để ngắm nhìn bức tranh này, tạo nên một trải nghiệm tham quan vô cùng tồi tệ khi phần lớn du khách chỉ có thể nhìn thấy bóng mờ của bức tranh từ khoảng cách rất xa qua rừng cánh tay chụp ảnh.

Bảo tàng Louvre là không gian triển lãm nghệ thuật rộng lớn nhất thế giới, và ngoại trừ phòng trưng bày bức họa Mona Lisa luôn quá tải, hầu hết các gian trưng bày tác phẩm nghệ thuật khác đều rất thưa vắng khách. Vấn đề quá tải của bảo tàng thực chất chỉ nằm ở duy nhất bức họa này.

Chuyên trang của tờ *New York Times* đã đăng tải bài viết đề xuất bảo tàng Louvre nên chủ động di dời bức Mona Lisa sang một tòa nhà triển lãm được xây dựng riêng biệt bên ngoài khuôn viên chính. Việc di dời này vừa giải quyết triệt để tình trạng ùn tắc giao thông cho bảo tàng, vừa tạo cơ hội cho du khách phân bổ đều thời gian thưởng thức hàng vạn tác phẩm nghệ thuật vô giá khác. Việc xây dựng một không gian trưng bày riêng biệt chắc chắn tiêu tốn khoản ngân sách khổng lồ, nhưng đối với một tác phẩm là biểu tượng văn hóa toàn cầu như Mona Lisa, việc thu hút các nguồn vốn tài trợ xã hội chắc chắn là vô cùng dễ dàng.

2. **Hiện tượng đa cấu trúc DNA di truyền kỳ lạ sau các ca phẫu thuật ghép tủy xương**

Các kỹ sư tại phòng thí nghiệm phân tích DNA thuộc Sở cảnh sát bang Nevada (Mỹ) mới đây đã gặp phải một trường hợp pháp y vô cùng hy hữu. Một bệnh nhân ung thư máu sau khi thực hiện ca phẫu thuật ghép tủy xương thành công được 4 năm, kết quả xét nghiệm cho thấy các mẫu tế bào máu, niêm mạc môi và má của anh đều chứa cấu trúc DNA của người hiến tặng tủy xương. Điều này đồng nghĩa với việc cơ thể anh hiện đang tồn tại song song hai hệ thống DNA khác biệt. Kinh ngạc hơn, toàn bộ cấu trúc DNA phát hiện trong tinh dịch của người này cũng hoàn toàn thuộc về người hiến tặng.

Các chuyên gia pháp y nhận định, cùng với sự phát triển của công nghệ ghép tạng và kỹ thuật sinh học hiện đại, hiện tượng một cá thể mang đồng thời nhiều bộ DNA khác nhau (chimerism) sẽ ngày càng trở nên phổ biến trong tương lai. Đây là yếu tố kỹ thuật mới mà các phòng khám nghiệm hiện trường vụ án bắt buộc phải lưu tâm khi phân tích các dấu vết DNA thu thập được.

3. **Nghiên cứu chỉ ra các chủng siêu vi khuẩn bệnh viện đang tiến hóa để kháng cự cồn sát trùng**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120903.jpg)

Để đảm bảo vệ sinh dịch tễ, các bệnh viện trên toàn thế giới đều sử dụng cồn sát trùng nồng độ cao (thường đạt mức 70% thay vì mức 23% của các sản phẩm gia dụng thông thường) để sát khuẩn tay và lau chùi các thiết bị y tế. Cồn nồng độ cao hoạt động trên nguyên lý phá hủy lớp màng tế bào của vi khuẩn làm chúng chết khô nhanh chóng.

Tuy nhiên, một nghiên cứu dài hạn của Đại học Melbourne (Úc) cảnh báo các chủng vi khuẩn thu thập từ các bệnh viện lớn đang có xu hướng tiến hóa mạnh mẽ để kháng cự lại tác nhân này. Kết quả thử nghiệm chỉ ra các chủng vi khuẩn thu thập trong giai đoạn 2009-2015 sở hữu khả năng sống sót cao gấp 10 lần trước sự cọ rửa bằng cồn nồng độ cao so với các chủng thu thập trước năm 2004. Phát hiện này đặt ra yêu cầu cấp thiết cho các bệnh viện phải kết hợp thêm các phương pháp diệt khuẩn vật lý hoặc hóa học khác bên cạnh việc lau cồn thông thường.

4. **Quân đội Mỹ chính thức thành lập Lực lượng Vũ trụ (U.S. Space Force)**

Lực lượng Vũ trụ Hoa Kỳ chính thức được thành lập vào ngày 20/12/2019 nhằm thực thi nhiệm vụ bảo vệ an ninh và lợi ích chiến lược của Mỹ trên không gian vũ trụ ngoài trái đất, trở thành quân chủng chính quy thứ 6 của quân đội Mỹ (bên cạnh Lục quân, Hải quân, Không quân, Thủy quân Lục chiến và Cảnh sát Biển).

Theo Luật Lực lượng Vũ trụ, quân chủng này có nhiệm vụ "đảm bảo tự do hành động của Mỹ trên không gian vũ trụ" và chịu trách nhiệm vận hành các khí tài không gian. Nhiều nhà vật lý vũ trụ đề xuất lực lượng này nên đảm nhận thêm các nhiệm vụ dân sự quan trọng như thu gom rác thải vệ tinh trên quỹ đạo và xây dựng hệ thống phòng thủ chống thiên thạch va chạm trái đất.

5. **Bộ đôi Mac Pro và màn hình chuyên nghiệp Pro Display XDR cấu hình tối đa vượt ngưỡng 50.000 USD**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121107.jpg)

Apple chính thức mở cổng đặt hàng cho dòng máy trạm Mac Pro thế hệ mới với mức giá khởi điểm từ 5.999 USD và có thể chạm mốc kỷ lục 52.599 USD cho phiên bản cấu hình tối đa (bao gồm vi xử lý Intel Xeon 28 nhân, 1.5TB RAM và hai card đồ họa chuyên dụng Radeon Pro Vega II Duo).

Nếu người dùng chọn mua kèm dòng màn hình Pro Display XDR phiên bản kính phủ nano chống lóa với mức giá 5.999 USD cộng thêm chân đế Pro Stand giá 999 USD, tổng chi phí cho trọn bộ máy trạm của Apple sẽ vượt ngưỡng 59.597 USD. Đây là mức giá chưa tính đến việc Mac Pro hỗ trợ xuất hình ảnh ra tối đa tới 8 màn hình chuyên nghiệp cùng lúc.

6. **Tin vắn**

- Báo cáo của Bộ Giáo dục Mỹ chỉ ra rằng trong danh sách 10 chuyên ngành đào tạo đại học có mức thu nhập bình quân của sinh viên sau khi tốt nghiệp năm thứ nhất cao nhất cả nước, có tới 9 vị trí thuộc về ngành Nha khoa (Dentistry).

- Dự án lò phản ứng hạt nhân thí điểm "Nhân tạo Thái Dương" thế hệ mới của Trung Quốc hoàn thành lắp đặt, hướng tới mục tiêu tạo ra môi trường nhiệt độ cực cao lên tới 200 triệu độ C để phục vụ các thí nghiệm phản ứng nhiệt hạch kiểm soát được vào năm sau.

- Một người dùng Instagram chia sẻ hình ảnh thú vị bên trong nhà vệ sinh của văn phòng Google Đài Bắc: thay vì dán các câu khẩu hiệu hay tranh trang trí thông thường, Google dán các tờ tài liệu hướng dẫn kỹ thuật chi tiết cách dò tìm và sửa các lỗi bug thường gặp trong mã nguồn (ảnh dưới).

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019122002.jpg)

## 文章 (Bài viết)

1、[Bài viết] [Làm thế nào để xây dựng một thư viện CSS dạng Utility-First tương tự như Tailwind CSS?](https://adamwathan.me/css-utility-classes-and-separation-of-concerns/) (Tiếng Anh)

Tác giả của framework nổi tiếng Tailwind CSS chia sẻ về hành trình tư duy của bản thân từ phương pháp viết CSS truyền thống (tách biệt mã nguồn) cho đến khi phát triển phương pháp tiếp cận hướng Utility-First giúp tái sử dụng tối đa các class CSS và tối ưu hóa tốc độ phát triển giao diện.

2、[Bài viết] [Hướng dẫn từng bước lập trình tự xây dựng một phiên bản React của riêng bạn](https://pomb.us/build-your-own-react/) (Tiếng Anh)

Bài viết hướng dẫn cực kỳ chi tiết kèm theo các đoạn mã nguồn tối giản mô phỏng lại các cơ chế hoạt động lõi của thư viện React: từ việc tạo phần tử ảo Virtual DOM, cơ chế Render, quy trình so sánh Diffing cho đến tính năng Concurrent Mode và React Hooks.

## 软件 (Phần mềm)

1、[EasyDB — Dịch vụ khởi tạo cơ sở dữ liệu đám mây tạm thời miễn phí](https://easydb.io/)

Cung cấp công cụ tạo nhanh một database (hỗ trợ MySQL, PostgreSQL, SQLite, Redis) trực tuyến chỉ với một cú click chuột để phục vụ chạy thử nghiệm dự án hoặc viết code demo, database sẽ tự động xóa sạch sau 24 giờ hoạt động.

2、[Sourcetrail — Công cụ phân tích và trực quan hóa cấu trúc mã nguồn dự án nguồn mở](https://www.sourcetrail.com/blog/open_source/)

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112116.jpg)

Phần mềm hỗ trợ các lập trình viên nhanh chóng làm quen với các dự án lớn bằng cách quét toàn bộ mã nguồn (hỗ trợ C/C++, Java, Python) để vẽ sơ đồ tương tác trực quan giữa các lớp, hàm và biến dữ liệu dưới dạng đồ thị tương tác.

3、[linjiashop — Dự án xây dựng hệ thống thương mại điện tử Web/Mobile hoàn chỉnh nguồn mở](https://github.com/microapp-store/linjiashop)

Dự án mẫu xây dựng hệ thống website bán hàng trực tuyến tích hợp ứng dụng di động hoàn chỉnh viết bằng Spring Boot (backend) và Vue.js (frontend), phù hợp cho các nhà phát triển tham khảo học tập kiến trúc hệ thống.

## 资源 (Tài nguyên)

1、[Tài liệu] [Tổng hợp các sự cố tai nạn nghiêm trọng trong lịch sử do lỗi phần mềm (Software Bugs) gây ra](https://www5.in.tum.de/~huckle/bugse.html)

Trang web tổng hợp thông tin, bài viết báo chí chi tiết về các sự cố tai nạn thảm khốc của nhân loại bắt nguồn từ lỗi lập trình phần mềm: từ sự cố nổ tên lửa Ariane 5, lỗi hệ thống điều trị bức xạ Therac-25 cho đến các lỗi tính toán định dạng ngày tháng.

2、[Tài liệu] [Bản dịch tiếng Trung bộ tài liệu quy chuẩn kỹ thuật Code Review của tập đoàn Google](https://github.com/xindoo/eng-practices-cn)

Dự án dịch thuật cộng đồng chia sẻ các quy tắc, tiêu chuẩn thực hành Code Review chính thức của Google: hướng dẫn cách viết nhận xét khoa học cho người review và cách tiếp nhận ý kiến chỉnh sửa của lập trình viên để nâng cao chất lượng mã nguồn.

## 图片 (Hình ảnh)

1. **Rotary Jails - Kiến trúc nhà tù xoay vòng tròn độc đáo của nước Mỹ đầu thế kỷ 20**

Vào cuối thế kỷ 19, hai kỹ sư người Mỹ đã đăng ký bản quyền sáng chế mẫu thiết kế nhà tù xoay tròn độc đáo. Các buồng giam được thiết kế xếp vòng tròn quanh một trục sắt lớn trung tâm, bao bọc bên ngoài là một lồng sắt bảo vệ chỉ có một lối ra duy nhất.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102420.jpg)

Khi cai ngục muốn cho phạm nhân của buồng nào ra ngoài, họ sẽ quay trục xoay để cửa buồng đó khớp với lối ra của lồng bảo vệ ngoài. Do cơ chế này chỉ cho phép mở duy nhất một buồng giam tại một thời điểm, nó giúp giảm thiểu tối đa nguy cơ vượt ngục tập thể và tiết kiệm nhân lực canh gác.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102421.jpg)

Đã có 16 nhà tù thuộc kiến trúc này được xây dựng tại Mỹ, nhưng do sự cố kẹt cơ khí thỉnh thoảng xảy ra gây nguy hiểm cho phạm nhân khi có hỏa hoạn, mô hình này đã bị bãi bỏ vào năm 1930. Hiện nay chỉ còn 4 nhà tù được bảo tồn làm bảo tàng tham quan.

2. **Câu chuyện đằng sau thiết kế logo quả táo ngược trên các dòng máy tính PowerBook cổ của Apple**

Trên các thế hệ máy tính xách tay đầu tiên của Apple, logo quả táo khuyết ở mặt lưng máy được thiết kế ngược đầu khi người dùng mở máy lên sử dụng (nhìn từ góc độ người đối diện).

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102503.jpg)

Lý giải cho thiết kế này, các kỹ sư Apple thời đó cho biết họ ưu tiên trải nghiệm của chính chủ sở hữu máy: khi máy tính đang đóng trên bàn, logo quả táo hướng đúng chiều về phía người dùng giúp họ định vị chính xác chiều mở nắp máy mà không bị mở ngược đầu. Steve Jobs thời kỳ đó cũng đồng tình với quan điểm trải nghiệm của người dùng máy quan trọng hơn ánh nhìn của người xung quanh.

Tuy nhiên sau này Steve Jobs đã thay đổi góc nhìn và quyết định xoay ngược lại logo quả táo như hiện nay để đảm bảo tính nhận diện thương hiệu tốt nhất khi người xung quanh quan sát sản phẩm.

## 文摘 (Văn trích)

1. **Cuộc đua công nghệ dệt may thể thao và những tranh cãi pháp lý quanh đôi giày chạy Vaporfly của Nike**

Vào ngày 12/10/2019, vận động viên người Kenya Eliud Kipchoge đã đi vào lịch sử điền kinh thế giới khi hoàn thành cự ly chạy Marathon dưới 2 giờ (chạm mốc 1 giờ 59 phút 40 giây) tại Vienna (Áo) trên chân đôi giày chạy Vaporfly được thiết kế đặc biệt của Nike.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102002.jpg)

Tương tự, kỷ lục marathon thế giới của nữ cũng được xác lập bởi vận động viên sử dụng dòng giày chạy này của Nike. Thống kê chỉ ra trong vòng 13 tháng qua, cả 5 thành tích chạy marathon nhanh nhất lịch sử nhân loại đều được xác lập bởi các vận động viên đi giày Nike Vaporfly. Thực tế này buộc Liên đoàn Điền kinh Quốc tế (World Athletics) phải cân nhắc thành lập ủy ban chuyên môn đánh giá xem liệu công nghệ sản xuất giày chạy của Nike có đang can thiệp quá sâu làm mất đi tính công bằng tự nhiên của môn thể thao này hay không.

Bản chất của cải tiến công nghệ trên đôi giày Vaporfly nằm ở sự kết hợp giữa hai yếu tố: lớp đệm bọt Pebax siêu nhẹ có khả năng hoàn trả năng lượng lên tới 30% (giúp giảm thiểu tối đa sự mỏi cơ của bắp chân ở những km cuối) và một tấm sợi carbon chịu lực dạng cong được luồn bên trong đế giày giúp định hình bàn chân tối ưu khi tiếp đất.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102004.jpg)

Nhiều nghiên cứu khoa học độc lập chỉ ra dòng giày chạy Vaporfly của Nike có thể giúp nâng cao hiệu suất chạy của vận động viên lên tới 3%. Đối với các vận động viên đỉnh cao, con số 3% này là khoảng cách chênh lệch khổng lồ quyết định trực tiếp đến tấm huy chương vàng Olympic. Hiện tại, liên đoàn đang xem xét việc đưa ra các quy định giới hạn độ dày tối đa của đế giày chạy và cấm sử dụng các thiết bị lò xo chịu lực cơ học bên trong đế giày để đảm bảo tính công bằng thể thao cho kỳ thế vận hội Tokyo sắp tới.

## 言论 (Danh ngôn)

1、

> "Nhiều người thường cho rằng người Nhật rất giỏi sao chép công nghệ của các nước khác. Nhưng tôi không nghĩ vậy, những gì người Nhật thực hiện thực chất là quá trình tái phát kiến (reinventing). Họ nghiên cứu sâu sắc các phát minh của người khác cho đến khi thực sự thấu hiểu tường tận bản chất của nó, để rồi từ đó chế tạo ra phiên bản thế hệ thứ hai hoàn thiện và tinh tế hơn rất nhiều so với bản gốc.
> 
> Tuy nhiên, chiến lược này chỉ thực sự phát huy hiệu quả tối đa đối với các ngành công nghiệp có tốc độ thay đổi chậm (như sản xuất thiết bị âm thanh hay ô tô). Còn đối với các ngành công nghiệp công nghệ cao thay đổi chóng mặt hàng ngày, chiến lược này sẽ gặp vô vàn khó khăn bởi khi bạn hoàn thành việc tái phát kiến sau vài năm nghiên cứu, sản phẩm gốc đã sớm bị thị trường đào thải từ lâu."
> 
> -- Steve Jobs (chia sẻ trong cuộc phỏng vấn năm 1985)

(Hết)
