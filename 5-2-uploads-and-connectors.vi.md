# 5.2 — Quản lý kiến thức tải lên và trình kết nối

- **Lĩnh vực (Domain):** 5
- **Nhiệm vụ (Task):** 5.2
- **Tên bài gốc:** Managing Uploaded Knowledge and Connectors
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/5-configuration-knowledge/5-2-uploads-and-connectors)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Kiến thức của Project là tài liệu Claude dựa vào bên trong Project đó. Tài liệu đến qua một trong hai cách. **Tải lên (upload)** đưa bản sao vào kho kiến thức: tài liệu, văn bản, mã và các tệp khác. **Trình kết nối (connector)** liên kết Claude với nguồn hiện hành, chẳng hạn Google Drive. Mỗi cách có đặc điểm mà cách kia không có. Lựa chọn phụ thuộc cách tài liệu thay đổi.

Hãy xét một đơn vị sơn và trang trí đang thiết lập Project để báo giá, lên kế hoạch công việc. Điều khoản, điều kiện và bản mô tả biện pháp thi công hầu như không đổi. Lịch công việc là Google Doc trong Drive, thay đổi mỗi tuần.

## Bản chụp tại một thời điểm hay nguồn hiện hành

Tệp tải lên là bản sao tại ngày tải. Mọi người dùng Project nhìn thấy cùng bản sao nên nội dung ổn định, dễ dự đoán. Khi tài liệu nguồn bị thay thế, bản sao vẫn giữ nguyên và không có gì thông báo. Sáu tháng sau, nó trông vẫn mới như ngày đầu. Điều này phù hợp với điều khoản, điều kiện nhưng không phù hợp lịch công việc sẽ sai sau một tuần.

Connector phù hợp tài liệu thay đổi vì truy cập nguồn hiện hành khi được yêu cầu. Tài liệu Google Workspace nêu rằng Google Docs được thêm vào chat và Project đồng bộ trực tiếp từ Google Drive, nên bạn luôn làm việc với phiên bản mới nhất. Tài liệu cũng nêu Claude chỉ truy cập dữ liệu khi bạn hỏi rõ một câu hoặc yêu cầu hành động cần dữ liệu đó, chỉ lấy lượng thông tin tối thiểu cần thiết.

Phiên bản mới nhất bao gồm cả phần đồng nghiệp đang sửa dở đúng lúc bạn hỏi. Nếu người quản lý văn phòng mới chuyển được một nửa công việc thứ Ba, Claude đọc phiên bản chuyển dở ấy. Tài liệu hiện hành cũng mang theo sự lộn xộn đang diễn ra, nên tài liệu tham khảo ổn định thường phù hợp tải lên hơn.

## Quyền truy cập và quản trị

Không phải ở mọi nơi làm việc, mỗi cá nhân đều có thể tự bật connector. Trên các gói Team và Enterprise, **Chủ sở hữu (Owner)** hoặc **Chủ sở hữu chính (Primary Owner)** cần bật connector cho tổ chức trước khi thành viên dùng. Nếu connector bị tắt trong không gian làm việc, bước đúng là yêu cầu người quản trị, không phải tự ứng biến.

Quyền truy cập phản ánh quyền mỗi người vốn có trong dịch vụ kết nối. Nếu ai đó không truy cập được tệp ở hệ thống nguồn, connector cũng không thể lấy tệp từ Claude cho họ. Hai đồng nghiệp dùng cùng Project có thể nhận câu trả lời khác nhau từ cùng connector. Đây là đặc điểm hệ thống phân quyền, không phải lỗi Project.

Connector không chỉ đọc. Chúng có thể lấy dữ liệu và thực hiện hành động trong dịch vụ kết nối. Connector Gmail có thể gửi, trả lời và chuyển tiếp email từ tài khoản của chính bạn. Mặc định, Claude hỏi bạn phê duyệt trước từng hành động. Đơn vị sơn vẫn duyệt từng email báo giá trước khi gửi.

## Truy xuất, không phải đọc toàn bộ từ đầu đến cuối

Project có kho kiến thức lớn không được đọc toàn bộ mỗi lần có câu hỏi. Tài liệu mô tả Claude tìm kiếm kiến thức Project và chỉ nạp nội dung liên quan nhất. Truy xuất được kích hoạt khi Project tiến gần hoặc vượt giới hạn cửa sổ ngữ cảnh. Cơ chế truy xuất phải tìm đúng tài liệu giữa mọi thứ đã cung cấp.

Hai cách được tài liệu hướng dẫn ghi nhận giúp ích. Tên tệp rõ ràng, có tính mô tả giúp tìm đúng tài liệu: `terms-and-conditions` tốt hơn `final-v2-new`. Bạn cũng có thể nêu tên tài liệu cụ thể trong prompt để tập trung tìm kiếm vào đó.

