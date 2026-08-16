# Bản tin chia sẻ công nghệ (Số 278): Vấn đề bản quyền AI hóc búa

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3599) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111405.webp)

Trạm Kê Minh nằm ở Trương Gia Khẩu, Hà Bắc, là di tích trạm dịch cổ lớn nhất hiện còn tồn tại ở Trung Quốc, nơi các sứ giả đưa thư thời xưa nghỉ ngơi và thay ngựa. (Nguồn: [Baidu Baike](https://baike.baidu.com/item/%E9%B8%A1%E9%B8%A3%E5%B3%84/8364068))

## 棘手的 AI 版权

AI là một thứ mới mẻ, mang lại nhiều vấn đề chưa từng có tiền lệ.

Hóc búa nhất, gây tranh cãi nhất và cũng thú vị nhất có lẽ chính là vấn đề bản quyền.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111103.webp)

Cụ thể, đó là câu hỏi dưới đây: **Khi huấn luyện (học tập), AI có được phép sử dụng các tài liệu có bản quyền, để từ đó sở hữu năng lực bắt chước chính chủ sở hữu bản quyền đó hay không?**

Ví dụ, cách đây một thời gian, trên mạng xuất hiện trào lưu "[AI Stefanie Sun](https://www.stcn.com/article/detail/872694.html)" (AI Tôn Yến Tư). Có người đã sử dụng các ca khúc của Tôn Yến Tư làm tài liệu huấn luyện, giúp AI bắt chước giọng hát của cô để trình bày các ca khúc của các ca sĩ khác.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111102.webp)

Tôi muốn hỏi mọi người, việc này có xâm phạm bản quyền của Tôn Yến Tư hay không?

Một luồng quan điểm cho rằng đây là hành vi xâm phạm bản quyền, bởi vì **giọng hát của Tôn Yến Tư đã bị bắt chước khi chưa được sự cho phép**. Nếu dung túng cho AI bắt chước giọng ca sĩ, khi người thật còn chưa hát thì AI đã hát trước rồi, sau này ai còn bỏ tiền ra nghe ca sĩ thật hát nữa?

Luồng quan điểm ngược lại cho rằng không hề xâm phạm bản quyền, bởi vì **AI chỉ đang học tập giọng hát của Tôn Yến Tư chứ không phải sao chép trực tiếp**. Bài hát mà AI thể hiện là bài hát chính chủ chưa từng hát, đây thuộc về sự sáng tạo của AI, do đó không tồn tại hành vi xâm phạm bản quyền.

Bạn đồng tình với quan điểm nào?

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111104.webp)

Điểm thú vị của vấn đề này là nếu thay thế AI bằng con người, tranh chấp sẽ lập tức biến mất.

Giả sử có một cô bé khổ luyện bắt chước giọng hát của Tôn Yến Tư, và cuối cùng cũng có thể hát với chất giọng y hệt. Vậy cô bé đó có xâm phạm bản quyền của Tôn Yến Tư không?

Tôi tin rằng tất cả mọi người đều đồng ý rằng đây không phải hành vi xâm phạm. **Một người bắt chước các đặc điểm của một người khác không hề xâm phạm bản quyền của người đó.**

Tôi bắt chước phong cách vẽ tranh của Van Gogh, bắt chước phong cách viết văn của Lỗ Tấn, hay bắt chước phong cách lập trình của những lập trình viên xuất sắc nhất đến mức có thể làm giả như thật. Chỉ cần tác phẩm tôi tạo ra là của riêng tôi, thì đó đều là những hành vi hoàn toàn hợp pháp. **Vậy tại sao khi AI làm điều tương tự, nó lại bị coi là xâm phạm bản quyền?**

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111105.webp)

Tuy nhiên, chúng ta cũng không thể hoàn toàn đồng nhất AI với con người. Có hàng ngàn họa sĩ bắt chước Van Gogh và điều đó không hề ảnh hưởng đến giá trị của tranh Van Gogh thật, nhưng với AI thì chưa chắc.

If cho phép "AI Tôn Yến Tư" và "Tôn Yến Tư thật" cùng tồn tại, rất có thể sẽ ảnh hưởng nghiêm trọng đến thu nhập của ca sĩ thật. Liệu mọi người có còn bỏ tiền ra mua nhạc của Tôn Yến Tư nữa hay không, điều đó thực sự khó nói.

