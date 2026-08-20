# Bản tin chia sẻ công nghệ (Số 388): Kiểm thử là hào nước sâu bảo vệ mới

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/9088) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030804.webp)

Một khu du lịch tại Phù Lăng, Trùng Khánh vừa đưa vào vận hành cầu cáp treo bằng đá khổng lồ đầu tiên trên thế giới. Mặt cầu được ghép từ các khối đá lớn độc lập cách nhau một khoảng, du khách chỉ cần sơ sẩy một chút là có thể bước hụt chân xuống vực sâu. ([via](https://www.cbg.cn/a/77561/20260214/7b37135efeb74f0fbbaf272a9b7f6ae0.html))

## 测试是新的护城河

Next.js hiện là framework JavaScript toàn năng (full-stack JS framework) đứng đầu thế giới hiện nay. Theo đánh giá cá nhân của tôi, có lẽ một nửa số ứng dụng web full-stack mà lập trình viên phát triển hiện nay đều đang sử dụng framework này.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022808.webp)

Thế nhưng cách đây hai tuần, một tin tức chấn động đã hoàn toàn làm đảo lộn vị thế của framework này.

Một kỹ sư của Cloudflare đã công bố dự án [vinext](https://vinext.io/), tuyên bố **anh đã tự xây dựng thành công toàn bộ Next.js bằng AI chỉ trong vòng vỏn vẹn một tuần**.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022809.webp)

Thực tế, anh chỉ mất đúng một ngày để hoàn thành phiên bản chạy thử nghiệm (prototype) ban đầu, và thời gian còn lại của tuần chỉ để tinh chỉnh và tối ưu hóa hệ thống.

> "Tôi chính thức bắt tay vào làm từ ngày 13 tháng 2, ngay trong đêm hôm đó toàn bộ các tính năng cốt lõi đã vận hành ổn định. Chiều ngày hôm sau, tôi đã hoàn thiện xong 10 trên tổng số 11 router của hệ thống. Đến ngày thứ ba, dự án đã được triển khai lên máy chủ thực tế và hoàn thành đầy đủ quy trình hydration phía client (client-side hydration).
>
> Những ngày tiếp theo tôi tập trung tối ưu hóa bảo mật hệ thống: vá các lỗi biên dịch ở các tình huống đặc biệt, mở rộng bộ công cụ kiểm thử tự động và nâng tỷ lệ bao phủ API đạt mức 94%."

Điều đáng chú ý là phiên bản tái cấu trúc này sở hữu hiệu năng vận hành vượt trội hơn cả phiên bản gốc của Next.js:

> "Các kết quả kiểm thử hiệu năng thời kỳ đầu cho thấy tốc độ build dự án đã tăng gấp 4 lần, dung lượng gói mã nguồn phân phối phía client được thu nhỏ tới 57%, và các ứng dụng Next.js thực tế trong môi trường production đã có thể chạy trực tiếp trên nền tảng này một cách mượt mà."

Mã nguồn của dự án [vinext](https://github.com/cloudflare/vinext) hiện đã được Cloudflare chia sẻ công khai trên GitHub.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022810.webp)

Tôi nghĩ **đây là một cú sốc cực kỳ lớn đối với Next.js và công ty chủ quản Vercel**.

Next.js là sản phẩm thương mại cốt lõi của công ty Vercel, được vận hành phát triển bởi một đội ngũ kỹ sư khổng lồ với mức đầu tư kinh phí cực lớn liên tục trong suốt 10 năm qua. Mặc dù là phần mềm mã nguồn mở, nhưng Vercel thu phí dịch vụ từ các tính năng phiên bản doanh nghiệp, hạ tầng đám mây, các plugin và giao diện mẫu chuyên dụng, mang lại nguồn doanh thu lên tới 200 triệu USD trong năm ngoái.

**Hào nước sâu bảo vệ (moat) tưởng chừng như không thể vượt qua này đã hoàn toàn bị AI đập tan**. Chỉ một kỹ sư duy nhất làm việc trong vòng một tuần đã có khả năng tái tạo lại toàn bộ thành quả công việc kéo dài suốt 10 năm của một đội ngũ kỹ sư khổng lồ. Các ứng dụng web hiện tại thậm chí không cần phải sửa đổi bất kỳ dòng mã nguồn nào, chỉ cần đưa lên hệ thống mới là có thể chạy ngay lập tức và hỗ trợ đầy đủ mọi tính năng của phiên bản gốc.

Bạn có biết tổng chi phí Token mà người kỹ sư này đã chi trả cho AI để hoàn thành công việc là bao nhiêu không? Chỉ vỏn vẹn 1.100 USD!

Thực tế này sẽ khiến Vercel gặp rất nhiều khó khăn trong việc thuyết phục hội đồng quản trị tiếp tục rót vốn đầu tư phát triển Next.js, và các khách hàng doanh nghiệp cũng sẽ cân nhắc kỹ trước khi quyết định chi trả các khoản phí dịch vụ đắt đỏ cho các tính năng thương mại của hãng.

Nhìn rộng ra, toàn bộ ngành công nghiệp phát triển phần mềm thương mại đều đang đối mặt với những thách thức tương tự. **Hào lũy bảo vệ bằng mã nguồn đã hoàn toàn biến mất, chỉ với một khoản đầu tư tài chính siêu nhỏ, AI đã có khả năng tái tạo nhanh chóng các hệ thống phần mềm quy mô lớn**.

Để bảo vệ mô hình kinh doanh của mình, bước đi tiếp theo của các hãng công nghệ chắc chắn phải tìm cách ngăn chặn các AI tiến hành sao chép và tái tạo sản phẩm của họ.

Giải pháp bảo vệ ở đây là gì? **Chìa khóa cốt lõi chính là các kịch bản kiểm thử (test cases)**.

Sở dĩ kỹ sư Cloudflare có thể tái tạo Next.js thành công là nhờ Next.js trang bị hệ thống tài liệu hướng dẫn vô cùng chi tiết, hàng triệu bài viết chia sẻ kinh nghiệm của cộng đồng cùng hệ thống kịch bản kiểm thử vô cùng toàn diện. Các API do AI sinh ra chỉ cần chạy vượt qua các bài kiểm thử tương thích mặc định là đã có thể bảo đảm khả năng tương thích hoàn toàn 100% với hệ thống cũ.

Nếu không tiếp cận được các kịch bản kiểm thử này, không một nhà phát triển nào dám tin tưởng đưa một hệ thống do AI viết lại vào vận hành thực tế trong môi trường sản xuất (production) vì lo ngại các sai sót hành vi mã nguồn phát sinh.

Có thể dự báo các dự án phần mềm lớn trong tương lai sẽ thắt chặt kiểm soát và đóng khóa hoàn toàn hệ thống kịch bản kiểm thử của mình để tránh bị AI sao chép. **Kiểm thử mới thực sự là hào nước sâu bảo vệ mới của phần mềm.**

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030601.webp)

Lấy ví dụ cơ sở dữ liệu phổ biến nhất hành tinh [SQLite](https://sqlite.org) sở hữu 156.000 dòng code lõi, nhưng hệ thống kịch bản kiểm thử đi kèm của nó lên tới [92,05 triệu dòng code](https://sqlite.org/testing.html) – gấp tới 590 lần dung lượng mã nguồn sản phẩm!

Trong đó bộ công cụ kiểm thử cốt lõi mang tên [TH3](https://sqlite.org/th3.html) hoàn toàn được đóng mã nguồn bảo mật nghiêm ngặt để kiểm thử các tình huống giới hạn và cực đoan trong các lĩnh vực đặc thù như hàng không vũ trụ và thiết bị y tế. Chính hệ thống kiểm thử bảo mật này là rào cản kỹ thuật giúp SQLite không thể bị sao chép hay thay thế.

Một diễn biến tương tự vừa diễn ra cách đây hai ngày khi dự án vẽ sơ đồ mã nguồn mở nổi tiếng [tldraw](https://github.com/tldraw/tldraw/issues/8082) cũng đã lên kế hoạch đóng mã nguồn đối với toàn bộ các kịch bản kiểm thử của mình.

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022811.webp)

Thành thật mà nói, việc đóng cửa các kịch bản kiểm thử sẽ gây ảnh hưởng tiêu cực nhất định đến sự phát triển chung của cộng đồng mã nguồn mở, nhưng đây là lựa chọn bắt buộc để các nhà phát triển tự bảo vệ quyền lợi kinh tế của mình trước năng lực ngày một mạnh mẽ của AI.

## AI 复刻的版权问题

Quy trình sử dụng AI để tái tạo phần mềm cũng làm phát sinh các tranh chấp pháp lý phức tạp về quyền sở hữu trí tuệ và bản quyền.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030602.webp)

Next.js sử dụng giấy phép nguồn mở MIT vô cùng thông thoáng nên việc sao chép không gặp rào cản pháp lý. Tuy nhiên, vụ việc một nhà phát triển sử dụng AI để viết lại dự án [chardet](https://github.com/chardet/chardet) đã thổi bùng lên các cuộc tranh luận gay gắt trong cộng đồng.

Dự án gốc chardet áp dụng giấy phép LGPL với rất nhiều điều khoản ràng buộc chặt chẽ. Nhà phát triển sau khi dùng AI viết lại đã tự ý chuyển đổi giấy phép dự án thành giấy phép MIT thông thoáng hơn, vấp phải sự phản đối kịch liệt từ tác giả sáng lập dự án gốc.

Các luồng ý kiến trên mạng xã hội hiện đang chia làm hai chiến tuyến rõ rệt:

- Luồng ý kiến ủng hộ lập luận rằng: AI chỉ học hỏi logic tính năng và giao diện API của dự án cũ để tự sinh ra cấu trúc mã nguồn mới hoàn toàn khác biệt, do đó nhà phát triển có toàn quyền thay đổi giấy phép bản quyền theo ý muốn.
- Luồng ý kiến phản đối chỉ ra điều khoản của giấy phép GPL quy định rõ: toàn bộ các sản phẩm phái sinh (derivative works) đều bắt buộc phải kế thừa nguyên vẹn giấy phép bản quyền của dự án gốc, và việc dùng AI viết lại thực chất vẫn chỉ là một dạng sản phẩm phái sinh.

Điểm phức tạp hơn cả là theo quy định pháp lý của Mỹ, các sản phẩm do trí tuệ nhân tạo tạo sinh ra hoàn toàn không được thừa nhận quyền bảo hộ tác giả mà thuộc về tài sản công cộng (public domain). Điều này đồng nghĩa với việc **các phần mềm được tái tạo lại bằng AI sẽ không có quyền áp đặt bất kỳ giấy phép bản quyền nào, và mọi thiết lập bản quyền đều vô hiệu trước pháp luật**.

Chiếu theo quy định này, giá trị của các giấy phép bản quyền phần mềm sẽ không còn nhiều ý nghĩa. Bất kể phần mềm của bạn đang sử dụng giấy phép chặt chẽ thế nào, người khác chỉ cần sử dụng AI quét và viết lại là đã có thể dễ dàng lách luật, và toàn bộ phiên bản viết lại bằng AI đó đều mặc nhiên không có bản quyền.

## 科技动态

1. **AI hỗ trợ tự động viết lại từ ngữ thô tục trong game**

Nền tảng trò chơi trực tuyến Roblox vừa thông báo sẽ áp dụng công nghệ AI để tự động điều chỉnh các đoạn hội thoại của người chơi theo thời gian thực để hướng tới môi trường giao tiếp văn minh hơn.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030701.webp)

Trước đây, nếu người chơi nhập các từ ngữ thô tục trong game, hệ thống sẽ lọc và chuyển chúng hiển thị thành dạng ký tự đại diện `####`, nhưng người đọc vẫn dễ dàng đoán được đối phương đang có thái độ tiêu cực.

Hiện tại, AI sẽ thực hiện viết lại toàn bộ câu nói theo hướng lịch sự và văn minh hơn, giúp người chơi khác hoàn toàn không nhận ra đối phương đang có hành vi chửi thề.

Mặc dù giải pháp này mang lại cảm giác có phần giả tạo, nhưng thực sự là một cải tiến cần thiết. Các diễn đàn thảo luận trực tuyến cũng nên nghiên cứu áp dụng giải pháp tương tự để tránh các hành vi công kích cá nhân làm suy giảm chất lượng trao đổi.

2. **Công nghệ truy cập Internet bằng tia laser trên máy bay**

Cơ quan Vũ trụ Châu Âu (ESA) đã thử nghiệm thành công công nghệ kết nối Internet bằng tia laser trên chuyến bay, giúp thiết lập đường truyền dữ liệu tốc độ cao trực tiếp giữa máy bay đang bay và vệ tinh.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030704.webp)

Dịch vụ Internet trên máy bay hiện nay chủ yếu vận hành qua sóng vô tuyến (chẳng hạn như mạng vệ tinh Starlink). Thí nghiệm lần này đã chuyển sang sử dụng chùm tia laser để kết nối.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030705.webp)

Hình ảnh trên hiển thị cụm thiết bị phát laser được lắp đặt trực tiếp trên cửa kính cabin máy bay.

Ưu điểm lớn nhất của công nghệ truyền tin bằng laser là băng thông rộng cực lớn và không bị giới hạn bởi các dải tần vô tuyến thông thường. Tốc độ kết nối thử nghiệm đạt mốc 2,6 Gbps, nhanh gấp 8 đến 10 lần so với mạng Starlink hiện nay.

Hạn chế của giải pháp này là đòi hỏi chùm tia laser kết nối giữa máy bay và vệ tinh phải luôn duy trì trên một đường thẳng tuyệt đối và không bị cản trở bởi các tầng mây hay bầu khí quyển. Do đó, công nghệ này có lẽ chỉ vận hành ổn định khi máy bay đạt đến độ cao bay hành trình trên mây.

3. **Cơ chế tạo bản sao chuyên gia viết lách của Grammarly**

Dịch vụ hỗ trợ viết lách nổi tiếng Grammarly cung cấp một tính năng trả phí mang tên "Đánh giá của chuyên gia" (Expert Reviews), cho phép người dùng nhận các lời khuyên nâng cao chất lượng bài viết từ các chuyên gia ngôn ngữ.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031002.webp)

