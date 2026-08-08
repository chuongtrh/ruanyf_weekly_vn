# 科技爱好者周刊（第 236 期）：中国的阳光地带

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần。

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn。

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2771) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập。

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121606.webp)

Rạng sáng ngày 16 tháng 12, bể cá hình trụ đứng lớn nhất thế giới AquaDom (cao 14m) đặt tại hành lang một khách sạn ở Berlin, Đức bất ngờ bị nứt vỡ hoàn toàn. Nguyên nhân ban đầu được xác định do nhiệt độ ban đêm ngoài trời hạ xuống quá thấp gây co ngót làm nứt vỡ kính cường lực. Sự cố khiến hơn 1.000 tấn nước cùng 1.500 chú cá nhiệt đới tràn ra đường phố bên ngoài. (Nguồn: [The Guardian](https://www.theguardian.com/world/2022/dec/16/huge-cylindrical-aquarium-housing-1500-exotic-fish-bursts-in-berlin))

## 本周话题：中国的阳光地带

Bước vào mùa đông, thời tiết tại Thượng Hải luôn trong trạng thái âm u và lạnh lẽo. Thỉnh thoảng lắm mới có những ngày mặt trời ló rạng.

Mỗi khi mùa đông đến, tôi lại nhen nhóm ý định chuyển đến một thành phố khác để tránh rét, tìm đến những nơi có nhiều ánh nắng ấm áp.

Năm nay thực sự lên kế hoạch di chuyển, tôi muốn tìm hiểu xem **những thành phố nào có lượng nắng nhiều nhất cả nước.**

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122007.webp)

Trong khí tượng học có một chỉ số thống kê cụ thể gọi là [“Thời lượng nắng hàng năm”](https://en.wikipedia.org/wiki/Sunshine_duration) (sunshine duration). Bách khoa toàn thư Wikipedia chỉ ra 3 yếu tố tự nhiên quyết định đến chỉ số này:

1. **Khí hậu khô hạn**: Những vùng khô hạn, ít mưa sẽ có lượng nắng nhiều hơn hẳn vùng ẩm ướt.
2. **Độ cao địa hình**: Các vùng cao nguyên có tầng khí quyển mỏng hơn, ít mây che phủ nên thời lượng nắng dài hơn.
3. **Vĩ độ**: Các vùng có vĩ độ cao thường có thời gian mặt trời lơ lửng gần đường chân trời lâu hơn, giúp thời gian nhận ánh sáng kéo dài hơn khi mặt trời xuống thấp.

Mọi trạm khí tượng đô thị đều thống kê tham số này và số liệu chi tiết được công bố trong cuốn *《Niên giám Thống kê Trung Quốc》* hàng năm. Tra cứu biểu đồ thống kê năm gần nhất, tôi đã lập danh sách so sánh.

Trước tiên là danh sách 10 đô thị có thời lượng nắng ít nhất cả nước:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122009.webp)

Không ngoài dự đoán, khu vực lòng chảo Tứ Xuyên (Thành Đô, Trùng Khánh) là nơi có lượng nắng ít nhất cả nước. Điều gây bất ngờ là phần lớn các đô thị lớn thuộc khu vực Hoa Trung, Hoa Đông và Hoa Nam cũng nằm trong nhóm nhận được lượng nắng khá khiêm tốn.

Còn dưới đây là danh sách 10 đô thị có thời lượng nắng nhiều nhất:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122010.webp)

Bảng xếp hạng này mang lại nhiều bất ngờ. Việc các thành phố thuộc khu vực cao nguyên (Thanh Tạng, Vân Quý) dẫn đầu là điều dễ hiểu do ưu thế địa hình. Tuy nhiên, các khu vực miền Đông Bắc, Hoa Bắc và Tây Bắc cũng sở hữu thời lượng nắng vô cùng dồi dào.

