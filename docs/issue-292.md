# Bản tin chia sẻ công nghệ (Số 292): Mọi đoạn mã đều là nợ kỹ thuật

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/4075) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030705.webp)

Ý tưởng thiết kế nhà ga mới cho sân bay Florence của Ý. Phía trên mái nhà ga sẽ được cải tạo thành một vườn nho rộng 7,7 ha chuyên phục vụ cho hoạt động sản xuất rượu vang nổi tiếng địa phương. (Nguồn: [Euronews](https://www.euronews.com/travel/2024/02/14/wine-meets-travel-florences-new-airport-will-have-a-vineyard-on-its-roof))

## 所有代码都是技术债

Mã nguồn (code) thường được các công ty xem là tài sản và khuyến khích các kỹ sư viết thật nhiều code. Tuy nhiên, nhiều người (đặc biệt là cấp quản lý) không nhận thức được rằng **bản thân code cũng chính là một khoản nợ**.

Viết càng nhiều code, khoản nợ tích lũy càng lớn, đó chính là khái niệm "nợ kỹ thuật" (technical debt) mà giới lập trình viên vẫn thường nhắc tới.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030702.webp)

Hôm nay, tôi muốn thảo luận về khái niệm "nợ kỹ thuật" này, và lý do vì sao việc sở hữu quá nhiều mã nguồn không hẳn là một dấu hiệu tốt cho doanh nghiệp.

Khái niệm "nợ kỹ thuật" (technical debt) xuất hiện lần đầu trong [một bài nghiên cứu](https://queue.acm.org/detail.cfm?id=2168798) của lập trình viên nổi tiếng Ward Cunningham. Ông đã đưa ra nhận định rất thực tế: "**Việc phát hành code cũng giống như việc bạn đi vay nợ vậy**."

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030703.webp)

Một khi đoạn code của bạn được triển khai lên môi trường thực tế (production), nó giống như một khoản nợ tài chính mà bạn bắt buộc phải liên tục trả lãi suất bảo trì định kỳ sau này, trừ phi đoạn code đó bị vô hiệu hóa hoàn toàn.

Phép so sánh này đã nhận được sự đồng thuận lớn của cộng đồng công nghệ, và **người ta gọi gánh nặng do mã nguồn mang lại là "nợ kỹ thuật"**.

Vì sao việc viết code lại tương tự như đi vay nợ? Điều này xuất phát từ hai nguyên nhân chính dưới đây.

Nguyên nhân thứ nhất là do các giới hạn về thời gian hay nguồn lực tại thời điểm phát triển, giải pháp kỹ thuật đưa ra có thể chưa tối ưu, chứa lỗi tiềm ẩn (Bug) hoặc lựa chọn các thư viện phụ thuộc kém chất lượng, đòi hỏi đội ngũ kỹ sư phải liên tục sửa đổi hoặc viết lại sau này.

Nguyên nhân thứ hai là ngay cả khi đoạn code của bạn được viết một cách hoàn hảo nhất, thì dưới sự phát triển không ngừng của công nghệ, nó cũng sẽ dần trở nên lỗi thời theo thời gian. Do đó, bạn bắt buộc phải liên tục bảo trì và cập nhật hệ thống để tương thích, và chi phí này thông thường còn cao hơn cả chi phí phát triển ban đầu.

Điều này đồng nghĩa với việc **dù bạn có cẩn thận đến đâu, bất kỳ đoạn code nào được phát hành cũng đều mang theo mình một khoản nợ kỹ thuật**. Chúng ta hoàn toàn có thể khẳng định rằng: [mọi đoạn mã được viết ra đều là nợ kỹ thuật](https://www.tokyodev.com/articles/all-code-is-technical-debt).

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030704.webp)

Sự nguy hại của nợ kỹ thuật nằm ở chỗ bạn bắt buộc phải liên tục trả lãi suất bảo trì định kỳ. Nếu bạn tìm cách trì hoãn, khoản nợ này sẽ tích tụ như quả cầu tuyết khiến chi phí bảo trì hệ thống tăng phi mã, cho đến khi hệ thống trở nên quá tải và buộc phải loại bỏ hoàn toàn.

Do mọi đoạn code đều là nợ kỹ thuật, các lập trình viên khi viết code bắt buộc phải cân nhắc kỹ lưỡng đến chi phí bảo trì dài hạn của nó để giảm thiểu gánh nặng cho bản thân và đồng nghiệp trong tương lai.

Một nguyên lý cơ bản là **viết càng ít code, nợ kỹ thuật càng nhỏ; không viết code thì không phát sinh nợ kỹ thuật**. Dưới góc nhìn này, quy trình phát triển phần mềm chuẩn xác nên tuân thủ hai quy tắc sau:

1. Chủ động dọn dẹp và xóa bỏ các đoạn code dư thừa.

2. Chỉ tập trung phát triển các tính năng thực sự cần thiết, tuyệt đối không bổ sung các tính năng dư thừa khi chưa có yêu cầu rõ ràng. Việc bổ sung tính năng mới chắc chắn sẽ làm phát sinh thêm code mới, và một khi đã tích hợp vào hệ thống thì việc gỡ bỏ nó sau này sẽ rất khó khăn.

## 葫芦 AI

Hầu hết các mô hình AI phổ biến hiện nay đều áp dụng mô hình trả phí định kỳ. Việc sử dụng đồng thời nhiều mô hình AI khác nhau sẽ tiêu tốn một khoản kinh phí không nhỏ hàng tháng của lập trình viên, đi kèm các thủ tục đăng ký thanh toán khá phức tạp.

> - GPT-4: 20 USD/tháng
> - ERNIE Bot: 49.9 Nhân dân tệ/tháng
> - Midjourney: 10 USD/tháng
> - DALL-E: 0.02 USD/mỗi ảnh tạo ra

Dịch vụ AI nội địa mang tên "Hồ Lô AI" (HuLu AI) ra đời nhằm giải quyết triệt để bài toán này. **Dịch vụ hỗ trợ người dùng truy cập đồng thời cả 4 mô hình AI trên trực tiếp trên một giao diện duy nhất**, hoạt động giống như một cổng mirror tích hợp tiện lợi.

Dịch vụ mới ra mắt đang trong chương trình ưu đãi trải nghiệm rất lớn, **chỉ với 298 Nhân dân tệ, người dùng được cấp quyền sử dụng không giới hạn trọn đời**, giúp loại bỏ các thủ tục thanh toán phức tạp của từng dịch vụ riêng lẻ đi kèm tốc độ phản hồi cực nhanh.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030706.webp)

