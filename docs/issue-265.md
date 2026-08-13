# Bản tin chia sẻ công nghệ (Số 265): Sau WiFi sẽ là LiFi

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3324) trong khu vực luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080303.webp)

Vào ngày 2 tháng 8 vừa qua, tại thành phố Noshiro, tỉnh Akita, Nhật Bản đã diễn ra lễ hội diễu hành đèn lồng khổng lồ thường niên mang tên “Thành phố không ngủ trên bầu trời”. Những chiếc đèn lồng giấy cao tầng được thắp sáng rực rỡ di chuyển dọc các tuyến phố chính tạo nên khung cảnh huyền ảo dễ bị lầm tưởng là tranh vẽ do AI sinh ra. (Nguồn: [Noshirotanabata](https://noshirotanabata.com/))

## WiFi 的后面是 LiFi

Vào tháng 6 vừa qua, Hiệp hội Kỹ sư Điện và Điện tử (IEEE) đã chính thức thông qua **tiêu chuẩn 802.11bb**.

Đây là bộ tiêu chuẩn kỹ thuật dành riêng cho công nghệ truyền thông bằng ánh sáng khả kiến – phương thức kết nối Internet thông qua ánh sáng, viết tắt là **LiFi** (Light Fidelity). Ngay từ tên gọi, chúng ta đã thấy mối liên hệ mật thiết giữa LiFi và WiFi, trong đó chữ L đại diện cho *Light* (Ánh sáng).

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023073105.webp)

Mặc dù thông tin về sự kiện này chưa được chia sẻ rộng rãi tại thị trường nội địa, đây thực sự là một bước tiến công nghệ rất thú vị đáng để chúng ta cùng tìm hiểu.

Trước hết, chúng ta cần làm rõ bản chất công nghệ của LiFi là gì?

Như đã biết, hệ thống mạng không dây WiFi hiện nay sử dụng sóng vô tuyến (sóng radio) để truyền tải thông tin bằng cách mã hóa dữ liệu mạng lồng vào các bước sóng vô tuyến.

Sóng vô tuyến thực chất là một dạng sóng điện từ, và ánh sáng khả kiến nhìn thấy được bằng mắt thường cũng là một dạng sóng điện từ. **Do đó về mặt lý thuyết, chúng ta hoàn toàn có thể điều chế tín hiệu mạng lồng vào các bước sóng ánh sáng để truyền tải dữ liệu kết nối.**

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023073106.webp)

Phương thức truyền tải dữ liệu bằng bước sóng ánh sáng mang lại một số ưu điểm vượt trội so với sóng vô tuyến:

**1. Băng thông truyền tải cực kỳ khổng lồ**

Mạng WiFi hiện nay hoạt động chủ yếu trên các băng tần tần số 2.4 GHz, 5 GHz hoặc mới nhất là 6 GHz. Trong khi đó, tần số của ánh sáng khả kiến dao động trong khoảng từ 430 THz đến 750 THz – tức là cao gấp hàng trăm ngàn lần so với tần số của sóng WiFi.

Trong nguyên lý truyền thông, tần số sóng càng cao thì lượng thông tin có thể mã hóa truyền tải đi trong một đơn vị thời gian càng lớn, mang lại băng thông kết nối siêu lớn. Tuy nhiên, đi kèm với tần số siêu cao là khả năng đâm xuyên vật cản (như tường nhà) cực kỳ kém.

**2. Hoàn toàn không gây nhiễu sóng vô tuyến**

Do hoạt động trên dải tần ánh sáng độc lập, LiFi hoàn toàn không gây nhiễu cho các thiết bị thu phát vô tuyến khác. Đặc tính này giúp LiFi cực kỳ phù hợp để triển khai tại các khu vực nhạy cảm với sóng vô tuyến như khoang hành khách máy bay hay phòng phẫu thuật y tế. Ánh sáng khả kiến cũng hoàn toàn không phát sinh bức xạ điện từ có hại cho cơ thể người.

**3. Không chịu giới hạn tài nguyên tần số**

Nhà sản xuất thiết bị LiFi không cần phải làm các thủ tục xin cấp phép sử dụng băng tần tần số vô tuyến phức tạp từ chính phủ do dải tần ánh sáng là tự do và vô cùng rộng lớn.

**4. Chi phí sản xuất thiết bị rẻ**

Công nghệ điều chế và giải điều chế tín hiệu quang học không quá phức tạp, giúp các nhà máy có thể nhanh chóng sản xuất hàng loạt thiết bị phần cứng đầu cuối với mức giá thành phải chăng.

