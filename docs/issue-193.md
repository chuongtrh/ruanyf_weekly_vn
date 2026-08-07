# 科技爱好者周刊（第 193 期）：前端与后端，谁更难？

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần. （**[Thông báo] Tuần sau đón Tết Nguyên Đán, bản tin sẽ tạm ngưng phát hành một số và trở lại vào ngày 11 tháng 2.**）

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2139) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012012.webp)

Hội thi Điêu khắc băng chuyên nghiệp toàn quốc lần thứ 41 đã khai mạc vào ngày 6/1 tại Công viên Triệu Lân, thành phố Cáp Nhĩ Tân. Trên mặt hồ đóng băng, các nghệ nhân điêu khắc tỉ mỉ các tác phẩm nghệ thuật của mình. Khi hoàng hôn buông xuống, ánh đèn màu thắp sáng lung linh trên nền tuyết trắng tạo nên một khung cảnh huyền ảo như truyện cổ tích. (Nguồn: [China News](http://news.china.com.cn/2022-01/08/content_77976699.htm))

## 主带话题：Front-end và Back-end, bên nào khó hơn?

Cộng đồng Hacker News là một trong những diễn đàn công nghệ lớn nhất dành cho các lập trình viên trên thế giới. Tôi thường ghé thăm trang này hàng ngày và rất nhiều chủ đề thú vị trong bản tin được trích dẫn từ đây.

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011601.webp)

Gần đây, tôi có đọc được một chủ đề thảo luận thu hút rất nhiều lượt tương tác:

Một lập trình viên Front-end lâu năm (bắt đầu từ năm 2007) chia sẻ rằng anh cảm thấy bế tắc và muốn chuyển hướng sang làm Back-end vì không thể theo kịp tốc độ thay đổi chóng mặt của công nghệ Front-end hiện nay:

> *"Tôi làm phát triển Front-end từ năm 2007. Cho đến nay, có rất nhiều công nghệ mới xuất hiện mà tôi không còn đủ sức làm quen. Mỗi khi mở Chrome DevTools và thấy hàng loạt tính năng mới chưa từng biết, tôi chỉ biết bấm bỏ qua.*
>
> *Nhiều công cụ và tính năng quen thuộc trước đây đều đã hoặc sắp sửa bị khai tử. Toàn bộ quy trình Front-end hiện đại dựa trên môi trường quản lý gói npm luôn phát sinh các lỗi biên dịch khó hiểu trên máy tính cục bộ, ngốn rất nhiều thời gian sửa lỗi cấu hình.*
>
> *Ngay cả những tác vụ đơn giản nhất nay cũng trở nên phức tạp vì phải xử lý quá nhiều trường hợp biên (edge cases). Phạm vi công việc tôi có thể hoàn thành tốt đang thu hẹp dần.*
> 
> *Tôi đã mất hoàn toàn tự tin để tiếp tục làm việc ở mảng Front-end và đang tự hỏi liệu làm Back-end có dễ thở hơn không?"*

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011602.webp)

Đúng như dự đoán, câu hỏi này đã châm ngòi cho một cuộc tranh luận vô cùng sôi nổi với rất nhiều luồng ý kiến khác nhau.

- Một nhóm đồng tình và cho rằng: Front-end ngày nay thực sự đã trở nên cực kỳ phức tạp. Tốc độ thay đổi công nghệ nhanh tới mức việc phát triển và bảo trì mã nguồn Front-end hiện nay đôi khi còn mệt mỏi hơn Back-end rất nhiều.
- Nhóm ngược lại cảnh báo: Back-end cũng không hề đơn giản. Nếu bạn không thể thích nghi tốt với môi trường Node.js thì việc chuyển sang viết mã bằng C++, Java hay Go cũng sẽ là một hành trình đầy gian nan, tuyệt đối không nên quyết định vội vã.

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011603.webp)

