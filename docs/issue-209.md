# 科技爱好者周刊（第 209 期）：程序员是怎样的人

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2426) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060910.webp)

Sân bay Vu Sơn Trùng Khánh nằm giữa những ngọn núi trập trùng bên cạnh danh thắng Tam Hiệp thuộc huyện Vu Sơn. Dự án đã phải san phẳng 7 ngọn núi và lấp đầy 6 thung lũng sâu để tạo ra 3.000 mẫu đất bằng phẳng ở độ cao hơn 1.700 mét so với mực nước biển. Sân bay có độ chênh lệch chiều cao thẳng đứng so với chân núi gần 1.000 mét, hành khách cần di chuyển dọc theo con đường đèo quanh co để lên đến đỉnh núi trước khi lên máy bay. (Nguồn: [Guancha](https://user.guancha.cn/wap/content?id=614529))

## 本周话题：程序员是怎样的人

Gần đây tôi có đọc về một thí nghiệm tâm lý học nổi tiếng mang tên "[Thí nghiệm nhà tù Stanford](https://moxie.org/2013/01/07/career-advice.html)" (Stanford Prison Experiment) năm 1971 và muốn chia sẻ vài góc nhìn cùng các bạn.

Năm 1971, một nhà tâm lý học người Mỹ đã thiết lập một mô hình nhà tù giả định tại tầng hầm của khoa Tâm lý học thuộc Đại học Stanford.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060818.webp)

Ông tuyển chọn một nhóm tình nguyện viên bình thường, cho họ tung đồng xu để phân chia ngẫu nhiên: một nửa đóng vai tù nhân và một nửa đóng vai cai ngục. Những tình nguyện viên này đều chưa từng tiếp xúc với môi trường nhà tù trước đó và cũng không được hướng dẫn cách thức nhập vai chi tiết.

Ban đầu, mọi người đều tỏ ra lóng ngóng, gượng gạo và cảm thấy trò chơi này có phần nực cười.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060821.webp)

Tuy nhiên, chỉ sau một thời gian ngắn, mọi thứ bắt đầu thay đổi nhanh chóng. Những người đóng vai tù nhân dần quên đi danh tính thực tế bên ngoài, họ bắt đầu đứng trên lập trường của tù nhân để suy nghĩ. Họ rơi vào trạng thái căng thẳng, bỏ ăn, bắt đầu phản kháng "cai ngục" và đổ lỗi lẫn nhau.

Trong khi đó, những người đóng vai cai ngục cũng bắt đầu hành xử như cai ngục thực thụ: thiết lập phòng biệt giam, áp đặt các hình phạt tâm lý, răn đe tù nhân và tuần tra hành lang với dùi cui trên tay.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060820.webp)

Điều đáng ngạc nhiên nhất là sau hai ngày, khi nhà nghiên cứu thử hoán đổi vai trò giữa hai nhóm, các tình nguyện viên lập tức thích nghi với vai diễn mới và thay đổi hành vi tương ứng một cách nhanh chóng.

Do các tình nguyện viên nhập vai quá mức dẫn đến những diễn biến tâm lý căng thẳng ngoài tầm kiểm soát, thí nghiệm dự kiến kéo dài hai tuần đã phải tuyên bố dừng lại ngay vào ngày thứ sáu.

Nhà nghiên cứu rút ra kết luận quan trọng từ thí nghiệm này: **Hành vi của con người bị định hình mạnh mẽ bởi môi trường làm việc. Bạn sẽ dần trở thành người mà môi trường yêu cầu bạn trở thành.** Một người bình thường khi bị đưa vào môi trường tù tội sẽ trở nên cam chịu hoặc lén lút phòng vệ; ngược lại khi nắm quyền cai trị, họ dễ trở nên hống hách, độc đoán.

Bài học rút ra là: **Hãy cẩn thận với công việc của bạn, bởi nó sẽ thay đổi tính cách và biến bạn thành một con người khác.** Chúng ta thường có định kiến rằng kế toán thường kỹ tính, nhạy cảm với tiền bạc; luật sư luôn ưu tiên tối ưu hóa lợi ích pháp lý; hay nhân viên hải quan luôn nhìn mọi người với ánh mắt hoài nghi. Đó chính là sự định hình tính cách do nghề nghiệp mang lại.

