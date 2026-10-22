# 1.4 — Điều chỉnh chiến lược theo loại nhiệm vụ

- **Lĩnh vực (Domain):** 1
- **Nhiệm vụ (Task):** 1.4
- **Tên bài gốc:** Adapting Strategy to Task Type
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/1-prompting-task-execution/1-4-task-type-strategies)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Loại nhiệm vụ là loại công việc bạn giao cho Claude. Mục tiêu này bao quát bốn loại: **phân tích (analysis)** — tìm hiểu tài liệu cho thấy điều gì; **nghiên cứu (research)** — thu thập thông tin từ các nguồn; **soạn thảo (drafting)** — viết một nội dung; và **động não (brainstorming)** — tạo ý tưởng. Tài liệu của Anthropic cho thấy Claude thực hiện cả bốn: phân tích dữ liệu biểu đồ, soạn mọi thứ từ tin nhắn đến kịch bản phim, đồng thời tạo ra các góc nhìn và khuyến nghị với vai trò đối tác phát triển ý tưởng. Một cách viết prompt không phù hợp với cả bốn loại. Mỗi loại đạt hiệu quả với một cấu trúc giao việc khác nhau, tức là những nội dung cần đưa vào prompt cũng khác nhau.

Một quản lý công ty môi giới cho thuê bất động sản có bốn việc trong tháng này. Cô phải tìm hiểu vì sao số lượt gia hạn hợp đồng thuê giảm, so sánh cách các công ty khác sàng lọc người thuê, viết thư cho chủ nhà về một khoản phí mới và tìm cách thu hút thêm chủ nhà sử dụng dịch vụ.

## Phân tích: Tài liệu cùng câu hỏi

Phân tích bắt đầu từ tài liệu. Hãy đính kèm bảng tính hoặc dán kết quả khảo sát, vì Claude làm việc dựa trên những gì được cung cấp. Tải tệp lên giúp đưa vào các tài liệu thực tế, kể cả tài liệu dài hàng trăm trang.

Tiếp theo, nêu những câu hỏi mà phân tích phải trả lời và quyết định sẽ dựa vào kết quả đó. “Phân tích dữ liệu này” không cho Claude một mục tiêu, nên nó sẽ mô tả thay vì phân tích. Người quản lý đính kèm bảng tính gia hạn hợp đồng và hỏi: vì sao số lượt gia hạn giảm, bất động sản nào mất nhiều người thuê nhất và cần thay đổi điều gì trước năm tới? Hãy yêu cầu các phát hiện chính, bằng chứng hỗ trợ, những hạn chế hoặc điểm cần lưu ý, cùng cách Claude đi đến từng kết luận để có thể kiểm tra lập luận. Kiểm tra lập luận đó là công việc thuộc Lĩnh vực 2.

## Nghiên cứu: Câu hỏi có phạm vi rõ ràng

Với câu hỏi cần nhiều nguồn, tính năng **Research** hoạt động theo cơ chế tác tử (agent): Claude thực hiện nhiều lượt tìm kiếm nối tiếp, mỗi lượt dựa trên kết quả trước đó, rồi trả về báo cáo có trích dẫn dễ kiểm tra. Với một thông tin hiện thời cần tra nhanh, tìm kiếm web thông thường là đủ. Ranh giới được tài liệu nêu rõ: tìm kiếm web phù hợp với câu hỏi sự kiện đơn giản, có thể trả lời sau một hoặc hai lượt tra cứu; Research phù hợp với việc thu thập thông tin kỹ lưỡng qua nhiều lượt tìm kiếm.

Dù dùng cách nào, hãy giao một câu hỏi nghiên cứu, thay vì chỉ đưa ra chủ đề. Nêu phạm vi, góc tiếp cận và quyết định mà kết quả phải hỗ trợ. Người quản lý yêu cầu Research tìm hiểu các công ty cùng quy mô trong khu vực sàng lọc người thuê như thế nào để quyết định có nên thay đổi cách làm của công ty mình hay không. Một chủ đề đơn thuần không định hướng được việc tìm kiếm và sẽ tạo ra báo cáo thiếu trọng tâm. Sau đó, hãy xác minh những trích dẫn quan trọng.

