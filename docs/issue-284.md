# Bản tin chia sẻ công nghệ (Số 284): Có bao nhiêu video trên YouTube?

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3814) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122614.webp)

Một nhiếp ảnh gia người Ý sau 6 năm kiên trì thử thách cuối cùng đã chụp được một bức ảnh phi thường trong tháng này: Vương cung thánh đường, đỉnh núi và mặt trăng nằm trên một đường thẳng hoàn hảo, và nhờ kỹ thuật phơi sáng lâu, ánh sáng mặt trời phản chiếu từ Trái Đất đã làm sáng rõ phần đỉnh của mặt trăng. (Nguồn: [APOD NASA](https://apod.nasa.gov/apod/ap231225.html))

## YouTube 有多少个视频？

YouTube là trang web chia sẻ video lớn nhất thế giới, nơi mọi người từ khắp nơi trên thế giới liên tục tải video lên.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122405.webp)

Tuy nhiên, nền tảng này chưa bao giờ công bố chính thức tổng số lượng video được lưu trữ trong hệ thống của họ.

Tuần trước, trên mạng xuất hiện [một bài viết rất thú vị](https://ethanzuckerman.com/2023/12/22/how-big-is-youtube/) sử dụng phương pháp xác suất thống kê để ước tính tổng số lượng video trên YouTube.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122406.webp)

Bài viết này mang tính gợi mở rất cao, và kiểu câu hỏi dạng này cũng thường xuất hiện trong các buổi phỏng vấn tuyển dụng. Dưới đây tôi xin chia sẻ cách thức tác giả thực hiện.

Như chúng ta đã biết, mỗi video trên YouTube đều sở hữu một mã định danh (ID) duy nhất nằm trong đường link URL.

Ví dụ, nếu URL của một video là `https://www.youtube.com/watch?v=NJHG0yuBabQ`, thì mã ID của video đó chính là chuỗi `NJHG0yuBabQ`.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122407.webp)

YouTube chưa từng tiết lộ thuật toán tạo ra mã ID này.

Tuy nhiên, qua quan sát thực tế, chúng ta có thể biết mã ID này là một chuỗi ký tự gồm 11 ký tự. Trong đó, 10 ký tự đầu tiên được chọn ngẫu nhiên từ tập hợp 64 ký tự tiêu chuẩn (`[a-zA-Z0-9_-]`), và ký tự thứ 11 cuối cùng chỉ được chọn từ tập hợp gồm 16 ký tự giới hạn.

Điều này có nghĩa là tổng số mã ID có thể tạo ra lên tới 2^64 khả năng – một con số cực kỳ khổng lồ, đủ sức chứa toàn bộ các video được tạo ra trong cả quá khứ lẫn tương lai.

Rõ ràng, không phải mã ID nào được tạo ra cũng tương ứng với một video thực tế đang tồn tại, phần lớn trong số đó là các mã trống (không có video), và số mã trống này vượt trội hoàn toàn so với số video thực tế. Nếu giả định YouTube có khoảng 1 tỷ video thực tế, bạn sẽ phải đoán ngẫu nhiên khoảng 18,4 tỷ lần mới trúng được một mã ID hợp lệ (với điều kiện các mã ID được phân bổ ngẫu nhiên đồng đều).

Từ quy luật này, **chúng ta có thể tính toán ngược lại: Dựa trên tỷ lệ đoán trúng mã ID hợp lệ để ước lượng tổng số lượng video thực tế trên YouTube**.

Ví dụ trực quan: Giả sử số điện thoại của một khu vực nằm trong dải số từ 843-000-0000 đến 843-999-9999 (tổng cộng 10 triệu số). Chúng ta chọn gọi thử ngẫu nhiên 100 số điện thoại. Nếu có 10 cuộc gọi kết nối thành công (tỷ lệ kết nối 10%), chúng ta có thể ước tính khu vực này hiện có khoảng 1 triệu số thuê bao đang hoạt động, và 9 triệu số còn lại vẫn là số trống.

Tác giả bài viết đã áp dụng chính xác phương pháp này: Tự động tạo ngẫu nhiên các chuỗi ID video và gửi yêu cầu kiểm tra xem video đó có tồn tại thực tế hay không. Kết quả phân tích đưa ra kết luận: Tính đến cuối năm 2023, **ước tính tổng số video trên YouTube đạt khoảng 13,325 tỷ video**.

Không chỉ ước tính tổng số video, nhóm tác giả còn phân tích và công bố rất nhiều chỉ số thống kê thú vị khác trên trang web [tubestats.org](https://tubestats.org/) trên.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122408.webp)

Một số thống kê thú vị thu được từ dự án bao gồm:

> - Tính đến năm 2023 YouTube có 13,3 tỷ video, tăng mạnh từ mốc 9,3 tỷ của năm 2022, tốc độ tăng trưởng hàng năm đạt trên 40%.
> - Khoảng 4,5% số video trên nền tảng chưa từng được ai bấm xem một lần nào.
> - Khoảng 72% số video không nhận được bất kỳ lượt bình luận nào.
> - Khoảng 60% số lượng video thuộc thể loại Vlog (chia sẻ cuộc sống cá nhân).
> - Thời lượng video phổ biến nhất nằm trong khoảng từ 9 đến 16 phút, chiếm tỷ lệ 20% tổng số video.

Bạn đọc quan tâm đến các số liệu chi tiết khác về xu hướng video có thể truy cập trang web trên để tìm hiểu.

Cuối cùng, một số độc giả nhận xét rằng phương pháp ước tính này thực chất không hề mới. Giới sinh vật học từ lâu đã áp dụng phương pháp này để ước lượng tổng số lượng cá sinh sống trong một hồ nước.

Quy trình thực hiện: Bạn câu được 100 con cá trong hồ, thực hiện đánh dấu ký hiệu lên tất cả chúng rồi thả trở lại hồ nước. Một tuần sau, bạn tiếp tục câu 100 con cá khác và phát hiện có 30 con trong số đó có vết đánh dấu từ tuần trước. Dựa trên tỷ lệ này, bạn có thể ước tính được tổng số lượng cá đang sinh sống trong hồ là bao nhiêu.

## 科技动态

1、[Đề xuất chuẩn đèn báo tín hiệu cho xe tự hành](https://www.cnn.com/2023/12/19/business/mercedes-adds-new-light-color-blue-for-self-driving/index.html)

Hãng xe Mercedes-Benz mới đây đã được cơ quan chức năng phê chuẩn việc tích hợp thêm hệ thống đèn chiếu sáng màu xanh ngọc bích (turquoise) trên các dòng xe của mình.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122006.webp)

Khi hệ thống đèn này bật sáng, nó báo hiệu cho những người xung quanh biết chiếc xe đang hoạt động ở chế độ tự hành hoàn toàn. Ngay cả khi có người ngồi ở ghế lái, người đó lúc này cũng không hề can thiệp hay kiểm soát vô lăng.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122007.webp)

Theo thiết kế minh họa, dải đèn báo này xuất hiện ở nhiều vị trí như đèn pha phía trước, cụm đèn hậu phía sau và tích hợp trên gương chiếu hậu.

Ý tưởng thiết kế này có thể sẽ trở thành tiêu chuẩn chung cho mọi dòng xe tự hành trong tương lai, giúp người đi đường dễ dàng nhận biết xe tự hành và xe do con người điều khiển. Tuy nhiên, nếu áp dụng rộng rãi, liệu các đường phố trong tương lai có ngập tràn ánh đèn màu xanh ngọc bích?

2、[Thế hệ laptop trang bị cấu hình chip 64 nhân khủng](https://notebook.pconline.com.cn/1694/16945317.html)

Một nhà sản xuất Trung Quốc đã thực hiện ý tưởng đưa dòng chip xử lý chuyên dụng cho máy chủ AMD EPYC 64 nhân vào bên trong một chiếc máy tính xách tay, đi kèm card đồ họa RTX 4080 và hệ thống tản nhiệt bằng chất lỏng.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121718.webp)

Đây hứa hẹn là mẫu laptop có hiệu năng xử lý mạnh mẽ nhất trên thị trường hiện nay nhờ thừa hưởng cấu hình máy chủ. Các dòng laptop cao cấp nhất hiện tại thông thường cũng chỉ trang bị dòng chip tối đa 16 nhân, trong khi thiết bị này sở hữu tới 64 nhân.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121719.webp)

