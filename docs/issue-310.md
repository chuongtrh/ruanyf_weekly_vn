# Bản tin chia sẻ công nghệ (Số 310): Cách kiếm tiền bằng AI của các trang trại nội dung (Content Farm)

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/4743) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072110.webp)

Chợ đêm sầm uất trên đường Nam Bân, Trùng Khánh, nằm ngay bên cạnh sông Trường Giang. Phía đối diện sông là các tòa nhà cao tầng của bán đảo Du Trung. (Nguồn: [Facebook](https://www.facebook.com/photo.php?fbid=785809217049222&id=100068604533594&set=a.526690652961081))

## 内容农场的 AI 赚钱术

"Trang trại nội dung" (Content Farm) là thuật ngữ chỉ các trang web sản xuất hàng loạt bài viết chất lượng thấp nhằm thu hút lượt nhấp chuột và kiếm tiền từ lưu lượng truy cập.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072004.webp)

Nó tự tạo ra hàng vạn bài viết rác, mỗi trang chứa đầy quảng cáo và được đặt những tiêu đề giật gân, tối ưu hóa từ khóa để thu hút độc giả click vào.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072005.webp)

Trước đây, các trang trại nội dung phải thuê người viết để thu thập tài liệu khắp nơi và tạo nội dung. Bây giờ thì đơn giản hơn nhiều, chỉ cần giao cho AI viết, tạo ra một bài viết chỉ mất 2 giây.

Hơn nữa, **chi phí sử dụng AI đã giảm xuống mức rất thấp, thấp đến mức chỉ cần doanh thu quảng cáo từ một lượt xem duy nhất cũng đủ để bù đắp chi phí**. Dưới đây, tôi sẽ minh họa cho bạn thấy việc xây dựng một trang trại nội dung bằng AI rẻ như thế nào.

Đầu tiên, bạn có thể dựa vào các từ khóa tìm kiếm hot để tìm các chủ đề mà độc giả quan tâm.

Ví dụ, chúng ta tìm kiếm một vấn đề CNTT thường xuyên được tra cứu, chẳng hạn như cách tắt tính năng cập nhật (update) của Windows.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072006.webp)

Sau đó, yêu cầu AI viết bài viết.

Lúc này bạn cần một đoạn câu lệnh gợi ý (prompt) chính xác. Tôi đã sao chép một đoạn từ [bài viết của một tác giả nước ngoài](https://batchmon.com/blog/ai-cheaper-than-ads/):

> Bạn là một cây bút viết blog xuất sắc. Các bài viết blog của bạn luôn xếp thứ hạng cao trên các công cụ tìm kiếm vì bạn hiểu rất rõ về SEO cũng như cách sử dụng các từ khóa xu hướng và có độ liên quan cao. Các bài viết của bạn chứa nhiều thông tin hữu ích giúp người dùng giải quyết được vấn đề họ đang tìm kiếm.
>
> Bạn sẽ nhận được truy vấn từ những người dùng đang tìm kiếm bài viết blog. Bạn sẽ tạo ra một bài viết blog khớp với truy vấn của họ, hữu ích và giải đáp hoặc liên quan đến nội dung họ đang tìm kiếm.
> 
> Chỉ phản hồi bằng nội dung bài viết blog.
> 
> Câu hỏi của độc giả là: Làm thế nào để tắt tính năng cập nhật của Windows?

Tôi nhập đoạn prompt này vào một AI nội địa Trung Quốc.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072401.webp)

AI ngay lập tức đưa ra bài viết dưới đây.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072007.webp)

Tiếp theo, chúng ta hãy tính toán xem bài viết trên tiêu tốn bao nhiêu tiền.

Chi phí sử dụng AI được tính dựa trên token. AI nội địa tôi dùng có biểu phí như sau:

> - Đầu vào (Input): 0,0008 nhân dân tệ / 1.000 tokens
> - Đầu ra (Output): 0,0020 nhân dân tệ / 1.000 tokens

