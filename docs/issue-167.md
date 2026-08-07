# 科技爱好者周刊（第 167 期）：广告拦截器太过分了

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1826) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071518.jpg)

Danh họa thời Phục hưng Michelangelo từng lên ý tưởng thiết kế một cây cầu bắc qua sông Tiber ở Rome nhưng chưa từng được thực hiện khi ông còn sống. Mới đây, một nhóm nghệ sĩ Pháp đã hiện thực hóa ý tưởng này bằng cách sử dụng ba quả khinh khí cầu helium khổng lồ để nâng một cây cầu mô hình dài 18 mét bay lơ lửng trên không trung ngay tại vị trí thiết kế năm xưa. (Nguồn: [Yahoo News](https://news.yahoo.com/flying-bridge-inspired-michelangelo-floats-170727926.html))

## 主带话题：Các bộ chặn quảng cáo đã đi quá giới hạn

Trong một số phát hành tháng trước của bản tin, đã xảy ra một chuyện kỳ lạ. Một độc giả để lại bình luận trên blog cá nhân của tôi: "Tại sao lại thiếu mất hai đoạn nội dung vậy, có phải anh bị sót bài không?" Trên trình duyệt của anh ấy, hai đoạn văn đã biến mất hoàn toàn.

Sau đó tôi mới phát hiện ra nguyên nhân: bộ chặn quảng cáo (ad blocker) đã tự động ẩn hai đoạn văn đó đi. Tuần này tôi muốn thảo luận về vấn đề này.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071411.jpg)

Đối với những độc giả chưa rõ, tôi xin giải thích ngắn gọn: Bộ chặn quảng cáo là các extension trình duyệt được thiết kế để phát hiện và ngăn chặn các mã quảng cáo hiển thị trên trang web.

Các extension này hoạt động dựa trên một bộ quy tắc lọc (filter rules) được cấu hình sẵn. Khi phát hiện bất kỳ phần tử nào trên trang web khớp với các quy tắc này, nó sẽ tự động ẩn đi hoặc ngăn không cho tải. Ví dụ, nó sẽ chặn tệp tin mã nguồn có tên là `ad.js` chỉ vì tên tệp chứa ký tự "ad" (quảng cáo).

Các bộ quy tắc lọc này chủ yếu được duy trì và chia sẻ thông qua các danh sách lọc (filter lists) nổi tiếng trên mạng, được các extension tải về cập nhật tự động hàng ngày. Hình ảnh dưới đây là giao diện cấu hình danh sách lọc.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071412.jpg)

**Easylist** là một trong những danh sách lọc nổi tiếng nhất, hầu như extension chặn quảng cáo nào cũng tích hợp mặc định. Danh sách này còn có các phiên bản tối ưu hóa cho từng quốc gia, người dùng thường cài thêm phiên bản tối ưu cho quốc gia của mình.

Nhấp vào tệp tin quy tắc lọc, tôi thử tìm kiếm từ khóa "ruanyifeng.com". Tôi rất ngạc nhiên khi thấy có tới mười mấy quy tắc được viết riêng để chặn nội dung trên trang blog cá nhân của mình.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071413.jpg)

Dưới đây là một số ví dụ quy tắc lọc cụ thể được áp dụng riêng cho blog của tôi:

```text
! Chặn tệp tin script checker.js
ruanyifeng.com/blog/checker.js

! Ẩn các liên kết rút gọn dạng t.cn
ruanyifeng.com##a[href^="http://t.cn/"]

! Ẩn các đoạn văn chứa từ khóa "đào tạo" (培训)
ruanyifeng.com##p:-abp-contains(培训)
```

Quy tắc cuối cùng ở trên quy định rằng bất kỳ đoạn văn nào tôi viết chứa từ khóa "đào tạo" (培训) sẽ tự động bị ẩn đi. Đó chính là lý do độc giả của tôi bị mất hai đoạn nội dung, chỉ vì trong đó xuất hiện từ khóa này (liên quan đến khóa học giới thiệu trong bản tin).

Thậm chí còn có một quy tắc cực đoan hơn xuất hiện trong một số danh sách lọc:

```text
ruanyifeng.com^$csp=script-src 'none'
```

