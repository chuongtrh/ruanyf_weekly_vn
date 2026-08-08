# 科技爱好者周刊（第 238 期）：停止寻找的最佳时间

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần。

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn。

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập。

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010507.webp)

Vào cuối năm ngoái, một buổi đấu giá bộ xương hóa thạch khủng long bạo chúa (T-Rex) khổng lồ đã bị hủy bỏ khẩn cấp. Nguyên nhân do có chuyên gia gửi báo cáo khiếu nại, chỉ ra cấu trúc xương sọ của bộ hóa thạch này giống hệt một mẫu vật T-Rex đang được trưng bày trước đó, dấy lên nghi vấn làm giả hóa thạch tinh vi để trục lợi đấu giá. (Nguồn: [Toutiao](https://www.toutiao.com/article/7168670394131022344/?wid=1672904731426))

## 本周话题：停止寻找的最佳时间

Gần đây, tôi có đọc một cuốn sách toán học ứng dụng của tác giả người Mỹ [Brian Christian](https://brianchristian.org/).

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010202.webp)

Tác phẩm gốc tiếng Anh có tựa đề là *《Algorithms to Live By》* (Thuật toán ứng dụng trong cuộc sống).

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010203.webp)

Bản dịch tiếng Trung của sách được xuất bản dưới tên gọi *《Vẻ đẹp của thuật toán》* (NXB Trung Tín, 2018).

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010204.webp)

Thực sự mà nói, tên bản dịch tiếng Trung dễ gây hiểu nhầm cho độc giả. **Tôi vốn nghĩ đây là một cuốn sách kỹ thuật viết về thuật toán lập trình máy tính, nhưng nội dung của nó thực chất là chia sẻ về cách ứng dụng các lý thuyết toán học vào giải quyết các vấn đề thường nhật.**

Cuốn sách được viết theo văn phong phổ biến kiến thức, hạn chế tối đa các công thức toán học hay dòng code phức tạp để hướng tới đại đa số độc giả. Tuy nhiên, việc thiếu các công thức chứng minh đôi lúc khiến việc giải thích logic ở một số chương trở nên hơi khó hiểu và chưa thực sự triệt để.

Dù vậy, cuốn sách vẫn chia sẻ rất nhiều kiến thức toán học ứng dụng thú vị. Hôm nay tôi muốn giới thiệu chương đầu tiên của sách mang tên **“Optimal Stopping” (Thời điểm dừng tối ưu) – Khi nào chúng ta nên dừng việc tìm kiếm để đưa ra quyết định?**

Trong cuộc sống, chúng ta liên tục phải đối mặt với các chuỗi “Tìm kiếm – Đưa ra quyết định”. Nếu dành quá nhiều thời gian để khảo sát hết tất cả các lựa chọn hiện có, chúng ta sẽ lãng phí thời gian và dễ bỏ lỡ các cơ hội tốt trước đó (những cơ hội sau chưa chắc đã tốt bằng cơ hội trước). Liệu có một mốc thời gian tối ưu nào giúp chúng ta dừng khảo sát và chọn ngay phương án tốt nhất với tỷ lệ thành công cao nhất hay không?

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010205.webp)