## Soạn thảo: Bản giao việc đầy đủ

Soạn thảo cần bản giao việc đầy đủ gồm năm thành phần từ mục tiêu 1.1: đối tượng đọc, mục đích, giọng văn, độ dài và định dạng. Bổ sung tài liệu mẫu khi văn phong của tổ chức là yếu tố quan trọng, vì ví dụ là một trong những cách đáng tin cậy nhất để định hướng định dạng, giọng văn và cấu trúc. Với lá thư về khoản phí, người quản lý nêu người đọc là các chủ nhà và đính kèm một lá thư trước đây. Hãy dự trù việc tinh chỉnh qua nhiều vòng theo mục tiêu 1.3. Với nội dung dài, thực hiện theo từng giai đoạn như mục tiêu 1.2: dàn ý trước, sau đó từng phần.

## Động não: Mở rộng trước, thu hẹp sau

Động não đảo ngược cách tiếp cận của soạn thảo: trước tiên mở rộng, yêu cầu số lượng và sự đa dạng, chẳng hạn 20 ý tưởng, trong đó có một số ý tưởng khác thường. Muốn vượt qua các ý tưởng hiển nhiên, hãy yêu cầu rõ điều đó thay vì để Claude tự suy ra. Tạm hoãn đánh giá, vì các ràng buộc chặt chẽ làm giảm sự đa dạng — vốn là mục đích của hoạt động này. Sau đó hội tụ ở bước thứ hai: áp dụng tiêu chí, lập danh sách rút gọn và phát triển các ý tưởng được giữ lại. Người quản lý yêu cầu 20 cách thu hút chủ nhà và để thông tin ngân sách đến bước chọn danh sách rút gọn mới đưa vào. Cách này biến Claude thành một đối tác phát triển ý tưởng thực thụ thay vì công cụ chỉ tạo ra ba đề xuất an toàn.

## Thói quen xác định loại nhiệm vụ

Hãy gọi tên loại nhiệm vụ, rồi chọn cấu trúc giao việc phù hợp.

| Loại nhiệm vụ | Cấu trúc giao việc |
| --- | --- |
| Phân tích | Tài liệu cùng câu hỏi. |
| Nghiên cứu | Câu hỏi có phạm vi rõ ràng, yêu cầu trích dẫn. |
| Soạn thảo | Bản giao việc đầy đủ cùng quá trình tinh chỉnh. |
| Động não | Mở rộng trước, thu hẹp sau. |

## Trong bài thi

Hướng dẫn thi nêu bốn loại nhiệm vụ này. Kỹ năng được kiểm tra là xác định đúng loại: đọc tình huống tại nơi làm việc, gọi tên loại nhiệm vụ và giao việc theo cấu trúc phù hợp. Đáp án sai áp dụng nhầm cách tiếp cận: động não bị ràng buộc quá chặt, nghiên cứu chỉ có một dòng chủ đề, phân tích không đính kèm tài liệu và soạn thảo không nêu người đọc. Trường hợp cuối là đáp án sai thường lặp lại với nhiệm vụ soạn thảo. Chọn tính năng sản phẩm hoặc mô hình để sử dụng thuộc Lĩnh vực 3; mục tiêu này tập trung vào phần giao việc sau khi đã chọn.

### Cẩn thận với việc áp dụng nhầm cách tiếp cận

Phần lớn câu hỏi giấu lỗi trong một kế hoạch có vẻ hợp lý nhưng dùng cấu trúc giao việc đúng cho sai loại nhiệm vụ. Hãy kiểm tra riêng từng phần trong phương án gồm nhiều nhiệm vụ: chỉ một chỗ áp dụng nhầm, chẳng hạn đưa ràng buộc vào giai đoạn mở rộng ý tưởng khi động não, cũng khiến phương án đó sai.