Điều này phản ánh một thực tế: Các tỉnh phía Bắc thực chất là một dải đất ngập tràn ánh nắng ấm áp vào mùa đông nhờ ưu thế khí hậu khô ráo và vĩ độ cao. Nếu các đô thị tại đây được chú trọng cải thiện môi trường cảnh quan và phủ xanh tốt, đây chắc chắn sẽ là những địa điểm rất lý tưởng để sinh sống vào mùa đông nhờ nguồn ánh sáng mặt trời dồi dào.

## 科技动态

1、[Dự án kính thực tế ảo VR dạng mũ bảo hiểm sử dụng khi nằm bị hủy bỏ](https://news.nweon.com/89728)

Một startup công nghệ của Nhật Bản vừa chính thức [thông báo](https://diver-x.jp/news/en/20220131.html) dừng dự án phát triển thiết bị kính thực tế ảo VR dạng mũ bảo hiểm (Diver-X) chuyên dụng cho người nằm trên giường do gặp khó khăn về tài chính và rào cản công nghệ:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072610.webp)

Ý tưởng của dự án khá độc đáo: thiết bị được thiết kế như một chiếc gối ôm quây kín đầu tích hợp kính hiển thị và tai nghe cao cấp giúp người dùng có thể thoải mái nằm lướt web hoặc chơi game VR:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072611.webp)

Do tư thế nằm không thể thao tác bằng chuột hay tay cầm chơi game thông thường, hãng đã thiết kế một cặp cảm biến đeo ở lòng bàn chân để người dùng điều khiển con trỏ bằng góc nghiêng của bàn chân.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072612.webp)

2、[Xu hướng ứng dụng công nghệ game engine trong ngành xây dựng](https://spectrum.ieee.org/unreal-engine)

Trong các dự án xây dựng lớn, việc thiết lập mô hình 3D trực quan để giới thiệu công trình hoàn thiện cho khách hàng là nhu cầu bắt buộc. Thay vì sử dụng các phần mềm dựng hình kiến trúc truyền thống, nhiều văn phòng thiết kế lớn đang chuyển dịch mạnh mẽ sang sử dụng các bộ công cụ phát triển game (game engine) như Unreal Engine:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080202.webp)

Nguyên nhân do năng lực kết xuất đồ họa, giả lập ánh sáng thời gian thực của game engine vượt trội hoàn toàn so với phần mềm kiến trúc cổ điển. Thư viện asset phong phú của game engine cũng giúp thiết kế viên dễ dàng chèn nhanh các mô hình cây cối, xe cộ sinh động vào bản vẽ:

![](https://cdn.beekka.com/blogimg/asset/202208/bg2022080203.webp)

Hơn nữa, game engine cho phép xuất ra các tour tham quan thực tế ảo 3D giúp khách hàng có thể tự do di chuyển góc nhìn khám phá mọi ngóc ngách của tòa nhà tương lai một cách chân thực nhất. Dịch vụ dựng hình VR này dự kiến sẽ phát triển thành một ngành công nghiệp phụ trợ xây dựng lớn.

3、[Sản xuất xi măng sinh học bằng công nghệ nuôi cấy tảo](https://interestingengineering.com/biogenic-limestone-from-microalgae)

Ngành sản xuất xi măng truyền thống là một trong những tác nhân gây ô nhiễm không khí lớn nhất thế giới do quá trình nung đá vôi giải phóng lượng khí CO2 khổng lồ vào khí quyển:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022063012.webp)

Một giáo sư đại học tại Mỹ đã đề xuất giải pháp kỹ thuật độc đáo: tận dụng quá trình kết tủa carbonat tự nhiên của sinh vật để tự nuôi cấy đá vôi sinh học:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022063013.webp)

Ông sử dụng loài vi tảo Coccolithophore có khả năng hấp thụ khí CO2 mạnh mẽ qua quang hợp để tự tạo ra lớp vỏ carbonat canxi cứng xung quanh tế bào. Bằng cách nuôi cấy loài tảo này ở quy mô công nghiệp, chúng ta có thể thu hoạch được lượng bột đá vôi sinh học chất lượng cao phục vụ sản xuất xi măng xanh hoàn toàn không phát thải khí nhà kính.

