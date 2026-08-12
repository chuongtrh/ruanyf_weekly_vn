# Bản tin chia sẻ công nghệ (Số 248): Đừng thổi phồng quá mức ChatGPT

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3022) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032108.webp)

Bức ảnh đoạt giải tại cuộc thi Nhiếp ảnh Thiên nhiên Thế giới năm 2022 ghi lại khoảnh khắc một chú chim cắt lưng hung đang làm tổ ngay bên trong một chiếc đèn đường rỉ sét tại thành phố Stara Zagora, miền trung Bulgaria. Hình ảnh này gợi liên tưởng sâu sắc đến hoàn cảnh sinh tồn chật vật của nhiều người lao động tại các đô thị lớn hiện nay. (Nguồn: [NiceNews](https://nicenews.com/environment/2022-world-nature-photography-awards/))

## 本周话题：不要夸大 ChatGPT

Chỉ mới ra mắt công chúng được vài tháng, nhưng các bạn có nhận thấy những luồng dư luận xung quanh ChatGPT đang ngày càng được đẩy lên mức cường điệu quá mức hay không?

Sự kinh ngạc và tán thưởng ban đầu của công chúng đang dần chuyển dịch thành những lời tâng bốc thiếu lý trí. Nhiều người quả quyết khẳng định rằng ChatGPT chắc chắn sẽ định hình lại toàn bộ cấu trúc xã hội loài người.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032804.webp)

Ví dụ như tạp chí danh tiếng [*The Economist*](https://redian.news/wxnews/269433) nhận định công nghệ này mang tính "xoay chuyển càn khôn":

> “Thuật ngữ GPT hoàn toàn có thể hiểu theo một nghĩa khác là General-Purpose Technology (Công nghệ đa dụng) – một cuộc cách mạng công nghệ mang tính chất xoay chuyển càn khôn, giúp nâng cao vượt bậc năng suất lao động cho mọi ngành nghề tương tự như động cơ hơi nước, điện năng và máy tính cá nhân trước đây.”

Một tác giả trong nước cũng [nhận định](https://www.163.com/dy/article/I0OFPKOV05561KQ6.html) nó sẽ "quét sạch tất cả":

> “Cơn bão do ChatGPT tạo ra đang càn quét mọi ngóc ngách.
> 
> Với tốc độ cải tiến công nghệ chóng mặt hiện tại, chúng ta hoàn toàn có thể dự đoán rằng trong tương lai, các mô hình AI dạng GPT này sẽ có khả năng thay thế nhân sự ở hầu hết các ngành nghề!”

Một số bài viết khác lại gieo rắc nỗi lo sợ về việc AI sẽ đào thải loài người với những tiêu đề giật gân kiểu: *“Trong kỷ nguyên AI bùng nổ, con người liệu có còn giá trị sinh tồn?”*.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032802.webp)

Trên mạng xã hội Weibo, danh sách các bài viết xu hướng cũng tràn ngập nỗi sợ hãi và lo âu về tương lai nghề nghiệp:

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032801.webp)

Sự lo ngại này nhanh chóng phản chiếu lên thị trường tài chính, tạo nên làn sóng đầu cơ thổi giá điên cuồng các mã cổ phiếu gắn mác "ChatGPT". Mã cổ phiếu của Hanwang Technology – một doanh nghiệp vốn hoạt động kém hiệu quả và liên tục báo lỗ – đã bị thổi giá từ mức 11 nhân dân tệ lên tới 40 nhân dân tệ chỉ trong thời gian ngắn sau khi ChatGPT ra mắt.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032803.webp)

Tôi cảm giác ChatGPT đang dần bị thần thánh hóa như một thực thể vạn năng có thể giải quyết mọi bài toán của nhân loại.

Quan điểm của tôi về vấn đề này là: **ChatGPT thực sự là một công cụ công nghệ rất kỳ diệu, một bước đột phá mang tính thời đại, nhưng chúng ta tuyệt đối không nên thổi phồng nó quá mức.**

ChatGPT vẫn tồn tại những giới hạn vật lý và logic cố hữu mà nó không bao giờ vượt qua được. Nhận định cho rằng ChatGPT đánh dấu "thời điểm bước ngoặt" (singularity) khi máy móc chính thức thay thế hoàn toàn trí tuệ con người là hoàn toàn sai lầm.

Những người ủng hộ quan điểm này đã bỏ qua một sự thật cốt lõi: **ChatGPT không phải là Trí tuệ nhân tạo tổng hợp (AGI), nó đơn thuần chỉ là một Mô hình ngôn ngữ lớn (LLM).**

