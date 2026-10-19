# Tuần san #413: Tạm biệt React Native

> **Tên gốc:** 科技爱好者周刊（第 413 期）：再见了，React Native  
> **Tác giả:** 阮一峰 · **Ngày:** 18/09/2026 · **Tổng hợp:** 19/10/2026  
> **Nguồn:** https://www.ruanyifeng.com/blog/2026/09/weekly-issue-413.html  
> **Hình thức:** Ghi chú đọc và phân tích bằng tiếng Việt, không phải bản dịch nguyên văn.

## Mục lục

1. Tổng quan
2. Vì sao Shopify rời React Native?
3. Bản đồ Mercator và Equal Earth
4. Tin công nghệ, bài đọc và công cụ
5. Tài nguyên, hình ảnh và câu nói
6. Góc nhìn AI và kết luận

## 1. Tổng quan

Chủ đề trung tâm là quyết định của Shopify chuyển ứng dụng di động từ React Native trở về Swift và Kotlin. Tác giả dùng ví dụ này để lập luận rằng AI làm chi phí viết lại mã giữa các nền tảng giảm, từ đó thay đổi lợi ích của một số lớp trừu tượng. Chủ đề thứ hai là cách phép chiếu bản đồ ảnh hưởng đến cách nhìn về diện tích các quốc gia. Các mục khác giới thiệu công cụ terminal, video, cộng tác, tài nguyên thiết kế và những nhận định về mã do AI tạo.

## 2. Shopify và câu hỏi: còn cần framework đa nền tảng không?

Năm 2020, Shopify từng tuyên bố chuyển mạnh sang React Native. Khi đó ba lợi ích được quảng bá là tránh làm cùng tính năng hai lần, cho phép kỹ sư linh hoạt giữa các nhóm và dành thời gian tiết kiệm được cho giá trị mới. Đằng sau đó còn có yếu tố kinh tế: duy trì một nền tảng phát triển chung có thể giảm nhân sự và công sức đồng bộ giữa iOS và Android.