Trình tự **mở rộng rồi hội tụ (diverge-then-converge)** trong động não là phương pháp điều phối hoạt động nhóm phổ biến được áp dụng cho Claude, không phải quy tắc từ tài liệu hướng dẫn sản phẩm.

## Những bẫy thường gặp trong bài thi

### Yêu cầu phân tích nhưng không nêu các câu hỏi cần trả lời

Tài liệu không kèm câu hỏi sẽ dẫn đến bản mô tả dữ liệu thay vì phân tích. Bản giao việc chuyên nghiệp cung cấp tài liệu, câu hỏi và quyết định sẽ dựa vào kết quả, đồng thời yêu cầu các phát hiện, bằng chứng và những hạn chế hoặc điểm cần lưu ý.

### Bắt đầu động não bằng các ràng buộc chặt và số lượng hướng đi được chấp nhận đã cố định

Ràng buộc áp dụng ở giai đoạn mở rộng sẽ loại bỏ chính sự đa dạng mà hoạt động cần tạo ra. Tiêu chí nên nằm ở giai đoạn hội tụ, nơi chúng giúp rút gọn một tập ý tưởng rộng thay vì bóp nghẹt ý tưởng từ trước khi xuất hiện.

### Giao việc nghiên cứu bằng một chủ đề thay vì câu hỏi có phạm vi rõ ràng

Chủ đề không xác định phạm vi sẽ tạo ra báo cáo thiếu trọng tâm. Câu hỏi nghiên cứu nêu phạm vi, góc tiếp cận và quyết định mà kết quả phải hỗ trợ, qua đó chỉ rõ cần tìm hiểu điều gì và các trích dẫn phải làm bằng chứng cho điều gì.

## Tình huống luyện tập

Một nhân viên hành chính của khoa đại học có bốn nhiệm vụ trong tuần này: tìm hiểu vì sao số người tham dự các buổi học hướng dẫn giảm trong học kỳ; tìm hiểu cách ba trường đại học khác tổ chức ngày hội tư vấn tuyển sinh; viết thư chào đón sinh viên đầu học kỳ mới; và tạo ý tưởng tăng lượng người tham dự ngày hội tư vấn tuyển sinh. Cô dự định dùng Claude cho cả bốn việc. Kế hoạch làm việc nào ghép đúng chiến lược với từng nhiệm vụ?

**Phương án A**

Đính kèm dữ liệu tham dự và nêu các câu hỏi cho phần phân tích; giao cho Research một câu hỏi có phạm vi rõ ràng về ngày hội tư vấn tuyển sinh; giao việc viết thư đầy đủ, dùng thư năm trước làm mẫu; và yêu cầu nhiều ý tưởng đa dạng trước khi lập danh sách rút gọn.

**Phương án B**

Dùng Research cho mọi nhiệm vụ, vì nguồn có trích dẫn nâng chất lượng của mọi đầu ra và một phương pháp thống nhất sẽ dễ quản lý hơn trong một tuần bận rộn.

**Phương án C**

Chỉ dùng Claude cho lá thư và các ý tưởng, còn tự thực hiện phân tích mức độ tham dự và nghiên cứu ngày hội tư vấn tuyển sinh vì hai nhiệm vụ đó đòi hỏi khả năng phán đoán thực sự.

**Phương án D**

Hỏi Claude vì sao tỷ lệ tham dự thường giảm ở các trường đại học nói chung; trả lời phần so sánh ngày hội tư vấn tuyển sinh bằng một lượt tìm kiếm web nhanh; gửi yêu cầu một dòng cho lá thư chào đón; và ngay từ đầu yêu cầu đúng ba ý tưởng an toàn, hợp lý.

## Bài tập thực hành: Giao việc cho cả bốn loại nhiệm vụ

**Thời gian:** 30 phút.

### Bạn sẽ học được

- Cách nhận biết loại nhiệm vụ trong một công việc thực tế.
- Cách giao việc phân tích với tài liệu, câu hỏi và quyết định mà kết quả hỗ trợ.
- Cách xác định phạm vi câu hỏi nghiên cứu, có góc tiếp cận và mục đích.
- Cách mở rộng ý tưởng khi bắt đầu động não rồi hội tụ ở bước thứ hai.

