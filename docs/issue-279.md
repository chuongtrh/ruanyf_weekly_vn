# Bản tin chia sẻ công nghệ (Số 279): Bi kịch của cộng đồng trực tuyến

Ghi lại những nội dung công nghệ đáng chia sẻ trong tuần qua，phát hành vào thứ Sáu hàng tuần.

Bản tin này là mã nguồn mở (GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly))，hoan nghênh gửi issue，đóng góp hoặc giới thiệu dự án của bạn.

Bài đăng [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/3599) trong khu vực thảo luận của bản tin cung cấp nhiều thông tin lập trình viên việc làm，hoan nghênh truy cập hoặc đăng tin tuyển dụng/thực tập.

## 封面图

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112007.webp)

Hai chủ cửa hàng sách cũ ở Shizuoka, Nhật Bản, mỗi thứ Ba hàng tuần kéo chiếc xe chứa tới 300 kg sách cũ đi quanh khu phố để người dân tiện mua. Điều này gần như là một tác phẩm nghệ thuật hành vi: mang theo một xe tri thức, nặng nề tiến bước để tìm kiếm người mua. (Nguồn: [NHK Shizuoka](https://www.nhk.or.jp/shizuoka/lreport/article/004/19/?fbclid=IwAR3TZwrGaafrpbA2wz0cwlTPurPb0Ti_xV88Zf15Z9cIFAal5L-1RB1zFqo))

## 网络社区的悲剧

Trong nửa đầu năm nay, diễn đàn trực tuyến nổi tiếng của Trung Quốc là "Tianya Club" (Thiên Nhai) đã chính thức thông báo đóng cửa.

Vào thời điểm đó, sau khi xem tin tức, tôi rất muốn viết một bài phân tích với chủ đề: **Tại sao các cộng đồng trực tuyến lại không thể duy trì lâu dài?**

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111805.webp)

Suốt nhiều năm qua, tôi đã chứng kiến vô số diễn đàn và cộng đồng trực tuyến lần lượt đóng cửa, bao gồm cả diễn đàn do chính tôi tự dựng lên từ những ngày đầu. Hầu như không có cộng đồng nào có thể duy trì sự thịnh vượng lâu dài.

Cũng không có bất kỳ ông lớn công nghệ nào coi mảng cộng đồng trực tuyến làm mảng kinh doanh cốt lõi của mình. Tieba của Baidu là cộng đồng trực tuyến lớn nhất Trung Quốc, nhưng tình hình hiện tại rất ảm đạm và chỉ được coi là một mảng kinh doanh "bỏ thì thương, vương thì tội".

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111804.webp)

Do đó, tôi luôn giữ quan điểm rằng: **Mô hình cộng đồng trực tuyến có những lỗ hổng cố hữu, tốt nhất là không nên tham gia**. Tuy nhiên vào thời điểm đó, tôi chưa có đủ luận cứ thuyết phục nên chưa viết bài.

Cách đây hai ngày, tôi tình cờ đọc được bài viết của một tác giả nước ngoài có quan điểm hoàn toàn trùng khớp với tôi. Anh ấy chỉ ra rằng **tử huyệt của các cộng đồng trực tuyến chính là mô hình "Cộng đồng chuyên gia" (Expert Communities)**, và bất kỳ cộng đồng nào hoạt động theo mô hình này đều chắc chắn sẽ đi đến hồi kết.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112008.webp)

Cái gọi là "Cộng đồng chuyên gia" nghĩa là cộng đồng đó phụ thuộc hoàn toàn vào một nhóm nhỏ người dùng cốt lõi (chuyên gia). Do đó, một khi những người này rời đi hoặc không còn muốn phát biểu, lượng tương tác và độ thảo luận của cộng đồng sẽ lập tức lao dốc và đi đến suy thoái.

Tác giả đó chỉ ra rằng hầu hết các cộng đồng trực tuyến đều hoạt động theo mô hình này, và đều trải qua 5 giai đoạn phát triển trước khi đi đến hồi kết. Tôi thấy phần mô tả của anh ấy cực kỳ sắc sảo, xin chia sẻ lại để mọi người cùng suy ngẫm.

