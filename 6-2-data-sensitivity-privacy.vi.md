# 6.2 — Xem xét độ nhạy cảm dữ liệu, quy định và quyền riêng tư

- **Lĩnh vực (Domain):** 6
- **Nhiệm vụ (Task):** 6.2
- **Tên bài gốc:** Applying Data Sensitivity, Regulatory and Privacy Considerations
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/6-governance-responsible-use/6-2-data-sensitivity-privacy)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

**Tài liệu nhạy cảm** là mọi thứ tổ chức không nên giao cho dịch vụ bên ngoài khi chưa có quyết định. Đó có thể là dữ liệu cá nhân hoặc tài liệu nhạy cảm vì chủ sở hữu hay cam kết liên quan. **Biện pháp bảo vệ (safeguard)** thay đổi những gì rời quyền kiểm soát của tổ chức. Có bốn bậc bảo vệ theo thứ tự cố định. **Biện pháp giả hiệu (placebo)** chỉ tác động sau khi tài liệu đã được gửi đi.

Quản lý nhà trẻ muốn Claude giải thích vì sao tiền học còn nợ tăng học kỳ này. Bảng tính có tên, ngày sinh, địa chỉ, ghi chú dị ứng của từng trẻ cùng số tài khoản, khoản thanh toán của phụ huynh. Tải nguyên bản đưa tất cả ra ngoài. Từ chối khiến nợ phí không được giải thích. Đáp án nằm giữa: biện pháp bảo vệ cho phép làm việc trong chính sách.

## Nhận diện tài liệu nhạy cảm

Danh sách dễ nhận ra gồm tên, địa chỉ, ngày sinh, mã tham chiếu và số tài khoản, sức khỏe, tài chính, mọi thông tin về trẻ em. Những nhóm về sở hữu và cam kết hay bị bỏ sót:

- Thông tin được giữ theo nghĩa vụ bảo mật.
- Số liệu bí mật thương mại.
- Tài liệu bên thứ ba chịu hợp đồng quy định cách xử lý.

Bảng giá nhà cung cấp không có dữ liệu cá nhân nhưng vẫn có thể là tài liệu bị hạn chế chặt nhất vì hợp đồng điều chỉnh nó. Bảng giá nhà cung cấp thực phẩm của nhà trẻ là ví dụ.

Chính sách sử dụng của Anthropic xem dữ liệu mật hoặc độc quyền, cùng thông tin liên hệ không công khai và dữ liệu sức khỏe, là thông tin riêng tư không được lạm dụng hay truy cập không phép. Chính sách cũng cấm vi phạm quyền riêng tư theo luật áp dụng, chẳng hạn chia sẻ thông tin cá nhân không có đồng thuận.

Bài về bảo vệ dữ liệu của Anthropic mô tả mã hóa khi truyền và lưu trữ, mặc định chặn nhân viên truy cập. Điều đó bảo vệ dữ liệu Anthropic đang giữ, không thay quyết định của tổ chức về thứ được phép rời quyền kiểm soát.

## Các bậc theo thứ tự

Mỗi bậc giữ lại nhiều phần công việc hơn bậc bên dưới, nên chọn bậc thấp nhất có tác dụng.

### 1. Loại bỏ (Remove)

Phần lớn phân tích không cần tên. Bỏ thông tin nhận diện và tiến hành ngay. Câu hỏi nợ phí cần mẫu thanh toán, nên bỏ tên và địa chỉ trẻ.

### 2. Ẩn danh hoặc tổng hợp (Anonymise or aggregate)

Dùng nhóm thay cá nhân, khoảng thay số chính xác. Nhà trẻ có thể nhóm gia đình theo phòng và biểu diễn nợ phí bằng khoảng.

### 3. Dùng cách xử lý được cho phép (Use an authorised route)

Chuyển việc sang không gian làm việc được phê chuẩn, theo thỏa thuận bao quát loại tài liệu này.

### 4. Xin phép (Seek authorisation)

Hỏi người phụ trách dữ liệu hoặc chính sách. Đây là hành động, không phải từ chối.

Từ bỏ nằm dưới cùng: ẩn danh cho phép phân tích tiếp, nên bỏ cuộc không đem lại lợi ích.

## Vì sao biện pháp giả hiệu thất bại?

Kiểm soát chính sách liên quan những gì rời quyền kiểm soát tổ chức, xảy ra lúc tải lên. Bước sau không đảo ngược được. Mọi biện pháp giả hiệu đều sai theo cách này: bảo Claude quên, tuyên bố tệp là mật, thêm dòng bảo mật vào prompt hoặc xóa chat. Nếu quản lý tải toàn bộ bảng rồi yêu cầu không lưu, chi tiết vẫn đã được gửi. Không câu nào gõ vào chat có thể điều chỉnh ngược việc đã tải. Bảo vệ phải xảy ra trước tải lên, nếu không là không có.

