# Bản tin chia sẻ công nghệ (Số 270): "Tinh gọn" trong "Phát triển tinh gọn" thực chất là gì?

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3425) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090607.webp)

Khu phức hợp thương mại Hymalaya Chứng Đại Nam Kinh là một dự án bất động sản được khánh thành vào năm 2020. Để làm nổi bật triết lý南京 là một “đô thị sơn thủy”, các kiến trúc sư đã thiết kế lớp vỏ ngoài của các tòa nhà uốn lượn nhấp nhô mô phỏng hình ảnh những dãy núi hùng vĩ bên dòng nước chảy. (Nguồn: [Sohu](https://www.sohu.com/a/460052910_791225))

## “精益开发”的精益是什么？

Mô hình phát triển phần mềm được áp dụng phổ biến nhất hiện nay chắc chắn là “Phát triển linh hoạt” (Agile Development).

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090201.webp)

Tuy nhiên, có một thực tế là **Agile thực chất chỉ là một hệ giá trị triết lý định hướng, chứ không phải là một phương pháp làm việc cụ thể.** Để hiện thực hóa các nguyên lý của Agile trong thực tế, cộng đồng công nghệ đã phát triển nhiều phương pháp luận quản trị dự án khác nhau, tiêu biểu bao gồm:

* Lập trình cực hạn (XP - Extreme Programming)
* Quy trình Scrum
* Phương pháp Kanban (Bảng Kanban)
* Phát triển tinh gọn (Lean Software Development)

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023082803.webp)

Đối với các lập trình viên mới vào nghề, việc tiếp cận hàng loạt thuật ngữ chuyên ngành này rất dễ gây hoang mang: chúng thực chất có ý nghĩa gì và có liên quan gì đến công việc viết mã hàng ngày?

Vừa qua tôi có đọc được một [bài viết rất hay](https://elijahpotter.dev/articles/on_iteration_and_lean_thinking) chia sẻ các câu chuyện lịch sử thú vị xoay quanh sự ra đời của phương pháp phát triển tinh gọn. Bài viết đã giúp tôi thấu hiểu cặn kẽ nguồn gốc của khái niệm “tinh gọn” và cách thức vận hành thực tế của nó. Xin được tóm tắt chia sẻ lại cùng bạn đọc.

Thuật ngữ “Tinh gọn” (tiếng Anh: *lean*) bắt đầu được biết đến rộng rãi sau khi bài nghiên cứu khoa học mang tên **《Chiến thắng của Hệ thống Sản xuất Tinh gọn》** được xuất bản vào năm 1988. Bài báo tập trung lý giải nguyên nhân sâu xa giúp các hãng sản xuất ô tô Nhật Bản đánh bại hoàn toàn các ông lớn ô tô của Mỹ trên sân nhà.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090202.webp)

Tác giả bài báo đã thực hiện phân tích đối chiếu quy trình sản xuất của hai đại diện tiêu biểu là Ford (Mỹ) và Toyota (Nhật Bản), qua đó chỉ ra hai doanh nghiệp áp dụng hai triết lý sản xuất hoàn toàn trái ngược nhau.

Ford là ông vua không ngai thống trị ngành ô tô thế giới thời kỳ đầu nhờ tiên phong áp dụng mô hình sản xuất hàng loạt (mass production) trên dây chuyền tự động, hướng tới tối ưu hóa tối đa năng suất để hạ giá thành sản phẩm. Thời điểm đó, khi mặt bằng giá ô tô trên thị trường dao động khoảng 3.000 USD/chiếc, dòng xe Ford Model T ra mắt với mức giá gây sốc chỉ 850 USD, và sau đó tiếp tục giảm sâu xuống mức 260 USD, giúp Ford nhanh chóng thâu tóm phần lớn thị phần ô tô tại Mỹ.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090203.webp)

Trong dân gian vẫn lưu truyền câu nói nổi tiếng của nhà sáng lập Henry Ford: *“Khách hàng có thể thoải mái lựa chọn bất kỳ màu sơn nào họ thích, miễn là nó màu đen”*. Thực tế, việc dòng xe Model T chỉ có duy nhất lựa chọn màu đen không phải do sở thích cá nhân của Henry Ford, mà bởi vì sơn màu đen có tốc độ khô nhanh nhất trên dây chuyền, giúp xe nhanh chóng xuất xưởng và giảm tối đa chi phí lưu kho.

Để duy trì mức giá bán siêu rẻ, quy trình sản xuất hàng loạt của Ford được vận hành theo các bước sau:

1. Thu mua nguyên vật liệu quy mô lớn đủ để sản xuất 100 chiếc xe.
2. Tiến hành sản xuất đồng loạt toàn bộ các linh kiện cần thiết cho 100 chiếc xe (với tổng số lượng lên tới hơn 10 vạn chi tiết máy).
3. Thực hiện lắp ráp hoàn thiện 100 chiếc xe và xuất xưởng bán ra thị trường.
4. Thu nhận phản hồi của khách hàng để điều chỉnh thiết kế cho các lô sản xuất tiếp theo.

Do mỗi công đoạn sản xuất hàng loạt đều tiêu tốn khoảng thời gian rất dài, chu kỳ lặp lại (iteration) của quy trình diễn ra rất chậm. Đó là lý do Ford rất ít khi thay đổi hay nâng cấp thiết kế các mẫu xe của mình qua các năm.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090204.webp)

Ở bên kia đại dương, hãng xe Toyota lại lựa chọn một phương thức sản xuất hoàn toàn khác. Thời kỳ đầu mới thành lập, Toyota chỉ là một xưởng sản xuất nhỏ, không có đủ tiềm lực tài chính để thu mua tích trữ lượng lớn nguyên vật liệu, cũng không đủ ngân sách để mua sắm các máy móc chuyên dụng cho từng loại chi tiết máy. Họ bắt buộc phải sử dụng các máy móc đa năng – tức là cùng một chiếc máy sẽ được tinh chỉnh để sản xuất nhiều loại linh kiện khác nhau tùy theo thời điểm.

Do đó, **họ lựa chọn giải pháp sản xuất cuốn chiếu: tập trung sản xuất hoàn thiện và bán nhanh từng chiếc xe một**. Quy trình này giúp họ lập tức phát hiện các lỗi phát sinh trên chiếc xe vừa hoàn thành để sửa đổi ngay trong dây chuyền, ngăn chặn việc tiếp tục sản xuất ra những chiếc xe bị lỗi tiếp theo:

1. Thu mua lượng nguyên vật liệu vừa đủ để sản xuất 1 chiếc xe.
2. Sản xuất các linh kiện cần thiết cho đúng 1 chiếc xe đó.
3. Lắp ráp hoàn thiện chiếc xe và lập tức bán ra thị trường.
4. Thu nhận nhanh phản hồi của khách hàng để áp dụng cải tiến ngay cho chiếc xe tiếp theo trên dây chuyền.

Quy trình cuốn chiếu này tạo điều kiện cho Toyota thực hiện liên tục các chu kỳ cải tiến nhỏ với tốc độ rất nhanh. Trải qua thời gian dài tích lũy, các dòng xe của Toyota dần đạt độ bền bỉ, tính ổn định cao và đáp ứng sát thực tế nhu cầu sử dụng của khách hàng.

Mặc dù xét trên chi phí sản xuất của từng chiếc xe đơn lẻ, phương pháp của Toyota có giá thành cao hơn so với mô hình sản xuất hàng loạt của Ford; tuy nhiên do chu kỳ cải tiến của Ford quá chậm, khi một linh kiện thiết kế bị lỗi, Ford vô tình đã sản xuất hàng vạn linh kiện lỗi đó trước khi phát hiện ra, gây nên sự lãng phí tài nguyên khổng lồ. Xét trên hiệu quả kinh tế tổng thể, Toyota lại đạt hiệu suất cao hơn.

Phương thức sản xuất cuốn chiếu tối ưu hóa quy trình của Toyota được giới quản trị đặt tên là “Phương pháp tinh gọn” (Lean Method). Từ *lean* trong tiếng Anh mang nghĩa gốc là “thon gọn, săn chắc và khỏe mạnh”, ẩn dụ cho một hệ thống vận hành linh hoạt, phản ứng nhanh nhạy và loại bỏ hoàn toàn các công đoạn dư thừa gây lãng phí.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090205.webp)

Về sau, triết lý quản trị này đã được nhân rộng sang nhiều lĩnh vực khác nhau: trong quản trị doanh nghiệp gọi là “Tư duy tinh gọn” (Lean Thinking), trong công nghiệp gọi là “Sản xuất tinh gọn” (Lean Manufacturing) và trong phát triển công nghệ gọi là “Phát triển phần mềm tinh gọn” (Lean Software Development).

Tựu trung lại, triết lý của “Phát triển tinh gọn” trong lập trình là: **tập trung xây dựng một phiên bản sản phẩm khả dụng tối thiểu (MVP) nhanh nhất có thể để bàn giao cho người dùng trải nghiệm, quan sát hành vi sử dụng thực tế của họ, từ đó liên tục thực hiện các cải tiến nhỏ để nâng cấp sản phẩm ở các phiên bản tiếp theo.** Phương pháp này giúp sản phẩm luôn bám sát sự thay đổi của thị trường và tránh lãng phí nguồn lực lập trình những tính năng phức tạp không ai dùng đến.

