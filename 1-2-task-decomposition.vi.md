# 1.2 — Chia nhỏ yêu cầu phức tạp

- **Lĩnh vực (Domain):** 1
- **Nhiệm vụ (Task):** 1.2
- **Tên bài gốc:** Decomposing Complex Requests
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/1-prompting-task-execution/1-2-task-decomposition)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Với công việc phức tạp, Claude tạo đầu ra tốt nhất khi công việc được chia thành các phần mà nó có thể xử lý đầy đủ, lần lượt từng phần. Cách chia này gọi là **phân rã nhiệm vụ (task decomposition)**. Các phần có liên hệ phụ thuộc vào nhau: phần sau cần đầu ra hoặc quyết định từ phần trước. Các phần độc lập có thể đứng riêng.

Một prompt được xây dựng tốt có thể xử lý khá nhiều việc, nhưng vẫn có giới hạn. Khi nhồi lượng yêu cầu của cả một dự án vào một tin nhắn, kết quả sẽ hời hợt và không đồng đều: một số phần được làm tốt, những phần khác chỉ được lướt qua. Hãy xét một quản lý siêu thị đang viết báo cáo hằng quý về phản hồi khách hàng cho trụ sở chính. Báo cáo cần có dàn ý, các phần thống nhất giọng văn và danh sách hành động. Cô cũng cần một bản tóm tắt về cửa hàng đối thủ, một thông cáo báo chí và một bảng ngân sách. Danh sách cách khắc phục câu trả lời không hữu ích trong Trung tâm trợ giúp có đề cập việc chia yêu cầu phức tạp thành các bước nhỏ. Tài liệu này cũng nói prompt nên chứa càng nhiều bối cảnh càng tốt.

## Bốn kỹ thuật, từ đơn giản đến cần tổ chức nhiều hơn

### 1. Các bước đánh số trong một prompt

Với các phần có liên hệ, hãy liệt kê chúng rõ ràng. Người quản lý viết: trước tiên tóm tắt các nhóm chủ đề phản hồi, sau đó xếp hạng theo tần suất, rồi đề xuất một hành động cải thiện cho mỗi chủ đề. Claude tuân theo một trình tự rõ ràng đáng tin cậy hơn nhiều so với một đoạn dài gộp nhiều yêu cầu. Anthropic hướng dẫn sử dụng các bước tuần tự được đánh số khi thứ tự hoặc tính đầy đủ là yếu tố quan trọng, đồng thời nêu cụ thể định dạng đầu ra và các ràng buộc.

### 2. Viết prompt theo từng giai đoạn trong cùng một cuộc trò chuyện

Với sản phẩm được xây dựng qua nhiều lớp, hãy yêu cầu dàn ý, xem xét và điều chỉnh, rồi soạn lần lượt từng phần. Bạn kiểm tra đầu ra của mỗi giai đoạn trước khi chạy giai đoạn tiếp theo. Đầu ra đã được duyệt trở thành nền tảng cho giai đoạn sau, vì vậy bạn có thể điều chỉnh hướng đi khi chi phí sửa đổi còn thấp. Người quản lý chỉnh dàn ý trước khi bất kỳ phần nội dung nào được viết.

### 3. Yêu cầu lập kế hoạch trước (Plan-first prompting)

Khi chưa rõ cấu trúc nào phù hợp, hãy yêu cầu Claude đề xuất cách tiếp cận trước. Ví dụ: “Trước khi viết bất kỳ nội dung nào, hãy liệt kê các phần bạn sẽ đưa vào và nội dung mỗi phần.” Xem xét một kế hoạch chỉ mất vài giây. Làm lại một bản nháp 2.000 từ đi sai hướng thì không như vậy.

### 4. Tách cuộc trò chuyện cho từng nhiệm vụ con

