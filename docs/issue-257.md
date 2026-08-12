# Bản tin chia sẻ công nghệ (Số 257): Câu chuyện Nvidia của Jensen Huang

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3157) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023053105.webp)

Tại thành phố Trú Mã Điếm, tỉnh Hà Nam, chính quyền địa phương đã huy động lực lượng thu hoạch lúa mì thâu đêm trước khi đợt mưa lớn ập đến. Hệ thống chiếu sáng phục vụ thu hoạch ban đêm được cung cấp bởi 100 thiết bị bay không người lái (drones). Các drones này được kết nối trực tiếp với cáp nguồn từ các xe máy phát điện đặt dưới mặt đất, cho phép duy trì hoạt động chiếu sáng liên tục suốt 10 tiếng đồng hồ. (Nguồn: [HNR](http://news.hnr.cn/djn/article/1/1663732007049814017))

## 黄仁勋的 Nvidia 故事

Jensen Huang (Hoàng Nhân Huân) có lẽ là doanh nhân công nghệ gốc Hoa có sức ảnh hưởng sâu rộng nhất tại Silicon Valley hiện nay.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052809.webp)

Năm 1993, ông cùng hai người bạn đồng hành đã đồng sáng lập nên tập đoàn thiết kế vi mạch bán dẫn Nvidia. Từ xuất phát điểm là một doanh nghiệp khởi nghiệp vô danh, đến nay Nvidia đã vươn lên trở thành tập đoàn công nghệ có giá trị vốn hóa lớn thứ 5 tại Mỹ (chỉ xếp sau các tên tuổi lớn là Apple, Microsoft, Google và Amazon).

Nếu bạn đầu tư mua cổ phiếu của Nvidia vào 10 năm trước thì khoản đầu tư đó hiện đã tăng trưởng lên tới [105 lần](https://www.chinaz.com/2023/0527/1528509.shtml)! Đây chính là mã cổ phiếu ghi nhận mức tăng trưởng mạnh mẽ nhất trên thị trường chứng khoán Mỹ trong thập kỷ qua.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052812.webp)

Tuần trước, Jensen Huang bất ngờ xuất hiện tại Đài Loan và những hình ảnh ông giản dị đi mua đồ ăn vặt tại chợ đêm Ráo Hà đã lan truyền chóng mặt trên mạng xã hội.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052810.webp)

Sau đó mọi người mới biết ông nhận lời tham dự và làm diễn giả danh dự tại Lễ tốt nghiệp của Đại học Quốc gia Đài Loan (NTU) vào ngày 27 tháng 5.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052811.webp)

Tôi thực sự khuyên các bạn nên tìm đọc [toàn văn bài phát biểu này](https://www.businessweekly.com.tw/focus/blog/3012429) (bài phát biểu gốc bằng tiếng Anh đã được dịch sang nhiều ngôn ngữ khác).

Bài chia sẻ của ông chỉ kéo dài khoảng 20 phút nhưng đã trả lời một cách trọn vẹn thắc mắc lớn nhất trong lòng tôi bấy lâu nay: Nvidia đã xây dựng đế chế của mình từ những cột mốc nào. Dưới đây là câu chuyện phát triển của Nvidia được tôi tổng hợp lại dựa trên bài phát biểu đó:

Jensen Huang chia sẻ: **Tại sao chúng tôi lại quyết định thành lập Nvidia? Bởi vì chúng tôi đặt niềm tin lớn vào xu hướng của Điện toán tăng tốc (Accelerated Computing).**

Nhu cầu xử lý tốc độ tính toán của nhân loại chắc chắn sẽ ngày một tăng cao. Các bộ vi xử lý CPU thông thường chỉ phù hợp xử lý các tác vụ tính toán đa dụng (general-purpose computing), trong khi việc tăng tốc tính toán cho các tác vụ chuyên sâu đòi hỏi phải có phần cứng chuyên dụng độc lập. Do đó, mục tiêu khởi nghiệp của chúng tôi là thiết kế ra các bộ vi xử lý phục vụ điện toán tăng tốc.

Thời điểm đó, mảng thị trường có nhu cầu điện toán tăng tốc lớn nhất và sẵn sàng chi trả chính là mảng xử lý đồ họa cho trò chơi điện tử (GPU). Vì vậy chúng tôi lựa chọn card đồ họa chơi game làm sản phẩm khởi nghiệp ban đầu. Chúng tôi định vị doanh nghiệp chỉ tập trung vào khâu thiết kế vi mạch bán dẫn và thuê các đối tác bên thứ ba gia công sản xuất hoàn thiện sản phẩm.

Vào năm 1994, khách hàng thương mại lớn đầu tiên của chúng tôi là tập đoàn game SEGA của Nhật Bản, Nvidia đảm nhận thiết kế chip đồ họa cho hệ máy chơi game thế hệ mới của họ:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052813.webp)

