# Bản tin chia sẻ công nghệ (Số 328): Phát triển mô hình AI không phải là một mô hình kinh doanh tốt

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/5610) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120405.webp)

Ga tàu Nam Thượng Hải đang tiến hành dự án cải tạo và nâng cấp quy mô lớn. Nửa phía bắc của nhà ga đang được rào chắn thi công trong khi nửa phía nam vẫn duy trì hoạt động phục vụ hành khách bình thường. Hai khu vực được ngăn tách biệt hoàn toàn bằng một bức màn bạt khổng lồ dựng từ trần nhà xuống đất.

## AI 模型不是一门好生意

Bộ ứng dụng văn phòng [Microsoft 365](https://finance.sina.com.cn/tech/digi/2024-11-05/doc-incuzhax4326302.shtml) của tập đoàn Microsoft mới đây đã chính thức tăng giá bán, với mức tăng cao nhất tại một số quốc gia lên tới 41%.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120117.webp)

Lý do được Microsoft đưa ra là nhằm bù đắp cho các khoản chi phí vận hành khổng lồ của trợ lý AI Copilot được tích hợp thêm vào hệ thống. Riêng tại thị trường Trung Quốc đại lục, do tính năng Copilot chưa được hỗ trợ vận hành nên giá dịch vụ tạm thời vẫn được giữ nguyên.

Không hẹn mà gặp, OpenAI cũng vừa phát đi thông tin dự kiến sẽ điều chỉnh tăng mạnh giá cước dịch vụ. Mức phí đăng ký sử dụng các mô hình AI cao cấp thế hệ mới của hãng có thể tăng vọt từ mức 20 USD/tháng hiện tại lên tới **2.000 USD/tháng**.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120118.webp)

*(Thông tin cập nhật mới nhất: Phiên bản ChatGPT Pro vừa được chính thức ra mắt đã áp dụng mức phí thuê bao mới là 200 USD/tháng).*

Chuỗi động thái điều chỉnh giá cước của các ông lớn công nghệ đã chứng minh một thực tế trần trụi: **Chi phí vận hành và huấn luyện các mô hình AI là cực kỳ tốn kém, đến mức ngay cả những tập đoàn giàu nhất thế giới cũng không thể gánh nổi** và buộc phải chuyển giao áp lực tài chính này lên vai người dùng.

Không chỉ riêng Microsoft hay OpenAI, hầu hết các công ty đang trực tiếp phát triển mô hình AI hiện nay đều đang phải trải qua những ngày tháng vô cùng khó khăn. Họ bắt buộc phải chấp nhận bù lỗ để cung cấp dịch vụ AI giá rẻ nhằm cạnh tranh giành giật thị phần.