Trí tuệ nhân tạo tổng hợp (Artificial General Intelligence - AGI) là mục tiêu tối thượng của giới nghiên cứu AI – nhằm tạo ra một cỗ máy có khả năng tư duy suy luận, phân tích đa chiều toàn diện giống hệt con người. Nếu công nghệ này thực sự ra đời, con người mới cần phải lo lắng về vị thế của mình.

Tuy nhiên, ChatGPT không phải là AGI mà là một LLM (Large Language Model - Mô hình ngôn ngữ lớn). Đúng như tên gọi "mô hình ngôn ngữ", nó chỉ được thiết kế để xử lý dữ liệu dạng ngôn từ ký tự (hoặc hệ thống ký hiệu quy ước), phân tích các quy luật thống kê xuất hiện của các từ ngữ để từ đó tự động sinh ra nội dung phù hợp theo gợi ý (prompt).

Điều này đồng nghĩa với việc **ChatGPT chỉ hoạt động hiệu quả trong các lĩnh vực đã được chuẩn hóa thành các hệ thống ký tự ghi chép.** Điều này dẫn đến hai giới hạn chí mạng:

1. **Vô dụng trước các khía cạnh phi ký tự**: Những khía cạnh tư duy không thể diễn đạt hoặc ghi lại bằng ký hiệu chữ viết như thế giới nội tâm phức tạp, trạng thái tiềm thức, linh cảm nghệ thuật hay những khoảnh khắc giác ngộ đột phá của con người là điều nằm ngoài khả năng mô phỏng của ChatGPT.
2. **Không thể tạo ra tri thức hoàn toàn mới vượt ngoài tập dữ liệu huấn luyện**: ChatGPT bắt buộc phải sử dụng kho tài liệu chữ viết có sẵn của nhân loại làm dữ liệu huấn luyện để tìm ra quy luật thống kê. Do đó, nó không thể tự sinh ra những tri thức vượt quá tầm hiểu biết hiện tại của con người.

Ví dụ cụ thể: **ChatGPT không thể tự mình chứng minh các giả thuyết toán học chưa có lời giải, cũng như không thể tự phát minh ra các định luật vật lý mới chưa từng được khám phá.**

Ngay cả khi chúng ta nạp toàn bộ các bài báo nghiên cứu toán học trong lịch sử nhân loại vào tập dữ liệu huấn luyện, ChatGPT cũng không thể tự chứng minh được Giả thuyết Riemann. Bởi vì kho tài liệu đó chỉ dạy cho AI các phương pháp chứng minh đã biết, trong khi việc giải quyết Giả thuyết Riemann đòi hỏi một phương pháp tư duy hoàn toàn mới chưa từng tồn tại.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032805.webp)

Công nghệ cốt lõi của ChatGPT là kiến trúc GPT (Generative Pre-trained Transformer). Tất cả các mô hình AI dựa trên kiến trúc này đều gặp chung một giới hạn: **chúng chỉ có khả năng học hỏi và tái hiện các khuôn mẫu (patterns) đã biết, chứ không thể tự tạo ra các khuôn mẫu hoàn toàn mới.**

Do đó, những phát kiến mang tính đột phá khai thiên lập địa vẫn bắt buộc phải dựa vào trí tuệ sáng tạo của con người.

Hơn nữa, về mặt logic còn tồn tại một nghịch lý: Nếu ChatGPT thực sự mạnh mẽ đến mức "quét sạch tất cả" và thay thế con người viết phần lớn các tài liệu văn bản trong tương lai, thì điều này sẽ trực tiếp dẫn đến sự suy tàn của chính nó. Bởi khi đó, lấy đâu ra nguồn tác phẩm mới do chính con người sáng tạo để tiếp tục làm dữ liệu huấn luyện chất lượng cao cho các thế hệ AI tiếp theo? AI chỉ có thể mô phỏng trí tuệ con người khi được học từ các sản phẩm tư duy nguyên bản của con người.

Tóm lại, ChatGPT là một công cụ mang tính cách mạng, đặt ra thách thức lớn đối với những công việc mang tính chất lặp đi lặp lại hoặc làm việc theo khuôn mẫu sẵn có của con người.

Tuy nhiên, cuộc sống của con người vẫn chứa đựng rất nhiều khía cạnh phi khuôn mẫu, đặc biệt là năng lực tư duy sáng tạo đột phá. ChatGPT không thể chạm tới thế giới sáng tạo này, do đó chúng ta không nên phóng đại quá mức tầm ảnh hưởng của nó đối với tương lai xã hội.

## 活动

