# 4.1 — Phân tích yêu cầu và trường hợp sử dụng

- **Lĩnh vực (Domain):** 4
- **Nhiệm vụ (Task):** 4.1
- **Tên bài gốc:** Analysing Requirements and Use Cases
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/4-workflow-integration/4-1-requirements-and-use-cases)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

**Yêu cầu (requirement)** là phát biểu về điều một công việc phải đạt được. **Phân tích trường hợp sử dụng (use-case analysis)** là đánh giá một nhiệm vụ có phù hợp để giao cho Claude hay không trước khi đầu tư công sức. **Chủ đề (theme)** là nhóm các ý kiến liên quan được đặt tên. Mục tiêu này kiểm tra hai kỹ năng có liên hệ: dùng Claude biến đầu vào lộn xộn thành yêu cầu có cấu trúc và phân tích trường hợp sử dụng. Mọi quyết định về quy trình trong lĩnh vực này bắt đầu từ đó: công việc đòi hỏi gì và Claude có phù hợp để tham gia vào bất kỳ phần nào không? Một nguyên tắc kết nối cả hai: Claude tổ chức thông tin; con người xác thực và chịu trách nhiệm về kết quả.

Hãy xét một cửa hàng bán báo có dịch vụ giao tận nhà. Chủ cửa hàng muốn tổ chức lại các tuyến giao báo. Tài liệu của cô gồm email khách hàng, ghi chép họp nhân viên, nhận xét trong sổ đơn hàng và các ý kiến trao đổi tại quầy.

## Tạo cấu trúc từ đầu vào lộn xộn

Yêu cầu thực tế xuất hiện qua chuỗi khiếu nại, ghi chép cuộc họp, ý kiến khảo sát và các cuộc trò chuyện chỉ còn được nhớ một phần, chứ không phải danh sách gọn gàng. Trung tâm trợ giúp liệt kê tóm tắt tài liệu và cuộc trò chuyện dài trong số công dụng cốt lõi của Claude, cùng với tạo các góc nhìn và đưa ra khuyến nghị. Khi được cung cấp tài liệu thô, Claude nhóm chúng theo chủ đề và phân biệt điều mọi người yêu cầu với điều có vẻ là nhu cầu thực sự của họ. Nó cũng chỉ ra nơi hai nhóm muốn những điều không thể đồng thời đáp ứng và nêu những gì chưa ai nhắc tới.

Với cửa hàng báo, Claude có thể đưa ra các chủ đề như báo giao muộn và giao nhầm tạp chí. Nó có thể đánh dấu một khu dân cư muốn nhận báo trước 7 giờ, trong khi nhân viên muốn bắt đầu muộn hơn. Công việc đọc tài liệu mất cả buổi chiều trở thành vài phút; những người liên quan có được cách phác họa vấn đề để xem xét và chất vấn.

## Chủ đề là một giả thuyết

Claude tổ chức những gì được cung cấp. Nó không có cách nào tự biết tổ chức bạn cần gì. Chủ đề nó đặt tên là giả thuyết về đầu vào, không phải kết luận đã xác nhận về doanh nghiệp. Những người có yêu cầu được mô tả phải xác nhận trước khi bất kỳ phương án nào được thiết kế dựa trên đó. Khung AI Fluency của Anthropic cũng phân chia trách nhiệm tương tự. **Khả năng phân định (Discernment)** — đánh giá những gì AI tạo ra — và **sự cẩn trọng, trách nhiệm (Diligence)** — duy trì trách nhiệm đối với kết quả — thuộc về con người.

Vì vậy, chủ cửa hàng xác nhận mâu thuẫn về giờ giao báo sớm với khách hàng ở khu dân cư và nhân viên trước khi điều chỉnh bất kỳ tuyến nào. Thiết kế trực tiếp từ các nhóm do Claude tạo sẽ nhầm đầu ra gọn gàng với yêu cầu đã được xác thực. Xác nhận là phần ít tốn công.

