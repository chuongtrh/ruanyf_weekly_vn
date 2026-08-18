# Bản tin chia sẻ công nghệ (Số 327): Kỷ nguyên Internet không liên kết

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/5610) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112802.webp)

Một cánh đồng lúa rộng lớn ở phía đông thành phố Qianjiang Century, Hàng Châu, được mệnh danh là "稻田 CBD" (CBD ruộng lúa), vừa bước vào mùa thu hoạch vàng óng. Khu đất nông nghiệp này được chính quyền thành phố bảo tồn nghiêm ngặt nhằm tạo ra sự giao thoa hài hòa giữa không gian đô thị hiện đại và cảnh quan làng quê thanh bình. (Nguồn: [QQ](https://news.qq.com/rain/a/20241114A06IXJ00))

## 没有链接的互联网

Bạn có thể tưởng tượng được một thế giới Internet hoàn toàn không có các liên kết (hyperlinks) bấm chuyển tiếp sẽ như thế nào không?

Không cần phải tưởng tượng xa xôi nữa, bởi thực tế này đang dần hiển hiện ngay trước mắt chúng ta.

Vào năm 2017, Facebook đã ban hành một chính sách thuật toán mới: Bất kỳ bài viết nào chứa liên kết dẫn ra ngoài nền tảng (external links) sẽ lập tức bị hệ thống tự động bóp nghẹt độ tiếp cận và giảm hiển thị (reach).

Điều này đồng nghĩa với việc: **Chỉ cần bạn chèn một liên kết trang web vào bài đăng của mình, những người dùng khác hầu như sẽ không thể nhìn thấy bài viết đó trên bảng tin của họ**. Mục tiêu của chính sách này nhằm ngăn chặn tối đa việc người dùng rời khỏi ứng dụng Facebook, đồng thời hạn chế việc kéo dòng lưu lượng (traffic) miễn phí sang các trang web khác.

Do đó, nếu lướt Facebook hiện nay, bạn sẽ bắt gặp một cách làm vô cùng kỳ lạ của cộng đồng: Mọi người đăng bài chia sẻ tuyệt đối không chèn bất kỳ liên kết trực tiếp nào. Thậm chí nhiều bài viết chỉ đăng tải một bức ảnh chụp dòng chữ mô tả ngắn (hình dưới), còn đường liên kết thực tế sẽ được tác giả khéo léo để dưới phần bình luận được ghim lên đầu.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024111602.webp)

Sau đó, hàng loạt các nền tảng mạng xã hội lớn nhỏ khác cũng nhanh chóng học tập và áp dụng các biện pháp thắt chặt liên kết tương tự.

Tiêu biểu nhất là mạng xã hội X (Twitter cũ), nền tảng liên tục cập nhật các giải pháp kỹ thuật nhằm giữ chân người dùng trong ứng dụng. Đầu tiên là việc ra mắt tính năng chuỗi bài viết (threads), tiếp theo là xóa bỏ hoàn toàn giới hạn ký tự cho phép viết các bài viết dài, nhằm triệt tiêu tối đa động lực chèn link liên kết ngoài của người dùng. Mới đây nhất, khi người dùng chèn link, hệ thống tự động chuyển đổi thành ảnh xem trước nhưng lại [ẩn hoàn toàn tiêu đề trang web](https://www.theverge.com/2023/10/4/23903859/x-elon-musk-headlines-links-image-twitter), khiến người xem khó lòng nhận biết đó là một liên kết có thể click được.

Ngay cả một công cụ tìm kiếm vốn sống nhờ dòng lưu lượng chuyển tiếp như Google cũng đang tìm mọi cách ngăn người dùng rời đi. Khi người dùng tìm kiếm thông tin, Google sẽ ưu tiên hiển thị ngay một đoạn tóm tắt nội dung do AI tự động tổng hợp (hình dưới), giúp giải đáp thắc mắc trực tiếp và giảm thiểu tối đa việc người dùng click vào các liên kết nguồn bên ngoài.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112201.webp)

Tại thị trường Trung Quốc, các siêu ứng dụng như WeChat hay Douyin thậm chí còn áp dụng các biện pháp thắt chặt và cô lập liên kết bên ngoài một cách triệt để và khắt khe hơn nhiều.

Tóm lại, **các tập đoàn Internet lớn đều đang tìm cách bài trừ các liên kết ngoài**. Triết lý vận hành chung của họ là bằng mọi giá phải giữ chân người dùng ở lại bên trong "khu vườn khép kín" (walled garden) của mình và ngăn họ rời đi.

Xu hướng này được dự báo sẽ còn diễn ra mạnh mẽ hơn nữa trong tương lai. Sự bùng nổ của các mô hình AI có khả năng tạo nội dung trực tiếp theo thời gian thực sẽ càng khiến nhu cầu truy cập vào các trang web nguồn bên ngoài của người dùng giảm đi rõ rệt.

**Kỷ nguyên không còn liên kết để click sẽ làm thay đổi hoàn toàn hệ sinh thái Internet**. Tôi có đọc [một bài phân tích](https://www.techspot.com/article/2908-the-zero-click-internet/) chỉ ra 7 hệ quả lớn của xu hướng này, được đúc kết rất sắc sảo:

**(1) Các trang web độc lập sẽ dần biến mất** do không còn nguồn dòng lưu lượng truy cập đổ về. Mọi nhà sáng tạo nội dung bắt buộc phải phụ thuộc và xuất bản nội dung trực tiếp trên các nền tảng lớn, nếu không sản phẩm của họ sẽ hoàn toàn bị chìm vào quên lãng.

**(2) Ngành xuất bản kỹ thuật số truyền thống sẽ đi đến hồi kết** khi quy trình xuất bản độc lập không còn cần thiết, người ta sẽ chọn đăng trực tiếp nội dung lên các siêu nền tảng mạng xã hội.

**(3) Tên miền (Domain) sẽ không còn giá trị giao dịch lớn** do các trang web nhỏ dù có sở hữu tên miền đẹp đến đâu cũng không thể thu hút được lượng người truy cập trực tiếp. Đại đa số các nhà đăng ký tên miền sẽ phải đối mặt với nguy cơ đóng cửa.

**(4) Mảng dịch vụ lưu trữ máy chủ (Hosting) sẽ bị thu hẹp đáng kể** do số lượng website hoạt động suy giảm nghiêm trọng, nhu cầu tự thuê máy chủ để vận hành trang web cá nhân ngày một ít đi.

**(5) Ngành quảng cáo trực tuyến độc lập sẽ bị khai tử**. Toàn bộ hoạt động quảng cáo trên Internet sẽ bị thâu tóm và kiểm soát hoàn toàn bởi các nền tảng lớn, khiến các mạng lưới quảng cáo độc lập (Ad Networks) trở nên vô giá trị. Các trang web nhỏ cũng không còn cơ hội kiếm tiền từ việc đặt quảng cáo trực tuyến.

**(6) Kỹ thuật tối ưu hóa công cụ tìm kiếm (SEO) sẽ trở nên vô nghĩa**. Khi các website nhỏ không còn nhận được dòng lưu lượng, việc cố gắng tối ưu hóa thứ hạng hiển thị trên công cụ tìm kiếm không còn mang lại giá trị thực tiễn.

**(7) Thông tin trên Internet sẽ bị nông cạn hóa**. Do người dùng rất khó để xuất bản và lưu trữ các nội dung phân tích chuyên sâu dài hạn trên các nền tảng mạng xã hội ăn liền, các thông tin trên mạng sẽ chủ yếu là các dạng tin tức ngắn bề nổi, khiến việc tìm kiếm các tài liệu nghiên cứu chuyên sâu chất lượng ngày một trở nên khó khăn.

## [本周软件] 扣子 Project IDE

Nếu bạn chưa biết đến nền tảng [Coze (扣子)](https://www.coze.cn/s/iDyjkPvH/), tôi xin giới thiệu ngắn gọn: Đây là nền tảng phát triển ứng dụng trí tuệ nhân tạo chuyên nghiệp của ByteDance, **hỗ trợ người dùng tự xây dựng các phần mềm ứng dụng dựa trên các mô hình AI khác nhau**.

Nếu bạn đang sở hữu các ý tưởng ứng dụng AI sáng tạo nhưng lại gặp khó khăn vì không biết lập trình phần mềm, Coze chính là giải pháp lý tưởng: Nền tảng cung cấp giao diện kéo thả đồ họa trực quan, lập trình low-code giúp những người không có kinh nghiệm viết mã vẫn có thể dễ dàng tiếp cận và sử dụng.

Mới đây, Coze đã chính thức tung ra bản cập nhật lớn khi giới thiệu giao diện lập trình trực tiếp trên trình duyệt mang tên **Project IDE** (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112706.webp)

Sau khi nhấp vào nút "Tạo mới" và chọn mục "Tạo ứng dụng", người dùng sẽ được đưa vào giao diện thiết kế chuyên nghiệp. Hệ thống cung cấp sẵn rất nhiều thành phần giao diện (UI components) trực quan, cho phép bạn chỉ cần kéo thả là đã có thể tự thiết kế nên giao diện frontend hoàn chỉnh cho ứng dụng (UBuilder), hỗ trợ hiển thị tối ưu trên các thiết bị di động.

Đồng thời, Project IDE cũng đơn giản hóa tối đa quy trình tương tác đọc ghi với cơ sở dữ liệu backend. Có nghĩa là: **Bạn chỉ cần thực hiện các thao tác nhấp chuột trực tiếp trên trình duyệt là đã có thể tự động tạo ra một ứng dụng AI hoàn chỉnh cả frontend lẫn backend**.

Sau khi hoàn tất thiết kế, ứng dụng có thể lập tức được xuất bản chạy trực tiếp trên các nền tảng như Coze, WeChat, Douyin hoặc cung cấp dưới dạng các cổng kết nối API để tích hợp sâu.

Các bạn muốn tự tay phát triển các ứng dụng AI cho riêng mình có thể truy cập trải nghiệm thử công cụ tuyệt vời này tại [liên kết Coze](https://www.coze.cn/s/iDyjkPvH/), hệ thống hoàn toàn miễn phí sử dụng (trong hạn mức tài nguyên cho phép).

Bên cạnh đó, **sự kiện offline "Coze Developer Day" sẽ được tổ chức tại Thượng Hải vào ngày 19 tháng 12 tới**. Đây là cơ hội tuyệt vời để gặp gỡ và đối thoại trực tiếp với đội ngũ kỹ sư AI của ByteDance về các phương pháp phát triển ứng dụng AI hiện đại. Quét mã QR trên poster để đăng ký tham dự trực tiếp hoặc đăng ký theo dõi buổi phát sóng trực tuyến.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112809.webp)

## 科技动态

1、[Kỷ niệm 50 năm phát hiện hóa thạch vượn cổ Lucy](https://theconversation.com/lucy-discovered-50-years-ago-in-ethiopia-stood-just-3-5-feet-tall-but-she-still-towers-over-our-understanding-of-human-origins-227866)

Tròn 50 năm trước (vào năm 1974), các nhà nhân chủng học người Mỹ trong lúc thực hiện khảo sát tại một vùng đất hoang vu thuộc Ethiopia đã phát hiện ra bộ xương hóa thạch Southern Ape có niên đại 3,2 triệu năm tuổi và đặt tên thân thương là "Lucy".

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112516.webp)

Kích thước cơ thể của Lucy tương đối nhỏ bé, chỉ tương đương với một bé gái 4 tuổi ngày nay, nhưng bộ xương của bà đã được khoa học chứng minh là hóa thạch của tổ tiên loài người cổ xưa nhất từng được tìm thấy. Bà thường được cộng đồng gọi với danh xưng tôn kính là "Người bà của nhân loại".

Trước khi phát hiện ra Lucy, giới khoa học luôn tin rằng tổ tiên loài người đã trải qua quá trình tiến hóa để phát triển bộ não lớn trước, rồi mới bắt đầu chuyển đổi sang tư thế đi thẳng. Tuy nhiên, bộ xương của Lucy cho thấy mặc dù bà sở hữu bộ não rất nhỏ nhưng đã hoàn toàn làm chủ tư thế đi thẳng bằng hai chân. Phát hiện này đã đảo ngược giả thuyết cũ, chứng minh loài người đã tiến hóa tư thế đi thẳng trước rồi mới phát triển bộ não sau.

2、[Công nghệ dán màng da cá mập bảo vệ máy bay](https://simpleflying.com/swiss-entire-boeing-777-fleet-aeroshark/)

Trước đây, ngành thể thao từng chứng kiến sự xuất hiện của loại đồ bơi da cá mập (Sharkskin swimsuit) mô phỏng cấu trúc bề mặt da cá mập giúp giảm thiểu đáng kể lực cản của nước, hỗ trợ các vận động viên bứt phá tốc độ bơi vượt trội.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024060510.webp)

Do hiệu quả cải thiện tốc độ của loại đồ bơi này quá lớn làm mất đi tính công bằng của thể thao, Hiệp hội Bơi lội Quốc tế (FINA) đã phải chính thức ban hành lệnh cấm sử dụng trang phục này trong các giải đấu chuyên nghiệp từ năm 2010.

Đến nay, một ý tưởng công nghệ táo bạo đã được đề xuất: Nếu chúng ta ứng dụng cấu trúc da cá mập này để chế tạo ra các tấm màng bảo vệ dán lên toàn bộ vỏ ngoài của máy bay, liệu có giúp giảm thiểu lực cản không khí để tiết kiệm nhiên liệu bay hay không?

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024060511.webp)

Hãng hàng không Swiss International Air Lines đã đi tiên phong thử nghiệm ý tưởng này khi tiến hành dán phủ toàn bộ lớp màng bảo vệ công nghệ da cá mập lên đội bay gồm 12 chiếc Boeing 777 của hãng. Phần vỏ ngoài máy bay có ánh phản quang trong hình chính là khu vực được dán màng bảo vệ AeroShark.

Mới đây, hãng đã chính thức công bố kết quả sau một năm thử nghiệm thực tế với số liệu vô cùng khả quan: Giải pháp đã giúp hãng tiết kiệm được gần 2.200 tấn dầu phản lực trong năm qua.

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024060512.webp)

Cấu trúc của lớp màng AeroShark này không hoàn toàn trơn nhẵn mà được thiết kế các rãnh lõm siêu nhỏ theo các nguyên lý động lực học chất lưu, giúp giảm tối đa lực ma sát giữa vỏ máy bay và các luồng không khí khi di chuyển.

Biết đâu trong tương lai, quy trình bảo trì máy bay cũng sẽ giống như chiếc điện thoại thông minh: Phải dán một lớp kính cường lực/màng bảo vệ trước khi đưa vào sử dụng.

3、[Quy chuẩn định nghĩa thế nào là kết nối băng thông rộng (Broadband)?](https://cloud.tencent.com/developer/article/1678884)

Trong kỷ nguyên số hiện nay, hầu hết mọi người đều sử dụng kết nối mạng băng thông rộng để truy cập Internet. Tuy nhiên, định nghĩa kỹ thuật thế nào mới được coi là băng thông rộng lại có sự thay đổi rất lớn theo thời gian.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112804.webp)

Theo các tài liệu cũ trước đây, các đường truyền đạt tốc độ từ 512kbps trở lên đã được xếp vào nhóm mạng băng thông rộng. Đây là một con số quá thấp so với tiêu chuẩn hiện nay khi tốc độ tải xuống tối đa thực tế chỉ đạt khoảng 64KB/s, tức người dùng sẽ phải mất tới hơn 26 phút chỉ để tải xuống một tệp tin dung lượng 100MB.

Ủy ban Truyền thông Liên bang Mỹ (FCC) trong năm nay đã chính thức nâng cao quy chuẩn kỹ thuật định nghĩa về mạng băng thông rộng: Nâng tốc độ tải xuống (downlink) tối thiểu từ 25Mbps lên mức **100Mbps**, và tốc độ tải lên (uplink) tối thiểu từ 3Mbps lên mức **20Mbps**.

Quy chuẩn mới xác lập tốc độ 100Mbps chính là ngưỡng tối thiểu để một đường truyền được gọi là mạng băng thông rộng, mọi kết nối có tốc độ thấp hơn mức này sẽ không được phép gắn nhãn băng thông rộng nữa.

4、**Các tin tức khác**

(1) Ứng dụng họp trực tuyến Microsoft Teams vừa giới thiệu [tính năng dịch giọng nói thông minh](https://techcrunch.com/2024/11/19/soon-microsoft-will-let-teams-meeting-attendees-clone-their-voices/), cho phép hệ thống tự động học và克隆 giọng nói của người dùng để phát ngôn trực tiếp bằng một ngôn ngữ khác khi giao tiếp với các đối tác nước ngoài.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112511.webp)

(2) Mạng lưới vệ tinh Starlink thông báo dự kiến trong năm tới sẽ chính thức thương mại hóa dịch vụ [kết nối internet vệ tinh trực tiếp tới thiết bị di động](https://www.starlink.com/business/direct-to-cell) (Direct to Cell). Tuy nhiên, dịch vụ yêu cầu thiết bị phải thu phát sóng trực tiếp ngoài trời và không hỗ trợ kết nối khi ở trong nhà kín.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112512.webp)

(3) Nhằm tối ưu hóa tài nguyên nước ngọt, Singapore mới đây đã giới thiệu dòng sản phẩm bia độc đáo được [sản xuất hoàn toàn từ nguồn nước thải sinh hoạt](https://apnews.com/article/beer-wastewater-sewage-recycling-singapore-climate-cop29-5ed7c8e19cd931f0748bddf97a2c542d) đã qua các quy trình lọc siêu sạch đạt chuẩn an toàn y tế.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112515.webp)

## 文章

1、[Hướng dẫn thiết lập thanh trạng thái (status bar) cho iTerm2](https://wompa.land/articles/iterm-status-bar) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024101604.webp)

iTerm2 là một trong những ứng dụng giả lập terminal phổ biến nhất trên macOS. Thiết bị được tích hợp sẵn tính năng hiển thị thanh trạng thái rất hữu dụng, bài viết hướng dẫn chi tiết cách cấu hình tính năng này.

2、[Trải nghiệm ứng dụng máy chiếu làm màn hình làm việc](https://sofiapandelea.medium.com/monitor-replacement-using-a-projector-for-a-home-office-setup-231d2891b3ae) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112506.webp)

Tác giả chia sẻ chi tiết về những trải nghiệm thực tế và các lưu ý kỹ thuật khi quyết định sử dụng máy chiếu (projector) thay thế cho màn hình máy tính truyền thống tại phòng làm việc tại gia.

3、[Những điểm bất cập khi tự thiết lập phòng máy chủ gia đình (HomeLab)](https://www.xda-developers.com/five-reasons-my-homelab-is-a-nightmare/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112601.webp)

Bài chia sẻ thẳng thắn của tác giả về 6 điểm khó khăn và phiền toái nhất khi tự duy trì một hệ thống phòng máy chủ HomeLab tại nhà, trong đó thách thức lớn nhất là chi phí tiền điện hằng tháng cực kỳ tốn kém.

4、[So sánh các giải pháp lưu trữ dữ liệu trên trình duyệt Web](https://rxdb.info/articles/localstorage-indexeddb-cookies-opfs-sqlite-wasm.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024101605.webp)

Bài viết phân tích chuyên sâu và đối chiếu các ưu nhược điểm của các giải pháp lưu trữ dữ liệu phía client hiện nay bao gồm: LocalStorage, IndexedDB, Cookies, hệ thống tệp tin OPFS và giải pháp WASM-SQLite.

5、[Hướng dẫn cấu hình lưu trữ website trực tiếp trên mạng xã hội Bluesky](https://danielmangum.com/posts/this-website-is-hosted-on-bluesky/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112514.webp)

Bluesky là mạng xã hội phi tập trung có giao diện tương tự như Twitter hoạt động trên giao thức AT Protocol mở. Giao thức này cho phép lưu trữ và tải lên các định dạng tệp tin, giúp các nhà phát triển có thể tận dụng hạ tầng Bluesky để lưu trữ và xuất bản một trang web tĩnh hoàn chỉnh.

6、[So sánh hai thư viện kiểm thử Jest và Vitest](https://www.speakeasy.com/post/vitest-vs-jest) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112701.webp)

Bài viết so sánh chi tiết về hiệu năng, cú pháp viết và khả năng tương thích của hai thư viện kiểm thử (testing frameworks) phổ biến nhất hiện nay cho các dự án JS/TS là Jest và Vitest.

## 工具

1、[Graphite](https://graphite.rs/)

Trình biên tập và chỉnh sửa hình ảnh vector trực tuyến chạy trực tiếp trên trình duyệt web, dự án được chia sẻ mã nguồn mở hoàn toàn.

2、[Gimel Studio](https://gimelstudio.github.io/)

Phần mềm thiết kế đồ họa 2D độc đáo với triết lý thiết kế mọi thao tác xử lý hình ảnh dưới dạng các khối nút liên kết (nodes), giúp người dùng dễ dàng kiểm soát các thông số của từng bước xử lý.

3、[Karpor](https://github.com/KusionStack/karpor)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112401.webp)

Công cụ trực quan hóa và giám sát hệ thống Kubernetes mã nguồn mở, tích hợp các công cụ tìm kiếm thông minh, phân tích sâu và hỗ trợ bởi trợ lý AI. (Đóng góp từ [@elliotxx](https://github.com/ruanyf/weekly/issues/5565))

4、[dmMiniPlayer](https://github.com/apades/dmMiniPlayer)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112406.webp)

Tiện ích mở rộng trình duyệt giúp bổ sung thêm các phím tắt điều hướng nhanh thanh tiến trình, điều chỉnh âm lượng trực quan ngay trên cửa sổ xem video dạng ảnh trong ảnh (Picture-in-Picture). (Đóng góp từ [@apades](https://github.com/ruanyf/weekly/issues/5574))

5、[Slide Lab (四象限编辑器)](https://github.com/KwokKwok/slide-lab)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112407.webp)

Công cụ trực tuyến mã nguồn mở hỗ trợ người dùng dễ dàng thiết kế và tạo các biểu đồ phân tích 4 phần (four-quadrant charts) để chèn vào các slide thuyết trình hoặc tài liệu báo cáo. (Đóng góp từ [@KwokKwok](https://github.com/ruanyf/weekly/issues/5578))

6、[Git Stats](https://github.com/lixianmin/git.stats)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112502.webp)

Tiện ích mở rộng dành cho VS Code giúp quản lý dự án trực quan hóa lịch sử commit và tần suất viết mã nguồn của từng kỹ sư trong đội ngũ phát triển. (Đóng góp từ [@lixianmin](https://github.com/ruanyf/weekly/issues/5585))

7、[Bootstrap React Logic](https://github.com/dafengzhen/bootstrap-react-logic)

Bộ thư viện các thành phần giao diện React (React Components) được phát triển dựa trên bộ khung CSS Bootstrap quen thuộc. (Đóng góp từ [@dafengzhen](https://github.com/ruanyf/weekly/issues/5601))

8、[rmtrash](https://github.com/TBXark/rmtrash)

Giải pháp thay thế an toàn cho lệnh xóa tệp `rm` mặc định của hệ điều hành macOS, giúp chuyển các tệp tin cần xóa vào thùng rác hệ thống (Trash) thay vì xóa vĩnh viễn trực tiếp, phòng ngừa các sự cố lỡ tay xóa nhầm. (Đóng góp từ [@TBXark](https://github.com/ruanyf/weekly/issues/5606))

9、[mpv](https://mpv.io/)

Trình phát video dòng lệnh tối giản và đa nền tảng, hỗ trợ chơi hầu hết các định dạng tệp tin đa phương tiện hiện nay với hiệu năng cực nhẹ.

10、[Animate.css](https://animate.style/)

Thư viện CSS hoạt họa kinh điển dành cho lập trình viên web. Bạn chỉ cần gán tên lớp CSS tương ứng cho các phần tử DOM là hệ thống đã tự động kích hoạt các hiệu ứng chuyển động mượt mà.

## AI 相关

1、[Lobe Chat](https://github.com/lobehub/lobe-chat)

Ứng dụng trò chuyện AI mã nguồn mở chất lượng cao, hỗ trợ người dùng dễ dàng tích hợp và trò chuyện với hầu hết các mô hình ngôn ngữ lớn LLM phổ biến hiện nay. (Đóng góp từ [@tcmonster](https://github.com/ruanyf/weekly/issues/5579))

2、[AI Git Commit (JetBrains Plugin)](https://github.com/ruanyf/weekly/issues/5572)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112405.webp)

Tiện ích bổ sung dành cho hệ điều hành lập trình IDE của hãng JetBrains, ứng dụng AI để phân tích sự thay đổi mã nguồn và tự động viết thông điệp commit (commit message) chuẩn xác cho lập trình viên. (Đóng góp từ [@HMYDK](https://github.com/ruanyf/weekly/issues/5572))

3、[UICloner Extension](https://github.com/AndySpider/uicloner-extension)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112503.webp)

Tiện ích mở rộng trình duyệt hỗ trợ lập trình viên sao chép nhanh cấu trúc mã nguồn HTML/CSS của một thành phần giao diện bất kỳ trên một trang web chỉ bằng một cú nhấp chuột. (Đóng góp từ [@AndySpider](https://github.com/ruanyf/weekly/issues/5587))

4、[MagicMirror](https://github.com/idootop/MagicMirror)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112704.webp)

Ứng dụng máy tính mã nguồn mở hỗ trợ người dùng trải nghiệm nhanh các tính năng AI thay đổi khuôn mặt, đổi kiểu tóc và thử nghiệm các bộ trang phục thời trang khác nhau trực quan. (Đóng góp từ [@idootop](https://github.com/ruanyf/weekly/issues/5602))

## 资源

1、[GitHub Insights Pro](https://github-insights-pro.toolsnav.top/)

Nền tảng phân tích và trực quan hóa dữ liệu từ kho chứa GitHub, cung cấp các biểu đồ thống kê chuyên sâu về hoạt động của các dự án và hồ sơ cá nhân của nhà phát triển, đi kèm bảng xếp hạng xu hướng công nghệ. (Đóng góp từ [@wincatcher](https://github.com/ruanyf/weekly/issues/5569))

Một dự án phân tích hồ sơ cá nhân tương tự khác là [GitHub Persona](https://github-persona.pages.dev/). (Đóng góp từ [@Ray-D-Song](https://github.com/ruanyf/weekly/issues/5589))

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112510.webp)

2、[Visual Sorting (Trực quan hóa các thuật toán sắp xếp)](https://mszula.github.io/visual-sorting/)

Trang web mô phỏng trực quan cơ chế hoạt động của các thuật toán sắp xếp dữ liệu kinh điển bằng các chuyển động hình họa sinh động, dự án được chia sẻ mã nguồn mở.

3、[看见概率论 (Trực quan hóa Xác suất thống kê)](https://probability.visualized.fun/)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112703.webp)

Trang web giáo dục toán học bằng tiếng Trung, hỗ trợ người học dễ dàng làm quen với các khái niệm phức tạp của bộ môn Xác suất thống kê thông qua các mô hình mô phỏng tương tác trực quan. (Đóng góp từ [@wincatcher](https://github.com/ruanyf/weekly/issues/5595))

## 图片

1、[Quy mô nhà xưởng của BYD](https://x.com/TaylorOgan/status/1859146242519167249/photo/1)

Bức ảnh vệ tinh đối chiếu trực quan quy mô xây dựng nhà máy sản xuất của BYD tại Trịnh Châu với tổ hợp siêu nhà máy Gigafactory của Tesla tại bang Texas, Mỹ ở cùng một tỷ lệ bản đồ.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112505.webp)

Khu tổ hợp nhà xưởng màu trắng khổng lồ ở phía bên trái là nhà máy BYD Trịnh Châu với chiều rộng trải dài lên tới khoảng 3,2 km.

Phía bên phải là siêu nhà máy Tesla Texas được biểu diễn ở cùng một tỷ lệ bản đồ để người xem dễ hình dung quy mô khổng lồ của BYD.

2、[Thông điệp Arecibo gửi vào không gian vũ trụ](https://en.wikipedia.org/wiki/Arecibo_message)

Vào ngày 16 tháng 11 năm 1974, các nhà khoa học Mỹ đã sử dụng kính viễn vọng vô tuyến khổng lồ Arecibo tại Puerto Rico để phát đi một thông điệp mã hóa nhị phân hướng về phía cụm sao M13 trong không gian.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112402.webp)

Khi thực hiện giải mã chuỗi nhị phân này, người nhận sẽ thu được một bức ảnh sơ đồ dọc ghi nhận nhiều thông tin cơ bản về Trái Đất: hình dáng con người, các nguyên tố hóa học cấu thành chuỗi DNA, sơ đồ hệ Mặt Trời và con số thống kê dân số Trái Đất năm 1974.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112403.webp)

Dự kiến luồng sóng tín hiệu vô tuyến này sẽ phải mất khoảng 25.000 năm di chuyển mới có thể tiếp cận được khu vực cụm sao M13.

## 文摘

1、[Quản lý những khung giờ làm việc hiệu quả nhất hằng ngày](https://ashore.io/journal/crossover-creativity/poisoning-the-day)

Quỹ thời gian một ngày có 24 tiếng, nhưng bộ não của con người hoàn toàn không thể duy trì trạng thái tập trung cao độ liên tục suốt cả ngày.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112702.webp)

Khung giờ làm việc đạt hiệu năng cao nhất (peak productivity) của mỗi người thông thường chỉ kéo dài trong một khoảng thời gian ngắn hằng ngày, và một khi năng lượng đó đã tiêu hao hết thì bộ não rất khó để phục hồi lại trạng thái đó trong ngày.

Do đó, nếu bạn nhận thấy bộ não bắt đầu rơi vào trạng thái mệt mỏi và mất tập trung, lời khuyên là hãy dừng việc cố gắng gượng ép bản thân lại. Hãy chấp nhận thực tế đó và chuyển hướng sang xử lý các đầu việc đơn giản hơn không yêu cầu nhiều tư duy phức tạp.

Tỷ phú Jeff Bezos — nhà sáng lập tập đoàn Amazon — từng chia sẻ: "Tôi luôn ưu tiên sắp xếp các cuộc họp quan trọng nhất vào lúc 10 giờ sáng. Nếu đã sang 5 giờ chiều, bộ não của tôi hầu như không thể đưa ra các quyết định sáng suốt được nữa, và tôi sẽ chủ động dời các cuộc họp quan trọng sang 10 giờ sáng ngày hôm sau."

Vì vậy, giải pháp tối ưu cho công việc hằng ngày của bạn là: **Hãy tập trung giải quyết các đầu việc khó khăn và quan trọng nhất càng sớm càng tốt ngay khi bắt đầu ngày mới**. Trong khung giờ vàng này, hãy chủ động ngắt mọi kết nối gây xao nhãng xung quanh để xử lý các tác vụ phức tạp nhất cho đến khi cảm thấy bộ não bắt đầu mỏi mệt.

Khi cơ thể đã phát đi tín hiệu mỏi mệt và mất tập trung, đừng cố gắng chống lại nó. Hãy chủ động dời các công việc chưa hoàn thành sang ngày hôm sau và chuyển sang dọn dẹp hòm thư điện tử, xử lý các tác vụ giấy tờ đơn giản, hoặc tốt nhất là đóng máy nghỉ ngơi hoàn toàn.

Nhiều lập trình viên lựa chọn giải pháp thức dậy thật sớm để làm việc yên tĩnh. Một số khác lại chọn làm việc tập trung cao độ trong khung giờ đêm muộn từ 11 giờ đêm đến 4 giờ sáng ngày hôm sau.

Tất cả họ đều đang chủ động né tránh những khung giờ hành chính ban ngày — khoảng thời gian thời tiết nóng nực, mọi người xung quanh liên tục nhắn tin trao đổi công việc tạo ra vô số các kích thích gây xao nhãng. Dù năng lực tập trung của bạn có tốt đến đâu, bạn cũng rất khó lòng bảo vệ bộ não của mình khỏi các kích thích xao nhãng này trong giờ hành chính.

Hãy luôn ghi nhớ: Mỗi sáng thức dậy, quỹ thời gian vàng của bạn đang liên tục trôi đi và bạn không thể biết chắc năng lượng tập trung của mình sẽ kéo dài được bao lâu. Câu hỏi quan trọng nhất bạn cần trả lời mỗi sáng là: Bạn có thể hoàn thành bao nhiêu việc khó trước khi năng lượng tập trung bị cạn kiệt hoàn toàn?

## 言论

1、

Vài năm trước khi Elon Musk công bố dự án tàu vũ trụ Starship đưa con người lên thám hiểm Sao Hỏa, tôi từng đưa ra một lời bông đùa rằng: Có khi tàu Starship đã đưa con người đặt chân lên Sao Hỏa thành công rồi mà dự án đường sắt cao tốc nối từ London đến Manchester của nước Anh vẫn chưa thể hoàn thành.

Không ngờ lời đùa đó nay đã trở thành sự thật phũ phàng khi Thủ tướng Anh mới đây đã chính thức công bố hủy bỏ toàn bộ dự án đường sắt cao tốc kết nối Manchester do chậm tiến độ và đội vốn.

-- [Peter Hague](https://x.com/peterrhague/status/1764746632011149655), nhà thiên văn học người Anh

2、

Khi phát hành phiên bản hệ điều hành Linux chuyên dụng cho doanh nghiệp vào năm 2019, hãng SUSE đã cam kết sẽ duy trì các dịch vụ hỗ trợ kỹ thuật liên tục cho phiên bản này cho đến tận năm 2038.

Tại sao thời gian hỗ trợ lại được ấn định là 19 năm mà không phải là các con số tròn chục như 18 hay 20 năm? Nguyên nhân nằm ở sự cố kỹ thuật năm 2038: Các hệ điều hành 32-bit sử dụng hệ mốc thời gian Unix (bắt đầu từ ngày 1/1/1970) sẽ bị tràn số bộ đếm thời gian vào năm 2038 gây sập hệ thống. Do đó, SUSE quyết định hỗ trợ kỹ thuật đến đúng mốc năm 2038, còn các sự cố tràn số sau đó họ sẽ không chịu trách nhiệm xử lý nữa.

-- [《Tại sao SUSE lại cấu hình chu kỳ hỗ trợ kéo dài đúng 19 năm》](https://www.zdnet.com/article/suse-upgrades-its-distros-with-19-years-of-support-no-other-linux-comes-close/)

3、

Tại sao ngôn từ sử dụng trong văn bản luật pháp lại luôn vô cùng khó hiểu đối với đại bộ phận công chúng? Một số học giả đưa ra giải thích rằng hiện tượng này tương tự như các câu thần chú cổ xưa: Ngôn từ thần chú luôn khác biệt hoàn toàn với ngôn ngữ giao tiếp hằng ngày nhằm tạo ra cảm giác huyền bí và thể hiện một uy quyền đặc biệt trước người nghe.

-- [《Tại sao ngôn từ luật pháp lại được viết theo phong cách khó hiểu như vậy?》](https://phys.org/news/2024-08-laws-written-incomprehensible-style.html)

4、

Tôi cực kỳ không thích việc xem các chương trình hòa nhạc giao hưởng phát sóng trên truyền hình. Về bản chất, trải nghiệm hòa nhạc giao hưởng là một trải nghiệm nghệ thuật âm thanh (thính giác). Tuy nhiên, máy quay truyền hình đã biến đổi nó thành một trải nghiệm thị giác khi hướng sự tập trung của khán giả vào các hình ảnh nhạc công biểu diễn trên màn hình.

Việc này làm giảm đi giá trị cốt lõi của âm nhạc, bởi âm nhạc sinh ra là để lắng nghe chứ không phải để quan sát bằng mắt.

-- [《Sự vô nghĩa của các chương trình hòa nhạc giao hưởng trên truyền hình》](https://www.theparisreview.org/blog/2024/05/20/televised-music-is-a-pointless-rigmarole/)

5、

Dãy số Fibonacci sở hữu một tính chất toán học vô cùng thú vị: Tỷ lệ giữa hai số liên tiếp trong dãy (ví dụ như: 5 và 8, hay 21 và 34) phản ánh khá chính xác tỷ lệ chuyển đổi khoảng cách giữa đơn vị Dặm (Miles) và Kilômét (Kilometers). Ví dụ: 5 dặm sẽ xấp xỉ bằng 8 km.

-- [《Ứng dụng dãy số Fibonacci để quy đổi nhanh đơn vị dặm và kilômét》](https://catonmat.net/fibonacci-miles-kilometers)

## 往年回顾

[Bàn về văn hóa gọi món tự động qua máy và lối sống hướng nội đô thị](https://www.ruanyifeng.com/blog/2023/12/weekly-issue-280.html) (2023 #280)

[Thống kê điện năng tiêu thụ thực tế của các thiết bị điện tử gia đình](https://www.ruanyifeng.com/blog/2022/11/weekly-issue-230.html) (2022 #230)

[Khảo sát: Đâu là thành phố đáng sống nhất tại Trung Quốc đối với bạn?](https://www.ruanyifeng.com/blog/2021/10/weekly-issue-180.html) (2021 #180)

[Mối lo ngại về xu hướng trẻ hóa độ tuổi người dùng trên mạng Internet](https://www.ruanyifeng.com/blog/2020/10/weekly-issue-130.html) (2020 #130)

(Hết)
