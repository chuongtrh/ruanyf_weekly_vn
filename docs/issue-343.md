# Bản tin chia sẻ công nghệ (Số 343): Làm thế nào để chặn AI Crawler

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua, phát hành vào thứ Sáu hàng tuần. (**[Thông báo] Tuần tới là kỳ nghỉ lễ Thanh minh, bản tin sẽ tạm nghỉ.**)

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly)), hoan nghênh gửi issue, đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/6189) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin việc làm lập trình viên, hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập. Hợp tác xin vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032602.webp)

Mô hình nông trại "Dâu tây trên không" độc đáo tại Lâm Bình, Hàng Châu. Các giỏ trồng dâu tây được bố trí trên các khung thép treo lơ lửng giữa không trung, có khả năng tự động nâng lên hoặc hạ xuống theo nhu cầu chăm sóc. (Nguồn: [163.com](https://www.163.com/dy/article/JRHE1LAS05149IKJ.html))

## 如何阻止 AI 爬虫

Các công ty phát triển mô hình lớn AI hiện nay đang điên cuồng thu thập dữ liệu huấn luyện từ khắp nơi trên thế giới.

**Họ liên tục gửi đi vô số robot cào dữ liệu (crawlers) để quét sạch thông tin trên Internet mà hầu như không có bất kỳ sự kiềm chế nào**. Số lượng robot truy cập quá lớn với tần suất cực cao tạo ra áp lực tải tương đương với các cuộc tấn công từ chối dịch vụ (DDoS) nhắm vào các máy chủ web.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032303.webp)

Tuần trước, người quản trị nền tảng lưu trữ mã nguồn SourceHut đã chính thức công bố [bài viết phân tích](https://thelibre.news/foss-infrastructure-is-under-attack-by-ai-companies/) (hình dưới), bày tỏ sự phẫn nộ trước hành vi **quét dữ liệu quá mức của các AI crawlers** làm máy chủ gặp sự cố quá tải nghiêm trọng và buộc phải tạm ngắt kết nối dịch vụ.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032304.webp)

Ông vô cùng bức xúc khi chỉ ra các robot cào dữ liệu này hoàn toàn phớt lờ các quy định khai báo trong tệp tin cấu hình tiêu chuẩn `robots.txt`. Chúng cố gắng quét sạch từng trang thông tin, từng đường dẫn liên kết và từng commit nhỏ nhất bên trong mọi kho lưu trữ Git trên hệ thống.

Các robot này sử dụng hàng vạn địa chỉ IP phân tán trên toàn cầu kết hợp cùng việc giả lập ngẫu nhiên các chuỗi khai báo User-Agent để ngụy trang tinh vi như một người dùng thông thường truy cập web, gây khó khăn lớn cho việc nhận diện và chặn lọc bằng các giải pháp thông thường.

Điều đáng bức xúc hơn cả là ngay sau khi hoàn thành chu kỳ cào dữ liệu toàn bộ hệ thống, chỉ đúng 6 tiếng sau, các robot này lại quay trở lại để tiếp tục quét lại chính những nội dung cũ đó một lần nữa!

Định kỳ mỗi tuần, người quản trị phải dành từ 20% đến 100% quỹ thời gian làm việc chỉ để xử lý các sự cố quá tải máy chủ do AI crawlers gây ra. SourceHut đã bị sập nguồn dịch vụ vài lần, đây là một sự cố chí tử đối với một công cụ cung cấp dịch vụ dạng SaaS.

Cuối cùng, ông khẳng định đây hoàn toàn không phải là sự cố cá biệt của riêng SourceHut mà toàn bộ các doanh nghiệp vận hành hạ tầng Internet hiện nay đều đang là nạn nhân chịu ảnh hưởng nghiêm trọng.

> "Những người bạn làm quản trị hệ thống của tôi đều đang phải đối mặt với các bài toán tương tự hằng ngày. Mỗi khi chúng tôi ngồi uống bia hoặc ăn tối cùng nhau, chủ đề câu chuyện nhanh chóng được dịch chuyển sang việc than phiền về các AI bots. Sự bất lực và tuyệt vọng hiển hiện rõ rệt trong các cuộc thảo luận đó."

Vậy có giải pháp kỹ thuật khả thi nào để giúp ngăn chặn các đợt cào dữ liệu điên cuồng này của AI crawlers hay không?

Giải pháp đơn giản nhất là kích hoạt [tính năng bảo vệ miễn phí](https://blog.cloudflare.com/declaring-your-aindependence-block-ai-bots-scrapers-and-crawlers-with-a-single-click/) do Cloudflare cung cấp, mạng lưới CDN của họ sẽ tự động nhận diện và chặn lọc các AI crawlers giúp bạn.

Tuy nhiên, một số dịch vụ doanh nghiệp đặc thù không phù hợp để cấu hình đi qua Cloudflare, đòi hỏi quản trị viên phải tự xây dựng giải pháp chặn lọc nội bộ.

Hôm nay tôi xin giới thiệu một công cụ chuyên dụng giải quyết bài toán này mang tên **Anubis**.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032306.webp)

Đây là một cổng trung gian ngược (Reverse Proxy) ứng dụng cơ chế xác thực bằng làm việc chứng minh (Proof-of-Work - PoW). Với mô hình reverse proxy, **toàn bộ các yêu cầu truy cập từ bên ngoài hướng tới website đích sẽ bắt buộc phải đi qua nó trước tiên**.

Đầu tiên, bạn cần khởi tạo một máy chủ chạy dịch vụ Anubis và cấu hình đặt nó ở phía trước website đích làm reverse proxy (ví dụ như khai báo cấu hình dưới đây):

```
reverse_proxy http://localhost:3000
```

Hệ quả là khi người dùng gửi yêu cầu truy cập, giao diện hiển thị đầu tiên họ nhìn thấy không phải là trang web đích mà là trang xác thực của Anubis (hình dưới).

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032305.webp)

Trang web này sẽ tự động kích hoạt một đoạn mã nguồn JavaScript chạy trực tiếp trên trình duyệt của người dùng để thực hiện các phép tính toán học phức tạp. Chỉ sau khi trình duyệt tìm ra đáp án chính xác gửi về máy chủ xác thực, người dùng mới được cấp quyền tiếp tục truy cập vào website đích.

Quy trình tính toán này đòi hỏi thời gian thực thi nhất định, thông thường mất từ 1 đến 2 phút để hoàn thành.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032307.webp)

