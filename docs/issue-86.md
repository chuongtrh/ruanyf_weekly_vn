# 科技爱好者周刊：第 86 期 (Bản tin chia sẻ công nghệ số 86)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), chào mừng gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục issue.

Mục tuyển dụng [《Ai đang tuyển dụng?》](https://github.com/ruanyf/weekly/issues/983) cung cấp nhiều thông tin việc làm hữu ích, hoan nghênh ghé thăm hoặc đăng tải thông tin tuyển dụng/thực tập.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112713.jpg)

Ảnh bìa: Ảnh chụp chế độ ban đêm (Night Sight) của Google Pixel 4 XL.

## 刊首语 (Lời tựa)

Gần đây, tôi có đọc được một bài trắc nghiệm tâm lý thú vị mang tên: "Bạn có phải là một người theo đuổi chủ nghĩa hoàn hảo không?", các câu hỏi thảo luận khá thực tế:

> 1. Bạn có thường xuyên đặt ra mục tiêu cho bản thân, nhưng kết cục phần lớn đều không đạt được chúng không?
> 2. Khi một công việc chưa được thực hiện tốt như ý, bạn có luôn thôi thúc muốn làm lại nó một lần nữa không?
> 3. Trong những khoảng thời gian nghỉ ngơi, đầu óc bạn có vẫn liên tục suy nghĩ về học tập, công việc hoặc các vấn đề chưa được giải quyết không?
> 4. Nếu có ai đó nói xen vào hoặc làm gián đoạn sự tập trung của bạn, bạn có cảm thấy không vui không?
> 5. Bạn có thường xuyên tự hỏi bản thân sau mỗi sự việc rằng nếu lúc đó chọn cách giải quyết khác thì kết quả có lẽ sẽ lý tưởng hơn không?

Nếu toàn bộ câu trả lời của bạn cho các câu hỏi trên đều là "Có", thì bạn đang sở hữu xu hướng của một người theo đuổi chủ nghĩa hoàn hảo (perfectist).

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121213.jpg)

