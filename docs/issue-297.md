# Bản tin chia sẻ công nghệ (Số 297): Đồ chơi chim uống nước

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/4204) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041107.webp)

Khu vực Trung Hoàn, Hồng Kông được trang trí hơn 200 mô hình "trứng phát sáng" có kích thước từ 3 đến 5 mét, được bố trí một phần trên cạn và một phần nổi trên mặt biển. Khi màn đêm buông xuống, các mô hình này sẽ tự động phát ra các ánh sáng màu sắc và âm thanh hiệu ứng đa dạng. (Nguồn: [Sohu](https://www.sohu.com/a/766773393_123753))

## 饮水鸟玩具

Mấy ngày trước, tôi vô tình thấy một bài giới thiệu về món đồ chơi vật lý mang tên "chim uống nước" (drinking bird), thấy tò mò và hứng thú nên đã đặt mua một chiếc trên mạng.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041303.webp)

Giá bán của món đồ này rất rẻ, chỉ khoảng mười mấy Nhân dân tệ. Sau khi nhận hàng và chơi thử, tôi nhận thấy đây là một thiết bị rất thú vị nên muốn chia sẻ tới mọi người.

Nó hoạt động như một công cụ vật lý mô phỏng cỗ máy chuyển động vĩnh cửu. Bạn chỉ cần ấn đầu chú chim cúi xuống cốc nước lạnh để phần mỏ chạm vào nước, sau đó chú chim sẽ tự động thực hiện chu kỳ đứng thẳng lên, cúi xuống, đứng lên, cúi xuống liên tục không ngừng...

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041304.webp)

Chú chim tôi đặt mua đã hoạt động liên tục như vậy suốt một ngày một đêm mà chưa hề có dấu hiệu dừng lại.

Điều thú vị nhất nằm ở nguyên lý vận hành vật lý của thiết bị mà có thể bạn chưa từng nghĩ tới.

Trước tiên, nếu lược bỏ toàn bộ các lớp trang trí bên ngoài, bản chất thiết bị chỉ là một ống thủy tinh kín có hình dạng đặc biệt.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041305.webp)

Hai đầu thiết bị là hai khoang hình cầu được kết nối với nhau bằng một ống thủy tinh ở giữa, phần khoang dưới chứa một lượng dung dịch chất lỏng dễ bay hơi (như dichloromethane, ether hoặc cồn).

Phần mỏ chim được bao phủ bằng một lớp nỉ dạ giúp giữ nước lạnh bám trên bề mặt lâu hơn.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041807.webp)

Khi mỏ chim chạm vào nước lạnh, nhiệt độ thấp kết hợp với quá trình bay hơi của nước sẽ làm nhiệt độ ở khoang trên giảm đi, kéo theo áp suất không khí ở khoang trên giảm xuống thấp hơn áp suất ở khoang dưới.

Sự chênh lệch áp suất này sẽ đẩy phần dung dịch chất lỏng từ khoang dưới đi dọc theo ống thủy tinh di chuyển lên khoang trên.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041808.webp)

Khi chất lỏng dồn lên phía trên làm cho đầu chim nặng dần, khiến trọng tâm thay đổi và đầu chim tự động đổ gục xuống cốc nước tạo tư thế uống nước.

Khi thân chim nằm nghiêng, phần đầu ống thủy tinh ở khoang dưới sẽ nhô ra khỏi bề mặt dung dịch chất lỏng, cho phép không khí lưu thông qua ống thủy tinh làm áp suất giữa hai khoang lập tức cân bằng trở lại.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041809.webp)

Dưới tác động của trọng lực, phần dung dịch chất lỏng ở khoang trên sẽ tự động chảy ngược trở lại khoang dưới, làm trọng tâm dịch chuyển về phía sau và đầu chim tự động ngóc dậy đứng thẳng lên.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041810.webp)

