# Bản tin chia sẻ công nghệ (Số 271): Thế giới phi tuyến tính và bạn - người tuyến tính

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3425) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091205.webp)

Hãng xe Wuling (Ngũ Lăng) từng cho ra mắt một mẫu xe ý tưởng độc đáo: cải tạo dòng xe điện siêu nhỏ “Hongguang MINI EV” thành một chiếc xe bán tải sáu bánh tí hon đi kèm thùng chở hàng siêu nhỏ phía sau. Dù tính ứng dụng thực tế trong công việc không cao, kiểu dáng dễ thương của chiếc xe vẫn thu hút sự chú ý lớn từ cộng đồng yêu xe. Hiện hãng mới chỉ sản xuất bản chạy thử nghiệm và chưa có kế hoạch thương mại hóa hàng loạt. (Nguồn: [Sohu](https://www.sohu.com/a/679911689_121645910))

## 非线性的世界，线性的你

Naval Ravikant là một nhà đầu tư mạo hiểm người Mỹ nổi tiếng trên Internet, tác giả của chuỗi bài viết chia sẻ tư duy tài chính kinh điển mang tên *“How to get rich”* (Làm thế nào để trở nên giàu có).

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091207.webp)

Các bài viết của ông sau đó đã được biên soạn và xuất bản thành cuốn sách bán chạy. Tại thị trường trong nước, tác phẩm được dịch với tựa đề *“Cuốn sách của Naval: Chỉ dẫn về sự giàu có và hạnh phúc”*, nhanh chóng đạt vị trí quán quân dòng sách quản trị và kinh tế học do cộng đồng Douban bình chọn năm 2022.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091208.webp)

Chuyên mục tuần báo của chúng ta đã từng nhiều lần trích dẫn các quan điểm sâu sắc của Naval. Xin được tổng hợp lại để bạn đọc cùng chiêm nghiệm:

* *“Nếu bạn vừa thấu hiểu kỹ thuật chế tạo sản phẩm, vừa thành thạo kỹ năng bán hàng, bạn sẽ là người bất khả chiến bại trên thị trường.”* (Bản tin Số 94)
* *“Hãy thận trọng, một khi đã nếm trải hương vị của sự tự do tự chủ, bạn sẽ không bao giờ muốn quay lại làm công ăn lương nữa.”* (Bản tin Số 105)
* *“Chìa khóa giúp bạn làm giàu là tìm ra điểm giao thoa hoàn hảo giữa ba yếu tố: Năng lực cá nhân - Nhu cầu thị trường - Thiết kế sản phẩm.”* (Bản tin Số 107)
* *“Hãy kiên trì làm công việc bạn yêu thích, cho đến khi bạn thực sự yêu thích việc mình đang làm.”* (Bản tin Số 184)
* *“Sự nguyên bản trong ý tưởng sẽ giúp bạn tránh khỏi mọi cuộc cạnh tranh khốc liệt. Về bản chất, nếu bạn đang phải cạnh tranh gay gắt với người khác, đó là vì hai bên đang làm những việc hoàn toàn giống nhau.”* (Bản tin Số 258)

Hôm nay, tôi muốn chia sẻ một quan điểm rất đáng suy ngẫm của ông trong buổi trò chuyện trực tiếp cùng MC podcast nổi tiếng Joe Rogan vào năm ngoái:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091209.webp)

Naval chia sẻ:

> *“Sai lầm phổ biến nhất của các nhà khởi nghiệp trẻ tuổi là họ luôn tin rằng mọi kết quả kinh doanh đều có thể dự báo và tính toán trước được. Họ tin rằng hễ mình nỗ lực làm việc chăm chỉ trong thời gian đủ dài thì chắc chắn sẽ gặt hái được thành quả tương xứng.”*
>
> *“Thực tế phũ phàng là kết quả luôn là thứ không thể dự đoán trước được. Mức độ làm việc chăm chỉ của bạn không đóng vai trò quyết định, điều quan trọng quyết định thành bại nằm ở chỗ bạn đang làm sản phẩm gì, bạn hợp tác cùng những ai và bạn đang triển khai nó ở thị trường nào.”*

Ý của Naval là hầu hết chúng ta đều dễ rơi vào một lối mòn tư duy: **luôn mặc định mối quan hệ giữa “nỗ lực cá nhân” và “kết quả gặt hái” là mối quan hệ tỷ lệ thuận tuyến tính** – tức là cứ chăm chỉ hơn thì kết quả sẽ tốt hơn.

