# Bản tin chia sẻ công nghệ (Số 299): Yếu tố cốt lõi của AI là dữ liệu ngữ liệu

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/4390) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042401.webp)

Đây là "Khối Băng" tại Thành phố Văn hóa Du lịch Trung Nguyên Đông Sáng ở Tân Hương, Hà Nam. Công trình mô phỏng hiệu ứng xếp chồng của các khối băng với 10 khối kính lớn ghép thành ba tổ hợp kiến trúc độc đáo. (Nguồn: [Archiposition](https://www.archiposition.com/items/20211223113906))

## AI 的关键是语料

Mọi người có nhận thấy hiện nay mỗi khi mở các trang tin tức công nghệ, tràn ngập thông tin đều là về các mô hình AI mới phát hành?

Hôm nay đơn vị A công bố một mô hình, ngày mai đơn vị B ra mắt một mô hình, và mô hình nào nghe qua cũng sở hữu những năng lực xử lý vô cùng phi thường.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050805.webp)

Một báo cáo thống kê vào tháng 5 năm 2023 chỉ ra rằng, tính đến thời điểm đó, riêng tại Trung Quốc đã có tới 79 mô hình AI sở hữu quy mô tham số trên 1 tỷ được công bố. Sau một năm phát triển, số lượng này hiện nay có lẽ đã lên tới hàng ngàn.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050806.webp)

Thành thật mà nói, hiện nay tôi cảm thấy tương đối bão hòa thông tin mỗi khi nghe tin về các mô hình AI mới ra mắt, và không đánh giá cao tính đột phá của các tin tức này.

Quan điểm cá nhân của tôi là việc nỗ lực tối ưu hóa cấu trúc thuật toán, tính năng hay quy mô tham số của mô hình chỉ mang lại hiệu quả giới hạn, **yếu tố mang tính quyết định thực sự đến chất lượng đầu ra của AI chính là dữ liệu ngữ liệu (datasets/corpus) dùng để huấn luyện.**

Thay vì quảng cáo mô hình của bạn mới mẻ hay mạnh mẽ như thế nào, hãy cho tôi biết bạn đã sử dụng nguồn dữ liệu ngữ liệu nào để huấn luyện nó.

Một mô hình có thuật toán hoàn hảo đến mấy nhưng sử dụng nguồn dữ liệu rác thì kết quả đầu ra vẫn là rác; ngược lại, một mô hình có cấu trúc thuật toán thông thường nhưng được cung cấp nguồn dữ liệu huấn luyện phong phú và chất lượng cao vẫn sẽ hoạt động rất hiệu quả. **Thuật toán mô hình không phải là yếu tố cốt lõi, dữ liệu ngữ liệu mới là chìa khóa.**

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050807.webp)

Đây thực tế không phải là quan điểm cá nhân tôi tự nghĩ ra, mà là đúc kết từ kỹ sư James Betker thuộc tập đoàn OpenAI - một chuyên gia AI hàng đầu và là tác giả chính của mô hình tạo ảnh nổi tiếng DALL-E.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050808.webp)

