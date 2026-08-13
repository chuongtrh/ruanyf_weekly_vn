# Bản tin chia sẻ công nghệ (Số 264): Bài học từ Elasticsearch

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3222) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072501.webp)

Tại khu vực cửa sông Trường Giang thuộc quận Bảo Sơn, Thượng Hải, chính quyền địa phương đã cho xây dựng tháp quan sát cảnh quan "Tháp Trường滩" với đường kính 25,7 mét và chiều cao lên tới 180 mét. Điều đặc biệt là tháp quan sát này thực chất là hệ thống tháp thông gió thoát khí của dự án đường hầm vượt sông Trường Giang, được khoác thêm lớp áo kính cường lực bên ngoài kết hợp bố trí đài quan sát du lịch và nhà hàng xoay ở phía trên. (Nguồn: [Shbsq](https://www.shbsq.gov.cn/shbs/rdtj/20221223/354447.html))

## Elasticsearch 的启示

Sự kiện Red Hat đơn phương thay đổi chính sách mã nguồn vào tháng trước đã chứng minh mô hình kinh doanh dựa vào dịch vụ hỗ trợ kỹ thuật (Customer Support Model) của các dự án nguồn mở đã đi vào ngõ cụt, tôi đã chia sẻ chi tiết nhận định này của mình ở [số tuần trước](http://www.ruanyifeng.com/blog/2023/07/weekly-issue-263.html).

Vậy câu hỏi đặt ra là: làm thế nào để một dự án phần mềm mã nguồn mở có thể tìm kiếm được nguồn thu bền vững? **Khi cả việc bán bản quyền phần mềm lẫn bán dịch vụ hỗ trợ kỹ thuật đều không khả thi, hướng đi nào sẽ dành cho các nhà phát triển?**

Tôi đã suy nghĩ rất nhiều về bài toán kinh doanh này, bởi nó có liên quan mật thiết đến lộ trình nghề nghiệp của lập trình viên và sự phát triển chung của toàn ngành phần mềm.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072304.webp)

Nhận định hiện tại của tôi là: **chỉ còn duy nhất một mô hình kinh doanh nguồn mở là thực sự khả thi** giúp doanh nghiệp có thể thương mại hóa sản phẩm thành công, đó chính là mô hình mà Elasticsearch đang áp dụng.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072305.webp)

Elasticsearch là công cụ tìm kiếm và phân tích dữ liệu vô cùng nổi tiếng, chiếm thị phần áp đảo trên thị trường và đứng sau hệ thống tìm kiếm của hàng vạn website lớn nhỏ hiện nay.

Vào năm 2004, lập trình viên người Israel Shay Banon vì muốn giúp vợ dễ dàng tra cứu nhanh các công thức nấu ăn trong bếp đã tự tay viết một công cụ tìm kiếm dữ liệu tối giản, đó chính là tiền thân của Elasticsearch sau này.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072306.webp)

Thời kỳ đầu, Elasticsearch được phân phối dưới giấy phép Apache cực kỳ cởi mở, cho phép bất kỳ cá nhân hay tổ chức nào cũng được tự do sao chép, sửa đổi và thương mại hóa mã nguồn mà hầu như không gặp bất kỳ rào cản pháp lý nào.

Sau đó, khi nhận được các khoản đầu tư mạo hiểm và thành lập doanh nghiệp chính thức, Shay Banon bắt buộc phải tuyển dụng thêm nhân sự và tìm kiếm nguồn doanh thu ổn định để duy trì bộ máy hoạt động.

**Giải pháp kinh doanh anh lựa chọn lúc đó là cung cấp dịch vụ đám mây (Cloud Service Model)**: Khách hàng không cần tốn công sức tự thiết lập hạ tầng máy chủ và cài đặt phần mềm nữa, Elasticsearch đã thiết lập sẵn cụm máy chủ tìm kiếm trên mây, khách hàng chỉ cần trả tiền dịch vụ là có thể nhúng tính năng tìm kiếm vào website của mình sử dụng ngay.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072307.webp)

Thế nhưng, anh không thể ngờ rằng mô hình kinh doanh dịch vụ đám mây nguồn mở này lại ẩn chứa rủi ro chí mạng. Nguyên nhân do mã nguồn của phần mềm là mở hoàn toàn và không có tính độc quyền, khi phần mềm của bạn quá phổ biến, các tập đoàn đám mây khổng lồ khác hoàn toàn có thể lấy chính mã nguồn đó để tự xây dựng dịch vụ đám mây của riêng họ với mức giá rẻ hơn để cướp đi thị phần của chính tác giả gốc.