Những phần thực sự độc lập, chẳng hạn bản tóm tắt về đối thủ, thông cáo báo chí hoặc bảng ngân sách, nên được xử lý trong các cuộc trò chuyện riêng. Như vậy, bối cảnh của mỗi cuộc trò chuyện được giữ gọn và tập trung. Ba công việc phụ của người quản lý được bố trí vào ba cuộc trò chuyện riêng.

## Lựa chọn kỹ thuật

Các phần có liên hệ nên nằm trong cùng một cuộc trò chuyện và được thực hiện theo giai đoạn, để các giai đoạn sau kế thừa phần đã được duyệt trước đó. Các sản phẩm độc lập nên nằm trong những cuộc trò chuyện riêng. Khi chưa rõ cấu trúc, hãy yêu cầu kế hoạch trước. Lựa chọn không phù hợp dẫn đến một trong hai kiểu thất bại: một “siêu prompt” phình to, yêu cầu hoàn thành sản phẩm 20 trang trong một lượt; hoặc chia vụn công việc có liên hệ sang nhiều cuộc trò chuyện. Ở kiểu thứ hai, mỗi cuộc trò chuyện mới đều không có dàn ý và các quyết định về giọng văn đã được xây dựng trước đó. Nếu tách các phần của báo cáo sang những cuộc trò chuyện khác nhau, người quản lý sẽ mất tính kế thừa về dàn ý và giọng văn.

## Chuyển tiếp bối cảnh

Một cuộc trò chuyện mới không tự động có tài liệu làm việc của cuộc trò chuyện khác. Hiện Claude đã có khả năng ghi nhớ giữa các cuộc trò chuyện dưới dạng các chủ đề riêng lẻ về vai trò, dự án, sở thích và bối cảnh công việc đang diễn ra của bạn. Đó là thông tin bối cảnh về bạn, không phải bản ghi nguyên cuộc trò chuyện. Tính năng này không tự mang dàn ý đã được duyệt, hướng dẫn giọng văn hoặc bản nháp viết dở sang cuộc trò chuyện mới. Trên các gói trả phí, bạn có thể yêu cầu Claude tìm trong các cuộc trò chuyện trước và đưa vào những chi tiết liên quan. Đó là thao tác truy xuất bạn phải chủ động yêu cầu, không phải sự chuyển tiếp tự động.

Cách đáng tin cậy là chủ động lưu giữ và chuyển tiếp thông tin. Dán đầu ra vào cuộc trò chuyện mới, đính kèm lại tệp hoặc lưu trong kho kiến thức của một **Project**. Project là không gian làm việc riêng, có lịch sử trò chuyện và kiến thức của chính nó. Khi quay lại báo cáo trong một cuộc trò chuyện mới, người quản lý dán dàn ý vào trước. Bạn là người chịu trách nhiệm chuyển tiếp đầu ra, không phải sản phẩm tự làm việc đó.

## Trong bài thi

Bài thi kiểm tra khả năng ghép kỹ thuật với tình huống, không phải khả năng đọc thuộc tên bốn kỹ thuật. Đáp án đúng tuân theo ba quy tắc lựa chọn ở trên. Cả hai kiểu thất bại đều xuất hiện trong các phương án gây nhiễu. Nên lưu giữ thông tin ở đâu là câu hỏi thuộc Lĩnh vực 3 và Lĩnh vực 5.

### Trạng thái hiện tại trong bản gốc — tháng 9 năm 2026

Tính năng ghi nhớ xuất hiện trên claude.ai vào ngày 11 tháng 9 năm 2025 cho các gói Team và Enterprise, sau đó có trên Pro và Max từ ngày 23 tháng 10 năm 2025. Tính đến ngày 30 tháng 9 năm 2026, tính năng này được bật mặc định cho Free, Pro và Max. Cũng tại thời điểm đó, trên Team và Enterprise, chủ sở hữu quyết định có cho phép dùng tính năng ghi nhớ hay không. Tính năng vẫn tắt đối với từng thành viên cho đến khi chính thành viên đó bật lên. Tìm kiếm cuộc trò chuyện — yêu cầu Claude tham chiếu các cuộc trò chuyện trước — có trên các gói trả phí. Không tính năng nào làm thay đổi quy tắc: ghi nhớ lưu bối cảnh về bạn theo các chủ đề riêng lẻ, còn tìm kiếm cuộc trò chuyện phải được yêu cầu qua prompt.