(Chú thích ảnh: Thử nghiệm trên trình duyệt di động ở hình trên mất tới 1 phút 53 giây mới hoàn thành phép tính).

Đối với các robot cào dữ liệu tự động, việc mỗi lượt gửi yêu cầu HTTP đều bắt buộc phải tiêu tốn một lượng tài nguyên tính toán khổng lồ để nhận về dữ liệu sẽ làm quá tải hệ thống máy chủ cào của họ, từ đó buộc họ phải tự động từ bỏ việc quét dữ liệu trang web của bạn.

Tất nhiên, người dùng thật khi truy cập trang web cũng sẽ phải trải qua chu trình xác thực tính toán này, gây ảnh hưởng tiêu cực đến trải nghiệm lướt web. Tuy nhiên giải pháp này vẫn tốt hơn nhiều so với việc để mặc cho các bot cào dữ liệu làm sập hoàn toàn máy chủ dịch vụ của bạn.

Vậy cụ thể Anubis yêu cầu trình duyệt của người dùng phải thực hiện phép tính toán gì?

Cụ thể, trình duyệt sẽ chạy đoạn code dưới đây để thực hiện phép tính băm (hash):

```javascript
const hash = await sha256(`${challenge}${nonce}`);
```

Đoạn code sử dụng thuật toán mã hóa SHA256 để tính toán giá trị băm của một chuỗi ký tự đầu vào.

Chuỗi ký tự này được cấu thành từ hai thành phần: Thành phần thứ nhất là `challenge` được sinh ra tự động từ các thông tin công khai của phiên truy cập (bao gồm địa chỉ IP của người dùng, chuỗi User-Agent của trình duyệt, ngày hiện tại và khóa công khai của máy chủ Anubis).

Thành phần thứ hai là `nonce` đại diện cho số lượt lặp tính toán, bắt đầu chạy thử từ mốc 1, tăng dần lên 2, 3... qua từng lượt lặp.

Thiết lập mặc định của Anubis yêu cầu **chuỗi kết quả băm tính ra phải có 5 ký tự đầu tiên đều bằng 0**. Nếu kết quả chưa thỏa mãn, giá trị `nonce` sẽ tự động tăng thêm 1 đơn vị để tiếp tục thực hiện lượt lặp tính toán tiếp theo cho đến khi tìm ra kết quả hợp lệ.

Trong nhiều kịch bản, trình duyệt sẽ phải thực hiện lặp đi lặp lại hàng triệu phép tính băm mới tìm ra đáp án đúng. Các bạn có hiểu biết về đồng Bitcoin chắc chắn sẽ nhận ra ngay: **Đây chính là thuật toán khai thác (mining) của Bitcoin**. Do quy trình đào Bitcoin tiêu tốn lượng điện năng và năng lực tính toán cực lớn, việc Anubis ứng dụng cơ chế này sẽ giúp tiêu tốn cực mạnh tài nguyên CPU của hệ thống máy chủ cào dữ liệu của đối phương.

Ngay sau khi trình duyệt tìm ra giá trị `nonce` hợp lệ (kết quả băm có 5 chữ số 0 đầu tiên), nó sẽ gửi giá trị này về máy chủ Anubis để xác thực nhanh. Nếu kết quả chính xác, Anubis sẽ tự động chuyển hướng người dùng đến trang web đích, đồng thời thiết lập một tệp tin Cookie trên trình duyệt của họ để ghi nhớ trạng thái xác thực nhằm tránh việc kích hoạt lại quy trình tính toán cho các yêu cầu truy cập tiếp theo.