*(Ảnh sản phẩm card đồ họa thế hệ đầu tiên [NV1](https://segaretro.org/NV1) của Nvidia thiết kế cho máy game SEGA)*

Thế nhưng ngay vào năm sau đó, tập đoàn Microsoft đã chính thức công bố chuẩn đồ họa Direct3D dành riêng cho hệ điều hành Windows. Sự kiện này khiến toàn bộ ban lãnh đạo Nvidia rơi vào trạng thái hoảng loạn do thiết kế kỹ thuật của Direct3D xung đột hoàn toàn với cấu trúc chip NV1 mà chúng tôi đang phát triển cho SEGA.

Đứng trước ngã ba đường, chúng tôi đã đưa ra quyết định vô cùng mạo hiểm: chủ động đề xuất chấm dứt hợp đồng phát triển với SEGA và **chuyển hướng toàn bộ nguồn lực sang tự nghiên cứu thiết kế dòng GPU tương thích chuẩn Windows**. Quyết định này đẩy công ty vào thế ngàn cân treo sợi tóc bởi SEGA khi đó là nguồn thu duy nhất của hãng. Lượng tiền mặt còn lại của Nvidia chỉ đủ duy trì bộ máy hoạt động trong vòng 6 tháng; nếu không thể ra mắt sản phẩm mới thành công trong thời gian đó, công ty chắc chắn sẽ phá sản.

May mắn thay đúng vào thời khắc cạn kiệt nguồn vốn, Nvidia đã hoàn thiện thành công dòng chip Riva 128 và sản phẩm đã gặt hái thành công rực rỡ trên thị trường. Đến cuối năm 1997, sản lượng xuất xưởng của dòng chip này vượt mốc 1 triệu đơn vị, giúp Nvidia chính thức vượt qua cơn khủng hoảng sinh tử.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052905.webp)

Chúng tôi tiếp tục bám trụ phát triển các thế hệ card đồ họa cho hệ điều hành Windows suốt 10 năm sau đó.

Mặc dù doanh số bán hàng rất tốt, chúng tôi vẫn đối mặt với một hạn chế lớn: **người dùng hầu như chỉ mua card đồ họa về để phục vụ chơi game, rất khó ứng dụng phần cứng này cho các tác vụ điện toán tăng tốc khác**. Nguyên nhân do các dòng GPU thời kỳ đó bắt buộc phải giao tiếp thông qua các API đồ họa của Windows, lập trình viên không thể trực tiếp tương tác hay lập trình các thuật toán xử lý dữ liệu sâu trên chip đồ họa.

Để mở rộng giới hạn ứng dụng của GPU, **vào năm 2007 chúng tôi đã công bố framework CUDA, hỗ trợ lập trình viên tương tác trực tiếp với tầng kiến trúc phần cứng của GPU** để tự do viết mã thuật toán giải quyết các bài toán khoa học chuyên sâu hay mô phỏng vật lý phức tạp.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052906.webp)

Tuy nhiên, phản hồi của thị trường trong những năm đầu là vô cùng ảm đạm trong khi chi phí để Nvidia phát triển và duy trì framework CUDA lại vô cùng lớn. Việc này đã bào mòn phần lớn lợi nhuận ròng của tập đoàn, khiến giá cổ phiếu lao dốc không phanh. Trong nội bộ công ty cũng phát sinh những tranh cãi gay gắt, nhiều ý kiến đề xuất chấm dứt hoàn toàn dự án CUDA để cắt lỗ.

Nhưng rồi bước ngoặt lịch sử đã xuất hiện một cách vô cùng bất ngờ. **Vào năm 2014, giới nghiên cứu AI đã phát hiện ra kiến trúc của CUDA và sức mạnh tính toán song song của GPU Nvidia đáp ứng một cách hoàn hảo các yêu cầu tính toán khổng lồ của việc huấn luyện mô hình học sâu (AI Deep Learning)**. Nhu cầu mua card đồ họa và ứng dụng CUDA bùng nổ mạnh mẽ trên toàn thế giới. Đi kèm sự trỗi dậy của làn sóng AI, Nvidia đã chính thức bước vào con đường phát triển rực rỡ, kéo theo giá trị cổ phiếu tăng trưởng phi mã.

Bên cạnh AI, chúng tôi cũng luôn chủ động tìm kiếm cơ hội đưa điện toán tăng tốc vào các thị trường mới nổi khác.

Vào năm 2007 khi chiếc iPhone đầu tiên ra đời mở ra kỷ nguyên di động, chúng tôi đã nghiêm túc cân nhắc việc thiết kế chip xử lý cho hệ điều hành Android.

