# 科技爱好者周刊（第 173 期）：网络收音机的设计

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1870) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082619.jpg)

Tại nhiều khu dân cư cũ ở Thượng Hải, do yếu tố lịch sử để lại, hệ thống dây cáp điện và dây viễn thông trên không chằng chịt gây mất mỹ quan đô thị nghiêm trọng. Trong dự án cải tạo cảnh quan đường Giang Âm năm nay, đơn vị thi công đã thử nghiệm quấn các sợi dây điện này bên trong các dải dây leo lá xanh nhân tạo độc đáo để làm dịu không gian sống. (Nguồn: [Eastday](http://n.eastday.com/palbum/1629955396017452))

## 主带话题：Triết lý thiết kế đài Radio Internet tối giản cho người cao tuổi

Gần đây, tôi có tìm mua một chiếc đài radio Internet (máy nghe nhạc/tin tức qua mạng) để tặng cho người lớn tuổi trong nhà.

Người lớn tuổi (đã ngoài 85 tuổi) hoàn toàn không biết gì về Internet hay công nghệ số. Việc sử dụng smartphone quá phức tạp với họ, họ thường bấm nhầm các nút hiển thị trên màn hình cảm ứng rồi không biết làm cách nào để khôi phục lại trạng thái cũ. Trò tiêu khiển duy nhất hàng ngày là bật TV xem phim truyền hình (thực chất là bật lên cho có âm thanh trong nhà chứ không thực sự chú ý). Những người già như vậy thuộc nhóm chịu nhiều thiệt thòi nhất trong kỷ nguyên số hóa này, nhưng quy mô tệp người dùng này thực tế không hề nhỏ (có thể lên tới hàng chục triệu người ở các nước).

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082413.jpg)

Tôi muốn tìm kiếm một chiếc đài radio kết nối mạng để giúp họ nghe được các kênh tin tức, kể chuyện, phong phú thêm cuộc sống tuổi già mà không gặp bất kỳ rào cản kỹ thuật nào. Yêu cầu của tôi rất đơn giản: Thao tác sử dụng càng tối giản càng tốt, người già không biết Internet vẫn dùng được dễ dàng.

Hãy thử đặt mình vào vị trí của nhà thiết kế sản phẩm: Bạn sẽ thiết kế chiếc đài này ra sao? Liệu một chiếc đài trang bị màn hình cảm ứng toàn phần hiển thị hàng loạt danh mục ứng dụng có phù hợp cho người cao tuổi không?

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082414.jpg)

Thực tế tôi đã tìm được một sản phẩm đáp ứng hoàn hảo yêu cầu này trên trang thương mại điện tử và lập tức đặt mua. Trải nghiệm thực tế của thiết bị này còn tuyệt vời hơn mong đợi của tôi rất nhiều.

Dưới đây không phải là bài viết quảng cáo cho sản phẩm, tôi chỉ mượn thiết kế của chiếc đài này để bàn luận về tư duy thiết kế phần cứng dành cho nhóm khách hàng lớn tuổi:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082415.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082416.jpg)

Nhà thiết kế chiếc đài này thực sự đã bỏ rất nhiều tâm huyết nghiên cứu hành vi người dùng, dũng cảm loại bỏ toàn bộ các tính năng rườm rà không cần thiết của một thiết bị Internet thông thường để tối giản hóa tối đa cấu hình thiết bị.

Tôi đánh giá rất cao 3 điểm đột phá trong thiết kế của máy:

1. **Tích hợp sẵn kho nội dung trực tiếp:** Máy tự động kết nối trực tiếp vào thư viện nội dung của nền tảng Ximalaya (một kho audiobook/podcast lớn). Thiết bị không yêu cầu đăng nhập, xác thực tài khoản hay tìm kiếm cấu hình URL phức tạp. Người dùng chỉ cần bật nút là nội dung tự động phát. Người già hoàn toàn không cần nhận biết sự hiện diện của khái niệm ứng dụng hay Internet.

   *Hãy thử đặt câu hỏi: Nếu để chuyển đổi chương trình, người già phải thao tác gõ nhập địa chỉ URL hoặc chọn luồng dữ liệu, họ có thể tự làm được không?*

