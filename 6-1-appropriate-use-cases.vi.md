# 6.1 — Nhận diện trường hợp sử dụng phù hợp và không phù hợp

- **Lĩnh vực (Domain):** 6
- **Nhiệm vụ (Task):** 6.1
- **Tên bài gốc:** Identifying Appropriate and Inappropriate Use Cases
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/6-governance-responsible-use/6-1-appropriate-use-cases)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Hai câu hỏi quyết định có giao nhiệm vụ cho Claude hay không. **Mức phù hợp thực tiễn (fit)** hỏi Claude có làm tốt không: đúng dạng việc, đúng khối lượng, đầu ra có người kiểm tra được. Lĩnh vực 4 đề cập khía cạnh này. **Tính thích hợp (appropriateness)** hỏi có nên giao nhiệm vụ ngay từ đầu không. Nó xem xét bằng chứng khác: mức độ hệ trọng, thẩm quyền công việc đòi hỏi và ai chịu trách nhiệm về kết quả. Một nhiệm vụ có thể hoàn toàn phù hợp về thực tiễn nhưng vẫn phải thuộc về người đủ chuyên môn.

## Làm tốt không đồng nghĩa được phép

Chủ cửa hàng xe đạp có hai việc: tóm tắt nhiều đánh giá khách hàng thành chủ đề và chấm điểm hồ sơ ứng tuyển thợ sửa xe để chọn người tuyển. Chấm hồ sơ rất phù hợp về thực tiễn: có cấu trúc, số lượng lớn, kiểm tra được. Nó vẫn có thể không thích hợp vì quyết định mà điểm số dẫn đến và người không thể phản đối quyết định đó. Đáp án sai thường suy luận từ chất lượng: Claude làm nhanh, tốt nên giao là ổn. Chất lượng chưa bao giờ là câu hỏi ở đây.

## Bốn nhóm sử dụng không thích hợp

**Thứ nhất, công việc cần thẩm quyền chuyên môn:** phán đoán pháp lý, y tế, tài chính và bảo vệ người cần được bảo vệ (safeguarding). Người đủ chuyên môn phải đưa ra và chịu trách nhiệm. Claude có thể giúp chuẩn bị, tóm tắt hoặc hiểu vấn đề, nhưng không thể là nguồn đưa ra lời khuyên. Ở cửa hàng xe đạp, lời khuyên y tế cho khách bị thương phải đến từ người đủ chuyên môn. Chính sách sử dụng nêu các **Lĩnh vực rủi ro cao (High-risk Areas)** gồm tư vấn pháp lý, y tế; tài chính, tín dụng, bảo hiểm, nhà ở, việc làm, giáo dục và khả năng tiếp cận chăm sóc sức khỏe. Trong các lĩnh vực này, người đủ năng lực phải rà khuyến nghị trước khi dùng làm lời khuyên hoặc quyết định, và “người đủ năng lực vẫn chịu trách nhiệm về độ chính xác và tính thích hợp của nội dung được đưa ra hoặc quyết định được thực hiện”. Chính sách loại trừ nội dung nâng cao sức khỏe như kiến thức về giấc ngủ, căng thẳng, dinh dưỡng hoặc tập luyện.

**Thứ hai, quyết định có hệ quả về người có thể nhận diện:** ai được nhận việc, phần thưởng, chế tài hoặc chuyến thăm. Lý do không phải đầu ra kém, mà là không ai chịu trách nhiệm về quyết định và người bị ảnh hưởng không thể phản đối. Chấm điểm ứng viên thợ sửa thuộc nhóm này.

**Thứ ba, bịa đặt nhưng trình bày như thật:** lời trích, nhận xét khách hàng, nghiên cứu tình huống hoặc bằng chứng được dựng lên, chẳng hạn lời chứng thực cửa hàng tự viết. Càng hợp lý, sự bịa đặt càng tệ vì nội dung dựng lên thuyết phục dễ được tin hơn. Các lệnh cấm thông tin sai lệch và hành vi lừa dối trong Chính sách sử dụng là nền tảng của nhóm này.

**Thứ tư, mọi việc bị Chính sách sử dụng hoặc chính sách tổ chức cấm.** Mục tiêu 6.3 đề cập nội dung đó.

## Phép thử thay thế

Hình dung một đồng nghiệp có năng lực, thiện chí nhưng:

- Không có chuyên môn được công nhận trong lĩnh vực.
- Không tiếp cận lịch sử của người liên quan.
- Không chịu trách nhiệm về kết quả.

Bạn có chấp nhận công việc này từ họ không? Phép thử biến câu hỏi trừu tượng thành phán đoán giao việc thông thường mà người làm nghề vốn biết. Bản tóm tắt đánh giá đạt: đồng nghiệp đó có thể viết và chủ cửa hàng kiểm tra. Chấm ứng viên không đạt cả ba khía cạnh. Khung AI Fluency của Anthropic gọi kỹ năng này là **Delegation — giao việc**.