Áp lực tài chính nặng nề này được dự báo sẽ còn kéo dài trong nhiều năm tới. Những phân tích dưới đây chỉ ra [nguyên nhân cốt lõi](https://benn.substack.com/p/do-ai-companies-work) tại sao việc phát triển mô hình AI thô lại không phải là một mô hình kinh doanh tốt (good business):

**(1) Phát triển mô hình AI yêu cầu nguồn vốn đầu tư khổng lồ thường trực.**

Các báo cáo tài chính cho thấy chi phí vận hành hằng năm của OpenAI đã chạm mốc 7 tỷ USD, Anthropic dự kiến tiêu tốn khoảng 2,7 tỷ USD trong năm nay, trong khi tập đoàn Meta (Facebook) mới đây cũng phải bổ sung thêm hàng tỷ USD ngân sách đầu tư cho mảng nghiên cứu AI của mình.

Để có thể cân đối thu chi và sinh lời từ mức đầu tư khổng lồ như vậy đòi hỏi doanh nghiệp phải sở hữu hàng trăm triệu người dùng sẵn sàng trả phí hằng tháng — một mục tiêu vô cùng gian nan.

**(2) Chi phí phát triển mô hình hoàn toàn không có tính hiệu quả theo quy mô (Scale Economies).**

Trong đại bộ phận các ngành công nghiệp truyền thống, quy mô sản xuất càng lớn sẽ giúp chi phí sản xuất trên một đơn vị sản phẩm càng giảm. Tuy nhiên, ngành phát triển mô hình AI lại vận hành theo quy luật hoàn toàn ngược lại: Mô hình có quy mô càng lớn thì chi phí biên để tiếp tục cải thiện hiệu năng lại càng đắt đỏ hơn.

Bởi lẽ khi mô hình đã đạt đến một ngưỡng giới hạn nhất định, việc tiếp tục nâng cấp hiệu năng dù chỉ một phần trăm nhỏ cũng sẽ đòi hỏi khối lượng tính toán và dữ liệu huấn luyện tăng lên theo cấp số nhân. Quá trình này tương tự như việc chinh phục đỉnh Everest: Khi đã vượt qua độ cao 8.000 mét, mỗi bước tiến lên phía trước đều khó khăn và tốn kém năng lượng hơn gấp bội. Chi phí để huấn luyện một mô hình AI hàng đầu năm 2024 đắt đỏ và phức tạp hơn rất nhiều so với năm 2023.

Trong khi đó, chất lượng đầu ra của AI lại phụ thuộc trực tiếp vào quy mô tham số và năng lực tính toán. Mô hình càng lớn, năng lực xử lý càng mạnh. Do đó, chi phí vận hành của các công ty AI chỉ có xu hướng tăng cao liên tục chứ không thể giảm đi.

**(3) Tốc độ khấu hao giá trị của mô hình AI diễn ra cực kỳ nhanh.**

Để giữ vững thị phần và mang lại niềm tin cho các nhà đầu tư, các công ty AI bắt buộc phải liên tục chạy đua ra mắt các mô hình mới có tốc độ xử lý nhanh hơn, thông minh hơn và mạnh mẽ hơn.

Sự ra đời liên tục của các thế hệ mô hình mới sẽ khiến giá trị thương mại của các thế hệ mô hình cũ sụt giảm nhanh chóng. Khi người dùng đã có thể sử dụng GPT-4, hầu như không còn ai muốn trả phí để dùng GPT-3 nữa. Chỉ cần đối thủ cạnh tranh ra mắt một mô hình ưu việt hơn, mô hình của bạn sẽ lập tức bị người dùng quay lưng.

Để duy trì vị thế cạnh tranh trên thị trường, bạn bắt buộc phải liên tục lọt vào nhóm sở hữu mô hình AI mạnh mẽ nhất. Điều này đồng nghĩa với việc dòng vốn đầu tư cho R&D của doanh nghiệp tuyệt đối không được phép dừng lại.

Ngay cả khi công nghệ chạm ngưỡng giới hạn vật lý khiến tốc độ ra mắt mô hình mới chậm lại, các mô hình cũ vẫn bị mất giá do sự phát triển mạnh mẽ của cộng đồng mã nguồn mở (như Llama của Meta hay Mistral). Nếu các mô hình thương mại trả phí không thể tạo ra khoảng cách hiệu năng đủ lớn, người dùng sẽ lập tức chuyển sang sử dụng miễn phí các mô hình mã nguồn mở trên GitHub.

Ví dụ điển hình là hãng Anthropic, trong lịch sử phát triển ngắn ngủi của mình, hãng đã phải tự tay khai tử và thay thế tới 10 thế hệ mô hình khác nhau và gánh chịu những khoản lỗ khổng lồ. 8 mô hình đầu tiên hiện nay hoàn toàn không còn giá trị thương mại, mô hình thứ 9 đã được chuyển thành mã nguồn mở, và hãng chỉ còn trông chờ vào mô hình thứ 10 để duy trì một lợi thế công nghệ mỏng manh trên thị trường.

Để có thể tiếp tục sinh tồn trong tương lai, Anthropic không có lựa chọn nào khác ngoài việc phải lập tức đổ tiền nghiên cứu thế hệ mô hình thứ 11.

**(4) Các công ty AI khó lòng thiết lập được rào cản độc quyền vững chắc.**

OpenAI hiện đang giữ vị thế dẫn đầu thị trường nhờ sở hữu năng lực tính toán khổng lồ. Tuy nhiên, toàn bộ hạ tầng tính toán vật lý này đều được thuê lại từ dịch vụ đám mây của các bên thứ ba chứ không thuộc quyền sở hữu của hãng. Chỉ cần sở hữu nguồn lực tài chính đủ lớn, bất kỳ đối thủ nào cũng có thể thuê lại chính hạ tầng tính toán tương đương đó. Hoàn toàn có thể xảy ra kịch bản một nhóm kỹ sư cốt cán rời bỏ OpenAI, huy động vốn đầu tư để thuê hạ tầng máy chủ và tự xây dựng nên một mô hình cạnh tranh sòng phẳng chỉ trong vòng vài tháng.

Nói cách khác, hệ thống trung tâm dữ liệu trị giá hàng tỷ USD của các nhà cung cấp đám mây mới là rào cản độc quyền vững chắc (moat), còn các thế hệ mô hình GPT cũ do OpenAI dày công phát triển không phải là rào cản, bởi lẽ các mô hình có tính năng tương đương hiện đã được chia sẻ miễn phí trên GitHub.

Việc các công ty AI cố gắng đầu tư tự xây dựng trung tâm dữ liệu riêng cũng không mang lại nhiều ý nghĩa, bởi đối thủ cạnh tranh hoàn toàn có thể chọn giải pháp thuê đám mây để tối ưu hóa chi phí đầu tư ban đầu mà vẫn đạt được hiệu quả tương đương.

Tóm lại, <u>phát triển mô hình AI thô đang là một ngành công nghiệp vô cùng khắc nghiệt: Doanh nghiệp bắt buộc phải liên tục duy trì nguồn vốn đầu tư khổng lồ hằng năm để bù đắp chi phí vận hành ngày một tăng cao, trong khi sản phẩm làm ra đối mặt với nguy cơ bị đào thải và mất trắng giá trị chỉ sau một đến hai năm</u>. Bạn không có công cụ hữu hiệu để ngăn chặn đối thủ sao chép, nhân sự cốt cán có thể rời đi bất kỳ lúc nào, và ưu thế công nghệ tạm thời rất khó để chuyển hóa thành lợi thế cạnh tranh dài hạn.

Do đó, các doanh nghiệp đang có ý định dấn thân vào mảng phát triển mô hình AI thô cần phải cân nhắc vô cùng kỹ lưỡng trước khi quyết định đầu tư.

Đối với các công ty đã lựa chọn con đường này, do đặc thù đốt tiền của ngành, doanh nghiệp nào gọi được nguồn vốn lớn nhất sẽ là người có cơ hội sống sót lâu nhất. Vì vậy, nhiệm vụ sống còn hiện nay của các hãng là phải huy động nguồn vốn đầu tư càng nhiều và càng nhanh càng tốt.

Bên cạnh đó, một giải pháp khả thi là tìm cách cá nhân hóa mô hình để tăng độ kết dính (stickiness) với người dùng. Ví dụ: **Cấu hình cho mô hình ghi nhớ toàn bộ dữ liệu lịch sử cá nhân của người dùng**. Khi AI có khả năng thấu hiểu sâu sắc các thói quen, lịch sử công việc và các mối quan tâm của bạn qua thời gian, bạn sẽ gặp rất nhiều khó khăn nếu muốn chuyển sang sử dụng mô hình của đối thủ khác do không muốn mất đi kho dữ liệu tích lũy đó.

## 豆包 MarsCode 系列活动

Doubao MarsCode là trợ lý lập trình thông minh ứng dụng mô hình ngôn ngữ lớn chuyên nghiệp do tập đoàn ByteDance phát triển.

Phối hợp cùng cộng đồng công nghệ Juejin (稀土掘金), trong tháng này Doubao MarsCode sẽ tổ chức chuỗi sự kiện hấp dẫn tại Thâm Quyến (ngày 14/12) và Thượng Hải (ngày 19/12) nhằm tạo không gian giao lưu và trải nghiệm lập trình AI thực tế cho các nhà phát triển.

(1) **Sự kiện "Doubao MarsCode Hands-on Lab" tại Thâm Quyến ngày 14 tháng 12.**

Các lập trình viên tham gia theo hình thức đội nhóm (tối đa 3 thành viên, hoặc có thể đăng ký thi đấu độc lập) sẽ **trực tiếp sử dụng trợ lý AI để lập trình và hoàn thiện một trò chơi nhỏ ngay tại sự kiện**. Đội ngũ kỹ sư của Doubao MarsCode sẽ túc trực hỗ trợ chuyên môn, giao lưu sâu sắc và đánh giá trao giải cho các sản phẩm xuất sắc nhất.

Đây là cơ hội tuyệt vời để trải nghiệm thực tế **cách thức ứng dụng AI để nhanh chóng hiện thực hóa các ý tưởng phần mềm**.

[Click vào đây](https://www.bagevent.com/event/8949689?bag_track=ryf) hoặc quét mã QR trên poster để xem chi tiết thể lệ và đăng ký tham dự.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120518.webp)

(2) **Giải đấu lập trình "Doubao MarsCode Coding Challenge" tại Thượng Hải ngày 19 tháng 12.**

Các thí sinh tham gia sẽ ứng dụng trợ lý AI để giải quyết nhanh 4 bài toán thuật toán trong khung thời gian quy định.

Đây là cơ hội rèn luyện tuyệt vời cho các kỳ thi tuyển dụng thực tế, đồng thời kết quả giải đấu cũng có thể làm phong phú thêm hồ sơ năng lực cá nhân của bạn. [Click vào đây](https://bytedance.larkoffice.com/docx/Sv8Cd8bCzoSlMax2DAscv5QLn9f) để xem chi tiết và đăng ký tham gia thử thách.

## 科技动态

1、[Máy tính cầm tay ứng dụng vi điều khiển Raspberry Pi](https://soulscircuit.com/pilet)

Một đội ngũ kỹ sư nước ngoài vừa giới thiệu nguyên mẫu máy tính cầm tay chạy trên bo mạch Raspberry Pi với thiết kế vô cùng ấn tượng.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120501.webp)

Thiết bị vận hành như một chiếc máy tính chạy hệ điều hành Linux hoàn chỉnh với thời lượng pin sử dụng liên tục đạt khoảng 7 giờ.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120502.webp)

Dự án còn cung cấp một phiên bản lắp ráp linh hoạt với phần màn hình hiển thị được thiết kế tách rời độc lập.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120505.webp)

Người dùng có thể dễ dàng ghép nối thiết bị với bàn phím mini hoặc tay cầm chơi game chuyên dụng.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120503.webp)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120504.webp)