Sử dụng [công cụ tính token](https://platform.openai.com/tokenizer) của OpenAI, chúng ta biết được prompt đầu vào là 168 tokens, và kết quả đầu ra là 622 tokens. Tổng chi phí được tính như sau:

> （168 * 0.0008 + 622 * 0.0020）/ 1000  
>  = 0.00138 nhân dân tệ

Nói cách khác, **chi phí cho bài viết này là 0,00138 nhân dân tệ**. Chỉ với 1 xu (1 fen = 0,01 tệ) bạn có thể tạo ra 7 bài viết, và tạo ra 1.000 bài viết cũng chỉ tốn 1,38 nhân dân tệ.

Vậy, tôi có thể kiếm được bao nhiêu tiền quảng cáo từ bài viết này?

Số liệu từ các nền tảng quảng cáo trong nước tương đối ít, nhưng ở nước ngoài, thông thường khi sử dụng Google AdSense, [doanh thu](https://snigel.com/blog/adsense-revenue-calculator) dao động từ 0,2 USD đến 2,5 USD cho mỗi 1.000 lượt xem.

Chúng ta lấy mức tối thiểu là 0,2 USD, tương đương khoảng 1,45 nhân dân tệ. Như vậy, doanh thu từ một lượt xem đơn lẻ là 0,00145 nhân dân tệ, vừa vặn cao hơn chi phí tạo ra bài viết.

Do đó, **mỗi lượt xem đều mang lại lợi nhuận**. Chỉ cần có người click vào là đã bù đắp được chi phí nội dung, những lượt xem tiếp theo hoàn toàn là lợi nhuận thuần túy.

Việc vận hành một trang trại nội dung chưa bao giờ dễ dàng đến thế. Đầu tiên tôi mua một cơ sở dữ liệu các từ khóa hot, sau đó chi khoảng hơn 100 nhân dân tệ để tạo ra 100.000 bài viết. Cuối cùng tích hợp quảng cáo, tối ưu SEO, đưa website lên mạng và chờ người dùng click vào.

Không khó để hình dung rằng các trang web tin tức trong tương lai hầu hết sẽ đi theo mô hình này. Việc con người tự sản xuất nội dung có chi phí quá cao, không thể cạnh tranh lại với nội dung do AI tạo ra, và định mệnh chỉ có thể tồn tại dưới dạng các trang web ngách nhỏ.

## 科技动态

1、[Màn hình xanh Windows](https://www.macrumors.com/2024/07/22/microsoft-blames-european-commission-for-outage/)

Tuần trước, hệ thống Windows đã gặp sự cố trên toàn cầu khiến hàng triệu máy tính bị màn hình xanh chết chóc (BSOD) và không thể khởi động.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072301.webp)

Nguyên nhân là do bản cập nhật của công ty phần mềm bảo mật CrowdStrike đã gây ra lỗi nhân (kernel).

Điều này thật kỳ lạ, tại sao một phần mềm ứng dụng của bên thứ ba lại có thể can thiệp và sửa đổi kernel của hệ điều hành?

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072302.webp)

Microsoft giải thích rằng, nhiều năm trước, Ủy ban châu Âu (EC) cho rằng phần mềm bảo mật Windows Defender của chính Microsoft có dấu hiệu độc quyền. Microsoft buộc phải mở quyền truy cập kernel tương tự cho các phần mềm bảo mật khác, đó là lý do tại sao CrowdStrike có thể can thiệp vào kernel.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072506.webp)

Ngược lại, Apple luôn kiên quyết không mở quyền truy cập kernel, vì vậy sự cố lần này không ảnh hưởng đến hệ điều hành Mac. Tuy nhiên, EC hiện đã hướng mũi nhọn chỉ trích về phía Apple.

May mắn là ô tô và máy bay không sử dụng hệ điều hành Windows, nếu không đang di chuyển mà đột ngột màn hình xanh thì thực sự nguy hiểm đến tính mạng.

2、[Cảm giác hạnh phúc](https://www.scientificamerican.com/article/young-adulthood-is-no-longer-one-of-lifes-happiest-times/)

Trước đây, các nhà tâm lý học tin rằng cảm giác hạnh phúc là một đường cong hình chữ U, cao ở hai đầu và thấp ở giữa, người trung niên là những người kém vui vẻ nhất.

Tuy nhiên, nghiên cứu mới nhất cho thấy tâm lý con người đã có sự thay đổi. Mức độ hạnh phúc hiện nay lại là một đường cong đi lên.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072108.webp)

Trong biểu đồ trên, đường cong màu xanh hiển thị khảo sát trước đây về mức độ hạnh phúc, tăng dần trước 30 tuổi, sau đó giảm xuống và chạm đáy ở tuổi 50. Sau khi bước vào tuổi già, nó lại tiếp tục tăng lên.