Chu trình này sẽ liên tục được lặp lại miễn là phần nước lạnh ở mỏ chim duy trì được sự chênh lệch nhiệt độ giữa hai khoang trên và dưới. **Về bản chất nhiệt động học, chim uống nước là một động cơ nhiệt hoạt động hoàn toàn dựa trên sự chênh lệch nhiệt độ môi trường mà không cần bất kỳ nguồn năng lượng hay pin cung cấp bên ngoài.**

Tôi đánh giá đây là một mô hình trực quan tuyệt vời giúp mô tả quá trình chuyển hóa nhiệt năng thành cơ năng. Tuy nhiên, ngoài ứng dụng làm đồ chơi giáo dục, tôi hầu như chưa thấy thiết bị này được đưa vào ứng dụng thực tế nào khác trong đời sống.

Mới đây tôi có đọc được [một bài viết](https://www.cnn.com/2024/03/14/climate/drinking-bird-energy-power-gadgets-climate-intl/index.html) chia sẻ về việc các nhà nghiên cứu [đề xuất](https://www.cell.com/device/fulltext/S2666-9986(24)00108-X) ứng dụng nguyên lý chim uống nước để phát triển thiết bị phát điện mini tận dụng chênh lệch nhiệt độ môi trường. Dù hiệu suất phát điện chắc chắn sẽ rất thấp, nhưng nếu dự án được thương mại hóa thành công thì đây sẽ là một giải pháp công nghệ rất thú vị.

## 掘金动手实验室：HarmonyOS 活动

"Juejin Hands-on Lab" (Phòng thí nghiệm thực hành Juejin) là một chuỗi hoạt động công nghệ lấy trải nghiệm thực tế làm trọng tâm, phối hợp cùng các hãng công nghệ lớn để mang lại cho cộng đồng lập trình viên cơ hội thực hành và sáng tạo trực quan.

Trong sự kiện lần này, **chương trình phối hợp cùng đội ngũ kỹ sư Huawei HarmonyOS để mang đến cơ hội trải nghiệm sớm hệ điều hành HarmonyOS NEXT hoàn toàn mới**, rất thích hợp cho các bạn đang quan tâm đến hệ sinh thái HarmonyOS và lập trình ứng dụng di động.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041706.webp)

Sự kiện mở cửa tự do đón tiếp toàn bộ nhân sự trong ngành bao gồm lập trình viên, nhà thiết kế giao diện UI/UX và các quản lý sản phẩm (Product Managers). Bạn không chỉ được tìm hiểu các tính năng công nghệ mới nhất trên HarmonyOS NEXT từ các chuyên gia Huawei mà còn **có cơ hội trực tiếp thực hành viết mã nguồn**.

Trong nửa sau của chương trình, ban tổ chức sẽ phân chia các nhóm thảo luận để brainstorming tìm kiếm các ý tưởng ứng dụng tiềm năng có thể phát triển trên HarmonyOS. Nếu ý tưởng khả thi, các nhóm có thể trực tiếp triển khai lập trình sản phẩm ngay tại sự kiện để làm quen với hệ thống công cụ phát triển của hãng. Người tham gia có thể đăng ký theo nhóm đông người hoặc đăng ký cá nhân.

**Thời gian diễn ra sự kiện kéo dài cả ngày Chủ nhật tuần này (21 tháng 4), hoàn toàn miễn phí tham dự**, địa điểm tổ chức tại khu Cao Hà Kính, Thượng Hải. Người tham gia có cơ hội nhận suất trải nghiệm bản thử nghiệm beta của HarmonyOS NEXT cùng nhiều phần quà hấp dẫn cho các nhóm chiến thắng.

