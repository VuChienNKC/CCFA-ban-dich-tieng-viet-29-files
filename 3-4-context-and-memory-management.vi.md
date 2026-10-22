# 3.4 — Quản lý giới hạn ngữ cảnh và bộ nhớ: Bắt đầu lại, tóm tắt, lưu giữ

- **Lĩnh vực (Domain):** 3
- **Nhiệm vụ (Task):** 3.4
- **Tên bài gốc:** Managing Context Limits and Memory: Restart, Summarise, Persist
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/3-product-model-selection/3-4-context-and-memory-management)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Một cuộc trò chuyện có không gian làm việc hữu hạn. Tất cả nội dung đã nói, đính kèm và tạo ra từ đầu đến hiện tại là những gì Claude đang làm việc cùng. Cuộc trò chuyện rất dài sẽ tiến gần giới hạn độ dài và hạn mức sử dụng của nền tảng; cuộc trò chuyện dài hơn cũng tiêu thụ nhiều hạn mức hơn. Tách biệt với điều đó, claude.ai có tính năng ghi nhớ giữa các cuộc trò chuyện. Tìm kiếm cuộc trò chuyện (chat search) là truy xuất được yêu cầu qua prompt, khi bạn nhờ Claude tìm thông tin trong các cuộc trò chuyện trước.

Một người bán rau quả đã lập kế hoạch các hộp rau Giáng sinh của cửa hàng trong một cuộc trò chuyện rất dài từ tháng 8. Cuộc trò chuyện chứa lựa chọn nhà cung cấp, ba phương án hộp đã bị bỏ, danh sách sản phẩm đã thống nhất và bảng giá được sửa nhiều lần.

Khi cuộc trò chuyện chạm giới hạn độ dài, hướng dẫn chính thức là bắt đầu cuộc trò chuyện mới hoặc dùng Project để làm việc với lượng thông tin lớn hơn. Hãy xem nó như một cuộc họp dài: biết rằng nó sẽ kết thúc và quyết định những gì phải được giữ lại sau đó.

## Ba hành động

### 1. Bắt đầu lại (Restart)

Bắt đầu cuộc trò chuyện mới khi một công việc đã hoàn thành, khi chat chứa các hướng đi bế tắc và bản nháp đã bị thay thế hoặc khi gần chạm giới hạn. Một cuộc trò chuyện kéo dài mang theo mọi thứ nó từng nhận, kể cả ba phương án hộp đã bỏ của người bán rau quả. Khởi đầu mới với đúng bối cảnh cần thiết tốt hơn việc tiếp tục mang theo tất cả.

### 2. Tóm tắt (Summarise)

Trước khi rời cuộc trò chuyện, nhờ Claude tóm tắt các quyết định đã đưa ra, trạng thái hiện tại và những việc còn lại. Sau đó tự xác minh bằng cách đối chiếu với hồ sơ nguồn. Bản tóm tắt kế thừa mọi lỗi chưa được sửa trong cuộc trò chuyện mà nó tóm tắt. Người bán rau quả kiểm tra bản của mình bằng email nhà cung cấp và hóa đơn. Bản tóm tắt đã xác minh trở thành bản giao việc mở đầu cho chat mới.

### 3. Lưu giữ và chuyển tiếp (Persist)

Lưu giữ mọi đầu ra làm việc cụ thể mà cuộc trò chuyện tiếp theo sẽ cần. Dán vào chat mới, đính kèm lại tệp hoặc lưu trong kho kiến thức của Project để mọi chat trong Project đều bắt đầu với tài liệu đó. Tài liệu dùng thường xuyên, liên tục được sửa và chia sẻ có nơi lưu thứ tư: artifact, được tinh chỉnh như một phiên bản thống nhất phát triển qua các lần sửa. Người bán rau quả dán danh sách sản phẩm đã thống nhất vào chat mới, tạo bảng giá hằng tuần cho nhân viên thành artifact và lưu danh sách nhà cung cấp trong kho kiến thức Project.

## Bộ nhớ mang theo điều gì và không mang theo điều gì?

Bộ nhớ được xây dựng dưới dạng các chủ đề riêng lẻ: vai trò, dự án, sở thích giao tiếp và bối cảnh công việc đang diễn ra của bạn. Đó là bối cảnh về bạn, không phải bản ghi nguyên cuộc trò chuyện, bản nháp hoặc tài liệu đính kèm. Mỗi Project có bộ nhớ riêng. Bên trong Project, Claude cũng dùng bộ nhớ từ các chat ngoài Project, nhưng không dùng bộ nhớ của Project khác. Vì vậy, tính năng ghi nhớ giúp bạn không phải tự giới thiệu lại. Nó không chuyển dàn ý đã được duyệt hoặc tệp dữ liệu sang chat tiếp theo một cách đáng tin cậy. Chat mới của người bán rau quả có thể biết về cửa hàng, nhưng bảng giá chỉ xuất hiện vì chính cô đã chủ động lưu giữ và chuyển tiếp.

