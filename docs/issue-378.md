# Bản tin chia sẻ công nghệ (Số 378): Dự đoán chính là xu hướng Internet mới

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/8332) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121101.webp)

Tháp cầu nâng hạ thang máy đầu tiên tại Vũ Hán vừa được khánh thành đi vào hoạt động. Do khu vực thượng nguồn sông có một nhà máy đóng tàu lớn nên cây cầu được thiết kế với 4 tháp nâng hạ khổng lồ để kéo nâng toàn bộ nhịp cầu lên cao khi có tàu lớn đi qua. ([via](https://www.wuhan.gov.cn/sy/whyw/202511/t20251101_2670804.shtml))

## 预测是新的互联网热点

Bạn có thể không ngờ rằng xu hướng công nghệ nóng nhất trên Internet Mỹ hiện nay không phải là các trang web AI thông thường mà lại là một thể loại website hoàn toàn mới, gọi là "**thị trường dự đoán (prediction market)**".

Các trang web thuộc thể loại này đang mọc lên như nấm sau mưa mỗi ngày. Nổi tiếng nhất trong số đó ở thời điểm hiện tại chính là [PolyMarket](https://polymarket.com/).

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121107.webp)

Mục đích của thị trường dự đoán là đưa ra phán đoán về khả năng xảy ra của mọi sự kiện trong đời sống. Lấy ví dụ với PolyMarket, ngay đầu trang chủ của họ là danh mục phân loại các sự kiện dự đoán:

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121108.webp)

> Sự kiện hot, Sự kiện đột xuất, Dự đoán mới nhất, Chính trị, Thể thao...

**Bất kỳ sự kiện nào bạn có thể nghĩ ra trong đầu, trang web đều có phần dự đoán tương ứng**.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121109.webp)

Lấy ví dụ với các sự kiện hot trên trang chủ vào tuần trước (hình trên):

> - Nhân vật của năm do tạp chí 《Time》 bình chọn là ai?
> - Liệu danh sách Nhân vật của năm của 《Time》 có bị rò rỉ trước không?
> - Quyết định lãi suất của Cục Dự trữ Liên bang Mỹ (Fed) vào tháng 1 là gì?
> - Thời điểm ra mắt dòng mô hình AI lớn tiếp theo của OpenAI là khi nào?

Bạn chỉ cần chọn một chủ đề bất kỳ và click vào bên trong sẽ thấy bảng tỷ lệ phần trăm cơ hội cho từng kịch bản xảy ra.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121110.webp)

Bức ảnh trên là dự đoán về số lượng bài viết (tweets) mà Elon Musk sẽ đăng tải trên X trong giai đoạn từ ngày 5 đến ngày 12 tháng 12 năm 2025.

Có thể thấy kịch bản có tỷ lệ cược cao nhất là từ 440 đến 450 bài viết với cơ hội đạt 33%, trong khi kịch bản thấp nhất là từ 400 đến 419 bài viết với cơ hội chỉ vỏn vẹn 1%.

Chính nhờ khả năng cập nhật tỷ lệ phần trăm cơ hội theo thời gian thực cho hầu hết mọi sự kiện xã hội, người dân Mỹ hiện tại đã bắt đầu giảm bớt sự tin tưởng vào các cuộc khảo sát dư luận truyền thống (polls) mà chuyển sang theo dõi các trang web dự đoán kiểu này. Bởi các cuộc khảo sát dư luận luôn có những hạn chế cố hữu về mặt phương pháp chọn mẫu và quy mô mẫu thử, trong khi các trang web dự đoán lại phản ánh sinh động và thực tế hơn quan điểm chung của thị trường.

Bạn sẽ tự hỏi: Làm thế nào các con số dự đoán này được tạo ra? Và làm sao bảo đảm được tính chính xác của chúng?

Câu trả lời cực kỳ đơn giản: **Các con số được quyết định bởi chính dòng tiền đặt cược của người dùng**.

Bạn tin tưởng vào kịch bản nào xảy ra thì có thể chi tiền đặt cược vào cửa đó. Kịch bản nào nhận được nhiều dòng tiền đặt cược thì tỷ lệ phần trăm cơ hội tương ứng sẽ tự động tăng lên, và ngược lại.