Năm ngoái, ông có chia sẻ [một bài viết ngắn](https://nonint.com/2023/06/10/the-it-in-ai-models-is-the-dataset/) chỉ gồm vài đoạn văn nhưng đã tạo nên làn sóng thảo luận lớn trong cộng đồng công nghệ thế giới. Tại Trung Quốc dường như chưa thấy ai đề cập đến bài viết này, nhưng cá nhân tôi đánh giá đây là một phân tích vô cùng quan trọng.

Ông chia sẻ rằng công việc hàng ngày của ông là nghiên cứu phát triển các mô hình AI, nhưng dù ông có nỗ lực gia tăng quy mô tham số hay tối ưu hóa các phương trình thuật toán đến đâu, hiệu quả cải thiện mô hình mang lại vẫn không rõ rệt bằng việc mở rộng quy mô của tập dữ liệu huấn luyện.

Việc bổ sung thêm nhiều tài liệu huấn luyện chất lượng cao giúp nâng cấp vượt bậc hiệu năng của mô hình và tác động lớn hơn nhiều so với bất kỳ yếu tố thuật toán nào khác. Điều kỳ diệu hơn cả là **các mô hình có cấu trúc thuật toán hoàn toàn khác nhau khi được huấn luyện trên cùng một tập dữ liệu ngữ liệu cuối cùng lại cho ra kết quả hoạt động vô cùng tương đồng.**

Đúc kết của ông chỉ ra sự khác biệt về thuật toán giữa các mô hình thực tế không phải là rào cản cốt lõi, yếu tố quyết định là tài liệu huấn luyện của bạn. Chỉ cần sở hữu nguồn dữ liệu ngữ liệu phong phú và chất lượng hơn, dù bạn ứng dụng cấu trúc mô hình nào thì kết quả thu được cũng sẽ tương tự.

Mới nghe qua bạn có thể cảm thấy kết luận này có vẻ khó tin, nhưng nếu suy ngẫm kỹ lưỡng dưới góc độ khoa học, bạn sẽ nhận thấy giả thuyết này nhiều khả năng là chính xác.

Bởi vì mục tiêu tối thượng của bất kỳ mô hình AI nào cũng là mô phỏng lại cách thức tư duy của bộ não con người. Bản thân dữ liệu ngữ liệu chính là sự phản ánh trực quan tư duy của con người. Đối với cùng một nguồn dữ liệu tư duy đó, dù bạn ứng dụng các quy tắc toán học nào để phân tích thì kết quả bản chất thu được cuối cùng vẫn phải đồng nhất, do cấu trúc tư duy chứa đựng trong dữ liệu là không đổi.

Điều này tương tự như việc **nhiều họa sĩ khác nhau cùng vẽ chân dung của một người mẫu. Nếu mục tiêu chung của các họa sĩ đều là phục dựng chân thực diện mạo của người mẫu, thì chỉ cần các họa sĩ đạt đến một trình độ chuyên môn nhất định, các bức vẽ cuối cùng thu được sẽ vô cùng giống nhau do cấu trúc khuôn mặt của người mẫu là bất biến.**

Phân tích này mang lại cho chúng ta hai bài học giá trị:

（1）Doanh nghiệp nào sở hữu kho dữ liệu ngữ liệu lớn hơn và chất lượng hơn, mô hình AI của doanh nghiệp đó chắc chắn sẽ vượt trội hơn các đối thủ.

（2）Các mô hình AI nguồn mở hoàn toàn có khả năng thay thế vị thế của các mô hình nguồn đóng thương mại, với điều kiện cộng đồng cung cấp đủ nguồn dữ liệu huấn luyện tương xứng.

Dưới đây là nội dung đoạn dịch bài chia sẻ gốc của James Betker, mời các bạn cùng đọc và suy ngẫm:

> Tôi đã làm việc tại OpenAI được gần một năm. Trong thời gian này, tôi đã tham gia huấn luyện rất nhiều mô hình AI tạo sinh, nhiều hơn bất kỳ số lượng nào mọi người có thể hình dung.
> 
> Mỗi khi dành hàng giờ đồng hồ ngồi quan sát và tinh chỉnh các thông số cấu hình của mô hình, điều khiến tôi ấn tượng sâu sắc nhất chính là sự tương đồng kỳ lạ giữa các kết quả huấn luyện.
> 
> Tôi ngày càng nhận thấy rõ rằng **các mô hình AI có xu hướng hội tụ và tiệm cận cực kỳ gần với cấu trúc dữ liệu huấn luyện của chúng.**
> 
> Thực tế này chứng minh rằng khi được huấn luyện trên cùng một tập dữ liệu đủ lâu, hầu như mọi mô hình sở hữu trọng số và thời gian huấn luyện đạt chuẩn đều sẽ hội tụ về cùng một kết quả duy nhất. Một mạng khuếch tán tích chập đủ lớn sẽ cho ra kết quả tương đương.
> 
> Đây thực sự là một phát hiện vô cùng kinh ngạc!
> 
> Nó chứng tỏ hành vi của AI không được quyết định bởi cấu trúc mô hình, tham số hay thuật toán tối ưu hóa. Nó được quyết định hoàn toàn bởi tập dữ liệu ngữ liệu huấn luyện của bạn chứ không phải yếu tố nào khác. Mọi yếu tố thuật toán khác thực chất chỉ là phương pháp tối ưu hóa năng lực tính toán để mô phỏng tiệm cận tập dữ liệu đó.
> 
> Khi chúng ta thảo luận về chất lượng của Lambda, ChatGPT, Bard hay Claude, thực chất cái chúng ta đang so sánh không phải là thuật toán mô hình mà là tập dữ liệu ngữ liệu huấn luyện phía sau của chúng.

## 稀土开发者大会：征集议题和早鸟票

Sự kiện offline kết nối cộng đồng lập trình viên lớn nhất cả nước sắp diễn ra. "Xitu Developer Conference" (Đại hội Lập trình viên Xitu) năm nay đã chính thức công bố lịch trình tổ chức vào cuối tháng Sáu.

Các chủ đề thảo luận tại đại hội năm nay vô cùng đa dạng bao gồm lập trình Frontend, AI công nghệ, điện toán đám mây, kiến trúc hệ thống, DevOps...

**Điểm đặc biệt nhất là đại hội mở cửa đăng ký diễn giả tự do cho toàn bộ cộng đồng lập trình viên**. Nếu bạn đang phát triển một công cụ hữu ích muốn giới thiệu rộng rãi, hoặc sở hữu các kinh nghiệm lập trình giá trị muốn chia sẻ, ban tổ chức sẵn sàng cung cấp sân khấu để bạn trình bày dự án trực tiếp trước hàng ngàn lập trình viên cả nước.

Chỉ cần bài chia sẻ của bạn mang lại nội dung kỹ thuật thực chất (dry run) thu hút sự quan tâm của người nghe, bạn đều có thể gửi đăng ký làm diễn giả để phát biểu tại các phân hội chuyên đề tương ứng. Diễn giả được duyệt sẽ được đài thọ vé tham dự miễn phí toàn bộ chương trình.

Đối với các bạn muốn tham gia giao lưu học hỏi tại sự kiện, ban tổ chức hiện đang mở bán các gói vé sớm (early bird). **Vé trọn gói hai ngày dành riêng cho học sinh, sinh viên chỉ 99 Nhân dân tệ** - tương đương giá của một vé xem phim thông thường. Gói vé thông thường mua theo nhóm (group buy) có giá 139 Nhân dân tệ, và gói vé VIP bao gồm suất ăn trưa hai ngày sự kiện có giá 799 Nhân dân tệ.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050906.webp)

