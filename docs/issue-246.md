# Bản tin chia sẻ công nghệ (Số 246): Danh tính mạng không bao giờ bị thất lạc

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2960) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031406.webp)

Do cuộc bãi công kéo dài của công nhân vệ sinh, đường phố Paris tuần này ngập tràn những đống túi rác thải xếp chồng chất lên nhau, người đi bộ buộc phải len lỏi di chuyển qua chúng. Nếu không có người dọn rác, một đô thị hiện đại có thể duy trì được cuộc sống bình thường trong bao nhiêu ngày? (Nguồn: [CNN](https://edition.cnn.com/2023/03/11/europe/paris-trash-strikes-intl/index.html))

## 本周话题：永不丢失的网络身份

1、

Trong các tác phẩm điện ảnh và truyền hình, chúng ta thường thấy những tình tiết quen thuộc: Một nhân vật tỉnh dậy sau cơn hôn mê dài, hoàn toàn bị mất trí nhớ và không thể nhớ ra "tôi là ai".

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031505.webp)

Anh ta không biết tên tuổi, địa chỉ nhà, không mang theo giấy tờ tùy thân hay vật chứng nào, cũng không có người quen nhận dạng.

Cứ như vậy, **anh ta bỗng chốc trở thành một người không có danh tính, mất đi mọi thứ từng thuộc về mình.**

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031506.webp)

Tuy nhiên ngoài đời thực ngày nay, những tình tiết như thế này rất hiếm khi xảy ra. Lý do là chúng ta đã có các cơ sở dữ liệu DNA toàn cầu, chỉ cần xét nghiệm DNA là có thể xác định được ngay bạn là ai. Ngay cả khi không tìm thấy thông tin chính xác của bạn, hệ thống vẫn có thể tìm ra những người thân có huyết thống gần nhất.

Câu hỏi "tôi là ai" về mặt sinh học cơ bản đã được giải quyết triệt để. Bạn luôn là chính bạn và danh tính xã hội của bạn sẽ không bao giờ bị thất lạc nữa.

2、

Tuy nhiên, bên cạnh danh tính xã hội ngoài đời thực, con người hiện đại ngày nay còn sở hữu thêm một loại danh tính thứ hai: **Danh tính mạng (Internet Identity).** Việc thất lạc hoặc mất quyền kiểm soát danh tính mạng mới chính là vấn đề thực tế và đau đầu hơn rất nhiều.

**Danh tính mạng thực chất chính là các tài khoản internet của bạn.** Nếu mất tài khoản, bạn sẽ mất đi toàn bộ tài sản số, danh sách liên lạc, lịch sử hoạt động đi kèm và gần như biến mất khỏi thế giới internet.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031507.webp)

Trong tương lai, các bộ phim truyền hình có lẽ sẽ đổi kịch bản thành thế này: Nhân vật tỉnh dậy sau tai nạn, mất trí nhớ và **hoàn toàn không thể nhớ ra tên đăng nhập cùng mật khẩu tài khoản mạng của mình.**

Không có danh tính mạng, toàn bộ cuộc sống kỹ thuật số của anh ta sẽ bị đóng băng và xóa sổ hoàn toàn.

3、

Nguy cơ mất danh tính mạng thực tế lớn hơn nhiều so với những gì chúng ta tưởng tượng.

Có một thực tế mà ít người nhận ra: **Tài khoản mạng của bạn không thực sự thuộc sở hữu của bạn.** Chúng không chỉ dễ dàng bị quên lãng hay đánh cắp, mà hoàn toàn có thể bị các nhà cung cấp dịch vụ tước đoạt một cách hợp pháp.

Các dịch vụ internet hiện nay hầu hết đều yêu cầu người dùng đăng ký tài khoản bằng số điện thoại di động hoặc địa chỉ email. Cả hai thông tin này đều không thực sự thuộc về bạn.

Số điện thoại thuộc quyền quản lý của nhà mạng viễn thông, địa chỉ email thuộc về nhà cung cấp dịch vụ thư điện tử và nhà đăng ký tên miền. Nếu các đơn vị này quyết định thu hồi số điện thoại hoặc tên miền email của bạn, danh tính mạng liên kết với chúng cũng sẽ gặp rủi ro bị mất quyền kiểm soát vĩnh viễn nếu không kịp thay đổi thông tin.

4、

