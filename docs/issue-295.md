# Bản tin chia sẻ công nghệ (Số 295): Thiết kế độc đáo của chiếc đồng hồ bóng LED

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần. (**[Thông báo] Tuần sau nghỉ lễ Thanh Minh, bản tin sẽ tạm dừng một số.**)

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/4075) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031801.webp)

Bảo tàng Nghệ thuật Trực tiếp Trên nước (Museum of Art on the Water) tại Nhật Chiếu, Sơn Đông là một công trình nghệ thuật độc đáo dài tới 1 km. Vào mùa xuân và mùa thu, toàn bộ hệ thống kính mặt ngoài có thể được trượt mở hoàn toàn để kết nối không gian trưng bày trong nhà với cảnh quan hồ nước bên ngoài. (Nguồn: [The Paper](https://m.thepaper.cn/newsDetail_forward_24815035))

## 巧妙的灯泡钟

Tuần này, tôi xin chia sẻ thiết kế vô cùng độc đáo của một chiếc [đồng hồ bóng LED](https://ironicsans.beehiiv.com/p/life-death-bulbdial-clock) (Bulbdial Clock).

Ý tưởng thiết kế của sản phẩm được lấy cảm hứng từ các mặt đồng hồ mặt trời (sundial) cổ đại. Như chúng ta đã biết, đồng hồ mặt trời là công cụ đo thời gian cổ xưa hoạt động dựa trên vị trí bóng nắng của kim đĩa chiếu xuống mặt đĩa để xác định thời gian trong ngày.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032412.webp)

Vào năm 2008, một nhà thiết kế người Mỹ đã nảy ra ý tưởng táo bạo: liệu có thể ứng dụng nguyên lý hoạt động của đồng hồ mặt trời để chế tạo một chiếc đồng hồ để bàn hiện đại?

Tuy nhiên ông nhanh chóng nhận ra ý tưởng này gặp nhiều trở ngại thực tế. Do vị trí bóng nắng thay đổi liên tục tùy thuộc vào vĩ độ địa lý khác nhau của người dùng nên rất khó để thiết kế một mặt số cố định chuẩn xác, đồng thời thiết bị hoàn toàn vô dụng vào ban đêm hoặc những ngày trời mưa âm u.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032411.webp)

*(Chú thích ảnh: Đồng hồ mặt trời cổ đại chỉ có khả năng chỉ giờ trong khoảng từ 7 giờ sáng đến 5 giờ chiều).*

Mặc dù vậy, ý tưởng sử dụng bóng đổ để biểu thị thời gian đã khơi gợi cảm hứng giúp nhà thiết kế đề xuất ý tưởng về một chiếc "đồng hồ bóng LED".

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032413.webp)

Cấu trúc cơ bản của đồng hồ bóng LED gồm một đĩa tròn phẳng, ở tâm đĩa cắm một thanh kim thẳng đứng vuông góc, xung quanh đĩa là ba vòng quỹ đạo chứa các bóng đèn chiếu sáng hướng vào thanh kim ở tâm để tạo bóng đổ lên mặt đĩa.

Điểm mấu chốt là cả ba vòng quỹ đạo chứa bóng đèn này đều tự động xoay quanh tâm đĩa với các chu kỳ vận tốc khác nhau tương ứng: 60 giây/vòng, 60 phút/vòng và 12 giờ/vòng đại diện cho các kim giây, kim phút và kim giờ.

Do đó vị trí của ba bóng đèn chiếu sáng sẽ thay đổi liên tục, kéo theo bóng đổ của thanh kim ở tâm cũng dịch chuyển tương ứng đóng vai trò như các cây kim đồng hồ để hiển thị thời gian hiện tại.

Đây là một ý tưởng thiết kế rất sáng tạo và hoàn toàn khả thi dưới góc độ chế tạo kỹ thuật. Nhược điểm duy nhất là việc đọc thời gian phụ thuộc hoàn toàn vào bóng đổ nên thiết bị chỉ hiển thị rõ nét trong các không gian tối (như nhà hàng, quán bar, rạp chiếu phim...) và rất khó quan sát dưới ánh sáng ban ngày.

Nhà thiết kế ban đầu chỉ công bố bản vẽ ý tưởng này lên internet như một dự án thiết kế sáng tạo cá nhân chứ chưa có ý định sản xuất thương mại. Tuy nhiên, một số kỹ sư đã vô cùng hào hứng và quyết định hiện thực hóa thiết bị này.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032414.webp)

Để tối ưu hóa chi phí sản xuất thương mại, phiên bản đồng hồ thực tế đã lược bỏ hoàn toàn hệ thống cơ khí xoay phức tạp. Thay vào đó, họ thiết kế ba vòng đèn LED cố định tương ứng chứa 60 bóng, 60 bóng và 12 bóng LED mini. Tại một thời điểm, trên mỗi vòng chỉ có duy nhất một bóng LED phát sáng để tạo bóng chỉ giờ, phút và giây.

