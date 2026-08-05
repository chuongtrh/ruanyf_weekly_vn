# 每周分享第 5 期 (Bản tin chia sẻ hàng tuần số 5)

Ghi lại những điều thú vị đáng chia sẻ tôi bắt gặp trong tuần qua, phát hành vào thứ Sáu hàng tuần.

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051801.jpg)

(Ảnh bìa: Công viên World Expo, Thượng Hải, 2018)

Tuần này, máy chủ của tôi bị tấn công DDoS khiến trang web bị sập liên tục suốt hơn 50 tiếng đồng hồ. Đã có lúc tôi nghĩ rằng số *Chia sẻ hàng tuần* này không thể phát hành đúng hẹn. Hiện tại cuộc tấn công đã tạm dừng, nhưng không ai biết khi nào nó sẽ quay trở lại. Tôi sẽ viết chi tiết về sự việc này trong một bài viết riêng sau, ở đây tôi chỉ muốn chia sẻ một vài cảm nhận cá nhân.

Ngay khi tin tức trang web bị sập lan truyền, rất nhiều người bạn chưa từng quen biết đã hỏi thăm và ngỏ ý hỗ trợ tài nguyên cá nhân hoặc hạ tầng công ty để giúp tôi vượt qua giai đoạn khó khăn. Cả Alibaba Cloud và Tencent Cloud đều gửi tặng tôi các gói dịch vụ IP chống DDoS cao cấp. Tôi xin trân trọng ghi nhớ sâu sắc mọi sự giúp đỡ này. Ngay cả trong thời điểm cuộc tấn công diễn ra dồn dập nhất, tôi chưa từng cảm thấy lo lắng, bởi tôi biết phía sau mình luôn có sự ủng hộ của rất nhiều người, các cuộc tấn công sẽ không thể đánh gục được tôi mà chỉ càng kích thích thêm ý chí chiến đấu của tôi mà thôi.

Trải nghiệm lớn nhất của tôi qua sự cố này là: Việc sống tử tế trên Internet thực sự là một điều "hời" nhất. Ngày thường, việc bạn làm chẳng qua chỉ là viết các bài hướng dẫn chia sẻ trên mạng, trả lời một số email thắc mắc kỹ thuật của người dùng, thực chất không phải là sự hy sinh gì quá to lớn. Nhưng nhờ khả năng lan tỏa của Internet, những việc làm tử tế nhỏ bé đó đều được mọi người ghi nhận và nhớ tới. Để rồi khi bạn gặp khó khăn, mọi người sẽ đồng loạt xuất hiện từ khắp nơi để hỗ trợ và âm thầm tiếp sức cho bạn.

Ngược lại, nếu bạn chọn làm kẻ xấu, ẩn nấp trong bóng tối để thực hiện các hành vi phá hoại tư lợi, có thể bạn sẽ đạt được mục đích ích kỷ trước mắt nhưng bạn sẽ không bao giờ có thể tin tưởng bất kỳ ai và luôn phải sống trong trạng thái lo âu sợ hãi vì người khác cũng có thể dùng chiêu trò tương tự để nhắm vào bạn. Đến lúc bạn gặp nạn, thay vì có người giúp đỡ, họ sẽ chỉ hả hê ăn mừng mà thôi. Tôi nghĩ cuộc đời như vậy thật đáng buồn và đáng thương.

## 新闻 (Tin tức)

