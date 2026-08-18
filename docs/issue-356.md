# Bản tin chia sẻ công nghệ (Số 356): Công ty ép dùng AI lập trình, tôi phải làm sao?

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/7169) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070311.webp)

Vào ngày 24 tháng 6 vừa qua, thành phố Thâm Quyến đã tổ chức một buổi diễn tập phòng cháy chữa cháy quy mô lớn, trình diễn công nghệ dùng thiết bị bay không người lái (drones) phun nước dập lửa cho các tòa nhà cao tầng. (Nguồn: [news.cn](https://www.news.cn/gongyi/20250625/932c2d4181b2459396da50a349a5e0be/c.html))

## 公司强推 AI 编程，我该怎么办

Mấy ngày trước, trên diễn đàn Hacker News xuất hiện một bài viết [kêu gọi hỗ trợ từ cộng đồng](https://news.ycombinator.com/item?id=44468375).

Người đăng là một kỹ sư lập trình đang gặp bế tắc khi công ty bắt đầu áp dụng chính sách bắt buộc nhân viên phải lập trình bằng AI, trong khi cá nhân anh lại không muốn sử dụng. Anh đăng bài để hỏi ý kiến mọi người nên xử lý tình huống này thế nào.

Bên dưới bài viết thu hút rất nhiều lượt thảo luận sôi nổi với nhiều góc nhìn thực tế khác nhau. Do đây là một bài toán rất thời sự trong giới công nghệ hiện nay, tôi xin tóm tắt và chia sẻ lại các nội dung cốt lõi của chủ đề này.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070905.webp)

Thực tế của năm 2025 chỉ ra rằng lập trình tích hợp AI (AI Coding) đã bước qua giai đoạn công nghệ thử nghiệm phòng thí nghiệm để trở thành một giải pháp công nghệ chín muồi và không thể né tránh.

Khả năng tự động sinh mã nguồn nhanh chóng đi kèm mức chi phí cực rẻ của AI khiến ban lãnh đạo các doanh nghiệp không thể không đẩy mạnh áp dụng. Điều này đặt các kỹ sư lập trình vào thế tương đối khó xử: Họ vừa phải học cách hợp tác hiệu quả với AI, vừa phải cạnh tranh và phòng ngừa nguy cơ bị chính AI cướp đi cơ hội việc làm.

Nội dung lời cầu cứu của lập trình viên được viết như sau:

> Tôi hiện đang là một kỹ sư phần mềm cao cấp (Senior Engineer) và đã cống hiến cho công ty được 5 năm. Thời gian gần đây ban lãnh đạo công ty đang chuyển sang thần thánh hóa phong cách phát triển nhanh (Vibe Coding), cả CEO và CTO đều tỏ ra mê mẩn các tính năng lập trình tự động của AI.
>
> Công ty đã ban hành chính sách bắt buộc mọi lập trình viên phải lập trình bằng AI, thậm chí yêu cầu để AI tự động sinh các đoạn mã kiểm thử đơn vị (Unit Tests). Khi phát hiện các lỗi kiểm thử không thông qua (failed tests), quy định yêu cầu kỹ sư ném thẳng lỗi cho AI tự sửa thay vì tự mình tìm hiểu nguyên nhân và sửa thủ công, mục đích để đẩy nhanh tốc độ hoàn thiện sản phẩm ra mắt thị trường.
>
> Tôi đang cân nhắc nghiêm túc việc nộp đơn xin từ chức vì không muốn bản thân bị cuốn vào quy trình làm việc tẻ nhạt này, biến mình từ một kỹ sư viết code thực thụ thành một "kỹ sư viết câu lệnh nhắc" (Prompt Engineer) chỉ biết gõ lệnh cho AI làm việc, và bất lực nhìn bộ kỹ năng lập trình của bản thân ngày một thui chột và lạc hậu. Tôi cũng không muốn trong 2, 3 năm tới phải gánh chịu hậu quả đi bảo trì một đống mã nguồn rác lộn xộn (spaghetti code) do AI sinh ra.
>
> Rất mong nhận được những lời khuyên hữu ích từ mọi người về cách thức đối phó với chính sách ép dùng AI của công ty.

Tổng hợp lại toàn bộ các ý kiến phản hồi của cộng đồng, chúng ta có thể chia các đề xuất thành 3 hướng lựa chọn thực tế dưới đây. Mỗi hướng đi đều sở hữu những lập luận thuyết phục riêng. Nếu rơi vào hoàn cảnh này, bạn sẽ quyết định thế nào?

### Hướng lựa chọn 1: Lắng nghe tiếng nói cá nhân

Nếu bạn thực sự cảm thấy ngột ngạt và kiệt sức với môi trường hiện tại thì giải pháp tốt nhất là lựa chọn rời đi. Ngay cả khi bạn cố gắng chịu đựng để làm một công việc mình ghét hằng ngày, trạng thái kiệt sức (burnout) cũng sẽ sớm gõ cửa.

Tình huống tồi tệ nhất là việc hằng ngày bạn phải cố gắng giả vờ tỏ ra tràn đầy nhiệt huyết với công nghệ AI trước mặt ban lãnh đạo để đối phó, trong khi thâm tâm lại hoàn toàn phản đối, đó sẽ là một sự tra tấn tinh thần cực kỳ nặng nề.

Việc phó mặc hoàn toàn cho AI viết code sẽ nhanh chóng tích tụ các khoản nợ kỹ thuật (Technical Debt) khổng lồ cho hệ thống, đưa dự án đến bờ vực đổ vỡ. Sớm muộn gì công ty cũng sẽ yêu cầu bạn đứng ra dọn dẹp đống lộn xộn do AI gây ra. Tại thời điểm đó nếu bạn báo cáo giải pháp duy nhất là phải đập đi viết lại thủ công toàn bộ mã nguồn, bạn vẫn đối mặt với nguy cơ bị sa thải như thường.

Đồng thời, một ban lãnh đạo gồm CEO và CTO mù quáng tin tưởng tuyệt đối vào AI như vậy cũng là tín hiệu cảnh báo về tương lai không mấy tươi sáng của doanh nghiệp.

Hiện tại vẫn có những doanh nghiệp tuyên bố rõ ràng quan điểm không sử dụng mã nguồn do AI viết cho các hệ thống vận hành chính thức (production code), bạn hoàn toàn có thể tìm kiếm các cơ hội việc làm tại các đơn vị này.

Tuy nhiên nếu chưa tích lũy đủ nguồn tài chính dự phòng an toàn, bạn nên cố gắng nhẫn nhịn thêm vài tháng, vừa làm việc tích lũy tài chính, vừa chủ động tìm kiếm cơ hội mới và dành thời gian rèn luyện thêm các kỹ năng kỹ thuật phức tạp khó bị thay thế bởi AI. Hãy luôn ghi nhớ: Trừ khi bạn là một ngôi sao công nghệ xuất chúng hoặc sở hữu tiềm lực tài chính dư dả, đừng bao giờ vội vã từ chức khi chưa cầm chắc trong tay một lời mời tuyển dụng mới.

### Hướng lựa chọn 2: Chấp nhận thực tế cuộc chơi

Dù bạn có chuyển dịch sang các doanh nghiệp khác thì thực tế cũng tương tự, bởi làn sóng ứng dụng AI trong lập trình hiện đã lan rộng ra khắp nơi. Nhiều doanh nghiệp thậm chí còn coi việc áp dụng AI là một bộ lọc tự nhiên để đào thải những nhân sự bảo thủ từ chối đổi mới.

Chúng ta sẽ không bao giờ có thể quay trở lại thời kỳ lập trình truyền thống trước đây nữa, một khi đã quen với hiệu suất của AI bạn sẽ thấy không thể quay đầu lại. Thế hệ kỹ sư lập trình tiếp theo sẽ lớn lên dưới sự đồng hành tự nhiên của AI. Việc bạn từ chối sử dụng AI lập trình tương tự như việc bạn cố chấp từ chối dùng máy tính để tiếp tục gõ văn bản bằng máy đánh chữ cổ điển vậy. Sự phổ cập của AI lập trình chỉ là bài toán thời gian, và những ai từ chối thích nghi chắc chắn sẽ bị đào thải.

Hơn nữa, đây là cơ hội tốt khi công ty đang chi trả tiền lương hằng tháng để bạn có điều kiện học tập và thực hành các công nghệ AI mới. Hãy thông minh tận dụng cơ hội này để nâng cao giá trị bản thân.

Thị trường lao động hiện nay đang thuộc về nhóm người sử dụng lao động, luôn có sẵn vô số ứng viên sẵn sàng thế chỗ của bạn. Dù bạn có may mắn tìm được một công ty hiện chưa áp dụng AI, điều đó nhiều khả năng phản ánh doanh nghiệp đó đang tụt hậu sâu so với thời đại, và họ cũng sẽ sớm phải chuyển dịch sang AI trong tương lai gần mà thôi.

Giải pháp tốt nhất là học cách thích nghi với thực tế để tìm kiếm chỗ đứng vững chắc cho mình. Ngay cả khi chưa chấp nhận về mặt tâm lý, hãy coi đây là cơ hội dùng ngân sách của công ty để trải nghiệm các công nghệ mới.

Bạn có thể bắt đầu bằng việc áp dụng AI ở một số phần việc nhỏ, sau đó dành thời gian kiểm soát kỹ lưỡng các đoạn mã do AI viết ra. Mã nguồn do AI viết luôn đòi hỏi quy trình rà soát và tái cấu trúc (refactoring) rất lớn từ con người, và giá trị chuyên môn của bạn nằm ở chính quy trình kiểm soát chất lượng này.

### Hướng lựa chọn 3: Lặng lẽ quan sát và chờ đợi thời cơ

Bạn có thể lựa chọn tiếp tục ở lại doanh nghiệp, vừa làm việc vừa tích cực học tập các công nghệ AI mới cùng các kỹ năng kỹ thuật khác, đồng thời lặng lẽ quan sát xem diễn biến tiếp theo của doanh nghiệp sẽ đi về đâu.

Nếu kết quả thực tế của công ty tiến triển tốt hơn mong đợi, AI hoạt động hiệu quả giúp dự án thành công, điều đó chứng minh bạn cần thay đổi tư duy cá nhân để chủ động chuẩn bị cho một phương thức làm việc mới.

Nếu diễn biến đúng như dự báo của bạn: Chất lượng mã nguồn của hệ thống nhanh chóng xuống cấp nghiêm trọng và dự án đi đến thất bại. Lúc này bạn đã tích lũy được nhiều kinh nghiệm thực tế quý báu về việc ứng dụng AI, thấu hiểu tường tận các ưu thế và nhược điểm thực tế của AI khi áp dụng ngoài thực địa. Hãy đưa các kinh nghiệm thực tế này vào hồ sơ cá nhân để làm bàn đạp tìm kiếm các cơ hội việc làm tốt hơn ở các công ty tiếp theo.

Bất kể kết quả thế nào, khoảng thời gian vài tháng tiếp theo bạn chọn ở lại công ty để trải nghiệm và quan sát chắc chắn sẽ mang lại nhiều bài học giá trị cho sự nghiệp lâu dài của bạn.

Tất nhiên song song với quá trình đó, bạn nên âm thầm bắt đầu quy trình tìm kiếm các cơ hội việc làm mới phù hợp hơn với định hướng cá nhân để chủ động đối phó với các tình huống xấu có thể xảy ra.

## 科技动态

（1）Thiết kế giao diện "Kính lỏng" mới của Apple từng gây tranh cãi khi thực hiện việc lật ngược chiều **biểu tượng Finder trên macOS** từ trái sang phải ở bản beta đầu tiên.

Sau khi vấp phải nhiều ý kiến thắc mắc từ người dùng, Apple đã quyết định đưa biểu tượng về chiều truyền thống cũ ở bản cập nhật beta tiếp theo.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025062603.webp)

Bức hình phía trên so sánh: Bên trái là biểu tượng Finder truyền thống, ở giữa là thiết kế lật ngược ở bản thử nghiệm đầu tiên, và bên phải là thiết kế điều chỉnh cuối cùng ở bản beta thứ hai.

Biểu tượng mới vẫn giữ phong cách chất liệu kính lỏng bóng bẩy và nhận được nhiều phản hồi tích cực.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025062604.webp)