## Đặc điểm của công việc phù hợp

Các trường hợp sử dụng Claude phù hợp có những đặc điểm dễ nhận ra:

- Công việc chủ yếu liên quan đến ngôn ngữ: soạn thảo, tóm tắt, định dạng lại, giải thích, so sánh. Đây là phạm vi được bài viết về trường hợp sử dụng của Trung tâm trợ giúp ghi nhận.
- Bạn có thể cung cấp tài liệu cần thiết.
- Đầu ra có thể được người đủ năng lực kiểm tra.
- Hoặc khối lượng công việc lớn, hoặc việc bắt đầu từ trang trắng là phần tốn công nhất.

AI Fluency gọi sự phán đoán này là **Giao việc (Delegation)** — quyết định công việc nào giao cho AI. Khung này xem Delegation là kỹ năng riêng, diễn ra trước khi viết bất kỳ prompt nào. Công việc ít phù hợp có đặc điểm ngược lại: cần thẩm quyền ra quyết định thay vì khả năng soạn thảo; phụ thuộc vào thông tin Claude không có quyền truy cập; hoặc là công việc duy trì quan hệ thay vì xử lý tài liệu.

Ở cửa hàng báo, thư thông báo giờ giao mới là trường hợp phù hợp vì chủ cửa hàng có thể kiểm tra. Chọn ai phụ trách tuyến nào cần thẩm quyền. Biết tờ báo đã được giao đến cửa nhà hay chưa cần thông tin Claude không có. Gọi cho khách quen vừa hủy dịch vụ là công việc duy trì quan hệ.

## Phép kiểm tra về người kiểm chứng

Đây là phép kiểm tra mọi người thường bỏ qua: nếu bạn không thể nhận ra câu trả lời sai, bạn chưa sẵn sàng dùng Claude cho nhiệm vụ đó. Không có người kiểm chứng, đầu ra sai được chấp nhận dễ như đầu ra đúng. Mức độ hệ trọng cao không phải lý do để bỏ công việc; thiếu người kiểm chứng cũng vậy. Cả hai đều đòi hỏi tìm người phân biệt được đầu ra tốt và kém rồi đưa họ vào quy trình.

Phép kiểm tra này cũng giúp phân rã trường hợp sử dụng kiểu giao toàn quyền: tuyên bố rằng Claude sẽ xử lý cả một nhóm công việc. Một nhóm công việc trộn cả nhiệm vụ phù hợp và không phù hợp. Cam kết áp dụng đồng loạt xuất hiện trước bước phân tích vốn phải định hình nó. Giao toàn bộ hành chính giao báo cho Claude sẽ gộp cả viết thư với phân bổ tuyến giao.

## Trong bài thi

Sai lầm thường được bài thi khai thác ở đây là bỏ qua bước xác nhận. Công việc có phù hợp với Claude hay không và phù hợp ở phần nào là câu hỏi của mục tiêu này. Diễn đạt yêu cầu sau đó như thế nào là kỹ năng của Lĩnh vực 1; dùng tính năng sản phẩm nào là kỹ năng của Lĩnh vực 3.

### Khái niệm cốt lõi

Khi phần dẫn của mục tiêu 4.1 kết thúc ở chỗ Claude vừa nhóm xong các chủ đề, đáp án đúng mang chúng trở lại những người sở hữu yêu cầu để xác nhận trước khi bắt đầu thiết kế. Các phương án gây nhiễu chấp nhận chủ đề như kết luận đã được xác nhận, giao luôn quyết định cho Claude hoặc bỏ công việc vì cảm thấy quá hệ trọng.

## Những bẫy thường gặp trong bài thi

### Chấp nhận chủ đề của Claude như kết luận đã xác thực vì chúng có nhanh và nghe hợp lý