Không chỉ thông tin đăng ký không thuộc về bạn, mà ngay cả quyền sở hữu pháp lý của chính tài khoản đó cũng không thuộc sở hữu của người dùng.

Ví dụ, tài khoản WeChat của bạn thực chất [thuộc quyền sở hữu của công ty Tencent](https://tech.sina.com.cn/roll/2020-09-08/doc-iivhuipp3172175.shtml). Trong Điều khoản dịch vụ của WeChat tại mục 7.1.2 đã ghi rõ:

> “Quyền sở hữu tài khoản WeChat thuộc về Tencent. Sau khi hoàn tất thủ tục đăng ký, người dùng chỉ được cấp quyền sử dụng tài khoản đó.”

Hầu hết tất cả các tài khoản dịch vụ mạng xã hội hiện nay đều hoạt động theo nguyên tắc này, người dùng chỉ thuê quyền sử dụng.

Do đó, **nhà cung cấp dịch vụ hoàn toàn có quyền đơn phương tạm khóa hoặc xóa sổ tài khoản của bạn bất cứ lúc nào một cách hoàn toàn hợp pháp.** Vụ việc cựu Tổng thống Mỹ Donald Trump bị Twitter khóa tài khoản vĩnh viễn chính là minh chứng điển hình cho điều này.

5、

Nếu chúng ta không thực sự làm chủ danh tính mạng của mình, điều đó đồng nghĩa với việc chúng ta không thực sự sở hữu bất kỳ tài sản số nào gắn liền với danh tính đó trên không gian mạng.

Vậy **liệu có giải pháp nào giúp danh tính mạng thực sự thuộc sở hữu tuyệt đối của người dùng, do người dùng toàn quyền kiểm soát, không ai có thể tước đoạt và không bao giờ bị thất lạc hay không?**

Câu trả lời là có, và công nghệ này đã được hiện thực hóa.

Giải pháp là sử dụng một cặp khóa mật mã (keypair) để đại diện cho danh tính mạng của bạn: Khóa công khai (public key) sẽ đóng vai trò là ID người dùng để định danh, còn khóa bí mật (private key) được giữ kín dùng để ký xác thực danh tính khi đăng nhập.

Cơ chế này bảo đảm danh tính của mỗi người dùng là độc nhất vô nhị trên thế giới. Miễn là bạn giữ an toàn cho khóa bí mật của mình, không một ai hay tổ chức nào có thể tước đoạt hoặc can thiệp vào tài khoản của bạn.

Thực tế, toàn bộ hệ thống định danh của thế giới tiền mã hóa (crypto) đang vận hành dựa trên cơ chế này. Tài khoản của người dùng chính là địa chỉ ví (khóa công khai), và chỉ có người giữ khóa bí mật tương ứng mới có quyền thực hiện các giao dịch trên ví đó.

Gần đây, một giao thức mạng xã hội phi tập trung mới ra đời mang tên [Nostr](https://nostr.com/) cũng áp dụng nguyên lý này:

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031601.webp)

Bạn có thể viết bài chia sẻ và kết nối với người dùng khác tương tự như Twitter. Điểm khác biệt cốt lõi là tài khoản của mỗi người chính là khóa công khai của họ, dữ liệu được truyền qua các máy chủ relay độc lập, do đó không một thực thể nào có thể khóa hay xóa tài khoản của bạn.

6、

Nếu tất cả mọi người đều sử dụng khóa công khai làm định danh tài khoản, chúng ta có thể ghi nhận toàn bộ các khóa công khai này lên một chuỗi blockchain công khai. Sau này, khi muốn tìm kiếm hay xác thực danh tính mạng của một ai đó, hệ thống chỉ cần truy vấn dữ liệu từ blockchain.

Đây là một trong những ứng dụng thực tế và hữu ích nhất của công nghệ blockchain mà tôi có thể nghĩ ra. Trở ngại duy nhất là việc đọc dữ liệu từ blockchain là hoàn toàn miễn phí, nhưng việc ghi thông tin mới lên chuỗi sẽ yêu cầu người dùng trả một khoản phí giao dịch nhỏ (gas fee).

Chúng ta có thể coi khoản phí ghi dữ liệu này giống như phí đăng ký danh tính mạng một lần duy nhất. Sau khi hoàn tất đăng ký, danh tính này sẽ tồn tại vĩnh viễn trên mạng internet, bất kỳ ai cũng có thể tra cứu và không một thế lực nào có thể giả mạo hay xóa bỏ nó.

7、

Đến đây, những độc giả tinh ý chắc chắn sẽ đặt câu hỏi: Cách làm này vẫn chưa giải quyết được tình huống mất trí nhớ được đề cập ở đầu bài viết.

Nếu bạn bị mất trí nhớ và quên mất khóa bí mật của mình, danh tính mạng của bạn chẳng phải cũng sẽ bị thất lạc vĩnh viễn hay sao?

Thực tế, bài toán hóc búa này cũng đã có người đưa ra giải pháp, đó chính là Sam Altman – CEO đương nhiệm của OpenAI:

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031602.webp)