Hồ Lô AI mong muốn thông qua chuyên mục của bản tin để giới thiệu sản phẩm đến cộng đồng lập trình viên. Sau khi kết thúc chương trình ưu đãi, mức giá dịch vụ trọn đời sẽ quay về mức giá gốc 498 Nhân dân tệ.

Hệ thống có cung cấp lượt dùng thử miễn phí, độc giả chỉ cần quét mã QR trên ảnh poster để **trải nghiệm dùng thử miễn phí dịch vụ**. Sau khi thấy hài lòng với chất lượng, bạn mới cần cân nhắc đến việc nâng cấp gói trả phí.

Bên cạnh đó, đối với những bạn mới bắt đầu tiếp cận AI, Hồ Lô AI tặng kèm bộ tài liệu học tập miễn phí. Khi quét mã QR trên ảnh poster để liên hệ bộ phận hỗ trợ khách hàng qua WeChat, bạn sẽ nhận được bộ tài liệu AI giá trị bao gồm: **【Cẩm nang nhập môn Sora】** + **【Thư viện prompt ChatGPT toàn tập】** + **【Cẩm nang thực chiến kiếm tiền từ công nghệ AI】**.

## 科技动态

1、[Thiết bị giảm ngứa do muỗi đốt kết nối qua cổng USB](https://shkspr.mobi/blog/2023/12/usb-c-cures-mosquito-bites/)

Trên thị trường gần đây xuất hiện một phụ kiện nhỏ kết nối qua cổng USB độc đáo, được thiết kế để hỗ trợ giảm ngứa hiệu quả sau khi bị muỗi đốt.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121911.webp)

Thiết bị sử dụng nguồn điện trực tiếp từ cổng USB-C của điện thoại thông minh, người dùng có thể điều chỉnh mức nhiệt độ thông qua ứng dụng di động đi kèm.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121912.webp)