Hai khẳng định lỗi thời sai theo hai hướng ngược nhau: Claude không thể nhớ bất cứ điều gì giữa các chat; và có thể tin bộ nhớ sẽ mang theo tài liệu làm việc. Chủ động lưu giữ và chuyển tiếp vẫn là cách đáng tin cậy đối với một đầu ra làm việc cụ thể.

## Trong bài thi

Mục tiêu này kiểm tra việc lập kế hoạch, không phải xử lý hậu quả sau sự cố; bài thi yêu cầu hiểu chính xác bộ nhớ giữ gì. Hãy chú ý thời điểm được mô tả trong phần dẫn. Câu hỏi lập kế hoạch mô tả cách tổ chức công việc cho giai đoạn tiếp theo: công việc dài sắp chạm giới hạn, dự án bước vào giai đoạn cuối hoặc kế hoạch bàn giao đang được chuẩn bị. Trường hợp người bán rau quả là một ví dụ. Chat đã tạo đầu ra kém và được chẩn đoán sau đó thuộc Lĩnh vực 7. Cùng một cuộc trò chuyện kéo dài có thể xuất hiện trong cả hai loại câu hỏi; đáp án đúng đi theo điều được hỏi. Ở đây, đó là kỷ luật chủ động: có chủ đích bắt đầu lại, tóm tắt kèm xác minh — Lĩnh vực 2 không ngừng áp dụng khi bàn giao — và lưu giữ những gì chat tiếp theo phụ thuộc vào.

Không có nội dung nào trong hướng dẫn chính thức khẳng định sản phẩm suy giảm chất lượng trong chat dài; không đáp án đúng nào dựa vào khẳng định đó. Ngày triển khai và việc tính năng có trên gói nào là thông tin phụ thuộc thời điểm, được đặt trong tài liệu tra cứu nhanh của lĩnh vực này.

### Ảo tưởng về tính liên tục

“Cuộc trò chuyện mới sẽ làm mất toàn bộ bối cảnh của chúng ta” là lý lẽ mạnh nhất để kéo dài chat, nhưng lý lẽ ấy sai. Bản tóm tắt đã xác minh và tài liệu được lưu giữ mang tiếp những bối cảnh đáng giữ với độ dài và mức tiêu thụ hạn mức nhỏ hơn nhiều.

## Những bẫy thường gặp trong bài thi

### Dựa vào bộ nhớ hoặc tìm kiếm chat để chuyển đầu ra làm việc cụ thể sang chat mới

Bộ nhớ lưu bối cảnh về bạn theo các chủ đề riêng lẻ, không lưu nguyên bản ghi, bản nháp hay tệp đính kèm; tìm kiếm chat là truy xuất cần được yêu cầu. Đầu ra mà chat tiếp theo phụ thuộc vào được chuyển bằng hành động chủ động: dán vào, đính kèm lại hoặc lưu trong kho kiến thức Project.

### Dán bản tóm tắt chưa xác minh vào chat mới và coi đó là bàn giao hiệu quả

Bản tóm tắt kế thừa mọi lỗi chưa sửa và quyết định lỗi thời trong cuộc trò chuyện được tóm tắt. Đối chiếu với hồ sơ nguồn là bước làm cho bàn giao đáng tin cậy, và đáp án đúng luôn có bước đó. Lĩnh vực 2 vẫn áp dụng khi bàn giao.

### Giữ mọi thứ trong một chat khổng lồ vì cho rằng bắt đầu lại sẽ mất bối cảnh

Đó là thói quen kéo dài chat được trình bày dưới danh nghĩa duy trì tính liên tục. Chat đầy các bản nháp bị thay thế và hướng đi bế tắc bên cạnh những quyết định quan trọng, tiến gần giới hạn độ dài và tiêu thụ nhiều hạn mức hơn. Tóm tắt và lưu giữ giúp chuyển tiếp tất cả những gì đáng giữ.

## Tình huống luyện tập

Một điều phối viên đám cưới đã dùng một cuộc trò chuyện khổng lồ trong ba tháng lập kế hoạch: quyết định địa điểm, trình tự chương trình, các bài đọc trong buổi lễ và các lần sửa tên. Tháng cuối cùng bắt đầu, chat đầy chi tiết đã bị thay thế và sắp chạm giới hạn độ dài của nền tảng. Một số tên và ngày tháng đã được sửa nhiều lần, nên bất kỳ bản tóm tắt nào của chat cũ cũng có thể chứa phiên bản lỗi thời. Kế hoạch nào tốt nhất?

**Phương án A**

Nhờ Claude tóm tắt việc lập kế hoạch đến hiện tại rồi dán thẳng vào chat mới, vì Claude đã viết từ toàn bộ lịch sử và đây là hồ sơ đáng tin cậy nhất hiện có.

**Phương án B**

Tiếp tục một cuộc trò chuyện đó đến ngày cưới, vì mọi quyết định đều nằm trong đó và chat mới sẽ mất ba tháng bối cảnh.

**Phương án C**

Nhờ Claude tóm tắt quyết định và các câu hỏi còn mở, xác minh bản tóm tắt bằng xác nhận đặt dịch vụ, dùng nó mở chat cho tháng cuối; chuyển sơ đồ chỗ ngồi và trình tự chương trình thành artifact, các tài liệu dùng thường xuyên vào kho kiến thức Project.