Về bản chất, mỗi kịch bản dự đoán tương đương với một mã cổ phiếu trên thị trường chứng khoán, với giá cổ phiếu chính là tỷ lệ phần trăm cơ hội xảy ra của nó: 1% cơ hội tương đương giá cổ phiếu 0,01 USD, và 100% cơ hội tương đương giá cổ phiếu 1 USD.

Ví dụ: Một kịch bản bất ngờ hiện tại chỉ có tỷ lệ cơ hội xảy ra là 2% (tương đương giá cổ phiếu 0,02 USD). Bạn tin tưởng kịch bản này chắc chắn sẽ diễn ra nên quyết định bỏ ra 100 USD để mua vào.

Nếu kịch bản đó thực sự diễn ra ngoài đời thực, tỷ lệ cơ hội của nó sẽ tăng lên 100% (tương ứng giá cổ phiếu đạt mốc 1 USD) – tức tăng gấp 50 lần so với thời điểm bạn mua vào. Khi đó, khoản tiền 100 USD đầu tư ban đầu của bạn sẽ biến thành 5.000 USD.

Ngược lại, nếu dự đoán của bạn sai và kịch bản đó không xảy ra, tỷ lệ cơ hội sẽ về mức 0% (giá trị 0 USD), và bạn sẽ mất trắng toàn bộ khoản tiền 100 USD đã bỏ ra.

Gần đây có [một tin tức rất hot](https://decrypt.co/351829/how-one-polymarket-user-turned-3k-into-125k-with-a-single-prediction) tại Mỹ về một người đàn ông đã mạo hiểm chi 3.000 USD đặt cược vào một kịch bản chỉ có 2% cơ hội xảy ra trên PolyMarket. Kết quả dự đoán chính xác đã giúp anh thu về tới 125.000 USD tiền thưởng.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121313.webp)

Để tạo điều kiện thuận lợi cho người dùng ở khắp nơi trên thế giới dễ dàng tham gia và bảo đảm tính ẩn danh, các trang web dự đoán này đều sử dụng các đồng tiền ổn định (stablecoin) để giao dịch.

Vì thế, bản chất của hệ thống này chính là một thị trường xổ số khổng lồ cho phép người dùng tự do giao dịch và đặt cược vào những chủ đề mà họ yêu thích và am hiểu nhất. Đây chính là động lực cốt lõi giúp mô hình này phát triển thần tốc. Và khi số lượng người tham gia đặt cược càng đông, các con số dự đoán phản ánh ngược lại sẽ càng đạt độ chính xác cao.

Tôi tin rằng mô hình này sở hữu tiềm năng phát triển vô cùng to lớn và sẽ bùng nổ mạnh mẽ trong tương lai gần, thậm chí có khả năng thay thế hoàn toàn mô hình xổ số truyền thống.

Nó biến mọi sự kiện không chắc chắn trong tương lai thành những tấm vé xổ số, trực quan hóa xác suất xảy ra của từng kịch bản theo thời gian thực và cung cấp cơ hội nhân nhiều lần tài sản cho người tham gia. Một mặt, đây là kênh tham khảo thông tin cực tốt để phán đoán các xu hướng tương lai, mặt khác nó lại mang tính giải trí và kích thích tinh thần vô cùng lớn đối với người chơi.

## 国产 Nano Banana Pro 的图片幻灯片生成

Tháng trước, Google đã ra mắt mô hình chỉnh sửa hình ảnh thế hệ mới mang tên Nano Banana Pro (đây thực chất là nhánh xử lý hình ảnh của Gemini 3 Pro).

Trong đó có một tính năng đã tạo nên cơn sốt: **Có khả năng biến mọi đoạn văn bản thô ráp, nhàm chán nhất thành những hình ảnh minh họa sinh động**, giúp chuyển đổi trải nghiệm từ "đọc văn bản" sang "xem hình ảnh".

Thời điểm đó tôi đã nghĩ rằng các mô hình trí tuệ nhân tạo trong nước chắc chắn sẽ nhanh chóng nghiên cứu và tung ra tính năng tương tự.

Quả thực, hôm qua khi mở trang của Mita AI (秘塔 AI), tôi thấy họ vừa cho ra mắt [tính năng này](https://mp.weixin.qq.com/s/CijVsVvj_MhyF6iezbO0Jg), được định vị đối đầu trực tiếp với Nano Banana Pro và NotebookLM, đồng thời tích hợp thêm một tính năng độc đáo của riêng mình – đó là thuyết trình bằng giọng nói.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121809.webp)

Bạn chỉ cần click vào nút "Tải tài liệu lên" (hình trên) và chọn các tài liệu tham khảo của mình (hỗ trợ tải lên nhiều tài liệu cùng lúc), hệ thống sẽ tự động phân tích xây dựng cơ sở kiến thức và xuất ra phần tóm tắt nội dung bằng AI. Lúc này, giao diện sẽ xuất hiện thêm nút "Thuyết trình cho tôi nghe".

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121810.webp)

Hình ảnh trên mô tả quá trình tôi tải lên một tài liệu hướng dẫn lập trình về cú pháp [Promise trong JavaScript](https://wangdoc.com/es6/promise) do tôi biên soạn. Khi click vào nút thuyết trình, hệ thống lập tức tự động sinh ra một slide trình chiếu kèm hình ảnh minh họa sinh động và chạy giọng thuyết minh tương ứng.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121811.webp)

Các bạn có thể truy cập trang chủ của họ tại địa chỉ [metaso.cn](https://metaso.cn/) (hoặc tải ứng dụng di động cùng tên) để trải nghiệm thử. Tính năng này vô cùng thú vị, giao diện trực quan dễ sử dụng và hoàn toàn **miễn phí** (thông qua hệ thống tặng điểm thưởng hàng ngày).

Bên cạnh việc tải tài liệu lên trực tiếp, bạn cũng có thể **gõ tìm kiếm nhanh một chủ đề bất kỳ, sau đó click vào nút "Tạo slide trình chiếu" ở bên dưới**. Hệ thống hỗ trợ tùy chọn tạo slide kèm hình ảnh với hơn 20 phong cách thiết kế khác nhau để bạn thoải mái lựa chọn và chỉnh sửa.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121812.webp)

## 科技动态

1. **Hành trình đi bộ vòng quanh thế giới**

Vào một ngày của thập niên 1990, một thanh niên người Anh đã tùy tiện tuyên bố trong quán rượu rằng anh có thể đi bộ ròng rã từ điểm cực nam của Nam Mỹ về tới Anh quốc. Bạn bè xung quanh đều không ai tin lời anh nói.

Anh đã cá cược với bạn bè rằng mình sẽ làm được. Năm 1998, anh chính thức bắt đầu hành trình đi bộ của mình từ điểm cực nam Chile ở tuổi 29.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121303.webp)

Hiện tại đã 27 năm trôi qua, anh đã ở tuổi 56 và vẫn đang tiếp tục hành trình trên những cung đường.

Tin vui là anh đã tiến rất sát tới chặng cuối cùng của cuộc hành trình, dự kiến sẽ đặt chân tới đích đến là nước Anh vào tháng 9 năm 2026.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121306.webp)

