# Bản tin chia sẻ công nghệ (Số 251): Đề xuất máy tính đơn bản (SBC) nội địa

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3022) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041803.webp)

Lễ hội Diều Quốc tế Duy Phường lần thứ 40 đã chính thức khai mạc vào ngày 15 tháng 4, bầu trời ngập tràn những cánh diều khổng lồ với đủ hình thù độc đáo và kỳ lạ. (Nguồn: [Tân Hoa Xã](http://www.news.cn/photo/2023-04/15/c_1129526643_2.htm))

## 本周话题：国产单板机值得推荐

Vài ngày trước, khi có nhu cầu bổ sung thêm thiết bị phần cứng cho phòng làm việc, tôi đã thử khảo sát giá bán của dòng máy tính nhúng Raspberry Pi (thường gọi là Pi) và thực sự bị sốc trước mức giá hiện tại của nó.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041907.webp)

Với những bạn đọc chưa quen thuộc với khái niệm này, tôi xin giới thiệu ngắn gọn: Raspberry Pi thực chất là một bảng mạch điện tử tích hợp sẵn bộ vi xử lý (CPU), bộ nhớ RAM cùng các cổng giao tiếp ngoại vi (IO). Về cơ bản, nó hoạt động như một thùng máy tính mini siêu nhỏ gọn. Sau khi mua về, bạn chỉ cần nạp hệ điều hành vào thẻ nhớ là có thể sử dụng nó như một máy tính văn phòng hoặc máy chủ chạy ngầm trong gia đình.

**Các sản phẩm máy tính được tích hợp gọn gàng trên một bảng mạch điện tử duy nhất như thế này được gọi chung là Máy tính đơn bản** (Single-Board Computer - viết tắt là SBC).

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041909.webp)

Các dòng máy tính đơn bản trên thị trường có kích thước rất đa dạng, trong đó Raspberry Pi thuộc nhóm siêu nhỏ gọn và từng có mức giá cực kỳ rẻ.

Vào tháng 6 năm 2019 khi dòng Raspberry Pi 4B chính thức ra mắt, mức giá công bố của hãng chỉ dao động từ 35 USD (cho phiên bản RAM 2GB) đến 55 USD (cho phiên bản cấu hình cao nhất RAM 8GB). Tính ra, giá của phiên bản đắt nhất thời điểm đó chỉ khoảng hơn 1,2 triệu đồng tiền Việt.

Thế nhưng trong giai đoạn dịch bệnh kéo dài, giá bán của dòng máy này liên tục bị đẩy lên cao do khan hiếm chip toàn cầu. Vào tháng 2 năm ngoái, tôi mua một bảng mạch Raspberry Pi 4B bản RAM 8GB với giá 800 nhân dân tệ (khoảng 2,7 triệu đồng) và lúc đó đã tự thấy mức giá này quá đắt đỏ.

Các bạn thử đoán xem giá của nó hiện tại là bao nhiêu?

Tại thời điểm tháng 4 năm 2023, phiên bản RAM 8GB đang được chào bán với giá khoảng 1.400 nhân dân tệ (gần 4,8 triệu đồng), và phiên bản RAM 2GB cũng có giá lên tới 900 nhân dân tệ (khoảng 3 triệu đồng).

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041910.webp)

Thật khó tin khi một bảng mạch điện tử đã được đưa vào sản xuất từ bốn năm trước, thay vì mất giá theo thời gian như các thiết bị công nghệ thông thường, nay lại tăng giá gấp hai đến ba lần! Có lẽ chúng ta phải thay đổi thế giới quan: hóa ra đồ điện tử đôi khi cũng là một kênh đầu tư giữ giá và sinh lời...

Quan điểm thực tế của tôi là với mức giá đắt đỏ như hiện nay, chúng ta hoàn toàn không cần cân nhắc mua Raspberry Pi nữa vì nó đã mất đi giá trị hiệu năng trên giá thành (P/P). **Thị trường hiện nay đã xuất hiện rất nhiều sản phẩm thay thế có giá rẻ hơn nhưng sở hữu hiệu năng mạnh mẽ hơn vượt trội.**

Tôi đề xuất các bạn nên hướng sự chú ý sang các dòng máy tính đơn bản (SBC) nội địa do các doanh nghiệp trong nước sản xuất. Trước đây, các dòng bo mạch mô phỏng Raspberry Pi của các hãng nội địa thường bị đánh giá là thô sơ, gia công kém và bị gọi là "bo mạch nhái" (shanzhai). Tuy nhiên, cục diện hiện nay đã hoàn toàn thay đổi.

