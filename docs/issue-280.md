# Bản tin chia sẻ công nghệ (Số 280): Gọi món bằng máy và văn hóa khép kín

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3684) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112005.webp)

Nhà triển lãm Quy hoạch Đô thị mới Khải Châu ở Đức Dương, Tứ Xuyên đã thiết kế một hành lang đi xuyên qua tòa nhà, kéo dài từ đầm sen đến tận đỉnh núi phía sau. Để phục vụ ý tưởng này, một khoảng trống lớn đã được mở ra ngay giữa tòa nhà nhằm nhấn mạnh sự giao hòa giữa con người và thiên nhiên. (Nguồn: [Archiposition](https://www.archiposition.com/items/20201123014453))

## 机器点餐与宅文化

Các cửa hàng đồ ăn nhanh hiện nay đều đã trang bị máy gọi món tự động.

Bạn có thể chọn gọi món trực tiếp tại quầy, hoặc sử dụng máy gọi món.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112404.webp)

Giả sử cả hai phương án đều tiện lợi như nhau (không phải xếp hàng), **bạn sẽ ưu tiên lựa chọn cách nào: Gọi món tại quầy hay dùng máy tự động?**

Câu hỏi này được đặt ra bởi [một lập trình viên người Hà Lan](https://willem.com/blog/2023-10-13_hello-stranger/). Một ngày nọ, khi đang ăn trưa tại một nhà hàng ở Amsterdam, anh tình cờ quan sát thấy những vị khách mới bước vào nhà hàng có xu hướng thích gọi món qua máy tự động hơn.

Mặc dù quầy thanh toán chỉ cách đó vài bước chân và họ hoàn toàn có thể trao đổi trực tiếp với nhân viên, những người này vẫn chọn đứng trước màn hình máy tự động.

Người lập trình này đã trầm ngâm suy nghĩ: **Liệu đây có phải là một xu hướng phổ biến, khi con người ngày nay thích tương tác với máy móc hơn là giao tiếp với đồng loại?**

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112406.webp)

Cuối cùng, anh rút ra kết luận rằng việc gọi món qua máy tự động mang lại rất nhiều lợi ích vượt trội, khiến mọi người tự nhiên ưu tiên lựa chọn phương án này:

> **(1) Quy trình được chuẩn hóa**. Từng bước trên máy gọi món đều được thiết kế rõ ràng, bạn sẽ không gặp khó khăn khi thao tác và mọi món ăn đều có mô tả chi tiết kèm hình ảnh minh họa.
> 
> **(2) Hiệu suất cao hơn**. Gọi món trực tiếp yêu cầu bạn phải trò chuyện với nhân viên, để tránh sai sót đôi khi bạn phải nhấn mạnh và nhắc lại nhiều lần, điều này làm chậm tiến độ. Chưa kể đôi lúc hai bên còn nghe không rõ lời nhau.
> 
> **(3) Trải nghiệm tốt hơn**. Khi sử dụng máy, bạn có đủ thời gian để suy nghĩ và đắn đo mà không sợ bị người khác hối thúc; dù có gọi những món ăn kết hợp kỳ lạ, bạn cũng không phải nhận những ánh nhìn dò xét từ nhân viên; nếu lỡ chọn sai, bạn có thể dễ dàng hủy bỏ và làm lại vô số lần mà không hề cảm thấy ngại ngùng.

Chính vì những lý do trên, việc mọi người thích tương tác với máy gọi món hơn là giao tiếp với nhân viên nhà hàng là điều hoàn toàn dễ hiểu.

**Tâm lý e ngại giao tiếp này của người dùng, cộng hưởng với sự phát triển của công nghệ thông tin, đã làm sụt giảm nhanh chóng tần suất giao tiếp trực tiếp giữa con người với nhau**, nhường chỗ cho các hoạt động tương tác giữa người và máy móc: Người giao hàng được thay thế bằng tủ khóa thông minh, nhà hàng được thay thế bằng các ứng dụng đặt đồ ăn, các lớp học trực tiếp được thay bằng các video bài giảng phát trực tuyến...

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112711.webp)