Tuy nhiên, chip xử lý di động đòi hỏi thiết kế tích hợp cao độ (SoC) bao gồm cả CPU, GPU và chip modem viễn thông. **Nếu muốn chen chân vào thị trường di động, Nvidia buộc phải đầu tư phát triển mảng chip modem viễn thông – một lĩnh vực hoàn toàn đi lệch khỏi triết lý cốt lõi của chúng tôi là tập trung vào điện toán tăng tốc.**

Nên chúng tôi đã đưa ra quyết định vô cùng khó khăn: chủ động từ bỏ thị trường chip di động đầy tiềm năng. Để bù đắp, **Nvidia đã chuyển hướng sang khai phá một phân khúc thị trường phù hợp hơn: phát triển chip xử lý chuyên dụng cho công nghệ tự lái của ô tô** – một mảng đòi hỏi khả năng xử lý lượng dữ liệu cảm biến khổng lồ và có không gian phát triển rất lớn.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052907.webp)

Lịch sử phát triển của Nvidia cho thấy một bài học lớn: Chỉ cần bạn kiên định đặt niềm tin vào định hướng cốt lõi dài hạn của mình là đúng đắn, hãy dũng cảm kiên trì theo đuổi nó đến cùng. Đừng quá lo sợ trước các khó khăn tạm thời, cũng đừng để bản thân bị lay động trước các cơ hội kiếm tiền ngắn hạn đi chệch định hướng, thành quả ngọt ngào chắc chắn sẽ đón chờ bạn ở cuối con đường.

## 活动消息

**1、[Hội thảo kỹ thuật: Chia sẻ thực tế phát triển hệ thống Android từ đội ngũ Douyin (Kỳ 4)](https://www.bagevent.com/event/8479092?bag_track=001)**

Để vận hành một siêu ứng dụng di động phục vụ hơn 1 tỷ người dùng hoạt động như Douyin (phiên bản TikTok nội địa), quy trình phát triển và tối ưu hóa hệ thống diễn ra như thế nào?

Chuỗi sự kiện giao lưu kỹ thuật do đội ngũ kỹ sư Android của Douyin tổ chức đã đi đến kỳ thứ 4. Ở kỳ này, ban tổ chức đã lắng nghe ý kiến phản hồi để đưa ra các chủ đề mang tính ứng dụng thực tế cao hơn trong lập trình phần mềm nói chung, bao gồm 5 bài chia sẻ chính:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060103.webp)

1. **Thực chiến quản lý mã nguồn**: Giải pháp đối phó với độ phức tạp của các dự án phần mềm siêu lớn.
2. **Kiến trúc plug-in**: Cách thức Douyin thiết kế và ứng dụng kiến trúc cắm rút tính năng linh hoạt.
3. **Tối ưu hóa máy ảo**: Cơ chế hoạt động của hệ thống máy ảo chạy ngầm trong ứng dụng.
4. **Tối ưu hóa trải nghiệm người dùng**: Phương pháp tinh chỉnh các chi tiết tương tác giao diện mượt mà.
5. **Đảm bảo tính ổn định và hệ thống công cụ bổ trợ**: Giải pháp giám sát và khắc phục sự cố ứng dụng.