Đây chính là điểm tiến thoái lưỡng nan. Nếu chúng ta quy định việc AI bắt chước không phải là xâm phạm bản quyền, chúng ta không biết hậu quả sẽ ra sao, liệu các tài sản bản quyền hiện tại có bị mất giá thê thảm hay không.

Hơn nữa, đối tượng chịu tác động lớn nhất từ AI không phải những người đã nổi tiếng, mà là những người lao động bình dân ở tầng đáy. Thử tưởng tượng, nếu không có sự bảo hộ bản quyền, hãng phim chỉ cần thuê diễn viên quần chúng trong một ngày, dùng AI học tập kỹ lưỡng mọi cử chỉ của họ, sau đó có thể vô hạn sử dụng "phân thân AI" của họ (chỉ cần chỉnh sửa lại khuôn mặt) mà không bao giờ cần thuê họ làm việc nữa.

Tóm lại, bản quyền AI là một vấn đề cực kỳ rắc rối. **Bản quyền bảo hộ "quyền sao chép" (Right to copy), nhưng AI lại liên quan đến "quyền học tập" (Right to learn)**. Nếu cấm quyền học tập của AI, điều đó tương đương với việc tuyên bố có những việc chỉ con người được làm còn máy móc thì không, điều này rất thiếu thuyết phục và cực kỳ khó thực hiện trong thực tế. Nhưng nếu không cấm, nó có thể ảnh hưởng trực tiếp đến sinh kế của những người sở hữu bản quyền.

Ngoài ra, bên cạnh việc bắt chước phong cách cá nhân, việc tóm tắt nội dung cũng gặp tình trạng tương tự. Bạn đọc xong một cuốn tiểu thuyết (hoặc xem xong một bộ phim) và kể lại cốt truyện cho bạn bè nghe, điều đó hoàn toàn hợp pháp. Nhưng liệu AI có được phép làm điều đó không – kiểu "tóm tắt nhanh nội dung tiểu thuyết trong 10 phút"? Chúng ta cũng có thể suy nghĩ về vấn đề này dưới cùng một góc nhìn.

## [本周软件] TGFX：强大易用的 2D 图形库

Tuần này, tôi muốn giới thiệu tới mọi người một công cụ phần mềm tương đối quan trọng.