**Phương án D**

Bắt đầu chat mới và dựa vào bộ nhớ cùng tìm kiếm chat để chuyển sơ đồ chỗ ngồi và trình tự chương trình, yêu cầu Claude nhớ các chi tiết kế hoạch, kể cả tên đã sửa và các bài đọc, trước khi đóng chat cũ kéo dài ba tháng.

## Bài tập thực hành: Áp dụng kỷ luật bàn giao cho chat dài nhất của bạn

**Thời gian:** 30 phút.

### Bạn sẽ học được

- Cách trích bản tóm tắt quyết định, trạng thái và việc còn lại từ cuộc trò chuyện dài.
- Cách xác minh bản tóm tắt bằng hồ sơ nguồn trước khi tin dùng.
- Cách mở chat mới từ bản giao việc đã xác minh.
- Cách phân loại đầu ra vào nhóm dán chuyển tiếp, artifact và kho kiến thức Project.
- Cách kiểm tra bộ nhớ mang theo gì và không mang theo gì sang chat mới.

### Bước 1 — Tìm cuộc trò chuyện Claude kéo dài lâu nhất của bạn

Yêu cầu Claude tóm tắt các quyết định đã đưa ra, trạng thái hiện tại và các câu hỏi còn mở.

**Vì sao:** Bản tóm tắt là tài liệu bàn giao. Chat dài chứa những quyết định đáng giữ bị chôn trong các chi tiết không còn cần thiết.

**Kết quả cần thấy:** Bản tóm tắt có cấu trúc ba phần: quyết định, trạng thái hiện tại và câu hỏi còn mở.

### Bước 2 — Xác minh bản tóm tắt bằng hồ sơ nguồn

Đối chiếu với email, xác nhận đặt chỗ hoặc tài liệu làm căn cứ cho quyết định, rồi sửa các chỗ sai.

**Vì sao:** Bản tóm tắt kế thừa mọi lỗi chưa sửa trong chat. Xác minh khiến nó đủ đáng tin để dùng làm nền tảng tiếp theo.

**Kết quả cần thấy:** Bản tóm tắt đã chỉnh, có ít nhất một chỗ được sửa hoặc ghi chú rằng không cần sửa.

### Bước 3 — Mở chat mới bằng bản tóm tắt đã xác minh

Ghi lại việc bắt đầu mới thay đổi các câu trả lời đầu tiên như thế nào.

**Vì sao:** Trải nghiệm sự khác biệt giữa bản giao việc gọn, rõ và cuộc trò chuyện kéo dài khiến quyết định bắt đầu lại trở nên cụ thể.

**Kết quả cần thấy:** Các câu trả lời làm việc từ đúng bối cảnh bạn chọn mang theo, không có nội dung đã bị thay thế cản trở.

### Bước 4 — Phân loại đầu ra làm việc của chat cũ vào nơi phù hợp

Xác định nội dung nào chỉ được dán chuyển tiếp một lần, nội dung nào thành artifact vì liên tục được sửa và chia sẻ, và nội dung nào thuộc kho kiến thức Project vì mọi chat sau đều cần.

**Vì sao:** Lưu giữ là quyết định chọn nơi chuyển đến. Mỗi nơi phục vụ vòng đời đầu ra khác nhau.

**Kết quả cần thấy:** Mỗi đầu ra quan trọng có một nơi lưu phù hợp; artifact đã được tạo và kiến thức Project đã được lưu.

### Bước 5 — Kiểm tra đóng góp của bộ nhớ khi bắt đầu mới

Ghi những điều Claude biết hữu ích về bạn và dự án, đồng thời xác nhận chính các đầu ra làm việc chỉ xuất hiện vì bạn đã chủ động lưu giữ và chuyển tiếp.

**Vì sao:** Nhìn thấy ranh giới trong công việc của mình củng cố sự phân biệt mà bài thi kiểm tra: bộ nhớ mang theo bối cảnh về bạn; lưu giữ chủ động mang theo công việc.

**Kết quả cần thấy:** Ghi chú hai dòng: bộ nhớ cung cấp gì và hành động lưu giữ, chuyển tiếp chủ động cung cấp gì.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Hạn mức sử dụng và giới hạn độ dài hoạt động như thế nào? — *How do usage and length limits work?*
- Dùng tìm kiếm cuộc trò chuyện và ghi nhớ của Claude để tiếp nối bối cảnh trước đó — *Use Claude's chat search and memory to build on previous context*.
- Đưa tính năng ghi nhớ đến Claude — *Bringing memory to Claude*.
- Project là gì? — *What are projects?*
- Artifact là gì và sử dụng như thế nào? — *What are artifacts and how do I use them?*
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [3.3 — Lựa chọn mô hình phù hợp với chi phí, tốc độ và chất lượng](3-3-cost-speed-quality.vi.md).
- **Bài tiếp theo:** [4.1 — Phân tích yêu cầu và trường hợp sử dụng](4-1-requirements-and-use-cases.vi.md).