2. **Sử dụng núm xoay cơ học thay cho nút bấm cảm ứng:** Núm xoay điều chỉnh âm lượng vật lý to, rõ ràng và có độ nảy tốt là thiết kế trực quan tuyệt vời. Núm xoay cơ học có thể dễ hỏng hơn nút cảm ứng, nhưng nó mang lại cảm nhận xúc giác (tactile feedback) quen thuộc nhất cho người già.

   ![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082417.jpg)

   Khi tôi chia sẻ hình ảnh thiết bị lên Twitter, một bạn lập trình viên đã bình luận rất hay: *"Mặc dù xu hướng công nghệ hiện nay là phần mềm hóa phần cứng (sử dụng màn hình cảm ứng để thay thế các nút bấm vật lý), nhưng đối với nhóm khách hàng lớn tuổi, triết lý ngược lại: phần cứng hóa tính năng phần mềm mới là hướng đi đúng đắn. Việc biến các cài đặt cấu hình số thành các công tắc gạt, núm xoay vật lý 'gạt là bật, xoay là tắt' mang lại sự thân thiện tối đa cho người già."*

3. **Không hỗ trợ kết nối Wi-Fi, chỉ dùng mạng di động 4G qua SIM tích hợp:** Nhiều người coi việc thiếu Wi-Fi là điểm trừ lớn, nhưng tôi lại cho rằng đây là ưu điểm đắt giá nhất của thiết bị.

   Mặc dù nó làm phát sinh chi phí duy trì nạp thẻ data 4G hàng năm (con cháu có thể nạp giúp qua app điện thoại), nhưng nó giải quyết triệt để vấn đề thiết lập Wi-Fi. Việc chọn mạng Wi-Fi, nhập mật mã trên một màn hình nhỏ là tác vụ bất khả thi với người già 80 tuổi. Sử dụng sóng di động 4G giúp chiếc đài hoạt động mượt mà ở mọi nơi, bật lên là nghe được nhạc ngay lập tức tương tự như sóng radio AM/FM truyền thống trước đây.

Tuy nhiên sản phẩm vẫn có thể cải thiện tốt hơn nếu thay thế toàn bộ nhãn chữ tiếng Anh trên các nút bấm vật lý bằng tiếng bản địa trực quan hơn.

Kiệt tác phần cứng tối giản này là minh chứng rõ nét cho triết lý thiết kế kinh điển: **Dũng cảm từ bỏ các tính năng phụ để đổi lấy sự đơn giản tuyệt đối của sản phẩm, trực tiếp nâng cao trải nghiệm người dùng cuối.** Đó chính là tinh thần cốt lõi của nguyên lý *"Less is more"* và *"Worse is better"* trong thiết kế hệ thống.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082618.jpg)

## Khóa học kiến trúc và đồng nhất phong cách lập trình Vue vs React

Hiện tại, hầu hết lập trình viên Front-end mới thường chỉ tập trung học sâu một trong hai thư viện phổ biến là Vue hoặc React.

Tuy nhiên, trong các dự án thực tế tại các doanh nghiệp lớn, việc làm việc song song hoặc chuyển đổi mã nguồn giữa hai framework này diễn ra rất phổ biến tùy thuộc vào kiến trúc của từng team dự án.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082608.jpg)

Nếu bạn chỉ thành thạo Vue nhưng dự án mới yêu cầu viết React, hoặc bạn đang viết một thư viện mã nguồn mở dùng chung cần hỗ trợ cả hai framework, việc tìm ra một kiến trúc thiết kế dùng chung (universal architecture) để tối đa hóa khả năng tái sử dụng logic là cực kỳ quan trọng.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082611.jpg)