## Phần lớn công việc là thích hợp

Điểm cân bằng quan trọng ngang bốn nhóm trên. Tài liệu chính thức mô tả phạm vi thích hợp rộng có chủ đích: viết nhiều định dạng, tóm tắt tài liệu dài, động não, phân tích hình ảnh và dữ liệu, dịch thuật. Soạn thảo, định dạng lại, phân tích tài liệu bạn có và chuẩn bị để con người quyết định đều thích hợp. Các nhóm không thích hợp hẹp và cụ thể. Xem mọi việc gần chúng là bị cấm sẽ bỏ công việc mà một biện pháp bảo vệ đơn giản có thể cho phép. Chủ cửa hàng vẫn có thể nhờ tóm tắt từng hồ sơ, rồi tự đọc và lựa chọn.

## Trong bài thi

Mục tiêu này hỏi khác phần còn lại của chứng nhận; thí sinh vừa học Lĩnh vực 4 thường trả lời nhầm câu hỏi. Phép thử thay thế bao quát toàn bộ phạm vi kiểm tra. Bài thi cũng đánh giá thận trọng quá mức là sai: đáp án đúng gần như luôn tạo cách thực hiện trong khuôn khổ quy tắc.

### Dấu hiệu trong câu hỏi thi

Thêm rà soát không sửa được việc giao một quyết định không thích hợp. Quản lý kiểm tra đầu ra của quyết định có hệ quả về người có thể nhận diện không khôi phục trách nhiệm phán đoán hay khả năng phản đối của người bị ảnh hưởng. Chủ cửa hàng đọc mọi điểm ứng viên cũng không thay đổi hai điều đó. Phương án coi rà soát là cách khắc phục đang kiểm tra chính điểm này.

Quy tắc rà soát trong Chính sách sử dụng trả lời câu hỏi khác. Khi thực hiện một cách dùng trong Lĩnh vực rủi ro cao, chính sách yêu cầu: “Một người đủ năng lực phải rà soát thực chất Khuyến nghị AI có rủi ro cao, có quyền thay đổi hoặc chỉnh sửa trước khi được đưa ra làm lời khuyên.” Ở đó, rà soát là biện pháp bắt buộc, được bài 2.4 dạy như tiêu chuẩn. Rà soát không biến quyết định vốn không nên giao thành quyết định nên giao. Trước tiên hỏi việc giao có thích hợp không; sau đó mới áp dụng yêu cầu rà soát.

Khung AI Fluency liệt kê bốn chữ D như tên mô-đun, không định nghĩa chúng. Hiểu Delegation là “quyết định giao gì cho AI và giữ gì lại” là cách tác giả diễn giải. Bài về công dụng Claude trong Trung tâm trợ giúp liệt kê việc phù hợp, không đưa lệnh cấm. Các nhóm không thích hợp dựa trên Chính sách sử dụng và hướng dẫn thi.

## Những bẫy thường gặp trong bài thi

### Xem mức phù hợp thực tiễn là quyền thực hiện

Hai phép đánh giá dựa vào bằng chứng khác nhau. Việc có cấu trúc, số lượng lớn, kiểm tra được — đủ điều Lĩnh vực 4 muốn — vẫn có thể không thích hợp. Tính thích hợp dựa vào trách nhiệm và khả năng phản đối, không phải Claude làm tốt đến đâu.

### Chấp nhận lý do chỉ dùng nội bộ

Kết quả không ra khỏi tổ chức là phương án gây nhiễu xuyên suốt lĩnh vực này, không phải đáp án đúng. Giữ nội bộ không khôi phục trách nhiệm cho quyết định trong đầu ra hoặc con đường phản đối của người bị ảnh hưởng.

### Từ chối cả hai phần của đề xuất hỗn hợp

Tránh dùng dưới vẻ thận trọng là phương án gần đúng dễ bị chọn. Khi đề xuất trộn việc thích hợp và không thích hợp, đáp án đúng giữ phần thích hợp, chỉ từ chối phần còn lại. Bỏ cả hai lãng phí công cụ và hiểu sai mục tiêu.

## Tình huống luyện tập

Quản lý trung tâm trẻ em được nhờ dùng Claude cho khảo sát gia đình hằng năm. Có hai đề xuất: tóm tắt 300 phản hồi tự do thành chủ đề để đánh giá dịch vụ và chấm phản hồi từng gia đình để đánh dấu ai cần được đến thăm tại nhà. Việc đánh giá dịch vụ cần các chủ đề. Chính sách cho dùng Claude với văn bản khảo sát nhưng cấm mọi công cụ chấm gia đình cho việc thăm nhà. Quản lý nên làm gì?

