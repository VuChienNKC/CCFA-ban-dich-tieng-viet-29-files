# 2.2 — Nhận diện thông tin bịa đặt, sự thiếu nhất quán và thiên lệch

- **Lĩnh vực (Domain):** 2
- **Nhiệm vụ (Task):** 2.2
- **Tên bài gốc:** Identifying Hallucinations, Inconsistencies and Bias
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/2-output-evaluation/2-2-hallucinations-inconsistencies-bias)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Mục tiêu 2.1 đã giới thiệu cách tiếp cận của người rà soát. Mục tiêu này gọi tên ba loại lỗi cần tìm khi rà soát. **Thông tin bịa đặt hay “ảo giác” (hallucination)** là nội dung nghe có vẻ thuyết phục nhưng không có căn cứ thực tế. **Sự thiếu nhất quán (inconsistency)** xảy ra khi đầu ra tự mâu thuẫn. **Thiên lệch (bias)** là cách định khung vấn đề, các giả định hoặc ngôn ngữ bị lệch. Mỗi loại có dấu hiệu nhận biết và cần một cách xử lý khác nhau.

Người quản lý một trung tâm kinh doanh cây cảnh và vật tư làm vườn giao cho Claude ba việc trong một tuần: hướng dẫn các bước tạo báo cáo tồn kho trong hệ thống bán hàng tại quầy, viết bản tóm tắt doanh số mùa xuân có bảng số liệu và soạn ghi chú đánh giá nhân viên thời vụ. Mỗi công việc đều có thể gặp một trong ba loại lỗi này.

## Thông tin bịa đặt: Trôi chảy, cụ thể nhưng được dựng lên

Trung tâm trợ giúp cho biết Claude “đôi khi có thể tạo ra câu trả lời sai hoặc gây hiểu lầm”. Claude cũng “có thể đưa ra các trích dẫn trông có vẻ đáng tin hoặc nghe thuyết phục nhưng không có căn cứ thực tế”. Cụm cuối chính là định nghĩa dùng trong bài này. Thông tin bịa đặt không nhất thiết mơ hồ hay dè dặt. Nó có thể xuất hiện dưới dạng một con số trông rất chính xác, một nguồn được nêu tên hoặc danh sách các bước được đánh số. Chi tiết bịa ra được trình bày với mức độ tự tin giống hệt chi tiết thật, nên sự cụ thể không phải là bằng chứng. Với mọi chi tiết, hãy hỏi: “Thông tin này có thể đến từ đâu?” Câu hỏi “Nghe có đúng không?” chỉ kiểm tra vẻ tự tin của cách trình bày.

Claude cũng có thể bịa ra chính khả năng của mình. Một bài viết khác trong Trung tâm trợ giúp cảnh báo rằng Claude có thể tuyên bố sai rằng nó đã gửi email, tạo tài liệu bên ngoài cuộc trò chuyện hoặc cung cấp liên kết hoạt động được. Claude không có quyền truy cập email hay chức năng truyền tệp nếu những khả năng đó chưa được tích hợp rõ ràng. Tuyên bố rằng Claude đã làm việc gì đó bên ngoài cuộc trò chuyện là điều cần kiểm tra, chưa phải xác nhận công việc đã được thực hiện. Nếu Claude nói đã gửi email số liệu tồn kho cho nhà cung cấp, người quản lý cần kiểm tra với nhà cung cấp.

## Rủi ro tập trung ở đâu?

Rủi ro bịa đặt phụ thuộc vào mức độ có căn cứ của thông tin. Rủi ro cao nhất ở những nơi Claude có ít cơ sở nhất để làm việc:

- Các hệ thống và tài liệu nội bộ riêng của tổ chức mà Claude chưa từng được cung cấp.
- Những sự kiện rất gần đây, diễn ra sau thời điểm dữ liệu huấn luyện của Claude.
- Những con số chính xác không có trong tài liệu nguồn.

Dạng có rủi ro cao nhất là hướng dẫn được đánh số, trình bày đầy tự tin về một công cụ nội bộ mà Claude chưa từng được xem tài liệu. Hướng dẫn đó trôi chảy, cụ thể nhưng không dựa trên cơ sở nào. Các bước tạo báo cáo tồn kho thuộc dạng này. Claude nêu tên các trình đơn trong hệ thống bán hàng mà nó chưa từng được xem; một số trình đơn có thể không tồn tại. Claude càng ít có khả năng tiếp cận căn cứ thực tế thì mức độ cụ thể của câu trả lời càng ít giá trị.