Ngược lại, phương pháp kiểu Ford truyền thống (Waterfall) yêu cầu lập kế hoạch chi tiết toàn bộ các tính năng ngay từ đầu, tập trung nguồn lực lập trình hoàn thiện tất cả rồi mới bàn giao sản phẩm một lần duy nhất cho khách hàng.

## 科技动态

1、[Trang tin công nghệ Gizmodo thử nghiệm thay thế đội ngũ biên dịch viên bằng AI](https://www.theverge.com/2023/9/1/23856029/gizmodo-shuts-down-spanish-language-site-ai-translations)

Trang tin tức công nghệ lâu đời Gizmodo vừa qua đã công bố quyết định sa thải toàn bộ đội ngũ biên dịch viên của phiên bản tiếng Tây Ban Nha, chuyển dịch toàn bộ quy trình dịch thuật nội dung sang hệ thống tự động ứng dụng trí tuệ nhân tạo:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090101.webp)

Dưới chân các bài viết thuộc phiên bản tiếng Tây Ban Nha hiện hiển thị dòng thông báo miễn trách nhiệm: *“Nội dung của bài viết này được dịch tự động bằng phần mềm dịch thuật AI, có thể xuất hiện một số sai lệch nhỏ so với văn bản gốc.”*

Trước đó, Gizmodo cũng từng thử nghiệm sử dụng AI để tự động viết các bài đưa tin ngắn: chỉ cần cung cấp các số liệu và sự kiện cơ bản, AI sẽ tự động biên soạn thành một bài viết hoàn chỉnh. Xu hướng ứng dụng AI này dự kiến sẽ sớm phổ biến trong ngành báo chí, trong đó các vị trí dịch thuật và biên tập viên tin tức ngắn sẽ là nhóm nhân sự đầu tiên đối mặt với nguy cơ bị thay thế.

2、[Cơn sốt trí tuệ nhân tạo mang lại nguồn doanh thu khổng lồ cho một đảo quốc nhỏ nhờ tên miền .ai](https://arstechnica.com/information-technology/2023/08/ai-fever-turns-anguillas-ai-domain-into-a-digital-gold-mine/)

Tên miền quốc gia cao cấp `.ai` vốn thuộc quyền quản lý của Anguilla – một hòn đảo nhỏ thuộc lãnh thổ hải ngoại của Vương quốc Anh nằm tại vùng biển Caribbean, sở hữu diện tích đất liền chỉ tương đương đảo Hong Kong:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090102.webp)

Sự bùng nổ toàn cầu của làn sóng công nghệ AI đã khiến nhu cầu đăng ký tên miền `.ai` của các startup công nghệ tăng vọt, mang lại nguồn thu khổng lồ cho chính quyền đảo quốc này. Mức phí đăng ký và duy trì tên miền `.ai` hiện dao động quanh mức 80 USD/năm (khoảng 1,9 triệu đồng) và vẫn có xu hướng tiếp tục tăng cao:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090103.webp)

Vào năm 2021, doanh thu từ đăng ký tên miền mang về cho hòn đảo 7,4 triệu USD. Sau sự xuất hiện của ChatGPT, doanh thu dự kiến trong năm nay của hòn đảo từ nguồn này ước tính đạt 30 triệu USD – chiếm tới 10% tổng GDP của toàn bộ đảo quốc.

Với dân số trên đảo chỉ khoảng 15.000 người, nguồn thu từ tên miền tương đương với việc mỗi người dân trên đảo nhận được khoản phân chia gián tiếp 2.000 USD/năm, một nguồn tài lộc bất ngờ từ trên trời rơi xuống nhờ làn sóng công nghệ.

3、[Sản phẩm gọi vốn cộng đồng bắt đầu giao hàng tới tay người dùng sau 10 năm trì hoãn](https://www.tomshardware.com/news/oscilloscope-watch-ships-after-10-years)

Cách đây một thập kỷ, mô hình gọi vốn cộng đồng (Crowdfunding) là phương thức ra mắt sản phẩm vô cùng thịnh hành. Các nhà sáng chế thu hút vốn từ cộng đồng mạng để đưa sản phẩm vào sản xuất thực tế và cam kết gửi sản phẩm hoàn thiện tới những người đóng góp vốn sau đó.

Tuy nhiên, có không ít dự án đã biến mất không dấu vết sau khi nhận tiền, hoặc mất rất nhiều năm mới có thể bàn giao sản phẩm. Mới đây, một dự án đồng hồ đeo tay gọi vốn từ 10 năm trước đã chính thức bắt đầu giao hàng:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090501.webp)

Đây là mẫu đồng hồ đeo tay được tích hợp tính năng máy hiện sóng (Oscilloscope Watch) độc đáo, thực hiện gọi vốn từ năm 2013 và sau đó hoàn toàn im hơi lặng tiếng. Cho đến khi hầu hết người dùng đóng góp vốn đã quên đi sự tồn tại của dự án, nhà phát triển bất ngờ thông báo bắt đầu giao sản phẩm từ ngày 30 tháng 7 năm nay:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090502.webp)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090503.webp)

