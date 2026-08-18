# Bản tin chia sẻ công nghệ (Số 363): Giải thích mạng nơ-ron dễ hiểu nhất từ trước đến nay

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/7408) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082708.webp)

Tại khu du lịch thiên khanh (hố sụt) huyện La Thành, thành phố Hà Trì, Quảng Tây, người ta đã xây dựng một "hiệu sách treo vách đá" độc đáo lưng chừng núi — cảnh tượng vô cùng ấn tượng. (Nguồn: [news.cn](https://www.news.cn/culture/20250811/b6c23974a3dd42ae8b1c00340235238c/a.html))

## 最好懂的神经网络解释

Mạng nơ-ron là nền tảng thuật toán của AI.

Mấy ngày trước, tôi đọc được một [bài phổ biến khoa học](https://www.quantamagazine.org/how-can-ai-id-a-cat-an-illustrated-guide-20250430/) trên tạp chí khoa học phổ thông *Quanta Magazine* của Mỹ. Bài viết dùng một ví dụ cực kỳ đơn giản kết hợp hình minh họa để giải thích mạng nơ-ron — có thể nói là hướng dẫn dễ hiểu nhất tôi từng đọc.

Dưới đây là phiên bản tiếng Việt tôi tổng hợp lại.

**1.**

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082601.webp)

Trong máy tính của bạn có hàng đống ảnh, bạn muốn tìm ra những bức ảnh có con mèo — phải làm thế nào?

Bạn nhanh chóng nhận ra, đây thực chất là **bài toán phân loại của máy tính**: Máy tính cần phân ảnh thành hai loại — ảnh có mèo và ảnh không có mèo.

**2.**

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082801.webp)

Hãy hình dung bài toán này như một bản đồ, ở giữa có một đường ranh giới chia bản đồ thành hai vùng lãnh thổ.

Nhiệm vụ của bạn là xác định chính xác vị trí đường ranh giới đó. Khi đã tìm được, với bất kỳ điểm nào trên bản đồ, bạn đều biết ngay nó nằm bên trái hay bên phải đường ranh giới.

**3.**

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082802.webp)

Là điều kiện đã biết, nhiều điểm trên bản đồ đã được gắn nhãn. Ví dụ trong hình trên: Các điểm tam giác thuộc vùng A, các điểm vuông thuộc vùng B.

Nhiệm vụ của bạn là từ các điểm đã biết đó, suy ra đường ranh giới.

**4.**

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082602.webp)

Chúng ta có thể xây dựng một hàm toán học (điểm N trong hình trên) để giải quyết bài toán này.

Hàm số này nhận hai tham số là tọa độ x và y của mỗi điểm, và trả về một giá trị từ 0 đến 1, biểu thị xác suất điểm đó thuộc về vùng tương ứng.

**5.**

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082603.webp)

Bạn dùng các điểm đã biết nhãn để huấn luyện hàm số này.

Máy tính tự động điều chỉnh trọng số (weight) của từng tham số dựa trên sai số của mỗi lần huấn luyện, cuối cùng tìm ra đường ranh giới gần đúng nhất.

**6.**

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082803.webp)

Đường ranh giới thẳng tắp chỉ là trường hợp lý tưởng. Trong thực tế, ranh giới thường là một đường cong ngoằn ngoèo phức tạp.

**7.**

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082604.webp)

Lúc này, chỉ dùng một hàm số để xác định ranh giới là không đủ. Bạn cần nhiều hàm số, mỗi hàm phán đoán từ một góc độ khác nhau.

**8.**

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082605.webp)

Quá trình phán đoán thậm chí cần được thực hiện theo nhiều giai đoạn, tức là cần nhiều lớp hàm số.

Mạng lưới các hàm số này trông giống hệ thần kinh của con người, vì vậy nó được gọi là **mạng nơ-ron (neural network)**. Mỗi hàm số là một nơ-ron trong mạng.

**9.**

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082606.webp)

Bây giờ quay lại bài toán ảnh mèo. Chúng ta tương tự cần xây dựng một hàm số để tính xác suất một ảnh là ảnh mèo.

