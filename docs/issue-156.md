# 科技爱好者周刊（第 156 期）：显卡缺货与异业竞争

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1652) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042313.jpg)

Bước sang tháng 4, số ca nhiễm COVID-19 tại Ấn Độ tăng vọt khiến nguồn dự trữ oxy y tế toàn quốc nhanh chóng rơi vào tình trạng cạn kiệt. Chính phủ đã phải huy động tối đa các xe bồn chở oxy lỏng đến các khu vực trọng điểm. Tại một số vùng không có hệ thống quốc lộ chất lượng cao, các xe bồn này buộc phải xếp lên các toa tàu hỏa để vận chuyển bằng đường sắt. (Nguồn: [Scroll.in](https://scroll.in/article/992928/how-grave-is-indias-oxygen-emergency-worse-than-the-government-admits))

## 主带话题：Cơn sốt khan hiếm card đồ họa và cạnh tranh chéo ngành

Gần đây, tôi định lắp thêm một chiếc máy tính để bàn mới, nhưng phát hiện ra rằng mình hoàn toàn không thể mua được card đồ họa (GPU). Cơn sốt tăng giá điên cuồng của tiền mã hóa đã khiến card đồ họa bị các thợ đào gom sạch không còn một vết tích.

Người ta tính toán rằng việc mua card đồ họa gia dụng về để đào coin chỉ mất khoảng 6 tháng là có thể hòa vốn, toàn bộ thời gian sau đó đều là lợi nhuận ròng. Nếu ghép nhiều card đồ họa lại thành các dàn trâu cày lớn, lợi nhuận thu về là vô cùng đáng kể. Do đó, toàn bộ card đồ họa mới ra mắt trên thị trường đều bị gom sạch, người dùng thông thường muốn mua chỉ có nước tìm mua hàng cũ đã qua sử dụng với mức giá cắt cổ.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042808.jpg)

May mắn thay, năm ngoái tôi đã kịp mua một chiếc card đồ họa để dùng tạm. Nhìn vào thị trường chuyển nhượng card cũ hiện nay, tôi không khỏi cảm thán và đăng một dòng tweet:

> *"Năm ngoái tôi mua một chiếc card đồ họa giá 2.000 NDT, sau một năm sử dụng mang bán lại vẫn thu về được 5.000 NDT."*

Một cư dân mạng bình luận bên dưới rằng anh ta mua chiếc card cũ một năm trước với giá 400 NDT, năm nay bán đi thu về tới 2.000 NDT. Sự khan hiếm đã đạt đến mức độ phi lý như vậy.

Tôi tự hỏi: Các thợ đào coin thì hồ hởi, nhưng thị trường linh kiện tự lắp ráp (DIY PC) thì lại chịu đòn nặng nề. Nếu bạn chỉ là một người yêu thích máy tính thông thường, hoàn toàn không quan tâm đến Bitcoin hay đào coin, bỗng nhiên một ngày bạn bị ảnh hưởng trực tiếp một cách vô lý. Dự định tự lắp ráp một chiếc PC cấu hình mơ ước để chơi game hay làm việc với dữ liệu lớn bỗng chốc tan thành mây khói, quả thực là tai bay vạ gió.

**Một sự việc diễn ra ở một lĩnh vực hoàn toàn xa lạ, bỗng nhiên lại giáng một đòn chí mạng lên cuộc sống và công việc của bạn. Trong kinh tế học, hiện tượng này được gọi là "cạnh tranh chéo ngành" (cross-industry competition).** Sự thay đổi của một ngành nghề tạo ra hiệu ứng tràn (spillover effect) ảnh hưởng sang một ngành nghề hoàn toàn khác. Những sự việc như vậy dường như đang xuất hiện ngày một nhiều trong thế giới hiện đại.

Tôi có thể lấy một vài ví dụ điển hình. Sự ra đời của điện thoại thông minh đã giáng đòn nặng nề lên các nhà mạng viễn thông, khi mọi người chuyển sang nhắn tin gọi điện qua các ứng dụng OTT miễn phí, khiến doanh thu từ cuộc gọi và tin nhắn SMS truyền thống sụt giảm không phanh. Hay như sự bùng nổ của các ứng dụng giao đồ ăn nhanh (food delivery) đã gián tiếp bóp nghẹt doanh số bán hàng của các hãng mì ăn liền.

Tuần này tôi còn đọc được tin tức: Chủ tịch hội đồng quản trị của Sân bay Thượng Hải chia sẻ rằng chính sách miễn thuế tại đảo Hải Nam đang gây ảnh hưởng vô cùng lớn đến doanh thu của sân bay. Trước đây, khi nghĩ đến việc mua đồ hiệu miễn thuế, người ta lập tức nghĩ đến việc ra sân bay đi nước ngoài. Nhưng hiện nay người dân không cần xuất cảnh vẫn có thể thỏa sức mua đồ miễn thuế tại đảo Hải Nam, và sắp tới các cửa hàng miễn thuế nội đô cũng sẽ được mở ngay tại Bắc Kinh, Thượng Hải. Điều này trực tiếp làm sụt giảm nguồn thu thương mại cực lớn của các sân bay lớn.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042809.jpg)

