# 科技爱好者周刊（第 137 期）：Slack 被收购，以及企业的技术选型

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1520) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120908.jpg)

Vào ngày 3 tháng 12, một robot do các kỹ sư Ai Cập phát triển đang thực hiện quét siêu âm thử nghiệm cho bệnh nhân tại bệnh viện nhằm giảm thiểu tiếp xúc trực tiếp giữa bác sĩ và người bệnh. (Nguồn: [Tân Hoa Xã](http://www.xinhuanet.com/world/2020-12/07/c_1126831143_7.htm))

## 主带话题：Thương vụ Slack bị thâu tóm và câu chuyện lựa chọn công nghệ của doanh nghiệp

Slack là một phần mềm liên lạc và cộng tác nhóm vô cùng xuất sắc. Nếu bạn chưa từng sử dụng trong công việc, tôi rất khuyên bạn nên dùng thử.

Nó sở hữu lượng người dùng khổng lồ trên toàn cầu, với doanh thu năm ngoái đạt 833 triệu USD.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120807.jpg)

Tuần trước, Slack đã đồng ý bán mình cho Salesforce với mức giá khổng lồ lên tới 27,7 tỷ USD (khoảng 180 tỷ Nhân dân tệ). Từ đây, Slack sẽ không còn hoạt động như một công ty độc lập mà trở thành một bộ phận trực thuộc Salesforce.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120808.jpg)

Đây thực chất là một quyết định có phần bất ngờ. Trong bối cảnh dịch bệnh đang thúc đẩy mạnh mẽ xu hướng làm việc từ xa, Slack đang ở thời kỳ hoàng kim nhưng lại quyết định rút lui và bán mình thay vì tiếp tục phát triển độc lập như một siêu kỳ lân công nghệ. Tại sao vậy?

Nguyên nhân chủ chốt có lẽ là do áp lực cạnh tranh khủng khiếp từ **Microsoft Teams**. Đây là công cụ cộng tác nhóm do Microsoft phát triển nhằm cạnh tranh trực tiếp với Slack, và được tích hợp miễn phí vào bộ ứng dụng Office phổ cập khiến Slack chịu sức ép vô cùng lớn.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120809.jpg)

Được phát hành vào tháng 10 năm 2016, chỉ trong vòng 4 năm, lượng người dùng hoạt động hàng ngày của Teams đã tăng từ con số 0 lên tới 115 triệu. Trong cùng khoảng thời gian đó, lượng người dùng của Slack chỉ tăng từ 4 triệu lên 12 triệu. Nói cách khác, tốc độ tăng trưởng của Microsoft Teams nhanh gấp hơn mười lần so với Slack!

Điều này thực tế rất dễ hiểu. Đối với phần mềm doanh nghiệp, việc có một gã khổng lồ chống lưng phía sau sẽ tạo ra sự khác biệt hoàn toàn về doanh số bán hàng. Khi hai phần mềm có tính năng tương đương nhau, một bên do một startup cung cấp và bên kia do Microsoft hậu thuẫn tích hợp sẵn trong hệ thống mà doanh nghiệp đã mua bản quyền, doanh nghiệp sẽ chọn ai?

Trước đây có một giả thuyết cho rằng các lập trình viên tuyến đầu có thể tự do lựa chọn công cụ phát triển rồi thúc đẩy "từ dưới lên" để toàn bộ doanh nghiệp áp dụng theo. Tôi cũng từng tin vào điều đó. Nhưng thực tế thì giả thuyết này rất phi thực tế: **Các lập trình viên trực tiếp viết code không có quyền quyết định mua sắm phần mềm hay lựa chọn công nghệ của doanh nghiệp, còn những người có quyền quyết định thì luôn e ngại việc phải chịu trách nhiệm nếu quyết định đó sai lầm.** Nếu bạn lựa chọn một phần mềm nhỏ từ một startup, vạn nhất nó xảy ra sự cố ngừng hoạt động hoặc bị lỗi bảo mật ảnh hưởng đến kinh doanh, người ra quyết định sẽ phải chịu trách nhiệm hoàn toàn.