Hiểu một cách đơn giản, chủ nghĩa hoàn hảo là việc luôn đặt ra và theo đuổi các mục tiêu ở tiêu chuẩn cực kỳ cao, đồng thời từ chối chấp nhận các kết quả ở mức độ thấp hơn dù chúng hoàn toàn có thể sử dụng được. Điều này thực chất không tốt. Bản thân tôi luôn tự răn đe mình tuyệt đối không được rơi vào cái bẫy của sự hoàn hảo. Như [một bài viết](https://medium.com/live-your-life-on-purpose/stop-trying-to-be-perfect-live-your-life-as-you-want-4735768055df) từng phân tích, rào cản lớn nhất của chủ nghĩa hoàn hảo là nó vô tình ép bạn phải đánh đổi bằng chi phí cơ hội và tài nguyên cực kỳ đắt đỏ:

> Chủ nghĩa hoàn hảo tạo ra một áp lực vô hình, ép bạn tự đặt ra những kỳ vọng phi thực tế cho bản thân. Dù bạn đã hoàn thành công việc ở mức độ tốt thông thường, nhưng do mục tiêu đặt ra quá cao, bạn vẫn có cảm giác mình còn cách đích đến rất xa. Tư duy của bạn sẽ luôn bị kẹt trong suy nghĩ: "Mọi thứ vẫn chưa đủ tốt, vẫn có thể cải tiến thêm nữa".
> 
> Việc này sẽ tiêu tốn toàn bộ lượng thời gian và tài nguyên quý giá nhất của chúng ta, làm phân tán sự tập trung khỏi những nhiệm vụ thực sự quan trọng cần ưu tiên trước mắt.

Trong [các số bản tin trước](https://www.ruanyifeng.com/blog/2019/08/weekly-issue-69.html), tôi từng chia sẻ quan điểm rằng "làm nhanh" quan trọng hơn nhiều so với "làm tốt". Thứ chúng ta thực sự cần là tạo ra tối đa lượng sản phẩm thực tế với chi phí tối thiểu, chứ không phải dồn hết nguồn lực đắt đỏ để trau chuốt duy nhất một tác phẩm hoàn mỹ. Việc theo đuổi sự hoàn hảo sẽ cản trở tốc độ triển khai của chúng ta.

Thêm vào đó, áp lực tinh thần quá lớn do chủ nghĩa hoàn hảo mang lại cũng không hề tốt cho sức khỏe thể chất và tâm lý. Hãy học cách chấp nhận sự tương đối và sống một cuộc sống thoải mái, tự do hơn.

## Quà tặng tài nguyên học tập Trí tuệ Nhân tạo

Trí tuệ nhân tạo (AI) đang là xu hướng công nghệ lớn nhất hiện nay của ngành IT, kéo theo nhu cầu tuyển dụng nhân sự chất lượng cao vô cùng lớn với mức thu nhập vượt trội. Phần lớn các bạn sinh viên tôi gặp đều có định hướng muốn theo học và phát triển sự nghiệp ở mảng này. Tuy nhiên, AI vốn là mảng không dễ tự học do đòi hỏi lượng kiến thức toán học, thuật toán nền tảng lớn kết hợp cùng kỹ năng lập trình thực chiến.

Nhằm hỗ trợ các bạn học tập hệ thống hơn, học viện Gupao gửi tặng độc giả của bản tin **gói tài nguyên học tập AI chuyên sâu dung lượng 200GB**, bám sát yêu cầu tuyển dụng thực tế của doanh nghiệp gồm các mảng: (1) Tài liệu lập trình Python, (2) Toán học nền tảng cho AI, (3) Kỹ thuật xử lý dữ liệu và Frameworks, (4) Học máy (Machine Learning) và Học sâu (Deep Learning).

Tài nguyên bao gồm đầy đủ các định dạng bài học: video bài giảng, sách chuyên ngành PDF, sơ đồ tư duy hệ thống và các dự án thực tế. Phần video bài giảng được trực tiếp giảng dạy bởi thầy Tần - cựu chuyên gia nghiên cứu thuật toán học sâu tại Google với hơn 10 năm kinh nghiệm nghiên cứu hạ tầng tìm kiếm. Dưới đây là lộ trình học tập AI hệ thống đi kèm (quét mã để xem hình lớn):

[![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121212.jpg)](https://cdn.beekka.com/blogimg/asset/201912/bg2019121211.jpg)

Học viện Gupao thành lập từ năm 2016, hiện đang là một trong những đối tác đào tạo công nghệ hàng đầu trên Tencent Classroom với hơn 400.000 lượt học viên theo học. Học viện đã hỗ trợ hơn 18.000 kỹ sư nâng cao thu nhập thành công và gia nhập các tập đoàn lớn (Alibaba, Baidu, Tencent, iFlytek). Lộ trình bài giảng do các chuyên gia hàng đầu thiết kế, cam kết dạy học tương tác trực tuyến và chia sẻ toàn bộ mã nguồn dự án. Các học viên xuất sắc sẽ nhận được thư giới thiệu ứng tuyển trực tiếp vào các doanh nghiệp lớn (Alibaba, Huawei, ByteDance).

Độc giả quan tâm có thể quét mã QR dưới đây để nhận miễn phí gói tài nguyên AI 200GB (chỉ giới hạn **199 suất đăng ký đầu tiên**):

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121112.jpg)

## 资讯 (Tin tức)

1. **Thực hiện thành công ca phẫu thuật não có robot hỗ trợ điều khiển từ xa đầu tiên trên thế giới**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110703.jpg)

Ngày 1/11, các bác sĩ tại Toronto (Canada) đã thực hiện thành công ca phẫu thuật can thiệp mạch máu não cho một bệnh nhân nữ 64 tuổi bằng cách điều khiển cánh tay robot từ xa qua máy tính để đặt coil và stent điều trị chứng phình động mạch não. Bác sĩ vận hành bảng điều khiển đặt cách giường bệnh nhân vài mét. Ca phẫu thuật diễn ra suôn sẻ trong vòng 2.5 giờ, bệnh nhân hồi phục tốt và được xuất viện ngay ngày hôm sau.

Trước đây, các hệ thống robot phẫu thuật (như da Vinci) thường chỉ được ứng dụng phổ biến trong phẫu thuật thay khớp gối, tuyến tiền liệt hoặc can thiệp tim mạch, chưa từng được áp dụng cho phẫu thuật não do cấu trúc mạch máu não vô cùng nhỏ và chằng chịt đòi hỏi độ chính xác tuyệt đối. Đội ngũ nghiên cứu kỳ vọng sẽ tiến tới thử nghiệm ca phẫu thuật não điều khiển hoàn toàn từ xa qua mạng internet vào năm tới, mở ra cơ hội cho các chuyên gia hàng đầu thực hiện các ca mổ phức tạp xuyên quốc gia.

2. **Cơn sốt săn lùng ngà voi ma mút bùng nổ tại các vùng đất đóng băng vùng Siberia**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112701.jpg)