Để người dùng dễ dàng phân biệt, ba vòng đèn LED được thiết lập phát ánh sáng ba màu cơ bản Red - Green - Blue khác nhau giúp tạo nên ba bóng đổ có màu sắc tương ứng vô cùng đẹp mắt.

Thiết kế sau đó đã được đưa vào sản xuất thương mại hàng loạt để bán ra thị trường.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032415.webp)

Cấu trúc bo mạch bên trong của sản phẩm khi tháo dỡ.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032416.webp)

Tuy nhiên phiên bản thương mại thực tế trông khá thô kệch và kém phần cuốn hút về mặt thẩm mỹ, điều này lý giải vì sao doanh số bán ra của sản phẩm tương đối ảm đạm.

Cuối cùng, doanh nghiệp sản xuất đã phải đóng cửa giải thể, dự án đồng hồ bóng LED thương mại bị hủy bỏ nhưng toàn bộ tài liệu thiết kế chi tiết đã được chia sẻ [nguồn mở (open source)](https://wiki.evilmadscientist.com/Bulbdial).

Nhờ nguồn tài liệu mở này, cộng đồng người dùng đam mê tự chế phần cứng (DIY) trên thế giới đã phát triển và tự chế tạo ra nhiều phiên bản đồng hồ bóng LED độc đáo của riêng mình, dưới đây là hai ví dụ điển hình.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032417.webp)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032418.webp)

Điểm chung của các thiết kế tự chế này là đều loại bỏ kim đồng hồ vật lý truyền thống và ứng dụng bóng đổ của đèn LED để hiển thị thời gian.

Tôi đánh giá đây là một ý tưởng thiết kế rất thú vị, độ khó chế tạo không quá cao và cực kỳ thích hợp làm dự án học tập thực hành thiết kế mạch điện tử cho các bạn đam mê công nghệ.

## HarmonyOS NEXT 的开发方案

Hệ điều hành HarmonyOS (Hồng Mông) của Huawei đang tạo nên một vị thế đặc biệt trên thị trường di động. Trước đây, do hệ thống được xây dựng dựa trên mã nguồn mở Android ASOP nên có khả năng tương thích tốt các ứng dụng Android truyền thống, lập trình viên hoàn toàn không cần đầu tư nguồn lực phát triển riêng. Tuy nhiên cục diện hiện tại đã thay đổi.

Huawei xác nhận sẽ chính thức phát hành phiên bản **HarmonyOS NEXT** vào mùa thu năm nay. Đây là một hệ điều hành được xây dựng hoàn toàn mới và hoàn toàn loại bỏ khả năng tương thích với ứng dụng Android.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032707.webp)

Quyết định này buộc **tất cả các ứng dụng di động hiện tại bắt buộc phải phát triển lại một phiên bản ứng dụng riêng biệt dành cho HarmonyOS** từ con số không, với đầy đủ các tính năng tương đương bản Android/iOS hiện hành, đòi hỏi một nguồn kinh phí đầu tư vô cùng lớn.

Tuy nhiên các doanh nghiệp khó có thể bỏ qua nền tảng này. Tại thị trường Trung Quốc, thiết bị Huawei đang nắm giữ thị phần thiết bị Android rất lớn và tập trung chủ yếu vào phân khúc khách hàng trung và cao cấp - nhóm khách hàng sở hữu tỷ lệ chi tiêu thanh toán trong ứng dụng cao nhất.

Các số liệu thống kê cho thấy tính đến quý 1 năm 2023, thị phần của HarmonyOS đã vượt mốc 8% và tiếp tục đà tăng trưởng mạnh mẽ. Do đó việc tối ưu và phát triển ứng dụng tương thích với hệ điều hành mới chỉ là vấn đề thời gian đối với các lập trình viên.

Chính quyền Trung Quốc cũng công bố nhiều chính sách ưu tiên hỗ trợ cho sự phát triển của hệ điều hành này tại các thành phố lớn như [Thâm Quyến](http://www.news.cn/local/20240303/dca3e6d4bd734380b4dc9602d5df9b76/c.html), [Thượng Hải](https://m.21jingji.com/timeline/6d9b6fd73a5bc98a293edc724554a46e.html), [Phúc Châu](https://www.fuzhou.gov.cn/zwgk/gb/202301/t20230111_4520047.htm). Nhiều ứng dụng đầu ngành (như Xiaohongshu, Alipay) đã sớm khởi động dự án phát triển phiên bản chuyên biệt cho hệ thống mới.

Đối với các tập đoàn công nghệ lớn sở hữu nguồn nhân lực dồi dào, việc này chỉ là bài toán phân bổ kỹ sư; nhưng đối với các doanh nghiệp vừa và nhỏ sở hữu đội ngũ lập trình viên hạn chế, đây thực sự là bài toán nan giải về mặt chi phí và nhân sự lập trình chuyên biệt.

Đối với các ứng dụng quy mô vừa và nhỏ, thực tế có một giải pháp kỹ thuật đơn giản giúp giải quyết nhanh bài toán tương thích hệ điều hành này.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032702.webp)