Vào năm 2020, ông đã đồng sáng lập dự án [Worldcoin](https://worldcoin.org/) để giải quyết triệt để bài toán định danh này.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031603.webp)

Trọng tâm của dự án là dịch vụ [World ID](https://techcrunch.com/2023/03/07/worldcoin-cofounded-by-sam-altman-is-betting-the-next-big-thing-in-ai-is-proving-you-are-human/) nhằm cấp phát một danh tính số toàn cầu duy nhất cho mỗi con người.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031604.webp)

Quy trình thực hiện là sử dụng một thiết bị chuyên dụng quét võng mạc (iris) của người dùng, mã hóa thông tin sinh trắc học này thành một mã định danh duy nhất lưu trên blockchain, đồng thời tạo ra một cặp khóa mật mã làm World ID.

Bằng cách này, ngay cả khi bạn bị mất trí nhớ hay thất lạc khóa bí mật, bạn chỉ cần thực hiện quét lại võng mạc của mình để hệ thống đối chiếu dữ liệu sinh trắc học và cấp lại quyền truy cập vào danh tính mạng tương ứng.

Dự án World ID vừa mới chính thức [công bố bộ công cụ phát triển phần mềm SDK](https://worldcoin.org/blog/announcements/introducing-world-id-and-sdk) để tích hợp vào các dịch vụ bên thứ ba. Nếu bạn không ngại việc chia sẻ dữ liệu quét võng mạc để đổi lấy một danh tính số vĩnh viễn, bạn có thể tìm hiểu thêm về dự án này. Tôi hy vọng mô hình ứng dụng cặp khóa bảo mật làm danh tính mạng sẽ ngày càng được phổ biến rộng rãi.

## Tin tức công nghệ

1、[Ý tưởng thiết lập hệ thống định vị và múi giờ riêng cho Mặt Trăng](https://www.esa.int/Applications/Navigation/Telling_time_on_the_Moon)

Trong vòng một thập kỷ tới, thế giới sẽ chứng kiến rất nhiều dự án thám hiểm Mặt Trăng được triển khai đồng thời. Các thiết bị tự hành hoạt động trên Mặt Trăng cần thiết lập kết nối viễn thông trực tiếp với nhau để phối hợp hoạt động.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031201.webp)

Hiện tại, toàn bộ các thiết bị hoạt động trên Mặt Trăng vẫn đang đồng bộ thời gian theo giờ Trái Đất. Cơ quan Vũ trụ Châu Âu (ESA) đang thảo luận phương án xây dựng một múi giờ Mặt Trăng độc lập cùng hệ thống định vị vệ tinh chuyên dụng.

Hệ thống này sẽ hoạt động giống như một mạng lưới GPS dành riêng cho Mặt Trăng, giúp các thiết bị tự xác định tọa độ và thời gian thực hiện lộ trình di chuyển mà không cần phụ thuộc vào việc chuyển tiếp tín hiệu từ Trái Đất. Trở ngại kỹ thuật lớn nhất là chu kỳ tự quay và quay quanh Trái Đất của Mặt Trăng kéo dài khoảng 28 ngày, khiến việc quy đổi đồng bộ thời gian gặp nhiều phức tạp.

2、[Biện pháp chống quay cóp thi cử độc đáo tại Philippines](https://www.bbc.com/news/world-asia-63363473)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102411.webp)

Tại một trường đại học ở Philippines, do tình trạng sinh viên quay cóp bài thi diễn ra khá phổ biến, một giảng viên đã đưa ra nội quy thi cử đặc biệt: Yêu cầu tất cả sinh viên phải tự thiết kế và đội những chiếc mũ có phần che kín tầm nhìn hai bên thái dương khi làm bài.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102412.webp)

Sinh viên của trường đã thỏa sức sáng tạo tự tay làm ra đủ loại mũ độc lạ từ các vật liệu tái chế như bìa carton, khay trứng hay mặt nạ hoạt hình. Những bức ảnh chụp phòng thi ngộ nghĩnh này đã nhanh chóng lan truyền trên mạng xã hội thu hút hàng ngàn lượt tương tác. Giảng viên cho biết biện pháp này mang lại hiệu quả rất tốt và không phát hiện trường hợp gian lận nào trong suốt kỳ thi.

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102413.webp)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022102414.webp)

3、[Tự chế màng lọc không khí tích hợp trên quạt trần](https://www.jefftk.com/p/ceiling-air-purifier)

Một lập trình viên đã chia sẻ dự án tự chế bộ lọc không khí cỡ lớn tận dụng hệ thống quạt trần có sẵn trong phòng khách:

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060512.jpg)

Cách thực hiện khá đơn giản: anh đã mua các tấm màng lọc HEPA tiêu chuẩn và ghép chúng thành một vòng tròn bao quanh quạt trần.

![](https://cdn.beekka.com/blogimg/asset/202206/bg2022060513.jpg)

Ưu điểm của thiết bị tự chế này là sải cánh quạt trần rộng giúp tạo ra luồng gió lưu thông lớn nhưng chạy cực kỳ êm ái không gây ồn như các máy lọc không khí thông thường. Kết quả đo đạc cho thấy thiết bị giúp làm giảm đáng kể chỉ số bụi mịn PM2.5 trong phòng khách.

4、[Thử nghiệm thành công máy sản xuất oxy MOXIE trên Hỏa tinh](https://phys.org/news/2022-08-moxie-reliably-oxygen-mars.html)

Vào tháng 2 năm 2021, xe tự hành Perseverance của NASA đã đáp xuống bề mặt Hỏa tinh mang theo một thiết bị thí nghiệm nhỏ mang tên MOXIE nhằm thử nghiệm khả năng tự sản xuất dưỡng khí trên hành tinh đỏ:

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090114.webp)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090115.webp)

Theo báo cáo tổng kết mới nhất, thiết bị MOXIE đã vận hành thành công 7 lần trong các điều kiện môi trường khí quyển khác nhau, đạt công suất sản xuất trung bình 6 gram oxy/giờ, đủ đáp ứng nhu cầu hô hấp của một phi hành gia trong vòng 10 phút.

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022090116.webp)

