# Bản tin chia sẻ công nghệ (Số 332): Tổng kết năm của Simon Willison, cuộc đối thoại cùng Lương Văn Phong

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/5830) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010104.webp)

"Đường hầm chiến thắng Thiên Sơn" — đường hầm cao tốc dài nhất thế giới — đã chính thức được thông xe kỹ thuật vào tuần này. Công trình có tổng chiều dài lên tới 22,13 km, các phương tiện sẽ mất khoảng 20 phút di chuyển liên tục bên trong hầm. Dự án giao thông trọng điểm này giúp kết nối thông suốt hai khu vực Nam Cương và Bắc Cương vốn bị chia cắt hoàn toàn bởi dãy núi Thiên Sơn hiểm trở. (Nguồn: [cjn.cn](http://news.cjn.cn/bsy/gnxw_19788/202412/t5064119.htm))

## 西蒙·威利森的年终总结，梁文锋的访谈

Lập trình viên người Anh Simon Willison trong hai năm trở lại đây đã trở nên vô cùng nổi tiếng trong cộng đồng công nghệ thế giới. [Trang blog cá nhân](https://simonwillison.net) của anh liên tục đăng tải các bài viết phân tích sâu sắc cập nhật các bước tiến mới nhất của lĩnh vực AI.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010216.webp)

Tuần này, anh đã phát hành một bài viết tổng hợp vô cùng dài mang tên [Nhìn lại thị trường mô hình ngôn ngữ lớn năm 2024](https://simonwillison.net/2024/Dec/31/llms-in-2024/) (bản dịch tiếng Trung phi chính thức [tại đây](https://www.163.com/dy/article/JKTHVG4C0511AQHO.html)), nội dung vô cùng xuất sắc.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010217.webp)

Trong bài viết, Simon nhấn mạnh rằng tốc độ phát triển của công nghệ AI đang diễn ra nhanh đến mức vượt ngoài mọi trí tưởng tượng của con người.

Chỉ mới cách đây một năm (vào cuối năm 2023), mô hình AI thống trị tuyệt đối thị trường là GPT-4 của OpenAI, và hầu như không có bất kỳ mô hình đối thủ nào có thể bắt kịp hiệu năng của nó.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010218.webp)

Tuy nhiên, chỉ sau một năm ngắn ngủi, các bạn có đoán được vị trí thứ hạng hiện tại của GPT-4 trên [bảng xếp hạng hiệu năng thế giới](https://lmarena.ai/?leaderboard) là bao nhiêu không?

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010219.webp)

Câu trả lời là vị trí thứ 69 (hình trên). Hiện tại đã có tới 18 nhà phát triển mô hình lớn khác nhau tự tin vượt qua hiệu năng của GPT-4 thế hệ đầu. Thậm chí, một số mô hình thế hệ mới với hiệu năng vượt trội còn có khả năng vận hành trực tiếp trên các dòng máy tính xách tay cá nhân của người dùng.

Chỉ trong vòng 12 tháng, mô hình hàng đầu đã bị hàng loạt đối thủ vượt mặt dễ dàng, và phần cứng gia đình thông thường cũng đã có thể vận hành các mô hình có năng lực xử lý tương đương. Tốc độ tiến hóa công nghệ này thực sự đáng kinh ngạc.

Đặc biệt, Simon Willison đã dành sự chú ý lớn đến mô hình lớn mới ra mắt từ Trung Quốc mang tên **DeepSeek V3**.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010220.webp)

Mô hình DeepSeek V3 chính thức được ra mắt vào ngày 25 tháng 12 năm 2024 bởi High-Flyer Quant (幻方量化) — một công ty quản lý quỹ định lượng có trụ sở tại Hàng Châu. Ngay khi vừa xuất hiện, DeepSeek V3 đã lập tức tạo nên cơn địa chấn chấn động giới công nghệ toàn cầu.

Mô hình này đã vượt qua dòng mô hình o1 mới nhất của OpenAI trên nhiều chỉ số kiểm thử hiệu năng độc lập. Hiện tại, DeepSeek V3 đang xếp vị trí thứ 7 trên bảng xếp hạng thế giới. Điều đáng nói là trong số top 10 mô hình mạnh nhất toàn cầu, DeepSeek V3 là **mô hình duy nhất được phát hành dưới dạng mã nguồn mở** (chia sẻ miễn phí tại [GitHub](https://github.com/deepseek-ai/DeepSeek-V3)) với giấy phép MIT vô cùng thông thoáng, trong khi các mô hình còn lại đều là các sản phẩm đóng độc quyền của các tập đoàn công nghệ khổng lồ.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010221.webp)

Không những thế, DeepSeek V3 sở hữu hiệu năng vận hành và tối ưu hóa chi phí huấn luyện vô cùng ấn tượng. Ước tính chi phí để huấn luyện mô hình này chỉ bằng 1/11 so với chi phí Meta bỏ ra để huấn luyện Llama 3.1 405B, trong khi hiệu năng đầu ra của Llama 3.1 thậm chí còn kém hơn. Điều này chứng minh đội ngũ kỹ sư DeepSeek đã tìm ra các giải pháp đột phá giúp tối ưu hóa phần cứng và nâng cao hiệu suất mô hình cực kỳ xuất sắc.

Simon Willison nhận định: "Chi phí huấn luyện của DeepSeek V3 chỉ rơi vào khoảng dưới 6 triệu USD. Đây là một tín hiệu vô cùng khả quan chứng minh chi phí huấn luyện các mô hình AI hoàn toàn có thể và chắc chắn sẽ còn tiếp tục giảm mạnh trong tương lai."

Giới truyền thông phương Tây hiện đang vô cùng tò mò: Làm thế nào DeepSeek có thể đạt được kỳ tích này?

Nhà sáng lập High-Flyer Quant — Lương Văn Phong (Liang Wenfeng) — sở hữu một lý lịch khác biệt hoàn toàn với đại bộ phận các nhà nghiên cứu AI hàng đầu khác khi không hề có thời gian học tập hay làm việc ở nước ngoài. Ông tốt nghiệp chuyên ngành Trí tuệ nhân tạo thuộc Khoa Kỹ thuật Điện tử của Đại học Chiết Giang.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010222.webp)

Để giải mã bí ẩn này, giới truyền thông phương Tây đã tiến hành dịch lại các bài phỏng vấn cũ của ông sang [tiếng Anh](https://www.chinatalk.media/p/deepseek-ceo-interview-with-chinas).

Bản thân tôi nhận thấy nội dung bài phỏng vấn tiếng Trung gốc ([Phần 1](https://mp.weixin.qq.com/s/Cajwfve7f-z2Blk9lnD0hA), [Phần 2](https://mp.weixin.qq.com/s/r9zZaEgqAa_lml_fOEZmjg)) thực sự vô cùng đáng đọc. Dưới đây tôi xin trích dẫn lại một số phát biểu nổi bật của ông, phản ánh tầm nhìn chiến lược và khát vọng to lớn của thế hệ nhà nghiên cứu công nghệ hàng đầu Trung Quốc:

(1) Mục tiêu cuối cùng của chúng tôi không chỉ dừng lại ở việc tạo ra các sản phẩm AI tạo sinh (Generative AI) thông thường, mà là hướng tới chinh phục Trí tuệ nhân tạo tổng quát (AGI). AI tạo sinh hiện tại chỉ là một chặng đường bắt buộc phải vượt qua, và tôi tin tưởng AGI chắc chắn sẽ được hiện thực hóa ngay trong thế hệ của chúng ta.

(2) Trong ngắn hạn, không có bất kỳ doanh nghiệp AI nào có thể sở hữu ưu thế công nghệ độc quyền tuyệt đối để đè bẹp các đối thủ khác. Bởi lẽ OpenAI đã vạch ra con đường đi rõ ràng, các nghiên cứu đều dựa trên các công bố khoa học và mã nguồn công khai, nên cả các tập đoàn lớn lẫn các công ty khởi nghiệp đều sẽ sớm tự xây dựng được các mô hình ngôn ngữ lớn cho riêng mình.

(3) Trước làn sóng thay đổi mang tính cách mạng của công nghệ, các rào cản độc quyền xây dựng bằng giải pháp đóng mã nguồn (closed-source) sẽ chỉ mang tính tạm thời. Ngay cả OpenAI dù có đóng mã nguồn cũng không thể ngăn cản việc bị các đối thủ khác đuổi kịp và vượt qua. Chúng tôi lựa chọn đầu tư tích lũy giá trị trực tiếp vào con người. Quy trình nghiên cứu giúp đội ngũ kỹ sư của chúng tôi trưởng thành, tích lũy được nhiều bí quyết công nghệ (know-how), từ đó định hình nên một tổ chức có năng lực đổi mới sáng tạo không ngừng — đó mới chính là rào cản độc quyền vững chắc nhất của chúng tôi.

(4) Chúng tôi kiên quyết không đóng mã nguồn. DeepSeek tin tưởng rằng việc chung tay xây dựng một hệ sinh thái công nghệ mở và mạnh mẽ là ưu tiên quan trọng hơn cả.

(5) Giai đoạn hiện tại là thời kỳ bùng nổ của các phát kiến đổi mới công nghệ cốt lõi, chứ chưa phải là thời kỳ bùng nổ của các ứng dụng thương mại. Rào cản kỹ thuật để phát triển ứng dụng trên các mô hình lớn sẽ ngày càng giảm thấp, các công ty khởi nghiệp quyết định gia nhập thị trường ở bất kỳ thời điểm nào trong vòng 20 năm tới đều có cơ hội thành công ngang nhau.

(6) Trong nhiều năm qua, rất nhiều doanh nghiệp Trung Quốc đã hình thành thói quen chờ đợi người khác thực hiện các phát kiến công nghệ cốt lõi, sau đó mang về đóng gói thành ứng dụng để kiếm tiền nhanh. Họ thụ động chờ đợi định luật Moore tự động mang lại các thế hệ phần cứng và phần mềm tối ưu hơn sau mỗi 18 tháng. Tuy nhiên, xuất phát điểm của DeepSeek hoàn toàn khác biệt: Chúng tôi không hướng tới việc tranh thủ kiếm một khoản tiền nhanh, mà muốn trực tiếp đứng ở tuyến đầu công nghệ để cùng thúc đẩy sự phát triển của toàn bộ hệ sinh thái thế giới. Trung Quốc cần phải chủ động đóng góp giá trị cho nhân loại chứ không thể mãi đi nhờ xe của người khác.

(7) Đại bộ phận các doanh nghiệp Trung Quốc có thói quen đi theo (follow) hơn là tự tìm tòi đổi mới. Sự thiếu hụt của công nghệ Trung Quốc hoàn toàn không nằm ở nguồn vốn đầu tư, mà là ở niềm tin chiến lược và phương pháp tổ chức thu hút các tài năng công nghệ chất lượng cao. Đội ngũ của chúng tôi hoàn toàn là nhân sự trong nước chứ không có nhân sự từ nước ngoài trở về. Mặc dù top 50 tài năng xuất sắc nhất thế giới hiện tại có thể không ở Trung Quốc, nhưng chúng tôi tin tưởng mình hoàn toàn có thể tự đào tạo và xây dựng nên những nhân tài như thế.

(8) Chúng tôi trao quyền tự quyết tối đa cho các kỹ sư trong việc điều phối nhân lực và tài nguyên phần cứng máy chủ. Chỉ cần có ý tưởng sáng tạo khả thi, bất kỳ kỹ sư nào cũng có quyền tự gọi lệnh sử dụng hạ tầng siêu máy tính để huấn luyện mô hình mà không cần trải qua các quy trình phê duyệt rườm rà. Đồng thời, do mô hình quản lý không phân cấp bậc hành chính, các nhân sự có thể chủ động liên hệ hợp tác chéo cùng nhau nếu có chung mối quan tâm.

(9) Tiêu chuẩn tuyển dụng cốt lõi của chúng tôi luôn đặt niềm đam mê và sự tò mò lên hàng đầu. Do đó, nhiều thành viên trong đội ngũ sở hữu những lý lịch trải nghiệm vô cùng độc đáo và thú vị. Khát vọng được trực tiếp tham gia nghiên cứu khoa học của họ lớn hơn rất nhiều so với sự quan tâm về thu nhập tài chính.

(10) Chúng tôi đang dấn thân vào những bài toán khó khăn nhất. Cách thức hữu hiệu nhất để thu hút các tài năng hàng đầu là trao cho họ cơ hội được trực tiếp tham gia giải quyết những thách thức lớn nhất của nhân loại. Thực tế, các nhân tài công nghệ đỉnh cao tại Trung Quốc hiện đang bị đánh giá thấp hơn giá trị thực tế do thị trường thiếu vắng các dự án đổi mới công nghệ cốt lõi (hardcore innovation) để họ thể hiện năng lực. Việc chúng tôi lựa chọn đi con đường khó khăn nhất chính là thỏi nam châm mạnh mẽ nhất thu hút họ.

(11) Tiến trình tái cơ cấu nền công nghiệp Trung Quốc sẽ ngày càng phụ thuộc sâu sắc vào năng lực đổi mới công nghệ cốt lõi. Nhiều người sẽ nhận ra rằng nguồn thu nhập nhanh trước đây chủ yếu đến từ yếu tố may mắn của thời đại, và khi cơ hội đó qua đi, họ sẽ có xu hướng tập trung làm các nghiên cứu thực chất hơn.

(12) Tôi lớn lên vào những năm 1980 tại một đô thị nhỏ cấp 5 thuộc tỉnh Quảng Đông. Cha tôi là một giáo viên tiểu học. Vào những năm 1990, Quảng Đông tràn ngập các cơ hội kinh doanh kiếm tiền nhanh khiến nhiều phụ huynh thời đó có quan điểm lệch lạc rằng việc học hành là không cần thiết. Tuy nhiên đến nay khi quay lại nhìn, tư duy của mọi người đều đã thay đổi hoàn toàn do cơ hội kiếm tiền dễ dàng không còn nữa, thậm chí cơ hội chạy taxi cũng đối mặt nguy cơ bị thay thế. Tư duy của cả một thế hệ đã thay đổi hoàn toàn chỉ trong một vòng đời. Trong tương lai, các phát kiến đổi mới công nghệ cốt lõi chắc chắn sẽ ngày một nhiều hơn do xã hội đã được giáo dục bởi thực tế. Khi xã hội tôn vinh và mang lại thành công xứng đáng cho những con người làm công nghệ thực chất, tư duy của số đông sẽ tự động thay đổi. Chúng tôi tin rằng đây là một tiến trình tất yếu của lịch sử.

## 科技动态

1、[Hộp sạc pin dài hạn chuyên dụng cho AirTag](https://www.elevationlab.com/blogs/news/introducing-timecapsule)

Thiết bị định vị AirTag của Apple là giải pháp hữu hiệu giúp theo dõi và tìm kiếm đồ đạc cá nhân. Tuy nhiên nếu thiết bị bị hết pin, tính năng định vị này sẽ hoàn toàn vô dụng.

Một lập trình viên nước ngoài đã trực tiếp trải nghiệm sự cố này khi chiếc túi máy ảnh chứa các thiết bị trị giá 10.000 USD đặt ở ghế sau xe hơi bị kẻ gian lấy trộm. Khi mở ứng dụng định vị để tìm kiếm, anh mới phát hiện chiếc AirTag để bên trong đã bị hết pin từ lâu do quên thay pin định kỳ.

Rút kinh nghiệm sâu sắc từ sự cố, anh đã tự thiết kế và chế tạo một chiếc hộp sạc chuyên dụng cho AirTag bằng cách thiết kế mạch kết nối AirTag trực tiếp với hai viên pin tiểu AA.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122623.webp)

Giải pháp này giúp thiết bị AirTag có khả năng hoạt động liên tục trong suốt 10 năm mà không cần lo lắng về vấn đề hết pin giữa chừng.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122624.webp)

Bạn chỉ cần đặt chiếc hộp sạc AirTag nhỏ gọn này vào cùng hành lý hoặc thiết bị cần theo dõi là có thể hoàn toàn yên tâm về khả năng định vị dài hạn.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122625.webp)

2、[Công nghệ thông quan không cần hộ chiếu giấy](https://www.ica.gov.sg/news-and-publications/newsroom/media-release/passport-less-clearance-fully-rolled-out-at-changi-airport)

Kể từ ngày 30 tháng 9 năm 2024, công dân Singapore khi thực hiện thủ tục xuất nhập cảnh tại sân bay quốc tế Changi sẽ không cần phải xuất trình hộ chiếu giấy truyền thống nữa.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122904.webp)

Hệ thống kiểm soát tại sân bay sẽ ứng dụng công nghệ nhận diện khuôn mặt kết hợp quét võng mạc để xác thực danh tính hành khách tự động, giúp rút ngắn tối đa thời gian chờ đợi và giảm thiểu chi phí vận hành.

Hộ chiếu giấy truyền thống đang dần trở nên lỗi thời và rất có thể sẽ hoàn toàn biến mất trong tương lai không xa.

3、[Tổ hợp khu dân cư in 3D quy mô lớn nhất thế giới](https://www.yahoo.com/news/worlds-largest-3d-printed-neighborhood-060654029.html)

Dự án xây dựng tổ hợp khu dân cư ứng dụng công nghệ in 3D lớn nhất thế giới gồm 100 căn hộ tại bang Texas, Mỹ đang đi vào những công đoạn hoàn thiện cuối cùng.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010208.webp)

Toàn bộ các mảng tường chịu lực của các ngôi nhà đều được tạo hình trực tiếp bằng hệ thống máy in 3D khổng lồ di động tại công trường.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010209.webp)

Vật liệu in sử dụng hỗn hợp đặc chủng gồm bột bê tông, nước, cát và các chất phụ gia liên kết. Hệ thống vòi phun sẽ phun hỗn hợp vật liệu dọc theo các đường chạy được lập trình sẵn trên máy tính, xếp chồng từng lớp một để tạo nên những bức tường kiên cố.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010210.webp)

Đơn vị thi công cho biết giải pháp xây dựng bằng công nghệ in 3D giúp đẩy nhanh tiến độ thi công đáng kể, tối ưu hóa chi phí đầu tư, giảm thiểu tối đa lượng rác thải vật liệu xây dựng và chỉ yêu cầu duy nhất một nhân sự vận hành máy tính điều khiển tại hiện trường.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010211.webp)

Để hoàn thiện toàn bộ phần tường cho một căn hộ một tầng gồm 3 đến 4 phòng ngủ, máy in chỉ mất khoảng thời gian vỏn vẹn 3 tuần. Sau đó, phần mái nhà và gia cố móng sẽ được hoàn thiện nốt bằng các phương pháp xây dựng truyền thống.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010212.webp)