Điều này khiến tôi tự hỏi: Nghề lập trình viên sẽ thay đổi tính cách của một người như thế nào?

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060822.webp)

Tôi nghĩ có một số đặc điểm tính cách sau dễ hình thành ở lập trình viên:

**1. Thói quen đơn thương độc mã tự giải quyết vấn đề:** Lập trình về bản chất là công việc cá nhân. Bạn không thể viết chung một hàm với người khác theo kiểu người viết đoạn đầu, người viết đoạn sau. Quy trình làm việc nhóm trong phát triển phần mềm thực chất là sự ráp nối các phần việc đã được phân chia độc lập cho từng cá nhân trước đó.

**2. Quen thuộc với sự cô đơn:** Lập trình đòi hỏi sự tập trung cao độ, ngày qua ngày tương tác chủ yếu với máy tính và rất ít khi giao tiếp trực tiếp với người khác. Trong các đợt chạy tiến độ dự án, việc cả ngày không nói chuyện với ai là điều bình thường.

**3. Cực kỳ tỉ mỉ và cẩn trọng:** Mọi chi tiết logic đều phải được xử lý chính xác tuyệt đối. Một ký tự sai, một dấu chấm phẩy thiếu hoặc một điều kiện logic sai lệch nhỏ cũng có thể khiến toàn bộ chương trình lỗi hoặc tạo ra các lỗ hổng bảo mật nghiêm trọng.

**4. Khả năng chịu đựng áp lực tâm lý cao:** Đây là công việc có áp lực tiến độ lớn. Lỗi hệ thống phát sinh đột ngột trên production trong khi khách hàng và quản lý liên tục thúc giục sẽ dễ khiến lập trình viên rơi vào trạng thái căng thẳng tột độ.

Tóm lại, nếu một người chọn theo nghề lập trình từ sớm khi tính cách chưa hoàn toàn định hình, họ có xu hướng trở thành người: thích làm việc độc lập, quen chịu đựng sự cô đơn, chú trọng chi tiết tỉ mỉ và chịu được áp lực cao. Nếu bạn cảm thấy mình sẵn sàng đón nhận những thay đổi tính cách này, bạn hoàn toàn có thể tự tin theo đuổi nghề lập trình viên.

## 个人如何提高抗风险能力

Trước dịp Tết Đoan Ngọ, thầy Tôn Minh Triển, nhà sáng lập công ty tư vấn tài chính Phổ Lam (Trussan) đã liên hệ giới thiệu chương trình hỗ trợ quản lý tài chính cá nhân dành cho độc giả bản tin.

Thầy Tôn là chuyên gia có hơn 30 năm kinh nghiệm trong ngành tài chính. Ông tốt nghiệp Thạc sĩ khoa Thống kê tại Đại học Trung Sơn và từng giữ các vị trí quản lý tại các tập đoàn bảo hiểm thuộc Fortune 500 trước khi sáng lập thương hiệu tư vấn tài chính Phổ Lam. Doanh nghiệp hiện đã vận hành hơn 10 năm và vừa hoàn thành vòng gọi vốn Series B thành công. Bạn đọc quan tâm có thể tìm hiểu thêm tại [Trang chủ Phổ Lam](http://www.trussan.com/about#company_detail).

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060401.webp)

Bên cạnh công việc kinh doanh, thầy Tôn cũng tham gia giảng dạy hệ thạc sĩ chuyên nghiệp tại Đại học Trung Sơn và duy trì viết bài chia sẻ kiến thức tài chính trên kênh tài khoản cá nhân của mình.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060403.webp)

Trong bối cảnh nền kinh tế có nhiều biến động ảnh hưởng tới nhiều ngành nghề (như bán lẻ, giáo dục, công nghệ), chương trình lần này tập trung vào chủ đề **"Làm thế nào để cá nhân nâng cao năng lực phòng ngừa rủi ro tài chính"**.