**Trong ngành phần mềm có một câu nói nổi tiếng: "Không ai bị sa thải vì lựa chọn Java".** Lựa chọn những công nghệ có sự bảo chứng từ các tập đoàn lớn như Oracle, Microsoft, IBM sẽ mang lại sự an tâm tuyệt đối cho doanh nghiệp. Những công nghệ đó có thể không quá tiên tiến, không hoàn hảo hay thậm chí rất nhàm chán, nhưng nó đảm bảo luôn được duy trì tích cực, sở hữu hệ sinh thái và cộng đồng khổng lồ, và đã được kiểm chứng qua các hệ thống lớn chịu tải cao. Doanh nghiệp luôn ưu tiên các công nghệ an toàn như vậy để hạn chế tối đa rủi ro.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120810.jpg)

Microsoft đổ nguồn lực khổng lồ đi kèm đội ngũ bán hàng chuyên nghiệp để tiếp thị Teams, Slack làm sao có thể tự mình cạnh tranh lại! Và cũng không phải ngẫu nhiên khi Slack chọn bán mình cho Salesforce - doanh nghiệp tuy có năng lực công nghệ chưa phải hàng đầu thế giới nhưng chắc chắn là một trong những công ty có năng lực bán hàng phần mềm doanh nghiệp mạnh nhất hành tinh.

Tương tự như vậy đối với mảng phát triển Front-end. Doanh nghiệp chọn các framework JS ít tên tuổi sẽ gánh nhiều rủi ro, và có thể dự đoán rằng kẻ chiến thắng cuối cùng ở quy mô doanh nghiệp vẫn là React. React là thư viện Front-end số 1 thế giới được chống lưng bởi Meta (Facebook), vì vậy "không ai bị sa thải vì lựa chọn React".

## Khóa học "Tối ưu hóa hiệu năng Front-end"

Tối ưu hóa hiệu năng thường là mảng kiến thức nâng cao trong phát triển phần mềm, thuộc nhóm yêu cầu dành cho các lập trình viên Front-end cấp cao. Một mặt, bạn cần đảm bảo hệ thống chạy đúng tính năng và bảo mật trước khi tối ưu hiệu năng; mặt khác, chỉ khi hiểu rõ các chi tiết vận hành ở tầng dưới (như cơ chế hoạt động của trình duyệt, luồng xử lý mạng) bạn mới có thể tối ưu hiệu năng hiệu quả.

Do đó, nắm vững kỹ năng tối ưu hóa hiệu năng sẽ là điểm cộng cực kỳ lớn khi phỏng vấn tăng lương và mở rộng không gian phát triển sự nghiệp của bạn.

Tuần này, chúng tôi chia sẻ khóa học video **《Tối ưu hóa hiệu năng Front-end chuyên sâu》** do thầy Đại Thánh giảng dạy. Thầy là cựu kiến trúc sư cao cấp tại Baidu và 360, hiện đang công tác tại Kaikeba.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120903.jpg)

Khóa học sẽ phân tích chi tiết các câu hỏi phỏng vấn tối ưu hóa hiệu năng tần suất cao như: Luồng xử lý chi tiết của trình duyệt sau khi gõ URL, cách rút ngắn thời gian tải trang đầu tiên (FCP)... Thầy cũng sẽ hướng dẫn các phương án tối ưu hóa hiệu năng thực chiến có thể áp dụng ngay vào dự án của bạn, đồng thời chia sẻ kinh nghiệm cá nhân giúp nâng cao năng lực cạnh tranh lõi để nâng mức lương từ khởi điểm 2 triệu đồng lên mức 40 triệu đồng.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120906.jpg)

Khóa học video kéo dài 325 phút với nhiều nội dung thực tế trị giá 699 tệ hiện dành tặng riêng **200 suất học miễn phí (0 tệ)** cho độc giả của bản tin. Bạn chỉ cần quét mã QR dưới đây để nhận tài liệu (không yêu cầu chia sẻ hay giới thiệu):

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120905.jpg)

## Tin tức

1、[Mẫu máy tính xách tay trang bị tới 7 màn hình](https://expanscape.com/the-aurora-7-prototype/the-story-of-the-aurora-7/)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112506.jpg)

Một công ty của Anh vừa chế tạo thành công mẫu máy tính xách tay tích hợp đầy đủ các trang bị phần cứng khủng nhất của một máy trạm:
- Trang bị tới 7 màn hình hiển thị (trong đó có 4 màn hình kích thước 17 inch độ phân giải 4K).
- Tích hợp 4 cổng mạng (gồm 2 cổng mạng không dây độc lập).
- Bàn phím cơ 104 phím có đèn nền.
- Bộ nhớ RAM lên tới 128GB.
- Ổ cứng lưu trữ SSD dung lượng 16TB.
- Màn hình phụ hiển thị trạng thái hệ thống riêng biệt.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112507.jpg)

