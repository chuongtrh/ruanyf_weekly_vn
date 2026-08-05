# 科技爱好者周刊：第 85 期 (Bản tin chia sẻ công nghệ số 85)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112509.jpg)

Ảnh bìa: Các tòa nhà chung cư rực rỡ sắc màu, Istanbul, Thổ Nhĩ Kỳ. Ảnh từ [The Guardian](https://www.theguardian.com/artanddesign/gallery/2019/nov/23/the-kaleidoscopic-patterns-of-turkeys-architecture-in-pictures).

## 刊首语 (Lời tựa)

Gần đây, tôi có xem một [video bài giảng](https://youtube.com/watch?v=oNThpVzjM00) của một vị giáo sư chia sẻ về những cảm nhận thực tế của ông khi đến thăm nước Mỹ.

Ông nhận xét rằng, nước Mỹ thu hút mọi tầng lớp xã hội từ khắp nơi trên thế giới đổ về: từ giới tinh hoa học thuật, doanh nhân thành đạt cho tới những người tị nạn nghèo khổ ở tầng đáy. Là quốc gia nhập cư lớn nhất hành tinh, bạn có thể dễ dàng bắt gặp bất kỳ mảnh ghép văn hóa, tôn giáo hay bối cảnh xã hội đặc thù nào ngay trên đất Mỹ.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120406.jpg)

Cấu trúc xã hội Mỹ vô cùng phức tạp và hỗn tạp, nhưng điều kỳ lạ là nó không hề rơi vào trạng thái hỗn loạn. Về mặt lý thuyết, việc tập hợp hàng vạn con người khác biệt về tư duy, sắc tộc, vốn thường xuyên xung đột quyền lợi như vậy đáng lẽ ra phải biến xã hội thành một đống hỗn độn mới đúng. Thế nhưng, thực tế là ngay cả những dân tộc vốn có lịch sử thù hằn sâu sắc ở quê nhà vẫn có thể chung sống hòa bình và hợp tác cùng nhau trên đất Mỹ. Hệ thống vận hành của xã hội Mỹ cực kỳ quy củ và có trật tự, tại sao lại như vậy?

Vị giáo sư lý giải rằng nguyên nhân cốt lõi nằm ở việc nước Mỹ xây dựng một bộ quy tắc vận hành cực kỳ tối giản, dễ hiểu và dễ tiếp cận cho tất cả mọi người, giúp cắt giảm tối đa chi phí thấu hiểu xã hội. Quy luật gốc rễ của xã hội Mỹ có thể đúc kết ngắn gọn trong một câu: Về chính trị, vận hành theo cơ chế bầu cử dân chủ - bên nào nhiều phiếu hơn thì bên đó nắm quyền lực điều hành; Về kinh tế, vận hành theo cơ chế cạnh tranh tự do - sản phẩm của bên nào tốt hơn thì bên đó giành được thị trường và kiếm tiền.

Mọi hoạt động của xã hội đều xoay quanh trục quy tắc cơ bản dễ hiểu này, mang lại tính khả thi và độ nhất quán cực kỳ cao. Đương nhiên, hệ thống luật pháp bổ trợ của Mỹ cực kỳ chi tiết và phức tạp bậc nhất thế giới, nhưng toàn bộ các điều luật con đó đều chỉ phục vụ duy nhất một mục tiêu: bảo vệ tính thực thi nghiêm túc của bộ quy tắc gốc kể trên. Khi mọi người nhập cư đặt chân đến Mỹ, chỉ cần hiểu và tuân thủ đúng bộ quy tắc này là có thể nhanh chóng hòa nhập. Khi tất cả mọi người đều hành xử theo cùng một bộ quy tắc chung, chi phí giao tiếp và phối hợp xã hội sẽ giảm đi đáng kể, giúp bộ máy chính phủ vận hành hiệu quả và tiết kiệm chi phí quản lý tối đa.

Mở rộng tư duy này, mỗi cá nhân và doanh nghiệp hoàn toàn có thể tham khảo áp dụng. Hãy cố gắng tối giản hóa các nguyên tắc sống cá nhân và quy định vận hành của doanh nghiệp, cuộc sống và công việc tự khắc sẽ trở nên nhẹ nhàng và hiệu quả hơn rất nhiều.

## Khóa học lập trình Vue.js miễn phí

Vue.js hiện đang là một trong những framework lập trình giao diện JavaScript phổ biến hàng đầu tại thị trường Việt Nam và Trung Quốc, với nhu cầu tuyển dụng kỹ sư vô cùng lớn. Nhờ ưu điểm dễ tiếp cận, tài liệu tiếng Trung/tiếng Anh phong phú và khả năng triển khai nhanh cho các dự án quy mô vừa và nhỏ, Vue thường là lựa chọn hàng đầu của các lập trình viên mới bắt đầu học frontend. Hệ sinh thái của Vue cũng vô cùng hoàn thiện với các công cụ đi kèm như Vuex, Vue-Router, Element UI, Element-Admin.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120504.jpg)