Để đăng ký tham gia và xem chi tiết lịch trình sự kiện, xin vui lòng quét mã QR trên poster hoặc click vào [Đường link đăng ký này](https://www.bagevent.com/event/8819409?bag_track=ruanyifeng). Sau khi hoàn thành đăng ký, trợ lý chương trình sẽ liên hệ hỗ trợ bạn tham gia vào nhóm WeChat cộng đồng của sự kiện, vui lòng lưu ý kiểm tra thông báo kết bạn WeChat!

## 科技动态

1、[Dự báo hiện tượng thiên văn kỳ thú: Trực tiếp quan sát vụ nổ sao đôi bằng mắt thường](https://phys.org/news/2024-04-huge-star-explosion-sky-lifetime.html)

Trong khoảng thời gian từ nay đến tháng 9 năm nay, người dân trên Trái Đất có cơ hội hiếm có để trực tiếp quan sát bằng mắt thường một vụ nổ sao siêu tân tinh ngoài không gian vũ trụ.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041101.webp)

Nằm cách Trái Đất khoảng 3.000 năm ánh sáng tại chòm sao Bắc Mian (Corona Borealis) có một hệ sao đôi độc đáo với hai ngôi sao chuyển động ở khoảng cách rất gần nhau.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041103.webp)

Chu kỳ khoảng 80 năm một lần, quỹ đạo chuyển động sẽ đưa hai ngôi sao này đến vị trí cực cận gần nhau nhất, lực hấp dẫn cực lớn giữa chúng sẽ kích hoạt phản ứng nổ hạt nhân từ vật chất sâu bên trong ngôi sao tạo nên vụ nổ sáng rực rỡ.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041102.webp)

Nhà thiên văn học người Ireland John Birmingham đã lần đầu tiên ghi nhận hiện tượng này vào năm 1866, sau đó nó tái diễn vào năm 1946. Và năm 2024 này sẽ đánh dấu sự lặp lại của hiện tượng thiên văn kỳ thú đó.

Tuy nhiên có một chi tiết vật lý thú vị là dù vụ nổ chuẩn bị hiển thị trước mắt chúng ta hiện nay, sự kiện thực tế đã diễn ra từ cách đây 3.000 năm trước ngoài không gian.

2、[Trận lũ lụt lịch sử tàn phá cơ sở hạ tầng đô thị tại Dubai](https://finance.eastmoney.com/a/202404173048968557.html)

Vào ngày 17 tháng 4, thành phố Dubai đã phải hứng chịu trận mưa lớn lịch sử có lượng mưa lớn nhất kể từ khi bắt đầu ghi nhận số liệu khí tượng năm 1949.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041707.webp)

Do Dubai nằm trong vùng khí hậu sa mạc khô hạn quanh năm nóng bức và thiếu nguồn nước ngọt tự nhiên nên hệ thống thoát nước đô thị hoàn toàn không được chú trọng đầu tư xây dựng. Trận mưa lớn kéo dài lập tức gây ngập lụt nghiêm trọng trên diện rộng, đẩy toàn bộ thành phố vào trạng thái hỗn loạn.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041708.webp)

Khu vực sân đỗ máy bay rộng lớn của Sân bay Quốc tế Dubai ngập chìm hoàn toàn dưới biển nước, biến sân bay bận rộn bậc nhất thế giới thành một sân bay trên nước.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041801.webp)

Hiện tượng biến đổi khí hậu toàn cầu đang khiến cấu trúc thời tiết thay đổi mạnh mẽ, đẩy nhiều vùng khô hạn vào trạng thái sa mạc hóa sâu sắc hơn trong khi một số khu vực khác lại xuất hiện lượng mưa tăng vọt. Xu hướng mưa lớn xuất hiện thường xuyên tại các vùng sa mạc khô cằn (bao gồm cả vùng Tây Bắc Trung Quốc) đang làm dấy lên giả thuyết liệu các sa mạc có thể chuyển dịch thành các ốc đảo xanh trong tương lai.

3、[Trải nghiệm dịch vụ nhân viên phục vụ từ xa trực tuyến](https://www.nytimes.com/2024/04/11/nyregion/nyc-restaurants-virtual-remote.html)

Cơ sở nhà hàng đặt tại New York, nhưng nhân viên phục vụ lại ngồi làm việc tại Philippines. Khi khách hàng tiếp cận quầy gọi món, màn hình sẽ tự động kích hoạt cuộc gọi video call để kết nối trực tiếp với nhân viên tại Philippines hỗ trợ gọi món.

Sau khi tiếp nhận yêu cầu từ màn hình gọi món, nhân viên tại Philippines sẽ chuyển thông tin đơn hàng về hệ thống máy in trong bếp tại New York để chuẩn bị đồ ăn.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041416.webp)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041417.webp)