Người dùng nhận về một thiết bị điện tử có cấu trúc linh kiện lỗi thời của 10 năm trước nhưng hoàn toàn không thể yêu cầu hoàn tiền hay đổi trả. Sàn gọi vốn Kickstarter quy định rất rõ ràng: việc đóng góp vốn mang bản chất là hoạt động đầu tư rủi ro hỗ trợ dự án phát triển chứ không phải là hành vi mua sắm thương mại thông thường tại cửa hàng.

4、[Apple đăng ký bằng sáng chế công nghệ kính chắn gió AR tích hợp tính năng dịch thuật thời gian thực](https://www.thedrive.com/news/apple-wants-to-patent-an-augmented-reality-windshield)

Apple mới đây đã nộp đơn đăng ký bằng sáng chế cho hệ thống kính chắn gió tích hợp công nghệ hiển thị thực tế tăng cường (AR) dành cho xe hơi thông minh:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090106.webp)

Khác với các công nghệ hiển thị HUD dạng chiếu ảnh thông thường, bằng sáng chế của Apple mô tả bản thân tấm kính chắn gió là một màn hình hiển thị trong suốt đặc biệt, cho phép hiển thị các thông tin hành trình, bản đồ dẫn đường và cảnh báo an toàn trực tiếp trên kính.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090608.webp)

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090609.webp)

Ý tưởng thiết kế độc đáo nhất là tính năng dịch thuật thời gian thực: khi xe di chuyển tại nước ngoài, hệ thống camera sẽ nhận diện các biển hiệu, biển báo giao thông bằng tiếng nước ngoài dọc đường và tự động hiển thị dòng chữ dịch đè lên vị trí biển báo đó trên kính chắn gió để tài xế dễ dàng quan sát (hình minh họa trên).

## Bài viết

1\. [Ông Nhậm Chính Phi chia sẻ về chiến lược thu hút và sử dụng nhân tài công nghệ của Huawei](https://www.bjnews.com.cn/detail/1693810149129843.html)（Tiếng Trung）

Huawei đã công bố bài phát biểu mới nhất của nhà sáng lập Nhậm Chính Phi tại cuộc họp nội bộ của nhóm công tác tuyển dụng và sử dụng nhân tài công nghệ cao cấp của tập đoàn. Bài phát biểu phác họa rõ nét quan điểm của hãng về việc xác định ranh giới nghiên cứu công nghệ cốt lõi và phương pháp trao quyền chủ động cho các nhà khoa học trẻ.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090402.webp)