Khóa học chuyên đề **《Vue and React Architecture & Style Unification》** sẽ giải đáp chi tiết các khía cạnh kỹ thuật này giúp bạn mở rộng tư duy lập trình:

- Làm thế nào để nhanh chóng tiếp cận và làm chủ React khi chỉ biết Vue (và ngược lại)?
- Thiết kế cấu trúc mã nguồn thế nào để tái sử dụng logic tối đa giữa React và Vue?
- Các tập đoàn công nghệ lớn thống nhất quy chuẩn chất lượng sản phẩm thế nào khi sử dụng cả hai framework?

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082610.jpg)

Khóa học được chia sẻ bởi cựu kiến trúc sư Full-stack Alibaba P8 giàu kinh nghiệm phát triển các dự án có quy mô hàng trăm triệu người dùng.

Học viên tham gia khóa học sẽ được tặng kèm hai khóa học bổ trợ: *《Lập trình Dart chuyên sâu cho Flutter》* và *《Phân tích xu hướng thu nhập của lập trình viên Front-end chất lượng cao》* để chuẩn bị cho các đợt tuyển dụng tiếp theo:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082612.jpg)

Độc giả bản tin có thể đăng ký tham gia khóa học hoàn toàn **miễn phí (0đ)** bằng cách quét mã QR trên đây.

## 科技动态

1、[Thử nghiệm trạm phát điện mặt trời trên không](https://mp.weixin.qq.com/s/euKVL7gllNQO0IaTMzSJJg)

Hạ tầng pin mặt trời đặt dưới mặt đất thường xuyên bị ảnh hưởng công suất bởi các đám mây, sương mù, mưa tuyết làm giảm thời gian chiếu sáng và cường độ bức xạ. Các nhà khoa học từ lâu đã mơ ước đưa pin mặt trời lên tầng không trung để đón ánh nắng trực tiếp liên tục.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080907.jpg)

Vào tháng 6/2021, Đại học Trùng Khánh phối hợp cùng các viện nghiên cứu bắt đầu xây dựng trạm thử nghiệm điện mặt trời không gian đầu tiên. Dự án đưa các tấm pin mặt trời lên độ cao từ 50 đến 300 mét bằng một khinh khí cầu cố định làm bệ đỡ. Nếu thành công, bước tiếp theo sẽ đưa hệ thống lên tầng bình lưu ở độ cao 22 km.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080908.jpg)

Hệ thống bệ đỡ bay tích hợp các thấu kính hội tụ ánh sáng mặt trời vào vùng pin quang điện để sản sinh dòng điện một chiều, sau đó chuyển đổi năng lượng này thành sóng vi ba (microwaves) truyền không dây thẳng về trạm thu dưới mặt đất.

2、[Facebook ra mắt phần mềm họp ảo VR Horizon Workrooms](https://www.axios.com/facebook-vr-zuckerberg-meetings-7b8b78fb-5345-42a6-a338-2abe19079c9d.html)

Tập đoàn Facebook chính thức giới thiệu phần mềm phòng họp ảo Horizon Workrooms nhằm mang lại trải nghiệm làm việc từ xa chân thực chưa từng có.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082101.jpg)

Khi đeo kính thực tế ảo VR Oculus Quest 2 và khởi chạy ứng dụng, bạn sẽ bước vào một phòng họp 3D sống động. AI sẽ tự động đồng bộ cử chỉ khuôn mặt, nụ cười và ánh mắt của bạn lên nhân vật ảo (avatar). Đồng thời hệ thống camera của kính sẽ quét chuyển động của đôi bàn tay ngoài đời thực để hiển thị chính xác lên nhân vật ảo tương ứng.

Ví dụ, khi bạn đang gõ phím máy tính ngoài đời thực, nhân vật ảo của bạn trong phòng họp cũng hiển thị hành vi gõ phím tương ứng:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082102.jpg)