Những năm gần đây, **ngành sản xuất máy tính đơn bản nội địa đã có những bước tiến vượt bậc**. Các sản phẩm không chỉ có chất lượng gia công bo mạch cực kỳ tinh xảo, đầy đủ cổng kết nối hiện đại mà còn sở hữu nhiều ý tưởng thiết kế sáng tạo cùng ngoại hình bắt mắt, xứng đáng xếp vào nhóm sản phẩm cao cấp. Hãy nhìn các mẫu sản phẩm dưới đây xem bạn có bị thu hút không:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041913.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041912.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041911.webp)

Tuy có kích thước nhỏ gọn nằm trong lòng bàn tay, hiệu năng của các bo mạch SBC này không hề yếu. Chúng hoàn toàn đáp ứng tốt các tác vụ văn phòng, máy chủ nhỏ, lưu trữ mạng gia đình với ưu điểm tiết kiệm điện năng tối đa và tính cơ động cao. Tất nhiên, do giới hạn phần cứng nên chúng không phù hợp cho các tác vụ xử lý đồ họa 3D nặng hay tính toán lượng dữ liệu lớn.

Tôi đã lần lượt mua thử vài mẫu bo mạch nội địa này để sử dụng và đều cảm thấy rất hài lòng. Trên nền tảng YouTube, nhiều lập trình viên nước ngoài sau khi mua trải nghiệm cũng dành những lời khen ngợi nhiệt tình và khuyên dùng các sản phẩm này.

Thực trạng của các dòng máy tính đơn bản nội địa hiện nay là: chất lượng phần cứng vô cùng tuyệt vời, nhưng điểm hạn chế lớn nhất lại nằm ở phần mềm. Hệ thống tài liệu hướng dẫn kỹ thuật bằng tiếng Anh còn thiếu sót, các bộ công cụ phát triển phần mềm đi kèm chưa tối ưu và cộng đồng người dùng hỗ trợ còn quá nhỏ bé, khoảng cách với các sản phẩm quốc tế ở mảng này vẫn còn khá lớn.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041914.webp)

Nhắc đến phần cứng nội địa, tôi muốn đặc biệt đề xuất các bạn tìm hiểu dòng **vi xử lý Rockchip RK3588**. Đây là dòng CPU cấu trúc ARM do doanh nghiệp trong nước tự thiết kế. Kể từ khi các lệnh cấm vận công nghệ áp đặt lên mảng chip của Huawei, RK3588 có lẽ là dòng chip ARM mạnh mẽ nhất do Trung Quốc tự thiết kế nội địa, với hiệu năng được đánh giá tương đương dòng chip Snapdragon 855 đến 865 của Qualcomm.

Rất nhiều dòng bo mạch SBC thế hệ mới hiện nay được trang bị con chip RK3588 này. Tôi khuyên các lập trình viên nên chú ý đến nó, bởi với hiệu năng xử lý mạnh mẽ, dung lượng RAM hỗ trợ lớn và đa dạng cổng kết nối ngoại vi, dòng chip này mở ra rất nhiều hướng ứng dụng thú vị, ví dụ như tự dựng một máy tính để bàn mini chạy hệ điều hành Android mượt mà.

Đặt lên bàn cân so sánh, Raspberry Pi hoàn toàn không có cửa so về hiệu năng và giá thành với các bo mạch RK3588 nội địa: các dòng máy chạy chip RK3588 có hiệu năng mạnh gấp 2 đến 3 lần Raspberry Pi, cung cấp nhiều cổng kết nối tốc độ cao hơn, nhưng giá bán thực tế lại rẻ hơn tới 1/3.

Tóm lại, các sản phẩm máy tính đơn bản nội địa đang sở hữu năng lực cạnh tranh cực kỳ đáng nể trên thị trường. Tôi tin rằng các nhà sản xuất, người tiêu dùng và các chính sách hỗ trợ cần chung tay thúc đẩy phân khúc sản phẩm này để hình thành nên một ngành công nghiệp mũi nhọn vững chắc, giúp tiếp cận sâu rộng thị trường quốc tế đồng thời nâng cao trình độ phát triển phần cứng và phần mềm nội địa.

## 科技动态