Quy tắc này sẽ chặn toàn bộ các tệp tin script JS (bao gồm cả inline script lẫn external script) trên trang để ngăn chặn các biện pháp chống chặn quảng cáo của quản trị viên. Trang web của bạn lập tức bị tê liệt tính năng JS, vô cùng độc đoán. Nếu muốn tìm hiểu sâu về cú pháp viết bộ lọc, bạn có thể tham khảo tài liệu hướng dẫn và cheat sheet chính thức của Adblock Plus.

Tôi hoàn toàn hiểu được việc người dùng không thích xem quảng cáo. Nhưng việc các bộ chặn quảng cáo tự ý ẩn các đoạn văn bản thường, chặn các script hệ thống và thay đổi giao diện trang web mà không được sự đồng ý của tác giả là một hành vi can thiệp thô bạo. Nó khiến độc giả lầm tưởng rằng trang web bị lỗi kỹ thuật, làm tổn hại nghiêm trọng đến uy tín của trang web và không hề thể hiện sự tôn trọng tối thiểu đối với tác giả tạo nội dung.

Do các extension chạy ở cấp đặc quyền cao hơn trang web, các quản trị viên web gần như không có khả năng chống đỡ. Lẽ ra các trình duyệt nên giới hạn quyền hạn của các plugin này, hoặc cung cấp cho các chủ trang web khả năng phát hiện và từ chối dịch vụ khi phát hiện plugin can thiệp thô bạo vào nội dung trang.

Không thể phủ nhận rằng một trang web không quảng cáo sẽ hiển thị sạch sẽ và tải nhanh hơn. Tuy nhiên, quảng cáo là một phần thiết yếu giúp duy trì tài chính vận hành cho các trang web chia sẻ tri thức miễn phí. Thế giới thực xung quanh chúng ta tràn ngập quảng cáo trên đường phố, trên tivi, trong mọi ứng dụng di động. Chúng ta chấp nhận sống chung với chúng nhưng lại tỏ ra cực đoan tuyệt đối không cho phép một trang web cá nhân nhỏ hiển thị vài banner quảng cáo để duy trì máy chủ, điều này có phải quá khắt khe hay không?

## Khóa học xây dựng HTTP Server bằng Node.js

Nếu bạn muốn bước chân vào ngành công nghệ thông tin và trở thành một kỹ sư phần mềm, con đường dễ tiếp cận nhất chính là Front-end. So với các nhánh khác như Backend, Hệ thống hay Đồ họa, lập trình Front-end dễ học trực quan hơn và nhu cầu tuyển dụng trên thị trường luôn rất lớn.

Dù bạn chọn phát triển web, app di động hay tiểu ứng dụng (Mini Program) thì có một nền tảng bạn bắt buộc phải làm quen, đó chính là **Node.js**. Hệ thống quản lý thư viện npm và các công cụ đóng gói hiện đại của Front-end đều vận hành trên nền tảng này.

Tuần này, chúng tôi giới thiệu khóa học thực hành **《Writing an HTTP Server with Node.js》** giúp bạn làm chủ nền tảng này:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071509.jpg)

Giáo trình đi từ cơ bản hướng dẫn học viên viết vài dòng code để dựng một máy chủ web tĩnh, giải thích chi tiết cấu trúc giao thức HTTP (phương thức GET/POST), cho đến tự tay thiết kế các API RESTful hoàn chỉnh hỗ trợ CORS (chia sẻ tài nguyên chéo nguồn) và tối ưu hóa bộ nhớ đệm (cache) trình duyệt.

Nội dung chi tiết của khóa học:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071511.jpg)

Khóa học do chuyên gia吴阳 (thành viên dự án Date-fns) trực tiếp giảng dạy trên nền tảng học tập **Geek Time**. Học viên sẽ được hướng dẫn viết code Node.js thực tế tích hợp các tính năng nâng cao như tải file ngắt quãng (breakpoint download) phục vụ dự án thực tế.

Độc giả bản tin có thể đăng ký khóa học hoàn toàn **miễn phí (0đ)** bằng cách quét mã QR dưới đây để kết nối với trợ lý khóa học:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071510.jpg)

## 科技动态