## Chọn lọc tốt hơn thu gom đầy đủ

Kho kiến thức Project không phải kho lưu trữ. Mỗi tài liệu không bao giờ cần đến làm loãng phạm vi tìm kiếm và tạo khả năng bị trích vào sai thời điểm. Một tập nhỏ tài liệu liên quan tốt hơn tải lên hàng loạt. Dọn các tệp không còn sử dụng tích cực thay vì để lại.

Khi được giao một ổ đĩa dùng chung, hãy chọn ít tài liệu mà công việc cần và đưa từng tài liệu vào bằng cách phù hợp với mức thay đổi. Tài liệu cập nhật liên tục như lịch công việc của đơn vị sơn đi qua connector đến nguồn hiện hành. Tài liệu tham khảo ổn định như bản mô tả biện pháp thi công được tải lên. Đồng nghiệp muốn đưa mọi thứ vào có ý tốt. Cái giá xuất hiện sau, trong câu trả lời dựa vào sai tài liệu.

## Trong bài thi

Câu hỏi kiểm tra bạn ghép cách đưa tài liệu vào với đặc điểm tài liệu hay không; dấu hiệu trong gần như mọi phần dẫn là cách tài liệu thay đổi. Tài liệu có được phép xuất hiện trong Project hay không vì quyền riêng tư, hợp đồng hoặc chính sách là câu hỏi của Lĩnh vực 6. Mục tiêu này quản lý những tài liệu đã được phép đưa vào.

### Trạng thái trong bản gốc: Nơi có thể dùng cách kết nối Drive

Hướng dẫn thi nêu Google Drive là connector cần quản lý cùng với tệp tải lên; đưa tài liệu cập nhật liên tục qua connector là phán đoán quyết định đáp án. Tính đến ngày 28 tháng 9 năm 2026, bài viết *Use Google Workspace connectors* mô tả cách thêm từ Drive là thêm từng tài liệu, chỉ vào phần **Files** của Project riêng tư. Bạn thêm từng tài liệu bằng cách tìm trong tài liệu gần đây hoặc dán liên kết. Bài viết cho biết tùy chọn này bị tắt với Project dùng chung, nơi phần Files nhận tệp tải lên. Connector vẫn hoạt động trong chat: Google Docs thêm vào chat đồng bộ trực tiếp từ Drive. Trong bài thi, hãy lựa chọn theo cách tài liệu thay đổi.

### Dấu hiệu trong câu hỏi thi

Câu hỏi tải lên hay connector dựa vào cách tài liệu thay đổi, không dựa vào mức độ quan trọng. Lịch công việc hằng tuần dùng connector dù trông nhỏ nhặt. Điều khoản, điều kiện hầu như không đổi được tải lên dù quan trọng đến đâu.

## Những bẫy thường gặp trong bài thi

### Đưa cả ổ đĩa dùng chung vào để không thiếu gì

Việc đổ toàn bộ dữ liệu trông như cẩn thận, nhưng chính là thói quen mà chọn lọc nhằm sửa. Truy xuất phải tìm đúng tài liệu giữa tất cả những gì được cung cấp, nên mỗi tệp không liên quan khiến tài liệu cần khó xuất hiện hơn và dễ bị thay thế bởi trích dẫn sai thời điểm.

### Chọn tải lên hay connector theo mức độ quan trọng

Tầm quan trọng là tiêu chí sai. Đáp án đúng lựa chọn theo thay đổi: tài liệu sửa thường xuyên nên dùng connector đến nguồn hiện hành; tài liệu tham khảo ổn định tải lên một lần. Lịch trực tải lên âm thầm lỗi thời dù công việc phụ thuộc nó đến mức nào.

### Để người dùng gói Team tự bật connector cho tổ chức

Owner hoặc Primary Owner phải bật connector cho tổ chức trước khi thành viên sử dụng. Vì vậy, cách xử lý đúng là hỏi người quản trị không gian làm việc. Phương án để thí sinh tự ứng biến việc bật đang kiểm tra chính bước quản trị này.

## Tình huống luyện tập

Một hội bảo tồn hang động du lịch đang thiết lập kiến thức cho Project về lịch trực hướng dẫn viên, tổ chức mở cửa và liên lạc tình nguyện viên. Lịch trực và giờ mở cửa — thay đổi theo mực nước sau mưa — nằm trong thư mục Drive dùng chung. Điều lệ, đánh giá rủi ro tại địa điểm và sổ tay hướng dẫn viên hầu như không đổi. Một thành viên ban quản trị đề xuất đưa toàn bộ ổ đĩa dùng chung vào để mọi thứ đều sẵn có. Tài liệu không liên quan ba lĩnh vực trên không nên có trong Project. Thiết lập nào tốt nhất?

**Phương án A**