## Những bẫy thường gặp trong bài thi

### Chọn “siêu prompt” làm tất cả để giữ toàn bộ sản phẩm ở một chỗ

Khi lượng yêu cầu của cả dự án bị đưa vào một tin nhắn, sự chú ý được phân bổ không đồng đều: một số phần tốt, phần khác chỉ được làm sơ sài; việc sửa sai chỉ diễn ra sau khi toàn bộ sản phẩm đã đi lệch hướng. Chia yêu cầu phức tạp thành các bước nhỏ là cách khắc phục đã được tài liệu hướng dẫn ghi nhận.

### Chia công việc có liên hệ sang các cuộc trò chuyện riêng

Mỗi cuộc trò chuyện mới đều thiếu dàn ý, các quyết định về giọng văn và nội dung đã được duyệt ở cuộc trò chuyện trước. Vì vậy, các phần có giọng văn khác nhau và cần được chỉnh cho thống nhất bằng tay. Cuộc trò chuyện riêng phù hợp với các sản phẩm độc lập, không phải các phần có liên hệ.

### Yêu cầu lập kế hoạch trước khi cấu trúc đã rõ và được thống nhất

Nhờ Claude đề xuất những phần bạn đã chốt là một bước vòng không cần thiết: thêm một lượt duyệt mà không bổ sung thông tin. Lập kế hoạch trước chỉ có giá trị khi cấu trúc phù hợp thực sự chưa rõ.

## Tình huống luyện tập

Giám đốc chương trình tại một tổ chức từ thiện phải tạo báo cáo tác động hằng năm dài 20 trang, gồm phần tổng quan, năm phần được soạn từ ghi chép của năm nhóm chương trình khác nhau và giọng văn thống nhất xuyên suốt. Giám đốc muốn duyệt từng phần ngay khi được tạo ra, đồng thời không muốn phải giải thích lại những quyết định đã chốt trong một cuộc trò chuyện mới. Nên tổ chức công việc với Claude như thế nào?

**Phương án A**

Gửi một prompt kèm ghi chép của cả năm nhóm và yêu cầu hoàn thành báo cáo 20 trang, bao gồm phần tổng quan, trong một lượt để không mất thông tin giữa các cuộc trò chuyện và giữ giọng văn nhất quán.

**Phương án B**

Dùng một cuộc trò chuyện: thống nhất dàn ý và hướng dẫn giọng văn trước, sau đó soạn từng phần; mỗi prompt cung cấp ghi chép cho phần đó. Viết phần tổng quan sau cùng dựa trên các phần đã hoàn thành.

**Phương án C**

Yêu cầu mỗi nhóm trong năm nhóm chương trình tự dùng một cuộc trò chuyện Claude theo phong cách mình thích, rồi ghép sáu bản nháp thu được thành một tài liệu sau đó.

**Phương án D**

Mở sáu cuộc trò chuyện riêng, mỗi phần một cuộc và phần tổng quan một cuộc, để mỗi cuộc trò chuyện đều nhỏ, tập trung và không cuộc nào chạm giới hạn độ dài.

## Bài tập thực hành: Thực hiện sản phẩm nhiều phần theo từng giai đoạn

**Thời gian:** 30 phút.

### Bạn sẽ học được

- Cách phân loại các phần của một sản phẩm thành có liên hệ và độc lập.
- Cách chọn kỹ thuật đơn giản nhất phù hợp với từng phần.
- Cách chỉnh dàn ý trước khi bắt đầu soạn nội dung.
- Cách chuyển tiếp đầu ra đã được duyệt sang các giai đoạn sau.