Sự kiện sẽ được phát sóng trực tuyến miễn phí vào chiều Chủ Nhật tuần sau (ngày 11 tháng 6). Bạn đọc quan tâm có thể [nhấp vào liên kết này](https://www.bagevent.com/event/8479092?bag_track=001) hoặc quét mã QR dưới đây để đăng ký nhận liên kết xem trực tuyến và tham gia chương trình bốc thăm may mắn nhận nhiều phần quà công nghệ ý nghĩa.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060104.webp)

**2、[Hội thảo kỹ thuật: Ứng dụng thực tiễn của công nghệ Serverless](https://www.bagevent.com/event/sales/rr8fx9nlwz3ykg7m65evetbr3ualrtjt)**

Mô hình tính toán Serverless (FaaS - Function as a Service) hỗ trợ chạy các đoạn mã xử lý dữ liệu trực tiếp trên đám mây đang nhận được nhiều sự quan tâm nhờ ưu điểm loại bỏ khâu tự cấu hình máy chủ backend, tự động co giãn tài nguyên và tiết kiệm tối đa chi phí vận hành.

Tuy nhiên khi đưa vào triển khai thực tế cho các hoạt động kinh doanh phức tạp, doanh nghiệp thường gặp nhiều khó khăn trong khâu thiết kế kiến trúc.

Chiều thứ Bảy tuần này (ngày 3 tháng 6), cộng đồng Juejin phối hợp cùng đội ngũ hạ tầng của ByteDance tổ chức buổi giao lưu thảo luận chuyên đề Serverless tại Trung tâm Thời trang Phương Hằng, Bắc Kinh (đây cũng chính là một trong những tòa nhà văn phòng làm việc của ByteDance):

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060105.webp)

Hội thảo quy tụ các bài tham luận thực tế từ các kỹ sư đầu ngành của ByteDance và Alibaba:

1. **ByteDance Serverless Worker**: Chia sẻ từ đội ngũ phát triển Node.js của ByteDance.
2. **Kinh nghiệm thực tiễn triển khai Serverless**: Chia sẻ từ đội ngũ đám mây Volcano Engine.
3. **Ứng dụng Serverless tối ưu hóa hiệu suất tài nguyên**: Chia sẻ từ kỹ sư Alibaba Cloud.
4. **Các tình huống ứng dụng Serverless cho mảng kinh doanh cốt lõi tại ByteDance**.

Hội thảo hỗ trợ cả hình thức tham gia trực tiếp tại văn phòng ByteDance và phát sóng trực tuyến. Bạn đọc quan tâm có thể [nhấp vào liên kết đăng ký này](https://www.bagevent.com/event/sales/rr8fx9nlwz3ykg7m65evetbr3ualrtjt) để đăng ký tham dự.

## 科技动态

1、[Mẫu thiết bị ổ cứng di động mô phỏng đĩa mềm tích hợp màn hình hiển thị](https://learn.adafruit.com/a-floppy-thumb-drive-with-a-color-file-icon-display)

Một lập trình viên người Mỹ đã tự thiết kế và chế tạo mẫu ổ cứng di động vô cùng sáng tạo:

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030202.webp)

Vỏ ngoài của thiết bị được in 3D mô phỏng hình dáng của chiếc đĩa mềm 3.5 inch cổ điển. Điểm độc đáo là trên bề mặt đĩa được trang bị một màn hình LCD màu hỗ trợ cảm ứng để hiển thị trực tiếp danh sách các tệp tin lưu trữ bên trong đĩa:

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030203.webp)

Hầu hết lập trình viên đều sở hữu khá nhiều USB và ổ cứng di động trong nhà. Khi cần tra cứu xem bên trong chứa tài liệu gì, chúng ta bắt buộc phải cắm thiết bị vào máy tính rất phiền phức. Sáng kiến nhỏ này giúp người dùng kiểm tra nhanh nội dung lưu trữ chỉ bằng cách nhìn lên màn hình của ổ cứng.

2、[Đức thử nghiệm mô hình trình diễn xiếc thú bằng công nghệ chiếu toàn ảnh 3D](https://www.smithsonianmag.com/smart-news/german-circus-uses-stunning-holograms-instead-live-animal-performers-180972376/)

Một rạp xiếc nổi tiếng tại Đức đã thực hiện buổi biểu diễn xiếc thú đặc biệt khi loại bỏ hoàn toàn việc sử dụng động vật sống, thay thế bằng công nghệ trình chiếu toàn ảnh 3D (Hologram):

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030204.webp)

Hệ thống sử dụng 11 máy chiếu laser công suất cao bố trí quanh đấu trường tròn để tạo ra các hình ảnh chuyển động 3D 360 độ sống động cho người xem.

Ban quản trị rạp xiếc chia sẻ giải pháp này giúp bảo vệ quyền động vật, chấm dứt việc nuôi nhốt và huấn luyện thú dữ phục vụ giải trí thương mại. Đồng thời công nghệ này cho phép tạo ra các hiệu ứng hình ảnh kỳ ảo vượt xa đời thực, ví dụ như hình ảnh chú cá vàng khổng lồ bơi lội giữa không trung.

3、[Wilson phát triển thành công mẫu bóng rổ in 3D không cần bơm hơi](https://www.dezeeen.com/2023/03/08/wilsons-airless-3d-printed-basketball/)

Thương hiệu sản xuất dụng cụ thể thao Wilson vừa công bố thế hệ bóng rổ in 3D không sử dụng hơi đầu tiên:

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031301.webp)

Quả bóng được chế tạo bằng công nghệ in 3D sử dụng vật liệu polymer đàn hồi đặc biệt. Cấu trúc của bóng được thiết kế rỗng với bề mặt dạng lưới lục giác xếp lớp giúp không khí lưu thông tự do, loại bỏ hoàn toàn nhu cầu bơm hơi truyền thống:

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031302.webp)

Bóng rổ da truyền thống luôn gặp vấn đề biến đổi độ nảy và cảm giác bóng khi áp suất hơi bên trong thay đổi theo nhiệt độ. Mẫu bóng in 3D này duy trì kích thước, trọng lượng và độ nảy ổn định tuyệt đối trong mọi môi trường thi đấu, thách thức hiện tại của sản phẩm chủ yếu nằm ở độ bền cơ học khi thi đấu thực tế ngoài trời.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031303.webp)