Độ dày của máy ở mức 4,6 cm, tuy chấp nhận được đối với cấu hình khủng nhưng kiểu dáng vuông vức thô kệch trông khá giống một viên gạch nung, thiết kế công nghiệp tổng thể còn tương đối đơn điệu.

3、[Chế độ lội nước đặc biệt trên xe bán tải Cybertruck](https://www.notebookcheck.net/Tesla-Cybertruck-seals-its-123-kWh-battery-during-river-crossings-using-the-air-suspension-tank.783958.0.html)

Elon Musk đã công bố trên X (hình dưới) rằng dòng xe Cybertruck sẽ cung cấp một gói phụ kiện nâng cấp giúp xe có khả năng di chuyển dưới nước như một chiếc thuyền trên quãng đường tối thiểu 100 mét.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122205.webp)

Trước đó, giới truyền thông đã phát hiện trong menu cài đặt của Cybertruck có tích hợp chế độ lội nước "Wade Mode" (hình dưới), chứng minh xe được thiết kế để di chuyển qua các vùng nước sâu.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122206.webp)

Tuy nhiên, với trọng lượng tự thân cực kỳ nặng, rất khó để hình dung chiếc xe này có thể nổi và di chuyển trên mặt nước. Nhiều khả năng chế độ này chỉ hỗ trợ xe lội qua các lòng suối nông nơi bánh xe vẫn có thể bám vào nền đất đáy suối.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122207.webp)

