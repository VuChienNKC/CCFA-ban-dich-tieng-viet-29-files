# 2.3 — Các kỹ thuật kiểm chứng sự thật và xác thực

- **Lĩnh vực (Domain):** 2
- **Nhiệm vụ (Task):** 2.3
- **Tên bài gốc:** Fact-Checking and Validation Techniques
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/2-output-evaluation/2-3-fact-checking-validation)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

**Xác thực (validation)** là kiểm tra các phát biểu trong đầu ra bằng cách đối chiếu với thứ có thể xác nhận chúng. Mục tiêu này cung cấp các công cụ cho quá trình rà soát ở mục tiêu 2.1, sắp xếp từ ít tốn công nhất đến cần nhiều công sức nhất. Một lớp phán đoán giúp quyết định mỗi đầu ra cần được kiểm tra kỹ đến mức nào. **Tài liệu sơ cấp (primary document)** là bản ghi gốc: ấn phẩm chính thức, văn bản của cơ quan quản lý, tiêu chí do bên tài trợ công bố hoặc hồ sơ của tổ chức.

Hãy xét một công ty chuyển nhà. Nhân viên văn phòng nhờ Claude soạn thư báo giá từ các ghi chép khảo sát và bảng giá đính kèm. Thư nêu tổng giá và quy định đỗ xe của chính quyền địa phương đối với tuyến phố đó. Claude cũng soạn các ý tưởng cho bản tin nội bộ.

Không nên xem Claude là nguồn sự thật duy nhất. Đầu ra có ảnh hưởng hệ trọng cần được xem xét kỹ. Claude có thể tạo ra nội dung trôi chảy, cụ thể, trông có vẻ đúng nhưng lại sai nghiêm trọng. Chỉ riêng sự cụ thể không chứng minh được độ chính xác.

## Bắt đầu từ cách ít tốn công nhất: Nguồn bạn đã cung cấp

Với đầu ra được xây dựng từ tài liệu đính kèm, việc kiểm tra đầu tiên là đối chiếu với chính tài liệu đó. Tài liệu đã có sẵn trong cuộc trò chuyện. Từng con số, từng phần và từng phát biểu hoặc khớp với nguồn, hoặc không. Đây là thói quen ở mục tiêu 2.1 được chuyển thành một kỹ thuật, và chỉ mất vài phút. Tổng giá được kiểm tra bằng ghi chép khảo sát và bảng giá. Chỉ chuyển sang cách kiểm tra tốn công hơn khi nguồn đã cung cấp không đủ để xác định vấn đề.

## Độc lập, có thẩm quyền và là nguồn sơ cấp

Các phát biểu về thông tin bên ngoài cần được kiểm tra từ bên ngoài. Tài liệu đính kèm không thể xác nhận quy định đỗ xe, vì thông tin đó không đến từ các tài liệu ấy. Câu trả lời dùng tìm kiếm web có trích dẫn “để bạn có thể dễ dàng tự kiểm tra nguồn”. Người dùng được khuyên đối chiếu chéo các nguồn được trích dẫn và dùng nguồn có thẩm quyền cho những quyết định quan trọng. Bài viết về thông tin bịa đặt trong Trung tâm trợ giúp khuyên rà soát các nguồn Claude trích dẫn, vì kiểm tra bản gốc giúp phát hiện cách diễn giải sai. Trích dẫn có mặt để bạn kiểm tra.

Tiêu chuẩn đối chiếu là tài liệu sơ cấp. Một bản tóm tắt khác do AI tạo, một bài đăng trên diễn đàn hoặc chính đầu ra trước đó của Claude không phải là xác thực độc lập. Phép kiểm tra kế thừa lỗi của nội dung đang được kiểm tra không chứng minh được điều gì. Với quy định đỗ xe, nguồn cần dùng là trang thông tin do chính quyền địa phương công bố. Tìm kiếm web ngay trong claude.ai là một cách hợp lệ để tiếp cận trang đó. Chính nguồn thực hiện vai trò xác thực, không phải thao tác tìm kiếm.

