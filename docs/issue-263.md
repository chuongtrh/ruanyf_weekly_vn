# Bản tin chia sẻ công nghệ (Số 263): Phần mềm nguồn mở kiếm tiền bằng cách nào?

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3222) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072012.webp)

Thủ đô Lima của Peru là một thành phố vô cùng độc đáo khi được xây dựng ngay trên mép các vách đá dựng đứng hướng thẳng ra Thái Bình Dương. Do địa hình đặc thù này, cư dân thành phố mỗi khi muốn đi dạo dưới bãi biển đều phải đi bộ xuống dốc men theo sườn vách đá. (Nguồn: [Instagram](https://www.instagram.com/p/CufbbVXPtA8/))

## 开源软件如何赚钱？

Hầu như ai làm việc trong ngành công nghệ cũng đều biết một sự thật: kiếm tiền từ các dự án phần mềm mã nguồn mở là vô cùng khó khăn, đặc biệt là đối với các dự án phân phối dưới giấy phép GPL.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071602.webp)

Giấy phép GPL quy định bắt buộc nhà phát triển phải cung cấp toàn bộ mã nguồn đi kèm cho người dùng, đồng thời trao cho người dùng quyền tự do chỉnh sửa và tái phân phối mã nguồn đó.

Điều này đồng nghĩa với việc **bất kỳ bên thứ ba nào cũng có quyền sao chép và phân phối miễn phí phần mềm của bạn**, khiến mô hình kinh doanh bán bản quyền phần mềm truyền thống hoàn toàn bất khả thi.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071706.webp)

**Nếu không thể bán bản quyền phần mềm, liệu chúng ta có thể chuyển sang bán các dịch vụ hỗ trợ kỹ thuật đi kèm?** Cụ thể là cung cấp dịch vụ hỗ trợ triển khai, tư vấn kỹ thuật hoặc viết mã tùy chỉnh theo yêu cầu của khách hàng?

Trong quá khứ, mô hình này được chứng minh là khả thi thông qua câu chuyện thành công kinh điển của tập đoàn Red Hat. Bằng việc cung cấp các gói dịch vụ hỗ trợ kỹ thuật và tư vấn cho hệ điều hành Linux cấp doanh nghiệp, Red Hat đã phát triển mạnh mẽ, niêm yết thành công lên sàn chứng khoán vào năm 1999 và sau đó được tập đoàn IBM mua lại vào năm 2019 với mức giá khổng lồ lên tới 34 tỷ USD.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071603.webp)

Tuy nhiên, câu chuyện thành công lãng mạn đó đã chính thức khép lại vào tháng trước. Một quyết định bất ngờ của Red Hat đã khiến giới công nghệ bừng tỉnh nhận ra: **mô hình kinh doanh dựa vào dịch vụ hỗ trợ kỹ thuật nguồn mở (Customer Support Model) đã không còn đất diễn**.

Dưới đây là chi tiết sự việc vừa diễn ra:

Sản phẩm thương mại cốt lõi mang lại doanh thu chính cho Red Hat là hệ điều hành Red Hat Enterprise Linux (viết tắt là RHEL). Hãng thu tiền dựa trên các gói dịch vụ hỗ trợ kỹ thuật và bảo trì hệ thống cho phiên bản này.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071707.webp)

Theo các điều khoản ràng buộc của giấy phép GPL, Red Hat bắt buộc phải công bố công khai mã nguồn của RHEL. Chính kẽ hở này đã tạo điều kiện cho **rất nhiều phiên bản sao chép (clone) miễn phí ra đời trên thị trường**. Các doanh nghiệp lớn muốn tiết kiệm chi phí dịch vụ chỉ cần cài đặt các phiên bản clone này để chạy hệ thống của mình mà không cần chi trả đồng nào cho Red Hat.

Trong quá khứ, phiên bản clone nổi tiếng nhất của Red Hat chính là CentOS. Thậm chí số lượng máy chủ chạy hệ điều hành CentOS trong thực tế còn vượt xa số lượng chạy phiên bản trả phí của Red Hat.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071708.webp)