### Bước 1 — Chọn một sản phẩm thực sự gồm nhiều phần trong công việc

Ví dụ: báo cáo hằng năm, kế hoạch dự án hoặc bộ tài liệu khóa học.

**Vì sao:** Việc phân rã chỉ cho thấy giá trị với công việc quá lớn để xử lý bằng một prompt. Nhiệm vụ nhỏ không giúp bạn thực hành đầy đủ các kỹ thuật.

**Kết quả cần thấy:** Một sản phẩm được nêu tên cùng danh sách các phần dưới dạng gạch đầu dòng.

### Bước 2 — Phân loại các phần theo mức độ liên hệ

Nhóm “có liên hệ” gồm các phần cung cấp đầu vào cho nhau. Nhóm “độc lập” gồm các phần có thể đứng riêng.

**Vì sao:** Đây là khả năng phán đoán bài thi kiểm tra: các phần có liên hệ cần một cuộc trò chuyện theo giai đoạn; các phần độc lập cần các cuộc trò chuyện riêng.

**Kết quả cần thấy:** Mỗi phần được gắn nhãn “có liên hệ” hoặc “độc lập”, kèm một cụm từ giải thích lý do.

### Bước 3 — Chọn kỹ thuật cho từng phần

Chọn giữa các bước đánh số, cuộc trò chuyện theo giai đoạn, lập kế hoạch trước hoặc cuộc trò chuyện riêng; với mỗi lựa chọn, viết một câu giải thích.

**Vì sao:** Ghép kỹ thuật với nhiệm vụ chính là mục tiêu bài học. Việc giải thích giúp bảo đảm lựa chọn có cơ sở.

**Kết quả cần thấy:** Một danh sách ngắn ghép từng phần với kỹ thuật và lý do lựa chọn.

### Bước 4 — Thực hiện giai đoạn đầu tiên và chỉnh sửa trước khi soạn nội dung

Giai đoạn đầu tiên là dàn ý hoặc kế hoạch. Hãy chỉnh nó trước khi bắt đầu viết.

**Vì sao:** Điều chỉnh hướng đi ở giai đoạn dàn ý chỉ mất vài giây; cùng thay đổi đó sau 2.000 từ có thể tốn cả buổi chiều.

**Kết quả cần thấy:** Một dàn ý đã được duyệt mà bạn có chủ động chỉnh sửa, thay vì chỉ chấp nhận nguyên trạng.

### Bước 5 — Ghi lại cách chuyển tiếp đầu ra

Mỗi khi giai đoạn sau cần đầu ra của giai đoạn trước, hãy ghi cách bạn chuyển tiếp: dán vào, đính kèm lại hoặc lưu trong Project.

**Vì sao:** Một cuộc trò chuyện mới không tự động có tài liệu làm việc của cuộc trò chuyện trước. Chủ động chuyển tiếp là cách đáng tin cậy.

**Kết quả cần thấy:** Mỗi giai đoạn có một ghi chú về phương thức chuyển tiếp bạn đã dùng.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Prompt của tôi không tạo ra câu trả lời hữu ích — *My prompt isn't giving me a helpful answer*.
- Các phương pháp tốt nhất khi viết prompt — *Prompting best practices*.
- Hạn mức sử dụng và giới hạn độ dài hoạt động như thế nào? — *How do usage and length limits work?*
- Dùng tìm kiếm cuộc trò chuyện và ghi nhớ của Claude để tiếp nối bối cảnh trước đó — *Use Claude's chat search and memory to build on previous context*.
- Đưa tính năng ghi nhớ đến Claude — *Bringing memory to Claude*.
- Project là gì? — *What are projects?*

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [1.1 — Tạo prompt hiệu quả cho công việc nghiệp vụ và kỹ thuật](1-1-effective-prompts.vi.md).
- **Bài tiếp theo:** [1.3 — Tinh chỉnh prompt qua nhiều vòng để cải thiện đầu ra](1-3-prompt-iteration.vi.md).