1、[Virgin Galactic hoàn thành chuyến bay thương mại đầu tiên lên rìa vũ trụ](https://www.yahoo.com/news/richard-branson-virgin-galactic-delay-125709148.html)

Vào ngày 11 tháng 7, tàu vũ trụ chở khách VSS Unity của hãng Virgin Galactic đã thực hiện thành công chuyến bay thử nghiệm chở người đầu tiên lên độ cao 86 km cách mặt đất (vùng ranh giới bắt đầu của không gian theo quy định của NASA).

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071202.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071203.jpg)

Trong chuyến bay, một máy bay chuyên dụng khổng lồ đã đưa tàu vũ trụ lên độ cao lớn trước khi tàu kích hoạt động cơ tên lửa đẩy để bứt phá khỏi lực hút Trái Đất hướng lên tầng bình lưu:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071206.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071204.jpg)

Tỷ phú 70 tuổi Richard Branson - nhà sáng lập hãng Virgin Galactic đã trực tiếp tham gia chuyến bay cùng 5 thành viên phi hành đoàn để trải nghiệm trạng thái không trọng lực trong khoảng 5 phút. Virgin Galactic dự kiến sẽ bắt đầu mở bán dịch vụ du lịch không gian thương mại từ năm tới với mức giá khoảng 250.000 USD mỗi vé.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071205.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071207.jpg)

2、[Bose ra mắt dòng máy trợ thính bán trực tiếp không cần đơn thuốc giá rẻ](https://www.fiercebiotech.com/medtech/bose-finally-launches-its-direct-to-consumer-soundcontrol-hearing-aid)

Các thiết bị máy trợ thính chuyên dụng tại Mỹ thường có giá rất đắt đỏ, dao động từ 5.000 đến 10.000 USD do quy định bắt buộc người dùng phải có đơn thuốc chỉ định của bác sĩ chuyên khoa và chi phí đo khám y tế đi kèm.

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021053106.jpg)

Để thay đổi thực trạng này, chính phủ Mỹ đã ban hành luật mới cho phép bán trực tiếp các dòng máy trợ thính không kê đơn (OTC). Hãng thiết bị âm thanh Bose đã tiên phong ra mắt dòng máy trợ thính SoundControl với giá chỉ 850 USD:

![](https://cdn.beekka.com/blogimg/asset/202105/bg2021053107.jpg)

Thiết bị cho phép người dùng tự kết nối với ứng dụng di động để tinh chỉnh các thông số lọc âm và khuếch đại phù hợp với tình trạng thính lực của mình thay vì phải đến phòng khám đo đạc phức tạp.

3、[Ý tưởng lắp đặt pin mặt trời trên các kênh dẫn nước tại California](https://theconversation.com/installing-solar-panels-over-californias-canals-could-yield-water-land-air-and-climate-payoffs-158754)

Trước tình trạng khô hạn kéo dài khiến lượng nước tại các hồ chứa sụt giảm nghiêm trọng, các chuyên gia năng lượng tại California đã đề xuất giải pháp lắp đặt các tấm pin mặt trời phủ kín các tuyến kênh dẫn nước tưới tiêu:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070901.jpg)

Giải pháp này mang lại lợi ích kép: vừa giúp sản xuất nguồn điện năng lượng tái tạo sạch tận dụng khoảng không gian trống trên kênh, vừa giúp che mát mặt nước giảm thiểu lượng nước bốc hơi do nắng nóng chiếu trực tiếp. Đồng thời, hơi nước mát từ kênh bốc lên cũng hỗ trợ làm hạ nhiệt độ tấm pin để tăng hiệu suất phát điện của pin mặt trời.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070902.jpg)

4、[Độ khó khai thác Bitcoin ghi nhận mức sụt giảm kỷ lục trong lịch sử](https://crypto.writer.io/p/the-biggest-downward-bitcoin-difficulty)

Đợt điều chỉnh độ khó khai thác (mining difficulty) mới nhất của mạng lưới Bitcoin đã ghi nhận mức giảm kỷ lục lên tới 27,94%. Sau ba chu kỳ điều chỉnh giảm liên tiếp, độ khó khai thác hiện đã giảm tới 42,6% so với mức đỉnh điểm vào tháng 5.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071410.jpg)