Độ khó dễ vốn mang tính chủ quan tùy thuộc vào thế mạnh của mỗi cá nhân, nên cuộc tranh luận này rất khó có được tiếng nói chung. Tuy nhiên, có một nhận định rất đáng chú ý chỉ ra sự khác biệt bản chất giữa hai mảng lập trình:

> *"Vấn đề của Front-end không hẳn là độ khó kỹ thuật, mà là do nó phải đối mặt trực tiếp với người dùng cuối (end-users). Bất kỳ khi nào thị hiếu, hành vi và sở thích của người dùng thay đổi, giao diện Front-end bắt buộc phải lập tức thay đổi để đáp ứng kịp thời.*
> 
> *Điều này buộc công nghệ Front-end phải liên tục cập nhật với tốc độ chóng mặt theo thị hiếu số đông.*
>
> *Ngược lại, Back-end không phải trực tiếp đối diện người dùng mà tập trung giải quyết các bài toán khoa học máy tính kinh điển như cấu trúc dữ liệu và giải thuật - những lý thuyết cốt lõi rất ít khi biến đổi qua nhiều năm, cho phép kế thừa các nghiên cứu cũ ổn định hơn."*

Nhận định này rất chính xác. Sự khác biệt thực tế nằm ở tính chất vấn đề cần giải quyết:

Front-end mang tính biến động, ồn ào và thay đổi liên tục vì đó là đặc tính của tệp người dùng cuối. Nếu bạn là người không thích ứng được với sự hỗn loạn và biến chuyển liên tục của công nghệ, bạn sẽ thấy Front-end rất mệt mỏi.

Back-end tuy ổn định hơn về mặt kiến trúc nhưng đòi hỏi tư duy logic trừu tượng cao, làm việc sâu với cấu trúc phần cứng, lý thuyết biên dịch và tối ưu hóa hệ thống. Việc làm chủ các kiến thức này đòi hỏi sự kiên trì tích lũy lâu dài.

Do đó, việc lựa chọn theo đuổi Front-end hay Back-end bên cạnh cơ hội thị trường cần dựa trên tính cách và sở thích cá nhân của bạn. Nếu bạn là người trầm tính, thích nghiên cứu sâu các lý thuyết trừu tượng, Back-end có thể là điểm đến phù hợp hơn.

Còn bạn thì sao? Bạn thấy Front-end hay Back-end khó hơn? Nếu được chọn lại từ đầu, bạn sẽ đi theo hướng đi nào?

## 给孩子的财经小课

Nhiều độc giả của bản tin đã làm cha mẹ và có con nhỏ.

Trẻ nhỏ có một đặc điểm là rất tò mò và thích đặt câu hỏi. Những câu hỏi về khoa học tự nhiên hay vũ trụ có thể dễ dàng giải đáp qua sách giáo khoa, nhưng những câu hỏi liên quan đến vận hành kinh tế và xã hội thường khiến các bậc phụ huynh bối rối.

Ví dụ như các câu hỏi thực tế dưới đây của trẻ nhỏ:

> - Tại sao lại có quy định về mức lương tối thiểu?
> - Tại sao rạp chiếu phim nào cũng bán bắp rang bơ?
> - Trở thành tuyển thủ eSports chơi game cũng kiếm được tiền phải không?
> - Nếu nhà nước in thật nhiều tiền, mọi người có giàu lên không?

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011501.webp)

Tuần này giới thiệu tới các bạn một chương trình âm thanh hữu ích mang tên **《Finance and Economics Course for Kids》** thiết kế riêng cho học sinh tiểu học và trung học cơ sở giúp giải đáp các thắc mắc thực tế về kinh tế xã hội xung quanh đời sống:

Chương trình được dẫn dắt bởi chuyên gia tài chính Sun Mingzhan. Tốt nghiệp Đại học Trung Sơn, ông từng giữ chức vụ quản lý tại các tập đoàn bảo hiểm thuộc Fortune 500 trước khi sáng lập doanh nghiệp tư vấn tài chính riêng.

