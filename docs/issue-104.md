# 科技爱好者周刊：第 104 期 (Bản tin chia sẻ công nghệ số 104)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

[Thông báo] Thứ Sáu tuần sau là kỳ nghỉ lễ 1/5, bản tin sẽ phát hành sớm một ngày vào thứ Năm (ngày 30 tháng 4).

## Ảnh bìa

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041808.jpg)

Cuộc thi bắp cải khổng lồ tổ chức ở Alaska, Mỹ, ba người đoạt giải chụp ảnh lưu niệm. Giải nhất (quả ở giữa) nặng 41,9 kg. ([Nguồn](https://www.npr.org/sections/thesalt/2014/08/20/341884706/why-vegetables-get-freakish-in-the-land-of-the-midnight-sun))

## Chủ đề tuần này: Công dụng của tổng hợp giọng nói

Google năm 2018 đã công bố [một bài báo](https://google.github.io/tacotron/publications/speaker_adaptation/), chỉ cần 5 giây giọng nói người thật, có thể trích xuất đặc trưng giọng nói, sau đó bất kỳ văn bản nào đều có thể chuyển thành giọng nói của người đó.

Link ở trên có nhiều mẫu giọng nói được tổng hợp bằng công nghệ này, mọi người có thể đến nghe thử, rất ấn tượng.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042202.jpg)

Nếu công nghệ này được phổ biến, thực ra khá nguy hiểm. Tôi biết một sự việc có thật, một đồng nghiệp hôm đó nhận điện thoại lừa đảo, tự xưng con anh ta bị bắt cóc, yêu cầu trả tiền chuộc. Tất nhiên anh ấy không bị lừa, nhưng nếu những kẻ lừa đảo đó dùng công nghệ này của Google, qua điện thoại phát một đoạn giọng nói tổng hợp của con trai anh ta, có lẽ rất dễ tin.

Tôi còn nghĩ đến một công dụng khác. Về sau khi người chết đi, giọng nói của họ vẫn còn sống, kết hợp với trí tuệ nhân tạo, có thể tiến hành hội thoại ảo với người đã khuất.

Nhà văn Mỹ Philip K. Dick đã viết một cuốn tiểu thuyết khoa học viễn tưởng "Ubik". Ông tưởng tượng trong thế giới tương lai, người sau khi chết vẫn có thể tiếp tục "tồn tại" một thời gian dưới dạng sóng não. Mọi người sẽ bảo quản lạnh thân thể người thân và bạn bè đã khuất trong nhà linh hồn, người sống dùng thiết bị sóng não để "nói chuyện" với sóng não của người đã khuất.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042201.jpg)

Tôi cho rằng, công nghệ hiện có đã có thể thực hiện lời tiên đoán này rồi. Đặc điểm sinh lý, thói quen hành vi, bài viết đã viết, lời đã nói của một người, đều có thể nhập vào máy tính tạo mô hình (tiếng Anh gọi là avatar), thu được ngoại hình, giọng nói, cách suy nghĩ, từng cử chỉ hành động giống hệt. Người khác tương tác với avatar này, giống như tương tác với người thật.

Mô hình này có thể được thương mại hóa, như đã nói ở trên, mọi người sẽ sẵn sàng mua avatar của người thân đã khuất, để người thân vẫn còn ở bên chúng ta. Avatar của một số người nổi tiếng nhất định có thị trường khổng lồ, thiếu niên yêu thích thần tượng về sau sẽ không đi xem buổi hòa nhạc, mà là mua avatar của thần tượng, muốn nghe bài gì thì nhờ nó hát cho nghe. Nền tảng thương mại điện tử cũng sẽ ra mắt bảng xếp hạng, avatar bán chạy nhất tuần này là ai, còn có những avatar nào mới lên bảng, v.v.

## Video chuẩn bị phỏng vấn front-end

Tài liệu khóa học tuần này là một 《Video chuẩn bị phỏng vấn front-end》miễn phí.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042204.jpg)

