# 科技爱好者周刊：第 63 期 (Bản tin chia sẻ công nghệ số 63)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Chào mừng mọi người gửi bài đóng góp hoặc tự đề xuất dự án cá nhân qua mục [issue](https://github.com/ruanyf/weekly/issues) tại kho lưu trữ GitHub [ruanyf/weekly](https://github.com/ruanyf/weekly).

![](https://cdn.beekka.com/blogimg/asset/201907/bg2019070402.jpg)

Mấy ngày trước, tôi đọc được một tin tức:

> "Ngày 17/5, nhà cung cấp dịch vụ CDN Trung Quốc ChinaCache phát đi thông báo cho biết do bị cáo buộc liên quan đến hành vi hối lộ doanh nghiệp, CEO Vương Tùng (ảnh trên) đã bị cảnh sát bắt giữ để điều tra.
> 
> Chịu ảnh hưởng bởi thông tin này, giá cổ phiếu ChinaCache trên sàn Nasdaq lập tức bốc hơi 30% xuống còn 0,77 USD/cổ phiếu. Sàn giao dịch Nasdaq cũng ra thông báo tạm dừng giao dịch cổ phiếu ChinaCache cho đến khi công ty cung cấp đầy đủ thông tin giải trình thỏa đáng."

Tôi thấy cái tên ChinaCache (Lam Tấn) rất quen thuộc. Nghĩ mãi mới nhớ ra, nhiều năm trước khi muốn sử dụng CDN cho blog cá nhân, tôi đã tra cứu giá của một số nhà cung cấp dịch vụ trong nước, trong đó có ChinaCache - một trong số ít doanh nghiệp chuyên biệt về CDN lúc bấy giờ.

Nhìn lại lịch sử của ChinaCache, điều đó hoàn toàn chính xác:

> Năm 2003, ChinaCache đã cung cấp dịch vụ cho 530 kênh nội dung của các ICP lớn, các thương hiệu lớn như Coca-Cola, Nokia và Sony đều là khách hàng của hãng. Năm 2010, ChinaCache niêm yết thành công trên sàn Nasdaq của Mỹ, tiến trình phát triển có vẻ đang đi vào quỹ đạo tăng trưởng nhanh.
> 
> Tuy nhiên, ngay sau khi niêm yết, doanh nghiệp đột ngột lao dốc. Trong ba năm từ 2014 đến 2016, ChinaCache liên tục thua lỗ, khoản lỗ năm 2016 lên tới 496,9 triệu nhân dân tệ. Nửa đầu năm 2017, doanh thu thuần của hãng sụt giảm 22.6% kèm khoản lỗ ròng 125,9 triệu nhân dân tệ, báo cáo tài chính giải trình nguyên nhân sụt giảm là do sự cạnh tranh khốc liệt của ngành.

Thời kỳ đầu của internet Trung Quốc, các công ty dịch vụ mạng mọc lên như nấm sau mưa. Chỉ cần thuê vài tủ rack trong phòng máy IDC là có thể mở công ty dịch vụ mạng. Tại sao sau này họ lại không thể duy trì? Tại sao ChinaCache bắt đầu suy tàn từ năm 2014?

Nguyên nhân rất đơn giản: do sự xuất hiện của Alibaba Cloud, tiếp theo là việc các ông lớn internet lớn khác cũng tự xây dựng hạ tầng dịch vụ đám mây (Cloud computing) của riêng mình. Các tập đoàn lớn hoạt động như những cục nam châm khổng lồ hút sạch tệp khách hàng, khiến các công ty dịch vụ mạng nhỏ lẻ không thể gượng dậy được.

Đây là xu hướng phổ biến "người thắng ăn cả" (winner-takes-all) của ngành công nghệ thông tin. Các ngành truyền thống có thể dung hòa nhiều doanh nghiệp cùng tồn tại (như ngành bán lẻ bách hóa có rất nhiều chuỗi cửa hàng). Nhưng thế giới internet thì khác, mỗi phân khúc thị trường thường chỉ có tối đa 2 doanh nghiệp dẫn đầu là sống khỏe, phần còn lại hầu hết đều chật vật hoặc bị đào thải.

Nếu bạn thấy một phân khúc nào đó vẫn đang cạnh tranh khốc liệt giữa nhiều bên, điều đó chỉ chứng tỏ thị trường đó chưa được thống nhất hoặc chưa được số hóa triệt để (như mảng giáo dục và đào tạo trực tuyến hiện tại). Xu hướng tương lai là bất kỳ mảng nào có sự tham gia của Alibaba hay Tencent thì hai ông lớn này sẽ thâu tóm toàn bộ thị phần, các bên khác khó có cơ hội chia phần. Nếu không thể đè bẹp đối thủ bằng công nghệ, họ sẽ đơn giản là mua lại đối thủ.

## Chương trình thiết kế kế hoạch bảo vệ tài chính gia đình

Bản tin số này rất hân hạnh nhận được sự đồng hành từ thầy Tôn Minh Triển. Dưới đây là chương trình tư vấn tài chính bảo hiểm gia đình miễn phí do anh tổ chức.

Thầy Tôn Minh Triển là thạc sĩ Khoa Thống kê Đại học Trung Sơn, có nhiều năm kinh nghiệm thiết kế sản phẩm và giải quyết bồi thường tại các hãng bảo hiểm lớn, hiện sáng lập thương hiệu tư vấn tài chính "Pulan" kiêm cố vấn thạc sĩ thực hành tại Khoa Tài chính Đại học Trung Sơn.

Bên cạnh công việc kinh doanh, anh còn vận hành trang tin cá nhân mang tên "Tôn Minh Triển" chuyên chia sẻ kiến thức về bảo hiểm gia đình, bảo hiểm cho trẻ em và tư duy tài chính cho trẻ nhỏ với hơn 500 bài viết phân tích tình huống thực tế rất giá trị.

**Nhằm quảng bá kiến thức bảo hiểm đúng đắn, anh tổ chức chương trình "Tư vấn thiết kế kế hoạch bảo hiểm gia đình" miễn phí.** Nếu bạn từng gặp sự cố bị nhân viên đại lý bảo hiểm lừa dối, lo ngại các điều khoản phức tạp của bảo hiểm, hoặc đơn giản muốn tối ưu hóa danh mục bảo vệ tài chính cho gia đình mình đều có thể tham gia. Đội ngũ chuyên gia sẽ trao đổi trực tiếp qua điện thoại hoặc trực tuyến để tư vấn dựa trên cấu trúc gia đình cụ thể.

Quét mã QR WeChat dưới đây, nhập từ khóa **<span style="color:red;">“阮一峰 + Số điện thoại của bạn”</span>** để đăng ký tham gia chương trình. Mỗi người tham gia sẽ nhận được một bản báo cáo đánh giá toàn diện năng lực bảo vệ tài chính gia đình trị giá 800 nhân dân tệ hoàn toàn miễn phí.

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019060903.jpg)