Một số trang tin đã chế ảnh hài hước dự đoán "gói phụ kiện" mà Elon Musk nhắc đến thực chất là một bộ đế phao khí đệm gắn dưới gầm xe Cybertruck.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122208.webp)

4、[Góc nhìn về biểu đồ lịch sử commit trên GitHub của lập trình viên](https://deliprao.substack.com/p/the-great-ai-weirding)

Nhiều chuyên viên tuyển dụng nhân sự (HR) mảng công nghệ tại nước ngoài thường có thói quen kiểm tra lịch sử đóng góp (commit wall) trên tài liệu GitHub của ứng viên.

Một bài viết chia sẻ rằng một biểu đồ đóng góp giống như hình dưới đây có thể để lại ấn tượng không tốt trong mắt nhà tuyển dụng và gián tiếp dẫn đến việc ứng viên bị từ chối.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122203.webp)

Lập trình viên sở hữu tài khoản này hầu như không hề viết code hay commit mã nguồn vào các ngày cuối tuần, cũng như hoàn toàn vắng bóng lịch sử đóng góp trong suốt các kỳ nghỉ lễ Giáng sinh, nghỉ xuân, nghỉ hè hay nghỉ thu.

5、[Mô hình thử nghiệm dùng cừu thay thế máy cắt cỏ tại trường đại học](https://www.ucdavis.edu/curiosity/news/surprising-benefits-of-sheep-mowers)

Để duy trì các thảm cỏ xanh trong khuôn viên luôn bằng phẳng gọn gàng, việc vận hành máy cắt cỏ là bắt buộc. Tuy nhiên, tiếng ồn lớn phát ra từ động cơ máy cắt cỏ thường gây ảnh hưởng đến không gian yên tĩnh học tập của trường.

Đại học California tại Davis mới đây đã thử nghiệm giải pháp đưa đàn cừu vào khuôn viên trường để chúng tự gặm cỏ thay thế cho máy cắt cỏ truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110210.webp)