Phỏng vấn là cửa ải cuối cùng của việc tìm kiếm việc làm, nếu chuẩn bị không tốt, sẽ dẫn đến công sức uổng phí. Hơn nữa, phỏng vấn của lập trình viên thường liên quan trực tiếp đến cấp độ và mức lương cuối cùng. Hai ứng viên các điều kiện khác đều tương tự, chỉ khác nhau về biểu hiện trong phỏng vấn, mức lương cuối cùng có thể có khoảng cách không nhỏ.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042310.jpg)

Ví dụ, nhiều nhà phỏng vấn thích hỏi về cách triển khai upload file, bạn sẽ trả lời thế nào?

> - Giáp: POST request của thư viện axios front-end + thanh tiến trình upload + Node.js backend nhận file
> - Ất: Triển khai upload file lớn theo phân mảnh và tiếp tục upload từ điểm dừng
> - Bính: Front-end giới hạn định dạng file upload + upload tức thì (kiểm tra xem backend đã có bản sao chưa)

Xin hỏi ba ứng viên Giáp, Ất, Bính, ai sẽ nhận được nhiều lương hơn, ai ít hơn?

Để giành được offer lương cao, ngoài việc chuẩn bị tốt các câu hỏi phỏng vấn cần thiết, còn nên thể hiện đặc điểm và quan điểm giá trị của mình trong quá trình phỏng vấn. Video 《Phỏng vấn front-end lương cao, câu hỏi phỏng vấn phải trả lời như thế này》 do **Kaikeba** cung cấp dưới đây, ngoài việc cho mọi người biết cách trả lời câu hỏi ở các cấp độ P5/P6/P7 khác nhau, còn giảng giải một câu hỏi phỏng vấn kinh điển của 《Jinri Toutiao》, cùng các nội dung khác.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042205.jpg)

Các bạn quan tâm, nhấn giữ mã QR bên trên hai lần, thêm thành công là có thể nhận miễn phí. Chỉ giới hạn **189 người đầu tiên**, ai đến trước được trước.

## Tin tức

