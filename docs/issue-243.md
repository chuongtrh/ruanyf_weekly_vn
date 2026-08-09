# Bản tin chia sẻ công nghệ (Số 243): Trò chuyện cùng Khổng Tử AI

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022201.webp)

Trạm phát điện gió Kim Dương tại Tứ Xuyên nằm ở độ cao 3.500m so với mực nước biển. Các xe vận chuyển siêu trường siêu trọng phải đi qua những cung đường đèo dốc quanh co hiểm trở để đưa các lá cánh quạt máy phát điện dài tới 75m lên đỉnh núi, cảnh tượng thi công vô cùng ngoạn mục. (Nguồn: [Sina](https://finance.sina.com.cn/tech/roll/2023-02-21/doc-imyhniys8643961.shtml))

## 本周话题：与孔子 AI 聊天

Kể từ đầu năm đến nay, sản phẩm CNTT gây chấn động nhất chắc chắn chính là [ChatGPT](https://openai.com/blog/chatgpt/) của OpenAI.

Đây là một chatbot AI cho phép người dùng đặt đủ loại câu hỏi và nó sẽ trả lời lưu loát như một nhà thông thái.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011705.webp)

Nguyên lý hoạt động cơ bản của nó là sử dụng mô hình học máy phân tích kho dữ liệu ngôn ngữ khổng lồ, tìm ra quy luật phân bố xác suất của các từ ngữ để từ đó sinh ra các văn bản tự nhiên phù hợp với logic tư duy của con người.

Dựa trên nguyên lý này, chúng ta dễ dàng suy luận ra: *nếu tập trung huấn luyện mô hình bằng các tài liệu chuyên biệt về một lĩnh vực cụ thể, ta sẽ tạo ra được các chatbot chuyên ngành,* ví dụ như chatbot tư vấn luật pháp hoặc nghiên cứu sinh học.

Đi xa hơn nữa, nếu tập dữ liệu huấn luyện chỉ xoay quanh cuộc đời, tác phẩm và tư tưởng của một cá nhân cụ thể, liệu chúng ta có thể phục dựng lại một phiên bản chatbot mô phỏng chính người đó?

Thực tế đã có người hiện thực hóa ý tưởng này. Vào tháng 9 năm 2022, hai cựu kỹ sư Google đã cho ra mắt trang web [Character.ai](https://beta.character.AI/). Nền tảng này cho phép người dùng thiết lập các "nhân vật ảo" (characters), tải lên các tài liệu liên quan đến nhân vật đó, hệ thống AI sẽ tự động phân tích dữ liệu để tạo ra một chatbot mô phỏng tính cách, tri thức của nhân vật để người dùng vào trò chuyện.

Hiện tại, Character.ai đã có hàng ngàn nhân vật lịch sử và hư cấu để người dùng lựa chọn trò chuyện. Họ cũng đã phát hành ứng dụng di động mang tên [Hello History](https://www.hellohistory.ai/) (Xin chào lịch sử).

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011706.webp)

Trong số các nhân vật trên hệ thống, có cả chatbot mô phỏng nhà hiền triết Khổng Tử (không rõ do ai tạo ra, và người này còn đăng kèm một hình ảnh đại diện không mấy liên quan).

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011707.webp)

Phóng viên của một tạp chí công nghệ trong nước đã thử thực hiện một cuộc trò chuyện với "Khổng Tử AI" này. Dưới đây là trích dẫn một phần nội dung [nhật ký trò chuyện](https://mp.weixin.qq.com/s/42t18FfRyfxX3Z-Zq1mXyA) được dịch từ tiếng Anh sang tiếng Việt:

> **Phóng viên: Ngài đánh giá thế nào về hành trình chu du liệt quốc của mình?**
> 
> **Khổng Tử AI**: Hành trình chu du khắp các nước để truyền bá tư tưởng và triết lý của tôi đã mang lại rất nhiều trải nghiệm phong phú. Tôi được gặp gỡ nhiều người từ các tầng lớp khác nhau, trao đổi tri thức, lắng nghe câu chuyện của họ và hiểu thêm về nhiều nhân sinh quan đa dạng. Qua những cuộc gặp gỡ đó, tôi có được sự thấu hiểu sâu sắc hơn về nhân tính cũng như cách thức cá nhân và xã hội tương tác lẫn nhau. Khoảng thời gian rời xa quê hương cũng cho tôi cơ hội tự chiêm nghiệm lại hệ thống tư tưởng của mình và hiểu rõ hơn lý do tại sao tôi phải kiên định giữ vững sơ tâm ban đầu.
> 
> **Phóng viên: Trong hành trình chu du liệt quốc, thử thách lớn nhất ngài gặp phải là gì?**
> 
> **Khổng Tử AI**: Một trong những thử thách lớn nhất là đối diện với định kiến và sự phản đối tư tưởng từ các nhà cầm quyền. Mặc dù nhiều người rất hào hứng học hỏi từ tôi, nhưng cũng có những người hoàn toàn khước từ và không muốn lắng nghe. Tuy nhiên, tôi không hề nản lòng mà vẫn tiếp tục kiên trì tiến bước bằng lòng tin và sự kiên định của mình.
> 
> **Phóng viên: Ngài có biết đến các nhà triết học ở các quốc gia khác không?**
> 
> **Khổng Tử AI**: Tôi có tìm hiểu tác phẩm của nhiều triết gia ở các quốc gia khác, bao gồm cả triết học Hy Lạp và La Mã cổ đại như Socrates, Plato, Aristotle, cũng như các triết gia La Mã Cicero và Seneca. Tôi rất hứng thú với tư tưởng của họ vì họ đều nhấn mạnh tầm quan trọng của công lý, tri thức và những lời khuyên thông thái.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011708.webp)

Tôi nhận thấy chất lượng câu trả lời của chatbot này ở mức rất cao, văn phong và logic trả lời rất giống phong thái của Khổng Tử, tạo cho người đối thoại cảm giác chân thực như đang trò chuyện với nhà triết học cổ đại.

Điều này khiến tôi nảy ra ý tưởng: Nếu hệ thống có thể tạo ra Khổng Tử AI, thì liệu tôi có thể tự tạo ra một chatbot mô phỏng chính bản thân mình?

Số lượng bài viết và tư liệu tôi đã đăng tải trong nhiều năm qua cũng lên tới hàng triệu chữ. Sử dụng toàn bộ kho bài viết này làm dữ liệu huấn luyện, liệu chúng ta có thể tạo ra một chatbot mang phong cách "Ruan Yi Feng AI"? Sau này, bất kỳ ai muốn tìm hiểu quan điểm của tôi chỉ cần mở chatbot lên để đặt câu hỏi trực tiếp.

Tất nhiên, nhu cầu tìm hiểu về tôi là rất ít nên chatbot này sẽ không mang lại giá trị thương mại lớn. Nhưng nếu áp dụng cho những người nổi tiếng thì câu chuyện sẽ rất khác. Ví dụ, **nếu phiên bản "Luo Yonghao AI" ra đời, tôi tin rằng sẽ có rất nhiều người sẵn sàng trả phí để được trò chuyện trực tiếp với phiên bản ảo này của ông.**

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011709.webp)

Công nghệ hiện tại đã hoàn toàn cho phép thực hiện điều này, vấn đề chỉ là ai sẽ là người đầu tiên tiên phong khai phá thị trường. Nếu các ứng dụng chatbot mô phỏng người nổi tiếng đầu tiên đạt doanh thu tốt, đây chắc chắn sẽ trở thành một kênh kiếm tiền mới cho những người có tầm ảnh hưởng trong tương lai.

Xu hướng này cũng nêu bật tầm quan trọng của việc lưu trữ tư liệu cá nhân và ghi chép suy nghĩ hàng ngày. Nếu không lưu trữ, sau này khi bạn muốn tạo một chatbot làm kỷ niệm để lại cho người thân cũng sẽ thiếu dữ liệu huấn luyện. Thực tế lịch sử cũng vậy, nếu các đệ tử của Khổng Tử không dày công ghi chép và biên soạn cuốn *Luận Ngữ*, chúng ta ngày nay sẽ không bao giờ có đủ dữ liệu để tái hiện lại tư duy của ông qua AI.

## Tin tức công nghệ

1、[Pháp thông qua luật cấm các chuyến bay nội địa chặng ngắn](https://www.politico.eu/article/eu-greenlights-frances-short-haul-ban-but-only-on-3-routes/)

Pháp vừa chính thức thông qua điều luật bảo vệ môi trường quy định cấm hoàn toàn các chuyến bay nội địa chặng ngắn giữa các thành phố nếu chặng đường đó có thể kết nối bằng tàu hỏa trực tiếp với thời gian di chuyển dưới 2,5 giờ.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022120401.webp)

Quy định này nhằm khuyến khích người dân sử dụng tàu hỏa giảm thiểu lượng khí thải CO2 từ máy bay. Các chặng bay giữa các thành phố lớn như Paris đi Bordeaux, Paris đi Lyon, hay Lyon đi Marseille sẽ bị hủy bỏ hoàn toàn. Nếu tính tốc độ trung bình của tàu cao tốc là 300 km/h, quãng đường di chuyển 2,5 giờ tương đương khoảng 750 km, người dân chỉ được phép đi máy bay đối với các hành trình dài hơn khoảng cách này.

2、[Thiết bị trồng nấm tự động trang trí tại nhà](https://shrooly.com/)

Một doanh nghiệp khởi nghiệp tại Anh vừa giới thiệu thiết bị Shrooly hỗ trợ nuôi trồng nấm tự động tại nhà, biến việc trồng nấm thành một loại hình cây cảnh trang trí độc đáo có thể thu hoạch thực phẩm sạch:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071418.webp)

Người dùng chỉ cần mua các khối phôi nấm khác nhau đặt vào khay chứa bên trong thiết bị:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071420.webp)