Là người cha của hai đứa con (12 tuổi và 6 tuổi), ông thường xuyên phải giải đáp các thắc mắc của con trai lớn về tiền bạc và kinh tế. Ý tưởng thu âm các buổi trò chuyện này thành một chương trình podcast dành cho trẻ em đã ra đời từ đó:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011502.webp)

Chương trình bắt đầu thu âm từ năm 2020 và duy trì phát sóng đều đặn hàng tuần. Rất nhiều phụ huynh phản hồi rằng chính họ cũng học hỏi được nhiều kiến thức tài chính bổ ích khi cùng nghe với con mình. Dưới đây là mục lục các chủ đề học của mùa 2:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011503.webp)

Khóa học giúp các bạn nhỏ hình thành tư duy tài chính lành mạnh thông qua các hiện tượng thực tế gần gũi. Phụ huynh quan tâm có thể truy cập [nền tảng Feimooc](https://www.feimooc.com/user/1255718) (khuyên dùng máy tính để bàn) để nghe thử miễn phí 20 chương đầu tiên của mùa 1 và mùa 2.

Độc giả bản tin đăng ký trọn gói mùa 2 sẽ được nhận mức giá ưu đãi chỉ **69 NDT** (giá gốc 199 NDT):

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011504.webp)

Gói đăng ký bao gồm toàn bộ 52 chương bài giảng của mùa 2 (thời lượng 10-20 phút/chương), 4 buổi học livestream tương tác trực tiếp với giảng viên. Khách hàng đăng ký sẽ được tặng kèm miễn phí 55 chương bài giảng của mùa 1 và một cuốn sách giáo dục tài chính trẻ em chất lượng cao.

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011715.webp)

Bạn đọc có thể quét mã QR trên đây hoặc bấm trực tiếp vào [liên kết đăng ký khóa học](http://m.feimooc.com/courseDetail/824?sencecode=fei_7125&spreadType=teacherCopy) để tham gia học thử. Sau khi thanh toán thành công, vui lòng kết nối với trợ lý khóa học để nhận trọn bộ quà tặng đính kèm.

## 科技动态

1、[Nữ nghệ sĩ piano lớn tuổi nhất thế giới chuẩn bị ra mắt album nhạc mới ở tuổi 97](https://www.bbc.com/news/entertainment-arts-59986543)

Nữ nghệ sĩ piano nổi tiếng người Mỹ Ruth Slenczynska chuẩn bị phát hành album âm nhạc mới vào ngày 18/3 tới ở tuổi 97, lập kỷ lục thế giới mới về người lớn tuổi nhất phát hành album chuyên nghiệp:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011807.webp)

Bà vốn là một thần đồng âm nhạc nổi tiếng từ khi mới 4 tuổi. Đoạn video ghi lại buổi biểu diễn piano trên sân khấu của bà ở tuổi lên 5 quay vào năm 1930 vẫn đang được lưu trữ trên [YouTube](https://www.youtube.com/watch?v=SPZiuPw-LLs). Điều này đồng nghĩa với việc bà có thể là người còn sống duy nhất hiện nay xuất hiện trong một video tư liệu lâu đời nhất lịch sử (92 năm trước):

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011808.webp)

2、[Hà Lan thử nghiệm mô hình khu dân cư nổi Schoomschip thích ứng biến đổi khí hậu](https://www.archdaily.com/964050/amsterdams-floating-neighbourhood-schoonschip-offers-a-new-perspective-on-circularity-and-resiliency)

Là quốc gia có phần lớn diện tích nằm dưới mực nước biển, Hà Lan thường xuyên phải đối mặt với tình trạng ngập lụt nghiêm trọng. Các kiến trúc sư nước này đang thử nghiệm mô hình xây dựng nhà ở nổi trên mặt nước:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120801.webp)

Họ đã thiết lập một khu dân cư gồm 46 căn hộ nổi trên hệ thống kênh rạch của thủ đô Amsterdam. Các căn nhà được neo cố định vào cột thép ngầm và có khả năng tự động trượt lên xuống theo mực nước thủy triều dâng, giúp loại bỏ hoàn toàn nguy cơ ngập lụt:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120802.webp)