4\. [Kỷ lục thế giới mới về hành trình đi vòng quanh 7 kỳ quan trong 7 ngày](https://www.usatoday.com/story/travel/2023/05/18/new-guinness-world-record-travel-seven-wonders-week/70232560007/)

Một du khách người Mỹ đã thiết lập kỷ lục thế giới Guinness mới khi hoàn thành chuyến đi tham quan 7 kỳ quan thế giới chỉ trong vòng chưa đầy một tuần lễ:

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052805.webp)

Tổng thời gian di chuyển thực tế của anh là 6 ngày 16 giờ 14 phút để lần lượt check-in tại các địa điểm:

* Vạn Lý Trường Thành (Trung Quốc)
* Đền Taj Mahal (Ấn Độ)
* Thành cổ Petra (Jordan)
* Đấu trường La Mã (Ý)
* Tượng Chúa Cứu Thế (Brazil)
* Thành cổ Machu Picchu (Peru)
* Kim tự tháp Chichen Itza (Mexico)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052806.webp)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052807.webp)

Do lịch trình di chuyển vô cùng khẩn trương, ngay sau khi check-in tại mỗi địa điểm, anh phải lập tức di chuyển ra sân bay để kịp đón chuyến bay tiếp theo. Toàn bộ thời gian ăn uống và ngủ nghỉ của anh đều diễn ra trên máy bay, bữa ăn thực tế duy nhất ngoài sân bay của anh là một phần ăn nhanh McDonald's tại Roma.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052808.webp)

Đơn vị tài trợ hành trình – một công ty du lịch quốc tế – cho biết họ sẵn sàng cung cấp gói tour tham quan tương tự cho các khách hàng có nhu cầu với mức giá từ 38.000 USD, tất nhiên với thời gian lịch trình giãn rộng hơn để bảo đảm sức khỏe cho du khách.

## Bài viết