Bầu khí quyển Hỏa tinh chứa tới 96% khí carbon dioxide (CO2). Thiết bị MOXIE đã sử dụng phương pháp điện phân ở nhiệt độ cao để phân tách các phân tử CO2 thành khí oxy (O2) và khí carbon monoxide (CO) thải ra ngoài. Thành công bước đầu này là tiền đề để NASA phát triển các hệ thống sản xuất oxy quy mô lớn phục vụ các sứ mệnh đưa con người đổ bộ Hỏa tinh trong tương lai.

## Bài viết

1\. [Hướng dẫn chạy mô hình ngôn ngữ lớn LLaMA trực tiếp trên máy tính cá nhân](https://til.simonwillison.net/llms/llama-7b-m2)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031407.webp)

LLaMA là mô hình AI mã nguồn mở được Meta công bố với hiệu năng được đánh giá vượt trội hơn so với GPT-3. Bài viết hướng dẫn chi tiết cách thức cấu hình để chạy trực tiếp mô hình LLaMA-7B trên CPU của dòng máy Mac sử dụng chip M1/M2 mà không cần đến card đồ họa GPU rời đắt đỏ.

2\. [Tìm hiểu thuộc tính CSS `initial-letter` hỗ trợ tạo chữ cái đầu dòng thả xuống](https://developer.chrome.com/blog/control-your-drop-caps-with-css-initial-letter/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011905.webp)

Đặc tả CSS mới bổ sung thuộc tính `initial-letter` giúp các lập trình viên dễ dàng định dạng kích thước và số dòng thụt lề cho ký tự đầu tiên của bài viết (drop cap) trực tiếp bằng mã CSS thay vì phải viết các thẻ span phức tạp.

3\. [WordPress đã được ra đời như thế nào?](https://levelup.gitconnected.com/meet-a-programmer-who-turned-an-open-source-platform-into-a-7-500-000-000-company-645e14c53c8)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011502.webp)

Bài viết kể về chặng đường phát triển từ năm 2003 của lập trình viên Matt Mullenweg – người đã xây dựng dự án mã nguồn mở WordPress từ khi mới 19 tuổi và phát triển nó thành một nền tảng CMS chiếm hơn 40% thị phần website toàn cầu.

4\. [Nhìn lại hành trình khởi nghiệp xây dựng nền tảng Replit](https://www.the5to9.xyz/p/replit-800m-side-project)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011603.webp)

Replit là một IDE trực tuyến chạy trực tiếp trên trình duyệt vô cùng phổ biến hiện nay. Bài viết phỏng vấn nhà sáng lập người Jordan kể về hành trình từ một dự án cá nhân nhỏ ban đầu phát triển thành một công ty công nghệ có giá trị định giá lên tới 800 triệu USD.

5\. [Hướng dẫn tự lắp đặt hệ thống lưu trữ NAS bằng bo mạch Orange Pi](https://www.instructables.com/DIY-Raspberry-Orange-Pi-NAS-That-Really-Looks-Like/)（Tiếng Anh）

Tác giả chia sẻ toàn bộ quy trình tự thiết kế phần cứng vỏ hộp bằng máy in 3D kết hợp sử dụng bo mạch máy tính nhúng Orange Pi để tự dựng một hệ thống lưu trữ mạng NAS gia đình chạy hệ điều hành nguồn mở.

![](https://cdn.beekka.com/blogimg/asset/202301/bg2023011601.webp)

6\. [Lịch sử phát triển các công cụ kết xuất đồ họa trình duyệt web](https://eylenburg.github.io/browser_engines.htm)（Tiếng Anh）

Bài viết tổng hợp và sơ đồ hóa chặng đường lịch sử phát triển của toàn bộ các bộ nhân kết xuất trình duyệt (browser engines) từ thời kỳ đầu sơ khai (như Mosaic, Netscape) cho tới các bộ nhân hiện đại (như Blink, WebKit, Gecko).

## AI 相关软件

Ngày càng có nhiều công cụ phần mềm tích hợp các tính năng trí tuệ nhân tạo bằng cách gọi trực tiếp API của OpenAI. Dưới đây là các dự án nguồn mở chất lượng do cộng đồng lập trình viên đóng góp:

1. [PromptPerfect](https://promptperfect.jina.ai/): Tiện ích hỗ trợ tự động tối ưu hóa cấu trúc câu lệnh prompt đầu vào giúp các mô hình AI sinh văn bản và hình ảnh chính xác hơn. (Đóng góp của [@hanxiao](https://github.com/ruanyf/weekly/issues/2974))
2. [Chatbox](https://github.com/Bin-Huang/chatbox): Ứng dụng khách (Client) đa nền tảng kết nối API OpenAI cài đặt trên máy tính, hỗ trợ quản lý và lưu trữ lịch sử trò chuyện prompt chuyên nghiệp. (Đóng góp của [@Bin-Huang](https://github.com/ruanyf/weekly/issues/2978))
3. [Chaty](https://github.com/cosin2077/chaty): Tiện ích dòng lệnh CLI hỗ trợ người dùng tương tác trực tiếp với ChatGPT nhanh chóng thông qua cửa sổ terminal. (Đóng góp của [@cosin2077](https://github.com/ruanyf/weekly/issues/2979))
4. [PowerGPT](https://github.com/ouromoros/PowerGPT): Module mở rộng dành cho Windows PowerShell giúp tự động chuyển dịch mô tả yêu cầu bằng ngôn ngữ tự nhiên thành các câu lệnh shell tương ứng. (Đóng góp của [@ouromoros](https://github.com/ruanyf/weekly/issues/2980))
5. [Writely](https://github.com/anc95/writely): Extension dành cho trình duyệt Chrome cung cấp trợ lý viết lách AI tích hợp trực tiếp trên mọi ô nhập liệu văn bản tương tự Notion AI. (Đóng góp của [@anc95](https://github.com/ruanyf/weekly/issues/2981))
6. [智能文案小助手](https://github.com/CatsAndMice/lanlan): Dự án mã nguồn mở xây dựng giao diện web nhập form mẫu hỗ trợ AI tự động tạo các bài viết quảng cáo, giới thiệu sản phẩm. (Đóng góp của [@CatsAndMice](https://github.com/ruanyf/weekly/issues/2984))

## Công cụ

1、[Jami: Ứng dụng nhắn tin và gọi điện nhóm phi tập trung nguồn mở](https://jami.net/)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122201.webp)

Một phần mềm cộng tác và đàm thoại nhóm mã nguồn mở bảo mật cao, hỗ trợ gửi tin nhắn, gọi điện video chất lượng cao và chia sẻ màn hình hoạt động dựa trên mạng ngang hàng (P2P).

2、[PhpWebStudy: Công cụ quản trị môi trường phát triển PHP và Web trên macOS](https://www.macphpstudy.com/)

Ứng dụng giao diện đồ họa hữu ích dành cho macOS giúp quản trị, cấu hình và khởi động nhanh các dịch vụ phát triển web thông dụng như Nginx, Apache, PHP, MySQL, Redis. (Đóng góp của [@xpf0000](https://github.com/ruanyf/weekly/issues/2973))

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031401.webp)

3、[Huntly: Công cụ tự lưu trữ quản lý thông tin đọc tin qua RSS](https://github.com/lcomplete/huntly)

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031405.webp)

Ứng dụng web tự lưu trữ hỗ trợ lưu trữ toàn bộ nội dung các trang web người dùng đã truy cập qua trình duyệt, tích hợp tính năng đọc tin tức qua kênh RSS và hỗ trợ tìm kiếm toàn văn. (Đóng góp của [@lcomplete](https://github.com/ruanyf/weekly/issues/2977))

4、[CircuitJS1: Trình giả lập mạch điện tử tương tác chạy trên trình duyệt](https://github.com/pfalstad/circuitjs1)

Một ứng dụng vẽ và mô phỏng hoạt động của các mạch điện tử trực tuyến chạy trên trình duyệt, cho phép người dùng tự lắp ráp linh kiện và theo dõi biểu đồ dòng điện thời gian thực. (Đóng góp của [@jerrylususu](https://github.com/ruanyf/weekly/issues/2975))

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031403.webp)

5、[RxEditor: Trình thiết kế giao diện low-code kéo thả sinh mã React](https://github.com/rxdrag/rxeditor)

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031404.webp)

Dự án mã nguồn mở xây dựng công cụ thiết kế giao diện web low-code trực quan, hỗ trợ lập trình viên kéo thả các component để sinh nhanh mã nguồn Front-end React. (Đóng góp của [@rxdrag](https://github.com/ruanyf/weekly/issues/2976))

6、[Zarm: Bộ thư viện component UI di động dành cho React](https://zarm.design/)

Bộ thư viện mã nguồn cung cấp các thành phần giao diện di động (Mobile UI components) được thiết kế đồng bộ, hiện đại chạy trên nền tảng React. (Đóng góp của [@dominicleo](https://github.com/ruanyf/weekly/issues/2982))

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031411.webp)

## 资源

1、[useragents.me: Trang web cập nhật chuỗi User Agent của các trình duyệt](https://www.useragents.me/)

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022121803.webp)

Dịch vụ web hữu ích chuyên cung cấp các chuỗi User Agent (UA) mới nhất của các dòng trình duyệt phổ biến trên thế giới phục vụ công tác kiểm thử phần mềm hoặc viết crawler.

2、[webЯcade: Trình giả lập chơi game console cổ điển trên trình duyệt](https://www.webrcade.com/)

![](https://cdn.beekka.com/blogimg/asset/202209/bg2022092604.webp)

Dự án mã nguồn mở xây dựng nền tảng giả lập chơi các hệ máy game cổ điển (như NES, Genesis) trực tiếp trên giao diện trình duyệt web, hỗ trợ người dùng tự tải tệp ROM cá nhân lên để chơi game.

3、[Comprehensive Rust: Khóa học lập trình Rust chuyên sâu của Google](https://google.github.io/comprehensive-rust/)

Bộ giáo trình đào tạo lập trình ngôn ngữ Rust trong vòng 4 ngày do đội ngũ kỹ sư Android của Google biên soạn, hướng dẫn từ cú pháp cơ bản cho đến các chủ đề nâng cao về tương thích hệ thống.

![](https://cdn.beekka.com/blogimg/asset/202212/bg2022122211.webp)

4、[A Gentle Introduction to Assembly Language Programming: Giáo trình hợp ngữ kiến trúc ARM 64](https://github.com/pkivolowitz/asm_book)

Cuốn sách điện tử nguồn mở viết bằng tiếng Anh giới thiệu các khái niệm lập trình hợp ngữ (Assembly) trên nền tảng kiến trúc vi xử lý ARM 64 dành cho những lập trình viên đã có kiến thức cơ bản về C/C++.

## 图片

1、**Lịch sử về FogCam - Chiếc webcam truyền hình ảnh trực tiếp lâu đời nhất thế giới**

Chiếc webcam đầu tiên trên thế giới ra đời gắn liền với mục đích phục vụ nhu cầu thực tế đời sống của các kỹ sư.

Vào năm 1994, một nghiên cứu sinh tại Đại học Bang San Francisco đã cho lắp đặt một chiếc camera ghi hình hướng ra sân trường để truyền hình ảnh trực tiếp lên trang web nội bộ:

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100402.webp)

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100403.webp)

Ý tưởng ban đầu của anh chỉ đơn giản là để mọi người trong phòng nghiên cứu có thể xem nhanh qua mạng xem bình cà phê đặt ở sảnh hành lang còn đầy hay đã cạn để biết đường mang theo cà phê cá nhân.

Về sau, camera này chuyển sang phát sóng trực tiếp phong cảnh khuôn viên trường học. Trải qua hơn 20 năm phát sóng liên tục, vào năm 2019, người quản lý tuyên bố sẽ ngừng hoạt động chiếc camera này do thiết bị cũ kỹ. Trước sự quan tâm của truyền thông và cựu sinh viên, nhà trường đã quyết định tiếp quản thiết bị này để tiếp tục phát sóng. Bạn đọc có thể xem trực tiếp hình ảnh tại [FogCam.org](https://fogcam.org/).

![](https://cdn.beekka.com/blogimg/asset/202210/bg2022100407.webp)

## 文摘

### Hệ quả của việc suy giảm tốc độ gió toàn cầu (Global terrestrial stilling)

Ngành công nghiệp khai thác điện gió đang được đầu tư phát triển vô cùng mạnh mẽ trên toàn thế giới để thay thế năng lượng hóa thạch. Tuy nhiên, hiệu quả của nguồn năng lượng này phụ thuộc hoàn toàn vào tốc độ gió tự nhiên. Vậy liệu có khi nào gió trên Trái Đất sẽ ngưng thổi?

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031413.webp)

Thực tế lịch sử gần đây ghi nhận vào giai đoạn mùa hè và mùa thu năm 2021, phần lớn khu vực châu Âu đã trải qua hiện tượng "hạn hán gió" (wind drought). Tốc độ gió trung bình tại nhiều quốc gia sụt giảm tới 15% so với mức trung bình nhiều năm, và nước Anh đã trải qua thời kỳ lặng gió nhất trong vòng 60 năm qua.

Nếu như vào tháng 9 năm 2020 sản lượng điện gió chiếm tới 18% tổng sản lượng điện của nước Anh, thì sang tháng 9 năm 2021 tỷ lệ này đã sụt giảm nghiêm trọng xuống chỉ còn 2%. Để bù đắp lượng điện năng thiếu hụt đột ngột này, chính phủ Anh đã buộc phải tái khởi động hai nhà máy nhiệt điện than đã đóng cửa trước đó.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031414.webp)

Một nghiên cứu khoa học cho thấy tốc độ gió trên đất liền toàn cầu đang có xu hướng giảm dần: trong giai đoạn từ năm 1978 đến năm 2010, tốc độ gió giảm trung bình 2,3% sau mỗi thập kỷ. Mặc dù từ năm 2010 đến năm 2019 tốc độ gió có xu hướng tăng nhẹ trở lại từ mức 7 dặm/giờ lên 7,4 dặm/giờ, các nhà khoa học dự báo tốc độ gió trung bình toàn cầu có thể giảm tới 10% vào năm 2100.

Nguyên nhân cốt lõi liên quan đến cơ chế hình thành gió của Trái Đất: Gió được tạo ra do sự chênh lệch nhiệt độ giữa hai cực lạnh giá và khu vực xích đạo nóng ấm dẫn đến luồng không khí di chuyển tuần hoàn. Tuy nhiên do tác động của biến đổi khí hậu toàn cầu, tốc độ tăng nhiệt độ ở khu vực Bắc Cực diễn ra nhanh hơn nhiều so với xích đạo, làm thu hẹp khoảng cách chênh lệch nhiệt độ giữa hai vùng và khiến gió thổi yếu đi. Ngoài ra, việc bùng nổ các công trình nhà cao tầng chọc trời tại các đô thị lớn trên thế giới cũng làm tăng độ nhám bề mặt Trái Đất, góp phần cản trở hướng di chuyển của các luồng gió.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023031415.webp)

Việc tốc độ gió suy giảm mang lại nhiều hệ lụy nghiêm trọng: Gió mạnh vốn giúp thổi bay khói bụi ô nhiễm tích tụ tại các đô thị lớn; tốc độ gió chậm khiến các đợt nắng nóng kéo dài khó hạ nhiệt hơn; và tốc độ gió yếu cũng gây cản trở cho máy bay cất cánh (do máy bay cần sức cản ngược chiều gió để tạo lực nâng). Số liệu tại một sân bay ở Hy Lạp cho thấy sức gió giảm kết hợp nhiệt độ tăng đã khiến tải trọng cất cánh tối đa của dòng máy bay Airbus A320 giảm mất 4 tấn trong vòng 30 năm qua.

## 言论

1、

> “Người nghệ sĩ không nhìn thế giới theo cách vốn có của nó, mà nhìn qua một lăng kính chắt lọc: vừa tối giản hơn nhưng lại phong phú và mạnh mẽ hơn rất nhiều.
> 
> Tác phẩm nghệ thuật ra đời không phải để người xem lặp lại trải nghiệm thực tế trần trụi, mà là để kiến tạo nên một điều mới mẻ từ thực tại đó, nhằm truyền tải một cảm xúc mạnh mẽ hơn đến người xem.”

-- [《Nghệ thuật biên tập hình ảnh》](https://simonsarris.substack.com/p/photo-editing-respecting-context)

2、

> “Một sự hiểu lầm rất phổ biến của người tiêu dùng là thực phẩm hết hạn sử dụng thì bắt buộc phải vứt bỏ.
> 
> Thực chất, hạn sử dụng ghi trên bao bì (Best before) hầu hết chỉ biểu thị mốc thời gian sản phẩm giữ được hương vị thơm ngon nhất chứ không đồng nghĩa với việc thực phẩm bị hỏng gây mất an toàn vệ sinh. Việc vứt bỏ ngay sản phẩm vừa mới hết hạn gây ra sự lãng phí thực phẩm cực kỳ lớn.”

-- [《Bốn ngộ nhận phổ biến về thực phẩm》](https://www.kiteandkeymedia.com/videos/common-myths-about-food-debunked/)

3、

> “Hành động chính là phương thuốc hữu hiệu nhất để đẩy lùi sự tuyệt vọng.”

-- [Joan Baez](https://www.brainyquote.com/quotes/joan_baez_132657), Nữ ca sĩ và nhạc sĩ người Mỹ

4、

> “Một số công ty phát triển phần mềm có khả năng biến những dự án lập trình đơn giản nhất thành một chuỗi quy trình làm việc vô cùng cồng kềnh phức tạp, đi kèm với vô số cuộc họp hành vô bổ kéo dài của các bên liên quan.
> 
> Bằng việc áp dụng các quy trình cứng nhắc hàng tuần, họ đã bóp nghẹt hoàn toàn niềm vui sáng tạo code và năng suất làm việc của các lập trình viên.”

-- [Một độc giả trên Hacker News](https://news.ycombinator.com/item?id=34368904)

## Lịch sử tuần này

- 2022年（第 199 期）：[An ninh mạng: Phân tích các sự cố liên quan đến chứng chỉ bảo mật HTTPS tại thị trường Nga](http://www.ruanyifeng.com/blog/2022/03/weekly-issue-199.html)
- 2021年（第 149 期）：[Ngành công nghiệp: Nhận định về cuộc đua thị phần xe điện toàn cầu và các thương hiệu dẫn đầu](http://www.ruanyifeng.com/blog/2021/03/weekly-issue-149.html)
- 2020年（第 97 期）：[Xã hội: Góc nhìn chia sẻ về nghị lực vượt khó học tập của các sĩ tử chuẩn bị thi đại học](http://www.ruanyifeng.com/blog/2020/03/weekly-issue-97.html)
- 2019年（第 47 期）：[Xu hướng nghề nghiệp: Thảo luận thực tế về việc phát triển nội dung ăn uống trực tuyến (Mukbang)](http://www.ruanyifeng.com/blog/2019/03/weekly-issue-47.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs là công cụ cộng tác tích hợp "soạn thảo tài liệu + bảng dữ liệu + ổ đĩa đám mây" hiệu quả cho cá nhân và nhóm.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
