# 科技爱好者周刊：第 102 期 (Bản tin chia sẻ công nghệ số 102)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/1148) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## Ảnh bìa

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040505.jpg)

Ngày 26 tháng 3, nhà máy Dongfeng Nissan tại Vũ Hán phục hồi hoạt động, nhân viên ăn trưa giữ khoảng cách. (AFP)

## Quan điểm tuần này: Niềm đam mê công việc đến từ đâu？

BBC [đưa tin](https://www.bbc.com/worklife/article/20200306-the-surprising-truth-about-finding-your-passion-at-work), một nhà tâm lý học Singapore đã phát minh ra "Thang đo nhiệt tình công việc", có thể đo mức độ đam mê của một người với công việc của mình.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040812.jpg)

Niềm đam mê công việc rất quan trọng, **nếu không có đam mê, làm gì cũng không thể xuất sắc.** Trump đã từng nói: "Không có đam mê, bạn không có năng lượng. Không có năng lượng, bạn không có gì cả."

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040813.jpg)

Niềm đam mê công việc có nhiều nguồn gốc: thu nhập kinh tế, triển vọng nghề nghiệp, danh dự xã hội... Nghe nói, "Thang đo nhiệt tình công việc" có thể đo lường những nhân tố kích thích này, ảnh hưởng của chúng đến bạn lớn đến đâu.

Tôi có một phương pháp đơn giản, hoàn toàn không cần bất kỳ bài kiểm tra tâm lý nào, đã biết bạn đam mê nhất với điều gì.

**Bạn chỉ cần tự hỏi một câu: Công việc mà dù không có thù lao bạn vẫn sẽ làm là gì?** Nếu một công việc hoàn toàn không có thù lao, bạn vẫn sẵn sàng làm, đó là điều bạn thích nhất, có đam mê nhất, nhất định phải trân trọng.

Khi JK Rowling viết tập đầu tiên của "Harry Potter", hoàn toàn không biết có được xuất bản không, bà chỉ là có xung lực viết, mỗi ngày đến góc quán cà phê viết đến tối. Richard Stallman là tác giả của GCC và Emacs, viết xong thì mã nguồn mở, tất cả mọi người đều có thể dùng miễn phí, mặc dù lúc đó ông còn không có chỗ ở, chỉ có thể ngủ trong văn phòng.

Niềm đam mê công việc của họ cao đến mức không cần kích thích tiền bạc nữa. Tôi chỉ là muốn làm, mặc kệ có thù lao hay không. **Những gì chúng ta muốn chính là trạng thái làm việc như vậy, đam mê không đến từ sự kích thích bên ngoài, mà đến từ nhu cầu tự hiện thực hóa bản thân từ bên trong, điều này mạnh mẽ hơn kích thích bên ngoài nhiều.** Nhiều tác phẩm xuất sắc nhất được tạo ra như vậy.

Nếu bạn có công việc như vậy, dù không được một xu, vẫn có xung lực mạnh mẽ để làm. Thì xin chúc mừng, bạn đã tìm thấy điều mình đam mê nhất. Bạn hoàn toàn không cần "Thang đo nhiệt tình công việc", giá trị nhiệt tình được đo bởi bảng đó, so với sự theo đuổi trong lòng chúng ta, không đáng kể gì cả. Trong lĩnh vực bạn đam mê nhất, khả năng bạn tạo ra thành quả xuất sắc, sẽ lớn hơn nhiều so với những lĩnh vực cần thang đo.

Trong lòng mỗi người đều có một ngọn lửa, đừng để nó tắt, hãy tìm thấy nó và thắp sáng nó.

## Video miễn phí về Webpack

Tài liệu khóa học tuần này là 《Hiểu sâu về Webpack》 từ "Kaikeba".

Thư viện Webpack, hầu hết các dự án front-end lớn hiện nay đều sử dụng, cả React và Vue đều cần nó để đóng gói module. Không chỉ dự án front-end, còn có mini program, React Native, Electron cũng dùng đến nó.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040905.jpg)

