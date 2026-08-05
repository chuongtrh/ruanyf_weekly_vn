# 科技爱好者周刊：第 87 期 (Bản tin chia sẻ công nghệ số 87)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121703.jpg)

Ảnh bìa: Hãng công nghệ Kneron (Mỹ) trình diễn việc sử dụng mặt nạ in 3D màu chất lượng cao để vượt qua hệ thống nhận diện khuôn mặt của các cổng thanh toán.

## 刊首语 (Lời tựa)

Nhiều năm trước, tôi từng giới thiệu một bài viết gối đầu giường cho các kỹ sư mới bước chân vào ngành công nghiệp internet. Bài viết mang tên [《Đừng tự coi mình là lập trình viên thuần túy》](http://www.ruanyifeng.com/blog/2011/10/dont_call_yourself_a_programmer.html), trong đó có một lời khuyên cốt lõi và thực tế nhất như sau:

> Mục tiêu tối thượng (và thực tế là duy nhất) mà các doanh nghiệp quan tâm là tăng trưởng doanh thu và tối ưu hóa chi phí.
> 
> Doanh nghiệp không thực sự cần các lập trình viên gõ code đơn thuần, họ cần những người có năng lực giúp họ gia tăng doanh số hoặc cắt giảm chi phí vận hành.
> 
> Doanh nghiệp tuyển dụng bạn là để hoàn thành các mục tiêu dự án giúp gia tăng doanh thu và tối ưu chi phí cho họ, chứ không phải để tài trợ cho các phát kiến phần mềm mang tính cá nhân của bạn.

Bài viết này sẽ giúp bạn hiểu rõ bản chất vận hành của ngành công nghiệp phần mềm, giải mã nhiều thực tế phũ phàng và bớt đi những ảo tưởng màu hồng khi mới đi làm. Dù đã qua nhiều năm, tôi vẫn khuyến nghị các bạn nên đọc lại.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121805.jpg)

Hôm nay, tôi muốn giới thiệu thêm một bài viết hay khác mang tên [《Năm nhiệm vụ đầu tiên của một kỹ sư phần mềm mới ra trường》](https://evanliman.to/2019/10/06/so-youre-a-new-grad-software-engineer.html), chia sẻ về những việc cụ thể một tân binh nên bắt tay vào làm khi gia nhập đội ngũ. Nếu bài viết trước đại diện cho tư duy cốt lõi (Đạo), thì bài viết này chính là cẩm nang thực hành (Thuật).

Tác giả chỉ ra 5 đầu việc quan trọng một lập trình viên mới cần thực hiện khi bắt đầu làm việc cùng nhóm. Bốn việc đầu tiên rất quen thuộc: làm quen với kiến trúc hệ thống, tìm hiểu quy trình phát triển nội bộ, củng cố các mảng kiến thức nền tảng còn thiếu và bắt tay vào giải quyết các lỗi nhỏ trước (như đóng vài issue dễ). Đây đều là những việc cơ bản, nhưng đầu việc thứ năm lại là thứ mà rất ít tân binh chủ động thực hiện dù hoàn toàn trong tầm tay: **Chủ động viết và hoàn thiện hệ thống tài liệu (documentation) cho đội ngũ.**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121807.jpg)

Thực trạng chung tại các doanh nghiệp công nghệ trong nước là hệ thống tài liệu dự án thường rất sơ sài hoặc thậm chí không có, do đội ngũ kỹ sư phải dồn toàn bộ thời gian và tâm sức cho tiến độ phát triển tính năng mới. Cách tiếp cận dự án thông thường của người mới là nghe giải thích truyền miệng từ đồng nghiệp đi trước, sau đó tự mò mẫm đọc mã nguồn. Bạn hoàn toàn có thể tận dụng chính quá trình tự nghiên cứu và làm quen code này để bổ sung các tài liệu hướng dẫn còn thiếu cho dự án. Không cần viết quá hoa mỹ, chỉ cần ghi chép trung thực các luồng chạy của code, sơ đồ kiến trúc chi tiết là đã giúp tiết kiệm rất nhiều thời gian cho những người mới gia nhập sau này (và cho chính bạn khi cần đọc lại).

