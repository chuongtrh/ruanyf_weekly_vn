# 科技爱好者周刊（第 226 期）：谷歌出了什么问题？

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần。

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn。

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2666) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập。

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022093002.webp)

Hệ thống mái che đỗ xe tích hợp các tấm pin năng lượng mặt trời tại Tấn Trung, tỉnh Sơn Tây. Mô hình bãi đỗ xe này cực kỳ lý tưởng cho các dòng xe điện: xe vừa được che nắng nóng, vừa có thể cắm sạc trực tiếp từ nguồn điện mặt trời trong thời gian đỗ. (Nguồn: [New York Times](https://www.nytimes.com/2022/09/26/business/china-electric-vehicles.html))

## 本周话题：谷歌出了什么问题？

Vào ngày cuối cùng của tháng trước (30 tháng 9), Google đã bất ngờ ra thông báo đóng cửa hoàn toàn nền tảng chơi game đám mây Stadia của mình.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101309.webp)

Quyết định này diễn ra cực kỳ đột ngột. Chỉ mới ngày hôm trước, các nhân viên phụ trách Stadia vẫn còn đăng bài trên mạng xã hội hỏi xin ý kiến phản hồi của game thủ để cải tiến dịch vụ.

[Các báo cáo truyền thông](http://finance.sina.com.cn/tech/csj/2022-10-06/doc-imqmmtha9943707.shtml) đã tiết lộ chi tiết cuộc họp khẩn cấp diễn ra vào buổi sáng hôm đó:

> *"Vào lúc 7 giờ sáng, giám đốc phụ trách dự án Stadia gửi email triệu tập toàn bộ nhân sự tham gia một cuộc họp quan trọng vào lúc 8 giờ 30 phút, yêu cầu mọi người tạm gác các công việc khác để tham dự.*
> 
> *Cuộc họp chỉ diễn ra vỏn vẹn trong 10 phút. Giám đốc thông báo ngắn gọn rằng toàn bộ nền tảng Stadia sẽ dừng hoạt động vào tháng 1 năm sau và tuyên bố giải tán cuộc họp. Ngay sau đó, thông cáo báo chí chính thức được đăng tải trên blog của Google."*

Điều này nghĩa là ngay cả đội ngũ nhân viên phát triển dự án cũng chỉ được biết tin trước công chúng đúng 1 tiếng đồng hồ.

Đây không phải lần đầu tiên Google bất ngờ khai tử một sản phẩm phần mềm của mình, và hành động này thực sự gây tổn thương sâu sắc tới lòng tin của người dùng và đối tác.

Chỉ sau một đêm, các kỹ sư mất việc làm, người chơi đứng trước nguy cơ đống thiết bị phần cứng và phần mềm game đã mua trở thành rác công nghệ. Dù Google cam kết hoàn trả lại tiền mua game, nhưng toàn bộ dữ liệu lưu trữ (save game) và các vật phẩm người chơi nỗ lực cày cuốc chắc chắn sẽ biến mất.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101310.webp)

Khác với các ứng dụng nội bộ trước đây, Stadia là một nền tảng trò chơi kết nối rất nhiều nhà phát triển và studio game độc lập bên ngoài. Việc đóng cửa đột ngột này khiến toàn bộ công sức, tiền bạc và thời gian chuẩn bị porting game của các studio bên thứ ba [đổ sông đổ bể](https://finance.sina.com.cn/tech/internet/2022-09-30/doc-imqqsmrp1052518.shtml). Khả năng Google đền bù cho họ là rất thấp.

Trong phần *Bài đọc thêm* cuối số bản tin tuần này, bạn đọc có thể theo dõi chia sẻ đầy phẫn uất của một studio game nhỏ để hiểu rõ hơn về mức độ ảnh hưởng của sự việc.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101311.webp)

Sau sự cố Stadia, có một điều chắc chắn: **Ngành công nghiệp game sẽ không bao giờ còn đặt niềm tin vào các dự án của Google nữa.** Google đã tự đóng cánh cửa bước vào thị trường game đầy tiềm năng khi sẵn sàng khai tử dịch vụ bất chấp thiệt hại của các nhà phát triển liên kết. Sẽ không còn ai dám mạo hiểm đầu tư tài nguyên để phát triển game cho một nền tảng của Google.

Đây chắc chắn sẽ là một trong những thất bại chiến lược lớn nhất trong lịch sử của Google. Thị trường game là một miếng bánh vô cùng béo bở với tốc độ tăng trưởng phi mã, việc tự rút lui là điều cực kỳ đáng tiếc.

Dù Stadia hoạt động thua lỗ và thiếu hụt các tựa game bom tấn độc quyền để thu hút người dùng mới, **giá trị chiến lược cốt lõi của nó là giúp Google duy trì sự hiện diện tại thị trường game**, làm cầu nối xây dựng mối quan hệ hợp tác lâu dài với các hãng game lớn. Việc đóng cửa Stadia đã cắt đứt hoàn toàn mối liên kết này.

Đáng nói hơn, Google sở hữu rất nhiều nguồn lực công nghệ lớn như: thuật toán AI hàng đầu, nền tảng đám mây Google Cloud, YouTube, Android, Google Play Store... Mảng game đám mây đáng lẽ là cơ hội tuyệt vời để liên kết toàn bộ sức mạnh này lại nhằm tạo ra một sản phẩm mang tính cách mạng cho người dùng.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101312.webp)