Các thành viên có thể cùng nhau phác thảo ý tưởng trên bảng trắng ảo, chia sẻ tài liệu và màn hình máy tính cá nhân. Facebook đã công bố đoạn video demo buổi họp ảo của CEO Mark Zuckerberg trình diễn mượt mà các tính năng này:

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=f3269m4u87c" allowFullScreen="true" width="600" height="400"></iframe>

3、[Trung Quốc thí điểm triển khai Giấy phép lái xe điện tử](http://china.qianlong.com/2021/0820/6179805.shtml)

Kể từ ngày 1/9, Bộ Công an Trung Quốc bắt đầu cho phép thí điểm cấp Giấy phép lái xe điện tử (Digital Driver's License) tại 28 thành phố trên cả nước với hiệu lực pháp lý tương đương bản giấy truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082303.jpg)

Người dân chỉ cần tải thông tin bằng lái về điện thoại thông minh qua ứng dụng hành chính công để xuất trình khi cảnh sát kiểm tra trên đường. Mã QR Code tích hợp trên giấy phép điện tử giúp cảnh sát quét nhanh để đối chiếu thông tin đăng ký xe và căn cước công dân.

4、[Rút ngắn một nửa chu kỳ sinh trưởng của cây lúa trong nhà](http://news.sciencenet.cn/htmlnews/2021/8/463517.shtm)

Viện Khoa học Nông nghiệp Trung Quốc công bố thử nghiệm thành công phương án trồng lúa nước trong phòng kín (vertical farming) giúp rút ngắn chu kỳ sinh trưởng của lúa xuống một nửa, chỉ mất khoảng 60 ngày để thu hoạch thay vì hơn 120 ngày ngoài đồng ruộng. Điều này giúp tăng tần suất thu hoạch lên 6 vụ mỗi năm.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082411.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082412.jpg)

Hệ thống sử dụng đèn LED được tinh chỉnh quang phổ ánh sáng chuyên dụng thay thế ánh nắng mặt trời và nuôi dưỡng cây bằng các dung dịch dinh dưỡng hữu cơ lỏng trong môi trường được kiểm soát chặt chẽ về nhiệt độ, độ ẩm và nồng độ khí CO2. Tuy nhiên, chi phí vận hành hệ thống điện chiếu sáng vẫn là rào cản lớn để thương mại hóa rộng rãi.

5、[Facebook đề xuất thiết kế kính VR hiển thị đôi mắt của người đeo](https://www.sohu.com/a/481676198_255990)

Một nhược điểm lớn khi đeo các thiết bị kính VR cồng kềnh là che khuất hoàn toàn khuôn mặt của người đeo, gây khó khăn cho việc giao tiếp trực tiếp với người xung quanh. Các kỹ sư Facebook đã phát triển giải pháp trang bị thêm một màn hình LCD nhỏ phía ngoài kính hiển thị đôi mắt ảo mô phỏng ánh nhìn thực tế của người đeo:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080905.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080906.jpg)

Hệ thống camera quét mắt phía trong kính sẽ thu lại hướng nhìn và chuyển động nháy mắt của người đeo để hiển thị thời gian thực lên màn hình ngoài giúp cuộc hội thoại trở nên tự nhiên hơn.

6、[Thương mại hóa súng điện từ cầm tay đầu tiên trên thế giới](https://www.thefirearmblog.com/blog/2021/08/05/arcflash-labs-gr-1-anvil/)

Hãng Arcflash Labs tại Mỹ công bố mở cổng đặt hàng mẫu súng điện từ dạng cuộn dây cầm tay (coilgun) thương mại đầu tiên mang tên GR-1 Anvil:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080705.jpg)

Khác với súng đạn thông thường sử dụng thuốc súng đốt cháy sinh áp lực khí đẩy đạn, súng điện từ sử dụng pin năng lượng tích điện vào các cuộn dây đồng để tạo ra lực từ trường cực mạnh hút và tăng tốc viên đạn sắt nhỏ bay đi với vận tốc cực lớn. Thiết bị được bán với mức giá đặt trước là 3.375 USD (chưa bao gồm bộ sạc pin chuyên dụng).

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080706.jpg)

7、[Vấn đề tranh chấp bản quyền sở hữu trí tuệ của hệ thống mã Captcha](https://www.eff.org/deeplinks/2021/08/captcha-patent-all-american-nightmare)

Một công ty công nghệ nhỏ tại Mỹ vừa đệ đơn kiện tuyên bố hệ thống xác thực hình ảnh reCAPTCHA của Google đang xâm phạm bằng sáng chế của hãng và yêu cầu toàn bộ các website đang sử dụng dịch vụ này phải đóng phí bản quyền:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080711.jpg)

Đại diện công ty cho biết họ đã được cấp bằng sáng chế cho ý tưởng *"sử dụng hình ảnh trực quan để phân biệt người dùng thực tế và bot lập trình tự động"* từ năm 2008:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080712.jpg)