Từ trải nghiệm cá nhân, tôi nhận thấy việc viết tài liệu mang lại sự phát triển năng lực cá nhân vô cùng lớn: (1) Giúp bạn nhanh chóng làm chủ và hiểu sâu về dự án; (2) Rèn luyện tư duy và năng lực diễn đạt mạch lạc; (3) Nâng cao trình độ kỹ thuật thực tế, bởi bạn chỉ có thể viết ra một cách rõ ràng khi đã thực sự hiểu thấu đáo bản chất của đoạn code; (4) Xây dựng uy tín và sức ảnh hưởng cá nhân trong nhóm, tài liệu của bạn càng chất lượng thì số người tìm đọc và tham khảo ý kiến của bạn khi gặp khó khăn càng nhiều. Lâu dần, bạn sẽ trở thành chuyên gia nắm rõ dự án nhất và là nhân sự không thể thay thế trong đội ngũ.

Tóm lại, các lập trình viên mới hãy đặc biệt coi trọng việc viết tài liệu, chủ động đóng góp công sức hoàn thiện hệ thống tài liệu cho nhóm. Việc này mang lại giá trị vô cùng lớn cho sự phát triển của cá nhân lẫn sự lớn mạnh của đội ngũ. Hãy bắt đầu viết ngay từ hôm nay. Về lâu dài, bạn sẽ nhận ra giá trị to lớn của thói quen này mang lại cho sự nghiệp của mình.

## Dịch thuật nhanh chóng với ứng dụng Caiyun Translator

Trong mỗi số bản tin tuần của chúng ta, phần lớn nội dung và đường dẫn tham khảo đều sử dụng ngôn ngữ tiếng Anh. Nhiều độc giả hỏi tôi làm thế nào để có thể đọc hiểu và chắt lọc thông tin từ các bài viết tiếng Anh này một cách hiệu quả nhất? Câu trả lời rất đơn giản: Hãy tận dụng sức mạnh của các công cụ dịch thuật tự động.

Với bất kỳ bài viết nào, các công cụ dịch thuật tự động ngày nay chỉ mất chưa đầy một giây để dịch toàn bộ nội dung sang ngôn ngữ đích, giúp bạn nắm nhanh ý chính của bài viết trước khi quyết định có dành thời gian đọc kỹ bản gốc hay không. Đặc biệt là các bài viết chuyên ngành công nghệ thường chứa nhiều thuật ngữ chuẩn mực và cấu trúc ngữ pháp rõ ràng, cực kỳ phù hợp để dịch tự động.

Hôm nay tôi muốn giới thiệu tới các bạn một công cụ dịch thuật chất lượng cao - [Caiyun Translator](https://fanyi.caiyunapp.com/#/web). Công cụ cung cấp cả phiên bản [tiện ích mở rộng Chrome](https://fanyi.caiyunapp.com/#/web) và ứng dụng di động [Caiyun Translator App](https://fanyi.caiyunapp.com/#/app), hỗ trợ hiển thị song ngữ trực quan ngay trên trang web chỉ với một cú click chuột.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121705.jpg)

Qua trải nghiệm thực tế, tôi đánh giá chất lượng dịch thuật của Caiyun rất sát nghĩa và tự nhiên, hỗ trợ dịch hai chiều Anh-Trung, Trung-Anh và cả tiếng Nhật. Bạn có thể bật tính năng tự động dịch trong phần cài đặt để trang web tự động hiển thị bản dịch song ngữ ngay khi mở trang, đồng thời hỗ trợ bôi đen để dịch từ vựng trực tiếp. Hiện tại, tiện ích trên Chrome Web Store đang nhận được đánh giá rất cao đạt 4.6/5 sao.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121506.jpg)