Nó là thành phần cốt lõi trong nhiều mảng dịch vụ hàng đầu tại Trung Quốc, mới chỉ được mở nguồn mở gần đây nên chưa có nhiều người biết đến. Đó chính là [thư viện đồ họa 2D TGFX](https://github.com/Tencent/tgfx) của Tencent.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111402.webp)

Nhiều bạn có thể chưa rõ thư viện đồ họa dùng để làm gì và tại sao nó lại quan trọng?

Mỗi ngày chúng ta sử dụng máy tính (bao gồm cả điện thoại di động) đều tiếp xúc với giao diện đồ họa. Những thành phần giao diện đẹp mắt đó đều phụ thuộc vào thư viện đồ họa. Bản chất máy tính chỉ là một công cụ tính toán và chỉ biết tính toán. **Nếu muốn có giao diện đồ họa, bạn bắt buộc phải gọi đến các thư viện đồ họa chuyên dụng** để có được khả năng hiển thị đồ họa.

Thư viện đồ họa thông thường do hệ điều hành cung cấp. Tuy nhiên, nếu phần mềm cần chạy đa nền tảng hoặc yêu cầu các hiệu ứng đặc biệt, họ bắt buộc phải sử dụng thư viện đồ họa bên ngoài. Hiện nay, thư viện đồ họa 2D đa dụng phổ biến nhất là Skia của Google. Đây là thư viện nguồn mở được sử dụng trong trình duyệt Chrome, hệ điều hành Android, Google Maps, v.v.

**Mục tiêu phát triển của TGFX là để thay thế Skia.** Nó có nguồn gốc từ [giải pháp hiệu ứng động PAG](https://pag.art/) của Tencent. Vào thời điểm đó, rất nhiều dự án nội bộ của Tencent có nhu cầu rất lớn về hiệu ứng hoạt họa và yêu cầu chạy đa nền tảng, do đó PAG ra đời như một công cụ chuyên biệt để tạo hiệu ứng động.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111403.webp)

Phần cốt lõi của PAG chính là thư viện đồ họa. Ban đầu họ sử dụng Skia, nhưng sau đó phát hiện ra hai vấn đề lớn: Thứ nhất, Skia có gánh nặng lịch sử lớn khiến dung lượng bộ thư viện khi đóng gói rất nặng, và hiệu năng cũng tương đối bảo thủ; Thứ hai, các nhà phát triển Trung Quốc thường quan tâm đến một số vấn đề đặc thù mà đội ngũ phát triển gốc của Skia không thể (hoặc không muốn) hỗ trợ giải quyết.

Cuối cùng, **đội ngũ PAG đã quyết định thay thế Skia để tự phát triển thư viện đồ họa riêng mang tên TGFX.** Đây là một nhiệm vụ cực kỳ khó khăn khi phải viết hoàn toàn bằng C++, tương thích với các cổng đồ họa của nhiều hệ điều hành khác nhau (hiện tại chủ yếu là OpenGL), dựng được nhiều loại hình dạng đồ họa và bảo đảm hiệu năng cũng như hiệu ứng hiển thị tốt. Họ bắt đầu làm từ năm 2021 và phải đến năm nay mới đạt được những thành tựu nhất định. TGFX sở hữu một vài đặc điểm nổi bật sau:

> (1) Tận dụng tối đa khả năng tính toán của các dòng GPU hiện đại để bảo đảm hiệu năng.
> 
> (2) Cung cấp khả năng xử lý đồ họa toàn diện: Hỗ trợ đầy đủ việc vẽ 2D cho các loại hình ảnh, vector và văn bản.
> 
> (3) Là giải pháp thay thế gọn nhẹ cho Skia: Dung lượng đóng gói chỉ khoảng 400KB, nhưng thực hiện được hầu hết các tính năng của bộ Skia nặng 2MB.
> 
> (4) Chi phí sử dụng thấp: Giao diện API cơ bản tương đồng với Skia, đồng thời được đơn giản hóa và tích hợp tốt hơn.

Sau khi PAG 4.0 chuyển đổi công cụ đồ họa từ Skia sang TGFX, dung lượng gói thư viện đã giảm 65% và hiệu năng dựng hình vector tăng 60%.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111110.webp)

Tính đến tháng 7 năm 2023, thông qua dự án PAG, TGFX đã chạy trên **hơn 1000 dịch vụ hàng đầu tại Trung Quốc**, bao gồm các ứng dụng lớn của Tencent như WeChat, QQ di động, Vương Giả Vinh Diệu, cũng như các dự án bên ngoài như Xiaohongshu, Zhihu, Bilibili... Độ ổn định của thư viện đã được xác minh trên hơn 1 tỷ thiết bị người dùng, hiệu năng thực tế cũng rất đáng nể, ví dụ giúp Tencent Docs giảm tới 50% lượng bộ nhớ tiêu thụ.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111404.webp)

TGFX trước đây là một phần của dự án PAG, gần đây mới được tách ra thành một dự án mã nguồn mở độc lập trên [GitHub](https://github.com/Tencent/tgfx). Nếu dự án của bạn cần một công cụ xử lý đồ họa, hãy thử trải nghiệm nó.

Dự án này mới chỉ bắt đầu mở nguồn mở, và Tencent sẽ tiếp tục đầu tư mạnh mẽ lâu dài vào nó. Những bạn đọc quan tâm đến lập trình đồ họa có thể tìm hiểu mã nguồn và tài liệu của dự án này, tin rằng bạn sẽ học hỏi được rất nhiều điều bổ ích. Mọi ý kiến đóng góp hay phản hồi đều được đội ngũ phát triển phản hồi và xử lý nhanh chóng.

## 科技动态

1、[Thiết bị đeo AI Pin](https://hu.ma.ne/)

Tuần trước, thiết bị AI đeo người đầu tiên trên thế giới đã được mở bán tại Mỹ với tên gọi AI Pin.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111001.webp)

Nó có thể được cài lên áo giống như một chiếc huy hiệu, bản thân cái tên Pin cũng mang ý nghĩa là "chiếc ghim cài".

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111003.webp)

