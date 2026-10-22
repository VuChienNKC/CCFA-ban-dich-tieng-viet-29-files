# 2.4 — Khi nào cần người rà soát hoặc xác minh bổ sung

- **Lĩnh vực (Domain):** 2
- **Nhiệm vụ (Task):** 2.4
- **Tên bài gốc:** When Human Review or Additional Verification Is Required
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/2-output-evaluation/2-4-human-review-escalation)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

**Chuyển rà soát (escalation)** là chuyển đầu ra của Claude cho một người đủ năng lực chuyên môn kiểm tra trước khi sử dụng. **Phân loại rà soát (triage)** là quyết định ai sẽ kiểm tra từng đầu ra. **Yếu tố kích hoạt (trigger)** là những đặc điểm của tình huống làm tăng hậu quả nếu xảy ra lỗi. Mục tiêu này đề cập khi nào việc bạn tự rà soát là chưa đủ và ai mới là người phù hợp để rà soát.

Chủ một trường dạy lái xe có bốn bản nháp do Claude tạo: nội dung quảng cáo trên website, thư trả lời về hoàn tiền theo điều khoản đặt lịch, ghi chú đánh giá một giáo viên và thông báo nhắc vệ sinh xe. Cả bốn đều được viết tốt.

## Các yếu tố kích hoạt

Mỗi yếu tố dưới đây đều đòi hỏi người đủ năng lực chuyên môn rà soát:

- Đối tượng tiếp nhận bên ngoài: khách hàng, công chúng, báo chí, bên tài trợ.
- Hệ quả pháp lý, tài chính hoặc hợp đồng.
- Quyết định về con người: tuyển dụng, đánh giá, phân bổ.
- Ảnh hưởng đến an toàn hoặc sức khỏe.
- Không thể đảo ngược sau khi gửi.

Chỉ một yếu tố cũng đủ để cần thêm một người đủ năng lực kiểm tra. Khi có nhiều yếu tố cùng xuất hiện, việc chuyển rà soát là bắt buộc. Sự tự tin và câu chữ trau chuốt không nằm trong danh sách, vì mọi bản nháp của Claude vốn đã có những đặc điểm đó. Claude không phải nguồn sự thật duy nhất; đầu ra có ảnh hưởng hệ trọng cần được xem xét kỹ.

Ở trường dạy lái xe, quảng cáo hướng đến người bên ngoài. Thư trả lời về hoàn tiền có hệ quả hợp đồng. Ghi chú đánh giá làm đầu vào cho quyết định về một người. Thông báo nhắc vệ sinh không có những yếu tố trên, nên chủ trường tự rà soát.

Đầu ra không có yếu tố kích hoạt cần được chính bạn kiểm tra cẩn thận, sử dụng các thói quen từ mục tiêu 2.1 đến 2.3. Đó là tài liệu làm việc nội bộ, bản nháp đầu tiên còn được tinh chỉnh và thông báo thường lệ với hệ quả thấp. Việc kiểm tra này phải thực chất, không phải miễn kiểm tra: phân loại rà soát quyết định ai kiểm tra, không bao giờ quyết định có cần ai kiểm tra hay không.

## Đủ năng lực chuyên môn, không chỉ có chức vụ cao

Chính sách sử dụng của Anthropic đặt ra tiêu chuẩn. Chính sách nêu các **Lĩnh vực rủi ro cao (High-risk Areas)**, chẳng hạn pháp lý, y tế, tài chính và việc làm, trong đó đầu ra của Claude có thể trở thành lời khuyên cho một người hoặc quyết định về người đó. Chính sách gọi đầu ra ấy là **Khuyến nghị AI có rủi ro cao (High-risk AI Recommendation)** và yêu cầu hai điều: người liên quan phải được thông báo rằng AI đã được sử dụng; đồng thời một người đủ năng lực chuyên môn phải rà soát. Quy tắc rà soát nêu:

> Một người đủ năng lực chuyên môn phải rà soát thực chất Khuyến nghị AI có rủi ro cao, có quyền thay đổi hoặc chỉnh sửa khuyến nghị đó, trước khi khuyến nghị được đưa ra dưới dạng lời khuyên.

Quy tắc tương tự cũng áp dụng trước khi đầu ra được dùng để ra quyết định. Tư vấn cho ai đó về quyền pháp lý của họ hoặc cách xử lý một vấn đề pháp lý cụ thể thuộc một trong các lĩnh vực này.