4、**Các tin tức khác**

(1) Cộng đồng mạng phát hiện trên các danh sách phát nhạc (playlists) của dịch vụ **Spotify** xuất hiện nhiều nghệ sĩ ảo hoàn toàn không tồn tại ngoài đời thực. Các sản phẩm âm nhạc của họ khả năng cao là các tác phẩm do AI tự động tạo ra, được Spotify chèn vào nhằm mục đích giảm thiểu chi phí chi trả bản quyền âm nhạc thực tế cho các nghệ sĩ.

(2) Tập đoàn Baidu ra mắt dịch vụ công cụ tìm kiếm thông minh mang tên [Ai 搜](https://chat.baidu.com/search), tích hợp đa dạng các tính năng tương tác hỗ trợ bởi trí tuệ nhân tạo.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010203.webp)

## 文章

1、[Đánh giá và khuyến nghị các bản phân phối Linux nổi bật năm 2024](https://linuxiac.com/best-linux-distro-of-2024-there-is-no-such-thing/) (tiếng Anh)

Tác giả chia sẻ quan điểm cá nhân và giới thiệu chi tiết về các bản phân phối Linux tối ưu nhất cho từng mục đích sử dụng cụ thể của người dùng trong năm qua.

2、[Chiêm nghiệm sau một thời gian làm việc tại cả thị trường Trung Quốc và Mỹ](https://wukan.me/?p=2649) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122801.webp)

"Trong suốt hơn 4 năm qua, do yêu cầu công việc, tôi đã luân chuyển từ San Francisco về Bắc Kinh, sau đó đến Thượng Hải và cuối cùng quay trở lại sinh sống tại Los Angeles trong hơn một năm rưỡi." Bài viết chia sẻ những so sánh thực tế về môi trường làm việc của một kỹ sư phần mềm tại hai quốc gia. (Đóng góp từ [@wukan](https://github.com/ruanyf/weekly/issues/5805))

3][10 lệnh terminal cốt lõi mọi lập trình viên cần làm chủ](https://www.trevorlasn.com/blog/10-essential-terminal-commands-every-developer-should-know/) (tiếng Anh)

Bài viết hướng dẫn cơ bản cách thức sử dụng 10 câu lệnh terminal quen thuộc (như `grep`, `awk`, `sed`, `find`...) phục vụ công việc lập trình hằng ngày.

4、[Chia sẻ kinh nghiệm sau 4 lần tham gia phỏng vấn tại Meta/Facebook](https://justyy.com/archives/67279) (tiếng Trung)

Tác giả chia sẻ chi tiết về quy trình tuyển dụng và những bài học kinh nghiệm quý báu tích lũy được sau 4 lần thử sức phỏng vấn tại tập đoàn công nghệ Meta. (Đóng góp từ [@DoctorLai](https://github.com/ruanyf/weekly/issues/5816))

5、[Cẩm nang ôn luyện kỹ năng phỏng vấn thuật toán](https://javayhu.com/2016-nian-mian-shi-zhi-nan-zhi-suan-fa-mian-shi-xin-de/) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010201.webp)

Bài viết tổng hợp các phương pháp học tập và chia sẻ những kinh nghiệm thực tế giúp lập trình viên vượt qua các bài thi kiểm tra thuật toán trong quy trình tuyển dụng. (Đóng góp từ [@javayhu](https://github.com/ruanyf/weekly/issues/5836))

6、[Tại sao chúng tôi quyết định chuyển hướng từ Next.js về React thuần?](https://www.comfydeploy.com/blog/you-dont-need-nextjs) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010206.webp)

Tác giả chia sẻ những bất cập về hiệu năng và độ phức tạp của Next.js trong quá trình vận hành dự án thực tế, dẫn đến quyết định loại bỏ framework này để quay về sử dụng React thuần.

7、[Hướng dẫn khai thác tính năng quản lý clipboard nâng cao trên Windows 11](https://www.xda-developers.com/permanently-save-items-clipboard-windows-11/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122906.webp)

Bài hướng dẫn chi tiết cách cấu hình tính năng đồng bộ hóa dữ liệu và lưu trữ vĩnh viễn các nội dung sao chép trong bộ nhớ tạm (clipboard) trên hệ điều hành Windows 11.

## 工具

1、[Ghostty](https://ghostty.org/docs)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122804.webp)

Trình giả lập terminal thế hệ mới hiệu năng cao hỗ trợ macOS và Linux, ứng dụng chip đồ họa (GPU) để tối ưu hóa tốc độ kết xuất giao diện. Dự án do chính nhà sáng lập công nghệ HashiCorp phát triển. Xem thêm bài viết [giới thiệu chi tiết](https://linuxiac.com/ghostty-1-0-gpu-accelerated-terminal-emulator-released/).

2、[Black Candy](https://github.com/blackcandy-org/blackcandy)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122905.webp)

Hệ thống máy chủ dịch vụ truyền tải âm nhạc cá nhân mã nguồn mở cho phép tự triển khai (self-host), đi kèm ứng dụng di động và giao diện web tiện lợi giúp bạn tự xây dựng kho nhạc đám mây của riêng mình.

3、[curl-impersonate](https://github.com/lexiforest/curl-impersonate)

Một phiên bản tùy biến của công cụ dòng lệnh quen thuộc curl, được thiết kế để tự động giả lập các thông số HTTP requests giống hệt như các yêu cầu gửi đi từ các trình duyệt phổ biến như Chrome hay Firefox nhằm vượt qua các bộ lọc robot.

4、[RSS.Beauty](https://rss.beauty/)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010202.webp)

Dịch vụ web hỗ trợ chuyển đổi các nguồn tin RSS/Atom thô thành giao diện đọc tin tức trực quan và đẹp mắt, dự án được [chia sẻ mã nguồn mở](https://github.com/ccbikai/RSS.Beauty). (Đóng góp từ [@ccbikai](https://github.com/ruanyf/weekly/issues/5838))

5、[iPalettes (Bộ công cụ tạo chủ đề giao diện Shadcn bằng AI)](https://ipalettes.com/theme/shadcn)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024123004.webp)

Công cụ trực tuyến miễn phí hỗ trợ nhà phát triển nhanh chóng thiết kế và tạo các bộ màu sắc chủ đề cho thư viện UI component Shadcn thông qua các từ khóa mô tả ý tưởng đầu vào. (Đóng góp từ [@meetqy](https://github.com/ruanyf/weekly/issues/5817))

6、[LazyCat Bookmark Cleaner (Lười miêu thư签)](https://github.com/Alanrk/LazyCat-Bookmark-Cleaner)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024123102.webp)

Tiện ích mở rộng Chrome mã nguồn mở hỗ trợ người dùng nhanh chóng quét dọn và loại bỏ các liên kết dấu trang (bookmarks) bị lỗi hoặc các thư mục lưu trữ trống rỗng. (Đóng góp từ [@Alanrk](https://github.com/ruanyf/weekly/issues/5832))

Một tiện ích quản lý dấu trang tương tự khác là **Bookmark Pro**. (Đóng góp từ [@wincatcher](https://github.com/ruanyf/weekly/issues/5833))

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024123103.webp)

7、[Nping](https://github.com/hanshuaikang/Nping)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024123006.webp)

Công cụ kiểm tra kết nối mạng (Ping) hiệu năng cao được phát triển bằng ngôn ngữ Rust, hỗ trợ thực hiện gửi lệnh Ping đồng thời tới nhiều địa chỉ đích khác nhau và trực quan hóa kết quả bằng biểu đồ đường thời gian thực. (Đóng góp từ [@hanshuaikang](https://github.com/ruanyf/weekly/issues/5821))

8、[peepDB](https://github.com/PeepDB-dev/peepdb)

Công cụ dòng lệnh tối giản cho phép lập trình viên nhanh chóng kết nối và truy vấn nhanh dữ liệu bảng từ nhiều hệ quản trị cơ sở dữ liệu quan hệ phổ biến hiện nay.

9、[File Pilot](https://filepilot.tech)

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010204.webp)

Ứng dụng quản trị tệp tin thế hệ mới dành cho hệ điều hành Windows, được thiết kế hướng tới mục tiêu thay thế hoàn toàn cho công cụ Windows File Explorer mặc định.

10、[Doggo](https://doggo.mrkaran.dev/docs/)

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024070204.webp)

Công cụ dòng lệnh hỗ trợ truy vấn thông tin bản ghi DNS nhanh chóng và dễ sử dụng.

Trang chủ của dự án tại địa chỉ [doggo.mrkaran.dev](https://doggo.mrkaran.dev/) cũng cung cấp sẵn công cụ truy vấn DNS trực tuyến miễn phí.

![](https://cdn.beekka.com/blogimg/asset/202407/bg2024070205.webp)

## AI 相关

1、[DeepSeek Coder App Generator](https://github.com/sing1ee/deepseekCoder)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122803.webp)

Ứng dụng hỗ trợ tự động thiết kế và tạo ứng dụng dựa trên mô hình ngôn ngữ lớn DeepSeek V3 thông qua mô tả ý tưởng đầu vào của người dùng. (Đóng góp từ [@sing1ee](https://github.com/ruanyf/weekly/issues/5808))

2、[GodView](https://godview.ai)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122902.webp)

Dịch vụ bản đồ thông minh cho phép người dùng thực hiện truy vấn các địa điểm trên bản đồ bằng ngôn ngữ tự nhiên (ví dụ: "Hãy hiển thị danh sách 10 thư viện lớn nhất tại Thượng Hải").

3、[TalkTo.CEO](https://talkto.ceo)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024123005.webp)

Dịch vụ web ứng dụng AI cho phép người dùng trải nghiệm hội thoại trực tuyến giả lập với các nhà quản trị nổi tiếng như Elon Musk, Trương Nhất Minh hay Nhậm Chính Phi. (Đóng góp từ [@5A59](https://github.com/ruanyf/weekly/issues/5819))

4、[Ithy](https://ithy.com)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024123104.webp)

Trang web tổng hợp kết quả sinh của nhiều mô hình AI khác nhau. Chỉ cần nhập một câu lệnh duy nhất, hệ thống sẽ hiển thị đồng thời kết quả trả về của các mô hình Llama 3.1, o1-mini, Claude 3.5 Sonnet, Grok 2 và Gemini 1.5 Pro để người dùng dễ dàng so sánh.

5、[AutoMouser](https://github.com/guoriyue/AutoMouser)

Tiện ích mở rộng Chrome mã nguồn mở hỗ trợ tự động ghi nhận các thao tác chuột của người dùng và ứng dụng AI để chuyển đổi chúng thành các đoạn kịch bản kiểm thử Selenium viết bằng Python (yêu cầu cấu hình OpenAI API Key). (Đóng góp từ [@guoriyue](https://github.com/ruanyf/weekly/issues/5809))

## 资源

1、[Search the arXiv](https://searchthearxiv.com)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122903.webp)

Công cụ tìm kiếm chuyên dụng cho kho lưu trữ các bài báo nghiên cứu khoa học arXiv, hỗ trợ tìm kiếm bằng ngôn ngữ tự nhiên thông minh.

2、[Dự án chuyển ngữ mã nguồn C++ cho sách giáo khoa Algorithms (Phiên bản 4)](https://github.com/landerrosette/algs4)

Kho chứa mã nguồn cung cấp các giải pháp lập trình bằng ngôn ngữ C++ mô phỏng lại toàn bộ các thuật toán được giới thiệu trong cuốn sách giáo khoa kinh điển *Algorithms (Version 4)* vốn sử dụng mã nguồn Java. (Đóng góp từ [@landerrosette](https://github.com/ruanyf/weekly/issues/5814))

3、[EmojiClick](https://emojis.click/zh)

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122802.webp)

Trang web hỗ trợ người dùng tìm kiếm nhanh các biểu tượng cảm xúc (Emoji) tương ứng thông qua mô tả bằng ngôn ngữ tự nhiên. (Đóng góp từ [@yijianbo](https://github.com/ruanyf/weekly/issues/5806))

4][Awesome Independent Tools (Bộ công cụ dành cho nhà phát triển độc lập)](https://github.com/yaolifeng0629/Awesome-independent-tools)

Kho lưu trữ tổng hợp các giải pháp công nghệ và công cụ hữu ích hỗ trợ đắc lực cho các nhà phát triển độc lập khi triển khai các dự án hướng tới thị trường nước ngoài. (Đóng góp từ [@yaolifeng0629](https://github.com/ruanyf/weekly/issues/5837))

## 图片

1、[Mẫu tờ tiền giấy đẹp nhất thế giới](https://www.theibns.org/joomla/index.php)

Hiệp hội Tiền giấy Quốc tế (IBNS) đã công bố kết quả bình chọn danh hiệu "Tờ tiền giấy đẹp nhất thế giới năm 2023". Tác phẩm chiến thắng thuộc về tờ tiền mệnh giá 2 Đô la do Ngân hàng Trung ương Đông Caribbe phát hành.

Thiết kế của tờ tiền giấy này sở hữu màu sắc phối vô cùng rực rỡ và bắt mắt. Mặt trước in hình ảnh huyền thoại môn bóng chày địa phương kết hợp cùng biểu tượng ngân hàng và hình ảnh sinh vật biển.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122805.webp)

Mặt sau trang trí hình ảnh rạn san hô, cá biển, rùa biển và bản đồ xanh của hòn đảo xinh đẹp.

![](https://cdn.beekka.com/blogimg/asset/202412/bg2024122806.webp)

2、[Những cây thông Giáng sinh mang đặc trưng của từng ngành nghề](https://www.instagram.com/p/DED6ejQyX31/)

Nhân dịp lễ Giáng sinh vừa qua, truyền thông Mỹ đã đăng tải những hình ảnh vô cùng thú vị về các mẫu cây thông Noel độc đáo do các cửa hàng tự sáng tạo từ chính các vật dụng quen thuộc của ngành mình.

Mẫu cây thông Noel làm từ vỏ hộp bánh pizza của một cửa hàng đồ ăn nhanh.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010223.webp)

Cây thông làm từ các tấm kính màu của một cửa hàng thiết kế trang trí nội thất.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010224.webp)

Mẫu cây thông ngộ nghĩnh ghép từ các khối nón cảnh báo giao thông của một đơn vị thi công cầu đường.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010226.webp)

Cây thông xếp từ những cuốn sách của một cửa hàng sách cũ.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010227.webp)

Thiết kế cây thông làm từ các linh kiện phần cứng máy tính tại một cửa hàng sửa chữa đồ điện tử.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010230.webp)

Cây thông Noel xếp từ những quả chuối tại quầy hoa quả của một siêu thị.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010229.webp)

## 文摘

1、[Tại sao dòng sông Amazon hùng vĩ lại không có một cây cầu nào bắc qua?](https://www.cntraveler.com/story/why-the-amazon-river-cant-be-crossed-by-bridge)

Sông Amazon tại Nam Mỹ là dòng sông có chiều dài lớn thứ hai trên thế giới, chỉ xếp sau sông Nile tại châu Phi.

![](https://cdn.beekka.com/blogimg/asset/202501/bg2025010231.webp)

Tuy nhiên, điều kỳ lạ là trong suốt toàn bộ chiều dài của mình, sông Amazon không hề sở hữu bất kỳ một cây cầu nào bắc qua. Đây là dòng sông lớn duy nhất trên thế giới hoàn toàn thiếu vắng các công trình cầu đường kết nối hai bờ. Nguyên nhân là do đâu?

Trước hết là do yếu tố thời tiết khắc nghiệt. Vào mùa mưa hằng năm, mực nước sông Amazon dâng cao gây ngập lụt diện rộng, chiều rộng lòng sông có thể nhanh chóng mở rộng từ mức 5km vào mùa khô lên tới 50km (hình dưới). Việc thiết kế và thi công một cây cầu chịu đựng được sự biến động lòng sông lớn như vậy là cực kỳ khó khăn về mặt kỹ thuật.

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092901.webp)

Thứ hai là do mật độ dân cư dọc hai bên bờ sông vô cùng thưa thớt, chủ yếu là các vùng rừng rậm nhiệt đới hoang vu. Đô thị lớn nhất dọc bờ sông cũng chỉ có quy mô dân số khoảng 500.000 người, dẫn đến nhu cầu di chuyển giao thương đường bộ kết nối hai bờ sông thực tế là không cao.

Cuối cùng là vấn đề bảo vệ môi trường. Rừng Amazon hai bên bờ sông là khu rừng rậm nguyên sinh quan trọng nhất của Trái Đất và hầu như chưa có hệ thống đường giao thông kết nối sẵn. Việc quyết định xây cầu đồng nghĩa với việc sẽ phải chặt phá một diện tích rừng nguyên sinh rất lớn để mở đường dẫn cầu và xây dựng hệ thống đường lộ kết nối, gây ra những tác động tiêu cực nghiêm trọng đến hệ sinh thái. Trong những năm gần đây, khi ý thức bảo vệ môi trường của cộng đồng ngày một nâng cao, làn sóng phản đối việc xây dựng cầu đường xuyên rừng Amazon ngày một mạnh mẽ.

## 言论

1、

Dưới sự bùng nổ mạnh mẽ của công nghệ AI hiện nay, tiếng Anh đang dần trở thành ngôn ngữ lập trình mới phổ biến nhất trên thế giới.

-- [Andrej Karpathy](https://addyo.substack.com/p/the-70-problem-hard-truths-about), *Nhà khoa học AI lừng danh thế giới*

2、

Trừ khi các dòng điện thoại thông minh tương lai được thiết kế tối ưu để có khả năng thay thế hoàn toàn cho máy tính cá nhân, nếu không tôi sẽ không bao giờ đầu tư nâng cấp điện thoại mới chỉ vì các thông số hiệu năng chip xử lý (CPU) nhanh hơn nữa.

-- *Ý kiến của cây viết chuyên mục trang tin Android Authority*

3、

Việc bảo vệ an toàn tuyệt đối cho hệ thống cáp quang dưới đáy đại dương khỏi mọi sự cố phá hoại thực tế là điều bất khả thi. Giải pháp kỹ thuật khả thi duy nhất mà các nhà mạng có thể làm là đầu tư xây dựng hệ thống dự phòng quy mô lớn. Việc đặt nhiều đường cáp quang song song ở các tọa độ khác nhau thực tế lại có chi phí rẻ hơn nhiều so với việc cố gắng bảo vệ một đường cáp duy nhất.

-- *Ý kiến độc giả trên diễn đàn Hacker News*

4、

Giá trị cốt lõi của một kỹ sư phần mềm xuất sắc không nằm ở tốc độ viết mã nguồn nhanh hay số lượng sản phẩm đầu ra nhiều, mà chính là năng lực giải quyết thành công những tác vụ phức tạp mà các kỹ sư thông thường khác hoàn toàn bó tay. Ngược lại, một lập trình viên yếu kém hầu như không thể tự mình hoàn thành tốt bất kỳ tác vụ nào.

Nếu bạn phải làm việc chung với một kỹ sư yếu kém, bạn có thể hỗ trợ họ, nhưng hãy luôn có ý thức bảo vệ quỹ thời gian của mình để tránh bị họ tiêu tốn hết thời gian làm việc cá nhân của bạn.

-- [《Phân tích về ranh giới giữa kỹ sư xuất sắc và kỹ sư yếu kém》](https://www.seangoedecke.com/weak-engineers/)

5、

Trí tuệ nhân tạo thực chất hoàn toàn không giúp giải phóng năng lực tưởng tượng phong phú của con người, mà nó đang dần đảm nhận thay thế (outsource) năng lực đó của chúng ta.

-- *Trích nhận định trên tờ báo The Guardian, Vương quốc Anh*

## 往年回顾

[Bản chất vấn đề: Tại sao các bản ghi nhớ (Memos) lại cho hiệu quả quản trị tốt hơn slide trình chiếu PPT](http://www.ruanyifeng.com/blog/2024/01/weekly-issue-285.html) (Số #285)

[Thảo luận về tỷ lệ thất nghiệp của lao động trẻ và các quyết định khởi động dự án khởi nghiệp](http://www.ruanyifeng.com/blog/2022/12/weekly-issue-235.html) (Số #235)

[Phân tích vụ đấu giá bản hiến pháp Hoa Kỳ — Một trường hợp điển hình ứng dụng công nghệ Blockchain](http://www.ruanyifeng.com/blog/2021/11/weekly-issue-185.html) (Số #185)

[Đánh giá những ngành nghề kinh doanh tối ưu nhất dành cho các nhà khởi nghiệp](http://www.ruanyifeng.com/blog/2020/11/weekly-issue-135.html) (Số #135)

(Hết)