**Tóm lại, thế giới ngày nay liên kết chặt chẽ với nhau ở mức độ chưa từng có, và các cuộc cạnh tranh chéo ngành diễn ra nhiều hơn và nhanh hơn rất nhiều.** Không chỉ những thay đổi trong học thuật hay trong nội bộ ngành của bạn mới ảnh hưởng đến bạn, mà một sự kiện diễn ra ở một góc khuất nào đó trên thế giới cũng có thể từ trên trời rơi xuống và làm đảo lộn công việc của bạn.

Đó chính là đặc trưng của kỷ nguyên Internet: cuộc sống của mỗi người trở nên đầy biến động và dễ bị ảnh hưởng bởi những phương thức không thể lường trước. Có những tác động tích cực và cả tiêu cực, và hầu như không có cách nào để chuẩn bị hay phòng ngừa trước. Điều duy nhất chúng ta có thể làm là không ngừng học hỏi để nâng cấp bản thân và chủ động thích ứng với mọi sự thay đổi.

## Khóa học phân tích nguyên lý Vue 3 nâng cao

Tuần này, chúng tôi giới thiệu chương trình đào tạo chuyên sâu về Front-end, dành riêng cho các lập trình viên muốn nâng cao trình độ phát triển với framework Vue.js.

Như các bạn đã biết, Vue.js là một trong những thư viện Front-end phổ biến nhất tại thị trường trong nước. Sau khi phiên bản 3.0 ra mắt với nhiều cải tiến cốt lõi, hệ sinh thái xung quanh cũng đang dần được hoàn thiện nhanh chóng. Việc làm chủ Vue 3 đã trở thành yêu cầu phỏng vấn bắt buộc tại các doanh nghiệp công nghệ lớn.

Tuy nhiên, các câu hỏi phỏng vấn hiện nay không chỉ dừng lại ở cách sử dụng API cơ bản mà đi sâu vào các bài toán nguyên lý thiết kế hệ thống phản ứng (reactivity system), tối ưu hóa Virtual DOM và thuật toán so khớp Diff. Để ghi điểm tốt nhất, lập trình viên cần hiểu rõ tư duy thiết kế bên dưới của tác giả.

Khóa học **《Vue 3 Principle Analysis》** do giảng viên **Thôi Hiệu Thụy** (nhà đóng góp mã nguồn - code contributor cho dự án Vue 3) trực tiếp giảng dạy sẽ hướng dẫn bạn tháo gỡ các khó khăn này:

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042901.jpg)

Nội dung khóa học sẽ dẫn dắt học viên tự tay viết một phiên bản Vue 3 tối giản (mini version) để thấu hiểu bản chất hoạt động của hệ thống proxy phản ứng, giúp hình thành tư duy phân tích hệ thống chuyên nghiệp.

Khóa học sẽ phát sóng trực tiếp vào **19:50 tối thứ Sáu (ngày 30 tháng 4)**. Đây là tài liệu học tập vô cùng thích hợp để bạn tận dụng kỳ nghỉ lễ sắp tới để nâng cấp kỹ năng lập trình cá nhân.