Công nghệ lập trình Web di động H5 (HTML5) sở hữu khả năng tương thích đa nền tảng xuất sắc, cho phép chạy tốt trên nhiều hệ điều hành khác nhau mà hầu như không cần sửa đổi mã nguồn, ví dụ điển hình là các ứng dụng Mini Programs.

Hiện nay phần lớn các dịch vụ đều sở hữu phiên bản WeChat Mini Program tương ứng. Nếu có một giải pháp hỗ trợ **chuyển đổi nhanh mã nguồn WeChat Mini Program thành ứng dụng chạy gốc (native app) trên hệ điều hành HarmonyOS**, đây sẽ là cứu cánh tuyệt vời cho các doanh nghiệp vừa và nhỏ.

Giải pháp phần mềm [FinClip](https://www.finclip.com/) được thiết kế để giải quyết bài toán này. Nó hoạt động như một bộ SDK chứa container Mini Program cho phép chạy trực tiếp các WeChat Mini Programs hay Alipay Cards mà hoàn toàn không cần sửa đổi mã nguồn ứng dụng.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032706.webp)

Mục tiêu thiết kế của FinClip giúp các Mini Programs có khả năng chạy độc lập trên nhiều môi trường khác nhau mà không bị phụ thuộc vào ứng dụng máy chủ (như WeChat hay Alipay). Hệ thống tương thích hoàn toàn với cấu trúc cú pháp và cơ chế đăng nhập của WeChat Mini Program, hiện đã hỗ trợ tốt các nền tảng Android, iOS, HarmonyOS NEXT, Flutter, Windows và các hệ thống màn hình thông minh trên ô tô.

Do đó lập trình viên có thể ứng dụng FinClip để **chuyển đổi nhanh WeChat Mini Program thành ứng dụng chạy gốc trên HarmonyOS NEXT chỉ với một cú click chuột**. Phiên bản SDK dành cho HarmonyOS sở hữu đầy đủ tính năng tương đương bản iOS/Android, hỗ trợ các API và component tương tự WeChat. FinClip đóng vai trò như một lớp tương thích trung gian chạy ngầm để biên dịch và đóng gói Mini Program thành một tệp ứng dụng độc lập chạy trực tiếp trên hệ điều hành mới.

Bên cạnh đó, container này hỗ trợ chạy đồng thời nhiều Mini Programs khác nhau, cho phép doanh nghiệp dễ dàng tích hợp nhiều dịch vụ con tạo thành một siêu ứng dụng (Super App) của riêng mình.

Tóm lại, đối với các ứng dụng đã có phiên bản WeChat Mini Program, [FinClip](https://www.finclip.com/) là một giải pháp tối ưu giúp tiết kiệm chi phí và thời gian chuyển đổi sang HarmonyOS NEXT. Bạn đọc quan tâm có thể đăng ký tài khoản trải nghiệm dịch vụ và có cơ hội nhận các phần quà hấp dẫn như Huawei Mate 60 Pro, MatePad 11...

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032814.webp)

## 科技动态

1、[Dự án bảo tồn nhân giúp thành công loài chim Kiwi hoang dã tại New Zealand](https://www.smithsonianmag.com/smart-news/wild-kiwis-born-near-new-zealands-capital-for-the-first-time-in-more-than-150-years-180983386/)

Loài chim biểu tượng quốc gia của New Zealand là chim Kiwi, một loài chim quý hiếm và không thể tìm thấy ở bất kỳ quốc gia nào khác ngoài tự nhiên.

Đặc điểm của chim Kiwi là hoàn toàn không biết bay, kích thước cơ thể tương đương một chú gà thông thường và sở hữu phần mỏ rất dài.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120714.webp)

Loài chim này từng sở hữu số lượng cá thể rất lớn tại New Zealand. Tuy nhiên kể từ khi loài chồn ecmin (stoat) được đưa vào New Zealand vào thế kỷ 19, chồn ecmin đã săn lùng và ăn thịt chim Kiwi khiến số lượng loài này suy giảm mạnh từ 2% đến 3% mỗi năm. Hiện nay số lượng chim Kiwi chỉ còn khoảng 68.000 cá thể, đối mặt nguy cơ tuyệt chủng trong vòng vài thập kỷ tới nếu không có các giải pháp bảo tồn hữu hiệu.

Để hỗ trợ phục hồi loài này ngoài tự nhiên, vào năm 2022 chính phủ New Zealand đã thiết lập một khu bảo tồn thiên nhiên nghiêm ngặt ở vùng ngoại ô thủ đô Wellington, đặt hơn 4.600 bẫy chồn để dọn sạch mối đe dọa trước khi thả nuôi hơn 60 cá thể chim Kiwi.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120715.webp)