> **Giai đoạn 1: Giai đoạn hình thành và tăng trưởng**.
> 
> Sở thích và mối quan tâm chung đã kết nối một nhóm nhỏ người dùng lại với nhau. Mọi người đều tràn đầy nhiệt huyết, tích cực trao đổi ý kiến và chia sẻ kiến thức trên mạng. Những thành viên mới luôn được chào đón nồng nhiệt và nhận được sự hướng dẫn tận tình.

> **Giai đoạn 2: Giai đoạn phổ biến rộng rãi**.
> 
> Lượng thành viên mới gia nhập cộng đồng tăng trưởng nhanh chóng. Họ liên tục đưa ra những câu hỏi sơ đẳng giống hệt nhau. Các thành viên cũ phải liên tục trả lời những câu hỏi lặp đi lặp lại này, dẫn đến cảm giác mệt mỏi và nhàm chán. Một số người bắt đầu rời bỏ cộng đồng.

> **Giai đoạn 3: Giai đoạn thiết lập quy chuẩn**.
> 
> Để tránh chất lượng thảo luận bị đi xuống, các thành viên cũ bắt đầu xây dựng một bộ quy tắc cộng đồng chi tiết và danh sách câu hỏi thường gặp (FAQ) dài dằng dặc.
>
> Tuy nhiên, các thành viên mới hầu như không bao giờ đọc chúng một cách nghiêm túc, thậm chí một số người còn cho rằng các quy tắc này rất phiền phức hoặc khó hiểu. Kết quả là các xung đột nội bộ bắt đầu nảy sinh, những người quản trị cốt lõi ngày càng ít dung thứ cho những ý kiến trái chiều, những người bất đồng quan điểm thường bị trục xuất và cộng đồng bắt đầu rạn nứt.

> **Giai đoạn 4: Giai đoạn thoái trào**.
> 
> Lượng thành viên mới bắt đầu sụt giảm, cộng đồng trở nên thưa thớt dần. Những chủ đề thảo luận sôi nổi ngày càng hiếm hoi, và các thành viên gắn bó lâu năm cũng bắt đầu rời đi.

> **Giai đoạn 5: Giai đoạn kết thúc**.
> 
> Cộng đồng rơi vào trạng thái trì trệ hoàn toàn. Cả thành viên mới và nội dung mới đều ngừng phát triển, giao diện và nền tảng phần mềm sử dụng cũng trở nên lỗi thời. Cuối cùng, chỉ còn lại một vài thành viên cũ quen biết nhau từ lâu thỉnh thoảng vào trò chuyện, chia sẻ vài câu chuyện phiếm về cuộc sống thường ngày.

Mọi người có đồng tình với 5 giai đoạn phát triển nêu trên không?

Bản thân tôi vô cùng đồng cảm vì đã từng trải qua nhiều lần. Những diễn đàn trực tuyến từng một thời làm mưa làm gió tại Trung Quốc như Tianya Club, Paowang, Kaidi Club... đều đã suy tàn theo đúng lộ trình này.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112304.webp)

Vào tháng 5 năm nay, sau khi Tianya Club đóng cửa, đã có nhóm cựu quản trị viên đứng ra tổ chức chiến dịch livestream gây quỹ với mục tiêu quyên góp 3 triệu Nhân dân tệ để hồi sinh diễn đàn này, nhưng kết quả thu về gần như bằng không.

Thực tế là ngay cả khi quyên góp đủ tiền, diễn đàn Thiên Nhai cũng không thể quay lại như xưa. Mô hình "Cộng đồng chuyên gia" phụ thuộc vào nhóm nhỏ người dùng cốt lõi là không thể cứu vãn, sự lụi tàn là điều tất yếu.

Tôi viết về chủ đề này hôm nay nhằm đưa ra lời khuyên cho mọi người: **Tốt nhất là không nên xây dựng các mô hình cộng đồng trực tuyến, bao gồm cả diễn đàn, nhóm chat người hâm mộ, trang hỏi đáp...** Mô hình của chúng có những khuyết tật bẩm sinh khó khắc phục.

Trong vài năm qua, có rất nhiều bạn đọc hỏi tôi liệu bản tin tuần này có nhóm giao lưu độc giả nào không. Tôi luôn trả lời là không, lý do chính là như vậy. Nếu không thể duy trì sự đầu tư nhân lực liên tục để quản lý, các nhóm này cuối cùng cũng chỉ biến thành các nhóm chat phiếm vô thưởng vô phạt, vậy thì thà không tạo ra còn hơn.