1、[Hiện tượng nhiệt độ ấm lên toàn cầu giúp gia tăng số lượng cú đánh全垒打](https://thehill.com/changing-america/sustainability/climate-change/3938917-goner-climate-change-helping-batters-hit-more-home-runs-study/)

Một nghiên cứu của các nhà khí tượng học Mỹ chỉ ra rằng kể từ năm 2010 trở lại đây, các siêu sao đánh bóng tại Giải bóng chày nhà nghề Mỹ (MLB) đạt hiệu suất đánh bóng bay ra ngoài sân (home run) tăng thêm khoảng 50 cú đánh mỗi năm.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041405.webp)

Các chuyên gia phân tích hiện tượng này có liên quan trực tiếp đến sự ấm lên của khí hậu toàn cầu. Khi nhiệt độ không khí tăng cao, các phân tử không khí chuyển động nhanh hơn dẫn đến mật độ không khí giảm đi, làm giảm đáng kể lực cản của không khí tác động lên quả bóng khi bay, giúp quả bóng bay được khoảng cách xa hơn.

Theo tính toán thực nghiệm, cứ mỗi khi nhiệt độ môi trường tăng thêm 1 độ C, tỷ lệ đánh trúng cú home run sẽ tăng thêm khoảng 1%. Các nhà khoa học nhận định sự thay đổi mật độ không khí do nhiệt độ này cũng sẽ góp phần cải thiện thành tích thi đấu của vận động viên trong các môn điền kinh ngoài trời khác.

2、[NASA thử nghiệm tuyển chọn nhân sự sinh hoạt trong mô hình cabin Hỏa tinh](https://www.theguardian.com/science/2023/apr/12/nasa-texas-humans-prepare-mars)

Cơ quan Vũ trụ Mỹ (NASA) đang tiến hành tuyển chọn 4 tình nguyện viên tham gia vào dự án thực nghiệm sinh hoạt cô lập kéo dài một năm bên trong cabin mô phỏng môi trường sống trên Hỏa tinh bắt đầu từ tháng 6 tới:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041506.webp)

Thực nghiệm kéo dài một năm này nhằm thu thập dữ liệu thực tế về các nhu cầu tài nguyên sinh hoạt thiết yếu giúp con người có thể sống sót lâu dài khi đổ bộ Hỏa tinh thực tế trong tương lai.

Cấu trúc của cabin mô phỏng này được dựng bằng công nghệ in 3D sử dụng vật liệu đất sét đỏ – đây cũng là phương án xây dựng nhà ở dự kiến được áp dụng khi con người đặt chân lên Hỏa tinh:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041504.webp)

Khu vực cảnh quan xung quanh bên ngoài cabin cũng được thiết kế và trang trí bằng cát đỏ để mang lại cảm giác chân thực nhất:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041503.webp)

Diện tích sinh hoạt bên trong cabin rộng khoảng 150 mét vuông, bao gồm 4 phòng ngủ đơn độc lập cho các thành viên, một nhà vệ sinh chung, khu vực làm việc nghiên cứu, trạm y tế và không gian sinh hoạt chung:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041505.webp)

Để tăng độ chân thực cho thử nghiệm, toàn bộ hệ thống liên lạc vô tuyến kết nối giữa cabin với thế giới bên ngoài sẽ bị áp đặt độ trễ tín hiệu kéo dài 22 phút – tương đương khoảng thời gian sóng vô tuyến truyền tải giữa Trái Đất và Hỏa tinh ngoài thực tế. Trong suốt thời gian cách ly, các tình nguyện viên phải tự trồng các loại rau xanh và cà chua bên trong cabin để bổ sung nguồn thực phẩm tươi.

3、[Công nghệ hỗ trợ đo chỉ số huyết áp không tiếp xúc qua camera](https://petapixel.com/2022/12/07/researchers-develop-way-to-measure-blood-pressure-using-a-camera-and-ai/)

Các nhà nghiên cứu tại Úc và Iraq đã công bố thử nghiệm giải pháp đo huyết áp cho người dùng hoàn toàn không cần tiếp xúc vật lý thông qua việc ghi hình bằng camera:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122209.webp)

Công nghệ này chỉ yêu cầu hướng camera ghi hình cận cảnh khuôn mặt của đối tượng trong vòng 10 giây. Hệ thống AI sẽ phân tích các thay đổi sắc tố siêu nhỏ trên hai vùng trán để trích xuất tín hiệu nhịp tim và sử dụng thuật toán để tính toán ra chỉ số huyết áp tương ứng.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122210.webp)