2\. [Chia sẻ chặng đường tự học lập trình từ con số không trở thành kỹ sư phần mềm chuyên nghiệp](https://www.zhihu.com/question/614706706/answer/3146012068)（Tiếng Trung）

Một bài chia sẻ thu hút nhiều lượt tương tác trên Zhihu, ghi lại chi tiết lộ trình học tập, rèn luyện kỹ năng viết mã và tìm kiếm cơ hội thực tập thực tế trong suốt 4 năm học đại học của một sinh viên từ chỗ hoàn toàn chưa biết gì về code đã tự học thành công để trở thành kỹ sư phần mềm. (Đóng góp của [@wind-liang](https://github.com/ruanyf/weekly/issues/3439))

3\. [Hướng dẫn cấu hình sử dụng công cụ quản lý mật khẩu iCloud trên trình duyệt Chrome](https://www.kocpc.com.tw/archives/508132)（Chữ Phồn thể）

Hệ thống quản lý mật khẩu mặc định iCloud Keychain của Apple trước đây chủ yếu chỉ hỗ trợ cho trình duyệt Safari. Sau khi ra mắt extension hỗ trợ cho Chrome trên Windows, hiện tại Apple đã chính thức hỗ trợ tiện ích này hoạt động mượt mà trên trình duyệt Chrome và Edge chạy trên hệ điều hành macOS.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023083109.webp)

4\. [Hướng dẫn các kỹ thuật cơ bản để tự xây dựng một Front-end Framework tối giản](https://18alan.space/posts/how-hard-is-it-to-build-a-frontend-framework.html)（Tiếng Anh）

Bài viết kỹ thuật hướng dẫn chi tiết hai kỹ thuật lập trình cốt lõi (xây dựng Virtual DOM tối giản và thiết lập cơ chế phản ứng dữ liệu reactive) giúp các lập trình viên Front-end thấu hiểu nguyên lý hoạt động của các thư viện lớn bằng cách tự tay lập trình xây dựng một mini framework của riêng mình.

![](https://cdn.beekka.com/blogimg/asset/202305/bg2023051502.webp)

5\. [Wikimedia chính thức giới thiệu dịch vụ phân giải tên miền Wikimedia DNS riêng](https://meta.wikimedia.org/wiki/Wikimedia_DNS)（Tiếng Anh）

Tổ chức Wikimedia (đơn vị vận hành bách khoa toàn thư Wikipedia) công bố triển khai dịch vụ phân giải tên miền miễn phí riêng mang tên Wikimedia DNS, hỗ trợ toàn diện các chuẩn truy vấn mã hóa an toàn DoH (DNS-over-HTTPS) và DoT (DNS-over-TLS) nhằm bảo vệ quyền riêng tư cho người dùng tránh bị theo dõi lịch sử duyệt web.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090704.webp)

6\. [Hướng dẫn các phương pháp tắt cưỡng bức một phiên làm việc bị treo trên Linux](https://linuxiac.com/how-to-terminate-user-session-in-linux/)（Tiếng Anh）

Trong quá trình quản trị hệ thống qua dòng lệnh Linux, kỹ sư thường gặp tình huống phiên kết nối terminal bị đóng băng, mất phản hồi. Bài viết hướng dẫn các câu lệnh dòng lệnh giúp người quản trị xác định nhanh ID phiên làm việc bị lỗi và ra lệnh tắt cưỡng bức (terminate) an toàn.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080308.webp)

7\. [Tài liệu tóm tắt các kiến thức nền tảng về hạ tầng mạng bên trong dịch vụ đám mây AWS](https://medium.com/codenation-engineering/fundamentals-of-networking-in-aws-3ad3d0dc01dd)（Tiếng Anh）

Bài viết hướng dẫn nhập môn chi tiết dành cho các kỹ sư đám mây mới tiếp cận nền tảng AWS: giải thích trực quan các khái niệm cốt lõi như VPC (Mạng riêng ảo), Subnet (Mạng con), bảng định tuyến Route Table, Internet Gateway và cơ chế thiết lập tường lửa bảo mật Security Group.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080401.webp)

8\. [Tổng hợp 17 quy tắc vàng giúp bảo đảm an toàn tài chính cá nhân bền vững](https://thetaoofwealth.wordpress.com/2013/02/17/harry-brownes-17-golden-rules-of-financial-safety/)（Tiếng Anh）

Bài viết giới thiệu và phân tích sâu 17 nguyên tắc cốt lõi về quản lý tài sản, đa dạng hóa danh mục đầu tư và kiểm soát rủi ro tài chính cá nhân dựa trên triết lý của nhà đầu tư nổi tiếng Harry Browne, một tài liệu tham khảo có giá trị cao trong cuộc sống hàng ngày.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090208.webp)

## 工具

1、[Gitstars: Công cụ hỗ trợ quản lý và phân loại các dự án gắn sao trên GitHub](https://github.com/cfour-hi/gitstars)

Ứng dụng web tiện lợi giúp người dùng đồng bộ, gắn tag phân loại chủ đề và lọc tìm kiếm nhanh danh sách các dự án mã nguồn mở mình từng ấn nút Star (thích) trên GitHub để tiện theo dõi. (Đóng góp của [@dllen](https://github.com/ruanyf/weekly/issues/3428))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090109.webp)

2、[Figma.Pub: Công cụ tự động sinh ảnh xuất từ bản vẽ thiết kế trên Figma](https://figma.pub/)

Tiện ích hỗ trợ thiết kế Front-end: tự động tạo liên kết hình ảnh trực tiếp (định dạng JPG, PNG hoặc SVG) trỏ thẳng vào các frame thiết kế trên Figma. Hình ảnh hiển thị qua link sẽ tự động được cập nhật tương ứng mỗi khi nhà thiết kế chỉnh sửa bản vẽ gốc trên Figma. (Đóng góp của [@airyland](https://github.com/ruanyf/weekly/issues/3431))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090111.webp)

3、[MusicFree: Trình phát nhạc mã nguồn mở hỗ trợ kết nối đa nguồn nhạc](https://github.com/maotoumao/MusicFreeDesktop)

Phiên bản phần mềm máy tính của trình phát nhạc mã nguồn mở nổi tiếng, hoạt động dựa trên cơ chế nạp plugin nguồn phát: bản thân phần mềm không tích hợp sẵn nhạc, người dùng có thể nạp các file plugin để nghe nhạc trực tuyến từ nhiều nguồn khác nhau. Bạn đọc có thể xem thêm [Kho plugin mẫu](https://github.com/maotoumao/MusicFreePlugins). (Đóng góp của [@maotoumao](https://github.com/ruanyf/weekly/issues/3451))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090601.webp)

4、[NiceShots: Ứng dụng iOS hỗ trợ thiết kế ảnh chụp màn hình điện thoại chuyên nghiệp](https://apps.apple.com/cn/app/niceshots/id6450619697)

Ứng dụng di động trên iOS giúp người dùng dễ dàng trang trí các bức ảnh chụp màn hình điện thoại: tự động lồng ghép ảnh vào các khung mô phỏng vỏ thiết bị di động (mockup) thời thượng và tùy chỉnh màu sắc hình nền phía sau. (Đóng góp của [@JimmyByte](https://github.com/ruanyf/weekly/issues/3452))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090602.webp)

5、[TabX: Tiện ích mở rộng Chrome hỗ trợ quản lý và sắp xếp thẻ tab](https://github.com/Developer27149/tabX)

Extension dành cho trình duyệt Chrome giúp người dùng dễ dàng quản lý, nhóm lại và dọn dẹp các thẻ tab đang mở để giảm tải bộ nhớ cho máy tính. (Đóng góp của [@Developer27149](https://github.com/ruanyf/weekly/issues/3441))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090207.webp)

6、[AI Town: Dự án game mô phỏng tiểu trấn ảo vận hành tự động bằng AI](https://github.com/get-convex/ai-town)

Mã nguồn mở xây dựng một trò chơi mô phỏng thị trấn nhỏ trên trình duyệt, điểm độc đáo là toàn bộ các nhân vật cư dân trong game đều được điều khiển độc lập bởi các tác nhân AI tự động trò chuyện, tương tác với nhau. Người chơi có thể tham gia vào thị trấn để giao tiếp cùng các AI này. (Đóng góp của [@dllen](https://github.com/ruanyf/weekly/issues/3442))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090401.webp)

7、[Android-Touch-Helper: Tiện ích hỗ trợ tự động bỏ qua quảng cáo mở màn hình trên Android](https://github.com/zfdang/Android-Touch-Helper)

Ứng dụng mã nguồn mở nhỏ gọn dành cho điện thoại Android, tự động phát hiện và mô phỏng thao tác nhấp chọn nút "Bỏ qua" (Skip) xuất hiện trên các quảng cáo chào mừng mỗi khi người dùng vừa mở các ứng dụng trên điện thoại. (Đóng góp của [@Lyeragain](https://github.com/ruanyf/weekly/issues/3402#issuecomment-1704958856))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090403.webp)

8、[MagicNotch: Ẩn phím tắt tính năng thông minh vào vùng tai thỏ trên macOS](https://apps.apple.com/cn/app/magicnotch-elegant-shortcut/id6447055708?mt=12)

Một ứng dụng nhỏ gọn dành cho người dùng Macbook: cho phép cấu hình gán các phím tắt tính năng ẩn vào khu vực "tai thỏ" (notch) ở viền trên màn hình, phím tắt sẽ tự động hiển thị ra khi người dùng di chuột vào khu vực này. (Đóng góp của [@fengyiqicoder](https://github.com/fengyiqicoder))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090404.webp)

9、[File Bridge: Kịch bản JS hỗ trợ truyền tải file trực tiếp giữa hai máy tính qua trình duyệt](https://github.com/ppz-pro/file-bridge)

Một tập lệnh JS gọn nhẹ hỗ trợ người dùng chia sẻ tệp tin trực tiếp giữa hai máy tính thông qua môi trường trình duyệt web mà không cần cài đặt thêm phần mềm và không yêu cầu hai thiết bị phải ở cùng mạng LAN cục bộ. (Đóng góp của [@daGaiGuanYu](https://github.com/ruanyf/weekly/issues/3449))

10、[Whisper Web: Tiện ích chuyển đổi âm thanh tiếng Anh sang văn bản trực tuyến](https://huggingface.co/spaces/Xenova/whisper-web)

Ứng dụng chạy trực tiếp trên trình duyệt web, sử dụng mô hình AI Whisper để chuyển đổi các tệp ghi âm giọng nói tiếng Anh thành văn bản thô một cách nhanh chóng mà không yêu cầu người dùng phải đăng ký tài khoản. (Đóng góp của [@Y024](https://github.com/ruanyf/weekly/issues/3457))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090709.webp)

11、[StableDiffusion XL: Trang web trải nghiệm vẽ tranh bằng mô hình SDXL miễn phí](https://www.stablediffusionai.ai/)

Cổng trải nghiệm trực tuyến mô hình vẽ tranh thế hệ mới Stable Diffusion XL do cộng đồng tự thiết lập, cho phép người dùng nhập câu lệnh văn bản (prompt) để sinh ảnh nghệ thuật trực tiếp hoàn toàn miễn phí và không cần đăng nhập. (Đóng góp của [@zengdamo](https://github.com/ruanyf/weekly/issues/3455))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090708.webp)

## 资源

1\. [Hello 算法: Giáo trình cấu trúc dữ liệu và giải thuật trực quan mã nguồn mở](https://github.com/krahets/hello-algo)

Bộ giáo trình học tập cấu trúc dữ liệu và giải thuật viết bằng tiếng Trung được mở nguồn hoàn toàn trên GitHub, sở hữu giao diện trình bày hiện đại đi kèm nhiều sơ đồ chuyển động trực quan giúp người học dễ dàng nắm bắt kiến thức nền tảng. (Đóng góp của [@Y024](https://github.com/ruanyf/weekly/issues/3430))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090110.webp)

2、[AIHub: Thư mục tổng hợp các trang web và tài nguyên trí tuệ nhân tạo](https://www.aihub.cn/)

Trang web thư viện chuyên thu thập, phân loại danh mục và cập nhật liên kết của hàng trăm ứng dụng, dịch vụ AI đang hoạt động trên toàn thế giới để người dùng tiện tra cứu. (Đóng góp của [@liuluanping](https://github.com/ruanyf/weekly/issues/3427))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090108.webp)

3\. [WebAV: Chuỗi bài viết hướng dẫn kỹ thuật xử lý âm thanh hình ảnh trên trình duyệt](https://hughfenghen.github.io/tag/WebAV/)

Tập hợp các bài viết phân tích kỹ thuật chuyên sâu hướng dẫn lập trình viên Front-end cách thức viết mã ứng dụng xử lý, cắt ghép và biên tập các luồng dữ liệu âm thanh video trực tiếp trên trình duyệt web. (Đóng góp của [@hughfenghen](https://github.com/ruanyf/weekly/issues/3434))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090112.webp)

4\. [yesicon: Thư viện tìm kiếm biểu tượng icon hỗ trợ từ khóa dịch nghĩa tiếng Trung](https://yesicon.app/)

Công cụ tìm kiếm biểu tượng đồ họa hữu ích dành cho nhà thiết kế và lập trình viên: tác giả đã ứng dụng AI để dịch nghĩa toàn bộ tên gọi của hơn 18 vạn icon trong kho Iconify sang tiếng Trung giúp việc gõ từ khóa tìm kiếm icon trở nên dễ dàng hơn. (Đóng góp của [@dongnaebi](https://github.com/dongnaebi))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090206.webp)

5\. [Awesome Domain LLM: Thư mục tổng hợp các mô hình LLM chuyên biệt ngành nghề](https://github.com/luban-agi/Awesome-Domain-LLM)

Repository tổng hợp liên kết của các dự án phát triển mô hình ngôn ngữ lớn chuyên sâu được tinh chỉnh (fine-tuned) dành riêng cho các ngành nghề cụ thể (như y tế, luật pháp, tài chính). (Đóng góp của [@wuyifan18](https://github.com/ruanyf/weekly/issues/3453))

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090603.webp)

## 图片

1、**Màu sắc đặc biệt "International Orange" và các ứng dụng trong thực tế**

“International Orange” (Màu cam quốc tế) là một tông màu cam đặc biệt được phát triển riêng cho ngành công nghiệp hàng không vũ trụ và các công trình xây dựng lớn nhằm mục đích tạo độ tương phản thị giác tối đa giúp phân biệt vật thể với môi trường xung quanh. Tông màu này có sắc cam nguyên bản nhưng sẫm màu và ngả nhiều sang sắc đỏ hơn:

* Mẫu trang phục phi hành gia thời kỳ đầu của NASA sử dụng tông màu này:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040616.webp)

* Công trình Cầu Cổng Vàng nổi tiếng tại San Francisco và cây cầu 25 tháng 4 tại Lisbon, Bồ Đào Nha (hình dưới) cũng được sơn phủ tông màu đặc trưng này:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040617.webp)

* Tháp truyền hình Tokyo và hệ thống cột anten đặt trên nóc các tòa nhà chọc trời cũng bắt buộc phải sơn xen kẽ màu cam quốc tế và màu trắng để cảnh báo an toàn hàng không:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040618.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040619.webp)

2、**Nghệ thuật vẽ tay các tấm bản đồ chi tiết của khu vực trượt tuyết núi cao**

Tại Mỹ có một nghệ sĩ nổi tiếng chuyên vẽ tay các tấm bản đồ địa hình dành cho các khu nghỉ dưỡng trượt tuyết núi cao, với độ tỉ mỉ mô phỏng chân thực từng rặng cây, sườn núi:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040806.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040807.webp)

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040808.webp)

* Một bức tranh bản đồ hoàn thiện sau khi vẽ:

![](https://cdn.beekka.com/blogimg/asset/202304/bg2023040809.webp)

Mặc dù trong thời đại hiện nay các tấm bản đồ không ảnh chụp từ vệ tinh có độ sắc nét rất cao, những tác phẩm bản đồ vẽ tay giàu tính nghệ thuật này vẫn được cộng đồng người đam mê trượt tuyết vô cùng yêu thích và sưu tầm như các tác phẩm nghệ thuật.

## ✍️ Bài đọc thêm

### Tại sao việc tái chế các loại rác thải chất liệu nhựa trong thực tế lại cực kỳ khó khả thi?

Chất thải nhựa hiện là một trong những nguồn gây ô nhiễm môi trường nghiêm trọng nhất trên Trái Đất. Nhiều người thường đề xuất giải pháp thu gom tái chế nhựa để tái sử dụng, tuy nhiên trong thực tế quy trình này gặp phải 3 rào cản chí mạng khiến nó khó hoạt động hiệu quả:

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090604.webp)

**1. Sự phân mảnh quá mức của các chủng loại nhựa**

Nhựa trong thực tế không phải là một chất liệu đơn nhất mà có hàng ngàn chủng loại nhựa khác nhau, mỗi loại sở hữu công thức hóa học, chất phụ gia chịu nhiệt và màu nhuộm riêng biệt, hoàn toàn không thể nấu nóng chảy để tái chế cùng nhau.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090605.webp)

Để tái chế, chúng ta bắt buộc phải phân loại rác thải nhựa thành từng nhóm chất liệu độc lập. Lấy ví dụ đơn giản: ngay trên một chai nước ngọt bằng nhựa thông thường, phần nắp chai và phần thân chai đã sử dụng hai chất liệu nhựa hoàn toàn khác nhau (PET#1 và HDPE#2) và bắt buộc phải bóc tách xử lý riêng biệt. Các loại rác thải sinh hoạt như cốc dùng một lần, khay đựng thức ăn nhanh của các cửa hàng đồ ăn nhanh thường được tạo thành từ 4-5 loại nhựa khác nhau, việc phân loại thủ công chúng trong thực tế là bất khả thi.

**2. Rủi ro cháy nổ và nguy cơ tồn dư hóa chất độc hại**

Quy trình gia công tái chế hạt nhựa tại nhà máy tiềm ẩn rủi ro cháy nổ rất cao giải phóng lượng lớn khí độc hại ra môi trường xung quanh. Đồng thời khác với kim loại hay thủy tinh, chất liệu nhựa không có tính trơ hóa học nên dễ dàng hấp thụ các chất độc hại trong quá trình sử dụng. Hạt nhựa tái sinh thu được thường có nguy cơ tồn dư độc tố hóa học cao, do đó nhiều quốc gia như Canada đã ban hành luật nghiêm cấm sử dụng nhựa tái chế để sản xuất bao bì đựng thực phẩm trực tiếp nhằm bảo vệ sức khỏe người dân.

**3. Bài toán kinh tế không có lời giải**

Hạt nhựa nguyên sinh mới sản xuất từ dầu mỏ hiện có giá thành cực kỳ rẻ. Trong khi đó, chi phí cần chi trả cho quy trình thu gom, vận chuyển, phân loại thủ công và xử lý nhiệt để tạo ra hạt nhựa tái sinh là cực kỳ đắt đỏ. Giá thành của nhựa tái sinh luôn cao hơn hẳn nhựa mới khiến các doanh nghiệp hoàn toàn không có động lực kinh tế để sử dụng nhựa tái chế trong sản xuất.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023090606.webp)

Vì 3 lý do cốt lõi nêu trên, hoạt động tái chế không thể giải quyết được triệt để bài toán ô nhiễm rác thải nhựa. Giải pháp khả thi duy nhất hiện nay vẫn là chủ động cắt giảm tối đa việc sử dụng các sản phẩm nhựa dùng một lần trong đời sống hàng ngày kết hợp các biện pháp chôn lấp tập trung khoa học.

## Lịch sử tuần này

- 2022年（第 223 期）：[Nghề nghiệp: Lập trình viên liệu có cần quá lo ngại trước các làn sóng sa thải nhân sự của ngành công nghệ](http://www.ruanyifeng.com/blog/2022/09/weekly-issue-223.html)
- 2021年（第 173 期）：[Thiết kế phần cứng: Tìm hiểu tư duy thiết kế và cấu tạo của các dòng máy thu thanh Internet](http://www.ruanyifeng.com/blog/2021/08/weekly-issue-173.html)
- 2020年（第 123 期）：[Quản trị doanh nghiệp: Mối liên hệ thú vị giữa cơ chế vận hành của công ty Internet và quân chế Tương quân](http://www.ruanyifeng.com/blog/2020/09/weekly-issue-123.html)
- 2019年（第 73 期）：[Khoa học dữ liệu: Sức mạnh và tầm ảnh hưởng của việc phân tích thống kê dữ liệu lớn trong xã hội](http://www.ruanyifeng.com/blog/2019/09/weekly-issue-73.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
