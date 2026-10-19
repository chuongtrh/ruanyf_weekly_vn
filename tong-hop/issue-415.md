# Tuần san công nghệ số 415: Phiên bản 3D của “Những thành phố vô hình”

> **Tên gốc:** 科技爱好者周刊（第 415 期）：3D 版《看不见的城市》  
> **Tác giả:** 阮一峰 (Nguyễn Nhất Phong)  
> **Phát hành:** 16/10/2026  
> **Tổng hợp:** 19/10/2026  
> **Nguồn chính:** https://www.ruanyifeng.com/blog/2026/10/weekly-issue-415.html  
> **Loại nội dung:** Ghi chú đọc và phân tích bằng tiếng Việt; không phải bản dịch nguyên văn.

## Mục lục

1. [Tổng quan và các ý chính](#1-tổng-quan-và-các-ý-chính)
2. [AI dựng 55 thành phố văn học thành không gian 3D](#2-ai-dựng-55-thành-phố-văn-học-thành-không-gian-3d)
3. [Máy tính hình bóng đèn](#3-máy-tính-hình-bóng-đèn)
4. [Deno và sức mạnh của hệ sinh thái Node.js](#4-deno-và-sức-mạnh-của-hệ-sinh-thái-nodejs)
5. [Sáu bài đọc đáng chú ý](#5-sáu-bài-đọc-đáng-chú-ý)
6. [Mười lăm công cụ](#6-mười-lăm-công-cụ)
7. [Tài nguyên, hình ảnh và trích đoạn](#7-tài-nguyên-hình-ảnh-và-trích-đoạn)
8. [Những câu nói đáng nhớ](#8-những-câu-nói-đáng-nhớ)
9. [Góc nhìn AI và bài học cho kỹ sư](#9-góc-nhìn-ai-và-bài-học-cho-kỹ-sư)
10. [Kết luận](#10-kết-luận)

## 1. Tổng quan và các ý chính

Số 415 xoay quanh sự chuyển dịch của AI: từ mô hình tạo văn bản, ảnh hoặc đoạn mã riêng lẻ sang tác nhân có thể tạo **toàn bộ ứng dụng tương tác**, điều khiển máy tính và phối hợp nhiều bước. Chủ đề đầu tiên đưa AI vào một thử thách khó: chuyển 55 thành phố chỉ tồn tại trong lời văn của Italo Calvino thành 55 cảnh ba chiều có thể khám phá. Chủ đề tiếp theo là thiết bị trình chiếu thông minh có hình bóng đèn, một cách hình dung máy tính không phụ thuộc màn hình cá nhân. Cuối cùng, tin về Deno trở thành một trường hợp điển hình cho việc thiết kế kỹ thuật tốt chưa đủ để thắng đối thủ có hệ sinh thái lớn.

Ba kết luận cần nhớ: (1) đầu ra chạy được khác xa đầu ra truyền tải đúng *ý định*; (2) khả năng tạo phần mềm bằng AI không thay thế kiểm thử, tối ưu hiệu năng và thiết kế giao diện; (3) hệ sinh thái và khả năng tương thích thường có giá trị kinh tế lớn hơn một số cải tiến đơn lẻ.

## 2. AI dựng 55 thành phố văn học thành không gian 3D

### Từ văn học sang yêu cầu thiết kế

*Những thành phố vô hình* (*Invisible Cities*, 1972) của nhà văn Ý Italo Calvino kể về Marco Polo thuật lại cho Hốt Tất Liệt 55 thành phố tưởng tượng. Những nơi đó không có bản vẽ sẵn, chỉ có mô tả bằng lời. Mỗi thành phố thể hiện một ý niệm về ký ức, khát vọng, thời gian, cảm giác hoặc đời sống. Dựng hình từ các mô tả này không chỉ là chuyển chữ thành vật thể: người dựng phải hiểu **chủ đề cảm xúc** và chuyển nó thành bố cục, ánh sáng, chất liệu, góc nhìn.

Piotr Migdał thử yêu cầu GPT-6 Astra qua Codex và Claude Opus 5.5 qua Claude Code tạo một ứng dụng Three.js cho toàn bộ 55 thành phố. [Bài thử nghiệm của Piotr Migdał](https://quesma.com/) được tuần san dẫn lại; tác giả cũng công bố các bản tương tác và mã nguồn qua liên kết ở [bài gốc](https://www.ruanyifeng.com/blog/2026/10/weekly-issue-415.html).

Theo đánh giá của người thử, cả hai đều xây được ứng dụng nhưng kết quả mang tính thẩm mỹ rất khác nhau. GPT-6 Astra thiên về hình khối và các thành phố dễ trông giống nhau. Claude Opus 5.5 tạo được sự phân biệt rõ hơn giữa các thành phố, bám tốt hơn không khí của các đoạn văn. Đây **không phải bảng xếp hạng năng lực mô hình**: hai quy trình, số tác nhân, thời gian và chi phí không đồng nhất.

### Irene: mô tả một thành phố ánh sáng

Trong tiểu thuyết, Irene được nhìn từ một nơi cao, thấp thoáng ánh sáng hồng, các ô cửa có đèn, khoảng tối của vườn và tháp tín hiệu. Một phiên bản 3D tốt phải tái hiện khoảng cách và bầu không khí mờ ảo, chứ không chỉ vẽ nhà. Theo tác giả tuần san, bản Claude thể hiện góc nhìn và ánh sáng hiệu quả hơn. Trường hợp này cho thấy kiểm tra **đủ đối tượng đồ họa** chưa nói lên việc người xem có cảm nhận được đặc trưng văn học hay không.

### Isidora: hình ảnh của tuổi trẻ và ký ức

Isidora là thành phố người lữ khách từng mơ ước, nhưng đến lúc đặt chân tới, người ấy đã già. Những công trình và cảnh tượng đáng ao ước còn nguyên; điều thay đổi là chính người đến. Phiên bản 3D có thể dựng tháp và cầu thang nhưng dễ làm mất ý trọng tâm: **mong muốn đã biến thành ký ức**. Tuần san đánh giá phiên bản Claude bổ sung được hình ảnh con người ngồi tại quảng trường, gần với không khí của tác phẩm hơn.

### Những giới hạn còn lại

Ứng dụng được tạo với Three.js, cho phép xoay, phóng to và quan sát cảnh trong trình duyệt. Tuy nhiên mô hình cảnh phức tạp kéo theo dung lượng tải lớn và trải nghiệm ban đầu chậm. Ở quy mô triển khai, cần đo thời gian tải, tốc độ khung hình, bộ nhớ và khả năng mở trên điện thoại.

Hai dự án khác được giới thiệu là [Sakura Fantasy](https://github.com/) — chuyến thuyền qua cảnh vật có thể đổi mùa, giờ trong ngày và thời tiết — cùng *Cyber Kowloon*, một bản dựng khu Cửu Long với 9.373 tòa nhà. Các đường dẫn cụ thể có trên [số 415](https://www.ruanyifeng.com/blog/2026/10/weekly-issue-415.html).

**Bình luận:** Đây là sự chuyển dịch từ yêu cầu “AI hãy tạo một hình minh họa” sang “AI hãy tạo một hệ thống hình học có cấu trúc và tương tác”. Việc đánh giá phải có cả tiêu chí nội dung, trải nghiệm, hiệu năng lẫn bảo trì.

## 3. Máy tính hình bóng đèn

Dự án [Lightbulb Computer](https://lightbulbcomputer.com/) hình dung một thiết bị kết hợp máy chiếu, camera, nhận dạng hình ảnh, cử chỉ và lời nói. Thay vì bắt người dùng nhìn vào điện thoại hoặc đeo kính, thông tin được chiếu lên tường, bàn, sách và đồ vật xung quanh. Khi nấu ăn có thể nhìn công thức trên tường; khi đọc sách có thể chỉ vào trang để hỏi; bản đồ có thể được chiếu trên bàn để nhiều người cùng xem.

Điểm đáng chú ý là **giao diện chung cho nhiều người**: màn hình kính thông minh mang tính cá nhân, trong khi hình ảnh chiếu vào không gian có thể cùng được quan sát. Nhà thiết kế cũng nhấn mạnh các hạn chế phần cứng của kính, đặc biệt về pin, nhiệt và trọng lượng.

Đây vẫn là nguyên mẫu ý tưởng, chưa phải bóng đèn thương mại nhỏ gọn. Những rủi ro thực tế gồm độ sáng trong phòng, độ trễ, nhận dạng sai cử chỉ, góc chiếu và riêng tư khi camera có thể quan sát không gian gia đình. Nó cho thấy AI có thể đổi mới giao diện máy tính, không chỉ cải thiện ứng dụng hiện có.

## 4. Deno và sức mạnh của hệ sinh thái Node.js

Ngày 09/10/2026, nhóm Deno [thông báo gia nhập Cloudflare](https://deno.com/). Theo kế hoạch công bố, Deno Runtime chủ yếu nhận sửa lỗi và cập nhật bảo mật trong khoảng một năm, rồi nhóm hiện tại dừng phát triển; Deno Deploy có lộ trình kết thúc ngắn hơn, còn JSR và một số thành phần khác tiếp tục theo kế hoạch riêng. **Mã nguồn mở không biến mất**, và cộng đồng vẫn có thể duy trì về sau.

Deno do Ryan Dahl, người tạo Node.js, khởi xướng. Ý tưởng ban đầu là làm lại môi trường chạy JavaScript với bảo mật theo quyền, hỗ trợ TypeScript và quản lý phụ thuộc đơn giản hơn. Dự án giải quyết được nhiều điểm bất tiện, nhưng khó vượt qua khối lượng thư viện, tài liệu, nhân sự và ứng dụng sẵn có của Node.js.

Đến Deno 2.0 năm 2024, khả năng tương thích Node.js trở thành ưu tiên lớn. Chính việc hỗ trợ đối thủ quá giống có thể làm giảm lý do chuyển từ Node sang Deno. Nếu đã chạy tốt trên Node, doanh nghiệp cần một lợi ích đủ lớn để bù mọi chi phí di chuyển.

**Bài học kỹ thuật:** đừng chỉ so sánh số liệu hiệu năng hay thiết kế API. Hãy đánh giá khả năng tuyển dụng, thư viện, công cụ triển khai, hỗ trợ dài hạn, chi phí vận hành và tính tương thích. Cũng không nên đánh đồng dự án không thắng thị phần với dự án không tạo ảnh hưởng: nhiều ý tưởng của đối thủ mới có thể thúc đẩy nền tảng cũ cải tiến.

## 5. Sáu bài đọc đáng chú ý

### 5.1. DeskMind: tự huấn luyện tác nhân điều khiển Mac với khoảng 600 USD

Tác giả [DeskMind](https://deskmind.dev/) kể quá trình ba tuần, khoảng 20 vòng tinh chỉnh dựa trên các mô hình Qwen3.5 cỡ 0,8B và 4B, cho tác nhân quan sát màn hình và quyết định nhấp, gõ, hỏi người dùng hoặc dừng nhiệm vụ. Hệ thống chạy với MLX trên Apple Silicon.

Kiến trúc hai tầng đặc biệt đáng chú ý: mô hình nhỏ xử lý việc dễ; khi ít tin cậy hoặc hành động có rủi ro, chuyển lên mô hình lớn. Tuy vậy nhiều bước vẫn phải leo thang, nên việc tiết kiệm tài nguyên chưa tối ưu.

Hai chi tiết quan trọng: gặp hai đơn hàng có cùng tên, tác nhân phải **hỏi thay vì đoán**; khi tác nhân tuyên bố xong, bộ điều khiển phải **kiểm tra trạng thái thật** trước khi công nhận. Bộ thử nghiệm 39/39 trên tập nhiệm vụ nhỏ không thể được hiểu là độ tin cậy tuyệt đối cho mọi ứng dụng.

### 5.2. Vì sao phần mềm điều khiển tên lửa hạn chế cấp phát động?

Bài viết về quy tắc lập trình C trong hệ thống an toàn cao giải thích lý do tránh những thao tác như malloc/free ở thành phần yêu cầu thời gian đáp ứng dự đoán được: cấp phát có độ trễ biến động, có thể phân mảnh bộ nhớ và tăng nguy cơ rò rỉ, truy cập sau giải phóng. Cách tổ chức bộ nhớ phụ thuộc tiêu chuẩn và hệ thống cụ thể; không phải mọi chương trình nhúng đều cấm tuyệt đối.

### 5.3. Làm cho giao diện web do AI tạo có chất lượng thiết kế

[Bài của Railcode](https://railcode.dev/) bàn về chất lượng thiết kế khi lập trình bằng AI. Không nên chỉ ra lệnh “làm đẹp hơn”: hãy định nghĩa quy tắc kiểu chữ, khoảng cách, màu, thành phần và trường hợp sử dụng, sau đó đánh giá bằng hình ảnh thực tế.

### 5.4. Vì sao điện thoại Linux độc lập khó cạnh tranh?

[Bài phân tích trên WordPress](https://amosbbatto.wordpress.com/) xem xét khó khăn của Linux điện thoại ngoài hệ Android: hỗ trợ SoC, trình điều khiển modem, camera, GPU, tiết kiệm pin, ứng dụng và nhà mạng. Nhân Linux không đủ để hình thành một sản phẩm di động hoàn chỉnh.

### 5.5. Vì sao AMD tăng hiệu năng mạnh qua vài thế hệ?

[Bài của Daniel Lemire](https://lemire.me/) so sánh Ryzen 7 5800X3D, 7800X3D và 9800X3D. Điểm nhấn: xung nhịp chỉ là một phần; số lệnh xử lý trên một chu kỳ, bộ nhớ đệm, các đơn vị thực thi, khả năng thực thi song song và véc-tơ cũng đóng vai trò lớn. Kết quả bài đo cụ thể không đồng nghĩa tất cả phần mềm đều tăng hiệu năng tương ứng.

### 5.6. Người làm công ăn lương vẫn có thể tích lũy tài sản

[Bài của Asher Adeniyi](https://asheradeniyi.com/) bàn về việc phát triển kỹ năng có giá trị, đo được tác động nghề nghiệp, kiểm soát chi tiêu và tích lũy dài hạn. Thu nhập là dòng tiền; tài sản là phần giá trị giữ lại sau quá trình tiêu dùng và đầu tư. Đây là nguyên tắc tổng quát, không phải khuyến nghị mua bán cụ thể.

## 6. Mười lăm công cụ

| Công cụ | Công dụng và điều cần chú ý |
|---|---|
| [REA](https://github.com/) | Dùng AI hỗ trợ phân tích ngược chương trình; cần lưu ý giấy phép và quyền tác giả |
| [SynthID Detector](https://synthid.com/) | Phát hiện dấu nhận dạng tương thích của nội dung AI; không phát hiện không chứng minh là nội dung do người tạo |
| ts-rust | Thử nghiệm trình biên dịch TypeScript viết bằng Rust; cần kiểm chứng tương thích |
| Doory | Công cụ thiết kế đồ họa trên trình duyệt, hướng tới lựa chọn nguồn mở cho Canva |
| HeadOrbit | Điều khiển Mac bằng chuyển động đầu qua cảm biến của AirPods |
| qrypt | Gắn kho lưu trữ đám mây thành thư mục trên máy |
| EdgeSSH | Giao diện web quản lý SSH/VPS trên hạ tầng Cloudflare |
| charts-rs | Tạo SVG và biểu đồ bằng Rust, không phụ thuộc trình duyệt |
| ItsPaint | Bảng vẽ và công cụ chú thích ảnh chụp màn hình trên macOS |
| Caplo | Quay màn hình Mac, tự phóng lớn quanh thao tác nhấp |
| bg2x | Phóng lớn ảnh bằng AI ngay trong trình duyệt |
| [EnvTrace](https://envtrace.net/) | Kiểm tra dấu vân tay và các tín hiệu rò rỉ của trình duyệt |
| Droidline | Điều khiển Android bằng tập lệnh sau khi ghép nối |
| ESP32 iPhone Agent | Thử dùng bo mạch ESP32-S3 để hỗ trợ tự động hóa iPhone |
| Bulchimbeon | Giữ Mac thức khi tác nhân lập trình làm việc, có cơ chế xử lý pin và nhiệt độ |

**Ứng dụng thực tế:** charts-rs đáng xem để sinh biểu đồ tự động từ Go hoặc dịch vụ khác; Caplo thích hợp khi quay hướng dẫn; Droidline và ESP32 iPhone Agent phục vụ các thí nghiệm tác nhân điều khiển thiết bị; Bulchimbeon nhắm đúng vấn đề tác nhân chạy lâu trên Mac. Các dự án nhỏ cần được thử khả năng ổn định trước khi áp dụng cho môi trường quan trọng.

Thông tin và các liên kết mã nguồn từng công cụ được tác giả tập hợp trong [mục 工具 của số 415](https://www.ruanyifeng.com/blog/2026/10/weekly-issue-415.html#工具).

## 7. Tài nguyên, hình ảnh và trích đoạn

Năm tài nguyên được giới thiệu gồm CNEquity — kho dữ liệu chứng khoán Trung Quốc tự triển khai với nhiều tập dữ liệu và giao diện SQL/Python/MCP; dự án viết lại *Tiên Kiếm Kỳ Hiệp Truyện* bằng TypeScript với hỗ trợ AI; hướng dẫn cấu hình fcitx5 và Rime trên Linux; [APPLORE](https://applore.app/) với hơn 18.000 biểu tượng ứng dụng; và trang tra cứu lịch sử biến đổi chữ Hán.

Phần hình ảnh giới thiệu không gian bên trong chóp bảo vệ tải trọng tên lửa Falcon 9: phần khổng lồ của tên lửa là các tầng tạo lực đẩy, còn tải trọng thật sự nằm ở vùng đỉnh, được chóp bảo vệ trong lúc bay qua khí quyển.

Phần văn trích giới thiệu một góc nhìn ca ngợi Australia nhờ tài nguyên, năng lượng mặt trời, tài sản hộ gia đình và nhịp sống. Đây là **ý kiến cá nhân**: những khẳng định như tài sản trung vị gấp ba một quốc gia khác hay tài chính chính phủ dư lớn cần kiểm tra lại dữ liệu thống kê cùng kỳ và cách định nghĩa trước khi trích như một sự thật.

## 8. Những câu nói đáng nhớ

- Một cuộc trò chuyện tốt không yêu cầu mọi giây đều phải có lời nói. Đồ ăn và thức uống giúp con người có khoảng dừng tự nhiên, giảm áp lực liên tục phải tìm chủ đề.
- Lời nhắc hài hước về việc đừng ngược đãi AI là một ý kiến suy đoán, không phải bằng chứng rằng các hệ thống hiện tại có khả năng nuôi ý định trả thù.
- Một lời bình luận phê phán lập trình bằng ngôn ngữ tự nhiên: lặp đi lặp lại việc chỉnh lời nhắc đôi khi chậm và kém chính xác hơn sửa mã trực tiếp.
- Luận điểm “tư duy sẽ trở thành sở thích” đặt câu hỏi: khi máy làm thay phần lớn hoạt động trí óc, liệu con người còn thường xuyên luyện tư duy sâu?
- Nhận xét về cách thưởng thức những điều nhỏ trong cuộc sống nhắc rằng các trải nghiệm bình thường có thể trở nên rất đáng quý khi thời gian không còn nhiều.

Đây là phần **diễn giải ý**, không phải bản dịch nguyên văn toàn bộ các câu nói. Có thể xem liên kết gốc từng lời nhận xét ở [mục 言论](https://www.ruanyifeng.com/blog/2026/10/weekly-issue-415.html#言论).

## 9. Góc nhìn AI và bài học cho kỹ sư

**Một: phân biệt kết quả đúng về chức năng và kết quả đúng về ý định.** Cảnh 3D hiển thị thành công chưa chắc truyền tải cảm xúc của văn học. Một tác nhân tạo mã chạy được chưa chắc đáp ứng mong muốn của người dùng. Cần kiểm tra cả hành vi lẫn chất lượng trải nghiệm.

**Hai: hệ thống điều khiển quan trọng không kém mô hình.** DeskMind nhấn mạnh quyền được hỏi khi mơ hồ và việc kiểm tra trạng thái sau hành động. Những quy tắc này cần được mã hóa trong bộ điều khiển, không nên chỉ nằm trong lời nhắc.

**Ba: tối ưu theo độ khó nhiệm vụ.** Chạy mô hình 4B cho mọi bước của công việc có thể quá tốn; chạy mô hình 0,8B cho mọi bước có thể quá rủi ro. Bộ định tuyến chỉ có giá trị khi được kiểm chứng bằng độ trễ, tỷ lệ hoàn thành và chi phí thực.

**Bốn: mã rẻ không làm mất chi phí duy trì.** Một ứng dụng đồ họa 3D do AI tạo vẫn cần đo bộ nhớ và khung hình. Một trò chơi viết lại vẫn cần đối chiếu hành vi. Một dự án đa nền tảng vẫn chịu rủi ro của hệ sinh thái.

**Năm: không nên đánh giá lựa chọn công nghệ chỉ bằng sự thanh lịch.** Deno là ví dụ rõ về tác động của tương thích và quy mô hệ sinh thái. Khi cân nhắc nền tảng, cần xét cả phụ thuộc, nhân sự, nâng cấp và chi phí chuyển đổi.

## 10. Kết luận

Tuần san số 415 đánh dấu một xu hướng đáng theo dõi: AI đã đi xa hơn việc tạo từng đoạn nội dung. Nó có thể xây cả cảnh tương tác, hỗ trợ tái tạo phần mềm cũ và ra quyết định cho tác vụ trên máy tính. Tuy nhiên, khoảng cách giữa **tạo ra kết quả** và **chứng minh kết quả đúng** vẫn còn rất lớn.

Trong kỹ thuật phần mềm, điều đáng đầu tư không chỉ là chọn mô hình sinh mã mạnh hơn. Cần xây quy trình có mục tiêu rõ, quyền hạn hợp lý, điểm dừng khi mơ hồ, đo hiệu năng và kiểm chứng độc lập. Những điều đó giúp biến một bản thử nghiệm AI ấn tượng thành sản phẩm đáng tin.

---

**Liên kết tham khảo chủ yếu**

- [Tuần san công nghệ 415 — bản gốc](https://www.ruanyifeng.com/blog/2026/10/weekly-issue-415.html)
- [Dự án Lightbulb Computer](https://lightbulbcomputer.com/)
- [Deno](https://deno.com/)
- [DeskMind](https://deskmind.dev/)
- [SynthID Detector](https://synthid.com/)
- [APPLORE](https://applore.app/)