Và đối thủ cạnh tranh trực tiếp lớn nhất mà Elasticsearch đụng độ chính là Amazon Web Services (AWS) – gã khổng lồ đang thống trị thị trường điện toán đám mây toàn cầu.

Amazon đã không tốn một đồng chi phí bản quyền nào để lấy toàn bộ mã nguồn của Elasticsearch về tự cấu hình dịch vụ tìm kiếm và bán cho các khách hàng của mình, nhanh chóng đẩy doanh nghiệp của tác giả gốc vào tình thế cạn kiệt nguồn thu.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072308.webp)

Đứng trước nguy cơ phá sản, ban lãnh đạo Elasticsearch đã đưa ra một quyết định mang tính lịch sử đầy tranh cãi:

Vào năm 2021, Shay Banon tuyên bố từ bỏ giấy phép Apache cởi mở để chuyển sang một giấy phép mới ràng buộc hơn: mã nguồn của Elasticsearch vẫn được mở để cộng đồng đọc hiểu, nhưng nghiêm cấm các nhà cung cấp bên thứ ba sử dụng phần mềm để kinh doanh dịch vụ điện toán đám mây thương mại, trừ phi nhà cung cấp đó sẵn sàng công bố toàn bộ mã nguồn hệ thống máy chủ dịch vụ của họ (không chỉ riêng phần công cụ tìm kiếm).

Yêu cầu này rõ ràng là điều không thể chấp nhận đối với một tập đoàn lớn như Amazon. Giấy phép mới đã chặn đứng hoàn toàn việc Amazon, Google hay Microsoft tiếp tục sử dụng miễn phí các bản cập nhật mới của Elasticsearch để kinh doanh kiếm lời.

Để đáp trả đòn pháp lý này, Amazon đã quyết định phân nhánh (fork) mã nguồn phiên bản Apache cũ của Elasticsearch để tự mình phát triển một dự án độc lập mang tên [OpenSearch](https://aws.amazon.com/cn/opensearch-service/) dưới giấy phép Apache mở hoàn toàn để lôi kéo cộng đồng sử dụng miễn phí. Hai bên chính thức bước vào cuộc chiến cạnh tranh gay gắt.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072601.webp)

Dù kết quả cuối cùng của cuộc đối đầu này chưa ngã ngũ, quyết định đổi giấy phép đã giúp Elasticsearch bảo toàn được nguồn thu cốt lõi của mình. Các doanh nghiệp muốn sử dụng dịch vụ tìm kiếm đám mây chính chủ bắt buộc phải mua gói dịch vụ trực tiếp từ công ty của tác giả gốc.

Tôi tin rằng **đây chính là mô hình kinh doanh khả thi duy nhất hiện nay dành cho các phần mềm nguồn mở lớn**.

Giới phân tích gọi đây là **“Mô hình kinh doanh lõi nguồn mở”** (Open-Core Business Model): Phần lõi cốt lõi của phần mềm được mở nguồn hoàn toàn miễn phí để xây dựng cộng đồng người dùng và danh tiếng thương hiệu; tuy nhiên các tính năng nâng cao dành cho doanh nghiệp lớn, các công cụ quản lý đi kèm hoặc dịch vụ đám mây sẽ được giữ kín dạng mã nguồn đóng hoặc ràng buộc bản quyền thương mại để thu phí dịch vụ.

Bên cạnh Elasticsearch, một tên tuổi lớn khác cũng đang gặt hái thành công lớn nhờ áp dụng mô hình này là cơ sở dữ liệu MongoDB.

**Lời khuyên của tôi dành cho các startup công nghệ định hướng nguồn mở là hãy áp dụng mô hình Open-Core này ngay từ đầu**. Bạn nên duy trì song song hai phiên bản độc lập: Một phiên bản Cộng đồng (Community Edition) mở nguồn hoàn toàn miễn phí để thu hút người dùng trải nghiệm và xây dựng uy tín; và một phiên bản Doanh nghiệp (Enterprise Edition) tích hợp thêm các tính năng bảo mật chuyên sâu, khả năng chịu tải lớn đi kèm gói hỗ trợ kỹ thuật độc quyền để thu phí thương mại.

## 科技动态

1、[Mỹ thử nghiệm kích hoạt trạng thái đông ngủ ở động vật bằng sóng siêu âm](https://www.science.org/content/article/ultrasound-brain-pulses-put-mice-hibernation-state)

Một nhóm nghiên cứu tại Đại học Washington mới đây đã công bố phát hiện khoa học độc đáo: khi sử dụng các xung sóng siêu âm hướng thẳng vào một vùng thần kinh cụ thể trong não bộ của chuột, hệ thống sẽ kích hoạt chuột tự động rơi vào trạng thái đông眠 tạm thời (giảm thân nhiệt và làm chậm nhịp tim sinh lý):

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052901.webp)

Phát hiện này chứng minh trạng thái đông ngủ hoàn toàn có thể được kích hoạt chủ động bằng tác nhân vật lý ngoài. Các nhà khoa học hy vọng nghiên cứu này có thể ứng dụng trên cơ thể con người trong tương lai, giúp các phi hành gia rơi vào trạng thái đông ngủ để tiết kiệm năng lượng và thực phẩm trong các hành trình du hành vũ trụ dài ngày.

Tuy nhiên, một số nhà khoa học độc lập bày tỏ sự hoài nghi về bản chất của hiện tượng: họ cho rằng sóng siêu âm mang năng lượng cao chỉ đơn thuần là kích thích các thụ thể cảm biến nhiệt độ trong não, đánh lừa não bộ rằng nhiệt độ môi trường đang tăng cao, khiến cơ thể tự động phản ứng hạ nhiệt và rơi vào trạng thái lờ đờ chứ không phải là trạng thái đông ngủ sinh học thực thụ.

2、[Mỹ công bố nhãn hiệu chứng nhận an toàn thông tin cho thiết bị thông minh](https://www.theverge.com/2023/7/18/23798153/fcc-cyber-trust-mark-biden-security)

Chính phủ Mỹ vừa công bố kế hoạch triển khai nhãn hiệu chứng nhận an toàn bảo mật thông tin mang tên “US Cyber Trust Mark” (nhãn dưới) dành riêng cho các dòng thiết bị gia dụng thông minh kết nối Internet bán ra tại thị trường nước này:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072401.webp)

Nhãn chứng nhận sẽ được in kèm theo một mã QR độc lập. Người dùng khi mua sắm có thể quét mã QR để truy cập nhanh vào trang web của chính phủ hiển thị chi tiết các thông số bảo mật, tần suất cập nhật phần mềm và mức độ mã hóa dữ liệu của thiết bị:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072402.webp)