Đường cong màu vàng đại diện cho khảo sát mới nhất. Mức độ hạnh phúc của người trẻ đã giảm mạnh so với trước đây, tuổi 15 là thời điểm thấp nhất, sau đó không ngừng tăng lên cho đến khi về già.

Lý giải từ các nhà tâm lý học là đối với thế hệ trẻ ngày nay, tuổi vị thành niên trở nên vô cùng khó khăn và trở thành điểm thấp nhất của cuộc đời. Khi mới bắt đầu cuộc sống tự lập, họ cảm thấy lo lắng, trầm cảm, không thấy hy vọng vào tương lai và dễ phạm phải một số sai lầm nghiêm trọng.

3、[Ly bia đồng hồ cát](https://asia.nikkei.com/Business/Food-Beverage/Happy-hourglass-Japan-brewer-helps-beer-go-down-slower)

Vào mùa hè, mọi người uống bia thường có xu hướng uống quá nhanh. Liệu có cách nào giúp làm chậm tốc độ uống bia của họ lại không?

Một công ty Nhật Bản đã giới thiệu sản phẩm "Ly bia đồng hồ cát", được cho là có thể làm giảm tốc độ uống bia đi gấp ba lần.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072303.webp)

Chiếc ly này có thể chứa được 350 ml bia, nhưng phần thắt nút ở giữa chỉ rộng 6 mm, tương đương với việc uống bia bằng một chiếc ống hút 6 mm. Hơn nữa, sau khi uống xong, việc thêm bia vào ly cũng rất phiền phức.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072304.webp)

Công ty định vị chiếc ly này như một món đồ chơi độc lạ với mong muốn "mọi người vừa thưởng thức đồ uống vừa tìm thấy niềm vui".

## 文章