Khi đầu thiết bị ấm lên, người dùng chỉ cần áp đầu nhiệt vào vị trí vết muỗi đốt giống như một liệu pháp chườm nóng giúp giảm nhanh cảm giác ngứa ngáy.

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023121910.webp)

Mặc dù có cấu trúc rất đơn giản, thiết bị này hiện đang được bán trên trang thương mại điện tử Amazon với mức giá lên tới 30 Bảng Anh (khoảng 270 Nhân dân tệ).

2、[Ý tưởng phát triển dòng máy bay hành khách siêu thanh giảm thiểu tiếng ồn](https://techxplore.com/news/2024-01-nasa-lockheed-martin-reveal-quiet.html)

Hiện nay trên thế giới không có các chuyến bay thương mại sử dụng máy bay siêu thanh do tiếng ồn cực lớn sinh ra khi máy bay vượt bức tường âm thanh (hiện tượng sonic boom) gây ảnh hưởng nghiêm trọng đến đời sống người dân khu vực đường bay.

Cơ quan Hàng không Vũ trụ Mỹ (NASA) đang phối hợp phát triển dòng máy bay siêu thanh thế hệ mới nhằm giảm thiểu tiếng ồn này, và hiện đã chế tạo thành công mô hình thử nghiệm.

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011704.webp)

Mẫu máy bay có chiều dài khoảng 30 mét, nổi bật với thiết kế phần mũi thon dài dạng hình nón chiếm tới gần 1/3 tổng chiều dài thân máy. Cấu trúc đặc biệt này được kỳ vọng sẽ triệt tiêu các sóng xung kích gây ra tiếng ồn cực lớn.

Tuy nhiên do thiết kế mũi quá dài nên khoang lái của phi công bị đẩy về vị trí giữa thân máy bay. Thiết kế khí động học này tuy giúp giảm tiếng ồn nhưng cũng làm giảm đáng kể không gian chứa hành khách.

3、[Thiết kế tuabin gió một cánh độc đáo](https://newatlas.com/energy/touchwind-floating-wind-turbine/)

Các dòng máy phát điện gió truyền thống thường được thiết kế với cấu trúc 3 cánh quạt lớn.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091702.webp)

Một công ty của Hà Lan mới đây đã giới thiệu thiết kế tuabin gió độc đáo chỉ sử dụng duy nhất một cánh quạt.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091703.webp)

Hệ thống tuabin được lắp đặt trên một phao nổi kết nối với khối neo nặng dưới đáy biển bằng xích sắt cố định.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091704.webp)

Nhờ cơ chế phao nổi, góc nghiêng của toàn bộ tuabin so với mặt biển có thể tự động điều chỉnh linh hoạt theo hướng gió và cường độ gió thực tế.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091705.webp)

Ưu điểm cốt lõi của giải pháp này là giúp tiết kiệm đáng kể chi phí sản xuất và thi công lắp đặt ngoài khơi. Dự án hiện đang trong giai đoạn thử nghiệm hiệu năng trước khi đưa vào sản xuất thương mại quy mô lớn.

4、[Hệ thống tự động thu hồi xe tự lái khi chủ xe chậm trả nợ](https://www.thedrive.com/news/future-fords-could-repossess-themselves-and-drive-away-if-you-miss-payments)

Lập trình viên và chủ xe khi vay mua xe trả góp cần chú ý: Ford đã đăng ký bằng sáng chế độc đáo cho phép xe tự động vô hiệu hóa các chức năng hoặc tự lái về đại lý thu hồi nợ nếu chủ xe trễ hạn thanh toán.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101811.webp)

Khi đến hạn thanh toán, hệ thống trên xe sẽ phát đi nhiều cảnh báo yêu cầu chủ xe thanh toán. Nếu chủ xe tiếp tục phớt lờ, xe sẽ tự động vô hiệu hóa dần các tính năng tiện ích như điều hòa, định vị GPS, điều khiển cửa kính...

Mỗi khi chủ xe bước vào trong cabin, hệ thống sẽ phát âm thanh nhắc nhở trả nợ liên tục.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101812.webp)

