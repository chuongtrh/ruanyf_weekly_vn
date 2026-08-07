# 科技爱好者周刊（第 176 期）：中国法院承认 GPL 吗？

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1913) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091605.jpg)

Hội nghị Robot Thế giới 2021 tổ chức tại Bắc Kinh đã trưng bày mẫu robot hình người mô phỏng gương mặt nhà bác học "Albert Einstein" đang sử dụng tiếng Trung để giảng bài cho các học sinh tham quan. (Nguồn: [CCTV](https://photo.cctv.com/2021/09/11/PHOA6GQ0lb0RFhGynbF5j6U0210911.shtml))

## 主带话题：Tòa án Trung Quốc phán quyết ra sao về vi phạm giấy phép nguồn mở GPL?

Phần mềm nguồn mở thường đi kèm các điều khoản giấy phép (licenses) chặt chẽ. Nhiều người trong giới công nghệ luôn thắc mắc: Nếu các đơn vị trong nước vi phạm điều khoản giấy phép nguồn mở, liệu tác giả có thể khởi kiện ra tòa án dân sự hay không?

Mới đây, Tòa án Nhân dân Trung cấp thành phố Thâm Quyến đã đưa ra một phán quyết sơ thẩm gây chú ý lớn, yêu cầu bị đơn bồi thường 500.000 NDT do vi phạm giấy phép nguồn mở GPL.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091509.jpg)

Phán quyết này khiến nhiều lập trình viên phấn khởi vì cho rằng đây là sự công nhận chính thức của hệ thống pháp luật đối với giấy phép GPL tại Trung Quốc.

Tuy nhiên, sau khi nghiên cứu kỹ văn bản phán quyết, tôi nhận thấy bản chất vụ án phức tạp hơn nhiều và không thể đơn giản quy nạp rằng tòa án đã công nhận hoàn toàn tính hiệu lực của giấy phép GPL.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091510.jpg)

Tôi xin tóm tắt ngắn gọn vụ án như sau:

Công ty công nghệ Luohe Jining đã phát hành mã nguồn phần mềm VirtualApp trên GitHub kèm giấy phép GPL. Đồng thời, công ty đính kèm thêm một tuyên bố: *"Nghiêm cấm sử dụng phần mềm vào mục đích thương mại trừ khi người dùng mua bản quyền thương mại từ công ty"*.

Theo bạn, tuyên bố đính kèm này có hợp lệ không? **Liệu ta có thể vừa áp dụng giấy phép GPL vừa cấm người khác sử dụng mã nguồn vào mục đích thương mại không?**

Câu trả lời là: Tuyên bố này hoàn toàn mâu thuẫn với tinh thần của GPL. Giấy phép GPL cho phép thương mại hóa mã nguồn thoải mái, chỉ cần bạn phát hành code dưới dạng GPL thì bất kỳ ai cũng có quyền sử dụng nó vào mục đích thương mại.

> *[Kiến thức nguồn mở]*
> 
> *Nếu muốn cấm sử dụng thương mại, bạn không được phép sử dụng các giấy phép thuộc nhóm Copyleft (như GPL), mà phải tự soạn thảo một tuyên bố cấp phép riêng biệt (ví dụ: "Mã nguồn chỉ phục vụ học tập cá nhân, nghiêm cấm thương mại hóa dưới mọi hình thức trừ khi được cấp phép thương mại").*

Do Luohe chọn sai giấy phép ngay từ đầu nên tranh chấp đã xảy ra. Một ứng dụng thương mại nổi tiếng tên là "Dianxin Desktop" đã nhúng VirtualApp vào code của mình. Luohe đệ đơn kiện yêu cầu đối tác bồi thường 20 triệu NDT vì hành vi sử dụng thương mại không trả phí chứ không phải vì đối tác vi phạm GPL (không mở mã nguồn ứng dụng). Do đó, phán quyết phạt bồi thường của tòa án bản chất dựa trên việc đối tác vi phạm thỏa thuận cấp phép thương mại, chứ không trực tiếp liên quan đến GPL.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091511.jpg)

Tuy nhiên, bị đơn đã vin vào điều khoản GPL (cho phép thương mại hóa) để tự bào chữa, tuyên bố họ sử dụng phiên bản GPL miễn phí của VirtualApp chứ không dùng bản thương mại.