## 资讯 (Tin tức)

1、[Tàu thăm dò Hayabusa2 của Nhật Bản chụp ảnh cận cảnh bề mặt tiểu hành tinh Ryugu từ độ cao 9 mét](https://www.cnet.com/news/japans-hayabusa2-spacecraft-snaps-close-up-just-30-feet-above-asteroid/)

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019060801.jpg)

Tàu vũ trụ thám hiểm cỡ nhỏ Hayabusa2 của Cơ quan Vũ trụ Nhật Bản (JAXA) sau gần một năm bay quanh tiểu hành tinh Ryugu đã gửi về bức ảnh siêu nét chụp cận cảnh bề mặt đá từ độ cao chỉ vỏn vẹn 9 mét. Đây là một kỳ tích kỹ thuật: tàu vũ trụ chỉ có kích thước bằng chiếc tủ lạnh và nặng 600 kg đã bay quãng đường 170 triệu dặm với tốc độ 15 dặm/giây để tiếp cận chính xác một tiểu hành tinh có đường kính chỉ 1 km, thực hiện đổ bộ thu thập mẫu đá thành công và dự kiến bay ngược về Trái Đất vào tháng 12/2020.

2、[Dự án xây dựng tòa nhà chung cư hộp ngủ khổng lồ 18 tầng giải quyết nạn thiếu nhà ở tại thung lũng Silicon](https://www.citylab.com/life/2019/06/cohousing-san-jose-room-for-rent-starcity-coliving-housing/590731/)

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019060802.jpg)

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019060803.jpg)