Làn sóng ấm lên toàn cầu đang làm tan chảy các lớp đất đóng băng vĩnh cửu tại vùng Siberia (Nga), vô tình hé lộ hàng triệu xác voi ma mút cổ đại bị chôn vùi dưới lòng đất suốt hàng vạn năm. Thực tế này đã thu hút hàng nghìn thợ săn ngà voi đổ về đây. Họ sử dụng các vòi rồng phun nước áp lực cao để quét sạch các lớp bùn đất đầm lầy nhằm tìm kiếm các cặp ngà voi ma mút khổng lồ còn nguyên vẹn để xuất khẩu sang thị trường châu Á với mức giá đắt đỏ.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112702.jpg)

Ước tính vẫn còn khoảng 10 triệu xác voi ma mút đang bị chôn vùi trong lớp băng vĩnh cửu tại Siberia, con số vượt xa tổng số lượng voi châu Phi đang sinh sống hiện nay. Trong hoạt động thương mại ngà voi mỹ nghệ, việc phân biệt giữa ngà voi ma mút cổ đại và ngà voi châu Phi tự nhiên bằng mắt thường là cực kỳ khó khăn.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112703.jpg)

3. **Ý tưởng bàn làm việc tích hợp máy phát điện đạp chân giúp lập trình viên vận động khi gõ code**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112704.jpg)

Một kỹ sư phần mềm người Mỹ đã tự thiết kế một hệ thống bàn làm việc thông minh tích hợp bộ bàn đạp xe đạp và máy phát điện ở phía dưới chân. Trong suốt thời gian ngồi gõ code làm việc với máy tính, anh sẽ liên tục đạp chân để phát điện trực tiếp duy trì hoạt động cho case máy tính, màn hình và sạc điện thoại di động. Đây là giải pháp thú vị giúp những người làm việc văn phòng duy trì vận động thể chất hàng ngày.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112705.jpg)

Tác giả chia sẻ: với tốc độ đạp xe đều đặn hàng giờ, anh có thể sản sinh ra lượng điện năng khoảng 60W, đồng thời giúp đốt cháy tới 300 calo năng lượng. Hệ thống bàn làm việc được trang bị 8 ổ cắm điện ngõ ra và tích hợp một máy tính nhúng nhỏ kết nối không dây, cho phép hiển thị biểu đồ thống kê sản lượng điện năng sản sinh và quản lý các thiết bị kết nối trực tiếp trên màn hình.

4. **Kỷ lục mới về việc giải mã bài toán phân tích số nguyên khổng lồ thành thừa số nguyên tố**

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019120403.jpg)