Tòa án đã bác bỏ lập luận này bằng cách chỉ ra Điều 8 của GPL quy định: Quyền cấp phép tự động chấm dứt nếu người dùng vi phạm các nghĩa vụ đi kèm (cụ thể ở đây là không chịu mở mã nguồn ứng dụng của mình). Do bị đơn vi phạm nghĩa vụ mở nguồn nên quyền sử dụng code dưới dạng GPL của họ lập tức vô hiệu, đồng nghĩa với việc hành vi nhúng code trở thành xâm phạm bản quyền thương mại của Luohe.

Phán quyết cho thấy: Tòa án Trung Quốc xem xét giấy phép GPL tương tự như một dạng hợp đồng dân sự thỏa thuận giữa tác giả và người dùng. Nghĩa là:

1. Chỉ có tác giả gốc của mã nguồn mới có quyền đứng ra khởi kiện vi phạm, cộng đồng không thể khởi kiện thay.
2. Ngay cả khi thắng kiện, phán quyết cao nhất cũng chỉ là yêu cầu gỡ bỏ phần mềm hoặc bồi thường thiệt hại tài chính chứ rất khó ép buộc bị đơn phải mở mã nguồn ứng dụng của họ do luật hợp đồng dân sự trong nước không có tiền lệ ép buộc này, đồng thời luật cho phép đối tác chọn đơn phương chấm dứt thực hiện hợp đồng.

## Khóa học viết công cụ dòng lệnh CLI bằng Node.js

Node.js ra mắt đã hơn 10 năm và làm thay đổi hoàn toàn bộ mặt của lập trình Front-end hiện đại. Tất cả các build tools cốt lõi hiện nay đều chạy trên môi trường Node.js.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091601.jpg)

Nhiều lập trình viên Front-end muốn học sâu Node.js để tự phát triển các công cụ tối ưu hóa công việc. Thực chất bạn chỉ cần làm chủ hai mảng kiến thức cốt lõi: **Định dạng module CommonJS và môi trường dòng lệnh (CLI - Command Line Interface)** cùng hệ thống API xử lý tệp tin (File System).

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091604.jpg)

Khóa học chuyên đề **《Build a Node.js CLI Tool from Scratch》** được thiết kế để dẫn dắt bạn thực hành mảng kiến thức này.

Khóa học đi thẳng vào việc hướng dẫn học viên tự tay viết một script dòng lệnh bằng JS, đóng gói cấu hình và phát hành trực tiếp lên hệ thống NPM để cộng đồng tải về sử dụng:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091602.jpg)

Khóa học được dẫn dắt bởi chuyên gia **Cui Xiaorui** (kỹ sư đóng góp mã nguồn Vue 3, người sáng lập Element3 UI và tác giả mini-vue) với phương pháp giảng dạy thực tế, tránh các lý thuyết tài liệu khô khan:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091603.jpg)

Độc giả bản tin có thể quét mã QR trên đây để đăng ký nhận video khóa học hoàn toàn **miễn phí (0đ)**.

## 科技动态

1、[Vận hành nhà máy thu hồi và hóa đá khí CO2 lớn nhất thế giới](https://climeworks.com/orca)

Nhà máy thu hồi và lưu trữ khí carbon (Direct Air Capture) mang tên Orca vừa chính thức đi vào vận hành tại Iceland.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091101.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091102.jpg)

Hệ thống sử dụng các cánh quạt hút khổng lồ để dẫn không khí đi qua các bộ lọc giữ lại khí CO2. Lượng CO2 sau đó được trộn với nước để hóa lỏng và bơm sâu 1.000 mét xuống các giếng địa chất sâu để phản ứng tự nhiên biến thành đá lưu trữ vĩnh viễn:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091103.jpg)

