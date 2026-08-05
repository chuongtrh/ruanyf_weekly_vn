# 科技爱好者周刊（第 399 期）：中国 AI 大厂访问记 (Bản tin công nghệ hàng tuần số 399: Nhật ký ghé thăm các hãng AI lớn của Trung Quốc)

Ghi lại nội dung công nghệ đáng chia sẻ hàng tuần, phát hành vào thứ Sáu.

Bản tin này [mã nguồn mở](https://github.com/ruanyf/weekly), hoan nghênh bạn [đóng góp](https://github.com/ruanyf/weekly/issues). Ngoài ra còn có dịch vụ [《Ai đang tuyển dụng》](https://github.com/ruanyf/weekly/issues/10147) đăng tải thông tin tuyển dụng lập trình viên. Hợp tác vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图 (Ảnh bìa)

![](https://cdn.beekka.com/blogimg/asset/202606/bg2026060402.webp)

Bảo tàng Mỹ thuật Quốc tế Thâm Quyến vừa mở cửa đón khách vào tuần này. ([via](https://sa.trip.com/moments/detail/shenzhen-26-146282837?locale=en-SA))

## 中国 AI 大厂访问记 (Nhật ký ghé thăm các hãng AI lớn của Trung Quốc)

Vào đầu tháng 5 năm nay, một phái đoàn đại diện từ Mỹ đã đến Trung Quốc và ghé thăm 14 công ty chuyên về AI và robot.

![](https://cdn.beekka.com/blogimg/asset/202606/bg2026060104.webp)

Các đơn vị trong chuyến ghé thăm bao gồm DeepSeek, Moonshot AI (Nguyệt Chi Ám Diện), MiniMax, Zhipu AI (Trí Phổ), ByteDance, Alibaba, Ant Group, Xiaomi, 01.AI (Linh Nhất Vạn Vật), Unitree (Vũ Thụ), cộng đồng ModelScope (Ma Đáp), v.v.

Tất cả thành viên trong phái đoàn đều là các nhà phân tích công nghệ. Sau khi quay trở về Mỹ, mỗi người đều viết lại những quan sát của mình: [Kevin Xu](https://interconnect.substack.com/p/chinai-mood-april-26-may-4-2026), [Afra Wang](https://afraw.substack.com/p/mandate-of-ai), [Florian Brand](https://florianbrand.com/posts/china-trip), [Nathan Lambert](https://www.interconnects.ai/p/notes-from-inside-chinas-ai-labs), [Azeem Azhar](https://www.exponentialview.co/p/inside-chinese-ai-labs-efficiency-moat), [Lily Ottinger và Kai Williams](https://archive.md/myA7R), [Jasmine Sun](https://jasmi.news/p/party-in-the-permanent-underclass), [Lingua Sinica](https://linguasinica.substack.com/p/notes-from-a-trip-to-chinas-ai-labs), [Caithrin](https://www.caithrin.com/p/searching-for-amanda-askell-with).

Các bài viết này chứa đựng rất nhiều nội dung thú vị, tôi đã trích dẫn lại một số ý chính dưới đây. Để đảm bảo trải nghiệm đọc liền mạch, tôi xin phép không chú thích nguồn gốc riêng cho từng đoạn văn.

### 1. Khoảng cách về năng lực tính toán (Compute Power)

Tại mọi công ty ghé thăm, chúng tôi đều nghe thấy một lời phàn nàn chung: Thiếu hụt năng lực tính toán. Điều này làm giảm số lượng thử nghiệm khoa học và thu hẹp quy mô của các mô hình.

Tình trạng thiếu năng lực tính toán của Trung Quốc chủ yếu do chính sách kiểm soát xuất khẩu chip bán dẫn của Mỹ gây ra. Chúng tôi rất muốn trực tiếp chứng kiến các công ty bản địa đối phó với việc này như thế nào.

Mặc dù nguồn cung không hoàn toàn bị cắt đứt — các công ty Trung Quốc vẫn có cách tiếp cận được card đồ họa Nvidia H100, B200 và B300 — nhưng số lượng họ sở hữu ít hơn ít nhất một cấp độ quy mô so với các đối thủ cạnh tranh tại Mỹ.

Hệ thống GB300 NVL72 mới nhất của Nvidia (kết hợp 72 chip GPU Blackwell mới nhất thành một hệ thống đồng nhất) có tốc độ xử lý suy luận (inference) thực tế nhanh gấp 30 lần so với cụm H100 cách đây ba năm, dung lượng bộ nhớ mỗi chip cao hơn 3.6 lần và mức tiêu thụ điện năng cho mỗi lần suy luận giảm tới 25 lần. Các tập đoàn Mỹ đang đặt hàng hàng loạt hệ thống này, trong khi các công ty Trung Quốc hoàn toàn không thể làm vậy.

Các công ty công nghệ Trung Quốc, đặc biệt là Huawei, đã có những bước tiến vượt bậc trong việc tự nghiên cứu phát triển chip AI. Nhưng ngay cả chip mới nhất Ascend 950PR do Huawei công bố vào tháng 3 năm nay cũng chỉ có hiệu năng tương đương với dòng chip H100 ra mắt từ năm 2022 của Nvidia. Hơn thế nữa, sản lượng xuất xưởng của dòng chip này thấp hơn rất nhiều so với H100. Theo ước tính, chỉ riêng tính đến trước tháng 10 năm 2025, Nvidia đã xuất xưởng tới 7 triệu chip GPU Hopper và Blackwell, và tốc độ xuất xưởng vẫn đang tăng trưởng không ngừng. Huawei dự kiến xuất xưởng 750.000 chip Ascend 950PR trong năm nay, con số này chỉ bằng khoảng một phần mười sản lượng xuất xưởng năm ngoái của Nvidia.

Kết quả là Mỹ đang nắm giữ lợi thế dẫn đầu khổng lồ về năng lực tính toán. Chúng tôi ước tính vào cuối năm 2025, năng lực tính toán của ngành công nghiệp AI tại Mỹ sẽ lớn gấp khoảng 8 lần so với Trung Quốc. Tổng năng lực tính toán của các công ty AI Trung Quốc hiện tại chỉ tương đương với quy mô của Mỹ vào năm 2023.

Khi chúng tôi chia sẻ với các nhà nghiên cứu Trung Quốc về số lượng GPU trung bình mà mỗi kỹ sư nghiên cứu tại OpenAI được phân bổ, họ đều tỏ ra vô cùng kinh ngạc. Tuy nhiên, ai cũng biết rằng các kỹ sư nghiên cứu tại OpenAI, hay tại bất kỳ công ty AI phương Tây nào, vẫn liên tục phàn nàn rằng năng lực tính toán của họ quá ít.

### 2. Cách phân bổ năng lực tính toán

Ở Mỹ, phần lớn năng lực tính toán được ưu tiên cho việc huấn luyện mô hình (training) thay vì phục vụ người dùng. Nhưng ở Trung Quốc thì khác, năng lực tính toán vừa phải dùng để huấn luyện mô hình, vừa phải dùng để phục vụ cho hàng trăm triệu người tiêu dùng cá nhân và các doanh nghiệp đang tăng trưởng cực kỳ nhanh chóng.

Nếu phải cắt ra một nửa năng lực tính toán để phục vụ người dùng, lượng tài nguyên dùng cho huấn luyện mô hình đương nhiên sẽ bị giảm đi.

Còn một yếu tố khác cần xem xét: Năng lực tính toán tại Mỹ được tập trung chủ yếu trong tay năm tập đoàn lớn: OpenAI, Anthropic, Google, Meta và xAI. Trong khi đó ở Trung Quốc, các công ty công nghệ lớn nhỏ đều đang tích cực tự phát triển mô hình tiên phong của riêng mình, khiến tài nguyên tính toán vốn đã ít lại càng bị phân mảnh.

### 3. Hiệu quả tính toán

Theo logic đó, nếu năng lực tính toán của Trung Quốc đi sau Mỹ khoảng hai năm, thì các mô hình của Trung Quốc đáng lẽ cũng phải đi sau Mỹ ít nhất hai năm. Nhưng thực tế không phải như vậy.

Rất nhiều phân tích chỉ ra rằng các mô hình của Trung Quốc chỉ đi sau Mỹ vài tháng. Trên thực tế, ở một số khía cạnh cụ thể, mô hình của hai nước dường như đang chạy đua song song ngang hàng.

Nguyên nhân là chính các chính sách cấm vận chip lại vô tình thúc đẩy các công ty Trung Quốc phải tìm mọi cách nâng cao hiệu quả tính toán. Chúng tôi phát hiện ra rằng, trên mỗi đơn vị năng lực tính toán, mức độ thông minh của mô hình Trung Quốc đạt hiệu quả cao gấp 4 đến 7 lần so với việc nâng cấp cấu hình thông thường, điều này đã bù đắp phần nào sự thiếu hụt tài nguyên tính toán.

### 4. Bất đồng về nguồn mở (Open Source)

Hiện tại, những mô hình AI nguồn mở tốt nhất thế giới đều do các công ty Trung Quốc phát hành. Tuy nhiên, nội bộ các công ty Trung Quốc đang tồn tại những bất đồng lớn về việc có nên tiếp tục mở nguồn các mô hình tiếp theo hay không.

Tình hình tài chính và áp lực doanh thu của doanh nghiệp ảnh hưởng trực tiếp đến quyết định mở nguồn. Hiện tại, ranh giới cho việc mở nguồn đang ngày càng rõ ràng ở mốc: Quy mô tham số 1.000 tỷ (1T).

Một số công ty cho rằng việc mở nguồn các mô hình từ 1.000 tỷ tham số trở lên là hành vi lãng phí tài nguyên, bởi vì không ai có thể chạy nổi một mô hình khổng lồ như vậy trên các thiết bị cục bộ của họ, trong khi kịch bản ứng dụng điển hình của mô hình nguồn mở chính là chạy cục bộ. Phương án tốt hơn đối với mô hình quy mô này là tự host trên hạ tầng đám mây của doanh nghiệp và cung cấp thông qua cổng API để người dùng dễ dàng sử dụng.

Nhưng đối với một số công ty khác, mô hình nguồn mở gần như là một đức tin, và việc xây dựng các mô hình quy mô nghìn tỷ tham số chính là tấm vé gia nhập vào cộng đồng nguồn mở toàn cầu.

### 5. Phong cách "Tây hóa" hay "Trung Quốc hóa"

Một số công ty AI Trung Quốc mang phong cách "Tây hóa" điển hình, tràn ngập không khí hiện đại và ngầu của Thung lũng Silicon, thể hiện rõ ngay cả trên những món quà lưu niệm họ tặng khách.

Một số công ty khác lại ngày càng "Trung Quốc hóa", coi việc xây dựng một phòng trưng bày hoành tráng, hào nhoáng là nhiệm vụ hàng đầu. Những phòng trưng bày này dùng để tiếp đón các đoàn khách tham quan, thường là CEO của các doanh nghiệp nhà nước hoặc lãnh đạo chính quyền địa phương. Sau chuyến tham quan luôn đi kèm các buổi tiệc chiêu đãi.

Tôi nghĩ đây vừa là sự lựa chọn chủ động, vừa là sự bắt buộc tùy thuộc vào nền tảng của nhà sáng lập cũng như tệp khách hàng mà công ty hướng tới.

### 6. Cách họ nhìn nhận về các đối thủ cạnh tranh

Chúng tôi nhận thấy mọi công ty AI Trung Quốc đều kính nể bộ phận Seed của ByteDance. Đó là đội ngũ nghiên cứu AI tiên phong đóng nguồn duy nhất tại Trung Quốc. Họ giống như một chú voi khổng lồ trong phòng nhưng lại có thể nhảy múa vô cùng linh hoạt. Ứng dụng Doubao của họ gần như độc chiếm lượng traffic người dùng AI, mô hình của họ có thể nhanh chóng tiếp cận lượng người dùng khổng lồ mà không công ty nào khác có thể so sánh được.

DeepSeek lại là công ty nhận được sự tôn trọng lớn nhất trong ngành, họ ngày càng đảm nhận nhiều phần việc ở tầng nền tảng cốt lõi: Kiến trúc mô hình, tối ưu hóa hiệu quả, tối ưu hóa suy luận và tương thích hóa với ngăn xếp giao thức của Huawei.

### 7. Lực lượng thực tập sinh

Nhân viên tại các công ty AI Trung Quốc phần nhiều là các "thực tập sinh" cực kỳ tài năng, độ tuổi trung bình khoảng 25-26 tuổi, hầu hết đang là nghiên cứu sinh tiến sĩ và có thể giao tiếp chuyên môn trơn tru bằng tiếng Anh. Phần lớn họ tốt nghiệp từ các trường đại học trong nước và không có kinh nghiệm đi du học.

Họ thực tập trong khoảng từ một đến hai năm, được hưởng mọi đãi ngộ và quyền hạn đầy đủ như nhân viên chính thức, có thể tự do đề xuất ý tưởng và chạy thử nghiệm các dự án. Điều này hoàn toàn trái ngược với các công ty AI hàng đầu phương Tây như OpenAI, Anthropic, Cursor khi họ hoàn toàn không tuyển thực tập sinh, còn các công ty khác (như Google) tuy có tuyển thực tập sinh cho dự án Gemini nhưng chỉ giao các phần việc phụ không mấy quan trọng.

Các công ty Trung Quốc coi trọng nguồn nhân lực trẻ này vì họ mang lại những ý tưởng mới mẻ và sức sáng tạo dồi dào. Để cải thiện mô hình cuối cùng, các thực tập sinh sẵn sàng làm cả những công việc tẻ nhạt không mấy ai chú ý. Đồng thời, những người mới tiếp cận mảng AI sẽ không bị ảnh hưởng bởi tư duy lối mòn cũ.

Đứng từ góc độ các trường đại học Trung Quốc, tài nguyên tính toán của nhà trường hoàn toàn không đủ để các sinh viên xuất sắc phát huy tài năng, vì thế việc gửi họ đến thực tập tại các công ty công nghệ có hạ tầng tính toán mạnh mẽ là phương án tối ưu, giúp hai bên cùng hợp tác xuất bản các bài báo khoa học và đạt được lợi ích song phương.

### 8. Thái độ đối với vấn đề an toàn AI

Khi tôi hỏi một số nhà nghiên cứu trẻ Trung Quốc về góc nhìn của họ đối với AGI (Trí tuệ nhân tạo tổng quát), họ đều đưa ra câu trả lời giống nhau: "AGI chính là lúc trí tuệ nhân tạo có thể thay thế tôi làm việc!"

Tôi nhận thấy họ không hề bày tỏ sự lo lắng hay sợ hãi việc bị thay thế, ngược lại họ vô cùng tò mò muốn xem liệu máy móc có thực sự vượt qua được con người tạo ra nó hay không. Nếu điều đó thực sự xảy ra, họ sẵn sàng chuyển sang làm việc khác.

Điều này trái ngược với các đồng nghiệp phương Tây, những người luôn cực kỳ lo ngại về vấn đề an toàn AI và các tác động xã hội của nó. Các nhà nghiên cứu Trung Quốc cũng coi trọng an toàn, ai cũng đồng ý rằng AI không được làm việc xấu. Nhưng làm sao để đảm bảo điều đó, họ tin rằng đó là nhiệm vụ của chính phủ và chính phủ sẽ có cách giải quyết.

### 9. Nhu cầu dịch vụ AI của doanh nghiệp Trung Quốc

Các doanh nghiệp Trung Quốc có sẵn sàng chi tiền mua dịch vụ AI trong nước hay không?

Một quan điểm phổ biến cho rằng thị trường AI của Trung Quốc quy mô rất nhỏ vì các doanh nghiệp nước này thường không có thói quen trả tiền cho phần mềm, do đó khó có thể nuôi sống các công ty AI bản địa.

Nhận định này chỉ đúng với các chi phí phần mềm mô hình SaaS, vốn dĩ có thị trường rất nhỏ tại Trung Quốc. Tuy nhiên, Trung Quốc lại sở hữu một thị trường điện toán đám mây khổng lồ.

Các công ty AI Trung Quốc đang tranh luận xem các doanh nghiệp sẽ coi dịch vụ AI là một sản phẩm SaaS (thị trường nhỏ) hay là hạ tầng điện toán đám mây (thị trường lớn)? Hiện tại xu hướng phát triển của AI đang nghiêng hẳn về hướng điện toán đám mây.

### 10. Ngành công nghiệp dữ liệu kém phát triển hơn Mỹ

Chúng tôi được biết các công ty AI của Mỹ như Anthropic hay OpenAI chi ra tới hơn 10 triệu USD mỗi năm để mua dữ liệu huấn luyện (hoặc môi trường học tăng cường), tổng chi phí tích lũy có thể lên tới hàng trăm triệu USD. Chúng tôi tò mò muốn biết liệu các công ty AI Trung Quốc có làm vậy không.

Câu trả lời nhận được là Trung Quốc gần như không có ngành công nghiệp dữ liệu thương mại, vì các công ty AI nhận thấy chất lượng dữ liệu thương mại bán ngoài thị trường rất kém, do đó họ tự chuẩn bị dữ liệu thủ công sẽ mang lại kết quả tốt hơn nhiều.

Các nhà nghiên cứu dành phần lớn thời gian để tự xây dựng môi trường huấn luyện học tăng cường, còn các tập đoàn lớn như ByteDance hay Alibaba thì có sẵn các đội ngũ dán nhãn dữ liệu (data labeling) nội bộ để hỗ trợ việc này.

### 11. Vai trò của chính phủ

Ai mới là người thực sự đứng sau thúc đẩy lĩnh vực AI tại Trung Quốc? Tương đương với các quỹ đầu tư mạo hiểm Sequoia Capital hay a16z tại Silicon Valley.

Một người bạn của tôi đã đưa ra câu trả lời: Chính quyền các thành phố Thượng Hải, Bắc Kinh và Hàng Châu. Những vị cán bộ chính quyền mẫn cán nhưng cũng đầy mệt mỏi này, bị thúc đẩy bởi tâm lý sợ bỏ lỡ (FOMO) và áp lực cạnh tranh sâu sắc, đang nỗ lực thúc đẩy ngành công nghiệp AI của địa phương mình bằng mọi giá.

## [Hoạt động] Trại thực tế sinh viên XEngineer

*(Phần này giới thiệu về chương trình XEngineer, giữ nguyên cấu trúc quảng cáo và thông tin liên hệ đăng ký).*

## 文章 (Bài viết)

1、[Trải nghiệm dùng AI tìm Bug của tôi](https://newsletter.semianalysis.com/p/finding-miscompiles-for-fun-not-profit) (Tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026053001.webp)

Tác giả sử dụng AI để dò tìm lỗi Bug của trình biên dịch (compiler), kết quả phát hiện ra chi phí vận hành AI đắt hơn cả mức lương của ông một cấp độ quy mô. Tuy nhiên nếu chấp nhận trả chi phí cao hơn, AI thực sự có thể tìm ra được nhiều lỗi hơn nữa. Đây là lần đầu tiên ông cảm thấy giá trị của AI vượt qua giá trị sức lao động của chính mình.

2. [Kiểm tra sức khỏe nút mạng trong cân bằng tải](https://singh-sanjay.com/2026/01/12/health-checks-client-vs-server-side-lb.html) (Tiếng Anh)

Bài viết giới thiệu cơ chế cân bằng tải có thể thực hiện ở phía máy chủ hoặc phía client, và cách kiểm tra phát hiện các nút mạng gặp sự cố trong cả hai trường hợp đó.

3. [Bốn trường hợp có thể dùng HTML thay thế JS](https://www.htmhell.dev/adventcalendar/2025/27/) (Tiếng Anh)

Bài viết chứng minh sức mạnh của HTML + CSS hiện tại đã đủ mạnh để xử lý nhiều tác vụ trước đây bắt buộc phải dùng JS, ví dụ như các hộp thoại popup hay tooltip hiển thị đè.

4. [Cách liên kết số điện thoại trên trang web](https://sethmlarson.dev/mobile-browsers-and-telephone-numbers) (Tiếng Anh)

Khi trình duyệt di động mở trang web có chứa số điện thoại, nó sẽ tự động tạo liên kết để người dùng click vào là có thể gọi điện. Bài viết hướng dẫn cách tùy chỉnh hành vi này, bao gồm cả việc hủy bỏ liên kết tự động hoặc thay đổi số điện thoại thực tế khi nhấn gọi.

5. [Sử dụng phần tử HTML tự định nghĩa](https://maurycyz.com/misc/make-up-tags/) (Tiếng Anh)

Trang web hoàn toàn có thể sử dụng các thẻ HTML tự định nghĩa thay thế cho thẻ `div` thông thường để tăng tính ngữ nghĩa (semantic structure) cho mã nguồn.

6. [Vực thẳm Challenger sâu cỡ nào](https://storymaps.arcgis.com/stories/0d389600f3464e3185a84c199f04e859) (Tiếng Anh)

Một bài viết đồ họa sinh động giới thiệu chi tiết về nơi sâu nhất trên Trái Đất — Vực thẳm Challenger (Challenger Deep) với độ sâu khoảng 11.000 mét.

## 工具 (Công cụ)

1、[Breathe CLI](https://github.com/marekkowalczyk/breathe-cli)

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026053103.webp)

Ứng dụng dòng lệnh cho macOS hiển thị một thanh tiến trình hướng dẫn người dùng tập hít thở chậm (khoảng 6 lần mỗi phút) để cải thiện chức năng tim mạch.

2、[NMLinux](https://github.com/thongor77/nmlinux)

Giao diện đồ họa quản lý kết nối mạng dành cho hệ điều hành Linux.

3、[Penpot](https://github.com/penpot/penpot)

Công cụ thiết kế UI/UX nguồn mở có thể thay thế cho Figma, hỗ trợ chuyển đổi bản vẽ thiết kế trực quan thành mã nguồn CSS + HTML.

4、[sky adb](https://github.com/sky22333/skyadb)

Công cụ quản lý ADB chạy trực tiếp trên điện thoại Android, giúp quản lý điện thoại, máy tính bảng và TV box thông qua kết nối WiFi ADB. (Đóng góp từ [@sky22333](https://github.com/ruanyf/weekly/issues/10101))

5、[readNeo](https://github.com/extrastu/readneo)

Bảng quản trị dữ liệu đọc sách WeChat Reading. Kết nối với Skill API của WeChat Reading để hiển thị tủ sách trực quan, thống kê thời gian đọc, quản lý các trích dẫn và hỗ trợ xuất dữ liệu nhanh. (Đóng góp từ [@extrastu](https://github.com/ruanyf/weekly/issues/10110))

6、[AppPorts](https://github.com/wzh4869/AppPorts)

Công cụ nguồn mở cho macOS giúp di chuyển các ứng dụng cài trên máy sang ổ cứng ngoài mà vẫn giữ cho chúng hoạt động bình thường, hỗ trợ khôi phục lại bất cứ lúc nào. (Đóng góp từ [@wzh4869](https://github.com/ruanyf/weekly/issues/10119))

7、[欢乐斗地主 (Fight the Landlord)](https://github.com/palemoky/fight-the-landlord)

Trò chơi đấu địa chủ nguồn mở chạy ngay trên terminal viết bằng ngôn ngữ Go, hỗ trợ chơi online ghép bàn, tự động kết nối lại khi mất mạng và có tích hợp robot thông minh chơi cùng. (Đóng góp từ [@palemoky](https://github.com/ruanyf/weekly/issues/10149))

8、[fuckssh](https://github.com/hczs/fuckssh)

Công cụ dòng lệnh đóng gói sẵn các lệnh SSH, cung cấp giao diện tương tác từng bước giúp dễ dàng cấu hình khóa bảo mật máy chủ. (Đóng góp từ [@hczs](https://github.com/ruanyf/weekly/issues/10184))

9、[StarGuard](https://github.com/m-ahmed-elbeskeri/Starguard)

Công cụ Python hỗ trợ quét kiểm tra xem một kho lưu trữ GitHub có sử dụng các tài khoản bot ảo để tăng lượt đánh giá sao (star) hay không.

10、[Nginx Proxy Manager](https://github.com/NginxProxyManager/nginx-proxy-manager)

Công cụ quản lý proxy ngược Nginx qua giao diện web, hỗ trợ tự động cấu hình và kích hoạt chứng chỉ bảo mật SSL.

## AI 相关 (AI Liên quan)

1、[Bảng xếp hạng tỷ lệ trúng cache của mô hình lớn](https://dirac.run/posts/cache-hit-rates-agents)

Giúp người dùng chọn lựa các mô hình có tỷ lệ trúng cache tốt nhằm tối ưu hóa chi phí gọi API.

2、[Endless Toil](https://github.com/AndrewVos/endless-toil)

Một plugin đùa vui cho Codex và Claude Code, phát ra tiếng rên rỉ khi AI đọc code. Code càng tệ tiếng rên rỉ càng lớn.

3、[Lightpanda Browser](https://github.com/lightpanda-io/browser)

Trình duyệt không đầu chuyên dụng chạy tác vụ AI, tiêu thụ RAM siêu nhẹ.

## 资源 (Tài nguyên)

1、[API thơ cổ Trung Quốc](https://github.com/palemoky/chinese-poetry-api)

Dịch vụ tra cứu thơ cổ viết bằng ngôn ngữ Go, có thể deploy nhanh lên Cloudflare. (Đóng góp từ [@palemoky](https://github.com/ruanyf/weekly/issues/10216))

2、[Các mẫu lập trình được kiểm chứng thực tế](https://totoro-jam.github.io/battle-tested-patterns/zh/patterns/) (Battle-Tested Patterns)

Tổng hợp 46 mẫu lập trình kèm code mẫu từ dự án thực tế. (Đóng góp từ [@Totoro-jam](https://github.com/ruanyf/weekly/issues/10257))

3、[WorldIP.io](https://worldip.io/)

Trang web tra cứu thông tin chi tiết địa chỉ IP miễn phí.

## 图片 (Hình ảnh)

1、[Phép chiếu hình trụ (圆柱投影)](https://liorsinai.github.io/mathematics/2020/08/27/secant-mercator.html)

Mô phỏng phép chiếu tọa độ bề mặt địa cầu lên một mặt phẳng hình trụ bao quanh trái đất để vẽ bản đồ thế giới phẳng.

## 文摘 (Văn trích)

1、[Khi nào kỹ sư phần mềm nên nghỉ hưu](https://thecodist.com/how-to-know-when-its-time-to-go/)

Trải qua một năm cân nhắc, tôi đã quyết định nghỉ hưu và rời bỏ công việc lập trình viên. Lý do không phải vì năng lực kém mà là vì tôi không còn muốn tiếp tục làm việc này nữa.

Ai rồi cũng đến một thời điểm không thể làm công việc mình đã làm cả đời. Việc này không liên quan đến tuổi tác, tôi biết nhiều lập trình viên trẻ hơn tôi rất nhiều cũng đã bỏ nghề.

Các lý do nghỉ hưu phổ biến bao gồm: (1) Năng lực không còn đáp ứng được yêu cầu công việc; (2) Không còn hứng thú với ngành công nghiệp này; (3) Thị trường việc làm đi xuống hoặc công ty đóng cửa; (4) Công nghệ thay đổi khiến kỹ năng cũ lỗi thời; (5) Tìm thấy đam mê mới; (6) Đã tích lũy đủ tài chính và cảm thấy kiệt sức, không còn động lực làm việc.

Tôi thích làm việc để tạo ra sự thay đổi và chinh phục các thử thách ý nghĩa. Tiền rất quan trọng, nhưng niềm vui tạo ra giá trị mới là thứ giữ chân tôi. Việc chủ động đưa ra quyết định nghỉ hưu sáng suốt khi nhận thấy mình bắt đầu tụt lại phía sau tốt hơn nhiều so với việc bị ép buộc phải rời bỏ ngành.

## 言论 (Phát ngôn)

1、

> "Nếu cuộc đời là một chiếc hộp, bất kỳ ai cố gắng mở rộng chiếc hộp đó ra đều sẽ nhận ra họ buộc phải đập vỡ bốn bức vách của nó mới được."
> 
> -- Charlie Munger, nhà đầu tư huyền thoại người Mỹ.

2、

> "Các lập trình viên sẵn sàng viết tài liệu vô cùng chi tiết cho AI đọc, nhưng lại kiên quyết không chịu viết tài liệu cho các lập trình viên khác đọc."
> 
> -- plover.com

3、

> "Tốc độ của AI quá nhanh đôi khi khiến tôi bực mình. Tôi vừa nghĩ bụng 'Cứ để AI tự viết code rồi mình đi ngủ trưa một lát', kết quả là tôi còn chưa kịp rời khỏi ghế thì nó đã viết xong code rồi."
> 
> -- Độc giả Hacker News

4、

> "Quy trình phát triển phần mềm truyền thống đang tan rã khi AI có thể đồng thời tự viết code, tự viết test và tự động deploy hệ thống."
> 
> "Kỹ năng mới cần trang bị là kỹ nghệ ngữ cảnh (context engineering), và chốt chặn bảo mật mới chính là khả năng giám sát (observability)."
> 
> -- 《Quy trình phát triển phần mềm truyền thống đã chết》

5、

> "Tôi luôn tin rằng việc tạo ra một trí tuệ nhân tạo thông minh hơn con người là cực kỳ mạo hiểm. Sự nguy hại của nó đối với loài người có lẽ cũng không kém gì những gì con người đã gây ra cho loài tinh tinh và chim dodo."
> 
> -- 《Thiết kế phần mềm trong thời đại AI》

## 往年回顾 (Nhìn lại các năm trước)

[Bug tracking system thế hệ mới trông như thế nào?](https://www.ruanyifeng.com/blog/2025/06/weekly-issue-352.html)（＃352）

[Khởi nghiệp tuy tốt, nhưng tôi không dám khuyến khích nữa](https://www.ruanyifeng.com/blog/2024/05/weekly-issue-302.html)（#302）

[Khởi nghiệp Internet ngày càng trở nên khó khăn](https://www.ruanyifeng.com/blog/2023/04/weekly-issue-252.html)（#252）

[Ba phương pháp học tập đầy tính gợi mở](https://www.ruanyifeng.com/blog/2022/04/weekly-issue-202.html)（#202）

(Hết)