Vào năm 2020, hãng điện thoại OPPO đã nộp đơn đăng ký bằng sáng chế cho dòng điện thoại thông minh được tích hợp bộ thu phát tín hiệu mạng LiFi:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023073107.webp)

Trên máy tính, người dùng cũng có thể sử dụng các bộ thu phát tín hiệu LiFi nhỏ gọn cắm qua cổng USB:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023073108.webp)

Tuy nhiên, LiFi cũng sở hữu những nhược điểm vật lý rất khó khắc phục:

Rào cản lớn nhất là để duy trì kết nối mạng LiFi, bạn bắt buộc phải có một bóng đèn phát sáng đặt trong phòng. Điều này đồng nghĩa với việc hễ bạn tắt đèn đi ngủ thì kết nối mạng cũng sẽ lập tức biến mất:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023073109.webp)

Đồng thời, mắt đọc cảm biến của thiết bị thu nhận phải được đặt hướng thẳng về phía bóng đèn phát sáng trong phạm vi khoảng cách tương đối gần (các thực nghiệm ghi nhận hiệu quả tốt nhất trong vòng 3 mét trở lại).

Bên cạnh đó là bài toán truyền dữ liệu chiều ngược lại (Upload): thiết bị di động hay máy tính của bạn cũng bắt buộc phải được trang bị một bóng đèn phát tín hiệu ánh sáng hướng ngược lại về phía máy thu của căn phòng để gửi dữ liệu lên mây.

Do đó, LiFi được định vị không phải để thay thế hoàn toàn cho WiFi mà đóng vai trò như một giải pháp bổ trợ đắc lực trong các tình huống đặc thù đòi hỏi băng thông truyền tải cực lớn ở khoảng cách gần.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080307.webp)

Gần đây, tôi có đọc báo cáo về việc các nhà sản xuất đang thử nghiệm **thay thế dây dẫn kim loại truyền thống bằng công nghệ truyền dẫn quang học trực tiếp bên trong khe cắm PCIe trên bo mạch chủ**. Đây chính là một môi trường ứng dụng hoàn hảo cho LiFi, giúp đáp ứng băng thông truyền tải dữ liệu siêu cao giữa card đồ họa và CPU mà không cần các sợi cáp nối phức tạp trong thùng máy.

Tựu trung, ý tưởng về việc lướt web thông qua ánh sáng phát ra từ một bóng đèn trần vẫn là một trải nghiệm công nghệ rất thú vị mang đậm màu sắc khoa học viễn tưởng. Với việc LiFi chính thức được chuẩn hóa quốc tế, hy vọng chúng ta sẽ sớm thấy các sản phẩm thương mại ứng dụng công nghệ này xuất hiện trên thị trường.

## 科技动态

1、[Biến đổi khí hậu đang làm thay đổi màu sắc của đại dương sang sắc xanh lá cây](https://www.vice.com/en/article/3aka3b/youre-not-imagining-it-the-ocean-has-changed-color-over-20-years-study-determines)

Màu xanh lam đặc trưng của các đại dương lớn trên Trái Đất có nguy cơ chuyển dần sang màu xanh lá cây trong tương lai.

Trung tâm Nghiên cứu Đại dương Vương quốc Anh đã công bố báo cáo phân tích số liệu ảnh vệ tinh thu thập liên tục suốt 20 năm qua, khẳng định màu sắc bề mặt của các đại dương đang có sự chuyển dịch rõ rệt sang tông màu xanh lá cây do tác động của biến đổi khí hậu:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023071303.webp)

Nguyên nhân chính do nhiệt độ nước biển tăng cao kết hợp lượng khí thải carbon dioxide trong không khí tăng mạnh đã kích thích sự sinh trưởng bùng nổ của các loài tảo và thực vật nổi trên mặt biển.

Các loài thực vật nổi này sở hữu lượng chất diệp lục lớn trong tế bào, có đặc tính hấp thụ ánh sáng xanh lam và phản xạ lại ánh sáng xanh lá cây. Tại các vùng biển ghi nhận sự phát triển quá mức của thực vật nổi, nước biển sẽ chuyển sang màu xanh lá cây đục.