Để một cộng đồng trực tuyến duy trì được sự thành công, cách duy nhất là phải luôn có lượng thành viên mới tham gia ổn định, sẵn sàng ở lại và tiếp quản vai trò của các thành viên cũ. Cơ chế tự động cập nhật nhân sự này, ngoài các diễn đàn BBS của các trường đại học ra, thực sự cực kỳ khó thực hiện ở các cộng đồng xã hội.

## 科技动态

1、[Rơi mất kính cửa sổ máy bay khi đang bay](https://www.flightradar24.com/blog/aaib-says-film-lights-caused-window-damage-on-titan-a321neo/)

Trên một chuyến bay tại Anh, sau khi máy bay cất cánh lên cao, phi hành đoàn kinh hoàng phát hiện ra hai ô kính cửa sổ cabin đã biến mất tự bao giờ, tạo thành hai chiếc lỗ lớn trên thân máy bay. Máy bay buộc phải quay đầu hạ cánh khẩn cấp.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111702.webp)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111703.webp)

Kết quả điều tra sau đó chỉ ra rằng, vào ngày hôm trước, chiếc máy bay này được thuê để quay một bộ phim. Khi đỗ trên sân đỗ, hệ thống đèn chiếu sáng công suất lớn của đoàn phim đã rọi trực tiếp vào cửa sổ máy bay trong thời gian dài. Nhiệt độ cực cao tỏa ra đã làm nóng chảy lớp keo niêm phong cửa sổ, dẫn đến việc kính cửa sổ bị rơi ra khi bay.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111704.webp)

Ảnh dưới đây là ô cửa sổ bên cạnh, có thể thấy rõ lớp bọt niêm phong đã bị nóng chảy biến dạng, nhưng may mắn là tấm kính vẫn chưa bị rơi ra.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111701.webp)

Sự cố này là lời cảnh báo về những rủi ro an toàn nghiêm trọng khi máy bay phải tiếp xúc với nguồn nhiệt cực cao ngoài đời thực.

2、[Bang Oregon bãi bỏ kỳ thi sát hạch luật sư](https://www.reuters.com/legal/government/no-bar-exam-required-practice-law-oregon-starting-next-year-2023-11-07/)

Bang Oregon (Mỹ) thông báo kể từ tháng 5 năm 2024, những người muốn hành nghề luật sư tại bang này sẽ không cần phải tham gia kỳ thi sát hạch tư pháp (Bar Exam).

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111014.webp)

Thay vào đó, các sinh viên tốt nghiệp trường luật chỉ cần hoàn thành 675 giờ làm việc thực tế tại các văn phòng luật sư và có các sản phẩm hồ sơ pháp lý thực tế do chính mình thực hiện là sẽ được cấp chứng chỉ hành nghề.

Quy trình này về cơ bản tương đồng với ngành lập trình. Lập trình viên không cần thi sát hạch để lấy chứng chỉ hành nghề, chỉ cần bạn có kinh nghiệm viết code và có các dự án thực tế chứng minh năng lực là mọi người sẽ công nhận bạn là lập trình viên.

Vậy tại sao ngành luật lại bắt buộc phải có kỳ thi sát hạch? Kinh nghiệm và hồ sơ làm việc thực tế rõ ràng là phương pháp chứng thực năng lực tốt hơn nhiều.

3、[Gia tăng độ tuổi nghỉ hưu của phi công Mỹ](https://www.flyingmag.com/house-committee-votes-to-push-back-pilot-retirement-age-2-years/)

Trước tình trạng thiếu hụt phi công trầm trọng trên các chuyến bay thương mại, chính phủ Mỹ đã buộc phải nâng độ tuổi nghỉ hưu của phi công từ 65 tuổi lên 67 tuổi.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061901.webp)

Sau này khi bay ở Mỹ, nếu bạn thấy một phi công tóc bạc trắng điều khiển máy bay thì cũng không cần quá ngạc nhiên. Vào năm 2007, tuổi nghỉ hưu của phi công Mỹ đã được nâng từ 60 lên 65 tuổi, nhưng tình hình thiếu hụt vẫn không được cải thiện buộc họ phải tiếp tục lùi thời hạn này.

Đáng chú ý là luật cấp bằng lái xe thông thường tại Mỹ không quy định giới hạn độ tuổi tối đa. Người dân ở bất kỳ độ tuổi nào cũng được phép lái xe, chỉ yêu cầu những người trên 80 tuổi phải thực hiện kiểm tra thị lực định kỳ.