Hàm số bản đồ chỉ cần 2 tham số X và Y, nhưng hàm số ảnh mèo thì khác — cần đưa toàn bộ bức ảnh vào. Nếu ảnh có 2.500 pixel, thì hàm số có 2.500 tham số.

**10.**

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082607.webp)

Số lượng tham số của hàm số có thể coi là số chiều của không gian: 2 tham số là không gian 2 chiều, 2.500 tham số là không gian 2.500 chiều.

Hàm số ảnh mèo chính là: Trong không gian 2.500 chiều đó, thông qua huấn luyện với lượng dữ liệu khổng lồ, tìm ra một đường ranh giới — từ đó tính xác suất bất kỳ bức ảnh nào nằm bên trong đường ranh giới (là ảnh mèo) cao đến đâu.

## 科技动态

（1）Thành phố Thanh Đảo tuần này đã khánh thành **tòa nhà "zero carbon" (không carbon) đầu tiên trên thế giới**, sử dụng 100% năng lượng xanh tái tạo.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082501.webp)

Tòa nhà cao 117 mét, gồm 23 tầng, toàn bộ mặt dựng bên ngoài đều là kính quang điện mặt trời (photovoltaic glass), mỗi ngày có thể phát ra 1.500 kWh điện.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082502.webp)

Điểm thú vị nhất là tòa nhà có một phòng năng lượng dưới lòng đất, đặt 14 chiếc ô tô điện đã hết hạn sử dụng. Pin của những xe này được tận dụng để lưu trữ điện dự phòng cho các giờ cao điểm tiêu thụ.

Ngoài ra, các xe điện đỗ trong bãi đỗ xe của tòa nhà cũng được kết nối với lưới điện của tòa nhà, cung cấp điện ngược từ xe vào tòa nhà — và chủ xe được nhận phí cung cấp điện.

（2）Trường Đại học Y khoa Quảng Châu vừa hoàn thành ca phẫu thuật **ghép phổi lợn vào người đầu tiên trên thế giới**.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082611.webp)

Họ đã ghép một buồng phổi lợn đã được chỉnh sửa gen tại 6 vị trí vào cơ thể một bệnh nhân chết não.

Ban đầu, phổi lợn cung cấp oxy và thải CO₂ thành công, nhưng trong vòng 24 giờ, cơ quan bắt đầu có dấu hiệu tổn thương, và vào ngày thứ 3 và ngày thứ 9 có dấu hiệu cơ thể đào thải.

Gia đình bệnh nhân đồng ý thử nghiệm để ủng hộ nghiên cứu y học, nhưng yêu cầu kết thúc thử nghiệm vào ngày thứ 9. Là lần thử đầu tiên, kết quả được đánh giá là khả quan, tuy nhiên một số người chỉ trích rằng vì chỉ ghép phổi trái trong khi phổi phải vẫn còn nguyên vẹn, thử nghiệm này chưa chứng minh được phổi lợn có thể duy trì sự sống độc lập.

（3）Các nhà phát minh Hàn Quốc đã tạo ra một chiếc **máy dập ghim 90 độ**, có thể dập ghim thành hình chữ L vuông góc.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082508.webp)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082509.webp)

Loại máy dập ghim này có nhiều ưu điểm thiết thực: Tiết kiệm bìa carton thừa ở góc chồng lên nhau, đồng thời loại bỏ hoàn toàn nhu cầu dùng băng keo và keo dán ở các góc nối.

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082510.webp)