Người đủ năng lực chuyên môn là “người có đào tạo hoặc kinh nghiệm để đánh giá đầu ra trong lĩnh vực đó”. Cụm từ quyết định người rà soát là **“trong lĩnh vực đó”**. Nội dung hợp đồng cần người có năng lực pháp lý; số liệu thuế cần kế toán; các phát biểu chuyên môn lâm sàng cần người hành nghề lâm sàng; tiêu chí tuyển dụng cần năng lực phán đoán nhân sự. Ngoài các Lĩnh vực rủi ro cao, chính sách không đặt ra quy tắc rà soát, nhưng năng lực chuyên môn vẫn là tiêu chí chọn người.

Chức vụ cao và việc đang rảnh không phải điều kiện cần, cũng không phải điều kiện đủ. Một người không có chuyên môn, dù chức vụ cao đến đâu, cũng không phát hiện được những lỗi khiến nội dung trở nên nguy hiểm. Một giám đốc bận rộn đọc lướt điều khoản thuê chỉ tạo cảm giác yên tâm chứ chưa phải rà soát thực chất. Thư trả lời về hoàn tiền được chuyển cho luật sư, không phải chỉ cho chủ trường.

## Hai hướng sai lầm

**Chuyển rà soát chưa đủ (under-escalation)** là sai lầm dễ hình dung. Người dùng gửi nội dung ra bên ngoài, trong đó có các phát biểu kéo theo hệ quả chuyên môn, vì bản nháp được viết có vẻ đáng tin cậy. Hoặc họ cho qua đầu ra vì cho rằng “chỉ dùng nội bộ”, dù nó làm đầu vào cho một quyết định bên ngoài hoặc có ảnh hưởng lớn. Theo mặc định, đầu ra của Claude đã có giọng văn đầy thẩm quyền, nhưng các yếu tố kích hoạt thuộc về tình huống và vẫn tồn tại dù câu chữ trau chuốt đến đâu. Đầu ra sẽ được dùng vào đâu quan trọng hơn nơi nó được soạn. Ghi chú đánh giá ở lại văn phòng nhưng làm căn cứ cho quyết định về một giáo viên.

**Chuyển rà soát quá mức (over-escalation)** có vẻ an toàn vì sự thận trọng thường tạo cảm giác như vậy. Nhưng thực tế không phải thế. Lập một hội đồng để duyệt thông báo lịch trực hoặc đưa mọi bản nháp thường lệ qua người rà soát chuyên môn là bước vòng không cần thiết. Việc này làm người rà soát quá tải, khiến công việc thường lệ đình trệ và khiến tổ chức dần phớt lờ chính kênh chuyển rà soát mà đầu ra có rủi ro cao cần đến. Luật sư phải đọc thông báo nhắc vệ sinh sẽ xử lý thư hoàn tiền muộn hơn. Kỹ năng cần có là phân loại đúng, không phải thận trọng ở mức tối đa.

## Hai lý do khác nhau để dừng lại

Mục tiêu này yêu cầu chuyển rà soát vì chất lượng và mức độ hệ trọng: điều gì xảy ra nếu đầu ra sai và ai đủ năng lực phát hiện lỗi. Lĩnh vực 6 đề cập các lý do dừng khác: dữ liệu là dữ liệu cá nhân hoặc thuộc diện quản lý, hoặc cách sử dụng nằm ngoài chính sách AI của tổ chức. Cả hai có thể xuất hiện trong cùng tình huống, chẳng hạn thư hoàn tiền trích dẫn dữ liệu cá nhân của học viên, nhưng yếu tố kích hoạt khác nhau. Việc chuyển xử lý kỹ thuật trong chương trình là loại thứ ba: chuyển nhiệm vụ cho Claude Developer hoặc Architect vì cần tự động hóa hay tích hợp. Đó là nhiệm vụ đã vượt quá phạm vi cuộc trò chuyện, không phải đầu ra cần người có chuyên môn rà soát.

## Trong bài thi