4、[Dự án phóng tên lửa bằng đại bác khổng lồ](https://newatlas.com/space/longshot-kinetic-launch/)

Công ty khởi nghiệp Longshot của Mỹ đang nghiên cứu hiện thực hóa một công nghệ tưởng chừng như chỉ có trong các cuốn tiểu thuyết viễn tưởng thế kỷ 19: Dùng đại bác để bắn tên lửa vào không gian.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080506.webp)

Họ dự kiến sẽ xây dựng một đường ống đại bác bằng bê tông dài tới 9,65 km để bắn các dòng tên lửa cỡ nhỏ vào không gian giống như bắn đạn đại bác.

Nguyên lý hoạt động là nén lượng khí sinh ra từ các vụ nổ trong lòng ống đại bác để tạo lực đẩy. Quá trình phóng sẽ có nhiều vụ nổ liên tục để gia tốc cho tên lửa. Công ty cho biết thiết bị có thể giúp tên lửa đạt tốc độ Mach 30 chỉ trong vòng 1 giây. Ảnh dưới là mô hình thử nghiệm của dự án trong phòng thí nghiệm.

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023080505.webp)

Ưu điểm lớn nhất của phương pháp này là chi phí cực kỳ rẻ, với mục tiêu dài hạn là chỉ khoảng 10 USD cho mỗi kg tải trọng phóng. Tuy nhiên, rào cản lớn là với kích thước khổng lồ như vậy, rất khó để dựng cao họng pháo hướng lên trời, do đó pháo có thể chỉ bắn được theo phương ngang, đồng nghĩa với việc họng pháo bắt buộc phải hướng ra phía biển lớn hoặc sa mạc không người.

## Bài viết