## Làm cho đầu ra có thể truy nguyên nguồn gốc

Đầu ra có thể truy nguyên nguồn gốc cho biết từng phát biểu đến từ đâu, nhờ đó có thể kiểm tra. Với đầu ra không thể truy nguyên, không nên mặc nhiên cho rằng nó đúng. Đối với tài liệu dài, hướng dẫn viết prompt của Anthropic khuyên yêu cầu Claude trích các phần liên quan từ nguồn trước khi thực hiện nhiệm vụ. Với công việc nghiên cứu, hướng dẫn khuyên yêu cầu Claude kiểm chứng thông tin qua nhiều nguồn. Với thư báo giá, hãy yêu cầu Claude chỉ ra nguồn của từng phát biểu và cách đi đến từng kết luận. Sau đó kiểm tra chọn lọc những điểm có ảnh hưởng lớn. Khi một con số duy nhất chi phối quyết định, hãy đối chiếu đa nguồn (triangulation): xác nhận con số đó ở hai nơi độc lập trước khi gửi đi.

## Kiểm tra tương xứng: Lớp phán đoán

Công sức xác thực cần tương xứng với hậu quả nếu thông tin sai. Khách hàng quyết định dựa trên tổng giá, nên tổng giá cần hai lần xác nhận độc lập. Các ý tưởng cho bản tin chỉ cần đọc rà soát. Kiểm tra qua loa một phát biểu có ảnh hưởng lớn là sai sót dễ nhận thấy. Kiểm tra quá nặng với công việc ít hệ trọng cũng là cách làm không phù hợp, chứ không đương nhiên an toàn hơn. Thời gian dùng để kiểm tra ba lần câu chữ trong bản tin mà không ai dựa vào đó để hành động sẽ lấy mất thời gian dành cho tổng giá.

Yêu cầu Claude tự kiểm tra lại đầu ra có một vai trò nhất định nhưng giới hạn. Hướng dẫn viết prompt của Anthropic cho biết tự kiểm tra giúp phát hiện lỗi, đặc biệt trong lập trình và toán học. Hướng dẫn nêu một ngoại lệ: Claude Opus 5 tự kiểm tra công việc tốt mà không cần được nhắc. Chỉ dẫn tự kiểm tra được viết cho các mô hình trước có thể khiến mô hình này kiểm tra quá mức. Tự kiểm tra là lượt rà soát ban đầu ít tốn công cho các lỗi tính toán và mâu thuẫn. Đây không phải xác thực độc lập: vẫn cùng mô hình và cùng những điểm mù.

## Trong bài thi

Câu hỏi kiểm tra các kỹ thuật và khả năng nhận biết mức kiểm tra tương xứng, theo cả hai hướng thiếu và thừa. Bẫy thường gặp nhất là tự kiểm tra được trình bày như thể đã xác minh. Một phương án yêu cầu người dùng nhờ Claude xác nhận, kiểm tra lại hoặc tự đánh giá công việc, rồi xem câu trả lời đầy tự tin là sự xác thực. Phần giải thích đáp án mẫu trong hướng dẫn thi nêu lý do cách này thất bại: mức độ tự tin do mô hình tự báo cáo không phải tín hiệu đáng tin cậy về độ chính xác.

### Khái niệm cốt lõi

Khi câu hỏi về xác thực đưa ra nhiều kế hoạch kiểm tra, hãy đánh giá từng kế hoạch bằng hai câu hỏi: Có thông tin độc lập được đưa vào phép kiểm tra hay không? Độ sâu kiểm tra có tương xứng với mức độ hệ trọng của từng phát biểu hay không? Đáp án đúng đáp ứng cả hai. Các phương án gây nhiễu thường trượt một trong hai: tự kiểm tra và nguồn tham chiếu vòng tròn không đáp ứng tính độc lập; xác minh mọi thứ ở mức tối đa như nhau không đáp ứng tính tương xứng.