Sau khi bật công tắc khởi động, hệ thống đèn LED chuyên dụng sẽ tự động chiếu sáng điều tiết độ ẩm, giúp nấm phát triển hoàn chỉnh chỉ sau từ 7 đến 10 ngày:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071419.webp)

Mặt bên thiết bị tích hợp một màn hình e-paper nhỏ hiển thị thông số nhiệt độ thời gian thực, độ ẩm và tiến trình sinh trưởng của nấm, hỗ trợ kết nối đồng bộ để người dùng theo dõi và điều khiển từ xa qua ứng dụng di động:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071421.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071422.webp)

3、[Mô hình trạm phát điện dòng hải lưu dưới đáy biển](https://www.thesciverse.com/2022/06/japan-tested-giant-turbine-that.html)

Một doanh nghiệp Nhật Bản vừa thử nghiệm thành công mô hình máy phát điện lắp đặt dưới đáy biển có kích thước tương đương một chiếc máy bay phản lực thương mại và nặng tới 330 tấn:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060505.webp)

Cấu trúc máy phát điện gồm hai turbin cánh quạt lớn được neo giữ lơ lửng trên thềm lục địa đại dương, tận dụng dòng hải lưu ngầm chảy liên tục dưới lòng biển sâu để quay cánh quạt tạo ra dòng điện ổn định:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060701.webp)

