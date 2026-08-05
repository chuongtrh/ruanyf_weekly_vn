# 科技爱好者周刊（第 392 期）：axios 投毒与好莱坞式骗术 (Bản tin công nghệ hàng tuần số 392: Mã độc axios và trò lừa bịp kiểu Hollywood)

Ghi lại nội dung công nghệ đáng chia sẻ hàng tuần, phát hành vào thứ Sáu.

Bản tin này [mã nguồn mở](https://github.com/ruanyf/weekly), hoan nghênh bạn [đóng góp](https://github.com/ruanyf/weekly/issues). Ngoài ra còn có dịch vụ [《Ai đang tuyển dụng》](https://github.com/ruanyf/weekly/issues/9454) đăng tải thông tin tuyển dụng lập trình viên. Hợp tác vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图 (Ảnh bìa)

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026040203.webp)

Khu phức hợp trụ sở mới của Tencent dự kiến đưa vào sử dụng trong năm nay, thường được gọi là "Đảo Cánh Cụt". Nơi đây không chỉ gồm các tòa nhà văn phòng mà còn tích hợp nhiều tòa nhà căn hộ lưu trú cho nhân viên. ([via](https://www.nfnews.com/content/0oXLNmjJo9.html))

## axios 投毒与好莱坞式骗术 (Mã độc axios và trò lừa bịp kiểu Hollywood)

Tuần trước, thư viện phần mềm nổi tiếng **axios** đã bị [tấn công đầu độc mã độc](https://cloud.tencent.com/announce/detail/2249). Hacker đã chiếm được token phát hành (publish token) của dự án và trực tiếp đẩy lên một phiên bản mới có chèn mã độc Trojan.

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026040703.webp)

Việc thư viện phần mềm bị cài mã độc không phải là chuyện mới, nhưng điểm gây sốc ở đây là cách thức rò rỉ token phát hành. Câu chuyện hậu trường của nó ly kỳ hệt như một bộ phim Hollywood, khiến nạn nhân hoàn toàn không có cách nào đề phòng.

axios là một trong những thư viện JS được sử dụng rộng rãi nhất thế giới, với lượt tải xuống hàng tuần lên tới gần 100 triệu lượt, do đó phạm vi ảnh hưởng của đợt đầu độc này cực kỳ nghiêm trọng.

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026040704.webp)

Hơn thế nữa, mã độc Trojan lần này có tính phá hoại rất cao. Theo [thông báo gỡ bỏ chính thức](https://github.com/axios/axios/issues/10636#issue-4195231282), nếu không may bị dính mã độc, **toàn bộ các khóa bảo mật (keys), token API và chứng thư số (credentials) lưu trên máy của bạn đều phải bị hủy bỏ ngay lập tức**. Mã độc này sẽ quét qua mọi thư mục trên ổ cứng, gom toàn bộ các khóa bảo mật tìm thấy rồi gửi ra ngoài.

Hãy nhớ rằng đối với những thư viện siêu phổ biến như axios, mọi khâu phát triển đều có cơ chế phòng vệ chặt chẽ và từng dòng code đều được kiểm duyệt gắt gao. **Đợt tấn công lần này hoàn toàn là một chiến dịch kỹ nghệ xã hội (social engineering) được dàn dựng vô cùng tinh vi**, vượt qua mọi lớp phòng vệ kỹ thuật đó.

Mục tiêu tấn công được xác định là nhà duy trì chính của dự án — Jason Saayman. Theo [chia sẻ cá nhân của anh ấy](https://github.com/axios/axios/issues/10636#issuecomment-4180237789), diễn biến sự việc như sau:

> "Họ đã thiết kế riêng một kịch bản hoàn hảo dành cho tôi, các bước cụ thể như sau:
> 
> 1. Họ giả danh làm nhà sáng lập của một công ty thật để liên hệ với tôi. Không chỉ làm giả thông tin cá nhân và hình ảnh của nhà sáng lập đó, họ còn làm giả trang web và hoạt động của chính công ty đó.
> 2. Sau đó, họ mời tôi gia nhập một không gian làm việc Slack có thật. Kênh Slack này sử dụng đầy đủ logo thương hiệu và tên gọi vô cùng thuyết phục. Không gian Slack được dàn dựng rất chi tiết, có riêng các kênh để chia sẻ bài viết trên LinkedIn. Tôi đoán các bài viết LinkedIn đó cũng được trích xuất từ tài khoản thật của công ty kia để tăng độ tin cậy. Họ cũng tạo sẵn một số tài khoản ảo đóng vai trò là nhân viên công ty và các nhà duy trì dự án mã nguồn mở khác.
> 3. Họ lên lịch hẹn gặp tôi qua ứng dụng Microsoft Teams để trao đổi công việc. Buổi họp trực tuyến có sự tham gia của một nhóm người.
> 4. Trong cuộc họp, họ chỉ ra một số thành phần trên hệ thống máy tính của tôi đã quá hạn. Tôi tin tưởng đó là vấn đề tương thích của phần mềm Teams nên đã tải xuống lắp đặt gói cập nhật do họ gửi qua, mà hoàn toàn không biết đó thực chất là một Trojan điều khiển từ xa (RAT).
> 5. Mọi khâu đều được sắp xếp bài bản, chuyên nghiệp và cực kỳ chính quy."

Có thể thấy, đợt tấn công này có kịch bản chi tiết, từng bước đi đều được chuẩn bị và tập dượt kỹ lưỡng, **thiết kế đo ni đóng giày riêng cho nạn nhân** chỉ chờ nạn nhân sập bẫy.

Kẻ lừa đảo cực kỳ kiên nhẫn và đầu tư chi phí ban đầu rất lớn. Bọn chúng làm giả website công ty, dựng sẵn kênh Slack chuyên nghiệp có thảo luận dự án và tài liệu chi tiết. Đáng nể nhất là chúng còn cử **một nhóm người thật lộ diện trong cuộc họp video trên Teams để ngồi họp cùng nạn nhân**.

Khi buổi họp diễn ra, người chủ trì bất ngờ nói: "Lạ nhỉ, hệ thống của anh có vẻ không tương thích với phần mềm của chúng tôi, có lẽ plugin Microsoft của anh bị lỗi thời rồi, để tôi gửi anh bản cập nhật mới nhất". Nạn nhân thấy mọi người trong cuộc họp đang đợi mình nên không mảy may nghi ngờ, tải về và nhấp đúp chạy file cài đặt. Thế là trúng bẫy, và token phát hành của axios bị đánh cắp chỉ trong vòng một nốt nhạc.

Trò lừa tinh vi đến mức đáng sợ.

Nó khiến tôi liên tưởng đến một [vụ án lừa đảo tại Ấn Độ](https://www.wsj.com/world/fake-cops-fake-judges-the-hollywood-style-scam-poised-to-go-global-e1e339a3?st=fXpKE6&mod=1440&user_id=66c4c9305d78644b3ac5df9c) mới đây, mức độ dàn dựng thậm chí còn tinh vi hơn nhiều.

Dịp Giáng sinh năm ngoái, một cụ bà 77 tuổi ở New Delhi nhận được cuộc gọi video qua WhatsApp từ một người tự xưng là "đồn cảnh sát". Góc dưới màn hình thậm chí còn có cả phiên dịch ngôn ngữ ký hiệu chuyên nghiệp.

"Cảnh sát" thông báo tài khoản ngân hàng của bà có liên quan đến đường dây rửa tiền lớn và yêu cầu bà hợp tác điều tra, nếu không toàn bộ tài sản sẽ bị phong tỏa tịch thu, đồng thời yêu cầu bà dự phiên điều trần trực tuyến của tòa án.

Báo chí sau đó đã phanh phui hình ảnh hiện trường đồn cảnh sát giả mà kẻ lừa đảo dựng lên, vô cùng chân thực. Bọn chúng dựng sẵn các phòng làm việc có biển hiệu cảnh sát Ấn Độ và cảnh sát Pakistan sát cạnh nhau trong cùng một tòa nhà để tiện bề lừa đảo nạn nhân của cả hai quốc gia đối địch này.

Vài ngày sau, cụ bà tham gia phiên điều trần trực tuyến do một "thẩm phán" giả chủ trì tại một phòng xét xử giả lập. Hắn xem xét sao kê dòng tiền, nghe "cảnh sát" trình bày chứng cứ và chất vấn cụ bà. Cuối cùng, "thẩm phán" yêu cầu cụ bà phải giữ kết nối video với đồn cảnh sát hàng ngày để phục vụ công tác xác minh tài sản cho đến khi vụ án được làm sáng tỏ.

Và đây là phần kịch tính nhất: Suốt 16 ngày liên tiếp, cụ bà luôn mở camera kết nối với đồn cảnh sát giả. Kẻ lừa đảo đã diễn sâu đến mức khó tin:

> "Trong 16 ngày đó, cụ bà dần nảy sinh tình cảm quý mến với các sĩ quan cảnh sát trực ca giả. Bà bắt đầu gọi họ là con của mình, và bọn chúng cũng ngọt ngào gọi bà là 'mẹ'.
> 
> Buổi tối, bà cùng một sĩ quan trẻ tuổi nhất ngồi đọc các kinh sách Ấn Độ giáo qua video, sĩ quan này thậm chí còn nhờ bà chép lại gửi cho hắn những đoạn kinh thư ý nghĩa.
> 
> 'Họ đối xử với tôi như người nhà vậy', cụ bà nhớ lại. 'Họ luôn động viên: Thưa bà, chúng con đang nỗ lực ngày đêm để sớm giải quyết xong vụ án cho bà'."

Bọn chúng kiên trì diễn kịch từ sáng đến đêm suốt 16 ngày, cùng đọc kinh sách, tâm sự chuyện đời với nạn nhân. Điều này giúp cụ bà hoàn toàn tin tưởng, tự nguyện bán hết các khoản đầu tư và thực hiện tổng cộng 9 lần chuyển tiền trị giá 1,6 triệu USD vào tài khoản của bọn lừa đảo. Ngày hôm sau, khi bà cố gắng liên lạc lại với "các con ở đồn cảnh sát" thì hệ thống đã hoàn toàn mất kết nối.

Qua hai ví dụ trên, chúng ta có thể thấy các trò lừa đảo công nghệ ngày nay đã được nâng tầm thành các chiến dịch "kịch bản phân vai" nhắm mục tiêu chính xác với tỷ lệ thành công cực cao. Nếu có thêm sự hỗ trợ của công nghệ deepfake AI trong tương lai, việc phân biệt thật giả sẽ là điều bất khả thi.

Trong phát triển phần mềm có nguyên tắc: Mọi yêu cầu gửi lên từ phía client đều không được tin tưởng và phải giả định là độc hại. Có lẽ cuộc sống thực tế sắp tới cũng sẽ như vậy: Mọi người lạ liên hệ đều phải giả định là một trò lừa đảo cho đến khi được xác minh rõ ràng.

## 算力依然不足 (Năng lực tính toán vẫn tiếp tục khan hiếm)

Ba sự việc diễn ra gần đây cho thấy năng lực tính toán (compute power) vẫn đang rơi vào trạng thái cực kỳ căng thẳng:

1. OpenAI [quyết định tạm dừng](https://finance.sina.cn/stock/jdts/2026-04-07/detail-inhtsezc7221412.d.html) cung cấp dịch vụ tạo video Sora do không đủ tài nguyên tính toán, hãng cần tập trung phần cứng cho các mảng kinh doanh cốt lõi.
2. Anthropic chính thức cấm việc dùng các gói thuê bao tháng cá nhân cho các dịch vụ gọi API của bên thứ ba (như OpenClaw, OpenCode...). Bởi vì nếu người dùng tận dụng tối đa gói thuê bao, lượng GPU tiêu thụ sẽ vượt xa số tiền họ trả. Hãng cần ưu tiên tài nguyên cho sản phẩm chính chủ của mình (như Claude Code).
3. Thống kê cho thấy lượng commit code trên GitHub trong 3 tháng đầu năm nay tăng gấp 14 lần so với cùng kỳ năm ngoái, chủ yếu do sự bùng nổ của lập trình bằng AI. Hệ thống của GitHub liên tục gặp sự cố quá tải do hạ tầng không đáp ứng kịp. Tỷ lệ uptime của GitHub trong 3 tháng qua chỉ đạt 89.47%, kém xa tiêu chuẩn 99.99%.

Những việc này cho thấy giá cả phần cứng AI sẽ còn tiếp tục tăng cao, và các dịch vụ miễn phí của các nền tảng lập trình như GitHub có xu hướng sẽ bị thu hẹp lại để chuyển sang thu phí hoàn toàn.

## 前端是不是重复劳动？ (Lập trình frontend có phải là công việc lặp đi lặp lại?)

Một nhà phát triển nhận định: Bản chất công việc của frontend luôn trùng lặp — hiển thị dữ liệu cho người dùng và cung cấp công cụ để người dùng xử lý dữ liệu đó.

Để tránh việc lặp đi lặp lại giải quyết một bài toán, ông đã xây dựng dự án "[Trình duyệt tự thích ứng](https://github.com/jonnonz1/adaptive-browser)" (Adaptive Browser). Hệ thống sử dụng AI để tự động sinh ra giao diện UI ở frontend, phía backend chỉ cần cung cấp dữ liệu thô và mô tả ngắn gọn mục đích của trang web. Đây có thể là một hướng đi mới cho tương lai của lập trình frontend.

## Adobe 修改 hosts 文件 (Adobe tự ý sửa đổi file hosts của hệ thống)

Nhiều người dùng cài đặt bộ phần mềm Creative Cloud của Adobe đã vô cùng ngỡ ngàng khi phát hiện trình cài đặt của hãng tự ý chỉnh sửa và chèn thêm các dòng cấu hình DNS cục bộ vào tệp tin hosts của hệ điều hành.

Theo các chuyên gia giải thích, đây là cơ chế Adobe dùng để kiểm tra xem máy người dùng đã cài đặt Creative Cloud hay chưa. Khi người dùng truy cập trang chủ của hãng, trang web sẽ gửi một yêu cầu ngầm đến domain nội bộ được định nghĩa trong file hosts, nếu nhận được phản hồi nghĩa là máy đã cài đặt phần mềm. Việc một hãng phần mềm lớn sử dụng giải pháp mang tính "cửa sau" này đối với chính những khách hàng trả phí của mình thực sự gây nhiều ngao ngán.

## 文章 (Bài viết)

1、[Kiến trúc hạ tầng frontend của MDN](https://developer.mozilla.org/en-US/blog/mdn-front-end-deep-dive/) (Tiếng Anh)

Phân tích sâu về cấu trúc hạ tầng frontend của trang tài liệu kỹ thuật lớn nhất internet MDN, với mức độ phức tạp vượt ngoài dự đoán của nhiều người.

2、[Khai tử người viết code](https://windliang.wang/2026/03/31/%E6%9D%80%E6%AD%BB%E9%82%A3%E4%B8%AA%E5%86%99%E4%BB%A3%E7%A0%81%E7%9A%84%E4%BA%BA/) (Tiếng Trung)

Tác giả là một lập trình viên frontend tại một tập đoàn lớn, chia sẻ lại trải nghiệm cá nhân trong năm qua từ việc tự gõ code chuyển hẳn sang lập trình bằng AI, làm thay đổi hoàn toàn tư duy và xóa bỏ nỗi lo sợ "bị sa thải ở tuổi 35". (Đóng góp từ [@wind-liang](https://github.com/ruanyf/weekly/issues/9545))

3、[Dựng SMS Gateway bằng điện thoại Android cũ](https://jonno.nz/posts/built-an-sms-gateway-with-a-20-dollar-android-phone/) (Tiếng Anh)

Hướng dẫn tận dụng một chiếc điện thoại Android cũ để thiết lập cổng SMS Gateway cá nhân, giúp gửi và nhận tin nhắn SMS thông qua kết nối mạng.

4、[Kiểm thử endian bằng phần mềm giả lập QEMU](https://www.hanshq.net/big-endian-qemu.html) (Tiếng Anh)

Tài liệu hướng dẫn C cơ bản, sử dụng máy ảo QEMU để chạy một chương trình ngắn dưới 10 dòng nhằm kiểm tra cấu trúc hệ thống là Big-Endian hay Little-Endian.

5、[Tính năng importtime trong Python](https://simonwillison.net/2025/Jun/20/python-importtime-graph/) (Tiếng Anh)

Việc gọi lệnh `import` các thư viện trong Python gây ảnh hưởng nhất định đến hiệu năng. Bài viết giới thiệu tính năng tích hợp sẵn `importtime` giúp đo đạc chi tiết thời gian load của từng module.

6、[Thảm họa tàu ngầm hạt nhân Kursk năm 2000](https://rarehistoricalphotos.com/kursk-submarine-disaster-photos/) (Tiếng Anh)

Tái hiện lại thảm họa nổ và chìm tàu ngầm hạt nhân Kursk của Nga khiến toàn bộ 118 thủy thủ tử nạn qua các tư liệu ảnh lịch sử chi tiết.

## 工具 (Công cụ)

1、[Google AI Edge Gallery](https://apps.apple.com/nl/app/google-ai-edge-gallery/id6749645337)

Google phát hành ứng dụng chính thức cho iOS cung cấp khả năng chạy offline mô hình Gemma 4 trực tiếp trên điện thoại mà không cần kết nối mạng.

2、[apfel](https://apfel.franzai.com/)

Công cụ dòng lệnh giúp gọi và sử dụng mô hình lớn tích hợp sẵn cục bộ của hệ điều hành macOS (vốn dĩ mặc định chỉ cấp quyền cho trợ lý ảo Siri gọi).

3、[Docking](https://docking.cc/)

Tiện ích giúp bổ sung thanh Dock ứng dụng tương tự macOS cho các giao diện màn hình máy tính chạy Linux.

4、[Tantivy](https://github.com/quickwit-oss/tantivy)

Thư viện tìm kiếm toàn văn (full-text search) viết bằng Rust đạt hiệu năng cao, giải pháp thay thế cho Apache Lucene.

5、[Open Screen](https://github.com/siddharthvaddem/openscreen)

Ứng dụng desktop đa nền tảng hỗ trợ quay màn hình và tích hợp sẵn trình chỉnh sửa video để tạo các video demo giới thiệu sản phẩm.

6、[epub-tts](https://github.com/rafael1mc/epub-tts)

Công cụ nguồn mở hỗ trợ chuyển đổi tệp sách điện tử định dạng epub sang file âm thanh audiobook dải giọng đọc tự nhiên.

7、[NVTOP](https://github.com/Syllo/nvtop)

Công cụ dòng lệnh cho Linux tương tự như lệnh `top` nhưng chuyên dùng để theo dõi hiệu năng, nhiệt độ và dung lượng bộ nhớ của card đồ họa GPU.

8、[dmcheck](https://github.com/PlayerYK/dmcheck)

Công cụ hỗ trợ quét kiểm tra nhanh tình trạng đăng ký của các tên miền liên quan đến một từ khóa chỉ định. (Đóng góp từ [@PlayerYK](https://github.com/ruanyf/weekly/issues/9542))

9、[Reze Studio](https://github.com/AmyangXYZ/reze-studio)

Trang web nguồn mở hỗ trợ chỉnh sửa và tạo các đường cong chuyển động (animation curve) trực quan. (Đóng góp từ [@AmyangXYZ](https://github.com/ruanyf/weekly/issues/9555))

10、[gitlogue](https://github.com/unhappychoice/gitlogue)

Tiện ích hiển thị hoạt họa lịch sử commit của kho Git trực tiếp trên giao diện terminal.

## 资源 (Tài nguyên)

1、[Phật Tân (佛津)](https://fojin.app/): Nền tảng số hóa và lưu trữ các thư tịch, cổ tịch Phật giáo trên toàn cầu. (Đóng góp từ [@xr843](https://github.com/ruanyf/weekly/issues/9507))

2、[Flight Viz](https://flight-viz.com/): Bản đồ trực quan 3D theo dõi thời gian thực các chuyến bay đang hoạt động trên toàn cầu. (Đóng góp từ [@haojiang99](https://github.com/ruanyf/weekly/issues/9538))

3、[Lịch sử phát triển GPU](https://sheets.works/data-viz/every-gpu): Biểu đồ hình ảnh tổng hợp quá trình phát triển của card đồ họa GPU từ dòng card Voodoo năm 1996 đến RTX 5090 năm 2025.

## 图片 (Hình ảnh)

1. [Phủ xanh đồi trọc bằng vỏ cam](https://www.sciencealert.com/how-12-000-tonnes-of-dumped-orange-peel-produced-something-nobody-imagined): Một nhà máy sản xuất nước cam tại Costa Rica đã đổ 12.000 tấn vỏ cam thải lên một vùng đồi trọc hoang hóa để làm phân bón tự nhiên. Sau 6 tháng vỏ cam phân hủy tạo thành lớp đất mùn đen màu mỡ, và sau 16 năm nơi đây đã hồi sinh thành một cánh rừng rậm rạp xanh tốt mà không cần thêm bất kỳ sự can thiệp nhân tạo nào.

2. [Ảnh đoạt giải Vật lý toàn cầu 2025](https://www.quantamagazine.org/global-physics-photowalk-2025-winners-revealed-20260401/): Tổng hợp các tác phẩm đoạt giải chụp ảnh các phòng thí nghiệm vật lý hạt lớn trên thế giới nhằm phổ cập khoa học đến công chúng.

## 文摘 (Văn trích)

1、[Tại sao cát ở bãi biển lại có tính bám dính?](https://www.mentalfloss.com/posts/why-is-sand-sticky)

Cát bãi biển có thành phần chính là silicon dioxide tương tự như đá thông thường, nhưng đá không bám dính còn cát lại dính chặt vào da và quần áo khi đi biển. Nguyên nhân là do cát có tính亲 thủy (hút nước), cơ thể người lại đổ mồ hôi dưới nắng tạo độ ẩm, sự liên kết của các phân tử nước tạo lực bám dính giữ cát lại trên da. Kem chống nắng, dầu dưỡng da và các nếp nhăn nhỏ trên da cũng góp phần giữ cát lại. Cách duy nhất để làm sạch cát là chờ cho da khô hoàn toàn rồi phủi sạch hoặc dùng nước rửa trôi.

## 言论 (Phát ngôn)

1、

> "Nếu bạn nghĩ tốc độ gõ code hiện tại là vấn đề lớn nhất của bạn, thì thực tế vấn đề bạn đang đối mặt còn lớn hơn thế rất nhiều (mấu chốt nằm ở việc hiểu rõ yêu cầu nghiệp vụ)."
> 
> -- Andrew Murphy, lập trình viên người Úc.

2、

> "Có một kiểu hưng phấn và lạc quan tột độ mà chỉ những người mới bắt đầu bước chân vào thị trường tiền mã hóa năm 2017 mới có được."
> 
> -- Andrew Murphy

3、

> "Tại các trường đại học, hội đồng khoa học yêu cầu nghiên cứu sinh tiến sĩ phải xuất bản bài báo khoa học, còn việc bạn viết cái gì, viết thế nào có thực chất liên quan đến hướng nghiên cứu hay không thì họ không mấy quan tâm. Khoa cần bài báo để chứng minh tính hợp lý của các khoản ngân sách được cấp, và ngân sách lại nuôi sống sự tồn tại của khoa. Sinh viên chỉ là tư liệu sản xuất phục vụ mục tiêu đó."
> 
> -- 《Máy móc không có vấn đề, vấn đề nằm ở chính con người chúng ta》

4、

> "Trở thành một thành phố tương lai đối với tôi là những nơi thân thiện có lối đi bộ và làn đường xe đạp như Amsterdam, chứ không phải là những nơi chằng chịt xa lộ 16 làn xe và tầng lớp lao động bị bóc lột phục vụ trong các trung tâm mua sắm xa xỉ kiểu Dubai."
> 
> -- Độc giả Hacker News

## 往年回顾 (Nhìn lại các năm trước)

[Chuẩn kết nối HDMI 2.2 có thể đã đạt tới giới hạn vật lý](https://www.ruanyifeng.com/blog/2025/04/weekly-issue-345.html) (#345)

[Mẫu đồng hồ bóng đèn độc đáo](https://www.ruanyifeng.com/blog/2024/03/weekly-issue-295.html)（#295）

[Nhà cao tầng chọc trời là thiết kế phản tự nhiên](https://www.ruanyifeng.com/blog/2023/03/weekly-issue-245.html)（#245）

[Bạn đã từng làm dự án nào mà hoàn toàn không quan tâm đến kết quả chưa?](https://www.ruanyifeng.com/blog/2022/02/weekly-issue-195.html)（#195）

(Hết)