1、[Động vật dài nhất thế giới](https://www.trt.net.tr/chinese/wen-hua-yi-zhu-yu-ke-ji/2020/04/14/ke-xue-jia-zai-hai-di-fa-xian-shi-jie-shang-zui-chang-de-dong-wu-1397776)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041701.jpg)

Các nhà khoa học phát hiện động vật dài nhất thế giới dưới đáy biển gần Australia. Đó là một siphonophore Apolemia, chiều dài đạt 45,7 mét. Những đường thẳng màu trắng trong hình trên đều là từng cá thể riêng lẻ.

Siphonophore là sinh vật cộng đồng bao gồm các cơ thể nhỏ, liên kết với nhau, di chuyển dưới dạng vòng tròn hoặc xoắn ốc ở đáy biển.

2、[Quảng cáo 5 giờ của iPhone](https://news.artnet.com/art-world/apple-five-hour-iphone-ad-hermitage-museum-1800798)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041702.jpg)

Để thể hiện độ bền pin của iPhone 11 pro, Apple đã quay một quảng cáo dài 5 giờ 19 phút 28 giây. Toàn bộ quảng cáo là dùng một chiếc iPhone 11 pro quay liên tục một cảnh, chứng tỏ video của nó có thể quay lâu như vậy, chất lượng tốt, hình ảnh cũng rất ổn định. Sau khi quay xong, điện thoại vẫn còn 19% pin.

Quảng cáo được quay tại Cung điện Mùa đông ở St. Petersburg, Nga, iPhone được cố định trên giá đỡ, quay liên tục 45 căn phòng lớn của cung điện này, không gian trưng bày 250 triệu feet vuông, ghi lại cung điện hùng vĩ và những bức tranh nổi tiếng trên tường, cùng các điệu múa hiện đại được sắp xếp trước. [Youtube](https://www.youtube.com/watch?v=49YeFsx1rIw) và [BiliBili](https://www.bilibili.com/video/BV1NE41137EZ/) có toàn bộ quảng cáo 5 giờ này.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041703.jpg)

3、[Bằng chứng của thuyết tương đối rộng](https://phys.org/news/2020-04-eso-telescope-star-supermassive-black.html)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041801.jpg)

27 năm trước, các nhà khoa học Pháp thông qua kính thiên văn rất lớn (VLT) của Đài thiên văn Nam Châu Âu (ESO), phát hiện có một ngôi sao S2 đang quay quanh một lỗ đen có khối lượng khổng lồ, điểm gần nhất cách 20 tỷ km (120 lần khoảng cách Mặt trời với Trái đất).

Tốc độ vận động của S2 là 3% tốc độ ánh sáng, quay một vòng mỗi 16 năm. Sau 27 năm quan sát liên tục, các nhà khoa học cuối cùng xác nhận, quỹ đạo vận hành của S2 không phải là hình elip như thuyết hấp dẫn vũ trụ của Newton tiên đoán, mà là hình bông hoa hồng như thuyết tương đối rộng của Einstein dự đoán (hình trên), điều này là do siêu khối lượng của lỗ đen gây ra. Dưới đây là [video hoạt hình](https://v.qq.com/x/page/m09536t9zaq.html) về quỹ đạo vận hành.

Đài thiên văn Nam Châu Âu (ESO) là tổ chức nghiên cứu do chính phủ 15 quốc gia tổ chức để hỗ trợ các nhà khoa học nghiên cứu thiên văn học ở Nam bán cầu, thành lập năm 1962, trụ sở đặt tại Munich, Đức, kính thiên văn và thiết bị đều đặt trong dãy núi ở Chile.

4、[Động vật tham gia hội nghị video](https://www.sweetfarm.org/goat-2-meeting)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041802.jpg)

Trong thời dịch bệnh, hội nghị video trở nên rất phổ biến. Một nông trại ở California, Mỹ ra mắt dịch vụ để động vật nông trại tham gia hội nghị video. Khi cuộc họp diễn ra, một con vật sẽ tham gia phát trực tiếp, như thể là một người tham gia cuộc họp.

Dịch vụ này có tính phí, tất cả phí thu được dùng để tài trợ hoạt động của nông trại. Người dùng đóng tối thiểu 65 đô la và gửi thời gian và link cuộc họp, có thể để một con vật tham dự cuộc họp từ xa trong 20 phút. Hiện tại, động vật có thể chọn chủ yếu là dê, sau này có thể có các loài động vật khác. Nông trại đặc biệt tuyên bố, không đảm bảo dê có trạng thái họp tốt, nó ngủ cũng là có thể.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041804.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041803.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041805.jpg)

5、[Mỹ khởi động lại chuyến bay có người lái](https://www.cnn.com/2020/04/17/tech/spacex-crew-dragon-nasa-demo-2-launch-date-scn/index.html)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041902.jpg)

NASA chính thức tuyên bố, vào lúc 4 giờ 32 phút chiều ngày 27 tháng 5 tháng tới, sẽ thông qua tên lửa của công ty SpaceX tại Florida, đưa hai phi hành gia lên Trạm Vũ trụ Quốc tế.

Kể từ khi tất cả tàu con thoi nghỉ hưu năm 2011, Mỹ không còn thực hiện chuyến bay có người lái nữa, tất cả phi hành gia Mỹ đều phải đến Nga, thông qua tàu Soyuz của Nga để đến Trạm Vũ trụ Quốc tế. Chuyến bay tháng tới sẽ là chuyến bay có người lái đầu tiên của SpaceX kể từ khi thành lập 18 năm, đánh dấu thành công lớn của công ty này. Hình trên là ảnh của hai phi hành gia Mỹ sắp lên vũ trụ.

6、**Tin tức một câu**

> - [Sinh viên đại học Mỹ](https://www.washingtonpost.com/education/2020/04/16/college-students-are-rebelling-against-full-tuition-after-classes-move-online/) phát động phong trào kiến nghị, yêu cầu trường đại học hoàn trả một phần học phí, vì trường học đều đóng cửa do dịch bệnh. Hiện tại, các trường đại học vẫn chưa đồng ý.

> - [Các nhà khoa học Mỹ](https://www.popularmechanics.com/science/a32190534/welding-tech-carbon-steel-3d-printing/) phát minh công nghệ in 3D mới, sử dụng bột thép được laser làm nóng chảy, in ra các bộ phận thép chắc chắn. Nếu sản phẩm thép cũng có thể in được, có thể thay đổi ngành thép.

> - [Microsoft](https://www.nvidia.com/en-us/geforce/news/minecraft-with-rtx-beta-out-now-download-play/) phát hành game Minecraft hỗ trợ RTX (theo dõi ánh sáng thời gian thực), hiện có thể tải xuống phiên bản trải nghiệm miễn phí.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041810.jpg)

> - [Microsoft](https://www.theverge.com/2020/4/22/21230816/microsoft-developers-bugs-machine-learning-numbers-statistics) tiết lộ, 47.000 lập trình viên của công ty tạo ra gần 30.000 bug mỗi tháng.

> - [Youtube](https://finance.sina.com.cn/roll/2020-02-14/doc-iimxyqvz2753575.shtml) tuyên bố, từ tháng 3 sẽ không còn chấp nhận người dùng iOS thanh toán đăng ký trong ứng dụng, người dùng chỉ có thể đăng ký qua trình duyệt. Vì Apple chiết khấu 30% cho việc mua trong ứng dụng, Google không muốn để Apple kiếm khoản tiền này.

> - [Cơ quan quản lý tên miền ICANN](https://www.namecheap.com/blog/icann-allows-com-price-increases-gets-more-money/) đồng ý ủy quyền cho Verisign, tăng giá tên miền `.com` 7% mỗi năm trong bốn năm tới.

> - [MIPS](https://www.cnx-software.com/2020/04/22/is-mips-dead-lawsuit-bankruptcy-maintainers-leaving-and-more/) là kiến trúc CPU mã nguồn mở, theo báo cáo tình hình hiện tại rất không khả quan. Chỉ còn lại một người duy trì cốt lõi, công ty sở hữu nó đã nộp đơn phá sản. Dự kiến kiến trúc này không lâu nữa sẽ chính thức chết.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042309.jpg)

## Bài viết

1、[Một số viên ngọc toán học từ John Conway](https://mattbaker.blog/2020/04/15/some-mathematical-gems-from-john-conway/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041610.jpg)

Gần đây, nhà toán học nổi tiếng John Conway đã qua đời vì virus COVID-19, trên mạng có nhiều bài viết tưởng niệm. Bài viết này tóm tắt một số phát hiện nhỏ ít được biết đến của ông.

Ví dụ, bất kỳ tam giác nào kéo dài các cạnh ra ngoài mỗi đỉnh, và khoảng cách bằng với cạnh đối diện, sáu điểm thu được sẽ nằm trên một đường tròn, đường tròn này gọi là "Đường tròn Conway".

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041609.jpg)

2、[Bảy lý do không nên tuyển nhà khoa học dữ liệu](https://learningwithdata.com/posts/tylerfolkman/7-reasons-not-to-hire-a-data-scientist/)（Tiếng Anh）

Bài viết này đề xuất hầu hết các công ty thực ra không cần thuê nhà khoa học dữ liệu, bốn lý do đầu tiên khá thú vị.

> - Bạn không có bất kỳ dữ liệu nào
> - Bạn không có dữ liệu đúng
> - Bạn không có vấn đề rõ ràng cần giải quyết
> - Những gì bạn thực sự cần là một nhà phân tích

3、[Tên lửa Trường Chinh 3B phóng thất bại](https://www.zhihu.com/question/386500368)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042004.jpg)

Ngày 9 tháng 4, tên lửa Trường Chinh 3B của Trung Quốc phóng thất bại. Một động cơ của giai đoạn ba không khởi động, dẫn đến cả vệ tinh và tên lửa đều bị phá hủy, rơi xuống biển gần Guam. Vì Trường Chinh 3B đã khá thuần thục, sự cố xảy ra rất bất thường, ảnh hưởng rất lớn đến các vụ phóng thương mại trong tương lai. Đây là một bài đăng trên Zhihu, thảo luận về sự kiện này phản ánh vấn đề gì trong hàng không vũ trụ Trung Quốc, và có ảnh hưởng sâu xa gì.

4、[Phân tích trình duyệt vô hiệu hóa Cookie bên thứ ba](https://juejin.im/post/5e97124df265da47b27d97ff)（Tiếng Trung）

Trình duyệt Safari bắt đầu vô hiệu hóa hoàn toàn Cookie bên thứ ba, bài viết này phân tích ảnh hưởng như thế nào, và làm thế nào để lấy dấu vân tay trình duyệt mà không có Cookie.

5、[Silicon Valley đua nhau xây dựng thế hệ internet tiếp theo: Metaverse (Vũ trụ ảo)](https://www.washingtonpost.com/video-games/2020/04/17/fortnite-metaverse-new-internet/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042005.jpg)

Phiên bản tiếp theo của internet được gọi là Metaverse (Vũ trụ ảo), nó đến từ tiểu thuyết khoa học viễn tưởng, chỉ không gian ảo được chia sẻ, tiếp tục trực tuyến và hoạt động ngay cả khi không có người đăng nhập. Hiện tại, hệ thống gần nhất với Metaverse là game trực tuyến Fortnite. Hình trên là người chơi xem trailer phim 《Star Wars》 trong Fortnite.

6、[Tôi lắp PC như thế nào](https://blog.codinghorror.com/building-a-pc-part-ix-downsizing/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042012.jpg)

Lập trình viên nổi tiếng Jeff Atwood gần đây đã "lắp ráp" một chiếc PC, đã 5 năm kể từ lần trước. Trong 5 năm đó, anh ấy không cần nâng cấp PC. Anh ấy cảm thán đây cũng là một dấu hiệu, kỷ nguyên PC sắp kết thúc.

Lần này, anh chọn case nhỏ DA2, nhét vào trong CPU i9-9900KS, GPU RTX 2080 và ba ổ cứng. Điều này không lo tản nhiệt sao?

7、[Demo server WebSocket của Node.js](https://lostmoa.com/blog/WebSocketDemoServerInNodeJS/)（Tiếng Anh）

Bài viết này giới thiệu cách tự viết một server WebSocket đơn giản.

8、[Tài nguyên học Python](https://x-team.com/blog/essential-python-resources/)（Tiếng Anh）

Bài viết này tóm tắt 10 giáo trình tiếng Anh về Python mà người mới bắt đầu nên đọc.

## Công cụ

1、[Falcon](https://github.com/plotly/falcon)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041611.jpg)

Trình soạn thảo SQL mã nguồn mở, có thể xem kết quả truy vấn.

2、[Wekan](https://wekan.github.io/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041612.jpg)

Phần mềm kanban mã nguồn mở, tương tự Trello.

3、[HoServer](https://github.com/hello-react/HoServer)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041704.jpg)

HoServer là dịch vụ giao diện RESTful và nền tảng quản lý dựa trên Node.js Express, một dòng code triển khai tất cả giao diện CRUD, tích hợp sẵn các tính năng cơ bản như người dùng, quyền hạn, có thể rút ngắn chu kỳ phát triển dự án, giảm chi phí phát triển. (@[hello-react](https://github.com/ruanyf/weekly/issues/1190) đóng góp)

4、[Learning-to-See-in-the-Dark](https://github.com/cchen156)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041809.jpg)

Một triển khai thuật toán TensorFlow, có thể thông qua machine learning, khôi phục ảnh tối tăm (bên trái nhất) thành hình dạng khi có ánh sáng (bên phải nhất).

5、[TablePlus](https://tableplus.com/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041901.jpg)

Công cụ quản lý cơ sở dữ liệu giao diện đồ họa hỗ trợ nhiều loại cơ sở dữ liệu quan hệ.

6、[tauthon](https://github.com/naftaliharris/tauthon)

Sau khi Python 2 không còn được duy trì chính thức, người dùng thông thường bắt đầu tiếp quản. Có người làm một dự án, chuyên chuyển các tính năng mới của Python 3 sang Python 2.

7、[pipedream](https://pipedream.com/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042101.jpg)

Nền tảng tích hợp dịch vụ đám mây, có thể chạy code của người dùng, xử lý đầu vào từ một dịch vụ đám mây rồi xuất ra dịch vụ đám mây khác. Hiện tại miễn phí sử dụng.

8、[avatarify](https://github.com/alievk/avatarify)

Phần mềm mã nguồn mở, chỉ cần cung cấp một ảnh chân dung, có thể tạo video nhân vật mở miệng nói chuyện.

9、[pattern.css](https://github.com/bansal-io/pattern.css)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042112.jpg)

Thư viện CSS thuần túy, cung cấp các hình nền với nhiều hình dạng khác nhau. Còn có một [trang web tương tự](http://www.heropatterns.com/).

10、[98.css](https://jdan.github.io/98.css/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042203.jpg)

Thư viện CSS cung cấp các component UI phong cách Windows 98.

## Tài nguyên

1、[ZoomerBackgrounds](https://zoomerbackgrounds.com/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041806.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020041807.jpg)

Phần mềm hội nghị video Zoom cho phép người dùng tùy chỉnh ảnh nền cuộc họp, trang web này cung cấp các tài nguyên ảnh nền khác nhau.

2、[《Học Scala bằng thực hành》](https://www.handsonscala.com/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042001.jpg)

Tutorial Scala tiếng Anh do Li Haoyi, con trai của Thủ tướng Singapore Lý Hiển Long phát hành. Li Haoyi sinh năm 1989, là developer cốt lõi của Scala.js, tốt nghiệp chuyên ngành máy tính MIT.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042002.jpg)

3、[Tiếng ồn thư viện](https://www.ox.ac.uk/soundsofthebodleian/#radcam)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042111.jpg)

Trang web này cung cấp tiếng ồn của thư viện Đại học Oxford. Các bạn thích môi trường thư viện có thể dùng nó làm âm thanh nền khi làm việc.

4、[Matheminecraft](https://www.epfl.ch/schools/sb/research/math/get-matheminecraft/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042113.jpg)

Game giáo dục toán học cho trẻ em dựa trên Minecraft.

5、[Tác phẩm nghệ thuật trí tuệ nhân tạo](https://art42.net/)

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021701.jpg)

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020021702.jpg)

Trang web này thu thập các bức tranh trừu tượng được machine learning tạo ra.

## Hình ảnh

1、[Cầu thang mèo ở Thụy Sĩ](https://99percentinvisible.org/article/swiss-cat-ladders-documenting-deconstructing-feline-friendly-infrastructure/)

Nhiều tòa nhà ở Thụy Sĩ có những cầu thang rất nhỏ trên mặt tường bên ngoài, đây không phải cho người đi, mà là cho mèo đi.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042008.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042009.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042010.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042011.jpg)

2、[Bản đồ mô hình của California](https://twitter.com/geo_spatialist/status/1251671066164056065?s=20)

Bản đồ dưới đây đã làm thành mô hình cho núi, sa mạc và đồng bằng của California.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042106.jpg)

## Bài đọc thêm

1、[Tại sao buổi standup của phát triển agile không được ưa chuộng？](https://geekbot.com/blog/alternatives-to-standup-meetings/)

Nhiều nhóm sử dụng phát triển agile, thực hiện họp đứng trực tiếp. Mục đích là để mọi người đều hiểu rõ công việc của mình, cung cấp cho nhau cập nhật trạng thái, thúc đẩy hợp tác, nâng cao chất lượng công việc.

Tuy nhiên, standup thường vì kéo dài, làm gián đoạn công việc, không liên quan cao mà gây ra sự không hài lòng của thành viên nhóm.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042301.jpg)

Thứ nhất, nếu standup được tổ chức vào lúc 10 giờ sáng mỗi ngày, đúng là lúc lập trình viên đang tiến hành dự án hoặc giải quyết các công việc tồn đọng. Lúc này để họ nghe ý kiến đồng nghiệp, và thảo luận của product manager, sẽ làm gián đoạn công việc của họ.

Thứ hai, mặc dù standup thường khoảng 15 phút, nhưng đôi khi thời gian rất dài, đặc biệt là nhóm lớn hơn, có thể đạt nửa giờ đến một giờ. Mỗi lập trình viên chỉ có thể phát biểu hai phút, thời gian còn lại không liên quan đến họ.

Cuối cùng, đối với các lập trình viên hướng nội, standup đặc biệt tệ. Chúng không chỉ dài, nhàm chán, mà còn đáng sợ. Không phải ai cũng sẵn sàng nói chuyện trước toàn nhóm, thực ra nhiều lập trình viên không muốn nói chuyện. Không ít lập trình viên thừa nhận, họ thà "ẩn náu trong bóng tối", hy vọng không đến lượt mình phát biểu.

2、[Giai thoại về Chủ tịch Nintendo Hiroshi Yamauchi](https://www.wired.com/2013/10/hiroshi-yamauchi-henk-rogers/)

Tôi chuyển đến Nhật vào cuối những năm 1970. Một ngày năm 1985, vợ tôi đọc một bài báo trên tạp chí Nhật, nói Chủ tịch Nintendo Hiroshi Yamauchi thích chơi cờ vây. Thật trùng hợp, có người tặng cho tôi game cờ vây trên Commodore 64. CPU của Commodore 64 cũng giống như máy game NES của Nintendo, đều là 6502.

Tôi đã gửi fax cho ông Yamauchi, nói tôi có thể phát triển game cờ vây cho máy game NES, tôi vốn không quen biết ông. Hôm sau, tôi đã nhận được trả lời, nói ông Yamauchi sẽ gặp tôi vào ngày mai.

Khi gặp mặt, ông nói: "Tôi không thể cho bạn bất kỳ lập trình viên nào."

Tôi nói: "Tôi không cần lập trình viên, tôi cần tiền."

"Bao nhiêu?"

Tôi nói: "30 triệu yên, khoảng 300.000 đô la." Đây là con số lớn nhất tôi có thể nghĩ ra. Ông bắt tay tôi, chúng tôi đã đạt được thỏa thuận. Tôi sau này mới biết, ông ra quyết định luôn nhanh như vậy, và không bao giờ thay đổi. Những quyết định này luôn là quyết định cuối cùng.

![](https://cdn.beekka.com/blogimg/asset/202002/bg2020020302.jpg)

Sau khi lấy tiền, tôi tìm được tác giả gốc của game cờ vây Commodore 64 ở Anh, thuyết phục anh ta đến Nhật cùng tôi làm dự án này. Chúng tôi thêm vào game một giao diện dễ thương, có một ninja nhỏ di chuyển quân cờ, làm cho người tiêu dùng Nintendo cảm thấy thú vị.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042302.jpg)

Chín tháng sau, tôi cuối cùng đã chuẩn bị xong game. Ông Yamauchi chơi game một lần, hay nói chính xác hơn, ông để cấp dưới điều khiển tay cầm, đặt quân cờ vào vị trí ông chỉ định. Ông chưa bao giờ cầm tay cầm Nintendo.

Ông dễ dàng thắng game, nói game này chưa đủ mạnh cho Nintendo. Nhưng tôi đã làm cho máy game 8-bit của ông có thể chơi cờ vây, đây thực sự là điều kỳ diệu, hoàn toàn thay đổi suy nghĩ của ông.

Cuối cùng tôi hỏi ông, công ty tôi có thể phát hành game này không. "Tôi sẽ nhận được bao nhiêu tiền?" ông nói.

"Mỗi khi tôi bán được một bản, tôi sẽ trả cho ông 100 yên." Ông lại bắt tay tôi, vì vậy tôi trở thành nhà phát triển game của Nintendo.

Sau đó, tôi cùng ông Yamauchi tham gia nhiều cuộc họp. Ban đầu, phòng họp luôn có nhiều người, nhưng sau khi cuộc họp kết thúc, chúng tôi cùng chơi cờ vây, lúc đó chỉ có tôi và ông.

Tôi có thể là người duy nhất trong ngành có cơ hội ở một mình với ông Yamauchi. Tất cả giám đốc cấp cao Nintendo đều coi tôi như quý tộc nước ngoài, tôi được đối xử cao nhất, có thể giao game sau thời hạn.

Tôi còn phát triển 《Tetris》trên máy game NES, sau đó lại chuyển game này sang máy game cầm tay Game Boy. Có người nói Tetris đã tạo nên Game Boy, cũng có người nói Game Boy đã tạo nên Tetris. Tôi cho rằng cả hai đều đúng.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020042303.jpg)

## Danh ngôn & Con số

1、

Tôi tin rằng, chỉ có sáu người đọc hết cuốn sách của tôi 《Principia Mathematica》, sau đó ba người trong số họ bị Hitler giết.

-- [Bertrand Russell](https://www.economist.com/books-and-arts/2020/04/18/listen-to-bertrand-russell-the-english-voltaire), triết học gia người Anh

2、

Vốn hóa thị trường của Apple bằng tổng vốn hóa thị trường của 30 công ty lớn nhất Đức, hoặc tổng vốn hóa thị trường của 200 công ty lớn nhất Australia.

-- [Financial Times](https://www.ft.com/content/6f69433a-40f0-11ea-a047-eae9bd51ceba)

3、

Tôi ban đầu muốn đặt tên cho tác phẩm của mình là 《Phân tích thuật toán》, nhà xuất bản nói: "Điều đó sẽ không bao giờ bán được."

-- [Donald Knuth](https://www.quantamagazine.org/computer-scientist-donald-knuth-cant-stop-telling-stories-20200416/), tác giả 《The Art of Computer Programming》

4、

Một ý tưởng mới giành chiến thắng, không phải vì thuyết phục được những người phản đối nó, mà vì những người phản đối cuối cùng đều chết đi, và thế hệ mới quen thuộc với ý tưởng này lớn lên.

-- [Planck](https://en.wikipedia.org/wiki/Planck%27s_principle), nhà vật lý người Đức

5、

Nếu có ai nói những lời có hại qua điện thoại, bạn sẽ không bắt công ty điện thoại chịu trách nhiệm. Chúng ta cũng nên đối xử với website như vậy.

-- [Zuckerberg](https://www.reuters.com/article/us-germany-security-facebook-idUSKBN2090MA), bàn về cách mọi người nên nhìn nhận Facebook

6、

Người ta thực sự nên ăn ít đường, tôi thậm chí còn thấy có người chấm táo với đường ăn. Chỉ cần vài tuần không ăn đồ ăn vặt hoặc đồ ăn có thêm đường, chanh cũng sẽ trở thành ngọt.

-- [Độc giả HN](https://news.ycombinator.com/item?id=22325739)

## Nhìn lại

- Tuần này năm 2019: [số 53](http://www.ruanyifeng.com/blog/2019/04/weekly-issue-53.html)
- Tuần này năm 2018: [số 1](http://www.ruanyifeng.com/blog/2018/04/weekly-issue-1.html)

## Đăng ký

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97).

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