1\. [Nhật ký trải nghiệm của nhân viên trong đợt cắt giảm nhân sự hàng loạt tại Meta](https://www.huxiu.com/article/1600148.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052604.webp)

Bài viết chia sẻ chi tiết góc nhìn chân thực và những xáo trộn tâm lý của một kỹ sư phần mềm thuộc tập đoàn Meta (Facebook) khi nhận được email thông báo sa thải nằm trong chiến dịch cắt giảm hơn 10.000 nhân sự của hãng.

2\. [Ứng dụng ChatGPT viết bài và sản xuất video tiếp thị tự động cho nhà máy](https://t.cj.sina.com.cn/articles/view/6286736254/176b7fb7e01901df3u)（Tiếng Trung）

Tác giả chia sẻ kinh nghiệm thực tế trong việc ứng dụng API của ChatGPT để tự động hóa khâu sản xuất hàng loạt các bài viết tiếp thị sản phẩm và tự động tạo kịch bản video giới thiệu cho một doanh nghiệp sản xuất linh kiện điện tử để gia tăng hiệu quả bán hàng.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052803.webp)

3\. [Kích thước tản nhiệt khổng lồ trên thiết kế card đồ họa thế hệ mới](https://m.cnbeta.com.tw/view/1362895.htm)（Tiếng Trung）

Thương hiệu MSI vừa trưng bày mẫu card đồ họa thử nghiệm có độ dày chiếm tới 4,2 khe cắm PCIe trên bo mạch chủ, được thiết kế để chuẩn bị cho khả năng tản nhiệt của dòng GPU RTX 5090 thế hệ tiếp theo:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060107.webp)

Khối card khổng lồ chủ yếu là hệ thống lá tản nhiệt đồng dày đặc, đòi hỏi các dòng vỏ máy tính chuyên dụng kích thước lớn mới có thể lắp vừa, cho thấy xu hướng tiêu thụ điện năng và tỏa nhiệt cực lớn của các GPU thế hệ mới.

4\. [Deno phiên bản 1.34 hỗ trợ đóng gói ứng dụng Node.js thành file nhị phân](https://deno.com/blog/v1.34)（Tiếng Anh）

Bản cập nhật Deno thế hệ mới bổ sung tính năng hỗ trợ lập trình viên đóng gói toàn bộ mã nguồn ứng dụng Node.js cùng các module npm đi kèm thành một tệp tin thực thi nhị phân duy nhất chạy trực tiếp trên các hệ điều hành Windows, macOS và Linux mà không cần cài đặt môi trường node.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052516.webp)

5\. [Giới thiệu tính năng hiển thị popover mặc định trên trình duyệt Chrome](https://developer.chrome.com/blog/introducing-popover-api/)（Tiếng Anh）

Hộp thoại popup (popover) là thành phần UI vô cùng phổ biến trên các trang web. Chrome chính thức công bố hỗ trợ Popover API mặc định trên trình duyệt, giúp lập trình viên Front-end dễ dàng tạo các hộp thoại popup tương tác chỉ bằng các thuộc tính HTML thô mà không cần viết các đoạn mã JS phức tạp.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052402.webp)

6\. [Hướng dẫn thiết kế trang hồ sơ cá nhân GitHub tương tác động](https://www.bengreenberg.dev/posts/2023-04-09-github-profile-dynamic-content/)（Tiếng Anh）

Bài viết hướng dẫn lập trình viên tối ưu hóa trang hiển thị cá nhân (GitHub Profile README) bằng cách viết các script tự động gọi API cập nhật thông tin bài viết blog mới hoặc hoạt động coding cá nhân thông qua công cụ tự động hóa GitHub Actions.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041101.webp)

7\. [Báo cáo rò rỉ nội bộ phân tích về rào cản công nghệ AI của Google](https://www.semianalysis.com/p/google-we-have-no-moat-and-neither)（Tiếng Anh）

Bài viết chia sẻ nội dung một bức thư phân tích rò rỉ được cho là của một kỹ sư nghiên cứu AI gửi tới ban lãnh đạo Google, chỉ ra rằng cả Google lẫn OpenAI thực tế đều không sở hữu rào cản công nghệ (moat) thực sự trong cuộc đua AI, mà chính cộng đồng phát triển mã nguồn mở với tốc độ cải tiến nhanh chóng mới là bên đang dẫn đầu thế cuộc.

## 工具

1、[csv2img: Tiện ích chuyển đổi dữ liệu CSV thành hình ảnh bảng biểu](https://github.com/fummicc1/csv2img)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011906.webp)

Một công cụ mã nguồn mở nhỏ gọn hỗ trợ lập trình viên nhanh chóng chuyển đổi các tệp bảng dữ liệu định dạng CSV thành tệp hình ảnh để tiện chèn vào các báo cáo.

2、[SAMIST: Ứng dụng GUI hỗ trợ cắt tách vật thể hình ảnh bằng AI](https://github.com/dibrale/samist)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052702.webp)

Ứng dụng desktop viết bằng Python cung cấp giao diện đồ họa trực quan kết nối với mô hình AI Segment Anything (SAM) của Meta, giúp người dùng dễ dàng nhấp chuột để tự động tách và trích xuất các vật thể bất kỳ ra khỏi bức ảnh chụp.

3、[git-sim: Tiện ích mô phỏng tác động của các lệnh Git bằng ảnh động](https://initialcommit.com/blog/git-sim)

Công cụ dòng lệnh hữu ích giúp lập trình viên trực quan hóa tác động của các lệnh Git (như merge, rebase) lên cấu trúc nhánh của kho chứa bằng cách tự động vẽ và xuất ra các tệp hình ảnh hoặc video hoạt họa minh họa:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012301.webp)

4、[Read Something: Tiện ích tối ưu hóa giao diện đọc web tích hợp AI](https://github.com/ReadSomething/ReadSomething)

Extension mã nguồn mở dành cho trình duyệt Chrome hỗ trợ trích xuất văn bản web sang chế độ đọc tinh giản (Reader Mode), đồng thời tích hợp sẵn các tính năng gọi AI viết tóm tắt nội dung, dịch thuật song ngữ và xuất tài liệu ra định dạng Markdown. (Đóng góp của [@zhongyiio](https://github.com/ruanyf/weekly/issues/3162))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060114.webp)

5、[MIB: Ứng dụng hỗ trợ sao lưu dữ liệu điện thoại Android lên PC](https://github.com/QC2168/mib)

Mã nguồn mở xây dựng ứng dụng Windows hỗ trợ người dùng dễ dàng kết nối và thực hiện sao lưu gia tăng (incremental backup) hình ảnh, danh bạ từ thiết bị di động Android sang máy tính lưu trữ một cách an toàn. (Đóng góp của [@QC2168](https://github.com/ruanyf/weekly/issues/3148))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060108.webp)

6\. [Rubic: Framework lập trình ứng dụng mini program theo kiến trúc Vue 3](https://rubic.jaskang.vip/)

Một framework hỗ trợ lập trình phát triển các ứng dụng nhỏ (mini programs) đa nền tảng, áp dụng mô hình quản lý trạng thái reactivity tương tự như Vue 3 giúp đơn giản hóa quy trình viết mã nguồn Front-end. (Đóng góp của [@JasKang](https://github.com/ruanyf/weekly/issues/3150))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060110.webp)

7、[SQLucky: Công cụ quản trị cơ sở dữ liệu trực quan viết bằng Java](https://github.com/tenie/SQLucky)

Hệ thống quản trị cơ sở dữ liệu trực quan nguồn mở hỗ trợ kết nối đa dạng các hệ quản trị CSDL phổ biến, là giải pháp miễn phí hoàn hảo thay thế cho các phần mềm thương mại đắt đỏ. (Đóng góp của [@tenie](https://github.com/ruanyf/weekly/issues/3154))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060112.webp)

8、[flutter_chatgpt: Ứng dụng client ChatGPT đa nền tảng viết bằng Flutter](https://github.com/bravekingzhang/flutter_chat_box)

Mã nguồn mở xây dựng ứng dụng giao diện trò chuyện với ChatGPT, được lập trình bằng framework Flutter hỗ trợ biên dịch chạy mượt mà trên cả thiết bị di động và máy tính. (Đóng góp của [@bravekingzhang](https://github.com/ruanyf/weekly/issues/3151))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060111.webp)

9、[IceCubesApp: Ứng dụng khách Mastodon chất lượng cao dành cho iOS](https://github.com/Dimillian/IceCubesApp)

Ứng dụng khách nguồn mở kết nối với mạng xã hội phi tập trung Mastodon dành riêng cho hệ điều hành iOS, sở hữu giao diện hiển thị mượt mà và đang được cộng đồng cập nhật tính năng liên tục.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012502.webp)

10、[Juice Shop: Ứng dụng web thử nghiệm rèn luyện kỹ năng bảo mật](https://github.com/juice-shop/juice-shop)

Một dự án huấn luyện an toàn thông tin của tổ chức OWASP, xây dựng một ứng dụng web bán hàng giả lập được tích hợp sẵn 10 lỗ hổng bảo mật kinh điển nhất để lập trình viên thực hành các kỹ thuật khai thác và vá lỗi bảo mật:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012503.webp)

## 资源

1、[Fluent 2: Ngôn ngữ thiết kế hệ thống thế hệ mới của Microsoft](https://fluent2.microsoft.design/)

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052804.webp)

Microsoft công bố phiên bản ngôn ngữ thiết kế Fluent 2 mới nhất, cung cấp bộ thư viện thành phần giao diện chuẩn hóa hỗ trợ lập trình viên xây dựng ứng dụng trên Web và iOS.

2\. [CS Study Roadmap: Sơ đồ lộ trình học tập ngành Khoa học Máy tính](https://hackway.org/docs/cs/intro)

Trang web tổng hợp và phân loại lộ trình học tập các kiến thức nền tảng của ngành Khoa học Máy tính (CS) chất lượng cao, được xây dựng dựa trên việc tham chiếu khung chương trình đào tạo của các trường đại học hàng đầu Mỹ. (Đóng góp của [@Stein283036](https://github.com/ruanyf/weekly/issues/3149))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060109.webp)

3\. [Docker and Kubernetes Guide: Giáo trình học Docker và K8s trực quan](https://www.bilibili.com/read/cv21266100)

Lớp học trực tuyến chất lượng về Docker và Kubernetes được chuyển ngữ phụ đề tiếng Trung, giúp lập trình viên nhanh chóng làm quen với việc đóng gói và triển khai ứng dụng Node.js lên cụm máy chủ container. (Đóng góp của [@lyf61](https://github.com/ruanyf/weekly/issues/3156))

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060113.webp)

4\. [Build Your Own Database: Hướng dẫn tự viết một cơ sở dữ liệu từ đầu](https://build-your-own.org/database/)

Cuốn sách kỹ thuật trực tuyến viết bằng tiếng Anh hướng dẫn lập trình viên cách thức tự viết mã lập trình xây dựng một hệ quản trị cơ sở dữ liệu và cấu trúc dữ liệu lưu trữ từ con số 0. Tác giả cũng có cuốn sách tương tự hướng dẫn [Tự viết lại Redis](https://build-your-own.org/redis/).

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042409.webp)

5\. [LLM University: Thư viện tài liệu học tập về mô hình ngôn ngữ lớn](https://docs.cohere.com/docs/llmu)

Trang web giáo trình trực tuyến miễn phí do Cohere xây dựng, cung cấp các bài viết lý thuyết và thực hành chi tiết giúp người học làm quen với cơ chế vận hành của các mô hình LLM.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052602.webp)

## 图片

1、**Bộ ảnh nghệ thuật chụp góc cao cảnh quan các bãi biển tại bang Florida**

Một nhiếp ảnh gia người Mỹ chuyên thực hiện các bộ ảnh chụp từ trên cao ghi lại khung cảnh rực rỡ sắc màu của các bãi biển đông đúc tại bang Florida, tạo nên những bức ảnh bố cục hình học rất đẹp mắt:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122202.webp)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122203.webp)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122204.webp)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122205.webp)

## ✍️ Bài đọc thêm

### Tại sao quy trình thiết kế và gỡ lỗi phần cứng (hardware) lại vô cùng khó khăn

Khoảng một năm trước, doanh nghiệp của chúng tôi liên tục nhận được báo cáo từ khách hàng về lỗi vận hành ngẫu nhiên rất kỳ lạ trên các robot công nghiệp do chúng tôi sản xuất.

Chúng tôi đã thu hồi các thiết bị lỗi về phòng thí nghiệm, cả đội ngũ kỹ sư phần cứng và phần mềm đã tiến hành hàng trăm bài kiểm thử hệ thống nhưng hoàn toàn không thể tái hiện lại lỗi của khách hàng.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060116.webp)

Sau nhiều ngày phân tích cấu trúc, chúng tôi đưa ra giả thuyết rằng nguyên nhân có thể do bộ khớp nối bánh xe bị lỏng khiến động cơ không thể truyền lực làm xoay bánh.

Do sản phẩm đã được phân phối rộng rãi trên thị trường và rất khó thu hồi hàng loạt, chúng tôi đã biên soạn hướng dẫn gửi cho các khách hàng tự mở nắp máy để siết chặt lại ốc khớp nối. Phương án này ghi nhận phản hồi tốt và sự cố ngẫu nhiên tạm thời biến mất. Chúng tôi đã yên tâm cho rằng lỗi đã được giải quyết dứt điểm suốt một năm sau đó.

Thế nhưng đến tháng trước, khi mùa đông lạnh giá ập đến, khách hàng lại tiếp tục báo cáo sự cố cũ quay trở lại.

Lần này chúng tôi tin chắc sự cố không nằm ở khớp nối. Thiết bị lỗi lại được thu hồi về phòng thí nghiệm. Trong điều kiện phòng ấm áp, robot hoạt động hoàn hảo và lỗi không xuất hiện.

Chỉ đến khi một kỹ sư đưa ra ý tưởng đặt robot vào trong tủ lạnh qua đêm, sáng hôm sau lấy ra chạy thử thì sự cố lập tức xuất hiện trở lại. Sau khoảng 10 phút để ở nhiệt độ phòng ấm lên, lỗi lại tự biến mất. Từ đó chúng tôi hiểu ra lỗi này có liên quan trực tiếp đến nhiệt độ môi trường.

Để gỡ lỗi triệt để, chúng tôi đã trưng dụng toàn bộ tủ lạnh đựng thức ăn của văn phòng để xếp đầy các cụm mạch của robot vào trong đó:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121801.webp)

Kết quả phân tích mạch điện cho thấy một linh kiện tụ điện bán dẫn trên bo mạch khi hoạt động ở nhiệt độ thấp sẽ sinh ra các dòng nhiễu tín hiệu tần số cao làm ngắt mạch điều khiển động cơ. Việc sửa lỗi rất đơn giản, chỉ cần tháo bỏ hai điện trở lọc nhiễu là xong.

Sự kiện năm ngoái lỗi tạm thời biến mất khi khách hàng tháo máy siết ốc thực chất do quá trình mở vỏ máy và thao tác tay của con người đã vô tình làm nhiệt độ cục bộ trong khoang máy ấm lên, khiến dòng nhiễu tạm thời biến mất chứ hoàn toàn không liên quan gì đến bộ khớp nối. Thêm vào đó, thời tiết mùa hè ấm áp sau đó cũng giúp lỗi không xuất hiện lại cho tới khi mùa đông năm nay quay lại.

Mẫu robot của chúng tôi có cấu trúc cơ khí rất đơn giản với chỉ vài trăm chi tiết linh kiện. Tuy nhiên chỉ cần một linh kiện siêu nhỏ gặp sự cố vật lý do tác động của nhiệt độ môi trường là đủ để gây ra lỗi hệ thống ngẫu nhiên cực kỳ khó chẩn đoán. Đây chính là lý do tại sao việc phát triển và bảo trì các sản phẩm phần cứng luôn khó khăn và rủi ro hơn nhiều so với phần mềm.

## Lịch sử tuần này

- 2022年（第 210 期）：[Lập trình: Phân tích các nguyên nhân cốt lõi khiến các dự án phần mềm ngày càng phình to và phức tạp](http://www.ruanyifeng.com/blog/2022/06/weekly-issue-210.html)
- 2021年（第 160 期）：[Sự nghiệp: Thảo luận về các thách thức và định hướng tháo gỡ khó khăn cho lập trình viên trung niên](http://www.ruanyifeng.com/blog/2021/05/weekly-issue-160.html)
- 2020年（第 110 期）：[Kinh tế số: Các cân nhắc lựa chọn sàn giao dịch thay thế khi doanh nghiệp không thể IPO tại Mỹ](http://www.ruanyifeng.com/blog/2020/06/weekly-issue-110.html)
- 2019年（第 60 期）：[Sách hay: Giới thiệu cuốn tự truyện khoa học phác họa lại chặng đường tiến hóa và nguồn gốc của loài người](http://www.ruanyifeng.com/blog/2019/06/weekly-issue-60.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs simplifies documents and workspaces.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