Trong thế giới thực, mối quan hệ này hoàn toàn không vận hành đơn giản như vậy. Giữa nỗ lực cơ bắp thuần túy và kết quả thực tế không tồn tại mối quan hệ nhân quả tất yếu.

> *“Bạn có thể dễ dàng quan sát thấy trong xã hội, những người kiếm được nhiều tiền nhất thường không phải là những người có thời gian làm việc dài nhất trong ngày. Ngược lại, những người lao động chân tay hay các chủ tiệm tạp hóa nhỏ làm việc cật lực từ sáng sớm đến đêm muộn nhưng thu nhập mang lại vẫn rất hạn chế.”*

Nguyên nhân cốt lõi là do **thế giới thực tế vận hành theo cơ chế phi tuyến tính và phi nhân quả**, trong khi não bộ con người lại có xu hướng phân tích mọi việc theo lối tư duy tuyến tính đơn giản và cố gắng tìm kiếm mối quan hệ nhân quả một chiều.

Lấy ví dụ trực quan: việc gửi tiền tiết kiệm vào ngân hàng là một hệ thống tuyến tính – bạn gửi tiền càng nhiều thì nhận về lượng tiền lãi càng lớn; ngược lại, thị trường chứng khoán là một hệ thống phi tuyến tính phức tạp – bạn đầu tư số tiền lớn hơn chưa chắc đã mang lại lợi nhuận cao hơn, thậm chí có nguy cơ thua lỗ trắng tay. Chúng ta tuyệt đối không được mang tư duy gửi tiết kiệm tuyến tính để áp dụng vào hoạt động đầu tư chứng khoán phi tuyến tính.

Tương tự như vậy trong sự nghiệp, liệu việc bạn liên tục tăng ca, hy sinh toàn bộ cuộc sống cá nhân để dốc sức cho công việc có chắc chắn mang lại thành công lớn? Câu trả lời phần lớn là không, bởi hai yếu tố này không tồn tại mối liên hệ nhân quả trực tiếp.

Lời khuyên của Naval dành cho chúng ta là:

> *“Điều quan trọng không nằm ở chỗ bạn cày cuốc chăm chỉ ra sao, mà nằm ở việc bạn dành thời gian phân tích và lựa chọn thật kỹ lĩnh vực mình sẽ dấn thân, những cộng sự sẽ đồng hành và dự án mình sẽ triển khai.”*
>
> *“Phương thức làm việc thông minh và hiệu quả không giống như việc chạy marathon xem ai bền bỉ chịu đựng lâu hơn, mà giống như việc chạy nước rút (sprinting): bạn tập trung bứt tốc mạnh mẽ khi cơ hội chín muồi xuất hiện, và dành phần lớn thời gian bình thường để nghỉ ngơi, phục hồi sức khỏe và tích lũy năng lượng.”*
>
> *“Hãy sống và làm việc với tư duy của loài sư tử: kiên nhẫn quan sát, tích lũy thể lực và thực hiện một cú nhảy vồ mồi quyết định khi mục tiêu xuất hiện; đừng chọn cách sống như loài trâu bò cày cuốc cật lực trên đồng ruộng từ sáng sớm đến tối mịt.”*

## 科技动态

1、[Trung Quốc lập kỷ lục thế giới mới về sản lượng phát điện của một tuabin gió đơn lẻ](https://electrek.co/2023/09/05/worlds-largest-wind-turbine-record-typhoon/)

Dòng tuabin gió ngoài khơi khổng lồ mang mã hiệu GWH252-16MW do tập đoàn Goldwind chế tạo hiện là hệ thống phát điện bằng sức gió có quy mô lớn nhất thế giới với chiều dài mỗi cánh quạt lên tới 123 mét và chiều cao của trục quay tương đương một tòa nhà 50 tầng.

Hệ thống được lắp đặt thử nghiệm tại vùng biển ngoài khơi huyện Bình Đàm, tỉnh Phúc Kiến mới đây đã lập nên kỷ lục thế giới mới về sản lượng phát điện:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090707.webp)

Vào ngày 1 tháng 9 vừa qua, khi cơn bão Haikui di chuyển sát vào bờ biển Phúc Kiến mang theo sức gió cực lớn, hệ thống tuabin này đã tận dụng luồng gió mạnh để sản xuất ra **384.100 kWh** điện năng chỉ trong vòng 24 giờ. Lượng điện này đủ để đáp ứng nhu cầu sinh hoạt cho 17 vạn hộ gia đình trong một ngày, thiết lập kỷ lục thế giới mới về sản lượng điện do một tuabin gió đơn lẻ sản xuất trong ngày.