Chủ đề là giả thuyết về đầu vào, không phải kết luận về doanh nghiệp. Thiết kế dựa trên mâu thuẫn chưa được xác nhận khiến bạn tự tin xây sai thứ cần xây. Vì vậy, đáp án đúng mang cấu trúc trở lại các bên liên quan trước. Xác nhận là bước ít tốn công; bỏ qua nó mới tốn kém.

### Giao cả quyết định cho Claude cùng với phần phân tích

Thẩm quyền ra quyết định không được giao cho AI. Claude tổ chức tài liệu và soạn nội dung xoay quanh quyết định, nhưng chọn chính sách, chọn bên thắng hoặc giải quyết tranh chấp vẫn thuộc những người chịu trách nhiệm. Phương án giao phán đoán ra ngoài là sai dù nghe hiệu quả đến đâu.

### Loại bỏ công việc vì cho rằng quá quan trọng để Claude tham gia

Tránh dùng hoàn toàn là nhầm mức độ hệ trọng với rủi ro. Hệ trọng cao đòi hỏi người kiểm chứng đủ năng lực được nêu rõ trong quy trình, không đòi hỏi từ bỏ sự hỗ trợ soạn thảo. Phép kiểm tra về người kiểm chứng là cách xử lý; bài thi xem từ chối đồng loạt là sai cũng như áp dụng đồng loạt.

## Tình huống luyện tập

Người quản lý một khu chợ đường phố vào thứ Bảy có thư mục email khiếu nại và ý kiến tiểu thương về cách phân bổ vị trí sạp. Cô muốn xác định phương án phân bổ công bằng hơn phải đáp ứng điều gì trước khi có người thiết kế. Claude nhóm tài liệu thành sáu chủ đề, gồm một mâu thuẫn: người bán thường xuyên cho rằng người bán không thường xuyên được các vị trí góc tốt nhất, trong khi người bán không thường xuyên mô tả chính những vị trí góc đó là dành riêng cho người bán thường xuyên. Cô không có thời gian tự đọc lại cả thư mục. Nên làm gì tiếp theo?

**Phương án A**

Xem các chủ đề là giả thuyết về đầu vào và mang trở lại tiểu thương để xác nhận, bắt đầu từ mâu thuẫn, trước khi triển khai bất kỳ công việc thiết kế nào.

**Phương án B**

Gác thư mục đó sang một bên và tự đọc lại mọi email, vì phân bổ vị trí sạp quá dễ gây tranh cãi để Claude được tham gia.

**Phương án C**

Giao toàn bộ vấn đề phân bổ: đưa Claude sơ đồ vị trí sạp và danh sách tiểu thương, yêu cầu tạo phương án công bằng nhất có thể cho mùa tiếp theo.

**Phương án D**

Chấp nhận sáu chủ đề thành tài liệu yêu cầu vì chúng đến trực tiếp từ lời của tiểu thương, rồi chuyển sang thiết kế cách phân bổ mới.

## Bài tập thực hành: Nhóm chủ đề, xác nhận rồi phân loại

**Thời gian:** 30 phút.

### Bạn sẽ học được

- Cách nhờ Claude tổ chức đầu vào thực sự lộn xộn.
- Cách xem chủ đề là giả thuyết và xác nhận với người sở hữu yêu cầu.
- Cách phân loại công việc dự kiến theo mức độ phù hợp với Claude.
- Cách áp dụng phép kiểm tra về người kiểm chứng trước khi cam kết một trường hợp sử dụng.

### Bước 1 — Thu thập đầu vào thực sự lộn xộn mà bạn phụ trách

Ví dụ: chuỗi phản hồi, ghi chép từ ba cuộc họp nhóm gần nhất hoặc thư mục khiếu nại về một quy trình.

**Vì sao:** Kỹ năng chỉ thể hiện khi gặp sự lộn xộn thực tế. Đầu vào gọn gàng che khuất chính phần tổ chức thông tin mà mục tiêu kiểm tra.