**Một biểu hiện rõ nét nhất của việc sụt giảm giao tiếp trực tiếp chính là sự trỗi dậy của "Văn hóa khép kín" (宅文化 - Hikikomori/Otaku)**.

Ngày càng có nhiều bạn trẻ chọn ở nhà trong thời gian dài, trở thành những "trạch nam", "trạch nữ" và hạn chế tối đa việc tương tác với xã hội bên ngoài. Nguyên nhân lớn là bởi Internet đã cung cấp đầy đủ các tiện ích để bạn giải quyết mọi nhu cầu cơ bản của cuộc sống ngay trên máy tính mà không cần phải bước chân ra ngoài hay giao tiếp với bất kỳ ai.

Đây là một xu hướng chung trên toàn cầu khi mọi người ngày càng ít ra ngoài hơn. Một [thống kê tại Mỹ](https://axios.com/2023/11/16/walking-americans-declines-map) cho thấy số lượt đi bộ hàng ngày của người Mỹ (tính các lượt đi từ 250 mét trở lên) đang sụt giảm nghiêm trọng, năm 2022 giảm tới 36% so với năm 2019.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112712.webp)

Điều này chứng minh thời gian người dân ở nhà đang tăng lên, đồng thời các hoạt động giao tiếp xã hội trực tiếp đang sụt giảm.

Nhìn về tương lai, "văn hóa khép kín" chắc chắn sẽ còn phát triển mạnh mẽ hơn nữa. Số lượng các công việc bắt buộc phải gặp mặt trực tiếp để giải quyết sẽ ngày càng ít đi.

Tôi không rõ xu hướng này sẽ dẫn dắt xã hội loài người đi về đâu khi mỗi cá nhân đều hạn chế tiếp xúc trực tiếp với đồng loại. Tuy nhiên, đây là kết quả tất yếu của sự phát triển công nghệ và chúng ta chỉ có thể học cách thích nghi với nó.

Khi đó, những dịch vụ giúp kết nối và gia tăng giao tiếp trực tiếp giữa con người sẽ trở nên rất thời thượng và được đón nhận nhiệt tình. Ví dụ như các buổi thảo luận chuyên đề, câu lạc bộ sách, buổi chia sẻ trực tiếp... sẽ rất phổ biến. Bên cạnh đó, các ứng dụng bạn đồng hành AI cũng hứa hẹn sẽ lên ngôi.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112503.webp)

## 科技动态

1、[Vấn đề bãi thải xe ô tô cũ tại quốc đảo Tonga](https://www.abc.net.au/news/science/2023-09-19/how-tonga-plans-to-recycle-its-mountain-of-scrap-cars/102614772)

Tonga, một quốc đảo nhỏ bé ở Thái Bình Dương, có tổng diện tích đất liền chỉ khoảng 260 km vuông (tương đương khu vực nội thành nhỏ của các thành phố lớn).

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092102.webp)

Quốc gia này hiện đang đau đầu đối phó với cuộc khủng hoảng xe ô tô hết hạn sử dụng. Số lượng xe phế thải đã vượt quá 30.000 chiếc và họ không còn chỗ để chứa chúng.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092103.webp)

Bãi tập kết xe phế liệu hiện tại đã chất cao như những tòa nhà vài tầng, các xe mới chuyển đến chỉ còn cách xếp chồng lên trên cùng.

Khi trời mưa, các kim loại hoen gỉ, lớp sơn bong tróc và lượng xăng dầu thừa từ đống phế liệu này sẽ bị cuốn trôi xuống đất, gây ô nhiễm nghiêm trọng nguồn nước sinh hoạt.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092104.webp)