Hệ thống chạy trên nền tảng Android, kết nối mạng thông qua thẻ SIM di động. Thiết bị tích hợp micro, loa và camera để người dùng có thể đối thoại trực tiếp với nó.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111004.webp)

Ví dụ, khi nhìn thấy một quả thanh long, bạn có thể hỏi nó: "Trái này chứa bao nhiêu đường?" Nó sẽ lập tức trả lời: "Toàn bộ quả chứa khoảng 7,31 gram đường."

Sau này nếu thấy ai đó tự nói chuyện một mình trên phố, bạn đừng quá ngạc nhiên, có thể họ đang trò chuyện với AI.

Bên cạnh việc điều khiển bằng giọng nói, thiết bị cũng hỗ trợ các thao tác chạm cảm ứng và chiếu giao diện lên lòng bàn tay.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111005.webp)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111006.webp)

Thiết bị có giá bán 699 USD (khoảng 17 triệu đồng), kèm theo phí dịch vụ hàng tháng là 24 USD (khoảng 600.000 đồng). Với mức giá đắt đỏ này cùng tính năng chưa vượt trội so với điện thoại thông minh, triển vọng doanh số của sản phẩm này khá mờ mịt và gần như chắc chắn sẽ thất bại.

2、[Tàu bay khổng lồ Pathfinder 1](https://techcrunch.com/2023/11/08/the-worlds-largest-aircraft-breaks-cover-in-silicon-valley/)

Vào ngày 8 tháng 11, phương tiện bay lớn nhất thế giới hiện nay mang tên Pathfinder 1 (探路者1号) đã thực hiện chuyến bay thử nghiệm đầu tiên. Đây là dự án được tài trợ bởi nhà đồng sáng lập Google Sergey Brin.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111007.webp)

Chiều dài của tàu bay lên tới 124,5 mét, dài hơn cả ba chiếc máy bay Boeing 737 Max xếp liền nhau.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111008.webp)

Nó được điều khiển bằng động cơ điện, bên trong chứa 13 túi khí heli, phần khung xương được chế tạo từ sợi carbon và kim loại titan, lớp vỏ ngoài cũng được phủ một lớp chống cháy đặc biệt, nhìn chung có độ an toàn rất cao.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111009.webp)

Toàn bộ phi hành đoàn và hành khách sẽ ngồi ở khoang hành khách phía dưới (căn phòng nhỏ dưới đáy tàu bay trong ảnh trên). Khoang này khá nhỏ, chỉ chở tối đa 14 người mỗi chuyến, với tải trọng từ 2 đến 5 tấn.

Ưu điểm của tàu bay là bay chậm ở tầm thấp, có thể bay treo tại chỗ và hoạt động cực kỳ yên tĩnh. Tuy nhiên, với sức chứa nhỏ và khả năng chống gió bão kém, sản phẩm này khó có thể ứng dụng rộng rãi vào thực tế.

3、[Ca ghép toàn bộ mắt đầu tiên trên thế giới](https://www.scientificamerican.com/article/doctors-complete-first-successful-face-and-whole-eye-transplant/)

Tuần trước, một bệnh viện ở New York thông báo đã thực hiện thành công ca phẫu thuật ghép toàn bộ mắt đầu tiên trên thế giới vào ngày 27 tháng 5 năm nay. Việc cấy ghép nhãn cầu của người này sang người khác quả là một thành tựu y học gây chấn động.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111010.webp)

Bệnh nhân là một người đàn ông 46 tuổi, bị hỏng mắt trái do tai nạn bỏng điện nghiêm trọng.

Năm tháng sau ca ghép, mắt của anh vẫn chưa phục hồi thị lực, nhưng não bộ đã có thể cảm nhận được các tín hiệu thần kinh từ mắt được ghép, đồng thời các mạch máu vẫn lưu thông bình thường. Các bác sĩ đánh giá ca phẫu thuật đã thành công bước đầu, và đang chờ các dây thần kinh tiếp tục phát triển để xem liệu thị lực có thể được khôi phục hay không.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111011.webp)