**Phương án A**

Tóm tắt thành chủ đề sau khi bỏ chi tiết nhận diện; giữ việc xác định gia đình cần thăm cho nhân viên đủ chuyên môn của trung tâm.

**Phương án B**

Chấm điểm như đề xuất, để phó quản lý rà mọi gia đình được đánh dấu trước khi thăm nhằm giữ con người trong quy trình.

**Phương án C**

Từ chối cả hai vì khảo sát gia đình quá nhạy cảm để bất kỳ công cụ AI nào tiếp cận.

**Phương án D**

Làm cả hai vì dữ liệu không rời trung tâm và gia đình đã đồng ý dùng cho lập kế hoạch dịch vụ khi hoàn thành khảo sát.

## Bài tập thực hành: Phân loại công việc thực tế trong hai tuần

**Thời gian:** 25 phút.

### Bạn sẽ học được

- Áp dụng phép thử thay thế cho nhiệm vụ thật.
- Nêu nhóm nào trong bốn nhóm khiến nhiệm vụ không thích hợp.
- Viết biện pháp bảo vệ cho nhiệm vụ còn ở ranh giới.
- Kiểm tra phán đoán để tránh thận trọng quá mức.

### Bước 1 — Liệt kê mười công việc gần nhất và hai việc bạn không bao giờ giao

Mười việc gồm những gì đã giao hoặc từng cân nhắc giao Claude.

**Vì sao:** Phép thử cần việc giao thực tế. Ví dụ dựng lên làm bài tập trông tốt và che thói quen thật.

**Kết quả cần thấy:** Mười hai nhiệm vụ, mỗi nhiệm vụ một dòng bằng lời của bạn.

### Bước 2 — Áp dụng phép thử thay thế cho từng việc

Bạn có chấp nhận từ đồng nghiệp giỏi nhưng không có chuyên môn lĩnh vực, không tiếp cận người liên quan và không chịu trách nhiệm kết quả không?

**Vì sao:** Phép thử biến tính thích hợp thành phán đoán giao việc bạn vốn biết làm.

**Kết quả cần thấy:** Đạt hoặc không đạt cho mỗi việc; nêu lý do không đạt: chuyên môn, lịch sử hoặc trách nhiệm.

### Bước 3 — Phân thành thích hợp và không thích hợp

Với mỗi việc không thích hợp, nêu một trong bốn nhóm.

**Vì sao:** Gọi tên nhóm là kỹ năng thi; cần nói được vì sao thay vì chỉ cảm thấy rủi ro.

**Kết quả cần thấy:** Nhãn thẩm quyền chuyên môn, quyết định hệ trọng, bịa đặt hoặc chính sách cấm cho từng việc không thích hợp.

### Bước 4 — Viết biện pháp bảo vệ cho việc ở ranh giới

Nêu cần thay đổi tài liệu, cách thực hiện hoặc sự cho phép thế nào để tiến hành được.

**Vì sao:** Đáp án đúng gần như luôn tạo cách thực hiện. Kỹ năng là tìm biện pháp bảo vệ, không tìm lý do từ chối.

**Kết quả cần thấy:** Mỗi nhiệm vụ ranh giới có biện pháp một dòng, cụ thể để ngày mai có thể làm.

### Bước 5 — Kiểm tra nhóm thích hợp có lớn hơn không

Nếu không, xem lại kết quả và nhớ điểm cân bằng của bài.

**Vì sao:** Thận trọng quá mức là lỗi các phương án gây nhiễu khai thác. Danh sách chủ yếu không thích hợp thường do đánh giá quá khắt khe.

**Kết quả cần thấy:** Tám việc trở lên trong mười hai việc thích hợp hoặc lý do bằng văn bản vì sao công việc bạn thực sự ngoại lệ.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Chính sách sử dụng — *Usage Policy*.
- Tôi có thể dùng Claude vào những việc gì? — *What are some things I can use Claude for?*
- AI Fluency: Khung năng lực và nền tảng — *AI Fluency: Framework and Foundations*.
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

**Ghi chú của tác giả bài gốc:** Bài Trung tâm trợ giúp mô tả cách dùng thích hợp nhưng không liệt kê lệnh cấm. Các nhóm không thích hợp đến từ Chính sách sử dụng và mục tiêu của hướng dẫn thi.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [5.4 — Thông báo, duy trì và cập nhật cấu hình](5-4-maintaining-configurations.vi.md).
- **Bài tiếp theo:** [6.2 — Xem xét độ nhạy cảm dữ liệu, quy định và quyền riêng tư](6-2-data-sensitivity-privacy.vi.md).