4、[Ý tưởng máy in mini sử dụng cuộn giấy chạy liên tục](https://minimalissimo.com/articles/roller-jet-printer)

Các dòng máy in văn phòng thông thường được thiết kế để in trên các khổ giấy cố định (như A4), gây lãng phí một lượng lớn giấy trắng nếu người dùng chỉ có nhu cầu in một vài dòng thông tin ngắn.

Một nhà thiết kế Hàn Quốc đã giới thiệu mẫu máy in mini Roller Jet Printer sử dụng lõi giấy cuộn chạy liên tục:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022091001.webp)

Thiết bị cho phép in các đoạn văn bản có độ dài bất kỳ và tự động cắt giấy theo đúng độ dài của nội dung, rất thích hợp để in nhanh các hóa đơn, ghi chú hoặc nhãn dán công việc cầm tay:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022091002.webp)

Máy sử dụng công nghệ in nhiệt trực tiếp nên không cần trang bị hộp mực hay mực ruy-băng, giúp tối giản hóa thiết kế phần cứng của máy in.

5、[Màu áo đấu màu kem bị loại bỏ tại giải bóng rổ NBA do công nghệ truyền hình](https://paullukas.substack.com/p/exclusive-the-inside-story-of-why)

Đội bóng rổ Milwaukee Bucks (NBA) vừa qua đã chính thức thông báo từ bỏ mẫu trang phục thi đấu màu kem sữa truyền thống của câu lạc bộ:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111701.webp)

Nguyên nhân bắt nguồn từ việc các đài truyền hình hiện nay ứng dụng các phần mềm tự động chèn quảng cáo và bảng số liệu thống kê thời gian thực lên mặt sân bóng.

Dưới hệ thống đèn chiếu sáng cường độ cao của sân đấu, sắc độ màu kem sữa của áo cầu thủ rất gần với tông màu gỗ sồi của mặt sân. Phần mềm tự động nhận diện mặt sân để chèn quảng cáo đôi lúc bị nhầm lẫn và chèn đè hình ảnh quảng cáo lên thân người cầu thủ, tạo nên những hình ảnh hiển thị kỳ lạ trên sóng truyền hình (như phần quần đùi cầu thủ bị biến mất hoàn toàn):

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111702.webp)

Hiện tượng tương tự cũng được ghi nhận trong các trận đấu khúc côn cầu trên băng khi áo đấu cầu thủ bị lẫn vào màu trắng của mặt băng:

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022111703.webp)

## 文章