Trong giai đoạn đầu, việc dán nhãn được thực hiện trên tinh thần tự nguyện đăng ký của các hãng sản xuất. Tuy nhiên giới phân tích lo ngại tiêu chuẩn này có thể sớm trở thành quy định bắt buộc, vô tình tạo nên một rào cản kỹ thuật thương mại phi thuế quan đối với các thiết bị thông minh nhập khẩu từ các quốc gia khác.

3、[Ứng dụng thiết bị hộp đen ghi nhận thông tin quy trình phẫu thuật tại bệnh viện](https://www.wsj.com/amp/articles/surgery-technology-data-black-boxes-a8bc483b)

Một doanh nghiệp y tế của Canada đã nghiên cứu và đưa vào ứng dụng dòng sản phẩm "Hộp đen bệnh viện" (Hospital Black Box) lắp đặt trong các phòng mổ, hoạt động tương tự như thiết bị hộp đen ghi nhận hành trình của máy bay:

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032102.webp)

Thiết bị sẽ tự động ghi lại toàn bộ diễn biến cuộc phẫu thuật bao gồm hình ảnh camera giám sát, âm thanh trao đổi của ê-kíp mổ và các thông số hoạt động của các thiết bị y tế đi kèm.

Dữ liệu hộp đen sẽ được các hội đồng chuyên môn phân tích sau ca mổ để đánh giá, phát hiện các lỗi thao tác y khoa ngẫu nhiên nhằm nâng cao mức độ an toàn cho bệnh nhân và phục vụ công tác đào tạo bác sĩ trẻ. Một số bác sĩ bày tỏ sự e ngại vì cho rằng thiết bị này hoạt động như một công cụ giám sát hành vi của nhân viên y tế và có thể làm gia tăng các vụ kiện cáo y tế. Để giải quyết mối lo ngại này, phần mềm tự động mã hóa ẩn danh toàn bộ khuôn mặt và giọng nói của nhân sự trước khi lưu trữ dữ liệu.