Dưới đây là sơ đồ lộ trình di chuyển của anh: xuất phát từ điểm cực nam của Nam Mỹ, đi dọc lên điểm cực bắc của Bắc Mỹ, vượt qua eo biển sang châu Á, đi qua châu Âu và cuối cùng trở về Anh.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121305.webp)

Trong suốt cả hành trình dài, anh chỉ được phép đi bộ hoặc tự bơi qua các vùng nước chứ hoàn toàn không được sử dụng bất kỳ phương tiện giao thông nào. Chặng đường gian nan nhất là việc vượt qua eo biển Bering ngăn cách giữa Bắc Mỹ và Nga. Để không phải lên tàu thuyền, anh đã chọn cách bò qua lớp băng biển đóng dày trong mùa đông lạnh giá.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121309.webp)

Trong suốt 27 năm qua, không phải ngày nào anh cũng đi bộ liên tục. Đôi khi vì các lý do bất khả kháng, anh phải tạm dừng hành trình một thời gian trước khi quay trở lại điểm dừng cũ để tiếp tục bước đi.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121307.webp)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121308.webp)

Anh chia sẻ rằng chỉ dựa vào nỗ lực của một cá nhân thì không thể hoàn thành được hành trình vĩ đại này, nó đòi hỏi sự ủng hộ to lớn từ gia đình, sự giúp đỡ nhiệt thành của những người lạ bắt gặp trên đường và cả nguồn tài trợ từ các nhà hảo tâm.

