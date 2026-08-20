# Bản tin chia sẻ công nghệ (Số 376): Tranh luận về trung tâm dữ liệu ngoài không gian

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn. Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/8332) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120304.webp)

Cầu cổng ngõ Đại Vận Hà Hàng Châu là một cây cầu đi bộ nằm tại điểm giao nhau giữa Đại Vận Hà và sông Tiền Đường, sắp sửa được khánh thành mở cửa. Thiết kế ba nhịp vòm của cây cầu mô phỏng đường nét thêu nghệ thuật truyền thống Hàng Châu và những con sóng cuộn trào của sông Tiền Đường. ([via](https://www.163.com/dy/article/KDAJVKT50514ETGI.html))

## 太空数据中心的争议

Cùng với sự bùng nổ của AI, các hệ thống trung tâm dữ liệu dưới mặt đất đang rơi vào tình trạng quá tải, kéo theo chi phí xây dựng và vận hành tăng vọt.

Điều này thúc đẩy ngày càng nhiều ý kiến đề xuất đưa các trung tâm dữ liệu lên vận hành ngoài không gian.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025113006.webp)

Đầu tiên là việc [Elon Musk tiết lộ](https://news.cctv.com/2025/11/11/ARTI6f0b2Jz9Q1WnTzbvH00W251111.shtml) tập đoàn SpaceX đang nghiên cứu phương án xây dựng hệ thống trung tâm dữ liệu ngay trên quỹ đạo Trái Đất.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025113007.webp)

Tiếp đó trong tuần này, Ủy ban Khoa học Công nghệ Bắc Kinh phối hợp cùng Ban Quản lý Khu Khoa học Trung Quan Thôn đã chính thức công bố [《Phương án quy hoạch xây dựng trung tâm dữ liệu ngoài không gian》](https://finance.sina.com.cn/tech/roll/2025-11-28/doc-infywkcw9025829.shtml).

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025113008.webp)

Mục tiêu đề ra là "xây dựng hệ thống trung tâm dữ liệu trên quỹ đạo cách mặt đất 700 km, có khả năng chứa các cụm máy tính hiệu năng cao quy mô hàng triệu card đồ họa để cung cấp dịch vụ tính toán và truyền phát trung chuyển dữ liệu dựa trên không gian".

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025113009.webp)

Theo các báo cáo, giới chuyên gia nhận định việc đưa trung tâm dữ liệu lên vũ trụ là xu thế "[势在必行 - bắt buộc phải làm](https://finance.sina.cn/7x24/2025-11-29/detail-infyzkhk9168276.d.html)" (hình trên) nhờ hai ưu thế vượt trội:

> （1）Các trung tâm dữ liệu ở quỹ đạo cao có thể tận dụng ánh sáng mặt trời cường độ cao 24/7 mà không bị ảnh hưởng bởi tầng khí quyển, hiệu suất phát điện đạt tới 95%.
> 
> （2）Nhiệt độ ngoài không gian sâu rơi vào khoảng -270°C, chỉ cần lắp đặt các vật liệu dẫn nhiệt là có thể tản nhiệt tự nhiên mà không cần đến các hệ thống làm mát bằng chất lỏng phức tạp dưới mặt đất, mang lại ưu thế lớn về mặt chi phí.

Cá nhân tôi thấy đây quả thực là hai lợi thế cực kỳ to lớn, và việc nghiên cứu xây dựng các trung tâm dữ liệu ngoài không gian là hướng đi vô cùng hứa hẹn.

Thế nhưng, ngay sau đó tôi lại đọc được [một bài viết phản biện](https://taranis.ie/datacenters-in-space-are-a-terrible-horrible-no-good-idea/) vô cùng sắc bén.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025113010.webp)

Tác giả bài viết là một kỹ sư kỳ cựu của NASA, người từng tham gia thiết kế nhiều dự án vệ tinh nhân tạo.

Dựa trên những kinh nghiệm thực tế từ quá trình vận hành Trạm Vũ trụ Quốc tế (ISS), ông cho rằng những rào cản kỹ thuật ở giai đoạn hiện tại là quá lớn, khiến việc hiện thực hóa các trung tâm dữ liệu ngoài không gian là cực kỳ khó khăn. Nếu cố tình triển khai, chi phí bỏ ra sẽ vô cùng khổng lồ trong khi hiệu quả thu về lại cực kỳ khiêm tốn.

Đây là lần đầu tiên tôi thấy một bài phân tích phản biện nghiêm túc và chi tiết về chủ đề này. Bản thân tôi không có kiến thức chuyên môn sâu trong lĩnh vực này để đánh giá xem các số liệu tính toán của ông có chuẩn xác hay không. Thêm vào đó, ISS cũng đã được khánh thành từ 25 năm trước, công nghệ kỹ thuật ngày nay rõ ràng đã vượt trội hơn thời kỳ đó rất nhiều.

Dù sao, tôi xin chia sẻ lại các luận điểm phản biện chính của ông dưới đây để chúng ta cùng thảo luận xem liệu ý tưởng này có thực sự khả thi:

**（1）Bài toán năng lượng**

Nguồn năng lượng ngoài không gian chủ yếu đến từ các tấm pin mặt trời. Hệ thống pin mặt trời lớn nhất ngoài không gian hiện nay được lắp đặt trên ISS sở hữu công suất đỉnh đạt hơn 200 kW, nhưng diện tích bề mặt của nó lại vô cùng khổng lồ lên tới 2.500 mét vuông (lớn hơn nửa sân bóng bầu dục Mỹ).

Trong khi đó, dòng card đồ họa chuyên dụng NVIDIA H200 có mức tiêu thụ điện khoảng 0,7 kW, và trong điều kiện vận hành thực tế hệ thống máy chủ cần cấp nguồn khoảng 1 kW cho mỗi card. Điều này đồng nghĩa với việc toàn bộ hệ thống pin mặt trời khổng lồ của ISS hiện tại chỉ đủ cung cấp năng lượng hoạt động cho vỏn vẹn 200 chiếc card H200.

Để so sánh, siêu trung tâm dữ liệu do OpenAI dự kiến xây dựng tại Na Uy được thiết kế để vận hành 100.000 GPU chuyên dụng, và mỗi GPU mới chắc chắn sẽ có mức tiêu thụ điện lớn hơn nhiều so với dòng H200.

**（2）Bài toán tản nhiệt**

Môi trường ngoài không gian sâu cực kỳ lạnh lẽo cận kề độ không tuyệt đối (-273°C), thoạt nhìn việc tản nhiệt có vẻ rất dễ dàng. Nhưng thực tế vật lý chỉ ra rằng nhiệt năng chỉ có thể được truyền đi bằng hai con đường: truyền nhiệt qua vật chất trung gian (đối lưu và dẫn nhiệt) hoặc bức xạ nhiệt.

Vũ trụ là môi trường chân không và hoàn toàn không có không khí. Do đó việc tản nhiệt thông qua cơ chế đối lưu không khí thông thường là bất khả thi, khiến các quạt tản nhiệt hay cánh nhôm tản nhiệt trên các dòng GPU trở nên hoàn toàn vô dụng.

Giải pháp duy nhất khả thi là làm mát bằng chất lỏng: dùng dung môi để dẫn nhiệt từ chip ra các tấm tản nhiệt lớn, sau đó bức xạ nhiệt ra ngoài không gian (các tấm bức xạ nhiệt này bắt buộc phải được bố trí ở phía khuất ánh nắng mặt trời).

Hệ thống tản nhiệt trên ISS cũng đang vận hành theo cơ chế bức xạ nhiệt này. Đó là một hệ thống cực kỳ phức tạp nhưng giới hạn công suất tản nhiệt tối đa chỉ đạt 16 kW – tức là chỉ đủ làm mát cho vỏn vẹn 16 card H200 (tương đương khoảng 1/4 công suất tản nhiệt của một tủ rack máy chủ thông thường dưới mặt đất).

Kích thước tấm bức xạ nhiệt của ISS là 13,6m × 3,12m (diện tích khoảng 42,5 mét vuông). Nếu muốn tản nhiệt cho cụm 200 card H200, diện tích tấm tản nhiệt bắt buộc phải mở rộng lên gấp 12,5 lần, đạt khoảng 531 mét vuông. Diện tích này thậm chí còn lớn gấp 2,6 lần so với diện tích của tấm pin mặt trời cung cấp năng lượng cho chính cụm GPU đó.

Như vậy, một trung tâm dữ liệu ngoài không gian thực tế sẽ sở hữu cấu trúc vật lý cực kỳ cồng kềnh, vượt xa quy mô của ISS, trong khi năng lực tính toán thực tế mang lại chỉ tương đương với vỏn vẹn 3 tủ rack máy chủ dưới mặt đất.

**（3）Hiệu ứng bức xạ hạt**

Ngoài không gian tràn ngập các hạt năng lượng cao di chuyển tốc độ cực lớn. Do không có bầu khí quyển và từ trường Trái Đất che chắn, các hạt này sẽ bắn trực tiếp vào bề mặt vi mạch chip gây ra những tổn hại vật lý. Hiện tượng phổ biến nhất là lỗi lật bit do hạt đơn lẻ (Single Event Upset - SEU), khi một hạt va chạm vào bóng bán dẫn làm thay đổi trạng thái nhị phân của dữ liệu.

Bên cạnh đó, do trung tâm dữ liệu phải vận hành liên tục trong thời gian dài, nó còn phải chịu hiệu ứng tổng liều lượng tích lũy (Total Ionizing Dose - TID). Việc liên tục bị các hạt năng lượng bắn phá sẽ khiến tốc độ đóng ngắt của các bóng bán dẫn chậm dần đi cho đến khi chip hoàn toàn ngừng hoạt động.

Để khắc phục, hệ thống cần được trang bị các lớp che chắn bức xạ dày. Tuy nhiên các tia vũ trụ năng lượng cao nhất có khả năng xuyên qua cả những lớp chì siêu dày. Thêm vào đó, năng lực tải trọng của các tên lửa đẩy hiện nay không cho phép vận chuyển các lớp che chắn quá nặng lên quỹ đạo.

Nếu muốn tăng cường khả năng kháng bức xạ của GPU và bộ nhớ, nhà sản xuất bắt buộc phải thiết kế lại kiến trúc chip chuyên dụng tích hợp các cơ chế chịu lỗi phần cứng. Nhưng điều này sẽ khiến hiệu năng tính toán của các chip chuyên dụng này sụt giảm nghiêm trọng so với các dòng GPU thương mại thông thường dưới mặt đất.

**（4）Rào cản băng thông truyền tải**

Hầu hết các vệ tinh hiện nay giao tiếp với mặt đất qua sóng vô tuyến, và việc đạt tốc độ truyền tải vượt mốc 1 Gbps là vô cùng khó khăn. Mặc dù các giải pháp truyền tin bằng tia laser đang được nghiên cứu để nâng cao băng thông nhưng công nghệ này lại đòi hỏi điều kiện thời tiết khí quyển mặt đất cực kỳ lý tưởng mới có thể vận hành ổn định.

Để so sánh, kết nối mạng giữa các trung tâm dữ liệu dưới mặt đất hiện nay tối thiểu cũng dễ dàng đạt băng thông 100 Gbps.

## [本周软件] 七牛云的大模型接入服务

 vài tuần trước, tôi có [giới thiệu](https://www.ruanyifeng.com/blog/2025/10/weekly-issue-370.html) trên bản tin dịch vụ của [Qiniu Cloud (七牛云)](https://s.qiniu.com/JrUbmm) – **một cổng kết nối hợp nhất hỗ trợ gọi hầu hết các mô hình AI lớn trong và ngoài nước**, được ví như phiên bản OpenRouter của Trung Quốc.

Tuy nhiên thời điểm đó tôi chưa giải thích rõ hai điểm quan trọng dưới đây khiến một số bạn đọc gặp khó khăn khi sử dụng, nay tôi xin bổ sung chi tiết:

Vào thứ Hai tuần này, DeepSeek vừa chính thức ra mắt mô hình V3.2 phiên bản Speciale và phiên bản thông thường, ngay tối hôm đó tôi đã thấy Qiniu Cloud cập nhật đưa lên hệ thống (hình dưới). Tốc độ cập nhật cực nhanh của họ khiến tôi muốn chia sẻ rõ hơn để các bạn dễ dàng trải nghiệm.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120202.webp)

**（1）Các mô hình AI nước ngoài**: Qiniu Cloud hỗ trợ kết nối tới hơn 70 dòng mô hình AI khác nhau. Tuy nhiên do một số quy định, danh sách các mô hình AI nước ngoài không hiển thị trực tiếp trên giao diện trang chủ của họ, nhưng thực tế hệ thống vẫn hỗ trợ kết nối bình thường.

Bạn có thể tra cứu danh sách và mã định danh (Model ID) đầy đủ của các mô hình AI tại [trang web này](https://sufy.com/zh-CN/services/ai-inference/models), hầu như mọi mô hình phổ biến hiện nay đều có mặt (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120201.webp)

Sau khi tìm được Model ID tương ứng (ví dụ `claude-4.5-opus`), bạn chỉ cần truyền chuỗi này vào tham số gọi mô hình trong code để Qiniu Cloud thực hiện kết nối.

**（2）Giới hạn tần suất cuộc gọi (Rate Limit)**: Đối với tài khoản nhà phát triển thông thường, giới hạn tần suất được thiết lập ở mức "5 yêu cầu/phút và 60 yêu cầu/giờ" – hoàn toàn đáp ứng tốt nhu cầu lập trình trải nghiệm cá nhân. Nếu gọi vượt quá tần suất này, hệ thống sẽ trả về lỗi nghẽn mạng (Status Code 429).

Mức giới hạn này thực tế không hề quá khắt khe nếu so sánh với gói dịch vụ trả phí Pro chính thức của Claude vốn cũng chỉ giới hạn ở mức 45 yêu cầu mỗi 5 giờ.

Lý do tôi giới thiệu Qiniu Cloud là bởi đây là một doanh nghiệp công nghệ lớn đã niêm yết trên sàn chứng khoán, bảo đảm dịch vụ có độ ổn định và cam kết hỗ trợ tốt. Đồng thời hệ thống của họ tương thích tốt với cấu trúc gọi API của cả OpenAI và Anthropic giúp lập trình viên tích hợp rất nhanh chóng (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120203.webp)

**Tài khoản mới đăng ký sẽ nhận ngay 3 triệu Token miễn phí**. Nếu đăng ký qua liên kết giới thiệu và mời thêm bạn bè sử dụng, bạn sẽ nhận thêm 5 triệu Token và người được mời nhận 10 triệu Token. Điểm cộng lớn là lượng Token tặng kèm này là vô cùng linh hoạt và có thể dùng chung cho mọi dòng mô hình AI mà họ hỗ trợ. Các bạn có thể đăng ký trải nghiệm thông qua [liên kết giới thiệu của tôi](https://s.qiniu.com/JrUbmm).

## 科技动态

1. **Khủng hoảng hải lưu của Iceland**

Chính phủ Iceland vừa tuyên bố sự bất ổn của các dòng hải lưu trên biển Đại Tây Dương là vấn đề an ninh quốc gia cấp bách đe dọa trực tiếp đến sự tồn vong của đất nước.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025113005.webp)

Dữ liệu quan trắc cho thấy do hiện tượng ấm lên toàn cầu, vòng tuần hoàn Đại Tây Dương (hệ thống AMOC) đang có xu hướng yếu đi. Hệ thống hải lưu này đóng vai trò như một băng tải khổng lồ vận chuyển dòng nước ấm từ khu vực xích đạo lên phía bắc, mang lại nền khí hậu ấm áp dễ chịu cho vùng Bắc Đại Tây Dương.

Một khi dòng hải lưu ấm áp này bị đứt gãy, nhiệt độ tại Iceland sẽ giảm sâu nghiêm trọng. Trong kịch bản tồi tệ nhất, đảo quốc này có thể bị bao phủ bởi các lớp băng dày, biến thành một "hòn đảo băng" thực sự và không còn phù hợp cho con người sinh sống.

2. **Âm thanh từ sao Hỏa**

Sao Hỏa sở hữu những âm thanh gì?

Các nhà khoa học cũng rất tò mò về điều đó. Khi robot Perseverance của NASA hạ cánh xuống sao Hỏa vào tháng 2 năm 2021, thiết bị đã được trang bị sẵn một mic thu âm chuyên dụng để lắng nghe âm thanh từ hành tinh đỏ.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120104.webp)

Bức ảnh trên mô tả cụm microphone được bố trí trên đỉnh tháp camera của robot.

Gần đây, một nhóm nghiên cứu đã tiến hành phân tích hơn 28 giờ dữ liệu âm thanh ghi nhận từ microphone này.

Họ đã nghe thấy những tiếng va đập trên bề mặt hành tinh, đồng thời đo lường được các tín hiệu điện trường tương ứng, từ đó đưa ra nhận định đây chính là âm thanh của những tia sét.

Đây là lần đầu tiên nhân loại biết được trên sao Hỏa cũng xuất hiện các hiện tượng sấm sét. Do bầu khí quyển trên sao Hỏa cực kỳ mỏng và không có hơi nước để tạo thành mây nên hiện tượng sét đánh không xuất hiện theo dạng phóng điện giữa các đám mây. Các nhà khoa học phán đoán hiện tượng phóng điện này được tạo ra do sự ma sát tĩnh điện giữa các hạt cát, bụi đất trong những cơn lốc xoáy khổng lồ.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120105.webp)

3. **Lá cây nhân tạo**

Một nhóm nghiên cứu của Mỹ vừa chế tạo thành công các tấm pin năng lượng mặt trời có hình dáng giống như những chiếc lá cây.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025042813.webp)