Điểm độc đáo của Caiyun là hỗ trợ dịch phụ đề video trực tiếp. Đối với các video sử dụng tệp phụ đề ngoài (như file `.srt`), Caiyun có thể dịch thời gian thực hiển thị song ngữ tiện lợi. Đối với các video không có sẵn phụ đề, bạn có thể cài đặt công cụ [Caiyun Interpret](https://www.caiyunapp.com/interpretation/) để tự động nhận dạng âm thanh từ microphone hệ thống và dịch sang tiếng Trung.

Ngoài ra, đối với các nhà phát triển, bạn hoàn toàn có thể tích hợp API dịch thuật của Caiyun vào ứng dụng cá nhân với hạn mức miễn phí lên tới 1 triệu ký tự dịch thuật mỗi tháng.

## 资讯 (Tin tức)

1. **Phát hiện xác cá thể chó cổ đại nguyên vẹn 18.000 năm tuổi trong lớp băng vĩnh cửu**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019113004.jpg)

Sự tan chảy của các lớp băng vĩnh cửu tại vùng Siberia đang giúp các nhà khoa học tiếp cận được nhiều mẫu vật cổ đại được bảo tồn hoàn hảo trong băng. Phát hiện mới nhất là xác một cá thể chó con có niên đại khoảng 18.000 năm trước. Cá thể này qua đời khi mới khoảng 2 tháng tuổi, được bảo quản gần như nguyên vẹn từ lớp lông mềm, mũi cho tới cấu trúc răng.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019113005.jpg)

Kết quả phân tích chuỗi DNA cho thấy cá thể này sở hữu cấu trúc gene chuyển tiếp đặc trưng giữa loài sói cổ đại và loài chó hiện đại, được xem là mẫu vật chó cổ xưa nhất từng được phát hiện. Các nghiên cứu trước đây chỉ ra loài người đã bắt đầu thuần hóa chó từ loài sói trong khoảng từ 20.000 đến 40.000 năm trước.

2. **Tỉnh Quebec (Canada) ban hành điều luật bắt buộc lắp khóa hơi thở ngăn chặn tài xế酒 lái**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019113007.jpg)

Do đặc thù khí hậu lạnh giá kéo dài, lượng tiêu thụ rượu bia tại Quebec là rất lớn, dẫn tới các vụ tai nạn do lái xe sau khi uống rượu bia làm khoảng 100 người tử vong và hàng nghìn người bị thương mỗi năm. Nhằm siết chặt quản lý, Quebec ban hành quy định mới: đối với các tài xế vi phạm lỗi uống rượu bia khi lái xe từ 2 lần trở lên trong vòng 10 năm, họ sẽ bắt buộc phải lắp đặt hệ thống máy đo nồng độ hơi thở liên kết trực tiếp với bộ khóa khởi động xe. Trước mỗi lần nổ máy xe, tài xế bắt buộc phải thổi nồng độ cồn, nếu phát hiện có cồn trong hơi thở, hệ thống sẽ tự động khóa động cơ không cho phép khởi động xe.

Nếu lực lượng cảnh sát tuần tra phát hiện tài xế thuộc diện quy định cố tình không lắp đặt thiết bị này, họ sẽ đối mặt với các hình phạt cực kỳ nghiêm khắc: phạt tiền 1.500 USD cho lần đầu vi phạm, tạm giam 90 ngày cho lần thứ hai và phạt tù chung thân cho lần vi phạm thứ ba. Đây được đánh giá là khung pháp lý nghiêm khắc nhất thế giới hiện nay đối với hành vi lái xe sau khi sử dụng rượu bia.

3. **Thế hệ củ sạc công nghệ mới ứng dụng vật liệu bán dẫn GaN siêu nhỏ gọn**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120304.jpg)

Kích thước của các bộ nguồn sạc máy tính xách tay và điện thoại đang có xu hướng thu nhỏ vượt trội nhờ ứng dụng vật liệu bán dẫn thế hệ mới GaN (Gallium Nitride) thay thế cho vật liệu silicon truyền thống, cho phép thiết kế các củ sạc công suất lớn trong một thân hình cực kỳ nhỏ gọn. Ảnh trên: bên trái là củ sạc 5W truyền thống của Apple, phía sau là hai củ sạc GaN công suất 30W và 45W mới với kích thước chênh lệch không đáng kể.

Vật liệu GaN sở hữu hiệu suất chuyển đổi năng lượng vượt trội, giảm thiểu tối đa lượng điện năng hao phí tỏa ra dưới dạng nhiệt, giúp củ sạc hoạt động mát mẻ hơn và loại bỏ hoàn toàn nguy cơ cháy nổ do quá nhiệt.

