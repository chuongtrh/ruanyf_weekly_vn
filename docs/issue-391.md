# 科技爱好者周刊（第 391 期）：AI 的贫富分化 (Bản tin công nghệ hàng tuần số 391: Sự phân hóa giàu nghèo của AI)

Ghi lại nội dung công nghệ đáng chia sẻ hàng tuần, phát hành vào thứ Sáu.

Bản tin này [mã nguồn mở](https://github.com/ruanyf/weekly), hoan nghênh bạn [đóng góp](https://github.com/ruanyf/weekly/issues). Ngoài ra còn có dịch vụ [《Ai đang tuyển dụng》](https://github.com/ruanyf/weekly/issues/9454) đăng tải thông tin tuyển dụng lập trình viên. Hợp tác vui lòng [liên hệ qua email](mailto:yifeng.ruan@gmail.com) (yifeng.ruan@gmail.com).

## 封面图 (Ảnh bìa)

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026040107.webp)

Trang trí trên bức tường của một nhà hàng ở Thượng Hải. (via [monana3838@Threads](https://www.threads.com/@monana3838/post/DWjVcmcAoh4))

## AI 的贫富分化 (Sự phân hóa giàu nghèo của AI)

Tôi ngày càng cảm thấy AI rất khác biệt so với các công nghệ khác. Nó không chỉ mang lại cuộc cách mạng công nghệ, mà còn kéo theo cả cuộc cách mạng xã hội.

Nói một cách đơn giản, AI sẽ tạo ra sự phân hóa giàu nghèo sâu sắc.

Hầu hết các công nghệ trước đây thực tế lại giúp xóa bỏ sự phân hóa giàu nghèo ở khía cạnh tiêu dùng, tạo ra "sự bình đẳng cho người tiêu dùng". Nghĩa là người giàu và người nghèo cùng tiêu dùng các sản phẩm giống nhau.

Ví dụ, mọi người đều uống cùng một loại Coca-Cola, dùng chung chiếc điện thoại iPhone, hay lái cùng một chiếc xe Tesla. Ngay cả mạng internet cũng vậy, người giàu nhất thế giới Elon Musk cũng lướt cùng một trang web và dùng chung một ứng dụng di động giống hệt bạn.

Thế nhưng các mô hình AI thì không như vậy. **Trước các mô hình lớn, người giàu và người nghèo hoàn toàn không bình đẳng**.

Trong tương lai, người bình thường chắc chắn không thể chi trả nổi phí sử dụng của các mô hình hàng đầu. Thực tế hiện nay đã chứng minh điều đó: Gói lập trình AI đắt nhất hiện tại là Max của Claude Code có giá tới 200 USD/tháng, mức giá mà rất nhiều người đã không thể gánh nổi.

OpenAI từng có ý định ra mắt [gói thuê bao trị giá 20.000 USD/tháng](https://www.thepaper.cn/newsDetail_forward_30320495) để cung cấp dịch vụ mô hình đỉnh cao nhất và không giới hạn dung lượng.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026032207.webp)

Nếu gói này thực sự ra mắt, chỉ có giới siêu giàu mới có thể tiếp cận.

Thực tế này phản ánh một quy luật đơn giản: **Chi phí càng đắt, mô hình hoạt động càng hiệu quả**. Bởi vì chất lượng mô hình phụ thuộc trực tiếp vào năng lực tính toán. Lượng GPU nhiều hơn, cửa sổ ngữ cảnh lớn hơn, số lượng tham số khổng lồ hơn đều đòi hỏi chi phí tài chính cực lớn.

Điều này trái ngược hoàn toàn với hàng hóa công nghiệp thông thường. Hàng công nghiệp có hiệu ứng quy mô (economies of scale), sản lượng càng lớn thì chi phí đơn vị càng giảm, giúp sản phẩm ngày càng rẻ khi sản xuất hàng loạt.

Ngược lại, **mô hình lớn không có hiệu ứng quy mô**. Việc mở rộng quy mô mô hình đòi hỏi thêm vô số máy chủ vật lý, không hề giúp giảm chi phí đơn vị mà trái lại còn làm tăng chi phí do phải mở rộng phòng máy, nâng cấp hệ thống điện nước tản nhiệt.

Xã hội tương lai có xu hướng sẽ phân chia: Người giàu và người nghèo sử dụng các mô hình khác nhau. Các dịch vụ cao cấp nhất của AI như lên kế hoạch, tư vấn doanh nghiệp, tạo nội dung, tự động hóa... đòi hỏi phí sử dụng đắt đỏ, trong khi người bình thường chỉ có thể tiếp cận các mô hình miễn phí với chất lượng rất đỗi bình thường.

Tuy nhiên, Elon Musk [gần đây nhận định](https://wap.cj.sina.cn/7x24/4762771) rằng tương lai vẫn có một khả năng khác xảy ra.

![](https://cdn.beekka.com/blogimg/asset/202603/bg2026032206.webp)

Ý ông là, năng lực tính toán về bản chất là một dạng năng lượng chuyển hóa. Một khi loài người hiện thực hóa được nguồn năng lượng sạch giá siêu rẻ với nguồn cung vô hạn (như điện mặt trời không gian), năng lực tính toán sẽ trở nên vô cùng rẻ và tất cả mọi người đều được sử dụng mô hình tốt nhất.

Điều này có khả thi không? Tôi không chắc chắn lắm, cảm giác kịch bản phân hóa ở trên vẫn thực tế hơn.

## 模型能力的一种衡量方法 (Một phương pháp đo lường năng lực mô hình)

Làm thế nào để đánh giá chính xác năng lực của mô hình lớn?

Phương pháp truyền thống là sử dụng các bộ đề test để chấm điểm mô hình. Nhược điểm là chỉ dùng để so sánh ngang hàng giữa các mô hình chứ khó đánh giá được tốc độ tiến hóa của chúng.

Gần đây, một nghiên cứu đã đề xuất [phương pháp đo lường mới](https://emptysqua.re/blog/review-measuring-ai-ability-to-complete-long-software-tasks/):

Đầu tiên, đo lường khoảng thời gian trung bình mà một con người cần để hoàn thành một tác vụ chỉ định. Ví dụ, tính phép cộng đơn giản mất 2 giây, còn tính nhân phức tạp mất 1 phút. Tiếp theo, test xem mô hình lớn có thể hoàn thành tác vụ đó với tỷ lệ thành công 50% hay không.

Kết quả nghiên cứu chỉ ra: Với tỷ lệ thành công 50%, GPT-2 chỉ giải quyết được tác vụ trong ngưỡng thời gian 2 giây của con người; Claude 3.7 Sonnet đạt mốc 50 phút; model o3 đạt gần 2 giờ; và Opus 4.6 chạm mốc 12 giờ.

Nghĩa là, đối với một tác vụ phức tạp đòi hỏi một chuyên gia con người làm liên tục suốt 12 giờ mới xong, mô hình Opus 4.6 đã có khả năng hoàn thành nó với tỷ lệ thành công đạt 50%.

![](https://cdn.beekka.com/blogimg/asset/202604/bg2026040201.webp)

Biểu đồ trên cho thấy, tốc độ tiến hóa của mô hình lớn là một đường thẳng tắp trên hệ tọa độ logarit: **Cứ sau mỗi 7 tháng, ngưỡng thời gian của các tác vụ mà mô hình lớn có thể giải quyết được (với tỷ lệ thành công 50%) lại tăng gấp đôi**. Theo xu hướng này, trong khoảng thời gian từ năm 2027 đến năm 2031, AI sẽ có khả năng hoàn thành các tác vụ phức tạp đòi hỏi chuyên gia con người làm việc ròng rã suốt một tháng trời với tỷ lệ thành công 50%.

Nếu nghiên cứu này chính xác, mô hình ra mắt vào cuối năm sẽ có năng lực mạnh gấp đôi mô hình đầu năm.

## 科技动态 (Tin tức Công nghệ)

1. [Giải thưởng từ Điều khoản dịch vụ](https://www.cape.co/blog/easter-egg-in-privacy-policy): Các văn bản Điều khoản dịch vụ (ToS) của phần mềm thường dài dòng và khó hiểu nên hầu như không ai đọc. Một nhà mạng Mỹ đã chèn ngầm một câu ẩn vào sâu trong văn bản của họ: "Nếu bạn đọc được dòng chữ này, hãy gửi email cho chúng tôi để nhận chuyến du lịch Thụy Sĩ miễn phí". Sau hai tuần mới có một cô gái phát hiện và gửi thư, thế là cô ấy có chuyến đi Thụy Sĩ hoàn toàn miễn phí. Thực tế là ngay cả khi có giải thưởng lớn, người dùng vẫn không đọc ToS. Cách làm của tôi hiện nay là quẳng văn bản đó cho AI đọc hộ và hỏi: "Văn bản này có những điều khoản nào bất lợi cho người dùng không?".

2. [Sơn móng tay cho màn hình cảm ứng](https://www.livescience.com/chemistry/chemistry-student-develops-clear-polish-that-turns-your-fingernail-into-a-touch-screen-stylus): Màn hình cảm ứng điện dung phổ biến đòi hỏi vật chạm phải có tính dẫn điện (như ngón tay) để nhận diện vị trí, nên khi đeo găng tay vào mùa đông sẽ bị liệt cảm ứng. Một sinh viên hóa học người Mỹ đã chế tạo loại sơn móng tay trong suốt chứa các hạt kim loại dẫn điện siêu nhỏ. Sơn này có thể quét lên đầu ngón tay của găng tay mà không làm thay đổi màu sắc của găng, giúp tương tác với màn hình cảm ứng dễ dàng khi đeo găng tay.

3. [Quảng cáo ẩn của Copilot](https://www.theregister.com/2026/03/30/github_copilot_ads_pull_requests/): Nhiều người dùng phát hiện công cụ GitHub Copilot tự ý chèn các nội dung quảng cáo giới thiệu ứng dụng Raycast vào phần cuối mô hình tóm tắt PR (Pull Request) tự động của họ. Quét tìm trên GitHub phát hiện hơn 11.400 PR chứa chung đoạn quảng cáo này. Sau khi bị người dùng phản đối mạnh mẽ, GitHub đã tạm dừng tính năng này, nhưng đây là tín hiệu cho thấy hãng đang tìm cách tận dụng người dùng để tăng doanh thu.

## 文章 (Bài viết)

1、[Đánh giá Xiaomi MiMo v2 Pro](https://decrypt.co/362633/xiaomi-mimo-v2-pro-review-so-good-mistaken-deepseek-v4) (Tiếng Anh)

Đánh giá chi tiết của truyền thông nước ngoài về dòng mô hình lớn mới ra mắt MiMo V2 của Xiaomi, dành nhiều lời khen ngợi cho hiệu năng của mô hình.

2、[Tôi dùng AI tự tạo một JavaScript engine](https://p.ocmatos.com/blog/jsse-a-javascript-engine-built-by-an-agent.html) (Tiếng Anh)

Nhật ký quá trình tác giả sử dụng AI Agent trong vòng 6 tuần để xây dựng một JS engine hoàn chỉnh vượt qua toàn bộ 98.426 kịch bản kiểm thử của bộ test262.

3、[Mổ xẻ thư mục .claude/](https://blog.dailydoseofds.com/p/anatomy-of-the-claude-folder) (Tiếng Anh)

Khám phá thư mục ẩn `.claude/` do công cụ Claude Code tự động tạo ra trong dự án để tìm hiểu cấu trúc dữ liệu lưu trữ phía dưới của AI.

4、[Giới thiệu thuật toán Consistent Hashing](https://eli.thegreenplace.net/2025/consistent-hashing) (Tiếng Anh)

Phân tích cơ chế hoạt động của thuật toán băm nhất quán (Consistent Hashing) thường dùng trong thiết lập cache hệ thống phân tán để hạn chế ảnh hưởng đến các vị trí cache sẵn có khi thêm bớt server.

5、[Biến màn hình laptop thành màn hiển thị HDMI cho Raspberry Pi](https://danielmangum.com/posts/laptop-hdmi-monitor-sbc/) (Tiếng Anh)

Hướng dẫn sử dụng card ghi hình (capture card) chuyển đổi tín hiệu HDMI sang cổng USB để tận dụng màn hình laptop làm màn hiển thị cho máy tính đơn mạch Raspberry Pi.

## 工具 (Công cụ)

1、[EmDash](https://github.com/emdash-cms/emdash)

Dự án tái lập hệ thống WordPress nguồn mở hoàn toàn bằng ngôn ngữ TypeScript do AI tự động viết ra, hỗ trợ đầy đủ các hệ thống plugin tương thích.

2、[SubsTracker](https://github.com/wangwangit/SubsTracker)

Hệ thống quản lý dịch vụ thuê bao (subscriptions) chạy trên Cloudflare Workers hỗ trợ gửi thông báo gia hạn qua Telegram, Webhook. (Đóng góp từ [@wangwangit](https://github.com/ruanyf/weekly/issues/9411))

3、[OpeniLink Hub](https://github.com/openilink/openilink-hub)

Nền tảng quản lý robot WeChat nguồn mở có tích hợp kho ứng dụng plugin phong phú để người dùng cài đặt thêm tính năng. (Đóng góp từ [@xixihhhh](https://github.com/ruanyf/weekly/issues/9404)). Một dự án tương tự là [wxWebHook](https://github.com/aristorechina/wxWebHook) hỗ trợ đẩy tin nhắn qua Webhook (Đóng góp từ [@aristorechina](https://github.com/ruanyf/weekly/issues/9412)).

4、[Lixian.Online](https://lixian.online/)

Công cụ hỗ trợ tải nhanh các tệp cài đặt offline của các plugin VSCode, extension Chrome và Docker images. (Đóng góp từ [@LiaoGuoYin](https://github.com/ruanyf/weekly/issues/9455))

5、[Rename.Tools](https://rename.tools/zh/app)

Ứng dụng web chạy offline hỗ trợ đổi tên file hàng loạt theo các quy tắc định nghĩa sẵn. (Đóng góp từ [@chenz24](https://github.com/ruanyf/weekly/issues/9461))

6、[FontInAss](https://github.com/Yuri-NagaSaki/FontInAss)

Công cụ nguồn mở hỗ trợ trích xuất font chữ và nhúng trực tiếp vào file phụ đề định dạng ASS. (Đóng góp từ [@Yuri-NagaSaki](https://github.com/ruanyf/weekly/issues/9466))

7、[pretext.video](https://github.com/fifteen42/pretext-video)

Ứng dụng nhỏ dựng trên thư viện pretext giúp chuyển đổi trực tiếp hình ảnh camera bắt viền cơ thể người thành nghệ thuật sắp đặt chữ (ASCII art) thời gian thực. (Đóng góp từ [@fifteen42](https://github.com/ruanyf/weekly/issues/9472))

8、[OxideTerm](https://github.com/AnalyseDeCircuit/oxideterm)

Ứng dụng SSH client đa nền tảng viết bằng Rust dựa trên framework Tauri. (Đóng góp từ [@AnalyseDeCircuit](https://github.com/ruanyf/weekly/issues/9474))

9、[wtree](https://github.com/FatDoge/wtree)

Giao diện quản lý đồ họa cho tính năng `git worktree`. (Đóng góp từ [@FatDoge](https://github.com/ruanyf/weekly/issues/9483))

## AI 相关 (AI Liên quan)

1、[Open Agent SDK](https://github.com/shipany-ai/open-agent-sdk)

Bộ thư viện mã nguồn mở thay thế cho claude-agent-sdk được dựng lại dựa trên mã nguồn rò rỉ của Claude Code để phục vụ lập trình AI Agent, tương thích hoàn toàn giao tiếp và không cần chạy tiến trình CLI cục bộ. (Đóng góp từ [@idoubi](https://github.com/ruanyf/weekly/issues/9473))

2、[Antigravity Gateway](https://github.com/Truthan49/Antigravity-Everywhere)

Giao diện điều khiển Web giúp quản lý tập trung các AI Agent chạy cục bộ của bạn, hỗ trợ chia không gian làm việc và đồng bộ nhóm qua Lark/Feishu. (Đóng góp từ [@Mr-ZhangBo](https://github.com/ruanyf/weekly/issues/9395))

3、[ArcReel](https://github.com/ArcReel/ArcReel)

Hệ thống AI tự động hóa sản xuất video ngắn: Tự dịch tiểu thuyết thành kịch bản, thiết kế nhân vật, vẽ phân cảnh storyboard và dựng video hoàn chỉnh. (Đóng góp từ [@Pollo3470](https://github.com/ruanyf/weekly/issues/9393))

4、[TermCanvas](https://github.com/blueberrycongee/termcanvas)

Ứng dụng desktop trải phẳng toàn bộ các cửa sổ terminal lên một bảng vẽ vô hạn để tiện quản lý các tác vụ AI. (Đóng góp từ [@blueberrycongee](https://github.com/ruanyf/weekly/issues/9434)). Một dự án tương tự là [OpenCove](https://github.com/DeadWaveWave/opencove) (Đóng góp từ [@DeadWaveWave](https://github.com/ruanyf/weekly/issues/9497)).

## 资源 (Tài nguyên)

1、[Claude Code thực hành](https://claude.nagdy.me/): Trang web hướng dẫn học cách sử dụng các tính năng của Claude Code qua 11 bài tập nhỏ trực quan.

2、[Claude Code Unpacked](https://ccunpacked.dev/): Phân tích chi tiết quy trình xử lý nội bộ của Claude Code sau khi nhận câu lệnh prompt dựa trên mã nguồn rò rỉ của dự án.

## 图片 (Hình ảnh)

1. [Cây của năm tại châu Âu](https://nicenews.com/environment/european-tree-of-the-year-winners-2026/): Giới thiệu cuộc thi bình chọn cây tiêu biểu hàng năm tại châu Âu giúp nâng cao nhận thức bảo tồn sinh thái và quảng bá du lịch địa phương. Cây đoạt giải năm nay là cây sồi 400 tuổi tại một ngôi làng ở Lithuania.

## 文摘 (Văn trích)

1、[Càng dùng AI tôi lại càng ít lo lắng](https://simonwillison.net/2025/Jul/4/identify-solve-verify/)

Thời gian tôi dùng AI để viết code càng nhiều thì tôi lại càng ít lo lắng về sự nghiệp lập trình của mình, dù AI đang ngày càng giỏi hơn. Bởi vì tôi nhận ra việc viết code chỉ là một khâu nằm ở giữa của quy trình làm việc. Công việc thực chất của tôi là: **Phát hiện ra bài toán có thể giải quyết bằng code, tiến hành giải quyết bài toán đó và kiểm chứng lại xem giải pháp có hoạt động hiệu quả không**. AI có thể làm thay hoàn toàn khâu gõ code ở giữa, nhưng luôn cần con người để xác định đề bài và xác nhận kết quả cuối cùng. Đó mới là 80% giá trị công việc của tôi.

2、[Sự kém bền vững của Định luật Moore](https://bzolang.blog/p/the-unsustainability-of-moores-law)

Bên cạnh việc mật độ bóng bán dẫn tăng gấp đôi sau mỗi 2 năm, Định luật Moore còn một hệ quả ít ai nhắc đến: Cứ sau mỗi 5 năm, chi phí xây dựng một nhà máy đúc chip (fab) lại tăng gấp đôi, và số lượng công ty có đủ tiềm lực tài chính để xây dựng fab sẽ giảm đi một nửa. Cách đây 25 năm có 40 công ty tự xây được fab với chi phí 2-4 tỷ USD/nhà máy. Ngày nay chỉ còn 2-3 công ty đúc được chip tiên tiến nhất với chi phí lên tới hàng chục tỷ USD. Khi tiến trình sản xuất chạm ngưỡng giới hạn vật lý 1nm, Định luật Moore sẽ sớm kết thúc và sự phát triển trong tương lai sẽ phụ thuộc vào quy mô cụm năng lực tính toán chung thay vì sức mạnh của một chip đơn lẻ.

## 言论 (Phát ngôn)

1、

> "Việc file sourcemap chứa mã nguồn gốc bị đẩy nhầm lên thư viện npm nghe qua có vẻ khó tin, nhưng sẽ rất dễ hiểu nếu bạn nhận ra phần lớn codebase của dự án bạn đang chuẩn bị release thực chất do AI tự viết."
> 
> -- Bình luận của độc giả về vụ rò rỉ code của Claude Code

2、

> "Sự bùng nổ của AI sẽ khiến nhu cầu của một số công việc văn phòng giảm đi, nhưng lại tạo ra lượng lớn cơ hội việc làm cho các thợ điện, thợ hàn và thợ sửa ống nước. Trước đây chúng ta khuyên thanh niên học đại học để làm ngân hàng, truyền thông hay luật; nay cần cân bằng lại vì các công việc tay chân kỹ thuật cao cũng mang lại sự nghiệp rất thành công."
> 
> -- Larry Fink, CEO của tập đoàn tài chính BlackRock.

3、

> "Mục đích của việc viết lách không phải là viết cho xong bài, mà để nâng cao hiểu biết của chính bạn và của những người xung quanh. Việc khoán toàn bộ việc viết lách cho AI giống như bạn bỏ tiền thuê người khác đi tập gym hộ bạn vậy."
> 
> -- 《Đừng để AI viết hộ bạn》

4、

> "Công việc của lập trình viên không phải là viết code, mà là thông qua các mức độ trừu tượng để quản lý độ phức tạp của phần mềm. Nếu bạn làm tốt khâu quản lý đó, việc viết code sẽ trở nên cực kỳ đơn giản."
> 
> -- 《Công việc của bạn không phải là lập trình》

## 往年回顾 (Nhìn lại các năm trước)

[Sản xuất công nghiệp đang dần chuyển dịch sang mô hình "kinh tế gig"](https://www.ruanyifeng.com/blog/2025/04/weekly-issue-344.html)（#344）

[Cảm tưởng về trận hải chiến Nhai Môn](https://www.ruanyifeng.com/blog/2024/03/weekly-issue-294.html)（#294）

[Kỷ nguyên Big Data đã kết thúc](https://www.ruanyifeng.com/blog/2023/03/weekly-issue-244.html)（#244）

[Kẻ bi quan thường đúng, người lạc quan thường thành công](https://www.ruanyifeng.com/blog/2022/02/weekly-issue-194.html)（#194）

(Hết)