![](https://cdn.beekka.com/blogimg/asset/202506/bg2025082511.webp)

（4）Thương hiệu laptop Mỹ [Framework](https://frame.work/ro/en/laptop16?tab=whats-new), nổi tiếng với các laptop dạng module có thể tháo lắp linh kiện, vừa ra mắt chiếc laptop cho phép **thay thế cả CPU lẫn GPU** — theo tôi biết đây là chiếc đầu tiên trên thế giới.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082707.webp)

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082706.webp)

Hình trên là module GPU rời của máy: Chỉ cần mở nắp lưng laptop, kéo module ra là có thể thay thế. Cách tiếp cận này xứng đáng được phổ biến rộng rãi vì giúp giảm thiểu rác thải điện tử đáng kể.

（5）Khi một người mất đi, dữ liệu họ để lại vẫn tồn tại.

Một luật sư Mỹ gần đây đề xuất pháp luật nên thiết lập **quyền di sản kỹ thuật số của người đã khuất** (digital legacy rights) để ngăn chặn việc dữ liệu của họ bị khai thác.

Đa số mọi người khi mất đi không để lại di chúc hướng dẫn xử lý các nội dung đã tạo ra trên các nền tảng internet. Luật sư cho rằng pháp luật cần quy định rõ ràng, ngăn các nền tảng sử dụng nội dung người đã khuất để huấn luyện AI.

## 文章

1、[Google thông báo chương trình xác minh nhà phát triển Android](https://www.androidauthority.com/android-developer-verification-requirements-3590911/) (tiếng Anh)

Android từ trước đến nay vẫn cho phép cài đặt ứng dụng tùy ý mà không qua cửa hàng ứng dụng. Google có kế hoạch thay đổi điều này: Từ tháng 9 năm sau, tất cả nhà phát triển ứng dụng sẽ phải trải qua quá trình xác minh danh tính. Điện thoại Trung Quốc do không có framework Google ước tính sẽ không bị ảnh hưởng.

2、[Tại sao giao thức OAuth được thiết kế như vậy](https://www.ducktyped.org/p/an-illustrated-guide-to-oauth) (tiếng Anh)

OAuth là giao thức đăng nhập bên thứ ba, được thiết kế khá phức tạp. Bài viết giải thích lý do đằng sau từng chi tiết thiết kế một cách rõ ràng và thấu đáo, giúp người đọc hiểu ra nhiều điều.

3、[Hàm random() trong CSS](https://webkit.org/blog/17285/rolling-the-dice-with-css-random/) (tiếng Anh)

Bài giới thiệu cách sử dụng hàm sinh số ngẫu nhiên `random()` trong CSS để tạo ra các hiệu ứng như bầu trời sao, bánh xe quay... hoàn toàn bằng CSS thuần túy.

4、[So sánh Portainer và Dockge — Hai công cụ quản lý Docker container phổ biến](https://www.xda-developers.com/reasons-use-two-apps-manage-docker-containers/) (tiếng Anh)

Khi bạn đang chạy nhiều Docker container cùng lúc, cần có công cụ quản lý trực quan. Bài viết so sánh chi tiết hai lựa chọn phổ biến nhất hiện nay là Portainer và Dockge.

5、[Cách xem thông tin tiến trình trên Mac](https://til.simonwillison.net/macos/fs-usage) (tiếng Anh)

Mac OS có lệnh nội trang [fs_usage](https://ss64.com/mac/fs_usage.html) cực kỳ mạnh mẽ để theo dõi thông tin tiến trình, đặc biệt hữu ích khi muốn biết một tiến trình đang thao tác với file nào.

6、[Biến Kindle cũ thành bảng điều khiển cá nhân (personal dashboard)](https://samkhawase.com/blog/hacking-kindle/) (tiếng Anh)

Tận dụng màn hình e-ink của Kindle cũ: Bài viết hướng dẫn chuyển đổi nó thành một bảng điều khiển hiển thị thông tin cá nhân (thời tiết, lịch, tin tức...).

## 工具

1、[Gonzo](https://github.com/control-theory/gonzo)

Công cụ xem file log ngay trên terminal, hỗ trợ tô màu cú pháp và lọc nội dung.

2、[Filestash](https://github.com/mickael-kerjean/filestash)

Trình quản lý file chạy trên web, hỗ trợ kết nối với nhiều giao thức và dịch vụ đám mây: S3, FTP, WebDAV, Git, MySQL, Backblaze...

3、[Anchor Relay](https://anchor.dev/relay)

Dịch vụ trực tuyến cấp chứng chỉ HTTPS miễn phí.

4、[PlutoPrint](https://github.com/plutoprint/plutoprint)

Thư viện Python chuyển đổi trang web HTML hoặc mã HTML sang file PDF chất lượng cao.

5、[MarkFlowy](https://markflowy.vercel.app/zh)

Trình soạn thảo Markdown desktop đa nền tảng tích hợp hỗ trợ AI, mã nguồn mở. (Đóng góp từ [@drl990114](https://github.com/ruanyf/weekly/issues/7618))

6、[Pixel Art Generator](https://imgtopixel.art/)

Ứng dụng web chuyển đổi ảnh thành pixel art chỉ bằng một click, có thể tùy chỉnh kích thước pixel, số màu và bảng màu. (Đóng góp từ [@leah626888](https://github.com/ruanyf/weekly/issues/7619))

7、[Peek Pop](https://github.com/u-Sir/peek-pop)

Tiện ích mở rộng mã nguồn mở cho trình duyệt: Khi rê chuột qua một liên kết, hiện ra cửa sổ nhỏ xem trước nội dung trang đích mà không cần click vào. (Đóng góp từ [@u-Sir](https://github.com/ruanyf/weekly/issues/7626))

8、[naive-ui-pro](https://github.com/Zheng-Changfu/naive-ui-pro)

Giải pháp frontend cho bảng quản trị trung/hậu đài, xây dựng trên nền Vue 3 + Vite. (Đóng góp từ [@Zheng-Changfu](https://github.com/ruanyf/weekly/issues/7627))

9、[文件快传 (File Quick Transfer)](https://github.com/MatrixSeven/file-transfer-go)

Ứng dụng web truyền file P2P mã nguồn mở, dựa trên công nghệ WebRTC cho phép truyền trực tiếp giữa hai máy không qua máy chủ trung gian. (Đóng góp từ [@MatrixSeven](https://github.com/ruanyf/weekly/issues/7631))

10、[Dataset Viewer](https://github.com/stardustai/dataset-viewer)

Trình xem file desktop mã nguồn mở hỗ trợ hầu hết các định dạng phổ biến, có thể nhanh chóng xem file lớn và file nén cả ở local lẫn trên cloud. (Đóng góp từ [@F-loat](https://github.com/ruanyf/weekly/issues/7634))

11、[Trình tạo vở tập chép chữ Hán](https://luhuadong.com/tools/calligraphy-generator)

Ứng dụng web: Nhập văn bản tiếng Trung, tự động tạo ra trang tập chép chữ với ô lưới mi tự (米字格) và phiên âm pinyin bên trên. (Đóng góp từ [@luhuadong](https://github.com/ruanyf/weekly/issues/7652))

12、[Trợ lý cổng serial trực tuyến "Bên kia mây"](https://serial.xywml.com/)

Ứng dụng web hỗ trợ gỡ lỗi cổng serial (serial port) trực tuyến, tương thích với các thiết bị STM32, DSP và IoT. (Đóng góp từ [@xywml](https://github.com/ruanyf/weekly/issues/7658))

## AI 相关

1、[DeepWiki](https://deepwiki.com/)

Dịch vụ chuyển đổi bất kỳ kho chứa GitHub nào thành một trang Wiki chi tiết giải thích toàn bộ quá trình hoạt động của code — trợ thủ đắc lực khi đọc mã nguồn người khác. Xem thêm [hướng dẫn sử dụng](https://www.aitidbits.ai/p/deepwiki).

2、[Daily Commit Summarizer](https://github.com/nanbingxyz/daily-commit-summarizer)

Template GitHub Actions tự động tổng hợp tất cả commit của một repository trong ngày thành báo cáo tóm tắt và gửi lên Feishu (飞书). (Đóng góp từ [@nanbingxyz](https://github.com/ruanyf/weekly/issues/7612))

3、[VideoAdGuard](https://github.com/Warma10032/VideoAdGuard)

Tiện ích mở rộng mã nguồn mở cho trình duyệt, sử dụng AI để tự động nhận diện và bỏ qua các đoạn quảng cáo được chèn vào video trên Bilibili. (Đóng góp từ [@Warma10032](https://github.com/ruanyf/weekly/issues/7646))

## 资源

1、[Atlas of Space (Bản đồ vũ trụ)](https://atlasof.space/)

Bản đồ hệ Mặt Trời trực tuyến, hiển thị vị trí và chuyển động của từng hành tinh theo ngày thực tế.

2、[all text in nyc](https://www.alltext.nyc/)

Trang web đã thực hiện nhận dạng chữ viết (OCR) trên toàn bộ ảnh street view của New York City, cho phép tìm kiếm bất kỳ từ nào và xem nó xuất hiện ở đâu trên bảng hiệu/biển đường phố New York.

3、[Mechanical Library (Thư viện cơ học)](https://mechanical-library.org/)

Trang web giới thiệu chi tiết 8 loại cơ cấu cơ học (ví dụ như [bánh răng giảm tốc](https://mechanical-library.org/gear-reduction)) kèm hình ảnh minh họa động.

4、[Is this tech dead?](https://www.isthistechdead.com/)

Nhập tên một công nghệ vào, trang web sẽ đánh giá dựa trên nhiều chỉ số (độ phổ biến trên mạng, tần suất cập nhật mã nguồn...) và cho biết công nghệ đó đã "chết" chưa.

## 图片

1、[Nhà ga đáng sợ nhất Nhật Bản](https://www.tokyocowboy.co/articles/doai-eki-japans-creepiest-station)

Ga Doai nằm ở ranh giới tỉnh Gunma và Niigata, Nhật Bản, là nhà ga không có nhân viên trực, được mệnh danh là nhà ga đáng sợ nhất đất nước mặt trời mọc.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082612.webp)

Nhà ga nằm sâu trong lòng núi. Từ cổng vào, phải đi bộ xuống theo 462 bậc thang dài 338 mét (hình dưới) đào xuyên qua đá mới đến được sân ga.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082613.webp)

Sân ga u tối lạnh lẽo, thêm tiếng nước ngầm chảy róc rách vang lên từ lòng đất.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082614.webp)

Trên sân ga chỉ có một phòng chờ nhỏ xíu và một nhà vệ sinh.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082615.webp)

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082616.webp)

Trong phòng chờ có để sẵn giấy bút để du khách để lại lời nhắn và dán ảnh — một phần để giúp giết thời gian chờ đợi.

![](https://cdn.beekka.com/blogimg/asset/202508/bg2025082617.webp)

Những lời nhắn ẩn danh và ảnh dán trên tường càng làm tăng thêm không khí kỳ bí cho nhà ga ngầm như hang động này — như đang lạc vào thế giới của trò chơi Silent Hill.

## 文摘

1、**Sự bất tiện làm bạn trở nên mạnh mẽ hơn**

Một cuốn sách bán chạy từng đề xuất khái niệm "hiệu ứng kích thích" (hormesis): Một lượng nhỏ áp lực hoặc cảm giác bất tiện sẽ giúp chúng ta trở nên mạnh mẽ hơn.

- Luyện tập nâng tạ → cơ bắp phát triển.
- Tiêm vaccine → miễn dịch tăng cường.
- Chấp nhận rủi ro thất bại → tự tin tăng trưởng.
- Giải quyết bài toán khó → khả năng sáng tạo mở rộng.

"Hiệu ứng kích thích" này cũng áp dụng cho não bộ: Thường xuyên suy nghĩ về những vấn đề khó, để tư duy của bạn được thử thách — đó chính là cách bạn học được cách tư duy thực sự.

Nhưng giờ đây với AI, nhiều người giao vấn đề cho AI suy nghĩ hộ và để não mình nghỉ ngơi. Tôi lo ngại rằng theo thời gian, chúng ta sẽ dần đánh mất khả năng tư duy, cho đến khi trở thành những cỗ máy sinh học.

Một nghiên cứu gần đây cho thấy: Các nhà khoa học yêu cầu những người tham gia hoàn toàn dựa vào AI để viết luận văn. Kết quả là 83% số người sau khi hoàn thành, không thể trích dẫn bất kỳ nội dung nào trong luận văn của chính mình. Ngay cả khi sau đó được yêu cầu viết lại độc lập, họ vẫn thể hiện hoạt động thần kinh não bộ giảm sút và không thể tập trung tư duy hoàn toàn, luôn có thói quen tìm kiếm sự trợ giúp của AI.

Các nhà nghiên cứu đặt ra thuật ngữ "nợ nhận thức" (cognitive debt) để mô tả hiện tượng này: AI mang lại sự tiện lợi, nhưng cái giá phải trả là hi sinh năng lực tư duy của chúng ta.

Máy móc cho bạn mượn sức mạnh trí tuệ, nhưng bạn phải trả lãi — bằng chính năng lực tư duy của mình.

Lời khuyên của tôi là: Hãy sử dụng AI một cách thông minh. Đừng để AI giải phương trình thay bạn — hãy để AI kiểm tra đáp án của bạn và giải thích chỗ nào bạn sai. Nguyên tắc là kiên trì tư duy độc lập, sau đó mới kết hợp AI vào.

Tư duy có thể làm bạn mệt mỏi và bất tiện, nhưng nó là sân tập của não bộ — sự bất tiện làm cho tư duy của bạn mạnh mẽ hơn.

## 言论

1、

Tôi cho rằng TSMC (Đài tích điện) là một trong những công ty tốt nhất trong lịch sử nhân loại, và bất kỳ ai muốn mua cổ phiếu TSMC đều là người rất thông minh.

-- *Jensen Huang (Hoàng Nhân Huân), Chủ tịch Nvidia, khi được phóng viên Đài Loan hỏi về khả năng chính phủ Mỹ mua cổ phần TSMC. Câu trả lời này không đắc tội bất kỳ ai, mà lại khiến tất cả đều vui lòng — ông thực sự là bậc thầy về ngôn từ.*

2、

Hệ thống phân tán (distributed system) không phải là hệ thống phân bổ trên nhiều máy tính khác nhau, mà là hệ thống bao gồm từ hai tiến trình tương tác trở lên, bất kể chúng có nằm trên cùng một máy chủ hay không.

-- *Trích bài viết 《Hệ thống phân tán thực ra là gì》*

3、

Mô hình AI lớn là một cách nén thông tin — dù không chính xác hoàn toàn, có ảo giác và thiếu sót, nhưng vẫn tốt hơn không có gì. Các mô hình AI lớn thực chất là một khung nhìn nén có mất mát nhưng có thể sử dụng và truy cập công khai về internet.

-- *Trích bài viết 《Trọng số của mô hình AI lớn là một phần của lịch sử》*

4、

Trước đây, viết phần mềm tốt hơn làm thủ công; bây giờ, viết câu lệnh AI (prompt) tốt hơn viết phần mềm.

-- *Trích bài viết 《Lập trình bằng câu lệnh nhắc》*

5、

Khi mô hình whisper-large-v3 chuyển đổi giọng nói từ video tiếng Trung, nó tự động sinh ra văn bản "Chỉ để học tập/nghiên cứu, vui lòng xóa sau 48 giờ" ở những đoạn im lặng. Điều này chứng tỏ nó được huấn luyện bằng các file phụ đề từ các nhóm dịch phim.

-- *Độc giả Hacker News*

## 往年回顾

- Số #316: [Câu chuyện về cuộc đời của bạn — Suy ngẫm về ý nghĩa và hành trình cuộc sống](https://www.ruanyifeng.com/blog/2024/09/weekly-issue-316.html)
- Số #266: [Tự tạo sách điện tử EPUB song ngữ của riêng bạn](https://www.ruanyifeng.com/blog/2023/08/weekly-issue-266.html)
- Số #216: [Sự chiến thắng của chủ nghĩa tối giản trong thiết kế và lối sống](https://www.ruanyifeng.com/blog/2022/07/weekly-issue-216.html)
- Số #166: [Học qua video có thực sự tốt hơn đọc sách không?](https://www.ruanyifeng.com/blog/2021/07/weekly-issue-166.html)

(Hết)
