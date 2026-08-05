# 科技爱好者周刊（第 396 期）：互联网通信的替代方案 (Bản tin công nghệ hàng tuần số 396: Giải pháp thay thế cho truyền thông internet)

Ghi lại nội dung công nghệ đáng chia sẻ hàng tuần, phát hành vào thứ Sáu.

Bản tin này [mã nguồn mở](https://github.com/ruanyf/weekly), hoan nghênh bạn [đóng góp](https://github.com/ruanyf/weekly/issues). Ngoài ra còn có dịch vụ [《Ai đang tuyển dụng》](https://github.com/ruanyf/weekly/issues/9815) đăng tải thông tin tuyển dụng lập trình viên. Hợp tác vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图 (Ảnh bìa)

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051414.webp)

"Trung tâm Tiểu Cầu Tân Xương" tại huyện Tân Xương, Chiết Giang, tích hợp khách sạn, trung tâm thương mại, nhà thi đấu, sân vận động và đường chạy bộ ngoài trời trong cùng một khối kiến trúc. ([via](https://www.archdaily.cn/cn/1036435/xin-chang-xiao-qiu-zhong-xin-line-plus-studio))

## 互联网通信的替代方案 (Giải pháp thay thế cho truyền thông internet)

Một buổi sáng thức dậy, bạn phát hiện toàn bộ kết nối internet đã bị cắt đứt thì phải làm sao?

Tôi đang nói đến tình huống mất mạng triệt để, hệ thống internet của toàn thành phố hoàn toàn tê liệt. Sự kiện này tuy có xác suất xảy ra rất nhỏ nhưng vẫn hoàn toàn khả thi, ví dụ khi gặp thiên tai nghiêm trọng hoặc chiến sự.

Giả sử mạng lưới viễn thông không thể khôi phục ngay lập tức, liệu có phương án thay thế nào không? Nói cách khác, **làm thế nào để chúng ta tự thiết lập một mạng lưới truyền thông độc lập**.

Mặc dù kiến trúc của internet là phi tập trung và việc dựng một mạng con nội bộ (subnet) không khó, nhưng để dựng một mạng diện rộng có thể bao phủ được nhiều người dùng nằm phân tán lại là thử thách lớn. Dù kết nối bằng router không dây, đường dây điện thoại, Bluetooth hay tự đi kéo cáp quang, độ phức tạp và chi phí đều rất cao.

Hôm nay, tôi xin chia sẻ một giải pháp tự thiết lập mạng lưới truyền thông đơn giản nhất mà tôi biết:

1. Phạm vi bao phủ đạt tới hàng chục kilomet, thậm chí xa hơn.
2. Không cần đi dây cáp, tự phát tín hiệu không dây.
3. Nguồn điện chỉ cần một viên pin sạc dự phòng, thậm chí là một viên pin tiểu.
4. Giá thành siêu rẻ, trọn bộ thiết bị chỉ khoảng vài trăm Nhân dân tệ (khoảng vài chục USD).

Nhược điểm duy nhất là băng thông rất nhỏ, không thể dùng để lướt web hay xem video, chỉ hỗ trợ truyền và nhận tin nhắn dạng văn bản (text messages).

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051412.webp)

Giải pháp này sử dụng công nghệ LoRa, viết tắt của cụm từ "Long Range" (Khoảng cách xa).

Giao thức LoRa được thiết kế chuyên biệt cho việc truyền thông khoảng cách xa. Chỉ cần một thiết bị nhỏ với mức tiêu thụ năng lượng cực thấp là có thể phát tín hiệu không dây ra môi trường xung quanh, tương tự như một trạm phát sóng radio cá nhân. Thuật toán mã hóa của nó đặc biệt chú trọng khả năng chống nhiễu, ngay cả khi tín hiệu cực kỳ yếu vẫn có thể giải mã chính xác giúp thu nhận tin tức từ khoảng cách rất xa.

Bản thân LoRa chỉ là một giao thức truyền tín hiệu không dây, người dùng cần có thiết bị thu phát tương ứng để mã hóa và giải mã thông tin. Dự án mã nguồn mở [Meshtastic](https://meshtastic.org) đã hiện thực hóa việc này bằng cách chuẩn hóa các giao tiếp phần mềm/phần cứng và cung cấp các thiết kế thiết bị cụ thể.

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051413.webp)

Vì vậy, mọi thứ trở nên rất đơn giản. **Chỉ cần mỗi người trang bị một thiết bị tương thích với Meshtastic là đã có thể cùng nhau tạo lập một mạng lưới truyền thông cơ bản**. Hệ thống sẽ tự động chuyển tiếp tiếp sức tin nhắn (mesh routing) qua lại giữa các nút mạng (nodes) của mọi người.

Trên các trang thương mại điện tử trong nước, thiết bị đầu cuối Meshtastic có giá dao động từ vài chục đến vài trăm Nhân dân tệ. Do là hệ thống nguồn mở nên bất kỳ nhà sản xuất nào cũng có thể chế tạo thiết bị tương thích. Trang chủ dự án cung cấp sẵn một [danh sách thiết bị](https://meshtastic.org/docs/hardware/devices/) để tham khảo. Dưới đây là hình ảnh thực tế của một số thiết bị đầu cuối:

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051005.webp)

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051007.webp)

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051006.webp)