### Bước 1 — Liệt kê bốn công việc thực tế trong tuần của bạn

Mỗi loại một việc: một nhiệm vụ phân tích, một câu hỏi nghiên cứu, một tài liệu cần soạn và một vấn đề cần ý tưởng.

**Vì sao:** Thói quen xác định loại nhiệm vụ chỉ hình thành khi gắn với công việc thật. Trên giấy, bốn loại có vẻ rõ ràng nhưng trong thực tế dễ bị lẫn.

**Kết quả cần thấy:** Bốn mô tả nhiệm vụ, mỗi mô tả dài một dòng và có nhãn loại nhiệm vụ.

### Bước 2 — Viết bản giao việc phân tích

Đính kèm tài liệu thực tế, rồi nêu các câu hỏi phải trả lời và quyết định sẽ dựa vào kết quả.

**Vì sao:** Tài liệu cùng câu hỏi là yếu tố phân biệt phân tích với mô tả dữ liệu.

**Kết quả cần thấy:** Một bản giao việc có đính kèm tệp thật cùng hai hoặc ba câu hỏi cụ thể.

### Bước 3 — Viết bản giao việc nghiên cứu

Diễn đạt thành một câu hỏi có phạm vi rõ ràng, có góc tiếp cận và mục đích. Ghi lại việc đó có cần Research hay chỉ cần tìm kiếm web nhanh.

**Vì sao:** Câu hỏi có phạm vi rõ ràng định hướng việc tìm kiếm. Chủ đề đơn thuần tạo ra báo cáo thiếu trọng tâm.

**Kết quả cần thấy:** Một câu hỏi nghiên cứu nêu phạm vi, góc tiếp cận và quyết định mà kết quả phải hỗ trợ, kèm một dòng yêu cầu sử dụng công cụ.

### Bước 4 — Viết bản giao việc soạn thảo và động não

Với soạn thảo, dùng đủ năm thành phần cùng tài liệu mẫu. Với động não, yêu cầu số lượng và sự đa dạng, tạm thời chưa đưa tiêu chí sàng lọc vào.

**Vì sao:** Hai cấu trúc này đối lập nhau: soạn thảo cần đặc tả đầy đủ, còn động não cần chủ động để mở.

**Kết quả cần thấy:** Một bản giao việc soạn thảo đầy đủ, có tài liệu mẫu đính kèm; và một yêu cầu động não đưa ra 20 ý tưởng, bao gồm các ý tưởng khác thường.

### Bước 5 — Chạy cả bốn yêu cầu và ghi nhận nguy cơ phải làm lại

Sau đó, ghi lại những chỗ mà cấu trúc giao việc không phù hợp có thể khiến bạn tốn thêm một vòng làm lại.

**Vì sao:** Nhìn thấy chi phí của việc áp dụng nhầm cách tiếp cận ngay trong công việc của mình giúp thói quen xác định loại nhiệm vụ trở nên bền vững.

**Kết quả cần thấy:** Bốn đầu ra cùng một ghi chú ngắn cho mỗi nhiệm vụ, nêu lỗi áp dụng nhầm mà bạn đã tránh được.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Sử dụng Research trên Claude — *Use research on Claude*.
- Khi nào nên dùng tìm kiếm web, suy nghĩ mở rộng và Research? — *When should I use web search, extended thinking, and research?*
- Tôi có thể dùng Claude vào những việc gì? — *What are some things I can use Claude for?*
- Tải tệp lên Claude — *Upload files to Claude*.
- Các phương pháp tốt nhất khi viết prompt — *Prompting best practices*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [1.3 — Tinh chỉnh prompt qua nhiều vòng để cải thiện đầu ra](1-3-prompt-iteration.vi.md).
- **Bài tiếp theo:** Đánh giá độ chính xác và tính đầy đủ của đầu ra — *Evaluating Outputs for Accuracy and Completeness*.