4. **Bệnh viện Thượng Hải ứng dụng nhận diện khuôn mặt ngăn chặn tình trạng黃牛 đầu cơ số khám bệnh**

Tại các bệnh viện tuyến đầu của Thượng Hải, việc đăng ký số khám bệnh của các bác sĩ chuyên khoa đầu ngành là cực kỳ khó khăn do tình trạng cò mồi (hoàng ngưu) đầu cơ số để bán lại với giá cắt cổ. Nhằm giải quyết triệt để vấn nạn này, Bệnh viện Ung bướu Thượng Hải trực thuộc Đại học Fudan đã đưa vào vận hành hệ thống đăng ký khám bệnh tích hợp công nghệ nhận diện khuôn mặt tại các cây ki-ốt tự động.

Bệnh nhân khi đăng ký khám bệnh bắt buộc phải quét thẻ căn cước công dân đồng thời chụp ảnh khuôn mặt trực tiếp tại camera của máy. Nếu hình ảnh chụp thực tế không khớp với ảnh trên thẻ căn cước, hệ thống sẽ lập tức từ chối giao dịch, loại bỏ hoàn toàn khả năng cò mồi sử dụng giấy tờ giả hoặc gom thẻ của người khác để xếp hàng đăng ký hộ. Đối với các trường hợp người thân đăng ký hộ bệnh nhân lớn tuổi hoặc người không tiện di chuyển, bệnh viện cho phép đăng ký liên kết thông tin căn cước của một người bảo hộ duy nhất cho mỗi tài khoản bệnh nhân.

5. **Pantone công bố Classic Blue là màu sắc đại diện của năm 2020**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120610.jpg)

Viện màu sắc toàn cầu Pantone chính thức công bố sắc màu của năm 2020 là tông màu xanh cổ điển "Classic Blue" (mã màu 19-4052) - một tông màu xanh lam trầm ấm mang lại cảm giác bình yên và tĩnh lặng cho tâm hồn.

Đại diện Pantone chia sẻ, Classic Blue gợi liên tưởng đến sắc màu của bầu trời lúc hoàng hôn buông xuống, sắc màu của những quả việt quất chín mọng, mang lại thông điệp về sự ổn định, tin cậy và khát khao xây dựng một nền tảng vững chắc cho tương lai trong bối cảnh thế giới nhiều biến động. Đồng thời, nghiên cứu thị hiếu chỉ ra rằng tông màu xanh lam trầm này không còn mang lại cảm giác u buồn hay cô đơn cho thế hệ trẻ ngày nay như các thế hệ trước thường nghĩ.

6. **Kao ra mắt công nghệ màng xịt da siêu mỏng ứng dụng trong mỹ phẩm và y tế**

Tập đoàn hóa mỹ phẩm Kao (Nhật Bản) giới thiệu dòng sản phẩm tạo màng da nhân tạo siêu mỏng độc đáo. Người dùng chỉ cần xịt một lớp bột polymer siêu mịn lên bề mặt da mặt, sau đó dùng lòng bàn tay ấn nhẹ, các sợi polymer sẽ tự động liên kết tạo thành một lớp màng trong suốt siêu mỏng ôm khít bề mặt da, giúp da trở nên mịn màng tự nhiên mà mắt thường hoàn toàn không thể phát hiện ra được. Lớp màng có cấu trúc lưới siêu vi giúp da vẫn có thể trao đổi khí và thoát mồ hôi tự nhiên.

Lớp màng này có tác dụng che phủ hiệu quả các vết nám, sẹo trên da, hỗ trợ giữ ẩm chuyên sâu và làm lớp nền trang điểm bảo vệ da. Khi muốn tẩy trang, người dùng chỉ cần dùng tay lột nhẹ lớp màng ra khỏi da mặt một cách dễ dàng. Dòng sản phẩm này có mức giá khá cao, khoảng 50.000 Yên (tương đương hơn 10 triệu VNĐ) cho một bộ thiết bị xịt phủ.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120703.jpg)