Mức lương trả cho nhân viên trực tuyến tại Philippines dao động khoảng 3 USD/giờ - cao gấp đôi mức thu nhập trung bình cho công việc tương đương tại nước sở tại, trong khi mức lương tối thiểu theo luật định tại bang New York hiện nay lên tới 16 USD/giờ.

## Bài viết

1\. [Hướng dẫn xây dựng hệ thống tìm kiếm hình ảnh tương đồng bằng công nghệ Vector Embeddings](https://harper.blog/2024/04/12/i-accidentally-built-a-meme-search-engine/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041406.webp)

Tác giả chia sẻ kinh nghiệm ứng dụng công nghệ nhúng vector (vector embeddings) để tích hợp tính năng tìm kiếm ảnh tương tự cho kho ảnh cá nhân, và nhận thấy quy trình triển khai thực tế đơn giản một cách bất ngờ.

2\. [Mẹo thiết lập hệ thống định tuyến mạng du lịch cùng Tailscale](https://mrkaran.dev/posts/travel-tailscale/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041601.webp)

Một số dịch vụ trực tuyến giới hạn phạm vi truy cập theo địa lý quốc gia. Bài viết hướng dẫn cấu hình định tuyến thông minh qua Tailscale để giúp người dùng khi đi công tác nước ngoài vẫn dễ dàng truy cập và sử dụng bình thường các dịch vụ nội địa ở quê nhà.

3\. [Tối ưu hóa trải nghiệm người dùng đối với các mã định danh UUID](https://unkey.dev/blog/uuid-ux)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041410.webp)

UUID là chuỗi định danh độc bản sử dụng phổ biến trong cơ sở dữ liệu. Bài viết thảo luận các giải pháp thiết kế giao diện giúp hiển thị và quản lý UUID thân thiện hơn đối với người dùng cuối.

Bên cạnh đó bạn đọc có thể tìm hiểu thêm về các phiên bản nâng cấp khác nhau của UUID tại [bài phân tích này](https://blog.daveallie.com/ulid-primary-keys/). Đưa ra khuyến nghị nên sử dụng UUIDv4 cho các nhu cầu định danh thông thường, và ưu tiên UUIDv7 cho các nhu cầu yêu cầu chuỗi có tính tăng dần theo thời gian.

4\. [Phương pháp phân tích tệp tin dump tìm kiếm nguyên nhân gây sập trình duyệt Chrome](https://blog.5udou.cn/blog/detail/1711630845567)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041607.webp)

Trình duyệt Chrome đôi khi bị thoát đột ngột (crash) khi mở một số trang web cụ thể. Tác giả hướng dẫn cách phân tích các tệp tin log ghi nhận lỗi Crash dump để tìm ra nguyên nhân cốt lõi gây sập trình duyệt. (Đóng góp của [@linxiaowu66](https://github.com/ruanyf/weekly/issues/4277))

5\. [Phân tích kích thước dòng code tối ưu cho một bản Pull Request](https://graphite.dev/blog/the-ideal-pr-is-50-lines-long)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021104.webp)

Kích thước dung lượng code bao nhiêu dòng là tối ưu nhất cho một bản Pull Request (PR) gửi lên GitHub? Bài viết nhận định con số 50 dòng là lý tưởng nhất, dao động trong khoảng từ 25 đến 100 dòng là hợp lý.

Các PR dưới 25 dòng thường quá vụn vặt làm gia tăng số lượng commit rác, trong khi các PR vượt quá 100 dòng sẽ làm tăng độ phức tạp logic và tiêu tốn nhiều thời gian kiểm duyệt của đồng nghiệp.

6\. [Góc nhìn phản biện về các hạn chế thiết kế của Tailwind CSS](https://nuejs.org/blog/tailwind-misinformation-engine/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202402/bg2024021901.webp)

Tailwind hiện là một CSS framework rất phổ biến với ưu điểm giúp tái sử dụng mã nguồn CSS nhanh chóng. Tuy nhiên tác giả bài viết đưa ra các phân tích kỹ thuật giải thích vì sao ông không đánh giá cao định hướng thiết kế này của Tailwind.

## 工具

1\. [sshx (Công cụ chia sẻ nhanh cửa sổ Terminal trực tuyến)](https://sshx.io/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110602.webp)

Tiện ích hỗ trợ chia sẻ nhanh giao diện dòng lệnh terminal của bạn cho đồng nghiệp thông qua một đường link URL duy nhất.

2\. [Hyphen (Thư viện cơ sở hỗ trợ thiết kế Web Components)](https://github.com/00000o1/-)

Thư viện lớp cơ sở hỗ trợ lập trình viên xây dựng nhanh các thành phần giao diện Web Components tùy biến của riêng mình. Một dự án có tính năng tương tự khác là [Cami.js](https://github.com/kennyfrc/cami.js).

3\. [Hono (Khung phát triển ứng dụng Web siêu nhẹ)](https://github.com/honojs/hono)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041608.webp)

Khung phát triển ứng dụng web tối giản viết bằng Node.js, được thiết kế tối ưu hóa tốc độ xử lý cho các kịch bản chạy trên hạ tầng Edge Computing.

4\. [Shiro (Bộ giao diện trang cá nhân phong cách tối giản)](https://github.com/Innei/Shiro)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041609.webp)

Bộ template thiết kế trang cá nhân đẹp mắt theo xu hướng tối giản, hoạt động như giao diện Frontend kết nối với hệ quản trị nội dung [Mix Space](https://github.com/mx-space). (Đóng góp của [@Innei](https://github.com/ruanyf/weekly/issues/4274))

5\. [Cover your tracks (Công cụ kiểm tra độ rò rỉ thông tin trình duyệt)](https://firstpartysimulator.org/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110603.webp)

Dịch vụ web hỗ trợ người dùng phân tích xem trình duyệt của mình đang cung cấp bao nhiêu thông tin cấu hình phần cứng cho máy chủ, từ đó tạo nên dấu vân tay trình duyệt (browser fingerprint) duy nhất.

6\. [TeleMonitor (Công cụ giám sát hệ thống qua Telegram)](https://github.com/bboysoulcn/telemonitor)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041403.webp)

Hệ thống giám sát tài nguyên máy chủ viết bằng Python, hỗ trợ theo dõi hiệu năng CPU, RAM, dung lượng ổ đĩa và tự động gửi cảnh báo qua Telegram. (Đóng góp của [@bboysoulcn](https://github.com/ruanyf/weekly/issues/4260))

7\. [Amprobe (Hệ thống giám sát hiệu năng máy chủ và Docker)](https://github.com/amuluze/amprobe)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041404.webp)

Ứng dụng giám sát tài nguyên máy chủ và trạng thái các container Docker gọn nhẹ viết bằng Go và Vue 3. (Đóng góp của [@amuluze](https://github.com/ruanyf/weekly/issues/4261))

8\. [ElemSnap (Tiện ích chụp ảnh màn hình và làm đẹp ảnh chụp)](https://chromewebstore.google.com/detail/elemsnap/mblkhbaakhbhiimkbcnmeciblfhmafna)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041606.webp)

Tiện ích mở rộng trên Chrome hỗ trợ chụp ảnh màn hình trang web, tích hợp sẵn công cụ lồng khung và làm đẹp ảnh chụp chuyên nghiệp trước khi chia sẻ. (Đóng góp của [@AydenGen](https://github.com/ruanyf/weekly/issues/4273))

9\. [stokado (Thư viện tối ưu hóa quản lý lưu trữ trình duyệt)](https://github.com/KID-joker/stokado)

Thư viện JavaScript hỗ trợ đóng gói các đối tượng lưu trữ trình duyệt (như localStorage, IndexedDB), cung cấp API đồng bộ và bổ sung tính năng quản lý thời hạn hết hạn lưu trữ (expiry time). (Đóng góp của [@KID-joker](https://github.com/ruanyf/weekly/issues/4279))

10\. [PPResume (Trình tạo CV chuyên nghiệp bằng LaTeX)](https://ppresume.com/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041802.webp)

Dịch vụ trực tuyến hỗ trợ thiết kế và tạo hồ sơ năng lực (CV) đẹp mắt dựa trên công nghệ biên dịch LaTeX, cho phép xuất file định dạng PDF với chất lượng đồ họa cực cao. (Đóng góp của [@xiaohanyu](https://github.com/ruanyf/weekly/issues/4285))

11\. [Tự luật thạch đầu (Ứng dụng iOS hỗ trợ quản lý thời gian sử dụng điện thoại)](https://apps.apple.com/cn/app/%E8%87%AA%E5%BE%8B%E7%9F%B3%E5%A4%B4-%E8%B5%B0%E8%B7%AF%E8%AF%BB%E4%B9%A6%E6%8D%A2%E6%97%B6%E9%97%B4-%E4%B8%8D%E5%81%9A%E6%89%8B%E6%9C%BA%E6%8E%A7/id6479392365)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041803.webp)

Ứng dụng di động trên iOS giúp hạn chế thời gian truy cập các ứng dụng được cài đặt trên máy nhằm giảm bớt thói quen nghiện sử dụng điện thoại. (Đóng góp của [@tuesda](https://github.com/ruanyf/weekly/issues/4284))

12\. [SoundBug (Trình biên tập và sản xuất âm thanh chuyên nghiệp)](https://www.soundbug.com/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041804.webp)

Phần mềm biên tập âm thanh kỹ thuật số (DAW) được phát triển bởi lập trình viên Trung Quốc, hỗ trợ hòa âm, phối khí và ghi âm với giao diện trực quan thân thiện dễ sử dụng. (Đóng góp của [@asoiso](https://github.com/ruanyf/weekly/issues/4286))

13\. [Moments (Mã nguồn trang blog cá nhân phong cách mạng xã hội)](https://github.com/kingwrcy/moments)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041805.webp)

Mã nguồn mở hỗ trợ xây dựng trang blog cá nhân dạng nhật ký ngắn, mô phỏng thiết kế giao diện mạng xã hội WeChat Moments. Trải nghiệm bản dùng thử [Demo tại đây](https://m.mblog.club/). (Đóng góp của [@kingwrcy](https://github.com/ruanyf/weekly/issues/4288))

14\. [Newcar (Thư viện thiết kế hoạt họa bằng JS trên Canvas)](https://github.com/dromara/newcar)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041806.webp)

Thư viện hoạt họa Frontend viết bằng JS phát triển dựa trên công nghệ WebAssembly của thư viện đồ họa Skia, hỗ trợ vẽ chuyển động hoạt hình mượt mà trên thẻ Canvas. (Đóng góp của [@sheepbox8646](https://github.com/ruanyf/weekly/issues/4287))

## AI 相关

1\. [Suno AI API (Thư viện API không chính thức cho trình tạo nhạc Suno AI)](https://github.com/gcui-art/suno-api)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041401.webp)

Dự án mã nguồn mở hỗ trợ tạo lập các cổng kết nối API để tương tác lập trình tự động với mô hình tạo nhạc Suno AI. (Đóng góp của [@blueeon](https://github.com/ruanyf/weekly/issues/4262))

Bên cạnh đó có thể tham khảo thêm [SunoApi](https://github.com/SunoApi/SunoApi) cung cấp giao diện web client thay thế. (Đóng góp của [@SunoApi](https://github.com/ruanyf/weekly/issues/4263))

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041414.webp)

2\. [Anime Filter (Dịch vụ chuyển đổi ảnh chân dung thành tranh vẽ anime)](https://www.animefilter.online/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041202.webp)

Ứng dụng web phát triển dựa trên mô hình Stable Diffusion hỗ trợ chuyển đổi ảnh chân dung thành các bức vẽ mang ba phong cách đồ họa anime khác nhau. (Đóng góp của [@Lucas-YYB](https://github.com/ruanyf/weekly/issues/4253))

3\. [StockCake (Công cụ tìm kiếm ảnh nghệ thuật tạo bằng AI miễn phí)](https://stockcake.com/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041408.webp)

Thư viện và công cụ tìm kiếm các hình ảnh nghệ thuật được thiết kế bằng công nghệ AI cho phép tải về sử dụng tự do không lo bản quyền.

4\. [StockTune (Thư viện tìm kiếm âm nhạc tạo bằng AI miễn phí)](https://stocktune.com/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041407.webp)

Trang web hỗ trợ tìm kiếm và tải về các đoạn nhạc, bài hát miễn phí được thiết kế bằng AI.

5\. [x-crawl (Thư viện thu thập dữ liệu web hỗ trợ bởi công nghệ AI)](https://github.com/coder-hxl/x-crawl)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041702.webp)

Thư viện crawler thu thập thông tin trang web viết bằng Node.js tích hợp AI hỗ trợ, cho phép người dùng mô tả yêu cầu bóc tách thông tin bằng câu lệnh ngôn ngữ tự nhiên sau khi trang web được tải về. (Đóng góp của [@coder-hxl](https://github.com/ruanyf/weekly/issues/4281))

6\. [DeepLearning Interview Awesome 2024](https://github.com/315386775/DeepLearing-Interview-Awesome-2024)

Kho lưu trữ chia sẻ bộ câu hỏi ôn luyện phỏng vấn tuyển dụng dành riêng cho khối ngành nghiên cứu và phát triển AI. (Đóng góp của [@315386775](https://github.com/ruanyf/weekly/issues/4278))

## 资源

1\. [Tổng hợp tệp tin thiết kế vector huy hiệu logo các trường Đại học Trung Quốc](https://www.urongda.com/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041201.webp)

Trang web chia sẻ các file đồ họa vector chất lượng cao mô tả logo hiệu huy hiệu của hơn 100 trường đại học tại Trung Quốc. (Đóng góp của [@incidunt](https://github.com/ruanyf/weekly/issues/4252))

2\. [Tổng hợp các nguồn tài liệu học tập miễn phí về Generative AI và LLMs](https://pankajpipada.com/posts/2024-04-15-genai-resources/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041501.webp)

Danh sách tổng hợp chọn lọc hơn mười nguồn học tập trực tuyến chất lượng cao về trí tuệ nhân tạo tạo sinh được chia sẻ miễn phí.

3\. [Bản dịch tiếng Trung tài liệu thực hành hạt nhân Linux Labs](https://linux-kernel-labs-zh.xyz/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041605.webp)

Bản dịch tiếng Trung của bộ tài liệu thực hành phát triển Driver hệ thống Linux Labs danh tiếng của Đại học Quốc gia Politehnica Bucharest. (Đóng góp của [@hanyujie2002](https://github.com/ruanyf/weekly/issues/4269))

## 图片

1\. [Hình ảnh sai sót minh họa cho Định lý Pythagore](https://mathtourist.blogspot.com/2009/02/pondering-artists-perplexing-tribute-to.html)

Số phát hành tháng 1 năm 2009 của Tạp chí Toán học Đại học (College Mathematics Journal - CMJ) đã lựa chọn hình vẽ minh họa cho Định lý Pythagore làm ảnh bìa.

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024041409.webp)

Bức ảnh vẽ minh họa này lại vấp phải nhiều sự tranh cãi của giới toán học do phát hiện lỗi sai hình học cơ bản.

Ba cạnh của tam giác vuông trong hình được vẽ với tỷ lệ độ dài 2 - 3 - 4. Với tỷ lệ này, theo định lý đảo của định lý Pythagore thì tam giác này bắt buộc phải là tam giác tù chứ không thể là tam giác vuông.

## ✍️ Bài đọc thêm

### Lịch sử ra đời của công nghệ chụp ảnh tốc độ cao

*Nội dung dưới đây được lược dịch từ tác phẩm "Con số không biết nói dối" (Numbers Don't Lie) của tác giả khoa học Vaclav Smil.*

Vào năm 1867, cựu Thống đốc bang California đã liên hệ với nhiếp ảnh gia Eadweard Muybridge (1830-1904) để nhờ ông giải quyết một cuộc tranh cãi học thuật kéo dài: **liệu khi ngựa phi nước kiệu, có khoảnh khắc nào cả bốn chân của nó đều nhấc hoàn toàn khỏi mặt đất hay không?**

Nhiếp ảnh gia nhận thấy đây là một thử thách kỹ thuật cực kỳ lớn do tốc độ màn trập của các dòng máy ảnh thời kỳ đó quá chậm khiến các bức ảnh chụp được đều bị nhòe hình và không thể quan sát rõ nét.

Để giải quyết vấn đề, ông đã nỗ lực tìm kiếm giải pháp rút ngắn tốc độ màn trập và đến năm 1878 đã chế tạo thành công chiếc máy ảnh có tốc độ màn trập đạt mức 1/1.000 giây (tương đương tốc độ chụp 1.000 khung hình/giây) chuyên dụng để ghi hình các vật thể chuyển động siêu nhanh.

Vào ngày 19 tháng 6 năm 1878, buổi thực nghiệm lịch sử đã được tổ chức tại trang trại Palo Alto thuộc Đại học Stanford. Nhiếp ảnh gia bố trí các phim âm bản trên một đĩa quay tốc độ cao để chụp lại liên tục chuyển động của chú ngựa đang phi nước đại.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023110607.webp)

Các bức ảnh khôi phục rõ nét đã đưa ra câu trả lời thuyết phục: khi phi nước đại, thực sự có những khoảnh khắc cả bốn móng guốc của chú ngựa đều rời khỏi mặt đất hoàn toàn.

Kỹ thuật chụp ảnh tốc độ cao này sau đó liên tục được nghiên cứu cải tiến, nâng tốc độ chụp từ 1.000 khung hình/giây lên mức 10.000 khung hình/giây.

Đến năm 1940, thiết kế máy ảnh phản chiếu gương xoay đã nâng tốc độ chụp đạt mức kỷ lục 1 triệu khung hình/giây.

Vào năm 1999, nhà khoa học Ahmed Zewail đã vinh dự nhận giải Nobel Hóa học nhờ công trình phát triển máy quang phổ có khả năng chụp lại sự dịch chuyển trạng thái của các phản ứng hóa học trong khoảng thời gian siêu ngắn femtoseconds (10⁻¹⁵ giây).

Ngày nay, các nhà khoa học thậm chí có thể ứng dụng các chùm tia laser siêu nhanh để ghi nhận các sự kiện diễn ra ở khoảng cách thời gian attoseconds (10⁻¹⁸ giây) - tốc độ chụp khủng khiếp cho phép con người ghi hình được cả chuyển động của các hạt electron.

## Lịch sử tuần này

- 2023年（第 250 期）：[Góc nhìn công nghệ: Rủi ro tiềm ẩn của các công nghệ mới nổi đối với xã hội](https://www.ruanyifeng.com/blog/2023/04/weekly-issue-250.html)
- 2022年（第 200 期）：[Triết lý công việc: Bí quyết duy trì kỳ vọng thấp và thử nghiệm nhiều hướng đi khác nhau](https://www.ruanyifeng.com/blog/2022/03/weekly-issue-200.html)
- 2021年（第 150 期）：[Góc nhìn nghệ thuật: Hoài niệm về thời kỳ âm nhạc còn là dịch vụ khan hiếm](https://www.ruanyifeng.com/blog/2021/03/weekly-issue-150.html)
- 2020年（第 100 期）：[Nhận định kinh tế: Xu hướng phát triển kinh tế toàn cầu trong kỷ nguyên lãi suất bằng không](https://www.ruanyifeng.com/blog/2020/03/weekly-issue-100.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