Họ cũng cung cấp [phần mềm client](https://meshtastic.org/docs/software/) tương ứng cho nhiều nền tảng hệ điều hành khác nhau, dưới đây là giao diện ứng dụng trên điện thoại di động:

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051004.webp)

Như đã đề cập, thiết bị tiêu thụ điện năng cực kỳ ít, chỉ cần kết nối với pin sạc dự phòng là có thể hoạt động liên tục nhiều ngày đến vài tuần. Nếu lắp thêm tấm pin năng lượng mặt trời mini đi kèm, hệ thống có thể duy trì hoạt động vĩnh viễn.

Khoảng cách truyền tải giữa hai nút mạng trong phạm vi 5km hoạt động rất ổn định. Nếu ở khu vực thưa thớt nhà cao tầng có thể đạt 10km - 15km; còn ở các địa hình trống trải (như trên mặt nước) có thể đạt tới hàng chục kilomet hoặc xa hơn. Khi có nhiều nút mạng cùng tham gia, tin nhắn sẽ được truyền tiếp sức giúp phạm vi kết nối mở rộng ra rất nhiều.

Tóm lại, đây là giải pháp tự thiết lập mạng lưới truyền thông đơn giản, thực dụng và rẻ tiền nhất cho cá nhân. Nó không thể thay thế cho việc duyệt web thông thường, nhưng hoàn toàn có thể thay thế tính năng gửi nhận tin nhắn nhắn tin của internet khi xảy ra sự cố mất mạng diện rộng.

## 开源 AI 开发平台 MonkeyCode (Nền tảng phát triển AI nguồn mở MonkeyCode)

MonkeyCode là một dự án nguồn mở cho phép bạn tự cài đặt giao diện web sử dụng AI tương tự như giao diện của các hãng công nghệ lớn, hiện đã đạt gần 3.000 sao trên GitHub.

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051203.webp)

Nó cung cấp đầy đủ các tính năng lập trình bằng AI, người dùng chỉ cần mở trình duyệt và đưa ra yêu cầu bằng ngôn ngữ tự nhiên để AI thực thi mà không cần chuyển đổi công cụ hay cấu hình môi trường phức tạp.