Để nâng cao năng lực kháng rủi ro tài chính, về cơ bản cần thực hiện tốt 3 yếu tố:
1. **Duy trì nguồn thu nhập ổn định:** Đến từ tiền lương công việc hoặc lợi nhuận từ các tài sản tích lũy.
2. **Phòng ngừa rủi ro chủ động:** Thiết lập và duy trì dòng tiền dự phòng hợp lý cho các tình huống khẩn cấp.
3. **Phân bổ tài sản khoa học:** Đầu tư tích lũy giúp tài sản bảo tồn giá trị và tăng trưởng bền vững trước lạm phát.

Tuy nhiên, các sản phẩm tài chính hay bảo hiểm hiện nay thường có cấu trúc điều khoản miễn trừ phức tạp khiến người dùng phổ thông khó đưa ra lựa chọn tối ưu.

Chương trình lần này cung cấp dịch vụ tư vấn 1-1 miễn phí từ các chuyên gia tài chính của Phổ Lam giúp bạn thiết lập lộ trình phân bổ tài sản an toàn:

Đầu tiên, các chuyên gia sẽ hỗ trợ phân tích sức khỏe tài chính gia đình, xây dựng bảng cân đối tài sản và chỉ ra các lỗ hổng rủi ro hiện có:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060406.webp)

Sau đó, họ sẽ đề xuất giải pháp phân bổ tỷ lệ dòng tiền tích lũy vào các kênh tiết kiệm, đầu tư, bảo hiểm phù hợp với nhu cầu hưu trí hoặc chuẩn bị quỹ giáo dục cho con cái:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060405.webp)

Bản kế hoạch phân bổ tài sản chi tiết sẽ được giải thích rõ ràng và khách quan bởi đội ngũ tư vấn viên chuyên nghiệp.

Độc giả của bản tin được đăng ký trải nghiệm miễn phí gói dịch vụ tư vấn tài chính này từ Phổ Lam, đồng thời 100 người đăng ký đầu tiên sẽ được tặng kèm cuốn cẩm nang hướng dẫn quản lý tài chính gia đình.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060407.webp)

Bạn đọc quan tâm có thể quét mã QR phía trên để tìm hiểu thông tin chi tiết và đăng ký tham gia chương trình (giới hạn 200 lượt đăng ký).

## 科技动态

1、[Sony đăng ký bằng sáng chế biến quả chuối thành tay cầm chơi game](https://www.businessinsider.com/sony-patents-new-system-converts-bananas-into-game-playstation-controllers-2021-3)

Tập đoàn Sony vừa nộp hồ sơ đăng ký bằng sáng chế cho giải pháp biến các vật dụng gia đình thông thường thành thiết bị điều khiển trò chơi PlayStation:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032014.webp)

Hồ sơ mô tả việc sử dụng một quả chuối làm ví dụ minh họa, người dùng cầm quả chuối và nhấn vào các nút bấm ảo trên bề mặt của nó để điều khiển nhân vật. Bằng sáng chế ghi nhận giải pháp này cũng có thể áp dụng tương tự trên quả cam, cốc cà phê hay cây bút viết.

Hệ thống hoạt động dựa trên một camera gắn ngoài theo dõi và phân tích vị trí chuyển động ngón tay của người dùng để dịch mã thành các lệnh điều khiển game tương ứng. Giải pháp này hướng tới việc hỗ trợ chơi game nhiều người khi thiếu tay cầm vật lý tại các buổi tụ họp gia đình.

2、[Vận hành tàu nuôi cá xa bờ quy mô lớn nhất thế giới](http://www.stdaily.com/index/kejixinwen/202205/43bff4a13a274dc6a6f31ff9abd0baf7.shtml)

Để nuôi trồng các loài cá có giá trị kinh tế cao (như cá đù vàng, cá song, cá hồi) vốn không phù hợp với môi trường nuôi sát bờ, một doanh nghiệp tại Thanh Đảo đã chế tạo con tàu nuôi cá xa bờ mang tên "Quốc Tín số 1" với tải trọng đạt 100.000 tấn:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053101.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053102.webp)

Tàu có chiều dài 250 mét, dự kiến cung cấp sản lượng cá nuôi đạt 3.700 tấn mỗi năm. Hệ thống trên tàu liên tục bơm tuần hoàn nước biển tự nhiên để duy trì chất lượng nước nuôi tối ưu, giúp cá sinh trưởng tốt và tránh được các thiên tai như bão biển hay hiện tượng thủy triều đỏ sát bờ.

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053103.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053104.webp)