Bài thi kiểm tra nội dung này dưới dạng phân loại rà soát: quyết định dựa trên hệ quả mà đầu ra mang theo, không dựa trên mức độ trau chuốt. Phán đoán sai theo cả hai hướng đều bị đánh giá là sai. Trong phần dẫn câu hỏi, hãy tìm nơi đầu ra sẽ được sử dụng và điều gì khiến người rà soát được nêu tên có đủ năng lực. Thí sinh ít khi nghĩ rằng chuyển rà soát quá mức cũng được kiểm tra, nhưng “chuyển tất cả để rà soát” thực sự có thể là đáp án sai. Bài thi phân biệt rõ các yếu tố kích hoạt thuộc Lĩnh vực 6.

### Khái niệm cốt lõi

Phân loại rà soát đặt hai câu hỏi theo thứ tự: Đầu ra này mang theo hệ quả gì? Nếu có hệ quả cần chú ý, ai có chuyên môn trong lĩnh vực đó để phát hiện những lỗi quan trọng? Các phương án trả lời bằng cấp bậc, sự sẵn có hoặc một quy trình áp dụng đồng loạt là phương án gây nhiễu.

## Những bẫy thường gặp trong bài thi

### Chọn người rà soát theo chức vụ hoặc sự sẵn có thay vì năng lực chuyên môn

Khi Chính sách sử dụng yêu cầu rà soát đối với lời khuyên hoặc quyết định trong một Lĩnh vực rủi ro cao, người rà soát phải đủ năng lực: có đào tạo hoặc kinh nghiệm để đánh giá đầu ra trong lĩnh vực đó. Ngoài các lĩnh vực này, năng lực vẫn là tiêu chí đúng. Việc quản lý cấp cao ký duyệt câu chữ pháp lý hoặc phát biểu lâm sàng chỉ tạo cảm giác yên tâm, chưa phải rà soát thực chất. Vì vậy, đáp án đúng nêu rõ năng lực: người thực sự có thể phát hiện lỗi nguy hiểm.

### Cho qua đầu ra vì chỉ dùng nội bộ

Yếu tố kích hoạt nằm ở hệ quả của đầu ra, không phải nơi đầu tiên nhận nó. Phân tích nội bộ làm đầu vào cho hồ sơ dự thầu bên ngoài hoặc quyết định về con người vẫn mang theo hệ quả ấy. Đáp án đúng chuyển rà soát dựa trên mục đích sử dụng cuối cùng và mức độ hệ trọng, không dựa trên nhãn “nội bộ”.

### Chuyển mọi thứ để rà soát cho an toàn

Chuyển rà soát quá mức là đáp án sai được kiểm tra, không phải đáp án đúng vì thận trọng. Đưa các bản nháp nội bộ thường lệ qua hội đồng hoặc chuyên gia làm người rà soát quá tải và suy yếu kênh mà đầu ra có rủi ro cao cần đến. Đáp án đúng chấp nhận việc tự kiểm tra cẩn thận đối với tài liệu thực sự ít hệ trọng.

## Tình huống luyện tập

Người quản lý một cơ sở đo khám thị lực có ba bản nháp do Claude tạo: nội dung quảng cáo cho dòng tròng kính mới với các khẳng định cụ thể về kết quả thị giác; chính sách đổi ca nội bộ được diễn đạt lại; và thư trả lời khiếu nại của bệnh nhân có đề cập những sai sót chuyên môn lâm sàng có thể đã xảy ra. Người quản lý không được đào tạo lâm sàng và không biết quảng cáo chăm sóc mắt được pháp luật cho phép cam kết điều gì. Mỗi bản nháp cần được người am hiểu lĩnh vực kiểm tra, đồng thời tránh chậm trễ không cần thiết. Cách phân loại rà soát nào phù hợp?

**Phương án A**

Đăng quảng cáo vì nội dung được viết chuyên nghiệp và soạn từ tài liệu sản phẩm, đồng thời nhờ chuyên viên đo khám thị lực xem chính sách lịch ca và thư trả lời khiếu nại.

**Phương án B**

Đưa cả ba bản nháp ra cuộc họp quản lý hằng tuần của cơ sở để tập thể ký duyệt trước khi sử dụng bất kỳ bản nào, nhằm chia sẻ trách nhiệm cho mọi tài liệu trong toàn nhóm.

**Phương án C**

Trước khi gửi, chuyển các khẳng định trong quảng cáo cho người có năng lực đánh giá tuyên bố về sức khỏe và chuyển thư trả lời khiếu nại cho chuyên viên đo khám thị lực; người quản lý tự đọc kiểm tra cẩn thận chính sách lịch ca.