4、[Trung Quốc khánh thành kính thiên văn vô tuyến quan sát mặt trời lớn nhất thế giới](http://www.stdaily.com/index/kejixinwen/202305/ae99861e29034bd59c22a768234af466.shtml)

Hệ thống kính thiên văn vô tuyến chuyên biệt phục vụ quan sát hoạt động của Mặt Trời có quy mô lớn nhất thế giới đã chính thức được đưa vào hoạt động tại huyện Đạo Thành, châu tự trị Cam Tư, Tứ Xuyên:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072701.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072702.webp)

Hệ thống bao gồm 313 đĩa anten parabol lớn được bố trí xếp thành một vòng tròn khổng lồ có đường kính lên tới 1 km. Ngay tại tâm của vòng tròn là tháp hiệu chuẩn trung tâm cao 100 mét làm nhiệm vụ thu phát tín hiệu phối hợp điều phối toàn bộ các đĩa anten:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072703.webp)

Mỗi đĩa anten có đường kính 6 mét, được trang bị hệ thống động cơ tự động xoay chuyển hướng liên tục bám sát theo đường đi của Mặt Trời trong ngày để thu thập các bức xạ điện từ:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072704.webp)

Bằng việc kết hợp đồng bộ dữ liệu thu phát từ 313 đĩa anten, hệ thống máy tính sẽ giả lập tạo ra một đĩa kính thiên văn ảo có đường kính khổng lồ tương đương 1 km, giúp chụp lại các bức ảnh có độ phân giải siêu cao về các đợt phun trào và bão Mặt Trời để phục vụ dự báo thời tiết vũ trụ.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072705.webp)

## Bài viết

