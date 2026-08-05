# 每周分享第 38 期 (Bản tin chia sẻ hàng tuần số 38)

Ghi lại những điều thú vị đáng chia sẻ tôi bắt gặp trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Chào mừng mọi người gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục [issue](https://github.com/ruanyf/weekly/issues) tại kho lưu trữ GitHub [ruanyf/weekly](https://github.com/ruanyf/weekly).

![](https://cdn.beekka.com/blogimg/asset/201901/bg2019010401.jpg)

(Ảnh bìa: Màn hình mực điện tử E-Ink hiển thị thông tin tại trạm xe buýt, Thượng Hải, 2018)

Gần đây tôi luôn trăn trở suy nghĩ: liệu các phương thức thanh toán qua điện thoại di động có thực sự tiện lợi như chúng ta vẫn tưởng?

Hiện tại, tôi có thể thoải mái tay không ra đường mà không cần mang theo bất kỳ thứ gì ngoài chiếc điện thoại. So với trước đây, đây rõ ràng là một bước tiến vô cùng tiện lợi. Tuy nhiên, mặt trái của sự tiện lợi này là tôi bắt buộc phải mang theo điện thoại mọi lúc mọi nơi. Trước đây là bắt buộc phải mang ví tiền, còn bây giờ là bắt buộc phải mang điện thoại. Nếu vô tình để quên điện thoại ở nhà, hoặc gặp sự cố rơi mất, hỏng hóc, hết pin giữa đường thì mọi thứ sẽ lập tức trở thành thảm họa: tôi không thể gọi điện liên lạc, không thể đi tàu điện ngầm và hoàn toàn không có cách nào để thanh toán mua sắm.

Giải pháp thanh toán tối ưu hơn có lẽ không phải là thanh toán qua điện thoại di động, mà phải là một phương thức xác thực sinh trắc học trực tiếp, ví dụ như thanh toán bằng nhận diện khuôn mặt (Face Pay). Chỉ cần hệ thống quét nhận diện khuôn mặt để xác định danh tính và tự động trừ tiền trong tài khoản liên kết, con người sẽ được giải phóng hoàn toàn khỏi sự phụ thuộc vào chiếc điện thoại. Tuy nhiên, phương án này lại đẩy toàn bộ chi phí đầu tư thiết bị và rủi ro kỹ thuật về phía các đơn vị bán hàng khi họ bắt buộc phải trang bị camera quét khuôn mặt chuyên dụng; và nếu thiết bị của họ gặp sự cố hỏng hóc, bạn vẫn không thể hoàn thành giao dịch.

Nhìn rộng hơn, tôi nhận thấy phương thức thanh toán càng tiện lợi thì hệ thống kỹ thuật vận hành phía sau lại càng phức tạp, đồng nghĩa với việc nó càng trở nên dễ bị tổn thương trước các sự cố hệ thống (fragile). Những phần việc phức tạp vốn thuộc về cá nhân (tự mang theo và bảo quản tiền mặt vật lý) nay đã được công nghệ đóng gói và xử lý tự động. Khi thời điểm toàn bộ xã hội loại bỏ hoàn toàn tiền giấy để chuyển dịch sang thanh toán số hóa tuyệt đối, yêu cầu đặt ra là hệ thống kỹ thuật phía sau không được phép xảy ra bất kỳ sai sót hay sự cố mất điện, mất mạng nào. Nếu xảy ra một sự cố mất điện trên diện rộng (blackout), chúng ta thậm chí sẽ không thể mua nổi những nhu yếu phẩm cơ bản và buộc phải quay lại phương thức ghi nợ thủ công thô sơ.

## 新闻 (Tin tức)

1、[Cảnh báo phương thức trộm xe hơi bằng cách khuếch đại sóng chìa khóa thông minh](https://www.cbc.ca/news/canada/toronto/car-thefts-rising-1.4930890)

![](https://cdn.beekka.com/blogimg/asset/201901/bg2019010402.jpg)

Tại Toronto (Canada) gần đây xuất hiện phương thức trộm xe hơi công nghệ cao nhắm vào các dòng xe sử dụng chìa khóa thông minh (smart key). Nhiều chủ xe có thói quen để chìa khóa trên tủ ngay gần cửa ra vào sau khi về nhà.

Tận dụng điều này, tin tặc sẽ tiếp cận cửa nhà trong đêm, sử dụng một thiết bị thu và khuếch đại sóng vô tuyến để bắt và chuyển tiếp tín hiệu của chìa khóa thông minh ra ngoài sân cho đồng bọn đứng cạnh xe. Đồng bọn sử dụng một thiết bị thu khác để phát tín hiệu giả lập đánh lừa hệ thống cảm biến của xe hơi, tự động mở cửa và khởi động xe phóng đi nhanh chóng mà không cần bẻ khóa cơ học.

2. **Dự án cải tạo các mỏ than bỏ hoang thành trang trại nông nghiệp thẳng đứng**

![](https://cdn.beekka.com/blogimg/asset/201901/bg2019010403.jpg)

Nhiều mỏ than cũ sở hữu hệ thống đường hầm sâu hun hút dưới lòng đất bị bỏ hoang sau khi khai thác hết tài nguyên. Các nhà khoa học Anh đang thử nghiệm giải pháp cải tạo các đường hầm này thành các trang trại nông nghiệp thẳng đứng (vertical farming).

Không gian sâu dưới lòng đất giúp bảo vệ cây trồng khỏi các biến động thời tiết thiên tai, đồng thời duy trì nhiệt độ và độ ẩm ổn định quanh năm. Hệ thống chiếu sáng sẽ được cung cấp bởi đèn LED hiệu năng cao hoặc các đường ống cáp quang dẫn ánh sáng mặt trời từ mặt đất xuống độ sâu 40 mét. Mô hình hứa hẹn mang lại năng lượng sạch tối ưu và năng suất cây trồng vượt trội so với canh tác nông nghiệp truyền thống trên mặt đất.

3、[Google Dịch cập nhật giao diện mới hỗ trợ tải lên dịch trực tiếp nhiều định dạng tài liệu](https://www.blog.google/products/translate/new-look-google-translate-web/)

Google Dịch (Google Translate) phiên bản web cập nhật giao diện mới trực quan hơn. Thay đổi kỹ thuật đáng chú ý nhất là việc bổ sung tính năng tải lên tài liệu trực tiếp, hỗ trợ dịch toàn bộ nội dung của các tệp tin định dạng `.doc`, `.docx`, `.pdf`, `.ppt`, `.pptx`, `.xls`, `.xlsx` mà vẫn giữ nguyên bố cục định dạng gốc của văn bản.

4. **Nghiên cứu khoa học nghi ngờ kỷ lục người thọ nhất lịch sử là giả mạo**

Cụ bà người Pháp Jeanne Calment được ghi nhận là người sống thọ nhất lịch sử nhân loại với tuổi thọ 122 tuổi (sinh năm 1875 và mất năm 1997). Tuy nhiên, một nhà nghiên cứu người Nga đã đưa ra bài phân tích nghi ngờ đây là một vụ giả mạo danh tính để trốn thuế và tiếp tục nhận lương hưu từ chính phủ.

Các phân tích nhân trắc học chỉ ra sự khác biệt lớn về khoảng cách giữa hai mắt và hình dạng tai trong các bức ảnh thời trẻ và khi về già của cụ. Tác giả đưa ra giả thuyết: người thực sự qua đời vào năm 1934 là cụ bà Jeanne Calment, và cô con gái Yvonne Calment đã quyết định mạo danh mẹ mình kể từ đó để tiếp tục nhận tiền trợ cấp tuổi già từ chính phủ cho đến khi qua đời vào năm 1997 ở độ tuổi thực tế là 99 tuổi.

5. **Qualcomm ra mắt dòng vi xử lý Snapdragon 8cx chuyên dụng cho máy tính xách tay**

Hãng chip Qualcomm giới thiệu dòng vi xử lý Snapdragon 8cx được sản xuất trên tiến trình 7nm dành riêng cho phân khúc laptop chạy Windows. Con chip kiến trúc ARM này tích hợp sẵn modem kết nối mạng di động 4G LTE tốc độ cao giúp máy tính luôn duy trì kết nối internet ngay cả khi ở chế độ ngủ (sleep mode) và mang lại thời lượng sử dụng pin vượt trội kéo dài hơn một ngày làm việc liên tục.

6. **Tập đoàn Volkswagen công bố lộ trình dừng phát triển động cơ đốt trong từ năm 2026**

Tập đoàn xe hơi Volkswagen (Đức) công bố kế hoạch ra mắt thế hệ động cơ chạy xăng và diesel cuối cùng vào năm 2026, trước khi chuyển dịch toàn bộ nguồn lực sang sản xuất xe thuần điện (EV) nhằm đáp ứng các tiêu chuẩn cắt giảm khí thải CO2 bảo vệ môi trường toàn cầu.

7、[Các nhà khoa học Nam Phi chế tạo gạch sinh học thân thiện môi trường từ nước tiểu](https://www.news-core.com/)

![](https://cdn.beekka.com/blogimg/asset/201901/bg2019010408.jpg)

Các kỹ sư xây dựng tại Đại học Cape Town (UCT) phát minh ra quy trình sản xuất vật liệu xây dựng độc đáo: sử dụng một chủng vi khuẩn đặc biệt để phân hủy urea trong nước tiểu, tạo ra phản ứng kết tủa canxi cacbonat (tương tự như cơ chế hình thành vỏ sò tự nhiên) để kết dính cát thành những viên gạch sinh học vững chắc ở nhiệt độ phòng. Quy trình giúp loại bỏ hoàn toàn khâu nung gạch ở nhiệt độ 1.400 độ C của gạch đất sét truyền thống vốn thải ra lượng lớn khí nhà kính.

8. **Thiết kế không gian khoang sinh hoạt của phi thuyền BFR tiến tới Sao Hỏa**

![](https://cdn.beekka.com/blogimg/asset/201901/bg2019010409.jpg)

Hành trình di chuyển đến Sao Hỏa kéo dài nhiều tháng trong không gian hẹp là thử thách tâm lý cực lớn đối với các phi hành gia. Thiết kế phi thuyền Big Falcon Rocket (BFR) của SpaceX bố trí khoảng 40 khoang sinh hoạt riêng biệt cho hành khách cùng các khu vực sinh hoạt chung rộng rãi dành cho hoạt động giải trí và tương tác xã hội để giảm thiểu hội chứng trầm cảm do không gian hẹp.

## 教程 (Hướng dẫn)

1、[Bài viết] [Tìm hiểu các kỹ thuật gỡ lỗi JavaScript bằng tính năng Breakpoint của Chrome DevTools](https://codeburst.io/learn-how-to-debug-javascript-with-chrome-devtools-9514c58479db) (Tiếng Anh)

Tài liệu hướng dẫn thực hành cách thiết lập các điểm dừng điều kiện (conditional breakpoints), theo dõi sự thay đổi của biến số qua Watch expressions và debug các sự kiện tương tác DOM trực quan trên trình duyệt.

2、[Bài viết] [Giải mã hiện tượng lịch sử tại sao phần lớn chủ cửa hàng photocopy tại Trung Quốc đều là người cùng một huyện](https://github.com/hangyan/Papers/blob/master/papers/%E6%96%B0%E5%8C%96%E5%A4%8D%E5%8D%B0%E4%BA%A7%E4%B8%9A%E7%9A%84%E7%94%9F%E5%91%BD%E5%8F%B2_%E5%86%AF%E5%86%9B%E6%97%97.pdf) (Chữ Trung)

Bản luận văn thạc sĩ xã hội học của Đại học Bắc Kinh điều tra hiện tượng kỳ lạ: hơn 70% số cửa hàng photocopy và in ấn tài liệu trên khắp Trung Quốc đều do người dân có gốc gác từ huyện Tân Hóa, tỉnh Hồ Nam làm chủ, giải mã mạng lưới kết nối đồng hương và chia sẻ bí quyết công nghệ sửa máy in cũ của dòng họ.

## 资源 (Tài nguyên)

1、[Sách] [CSS Animation 101 — Giáo trình học thiết kế chuyển động CSS Animation từ cơ bản](https://github.com/cssanimation/css-animation-101)

Sách hướng dẫn nguồn mở chi tiết giúp lập trình viên Frontend làm chủ các thuộc tính chuyển động `transition`, `keyframes` và các nguyên lý thiết kế chuyển động UI mượt mà trên trang web.

2、[Nhiếp ảnh] [Faces of Open Source — Bộ sưu tập chân dung nghệ thuật các lập trình viên thúc đẩy cuộc cách mạng nguồn mở](http://facesofopensource.com/)

![](https://cdn.beekka.com/blogimg/asset/201901/bg2019010413.jpg)

Dự án nhiếp ảnh ghi lại những bức chân dung nghệ thuật chất lượng cao của các tên tuổi lớn có đóng góp vĩ đại cho cộng đồng nguồn mở như Linus Torvalds, Richard Stallman kèm theo câu chuyện lịch sử của họ.

## 工具 (Công cụ)

1、[GAN Paint — Công cụ chỉnh sửa hình ảnh thông minh ứng dụng mạng GAN của MIT](http://gandissect.res.ibm.com/ganpaint.html)

Một ứng dụng web ấn tượng cho phép người dùng vẽ hoặc xóa các chi tiết kiến trúc (như cửa sổ, cây cối, gạch đá) trực tiếp trên ảnh chụp thực tế, thuật toán AI sẽ tự động sinh ra các điểm ảnh mới tương thích hoàn hảo với bối cảnh xung quanh.

2、[cloc — Công cụ dòng lệnh thống kê số dòng code chi tiết cho dự án](https://github.com/AlDanial/cloc)

Một công cụ siêu nhẹ và mạnh mẽ giúp lập trình viên nhanh chóng thống kê số lượng file nguồn, đếm số dòng code thực tế, dòng comment và dòng trống phân loại theo từng ngôn ngữ lập trình trong dự án.

## 文摘 (Văn trích)

1. **Khái niệm 'Premium Mediocre' (Sự bình dân hóa cao cấp) trong nền kinh tế tiếp thị**

Khái niệm "Premium Mediocre" mô tả chiến lược tiếp thị của các thương hiệu nhằm biến các sản phẩm bình dân trở nên sang chảnh hơn trong mắt người tiêu dùng bằng cách gắn thêm các nhãn mác như "thủ công" (artisanal), "精酿" (bia thủ công), "chữ ký của bếp trưởng". Chiến lược này cũng được các hãng thời trang xa xỉ áp dụng triệt để khi tung ra các dòng sản phẩm phụ kiện bình dân như ví da nhỏ, dép nhựa mang logo hãng để tiếp cận và khai thác phân khúc khách hàng đại chúng muốn sở hữu hào quang của thương hiệu cao cấp với mức giá dễ tiếp cận.

## 本周图片 (Hình ảnh tuần này)

1. **Cấu trúc nguồn doanh thu chính của các tập đoàn công nghệ lớn toàn cầu**

![](https://cdn.beekka.com/blogimg/asset/201901/bg2019010422.jpg)

Biểu đồ so sánh mô hình kinh doanh của các ông lớn công nghệ: doanh thu của Apple phụ thuộc 63% vào iPhone; Google phụ thuộc 88% vào quảng cáo; Facebook phụ thuộc 97% vào quảng cáo; trong khi Amazon có nguồn thu chính 72% từ bán lẻ hàng hóa và Microsoft phân bổ đều từ các mảng phần mềm Office, Windows và dịch vụ đám mây Azure.

## 本周金句 (Kim ngôn tuần này)

1、

> "Nếu bạn sở hữu một chiếc điện thoại thông minh cao cấp mua vào năm 2018 và không có nhu cầu chơi các tựa game đồ họa nặng, bạn hoàn toàn có thể duy trì sử dụng thiết bị này ổn định trong suốt 10 năm tới mà không cần nâng cấp do năng lực xử lý của chip di động hiện tại đã vượt xa nhu cầu sử dụng ứng dụng cơ bản hàng ngày của phần lớn người dùng."
> 
> -- Trích phân tích xu hướng thị trường di động.

2. **Cách thức Google cải tiến giao thức mạng TCP bằng giải pháp phát triển QUIC chạy trên UDP**

> "Tập đoàn Google mong muốn tối ưu hóa tốc độ của giao thức truyền tải dữ liệu TCP, nhưng do TCP được tích hợp và quản lý trực tiếp ở tầng nhân hệ điều hành (OS kernel) vốn rất khó để cập nhật đồng loạt trên mọi thiết bị toàn cầu, họ đã chọn giải pháp lập trình lại một giao thức truyền tải mới mang tên QUIC chạy đè lên giao thức UDP vốn cho phép tùy biến linh hoạt từ tầng ứng dụng."
> 
> -- Trích tài liệu mật mã học.

(Hết)