Toàn bộ sơ đồ thiết kế của dự án được chia sẻ mã nguồn mở, đội ngũ phát triển kỳ vọng sẽ tối ưu hóa chi phí sản xuất thiết bị ở mức dưới 250 USD.

2、[Bồn tắm làm sạch bằng sóng siêu âm](https://www.core77.com/posts/134471/A-Washing-Machine-for-Human-Beings-from-1970)

Tại Hội chợ triển lãm thế giới Expo Osaka năm 1970, tập đoàn Sanyo từng gây chú ý lớn khi trưng bày nguyên mẫu bồn tắm làm sạch bằng sóng siêu âm chuyên dụng cho con người.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120513.webp)

Người dùng sẽ ngồi vào bên trong bồn chứa đầy nước ấm và chỉ chừa phần đầu lộ ra bên ngoài thiết bị.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120514.webp)

Khi khởi động, hệ thống sẽ phát ra các luồng sóng siêu âm tạo ra các rung động nước tần số cao để đánh bay mọi bụi bẩn trên cơ thể một cách nhẹ nhàng.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120515.webp)

Cơ chế vận hành của thiết bị hoàn toàn tương đồng với các dòng máy làm sạch bằng sóng siêu âm (như máy rửa kính mắt) phổ biến hiện nay, điểm khác biệt là nó được phóng to kích thước để phục vụ tắm rửa cho con người.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120516.webp)