1\. [Phân tích chi tiết sự cố phóng thử nghiệm lần thứ hai của siêu tên lửa Starship](https://mp.weixin.qq.com/s/N1akMdMZrolD-DzikHnY_Q)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112104.webp)

Tuần trước, tàu vũ trụ Starship của SpaceX đã thực hiện chuyến bay thử nghiệm quỹ đạo lần thứ hai và đã phát nổ trên không trung. Đội ngũ chuyên gia Trung Quốc đã viết một bài phân tích dài hơn vạn chữ về sự cố phóng này.

2\. [Bài phỏng vấn Sam Altman trên tạp chí "Doanh nhân Trung Quốc"](https://weibo.com/ttarticle/x/m/show/id/2309404969066262823141)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112002.webp)

Vài ngày trước khi bị hội đồng quản trị OpenAI sa thải, Sam Altman đã có buổi phỏng vấn trực tiếp với tạp chí Doanh nhân Trung Quốc, tuy nhiên các nội dung chia sẻ tương đối phổ thông. (Đóng góp của [@Lyeragain](https://github.com/ruanyf/weekly/issues/3643))

3\. [Hướng dẫn nhập môn sử dụng ChatGPT hiệu quả](https://blog.warmplace.cn/post/chatgpt)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112302.webp)

Dựa trên kinh nghiệm sử dụng thực tế của bản thân, tác giả hướng dẫn chi tiết quy trình đăng ký, kích hoạt tài khoản cũng như các mẹo sử dụng và nguyên lý hoạt động của ChatGPT. (Đóng góp của [@guojingwen](https://github.com/ruanyf/weekly/issues/3656))

4\. [Tìm hiểu về đường ống có đặt tên (Named Pipes) trong Linux](https://goodyduru.github.io/os/2023/09/26/ipc-named-pipes.html)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202310/bg2023101001.webp)

Nằm trong chuỗi bài viết giới thiệu về cơ chế giao tiếp liên tiến trình (IPC) trong Linux, bài viết này là tài liệu hướng dẫn cơ bản giới thiệu khái niệm Named Pipes một cách rất ngắn gọn và trực quan. Bạn đọc cũng có thể tham khảo thêm các bài viết cùng chuyên đề như [Tìm hiểu về Sockets](https://goodyduru.github.io/os/2023/10/03/ipc-unix-domain-sockets.html) và [Tìm hiểu về Unix Signals](https://goodyduru.github.io/os/2023/10/05/ipc-unix-signals.html).

5\. [Lỗ hổng bảo mật của thuộc tính target="_blank" trên thẻ link](https://blog.bolajiayodeji.com/the-security-vulnerabilities-of-the-target-blank-attribute)（Tiếng Trung）

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023083003.webp)

Một bài viết phân tích kỹ thuật giới thiệu rủi ro bảo mật khi sử dụng thuộc tính `target="_blank"` trên thẻ liên kết `<a>`. Thuộc tính này cho phép trang web mới mở có quyền tham chiếu ngược lại trang web gốc, tiềm ẩn nguy cơ bị tấn công giả mạo.

6\. [Xử lý hiệu ứng phối cảnh cho ảnh chụp từ trên cao](https://leifgehrmann.com/2021/09/05/photogrammetry-on-a-plane/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023083101.webp)

Tác giả hướng dẫn một phương pháp đơn giản để xử lý ảnh chụp từ máy bay, giúp căn chỉnh hình ảnh khớp với bản đồ thực tế thông qua việc hiệu chỉnh hình thang.

7\. [Chia sẻ trải nghiệm thực tế với React Server Components (RSC)](https://www.mux.com/blog/what-are-react-server-components)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202308/bg2023083113.webp)

Thư viện React ban đầu sử dụng cơ chế dựng hình phía client (CSR), sau đó bổ sung thêm dựng hình phía server (SSR) và hiện tại đang tập trung thúc đẩy mô hình React Server Components (RSC).

Tác giả chia sẻ những kinh nghiệm thực tế của bản thân sau khi chuyển đổi dự án sang sử dụng RSC, đi kèm với đó là các lời khuyên hữu ích cho lập trình viên.

8\. [Công cụ curl bổ sung hỗ trợ giao thức IPFS](https://daniel.haxx.se/blog/2022/08/10/ipfs-and-their-gateways/)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092503.webp)

Công cụ dòng lệnh kinh điển `curl` gần đây đã bổ sung tính năng tải dữ liệu từ giao thức IPFS. Bài viết phân tích các khía cạnh kỹ thuật của quyết định này, chi tiết cách dùng có thể xem thêm tại [tài liệu hướng dẫn](https://github.com/curl/curl/blob/master/docs/IPFS.md).

## 翻译软件

Chuyên mục tuần này giới thiệu một số phần mềm hỗ trợ dịch thuật hữu ích:

1、[Easydict](https://github.com/tisfeng/Easydict)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112210.webp)

Ứng dụng mã nguồn mở trên hệ điều hành macOS hỗ trợ tra từ điển và dịch thuật văn bản. Phần mềm tích hợp tính năng dịch nhanh đoạn văn bản đang chọn và nhận diện chữ từ ảnh chụp màn hình (OCR), cho phép tích hợp nhiều nguồn từ điển khác nhau. (Đóng góp của [@tisfeng](https://github.com/ruanyf/weekly/issues/3648))

2、[KISS Translator (Dịch thuật tối giản)](https://github.com/fishjar/kiss-translator)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112208.webp)

Tiện ích mở rộng trên trình duyệt web hỗ trợ dịch song ngữ song song trực tiếp trên giao diện trang web. (Đóng góp của [@fishjar](https://github.com/ruanyf/weekly/issues/3651))

3、[Pot (Translator of Pylogmon)](https://github.com/pot-app/pot-desktop)

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060201.webp)

Phần mềm dịch thuật đa nền tảng mã nguồn mở, cho phép bôi đen văn bản để dịch nhanh và hỗ trợ cấu hình nhiều API dịch thuật khác nhau.

4、[Baicizhan Helper (Trợ lý từ vựng)](https://github.com/marmot-z/baicizhan-helper)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112301.webp)

Tiện ích mở rộng Chrome hỗ trợ tra từ và lưu từ vựng trực tiếp trên web, có thể đồng bộ với ứng dụng học từ vựng Baicizhan để xây dựng sổ từ tay cá nhân. (Đóng góp của [@marmot-z](https://github.com/ruanyf/weekly/issues/3655))

## 工具

1、[vectorious](https://github.com/mateogianolio/vectorious)

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023060303.webp)

Thư viện JavaScript hiệu năng cao chuyên dùng để xử lý các phép toán ma trận.

2、[EpubPress](https://github.com/sunxen/EpubPressX)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112001.webp)

Tiện ích mở rộng trên trình duyệt Chrome giúp gộp nhiều tab trang web đang mở thành một cuốn sách điện tử định dạng EPUB để đọc ngoại tuyến. (Đóng góp của [@sunxen](https://github.com/ruanyf/weekly/issues/3642))

3、[Công cụ nhân bản giọng nói Clone Voice](https://github.com/jianchang512/clone-voice)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112209.webp)

Dự án mã nguồn mở hỗ trợ trích xuất âm sắc từ file âm thanh mẫu, từ đó chuyển đổi một đoạn văn bản hoặc file âm thanh khác thành giọng nói của người mẫu, tương đương với việc sao chép giọng nói của người khác.

Công cụ hỗ trợ dịch thuật qua lại giữa 4 ngôn ngữ: tiếng Trung, tiếng Anh, tiếng Nhật và tiếng Hàn, đi kèm tính năng ghi âm trực tiếp từ micro. (Đóng góp của [@jianchang512](https://github.com/ruanyf/weekly/issues/3652))

4、[Elog](https://github.com/LetTTGACO/elog)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112003.webp)

Công cụ hỗ trợ đồng bộ nội dung bài viết từ các nền tảng soạn thảo (Yuque, Feishu, Notion, FlowUs) để tự động đăng tải lên các trang blog cá nhân (Hexo, Vitepress, Confluence, WordPress). (Đóng góp của [@LetTTGACO](https://github.com/ruanyf/weekly/issues/3644))

5、[ConfigCenterComparer](https://github.com/hxz393/ConfigCenterComparer)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112004.webp)

Ứng dụng hỗ trợ so sánh dữ liệu cấu hình giữa các trung tâm cấu hình (Config Centers) khác nhau, hiện chỉ hỗ trợ nền tảng Windows. (Đóng góp của [@hxz393](https://github.com/ruanyf/weekly/issues/3645))

6、[GPTs URL](https://github.com/CH563/gtps-url)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112207.webp)

Dự án mã nguồn mở xây dựng trang web danh mục và phân loại các tài nguyên trực tuyến dựa trên framework Astro. Xem bản [Demo tại đây](https://www.gptsurl.com/). (Đóng góp của [@CH563](https://github.com/ruanyf/weekly/issues/3646))

7、[PPz's chrome filter](https://github.com/ppz-pro/chrome-filter)

Tiện ích mở rộng Chrome siêu tối giản giúp chuyển đổi giao diện trang web sang chế độ tối (Dark Mode), mã nguồn chỉ gồm đúng 11 dòng JavaScript, rất thích hợp làm ví dụ học viết extension. (Đóng góp của [@daGaiGuanYu](https://github.com/ruanyf/weekly/issues/3654))

## 资源

1、[Tài liệu hướng dẫn sử dụng Deno toàn tập](https://medium.com/deno-the-complete-reference/an-ultimate-guide-to-deno-bc02535754f0)（Tiếng Anh）

![](https://cdn.beekka.com/blogimg/asset/202309/bg2023092601.webp)

Chuỗi bài viết chi tiết giới thiệu cách sử dụng Deno từ cơ bản đến nâng cao với số lượng hàng chục bài viết.

2、[VAVE BG](https://vavebg.com/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112101.webp)

Trang web chia sẻ các hình nền nghệ thuật chất lượng cao được tạo hoàn toàn bằng công nghệ AI.

3、[Quy chuẩn viết code của Google](https://google.github.io/styleguide/)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111607.webp)

Tài liệu chính thức quy định các quy chuẩn và phong cách viết code (Style Guide) cho nhiều ngôn ngữ lập trình khác nhau của Google.

4、[Danh sách các bài giảng video xuất sắc nhất](https://news.ycombinator.com/item?id=34591291)

Một chủ đề thảo luận sôi nổi trên diễn đàn Hacker News, nơi mọi người chia sẻ các video bài giảng khoa học và công nghệ hay nhất mà họ từng xem (tiếng Anh).

## 图片

1、[Vẻ đẹp của các hồ bơi trong nhà tại Berlin](https://www.bbc.com/travel/article/20231116-the-hidden-beauty-of-berlins-indoor-pools)

Thành phố Berlin (Đức) có truyền thống xây dựng các hồ bơi công cộng trong nhà với kiến trúc vô cùng lộng lẫy.

Hiện nay, Berlin sở hữu hơn 60 hồ bơi công cộng trong nhà với thiết kế tráng lệ, tạo cho người dân cảm giác như đang được bơi lội bên trong các cung điện cổ kính.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111901.webp)

Hàng năm, hệ thống hồ bơi này thu hút hơn 6 triệu lượt khách ghé thăm. Nhiều cuốn sách hướng dẫn du lịch thậm chí còn dành riêng một chương để giới thiệu về các hồ bơi độc đáo này.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111902.webp)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111903.webp)

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023111904.webp)

2、[Bản đồ nổi dành cho người khiếm thị từ năm 1837](https://www.davidrumsey.com/blog/2012/5/21/atlas-for-the-blind-1837)

Vào năm 1837, một cuốn bản đồ thế giới dành riêng cho người khiếm thị đã được xuất bản tại Mỹ với toàn bộ các đường nét địa hình được in nổi.

Cuốn sách giúp chúng ta thấu hiểu phần nào những khó khăn của người khiếm thị khi muốn hình dung và học tập về bản đồ địa lý thời kỳ trước.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061406.webp)

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061407.webp)

Phần văn bản giải thích cũng được in nổi.

![](https://cdn.beekka.com/blogimg/asset/202306/bg2023061408.webp)

Tuy nhiên, hệ chữ nổi được sử dụng trong cuốn sách này không phải là hệ thống chữ nổi Braille 6 chấm phổ biến hiện nay. Hệ thống chữ nổi Braille được phát minh tại Pháp từ năm 1824 nhưng chưa được nước Mỹ chấp nhận vào thời điểm đó. Các nghiên cứu sau này đều chứng minh chữ Braille thân thiện và dễ đọc hơn nhiều so với hệ chữ in nổi mô phỏng chữ cái thông thường này.

## ✍️ Bài đọc thêm

### Bàn về thói quen viết tài liệu trong các công ty khởi nghiệp

Văn hóa họp hành liên miên gây tổn hại lớn đến năng suất của doanh nghiệp, đặc biệt các công ty khởi nghiệp nên triệt để hạn chế các cuộc họp không cần thiết.

![](https://cdn.beekka.com/blogimg/asset/202311/bg2023112303.webp)

**Các công ty khởi nghiệp nên họp ít đi và viết tài liệu nhiều hơn**. Ưu tiên hàng đầu là viết tài liệu, họp hành chỉ là phương án thứ hai.

(1) Trong môi trường khởi nghiệp nơi thời gian là vàng bạc, các cuộc họp cực kỳ lãng phí thời gian. Tất nhiên không phải mọi cuộc họp đều vô dụng, nhưng về mặt nguyên tắc, doanh nghiệp nên cố gắng giảm thiểu số lượng cuộc họp và tinh giản tối đa thành phần tham dự.

(2) Tình trạng họp hành liên tục là biểu hiện của một vấn đề sâu sắc hơn: Sự thiếu hụt các tài liệu hướng dẫn rõ ràng, dễ tiếp cận và đáng tin cậy.

Nếu mọi quy trình làm việc đều có tài liệu hướng dẫn rõ ràng, bạn sẽ không cần mất cả giờ đồng hồ họp để giải thích công việc. Nếu mọi quyết định đều được ghi chép lại, bạn sẽ không cần triệu tập cả phòng họp chỉ để giải thích lý do đưa ra quyết định đó. Nếu mọi nhóm làm việc đều có tài liệu lưu trữ, bạn sẽ không cần tổ chức các buổi thảo luận nhóm rườm rà mỗi khi có nhân sự mới gia nhập.

(3) Các cuộc họp thường tạo ra ảo giác về năng suất làm việc. Bạn cứ nghĩ họp hành giúp nâng cao hiệu quả, nhưng thực chất nó đang cản trở tiến độ công việc.

Mỗi cuộc họp không cần thiết là một sự lãng phí tài nguyên của doanh nghiệp. Khoảng thời gian đó đáng lẽ nên dành để tối ưu hóa thuật toán sản phẩm, hoặc thậm chí để nhân viên học hỏi thêm kiến thức mới hoặc nghỉ ngơi tái tạo sức lao động. Việc cắt giảm họp hành không chỉ giúp tiết kiệm thời gian, mà quan trọng hơn là giúp mọi người tập trung cao độ để sáng tạo – yếu tố sống còn của một công ty khởi nghiệp.

(4) Các cuộc họp có xu hướng tự động kéo dài ngoài tầm kiểm soát. Ban đầu bạn chỉ lên lịch họp 30 phút để thảo luận nhanh một vấn đề nhỏ. Nhưng trong quá trình họp, một vấn đề phát sinh ngoài dự kiến xuất hiện và cuộc tranh luận có thể kéo dài liên tục tới hai tiếng đồng hồ.

(5) Các cuộc họp rất khó để chốt chính xác các chi tiết kỹ thuật. Những câu nói bộc phát, cách diễn đạt mơ hồ hoặc sự hiểu lầm ý kiến giữa các bên sẽ làm giảm độ rõ ràng của nội dung họp. Cuối cùng, phương án giải quyết triệt để vẫn là phải ghi chép mọi thứ ra văn bản.

(6) **Kết quả cuộc họp thường có xu hướng nghiêng về ý kiến của những người nói to nhất, chứ không hẳn thuộc về những người có ý tưởng xuất sắc nhất**. Điều này vô tình triệt tiêu sự sáng tạo và tính đa dạng trong tư duy tập thể. Ngược lại, tài liệu văn bản mang lại một môi trường bình đẳng, nơi mọi thành viên đều có thể trình bày ý kiến một cách mạch lạc, khuyến khích văn hóa suy nghĩ chín chắn thay vì đưa ra các quyết định vội vã cảm tính.

(7) Kết luận: Thời gian và tài nguyên của doanh nghiệp nên được đầu tư vào việc viết tài liệu lưu trữ thay vì tiêu tốn vào các cuộc họp hành. Hầu hết các cuộc họp đều có thể được thay thế hiệu quả bằng một bản tài liệu dự thảo được chuẩn bị chu đáo, cung cấp đầy đủ số liệu và đề xuất cụ thể để mọi người cùng cho ý kiến phản hồi.

## Lịch sử tuần này

- 2022年（第 232 期）：[Thiết kế đồ họa: Giới thiệu các phần mềm thiết kế và chỉnh sửa giao diện chuyên nghiệp](http://www.ruanyifeng.com/blog/2022/11/weekly-issue-232.html)
- 2021年（第 182 期）：[Chiến lược kinh doanh: Phân tích các rủi ro dài hạn của chính sách ưu đãi dành cho khách hàng mới](http://www.ruanyifeng.com/blog/2021/11/weekly-issue-182.html)
- 2020年（第 132 期）：[Kỹ năng làm việc: So sánh vai trò của năng lực phản ứng nhanh và năng lực tư duy sâu](http://www.ruanyifeng.com/blog/2020/11/weekly-issue-132.html)
- 2019年（第 82 期）：[Lựa chọn nghề nghiệp: Lời khuyên về việc ưu tiên lựa chọn các ngành công nghiệp có tốc độ tăng trưởng nhanh nhất](http://www.ruanyifeng.com/blog/2019/11/weekly-issue-81.html)

## 说明

Tuần báo được phát hành vào thứ Sáu hàng tuần trên [Trang blog cá nhân của tôi](http://www.ruanyifeng.com/blog) và tài liệu WeChat cá nhân. Hoan nghênh bạn đọc đăng ký theo dõi.

Nội dung bản tin được phát hành dưới dạng mã nguồn mở tự do, repository lưu trữ đặt tại GitHub: [ruanyf/weekly](https://github.com/ruanyf/weekly). Mọi đóng góp nội dung xin gửi về mục issue của repo. Ngoài ra bản tin cung cấp kênh thông tin việc làm [《Ai đang tuyển dụng？》](https://github.com/ruanyf/weekly/issues/2827) hỗ trợ tuyển dụng lập trình viên.

Liên hệ hợp tác thương mại hoặc giới thiệu sản phẩm xin gửi email về địa chỉ: `yifeng.ruan@gmail.com`.

## Cảm ơn

Cảm ơn phần mềm quản lý tri thức và cộng tác nhóm **[FlowUs](https://flowus.cn?promotionChannel=GW_RYF_01)** hỗ trợ không gian lưu trữ chuyên mục cho bản tin. Độc giả có thể quét mã QR bên dưới hoặc click vào [Thư mục chuyên mục FlowUs của Bản tin](https://ruanyf-weekly.flowus.cn/?code=FLOWUS&promotionChannel=WX_RYF_00) để xem chi tiết. FlowUs makes knowledge management and team collaboration intuitive and smooth.

![](https://cdn.beekka.com/blogimg/asset/202303/bg2023030205.webp)

（Hết）