Để gửi đề xuất chủ đề chia sẻ hoặc mua vé tham gia chương trình, xin vui lòng click vào [Đường link sự kiện này](https://conf.juejin.cn/xdc2024/?utm_source=ryf) hoặc quét mã QR trên poster phía trên. Số lượng vé early bird có hạn, các bạn quan tâm muốn mở rộng vòng kết nối và cập nhật xu hướng công nghệ mới nhất hãy nhanh tay đăng ký.

## 科技动态

1、[airbnb ra mắt mô hình nhà bóng bay mô phỏng phim hoạt hình Up](https://zh.airbnb.com/rooms/1126185893236246260)

Nền tảng cho thuê phòng airbnb mới đây đã công bố gói phòng [nhà bóng bay độc đáo](https://zh.airbnb.com/rooms/1126185893236246260) phục dựng chân thực bối cảnh ngôi nhà bay trong bộ phim hoạt hình nổi tiếng "Up" của hãng Pixar, cho phép khách du lịch đăng ký trải nghiệm thực tế.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050402.webp)

Toàn bộ hệ thống đồ nội thất và cách sắp xếp không gian bên trong ngôi nhà được phục dựng giống hệt các phân cảnh trong phim hoạt hình.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050403.webp)

Phần mái nhà được trang bị hệ thống gồm hơn 8.000 quả bóng bay bơm khí Heli sặc sỡ.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050404.webp)

Đặc biệt, ngôi nhà này thực sự có thể "bay" lên không trung. Tất nhiên lực nâng không đến từ bóng bay mà nhà hàng sử dụng một hệ thống cần cẩu lớn để treo lơ lửng ngôi nhà giữa không trung cho du khách sinh hoạt bên trong.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050405.webp)

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050406.webp)

Tôi đang tự hỏi trong điều kiện treo lơ lửng giữa không trung như vậy, hệ thống điện nước của ngôi nhà sẽ được kết nối như thế nào? Nhiều khả năng công trình đã được tích hợp sẵn các bể chứa nước độc lập, hệ thống máy bơm tăng áp, máy phát điện và ắc quy dự phòng.

2、[Tổ chức cuộc thi sắc đẹp dành riêng cho người mẫu ảo AI trên thế giới](https://www.euronews.com/culture/2024/04/25/miss-ai-worlds-first-beauty-contest-with-computer-generated-women)

Một doanh nghiệp Internet của Anh mới đây đã công bố tổ chức cuộc thi hoa hậu thế giới dành riêng cho các người mẫu ảo tạo lập bằng công nghệ AI.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050109.webp)

Các nhà thiết kế đồ họa trên toàn thế giới có thể gửi tác phẩm đăng ký tham gia trên [cổng thông tin chính thức của cuộc thi](https://www.waicas.com/) trước thời hạn ngày 10 tháng 5 năm nay.

Tiêu chí chấm giải không chỉ dựa trên chất lượng hình ảnh người mẫu ảo do AI tạo ra mà còn đánh giá năng lực tương tác của nhân vật với người hâm mộ trên các mạng xã hội và tốc độ tăng trưởng fan thực tế.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050110.webp)

Hội đồng giám khảo sẽ lựa chọn ra top 3 tác phẩm xuất sắc nhất để vinh danh danh hiệu "Miss AI" đi kèm tổng giá trị giải thưởng tiền mặt lên tới 20.000 USD.