Các nhà khoa học quốc tế công bố đã thực hiện thành công việc phân tích một số nguyên khổng lồ có độ dài 240 chữ số thập phân (tương đương khóa mật mã có độ dài 795 bit nhị phân) thành tích của hai số nguyên tố lớn. Đây là kỷ lục mới về độ dài khóa mật mã bị giải mã thành công, vượt qua kỷ lục giải mã khóa 768 bit trước đó.

Phép toán phân tích số nguyên lớn thành thừa số nguyên tố là nền tảng toán học cốt lõi bảo vệ sự an toàn của hệ thống mật mã mã hóa công khai RSA hiện đại. Một khi bài toán này được giải quyết nhanh chóng, toàn bộ các cổng bảo mật HTTPS trên internet sẽ bị vô hiệu hóa. Tuy nhiên, do các tiêu chuẩn bảo mật hiện nay đều khuyến nghị độ dài khóa tối thiểu 2048 bit nên hệ thống vẫn tuyệt đối an toàn. Ca giải mã kỷ lục lần này tiêu tốn năng lượng tính toán tương đương 4.000 năm chạy liên tục của một nhân CPU 2.1 GHz với tổng chi phí ước tính khoảng hơn 100.000 USD.

5. **Hệ thống hiển thị mức độ đông đúc của xe bus theo thời gian thực tại Thượng Hải**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112709.jpg)

Các trạm chờ xe bus tại Thượng Hải đang tiến hành chạy thử nghiệm bảng điện tử thông minh hiển thị mức độ đông đúc của chuyến xe tiếp theo sắp cập bến. Phía sau thông tin tuyến xe, bảng sẽ hiển thị từ 1 đến 3 biểu tượng hình người tương ứng với các trạng thái: "Thoải mái (ít khách), Vừa phải, Đông đúc".

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112710.jpg)

Hệ thống hoạt động dựa trên thuật toán phân tích hình ảnh camera lắp trong xe. Sau khi xe xuất phát khỏi trạm được 30 giây, các camera an ninh trong xe sẽ ghi lại hình ảnh mật độ hành khách và gửi về máy chủ trung tâm để thuật toán AI tự động phân tích tính toán không gian trống. Việc này giúp hành khách tại trạm chủ động lựa chọn lên xe hoặc chờ chuyến sau trống hơn, đồng thời hỗ trợ bộ phận điều hành tự động điều chỉnh tần suất xuất bến của các xe để tối ưu hóa khoảng cách giãn cách xe trên tuyến.

6. **Giải pháp sản xuất giấy viết bảo vệ môi trường làm từ đá tự nhiên**

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112801.jpg)

Hoạt động sản xuất giấy viết truyền thống từ bột gỗ cây rừng thường gây ra các vấn đề tàn phá rừng và ô nhiễm nguồn nước do hóa chất tẩy trắng. Để giải quyết vấn đề này, các nhà sản xuất đang đẩy mạnh thương mại hóa dòng sản phẩm "Giấy đá" (Stone Paper) với các đặc tính chống nước, độ bền cao và thân thiện môi trường do không sử dụng gỗ cây rừng hay hóa chất tẩy trắng công nghiệp.

Giấy đá được sản xuất với thành phần chứa khoảng 80% bột canxi cacbonat (thành phần chính cấu tạo nên đá vôi và đá cẩm thạch) thu gom từ phế thải đá của các mỏ khai thác đá và công trường xây dựng, được nghiền mịn thành bột rồi trộn cùng một lượng nhỏ nhựa sinh học để cán mỏng thành các tờ giấy. Do cấu trúc được hình thành từ các hạt bột đá mịn thay vì các sợi xenlulozo thô của gỗ cây, bề mặt giấy đá mang lại cảm giác viết vô cùng mượt mà, êm ái hơn hẳn giấy thường. Tuy nhiên, dòng giấy này bắt buộc phải có quy trình phân loại tái chế chuyên biệt, không thể trộn lẫn cùng giấy gỗ thông thường.