（2）Một kỹ sư người Bỉ vừa phát triển thành công ứng dụng chạy trên kính AR hỗ trợ **nhận diện và tự động che chắn các biển quảng cáo dọc đường đi** (Real-world Ad Block) thời gian thực.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025062902.webp)

Mỗi khi phát hiện ra sự xuất hiện của các biển quảng cáo, hệ thống sẽ tự động phủ một lớp màu đỏ đè lên vị trí đó, giúp người dùng hoàn toàn không bị làm phiền bởi các thông tin quảng cáo ngoài đời thực.

Đây được đánh giá là một ứng dụng mang tính thực tiễn và sáng tạo rất cao của công nghệ AR.

（3）Truyền thông đưa tin về câu chuyện của **một lập trình viên 41 tuổi tại Thâm Quyến** đã quyết định từ bỏ việc thuê nhà để chuyển sang sinh hoạt ngay trên chiếc xe hơi của mình suốt 3 năm qua.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070307.webp)

Gia đình anh sinh sống tại thành phố Dương Giang cách Thâm Quyến khoảng 300 km. Cuối tuần anh sẽ lái xe về thăm vợ con, còn những ngày trong tuần anh làm việc và ngủ nghỉ trực tiếp trên xe.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070309.webp)

Anh chia sẻ trước đây chi phí thuê một phòng trọ nhỏ chật hẹp với điều kiện vệ sinh kém tại Thâm Quyến ngốn khoảng 2.500 Nhân dân tệ hằng tháng. Hiện tại anh cảm thấy cuộc sống trên xe rất thoải mái khi xe trang bị hệ thống điều hòa mát mẻ.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070310.webp)