Dưới đây là hai bộ video bài giảng chuyên sâu về Vue.js hoàn toàn miễn phí được đối tác đào tạo Kaikeba dành tặng riêng cho độc giả bản tin:

Bộ bài giảng thứ nhất: **《Làm chủ kỹ năng lập trình Vue thực chiến》**. Nội dung bao gồm: Kiến thức nền tảng Vue, hướng dẫn sử dụng công cụ khởi tạo dự án Vue-CLI, cấu hình định tuyến Vue-Router, kỹ thuật kết nối API bằng Axios và cấu hình đóng gói dự án với Webpack.

Bộ bài giảng thứ hai: **《Phân tích chi tiết kiến trúc mã nguồn của Vue.js》**. Nội dung tập trung: Hướng dẫn thiết lập môi trường debug mã nguồn Vue, phân tích tệp tin khởi tạo hệ thống, giải mã quy trình khởi tạo thực thể Vue, phân tích cơ chế theo dõi dữ liệu tự động (Data Reactivity) và đúc kết quy trình tự nghiên cứu mã nguồn framework hiệu quả.

Độc giả quan tâm có thể quét mã QR dưới đây để nhận khóa học miễn phí:

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120503.jpg)

## 资讯 (Tin tức)

1. **Ý tưởng tháp đất xử lý chất thải sinh học của thú cưng bằng giun đất tại Thượng Hải**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112117.jpg)

Trào lưu nuôi thú cưng (chó, mèo) tại các đô thị lớn đang ngày càng phổ biến. Việc thú cưng phóng uế bừa bãi khi đi dạo gây mất vệ sinh môi trường đô thị. Để giải quyết bài toán này, một khu dân cư tại quận Tùng Giang (Thượng Hải) đã triển khai thí điểm mô hình "Tháp giun đất" (Earthworm Tower) chuyên biệt để xử lý chất thải sinh học của vật nuôi.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112118.jpg)

Tháp giun đất được thiết kế cắm ngầm khoảng 20cm dưới lòng đất. Cư dân khi遛 thú cưng có thể thu gom chất thải đổ trực tiếp vào tháp, kết hợp cùng một số loại vỏ trái cây. Các nhân viên quản lý sẽ định kỳ thả giun đất xung quanh chân tháp. Giun đất sẽ chui qua các lỗ thoáng dưới đáy tháp để ăn chất thải hữu cơ bên trong. Quá trình di chuyển đào bới của giun giúp làm tơi xốp đất, tăng độ thông thoáng và thoát nước cho đất trồng xung quanh, đồng thời dịch tiết sinh học từ phân giun đất chính là nguồn phân bón tự nhiên vô cùng giàu dinh dưỡng (chứa nhiều nitơ, kali và vi sinh vật có lợi) giúp cỏ cây xung quanh phát triển tươi tốt.

2. **Lớp phủ siêu trơn sinh học giúp cắt giảm 50% lượng nước xả toilet**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112119.jpg)