Đó chính là toàn bộ nguyên lý vận hành của giải pháp chặn bot cào dữ liệu. Nguyên lý hoạt động vô cùng trực quan và quy trình triển khai kỹ thuật cũng tương đối đơn giản.

Các số liệu thực tế đã chứng minh tính hiệu quả vượt trội của giải pháp này. Một quản trị viên chia sẻ: Trong vòng 2,5 tiếng chạy thử nghiệm, website của ông ghi nhận tổng cộng 81.000 lượt yêu cầu truy cập, trong đó chỉ có vỏn vẹn 3% số lượt truy cập thực hiện thành công quy trình xác thực PoW của Anubis. Điều này đồng nghĩa với việc có tới 97% lượng băng thông truy cập trước đó thực chất đều là từ robot tự động!

Một con số thực sự kinh ngạc phản ánh mức độ猖獗 (hoạt động điên cuồng) của các AI crawlers hiện nay. Nếu trang web của bạn cũng đang đối mặt với bài toán quá tải do robot cào dữ liệu gây ra mà hoàn toàn không thể chuyển dịch qua dịch vụ của Cloudflare, giải pháp xác thực PoW của Anubis là một lựa chọn rất đáng cân nhắc.

## 科技动态

1、Đại học Khai mỏ và Công nghệ Trung Quốc công bố nghiên cứu chế tạo thành công mẫu robot khai thác tài nguyên vũ trụ độc đáo.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032605.webp)

Thiết kế robot trang bị hệ thống 6 chân đa năng, trong đó có 3 chân tích hợp bánh xe di chuyển và 3 chân còn lại thiết kế dạng móng vuốt phục vụ tác vụ đào bới khai thác khoáng sản.

2、Người dân tại khu vực Vương quốc Anh tuần này đồng loạt chia sẻ hình ảnh về hiện tượng đám mây xoắn ốc phát sáng kỳ lạ xuất hiện trên bầu trời đêm.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032610.webp)

Cơ quan Khí tượng Anh sau khi tiến hành xác minh đã đưa ra thông báo giải thích: Hiện tượng này thực chất được tạo ra bởi luồng khí thải thoát ra từ động cơ của tên lửa Falcon 9 (SpaceX) trong quá trình tự xoay chuyển箭 thể khi phóng.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032611.webp)

Luồng khí thải gặp nhiệt độ cực lạnh trong không gian vũ trụ đã lập tức bị đóng băng, tạo nên các tinh thể phản chiếu ánh sáng mặt trời tạo thành hình ảnh đám mây phát sáng đẹp mắt.

3、Các nhà khoa học đưa ra giả thuyết mới cho rằng nguồn gốc sơ khai của sự sống trên Trái Đất nhiều khả năng không bắt nguồn từ đại dương đại dương, mà được hình thành tại các khu vực hồ chứa nước kiềm (sodium carbonate) khép kín có quy mô lớn.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032604.webp)

Bởi lẽ các phản ứng hóa học sơ khởi hình thành nên sự sống đòi hỏi môi trường có nồng độ phốt pho cực cao. Hàm lượng phốt pho trong nước đại dương tự nhiên là rất thấp, trong khi các hồ nước kiềm giàu phốt pho là môi trường lý tưởng đáp ứng tốt điều kiện hóa học này.

4、Hãng sản xuất Yeston giới thiệu dòng sản phẩm card đồ họa GPU độc đáo tích hợp tính năng tỏa hương thơm khi vận hành.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032607.webp)

Thiết bị được thiết kế tích hợp các khay chứa sáp thơm chuyên dụng bên trong. Khi hệ thống hoạt động và quạt tản nhiệt quay sẽ tự động khuếch tán hương thơm ra không gian phòng làm việc của người dùng.

5、**Các tin tức khác**

(1) Báo cáo thống kê từ Cloudflare cho thấy có tới **41% số lượng yêu cầu đăng nhập trên Internet hiện nay đang sử dụng các thông tin mật khẩu đã bị rò rỉ trước đó** trong các vụ hack dữ liệu. Nguyên nhân cốt lõi do đại bộ phận người dùng vẫn duy trì thói quen sử dụng chung một mật khẩu cho nhiều tài khoản dịch vụ khác nhau.

(2) Thống kê từ Hiệp hội Nghiên cứu Giấc ngủ Trung Quốc cho thấy trong năm 2025, **quỹ thời gian ngủ trung bình ban đêm của người dân đạt mốc 6,85 giờ**, tăng nhẹ 6 phút so với năm trước. Mốc thời gian đi ngủ trung bình ghi nhận vào lúc 0h18 đêm, trễ hơn khoảng 17 phút so với số liệu năm trước.

(3) Một công trình nghiên cứu y khoa công bố kết luận việc duy trì chế độ ăn uống giới hạn thời gian trong ngày dưới 8 tiếng (nhịn ăn gián đoạn 16:8) mang lại hiệu quả hỗ trợ giảm cân và cải thiện các chỉ số sức khỏe vô cùng rõ rệt đối với những người thừa cân.

## 文章