Trong toán học xác suất, bài toán này được gọi là [“Bài toán thư ký”](https://en.wikipedia.org/wiki/Secretary_problem).

Giả sử một công ty cần tuyển dụng 1 vị trí thư ký và có 100 ứng viên tham gia phỏng vấn lần lượt. Quy tắc đặt ra là ngay sau khi kết thúc cuộc phỏng vấn với mỗi ứng viên, nhà tuyển dụng phải đưa ra quyết định ngay lập tức là nhận hay từ chối người đó. Bạn không thể phỏng vấn hết 100 người rồi mới quay lại chọn người tốt nhất; một khi bạn đã từ chối một ứng viên, cơ hội sở hữu người đó sẽ trôi qua vĩnh viễn.

Quy định này mô phỏng chân thực các cơ hội xuất hiện trong cuộc sống: cơ hội thường đến nhanh và trôi qua rất mau, nếu bạn không quyết định nắm giữ ngay, bạn sẽ không thể lấy lại nó sau này.

Vậy trong tình huống này, bạn nên phỏng vấn bao nhiêu ứng viên để làm cơ sở rồi mới bắt đầu đưa ra quyết định tuyển dụng?

Nếu quyết định chọn quá sớm, bạn có thể bỏ lỡ những ứng viên xuất sắc hơn phía sau; nếu chần chừ chọn quá muộn, bạn có thể đã vô tình từ chối mất ứng viên đạt chuẩn nhất ở nhóm đầu.

Các nhà toán học đã nghiên cứu sâu bài toán này và chứng minh được phương pháp mang lại tỷ lệ chọn trúng người tốt nhất là **“Quy tắc 1/e”** (1/e law). Với e là hằng số logarit tự nhiên xấp xỉ bằng 2,718, tỷ số 1/e sẽ tương đương khoảng 37%. Do đó quy tắc này còn được gọi là **“Quy tắc 37%”**.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010206.webp)

**Ý nghĩa của Quy tắc 37% là: Hãy dành 37% thời gian hoặc số lượng cơ hội đầu tiên để làm giai đoạn khảo sát chuẩn.** Đối với 100 ứng viên, bạn hãy phỏng vấn 37 người đầu tiên và hoàn toàn không tuyển dụng họ – nhóm này chỉ đóng vai trò thiết lập thang điểm chuẩn đánh giá. Từ ứng viên thứ 38 trở đi, ngay khi gặp ứng viên nào có điểm số đánh giá vượt trội hơn tất cả những người trong nhóm 37 người đầu tiên, bạn hãy quyết định ký hợp đồng ngay lập tức và dừng phỏng vấn.

Tất nhiên, nếu ứng viên tốt nhất thực sự nằm ở nhóm 37 người đầu tiên, bạn bắt buộc phải chấp nhận bỏ lỡ họ như một chi phí khảo sát bắt buộc của thuật toán. Lựa chọn sau đó của bạn sẽ là ứng viên tốt nhất còn lại của nhóm sau.

Quy tắc 37% này rất hữu dụng và có thể áp dụng vào nhiều khía cạnh đời sống:

1. **Tìm kiếm bạn đời**: Nếu bạn dự định làm quen và hẹn hò với khoảng 10 đối tượng trước khi kết hôn, hãy dành 3 đến 4 người đầu tiên làm nhóm tìm hiểu thiết lập tiêu chuẩn. Từ đối tượng thứ 5 trở đi, nếu gặp ai tốt hơn tất cả những người trước đó, bạn nên nghiêm túc cân nhắc tiến tới hôn nhân.
2. **Thuê nhà**: Nếu bạn dành ra 30 ngày để tìm thuê nhà, hãy tính toán 37% của 30 ngày là 11 ngày. Dành 11 ngày đầu tiên để đi xem và khảo sát giá cả thị trường. Từ ngày thứ 12, hễ gặp căn hộ nào tốt hơn tất cả các căn hộ đã xem ở nhóm trước, hãy quyết định xuống tiền cọc ngay lập tức.
3. **Đọc sách**: Nếu một cuốn sách dày 100 trang, bạn hãy kiên nhẫn đọc hết 37 trang đầu. Nếu sau trang 37 cuốn sách vẫn không mang lại cho bạn nội dung hứng thú, bạn có thể dừng lại và từ bỏ cuốn sách.
4. **Xem phim**: Đối với một bộ phim truyền hình dài 10 tập, tập 4 chính là thời điểm tối ưu để bạn quyết định có nên bỏ phim (drop) nếu thấy nội dung không hấp dẫn.
5. **Xem video ngắn**: Đối với một video thời lượng 10 phút, nếu xem đến 3 phút 42 giây đầu tiên mà bạn vẫn thấy tẻ nhạt, bạn nên tắt video để tiết kiệm thời gian.
6. **Định hướng sự nghiệp**: Nếu một người trẻ muốn dành 7 năm (từ 18 tuổi đến 24 tuổi) để thử nghiệm tìm kiếm hướng đi cuộc đời. Anh ta sẽ có khoảng 2,59 năm đầu (tương đương đến hết học kỳ 2 năm thứ 3 đại học) để tự do thử nghiệm các lĩnh vực khác nhau. Sau mốc này, anh ta nên tập trung phát triển sự nghiệp theo hướng đã chọn và hạn chế thay đổi trừ khi gặp cơ hội cực kỳ đột phá.