Thống kê cho thấy lượng nước tiêu thụ hàng ngày để xả bồn cầu trên toàn thế giới vượt ngưỡng 141 tỷ lít, gây lãng phí tài nguyên nước nghiêm trọng tại nhiều khu vực khan hiếm nước ngọt. Nếu có giải pháp giúp tiết kiệm 50% lượng nước xả toilet sẽ mang lại ý nghĩa vô cùng lớn. Các nhà nghiên cứu tại Đại học Pennsylvania (Mỹ) đã phát triển thành công một lớp phủ xịt sinh học siêu trơn giúp bồn cầu luôn sạch sẽ và giảm thiểu tối đa lượng nước cần dùng để xả trôi chất bẩn.

Lớp xịt phủ sau khi khô sẽ tạo ra một lớp màng phân tử siêu mỏng có cấu trúc như các sợi lông mịn, tiếp theo một lớp bôi môi trơn silicone mỏng được phủ lên để tạo ra bề mặt siêu trơn (super-slippery). Mọi chất bẩn bám lên bồn cầu sẽ tự động trượt xuống dưới mà không để lại bất kỳ vết bám nào, cho phép xả sạch bồn cầu chỉ với lượng nước rất nhỏ. Ngoài ra, lớp phủ còn có đặc tính chống bám dính vi khuẩn hiệu quả, ngăn chặn sự phát triển của các chủng vi khuẩn gây mùi hôi và truyền nhiễm. Lớp phủ có độ bền cơ học đạt khoảng 500 lần xả nước trước khi cần xịt lại lớp mới.

3. **Nguy cơ gây mất an toàn lưới điện từ trào lưu sử dụng bóng bay tráng nhôm trong các bữa tiệc**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112207.jpg)

Sự phổ biến của các hình ảnh trang trí tiệc sinh nhật lộng lẫy trên các mạng xã hội đang thúc đẩy nhu cầu sử dụng bóng bay tráng nhôm (Mylar balloons) phát sáng. Tuy nhiên, các dòng bóng bay này được bơm khí heli nhẹ hơn không khí nên dễ bay lên trời. Nếu không may bị tuột tay bay vướng vào các đường dây tải điện cao thế ngoài trời, lớp vỏ tráng nhôm có tính dẫn điện cao này sẽ lập tức gây ra sự cố đoản mạch, cháy nổ làm mất điện diện rộng.

Ngày 1/10 vừa qua, sự cố bóng bay tráng nhôm vướng vào đường dây điện đã làm tê liệt hệ thống điện của một đô thị thuộc Nam California suốt hơn nửa giờ. Đơn vị vận hành lưới điện cảnh báo hiện tượng này đang gia tăng chóng mặt, ghi nhận tới 1.128 sự cố mất điện do bóng bay tráng nhôm gây ra tại khu vực này trong suốt năm 2018, tăng gần gấp đôi so với 4 năm trước. Thêm vào đó, chất liệu màng nhôm polyme của bóng bay cực kỳ khó phân hủy tự nhiên, gây ra các vấn đề rác thải nhựa nghiêm trọng khi bay lạc ra môi trường tự nhiên.

4. **Ngôi nhà 3D mô phỏng kiến trúc trạm cư trú Sao Hỏa hoàn thiện ngoài đời thực**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112208.jpg)

Một startup công nghệ Mỹ giới thiệu mô hình cabin rừng gỗ được xây dựng hoàn toàn bằng công nghệ in 3D sử dụng chất liệu composite đá bazan và polyme sinh học đặc chủng. Toàn bộ quy trình thi công được thực hiện tự động bằng cánh tay robot in 3D khổng lồ mà không cần công nhân xây dựng thao tác tại hiện trường. Ý tưởng thiết kế căn hộ này được phát triển để hướng tới việc xây dựng các trạm cư trú tương lai trên Sao Hỏa, nơi cát đá bazan chính là nguồn vật liệu bản địa sẵn có chiếm tỷ trọng lớn nhất trên bề mặt hành tinh đỏ.

Trước đó, thiết kế căn hộ này đã xuất sắc giành giải quán quân trong cuộc thi thiết kế nhà ở Sao Hỏa do NASA tổ chức. Hiện tại, công ty kiến trúc đã hiện thực hóa bản vẽ thành công trình thực tế đặt tại khu rừng hoang dã ngoại ô New York. Căn hộ cao 8 mét, diện tích mặt sàn đạt 46.4 m² và hiện đang được mở bán các gói trải nghiệm lưu trú qua đêm cho khách du lịch trải nghiệm cuộc sống tương lai.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019101905.jpg)