Nhiều năm gần đây, năng lực sáng tạo của Google dường như đang gặp vấn đề nghiêm trọng khi số lượng sản phẩm mới mang lại sự đột phá ngày càng thưa thớt.

Thử nhìn lại chặng đường 10 năm qua, hầu như không có một sản phẩm mới nào của Google khiến người dùng thực sự ấn tượng. Hãy thử tìm kiếm trên [trang danh mục sản phẩm](https://about.google/products/#all-products) của Google:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101313.webp)

Tại Google, một sản phẩm chỉ được coi là thành công lớn khi đạt mốc 1 tỷ người dùng thường xuyên. **Hiện tại, Google đang sở hữu 9 sản phẩm đạt mốc [1 tỷ người dùng](https://www.techspot.com/news/81119-photos-becomes-ninth-google-product-pass-one-billion.html)** bao gồm: Google Search, Google Maps, Gmail, Google Chrome, Google Drive, Android, Google Play Store, Google Photos và YouTube.

Điểm chung duy nhất của cả 9 sản phẩm cốt lõi này là: **Tất cả chúng đều được ra mắt trước năm 2012.** Nghĩa là suốt một thập kỷ qua, Google không tạo thêm được bất kỳ một sản phẩm tỷ người dùng mới nào.

Từ vị thế một biểu tượng công nghệ luôn dẫn đầu các xu hướng mới trên Internet, Google của những năm gần đây đang tỏ ra chậm chạp và thiếu đi sự sáng tạo đột phá. Việc khai tử Stadia và tự đánh mất cơ hội ở mảng game một lần nữa đặt ra dấu hỏi lớn về năng lực quản trị chiến lược dài hạn của gã khổng lồ tìm kiếm.

## 科技动态

1、[Tesla công bố loại bỏ cảm biến siêu âm trên các dòng xe điện](https://arstechnica.com/cars/2022/10/after-cutting-radar-tesla-now-dropping-ultrasonic-sensors-from-its-evs/)

Sau khi tuyên bố loại bỏ radar vào năm 2021 để chuyển hoàn toàn sang sử dụng thị giác máy tính qua camera hỗ trợ lái xe tự động (Tesla Vision), tháng này Tesla tiếp tục thông báo loại bỏ toàn bộ các cảm biến siêu âm lắp đặt tại cản trước và cản sau của xe:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100703.webp)

Cảm biến siêu âm vốn đóng vai trò đo đạc khoảng cách vật cản cự ly gần khi lùi hoặc đỗ xe. Việc loại bỏ phần cứng này đồng nghĩa tính năng tự động đỗ xe của Tesla sắp tới sẽ phụ thuộc hoàn toàn vào camera. Nhiều chuyên gia đặt câu hỏi liệu các mô hình AI thị giác máy tính của Tesla có đủ độ tin cậy để thay thế hoàn toàn các cảm biến vật lý này hay không.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100704.webp)

2、[Mỹ chế tạo thành công máy ảnh thiên văn lớn nhất thế giới](https://petapixel.com/2022/10/04/3200-megapixels-the-worlds-largest-camera-is-almost-complete/)

Các nhà khoa học Mỹ vừa hoàn thành việc lắp ráp mẫu máy ảnh thiên văn lớn nhất lịch sử, chuẩn bị vận chuyển đến lắp đặt tại một đài quan sát vũ trụ trên sa mạc Chile để ghi lại hình ảnh bầu trời đêm:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101002.webp)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101004.webp)