## 科技动态

1、[Intel công bố phần mềm phát hiện video deepfake dựa trên lưu lượng tuần hoàn máu](https://www.zdnet.com/article/intels-new-deepfake-detector-can-spot-a-real-or-fake-video-based-on-blood-flow-in-video-pixels/)

Các công cụ AI tạo video giả mạo (deepfake) ngày càng tinh vi khiến người xem mắt thường rất khó phát hiện ra thật giả:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111903.webp)

Tập đoàn Intel vừa giới thiệu công cụ phần mềm mang tên FakeCatcher hỗ trợ phát hiện các video deepfake với độ chính xác đạt tới 96%. Nguyên lý của phần mềm dựa trên việc phân tích lưu lượng tuần hoàn máu hiển thị qua sự thay đổi màu sắc cực nhỏ của các điểm ảnh (pixel) trên da mặt người trong video. Đối với các video do AI vẽ ra, cấu trúc tuần hoàn máu tự nhiên này hoàn toàn không tồn tại.

2、[Hệ thống cứu thương khẩn cấp bằng drone trợ lực](https://finance.sina.com.cn/jjxw/2023-01-04/doc-imxyyvkp9014558.shtml)

Đại học Chiết Giang vừa công bố dự án nghiên cứu hệ thống thiết bị bay cứu thương không người lái (drone) hỗ trợ y tế khẩn cấp:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010406.webp)

Khi bệnh nhân gặp sự cố chấn thương hoặc tim mạch đột ngột ở khu vực hẻo lánh, drone sẽ tự động bay đến vị trí GPS định vị để thả hộp thuốc tự động cứu trợ. Thiết bị tiêm thuốc được thiết kế dạng đai áp sát vào da, lực nén lò xo sẽ tự động kích hoạt đẩy các đầu kim siêu nhỏ bơm thuốc qua da mà không cần thao tác tiêm của nhân viên y tế. Tuy nhiên tính thực tiễn của dự án bị hoài nghi vì nếu bệnh nhân vẫn đủ tỉnh táo để tự lấy thuốc từ drone đeo vào người thì tình trạng bệnh thường chưa đến mức quá nguy kịch.

3、[Microsoft công bố nghiên cứu về xu hướng 3 đỉnh làm việc của nhân sự làm việc từ xa](https://www.microsoft.com/en-us/worklab/triple-peak-day)

Đội ngũ phát triển ứng dụng Office 365 của Microsoft vừa thực hiện thống kê hành vi sử dụng công cụ làm việc trực tuyến của nhân sự làm việc tại nhà (Work From Home) và phát hiện ra hiện tượng "Triple Peak Day" (Ngày làm việc 3 đỉnh):

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010407.webp)

Bên cạnh hai đỉnh làm việc thông thường vào ban ngày (10h-11h sáng và 2h-3h chiều), biểu đồ ghi nhận một đỉnh làm việc thứ ba xuất hiện vào ban đêm từ 10h đến 11h tối trước khi đi ngủ. Dữ liệu gợi ý các nhà quản lý có thể linh hoạt rút ngắn thời gian làm việc văn phòng buổi chiều để nhân viên nghỉ ngơi và xử lý nốt công việc trực tuyến vào ban đêm.

4、[Hệ thống sạc siêu nhanh công suất lớn cho xe điện](https://insideevs.com/news/621173/cavotec-brugg-econnect-3mw-mcs-connector/)

Hai doanh nghiệp Thụy Sĩ vừa phối hợp nghiên cứu thành công hệ thống sạc pin siêu nhanh công suất lớn dành cho xe điện với điện áp ngõ ra 1.250V và cường độ dòng điện lên tới 3.000A:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010508.webp)