1、[Aliyun Public DNS phiên bản miễn phí giới hạn tốc độ](https://www.landiannews.com/archives/105048.html) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072008.webp)

Dịch vụ DNS miễn phí của Alibaba Cloud bắt đầu giới hạn tốc độ từ ngày 30 tháng 9. Số lượng yêu cầu từ một IP đơn lẻ không được vượt quá 20 QPS (Queries Per Second), nếu vượt quá sẽ cần sử dụng phiên bản trả phí. Đây là đơn vị tiên phong trong việc giới hạn tốc độ DNS công cộng.

2、[Vấn đề lừa đảo của tên miền `.top`](https://krebsonsecurity.com/2024/07/phish-friendly-domain-registry-top-put-on-notice/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072501.webp)

`.top` là một trong những tên miền có tỷ lệ trang web lừa đảo tràn lan nhất, và đơn vị quản lý đăng ký của nó là một công ty Trung Quốc. Tổ chức ICANN đã yêu cầu công ty này phải thực hiện các biện pháp xử lý, nếu không sẽ bị thu hồi quyền quản lý tên miền.

3、[Hướng dẫn cơ bản về thư viện kiểm thử Jest của JS](https://blog.stackademic.com/testing-in-javascript-with-jest-085b26e1750e) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072106.webp)

Hướng dẫn dành cho người mới bắt đầu, giới thiệu ngắn gọn cách sử dụng Jest để viết các trường hợp kiểm thử (test cases). (Đóng góp từ độc giả [@Faizan711](https://github.com/ruanyf/weekly/issues/4852))

4、[Hướng dẫn về tác vụ định kỳ Cron](https://linuxiac.com/how-to-use-cron-and-crontab-on-linux/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202403/bg2024030602.webp)

Một bài hướng dẫn chi tiết dành cho người mới bắt đầu sử dụng Linux về cách thiết lập các tác vụ tự động bằng cron.

5、[Tổng quan về hệ thống xây dựng (Build Systems) trong Frontend](https://sunsetglow.net/posts/frontend-build-systems.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202406/bg2024062301.webp)

Bài viết giới thiệu tổng hợp các khái niệm, quy trình và công cụ trong hệ thống xây dựng frontend.

6、[Vấn đề bảo mật của các kho lưu trữ (repository) fork trên GitHub](https://trufflesecurity.com/blog/anyone-can-access-deleted-and-private-repo-data-github) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072502.webp)

GitHub cho phép người dùng fork (sao chép) kho lưu trữ của người khác. Chỉ cần một kho lưu trữ từng được fork, nó sẽ không bao giờ có thể bị xóa hoàn toàn khỏi hệ thống mạng lưới. Ngay cả khi bạn chuyển kho lưu trữ của mình sang chế độ riêng tư (private), người khác vẫn có thể truy cập được các đoạn mã mới mà bạn commit.

7、**Các bài viết khác**

- Ngày [22 tháng 7](http://www.stdaily.com/index/kejixinwen/202407/1b9a0db4eee24f3184101054da3783a7.shtml) là ngày nóng nhất toàn cầu từng được ghi nhận trong lịch sử khí tượng.
- [Tencent Games](https://finance.sina.com.cn/roll/2024-07-25/doc-incfikph3095737.shtml) áp dụng biện pháp bắt buộc tự động nhận diện khuôn mặt mỗi giây một lần đối với các game thủ chưa trẻ tuổi/vị thành niên.
- Đội ngũ phát triển [Node.js](https://github.com/nodejs/node/pull/53725) chính thức bổ sung tính năng tự động loại bỏ (strip) các đoạn mã khai báo kiểu của TypeScript.

## 工具

1、[Foliate](https://github.com/johnfactotum/foliate)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072112.webp)

Phần mềm đọc sách điện tử định dạng epub trên nền tảng Linux.

2、[Sendune](https://github.com/SendWithSES/Drag-and-Drop-Email-Designer)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072002.webp)

Một công cụ kéo thả trực quan để thiết kế email HTML với mã nguồn mở. Một thư viện thiết kế email tương tự là [mjml](https://documentation.mjml.io).

3、[hash-wasm](https://github.com/Daninet/hash-wasm)

Một thư viện hàm băm siêu nhẹ cung cấp hơn 20 thuật toán băm phổ biến như MD5, SHA-1, cũng như thuật toán bảo mật cao BLAKE3.

4、[Page Replica](https://github.com/html5-ninja/page-replica)

Công cụ mã nguồn mở dùng để thiết lập một trang web lưu trữ đệm (cache website), có khả năng thu thập và sao lưu các trang web khác làm phiên bản trung gian truy cập.

5、[WebUI](https://github.com/webui-dev/webui)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024010704.webp)

Công cụ đóng gói ứng dụng desktop đa nền tảng, cho phép sử dụng trực tiếp trình duyệt làm frontend của ứng dụng, nhẹ hơn nhiều so với Electron và tránh sử dụng WebView.

6、[Squat Counter (深蹲计数器)](https://github.com/zhaoolee/Sport)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072402.webp)

Một ứng dụng web mã nguồn mở sử dụng gia tốc kế của thiết bị di động để đếm số lần đứng lên ngồi xuống (squat). (Đóng góp từ [@zhaoolee](https://github.com/ruanyf/weekly/issues/4869))

7、[Anori](https://anori.app/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042002.webp)

Một tiện ích mở rộng trình duyệt cho phép tùy biến nhiều widget tiện ích trên trang chủ mới.

8、[Blurmatic](https://www.blurmatic.com/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042004.webp)

Một công cụ trực tuyến giúp thêm hiệu ứng mờ nhòe chiều sâu (bokeh) cho ảnh và hỗ trợ xoay ảnh 3D.

9、[FastDownload.io](https://www.fastdownload.io/)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042202.webp)

Công cụ trực tuyến hỗ trợ tải video từ nhiều nền tảng phát trực tuyến như YouTube và TikTok.

10、[Stack](https://github.com/stackframe-projects/stack)

![](https://cdn.beekka.com/blogimg/asset/202404/bg2024042204.webp)

Giải pháp quản lý người dùng mã nguồn mở, đi kèm với các thành phần giao diện frontend và trang quản trị backend.

## AI 相关

1、[Album AI](https://github.com/gcui-art/album-ai)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072107.webp)

Công cụ mã nguồn mở cho phép tải ảnh của bạn vào AI và tìm kiếm ảnh thông qua trò chuyện, tương đương với việc AI sắp xếp và quản lý album ảnh. (Đóng góp từ [@blueeon](https://github.com/ruanyf/weekly/issues/4856))

2、[Essay.Art](https://www.essay.art/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072403.webp)

Công cụ sử dụng GPT-4 để chấm điểm và sửa bài luận tiếng Anh IELTS và TOEFL. (Đóng góp từ [@zengdamo](https://github.com/ruanyf/weekly/issues/3483))

3、[AskAITools](https://github.com/askaitools/askaitools-community-edition)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072102.webp)

Công cụ tìm kiếm ứng dụng AI mã nguồn mở, lập chỉ mục cho hơn 10.000 ứng dụng AI khác nhau. (Đóng góp từ [@xiaoguopku](https://github.com/ruanyf/weekly/issues/4849))

4、[Brev AI](https://brev.ai/zh-CN)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072210.webp)

Trình tạo nhạc AI trực tuyến miễn phí, không yêu cầu đăng ký tài khoản. (Đóng góp từ [@zdamo4194](https://github.com/ruanyf/weekly/issues/4862))

## 资源

1、[AIEmoji](https://ai-emoji.bettergogo.com/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072101.webp)

Công cụ tìm kiếm Emoji, nhập nội dung bạn muốn thể hiện để nhận về biểu tượng Emoji phù hợp nhất. (Đóng góp từ [@bettergoo](https://github.com/ruanyf/weekly/issues/4848))

2、[Trực quan hóa thuật toán](https://gallery.selfboot.cn/algorithms/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072105.webp)

Trang web trực quan hóa tương tác của các thuật toán kinh điển được tác giả phát triển với sự hỗ trợ của AI, mã nguồn mở. (Đóng góp từ [@selfboot](https://github.com/ruanyf/weekly/issues/4851))

3、[Tỷ lệ trúng tuyển của các trường đại học Mỹ](https://flowingdata.com/2024/07/16/more-or-less-college-admissions-time/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072211.webp)

Trang web này cho phép tra cứu tỷ lệ trúng tuyển qua các năm của các trường đại học tại Mỹ. Hình ảnh trên hiển thị dữ liệu của Đại học Bang New York tại Stony Brook (Stony Brook University), với tỷ lệ trúng tuyển trong những năm gần đây duy trì ở mức khoảng 50%.

4、[DevDocs](https://devdocs.io/)

![](https://cdn.beekka.com/blogimg/asset/202401/bg2024011506.webp)

Trang web tra cứu tài liệu API của các tiêu chuẩn Web và các công cụ/phần mềm phổ biến hiện nay.

## 图片

Hôm nay xin giới thiệu một số nét thú vị về đất nước Mexico.

1、[Diện tích của Mexico](https://unchartedterritories.tomaspueyo.com/p/25-fascinating-facts-about-mexico)

Mexico là một quốc gia có diện tích rất lớn, lớn hơn nhiều so với những gì bạn tưởng tượng.

Diện tích của 30 quốc gia châu Âu có thể xếp vừa vặn vào trong bản đồ Mexico, bao gồm cả Đức, Anh, Ireland, Áo, Cộng hòa Séc, Hungary, v.v.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071901.webp)

Trong lịch sử, lãnh thổ Mexico thậm chí từng lớn gấp đôi so với diện tích hiện tại.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024071902.webp)

Trong bản đồ trên, phần màu xanh lá là diện tích lãnh thổ Mexico trong quá khứ, và hai đường kẻ màu đỏ là biên giới Mexico ngày nay.

Lãnh thổ của Mexico chủ yếu bị Hoa Kỳ sáp nhập. Toàn bộ các bang Texas, California, Nevada và Utah ngày nay, cũng như một phần của Arizona, Colorado, New Mexico và Wyoming trong lịch sử đều thuộc về Mexico.

Chiến tranh Mỹ - Mexico diễn ra từ năm 1846 đến năm 1848 đã kết thúc với việc Mexico phải nhượng lại toàn bộ các vùng lãnh thổ này cho Mỹ.

2、[Biên giới Mỹ - Mexico](https://unchartedterritories.tomaspueyo.com/p/whats-mexicos-future)

Dưới đây là hình ảnh biên giới phân chia giữa Mỹ và Mexico.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072204.webp)

Phía bên trái là thành phố San Diego của Mỹ, cảnh quan chủ yếu là vùng nông thôn ngoại ô; còn phía bên phải là thành phố Tijuana của Mexico, hoàn toàn là một đô thị sầm uất với mật độ xây dựng dày đặc.

Sự tương phản lớn giữa hai bên biên giới chủ yếu do nền kinh tế phía bắc Mexico phụ thuộc hoàn toàn vào Mỹ, khu vực nào càng gần biên giới Mỹ thì kinh tế càng phát triển phồn vinh.

## 文摘

1、[Những niềm tin lập trình của tôi](https://evanhahn.com/programming-beliefs-as-of-july-2024/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024072505.webp)

Dưới đây là một số quan điểm hiện tại của tôi về lập trình máy tính, tất cả đều được đúc kết từ kinh nghiệm thực tế của bản thân.

(1) Khi đối mặt với một nhiệm vụ khó khăn, tôi sẽ tự hỏi bản thân: "**Nếu tôi không làm việc này thì sẽ ra sao?**"

Hầu hết các trường hợp, đó là một câu hỏi ngớ ngẩn và tôi bắt buộc phải làm nó. Nhưng trong khoảng 5% tình huống, tôi nhận ra mình thực sự có thể bỏ qua hoàn toàn công việc đó mà không ảnh hưởng gì.

(2) **Sự khác biệt giữa "đơn giản" (simple) và "dễ dàng" (easy) là rất quan trọng**. Đơn giản là từ trái nghĩa của phức tạp. Sự phức tạp phát sinh khi có quá nhiều thứ bị ràng buộc, đan xen lại với nhau.

Dễ dàng lại là một khía cạnh khác, những thứ phức tạp cũng có thể được thực hiện một cách dễ dàng. Hiểu được sự khác biệt giữa hai khái niệm này sẽ giúp bạn phát triển những phần mềm gọn gàng và đơn giản hơn.

(3) **Triệt tiêu trạng thái vô giá trị (NULL)**. Nếu tôi có thể thiết kế dữ liệu/kiểu dữ liệu để ngăn chặn các trạng thái vô hiệu, tôi có thể loại bỏ được một lượng lớn nguồn gốc gây ra lỗi. Một chút rắc rối ban đầu khi thiết kế hệ thống kiểu hoặc cấu trúc cơ sở dữ liệu hoàn toàn là xứng đáng.

(4) **Khả năng kiểm thử (testability) của mã nguồn** về cơ bản chính là khả năng mô-đun hóa (modularity) của mã đó.

(5) **Những vấn đề quan trọng nhất của phần mềm thường lại phi kỹ thuật**. Các vấn đề thực tế của thế giới thực thường là cốt yếu nhất: Thứ tôi đang xây dựng sẽ giúp ích cho ai? Đội ngũ của tôi có đang vận hành một cách lành mạnh hay không?

(6) **Làm những thứ "vô dụng"** đôi khi lại là phương pháp tốt nhất để học hỏi những điều mới mẻ. Tôi từng dành rất nhiều thời gian viết một bộ mã hóa PNG tùy chỉnh cho một dự án phụ lúc rảnh rỗi. Tôi chưa bao giờ nghĩ nó sẽ có ích, nhưng vài tháng sau, khi một dự án khác của tôi cần đến tính năng tương tự, tôi đã biết chính xác mình cần phải làm gì.

2、[Tại sao các công ty Đông Á coi trọng văn hóa nhậu?](https://www.ggd.world/p/why-do-east-asian-firms-value-drinking)

Các doanh nhân Đông Á thường xuyên đi uống rượu cùng nhau và thảo luận công việc ngay trên bàn nhậu. Nhiều khu vực khác trên thế giới không có thói quen này, tại sao vậy?

Điều này có liên quan mật thiết đến văn hóa Đông Á. Văn hóa Đông Á nhấn mạnh chủ nghĩa tập thể và tính phân cấp thứ bậc rõ rệt, mọi người thường không trực tiếp nói ra suy nghĩ thật trước mặt người khác mà thích biểu đạt một cách gián tiếp và ẩn ý hơn.

Mọi người cố gắng tránh xung đột trực diện và kiềm chế cảm xúc cá nhân, điều này khiến chúng ta rất khó để thấu hiểu được suy nghĩ thực sự của đối phương.

Nhậu nhẹt là một giải pháp bù đắp. Chất cồn giúp giảm bớt sự kiềm chế của con người, từ đó thúc đẩy việc chia sẻ thông tin và thắt chặt các mối quan hệ xã giao.

Uống rượu mang lại cơ hội quý giá — dù là trong nội bộ hay bên ngoài doanh nghiệp, giúp các bên tham gia thả lỏng bản thân, chia sẻ cảm xúc thật và xây dựng sự tin cậy lẫn nhau.

## 言论

1、

Một câu nói của Vương Truyền Phúc (Chủ tịch BYD) từ nhiều năm trước về việc chế tạo ô tô đã tiếp thêm cho tôi rất nhiều dũng khí.

Ông nói rằng có nhiều doanh nghiệp vì không hiểu rõ nên thường thần thánh hóa công nghệ đến mức đáng sợ. Sự sợ hãi này thực chất chính là rào cản tâm lý mà những kẻ đi trước dựng lên để đe dọa những người đến sau trong ngành. Họ liên tục nói với bạn rằng bạn sẽ không làm được đâu, vốn đầu tư khổng lồ lắm, nghiên cứu phát triển vô cùng gian nan, cho đến khi bạn bỏ cuộc mới thôi. Thực ra, vấn đề bạn không giải quyết được không phải vì bạn thiếu năng lực, mà là vì bạn đang thiếu đi dũng khí.

-- [Bài phát biểu thường niên của Lôi Quân](https://finance.sina.com.cn/tech/roll/2024-07-23/doc-incfcpey8084281.shtml)

2、

Vitalik Buterin, một trong những người sáng lập Ethereum, vào năm 2017 từng đưa ra nhận định về "Tam đề nan của Blockchain" (Blockchain Trilemma): Một mạng lưới blockchain không thể đồng thời đạt được cả ba yếu tố: phi tập trung, khả năng mở rộng và tính bảo mật.

-- [《Tam đề nan của Blockchain》](https://ieeexplore.ieee.org/document/10549891)

3、

Tuyến xe buýt dài nhất thế giới chạy từ London (Anh) đến Kolkata (Ấn Độ), với tổng chiều dài hành trình lên tới 16.000 km và mất 50 ngày cho một chiều di chuyển.

Tuyến xe này đã dừng hoạt động vào năm 1976. Giá vé thời kỳ đó tương đương khoảng 2.200 bảng Anh ngày nay (khoảng 20.000 nhân dân tệ).

-- [Wikipedia](https://en.wikipedia.org/wiki/London%E2%80%93Calcutta_bus_service)

4、

Slack là một công cụ trò chuyện cộng tác hỗ trợ tăng năng suất công việc vô cùng phổ biến, nhưng có thể bạn chưa biết, từ "Slack" thực chất là một cụm từ viết tắt của "Searchable Log of All Communication and Knowledge" (Nhật ký có thể tìm kiếm của mọi thông tin liên lạc và kiến thức).

-- [《Slack là một từ viết tắt》](https://www.theverge.com/2016/9/28/13098164/slack-is-an-acronym)

5、

Chúng ta có thể sử dụng bộ quy tắc dưới đây để mô tả phản ứng của con người đối với công nghệ mới theo thời gian:

(1) Mọi thứ tồn tại trên thế giới khi bạn sinh ra đều là điều bình thường, hiển nhiên và là một phần quy luật vận hành tự nhiên của thế giới.

(2) Bất kỳ công nghệ nào được phát minh ra trong độ tuổi từ 15 đến 35 của bạn đều là những thứ mới mẻ, thú vị và mang tính cách mạng, và bạn rất có thể sẽ tìm kiếm sự nghiệp phát triển từ nó.

(3) Bất kỳ thứ gì được phát minh ra sau khi bạn bước sang tuổi 35 đều là đi ngược lại với quy luật tự nhiên của vạn vật.

-- [Douglas Adams](https://fs.blog/douglas-adams-reactions-technology-over-time/), nhà văn người Anh

## 往年回顾

[Làm thế nào để kiếm tiền từ phần mềm nguồn mở?](https://www.ruanyifeng.com/blog/2023/07/weekly-issue-263.html) (2023 #263)

[Đảo tri thức và phần mềm tri thức](https://www.ruanyifeng.com/blog/2022/07/weekly-issue-213.html) (2022 #213)

[Thành phố của bạn có bao nhiêu giường bệnh?](https://www.ruanyifeng.com/blog/2021/06/weekly-issue-163.html) (2021 #163)

[Tại sao tội phạm bạo lực ngày càng ít đi?](https://www.ruanyifeng.com/blog/2020/06/weekly-issue-113.html) (2020 #113)

(Hết)