**Phương án D**

Với tư cách người quản lý chịu trách nhiệm, tự kiểm tra kỹ cả ba rồi gửi đi, để xử lý nhanh và tập trung trách nhiệm vào một người.

## Bài tập thực hành: Phân loại rà soát năm đầu ra gần nhất

**Thời gian:** 25 phút.

### Bạn sẽ học được

- Cách nhận ra các yếu tố đòi hỏi người đủ năng lực chuyên môn rà soát.
- Cách xác định người rà soát theo chuyên môn thay vì chức vụ.
- Cách kiểm tra phân loại rà soát để tránh cả hai hướng sai lầm.
- Cách biến một lần phân loại thành danh sách chuyển rà soát dùng thường xuyên.

### Bước 1 — Liệt kê năm nội dung gần nhất Claude đã soạn cho bạn

Hoặc tạo năm nội dung tiêu biểu cho vai trò công việc của bạn.

**Vì sao:** Phân loại rà soát chỉ trở thành thói quen khi được thực hành trên chính sự pha trộn mức độ hệ trọng mà công việc của bạn tạo ra.

**Kết quả cần thấy:** Năm mô tả đầu ra thực tế, mỗi mô tả một dòng, từ thường lệ đến có ảnh hưởng lớn.

### Bước 2 — Đánh dấu yếu tố kích hoạt của từng đầu ra

Xem xét: đối tượng bên ngoài, hệ quả pháp lý hoặc tài chính, quyết định về con người, ảnh hưởng đến an toàn hoặc sức khỏe và việc không thể đảo ngược sau khi gửi.

**Vì sao:** Yếu tố kích hoạt là đặc điểm của tình huống. Liệt kê chúng giúp tránh để sự trau chuốt của câu chữ quyết định việc phân loại.

**Kết quả cần thấy:** Mỗi đầu ra có các yếu tố kích hoạt được đánh dấu hoặc được ghi rõ là không có.

### Bước 3 — Xác định người đủ năng lực rà soát cho từng mục có yếu tố kích hoạt

Chọn một người hoặc vai trò trong tổ chức có năng lực về đúng lĩnh vực đó, không chỉ có chức vụ cao.

**Vì sao:** Nêu một người cụ thể giúp kiểm tra xem kênh chuyển rà soát có thực sự tồn tại trước khi bạn cần đến hay không.

**Kết quả cần thấy:** Mỗi mục có yếu tố kích hoạt được gắn với người rà soát cụ thể và năng lực khiến họ phù hợp.

### Bước 4 — Ghi nội dung tự kiểm tra cho từng mục không có yếu tố kích hoạt

Dùng thói quen kiểm tra hai lượt từ mục tiêu 2.1 làm danh sách kiểm tra.

**Vì sao:** Tự kiểm tra là kết quả phù hợp với công việc ít hệ trọng. Viết rõ cách kiểm tra giúp bảo đảm đây là rà soát thực chất thay vì bỏ qua.

**Kết quả cần thấy:** Mỗi mục không có yếu tố kích hoạt có một ghi chú ngắn về việc tự kiểm tra.

### Bước 5 — Kiểm tra cả hai hướng sai lầm và lưu danh sách dùng thường xuyên

Rà lại toàn bộ kết quả phân loại để phát hiện chuyển rà soát chưa đủ hoặc quá mức, rồi giữ lại làm danh sách chuyển rà soát thường trực.

**Vì sao:** Cả thiếu và thừa chuyển rà soát đều được kiểm tra trong bài thi và đều hiện rõ trong một bảng phân loại được viết ra.

**Kết quả cần thấy:** Không có nội dung hướng ra bên ngoài bị cho qua; không có nội dung thường lệ phải xếp hàng chờ hội đồng; và có một danh sách có thể tái sử dụng.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Chính sách sử dụng — *Usage Policy*.
- Claude đang đưa ra câu trả lời sai hoặc gây hiểu lầm. Chuyện gì đang xảy ra? — *Claude is providing incorrect or misleading responses. What's going on?*
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [2.3 — Các kỹ thuật kiểm chứng sự thật và xác thực](2-3-fact-checking-validation.vi.md).
- **Bài tiếp theo:** [2.5 — Biên tập, điều chỉnh và so sánh đầu ra cho đối tượng đọc](2-5-editing-adapting-outputs.vi.md).
