# Bản tin chia sẻ công nghệ (Số 261): Cách tổ chức Hackathon đúng đắn

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3222) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070601.webp)

Tại thành phố Từ Khê, Ninh Ba, các nhà vườn đang tích cực thực hiện thụ phấn nhân tạo bằng tay cho hoa thanh long vào ban đêm. Hoa của cây thanh long thường chỉ bắt đầu nở bung sau khi mặt trời lặn hoàn toàn và sẽ tự động khép cánh lại vào sáng sớm ngày hôm sau. (Nguồn: [Nhân Dân Nhật Báo](http://zj.people.com.cn/n2/2023/0630/c370990-40477513-2.html))

## 黑客马拉松的正确方式

Bạn đã từng trực tiếp đăng ký tham gia một giải đấu Hackathon (Cuộc thi lập trình nhanh) nào chưa?

Đó là một thể thức thi tài lập trình, nơi các kỹ sư phần mềm tập trung tại một không gian làm việc (thường là một phòng hội nghị lớn), cùng nhau cật lực làm việc trong thời gian quy định để hoàn thiện dự án của mình trước khi ban giám khảo chấm điểm chọn ra đội chiến thắng.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070512.webp)

Hầu hết các giải Hackathon mà tôi biết đều diễn ra với bầu không khí vô cùng căng thẳng. Thí sinh bắt buộc phải hoàn thiện sản phẩm demo chạy được trong vòng 24 đến 48 tiếng liên tục, điều này đồng nghĩa với việc họ gần như không có thời gian ngủ và phải thức thâu đêm suốt sáng để viết code.

Dưới đây là một phần thể lệ thi đấu tiêu biểu của một giải Hackathon truyền thống:

> * **Quy mô đội ngũ**: Giới hạn số lượng thành viên tối đa của mỗi đội thi là 5 người.
> * **Sản phẩm bàn giao**: Các đội bắt buộc phải trình diễn được sản phẩm nguyên mẫu (prototype) chạy thực tế, có thể kết hợp trình chiếu slide thuyết trình hoặc video mô tả.
> * **Thể thức thi đấu**: Các đội thi tập trung làm việc tại một địa điểm tập trung và cùng thực hiện giải quyết một đề bài chung do ban tổ chức đưa ra trong thời gian quy định.

Tuy nhiên gần đây, khi vô tình đọc được thông báo tuyển thành viên tham gia một giải Hackathon quốc tế, tôi mới nhận ra chúng ta hoàn toàn có một cách tiếp cận khác nhân văn hơn, và tôi tin đó mới chính là cách tổ chức Hackathon đúng đắn nhất.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070201.webp)

Giải đấu này mang tên *“NixOS Ocean Sprint 2023”*, hướng tới mục tiêu tìm kiếm và vá các lỗ hổng bảo mật cho hệ điều hành NixOS.

Giải dự kiến tổ chức vào tháng 10 năm nay, mở đăng ký tự do cho tất cả các nhà phát triển trên thế giới để ban tổ chức sàng lọc chọn ra 20 ứng viên xuất sắc nhất tham dự vòng chung kết.

Điểm độc đáo nhất nằm ở địa điểm tổ chức vòng chung kết: Quần đảo Canary!

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070202.webp)

Đây là quần đảo nhiệt đới nổi tiếng của Tây Ban Nha nằm trên Đại Tây Dương, một thiên đường du lịch thu hút hàng triệu du khách quốc tế ghé thăm mỗi năm nhờ phong cảnh thiên nhiên tuyệt đẹp.

Ban tổ chức đã thuê trọn một căn biệt thự sang trọng có hồ bơi lớn làm không gian làm việc chung. Buổi tối các thí sinh sẽ về nghỉ ngơi tại khách sạn, ban ngày họ tập trung tại biệt thự để cùng nhau thảo luận và viết code:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070203.webp)

Mỗi khi cảm thấy mệt mỏi hay bí ý tưởng lập trình, thí sinh có thể thoải mái nhảy xuống hồ bơi thư giãn. Đến giờ ăn, tất cả mọi người sẽ cùng quây quần bên bàn tiệc buffet để ăn uống và trò chuyện vui vẻ:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070204.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070205.webp)

Vào sáng sớm hoặc chiều tối, bạn có thể tự do chạy bộ dọc bãi cát ven biển. Sau khi kết thúc giải đấu, các thành viên sẽ cùng nhau tham quan khám phá hòn đảo xinh đẹp.