7. **Tin vắn**

- Thống kê nội bộ của tập đoàn IBM chỉ ra rằng các nhân sự sử dụng máy tính Mac có hiệu suất làm việc vượt trội và ít gặp lỗi hệ thống hơn so với Windows: chỉ có khoảng 5% người dùng Mac yêu cầu hỗ trợ kỹ thuật từ bộ phận IT so với 40% của người dùng Windows, giúp IBM tiết kiệm trung bình từ 273 đến 543 USD chi phí vận hành cho mỗi thiết bị Mac được trang bị thay thế PC.

- Một nhóm nghị sĩ Pháp đề xuất dự thảo luật cấm tổ chức ngày hội mua sắm giảm giá Black Friday tại nước này nhằm hạn chế tình trạng tiêu dùng quá đà gây lãng phí tài nguyên và ô nhiễm môi trường từ việc giao nhận hàng hóa.

- Bang California (Mỹ) thông qua luật mới quy định các trường trung học cơ sở không được phép bắt đầu giờ học trước 8 giờ sáng và trung học phổ thông không trước 8 giờ 30 phút sáng nhằm đảm bảo thời gian ngủ đủ giấc cho học sinh phát triển thể chất.

- Microsoft công bố thiết kế chính thức của dòng máy chơi game console thế hệ mới Xbox Series X với kiểu dáng hình hộp chữ nhật đứng tối giản cùng hệ thống tản nhiệt lớn ở mặt trên, hiệu năng xử lý đồ họa gấp 4 lần thế hệ Xbox One X hiện tại.

- Các nhà khoa học Israel phát triển thuật toán xử lý hình ảnh độc đáo cho phép loại bỏ hoàn toàn các hiệu ứng khúc xạ ánh sáng, gợn sóng nước từ các bức ảnh chụp dưới nước, giúp tái tạo lại độ chi tiết và màu sắc chân thực của rạn san hô như được chụp trên cạn (ảnh dưới).

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111504.jpg)

## 文章 (Bài viết)