Thị trường lao động Silicon liên tục phình to kéo theo dòng người nhập cư khổng lồ khiến nhà ở trở thành gánh nặng đắt đỏ khi giá thuê một căn hộ một phòng ngủ tại San Jose lên tới 2.700 USD/tháng. Nhà phát triển Starcity công bố dự án xây dựng tòa chung cư đồng sinh hoạt (co-living) lớn nhất khu vực với chiều cao 18 tầng cung cấp 803 phòng ngủ mini tự lập. Giá thuê khởi điểm từ 2.000 USD/tháng với các khu bếp chung (ảnh dưới) và khu phòng khách giải trí chung (ảnh trên) được chia sẻ giữa các cư dân.

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019060804.jpg)

3、[NASA chính thức mở cửa Trạm vũ trụ quốc tế ISS đón khách du lịch tư nhân tham quan](https://www.bbc.com/news/world-us-canada-48560874)

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019060805.jpg)

Trạm vũ trụ quốc tế ISS bắt đầu xây dựng từ 20 năm trước, chủ yếu do Mỹ và Nga vận hành. Mỹ có kế hoạch tư nhân hóa trạm ISS và rút ngân sách chính phủ khỏi dự án trước năm 2025. Để bắt đầu lộ trình thương mại hóa, NASA công bố cho phép các chuyến bay du lịch tư nhân cập bến trạm ISS thông qua sự điều phối của hai hãng đối tác là SpaceX và Boeing. Dự kiến mỗi năm có tối đa 2 chuyến bay đưa du khách lên lưu trú trên trạm tối đa 30 ngày với chi phí do các hãng bay tự định giá. (Trước đây, do thiếu kinh phí, Nga từng bán vé cho doanh nhân Mỹ Dennis Tito lên trạm vào năm 2001 với chi phí khoảng 20 triệu USD khứ hồi).

4、[Xu hướng đặt phụ đề sách siêu dài để tối ưu hóa SEO trên các công cụ tìm kiếm](https://www.washingtonpost.com/entertainment/books/book-subtitles-are-getting-ridiculously-long-what-is-going-on/2019/06/04/3150bcc8-86c3-11e9-98c1-e945ae5db8fb_story.html)

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019060806.jpg)

Tờ *The Washington Post* đưa tin, nhằm giúp sách giấy dễ dàng được hiển thị trên kết quả tìm kiếm trực tuyến của người dùng, các tác giả có xu hướng đặt phụ đề sách (subtitles) siêu dài chứa nhiều từ khóa mô tả chi tiết. (Ảnh trên: Cuốn sách có tiêu đề chính là *Solitude and Company*, kèm phụ đề dài dằng dặc: "Câu chuyện về Gabriel García Márquez qua lời kể của bạn bè, gia đình, người hâm mộ, những người phản biện, đồng nghiệp, bạn nhậu và một số linh kiện đáng kính của cuộc đời ông").

5、[Vụ kiện đầu tiên liên quan đến thuật toán AI giao dịch tài chính thua lỗ khổng lồ tại Hồng Kông](https://www.bloomberg.com/news/articles/2019-05-06/who-to-sue-when-a-robot-loses-your-fortune)

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019060901.jpg)

Doanh nhân Hồng Kông Li Jianqin mua gói quỹ phòng hộ ủy quyền giao dịch tối đa 2,5 tỷ USD của một công ty tài chính, vận hành hoàn toàn tự động bằng thuật toán AI. Quỹ quảng cáo có tỷ lệ sinh lời 15.54% và độ chính xác tín hiệu đạt 69.05%. Tuy nhiên sau khi mua, thuật toán liên tục giao dịch thua lỗ lớn, đỉnh điểm có ngày bốc hơi 20 triệu USD. Khách hàng đã đệ đơn kiện nhân viên tư vấn thổi phồng năng lực AI. Đây là vụ kiện pháp lý đầu tiên trên thế giới liên quan đến trách nhiệm thiệt hại do thuật toán giao dịch tự động gây ra.

6、[Nắng nóng kỷ lục càn quét châu Âu đẩy cuộc sống người dân vào cảnh khó khăn do thiếu điều hòa](https://www.nationalgeographic.com/environment/2019/06/europe-has-had-five-500-year-summers-in-15-years/)

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019063001.jpg)