Toàn bộ các thông số nhiệt độ, lượng oxy và phân bổ thức ăn trong các khoang nuôi đều được điều khiển tự động. Doanh nghiệp dự kiến sẽ đưa vào vận hành tiếp hai tàu "Quốc Tín số 2" và "Quốc Tín số 3" trong vòng hai năm tới.

3、[Đại học Thanh Hoa chế tạo robot siêu nhỏ kiểm tra đường ống cơ khí](https://www.tsinghua.edu.cn/info/1175/95080.htm)

Đội ngũ nghiên cứu khoa Cơ khí Đại học Thanh Hoa vừa chế tạo thành công mẫu robot siêu nhỏ phục vụ kiểm tra đường ống kỹ thuật:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060305.webp)

Robot có đường kính chưa đầy 1cm, dài 4,7cm và chỉ nặng 2,2g nhưng được tích hợp đầy đủ hệ thống truyền động, pin nguồn, camera siêu nhỏ và bộ thu phát tín hiệu không dây.

Mẫu robot này có thể di chuyển tiến lùi, chuyển hướng linh hoạt theo lệnh điều khiển với tốc độ 5cm/giây và có khả năng uốn dẻo để len lỏi qua các đoạn ống cong hẹp. Thiết bị hướng tới ứng dụng kiểm tra các vết nứt hỏng bên trong đường ống động cơ máy bay phản lực.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060304.webp)

4、[Liên minh Châu Âu thống nhất áp dụng chuẩn sạc USB Type-C](https://www.europarl.europa.eu/news/en/press-room/20220603IPR32196/deal-on-common-charger-reducing-hassle-for-consumers-and-curbing-e-waste)

Liên minh Châu Âu (EU) vừa thông qua dự luật yêu cầu tất cả các thiết bị điện tử di động cỡ nhỏ và trung bình bán ra tại thị trường EU bắt buộc phải chuyển sang sử dụng cổng sạc chuẩn USB Type-C từ mùa thu năm 2024:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060805.webp)

Quy định áp dụng cho điện thoại di động, máy tính bảng, máy đọc sách, tai nghe không dây, máy ảnh kỹ thuật số và máy chơi game cầm tay. Riêng máy tính xách tay sẽ có thời hạn chuyển đổi chậm hơn là 40 tháng.

Mục tiêu của dự luật nhằm giảm thiểu lượng rác thải điện tử (ước tính khoảng 11.000 tấn sạc cũ bị thải bỏ hàng năm tại EU) và giúp người tiêu dùng tiết kiệm khoảng 250 triệu Euro chi phí mua sạc mới mỗi năm. Apple sẽ là hãng chịu ảnh hưởng lớn nhất từ quy định này, tuy nhiên do luật không cấm sạc không dây, Apple hoàn toàn có thể lựa chọn loại bỏ hoàn toàn cổng sạc vật lý trên iPhone trong tương lai.

5、[Nghiên cứu ứng dụng băng dán điện tử hỗ trợ làm lành vết thương nhanh](https://newatlas.com/medical/epatch-bandage-speeds-healing/)

Phương pháp sử dụng dòng điện cực nhỏ để diệt khuẩn và kích thích tái tạo tế bào da đã được chứng minh hiệu quả trong y học. Các nhà khoa học Mỹ đã phát triển loại băng dán điện tử hydrogel tích hợp mạng lưới dây nano bạc siêu nhỏ dẫn điện:

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022042501.webp)

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022042502.webp)

Khi kết nối với nguồn phát điện nhẹ bên ngoài, băng dán sẽ tạo ra luồng điện phân bổ đều trên bề mặt vết thương. Chất liệu nano bạc giúp kháng khuẩn tự nhiên và tránh gây bám dính khi tháo băng. Thử nghiệm lâm sàng trên chuột cho thấy vết thương sử dụng băng điện tử chỉ mất 7 ngày để lành hoàn toàn so với 20 ngày của nhóm đối chứng.

## 文章