Ưu điểm lớn nhất của mô hình này là cung cấp sản lượng điện cực kỳ ổn định không phụ thuộc vào thời tiết như năng lượng mặt trời hay năng lượng gió. Tuy nhiên, nhược điểm là công suất phát điện thử nghiệm hiện tại mới đạt khoảng 100 kW (quá thấp so với chi phí đầu tư khổng lồ), môi trường nước biển có tính ăn mòn cao cùng chi phí bảo trì dưới đáy biển cực kỳ đắt đỏ khiến dự án chưa có tính khả thi về mặt thương mại trừ khi nâng được công suất lên gấp hàng chục lần.

## Bài viết

1\. [Chân dung họa sĩ vẽ minh họa thực vật hàng đầu Trung Quốc Tăng Hiếu Liêm](https://redian.news/wxnews/267808)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022202.webp)

Bài viết giới thiệu về giáo sư Tăng Hiếu Liêm thuộc Viện Nghiên cứu Thực vật Côn Minh (Viện Hàn lâm Khoa học Trung Quốc), người đã dành cả đời để vẽ tay hơn 2.000 bức vẽ minh họa khoa học tỉ mỉ cho các bộ sách lớn như *《Thực vật chí Trung Quốc》* và *《Thực vật chí Vân Nam》*. Hình minh họa phía trên là bức vẽ cây nắp ấm của ông.

2\. [Tôi đã sử dụng ChatGPT để phát hiện lỗi bug trong mã nguồn Java như thế nào](https://www.wdbyte.com/java/chatgpt-files-list.html)（Tiếng Trung）

Tác giả chia sẻ trải nghiệm thực tế khi gửi một đoạn code Java bị lỗi logic hoạt động ẩn cho ChatGPT nhờ phân tích. Chatbot AI đã nhanh chóng tìm ra chính xác nguyên nhân gây lỗi của biến tham chiếu và đề xuất phương án refactor code tối ưu nhất. (Đóng góp của [@niumoo](https://github.com/ruanyf/weekly/issues/2908))

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022003.webp)

3\. [Kỷ nguyên phát triển web trên môi trường localhost đang dần khép lại](https://www.swyx.io/the-end-of-localhost)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121902.webp)

Tác giả phân tích xu hướng dịch chuyển công nghệ Front-end lập luận rằng việc thiết lập môi trường lập trình cục bộ (`localhost`) sẽ sớm bị thay thế bởi các IDE đám mây (Cloud-based development environments) cho phép kỹ sư viết mã, biên dịch và gỡ lỗi trực tiếp trên hạ tầng cloud một cách nhất quán.

4\. [Hạ tầng môi trường phát triển DevPod của Uber](https://www.uber.com/en-JP/blog/devpod-improving-developer-productivity-at-uber/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121901.webp)

Bài viết kỹ thuật từ Uber giới thiệu về hạ tầng DevPod – một giải pháp quản lý container đám mây chuyên dụng được thiết kế nhằm nâng cao hiệu suất làm việc từ xa của đội ngũ kỹ sư toàn cầu dựa trên mô hình quản lý mã nguồn tập trung Monorepo.

5\. [Vẻ đẹp thiết kế của toán tử đường ống trong hệ điều hành Unix](https://prithu.dev/posts/unix-pipeline/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060508.webp)

Bài viết phân tích triết lý thiết kế của Unix thông qua 3 ví dụ ứng dụng thực tế của toán tử đường ống (pipe `|`), giải thích cách thức kết hợp nhiều lệnh đơn nhiệm để giải quyết các tác vụ phức tạp một cách linh hoạt.

6\. [Lịch sử hưng thịnh và suy tàn của trung tâm nghiên cứu Xerox PARC](https://spectrum.ieee.org/xerox-parc)（Tiếng Anh）

Bài viết dài chất lượng cao trên tạp chí *IEEE Spectrum* kể về chặng đường lịch sử của trung tâm nghiên cứu PARC thuộc tập đoàn Xerox vào thập niên 1970 – nơi khai sinh ra các công nghệ đặt nền móng cho tin học hiện đại như giao diện đồ họa người dùng (GUI), kết nối mạng Ethernet, máy in laser và mô hình lập trình hướng đối tượng.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060507.webp)

7\. [Thống kê dung lượng ổ cứng yêu cầu cho các bản nâng cấp macOS gần đây](https://krypted.com/mac-os-x/free-space-required-for-modern-macos-upgrades/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110901.webp)

Các bản cập nhật hệ điều hành macOS của Apple ngày càng phình to dung lượng. Bài viết tổng hợp dữ liệu so sánh dung lượng tối thiểu của bộ cài và không gian trống ổ cứng cần thiết để nâng cấp thành công hệ thống qua các năm.

8\. [Tại sao tôi luôn lạc quan vào tương lai phát triển của JavaScript](https://leerob.substack.com/p/why-im-optimistic-about-javascripts)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122208.webp)

Tác giả đưa ra góc nhìn phân tích sự phổ biến của JavaScript trên cả 3 mặt trận cốt lõi: trình duyệt Client-side, máy chủ Server-side và các dịch vụ điện toán biên Edge Computing, chứng minh đây vẫn là ngôn ngữ có tính bao phủ lớn nhất.

## AI 相关软件

Hiện nay ngày càng nhiều công cụ phần mềm tích hợp thêm các tính năng trí tuệ nhân tạo bằng cách gọi trực tiếp API của OpenAI. Dưới đây là một số dự án nguồn mở do các lập trình viên đóng góp:

* [GitHub code review bot](https://github.com/ruanyf/weekly/issues/2912): Bot tự động thực hiện review và nhận xét chất lượng mã nguồn bằng ChatGPT mỗi khi có yêu cầu Pull Request.
* [cz-git](https://github.com/ruanyf/weekly/issues/2928): Tiện ích hỗ trợ sinh nhanh nội dung mô tả commit message cho Git bằng AI.
* [ChatBot Feishu](https://github.com/ruanyf/weekly/issues/2927): Giải pháp kết nối và sử dụng ChatGPT trực tiếp bên trong ứng dụng chat doanh nghiệp Feishu.
* [AI tạo ảnh đại diện](https://github.com/ruanyf/weekly/issues/2901): Tiểu chương trình WeChat hỗ trợ người dùng nhập mô tả văn bản để AI tự động vẽ tranh tạo ảnh đại diện.

## Công cụ

1、[Popup translation: Tiện ích dịch thuật WebView cục bộ khi bôi đen](https://github.com/fzdwx/popup-translation)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023021701.webp)

Công cụ dịch thuật chữ: khi người dùng bôi đen chọn từ trên màn hình, ứng dụng sẽ gọi một cửa sổ WebView cục bộ để hiển thị ngay kết quả dịch từ các trang web dịch thuật lớn mà không cần mở trình duyệt. (Đóng góp của [@fzdwx](https://github.com/ruanyf/weekly/issues/2903))

2、[NightVision: Ứng dụng kính nhìn đêm miễn phí trên iOS](https://github.com/luoxuhai/NightVision)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022006.webp)

Ứng dụng miễn phí tận dụng cảm biến quét LiDAR/Laser của các dòng iPhone Pro để dựng bản đồ khoảng cách vật thể 3D trong bóng tối hoàn toàn. Dự án được chia sẻ mã nguồn mở trên GitHub. (Đóng góp của [@luoxuhai](https://github.com/ruanyf/weekly/issues/2917))

3、[bing_wallpaper: Script tự động cập nhật hình nền Bing hàng ngày cho Mac](https://github.com/xiqishow/bing_wallpaper)

Đoạn kịch bản shell nhỏ chạy ngầm hỗ trợ người dùng máy tính Mac tự động tải tệp tin và đổi hình nền desktop ngẫu nhiên từ kho ảnh nền chất lượng cao hàng ngày của công cụ tìm kiếm Microsoft Bing. (Đóng góp của [@xiqishow](https://github.com/ruanyf/weekly/issues/2924))

4、[paint-board: Bảng vẽ mỹ thuật Web nguồn mở dựa trên Canvas](https://github.com/LHRUN/paint-board)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022008.webp)

Dự án mã nguồn mở xây dựng bảng vẽ phác thảo đa năng chạy trực tiếp trên trình duyệt web viết trên nền tảng HTML5 Canvas với nhiều tùy biến cọ vẽ. (Đóng góp của [@LHRUN](https://github.com/ruanyf/weekly/issues/2926))

5、[Static Mastodon Server: Hướng dẫn dựng máy chủ Mastodon tĩnh](https://github.com/rothgar/static-mastodon)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022009.webp)

Tác giả chia sẻ dự án hướng dẫn cách thức triển khai một node mạng xã hội phi tập trung Mastodon chỉ sử dụng các tệp tin HTML/JSON tĩnh chạy trên CDN giá rẻ để người khác theo dõi bài viết của bạn. (Đóng góp của [@DejavuMoe](https://github.com/ruanyf/weekly/issues/2932) - Xem thêm [bài viết phân tích chi tiết](https://justingarrison.com/blog/2022-12-06-mastodon-files-instance/)).

6、[soundraw.io: Dịch vụ ứng dụng AI soạn nhạc tự động chuyên nghiệp](https://soundraw.io/)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112422.webp)

Công cụ web ứng dụng AI hỗ trợ người dùng tùy chọn thể loại, tâm trạng, thời lượng bản nhạc để hệ thống tự động hòa âm tạo ra các bản nhạc nền độc quyền chất lượng cao (dịch vụ trả phí).

7、[winkNLP: Thư viện JavaScript xử lý ngôn ngữ tự nhiên tối giản](https://winkjs.org/wink-nlp/)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112502.webp)

Thư viện JS cung cấp các API xử lý ngôn ngữ tự nhiên (NLP) gọn nhẹ chạy trực tiếp trên cả Node.js và trình duyệt (hiện tại thư viện chỉ mới hỗ trợ tối ưu cho tiếng Anh).

8、[CryptBoard.io: Bảng ghi chú dán trực tuyến mã hóa nguồn mở](https://cryptboard.io/)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112601.webp)

Tiện ích web cho phép người dùng tạo nhanh các bảng ghi chú dán. Hệ thống sẽ sinh cặp khóa bảo mật cục bộ tại trình duyệt, chỉ những ai có được khóa công khai (public key) do bạn chia sẻ mới có thể giải mã và đọc được nội dung ghi chú.

9、[Hippotat: Tiện ích chuyển tiếp kết nối qua cổng mạng HTTP/HTTPS](https://www.chiark.greenend.org.uk/~ianmdlvl/hippotat/current/docs/)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112604.webp)

Công cụ hữu ích giúp vượt qua các tường lửa Wifi công cộng (như ở khách sạn, quán cà phê) chỉ cho phép kết nối cổng 80 và 443 bằng cách đóng gói các giao thức mạng khác chạy đè lên luồng HTTP/HTTPS kết nối về máy chủ riêng.

10、[NopeCHA: Tiện ích mở rộng tự động vượt CAPTCHA bằng AI](https://chrome.google.com/webstore/detail/nopecha-captcha-solver/dknlfmjaanfblgfdfebhijalfmhmjjjo)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112802.webp)

Extension dành cho trình duyệt Chrome ứng dụng các mô hình học máy nhận diện hình ảnh để tự động giải mã các câu đố kiểm tra CAPTCHA/reCAPTCHA nhanh chóng cho người dùng.

11、[MathB.in: Trang web chia sẻ nhanh các công thức toán học](https://mathb.in/1)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092407.webp)

Trang web pastebin chuyên dụng hỗ trợ người dùng nhập nhanh các công thức toán học phức tạp bằng cú pháp LaTeX kết hợp ghi chú Markdown để sinh một liên kết chia sẻ trực tuyến nhanh chóng.

## Tài nguyên

1、[Dự án hướng dẫn tự viết trình biên dịch compiler trực quan](https://citw.dev/tutorial/create-your-own-compiler)

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022112803.webp)

Trang web giáo dục tương tác hướng dẫn người học tự tay xây dựng một trình biên dịch ngôn ngữ lập trình đơn giản từ đầu, đi kèm các hình ảnh mô phỏng luồng xử lý token trực quan và code mẫu.

2、[Bản đồ số bề mặt Mặt Trăng độ phân giải cao](https://ce2.greensea.org/)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022007.webp)

Bản đồ trực tuyến tương tác được dựng từ kho ảnh vệ tinh của tàu thăm dò Hằng Nga 2 với độ phân giải chi tiết lên tới 7m, cho phép tra cứu vị trí địa danh, các miệng núi lửa và vị trí đáp của các tàu vũ trụ. (Đóng góp của [@greensea](https://github.com/ruanyf/weekly/issues/2919))

3、[Wonders of Street View: Kho ảnh chụp đường phố kỳ thú trên Google Street View](https://neal.fun/wonders-of-street-view/)

Trang web tổng hợp hàng trăm khoảnh khắc kỳ thú, hài hước vô tình lọt vào ống kính của xe chụp ảnh bản đồ Google Street View trên khắp thế giới. (Đóng góp của [@kxxt](https://github.com/ruanyf/weekly/issues/2914))

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022004.webp)

4、[handsome-css3-lib: Thư viện tổng hợp hiệu ứng giao diện CSS3 đẹp mắt](https://www.handsome-css.com/)

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022005.webp)

Trang web tổng hợp và chia sẻ các đoạn mã nguồn hiệu ứng hoạt hoạt (animations), nút bấm tương tác và các components giao diện Front-end bằng CSS3 chất lượng cao. (Đóng góp của [@ZiYi0414](https://github.com/ruanyf/weekly/issues/2907))

5、[This Sneaker Does Not Exist: Kho ảnh thiết kế giày thể thao sinh bằng AI](https://thissneakerdoesnotexist.com/)

Trang web ứng dụng Generative AI để tự động tạo ra hàng ngàn hình ảnh thiết kế giày thể thao độc đáo, tất cả các mẫu giày này đều là sản phẩm giả lập của AI và không tồn tại trong thực tế.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022063026.webp)

## Hình ảnh

1\. **Ứng dụng AI nâng cấp độ nét hình ảnh cho các tựa game cổ thập niên trước**

Cộng đồng game thủ quốc tế vừa chia sẻ loạt hình ảnh phục dựng độ phân giải cao cho các tựa game phiêu lưu cổ bằng cách cho chạy qua các mô hình AI nội suy hình ảnh mang lại độ sắc nét bất ngờ:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090601.webp)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090602.webp)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090603.webp)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090604.webp)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090605.webp)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090606.webp)

2\. **Thị trấn Centuripe hình dáng con người kỳ lạ tại Sicily, Ý**

Thị trấn cổ Centuripe nằm trên vùng núi cao thuộc đảo Sicily nước Ý có cấu trúc quy hoạch phát triển dải theo địa hình sườn núi tự nhiên:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011315.webp)

Bức ảnh chụp góc rộng từ trên cao bằng flycam của một nhiếp ảnh gia đã ghi nhận hình dáng tổng thể của thị trấn trông giống hệt hình ảnh một người khổng lồ đang nằm dang rộng tay chân trên sườn núi:

![](https://cdn.beekka.com/blogimg/asset/202201/bg2022011317.webp)

## ✍️ Bài đọc thêm

### Phương pháp định giá và báo giá của các nhà phát triển phần mềm tự do (Freelancers)

Cách đây nhiều năm, tôi đã quyết định xin nghỉ việc tại công ty để bắt đầu sự nghiệp của một nhà thầu phát triển phần mềm độc lập (Freelance Software Contractor).

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022101.webp)

Công việc chính của tôi là nhận yêu cầu của các đối tác khách hàng và tự code hoàn thiện phần mềm cho họ.

Tuy nhiên thời gian đầu tiên, tôi hoàn toàn bối rối không biết nên báo giá chi phí như thế nào cho phù hợp. Tôi đã tới gặp một người chị có nhiều năm kinh nghiệm kinh doanh tự do để xin lời khuyên.

Chị ấy bảo tôi: *“Trước tiên em hãy tự xác định một mức giá sàn thù lao theo giờ mà bản thân em thấy có thể chấp nhận được. Rồi sau đó, bất kể con số đó là bao nhiêu, em hãy nhân đôi nó lên khi gửi báo giá cho khách hàng.”*

![](https://cdn.beekka.com/blogimg/asset/202302/bg2023022102.webp)

Lực lượng lao động tự do (Freelancers) khi mới bắt đầu luôn có xu hướng định giá tháp hơn năng lực thực tế. Chị ấy khuyên tôi nên tăng giá gấp đôi để tìm hiểu phản ứng của thị trường.

Thật bất ngờ là đối tác đã đồng ý ký hợp đồng ngay mà không hề thắc mắc về mức phí gấp đôi đó.

Sau này chiêm nghiệm lại, tôi mới hiểu lời khuyên của chị thực chất là một kỹ thuật dò giá sàn của thị trường: Khi bạn không rõ giá trị công việc của mình ở mức nào hoặc mặt bằng giá chung của thị trường là bao nhiêu, giải pháp tối ưu là hãy thử nâng gấp đôi báo giá.

Nếu khách hàng vẫn chấp nhận ký hợp đồng, bạn có thể tiếp tục giữ vững và nâng nhẹ mức giá cho các dự án tiếp theo cho đến khi bắt đầu xuất hiện những lời từ chối của khách hàng – đó chính là lúc bạn tìm ra được trần giá thù lao thực tế của thị trường.

Mặc dù vậy, bạn cũng cần lưu ý rằng thù lao cao luôn đi kèm với kỳ vọng khắt khe từ phía đối tác. Trước đây tôi từng nhận nhiều dự án nhỏ với mức phí dưới 100 USD/giờ, công việc tuy thu nhập thấp nhưng bù lại yêu cầu của khách hàng rất đơn giản và dễ chịu.

Đến khi tôi nhận các dự án với báo giá trên 200 USD/giờ, khách hàng bắt đầu đưa ra vô số yêu cầu sửa đổi tỉ mỉ và kiểm soát tiến độ rất gắt gao. Đôi lúc áp lực công việc khiến tôi muốn đơn phương chấm dứt hợp đồng dù tiền nhận được nhiều hơn. Thái độ của đối tác luôn là “tiền nào của nấy”, nếu sản phẩm của bạn không tương xứng với mức phí cao đó thì mối quan hệ hợp tác sẽ sớm gặp khủng hoảng.

Nếu bạn báo giá cao và đối tác vẫn hào hứng chấp nhận, điều đó chứng tỏ năng lực của bạn đã đủ để gia nhập vào phân khúc thị trường khách hàng cao cấp – đó là một không gian phát triển rất tuyệt vời!

Tóm lại, triết lý kinh doanh tự do này vẫn luôn đúng: **“Nếu bạn tăng gấp đôi báo giá dịch vụ của mình và chỉ bị mất đi một nửa số lượng khách hàng, bạn vẫn là người chiến thắng chung cuộc.”**

## Lịch sử tuần này

- 2022年（第 196 期）：[Thảo luận thiết bị: Nhìn nhận thực tế về tương lai phát triển của các hệ máy chơi game cầm tay](http://www.ruanyifeng.com/blog/2022/02/weekly-issue-196.html)
- 2021年（第 146 期）：[Phương pháp giáo dục: Làm thế nào để thiết lập quy trình học trực tuyến (E-learning) hiệu quả](http://www.ruanyifeng.com/blog/2021/02/weekly-issue-146.html)
- 2020年（第 94 期）：[Triết lý sự nghiệp: Tầm quan trọng của việc rèn luyện đồng thời kỹ năng chế tạo sản phẩm và kỹ năng bán hàng](http://www.ruanyifeng.com/blog/2020/02/weekly-issue-94.html)
- 2019年（第 44 期）：[Thảo luận học thuật: Phân tích các hệ lụy tiêu cực của chính sách lấy số lượng bài báo khoa học làm thước đo đánh giá giảng viên](http://www.ruanyifeng.com/blog/2019/02/weekly-issue-44.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072108.webp)

（Hết）