Về nguồn động lực giúp anh kiên trì đi bộ suốt gần 30 năm qua, anh chia sẻ: "Bạn cần phải tự mình quan sát thế giới thực tại và cuộc sống của những con người đang sinh sống trên đó, đây chính là lớp học giáo dục tốt nhất mà bạn có thể nhận được trong đời."

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121310.webp)

2. **Robot 6 tay**

Tập đoàn Midea (美的) vừa giới thiệu mẫu robot 6 tay thế hệ mới, dự kiến sẽ được đưa vào vận hành tại dây chuyền sản xuất của nhà máy Vô Tích.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121301.webp)

Robot sở hữu khả năng phối hợp 6 cánh tay để thực hiện đồng thời 3 tác vụ khác nhau cùng một lúc. Nhờ vậy, hiệu suất làm việc của 1 robot có thể tương đương với 3 công nhân bình thường cộng lại.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121302.webp)

3. **Máy giặt quay tay**

Một cựu kỹ sư của hãng Dyson vừa phát minh ra một mẫu máy giặt quay tay chuyên dụng dành cho các khu vực kém phát triển trên thế giới.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121401.webp)

Thiết bị hoàn toàn không tiêu thụ điện năng, người dùng chỉ cần quay tay trong vài phút là có thể giặt sạch 5kg quần áo, đồng thời giúp tiết kiệm tới một nửa lượng nước sử dụng so với thông thường.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121402.webp)

Nếu sản phẩm này thực sự hiệu quả, tôi xin đưa ra một gợi ý nhỏ: nên chuyển đổi cơ chế quay tay thành đạp bàn đạp giống như đi xe đạp, chỉ cần đạp chân 5 phút là có thể hoàn thành một mẻ giặt đồ.

## 文章