Mỗi căn hộ nổi đều được trang bị hệ thống lọc nước thải sinh hoạt cục bộ, pin năng lượng mặt trời áp mái và kết nối với bờ qua hệ thống cầu phao di động linh hoạt:

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120804.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120803.webp)

3、[Đại học Yale phát triển cảm biến đeo kẹp áo Fresh Air Clip phát hiện sớm virus](https://www.ifanr.com/1466653)

Phương pháp xét nghiệm PCR hiện nay yêu cầu người dùng phải chủ động đi test, dẫn tới việc khó phát hiện sớm các trường hợp phơi nhiễm virus corona thụ động ngoài cộng đồng. Nhóm nghiên cứu thuộc Đại học Yale đã phát triển một thiết bị cảm biến đeo nhỏ gọn mang tên **Fresh Air Clip**:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011701.webp)

Thiết bị dạng kẹp ghim nhỏ có thể gắn trực tiếp lên cổ áo khi di chuyển ngoài đường. Cảm biến tích hợp màng lọc Polymer đặc biệt hỗ trợ hấp phụ và lưu giữ các hạt virus bay lơ lửng trong không khí xung quanh:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011702.webp)

Sau khi trở về, người dùng chỉ cần gửi thiết bị tới phòng lab để phân tích xem có dấu vết của virus hay không, từ đó xác định xem lộ trình di chuyển trong ngày có đi qua vùng dịch tễ nguy cơ cao hay không.

4、[Trung Quốc chế tạo robot bốn chân cơ khí mô phỏng dã thú YAK khổng lồ](https://finance.sina.com.cn/jjxw/2022-01-14/doc-ikyakumy0382310.shtml)

Đơn vị chế tạo cơ khí quân sự trong nước vừa công bố chế tạo thành công mẫu robot bốn chân chạy bằng động cơ điện mô phỏng hình dạng dã thú Tây Tạng "YAK":

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011710.webp)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012101.webp)

Robot có khả năng di chuyển với vận tốc 10 km/h trên địa hình đồi núi phức tạp, chịu được tải trọng hành lý nặng tới 160 kg. Đây hiện là mẫu robot bốn chân chạy điện có kích thước và tải trọng lớn nhất thế giới, phục vụ đắc lực cho công tác vận tải nhu yếu phẩm lên các chốt biên phòng vùng cao hoặc do thám địa hình hiểm trở:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011711.webp)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011712.webp)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011714.webp)

5、[Nhật Bản thử nghiệm thành công đường truyền dẫn điện siêu dẫn nitơ lỏng thực tế](https://cn.nikkei.com/industry/scienceatechnology/47301-2022-01-13-02-19-33.html)

Nhật Bản vừa triển khai vận hành thử nghiệm tuyến cáp truyền tải điện ứng dụng công nghệ siêu dẫn (Superconductivity) dài nhất thế giới tại tỉnh Miyazaki:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011311.webp)