Quy trình tự động điều chỉnh độ khó sau mỗi 2.016 block được thiết kế để giữ thời gian khai thác trung bình của mỗi block luôn ở mức 10 phút. Đợt sụt giảm độ khó kỷ lục này là hệ quả trực tiếp từ việc chính phủ Trung Quốc siết chặt quản lý khiến hàng loạt mỏ đào coin lớn tại đây dừng hoạt động, làm tổng năng lực băm (hashrate) của mạng lưới sụt giảm mạnh.

5、[Volkswagen công bố giá thuê xe tự hành taxi trong tương lai](https://arstechnica.com/cars/2021/06/volkswagen-plans-to-offer-subscriptions-for-autonomous-driving-extra-ev-range/)

Hãng xe Volkswagen (Đức) công bố kế hoạch cung cấp dịch vụ gọi xe tự hành taxi trong tương lai với mức phí thuê chỉ khoảng 8,5 USD (tương đương 55 NDT) mỗi giờ sử dụng. Mức phí này rẻ hơn đáng kể so với cước phí taxi truyền thống có tài xế hiện nay.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061102.jpg)

6、[Trung tâm dữ liệu tiêu thụ lượng điện khổng lồ đe dọa lưới điện Ireland](https://www.theregister.com/2021/06/11/ireland_data_cnetre_electricity/)

Tổng công ty điện lực Ireland phát đi cảnh báo về nguy cơ xảy ra mất điện diện rộng do nhu cầu tiêu thụ điện năng tăng vọt của các trung tâm dữ liệu. Do các chính sách ưu đãi thuế, Ireland là nơi tập trung các máy chủ khổng lồ của các ông lớn công nghệ Mỹ như Google, Meta, Microsoft và Amazon.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061402.jpg)

Ước tính đến năm 2030, lượng điện năng tiêu thụ để làm mát và vận hành các trung tâm dữ liệu này sẽ chiếm tới 25% đến 33% tổng sản lượng điện của toàn quốc, gây áp lực khủng khiếp lên hệ thống truyền tải điện của quốc gia này.

7、[Microsoft ra mắt dịch vụ thuê máy tính ảo Windows 365](https://www.microsoft.com/en-us/windows-365)

Microsoft công bố dịch vụ đám mây mới mang tên Windows 365, cho phép người dùng thuê và chạy trực tiếp hệ điều hành Windows 10 hoặc Windows 11 ngay trên trình duyệt web của bất kỳ thiết bị nào (kể cả macOS, Android hay iOS).

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071505.jpg)

Toàn bộ dữ liệu cấu hình và trạng thái ứng dụng của người dùng được lưu trữ đồng bộ trên đám mây Azure, giúp bạn có thể tiếp tục công việc đang làm dở tại văn phòng ngay trên điện thoại hoặc máy tính cá nhân ở nhà mà không bị gián đoạn.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071506.jpg)

## 文章