**1、Hội thảo Khoa học về Công nghệ AIGC và Ứng dụng Sáng tạo**

Chương trình "Juejin City Salon - Beijing" quy tụ các chuyên gia và kỹ sư AI hàng đầu đến từ ByteDance, Intel, Google và Đại học Thanh Hoa nhằm chia sẻ các chủ đề học thuật chuyên sâu về Trí tuệ nhân tạo tạo sinh (AIGC), bao gồm nguyên lý vận hành của các mô hình lớn, phương pháp huấn luyện và xu hướng chuyển đổi công nghệ trong tương lai.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023033003.webp)

* Thời gian: Chiều ngày 13 tháng 4.
* Địa điểm: Trung tâm Thời trang Phương Hằng (cạnh ga tàu điện ngầm Dazhongsi, Bắc Kinh). Do số lượng chỗ ngồi trực tiếp giới hạn, bạn đọc quan tâm có thể quét mã QR phía trên để đăng ký tham gia trực tiếp hoặc đăng ký xem truyền hình trực tuyến.

**2、[Hội thảo kỹ thuật: Khám phá hạ tầng công nghệ Android của Douyin](https://www.bagevent.com/event/8426971?bag_track=001)**

ByteDance Technical Salon tổ chức buổi chia sẻ kỹ thuật với sự tham gia của 5 kiến trúc sư trưởng từ đội ngũ phát triển Android của ứng dụng Douyin (TikTok bản Trung Quốc) để giao lưu về các kinh nghiệm lập trình thực tế:

* Giải pháp tối ưu dung lượng gói cài đặt (APK size) cho ứng dụng Douyin.
* Kiến trúc xây dựng nền tảng giám sát hiệu năng khởi động của ứng dụng.
* Các nghiên cứu và thực tế tối ưu độ mượt mà (smoothness) khi cuộn màn hình.
* Ứng dụng phân tích mã nguồn tĩnh (static code analysis) trong việc cải thiện trải nghiệm người dùng.
* Quy trình phát triển nền tảng phòng chống suy giảm hiệu năng cho ứng dụng.

* Thời gian: Chiều ngày 15 tháng 4. Bạn đọc có thể quét mã QR bên dưới hoặc [nhấp vào liên kết](https://www.bagevent.com/event/8426971?bag_track=001) để đăng ký nhận vé xem phát sóng trực tiếp miễn phí.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023033001.webp)

Cả hai sự kiện trên đều có các chương trình bốc thăm trúng thưởng nhiều phần quà công nghệ hấp dẫn dành cho người tham gia.

## 科技动态

1、[Ý tưởng xây dựng nhà máy nuôi dưỡng thai nhi bằng tử cung nhân tạo](https://thenextweb.com/news/berlin-scientist-solution-population-decline-artificial-wombs)

Trước thực trạng tỷ lệ sinh liên tục sụt giảm tại các quốc gia châu Âu, một nhà khoa học đã đề xuất mô hình giải pháp độc đáo: xây dựng hệ thống nhà máy nuôi dưỡng thai nhi bằng tử cung nhân tạo đầu tiên trên thế giới mang tên EctoLife:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122002.webp)

Theo bản thiết kế ý tưởng, tổ hợp nhà máy này sẽ bao gồm 75 phòng thí nghiệm hiện đại, mỗi phòng trang bị tối đa 400 buồng nuôi cấy thai nhi (growth pods), ước tính có thể nuôi dưỡng hoàn chỉnh hơn 30.000 trẻ sơ sinh mỗi năm.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122003.webp)

Các buồng nuôi cấy được tích hợp hệ thống cảm biến theo dõi chỉ số sinh tồn 24/7 và đồng bộ dữ liệu thời gian thực tới ứng dụng di động của cha mẹ. Cha mẹ có thể quan sát hình ảnh phát triển độ nét cao của thai nhi, trò chuyện với con qua hệ thống loa tích hợp hoặc mặc áo phản hồi xúc giác để cảm nhận các cử động đạp của em bé.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122004.webp)

Mỗi buồng nuôi cấy kết nối với hai hệ thống ống dẫn: một ống chuyên bơm chất dinh dưỡng và oxy trực tiếp vào dây rốn nhân tạo, ống còn lại đảm nhận nhiệm vụ xử lý và đào thải các chất thải sinh học của thai nhi ra ngoài. Sau khi thai nhi phát triển đủ tháng, buồng nuôi cấy sẽ được mở ra để bàn giao em bé cho cha mẹ.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122005.webp)