Mặc dù loại phẫu thuật này đã được thực hiện nhiều lần trên động vật, mắt người tinh vi và phức tạp hơn rất nhiều. Trước khi phẫu thuật, các bác sĩ phải sử dụng mô phỏng 3D trên máy tính để căn chỉnh chính xác vị trí xương và nhãn cầu cấy ghép (hình trên).

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111012.webp)

Toàn bộ ca phẫu thuật kéo dài liên tục trong 21 giờ, với sự tham gia của hơn 140 y bác sĩ và nhân viên hỗ trợ (hình trên).

Nếu ca phẫu thuật này có thể phục hồi thị lực thành công, đây sẽ là một tin vui vô cùng lớn cho những người bị mù do chấn thương ngoại lực.

4、[Ý tưởng quảng cáo độc đáo của Steam Deck](https://idlethumbs.social/@ja2ke/111396017651485944)

Hãng Valve chuẩn bị mở bán phiên bản mới của máy chơi game cầm tay Steam Deck mang tên "Steam Deck OLED". Điểm nhấn lớn nhất của phiên bản này là màn hình OLED có độ sáng cao hơn rõ rệt.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111313.webp)

Để làm nổi bật ưu điểm này, họ đã nghĩ ra một ý tưởng quảng cáo độc đáo: dùng chính ánh sáng phát ra từ các máy Steam Deck OLED để tự chiếu sáng.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111308.webp)

Hình ảnh trên là ảnh chụp từ video quảng cáo, chiếc Steam Deck OLED ở trung tâm được chiếu sáng hoàn toàn bởi nguồn sáng phát ra từ những chiếc Steam Deck OLED xung quanh.

Để thực hiện được hiệu ứng này, họ đã chế tạo một quả cầu kim loại khổng lồ và treo rất nhiều máy chơi game lên đó.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111309.webp)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111310.webp)

Đồng thời, họ sử dụng phần mềm để đồng bộ hóa nội dung hiển thị trên toàn bộ các màn hình, và nhiếp ảnh gia sẽ đứng bên trong quả cầu để thực hiện việc bấm máy.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111311.webp)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111312.webp)

## Bài viết

