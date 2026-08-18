# Bản tin chia sẻ công nghệ (Số 351): GitHub Issues (gần như) là ứng dụng ghi chú tốt nhất

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/6965) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060101.webp)

Tòa nhà mới của Viện Thiết kế Điện lực Hoa Đông tại Thượng Hải sở hữu một hệ thống cầu thang xoắn ốc ngoài trời cao tới 15 tầng vô cùng độc đáo, mang ý nghĩa biểu tượng mô phỏng theo cấu trúc cuộn dây Tesla. (Nguồn: [archiposition.com](https://www.archiposition.com/items/20240812045536))

## GitHub Issues（几乎）是最好的笔记应用

[Issues](https://github.com/features/issues) là công cụ quản lý lỗi (Bug tracking) mặc định được tích hợp sẵn trên mọi kho lưu trữ mã nguồn của GitHub.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025053102.webp)

Không chỉ giới hạn ở nhiệm vụ theo dõi lỗi lập trình, công cụ này còn được cộng đồng công nghệ khai thác cho rất nhiều mục đích sáng tạo khác.

Ví dụ tiêu biểu là bản thân tôi đã biến khu vực Issues của bản tin thành một diễn đàn thảo luận mở, nơi mọi người có thể tự do gửi bài viết giới thiệu các dự án cá nhân của mình.

Nhiều lập trình viên khác lại lựa chọn biến Issues thành một hệ quản trị nội dung (CMS) cá nhân để viết blog hoặc lưu trữ các bài viết chuyên môn.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025053105.webp)

Mới đây, nhà phát triển nổi tiếng Simon Willison (đồng tác giả của bộ khung Django danh tiếng) đã chia sẻ bài viết [đưa ra nhận định](https://simonwillison.net/2025/May/26/notes/) rằng: **GitHub Issues (gần như) là ứng dụng ghi chú cá nhân xuất sắc nhất trên thế giới**.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025053103.webp)

Giữa vô vàn các phần mềm ghi chú chuyên dụng hiện nay trên thị trường, tại sao ông lại dành sự ưu ái đặc biệt này cho một công cụ vốn dĩ không được thiết kế cho tác vụ ghi chép như GitHub Issues?

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025053104.webp)

Dưới đây là các lập luận thuyết phục được ông đưa ra:

（1）**Hoàn toàn miễn phí** và không bị giới hạn về không gian lưu trữ hay số lượng ghi chú khởi tạo.

（2）Hỗ trợ linh hoạt chế độ hiển thị: Ghi chú có thể công khai (public) cho cộng đồng cùng đọc hoặc thiết lập riêng tư (private) cho cá nhân.

（3）Hỗ trợ hệ thống thẻ nhãn dán (labels) để phân loại ghi chú khoa học, thậm chí hỗ trợ cấu trúc [ghi chú phân tầng](https://docs.github.com/en/issues/tracking-your-work-with-issues/using-issues/adding-sub-issues) (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025053106.webp)

（4）Tương thích hoàn hảo với cú pháp Markdown, hỗ trợ làm nổi bật cú pháp mã nguồn (code syntax highlighting) và chèn tốt [các định dạng sơ đồ, đồ thị](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/creating-diagrams) phức tạp (như sơ đồ Mermaid).

（5）Hỗ trợ tải lên hình ảnh và video hoàn toàn miễn phí.

（6）Hỗ trợ cơ chế liên kết nội bộ thông minh: Tự động chuyển đổi các đường dẫn liên kết URL của GitHub thành tiêu đề trang tương ứng một cách trực quan (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060407.webp)

（7）Tích hợp sẵn các tính năng thảo luận bình luận và công cụ tìm kiếm nội dung mạnh mẽ.

（8）Bên cạnh phiên bản giao diện Web, hệ thống cung cấp sẵn các ứng dụng native mượt mà chạy trên Windows, macOS, Android và iOS.

（9）Cung cấp bộ cổng kết nối API toàn diện, hỗ trợ lập trình tự động hóa các thao tác tạo mới, chỉnh sửa hoặc xuất dữ liệu ghi chú, đồng thời có thể kết hợp cùng dịch vụ GitHub Actions để tự động hóa mọi quy trình xuất bản dữ liệu lên website cá nhân.

Điểm hạn chế duy nhất của giải pháp này là việc thiếu tính năng hỗ trợ hoạt động ngoại tuyến (offline). Nếu thiết bị của bạn hoàn toàn mất kết nối mạng internet, bạn sẽ không thể truy cập hay soạn thảo ghi chú được.

Liệu các lập luận trên đã đủ sức thuyết phục bạn chưa?

Dưới góc nhìn cá nhân, tôi thấy phân tích của tác giả rất hợp lý và thực tế. Các bạn hoàn toàn có thể thử trải nghiệm chuyển dịch kho ghi chú cá nhân của mình sang quản lý bằng công cụ GitHub Issues xem sao.

## [活动] 稀土掘金“夏日寻宝”

Cộng đồng nhà phát triển công nghệ nổi tiếng tại Trung Quốc "Xitu Juejin" trong tháng này đang triển khai một chiến dịch trải nghiệm mới rất hấp dẫn.

Nhằm thúc đẩy phong trào ứng dụng AI trong lập trình, họ đã kết hợp cùng Trae để khởi động chiến dịch mang tên **"Cuộc săn lùng kho báu trong thế giới lập trình thông minh Trae"** (夏日寻宝).

> Trae là trình soạn thảo mã nguồn tích hợp AI đầu tiên được phát triển tối ưu cho cộng đồng người dùng tiếng Trung, cung cấp môi trường lập trình AI toàn diện và dễ dàng tiếp cận cho mọi đối tượng.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060504.webp)

Đối với nhóm người dùng mới, chỉ cần hoàn thành các tác vụ trải nghiệm tính năng cơ bản của Trae theo yêu cầu là bạn đã nhận được số điểm tích lũy tương ứng. Đối với nhóm người dùng hiện tại, việc giới thiệu bạn bè đăng ký trải nghiệm Trae thành công cũng sẽ giúp bạn gia tăng điểm tích lũy của mình trên hệ thống.

**Số điểm tích lũy được sử dụng để đổi lấy các phần quà công nghệ vô cùng giá trị (tích lũy càng nhiều điểm, quà nhận được càng lớn)** như camera DJI Pocket 3, đồng hồ thông minh Apple Watch, thẻ mua sắm JD, bàn phím cơ gaming...

Nếu bạn đang lên kế hoạch làm chủ một công cụ lập trình AI IDE chất lượng, đồng thời muốn nhận được các phần quà công nghệ giá trị, đây là cơ hội trải nghiệm rất tốt không nên bỏ lỡ.

Các bạn có thể click truy cập [địa chỉ đăng ký chính thức](https://sourl.co/cFpPWp) hoặc quét mã QR trên poster để xem chi tiết thể lệ tham gia. Cổng đăng ký hiện đã mở và sẽ chính thức đóng lại vào ngày 30 tháng 6 tới.

## 科技动态

1、[Mở ra cơ hội mới cho bệnh nhân liệt nhờ công nghệ não - tủy](https://news.cgtn.com/news/2025-03-05/China-conducts-4th-brain-spine-interface-surgery-on-paralyzed-patients-1Bux8OhJ8ZO/p.html)

Bệnh viện Trung Sơn tại Thượng Hải vừa thực hiện thành công ca phẫu thuật cấy ghép thiết bị "giao diện não - tủy" (Brain-Spine Interface) để hỗ trợ điều trị cho bệnh nhân bị liệt nửa người.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060102.webp)

Nguyên nhân cốt lõi dẫn đến tình trạng liệt là do sự đứt gãy liên kết dẫn truyền thần kinh giữa não bộ và tủy sống, khiến các tín hiệu vận động từ não không thể truyền tới tủy sống để điều khiển cơ bắp.

Các nhà khoa học đã tiến hành cấy ghép các hạt điện cực siêu nhỏ trực tiếp vào vỏ não vận động để ghi nhận tín hiệu sóng não, sau đó truyền các tín hiệu này bỏ qua đoạn đứt gãy để kích thích trực tiếp vào các dây thần kinh tủy sống tương ứng, hoạt động như một chiếc cầu nối nhân tạo dẫn truyền tín hiệu.

Ca phẫu thuật lâm sàng đầu tiên được thực hiện vào tháng 1 vừa qua đã ghi nhận kết quả rất tích cực khi giúp một bệnh nhân bị liệt vận động lâu năm có thể tự đứng dậy và thực hiện các bước đi ngắn chỉ sau 24 giờ hoàn thành phẫu thuật.

2、[Nghiên cứu thành công dòng máu nhân tạo không phân biệt nhóm máu](https://www.tokyoweekender.com/entertainment/tech-trends/japanese-scientists-develop-artificial-blood/)

Các nhà khoa học tại Nhật Bản công bố nghiên cứu chế tạo thành công mẫu máu nhân tạo đa năng có khả năng truyền an toàn cho mọi người nhận mà không bận tâm đến nhóm máu.

Nguyên nhân cấu trúc phân định các nhóm máu khác nhau của con người xuất phát từ việc bề mặt các tế bào hồng cầu sinh học sở hữu các loại kháng nguyên (antigens) khác biệt.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060314.webp)

Để giải quyết bài toán tương thích này, nhóm nghiên cứu đã tiến hành bóc tách các phân tử hemoglobin từ nguồn máu hiến tặng quá hạn sử dụng, sau đó thiết lập một lớp vỏ bọc bảo vệ nhân tạo bao quanh các phân tử này.

Lớp vỏ bọc bảo vệ này bảo đảm không gây ảnh hưởng đến năng lực vận chuyển oxy cốt lõi của hemoglobin, đồng thời loại bỏ hoàn toàn các cấu trúc kháng nguyên bề mặt, giúp nguồn máu nhân tạo này có thể truyền an toàn cho bất kỳ bệnh nhân nào mà hoàn toàn không xảy ra hiện tượng đào thải miễn dịch.

3、Người dùng phát hiện ra cấu trúc bắt đầu (Start Menu) của hệ điều hành Windows 11 thực chất được xây dựng trên bộ khung lập trình di động **React Native**.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025053006.webp)

Chi tiết thiết kế này đang vấp phải nhiều sự phàn nàn của cộng đồng về mặt hiệu năng. Các thử nghiệm cho thấy mỗi khi người dùng click mở Start Menu, mức độ chiếm dụng tài nguyên của một nhân CPU có thể đột ngột tăng vọt lên tới ngưỡng từ 30% đến 70%.

4、Tổng công ty Bưu chính Nhật Bản giới thiệu dịch vụ **"Địa chỉ số"** độc đáo, cho phép mỗi người dân đăng ký một mã số định danh gồm 7 chữ số đại diện cho địa chỉ cư trú thực tế của mình, hoạt động tương tự như mô hình hộp thư bưu điện.

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052904.webp)

Khi gửi nhận bưu phẩm, người dùng chỉ cần điền mã số định danh này thay vì phải viết toàn bộ địa chỉ chi tiết bằng chữ. Giải pháp này không chỉ giúp đơn giản hóa quy trình gửi nhận thư, mà còn giúp người dùng giữ nguyên mã số địa chỉ liên hệ này ngay cả khi chuyển nhà sang sinh sống tại các địa phương khác.

5、Đội ngũ phát triển dự án mã nguồn mở .NET của Microsoft mới đây đã quyết định cấp quyền cho trợ lý ảo GitHub Copilot tự động tạo và gửi các bản cập nhật sửa lỗi (Pull Requests), dẫn đến một [tình huống đối thoại dở khóc dở cười](https://nmn.gl/blog/ai-scam).

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052517.webp)

Hệ thống AI đã tự động gửi lên một bản cập nhật code chứa lỗi lập trình khá ngớ ngẩn. Khi lập trình viên con người chỉ ra lỗi sai, AI lập tức phản hồi tự tin khẳng định mã nguồn của mình hoàn toàn chính xác.

Kỹ sư phần mềm buộc phải viết các đoạn giải thích chi tiết giải thích rõ bản chất lỗi logic cho AI hiểu, và chu trình giải thích - phản biện này phải lặp đi lặp lại tới vài lần AI mới chịu ghi nhận và sửa đổi.

Kịch bản đối thoại này nhiều khả năng sẽ xuất hiện ngày một phổ biến hơn trong tương lai, khi con người phải tốn rất nhiều công sức chỉ để giải thích và chứng minh cho AI hiểu tại sao các kết xuất của nó là sai lệch.

## 文章

1、[Chia sẻ kinh nghiệm tham gia quy trình phỏng vấn tại tập đoàn Canonical](https://dustri.org/b/my-experience-with-canonicals-interview-process.html) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060203.webp)

Canonical là doanh nghiệp đứng sau hỗ trợ sự phát triển của hệ điều hành Linux Ubuntu nổi tiếng. Tác giả chia sẻ chi tiết trải nghiệm phỏng vấn tuyển dụng thực tế của mình đi qua nhiều vòng đánh giá khắt khe từ sơ tuyển đến vòng phỏng vấn cuối cùng với ban lãnh đạo.

Diễn biến quy trình phỏng vấn làm người đọc khá kinh ngạc khi một trong những câu hỏi cốt lõi quyết định kết quả tuyển dụng lại tập trung vào việc đánh giá điểm số học tập thời kỳ trung học của ứng viên. Dựa trên trải nghiệm phỏng vấn có phần kỳ lạ này, tác giả đưa ra những nhận định tương đối bi quan về định hướng phát triển tương lai của Ubuntu.

2、[Đánh giá về độ tin cậy của các thẻ nhớ microSD trong lưu trữ dữ liệu](https://old.reddit.com/r/raspberry_pi/comments/1l0v25s/how_reliable_are_microsd_cards_well_as_it_turns/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060204.webp)

Tác giả đã thực hiện các thử nghiệm đo đạc thực tế trên hơn 200 chiếc thẻ nhớ microSD khác nhau, đưa ra kết luận độ bền bỉ dài hạn của dòng thẻ nhớ này là khá kém. Sau khi trải qua khoảng 3.000 chu kỳ đọc ghi dữ liệu liên tục, hầu hết các thẻ nhớ đều bắt đầu xuất hiện các sự cố hư hỏng hoặc phát sinh lỗi ghi chép.

Bài viết cũng đưa ra các nhận xét đánh giá chi tiết về chất lượng của hơn 10 thương hiệu thẻ nhớ phổ biến trên thị trường để người dùng tham khảo khi mua sắm.

3、[Đội ngũ phát triển Go tuyên bố ngừng các nỗ lực thay đổi cú pháp xử lý lỗi](https://go.dev/blog/error-syntax) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060403.webp)

Ngôn ngữ Go sở hữu cơ chế xử lý ngoại lệ đặc thù khi trả về lỗi như một giá trị độc lập, dẫn đến việc nhà phát triển phải liên tục viết các khối lệnh kiểm tra lỗi lặp đi lặp lại khiến mã nguồn bị phình to và rườm rà.

Trong nhiều năm qua, cộng đồng nhà phát triển liên tục gửi các yêu cầu mong muốn ban quản trị thiết lập một cú pháp xử lý lỗi ngắn gọn và hiện đại hơn. Đội ngũ phát triển Go đã thử nghiệm nhiều giải pháp cú pháp khác nhau nhưng đều không đạt được sự đồng thuận cao. Mới đây, ban quản trị đã chính thức thông báo sẽ dừng toàn bộ các nỗ lực thay đổi cú pháp này và quyết định duy trì cơ chế xử lý lỗi truyền thống của Go.

4、[Giới thiệu giao thức kết nối NLWeb mới dành cho AI](https://glama.ai/blog/2025-06-01-what-is-nlweb) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060309.webp)

NLWeb là giao thức kết nối giao tiếp mới do Microsoft đề xuất với cơ chế hoạt động tương tự như giao thức MCP của Anthropic. Mục tiêu của NLWeb là chuẩn hóa cổng kết nối giao tiếp giữa các website trực tuyến với các mô hình ngôn ngữ lớn AI, giúp AI dễ dàng truy xuất và cập nhật dữ liệu từ trang web. Bài viết giới thiệu tổng quan các tính năng kỹ thuật của giao thức mới này.

5、[Hướng dẫn các bước chạy các mô hình AI cục bộ trên máy tính cá nhân](https://anthonylewis.com/2025/06/01/run-your-own-ai/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060404.webp)

Bài hướng dẫn ngắn gọn các bước thiết lập và sử dụng thư viện Python **llm** để nhanh chóng tải và khởi chạy trực tiếp các mô hình AI mã nguồn mở ngay trên phần cứng máy tính cá nhân của bạn.

## 工具

1、[Quarkdown](https://github.com/iamgio/quarkdown)

Hệ thống biên tập và dàn trang tài liệu trực quan dựa trên cú pháp định dạng Markdown tối giản.

2、[RsyncUI](https://github.com/rsyncOSX/RsyncUI)

Ứng dụng mã nguồn mở dành cho hệ điều hành macOS, cung cấp giao diện đồ họa trực quan (GUI) cho câu lệnh rsync truyền thống giúp đơn giản hóa quy trình đồng bộ và truyền tải tệp tin với máy chủ từ xa.

3、[Donut](https://donutbrowser.com/)

Công cụ quản lý trình duyệt độc đáo, hỗ trợ người dùng thiết lập và lưu trữ nhiều hồ sơ cấu hình trình duyệt khác nhau (về cookie, tài khoản, proxies...) để nhanh chóng kích hoạt khi cần thiết.

4、[Read Frog (陪读蛙)](https://readfrog.mengxi.work/zh)

Tiện ích mở rộng trình duyệt hỗ trợ dịch thuật trang web trực quan, tự động trích xuất nội dung chính của bài viết và cung cấp tính năng phân tích chi tiết ý nghĩa của các từ vựng và câu văn phức tạp cho người học ngoại ngữ, dự án [chia sẻ mã nguồn mở tại GitHub](https://github.com/mengxi-ream/read-frog). (Đóng góp từ [@mengxi-ream](https://github.com/ruanyf/weekly/issues/6956))

5、**Từ Tiểu Ngộ (词小悟)**

Ứng dụng nhỏ (Mini Program) trên WeChat hỗ trợ người dùng học và ghi nhớ từ vựng tiếng Anh hiệu quả thông qua việc so khớp hình ảnh minh họa trực quan. (Đóng góp từ [@fluidog](https://github.com/ruanyf/weekly/issues/6962))

6、[Datetime.app](https://datetime.app/)

Dự án trang web hiển thị thông tin ngày giờ và múi giờ quốc tế chính xác mã nguồn mở, được phát triển như một giải pháp thay thế tự chủ chất lượng cho trang web nổi tiếng time.is. (Đóng góp từ [@airyland](https://github.com/ruanyf/weekly/issues/6970))

7、[naviix](https://github.com/wswmsword/naviix)

Thư viện JavaScript mã nguồn mở hỗ trợ thiết lập tính năng điều hướng bàn phím cho trang web, cho phép người dùng sử dụng các phím mũi tên lên/xuống/trái/phải để chuyển đổi nhanh tiêu điểm giữa các phần tử trên trang. (Đóng góp từ [@wswmsword](https://github.com/ruanyf/weekly/issues/6975))

8、[go-v2ex](https://github.com/seth-shi/go-v2ex)

Dự án xây dựng ứng dụng đọc và tương tác với diễn đàn công nghệ V2EX trực tiếp bên trong giao diện dòng lệnh terminal viết bằng ngôn ngữ Go. (Đóng góp từ [@seth-shi](https://github.com/ruanyf/weekly/issues/6978))

9、[TL-RTC-APP](https://github.com/tl-open-source/tl-rtc-app)

Hệ thống truyền thông tin và chia sẻ tệp tin trực tuyến đa năng mã nguồn mở phát triển hoàn toàn trên giao thức WebRTC. (Đóng góp từ [@iamtsm](https://github.com/ruanyf/weekly/issues/6986))

## AI 相关

1、[Google AI Edge Gallery](https://github.com/google-ai-edge/gallery)

Ứng dụng di động do Google phát hành cho phép người dùng tải và khởi chạy trực tiếp các mô hình AI mã nguồn mở từ kho chứa Hugging Face ngay trên phần cứng của điện thoại Android mà không cần kết nối mạng.

2、[Bing Video Creator](https://www.bing.com/images/create/make-a-video/645d21a9470d4f4388cf46635f40809d)

Dịch vụ tìm kiếm Bing của Microsoft chính thức tích hợp tính năng sinh video từ mô tả văn bản hoàn toàn miễn phí cho người dùng, vận hành dựa trên lõi công nghệ mô hình sinh video Sora của OpenAI (tính năng hiện được phát hành giới hạn trên ứng dụng di động Bing).

3、[AIDocGenius (Trợ lý tài liệu thông minh)](https://github.com/jiangmuran/AIDocGenius)

Bộ kịch bản Python hỗ trợ tự động kết nối mô hình AI để tiến hành tóm tắt nội dung tài liệu, dịch thuật ngôn ngữ, phân tích dữ liệu và tự động chuyển đổi định dạng tệp tin văn bản. (Đóng góp từ [@jiangmuran](https://github.com/ruanyf/weekly/issues/6958))

4、[Low Fade AI](https://lowfade.app/)

Dịch vụ trực tuyến miễn phí ứng dụng AI hỗ trợ người dùng thử nghiệm thay đổi các kiểu tóc và màu nhuộm tóc khác nhau trên ảnh chân dung mà không cần đăng ký tài khoản. (Đóng góp từ [@twjiem](https://github.com/ruanyf/weekly/issues/6961))

5、[Read Bridge](https://github.com/WindChimeEcho/read-bridge)

Trợ lý đọc sách điện tử định dạng EPUB thông minh, tích hợp AI hỗ trợ phân tích sâu ý nghĩa ngữ cảnh của các câu văn phức tạp trong sách, hỗ trợ trải nghiệm trực tuyến tại [readbridge.cc](https://readbridge.cc). (Đóng góp từ [@WindChimeEcho](https://github.com/ruanyf/weekly/issues/6977))

6、[TEN VAD](https://github.com/TEN-framework/ten-vad)

Mô hình AI nhỏ gọn sở hữu tốc độ xử lý cực nhanh chuyên dụng cho tác vụ nhận diện sự xuất hiện của giọng nói con người (Voice Activity Detection) từ các luồng âm thanh đầu vào thời gian thực. (Đóng góp từ [@bluemotional](https://github.com/ruanyf/weekly/issues/6979))

## 资源

1、[Thư viện Sách kỹ thuật số dành cho người khiếm thị Trung Quốc](http://www.cdlvi.cn)

Kho lưu trữ sách trực tuyến do Thư viện Quốc gia Trung Quốc thiết lập dành riêng cho người khiếm thị, toàn bộ trang web được xây dựng tối ưu theo các tiêu chuẩn tiếp cận không rào cản (accessibility) đi kèm tính năng đọc thành tiếng cho toàn bộ nội dung.

2、[Thư viện Tài liệu Sáng tạo và Khởi nghiệp dành cho sinh viên](https://cy.urongda.com/explore)

Kho lưu trữ tài liệu trực tuyến miễn phí tổng hợp các hồ sơ dự án mẫu và tài liệu hướng dẫn chất lượng của các cuộc thi khởi nghiệp sinh viên lớn. (Đóng góp từ [@urongda](https://github.com/ruanyf/weekly/issues/6959))

3、[Cơ sở tri thức Vũ trụ Thông Liêu (通辽宇宙知识库)](https://www.tongliaouniverse.cn)

Trang web cơ sở dữ liệu lịch sử tương tác độc đáo được xây dựng dành riêng cho cộng đồng người hâm mộ của kênh YouTube lịch sử nổi tiếng "Tiểu Ước Hàn Khả Hãn". (Đóng góp từ [@Acorn2](https://github.com/ruanyf/weekly/issues/6990))

4、[Reddit Top](https://reddit-top.pages.dev/)

Dịch vụ web hỗ trợ tổng hợp và hiển thị các bài viết nhận được lượng tương tác nóng hổi nhất trên diễn đàn Reddit từ các subreddits chỉ định của người dùng. (Đóng góp từ [@zhangchenchen](https://github.com/ruanyf/weekly/issues/6957))

5、[Công cụ sinh địa chỉ Mỹ mẫu (US Address Generator)](https://www.usaddrgen.com/zh/)

Dịch vụ web hỗ trợ tạo các dữ liệu thông tin cá nhân giả lập tại Mỹ (bao gồm thông tin địa chỉ nhà, tên tuổi, thẻ tín dụng mẫu, tình trạng việc làm...) phục vụ cho các nhu cầu kiểm thử tính năng biểu mẫu của lập trình viên. (Đóng góp từ [@watianle](https://github.com/ruanyf/weekly/issues/6972))

## 图片

1、[Tác phẩm nghệ thuật đường phố mới nhất của nghệ sĩ Banksy](https://www.smithsonianmag.com/smart-news/banksy-unveils-new-lighthouse-mural-with-the-words-i-want-to-be-what-you-saw-in-me-in-france-180986719/)

Banksy là nghệ sĩ graffiti đường phố nổi tiếng thế giới với phong cách vẽ ẩn danh luôn bất ngờ để lại các tác phẩm nghệ thuật độc đáo tại các mảng tường công cộng trên thế giới.

Vào ngày 29 tháng 5 vừa qua, một tác phẩm mới của ông đã được phát hiện xuất hiện trên một bức tường tại thành phố Marseille (Pháp).

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060305.webp)

Ông đã khéo léo vẽ thêm phần hình ảnh bóng đổ của chiếc cột thép rào bảo vệ vỉa hè lên bức tường phía sau, biến chiếc bóng đổ đơn điệu thành hình ảnh một ngọn hải đăng đang tỏa sáng.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060306.webp)

Bên dưới bức vẽ là dòng chữ thông điệp: "I want to be what you saw in me" (Tôi mong muốn trở thành ngọn hải đăng mà bạn nhìn thấy từ tôi).

Thông điệp mang ý nghĩa nhân văn sâu sắc: Dù bản thân tôi ngoài đời thực chỉ là một chiếc cột sắt nhỏ bé và tầm thường chắn đường, tôi vẫn luôn nỗ lực nuôi dưỡng ước mơ trở thành một ngọn hải đăng soi sáng dẫn lối trong mắt bạn.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060307.webp)

2、[Năng lực viết văn xuôi đầy cảm xúc của ChatGPT](https://fakepixels.substack.com/p/ai-heidegger-and-evangelion)

Một người dùng công nghệ đã thử thách ChatGPT viết một đoạn văn ngắn bằng ngôn ngữ văn chương để mô tả về cuộc sống sinh hoạt hằng ngày tại thành phố New York.

Hệ thống AI đã kết xuất ra câu trả lời dưới đây:

![](https://cdn.beekka.com/blogimg/asset/202505/bg2025052516.webp)

> New York là không gian đô thị duy nhất trên thế giới mang lại cho bạn cảm giác những điều kỳ diệu luôn hiện hữu trong tầm tay. Nhịp sống hỗn loạn nơi đây sẽ liên tục mài giũa ý chí phấn đấu của bạn, và mỗi góc đường phố xuất hiện như một tấm gương phản chiếu, thôi thúc bạn suy ngẫm về mẫu hình nhân cách mình muốn trở thành trong tương lai.
>
> Bạn dành tình yêu cho New York bởi nơi đây giúp cụ thể hóa mọi khát vọng của bản thân. Một không gian đô thị nơi sự xa lạ và sự gần gũi cùng tồn tại song song; nơi bạn có thể đắm chìm vào sự cô độc tuyệt đối của cá nhân nhưng vẫn cảm nhận được nhịp đập kết nối đồng điệu với hàng triệu con người xung quanh. Nhịp sống của thành phố tương thích hoàn hảo với tốc độ của bạn. Tại đây, người dân lựa chọn cách kiên cường đối mặt với các khó khăn sinh hoạt: Họ sẵn lòng chi trả những khoản tiền thuê nhà đắt đỏ để sinh sống trong những căn hộ chật hẹp ở tầng năm của các khu chung cư cũ không có thang máy, chỉ để đổi lấy cơ hội được tiếp cận gần nhất với nguồn năng lượng sống rực rỡ, nghệ thuật, tiền tài và sự điên cuồng của thành phố này.

Đoạn văn văn xuôi sở hữu chất lượng nghệ thuật rất cao làm kinh ngạc giới chuyên môn, chứng minh năng lực của AI hoàn toàn có khả năng viết ra các tác phẩm văn xuôi tinh tế ngang ngửa các nhà văn thực thụ ngoài đời.

## 文摘

1、[Mối đe dọa sinh học đối với sự sống trên Trái Đất khi Mặt Trời đi vào giai đoạn cuối của vòng đời](https://www.space.com/astronomy/when-the-sun-dies-could-life-survive-on-the-jupiter-ocean-moon-europa)

Ước tính sau khoảng 4,5 tỷ năm nữa, Mặt Trời của chúng ta sẽ chính thức bước vào giai đoạn cuối cùng của chu kỳ tiến hóa sao.

Quy trình phản ứng nhiệt hạch hydro bên trong lõi Mặt Trời sẽ không ngừng phình to ra, biến ngôi sao này thành một hành tinh Đỏ khổng lồ (Red Giant). Sự phình to cực đại của đường kính Mặt Trời sẽ nuốt chửng hoàn toàn Sao Thủy và Sao Kim, đồng thời thiêu rụi toàn bộ bề mặt Trái Đất thành tro bụi.

Trong kịch bản tốt nhất, Trái Đất lúc bấy giờ chỉ còn là một khối sắt và niken nguội lạnh không còn sự sống. Trong kịch bản xấu nhất, hành tinh của chúng ta sẽ bị bốc hơi hoàn toàn và biến mất khỏi bản đồ vũ trụ.

Khi nhiệt lượng phát ra từ Mặt Trời phình to tăng mạnh, vùng có thể sinh sống được (Habitable Zone - khu vực xung quanh ngôi sao có nhiệt độ vừa đủ để nước tồn tại ở dạng lỏng trên bề mặt hành tinh) sẽ dịch chuyển dần ra các hành tinh ở vòng ngoài của hệ Mặt Trời.

Tại thời điểm đó, vệ tinh Europa của Sao Mộc sẽ nhận được lượng nhiệt lượng dồi dào. Một phần do bức xạ nhiệt tăng mạnh từ Mặt Trời, phần khác do bản thân Sao Mộc khổng lồ cũng nóng lên phản chiếu thêm nhiều ánh sáng ấm áp chiếu rọi xuống Europa.

Vệ tinh Europa ở thời điểm hiện tại là một thiên thể băng giá lạnh lẽo được bao phủ hoàn toàn bởi lớp vỏ băng dày bên ngoài. Khi nhiệt độ tăng cao trong tương lai, lớp băng bề mặt của Europa sẽ thăng hoa biến mất, giải phóng đại dương nước lỏng khổng lồ ẩn giấu bên dưới lớp băng bốc hơi.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025060401.webp)

(Hình minh họa: Bản vẽ mô phỏng tàu thám hiểm của NASA thực hiện nhiệm vụ bay sát qua bề mặt băng giá của Europa. Tàu thám hiểm đã được phóng thành công vào ngày 14 tháng 10 năm 2024 vừa qua và dự kiến sẽ tiếp cận quỹ đạo Europa vào tháng 4 năm 2030 tới).

Mặt của Europa luôn hướng về phía Sao Mộc do nhận được lượng nhiệt lượng khúc xạ lớn nhất nên sẽ ghi nhận mức tăng nhiệt độ mạnh nhất. Đồng thời, khu vực vành đai xích đạo của vệ tinh cũng đối mặt với tình trạng thoát hơi nước nghiêm trọng ra ngoài không gian.

Tuy nhiên ở khu vực hai cực Nam và Bắc ở mặt lưng không hướng về phía Sao Mộc, nhiệt độ sẽ duy trì ở mức vừa phải và sự thất thoát nước diễn ra chậm hơn nhiều. Các nhà khoa học dự báo tại các khu vực này nhiều khả năng sẽ hình thành nên một lớp khí quyển hơi nước mỏng ổn định.

Trong tương lai xa xôi đó của vũ trụ, Europa rất có thể sẽ trở thành ngôi nhà duy nhất dung dưỡng các mầm sống cuối cùng còn sót lại của hệ Mặt Trời.

## 言论

1、

Hiện nay đang xuất hiện một phong cách lập trình mới mà tôi muốn đặt tên là "Lập trình theo trào lưu" (Hype Coding), dùng để chỉ việc lập trình viên phụ thuộc hoàn toàn vào các công cụ AI theo các bài viết quảng cáo thổi phồng trên truyền thông.

Họ vừa lướt các video ngắn giải trí trên điện thoại, vừa ra lệnh cho một nhóm trợ lý AI tự viết code cho mình. Nếu chương trình phát sinh lỗi, họ chỉ việc yêu cầu AI chạy lại mà hoàn toàn không dành thời gian đọc hiểu các dòng mã nguồn kết xuất ra, chỉ đơn giản copy các đoạn thông báo lỗi ném ngược lại cho AI xử lý cho đến khi chương trình chạy được thì thôi. Nếu cuối cùng vẫn không chạy được, họ đơn giản là dừng lại và chờ đợi thế hệ mô hình AI tiếp theo được phát hành để thử lại.

-- *Simon Willison, nhà phát triển phần mềm nổi tiếng chia sẻ*

2、

Giữa một kỷ nguyên công nghệ nơi máy móc đang liên tục sản xuất hàng loạt các sản phẩm sáng tạo ở mức độ trung bình và thiếu bản sắc, hãy tự tay bắt đầu làm một cái gì đó của riêng mình. Hãy chấp nhận để sản phẩm đó có phần chưa hoàn hảo. Hãy để nó có những nét thô mộc tự nhiên. Việc quan trọng nhất là bạn đã tự mình bắt tay vào hành động thực tế.

-- *Trích bài phân tích 《Giữa thời đại này, hầu như không còn ai bận tâm đến nội dung bạn viết ra nữa》*

3、

Báo cáo nghiên cứu y khoa công bố trên chuyên san tâm lý học cho thấy để một cá nhân hình thành và duy trì được một thói quen sinh hoạt mới trong cuộc sống, trung bình chúng ta cần tới khoảng 66 ngày kiên trì liên tục, và trong một số kịch bản có thể kéo dài tới 8 tháng.

-- *Trích công bố trên Tạp chí Tâm lý học Xã hội Châu Âu*

4、

Thế hệ trẻ lớn lên trong sự đồng hành và phụ thuộc hoàn toàn vào các mô hình AI lớn trong tương lai nhiều khả năng sẽ không còn thấu hiểu được vai trò lịch sử và giá trị thực tế của các thư viện truyền thống đối với nhân loại nữa.

-- *Nhà nghiên cứu Benjamin Breen chia sẻ*

5、

Những thời khắc tươi đẹp và đáng nhớ nhất trong cuộc đời của một người hoàn toàn không phải là những khoảng thời gian chúng ta được thụ động đón nhận các chế độ an nhàn hay thả lỏng tận hưởng cuộc sống, mà chính là những khoảnh khắc chúng ta tự nguyện thử thách bản thân, dốc hết toàn bộ sức lực và trí tuệ để nỗ lực hoàn thành một tác vụ khó khăn nhưng mang lại giá trị thực tế lớn lao cho xã hội.

-- *Mihaly Csikszentmihalyi, nhà tâm lý học lỗi lạc (người đầu tiên đề xuất lý thuyết về trạng thái tâm lý tối ưu Flow - dòng chảy) chia sẻ*

## 往年回顾

- Số #304: [Khám phá kết quả khảo sát về sắc màu được yêu thích nhất trên thế giới](https://www.ruanyifeng.com/blog/2024/06/weekly-issue-304.html)
- Số #254: [Chiêm nghiệm cuộc sống: Thành công của cuộc đời thực chất là bài toán phát huy tối đa ưu thế cạnh tranh của bản thân (Lợi thế tấm ván dài)](https://www.ruanyifeng.com/blog/2023/05/weekly-issue-254.html)
- Số #204: [Chia sẻ các giải pháp tâm lý giúp vượt qua các giai đoạn khó khăn của dịch bệnh, làn sóng sa thải và biến động xã hội](https://www.ruanyifeng.com/blog/2022/04/weekly-issue-204.html)
- Số #154: [Chiêm nghiệm lại các dự báo lịch sử từ năm 1982 về sự hình thành của xã hội thông tin ngày nay](https://www.ruanyifeng.com/blog/2021/04/weekly-issue-154.html)

(Hết)