Phần cuống của những chiếc lá này được kết nối trực tiếp với các chất xúc tác hóa học. Khi hấp thụ ánh sáng mặt trời, hệ thống có khả năng chuyển hóa khí CO2 và nước thành các dạng nhiên liệu hữu ích.

Nếu ghép nhiều chiếc lá này lại với nhau để tạo thành một cây nhân tạo hoàn chỉnh, nó sẽ trở thành một nhà máy sản xuất nhiên liệu mini độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202504/bg2025042814.webp)

Điều này gợi ý cho chúng ta rằng các thiết bị năng lượng mặt trời hoàn toàn có thể được thiết kế dưới nhiều hình dáng sinh động mô phỏng tự nhiên thay vì chỉ là các tấm phẳng truyền thống.

## 文章

1. [Thông cáo chính thức phản hồi về các báo cáo bảo mật ứng dụng tiện ích trình duyệt gần đây](https://mp.weixin.qq.com/s/E8YQLWZFM2J7r5DZNSl47w) (tiếng Trung)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120403.webp)

Một nhóm nghiên cứu bảo mật quốc tế gần đây đã công bố [một báo cáo](https://programnotes.cn/browser-security-ShadyPanda/index.html) chỉ ra một số tiện ích mở rộng trình duyệt phổ biến (như Clean Master, WeTab) có chứa mã độc hại. Bài viết là phản hồi chính thức từ đội ngũ phát triển các tiện ích này tại Trung Quốc.

Họ cho biết dự án Clean Master đã được chuyển nhượng hoàn toàn cho đơn vị khác từ năm ngoái và không còn liên quan đến họ, còn các cảnh báo đối với các tiện ích khác là do hệ thống nhận diện nhầm. Độc giả nên tham khảo cả [báo cáo bảo mật gốc](https://programnotes.cn/browser-security-ShadyPanda/index.html) để có cái nhìn đa chiều. (Đóng góp từ [@yiGmMk](https://github.com/ruanyf/weekly/issues/8349))

2. [So sánh chi tiết giữa hai giải pháp phát triển ứng dụng desktop: Electron và Tauri](https://www.dolthub.com/blog/2025-11-13-electron-vs-tauri/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112801.webp)

Electron và Tauri hiện là hai công nghệ chủ lưu nhất để xây dựng các ứng dụng desktop đa nền tảng. Bài viết tiến hành so sánh chuyên sâu về kiến trúc kỹ thuật cũng như những ưu và nhược điểm cụ thể của từng giải pháp.

3. [Lý do tôi quyết định chuyển toàn bộ mã nguồn dự án khỏi GitHub](https://dillo-browser.org/news/migration-from-github/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120103.webp)

Cảm thấy hệ thống của GitHub đã trở nên quá cồng kềnh và không còn phù hợp với nhu cầu phát triển tinh gọn, tác giả đã tự xây dựng một hệ thống quản lý và lưu trữ mã nguồn nội bộ của riêng mình. Bài viết là tài liệu tham khảo hữu ích cho những ai có ý định tự thiết lập máy chủ Git cá nhân.

4. [Định dạng Protobuf ưu việt hơn JSON trong truyền tải dữ liệu](https://aloisdeniel.com/blog/better-than-json) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120215.webp)

Tác giả bài viết đưa ra lời kêu gọi cộng đồng lập trình nên chuyển đổi sang sử dụng định dạng Protobuf thay thế cho JSON khi truyền tải dữ liệu. Anh lập luận rằng ưu điểm duy nhất của JSON hiện tại chỉ là giúp con người có thể đọc hiểu trực tiếp bằng mắt thường.

5. [Hướng dẫn cách viết một tệp cấu hình CLAUDE.md chất lượng cho dự án](https://www.humanlayer.dev/blog/writing-a-good-claude-md) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120102.webp)

Nhiều công cụ hỗ trợ lập trình bằng AI hiện nay sử dụng một tệp văn bản đặc biệt đặt ở thư mục gốc của dự án làm dữ liệu ngữ cảnh mặc định cho mỗi phiên làm việc. Bài viết lấy tệp `CLAUDE.md` làm ví dụ để hướng dẫn cách tối ưu hóa nội dung tệp này nhằm tăng độ chính xác cho AI.

6. [Hệ thống quản lý tệp tin ZFS ưu việt hơn Btrfs](https://www.xda-developers.com/how-zfs-is-superior-to-btrfs/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202502/bg2025022202.webp)

ZFS và Btrfs là hai hệ thống quản lý tệp tin (File System) hiện đại phổ biến hiện nay. Bài viết phân tích các đặc tính kỹ thuật của hai hệ thống và lập luận giải thích tại sao ZFS lại mang lại độ tin cậy và an toàn dữ liệu cao hơn.

## 工具

1. [Fizzy](https://github.com/basecamp/fizzy)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120401.webp)

Công ty công nghệ nổi tiếng 37Signals vừa chính thức mở nguồn mở ứng dụng quản lý công việc dạng bảng Kanban mà họ sử dụng nội bộ bấy lâu nay.

2. [Fresh](https://github.com/sinelaw/fresh)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120402.webp)

Một trình soạn thảo văn bản gọn nhẹ vận hành hoàn toàn trên giao diện dòng lệnh terminal.

3. [Gitmal](https://github.com/antonmedv/gitmal)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120216.webp)

Công cụ hỗ trợ tự động đóng gói và biến đổi toàn bộ kho lưu trữ Git thành một trang web tĩnh, cho phép duyệt tệp, xem lịch sử commit và hiển thị màu code trực quan trên trình duyệt.

4. [GitHub Card](https://githubcard.com)

Dịch vụ web hỗ trợ tự động tạo ảnh thẻ chia sẻ đẹp mắt cho tài khoản cá nhân hoặc kho lưu trữ dự án trên GitHub. (Đóng góp từ [@Cactusinhand](https://github.com/ruanyf/weekly/issues/8303))

5. [EasyDB](https://github.com/shencangsheng/easydb_app)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112804.webp)

Ứng dụng quản trị cơ sở dữ liệu đa nền tảng chạy trên máy tính, hỗ trợ sử dụng ngôn ngữ SQL để truy vấn trực tiếp trên nhiều định dạng tệp dữ liệu khác nhau như SQLite, CSV, Excel hay JSON. (Đóng góp từ [@shencangsheng](https://github.com/ruanyf/weekly/issues/8313))

6. [Webhooker](https://github.com/TokenRollAI/webhooker)

Hệ thống cổng trung chuyển và chuyển tiếp các tín hiệu Webhook, ví dụ hỗ trợ tự động chuyển tiếp các tin nhắn từ kênh Slack sang ứng dụng Feishu (Lark) hoặc DingTalk. (Đóng góp từ [@Disdjj](https://github.com/ruanyf/weekly/issues/8318))

7. [PySInfo](https://github.com/EasyCam/Pysinfo)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120101.webp)

Đoạn kịch bản Python hỗ trợ hiển thị nhanh toàn bộ thông tin phần cứng và hệ thống máy tính ngay trên dòng lệnh, tương tự công cụ `fastfetch`. (Đóng góp từ [@cycleuser](https://github.com/ruanyf/weekly/issues/8333))

8. [PocketMocker](https://github.com/tianchangNorth/pocket-mocker)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120204.webp)

Thư viện Mock dữ liệu chạy ở frontend, hoạt động bằng cách chặn các yêu cầu `fetch` và `XMLHttpRequest` trực tiếp trên trang web kèm bảng điều khiển trực quan. (Đóng góp từ [@tianchangNorth](https://github.com/ruanyf/weekly/issues/8345))

9. [code996](https://github.com/hellodigua/code996)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120302.webp)

Công cụ dòng lệnh hỗ trợ phân tích thời gian thực hiện các commit trên kho lưu trữ Git để đưa ra thống kê về mức độ cường độ làm việc và tình trạng làm việc ngoài giờ (OT) của dự án. (Đóng góp từ [@hellodigua](https://github.com/ruanyf/weekly/issues/8361))

10. [Markdown2PNG (玉桃文飨轩)](https://github.com/nicejade/markdown2png)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120305.webp)

Ứng dụng web mã nguồn mở hỗ trợ chuyển đổi nhanh các nội dung văn bản định dạng Markdown thành hình ảnh định dạng PNG đẹp mắt. (Đóng góp từ [@nicejade](https://github.com/ruanyf/weekly/issues/8363))

## AI 相关

1. [ClipSketch AI](https://github.com/RanFeng/clipsketch-ai)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120217.webp)

Ứng dụng web mã nguồn mở sử dụng mô hình Gemini để tự động chuyển đổi nội dung các video trên Xiaohongshu hoặc Bilibili thành một chuỗi hình ảnh truyện vẽ tay trực quan. (Đóng góp từ [@RanFeng](https://github.com/ruanyf/weekly/issues/8353))

2. [Banana Prompt Quicker](https://github.com/glidea/banana-prompt-quicker)

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120306.webp)

Plugin trình duyệt mã nguồn mở tổng hợp các từ khóa gợi ý (prompt) phổ biến dành riêng cho mô hình Nano Banana giúp người dùng dễ dàng tái sử dụng nhanh chóng. (Đóng góp từ [@glidea](https://github.com/ruanyf/weekly/issues/8364))

3. [git-rewrite-commits](https://github.com/f/git-rewrite-commits)

Công cụ ứng dụng trí tuệ nhân tạo (AI) hỗ trợ tự động quét và viết lại toàn bộ lịch sử thông điệp commit (commit messages) của Git trở nên rõ ràng, chi tiết và chuẩn hóa hơn.

## 资源

1. **Các bức ảnh báo chí xuất sắc nhất năm 2025**

Tạp chí danh tiếng 《Time》 chính thức công bố danh sách [100 bức ảnh báo chí xuất sắc nhất năm 2025](https://time.com/7336112/top-100-photos-2025/), bên cạnh đó hãng thông tấn [Reuters cũng công bố danh sách ảnh năm tương tự](https://www.reuters.com/investigates/special-report/year-end-2025-photos-best/).

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112901.webp)

2. **Những bài viết được đọc nhiều nhất trên Wikipedia năm 2025**

Quỹ Wikimedia công bố danh sách [20 bài viết tiếng Anh được truy cập nhiều nhất trên Wikipedia năm 2025](https://wikimediafoundation.org/news/2025/12/02/announcing-wikipedias-most-read-articles-of-2025/), phần lớn các chủ đề tập trung vào các sự kiện chính trị lớn, văn hóa đại chúng và những nhân vật nổi tiếng qua đời trong năm.

![](https://cdn.beekka.com/blogimg/asset/202512/bg2025120303.webp)

3. **Trang thông tin về các loài chim ruồi (HummingbirdSpot)**

Dự án website do một cựu nữ giáo viên người Mỹ xây dựng với mục tiêu chụp ảnh toàn bộ các loài chim ruồi trên Trái Đất. Trong tổng số 366 loài chim ruồi được ghi nhận trên thế giới, cô đã tự tay ghi hình được 277 loài.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025112707.webp)

## 图片

1. **Bảo tàng Hoàng tử bé**

Tác phẩm văn học kinh điển 《Hoàng tử bé》 xuất bản lần đầu vào năm 1943 và đã trở thành cuốn sách gối đầu giường của hàng triệu độc giả trên toàn cầu.

Để tôn vinh tác phẩm cùng cuộc đời của nhà văn Antoine de Saint-Exupéry, Thụy Sĩ gần đây đã khánh thành một bảo tàng chuyên biệt dành riêng cho Hoàng tử bé.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025113001.webp)

Bảo tàng là nơi lưu giữ nhiều phiên bản in ấn của cuốn sách qua các thời kỳ và các ngôn ngữ khác nhau cùng nhiều kỷ vật độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025113002.webp)

Cốt truyện của tác phẩm kể về một vị hoàng tử bé sinh sống trên tiểu hành tinh B612 nhỏ bé. Tiểu hành tinh này chỉ vừa đủ chỗ cho hai ngọn núi lửa đang hoạt động, một ngọn núi lửa đã tắt và một bông hoa hồng duy nhất.

Hoàng tử bé đã rời hành tinh B612 để lần lượt ghé thăm 6 tiểu hành tinh lân cận – nơi sinh sống của một vị vua, một kẻ hợm hĩnh, một gã nát rượu, một nhà doanh nghiệp, một người gác đèn trung thành và một nhà địa lý. Cuối cùng, hoàng tử đặt chân tới Trái Đất trước khi quay trở lại hành tinh thân yêu của mình.

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025113003.webp)

![](https://cdn.beekka.com/blogimg/asset/202511/bg2025113004.webp)

## 文摘

1. [Tại sao chất lượng mã nguồn tại các tập đoàn công nghệ lớn lại thường không cao?](https://www.seangoedecke.com/bad-code-at-big-companies/)

Trái ngược với suy nghĩ của phần lớn công chúng, chất lượng code tại các tập đoàn công nghệ lớn (Big Tech) thực tế lại không hề cao.

Điều này nghe có vẻ phi lý, bởi các tập đoàn lớn luôn đưa ra mức đãi ngộ cực kỳ hấp dẫn để chiêu mộ những kỹ sư giỏi nhất thị trường, đi kèm môi trường làm việc lý tưởng, trang thiết bị hiện đại cùng quy trình phát triển chuyên nghiệp.

Thế nhưng thực tế là chất lượng code của họ lại không hề tương xứng với những lợi thế đó.

Nguyên nhân vô cùng đơn giản: phần lớn mã nguồn của các hệ thống được viết bởi những lập trình viên chưa có nhiều kinh nghiệm thực tế trong lĩnh vực cụ thể đó (những người mới trong mảng đó).

Họ không phải là những kỹ sư kém cỏi, mà chỉ đơn thuần là do họ bị luân chuyển và buộc phải đảm nhận những dự án nằm ngoài chuyên môn sâu của mình.

Trong đời thực, kỹ sư tại các tập đoàn lớn hiếm khi gắn bó lâu dài với một dự án cụ thể. Cơ cấu thưởng bằng cổ phiếu của các Big Tech thường được thiết kế theo chu kỳ 4 năm. Sau 4 năm, khi lượng cổ phiếu thưởng ban đầu đã nhận hết, thu nhập của kỹ sư sẽ sụt giảm đáng kể nếu họ không được thăng chức, và đây là thời điểm họ thường lựa chọn ra đi.

Tình trạng luân chuyển nội bộ thậm chí còn khiến mọi việc tệ hơn. Bản thân tôi khi làm việc tại một đội ngũ hoặc phụ trách một kho lưu trữ code, khoảng thời gian dài nhất cũng chỉ dừng lại ở mức 3 năm. Về sau, hầu như năm nào tôi cũng trải qua các đợt tái cấu trúc nhân sự, liên tục chuyển đổi dự án hoặc đội ngũ phát triển.

Tuy nhiên, các kho lưu trữ mã nguồn của các tập đoàn lớn lại có tuổi đời rất dài, nhiều hệ thống đã vận hành ổn định suốt 10 năm hoặc lâu hơn. Rắc rối là trong suốt 10 năm đó, kho lưu trữ code đã đi qua tay vô số chủ sở hữu khác nhau, và phần lớn các thay đổi mã nguồn sau này được thực hiện bởi các kỹ sư mới tiếp nhận dự án chưa đầy 6 tháng.

Bạn sẽ tự hỏi: Vậy những kỹ sư lão luyện (senior/staff engineers) tại các tập đoàn lớn không trực tiếp viết code sao? Những người đã tích lũy chuyên môn sâu suốt nhiều năm và có khả năng review code sắc bén để phát hiện lỗi hiện đang làm gì?

Thứ nhất, các tập đoàn lớn thường không quá chú trọng đến việc duy trì các nhân sự chuyên môn sâu lâu năm cho một dự án cụ thể. Trước sau gì họ cũng sẽ bị luân chuyển sang một bộ phận khác để bắt đầu tiếp cận một hệ thống hoàn toàn mới từ đầu.

Thứ hai, khối lượng công việc của các kỹ sư lão luyện là vô cùng khổng lồ. Là một trong số ít người thực sự thấu hiểu hệ thống, họ luôn bận rộn với hàng tá cuộc họp và công việc chuyên môn riêng, không thể đủ thời gian để trực tiếp review chi tiết từng dòng code thay đổi của cấp dưới.

Tóm lại, thực tế tại các tập đoàn lớn là bạn luôn bị đẩy vào các dự án mới và liên tục phải chạy đua với các deadline sát nút. Lập trình viên phải nỗ lực hết mình trong một môi trường không hề lý tưởng cho việc viết ra những dòng code chất lượng cao.

Trong bối cảnh đó, việc duy trì chất lượng code hoàn hảo là điều bất khả thi. Kịch bản phổ biến nhất là một lập trình viên cấp dưới (junior) tiếp nhận một ticket sửa lỗi bug khó chịu trong một kho lưu trữ code mà anh ta chưa hề quen thuộc. Sau vài ngày mò mẫm, anh ta đưa ra một giải pháp chắp vá tạm thời. Nếu may mắn, một kỹ sư lão luyện sẽ dành ra 30 phút rảnh rỗi để lướt qua, bác bỏ giải pháp đó và đưa ra một hướng xử lý tốt hơn đôi chút để chạy được hệ thống. Lập trình viên junior cố gắng hiện thực hóa giải pháp đó, chạy test cơ bản thấy chạy được liền submit và release, và tất cả mọi người lại lập tức quay sang xử lý các đầu việc ưu tiên cao tiếp theo.

## 言论

1.

Người dân tại các quốc gia châu Á hiện đang trải qua giai đoạn chuyển dịch lớn từ cuộc sống nông nghiệp vất vả sang cuộc sống đô thị công nghiệp tại các nhà máy. Sự chuyển dịch này dường như đang thổi bùng ngọn lửa nhiệt huyết lao động, giúp họ sẵn sàng làm việc cật lực để đổi lấy những giá trị mà người dân châu Âu hiện nay coi là nhỏ nhặt, không đáng kể.

Đó là điều tốt cho họ. Nhưng tại châu Âu, chúng ta đã đi qua giai đoạn chuyển dịch đó từ lâu và dần trở nên lười biếng, thiếu đi động lực phấn đấu. Một xã hội mà mọi nhu cầu thiết yếu hàng ngày đều được sản xuất và cung cấp bởi người khác là một mô hình không thể phát triển bền vững lâu dài.

-- Chia sẻ từ một độc giả người Đức trên diễn đàn Hacker News

2.

Màn hình hiển thị điện tử trên xe ô tô thực tế cực kỳ có hại khi lái xe vào ban đêm, đặc biệt đối với những người lái xe trên 40 tuổi. Ở độ tuổi này, thị lực bắt đầu suy giảm, khả năng điều tiết tiêu cự và thích ứng ánh sáng của mắt chậm đi, ánh sáng từ màn hình điện tử sẽ làm giảm khả năng quan sát bóng tối, khiến họ khó nhìn rõ các chướng ngại vật trên đường phía trước.

-- Độc giả trên diễn đàn Hacker News

3.

Người bình thường không thể đọc hiểu các bài báo cáo nghiên cứu toán học, nhưng có một sự thật trong giới mà người ngoài ít biết: chính các nhà toán học cũng không thể đọc hiểu được rất nhiều bài báo cáo nghiên cứu của các đồng nghiệp khác.

-- Tạp chí khoa học danh tiếng 《Science》

4.

Trong kỷ nguyên của các mô hình AI lớn, chúng ta dường như đang đánh mất đi một thứ vô cùng quý giá: giọng văn độc bản của chính mình.

Mọi bài viết do AI tạo ra đều mang một tông giọng chung chung, đều tăm tắp như thể được viết ra bởi cùng một người phát ngôn quan hệ công chúng vậy.

Nếu bạn phó mặc hoàn toàn việc viết lách cho các mô hình AI, bạn đã tự nguyện từ bỏ giọng nói cá nhân của mình. Giọng văn riêng biệt là tài sản vô giá được nhào nặn từ chính những trải nghiệm sống độc nhất của bạn, và không một mô hình AI nào có thể sao chép hoàn hảo được nó.

-- [《Mô hình AI lớn đang cướp đi giọng nói của chúng ta》](https://tonyalicea.dev/blog/were-losing-our-voice-to-llms/)

## 往年回顾

[Công cụ vẽ sơ đồ D2 chuyên nghiệp](https://www.ruanyifeng.com/blog/2024/12/weekly-issue-329.html) (#329)

[Bi kịch của các cộng đồng trực tuyến](https://www.ruanyifeng.com/blog/2023/11/weekly-issue-279.html) (#279)

[Lời giải cho bài toán sạc pin điện thoại](https://www.ruanyifeng.com/blog/2022/11/weekly-issue-229.html) (#229)

[Phương thức ứng dụng đúng đắn của công nghệ AR](https://www.ruanyifeng.com/blog/2021/10/weekly-issue-179.html) (#179)

(Hết)