Độc giả đăng ký tham gia khóa học qua mã QR dưới đây sẽ được nhận **miễn phí** bộ tài liệu bổ trợ chuyên đề nâng cao về ngôn ngữ ES6 và lập trình hướng đối tượng:

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042902.jpg)

Học viên hoàn thành khóa học cũng sẽ nhận được cẩm nang phỏng vấn Vue 3 nâng cao từ ban tổ chức.

## 科技动态

1、[Xe tự hành Perseverance thực hiện thành công thí nghiệm chiết xuất oxy trên Sao Hỏa](https://new.qq.com/rain/a/20210422A02OXP00)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042304.jpg)

NASA công bố thiết bị thí nghiệm MOXIE gắn trên xe tự hành Perseverance đã thực hiện thành công việc sản xuất oxy trực tiếp từ bầu khí quyển Sao Hỏa. Thiết bị đã chiết xuất được 10 gram oxy tinh khiết trong vòng một giờ hoạt động, đủ lượng dưỡng khí cho một phi hành gia hô hấp trong 10 phút.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042305.jpg)

Thành tựu này đặt nền móng quan trọng cho các kế hoạch đổ bộ và xây dựng căn cứ có người ở trên Sao Hỏa trong tương lai. Oxy không chỉ phục vụ hô hấp mà còn đóng vai trò là chất oxy hóa thiết yếu cho động cơ tên lửa đẩy chiều về. Việc phóng một tàu vũ trụ chở 4 phi hành gia rời Sao Hỏa quay lại Trái Đất ước tính cần khoảng 7 tấn nhiên liệu và tới 25 tấn oxy. Thiết bị MOXIE hoạt động bằng cách sử dụng năng lượng mặt trời để điện phân luồng khí CO2 (chiếm 95% khí quyển Hỏa Tinh) thành khí oxy (O2) và carbon monoxide (CO).

2、[Sự chênh lệch giá thành sản xuất điện thoại lắp ráp tại Mỹ và Trung Quốc](https://puri.sm/posts/librem-5-and-librem-5-usa-what-are-the-differences/)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041711.jpg)

Purism - một doanh nghiệp Mỹ chuyên phát triển các thiết bị phần cứng chạy hệ điều hành mã nguồn mở Linux, vừa công bố thông tin so sánh giá bán của hai dòng điện thoại mới: Librem 5 và Librem 5 USA. Hai phiên bản này sở hữu cấu hình phần cứng và tính năng bảo mật giống hệt nhau.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041712.jpg)

Điểm khác biệt duy nhất nằm ở chuỗi cung ứng sản xuất: Phiên bản Librem 5 thông thường có các linh kiện chính được sản xuất gia công tại Trung Quốc và lắp ráp hoàn thiện, trong khi phiên bản Librem 5 USA có toàn bộ linh kiện và quá trình sản xuất bo mạch được thực hiện native tại các nhà máy ở Mỹ.

Mức giá chênh lệch cụ thể như sau:
- Phiên bản Librem 5 (gia công Trung Quốc): **799 USD**
- Phiên bản Librem 5 USA (sản xuất tại Mỹ): **1.999 USD**

3、[Thư viện nghệ thuật độc đáo "Cloud Loop Library" khánh thành tại Hải Khẩu](https://mp.weixin.qq.com/s/Gu0xMcm6pNhc7ma56h8gHg?)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041715.jpg)

Công trình thư viện nghệ thuật độc đáo "Cloud Loop Library" (Thư viện Vân Động) do văn phòng kiến trúc MAD thiết kế đã chính thức mở cửa đón khách tại thành phố Hải Khẩu, Hải Nam. Đây là công trình đầu tiên được hoàn thành trong chuỗi dự án 16 trạm dừng chân nghệ thuật ven biển của thành phố. Tòa nhà bê tông đúc nguyên khối màu trắng này từng được tạp chí *The Times* bình chọn là một trong những công trình kiến trúc đáng mong đợi nhất năm 2021.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041814.jpg)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041815.jpg)