Thấu kính của máy ảnh có đường kính lên tới 1,57m, trọng lượng đạt 3 tấn và đã được chứng nhận kỷ lục Guinness cho thấu kính máy ảnh lớn nhất thế giới. Cảm biến ảnh của thiết bị có độ phân giải khổng lồ 3,2 tỷ pixel, ghép từ 189 cảm biến nhỏ lẻ và dự kiến kết xuất khoảng 15 TB dữ liệu thô mỗi đêm hoạt động:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101003.webp)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101006.webp)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101005.webp)

3、[Robot hai chân Cassie thiết lập kỷ lục chạy cự ly 100m](https://www.theverge.com/2022/9/30/23380061/bipedal-robot-100-meter-record-run-time-cassie-agility-robotics-osu)

Mẫu robot hai chân Cassie do Đại học Bang Oregon chế tạo vừa thiết lập kỷ lục Guinness thế giới mới cho robot hai chân chạy 100m với thời gian 24,73 giây:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100105.webp)

Dù kết quả này vẫn còn khoảng cách xa so với kỷ lục chạy 100m dưới 10 giây của con người, nhưng do robot không được nhấc cả hai chân khỏi mặt đất cùng lúc (tương đương đi bộ thể thao nhanh), tốc độ di chuyển của nó vẫn rất ấn tượng. 

Các kỹ sư cho biết phần khó nhất trong thiết kế giải thuật điều khiển không phải là duy trì thăng bằng khi di chuyển mà là xử lý gia tốc từ trạng thái đứng yên ban đầu và hãm tốc để đứng vững khi hoàn thành chặng chạy. (Xem [Video chạy thực tế](https://v.qq.com/x/page/v3359hf8oto.html)).

<iframe frameborder="0" src="https://v.qq.com/txp/iframe/player.html?vid=v3359hf8oto" allowFullScreen="true" width="600" height="400"></iframe>

Thiết bị cũng được tích hợp thêm hai cánh tay cơ khí hỗ trợ mang vác các gói hàng nhỏ:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100106.webp)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100201.webp)

4、[Phong trào vận động cấm đặt biển quảng cáo ngoài trời tại Anh](https://www.bbc.com/news/business-62806697)

Một tổ chức phi chính phủ tại Anh đang vận động chính phủ ban hành luật cấm đặt các biển quảng cáo thương mại ngoài trời tại các không gian đô thị công cộng để tránh ô nhiễm cảnh quan:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100501.webp)

Tổ chức bày tỏ lo ngại nếu không được kiểm soát tốt, quảng cáo thương mại sẽ bao phủ mọi mảng tường trống trên đường phố gây ảnh hưởng tới tâm lý người dân. Một nghiên cứu ghi nhận kể từ khi London ban hành lệnh cấm quảng cáo các sản phẩm đồ uống nhiều đường, thực phẩm nhiều muối và chất béo trên xe buýt và tàu điện ngầm vào năm 2019, thành phố đã giảm bớt gần 100.000 ca béo phì ở trẻ em.

5、[Sony ra mắt giải pháp ký chữ ký số chống giả mạo trên ảnh chụp](https://petapixel.com/2022/08/08/sonys-forgery-proof-tech-adds-crypto-signature-to-photos-in-camera/)

Hãng Sony công bố giải pháp nhúng trực tiếp chữ ký số mã hóa vào tệp hình ảnh ngay khi cảm biến thực hiện chụp:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082302.webp)

Công nghệ giúp bảo vệ bản quyền tác phẩm cho nhiếp ảnh gia trước sự phát triển của các công cụ chỉnh sửa ảnh AI: nếu tệp ảnh bị thay đổi dù chỉ 1 pixel, hệ thống kiểm tra chữ ký số sẽ phát hiện và cảnh báo bức ảnh đã bị chỉnh sửa. Tính năng hiện được triển khai thí điểm trên dòng máy ảnh cao cấp Sony Alpha 7 IV trước khi phổ cập rộng rãi.