1\. [Báo cáo rò rỉ dữ liệu bảng lương và phân bổ cổ phiếu của nhân sự tại Google](https://www.businessinsider.com/google-salaries-leaked-data-employees-engineers-sales-cloud-2023-7)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072102.webp)

Nội dung một tài liệu thống kê nội bộ của Google bị rò rỉ ra ngoài, phác họa chi tiết mức thu nhập cơ bản, các khoản thưởng dự án và giá trị cổ phiếu thưởng (RSU) của các vị trí kỹ sư phần mềm, nhân viên kinh doanh và chuyên gia đám mây của hãng trong năm qua. Số liệu chỉ ra mức thu nhập trung vị của nhân sự Google trong năm 2022 đạt con số rất cao lên tới 279.802 USD, khẳng định vị trí là một trong những doanh nghiệp có chế độ đãi ngộ kỹ sư tốt nhất thế giới.

2\. [Lập trình viên nổi tiếng Dan Abramov thông báo chính thức rời khỏi dự án React của Meta](https://www.reddit.com/r/reactjs/comments/154trk7/comment/jsrbysw/)（Tiếng Anh）

Kỹ sư lập trình giao diện nổi tiếng Dan Abramov đã đăng tải chuỗi chia sẻ trên mạng xã hội giải thích chi tiết các lý do cá nhân dẫn đến quyết định xin thôi việc tại Meta và chính thức rút khỏi đội ngũ phát triển cốt lõi của thư viện React. (Đóng góp của [@hacker0limbo](https://github.com/ruanyf/weekly/issues/3289))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072706.webp)

3\. [Hướng dẫn ứng dụng cấu trúc dữ liệu Map và WeakMap để xử lý phần tử DOM](https://www.macarthur.me/posts/maps-for-dom-nodes)（Tiếng Anh）

Cấu trúc dữ liệu `Map` và `WeakMap` được bổ sung vào ngôn ngữ JavaScript hiện đại mang lại nhiều ưu điểm lớn về hiệu năng quản lý bộ nhớ nhưng chưa được nhiều lập trình viên hiểu rõ. Bài viết đưa ra ví dụ thực tế hướng dẫn cách tận dụng `WeakMap` để liên kết dữ liệu động trực tiếp vào các nút DOM mà không lo ngại rò rỉ bộ nhớ (memory leaks).

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050602.webp)

4\. [Phân tích lựa chọn giữa hai cơ chế Kế thừa và Tổ hợp trong thiết kế OOP](https://buttondown.email/hillelwayne/archive/when-to-prefer-inheritance-to-composition/)（Tiếng Anh）

Khi cần mở rộng tính năng của lớp (class) trong lập trình hướng đối tượng, lập trình viên có hai giải pháp: Kế thừa (Inheritance) hoặc Tổ hợp (Composition). Bài viết phân tích sâu sự khác biệt về mặt kiến trúc, các ưu nhược điểm và đưa ra lời khuyên về các tình huống cụ thể nên ưu tiên áp dụng từng giải pháp.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050601.webp)

5\. [Tìm hiểu tác động của các câu lệnh rẽ nhánh CPU đến hiệu năng xử lý của code](https://johnnysswlab.com/how-branches-influence-the-performance-of-your-code-and-what-can-you-do-about-it/)（Tiếng Anh）

Bài viết phân tích sâu cơ chế hoạt động của bộ dự đoán rẽ nhánh (Branch Predictor) tích hợp trong CPU phần cứng, từ đó hướng dẫn lập trình viên các phương pháp viết câu lệnh điều kiện `if-else` tối ưu giúp CPU xử lý nhanh hơn và hạn chế tình trạng trượt dự đoán (branch misprediction).

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050610.webp)

6\. [Lý giải kiểu dữ liệu trả về của phương thức Object.keys() trong TypeScript](https://vladimirzdrazil.com/posts/object-keys-keyof-t/)（Tiếng Anh）

Bài viết kỹ thuật giải thích một chi tiết gây thắc mắc cho nhiều lập trình viên TypeScript: tại sao phương thức `Object.keys()` mặc định luôn trả về kiểu mảng chuỗi chung `string[]` thay vì kiểu dữ liệu chặt chẽ hơn là mảng các thuộc tính của đối tượng `(keyof T)[]`.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023050802.webp)

7\. [Cẩm nang hướng dẫn cài đặt nhanh hệ điều hành Linux NixOS](https://borretti.me/article/nixos-for-the-impatient)（Tiếng Anh）

NixOS là hệ điều hành Linux sở hữu cơ chế cấu hình độc đáo: toàn bộ thông tin phần mềm và thiết lập hệ thống được khai báo tập trung trong một file cấu hình duy nhất. Bài viết hướng dẫn nhanh quy trình cài đặt dành cho những người dùng muốn nhanh chóng làm quen với trải nghiệm hệ điều hành này.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051001.webp)

8\. [Hướng dẫn tự thiết lập máy chủ web chạy trực tiếp từ chiếc điện thoại Android cũ](https://androidblog.a.pinggy.io/)（Tiếng Anh）

Tác giả chia sẻ chi tiết cách thức tận dụng hiệu năng phần cứng của một chiếc điện thoại di động Android cũ, cài đặt môi trường máy chủ và chạy ứng dụng tunnel để biến nó thành một máy chủ web thực thụ phục vụ lưu trữ blog cá nhân.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051002.webp)

## 工具

1、[Aimless.js: Thư viện JavaScript hỗ trợ tạo các giá trị ngẫu nhiên đa dạng](https://github.com/ChrisCavs/aimless.js)

Một thư viện JS nhỏ gọn cung cấp hàng loạt thuật toán và phương thức hỗ trợ lập trình viên sinh nhanh các chuỗi ngẫu nhiên, số ngẫu nhiên theo phân phối đặc thù phục vụ thiết kế game hoặc chạy test dữ liệu.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052221.webp)

2、[Primo: Hệ thống quản lý nội dung CMS nguồn mở dựa trên Svelte](https://primocms.org/)

Dự án phát triển hệ thống quản trị nội dung website (CMS) nguồn mở hướng tới mục tiêu thay thế WordPress, được phát triển trên nền tảng framework Svelte của JS cho tốc độ hiển thị trang cực nhanh.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072202.webp)

3、[Link Redirect Trace: Tiện ích theo dõi lịch sử chuyển hướng liên kết](https://chrome.google.com/webstore/detail/link-redirect-trace/nnpljppamoaalgkieeciijbcccohlpoh)

Extension dành cho trình duyệt Chrome giúp các chuyên gia SEO và lập trình viên dễ dàng theo dõi và ghi lại toàn bộ lịch sử các bước chuyển hướng URL (Redirect 301, 302, Javascript Redirect) của một liên kết trước khi tới trang đích.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052510.webp)

4、[Clang.js: Thư viện hỗ trợ chạy trực tiếp mã nguồn C/C++ trên trình duyệt](https://github.com/luoxuhai/clang.js)

Dự án ứng dụng công nghệ WebAssembly giúp lập trình viên nhúng và chạy trực tiếp các đoạn mã viết bằng C/C++ ngay trong môi trường trình duyệt web mà không cần thông qua máy chủ backend. (Đóng góp của [@luoxuhai](https://github.com/ruanyf/weekly/issues/3297))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072707.webp)

5、[mess-reader: Ứng dụng đọc sách điện tử Epub trực tuyến hoạt động offline](https://github.com/ppz-pro/mess-reader)

Trình đọc sách điện tử định dạng Epub chạy trực tiếp trên trình duyệt web, hỗ trợ lưu trữ cục bộ dữ liệu sách để người dùng có thể mở đọc bình thường ngay cả khi thiết bị không có kết nối mạng. (Đóng góp của [@daGaiGuanYu](https://github.com/ruanyf/weekly/issues/3302))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072708.webp)

6、[Automa: Tiện ích mở rộng Chrome hỗ trợ tự động hóa thao tác kéo thả](https://www.automa.site/)

Extension mạnh mẽ giúp người dùng thiết lập các kịch bản tự động hóa duyệt web (như tự động điền form, cào dữ liệu, click nút) thông qua sơ đồ khối kéo thả trực quan. Bên cạnh đó bạn đọc cũng có thể tham khảo [Công cụ ghi nhận hành vi Recorder mặc định của DevTools](https://developer.chrome.com/docs/devtools/recorder/). (Đóng góp của [@dllen](https://github.com/ruanyf/weekly/issues/3301))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072710.webp)

7、[Rickrack: Phần mềm quản lý bảng màu nghệ thuật mã nguồn mở](https://eigenmiao.com/yanhuo)

Ứng dụng quản lý và phối màu sắc (Palette manager) mã nguồn mở sở hữu giao diện nghệ thuật đẹp mắt, cung cấp nhiều thuật toán phối màu hài hòa hỗ trợ đắc lực cho các nhà thiết kế giao diện. (Đóng góp của [@eigenmiao](https://github.com/ruanyf/weekly/issues/3306))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072711.webp)

8、[iFrame Resizer: Thư viện tự động co giãn kích thước thẻ iframe theo nội dung](http://davidjbradshaw.github.io/iframe-resizer/)

Thư viện JS hữu ích giúp giải quyết vấn đề hiển thị của thẻ `<iframe>`: tự động tính toán chiều cao và độ rộng của trang web bên trong được nạp để tự động co giãn kích thước thẻ iframe tương ứng, tránh hiện tượng xuất hiện thanh cuộn xấu.

9、[Standard Ebooks: Bộ công cụ đóng gói và định dạng sách điện tử Epub](https://github.com/standardebooks/tools)

Mã nguồn mở cung cấp các công cụ dòng lệnh hỗ trợ biên tập, kiểm tra định dạng và đóng gói các văn bản thô thành tệp tin sách điện tử Epub tiêu chuẩn chất lượng cao. (Xem thêm [Tài liệu hướng dẫn từng bước](https://standardebooks.org/contribute/producing-an-ebook-step-by-step)).

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011103.webp)

10、[Tablane: Phần mềm quản lý công việc và danh sách dữ liệu nguồn mở](https://github.com/Tablane/tablane)

Ứng dụng web nguồn mở hỗ trợ quản lý dự án và phân chia công việc theo dạng bảng danh sách trực quan, phù hợp cho cá nhân hoặc nhóm nhỏ phối hợp công việc.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011206.webp)

## 资源

1、[Starlink Satellite Map: Bản đồ hiển thị vị trí thời gian thực của chòm vệ tinh Starlink](https://satellitemap.space/)

Trang web mô phỏng 3D trực quan vị trí bay và vùng phủ sóng thời gian thực của hơn 4.000 vệ tinh thuộc dự án phủ sóng Internet không gian Starlink của SpaceX trên quỹ đạo Trái Đất.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042907.webp)

2、[GhostlyStock: Thư viện công cụ tìm kiếm hình ảnh nghệ thuật sinh bởi AI](https://www.ghostlystock.com/)

Trang web hoạt động như một công cụ tìm kiếm hình ảnh chuyên biệt: toàn bộ các bức ảnh hiển thị trong kết quả tìm kiếm đều là tác phẩm do các mô hình trí tuệ nhân tạo (Generative AI) tự động vẽ và cho phép tải về sử dụng miễn phí.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100101.webp)

3、[ChatGPT Online: Giao diện web kết nối ChatGPT tiếng Trung trực tuyến](https://codenews.cc/chatgpt)

Trang web cung cấp cổng giao tiếp kết nối API với ChatGPT giúp người dùng trong nước dễ dàng trải nghiệm trò chuyện trực tiếp, đồng thời tổng hợp các tài nguyên hướng dẫn viết câu lệnh prompt tối ưu. (Đóng góp của [@jqsl2012](https://github.com/ruanyf/weekly/issues/3307))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072709.webp)

4、[Ứng dụng tìm kiếm và lưu trữ video học tập âm nhạc và thể thao dành cho trẻ em](https://github.com/ruanyf/weekly/issues/3287)

Tác giả chia sẻ mã nguồn một dự án nhỏ phát triển dưới dạng WeChat mini program, giúp các phụ huynh dễ dàng tìm kiếm, chọn lọc và lưu trữ nhanh các video bài giảng hướng dẫn chơi nhạc cụ hoặc tập luyện thể thao từ các nền tảng video về cho con học tập. (Đóng góp của [@rmrf](https://github.com/ruanyf/weekly/issues/3287))

5、[GPYTHON: Trang web hỗ trợ tự học lập trình ngôn ngữ Python có AI trợ giúp](https://gpython.aibang.run/)

Dịch vụ web giáo dục cung cấp môi trường viết và chạy code Python trực tuyến tương tác, tích hợp sẵn trợ lý ảo AI để giải thích lỗi code và đưa ra các bài tập rèn luyện thực hành. (Đóng góp của [@stanxing](https://github.com/ruanyf/weekly/issues/3308))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072712.webp)

## 图片

1\. **Bức ảnh ghi lại tầm nhìn xa bằng mắt thường đạt kỷ lục thế giới**

Vào ngày 16 tháng 7 năm 2016, một nhiếp ảnh gia leo núi đã thực hiện chụp một bức ảnh đặc biệt từ độ cao 2.820 mét trên đỉnh núi thuộc dãy Pyrenees nằm trên biên giới Tây Ban Nha:

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020819.webp)

Bức ảnh ghi nhận hình ảnh mờ ảo của đỉnh núi thuộc dãy Alps, Pháp nằm cách địa điểm chụp một khoảng cách địa lý khổng lồ lên tới **443 km**. Bức ảnh này đã được Tổ chức Kỷ lục Thế giới Guinness chính thức chứng nhận là bức ảnh ghi lại tầm nhìn xa trực tiếp bằng mắt thường đạt kỷ lục thế giới từ trước đến nay:

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020820.webp)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020821.webp)

2、**Hình ảnh Vạn Lý Trường Thành được phác họa theo phong cách búp bê Barbie bằng AI**

Sự bùng nổ của công nghệ AI tạo ảnh giúp con người dễ dàng hiện thực hóa mọi ý tưởng hình ảnh độc đáo.

Nhân dịp bộ phim điện ảnh *Barbie* ra mắt làm bùng nổ tông màu hồng trên thế giới, một kiến trúc sư đã yêu cầu AI phác họa lại công trình Vạn Lý Trường Thành của Trung Quốc nếu được phủ lên lớp sơn màu hồng rực rỡ đặc trưng của búp bê Barbie:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072719.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072720.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072721.webp)

## ✍️ Bài đọc thêm

### Chặng đường thăng trầm và sự trở lại ấn tượng của sợi vải dệt nhân tạo Polyester

Sợi Polyester (tên tiếng Trung: 涤纶) là một loại sợi tổng hợp nhân tạo được phát minh lần đầu tiên vào những năm 1920 và nhanh chóng tạo nên một cuộc cách mạng trong ngành dệt may thế giới:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072713.webp)

Thời kỳ đầu, Polyester được ca tụng như một chất liệu vải kỳ diệu của tương lai.

Vải có ưu điểm vượt trội là không bao giờ bị nhăn, giúp người mặc hoàn toàn không cần ủi là quần áo, chất vải lại rất mềm, dễ nhuộm các tông màu sặc sỡ nên lên hình chụp hoặc lên sóng truyền hình vô cùng bắt mắt.

Quan trọng hơn hết, chất liệu này có giá thành sản xuất cực kỳ rẻ và độ bền sợi rất cao, khó bị sờn rách sau thời gian dài sử dụng:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072714.webp)

Tuy nhiên đến những năm 1980, chất liệu vải này bỗng nhiên bị người tiêu dùng quay lưng và rơi vào tình trạng ế ẩm nghiêm trọng.

Nguyên nhân do vải dễ phát sinh hiện tượng xơ lông và vón cục sau vài lần giặt khiến bề mặt quần áo trông rất cũ kỹ.

Điểm yếu chí mạng nhất của Polyester thời kỳ đầu là khả năng thông khí cực kỳ kém. Người mặc quần áo Polyester khi vận động sẽ bị bí bách mồ hôi dẫn đến cảm giác ngột ngạt và phát sinh mùi cơ thể khó chịu. Dần dần, định kiến xã hội hình thành cho rằng chỉ có những người thu nhập thấp mới lựa chọn mặc các trang phục làm từ sợi Polyester rẻ tiền này.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072716.webp)

Giá trị thương mại của sợi Polyester sụt giảm thê thảm. Nhưng đúng vào thời điểm mọi người cho rằng chất liệu này sẽ sớm bị khai tử hoàn toàn, bước ngoặt mới đã xuất hiện.

Bước sang thế kỷ 21, xu hướng rèn luyện sức khỏe, chạy bộ ngoài trời, tập gym và leo núi dã ngoại bùng nổ mạnh mẽ trên toàn cầu. Các thương hiệu thời trang thể thao nhanh chóng nhận ra các đặc tính vật lý của Polyester lại cực kỳ phù hợp cho các hoạt động thể thao dã ngoại: vải có tính cản gió giữ nhiệt tốt; trọng lượng siêu nhẹ giúp giảm bớt sức nặng trang phục và sợi dai chịu lực kéo tốt trong môi trường rừng núi dã ngoại:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072717.webp)

Khi phân khúc thị trường thể thao dã ngoại bùng nổ, các doanh nghiệp đã đầu tư nghiên cứu khoa học vật liệu để cải tiến sâu cấu trúc sợi Polyester.

Họ đã phát triển công nghệ dệt giả lập cấu trúc của sợi len cừu tự nhiên, giúp tạo ra loại vải Polyester giả len siêu nhẹ nhưng có khả năng giữ nhiệt tốt hơn và thoát nước nhanh hơn len tự nhiên gấp nhiều lần, giúp Polyester nhanh chóng thống trị phân khúc áo khoác dã ngoại ngoài trời:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072718.webp)

Một hạn chế tự nhiên của Polyester là tính kỵ nước (không thấm nước), khiến mồ hôi cơ thể không thể thấm qua lớp vải để bay hơi ra ngoài được, gây cảm giác dính dớp khó chịu khi mặc sát da.

Các nhà khoa học vật liệu đã tập trung nghiên cứu giải quyết điểm nghẽn này. Sau nhiều năm thử nghiệm, họ đã cho ra mắt dòng sợi Polyester rỗng: cấu trúc bên trong sợi được thiết kế có các đường rãnh rỗng chạy dọc thân sợi. Thiết kế này tạo ra hiệu ứng mao dẫn vật lý, giúp chủ động hút mồ hôi từ bề mặt da truyền nhanh ra bề mặt phía ngoài của vải để bay hơi lập tức.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072715.webp)

Sau khi giải quyết được bài toán hút ẩm và thoát mồ hôi, Polyester trở thành nguyên liệu hàng đầu để sản xuất các loại áo thun thể thao và đồ lót vận động nhờ ưu điểm mỏng nhẹ, bền dai, không giữ mùi hôi và giặt máy dễ dàng.

Nhờ sự gia tăng của dân số tập luyện thể thao cùng ưu thế vượt trội về giá thành sản xuất, ngày nay Polyester đã vươn lên thành loại sợi dệt may có sản lượng tiêu thụ lớn nhất thế giới, chiếm hơn một nửa tổng lượng tiêu thụ sợi dệt toàn cầu (gấp đôi sản lượng của sợi bông tự nhiên xếp thứ hai). Sản lượng hàng năm của sợi Polyester hiện đạt gần 58 triệu tấn, gấp hơn 10 lần so với giai đoạn khủng hoảng những năm 1980.

## Lịch sử tuần này

- 2022年（第 217 期）：[Kiến trúc đô thị: Thiết kế và tham vọng xây dựng siêu đô thị tương lai The Line của Ả Rập Xê Út](http://www.ruanyifeng.com/blog/2022/08/weekly-issue-217.html)
- 2021年（第 167 期）：[Môi trường mạng: Thảo luận về việc các công cụ chặn quảng cáo đang đi quá giới hạn can thiệp web](http://www.ruanyifeng.com/blog/2021/07/weekly-issue-167.html)
- 2020年（第 117 期）：[Quyền riêng tư: Các biện pháp kỹ thuật giúp người dùng bảo vệ thông tin nhận diện khuôn mặt cá nhân](http://www.ruanyifeng.com/blog/2020/07/weekly-issue-117.html)
- 2019年（第 67 期）：[Lý thuyết hệ thống: Tại sao các hệ thống có cấu trúc quá phức tạp luôn tiềm ẩn nguy cơ đổ vỡ tất yếu](http://www.ruanyifeng.com/blog/2019/08/weekly-issue-67.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes team collaboration and document management seamless.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