1. [Sự bế tắc của các lập trình viên khi tự đặt tên cho các công cụ của mình](https://larr.net/p/namings.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121204.webp)

Bài viết đưa ra những lời phê bình đối với thói quen của nhiều lập trình viên khi đặt những cái tên vô nghĩa, kỳ dị cho các phần mềm họ phát triển, khiến người dùng hoàn toàn không thể đoán biết được công dụng của công cụ. Tác giả khuyên tên phần mềm nên có sự liên hệ logic với tính năng thực tế của nó.

2. [Giải mật tài liệu rò rỉ của Edward Snowden](https://libroot.org/posts/going-through-snowden-documents-part-1/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121203.webp)

Bài viết phân tích chi tiết các tài liệu mật do Edward Snowden rò rỉ vào năm 2013. Phần đầu tiên của loạt bài tập trung phân tích hoạt động tình báo của Mỹ nhắm vào tập đoàn công nghiệp quốc phòng Norinco của Trung Quốc, cho thấy quy mô giám sát đáng kinh ngạc của tình báo Mỹ.

3. [Hành trình chuyển đổi từ văn bản thô sang các Token từ nguyên](https://www.paradedb.com/blog/when-tokenization-becomes-token) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121311.webp)

Bài viết khoa học phổ thông giải thích một cách dễ hiểu cơ chế hoạt động của các bộ máy tìm kiếm khi thực hiện bóc tách và chuyển đổi các đoạn văn bản truy vấn thô sang các Token từ nguyên chuẩn hóa phục vụ tra cứu dữ liệu.

4. [Phương pháp ứng dụng mô hình AI hiệu quả để sinh nhanh các trang web HTML](https://simonwillison.net/2025/Dec/10/html-tools/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121105.webp)

Bài viết dài của lập trình viên nổi tiếng Simon Willison tổng hợp lại những bài học kinh nghiệm thực tế của ông khi sử dụng các mô hình AI lớn để sinh và hoàn thiện các ứng dụng web chạy trên trình duyệt.

5. [Thời kỳ tuần trăng mật của công nghệ GraphQL đã khép lại](https://johnjames.blog/posts/graphql-the-enterprise-honeymoon-is-over) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121501.webp)

Tác giả lập luận rằng phạm vi giải quyết vấn đề của GraphQL thực tế hẹp hơn rất nhiều so với những gì người ta tưởng tượng, và hoàn toàn có thể xử lý tốt bằng các phương án khác đơn giản hơn. Việc lạm dụng công nghệ này trong doanh nghiệp hiện nay đang mang lại nhiều gánh nặng kỹ thuật hơn là lợi ích thực tế.

6. [Giải thích chi tiết về tham số `-p` của lệnh `git add`](https://techne98.com/blog/using-git-add-p/) (tiếng Anh)

Bài viết giới thiệu về lệnh `git add -p`. Khi thực thi, hệ thống sẽ hiển thị một giao diện tương tác trực quan cho phép lập trình viên duyệt và xác nhận từng thay đổi nhỏ (hunk) trong mã nguồn trước khi đưa vào vùng tạm lưu (staging area).

## 工具

1. [Cosmic](https://system76.com/cosmic)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121202.webp)

Phiên bản Cosmic 1.0 chính thức được phát hành vào tuần trước. Đây là một môi trường desktop hoàn toàn mới dành cho hệ điều hành Linux với giao diện tuyệt đẹp và các tính năng mạnh mẽ, mang lại sự lựa chọn chất lượng bên cạnh hai giao diện quen thuộc là Gnome và KDE.

2. [Keyden](https://github.com/tasselx/Keyden)

Ứng dụng mã nguồn mở chạy trên thanh menu của hệ điều hành macOS hỗ trợ tạo mã xác thực hai lớp (TOTP), toàn bộ khóa bảo mật được mã hóa và lưu trữ an toàn trong macOS Keychain. (Đóng góp từ [@tasselx](https://github.com/ruanyf/weekly/issues/8446))

3. [WeMD](https://github.com/tenngoxars/WeMD)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121205.webp)

Trình soạn thảo văn bản hỗ trợ định dạng Markdown mã nguồn mở chuyên dụng để thiết kế bài viết cho trang WeChat Official Accounts. (Đóng góp từ [@tenngoxars](https://github.com/ruanyf/weekly/issues/8432))

4. [starling-speak](https://starling-speak.online/)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121106.webp)

Trang web hỗ trợ chuyển đổi văn bản thành giọng nói đa ngôn ngữ tích hợp sẵn tính năng ghi âm giọng đọc trực tiếp trên trình duyệt. (Đóng góp từ [@Keldon-Pro](https://github.com/ruanyf/weekly/issues/8424))

5. [shift](https://github.com/hubenchang0515/shift)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121312.webp)

Trình soạn thảo mã nguồn trực tuyến vận hành dựa trên công nghệ WebAssembly, cho phép chạy trực tiếp các đoạn code Python, Lua hay Ruby ngay trên trình duyệt web mà không cần cài đặt môi trường. (Đóng góp từ [@hubenchang0515](https://github.com/ruanyf/weekly/issues/8440))

6. [EasyImg](https://github.com/chaos-zhu/easyimg)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121404.webp)

Giải pháp tự xây dựng kho lưu trữ hình ảnh (image hosting/图床) cá nhân phát triển dựa trên Nuxt 4, trang bị trang quản trị admin cấu hình phong phú. (Đóng góp từ [@chaos-zhu](https://github.com/ruanyf/weekly/issues/8443))

7. [Go-WXPush](https://github.com/hezhizheng/go-wxpush)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121503.webp)

Dịch vụ gửi thông báo tin nhắn qua ứng dụng WeChat viết bằng Go, cung cấp một API giao tiếp cực kỳ tối giản. Dự án mở nguồn mở và hỗ trợ hạn ngạch gửi tin miễn phí lên tới 100.000 lượt/ngày. (Đóng góp từ [@hezhizheng](https://github.com/ruanyf/weekly/issues/8445))

8. [ZeroLaunch-rs](https://github.com/ghost-him/ZeroLaunch-rs)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121504.webp)

Thanh tìm kiếm và khởi chạy nhanh ứng dụng dành cho Windows, hỗ trợ tìm kiếm nhanh bằng chữ bính âm (Pinyin) viết tắt, phát triển bằng Rust phối hợp Tauri và Vue.js. (Đóng góp từ [@ghost-him](https://github.com/ruanyf/weekly/issues/8453))

9. [MrRSS](https://github.com/WCY-dt/MrRSS)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121505.webp)

Ứng dụng đọc tin RSS mã nguồn mở đa nền tảng chạy trên desktop, tích hợp sẵn các trợ lý AI hỗ trợ tự động dịch thuật, tóm tắt tin tức và gợi ý các nguồn tin mới. (Đóng góp từ [@ch3ny4ng](https://github.com/ruanyf/weekly/issues/8454))

10. [PVE Touch](https://github.com/hanxi/pve-touch)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121601.webp)

Giao diện quản trị hệ thống ảo hóa Proxmox VE được tối ưu hóa cho màn hình cảm ứng di động, giúp quản lý các máy ảo dễ dàng ngay trên điện thoại. (Đóng góp từ [@hanxi](https://github.com/ruanyf/weekly/issues/8455))

## AI 相关

1. [Disco](https://labs.google/disco)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121207.webp)

Dự án trình duyệt tích hợp trí tuệ nhân tạo thử nghiệm do Google Labs phát triển, cho phép người dùng nhận trực tiếp câu trả lời bỏ qua bước tìm kiếm web thông thường, hiện đang mở đăng ký danh sách chờ trải nghiệm.

2. [Flowers](https://github.com/snailfrying/flowers)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121206.webp)

Plugin trợ lý AI mã nguồn mở trên trình duyệt, cung cấp các tính năng dịch thuật nội dung trang web, hỏi đáp nhanh và tạo ghi chú thông minh. (Đóng góp từ [@snailfrying](https://github.com/ruanyf/weekly/issues/8434))

3. [DeepAudit](https://github.com/lintsinghua/DeepAudit)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121602.webp)

Nền tảng kiểm thử mã nguồn mã nguồn mở vận hành bằng AI Agent, hỗ trợ tự động dò quét phát hiện lỗ hổng bảo mật và chạy xác thực mã độc trong môi trường hộp cát (sandbox). Dự án hỗ trợ kết nối với Ollama để chạy mô hình local bảo đảm mã nguồn không bị lọt ra ngoài mạng nội bộ. (Đóng góp từ [@lintsinghua](https://github.com/ruanyf/weekly/issues/8456))

## 资源

1. [So sánh kích thước của các sinh vật sống (neal.fun/size-of-life)](https://neal.fun/size-of-life/)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121104.webp)

Trang web trực quan hóa kích thước so sánh của các thực thể sống trên Trái Đất, bắt đầu từ chuỗi DNA siêu nhỏ cho tới loài cá voi xanh khổng lồ.

2. [Hướng dẫn tự lập trình trình biên dịch Lisp bằng ngôn ngữ C](https://buildyourownlisp.com/contents)

Sách điện tử tiếng Anh miễn phí dành cho người mới bắt đầu, hướng dẫn quy trình viết một trình biên dịch đơn giản cho ngôn ngữ Lisp bằng ngôn ngữ lập trình C.

3. [A Soft Murmur](https://asoftmurmur.com/)

Trang web cung cấp hệ thống âm thanh nền thư giãn, cho phép người dùng tự do lựa chọn kết hợp và điều chỉnh âm lượng của nhiều hiệu ứng âm thanh tự nhiên khác nhau (tiếng mưa, tiếng sóng, tiếng gió...).

## 图片

1. **Vẽ tranh động vật từ 13 hình tròn**

Một nghệ sĩ đồ họa đã thử thách bản thân bằng việc vẽ phác họa chân dung các loài động vật chỉ bằng việc kết hợp từ đúng 13 hình tròn:

Hình chim cú mèo:

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025040304.webp)

Hình thỏ con:

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025040305.webp)

Hình khỉ con:

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025040306.webp)

## 文摘

1. [Claude 4.5 Opus là mô hình AI đầu tiên khiến tôi thực sự lo ngại về nguy cơ mất việc làm](https://www.reddit.com/r/ClaudeAI/comments/1pmgk5c/opus_45_is_the_first_model_that_makes_me_actually/)

Trải nghiệm với Claude 4.5 Opus thực sự mang lại sự khác biệt hoàn toàn so với các dòng mô hình AI khác trước đó. Những ai chưa từng trực tiếp sử dụng nó sẽ khó lòng hình dung được những thay đổi to lớn sẽ diễn ra trong vòng 2 đến 3 năm tới, và năm sau rất có thể sẽ là cột mốc chuyển dịch mang tính quyết định.

Tôi băn khoăn không biết bản thân nên làm thế nào để thích nghi tiếp theo. Ở giai đoạn hiện tại, tôi hoàn toàn có thể giao việc cho Opus tự chạy và thỉnh thoảng can thiệp sửa một vài lỗi nhỏ, nhưng chỉ một thời gian ngắn nữa thôi thì ngay cả bước can thiệp nhỏ đó cũng không còn cần thiết nữa.

Bài toán viết code cơ bản coi như đã được AI giải quyết triệt để, tiếp theo các mảng việc như thiết kế kiến trúc hệ thống hay bảo mật mạng cũng sẽ sớm được AI xử lý trơn tru. Tôi ước tính chỉ cần trải qua khoảng 2 đến 3 bản cập nhật lớn nữa thôi, 80% lực lượng nhân sự kỹ thuật công nghệ hiện nay sẽ trở nên dư thừa. Tất nhiên các doanh nghiệp sẽ cần một khoảng thời gian đệm để tái cấu trúc tổ chức, nhưng họ chắc chắn sẽ tìm mọi phương án tối ưu để cắt giảm nhân sự lập trình nhanh nhất có thể.

Dù bản thân là một người vô cùng đam mê công nghệ AI nhưng tôi vẫn không khỏi chạnh lòng và lo lắng khi nghĩ về tương lai mà công nghệ này đang hướng tới.

2. [Lý do chúng ta cần học bộ môn Vật lý](https://calteches.library.caltech.edu/46/2/LatinAmerica.htm)

*(Bài viết trích từ bài phát biểu của nhà vật lý lỗi lạc Richard Feynman vào tháng 6 năm 1963 tại Hội nghị Giáo dục Vật lý Châu Mỹ diễn ra ở Rio de Janeiro).*

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025121603.webp)

Có 5 nguyên nhân cốt lõi giải thích tại sao chúng ta bắt buộc phải giảng dạy bộ môn Vật lý trong nhà trường:

（1）Vật lý là môn khoa học nền tảng, làm cơ sở ứng dụng cho rất nhiều ngành kỹ thuật công nghệ khác nhau như kỹ thuật công nghiệp, hóa học hay sinh học.

Vật lý là môn khoa học nghiên cứu và thấu hiểu các quy luật vận hành của tự nhiên, giúp con người hiểu được cơ chế hoạt động của vạn vật xung quanh cũng như nguyên lý vận hành của các thiết bị công nghệ hiện đại. Do đó, một người nắm vững kiến thức vật lý sẽ sở hữu năng lực xử lý rất tốt các vấn đề kỹ thuật phát sinh trong thực tế công việc.

（2）Bộ môn Vật lý rèn luyện cho bạn kỹ năng thực hành và vận hành công việc. Nó đào tạo các kỹ năng đo lường, tính toán và xử lý vật chất thực tế – những năng lực có phạm vi ứng dụng rộng lớn hơn nhiều so với một lĩnh vực nghiên cứu học thuật thuần túy.

（3）Đối với nhiều người, việc nghiên cứu Vật lý học mang lại một niềm vui tinh thần vô cùng to lớn.

Quá trình đào tạo khoa học giúp hình thành nên các nhà khoa học, những người không chỉ đóng góp trực tiếp cho sự phát triển của công nghiệp và kho tàng tri thức nhân loại, mà bản thân họ còn được tham gia vào cuộc phiêu lưu vĩ đại của thời đại và nhận về niềm vui khám phá to lớn.

Ngay cả đối với một người bình thường không đi theo con đường nghiên cứu chuyên nghiệp, việc học vật lý cũng giúp họ biết cách chiêm ngưỡng vẻ đẹp và sự kỳ diệu của thế giới tự nhiên xung quanh. Sự thấu hiểu tự nhiên mang lại cho con người cảm giác vững chãi, thực tế và giúp xua tan đi nhiều nỗi sợ hãi cùng các định kiến mê tín dị đoan.

（4）Vật lý dạy cho con người cách nhận biết thế giới và rèn luyện tư duy phản biện hoài nghi khoa học trước mọi vấn đề. Giá trị của việc hoài nghi và tự do tư duy là vô cùng rõ nét không chỉ cho khoa học mà cho tất cả các lĩnh vực đời sống.

Khoa học dạy chúng ta cách nhận thức bản chất vấn đề: đâu là những điều chưa biết, mức độ thấu hiểu của chúng ta đối với sự vật đã đạt đến đâu, cách thức đối diện với những nghi ngờ và sự không chắc chắn, các quy tắc xác thực chứng cứ là gì, và phương pháp tư duy để đưa ra các phán đoán độc lập phân định giữa sự thật và sự lừa dối. Đây chính là những giá trị giáo dục cốt lõi nhất của bộ môn Vật lý.

（5）Trong suốt hành trình học hỏi khoa học, bạn sẽ học được phương pháp thử và sai (trial and error), từ đó nuôi dưỡng tinh thần tự do khám phá và phát minh sáng tạo – những phẩm chất có giá trị vượt xa phạm vi của riêng ngành khoa học.

Người học sẽ luôn tự đặt ra câu hỏi cho bản thân: "Liệu có phương án nào tối ưu hơn không?". Ý thức này chính là cội nguồn của mọi ý tưởng đột phá, các phát minh sáng tạo và là động lực thúc đẩy mọi tiến trình văn minh của nhân loại.

## 言论

1.

Tại sao con người lại sở hữu hai lỗ mũi thay vì chỉ là một chiếc hố lớn duy nhất trên khuôn mặt?

Bởi phổi của chúng ta cần được cung cấp dưỡng khí liên tục không ngừng nghỉ, việc thiết kế hai lỗ mũi giúp hệ thống có khả năng luân phiên hoạt động để một bên mũi có thời gian nghỉ ngơi và hồi phục độ ẩm.

-- Tạp chí khoa học 《Popular Science》 của Mỹ

2.

Một tòa soạn tuyển dụng tôi vào vị trí biên tập viên viết bài. Tôi cứ ngỡ công việc của mình là trực tiếp viết bài, nhưng thực tế họ lại chi trả mức thù lao cực thấp và bắt tôi làm công việc chỉnh sửa lại các bản thảo bài viết do AI tự động sinh ra, với lý do là "hầu hết các phần việc khó khăn đã được AI hoàn thành giúp rồi".

Điều này thực sự giáng một đòn mạnh vào lòng tự trọng nghề nghiệp của tôi. Tôi từng nghĩ năng lực viết lách của mình là có giá trị và được tôn trọng, tự tin hướng tới một sự nghiệp rạng rỡ, nhưng giờ đây công việc hàng ngày chỉ là đi dọn rác ngôn từ cho các văn bản do máy tự sinh.

-- Chia sẻ từ một nhà viết bài tự do (freelance copywriter)

3.

Ngành công nghiệp phần mềm dịch vụ SaaS sẽ đối mặt với sự suy thoái nghiêm trọng, đặc biệt là các phần mềm SaaS có tính năng đơn giản. Bởi hiện nay các doanh nghiệp hoàn toàn có thể sử dụng AI để tự sinh nhanh các dịch vụ vận hành nội bộ đáp ứng tốt nhu cầu mà không cần thuê ngoài.

-- [《Trí tuệ nhân tạo đang gặm nhấm thị phần SaaS》](https://martinalderson.com/posts/ai-agents-are-starting-to-eat-saas/)

4.

Tôi nhận thấy trong giao tiếp ngôn ngữ, người Trung Quốc thường có xu hướng tránh việc trả lời khẳng định trực tiếp dạng "Đúng vậy" (True) mà thích sử dụng cấu trúc phủ định kép dạng "Không tệ" (!False) hơn. Ví dụ trong tiếng Anh nói "Very good", tiếng Trung sẽ nói "Không tồi"; tiếng Anh nói "Right", tiếng Trung nói "Không sai"; tiếng Anh nói "Normal", tiếng Trung nói "Không vấn đề gì".

Việc lạm dụng phủ định kép giúp tăng tính linh hoạt và tạo ra không gian回旋 (xoay chuyển) trong giao tiếp, giúp người nói tránh được việc phải thể hiện thái độ hay lập trường quá rõ ràng, dứt khoát ngay lập tức.

-- [《Tại sao tiếng Trung lại từ chối nói True》](https://suggger.substack.com/p/the-architecture-of-not-bad-decoding)

## 往年回顾

[Bạn rất có thể chỉ là một nhân vật NPC trong đời thực](https://www.ruanyifeng.com/blog/2024/12/weekly-issue-331.html) (#331)

[Quyết định chính sách quy hoạch hạ tầng mới](https://www.ruanyifeng.com/blog/2023/12/weekly-issue-281.html) (#281)

[Một công ty Internet thực tế cần quy mô bao nhiêu nhân sự?](https://www.ruanyifeng.com/blog/2022/11/weekly-issue-231.html) (#231)

[Thiết kế thanh toán di động thế nào cho đúng?](https://www.ruanyifeng.com/blog/2021/10/weekly-issue-181.html) (#181)

(Hết)