Ban tổ chức chia sẻ mục tiêu của cuộc thi nhằm quảng bá tầm ảnh hưởng của công nghệ AI và hỗ trợ các nhà sáng tạo nội dung số hóa tìm kiếm giải pháp thương mại hóa sản phẩm. Sự kiện này cho thấy ngành giải trí và nghệ thuật số dự kiến sẽ là một trong những lĩnh vực sớm nhất chịu tác động mạnh mẽ của công nghệ AI.

3、[Tác động của tiếng gầm rú động cơ xe máy trong đô thị](https://boehs.org/node/everything-i-know-about-the-xz-backdoor)

Một bộ phận người lái xe mô tô phân khối lớn có thói quen độ pô xe để tạo ra âm thanh gầm rú rất lớn khi di chuyển. Họ lập luận rằng âm thanh lớn giúp thu hút sự chú ý của các phương tiện xung quanh từ xa để giảm thiểu tai nạn va chạm giao thông.

Để kiểm chứng tính xác thực của lập luận này, một nhóm nghiên cứu tại Romania đã tổ chức cuộc thực nghiệm thực tế.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040704.webp)

Họ tiến hành đo đạc với 6 mẫu xe mô tô phân khối lớn khác nhau phát ra âm thanh dao động từ 80 đến 110 decibel. Để dễ hình dung, cường độ âm thanh khi máy bay phản lực cất cánh dao động từ 100 đến 120 decibel, nghĩa là tiếng pô xe mô tô độ lớn tương đương.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024040705.webp)

Các số liệu đo đạc chỉ ra rằng trong điều kiện xe ô tô đóng kín cửa kính, người lái xe ô tô chỉ có thể bắt đầu nghe thấy tiếng động cơ mô tô khi khoảng cách giữa hai xe co hẹp dưới 10 mét. Điều này có nghĩa là khi di chuyển tốc độ cao, người lái ô tô hoàn toàn không có đủ thời gian phản xạ xử lý tình huống.

Kết quả thực nghiệm chứng minh rằng yếu tố cốt lõi giúp đảm bảo an toàn giao thông không phải là tiếng pô xe gầm rú lớn mà là việc chủ động làm chủ tốc độ di chuyển.

## Bài viết