Ban đầu đây chỉ là một dự án thử nghiệm nhỏ. Tuy nhiên kết quả thực tế cho thấy sự xuất hiện của đàn cừu thong dong gặm cỏ không chỉ làm sạch cỏ hiệu quả mà còn tạo nên một cảnh quan thiên nhiên tuyệt đẹp, mang lại hiệu ứng liệu pháp tâm lý tự nhiên giúp sinh viên cảm thấy thư thái tâm hồn.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110211.webp)

Hiện tại, việc thả đàn cừu gặm cỏ hàng ngày đã trở thành hoạt động thường niên của trường. Nhiều sinh viên chia sẻ rằng việc ngắm nhìn đàn cừu giúp họ giải tỏa áp lực học hành thi cử rất hiệu quả.

Tuy nhiên, mô hình này đòi hỏi công tác quản lý chăn nuôi khá phức tạp. Hàng ngày ban quản lý phải dùng xe tải vận chuyển đàn cừu từ trang trại vào khuôn viên trường học từ sáng sớm và đưa chúng trở lại chuồng vào buổi tối, rào cản này khiến dự án rất khó nhân rộng ra các trường khác.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110212.webp)

## Bài viết

1\. [Giải mã hiện tượng vì sao 1% pin cuối cùng trên điện thoại thường dùng được rất lâu](https://m.huxiu.com/article/2467552.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122602.webp)

Bài viết giải thích chi tiết về thuật toán ước lượng và hiển thị dung lượng pin còn lại của hệ điều hành trên các dòng điện thoại thông minh hiện nay.

2\. [Hướng dẫn gỡ bỏ hoàn toàn trình duyệt Edge trên hệ điều hành Windows](https://github.com/ruanyf/weekly/issues/3804)（Tiếng Trung）

Để tuân thủ các quy định pháp lý của Liên minh Châu Âu (EU), Microsoft buộc phải cho phép người dùng tại khu vực này gỡ cài đặt trình duyệt Edge và công cụ tìm kiếm Bing tích hợp sẵn. Độc giả đã tìm ra mẹo nhỏ giúp người dùng ở các quốc gia ngoài EU vẫn có thể thực hiện gỡ bỏ Edge. (Đóng góp của [@WFANG12719](https://github.com/ruanyf/weekly/issues/3804))

3\. [Cảnh báo tính năng cho phép ứng dụng ngầm định vị người dùng trên iPhone](https://wingu.se/2023/11/30/only-apple-can-do-allow-apps-tracking-users-location-without-consensus.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122201.webp)

Hệ điều hành iOS cung cấp một API cho phép ứng dụng đọc thông tin về các điểm truy cập Wi-Fi xung quanh thiết bị, từ đó hỗ trợ xác định chính xác vị trí thực tế của người dùng mà họ không hề hay biết, và hiện tại người dùng vẫn chưa thể chủ động tắt tính năng này.

4\. [Tìm hiểu sâu về kiến trúc đồ họa X Window System trên Linux](https://silaoa.github.io/2020/2020-04-25-Cygwin%E7%B3%BB%E5%88%97%EF%BC%88%E4%B8%80%EF%BC%89%EF%BC%9A%E4%BA%86%E8%A7%A3X.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122401.webp)

Lớp nền tảng đồ họa trên hệ điều hành Linux được xây dựng dựa trên hệ thống X Window. Bài viết giới thiệu tổng quan trực quan về nguyên lý hoạt động của cấu trúc đồ họa này. (Đóng góp của [@silaoA](https://github.com/ruanyf/weekly/issues/3790))

5\. [Sự trỗi dậy của các dòng sản phẩm phần cứng mã nguồn mở và bài toán cạnh tranh](https://lucumr.pocoo.org/2023/12/25/life-and-death-of-open-source/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122615.webp)

Một kỹ sư chia sẻ trải nghiệm sau khi mua và sử dụng dòng máy in 3D Bambu Lab A1 do Trung Quốc sản xuất. Anh đánh giá cao chất lượng máy in và nhận định các doanh nghiệp Trung Quốc đang tận dụng rất tốt các phần mềm mã nguồn mở của cộng đồng để xây dựng nên các sản phẩm phần cứng vượt trội, vô hình trung tạo ra áp lực cạnh tranh sinh tồn rất lớn cho chính các công ty phát triển mã nguồn mở ban đầu.

6\. [Hướng dẫn xây dựng công cụ dòng lệnh (CLI) bằng Node.js tiêu chuẩn](https://evertpot.com/node-changelog-cli-tool/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111320.webp)

Bài viết hướng dẫn lập trình viên tận dụng thư viện tiêu chuẩn (standard library) của Node.js để tự xây dựng một công cụ CLI hoàn chỉnh mà không cần cài đặt thêm bất kỳ module hay thư viện bên ngoài nào.

7\. [Mẹo sao chép các đoạn văn bản bị khóa tính năng copy trên Windows](https://www.howtogeek.com/how-to-copy-uncopyable-texts-on-windows/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111322.webp)

Bài viết giới thiệu 3 phương pháp đơn giản giúp bạn sao chép thành công các đoạn chữ hiển thị trên các bảng thông báo hệ thống hoặc hộp thoại ứng dụng vốn bị khóa tính năng bôi đen copy thông thường.

8\. [Tính năng quản lý đa tài khoản bằng phân vùng Container trên Firefox](https://support.mozilla.org/en-US/kb/containers)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111503.webp)

Trình duyệt Firefox hỗ trợ tính năng thiết lập các phân vùng độc lập (Multi-Account Containers). Tiện ích này không chỉ giúp bảo vệ thông tin riêng tư của bạn mà còn cho phép đăng nhập đồng thời nhiều tài khoản khác nhau của cùng một dịch vụ trên các tab trình duyệt.

## 工具

1\. [Score In URL](https://powersnail.com/ScoreInUrl/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080411.webp)

Dịch vụ trực tuyến cho phép soạn thảo và chia sẻ nhanh các bản nhạc ký âm trực tiếp trên trình duyệt, toàn bộ thông tin bản nhạc được lưu trữ gọn gàng ngay trong địa chỉ đường link URL.

2\. [Teamlinker](https://github.com/Teamlinker/Teamlinker/blob/main/README-ZH-CN.md)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122204.webp)

Dự án mã nguồn mở xây dựng nền tảng cộng tác và làm việc nhóm toàn diện tích hợp các tính năng quản lý dự án, tài liệu Wiki, lịch làm việc, họp trực tuyến, trò chuyện nhóm và lưu trữ đám mây. (Đóng góp của [@xbdsky](https://github.com/ruanyf/weekly/issues/3780))

3\. [Rspress](https://rspress.dev/zh/)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122501.webp)

Công cụ tạo trang web tĩnh hiệu năng cao dựa trên Rspack tích hợp sẵn chuỗi công cụ Rust, mang lại tốc độ biên dịch cực nhanh và thao tác cấu hình đơn giản. (Đóng góp của [@sanyuan0704](https://github.com/ruanyf/weekly/issues/3792))

4\. [AudioCut](https://audiocut.app/)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122609.webp)

Công cụ web hỗ trợ tự động cắt ghép file âm thanh, nhận diện loại bỏ khoảng lặng nhiễu hoặc các câu từ lặp lại không mong muốn, rất thích hợp cho công việc biên tập biên tập podcast. (Đóng góp của [@tangpanqing](https://github.com/ruanyf/weekly/issues/3794))

5\. [Tianji (Thiên Cơ)](https://github.com/msgbyte/tianji)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122610.webp)

Dự án mã nguồn mở tích hợp tính năng phân tích lưu lượng truy cập website, giám sát cảnh báo dịch vụ và theo dõi hiệu năng hệ thống máy chủ "3 trong 1". (Đóng góp của [@moonrailgun](https://github.com/ruanyf/weekly/issues/3795))

7\. [Memo Card](https://memocard.net/)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122611.webp)

Trang web hỗ trợ thiết kế nhanh các thẻ hình ảnh chia sẻ trích dẫn chữ nghệ thuật đẹp mắt. (Đóng góp của [@ivone-liu](https://github.com/ruanyf/weekly/issues/3803))

8\. [vocal-separate](https://github.com/ruanyf/weekly/issues/3806)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122612.webp)

Công cụ tối giản hỗ trợ tách giọng nói ca sĩ và âm nhạc nền từ file video/âm thanh, ứng dụng chạy ngoại tuyến hoàn toàn trên máy tính cá nhân giúp bảo mật dữ liệu. (Đóng góp của [@jianchang512](https://github.com/ruanyf/weekly/issues/3806))

9\. [DouyinLiveRecorder](https://github.com/ihmily/DouyinLiveRecorder)

Phần mềm hỗ trợ tự động ghi nhận và lưu lại video phát trực tiếp (livestream) từ các nền tảng phổ biến như Douyin, TikTok, Kuaishou, Huya, Douyu, Bilibili, Xiaohongshu. (Đóng góp của [@ihmily](https://github.com/ruanyf/weekly/issues/3809))

10\. [Drawing Prompt](https://drawing-prompt.com/en)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122705.webp)

Công cụ hỗ trợ tạo prompt vẽ ảnh nghệ thuật: Tự động phân tích mở rộng các mô tả ngắn bằng nhiều ngôn ngữ thành đoạn prompt tiếng Anh chi tiết, tích hợp sẵn mô hình Fast SDXL để xem trước nhanh kết quả, dịch vụ miễn phí hoàn toàn không cần đăng ký. (Đóng góp của [@dongan-beta](https://github.com/ruanyf/weekly/issues/3810))

11\. [cloudflare-ai-web](https://github.com/Jazee6/cloudflare-ai-web)

Dự án hỗ trợ xây dựng trang web giao diện AI cá nhân tận dụng dịch vụ miễn phí Cloudflare Workers, tương thích tốt với nhiều mô hình AI khác nhau. Xem bản [Demo tại đây](https://ai.jaze.top/). (Đóng góp của [@Jazee6](https://github.com/ruanyf/weekly/issues/3812))

12\. [Penumbra](https://github.com/nealmckee/penumbra)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080503.webp)

Bảng màu giao diện tối giản gồm hai chủ đề sáng và tối, được tính toán dựa trên các công thức toán học giúp mang lại độ tương phản tối ưu và giảm mỏi mắt cho người dùng.

## 资源

1\. [Trang xếp hạng các bài nghiên cứu Khoa học Máy tính nổi bật](https://trendingpapers.com/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121803.webp)

Trang web hỗ trợ cập nhật danh sách và thứ hạng thảo luận của các công trình nghiên cứu khoa học mới nhất trong ngành máy tính.

2\. [HN Telegraph](https://hntelegraph.com/)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121720.webp)

Trang web ứng dụng công nghệ AI để tự động biên tập các chủ đề nóng hàng ngày trên diễn đàn Hacker News thành các bài báo đưa tin chuyên nghiệp.

3\. [Mẫu xếp giấy các dòng máy tính cổ điển](http://rockybergen.com/papercraft)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110606.webp)

Trang web chia sẻ bản vẽ thiết kế để người dùng tải về tự gấp mô hình đồ chơi giấy các dòng máy tính cổ xưa.

4\. [Tổng hợp mẹo định dạng Markdown trên GitHub (Kickass markdown)](https://github.com/Olwiba/Kickass-markdown)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110710.webp)

Kho lưu trữ tài liệu chia sẻ các mẹo trình bày văn bản Markdown trên GitHub, ví dụ như hiển thị định dạng chữ màu trắng trên nền màu đỏ (hình minh họa trên).

5\. [Cổng tài liệu học tập của Hugging Face](https://huggingface.co/learn)

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062815.webp)

Kênh chia sẻ tri thức chính thức từ nền tảng AI Hugging Face, hiện cung cấp 3 khóa học cốt lõi: Xử lý ngôn ngữ tự nhiên (NLP), Học sâu (Deep Learning) và Xử lý âm thanh bằng AI.

## 图片

1\. [Thiết kế tường gạch lượn sóng độc đáo](https://twistedsifter.com/2020/06/how-wavy-crinkle-crankle-walls-use-less-bricks-than-straight-walls/)

Tại Anh, nhiều bức tường ngăn bằng gạch được xây dựng theo kiểu uốn lượn hình làn sóng.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072803.webp)

Về mặt cảm quan, kiểu thiết kế này trông có vẻ vừa tốn diện tích đất vừa mất nhiều công xây dựng hơn, nhưng thực tế nó lại sở hữu ưu điểm kỹ thuật rất lớn.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072804.webp)

Tương tự như cơ chế chịu lực của các vòm cầu cong, bức tường lượn sóng có khả năng chịu lực tác động tốt hơn nhiều so với tường thẳng đứng truyền thống. Do đó, thợ xây có thể dựng tường với độ dày mỏng hơn (chỉ cần một lớp gạch) mà vẫn đảm bảo độ vững chãi, giúp tiết kiệm lượng gạch vật liệu đáng kể.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072805.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072806.webp)

## ✍️ Bài đọc thêm

### Giai thoại thú vị giữa nhà vật lý Albert Einstein và Claude Shannon

Cuốn hồi ký của Claude Shannon - người được mệnh danh là cha đẻ của Thuyết thông tin - có ghi lại một câu chuyện giao lưu ngắn ngủi đầy hài hước giữa ông và nhà vật lý vĩ đại Albert Einstein.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122702.webp)

Sau khi tốt nghiệp học vị Tiến sĩ, Shannon chuyển đến làm nghiên cứu tại Viện Nghiên cứu Cao cấp Princeton, nơi Einstein cũng đang làm việc tại đây.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122703.webp)

Vào thời điểm đó, Shannon mới chỉ là một giảng viên trẻ tuổi vô danh, trong khi danh tiếng của Einstein đã lẫy lừng khắp thế giới.

Trong một buổi lên lớp giảng bài của Shannon cho các nhà toán học tại viện nghiên cứu, cánh cửa phía sau giảng đường khẽ mở và Einstein bước vào.

Einstein đứng lặng im nghe giảng ở góc phòng học trong vài phút, sau đó ghé tai thì thầm trò chuyện một câu ngắn với người ngồi hàng ghế cuối cùng rồi rời đi.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122704.webp)

Ngay khi buổi học kết thúc, Shannon đã vội vã chạy xuống hàng ghế cuối để tìm gặp người được Einstein thì thầm trò chuyện ban nãy, vô cùng hồi hộp muốn biết xem vị học giả vĩ đại kia đã đưa ra nhận xét hay đánh giá học thuật gì về bài giảng của mình.

Người đó đã mỉm cười trả lời ông: "Einstein thực ra chỉ hỏi tôi lối đi ra nhà vệ sinh ở đâu."

## Lịch sử tuần này

- 2022年（第 237 期）：[Mạng xã hội: Giải thích các phương pháp kỹ thuật giúp xác định vị trí thực tế của người dùng](https://www.ruanyifeng.com/blog/2022/12/weekly-issue-237.html)
- 2021年（第 187 期）：[Xu thế công nghệ: Thảo luận về triển vọng và khả năng thành công thực tế của mô hình Vũ trụ ảo (Metaverse)](https://www.ruanyifeng.com/blog/2021/12/weekly-issue-187.html)
- 2020年（第 137 期）：[Thương vụ công nghệ: Phân tích sự kiện Slack được mua lại và bài học về lựa chọn công nghệ của doanh nghiệp](https://www.ruanyifeng.com/blog/2020/12/weekly-issue-136.html)
- 2019年（第 87 期）：[Phương pháp làm việc: Lời khuyên về tầm quan trọng của việc thành viên mới chủ động viết tài liệu cho nhóm](https://www.ruanyifeng.com/blog/2019/12/weekly-issue-87.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