5. **Cá thể tê giác Sumatra cuối cùng tại Malaysia qua đời**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112403.jpg)

Ngày 23/11, cá thể tê giác Sumatra cuối cùng sinh sống tại Malaysia đã chính thức qua đời vì căn bệnh ung thư cổ tử cung. Cá thể tê giác cái mang tên Iman này đã được phát hiện mắc khối u xơ tử cung nghiêm trọng kể từ khi được đưa vào khu bảo tồn chăm sóc đặc biệt vào năm 2014. Trước đó vào tháng 5 năm nay, cá thể tê giác Sumatra đực cuối cùng của Malaysia cũng đã qua đời. Các chuyên gia sinh học đã kịp thời thu thập và bảo quản đông lạnh các tế bào trứng của Iman để phục vụ các dự án nghiên cứu thụ tinh nhân tạo trong tương lai.

Tê giác Sumatra là loài tê giác duy nhất sở hữu hai sừng đặc trưng và là loài tê giác có kích thước nhỏ nhất còn tồn tại trên trái đất. Chúng từng phân bố rộng khắp khu vực Châu Á, bao gồm cả vùng Hoa Nam Trung Quốc nhưng đã bị tuyệt chủng hoàn toàn tại Trung Quốc từ năm 1916 do nạn săn bắn lấy sừng làm dược liệu y học cổ truyền. Hiện nay loài này nằm trong danh mục động vật cực kỳ nguy cấp, chỉ còn lại một số lượng rất ít cá thể sống rải rác trong các khu rừng sâu của Indonesia.

6. **Dịch vụ "Livestream đổi phòng trọ" độc đáo tại Nhật Bản**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019113008.jpg)

Một nhà nghỉ bình dân tại thành phố Fukuoka (Nhật Bản) đã đưa ra chương trình quảng bá độc đáo: khách hàng khi lưu trú tại đây chỉ phải chi trả mức phí tượng trưng 100 Yên/đêm (tương đương khoảng 22.000 VNĐ), với điều kiện đồng ý cho phép nhà nghỉ phát sóng trực tiếp (livestream) toàn bộ quá trình sinh hoạt của mình trong phòng lên kênh YouTube chính thức của nhà nghỉ.

Trong quá trình livestream, khách hàng chỉ được tắt đèn khi đi ngủ, các khu vực nhà vệ sinh và nhà tắm riêng tư hoàn toàn không lắp camera, và kênh nghiêm cấm phát sóng các nội dung nhạy cảm. Vào những đêm không có khách lưu trú, kênh sẽ phát sóng trực tiếp khung cảnh bàn làm việc trống của chủ nhà nghỉ. Chỉ sau một tháng triển khai, nhà nghỉ đã tiếp đón 4 vị khách đồng ý tham gia chương trình "livestream đổi phòng" và kênh YouTube của nhà nghỉ đã nhanh chóng thu hút hơn 1.000 lượt đăng ký theo dõi.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019113010.jpg)

7. **Tin vắn**

- Một báo cáo y khoa trên tạp chí *BMJ* chia sẻ về ca bệnh hy hữu khi một bệnh nhân hoàn toàn không uống rượu nhưng liên tục có biểu hiện ngộ độc cồn. Kết quả sinh thiết cho thấy hệ vi sinh đường ruột của bệnh nhân chứa lượng nấm men hoạt động mạnh, tự động lên men toàn bộ lượng carbohydrate (tinh bột) nạp vào từ thức ăn thành cồn trực tiếp trong cơ thể.

- Trang thương mại điện tử của tập đoàn bán lẻ Costco gặp sự cố sập máy chủ kéo dài tới 16.5 giờ liên tục đúng vào đêm hội mua sắm Black Friday do lượng truy cập quá tải, ước tính thiệt hại doanh số trực tiếp lên tới hơn 11 triệu USD.