Một người dùng ở nước ngoài khi trải nghiệm tính năng này đã vô cùng sốc khi phát hiện một trong những chuyên gia đưa ra đánh giá bài viết cho mình chính là người sếp cũ đã qua đời trước đó của anh (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031003.webp)

Sự thật sau đó được bộc lộ: hệ thống không sử dụng chuyên gia thật mà thực chất là các bản sao số (digital twins) của họ được huấn luyện bằng các bài viết cũ của các chuyên gia để AI tự động tạo lời khuyên dưới danh nghĩa của họ.

Hiện tượng này dấy lên những làn sóng tranh cãi lớn về mặt đạo đức: liệu chúng ta có quyền tự ý xây dựng các bản sao kỹ thuật số của một cá nhân và gắn nhãn tên tuổi của họ (chẳng hạn như "bản sao Khổng Tử" hay "bản sao Einstein") để cung cấp dịch vụ thương mại hay không?

4. **Giải pháp cải tiến hòm thư bưu điện sử dụng năng lượng mặt trời**

Trong kỷ nguyên kết nối Internet phổ cập hiện nay, số phận của các hòm thư truyền thống trên đường phố sẽ đi về đâu?

Công ty Bưu điện Hoàng gia Anh đã đưa ra sáng kiến chuyển đổi 3.500 hòm thư truyền thống trên khắp cả nước thành các "hòm thư năng lượng mặt trời".

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110505.webp)