Tôi lập tức nhận ra đây mới chính là cách thức vận hành đúng nghĩa của một ngày hội lập trình. Thể thức thi đấu tập trung kiểu giam lỏng trước đây quá nặng nề tính ganh đua giành giải thưởng, vô tình biến ngày hội công nghệ thành một cuộc đua vắt kiệt sức và làm mất đi hoàn toàn niềm vui giao lưu học hỏi.

Thực tế, kết quả thắng thua của một giải Hackathon kéo dài vài chục tiếng không quá quan trọng, khó có thể đòi hỏi một sản phẩm phần mềm hoàn hảo hay có giá trị thương mại lớn ra đời trong thời gian ngắn ngủi như vậy. Giá trị lớn nhất của sự kiện chính là việc tạo không gian cho những người trẻ xa lạ có cơ hội kết bạn, chia sẻ kiến thức và cùng nhau thảo luận các ý tưởng công nghệ mới. Thêm vào đó, việc kết hợp "lập trình + du lịch nghỉ dưỡng" tại một hòn đảo nhiệt đới xinh đẹp chắc chắn sẽ là những kỷ niệm khó quên trong đời mỗi lập trình viên.

Mô hình này hướng tới đúng tinh thần cốt lõi của thế giới Hacker: **Lập trình là để thỏa mãn sự tò mò, tìm kiếm niềm vui sáng tạo và khám phá giới hạn mới chứ không phải để đua tranh danh hiệu.**

Tôi hy vọng các đơn vị tổ chức Hackathon trong nước có thể tham khảo mô hình này, đưa địa điểm tổ chức tới các khu du lịch nghỉ dưỡng yên bình và thiết kế nhiều hoạt động giao lưu trò chuyện giữa các đội thi, đặt mục tiêu kết nối lên hàng đầu và thi đấu chỉ là thứ yếu.

## 指纹浏览器 AdsPower

Có khá nhiều phần mềm chất lượng do các đội ngũ kỹ sư trong nước phát triển nhưng do đặc thù phân khúc thị trường nên ít được biết đến ở thị trường nội địa, ngược lại sản phẩm lại ghi nhận sự thành công rất lớn tại thị trường quốc tế. Hôm nay, tôi xin giới thiệu một sản phẩm tiêu biểu như vậy: trình duyệt bảo mật AdsPower ([Trang tiếng Trung](https://www.adspower.net/), [Trang tiếng Anh](https://www.adspower.com/)).

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023063008.webp)

Đây là một trình duyệt chống dấu vân tay (Anti-detect Browser), hay nói chính xác hơn là **trình duyệt bảo vệ người dùng trước sự thu thập dấu vân tay trình duyệt của các trang web**.

Khái niệm "Dấu vân tay trình duyệt" (Browser Fingerprinting) là phương thức các trang web thu thập các thông số kỹ thuật phần cứng và phần mềm của máy khách để tạo nên một mã định danh duy nhất cho từng người dùng nhằm mục đích theo dõi hành vi trực tuyến, sử dụng nhiều kỹ thuật phân tích sâu:

* **Chỉ số vân tay cơ bản**: Chuỗi UserAgent, độ phân giải màn hình hiển thị, số nhân CPU, dung lượng RAM, danh sách plugin đã cài, ngôn ngữ hệ thống...
* **Chỉ số nâng cao**: Kỹ thuật render Canvas, WebGL, AudioContext xử lý âm thanh, giao thức WebRTC, danh mục phông chữ hệ thống...
* **Thông tin địa lý**: Địa chỉ IP, múi giờ hệ thống, cấu hình DNS, chứng chỉ bảo mật SSL...

Hầu như mọi website bạn ghé thăm hàng ngày đều có khả năng thu thập đầy đủ các thông số trên để định danh chính xác thiết bị của bạn.

Giải pháp bảo mật truyền thống là cài đặt thêm các tiện ích mở rộng để làm giả các thông số này thành dạng động. Tuy nhiên cách làm này đòi hỏi cấu hình phức tạp và khó áp dụng cho người dùng phổ thông.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070102.webp)

AdsPower đã giải quyết triệt để vấn đề này bằng cách xây dựng một trình duyệt độc lập tích hợp sẵn toàn bộ các giải pháp chống thu thập vân tay. Dưới đây là các tính năng cốt lõi của phần mềm:

1. **[Làm giả dấu vân tay trình duyệt linh hoạt](https://www.adspower.net/blog/338)**: Giúp người dùng hoàn toàn ẩn danh trên môi trường mạng và ngăn chặn các tracker theo dõi.
2. **Cấu hình môi trường duyệt web đa dạng**: Hỗ trợ chuyển đổi nhanh chóng giữa hai nhân trình duyệt Chromium (Chrome) và Gecko (Firefox).
3. **[Tự động hóa tác vụ](https://www.adspower.net/blog/339)**: Tích hợp các bộ công cụ giả lập hành vi người dùng để tự động hóa các tác vụ lặp đi lặp lại.
4. **[Đồng bộ hóa thao tác đa cửa sổ](https://www.adspower.net/news/379)**: Cho phép người dùng thao tác chuột và bàn phím trên một cửa sổ trình duyệt chính, các cửa sổ trình duyệt phụ ở các môi trường độc lập khác sẽ tự động đồng bộ theo thời gian thực.

Nhờ bộ tính năng mạnh mẽ này, AdsPower được ứng dụng rộng rãi trong các công việc thu thập dữ liệu lớn (web scraping), chạy thử nghiệm phần mềm tự động hóa và đặc biệt hữu dụng trong ngành thương mại điện tử như quản lý đồng thời nhiều gian hàng trực tuyến, quản trị nhiều tài khoản mạng xã hội hay xử lý các giao dịch thanh toán xuyên biên giới của doanh nghiệp.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070103.webp)

Để phục vụ phân khúc khách hàng doanh nghiệp, phần mềm cung cấp các tính năng quản lý phân quyền thành viên nhóm, cộng tác chia sẻ tài khoản và mã hóa dữ liệu an toàn với hệ thống máy chủ tăng tốc phân bố rộng khắp tại châu Á, châu Âu và châu Mỹ.

AdsPower hiện ghi nhận tốc độ tăng trưởng rất nhanh với hơn 80.000 người dùng thường xuyên trên toàn thế giới và được đánh giá cao tại thị trường các nước Đông Nam Á, Nam Á và châu Âu với việc hỗ trợ tới 12 ngôn ngữ giao diện khác nhau.

Phiên bản miễn phí của phần mềm hỗ trợ người dùng tạo lập và quản lý đồng thời 2 môi trường duyệt web độc lập. Bạn đọc có nhu cầu quản lý quy mô lớn hơn có thể đăng ký gói trả phí tùy theo nhu cầu sử dụng.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070104.webp)

Bạn đọc quan tâm có thể quét mã QR phía trên hoặc truy cập [Trang chủ AdsPower](https://www.adspower.net/) để tải về dùng thử và tham khảo tài liệu hướng dẫn sử dụng.

## 科技动态

1、[Anh thử nghiệm mô hình sưởi ấm bể bơi công cộng bằng nhiệt lượng tỏa ra từ phòng máy chủ](https://arstechnica.com/information-technology/2023/03/free-data-center-heat-is-allegedly-saving-a-struggling-public-pool-24k-a-year/)

Các phòng máy chủ (data centers) luôn tỏa ra một lượng nhiệt khổng lồ đòi hỏi chi phí làm mát rất lớn. Một doanh nghiệp tại Anh mới đây đã đưa ra giải pháp độc đáo: xây dựng hệ thống phòng máy mini đặt trực tiếp tại các bể bơi công cộng để tận dụng nhiệt lượng tỏa ra sưởi ấm cho nguồn nước bể bơi:

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032104.webp)

Hệ thống máy chủ phục vụ các tác vụ tính toán AI được ngâm trực tiếp trong bồn chứa chất lỏng tản nhiệt chuyên dụng. Dòng chất lỏng mang nhiệt lượng này sau đó được dẫn qua bộ trao đổi nhiệt kết nối trực tiếp với hệ thống đường ống lọc nước của bể bơi để truyền nhiệt làm ấm nước.

Doanh nghiệp cho biết giải pháp này giúp bể bơi công cộng cắt giảm tới 62% chi phí nhiên liệu đốt sưởi ấm nước hàng năm, đồng thời giúp công ty máy chủ tiết kiệm chi phí vận hành quạt gió làm mát.

2、[Mẫu điện thoại di động thông minh sở hữu điểm số dễ dàng sửa chữa cao nhất thế giới](https://arstechnica.com/gadgets/2023/07/fairphone-is-coming-to-america/)

Theo bảng xếp hạng tháo rã đồ công nghệ của chuyên trang iFixit, mẫu điện thoại Fairphone 4 do một doanh nghiệp Hà Lan sản xuất đã xuất sắc đạt điểm số tối đa 10/10 về tiêu chí dễ dàng tự sửa chữa và thay thế linh kiện:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070506.webp)

Toàn bộ cấu trúc bên trong của máy được thiết kế dưới dạng các khối module độc lập liên kết với nhau bằng ốc vít tiêu chuẩn. Người dùng thông thường chỉ cần sử dụng một chiếc tuốc nơ vít nhỏ là có thể tự tháo mở máy và thay thế màn hình, pin hay camera bị hỏng trong vài phút:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070507.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070508.webp)

Hạn chế lớn nhất của dòng sản phẩm này nằm ở cấu hình phần cứng tương đối lỗi thời (chip Qualcomm Snapdragon 750G, RAM 8GB) nhưng lại được định giá khá cao lên tới 700 Euro (khoảng 18 triệu đồng). Mức giá đắt đỏ này được cho là khó thuyết phục những người dùng đam mê công nghệ lựa chọn dù sản phẩm sở hữu tính năng bảo vệ môi trường độc đáo.

3、[Đường sắt Anh lên kế hoạch đóng cửa toàn bộ các phòng bán vé tàu truyền thống](https://www.sohu.com/a/694826920_119038)

Hiệp hội Đường sắt Anh vừa công bố kế hoạch đóng cửa toàn bộ hệ thống quầy bán vé tàu hỏa trực tiếp tại các nhà ga trên toàn quốc trong vòng 3 năm tới:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070509.webp)

Hành khách có nhu cầu mua vé tàu sau này sẽ được hướng dẫn tự mua qua các máy bán vé tự động bố trí tại ga hoặc đặt mua trực tuyến qua ứng dụng di động. Việc cắt giảm quầy bán vé trực tiếp giúp các hãng đường sắt tiết kiệm chi phí nhân sự vận hành rất lớn. Xu hướng tự động hóa này đang diễn ra mạnh mẽ trên thế giới, tương tự như việc Bảo tàng Cố Cung ở Bắc Kinh đã dỡ bỏ hoàn toàn quầy bán vé giấy trực tiếp từ nhiều năm trước để chuyển sang đặt vé online.

4、[Thử nghiệm ứng dụng công nghệ thực tế ảo giúp giảm lượng thuốc gây mê trong phẫu thuật](https://www.technologyreview.com/2022/09/21/1059869/patients-virtual-reality-surgery-anesthetic/)

Các nhà nghiên cứu tại Đại học Y khoa Colorado, Mỹ đã tiến hành thử nghiệm phương pháp cho bệnh nhân đeo kính thực tế ảo VR trong suốt quá trình phẫu thuật ngoại khoa để giảm bớt lượng thuốc gây mê cần sử dụng:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092903.webp)

Trong lúc bác sĩ thực hiện phẫu thuật, bệnh nhân sẽ đeo kính VR để xem các video phong cảnh thiên nhiên 3D yên bình như đồng cỏ, rừng thông hay bầu trời sao kết hợp nghe nhạc thiền thư giãn. Kết quả lâm sàng cho thấy nhóm bệnh nhân đeo kính VR đòi hỏi lượng thuốc gây mê ít hơn hẳn so với nhóm đối chứng.

Các bác sĩ nhận định hình ảnh VR giúp đánh lạc hướng sự tập trung của não bộ vào cơn đau và làm giảm nhịp tim căng thẳng của bệnh nhân, nhờ đó giúp người bệnh phục hồi nhanh hơn sau phẫu thuật nhờ giảm thiểu các tác dụng phụ của thuốc gây mê.

## 文章

1\. [Phân tích tác động của lệnh hạn chế xuất khẩu hai kim loại bán dẫn Gali và Gecmani của Trung Quốc](https://m.laoyaoba.com/n/867801)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070409.webp)

Bộ Thương mại Trung Quốc mới đây đã công bố áp đặt quy định kiểm soát xuất khẩu đối với hai kim loại hiếm là Gali và Gecmani – hai nguyên liệu đầu vào cốt lõi để chế tạo chip bán dẫn và thiết bị quang điện tử. Bài viết phân tích các ứng dụng công nghiệp quan trọng của hai nguyên liệu này và tác động của lệnh cấm đối với chuỗi cung ứng công nghệ toàn cầu.

2\. [Nhìn lại câu chuyện lịch sử thành lập tập đoàn sản xuất chip SMIC tại Thượng Hải](https://www.eet-china.com/mp/a232813.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070408.webp)

Bài hồi ký ý nghĩa ghi lại những đóng góp to lớn của cố kỹ sư Giang Thượng Chu vào năm 2001 trong việc thuyết phục chính quyền thành phố Thượng Hải đưa ra các cơ chế ưu đãi đặc biệt để thu hút đội ngũ sáng lập xây dựng nên tập đoàn đúc chip SMIC hàng đầu cả nước hiện nay.

3\. [Giới thiệu các công cụ phần mềm tự học tiếng Anh hiệu quả](https://sspai.com/post/80086)（Tiếng Trung）

Tác giả chia sẻ kinh nghiệm sử dụng và đánh giá chi tiết các ứng dụng di động, tiện ích mở rộng trình duyệt và dịch vụ trực tuyến giúp nâng cao hiệu quả tự học từ vựng và rèn luyện kỹ năng nghe nói tiếng Anh hàng ngày.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070105.webp)

4\. [Hướng dẫn nhúng tính năng bình luận bằng GitHub Issues vào trang blog tĩnh](https://richard-docs.netlify.app/blogs/b-027)（Tiếng Trung）

Bài viết hướng dẫn chi tiết cách thức cấu hình cho các trang blog tĩnh xây dựng bằng VitePress có thể tích hợp hệ thống bình luận Utterances hoặc Giscus: tận dụng API của GitHub để biến phần Issue của repo dự án thành nơi lưu trữ và hiển thị các bình luận của bạn đọc. (Đóng góp của [@Richard-Zhang1019](https://github.com/ruanyf/weekly/issues/3237))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070405.webp)

5\. [Tại sao việc phát triển hệ thống xác thực OAuth vẫn luôn là bài toán khó](https://www.nango.dev/blog/why-is-oauth-still-hard)（Tiếng Anh）

OAuth là giao thức xác thực phân quyền được ứng dụng rộng rãi nhất hiện nay trên Internet. Bài viết phân tích các điểm nghẽn kỹ thuật phức tạp trong cơ chế trao đổi khóa (token exchange) khiến các lập trình viên vẫn gặp nhiều lỗi bảo mật khi tự tay cấu hình hệ thống này. Bạn đọc cũng có thể tham khảo thêm [Bài viết giới thiệu tổng quan về OAuth2](https://metacpan.org/dist/LWP-Authen-OAuth2/view/lib/LWP/Authen/OAuth2/Overview.pod) để nắm vững lý thuyết nền tảng.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042601.webp)

6\. [Hướng dẫn cài đặt hệ điều hành Linux trên các dòng MacBook Air đời cũ](https://boilingsteam.com/liberating-the-macbook-air-2013-with-linux-complete-guide/)（Tiếng Anh）

Bài viết hướng dẫn chi tiết từng bước chuẩn bị phân vùng ổ cứng, tạo USB boot và cấu hình driver để cài đặt hoàn thiện hệ điều hành Linux chạy mượt mà trên chiếc MacBook Air 2013 cũ, giúp tận dụng lại hiệu năng phần cứng cũ để làm máy chủ cá nhân.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040601.webp)

7\. [Phân tích sự khác biệt về cấu trúc dữ liệu giữa MySQL và MariaDB](https://www.skeema.io/blog/2023/05/10/mysql-vs-mariadb-schema/)（Tiếng Anh）

MariaDB vốn được tách ra từ nhánh mã nguồn mở của MySQL. Bài viết phân tích sâu các điểm khác biệt đã phát sinh sau nhiều năm phát triển độc lập giữa hai hệ quản trị CSDL quan hệ này, đặc biệt là sự khác nhau trong cú pháp định nghĩa bảng dữ liệu (schema) và các công cụ tối ưu hóa truy vấn.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051201.webp)

8\. [Kỷ nguyên chạy đua kích thước mô hình AI lớn dường như đã chạm giới hạn](https://www.economist.com/science-and-technology/2023/06/21/the-bigger-is-better-approach-to-ai-is-running-out-of-road)（Tiếng Anh）

Bài viết phân tích trên tạp chí *The Economist* chỉ ra rằng phương pháp huấn luyện AI bằng cách liên tục gia tăng số lượng tham số và nạp thêm dữ liệu khổng lồ đang gặp phải rào cản lớn về chi phí phần cứng và sự cạn kiệt nguồn dữ liệu chất lượng trên Internet, dự báo hướng đi tiếp theo sẽ chuyển dịch sang tối ưu hóa thuật toán và tinh chỉnh chuyên sâu các mô hình cỡ nhỏ.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062507.webp)

## 工具

1、[jianmu: Công cụ tự động hóa quy trình CI/CD hỗ trợ giao diện kéo thả trực quan](https://jianmu.dev/)

Hệ thống quản lý quy trình CI/CD nguồn mở của Trung Quốc, cho phép các kỹ sư DevOps thiết lập luồng build và deploy ứng dụng thông qua giao diện kéo thả các khối chức năng trực quan. (Đóng góp của [@lxitgto](https://github.com/ruanyf/weekly/issues/3233))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070404.webp)

2、[Milky Warp: Ứng dụng kính lúp phóng to vùng màn hình máy tính](https://github.com/hugoattal/milky-warp)

Phần mềm nhỏ gọn chạy trên desktop cho phép người dùng nhanh chóng tạo ra một vùng kính lúp di động để phóng to các chi tiết nhỏ trên màn hình, rất tiện lợi cho các lập trình viên hoặc nhà thiết kế đồ họa khi cần soi chi tiết pixel giao diện.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070402.webp)

3、[ICP Query: Tiện ích tra cứu nhanh thông tin đăng ký tên miền website](https://github.com/yuedanlabs/icp-query-extension)

Extension mã nguồn mở dành cho trình duyệt Chrome giúp người dùng kiểm tra nhanh giấy phép đăng ký ICP, thông tin Whois, bản ghi DNS, vị trí máy chủ vật lý và nhà cung cấp dịch vụ mạng của website đang truy cập. (Đóng góp của [@yuedanlabs](https://github.com/ruanyf/weekly/issues/3223))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070401.webp)

4、[艺码 (Yima): Tiện ích web tạo tranh vẽ nghệ thuật từ mã QR bằng AI](https://yima.me/)

Ứng dụng web trực tuyến cho phép người dùng dán liên kết mã QR và gõ mô tả bức tranh mong muốn, AI sẽ tự động tính toán phối màu để vẽ nên một bức tranh nghệ thuật độc đáo có lồng ghép mã QR quét được. (Đóng góp của [@Cobb9527](https://github.com/ruanyf/weekly/issues/3226))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070403.webp)

5、[Language Reactor: Tiện ích hỗ trợ hiển thị song ngữ phụ đề trên Youtube](https://www.languagereactor.com/)

Extension trình duyệt hỗ trợ dịch và hiển thị đồng thời hai dòng phụ đề ngôn ngữ khác nhau khi xem phim trên Netflix hoặc Youtube, đi kèm tính năng nhấp chuột vào từ vựng để tra nghĩa trực tiếp rất hữu ích cho người học ngoại ngữ.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050701.webp)

6、[Directus: Công cụ tự động tạo hệ thống API cho cơ sở dữ liệu](https://github.com/directus/directus)

Giải pháp mã nguồn mở chạy trực tiếp trên các hệ quản trị cơ sở dữ liệu hiện có để tự động phân tích và sinh ra hệ thống API REST và GraphQL tương ứng, đi kèm giao diện quản trị Admin trực quan.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050905.webp)

7、[CheerpJ: Trình chạy mã nguồn Java trực tiếp trên môi trường web](https://leaningtech.com/announcing-cheerpj-3-0-a-jvm-replacement-in-html5-and-webassembly-to-run-java-applications-and-applets-on-modern-browsers/)

Dự án thử nghiệm công nghệ giúp chuyển đổi môi trường máy ảo JVM chạy trực tiếp trên trình duyệt web thông qua WebAssembly, cho phép các ứng dụng Java Applet đời cũ có thể chạy trực tiếp trên web mà không cần cài đặt phần mềm Java ngoài.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051003.webp)

8、[SailboatUI: Bộ sưu tập các component giao diện xây dựng trên Tailwind CSS](https://sailboatui.com/)

Bộ thư viện mã nguồn mở cung cấp hơn 150 thành phần giao diện (UI components) HTML được thiết kế đẹp mắt và tối ưu hóa CSS bằng Tailwind CSS giúp lập trình viên Front-end đẩy nhanh tiến độ làm giao diện web.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022123103.webp)

9、[komorebi: Trình quản lý sắp xếp cửa sổ ứng dụng tự động trên Windows](https://github.com/LGUG2Z/komorebi)

Tiện ích hỗ trợ người dùng Windows tự động sắp xếp và chia nhỏ các cửa sổ ứng dụng đang mở trên màn hình theo dạng lưới (Tiling Window Manager) tương tự như các môi trường desktop của Linux.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101201.webp)

10、[WezTerm: Ứng dụng terminal giả lập đa nền tảng tăng tốc đồ họa bằng GPU](https://wezfurlong.org/wezterm/)

Một ứng dụng terminal dòng lệnh mã nguồn mở hỗ trợ cấu hình bằng ngôn ngữ Lua, tận dụng sức mạnh xử lý đồ họa của GPU để tăng tốc độ cuộn hiển thị văn bản dòng lệnh. Một giải pháp terminal dựa trên công nghệ web khác cũng rất đáng trải nghiệm là [Hyper](https://hyper.is/) phát triển trên nhân Electron.

![](https://cdn.beekka.com/blogimg/asset/220204/bg2022042503.webp)

## 资源

1、[WebAuthn.wtf: Trang thông tin tổng hợp kiến thức về giao thức WebAuthn](https://webauthn.wtf/)

Trang web lưu trữ tài liệu giải thích chi tiết cấu trúc kỹ thuật và hướng dẫn lập trình tích hợp giao thức đăng nhập bảo mật không mật khẩu WebAuthn dành cho các nhà phát triển hệ thống.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050803.webp)

2、[mess with DNS: Trang web thử nghiệm cấu hình DNS miễn phí](https://messwithdns.net/)

Một dịch vụ web hữu ích cung cấp cho mỗi người dùng truy cập một tên miền con miễn phí kèm theo giao diện quản trị trực quan, giúp lập trình viên thực hành cấu hình các bản ghi DNS (A, CNAME, MX...) và quan sát kết quả cập nhật ngay lập tức.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050906.webp)

3、[68k.news: Trang web chuyển đổi tin tức Google News sang dạng văn bản thuần](http://68k.news/)

Dịch vụ web hỗ trợ trích xuất toàn bộ nội dung tin tức từ Google News và chuyển đổi thành giao diện văn bản thuần túy không chứa quảng cáo hay ảnh nặng, giúp các thiết bị máy tính đời cổ có cấu hình yếu vẫn có thể cập nhật tin tức nhanh chóng.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040208.webp)

4、[Pirate Weather: Dịch vụ API cung cấp thông tin dự báo thời tiết miễn phí](https://pirateweather.net/)

Dịch vụ cung cấp API thời tiết miễn phí dành cho các nhà phát triển ứng dụng, hỗ trợ hạn mức gọi API lên tới 20.000 lượt mỗi tháng.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011105.webp)

5、[APIVault: Công cụ tìm kiếm danh mục các API công cộng hữu ích](https://apivault.dev/)

Trang web tổng hợp và phân loại hàng ngàn dịch vụ API công cộng miễn phí trên thế giới, hoạt động như một công cụ tìm kiếm giúp lập trình viên tìm ra các nguồn cấp dữ liệu phù hợp cho dự án của mình.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052502.webp)

## 图片

1、**Hệ thống tản nhiệt nước khổng lồ của siêu máy tính nhanh nhất thế giới**

Tại Phòng thí nghiệm Quốc gia Oak Ridge thuộc bang Tennessee, Mỹ đang vận hành hệ thống siêu máy tính nhanh nhất thế giới mang tên Frontier với tốc độ tính toán đạt mức Exascale (百亿亿次):

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011208.webp)

Siêu máy tính này chiếm diện tích mặt sàn hơn 600 mét vuông với hơn 9.000 nút tính toán độc lập. Để giải quyết lượng nhiệt khổng lồ tỏa ra khi vận hành, hệ thống yêu cầu dòng nước làm mát tuần hoàn liên tục có khối lượng lên tới hơn 20 tấn. Hình ảnh dưới đây phác họa hệ thống đường ống nước lạnh của nó:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011209.webp)

Hệ thống nước làm mát tuần hoàn này nặng tới hơn 400 tấn và yêu cầu các máy bơm áp lực lớn hoạt động liên tục:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011210.webp)

Tại mỗi tủ rack tính toán, các đường ống nước xanh biểu thị dòng nước lạnh đi vào và đường ống đỏ dẫn nước nóng đi ra sau khi hấp thụ nhiệt từ chip xử lý:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011211.webp)

Toàn bộ siêu máy tính bao gồm 74 tủ rack lớn với tổng chiều dài dây cáp kết nối bên trong lên tới hơn 118 km, cho thấy độ phức tạp khổng lồ của cơ sở hạ tầng này:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011212.webp)

2、**Mô hình mô phỏng kích thước quả tim lớn nhất thế giới của loài cá voi xanh**

Cá voi xanh là loài động vật có kích thước cơ thể lớn nhất từng được ghi nhận trong lịch sử Trái Đất.

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081202.webp)

Đi kèm với thân hình khổng lồ đó là một quả tim có kích thước lớn nhất trong thế giới tự nhiên, tương đương với thể tích của một căn phòng nhỏ:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081203.webp)

Để có thể bơm máu đi nuôi dưỡng toàn bộ cơ thể khổng lồ dài hàng chục mét, cơ tim của cá voi xanh phải tạo ra một áp lực co bóp cực lớn. Giới sinh vật học chỉ ra rằng giới hạn áp lực mạch máu này cũng chính là yếu tố tự nhiên ngăn cản các loài động vật có vú phát triển cơ thể vượt quá kích thước của cá voi xanh.

## ✍️ Bài đọc thêm

### Tại sao tốc độ phát triển phần mềm lại quyết định lớn tới chi phí của doanh nghiệp?

Để giảm thiểu chi phí vận hành mảng công nghệ của một doanh nghiệp, chúng ta thường tập trung vào hai hướng tiếp cận chính:

1. **Gia tăng tốc độ viết mã của lập trình viên**: Tránh việc kéo dài thời gian phát triển dự án gây thâm hụt nguồn vốn.
2. **Tối ưu hóa hiệu năng phần mềm**: Giúp giảm thiểu lượng tài nguyên phần cứng máy chủ cần sử dụng.

Vậy hướng đi nào mang lại hiệu quả cắt giảm chi phí rõ rệt hơn cho doanh nghiệp?

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070602.webp)

Chúng ta hãy cùng phân tích các số liệu thực tế được công bố bởi tập đoàn Google vào năm 2020:

Vào năm 2020, tổng lượng điện năng tiêu thụ cho toàn bộ hệ thống máy chủ và văn phòng của Google đạt mức 15,5 TWh. Nếu tính theo mức giá điện công nghiệp trung bình tại bang California (khoảng 0,199 USD mỗi kWh), tổng chi phí tiền điện của Google rơi vào khoảng **3,08 tỷ USD**.

Cũng trong năm đó, số lượng kỹ sư phần mềm làm việc tại Google ghi nhận khoảng 27.169 nhân sự. Nếu tạm tính theo mức lương bình quân hàng năm của một lập trình viên cấp trung tại Silicon Valley (khoảng 178.751 USD), chi phí tiền lương nhân sự của Google đã lên tới **4,85 tỷ USD**.

Báo cáo cho thấy chi phí tiền lương chi trả cho đội ngũ kỹ sư lập trình lớn hơn nhiều so với chi phí tiền điện để vận hành hệ thống máy chủ.

Việc gia tăng tốc độ viết mã của lập trình viên sẽ giúp doanh nghiệp tiết kiệm trực tiếp chi phí nhân sự phát triển, trong khi việc tối ưu hóa hiệu năng code giúp tiết kiệm chi phí điện năng máy chủ. Do đó, việc tập trung đầu tư tối ưu hóa tốc độ và năng suất làm việc của lập trình viên thường đem lại hiệu quả cắt giảm chi phí vận hành rõ rệt hơn cho các doanh nghiệp công nghệ lớn.

## Lịch sử tuần này

- 2022年（第 214 期）：[Thông tin địa lý: Tại sao hầu hết các bản đồ thế giới phẳng chúng ta xem hàng ngày đều bị sai lệch tỷ lệ](https://www.ruanyifeng.com/blog/2022/07/weekly-issue-214.html)
- 2021年（第 164 期）：[Đào tạo nghề: So sánh tỷ lệ tìm kiếm việc làm thành công giữa học viên các trung tâm code camp và sinh viên đại học](https://www.ruanyifeng.com/blog/2021/06/weekly-issue-164.html)
- 2020年（第 114 期）：[Xã hội số: Khái niệm về phong cách sống tự do và xu hướng làm việc tự do trong nền kinh tế gig](https://www.ruanyifeng.com/blog/2020/07/weekly-issue-114.html)
- 2019年（第 64 期）：[Sự nghiệp công nghệ: Hướng đi nào cho các nhân sự mới muốn gia nhập ngành công nghiệp Internet](https://www.ruanyifeng.com/blog/2019/07/weekly-issue-64.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge organization smooth and efficient.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