Thiết bị hiện ở dạng nguyên mẫu thử nghiệm (prototype) chưa công bố giá bán thương mại. Điểm hạn chế lớn nhất của nó là trọng lượng nặng tới 10kg.

2、[Tàu thăm dò Hayabusa-2 của Nhật Bản mang mẫu đá tiểu hành tinh về Trái Đất](https://www.bbc.com/news/science-environment-55201662)

Tháng 12 năm 2014, Nhật Bản phóng tàu thăm dò không người lái Hayabusa-2 hướng tới tiểu hành tinh Ryugu và tiếp cận mục tiêu vào năm 2018.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120516.jpg)

Năm 2019, tàu đáp xuống bề mặt tiểu hành tinh Ryugu và thực hiện bắn một viên đạn kim loại xuống mặt đất Ryugu để tạo ra một hố va chạm nhân tạo nhằm thu thập các mẫu đá nằm sâu dưới lòng đất chưa bị bức xạ vũ trụ làm thay đổi.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120517.jpg)

Ngày 6 tháng 12 năm 2020, cabin chứa mẫu vật được tàu thả rơi tự do xuống bầu khí quyển Trái Đất và đáp an toàn bằng dù xuống vùng sa mạc phía nam nước Úc, mang về thành công mẫu vật tiểu hành tinh đầu tiên cho nhân loại.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120519.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120518.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120520.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120521.jpg)

Hiện tại, tàu Hayabusa-2 tiếp tục hành trình bay tới một tiểu hành tinh khác để thực hiện nhiệm vụ tiếp theo dự kiến kéo dài đến năm 2031.

3、[Hệ thống camera AI giám sát việc xích chó khi dạo phố](http://static.zhoudaosh.com/6C13A88B1564424729BF877958D0D98C4B39F14DC8C71DB570EAB0B4546D7E8F)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120112.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120113.jpg)

Quy định nuôi chó của thành phố Thượng Hải bắt buộc chủ nuôi phải xích chó khi ra đường, nếu vi phạm sẽ bị xử phạt. Mới đây, Công an quận Hồng Khẩu đã triển khai thí điểm hệ thống camera giám sát thông minh tại nhiều khu dân cư để phát hiện lỗi vi phạm này.

Hệ thống AI sẽ tự động khoanh vùng vật nuôi xuất hiện trong khung hình, sau đó phân tích tần suất di chuyển cùng hướng của những người đi bên cạnh để xác định chính xác chủ sở hữu của chú chó. Hệ thống tự động trích xuất hình ảnh gửi về cho cảnh sát khu vực để tiến hành phạt nguội chủ nuôi. Hệ thống này cũng có thể nhận diện và theo dõi các chú chó đi lạc để thu gom về trung tâm cứu hộ.

4、[Trục vớt tàu chở xe hơi lật úp ngoài khơi Mỹ](https://jalopnik.com/a-chain-just-cut-through-a-capsized-cargo-ship-filled-w-1845784581)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120304.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120305.jpg)

Tháng 9 năm 2019, một con tàu chở xe hơi dài 200 mét chở theo 4.000 chiếc ô tô mới đã bị lật úp ngoài khơi bang Georgia, Mỹ. Mới đây, đội trục vớt đã tiến hành cắt đôi thân tàu để nâng từng phần lên xà lan cứu hộ tạo nên cảnh tượng vô cùng ấn tượng.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120307.jpg)

Phần thân tàu bị cưa đứt lộ ra hàng trăm chiếc ô tô bên trong đã bị ép bẹp rúm do lực ép và nước biển ăn mòn.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120308.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120309.jpg)

5、**Tin tức một câu**