## Những bẫy thường gặp trong bài thi

### Nhờ Claude xác nhận hoặc kiểm tra lại các phát biểu rồi xem đó là xác minh

Không có thông tin độc lập được đưa vào phép kiểm tra, và chính điểm mù tạo ra lỗi có thể tiếp tục xác nhận lỗi đó. Tự kiểm tra là lượt rà soát ban đầu hợp lý cho các sơ suất và mâu thuẫn, nhưng đáp án đúng luôn tìm đến nguồn độc lập đối với các phát biểu quan trọng.

### Kiểm tra một phát biểu bằng bản tóm tắt AI khác hoặc đầu ra trước đó của Claude

Xác minh vòng tròn kế thừa lỗi của nội dung đang được kiểm tra. Tính độc lập là yếu tố làm cho việc xác thực có ý nghĩa, nên đáp án đúng tìm đến tài liệu sơ cấp: ấn phẩm chính thức, tiêu chí được công bố hoặc hồ sơ của tổ chức.

### Xác minh mọi câu ở cùng mức tối đa bất kể mức độ hệ trọng

Tính tương xứng là kỹ năng được kiểm tra: kiểm tra đồng loạt với mức độ nặng sẽ tiêu tốn thời gian có hạn cho những câu văn không làm căn cứ cho điều gì. Đây là một bước vòng do tổ chức công việc quá mức, không phải lựa chọn an toàn hơn. Đáp án đúng tập trung kiểm tra các phát biểu mà quyết định phụ thuộc vào.

## Tình huống luyện tập

Một điều phối viên tình nguyện viên tại đơn vị vận hành tuyến đường sắt di sản nhờ Claude soạn hồ sơ xin tài trợ. Bản nháp nêu số lượt khách hằng năm, tỷ lệ phần trăm tăng trưởng các chuyến tham quan của trường học và khẳng định đơn vị đáp ứng các tiêu chí đủ điều kiện do bên tài trợ công bố. Cô chỉ có một buổi tối, không đủ thời gian kiểm tra sâu từng dòng, và không nội dung nào được phép chỉ dựa vào lời Claude. Kế hoạch xác thực nào phù hợp trước khi nộp?

**Phương án A**

Yêu cầu Claude kiểm tra lại cẩn thận toàn bộ bản nháp và xác nhận từng phát biểu, sau đó nộp khi Claude khẳng định các con số của mình là đúng.

**Phương án B**

Kiểm tra số lượt khách dựa trên hồ sơ của chính đơn vị đường sắt, tính lại tỷ lệ phần trăm từ những hồ sơ đó và kiểm tra các khẳng định về điều kiện nhận tài trợ dựa trên tài liệu tiêu chí do bên tài trợ công bố.

**Phương án C**

Kiểm tra các khẳng định về điều kiện nhận tài trợ dựa trên bản tóm tắt tiêu chí mà Claude đã tạo trước đó trong cuộc trò chuyện, đồng thời xác nhận số lượt khách nhất quán ở mọi chỗ xuất hiện trong toàn bộ bản nháp.

**Phương án D**

Xác minh độc lập từng câu trong hồ sơ với cùng độ sâu, kể cả phần mô tả lịch sử, trước khi cho bất kỳ ai xem.

## Bài tập thực hành: Lập kế hoạch xác thực cho một tài liệu thực tế

**Thời gian:** 35 phút.

### Bạn sẽ học được

- Cách xác định nguồn có thẩm quyền để kiểm tra từng phát biểu.
- Cách phân loại phát biểu theo hậu quả nếu sai và ấn định độ sâu kiểm tra.
- Cách làm cho đầu ra có thể truy nguyên nguồn gốc trước khi kiểm tra chọn lọc.
- Cách nhận ra những gì sẽ bị bỏ sót nếu chỉ dùng tự kiểm tra.

