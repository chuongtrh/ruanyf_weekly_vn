# Bản tin chia sẻ công nghệ (Số 357): Ván cờ Stablecoin

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/7169) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071601.webp)

Năm thứ hai liên tiếp, thành phố Tây An triển khai mở cửa các hầm trú ẩn phòng không cũ để cải tạo thành những "trung tâm tránh nóng" miễn phí phục vụ người dân, bên trong trang bị đầy đủ bàn ghế, hệ thống Wifi, tivi truyền hình, máy nước uống và nhiều tiện ích thiết thực khác. (Nguồn: [cnwest.com](http://m.cnwest.com/bwyc/a/2025/07/15/23156309.html))

## 稳定币的博弈

Stablecoin (tiền ổn định) đang là tâm điểm chú ý của giới công nghệ tài chính thời gian gần đây và liên tục được truyền thông nhắc tới.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071201.webp)

Khởi nguồn là vào tháng 5 năm nay, chính quyền Hồng Kông đã chính thức thông qua [《Đạo luật Stablecoin》](https://www.hkma.gov.hk/gb_chi/news-and-media/press-releases/2025/05/20250521-3/) và sẽ chính thức có hiệu lực từ ngày 1 tháng 8 tới, cho phép các doanh nghiệp nộp hồ sơ xin cấp phép để phát hành stablecoin hợp pháp.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071202.webp)

Có thể dự báo rằng **sự xuất hiện của stablecoin pháp định tại Hồng Kông sẽ mở ra thêm những cơ hội tài chính và cung cấp thêm một công cụ giao dịch mới hữu ích cho mọi người**.

Tuy nhiên hầu hết mọi người vẫn chưa thực sự thấu hiểu: Stablecoin thực chất là gì và nó mang lại những giá trị ứng dụng thực tế nào?

Dưới đây tôi xin chia sẻ một vài phân tích để làm nổi bật ý nghĩa to lớn của việc Hồng Kông phát hành stablecoin dưới góc nhìn tối giản dễ hiểu nhất.

### (1) Bản chất của Stablecoin

Stablecoin được xếp vào một danh mục của tiền mã hóa (cryptocurrency), và sự ra đời của nó có liên quan mật thiết đến Bitcoin.

Bitcoin là đồng tiền mã hóa đầu tiên của nhân loại nhưng sở hữu mức độ biến động giá cực kỳ khốc liệt. Hôm nay nó có thể tương đương giá trị của 5 chiếc bánh nướng, ngày mai tăng lên 8 chiếc, nhưng ngày kia đã sụt xuống chỉ còn 4 chiếc.

Đặc tính biến động mạnh này khiến Bitcoin hoàn toàn không phù hợp để làm công cụ thanh toán hằng ngày, người dùng thực tế sẽ không muốn mạo hiểm dùng nó để thực hiện mua bán các hàng hóa thông thường khác.

Hệ quả là giới công nghệ đã nghĩ ra giải pháp kiến tạo nên **một dòng tiền mã hóa sở hữu mức giá ổn định — thường gọi là Stablecoin**. Lấy ví dụ đồng stablecoin có vốn hóa lớn nhất thế giới hiện nay là USDT, được công ty Tether phát hành từ năm 2014 (Bitcoin ra đời năm 2009).

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071203.webp)

Công ty Tether đưa ra cam kết bảo đảm tỷ giá của đồng USDT luôn cố định ở mốc 1 USDT đổi 1 USD. Khi bạn gửi cho Tether 1 USD tiền mặt, bạn sẽ nhận về 1 USDT (dữ liệu được ghi nhận an toàn trên sổ cái blockchain). Đến khi không còn nhu cầu sử dụng, bạn có thể gửi trả USDT cho Tether để nhận lại 1 USD tiền mặt tương ứng.

Về mặt lý thuyết, chỉ cần Tether luôn duy trì đầy đủ lượng tài sản USD dự trữ an toàn tương ứng với số lượng coin đã phát hành thì tỷ giá 1:1 với đồng USD sẽ luôn được bảo đảm ổn định. Tether cũng định kỳ công bố báo cáo tài chính chứng minh phần lớn số tiền USD nhận về được họ đem đi đầu tư vào trái phiếu chính phủ Mỹ để đảm bảo thanh khoản, nhờ đó niềm tin của người dùng được củng cố vững chắc.

Một khi xã hội đã công nhận stablecoin sở hữu giá trị tương đương tiền USD thật, thì **ở bất kỳ đâu chấp nhận thanh toán bằng USD, người dùng đều có thể sử dụng stablecoin** để giao dịch mua bán hàng hóa một cách tiện lợi.

Hiện nay USDT đang nắm giữ vị thế đồng tiền mã hóa có khối lượng giao dịch hằng ngày lớn nhất thế giới, vượt qua cả Bitcoin. Phần lớn trường hợp nó được khai thác làm công cụ trung gian để mua bán các đồng tiền mã hóa khác.

### (2) Lách khỏi tầm kiểm soát của Mỹ

Trong quá trình sử dụng stablecoin, người dùng nhanh chóng nhận ra **nó cung cấp khả năng lách qua các hệ thống kiểm soát tài chính của chính phủ Mỹ**.

Mọi luồng di chuyển của stablecoin đều được thực hiện hoàn toàn độc lập bên ngoài hệ thống ngân hàng truyền thống, diễn ra trực tiếp giữa các ví ẩn danh trên blockchain, khiến việc truy vết và áp đặt các biện pháp phong tỏa là cực kỳ khó khăn.

Lấy ví dụ thực tế: Nếu chính phủ Mỹ ban hành lệnh cấm giao dịch bằng USD đối với một cá nhân A nào đó. Trong kịch bản này, cá nhân A hoàn toàn có thể chuyển sang sử dụng stablecoin để mua sắm hàng hóa từ đối tác B, và đối tác B sau đó có thể chủ động quy đổi số stablecoin này ngược trở lại thành USD tiền mặt ở các thị trường tự do.

Chính phủ Mỹ hầu như không có cách nào phát hiện ra giao dịch chuyển nhượng tài sản ngầm này. Dù cơ quan chức năng có nỗ lực giám sát quy trình quy đổi sang USD, người dùng vẫn có thể dễ dàng lách luật bằng cách chuyển đổi stablecoin sang các đồng tiền mã hóa trung gian khác trước khi rút tiền mặt.

Nhận thức rõ lỗ hổng quản lý nghiêm trọng này, chính phủ Mỹ tuần này đang thúc đẩy việc thông qua [《Đạo luật GENIUS》](https://en.wikipedia.org/wiki/GENIUS_Act) — bộ luật toàn diện đầu tiên của lịch sử chuyên trách quản lý hoạt động của các đồng stablecoin.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071609.webp)

Nội dung cốt lõi của đạo luật này tập trung vào 3 quy định nghiêm khắc sau:

1.  Mọi tổ chức phát hành stablecoin (neo giá theo USD) bắt buộc phải đăng ký trụ sở pháp lý trong phạm vi quyền hạn của Mỹ và phải được sự cấp phép của chính phủ.
2.  Tổ chức phát hành bắt buộc phải ký gửi toàn bộ số USD bảo chứng tương ứng 1:1 làm tiền gửi tại hệ thống ngân hàng thương mại được bảo hiểm.
3.  Chính phủ Mỹ có toàn quyền ban hành các lệnh phong tỏa, đóng băng hoặc trực tiếp tiêu hủy các đồng stablecoin (neo giá USD) do các tổ chức nước ngoài phát hành khi cần thiết.

### (3) Nước đi thông minh của Hồng Kông

Đạo luật Stablecoin mới được chính quyền Hồng Kông thông qua được đánh giá là một nước đi chiến lược cực kỳ thông minh: **Đạo luật cho phép các tổ chức được cấp phép phát hành các đồng stablecoin được bảo chứng bằng đồng Đô la Hồng Kông (HKD)**.

Như chúng ta đều biết, tỷ giá giữa HKD và USD từ lâu đã được neo cố định ở mốc 7,8 HKD đổi 1 USD, do đó tỷ giá của đồng stablecoin bảo chứng bằng HKD cũng sẽ tự động neo cố định tương ứng với USD.

Hệ quả là **đồng stablecoin bảo chứng bằng HKD hoàn toàn có thể thay thế vai trò của các đồng stablecoin bảo chứng bằng USD, từ đó gián tiếp thay thế vai trò thanh toán của USD**. Điểm mấu chốt nhất là quy trình phát hành và vận hành của đồng stablecoin HKD này hoàn toàn nằm ngoài tầm kiểm soát pháp lý của chính phủ Mỹ.

Nói cách khác, Hồng Kông đã kiến tạo nên một công cụ tài chính có giá trị neo theo USD nhưng hoàn toàn độc lập và không sợ các lệnh trừng phạt tài chính từ Mỹ. Chúng ta hoàn toàn có thể hình dung trong các kịch bản tương lai khi các giao dịch thương mại quốc tế gặp khó khăn khi thanh toán bằng USD truyền thống, các đối tác có thể chuyển sang sử dụng đồng stablecoin HKD này để thực hiện thanh toán một cách an toàn.

### (4) Liệu có thể có Stablecoin bảo chứng bằng Nhân dân tệ (RMB)?

Câu hỏi đặt ra là liệu có cơ hội ra đời đồng stablecoin bảo chứng bằng Nhân dân tệ hay không?

Như đã phân tích ở trên, đặc tính của stablecoin là cực kỳ khó quản lý dòng chảy và hỗ trợ tự do quy đổi sang ngoại tệ như USD. Do đó dưới chính sách kiểm soát ngoại hối nghiêm ngặt của Trung Quốc đại lục, tôi nhận định đồng stablecoin neo giá theo RMB nhiều khả năng sẽ không được phép ra đời.

## 科技动态

（1）Gã khổng lồ trong mảng cho thuê xe hơi của Mỹ Hertz vừa triển khai áp dụng hệ thống **máy quét kiểm tra xe hơi tự động bằng AI** (Vehicle Scanner).

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071408.webp)

Tại thời điểm khách hàng trả xe, hệ thống máy quét sẽ sử dụng dàn camera độ phân giải cao để chụp hàng nghìn bức ảnh chi tiết toàn bộ thân vỏ xe, sau đó dùng thuật toán AI đối chiếu tự động với dữ liệu ảnh chụp lúc nhận xe. Mọi vết xước hay móp méo mới phát sinh sẽ được phát hiện chính xác để yêu cầu bồi thường.

Giải pháp này không chỉ mang lại hiệu năng cao cho doanh nghiệp mà còn giảm thiểu tối đa các tranh cãi nhờ bằng chứng hình ảnh rõ ràng. Kể từ khi đưa vào vận hành, số tiền phạt thu về từ khách hàng của hãng đã tăng vọt lên gấp 6 lần so với trước đó.

（2）Một chi nhánh nhà hàng lẩu Haidilao tại Hợp Phì gây chú ý khi yêu cầu nhân viên phục vụ **đeo thẻ ngực in mã QR** khi bưng bê phục vụ món ăn.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071407.webp)