Thêm lịch trực và giờ mở cửa từ Drive để chat dựa vào phiên bản hiện hành; tải điều lệ, đánh giá rủi ro và sổ tay dưới dạng tệp; không đưa phần còn lại của ổ đĩa vào.

**Phương án B**

Tải mọi thứ thành tệp, kể cả lịch trực và giờ mở cửa hiện tại, để mọi người dùng Project luôn nhìn thấy đúng cùng một tập tài liệu ổn định khi hỏi.

**Phương án C**

Không đưa kiến thức vào Project; ai hỏi thì dán lịch trực và giờ mở cửa hiện tại vào chat mỗi lần.

**Phương án D**

Đưa cả ổ đĩa dùng chung vào như đề xuất để mọi tài liệu hội có, từ biên bản họp đến thư từ cũ, đều sẵn cho Project ngay ngày đầu mà không ai phải lựa chọn.

## Bài tập thực hành: Chọn cách đưa tài liệu của Project vào theo mức thay đổi

**Thời gian:** 30 phút.

### Bạn sẽ học được

- Cách phân loại từng tài liệu theo tần suất thay đổi.
- Cách dùng connector cho tài liệu cập nhật liên tục và tải lên tài liệu ổn định.
- Cách kiểm tra quy định quản trị connector trước khi dựa vào nó.
- Cách kiểm tra Project thực sự trích phiên bản nào của tài liệu đã thay đổi.

### Bước 1 — Liệt kê mọi tài liệu công việc lặp lại cần

Đánh dấu từng tài liệu: thay đổi hằng tuần, hằng tháng hoặc hầu như không đổi.

**Vì sao:** Quyết định được đưa ra theo từng tài liệu; tần suất thay đổi là trục chính của toàn bộ mục tiêu.

**Kết quả cần thấy:** Danh sách hai cột: tài liệu cập nhật liên tục một bên, tài liệu ổn định một bên.

### Bước 2 — Tải phiên bản hiện hành của nhóm ổn định vào kiến thức Project

Ghi lại ngày tải lên.

**Vì sao:** Tài liệu ổn định hưởng đúng thế mạnh của tải lên: dễ dự đoán, giống nhau cho mọi người và được tham khảo không phụ thuộc nguồn đang thay đổi.

**Kết quả cần thấy:** Các tài liệu ổn định trong kho kiến thức, kèm ghi chú ngày tải.

### Bước 3 — Xác định nơi lưu phiên bản hiện hành của nhóm cập nhật liên tục

Nếu nằm trong Google Drive và nơi làm việc cho phép connector, thêm tài liệu từ Drive thay vì tải bản sao.

**Vì sao:** Connector giữ tài liệu hiện hành mà không cần ai nhớ tải lại, tránh kiểu thất bại vốn có của tệp tải lên.

**Kết quả cần thấy:** Tài liệu cập nhật liên tục truy cập được qua connector Drive hoặc có yêu cầu bằng văn bản gửi người quản trị nếu connector chưa bật.

### Bước 4 — Cắt bỏ quyết liệt và đặt tên rõ ràng

Loại mọi tài liệu chỉ được liệt kê vì có thể một ngày nào đó hữu ích. Đặt tên mô tả rõ cho các tệp còn lại.

**Vì sao:** Tài liệu không bao giờ cần làm loãng truy xuất. Tên tệp tốt giúp tìm đúng nội dung.

**Kết quả cần thấy:** Danh sách kiến thức ngắn hơn, mỗi tệp có lý do tồn tại và tên nói rõ nội dung.

### Bước 5 — Thử câu hỏi có câu trả lời vừa thay đổi

Kiểm tra Project trích phiên bản nào.

**Vì sao:** Phép thử chứng minh cách đưa tài liệu vào có đúng không: tài liệu kết nối nên cho câu trả lời từ phiên bản hiện tại; câu trả lời cũ cho thấy tài liệu cập nhật liên tục đã bị tải lên thành bản sao.

**Kết quả cần thấy:** Câu trả lời trích phiên bản hiện hành hoặc xác định được tệp cụ thể cần đổi cách đưa vào.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Tạo sinh tăng cường truy xuất (RAG) cho Project — *Retrieval augmented generation (RAG) for projects*.
- Dùng connector để mở rộng khả năng của Claude — *Use connectors to extend Claude's capabilities*.
- Sử dụng connector Google Workspace — *Use Google Workspace connectors*.
- Hạn mức sử dụng và giới hạn độ dài hoạt động như thế nào? — *How do usage and length limits work?*
- Project là gì? — *What are projects?*
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [5.1 — Cấu hình Project với chỉ dẫn và nguồn kiến thức](5-1-project-instructions-knowledge.vi.md).
- **Bài tiếp theo:** [5.3 — Tạo chỉ dẫn cấp hệ thống hiệu quả](5-3-system-level-instructions.vi.md).