Đợt nắng nóng kỷ lục càn quét châu Âu khiến nhiệt độ tại Pháp và Tây Ban Nha chạm mốc 45°C, Đức lên tới 38°C. Do các nước Bắc Âu có lịch sử mùa hè mát mẻ nên tỷ lệ lắp đặt điều hòa nhiệt độ cực kỳ thấp (Pháp dưới 5% hộ gia đình lắp điều hòa, Đức dưới 2%), khiến cuộc sống người dân gặp nhiều bất tiện. Thống kê khí hậu chỉ ra 5 mùa hè nóng nhất trong vòng 500 năm qua tại châu Âu đều diễn ra trong 15 năm gần nhất.

7、[Báo cáo rò rỉ cho thấy Boeing thuê các kỹ sư phần mềm Ấn Độ giá 9 USD/giờ để viết code cho 737 Max](https://www.bloomberg.com/news/articles/2019-06-28/boeing-s-737-max-software-outsourced-to-9-an-hour-engineers)

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019063003.jpg)

Hai vụ tai nạn thảm khốc của dòng máy bay Boeing 737 Max được xác định có liên quan trực tiếp đến lỗi hệ thống phần mềm điều khiển bay (MCAS) - lỗi phần mềm gây hậu quả nghiêm trọng nhất lịch sử hàng không. Báo cáo mới tiết lộ Boeing đã thuê ngoài (outsource) nhiều gói phần mềm hiển thị buồng lái và kiểm thử cho các công ty công nghệ Ấn Độ như HCL và Cyient. Các kỹ sư tham gia dự án cho biết họ được trả mức thù lao rẻ mạt chỉ khoảng 9 USD/giờ để viết và test code cho dòng máy bay này.

8、**Tin vắn**

- Nghiên cứu của Đại học Berkeley chỉ ra việc tiếp nhận các thông tin mới kích thích não bộ tiết ra chất dopamine tương tự như khi nhận được tiền bạc hay đồ ăn ngon, giải thích chứng nghiện lướt điện thoại xem tin tức của con người hiện đại.

- Thành phố Chennai (lớn thứ 6 tại Ấn Độ) lâm vào cuộc khủng hoảng nước ngọt nghiêm trọng sau hơn 200 ngày liên tiếp không có mưa. 4.6 triệu dân thành phố phải sống dựa vào nguồn nước sinh hoạt chở bằng xe bồn từ nơi khác đến.

- Bản đồ Google Maps chỉ dẫn sai đường khiến hàng loạt tài xế tại Denver đi vào một con đường đất ngập bùn ven ruộng, làm hơn 100 chiếc ô tô bị kẹt cứng giữa đồng ruộng (ảnh dưới).

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019062907.jpg)

## 文章 (Bài viết)