Ý tưởng ban đầu nhằm mục đích giúp khách hàng dễ dàng quét mã để thưởng tiền boa (tips) cho nhân viên phục vụ tốt. Tuy nhiên việc này vấp phải nhiều ý kiến trái chiều cho rằng đây là hành vi biến tướng đòi tiền boa gây khó chịu cho thực khách. Trước phản hồi của dư luận, nhà hàng đã quyết định tháo bỏ các thẻ QR này.

Tuy nhiên dưới góc nhìn cá nhân, tôi thấy giải pháp này không nên bị bãi bỏ mà nên được chuẩn hóa nhân rộng trong ngành dịch vụ với tên gọi "Mã nhân viên", bên cạnh việc thưởng tiền có thể tích hợp thêm tính năng để khách hàng quét phản ánh chất lượng phục vụ hoặc gửi lời khen ngợi trực tiếp.

（3）Câu chuyện hy hữu xảy ra tại Canada khi một ban nhạc mới mang tên Velvet Sundown bất ngờ xuất hiện và nhanh chóng lọt vào danh sách các ca khúc được nghe nhiều nhất trên Spotify.

Ban đầu không ai biết các thành viên ban nhạc là ai, hệ thống hoàn toàn sạch bóng các hình ảnh chân dung hay thông tin giới thiệu cá nhân, khiến dư luận nghi ngờ đây là một sản phẩm âm nhạc được tạo ra hoàn toàn bởi công nghệ AI.