Sau khi sáp nhập vào IBM, ban lãnh đạo hãng nhận thấy các phiên bản clone miễn phí đang gây ảnh hưởng nghiêm trọng tới biên lợi nhuận của họ. Red Hat đã tiến hành thâu tóm CentOS và chính thức khai tử hệ điều hành này vào hai năm trước, chuyển đổi nó thành một phiên bản thử nghiệm mang tên CentOS Stream – biến cộng đồng người dùng thành nơi chạy thử và phát hiện lỗi cho hãng.

Quyết định này vấp phải làn sóng phản đối dữ dội từ cộng đồng. Do mã nguồn của RHEL vẫn được công khai, các phiên bản clone miễn phí khác nhanh chóng được cộng đồng phát triển để thay thế CentOS, tiêu biểu nhất là Alma Linux và Rocky Linux:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071710.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071711.webp)

Và sự kiện gây chấn động xảy ra vào tháng trước khi Red Hat [bất ngờ ra thông báo](https://www.redhat.com/en/blog/furthering-evolution-centos-stream): **Hãng sẽ chấm dứt việc công bố công khai mã nguồn của RHEL ra cộng đồng, toàn bộ mã nguồn sẽ chỉ được cung cấp riêng tư cho các khách hàng có trả phí dịch vụ**.

Tuyên bố này giống như một quả bom dội vào cộng đồng mã nguồn mở thế giới, bởi chưa từng có tiền lệ doanh nghiệp nào hành động như vậy trước đây.

Tuy nhiên sau khi phân tích kỹ các điều khoản pháp lý, giới luật sư nhận định hành động này của Red Hat hoàn toàn hợp pháp và không vi phạm giấy phép GPL. Giấy phép GPL chỉ yêu cầu nhà phát triển cung cấp mã nguồn cho những đối tượng trực tiếp sử dụng sản phẩm phần mềm (ở đây là các khách hàng trả phí của Red Hat). Do đó, hãng hoàn toàn có quyền từ chối công bố mã nguồn ra ngoài cộng đồng.

Điểm mấu chốt nằm ở chỗ khi đăng ký dịch vụ trả phí của Red Hat, khách hàng bắt buộc phải ký vào một bản Thỏa thuận người dùng (User Agreement), trong đó quy định rõ: **Nếu khách hàng tự ý tái phân phối mã nguồn được cung cấp ra ngoài, Red Hat có quyền đơn phương chấm dứt hợp đồng dịch vụ ngay lập tức**. Điều khoản này đồng nghĩa với việc các nhà phát triển Alma Linux hay Rocky Linux sẽ không thể tiếp cận mã nguồn RHEL được nữa, qua đó gián tiếp khai tử các hệ điều hành clone miễn phí.

Quyết định tinh quái này chứng minh Red Hat đã tốn rất nhiều công sức nghiên cứu pháp lý để triệt tiêu các phiên bản clone mà không vi phạm giấy phép GPL.

Tác động dài hạn của quyết định này lên uy tín thương hiệu của Red Hat vẫn cần thời gian trả lời, nhưng nó cho thấy một thực tế: **mức doanh thu mang lại từ mô hình dịch vụ hỗ trợ kỹ thuật truyền thống là không đủ hấp dẫn, buộc Red Hat phải tìm cách triệt tiêu các bản miễn phí để ép người dùng chuyển sang mua gói dịch vụ trả phí**.

Red Hat – vốn được coi là ngọn hải đăng duy nhất chứng minh sự thành công của mô hình dịch vụ hỗ trợ kỹ thuật nguồn mở – nay đã tự mình chấm dứt mô hình đó. Từ nay về sau, cơ hội để một startup nguồn mở có thể lớn mạnh chỉ nhờ bán dịch vụ hỗ trợ kỹ thuật hầu như sẽ không còn tồn tại.

Giới phân tích công nghệ quốc tế đã đúc kết **4 lý do chính khiến mô hình dịch vụ hỗ trợ kỹ thuật nguồn mở thất bại**:

1. **Biên lợi nhuận vô cùng thấp**: Khách hàng doanh nghiệp thường sẵn sàng chi trả số tiền lớn để mua bản quyền phần mềm độc quyền nhưng lại cực kỳ keo kiệt khi chi trả cho dịch vụ tư vấn, hỗ trợ kỹ thuật.
2. **Khó mở rộng quy mô kinh doanh (Scalability)**: Một doanh nghiệp có thể tự do cài đặt phần mềm nguồn mở của bạn trên hàng ngàn máy chủ nhưng họ chỉ cần mua đúng một gói dịch vụ hỗ trợ kỹ thuật tối thiểu cho một kỹ sư của họ là đủ.
3. **Mâu thuẫn với sự phát triển chất lượng phần mềm**: Phần mềm nguồn mở của bạn càng dễ cài đặt, hoạt động càng ổn định và ít lỗi thì khách hàng lại càng không có lý do để mua gói hỗ trợ kỹ thuật của bạn. Nói cách khác, việc bạn tối ưu hóa phần mềm vô tình lại triệt tiêu nguồn thu dịch vụ hỗ trợ của chính mình.
4. **Khó mang lại doanh thu trong giai đoạn đầu**: Đối với các startup, việc tìm kiếm được 100 khách hàng sử dụng sản phẩm ban đầu đã là thử thách lớn, trong số đó tỷ lệ khách hàng sẵn sàng bỏ tiền mua dịch vụ hỗ trợ kỹ thuật là vô cùng thấp, thậm chí bằng không.

Do đó, mô hình kiếm tiền bền vững của các dự án nguồn mở trong tương lai chắc chắn không phải là dịch vụ hỗ trợ kỹ thuật. Tuy nhiên chủ đề này đã khá dài, tôi xin phép được hẹn gặp lại các bạn để thảo luận sâu hơn về các mô hình kiếm tiền thay thế ở số tuần sau.

## 科技动态

1、[Mẫu màn hình hiển thị danh sách công việc hàng ngày độc đáo để bàn](https://peppe.rs/posts/plain_text_journaling/)

Một lập trình viên nước ngoài đã tận dụng màn hình hiển thị của máy tính bảng cũ để tự chế tạo bảng lịch và danh sách công việc (todo list) đặt bàn làm việc:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062003.webp)

Thiết bị được đặt ngay ngắn trên bàn làm việc hàng ngày để nhắc nhở chủ nhân các đầu việc cần xử lý và theo dõi tiến độ công việc trực quan.

Phần trên của màn hình hiển thị lịch của các tháng gần nhất, phía dưới hiển thị danh sách các đầu việc cần làm trong tuần và thanh trạng thái tiến độ hoàn thành:

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062004.webp)