Phần mái hòm thư được lắp đặt các tấm pin năng lượng mặt trời, và tính năng của hòm thư được nâng cấp từ việc gửi thư giấy thông thường sang mảng nhận và gửi các bưu kiện chuyển phát nhanh kích thước nhỏ.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110506.webp)

Giải pháp này vừa giúp bảo tồn được nét kiến trúc độc đáo của các hòm thư màu đỏ đặc trưng trên đường phố Anh, vừa mang lại những tiện ích thiết thực cho nhu cầu chuyển phát bưu kiện hiện đại của người dân.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025110507.webp)

## 文章

1. [Phát hiện phương thức tấn công tiêm mã độc vào tiêu đề GitHub Issue](https://grith.ai/blog/clinejection-when-your-ai-tool-installs-another) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030703.webp)

Đây có thể coi là trường hợp tấn công tiêm mã độc (prompt injection) thực tế đầu tiên nhắm vào các mô hình AI. Dự án Cline sử dụng AI để tự động phân loại các Issue trên GitHub. Kẻ tấn công đã chèn các câu lệnh độc hại trực tiếp vào tiêu đề của Issue, từ đó đánh lừa AI để chiếm đoạt mã bảo mật npm token thành công và phát hành một phiên bản mã nguồn chứa mã độc. Bài viết phân tích chi tiết về quy trình tấn công này.

2. [Đánh giá lại giá trị thực tế của tệp tin `AGENTS.md`](https://www.infoq.com/news/2026/03/agents-context-file-value-review/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030901.webp)

Một nghiên cứu công nghệ mới nhất chỉ ra rằng việc bổ sung tệp cấu hình `AGENTS.md` thực tế không mang lại hiệu quả hỗ trợ lập trình cho AI như khuyến nghị trước đây mà ngược lại còn gây cản trở.

Tệp tin này chỉ khiến mô hình AI tốn nhiều bước suy nghĩ logic hơn (làm tăng chi phí tiêu thụ token) mà không giúp cải thiện chất lượng mã nguồn sinh ra (làm giảm hiệu năng xử lý).

3. [Hành trình 9 năm phát triển của dự án Temporal API](https://bloomberg.github.io/js-blog/post/temporal/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031205.webp)

Tuần này, chuẩn Temporal API đã chính thức vượt qua giai đoạn đánh giá thứ 4 để chính thức gia nhập vào chuẩn ES2026 và trở thành một cú pháp mặc định trong ngôn ngữ JavaScript. Bài viết chia sẻ những dòng hồi ký của tác giả soạn thảo chuẩn về hành trình kiên trì thúc đẩy dự án suốt 9 năm qua.

4. [Bộ kiểm thử khả năng phân định thông tin ảo giác của AI (BullshitBench)](https://decrypt.co/360596/benchmark-test-measures-ai-bullshit-most-models-fail) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031206.webp)

Cộng đồng giới thiệu công cụ kiểm thử [BullshitBench](https://petergpt.github.io/bullshit-benchmark/viewer/index.v2.html) chuyên đưa ra các câu hỏi vô nghĩa hoặc thông tin sai lệch để đánh giá xem mô hình AI có khả năng nhận biết lỗi logic để từ chối trả lời hay vẫn trả lời một cách nghiêm túc.

5. [Sức mạnh của mã nguồn CSS thuần (Vanilla CSS)](https://www.zolkos.com/2025/12/03/vanilla-css-is-all-you-need) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120704.webp)

Bài phân tích mã nguồn CSS thực tế của công ty 37Signals cho thấy việc phát triển dự án hoàn toàn không cần phụ thuộc vào bất kỳ framework CSS nào (như Tailwind) hay các công cụ build (như Sass) mà vẫn bảo đảm giao diện vận hành hoàn hảo và tối ưu.

6. [Giải thích hiện tượng sinh học dưới góc nhìn vật lý học](https://theconversation.com/physics-of-poo-why-it-takes-you-and-an-elephant-the-same-amount-of-time-76696) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030802.webp)

Bài viết khoa học giải thích về một hiện tượng sinh học thú vị: tại sao mọi loài động vật có vú bất kể kích thước cơ thể lớn hay nhỏ đều có thời gian đại tiện trung bình ổn định trong khoảng từ 5 đến 19 giây (trung bình là 12 giây).

## 工具

1. [KULA](https://github.com/c0m4r/kula)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030706.webp)

Bộ công cụ giám sát hiệu năng máy chủ Linux gọn nhẹ được đóng gói duy nhất trong một file thực thi nhị phân.

2. [AnsiSaver](https://github.com/lardissone/ansi-saver)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030803.webp)

Ứng dụng bảo vệ màn hình (screensaver) độc đáo dành cho máy tính Mac sử dụng các bức tranh vẽ từ ký tự ANSI nhiều màu sắc để làm họa tiết bảo vệ.

3. [upiano](https://github.com/eliasdorneles/upiano)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023081012.webp)

Công cụ giải trí độc đáo hỗ trợ người dùng mô phỏng và chơi đàn piano trực tiếp ngay trên giao diện dòng lệnh terminal.

4. [WSL Distro Manager](https://github.com/bostrot/wsl2-distro-manager)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031207.webp)

Phần mềm mã nguồn mở dành cho hệ điều hành Windows cung cấp giao diện đồ họa giúp người dùng dễ dàng quản lý và cài đặt các phân phối của Windows Subsystem for Linux (WSL).

5. [Mole](https://github.com/tw93/Mole)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031213.webp)

Bộ công cụ mã nguồn mở hỗ trợ quét dọn rác và tối ưu hóa hệ thống dành riêng cho máy tính Mac.

6. [PipeGate](https://github.com/janbjorge/pipegate)

Công cụ thiết lập đường truyền tunnel giúp ánh xạ các dịch vụ mạng nội bộ ra môi trường Internet công cộng, ưu điểm là cấu trúc tối giản viết bằng Python và hỗ trợ cơ chế bảo mật xác thực client qua UUID.

7. [HookListener](https://www.hooklistener.com)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024121804.webp)

Dịch vụ trực tuyến hỗ trợ nhà phát triển quản lý và kiểm thử kết nối Webhook tiện lợi, có chính sách miễn phí cho tài khoản cá nhân.

8. [Sentinel](https://github.com/suzuran0y/CCTV-Smartphone-AI-Monitoring)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031201.webp)

Dự án hỗ trợ biến chiếc điện thoại Android cũ thành hệ thống camera giám sát an ninh mạng hỗ trợ thu thập hình ảnh thời gian thực. (Đóng góp từ [@suzuran0](https://github.com/ruanyf/weekly/issues/9201))

9. [Flux Monitor](https://github.com/chentao1006/FluxMonitor)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031203.webp)

Bảng điều khiển theo dõi và quản trị tài nguyên hệ thống trực quan dành riêng cho máy tính Mac. (Đóng góp từ [@chentao1006](https://github.com/ruanyf/weekly/issues/9207))

## AI 相关

1. [Agentic Metric](https://github.com/MrQianjinsi/agentic-metric)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030603.webp)

Công cụ dòng lệnh viết bằng Python hỗ trợ lập trình viên theo dõi và thống kê chi tiết lượng tiêu thụ token của các trợ lý coding agents khác nhau (như Claude Code, Codex, OpenCode) chạy local. (Đóng góp từ [@MrQianjinsi](https://github.com/ruanyf/weekly/issues/9165))

2. [cc-connect](https://github.com/chenhg5/cc-connect)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031202.webp)

Bộ kết nối mã nguồn mở giúp liên kết các công cụ lập trình AI với các ứng dụng trò chuyện trên thiết bị di động của lập trình viên. (Đóng góp từ [@chenhg5](https://github.com/ruanyf/weekly/issues/9202))

3. [Page Agent](https://github.com/alibaba/page-agent)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030702.webp)

Thư viện JavaScript hỗ trợ tích hợp tính năng điều khiển trang web bằng ngôn ngữ tự nhiên, ví dụ người dùng có thể ra lệnh: "Click chọn liên kết tài liệu hướng dẫn trên thanh menu và tóm tắt nội dung trang web đó cho tôi".

4. [Agent Safehouse](https://github.com/eugene1g/agent-safehouse)

Công cụ quản lý sandbox dành cho macOS hỗ trợ lập trình viên chạy các công cụ lập trình AI trong môi trường cách ly an toàn để tránh mã độc gây hại cho máy tính.

5. [Repo Tokens](https://github.com/qwibitai/nanoclaw/tree/main/repo-tokens)

![](https://cdn.beekka.com/blogimg/asset/202602/bg2026022801.webp)

Tiện ích GitHub Action tự động tạo nhãn đồ họa (badge) cho repository để hiển thị quy mô dự án tương đương với bao nhiêu mã Token đầu vào phục vụ việc ước tính chi phí huấn luyện cho các mô hình AI lớn.

## 资源

1. [World Monitor](https://www.worldmonitor.app)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026030801.webp)

Bảng tin trực quan cập nhật diễn biến tình hình quốc tế theo thời gian thực bằng việc tổng hợp đa dạng các nguồn tin tức uy tín trên cùng một giao diện trang web duy nhất.

2. [Bản đồ tương tác khám phá quy trình lọc dầu](https://fuelingcuriosity.com/game.html)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031204.webp)

Trang web sử dụng các hiệu ứng đồ họa hoạt hình tương tác sinh động để giải thích chi tiết quy trình nhà máy lọc dầu chưng cất dầu mỏ thành xăng và dầu diesel thương mại.

3. [Mô phỏng cơ cấu chuyển động cơ khí Mechanical Pencil](https://mechanical-pencil.com)

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031001.webp)

Trang web tổng hợp các hình ảnh mô phỏng 3D hoạt động cơ học của các vật dụng quen thuộc hàng ngày như bút bấm, bật lửa... giúp người xem thấu hiểu nguyên lý cơ cấu chuyển động.

## 图片

1. **Ý tưởng thiết kế phương thức xác thực mật khẩu thân thiện hơn**

Một lập trình viên đã chia sẻ ý tưởng thiết kế phương thức bảo mật mật khẩu mới bằng hình ảnh, hãy xem giải pháp này có tính khả thi thực tế hay không?

Hệ thống hiển thị một bộ bài tú lơ khơ 52 quân bài và yêu cầu người dùng chọn lần lượt 5 quân bài theo trình tự nhất định để làm chuỗi mật khẩu thiết lập:

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025073110.webp)

Trong các lần đăng nhập tiếp theo, người dùng bắt buộc phải chọn đúng 5 quân bài đó theo đúng trình tự đã thiết lập ban đầu để truy cập hệ thống thành công.

## 文摘

1. **Nguyên nhân dẫn đến sự sụp đổ của các xã hội phức tạp**

Chúng ta đều thấu hiểu một thực tế trong phát triển phần mềm: một khi độ phức tạp của mã nguồn vượt quá một ngưỡng giới hạn nhất định, hệ thống sẽ trở nên cực kỳ khó bảo trì và cuối cùng buộc phải bị loại bỏ để viết lại.

Nhà sử học người Mỹ Joseph Tainter lập luận rằng cấu trúc xã hội loài người cũng tuân theo quy luật tương tự. Nếu độ phức tạp trong vận hành của một xã hội vượt quá ngưỡng chịu đựng, xã hội đó mặc nhiên sẽ bước vào chu kỳ sụp đổ.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026031214.webp)

Vào năm 1988, ông đã xuất bản cuốn sách nổi tiếng mang tên "Sự sụp đổ của các xã hội phức tạp", phân tích chi tiết về sự hưng thịnh và suy vong của các nền văn minh vĩ đại như Đế chế La Mã, người Maya để trả lời cho câu hỏi bấy lâu nay của giới học thuật: **Tại sao các quốc gia hùng mạnh lại đi đến con đường sụp đổ?**

Luận điểm chính của ông chỉ ra kẻ thù lớn nhất tàn phá các xã hội chính là độ phức tạp (complexity).

Cùng với tiến trình phát triển văn minh, xã hội sẽ liên tục tích lũy thêm các tầng nấc phức tạp mới: thiết lập thêm nhiều cấp bậc quản lý, phình to bộ máy quan liêu và phân hóa sâu sắc các giai tầng cấu trúc xã hội.

Ở giai đoạn ban đầu, việc phình to bộ máy quản trị mang lại những hiệu quả thiết thực như thúc đẩy sản lượng kinh tế phát triển và tăng cường nguồn thu thuế. Tuy nhiên khi đạt đến một ngưỡng giới hạn, quy luật hiệu suất giảm dần (diminishing returns) sẽ lập tức xuất hiện: việc tiếp tục tăng thêm độ phức tạp quản lý chỉ mang lại giá trị gia tăng ngày một thấp, thậm chí tiệm cận mốc bằng 0 hoặc mang giá trị âm gây hại cho xã hội.

- Hệ thống luật pháp cồng kềnh kết hợp bộ máy hành chính phình to làm gia tăng chi phí vận hành quốc gia lên mức khổng lồ, lâu dài sẽ trở thành gánh nặng vượt quá sức chịu đựng kinh tế của xã hội.
- Độ phức tạp quản trị gia tăng sẽ khoét sâu thêm sự bất bình đẳng xã hội. Do số lượng người thấu hiểu tường tận toàn bộ các quy tắc xã hội ngày một ít đi, vai trò của giới luật sư trở nên độc quyền và những người am hiểu luật chơi đương nhiên sẽ chiếm dụng được nhiều lợi thế vượt trội hơn hẳn phần còn lại của xã hội.
- Càng nhiều quy định ràng buộc sẽ kéo theo sự ra đời của càng nhiều cơ quan giám sát thực thi pháp luật, gián tiếp bóp nghẹt hiệu suất hoạt động và tính linh hoạt tự nhiên của toàn xã hội.
- Cuối cùng, độ phức tạp quá mức sẽ làm giãn rộng khoảng cách giàu nghèo và phân hóa sâu sắc các giai tầng xã hội, là nguồn cơn dẫn đến các cuộc xung đột đối kháng nội bộ tàn phá đất nước.

Sự cộng hưởng của các yếu tố bất lợi trên chính là nguyên nhân cốt lõi dẫn đến sự sụp đổ không thể tránh khỏi của rất nhiều đế chế hùng mạnh trong lịch sử nhân loại.

## 言论

1.

Thời điểm năm 2021, tôi cảm giác làm một kỹ sư phần mềm là công việc tuyệt vời nhất thế giới. Ngành công nghiệp phần mềm bùng nổ mạnh mẽ với vô vàn cơ hội nghề nghiệp rộng mở, tôi thực sự yêu công việc này và nghĩ mình có thể cống hiến gắn bó với nó cả đời.

Thế nhưng đến năm 2026 hiện tại, tôi hoàn toàn mơ hồ về tương lai của ngành phần mềm trong 10 năm tới. Ngay cả khi công việc này vẫn tồn tại, chắc chắn diện mạo của nó sẽ hoàn toàn khác biệt so với hiện nay. Tôi có thể phải chật vật tìm lối đi mới hoặc buộc phải chấp nhận rời bỏ ngành để chuyển hướng. Dù kịch bản nào xảy ra, công việc lập trình phần mềm mà tôi từng yêu thích sâu sắc đang dần biến mất.

-- Trích bài viết [《Tôi thực sự không biết liệu công việc của mình có còn tồn tại sau 10 năm nữa không》](https://www.seangoedecke.com/will-my-job-still-exist/)

2.

Cảm giác đối đầu trực tiếp với một hệ thống AI mạnh mẽ sẽ như thế nào?

Bạn sẽ liên tục trải qua cảm giác bản thân bỗng nhiên trở nên vô cùng yếu thế một cách khó hiểu, và mọi hành động hay kết quả xử lý của AI đều vượt xa các dự báo và khả năng phản ứng của bạn.

Hiện tượng này tương tự như việc bạn đang chơi một trò chơi có tính ngẫu nhiên cao với một đối thủ có đẳng cấp vượt trội hoàn toàn, và bạn luôn có cảm giác đối phương luôn được thần may mắn mỉm cười hỗ trợ trong mọi lượt đi.

-- Trích chia sẻ trên trang blog probablydance.com

3.

Việc lãng phí thời gian để đọc các cuốn sách về nghệ thuật thương trường hay sách dạy làm giàu là điều vô nghĩa. Các cuốn sách này thường cố gắng biến các câu chuyện tình huống đơn giản thành những bài học kinh nghiệm vạn năng, quy kết các thành công ngẫu nhiên trên thị trường thành các chiến lược kinh doanh phổ quát, và sử dụng các câu khẩu hiệu truyền cảm hứng sáo rỗng để khỏa lấp đi bức tranh thị trường đầy biến động và phức tạp thực tế.

Sự thành công về mặt doanh số của các cuốn sách này hoàn toàn không phải vì nội dung kiến thức của chúng chính xác, mà đơn giản vì chúng quá dễ đọc và mang lại cảm giác dễ chịu cho độc giả.

-- Trích bài viết [《Tại sao đọc sách kinh doanh chỉ là hành vi lãng phí thời gian》](https://antemedian.substack.com/p/why-reading-business-books-is-a-waste)

4.

Trong trường hợp tôi muốn AI hướng dẫn cách thức vận hành một bộ công cụ công nghệ mới hoàn toàn mà ngay cả dữ liệu của AI cũng chưa được cập nhật tính năng, tôi sẽ gõ câu lệnh yêu cầu AI: "Hãy chạy lệnh `xxx-tool --help` để tự tìm hiểu về tính năng công cụ này" (với giả định tên công cụ là `xxx-tool`), ngay lập tức AI sẽ tự đọc hiểu tài liệu hướng dẫn và làm chủ được cách thức vận hành công cụ đó cho tôi.

-- Lập trình viên nổi tiếng Simon Willison chia sẻ mẹo làm việc với AI

5.

Thời gian chính là loại tài nguyên hữu hạn duy nhất của đời người mà không có khả năng tái tạo. Sử dụng dịch vụ trả phí của các mô hình AI lớn theo đánh giá của tôi chính là giải pháp tiết kiệm chi phí nhất để chúng ta mua thêm thời gian rảnh rỗi cho bản thân.

-- Trích bài viết [《Lời khuyên đừng nên quá đắn đo về các khoản phí đăng ký dịch vụ AI hàng tháng》](https://steipete.me/posts/2025/stop-overthinking-ai-subscriptions)

## 往年回顾

[Dự báo xu hướng phát triển của mô hình lập trình Low-code sẽ khó đi đến thành công](https://www.ruanyifeng.com/blog/2025/03/weekly-issue-341.html) (#341)

[Làn sóng công nghệ AI thực chất không có rào cản phòng thủ vững chắc](http://www.ruanyifeng.com/blog/2024/03/weekly-issue-291.html) (#291)

[Động lực tăng trưởng kinh tế của Trung Quốc đang dịch chuyển sâu vào nội địa](http://www.ruanyifeng.com/blog/2023/02/weekly-issue-241.html) (#241)

[Hành trình tự chủ tài chính cá nhân của một lập trình viên](http://www.ruanyifeng.com/blog/2022/01/weekly-issue-191.html) (#191)

(Hết)