- Cục Quản lý Không gian mạng Trung Quốc ban hành quy định mới siết chặt quản lý nội dung số: Yêu cầu mọi nội dung video, âm thanh được tạo ra bởi trí tuệ nhân tạo (như công nghệ Deepfake) bắt buộc phải dán nhãn cảnh báo rõ ràng cho người xem, và nghiêm cấm sử dụng AI để tự động tạo ra các tin tức báo chí giả mạo.

- Đọc sách trên Instagram: Nhằm khuyến khích thói quen đọc sách của giới trẻ, Thư viện Công cộng New York đã triển khai dự án biên tập và đăng tải các tác phẩm văn học kinh điển lên tính năng Instagram Stories của trang cá nhân, thu hút hơn 300.000 lượt đọc sau một năm hoạt động.

- Bang California (Mỹ) thông qua điều luật sửa đổi cho phép người dân thu gom xác các loài động vật hoang dã (như hươu, nai) vô tình bị xe tông chết trên cao tốc mang về làm thực phẩm chế biến món ăn để tránh lãng phí nguồn thịt sạch, ước tính có khoảng 20.000 con hươu bị tông chết hàng năm tại bang này.

- Tập đoàn Huawei ra mắt dòng bo mạch chủ máy tính cá nhân sử dụng kiến trúc ARM đầu tiên của hãng, chạy bộ vi xử lý tự phát triển Kunpeng 920.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120501.jpg)

## 文章 (Bài viết)