## 文章

1\. [Phân tích nguyên nhân các nhà mạng chưa đẩy mạnh eSIM trên điện thoại](https://finance.sina.com.cn/jjxw/2022-09-29/doc-imqqsmrp0933136.shtml)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092907.webp)

Công nghệ thẻ SIM điện tử (eSIM) giúp người dùng dễ dàng chuyển đổi nhà mạng mà không cần thay thẻ SIM vật lý. Bài viết phân tích các nguyên nhân khiến các nhà mạng viễn thông trong nước chưa mặn mà với việc triển khai công nghệ này trên điện thoại thông minh do lo ngại tỷ lệ người dùng chuyển mạng giữ số tăng cao.

2\. [Đám cưới tổ chức trong vũ trụ ảo Metaverse gây chú ý](http://www.stcn.com/article/detail/698557.html)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101319.webp)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101318.webp)

Chủ tịch tập đoàn ZQGame đã thu hút sự chú ý khi tổ chức đám cưới của mình trong không gian ảo Metaverse, cho phép khách mời đăng nhập nhân vật 3D tham gia chúc mừng trực tuyến và nạp tiền quy đổi vàng ảo gửi bao lì xì mừng cưới.

3\. [Lý giải tại sao Trung Quốc cổ đại không phát triển mạnh ngành sản xuất thủy tinh](https://erikexamines.substack.com/p/did-the-teacup-hinder-chinese-scientific)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022082101.webp)

Tác giả phân tích dưới góc nhìn lịch sử: do kỹ nghệ sản xuất đồ gốm sứ thủ công của Trung Quốc cổ đại quá phát triển và đáp ứng tốt nhu cầu sinh hoạt hàng ngày (như uống trà), xã hội không có động lực nghiên cứu và phát triển các vật liệu thủy tinh trong suốt vốn là nền tảng chế tạo thấu kính phục vụ nghiên cứu vật lý học Tây phương.

4\. [Tìm hiểu chi tiết cơ chế kích hoạt lại kết xuất đồ họa trong thư viện React](https://www.joshwcomeau.com/react/why-react-re-renders/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022081704.webp)

Bài viết hướng dẫn chi tiết dành cho lập trình viên Front-end: giải thích cơ chế so sánh virtual DOM và các điều kiện state/props thay đổi khiến React kích hoạt quy trình re-render component để tối ưu hóa hiệu năng ứng dụng.

5\. [Tìm hiểu xu hướng phát triển web động vừa phải Mildly Dynamic Websites](https://www.devever.net/~hl/mildlydynamic)

Tác giả nhìn lại chặng đường phát triển web từ các trang tĩnh, trang động (PHP), trang blog tĩnh (Jekyll) đến các full-stack JS framework (Next.js) hiện đại, đề xuất xu hướng tương lai sẽ là các trang web tĩnh kết hợp một số thành phần động nhỏ tải từ server để tối ưu tốc độ và chi phí vận hành.

6\. [Cẩm nang giới thiệu 11 công cụ hữu ích trong bộ Microsoft PowerToys](https://www.fourth-wall.co.uk/post/powertoys-11-awesome-features-microsoft-won-t-add-to-windows)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022050901.webp)

Bài viết hướng dẫn chi tiết cách khai thác bộ công cụ nâng cao PowerToys do chính Microsoft phát hành cho hệ điều hành Windows bao gồm các tính năng hữu ích như ghim cửa sổ, chia màn hình nâng cao, đo màu và đổi tên file hàng loạt.

7\. [Giới thiệu tuyển tập 25 ứng dụng hữu ích giúp tăng hiệu năng trên macOS](https://medium.com/@parttimeben/10-little-macos-apps-that-make-a-big-difference-in-2022-part-1-c6428f92a079)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022070901.webp)

Loạt bài viết tổng hợp giới thiệu 25 phần mềm nhỏ gọn, chạy mượt mà và hầu hết được cung cấp miễn phí giúp tối ưu hóa trải nghiệm sử dụng phím tắt, clipboard và thanh menu trên hệ điều hành macOS.

## 工具

1、[Lyra: Thư viện tìm kiếm toàn văn lưu trữ trực tiếp trên bộ nhớ RAM viết bằng TS](https://lyrasearch.io/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080204.webp)

Bộ thư viện全文 search gọn nhẹ chạy cực nhanh trên RAM dành cho các ứng dụng JavaScript/TypeScript hỗ trợ thiết lập tính năng tìm kiếm nhanh không cần kết nối cơ sở dữ liệu ngoài.

2、[Fleet: Trình soạn thảo mã nguồn thế hệ mới từ JetBrains](https://www.jetbrains.com/fleet/)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101316.webp)

Công cụ soạn thảo code tối giản, khởi động siêu tốc thiết kế định hướng cạnh tranh trực tiếp với VS Code của Microsoft, tích hợp sẵn công cụ hỗ trợ code thông minh kế thừa từ IntelliJ IDEA. Hiện tại ứng dụng đang được mở thử nghiệm miễn phí.

3、[Make-A-Video: Mô hình AI hỗ trợ tạo video ngắn từ văn bản của Meta](https://makeavideo.studio/)

Hệ thống AI do Meta công bố cho phép người dùng nhập mô tả văn bản để tự động tạo ra một đoạn video ngắn tương ứng (bạn đọc cũng có thể tham khảo công cụ tương tự mang tên [Phenaki](https://phenaki.video/)).

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022093003.webp)

4、[Pagefind: Tiện ích tìm kiếm toàn văn chạy local cho trang web tĩnh](https://pagefind.app/)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080207.webp)

Giải pháp tìm kiếm tĩnh nguồn mở tự động xây dựng chỉ mục dữ liệu trong quá trình build để phục vụ tính năng tìm kiếm nhanh ngay tại trình duyệt client, không cần thiết lập máy chủ tìm kiếm.

5、[Howdz Dashboard: Extension trình duyệt hỗ trợ tùy biến thiết kế trang tab mới](https://github.com/leon-kfd/Dashboard)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101011.webp)

Tiện ích mở rộng nguồn mở dành cho Chrome/Firefox giúp người dùng tự thiết kế bố cục, phím tắt nhanh và hiển thị widget dự báo thời tiết trên trang Start Page. (Đóng góp của [@leon-kfd](https://github.com/ruanyf/weekly/issues/2673))

6、[MusicFree: Trình phát nhạc mã nguồn mở tùy biến nguồn nhạc trên Android](https://github.com/maotoumao/MusicFree)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101012.webp)

Ứng dụng nghe nhạc viết bằng React Native hỗ trợ người dùng tự viết các plugin để kết nối và nghe nhạc từ các nguồn lưu trữ đám mây hoặc trang chia sẻ nhạc cá nhân. (Đóng góp của [@maotoumao](https://github.com/ruanyf/weekly/issues/2674))

7、[pcl.js: Thư viện Point Cloud Library biên dịch sang WebAssembly](https://pcljs.org/zh-cn/)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101013.webp)

Dự án biên dịch bộ thư viện xử lý đám mây điểm 3D C++ (PCL) sang định dạng Wasm, giúp các ứng dụng JavaScript có thể chạy trực tiếp các thuật toán lọc điểm và dựng hình ảnh 3D trên trình duyệt. (Đóng góp của [@luoxuhai](https://github.com/ruanyf/weekly/issues/2676))

8、[OneDev: Nền tảng tự lưu trữ mã nguồn Git tích hợp CI/CD](https://github.com/theonedev/onedev)

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080304.webp)

Giải pháp tự vận hành repository Git thay thế GitHub/GitLab gọn nhẹ, tích hợp sẵn hệ thống build CI/CD tự động và bảng Kanban quản lý tiến độ công việc.

9、[Stormah: Ứng dụng ghi chú trực tuyến đồng bộ dữ liệu qua Git](https://stormah.com/)

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022061614.webp)

Trình soạn thảo ghi chú Markdown trực quan chạy trên Web, hỗ trợ đồng bộ lưu trữ toàn bộ dữ liệu ghi chép trực tiếp vào kho chứa Git cá nhân của người dùng.

10、[NoSleep.js: Thư viện JS ngăn chặn thiết bị di động tắt màn hình](https://github.com/richtr/NoSleep.js)

Giải pháp lập trình ngăn điện thoại chuyển sang chế độ ngủ tắt màn hình khi đang duyệt web bằng cách chạy ngầm một đoạn video vô hình siêu nhỏ lặp liên tục trên trang.

## 资源

1、[识典古籍: Nền tảng số hóa cổ tịch Trung Quốc trực tuyến](https://www.shidianguji.com/)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101320.webp)

Dự án hợp tác phi lợi nhuận giữa Đại học Bắc Kinh và ByteDance: số hóa và mở cổng tra cứu miễn phí hơn 390 bộ cổ tịch kinh điển với quy mô 30 triệu từ, hỗ trợ đắc lực cho công tác nghiên cứu văn học cổ.

2、[Deep Learning for Coders: Khóa học thực hành học sâu của fast.ai](https://course.fast.ai/)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072201.webp)

Chương trình đào tạo trực tuyến miễn phí hướng dẫn lập trình viên tiếp cận và xây dựng các dự án học máy, thị giác máy tính thực tế kèm theo kho tài nguyên mã nguồn mở đầy đủ.

3、[Tổng hợp tin nhắn riêng tư về thương vụ Twitter của Elon Musk](https://danluu.com/elon-twitter-texts/)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100701.webp)

Trang web tổng hợp và phân loại chi tiết các nội dung tin nhắn SMS trao đổi cá nhân của tỷ phú Elon Musk liên quan đến vụ kiện thâu tóm mạng xã hội Twitter do tòa án công bố công khai.

4、[Podcast.ai: Đoạn hội thoại phỏng vấn giả lập Steve Jobs bằng trí tuệ nhân tạo](https://podcast.ai/)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101106.webp)

Sản phẩm ứng dụng AI mô phỏng hoàn hảo giọng nói, ngữ điệu và tư duy tranh biện của Steve Jobs trong một buổi phỏng vấn giả lập dài 20 phút với người dẫn chương trình Joe Rogan.

## 图片

1\. [Hướng dẫn phương pháp bóc giấy ghi chú Post-it đúng cách](https://tylercipriani.com/blog/2022/05/28/on-the-proper-use-of-post-its/)

Cách bóc giấy ghi chú Post-it đúng cách để giữ nếp giấy phẳng phiu khi dán là thực hiện xé giấy theo chiều ngang từ cạnh bên thay vì bóc kéo ngược từ dưới lên trên (vốn làm cong mép dính giấy):

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053009.webp)

![](https://cdn.beekka.com/blogimg/asset/202205/bg2022053010.webp)

2\. [Hình ảnh so sánh sự phát triển của thấu kính viễn vọng chụp sao Mộc](https://twitter.com/BrianRoemmele/status/1579946200941617152)

Hình ảnh chụp sao Mộc ghi nhận qua các thời kỳ phát triển công nghệ kính thiên văn từ năm 1900 đến 2020:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101315.webp)

Từ hình ảnh một vệt bóng mờ đen trắng thô sơ ban đầu, sự phát triển của quang học và cảm biến số hiện đại đã giúp ghi lại chi tiết các dải mây bão khí quyển sắc nét của mộc tinh.

## 2022年诺贝尔生理医学奖

Giải Nobel Y sinh năm 2022 đã chính thức được trao cho nhà sinh vật học tiến hóa người Thụy Điển Svante Pääbo nhờ thành tựu đột phá trong việc giải mã thành công hệ gen của người Neanderthal - phân loài người cổ đã tuyệt chủng hàng chục vạn năm trước:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100301.webp)

Để vượt qua thử thách DNA cổ bị phân hủy nghiêm trọng trong xương hóa thạch đất đá suốt hàng trăm ngàn năm, ông đã cống hiến cả sự nghiệp nghiên cứu các phương pháp bảo tồn và bóc tách gen cổ sinh.

Tác phẩm tự truyện khoa học phổ thông nổi tiếng của ông mang tên *《Neanderthal Man: In Search of Lost Genomes》* mô tả chi tiết chặng đường nghiên cứu đầy khó khăn gian khổ nhưng tràn đầy đam mê khoa học. (Bản tin [Số 60](http://www.ruanyifeng.com/blog/2019/06/weekly-issue-60.html) từng đăng tải giới thiệu chi tiết cuốn sách này).

![](https://cdn.beekka.com/blogimg/asset/201906/bg2019061429.jpg)

## ✍️ Bài đọc thêm

### Phản ứng bất lực của một studio game nhỏ trước quyết định đóng cửa đột ngột Stadia của Google

Ngay sau thông tin Google khai tử nền tảng đám mây Stadia, đại diện một nhóm phát triển game độc lập đã chia sẻ bài đăng đầy phẫn uất trên diễn đàn Reddit:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101314.webp)

> *"Đội ngũ kỹ sư nhỏ của chúng tôi đã dành ròng rã suốt 5 tháng qua chỉ để thực hiện việc tối ưu hóa và porting trò chơi của mình tương thích với nền tảng đám mây Stadia. Lần gửi kiểm duyệt đầu tiên, nhân viên Google phản hồi danh sách hơn 20 lỗi kỹ thuật cần sửa. Sau hai tuần miệt mài vá lỗi gửi lại, họ tiếp tục gửi thêm 10 yêu cầu tinh chỉnh mới.*
> 
> *Chúng tôi đã đầu tư rất nhiều thời gian và công sức nghiên cứu sâu các API và công nghệ hệ thống riêng biệt của Stadia. Cuối cùng, vào ngày 29 tháng 9, chúng tôi đã hoàn tất việc sửa toàn bộ lỗi, game đã chạy rất mượt mà ổn định và sẵn sàng lên kệ. Thế nhưng, ngay sáng hôm sau (ngày 30 tháng 9), chúng tôi nhận được tin sét đánh qua báo chí rằng Google sẽ đóng cửa Stadia.*
> 
> *Chỉ sau một đêm, toàn bộ nỗ lực làm việc suốt 5 tháng qua của cả nhóm chính thức biến thành con số không.*
> 
> *Khi nhận tin dữ, tôi thậm chí vẫn đang ngồi build phiên bản phát hành cuối cùng trước máy tính. Tôi cảm thấy vô cùng hụt hẫng và bất lực. 5 tháng đó đáng lẽ chúng tôi có thể làm được rất nhiều việc có ích khác thay vì ném tài nguyên vào một dự án sắp chết của Google..."*

Bên dưới bài đăng, một độc giả đã đưa ra lời khuyên thiết thực:

> *"Việc bạn cần làm ngay bây giờ không phải là ngồi buồn bã hay trách móc nữa. Hãy nhanh chóng viết một bài phân tích chi tiết (post-mortem) chia sẻ chân thực về sự cố này và đăng tải lên các diễn đàn lớn.*
> 
> *Hãy tận dụng sự quan tâm của truyền thông đối với sự kiện Stadia để quảng bá cho trò chơi của bạn, biến đây thành cơ hội thu hút sự chú ý của cộng đồng game thủ để thúc đẩy doanh số bán game trên các nền tảng phân phối khác như Steam hoặc console."*

## 历史上的本周

- 2021年10月8日：[Năng lượng sạch: Xu hướng phát triển mạnh mẽ của giải pháp điện mặt trời áp mái tại các hộ gia đình](https://www.ruanyifeng.com/blog/2021/10/weekly-issue-178.html)
- 2020年10月9日：[Tư duy xã hội: Các phân tích khoa học trả lời câu hỏi liệu thế giới hiện đại có đang chuyển dịch theo hướng viễn tưởng "cyberpunk"](https://www.ruanyifeng.com/blog/2020/10/weekly-issue-128.html)
- 2019年10月4日：[Định hướng sự nghiệp: Cách thức chuyển đổi sở thích cá nhân thành một nghề nghiệp có thu nhập thông qua video ngắn](https://www.ruanyifeng.com/blog/2019/10/weekly-issue-76.html)
- 2018年10月5日：[Nhìn lại chặng đường phát triển 10 năm của hệ điều hành di động Android](https://www.ruanyifeng.com/blog/2018/10/weekly-issue-25.html)

## 鸣谢

Nền tảng quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072108.webp)

（Hết）