Tuy nhiên, thiết bị độc đáo này chưa từng được đưa vào sản xuất thương mại thực tế tại thời điểm đó. Vào năm tới (2025), Osaka sẽ một lần nữa đăng cai tổ chức hội chợ triển lãm Expo. Một công ty công nghệ đã quyết định tái sản xuất và nâng cấp nguyên mẫu bồn tắm siêu âm này để ứng dụng chuyên biệt cho lĩnh vực y tế và chăm sóc sức khỏe người cao tuổi.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120517.webp)

3、[Mẫu giày co giãn điều chỉnh kích thước](https://www.yankodesign.com/2024/10/02/revolutionary-sneakers-expand-to-fit-your-growing-feet/)

Giày dép của trẻ em tuổi dậy thì thường chỉ có thể sử dụng trong vòng chưa đầy một năm là đã bị chật do bàn chân của trẻ phát triển rất nhanh.

Thấu hiểu điều đó, một doanh nghiệp Mỹ đã thiết kế dòng giày thể thao thông minh có khả năng tự co giãn kích thước theo sự phát triển của bàn chân.

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024100410.webp)

Giải pháp kỹ thuật của họ là chia phần đế giày làm hai phần độc lập và kết nối với nhau bằng một vật liệu polyme có tính đàn hồi cao.

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024100411.webp)

Khi bàn chân của trẻ phát triển dài ra, phần đế giày sẽ tự động được kéo giãn rộng ra tương ứng.

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024100412.webp)