Sự kiện gợi mở một hướng đi công nghệ thú vị: các cơn bão nhiệt đới tuy mang lại sức tàn phá lớn nhưng cũng chứa đựng nguồn năng lượng khổng lồ, nếu chúng ta nghiên cứu phát triển được các dòng tuabin chịu bão tốt để thu hoạch nguồn năng lượng này thì sẽ giải quyết được lượng lớn nhu cầu điện năng sạch.

2、[Hà Lan ra mắt dòng quan tài hữu cơ tự phân hủy nuôi nấm thân thiện môi trường](https://apnews.com/article/nature-burial-mushrooms-netherlands-sustainable-coffin-5b211105cc5566c9ada430f2e2e8e3a0)

Một startup công nghệ sinh học của Hà Lan vừa qua đã cho mắt dòng sản phẩm “quan tài tự nhiên” độc đáo, hoạt động tương tự như một hạt giống hữu cơ giúp cải tạo đất sau khi chôn cất:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052503.webp)

Vỏ ngoài của quan tài được ép từ các sợi thực vật tự nhiên phân hủy nhanh, phần lòng trong được phủ kín bởi một lớp hệ sợi nấm (mycelium) đang hoạt động. Khi được chôn cất dưới lòng đất, độ ẩm sẽ kích hoạt các sợi nấm phát triển mạnh mẽ, giúp đẩy nhanh quá trình phân hủy tự nhiên của cơ thể và chuyển hóa các chất hữu cơ thành nguồn dinh dưỡng sạch cải tạo độ phì nhiêu cho đất chỉ trong vòng một tháng rưỡi.

Mức giá bán lẻ của sản phẩm hiện được niêm yết ở mức 995 Euro (khoảng 26 triệu đồng).

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052504.webp)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052505.webp)

3、[Na Uy cắt giảm các ưu đãi thuế cho xe điện để chuyển sang hỗ trợ người đi bộ và đi xe đạp](https://electrek.co/2022/05/17/norway-rolls-back-ev-incentives-while-boosting-walking-and-cycling/)

Na Uy hiện là quốc gia đi đầu thế giới về tỷ lệ phổ cập xe điện khi có tới hơn 65% lượng xe ô tô mới bán ra trên thị trường là xe thuần điện:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090705.webp)

Trước đây, để khuyến khích người dân mua xe điện, chính phủ đã đưa ra nhiều chính sách ưu đãi lớn như miễn thuế tiêu thụ đặc biệt, giảm phí đỗ xe và phí đường bộ. Tuy nhiên mới đây, chính phủ Na Uy tuyên bố sẽ dừng dần các chính sách ưu đãi này cho xe điện, chuyển hướng nguồn ngân sách để hỗ trợ và khuyến khích người dân lựa chọn đi bộ hoặc đạp xe:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090706.webp)

Chính quyền Na Uy nhận thấy việc quá nhiều xe điện lưu thông vẫn tạo ra áp lực lớn lên hạ tầng giao thông và gây nên tình trạng ùn tắc tại đô thị. Người dân dần nhận thức được rằng giải pháp bảo vệ môi trường triệt để nhất không phải là chuyển từ lái xe xăng sang lái xe điện, mà là hạn chế tối đa việc sử dụng xe ô tô cá nhân khi di chuyển trong thành phố.

4、[Trào lưu cài đặt tính năng đòi tiền tip trên các máy thanh toán tự động gây tranh cãi tại Mỹ](https://www.foxbusiness.com/retail/self-checkout-machines-ask-tips-latest-squeeze-customers)

Tại các cửa hàng dịch vụ ở Mỹ như tiệm bánh ngọt, quán cafe hay phòng tập gym, văn hóa trả tiền tip (tiền boa) cho nhân viên phục vụ là điều phổ biến.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061801.webp)

Tuy nhiên, khi các cửa hàng này chuyển sang áp dụng các máy thanh toán tự động (Self-checkout), do không có nhân viên trực tiếp phục vụ, doanh thu từ tiền tip của cửa hàng bị sụt giảm mạnh. Để bù đắp, nhiều chủ cửa hàng đã cài đặt thêm một màn hình yêu cầu trả tiền tip (gợi ý từ 15% đến 25%) xuất hiện ngay trước bước thanh toán của khách hàng trên máy tự động (hình trên).

Xu hướng này đang vấp phải sự phản đối mạnh mẽ từ người tiêu dùng và giới truyền thông: việc yêu cầu trả tiền tip cho một chiếc máy tự động khi bản thân khách hàng phải tự phục vụ từ đầu đến cuối là điều vô lý và làm méo mó bản chất tốt đẹp ban đầu của văn hóa tiền tip.