7. **Tin vắn**

- Báo cáo nghiên cứu kinh tế của EU chỉ ra rằng các nhóm ngành công nghiệp ứng dụng tri thức vật lý thực nghiệm chuyên sâu (như kỹ thuật điện, cơ khí, kỹ thuật xây dựng và công nghệ thông tin) có đóng góp tỷ trọng GDP cho liên bang lớn hơn cả ngành dịch vụ tài chính hay bán lẻ.

- Mạng xã hội Instagram chính thức chạy thử nghiệm tính năng ẩn số lượng lượt thích (likes) hiển thị dưới các bài viết nhằm giảm thiểu áp lực tâm lý so sánh và các cuộc đua tương tác vô nghĩa của người dùng.

- Do tình trạng quá tải công suất sản xuất chip 14nm, tập đoàn Intel quyết định tái khởi động một phần dây chuyền sản xuất tiến trình 22nm cũ để tiếp tục sản xuất dòng CPU giá rẻ Pentium Haswell đáp ứng nhu cầu thị trường máy tính phân khúc thấp.

- Một kỹ sư người Israel thiết kế bộ điều khiển gắn cánh quạt đặc biệt cho phép lắp lên các mẫu máy bay giấy xếp tay thông thường để điều khiển quỹ đạo bay của máy bay giấy qua ứng dụng di động, dự án thu hút hơn 1 triệu USD vốn góp cộng đồng trên Kickstarter.

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019110102.jpg)

## 文章 (Bài viết)