Trong trường hợp chủ xe vẫn kiên quyết không thanh toán, bằng sáng chế mô tả một giải pháp thu hồi tài sản triệt để: xe sẽ kích hoạt tính năng tự lái để tự động di chuyển về bãi đậu xe của công ty thu hồi nợ hoặc đại lý của Ford.

## Bài viết

1\. [Tìm hiểu nội dung phản hồi của OpenAI đối với đơn kiện của Elon Musk](https://finance.sina.com.cn/stock/usstock/c/2024-03-06/doc-inamkuik5589602.shtml)（Tiếng Trung）

Tỷ phú Elon Musk [đã đệ đơn kiện OpenAI](https://finance.sina.cn/2024-03-01/detail-inakvvhe8160978.d.html) với cáo buộc công ty vi phạm cam kết phát triển nguồn mở ban đầu để trở thành một công ty con tìm kiếm lợi nhuận cho tập đoàn Microsoft.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030708.webp)

Bài viết chia sẻ bản dịch tiếng Trung từ [bài viết phản hồi chính thức của OpenAI](https://openai.com/blog/openai-elon-musk) hé lộ nhiều thông tin nội bộ. Phía OpenAI lập luận rằng việc phát triển AI đòi hỏi nguồn tài chính khổng lồ buộc họ phải thành lập pháp nhân thương mại, và khẳng định Elon Musk hoàn toàn biết rõ và từng ủng hộ định hướng này thời kỳ đầu.

2\. [Thảo luận về triển vọng thay thế công cụ tìm kiếm truyền thống của ứng dụng Perplexity AI](https://wallstreetcn.com/articles/3709779)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030607.webp)

CEO Nvidia Jensen Huang chia sẻ ông thường xuyên sử dụng công cụ AI Perplexity cho nhu cầu tìm kiếm thông tin hàng ngày. Bài viết giới thiệu chi tiết về mô hình công cụ tìm kiếm hội thoại độc đáo này.

3\. [Suy ngẫm sau 15 năm làm nghề: Lập trình vẫn là một công việc đầy thử thách](https://mp.weixin.qq.com/s/B7Z0ROkiBqqxVKkLNR9BxQ)（Tiếng Trung）

Bài viết tổng hợp 8 bài học kinh nghiệm sâu sắc đúc kết sau 15 năm làm việc trong ngành phát triển phần mềm của một chuyên gia công nghệ tại tập đoàn Tencent.

4\. [Chia sẻ về nguồn thu nhập thực tế từ hoạt động tài trợ cho các dự án mã nguồn mở quy mô lớn](https://juejin.cn/post/7341593721100451880)（Tiếng Trung）

Tác giả chia sẻ câu chuyện thực tế khi tích hợp mã QR nhận tiền tài trợ vào dự án mã nguồn mở có hơn 1 triệu lượt cài đặt của mình, kết quả chỉ mang lại nguồn thu nhập ít ỏi 330 Nhân dân tệ sau một năm. (Đóng góp của [@xxxily](https://github.com/ruanyf/weekly/issues/4092))

5\. [Giới thiệu thành phần điều khiển Switch mặc định mới trong HTML](https://webkit.org/blog/15054/an-html-switch-control/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024022915.webp)

Phiên bản trình duyệt Safari 17.4 giới thiệu thành phần điều khiển biểu mẫu "switch" (nút gạt) mặc định mới, giúp mang giao diện nút gạt đặc trưng trên iOS lên trang web một cách dễ dàng.

6\. [Phân tích nguyên nhân chuyển đổi từ framework Electron sang Tauri trong phát triển ứng dụng desktop](https://aptabase.com/blog/why-chose-to-build-on-tauri-instead-electron)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111608.webp)

Tác giả chia sẻ kinh nghiệm thực tế khi quyết định chuyển dịch nền tảng phát triển ứng dụng desktop đa nền tảng từ Electron sang framework Tauri hiện đại hơn.

7\. [Tối ưu hóa khả năng ngắt dòng văn bản bằng thuộc tính CSS text-wrap](https://clagnut.com/blog/2424)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100516.webp)

Việc ngắt dòng tự động của các đoạn văn bản dài có thể được tối ưu hóa bằng thuộc tính CSS `text-wrap`. Bài viết thảo luận cách ứng dụng thuộc tính này để trình bày các tiêu đề bài viết đẹp mắt hơn.

8\. [Hệ thống máy tính đồng bộ và lấy thông tin thời gian chuẩn từ đâu?](https://dotat.at/@/2023-05-26-whence-time.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100607.webp)

Các thiết bị máy tính thường đồng bộ thời gian từ các máy chủ NTP (Network Time Protocol), vậy các máy chủ NTP lấy mốc thời gian chuẩn xác nhất từ đâu? Bài viết giới thiệu chi tiết về cách thức con người định vị và đo lường thời gian.

9\. [Hướng dẫn phương pháp kiểm thử trình duyệt Safari trên hệ điều hành Windows](https://james.darpinian.com/blog/safari-on-windows)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100808.webp)

Do Apple đã dừng hỗ trợ Safari cho Windows từ lâu, bài viết chia sẻ giải pháp kỹ thuật giúp lập trình viên chạy thử nghiệm và gỡ lỗi hiển thị web trên trình duyệt Safari trực tiếp từ hệ điều hành Windows.

## 工具

1\. [Ente (Giải pháp lưu trữ ảnh mã nguồn mở bảo mật)](https://github.com/ente-io/ente)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030301.webp)

Dịch vụ lưu trữ và quản lý ảnh cá nhân thay thế cho Google Photos và iCloud Photos, hỗ trợ mã hóa đầu cuối (end-to-end encryption) an toàn, dự án vừa chính thức được chuyển đổi sang mã nguồn mở.

Bên cạnh đó, bạn cũng có thể tham khảo hai dự án quản lý ảnh tự vận hành chất lượng khác là [Immich](https://immich.app/) và [PhotoPrism](https://github.com/photoprism/photoprism).

2\. [Earthly](https://earthly.dev/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072502.webp)

Một framework xây dựng CI/CD mã nguồn mở mạnh mẽ, cho phép lập trình viên tự thiết lập và chạy các tác vụ build tự động trên máy cục bộ.

3\. [Vikunja (Ứng dụng quản lý công việc tối giản)](https://vikunja.io/)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023120707.webp)

Ứng dụng quản lý danh sách công việc cần làm (to-do list) mã nguồn mở, hỗ trợ nhiều giao diện hiển thị trực quan, tương thích tốt trên môi trường web, desktop hoặc tự triển khai trên server riêng.

4\. [Công cụ định dạng và làm đẹp văn bản tiếng Nhật](https://miusuncle.github.io/japen/)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030202.webp)

Dịch vụ trực tuyến giúp tạo định dạng văn bản tiếng Nhật đẹp mắt, hỗ trợ hiển thị dạng dòng dọc/ngang truyền thống, tự động thêm phiên âm furigana, tùy biến phông chữ, chủ đề sáng/tối... (Đóng góp của [@miusuncle](https://github.com/ruanyf/weekly/issues/4080))

5\. [Web-Check (Công cụ phân tích cấu trúc trang web trọn gói)](https://github.com/Lissy93/web-check)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030401.webp)

Dự án mã nguồn mở hỗ trợ thu thập và phân tích nhanh các thông tin kỹ thuật của một trang web như địa chỉ IP, chứng chỉ SSL, bản ghi DNS, Cookie, vị trí máy chủ, hiệu năng tải trang... Trải nghiệm bản dùng thử [Demo tại đây](https://web-check.xyz/). (Đóng góp của [@WFANG12719](https://github.com/ruanyf/weekly/issues/4086))

6\. [ImageTools](https://ai-image.tools/home)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030501.webp)

Dịch vụ trực tuyến hỗ trợ xóa nền ảnh chân dung nhanh chóng bằng công nghệ AI. (Đóng góp của [@handsometong](https://github.com/ruanyf/weekly/issues/4087))

7\. [zz-plan](https://zz-plan.com/)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030502.webp)

Công cụ thiết kế sơ đồ Gantt trực tuyến giúp quản lý tiến độ dự án. (Đóng góp của [@lizhichao](https://github.com/ruanyf/weekly/issues/4088))

8\. [Windows in container](https://github.com/dockur/windows)

Dự án Docker hỗ trợ chạy hệ điều hành Windows trực tiếp trong container, hỗ trợ các phiên bản Windows 7/10/11 đi kèm cơ chế tự động kích hoạt bản quyền và kết nối qua Remote Desktop. (Đóng góp của [@wrenashe](https://github.com/ruanyf/weekly/issues/4091))

9\. [Rsdoctor](https://github.com/web-infra-dev/rsdoctor)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030601.webp)

Công cụ phân tích hiệu năng đóng gói code dành cho các bộ build Rspack và Webpack, hỗ trợ hiển thị trực quan mối quan hệ phụ thuộc giữa các module và phân tích các thay đổi mã nguồn trong quá trình build. (Đóng góp của [@easy1090](https://github.com/ruanyf/weekly/issues/4095))

10\. [Photo Relay](https://github.com/zobor/photo-relay)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030503.webp)

Dịch vụ trực tuyến hỗ trợ thiết kế nhanh các ảnh bìa, poster truyền thông. Trải nghiệm bản dùng thử [Demo tại đây](https://www.duelpeak.com/pages/poster). (Đóng góp của [@zobor](https://github.com/ruanyf/weekly/issues/4094))

11\. [opfs-tools](https://github.com/hughfenghen/opfs-tools)

Thư viện JavaScript bao bọc lớp API của hệ thống tệp tin Origin Private File System (OPFS) trên trình duyệt, giúp thao tác với file dễ dàng hơn. (Đóng góp của [@hughfenghen](https://github.com/ruanyf/weekly/issues/4099))

12\. [ast-grep VSCode](https://marketplace.visualstudio.com/items?itemName=ast-grep.ast-grep-vscode)

Tiện ích mở rộng trên VSCode hỗ trợ tìm kiếm và thay thế mã nguồn thông minh dựa trên cấu trúc cây cú pháp AST thay vì regex thông thường. (Đóng góp của [@HerringtonDarkholme](https://github.com/ruanyf/weekly/issues/4100))

## 掘金动手实验室

Để làm chủ một công nghệ mới, việc thực hành trực tiếp đóng vai trò then chốt, tuy nhiên các cơ hội thực hành thực tế trong công việc hàng ngày của lập trình viên thường tương đối hạn chế.

Tuần này có một tin vui dành cho cộng đồng: **Phòng thí nghiệm thực hành Cát Thổ Quyết Kim (JUEJIN Code Lab)** đã chính thức được ra mắt!

Đây là chuỗi hoạt động trải nghiệm thực hành công nghệ mới, hướng tới việc **chuyển hóa lý thuyết khoa học thành các ứng dụng thực tế** và tạo không gian giao lưu kết nối kỹ thuật cho các kỹ sư.

Hoạt động do cộng đồng công nghệ Quyết Kim tổ chức phối hợp cùng nhiều nhà cung cấp nền tảng lớn, bao quát nhiều lĩnh vực công nghệ đa dạng đảm bảo mang lại giá trị thiết thực cho người tham gia.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030707.webp)

Chủ đề của số đầu tiên tập trung vào lĩnh vực AI nóng nhất hiện nay, đồng tổ chức bởi cộng đồng Quyết Kim và nền tảng phát triển chatbot Coze (coze.cn). **Hoạt động sẽ giúp bạn biến các ý tưởng sáng tạo thành sản phẩm thực tế thông qua các bài thực hành trực quan.**

Chương trình được tổ chức trực tiếp tại văn phòng của ByteDance tại hai khu vực: [Bắc Kinh vào ngày 16 tháng 3](https://www.bagevent.com/event/8791420?bag_track=ryf) và [Thâm Quyến vào ngày 30 tháng 3](https://www.bagevent.com/event/8796081?bag_track=ryf).

Các học viên tham gia trực tiếp ngoài việc được trải nghiệm quy trình phát triển ứng dụng AI còn có cơ hội nhận được các phần quà lưu niệm giá trị từ ban tổ chức, đi kèm cơ hội xuất hiện trên trang chủ của Coze, quyền trải nghiệm sớm các API nội bộ và tham gia các buổi phỏng vấn chuyên sâu.

Độc giả quan tâm có thể [truy cập đường link đăng ký](https://www.bagevent.com/event/8791420?bag_track=ryf) hoặc quét mã QR trên poster để đăng ký tham gia chương trình thực hành phát triển AI.

## 资源

1\. [Dịch vụ dịch thuật song ngữ các tài liệu nghiên cứu khoa học arXiv](https://yiyibooks.cn/)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030204.webp)

Trang web hỗ trợ tìm kiếm và tải lên các tài liệu nghiên cứu arXiv (hiện tại mới hỗ trợ định dạng HTML), hệ thống sẽ tự động dịch thuật và hiển thị nội dung song ngữ giúp người đọc dễ dàng đối chiếu. (Đóng góp của [@yiyibooks](https://github.com/ruanyf/weekly/issues/4083))

2\. [Kinh Mặc (Thư viện văn hóa cổ điển Trung Quốc)](https://github.com/hefengbao/jingmo)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030203.webp)

Ứng dụng Android mã nguồn mở đóng vai trò như một thư viện bỏ túi lưu trữ các tác phẩm thơ ca cổ điển, thành ngữ, câu đố... (Đóng góp của [@hefengbao](https://github.com/ruanyf/weekly/issues/4081))

3\. [OpenMoji (Thư viện Emoji mã nguồn mở)](https://github.com/hfg-gmuend/openmoji)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023091302.webp)

Dự án cộng đồng thu thập các thiết kế Emoji mã nguồn mở, cho phép các nhà thiết kế tự do đóng góp các thiết kế cá nhân.

4\. [Docker Compose Examples](https://github.com/Haxxnet/Compose-Examples)

Kho lưu trữ tổng hợp các file cấu hình Docker Compose mẫu cho nhiều dịch vụ phổ biến giúp lập trình viên nhanh chóng triển khai ứng dụng.

5\. [Tài liệu nhập môn ngôn ngữ lập trình hợp ngữ x86-64](http://www.egr.unlv.edu/~ed/x86.html)

![](https://cdn.beekka.com/blogimg/asset/202312/bg2023122601.webp)

Cuốn sách giáo trình tiếng Anh giới thiệu các kiến thức cơ bản về hợp ngữ, lấy ví dụ thực hành trên hệ điều hành Ubuntu.

## 图片

1\. [Nghệ thuật sắp đặt từ lá cây rụng](https://kottke.org/23/09/artistic-leaf-raking)

Một nghệ sĩ châu Âu đã thu gom và sắp xếp các lá cây rụng trong công viên thành nhiều hình khối nghệ thuật độc đáo, mang lại không gian vui tươi cho công viên.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092809.webp)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092810.webp)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092811.webp)

2\. [Giai thoại về tựa game cổ điển The Last Express](https://www.filfre.net/2023/10/the-last-express/)

"The Last Express" là tựa game phiêu lưu trinh thám nổi tiếng được phát hành vào cuối thế kỷ trước.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100801.webp)

Bối cảnh game xoay quanh câu chuyện của một hành khách người Mỹ bước lên chuyến tàu cuối cùng của tuyến đường sắt "Phương Đông nhanh hành" (Orient Express) kết nối Paris và Istanbul vào năm 1914.

Toàn bộ diễn biến trò chơi đều xảy ra bên trong các khoang tàu. Dưới đây là hình ảnh thực tế của khoang tàu Orient Express trong lịch sử.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100802.webp)

Các nhà thiết kế game đã dựa trên bức ảnh tư liệu này để dựng mô hình 3D, tái hiện sinh động không gian nội thất khoang tàu thời kỳ đó trong trò chơi.

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100803.webp)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100804.webp)

## ✍️ Bài đọc thêm

### Thảo luận về hiện tượng những người có tư duy sáo rỗng giống như các mô hình AI

Nhiều người thường nhận xét các mô hình AI như ChatGPT ngày càng giao tiếp giống con người, nhưng tôi lại nhận thấy một khía cạnh ngược lại: **có không ít người đang tư duy và phát ngôn rất giống ChatGPT**, đặc biệt là trong giới học thuật.

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030801.webp)

Mô hình ChatGPT thực chất hoàn toàn không hiểu ý nghĩa của các tài liệu huấn luyện, nhưng nó sở hữu khả năng tổng hợp thông tin cực nhanh để đưa ra câu trả lời có cấu trúc ngữ pháp rất hợp lý. Khả năng bắt chước này tạo nên những câu trả lời nghe qua vô cùng thuyết phục, giống như ý kiến của một chuyên gia sâu sắc về lĩnh vực đó.

Nhiều học giả trong giới nghiên cứu cũng đang làm việc theo cách tương tự: họ rất thông minh, nhanh chóng nắm bắt các lý thuyết và thuật ngữ chuyên ngành để viết nên những bài phân tích nghe qua rất học thuật.

Tuy nhiên, nếu bạn đặt các câu hỏi đi sâu vào bản chất vấn đề, bạn sẽ nhanh chóng nhận ra mức độ hiểu biết thực tế của họ rất hạn chế. Mọi phân tích dài dòng chỉ nằm ở bề nổi sáo rỗng thiếu chiều sâu. Đó thực chất chỉ là hành vi sao chép bắt chước kiến thức chứ không phải tư duy sáng tạo thực thụ, viết ra nhằm mục đích tạo cảm giác thông thái giả tạo cho người đọc.

Many người ở các ngành khoa học xã hội - những lĩnh vực ít đòi hỏi các hoạt động kiểm chứng thực nghiệm hay đối chiếu dữ liệu thực tế, hoạt động như một phiên bản người thật của ChatGPT. Lượng văn bản sáo rỗng họ sản xuất ra càng nhiều càng gây nguy hại cho tri thức xã hội.

Dấu hiệu nhận biết nhóm người này khá rõ ràng: họ thường xuyên sử dụng các thuật ngữ rất chung chung sáo rỗng, các biệt ngữ chuyên ngành phức tạp nhưng nội dung bài viết lại thiếu hụt các số liệu thực tế, các ví dụ minh họa hời hợt ngẫu nhiên, không thể hiện góc nhìn cá nhân rõ ràng và né tránh việc bày tỏ quan điểm phản biện trực diện.

Trải nghiệm này giúp tôi nhận ra rằng khi mình không thể hiểu một bài phát biểu nào đó, lý do rất có thể không phải vì kiến thức của mình kém, mà do chính người nói cũng đang mơ hồ về chủ đề họ đang nói và chỉ đang phát ngôn sáo rỗng giống như một cỗ máy AI.

Tôi gọi đây là kỹ năng "thổi bong bóng" - khả năng phát biểu dài dòng thuyết phục dù hoàn toàn rỗng tuếch bên trong. Đây lại là kỹ năng thường thấy ở nhiều nhà quản lý cấp cao trong các trường đại học.

Sự xuất hiện của ChatGPT chứng minh cho chúng ta thấy việc tạo ra một chuỗi văn bản nghe qua có vẻ logic từ một lượng lớn tài liệu mà không cần thực sự hiểu bản chất là điều hoàn toàn khả thi. Điều này phản ánh xu hướng không lành mạnh trong xã hội: con người nên bước ra ngoài thực tế, quan sát thế giới và thẳng thắn bày tỏ cảm nhận chân thực của cá nhân.

Trải nghiệm này giúp tôi xác định rõ hơn sở thích cá nhân: tôi muốn làm việc cạnh những con người có tư duy độc lập sáng tạo thay vì những cỗ máy nói sáo rỗng.

## Lịch sử tuần này

- 2023年（第 245 期）：[Góc nhìn kiến trúc: Nhận định về việc các tòa nhà chọc trời cao tầng đang đi ngược lại tự nhiên](https://www.ruanyifeng.com/blog/2023/03/weekly-issue-245.html)
- 2022年（第 195 期）：[Tư duy phát triển: Bạn đã từng thực hiện dự án cá nhân nào hoàn toàn vì sở thích chưa?](https://www.ruanyifeng.com/blog/2022/02/weekly-issue-195.html)
- 2021年（第 145 期）：[Kinh tế vĩ mô: Thảo luận về các giải pháp duy trì tăng trưởng kinh tế khi người dân hạn chế ra ngoài](https://www.ruanyifeng.com/blog/2021/02/weekly-issue-145.html)
- 2020年（第 95 期）：[Quản trị nhân sự: Xu hướng làm việc từ xa giúp doanh nghiệp phát hiện các vị trí nhân sự dư thừa](https://www.ruanyifeng.com/blog/2020/02/weekly-issue-95.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