### Bước 1 — Chọn một tài liệu công việc do Claude soạn

Tài liệu cần có ít nhất ba phát biểu có thể kiểm tra: một con số, một thông tin thực tế bên ngoài và một khẳng định về việc đáp ứng yêu cầu đã được công bố.

**Vì sao:** Ba loại phát biểu này cần ba cách xác thực khác nhau, tạo thành một bộ công cụ thu nhỏ.

**Kết quả cần thấy:** Một tài liệu có ít nhất ba phát biểu được gạch chân và phân loại.

### Bước 2 — Xác định nguồn có thẩm quyền cho từng phát biểu

Nêu nguồn có thể xác định phát biểu đúng hay sai: hồ sơ của tổ chức bạn, ấn phẩm chính thức hoặc tiêu chí được công bố.

**Vì sao:** Phát biểu không xác định được nguồn là phát biểu không thể truy nguyên; với những phát biểu như vậy, không nên mặc nhiên cho rằng chúng đúng.

**Kết quả cần thấy:** Mỗi phát biểu được ghép với một nguồn cụ thể hoặc được đánh dấu là không thể truy nguyên.

### Bước 3 — Phân loại các phát biểu theo mức độ hệ trọng

Với con số làm căn cứ chính cho quyết định, bố trí hai lần xác nhận độc lập. Với cách diễn đạt ít hệ trọng, chỉ cần đọc rà soát. Viết một câu giải thích vì sao mỗi phát biểu được kiểm tra ở mức độ đó.

**Vì sao:** Tính tương xứng là lớp phán đoán bài thi kiểm tra. Việc viết câu giải thích buộc bạn thể hiện rõ cơ sở lựa chọn.

**Kết quả cần thấy:** Một kế hoạch kiểm tra trong đó độ sâu thay đổi rõ ràng theo mức độ hệ trọng.

### Bước 4 — Yêu cầu chỉ rõ nguồn và kiểm tra chọn lọc các điểm quan trọng

Yêu cầu Claude chỉ ra từng phát biểu còn lại đến từ đâu và cách đi đến từng kết luận, rồi kiểm tra chọn lọc những điểm có ảnh hưởng lớn.

**Vì sao:** Khả năng truy nguyên biến việc đọc lướt mơ hồ thành quá trình rà soát có thể đối chiếu, đồng thời tập trung công sức vào nơi mang lại giá trị.

**Kết quả cần thấy:** Các phát biểu được gắn với nguồn và lập luận; những điểm quan trọng đã được xác nhận.

### Bước 5 — Thực hiện kế hoạch và ghi lại kết quả

Ghi nhận phát biểu nào không vượt qua kiểm tra, nguồn nào giúp phát hiện vấn đề và kế hoạch chỉ dùng tự kiểm tra sẽ bỏ sót điều gì.

**Vì sao:** So sánh với cách chỉ dùng tự kiểm tra giúp nguyên tắc độc lập trở nên cụ thể ngay trong công việc của bạn.

**Kết quả cần thấy:** Một bản ghi ngắn gồm các lỗi đã phát hiện, nguồn giúp phát hiện chúng và những điểm mà tự kiểm tra sẽ bỏ sót.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Bật và sử dụng tìm kiếm web — *Enable and use web search*.
- Claude đang đưa ra câu trả lời sai hoặc gây hiểu lầm. Chuyện gì đang xảy ra? — *Claude is providing incorrect or misleading responses. What's going on?*
- Sử dụng Research trên Claude — *Use research on Claude*.
- Các phương pháp tốt nhất khi viết prompt — *Prompting best practices*.
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [2.2 — Nhận diện thông tin bịa đặt, sự thiếu nhất quán và thiên lệch](2-2-hallucinations-inconsistencies-bias.vi.md).
- **Bài tiếp theo:** Khi nào cần người rà soát hoặc xác minh bổ sung — *When Human Review or Additional Verification Is Required*.