1\. [Làm thế nào để phát hành một gói thư viện TypeScript?](https://blog.liblab.com/typescript-npm-packages-done-right/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092501.webp)

Bài viết hướng dẫn chi tiết quy trình đóng gói và phát hành một thư viện được viết bằng ngôn ngữ TypeScript lên kho lưu trữ npm.

2\. [Kiến thức cơ bản về Fiber trong C++](https://agraphicsguynotes.com/posts/fiber_in_cpp_understanding_the_basics/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092502.webp)

Thư viện React có giới thiệu khái niệm Fiber, vậy thuật ngữ này thực chất có ý nghĩa gì? Nó vốn có nguồn gốc từ ngôn ngữ C++, bài viết giới thiệu những kiến thức cơ bản về Fiber trong C++ với các phần giải thích rất dễ hiểu.

3\. [Đoạn mã StackOverflow được sao chép nhiều nhất thế giới](https://programming.guide/worlds-most-copied-so-snippet.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092808.webp)

Đâu là đoạn mã nguồn được nhiều lập trình viên copy nhất trên trang hỏi đáp StackOverflow? Bài viết sẽ tiết lộ câu trả lời và chỉ ra một lỗi sai nhỏ vẫn tồn tại trong đoạn mã kinh điển này.

4\. [Cách hiện thực hóa các đối tượng kéo thả trên trang web](https://www.redblobgames.com/making-of/draggable/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023093006.webp)

Tác giả hướng dẫn chi tiết cách viết code để tạo ra các đối tượng có thể kéo thả trên giao diện web, tương thích tốt với cả thao tác chuột và cảm ứng tay.

5\. [Tự động co giãn chiều cao của thẻ textarea bằng CSS](https://www.amitmerchant.com/textarea-auto-increase-height/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100102.webp)

Làm thế nào để khung nhập văn bản (textarea) trên trang web tự động tăng chiều cao khi người dùng gõ thêm nhiều dòng chữ mà không cần dùng đến JavaScript? Bài viết hướng dẫn cách thực hiện chỉ bằng CSS.

6\. [Cách thuật toán tự động tạo ra một bản đồ thế giới giả lập](https://frozenfractal.com/blog/2023/11/2/around-the-world-1-continents/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111509.webp)

Để phát triển một tựa game du hành thế giới, tác giả đã viết thuật toán giúp tự động tạo ra các lục địa giả lập. Bài viết minh họa trực quan từng bước thực hiện bằng hình ảnh rất sinh động.

7\. [Tác phẩm đoạt giải nhất cuộc thi hoạt hình thiếu nhi Anh Quốc](https://younganimator.uk/winner/1699875910225x437970782709919500)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111603.webp)

Tác giả đoạt giải nhất cuộc thi hoạt hình dành cho thiếu nhi tại Anh năm nay là một thiếu niên 16 tuổi. Tác phẩm mang tên "Robot làm xiên que" của cậu có mức độ hoàn thiện về mặt hình ảnh khiến giới chuyên môn phải kinh ngạc.

## 工具

1、[ShortbreadAI](https://shortbread.ai/)

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023100701.webp)

Trang web hỗ trợ người dùng tự tạo các bức vẽ truyện tranh một cách dễ dàng và nhanh chóng.

2、[ripsecrets](https://github.com/sirwart/ripsecrets)

Công cụ chuyên dùng để quét mã nguồn nhằm phát hiện xem có bị rò rỉ các khóa bảo mật (secrets) hay không. Thiết bị có thể cấu hình để chạy tự động trong quy trình CI/CD.

3、[EmojiGen](https://emoji.fly.dev/)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090904.webp)

Trang web hỗ trợ tạo ra các hình vẽ biểu cảm Emoji dựa trên các câu lệnh văn bản gợi ý.

4、[screenshot-to-code](https://github.com/abi/screenshot-to-code)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111609.webp)

Ứng dụng mã nguồn mở cho phép người dùng tải lên ảnh chụp màn hình một trang web, hệ thống sẽ tự động chuyển đổi thành mã nguồn HTML/Tailwind/JS tương ứng.

5、[PageSpyWeb](https://github.com/HuolalaTech/page-spy-web)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111206.webp)

Bộ công cụ debug từ xa mã nguồn mở, cung cấp giao diện tương tự như Console của trình duyệt để hỗ trợ quá trình sửa lỗi sản phẩm. (Đóng góp của [@wqcstrong](https://github.com/ruanyf/weekly/issues/3616))

6、[IPS](https://github.com/sjzar/ips)

Công cụ dòng lệnh chuyên dùng để tra cứu và xử lý các cơ sở dữ liệu vị trí địa lý của địa chỉ IP. (Đóng góp của [@sjzar](https://github.com/ruanyf/weekly/issues/3631))

7、[GWS](https://github.com/lxzan/gws)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111324.webp)

Thư viện WebSocket hiệu năng cao nguồn mở được viết hoàn toàn bằng ngôn ngữ Go, bao gồm cả phần máy chủ và máy khách. (Đóng góp của [@lxzan](https://github.com/ruanyf/weekly/issues/3623))

8、[ChatGot](https://start.chatgot.io/login)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111325.webp)

Ứng dụng cho phép trò chuyện đồng thời với nhiều mô hình AI khác nhau trong cùng một cửa sổ, ví dụ bạn có thể yêu cầu GPT xuất văn bản và dùng Midjourney vẽ ảnh trực tiếp. (Đóng góp của [@qinleilxl](https://github.com/ruanyf/weekly/issues/3624))

9、[Review giao diện web bằng AI](https://uxaudit.vercel.app/)

Ứng dụng hỗ trợ đánh giá giao diện dựa trên URL người dùng cung cấp, đưa ra các nhận xét về mặt thiết kế và gợi ý cải thiện trải nghiệm người dùng.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111013.webp)

Dịch vụ được cung cấp miễn phí, tuy nhiên hệ thống sẽ tạm dừng hoạt động nếu lượng người dùng truy cập quá đông cùng lúc.

10、[AITDK](https://aitdk.com/zh-CN/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111205.webp)

Công cụ hỗ trợ tối ưu hóa SEO. Người dùng chỉ cần nhập chủ đề bài viết, hệ thống sẽ tự động tạo ra tiêu đề, mô tả, từ khóa và các câu hỏi thường gặp phù hợp nhất với SEO. (Đóng góp của [@typewe](https://github.com/ruanyf/weekly/issues/3614))

## 资源

1\. **Thư mục tổng hợp các công cụ GPT**

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111207.webp)

Số lượng các công cụ được phát triển dựa trên mô hình GPT ngày càng nhiều. Dưới đây là danh sách các trang web tổng hợp và phân loại các công cụ này để người dùng tiện tra cứu:

- [GPTsHunter](https://www.gptshunter.com/)（Đóng góp của [@airyland](https://github.com/ruanyf/weekly/issues/3617)）
- [AwesomeGPTs](https://awesomegpts.pro/)（Đóng góp của [@GregoryZeng](https://github.com/ruanyf/weekly/issues/3619)）
- [BestGPTs](https://bestgpts.app/)（Đóng góp của [@qinleilxl](https://github.com/ruanyf/weekly/issues/3624)）
- [GPTs Works](https://gpts.works/)（Đóng góp của [@idoubi](https://github.com/ruanyf/weekly/issues/3629)）
- [GPTs Today](https://gptstoday.com/)（Đóng góp của [@KarnaughK](https://github.com/ruanyf/weekly/issues/3635)）
- [GPTs-store](https://gpts-store.net/)（Đóng góp của [@RunnningDogg](https://github.com/ruanyf/weekly/issues/3637)）

2\. [Bubble](https://github.com/LHRUN/bubble)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111323.webp)

Kho lưu trữ tổng hợp các widget trang trí độc đáo có thể tích hợp trực tiếp vào phần giới thiệu GitHub Profile hoặc file Readme của dự án. (Đóng góp của [@LHRUN](https://github.com/ruanyf/weekly/issues/3620))

3\. [Bing Image Creator](https://www.bing.com/images/create)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111505.webp)

Dịch vụ vẽ tranh bằng AI chính thức do Microsoft cung cấp.

4\. [YesChat.ai](https://www.yeschat.ai/zh-CN)

Trang web cho phép trải nghiệm miễn phí các mô hình AI thế hệ mới nhất như GPT-4V, DALL-E 3, Claude 2 (có giới hạn số lượt sử dụng hàng ngày). (Đóng góp của [@zengdamo](https://github.com/ruanyf/weekly/issues/3632))

5\. [Tài liệu hướng dẫn học máy cho người mới bắt đầu](https://github.com/microsoft/ML-For-Beginners)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111606.webp)

Bộ tài liệu giảng dạy nhập môn về lĩnh vực Trí tuệ nhân tạo / Học máy do chính Microsoft biên soạn (tiếng Anh).

## 图片

1\. [Túi đựng dụng cụ bị thất lạc trong không gian](https://www.usatoday.com/story/news/nation/2023/11/10/nasa-tool-bag-dropped-by-astronauts-international-space-station/71536725007/)

Vào ngày 1 tháng 11, các phi hành gia trên Trạm Vũ trụ Quốc tế (ISS) khi ra ngoài thực hiện bảo trì định kỳ đã vô tình làm tuột tay rơi mất chiếc túi đựng tuốc-nơ-vít vào không gian.

Chiếc túi này hiện đã trở thành một vệ tinh nhân tạo bất đắc dĩ (thực chất là rác vũ trụ) quay quanh Trái Đất ở độ cao hơn 300 km. Bức ảnh dưới đây ghi lại hình ảnh chiếc túi nhìn từ trạm ISS.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111501.webp)

Điều thú vị là hiện nay người dân trên Trái Đất nếu sử dụng kính viễn vọng thiên văn loại phổ thông hướng về phía trạm ISS hoàn toàn có thể quan sát thấy chiếc túi dụng cụ này.

2\. [Dùng GPT-4V để tự động vẽ biểu đồ trực quan](https://resobscura.substack.com/p/generative-ai-for-historical-research)

Mới đây, OpenAI đã mở rộng tính năng nhận diện hình ảnh GPT-4 Vision (gọi tắt là GPT-4V) cho người dùng. Bạn có thể tải lên một bức ảnh và yêu cầu GPT thực hiện các thao tác xử lý dữ liệu.

Một người dùng đã thử tải lên ảnh chụp một bảng dữ liệu dạng văn bản (ảnh bên trái), và yêu cầu AI tự động vẽ thành biểu đồ trực quan tương ứng (ảnh bên phải):

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111604.webp)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111605.webp)

Kết quả thử nghiệm cho thấy GPT-4V có khả năng tự động viết và thực thi mã Python để trực quan hóa dữ liệu trực tiếp từ các thông tin trích xuất trong hình ảnh.

3\. [Ma trận hộp thoại yêu cầu cấp quyền trên MacOS](https://sixcolors.com/post/2023/11/a-picture-is-worth-a-thousand-permissions-requests/)

Hệ điều hành macOS của Apple đang ngày càng trở nên rườm rà với vô số các hộp thoại cảnh báo bảo mật và yêu cầu cấp quyền truy cập liên tục.

Bức ảnh dưới đây ghi lại cảnh tượng khi một quản trị viên thực hiện chuyển đổi dữ liệu từ máy Mac cũ sang máy Mac mới mua.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111208.webp)

Sau khi quá trình đồng bộ hoàn tất, toàn bộ các ứng dụng được cài đặt ở chế độ tự động khởi động cùng hệ thống đồng loạt chạy lên và tạo ra một màn hình ngập tràn các hộp thoại xác nhận quyền như trên.

## ✍️ Bài đọc thêm

### Bàn về vai trò của khả năng truyền tải câu chuyện sáng lập

Thế giới hiện đại là một thế giới dư thừa dòng vốn đầu tư, chỉ cần bạn thuyết phục được đủ số lượng người tin tưởng vào ý tưởng của mình, bạn sẽ dễ dàng nhận được nguồn vốn lớn cùng mức định giá công ty rất cao.

Đối với các nhà sáng lập, **năng lực truyền tải câu chuyện (Storytelling) sẽ quyết định trực tiếp đến sự thành bại của dự án**.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111610.webp)

Chỉ cần bạn có thể giải thích rõ ràng ý tưởng sản phẩm, nêu bật được các điểm sáng giá của dự án và tiếp cận công chúng theo một cách đúng đắn nhất, cơ hội nhận được vốn đầu tư của bạn là rất lớn.

Câu chuyện của Elon Musk và hãng xe điện Tesla là một minh chứng rõ nét nhất. Định giá của Tesla ở mức cực kỳ cao, chỉ cần các nhà đầu tư còn tin tưởng vào câu chuyện tương lai của hãng, Tesla sẽ có đủ thời gian để hiện thực hóa giá trị định giá đó. Ngược lại, nếu lòng tin của nhà đầu tư đổ vỡ, định giá bong bóng của hãng cũng sẽ sụp đổ theo.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111611.webp)

Điều này cho thấy các phát ngôn hay hành động gây tranh cãi của Elon Musk trên truyền thông không đơn thuần là để gây sự chú ý. Thực chất đó là một phương pháp tiếp thị với chi phí cực kỳ rẻ nhằm xây dựng lòng tin của công chúng vào câu chuyện phát triển của doanh nghiệp, từ đó hỗ trợ vững chắc cho mức định giá cao của tập đoàn.

Doanh nghiệp nào truyền tải câu chuyện của mình càng thuyết phục, họ càng dễ tiếp cận dòng vốn và sở hữu chỉ số P/E càng cao.

## Lịch sử tuần này

- 2022年（第 231 期）：[Quy mô nhân sự: Thảo luận về số lượng nhân sự tối ưu cần thiết của một công ty công nghệ](http://www.ruanyifeng.com/blog/2022/11/weekly-issue-231.html)
- 2021年（第 181 期）：[Thanh toán di động: Bàn luận về các nguyên lý và phương pháp thiết kế giao diện thanh toán tối ưu](http://www.ruanyifeng.com/blog/2021/10/weekly-issue-181.html)
- 2020年（第 131 期）：[Tư duy lập trình: Khám phá sự khác biệt giữa tư duy logic nhị phân và logic tam phân](http://www.ruanyifeng.com/blog/2020/10/weekly-issue-131.html)
- 2019年（第 81 期）：[Góc nhìn xã hội: Liệu thế hệ con cháu có thể vượt qua thế hệ cha ông một cách vượt trội?](http://www.ruanyifeng.com/blog/2019/11/weekly-issue-81.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