1、**Đánh giá mô hình lớn Gemini 2.5 Pro**

Tuần này, Google đã chính thức công bố thế hệ mô hình lớn mạnh nhất của hãng mang tên [Gemini 2.5 Pro](https://blog.google/technology/google-deepmind/gemini-model-thinking-updates-march-2025/), nhanh chóng vươn lên dẫn đầu các bảng xếp hạng hiệu năng.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032801.webp)

Lập trình viên nổi tiếng Simon Willison đã tiến hành [chạy thử nghiệm đánh giá chuyên sâu](https://simonwillison.net/2025/Mar/25/gemini/) và đưa ra những phản hồi khen ngợi rất cao về năng lực xử lý của mô hình mới.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032714.webp)

[Một lập trình viên khác](https://everything.intellectronica.net/p/negotiating-with-the-machine) đã thử thách mô hình bằng một bài toán lập trình vô cùng phức tạp. Sau một thời gian phân tích suy nghĩ, hệ thống AI đã đưa ra phản hồi thẳng thắn nhận định yêu cầu này quá phức tạp để có thể hoàn thành chỉ trong một bước xử lý duy nhất, và đề xuất giải pháp thu nhỏ quy mô bài toán để hoàn thiện một phiên bản tối giản trước tiên.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032701.webp)

Phản hồi này làm giới công nghệ kinh ngạc. Bởi các thế hệ AI trước đây khi đối mặt với các bài toán vượt quá năng lực thường có xu hướng tự động sinh ra các câu trả lời sai lệch (hallucinations), trong khi thế hệ AI mới này đã sở hữu khả năng tự phân tích và chủ động thừa nhận giới hạn năng lực của bản thân.

2、[Tin tức: Google có kế hoạch hạn chế tính mở của dự án Android](https://www.androidauthority.com/google-android-development-aosp-3538503/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032702.webp)

Nguồn tin rò rỉ cho biết Google đang lên kế hoạch khép kín hóa quy trình nghiên cứu phát triển hệ điều hành Android, ngừng tiếp nhận các đóng góp mã nguồn (pull requests) từ cộng đồng phát triển bên ngoài nhằm giảm thiểu các xung đột kỹ thuật phát sinh trong quy trình đồng bộ hóa giữa phiên bản Android mã nguồn mở (AOSP) với phiên bản thương mại nội bộ của hãng.

Theo định hướng mới, Google sẽ hoàn thiện các bản cập nhật Android mới và phân phối trước cho các đối tác phần cứng (OEMs), sau đó mới phát hành bản sao mã nguồn mở AOSP lên hệ thống mà hoàn toàn không tiếp nhận thêm các đóng góp chỉnh sửa từ bên ngoài.

3、[Phân tích lỗ hổng bảo mật liên quan đến cấu trúc Middleware của Next.js](https://simonwillison.net/2025/Mar/23/nextjs-and-the-corrupt-middleware/) (tiếng Anh)

Tuần này, cộng đồng bảo mật ghi nhận một lỗ hổng nghiêm trọng trên bộ khung Next.js. Nếu quy trình xác thực đăng nhập của hệ thống được lập trình xử lý bên trong cấu trúc Middleware, tin tặc hoàn toàn có thể khai thác lỗ hổng để vượt qua bước xác thực này và truy cập trái phép vào tài khoản. Bài viết phân tích chi tiết cơ chế phát sinh lỗ hổng từ mã nguồn.

4、[Hướng dẫn khai báo kiểu dữ liệu cho hàm trong TypeScript](https://bhoot.dev/2025/typescript-function-type-syntaxes/) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032201.webp)

Bài viết hướng dẫn kỹ thuật cơ bản giới thiệu 3 phương thức khai báo kiểu dữ liệu (types definition) chuyên dụng cho các hàm xử lý trong ngôn ngữ TypeScript.

5、[Góc nhìn phản biện về giao thức Model Context Protocol (MCP)](https://taoofmac.com/space/notes/2025/03/22/1900) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032501.webp)

MCP là giao thức chuẩn hóa cổng kết nối giữa các ứng dụng và mô hình AI do hãng Anthropic đề xuất. Tác giả bài viết đưa ra các lập luận phản biện chỉ ra những nhược điểm và sự bất tiện của giao thức này trong quá trình lập trình thực tế.

6、[Khuyến nghị chuyển dịch hoàn toàn sang mô hình Module ESM](https://antfu.me/posts/move-on-to-esm-only) (tiếng Anh)

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032612.webp)

Tác giả đưa ra các lập luận khẳng định đã đến lúc lập trình viên JavaScript có thể hoàn toàn từ bỏ định dạng module CommonJS truyền thống để chuyển dịch hoàn toàn sang chuẩn module ESM hiện đại, đặc biệt khi câu lệnh `require` mặc định hiện đã hỗ trợ tốt việc import các module ESM trực tiếp.

## 工具

1、[CSS FlexCode](https://github.com/xutao-o/css-flex-code)

Tiện ích mở rộng trên VS Code hỗ trợ lập trình viên nhanh chóng sinh mã nguồn CSS cho các cấu trúc bố cục Flexbox và Grid thông qua các biểu tượng giao diện trực quan. (Đóng góp từ [@xutao-o](https://github.com/ruanyf/weekly/issues/6347))

2、[StreamCap](https://github.com/ihmily/StreamCap)

Ứng dụng máy tính (hỗ trợ cả hệ điều hành Windows và macOS) chuyên dụng cho việc ghi hình tự động các chương trình phát sóng trực tiếp (livestreams), hỗ trợ kết nối với hơn 40 nền tảng livestream lớn trong và ngoài nước dựa trên lõi công nghệ FFmpeg. (Đóng góp từ [@ihmily](https://github.com/ruanyf/weekly/issues/6393))

3、[Bilibili History Analyzer](https://github.com/2977094657/BilibiliHistoryFetcher)

Bộ công cụ hỗ trợ người dùng trích xuất và quản lý lịch sử xem video trên Bilibili cá nhân, hỗ trợ các tính năng tải video tự động, phân tích thống kê số liệu và kết nối AI tóm tắt nội dung video, phát triển bằng Python và SQLite. (Đóng góp từ [@2977094657](https://github.com/ruanyf/weekly/issues/6366))

4、[GoRead](https://github.com/Ray-D-Song/goread)

Dự án mã nguồn mở phát triển công cụ đọc sách điện tử định dạng EPUB trực tiếp bên trong giao diện dòng lệnh terminal viết bằng ngôn ngữ Go. (Đóng góp từ [@Ray-D-Song](https://github.com/ruanyf/weekly/issues/6369))

5、[GateShift](https://github.com/ourines/GateShift)

Công cụ dòng lệnh viết bằng Go hỗ trợ quản trị viên nhanh chóng chuyển đổi cấu hình cổng kết nối mạng (Gateway) mặc định trên máy tính chỉ bằng một câu lệnh duy nhất, rất hữu ích cho các mạng gia đình trang bị song song cả router OpenWrt và router thường. (Đóng góp từ [@ourines](https://github.com/ruanyf/weekly/issues/6353))

6、[Drawnix](https://github.com/plait-board/drawnix)

Dịch vụ bảng vẽ trực tuyến mã nguồn mở tích hợp đa năng các tính năng vẽ sơ đồ tư duy, sơ đồ quy trình và bộ công cụ cọ vẽ đồ họa trực quan. (Đóng góp từ [@pubuzhixing8](https://github.com/ruanyf/weekly/issues/6379))

7、[Xiaomi Notes Obsidian Plugin](https://github.com/emac/obsidian-minote-plugin)

Tiện ích mở rộng dành cho ứng dụng ghi chú Obsidian hỗ trợ tự động đồng bộ hóa và chuyển đổi toàn bộ các ghi chú của bạn trên ứng dụng Xiaomi Notes sang định dạng Markdown để lưu trữ nội bộ. (Đóng góp từ [@emac](https://github.com/ruanyf/weekly/issues/6355))

8、[wxlogin](https://github.com/liyaodev/wxlogin)

Giải pháp mã nguồn mở xây dựng tính năng đăng nhập trang web thông qua tương tác với tài khoản WeChat Official Account phát triển trên Next.js, người dùng lấy mã xác thực gửi từ Official Account để đăng nhập vào trang web. (Đóng góp từ [@liyaodev](https://github.com/ruanyf/weekly/issues/6372))

9、[Docxy](https://github.com/harrisonwang/docxy)

Dịch vụ proxy trung gian mã nguồn mở hỗ trợ kết nối tải nhanh các gói container từ kho chứa Docker Hub. (Đóng góp từ [@harrisonwang](https://github.com/ruanyf/weekly/issues/6395))

10、[Bondma](https://github.com/HeroIsUseless/bondma)

Hệ thống quản lý dịch thuật đa ngôn ngữ mã nguồn mở, cung cấp giao diện quản trị Web UI trực quan giúp kiểm soát các bản dịch của dự án. (Đóng góp từ [@HeroIsUseless](https://github.com/ruanyf/weekly/issues/6389))

11、[DeepPDF](https://deeppdf.ai/pdf-translator)

Dịch vụ trực tuyến miễn phí hỗ trợ dịch thuật nhanh các tài liệu PDF sang ngôn ngữ khác mà vẫn bảo toàn nguyên vẹn cấu trúc dàn trang và định dạng ban đầu của tệp tin. (Đóng góp từ [@icaohongyuan](https://github.com/ruanyf/weekly/issues/6398))

12、[RSSPod](https://rsspod.pro)

Dịch vụ web tối giản chuyên dụng cho việc tìm kiếm, đăng ký và thưởng thức các chương trình podcast trực tuyến. (Đóng góp từ [@Jaksay](https://github.com/ruanyf/weekly/issues/6399))

13][Supa Simple Socket](https://github.com/JustinGastby/supa-simple-socket)

Thư viện JavaScript client gọn nhẹ hỗ trợ giao thức kết nối WebSocket, tích hợp sẵn cơ chế gửi tin nhắn kiểm tra trạng thái kết nối (heartbeat), tự động kết nối lại khi mất mạng, quản lý đăng ký sự kiện và hỗ trợ truyền tải tệp tin. (Đóng góp từ [@JustinGastby](https://github.com/ruanyf/weekly/issues/6406))

14、[Inscribed.app](https://inscribed.app/)

Dịch vụ web hỗ trợ người dùng nhanh chóng phác họa các ý tưởng thiết kế và tạo các đoạn phim hoạt họa ngắn dựa trên cấu trúc các slide thuyết trình. (Đóng góp từ [@chunrapeepat](https://github.com/ruanyf/weekly/issues/6388))

15、[LinkAndroid](https://github.com/modstart-lib/linkandroid)

Ứng dụng kết nối di động mã nguồn mở giúp đơn giản hóa quy trình kết nối và truyền tải dữ liệu giữa điện thoại Android và máy tính. (Đóng góp từ [@modstart](https://github.com/ruanyf/weekly/issues/6408))

16、[Teleprompter.today](https://www.teleprompter.today/)

Dịch vụ máy nhắc chữ (Teleprompter) trực tuyến miễn phí hỗ trợ đắc lực cho các diễn giả, nhà sáng tạo nội dung video và streamer với các tùy biến đa dạng về định dạng văn bản hiển thị. (Đóng góp từ [@s87343472](https://github.com/ruanyf/weekly/issues/6412))

## AI 相关

1、[Web Design AI Agent](https://github.com/mggger/WebCraft)

Ứng dụng AI mã nguồn mở hỗ trợ tự động thiết kế và xuất bản mã nguồn trang web dựa trên hình ảnh phác thảo hoặc mô tả yêu cầu bằng văn bản, ứng dụng mô hình Claude AI và triển khai trên Cloudflare Workers. (Đóng góp từ [@mggger](https://github.com/ruanyf/weekly/issues/6371))

2、[AigcPanel](https://github.com/modstart-lib/aigcpanel)

Dự án phần mềm mã nguồn mở cung cấp giải pháp tự động tạo hình ảnh và cử động cho người số AI (Digital Human Generator). (Đóng góp từ [@modstart](https://github.com/ruanyf/weekly/issues/6407))

3、[EmojiMyFace](https://emojimyface.com/)

Dịch vụ trực tuyến miễn phí ứng dụng AI hỗ trợ nhận diện gương mặt trên ảnh chụp và thay thế tự động bằng các biểu tượng cảm xúc Emoji để bảo mật thông tin cá nhân. (Đóng góp từ [@Takea-nap](https://github.com/ruanyf/weekly/issues/6410))

4、[aisubtranslate.top](https://aisubtranslate.top/)

Dịch vụ trực tuyến miễn phí hỗ trợ dịch thuật tự động các tệp tin phụ đề phim (srt, vtt...) thông qua kết nối các mô hình AI lớn. (Đóng góp từ [@LetheTK](https://github.com/ruanyf/weekly/issues/6397))

## 资源

1、[Hệ thống kiểm tra tốc độ phản hồi của máy chủ DNS](https://dnsspeedtest.online/)

Trang web hỗ trợ đo đạc thời gian phản hồi (latency) từ máy tính của bạn đến các hệ thống máy chủ phân giải DNS công cộng lớn trên toàn cầu.

Công cụ đo đạc DNS tương tự hoạt động qua dòng lệnh terminal là **dnspy**. (Đóng góp từ [@xxnuo](https://github.com/ruanyf/weekly/issues/6368))

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032613.webp)

2、[Orbit](https://www.bbc.co.uk/orbitmusic)

Dịch vụ web của đài BBC cung cấp trải nghiệm tìm kiếm và khám phá các ca khúc âm nhạc mới thông qua giao diện trực quan hóa sinh động.

3、[Top Hacker News](https://www.tophn.co/)

Chuyên trang tổng hợp thông tin: Tự động cập nhật các bài viết nóng hổi nhất trên diễn đàn Hacker News theo thời gian thực đi kèm hình ảnh đại diện và bản tóm tắt nội dung súc tích. (Đóng góp từ [@heyppen](https://github.com/ruanyf/weekly/issues/6384))

4、[MusicMint](https://www.musicmint.ai/)

Trang web giới thiệu và chia sẻ các tác phẩm âm nhạc được sáng tác hoàn toàn bởi trí tuệ nhân tạo. (Đóng góp từ [@250465043](https://github.com/ruanyf/weekly/issues/6361))

5、[Travel Plug Advisor (Tra cứu chuẩn phích cắm điện du lịch)](https://remit.ee/tools/check-plug-travel-adapter/)

Dịch vụ web hữu ích hỗ trợ tra cứu nhanh các chủng loại phích cắm điện và thông số điện áp tiêu chuẩn của các quốc gia trên thế giới giúp chuẩn bị tốt cho các chuyến du lịch. (Đóng góp từ [@imowen](https://github.com/ruanyf/weekly/issues/6351))

## 图片

1、[So sánh tương quan kích thước giữa Trái Đất và Mặt Trời](https://www.facebook.com/permalink.php?story_fbid=pfbid0xD8yB6UiCKtNhvyfM6w8ARCRXzxukjMgfYcShuAcNAthBbBToy9j3LC3vDExaz1yl&id=100064747956101)

Kích thước của Mặt Trời là vô cùng khổng lồ so với Trái Đất nhỏ bé của chúng ta. Đường kính của Mặt Trời lớn gấp 109 lần đường kính Trái Đất, và thể tích của nó lớn gấp khoảng 1,3 triệu lần thể tích Trái Đất.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032603.webp)

Quan sát hình ảnh mô phỏng phía trên, đốm tròn màu xanh lam nhỏ bé ở góc dưới cùng bên trái chính là hình ảnh đại diện cho Trái Đất.

Do đó, chỉ cần khai thác được một phần vô cùng nhỏ năng lượng bức xạ mặt trời tỏa ra đã hoàn toàn đủ đáp ứng nhu cầu tiêu thụ năng lượng của toàn bộ nhân loại trên Trái Đất.

2、[Tính năng tự động tạo meme bằng mô hình DALL-E 3](https://www.facebook.com/Coyoter.Huang/posts/pfbid0gq7MrwSf7R1nM4ETzDoS2o8a4w4neu65We7fZBhEGgM9xr1W1fwX6U9qgrNcd9TJl)

Tuần trước, OpenAI đã chính thức mở rộng tính năng [tự động sinh hình ảnh trực tiếp](https://openai.com/index/introducing-4o-image-generation/) cho mô hình GPT-4o. Người dùng phát hiện ra khi tải lên một bức ảnh bất kỳ, hệ thống có khả năng tự động tạo ra các bức ảnh meme vô cùng hài hước và khớp biểu cảm.

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032712.webp)

Câu lệnh gợi ý được sử dụng: "Hãy vẽ lại nhân vật trong bức ảnh theo phong cách nhân vật chibi dễ thương, và thiết kế thành một bộ sưu tập biểu cảm gồm 12 tư thế chuyển động đi kèm các đoạn chữ tương ứng".

![](https://cdn.beekka.com/blogimg/asset/202503/bg2025032713.webp)

## 文摘

1、[Tại sao chúng ta nên tiếp tục hành động tự chế tác lại những thứ đã có (Reinventing the Wheel)?](https://tobloef.com/blog/wheel-reinventors-principles/)

Tôi là người đặc biệt thích tự lập trình xây dựng mọi thứ từ con số không, và thường xuyên nhận được những lời khuyên từ mọi người xung quanh rằng tôi đang lãng phí thời gian để "chế tạo lại chiếc bánh xe" vốn đã có sẵn trên thị trường.

Dưới đây là một số lý do thúc đẩy tôi tiếp tục duy trì thói quen này:

(1) **Mục tiêu học tập**: Thông qua quy trình tự chế tác lại từ đầu, tôi học hỏi được vô số kiến thức hệ thống quý giá, thấu hiểu sâu sắc cơ chế hoạt động thực tế của công nghệ và làm chủ quy trình phát triển sản phẩm.

(2) **Khả năng tùy biến sâu**: Không có một giải pháp chung nào có thể đáp ứng hoàn hảo cho mọi kịch bản thực tế. Việc tự xây dựng công cụ cho phép tôi tự do cấu hình và tối ưu hóa sâu tính năng tương thích tốt nhất với nhu cầu cá nhân.

(3) **Cơ hội đổi mới sáng tạo**: Nhiều công cụ có sẵn trên thị trường thực chất có chất lượng rất tệ. Quy trình tự thiết kế lại chính là cơ hội tốt để tôi thử nghiệm và áp dụng các ý tưởng thiết kế sáng tạo mới.

(4) **Niềm vui cá nhân**: Ngay cả khi bỏ qua cả 3 lý do thực tế kể trên, tôi vẫn tiếp tục tự chế tác đơn giản vì tôi vô cùng yêu thích cảm giác tự tay làm ra sản phẩm. Cảm giác nhìn thấy một hệ thống do chính mình viết ra hoạt động hoàn hảo mang lại niềm hạnh phúc cực kỳ lớn.

Tuy nhiên, tôi hoàn toàn không khuyến nghị tất cả mọi người đều nên học theo giải pháp này. Quy trình tự chế tác lại từ đầu cũng đi kèm nhiều nhược điểm lớn không thể ngó lơ:

(5) Quy trình tự phát triển đòi hỏi sự đầu tư một lượng quỹ thời gian cực kỳ lớn.

(6) Sản phẩm cuối cùng do bạn tự làm ra có thể cho hiệu năng và độ ổn định kém xa so với các giải pháp chuyên nghiệp sẵn có trên thị trường.

(7) Bạn rất dễ bị rơi vào chuỗi lặp vô tận: Để chế tạo được chiếc bánh xe, trước tiên bạn lại phải mất công đi chế tạo ra chiếc búa và cái đục...

Do đó, nếu bạn có kế hoạch tự chế tác lại một công cụ nào đó, hãy cân nhắc kỹ hai câu hỏi: Thứ nhất, bạn có thực sự dư dả quỹ thời gian hay không (đặc biệt khi dự án có sự tham gia của các thành viên khác). Thứ hai, hãy xác định rõ giới hạn phân vùng của những thứ bạn sẽ tự chế tác để tránh bị sa đà đi quá xa khỏi mục tiêu cốt lõi ban đầu của dự án.

## 言论

1、

Một lập trình viên xuất sắc thường trải qua tiến trình phát triển sự nghiệp gồm 3 giai đoạn: Khởi đầu ở vai trò người thực thi (Implementer - viết code theo thiết kế sẵn), sau đó nâng cấp lên người giải quyết vấn đề (Solver - tự tìm giải pháp kỹ thuật) và cuối cùng đạt tới cấp độ người định vị (Finder - phát hiện ra các bài toán cốt lõi cần giải quyết).

-- *Trích bài viết 《Người thực thi, Người giải quyết và Người định vị》*

2、

Nếu bạn đang nỗ lực phát triển một ứng dụng phần mềm với định hướng duy trì hoạt động dài hạn, việc tranh luận xem nên lựa chọn framework frontend nào thực chất là quyết định kỹ thuật ít quan trọng nhất. Thời gian bạn dành ra để tranh cãi xem React hay Vue tốt hơn chỉ đơn thuần là sự lãng phí năng lượng vô ích.

Bởi lẽ dù bạn đưa ra quyết định chọn lựa thế nào, chỉ sau 5 năm nữa, bộ khung đó chắc chắn cũng sẽ lỗi thời, hoặc ngay cả khi nó vẫn tồn tại thì cú pháp và triết lý vận hành của nó lúc đó cũng đã thay đổi hoàn toàn so với phiên bản hiện tại. Đó chính là cơ chế vận hành của thế giới frontend.

-- *Trích bài viết 《Vòng chạy vô tận của thế giới Frontend》*

3、

Việc phát triển một ứng dụng Web trong năm 2025 có nhiều nét tương đồng với việc bạn đi mua và tự lắp ráp đồ nội thất của hãng IKEA. Công việc của bạn phần lớn là tìm cách chắp vá và cấu hình một loạt các dịch vụ độc lập lại với nhau: từ frontend, backend, CDN, chứng chỉ bảo mật HTTPS, cơ sở dữ liệu, dịch vụ xác thực người dùng, cổng thanh toán...

Nhiệm vụ cốt lõi của kỹ sư phần mềm lúc này không còn là viết các thuật toán code thuần túy, mà chuyển dịch sang vai trò cấu hình hệ thống, thiết lập đường ống dẫn dữ liệu, điều phối quy trình và áp dụng các tiêu chuẩn vận hành tối ưu.

-- *Andrej Karpathy, nhà khoa học AI nổi tiếng chia sẻ*

4、

Sự giận dữ là một trạng thái cảm xúc mang tính tàn phá mạnh mẽ, kích thích mong muốn trả đũa đối phương nhưng thực chất lại gây tổn hại lớn nhất đến lợi ích cốt lõi của chính bản thân bạn. Giải pháp ứng xử lý trí nhất là hãy cố gắng kiềm chế mong muốn trả đũa ban đầu, bình tĩnh suy ngẫm xem giữa bạn và đối phương có tồn tại lợi ích chung nào hay không để từ đó tìm kiếm cơ hội hợp tác và đạt được sự thấu hiểu lẫn nhau.

-- *Trích bài viết 《Vượt lên trên sự giận dữ》*

5、

Mọi tổ chức tôn giáo trong lịch sử tiến hành trục xuất các tín đồ dị giáo hoàn toàn không phải vì họ lo sợ lập luận của người đó là sai lầm, mà bởi họ lo sợ rằng lập luận đó rất có thể lại là chân lý chính xác.

-- *Edsger W. Dijkstra, nhà khoa học máy tính lỗi lạc chia sẻ*

## 往年回顾

- Số #296: [Tìm hiểu về chân dung của nhà phát triển Jia Tan phía sau sự cố cài cắm cửa sau (Backdoor) xz](http://www.ruanyifeng.com/blog/2024/04/weekly-issue-296.html)
- Số #246: [Thảo luận về giải pháp xây dựng một định danh trực tuyến vĩnh viễn không bao giờ bị thất lạc](http://www.ruanyifeng.com/blog/2023/03/weekly-issue-246.html)
- Số #196: [Phân tích về xu hướng phát triển của các dòng máy chơi game cầm tay (Handheld Consoles) trong tương lai](http://www.ruanyifeng.com/blog/2022/02/weekly-issue-196.html)
- Số #146: [Thảo luận các giải pháp nâng cao hiệu quả chất lượng của hoạt động dạy và học trực tuyến](http://www.ruanyifeng.com/blog/2021/02/weekly-issue-146.html)

(Hết)