Do không có hạ tầng xử lý xe cũ, các phương tiện di chuyển trên đường phố Tonga đều rất xập xệ, mỗi chiếc xe đều phải gồng gánh hoạt động qua nhiều năm và liên tục được chắp vá sửa chữa để tiếp tục chạy.

Tonga không thể tự giải quyết vấn đề này và đang đàm phán với Nhật Bản with hy vọng vận chuyển toàn bộ số xe phế thải này sang Nhật Bản để tái chế.

2、[Thử nghiệm thành công tàu khí tượng không người lái](https://www.eworldship.com/html/2023/new_ship_type_1122/198244.html)

Trung Quốc mới đây đã thực hiện thành công chuyến hải trình thử nghiệm của tàu khí tượng tự hành không người lái.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112510.webp)

Một chiếc tàu không người lái dài 12 mét đã di chuyển liên tục 16 giờ trên biển với tổng quãng đường 110 hải lý để thu thập các dữ liệu khí tượng hải văn.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112511.webp)

Sự xuất hiện của tàu tự hành giúp giải quyết triệt để vấn đề thiếu hụt trạm quan trắc khí tượng ở các vùng biển xa, đồng thời hỗ trợ khảo sát nhanh các hiện tượng thời tiết bất thường trên biển một cách an toàn và tiện lợi.

3、[Phán quyết quan trọng trong vụ kiện bản quyền AI](https://www.hollywoodreporter.com/business/business-news/sarah-silverman-lawsuit-ai-meta-1235669403/)

Một nữ nhà văn người Mỹ (hình dưới) đã đệ đơn kiện tập đoàn Meta vì tự ý sử dụng các tác phẩm của cô để huấn luyện mô hình ngôn ngữ lớn Llama.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112806.webp)

Tòa án mới đây đã đưa ra phán quyết bác bỏ đơn kiện của cô với lý do nguyên đơn không chứng minh được mô hình AI đã thực hiện hành vi sao chép hay cải biên trực tiếp tác phẩm của mình.

Điều này đồng nghĩa với việc tòa án xác định: **Hành vi sử dụng tác phẩm có bản quyền để huấn luyện mô hình AI không cấu thành vi phạm pháp luật, trừ khi sản phẩm đầu ra của AI cho thấy sự sao chép rõ ràng từ tác phẩm gốc**.

Quyết định này mở đường cho việc các nhà phát triển AI tại Mỹ được phép sử dụng hợp pháp các tài liệu có bản quyền để huấn luyện mô hình. Nhiều khả năng hệ thống pháp luật Trung Quốc cũng sẽ áp dụng quan điểm tương tự nhằm tránh làm mất đi lợi thế cạnh tranh của các mô hình AI nội địa so với Mỹ.

4、[Hạ thủy trung tâm dữ liệu dưới lòng đại dương](https://www.hinews.cn/news/system/2023/11/24/033078392.shtml)

Vào ngày 24 tháng 11, trung tâm dữ liệu thương mại đặt dưới đáy biển đầu tiên trên thế giới đã chính thức được hạ thủy tại vùng biển Hải Nam, Trung Quốc.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112512.webp)

Khối thiết bị nặng 1300 tấn chứa 100 máy chủ đã được thả xuống độ sâu 35 mét dưới lòng đại dương.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112513.webp)

Việc đặt phòng máy dưới biển giúp doanh nghiệp tiết kiệm quỹ đất xây dựng trên đất liền, loại bỏ nhu cầu tiêu thụ nước ngọt để làm mát hệ thống và giảm từ 40% đến 60% lượng điện năng tiêu thụ.

Tập đoàn Microsoft từng thử nghiệm mô hình này nhưng chưa đưa vào khai thác thương mại thực tế. Dự án của Trung Quốc lần này sẽ bàn giao trực tiếp cho khách hàng sử dụng, và nếu hoạt động hiệu quả sẽ được nhân rộng ra nhiều tỉnh ven biển khác.