Chi phí đỗ xe qua đêm tại công viên chỉ tốn 6 Nhân dân tệ hằng ngày, và anh sử dụng nhà vệ sinh công cộng để vệ sinh cá nhân cơ bản (hình trên). Hằng ngày sau giờ làm việc anh đến phòng tập gym để tập luyện và tắm rửa sạch sẽ trước khi lái xe về công viên đi ngủ. Lượng quần áo bẩn sẽ được anh gom lại để mang về nhà giặt vào cuối tuần.

（4）Hãng xe điện **Tesla** tuần trước đã triển khai thử nghiệm quy trình giao xe tự động hoàn toàn (FSD) cho khách hàng mà không cần nhân viên đi cùng.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070102.webp)

Chiếc xe mới sau khi xuất xưởng đã tự động kích hoạt hệ thống tự lái để tự di chuyển hành trình dài 30 phút đi qua cả đoạn đường cao tốc phức tạp để đỗ chính xác trước cửa nhà khách hàng mua xe.

（5）Chính quyền Mỹ chính thức đưa vào vận hành khu giam giữ đặc biệt mang tên "**Đảo cá sấu**" (Alligator Island) chuyên dụng phục vụ việc tạm giam những người nhập cư trái phép.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070202.webp)

Khu giam giữ được thiết lập ngay trên đường băng của một sân bay quân sự bỏ hoang thuộc khu vực khí hậu nhiệt đới của bang Florida.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070203.webp)