Trước những hoài nghi, ban nhạc chọn giải pháp giữ im lặng. Cho đến một ngày, một người đàn ông tự nhận là đại diện truyền thông của ban nhạc đã đăng tải loạt ảnh chụp chân dung các thành viên lên mạng xã hội để chứng minh họ là người thật.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070703.webp)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070704.webp)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070705.webp)

Tuy nhiên các bức ảnh này ngay lập tức bị cư dân mạng bóc phốt là sản phẩm vẽ lỗi bằng AI, càng củng cố thêm nghi vấn ban đầu. Khi sự việc vỡ lở, ban nhạc buộc phải ra thông báo chính thức thừa nhận: Người tự nhận là đại diện truyền thông kia là giả mạo, các bức ảnh là do người hâm mộ tự chế, nhưng đồng thời cũng thừa nhận toàn bộ phần âm nhạc của họ thực tế đúng là do AI tự động sinh dựng.

Điều trớ trêu là sau vụ bê bối truyền thông này, mức độ nhận diện của ban nhạc lại càng tăng vọt và lượng người nghe nhạc của họ tiếp tục tăng trưởng mạnh. Chứng kiến hoạt động này chắc hẳn nhiều nhạc sĩ chân chính ngoài đời thực sẽ cảm thấy vô cùng nản lòng trước tương lai của âm nhạc truyền thống.

（4）Giám đốc phụ trách bộ phận Android của Google vừa tiết lộ thông tin về kế hoạch **sáp nhập hệ điều hành ChromeOS vào Android** trong tương lai.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071501.webp)

Chiến lược của Google nhằm đồng bộ hóa toàn diện các trải nghiệm phần mềm trên điện thoại, máy tính bảng và máy tính xách tay về một nền tảng chung. Trong tương lai, các dòng máy tính xách tay Android có thể chạy trực tiếp các ứng dụng di động một cách mượt mà.