2、[Diễn viên lồng tiếng lên tiếng cảnh báo nguy cơ bị AI cướp mất cơ hội nghề nghiệp](https://www.axios.com/2023/07/24/ai-voice-actors-victoria-atkin-assassins-creed)

Nữ diễn viên lồng tiếng nổi tiếng Victoria Atkin – người từng đảm nhận lồng tiếng cho nhân vật nữ chính trong tựa game đình đám *Assassin's Creed Syndicate* của hãng Ubisoft năm 2015:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080101.webp)

Mới đây cô vô cùng ngạc nhiên khi phát hiện một nhóm người hâm mộ đã tự ý trích xuất toàn bộ các tệp âm thanh giọng nói của cô từ game cũ để nạp làm dữ liệu huấn luyện cho mô hình AI, từ đó tự động sinh ra một gói lồng tiếng hội thoại hoàn chỉnh cho nhân vật trong tựa game khác là *The Elder Scrolls V: Skyrim* để chia sẻ miễn phí trên mạng:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080102.webp)

Nữ diễn viên chia sẻ mối lo ngại lớn nhất của cô không chỉ dừng lại ở vấn đề vi phạm bản quyền giọng nói cá nhân, mà là xu hướng các hãng game sẽ chuyển sang sử dụng hoàn toàn giọng nói nhân tạo của AI để cắt giảm chi phí thuê diễn viên lồng tiếng, đẩy toàn bộ nhân sự trong ngành vào nguy cơ thất nghiệp. Hiệp hội Diễn viên Lồng tiếng Mỹ hiện đang tích cực thương thảo với các nghiệp đoàn sản xuất game để đưa ra các điều khoản giới hạn việc lạm dụng AI giọng nói để bảo vệ quyền lợi cho người lao động.

3、[Mẫu súng ngắn thông minh tích hợp cảm biến sinh trắc học đầu tiên mở bán tại Mỹ](https://www.wsj.com/amp/articles/the-first-smart-gun-is-finally-coming-to-market-will-anyone-buy-it-67314e0)

Thương hiệu vũ khí Biofire của Mỹ vừa công bố mở bán dòng súng ngắn thông minh đầu tiên trên thế giới tích hợp các chốt khóa an toàn sinh trắc học, ngăn không cho người lạ sử dụng súng:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072911.webp)

Phần báng súng được trang bị cảm biến quét dấu vân tay, đồng thời mặt sau của thân súng tích hợp hệ thống camera quét khuôn mặt hồng ngoại. Súng chỉ mở khóa chốt cò khi nhận diện chính xác chủ sở hữu hợp pháp. Thiết bị vận hành bằng pin sạc tích hợp bên trong thân súng:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072912.webp)

Sản phẩm được định giá bán lẻ ở mức 1.499 USD (trong khi các dòng súng ngắn thông thường cùng phân khúc chỉ có giá dao động từ 400 đến 800 USD). Nhà sản xuất kỳ vọng công nghệ này giúp ngăn ngừa các tai nạn cướp cò thương tâm do trẻ em nghịch súng hoặc ngăn kẻ xấu sử dụng súng cướp được để gây án.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023072913.webp)

4、[Quy định bảo mật nghiêm ngặt của Apple đối với bộ công cụ phát triển Vision Pro](https://arstechnica.com/gadgets/2023/07/here-are-the-rules-for-apples-new-vision-pro-dev-kit-your-family-cant-see-it/)

Apple đã bắt đầu gửi các bộ thiết bị kính thực tế ảo Vision Pro phiên bản thử nghiệm (Developer Kit) cho các đối tác đăng ký để phát triển trước các ứng dụng phần mềm đón đầu ngày mở bán.

Tuy nhiên, thỏa thuận bảo mật bắt buộc đi kèm thiết bị được đánh giá là cực kỳ khắt khe:

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023073001.webp)

Các nhà phát triển nhận máy phải cam kết:

* Chỉ được phép mở hộp và sử dụng thiết bị trong một **phòng làm việc có khóa kín và không có cửa sổ kính**.
* Tuyệt đối không cho phép bạn bè, người thân hay đồng nghiệp ngoài dự án được nhìn thấy hoặc chạm vào thiết bị.
* Khi không sử dụng, thiết bị bắt buộc phải được cất gọn gàng vào trong hộp bảo vệ và khóa lại.
* Không được phép mang thiết bị ra khỏi địa chỉ đăng ký (ví dụ mang về nhà riêng) khi chưa có sự đồng ý bằng văn bản từ Apple.
* Nếu nhà phát triển có kế hoạch đi công tác hoặc nghỉ mát rời khỏi văn phòng làm việc quá 10 ngày, họ bắt buộc phải thông báo cho Apple để có phương án bảo quản thiết bị an toàn.