Vụ kiện làm dấy lên những tranh luận nảy lửa trong giới luật pháp công nghệ: Liệu một ý tưởng logic trừu tượng thông thường có nên được cấp bằng sáng chế để ngăn cản các đơn vị khác tự lập trình phát triển các giải pháp tương tự hay không.

## 文章

1、[Tại sao chip quản lý nguồn điện (PMIC) lại rất khó chế tạo?](https://finance.sina.com.cn/chanjing/cyxw/2021-07-29/doc-ikqciyzk8373189.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080910.jpg)

Với sự phức tạp của các tiêu chuẩn sạc nhanh thiết bị hiện nay, mọi bảng mạch điện tử đều cần chíp quản lý nguồn (PMIC) để điều phối dòng điện an toàn. Bài viết phân tích rào cản kỹ thuật của PMIC và thực trạng thị trường hiện tại vẫn bị thâu tóm bởi một vài tập đoàn bán dẫn lớn của nước ngoài.

2、[Đánh giá về hệ thống tên miền độc lập ".chn" tại Trung Quốc](https://www.zhihu.com/question/324843186)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081707.jpg)

Chuyên mục thảo luận trên Zhihu phân tích dự án ra mắt đuôi tên miền ".chn" tự phát của một doanh nghiệp trong nước nhằm thoát ly sự phụ thuộc vào tổ chức quản lý tên miền quốc tế ICANN. Tuy nhiên do không được ICANN hay CNNIC thừa nhận nên trình duyệt thông thường không thể truy cập các website này nếu người dùng không tự cấu hình tệp tin hosts trên máy tính.

3、[Thông báo lỗi kỳ lạ của lệnh man trên Linux](https://unix.stackexchange.com/questions/405783/why-does-man-print-gimme-gimme-gimme-at-0030)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021073002.jpg)

Một lập trình viên phát hiện chi tiết thú vị: Khi chạy lệnh tra cứu hướng dẫn `man` trên hệ điều hành Linux đúng vào thời điểm nửa đêm 00:30, hệ thống thỉnh thoảng trả về dòng thông báo lỗi kỳ lạ *"gimme gimme gimme"*. Cộng đồng đã tìm ra đây là một easter egg hài hước do lập trình viên viết mã nguồn lệnh lồng vào dựa theo tên ca khúc nổi tiếng của ban nhạc ABBA.

4、[Hướng dẫn sử dụng CSS phát hiện thiết bị hỗ trợ sự kiện hover](https://css-irl.info/detecting-hover-capable-devices/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071607.jpg)

Các thiết bị di động dùng màn hình cảm ứng không sử dụng con trỏ chuột nên không có sự kiện hover. Tác giả hướng dẫn sử dụng thuộc tính CSS `@media (hover: hover)` để kiểm tra chính xác thiết bị của khách truy cập nhằm ẩn hiển các chi tiết giao diện cho phù hợp.

5、[Thực trạng phân mảnh xử lý thuộc tính SameSite cookie trên các trình duyệt](https://simonwillison.net/2021/Aug/3/samesite/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080704.jpg)

Các trình duyệt hiện đại đều áp dụng thuộc tính `SameSite` cho cookie để ngăn chặn tấn công giả mạo yêu cầu chéo trang CSRF. Tuy nhiên, bài viết chỉ ra cơ chế nhận diện và chặn cookie bên thứ ba của Chrome, Safari và Firefox có những khác biệt lớn gây khó khăn cho lập trình viên khi đồng bộ phiên làm việc.

6、[Ứng dụng thuộc tính download của thẻ liên kết HTML](https://shkspr.mobi/blog/2021/08/to-download-this-page-click-here/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080904.jpg)

Tác giả chia sẻ cách thức sử dụng thuộc tính `download` trên thẻ `<a>` giúp lập trình viên tạo nhanh tính năng cho phép khách click tải trực tiếp toàn bộ trang web hiện tại về máy tính dưới dạng file HTML lưu trữ.

7、[Hướng dẫn sử dụng test.todo() trong Jest](https://heyfirst.co/blog/how-to-use-test-todo-in-jest)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080903.jpg)

Bài viết hướng dẫn cách tận dụng phương thức `test.todo()` của thư viện kiểm thử Jest để ghi chú nhanh cấu trúc các ca kiểm thử cần viết bổ sung trong tương lai mà không làm gián đoạn luồng chạy test hiện tại.

8、[Hướng dẫn toàn tập về thuộc tính CSS transform](https://www.joshwcomeau.com/css/transforms/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081013.jpg)

Một bài hướng dẫn CSS rất chất lượng mô tả cách sử dụng thuộc tính `transform` để thiết kế các hiệu ứng xoay, thu phóng, nghiêng các phần tử giao diện web đi kèm nhiều hoạt ảnh minh họa trực quan tương tác.

## 工具

1、[RAWGraphs](https://rawgraphs.io/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081028.jpg)

Tiện ích trực tuyến hỗ trợ người dùng dán nhanh các bảng dữ liệu Excel/CSV để tự động sinh ra các biểu đồ trực quan hóa dữ liệu (data visualization) vô cùng đẹp mắt mà không cần viết code.

2、[Cross Context Events](https://github.com/mia1024/cross-context-events)

Thư viện JavaScript gọn nhẹ hỗ trợ đồng bộ hóa và phát các sự kiện (custom events) chạy song song giữa nhiều tab trình duyệt hoặc iframe đang mở của người dùng.

3、[obvious.js: Framework micro-frontend tối giản](https://github.com/ObviousJs/obvious-core)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082501.jpg)

Framework micro-frontend nguồn mở hỗ trợ quản lý vòng đời và truyền nhận dữ liệu dùng chung giữa ứng dụng React và Vue chạy trên cùng một giao diện trang web. (Đóng góp của [@run-nan](https://github.com/ruanyf/weekly/issues/1899))

4、[Web Captioner: Nhận diện giọng nói trên web](https://webcaptioner.com/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082503.jpg)

Ứng dụng web nhận diện giọng nói tiếng Trung trực tiếp thành văn bản chữ viết sử dụng API Web Speech tích hợp sẵn trong trình duyệt Chrome. Xem thêm [mã nguồn dự án](https://github.com/bensonruan/Chrome-Web-Speech-API). (Đóng góp của @jerrylususu)

5、[Maestral: Client Dropbox nguồn mở gọn nhẹ](https://github.com/SamSchott/maestral)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081206.jpg)

Ứng dụng khách Dropbox không chính thức tối ưu hóa riêng cho Linux và macOS với ưu điểm tiêu thụ cực ít tài nguyên bộ nhớ RAM.

6、[Padka: Hiệu ứng chuyển động cho Zoom Meetings](https://www.padka.com/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081211.jpg)

Phần mềm thiết kế hoạt ảnh độc đáo dành cho các lớp học trực tuyến qua Zoom. Hệ thống tự động nhận diện ngôn ngữ cơ thể và cao độ giọng nói của giáo viên để chèn thêm các hiệu ứng âm thanh và sticker hoạt hình tương ứng thời gian thực.

7、[Mantine UI Components](https://mantine.dev/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080409.jpg)

Thư viện components giao diện phong phú cho React được tối ưu hóa hiển thị chế độ tối (dark mode) và hỗ trợ khả năng tùy biến style chi tiết.

8、[react-class-to-fc](https://github.com/yklydxtt/react-class-to-fc)

Công cụ dòng lệnh CLI hỗ trợ tự động chuyển đổi cấu trúc mã nguồn các React Class Components cũ sang cấu trúc Function Components sử dụng React Hooks hiện đại. (Đóng góp của [@yklydxtt](https://github.com/ruanyf/weekly/issues/1907))

9、[FireCMS Content Management](https://firecms.co/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080202.jpg)

Hệ quản trị nội dung CMS xây dựng trên nền tảng Firebase hỗ trợ thiết lập nhanh chóng giao diện quản trị cơ sở dữ liệu cho các lập trình viên.

## Tài nguyên

1、[StackOverflow Developer Survey 2021](https://insights.stackoverflow.com/survey/2021)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080303.jpg)

Báo cáo kết quả cuộc khảo sát lập trình viên thường niên lớn nhất thế giới của StackOverflow với sự tham gia của hơn 80.000 lập trình viên phản ánh các xu hướng công nghệ nổi bật.

2、[thosefree.com: Kho tài nguyên thiết kế Front-end miễn phí](https://www.thosefree.com/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082502.jpg)

Trang web cá nhân tổng hợp giới thiệu hàng trăm liên kết tải tài nguyên phông chữ, biểu tượng, hình vẽ vector và các template CSS miễn phí chất lượng cao. (Đóng góp của [@weyman-git](https://github.com/ruanyf/weekly/issues/1900))

3、[Cộng đồng làm việc từ xa Điện Áp (eleduck.com)](https://eleduck.com/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082504.jpg)

Diễn đàn cộng đồng lớn tại Trung Quốc chuyên thảo luận và chia sẻ các cơ hội làm việc từ xa (remote work), dự án outsource phát triển phần mềm tự do. (Đóng góp của [@qrk12](https://github.com/ruanyf/weekly/issues/1902))

4、[MetaNumbers: Công cụ tra cứu thuộc tính số học](https://metanumbers.com/)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021073001.jpg)

Tiện ích tra cứu nhanh các thông tin toán học lý thuyết số đặc thù của một số nguyên dương bất kỳ (hỗ trợ các số có giá trị cực lớn).

5、[IoT for Beginners by Microsoft](https://github.com/microsoft/IoT-For-Beginners)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071513.jpg)

Khóa học 12 tuần nhập môn lập trình thiết bị Internet vạn vật (IoT) do đội ngũ kỹ sư Microsoft phát hành miễn phí trên GitHub.

## 图片

1、[Các tác phẩm hội họa vẽ tự động bởi AI CLIP](https://ml.berkeley.edu/blog/posts/clip-art/)

Mô hình AI tạo ảnh CLIP mới ra mắt của OpenAI sở hữu khả năng tự động phác họa các bức tranh phong cảnh nghệ thuật tuyệt đẹp dựa theo mô tả văn bản ngắn của người dùng:

- Bức tranh *"Đêm thành phố"*:
  ![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070309.jpg)

- Bức tranh *"Gió thổi"*:
  ![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070312.jpg)

- Bức tranh *"Ngôi nhà gỗ nhỏ trong bão tuyết đỉnh núi rực ánh đèn hoàng hôn"*:
  ![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070314.jpg)

- Bức tranh *"Nhà trong núi đêm muộn ngập tràn đom đóm (phong cách hoạt hình Ghibli Studio)"*:
  ![](https://cdn.beekka.com/blogimg/asset/202107/bg2021070315.jpg)

## Bài đọc thêm

### Triết lý thiết kế cơ học của門 tay nắm trong đời sống

*Trích cuốn sách tâm lý học thiết kế kinh điển "The Design of Everyday Things" phân tích về tay nắm cửa:*

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082613.jpg)

Nhiều đồ vật sử dụng hàng ngày quanh ta thực chất có thiết kế chưa tối ưu gây nhầm lẫn khi sử dụng, ví dụ như tay nắm cửa ở các tòa nhà công cộng khiến mọi người lúng túng không biết nên đẩy hay kéo cửa.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082614.jpg)

Giải pháp thô sơ nhất là dán nhãn chữ chỉ dẫn "Đẩy" hoặc "Kéo" lên cửa, tuy nhiên thiết kế này bắt buộc người dùng phải đọc hiểu chữ trước khi hành động và vô hiệu với người nước ngoài.

Tác giả đề xuất giải pháp thiết kế cơ học trực quan: Quy định tay nắm dạng thanh dọc chuyên dùng cho thao tác kéo, và tay nắm dạng tấm thanh ngang phẳng chuyên dùng cho thao tác đẩy:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082615.jpg)

Hoặc tối giản nhất, đối với các cánh cửa chỉ được phép đẩy, hãy loại bỏ hoàn toàn tay nắm vật lý ở mặt đó để người dùng tự hiểu họ chỉ có thể dùng tay đẩy phẳng vào cửa:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082616.jpg)

Tác giả hóm hỉnh chia sẻ thiết kế tốt nhất ông từng thử nghiệm ở nhà riêng là dùng một sợi dây thừng buộc làm tay nắm cửa, chỉ cần nhìn thấy sợi dây là người dùng tự khắc biết họ chỉ có thể dùng lực kéo cửa:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082617.jpg)

## 言论

1、

Một lập trình viên xuất sắc được định nghĩa bởi khả năng đưa ra giải pháp tối giản để giải quyết một bài toán phức tạp. Ngược lại, những lập trình viên nghiệp dư luôn đề xuất những cấu trúc code vô cùng phức tạp chỉ để giải quyết những bài toán đơn giản.

-- Thảo luận trên Hacker News

2、

Theo kinh nghiệm quản lý của tôi, hầu hết các lập trình viên mới thường mất khoảng 6 đến 8 tháng làm việc để hoàn toàn hòa nhập và phát huy 100% năng lực tại công ty mới. Sau khoảng 2 đến 3 năm cống hiến tại cùng một vị trí, phần lớn nhân sự bắt đầu xuất hiện dấu hiệu chững lại và giảm hứng thú công việc. Do đó, việc luân chuyển nhân sự hoặc thay đổi môi trường sau 2-3 năm là bình thường của thị trường lao động.

-- Thảo luận trên Hacker News

3、

Mã nguồn dự án của bạn viết ra nên mang chất lượng như một bức thư tình gửi tới người đồng nghiệp tiếp theo tiếp quản dự án.

-- AgriWebb

## 历史上的本周

- 2020年（第 122 期）：[Phân tích góc nhìn tài chính về định giá cao của các công ty Internet](https://www.ruanyifeng.com/blog/2020/08/weekly-issue-122.html)
- 2019年（第 70 期）：[Tìm hiểu bản chất kinh tế và ảnh hưởng của kỷ nguyên lãi suất âm toàn cầu](https://www.ruanyifeng.com/blog/2019/08/weekly-issue-70.html)
- 2018年（第 19 期）：[Góc nhìn về thế giới thực tế ảo OASIS trong bộ phim điện ảnh bom tấn Ready Player One](https://www.ruanyifeng.com/blog/2018/08/weekly-issue-19.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