Khu vực này hoàn toàn không cần xây dựng hệ thống tường bao kiên cố, bởi xung quanh là vùng đầm lầy ngập nước rộng lớn (hình trên) — nơi cư ngụ của hàng vạn con cá sấu hoang dã hung dữ, khiến việc vượt ngục trốn chạy bằng đường bộ là điều hầu như không thể thực hiện. Ý tưởng tận dụng địa hình tự nhiên này để làm nơi giam giữ thực sự khiến nhiều người kinh ngạc.

（6）Tập đoàn Microsoft chính thức bổ sung quy định đánh giá năng lực nhân viên mới, quy định **đo đạc và đánh giá tần suất khai thác các công cụ AI** trong công việc hằng ngày của nhân sự như một chỉ tiêu đánh giá hiệu quả bắt buộc.

## 文章

1、[Giới thiệu nguyên lý hoạt động của cấu trúc bộ lọc Bloom Filters qua ví dụ minh họa](https://llimllib.github.io/bloomfilter-tutorial/zh_CN/) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025063007.webp)

Bài viết hướng dẫn cơ bản giới thiệu về cấu trúc dữ liệu Bloom Filters — một giải pháp toán học hiệu quả chuyên dụng để kiểm tra nhanh sự tồn tại của một phần tử bên trong một tập hợp dữ liệu lớn.

2、[Hướng dẫn chi tiết quy trình toán học chứng minh công thức xấp xỉ Stirling](https://www.longluo.me/blog/stirlings-formula/) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070801.webp)

Bài viết phổ biến kiến thức toán học giới thiệu về công thức Stirling — một công thức toán học quan trọng chuyên dùng để tính nhanh giá trị giai thừa của các số lớn ($n!$). Tác giả nỗ lực sử dụng ngôn ngữ trực quan để giải thích quy trình chứng minh công thức này. (Đóng góp từ [@longluo](https://www.longluo.me/blog/stirlings-formula/))

3、[Tại sao các chuyên gia Git nên tìm hiểu và trải nghiệm công cụ Jujutsu](https://pksunkara.com/thoughts/git-experts-should-try-jujutsu/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070515.webp)

Jujutsu là một công cụ giao diện dòng lệnh mới (CLI frontend) được thiết kế hoạt động tương thích hoàn toàn trên nền tảng kho chứa của Git. Bài viết phân tích các ưu thế của Jujutsu khi giúp đơn giản hóa đáng kể các thao tác câu lệnh phức tạp của Git.

4、[Đánh giá trải nghiệm thực tế công cụ chạy container native Apple Container trên macOS](https://www.xda-developers.com/apple-container-turned-my-mac-into-a-self-hosting-war-machine/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025062704.webp)

Việc vận hành các container Docker trên hệ điều hành macOS từ trước đến nay luôn ngốn rất nhiều tài nguyên phần cứng. Apple mới đây đã cho ra mắt công cụ chạy container native là Apple Container để giải quyết bài toán này. Tác giả chia sẻ các đánh giá thực tế và chỉ ra những hạn chế hiện tại của công cụ mới.

5、[Các giải pháp kỹ thuật xác định trạng thái kết nối mạng của thiết bị](https://antonz.org/is-online/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070903.webp)

Bài hướng dẫn giới thiệu phương pháp lập trình gửi nhanh các yêu cầu kết nối HTTP ngắn đến các địa chỉ máy chủ chuyên dụng (tiêu biểu như `google.com/generate_204`) để xác định chính xác thiết bị hiện tại có đang kết nối internet hay không.

6、[Cảnh báo bảo mật: Những thông tin cá nhân có thể bị rò rỉ thông qua danh sách bài viết yêu thích](https://noperator.dev/posts/o3-pocket-profile/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070904.webp)

Tác giả đã thử nghiệm xuất toàn bộ danh sách gần 900 bài viết anh từng lưu và yêu thích trên ứng dụng Pocket suốt 7 năm qua để gửi lên mô hình AI o3, yêu cầu AI phân tích sâu về đặc điểm tính cách và thông tin cá nhân của chủ tài khoản.

Kết quả nhận về khiến tác giả vô cùng chấn động khi mô hình AI đã kết xuất ra một bản phân tích dài hơn 2.000 chữ phác họa cực kỳ chuẩn xác các thông tin đời tư, sở thích và tính cách thực tế của anh.

7、[Giải pháp xác định tọa độ vị trí của Trạm Vũ trụ Quốc tế ISS thông qua truy vấn hệ thống DNS](https://shkspr.mobi/blog/2025/07/get-the-location-of-the-iss-using-dns/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070702.webp)

Bài viết hướng dẫn một mẹo kỹ thuật khai thác bản ghi LOC (Location) trong hệ thống phân giải tên miền DNS để xác định chính xác kinh độ và vĩ độ của máy chủ, và ứng dụng nó để cung cấp thông tin vị trí thời gian thực của trạm không gian ISS.

## 工具

1、[giscus](https://giscus.app/zh-CN)

Hệ thống bình luận trực quan dành cho các trang web tĩnh hoạt động dựa trên nền tảng tính năng thảo luận GitHub Discussions.

2、[phpIPAM](https://phpipam.net/)

Ứng dụng quản trị hệ thống mã nguồn mở hỗ trợ theo dõi và quản lý tập trung toàn bộ dải địa chỉ IP của các thiết bị trong mạng nội bộ thông qua giao diện Web trực quan. Xem thêm bài viết [hướng dẫn cài đặt và sử dụng](https://www.xda-developers.com/phpipam-track-your-self-hosted-services/).

3、[NumPad](https://numpad.io/)

Dịch vụ ghi chép trực tuyến tối giản hỗ trợ người dùng thực hiện nhanh các phép toán ngay trên giao diện soạn thảo văn bản (nhập `1 + 1` hệ thống sẽ tự động hiển thị kết quả `2`).

4、[LiteOps](https://github.com/opsre/LiteOps)

Hệ thống DevOps mã nguồn mở gọn nhẹ tự lưu trữ hỗ trợ quản lý các quy trình CI/CD tự động cho các dự án phần mềm. (Đóng góp từ [@hukdoesn](https://github.com/ruanyf/weekly/issues/7203))

5、[Ech0](https://github.com/lin-snow/Ech0)

Dự án phần mềm hỗ trợ người dùng tự dựng một trang nhật ký cá nhân (Microblog) tối giản, tham khảo giao diện chạy mẫu tại [memo.vaaat.com](https://memo.vaaat.com/). (Đóng góp từ [@lin-snow](https://github.com/ruanyf/weekly/issues/7205))

6、[PageTemplatify](https://github.com/GeekAtTeam/PageTemplatify)

Công cụ hỗ trợ tạo nhanh các trang giao diện HTML tĩnh dựa trên kho biểu mẫu thiết kế có sẵn phục vụ công tác kiểm thử nhanh. (Đóng góp từ [@luhuadong](https://github.com/ruanyf/weekly/issues/7210))

7、[REM](https://github.com/liriliri/rem)

Ứng dụng quản lý tệp tin đa nền tảng hoạt động dựa trên công cụ Rclone, hỗ trợ người dùng quản lý và truyền nhận dữ liệu qua lại giữa nhiều tài khoản lưu trữ đám mây khác nhau trên một giao diện duy nhất. (Đóng góp từ [@surunzi](https://github.com/ruanyf/weekly/issues/7222))

8、[OnlyOffice Web](https://github.com/ranuts/document)

Dự án biên dịch bộ công cụ văn phòng OnlyOffice sang định dạng WebAssembly (WASM), cho phép người dùng mở và biên tập trực tiếp các tệp tin Word, Excel, PowerPoint ngay trên trình duyệt máy khách mà hoàn toàn không cần kết nối máy chủ xử lý. Trải nghiệm trực tuyến tại [ranuts.github.io/document](https://ranuts.github.io/document/). (Đóng góp từ [@chaxus](https://github.com/ruanyf/weekly/issues/7213))

9、[Công cụ ghép ảnh trực tuyến](https://img.ops-coffee.cn/zh/)

Dịch vụ web miễn phí hỗ trợ người dùng ghép nhanh nhiều hình ảnh nhỏ thành một bức ảnh lớn theo các bố cục đa dạng. (Đóng góp từ [@ops-coffee](https://github.com/ruanyf/weekly/issues/7217))

10、[Portfolio](https://github.com/austenstone/portfolio)

Mẫu thiết kế trang web giới thiệu năng lực cá nhân (Portfolio) chuyên nghiệp được xây dựng trên bộ khung trang tĩnh Docusaurus, xem giao diện chạy thực tế tại [austen.info/blog](https://austen.info/blog).

11、[Postcard](https://postcard.page)

Dự án mã nguồn mở hỗ trợ người dùng tự thiết lập trang web cá nhân kết hợp cùng hệ thống gửi bản tin tin tức (Newsletter) tự động. Xem thêm bài viết [giới thiệu chi tiết của tác giả](https://www.contraption.co/postcard-open-source/).

## AI 相关

1、[OpenCode](https://github.com/sst/opencode)

Bộ công cụ dòng lệnh kết nối AI mã nguồn mở hỗ trợ tương tác trực tiếp với các mô hình ngôn ngữ lớn để quản lý và chỉnh sửa tệp tin, được thiết kế như một giải pháp thay thế tự chủ cho Claude Code và không giới hạn nhà cung cấp AI.

2、[Simple Chromium AI](https://github.com/kstonekuan/simple-chromium-ai)

Kể từ phiên bản 138, trình duyệt Chrome đã được tích hợp sẵn mô hình AI Gemini Nano cục bộ đi kèm bộ API kết nối. Thư viện mã nguồn mở này giúp đơn giản hóa và tối ưu hóa các thao tác gọi bộ API AI Prompt của trình duyệt.

3、[TouchFS](https://github.com/kristerhedfors/touchfs)

Công cụ dòng lệnh AI độc đáo: Khi người dùng khởi tạo một tệp tin mới (ví dụ gõ câu lệnh `touch README.md`), hệ thống AI sẽ tự động phân tích tên tệp và tự động viết trước các nội dung mẫu tương ứng vào bên trong tệp tin đó.

4、[yutu](https://github.com/eat-pray-ai/yutu)

Dự án xây dựng cổng kết nối giao thức MCP dành cho nền tảng chia sẻ video YouTube, hỗ trợ các trợ lý AI tự động thực hiện các thao tác tìm kiếm và truy xuất thông tin trên YouTube bằng ngôn ngữ tự nhiên. (Đóng góp từ [@OpenWaygate](https://github.com/ruanyf/weekly/issues/7214))

5、[Pointer](https://github.com/experdot/pointer)

Ứng dụng máy tính hỗ trợ kết nối trò chuyện AI với tính năng quản lý lịch sử trò chuyện theo cấu trúc thư mục khoa học, hỗ trợ tìm kiếm toàn văn và phân tích dữ liệu trực quan. (Đóng góp từ [@experdot](https://github.com/ruanyf/weekly/issues/7241))

6、[TTS Omni](https://www.ttsomni.com/)

Dịch vụ chuyển đổi văn bản thành giọng nói (Text-to-Speech) miễn phí chất lượng cao hoạt động dựa trên mô hình Qwen-TTS mới công bố. (Đóng góp từ [@CurioChen77](https://github.com/ruanyf/weekly/issues/7209))

## 资源

1、[Bản đồ nhiệt độ toàn cầu (Zoom Earth)](https://zoom.earth/maps/temperature/)

Bản đồ tương tác trực quan hỗ trợ người dùng theo dõi các dữ liệu về nhiệt độ và thời tiết khí hậu thời gian thực trên khắp thế giới. (Đóng góp từ [@Codeniu](https://github.com/ruanyf/weekly/issues/7219))

2、[Thư viện chia sẻ các mẫu quy trình tự động hóa n8n](https://n8nworkflow.net/zh)

Nền tảng n8n là công cụ lập trình quy trình tự động hóa mã nguồn mở rất phổ biến. Trang web này chuyên tổng hợp và chia sẻ hơn 2.000 mẫu quy trình n8n được thiết lập sẵn phục vụ nhiều tác vụ đa dạng. (Đóng góp từ [@panyanyany](https://github.com/ruanyf/weekly/issues/7227))

Tham khảo thêm bài hướng dẫn [kết hợp n8n và Notion](https://www.xda-developers.com/combined-notion-with-n8n-automate-bookmarking/) để tự thiết lập quy trình tự động lưu trữ các đường dẫn web yêu thích về cơ sở dữ liệu Notion.

3、[Cơ chế phối màu tối giản 4 màu (4 colors)](https://www.iamsajid.com/colors/)

Trang web chia sẻ triết lý thiết kế giao diện tối giản chỉ cần khai thác tối đa 4 tông màu chính: Màu tiền cảnh (Foreground), màu nền (Background), màu nhấn (Accent) và màu điểm xuyết (Cool color). Dịch vụ hỗ trợ người dùng tự động sinh các bảng phối màu tương thích theo triết lý này.

## 图片

1、[Mẫu ghế thiết kế Rubik độc đáo](https://mossandfog.com/rubiks-cube-chair-makes-you-work-for-your-seat/)

Một nhà thiết kế nước ngoài vừa giới thiệu tác phẩm ghế ngồi mô phỏng khối Rubik độc đáo:

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070506.webp)

Toàn bộ chiếc ghế chính là một khối Rubik khổng lồ, và người dùng bắt buộc phải xoay giải hoàn thành khối Rubik này để tạo nên một mặt phẳng vững chắc trước khi ngồi lên.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070507.webp)

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070508.webp)

Trên thực tế, người dùng chỉ cần xoay để đưa 4 chân ghế về cùng một mặt phẳng là chiếc ghế đã có thể sử dụng được.

2、[Tác phẩm sách có quy mô đồ sộ nhất trong lịch sử Trung Quốc](https://www.baijiayoupu.com/c/6599.html)

Cuốn sách giấy có kích thước lớn và nặng nhất được ghi nhận tại Trung Quốc là cuốn gia phả hoàng tộc "Ngọc Diệp" (玉牒) được biên soạn dưới triều đại nhà Thanh. Mỗi tập sách sở hữu độ dày lên tới 85 cm và nặng khoảng 90 kg.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071004.webp)

Cuốn sách ghi chép chi tiết gia phả của hoàng gia với danh sách hơn 100.000 thành viên nam giới thuộc tôn thất nhà Thanh do Tông Nhân Phủ chịu trách nhiệm biên soạn, hiện đang được bảo quản nghiêm ngặt tại Viện Lưu trữ Lịch sử Số 1 Trung Quốc tại Bắc Kinh.

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025071005.webp)

## 文摘

1、**Máy tính tương tự như chiếc xe đạp**

*Trích dịch chia sẻ của Steve Jobs trong cuộc phỏng vấn năm 1980:*

![](https://cdn.beekka.com/blogimg/asset/202507/bg2025070901.webp)

Tôi còn nhớ vào năm khoảng 12 tuổi, tôi có cơ hội đọc được một bài phân tích rất thú vị trên tạp chí khoa học *Scientific American*.

Bài viết thực hiện các đo đạc so sánh về mức độ hiệu quả năng lượng khi di chuyển của các sinh vật trên Trái Đất — tính toán xem với cùng một cự ly di chuyển từ điểm A đến điểm B, mỗi loài sinh vật tiêu tốn bao nhiêu năng lượng cơ thể.

Kết quả đo đạc cho thấy loài chim kền kền xếp ở vị trí dẫn đầu bảng xếp hạng nhờ khả năng bay lượn tận dụng luồng gió cực kỳ tiết kiệm năng lượng. Trong khi đó loài người chúng ta lại xếp ở nhóm 1/3 cuối bảng xếp hạng — một kết quả tương đối khiêm tốn đối với sinh vật tự nhận là "chúa tể muôn loài".

Tuy nhiên tác giả bài viết đã có một ý tưởng so sánh rất độc đáo khi tiến hành đo đạc thêm hiệu suất di chuyển của con người khi kết hợp sử dụng xe đạp. Kết quả thật kinh ngạc khi hiệu suất của con người lúc này vọt lên dẫn đầu bảng xếp hạng và bỏ xa loài chim kền kền.

Chi tiết này đã để lại cho tôi một ấn tượng cực kỳ sâu sắc suốt cuộc đời. Bản chất của loài người chúng ta là những sinh vật biết chế tạo và sử dụng công cụ. Chúng ta có khả năng sáng tạo ra các công cụ giúp nhân rộng năng lực tự nhiên của bản thân lên gấp vô số lần.

Đối với tôi, chiếc máy tính cá nhân chính là chiếc "xe đạp cho trí tuệ" của con người. Nó là công cụ giúp giải phóng và khuếch đại năng lực tư duy của chúng ta vượt qua các giới hạn tự nhiên.

Tôi nhận định nhân loại hiện nay mới chỉ đang ở những bước đi chập chững đầu tiên của kỷ nguyên máy tính — một giai đoạn rất sơ khởi. Chúng ta mới đi được một chặng đường ngắn, công nghệ máy tính vẫn đang tiếp tục tiến hóa mạnh mẽ, nhưng những thay đổi vĩ đại nó mang lại cho xã hội đã là vô cùng khổng lồ.

Tôi tin rằng những thành tựu công nghệ chúng ta đang chứng kiến hiện nay sẽ chỉ là một hạt cát nhỏ bé nếu đặt lên bàn cân so sánh với những bước phát triển vĩ đại của máy tính trong một trăm năm tới.

## 言论

1、

Trong suốt hành trình sự nghiệp dài hạn, bạn đã dành vô vàn mồ hôi công sức để rèn luyện kỹ năng và tự hào định vị bản thân là một kỹ sư lập trình chuyên nghiệp. Viết code đã trở thành một phần cốt lõi cấu thành nên danh tính cá nhân và là nguồn sống tạo nên giá trị cuộc sống của bạn. Rồi đột nhiên các công cụ AI xuất hiện và dễ dàng làm thay thế hầu hết các kỹ năng đó, khiến cảm giác về giá trị cá nhân của bạn bị lung lay dữ dội. Đây chính là nguyên nhân sâu xa giải thích tại sao nhiều lập trình viên kỳ cựu lại tỏ ra bài xích và phản đối AI dữ dội đến vậy.

-- *Trích bài viết 《Khi AI có khả năng tự viết code, kỹ sư lập trình còn lại giá trị gì?》*

2、

Bài toán giao thông nan giải của thành phố Los Angeles nằm ở quy mô diện tích quá rộng lớn và phân tán, trong khi hệ thống giao thông công cộng lại cực kỳ nghèo nàn buộc mọi người phải tự lái xe cá nhân. Thực trạng này vô tình triệt tiêu hoàn toàn cơ hội để bạn tình cờ gặp gỡ những con người thú vị ngoài đường phố, bởi tất cả mọi người đều đang bị cô lập bên trong chiếc hộp xe hơi của mình.

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

- Số #309: [Thảo luận chuyên sâu về hai mặt lợi và hại của làn sóng dịch vụ xe taxi tự lái (Robotaxi)](https://www.ruanyifeng.com/blog/2024/07/weekly-issue-309.html)
- Số #259: [Tổng hợp các phương thức khai thác và sử dụng dịch vụ ChatGPT hoàn toàn miễn phí](https://www.ruanyifeng.com/blog/2023/06/weekly-issue-259.html)
- Số #209: [Phác họa bức chân dung chân thực về tính cách và thói quen làm việc của giới lập trình viên](https://www.ruanyifeng.com/blog/2022/06/weekly-issue-209.html)
- Số #159: [Khảo sát thực tế về thu nhập hằng năm của các nhà phát triển game trên thế giới](https://www.ruanyifeng.com/blog/2021/05/weekly-issue-159.html)

(Hết)