Tuy nhiên công suất thiết kế của nhà máy còn rất nhỏ so với lượng khí phát thải khổng lồ của nhân loại. Orca chỉ lọc được khoảng 4.000 tấn CO2 mỗi năm (tương đương lượng phát thải của 800 chiếc ô tô), trong khi lượng phát thải CO2 toàn cầu đã vượt quá 36 tỷ tấn. (Đóng góp của [@emac](https://github.com/ruanyf/weekly/issues/1946))

2、[Nghiên cứu Ig Nobel: Việc đi bộ xem điện thoại gây va chạm đám đông](https://mp.weixin.qq.com/s/9mTIHBJox5JMkrbl9nJcqA)

Giải thưởng khoa học Ig Nobel 2021 đã trao giải Động lực học cho nhóm nghiên cứu thuộc Đại học Kyoto, Nhật Bản với thí nghiệm nghiên cứu hành vi đám đông trên phố:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091303.jpg)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091304.jpg)

Kết quả đo đạc quỹ đạo di chuyển cho thấy khi hai dòng người đi bộ di chuyển ngược chiều nhau trên phố, chỉ cần có một vài cá nhân vừa đi vừa chăm chú nhìn màn hình điện thoại, nhịp độ di chuyển chung sẽ lập tức bị rối loạn và tỷ lệ xảy ra va chạm đám đông tăng lên đáng kể do các cá nhân xung quanh mất đi khả năng phán đoán hướng tránh tự nhiên. Đây là năm thứ 15 liên tiếp các học giả Nhật Bản nhận giải thưởng Ig Nobel độc đáo này:

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091305.jpg)

3、[Vận động viên vô địch giải marathon Vienna bị tước huy chương vì đế giày quá dày](https://www.thepaper.cn/newsDetail_forward_14479959)

Tại giải chạy Vienna Marathon ngày 12/9, vận động viên người Ethiopia cán đích đầu tiên với thành tích 2 giờ 09 phút 22 giây đã bị ban tổ chức tước bỏ huy chương vô địch do vi phạm quy chuẩn thiết kế giày chạy.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091401.jpg)

Theo quy định mới nhất của Liên đoàn Điền kinh Thế giới, độ dày phần đế giày của vận động viên không được phép vượt quá 40mm. Tuy nhiên, đôi giày chạy công nghệ mới của vận động viên này có độ dày đế lên tới 50mm, giúp tăng đáng kể lực đàn hồi phản hồi bước chạy để tiết kiệm thể lực.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091402.jpg)

4、[Thực trạng suy thoái của các trung tâm game xèng Arcade tại Nhật Bản](https://www.japantimes.co.jp/life/2021/06/06/digital/japanese-gaming-arcades-pandemic/)

Các trung tâm trò chơi điện tử xèng (Arcade gaming) từng là biểu tượng văn hóa giải trí thịnh vượng của Nhật Bản thời thập niên 80-90. Tuy nhiên ngành công nghiệp này đang chứng kiến đợt suy thoái mạnh mẽ.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082006.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082007.jpg)

Theo số liệu thống kê, vào năm 1986 Nhật Bản có tới 26.573 trung tâm game xèng hoạt động, nhưng con số này đã giảm xuống chỉ còn 4.022 cửa hàng vào năm 2019. Đợt dịch bệnh vừa qua tiếp tục giáng đòn mạnh khiến lượng cửa hàng đóng cửa tăng cao. Sự phổ biến của máy chơi game gia đình (consoles) và game di động là nguyên nhân chính khai tử các máy chơi game Arcade. Các tập đoàn game lớn như Sega, Square Enix đang kêu gọi chính phủ hỗ trợ tài chính để bảo tồn nét văn hóa giải trí độc đáo này:

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082008.jpg)

5、[Nhà máy điện mặt trời nổi quy mô lớn nhất thế giới đi vào hoạt động](http://m.cnhubei.com/content/2021-05/15/content_13795434.html)

Tại thành phố Đức Châu, tỉnh Sơn Đông mới đây đã khánh thành nhà máy điện mặt trời nổi trên mặt nước (floating solar farm) quy mô đơn thể lớn nhất thế giới. Dự án phủ kín các tấm pin mặt trời trên diện tích hồ nước rộng 146 ha với tổng công suất thiết kế 320 MW.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021090906.jpg)

Mô hình pin mặt trời nổi mang lại nhiều lợi ích kép: tiết kiệm tối đa chi phí giải phóng mặt bằng đất, giảm lượng nước bốc hơi của hồ chứa và hạn chế tảo sinh trưởng nhờ che phủ ánh sáng. Ngược lại, nhiệt độ mát mẻ của dòng nước phía dưới giúp hạ nhiệt các tấm pin mặt trời, tăng hiệu suất phát điện lên khoảng 10% so với đặt trên đất khô.

6、[Thí nghiệm về tác hại của lối sống cách ly độc lập ở loài ruồi giấm](https://www.nature.com/articles/d41586-021-02194-2)

Tạp chí *Nature* đăng tải công trình nghiên cứu hành vi xã hội của loài ruồi giấm. Các nhà khoa học đã tiến hành nuôi cách ly hoàn toàn các cá thể ruồi giấm độc lập và so sánh với nhóm ruồi giấm sinh hoạt bầy đàn bình thường.

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082105.jpg)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082104.jpg)