## Sự thiếu nhất quán: Đầu ra tự mâu thuẫn

Không cần nguồn bên ngoài để phát hiện sự thiếu nhất quán. Các dạng thường gặp gồm: con số trong phần văn bản mâu thuẫn với bảng, khuyến nghị trái với kết quả phân tích và hai phần ghi ngày khác nhau cho cùng một sự kiện. Mâu thuẫn nội bộ là dấu hiệu cảnh báo về độ tin cậy của toàn bộ đầu ra, không chỉ là một lỗi đánh máy cần sửa. Quy trình đã tạo ra một lỗi nhìn thấy được cũng hoàn toàn có thể đã tạo ra những lỗi chưa nhìn thấy. Vì vậy, hãy xác minh lại toàn bộ đầu ra bằng cách đối chiếu với nguồn, thay vì chỉ sửa chỗ không khớp bạn nhận ra rồi gửi phần còn lại. Nếu phần văn bản và bảng trong báo cáo doanh số mùa xuân đưa ra số liệu khác nhau về phân compost, người quản lý cần kiểm tra cả bản tóm tắt dựa trên dữ liệu của hệ thống bán hàng.

## Thiên lệch: Nhìn vào khuôn mẫu xuyên suốt

Thiên lệch gây hậu quả đáng kể nhất trong các đầu ra liên quan đến con người: tài liệu tuyển dụng, đánh giá nhân sự, mô tả khách hàng và mọi nội dung xếp hạng hoặc nhận xét đặc điểm của các nhóm người. Chính sách sử dụng của Anthropic cho thấy mức độ hệ trọng khi xem các quyết định về việc làm, nhà ở, tài chính và chăm sóc sức khỏe đối với cá nhân là những trường hợp sử dụng có rủi ro cao. Sự thiên lệch nằm trong khuôn mẫu xuyên suốt, nên hãy so sánh giữa các mô tả thay vì chỉ đọc từng câu riêng lẻ. Giả sử phần đánh giá mô tả nhân viên lớn tuổi bằng sự đáng tin cậy, còn nhân viên trẻ bằng khả năng đổi mới. Không câu riêng lẻ nào có vấn đề rõ ràng, nhưng toàn bộ đầu ra vẫn có thiên lệch. Hãy tìm ngôn ngữ ngầm mang định kiến và các giả định không được nói ra về tuổi tác, giới tính, xuất thân hoặc năng lực. Sau đó áp dụng phép thử đọc thành tiếng: cách mô tả ấy có còn phù hợp nếu được đọc trực tiếp cho chính nhóm người mà nó đang mô tả hay không?

## Trong bài thi

Bài thi kiểm tra khả năng phân biệt ba loại lỗi và xử lý đúng từng loại, vì cách xử lý của chúng khác nhau. Với sự thiếu nhất quán, điểm được kiểm tra là cách phản ứng: xác minh lại toàn bộ đầu ra. Các phương án gây nhiễu áp dụng nhầm cách xử lý: chỉ vá một mâu thuẫn, xóa một từ mang định kiến hoặc yêu cầu Claude xác nhận chính các bước nó đã bịa ra.

### Ghép cách xử lý với loại lỗi

Thông tin bịa đặt cần được xác minh bằng nguồn có thẩm quyền. Sự thiếu nhất quán dẫn đến việc xác minh lại toàn bộ đầu ra. Thiên lệch cần được chỉnh sửa ở cấp độ khuôn mẫu xuyên suốt tài liệu. Một câu hỏi đơn thuần như “Điều này có đúng không?” không phải là một phép kiểm tra. Anthropic ghi nhận hai cách kiểm tra: chạy lại yêu cầu rồi so sánh với đầu ra đầu tiên; và gửi chỉ dẫn tiếp nối yêu cầu Claude xác minh các phát biểu trước đó, đánh dấu những điểm không hợp lý hoặc không khớp. Mỗi cách tạo ra một danh sách cần đối chiếu với nguồn. Với các bước tạo báo cáo tồn kho, nguồn đó là tài liệu hướng dẫn của hệ thống bán hàng.

