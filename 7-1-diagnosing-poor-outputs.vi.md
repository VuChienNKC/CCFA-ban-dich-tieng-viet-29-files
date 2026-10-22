# 7.1 — Chẩn đoán và xử lý prompt kém hiệu quả, đầu ra chưa đạt

- **Lĩnh vực (Domain):** 7
- **Nhiệm vụ (Task):** 7.1
- **Tên bài gốc:** Diagnosing and Resolving Underperforming Prompts and Poor Outputs
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/7-troubleshooting-optimisation/7-1-diagnosing-poor-outputs)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

**Đầu ra chưa đạt** là câu trả lời không đáp ứng điều yêu cầu cần. **Chẩn đoán** là gọi tên vì sao yêu cầu trông hợp lý lại tạo kết quả đó, trước khi thay đổi gì. Cấu hình Project gồm chỉ dẫn và kiến thức.

Chủ hiệu sách độc lập có Project cho bản tin sách mới hằng tuần, còn thẻ giới thiệu sách trên kệ làm một lần được yêu cầu trong chat thông thường.

## Câu hỏi định hướng chẩn đoán

Câu hữu ích nhất: điều đó xảy ra một lần hay lần nào cũng vậy? Tóm tắt nhạt từ một yêu cầu thiếu thông tin là vấn đề prompt, sửa bằng bản giao việc tốt hơn. Cùng giọng văn, định dạng hay giả định sai trong mọi đầu ra của cùng Project là vấn đề cấu hình. Dấu hiệu là từ **“mọi”**. Chỉ dẫn hoặc kiến thức tạo ra lỗi, nên sửa cấu hình một lần. Sửa tay từng đầu ra khiến phải trả cùng chi phí mãi.

Một thẻ sách nhạt cần bản giao việc tốt hơn. Giọng cứng nhắc ở mọi bản tin cần sửa một lần trong chỉ dẫn Project.

## Danh sách nguyên nhân kiểm tra được trong một phút

Sáu nguyên nhân bao quát gần như mọi trường hợp:

- Thiếu ngữ cảnh.
- Quá tải chỉ dẫn.
- Lỗi cấu hình.
- Cuộc trò chuyện không còn hiệu quả.
- Tài liệu lỗi thời hoặc đã bị thay thế.
- Tính năng hay thiết lập không phù hợp.

Thiếu ngữ cảnh phổ biến nhất. Yêu cầu không có người đọc, mục đích, tài liệu nguồn chỉ tạo nội dung chung chung vì Claude không đoán được điều bị giữ lại. Trung tâm trợ giúp khuyên cung cấp càng nhiều bối cảnh càng tốt, như hướng dẫn người không biết gì về nhiệm vụ. Bổ sung điều thiếu. Yêu cầu mạnh giọng hơn không thêm thông tin. Thẻ sách cần người đọc, mục đích và lời giới thiệu cuốn sách.

Tiếp theo là quá tải. Yêu cầu mang cả chục điều kiện sẽ bỏ sót vài điều. Cách được hướng dẫn là tổ chức lại: chia yêu cầu phức tạp thành bước nhỏ, nhóm và ưu tiên để yêu cầu quan trọng không bị chìm. Gửi lại cùng danh sách và viết hoa mục bị bỏ sót không thêm gì mới. Bản giao việc bản tin liên tục thiếu giờ mở cửa cần được chia, sắp ưu tiên.

## Khi chính cuộc trò chuyện là vấn đề

Chat dài tích lũy nháp bị thay thế, lần sửa sau đó bị phủ định và chủ đề không liên quan. Claude phải làm việc với tất cả. Cuối cùng chat chạm giới hạn độ dài. Cuộc trò chuyện dài kích hoạt quản lý ngữ cảnh tự động cũng tiêu thụ nhiều hạn mức hơn. Hướng dẫn được ghi nhận: chia nội dung, tóm tắt phần quan trọng hoặc mở chat mới. Project xử lý tài liệu lớn lặp lại bằng truy xuất. Cách sửa chat không còn hiệu quả là chat mới mang bản tóm tắt đã xác minh về điều còn quan trọng. Chat chứa ba bản tin nháp bắt đầu lại từ bản tóm tắt.

## Các kiểu lỗi Anthropic nêu

Bài khắc phục trong Trung tâm trợ giúp nêu các triệu chứng. Câu trả lời sai hoặc gây hiểu lầm gồm trích dẫn bịa trông có vẻ đúng. Claude không phải nguồn sự thật duy nhất, nên xem kỹ khẳng định hệ trọng và nguồn trích, như câu nói của tác giả trong bản tin. **Bịa đặt khả năng** là liên kết trông dùng được nhưng không hoạt động hoặc tuyên bố đã gửi email. Claude không truy cập email hay phần mềm chưa được tích hợp rõ ràng. Chẩn đoán là khả năng bị bịa, không phải thư cần theo dõi.

