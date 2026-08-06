# 科技爱好者周刊：第 106 期 (Bản tin chia sẻ công nghệ số 106)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1206) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## Ảnh bìa

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042905.jpg)

Gần đây số người đi máy bay giảm mạnh, hãng hàng không không có chỗ để đỗ máy bay. Đường băng của một sân bay ở miền Nam California đầy ắp máy bay. ([Nguồn](https://www.thedrive.com/the-war-zone/33141/these-aerial-and-satellite-photos-of-an-airport-absolutely-stuffed-with-airliners-are-nuts))

## Chủ đề kỳ này: Du mục kỹ thuật số

Hôm nay, hãy cùng tìm hiểu một từ vựng tiếng Anh mới ["digital nomad"](https://en.wikipedia.org/wiki/Digital_nomad), nghĩa tiếng Việt là "du mục kỹ thuật số".

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050303.jpg)

Nó chỉ những người kiếm sống bằng công nghệ số, không có nơi cư trú cố định. Những người như vậy kiếm tiền qua internet, chỉ cần có thể lên mạng, sống ở đâu cũng được.

Họ thường chuyển đến những nơi có phong cảnh đẹp, khí hậu ôn hòa, vật giá rẻ. Nước ngoài có một trang web gọi là [Nomad List](https://nomadlist.com/), bình chọn những nơi phù hợp nhất để "du mục kỹ thuật số" sinh sống, hai vị trí đầu là Budapest và Bali.

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050304.jpg)

Ban đầu, khi tôi thấy từ này, nghĩ đây chỉ là hippie thời đại mới, không cần quan tâm nhiều. Nhưng bây giờ, suy nghĩ của tôi khác rồi, đây là một từ rất quan trọng, mô tả cách sống của mọi người trên internet.

Tôi không nói rằng mọi người sẽ chuyển đến Bali, mà là hành vi mẫu trên internet chính là "du mục".

**Không ai có nơi cư trú cố định trên mạng, trên mạng cũng không có quê hương. Chúng ta trên internet đều là du mục,** tháng này xuất hiện ở trang A, tháng sau xuất hiện ở trang B. Chỉ cần có công cụ mạnh hơn, rẻ hơn được phát hành, người dùng lâu năm hôm sau sẽ rời đi. Hành vi mẫu này không phải "du mục kỹ thuật số" thì là gì?

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050305.jpg)

Đối với những người kiếm tiền trên mạng, cách "du mục kỹ thuật số" còn rõ ràng hơn. Nền tảng nào dễ kiếm tiền thì đến nền tảng đó, giống như du mục thời cổ đại, ở đâu có nước và cỏ phong phú thì đến đó. Hơn nữa, internet cho phép bạn kinh doanh trên nhiều nền tảng cùng lúc, khiến họ càng không có lòng trung thành với nền tảng. [Tạp chí Wired](https://www.wired.co.uk/article/dropshipping-instagram-ads) có một bài viết, mô tả "du mục kỹ thuật số" kiếm tiền trên mạng như thế nào.

> Họ tìm sản phẩm trên AliExpress, dùng Shopify xây dựng trang web, đăng quảng cáo Facebook để quảng bá, thu hút người hâm mộ trên Instagram, phát triển kinh doanh viên cấp tiếp theo trên Wayfair.

Trong tương lai, ngày càng nhiều người có cách kiếm sống liên quan đến internet. Lúc đó, "du mục kỹ thuật số" sẽ không chỉ là hành vi mẫu trên internet, mà sẽ ảnh hưởng đến cuộc sống thực. Chúng ta thực sự sẽ như du mục, không cần đến công ty làm việc mỗi ngày, mà đến nơi mình muốn đến, vừa "du mục kỹ thuật số" vừa làm việc.

## PR nhẹ của Gitee

Dưới đây là giới thiệu phần mềm nội địa tuần này, nhân vật chính hôm nay là [Gitee](https://gitee.com/).

Với những bạn chưa biết, tôi giới thiệu ngắn gọn. Gitee là nền tảng lưu trữ code hàng đầu trong nước, dùng để quản lý code phần mềm, tính năng hoàn toàn không thua các trang web cùng loại ở nước ngoài, và có nhiều thiết kế địa phương hóa cho người dùng trong nước (ví dụ quyền chỉ đọc ở cấp độ file). Ưu điểm nổi bật của nó là tốc độ truy cập cực nhanh, hầu hết các thao tác đều có thể hoàn thành ngay lập tức, không bị giật lag.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042110.png)

Tôi đã hỏi nhân viên kinh doanh của họ, hiện tại người dùng đã vượt quá 5 triệu, kho code lưu trữ hơn 10 triệu, khách hàng doanh nghiệp cũng vượt quá 100.000 doanh nghiệp.

Gần đây, họ ra mắt một tính năng mới — [PR nhẹ](https://blog.gitee.com/2020/03/15/prlite/), rất dễ dùng, rất đáng để mọi người tìm hiểu.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042109.jpg)

Lập trình viên đều biết, dự án phần mềm hợp tác nhiều người không thể thiếu PR (viết tắt của pull request), nếu bạn muốn sửa code của người khác, hoặc muốn code của mình được merge vào nhánh chính, cần phải tạo một PR. Nhưng, đây là thao tác rất nặng, dù bạn chỉ sửa một ký tự, cũng phải clone toàn bộ kho code, sau đó mới có thể gửi yêu cầu.

PR nhẹ được thiết kế để giải quyết điểm đau này. Với những sửa đổi nội dung ít (ví dụ lỗi đánh máy trong tài liệu), có thể hoàn thành trực tiếp trên trang web, bỏ qua bước clone kho code. Trước tiên vào trang source code file, nhấn nút "Chỉnh sửa" ở góc trên phải, vào hộp chỉnh sửa, sau khi sửa và gửi sẽ tạo ra một PR, rất tiện lợi.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042107.jpg)

Nếu cần sửa nhiều file, nhấn nút "Web IDE" bên cạnh, sẽ vào một môi trường phát triển tích hợp trên trang web, sau khi sửa nhiều file cùng lúc gửi là xong.

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050405.jpg)

Nếu bạn chưa dùng Gitee, hoan nghênh [đăng ký](https://gitee.com/login) thử tính năng PR nhẹ. Ngay cả khi tạm thời chưa có nhu cầu lưu trữ code, cũng có thể xem [nhiều dự án mã nguồn mở xuất sắc](https://gitee.com/explore) trên đó, cùng đóng góp cho hệ sinh thái mã nguồn mở trong nước.

## Tin tức

1、[Nơi nguy hiểm nhất (từng tồn tại) trên Trái đất](https://www.sciencealert.com/palaeontologists-say-ancient-sahara-was-most-dangerous-place-in-earth-s-history)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020043001.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020043002.jpg)

Một nhóm nhà nghiên cứu gần đây đã xem xét các hóa thạch ở một địa điểm gọi là Kem Kem beds ở Morocco, Bắc Phi, xác nhận sự tồn tại của nhiều mảnh vỡ tàn tích sinh vật cổ đại. Vì vậy, họ cho rằng 100 triệu năm trước, đó là một hồ nước nơi các loài động vật ăn thịt lớn tụ cư, được coi là nơi nguy hiểm nhất trên Trái đất.

Trong số 10 loài khủng long ăn thịt lớn nhất được biết đến, bốn loài có hóa thạch xuất hiện ở địa điểm này. Ngoài ra, nơi này còn có nhiều loài cá nước ngọt khổng lồ, trong đó có một con cá mập nước ngọt khổng lồ Onchopristis, có răng sắc như dao găm. Vô số sinh vật đến nơi này bị xé vụn, trở thành hóa thạch ngày nay.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020043003.jpg)

2、[Hệ điều hành điện thoại cho trẻ em](https://techless.com/news-posts/kid-safe-smartphone-launch)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020043004.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020043005.jpg)

Một công ty khởi nghiệp Mỹ ra mắt hệ điều hành điện thoại cho trẻ em KidOS, chỉ có thể gọi điện, nhắn tin và chụp ảnh, không thể lên mạng và xem video, ngoài ra còn có một số công cụ nhỏ, ví dụ đồng hồ và máy tính.

Nó dựa trên hệ thống Android, có thể cài đặt trên điện thoại Android hiện có. Giao diện khá đơn giản, thậm chí không có icon, trông rất tươi sáng.

3、[CPU Intel Core thế hệ thứ 10](https://www.intel.com/content/www/us/en/products/docs/processors/core/10th-gen-processors.html)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020043006.jpg)

Ngày 30 tháng 4, Intel ra mắt CPU Core desktop thế hệ thứ 10, flagship i9-10900K có 10 nhân, tần số cơ bản là 3,7GHz, cao nhất có thể đạt 5,3GHz. Nó có nhiều nhân hơn và hiệu năng tốt hơn so với i9-9900K thế hệ trước, nhưng giá bán không tăng, giá chính thức đều là 488 đô la. Điều này chủ yếu để đối phó với cuộc tấn công mạnh mẽ từ AMD.

Tuy nhiên, quy trình sản xuất thế hệ thứ 10 vẫn là 14nm, vì vậy không giống sản phẩm thế hệ mới, mà giống phiên bản nâng cao hiệu năng của thế hệ trước, nhét thêm hai nhân, nâng xung nhịp. Hậu quả là tiêu thụ điện năng tăng mạnh so với thế hệ trước, i9-10900K là 125W, i9-9900K là 95W, cao hơn đến 30W, phải dùng bộ tản nhiệt mạnh hơn.

4、[Chu kỳ lây lan của cúm](https://www.cbsnews.com/news/coronavirus-pandemic-two-years-70-percent-immunity/)

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050301.jpg)

Trung tâm Nghiên cứu Bệnh Truyền nhiễm Đại học Minnesota gần đây đã nghiên cứu tám đại dịch cúm từ thế kỷ 18 đến nay. Các nhà khoa học phát hiện bảy trong số đó, sau sáu tháng kể từ khi đỉnh điểm đầu tiên qua đi, xuất hiện đỉnh điểm lây nhiễm thứ hai. Đại dịch năm 1918, đỉnh điểm đầu tiên qua đi khi mùa hè đến, nhưng đến cuối thu xuất hiện đỉnh điểm thứ hai, chết nhiều người hơn đỉnh điểm đầu tiên.

Đại dịch trung bình cần 18 đến 24 tháng mới lắng xuống, vì lúc đó 70% cá thể trong toàn bộ quần thể đã có miễn dịch. Vì vậy, các nhà khoa học Mỹ cho rằng virus COVID-19 lắng xuống hoàn toàn, có thể cũng cần thời gian dài như vậy.

5、[Biến CO2 thành khoáng vật](https://eos.org/articles/basalts-turn-carbon-into-stone-for-permanent-storage)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042105.jpg)

Hiện tại, các quốc gia trên thế giới đều đang nghiên cứu công nghệ thu giữ CO2, để giảm hàm lượng CO2 trong khí quyển. Hình trên là nhà máy địa nhiệt Hellisheiði ở Iceland, đây là nhà máy địa nhiệt lớn thứ ba thế giới, nơi đang tiến hành thí nghiệm biến CO2 thành khoáng vật.

Nhà máy phát điện này nằm trên nham thạch núi lửa giàu đá bazan, đá bazan chứa nồng độ cao ion canxi và magiê, có thể phản ứng hóa học với CO2, tạo ra calcite, dolomite và magnesite. Các nhà khoa học trước tiên hòa tan CO2 vào nước, sau đó bơm vào vài trăm mét dưới lòng đất, để đá bazan hấp thụ và biến thành khoáng vật cacbonat, từ đó để đá dưới lòng đất hấp thụ CO2.

6、**Tin tức một câu**

> - [Facebook](https://venturebeat.com/2020/04/29/facebook-open-sources-blender-a-chatbot-that-people-say-feels-more-human/) mã nguồn mở framework chatbot Blender, được cho là chatbot mạnh mẽ nhất thế giới hiện nay, sử dụng đến 9,4 tỷ tham số, nhiều hơn 3,6 lần so với hệ thống trước đây.

> - [OpenAI](https://openai.com/blog/jukebox/) phát hành trình tạo bài hát Jukebox, có thể tự động tạo ra bài hát do một ca sĩ nào đó hát. Bạn nghe thấy có lời bài hát, nhưng thực ra không có, chỉ là mô phỏng giọng ca sĩ ghép lại. Nghe thử bài hát Tori Amos do máy tạo ra dưới đây, hiệu quả rất ấn tượng, [link này](https://jukebox.openai.com/?song=802871497) có nhiều bài hát hơn.

> - [Chính phủ Pháp](https://www.cyclingweekly.com/news/latest-news/france-offers-each-cyclist-e50-for-bike-repairs-once-lockdown-ends-455140) tuyên bố, mỗi người Pháp đi xe đạp đều có thể nhận được 50 euro quỹ sửa chữa, không thể rút tiền mặt, chỉ có thể khấu trừ phí sửa xe đạp. Đây là để cải thiện chất lượng không khí, khuyến khích đi xe đạp nhiều hơn.

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050201.jpg)

> - [Tỉnh Tứ Xuyên](http://scnews.newssc.org/system/20200429/001063516.html) trưng bày kết quả khảo cổ dưới nước trục vớt "kho bạc chìm xuống sông của Trương Hiến Trung năm 1646", phát hiện một con dấu vàng nặng khoảng 16 cân, hàm lượng vàng đạt 95%, trên đó khắc chữ "蜀世子宝", đây là con dấu của con trai Vương Thục thời Minh (tổng cộng mười ba đời), là vật Zhang Xianzhong cướp được.

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050209.jpg)

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050210.jpg)

> - [Một kỹ sư Nhật Bản](https://www.kocpc.com.tw/archives/319919) trong cuộc họp video từ xa, để không cho người khác thấy phòng lộn xộn, đã phát minh ra một tấm nền bằng bìa cứng có thể "mặc" được.

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050211.jpg)

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050212.jpg)

> - [Chính phủ Ấn Độ](https://www.reuters.com/article/us-health-coronavirus-india-app-idUSKBN22E07K) yêu cầu tất cả nhân viên trên toàn quốc đều phải cài đặt một app điện thoại gọi là Aarogya Setu (Cầu Sức khỏe), dùng để theo dõi người đã tiếp xúc trong cuộc sống.

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050302.jpg)

## Bài viết

1、[Tôi đã xây dựng cluster Kubernetes của riêng mình như thế nào](https://blog.quickbird.uk/domesticating-kubernetes-d49c178ebc41)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050104.jpg)

Tác giả trước tiên giới thiệu khái niệm Kubernetes (lớp hệ thống ảo hóa trên cơ sở hạ tầng phân tán), sau đó giới thiệu cách dùng máy tính cũ ở nhà (hình trên) để lắp ráp một cluster.

2、[Cách xây dựng tìm kiếm toàn văn bằng SQLite？](https://24ways.org/2018/fast-autocomplete-search-for-your-website/)（Tiếng Anh）

Đối với các trang web vừa và nhỏ, dùng SQLite để xây dựng tìm kiếm toàn văn, hoàn toàn có thể đáp ứng nhu cầu. Mặc dù tính năng không bằng Elasticsearch, nhưng chi phí và độ phức tạp thấp hơn nhiều.

3、[Tại sao Serverless quan trọng？](https://www.vladimircicovic.com/2019/07/why-is-serverless-important)（Tiếng Anh）

Bài giải thích khái niệm Serverless, rất đơn giản rõ ràng, phù hợp cho người mới tìm hiểu nó là gì.

4、[Tôi đã thu nhỏ file Docker image như thế nào](https://hampton.pw/posts/shrinking-this-sites-docker-image/)（Tiếng Anh）

Tác giả giới thiệu cách sửa file Dockerfile, làm cho kích thước file image của một dự án Node.js, từ 419MB thành 39MB. Phương pháp của ông có giá trị thông dụng cao, đơn giản và thực dụng.

5、[So sánh lương kỹ sư phần mềm ở các thành phố lớn châu Âu và Mỹ](https://javednissar.ca/comparing-software-engineer-salaries-across-cities/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050401.jpg)

Tác giả xem xét cả lương, thuế và chi phí sinh hoạt, so sánh thu nhập ròng của kỹ sư phần mềm ở thành phố nào là lớn nhất.

6、[Cải tạo một chiếc xe tải cũ năm 1953](https://www.cool3c.com/article/153364)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050402.jpg)

Bài báo ảnh, giới thiệu một kỹ sư Mỹ cải tạo một chiếc xe tải năm 1953 (hình trên) thành xe lai điện-xăng như thế nào.

7、[EOF không phải là ký tự](https://ruslanspivak.com/eofnotchar/)（Tiếng Anh）

Ngôn ngữ C thông qua việc kiểm tra dấu hiệu EOF để tìm cuối chuỗi file. Nhưng, bản thân dấu hiệu EOF không phải là ký tự, ký tự cuối cùng của file cũng không phải là nó.

8、[Kiểm thử CPU x86 sản xuất tại Trung Quốc](https://www.anandtech.com/show/15493/hygon-dhyana-reviewed-chinese-x86-cpus-amd)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202003/bg2020031003.jpg)

Năm 2016, AMD bán giấy phép thiết kế CPU Zen x86 thế hệ đầu tiên cho Trung Quốc, và thành lập công ty liên doanh. Bài viết này là kết quả kiểm thử CPU x86 sản xuất trong nước của tổ chức nước ngoài.

## Công cụ

1、[Tara](https://tara.ai/)

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050101.jpg)

Phần mềm quản lý dự án Jira bản copy miễn phí.

2、[Insomnia](https://insomnia.rest/)

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050103.jpg)

Phần mềm desktop mã nguồn mở, dùng để đơn giản hóa thiết kế và phát triển API.

3、[pipedream](https://rss.pipedream.com/)

Dịch vụ xử lý mã nguồn mở, dùng để xử lý nội dung RSS. Ví dụ, một khi nhận được nội dung mới, sẽ gửi một email, hoặc gửi đến Twitter, Slack hoặc các dịch vụ Web khác.

4、[Sitesauce](https://sitesauce.app/)

Một dịch vụ trả phí rất thú vị, tự động chuyển đổi trang web động (ví dụ WordPress) thành trang web tĩnh, giữ nội dung đồng bộ.

5、[uPlot](https://github.com/leeoniya/uPlot)

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050206.jpg)

Thư viện biểu đồ trang web nhỏ gọn bằng JS, dùng để render nhanh tập dữ liệu siêu lớn, chiếm ít tài nguyên hệ thống.

6、[CodePen hỗ trợ framework Flutter](https://medium.com/flutter/announcing-codepen-support-for-flutter-bb346406fe50)

CodePen bây giờ có thể chạy code Flutter trên trang web, đây có một [demo Nike Store](https://codepen.io/joshuadeguzman/pen/jObrzJB) viết bằng framework Flutter, có thể chỉnh sửa trực tuyến và xem trước. Các bạn muốn trải nghiệm Flutter không cần phải dựng môi trường trên máy trước nữa. (@[jwenjian](https://github.com/ruanyf/weekly/issues/1211) đóng góp)

7、[Nền tảng phỏng vấn trực tuyến Coderlane](https://coderlane.net/)

Người dùng có thể tạo lời mời phỏng vấn trực tuyến trong 5 giây trên trình duyệt, hỗ trợ lập trình cộng tác trực tuyến, đồng bộ nhiều người dùng. (@[monsterooo](https://github.com/ruanyf/weekly/issues/1213) đóng góp)

8、[liandi](https://github.com/88250/liandi)

Phần mềm ghi chú Markdown desktop sản xuất trong nước. (@[YLongo](https://github.com/ruanyf/weekly/issues/1218) đóng góp)

9、[PicPlus](https://www.coolapk.com/apk/name.gudong.pic)

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050208.jpg)

Ứng dụng Android, hỗ trợ tải ảnh điện thoại lên image hosting (Qiniu Cloud, Alibaba Cloud, Upyun, GitHub, Gitee, v.v.). (@[maoruibin](https://github.com/ruanyf/weekly/issues/1216) đóng góp)

10、[makeJs](https://github.com/zuluoaaa/makeJs)

Dự án demo, trình thông dịch JS viết bằng JS, có thể dùng để học nguyên lý biên dịch. (@[zuluoaaa](https://github.com/ruanyf/weekly/issues/1222) đóng góp)

## Tài nguyên

1、[Ảnh miễn phí từ Bảo tàng Anh](https://www.britishmuseum.org/collection)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042907.jpg)

Bảo tàng Anh gần đây đã cập nhật trang web của mình, hiện cung cấp miễn phí cho công chúng 1,9 triệu ảnh về các hiện vật của họ.

2、[Hình nền Ghibli](http://www.ghibli.jp/info/013251/)

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050102.jpg)

Studio Ghibli của Miyazaki Hayao phát hành một loạt ảnh hoạt hình, có thể tải xuống miễn phí, dùng làm hình nền hội nghị từ xa trong thời dịch bệnh. Hình trên là hình nền phim "My Neighbor Totoro".

3、[Mô phỏng 3D lăng mộ Ramesses VI](https://my.matterport.com/show/?m=NeiMEZa9d93&mls=1)

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050205.jpg)

Trang web này là mô phỏng cảnh thực 3D của lăng mộ Ramesses VI của Ai Cập cổ đại (khoảng năm 1145 TCN đến khoảng 1137 TCN tại vị), hiệu quả rất tốt, chi tiết phóng to lên đều rõ ràng, điện thoại cũng có thể duyệt.

4、[Tutorial biểu thức chính quy cho người bình thường](https://refrf.shreyasminocha.me/)

Sách giáo trình tiếng Anh miễn phí, giới thiệu biểu thức chính quy cho người mới bắt đầu, có nhiều ví dụ thực tế.

5、[Lập trình Web hiện đại từ cơ bản đến nâng cao](https://fullstackopen.com/zh/)

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050207.jpg)

Phiên bản tiếng Trung của khóa học full-stack công khai của Phần Lan. (@[RichardStark](https://github.com/ruanyf/weekly/issues/1214) đóng góp)

6、[Tutorial OpenGL ES tối giản cho Android](https://github.com/githubhaohao/NDK_OpenGLES_3_0)

Để giúp developer Android nhanh chóng làm quen với phát triển OpenGL ES (giao diện đồ họa ba chiều), tác giả đã tạo ra tutorial tối giản tiếng Trung, bao gồm kiến thức lý thuyết cơ bản và ứng dụng thực tiễn. (@[githubhaohao](https://github.com/ruanyf/weekly/issues/1215) đóng góp)

7、[Bản dịch tiếng Trung Pragmatic Programmer](https://github.com/caicaishmily/pragmatic-programmer-zh)

Người dịch mất hai tháng để dịch 《Pragmatic Programmer》 sang tiếng Trung. (@[caicaishmily](https://github.com/ruanyf/weekly/issues/1220) đóng góp)

## Hình ảnh

1、[Điểm không thể đến được ở Nam Cực](https://en.wikipedia.org/wiki/Pole_of_inaccessibility#Southern_pole_of_inaccessibility)

"Điểm không thể đến được" chỉ địa điểm khó đến nhất. "Điểm không thể đến được ở Nam Cực" là địa điểm xa biển nhất trên lục địa Nam Cực (chấm đỏ trong hình dưới), cách cực Nam địa lý khoảng 878 km.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020022003.jpg)

Ngày 14 tháng 12 năm 1958, một đội gồm 18 người của Đoàn thám hiểm Nam Cực lần thứ 3 của Liên Xô đã đến địa điểm này. Đội thám hiểm sử dụng máy kéo, mang theo một ngôi nhà nhỏ cho bốn người sử dụng, một nhà vô tuyến và một nhà điện, có kế hoạch xây dựng một trạm khảo sát vĩnh cửu ở đó.

Ngày 26 tháng 12, đội thám hiểm từ bỏ xây dựng trạm khảo sát, toàn bộ rút lui, vì nơi đó quá xa các trạm khảo sát khác, khó có thể đóng quân vĩnh cửu, chỉ có thể ghé thăm ngắn hạn. Trước khi rút lui, họ dựng lên một tượng bán thân Lenin phía trên trạm khảo sát.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020022005.jpg)

Nhiều năm sau, các nhà thám hiểm đến thăm lại trạm, phát hiện toàn bộ trạm khảo sát đã bị tuyết chôn vùi, hoàn toàn không nhìn thấy được, tượng Lenin chỉ còn một nửa, dựng trên tuyết.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020022006.jpg)

## Bài đọc thêm

1、[Tại sao phải học đại học？](https://amgreatness.com/2020/04/29/the-long-decline-of-american-higher-education-has-begun/)

Nhà kinh tế học Mỹ Bryan Caplan đã viết một cuốn sách, nghiên cứu tại sao mọi người muốn học đại học.

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050202.jpg)

Ông phát hiện, việc học đại học xuất phát từ ba động cơ.

1) Muốn học một số thứ, dù là bồi dưỡng thế giới quan hay phát triển kỹ năng thực hành.

2) Muốn quen biết những người thông minh, trở thành bạn bè với họ.

3) Muốn chứng minh với nhà tuyển dụng rằng mình đủ thông minh, có khả năng hoàn thành công việc.

Đây cũng có thể nói là ba chức năng của đại học, rất khó phân tách hoàn toàn: đại học không thể chỉ cung cấp một trong số đó, không cung cấp hai cái còn lại. Ngay cả khi bạn chỉ muốn đạt được một trong ba lợi ích, cũng phải học đại học trọn vẹn.

Trong ba động cơ này, động cơ mạnh nhất thực ra là động cơ thứ ba, vì hiệu quả của nó rõ ràng nhất. Khó khăn của động cơ thứ nhất là, dù bạn học thêm gấp đôi kỹ năng mới (ví dụ lấy thêm bằng thứ hai), cũng không thể nhận được mức lương gấp đôi. Thực tế, tăng trưởng lương do học thêm khóa học đại học mang lại, đến một mức độ nhất định thì không còn rõ ràng nữa.

Vì vậy, để thúc đẩy tuyển sinh, đại học nên tìm cách tăng cường động cơ thứ ba, làm cho sinh viên xuất sắc dễ được nhà tuyển dụng nhận ra hơn.

Ví dụ, đánh giá điểm thang 100 tốt hơn thang ABCD bốn cấp độ, vì dễ nổi bật sinh viên xuất sắc hơn. Ngoài ra, nâng cao độ khó tốt nghiệp, làm cho một bộ phận sinh viên không thể lấy được bằng, thực ra cũng có lợi cho việc tuyển thêm sinh viên.

2、[Hằng số Brun và Bug CPU](https://buzzorange.com/techorange/2019/11/08/intel-pentium-bug/)

Thời Hy Lạp cổ đại, Euclid đã chứng minh số nguyên tố có vô số. Các nhà toán học đời sau phát hiện, tính từ 1, số càng lớn, phân bố của số nguyên tố càng thưa; nhưng kỳ lạ là, dù phân bố thưa đến đâu, chỉ cần xuất hiện một số nguyên tố, có thể tìm thấy một số nguyên tố khác gần nó, ví dụ 41 và 43, 101 và 103, 10007 và 10009, chúng đều cách nhau 2.

Các nhà toán học gọi các số nguyên tố liên tiếp cách nhau 2 là "số nguyên tố sinh đôi".

Năm 1919, nhà toán học Na Uy Viggo Brun chứng minh, tổng nghịch đảo của tất cả các cặp số nguyên tố sinh đôi hội tụ về một hằng số. Số này được gọi là hằng số Brun.

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050203.jpg)

Nhưng, các nhà toán học không thể chứng minh hằng số Brun có phải là số vô tỷ không, tức là không thể chứng minh số lượng số nguyên tố sinh đôi là hữu hạn hay vô hạn. Vấn đề này khiến các nhà toán học đau đầu hàng nghìn năm, được gọi là "Giả thuyết số nguyên tố sinh đôi", là vấn đề khó kinh điển trong toán học.

Sau khi máy tính ra đời, các nhà toán học thử dùng phương pháp brute force, dùng máy tính tính toán hằng số Brun, cố gắng giải quyết giả thuyết số nguyên tố sinh đôi, nhưng đến nay vẫn chưa giải quyết được.

Năm 1994, Intel ra mắt bộ xử lý Pentium, đây là một trong những bộ xử lý tiên tiến nhất lúc bấy giờ. Giáo sư toán học Mỹ Thomas Nicely dùng nó để tính hằng số Brun.

![](https://cdn.beekka.com/blogimg/asset/202005/bg2020050204.jpg)

Để giảm rủi ro tính sai, Nicely đồng thời sử dụng hai phương pháp tính hằng số Brun. Sau khi tính toán thực tế, ông phát hiện giá trị tính bằng hai cách chênh lệch nhau nhiều.

Sau khi kiểm tra, Nicely phát hiện vấn đề nằm ở việc máy tính tính sai chữ số thập phân thứ 10 của nghịch đảo cặp số nguyên tố sinh đôi 824.633.702.441 và 824.633.702.443.

Để xác nhận vấn đề này nằm ở phần cứng hay phần mềm, Nicely tính bằng CPU 486 phiên bản cũ của Intel, phát hiện số 486 tính ra là đúng. Vì vậy, xác nhận vấn đề nằm ở bộ xử lý Pentium.

Nicely liên hệ Intel, thông báo vấn đề bộ xử lý Pentium, nhưng bị đối xử lạnh nhạt. Ông liền viết thư kể chuyện này với bạn bè, sau đó được CNN và các phương tiện truyền thông lớn đưa tin, Intel không thể không thu hồi bộ xử lý Pentium trên thị trường. Lúc đó đã bán hơn 1 triệu chiếc máy tính có bộ xử lý Pentium, do thu hồi, Intel thiệt hại 475 triệu đô la.

Sau đó Intel thừa nhận, khi sản xuất Pentium đã phát hiện vấn đề rồi, nhưng Intel cho rằng chỉ có 1 trong 9 tỷ người dùng bị ảnh hưởng, nên không thu hồi. Vấn đề này sau đó được gọi là Pentium FDIV bug.

## Danh ngôn

1、

Bạn ghi nhớ số điện thoại bằng ngôn ngữ nào, đó là tiếng mẹ đẻ của bạn.

-- Người dùng Twitter

2、

Khi gặp logic cực kỳ phức tạp, tôi thích viết từng bước thành một biến, làm cho nó đọc như tiếng Anh.

-- [Người dùng Hacker News](https://news.ycombinator.com/item?id=23051063)

3、

Indonesia rất may mắn, có quá nhiều đảo (tổng cộng 17.508 đảo), hạn chế việc đi lại của mọi người, vì vậy số người nhiễm virus không nhiều lắm.

-- [Một nhà dịch tễ học Indonesia](https://www.nytimes.com/2020/05/03/world/asia/coronavirus-spread-where-why.html)

4、

Mọi người không muốn giá thấp, họ muốn đồ rẻ.

-- [《Giá thấp không bằng đồ rẻ》](https://creativesamba.substack.com/p/the-low-prices-vs-bargains-dilemma-20-01-27)

5、

Khoa học yêu cầu khả năng tái tạo, người khác có thể tái tạo kết quả của bạn. Kinh doanh thì không, yêu cầu không thể tái tạo, người khác tốt nhất không thể sao chép mô hình kinh doanh của bạn.

-- [《Nghệ thuật kết hợp kinh doanh và khoa học》](https://www.younglingfeynman.com/essays/artofbusiness)

6、

Hội chứng tất thứ hai chỉ việc đan tất đầu tiên thường rất nhanh. Nhưng cái thứ hai thì bị trì hoãn, không bao giờ hoàn thành, cũng không đặt nó lên đầu tiên trong danh sách công việc.

-- [《Hội chứng tất thứ hai》](https://sheepamongwolves.net/2018/09/second-sock-syndrome-what-it-is-and-how-to-fight-it/)

## Nhìn lại

- Tuần này năm 2019: [số 55](http://www.ruanyifeng.com/blog/2019/05/weekly-issue-55.html)
- Tuần này năm 2018: [số 3](http://www.ruanyifeng.com/blog/2018/05/weekly-issue-3.html)

## Đăng ký

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97).

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