## Bạn đang dùng sản phẩm nào?

Hai bài quyền riêng tư hiện hành của Anthropic có cùng tên **Is my data used for model training?** Một bài về sản phẩm tiêu dùng, một về sản phẩm thương mại, và trả lời khác nhau. Mặc định, Anthropic không dùng đầu vào, đầu ra của sản phẩm thương mại như Claude for Work để huấn luyện mô hình. Xử lý dữ liệu phụ thuộc gói; chi tiết đã thay đổi trong lịch sử tài liệu. Vì vậy, hỏi ba câu thay vì học thuộc câu trả lời hôm nay: Tôi dùng sản phẩm nào? Tài liệu hiện tại nói gì? Thỏa thuận tổ chức bổ sung gì? Quản lý nhà trẻ hỏi chúng trước. Bài 6.3 đề cập hệ quả của câu trả lời.

## Trong bài thi

Câu hỏi mẫu có quản lý dự án muốn tải bảng tính tên và số tài khoản khách. Đáp án đúng không tải nguyên trạng cũng không bỏ phân tích, mà ẩn danh để làm trong chính sách. Biện pháp cho phép tiến hành nằm giữa hai cực sai chính là mục tiêu thu nhỏ. Thứ tự các bậc là kỹ năng kiểm tra. Bỏ cuộc gần như không phải đáp án đúng vì giải thích của hướng dẫn nói ẩn danh cho phép phân tích. Hướng dẫn cũng nói yêu cầu mô hình không giữ dữ liệu không đáp ứng kiểm soát chính sách.

### Dấu hiệu trong câu hỏi thi

Phương án có biện pháp chỉ hoạt động sau tải lên đều sai. Biện pháp giả hiệu không bao giờ là đáp án đúng. Đáp án đúng thay đổi đầu vào, không phải những gì diễn ra sau đó.

Chi tiết xóa và lưu giữ thường thay đổi. Tài liệu tra cứu nhanh Lĩnh vực 6 có số liệu hiện hành kèm ngày.

## Những bẫy thường gặp trong bài thi

### Xem chỉ dẫn bảo mật hoặc xóa sau đó là biện pháp bảo vệ

Giải thích câu hỏi mẫu nói rõ yêu cầu không giữ dữ liệu không đáp ứng kiểm soát chính sách. Việc tiết lộ xảy ra lúc tải; mọi cách giả hiệu đều tác động sau đó.

### Chuyển lên bậc cao khi chỉ cần loại bỏ

Dùng không gian được phê chuẩn hoặc xin phép nghe cẩn thận, nhưng nếu bỏ thông tin nhận diện đã cho phép làm ngay, bậc cao chỉ tốn thời gian mà không tăng bảo vệ. Đáp án đúng là bậc thấp nhất có tác dụng.

### Cho phép tài liệu vì không có tên

Độ nhạy cảm không chỉ là thông tin nhận diện. Nghĩa vụ bảo mật, bí mật thương mại và hạn chế hợp đồng bên thứ ba vẫn ràng buộc dù không có tên ai. Đây là lỗi nhận diện người làm nghề hay mắc nhất.

### Trả lời bằng thời hạn lưu hoặc mặc định huấn luyện học thuộc

Số liệu lưu giữ, mặc định và ngày hiệu lực là sự thật sản phẩm phụ thuộc thời điểm, đã thay đổi ngay trong lịch sử tài liệu. Câu hỏi chọn hành vi bền vững: kiểm tra tài liệu hiện hành cho sản phẩm và thỏa thuận của bạn.

## Tình huống luyện tập

Điều phối viên chương trình đào tạo lái xe buýt nhỏ muốn hiểu vì sao tỷ lệ đỗ giảm năm nay. Hồ sơ có tên, số giấy phép, ngày sinh và khai báo đủ sức khỏe của học viên. Chính sách chỉ cho đưa thông tin cá nhân hoặc sức khỏe vào AI khi nhiệm vụ không thể làm nếu thiếu chúng. Cách phù hợp nhất là gì?

**Phương án A**

Bỏ thông tin nhận diện và khai báo sức khỏe, rồi phân tích tỷ lệ đỗ theo nhóm học viên, giảng viên và ngày khóa học.

**Phương án B**

Tải nguyên hồ sơ vì đây là đánh giá nội bộ và kết quả ở lại chương trình.

**Phương án C**