![](https://cdn.beekka.com/blogimg/asset/202410/bg2024100413.webp)

Để bảo đảm trải nghiệm êm ái khi di chuyển, phần thân giày bên trên cũng sử dụng các sợi dệt co giãn tạo cấu trúc lưới thoáng khí ôm sát chân như một chiếc tất tiện lợi.

Ưu điểm lớn của mẫu giày này là giúp giảm thiểu tối đa việc phân chia kích cỡ giày (size) phức tạp, khi một đôi giày có thể ôm vừa vặn nhiều kích cỡ chân khác nhau.

4、**Các tin tức khác**

(1) Các kỹ sư của Samsung vừa chế tạo thành công một mẫu [robot hỗ trợ chụp ảnh tự động](https://spectrum.ieee.org/photo-robot). Người dùng chỉ cần mô tả phong cách bức ảnh mong muốn, robot sẽ tự động di chuyển chọn góc chụp và căn chỉnh tư thế tối ưu nhất để thực hiện chụp ảnh cho bạn.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120510.webp)

## 文章

1、[Tại sao chúng tôi quyết định chuyển dịch hệ thống sang Astro?](https://www.datocms.com/blog/why-we-switched-to-astro) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120507.webp)

Tác giả chia sẻ trải nghiệm thực tế của doanh nghiệp khi quyết định từ bỏ Next.js do mệt mỏi với các vấn đề phức tạp phát sinh của React/Next.js để chuyển dịch toàn bộ hệ thống trang web sang sử dụng Astro framework.

2、[Phiên bản Phoenix LiveView 1.0.0 chính thức ra mắt](https://www.phoenixframework.org/blog/phoenix-liveview-1.0-released) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120508.webp)

Phoenix LiveView là nền tảng phát triển ứng dụng web dựa trên ngôn ngữ Elixir, hướng tới mục tiêu cung cấp giải pháp lập trình đơn giản hơn nhưng vẫn đáp ứng đầy đủ các tính năng tương tác thời gian thực của React và hỗ trợ khả năng xử lý đồng thời cực cao. Bài viết giới thiệu chi tiết về bản cập nhật này.

3、[Cách tôi khai thác mạng Wi-Fi trên máy bay để xác định tọa độ bay](https://robertheaton.com/pymyflyspy/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120506.webp)

Tác giả chia sẻ thủ thuật lập trình khai thác luồng dữ liệu từ máy chủ nội bộ của hãng hàng không cung cấp trên mạng Wi-Fi chuyến bay để tự vẽ nên bản đồ đường bay thực tế của chiếc máy bay mình đang ngồi.

4、[Hướng dẫn cấu hình chuyển hướng liên kết (Redirect) miễn phí bằng Cloudflare](https://codethoughts.io/posts/2024-07-31-redirecting-urls-with-cloudflare/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202408/bg2024080407.webp)

Bài hướng dẫn chi tiết cách cấu hình dịch vụ DNS Cloudflare để tự động chuyển hướng toàn bộ lưu lượng từ tên miền cũ sang tên miền mới hoàn toàn miễn phí khi thay đổi tên miền website.

5、[Khuyến nghị: Không sử dụng hàm COUNT(*) so sánh với số 0 trong SQL](https://www.depesz.com/2024/12/01/sql-best-practices-dont-compare-count-with-0/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120509.webp)

Bài viết phân tích các nguyên lý tối ưu hóa câu lệnh SQL, khuyến nghị các nhà phát triển không nên sử dụng cú pháp so sánh kết quả phép đếm `COUNT(*) = 0` chỉ để kiểm tra xem một bảng dữ liệu có tồn tại bản ghi thỏa mãn điều kiện hay không nhằm tránh gây quá tải hệ thống.

6、[Hướng dẫn cấu hình mở khóa máy tính Windows bằng cảm biến vân tay điện thoại](https://www.xda-developers.com/unlock-windows-pc-fingerprint-scanner-android/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120511.webp)

Hệ điều hành Windows 11 hỗ trợ tính năng kết nối bảo mật cho phép người dùng khai thác cảm biến vân tay hoặc nhận diện khuôn mặt trên điện thoại di động Android để mở khóa máy tính từ xa.

7、[Hướng dẫn cài đặt phpMyAdmin bằng công cụ Docker Compose](https://linuxiac.com/how-to-install-phpmyadmin-with-docker-compose/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202409/bg2024090702.webp)

Bài viết hướng dẫn cơ bản dành cho lập trình viên mới bắt đầu cách viết tệp cấu hình Docker Compose để nhanh chóng triển khai một ứng dụng quản trị cơ sở dữ liệu MySQL trên môi trường máy cục bộ.

## 工具

1、[Bananas](https://github.com/mistweaverco/bananas)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120512.webp)

Ứng dụng chia sẻ màn hình máy tính đa nền tảng hoạt động trên giao thức kết nối ngang hàng (Peer-to-Peer), không yêu cầu người dùng phải đăng ký tài khoản hay phụ thuộc vào bất kỳ máy chủ trung gian nào (ngoại trừ quá trình thiết lập kết nối ban đầu).

2、[jsontr.ee](https://github.com/xzitlou/jsontr.ee)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112806.webp)

Thư viện JavaScript gọn nhẹ hỗ trợ tự động phân tích cú pháp và trực quan hóa các chuỗi dữ liệu định dạng JSON dưới dạng sơ đồ hình cây trực quan.

3、[WatchAlert](https://github.com/opsre/WatchAlert)

Hệ thống giám sát hệ thống và cảnh báo lỗi gọn nhẹ nguồn mở được phát triển bằng ngôn ngữ Go kết hợp giao diện React. (Đóng góp từ [@Cairry](https://github.com/ruanyf/weekly/issues/5627))

4、[Easy Resizer](https://easyresizer.com)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120201.webp)

Công cụ trực tuyến hỗ trợ người dùng nhanh chóng điều chỉnh kích thước (resize) hình ảnh hàng loạt tiện lợi. (Đóng góp từ [@mywebtools](https://github.com/ruanyf/weekly/issues/5612))

5、[IconEase](https://github.com/JiuRanYa/IconEase)

Ứng dụng máy tính đa nền tảng mã nguồn mở chuyên dụng hỗ trợ quản lý, tìm kiếm và phân loại các tệp tin icon hệ thống lưu trữ cục bộ. (Đóng góp từ [@JiuRanYa](https://github.com/ruanyf/weekly/issues/5644))

6、[X.Ryder](https://github.com/pipijoe/xryder-web)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120402.webp)

Bộ giao diện (template) mẫu thiết kế giao diện quản trị (admin dashboard) đẹp mắt dành cho các dự án Web. (Đóng góp từ [@pipijoe](https://github.com/ruanyf/weekly/issues/5639))

7、[Peninsula](https://github.com/Celve/Peninsula)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120404.webp)

Ứng dụng quản trị cửa sổ làm việc và trung tâm thông báo độc đáo dành cho các dòng máy Mac, được thiết kế tận dụng tối ưu không gian hiển thị xung quanh khu vực "tai thỏ" (notch) màn hình. (Đóng góp từ [@Celve](https://github.com/ruanyf/weekly/issues/5641))

8、[Summary Cat](https://www.summarycat.com/)

Ứng dụng web hữu ích ứng dụng trí tuệ nhân tạo để tự động tóm tắt nội dung chính của một video YouTube bất kỳ thông qua liên kết người dùng cung cấp.

9、[ubicloud](https://www.ubicloud.com/use-cases/github-actions)

Giải pháp điện toán đám mây mã nguồn mở cho phép người dùng tự triển khai một môi trường máy chủ riêng biệt để thực thi trực tiếp các kịch bản tự động hóa GitHub Actions.

10、[matcha.css](https://matcha.mizu.sh/)

Thư viện CSS tối giản không yêu cầu thiết lập class, giúp tự động tối ưu hóa và làm đẹp giao diện hiển thị mặc định của các thẻ HTML cơ bản trên trình duyệt.

## AI 相关

1、[Bylo.ai](https://bylo.ai)

Dịch vụ web hỗ trợ tạo ảnh nghệ thuật bằng trí tuệ nhân tạo (AI Image Generator) hoàn toàn miễn phí. (Đóng góp từ [@aaamomo64](https://github.com/ruanyf/weekly/issues/5630))

2、[Color Diffusion](https://github.com/ErwannMillon/Color-diffusion)

Chương trình Python mã nguồn mở ứng dụng mô hình AI khuếch tán (Diffusion Model) để tự động phục chế màu sắc cho các bức ảnh đen trắng cổ xưa.

3、[Onion AI (Bộ công cụ tìm kiếm AI tổng hợp)](https://onionai.so)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120202.webp)

Trang web tổng hợp cổng kết nối với nhiều công cụ tìm kiếm AI phổ biến hiện nay, cho phép người dùng dễ dàng chuyển đổi qua lại giữa các công cụ để so sánh kết quả tìm kiếm. (Đóng góp từ [@ovelv](https://github.com/ruanyf/weekly/issues/5616))

## 资源

1、[Hi Speaking](https://hispeaking.com/)

Trang web hỗ trợ luyện nói tiếng Anh giao tiếp trực tuyến tiện lợi. Hệ thống tích hợp tính năng tự động chuyển câu bài học tiếp theo ngay sau khi ghi âm xong câu trước mà không yêu cầu người dùng phải click chuột thủ công. (Đóng góp từ [@jiweiyuan](https://github.com/ruanyf/weekly/issues/5625))

2][In Pieces - Trực quan hóa 30 loài động vật có nguy cơ tuyệt chủng](http://www.species-in-pieces.com/#)

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110515.webp)

Một dự án thiết kế web đầy tính sáng tạo nghệ thuật, ứng dụng các thuộc tính CSS nâng cao để ghép nối các đa giác tạo hình 30 loài động vật quý hiếm đang có nguy cơ tuyệt chủng trên thế giới.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024110516.webp)

3、[Thư mục phân loại các giải pháp trực quan hóa dữ liệu](https://datavizcatalogue.com/search.html)

Trang web chuyên tổng hợp và phân loại các dạng biểu đồ hiển thị số liệu dựa trên các mục đích truyền tải thông tin khác nhau, giúp các nhà thiết kế dễ dàng lựa chọn loại biểu đồ phù hợp nhất.

## 图片

1、[Phân tích thiết kế giao diện từ các mô hình Lego](https://interactionmagic.com/UX-LEGO-Interfaces/)

Các bộ lắp ráp Lego chủ đề máy móc hoặc tàu vũ trụ thường đi kèm rất nhiều chi tiết bảng điều khiển (control panels) với đa dạng phong cách thiết kế giao diện.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112903.webp)

Việc phân tích các thiết kế này sẽ mang lại nhiều bài học bổ ích về cách thức thiết kế giao diện người dùng (UI/UX) trực quan trong thực tế.

Dưới đây là một ví dụ về phong cách thiết kế UI tồi, khi các nút bấm được sắp xếp lộn xộn khiến người vận hành rất khó phân biệt nút nào điều khiển tính năng nào.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112904.webp)

Nếu chúng ta thực hiện phân nhóm các nút bấm có tính năng tương đồng lại với nhau thành các khu vực riêng biệt, độ nhận diện của bảng điều khiển sẽ được cải thiện rõ rệt.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112905.webp)

Trong số các phương án trên, thiết kế ở góc ngoài cùng bên phải được đánh giá là cho khả năng nhận diện tốt nhất.

Dưới đây là ba mẫu thiết kế bảng điều khiển Lego được đánh giá là xuất sắc nhất nhờ phong cách thiết kế tối giản, sạch sẽ và tích hợp các yếu tố chỉ thị trực quan cao.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112906.webp)

2、[Tại sao những người trong các bức ảnh chụp thời xưa thường không mỉm cười?](https://www.upworthy.com/why-didn-t-people-smile-in-old-photographs-it-wasn-t-just-about-the-long-exposure-times)

Trong các bức ảnh chụp chân dung từ cuối thế kỷ 19 và đầu thế kỷ 20, chúng ta thường thấy nét mặt của những người trong ảnh vô cùng nghiêm nghị và hầu như không nở một nụ cười nào.

![](https://cdn.beekka.com/blogimg/asset/202411/bg2024112803.webp)

Nguyên nhân kỹ thuật cốt lõi là do công nghệ máy ảnh thời kỳ đó yêu cầu thời gian phơi sáng cực kỳ dài. Để hoàn thành một bức ảnh chụp, người mẫu bắt buộc phải ngồi bất động hoàn toàn trước ống kính trong khoảng thời gian kéo dài vài phút.

Nụ cười vốn là một phản ứng biểu cảm tức thời của cơ mặt và rất khó để duy trì liên tục trong thời gian dài. Khi bạn buộc phải ngồi im thin thít suốt nhiều phút để chụp ảnh, việc cố gắng giữ cơ mặt mỉm cười liên tục là điều hầu như không thể thực hiện được.

## 文摘

1、[Mối liên hệ giữa nhịp tim và tuổi thọ của các loài động vật](https://kottke.org//13/02/does-every-species-get-a-billion-heartbeats-per-lifetime)

Tại sao các loài động vật có kích thước cơ thể càng lớn thì nhịp tim của chúng lại càng có xu hướng đập chậm hơn?

Số liệu thống kê cho thấy nhịp tim trung bình mỗi phút của chuột hamster là 450 lần, của mèo là 150 lần, của lợn là 70 lần, của voi là 30 lần và của cá voi chỉ vỏn vẹn 20 lần.

Nguyên lý sinh học này có thể được giải thích như sau: Giả sử kích thước cơ thể của mèo lớn gấp 10 lần chuột hamster, thì về mặt lý thuyết tốc độ trao đổi chất (mức độ đốt cháy năng lượng để duy trì sự sống) của mèo cũng phải lớn gấp 10 lần hamster do cơ thể mèo sở hữu số lượng tế bào tiêu thụ năng lượng nhiều gấp 10 lần.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024120406.webp)

Tuy nhiên, điều này là bất khả thi trên thực tế. Nếu tốc độ trao đổi chất tăng tuyến tính như vậy, chú mèo sẽ nhanh chóng bị tử vong do thân nhiệt tăng cao quá mức. Quá trình trao đổi chất luôn sinh ra nhiệt năng và yêu cầu cơ thể phải tỏa nhiệt ra môi trường. Nhưng diện tích bề mặt cơ thể của mèo hoàn toàn không lớn gấp 10 lần so với hamster, dẫn đến một lượng lớn nhiệt năng bị giữ lại bên trong cơ thể gây quá nhiệt.

Tại sao diện tích bề mặt cơ thể của loài vật lớn lại không tăng tương ứng với thể tích?

Nguyên lý toán học cơ bản chỉ ra tốc độ tăng trưởng của diện tích bề mặt luôn chậm hơn tốc độ tăng trưởng của thể tích. Ví dụ: Khi thể tích của một hình cầu tăng gấp đôi (200%), thì diện tích bề mặt của nó chỉ tăng khoảng 1,59 lần (159%).

Do không thể tỏa hết nhiệt năng ra ngoài, các loài động vật lớn buộc phải tiến hóa để giảm tốc độ trao đổi chất thấp hơn so với các loài động vật nhỏ. Biểu hiện trực quan nhất của cơ chế tự bảo vệ này chính là việc nhịp tim của thú lớn đập chậm đi đáng kể để giảm cường độ trao đổi chất.

Các nhà động vật học còn phát hiện ra một quy luật tự nhiên vô cùng thú vị: Đại đa số các loài động vật có vú, bất kể kích thước lớn nhỏ ra sao, đều sở hữu tổng số nhịp tim trong suốt cuộc đời dao động ở con số khoảng **1 tỷ lần**.

Vòng đời trung bình của chuột hamster là 3 năm, của mèo là 15 năm, của lợn là 25 năm, của voi là 70 năm và của cá voi là 80 năm.

Nếu đem nhân nhịp tim trung bình với thời gian sống, chúng ta sẽ thu được tổng số nhịp tim cả đời của chuột hamster là khoảng 710 triệu lần, của mèo là 1,18 tỷ lần, của lợn là 920 triệu lần, của voi là 1,1 tỷ lần và của cá voi là 840 triệu lần.

Tất cả các số liệu này đều xoay quanh mốc giới hạn 1 tỷ nhịp tim.

Điều kỳ lạ là con người là loài duy nhất nằm ngoài quy luật tự nhiên này. Với nhịp tim trung bình 60 lần/phút và tuổi thọ bình quân 70 năm, tổng số nhịp tim cả đời của một người đạt tới **2,21 tỷ lần** — gấp đôi so với các loài động vật có vú khác.

## 言论

1、

Chính phủ El Salvador hiện đang nắm giữ khoảng 5.940 Bitcoin làm tài sản dự trữ quốc gia, tương đương giá trị khoảng 582 triệu USD.

Tuy nhiên, câu hỏi đặt ra là làm thế nào họ bảo mật và lưu trữ an toàn các mã khóa cá nhân (private keys) của ví tiền này? Chỉ cần một sự cố rò rỉ mã khóa xảy ra, toàn bộ nền tài chính quốc gia sẽ lập tức đối mặt với nguy cơ phá sản.

-- [Ý kiến độc giả trên diễn đàn Hacker News](https://news.ycombinator.com/item?id=42285619)

2、

Vào giai đoạn đầu, triết gia người Đức thế kỷ 19 Friedrich Nietzsche thường viết sách với phong cách hành văn chứa các câu văn dài phức tạp, đi kèm các lập luận và diễn giải vô cùng rối rắm.

Tuy nhiên, kể từ khi chuyển sang sử dụng máy đánh chữ để soạn thảo văn bản, phong cách hành văn của ông đã có sự chuyển dịch rõ rệt: Các câu văn dài được thay thế bằng những câu châm ngôn ngắn gọn, cô đọng và súc tích giống như các bức điện tín.

-- [《Chi tiết cách chiếc máy đánh chữ làm thay đổi tư duy viết lách của Nietzsche》](https://thereader.mitpress.mit.edu/how-typing-transformed-nietzsches-consciousness/)

3、

Hiệu ứng nền tảng nội bộ (Inner-platform effect) là thuật ngữ dùng để chỉ xu hướng của các kỹ sư phần mềm khi cố gắng tự phát triển một hệ thống quản lý nội bộ có thể tùy biến sâu, nhưng vô tình hệ thống đó lại trở thành một bản sao chép tồi tệ của chính phần mềm hệ thống bên ngoài mà họ đang sử dụng.

-- [Wikipedia](https://en.wikipedia.org/wiki/Inner-platform_effect)

4Roll

Tôi luôn dành tình cảm yêu mến đặc biệt cho những con người luôn khao khát chinh phục những điều không thể.

—— [Johann Wolfgang von Goethe](https://boehs.org/node/dark-web-security)

5、

Tôi vốn là người rất e ngại việc đưa ra các dự báo về xu hướng công nghệ tương lai. Tuy nhiên, đứng trước năng lực viết lách cực kỳ xuất sắc của các mô hình AI hiện nay, tôi hoàn toàn tự tin đưa ra dự báo rằng: Chỉ trong vòng vài thập kỷ tới, số lượng con người thực sự sở hữu kỹ năng tự viết văn bản chất lượng chắc chắn sẽ còn lại rất ít.

-- [Paul Graham](https://paulgraham.com/writes.html), *Nhà đồng sáng lập quỹ đầu tư Y Combinator*

## 往年回顾

[Bàn về việc lựa chọn giải pháp phát triển cơ sở hạ tầng thông tin thế hệ mới](https://www.ruanyifeng.com/blog/2023/12/weekly-issue-281.html) (2023 #281)

[Khảo sát quy mô nhân sự tối ưu cho hoạt động của các doanh nghiệp Internet](https://www.ruanyifeng.com/blog/2022/11/weekly-issue-231.html) (2022 #231)

[Bàn về triết lý thiết kế và trải nghiệm của các giải pháp thanh toán di động](https://www.ruanyifeng.com/blog/2021/10/weekly-issue-181.html) (2021 #181)

[Tư duy phân tích của bạn đang vận hành theo logic nhị phân hay logic tam phân?](https://www.ruanyifeng.com/blog/2020/10/weekly-issue-131.html) (2020 #131)

(Hết)