## Bài viết

1\. [Tiết lộ nội dung cuốn tiểu sử mới xuất bản phác họa chặng đường phát triển AI của Elon Musk](https://finance.sina.cn/2023-09-08/detail-imzkzkea2108254.d.html)（Tiếng Trung）

Tuần này cuốn tiểu sử chính thức của Elon Musk do cây viết nổi tiếng Walter Isaacson (tác giả cuốn tiểu sử Steve Jobs) chấp bút đã chính thức phát hành. Tạp chí *Time* đã đăng tải trích đoạn chương sách chi tiết kể về những trăn trở, quyết định đầu tư và lộ trình xây dựng các dự án trí tuệ nhân tạo của Musk (từ OpenAI đến xAI) để đối trọng với các ông lớn công nghệ.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090908.webp)

2\. [Bài viết phân tích chuyên sâu: “OpenAI thực sự mong muốn đạt được điều gì?”](https://www.wired.com/story/what-openai-really-wants/)（Tiếng Anh）

Cây viết công nghệ kỳ cựu Steven Levy của tạp chí *Wired* có bài phân tích sâu sắc về hậu trường vận hành, các mục tiêu chiến lược và tầm nhìn dài hạn của ban lãnh đạo OpenAI trong cuộc đua phát triển trí tuệ nhân tạo tổng hợp (AGI). (Hình trên chụp chân dung bốn nhân sự lãnh đạo cốt lõi của OpenAI).

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090906.webp)