Câu trả lời quá ngắn là vấn đề prompt: điều chỉnh lại. Đưa prompt và câu trả lời trước cho Claude để tiếp tục từ nơi dừng. Thông báo lỗi không phải lỗi chất lượng. Thông báo quá tải hệ thống nghĩa là chờ rồi thử lại. Thông báo giới hạn độ dài nghĩa là chia, tóm tắt hoặc bắt đầu mới. Một nửa công việc chẩn đoán là nhận ra triệu chứng thuộc loại nào vì mỗi loại có cách sửa riêng.

## Phản xạ nâng cấp

Bẫy hay gặp nhất là chọn mô hình mạnh nhất hoặc mức nỗ lực cao hơn vì thất vọng. Bản giao việc mơ hồ thất bại ở mọi cấp: mô hình nào cũng thiếu cùng bối cảnh. Nâng cấp mua cùng câu trả lời chung chung nhưng kỹ hơn, tốn hơn; thẻ sách vẫn nhạt. Đổi tính năng, thiết lập hợp lý khi nhiệm vụ cần chiều sâu — mức nỗ lực, suy nghĩ mở rộng — hoặc thông tin ngoài hiện thời — web, Research. Chỉ dùng sau khi bản giao việc đã tốt.

## Trong bài thi

Mọi câu trong lĩnh vực này bắt đầu sau khi có vấn đề. Viết yêu cầu tốt là Lĩnh vực 1; chẩn đoán kết quả kém là lĩnh vực này. Sửa cấu hình thuộc Lĩnh vực 5; nhận ra cần sửa là kỹ năng ở đây. Thí sinh mất điểm vì tìm cách sửa trước khi gọi tên nguyên nhân.

### Khái niệm cốt lõi

Phân loại triệu chứng trước khi đọc phương án: một lần hay mọi lần, thuộc kiểu lỗi nào. Đáp án đúng sửa nguyên nhân. Ít nhất một phương án xử lý biểu hiện, thường viết lại prompt vốn không phải vấn đề.

### Những gì nguồn không nói

Không nguồn chính thức nào nói chat dài chậm hơn hoặc Claude nhầm lẫn các chủ đề. Lý do bắt đầu mới dựa trên điều tài liệu thực sự ghi nhận.

## Những bẫy thường gặp trong bài thi

### Viết lại prompt hôm nay khi phần dẫn nói mọi đầu ra đều cùng lỗi

Lỗi ở mọi đầu ra cùng loại xuất phát thiết lập. Sửa chỉ dẫn hoặc kiến thức một lần. Viết lại từng prompt, sửa tay từng đầu ra trả cùng chi phí mãi và để nguyên nguyên nhân.

### Nâng mô hình hoặc mức nỗ lực ngay khi thất vọng

Nếu chưa nêu người đọc, đính kèm tài liệu, nâng cấp trả cùng câu chung chung chậm và tốn hơn. Chẩn đoán trước: bản giao việc thiếu cần bổ sung bối cảnh; không cấp nào đoán được điều chưa cung cấp.

### Xem thông báo lỗi là lỗi chất lượng rồi đổi câu chữ

Thông báo quá tải, giới hạn độ dài có cách xử lý được ghi nhận: chờ ngắn rồi thử lại hoặc chia, tóm tắt, mở mới. Đổi câu chữ trả lời một vấn đề hệ thống không đặt ra.

### Theo dõi email Claude tuyên bố đã gửi

Không có tích hợp rõ ràng, Claude không truy cập email hay phần mềm đó. Tuyên bố gửi là bịa khả năng, không phải lỗi chuyển thư. Kiểm tra thư đi hoặc yêu cầu gửi lại là truy đuổi việc chưa diễn ra.

## Tình huống luyện tập

Nhân viên hành chính phòng tranh nhỏ soạn thư đề nghị mượn tác phẩm trong Project thư từ. Hai tháng qua, mọi thư đều dùng chính tả Mỹ; cô sửa tay trước khi gửi. Mô hình mạnh hơn vẫn vậy. Cô muốn dừng sửa tay và tiếp tục dùng Project. Bước tiếp theo phù hợp nhất là gì?

**Phương án A**

Tiếp tục sửa tay vì mỗi lần chỉ mất vài phút, các phần khác đã đúng ý.

**Phương án B**