## Những bẫy thường gặp trong bài thi

### Tin vào hướng dẫn từng bước đầy tự tin cho hệ thống nội bộ riêng

Claude không có quyền truy cập phần mềm nội bộ của tổ chức nếu tài liệu về phần mềm đó chưa được cung cấp trong cuộc trò chuyện. Vì vậy, sự cụ thể thiếu căn cứ là dạng bịa đặt có rủi ro cao nhất. Đáp án đúng xem các bước này là chưa được xác minh và tìm đến tài liệu chính thức của hệ thống.

### Tin lời Claude tuyên bố đã gửi email hoặc tạo tệp bên ngoài

Claude có thể bịa ra khả năng của mình và không có quyền truy cập những công cụ chưa được tích hợp. Do đó, tuyên bố hoàn thành cũng là một phát biểu cần kiểm tra như mọi phát biểu khác. Đáp án đúng xác minh rằng hành động thực sự đã diễn ra thay vì xem lời tuyên bố là xác nhận.

### Sửa một mâu thuẫn đã phát hiện rồi gửi phần còn lại

Sự thiếu nhất quán nội bộ là bằng chứng cho thấy quy trình tạo đầu ra đã sai ở đâu đó, nên cần xác minh lại toàn bộ đầu ra bằng cách đối chiếu với nguồn. Sửa mang tính hình thức vẫn giữ nguyên một tài liệu đã cho thấy bạn không thể tin từng dòng mà không kiểm tra.

### Xem thiên lệch là một từ không phù hợp cần xóa

Thiên lệch nằm trong khuôn mẫu xuyên suốt các mô tả: ai bị kèm những nhận xét dè dặt, thành tích của ai bị diễn đạt theo cách giảm nhẹ và những nhóm nào được mô tả bằng các tiêu chí khác nhau. Xóa một cụm từ mang định kiến vẫn để nguyên sự thiên lệch, nên đáp án đúng điều chỉnh khuôn mẫu mô tả chứ không chỉ một từ.

## Tình huống luyện tập

Người quản lý một phòng khám da liễu hỏi Claude cách tạo báo cáo nhắc bệnh nhân tái khám hằng tháng trong phần mềm quản lý của phòng khám. Claude chưa từng được truy cập phần mềm này hoặc bất kỳ tài liệu nào viết về nó, nhưng vẫn trả lời bằng các bước được đánh số đầy tự tin, nêu tên cụ thể các trình đơn và nút bấm. Người quản lý vẫn muốn dùng Claude cho những công việc khác liên quan đến phần mềm này. Cô nên xử lý các bước đó thế nào?

**Phương án A**

Làm theo đúng các bước đã viết: mức độ chi tiết đến tận tên trình đơn và nút bấm cho thấy Claude có kiến thức đáng tin cậy về phần mềm này.

**Phương án B**

Ngừng dùng Claude cho mọi công việc liên quan đến phần mềm của phòng khám, vì nó vừa cho thấy sẽ bịa ra hướng dẫn nghe có vẻ hợp lý thay vì thừa nhận không biết câu trả lời.

**Phương án C**

Yêu cầu Claude kiểm tra lại từng bước bằng cách đối chiếu với phần mềm của phòng khám và xác nhận tất cả đều đúng trước khi thử, để không chi tiết bịa đặt nào lọt qua.

**Phương án D**

Xem các bước là chưa được xác minh và kiểm tra tài liệu của nhà cung cấp phần mềm hoặc phần trợ giúp tích hợp sẵn.

## Bài tập thực hành: Rà soát cả ba loại lỗi

**Thời gian:** 30 phút.

### Bạn sẽ học được

- Cách phân biệt các phát biểu có thể truy nguyên nguồn gốc với những phát biểu chưa được xác minh.
- Cách xử lý khi đầu ra tự mâu thuẫn.
- Cách so sánh các mô tả về con người để nhận ra khuôn mẫu thiên lệch.
- Cách ghép cách xử lý phù hợp với từng loại lỗi.

### Bước 1 — Thu thập ba đầu ra thực tế của Claude trong công việc

Chọn một đầu ra đưa ra các phát biểu về sự thật, một đầu ra có cùng những con số xuất hiện ở nhiều chỗ và một đầu ra mô tả hoặc so sánh con người.