1、[Firefox 60 hỗ trợ cơ chế bảo mật Cookie SameSite chống tấn công CSRF](https://blog.mozilla.org/security/2018/04/24/same-site-cookies-in-firefox-60/)

Phiên bản Firefox 60 vừa phát hành đầu tháng này tích hợp một tính năng bảo mật rất quan trọng giúp giải quyết triệt để phương thức tấn công CSRF.

Tấn công CSRF (Cross-Site Request Forgery) là hình thức lợi dụng các tệp tin Cookie hợp lệ của người dùng để thực hiện các hành vi độc hại. Ví dụ, khi người dùng truy cập trang web B độc hại có chứa một thẻ hình ảnh trỏ về trang web A, trình duyệt của người dùng sẽ tự động gửi yêu cầu lấy ảnh tới trang web A kèm theo toàn bộ Cookie của trang web A đang lưu trên máy. Nếu đường dẫn hình ảnh đó được kẻ xấu thiết kế tinh vi (ví dụ lệnh yêu cầu chuyển tiền), máy chủ của trang web A sẽ hiểu nhầm đây là yêu cầu hợp lệ của người dùng do Cookie gửi kèm hoàn toàn chính xác, từ đó tự động thực hiện các thao tác chuyển tiền nguy hiểm.

Theo tiêu chuẩn mới, Firefox 60 bổ sung thuộc tính `SameSite` cho Cookie, quy định rõ ràng rằng khi người dùng truy cập trang web B, mọi yêu cầu ngầm trỏ về trang web A sẽ tuyệt đối không được mang theo Cookie của trang web A nữa, giúp ngăn chặn triệt để nguy cơ tấn công CSRF từ gốc rễ. Ngoài ra, Firefox 60 cũng chính thức kích hoạt mặc định tính năng hỗ trợ ES6 module.

2、[Sàn giao dịch Binance đạt lợi nhuận vượt ngân hàng Deutsche Bank dù mới thành lập 8 tháng](http://finance.sina.com.cn/blockchain/coin/2018-04-28/doc-ifztkpip2834593.shtml)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051802.png)

Binance công bố lợi nhuận quý trước của sàn giao dịch đạt mốc 200 triệu USD, chính thức vượt qua Deutsche Bank — ngân hàng lớn nhất nước Đức có lợi nhuận quý I/2018 đạt 146 triệu USD.

Deutsche Bank sở hữu lịch sử phát triển 148 năm với quy mô hơn 100.000 nhân viên. Trong khi đó, cách đây hơn 8 tháng, Binance thậm chí còn chưa tồn tại. Sàn giao dịch tiền mã hóa Binance do CEO Triệu Trường Bằng (CZ) sáng lập hiện đã vươn lên trở thành sàn giao dịch tiền mã hóa lớn nhất thế giới về khối lượng giao dịch.

3、[Mối lo ngại khi các tổ chức CA tự ý thu hồi chứng chỉ HTTPS](https://scotthelme.co.uk/the-power-to-revoke-lies-with-the-ca/)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051803.jpg)

Mọi trang web mã hóa an toàn đều cần chứng chỉ bảo mật HTTPS do các tổ chức CA (Certificate Authority) cấp phát. Mới đây, một tổ chức CA đã tự ý thu hồi chứng chỉ bảo mật của trang web hoạt động hoàn toàn hợp pháp `stripe.ian.sh` với lý do duy nhất: Tên miền này hiển thị chứng chỉ dễ gây nhầm lẫn với trang chủ của hãng thanh toán Stripe (`stripe.com`).

Biểu đồ so sánh ở trên cho thấy tên miền của tác giả dễ khiến người dùng nhầm lẫn rằng họ đang truy cập trang chủ chính thức của Stripe. Sự việc đặt ra dấu hỏi lớn về việc quyền lực của các tổ chức CA hiện nay có đang quá lớn hay không khi họ có quyền đơn phương đình chỉ hoạt động của một website thương mại chỉ bằng một lệnh thu hồi chứng chỉ bảo mật. Trước đó, trang web chia sẻ tài liệu học thuật Sci-Hub cũng đã bị các tổ chức CA đồng loạt thu hồi chứng chỉ HTTPS do tranh chấp bản quyền.

4、[Robot chó cưng thông minh Sony Aibo](https://aibo.sony.jp/en/)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051804.jpg)

Sony giới thiệu dòng robot chó cưng thế hệ mới **aibo**. Với các cảm biến thông minh và AI tích hợp, robot aibo có khả năng tương tác tự nhiên và biểu cảm sinh động cực kỳ giống với một chú chó thật, mở ra kỷ nguyên robot làm bạn đồng hành cùng con người trong gia đình.

5、[Notepad của Microsoft hỗ trợ định dạng xuống dòng của Unix](https://blogs.msdn.microsoft.com/commandline/2018/05/08/extended-eol-in-notepad/)

Ký tự xuống dòng của tệp tin văn bản (text file) từ lâu đã không đồng nhất giữa các hệ điều hành: Hệ thống Unix sử dụng ký tự `\n` (LF), còn Windows sử dụng cặp ký tự `\r\n` (CRLF). Hậu quả là khi dùng phần mềm Notepad của Windows để mở các file văn bản soạn thảo từ Unix, toàn bộ nội dung file sẽ bị hiển thị dồn trên một dòng duy nhất vô cùng khó đọc.

Microsoft rốt cuộc đã công bố bản cập nhật Windows 10 tiếp theo cho phần mềm Notepad hỗ trợ hiển thị chính xác định dạng xuống dòng của Unix (LF) và macOS (CR).

6、[Tính năng Smart Compose hỗ trợ viết email thông minh trên Gmail](https://www.businessinsider.sg/google-gmail-gets-smart-compose-automatic-reply-suggestion-service-2018-5/)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051805.jpg)

Tại hội nghị Google I/O, hãng giới thiệu tính năng Smart Compose cho Gmail. Dựa trên công nghệ AI học máy, khi người dùng gõ một vài từ đầu tiên, hệ thống sẽ tự động dự đoán và hiển thị câu hoàn chỉnh gợi ý tiếp theo giúp đẩy nhanh tốc độ soạn thảo email công việc.

7、[Dịch vụ lưu trữ đám mây Google One](https://one.google.com/getupdates)

![](https://cdn.beekka.com/blogimg/asset/2018/bg2018051806.png)

Google nâng cấp dịch vụ lưu trữ đám mây Drive thành thương hiệu Google One với các gói cước mới cạnh tranh: Gói 100GB giá 2 USD/tháng, 200GB giá 3 USD/tháng và 2TB giá 10 USD/tháng. Động thái giảm giá sâu này hứa hẹn gây áp lực rất lớn lên đối thủ Dropbox (vốn đang duy trì gói 1TB giá 10 USD/tháng). Tuy nhiên mức dung lượng này vẫn chưa thể so sánh với dịch vụ Baidu Cloud của Trung Quốc (tặng miễn phí 2TB dung lượng lưu trữ cho người dùng mới).

## 教程 (Hướng dẫn)

1、[Bài viết] [Trực quan hóa mô hình Xích Markov đơn giản nhất](http://setosa.io/ev/markov-chains/) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051809.png)

Bài viết trực quan hóa Xích Markov (Markov Chain) gồm hai trạng thái A và B với 4 đường chuyển đổi trạng thái: A -> A, A -> B, B -> A, B -> B. Khi xác suất xảy ra của mỗi đường chuyển đổi là 50%, hệ thống sẽ sinh ra một quỹ đạo di chuyển ngẫu nhiên. Một ví dụ thực tế là mô phỏng thời tiết hàng ngày dạng "nắng" và "mưa" với xác suất chuyển đổi 50% để dự báo xu hướng thời tiết tuần tới.

2、[Bài viết] [Nhập môn mô hình học máy Cây quyết định](https://heartbeat.fritz.ai/introduction-to-decision-tree-learning-cd604f85e236) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051810.jpg)

Mô hình Cây quyết định (Decision Tree) là một trong những mô hình học máy cơ bản, trực quan và dễ hiểu nhất để hỗ trợ ra quyết định khi chịu ảnh hưởng bởi nhiều tham số đầu vào khác nhau.

3、[Bài viết] [Tại sao câu lệnh "go" trong lập trình đồng thời có thể gây hại?](https://vorpus.org/blog/notes-on-structured-concurrency-or-go-statement-considered-harmful/) (Tiếng Anh)

Phân tích về lập trình đa luồng, tác giả lập luận việc sử dụng câu lệnh `go` tự do để tách một luồng con chạy độc lập ngoài luồng chính rồi trả kết quả về có thể gây mất kiểm soát luồng hoạt động của chương trình và khiến mã nguồn dự án nhanh chóng trở nên hỗn loạn.

4、[Mã nguồn] [Xây dựng Kanban App bằng ngôn ngữ Elm và Rust](https://github.com/huytd/kanban-app) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051812.jpg)

Thông thường khi lập trình ứng dụng desktop bằng công nghệ web, lập trình viên hay dùng Electron. Nhược điểm lớn nhất của Electron là bắt buộc phải đóng gói kèm theo toàn bộ nhân trình duyệt Chromium và engine V8 khiến dung lượng ứng dụng tối thiểu lên tới hàng chục MB dù tính năng rất đơn giản. Dự án giới thiệu một phương pháp tiếp cận mới gọn nhẹ hơn: Sử dụng chính thành phần WebView có sẵn của hệ điều hành kết hợp với lớp bọc bằng Rust để chạy phần giao diện web viết bằng Elm, giúp ứng dụng desktop có dung lượng siêu nhẹ chỉ vài trăm KB và tiêu tốn cực ít tài nguyên RAM.

5、[Bài viết] [Kinh nghiệm triển khai hệ thống có độ sẵn sàng cao (High Availability)](https://medium.com/@NetflixTechBlog/tips-for-high-availability-be0472f2599c) (Tiếng Anh)

Đội ngũ kỹ sư Netflix chia sẻ các phương pháp triển khai mã nguồn (deployment) giúp nâng cao độ sẵn sàng của hệ thống dịch vụ, ví dụ như mô hình triển khai Red-Black deployment, thiết lập cửa sổ triển khai an toàn...

6、[Tài liệu] [Tập hợp bài giảng khóa học CS109: Cơ sở Khoa học Dữ liệu của Đại học Harvard](http://cs109.github.io/2015/index.html) (Tiếng Anh)

Giáo trình giảng dạy nhập môn Khoa học Dữ liệu bằng ngôn ngữ Python, các mô hình toán học và lý thuyết thống kê cơ bản đi kèm các video bài giảng và slide tải về miễn phí.

7、[Tài liệu] [Tổng hợp kiến thức nền tảng phục vụ phỏng vấn kỹ thuật](https://github.com/CyC2018/Interview-Notebook) (Tiếng Trung)

Kho tài liệu tổng hợp đầy đủ các kiến thức khoa học máy tính cốt lõi thường xuất hiện trong các buổi phỏng vấn tuyển dụng.

## 工具 (Công cụ)

1、[sonarwhal](https://sonarwhal.com)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051813.jpg)

Công cụ quét lint trang web nguồn mở do Microsoft phát hành giúp phân tích chi tiết website trên 5 tiêu chí: khả năng tiếp cận (accessibility), hiệu năng, bảo mật, PWA và tính tương thích thiết bị để đưa ra các gợi ý tối ưu.

2、[IPBlade](https://chrome.google.com/webstore/detail/ipblade-privacy-protector/hojjgiebfmgmlpjojjkaehgohkolmoea)

Tiện ích mở rộng Chrome hỗ trợ thay đổi nhanh IP của trình duyệt sang các quốc gia khác để truy cập các dịch vụ bị giới hạn vị trí địa lý.

3、[add-gitignore](https://github.com/TejasQ/add-gitignore)

Công cụ dòng lệnh hỗ trợ tự động tạo tệp tin cấu hình `.gitignore` chuẩn hóa dựa trên các tùy chọn công nghệ của dự án.

4、[jGoBoard](http://jgoboard.com/)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051816.jpg)

Thư viện JavaScript hỗ trợ vẽ và tương tác bàn cờ vây trực quan trên web. Một công cụ tương tự là bàn cờ vây của AlphaGo dựa trên thư viện WGO.js.

5、[Pyre](https://github.com/facebook/pyre-check)

Công cụ kiểm tra kiểu dữ liệu tĩnh (static type checker) cho ngôn ngữ Python do Facebook phát triển, đóng vai trò tương tự như Flow đối với JavaScript.

## 文摘 (Văn trích)

1、[AI sẽ chấm dứt chủ nghĩa tư bản](https://www.washingtonpost.com/news/theworldpost/wp/2018/05/03/end-of-capitalism/?utm_term=.0b7dc0245ff0)

> GS. Phùng Tượng thuộc Đại học Thanh Hoa nhận định: Sự phát triển vượt bậc của AI sẽ dần tập trung toàn bộ của cải xã hội được tạo ra từ tự động hóa vào tay một nhóm nhỏ các tỷ phú công nghệ sở hữu robot, dẫn tới tình trạng thất nghiệp diện rộng của người lao động. Sự thất nghiệp hàng loạt bắt buộc nhà nước phải can thiệp để quốc hữu hóa tài nguyên AI và thiết lập các phúc lợi xã hội toàn dân, từ đó dẫn tới sự kết thúc của mô hình kinh tế thị trường tự do.

2、[Tỷ lệ người làm việc đúng ngành sau 20 năm tốt nghiệp](https://improvingsoftware.com/2009/05/19/programmers-before-you-turn-40-get-a-plan-b/)

> Số liệu khảo sát của Cục Thống kê Dân số Mỹ chỉ ra: Sau 10 năm tốt nghiệp đại học ngành khoa học máy tính, 57% sinh viên vẫn đang làm lập trình viên; sau 15 năm tỷ lệ này giảm xuống 34%; và sau 20 năm tốt nghiệp (tầm tuổi hơn 40) tỷ lệ người còn theo nghề lập trình viên chỉ còn vỏn vẹn 19%. Để so sánh, tỷ lệ này ở ngành kỹ sư xây dựng lần lượt là 61%, 52% và 52%. Thực trạng thiếu vắng lập trình viên ngoài 40 tuổi là vấn đề chung của ngành công nghiệp phần mềm trên toàn cầu.

3、[Triết lý lập trình từ dưới lên (Bottom-up Programming)](http://www.paulgraham.com/progbot.html), tác giả Paul Graham

> Khác với phương pháp thiết kế từ trên xuống (top-down) truyền thống chia nhỏ một chương trình lớn thành các khối chức năng con độc lập, các lập trình viên Lisp thường ưa chuộng phương pháp lập trình từ dưới lên: Thay đổi chính ngôn ngữ lập trình để thích ứng và giải quyết bài toán. Bạn xây dựng thêm các toán tử và hàm trừu tượng mới bổ sung vào ngôn ngữ gốc để phục vụ việc giải quyết bài toán, giúp chương trình cuối cùng có cấu trúc gọn gàng và mức độ trừu tượng hóa cao hơn.

4、[Lượng sao trên bầu trời đêm](http://www.skyandtelescope.com/astronomy-resources/how-many-stars-night-sky-09172014/)

> Ở các điều kiện lý tưởng tối nhất trên Trái Đất, mắt người có thể nhìn thấy khoảng 9.096 ngôi sao có độ sáng đạt chuẩn mắt thường nhìn thấy. Do tại một thời điểm chúng ta chỉ quan sát được một nửa bán cầu bầu trời, số lượng sao tối đa nhìn thấy được ở bầu trời đêm nguyên sơ nhất là khoảng 4.548 ngôi sao. Ở các vùng ngoại ô thành phố lớn bị ảnh hưởng bởi ô nhiễm ánh sáng, số lượng sao giảm xuống chỉ còn khoảng 900 ngôi sao; và ở trung tâm các thành phố lớn bị ô nhiễm ánh sáng nặng nề, con số này sụt giảm nghiêm trọng chỉ còn khoảng 35 ngôi sao nhìn thấy được.

## 本周图片 (Hình ảnh tuần này)

1、[Bãi nghĩa địa xe đạp chia sẻ khổng lồ tại Trung Quốc](https://www.theatlantic.com/photo/2018/03/bike-share-oversupply-in-china-huge-piles-of-abandoned-and-broken-bicycles/556268/?single_page=true)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051820.jpg)

Sự bùng nổ của mô hình xe đạp chia sẻ thực chất là các hãng đang chuyển dịch chi phí bến bãi đỗ xe sang không gian công cộng của đô thị. Các bãi tập kết xe đạp bị bỏ hoang chất cao như núi đang trở thành vấn đề nan giải của quản lý đô thị.

2、[Google sửa lỗi hiển thị Emoji trên Android](https://www.businessinsider.sg/google-ceo-apologizes-for-android-burger-emoji-shows-off-new-beer-design-2018-5/?r=US&IR=T)

![](https://cdn.beekka.com/blogimg/asset/201805/bg2018051821.jpg)

Google đã cập nhật và sửa lại thiết kế của hai hình vẽ Emoji bị sai sót trên Android: Sắp xếp lại lớp phô mai đặt phía trên miếng thịt của bánh hamburger (trước đây vẽ nằm dưới cùng sát lát bánh mì) và sửa lại ly bia vơi một nửa không còn bọt bia tràn ra ngoài thành ly phi vật lý.

## 本周金句 (Kim ngôn tuần này)

1、

> "Độ lớn của các hàm chức năng trong code không nên thiết kế quá đồ sộ. Một hàm quá dài dễ che giấu các lỗi logic bên trong, giống như một thành phố quá lớn dễ ẩn náu các tội phạm truy nã vậy."
> 
> -- Paul Graham

2、

> "Thứ các kỹ sư phần mềm, phần cứng hay máy tính hiện nay phải đối mặt là chu kỳ bán rã kiến thức (half-life of knowledge) cực kỳ ngắn ngủi chỉ trong vòng vài năm."
> 
> -- Craig Barrett, đồng sáng lập Intel.

(Hết)