1、[Bài viết] [Tìm hiểu về cơ chế hoạt động của AudioContext API hỗ trợ sinh mã dấu vân tay âm thanh để theo dõi người dùng](https://iq.opengenus.org/audio-fingerprinting/) (Tiếng Anh)

Phân tích một phương thức theo dõi người dùng tinh vi (Audio Fingerprinting): thay vì dùng Cookie vốn dễ bị trình duyệt chặn, trang web sẽ sử dụng thư viện AudioContext API để tạo ra một dải sóng âm thanh tần số cao đặc thù qua loa thiết bị và đo đạc sự phản hồi của phần cứng để tạo ra một mã định danh duy nhất (vân tay) của thiết bị người dùng.

2、[Bài viết] [Tại sao việc lạm dụng lệnh git rebase lại tiềm ẩn nhiều nguy cơ cho mã nguồn dự án?](https://www.fossil-scm.org/fossil/doc/trunk/www/rebaseharm.md) (Tiếng Anh)

Phân tích chi tiết về mặt kỹ thuật lý do tại sao lệnh `git rebase` có thể gây mất mát lịch sử commit thực tế của dự án, làm xáo trộn lịch sử code và gây khó khăn cho việc debug tìm kiếm nguồn gốc lỗi trên các nhánh phát triển chung của đội ngũ lập trình.

3、[Bài viết] [Lời khuyên hữu ích cho quản trị viên tên miền: Hạn chế cài đặt chỉ số TTL quá thấp cho bản ghi DNS](https://00f.net/2019/11/03/stop-using-low-dns-ttls/) (Tiếng Anh)

TTL (Time to Live) quy định thời gian các máy chủ trung gian được phép cache thông tin phân giải tên miền của bạn. Tác giả phân tích tác hại khi đặt TTL quá ngắn: làm tăng lượng truy vấn DNS không cần thiết lên máy chủ tên miền gốc và làm chậm tốc độ tải trang ban đầu của người dùng, đề xuất mức cấu hình an toàn từ 40 phút đến 1 giờ.

## 软件 (Phần mềm)

1、[fingerprint.js — Thư viện JavaScript hỗ trợ tạo mã dấu vân tay trình duyệt để định danh thiết bị](https://github.com/Valve/fingerprintjs2)

Giải pháp phân tích các thông số cấu hình trình duyệt (phông chữ hệ thống, độ phân giải màn hình, card đồ họa, WebGL) để sinh ra một chuỗi mã định danh duy nhất của thiết bị mà không cần dùng đến cookie của người dùng.

2、[erra — Công cụ hỗ trợ debug, đánh chặn và giả lập dữ liệu API viết bằng Node.js](https://github.com/hughfenghen/erra)

Giúp các nhà phát triển dễ dàng kiểm tra hoạt động mạng: tự động đánh chặn các gói tin HTTP/HTTPS của ứng dụng, cho phép sửa đổi dữ liệu request/response trực tiếp để chạy thử nghiệm các kịch bản kiểm thử API.

3、[fast-astar — Tiện ích trực quan hóa thuật toán tìm đường tối ưu A* (A-Star) trên nền tảng web](https://sbfkcel.github.io/fast-astar/)

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019111201.jpg)

Giúp học viên dễ dàng hiểu nguyên lý hoạt động của thuật toán tìm đường đi ngắn nhất A* thông qua bản đồ lưới tương tác trực quan, cho phép tùy chỉnh vị trí điểm đầu, điểm cuối và các khối chướng ngại vật để quan sát quá trình dò đường.

## 资源 (Tài nguyên)

1、[Sách] [Giáo trình tự học tiếng Đức căn bản dành cho người đã biết tiếng Anh](https://courses.dcs.wisc.edu/wp/readinggerman/print-entire-textbook/)

Tài liệu giảng dạy tiếng Đức hệ thống được biên soạn và chia sẻ miễn phí bởi Đại học Wisconsin, thiết kế phương pháp học tập so sánh ngữ pháp trực quan giúp người học dễ dàng tiếp cận.

2、[Tài liệu] [Tài liệu hướng dẫn thiết kế chuẩn giao tiếp REST API của tập đoàn Microsoft](https://github.com/microsoft/api-guidelines/blob/master/Guidelines.md)

Tài liệu hướng dẫn chính thức quy định các tiêu chuẩn thiết kế tên miền API, định dạng dữ liệu JSON phản hồi, các mã trạng thái HTTP sử dụng và phương thức quản lý phiên bản (versioning) của Microsoft.

## 图片 (Hình ảnh)

1. **Norilsk - Khung cảnh đóng băng khắc nghiệt của thành phố công nghiệp cực bắc thế giới**

Thành phố Norilsk (Nga) nằm cách vòng cực bắc hơn 400km về phía bắc, ghi nhận nhiệt độ mùa đông thường xuyên giảm sâu dưới -40 độ C. Đây là đô thị được xây dựng từ thời kỳ khai thác mỏ tài nguyên khí đốt lớn của Nga.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019101301.jpg)

Nhiếp ảnh gia Elena Chernyshova đã dành 7 tháng sinh sống tại đây để ghi lại những hình ảnh chân thực về đời sống người dân: từ những sảnh hành lang chung cư đóng băng phủ đầy tuyết trắng do hệ thống sưởi rò rỉ cho đến các con phố ngập trong bóng tối của mùa cực đêm kéo dài.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121121.jpg)

2. **Những phát minh kỳ quặc nhưng vô hại của nhà thiết kế sáng tạo**

Chuyên trang tổng hợp những ý tưởng thiết kế độc đáo nhưng không mang lại giá trị sử dụng thực tế cao:

Mẫu kính đặc biệt tích hợp gương phản chiếu hỗ trợ người đi bộ dễ dàng quan sát toàn bộ khung cảnh phía sau lưng mà không cần quay đầu lại.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102101.jpg)

Chiếc áo phông tích hợp các tấm pin năng lượng mặt trời mỏng ở mặt trước hỗ trợ sạc điện thoại di động khi đi dạo ngoài trời nắng.

![](https://cdn.beekka.com/blogimg/asset/201910/bg2019102103.jpg)

## 文摘 (Văn trích)

1. **Lịch sử ra đời của mô hình rạp chiếu phim ô tô (Drive-in Theater) độc đáo của nước Mỹ**

Vào đầu thập niên 1930, một người đàn ông tên Richard Hollingshead sống tại bang New Jersey đã nảy ra ý tưởng đặt một máy chiếu phim gia đình lên nóc chiếc ô tô của mình, rồi ngồi ở hàng ghế trước xe để thưởng thức bộ phim chiếu lên cánh cửa gara nhà.

Hàng xóm xung quanh phát hiện ra sự việc thú vị này đã kéo nhau sang sân nhà ông để cùng xem ké phim từ cabin ô tô của họ. Nhận thấy tiềm năng thương mại lớn, Hollingshead đã đăng ký bản quyền sáng chế và chính thức khai trương rạp chiếu phim ô tô (Drive-in Theater) thương mại đầu tiên vào năm 1933 tại thị trấn Camden.

![](https://cdn.beekka.com/blogimg/asset/201912/bg2019121119.jpg)

Đến thập niên 1950 khi ô tô trở thành phương tiện phổ thông của mọi gia đình Mỹ, mô hình rạp chiếu phim này đã bùng nổ mạnh mẽ, tăng trưởng thần tốc từ con số không lên tới hơn 6.000 rạp chiếu phim ô tô trên khắp cả nước chỉ trong vòng chưa đầy 10 năm.

Mô hình này mang lại nhiều sự tiện lợi: các gia đình có con nhỏ có thể cho con mặc đồ ngủ nằm chơi ở hàng ghế sau mà không sợ làm phiền người khác, bớt được chi phí thuê người trông trẻ. Nhiều rạp thậm chí còn liên kết cung cấp các dịch vụ giặt là: khách hàng giao túi đồ bẩn khi vào rạp và nhận lại quần áo đã giặt sấy thơm tho sau khi phim kết thúc.

Tuy nhiên, mô hình rạp chiếu phim ô tô cũng nhanh chóng bộc lộ các nhược điểm gây suy giảm trải nghiệm: việc ngồi liên tục trong cabin xe chật hẹp khiến người xem dễ bị mỏi lưng đè vô lăng, tầm nhìn ra màn hình lớn ngoài trời dễ bị hạn chế bởi bụi đường hay xác côn trùng bám trên kính chắn gió của xe, âm thanh phát ra từ những chiếc loa nhỏ treo bên cửa kính xe có chất lượng khá tệ. Vào những đêm trời lạnh, hơi ấm từ hơi thở của người ngồi trong xe làm kính chắn gió liên tục bị mờ sương buộc hành khách phải lau kính liên tục, và hoạt động chiếu phim ngoài trời hoàn toàn bị tê liệt mỗi khi trời mưa lớn. Đó chính là lý do mô hình rạp chiếu phim độc đáo này nhanh chóng thoái trào nhường chỗ cho các phòng chiếu phim hiện đại có điều hòa và ghế ngồi êm ái.

## 言论 (Danh ngôn)

1、

> "Triết lý phát triển tinh gọn (Agile) luôn yêu cầu toàn bộ đội ngũ lập trình phải duy trì tốc độ phát triển cực cao trong suốt dự án. Hãy tự hỏi: có vận động viên điền kinh nào có khả năng chạy nước rút với vận tốc tối đa từ vạch xuất phát cho tới tận đích của một cuộc chạy cự ly dài hay không? Câu trả lời là không, chạy nước rút chỉ khả thi ở cự ly ngắn.
> 
> Giải pháp chắp vá mà Agile đưa ra thực ra rất đơn giản: họ chia nhỏ toàn bộ chặng đường phát triển dài hạn thành các đoạn ngắn 100 mét (sprints) và yêu cầu các lập trình viên phải thực hiện các cuộc chạy nước rút liên tục trên từng đoạn ngắn đó."
> 
> -- Rich Hickey, cha đẻ ngôn ngữ Clojure

(Hết)