（5）Mô hình AI Grok 4 mới được công ty X (Twitter) công bố tuần trước khiến người dùng bất ngờ khi phát hiện: Mỗi khi được hỏi về các tin tức thời sự nóng hổi, hệ thống sẽ tự động **quét và tham khảo quan điểm cá nhân của Elon Musk trước tiên** để làm căn cứ phản hồi (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071104.webp)

Các chuyên gia dự báo đây không phải là một thiết kế thiên vị được lập trình cố ý. Bản chất Grok được cấu hình để quét thông tin thời gian thực từ các bài đăng của người dùng trên nền tảng X, và do tài khoản của Elon Musk sở hữu lượng tương tác lớn nhất hệ thống nên thuật toán AI đã tự động ưu tiên quét tài khoản của ông trước.

Sự việc sau đó trở nên hài hước hơn khi để dập tắt các tranh cãi, đội ngũ kỹ thuật xAI đã [công khai cập nhật tài liệu prompt hệ thống](https://github.com/xai-org/grok-prompts/commit/e517db8b4b2539ea825bc4038917740e35bcaeba) bổ sung thêm điều khoản yêu cầu mô hình AI tuyệt đối không được tham khảo hay trích dẫn các bài đăng phát ngôn của Elon Musk khi trả lời.

## 文章

1、[Nhìn lại chặng đường lịch sử 20 năm ra đời của bộ khung Django](https://simonwillison.net/2025/Jul/13/django-birthday/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071410.webp)

Đánh dấu cột mốc tròn 20 năm phát triển của framework lập trình web Django nổi tiếng viết bằng Python. Nhà đồng sáng lập Simon Willison chia sẻ những câu chuyện hậu trường thú vị thuở sơ khai, bao gồm cả chi tiết ban đầu ông chỉ lên kế hoạch tìm kiếm một giải pháp viết bằng Python để thay thế cho ngôn ngữ PHP 4 thời kỳ đó.

2、[Hướng dẫn tự chế thiết bị điều khiển máy tính từ xa PiKVM bằng Raspberry Pi](https://www.xda-developers.com/built-pikvm-control-pc-remotely-game-changer/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070503.webp)

Để có khả năng kết nối điều khiển máy tính từ xa ở tầng phần cứng sâu (ngay từ màn hình khởi động BIOS), giải pháp tối ưu là sử dụng các thiết bị KVM chuyên dụng. Bài viết hướng dẫn chi tiết cách tận dụng chiếc máy tính nhúng Raspberry Pi để tự xây dựng hệ thống [PiKVM](https://pikvm.org/) tiện lợi với chi phí tiết kiệm.

3、[Đánh giá về thực trạng phát triển của ngôn ngữ Elm dưới kỷ nguyên hiện nay](https://engagesoftware.com/news/post/7033/using-elm-in-2025) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071502.webp)

Elm là một ngôn ngữ lập trình frontend có cấu trúc thiết kế rất độc đáo, tuy nhiên dự án đã không phát hành phiên bản cập nhật mới nào kể từ năm 2019. Bài phân tích chỉ ra Elm hoàn toàn chưa chết mà vẫn đang được ứng dụng ổn định nhờ cộng đồng nhà phát triển rất trung thành và hoạt động tích cực.

4、[Giới thiệu tính năng hàm điều kiện if() mới được bổ sung trong CSS](https://developer.chrome.com/blog/if-article?hl=zh-cn) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071712.webp)

Kể từ phiên bản Chrome 137, trình duyệt đã bắt đầu hỗ trợ cú pháp viết hàm điều kiện `if()` trực tiếp trong mã nguồn CSS. Ngôn ngữ CSS đang ngày một bổ sung thêm nhiều đặc tính lập trình của các ngôn ngữ lập trình thực thụ.

5、[Hướng dẫn các bước tự thiết lập các câu lệnh con tùy biến trong Git](https://github.com/shangwenhe/shangwenhe.github.io/issues/69) (tiếng Trung)

Bài viết hướng dẫn kỹ thuật giúp lập trình viên tự viết các script để bổ sung thêm các câu lệnh con cá nhân hóa (tiêu biểu như câu lệnh `git branch.note`) vào hệ thống Git để tối ưu hóa công việc. (Đóng góp từ [@shangwenhe](https://github.com/ruanyf/weekly/issues/7294))

6、[Tại sao bạn nên hạn chế sử dụng từ khóa continue trong các vòng lặp](https://www.teamten.com/lawrence/programming/avoid-continue.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025042501.webp)

Tác giả đưa ra các lập luận phân tích cho rằng việc lạm dụng từ khóa continue trong các cấu trúc vòng lặp là không thực sự cần thiết, gây đứt gãy mạch đọc logic của mã nguồn và khuyên các lập trình viên nên ưu tiên sử dụng các cấu trúc rẽ nhánh if/else để mã nguồn sáng sủa hơn.

## 工具

1、[Anytype](https://download.anytype.io/)

Phần mềm ghi chú cá nhân đa nền tảng mã nguồn mở được phát triển như một giải pháp thay thế chất lượng cho Obsidian, tích hợp sẵn các tính năng đồng bộ dữ liệu ngang hàng (P2P) bảo mật.

2、[Pangolin](https://github.com/fosrl/pangolin)

Dự án xây dựng máy chủ proxy ngược (Reverse Proxy) đi kèm giao diện quản trị Web trực quan giúp người dùng dễ dàng ánh xạ mở cổng các dịch vụ nội bộ ra ngoài internet, được phát triển như giải pháp thay thế mã nguồn mở cho Cloudflare Tunnel.

3、[Upyo](https://github.com/dahlia/upyo)

Thư viện JavaScript gọn nhẹ cung cấp đầy đủ các tính năng lập trình hỗ trợ gửi nhận thư điện tử email.

4、[OpenCut](https://github.com/OpenCut-app/OpenCut)

Dự án phần mềm biên tập video mã nguồn mở hoạt động ngay trên giao diện web, hướng tới mục tiêu xây dựng một giải pháp thay thế tự chủ cho ứng dụng CapCut.

5、[Tooboo](https://apps.apple.com/cn/app/id6736378337)

Ứng dụng bản đồ và dẫn đường dã ngoại dành cho các thiết bị Apple, hỗ trợ tải bản đồ ngoại tuyến, hiển thị đường đồng mức và bản đồ vệ tinh 3D, hỗ trợ tự động kết xuất video hành trình chuyển động thực tế (hoàn toàn miễn phí trên thiết bị di động). (Đóng góp từ [@haozes](https://github.com/ruanyf/weekly/issues/7258))

6、[TcpViz](https://github.com/ruanyf/weekly/issues/7260)

Dịch vụ web hỗ trợ phân tích và trực quan hóa các tệp tin gói tin mạng dạng pcap, giúp kỹ sư nhanh chóng kết xuất các báo cáo phân tích sự cố mạng chỉ với thao tác tải tệp tin đơn giản. (Đóng góp từ [@jlingjace](https://github.com/ruanyf/weekly/issues/7260))

7、[WebCurl](https://github.com/o8oo8o/WebCurl)

Công cụ kiểm thử kết nối API hoạt động ngay trên trình duyệt web tối giản với cấu trúc mã nguồn chỉ gồm duy nhất một tệp tin HTML đơn lẻ, được phát triển thay thế cho Postman. (Đóng góp từ [@o8oo8o](https://github.com/ruanyf/weekly/issues/7254))

8、[HubProxy](https://github.com/sky22333/hubproxy)

Dự án mã nguồn mở phát triển trên Go cho phép người dùng tự dựng máy chủ trung gian để tăng tốc độ tải dữ liệu từ các kho chứa Docker Hub và GitHub. (Đóng góp từ [@sky22333](https://github.com/ruanyf/weekly/issues/7278))

9、[Trình quản lý tệp tin cấu hình (配置文件管理器)](https://github.com/HeroIsUseless/configeditor)

Ứng dụng máy tính đa nền tảng hỗ trợ kỹ sư kết nối chỉnh sửa nhanh các tệp tin cấu hình hệ thống cục bộ hoặc từ xa, hỗ trợ tự động lưu và khởi động lại các dịch vụ liên quan sau khi chỉnh sửa. (Đóng góp từ [@HeroIsUseless](https://github.com/ruanyf/weekly/issues/7257))

Tham khảo thêm một công cụ tương tự dành riêng cho macOS mang tên [Configs](https://github.com/iHongRen/configEditor) có khả năng tự động quét phát hiện các tệp cấu hình trên máy. (Đóng góp từ [@iHongRen](https://github.com/ruanyf/weekly/issues/7270))

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071607.webp)

10、[MeetSpot](https://github.com/JasonRobertDestiny/MeetSpot)

Ứng dụng bản đồ mã nguồn mở độc đáo: Người dùng nhập vào địa điểm xuất phát của các thành viên tham gia cuộc hẹn, hệ thống sẽ tự động tính toán và gợi ý địa điểm tụ họp phù hợp nhất (quán cà phê, nhà hàng...) giúp tối thiểu hóa quãng đường di chuyển chung cho cả nhóm. (Đóng góp từ [@JasonRobertDestiny](https://github.com/ruanyf/weekly/issues/7289))

11、[Hảo Hưởng Ký Chướng (好享记账)](https://github.com/suyu610/journal-flutter)

Dự án sổ tay ghi chép chi tiêu cá nhân mã nguồn mở, liên kết trên dẫn tới kho chứa mã nguồn frontend viết bằng Flutter, tham khảo thêm [kho chứa mã nguồn backend viết bằng Java](https://github.com/suyu610/journal-server). (Đóng góp từ [@suyu610](https://github.com/ruanyf/weekly/issues/7293))

## AI 相关

1、[EPUB Translator](https://github.com/oomol-lab/epub-translator)

Thư viện Python tích hợp AI hỗ trợ người dùng tự động dịch thuật các cuốn sách điện tử định dạng EPUB sang phiên bản song ngữ nhanh chóng. (Đóng góp từ [@BlackHole1](https://github.com/ruanyf/weekly/issues/7273))

2、[PoPo](https://github.com/AmyangXYZ/PoPo)

Dự án mã nguồn mở thú vị cho phép người dùng nhập các khẩu lệnh bằng ngôn ngữ tự nhiên (như "cúi người", "cười lớn"...) để điều khiển các chuyển động cơ thể của một mô hình nhân vật 3D trên trang web, trải nghiệm trực tuyến tại [popo.love](https://popo.love/). (Đóng góp từ [@AmyangXYZ](https://github.com/ruanyf/weekly/issues/7268))

## 资源

1、[Công cụ tổng hợp tin tức tự động Kite](https://kite.kagi.com/)

Trang web tổng hợp tin tức do công cụ tìm kiếm Kagi công bố vận hành hoàn toàn tự động bằng AI: Hệ thống tự động chọn lọc tin tức nóng hổi, tiến hành tóm tắt nội dung cốt lõi và tự động chuyển dịch sang ngôn ngữ hiển thị do người đọc cấu hình.

2、[Tài liệu hướng dẫn học lập trình ngôn ngữ lắp ráp x86-64 cho người mới](https://gpfault.net/posts/asm-tut-0.txt.html) (tiếng Anh)

Bộ tài liệu hướng dẫn học assembly cơ bản từ con số không, giải thích cặn kẽ về cấu trúc bộ nhớ và các thanh ghi của máy tính. Liên kết trên dẫn tới bài học đầu tiên, tham khảo tiếp các bài học [Phần 2](https://gpfault.net/posts/asm-tut-1.txt.html), [Phần 3](https://gpfault.net/posts/asm-tut-2.txt.html) và [Phần 4](https://gpfault.net/posts/asm-tut-3.txt.html).

3、[Giải nghĩa chi tiết toàn bộ các mã trạng thái HTTP (HTTP Status Codes)](https://evertpot.com/http/) (tiếng Anh)

Chuỗi bài viết chuyên sâu giải thích cặn kẽ ý nghĩa kỹ thuật và kịch bản ứng dụng của toàn bộ 68 mã trạng thái HTTP chuẩn quốc tế.

## 图片

1、[Tác phẩm điện ảnh Hollywood được quay hoàn toàn bằng điện thoại iPhone](https://www.indiewire.com/features/craft/28-years-later-iphone-hollywood-movie-1235134798/)

Bộ phim điện ảnh về đề tài zombie mới ra mắt của Mỹ mang tên "28 năm sau" (28 Years Later) được tiết lộ đã được bấm máy quay hoàn toàn bằng các thiết bị điện thoại iPhone 15 Pro Max.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071603.webp)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071604.webp)

Hình ảnh phía trên minh họa hệ thống giàn quay tích hợp cùng lúc 20 chiếc iPhone để thực hiện các cảnh quay đa góc độ đồng thời.

Đạo diễn chia sẻ quyết định lựa chọn iPhone nhằm mục đích thử nghiệm các góc quay mới lạ nhờ kích thước nhỏ gọn của điện thoại cho phép dễ dàng gắn trực tiếp lên cơ thể của diễn viên khi thực hiện các cảnh hành động.

Tất nhiên để bảo đảm chất lượng hình ảnh chiếu rạp tốt nhất, quá trình quay phim vẫn đòi hỏi sự hỗ trợ của rất nhiều thiết bị phụ trợ chuyên nghiệp như các ống kính điện ảnh gắn ngoài và cụm gimbal chống rung chuyên dụng.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071605.webp)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071606.webp)

2、[Mẫu thiết kế mô hình giải phẫu người gỗ Lego](https://kottke.org//12/06/cool-anatomical-sculptures-of-lego-people)

Một nghệ sĩ người Mỹ chia sẻ tác phẩm cải tạo các nhân vật đồ chơi Lego thông thường thành những mô hình giải phẫu cơ thể người độc đáo.

Dưới đây là hình ảnh nhân vật Lego tiêu chuẩn quen thuộc:

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071602.webp)

Và đây là hình ảnh nhân vật sau khi được nghệ sĩ chạm khắc bổ sung cấu trúc xương và các cơ quan nội tạng giải phẫu bên trong:

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071405.webp)

Sự sáng tạo tỉ mỉ này đã biến những món đồ chơi nhựa thông thường thành những tác phẩm nghệ thuật trưng bày rất ấn tượng.

## 文摘

1、**Bài học về tầm quan trọng của số lượng so với chất lượng**

*Trích dịch câu chuyện từ bài phân tích của tác giả:*

Vào đầu học kỳ, vị giáo sư phụ trách lớp học nghệ thuật nhiếp ảnh tại Đại học Florida đã quyết định phân chia các sinh viên trong lớp thành hai nhóm học tập độc lập để áp dụng cơ chế chấm điểm khác nhau.

*   **Nhóm 1 được đặt tên là "Nhóm Số Lượng"**: Điểm số cuối kỳ của sinh viên nhóm này sẽ được chấm hoàn toàn dựa trên số lượng tác phẩm ảnh họ nộp về. Sinh viên chụp và nộp đủ 100 bức ảnh đạt chuẩn sẽ nhận điểm A, nộp 90 bức nhận điểm B, 80 bức nhận điểm C...
*   **Nhóm 2 được đặt tên là "Nhóm Chất Lượng"**: Sinh viên nhóm này trong cả học kỳ chỉ cần nộp duy nhất một bức ảnh, và điểm số cuối kỳ của họ sẽ phụ thuộc hoàn toàn vào mức độ hoàn mỹ của bức ảnh duy nhất đó.

Nếu là một sinh viên đăng ký lớp học này, bạn sẽ ưu tiên lựa chọn tham gia vào nhóm nào?

Kết quả bất ngờ vào cuối học kỳ được vị giáo sư ghi nhận: Toàn bộ các bức ảnh xuất sắc và nghệ thuật nhất của lớp học đều đến từ các sinh viên thuộc "Nhóm Số Lượng".

Nguyên nhân do yêu cầu bắt buộc phải nộp đủ số lượng lớn tác phẩm đã thôi thúc các sinh viên nhóm 1 phải liên tục xách máy lên đi chụp hằng ngày. Quy trình thực hành liên tục giúp họ dần làm quen và chấp nhận những lỗi sai nhỏ, rút kinh nghiệm qua từng lần bấm máy và nâng cao tay nghề một cách tự nhiên. Bức ảnh hoàn mỹ cuối cùng của họ được sinh ra một cách tất yếu từ chính quá trình tích lũy hàng trăm lần bấm máy chưa hoàn hảo trước đó.

Thử phân tích xem con số 100 lần bấm máy mang lại những giá trị gì: Đó là 100 cuộc đối thoại thực tế với ánh sáng, 100 cơ hội thử nghiệm bố cục khung hình, 100 lần tự soi xét đánh giá sai lệch giữa ý đồ nghệ thuật trong tâm trí với kết quả ảnh thực tế thu về để tự điều chỉnh ở các lần chụp sau.

Ngược lại, các sinh viên thuộc "Nhóm Chất Lượng" do áp lực bắt buộc phải tạo ra tác phẩm hoàn hảo duy nhất đã dành phần lớn thời gian học kỳ để ngồi nghiên cứu các lý thuyết nhiếp ảnh phức tạp, tìm hiểu cách thức căn chỉnh bố cục lý tưởng và học các mẹo kỹ thuật chụp tối ưu trên giấy. Họ tích lũy được một kho kiến thức lý thuyết nhiếp ảnh đồ sộ nhưng lại hoàn toàn thiếu đi cảm giác nhạy bén và trực giác nghệ thuật vốn chỉ có thể được rèn luyện thông qua hành động nhấn nút chụp lặp đi lặp lại ngoài thực địa.

Việc này tương tự như việc sinh viên nhóm chất lượng là những chuyên gia nghiên cứu bản đồ, còn sinh viên nhóm số lượng là những nhà thám hiểm thực thụ. Kết thúc khóa học, nhóm chất lượng có thể viết những bài phân tích rất hay giải thích tại sao một bức ảnh là đẹp, còn nhóm số lượng lại trực tiếp chụp ra được những bức ảnh đẹp đó.

## 言论

1、

Trong suốt nhiều năm trời, bạn đã dành vô vàn tâm huyết học tập để trở thành một lập trình viên chuyên nghiệp. Kỹ năng viết code đã trở thành một phần cốt lõi định hình nên danh tính cá nhân và là nguồn sống tạo nên giá trị sống của bạn. Rồi đột nhiên các công cụ AI xuất hiện và dễ dàng làm thay thế hầu hết các kỹ năng đó, khiến cảm giác về giá trị cá nhân của bạn bị lung lay dữ dội. Đây chính là nguyên nhân sâu xa giải thích tại sao nhiều lập trình viên kỳ cựu lại tỏ ra bài xích và phản đối AI dữ dội đến vậy.

-- *Trích bài viết 《Khi AI có khả năng lập trình, lập trình viên còn lại giá trị gì?》*

2、

Bài toán quy hoạch của thành phố Los Angeles nằm ở diện tích quá rộng lớn và phân tán, đi kèm hệ thống giao thông công cộng yếu kém buộc mọi người phải di chuyển bằng xe hơi riêng. Thực trạng này vô tình triệt tiêu cơ hội để bạn tình cờ gặp gỡ những con người thú vị trên đường phố, bởi tất cả mọi người đều đang bị cô lập bên trong chiếc hộp xe hơi của mình.

-- *Chia sẻ của một độc giả trên diễn đàn Hacker News*

3、

Hệ thống AI không hề thiếu vắng tri thức, điểm hạn chế lớn nhất của nó nằm ở việc hoàn toàn không biết hoài nghi trước những tri thức sẵn có.

Để một mô hình AI có thể đạt tới tầm vóc phát kiến vĩ đại của nhà bác học Albert Einstein, việc trang bị cho nó kho tri thức vạn vật là chưa đủ. Yêu cầu cốt lõi là phải rèn luyện cho AI năng lực tự đặt ra những câu hỏi phản biện độc đáo mà trước đó chưa có ai từng nghĩ tới hoặc không ai dám đặt câu hỏi nghi vấn.

-- *Thomas Wolf, nhà đồng sáng lập Hugging Face chia sẻ*

4、

Báo *New York Times* đưa tin các nhà tuyển dụng hiện nay đang bị nhấn chìm hoàn toàn trong làn sóng các hồ sơ xin việc (resumes) do AI tự động sinh ra. Theo thống kê của các trang tuyển dụng lớn, số lượng hồ sơ nộp về trong năm nay ghi nhận mức tăng vọt kỷ lục tới 45% so với năm trước.

Sự bùng nổ của AI có thể sẽ khai tử hoàn toàn vai trò của các bản CV truyền thống, bởi các tài liệu do AI tự tạo ra đã không còn khả năng giúp nhà tuyển dụng định vị hay đánh giá năng lực thực tế của ứng viên nữa. Quy trình tuyển dụng tương lai bắt buộc phải chuyển dịch sang các hình thức đánh giá trực tiếp mà AI không thể can thiệp được (như yêu cầu ứng viên giải quyết trực tiếp các bài toán kỹ thuật tại chỗ).

-- *Trích bài viết 《AI đang khai tử các bản CV xin việc truyền thống》*

5、

Nếu bạn lên kế hoạch biến sở thích cá nhân thành một nghề nghiệp kiếm sống chính thức để nuôi bản thân, sau khi giai đoạn hào hứng ban đầu đi qua, bạn sẽ nhanh chóng nhận ra những hào hứng thuở sơ khai đó thực chất chưa là gì cả. Khó khăn thực sự nằm ở chặng đường phía sau, khi vô vàn các đầu việc tẻ nhạt, vụn vặt và lặp đi lặp lại hằng ngày đang kiên nhẫn chờ đợi bạn xử lý.

Thời điểm này được giới tâm lý học gọi là "Điểm từ bỏ" (Quitting Point) — cột mốc thử thách mà phần lớn mọi người sẽ quyết định dừng cuộc chơi.

Mỗi người trong chúng ta đều sở hữu những cột mốc điểm từ bỏ khác nhau, nhưng nó chắc chắn sẽ tìm đến. Đối với một nhà văn, điểm từ bỏ có thể xuất hiện khi họ viết đến trang thứ 30 của cuốn tiểu thuyết, khi nguồn cảm hứng thăng hoa ban đầu cạn kiệt và họ hoàn toàn bế tắc không biết triển khai nội dung tiếp theo ra sao. Đối với một nhà khởi nghiệp, điểm từ bỏ xuất hiện sau vài tháng đầu tiên vận hành sản phẩm, khi phản hồi của thị trường lạnh nhạt hơn nhiều so với những lời khen ngợi ban đầu của người thân và bạn bè. Đối với một nghệ sĩ, điểm từ bỏ xuất hiện khi họ lần đầu tiên trưng bày tác phẩm của mình và đau đớn nhận ra khoảng cách mênh mông giữa ý tưởng sáng tạo trong tâm trí với năng lực thực tế của bản thân.

-- *Trích bài phân tích 《Sự kỳ vọng quá cao thực chất là một hình thức tự hủy hoại bản thân tinh vi》*

## 往年回顾

- Số #310: [Tìm hiểu các chiêu trò kiếm tiền trực tuyến của các trang trại nội dung (Content Farms) ứng dụng AI](https://www.ruanyifeng.com/blog/2024/07/weekly-issue-310.html)
- Số #260: [Chiêm nghiệm cuộc sống: Hành trình khởi nghiệp phát triển bản thân của bạn sẽ không bao giờ dừng lại ở Ngày đầu tiên](https://www.ruanyifeng.com/blog/2023/06/weekly-issue-260.html)
- Số #210: [Phân tích các nguyên nhân kỹ thuật khiến hệ thống phần mềm ngày một trở nên phức tạp và phình to](https://www.ruanyifeng.com/blog/2022/06/weekly-issue-210.html)
- Số #160: [Thảo luận về những khó khăn và lối thoát sự nghiệp của các lập trình viên bước vào tuổi trung niên](https://www.ruanyifeng.com/blog/2021/05/weekly-issue-160.html)

(Hết)