1、[Bài viết] [Tại sao một số loài thực vật lại sở hữu màu sắc hoàn toàn không phải màu xanh lá?](https://plantsandprejudice.wordpress.com/2013/08/07/how-do-non-green-plants-work/) (Tiếng Anh)

Hầu hết thực vật thực hiện quang hợp nhờ chất diệp lục mang sắc tố xanh lá cây. Bài viết khoa học giải thích về cơ chế sinh học đặc biệt của một số loài thực vật không chứa chất diệp lục (như loài hoa ký sinh không có lá): cách chúng cộng sinh hoặc hút chất dinh dưỡng từ hệ rễ và nấm của các loài cây khác xung quanh để sinh tồn.

2、[Bài viết] [Ai đã giết chết thanh cuộn (Scrollbar) trên giao diện web?](https://ello.co/dredmorbius/post/0hgfswmoti3fi5zgftjecq) (Tiếng Anh)

Tác giả phê phán xu hướng thiết kế giao diện web hiện đại cố tình ẩn đi thanh cuộn dọc màn hình để tạo cảm giác tối giản giống giao diện ứng dụng di động. Tác giả lập luận thanh cuộn đóng vai trò trực quan hóa cực kỳ quan trọng giúp người đọc ước lượng được độ dài bài viết và hỗ trợ định vị di chuyển nhanh trang web, việc ẩn đi gây suy giảm trải nghiệm sử dụng thực tế của người dùng máy tính.

3、[Bài viết] [Hướng dẫn tối ưu hóa chiều cao giao diện trên thiết bị di động tránh sử dụng đơn vị 100vh](https://chanind.github.io/javascript/2019/09/28/avoid-100vh-on-mobile-web.html) (Tiếng Anh)

Phân tích lỗi hiển thị giao diện web phổ biến trên thiết bị di động: do các trình duyệt di động (Safari, Chrome) có cơ chế tự động ẩn/hiển thị thanh địa chỉ khi cuộn trang, việc đặt chiều cao CSS `100vh` sẽ khiến một phần nội dung trang bị che khuất dưới thanh công cụ. Bài viết chia sẻ các mẹo sử dụng biến CSS và JavaScript để tính toán chính xác chiều cao viewport thực tế của thiết bị.

## 软件 (Phần mềm)

1、[SingleFileZ — Tiện ích trình duyệt giúp lưu trữ toàn bộ trang web thành một tệp zip nén duy nhất](https://github.com/gildas-lormeau/SingleFileZ)

Hỗ trợ lưu lại giao diện trang web, bao gồm toàn bộ file ảnh, stylesheet và script đi kèm thành một tệp tin nén định dạng `.html` (thực chất là một file zip đổi đuôi) giúp dễ dàng lưu trữ ngoại tuyến và chia sẻ nhanh chóng.

2、[PostgREST — Tiện ích mở rộng tự động sinh cổng API RESTful từ cơ sở dữ liệu PostgreSQL](https://github.com/PostgREST/postgrest)

Công cụ viết bằng Haskell giúp kết nối trực tiếp vào database PostgreSQL để tự động phân tích cấu trúc bảng dữ liệu và sinh ra các endpoint API đạt chuẩn RESTful đầy đủ tính năng CRUD, phân trang và bảo mật mà không cần viết mã backend.

3、[Tàu Điện Nhật Bản (Japan Transit) — Ứng dụng dẫn đường giao thông công cộng tối giản cho khách du lịch](https://github.com/ruanyf/weekly/issues/933)

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110406.jpg)

App dẫn đường giao thông công cộng được tối ưu hóa giao diện hoàn toàn bằng tiếng Trung/tiếng Anh, hỗ trợ tìm kiếm chuyển tuyến tàu điện ngầm, xe bus, tàu Shinkansen nhanh chóng, không chứa quảng cáo phiền toái.

4、[snapdrop — Công cụ chia sẻ tệp tin ngang hàng trong cùng mạng nội bộ chạy trực tiếp trên trình duyệt](https://github.com/RobinLinus/snapdrop)

Giải pháp chia sẻ file nhanh chóng tương tự như AirDrop của Apple nhưng hoạt động đa nền tảng (chạy được trên cả Android, Windows, Linux) nhờ ứng dụng giao thức kết nối trực tiếp WebRTC qua mạng Wi-Fi nội bộ mà không cần cài đặt phần mềm.

## 资源 (Tài nguyên)

1、[Tài liệu] [Hacker Laws - Tổng hợp các định luật, nguyên lý thiết kế và mô hình lập trình cốt lõi dành cho kỹ sư](https://github.com/nusr/hacker-laws-zh)

Bản dịch tiếng Trung của kho lưu trữ nổi tiếng giới thiệu ngắn gọn ý nghĩa của các định luật kinh điển trong ngành công nghệ: Định luật Moore, Định luật Hofstadter, Định luật Murphy, Nguyên lý KISS, Nguyên lý YAGNI giúp lập trình viên nâng cao tư duy thiết kế hệ thống.

2、[Tài liệu] [Node.js Best Practices - Tổng hợp các tiêu chuẩn lập trình Node.js thực chiến tốt nhất](https://github.com/goldbergyoni/nodebestpractices)

Kho lưu trữ GitHub tổng hợp hơn 80 nguyên tắc, tiêu chuẩn thiết kế mã nguồn, cấu trúc dự án, xử lý lỗi bảo mật và tối ưu hóa hiệu năng thực tế dành cho các nhà phát triển ứng dụng Node.js backend.

## 图片 (Hình ảnh)

1. **Space Cemetery - Thực trạng nhặt phế liệu vũ trụ độc đáo của người dân vùng núi Altai (Nga)**

Trung tâm Hàng không vũ trụ Baikonur của Nga nằm sâu trong nội địa nên toàn bộ các mảnh vỡ vỏ tên lửa đẩy sau khi剥 tách ở các tầng bay đều rơi tự do xuống các thung lũng hoang vu của vùng núi Altai thay vì rơi xuống biển như các vụ phóng của Mỹ.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100718.jpg)

Ước tính từ thập niên 1950 đến nay đã có hơn 2.500 tấn rác thải vũ trụ rơi xuống khu vực này. Nhiều người dân địa phương đã phát triển một nghề sinh kế độc đáo: sử dụng ống nhòm theo dõi đường rơi của tên lửa trong đêm, lái xe Jeep tiếp cận hiện trường để dùng đèn khò cắt xẻ các khối hợp kim titan, nhôm siêu nhẹ và dây cáp đồng từ mảnh vỡ tên lửa đem bán phế liệu. Việc này tiềm ẩn nhiều nguy cơ sức khỏe nghiêm trọng do nhiên liệu tên lửa dư thừa chứa nhiều chất hóa học cực độc ngấm vào đất và nguồn nước ngầm của khu vực.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019100720.jpg)

2. **Tượng Lion-Man - Tác phẩm điêu khắc nghệ thuật cổ xưa nhất của lịch sử loài người**

Tượng người đầu sư tử (Lion-Man) làm từ ngà voi ma mút có chiều cao 31cm, được chế tạo cách đây khoảng 40.000 đến 50.000 năm trước. Đây là tác phẩm điêu khắc nghệ thuật cổ xưa nhất được ghi nhận của nhân loại.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019101202.jpg)

Các mảnh vỡ của bức tượng được phát hiện lần đầu tiên vào năm 1939 tại một hang động ở Đức. Trải qua nhiều đợt tìm kiếm và ghép nối phục dựng tỉ mỉ vào các năm 1970, 1987 và hoàn thiện vào năm 2013, bức tượng hiện đã được khôi phục gần như nguyên vẹn cấu trúc ban đầu.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019101203.jpg)

## 文摘 (Văn trích)

1. **Thực trạng bất đối xứng về thời gian ước lượng hoàn thành dự án giữa kỹ sư và nhà quản lý**

Trong suốt quá trình làm nghề lập trình viên từ mảng web CRUD đơn giản cho đến khi chuyển dịch sang mảng tính toán phân tán phức tạp (như xử lý dữ liệu lớn, khoa học dữ liệu), tôi phát hiện ra một thực tế kỳ lạ: Các nhà quản lý dự án (Project Managers) hầu như không có bất kỳ sự thay đổi nào về thời gian kỳ vọng hoàn thành công việc.

Họ vẫn luôn kỳ vọng một hệ thống tính toán phân tán thời gian thực phức tạp có thể được lập trình hoàn thiện chỉ trong vòng vài tuần tương tự như việc dựng một trang web REST API đơn giản trước đây. Bất kể bạn có nỗ lực giải thích, chia nhỏ đầu việc và dự phòng rủi ro ra sao, họ vẫn cho rằng sự chậm trễ tiến độ là do lỗi năng lực cá nhân của lập trình viên chứ không phải do độ khó nội tại của bài toán kỹ thuật.

Điều này dẫn tới một thực trạng đau lòng: Các nhà quản lý dự án hoàn toàn không có khái niệm thực tế về thời gian cần thiết để giải quyết một bài toán kỹ thuật phức tạp. 

Thế giới phần mềm ngày càng trở nên phức tạp hơn do chúng ta đang nỗ lực giải quyết các bài toán khó hơn của xã hội. Tuy nhiên, ban quản lý thường có niềm tin ngây thơ rằng mọi công nghệ hiện nay đều có thể được xây dựng nhanh chóng qua vài thao tác kéo thả. Khoảng cách kỳ vọng quá lớn này buộc lập trình viên phải liên tục đưa ra các giải pháp chắp vá bằng "băng keo và hồ dán" để kịp chạy deadline bàn giao sản phẩm, để lại một núi lỗi kỹ thuật (technical debt) khổng lồ cho đội ngũ vận hành gánh chịu, còn bản thân họ sẽ tiếp tục quay cuồng sửa lỗi cho đến khi kiệt sức và chọn giải pháp nghỉ việc.

## 言论 (Danh ngôn)

1、

> "Để mô tả通 tài của một con người: Một người phải có khả năng tự thay tã cho con, lập kế hoạch chiến tranh, mổ lợn, lái tàu, thiết kế nhà cửa, viết thơ sonnet, hạch toán sổ sách, xây tường, nắn khớp xương trật, an ủi người sắp qua đời, phục tùng mệnh lệnh, đưa ra mệnh lệnh, hợp tác đồng đội, hành động độc lập, giải phương trình toán học, phân tích vấn đề mới, xúc phân chuồng, lập trình máy tính và dũng cảm đối mặt cái chết. Sự chuyên biệt hóa chỉ nên dành cho các loài côn trùng."
> 
> -- Robert Heinlein, nhà văn khoa học viễn tưởng Mỹ

(Hết)