Do cường độ dòng điện cực lớn sinh nhiệt cao, dây dẫn điện và đầu cắm sạc được chế tạo với kích thước khổng lồ vượt xa các súng sạc xe điện thông thường để bảo đảm an toàn:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010509.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010510.webp)

Lõi cáp sạc gồm 4 đường ống đồng dẫn điện có đường kính lớn bằng miệng bát cơm để tối ưu hóa khả năng truyền tải điện năng mà không gây quá nhiệt:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010511.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010512.webp)

## 文章

1\. [Làm thế nào để xây dựng các tòa nhà chống động đất hiệu quả?](https://mp.weixin.qq.com/s/JHJ-GTQqbK9ZmxMAtlNszA)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010504.webp)

Bài thuyết trình khoa học của một tiến sĩ ngành kiến trúc giải thích các giải pháp thiết kế kết cấu thép, móng giảm chấn lò xo giúp các tòa tháp cao tầng tự triệt tiêu lực chấn động của động đất để bảo đảm an toàn xây dựng.

2\. [Tại sao hàm calloc() tồn tại song song với malloc() trong C?](https://vorpus.org/blog/why-does-calloc-exist/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111408.webp)

Ngôn ngữ lập trình C cung cấp hai hàm cấp phát bộ nhớ động là `malloc()` và `calloc()`. Bài viết phân tích các tối ưu hóa phần cứng của hệ điều hành giúp hàm `calloc()` (tự động xóa trắng vùng nhớ về giá trị 0) hoạt động hiệu quả hơn so với việc gọi `malloc()` rồi chạy vòng lặp gán giá trị thủ công.

3\. [Lịch sử thăng trầm của hệ điều hành máy tính BeOS](https://www.abortretry.fail/p/be-is-nice-end-of-story)（Tiếng Anh）

Bài viết kể về chặng đường lịch sử của hệ điều hành BeOS. Vào năm 1996 khi Apple khủng hoảng tìm kiếm hệ điều hành mới để mua lại, họ đã cân nhắc giữa BeOS và NeXT (của Steve Jobs). Cuối cùng Apple chọn NeXT, còn BeOS sau đó dừng phát triển thương mại và được cộng đồng phát triển mã nguồn mở tiếp quản dưới tên dự án Haiku OS hiện nay.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111603.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111604.webp)

4\. [Phân tích các nguyên nhân khiến Git phức tạp và khó sử dụng](https://www.highflux.io/blog/what-makes-git-hard-to-use)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111723.webp)

Bài viết phân tích các khái niệm thiết kế kiến trúc lưu trữ của Git (như Index, Staging Area, Detached HEAD) giải thích lý do tại sao các câu lệnh của Git thường khó hiểu và dễ gây ra nhầm lẫn cho các lập trình viên mới.

5\. [Các mẹo tối ưu khi nạp dữ liệu bằng thư viện Pandas](https://dataground.io/2022/08/02/loading-data-into-pandas-5-tips-and-tricks-you-may-or-may-not-know/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080501.webp)

Giới thiệu 5 mẹo lập trình hữu ích giúp tối ưu hóa bộ nhớ và tăng tốc độ xử lý khi sử dụng thư viện Pandas của Python để đọc các tệp tin dữ liệu CSV, JSON dung lượng lớn.

6\. [Viết cấu trúc ảnh SVG đơn giản tương tự như CSS](https://yuanchuan.dev/experimenting-a-new-syntax-to-write-svg)（Tiếng Anh）

Tác giả chia sẻ công cụ do mình phát triển giúp đơn giản hóa cú pháp手 viết ảnh vector SVG, chuyển đổi các thẻ vẽ hình học phức tạp thành dạng cú pháp thuộc tính ngắn gọn, trực quan tương tự như CSS.

7\. [Hướng dẫn thiết lập quy trình Blue-Green Deployment cho web cá nhân](https://casparwre.de/blog/webapp-python-deployment/)（Tiếng Anh）

Bài viết hướng dẫn thiết lập hệ thống tự động hóa triển khai ứng dụng web sử dụng đồng thời hai máy chủ (một chạy Production nhận traffic và một chạy Staging thử nghiệm) để cập nhật phiên bản mới không gây gián đoạn hệ thống.

8\. [Các phương pháp kiểm tra rò rỉ bộ nhớ trong Node.js](https://blog.appsignal.com/2022/09/28/minimize-heap-allocations-in-nodejs.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092902.webp)

Bài hướng dẫn chi tiết cách thức sử dụng các công cụ Chrome DevTools để chụp ảnh bộ nhớ đệm (heap snapshots) phục vụ tìm kiếm các đối tượng rò rỉ bộ nhớ (memory leaks) trong ứng dụng Node.js chạy trên server.

## 工具

1、[Bolt.css: Framework định dạng CSS tối giản không dùng class](https://boltcss.com/)

Tiện ích CSS siêu nhẹ tự động tối ưu hóa hiển thị cho toàn bộ các thẻ HTML gốc mà không yêu cầu lập trình viên phải khai báo các class CSS tùy biến.

2、[zlib searcher: Công cụ tìm kiếm sách điện tử z-library cục bộ](https://github.com/zlib-searcher/zlib-searcher)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022123006.webp)

Dự án mã nguồn mở cho phép người dùng thiết lập máy chủ tìm kiếm dữ liệu thư viện sách z-library ngoại tuyến ngay trên máy tính cá nhân để phục vụ tra cứu học tập. (Tham khảo bản [Demo 1](https://zlib.knat.network/) hoặc [Demo 2](https://zlib.freedit.eu/)).

3、[Auth.js: Thư viện xác thực đăng nhập đa năng cho lập trình web](https://authjs.dev/)

Thư viện xác thực tài khoản đăng nhập đa năng hỗ trợ kết nối nhanh với hàng chục dịch vụ OAuth lớn (GitHub, Google, Apple) được nâng cấp từ module NextAuth.js để hỗ trợ rộng rãi cho mọi JS frameworks:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022123101.webp)

4、[Mind FM: Ứng dụng iOS hỗ trợ nghe nhạc nền tập trung công việc](https://apps.apple.com/cn/app/mind-fm/id6443691710)

Ứng dụng di động cung cấp kho âm thanh tiếng ồn trắng, nhạc LoFi và sóng não giúp người dùng thư giãn, nâng cao năng suất tập trung khi viết code. (Đóng góp của [@ddiiiik](https://github.com/ruanyf/weekly/issues/2834))

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010503.webp)

5、[sapic: Hệ thống tự vận hành kho lưu trữ hình ảnh nguồn mở](https://github.com/sapicd/sapic)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010502.webp)

Mã nguồn mở xây dựng trang dịch vụ lưu ảnh (圖床), hỗ trợ đồng bộ lưu trữ ảnh lên thư mục local hoặc kết nối API tải ảnh lên các dịch vụ đám mây lớn (Aliyun, Tencent Cloud, S3, GitHub). (Đóng góp của [@staugur](https://github.com/ruanyf/weekly/issues/2833))

6、[steganography: Tiện ích dòng lệnh ẩn giấu tệp tin vào ảnh viết bằng C++](https://github.com/7thSamurai/steganography)

Công cụ mã hóa dữ liệu sử dụng kỹ thuật giấu tin (steganography) cho phép người dùng nén và ẩn giấu hoàn toàn một tệp tin zip vào bên trong một bức ảnh dạng PNG mà không làm thay đổi chất lượng hiển thị của ảnh.

## JSON 可视化工具

Dữ liệu JSON là định dạng truyền tải thông tin mạng phổ biến nhưng có cấu trúc thô khó đọc và sửa đổi bằng mắt thường. Dưới đây là các tiện ích web hỗ trợ trực quan hóa dữ liệu JSON:

1、[JSON Visualization (Bảng hóa dữ liệu JSON)](https://altearius.github.io/tools/json/index.html)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112905.webp)

Công cụ hỗ trợ chuyển đổi nhanh cấu trúc dữ liệu JSON phức tạp thành dạng bảng biểu hàng cột trực quan dễ theo dõi.

2、[JSON Viewer (jsonhero.io): Trình xem cấu trúc JSON phân tầng](https://jsonhero.io/)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112906.webp)

Giao diện web trực quan hiển thị cấu trúc phân nhánh của dữ liệu JSON giúp lập trình viên nhanh chóng kiểm tra các trường thông tin lồng nhau.

3、[jq play: Môi trường chạy thử nghiệm dòng lệnh truy vấn JSON](https://jqplay.org/)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112603.webp)

Trình giả lập chạy thử các câu lệnh truy vấn dữ liệu JSON bằng công cụ dòng lệnh `jq` ngay trên giao diện web để kiểm tra kết quả filter.

4、[JsonT.run: Tiện ích trực tuyến chỉnh sửa JSON gọn nhẹ](https://www.jsont.run/)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010501.webp)

Công cụ web trực tuyến hỗ trợ định dạng, kiểm tra lỗi cú pháp và chỉnh sửa cấu trúc file dữ liệu JSON nhanh chóng cho lập trình viên. (Đóng góp của [@bimohxh](https://github.com/ruanyf/weekly/issues/2832))

## 资源

1、[Systemd by Example: Trang web học viết cấu hình Systemd trực quan](https://systemd-by-example.com/)

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022012604.webp)

Dịch vụ web giáo dục cung cấp các ví dụ mẫu hướng dẫn viết tệp tin cấu hình dịch vụ Systemd trên Linux, tích hợp trình chạy ảo để người dùng kiểm tra kết quả khởi chạy dịch vụ trực tiếp.

2、[Danh sách thống kê top 1 triệu tên miền lớn nhất thế giới của Google](https://github.com/zakird/crux-top-lists)

Dữ liệu thống kê nguồn mở tải về dạng CSV lưu trữ thông tin về 1 triệu trang web có lưu lượng truy cập lớn nhất toàn cầu dựa trên dữ liệu báo cáo ẩn danh Chrome User Experience Report của Google.

3、[Killed by Microsoft (Nghĩa trang các sản phẩm bị Microsoft khai tử)](https://killedbymicrosoft.info/)

Trang web tổng hợp thông tin lịch sử ghi lại chi tiết các phần mềm, dịch vụ đám mây và thiết bị phần cứng đã bị tập đoàn Microsoft chính thức ngừng phát triển và khai tử trong lịch sử:

![](https://cdn.beekka.com/blogimg/asset/202203/bg2022032903.webp)

4、[Giáo trình hướng dẫn chuyển đổi sử dụng zsh trên hệ điều hành macOS](https://scriptingosx.com/2019/06/moving-to-zsh/)（Tiếng Anh）

Bộ tài liệu hướng dẫn chi tiết gồm 8 phần giúp lập trình viên làm quen và cấu hình Terminal sử dụng shell `zsh` khi Apple chính thức chuyển đổi shell mặc định từ Bash sang zsh trên macOS.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072303.webp)

## 图片

1\. **Sự cố dập kính nung chảy nhựa ô tô của tòa nhà kính cong tại London**

Năm 2012, một tòa cao ốc văn phòng mặt kính tại trung tâm London hoàn thành thi công với kiến trúc phần đỉnh phình to hơn phần đế và mặt kính thiết kế hơi lõm vào trong:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010304.webp)

Khi đưa vào hoạt động, vào những ngày nắng gắt, toàn bộ mặt kính cong lõm của tòa nhà vô tình hoạt động như một thấu kính hội tụ (凹面镜) khổng lồ:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010305.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010306.webp)

Toàn bộ ánh sáng mặt trời phản xạ từ mặt kính được hội tụ vào một khu vực nhỏ dưới lòng đường bên dưới:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010307.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010308.webp)

Nhiệt độ tại điểm hội tụ đo được lên tới 72 độ C, làm chảy các chi tiết nhựa và nứt kính của những chiếc xe ô tô đỗ bên dưới. Người dân địa phương thậm chí đã thực hiện chiên trứng chín trực tiếp tại điểm hội tụ nắng này:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010309.webp)

Chủ đầu tư tòa nhà sau đó đã phải chi trả toàn bộ chi phí bồi thường thiệt hại cho các chủ xe và tiến hành lắp đặt hệ thống mái che nắng vĩnh viễn tại khu vực hội tụ ánh sáng này để khắc phục sự cố kiến trúc.

## ✍️ Bài đọc thêm

### Hiện tượng "Tâm lý phủ nhận" của con người trước các hiểm họa lớn

Dưới đây là một đoạn trích dẫn phân tích từ cuốn sách nổi tiếng *《Sụp đổ: Các xã hội đã thất bại hoặc thành công như thế nào》* của nhà sinh vật học Jared Diamond (tác giả cuốn sách đạt giải Pulitzer *Súng, vi trùng và thép*):

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010513.webp)

Một cuộc điều tra xã hội học được thực hiện đối với các hộ dân cư sinh sống dọc theo một thung lũng sông hẹp nằm ở khu vực hạ lưu của một con đập thủy điện khổng lồ:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010514.jpg)

Kết quả khảo sát thu được một số liệu rất bất ngờ: Những hộ dân sống cách con đập vài dặm về phía hạ lưu lại là nhóm người biểu thị sự lo lắng cao nhất về nguy cơ con đập có thể bị vỡ. Trong khi đó, các hộ dân sinh sống ngay sát chân đập thủy điện lại hoàn toàn thản nhiên và không hề lo sợ.

Nguyên nhân của hiện tượng này được lý giải bằng khái niệm **“Psychological denial” (Tâm lý phủ nhận)** trong tâm lý học:

Những người dân sống sát chân đập hàng ngày hễ ngẩng đầu lên là nhìn thấy bức tường bê tông khổng lồ của đập nước. Nếu họ luôn sống trong sự nơm nớp lo sợ con đập có thể vỡ bất cứ lúc nào, cuộc sống hàng ngày của họ sẽ rơi vào trạng thái hoảng loạn không thể chịu đựng nổi.

Để bảo vệ tâm lý ổn định cho bản thân để tiếp tục sinh sống, cơ chế phòng vệ của não bộ sẽ tự động khởi động trạng thái "phủ nhận" – từ sâu trong tiềm thức, họ tự thuyết phục bản thân rằng con đập này tuyệt đối an toàn và không bao giờ có thể vỡ, bất chấp các nguy cơ vật lý thực tế.

Đây là cơ chế phản ứng phi lý trí của con người khi đối mặt với một mối hiểm họa quá lớn nằm ngoài khả năng giải quyết của cá nhân, não bộ sẽ tự động đè nén nhận thức về mối nguy hiểm đó để tránh sự đau khổ về tinh thần, dù hành vi này đôi khi dẫn đến những hậu quả thảm khốc nếu tai nạn thực sự xảy ra.

## 历史上的本周

- 2021年（第 190 期）：[Định hướng tư duy: Tầm quan trọng của việc xây dựng tư duy đóng gói sản phẩm thương mại đối với lập trình viên](https://www.ruanyifeng.com/blog/2021/12/weekly-issue-190.html)
- 2020年（第 140 期）：[Kinh tế lao động: Thống kê và phân tích mức lương trung bình của lập trình viên tại thị trường Ấn Độ](https://www.ruanyifeng.com/blog/2020/12/weekly-issue-140.html)
- 2019年（第 88 期）：[Triết lý cuộc sống: Bài học ứng biến thực tế khi bạn bất ngờ đối mặt với một tình huống nguy hiểm](https://www.ruanyifeng.com/blog/2019/12/weekly-issue-88.html)
- 2018年（第 37 期）：[Thảo luận thời đại: Tại sao thời kỳ hoàng kim của các nhà văn tiểu thuyết truyền thống đã trôi qua vĩnh viễn](https://www.ruanyifeng.com/blog/2018/12/weekly-issue-37.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## 鸣谢

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072108.webp)

（Hết）