1\. [Phân tích giới hạn vật lý của công nghệ ép xung nhịp xử lý CPU](https://www.163.com/dy/article/J1IE4PAD0511BLFD.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050701.webp)

Nhiều game thủ yêu thích việc ép xung (overclock) chip CPU để đạt hiệu năng xử lý cao nhất. Tuy nhiên khi tiệm cận giới hạn vật lý của vật liệu bán dẫn thì việc cải thiện hiệu năng trở nên vô cùng khó khăn. Giới công nghệ đã phải mất ròng rã 15 năm trời để thiết lập kỷ lục ép xung nhịp mới tăng từ mức 8 GHz lên 9 GHz.

2\. [Rủi ro phát sinh chi phí lớn từ các bộ lưu trữ Amazon S3 trống](https://medium.com/@maciej.pocwierz/how-an-empty-s3-bucket-can-make-your-aws-bill-explode-934a383cb8b1)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024043008.webp)

Amazon S3 là dịch vụ lưu trữ đám mây rất phổ biến hiện nay. Tác giả chia sẻ câu chuyện hy hữu khi khởi tạo một bucket S3 trống hoàn toàn và chưa hề ghi nhận bất kỳ dữ liệu tải lên nào nhưng vẫn phát sinh hóa đơn thanh toán lên tới 1.300 USD chỉ sau hai ngày vận hành.

3\. [Chia sẻ lời giải một số bài tập kỳ thi Toán học Toàn cầu Alibaba 2024](https://www.longluo.me/blog/2024/04/16/2024-alibaba-global-mathematics-competition-qualifying-round/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050201.webp)

Tác giả tham gia vòng sơ loại kỳ thi Toán học Toàn cầu Alibaba năm 2024, tự đánh giá chỉ giải quyết được 3 trên tổng số 7 bài toán (các câu 1, 2 và 6) và chia sẻ chi tiết phương pháp giải đề. (Đóng góp của [@longluo](https://github.com/ruanyf/weekly/issues/4394))

4\. [Hướng dẫn sao lưu và quản lý mã nguồn Git hoàn toàn ngoại tuyến](https://www.gibbard.me/using_git_offline/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010913.webp)

Bài viết hướng dẫn lập trình viên các phương pháp sao lưu và đồng bộ kho lưu trữ Git trong điều kiện hoàn toàn không có kết nối internet, ví dụ như cấu hình đẩy mã nguồn trực tiếp sang ổ đĩa USB cầm tay.

5\. [Giải pháp thiết lập các mốc lưu trữ checkpoint tự động cho dự án](https://kyleshevlin.com/make-checkpoint/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024033101.webp)

Bài viết giới thiệu mẹo khai thác các lệnh Makefile để tự động thiết lập các điểm ghi nhận trạng thái (checkpoint) cho mã nguồn trong repository công việc.

6\. [So sánh các giải pháp công nghệ nhận dữ liệu thời gian thực từ máy chủ](https://rxdb.info/articles/websockets-sse-polling-webrtc-webtransport.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024031902.webp)

Bài phân tích chi tiết và so sánh ưu nhược điểm của 5 phương án kỹ thuật giúp trình duyệt nhận dữ liệu real-time từ server bao gồm WebSockets, Server-Sent Events (SSE), Long Polling, WebRTC và WebTransport.

## AI 相关

1\. [Remix Yourself (Ứng dụng trộn ảnh chân dung nghệ thuật bằng AI)](https://styleof.com/s/remix-yourself)

Ứng dụng trực tuyến cho phép người dùng đăng tải 3 bức ảnh mẫu tương ứng gồm ảnh bố cục gốc, ảnh phong cách mỹ thuật cần học và ảnh chân dung cá nhân.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042702.webp)

Hệ thống AI sẽ tự động phân tích và phối trộn tạo nên một tác phẩm nghệ thuật chân dung mới kết hợp các yếu tố trên.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042703.webp)

2\. [twogether.ai (Công cụ ghép ảnh đôi thông minh bằng AI)](https://twogether.ai/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111502.webp)

Trang web ứng dụng AI hỗ trợ tự động cắt ghép và xử lý ánh sáng để tạo nên các bức ảnh chụp chung của hai người bất kỳ (ví dụ ghép ảnh cá nhân đứng cạnh người nổi tiếng) vô cùng chân thực.

3\. [AI nói đồ giải đồ (Công cụ tạo mô tả ảnh bằng AI)](https://imagedescriptiongenerator.xyz/zh)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042901.webp)

Dự án [mã nguồn mở](https://github.com/ShurshanX/AI-Image-Description) hỗ trợ tự động phân tích và sinh đoạn văn bản mô tả nội dung của hình ảnh tải lên, phát triển dựa trên API của ERNIE 3.5 và Gemini Pro 1.5. (Đóng góp của [@ShurshanX](https://github.com/ruanyf/weekly/issues/4370))

4\. [Video âm nhạc thời lượng dài đầu tiên được tạo hoàn toàn bằng AI](https://mashable.com/article/ai-music-videos)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050706.webp)

Tập đoàn OpenAI đã công bố một video âm nhạc dài 4 phút với toàn bộ phần hình ảnh chuyển động và âm nhạc đi kèm đều được thiết kế tự động bởi các công cụ AI. Đây là video AI tự tạo có thời lượng dài nhất từng được công bố.

5\. [Trang tin tóm tắt tin tức công nghệ Hacker News hàng ngày bằng AI](https://www.supertechfans.com/cn)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042903.webp)

Dự án tự động thu thập và dịch tóm tắt các bài viết nổi bật hàng ngày trên trang công nghệ Hacker News sang tiếng Trung bằng AI, hỗ trợ đăng tải trên web và gửi tin qua [Feishu](https://lw9eez9cc6.feishu.cn/wiki/Z408wHLlRi8MdCk6QfacpW6bnB0). (Đóng góp của [@rmrf](https://github.com/ruanyf/weekly/issues/3634))

6\. [MaxKB (Hệ thống trả lời câu hỏi thông minh dựa trên tri thức nội bộ)](https://github.com/1Panel-dev/MaxKB)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024043001.webp)

Dịch vụ xây dựng hệ thống hỏi đáp tự động dựa trên mô hình ngôn ngữ lớn LLM kết hợp cơ sở tri thức nội bộ, cho phép nhúng trực tiếp dạng khung chat hỗ trợ khách hàng vào các trang web bên thứ ba. (Đóng góp của [@maninhill](https://github.com/ruanyf/weekly/issues/4386))

7\. [GeoSpy AI (Công cụ định vị địa điểm chụp ảnh thông minh)](https://geospy.ai/)

Dịch vụ web ứng dụng AI để phân tích các chi tiết cảnh quan trong ảnh tải lên nhằm dự đoán tọa độ vị trí chụp bức ảnh đó.

8\. [Tổng hợp 7 dịch vụ LLM Playground hỗ trợ trải nghiệm AI trực tuyến](https://www.bilibili.com/read/cv34309921/)

Bài viết tổng hợp danh sách 7 trang web uy tín cho phép lập trình viên trải nghiệm và chạy thử nghiệm miễn phí nhiều mô hình ngôn ngữ lớn trực tuyến. (Đóng góp của [@webup](https://github.com/ruanyf/weekly/issues/4408))

## 工具

1\. [ElysiaJS (Khung phát triển ứng dụng Web hiệu năng cao cho Bun)](https://elysiajs.com/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011107.webp)

Khung phát triển Web viết bằng JS được tối ưu hóa đặc biệt và thiết kế chuyên dụng cho môi trường Bun runtime.

2\. [mcfly (Trình tìm kiếm lịch sử câu lệnh shell thông minh)](https://github.com/cantino/mcfly)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011302.webp)

Công cụ tìm kiếm lịch sử nhập lệnh trong Terminal ứng dụng thuật toán mạng nơ-ron giúp dự đoán nhanh câu lệnh cần tìm, giải pháp thay thế thông minh cho phím tắt `Ctrl + R` truyền thống.

3\. [DocKit (Trình quản lý cơ sở dữ liệu Elasticsearch/OpenSearch thông minh)](https://github.com/geek-fun/dockit)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042902.webp)

Ứng dụng quản lý dữ liệu đa nền tảng cho Elasticsearch và OpenSearch, tích hợp OpenAI cho phép người dùng truy vấn dữ liệu bằng câu lệnh ngôn ngữ tự nhiên. (Đóng góp của [@Blankll](https://github.com/ruanyf/weekly/issues/4374))

4\. [IMaker (Trình thiết kế ảnh bìa trực tuyến tối giản)](https://github.com/slince-zero/IMaker)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042906.webp)

Công cụ thiết kế ảnh bìa (cover image) mã nguồn mở viết bằng JavaScript chạy trực tiếp trên trình duyệt. Trải nghiệm bản dùng thử [Demo tại đây](https://img-maker.vercel.app/). (Đóng góp của [@slince-zero](https://github.com/ruanyf/weekly/issues/4385))

5\. [VideoSubtitleGenerator (Công cụ tự động dịch và chèn phụ đề video hàng loạt)](https://github.com/buxuku/VideoSubtitleGenerator)

Tiện ích dòng lệnh hỗ trợ nhận diện giọng nói trong video để tự động tạo file phụ đề và dịch thuật hàng loạt cho các file video trên máy cục bộ. (Đóng góp của [@buxuku](https://github.com/ruanyf/weekly/issues/4393))

6\. [vmr (Công cụ quản lý đa phiên bản ngôn ngữ lập trình)](https://github.com/gvcgo/version-manager)

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050401.webp)

Giải pháp quản lý phiên bản (version manager) đa nền tảng hỗ trợ chuyển đổi nhanh phiên bản của hơn 40 ngôn ngữ lập trình và công cụ phát triển phổ biến. (Đóng góp của [@moqsien](https://github.com/ruanyf/weekly/issues/4398))

Một công cụ có tính năng tương đương khác là [vfox](https://github.com/version-fox/vfox). (Đóng góp của [@aooohan](https://github.com/ruanyf/weekly/issues/4233))

7\. [Pichome (Mã nguồn lưu trữ và quản lý kho ảnh đám mây)](https://github.com/zyx0814/Pichome)

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050707.webp)

Mã nguồn mở hỗ trợ thiết kế trang web lưu trữ và hiển thị thư viện ảnh viết bằng PHP. (Đóng góp của [@fhxsnabi](https://github.com/ruanyf/weekly/issues/4405))

8\. [Bút.COOL (Trình thực thi và xem trực tiếp mã nguồn Frontend)](https://bi.cool/bi)

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050708.webp)

Dịch vụ trực tuyến của Trung Quốc tương tự CodePen, hỗ trợ biên dịch và hiển thị kết quả trực tiếp của các đoạn mã HTML, CSS và JavaScript. (Đóng góp của [@uovol](https://github.com/ruanyf/weekly/issues/4407))

9\. [vue-styled-components (Thư viện styled-components hỗ trợ Vue 3)](https://github.com/v-vibe/vue-styled-components)

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050709.webp)

Thư viện CSS-in-JS hữu ích tương tự styled-components hỗ trợ đắc lực cho các dự án Vue 3. (Đóng góp của [@akinocccc](https://github.com/ruanyf/weekly/issues/4409))

10\. [MonsterMusic (Trình phát nhạc mã nguồn mở trên Android)](https://github.com/ZTFtrue/MonsterMusic)

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050710.webp)

Ứng dụng nghe nhạc ngoại tuyến mã nguồn mở dành riêng cho các thiết bị chạy hệ điều hành Android. (Đóng góp của [@ZTFtrue](https://github.com/ruanyf/weekly/issues/4411))

11\. [Tiện ích hỗ trợ tra cứu thông tin sách thư viện trên trang豆瓣 (Douban)](https://github.com/wyj0605/douban_library)

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050905.webp)

Tiện ích mở rộng trình duyệt giúp tự động kiểm tra xem cuốn sách đang xem trên Douban có sẵn trong kho sách của các thư viện công cộng chỉ định hay không. (Đóng góp của [@wyj0605](https://github.com/ruanyf/weekly/issues/4424))

## 资源

1\. [Thư viện sơ đồ trực quan hóa các khái niệm công nghệ hệ thống](https://github.com/ByteByteGoHq/system-design-101#rest-api-vs-graphql)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023102601.webp)

Kho lưu trữ tổng hợp các hình ảnh đồ họa trực quan giải thích các khái niệm kỹ thuật máy tính phức tạp một cách sinh động.

2\. [Hải Đường thi xã (Trình tra cứu thơ ca cổ đại Trung Quốc)](https://haitang.app/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042905.webp)

Dịch vụ web được phát triển bởi lập trình viên hỗ trợ tra cứu và đọc các tác phẩm thơ ca cổ đại đẹp mắt. (Đóng góp của [@javayhu](https://github.com/ruanyf/weekly/issues/4384))

3\. [svgl (Thư viện tìm kiếm logo thương hiệu định dạng vector)](https://svgl.vercel.app/)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121702.webp)

Trang web hỗ trợ tìm kiếm và tải về file đồ họa vectơ định dạng SVG logo của hầu hết các thương hiệu công nghệ nổi tiếng trên thế giới.

4\. [Brick Center (Trình tự động vẽ sơ đồ lắp ghép Lego bằng AI)](https://www.brickcenter.net)

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050904.webp)

Dịch vụ web độc đáo giúp tự động tạo mô hình hướng dẫn lắp ghép Lego từ từ khóa mô tả do người dùng nhập vào. (Đóng góp của [@husu](https://github.com/ruanyf/weekly/issues/4421))

## 图片

1\. [Thảo luận xoay quanh dung lượng RAM cơ bản trên các dòng máy tính MacBook](https://www.macrumors.com/2024/04/26/apple-mac-base-ram-boosts-ended-tim-cook/)

Các dòng máy tính MacBook cấu hình cơ bản của Apple hiện nay vẫn chỉ trang bị dung lượng RAM khiêm tốn 8GB. Người dùng muốn nâng cấp dung lượng RAM lớn hơn bắt buộc phải trả thêm khoản chi phí rất đắt đỏ.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042602.webp)

Dư luận xã hội đang đặt dấu hỏi lớn vì sao Apple duy trì mức RAM cơ bản thấp như vậy trong khi các dòng máy tính chạy Windows hiện nay hầu hết đã trang bị RAM tối thiểu 16GB.

Đại diện Apple lập luận rằng hệ điều hành macOS sở hữu kiến trúc quản lý bộ nhớ tối ưu cao, cho phép dung lượng 8GB RAM trên máy Mac mang lại hiệu năng tương đương 16GB RAM trên các hệ thống khác.

Dưới đây là biểu đồ thống kê tiến trình nâng cấp dung lượng RAM cơ bản của dòng máy Mac qua các thời kỳ do cộng đồng tổng hợp.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042601.webp)

Biểu đồ cho thấy trong các giai đoạn lịch sử trước đây, Apple duy trì chu kỳ nâng cấp dung lượng bộ nhớ RAM cơ bản tương đối đều đặn sau vài năm.

Tuy nhiên kể từ sau năm 2011, hãng chỉ thực hiện một đợt nâng cấp duy nhất đưa mức RAM cơ bản từ 6GB lên 8GB và giữ nguyên mức này suốt từ đó đến nay.

Một chi tiết thú vị là mốc thời gian năm 2011 cũng chính là thời điểm Tim Cook chính thức đảm nhiệm vai trò CEO của Apple. Ông vốn là chuyên gia quản trị chuỗi cung ứng nổi tiếng với các chiến lược kiểm soát chi phí sản xuất cực kỳ nghiêm ngặt.

2\. [Hoài niệm về hệ điều hành di động PalmOS thời kỳ đầu](https://www.nkorth.com/palm/apps/#totp-authenticator)

Liệu độc giả nào còn nhớ đến thế hệ điện thoại thông minh xuất hiện trước thời kỳ ra đời của chiếc iPhone huyền thoại?

Thời điểm đó thị trường hệ điều hành di động chủ yếu là sự chia sẻ thị phần của các hệ điều hành Nokia Symbian, Microsoft Windows CE và PalmOS. Dưới đây là hình ảnh chiếc điện thoại chạy hệ điều hành Palm danh tiếng một thời.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050702.webp)

Giao diện tương tác người dùng của PalmOS qua các bức ảnh dưới đây.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050703.webp)

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050704.webp)

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050705.webp)

Dù trông có vẻ thô sơ so với tiêu chuẩn ngày nay, nhưng đây từng là hệ điều hành di động tiên tiến nhất thế giới thời kỳ đó với giá bán mỗi thiết bị lên tới vài ngàn Nhân dân tệ.

## ✍️ Bài đọc thêm

### Tìm hiểu về chỉ số tạo cảm giác no bụng của các loại thực phẩm

Loại thực phẩm nào có khả năng xoa dịu cảm giác đói bụng tốt nhất cho cơ thể?

Một nhà khoa học người Úc đã thiết lập nên "Chỉ số tạo cảm giác no" (Satiety Index) để giải đáp bài toán này. Ông lựa chọn khảo sát trên 38 loại thực phẩm thông dụng khác nhau với điều kiện định lượng phần ăn cung cấp mức năng lượng tương đương nhau là 240 calo.

Các tình nguyện viên tham gia thực nghiệm sẽ lần lượt ăn từng loại thực phẩm, sau đó tự đánh giá và cho điểm mức độ no bụng của cơ thể sau mỗi 15 phút kéo dài liên tục trong vòng hai tiếng tiếp theo.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050809.webp)

Kết quả thực nghiệm chỉ ra nhóm thực phẩm giàu carbohydrate (như bánh mì, khoai tây chiên, khoai tây luộc) mang lại hiệu quả tốt nhất. Trong đó, món khoai tây luộc đạt chỉ số tạo cảm giác no cao nhất trong bảng xếp hạng.

Nguyên lý khoa học giải thích do các loại thực phẩm chứa nhiều chất xơ, protein và nước sẽ tiêu tốn thời gian tiêu hóa lâu hơn trong dạ dày giúp duy trì cảm giác no kéo dài. Đồng thời nhóm chất carbohydrate có khả năng nhanh chóng làm tăng lượng đường trong máu giúp hệ thần kinh trung ương nhận biết tín hiệu đã ăn no tức thì.

Món khoai tây luộc chứa hàm lượng chất xơ và nước rất lớn, cùng một mức năng lượng 240 calo nhưng nó cung cấp thể tích phần ăn lớn hơn nhiều và làm tăng nhanh đường huyết giúp duy trì cảm giác no bụng lâu nhất.

![](https://cdn.beekka.com/blogimg/asset/202405/bg2024050810.webp)

Nhóm hoa quả trái cây cũng sở hữu chỉ số no bụng rất cao do hàm lượng nước và chất xơ lớn. Tuy nhiên do hoa quả chứa ít calo nên để đạt mức 240 calo cơ thể cần nạp lượng hoa quả rất lớn dễ gây cảm giác ngấy. Thêm vào đó, tốc độ đào thải của hoa quả ra khỏi dạ dày rất nhanh khiến cảm giác no bụng nhanh chóng biến mất sau giờ thứ hai.

Nhóm thực phẩm giàu chất béo (như mỡ động vật) có chỉ số no bụng rất kém do tốc độ tiêu hóa của chúng trong dạ dày diễn ra rất nhanh, khiến cơ thể nhanh chóng có cảm giác đói bụng trở lại.

Do đó bài viết đưa ra khuyến nghị một chế độ ăn uống khoa học nên phối hợp sử dụng hoa quả kết hợp nhóm carbohydrate và protein chất lượng cao (ví dụ: bánh mì nguyên cám + thịt nạc + cam tươi) để duy trì năng lượng ổn định cho cơ thể.

## Lịch sử tuần này

- 2023年（第 252 期）：[Góc nhìn khởi nghiệp: Phân tích nguyên nhân vì sao hành trình khởi nghiệp công nghệ Internet ngày càng khó khăn](https://www.ruanyifeng.com/blog/2023/04/weekly-issue-252.html)
- 2022年（第 202 期）：[Phương pháp học tập: Giới thiệu ba phương pháp tiếp cận kiến thức mới đầy tính gợi mở](https://www.ruanyifeng.com/blog/2022/04/weekly-issue-202.html)
- 2021年（第 152 期）：[Góc nhìn xã hội: Câu chuyện hướng nghiệp từ giảng đường đại học Bắc Đại đến các trường nghề kỹ thuật](https://www.ruanyifeng.com/blog/2021/04/weekly-issue-152.html)
- 2020年（第 102 期）：[Triết lý cuộc sống: Tìm hiểu nguồn gốc tạo nên tinh thần nhiệt huyết hăng say trong công việc](https://www.ruanyifeng.com/blog/2020/04/weekly-issue-102.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