Tuyến cáp được thiết kế với ống dẫn cách nhiệt bọc ngoài chứa đầy dung dịch nitơ lỏng nhiệt độ cực thấp để làm mát dây dẫn siêu dẫn bên trong. Hiện tượng siêu dẫn giúp triệt tiêu hoàn toàn điện trở vật lý trên đường dây, loại bỏ hao hụt điện năng tỏa nhiệt trên đường truyền tải đường dài. Việc chế tạo thành công vật liệu siêu dẫn ở nhiệt độ nitơ lỏng (khoảng -196 độ C) thay vì helium lỏng đắt đỏ (-269 độ C) đã giúp giảm 90% chi phí vận hành, mở ra triển vọng thương mại hóa diện rộng công nghệ này. (Đóng góp của [@wingor](https://github.com/ruanyf/weekly/issues/2162))

## 文章

1、[Hành trình phát hiện cây óc chó cổ đại lớn nhất Trung Quốc dã sinh](https://mp.weixin.qq.com/s/QRiraXxdswb333H0ULA3ng)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011814.webp)

Bài viết ghi lại hành trình khảo sát thực địa của một nhóm nghiên cứu sinh tại tỉnh Vân Nam phát hiện cây quả óc chó dã sinh có chiều cao kỷ lục hơn 40 mét, đường kính thân rộng gần 2 mét và tuổi đời được xác định trên 300 năm tuổi.

2、[Chia sẻ kinh nghiệm khởi nghiệp của nhà thiết kế phông chữ chữ Hán](https://mp.weixin.qq.com/s/hZ6KeQCFzyWbQw_J1fDjug)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011816.webp)

Tác giả chia sẻ cơ duyên từ một lập trình viên có niềm đam mê với nghệ thuật kiểu chữ đã tự học vẽ vector và xây dựng doanh nghiệp cung cấp phông chữ (font foundry) thiết kế thương mại thành công.

3、[Báo cáo hiện trạng tài nguyên rừng toàn cầu năm 2020 của FAO](https://www.fao.org/forest-resources-assessment/2020/zh)（Tiếng Trung）

Báo cáo phân tích dữ liệu lâm nghiệp chính thức từ Tổ chức Lương thực và Nông nghiệp Liên Hợp Quốc (FAO) được thể hiện bằng giao diện web đồ họa tương tác trực quan rất trực quan và chuyên nghiệp.

4. [Thế nào là tái cấu trúc phần mềm (Refactoring)?](https://understandlegacycode.com/blog/refactoring-and-defactoring/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122013.webp)

Bài review chia sẻ góc nhìn sau khi đọc cuốn sách kinh điển *Refactoring* của tác giả Martin Fowler: định nghĩa chuẩn xác về quy trình cải tiến cấu trúc code bên trong để dễ bảo trì hơn mà tuyệt đối không được làm thay đổi tính năng đầu ra hiện có.

5、[Giới thiệu thư viện quản lý thời gian Temporal API mới của JavaScript](https://blog.openreplay.com/is-it-time-for-the-javascript-temporal-api)（Tiếng Anh）

Giới thiệu dự án phát triển thư viện chuẩn quản lý ngày tháng thế hệ mới `Temporal` của JavaScript nhằm thay thế hoàn toàn đối tượng `Date` vốn tồn tại nhiều lỗi thiết kế lịch sử phức tạp.

6、[Hướng dẫn lập trình thuật toán mã hóa RSA cơ bản bằng Python](https://coderoasis.com/implementing-rsa-from-scratch-in-python/)（Tiếng Anh）

Bài hướng dẫn ngắn gọn giúp lập trình viên hiểu rõ bản chất toán học đằng sau giải thuật mã hóa bất đối xứng RSA thông qua các dòng code Python đơn giản.

7、[Sử dụng tính năng Recorder ghi thao tác người dùng trên Chrome DevTools](https://developer.chrome.com/docs/devtools/recorder/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120204.webp)

Chrome vừa cập nhật công cụ Recorder trong DevTools hỗ trợ tự động ghi lại toàn bộ hành vi click, gõ phím của người dùng trên trang web để xuất ra file kịch bản chạy thử tự động cho Puppeteer.

8、[Tổng quan cơ bản về lý thuyết hàng đợi (Queue Theory) trong lập trình](https://thenewstack.io/an-introduction-to-queue-theory-why-disaster-happens-at-the-edges/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111507.jpg)

Hầu hết các bài toán nghẽn cổ chai trong hệ thống đều là bài toán hàng đợi (queue). Bài viết giới thiệu các khái niệm cơ bản về lý thuyết hàng đợi giúp lập trình viên tối ưu hóa bộ nhớ đệm (caching) và xử lý bất đồng bộ.

## 工具

1、[MockingBird: Dự án clone giọng nói tiếng Trung siêu tốc](https://github.com/babysor/MockingBird)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122803.webp)

Ứng dụng trí tuệ nhân tạo nguồn mở hỗ trợ phân tích mẫu ghi âm giọng nói chỉ dài 5 giây để học tông giọng và tự động phát âm đọc bất kỳ đoạn văn bản tiếng Trung nào bằng chính giọng nói đó.

2、[Redirector: Tiện ích tự động chuyển hướng URL theo biểu thức chính quy](https://github.com/einaregilsson/Redirector)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122501.webp)

Extension trình duyệt cực kỳ hữu ích cho phép lập trình viên thiết lập các cấu hình quy tắc regex để tự động chuyển hướng các trang web đích (như tự động nhảy từ link di động sang giao diện desktop tương ứng).

3、[Imagor: Máy chủ tối ưu hóa và sinh ảnh thu nhỏ viết bằng Go](https://github.com/cshum/imagor)

Bộ mã nguồn máy chủ xử lý ảnh gọn nhẹ hiệu năng cao, hỗ trợ tự động cắt cúp, nén dung lượng và sinh ảnh thu nhỏ (thumbnails) nhanh chóng thông qua tham số URL.

4、[Gatsby: Nền tảng video chia sẻ P2P hoạt động trên mạng IPFS](https://gatsby.video/)

![](https://cdn.beekka.com/blogimg/asset/202110/bg2021101101.jpg)

Dự án phát triển nền tảng phát video phi tập trung hoạt động dựa trên cơ sở dữ liệu phân tán IPFS giúp giảm thiểu sự phụ thuộc vào máy chủ trung tâm.

5、[CheerpX's REPL: Trình chạy thử code đa ngôn ngữ trực tuyến](https://repl.leaningtech.com/)

Trang web cung cấp môi trường chạy thử code dòng lệnh (REPL) trực tiếp trên trình duyệt hỗ trợ 5 ngôn ngữ lập trình phổ biến bao gồm Python, Ruby, NodeJS, Lua và C++.

6、[emojimix: Tiện ích ghép nối hai hình vẽ Emoji tự động](https://tikolu.net/emojimix/)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112304.jpg)

Trang web giải trí thú vị hỗ trợ người dùng lựa chọn hai hình vẽ Emoji bất kỳ để thuật toán tự động kết hợp chúng lại thành một biểu tượng đồ họa Emoji mới rất hài hước.

7、[Tesla Light Show: Mã nguồn lập trình trình diễn đèn xe điện Tesla](https://github.com/teslamotors/light-show)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122505.webp)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122504.webp)

Dự án chính thức được chia sẻ bởi Tesla hỗ trợ người dùng tự biên soạn kịch bản nháy đèn pha và đèn xi-nhan đồng bộ với nhạc thông qua phần mềm chỉnh nhạc xlights để nạp vào xe biểu diễn.

8、[FakeYou: Công cụ chuyển đổi văn bản sang giọng nói của người nổi tiếng](https://fakeyou.com/)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122602.webp)

Ứng dụng web chuyển đổi Text-to-Speech hỗ trợ mô phỏng giọng đọc tiếng Anh của hơn 80 chính trị gia và nhân vật phim hoạt hình nổi tiếng thế giới.

9、[Jodd: Bộ công cụ mở rộng tối giản hỗ trợ lập trình Java](https://jodd.org/)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011804.webp)

Thư viện Java gọn nhẹ chưa đầy 1.7MB bổ sung nhiều hàm tiện ích hỗ trợ xử lý chuỗi, định dạng thời gian và gỡ lỗi tối ưu thay thế cho các hàm mặc định của JDK.

## 资源

1、[Video Game Vending Machines: Kho thiết kế máy bán nước tự động trong game](https://vgsmproject.com/)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121115.webp)

Trang web tổng hợp hình vẽ thiết kế của các máy bán nước tự động xuất hiện trong bối cảnh các tựa game nổi tiếng như Fortnite, Fallout.

2、[Windows Control Panel Evolution: Lịch sử thay đổi giao diện Control Panel](https://www.versionmuseum.com/history-of/all-windows-control-panels)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121801.webp)

Chuyên trang tổng hợp ảnh chụp màn hình giao diện bảng điều khiển cấu hình hệ thống Control Panel của Windows qua các thế hệ từ bản Windows 1.0 sơ khai đến bản Windows 10 hiện đại.

3、[ihavenotv.com: Thư viện phim tài liệu khoa học tiếng Anh miễn phí](https://ihavenotv.com/)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111506.jpg)

Trang web tổng hợp liên kết xem trực tuyến hơn 3.500 bộ phim tài liệu khoa học, lịch sử và thiên văn học chất lượng cao (phụ đề tiếng Anh).

4、[Blockchain Engineer Roadmap (Tài liệu tự học phát triển Blockchain)](https://betterprogramming.pub/how-to-become-a-blockchain-engineer-fa4386a0504f)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021121802.webp)

Bản danh sách tổng hợp lộ trình học tập và các liên kết tài liệu tiếng Anh hướng dẫn tự học phát triển ứng dụng phi tập trung Web3.

5、[12 Books Every Software Engineer Should Read](https://medium.com/@iamjwr/software-engineer-roadmap-via-books-a6aabdc2589c)

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021122005.webp)

Tác giả chia sẻ danh sách tuyển chọn 12 cuốn sách chuyên ngành CNTT kinh điển về tư duy viết mã sạch và thiết kế hệ thống phần mềm khuyên đọc cho các lập trình viên.

## 图片和视频

1、[Mẫu tòa nhà gỗ tái chế 700 ô cửa sổ cũ tại Nhật Bản](https://www.nakam.info/jp/works/kamikatsu0/)

Nhà máy xử lý rác thải tái chế tại thị trấn Kamikatsu, Tokushima Nhật Bản được dựng hoàn toàn bằng khung gỗ tự nhiên địa phương kết hợp với hơn 700 khung cửa sổ kính cũ thu gom từ các ngôi nhà cổ bị tháo dỡ:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111301.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111305.jpg)

Mặt sàn công trình cũng tái sử dụng các mảnh gốm và thủy tinh tái chế ép keo tạo nên điểm nhấn kiến trúc xanh độc đáo:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111302.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111303.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111306.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021111307.jpg)

2、[eboy Pixoramas: Tranh pixel nghệ thuật đô thị tương lai độc đáo](https://hello.eboy.com/pool/~Pixorama/1?q=project)

eboy là nhóm nghệ sĩ đồ họa nổi tiếng thế giới với phong cách vẽ tranh pixel chi tiết. Tác phẩm mô phỏng đô thị tương lai rực rỡ sắc màu được thiết kế tỉ mỉ trong vòng 6-8 tuần:

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112106.jpg)

![](https://cdn.beekka.com/blogimg/asset/202111/bg2021112104.jpg)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012102.webp)

3、[Samsung giới thiệu các nguyên mẫu màn hình gập OLED thế hệ mới tại CES 2022](https://www.youtube.com/watch?v=P0wL65A3Iyo&ab_channel=CNET)

Xem video giới thiệu 1 phút các mẫu màn hình dẻo OLED tự cuộn và gập 3 khúc độc đáo đang được Samsung phát triển thử nghiệm:

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=t3318axh68i" allowFullScreen="true" width="600" height="400"></iframe>

## Bài đọc thêm

### Độc quyền tốt và độc quyền xấu theo định nghĩa của Peter Thiel

Trong cuốn sách kinh điển *Zero to One* (Từ không đến một), nhà đầu tư Peter Thiel phân loại sự độc quyền trên thị trường thành hai trạng thái đối lập:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012013.webp)

- **Độc quyền xấu (Bad Monopoly):** Đạt được trạng thái độc quyền nhờ các thủ đoạn phi pháp chèn ép đối thủ cạnh tranh, cản trở phát triển chung. Đây là hành vi cần bị pháp luật chống độc quyền xử lý nghiêm ngặt.
- **Độc quyền tốt/Độc quyền tự nhiên (Good/Natural Monopoly):** Đạt được vị thế thống trị thị trường nhờ tự phát triển được sản phẩm ưu việt vượt trội hoàn toàn so với đối thủ cạnh tranh, được người dùng tự nguyện tin dùng.

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012014.webp)

Peter Thiel phân tích rằng trong một thị trường cạnh tranh hoàn hảo, biên lợi nhuận của các doanh nghiệp sẽ bị kéo tụt dần về mốc bằng không. Để sống sót, các hãng bắt buộc phải giảm thiểu chi phí bằng cách dìm lương công nhân, cắt giảm tối đa chi phí nghiên cứu phát triển (R&D) và giảm chất lượng nguyên liệu. Điều này cản trở sự đổi mới sáng tạo chung của xã hội.

Ngược lại, khi một doanh nghiệp đạt được độc quyền tự nhiên nhờ sản phẩm xuất sắc, họ sẽ không còn lo sợ bị dìm giá bởi đối thủ. Nguồn thặng dư khổng lồ thu được sẽ giúp doanh nghiệp nâng cao đáng kể mức lương cho kỹ sư, đầu tư mạnh mẽ vào R&D sản phẩm thế hệ mới và quan tâm hơn tới các nghĩa vụ môi trường xã hội. Đối với khách hàng, họ không hề bị giới hạn lựa chọn, trái lại còn được tiếp cận các đột phá công nghệ mới chất lượng cao hơn.

## 言论

1\.

Với việc tải trọng của các tên lửa thế hệ mới ngày càng lớn, tần suất phóng tăng cao và chi phí phóng giảm sâu, ngành nghiên cứu vũ trụ đang bước sang kỷ nguyên mới cho phép đưa các thiết bị quan sát thiên văn khổng lồ trực tiếp lên không gian dễ dàng.

-- Trích bài viết "NASA is on the cusp of a new era"

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120918.webp)

2\.

Thống kê cho thấy trong số 101 phát hiện về liệu pháp y học hoặc thuốc mới được công bố trên các tạp chí khoa học danh tiếng giai đoạn 1979-1983, 10 năm sau đó chỉ có 5 nghiên cứu được thương mại hóa thành công. Và 20 năm sau (năm 2003) chỉ còn duy nhất 1 loại thuốc được ứng dụng lâm sàng rộng rãi. Độc giả nên giữ sự thận trọng trước các tin tức giật gân về đột phá y tế mới vì tỷ lệ thành công thực tế của chúng là rất nhỏ.

-- Theo Vox.com

## 历史上的本周

- 2021年（第 142 期）：[Thảo luận triết học: Năm 2020 mới thực sự là năm khởi đầu của thế kỷ 21](https://www.ruanyifeng.com/blog/2021/01/weekly-issue-142.html)
- 2020年（第 90 期）：[Phân tích sự khác biệt bản chất giữa kỹ năng quản trị nhân sự và năng lực kỹ thuật của lập trình viên](https://www.ruanyifeng.com/blog/2020/01/weekly-issue-90.html)
- 2019年（第 39 期）：[Phân tích nội dung hai bức thư ngỏ nổi tiếng của ban lãnh đạo tập đoàn Apple gửi khách hàng](https://www.ruanyifeng.com/blog/2019/01/weekly-issue-39.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