Trong [thông báo mới](https://shopify.engineering/back-to-native), Shopify chọn trở lại phát triển bản địa bằng Swift và Kotlin. Theo diễn giải của Ruan Yifeng, coding agent làm việc chuyển đổi logic giữa hai ngôn ngữ rẻ hơn, khiến chi phí duy trì hai codebase không còn cao như trước. Nếu vậy, doanh nghiệp có thể ưu tiên hiệu năng, khả năng tích hợp hệ điều hành và trải nghiệm native thay vì tối ưu lượng mã viết tay.

**Cần phân biệt ý kiến và dữ kiện:** quyết định của một công ty không có nghĩa React Native đã hết giá trị trong mọi sản phẩm. Framework đa nền tảng không chỉ giảm số dòng mã: nó còn chia sẻ thành phần UI, mô hình lập trình, thư viện, nhân lực và cách tổ chức nhóm. AI có thể dịch logic, nhưng khác biệt về API nền tảng, accessibility, vòng đời ứng dụng, build, signing và release vẫn phải được xử lý.

Để quyết định có chuyển hay không, cần đo: thời gian phát triển tính năng trên hai nền tảng; hiệu năng startup, scroll, animation; lỗi crash; chi phí tuyển dụng và bảo trì; khả năng kiểm thử đồng nhất. Việc AI viết mã nhanh hơn chỉ làm thay đổi một phần của phương trình tổng chi phí sở hữu.

## 3. Equal Earth: vì sao bản đồ quen thuộc có thể đánh lừa mắt?

Trái Đất gần hình cầu, còn bản đồ là mặt phẳng. Mọi phép chiếu đều phải đánh đổi một số thuộc tính: hình dạng, diện tích, góc hoặc khoảng cách. Mercator rất hữu ích trong hàng hải vì bảo toàn góc cục bộ, nhưng làm phóng đại diện tích vùng vĩ độ cao. Greenland hay các nước phía bắc trông lớn hơn tương quan thực tế.

Tuần san bàn đến phép chiếu Equal Earth, được thiết kế để thể hiện diện tích tương đối tốt hơn và tạo hình dáng thế giới dễ nhìn. Ý nghĩa không chỉ là kỹ thuật bản đồ: lựa chọn cách trực quan hóa ảnh hưởng tới trực giác chính trị và địa lý của người xem.

Bài có nhắc thông tin về một cuộc bỏ phiếu liên quan đến việc từ bỏ Mercator; không nên hiểu là tất cả bản đồ Mercator bị cấm. Từng mục đích vẫn cần phép chiếu phù hợp: hàng hải, địa lý học, bản đồ web và thống kê dân số có tiêu chí khác nhau.

## 4. Sáu bài đọc

1. **[Mẫu HTML cá nhân](https://vale.rocks/posts/html-boilerplate)** — Một bộ khung HTML tự xây giúp tác giả hiểu cấu trúc mặc định và tránh lệ thuộc quá nhiều vào boilerplate sinh sẵn.

2. **[Lướt web khi không có CSS](https://css-tricks.com/that-time-i-tried-browsing-the-web-without-css/)** — Thử nghiệm tắt stylesheet để thấy vai trò của HTML ngữ nghĩa và khả năng truy cập.

3. **[Công cụ quản lý container và reverse proxy](https://web.archive.org/web/20250401115923/https://kiranet.org/posts/self-hosting-like-its-2025/)** — Giới thiệu các công cụ giúp tự lưu trữ dịch vụ với cấu hình container và proxy.

4. **[Những điểm kỳ lạ của JavaScript](https://stack-auth.com/blog/on-javascripts-weirdness)** — Các hành vi không trực giác của ngôn ngữ nhắc lập trình viên chú ý chuyển kiểu và quy tắc runtime.

5. **[Tham số udm của Google Search](https://serpapi.com/blog/every-google-udm-in-the-world/)** — Tìm hiểu các biến thể giao diện và bộ lọc tìm kiếm được kích hoạt bằng tham số URL.

6. **[Giải thích entropy bằng ví dụ](https://www.engineersedge.com/thermodynamics/entropy_explained_with_sheep_15961.htm)** — Bài diễn giải khái niệm entropy trong nhiệt động lực học theo cách trực quan.

**Góc nhìn chung:** các bài trải từ HTML/CSS và JavaScript đến hạ tầng self-host và kiến thức nền. Chúng nhắc rằng AI có thể tạo giao diện nhanh nhưng người phát triển vẫn cần hiểu HTML ngữ nghĩa, các hành vi runtime và giao thức hạ tầng để kiểm tra đầu ra.

## 5. Mười công cụ

1. **[Great Tables](https://github.com/posit-dev/great-tables)** — Tạo bảng trình bày đẹp từ dữ liệu, phục vụ báo cáo.

2. **[ghostty-web](https://github.com/coder/ghostty-web)** — Thành phần terminal trên web dựa trên công nghệ của Ghostty.

3. **[Infat](https://github.com/philocalyst/infat)** — Công cụ được giới thiệu trong tuần san; cần xem tài liệu dự án để đánh giá chi tiết.

4. **[mini-img-editor](https://github.com/xdadda/mini-photo-editor)** — Chỉnh sửa ảnh gọn nhẹ.

5. **[CryptPad](https://cryptpad.fr/)** — Bộ công cụ cộng tác trực tuyến tập trung vào bảo mật và mã hóa.

6. **[Lyrimuse](https://github.com/Yudaotor/lyrimuse)** — Công cụ âm nhạc/lời bài hát.

7. **[capcut-cli](https://github.com/renezander030/capcut-cli)** — Điều khiển các tác vụ biên tập video CapCut qua dòng lệnh.

8. **[mailez](https://github.com/mailez-hq/mailez)** — Công cụ hỗ trợ workflow email.

9. **[Status Trio](https://github.com/lingyired/status-trio)** — Hiển thị hoặc theo dõi trạng thái hệ thống.

10. **[Polycompiler](https://github.com/EvanZhouDev/polycompiler)** — Thử nghiệm liên quan đến biên dịch/chuyển đổi nhiều ngôn ngữ.

**Đánh giá thực dụng:** ghostty-web phù hợp nếu xây terminal trong trình duyệt; capcut-cli đáng chú ý cho pipeline tạo video; CryptPad hữu ích khi cộng tác với dữ liệu nhạy cảm. Với các dự án nhỏ hoặc mới, nên kiểm tra lịch sử commit, giấy phép và tình trạng duy trì thay vì suy đoán độ trưởng thành từ ảnh demo.

## 6. Bốn tài nguyên

1. **[gpcb.net](https://gpcb.net/net/)** — Tài nguyên trực tuyến về mạng máy tính.

2. **[Từ điển phong cách thị giác](https://visualstyles.jerrymakes.com/)** — Kho tham khảo phong cách thiết kế hình ảnh.

3. **[Kiểm tra IP cho AI](https://store.xiu.ai/zh/ai-ip/)** — Công cụ đánh giá IP/địa chỉ mạng cho truy cập dịch vụ AI.

4. **[Gravity](https://qunabu.github.io/Gravity/#what-is-gravity)** — Trang trực quan hóa kiến thức về trọng lực.

## 7. Hình ảnh và câu nói đáng nhớ

Tuần san có những hình ảnh và nhận xét về cách công nghệ định hình cách chúng ta nhìn thế giới. Các trích đoạn bàn về hiện tượng “slop lasagna”: mã bên trong từng module có thể không đẹp, nhưng nếu các module có ranh giới và hợp đồng rõ, hệ thống vẫn có thể thay thế từng phần tương đối dễ dàng. Đây là một nhận xét có giá trị trong thời AI sinh mã.

Một ý tưởng khác là hình ảnh “thời đại của các phù thủy”: con người dùng hệ thống mạnh mà không hiểu hết bên trong, nên phải dựa nhiều hơn vào thực nghiệm và kiểm chứng. Cách diễn giải này không nên hiểu rằng kiến thức kỹ thuật không còn cần thiết; trái lại, cần hiểu đủ để biết nên kiểm tra điều gì.

## 8. AI thay đổi giá trị của lớp trừu tượng ra sao?

Trước AI, một framework thường mang giá trị rõ ràng vì tiết kiệm công viết mã. Khi AI giảm chi phí sinh mã, giá trị ấy có thể giảm tương đối. Nhưng những trừu tượng thật sự có ích còn giúp giảm độ phức tạp nhận thức, quản lý trạng thái, giảm khác biệt nền tảng và duy trì tiêu chuẩn chất lượng. Chúng không biến mất chỉ vì mã rẻ hơn.

Ví dụ trong một ứng dụng Go, AI có thể viết CRUD rất nhanh; điều đó không làm cho ranh giới transaction, kiểm soát truy cập, schema migration và quan sát lỗi trở nên vô nghĩa. Những thứ khó vẫn là tính đúng, nhất quán và khả năng vận hành.

**Ba hành động sau khi đọc:** (1) đánh giá framework theo chi phí vận hành thay vì số dòng mã; (2) đặt contract và test quanh module để AI có thể sửa từng phần an toàn; (3) đo hiệu năng và trải nghiệm trên thiết bị thực trước khi quyết định viết lại.

**Kết luận:** React Native là ví dụ để thảo luận một thay đổi kinh tế sâu hơn: AI làm việc chuyển đổi mã rẻ đi, nhưng không xóa chi phí phối hợp và trách nhiệm kỹ thuật. Một kiến trúc tốt phải tiếp tục chứng minh giá trị ở những thứ khó kiểm chứng và khó thay thế.

---
*Đối chiếu: [Markdown gốc #413](https://github.com/ruanyf/weekly/blob/master/docs/issue-413.md).*