Nhóm nghiên cứu tuyên bố độ chính xác của phương pháp này có thể đạt tới 90%. Tuy nhiên giới chuyên môn vẫn hoài nghi về tính thực tiễn của nghiên cứu này, bởi ngay cả các thiết bị đeo thông minh tiếp xúc trực tiếp trên cổ tay hiện nay vẫn gặp nhiều khó khăn trong việc đo chính xác huyết áp, nên việc chỉ dùng camera ghi hình từ xa đạt độ chính xác cao là điều khó tin.

4、[MIT chế tạo thành công tấm pin năng lượng mặt trời siêu mỏng nhẹ như giấy](https://spectrum.ieee.org/thin-film-solar-panels)

Các kỹ sư tại Viện Công nghệ Massachusetts (MIT) đã phát triển thành công thế hệ pin mặt trời màng mỏng siêu nhẹ, với độ dày tối thiểu và trọng lượng mỗi mét vuông chỉ khoảng 100 gram:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122301.webp)

Để so sánh, các tấm pin mặt trời khung kính truyền thống có trọng lượng lên tới 10,7 kg trên mỗi mét vuông, nặng gấp 100 lần so với thiết kế mới này. Nhờ độ mỏng và trọng lượng siêu nhẹ, tấm pin này có thể cuộn lại như một tấm thảm trải trực tiếp lên mái nhà, giúp tiết kiệm tối đa chi phí lắp đặt khung đỡ.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122302.webp)

Đồng thời, sản phẩm này mở ra khả năng tích hợp năng lượng mặt trời lên các bề mặt di động chịu tải kém trước đây như cánh buồm thuyền, cánh máy bay không người lái (UAV), lều dã ngoại hoặc dán trực tiếp lên bề mặt cửa kính tòa nhà.

5、[Bác sĩ Thử nghiệm áp dụng liệu pháp kê đơn đi bảo tàng điều trị trầm cảm](https://www.theguardian.com/world/2022/sep/17/museums-on-prescription-brussels-tests-cultural-visits-to-treat-anxiety)

Để giúp các bệnh nhân đối phó với hội chứng lo âu và trầm cảm do áp lực cuộc sống hiện đại, các bác sĩ tại Bỉ đã thử nghiệm phương án điều trị mới mang tên "liệu pháp bảo tàng":

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092112.webp)

Các bác sĩ sẽ kê đơn yêu cầu bệnh nhân cùng gia đình hoặc bạn bè thực hiện các chuyến tham quan tới hệ thống các bảo tàng nghệ thuật và lịch sử của thành phố Brussels.

Cơ sở khoa học của phương pháp này dựa trên nhận định chứng lo âu và trầm cảm có một phần nguyên nhân từ việc người bệnh tự cô lập trong không gian kín và thiếu các tương tác xã hội ngoài trời. Việc bước chân ra ngoài, cùng người thân tản bộ trong không gian yên tĩnh, thư thái đầy tính nghệ thuật của bảo tàng và tiếp xúc gián tiếp với những người xung quanh giúp xoa dịu hệ thần kinh và phục hồi tâm trạng bình tĩnh cho người bệnh.

## Bài viết