Rà chỉ dẫn và kiến thức Project để tìm nguyên nhân, nêu chuẩn chính tả ở đó một lần.

**Phương án C**

Chuyển Project sang mô hình mạnh hơn để đúng chính tả ngay lần đầu, không cần sửa tay.

**Phương án D**

Soạn thư sau trong chat mới ngoài Project để thiết lập Project không ảnh hưởng chính tả.

## Bài tập thực hành: Chẩn đoán lần thất vọng gần nhất

**Thời gian:** 25 phút.

### Bạn sẽ học được

- Định hướng triệu chứng bằng câu hỏi một lần hay mọi lần.
- Kiểm tra danh sách nguyên nhân trước khi sửa prompt.
- Nhận diện kiểu lỗi Anthropic ghi nhận.
- Áp dụng một cách sửa và xem triệu chứng có thay đổi.

### Bước 1 — Tìm công việc Claude gần nhất khiến bạn thất vọng

Chưa viết lại gì cho đến khi chẩn đoán xong.

**Vì sao:** Kỷ luật cốt lõi là gọi nguyên nhân trước sửa. Viết lại ngay là phản xạ bài tập điều chỉnh.

**Kết quả cần thấy:** Đầu ra và yêu cầu tạo nó đặt cạnh nhau, chưa thay đổi.

### Bước 2 — Hỏi câu định hướng trước

Xảy ra một lần hay mọi lần làm loại việc này?

**Vì sao:** Lỗi riêng lẻ hướng đến yêu cầu hoặc chat; lỗi lặp hướng đến thiết lập. Hai chẩn đoán dẫn đến cách sửa hoàn toàn khác.

**Kết quả cần thấy:** Ghi “một lần” hoặc “mọi lần”.

### Bước 3 — Nếu một lần, kiểm tra danh sách nguyên nhân

Thiếu bối cảnh, quá nhiều yêu cầu, chat quá dài, tài liệu bị thay thế hoặc nhiệm vụ cần tính năng, thiết lập mà câu chữ không cung cấp được.

**Vì sao:** Danh sách ngắn thực hiện được tốt hơn tìm vô hạn. Phần lớn lỗi riêng lẻ thiếu bối cảnh; danh sách ngăn bỏ sót nguyên nhân ít gặp.

**Kết quả cần thấy:** Một nguyên nhân được nêu tên với một câu bằng chứng.

### Bước 4 — Nếu mọi lần, mở chỉ dẫn và kiến thức Project

Tìm dòng gây lỗi hoặc dòng còn thiếu.

**Vì sao:** Lỗi lặp được cấu hình tạo ra. Bằng chứng nằm ở chỉ dẫn, kiến thức, không phải từng chat riêng.

**Kết quả cần thấy:** Dòng có vấn đề được xác định hoặc ghi chuẩn cần thiết chưa từng được nêu.

### Bước 5 — Áp dụng một cách sửa theo chẩn đoán và chạy lại cùng yêu cầu

Ghi triệu chứng có thay đổi không trước khi đụng điều khác.

**Vì sao:** Đổi một điều rồi kiểm tra biến dự đoán thành chẩn đoán. Nếu triệu chứng đổi, đã tìm nguyên nhân; nếu không, danh sách vẫn mở.

**Kết quả cần thấy:** Cặp đầu ra trước, sau và kết luận một dòng về hiệu quả cách sửa.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Prompt không tạo câu trả lời hữu ích — *My prompt isn't giving me a helpful answer*.
- Claude trả lời sai hoặc gây hiểu lầm. Chuyện gì xảy ra? — *Claude is providing incorrect or misleading responses. What's going on?*
- Claude tạo liên kết không hoạt động, tuyên bố sai đã gửi email hoặc tạo tài liệu ngoài — *Claude is producing links that don't work and falsely claiming that it has sent emails or produced external documents*.
- Câu trả lời quá ngắn — *Claude's response to my prompt is too brief*.
- Khắc phục thông báo lỗi Claude — *Troubleshoot Claude error messages*.
- Hạn mức sử dụng và giới hạn độ dài — *How do usage and length limits work?*
- Đổi mô hình, mức nỗ lực, thiết lập suy nghĩ — *Change the model, effort, and thinking settings*.
- Khi nào dùng web, suy nghĩ mở rộng và Research? — *When should I use web search, extended thinking, and research?*

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [6.4 — Hiểu những hệ quả đạo đức của việc sử dụng AI](6-4-ethical-implications.vi.md).
- **Bài tiếp theo:** [7.2 — Điều chỉnh cách làm dựa trên phản hồi và kết quả](7-2-adjusting-from-feedback.vi.md).