**Kết quả cần thấy:** Một tập tài liệu thô chưa biên tập, được tập hợp trong một tài liệu hoặc cuộc trò chuyện.

### Bước 2 — Yêu cầu Claude nhóm theo chủ đề, chỉ ra mâu thuẫn và khoảng trống

Nhờ Claude nhóm tài liệu, đánh dấu nơi hai người muốn những điều không thể đồng thời đáp ứng và nêu những gì chưa ai nhắc tới.

**Vì sao:** Ba yêu cầu bao quát những gì khó nhìn ra nhất trong tài liệu: khuôn mẫu, mâu thuẫn và điều còn vắng mặt.

**Kết quả cần thấy:** Các chủ đề có tên, ít nhất một điểm xung đột được đánh dấu và một hoặc hai khoảng trống.

### Bước 3 — Phân biệt chủ đề đã xác nhận với giả thuyết và xác nhận các điểm quan trọng

Đánh dấu từng chủ đề là “đã xác nhận” hoặc “giả thuyết”. Mang hai giả thuyết làm cơ sở quan trọng nhất trở lại người sở hữu để xác nhận và ghi điều thay đổi.

**Vì sao:** Đây là kỷ luật bài thi kiểm tra: chủ đề vẫn là giả thuyết về đầu vào cho đến khi người sở hữu yêu cầu xác nhận.

**Kết quả cần thấy:** Ít nhất một chủ đề được sửa hoặc định khung lại sau một cuộc trao đổi thực tế.

### Bước 4 — Liệt kê công việc từ yêu cầu đã xác nhận và phân loại

Phân thành công việc liên quan đến ngôn ngữ với tài liệu có thể cung cấp, hoặc công việc phụ thuộc thẩm quyền, quyền truy cập hay quan hệ.

**Vì sao:** Phân tích trường hợp sử dụng diễn ra cho từng công việc, không bao giờ áp chung cả nhóm công việc. Phân loại giúp nhìn rõ việc phù hợp và không phù hợp.

**Kết quả cần thấy:** Hai danh sách, mỗi công việc nằm đúng một danh sách.

### Bước 5 — Xác định người kiểm chứng cho mọi công việc định giao Claude

Nêu người có thể phân biệt đầu ra sai và đúng. Nếu chưa xác định được ai, trường hợp sử dụng chưa sẵn sàng.

**Vì sao:** Phép kiểm tra về người kiểm chứng là bộ lọc sắc bén nhất trong mục tiêu; nêu một người thực tế khiến phép kiểm tra có ý nghĩa thực chất.

**Kết quả cần thấy:** Mỗi công việc định giao Claude có người kiểm chứng cụ thể bên cạnh hoặc ghi chú cần tìm ai tham gia.

## Tài liệu tham khảo

Các tài liệu được liệt kê trong bản gốc:

- **Anthropic:** Tôi có thể dùng Claude vào những việc gì? — *What are some things I can use Claude for?*
- **Anthropic:** AI Fluency: Khung năng lực và nền tảng — *AI Fluency: Framework and Foundations*.
  - Ghi chú của tác giả bài gốc: tên các thành phần là tên mô-đun của khóa học; phần giải thích ngắn cho từng thành phần là cách tác giả diễn giải nội dung khóa học.
- **Anthropic:** Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.
  - Ghi chú của tác giả bài gốc: đây là hướng dẫn thi; các nhận định về thực hành nghề nghiệp là phán đoán của tác giả, không phải hướng dẫn của Anthropic.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [3.4 — Quản lý giới hạn ngữ cảnh và bộ nhớ: Bắt đầu lại, tóm tắt, lưu giữ](3-4-context-and-memory-management.vi.md).
- **Bài tiếp theo:** Sử dụng Claude cho nghiên cứu, lập kế hoạch và tối ưu hóa quy trình — *Using Claude for Research, Planning and Process Optimisation*.