Vào tháng 11 năm 2023, các nhân viên bảo tồn vô cùng vui mừng khi phát hiện sự xuất hiện của hai chú chim Kiwi hoang dã mới sinh tại đây. Đây là lần đầu tiên sau hơn 150 năm ghi nhận sự sinh sản thành công của chim Kiwi hoang dã ngay tại khu vực thủ đô New Zealand.

2、[Phát hiện bằng chứng khảo cổ trực tiếp đầu tiên chứng minh tập tính ăn thịt của khủng long bạo chúa](https://web.archive.org/web/20231210161239/https://www.scientificamerican.com/article/tyrannosaurs-stomach-contents-have-been-found-for-the-first-time/)

Khủng long bạo chúa (Tyrannosaurus Rex - T-Rex) là loài khủng long ăn thịt hung dữ và nặng ký nhất từng được ghi nhận trong lịch sử.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121104.webp)

Tuy nhiên từ trước đến nay, việc khẳng định T-Rex là loài ăn thịt chủ yếu dựa trên các giả thuyết khoa học phân tích cấu trúc răng, móng vuốt và hóa thạch phân của chúng chứ chưa có các bằng chứng thực tế trực tiếp chứng minh.

Mới đây, các nhà khoa học đã tìm thấy bằng chứng trực tiếp đầu tiên khi khai quật một hóa thạch khủng long bạo chúa nhỏ (hình dưới), bên trong vùng dạ dày hóa thạch vẫn còn lưu giữ nguyên vẹn tàn tích cấu trúc xương của các loài khủng long khác mà nó đã ăn thịt trước khi chết.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121105.webp)

Phát hiện khảo cổ này cho thấy sự khó khăn của ngành cổ sinh vật học khi các nhà khoa học phải đóng vai trò như các thám tử thu thập thông tin từ những mảnh hóa thạch đá nhỏ để phục dựng lại lịch sử thế giới tự nhiên cổ đại.

3、[Thiết kế thiết bị chuột máy tính đeo ngón tay độc đáo](https://www.core77.com/posts/125315/A-Wearable-Mouse)

Một công ty khởi nghiệp của Đức mới đây đã giới thiệu thiết bị chuột di động đeo ngón tay vô cùng độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081501.webp)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081502.webp)

Thiết bị được đeo kẹp trực tiếp vào hai ngón tay của người dùng, tích hợp hệ thống cảm biến con quay hồi chuyển để nhận diện chuyển động của bàn tay và các thao tác nhấp chuột trái, chuột phải, nhấp đúp hoặc cuộn trang.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081503.webp)

Chuột đeo ngón tay kết nối với thiết bị máy tính thông qua sóng Bluetooth, rất gọn nhẹ và tiện lợi cho việc di chuyển, hiện được bán với mức giá khoảng 65 USD (tương đương 470 Nhân dân tệ).

4、[Mối lo ngại về lượng nước tiêu thụ khổng lồ để làm mát máy chủ AI](https://apnews.com/article/chatgpt-gpt4-iowa-ai-water-consumption-microsoft-f551fde98083d17a7e8d904f8be822c4)

Các tập đoàn công nghệ lớn đang trở thành những đơn vị tiêu thụ nước khổng lồ phục vụ cho việc vận hành các hệ thống tháp giải nhiệt cho máy chủ trong trung tâm dữ liệu.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091103.webp)

Tập đoàn Microsoft mới đây công bố báo cáo cho thấy lượng nước tiêu thụ năm 2022 của hãng tăng vọt tới 34% so với năm 2021, tiêu tốn thêm khoảng 6,44 triệu tấn nước - tương đương lượng nước đổ đầy cho hơn 2.500 hồ bơi tiêu chuẩn quốc tế.

Giới phân tích nhận định nguyên nhân cốt lõi do Microsoft bắt đầu triển khai các tác vụ tính toán AI quy mô lớn đòi hỏi năng lực giải nhiệt lớn từ hệ thống nước.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091104.webp)

Các nhà nghiên cứu tại Đại học California ước tính cứ mỗi lượt ChatGPT trả lời từ 5 đến 50 câu hỏi sẽ tiêu tốn tương đương 500 ml nước làm mát (tương đương dung tích một chai nước khoáng thông thường). Sự bùng nổ của công nghệ AI dự báo sẽ làm gia tăng áp lực thiếu hụt nguồn nước ngọt trên toàn cầu.

## Bài viết