Việc Apple kiểm soát quá chặt chẽ hình ảnh thực tế của Vision Pro và việc chưa có bất kỳ hình ảnh nào của các lãnh đạo cấp cao Apple trực tiếp đeo chiếc kính này khiến giới truyền thông hoài nghi rằng thiết bị thực tế vẫn còn một số lỗi phần cứng chưa tối ưu tốt như kỳ vọng quảng cáo, buộc hãng phải giữ bí mật tối đa để tránh gây thất vọng cho thị trường trước ngày mở bán chính thức.

## Bài viết

1\. [Trung Quốc phóng thành công tên lửa vận hành bằng nhiên liệu oxy lỏng - metan đầu tiên trên thế giới](https://news.sina.com.cn/c/2023-08-01/doc-imzesefx8781568.shtml)（Tiếng Trung）

Vào ngày 12 tháng 7 vừa qua, doanh nghiệp hàng không vũ trụ tư nhân LandSpace của Trung Quốc đã thực hiện phóng thành công tên lửa đẩy Chu Tước 2 vào quỹ đạo trái đất. Đây được ghi nhận là dòng tên lửa vận hành bằng động cơ nhiên liệu hỗn hợp Oxy lỏng - Metan đầu tiên trên thế giới thử nghiệm thành công, mở ra hướng đi mới giúp cắt giảm chi phí phóng nhờ nhiên liệu metan dễ sản xuất và ít để lại muội than bám động cơ so với dầu hỏa truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080201.webp)

2\. [Khám phá các công cụ dòng lệnh hữu ích ẩn trong thư viện tiêu chuẩn của Python](https://til.simonwillison.net/python/stdlib-cli-tools)（Tiếng Anh）

Bài viết giới thiệu một số công cụ dòng lệnh (CLI tools) vô cùng hữu ích được tích hợp sẵn bên trong thư viện mặc định của ngôn ngữ Python mà người dùng có thể gọi chạy trực tiếp từ terminal (ví dụ chạy nhanh một local web server, nén file zip hay định dạng lại chuỗi JSON) mà không cần viết thêm mã code.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023063003.webp)

3\. [Hướng dẫn cài đặt giao diện máy tính Linux chạy trực tiếp trên điện thoại Android](https://mrs-t.medium.com/transform-your-android-device-into-a-linux-desktop-110a3d084ac6)（Tiếng Anh）

Bài viết hướng dẫn chi tiết cách thức tận dụng ứng dụng terminal Termux trên hệ điều hành Android để cài đặt phân vùng và khởi chạy môi trường máy tính Linux hoàn chỉnh (như Ubuntu với giao diện XFCE) trực tiếp trên màn hình điện thoại di động.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080205.webp)

4\. [Giải pháp cấu hình cơ sở dữ liệu SQLite hỗ trợ kết nối truy vấn qua mạng](https://blog.turso.tech/sqlite-based-databases-on-the-postgres-protocol-yes-we-can-358e61171d65)（Tiếng Anh）

SQLite vốn được thiết kế là một cơ sở dữ liệu dạng file cục bộ không hỗ trợ kết nối mạng. Tác giả bài viết chia sẻ giải pháp tinh chỉnh mã nguồn và đóng gói để biến SQLite thành một cơ sở dữ liệu phân tán có thể tiếp nhận các yêu cầu truy vấn dữ liệu từ xa thông qua giao thức mạng TCP (dự án LibSQL/Turso).

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070406.webp)