Cấu trúc phía Nam của công trình được bố trí làm phòng đọc sách hướng biển, trong khi phía Bắc là khu vực dịch vụ công cộng gồm quán cà phê, phòng nghỉ chân cho người đi bộ. Cầu nối kiến trúc uốn lượn được đúc bê tông tích hợp từ mô hình thiết kế số hóa 3D.

Hệ thống các hốc tròn rỗng có kích thước lớn nhỏ khác nhau xuyên qua thân nhà giúp đón nhận tối đa ánh sáng mặt trời tự nhiên và tạo các luồng thông gió đối lưu tự nhiên mát mẻ từ biển thổi vào.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041816.jpg)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041817.jpg)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041818.jpg)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041819.jpg)

4、**Tin tức một câu**

> - Sau hành trình bay liên tục kéo dài 15 năm kể từ khi phóng, tàu vũ trụ thăm dò New Horizons đã chính thức vượt qua mốc khoảng cách 50 đơn vị thiên văn (AU) cách Mặt Trời, trở thành thiết bị nhân tạo thứ 5 đi vào vành đai Kuiper ngoài rìa Hệ Mặt Trời.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041701.jpg)

> - Quốc hội Anh thông qua đạo luật hiến tạng mới, tự động coi mọi công dân trưởng thành đã qua đời mặc định đồng ý hiến tạng trừ phi cá nhân đã thực hiện ký văn bản đăng ký từ chối hiến tạng trước đó.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042405.jpg)

> - Bộ Quốc phòng Mỹ chính thức lựa chọn ba nhà thầu quốc phòng để bắt đầu thiết kế hệ thống động cơ đẩy sử dụng năng lượng hạt nhân nhằm trang bị cho các tàu tuần tra cơ động ngoài không gian.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041417.jpg)

> - Cảnh sát giao thông thành phố Ôn Châu phát hiện các xe tuần tra liên tục bị các đoàn xe chở quá tải né tránh lịch trình kiểm soát một cách chính xác do gầm xe tuần tra đã bị các đối tượng lén gắn thiết bị định vị GPS nam châm nhỏ gọn bằng bao thuốc lá để theo dõi từ xa.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041112.jpg)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041113.jpg)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041114.jpg)

> - Startup công nghệ Qonos ra mắt sản phẩm khung tranh kỹ thuật số treo tường thông minh, tự động tải và hiển thị bộ sưu tập các bức họa nổi tiếng thế giới lên màn hình độ phân giải cao theo lịch trình cài đặt sẵn của người dùng.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032601.jpg)

> - Meta (Facebook) công bố dự án phát triển vòng đeo tay thông minh thu nhận sóng điện cơ từ các sợi cơ cổ tay để chuyển dịch trực tiếp thành các lệnh cử chỉ điều khiển ngón tay trong không gian thực tế ảo VR/AR mà không cần cầm tay cầm vật lý.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021032101.jpg)

## 文章