1\. [Nghiên cứu thực tế về xu hướng ứng dụng công nghệ AI của các nhà sáng tạo](https://finance.sina.com.cn/tech/internet/2023-04-14/doc-imyqirfn0665866.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041401.webp)

Bài đăng trên tạp chí *Tuần báo Tin tức Trung Quốc* khảo sát thực tế việc các tác giả viết văn, họa sĩ vẽ minh họa và nhạc sĩ trong nước đang tích cực đưa các công cụ trí tuệ nhân tạo (AI) vào quy trình sáng tác nghệ thuật hàng ngày để nâng cao hiệu suất.

2\. [Hướng dẫn chi tiết quy trình thuê card đồ họa GPU trên đám mây AWS](https://mp.weixin.qq.com/s/47DW9OBNOS0_fUxDAicARQ)（Tiếng Trung）

Đối với các nhà phát triển muốn tự chạy thử nghiệm các mô hình AI lớn, chi phí đầu tư phần cứng GPU vật lý là rất lớn. Giải pháp tối ưu là thuê các máy chủ ảo có card đồ họa GPU từ các nhà cung cấp đám mây. Tác giả chia sẻ chi tiết kinh nghiệm thiết lập và thuê GPU trên hạ tầng AWS. (Đóng góp của [@cocomany](https://github.com/ruanyf/weekly/issues/3054))

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041801.webp)

3\. [Ứng dụng API `Intl.Segmenter` hỗ trợ phân đoạn từ vựng trong JavaScript](https://www.stefanjudis.com/today-i-learned/how-to-split-javascript-strings-with-intl-segmenter/)（Tiếng Anh）

`Intl.Segmenter` là một API tiêu chuẩn được tích hợp sẵn trong các trình duyệt hiện đại hỗ trợ lập trình viên thực hiện phân đoạn từ vựng (word segmentation) một cách thông minh cho nhiều ngôn ngữ khác nhau (bao gồm cả các ngôn ngữ không sử dụng khoảng trắng phân cách từ như tiếng Trung, tiếng Nhật). Bài viết giới thiệu cách sử dụng cơ bản của API này.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023010403.webp)

4\. [Những bài học đúc kết sau chặng đường 5 năm làm nhà phát triển độc lập](https://allisonseboldt.com/5-years-of-indie-hacking/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041906.webp)

Tác giả chia sẻ những câu chuyện thực tế và đúc kết ra 3 bài học kinh nghiệm quản lý tài chính và định hướng sản phẩm quan trọng sau 5 năm quyết định xin nghỉ việc tại công ty để tự phát triển các sản phẩm phần mềm cá nhân (Indie Hacker).

5\. [Bài viết phân tích và so sánh hiệu năng thực tế giữa Bun và Node.js](https://grifel.dev/bun-dev-experience/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030711.webp)

Bun là một runtime JavaScript thế hệ mới đang nổi lên như một giải pháp thay thế cho Node.js với ưu điểm tốc độ xử lý vượt trội. Tác giả thực hiện các bài benchmark thực tế so sánh tốc độ khởi động và xử lý tác vụ mạng giữa hai môi trường này.

6\. [Mô hình bản tin điện tử TLDR Newsletter đem lại doanh thu triệu USD](https://growthinreverse.com/tldr/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011301.webp)

Bài phân tích kỹ kinh doanh kể về hành trình xây dựng bản tin công nghệ TLDR Newsletter – một bản tin điện tử gửi qua email hàng ngày được vận hành bởi một người duy nhất nhưng đã thu hút hàng triệu người đăng ký đọc tin và mang lại doanh thu quảng cáo vượt mốc 5 triệu USD mỗi năm.

7\. [Lý do tôi từng lựa chọn giải thuật sắp xếp không ổn định cho nhân V8 Chrome](https://medium.com/@erik_68861/sorting-algorithms-that-dont-hate-you-165ba313bbc2)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011303.webp)

Tác giả – một cựu thành viên phụ trách thuật toán sắp xếp của đội ngũ phát triển V8 Engine – giải thích nguyên nhân và các cân nhắc tối ưu hóa hiệu năng tại thời điểm đó khi quyết định chọn thuật toán sắp xếp không ổn định (unstable sort) cho hàm `Array.prototype.sort()` của Chrome (dù sau này đặc tả ECMA đã chính thức thay đổi yêu cầu bắt buộc phải là thuật toán ổn định).

8\. [Trình duyệt Firefox thử nghiệm tính năng tự động chặn các banner xin quyền Cookie](https://www.ghacks.net/2023/04/17/firefox-may-interact-with-cookie-prompts-automatically-soon/)（Tiếng Anh）

Hầu hết các trang web nước ngoài hiện nay đều hiển thị một hộp thoại popup lớn yêu cầu người dùng nhấp chọn đồng ý lưu trữ Cookie (Cookie banners) gây phiền toái khi lướt web. Firefox công bố đang thử nghiệm tính năng tự động chặn và ẩn các popup phiền toái này cho người dùng.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041905.webp)

## Công cụ

1、[Nango: Dịch vụ nguồn mở quản lý các token xác thực OAuth](https://www.nango.dev/)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020804.webp)

Một giải pháp phần mềm nguồn mở cho phép các nhà phát triển tự thiết lập máy chủ chuyên quản lý và làm mới các token xác thực OAuth của người dùng khi kết nối với các API dịch vụ bên thứ ba (như GitHub, Google, Slack).

2、[docker-rollout: Cập nhật các container Docker Compose không gây gián đoạn](https://github.com/Wowu/docker-rollout)

Tiện ích dòng lệnh hỗ trợ cập nhật phiên bản ứng dụng trong Docker Compose theo cơ chế cuộn (rollout): hệ thống sẽ tự động khởi chạy container mới song song với container cũ, chờ kiểm tra trạng thái hoạt động ổn định rồi mới tắt container cũ để bảo đảm hệ thống hoạt động liên tục không bị gián đoạn.

3、[Web LLM: Khởi chạy các mô hình ngôn ngữ lớn trực tiếp trên trình duyệt](https://mlc.ai/web-llm/)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041601.webp)

Dự án nghiên cứu đột phá sử dụng thư viện WebGPU để cho phép người dùng tải và chạy trực tiếp các mô hình ngôn ngữ lớn (LLM) ngay trên môi trường trình duyệt web mà không cần gửi dữ liệu về máy chủ, hỗ trợ hoạt động ngoại tuyến (offline) hoàn toàn. Bạn đọc có thể xem thêm [bài viết đánh giá chi tiết](https://simonwillison.net/2023/Apr/16/web-llm/).

4. [openai-public: Dự án giao diện web kết nối API OpenAI viết bằng Node.js](https://github.com/KiritoCheng/openai-public)

Mã nguồn mở xây dựng ứng dụng frontend trò chuyện với ChatGPT, được lập trình bằng Express Node.js kết nối trực tiếp với API của OpenAI. (Đóng góp của [@KiritoCheng](https://github.com/ruanyf/weekly/issues/3055) - Xem thêm [mã nguồn backend](https://github.com/KiritoCheng/openai-server)).

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041802.webp)

5、[Animated Drawings: Công cụ AI biến hình vẽ phác thảo tay thành hoạt ảnh](https://github.com/facebookresearch/AnimatedDrawings)

Dự án nghiên cứu nguồn mở từ Meta (Facebook Research) cung cấp công cụ AI tự động nhận diện các khớp xương trên hình vẽ nhân vật do trẻ em tự vẽ tay trên giấy để tự động sinh ra các đoạn hoạt hình di động ngộ nghĩnh:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041402.webp)

6、[scrutiny: Tiện ích giám sát sức khỏe ổ cứng theo chỉ số S.M.A.R.T qua giao diện web](https://github.com/AnalogJ/scrutiny)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111403.webp)

Hệ thống giám sát và quản lý ổ cứng nguồn mở hỗ trợ thu thập và phân tích các chỉ số S.M.A.R.T của toàn bộ ổ cứng trong máy, hiển thị cảnh báo sức khỏe chi tiết qua một trang web dashboard đẹp mắt chạy bằng Docker.

7、[browsertunnel: Tiện ích truyền tải thông tin ẩn ngầm qua giao thức DNS](https://github.com/veggiedefender/browsertunnel)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111405.webp)

Công cụ mô phỏng phương thức truyền tải dữ liệu từ trình duyệt ra máy chủ bên ngoài bằng cách đóng gói thông tin ẩn bên trong các truy vấn truy tìm tên miền (DNS Queries) thay vì dùng kết nối HTTP thông thường, giúp vượt qua các hệ thống tường lửa giám sát mạng của doanh nghiệp một cách tinh vi.

8、[Upbase: Ứng dụng quản trị công việc và cộng tác nhóm tất-cả-trong-một](https://upbase.io/)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111406.webp)

Một ứng dụng web hướng tới việc tối ưu hóa hiệu suất làm việc nhóm, tích hợp đồng bộ các tính năng quản lý dự án (Project Management), lịch biểu công việc cá nhân, ứng dụng chat nội bộ và tài liệu cộng tác trên cùng một nền tảng.

9、[Bot Aquarium: Dự án máy ảo Linux vận hành hoàn toàn bằng AI OpenAI](https://github.com/fafrd/aquarium)

Dự án thử nghiệm thú vị: thiết lập một môi trường máy ảo Linux và chuyển quyền điều khiển hoàn toàn cho AI. Người dùng chỉ cần gõ yêu cầu công việc mong muốn bằng ngôn ngữ tự nhiên, hệ thống sẽ gửi yêu cầu tới OpenAI để tự động sinh lệnh shell và thực thi trực tiếp trên máy ảo cho đến khi hoàn thành mục tiêu.

10、[Autodoc: Tự động biên soạn tài liệu mã nguồn bằng AI tích hợp CI/CD](https://github.com/context-labs/autodoc)

Công cụ ứng dụng các mô hình LLM để tự động phân tích cấu trúc mã nguồn của dự án và viết tài liệu hướng dẫn kỹ thuật chi tiết (documentation), hỗ trợ tích hợp sâu vào quy trình CI/CD để tự động cập nhật tài liệu mỗi khi có pull request mới.

11、[SceneXplain: Dịch vụ ứng dụng AI mô tả chi tiết nội dung hình ảnh](https://scenex.jina.ai/)

Dịch vụ web ứng dụng trí tuệ nhân tạo hỗ trợ phân tích sâu các chi tiết trong bức ảnh người dùng tải lên để đưa ra một đoạn văn bản mô tả bối cảnh và sự vật một cách tỉ mỉ và tự nhiên.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040613.webp)

## 资源

1、[SICP JavaScript Edition: Giáo trình cấu trúc chương trình máy tính phiên bản JS](https://sourceacademy.org/sicpjs/index)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023020807.webp)

Bản dịch chính thức sử dụng ngôn ngữ JavaScript của cuốn sách giáo khoa kinh điển *SICP (Structure and Interpretation of Computer Programs)* do MIT Press phát hành, cho phép sinh viên đọc trực tuyến hoàn toàn miễn phí.

2、[WebGPU Fundamentals: Giáo trình học lập trình WebGPU cho Front-end](https://webgpufundamentals.org/)

Trang web cung cấp hệ thống các bài học viết bằng tiếng Anh hướng dẫn chi tiết từ cơ bản đến nâng cao cách thức khai thác sức mạnh đồ họa của GPU thông qua thư viện API WebGPU thế hệ mới trên trình duyệt.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041603.webp)

3、[GPT Unicorn: Dự án ghi nhận tiến trình tiến hóa tư duy đồ họa của GPT-4](https://gpt-unicorn.adamkdean.co.uk/)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041404.webp)

Một trang web ghi lại nhật ký vẽ tranh của GPT-4: hàng ngày hệ thống sẽ gửi cùng một câu lệnh yêu cầu GPT-4 tự viết mã nguồn SVG để vẽ một chú độc giác thú (unicorn) và đăng lên web để cộng đồng theo dõi sự thay đổi năng lực dựng hình của AI qua các ngày.

4、[Vercel AI Playground: Nền tảng thử nghiệm và so sánh các mô hình AI lớn](https://play.vercel.ai/)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023041903.webp)

Dịch vụ web do tập đoàn Vercel xây dựng cho phép lập trình viên chạy thử nghiệm và đặt cạnh nhau để so sánh trực quan chất lượng kết quả trả về của nhiều mô hình ngôn ngữ lớn (LLMs) khác nhau cùng lúc.

5、[Playlist Genius: Trình tự động tạo danh sách phát nhạc Spotify bằng AI](https://www.playlistgeniusai.com/)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040201.webp)

Tiện ích web kết nối với tài khoản Spotify: người dùng chỉ cần mô tả tâm trạng hoặc thể loại nhạc muốn nghe bằng ngôn ngữ tự nhiên, AI sẽ tự động tìm kiếm và tạo ra một playlist nhạc phù hợp nhất.

## 图片

1、**Chiến dịch tỉ mỉ phục dựng các cổ vật thủy tinh bị phá hủy sau vụ nổ cảng Beirut**

Vào ngày 4 tháng 8 năm 2020, vụ nổ hóa chất kinh hoàng tại cảng Beirut, Liban đã tàn phá nặng nề các khu vực xung quanh. Bảo tàng khảo cổ học địa phương cũng chịu ảnh hưởng lớn: sức ép của vụ nổ làm vỡ vụn tủ trưng bày chứa 74 bình thủy tinh cổ đại quý hiếm, các mảnh vỡ cổ vật trộn lẫn với mảnh kính cửa sổ vỡ vụn rải khắp mặt sàn:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042006.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110805.webp)

Các nhân viên bảo tàng đã kiên trì nhặt nhạnh và phân loại từng mảnh vỡ nhỏ nhất để chuẩn bị cho công tác phục dựng:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110806.webp)

Do độ khó quá cao, toàn bộ các thùng mảnh vỡ sau đó đã được chuyển đến phòng phục chế của Bảo tàng Anh (London) để các chuyên gia hàng đầu thực hiện ghép lại bằng các chất keo chuyên dụng dưới kính hiển vi:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110807.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110808.webp)

Dưới đây là hình ảnh bốn chiếc bình cổ đại đã được phục dựng thành công về nguyên trạng. Đến nay, các chuyên gia đã khôi phục hoàn chỉnh được 26 món cổ vật và vẫn đang tiếp tục xử lý các phần còn lại:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110809.webp)

2、**Màn trình diễn flycam phục dựng lại kiến trúc cổ đại bị phá hủy của Hà Lan**

Một nhóm nghệ sĩ người Hà Lan đã thực hiện dự án nghệ thuật đặc biệt: sử dụng hàng trăm thiết bị bay không người lái (drones) lập trình chiếu sáng tự động trong đêm để vẽ lại hình dáng nguyên bản của các công trình kiến trúc cổ đại bị tàn phá ngay trên nền phế tích hiện tại:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110810.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110811.webp)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110812.webp)

## ✍️ Bài đọc thêm

### Mối tương quan giữa thói quen đóng cửa và mở cửa phòng làm việc của các nhà khoa học

Đoạn trích dưới đây được trích từ bài phát biểu chia sẻ kinh nghiệm nghiên cứu khoa học kinh điển mang tên *“Bạn và các nghiên cứu của bạn” (You and Your Research)* của nhà toán học kiêm kỹ sư máy tính nổi tiếng Richard Hamming tại phòng thí nghiệm Bell:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042002.webp)

> “Tại phòng nghiên cứu của tập đoàn Bell, mỗi nhà khoa học đều được bố trí một văn phòng làm việc độc lập.
> 
> Tôi đã dành nhiều năm quan sát thói quen sinh hoạt của các đồng nghiệp xung quanh và nhận thấy một quy luật rất thú vị: Nếu bạn chọn cách đóng chặt cửa phòng làm việc của mình, bạn sẽ ít bị làm phiền hơn, từ đó hoàn thành được nhiều đầu việc hơn trong ngày và có năng suất làm việc ngắn hạn cao hơn hẳn so với số đông còn lại.
> 
> Thế nhưng, sau khoảng chặng đường 10 năm nhìn lại, có một hiện tượng kỳ lạ xảy ra: những nhà nghiên cứu có thói quen đóng cửa phòng dần mất đi khả năng nhạy bén trong việc xác định xem đâu là những bài toán khoa học thực sự có giá trị cốt lõi cần tập trung giải quyết. Toàn bộ những công việc họ cặm cụi nghiên cứu suốt nhiều năm qua bỗng trở nên ít quan trọng và thiếu tính ứng dụng thực tế.
> 
> Trong khi đó, những nhà khoa học chọn cách luôn mở rộng cửa phòng làm việc của mình khi nghiên cứu tuy thường xuyên phải đối mặt với đủ loại xao nhãng phát sinh từ những người xung quanh đi qua đi lại, nhưng đổi lại họ luôn nhận được những luồng thông tin gợi ý mới mẻ từ thế giới bên ngoài để biết được xu hướng phát triển thực tế của ngành công nghiệp đang ra sao và đâu là những bài toán lớn thực sự cần tìm lời giải.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042001.webp)

> Tôi nhận thấy có một mối tương quan chặt chẽ giữa những người có thói quen mở cửa phòng làm việc với nhóm những nhà khoa học gặt hái được những thành tựu nghiên cứu vĩ đại có tầm ảnh hưởng lớn sau này.
> 
> Mặc dù những người đóng cửa phòng làm việc thường có thái độ cặm cụi chăm chỉ hơn, nhưng do thiếu đi sự giao thoa chia sẻ thông tin với thế giới xung quanh, họ rất dễ đi chệch hướng nghiên cứu và bỏ lỡ cơ hội chạm tay vào những phát kiến vĩ đại của cuộc đời mình.”

## Lịch sử tuần này

- 2022年（第 204 期）：[Phương pháp tư duy: Lời khuyên về cách giữ vững tinh thần vượt qua dịch bệnh và khó khăn](http://www.ruanyifeng.com/blog/2022/04/weekly-issue-204.html)
- 2021年（第 154 期）：[Lịch sử công nghệ: Nhìn lại các dự báo về sự phát triển của xã hội thông tin từ năm 1982](http://www.ruanyifeng.com/blog/2021/04/weekly-issue-154.html)
- 2020年（第 104 期）：[Công nghệ âm thanh: Khảo sát thực tế các ứng dụng thực tiễn của công nghệ tổng hợp giọng nói](http://www.ruanyifeng.com/blog/2020/04/weekly-issue-104.html)
- 2019年（第 54 期）：[Hoạt động cộng đồng: Thảo luận về loại hình sự kiện có khả năng mở rộng quy mô tốt nhất](http://www.ruanyifeng.com/blog/2019/05/weekly-issue-54.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs is a dynamic collaboration space.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
