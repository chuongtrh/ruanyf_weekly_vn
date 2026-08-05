# 每周分享第 7 期 (Bản tin chia sẻ hàng tuần số 7)

Ghi lại những điều thú vị đáng chia sẻ tôi bắt gặp trong tuần qua, phát hành vào thứ Sáu hàng tuần.

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053001.jpg)

(Ảnh bìa: Dưới đáy biển ngập tràn rác chai nhựa.)

Tôi đọc được một [báo cáo](https://news.nationalgeographic.com/2018/05/plastic-bag-mariana-trench-pollution-science-spd/) trên tạp chí *National Geographic*. Nơi sâu nhất trên Trái Đất là rãnh Mariana ở Thái Bình Dương, nằm sâu 11 km dưới mực nước biển. Năm 2016, một tàu ngầm thám hiểm đã lặn xuống đây và chụp một loạt ảnh gửi về. Mới đây, khi phân tích kỹ các bức ảnh này, các nhà khoa học phát hiện một vật thể trong suốt lơ lửng. Ban đầu họ đoán đó là một loài sinh vật biển sâu chưa từng được biết đến, nhưng sau đó đã xác thực: Đó là một chiếc túi nilon.

Nếu ngay cả nơi khó tiếp cận nhất trên bề mặt Trái Đất cũng đã xuất hiện rác thải của con người, thì không khó để tưởng tượng đại dương ngoài kia đang ngập trong rác đến mức nào! Tôi thường trăn trở, nhân loại thải ra lượng rác khổng lồ như vậy thì tương lai sẽ đi về đâu? Chỉ tính riêng việc mua sắm online hàng ngày đã sinh ra biết bao rác thải từ bao bì đóng gói. Mức tiêu dùng cá nhân của tôi thực tế rất ít, nhưng lượng rác thải sinh hoạt mỗi tháng cũng đủ để lấp đầy một thùng rác 0,5 mét khối.

Thực lòng mà nói, loài người hiện tại gần như bất lực trước vấn đề rác thải. Rác hữu cơ có thể đem đốt, còn các loại rác khác hiện nay hầu hết chỉ có thể đem chôn lấp. Do nước ta chưa áp dụng triệt để hệ thống phân loại rác thải tại nguồn nên [hơn 80%](http://www.wangqi19.com/NWCI/Files/J10.3_Cover/Introduction/Analysis%20of%20Landfills%20in%20China.pdf) lượng rác hiện nay được xử lý bằng cách chôn lấp trực tiếp. Bạn nghĩ rác được xe chở đi là đã biến mất sao? Không, chúng được chôn sâu xuống lòng đất, âm thầm ô nhiễm nguồn nước và đất đai, và cuối cùng con người sẽ là đối tượng gánh chịu hậu quả. Lượng rác khổng lồ thải ra mỗi ngày trên khắp cả nước đang được chôn giấu ở mọi ngóc ngách của đất nước, nghĩ đến thôi đã thấy vô cùng đáng sợ. Đáng sợ hơn là tư tưởng chủ đạo của xã hội hiện nay vẫn là chủ nghĩa tiêu dùng (tiêu dùng càng nhiều càng hạnh phúc), dẫn tới lượng rác thải trong tương lai sẽ chỉ có tăng chứ không giảm. Chúng ta đang tự hủy hoại tương lai của chính mình. We are doomed.

## 新闻 (Tin tức)

1、[Chính phủ Đức ban hành "Bộ quy tắc đạo đức cho thuật toán xe tự lái"](https://360.here.com/autonomous-cars-get-a-lesson-in-ethics)

Chính phủ Đức đã thiết lập "Yêu cầu đối với thuật toán tự lái", đưa ra một chuỗi các điều kiện pháp lý bắt buộc hệ thống xe tự lái phải tuân thủ khi vận hành:

* Khi xảy ra tai nạn, an toàn tính mạng con người là ưu tiên tuyệt đối cao hơn an toàn tài sản hoặc động vật.
* Khi xảy ra tai nạn, thuật toán không được phép có bất kỳ sự phân biệt đối xử nào dựa trên tuổi tác, giới tính, sắc tộc... (Nghĩa là xe tự lái không được phép lập trình để chọn đâm vào người già để tránh đâm vào trẻ em).
* Bắt buộc phải trang bị "hộp đen" lưu trữ toàn bộ lịch sử hành trình và dữ liệu vận hành.
* Trong các tình huống khẩn cấp, con người có quyền can thiệp và giành lại quyền kiểm soát phương tiện bất cứ lúc nào.

2、[Quy trình đăng ký tài khoản không cần mật khẩu tương lai của W3C](https://www.w3.org/TR/webauthn/)

Liên minh W3C đang thiết kế một tiêu chuẩn đăng ký tài khoản web dựa trên khóa bảo mật (WebAuthn). Trong tương lai, người dùng đăng ký tài khoản sẽ không cần đặt mật khẩu và không còn lo sợ nguy cơ bị rò rỉ hay hack mật khẩu.

Nguyên lý cơ bản: Khi đăng ký, trình duyệt sẽ tự động sinh ra một cặp khóa công khai (public key) và khóa bí mật (private key). Khóa công khai được gửi lên lưu trữ tại máy chủ dịch vụ, còn khóa bí mật được lưu trữ bảo mật ngay tại thiết bị cục bộ của người dùng. Khi đăng nhập, người dùng chỉ cần điền tên tài khoản, trình duyệt dùng khóa bí mật mã hóa yêu cầu gửi lên server, nếu máy chủ dùng khóa công khai giải mã thành công sẽ xác thực danh tính hợp lệ.

3、[Cấy ghép thành công buồng trứng in 3D sinh học hoạt động tốt trên chuột](https://www.smithsonianmag.com/smart-news/functional-3d-printed-ovary-transplanted-mice-180963337/?no-ist)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053002.jpg)

Các nhà khoa học Mỹ đã sử dụng công nghệ in 3D sinh học với chất liệu gelatin để chế tạo buồng trứng nhân tạo và cấy ghép thay thế buồng trứng tự nhiên của chuột. Kết quả thử nghiệm vô cùng kinh ngạc: 3 trong số 7 con chuột thí nghiệm đã sinh con hoàn toàn khỏe mạnh bình thường.

Những kịch bản viễn tưởng mô tả trong cuốn sách *Lược sử tương lai* (Homo Deus) đang dần thành hiện thực: Con người tương lai sẽ không còn là sản phẩm thuần tự nhiên nữa mà chuyển dịch sang dạng sinh vật bán tự nhiên, bán nhân tạo.

4、[Tốc độ phát triển chóng mặt của năng lực tính toán AI](https://blog.openai.com/ai-and-compute/?)

Nghiên cứu chỉ ra từ năm 2012, năng lực tính toán phục vụ huấn luyện các mô hình AI lớn tăng gấp đôi sau mỗi 3,5 tháng, tính đến nay đã tăng trưởng hơn 300.000 lần. Để so sánh, Định luật Moore (năng lực chip tăng gấp đôi sau mỗi 18 tháng) trở nên quá chậm chạp khi theo định luật này, năng lực tính toán chỉ tăng trưởng khoảng 12 lần trong cùng khoảng thời gian. Tốc độ tiến hóa của AI đang vượt xa trí tưởng tượng của con người.

5、[Nghiên cứu đặt giả thuyết bạch tuộc có nguồn gốc từ ngoài Trái Đất](http://bgr.com/2018/05/17/octopus-aliens-cephalopods-research-study/)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053003.jpg)

Một nhóm nghiên cứu đưa ra giả thuyết gây tranh cãi cho rằng các loài động vật chân đầu như bạch tuộc, mực có thể có nguồn gốc ngoài hành tinh do bộ gene của chúng vô cùng phức tạp và khác biệt hoàn toàn với tất cả các loài động vật khác trên Trái Đất. Giả thuyết cho rằng trứng hoặc phôi của chúng đã được bảo quản đông lạnh trong các lõi sao chổi băng va chạm với Trái Đất từ hàng triệu năm trước và phát triển thành loài bạch tuộc ngày nay để giải thích cho sự xuất hiện đột ngột của bộ não phức tạp, hệ thần kinh nhạy bén và khả năng ngụy trang đổi màu sắc siêu việt trong tiến hóa sinh học.

6、[Máy pha cà phê di động tiện dụng cho công trường](http://alphr.com/technology/1008859/makita-coffee-maker-drill-batteries)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053004.jpg)

Thói quen uống cà phê đang lan rộng từ giới lập trình viên và văn phòng sang các ngành nghề lao động chân tay ngoài trời. Hãng sản xuất dụng cụ điện cầm tay Makita của Nhật Bản đã giới thiệu dòng máy pha cà phê di động phục vụ cho công nhân xây dựng ngay tại công trường. Điểm độc đáo của máy là sử dụng chung pin lithium của các dòng máy khoan cầm tay Makita. Sau khi hoàn thành việc khoan cắt, công nhân có thể tháo pin lắp vào máy để pha được khoảng 5 cốc cà phê ấm nóng.

7、[Đạo luật GDPR chính thức có hiệu lực, Whois ẩn thông tin đăng ký](https://www.alibabacloud.com/zh/notice/yuming0525)

Đạo luật bảo vệ dữ liệu GDPR của EU chính thức có hiệu lực yêu cầu các dịch vụ không được phép chia sẻ hay công khai thông tin cá nhân của người dùng khi chưa được đồng ý. Hệ quả trực tiếp là cổng truy vấn thông tin chủ sở hữu tên miền Whois hiện nay đã ẩn toàn bộ thông tin tên tuổi, điện thoại, địa chỉ của người đăng ký và chỉ hiển thị thông tin chung của nhà đăng ký tên miền.

## FrontJS

Bản tin tuần này nhận được sự tài trợ của nền tảng giám sát lỗi frontend **FrontJS** ([www.frontjs.com](http://www.frontjs.com/?utm_source=ruanyf)).

[![](https://cdn.beekka.com/blogimg/asset/201806/bg2018060601.jpg)](https://www.frontjs.com/?utm_source=ruanyf)

FrontJS là giải pháp giám sát lỗi hiệu năng dành cho các ứng dụng Web và WeChat Mini Program, hỗ trợ tự động thu thập các lỗi console log / warn / error hiển thị trực quan cho nhà phát triển dễ dàng debug và tối ưu hóa hệ thống.

[![](https://cdn.beekka.com/blogimg/asset/201806/bg2018060602.jpg)](https://www.frontjs.com/?utm_source=ruanyf)

## 教程 (Hướng dẫn)

1、[Trang web] [DiscoverDev.io](https://www.discoverdev.io/) (Tiếng Anh)

Trang web tổng hợp và giới thiệu từ 5 đến 10 bài viết kỹ thuật công nghệ xuất sắc nhất hàng ngày.

2、[Khóa học] [Bộ video hướng dẫn Machine Learning thực tế của Facebook](https://research.fb.com/the-facebook-field-guide-to-machine-learning-video-series/) (Tiếng Anh)

Khóa học gồm 6 phần do đội ngũ kỹ sư tối ưu hóa quảng cáo bằng học máy của Facebook xây dựng, chia sẻ các kinh nghiệm thực tế tốt nhất khi ứng dụng thuật toán học máy giải quyết các bài toán kinh doanh thực tế.

3、[Bài viết] [Kiến thức cơ bản về khí áp và khí tượng học](https://www.thoughtco.com/low-and-high-pressure-1434434) (Tiếng Anh)

Giải thích cơ bản về áp suất khí quyển, sự chênh lệch khí áp tạo ra gió và bão nhiệt đới, cùng cơ chế hình thành các đới gió trên Trái Đất do chênh lệch nhiệt độ và áp suất giữa xích đạo và các cực.

4、[Tài liệu] [Bản dịch tiếng Trung của cuốn Flask Mega-Tutorial](https://github.com/luhuisicnu/The-Flask-Mega-Tutorial-zh) (Tiếng Trung)

Bộ tài liệu hướng dẫn cực kỳ chi tiết cách xây dựng ứng dụng web từ cơ bản đến nâng cao bằng Python và Flask framework.

5、[Danh sách] [arl: Xếp hạng các dự án nguồn mở hot nhất theo từng ngôn ngữ lập trình](https://github.com/kaxap/arl)

Bảng xếp hạng cập nhật các repository nhận được nhiều sao nhất trên GitHub phân loại theo ngôn ngữ lập trình.

6、[Tài liệu] [Quy chuẩn viết script Shell/Bash của Google](https://google.github.io/styleguide/shell.xml) (Tiếng Anh)

Do cú pháp script Shell rất lỏng lẻo dễ dẫn tới viết code lộn xộn khó đọc, tài liệu đưa ra các quy tắc viết code Bash chuẩn hóa của Google giúp bảo trì script tốt hơn.

7、[Bài viết] [Các trường HTTP Header dư thừa không cần thiết](https://www.fastly.com/blog/headers-we-dont-want) (Tiếng Anh)

Thống kê và đánh giá 30 trường HTTP header phổ biến để chỉ ra những trường nào thực sự cần thiết và những trường nào nên loại bỏ để tối ưu hóa băng thông truyền tải.

8、[Bài viết] [Hai giải pháp CSS dựng bảng hiển thị co giãn trên di động](http://lea.verou.me/2018/05/responsive-tables-revisited/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053008.jpg)

Chuyên gia CSS Lea Verou chia sẻ hai phương pháp sử dụng thuộc tính `text-shadow` hoặc hàm `element()` của CSS để nhân bản tiêu đề bảng và hiển thị bảng dạng key-value co giãn mượt mà trên di động mà không cần thêm thẻ HTML dư thừa.

## 工具 (Công cụ)

1、[DocHub](https://github.com/TruthHun/DocHub)

Hệ thống thư viện chia sẻ tài liệu trực tuyến nguồn mở tự phát triển mô phỏng theo mô hình của Baidu Wenku.

2、[ShellCheck](https://www.shellcheck.net/)

Công cụ phân tích tĩnh nguồn mở hỗ trợ phát hiện lỗi cú pháp và cảnh báo rủi ro cho các đoạn mã script Bash/Shell.

3、[Crunch](https://github.com/chrissimpkins/Crunch)

Công cụ dòng lệnh hỗ trợ tối ưu hóa và nén ảnh định dạng PNG đạt hiệu năng nén rất tốt mà không làm suy giảm chất lượng ảnh.

4、[nomulus](https://github.com/google/google/nomulus)

Hệ thống quản lý đăng ký tên miền cấp cao nhất (TLD registry) được Google mở nguồn, chính là hạ tầng chạy phía dưới của cổng đăng ký tên miền Google Registry.

5、[Termux](https://termux.com/)

Ứng dụng giả lập terminal Linux mạnh mẽ dành cho các thiết bị Android chạy offline không cần root máy.

6、[Material-UI v1.0.0](https://github.com/mui-org/material-ui/releases/tag/v1.0.0)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053009.jpg)

Thư viện React UI component mô phỏng theo ngôn ngữ thiết kế Material Design của Google chính thức phát hành phiên bản 1.0 hoạt động ổn định giúp xây dựng giao diện web mượt mà.

7、[tlsh-js](https://github.com/idealista/tlsh-js)

Thư viện JavaScript hỗ trợ sinh mã băm từ chuỗi văn bản với đặc tính: hai chuỗi có nội dung càng tương đồng thì mã băm sinh ra càng giống nhau, giúp so sánh nhanh độ tương đồng giữa hai văn bản.

8、[libui](https://github.com/andlabs/libui)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053010.jpg)

Thư viện giao diện đồ họa (GUI library) viết bằng C hỗ trợ đa nền tảng tốt để build app desktop native chạy đồng nhất trên Windows, macOS và Linux.

## 文摘 (Văn trích)

1、[Tài năng thiết kế đồ họa của nhà văn Lỗ Tấn](http://new.qq.com/omn/20180119/20180119A0VPMZ.html)

Bên cạnh sự nghiệp văn chương đồ sộ, nhà văn Lỗ Tấn còn là một nhà thiết kế đồ họa xuất sắc của thời kỳ Dân quốc. Thời chưa có phần mềm đồ họa máy tính, ông tự tay vẽ tay hầu hết bìa sách cho các tác phẩm của mình và bìa các tạp chí lớn, thể hiện tư duy nghệ thuật hiện đại qua các nét vẽ cách điệu chữ viết độc đáo.

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053011.jpg)

Bìa tác phẩm *Nghệ thuật luận* với chữ vẽ tay lồng ghép các họa tiết hình học trừu tượng hài hòa.

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053012.jpg)

Bìa cuốn *Nhi dĩ tập* với các đường nét phóng khoáng đầy tính nghệ thuật cổ nhã.

2、[Mô phỏng cơ chế Machine Learning qua 4 câu thoại](https://twitter.com/PPathole/status/995294997552381955)

> Người: 11 × 11 bằng bao nhiêu?
> Máy: 65
> Người: Sai bét, bằng 121 mới đúng. Thế rốt cuộc 11x11 bằng bao nhiêu?
> Máy: 121

3、[Phỏng vấn Hamano Junio — nhà duy trì chính của dự án Git](https://linux.cn/article-2052-1.html)

Sau khi Linus Torvalds bàn giao lại quyền quản lý Git, kỹ sư người Nhật Hamano Junio (làm việc tại Google) đã đảm nhận vai trò nhà duy trì chính (maintainer) của dự án. Ông chia sẻ lại những kỷ niệm thời kỳ đầu đóng góp mã nguồn cho Git và cơ chế viết code merge tinh tế của Linus.

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053013.jpg)

4、[Ý nghĩa của các thuật ngữ độ phân giải màn hình](https://medium.com/@yashwate07/explained-1-display-resolution-11a67a6096c)

* **720p**: 1280 x 720, tiêu chuẩn HD (High Definition)
* **1080p**: 1920 x 1080, tiêu chuẩn Full HD
* **1440p**: 2560 x 1440, tiêu chuẩn QHD (Quad HD - nét gấp 4 lần HD)
* **2160p**: 3840 x 2160, tiêu chuẩn 4K
* **4320p**: 7680 x 4320, tiêu chuẩn 8K

## 新奇 (Sự độc đáo)

1、[Nhịp đập Luân Đôn (London Tube Heartbeat)](http://tubeheartbeat.com/london/)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053014.jpg)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053015.jpg)

Dự án trực quan hóa dữ liệu lưu lượng hành khách di chuyển trên hệ thống tàu điện ngầm London theo thời gian thực, độ dày của các tuyến đường đại diện cho mật độ người đi lại co bóp nhịp nhàng sinh động hệt như nhịp đập trái tim của đô thị.

## 本周图片 (Hình ảnh tuần này)

1、[Sự thay đổi thiết kế nút bấm của trang web Dribbble](https://www.toptal.com/designers/ui/button-design-dribbble-timeline)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053016.jpg)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053017.jpg)

Sơ đồ tổng hợp sự thay đổi thiết kế nút bấm trên trang chủ Dribbble từ năm 2009 đến 2017 phản ánh xu hướng thiết kế giao diện dịch chuyển mạnh mẽ từ mô phỏng nổi khối 3D sang phong cách phẳng hóa tối giản hiện đại.

2、[Lệnh npm install trực quan hóa bằng hình ảnh](https://twitter.com/brad_frost/status/996014341592961025)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018053018.jpg)

Một bức ảnh hài hước mô tả cảnh tượng ổ cứng máy tính bị chất đầy đống lộn xộn các file rác sau khi chạy lệnh `npm install` để tải các thư viện node_modules.

## 本周金句 (Kim ngôn tuần này)

Việc đọc bao nhiêu sách cũng không thể so sánh với những thay đổi lớn lao mà động lực tự thân bên trong mang lại cho một con người.

(Hết)