Tôi nghĩ hầu hết mọi người đã dùng Webpack, hoặc scaffold tool của bạn đã tích hợp sẵn. Nhưng, rất ít người chịu tìm hiểu kỹ nó, chỉ thao tác theo tài liệu, dù sao cấu hình của nó cũng khá nhiều, cũng không dễ hiểu. Hậu quả của điều này là, gặp lỗi đóng gói thì bó tay, không biết cách khắc phục. Nói đến nâng cao hiệu năng lại càng không biết bắt đầu từ đâu.

Video miễn phí dưới đây sẽ trước tiên giảng giải quy trình đóng gói của Webpack, cùng kiến thức cơ bản về AST (Cây cú pháp trừu tượng), phân tích biểu đồ phụ thuộc giữa các module, cuối cùng lại dẫn mọi người tự tay triển khai một Webpack đơn giản.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040906.jpg)

> Các tài liệu video trên được cung cấp độc quyền bởi **Kaikeba**.
>
> Kaikeba là thương hiệu giáo dục nghề mới cho người internet đầu tiên trong ngành tập hợp tài nguyên từ các công ty IT lớn như Baidu, DiDi, Alibaba, Microsoft, đưa các dự án thực chiến tiền tuyến trong lĩnh vực công nghệ internet vào nội dung giảng dạy, giúp học viên nâng cao năng lực và kết nối liền mạch với nhu cầu tuyển dụng của các công ty lớn.

## Tin tức

1、[Lễ tốt nghiệp từ xa](https://www.sohu.com/a/385137145_161795)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040803.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040804.jpg)

Trong thời dịch bệnh, Trường Kinh doanh Doanh nhân ở Tokyo, Nhật Bản tổ chức lễ tốt nghiệp từ xa tại một khách sạn. Học sinh không đến hiện trường, mà điều khiển robot tại nhà. "Khuôn mặt" của robot là máy tính bảng, hiển thị khuôn mặt sinh viên tốt nghiệp theo thời gian thực qua camera.

Người dẫn chương trình thông báo bắt đầu nhận bằng tốt nghiệp, học sinh điều khiển robot từ xa "đi" về phía bục chủ tịch, nhận bằng tốt nghiệp từ tay Hiệu trưởng Kenichi Ohmae, nhân viên vỗ tay nói: "Chúc mừng!". Hiệu trưởng đặt bằng vào tay robot, sau đó chụp ảnh lưu niệm.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040801.jpg)