**Vì sao:** Mỗi dạng đầu ra là nơi thường xuất hiện một loại lỗi, nên việc rà soát giúp bạn học nhận diện cả ba dạng trên tài liệu thực tế.

**Kết quả cần thấy:** Ba đầu ra đã được mở và sẵn sàng: tài liệu chứa các phát biểu về sự thật, tài liệu số liệu và tài liệu về con người.

### Bước 2 — Rà soát thông tin bịa đặt

Gạch chân mọi chi tiết cụ thể không đến từ tài liệu bạn đã cung cấp: số liệu, tên, tài liệu tham chiếu và hướng dẫn. Đánh dấu từng chi tiết là “có thể truy nguyên nguồn gốc” hoặc “chưa được xác minh”.

**Vì sao:** Sự cụ thể là đặc trưng thường thấy của thông tin bịa đặt. Vì vậy, mọi chi tiết cụ thể thiếu căn cứ đều là một trường hợp đáng nghi cho đến khi truy được nguồn gốc.

**Kết quả cần thấy:** Một đầu ra có chú thích, trong đó mọi chi tiết cụ thể đều được gắn một trong hai nhãn.

### Bước 3 — Rà soát sự thiếu nhất quán

So sánh mọi con số, ngày tháng và kết luận xuất hiện nhiều lần. Nếu hai lần xuất hiện không khớp, hãy đánh dấu toàn bộ đầu ra là cần xác minh lại.

**Vì sao:** Khả năng phán đoán được kiểm tra ở đây là nhận ra một mâu thuẫn làm giảm độ tin cậy của quy trình, không chỉ của câu chứa nó.

**Kết quả cần thấy:** Hoặc đối chiếu chéo không phát hiện vấn đề, hoặc toàn bộ đầu ra được đánh dấu cần xác minh lại; không dừng ở việc vá một con số đơn lẻ.

### Bước 4 — Rà soát thiên lệch

Đọc đối chiếu giữa các mô tả về con người thay vì chỉ đọc tuần tự từng mô tả. Ghi nhận liệu những người hoặc nhóm khác nhau có bị mô tả một cách có hệ thống bằng những tiêu chí khác nhau hay không.

**Vì sao:** Không cần có câu riêng lẻ nào rõ ràng không phù hợp thì toàn bộ đầu ra vẫn có thể có vấn đề. Chính khuôn mẫu mô tả là điều cần phát hiện.

**Kết quả cần thấy:** Một ghi chú về việc khuôn mẫu mô tả có vượt qua phép thử đọc thành tiếng hay không.

### Bước 5 — Ghi lại cách xử lý phù hợp cho từng vấn đề đã đánh dấu

Với mỗi vấn đề, viết cách xử lý đúng: xác minh bằng nguồn, xác minh lại toàn bộ đầu ra hoặc điều chỉnh khuôn mẫu mô tả.

**Vì sao:** Gọi tên cách xử lý giúp củng cố mối liên hệ mà bài thi kiểm tra: mỗi loại lỗi có cách khắc phục riêng.

**Kết quả cần thấy:** Kế hoạch xử lý dài ba dòng, mỗi loại lỗi một dòng.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Claude đang đưa ra câu trả lời sai hoặc gây hiểu lầm. Chuyện gì đang xảy ra? — *Claude is providing incorrect or misleading responses. What's going on?*
- Claude đang tạo các liên kết không hoạt động và tuyên bố sai rằng đã gửi email hoặc tạo tài liệu bên ngoài. Chuyện gì đang xảy ra? — *Claude is producing links that don't work and falsely claiming that it has sent emails or produced external documents. What's going on?*
- Dữ liệu huấn luyện của Claude được cập nhật đến đâu? — *How up-to-date is Claude's training data?*
- Giảm thông tin bịa đặt — *Reduce hallucinations*.
- Chính sách sử dụng — *Usage Policy*.
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** Đánh giá độ chính xác và tính đầy đủ của đầu ra — *Evaluating Outputs for Accuracy and Completeness*.
- **Bài tiếp theo:** [2.3 — Các kỹ thuật kiểm chứng sự thật và xác thực](2-3-fact-checking-validation.vi.md).