3\. [Cẩm nang đúc kết quy trình thực hiện Code Review chất lượng từ chuyên gia kỹ thuật Tencent](https://mp.weixin.qq.com/s/HoFSNCd1U3eoUqYaQiEgwQ)（Tiếng Trung）

Bài viết chia sẻ trên trang chính thức của Tencent Cloud: các kỹ sư trưởng của Tencent chia sẻ chi tiết về phương pháp thiết lập bộ tiêu chuẩn rà soát mã nguồn (Code Review), cách thức tổ chức các phiên rà soát hiệu quả trong đội ngũ phát triển để bảo đảm chất lượng mã nguồn dự án mà không gây ức chế cho lập trình viên.

4\. [Bảng xếp hạng mức độ phổ biến của các ngôn ngữ lập trình năm 2023](https://spectrum.ieee.org/the-top-programming-languages-2023)（Tiếng Anh）

Tạp chí danh tiếng *IEEE Spectrum* công bố bảng xếp hạng các ngôn ngữ lập trình được sử dụng phổ biến nhất năm 2023 dựa trên các số liệu thực tế từ công cụ tìm kiếm, GitHub và các diễn đàn công nghệ. Điểm đặc biệt của bảng xếp hạng này là xếp cả các kỹ năng viết mã truy vấn SQL và HTML vào danh sách đánh giá.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091206.webp)

5\. [Lý giải nguyên nhân iPhone 15 bản tiêu chuẩn chỉ hỗ trợ tốc độ kết nối USB 2.0](https://www.pcgamer.com/apple-finally-put-usb-c-in-the-new-iphone-but-its-inexplicably-limited-to-23-year-old-usb-20-speeds/)（Tiếng Anh）

Mặc dù Apple đã chính thức chuyển đổi cổng sạc trên dòng iPhone 15 sang cổng USB-C tiện lợi, tuy nhiên tốc độ truyền tải dữ liệu trên phiên bản tiêu chuẩn vẫn bị giới hạn ở chuẩn USB 2.0 cũ kỹ. Bài viết phân tích các nguyên nhân kỹ thuật liên quan đến chip xử lý A16 Bionic tích hợp trên máy khiến Apple không thể nâng cấp tốc độ kết nối này tương tự dòng Pro.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091405.webp)

6\. [Phân tích nguyên nhân giúp SQLite trở thành cơ sở dữ liệu hoàn hảo cho điện toán biên](https://blog.turso.tech/why-sqlite-is-so-great-for-the-edge-ee00a3a9a55f)（Tiếng Anh）

Tác giả phân tích chi tiết các đặc tính kỹ thuật vượt trội của SQLite (dung lượng cực nhẹ, hoạt động dạng file không cần cấu hình server, thời gian phản hồi micro giây) giúp nó trở thành sự lựa chọn tối ưu cho các môi trường chạy serverless và điện toán biên (Edge Computing).

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060702.webp)

7\. [Bài viết minh họa bằng tranh vẽ phân tích các chính sách bảo mật của ứng dụng Threads](https://growth.design/case-studies/apple-privacy-policy)（Tiếng Anh）

Nhằm cạnh tranh trực tiếp với Twitter, Meta đã cho ra mắt ứng dụng Threads. Bài viết phân tích chi tiết các điều khoản thu thập dữ liệu người dùng của ứng dụng này được thiết kế sáng tạo dưới dạng một cuốn truyện tranh tương tác sinh động, giúp người đọc dễ dàng nắm bắt thông tin.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090903.webp)

8\. [Nghiên cứu khoa học lý giải khả năng truyền sóng âm qua môi trường chân không](https://finance.sina.com.cn/tech/roll/2023-09-05/doc-imzkrvvf8319091.shtml)（Tiếng Trung）

Sóng âm bản chất là các sóng cơ học cần môi trường vật chất để truyền dẫn nên không thể truyền qua chân không. Tuy nhiên, nghiên cứu vật lý mới đây chỉ ra nếu đặt hai cấu trúc vật liệu tinh thể có tính áp điện ở khoảng cách siêu nhỏ (nano mét), dao động cơ học có thể vượt qua khoảng chân không để truyền tín hiệu âm thanh sang bên kia.

## 工具

1、[echoserver: Dịch vụ hỗ trợ lập trình viên tùy biến HTTP Header phản hồi](https://echoserver.dev/)

Một công cụ trực tuyến miễn phí cho phép các lập trình viên cấu hình tùy biến các thông số HTTP Header trả về của server, phục vụ công tác kiểm thử (testing) và gỡ lỗi kết nối mạng của ứng dụng Front-end.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052101.webp)

2、[DocuSeal: Ứng dụng trực tuyến mã nguồn mở hỗ trợ ký số tài liệu số](https://github.com/docusealco/docuseal)

Giải pháp phần mềm tự triển khai mã nguồn mở hỗ trợ người dùng dễ dàng thiết lập quy trình tạo mẫu tài liệu, điền thông tin và thực hiện ký chữ ký số bảo mật trực tuyến tương tự như DocuSign.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072101.webp)

3、[g: Công cụ dòng lệnh ls thay thế viết bằng ngôn ngữ Go](https://github.com/Equationzhao/g)

Một tiện ích dòng lệnh viết bằng Go hỗ trợ hiển thị danh sách thư mục và tệp tin thay thế cho lệnh `ls` truyền thống trên Windows, macOS và Linux với giao diện hiển thị màu sắc trực quan, biểu tượng đẹp mắt. (Đóng góp của [@Equationzhao](https://github.com/ruanyf/weekly/issues/3465))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090907.webp)

4、[GitHub Old Feed: Tập lệnh userscript khôi phục giao diện bảng tin cũ trên GitHub](https://github.com/wangrongding/github-old-feed)

Tiện ích mở rộng chạy trên trình duyệt thông qua tiện ích Tampermonkey, giúp người dùng khôi phục giao diện hiển thị bảng tin (feed) hoạt động cũ trên trang chủ GitHub để dễ dàng theo dõi các hoạt động star, follow của bạn bè. (Đóng góp của [@wangrongding](https://github.com/ruanyf/weekly/issues/3478))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091301.webp)

5、[LoremGenie: Plugin Figma hỗ trợ sinh nhanh các đoạn văn bản giả điền chỗ trống](https://loremgenie.com)

Một plugin hữu ích dành cho các nhà thiết kế giao diện trên Figma, hỗ trợ tạo nhanh các đoạn văn bản giả (Lorem Ipsum) theo độ dài chỉ định để điền nhanh vào các khối thiết kế giao diện giúp hoàn thiện bản vẽ demo trực quan. (Đóng góp của [@guojiangnian](https://github.com/ruanyf/weekly/issues/3473))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091105.webp)

6、[NoteAI: Công cụ hỗ trợ tóm tắt câu trả lời từ công cụ tìm kiếm bằng AI](https://noteai.com/)

Ứng dụng web tích hợp trí tuệ nhân tạo: khi người dùng nhập câu hỏi tra cứu, hệ thống sẽ thực hiện tìm kiếm trên Internet và tự động phân tích tóm tắt các nội dung từ các trang web kết quả để đưa ra câu trả lời ngắn gọn nhất.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091404.webp)

7、[Idify: Ứng dụng nguồn mở hỗ trợ tự tạo ảnh thẻ từ ảnh chụp chân dung](https://github.com/zhbhun/idify)

Một phần mềm mã nguồn mở chạy hoàn toàn trên trình duyệt máy khách, hỗ trợ tách nền hình ảnh chân dung và ghép trang phục lịch sự để tạo ra các bức ảnh thẻ, ảnh căn cước đúng tiêu chuẩn mà không cần tải dữ liệu ảnh lên máy chủ, bảo đảm an toàn quyền riêng tư. (Đóng góp của [@zhbhun](https://github.com/ruanyf/weekly/issues/3481))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091409.webp)

8、[Plane: Giải pháp quản lý công việc và dự án nguồn mở thay thế cho JIRA](https://github.com/makeplane/plane)

Một hệ thống quản lý dự án (Project Management) và điều phối công việc nguồn mở chạy trên nền web sở hữu giao diện tinh tế, hiện đại, là giải pháp thay thế hoàn hảo cho phần mềm JIRA.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023053103.webp)

9、[Octos: Phần mềm Windows hỗ trợ quản lý hình nền máy tính tương tác bằng HTML](https://github.com/underpig1/octos)

Ứng dụng nhỏ gọn dành cho người dùng Windows, cho phép cấu hình thiết lập các trang web thiết kế bằng HTML/CSS/JS làm hình nền máy tính động có khả năng tương tác trực tiếp với con trỏ chuột của người dùng.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072303.webp)

10\. [Essay.art: Ứng dụng chấm điểm sửa lỗi bài viết luận tiếng Anh IELTS/TOEFL bằng AI](https://www.essay.art/)

Dịch vụ web ứng dụng mô hình ngôn ngữ lớn GPT-4 hỗ trợ đắc lực cho các học viên ôn thi chứng chỉ tiếng Anh: tự động phân tích lỗi ngữ pháp, chấm điểm bài luận và đưa ra các đề xuất viết lại câu nâng cao theo đúng tiêu chuẩn thi IELTS/TOEFL. (Đóng góp của [@zengdamo](https://github.com/ruanyf/weekly/issues/3483))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091411.webp)

11、[RustRover: Trình biên tập mã nguồn chuyên biệt dành cho Rust của JetBrains](https://www.jetbrains.com/rust/)

Hãng phát triển IDE nổi tiếng JetBrains vừa công bố phát hành bản thử nghiệm của trình biên tập mã nguồn chuyên biệt dành riêng cho ngôn ngữ lập trình Rust mang tên RustRover, hiện đang được cung cấp hoàn toàn miễn phí cho cộng đồng trải nghiệm.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091410.webp)

## 资源

1、[permission.site: Trang web thử nghiệm các hộp thoại yêu cầu quyền truy cập của trình duyệt](https://permission.site/)

Một công cụ trực tuyến hữu ích giúp lập trình viên kiểm tra nhanh cách thức hoạt động của các hộp thoại cảnh báo xin quyền truy cập (như camera, vị trí, âm thanh, thông báo đẩy) trên các dòng trình duyệt khác nhau.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080203.webp)

2、[Prisma Data Guide: Tài liệu tự học thiết kế cơ sở dữ liệu cơ bản](https://www.prisma.io/dataguide)

Hãng phát triển thư viện ORM nổi tiếng Prisma cung cấp một bộ cẩm nang hướng dẫn tự học lập trình cơ sở dữ liệu viết bằng tiếng Anh chất lượng cao, giải thích cặn kẽ từ các khái niệm thiết kế bảng dữ liệu, lập chỉ mục cho đến việc tối ưu hóa truy vấn.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091106.webp)

3、[Modern CSS Solutions: Loạt bài viết hướng dẫn các giải pháp CSS hiện đại](https://moderncss.dev/)

Chuyên mục tổng hợp hơn 30 bài viết hướng dẫn kỹ thuật CSS nâng cao, phân tích cách thức ứng dụng các cú pháp và tính năng CSS mới nhất hiện nay để giải quyết triệt để các thách thức thiết kế giao diện web đáp ứng.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061802.webp)

4、[EarTrainX: Công cụ trực tuyến rèn luyện khả năng cảm âm cho người mới học nhạc](https://www.eartrainx.com/)

Trang web giáo dục âm nhạc cung cấp các bài tập nghe nhạc tương tác trực quan, giúp các học viên mới bắt đầu học nhạc lý rèn luyện khả năng nhận diện cao độ nốt nhạc, tiết tấu và giai điệu bài hát. (Đóng góp của [@xzzxy0413](https://github.com/ruanyf/weekly/issues/3467))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091102.webp)

5、[LaTeX Book: Tập hợp các bài viết bàn luận về triết lý viết lách của các nhà văn nổi tiếng](https://github.com/Macin20/why-we-write)

Một lập trình viên yêu thích viết lách đã sử dụng hệ thống LaTeX để biên soạn và xuất bản một cuốn sách nhỏ dạng PDF, tổng hợp các bài phát biểu và phân tích của các tiểu thuyết gia nổi tiếng bàn về triết lý và phương pháp viết lách. (Đóng góp của [@Macin20](https://github.com/ruanyf/weekly/issues/3459))

## 图片

1、**Hình ảnh ghi lại ca phóng tên lửa đẩy thương mại trên biển của Trung Quốc**

Vào ngày 5 tháng 9 vừa qua, công ty vũ trụ tư nhân Galactic Energy của Trung Quốc đã thực hiện phóng thành công tên lửa đẩy thương mại Ceres-1 từ bệ phóng nổi đặt trên vùng biển ngoài khơi Hải Dương, tỉnh Sơn Đông:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091406.webp)

Khu vực biển Hải Dương hiện đã được quy hoạch xây dựng thành trung tâm phóng tên lửa trên biển chuyên dụng của Trung Quốc, hoạt động phóng tên lửa thu hút rất đông khách du lịch đổ về theo dõi trực tiếp từ các tàu du lịch gần đó:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091407.webp)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091408.webp)

2、**Dự án đắp đập ngăn biển Hồng Hải để phát thủy điện khổng lồ đầy táo bạo**

Hồng Hải (biển Đỏ) là vùng biển hẹp kẹp giữa bán đảo Ả Rập và lục địa Đông Phi, trong đó lối thoát phía nam kết nối ra vịnh Aden là một eo biển rất hẹp mang tên Bab-el-Mandeb với chiều rộng chỉ khoảng 29 km:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040901.webp)

Một số kỹ sư đã đưa ra một ý tưởng vô cùng táo bạo: xây dựng một con đập khổng lồ chắn ngang eo biển Bab-el-Mandeb này nhằm chặn dòng nước chảy từ Ấn Độ Dương vào Hồng Hải.

Do Hồng Hải được bao quanh bởi các vùng sa mạc có nhiệt độ cực cao, tốc độ bốc hơi tự nhiên của nước biển tại đây diễn ra rất nhanh. Tính toán chỉ ra nếu đắp đập ngăn dòng chảy bồi đắp, mực nước Hồng Hải sẽ tự động tụt giảm trung bình 2,1 mét mỗi năm:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040902.webp)

Sự sụt giảm này sẽ tạo ra độ chênh lệch mực nước lớn giữa đại dương bên ngoài và Hồng Hải bên trong đập. Bằng việc dẫn dòng nước biển từ ngoài tràn qua đập vào trong qua hệ thống tuabin, con đập có thể tạo ra sản lượng điện năng khổng lồ lên tới 50 Gigawatt – gấp hàng chục lần công suất của các nhà máy điện hạt nhân lớn nhất thế giới hiện nay, mang lại nguồn năng lượng sạch vô hạn cho các quốc gia Đông Phi và Trung Đông. Tuy nhiên, đa số các nhà môi trường học nhận định đây là một ý tưởng không khả thi và tiềm ẩn nguy cơ hủy hoại nghiêm trọng hệ sinh thái biển Hồng Hải.

## ✍️ Bài đọc thêm

### Chín lý do chính tại sao tôi kiên trì viết blog cá nhân hàng ngày

*Bài viết chia sẻ quan điểm của lập trình viên Danny Guo bàn về vai trò của hoạt động viết lách.*

Mọi người xung quanh thường đặt câu hỏi cho tôi: tại sao một lập trình viên bận rộn như tôi lại luôn coi trọng và dành nhiều thời gian để duy trì viết blog cá nhân đến vậy?

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091303.webp)

Dưới đây là các lý do cốt lõi của tôi:

**1. Viết lách giúp sắp xếp và làm sáng tỏ mạch tư duy**

Tôi tự nhận mình không phải là người có khả năng phản ứng nhanh nhạy lập tức tại chỗ, tôi thường làm việc tốt hơn khi có thời gian suy ngẫm sâu sau khi sự việc diễn ra. Hoạt động viết lách ép buộc tôi phải tìm cách liên kết các ý tưởng lộn xộn lại thành các đoạn văn logic mạch lạc, qua đó giúp tôi tự phát hiện ra những điểm phi lý trong tư duy của mình. Viết lách giống như một bộ lọc giúp loại bỏ hoàn toàn các suy nghĩ dư thừa.

Trước đây tôi từng nghĩ viết lách chỉ đơn giản là việc ghi chép lại những ý tưởng sẵn có trong đầu ra trang giấy. Giờ đây tôi nhận ra quá trình viết thực chất chính là quá trình giúp bạn phát triển, mài giũa và sinh ra các ý tưởng mới sâu sắc hơn.

**2. Chia sẻ tri thức hữu ích tới cộng đồng**

Các bài viết blog thường cung cấp các thông tin chi tiết kỹ thuật sâu sắc hơn so với các dòng chia sẻ ngắn trên mạng xã hội, đồng thời tiết kiệm thời gian đọc hơn nhiều so với việc đọc một cuốn sách dày. Người đọc có thể dễ dàng kiểm soát tốc độ đọc hiểu của mình theo bài viết, đồng thời việc dẫn link trỏ nguồn tài liệu tham khảo cũng rất dễ dàng.

Việc biết rằng bài viết của mình giúp ích được cho ai đó ngoài kia mang lại cho tôi niềm vui lớn.

**3. Thúc đẩy bản thân liên tục học hỏi điều mới**

Đôi khi tôi chủ động lựa chọn viết về một chủ đề công nghệ mới mà bản thân chưa thực sự hiểu rõ. Quá trình tìm kiếm tài liệu, viết mã thử nghiệm để biên soạn bài viết blog là cách tốt nhất ép buộc tôi phải đào sâu nghiên cứu cặn kẽ mọi chi tiết kỹ thuật của chủ đề đó.

Kể cả khi viết về một đề tài bản thân đã rất quen thuộc, việc viết lại một cách khoa học cũng giúp tôi phát hiện thêm nhiều chi tiết thú vị mà trước đây mình bỏ qua.

**4. Rèn luyện kỹ năng viết**

Viết blog giống như một bài tập thể dục rèn luyện tư duy ngôn từ hàng ngày. Do blog thuộc quyền sở hữu cá nhân nên tôi hoàn toàn tự do viết về bất kỳ chủ đề nào mình thích mà không gặp rào cản kiểm duyệt, tạo cảm hứng để viết nhiều hơn.

**5. Nhận phản hồi để tự sửa lỗi**

Việc xuất bản bài viết công khai trên Internet là cách nhanh nhất giúp tôi phát hiện ra các sai sót chuyên môn của mình. Bạn đọc dưới phần bình luận luôn rất nhiệt tình chỉ ra các điểm thiếu chính xác để tôi sửa đổi kịp thời.

**6. Tiết kiệm thời gian giải đáp các câu hỏi lặp lại**

Mỗi khi gặp một câu hỏi kỹ thuật xuất hiện lặp đi lặp lại nhiều lần từ đồng nghiệp hay đối tác, tôi sẽ viết một bài blog phân tích chi tiết chủ đề đó. Sau này khi có ai hỏi, tôi chỉ cần gửi link bài viết cho họ là xong, vô cùng tiết kiệm thời gian.

**7. Thỏa mãn niềm vui cá nhân**

Mỗi khi một bài viết tâm huyết của mình nhận được lượt truy cập lớn hoặc được chia sẻ rộng rãi trên các diễn đàn công nghệ lớn, tôi cảm thấy rất tự hào và có thêm động lực sáng tạo.

**8. Mở ra nhiều cơ hội hợp tác nghề nghiệp bất ngờ**

Nhiều đối tác đã tìm đến tôi đề xuất các dự án viết sách, tư vấn giải pháp có trả phí sau khi đọc được các bài viết chia sẻ chất lượng trên blog cá nhân của tôi.

**9. Mang lại nguồn thu nhập phụ từ quảng cáo**

Việc tích hợp các banner quảng cáo nhỏ trên trang blog giúp tôi có thêm một nguồn thu nhập thụ động nhỏ hàng tháng để duy trì chi phí server.

## Lịch sử tuần này

- 2022年（第 224 期）：[Thiết kế giao diện: Phân tích các nguyên nhân cốt lõi giúp Figma đánh bại Sketch trên thị trường](http://www.ruanyifeng.com/blog/2022/09/weekly-issue-224.html)
- 2021年（第 174 期）：[Lộ trình nghề nghiệp: Thảo luận về việc lựa chọn làm một kỹ sư đa năng hay kỹ sư chuyên sâu](http://www.ruanyifeng.com/blog/2021/09/weekly-issue-174.html)
- 2020年（第 124 期）：[Quản trị nhân sự: Tìm hiểu phương pháp đánh giá năng lực và quản lý nhân sự tại tập đoàn Huawei](http://www.ruanyifeng.com/blog/2020/09/weekly-issue-124.html)
- 2019年（第 74 期）：[Kinh tế số: Tại sao mô hình kinh doanh thông tin trong kỷ nguyên số lại không nên thu phí đọc](http://www.ruanyifeng.com/blog/2019/09/weekly-issue-74.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration smooth and efficient.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