2、[Tuổi chính xác của cá mập voi](https://www.bbc.com/news/science-environment-52155008)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040602.jpg)

Cá mập voi là loài cá mập lớn nhất trên Trái đất, dài khoảng 18m, trọng lượng trung bình khoảng 20 tấn, có đốm trắng dễ nhận biết trên mình. Các nhà khoa học Úc gần đây tìm ra một phương pháp đo tuổi chính xác của cá mập voi.

Bắt đầu từ cuối những năm 1940, Mỹ, Liên Xô và các nước khác tiến hành nhiều vụ thử bom nguyên tử. Một tác dụng phụ của những vụ nổ hạt nhân này là làm cho hàm lượng đồng vị carbon-14 trong khí quyển tăng gấp đôi. Tất cả sinh vật trên Trái đất đều hấp thụ carbon-14 này qua không khí. Do có chu kỳ bán rã, đồng vị này sẽ giảm theo thời gian, vì vậy sinh vật càng già, carbon-14 tìm thấy trong cơ thể càng ít.

Các nhà khoa học phân tích mẫu đốt sống của cá mập voi đã chết, phát hiện loài động vật này có tuổi thọ rất dài, có thể lên đến 100-150 tuổi.

3、[Tìm kiếm lập trình viên COBOL](https://www.northjersey.com/story/news/new-jersey/2020/04/04/coronavirus-nj-40-year-old-system-adds-delay-unemployment-checks/2944985001/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040514.jpg)

Thống đốc bang New York công khai tìm kiếm lập trình viên COBOL trên truyền hình. Hệ thống bảo hiểm thất nghiệp của bang này được phát triển bằng COBOL, đã có lịch sử hơn 40 năm. Gần đây, số người thất nghiệp ở Mỹ tăng mạnh (hơn 7 triệu người), hệ thống này không chịu được tải, phản hồi cực chậm, mỗi thao tác phải chờ rất lâu, khiến người ta lo lắng nó có thể sụp đổ bất cứ lúc nào.

Ngôn ngữ COBOL ra đời vào những năm 1970, lúc đó có nhiều tổ chức tài chính và cơ quan chính phủ sử dụng ngôn ngữ này, phát triển nhiều hệ thống quan trọng. Sau đó, COBOL dần suy tàn, lập trình viên hiểu nó ngày càng ít. Nhưng các hệ thống dựa trên nó, do rủi ro và chi phí, vẫn đang hoạt động đến ngày nay, chưa bao giờ được nâng cấp.

4、[Sinh vật sống do con người thiết kế](https://www.nytimes.com/2020/04/03/science/xenobots-robots-frogs-xenopus.html)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040507.jpg)

Các nhà khoa học Mỹ chiết xuất tế bào từ phôi ếch (hình trên), sau đó dựa trên kết quả từ mô hình máy tính, kết hợp những tế bào này lại với nhau, tạo ra loại "sinh vật có thể lập trình" đầu tiên trên thế giới (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040508.jpg)

Những dạng sống này không có cơ quan sinh dục, không có dạ dày, não hay hệ thần kinh, chỉ là một sinh vật được tạo thành từ khoảng 2000 tế bào sống. Các nhà khoa học tập hợp chúng lại thành sinh vật sống. Dựa theo tên của ếch vuốt châu Phi Xenopus laevis, chúng được đặt tên là Xenobots, tức robot tế bào ếch. Những sinh vật này ăn lòng đỏ trứng, chỉ có thể sống khoảng một tuần.

5、[Sự phân hóa giàu nghèo trong cách ly](https://www.nytimes.com/interactive/2020/04/03/us/coronavirus-stay-home-rich-poor.html)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040506.jpg)

New York Times phân tích dữ liệu vị trí điện thoại thông minh, phát hiện cả các khu vực thu nhập cao nhất và khu vực nghèo ở Mỹ đều xuất hiện sự giảm sút trong các hoạt động ngoài trời gần đây. Nhưng, các khu vực thu nhập cao giảm hoạt động xuất hiện sớm hơn và ở mức độ sâu hơn. Nghĩa là, người nghèo ở nhà ít hơn, ra ngoài nhiều hơn.

Hình trên là biểu đồ đường giảm hoạt động, màu xanh dương là khu vực giàu, màu vàng là khu vực nghèo. Có thể thấy, màu xanh dương bước vào cách ly sớm hơn màu vàng ba ngày, và mức độ cách ly sâu hơn.

6、**Tin tức một câu**

> - Tỷ lệ tử vong do COVID-19 của [Ý](https://swprs.org/a-swiss-doctor-on-covid-19/) rất cao, nhưng tỷ lệ tử vong toàn dân (bao gồm tất cả nguyên nhân tử vong) vẫn rất bình thường, thậm chí thấp hơn mức trung bình hàng năm.

> - [NASA](https://twitter.com/DMOberhaus/status/1247607588319100936) tuyên bố, đang nghiên cứu khả năng xây dựng kính thiên văn vô tuyến trong hố thiên thạch ở phía sau Mặt trăng. Do các hố thiên thạch đều rất to lớn, kính thiên văn như vậy có thể có đường kính vượt quá 5 km.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040808.jpg)

> - [Một công ty khởi nghiệp ở Thâm Quyến](https://spectrum.ieee.org/automaton/transportation/self-driving/robot-vehicles-make-contactless-deliveries-amid-coronavirus-quarantine) bắt đầu sử dụng xe không người lái để giao hàng và phun dung dịch khử trùng trong khuôn viên. Xe sử dụng LiDAR để nhận dạng đường, nếu gặp tình huống không thể phán đoán, sẽ truyền về trung tâm điều khiển để nhận điều khiển từ xa.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040802.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040903.jpg)

> - [Cloudflare](https://blog.cloudflare.com/moving-from-recaptcha-to-hcaptcha/) tuyên bố. Do dịch vụ reCAPTCHA của Google bắt đầu thu phí, sau khi đánh giá sẽ chuyển sang hCAPTCHA. Điều khó hiểu là, bài kiểm tra mới vẫn là thách thức nhận dạng hình ảnh, không đổi thành thách thức thanh trượt như Geetest. Tôi nghĩ, thanh trượt rõ ràng thân thiện hơn với người dùng.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040809.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040810.jpg)

> - [Facebook](https://www.nytimes.com/2020/01/29/technology/facebook-privacy-lawsuit-earnings.html) đồng ý trả 550 triệu đô la để bồi thường cho người dùng Illinois. Nguyên nhân là Facebook thu thập dữ liệu khuôn mặt từ ảnh của hàng triệu người dùng bang này mà không có sự cho phép.

> - Tổng doanh thu ngành [nhà hàng Mỹ](https://news.ycombinator.com/item?id=22152680) năm 2019 là 863 tỷ đô la, so với đó, tổng doanh thu ngành phần mềm toàn cầu là 467 tỷ đô la.

## Bài viết

1、[Tôi đã phá mật khẩu ví Bitcoin như thế nào？](https://reperiendi.wordpress.com/2020/04/03/how-i-recovered-over-300k-of-bitcoin/)（Tiếng Anh）

Có người nhiều năm trước đã mua Bitcoin, nhưng quên mật khẩu ví. Về lý thuyết, những Bitcoin này không thể tìm lại. Ông không cam lòng, tìm đến một nhà mật mã học, sẵn sàng trả 100.000 đô la để phá mật khẩu ví. Bài viết có một chút khó, nhưng đáng đọc.

2、[Lệnh tùy chỉnh bắt đầu bằng dấu phẩy](https://rhodesmill.org/brandon/2009/commands-with-comma/)（Tiếng Anh）

Tác giả đề xuất, tất cả lệnh tùy chỉnh của hệ thống Linux đều bắt đầu bằng dấu phẩy. Như vậy tra cứu sẽ rất tiện lợi, trước tiên nhập dấu phẩy, sau đó nhấn phím Tab, tất cả lệnh tùy chỉnh sẽ hiển thị.

3、[Netflix trở thành công ty streaming như thế nào](https://www.fastcompany.com/3004709/inside-netflixs-project-griffin-forgotten-history-roku-under-reed-hastings)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040904.jpg)

Netflix ban đầu là công ty cho thuê đĩa DVD, người dùng đặt hàng trên website, Netflix sẽ gửi DVD đến nhà người dùng (hình trên). Bài viết này giới thiệu cách họ trở thành công ty streaming video theo yêu cầu, câu chuyện rất hấp dẫn.

4、[Cách sử dụng Wireguard？](https://miguelmota.com/blog/getting-started-with-wireguard/)（Tiếng Anh）

Wireguard gần đây đã vào kernel Linux, bài viết này giới thiệu chi tiết các bước cài đặt và sử dụng nó.

5、[CLUI: Giao diện người dùng dòng lệnh](https://blog.repl.it/clui)

![](https://cdn.beekka.com/blogimg/asset/202003/bg2020030608.jpg)

![](https://cdn.beekka.com/blogimg/asset/202003/bg2020030609.jpg)

Giao diện dòng lệnh CLI không thân thiện với người mới, phải xem tài liệu mới biết dùng. Giao diện đồ họa GUI không phù hợp với phần mềm nhiều tính năng, lại còn kém hiệu quả.

Có người đề xuất một giao diện CLUI (Command Line UI) kết hợp ưu điểm của cả hai: hiển thị hộp gợi ý đồ họa dưới dòng lệnh.

6、[Cách thêm người dùng AWS](https://ncona.com/2020/03/introduction-to-aws-cli/)（Tiếng Anh）

Bài viết này hướng dẫn bạn bắt đầu với Amazon Web Services AWS, bước cơ bản nhất, tạo thêm một người dùng quản trị. Đây còn có một [bài viết tương tự](https://devops.novalagung.com/en/aws-create-individual-iam-user.html), giới thiệu cách sử dụng dịch vụ IAM để thêm người dùng AWS.

7、[Cách sử dụng hàm async với Array.forEach](https://advancedweb.hu/how-to-use-async-functions-with-array-foreach-in-javascript/)（Tiếng Anh）

Trong ngôn ngữ JavaScript, nếu muốn thực hiện thao tác bất đồng bộ trên từng thành viên của mảng qua phương thức Array.forEach(), sử dụng hàm async có thể không đạt được mục đích bạn muốn. Bài viết này giới thiệu cách sử dụng phương thức Array.reduce() để đảm bảo thực hiện thao tác kế tiếp trên từng thành viên.

8、[Rome, một thư viện công cụ JavaScript mới](https://jasonformat.com/rome-javascript-toolchain/)（Tiếng Anh）

Sản phẩm mới của người sáng lập Babel, đưa tất cả các công cụ chính của JS vào một thư viện. Không cần webpack, eslint, prettier, babel, nó đều cung cấp.

Tư tưởng cốt lõi của nó là, thống nhất tất cả các tính năng dựa trên AST (Cây cú pháp trừu tượng), không để mỗi công cụ tự thực hiện phân tích AST một lần.

## Công cụ

1、[Messenger phiên bản desktop](https://www.microsoft.com/en-us/p/messenger/9wzdncrf0083#activetab=pivot:overviewtab)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040302.jpg)

Facebook thông báo, để thích ứng với lượng cuộc gọi tăng mạnh, phần mềm liên lạc Messenger ra mắt phiên bản desktop, cung cấp chat video nhiều người miễn phí không giới hạn. Trên đây là link tải phiên bản Windows, phiên bản Mac tải ở [đây](https://apps.apple.com/us/app/messenger/id1480068668).

2、[Silent Down](https://silentdown.com/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040501.jpg)

Dịch vụ giám sát server có trực tuyến không, người dùng không trả phí có thể giám sát 5 server, kiểm tra mỗi 5 phút. Nếu bị sập, sẽ thông báo cho người dùng qua email hoặc các kênh khác.

3、[Desktop Info](https://www.glenn.delahoy.com/desktopinfo/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040502.jpg)

Một tiện ích Windows, có thể hiển thị thông tin hệ thống trên desktop, nội dung có thể tùy chỉnh.

4、[lossless-cut](https://github.com/mifi/lossless-cut)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040503.jpg)

Một dự án mã nguồn mở, phát triển giao diện đồ họa GUI cho thư viện công cụ video ffmpeg.

5、[DeepL](https://www.deepl.com/translator)

Công cụ dịch máy do một công ty khởi nghiệp ra mắt, được cho là dịch tốt hơn Google Dịch. (@[ketra21](https://github.com/ruanyf/weekly/issues/1169) đóng góp)

6、[plausible](https://github.com/plausible-insights/plausible)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040901.jpg)

Giải pháp thay thế mã nguồn mở của Google Analytics, có thể tự dựng thống kê truy cập website. Đặc điểm là nhẹ, cấu trúc đơn giản.

7、[apioak](https://github.com/apioak/apioak/blob/master/README_CN.md)

API gateway mã nguồn mở do Trung Quốc sản xuất, có thể dùng làm tầng ánh xạ giữa front-end và back-end. Dựa trên OpenResty, hiệu năng tốt, tính năng mạnh. (@[shuaijinchao](https://github.com/ruanyf/weekly/issues/1173) đóng góp)

8、[like-mysql](https://github.com/LuKks/like-mysql)

Thư viện Node.js, tầng ánh xạ ORM cho cơ sở dữ liệu MySQL, sử dụng rất tiện lợi, nhưng tính năng cũng tương đối ít.

9、[esbuild](https://github.com/evanw/esbuild/)

Công cụ đóng gói JS script viết bằng ngôn ngữ Go, theo dữ liệu tác giả cung cấp, thời gian đóng gói chỉ bằng vài chục phần trăm của Webpack.

10、[plink-plonk.js](https://gist.github.com/tomhicks/6cb5e827723c4eaef638bf9f7686d2d8)

Tác giả cung cấp một đoạn code JS, chỉ cần chèn vào trang web, có thể làm cho các thay đổi DOM phát ra âm thanh. Nếu DOM có thay đổi, bạn sẽ nghe thấy âm thanh.

## Tài nguyên

1、[Pluralsight](https://www.pluralsight.com/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040301.jpg)

Pluralsight tuyên bố miễn phí cho người dùng trong tháng Tư, hơn 7.000 khóa học video trên website đều có thể nghe miễn phí. Khóa học C# của họ rất nổi tiếng, gần đây cũng thêm khá nhiều khóa học Python, JS, Java, DevOps.

2、[Khẩu trang in 3D](https://www.makermask.com/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040510.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040511.jpg)

Trang web này cung cấp phương án khẩu trang mã nguồn mở, về bản chất là bộ lọc không khí đeo trên mặt, có thể in 3D. Lớp lọc sử dụng vật liệu HEPA bộ lọc không khí.

3、[Cây thú có vú](http://vertlife.org/data/mammals/)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040601.jpg)

Một tác phẩm trực quan hóa dữ liệu, dựa vào loài và giống của 5.911 loài động vật, vẽ chúng thành một cái cây hình kim tự tháp ngược, có thể phóng to liên tục để xem.

4、[TensorFlow 2 đơn giản thô bạo](https://tf.wiki/)

Đây là bản dịch tiếng Trung của một cuốn sổ tay nhập môn TensorFlow 2 ngắn gọn, cố gắng giúp các nhà phát triển có nền tảng nhất định về machine learning và Python nhanh chóng làm quen với TensorFlow 2. (@[ketra21](https://github.com/ruanyf/weekly/issues/1164) đóng góp)

5、[Dashengpan](https://www.dashengpan.com/)

Công cụ tìm kiếm tài nguyên Baidu Netdisk, được web crawler tự động thu thập. (@[ketra21](https://github.com/ruanyf/weekly/issues/1174) đóng góp)

## Hình ảnh

1、[Con đường dốc nhất thế giới](https://en.wikipedia.org/wiki/Baldwin_Street)

Trước năm 2019, đường Baldwin ở Dunedin, New Zealand là con đường khu dân cư dốc nhất thế giới. Dài 350 mét, độ dốc 35 độ.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040603.jpg)

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040604.jpg)

Năm 2019, ở Wales, Anh có một con đường mới vượt qua nó, độ dốc đạt 37,5 độ. Thị trưởng Dunedin nói, sẽ xem xét đổi chữ trên biển đường Baldwin từ con đường dốc nhất thế giới thành con đường dốc nhất bán cầu Nam.

2、[Sóng hấp dẫn là gì？](https://www.facebook.com/natgeomedia/posts/1571121353051484)

Einstein đề xuất "sóng hấp dẫn" vào năm 1916, một trăm năm sau cuối cùng được phát hiện.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040805.jpg)

Cách hình dung đơn giản về sóng hấp dẫn là, bạn có một tờ vải trải phẳng, trên đó vẽ lưới ô vuông tiêu chuẩn. Tiếp theo hãy tưởng tượng bạn đặt một vật nặng lên tờ vải, ví dụ quả bóng bowling. Khối lượng của quả bóng bowling làm tờ vải bị lõm xuống.

Khi một vật di chuyển trên tờ vải (hãy tưởng tượng một viên bi lăn từ bên này sang bên kia), nếu vật quá gần quả bóng bowling sẽ bị lệch đường. Hãy tưởng tượng cầm quả bóng bowling di chuyển lên xuống trên tờ vải, nếu làm như vậy, không khó thấy các gợn sóng lan ra ngoài trên tờ vải, đó chính là sóng hấp dẫn. Gợn sóng của sóng hấp dẫn gây ra sự biến dạng của không gian và thời gian.

## Bài đọc thêm

1、[Chúng ta không phải gia đình](https://tw.appledaily.com/property/20200223/JWWUCXVVLE5XNSUJE7A7LHBHMM/)

CEO Netflix Reed Hastings vào năm 2009 từng công bố một bức thư ngỏ, có nhiều câu nói gây sốc về văn hóa làm việc mạnh mẽ của Netflix. Trong đó câu nổi tiếng nhất chính là "We Are Not Family" (Chúng ta không phải gia đình).

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040504.jpg)

Theo thống kê của Glassdoor, lương kỹ sư cấp cao Netflix trung bình cao hơn Google 60%. Nếu lên Teamblind tìm kiếm, bạn có thể thấy có người ở Netflix lương năm lên đến 400.000 đô la, thậm chí có người 500.000. Lương 400.000 đô la ở Mỹ, là mức lương ngang với Tổng thống.

Không có mức lương cao nào mà không có lý do. Netflix chỉ muốn những người thành công, và muốn những người thành công năm này qua năm khác không bao giờ dừng lại. Quan điểm tuyển dụng của Netflix là: một người hạng A rẻ hơn hai người hạng B, vì vậy họ chỉ muốn người hạng A trong những người hạng A.

Sau lợi nhuận cao là áp lực cao. Công ty này nuôi dưỡng một nền văn hóa lính đánh thuê rất đặc biệt, họ không muốn lòng trung thành, chỉ muốn anh hùng có thể chiến đấu.

Hastings tuyên bố rõ ràng rằng, gia đình có tình yêu và bao dung vô hạn, gia đình phải lặp đi lặp lại chịu đựng sai lầm và thất bại. Netflix sẽ không coi bạn như gia đình. Đội nhóm ở đây chỉ có một nhiệm vụ, đó là đẩy mỗi người đến giới hạn không thể. Ở đây không có bao dung, làm không được sẽ bị thay thế.

• Chúng tôi không cung cấp sushi, rượu vang. Bạn đến để chiến đấu, không phải để tiệc tùng.
• Chúng tôi không xem nỗ lực hay số giờ làm việc, chúng tôi chỉ xem kết quả chiến đấu.
• Chúng tôi chỉ muốn người hạng A, đổi lại cũng là phần thưởng của hạng A.
• Nếu bạn là hạng B, dù nỗ lực của hạng A, chúng tôi vẫn sẽ mời bạn ra đi.
• Chúng tôi không muốn lòng trung thành, chỉ muốn thành công.
• Nếu bạn chỉ muốn tìm một công việc ổn định, hãy rời đi ngay bây giờ.
• Chúng tôi muốn những chiến binh tự chủ, tự kỷ luật. Chúng tôi không dạy bạn cách chiến đấu, cũng không có thời gian dạy bạn cách tồn tại.
• Công ty không có quy trình và quy tắc. Chúng tôi loại bỏ tất cả các thủ tục rườm rà. Thủ tục rườm rà chỉ phù hợp để quản lý những kẻ ngốc.
• Chúng tôi không theo dõi giờ làm, chỉ theo dõi tiến độ.
• Công tác, ăn uống và thanh toán công vụ không cần hóa đơn. Bao nhiêu tự quyết định.
• Chúng tôi cho bạn tất cả sự tự do, nhưng bạn cũng phải gánh tất cả trách nhiệm.
• Chúng tôi trả cho bạn mức thù lao vô song, dù lời hay lỗ đều như vậy. Thù lao tính theo kết quả, không tính theo thâm niên.
• Nếu bạn định ở lại, thì chỉ vì thành tựu và tiền bạc, không cần bất kỳ lý do nào khác.
• Chúng tôi chỉ cho bạn biết mục tiêu, sẽ không cho bạn biết cách đạt được.
• Chúng tôi chỉ muốn siêu anh hùng.

2、[Kho dự trữ dầu mỏ của Mỹ](https://science.howstuffworks.com/environmental/energy/strategic-petroleum-reserve1.htm)

Từ năm 1977, Bộ Năng lượng Mỹ đã mua lại 62 hang muối khổng lồ ở khu vực ven biển Louisiana và Texas để lưu trữ dầu thô.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040806.jpg)

Những hang muối này được tạo ra bằng cách khoan giếng vào tầng muối dưới lòng đất, sau đó bơm nước ngọt vào để hòa tan muối. Các công ty khai thác mỏ bơm muối đã hòa tan trở lên mặt đất, quá trình này gọi là khai thác dung dịch, có thể tạo ra các hang động với kích thước rất chính xác. Trung bình mỗi hang động có thể chứa 10 triệu thùng dầu.

Những hang động dưới lòng đất này dùng để lưu trữ dầu, thực ra rất an toàn. Một mặt, vì chúng nằm sâu 600 mét đến 1 km dưới lòng đất, áp suất cực cao ở đó có thể ngăn hình thành vết nứt, nên không bị rò rỉ. Ngoài ra, chênh lệch nhiệt độ tự nhiên giữa đỉnh và đáy mỗi hang động thúc đẩy dầu thô lưu thông, từ đó duy trì chất lượng của nó.

![](https://cdn.beekka.com/blogimg/asset/202004/bg2020040807.jpg)

Nếu muốn thu hồi dầu thô từ một hang động, chỉ cần bơm nước vào đáy. Do dầu sẽ nổi trên nước, nên dầu thô sẽ dâng lên bề mặt. Hơn nữa, vì những hang động này nằm gần vịnh Mexico, có đường ống vận chuyển dầu hiện có, cũng tiện cho việc đưa lên tàu để chuyển đi.

Hiện tại, toàn bộ kho dự trữ dầu mỏ của Mỹ là 727 triệu thùng, theo nhu cầu năng lượng 20,7 triệu thùng, có thể đáp ứng 35 ngày. Nếu lưu trữ tăng đến 1 tỷ thùng, sẽ kéo dài đến 48 ngày.

## Danh ngôn & Con số

1、

Tôi sẽ mua Huawei làm điện thoại tiếp theo của mình, để tránh sử dụng dịch vụ của Google.

-- [Độc giả HN](https://news.ycombinator.com/item?id=22778316)

2、

Đối với tôi, tiếng Anh là ngôn ngữ khó viết hơn C hoặc Java.

-- [Cảm nhận khi viết 《Crafting Interpreters》](http://journal.stuffwithstuff.com/2020/04/05/crafting-crafting-interpreters/)

3、

《Từ điển tiếng Anh Oxford》từ "A" đến "ant" mất 10 năm, phần còn lại mất thêm 60 năm mới hoàn thành.

-- [《Từ điển tiếng Anh Oxford ra đời như thế nào》](https://www.abc.net.au/news/2020-04-09/history-of-the-oxford-english-dictionary/12010628)

4、

Đại dịch virus toàn cầu đã chứng minh mối quan hệ phụ thuộc lẫn nhau giữa các quốc gia, hy vọng sự kiện này sẽ không làm kết thúc mối quan hệ đó.

-- [《Coronavirus sẽ để lại gì cho chúng ta》](https://medium.com/@farainechikwiranechz/what-the-coronavirus-will-leave-on-us-8ea4d540005f)

5、

Bằng cách xóa 20 KB phụ thuộc JavaScript trong plugin Mailchimp cho WordPress, tôi ước tính đã giảm phát thải CO2 khoảng 59.000 kg mỗi tháng.

-- [《Lượng khí thải CO2 của Internet》](https://dannyvankooten.com/website-carbon-emissions/)

6、

Năm đầu tiên bỏ học để làm lập trình viên, thu nhập của tôi chỉ ít hơn 4.000 đô la so với đỉnh cao sự nghiệp của cha tôi. Thu nhập hàng năm mà bố mẹ tôi nuôi bảy đứa con ít hơn thu nhập của tôi ở giai đoạn đầu sự nghiệp, nghĩ đến điều này tôi cảm thấy rất không thoải mái.

Đây là khoảnh khắc quan trọng với tôi, tôi nhận ra tiền bạc cung cấp nhiều cơ hội mà nhiều người có thể chưa bao giờ trải nghiệm: du lịch quốc tế, kỳ nghỉ, và những thứ khác mà chúng ta có thể không cần nhưng chắc chắn muốn.

-- [《Lợi ích của việc có đủ tiền》](https://dragonquest64.blogspot.com/2020/02/having-fu-career.html)

## Nhìn lại

Tuần này năm ngoái: [《Bản tin số 51》](http://www.ruanyifeng.com/blog/2019/04/weekly-issue-51.html)

![](https://cdn.beekka.com/blogimg/asset/201904/bg2019041201.jpg)

## Đăng ký

Bản tin này phát hành vào thứ Sáu hàng tuần, cập nhật đồng thời trên [Blog cá nhân của Ruan Yifeng](http://www.ruanyifeng.com/blog) và [Tài khoản công khai WeChat](http://weixin.sogou.com/weixin?query=%E9%98%AE%E4%B8%80%E5%B3%B0%E7%9A%84%E7%BD%91%E7%BB%9C%E6%97%A5%E5%BF%97).

Tìm kiếm "阮一峰的网络日志" trên WeChat hoặc quét mã QR để đăng ký.

![](http://www.ruanyifeng.com/blogimg/asset/2018/bg2018042311.jpg)

（Hết）