2、[Hiện tượng gấu đen không còn ngủ đông tại vùng du lịch hồ Tahoe](https://www.tahoedailytribune.com/news/with-food-available-many-bears-at-tahoe-forgo-hibernation/)

Khu vực hồ Tahoe (Mỹ) là địa điểm du lịch nổi tiếng đồng thời là vùng sinh sống tự nhiên của loài gấu đen hoang dã. Trong mùa đông năm nay, nhiều cư dân địa phương bất ngờ ghi nhận hình ảnh những chú gấu đen vẫn đi lang thang kiếm ăn xung quanh khu dân cư mà không hề ngủ đông như tập tính tự nhiên.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122011.webp)

Tập tính ngủ đông của loài gấu thực chất là phản ứng sinh học nhằm giảm thiểu tối đa mức tiêu thụ năng lượng của cơ thể trong giai đoạn mùa đông khan hiếm thức ăn. Về mặt lý thuyết, nếu nguồn thức ăn luôn được bảo đảm đầy đủ trong suốt mùa đông thì gấu không cần thiết phải ngủ đông. Việc phát triển các khu du lịch và khu dân cư tại hồ Tahoe đã vô tình cung cấp cho loài gấu đen một lượng thức ăn dư thừa dồi dào từ các thùng rác sinh hoạt của con người, đây chính là nguyên nhân chính khiến loài gấu đen tại đây từ bỏ thói quen ngủ đông.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122012.webp)

3、[Xu hướng thời lượng các bài hát nhạc trẻ ngày càng ngắn lại](https://www.billboard.com/pro/songs-getting-shorter-tiktok-streaming/)

Một nghiên cứu thị trường âm nhạc chỉ ra rằng kể từ năm 2000 trở lại đây, thời lượng phát sóng của các bài hát nhạc trẻ thịnh hành đang có xu hướng ngắn dần qua các năm:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122001.webp)

Thời lượng trung bình của một bài hát đã giảm từ mốc 4 phút 10 giây trước đây xuống chỉ còn khoảng 3 phút 30 giây. Đặc biệt, trong danh sách 50 ca khúc thịnh hành nhất tại Mỹ năm 2021, thời lượng trung bình đã rút ngắn xuống chỉ còn 3 phút 07 giây, trong đó có tới 38% số ca khúc có thời lượng chưa đầy 3 phút. Các nhà phân tích nhận định xu hướng này phản ánh sự suy giảm thời gian tập trung (attention span) của người nghe nhạc hiện đại cùng sự bùng nổ của định dạng video ngắn trên nền tảng TikTok.

4、[Giả thuyết mới về nguồn gốc tiến hóa của động vật có vú từ Nam bán cầu](https://www.australiangeographic.com.au/news/2022/12/discovery-identifies-australia-as-birthplace-of-all-modern-mammals/)

Các nhà khoa học Úc mới đây đã công bố nghiên cứu lập luận rằng tổ tiên của toàn bộ động vật có vú hiện đại có thể đã tiến hóa từ Nam bán cầu thay vì Bắc bán cầu như các quan điểm lịch sử trước đây.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122006.webp)

Quan niệm khảo cổ học truyền thống cho rằng động vật có vú bắt nguồn từ Bắc bán cầu do khu vực này sở hữu diện tích đất liền rộng lớn tạo môi trường sống đa dạng. Tuy nhiên, nhóm nghiên cứu chỉ ra rằng cả 3 nhánh phân loại chính của thú có vú bao gồm: thú có túi (như chuột túi), thú có nhau thai (như con người) và thú đơn huyệt đẻ trứng (như thú mỏ vịt) đều phân bố tại nước Úc, trong đó có hai nhánh chỉ tồn tại duy nhất tại Châu Đại Dương. Sự đa dạng này cùng việc phát hiện nhiều mẫu hóa thạch cổ xưa tại Úc là minh chứng mạnh mẽ ủng hộ giả thuyết mới này.

5、[Công nghệ sản xuất tròng kính chống bám sương mù của Thụy Sĩ](https://gizmodo.com/glasses-fog-anti-no-fog-without-spray-heating-gold-laye-1849887511)

Đối với những người phải đeo kính cận thị, hiện tượng tròng kính bị bám sương mù khi thay đổi nhiệt độ đột ngột hoặc khi đeo khẩu trang là một trải nghiệm rất khó chịu. Các nhà khoa học Thụy Sĩ đã phát triển thành công công nghệ tròng kính mới giúp loại bỏ triệt để hiện tượng này:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122101.webp)

*Tròng kính thông thường bên trái bị mờ sương, tròng kính chống bám sương mới bên phải hoàn toàn trong suốt*