Kết luận hồ sơ quá nhạy cảm để Claude tiếp cận, tổng hợp năm nay trên giấy.

**Phương án D**

Tải hồ sơ với chỉ dẫn bảo mật trong prompt, rồi xóa chat khi phân tích xong.

## Bài tập thực hành: Áp dụng các bậc cho một tập dữ liệu thật

**Thời gian:** 30 phút.

### Bạn sẽ học được

- Liệt kê thành phần nhạy cảm trong tài liệu thật.
- Tách điều câu hỏi cần khỏi những gì tài liệu chứa.
- Loại bỏ, tổng hợp trước khi chuyển cấp xử lý.
- Xác định cách được phép hoặc người phụ trách khi thành phần nhạy cảm là thiết yếu.

### Bước 1 — Chọn tài liệu hoặc dữ liệu bạn thực sự muốn được hỗ trợ

Liệt kê nhận diện, sức khỏe, tài chính, trẻ em, nghĩa vụ bảo mật, bí mật thương mại, tài liệu bên thứ ba theo hợp đồng.

**Vì sao:** Nhận diện đi trước kỹ thuật. Nhóm hay bị bỏ sót chỉ hiện ra khi chủ động tìm.

**Kết quả cần thấy:** Danh sách từng thành phần kèm vì sao nhạy cảm: nhận diện ai, thuộc ai hoặc có cam kết gì.

### Bước 2 — Viết câu hỏi thực sự cần trả lời

Đánh dấu thành phần nhạy cảm mà câu hỏi thực sự cần.

**Vì sao:** Khoảng cách giữa nội dung tài liệu và nhu cầu câu hỏi là nơi các bậc phát huy tác dụng.

**Kết quả cần thấy:** Câu hỏi một câu và danh sách thiết yếu ngắn hơn nhiều; có thể ít hơn bạn nghĩ.

### Bước 3 — Áp dụng hai bậc đầu

Bỏ điều không cần; tổng hợp hoặc ẩn danh điều chỉ cần ở mức khái quát.

**Vì sao:** Bậc thấp nhất có tác dụng là đáp án chuyên nghiệp và thường cho phép làm ngay hôm nay.

**Kết quả cần thấy:** Bản đã bỏ nhận diện, thành phần nhạy cảm còn lại được giảm thành nhóm hoặc khoảng.

### Bước 4 — Nếu thành phần nhạy cảm thực sự thiết yếu, xác định cách được phép

Nếu có, nêu cách được phê chuẩn; nếu không, xác định người phụ trách dữ liệu hoặc chính sách, soạn yêu cầu ngắn sẽ gửi họ.

**Vì sao:** Chuyển xử lý là hành động, không phải từ chối. Nêu người hay cách thực tế phân biệt nó với do dự chung chung.

**Kết quả cần thấy:** Tên không gian được phê chuẩn cho loại tài liệu hoặc yêu cầu hai câu đến người phụ trách cụ thể.

### Bước 5 — Ghi biện pháp giả hiệu bạn dễ bị cám dỗ nhất

Giải thích một câu vì sao nó không phải kiểm soát.

**Vì sao:** Nhận ra cám dỗ của mình giúp tránh phiên bản gây nhiễu khi chịu áp lực thi.

**Kết quả cần thấy:** Một câu bằng lời của bạn giải thích biện pháp ấy hoạt động sau khi đã tiết lộ.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Bạn lưu dữ liệu của tôi bao lâu? — *How long do you store my data?*
- Dữ liệu của tôi có dùng để huấn luyện mô hình không? (sản phẩm tiêu dùng) — *Is my data used for model training? (consumer products)*.
- Dữ liệu của tôi có dùng để huấn luyện mô hình không? (sản phẩm thương mại) — *Is my data used for model training? (commercial products)*.
- Anthropic bảo vệ dữ liệu cá nhân của người dùng Claude thế nào? — *How does Anthropic protect the personal data of Claude users?*
- Chính sách sử dụng — *Usage Policy*.
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

**Ghi chú của tác giả bài gốc:** Thứ tự các bậc và nguyên tắc biện pháp giả hiệu đến từ giải thích Câu hỏi mẫu 3. Tra cứu nhanh Lĩnh vực 6 có chi tiết lưu giữ, xóa hiện hành kèm ngày.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [6.1 — Nhận diện trường hợp sử dụng phù hợp và không phù hợp](6-1-appropriate-use-cases.vi.md).
- **Bài tiếp theo:** [6.3 — Tuân thủ chính sách AI và tiêu chuẩn quản trị của tổ chức](6-3-organisational-ai-policies.vi.md).