1、[Tại sao lập trình logic một cánh cửa trong game 3D lại cực kỳ khó?](https://www.yystv.cn/p/7800)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041418.jpg)

Nhiều nhà phát triển game chia sẻ việc lập trình một cánh cửa tương tác cơ học trong không gian 3D là tác vụ phát sinh nhiều bug nhất trong dự án. Cửa không chỉ có đóng và mở, mà còn phải xử lý tương tác vật lý khi nhân vật đâm vào, cơ chế khóa mở bằng chìa, hoạt ảnh lắc lư tự nhiên và xử lý AI định tuyến của NPC khi đi qua cửa.

2、[Vạch kẻ đường đi bộ hình chữ Z giúp phòng ngừa tai nạn giao thông](https://mp.weixin.qq.com/s/xZN419WSw3zrCYjyqw2S0g)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041413.jpg)

Nhiều đô thị tại Trung Quốc đưa vào thử nghiệm vạch kẻ đường đi bộ hình chữ Z. Thiết kế này bắt buộc người đi bộ khi sang đường phải di chuyển theo lối đi gấp khúc chữ Z hướng mặt về phía dòng xe đang chạy tới để tăng khả năng quan sát tránh xe, tuy nhiên tính thực tế của giải pháp này vẫn đang gây tranh cãi.

3、[Mô hình tàu điện ray trên cao cỡ nhỏ "Cloud Bus" có tiềm năng phát triển?](https://finance.sina.com.cn/tech/2021-04-16/doc-ikmxzfmk7228054.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041820.jpg)

Tuyến tàu điện một ray chạy trên cao tự hành "Cloud Bus" (Vân Ba) đầu tiên do hãng xe điện BYD phát triển đã chính thức đi vào hoạt động tại Trùng Khánh. Bài viết phân tích các ưu điểm về chi phí giải phóng mặt bằng thấp của tuyến metro mini này.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041821.jpg)

4、[Phân tích mối tương quan giữa độ phân giải, bitrate và khung hình video](https://support.shangzhibo.tv/hc/kb/article/1028655/)（Tiếng Trung）

Bài viết hướng dẫn cơ bản cho người làm kỹ thuật truyền hình giải thích chi tiết cách thiết lập các thông số bitrate (tốc độ dữ liệu), resolution (độ phân giải) và fps (tốc độ khung hình) phù hợp để tối ưu hóa dung lượng lưu trữ nhưng vẫn giữ được độ sắc nét cho video.

5、[Bí ẩn phép toán chia biến mất trong mã assembly](https://cjting.me/the-missing-div-instruction-part1/)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042612.jpg)

Khi viết chương trình bằng ngôn ngữ C, tác giả phát hiện ra một hiện tượng thú vị: Phép toán chia `/` khi được trình biên dịch chuyển dịch sang mã assembly không hề sử dụng lệnh chia máy `div` mà được thay thế bằng chuỗi lệnh nhân `mul` kết hợp dịch bit. Bài viết giải thích nguyên lý toán học đằng sau kỹ thuật tối ưu hóa hiệu năng này. ([@cj1128](https://github.com/ruanyf/weekly/issues/1738) đóng góp)

6、[So sánh hiệu năng các dòng cơ sở dữ liệu Serverless Cloud](https://news-app-two-omega.vercel.app/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041412.jpg)

Bài viết tiến hành đo đạc hiệu năng thực tế (độ trễ đọc ghi, thông lượng) của ba nhà cung cấp dịch vụ cơ sở dữ liệu serverless phổ biến hiện nay bao gồm AWS DynamoDB, FaunaDB và Upstash để giúp lập trình viên lựa chọn.

7、[Hướng dẫn sử dụng các tính năng GitHub Actions trực tiếp trên dòng lệnh](https://github.blog/2021-04-15-work-with-github-actions-in-your-terminal-with-github-cli/)（Tiếng Anh）

Trang blog của GitHub giới thiệu các tính năng cập nhật của công cụ dòng lệnh GitHub CLI (lệnh `gh`), hỗ trợ lập trình viên theo dõi tiến độ chạy, xem log chi tiết và quản lý các workflow chạy tự động của dự án trực tiếp trên terminal.

8、[Hướng dẫn thiết kế website giao diện Windows 95 retro cổ điển](https://ash.ms/2019-10-02/retro-website-launch/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041808.jpg)

Tác giả chia sẻ chi tiết các bước sử dụng mã CSS và HTML để tái dựng lại toàn bộ giao diện màn hình desktop, các nút bấm menu Start và khung cửa sổ làm việc đặc trưng của hệ điều hành Windows 95 huyền thoại cho trang blog cá nhân của mình.

9、[Hướng dẫn tự viết hệ thống gọi hàm từ xa RPC bằng ngôn ngữ C](https://alexanderell.is/posts/rpc-from-scratch/)（Tiếng Anh）

Remote Procedure Call (RPC) là giao thức nền tảng trong giao tiếp mạng giữa các máy chủ. Bài viết hướng dẫn chi tiết cách thiết lập kết nối socket TCP, đóng gói tuần tự hóa dữ liệu và thực thi gọi hàm từ xa thông qua code mẫu C tối giản.

## 工具

1、[MetricsGraphics.js](https://github.com/metricsgraphics/metrics-graphics)

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021031802.jpg)

Thư viện biểu đồ viết trên nền tảng D3 chuyên dụng để hiển thị trực quan hóa các chuỗi dữ liệu thời gian (time-series), sở hữu thiết kế API gọn nhẹ và hiển thị giao diện tinh tế.

2、[ClearURLs](https://github.com/ClearURLs/Addon)

Extension trình duyệt web mạnh mẽ tự động rà soát và loại bỏ toàn bộ các chuỗi tham số theo dõi thông tin người dùng (như các tham số `utm_`) đằng sau các đường link liên kết URL trước khi truy cập.

3、[regexploit](https://github.com/doyensec/regexploit)

Tiện ích bảo mật mã nguồn hỗ trợ quét và phát hiện các biểu thức chính quy (regular expressions) có cấu trúc bị lỗi thiết kế dễ dẫn tới nguy cơ treo máy chủ do đòn tấn công từ chối dịch vụ ReDoS.

4、[NPlayer](https://nplayer.js.org/)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042511.jpg)

Một trình phát video HTML5 (media player) viết bằng JavaScript hỗ trợ đầy đủ các tính năng nâng cao, đặc biệt tích hợp sẵn module hiển thị luồng bình luận chạy ngang màn hình (danmaku) thường dùng ở các trang video. ([@woopen](https://github.com/ruanyf/weekly/issues/1734) đóng góp)

5、[JS image carver](https://trekhleb.dev/js-image-carver/)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041704.jpg)

Công cụ trực tuyến ứng dụng thuật toán Seam Carving (cắt nối đường may), cho phép người dùng thay đổi kích thước ngang dọc của hình ảnh một cách thông minh bằng cách tự phát hiện và loại bỏ các dải pixel rác ít thông tin mà không làm biến dạng tỷ lệ của các vật thể chính trong ảnh.

6、[LuckDraw](https://100px.net/)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042506.jpg)

Bộ linh kiện UI抽奖 (vòng quay may mắn, ô số trúng thưởng) đa nền tảng viết bằng JavaScript, tương thích tốt với các framework phổ biến (React, Vue) và các nền tảng mini program. ([@buuing](https://github.com/ruanyf/weekly/issues/1724) đóng góp)

7、[GoGoCode](https://github.com/thx/gogocode)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042509.jpg)

Công cụ xử lý cây cú pháp trừu tượng AST (Abstract Syntax Tree) của JavaScript với cú pháp đơn giản, giúp lập trình viên dễ dàng viết các script tự động nâng cấp mã nguồn hoặc refactor code quy mô lớn. ([@kuangyanit](https://github.com/ruanyf/weekly/issues/1730) đóng góp)

8、[Storyteller](https://storyteller.webzard.io/)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042508.jpg)

Công cụ trực tuyến hỗ trợ thiết kế các bài viết hướng dẫn sử dụng phần mềm dạng tương tác trực quan (interactive tutorial) từng bước một cách sinh động mà không cần viết code. ([@netweng](https://github.com/ruanyf/weekly/issues/1728) đóng góp)

9、[Varlet](https://github.com/haoziqaq/varlet)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042507.jpg)

Bộ thư viện thành phần giao diện di động (mobile UI component library) dành cho Vue 3 được thiết kế đồng bộ theo ngôn ngữ thiết kế Material Design của Google. ([@BeADre](https://github.com/ruanyf/weekly/issues/1727) đóng góp)

10、[chore-cli](https://github.com/iwfan/chore-cli)

Tiện ích dòng lệnh CLI hỗ trợ các nhà phát triển khởi tạo cấu trúc khung xương (scaffold) chuẩn hóa cho các dự án lập trình sử dụng TypeScript. ([@iwfan](https://github.com/ruanyf/weekly/issues/1737) đóng góp)

## Tài nguyên

1][lofi.cafe: Kênh phát nhạc lofi thư giãn khi làm việc](https://lofi.cafe/)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041416.jpg)

Một website phát nhạc lofi trực tuyến với giao diện thiết kế theo phong cách hoài cổ rất đẹp mắt, cung cấp các dải nhạc nền nhẹ nhàng giúp tăng độ tập trung cho người làm việc trí óc.

2、[Become an iOS Developer: Lộ trình học lập trình iOS toàn diện](https://matteomanferdini.com/become-an-ios-developer/)

Bài phân tích chi tiết giới thiệu lộ trình học tập, tài liệu tham khảo và giải đáp các thắc mắc cốt lõi (như nên học Swift hay Objective-C) dành cho những ai muốn bắt đầu tự học phát triển ứng dụng hệ điều hành iOS.

3、[Yamauchi Family Office: Trang web văn phòng gia đình cố chủ tịch Nintendo](https://y-n10.com/)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041415.jpg)

Trang web giới thiệu văn phòng quỹ gia đình của cố chủ tịch Nintendo Yamauchi Hiroshi sở hữu giao diện thiết kế đồ họa dạng game 8-bit tương tác vô cùng sáng tạo và ấn tượng, mang đậm chất di sản trò chơi của Nintendo.

4、[free-python-books: Repo tổng hợp sách học Python miễn phí](https://github.com/pamoroso/free-python-books)

Kho lưu trữ GitHub tổng hợp liên kết tải về hàng chục đầu sách hướng dẫn học lập trình Python chất lượng (bằng tiếng Anh) được chia sẻ miễn phí trực tuyến.

5、[HelloZooKeeper: Giáo trình nhập môn Apache ZooKeeper](https://github.com/HelloGitHub-Team/HelloZooKeeper)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042510.jpg)

Cuốn tài liệu tiếng Trung hướng dẫn chi tiết từ cài đặt, sử dụng API cơ bản đến tìm hiểu cơ chế đồng thuận phân tán bên dưới của Apache ZooKeeper bằng văn phong hình họa sinh động, hài hước. ([@521xueweihan](https://github.com/ruanyf/weekly/issues/1733) đóng góp)

## 图片

1、[Cơn sốt thú cưng bằng đá "Pet Rock" năm 1975](https://en.wikipedia.org/wiki/Pet_Rock)

Vào năm 1975, Gary Dahl khi nghe bạn bè phàn nàn về việc nuôi chó mèo gặp nhiều phiền phức (phải dọn dẹp, cho ăn, tắm rửa) đã nảy ra ý tưởng điên rồ: Bán những viên đá cuội mịn lấy từ bãi biển Mexico làm "thú cưng" không bao giờ ốm chết.

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041411.jpg)

Ông đã thiết kế bao bì hộp carton có lỗ thông khí lót rơm giống như hộp vận chuyển thú cưng thật và viết một cuốn sách hướng dẫn huấn luyện đá cuội cách "nằm yên" hay "giả chết". Mỗi viên đá có giá vốn chỉ 1 xu được bán ra với giá 4 USD. Cơn sốt bùng nổ dịp Giáng sinh năm đó đã giúp ông bán ra hơn 1 triệu sản phẩm và trở thành triệu phú chỉ sau một mùa kinh doanh.

2、[Mô hình cơ học ba trục Tourbillon chế tạo bằng máy in 3D](https://www.myminifactory.com/crowdfunding/tourbillon-mechanica-tri-axial-crowdfunding-250)

Bộ thoát Tourbillon ba trục (Tri-axial Tourbillon) là cơ cấu cơ học tinh vi và đắt đỏ bậc nhất trong đồng hồ cơ khí nhằm triệt tiêu tác động của trọng lực lên độ chính xác của giờ.

Một nhà thiết kế đã sử dụng máy in 3D gia đình rẻ tiền để in và lắp ráp thành công một mô hình cơ cấu Tourbillon ba trục hoạt động hoàn hảo bằng nhựa dẻo:

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041501.jpg)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041502.jpg)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041503.jpg)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041504.jpg)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021041505.gif)

## Bài đọc thêm

### Kim tự tháp Maslow áp dụng cho đánh giá chất lượng mã nguồn

*Tương tự như mô hình phân cấp nhu cầu nổi tiếng của Maslow, chất lượng mã nguồn phần mềm cũng có thể được phân chia thành 5 mức độ từ cơ bản đến nâng cao:*

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021042807.jpg)

![](https://cdn.beekka.com/blogimg/asset/202104/bg2021040705.jpg)

**Mức 1: Đúng đắn (Correct)**
Yêu cầu cơ bản nhất: Mã nguồn phải thực thi đúng logic nghiệp vụ được thiết kế, xử lý tốt các trường hợp biên và có đầy đủ các ca kiểm thử đơn vị (unit test) đi kèm.

**Mức 2: An toàn (Secure)**
Mã nguồn phải đảm bảo không chứa các lỗ hổng bảo mật nghiêm trọng (như SQL Injection, XSS), bảo vệ tốt thông tin định danh cá nhân (PII) và thực hiện lọc dữ liệu đầu vào nghiêm ngặt.

**Mức 3: Dễ đọc (Readable)**
Cấu trúc code phải tường minh, đặt tên biến và hàm gợi nhớ ý nghĩa rõ ràng, tuân thủ các quy chuẩn trình bày chung của dự án để giảm thiểu tối đa tải nhận thức của các lập trình viên khác khi đọc code.

**Mức 4: Tao nhã (Elegant)**
Mã nguồn tận dụng hợp lý các mẫu thiết kế (design patterns) kinh điển, giải quyết bài toán phức tạp bằng cấu trúc logic ngắn gọn, sạch sẽ nhất. Việc viết và đọc mã nguồn mang lại cảm giác thích thú cho lập trình viên.

**Mức 5: Vị tha (Altruist)**
Mức độ cao nhất: Mã nguồn được thiết kế tốt đến mức đóng vai trò làm tài liệu học tập, truyền cảm hứng cải tiến kỹ thuật cho các kỹ sư khác khi tiếp cận dự án.

## 言论

1、

Gần đây tôi thử tắt hoàn toàn tính năng hoạt ảnh chuyển động (animations) trong phần cài đặt của điện thoại Android. Tốc độ phản hồi tức thì không có độ trễ của thiết bị khiến tôi thực sự kinh ngạc, cảm giác như chiếc điện thoại bỗng dưng chạy nhanh hơn gấp đôi vậy.

-- Trích chia sẻ trên Hacker News

2、

Mục đích của việc đi du lịch không phải là để ngắm nhìn những cảnh vật xa lạ khác biệt, mà là để học cách nhìn nhận mọi sự việc xung quanh dưới một góc nhìn mới mẻ khác đi.

-- Ben Davenport, nhà đầu tư mạo hiểm

3、

Những ai sang Thái Lan để làm việc thường phàn nàn đó là một nơi tệ hại; nhưng những ai sang Thái Lan để nghỉ dưỡng thì đều ca ngợi đó là một thiên đường tuyệt vời.

-- Trích bình luận của cư dân mạng

4、

Triết lý của lập trình hướng đối tượng (OOP) là cố gắng thiết kế mô hình hóa ngôn ngữ lập trình để thích ứng với bài toán thực tế, thay vì bẻ cong bài toán thực tế để ép nó thích ứng với cấu trúc cú pháp của ngôn ngữ.

-- Trích giáo trình 《C Primer Plus》

5、

Khi mới vào nhận việc, công ty cấp cho mỗi nhân viên mới một chiếc máy tính xách tay. Nhìn bề ngoài thì giống như mỗi người đang sở hữu một chiếc máy tính, nhưng thực tế bản chất là công ty đang trang bị cho mỗi chiếc máy tính một nhân sự vận hành tương ứng mà thôi.

-- Trích châm ngôn mạng

## 历史上的本周

- 2020年（第 105 期）：[Kỷ nguyên bùng nổ của các ngành dịch vụ trực tuyến](https://www.ruanyifeng.com/blog/2020/04/weekly-issue-105.html)
- 2019年（第 53 期）：[Dùng kết quả xét nghiệm DNA để tìm kiếm bạn đời](https://www.ruanyifeng.com/blog/2019/04/weekly-issue-53.html)
- 2018年（第 2 期）：[Tại sao tôi lại kiên trì viết bản tin hàng tuần?](https://www.ruanyifeng.com/blog/2018/04/weekly-issue-2.html)

## 订阅

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97)。

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](https://cdn.beekka.com/blogimg/asset/202103/bg2021030402.jpg)

（Hết）