1、[Thí nghiệm ghép tử cung cho chuột đực mang thai sinh con](https://mp.weixin.qq.com/s/WFjUA6d8-IxDRF2kPUlq0Q)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070103.jpg)

Bài viết phân tích các khía cạnh kỹ thuật và tranh cãi đạo đức y học xung quanh thí nghiệm của các nhà khoa học Trung Quốc khi tiến hành ghép tử cung thành công cho chuột đực và phối hợp liên kết tuần hoàn máu với chuột cái mang thai để giúp chuột đực sinh sản ra 10 chú chuột con khỏe mạnh.

2、[Tại sao chú sói AI trong game lại chọn cách tự tử?](https://mp.weixin.qq.com/s/kpqakpeKru7dpkE0f8pySA)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070702.jpg)

Một câu chuyện thú vị về lập trình thuật toán học sâu cho game "sói đuổi cừu": Tác giả thiết lập quy tắc cộng 10 điểm nếu sói bắt được cừu, trừ 1 điểm nếu đâm vào đá và trừ 0,1 điểm cho mỗi giây trôi qua để khuyến khích sói bắt cừu nhanh. Kết quả là chú sói AI sau khi tính toán đã chọn cách đâm đầu vào đá tự tử ngay khi vào game do thuật toán phạt điểm theo thời gian quá nặng khiến việc tự tử để kết thúc game sớm là phương án đạt tối ưu điểm số nhất.

3、[Tìm hiểu chi tiết về Pixel và mật độ điểm ảnh](https://blog.infolink.com.tw/2021/rediscover-pixel-dpi-ppi-and-pixel-density/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071421.jpg)

Bài phân tích chi tiết giúp lập trình viên phân biệt rõ nét các khái niệm kỹ thuật màn hình như Pixel vật lý, CSS Pixel, DPI, PPI, DPR và cách tính mật độ điểm ảnh để tối ưu hóa hiển thị giao diện web. (Đóng góp của [@Leon0824](https://github.com/ruanyf/weekly/issues/1841))

4、[Nhìn lại chặng đường 20 năm phát triển của giao thức BitTorrent](https://torrentfreak.com/bittorrent-turns-20-the-file-sharing-revolution-revisited-210702/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070401.jpg)

Giao thức chia sẻ tệp tin ngang hàng (P2P) BitTorrent được giới thiệu lần đầu tiên vào ngày 2 tháng 7 năm 2001. Bài viết nhìn lại chặng đường 20 năm phát triển đầy thăng trầm của giao thức này và những đóng góp của nó đối với kiến trúc truyền tải dữ liệu internet hiện đại.

5、[Kỹ thuật bẫy hacker tấn công để lộ địa chỉ IP thật](https://blog.0x3a.com/post/141950176719/playing-games-with-an-attacker-how-i-messed-with)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070402.jpg)

Tác giả chia sẻ kinh nghiệm xử lý khi trang web bị hacker liên tục quét lỗi bảo mật thông qua mạng ẩn danh Tor. Anh đã thiết lập một trang admin giả (honeypot) và cố tình để lộ liên kết trang này trong file báo lỗi. Khi hacker truy cập trang admin giả, script đặc biệt sẽ dụ trình duyệt của hacker gửi yêu cầu lấy file trực tiếp không qua proxy để ghi lại địa chỉ IP thật của đối tượng.

6、[Tại sao Tesla không sử dụng cảm biến LiDAR cho xe tự lái?](https://venturebeat.com/2021/07/03/tesla-ai-chief-explains-why-self-driving-cars-dont-need-lidar/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070501.jpg)

Giám đốc bộ phận trí tuệ nhân tạo của Tesla giải thích lý do hãng kiên quyết loại bỏ cảm biến LiDAR đắt đỏ trên các dòng xe tự lái của mình để chuyển dịch hoàn toàn sang sử dụng hệ thống camera thị giác máy tính kết hợp thuật toán học sâu để dựng mô hình không gian 3D.

7、[Hướng dẫn thiết kế UI/UX tối ưu cho biểu mẫu đăng nhập](https://learnui.design/blog/tips-signup-login-ux.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062804.jpg)

Tổng hợp 11 quy tắc vàng và mẹo nhỏ trong thiết kế giao diện giúp xây dựng các biểu mẫu đăng ký, đăng nhập tài khoản trực quan, mượt mà và giảm thiểu tỷ lệ thoát trang của người dùng.

8、[Các phương pháp đo thời gian thực thi của chương trình](https://serhack.me/articles/measure-execution-time-program/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070601.jpg)

Bài hướng dẫn giải thích các phương pháp đo đạc thời gian chạy thực tế của các hàm hoặc câu lệnh bằng ngôn ngữ C thông qua việc đo chu kỳ xung nhịp CPU hoặc đo thời gian hệ thống mili-giây.

## 工具

1、[Git: An Interactive History](https://git-history.jpalmer.dev/)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070109.jpg)

Một dự án trực quan hóa lịch sử các commit của kho mã nguồn Git dưới dạng sơ đồ tương tác 3D sinh động, giúp theo dõi luồng phát triển trực quan.

2、[phpsandbox.io](https://phpsandbox.io/)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061503.jpg)

Môi trường phát triển và thử nghiệm ngôn ngữ PHP trực tuyến chạy ngay trên trình duyệt web không cần cấu hình local server phức tạp.

3、[Utopia](https://utopia.app/)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061605.jpg)

Công cụ hỗ trợ thiết kế giao diện ứng dụng trực quan và tự động sinh ra mã nguồn React tương ứng thời gian thực.

4、[markdown-css-smartisan](https://github.com/nihaojob/markdown-css-smartisan)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071419.jpg)

Bộ theme CSS phong cách tối giản của ứng dụng ghi chép Smartisan Notes dành cho các trang web hiển thị tài liệu Markdown. (Đóng góp của [@nihaojob](https://github.com/ruanyf/weekly/issues/1839))

5、[Kindle2Flomo](https://github.com/Tit1e/kindle2Flomo)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071418.jpg)

Tiện ích hỗ trợ xuất nhanh các dòng ghi chú, highlight từ máy đọc sách Kindle trực tiếp sang phần mềm ghi chép cá nhân Flomo. (Đóng góp của [@chempeng](https://github.com/ruanyf/weekly/issues/1842))

6、[popular-message](https://github.com/nihaojob/popular-message)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071416.jpg)

Thư viện JavaScript siêu nhẹ không phụ thuộc hỗ trợ hiển thị các hộp thoại thông báo prompt đẹp mắt trên trang web. (Đóng góp của [@nihaojob](https://github.com/ruanyf/weekly/issues/1838))

7、[EFTP](https://github.com/newham/eftp)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071508.jpg)

Phần mềm SFTP client mã nguồn mở chạy trên hệ điều hành macOS hỗ trợ quản trị và truyền tải tệp tin trên máy chủ FTP nhanh chóng. (Đóng góp của [@newham](https://github.com/ruanyf/weekly/issues/1843))

8、[check-if-email-exists](https://github.com/reacherhq/check-if-email-exists)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070305.jpg)

Thư viện viết bằng Rust hỗ trợ kiểm tra chi tiết tính hợp lệ của địa chỉ email (kiểm tra hộp thư tồn tại thực tế, định dạng email dùng một lần, kiểm tra rò rỉ dữ liệu).

9、[Acid Tabs](https://github.com/jdhayford/acid-tabs-extension)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070502.jpg)

Extension trình duyệt Chrome hỗ trợ tự động gom nhóm và gập gọn các tab đang mở theo các bộ quy tắc tự định nghĩa để tiết kiệm không gian hiển thị.

## Tài nguyên

1、[Packet Traveling (Hành trình gói tin)](https://www.practicalnetworking.net/series/packet-traveling/packet-traveling/)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021062811.jpg)

Bộ bài viết trực quan giải thích chi tiết hành trình di chuyển của các gói tin dữ liệu trên mạng Internet từ cấu trúc gói tin cho đến nguyên lý hoạt động của các bộ định tuyến router.

2、[NASA Space Tourism Posters](https://www.jpl.nasa.gov/galleries/visions-of-the-future)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070102.jpg)

Phòng thí nghiệm JPL của NASA phát hành bộ 14 tác phẩm tranh vẽ cổ động du lịch không gian mang phong cách khoa học viễn tưởng cổ điển cho phép tải về in ấn miễn phí.

3、[Bảng giá thị trường của các nguyên tố hóa học](https://en.wikipedia.org/wiki/Prices_of_chemical_elements)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070108.jpg)

Trang Wikipedia tổng hợp bảng giá thị trường của các nguyên tố hóa học, chỉ ra nguyên tố rẻ nhất là Clo và nguyên tố đắt nhất là Poloni (gần 50 nghìn tỷ USD mỗi kg).

4、[Thị phần sản lượng vi xử lý CPU Intel và AMD](https://www.cpubenchmark.net/market_share.html)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021061901.jpg)

Trang web thống kê biểu đồ thị phần sử dụng CPU giữa hai gã khổng lồ Intel (đường màu xanh) và AMD (đường màu đỏ) từ năm 2004 đến nay.

## 图片

1、[Chuột chũi trần: Loài động vật nắm giữ bí quyết trường thọ](https://www.wired.com/story/long-strange-life-worlds-oldest-naked-mole-rat/)

Naked mole-rat (chuột chũi trần) là loài động vật gặm nhấm đặc hữu sống dưới lòng đất tại châu Phi với ngoại hình nhăn nheo không lông kỳ dị:

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060412.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060413.jpg)

Tuy nhiên, loài chuột này lại sở hữu tuổi thọ lên tới hơn 30 năm (gấp 30 lần chuột thông thường) và hầu như không bao giờ mắc bệnh ung thư. Bí quyết nằm ở tốc độ chuyển hóa năng lượng và nhịp thở của chúng cực kỳ thấp, giúp giảm thiểu tối đa sự lão hóa tế bào. Các nhà khoa học đang nghiên cứu cấu trúc mã gen tương đồng 93% giữa chuột chũi trần và người để ứng dụng các liệu pháp kéo dài tuổi thọ cho con người.

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060414.jpg)

2、[Bastle house: Kiểu nhà pháo đài thời Trung Cổ](https://en.wikipedia.org/wiki/Bastle_house)

Vào thời trung cổ tại vùng biên giới Anh - Scotland thường xuyên có cướp bóc hoành hành, người dân đã xây dựng các ngôi nhà bastle house kiên cố với bức tường đá dày tới 1 mét, các cửa sổ nhỏ trên cao và hoàn toàn không có cửa ra vào ở tầng trệt để chống cướp (muốn vào nhà phải leo thang lên tầng 2):

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060409.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060410.jpg)

![](https://cdn.beekka.com/blogimg/asset/202106/bg2021060411.jpg)

## Bài đọc thêm

### Định nghĩa về lỗ sâu vũ trụ (Wormhole)

*Trích sách "追逐类星体" giải thích trực quan về khái niệm Wormhole:*

Để giải thích lỗ sâu, trước hết phải nói về Hố Đen (Black Hole) - vùng không gian có lực hấp dẫn cực lớn hút mọi vật chất và ánh sáng đi qua vào trong.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071514.jpg)

Ngược lại với Hố Đen là khái niệm Hố Trắng (White Hole) - vùng không gian liên tục phun trào vật chất từ trong ra ngoài.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071515.jpg)

Giả thuyết đặt ra là nếu kết nối đáy của một Hố Đen với một Hố Trắng, vật chất bị hút vào Hố Đen sẽ được dẫn truyền qua một đường ống trung gian để phun ra ngoài ở Hố Trắng. Đường ống kết nối này chính là "Lỗ Sâu" (Wormhole). Lỗ Sâu đóng vai trò như một đường hầm không chứa vật chất ổn định kết nối các vùng không gian hoặc các vũ trụ song song khác nhau trong đa vũ trụ.

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071516.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071517.jpg)

## 言论

1、

Rất nhiều lập trình viên đòi hỏi các phần mềm phải hỗ trợ tính năng tương thích ngược tuyệt đối (backward compatibility), nhưng họ không nhận ra rằng điều đó đồng nghĩa với việc nhà phát triển buộc phải cam kết giữ nguyên các lỗi thiết kế của phiên bản cũ mãi mãi trong mã nguồn mới.

-- Trích bài viết về phát triển phần mềm

2、

Thay vì mất thời gian viết các dòng comment giải thích rườm rà (như Javadoc), việc đặt tên biến và tên hàm rõ nghĩa thể hiện chính xác mục đích logic của đoạn code (self-documenting code) sẽ mang lại hiệu quả đọc hiểu code tốt hơn nhiều cho đội ngũ làm việc chung.

-- Trích bài viết "On Comments in Code"

3、

Để bảo vệ các cửa hàng sách truyền thống nhỏ trước sự cạnh tranh của các sàn thương mại điện tử lớn, chính phủ Đức vào năm 2002 đã ban hành luật buộc toàn bộ hiệu sách (kể cả online) phải bán sách mới với giá niêm yết đồng nhất, tuyệt đối không được phép chiết khấu giảm giá.

-- Trích bài viết giải pháp bảo vệ hiệu sách tại Đức

## 历史上的本周

- 2020年（第 116 期）：[Phân tích xu hướng biến động và các bất ổn địa chính trị thế giới](https://www.ruanyifeng.com/blog/2020/07/weekly-issue-116.html)
- 2019年（第 64 期）：[Lời khuyên nhập môn cho người trẻ muốn bước chân vào ngành Internet](https://www.ruanyifeng.com/blog/2019/07/weekly-issue-64.html)
- 2018年（第 13 期）：[Tại sao bản tin tuần này chỉ thảo luận các chủ đề công nghệ?](https://www.ruanyifeng.com/blog/2018/07/weekly-issue-13.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