1\. [Hướng dẫn lựa chọn mô hình ngôn ngữ lớn LLM phù hợp để chạy trên máy tính cá nhân](https://www.bentoml.com/blog/navigating-the-world-of-large-language-models)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032202.webp)

Trong trường hợp muốn thiết lập và chạy thử nghiệm mô hình ngôn ngữ lớn LLM trực tiếp trên máy tính cá nhân tại nhà, lập trình viên nên ưu tiên lựa chọn mô hình nào? Bài viết phân tích và đánh giá ưu nhược điểm của các dòng LLM phổ biến nhất hiện nay.

2\. [Hành trình tìm kiếm quản trị viên bí ẩn của trang web sao lưu archive.today](https://gyrovague.com/2023/08/05/archive-today-on-the-trail-of-the-mysterious-guerrilla-archivist-of-the-internet/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080508.webp)

Trang web [archive.today](https://archive.today/) là một dịch vụ lưu trữ dữ liệu web bí ẩn cho phép tạo bản sao chụp của bất kỳ trang web nào để lưu trữ trực tuyến, tuy nhiên thông tin về người sáng lập dịch vụ hoàn toàn được giữ kín. Tác giả bài viết đã thực hiện cuộc điều tra để tìm lời giải đáp.

3\. [Phân tích kiến trúc hệ thống gửi nhận tin nhắn thời kỳ đầu của WeChat](https://mp.weixin.qq.com/s/dD-aPhnynOqSC3MUYLjeAA)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032813.webp)

Bài viết tóm tắt các nguyên lý cốt lõi giúp hệ thống WeChat xử lý mượt mà tác vụ gửi nhận tin nhắn tức thời của hàng triệu người dùng trong giai đoạn đầu mới phát triển. (Đóng góp của [@ryantang1991](https://github.com/ruanyf/weekly/issues/4193))

4\. [Tìm hiểu API lưu trữ ảo OPFS trên trình duyệt web](https://hughfenghen.github.io/posts/2024/03/14/web-storage-and-opfs/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032810.webp)

Việc cho phép các đoạn mã chạy trên trang web tương tác trực tiếp với hệ thống file trên máy người dùng thường bị hạn chế vì lý do bảo mật. Bài viết giới thiệu cách thức khai thác API OPFS của trình duyệt để tạo không gian lưu trữ ảo cục bộ bảo mật cho trang web. (Đóng góp của [@hughfenghen](https://github.com/ruanyf/weekly/issues/4189))

5\. [Mẹo cấu hình tự động chuyển đổi thông tin tài khoản Git cho từng dự án](https://garrit.xyz/posts/2023-10-13-organizing-multiple-git-identities)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101404.webp)

Mỗi khi làm việc với Git, lập trình viên cần thiết lập thông tin username và email tương ứng. Bài viết chia sẻ mẹo cấu hình Git giúp tự động nhận diện và chuyển đổi thông tin tài khoản phù hợp cho từng dự án công việc hoặc dự án cá nhân.

6\. [Kinh nghiệm thiết lập hệ điều hành Linux Asahi trên máy tính Mac Mini ARM](https://jasoneckert.github.io/myblog/ultimate-linux-arm64-workstation/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101617.webp)

Asahi là một bản phân phối Linux được phát triển tối ưu riêng cho dòng chip Apple Silicon ARM. Tác giả chia sẻ trải nghiệm cài đặt hệ thống này lên Mac Mini để tạo nên một máy trạm Linux có tốc độ xử lý nhanh ấn tượng.

7\. [Hướng dẫn thiết lập Content Security Policy chống tấn công tiêm mã độc XSS](https://www.akshaykhot.com/content-security-policy/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080507.webp)

Bài viết hướng dẫn lập trình viên cấu hình các chính sách an toàn thông tin Content Security Policy (CSP) trên trình duyệt để ngăn ngừa hiệu quả các lỗ hổng bị khai thác tấn công chèn mã độc script XSS.

8\. [Tìm hiểu cơ chế hóa học của hiện tượng rỉ sét kim loại](https://books.worksinprogress.co/book/maintenance-of-everything/vehicles/digression-3-corrosion-rust-never-sleeps/1)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092410.webp)

Bài viết giới thiệu một cách trực quan về hiện tượng ăn mòn và rỉ sét của vật liệu kim loại đi kèm các giai thoại lịch sử thú vị (hình trên mô tả hòm thư sắt đã rỉ sét hoàn toàn trong khi tấm tôn mạ kẽm phía sau vẫn nguyên vẹn nhờ lớp bảo vệ kẽm).

## 工具

1\. [Garnet (Dịch vụ cache hiệu năng cao do Microsoft phát triển)](https://github.com/microsoft/garnet)

Tuần trước, Redis đã chính thức công bố thay đổi giấy phép bản quyền phần mềm (license), thắt chặt việc các doanh nghiệp tự ý sử dụng mã nguồn Redis để xây dựng các gói dịch vụ đám mây thương mại.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032201.webp)

Ngay trước thời điểm đó, Microsoft đã công bố dự án Garnet - một hệ thống lưu trữ cache hiệu năng cao tương thích tốt với các tập lệnh của Redis, thu hút sự chú ý lớn của giới công nghệ.

Song song đó, cộng đồng mã nguồn mở cũng đã fork dự án Redis thành hai nhánh phát triển hoàn toàn miễn phí là [Redict](https://redict.io/) và [Valkey](https://github.com/valkey-io/valkey) để thay thế cho phiên bản Redis thương mại.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032805.webp)

2\. [Superjson (Thư viện tối ưu hóa xử lý định dạng JSON trong JS)](https://github.com/blitz-js/superjson)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102207.webp)

Một mô-đun JavaScript được thiết kế để chuyển đổi kiểu dữ liệu qua lại giữa chuỗi JSON và các cấu trúc dữ liệu JavaScript phức tạp hơn.

3\. [Copilot for Obsidian](https://github.com/logancyang/obsidian-copilot)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032304.webp)

Một plugin mã nguồn mở dành cho trình biên tập ghi chú Obsidian hỗ trợ kết nối nhanh với các mô hình AI chạy cục bộ để làm trợ lý ghi chú. Xem thêm [bài viết hướng dẫn cài đặt](https://mp.weixin.qq.com/s/at7K_8lEfVzQJq5qnpzvUg). (Đóng góp của [@ivone-liu](https://github.com/ruanyf/weekly/issues/4171))

4\. [LunarLink (Nền tảng quản lý kiểm thử tự động API)](https://github.com/tahitimoon/LunarLink)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032806.webp)

Dịch vụ web hỗ trợ lập trình viên xây dựng và thực thi các kịch bản kiểm thử tự động (automation test) cho hệ thống API một cách nhanh chóng. (Đóng góp của [@tahitimoon](https://github.com/ruanyf/weekly/issues/4173))

5\. [text2video](https://github.com/bravekingzhang/text2video)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032808.webp)

Phần mềm mã nguồn mở hỗ trợ tự động thiết kế và tạo các video ngắn dạng trình bày phụ đề từ văn bản mô tả đầu vào. (Đóng góp của [@bravekingzhang](https://github.com/ruanyf/weekly/issues/4187))

6\. [simple-mind-map (Công cụ thiết kế sơ đồ tư duy trên nền Web)](https://github.com/wanglin2/mind-map)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032812.webp)

Trình thiết kế sơ đồ tư duy (mind map) mã nguồn mở chạy trực tiếp trên trình duyệt. Trải nghiệm bản dùng thử [Demo tại đây](https://wanglin2.github.io/mind-map/). (Đóng góp của [@wanglin2](https://github.com/ruanyf/weekly/issues/4190))

7\. [Shap-E](https://github.com/openai/shap-e)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050612.webp)

Mô hình AI do OpenAI phát triển hỗ trợ tạo lập các mô hình đồ họa 3D chuyển động từ câu mô tả văn bản.

8\. [blog-cells](https://github.com/rameshvarun/blog-cells)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082403.webp)

Công cụ hỗ trợ tích hợp các khung code JavaScript tương tác trực tiếp lên trang blog cá nhân tương tự như mô hình hoạt động của Jupyter Notebook.

9\. [Magic Wormhole (Giao thức truyền dữ liệu điểm-điểm an toàn)](https://github.com/magic-wormhole/magic-wormhole)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082501.webp)

Giao thức truyền tải tệp tin an toàn giữa hai máy tính kết nối mạng (không yêu cầu chung mạng nội bộ). Người gửi nhận được một mã khóa ngắn tương ứng để gửi cho người nhận nhập mã tải file.

Nhiều ứng dụng khách hỗ trợ giao thức này đã được phát triển như các dự án [Destiny](https://github.com/LeastAuthority/destiny) hoặc [Mobile Wormhole](https://github.com/pavelsof/mobile-wormhole).

10\. [Mist (Giải pháp chèn watermark chống AI học trộm ảnh)](https://mist-project.github.io)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082502.webp)

Công cụ hỗ trợ chèn các lớp watermark ẩn thông minh lên bề mặt hình ảnh tác phẩm nghệ thuật, khiến các mô hình AI không thể sử dụng hình ảnh này để huấn luyện sao chép phong cách vẽ (hình trên mô tả ảnh sau khi chèn watermark (trái) và lớp watermark phóng đại (phải)).

## 资源

1\. [Dịch vụ trực quan hóa lịch sử nhân vật cổ đại Trung Quốc](https://tools.buyixiao.xyz/historical-figure-query)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032303.webp)

Trang web hỗ trợ tra cứu thông tin của hơn 52.000 nhân vật lịch sử cổ đại, hiển thị trực quan sơ đồ các mối quan hệ xã hội, gia phả dòng họ và bản đồ hành trình cuộc đời của nhân vật (hình trên hiển thị bản đồ hành trình cuộc đời của thi sĩ Lý Bạch). Xem thêm [bài viết giới thiệu công cụ](https://mp.weixin.qq.com/s/evUacKtLOVCrZahgRmnjsg). (Đóng góp của [@inspurer](https://github.com/ruanyf/weekly/issues/4170))

2\. [Bảng xếp hạng mức độ phổ biến của các framework CSS](https://www.libhunt.com/css)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032301.webp)

Trang web thực hiện xếp hạng mức độ phổ biến của các thư viện CSS dựa trên số lượng ngôi sao (stars) nhận được trên GitHub.

3\. [Cẩm nang học tập thuật toán trí tuệ nhân tạo thực hành (AI by doing)](https://aibydoing.com/intro)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032807.webp)

Cuốn sách điện tử tiếng Trung hướng dẫn lập trình viên từng bước làm chủ các thuật toán AI thông qua các bài thực hành lập trình trực quan. (Đóng góp của [@huhuhang](https://github.com/ruanyf/weekly/issues/4178))

4\. [Lamucal (Công cụ phân tích hợp âm bài hát bằng AI)](https://lamucal.ai/)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032809.webp)

Dịch vụ web hỗ trợ tự động phân tích và trích xuất thông tin hợp âm, nhịp điệu, lời bài hát của một bản nhạc từ file audio dựa trên mô hình thuật toán Hybrid-Net. (Đóng góp của [@liufeigit](https://github.com/ruanyf/weekly/issues/4188))

5\. [Z2H (Công cụ thiết kế mẫu tập viết chữ trực tuyến)](https://paper.z2h.cn/)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032811.webp)

Dịch vụ trực tuyến hỗ trợ tạo lập các trang giấy tập viết chữ đẹp cho cả ngôn ngữ tiếng Anh và tiếng Trung. (Đóng góp của [@liamwang](https://github.com/ruanyf/weekly/issues/4191))

## 图片

1\. [Hình ảnh bộ dụng cụ phẫu thuật y tế đầu thế kỷ 19](https://oldoperatingtheatre.com/step-into-the-role-of-a-surgeon-in-our-interactive-game/)

Thời điểm đầu thế kỷ 19 khi y học chưa phát minh ra thuốc gây mê và các chất khử trùng y tế, các ca phẫu thuật ngoại khoa luôn là nỗi ám ảnh kinh hoàng đối với người bệnh.

Bộ dụng cụ phẫu thuật thực tế sử dụng tại bệnh viện St. Thomas (Anh) thời kỳ đó vẫn được lưu giữ nguyên vẹn đến ngày nay.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120502.webp)

Nhìn vào bộ dụng cụ thô sơ này, đặc biệt là chiếc cưa xương, dễ hiểu vì sao tỷ lệ tử vong trên bàn mổ của các ca phẫu thuật thời kỳ đó lên tới gần 50%.

2\. [Biểu đồ thống kê tốc độ trung bình của các nhà vô địch giải đua xe đạp Tour de France](https://www.statista.com/chart/22981/average-speed-of-tour-de-france-winners-by-decade/)

Tour de France là giải đua xe đạp đường trường danh giá nhất thế giới. Biểu đồ dưới đây thống kê tốc độ đạp xe trung bình của các nhà vô địch giải đấu kể từ mùa giải đầu tiên năm 1903.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071106.webp)

Tốc độ đạp xe trung bình liên tục tăng trưởng mạnh mẽ, từ mức 26,85 km/h ở mùa giải đầu tiên lên tới 41,17 km/h ở mùa giải 2021. Tuy nhiên đà tăng trưởng dường như có xu hướng chững lại từ đầu thế kỷ 21.

Trong bối cảnh tổng quãng đường đua duy trì ổn định khoảng 3.500 km, việc gia tăng tốc độ chủ yếu được giải thích nhờ các cải tiến công nghệ vật liệu chế tạo xe đạp nhẹ hơn hoặc do các vận động viên sử dụng các chất kích thích hỗ trợ lực.

3、[Hình ảnh mô phỏng sóng vô tuyến truyền phát trong không gian](https://lcamtuf.substack.com/p/radios-how-do-they-work)

Sóng vô tuyến hoạt động như thế nào? Chúng ta có thể hình dung nó tương tự như việc kéo giãn các bản cực của một tụ điện tích điện, khiến điện trường bên trong tràn ra không gian xung quanh.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024032815.webp)

Khi thực hiện trực quan hóa điện trường để vẽ các đường đi của điện tích ảo, chúng ta sẽ thấy xuất hiện các đường cong kết nối hai cực kéo dài vô tận ra hai bên.

Điện trường tĩnh không mang lại nhiều giá trị cho việc truyền phát thông tin, tuy nhiên việc liên tục thay đổi trạng thái điện tích ở hai đầu cực sẽ tạo nên sự biến thiên điện trường phát đi sóng vô tuyến.

## ✍️ Bài đọc thêm

### Câu chuyện lịch sử về chuyến bay chở người liên tục dài ngày nhất trong lịch sử

Thời gian bay liên tục lâu nhất của một chuyến bay chở người là bao nhiêu ngày?

Từ tháng 12 năm 1958 đến tháng 2 năm 1959, hai phi công người Mỹ đã thực hiện chuyến bay liên tục trên một chiếc máy bay cỡ nhỏ kéo dài tới 64 ngày 22 giờ 19 phút, kỷ lục này đến nay vẫn chưa bị phá vỡ.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121301.webp)

Điều bất ngờ là hai phi công này hoàn toàn không phải là các phi công quân sự hay nhà nghiên cứu khoa học chuyên nghiệp, mà là nhân viên phục vụ tại một trung tâm giải trí ở Las Vegas.

Thời điểm đó, để quảng bá thu hút khách hàng cho trung tâm, họ đưa ra ý tưởng sơn logo thương hiệu lên thân máy bay và thực hiện chuyến bay lập kỷ lục thế giới về thời gian bay liên tục và nhận được sự đồng ý tài trợ của ban giám đốc.

Vào lúc 15h52 ngày 4 tháng 12 năm 1958, chuyến bay chính thức cất cánh. Một xe ô tô mui trần chạy đuổi theo máy bay trên đường băng để quét một lớp sơn trắng lên lốp máy bay nhằm chứng minh bánh xe hoàn toàn không tiếp đất trong suốt hành trình.

Để duy trì hoạt động liên tục trên không, máy bay cần tiếp nhiên liệu định kỳ. Mỗi ngày hai lần, phi công điều khiển máy bay hạ độ cao bay sát mặt đường băng để kết nối ống tiếp dầu và nhận nhu yếu phẩm sinh hoạt chuyển lên từ một chiếc xe tải chạy song song phía dưới.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121302.webp)

Trong suốt hành trình 65 ngày bay, xe tải đã thực hiện tiếp nhiên liệu thành công tổng cộng 128 lần.

Hai phi công luân phiên điều khiển máy bay và nghỉ ngơi ngay trong khoang lái chật hẹp, họ đọc truyện tranh, chơi game và đếm số lượng xe ô tô di chuyển trên đường lộ phía dưới để giết thời gian. Rác thải sinh hoạt được đóng gói cẩn thận để ném xuống các vùng sa mạc hoang vắng dọc hành trình.

Trong một sự cố hy hữu, do quá kiệt sức sau nhiều ngày bay liên tục, phi công điều khiển đã ngủ thiếp đi và chiếc máy bay đã tự bay tự động trong suốt hơn một giờ đồng hồ trước khi anh tỉnh lại mà không gặp sự cố nghiêm trọng nào.

Sau nhiều ngày vận hành liên tục, động cơ và các thiết bị đo trên máy bay bắt đầu xuất hiện các lỗi kỹ thuật nhỏ. Họ quyết định kết thúc hành trình và hạ cánh an toàn vào ngày 7 tháng 2 năm 1959.

Hiện nay, chiếc máy bay lập kỷ lục lịch sử này được treo trưng bày trang trọng tại sảnh nhận hành lý của Sân bay Quốc tế McCarran ở Las Vegas.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121303.webp)

Việc một động cơ máy bay từ những năm 1950 có khả năng hoạt động bền bỉ liên tục hơn 1.500 giờ là một kỳ tích cơ khí ấn tượng. Nhưng phi thường hơn cả là khả năng chịu đựng của hai phi công khi phải sinh hoạt và chịu đựng tiếng ồn động cơ liên tục suốt hơn hai tháng trong khoang lái siêu chật hẹp - điều mà người bình thường khó có thể vượt qua.

## Lịch sử tuần này

- 2023年（第 248 期）：[Góc nhìn công nghệ: Khuyến nghị không nên thần thánh hóa thái quá năng lực của ChatGPT](https://www.ruanyifeng.com/blog/2023/03/weekly-issue-248.html)
- 2022年（第 198 期）：[Kinh tế vĩ mô: Thảo luận về tính khả thi của việc phục hưng ngành sản xuất chế tạo tại Mỹ](https://www.ruanyifeng.com/blog/2022/03/weekly-issue-198.html)
- 2021年（第 148 期）：[Nhận định kinh tế: Xu hướng phát triển của nền kinh tế trong kỷ nguyên tăng trưởng thấp](https://www.ruanyifeng.com/blog/2021/03/weekly-issue-148.html)
- 2020年（第 98 期）：[Kỹ năng mềm: Phương pháp rèn luyện khả năng trình bày luận điểm cá nhân một cách mạch lạc](https://www.ruanyifeng.com/blog/2020/03/weekly-issue-98.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