1\. [Giải thích dễ hiểu về đột phá năng lượng trong phản ứng hạt nhân nhiệt hạch](https://mp.weixin.qq.com/s/44H689gZQ-26ZbzC9D-RTg)（Tiếng Trung）

Bài viết tóm tắt khoa học đại chúng giải thích về sự kiện Bộ Năng lượng Mỹ công bố đạt được bước tiến lớn "net energy gain" (độ lợi năng lượng thuần - lượng năng lượng thu về lớn hơn năng lượng kích hoạt ban đầu) trong phản ứng hạt nhân nhiệt hạch kiểm soát, mở ra triển vọng về nguồn năng lượng sạch vô tận cho nhân loại. (Đóng góp của [@marmul2](https://github.com/ruanyf/weekly/issues/2811))

2\. [Phân tích các ưu thế địa lý tự nhiên độc nhất vô nhị của nước Mỹ](https://unchartedterritories.tomaspueyo.com/p/world-chessboard)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122106.webp)

Bài phân tích chi tiết về mặt địa chính trị và kinh tế học lý giải các ưu thế địa lý của Mỹ: hai đại dương lớn bao bọc cô lập, vùng đồng bằng trung tâm rộng lớn màu mỡ phục vụ nông nghiệp và hệ thống sông ngòi nội địa dài có khả năng liên thông vận tải thủy giá cực rẻ. Bài viết đính kèm hình ảnh so sánh trực quan kích thước khổng lồ của thuyền tầm bảo của Trịnh Hòa thời Minh so với thuyền vượt đại dương của Colombo.

3\. [Hướng dẫn chi tiết giới thiệu về mạng xã hội phi tập trung Mastodon](https://wordsmith.social/elilla/a-futuristic-mastodon-introduction-for-2021)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110306.webp)

Bài viết giới thiệu chi tiết cho người dùng về kiến trúc hoạt động phi tập trung (decentralized) sử dụng giao thức ActivityPub của mạng xã hội Mastodon, hướng dẫn cách lựa chọn server instance và tham gia cộng đồng.

4\. [CDN Bunny.net ứng dụng AI tự động sinh ảnh đại diện thỏ độc bản](https://bunny.net/blog/introducing-bunny-optimizer-ai-a-new-way-of-creating-content/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121602.webp)

Nhà cung cấp dịch vụ CDN Bunny.net chia sẻ giải pháp kỹ thuật thú vị: tích hợp mô hình AI tạo ảnh tự động sinh ra các ảnh đại diện hình chú thỏ độc bản không trùng lặp cho mỗi khách hàng mới đăng ký tài khoản.

5\. [Hướng dẫn cách sử dụng thẻ `<picture>` tối ưu hóa hiển thị ảnh đa kích thước](https://jfhr.me/optimizing-images-with-the-html-picture-tag/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202211/bg2022110309.webp)

Bài hướng dẫn cơ bản cho lập trình viên Front-end cách thức sử dụng thẻ `<picture>` trong HTML5 kết hợp thẻ `<source>` để trình duyệt tự động lựa chọn kích thước ảnh phù hợp nhất theo độ rộng màn hình của thiết bị.

6\. [Mẹo thiết lập tối giản hóa trang web loại bỏ yêu cầu tải favicon](https://tdarb.org/blog/under-1kb.html)（Tiếng Anh）

Tác giả chia sẻ các mẹo tối ưu hóa mã nguồn HTML để nén dung lượng trang web xuống dưới mốc 1KB, trong đó có thủ thuật chèn chuỗi mã hóa để ngăn trình duyệt tự động gửi yêu cầu HTTP tải tệp tin biểu tượng `favicon.ico`.

7\. [Lợi thế trường tồn của cơ sở dữ liệu quan hệ so với NoSQL](https://www.simplethread.com/relational-databases-arent-dinosaurs-theyre-sharks/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072613.webp)

Bài viết lập luận sắc bén chứng minh các hệ quản trị cơ sở dữ liệu quan hệ (RDBMS) truyền thống sử dụng ngôn ngữ truy vấn SQL vẫn giữ vai trò xương sống của ngành phần mềm nhờ tính nhất quán giao dịch (ACID) vượt trội so với các trào lưu NoSQL.

8\. [8 quan niệm sai lầm phổ biến về hệ thống mạng phân tán](https://architecturenotes.co/fallacies-of-distributed-systems/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060504.webp)

Bài viết phân tích sâu sắc các quan niệm sai lầm kinh điển của lập trình viên khi bắt tay thiết kế kiến trúc phân tán (như giả định mạng luôn tin cậy, độ trễ bằng không, băng thông vô hạn), giải thích các bài toán phức tạp của hệ thống phân tán thực tế.

## 工具

1、[tremor: Thư viện component UI React chuyên dụng cho bảng dữ liệu Dashboard](https://www.tremor.so/)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022101103.webp)

Bộ thư viện mã nguồn mở cung cấp các React components thiết kế hiện đại, tinh gọn hỗ trợ lập trình viên xây dựng nhanh các trang Dashboard quản trị hiển thị các biểu đồ số liệu.

2、[GPTAnywhere: Tiện ích mở nhanh giao diện tương tác ChatGPT trên Chrome](https://chrome.google.com/webstore/detail/gptanywhere/pklibapjplkpanekidgnckgjablljhni)

Plugin trình duyệt cho phép người dùng nhấp chọn nhanh biểu tượng trên thanh công cụ để mở ngay khung hội thoại tương tác với ChatGPT mà không cần mở tab trang chủ.

3、[Obsidian Canvas: Tính năng thiết lập sơ đồ tư duy trực quan trên Obsidian](https://obsidian.md/canvas)

Công cụ ghi chú nổi tiếng Obsidian vừa phát hành tính năng Canvas cho phép người dùng tạo một không gian vô cực kéo thả tự do để liên kết các ghi chú, hình ảnh thành dạng sơ đồ tư duy (mindmap) trực quan:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122104.webp)

4、[Enhance Speech: Tiện ích lọc nhiễu âm nâng cao chất lượng giọng nói AI của Adobe](https://podcast.adobe.com/enhance)

Ứng dụng web chạy AI miễn phí của hãng Adobe hỗ trợ người dùng tải lên các file ghi âm giọng nói thông thường chứa tạp âm để hệ thống tự động lọc sạch tiếng ồn, tái tạo chất giọng trong trẻo như đang thu âm trong phòng thu chuyên nghiệp.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121904.webp)

5、[One Tab Group: Tiện ích quản lý và đồng bộ nhóm tab trình duyệt](https://www.onetab.group/)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122111.webp)

Extension Chrome hỗ trợ người dùng gom nhóm các tab đang mở ngăn nắp, quản lý bộ nhớ đệm và hỗ trợ đồng bộ hóa danh sách tab lên đám mây. (Đóng góp của [@xiaoluoboding](https://github.com/ruanyf/weekly/issues/2812))

6、[Forgejo: Dự án git client phi thương mại tách ra từ Gitea](https://forgejo.org/)

Sau khi đội ngũ quản trị phần mềm Gitea quyết định thành lập công ty thương mại, một nhóm nhà phát triển cộng đồng lo ngại mất tính mở đã tách nhánh (fork) mã nguồn để xây dựng dự án Forgejo hoạt động phi lợi nhuận độc lập:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121603.webp)

7、[Satori: Thư viện JavaScript chuyển đổi HTML/CSS sang định dạng SVG](https://github.com/vercel/satori)

Thư viện JS gọn nhẹ do Vercel phát triển hỗ trợ biên dịch nhanh các thẻ HTML và thuộc tính định dạng CSS cơ bản thành một tệp hình ảnh đồ họa vector SVG động, rất hữu ích để tự động sinh các ảnh xem trước (OG image) cho trang web.

8、[Agreper: Diễn đàn tối giản viết bằng Python hoàn toàn không dùng JS](https://github.com/Demindiro/agreper)

Dự án mã nguồn xây dựng diễn đàn thảo luận tối giản viết bằng Python, điểm đặc biệt là hệ thống vận hành hoàn toàn dựa trên cơ chế HTTP request truyền thống và không cần tải bất kỳ dòng code JavaScript nào ở trình duyệt client.

9、[Rmt.rs: Tiện ích dòng lệnh CLI thay thế lệnh rm tích hợp thùng rác](https://github.com/AmineZouitine/rmt.rs)

Công cụ dòng lệnh viết bằng Rust hoạt động tương tự lệnh xóa tệp `rm` nhưng thay vì xóa vĩnh viễn, tệp tin sẽ được chuyển vào một thư mục thùng rác (recycle bin) tạm thời để người dùng có thể khôi phục lại khi cần.

## 资源

1、[Sundial Zone: Hướng dẫn tự chế tạo đồng hồ mặt trời bằng giấy cứng](https://www.sundialzone.com/zh/)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022091802.webp)

Trang web học tập khoa học hướng dẫn chi tiết cách vẽ sơ đồ và cắt dán giấy bìa cứng để tự chế tạo một chiếc đồng hồ mặt trời (nhật quỹ) xem giờ dựa vào bóng nắng mặt trời tại tọa độ nhà bạn.

2、[The Ruby Reference (Tài liệu tra cứu học ngôn ngữ lập trình Ruby)](https://rubyreferences.github.io/rubyref/)

Trang web tổng hợp tài liệu hướng dẫn học và tra cứu nhanh cú pháp, các phương thức xây dựng sẵn của ngôn ngữ lập trình Ruby trực tuyến hoàn toàn miễn phí.

3、[Kho tải bộ sưu tập hình nền mặc định độ phân giải 6K của hệ điều hành macOS](https://512pixels.net/projects/default-mac-wallpapers-in-5k/)

Trang web tổng hợp và cung cấp link tải hình ảnh chất lượng cao độ phân giải 5K và 6K các bức ảnh phong cảnh đại diện mặc định của mọi phiên bản macOS từ xưa đến nay:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071426.webp)

4、[The Algorithms: Kho lưu trữ mã nguồn thuật toán đa ngôn ngữ lớn trên GitHub](https://the-algorithms.com/zh_Hans)

Dự án tổng hợp các cách triển khai viết mã nguồn của hàng trăm bài toán thuật toán thông dụng phân loại theo ngôn ngữ lập trình (Java, Python, C++, Go...) trên GitHub hỗ trợ đắc lực cho việc ôn tập thuật toán.

## 图片

1\. **Các dòng thiết bị máy khai thác mỏ hầm hố của Nga sản xuất**

Hình ảnh các dòng máy cào và khai thác khoáng sản dưới lòng đất mã hiệu 1ГПКС do Nga sản xuất phục vụ khai thác mỏ than. Thiết bị có thiết kế cơ khí thô ráp, đồ sộ mang đậm phong cách khoa học viễn tưởng:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071702.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071704.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071705.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022071706.webp)

2\. **Mở bán đấu giá mô hình robot cơ khí nguyên bản của nhân vật ET năm 1982**

Mô hình cơ khí cử động của nhân vật người ngoài hành tinh ET sử dụng trong bộ phim khoa học viễn tưởng kinh điển *E.T. the Extra-Terrestrial (1982)* của đạo diễn lừng danh Steven Spielberg vừa qua được đưa ra đấu giá với mức giá khởi điểm ước tính lên tới 2,5 triệu USD:

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122107.webp)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122108.webp)

Nếu bộ phim được sản xuất ở thời điểm hiện tại, đoàn làm phim chắc chắn sẽ không đầu tư chế tạo mô hình cơ khí phức tạp đắt đỏ này mà thay thế hoàn toàn bằng công nghệ ghi hình chuyển động (motion capture) kết hợp kỹ xảo máy tính (CGI).

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122109.webp)

3\. **Tượng Thần Chiến Thắng Samothrace cẩm thạch không đầu nổi tiếng**

Bức tượng Winged Victory of Samothrace (tạc tác phẩm nữ thần Nike dang cánh trên mũi tàu chiến cổ đại) bằng đá cẩm thạch không đầu trưng bày ở bậc thang lớn bảo tàng Louvre nước Pháp, là một trong những kiệt tác điêu khắc Hy Lạp cổ đại có sức ảnh hưởng nhất lịch sử:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072001.webp)

Tác phẩm được tìm thấy dưới đáy biển biển Địa Trung Hải trong trạng thái bị vỡ mất phần đầu và hai tay:

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072002.webp)

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072003.webp)

## ✍️ Bài đọc thêm

### Bài học bảo mật đắt giá từ sự cố hệ thống thanh toán lỗi tại Uber Eats Ấn Độ

Khoảng 3 năm trước, ứng dụng gọi đồ ăn Uber Eats tại thị trường Ấn Độ đã gặp phải một sự cố hệ thống vô cùng nghiêm trọng liên quan đến cơ chế xử lý thanh toán trực tuyến, giúp hàng ngàn người dùng có thể đặt đồ ăn hoàn toàn miễn phí mà không mất tiền:

Một buổi sáng, một khách hàng tại Ấn Độ thực hiện đặt đồ ăn trên Uber Eats và lựa chọn thanh toán qua ví điện tử Paytm. Tuy nhiên do tài khoản ví Paytm của anh không đủ số dư, giao dịch lập tức bị báo lỗi thất bại và đơn hàng không được tạo.

Không từ bỏ, người này tiếp tục nhấn nút đặt lại đơn hàng một lần nữa. Kỳ lạ thay, lần thứ hai hệ thống lập tức báo đặt hàng thành công dù ví của anh vẫn không hề có tiền nạp.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122206.webp)

Thông tin về lỗ hổng đặt đồ ăn miễn phí này nhanh chóng lan truyền chóng mặt trên mạng xã hội. Lượng đơn hàng rác tăng vọt trong thời gian ngắn khiến hàng loạt nhà hàng quá tải và buộc phải tạm dừng nhận đơn. Đội ngũ Uber Eats sau khi phát hiện sự cố đã lập tức tắt tính năng thanh toán qua ví Paytm để khắc phục lỗi.

Kết quả điều tra nguyên nhân sự cố chỉ ra lỗi bắt nguồn từ một cập nhật mã nguồn tưởng chừng vô hại của đội ngũ kỹ sư Paytm vào ngày hôm trước: **Họ đã thay đổi mã lỗi phản hồi của API thanh toán thất bại từ cơ chế nhất quán (Idempotent) sang bất nhất quán (Non-idempotent).**

Tính nhất quán (Idempotency) của API quy định rằng: nếu bạn gửi lặp lại cùng một yêu cầu HTTP API, hệ thống phải luôn trả về một phản hồi đồng nhất.

* Trước khi cập nhật, nếu ví không đủ tiền, API của Paytm luôn trả về cùng một mã lỗi:
  - Yêu cầu thanh toán lần 1 không đủ tiền -> Phản hồi: `Error_Code_A`
  - Yêu cầu thanh toán lần 2 không đủ tiền -> Phản hồi: `Error_Code_A`

* Sau khi cập nhật, Paytm thay đổi mã phản hồi của lần lỗi tiếp theo:
  - Yêu cầu thanh toán lần 1 không đủ tiền -> Phản hồi: `Error_Code_A`
  - Yêu cầu thanh toán lần 2 không đủ tiền -> Phản hồi: `Error_Code_B`

Sự thay đổi nhỏ này đã đụng phải lỗi logic nghiêm trọng trong mã nguồn xử lý của Uber Eats: Các lập trình viên Uber Eats viết code giả định API này luôn nhất quán. Mã nguồn của họ chỉ so sánh phản hồi của lần yêu cầu thứ 2 với lần thứ 1, **nếu thấy chuỗi phản hồi khác nhau lập tức mặc định coi là giao dịch thứ hai đã thực hiện thành công và chuyển trạng thái đơn hàng sang đã thanh toán.**

Sự cố khiến cả hai tập đoàn lớn phải gánh chịu thiệt hại chi phí bù tiền cho các nhà hàng đối tác và là bài học đắt giá cho các lập trình viên về tầm quan trọng của việc thống nhất cấu trúc API và viết mã kiểm tra logic thanh toán chặt chẽ.

## 历史上的本周

- 2021年（第 188 期）：[Thảo luận nghệ thuật: Tại sao thói quen đeo tai nghe thưởng thức âm nhạc cá nhân vô tình làm gia tăng sự cô lập xã hội](https://www.ruanyifeng.com/blog/2021/12/weekly-issue-188.html)
- 2020年（第 138 期）：[Quan điểm cuộc sống: Đối mặt với làn sóng sa thải công nghệ, lập trình viên nên chuẩn bị kế hoạch tái cấu trúc định hướng bản thân](https://www.ruanyifeng.com/blog/2020/12/weekly-issue-138.html)
- 2019年（第 86 期）：[Lời khuyên nghề nghiệp: Tại sao lập trình viên không nên cố gắng trở thành một người theo đuổi chủ nghĩa hoàn hảo cực đoan](https://www.ruanyifeng.com/blog/2019/12/weekly-issue-86.html)
- 2018年（第 35 期）：[Xu hướng tiêu dùng: Phân tích sự bùng nổ của các mô hình kinh doanh dịch vụ đóng gói dành riêng cho khách hàng đơn thân](https://www.ruanyifeng.com/blog/2018/12/weekly-issue-35.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2771) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## 鸣谢

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202207/bg2022072108.webp)

（Hết）
