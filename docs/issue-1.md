# 每周分享第 1 期 (Bản tin chia sẻ hàng tuần số 1)

Ghi lại những điều thú vị đáng chia sẻ tôi bắt gặp trong tuần qua.

Từ lâu tôi đã luôn cố gắng sắp xếp danh sách yêu thích (bookmarks) của mình bằng nhiều cách khác nhau. Gần đây tôi chợt nghĩ, viết chúng thành một bài viết chia sẻ công khai có lẽ sẽ mang lại hiệu quả tốt hơn.

## 语雀 (Yuque)

Yuque ([yuque.com](https://yuque.com?utm_source=ruanyifeng.com)) là nền tảng tài liệu nội bộ lớn nhất của tập đoàn Alibaba, đồng thời cũng là một trong những công cụ quản lý tri thức và cộng tác nhóm chủ chốt của hệ sinh thái Alibaba.

Hôm nay (23/4) là Ngày Sách Thế giới, [Yuque](https://yuque.com/) đã chọn ngày này để mở cổng đăng ký tự do mà không cần mã mời (invite code) nữa. Người dùng có thể đăng ký trực tiếp và sử dụng mọi tính năng giống như một nhân viên chính thức của Alibaba.

[![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042301.png)](https://yuque.com?utm_source=ruanyifeng.com)

Để hưởng ứng Ngày Sách Thế giới, Yuque cũng mời một số nhân vật nổi tiếng trong ngành Internet viết danh sách sách khuyên đọc của họ, tiêu biểu như CTO của Ant Financial — [Trình Lập](https://yuque.com/book-academy/2018/lusu?utm_source=ruanyifeng.com).

## 新闻 (Tin tức)

1、[Instagram](https://www.macrumors.com/2018/04/04/instagram-disables-third-party-app-apis/) và [Twitter](https://blog.twitter.com/developer/en_us/topics/tools/2017/announcing-more-functionality-to-improve-customer-engagements-on-twitter.html) hạn chế bên thứ ba gọi API

Vào ngày 4/4, Instagram bất ngờ thông báo hủy bỏ ngay lập tức hàng loạt [API](https://www.instagram.com/developer/changelog/), khiến các dữ liệu như follower hay like của người dùng không còn lấy được nữa. Đồng thời họ cũng thông báo giới hạn số lượng yêu cầu API mỗi giờ của mỗi người dùng giảm từ 5000 xuống còn 200. Ngoài ra, họ còn lên kế hoạch từ ngày 11/12/2018 sẽ không cho phép các ứng dụng bên thứ ba truy cập nội dung công khai của mình.

Trước đó không lâu, Twitter cũng thông báo sau ngày 19/6/2018 sẽ ngừng cung cấp dịch vụ streaming services. Điều này đồng nghĩa với việc các client bên thứ ba như Tweetbot, Tweetings, Twitterrific sẽ không thể tự động làm mới dòng thời gian (timeline), người dùng bắt buộc phải tự vuốt làm mới thủ công để xem nội dung mới. Có người đã lập trang web [apps-of-a-feather.com](http://apps-of-a-feather.com/) để kêu gọi Twitter thay đổi quyết định này.

Thông điệp từ các mạng xã hội khổng lồ này đã quá rõ ràng: Chúng tôi không chào đón các client bên thứ ba.

2、[Lập trình viên lương tháng 7 vạn tệ có thể nhập hộ khẩu Bắc Kinh](https://www.zhihu.com/question/269506059)

Ngày 21/3, chính quyền thành phố Bắc Kinh công bố "Một số biện pháp tối ưu hóa dịch vụ nhân tài thúc đẩy đổi mới khoa học công nghệ và phát triển công nghiệp công nghệ cao", trong đó có điều khoản:

> Đối với nhân sự đảm nhận công việc quan trọng tại các chủ thể đổi mới công nghệ như doanh nghiệp công nghệ cao, trụ sở đổi mới sáng tạo, cơ quan nghiên cứu phát triển thế hệ mới thuộc phạm vi hành chính thành phố, có thu nhập chịu thuế hàng năm trong 3 năm gần nhất vượt mức bội số quy định so với lương bình quân của người lao động toàn thành phố năm trước (đối với doanh nghiệp đăng ký tại 6 quận nội thành và Khu phát triển kinh tế kỹ thuật Bắc Kinh là gấp 8 lần, đăng ký tại các khu vực khác của thành phố là gấp 6 lần).

Theo số liệu từ Cục Thống kê và Cục Nhân sinh Xã hội Bắc Kinh, lương năm bình quân của người lao động Bắc Kinh năm 2016 là 92.477 tệ, lương tháng bình quân là 7706 tệ. Trong khi đó, "Báo cáo xu hướng nhân tài mùa cao điểm 2018" của một trang web tuyển dụng lớn chỉ ra mức lương tháng bình quân tại Bắc Kinh đạt 10.712 tệ. Từ đó ước tính lập trình viên cần có mức lương tháng ít nhất 7 vạn tệ (khoảng 10.000 USD) mới đủ điều kiện nộp hồ sơ xin cấp hộ khẩu diện thu hút nhân tài.

3、[Lỗi hy hữu của Travis-CI làm trống sạch cơ sở dữ liệu production](https://blog.travis-ci.com/2018-04-03-incident-post-mortem)

Travis-CI công bố báo cáo điều tra sự cố sập cơ sở dữ liệu production vào ngày 13/3. Một nhà phát triển sau khi thực hiện kiểm tra môi trường production đã chạy kiểm thử (tests) ngay trên cùng một Session. Do địa chỉ cơ sở dữ liệu được cấu hình bằng biến môi trường (environment variables), tại thời điểm đó biến môi trường của địa chỉ database trong Session vẫn đang trỏ đến môi trường production, dẫn đến kết quả là script chạy test đã dọn dẹp trống sạch toàn bộ cơ sở dữ liệu thực tế đang chạy.

4、[Giá nhà ở Thung lũng Silicon tăng 800 USD mỗi ngày làm việc](https://www.bloomberg.com/news/articles/2018-04-09/home-values-are-rising-by-800-a-day-in-san-jose)

Theo thống kê tại San Jose — thành phố lớn nằm gần Thung lũng Silicon nhất, một căn nhà bình thường giá khoảng 1 triệu USD vào năm ngoái đã tăng trung bình 798 USD sau mỗi ngày làm việc, tương đương mức tăng 200.000 USD trong vòng một năm, dẫn đầu nước Mỹ về tốc độ tăng giá nhà. Đứng thứ hai là San Francisco với mức tăng 481 USD mỗi ngày làm việc; đứng thứ ba là Seattle (nơi đặt trụ sở Microsoft) với mức tăng 434 USD.

## 教程 (Hướng dẫn)

1、[Sách điện tử miễn phí] [《Machine Learning Yearning》](http://www.mlyearning.org/), tác giả Andrew Ng (Ngô Ân Đạt)

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042302.png)

Andrew Ng là giáo sư tại Đại học Stanford, một chuyên gia đầu ngành trong lĩnh vực trí tuệ nhân tạo và từng đảm nhận vai trò nhà khoa học trưởng của Baidu.

Cuốn sách mới của ông mang tên *Machine Learning Yearning* hiện đã cho phép [đăng ký nhận miễn phí](http://www.mlyearning.org/). Trong những tháng tới, cứ mỗi khi hoàn thành xong một phần sách mới, ông sẽ gửi email thông báo để bạn có thể đọc ngay lập tức. Theo mô tả, cuốn sách dày khoảng 100 trang với các chương ngắn gọn, cực kỳ dễ đọc. Nội dung tập trung vào cách triển khai dự án machine learning thực tế của riêng bạn, trọng tâm không phải là thuật toán chuyên sâu mà là cách áp dụng thuật toán vào các bài toán thực tế.

2、[Khóa học video miễn phí] [《Foundations of Data Science》](https://data.berkeley.edu/education/data-8x), giảng dạy bởi Đại học California, Berkeley

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042303.png)

Khóa học video [《Foundations of Data Science》](https://data.berkeley.edu/education/data-8x) (Cơ sở Khoa học Dữ liệu) của UC Berkeley hiện đã được đưa lên internet. Đăng ký học hoàn toàn miễn phí, chỉ thu phí nếu bạn có nhu cầu cấp chứng chỉ.

Khóa học được chia làm ba phần, mỗi phần yêu cầu 5 tuần học tập dưới sự giảng dạy trực tiếp từ các giảng viên của UC Berkeley. Toàn bộ chương trình được thiết kế dành cho người mới bắt đầu, không yêu cầu bất kỳ nền tảng kiến thức nào về thống kê hay lập trình.

* Phần 1: [Xử lý dữ liệu bằng Python](https://www.edx.org/course/foundations-data-science-computational-uc-berkeleyx-data8-1x)
* Phần 2: [Suy luận mẫu](https://www.edx.org/course/foundations-data-science-inferential-uc-berkeleyx-data8-2x)
* Phần 3: [Dự đoán và Machine Learning](https://www.edx.org/course/foundations-data-science-prediction-uc-berkeleyx-data8-3x)

3、[Bài viết] [Programming Blockchains Step-by-Step](https://github.com/openblockchains/programming-blockchains-step-by-step), tác giả Gerald Bauer

Hướng dẫn cách sử dụng ngôn ngữ Ruby để xây dựng một blockchain từ con số không, mã nguồn vô cùng dễ hiểu đi kèm giải thích các khái niệm nền tảng.

4、[Bài viết] [Low Level Bit Hacks You Absolutely Must Know](http://www.catonmat.net/blog/low-level-bit-hacks-you-absolutely-must-know/), tác giả Peter Krumins

Tổng hợp các trường hợp ứng dụng thực tế của phép toán bit (bit operation) mà bạn bắt buộc phải biết.

5、[Bài viết] [React - Basic Theoretical Concepts](https://github.com/reactjs/react-basic)

Tài liệu giải thích chính thức từ đội ngũ phát triển về tư tưởng thiết kế nguyên bản của React.

6、[Hình ảnh] [Sơ đồ vòng đời React v16.3 (Lifecycle)](https://github.com/wojtekmaj/react-lifecycle-methods-diagram)

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042304.png)

7、[Sách điện tử] [Cẩm nang tự học phỏng vấn Google](https://github.com/jwasham/coding-interview-university/blob/master/translations/README-cn.md)

Cẩm nang chuẩn bị phỏng vấn kỹ thuật vào Google do một lập trình viên tự tổng hợp.

8、[Bài viết] [Một số mẹo hay khi sử dụng Chrome DevTools](https://flaviocopes.com/chrome-devtools-tips/#drag-and-drop-in-the-elements-panel)

9、[Bài viết] [Color: From Hexcodes to Eyeballs](http://jamie-wong.com/post/color/)

Giải thích cách mắt người cảm nhận màu sắc, bài viết yêu cầu người đọc có một chút kiến thức vật lý nền tảng.

## 文摘 (Văn trích)

1、[Kinh nghiệm đúc rút từ lập trình viên chiến đấu ở tuyến đầu](https://cloud.tencent.com/developer/article/1004735), tác giả Khang Lượng

> Năm 2011, khi làm việc tại đội ngũ phát triển trình duyệt Baidu, tôi đã gặp vài sự kiện vô cùng đáng nhớ. Có lần họp, bên Product đưa ra bản DEMO sản phẩm của Google có hiệu ứng 3D rất bắt mắt và yêu cầu lập trình viên phải làm theo bằng được chỉ trong vòng 2 ngày, khiến ai nấy đều chết lặng. Để kịp tiến độ ép buộc đó, đội phát triển đã tạo ra vô số bug. Để sửa bug, leader đã chia đều số bug theo đầu người, dẫn đến việc các lập trình viên ở các module khác nhau đi sửa code chéo của nhau... Thật khó tin nổi, giống như bắt một đầu bếp chuyên làm bánh bao chay đi điều chỉnh hương vị món cá chép chua ngọt Tây Hồ vậy.
> 
> Hậu quả ban đầu là: Số lượng bug giảm rất chậm, bug phát sinh mới lại tăng lên, mọi người kiệt sức, phong cách viết code trở nên vô cùng hỗn loạn, các giải pháp chắp vá tạm thời xuất hiện tràn lan để kịp deadline.
> 
> Đến giai đoạn giữa: Lập trình viên nghỉ việc hàng loạt, code trở nên bất khả thi để bảo trì, các yêu cầu tính năng mới xung đột chan chát với các đoạn code vá tạm trước đó.
> 
> Đến giai đoạn cuối: Muốn sửa đổi hay tái cấu trúc hệ thống nhưng vẫn phải đảm bảo hệ thống vận hành bình thường, độ khó giống như việc bạn cố gắng tháo lắp sửa chữa các bộ phận của một chiếc máy bay đang bay trên bầu trời vậy.
> 
> Và thế là tôi cũng vội vàng xin nghỉ việc... Thực sự không nhìn thấy bất kỳ cơ hội thành công nào.

2、[Tại sao chúng tôi không sử dụng Git?](https://sqlite.org/whynotgit.html), chia sẻ từ SQLite

> Dự án SQLite không sử dụng hệ thống quản lý phiên bản Git, mà sử dụng Fossil. Cả Fossil và Git đều là hệ thống quản lý phiên bản phân tán dạng chuỗi, lưu trữ nội dung dưới dạng một chuỗi các commit bất biến được xác định bằng mã băm mật mã học. Git cực kỳ phổ biến và nhiều nhà phát triển không quen thuộc với bất kỳ công cụ quản lý phiên bản nào khác. Tuy nhiên, SQLite ưa thích sử dụng Fossil hơn, bài viết này sẽ giải thích lý do tại sao.

3、[Sự thật về các số liệu tại Mỹ](https://mp.weixin.qq.com/s?__biz=MzI2NjA3ODk2MA%3D%3D&from=1084195010&idx=4&mid=2650848195&sn=7399ea1a80effc77cd2f788373b412d4&weiboauthoruid=5493934570&wm=9006_2001)

> Tuổi thọ trung bình của người dân Mỹ đã giảm liên tục trong hai năm qua. Nếu không nói tên quốc gia mà bắt bạn đoán, bạn chắc chắn sẽ nghĩ sự sụt giảm này chỉ xảy ra ở các nước đang có chiến tranh. Đáng tiếc thay, điều này lại đang diễn ra ngay tại Mỹ.
> 
> Vào năm 2016, tỷ lệ hộ gia đình không có tài sản hoặc có tài sản ròng âm đã chạm mốc 30,4%. Nghĩa là chỉ cần bạn có 1 USD tiền tiết kiệm và không mắc nợ ai, dù bạn là người vô gia cư đi nữa, bạn vẫn giàu có hơn 30% số hộ gia đình tại Mỹ.
> 
> Người Mỹ thực tế nghèo đến mức nào? 69% người Mỹ có số tiền tiết kiệm ít hơn 1000 USD. Nhiều người nói người Mỹ rất giàu, điều đó đúng nếu bạn có công việc tốt với thu nhập rất cao. Nhưng thực tế phần lớn người Mỹ khá nghèo, sống phụ thuộc nhiều vào các khoản trợ cấp và phúc lợi xã hội. Một nửa số người Mỹ có thu nhập bình quân năm dưới 25.000 USD. Thu nhập bình quân của Mỹ là hơn 40.000 USD nhưng mức thu nhập trung vị (median) chỉ có 25.000 USD. Thu nhập trung vị nghĩa là 50% số dân có thu nhập cao hơn con số này, và 50% có thu nhập thấp hơn.

4、[Thời báo Hoàn Cầu: Phát triển chip nội địa — Việc này không thể trì hoãn thêm nữa](http://finance.sina.com.cn/stock/y/2018-04-18/doc-ifzfkmth6405788.shtml)

> Kể từ bây giờ, ảo tưởng rằng chúng ta có thể sống tốt dựa vào nguồn chip nhập khẩu từ Mỹ nên được dập tắt hoàn toàn. Chúng ta có năng lực nghiên cứu phát triển khoa học công nghệ quốc gia và có sức mạnh huy động cần thiết để dần thay thế chip ngoại bằng chip nội địa, thứ quan trọng nhất chính là quyết tâm.
> 
> Chính quyền Trump đang giúp chúng ta củng cố quyết tâm này. Nếu chúng ta thực sự thay đổi tư duy, có lẽ nhiều năm sau nhìn lại, chúng ta sẽ phải cảm ơn quyết định hạn chế của Mỹ ngày hôm nay vì đã giúp chúng ta sớm tỉnh ngộ.

## 工具 (Công cụ)

1、[Spectrum](https://github.com/withspectrum/spectrum)

Phần mềm diễn đàn/cộng đồng nguồn mở với thiết kế giao diện hiện đại và đẹp mắt.

2、[jsonstore.io](https://github.com/bluzi/jsonstore)

Dịch vụ lưu trữ dữ liệu JSON miễn phí hỗ trợ đọc viết qua HTTP Header.

3、[flamebearer](https://github.com/mapbox/flamebearer)

Công cụ hỗ trợ tạo biểu đồ ngọn lửa (flame graph) cho các ứng dụng Node.js để phân tích hiệu năng.

4、[DNS Performance Test](https://github.com/cleanbrowsing/dnsperftest)

Script dòng lệnh giúp kiểm tra và so sánh tốc độ phản hồi của các DNS server khác nhau.

5、[merge-images](https://github.com/lukechilds/merge-images)

Thư viện JavaScript chạy ở trình duyệt hỗ trợ ghép nhiều hình ảnh thành một hình ảnh duy nhất thông qua Canvas.

6、[Tabler](https://github.com/tabler/tabler)

Bộ UI component thiết kế dashboard giao diện quản trị dựa trên Bootstrap 4.

7、[Etherpad](http://etherpad.org/)

Công cụ cộng tác và biên tập tài liệu thời gian thực hỗ trợ nhiều người viết cùng lúc nổi tiếng.

## 新奇 (Sự độc đáo)

1、[Braille Neue](http://brailleneue.com/)

[![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042305.jpg)](http://brailleneue.com/)

[![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042306.png)](http://brailleneue.com/)

Braille Neue là sự kết hợp hoàn hảo giữa hệ thống chữ nổi Braille cho người khiếm thị và các ký tự chữ cái alphabet thông thường. Đây là một hình mẫu xuất sắc cho thiết kế无 chướng ngại (accessibility), thật khó hiểu tại sao trước đây chưa từng có ai nghĩ ra ý tưởng này.

2、[Biến màn hình MacBook thành cảm ứng chỉ với 1 USD](https://github.com/bijection/sistine)

[![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042307.jpg)](https://github.com/bijection/sistine)

Dự án phần cứng sáng tạo cực chất: Tác giả lắp một mảnh gương nhỏ đặt chéo phía trước webcam của MacBook để phản chiếu hình ảnh ngón tay chạm màn hình, sau đó dùng thuật toán xử lý ảnh tự động nhận diện và tính toán tọa độ chạm của ngón tay.

3、[Jelly Mario Bros](http://jellymar.io/)

[![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042308.png)](http://jellymar.io/)

Phiên bản game Mario chạy trên web phong cách "sứa biển", trong đó mọi nhân vật, vật phẩm và gạch đá đều mềm nhũn và co giãn biến dạng khi va chạm.

__4、Mẫu USB hình chú chó độc đáo__

[![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042309.jpg)](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042309.jpg)

[![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042310.jpg)](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042310.jpg)

## 本周金句 (Kim ngôn tuần này)

Cuộc đời giống như chú ruồi đậu trên cửa kính: Tương lai trước mắt tràn đầy ánh sáng, nhưng lại loay hoay không tìm thấy lối ra.

## 欢迎订阅 (Chào mừng đăng ký theo dõi)

Chuyên mục này sẽ được cập nhật đồng thời trên [trang web cá nhân](http://www.ruanyifeng.com/blog), [kênh WeChat](http://weixin.sogou.com/weixin?type=1&query=阮一峰的网络日志) và tài khoản [Yuque](https://yuque.com/ruanyf/share/) của tôi.

(Hết)