Hiện tượng mờ sương xảy ra do hơi ẩm trong không khí tiếp xúc với bề mặt tròng kính có nhiệt độ thấp hơn và ngưng tụ thành các hạt nước li ti. Công nghệ mới đã giải quyết bài toán này bằng cách phủ lên tròng kính một lớp hợp kim vàng siêu mỏng và trong suốt:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122102.webp)

Lớp phủ kim loại này có khả năng hấp thụ chọn lọc các tia hồng ngoại từ ánh sáng mặt trời để tự động làm nóng bề mặt tròng kính lên thêm khoảng 8 độ C, ngăn chặn hiện tượng ngưng tụ hơi nước. Nhược điểm duy nhất của giải pháp này là nó sẽ không hoạt động hiệu quả trong môi trường đêm tối thiếu ánh sáng mặt trời.

## Bài viết

1\. [Wikimedia Foundation công bố Sound Logo chiến thắng cho dự án Wikipedia](https://wikimediafoundation.org/news/2023/03/28/wikipedias-new-sound-logo-winner/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032907.webp)

Tổ chức Wikimedia Foundation đã chính thức công bố mẫu Sound Logo được bình chọn nhiều nhất để làm bộ nhận diện âm thanh tiêu chuẩn cho các sản phẩm nội dung âm thanh và video của Wikipedia trên toàn cầu.

2\. [Tại sao chúng tôi quyết định ngừng sử dụng giải pháp CSS-in-JS](https://dev.to/srmagura/why-were-breaking-up-wiht-css-in-js-4g9b)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102410.webp)

Tác giả phân tích các nhược điểm nghiêm trọng về mặt hiệu năng render của giải pháp viết trực tiếp mã CSS bên trong các tệp tin script JavaScript (CSS-in-JS), đặc biệt là việc làm tăng thời gian phản hồi giao diện của trình duyệt và khuyên lập trình viên nên chuyển sang các giải pháp biên dịch CSS tĩnh.

3\. [Giới thiệu các đơn vị đo khung nhìn CSS mới `lvh` và `svh` cho di động](https://web.dev/viewport-units/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120202.webp)

Bài viết kỹ thuật giới thiệu các đơn vị đo kích thước khung nhìn mới được bổ sung trong CSS như `lvh` (Large Viewport Height) và `svh` (Small Viewport Height), được thiết kế chuyên dụng để tối ưu hóa hiển thị giao diện trang web co giãn mượt mà khi các thanh công cụ hệ thống của trình duyệt di động ẩn/hiện động.

4\. [Bài viết phân tích so sánh chi tiết giữa Cloudflare R2 và AWS S3](https://www.vantage.sh/blog/cloudflare-r2-aws-s3-comparison)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071601.webp)

Dịch vụ lưu trữ đối tượng Cloudflare R2 mới ra mắt được coi là đối thủ cạnh tranh trực tiếp với AWS S3 nhờ chính sách miễn phí hoàn toàn cước phí truyền tải dữ liệu ra ngoài (egress bandwidth). Bài viết so sánh chi tiết về hiệu năng, tính năng và chi phí vận hành thực tế giữa hai dịch vụ này.

5\. [Nhìn lại chặng đường lịch sử thay đổi thiết kế giao diện trang chủ Apple](https://webflow.com/blog/apple-homepage-history)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102201.webp)

Bài viết tổng hợp hình ảnh giao diện trang chủ của tên miền Apple.com từ những năm đầu sơ khai cho đến nay. Bức ảnh phía trên là giao diện trang chủ của Apple vào năm 1997 – thời kỳ khủng hoảng trước khi Steve Jobs quay trở lại để tái cơ cấu tập đoàn.

6\. [Khảo sát tình hình hỗ trợ giải mã định dạng nén video thế hệ mới AV1](https://bitmovin.com/av1-playback-support/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102205.webp)

AV1 là định dạng mã hóa video thế hệ mới giúp tiết kiệm đáng kể băng thông truyền tải mà vẫn giữ nguyên chất lượng hình ảnh sắc nét. Bài viết tổng hợp dữ liệu hỗ trợ giải mã của các hệ điều hành và trình duyệt phổ biến, chỉ ra rằng hệ sinh thái thiết bị của Apple là đơn vị chậm trễ nhất trong việc hỗ trợ định dạng này.

7\. [Tổng hợp các lưu ý quan trọng và điểm khó khi tự học lập trình ngôn ngữ C](https://tmewett.com/c-tips/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112904.webp)

Tác giả tổng hợp lại những ghi chép cá nhân trong suốt quá trình tự học lập trình C, chỉ ra các lỗi logic thường gặp liên quan đến quản lý con trỏ bộ nhớ, giải phóng bộ nhớ động và cách phòng tránh lỗi tràn bộ đệm.

8\. [接手老项目: Lập trình viên nên refactor mã nguồn cũ hay đập đi xây lại hoàn toàn?](https://herbcaudill.com/words/20190219-rewrite-refactor-reinvent)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020502.webp)

Khi tiếp quản một dự án phần mềm cũ có chất lượng mã nguồn kém và khó bảo trì, quyết định nên tiếp tục tối ưu hóa code cũ hay tiến hành viết lại toàn bộ hệ thống từ đầu luôn là bài toán nan giải. Tác giả phân tích kỹ lưỡng 6 trường hợp thực tế để giúp lập trình viên đưa ra quyết định đúng đắn.

## Công cụ

1、[Microsoft Loop: Công cụ cộng tác làm việc nhóm thế hệ mới của Microsoft](https://loop.microsoft.com)

Microsoft chính thức phát hành phiên bản thử nghiệm miễn phí của ứng dụng cộng tác Loop:

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032401.webp)

Nằm trong hệ sinh thái Microsoft 365, Loop cho phép người dùng tạo các trang tài liệu cộng tác tương tự như Notion, hỗ trợ liên kết và đồng bộ trực tiếp các thành phần dữ liệu từ Word, Excel hay PowerPoint vào trang viết chung. Bạn đọc có thể xem chi tiết giới thiệu tại [Microsoft Loop Blog](https://www.microsoft.com/en-us/microsoft-365/blog/2023/03/22/new-microsoft-loop-app-is-built-for-modern-co-creation/).

2、[Mafs: Thư viện component vẽ đồ thị toán học tương tác dựa trên React](https://mafs.dev/)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010301.webp)

Một thư viện nguồn mở chất lượng cao dành cho React hỗ trợ các lập trình viên dễ dàng vẽ và hiển thị các đồ thị toán học, vector hay hình học không gian có tính năng tương tác kéo thả mượt mà trên giao diện web.

3、[ChatGPT-Desktop: Ứng dụng client ChatGPT đa nền tảng viết bằng Vue3](https://github.com/ChatGPT-Desktop/ChatGPT-Desktop)

Dự án mã nguồn mở xây dựng ứng dụng khách (client) để trò chuyện với ChatGPT cài đặt trực tiếp trên các hệ điều hành Windows/macOS/Linux, viết trên nền tảng framework Tauri và Vue 3. (Đóng góp của [@orangelckc](https://github.com/ruanyf/weekly/issues/3010))

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032903.webp)

4、[Tartelet: Tiện ích chạy GitHub Actions cục bộ thông qua máy ảo trên Mac](https://github.com/shapehq/tartelet)

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032917.webp)

Công cụ hỗ trợ các nhà phát triển chạy và kiểm thử nhanh các kịch bản tự động hóa CI/CD GitHub Actions ngay trên máy tính Mac cá nhân thông qua cơ chế khởi tạo các máy ảo độc lập bảo mật. Xem thêm [bài viết giới thiệu chi tiết](https://shape.dk/news/tartelet).

5、[RSS.cafe: Trình đọc tin tức RSS tích hợp quản lý tri thức](https://rss.cafe/)

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032901.webp)

Một ứng dụng đọc tin tức RSS do lập trình viên trong nước phát triển, tích hợp thêm nhiều tính năng quản lý tri thức cá nhân, lưu trữ bài viết yêu thích và đăng ký theo dõi các tạp chí trực tuyến chuyên sâu. (Đóng góp của [@zhi-wenzheng](https://github.com/ruanyf/weekly/issues/3007))

6、[PodFind: Công cụ tìm kiếm nội dung văn bản trong các tập Podcast](https://github.com/mazzzystar/PodFind)

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032904.webp)

Một dự án nguồn mở thú vị: công cụ hỗ trợ người dùng tìm kiếm nhanh các đoạn hội thoại bằng văn bản bên trong các file âm thanh của các kênh podcast. Toàn bộ mã nguồn của dự án này được viết tự động bởi mô hình GPT-4. (Đóng góp của [@mazzzystar](https://github.com/ruanyf/weekly/issues/3015))

7、[SQL Chat: Truy vấn và trò chuyện với cơ sở dữ liệu bằng ngôn ngữ tự nhiên](https://www.sqlchat.ai/)

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032906.webp)

Dịch vụ web nguồn mở hỗ trợ kết nối tới các cơ sở dữ liệu MySQL và PostgreSQL, cho phép người dùng gõ câu hỏi bằng ngôn ngữ tự nhiên để AI tự động biên dịch thành các câu lệnh truy vấn SQL tương ứng. Mã nguồn dự án được chia sẻ tại [SQL Chat GitHub](https://github.com/bytebase/sqlchat). (Đóng góp của [@tianzhou](https://github.com/ruanyf/weekly/issues/3017))

8、[FeatureProbe: Nền tảng quản lý và phân phối tính năng phần mềm nguồn mở](https://github.com/FeatureProbe/FeatureProbe)

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032905.webp)

Hệ thống quản lý tính năng (Feature Flags) nguồn mở hỗ trợ các đội ngũ phát triển phần mềm thực hiện phân phối thử nghiệm AB, phát hành tính năng dạng cuốn chiếu (canary releases) và thay đổi cấu hình hệ thống thời gian thực mà không cần deploy lại code. (Đóng góp của [@nanxijms](https://github.com/ruanyf/weekly/issues/3016))

9、[CubeTrek: Công cụ nhập tọa độ GPS dựng bản đồ lộ trình địa hình 3D](https://cubetrek.com/static/join.html)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010402.webp)

Dịch vụ web cho phép người dùng nạp các tệp tin tọa độ GPS lộ trình di chuyển (file GPX) để vẽ và mô phỏng lại lộ trình đó dưới dạng bản đồ tương tác 3D trực quan, rất thích hợp cho dân leo núi hay chạy bộ.

10、[ov: Công cụ CLI đọc và duyệt văn bản nhanh thay thế cho less](https://noborus.github.io/ov/)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010405.webp)

Tiện ích dòng lệnh viết bằng Go hỗ trợ duyệt xem nội dung các file văn bản lớn tốc độ cao, hỗ trợ highlight từ khóa tìm kiếm và cuộn trang mượt mà nhằm thay thế cho công cụ `less` truyền thống.

## 资源

1、[3D in CSS: Trang web tương tác tìm hiểu các thuộc tính CSS 3D](https://garden.bradwoods.io/notes/css/3d)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011001.webp)

Trang web cung cấp các mô hình hộp 3D trực quan chạy bằng CSS, cho phép người dùng thay đổi các thông số của thuộc tính `transform-style`, `perspective` hay `rotateX/Y/Z` để quan sát sự thay đổi hiển thị thời gian thực.

2、[AI 研究所: Trang tổng hợp kho công cụ và phần mềm trí tuệ nhân tạo](https://www.aiyjs.com/)

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032902.webp)

Một website tiếng Trung chuyên cập nhật và phân loại thông tin về các ứng dụng, website và thư viện lập trình liên quan đến trí tuệ nhân tạo (AI) mới nhất trên thị trường. (Đóng góp của [@xlys997](https://github.com/ruanyf/weekly/issues/3011))

3、[Deep Learning Self-Study: Bộ giáo trình tự học Deep Learning chất lượng](https://dataflowr.github.io/website/)

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032918.webp)

Website cung cấp bộ giáo trình và bài tập thực hành lập trình miễn phí về chủ đề Học sâu (Deep Learning), sử dụng thư viện PyTorch đi kèm các bài giảng video trực quan.

4、[Web Applications 101: Bài viết phổ biến kiến trúc phát triển ứng dụng web](https://www.robinwieruch.de/web-applications/)

Bài viết chi tiết phân tích rõ ràng và hệ thống lại các khái niệm cơ bản của phát triển web hiện đại, giúp lập trình viên phân biệt rõ cơ chế hoạt động của SPA (Single Page App), SSR (Server-Side Rendering) và SSG (Static Site Generation).

## 图片

1、**Những tác phẩm điêu khắc cây nghệ thuật độc đáo của Christophe Guinet**

Một nghệ sĩ người Pháp chuyên sáng tác các tác phẩm điêu khắc có hình dáng vô cùng kỳ lạ lấy cảm hứng từ thiên nhiên:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102609.webp)

Nhìn thoáng qua, người xem sẽ nghĩ đây là những cành cây khô tự nhiên uốn lượn. Thực chất, phần lõi của tác phẩm được tạo hình bằng thạch cao, sau đó nghệ sĩ đã dán tỉ mỉ từng mảng vỏ cây thông thật lên bề mặt ngoài để tạo độ chân thực tối đa:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102610.webp)

Nghệ sĩ chia sẻ anh thường xuyên đi bộ sâu vào các cánh rừng để tìm kiếm nguồn cảm hứng sáng tác. Anh hy vọng khi mọi người vô tình bắt gặp những bức tượng này giữa rừng sâu, họ sẽ trải qua cảm giác kinh ngạc và thú vị, đồng thời suy ngẫm về sức sống kỳ diệu của cỏ cây.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102611.webp)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102612.webp)

Nếu không được báo trước, việc bất ngờ bắt gặp những bức tượng hình thù kỳ quái này giữa rừng hoang vắng chắc chắn sẽ khiến nhiều người giật mình hoảng sợ.

## ✍️ Bài đọc thêm

### Tại sao chúng ta cần phải học môn Vi tích phân (Calculus)?

Vào năm học cuối cấp ba, trường học của tôi có đưa môn Vi tích phân vào chương trình giảng dạy.

Ngay trong buổi học đầu tiên, một học sinh đã giơ tay hỏi: *“Thưa thầy, trong cuộc sống hàng ngày sau này, liệu có khi nào chúng ta cần dùng đến vi tích phân hay không?”*

Thầy giáo thẳng thắn trả lời: *“Không, các em sẽ gần như không bao giờ phải sử dụng các công thức vi tích phân trong cuộc sống sinh hoạt hàng ngày. Thực tế, ngay cả trong công việc chuyên môn sau này của phần lớn các em ở đây, các em cũng sẽ không bao giờ chạm tới nó.”*

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032912.webp)

Nhìn thấy vẻ mặt hoang mang và đầy thắc mắc của cả lớp, thầy mỉm cười và hỏi tiếp: *“Vậy các em có thực sự muốn biết tại sao nhà trường vẫn bắt buộc các em phải học môn học này không?”*

Chúng tôi tò mò gật đầu đồng ý.

Thầy liền chỉ vào một bạn học sinh trong lớp vốn là thành viên chủ chốt của đội bóng đá của trường và hỏi: *“Em vẫn thường xuyên tham gia tập luyện bóng đá cùng đội đúng không?”*

*“Dạ đúng thưa thầy”*, bạn học sinh trả lời. *“Hầu như ngày nào chúng em cũng tập.”*

*“Vậy huấn luyện viên của em có yêu cầu cả đội phải tập nâng tạ trong phòng gym không?”*

*“Có ạ. Mỗi tuần vào thứ Ba và thứ Năm, chúng em đều phải vào phòng gym để tập nâng tạ.”*

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032913.webp)

*“Để làm gì vậy?”* Thầy giáo hỏi tiếp. *“Tại sao cầu thủ bóng đá lại phải tập nâng tạ? Luyện tập nâng tạ có giúp em trực tiếp xô đẩy các cầu thủ đối phương trên sân cỏ hay không?”*

*“Dạ tất nhiên là không phải như vậy rồi ạ.”*

*“Vậy lý do thực sự của việc nâng tạ là gì?”*

*“Nó giúp cho cơ bắp của chúng em trở nên săn chắc và mạnh mẽ hơn ạ”*, bạn học sinh trả lời.

*“Chính xác!”* Thầy giáo gật đầu và kết luận. *“Bài toán học vi tích phân cũng hoàn toàn tương tự như vậy. Các em học vi tích phân không phải để áp dụng trực tiếp các công thức tính đạo hàm hay tích phân vào việc đi chợ mua rau hàng ngày, mà bởi vì quá trình tư duy để giải quyết các bài toán phức tạp đó sẽ rèn luyện cho não bộ của các em trở nên nhạy bén, logic và mạnh mẽ hơn rất nhiều.”*

Tôi đã ghi nhớ sâu sắc bài học đầy ý nghĩa của người thầy giáo năm đó suốt cuộc đời mình.

## Lịch sử tuần này

- 2022年（第 201 期）：[Ngành bán dẫn: Phân tích sự cần thiết của việc thành lập Bộ công nghiệp bán dẫn tại Trung Quốc](http://www.ruanyifeng.com/blog/2022/04/weekly-issue-201.html)
- 2021年（第 151 期）：[Công nghệ số: Tìm hiểu về khái niệm NFT là gì và thực trạng cơn sốt đầu cơ tài sản số](http://www.ruanyifeng.com/blog/2021/03/weekly-issue-151.html)
- 2020年（第 101 期）：[Xã hội số: Nhìn nhận thực tế khi kết nối internet không còn là tài nguyên khan hiếm trong đời sống](http://www.ruanyifeng.com/blog/2020/04/weekly-issue-101.html)
- 2019年（第 51 期）：[Công nghệ phần cứng: Phân tích nguyên nhân khiến tốc độ phát triển chip của laptop bị chậm lại](http://www.ruanyifeng.com/blog/2019/04/weekly-issue-51.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