![](https://cdn.beekka.com/blogimg/asset/202605/bg2026051101.webp)

Thông qua giao diện web của nó, bạn có thể **khởi tạo nhiều máy ảo** trên máy vật lý để chạy độc lập các dự án AI khác nhau, hệ thống cũng cung cấp sẵn nhiều loại ảnh đĩa (images) hệ điều hành cho máy ảo.

Nó cũng hỗ trợ cấu hình gửi thông báo qua DingTalk, Lark, WeChat doanh nghiệp, Webhook và liên kết với các kho lưu trữ mã nguồn trên GitHub, GitLab, Gitee, Gitea.

Ngoài việc tự host, dự án còn cung cấp [môi trường phát triển trên cloud miễn phí](https://monkeycode-ai.com/console) hỗ trợ điều khiển đa thiết bị trên cả điện thoại và máy tính. Hạn mức miễn phí hàng ngày trên đám mây là 20 triệu Token và hỗ trợ gọi nhiều loại mô hình lớn khác nhau.

## 逆向验证码 (Mã xác thực ngược - Reverse Captcha)

Mã xác thực Captcha thông thường được dùng để xác nhận lượt truy cập là con người thực sự chứ không phải bot tự động.

Hiện nay, thư viện tự động hóa trình duyệt nguồn mở Browser-use đã đề xuất khái niệm **Mã xác thực ngược**. Loại mã này được thiết kế để chặn con người thực và chỉ cho phép AI bot đi qua, thường được dùng để bảo vệ các cổng API chuyên dụng cho AI sử dụng.

Dưới đây là một câu đố toán học được dùng làm mã xác thực ngược:

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026042007.webp)

Giao diện hiển thị này khiến con người rất khó đọc hiểu để trả lời. Tuy nhiên, các mô hình ngôn ngữ lớn có thể dễ dàng loại bỏ các chữ in hoa nhiễu, ký tự ngẫu nhiên và khoảng trống để lọc ra câu hỏi gốc:

> "Hai đoàn tàu chạy ngược chiều nhau trên một đường ray thẳng dài d với vận tốc v1 và v2. Một chú chim xuất phát từ đoàn tàu này bay sang đoàn tàu kia với vận tốc vb, sau đó lập tức quay đầu bay trở lại, và lặp lại quá trình đó cho đến khi hai đoàn tàu gặp nhau. Hỏi chú chim đã bay được tổng cộng quãng đường bao nhiêu?"

Sau khi hiểu câu hỏi, mô hình lớn sẽ áp dụng công thức toán học để tính ra đáp án chính xác và vượt qua mã xác thực một cách dễ dàng.

## 科技动态 (Tin tức Công nghệ)

1. [Định nghĩa lại con trỏ chuột](https://deepmind.google/blog/ai-pointer/): Kể từ khi được phát minh, con trỏ chuột luôn đại diện cho vị trí thao tác hiện tại của người dùng. Google đề xuất một giải pháp mới thay đổi khái niệm này: Con trỏ chuột sẽ chỉ dùng để hiển thị trực quan các bước thao tác của AI để người dùng biết AI đang làm gì. Điều này đồng nghĩa với việc khi chạy mô hình AI, người dùng không thể di chuột trực tiếp mà phải điều khiển qua bàn phím hoặc giọng nói.

2. [Thu hồi dây đồng cũ](https://www.bloomberg.com/news/articles/2024-05-29/telcos-hunt-down-billions-worth-of-buried-copper-as-prices-soar): Kỷ nguyên năng lượng mới (xe điện, điện mặt trời, điện gió) đòi hỏi lượng dây đồng khổng lồ làm dây dẫn, khiến giá đồng tăng vọt và đưa việc thu hồi dây đồng cũ trở thành mảng kinh doanh béo bở. Các đường dây điện thoại, cáp mạng đồng cũ trước đây nay đều bị bỏ không do cáp quang và mạng di động thay thế. Nếu thu hồi được lượng đồng khổng lồ chôn dưới đất hoặc trong thiết bị cũ này sẽ mang lại giá trị kinh tế rất lớn do đồng tái chế có độ tinh khiết cao.

3. [Robot giao hàng chiếm dụng vỉa hè](https://blockclubchicago.org/2025/12/08/delivery-robots-take-over-chicago-sidewalks-sparking-debate-and-a-petition-to-hit-pause/): Thành phố Chicago (Mỹ) đang sử dụng lượng lớn robot giao hàng tự động trên đường phố và vấp phải sự phản đối của người dân. Do robot di chuyển trên vỉa hè dành cho người đi bộ nên gây cản trở giao thông của người dân. Người dân lo ngại không gian đi bộ yên tĩnh của họ sẽ bị ảnh hưởng khi có hàng trăm chiếc robot chạy qua lại hàng ngày.

## 文章 (Bài viết)

1、[Tại sao Trace ID nên dài 128-bit?](https://newsletter.signoz.io/p/why-should-a-trace-id-be-128-bits) (Tiếng Anh)

Khi cần tạo ID ngẫu nhiên để theo vết yêu cầu của người dùng, độ dài tối ưu là 128-bit nhằm tránh nguy cơ trùng lặp (collision) đối với các dịch vụ có lượng truy cập cực kỳ lớn.

2、[AI nên xuất ra định dạng HTML](https://simonwillison.net/2026/May/8/unreasonable-effectiveness-of-html/) (Tiếng Anh)

Thay vì xuất ra định dạng Markdown thông dụng hiện nay, bài viết lập luận AI nên xuất ra định dạng HTML trực tiếp để có thể chèn các biểu đồ SVG, thành phần tương tác hoặc menu điều hướng nội dung phong phú hơn.

3、[Mối lo ngại về Bun](https://wwj.dev/posts/i-am-worried-about-bun/) (Tiếng Anh)

Bun là một JS runtime tốc độ cao, được Anthropic mua lại vào tháng 12 năm 2025. Tác giả bày tỏ mối lo ngại rằng Bun trong tương lai có thể bị lạm dụng chèn quá nhiều mã do AI tự động tạo ra làm giảm chất lượng tổng thể của dự án.

4、[Bảo vệ khóa SSH private key bằng sinh trắc học](https://ahelwer.ca/post/2026-05-08-builtin-u2f/) (Tiếng Anh)

Hướng dẫn cấu hình khóa SSH private key tận dụng cơ chế bảo mật phần cứng của máy tính, yêu cầu xác thực vân tay (Touch ID) hoặc khuôn mặt (Face ID) mỗi khi gọi khóa nhằm tránh nguy cơ bị mã độc lấy cắp.

5、[Tôi mở cổng Port 22 trong vòng 54 ngày](https://arman-bd.hashnode.dev/i-left-port-22-open-on-the-internet-for-54-days-here-s-who-showed-up) (Tiếng Anh)

Cổng 22 mặc định cho kết nối SSH luôn là mục tiêu quét lỗi của hacker. Tác giả đã dựng một hệ thống bẫy (honeypot) mở cổng 22 để ghi nhận các hành vi dò mật khẩu và các dòng lệnh mà hacker thực thi sau khi xâm nhập.

6、[Khác biệt giữa Ibuprofen và Tylenol](https://asteriskmag.com/issues/14/the-mystery-in-the-medicine-cabinet) (Tiếng Anh)

So sánh cơ chế hoạt động của hai loại thuốc hạ sốt giảm đau phổ biến là Ibuprofen và Tylenol (Paracetamol). Tác giả cho rằng nếu sử dụng đúng liều lượng chỉ định, Tylenol mang lại hiệu quả tốt và ít tác dụng phụ hơn Ibuprofen trong phần lớn các trường hợp thông thường.

## 工具 (Công cụ)

1、[RethinkDNS](https://github.com/serverless-dns/serverless-dns)

Dịch vụ máy chủ DNS nguồn mở hỗ trợ triển khai trên các môi trường không máy chủ Serverless (như Cloudflare Workers).

2、[Pinta](https://www.pinta-project.com/)

Phần mềm chỉnh sửa hình ảnh nguồn mở gọn nhẹ thay thế PhotoShop trên các hệ điều hành desktop.

3、[GitForms](https://github.com/Luigigreco/gitforms)

Ứng dụng nguồn mở giúp lưu trữ trực tiếp dữ liệu từ các form đăng ký trang web vào mục Issue của GitHub, giúp bạn xây dựng trang thu thập ý kiến người dùng mà không cần xây dựng server backend riêng.

4、[gecit](https://github.com/boratanrikulu/gecit)

Công cụ dòng lệnh giúp tùy biến và thay đổi trường SNI (domain name) của các gói tin mạng gửi đi từ máy cục bộ.

5、[MapPoster Online](https://github.com/ianho7/maptoposter-online)

Ứng dụng web nguồn mở giúp chuyển đổi bản đồ đường phố của các thành phố thành các bức tranh poster nghệ thuật độc đáo. (Đóng góp từ [@ianho7](https://github.com/ruanyf/weekly/issues/9880))

6、[boss-agent-cli](https://github.com/can4hou6joeng4/boss-agent-cli)

Công cụ dòng lệnh hỗ trợ tìm kiếm và xem tin tuyển dụng trên các trang tuyển dụng lớn tại Trung Quốc, hỗ trợ tích hợp với AI Agent. (Đóng góp từ [@can4hou6joeng4](https://github.com/ruanyf/weekly/issues/9908))

7、[TITAN PLANET](https://github.com/ezet-galaxy/-ezetgalaxy-titan)

Một dự án sáng tạo cho phép viết backend bằng JavaScript nhưng biên dịch ra tệp tin chạy binary bằng Rust giúp tăng tốc độ thực thi đáng kể.

8、[qjp](https://github.com/plainas/qjp)

Công cụ dòng lệnh hỗ trợ hiển thị và duyệt nhanh cấu trúc các tệp tin dữ liệu định dạng JSON theo dạng cây thư mục tương tác.

9、[tinypdf](https://github.com/Lulzx/tinypdf)

Thư viện JavaScript siêu nhẹ chỉ 3KB dùng để khởi tạo nhanh tệp tin PDF.

10、[edge-tts](https://github.com/rany2/edge-tts)

Thư viện Python hỗ trợ gọi dịch vụ chuyển đổi văn bản thành giọng nói (TTS) trực tuyến của Microsoft.

## AI 相关 (AI Liên quan)

1、[FeedFuse](https://github.com/BryanHoo/FeedFuse)

Trình đọc tin RSS Web nguồn mở tích hợp tính năng AI giúp tự động lấy toàn bộ nội dung bài viết, tóm tắt ý chính và dịch thuật tự động. (Đóng góp từ [@BryanHoo](https://github.com/ruanyf/weekly/issues/9916))

2、[IBus LLM Pinyin Input](https://github.com/volsifly/ibus_llm_pinyin_input)

Bộ gõ tiếng Trung Pinyin chạy trên IBus sử dụng mô hình ngôn ngữ lớn để gợi ý từ khóa thông minh theo ngữ cảnh người dùng gõ. (Đóng góp từ [@volsifly](https://github.com/ruanyf/weekly/issues/9911))

3、[kooky](https://github.com/iAmCorey/kooky)

Ứng dụng terminal cực giản trên macOS được tối ưu riêng cho lập trình bằng AI, hỗ trợ khởi động nhanh các agent như Claude Code/Codex và chia màn hình theo dõi trạng thái. (Đóng góp từ [@iAmCorey](https://github.com/ruanyf/weekly/issues/9921))

## 资源 (Tài nguyên)

1、[taken.](https://sinceyouarrived.world/taken)

Trang web giúp kiểm tra xem yêu cầu HTTP gửi đi từ trình duyệt của bạn đang làm lộ bao nhiêu thông tin cá nhân.

2、[DataCenter.fm](https://datacenter.fm)

Trình phát âm thanh nền mô phỏng tiếng ồn hoạt động của các phòng máy chủ (data center).

3、[MathNet](https://mathnet.mit.edu/)

Trang web do Viện Công nghệ Massachusetts (MIT) vận hành, lưu trữ dữ liệu của hơn 30.000 câu đố toán học học thuật.

4、[Các quy luật của trải nghiệm người dùng](https://lawsofux.com/)

Tổng hợp các định luật thiết kế UX kinh điển như Định luật Miller: Một người bình thường chỉ có thể ghi nhớ đồng thời từ 5 đến 9 mục thông tin cùng lúc.

## 图片 (Hình ảnh)

1. [Ô nhiễm do vệ tinh](https://apod.nasa.gov/apod/ap260427.html): Số lượng vệ tinh nhân tạo tầm thấp tăng nhanh làm ảnh hưởng nghiêm trọng đến việc chụp ảnh thiên văn do chúng phản xạ ánh sáng mặt trời tạo thành các đường vạch đè lên ảnh phơi sáng (hình minh họa). Thiên văn học đề xuất nên chuyển các kính viễn vọng không gian sang lắp đặt tại mặt sau của Mặt Trăng.

## 文摘 (Văn trích)

1、[Máy pha cà phê vũ trụ](https://mceglowski.substack.com/p/bitter-lessons-from-the-isspresso)

Để宇航 viên trên Trạm vũ trụ quốc tế (ISS) uống được cà phê nóng, NASA đã đặt hàng một công ty Ý thiết kế máy pha cà phê hoạt động trong môi trường không trọng lực. Thiết bị phải đảm bảo các tiêu chuẩn khắt khe: Không làm ảnh hưởng hệ thống điện, không nhiễu sóng vô tuyến, không rò rỉ nước sôi, không có nguy cơ hỏa hoạn, không chói mắt, không gây điện giật, không quá nóng, không ồn và không sinh khí độc hại. Trọng lượng máy tăng từ 3.5kg dưới mặt đất lên tới 20kg trong vũ trụ với chi phí nghiên cứu lên tới hàng triệu USD để tạo ra những túi cà phê uống qua vòi bóp.

2、[Đừng tin câu nói "Ai không dùng AI sẽ tụt lại phía sau"](https://migrainebrain.bearblog.dev/people-who-dont-use-ai-will-be-left-behind/)

Tôi không đồng ý với quan điểm này. Thực tế có thể ngược lại: Những người phụ thuộc hoàn toàn vào AI trong tương lai sẽ mất đi năng lực tư duy độc lập, mất kỹ năng viết lách, mất kỹ năng tra cứu thông tin cơ bản và không phân biệt được thật giả. Họ sẽ quên mất cách học hỏi — thứ vốn dĩ rất tốt đẹp của con người. Nếu nhận thấy AI đang làm tốt hơn mình, việc bạn cần làm là rèn luyện để bản thân trở nên xuất sắc hơn ở những mảng mà AI không thể chạm tới.

## 言论 (Phát ngôn)

1、

> "Thị trường toàn cầu tiêu thụ 1,5 tỷ điện thoại thông minh mỗi năm, hầu hết chỉ được dùng trong vòng chưa đầy hai năm rồi bị vứt bỏ hoặc bỏ xó. Đây là sự lãng phí tài nguyên tính toán khổng lồ trong khi cấu hình của chúng hoàn toàn có thể tận dụng phục vụ mạng tính toán chung."
> 
> -- 《Tái tận dụng điện thoại thông minh cũ》

2、

> "Ngôn ngữ lập trình của tương lai sẽ không phải là ngôn ngữ dễ học nhất với con người, mà là ngôn ngữ dễ học nhất đối với AI."
> 
> -- @RealRichomie

3、

> "Sức sáng tạo có bị suy giảm theo tuổi tác không? Nghiên cứu chỉ ra khả năng liên kết sáng tạo (associative innovation) có xu hướng tăng lên theo tuổi tác, trong khi khả năng sáng tạo mang tính đột phá (disruptive innovation) sẽ giảm dần."
> 
> -- 《Tiến bộ khoa học đôi khi phải trả giá bằng các buổi tang lễ》

4、

> "Mô hình ngôn ngữ lớn là một dạng nén dữ liệu có mất mát (lossy compression) từ dữ liệu huấn luyện, mà bản thân dữ liệu huấn luyện lại là một mẫu lấy từ thế giới thực tế."
> 
> "Khi AI tạo ra kết quả, nó đang làm nhiệm vụ phình to dữ liệu đã nén để điền vào các thông tin bị thiếu hụt nhằm tạo ra các bài viết, hình ảnh hoặc video hoàn chỉnh."
> 
> -- 《Công cụ phình to dữ liệu》

## 往年回顾 (Nhìn lại các năm trước)

[Người phát minh ra thuật toán mạng thần kinh nhân tạo](https://www.ruanyifeng.com/blog/2025/05/weekly-issue-349.html)（#349）

[Mấu chốt của AI chính là kho ngữ liệu (corpus)](https://www.ruanyifeng.com/blog/2024/05/weekly-issue-299.html)（#299）

[Nhà doanh nghiệp phần mềm thành công nhất](https://www.ruanyifeng.com/blog/2023/04/weekly-issue-249.html)（#249）

[Vấn đề chứng chỉ bảo mật HTTPS của Nga](https://www.ruanyifeng.com/blog/2022/03/weekly-issue-199.html)（#199）

(Hết)