1、[Phân tích làn sóng khởi nghiệp thiết kế chip GPU tại thị trường trong nước](https://www.latepost.com/news/dj_detail?id=1166)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060806.webp)

Thị trường chip đồ họa độc lập (dGPU) hiện nay hầu như bị độc quyền bởi Nvidia và AMD do rào cản công nghệ cực cao. Bài viết phân tích nguyên nhân và cơ hội giúp hàng loạt startup thiết kế GPU trong nước thu hút được dòng vốn đầu tư lớn trong thời gian qua.

2、[Dịch vụ tra cứu nhanh các tài khoản liên kết số điện thoại di động](https://www.sohu.com/a/555332422_120388781)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060901.webp)

Viện Công nghệ thông tin Trung Quốc ra mắt cổng dịch vụ hỗ trợ người dùng tra cứu nhanh danh sách các tài khoản mạng xã hội (như Weibo, Taobao, Douyin, Meituan) đang liên kết với số điện thoại cá nhân và hỗ trợ tính năng hủy liên kết nhanh để bảo mật thông tin.

3、[Bài viết ngắn giới thiệu tổng quan về tài sản số NFT và ứng dụng thực tế](https://mp.weixin.qq.com/s/IwbB4ZwPn-8xSHlAY9EIRA)（Tiếng Trung）

Bài viết giải thích bằng ngôn ngữ phổ thông dễ hiểu về bản chất của mã thông báo không thể thay thế (NFT), cách thức hoạt động của công nghệ blockchain đi kèm và xu hướng ứng dụng dưới dạng các bộ sưu tập số trong nước.

4、[Giới thiệu một số thuộc tính thẻ HTML hữu ích ít được lập trình viên sử dụng](https://www.smashingmagazine.com/2022/03/html-attributes-you-never-use/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022040501.jpg)

Bài viết hướng dẫn chi tiết cách ứng dụng một số thuộc tính HTML hữu ích như thuộc tính `enterkeyhint` trên thẻ `<input>` giúp thay đổi hiển thị nút Enter trên bàn phím ảo của thiết bị di động.

5、[Chia sẻ 3 mẹo nhỏ hữu ích khi soạn thảo tài liệu bằng Markdown](https://www.stefanjudis.com/blog/three-markdown-tricks-i-just-learned/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202112/bg2021120807.webp)

Hướng dẫn một số mẹo nhỏ khi định dạng văn bản Markdown, tiêu biểu là cách hiển thị ký tự dấu nháy ngược (backticks) ngay bên trong một đoạn mã inline code block.

6、[Hướng dẫn thao tác đọc ghi dữ liệu từ clipboard thông qua dòng lệnh Terminal](https://letterstoanewdeveloper.com/2021/03/15/use-the-clipboard-from-the-command-line/)（Tiếng Anh）

Cả Windows và macOS đều cung cấp sẵn các lệnh CLI hỗ trợ người dùng đọc hoặc ghi nội dung văn bản vào bộ nhớ tạm (clipboard) của hệ thống. Bài viết hướng dẫn các câu lệnh cơ bản phục vụ cho việc tự động hóa script.

7、[So sánh chất lượng tạo ảnh từ mô tả văn bản giữa mô hình Imagen và DALL-E](https://threadreaderapp.com/thread/1529510695452164097.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022052702.webp)

Tác giả tiến hành thử nghiệm nhập cùng một câu mô tả chi tiết (ví dụ: *"Một chú chim màu xanh đứng trên giỏ bánh macaron sắc màu cầu vồng"*) vào hai mô hình AI tạo ảnh hàng đầu hiện nay là Imagen của Google và DALL-E của OpenAI để đánh giá độ chi tiết và tính chân thực của bức ảnh xuất ra.

8、[Hướng dẫn sử dụng công cụ dòng lệnh dig tra cứu thông tin hệ thống DNS](https://jvns.ca/blog/2021/12/04/how-to-use-dig/)（Tiếng Anh）

Bài viết hướng dẫn lập trình viên sử dụng công cụ dòng lệnh `dig` để truy vấn thông tin phản hồi từ máy chủ DNS, kiểm tra các bản ghi phân giải tên miền (A record, CNAME, MX record) một cách chi tiết.

9、[Hướng dẫn cơ bản so sánh chính xác số thực dấu phẩy động trong Python](https://davidamos.dev/the-right-way-to-compare-floats-in-python/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022033116.webp)

Bài viết hướng dẫn lập trình viên mới làm quen cách xử lý sai số làm tròn số thực dấu phẩy động (float precision) trong Python và cách sử dụng hàm `math.isclose()` để so sánh dữ liệu số thực chính xác.

## 工具

1、[WeekToDo: Phần mềm quản lý danh sách công việc cần làm hàng tuần tối giản](https://weektodo.me/)

Ứng dụng quản lý công việc (todo list) thiết kế giao diện dạng cột chia theo các ngày trong tuần giúp người dùng dễ dàng lên lịch trình công việc trực quan, hỗ trợ đầy đủ bản cài đặt máy tính và bản Web.

2、[Xournal: Phần mềm ghi chép viết tay hỗ trợ công thức toán học trên Linux](http://xournal.sourceforge.net/)

Phần mềm ghi chú mã nguồn mở tối ưu cho hệ điều hành Linux hỗ trợ nhập liệu viết tay, vẽ sơ đồ hình học và chèn các công thức toán học phù hợp khi kết hợp với bảng vẽ điện tử (graphics tablet).

3、[go-zero: Framework microservice hiệu năng cao viết bằng Go](https://github.com/zeromicro/go-zero)

Hệ thống framework tích hợp sẵn các công cụ quản lý tải, kiểm soát giới hạn băng thông (rate limiting) và sinh mã nguồn tự động hỗ trợ lập trình viên xây dựng hệ thống microservices tin cậy trên ngôn ngữ Go. (Đóng góp của [@kevwan](https://github.com/ruanyf/weekly/issues/2430))

4、[SiYuan: Hệ thống quản lý tri thức cá nhân hỗ trợ soạn thảo dạng khối block](https://github.com/siyuan-note/siyuan/blob/master/README_zh_CN.md)

Công cụ quản lý ghi chú cá nhân nội địa hỗ trợ soạn thảo văn bản markdown trực quan, sơ đồ liên kết ý tưởng và lưu trữ local an toàn (tính năng đồng bộ đám mây đa thiết bị yêu cầu đăng ký trả phí). (Đóng góp của [@Geo123abc](https://github.com/ruanyf/weekly/issues/2424))

5、[AI Doc Writer: Plugin hỗ trợ tự động viết chú thích code thông minh](https://www.mintlify.com/)

Plugin dành cho VS Code và các IDE của JetBrains hỗ trợ phân tích hàm code đang chọn để tự động sinh ra đoạn chú thích tài liệu chuẩn hóa (Javadoc, Docstring) cho nhiều ngôn ngữ lập trình.

6、[SwiftBar: Tiện ích tùy biến menu bar đa dạng widget cho macOS](https://github.com/swiftbar/SwiftBar)

Công cụ nguồn mở hỗ trợ lập trình viên viết script tùy biến nội dung hiển thị trên thanh menu bar của máy Mac thông qua kho widget phong phú có sẵn.

7、[BiglyBT: Trình tải tệp tin torrent nguồn mở tích hợp nhiều tính năng nâng cao](https://www.biglybt.com/)

Phần mềm máy tính hỗ trợ tải tệp torrent đa nền tảng cung cấp đầy đủ các biểu đồ thống kê băng thông, phân tích nguồn chia sẻ và tối ưu hóa kết nối mạng.

8、[Lemon Design: Bộ React component thiết kế dựa trên Tailwind CSS](https://lemondesign.dev/)

Thư viện các thành phần giao diện UI (components) thiết kế sẵn tối giản, hiện đại dành cho lập trình viên xây dựng nhanh giao diện website React kết hợp Tailwind CSS.

9、[Mizu: Tiện ích theo dõi lưu lượng mạng giữa các microservices trên Kubernetes](https://github.com/up9inc/mizu)

Công cụ hỗ trợ nhà quản trị hệ thống giám sát và phân tích chi tiết các gói tin dữ liệu API truyền qua lại giữa các container microservice đang vận hành trong cụm Kubernetes.

10、[Freeplane: Phần mềm thiết kế sơ đồ tư duy đa nền tảng](https://www.freeplane.org/)

Ứng dụng máy tính nguồn mở hỗ trợ người dùng phác thảo nhanh các ý tưởng, lập sơ đồ tư duy phân cấp và quản lý hệ thống thông tin cá nhân.

## 资源

1、[Museum of Endangered Sounds: Trang web lưu trữ các âm thanh công nghệ cũ](http://savethesounds.info/)

Trang web lưu trữ độc đáo tập hợp các âm thanh của các thiết bị công nghệ cũ đang dần biến mất trong đời sống hiện đại như tiếng gõ bàn phím cơ thế hệ cũ, tiếng máy in kim chạy hay tiếng nhạc khởi động của Windows 95.

2、[Markov Chains for Programmers: Sách điện tử giới thiệu lý thuyết chuỗi Markov](https://czekster.github.io/markov/)

Cuốn sách điện tử chia sẻ miễn phí cung cấp các kiến thức toán học nền tảng về chuỗi Markov và các bài toán mô phỏng thuật toán ứng dụng thực tế dành cho lập trình viên.

3、[pianos.pub: Bản đồ định vị các địa điểm đặt đàn piano công cộng](https://pianos.pub/)

Chuyên trang cập nhật bản đồ định vị hơn 8.391 địa điểm đặt các cây đàn piano công cộng trên khắp các thành phố lớn trên thế giới phục vụ những người yêu âm nhạc ghé qua biểu diễn tự do.

4、[Think DSP: Giáo trình xử lý tín hiệu số ứng dụng ngôn ngữ Python](https://github.com/AllenDowney/ThinkDSP)

Cuốn sách điện tử nguồn mở giới thiệu các kiến thức cơ bản về xử lý tín hiệu số (Digital Signal Processing) dành cho người mới thông qua các ví dụ thực hành viết bằng mã nguồn Python.

5、[New Language Features in Java 8 to 17: Tổng hợp các cải tiến cú pháp Java](https://advancedweb.hu/new-language-features-since-java-8-to-17/)（Tiếng Anh）

Bài viết tổng hợp và giải thích chi tiết các đặc tính cú pháp mới nổi bật được bổ sung qua từng phiên bản phát hành của ngôn ngữ lập trình Java từ thế hệ Java 8 đến Java 17.

## 图片

1\. [Mô phỏng thói quen đọc sách chủ động và tương tác hiệu quả](https://dkb.io/post/how-to-read-a-book)

Đa số mọi người có thói quen đọc sách thụ động theo kiểu: đọc dòng chữ -> hiểu ý nghĩa -> lưu thông tin vào não (đọc một chiều):

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021601.webp)

Tuy nhiên, phương pháp đọc sách chủ động giúp tiếp thu tri thức hiệu quả hơn được mô tả theo sơ đồ: đọc dòng chữ -> đặt câu hỏi phản biện -> quay lại tra cứu tìm kiếm câu trả lời trong trang sách -> đúc kết tri thức:

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021602.webp)

2\. [Chân dung tả thực các nhân vật hoạt hình Disney qua nét vẽ của công nghệ AI](https://www.cartoonbrew.com/tech/artists-uses-ai-to-create-photorealistic-versions-of-disney-and-simpsons-characters-213045.html)

Một nghệ sĩ người Brazil ứng dụng thuật toán học máy tái hiện hình ảnh chân dung đời thực của các nhân vật phim hoạt hình nổi tiếng:

*(Nhân vật Aladdin)*

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021904.webp)

*(Nhân vật Hoa Mộc Lan)*

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021905.webp)

*(Nhân vật cụ ông Carl Fredricksen trong phim Up)*

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021906.webp)

*(Nhân vật Thủy thủ Mặt Trăng Usagi Tsukino)*

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022021908.webp)

## 💡 Bài đọc thêm

### Phân tích triển vọng ứng dụng xe tăng chiến đấu chạy động cơ điện

Xe tăng vốn là phương tiện chiến đấu bọc thép hạng nặng đòi hỏi độ bền bỉ cao trong các điều kiện chiến trường khắc nghiệt, khiến nhiều người cho rằng động cơ điện không phù hợp cho phương tiện này.

![](https://cdn.beekka.com/blogimg/asset/202202/bg2022020613.webp)

Tuy nhiên, động cơ điện thực tế sở hữu nhiều ưu điểm chiến thuật vượt trội phù hợp ứng dụng trên xe tăng:

1. **Khả năng tự chủ nguồn sạc:** Quân đội có thể mang theo các lò phản ứng hạt nhân di động quy mô nhỏ ngoài tiền tuyến để sạc pin cho các xe tăng vào ban đêm mà không cần xây dựng hệ thống cung cấp nhiên liệu hóa thạch cồng kềnh.
2. **Tối ưu hóa công tác hậu cần:** Một sư đoàn thiết giáp hành quân tiêu thụ hàng triệu lít nhiên liệu mỗi ngày. Việc vận chuyển dầu tiếp tế qua các vùng chiến sự luôn đối mặt với rủi ro bị phục kích lớn. Động cơ điện giúp loại bỏ hoàn toàn sự phụ thuộc này.
3. **Đơn giản hóa quy trình bảo trì:** Xe tăng điện có kết cấu ít chi tiết cơ học chuyển động hơn, không cần thay dầu bôi trơn định kỳ và ít bị mài mòn linh kiện động cơ hơn so với động cơ diesel truyền thống.
4. **Thiết kế phân rã mô-đun an toàn:** Hệ thống điện có thiết kế dạng mô-đun cho phép nhanh chóng tháo lắp sửa chữa ngoài thực địa. Một xe tăng điện có thể trang bị nhiều động cơ độc lập phân bổ ở các bánh xích và nhiều khoang chứa pin riêng biệt giúp xe duy trì khả năng di chuyển ngay cả khi một vài mô-đun bị trúng đạn phá hủy.
5. **Gia tăng mô-men xoắn tăng tốc nhanh:** Động cơ điện cho khả năng đạt mô-men xoắn cực đại tức thì giúp xe tăng nhanh chóng bứt tốc né tránh hỏa lực tầm xa.
6. **Khả năng lội nước sâu:** Động cơ điện không cần ống hút khí nạp hay khí thải như động cơ đốt trong giúp xe tăng điện có thể di chuyển chìm hoàn toàn dưới lòng sông sâu dễ dàng.
7. **Khả năng ẩn mình tối ưu:** Xe tăng điện vận hành cực kỳ êm ái không phát ra tiếng ồn động cơ và có mức tỏa nhiệt hồng ngoại cực thấp giúp xe tránh được các hệ thống camera tầm nhiệt tầm xa của đối phương.

Rào cản lớn nhất hiện nay là việc phát triển các dòng pin thể rắn (solid-state battery) có độ an toàn cao chống cháy nổ tốt khi bị trúng đạn và tối ưu hóa chi phí chế tạo đắt đỏ. Tuy nhiên, sự xuất hiện của các phương tiện chiến đấu tự hành, drone chạy điện hiện nay cho thấy sự hiện diện của xe tăng điện trên chiến trường tương lai chỉ là vấn đề thời gian.

## 历史上的本周

- 2021年（第 161 期）：[Thảo luận định hướng giáo dục: Xu hướng cắt giảm chỉ tiêu hệ đào tạo Thạc sĩ học thuật](https://www.ruanyifeng.com/blog/2021/06/weekly-issue-161.html)
- 2020年（第 110 期）：[Phân tích kinh tế: Lựa chọn hướng đi của các startup công nghệ khi gặp khó khăn niêm yết tại thị trường Mỹ](https://www.ruanyifeng.com/blog/2020/06/weekly-issue-110.html)
- 2019年（第 59 期）：[Góc nhìn xã hội: Tại sao việc xây dựng các mối quan hệ bạn bè bền vững trong kỷ nguyên Internet ngày càng khó khăn?](https://www.ruanyifeng.com/blog/2019/06/weekly-issue-59.html)
- 2018年（第 8 期）：[Thảo luận công nghệ y học: Liệu các đột phá trong phòng thí nghiệm sinh học có thể tạo ra con người nhân tạo trong tương lai?](https://www.ruanyifeng.com/blog/2018/06/weekly-issue-8.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