Kết quả cho thấy những cá thể ruồi giấm bị cô lập có biểu hiện rối loạn giấc ngủ nghiêm trọng (ngủ ít hơn) và tiêu thụ lượng thức ăn nhiều hơn rõ rệt. Nghiên cứu cảnh báo lối sống thiếu giao tiếp xã hội kéo dài có thể gây ra các biến đổi sinh học tiêu cực tương tự trên cơ thể con người.

## 文章

1、[Mười năm ngày khai tử hệ điều hành di động WebOS của Palm](https://sspai.com/post/68372)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082206.jpg)

Bài viết nhìn lại lịch sử thăng trầm của hệ điều hành WebOS do hãng Palm phát triển. Ra mắt cùng thời kỳ với iOS và Android, WebOS sở hữu giao diện thẻ vuốt đa nhiệm (card-based multitasking) và thanh thông báo thông minh cực kỳ đột phá đi trước thời đại trước khi bị khai tử vào ngày 11/8/2011.

2、[Xu hướng loại bỏ gương chiếu hậu vật lý trên các dòng xe ô tô mới](https://mp.weixin.qq.com/s/tUeFiMbQhpmXkffxVsts5w)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082405.jpg)

Bài viết phân tích xu hướng thiết kế ô tô hiện đại thay thế gương chiếu hậu kính bằng camera kỹ thuật số nhỏ hiển thị màn hình trong cabin giúp giảm tối đa hệ số cản gió của xe, từ đó tăng quãng đường di chuyển cho xe điện.

3、[Hướng dẫn dựng trình soạn thảo VS Code chạy trên nền web miễn phí](https://justyy.com/archives/45744)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091514.jpg)

Tác giả chia sẻ cách thức deploy và cấu hình trình soạn thảo VS Code (phiên bản web open-source) chạy trên các server cloud miễn phí phục vụ nhu cầu ghi chép và sửa code nhanh từ xa. (Đóng góp của [@DoctorLai](https://github.com/ruanyf/weekly/issues/1953))

4、[Những điều bạn chưa biết về tập đoàn bán dẫn ASML](https://threadreaderapp.com/thread/1429464932446183431.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082306.jpg)

Bài phân tích chi tiết về vị thế độc quyền của tập đoàn ASML (Hà Lan) - đơn vị duy nhất trên thế giới chế tạo thành công các dòng máy quang khắc cực tím EUV phục vụ đúc các dòng chip bán dẫn cao cấp dưới 7nm cho TSMC hay Intel.

5、[Bộ sưu tập 12 hình ảnh gây đánh lừa thị giác ấn tượng](https://nautil.us/blog/12-mind_bending-perceptual-illusions)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082803.jpg)

Giới thiệu các bức ảnh gây ảo giác thị giác nổi tiếng. Ví dụ như hai hình ảnh phía trên thực chất là một bức ảnh chụp con đường được nhân đôi đặt cạnh nhau nhưng não bộ tự động phân tích độ sâu khiến người xem cảm giác hai góc chụp lệch hướng khác nhau.

6、[Phép tính lấy giá trị tuyệt đối trong máy tính không đơn giản như bạn nghĩ](https://habr.com/en/post/574082/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082305.jpg)

Bài viết phân tích các lỗi tràn bộ nhớ (overflow) xảy ra trong các ngôn ngữ lập trình (như C++) khi thực hiện phép tính lấy giá trị tuyệt đối `abs()` của số nguyên âm nhỏ nhất (định dạng bù 2) do giới hạn lưu trữ bit của hệ thống.

7、[Tự viết custom hook usePrevious trong React](https://davidwalsh.name/react-useprevious-hook)（Tiếng Anh）

Tác giả hướng dẫn cách kết hợp bộ đôi hook tiêu chuẩn `useEffect` và `useRef` để tự xây dựng một custom hook `usePrevious` hỗ trợ lưu giữ và tra cứu giá trị props của lần render liền trước.

8、[Tìm hiểu tính năng Import Maps hỗ trợ ES Module trong trình duyệt](https://github.com/import-maps)（Tiếng Anh）

Giới thiệu tính năng Import Maps chính thức được hỗ trợ từ Chrome 89 cho phép lập trình viên Front-end cấu hình gán các biệt danh (alias) ngắn gọn cho các đường dẫn tải tệp tin ES Module trực tiếp mà không cần cấu hình qua Webpack.

## 工具

1、[Ventoy: Tiện ích tạo USB boot cài đặt đa hệ điều hành](https://github.com/ventoy/Ventoy)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082403.jpg)

Công cụ tạo USB cài win/linux cực kỳ mạnh mẽ, người dùng chỉ cần copy trực tiếp file ISO vào USB đã cài Ventoy là đã có thể khởi động cài đặt mà không cần format lại USB hay giải nén file.

2、[WebDen Code Editor](https://webden.dev/landing/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021082605.jpg)

Môi trường soạn thảo code HTML/CSS/JS gọn nhẹ được tối ưu giao diện chuyên dụng chạy mượt mà ngay trên các trình duyệt điện thoại di động giúp học lập trình cơ bản.

3、[View Source Online](https://neatnik.net/view-source/)

Tiện ích web gọn nhẹ, người dùng chỉ cần dán link URL trang web bất kỳ để hệ thống tự động bóc tách và hiển thị mã nguồn HTML được làm nổi bật cú pháp trực quan.

4、[fishdraw: Thư viện sinh hình vẽ cá ngẫu nhiên](https://github.com/LingDong-/fishdraw)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081311.jpg)

Một script JavaScript thú vị ứng dụng thuật toán hình học để tự động sinh ra các nét vẽ hình con cá ngẫu nhiên sinh động bằng nét vẽ chì Canvas. Xem thêm thư viện [tự vẽ cây tương tự](https://github.com/zv/tree).

5、[MDvideo: Chuyển đổi Markdown thành video tự động](http://mdvideo.gshll.com/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091513.jpg)

Ứng dụng hỗ trợ quét tệp tin Markdown, tự động tải các hình ảnh, video đính kèm link để biên tập thành một đoạn video giới thiệu sản phẩm hoàn chỉnh đi kèm giọng đọc thuyết minh AI. (Đóng góp của [@linqian02](https://github.com/ruanyf/weekly/issues/1952))

6、[group-by-repo-on-github Tampermonkey Script](https://github.com/foamzou/group-by-repo-on-github)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091210.jpg)

Script hỗ trợ nhóm kết quả tìm kiếm code trên trang GitHub theo từng repository tương ứng và tự động load trang tiếp theo khi cuộn chuột giúp tiết kiệm thời gian bấm Next. (Đóng góp của [@foamzou](https://github.com/ruanyf/weekly/issues/1941))

7、[iDraw.js Canvas Drawing Library](https://idraw.js.org/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091308.jpg)

Thư viện hỗ trợ lập trình viên viết script vẽ hình khối, text, chèn ảnh Canvas hoặc xuất bản vẽ dưới định dạng ảnh SVG chuyên nghiệp. (Đóng góp của [@chenshenhai](https://github.com/ruanyf/weekly/issues/1949))

8、[PikaScript: Chạy Python trên vi điều khiển cấu hình yếu](https://github.com/pikasTech/pikascript)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091306.jpg)

Dự án phát triển nhân dịch ngôn ngữ Python siêu gọn nhẹ giúp lập trình viên viết code Python để vận hành trực tiếp các dòng vi điều khiển (MCU) cấu hình RAM dưới 4KB trong thiết kế IoT. (Đóng góp của [@pikasTech](https://github.com/ruanyf/weekly/issues/1944))

9、[mini-stores: Quản lý trạng thái cho các App Mini Program](https://github.com/linjc/mini-stores)

Thư viện quản lý state gọn nhẹ giúp đồng bộ dữ liệu dùng chung giữa các trang (pages) dành riêng cho các ứng dụng nhỏ Mini Program (WeChat, Alipay). (Đóng góp của [@linjc](https://github.com/ruanyf/weekly/issues/1940))

10、[Neumorphism Flutter Shadow Generator](https://neumorphism.coldstone.fun/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091512.jpg)

Công cụ trực tuyến hỗ trợ thiết kế trực quan và tự sinh mã code Flutter tạo hiệu ứng đổ bóng 3D nổi theo phong cách Neumorphism. Xem thêm [phiên bản CSS](https://neumorphism.io/). (Đóng góp của [@xrr2016](https://github.com/ruanyf/weekly/issues/1951))

## Tài nguyên

1、[Samantha Ming Frontend Tips](https://www.samanthaming.com/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091307.jpg)

Trang blog chia sẻ các bài viết ngắn phân tích cú pháp HTML/CSS/JS chất lượng cao của nữ kỹ sư người Canada đi kèm các hình vẽ đồ họa giải thích vô cùng sinh động. (Đóng góp của [@wxyudl](https://www.samanthaming.com/))

2、[Chuyên trang giáo dục sức khỏe bệnh tiểu đường UCSF](https://dtc.ucsf.edu/zh-hans/)

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091110.jpg)

Trang tin y khoa của Đại học California San Francisco cung cấp các kiến thức khoa học thường thức bằng tiếng Trung về chế độ ăn uống, tập luyện phòng bệnh tiểu đường. (Đóng góp của [@Stupid-Human](https://github.com/ruanyf/weekly/issues/1938))

3、[Programmer's Introduction to Mathematics (Toán học cho lập trình viên)](https://pimbook.org/)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021081702.jpg)

Sách hướng dẫn toán học trực tuyến miễn phí (hỗ trợ tải bản PDF) dành riêng cho lập trình viên tự học bổ sung kiến thức giải tích, tuyến tính gắn liền với các ví dụ viết code mã hóa thực tế.

4、[SQL Bolt Interactive Tutorial](https://sqlbolt.com/)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071714.jpg)

Khóa học trực tuyến tương tác gồm 19 bài giảng thực hành truy vấn SQL cơ bản trực quan giúp người mới làm quen với thao tác kết nối database.

5、[Global Sourcebook: Danh mục định dạng dữ liệu quốc tế](http://www.grcdi.nl/gsb/global%20sourcebook.html)

![](https://cdn.beekka.com/blogimg/asset/202108/bg2021080512.jpg)

Bảng tra cứu định dạng địa chỉ nhà riêng, mã zip code, định dạng số điện thoại và loại tiền tệ của tất cả các quốc gia trên thế giới phục vụ thiết kế form nhập liệu toàn cầu.

## 图片

1、[Học lập trình web qua màn hình điện thoại di động](https://www.linkedin.com/posts/shubham-sharma-34bbab18b_webdevelopment-css-html-activity-6820715919568961536-WApS/)

Một thầy giáo tại Nepal chia sẻ bức ảnh chụp cậu học trò nghèo do không có máy tính xách tay đã tự thiết lập môi trường soạn thảo code ngay trên chiếc điện thoại di động cũ để kiên trì học lập trình web:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021072205.jpg)

Sau hai tháng kiên trì tự học, cậu học sinh đã bước đầu làm chủ được các kiến thức HTML, CSS và JS cơ bản.

2、[Chế tạo chiếc đàn piano dài nhất thế giới tại New Zealand](https://www.alexanderpiano.nz/page/the-alexander-piano)

Chất lượng âm thanh trầm của đàn piano phụ thuộc nhiều vào độ dài của sợi dây kim loại. Để tạo ra chiếc đàn có thể phát ra âm tần siêu trầm tự nhiên, anh Adrian - một thanh niên người New Zealand đã tự nghiên cứu bản vẽ kỹ thuật để tự đóng một chiếc đàn piano siêu dài:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071706.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071707.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071708.jpg)

Chiếc đàn piano hoàn thiện có chiều dài lên tới gần 10 mét. Tác giả hóm hỉnh chia sẻ anh rất muốn đóng chiếc đàn dài hơn nữa nhưng diện tích nhà kho của gia đình đã hết chỗ chứa:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071704.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071705.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071709.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071710.jpg)

Chất lượng âm trầm tuyệt vời của chiếc đàn độc nhất vô nhị này đã thu hút nhiều nghệ sĩ piano chuyên nghiệp tới biểu diễn trải nghiệm và thu âm phát hành đĩa nhạc:

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071711.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071712.jpg)

![](https://cdn.beekka.com/blogimg/asset/202107/bg2021071713.jpg)

## Bài đọc thêm

### Giai thoại lịch sử Pixar: Vụ tranh cãi chiếc bảng viết của Steve Jobs

*Trích cuốn tiểu sử Steve Jobs mô tả giai đoạn ông quản lý Pixar:*

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091611.jpg)

Sau khi bị trục xuất khỏi Apple vào năm 1985, Steve Jobs thành lập công ty máy tính NeXT đồng thời đầu tư rót vốn cứu vãn startup đồ họa máy tính Pixar đang đứng trước nguy cơ phá sản.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091613.jpg)

Thời kỳ đầu những năm 90, cả NeXT lẫn Pixar đều gặp khó khăn lớn về tài chính và chưa ra mắt được sản phẩm thương mại đột phá tạo doanh thu khiến Jobs chịu áp lực tinh thần rất lớn. Trong một buổi họp tại văn phòng Pixar, Jobs đã lớn tiếng chỉ trích gay gắt đội ngũ quản lý của Pixar do liên tục trễ hạn hoàn thiện bản vẽ bo mạch đồ họa thế hệ mới.

Nhà sáng lập Pixar là Alvy Ray Smith đã thẳng thắn phản bác lại: *"Thế bo mạch của NeXT bên ông đã làm xong chưa mà ông đứng đó chỉ trích chúng tôi?"*.

![](https://cdn.beekka.com/blogimg/asset/202109/bg2021091612.jpg)

Câu trả lời khiến Steve Jobs nổi giận lôi đình và lớn tiếng nhại lại giọng西南 đặc trưng của Smith để chế giễu. Cả hai đã đứng đối mặt nhau sát sạt để tranh cãi nảy lửa. Steve Jobs vốn có thói quen độc chiếm chiếc bảng viết trắng trong phòng họp và không cho ai sử dụng. Smith với thân hình cao lớn đã chủ động đẩy nhẹ Jobs ra để tự tay cầm bút viết giải thích ý tưởng lên bảng. Jobs hét lớn yêu cầu Smith dừng lại nhưng Smith phản pháo: *"Bảng này là của riêng ông à? Tại sao tôi không được viết lên đây?"*. Buổi họp kết thúc bằng việc Jobs tức giận bỏ về.

Ít lâu sau sự việc, Smith đã quyết định từ chức rời khỏi Pixar để tự thành lập một công ty phần mềm đồ họa mới. Công ty này sau đó đã được tập đoàn Microsoft mua lại thành công. Smith trở thành người duy nhất trong lịch sử công nghệ sáng lập hai công ty phần mềm lớn, một công ty bán cho Steve Jobs và công ty còn lại bán cho Bill Gates.

## 言论

1、

Đối với các lập trình viên, một trong những kinh nghiệm xương máu nhất là: Tuyệt đối không bao giờ thực hiện việc copy và paste trực tiếp các đoạn mã nguồn do người khác viết trên các diễn đàn (như StackOverflow) vào dự án của mình. Nếu muốn sử dụng, hãy tự tay gõ lại từng ký tự. Việc tự gõ lại từng chữ buộc bộ não của bạn phải suy nghĩ thấu đáo logic thực tế của dòng code đó hoạt động ra sao và dễ phát hiện ra các lỗi tiềm ẩn.

-- Thảo luận trên Hacker News

2、

Sự không chắc chắn của áp lực (uncertainty of stress) thực tế gây tổn hại tinh thần lớn hơn bản thân áp lực đó. Một nghiên cứu y khoa về đợt ném bom London thế chiến 2 ghi nhận: tỷ lệ bệnh nhân bị loét dạ dày tăng mạnh ở các vùng ngoại ô (nơi thỉnh thoảng mới có bom rơi ngẫu nhiên không báo trước) cao hơn nhiều so với khu vực trung tâm thành phố (nơi người dân đã quen với tần suất bom rơi cố định hàng đêm và chủ động chuẩn bị hầm trú ẩn).

-- Trích bài viết "Become an Uncertainty Killer"

3、

Bí quyết để duy trì hạnh phúc trong cuộc sống thực chất là hãy giữ cho bản thân một mức kỳ vọng thấp (low expectations).

-- Thảo luận trên Hacker News

## 历史上的本周

- 2020年（第 125 期）：[Phân tích vai trò và mục tiêu thay thế tiền mặt truyền thống của đồng Nhân dân tệ kỹ thuật số](https://www.ruanyifeng.com/blog/2020/09/weekly-issue-125.html)
- 2019年（第 73 期）：[Tìm hiểu sức mạnh của việc thống kê và trực quan hóa dữ liệu trong khoa học xã hội](https://www.ruanyifeng.com/blog/2019/09/weekly-issue-73.html)
- 2018年（第 22 期）：[Tranh chấp bản quyền thú vị xung quanh bản quyền bức ảnh tự sướng của chú khỉ Naruto ngoài tự nhiên](https://www.ruanyifeng.com/blog/2018/09/weekly-issue-22.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