5\. [Chia sẻ các phương pháp thiết lập và bảo vệ danh tính ẩn danh trên Internet](https://k3tan.com/starting-a-new-digital-identity)（Tiếng Anh）

Tác giả chia sẻ câu chuyện thực tế và tổng hợp các công cụ kỹ thuật (như sử dụng hệ điều hành Tails, trình duyệt bảo mật, hòm thư ẩn danh và thanh toán tiền điện tử) giúp người dùng bảo vệ quyền riêng tư và che giấu hoàn toàn danh tính số khi hoạt động trên mạng Internet.

![](https://cdn.beekka.com/blogimg/asset/202307/bg2023070407.webp)

6\. [Tài liệu hướng dẫn lập trình hợp ngữ Assembly cấu trúc Arm64 dành cho người mới](https://www.deusinmachina.net/p/the-basics-of-arm64-assembly)（Tiếng Anh）

Bài viết giới thiệu các kiến thức nền tảng về tập lệnh hợp ngữ Assembly dành riêng cho cấu trúc chip xử lý ARM64, hướng dẫn chi tiết cách thức quản lý thanh ghi và viết chương trình đầu tay đơn giản từ con số không.

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040701.webp)

7\. [Giới thiệu so sánh trực quan giữa 3 công cụ điều phối container Docker và Kubernetes](https://mp.weixin.qq.com/s/F9g-r4yBYDZ1Q9z6uq5feQ)（Tiếng Trung）

Bài viết sử dụng ngôi kể thứ nhất vô cùng hài hước để giới thiệu vai trò, nhiệm vụ và các kịch bản phối hợp vận hành thực tế của 3 công cụ quản lý container phổ biến hiện nay là Docker Compose, Docker Swarm và cụm Kubernetes (K8s). (Đóng góp của [@xxxsalted](https://github.com/ruanyf/weekly/issues/3325))

8\. [Hướng dẫn chi tiết phương pháp giải mã thủ công mã QR bằng giấy và bút chì](https://blog.qartis.com/decoding-small-qr-codes-by-hand/)（Tiếng Anh）

Một thực nghiệm toán học thú vị: tác giả hướng dẫn từng bước cách thức đọc và giải mã thông tin chứa bên trong một mã QR cỡ nhỏ chỉ bằng cách quan sát các ô vuông đen trắng trên giấy và tính toán hệ nhị phân thủ công bằng bút chì mà không cần dùng camera điện thoại.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060302.webp)

## 工具

1、[Vanilla: Bộ mã nguồn diễn đàn thảo luận viết bằng PHP chuyên nghiệp](https://open.vanillaforums.com/)

Một giải pháp xây dựng trang diễn đàn thảo luận (Forum) mã nguồn mở viết bằng ngôn ngữ PHP, sở hữu giao diện hiển thị hiện đại, tốc độ tải trang nhanh và cung cấp hệ thống phân quyền thành viên chặt chẽ.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111401.webp)

2、[GitHub Business Card: Trang web hỗ trợ tạo danh thiếp cá nhân từ tài khoản GitHub](https://github-business-card.vercel.app/)

Tiện ích web vui vẻ giúp người dùng tự động thu thập các thông số đóng góp (contributions), ngôn ngữ lập trình sử dụng từ trang cá nhân GitHub để thiết kế thành một tấm danh thiếp cá nhân dạng pixel retro độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111402.webp)

3、[Equal UI: Bộ sưu tập component giao diện Vue 3 dựa trên Tailwind CSS](https://equal-ui.github.io/Equal/)

Bộ thư viện component Front-end tinh tế dành riêng cho framework Vue 3, hỗ trợ lập trình viên xây dựng nhanh giao diện web đáp ứng nhờ việc cấu trúc CSS tối ưu bằng Tailwind CSS.

4、[emaction: Linh kiện Web Component tạo thanh Emoji tương tác cho bài viết](https://github.com/emaction/emaction.frontend)

Một đoạn mã Web Component gọn nhẹ hỗ trợ lập trình viên tích hợp nhanh thanh thả biểu cảm cảm xúc (Emoji reactions) dưới chân bài viết blog tương tự như giao diện tương tác của GitHub. (Đóng góp của [@tiezhudotwang](https://github.com/ruanyf/weekly/issues/3309))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080210.webp)

5、[ChatHub: Extension Chrome hỗ trợ chat đồng thời với nhiều mô hình AI](https://github.com/chathub-dev/chathub)

Tiện ích mở rộng trình duyệt cho phép người dùng chia đôi hoặc chia bốn màn hình để trò chuyện và so sánh kết quả phản hồi đồng thời từ nhiều chatbot AI khác nhau (như ChatGPT, Bing Chat, Google Bard, Claude) trên cùng một giao diện. (Đóng góp của [@wong2](https://github.com/ruanyf/weekly/issues/3310))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080211.webp)

6、[Whistle Client: Ứng dụng debug và phân tích gói tin mạng đa nền tảng](https://github.com/avwo/whistle-client)

Phần mềm máy tính phát triển dựa trên Electron kết hợp công cụ dòng lệnh Whistle, cung cấp giao diện đồ họa trực quan giúp các nhà phát triển dễ dàng cấu hình proxy, bắt gói tin (packet capture) và phân tích các luồng dữ liệu mạng. (Đóng góp của [@ATQQ](https://github.com/ruanyf/weekly/issues/3312))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080212.webp)

7、[Erin: Extension Chrome quản lý tab trình duyệt theo dạng thanh Dock](https://erin-homepage.vercel.app/)

Tiện ích mở rộng giúp thay đổi giao diện quản lý các thẻ tab đang mở của Chrome thành một thanh biểu tượng động bố trí sát viền dưới màn hình tương tự như thanh Dock ứng dụng của hệ điều hành macOS. (Đóng góp của [@Developer27149](https://github.com/ruanyf/weekly/issues/3318))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080304.webp)

8、[AI Code Translator: Dịch vụ web hỗ trợ chuyển đổi ngôn ngữ lập trình bằng AI](https://aicodeconvert.com/)

Ứng dụng web tích hợp trí tuệ nhân tạo hỗ trợ lập trình viên chuyển đổi các đoạn mã nguồn từ một ngôn ngữ lập trình này sang ngôn ngữ khác (ví dụ chuyển từ Python sang Go), hoặc mô tả yêu cầu tính năng bằng văn bản để AI tự động sinh code. (Đóng góp của [@JustAIGitHub](https://github.com/ruanyf/weekly/issues/3322))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080305.webp)

9、[Slashbase: Công cụ quản trị cơ sở dữ liệu Postgres và MongoDB trên nền web](https://github.com/slashbaseide/slashbase)

Ứng dụng quản trị cơ sở dữ liệu chạy trực tiếp trên trình duyệt viết bằng Go, hỗ trợ kết nối trực quan hóa dữ liệu và thực hiện các câu lệnh truy vấn nhanh dành riêng cho hai hệ CSDL PostgreSQL và MongoDB.

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110902.webp)

10、[YouPlot: Tiện ích vẽ biểu đồ dữ liệu bằng ký tự ASCII trong terminal](https://github.com/red-data-tools/YouPlot)

Một công cụ dòng lệnh độc đáo viết bằng Ruby, cho phép lập trình viên vẽ nhanh các dạng biểu đồ cột, biểu đồ đường trực quan ngay trong màn hình terminal bằng các ký tự văn bản ASCII.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011302.webp)

11、[PrettyPolly: Ứng dụng AI hỗ trợ luyện tập giao tiếp nói ngoại ngữ](https://www.prettypolly.app/app)

Ứng dụng học tập ngoại ngữ ứng dụng trí tuệ nhân tạo: cung cấp môi trường luyện nói tương tác trực tiếp bằng giọng nói với AI hỗ trợ tới 26 ngôn ngữ khác nhau (bao gồm cả tiếng Anh, tiếng Trung, tiếng Nhật). Đây là giải pháp công nghệ có khả năng thay thế dần các mô hình gia sư dạy nói ngoại ngữ truyền thống nhờ chi phí cực rẻ.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080310.webp)

## 资源

1\. [JavaScript Frameworks History: Sách tóm tắt lịch sử phát triển của các JS Framework](https://programmingsoup.com/history-of-javascript-frameworks)

Cuốn sách điện tử nhỏ viết bằng tiếng Anh giới thiệu chặng đường phát triển của các framework lập trình giao diện Front-end từ thời kỳ sơ khai của Prototype.js, Dojo, Mootools cho đến kỷ nguyên hiện tại của các kiến trúc Micro-frontend hay Island Architecture.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051204.webp)

2、[Makefile Tutorial: Tài liệu hướng dẫn tự học lập trình file cấu hình Makefile](https://makefiletutorial.com/)

Trang web tổng hợp tài liệu hướng dẫn viết file Makefile từ cơ bản đến nâng cao dành cho các lập trình viên C/C++ muốn làm chủ quy trình biên dịch dự án tự động.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051601.webp)

3\. [NixOS & Flakes Guide: Sách hướng dẫn tự học NixOS dành cho người mới](https://nixos-and-flakes.thiscute.world/zh/)

Cuốn sách hướng dẫn kỹ thuật viết bằng tiếng Trung giúp người dùng nhanh chóng làm quen với cơ chế quản lý cấu hình hệ thống khai báo của hệ điều hành NixOS và cách ứng dụng tính năng Flakes để quản lý phiên bản phần mềm. (Đóng góp của [@ryan4yin](https://github.com/ruanyf/weekly/issues/3315))

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080213.webp)

4\. [SwiftUI 100 Days: Khóa học 100 video bài giảng tự học lập trình SwiftUI](https://www.hackingwithswift.com/100/swiftui)

Chuỗi video bài giảng trực tuyến chất lượng cao kéo dài trong 100 ngày hướng dẫn lập trình viên tự học phát triển ứng dụng di động iOS sử dụng framework SwiftUI mới nhất của Apple.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061702.webp)

## 图片

1、**Tháp Sway Tower: Tòa nhà bằng bê tông không có cốt thép cao nhất thế giới**

Vào năm 1879, một vị thẩm phán người Anh sau khi nghỉ hưu từ Ấn Độ trở về quê nhà tại miền nam nước Anh đã tuyên bố nhận được chỉ thị của thần linh yêu cầu ông phải xây dựng một tòa tháp cao tại khu đất của mình.

Vì lý do đó, ông đã chi tiền thuê nhân công xây dựng một tòa tháp có kiểu dáng khá kỳ lạ:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050511.webp)

Đến năm 1886, tòa tháp chính thức hoàn thành với chiều cao 66 mét. Điều đáng kinh ngạc là toàn bộ cấu trúc tháp được đổ hoàn toàn bằng bê tông cốt liệu thô mà không sử dụng bất kỳ thanh sắt hay thép chịu lực nào bên trong. Đến nay, công trình vẫn đứng vững và giữ kỷ lục là tòa nhà bằng bê tông không cốt thép cao nhất thế giới:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050512.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050513.webp)

Do công trình không có công năng sử dụng thực tế nào ngoài việc làm cảnh quan, sau khi vị thẩm phán qua đời vào năm 1906, tháp dần bị bỏ hoang và biến thành nơi nuôi bồ câu. Đến cuối thế kỷ trước, một cá nhân đã mua lại công trình và cải tạo không gian bên trong thành một căn hộ sinh hoạt độc đáo để bán đấu giá:

* Cấu trúc cầu thang xoắn ốc chạy dọc thân tháp:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050514.webp)

* Không gian phòng sinh hoạt bên trong tháp sau khi cải tạo:

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050515.webp)

2、**Bí ẩn đằng sau thiết kế nâng cao thanh ngang của chữ F trong bảng hiệu của công viên Disney**

Tại khu vực cổng vào của công viên Disneyland California Adventure thời kỳ đầu có bố trí một cụm chữ cái lớn ghép thành từ “CALIFORNIA” chào đón du khách:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080104.webp)

Cụm chữ cái sử dụng phông chữ Futura Condensed nổi tiếng. Tuy nhiên nếu quan sát kỹ, người xem sẽ nhận thấy chữ cái F có sự thay đổi cấu trúc nhỏ so với thiết kế phông chữ gốc:

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080105.webp)

*Hình ảnh trên mô tả đường viền màu trắng của phông chữ gốc và màu xanh lá của chữ cái thực tế sau khi sửa đổi: thanh ngang phía dưới của chữ F đã được nâng lên cao hơn hẳn.*

Các kỹ sư thiết kế của Disney giải thích sự thay đổi này nhằm hai mục đích an toàn thực tế: nâng cao thanh ngang để ngăn trẻ em trèo lên ngồi chơi trên chữ cái gây nguy cơ ngã, đồng thời tránh việc du khách đi bộ phía dưới vô tình va đầu vào cạnh của thanh ngang chữ F.

## ✍️ Bài đọc thêm

### Góc khuất quy trình sản xuất của ngành công nghiệp thiết bị âm thanh tiêu dùng

Tôi đã có vài năm làm việc tại bộ phận kế hoạch của một doanh nghiệp chuyên sản xuất thiết bị âm thanh tiêu dùng (tai nghe và loa cầm tay) hướng tới phân khúc thị trường trung cấp với giá bán sản phẩm dao động từ 100 đến 300 USD.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080306.webp)

Dưới đây tôi xin chia sẻ một số quy luật vận hành thực tế của ngành này – những điều vốn không phải là bí mật đối với người trong ngành nhưng hầu như người tiêu dùng bên ngoài không hề hay biết:

**1. Chi phí sản xuất thực tế thường không vượt quá 30% giá bán lẻ**

Một chiếc tai nghe được bán trên kệ với giá 100 USD thì chi phí nguyên vật liệu và nhân công sản xuất tại nhà máy chỉ rơi vào khoảng 30 USD. Khoảng 50 USD sẽ thuộc về chiết khấu của đại lý bán lẻ và 20 USD còn lại là biên lợi nhuận gộp của thương hiệu. Đối với các dòng tai nghe phân khúc cao cấp, chi phí sản xuất thực tế của chúng không cao hơn nhiều so với hàng trung cấp, mức giá đắt đỏ chủ yếu đến từ giá trị định vị thương hiệu.

**2. Rất ít hãng âm thanh sở hữu nhà máy sản xuất riêng**

Hầu như tuyệt đại đa số các thương hiệu âm thanh nổi tiếng trên thị trường hiện nay đều hoạt động dưới dạng mua bản quyền thiết kế OEM/ODM hoặc thuê các nhà máy gia công bên thứ ba lắp ráp sản phẩm chứ không trực tiếp vận hành dây chuyền sản xuất.

**3. Các nhà máy gia công thừa năng lực sản xuất đồ cao cấp, nhưng khách hàng không yêu cầu**

Nhiều người cho rằng chất lượng gia công của các nhà máy Trung Quốc là kém. Thực tế, các kỹ sư và nhà máy tại đây hoàn toàn đủ năng lực sản xuất ra các linh kiện âm thanh chất lượng đỉnh cao. Tuy nhiên, các thương hiệu đặt hàng gia công luôn yêu cầu nhà máy phải cắt giảm chi phí tối đa để hạ giá thành sản xuất. Doanh nghiệp luôn ưu tiên bán 100.000 sản phẩm giá rẻ để thu lời mỏng hơn là sản xuất 100 sản phẩm cao cấp kén người mua.

**4. Việc thành lập một hãng âm thanh ngày nay không đòi hỏi bằng cấp kỹ sư**

Trong kỷ nguyên chuỗi cung ứng toàn cầu hóa hiện nay, bạn hoàn toàn có thể tự xây dựng một thương hiệu tai nghe của riêng mình mà không cần sở hữu bằng cấp kỹ thuật nào. Mọi khâu từ nghiên cứu màng loa, thiết kế mạch cho đến gia công vỏ hộp đều có thể thuê ngoài trọn gói từ các đối tác chuyên nghiệp. Thương hiệu chỉ cần tập trung nguồn lực vào khâu làm marketing, lên kế hoạch truyền thông và định giá bán sản phẩm.

**5. Chi phí vận chuyển và bao bì đóng hộp chiếm tỷ trọng rất lớn**

Đối với các dòng tai nghe nhét tai (in-ear) phân khúc giá rẻ, chi phí sản xuất và in ấn vỏ hộp carton đẹp đẽ bên ngoài đôi khi còn cao hơn cả chi phí sản xuất của chính củ tai nghe bên trong. Bạn hoàn toàn có thể mua một cặp tai nghe giá gốc tại xưởng chỉ 2 USD, đặt nó vào một vỏ hộp sang trọng có chi phí in ấn 3 USD và bán nó trên Amazon với giá 20 USD.

Tóm lại, tỷ lệ chi phí sản xuất chiếm 30% giá bán lẻ là mức phân bổ hoàn toàn hợp lý và công bằng đối với các thương hiệu có đầu tư nghiên cứu phát triển thực sự. Nếu ép giá thành sản phẩm xuống quá thấp, người tiêu dùng sẽ chỉ nhận lại những sản phẩm có chất lượng gia công cực kỳ kém hoặc doanh nghiệp sẽ sớm bị phá sản do không đủ chi phí duy trì bộ máy.

## Lịch sử tuần này

- 2022年（第 218 期）：[Khí hậu: Mối liên hệ giữa sản lượng thu hoạch nho, mùa hoa anh đào nở sớm và hiện tượng nóng lên toàn cầu](http://www.ruanyifeng.com/blog/2022/08/weekly-issue-218.html)
- 2021年（第 168 期）：[Trải nghiệm game: Góc nhìn triết học về sự thức tỉnh của trí tuệ nhân tạo trong tựa game Detroit: Become Human](http://www.ruanyifeng.com/blog/2021/07/weekly-issue-168.html)
- 2020年（第 118 期）：[Sự nghiệp: Một số kinh nghiệm hướng nghiệp và cách lựa chọn ngành học phù hợp cho các sĩ tử sau kỳ thi đại học](http://www.ruanyifeng.com/blog/2020/07/weekly-issue-118.html)
- 2019年（第 68 期）：[Phát triển cá nhân: Tại sao việc tập trung tích lũy năng lực chuyên môn trong giai đoạn đầu sự nghiệp lại quan trọng hơn mức lương ban đầu](http://www.ruanyifeng.com/blog/2019/08/weekly-issue-68.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge organization and team coordination intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