Thiết bị tự chế có chi phí linh kiện rất rẻ và giao diện tối giản, là phương án thay thế hoàn hảo cho các cuốn lịch để bàn bằng giấy truyền thống.

2、[Ấn Độ khánh thành tòa nhà văn phòng có diện tích mặt sàn lớn nhất thế giới](https://edition.cnn.com/style/india-largest-office-building-surat-diamond-bourse/index.html)

Tòa nhà văn phòng lớn nhất thế giới vừa được khánh thành tại thành phố Surat, nằm cách Mumbai khoảng 250 km về phía Bắc:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072001.webp)

Thành phố Surat được biết đến là trung tâm gia công và cắt gọt kim cương lớn nhất thế giới, xử lý khoảng 90% sản lượng kim cương toàn cầu. Công trình mới khánh thành này chính là Sàn giao dịch kim cương của thành phố.

Tòa nhà sở hữu tổng diện tích mặt sàn lên tới 660.000 mét vuông với thiết kế bao gồm 9 khối nhà hình chữ nhật được kết nối với nhau thông qua một hành lang trung tâm. Công trình cao 15 tầng này có sức chứa lên tới 65.000 nhân viên làm việc cùng lúc:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072002.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072003.webp)

Kỷ lục tòa nhà văn phòng lớn nhất thế giới trước đó thuộc về tòa nhà Lầu Năm Góc của Bộ Quốc phòng Mỹ với diện tích 610.000 mét vuông. Danh hiệu tòa nhà có thể tích xây dựng lớn nhất thế giới hiện vẫn thuộc về Trung tâm Toàn cầu Tân thế kỷ tại Thành Đô với diện tích sàn lên tới 1,76 triệu mét vuông.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072004.webp)

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072005.webp)