> - [Microsoft](https://gear.xbox.com/products/windows-95-ugly-sweater) mở bán mẫu áo len dệt họa tiết Windows 95 trên cửa hàng Xbox Store với giá 69,99 USD, thiết kế màu lam sọc trắng mô phỏng hình ảnh bầu trời xanh mây trắng của hình nền mặc định Windows 95 huyền thoại.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120513.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120514.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120515.jpg)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020121006.jpg)

> - [Thiết bị lò phản ứng hạt nhân mô phỏng Mặt Trời nhân tạo](https://www.sohu.com/a/436289282_114986) "Huanliu-2M" của Trung Quốc đã thực hiện thành công lần phóng điện đầu tiên tại Thành Đô, đánh dấu bước phát triển trong nghiên cứu công nghệ năng lượng hạt nhân thế hệ mới.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120503.jpg)

> - [Singapore](https://edition.cnn.com/2020/12/02/business/lab-grown-chicken-intl-scli-scn/index.html) trở thành quốc gia đầu tiên trên thế giới phê duyệt cho phép thương mại hóa sản phẩm "thịt gà nhân tạo" được nuôi cấy trực tiếp từ các tế bào thịt gà trong phòng thí nghiệm.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120402.jpg)

> - [Hãng hàng không Lufthansa](https://edition.cnn.com/travel/article/lufthansa-sleepers-row-lie-flat-economy-seat/index.html) triển khai dịch vụ "giường nằm kinh tế" bằng cách cho phép hành khách mua thêm một hàng ghế trống với giá 260 USD để gạt tay vịn và nằm thẳng lưng trong các chuyến bay dài vắng khách.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112801.jpg)

> - [Một nông dân Indonesia](https://www.bbc.com/news/world-asia-55013725) bỗng chốc đổi đời khi một mảnh thiên thạch hiếm carbon nặng khoảng 2kg rơi thủng mái nhà của anh và được một nhà sưu tập Mỹ mua lại với mức giá ước tính lên tới hơn 1 triệu USD.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112209.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112205.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112206.jpg)

> - [Một kỹ sư Thụy Điển](https://www.boredpanda.com/magpies-recycling-machine-bottle-caps/) đã thiết kế một máy cấp thức ăn tự động cho chim ác là, máy sẽ nhả hạt thức ăn mỗi khi chú chim ngậm nắp chai nhựa hoặc rác bỏ vào khay thu hồi.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112301.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112303.jpg)

## Bài viết

1、[Ngành sản xuất máy công cụ Trung Quốc đi về đâu?](https://finance.sina.com.cn/stock/s/2020-12-06/doc-iiznctkc5115023.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120702.jpg)

Năm 2012, Shenyang Machine Tool từng đứng số 1 thế giới về sản lượng bán ra nhưng nay đã tuyên bố phá sản. Hơn 18 doanh nghiệp máy công cụ (máy tiện CNC) lớn của Trung Quốc hầu như đều sa sút nghiêm trọng và hiện tại hơn 90% dòng máy CNC cao cấp phục vụ sản xuất chính xác của nước này vẫn phụ thuộc hoàn toàn vào nhập khẩu. Bài viết phân tích sâu nguyên nhân dẫn đến thực trạng này.

2、[Đánh giá và chạy thử các dịch vụ chơi game đám mây Cloud Gaming trên Linux](https://boilingsteam.com/cloud-gaming-services-explained-and-tested-on-linux/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120111.jpg)

Cloud Gaming chạy trực tiếp game trên máy chủ Cloud và truyền hình ảnh về thiết bị khách. Bài viết đánh giá trải nghiệm thực tế các dịch vụ Google Stadia, Amazon Luna, Geforce Now trên hệ điều hành Linux.

3、[Các công trình kiến trúc đạt giải thưởng thiết kế Trung Quốc năm 2020](https://www.allnow.com/post/5fcdfff5c84b905ab2b38373)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120918.jpg)

Giới thiệu các thiết kế kiến trúc độc đáo đạt giải thưởng thiết kế quốc gia do Bảo tàng Nghệ thuật Đương đại Thượng Hải trao tặng. Hình ảnh trên là công trình thư viện cộng đồng tự nhiên được xây dựng bằng vật liệu gỗ đá địa phương tại ngôi làng cổ Chiết Thủy, Sơn Tây.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120917.jpg)

4、[6 cấu trúc mạng thần kinh nhân tạo cơ bản mà kỹ sư dữ liệu cần biết](https://lionbridge.ai/articles/6-types-of-neural-networks-every-data-scientist-must-know/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120203.jpg)

Bài viết giới thiệu về cấu trúc và nguyên lý hoạt động của 6 mạng Neural cơ bản nhất trong Machine Learning, mở đầu là mô hình sơ khởi Perceptron (nhận thức đơn tầng).

5、[Tìm hiểu các giao thức mạng phi tập trung đằng sau Dweb](https://blog.space.storage/posts/the-dweb-protocols-behind-space)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120401.jpg)

Dweb (Decentralized Web) hướng tới mô hình internet phân tán loại bỏ vai trò của các máy chủ trung tâm. Bài viết giới thiệu cấu trúc các giao thức mạng lõi hỗ trợ cho mô hình này như IPFS, Libp2p.

6、[Các quy tắc phòng chống tấn công XSS khi lập trình React](https://react.christmas/2020/3)（Tiếng Anh）

Mặc dù React được tích hợp sẵn cơ chế tự động escape chuỗi để chống lỗi bảo mật chèn mã độc XSS, lập trình viên vẫn cần lưu ý các kịch bản nguy hiểm khi sử dụng thuộc tính `dangerouslySetInnerHTML` hoặc truyền link URL động vào thẻ `href`.

7、[Chia sẻ kinh nghiệm phỏng vấn vị trí SRE tại Google London](https://justyy.com/archives/45126)（Tiếng Trung）

Bài viết chia sẻ thực tế của một kỹ sư về quy trình phỏng vấn kỹ thuật vị trí Site Reliability Engineer tại văn phòng Google London, phân tích cấu trúc câu hỏi thuật toán và cấu trúc hệ thống. ([@DoctorLai](https://github.com/ruanyf/weekly/issues/1535) đóng góp)

8、[Viết chữ dọc kết hợp số ngang bằng CSS](http://www.deathghost.cn/article/css/86)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120901.jpg)

Mẹo sử dụng thuộc tính CSS `writing-mode` và `text-combine-upright` để hiển thị chữ tiếng Trung theo hàng dọc đồng thời giữ các chữ số hiển thị theo hàng ngang (hình trên). ([@232650413](https://github.com/ruanyf/weekly/issues/1531) đóng góp)

9、[Cách cấu hình Google Analytics theo dõi truy cập không dùng Cookie](https://evrim.io/using-google-analytics-without-gdpr-consent/)（Tiếng Anh）

Để tuân thủ các quy định bảo mật GDPR nghiêm ngặt, bài viết hướng dẫn giải pháp phân biệt người dùng ghé thăm website thông qua việc tạo chuỗi mã hóa dấu vân tay trình duyệt (browser fingerprinting) thay thế cho việc ghi cookie thông thường.

10、[20 quan điểm lập trình gây tranh cãi nhiều nhất trên StackOverflow](https://programmers.blogoverflow.com/2012/08/20-controversial-programming-opinions/)（Tiếng Anh）

Tổng hợp các thảo luận nhận được nhiều ý kiến trái chiều nhất của cộng đồng lập trình viên trên StackOverflow, ví dụ như lập luận: "Việc sử dụng rập khuôn các mẫu thiết kế (Design Patterns) đôi khi gây hại nhiều hơn lợi cho cấu trúc mã nguồn".

## 工具

1、[nonstop](https://github.com/yuxiaoy1/nonstop)

Tiện ích mở rộng trình duyệt giúp tự động bỏ qua các trang trung gian cảnh báo xác nhận link ngoài của Zhihu, Weibo, Jianshu để chuyển hướng trực tiếp người dùng đến trang đích. ([@Yuxiaoy1](https://github.com/ruanyf/weekly/issues/1525) đóng góp)

2、[screenity](https://github.com/alyssaxuu/screenity)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120201.jpg)

Một extension ghi màn hình cực kỳ mạnh mẽ dành cho Chrome, hỗ trợ vẽ ghi chú, chèn hình webcam trực tiếp lên video khi đang quay. ([@jeff-fe](https://github.com/ruanyf/weekly/issues/1527) đóng góp)

3、[texme](https://github.com/susam/texme)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120202.jpg)

Một thư viện JavaScript siêu gọn nhẹ hỗ trợ tự động kết xuất mã nguồn markdown có chứa công thức toán học LaTeX trực tiếp thành trang HTML hoàn chỉnh. ([@baddate](https://github.com/ruanyf/weekly/issues/1530) đóng góp)

4、[dumpster-fire](https://hey.science/dumpster-fire/)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112503.jpg)

Một trang web giải trí độc đáo: Bạn gửi một email tới hòm thư của trang web, hệ thống sẽ tự động in nội dung email đó ra giấy và ném vào thùng rác đang bốc cháy trên sóng livestream thời gian thực.

5、[buster](https://github.com/dessant/buster)

Extension trình duyệt hỗ trợ vượt qua các mã xác nhận reCAPTCHA dạng hình ảnh bằng cách sử dụng công nghệ nhận dạng giọng nói tự động của file âm thanh đi kèm.

6、[ruffle](https://ruffle.rs/)

Trình giả lập trình phát Flash viết bằng ngôn ngữ Rust thông qua WebAssembly, giúp các trang web hiện đại tiếp tục chạy được các tệp tin game và hoạt họa Flash cũ sau khi Adobe Flash Player bị khai tử.

7、[twtxt](https://github.com/jointwt/twtxt)

Dự án mã nguồn mở cho phép người dùng tự lưu trữ và vận hành một nền tảng blog cá nhân phi tập trung gọn nhẹ, trao đổi cập nhật thông tin thông qua tệp tin văn bản tĩnh.

8、[Cyberbrain](https://github.com/laike9m/Cyberbrain)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112907.jpg)

Extension dành cho VS Code hỗ trợ tạo môi trường debug trực quan hóa đường chạy của các biến số và luồng xử lý dữ liệu trong Python.

9、[repl.it Multiplayer](https://repl.it/site/multiplayer)

Nền tảng hỗ trợ lập trình viên cùng thao tác viết code và biên dịch chạy chương trình trực tiếp trên trình duyệt theo thời gian thực (collaborative programming).

10、[RegExper](https://regexper.com/)

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120108.jpg)

Công cụ trực tuyến giúp chuyển đổi các biểu thức chính quy (Regular Expression) phức tạp thành các sơ đồ luồng hình ảnh trực quan giúp dễ dàng đọc hiểu.

## Tài nguyên

1、[This X Does Not Exist](https://thisxdoesnotexist.com/)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112204.jpg)

Trang web tổng hợp danh sách các dự án ứng dụng trí tuệ nhân tạo (GAN) để sinh ảnh giả lập siêu thực: Người không có thật, mèo không có thật, thiết kế phòng không có thật...

2、**Các trang web hiển thị ảnh vẽ vô cực zoom-in không điểm dừng**
- [Zoomquilt](https://zoomquilt.org/)
- [Zoomquilt2](http://zoomquilt2.com/)
- [Arkadia Zoomquilt](http://arkadia.xyz/)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112401.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112402.jpg)

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112403.jpg)

3、[Unix 操作系统简介](https://chsasank.github.io/classic_papers/unix-time-sharing-system.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020111502.jpg)

Bản dịch bài viết nghiên cứu khoa học lịch sử năm 1974 của hai cha đẻ hệ điều hành Unix là Dennis Ritchie và Ken Thompson giải thích các triết lý thiết kế cốt lõi của Unix.

4、[File Formats Wiki](http://fileformats.archiveteam.org/wiki/Main_Page)

Trang thư viện bách khoa toàn thư tra cứu cấu trúc dữ liệu, tiêu chuẩn hiển thị và cách đọc ghi của mọi định dạng phần mở rộng file trên máy tính.

5、[Hello DNS](https://powerdns.org/hello-dns/)

Tài liệu tiếng Anh hướng dẫn từ cơ bản đến nâng cao về cấu trúc hoạt động và các bản ghi thông tin của hệ thống tên miền DNS.

6、[Maven 手册](https://www.yuque.com/inuter/bc7ikc/ngeqot)

Tài liệu tiếng Trung hướng dẫn sử dụng công cụ quản lý dự án và xây dựng mã nguồn Maven dành cho lập trình viên Java. ([@inuter](https://github.com/ruanyf/weekly/issues/1538) đóng góp)

## Hình ảnh

1、[Đài tưởng niệm "Thư viện trống" tại Berlin](https://en.wikipedia.org/wiki/The_Empty_Library)

Tại quảng cáo Bebelplatz ở Berlin, Đức có một tác phẩm nghệ thuật sắp đặt độc đáo tên là "Thư viện trống" gồm các kệ sách bằng gỗ sơn trắng trống rỗng đặt ngầm dưới lòng đất nhìn qua lớp kính trong suốt trên mặt đường. Công trình nhằm nhắc nhở mọi người về sự kiện phát xít Đức đã tổ chức đốt hơn 20.000 cuốn sách của các nhà văn Do Thái và tác phẩm triết học Marx tại chính quảng trường này vào năm 1933.

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020052601.jpg)

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020052602.jpg)

2、[Trò đùa ngày Cá tháng Tư núi lửa phun trào lớn nhất lịch sử](http://hoaxes.org/af_database/permalink/the_eruption_of_mount_edgecumbe/)

Sáng ngày 1 tháng 4 năm 1974, người dân tại thị trấn Sitka thuộc đảo Alaska thức dậy và hốt hoảng khi thấy ngọn núi lửa Edgecumbe vốn ngủ yên 400 năm qua bất ngờ bốc khói đen kịt báo hiệu sắp phun trào.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120101.jpg)

Khi lực lượng tuần duyên phái trực thăng tiếp cận đỉnh núi để khảo sát tình hình sơ tán, họ phát hiện ra đây thực chất là một trò đùa Cá tháng Tư quy mô lớn do một người dân địa phương dàn dựng. Anh đã thuê trực thăng chở 70 lốp xe cũ lên miệng núi lửa, đổ dầu hỏa và châm lửa đốt tạo khói đen giả lập.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120102.jpg)

## Bài đọc thêm

### 1. Vụ ám sát nhà khoa học hạt nhân Iran bằng súng máy AI điều khiển qua vệ tinh

Vụ ám sát nhà khoa học hạt nhân hàng đầu Iran Mohsen Fakhrizadeh diễn ra vào ngày 27 tháng 11 vừa qua chứa đựng nhiều tình tiết như trong phim viễn tưởng. Mặc dù đi cùng đội bảo vệ 11 người trên xe chống đạn, ông vẫn bị sát hại bởi một khẩu súng máy thông minh điều khiển từ xa qua vệ tinh.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120803.jpg)

Đại diện Lực lượng Vệ binh Cách mạng Hồi giáo Iran tiết lộ chi tiết: Chiếc xe của ông Fakhrizadeh bất ngờ bị trúng đạn nhẹ, ông nghĩ xe gặp sự cố nên bước xuống kiểm tra. Ngay lập tức, một khẩu súng máy tự động lắp trên thùng một chiếc xe bán tải Nissan đỗ cách đó 150 mét bắt đầu nổ súng.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120804.jpg)

Khẩu súng máy được tích hợp camera nhận diện khuôn mặt bằng AI chỉ nhắm bắn chính xác vào mặt ông Fakhrizadeh với 13 phát đạn. Vợ ông ngồi bên cạnh chỉ cách 25cm hoàn toàn không bị trầy xước. Toàn bộ vụ ám sát diễn ra trong vòng 3 phút bằng tín hiệu điều khiển vệ tinh không có bóng dáng sát thủ tại hiện trường. Sau khi hoàn thành nhiệm vụ, chiếc xe bán tải chứa súng máy tự động kích nổ bom tự hủy để xóa dấu vết.

![](https://cdn.beekka.com/blogimg/asset/202012/bg2020120805.jpg)

### 2. Trải nghiệm game cô đơn: Nếu một đêm đông bạn ở khu chung cư ngoại ô nước Nga

Năm ngoái, hai lập trình viên người Nga đã phát hành một tựa game vô cùng đặc biệt tên là **It's Winter**.

Tựa game hoàn toàn không có cốt truyện, không có nhiệm vụ, không có kẻ thù và thậm chí không có bất kỳ nhân vật nào khác ngoài người chơi. Game chỉ tập trung vào việc mô phỏng chân thực bầu không khí cô tịch của một đêm đông phủ đầy tuyết trắng tại một khu chung cư kiểu cũ ở ngoại ô nước Nga.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112910.jpg)

Người chơi bắt đầu trò chơi trong một căn hộ nhỏ ấm cúng nhưng trống trải. Bạn có thể bật tắt đèn bếp, nướng vài lát bánh mì, luộc một quả trứng.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112911.jpg)

Nhìn ra ngoài cửa sổ kính là khoảng sân chung phủ đầy tuyết trắng xóa tĩnh lặng dưới ánh đèn đường leo lét.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112912.jpg)

Bạn có thể xách túi rác đi xuống cầu thang, bước ra khoảng sân vắng tanh không một bóng người dạo chơi. Các cửa hàng làm tóc và tạp hóa ở góc phố đều đã khóa cửa im lìm. Game mang tính chất một không gian "sandbox" mang lại trải nghiệm trầm buồn về cuộc sống đơn điệu của những chung cư hậu Xô Viết: "Không có gì chờ đợi bạn, không có cơ hội rời đi, không có phiêu lưu và cũng không có điều gì bất ngờ xảy đến." Game hiện được bán trên Steam với giá khoảng 37 Nhân dân tệ.

![](https://cdn.beekka.com/blogimg/asset/202011/bg2020112909.jpg)

## 言论

1、

Độ dày tài liệu đặc tả kỹ thuật của giao thức DNS liên tục phình to trong 30 năm qua với tốc độ trung bình tăng thêm 1 trang sau mỗi 2 ngày. Hiện nay tài liệu DNS đã lên tới hàng nghìn trang văn bản kỹ thuật dày đặc khiến không một lập trình viên nào có thể đọc hết toàn bộ trước khi bắt tay vào code. Độ phức tạp của DNS hiện đã vượt quá giới hạn nhận thức của một cá nhân, đồng nghĩa việc tự phát triển một trình phân giải DNS hoàn toàn mới từ đầu là điều gần như bất khả thi.

-- [《放牧 DNS 骆驼》](https://www.ietf.org/blog/herding-dns-camel/)

2、

Dù bạn có thông minh hay giàu kinh nghiệm đến đâu, phần lớn các ý tưởng thiết kế sản phẩm ban đầu của bạn đều sẽ không hoạt động tốt. Một ý tưởng tuyệt vời luôn cần rất nhiều thời gian và sự kiên trì cải tiến lặp đi lặp lại để trở thành một sản phẩm thực tế được thị trường chấp nhận.

-- [《Làm sao để trở thành nhà sáng lập hiểu người dùng》](https://mgadams.com/the-founders-guide-to-actually-understanding-users-c68feaecac44)

3、

Những người từng bơi vượt eo biển Anh chia sẻ rằng giai đoạn khó khăn nhất chính là chặng cuối cùng: Khi bạn đã nhìn thấy bờ cát của đất liền ngay trước mắt nhưng thực tế bạn vẫn phải bơi thêm một quãng đường rất dài nữa mới có thể chạm chân tới đích. Quá trình phát triển các tính năng phần mềm mới cũng tương tự như vậy.

-- Bài viết 《Nỗi đau khi phát triển tính năng mới》

4、

Cách tốt nhất để nâng cao tỷ lệ bao phủ kiểm thử (Test Coverage) cho dự án phần mềm không phải là viết thêm test case, mà là tiến hành rà soát và xóa bỏ những đoạn mã code thừa thãi không thực sự cần thiết trong hệ thống.

-- [《Huyền thoại về độ bao phủ code》](https://preslav.me/2020/12/03/the-myth-of-code-coverage/)

5、

Một quy luật chung của ngành công nghệ: Các công nghệ đỉnh cao thường bị thay thế rất nhanh nên có vòng đời sử dụng ngắn; ngược lại, các công nghệ lỗi thời nhưng có giá thành cực kỳ rẻ lại có sức sống bền bỉ và tiếp tục tồn tại suốt hàng thập kỷ.

-- [《Tương lai của hệ điều hành Linux 32-bit》](https://lwn.net/SubscriberLink/838807/9b293f03c03ef0c5/)

## Nhìn lại

Tuần này năm 2019 (số 86): [Tuyệt đối đừng theo đuổi chủ nghĩa hoàn hảo](http://www.ruanyifeng.com/blog/2019/12/weekly-issue-86.html)

![](https://cdn.beekka.com/blogimg/asset/201911/bg2019112713.jpg)

Tuần này năm 2018 (số 34): [Giải pháp tối hậu cho thẻ căn cước: Cấy chip thông minh dưới da](http://www.ruanyifeng.com/blog/2018/12/weekly-issue-34.html)

![](https://cdn.beekka.com/blogimg/asset/201812/bg2018120702.jpg)

## Đăng ký

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