1、[Bài viết] [Lập trình viên chia sẻ kỹ thuật vượt qua cơ chế xác thực OAuth của GitHub để nhận thưởng 25.000 USD](https://blog.teddykatz.com/2019/11/05/github-oauth-bypass.html) (Tiếng Anh)

Tác giả chia sẻ chi tiết lỗ hổng bảo mật nghiêm trọng do anh phát hiện trên GitHub liên quan đến việc gửi các yêu cầu phương thức HTTP `HEAD` đặc biệt để bỏ qua bước xác thực tài khoản OAuth, cho phép truy cập trái phép vào các kho dữ liệu riêng tư. GitHub đã nhanh chóng vá lỗi và trao tặng khoản tiền thưởng bảo mật trị giá 25.000 USD cho anh.

2、[Bài viết] [Khảo sát thực nghiệm về giới hạn số tầng lồng nhau tối đa của các thư viện Parser JSON trên các ngôn ngữ lập trình](https://github.com/lovasoa/bad_json_parsers/blob/master/README.md) (Tiếng Anh)

Do đặc tả kỹ thuật tiêu chuẩn của JSON không quy định giới hạn số lượng tầng lồng nhau tối đa của các cặp ngoặc `{}` hoặc `[]`, tác giả đã viết kịch bản kiểm thử tự động để đo đạc giới hạn chịu tải của các thư viện parser JSON phổ biến trên nhiều ngôn ngữ lập trình trước khi xảy ra lỗi tràn bộ nhớ đệm (stack overflow) (ví dụ: Node.js có khả năng parser tối đa 5.712 tầng lồng nhau).

3、[Bài viết] [Tìm hiểu về mô hình phát triển phần mềm dạng Thác nước (Waterfall) và lý do mô hình Tinh gọn (Agile) chiếm ưu thế](https://martinfowler.com/bliki/WaterfallProcess.html) (Tiếng Anh)

Chuyên gia công nghệ nổi tiếng Martin Fowler phân tích về lịch sử, ưu nhược điểm của mô hình phát triển phần mềm tuần tự Waterfall truyền thống, giải thích tại sao mô hình này thường dẫn tới rủi ro chậm trễ tiến độ lớn trong các dự án hiện đại và so sánh với hiệu quả của Agile.

## 软件 (Phần mềm)

1、[vy — IDE tối giản vận hành hoàn toàn trên môi trường dòng lệnh CLI](https://github.com/vyapp/vy)

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111412.jpg)

Công cụ soạn thảo mã nguồn gọn nhẹ dành riêng cho lập trình viên yêu thích làm việc trên terminal, tích hợp sẵn các phím tắt điều hướng nhanh tương tự như Vim và hỗ trợ quản lý nhiều tab công việc linh hoạt.

2、[Joplin — Ứng dụng ghi chú và quản lý công việc nguồn mở hỗ trợ mã hóa đầu cuối](https://github.com/laurent22/joplin)

Giải pháp ghi chú mạnh mẽ thay thế hoàn hảo cho Evernote, hỗ trợ định dạng Markdown, có sẵn ứng dụng cho cả máy tính (Windows, macOS, Linux) và điện thoại di động (iOS, Android), hỗ trợ đồng bộ dữ liệu bảo mật qua các dịch vụ đám mây Nextcloud, Dropbox, WebDAV.

3、[whocanuse — Công cụ trực tuyến kiểm tra khả năng tiếp cận màu sắc (Accessibility) của thiết kế](https://whocanuse.com/)

Hỗ trợ các nhà thiết kế web đánh giá độ tương phản của phối màu chữ và nền đối với người dùng mắc các hội chứng suy giảm thị lực (như mù màu, đục thủy tinh thể, tăng nhãn áp) theo tiêu chuẩn WCAG giúp tối ưu hóa giao diện cho mọi người.

## 资源 (Tài nguyên)

1、[Tài liệu] [Chia sẻ miễn phí tệp quét 3D độ phân giải cao của bức tượng bán thân Nữ hoàng Ai Cập Nefertiti](https://www.thingiverse.com/thing:3974391)

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120103.jpg)

Bức tượng bán thân Nữ hoàng Nefertiti chế tác từ năm 1345 TCN là báu vật khảo cổ vô giá đang được lưu giữ tại bảo tàng Berlin. Bảo tàng đã thực hiện quét laser 3D độ phân giải cực cao và chia sẻ công khai tệp tin thiết kế lên internet cho phép người dùng toàn cầu tải về phục vụ in 3D sao chép chính xác.

## 图片 (Hình ảnh)

1. **Chiến dịch quảng cáo đầy châm biếm chống lại Google của Basecamp**

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102104.jpg)

Hãng phần mềm Basecamp đã mua vị trí quảng cáo đầu tiên trên Google tìm kiếm với tiêu đề: "Chúng tôi thực sự không muốn chạy quảng cáo này".

Nội dung quảng cáo ghi rõ: "Basecamp là kết quả tìm kiếm tự nhiên số 1 cho từ khóa này, nhưng Google vẫn cho phép các đối thủ cạnh tranh mua vị trí quảng cáo hiển thị đè lên trên tên thương hiệu của chúng tôi. Vì vậy chúng tôi bắt buộc phải chi tiền mua vị trí này, giống như việc một doanh nghiệp độc lập nhỏ phải trả tiền chuộc cho một gã khổng lồ công nghệ vậy".

2. **Kuandinsky Bridge - Cây cầu gỗ mục nát nguy hiểm nhất thế giới tại Nga**

Cây cầu Kuandinsky bắc ngang qua sông Vitim thuộc khu vực Siberia (Nga) ban đầu được thiết kế làm cầu tạm phục vụ thi công tuyến đường sắt nhưng sau đó được tận dụng làm cầu đường bộ cho xe ô tô di chuyển qua sông.

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019083002.jpg)

Cây cầu dài hơn 500 mét nhưng chỉ rộng đúng 2 mét, hoàn toàn không có lan can bảo vệ hay bất kỳ thiết bị cứu hộ nào. Bề mặt cầu được lát bằng các thanh tà vẹt gỗ đã mục nát theo thời gian, trơn trượt dữ dội vào mùa tuyết rơi kết hợp cùng gió lớn ngoài sông khiến mọi tài xế khi đi qua đây đều đối mặt với hiểm họa rơi xuống sông bất kỳ lúc nào.

![](https://cdn.beekka.com/blogimg/asset/201908/bg2019083003.jpg)

## 文摘 (Văn trích)

1. **Thực trạng khai thác và bài toán tái chế đầy thách thức của nguồn pin Lithium trên xe điện**

Các dòng xe điện hiện đại sử dụng nguồn năng lượng lưu trữ từ pin Lithium-ion. Ưu điểm lớn nhất của pin Lithium là hiệu suất chuyển đổi năng lượng rất cao đạt từ 60% đến 80% (trong khi động cơ đốt trong truyền thống chỉ đạt hiệu suất từ 20% đến 60%).

Tuy nhiên, nhược điểm chí mạng của pin Lithium nằm ở mật độ năng lượng (Energy Density). Hiện nay, mỗi kg pin Lithium-ion chỉ có thể lưu trữ được lượng điện năng khoảng 0.2 kWh, trong khi mỗi kg xăng truyền thống có khả năng giải phóng nhiệt lượng tương đương 2 kWh điện - nghĩa là mật độ năng lượng của xăng cao gấp 10 lần so với pin Lithium. Ví dụ thực tế: một bình xăng ô tô 60 lít chứa khoảng 43 kg xăng, để tích trữ được lượng năng lượng tương đương bằng pin Lithium-ion hiện nay, chiếc xe điện sẽ phải mang theo một khối pin nặng tới hơn 400 kg.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121903.jpg)

Tuổi thọ và nguồn nguyên liệu sản xuất pin cũng là những thách thức lớn đối với môi trường. Để đảm bảo pin xe điện hoạt động bền bỉ qua hàng nghìn chu kỳ sạc xả, nhà sản xuất bắt buộc phải sử dụng các kim loại quý hiếm như coban, niken và graphite (than chì) để chế tạo các điện cực. Nguồn lithium toàn cầu hiện nay chủ yếu được khai thác từ khu vực "Tam giác Lithium" ở Nam Mỹ (gồm Argentina, Chile và Bolivia) và một lượng ít ở Úc và Trung Quốc. Hoạt động khai thác lithium tiêu thụ và làm ô nhiễm nguồn nước ngầm nghiêm trọng (tại Chile, 65% lượng nước ngọt của khu vực mỏ được dùng cho tuyển quặng lithium).

Bên cạnh đó, hoạt động khai thác coban tại Cộng hòa Dân chủ Congo (nơi cung cấp 50% sản lượng coban toàn cầu) đang đối mặt với các vấn đề nhân đạo nghiêm trọng khi UNICEF ước tính có khoảng 40.000 trẻ em đang phải lao động thủ công trong các hầm mỏ khai thác quặng thô độc hại tại đây.

Quy trình tái chế pin Lithium hết hạn sử dụng cũng đang gặp bế tắc khi tỷ lệ tái chế thực tế tại các nước phát triển như Úc chỉ đạt khoảng 2% do chi phí tách chiết lithium tinh khiết từ pin cũ cao hơn nhiều so với việc khai thác quặng thô mới. Do đó, pin Lithium chưa phải là giải pháp vạn năng cho bài toán biến đổi khí hậu toàn cầu, nhân loại vẫn cần đẩy mạnh nghiên cứu các công nghệ lưu trữ năng lượng thế hệ mới xanh hơn.

## 言论 (Danh ngôn)

1、

> "Tất cả chúng ta đều biết rằng, nếu có thể du hành thời gian quay lại quá khứ để thay đổi dù chỉ một chi tiết nhỏ nhặt nhất, toàn bộ cục diện tương lai sau đó sẽ bị xoay chuyển hoàn toàn.
> 
> Thế nhưng, hầu như không một ai trong chúng ta nghĩ đến việc chỉ cần chủ động thực hiện một thay đổi nhỏ ngay trong ngày hôm nay, tương lai của chính bản thân họ cũng sẽ được định hình theo một hướng hoàn toàn khác."
> 
> -- Danh ngôn chia sẻ trên Twitter

(Hết)