1、[Bài viết] [Tìm hiểu 84 thiên kiến nhận thức tâm lý giúp tối ưu hóa chuyển đổi sản phẩm](https://www.mobilespoon.net/2019/04/collection-cognitive-biases-how-to-use.html) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019061307.jpg)

Hướng dẫn cách vận dụng các hiệu ứng tâm lý học hành vi (như hiệu ứng khan hiếm, hiệu ứng mỏ neo, hiệu ứng hào quang...) vào thiết kế sản phẩm phần mềm để tăng mức độ tương tác và tỷ lệ chuyển đổi của người dùng.

2、[Bài viết] [BBC phóng sự ảnh về cuộc sống của những người dân nghèo chọn chuyển vào sinh sống trong vùng cấm phóng xạ Chernobyl](https://www.bbc.com/news/resources/idt-sh/moving_to_Chernobyl) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019061308.jpg)

Bản tin phóng sự ảnh đặc biệt kể về những gia đình Ukraine chạy trốn chiến sự vùng biên giới đã chấp nhận dọn vào sinh sống tại các ngôi nhà hoang trong vùng cách ly 30km xung quanh nhà máy Chernobyl để lánh nạn và tự trồng trọt sinh tồn.

3、[Bài viết] [Tại sao bạn không nên lạm dụng dịch vụ chống bot ReCAPTCHA của Google?](https://kevv.net/you-probably-dont-need-recaptcha/) (Tiếng Anh)

Phân tích các nhược điểm của công cụ ReCAPTCHA v2/v3: gây suy giảm trải nghiệm người dùng nghiêm trọng, thu thập dữ liệu cá nhân của độc giả và đề xuất các giải pháp chặn spam thay thế nhẹ nhàng hơn (như honeypot field, hashcash).

## 软件 (Phần mềm)

1、[PaperCSS — Thư viện component CSS mang phong cách vẽ phác thảo tay bằng bút chì độc đáo](https://github.com/papercss/papercss)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019052602.jpg)

Thư viện CSS giúp biến toàn bộ các nút bấm, khung viền, font chữ trên website thành phong cách vẽ tay nguệch ngoạc trên giấy nháp rất nghệ thuật.

2、[matomo — Hệ thống phân tích lưu lượng truy cập web mã nguồn mở tự host thay thế Google Analytics](https://github.com/matomo-org/matomo)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019052901.jpg)

Tên gọi cũ là Piwik, cho phép tự cài đặt máy chủ phân tích hành vi người dùng trên web/app để đảm bảo quyền riêng tư và sở hữu 100% dữ liệu thống kê không bị Google khai thác.

3、[Mattermost — Giải pháp chat nhóm cộng tác doanh nghiệp mã nguồn mở, thay thế Slack](https://github.com/mattermost/mattermost-server)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019052902.jpg)

Hệ thống giao tiếp nội bộ mạnh mẽ có thể tự host trên server riêng, hỗ trợ tích hợp Webhooks, ứng dụng di động/desktop đầy đủ, hoạt động tương thích với các API của Slack.

4、[star-history — Công cụ trực quan hóa biểu đồ tăng trưởng số sao (stars) của các dự án GitHub](https://github.com/timqian/star-history)

![](https://cdn.beekka.com/blogimg/asset/201905/bg2019052903.jpg)

Giúp người dùng vẽ biểu đồ đường cong lịch sử nhận star của bất kỳ repository nào trên GitHub để đánh giá mức độ tăng trưởng cộng đồng của dự án.

## 资源 (Tài nguyên)

1、[Trang web] [No More Google - Kho danh sách tổng hợp các giải pháp nguồn mở thay thế dịch vụ Google](https://nomoregoogle.com/)

Bản danh sách hữu ích tập hợp các ứng dụng, dịch vụ đám mây chú trọng quyền riêng tư để thay thế cho Google Search, Gmail, Google Drive, Chrome, YouTube...

## 图片 (Hình ảnh)

1. **Francis Crick viết thư tay cho con trai công bố phát hiện cấu trúc xoắn kép của DNA năm 1953**

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019060302.jpg)

Lá thư tay lịch sử dài 7 trang do nhà sinh học Francis Crick viết gửi con trai Michael vào tháng 3/1953 để thông báo tin vui ông cùng James Watson đã dựng thành công mô hình cấu trúc xoắn kép của DNA. Lá thư này đã được đấu giá thành công với mức giá kỷ lục 5.3 triệu USD vào năm 2013.

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019060303.jpg)

2. **Ý tưởng thiết kế logo Olympic Tokyo 2020 tuyệt đẹp của một designer nghiệp dư người Anh**

![](https://cdn.beekka.com/blogimg/asset/201907/bg2019070204.jpg)

Bản thiết kế logo Olympic Tokyo 2020 do nhà thiết kế Ben Thompson tự vẽ: lồng ghép khéo léo 3 vòng tròn đỏ (biểu tượng cờ Nhật) tạo thành số 2020 kết hợp 5 vòng tròn Olympic tối giản. Nhiều người đánh giá thiết kế này xuất sắc và dễ nhớ hơn nhiều so với logo chính thức của ban tổ chức (ảnh dưới).

![](https://cdn.beekka.com/blogimg/asset/201907/bg2019070205.jpg)

## 言论 (Danh ngôn)

1、

> "Thái độ sống lành mạnh hoặc là sự lạc quan ôn hòa, hoặc là sự bi quan ôn hòa. Kẻ bi quan cực đoan tin rằng mọi sự đều vô nghĩa nên không cần làm gì, kẻ lạc quan cực đoan tin rằng mọi sự rồi sẽ tự tốt đẹp nên cũng không chịu làm gì - cả hai thái độ cực đoan này đều dẫn tới sự lười biếng vô vi."
>
> -- Peter Thiel

2、

> "Thực tế là trong ngành vật lý, thực tế (facts) mới là thứ quan trọng nhất chứ không phải là bằng chứng (evidence). Vật lý lý thuyết hoàn toàn có thể tiến bộ mà không cần bằng chứng thực nghiệm ngay lập tức, nhưng nếu không có các sự kiện thực tế quan sát được làm mốc tiêu chuẩn thì chúng ta sẽ hoàn toàn mất phương hướng."
>
> -- Richard Feynman

(Hết)