5、[Giải thưởng toán học AI](https://aimoprize.com/)

Kỳ thi Olympic Toán học Quốc tế (IMO) là sân chơi trí tuệ dành cho học sinh trung học với các đề thi có độ khó rất cao.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113017.webp)

Một quỹ đầu tư của Mỹ mới đây đã công bố giải thưởng trị giá 10 triệu USD (hình trên) dành cho bất kỳ mô hình AI mã nguồn mở nào đầu tiên đạt được thành tích tương đương huy chương Vàng IMO.

Đây là một cột mốc mang tính bước ngoặt. Các mô hình AI hiện nay về bản chất chỉ là mô hình ngôn ngữ lớn dựa trên dự báo thống kê. Nếu trong tương lai AI có thể tự mình giải quyết và chứng minh các bài toán lý thuyết phức tạp, điều đó chứng tỏ AI đã sở hữu năng lực lập luận và suy luận logic thực sự, và thời điểm "Trí tuệ nhân tạo tổng hợp (AGI)" xuất hiện có lẽ không còn xa.

## Bài viết

1\. [Sự kiện ra mắt dòng chip CPU nội địa Loongson 3A6000](https://www.ithome.com/0/735/479.htm)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113010.webp)

Tuần này, thế hệ chip CPU nội địa Loongson 3A6000 đã chính thức được công bố. Các video thử nghiệm thực tế cho thấy khi hoạt động ở xung nhịp 2.5GHz, hiệu năng của chip tiệm cận dòng Intel Core i5-14600K và có thể ép xung lên tới 3GHz. Việc chip nội địa đạt được cột mốc hiệu năng này là một bước tiến rất đáng nể.

2\. [Nhìn lại chặng đường 18 năm làm việc tại Google](https://finance.sina.com.cn/stock/usstock/c/2023-11-24/doc-imzvsncv7037099.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112505.webp)

Tác giả đã gắn bó với Google suốt 18 năm trước khi quyết định từ chức vào tháng này. Anh đã viết một bài chia sẻ thẳng thắn chê trách Google đã đánh mất đi tinh thần lý tưởng thuở ban đầu để trở thành một cỗ máy cồng kềnh đầy quan liêu và kém sáng tạo.

Bài viết là bản tin tiếng Trung về sự kiện, bạn đọc quan tâm có thể xem thêm [Bản gốc tiếng Anh](https://ln.hixie.ch/?start=1700627373) hoặc [Bản dịch tiếng Việt](https://icloudnative.io/posts/reflecting-on-18-years-at-google/). (Đóng góp của [@yangchuansheng](https://github.com/ruanyf/weekly/issues/3660))

3\. [Trải nghiệm mua xe điện giá rẻ của tôi từ Trung Quốc](https://electrek.co/2023/11/21/my-love-of-weird-electric-vehicles-landed-me-on-china-state-tv/)（Tiếng Anh）

Tác giả là một chuyên gia về pin tại Mỹ. Ban đầu vì tò mò, anh phát hiện ra trên trang Alibaba bán rất nhiều dòng xe điện có thiết kế độc lạ với giá cực kỳ rẻ.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112403.webp)

Anh đã quyết định đặt mua thử một chiếc xe và vận chuyển về Mỹ. Kể từ đó, anh trở nên đam mê dòng sản phẩm này và viết rất nhiều bài giới thiệu xe điện giá rẻ Trung Quốc tới cộng đồng người dùng Mỹ.

4\. [Hầu hết các công ty khởi nghiệp AI đều cầm chắc thất bại](https://weightythoughts.com/p/most-ai-startups-are-doomed)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112901.webp)

Góc nhìn của một nhà đầu tư mạo hiểm: Rất tin tưởng vào tương lai của công nghệ AI nhưng lại hoài nghi về khả năng thành công của các startup mảng này. Bài viết phân tích các nguyên nhân, trong đó có một nhận định thực tế: "Nếu bạn có thể viết xong sản phẩm đó trong hai ngày cuối tuần, thì những người khác cũng làm được điều tương tự."

5\. [Giải mã nguyên nhân khiến Web Components vẫn chưa thể phổ biến](https://daverupert.com/2023/07/why-not-webcomponents/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080302.webp)

Công nghệ Web Components đã ra đời được 10 năm nhưng vẫn chưa được ứng dụng rộng rãi. Tại sao một giải pháp được trình duyệt hỗ trợ gốc lại gặp khó khăn trong việc tiếp cận nhà phát triển? Tác giả phân tích những điểm chưa hợp lý trong thiết kế của bộ tiêu chuẩn này.

6\. [Deno công bố tính năng Deno Cron](https://deno.com/blog/cron)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113002.webp)

Dịch vụ Deno Deploy chính thức bổ sung tính năng lập lịch chạy tác vụ tự động Deno Cron, mang lại giải pháp tiện lợi cho các lập trình viên khi cần lên lịch thực thi các đoạn mã JavaScript.

7\. [Đánh giá trải nghiệm phát triển game trên 6 nền tảng khác nhau](https://ruoyusun.com/2023/10/12/one-game-six-platforms.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101402.webp)

Tác giả so sánh các ưu nhược điểm thực tế khi phát triển và tối ưu hóa cùng một tựa game trên 6 nền tảng phổ biến: Web, Windows, macOS, Linux, Android và iOS.

8\. [Robot làm việc nhà Dobb-E](https://dobb-e.com/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113011.webp)

Đội ngũ nghiên cứu tại Đại học New York đã thiết kế một dòng robot hỗ trợ việc nhà với tiêu chí giá rẻ và đa năng. Robot học hỏi và bắt chước các thao tác dọn dẹp thông qua việc quan sát hành vi của con người. Nhóm nghiên cứu hiện đã công bố mã nguồn mở thiết kế của dự án này.

## [本周软件] esProc

Bản tin số 273 từng giới thiệu về SPL - một engine tính toán dữ liệu hiệu năng cao do đội ngũ Trung Quốc tự phát triển.

Nhằm giúp người dùng phổ thông dễ dàng tiếp cận công nghệ này, đội ngũ phát triển đã xây dựng một công cụ đồng hành rất tiện lợi mang tên "esProc" (集算器).

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112903.webp)

Giao diện và cách sử dụng của esProc rất giống với Microsoft Excel, giúp người dùng không có nền tảng lập trình vẫn có thể nhanh chóng làm quen. Tuy nhiên, năng lực lập trình xử lý dữ liệu của nó mạnh mẽ hơn nhiều, thực chất đây là một **ngôn ngữ lập trình chạy trên các ô dữ liệu (cell-based)**.

Tên của các ô đóng vai trò là tên biến (ví dụ ô `A1` chứa giá trị thì lệnh tại ô `B1` gọi `A1 + 5` sẽ cho ra kết quả tương ứng). Cách thiết kế này giúp việc tham chiếu các bước xử lý trước đó trở nên vô cùng trực quan và dễ theo dõi.

Dưới đây là một [ví dụ thực tế](https://c.raqsoft.com.cn/article/1536756719594) minh họa cách viết chỉ 10 dòng code kết hợp các hàm xử lý dữ liệu lớn để tạo ra một "Robot làm thơ cổ" khá thú vị.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112904.webp)

esProc được mở mã nguồn mở hoàn toàn, hỗ trợ các hệ điều hành Windows, macOS, Linux cũng như cung cấp gói thư viện Java. Bạn đọc có thể tìm hiểu thêm mã nguồn dự án trên [GitHub](https://github.com/SPLware/esProc).

## 工具

1、[Biome](https://biomejs.dev/)

Đội ngũ phát triển công cụ format code Prettier trước đây từng treo giải thưởng 20.000 USD cho bất kỳ dự án nào viết lại được Prettier bằng ngôn ngữ Rust và vượt qua toàn bộ các ca kiểm thử sẵn có.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112804.webp)

Chỉ sau hai tuần công bố, dự án Biome đã xuất sắc giành được giải thưởng này.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112805.webp)

Biome là một bộ công cụ all-in-one dành cho JavaScript/TypeScript, hỗ trợ format và lint code nhanh chóng mà không cần cấu hình phức tạp, sở hữu hiệu năng xử lý cực kỳ ấn tượng.

2、[IP Guide](https://ip.guide/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112502.webp)

Trang web cung cấp cổng API miễn phí để tra cứu thông tin địa lý của địa chỉ IP.

3、[macOS Screen Saver as Chrome New Tab](https://github.com/jason5ng32/macOS-Screen-Saver-as-Chrome-New-Tab)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113015.webp)

Tiện ích mở rộng trên Chrome/Edge giúp hiển thị các video màn hình chờ (screensaver) chất lượng 4K của macOS mỗi khi bạn mở tab mới. (Đóng góp của [@Y024](https://github.com/ruanyf/weekly/issues))

4、[streamlit-shadcn-ui](https://github.com/ObservedObserver/streamlit-shadcn-ui)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113005.webp)

Thư viện component UI phong cách shadcn dành cho framework phát triển web Python Streamlit. (Đóng góp của [@ObservedObserver](https://github.com/ruanyf/weekly/issues/3668))

5、[miniPaint](https://zaixianps.net/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113003.webp)

Trang web hỗ trợ vẽ và chỉnh sửa ảnh trực tuyến được việt hóa dựa trên dự án mã nguồn mở gốc miniPaint. (Đóng góp của [@geeeeeeeek](https://github.com/ruanyf/weekly/issues/3665))

6、[Rsbuild](https://github.com/web-infra-dev/rsbuild)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112709.webp)

Bộ công cụ build web hiệu năng cao thay thế cho Webpack, giúp giảm thiểu 90% cấu hình phức tạp và tăng tốc độ đóng gói lên gấp 10 lần. (Đóng góp của [@chenjiahan](https://github.com/ruanyf/weekly/issues/3662))

7、[Chatfairy](https://github.com/yuxiaoy1/chatfairy)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112504.webp)

Đoạn mã Python siêu tối giản chỉ với 115 dòng giúp dựng nhanh một phòng chat trực tuyến trên web, sử dụng giao thức Server-Sent Events (SSE) để đẩy tin nhắn thời gian thực. (Đóng góp của [@yuxiaoy1](https://github.com/ruanyf/weekly/issues/3659))

8、[Gmeek](https://github.com/Meekdai/Gmeek)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113006.webp)

Mẫu thiết kế blog cá nhân siêu nhẹ, hỗ trợ tự động chuyển đổi các bài viết từ mục Issue trên GitHub thành giao diện website. (Đóng góp của [@Meekdai](https://github.com/ruanyf/weekly/issues/3669))

9、[TQUIC](https://github.com/Tencent/tquic)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113009.webp)

Thư viện triển khai giao thức mạng QUIC thế hệ mới do tập đoàn Tencent mở nguồn mở. (Đóng góp của [@ryantang1991](https://github.com/ruanyf/weekly/issues/3671))

10、[ai-teacher](https://github.com/guojingwen/ai-teacher)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113004.webp)

Mẫu giao diện frontend kết nối với ChatGPT, thích hợp làm tài liệu tham khảo cho lập trình viên. (Đóng góp của [@guojingwen](https://github.com/ruanyf/weekly/issues/3667))

11、[DevOpsGPT](https://github.com/kuafuai/DevOpsGPT)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112710.webp)

Ứng dụng hỗ trợ quy trình phát triển phần mềm bằng AI: tự động tạo tài liệu đặc tả yêu cầu và chuyển đổi thành mã nguồn tương ứng. (Đóng góp của [@qinwanglsm](https://github.com/ruanyf/weekly/issues/3664))

## 资源

1、[Trải nghiệm vẽ tranh siêu tốc SDXL Turbo](https://sdxlturbo.ai/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113008.webp)

Trang web cho phép dùng thử miễn phí mô hình vẽ tranh thế hệ mới SDXL Turbo với tốc độ phản hồi gần như tức thì mà không cần chờ đợi. (Đóng góp của [@zengdamo](https://github.com/ruanyf/weekly/issues/3680))

2、[Lễ hội Podcast Công nghệ Trung Quốc](https://podfest.tech/zh-CN)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113007.webp)

Sự kiện diễn ra từ ngày 4 đến ngày 8 tháng 12, nơi các kênh Podcast công nghệ lớn sẽ đồng loạt đăng tải các số phát sóng đặc biệt xoay quanh nhiều chủ đề kỹ thuật đa dạng. (Đóng góp của [@le0zh0u](https://github.com/ruanyf/weekly/issues/3683))

3、[ataiva.com](https://ataiva.com/archives/)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100101.webp)

Trang blog công nghệ cá nhân chứa chuỗi bài viết hướng dẫn chi tiết về Docker và các kiến thức nhập môn Học máy.

4、[Khóa học Generative AI dành cho người mới bắt đầu](https://github.com/Microsoft/generative-ai-for-beginners)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112501.webp)

Khóa học nhập môn về Trí tuệ nhân tạo tạo sinh gồm 12 bài giảng do Microsoft biên soạn.

## 图片

1、[Sự nhầm lẫn về hiện tượng tự tương quan trong nghiên cứu](https://economicsfromthetopdown.com/2022/04/08/the-dunning-kruger-effect-is-autocorrelation/)

Nhiều bài báo nghiên cứu khoa học thường mắc lỗi logic cơ bản mang tên "Tự tương quan" (Autocorrelation) - khi tác giả kết luận hai biến số có mối quan hệ nhân quả với nhau nhưng thực chất biến đó chỉ đang tương quan với chính nó.

Ví dụ, giả sử hai biến số x và y hoàn toàn độc lập và không liên quan gì đến nhau, biểu đồ phân tán của chúng sẽ hiển thị ngẫu nhiên như hình dưới:

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112601.webp)

Bây giờ, chúng ta tạo ra biến số thứ ba z = x + y, khi đó biểu đồ phân tán giữa x và z sẽ xuất hiện như sau:

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112602.webp)

Về mặt trực quan, biểu đồ cho thấy mối quan hệ tương quan tuyến tính rất mạnh mẽ giữa x và z. Tuy nhiên thực chất đây chỉ là sự tự tương quan của chính biến x, còn sự góp mặt của y chỉ đóng vai trò như một yếu tố gây nhiễu thống kê.

Nếu người nghiên cứu không hiểu rõ bản chất toán học này, họ sẽ dễ dàng đưa ra kết luận sai lầm rằng x và z có mối quan hệ tác động qua lại lẫn nhau.

2、[Thiết bị hồi sức chim yến trong hầm mỏ](https://museumcrush.org/this-device-was-used-to-resuscitate-canaries-in-coal-mines/)

Vào năm 1896, một kỹ sư người Anh đã chứng minh các vụ nổ trong hầm mỏ phần lớn do khí độc carbon monoxide (CO) tích tụ gây ra, và nhân loại cần tìm một giải pháp phát hiện sớm lượng khí CO rò rỉ này.

Ông đã nghĩ đến việc sử dụng chim yến (hoặc chim hoàng yến) làm vật thử nghiệm. Chim yến cực kỳ nhạy cảm với khí CO và sẽ có dấu hiệu trúng độc nhanh hơn con người rất nhiều. Khi thợ mỏ thấy chim yến lảo đảo suy kiệt, họ sẽ biết ngay khí độc đang rò rỉ để kịp thời sơ tán.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011004.webp)

Ông đã chế tạo ra một chiếc lồng đặc biệt bằng kính và kim loại với một mặt lưới thông khí bên ngoài.

Điểm độc đáo là chiếc lồng tích hợp sẵn một bình dưỡng khí nhỏ phía trên. Ngay khi thợ mỏ phát hiện chim yến có dấu hiệu lờ đờ trúng độc CO, họ sẽ đóng kín mặt lưới thông khí và mở van xả oxy để cứu sống chú chim, đồng thời toàn bộ đội thợ mỏ sẽ lập tức di chuyển ra khỏi khu vực nguy hiểm.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011005.webp)

## ✍️ Bài đọc thêm

### Tìm hiểu về hội chứng ảo tưởng kiến thức thời đại Internet

Hội chứng "ảo tưởng kiến thức" (The illusion of knowledge) là trạng thái khi một người tự tin cho rằng mình đã am hiểu hoặc làm chủ một kỹ năng nào đó, nhưng thực tế năng lực của họ lại hoàn toàn bằng không.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023113016.webp)

Một nghiên cứu khoa học gần đây chỉ ra rằng Internet đang góp phần làm trầm trọng thêm hội chứng này, khiến con người trở nên tự tin thái quá vào trình độ thực tế của bản thân.

Các nhà nghiên cứu đã yêu cầu những người tham gia khảo sát xem đi xem lại một video hướng dẫn một kỹ năng cụ thể (ví dụ như ném phi tiêu hoặc nhảy breakdance) với số lượng tối đa lên tới 20 lần.

Sau khi xem xong, những người này được yêu cầu tự đánh giá mức độ am hiểu và tự tin thực hiện kỹ năng đó của bản thân.

Hầu hết người tham gia đều khẳng định họ đã cơ bản nắm vững kỹ năng thông qua việc xem video. Đặc biệt những người xem video càng nhiều lần thì câu trả lời của họ càng dứt khoát và tỏ ra vô cùng tự tin.

Tuy nhiên, khi bước vào phần thực hành thực tế trước đám đông, kết quả thu về lại cực kỳ thất vọng. Hầu như không một ai có thể thực hiện thành công kỹ năng đó. Nhóm nghiên cứu nhận định: "Màn trình diễn thực tế của họ không cho thấy bất kỳ dấu hiệu nào chứng tỏ họ đã tiếp thu được kiến thức từ video."

Các lập trình viên nên đặc biệt lưu tâm đến hội chứng này. Việc đọc xong một cuốn sách giáo trình hay tài liệu hướng dẫn (documentation) không đồng nghĩa với việc bạn đã làm chủ được công nghệ đó. Bạn bắt buộc phải tự tay viết code và hoàn thành các dự án thực tế thì mới thực sự biến kiến thức đó thành của mình.

## Lịch sử tuần này

- 2022年（第 233 期）：[Góc nhìn cuộc sống: Suy ngẫm về hình ảnh cuộc sống của chúng ta tương đồng với một bể cá cảnh](https://www.ruanyifeng.com/blog/2022/12/weekly-issue-233.html)
- 2021年（第 183 期）：[Chế độ đãi ngộ: Tìm hiểu về các chính sách phúc lợi hưu trí dành cho nhân viên tại tập đoàn Tencent](https://www.ruanyifeng.com/blog/2021/11/weekly-issue-183.html)
- 2020年（第 133 期）：[Phát triển vùng miền: Thảo luận về tiềm năng xây dựng tỉnh Quý Châu thành một Thụy Sĩ của châu Á](https://www.ruanyifeng.com/blog/2020/11/weekly-issue-133.html)
- 2019年（第 83 期）：[Góc nhìn xã hội: Bàn luận về việc công nghệ không thể giải quyết sự đối lập tư tưởng giữa con người](https://www.ruanyifeng.com/blog/2019/11/weekly-issue-83.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