3、[Trang web thu âm các điều khoản sử dụng dài dòng của mạng xã hội làm nhạc ru ngủ](https://petapixel.com/2023/07/13/legal-lullabies-puts-you-to-sleep-by-reading-social-media-terms-of-use/)

Bản Thỏa thuận điều khoản sử dụng của các mạng xã hội lớn luôn tràn ngập các thuật ngữ pháp lý phức tạp, dài dòng và cực kỳ khô khan khiến người đọc rất nhanh buồn ngủ nếu cố gắng đọc chi tiết.

Tận dụng đặc điểm này, một lập trình viên đã nảy ra ý tưởng thuê các diễn viên lồng tiếng chuyên nghiệp đọc lại toàn bộ các điều khoản dịch vụ này với tông giọng trầm ấm để làm liệu pháp âm thanh ru ngủ cho người dùng:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072008.webp)

Nếu bạn gặp chứng mất ngủ, hãy truy cập trang web [zzzuckerberg.com](https://www.zzzuckerberg.com/) để lắng nghe các đoạn ghi âm này.

Bản thu âm điều khoản sử dụng của Instagram có độ dài lên tới 51 phút, trong khi bản của TikTok kéo dài khoảng 38 phút.

4、[Nền tảng âm nhạc AI Mubert công bố kho nhạc số đạt mốc 100 triệu bài hát](https://www.digitalmusicnews.com/2023/07/12/ai-generated-music-platform-mubert-says-catalog-now-tops-100-million-songs/)

Khác biệt với các nền tảng phân phối nhạc truyền thống vốn lưu trữ các tác phẩm do con người sáng tác, một dịch vụ âm nhạc trực tuyến mới đã ra mắt chuyên lưu trữ và phân phối các bản nhạc do AI tự động biên soạn:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072009.webp)

Nền tảng mang tên [Mubert](https://mubert.com/) thông báo kho nhạc của họ hiện đã vượt mốc 100 triệu bản nhạc, tương đương với quy mô thư viện bài hát của dịch vụ Spotify lớn nhất thế giới, cho phép người dùng nghe nhạc không giới hạn.

Toàn bộ nhạc do AI sinh ra trên nền tảng đều được miễn phí bản quyền tác giả và cho phép người dùng tải về ứng dụng trực tiếp vào các dự án thương mại của mình. Website cũng cung cấp công cụ cho phép người dùng tự tạo ra các giai điệu theo sở thích cá nhân để đóng góp vào thư viện chung.

## Bài viết

1\. [GitHub chính thức ra mắt tính năng đăng nhập không mật khẩu bằng Passkey](https://github.blog/2023-07-12-introducing-passwordless-authentication-on-github-com/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071401.webp)

Nền tảng lưu trữ mã nguồn lớn nhất thế giới GitHub công bố chính thức hỗ trợ phương thức xác thực bảo mật không mật khẩu Passkey từ tháng này. Bài viết hướng dẫn chi tiết các bước thiết lập kích hoạt tính năng này trong phần quản lý tài khoản cá nhân.

2\. [Phỏng vấn chuyên sâu tác giả cuốn sách lịch sử bán chạy “Chiến tranh chip”](https://www.noahpinion.blog/p/interview-chris-miller-historian)（Tiếng Anh）

Bài phỏng vấn thú vị với sử gia Chris Miller – tác giả cuốn sách nghiên cứu nổi tiếng *“Chip War”*, chia sẻ các góc nhìn chuyên sâu về chiến lược phát triển vi mạch bán dẫn của chính phủ Mỹ và tình hình cạnh tranh công nghệ vi mạch giữa hai cường quốc Mỹ và Trung Quốc.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071202.webp)

3\. [Giới thiệu hàm toàn cục sao chép sâu structuredClone mới trong Javascript](https://developer.mozilla.org/en-US/docs/Web/API/structuredClone)（Tiếng Anh）

Trước đây khi cần thực hiện sao chép sâu (deep clone) cấu trúc dữ liệu đối tượng trong JS, lập trình viên thường phải tự viết đệ quy hoặc sử dụng các thư viện bổ trợ bên ngoài. Bài viết giới thiệu hàm toàn cục `structuredClone()` hiện đã được tích hợp mặc định trên các trình duyệt hiện đại giúp thực hiện sao chép sâu dữ liệu nhanh chóng và an toàn.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052814.webp)

4\. [Giải mã bài toán hình học bánh xe lăn quanh một vòng tròn lớn](https://plus.maths.org/content/circles-rolling-circles)（Tiếng Anh）

Một câu hỏi hình học lý thuyết thú vị: *"Giả sử có hai vòng tròn với bán kính lần lượt là r và 4r (hình minh họa). Cho vòng tròn nhỏ lăn men theo chu vi phía ngoài của vòng tròn lớn đúng một vòng khép kín. Hỏi vòng tròn nhỏ thực tế đã tự xoay quanh tâm của chính nó bao nhiêu vòng?"* (Gợi ý: Đáp án chính xác không phải là 4 vòng).

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052903.webp)

5\. [Tài liệu hướng dẫn nhập môn sử dụng Media Query trong thiết kế CSS](https://engineering.kablamo.com.au/posts/2023/media-queries-and-responsive-design/)（Tiếng Anh）

Bài viết hướng dẫn lập trình viên Front-end cách thức viết mã ứng dụng bộ lọc Media Query trong CSS để xây dựng giao diện hiển thị co giãn tương thích (Responsive Web Design) mượt mà trên nhiều kích thước màn hình thiết bị khác nhau.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023052904.webp)

6\. [Tài liệu tóm tắt cơ bản về kiến trúc lưu trữ nội bộ của hệ thống Git](https://sites.google.com/a/chromium.org/dev/developers/fast-intro-to-git-internals)（Tiếng Anh）

Tài liệu ngắn gọn do kỹ sư thuộc đội ngũ phát triển trình duyệt Chromium biên soạn, giải thích trực quan cách thức Git quản lý dữ liệu dưới dạng sơ đồ cây đối tượng (blob, tree, commit) giúp lập trình viên hiểu sâu hơn cơ chế hoạt động của các lệnh Git.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061803.webp)

7\. [Bài viết khoa học phổ thông giải thích khái niệm cấu trúc dữ liệu băm](https://samwho.dev/hashing/)（Tiếng Anh）

Một bài viết hướng dẫn trực quan sinh động sử dụng các hình ảnh đồ họa tương tác để giải thích bản chất của hàm băm (Hash Function), các tình huống ứng dụng trong lưu trữ mật khẩu và cách hệ thống xử lý khi xảy ra hiện tượng đụng độ mã băm (hash collision).

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023062103.webp)

8\. [Tìm hiểu định nghĩa và cơ chế hoạt động của Socket trong mạng máy tính](https://mp.weixin.qq.com/s/Ebvjy132eRDOmcIL5cmxJw)（Tiếng Trung）

Khái niệm Socket luôn là câu hỏi phỏng vấn kinh điển trong các kỳ tuyển dụng lập trình viên backend. Bài viết giải thích cặn kẽ cơ chế thiết lập kết nối Socket ở tầng hệ điều hành và cách thức truyền nhận gói tin trong mạng máy tính. (Đóng góp của [@xxxsalted](https://github.com/ruanyf/weekly/issues/3274))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071902.webp)

## 工具

1、[hiSHtory: Công cụ tìm kiếm lịch sử câu lệnh terminal nâng cao](https://github.com/ddworken/hishtory)

Một tiện ích mạnh mẽ hỗ trợ lập trình viên nhanh chóng tìm kiếm các dòng lệnh terminal đã chạy trong lịch sử hệ thống, cung cấp thuật toán tìm kiếm thông minh thay thế hoàn hảo cho tính năng tìm kiếm bằng phím tắt `Ctrl + R` mặc định của Shell.

2、[talk: Ứng dụng phòng chat nhóm WebRTC đa nền tảng nguồn mở](https://github.com/vasanthv/talk)

Mã nguồn mở xây dựng ứng dụng trò chuyện nhóm trực tuyến hoạt động trên trình duyệt dựa trên giao thức truyền thông ngang hàng WebRTC, hỗ trợ gọi điện thoại truyền hình (video call), gọi thoại và chat văn bản bảo mật không lưu dữ liệu trên server.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122401.webp)

3、[TinyVG: Định dạng ảnh vector nhị phân tối giản thay thế cho SVG](https://tinyvg.tech/)

Đề xuất định dạng lưu trữ hình ảnh đồ họa vector dưới dạng file nhị phân tối ưu, giúp cắt giảm đáng kể dung lượng tệp tin so với định dạng văn bản XML của tệp SVG truyền thống để tăng tốc độ tải trang web.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023032101.webp)

4、[Gitstars: Công cụ quản lý và phân loại các dự án đã gắn sao trên GitHub](https://github.com/cfour-hi/gitstars)

Ứng dụng web nguồn mở hỗ trợ lập trình viên đồng bộ, gắn tag phân loại và lọc tìm kiếm nhanh các dự án mã nguồn mở mình từng ấn nút Star (thích) trên GitHub để tiện tra cứu sau này. (Đóng góp của [@cfour-hi](https://github.com/ruanyf/weekly/issues/3286))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072007.webp)

5、[迅排设计 (poster-design): Công cụ thiết kế poster đồ họa trực tuyến nguồn mở](https://github.com/palxiao/poster-design)

Một ứng dụng web cung cấp giao diện kéo thả thiết kế các mẫu poster quảng cáo, ảnh bìa trực quan tương tự như công cụ Canva, được phát triển hoàn toàn bằng mã nguồn mở. (Đóng góp của [@palxiao](https://github.com/ruanyf/weekly/issues/3284))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072006.webp)

6、[Spring Startup Analyzer: Tiện ích phân tích hiệu năng khởi động của Spring](https://github.com/linyimin0812/spring-startup-analyzer)

Công cụ hỗ trợ các nhà phát triển Java phân tích chi tiết quá trình khởi tạo các Bean hệ thống trong dự án Spring Boot, tự động đo đạc thời gian nạp để xuất ra báo cáo đồ họa tương tác giúp tối ưu hóa thời gian startup của ứng dụng. (Đóng góp của [@linyimin0812](https://github.com/ruanyf/weekly/issues/3280))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071904.webp)

7、[WebAV: Thư viện xử lý và biên tập âm thanh video trực tiếp bằng Javascript](https://github.com/hughfenghen/WebAV)

Dự án thử nghiệm tận dụng API WebCodecs mới được tích hợp trên trình duyệt Chrome để cho phép lập trình viên viết mã JS trực tiếp xử lý phân tích và ghép nối các luồng dữ liệu âm thanh hình ảnh ngay trên trình duyệt mà không cần cài đặt phần mềm ngoài. (Đóng góp của [@hughfenghen](https://github.com/ruanyf/weekly/issues/3282))

8、[kafka-console-ui: Giao diện đồ họa quản trị Kafka siêu nhẹ](https://github.com/xxd763795151/kafka-console-ui)

Ứng dụng web quản trị và giám sát trực quan các cụm máy chủ truyền tin Apache Kafka, được thiết kế với dung lượng siêu nhẹ và dễ dàng cài đặt. (Đóng góp của [@xxd763795151](https://github.com/ruanyf/weekly/issues/3272))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071901.webp)

9、[killport: Tiện ích dòng lệnh viết bằng Rust giúp đóng nhanh các cổng port bị chiếm](https://github.com/jkfran/killport)

Một công cụ dòng lệnh gọn nhẹ viết bằng Rust, giúp lập trình viên nhanh chóng tắt toàn bộ các tiến trình đang chạy ngầm chiếm dụng các cổng mạng chỉ định (ví dụ port 8080) để giải phóng tài nguyên.

10、[Sniffnet: Ứng dụng giám sát và trực quan hóa lưu lượng mạng đa nền tảng](https://github.com/GyulyVGC/sniffnet)

Phần mềm máy tính hỗ trợ người dùng theo dõi thời gian thực toàn bộ lưu lượng dữ liệu mạng ra vào thiết bị, tự động phân tích phân loại địa chỉ kết nối và biểu diễn dưới dạng biểu đồ động trực quan.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051903.webp)

## 资源

1、[Triviance: Thư viện câu hỏi trắc nghiệm khổng lồ sinh bởi ChatGPT](https://triviance.com/)

Trang web tổng hợp kho dữ liệu trắc nghiệm kiến thức tổng hợp với hơn 1 triệu câu hỏi bốn đáp án do AI ChatGPT tự động biên soạn, được phân chia khoa học theo nhiều chuyên mục chủ đề khác nhau để người dùng thử sức.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023042502.webp)

2、[FastGPT: Công cụ tìm kiếm thông tin kết hợp chatbot AI miễn phí](https://labs.kagi.com/fastgpt)

Dịch vụ chatbot AI do công cụ tìm kiếm mới nổi Kagi phát triển, hỗ trợ người dùng đặt câu hỏi và tra cứu thông tin tổng hợp từ Internet hoàn toàn miễn phí, có hỗ trợ phản hồi tốt bằng tiếng Việt.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071601.webp)

3、[ToolAI: Danh mục tổng hợp các dịch vụ và ứng dụng AI trên thế giới](https://www.toolai.io/)

Trang web thư viện chuyên tổng hợp và phân loại liên kết của hơn 5.000 ứng dụng và dịch vụ trí tuệ nhân tạo đang hoạt động trên toàn thế giới. (Đóng góp của [@littledot2020](https://github.com/ruanyf/weekly/issues/3276))

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071903.webp)

4\. [Python for Data Analysis: Giáo trình hướng dẫn phân tích dữ liệu bằng Python](https://wesmckinney.com/book/)

Bản in cập nhật thứ ba của cuốn sách giáo khoa tiếng Anh kinh điển hướng dẫn lập trình viên sử dụng ngôn ngữ Python và các thư viện pandas, numpy để thực hiện phân tích thống kê dữ liệu lớn, hỗ trợ đọc trực tuyến miễn phí.

## 图片

1、**Bộ ảnh nghệ thuật chụp mặt dưới của các tảng băng trôi khổng lồ**

Chúng ta đều biết câu nói quen thuộc: phần tảng băng trôi nổi trên mặt nước chỉ chiếm chưa đầy 20% thể tích thực của nó.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012102.webp)

Một nữ nhiếp ảnh gia lặn biển chuyên nghiệp người Đức đã lặn sâu dưới làn nước băng giá tại vùng biển Greenland để ghi lại những hình ảnh vô cùng ấn tượng về phần chìm khổng lồ của các tảng băng trôi dưới lòng đại dương:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012103.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012104.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012105.webp)

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012107.webp)

2、**Hóa thạch bông hoa hổ phách có niên đại 30 triệu năm tuổi**

Vào năm 1872, tại khu vực rừng thông cổ ven biển Baltic thuộc Bắc Âu, các nhà khảo cổ đã phát hiện một khối hổ phách tự nhiên có tuổi thọ ước tính hơn 30 triệu năm:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012108.webp)

Điểm kỳ diệu của khối hổ phách này là nó lưu giữ nguyên vẹn một bông hoa đang kỳ nở rộ:

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023012109.webp)

Đây là hóa thạch bông hoa nguyên vẹn lớn nhất từng được phát hiện từ trước đến nay với chiều dài cánh hoa đạt 28 mm, giúp các nhà thực vật học nghiên cứu chi tiết về cấu trúc của các loài hoa cổ đại.

## ✍️ Bài đọc thêm

### Giai đoạn trưởng thành nhanh và chậm trong xã hội hiện đại

Chúng ta đang sống trong một xã hội có xu hướng phát triển khá nghịch lý: trẻ em thì cư xử và có suy nghĩ già dặn như người trưởng thành, trong khi người lớn lại bộc lộ nhiều nét tính cách trẻ con, thiếu chín chắn.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072010.webp)

Trẻ em ngày nay nhờ sự phổ cập của Internet và các thiết bị di động thông minh đã được tiếp cận thế giới của người lớn từ rất sớm.

Ngay từ khi còn nhỏ, các em đã có thể tự do xem các video bạo lực, tin tức chiến tranh hay các hình ảnh nhạy cảm trên mạng xã hội mà không có sự kiểm soát của cha mẹ, dẫn đến quá trình người lớn hóa diễn ra rất nhanh.

Tuy nhiên khi thực sự bước vào tuổi trưởng thành pháp lý, thế hệ trẻ lại gặp nhiều khó khăn trong việc tự lập về mặt tài chính và thiếu các cơ hội để gánh vác trách nhiệm thực tế trong đời sống xã hội.

Hệ quả là nền văn hóa chung của xã hội xuất hiện xu hướng trẻ con hóa: nhiều người trưởng thành sợ phải đưa ra các cam kết dài hạn (trong công việc cũng như hôn nhân), thiếu tự tin vào bản thân và luôn cảm thấy bấp bênh trước cuộc sống. Cách thức ứng xử và đối mặt với các vấn đề xã hội của họ vẫn dừng lại ở mức của một thiếu niên mới lớn.

### Câu chuyện hài hước xoay quanh điều khoản sử dụng của phần mềm JSLint

Douglas Crockford – người có công lớn trong việc chuẩn hóa và phổ biến định dạng dữ liệu JSON – đã chia sẻ một câu chuyện pháp lý hài hước trong sự nghiệp của mình:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072011.webp)

Khi phát hành công cụ kiểm tra lỗi code JSLint, ông đã thêm vào giấy phép sử dụng của phần mềm một điều khoản mang tính đạo đức: *“Phần mềm này nên được sử dụng cho các mục đích hướng thiện, không được dùng cho việc ác”*.

Một thời gian sau, ông nhận được thư chính thức từ đội ngũ luật sư của tập đoàn công nghệ IBM.

Các luật sư cho biết IBM rất muốn đưa phần mềm JSLint vào bộ công cụ phát triển phần mềm của hãng. Tuy nhiên điều khoản yêu cầu "không dùng cho việc ác" của giấy phép khiến họ gặp vướng mắc lớn về mặt pháp lý. Họ có thể bảo đảm các kỹ sư IBM không dùng phần mềm làm việc xấu, nhưng hãng không có cách nào kiểm soát và bảo đảm hành vi của hàng triệu khách hàng mua phần mềm của họ sau này. Do đó, các luật sư đề xuất Crockford cung cấp cho IBM một giấy phép đặc biệt khác.

Crockford đã phản hồi qua thư: *"Đồng ý. Tôi chính thức cấp quyền cho tập đoàn IBM, các đối tác và khách hàng của hãng được phép sử dụng phần mềm JSLint cho các mục đích làm việc ác"*.

Đại diện luật sư IBM sau đó đã phản hồi: *"Cảm ơn ông rất nhiều, Crockford!"* và vướng mắc pháp lý đã được tháo gỡ thành công.

## Lịch sử tuần này

- 2022年（第 216 期）：[Triết lý thiết kế: Sự lên ngôi và chiến thắng của chủ nghĩa tối giản trong thiết kế công nghiệp](http://www.ruanyifeng.com/blog/2022/07/weekly-issue-216.html)
- 2021年（第 166 期）：[Phương pháp học tập: Việc học tập qua video liệu có mang lại hiệu quả vượt trội hơn so với việc đọc sách truyền thống](http://www.ruanyifeng.com/blog/2021/07/weekly-issue-166.html)
- 2020年（第 116 期）：[Xã hội học: Tại sao tương lai phát triển của thế giới lại tiềm ẩn nhiều nguy cơ bất ổn như thùng thuốc súng](http://www.ruanyifeng.com/blog/2020/07/weekly-issue-116.html)
- 2019年（第 66 期）：[Kinh doanh số: Tại sao hành trình khởi nghiệp công nghệ không phải là một trò chơi có tổng bằng không](http://www.ruanyifeng.com/blog/2019/07/weekly-issue-66.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge organization smooth and efficient.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
