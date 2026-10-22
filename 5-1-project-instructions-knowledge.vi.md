# 5.1 — Cấu hình Project với chỉ dẫn và nguồn kiến thức

- **Lĩnh vực (Domain):** 5
- **Nhiệm vụ (Task):** 5.1
- **Tên bài gốc:** Configuring Projects with Instructions and Knowledge Sources
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/5-configuration-knowledge/5-1-project-instructions-knowledge)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

### Hai nơi lưu, hai nhiệm vụ

Trung tâm trợ giúp của Anthropic mô tả **Project** là không gian làm việc độc lập có lịch sử trò chuyện và kho kiến thức riêng. Project có hai phần có thể cấu hình, được hướng dẫn riêng vì chúng thực hiện hai nhiệm vụ khác nhau. **Chỉ dẫn tùy chỉnh (custom instructions)** là nơi đặt cách Claude nên hành xử và trả lời. Chúng điều chỉnh câu trả lời, chẳng hạn dùng giọng văn trang trọng hơn hoặc trả lời từ góc nhìn của một vai trò hay ngành cụ thể. **Kiến thức Project (project knowledge)** là tài liệu Claude dùng làm cơ sở. Bạn tải tài liệu, văn bản và tệp liên quan vào kho kiến thức. Claude dựa vào chúng để hiểu bối cảnh và thông tin nền của các chat trong Project. Chỉ dẫn trả lời “công việc này nên được thực hiện như thế nào?”. Kiến thức trả lời “nên thực hiện dựa trên tài liệu gì?”.

Hãy xét một công ty vệ sinh cửa kính có người quản lý viết báo giá và thư nhắc hằng tuần. Mỗi lần, cô đều dặn Claude viết cho chủ nhà bằng từ ngữ dễ hiểu và nêu ngày ghé làm dịch vụ tiếp theo. Mỗi lần, cô đều đính kèm bảng giá, điều khoản dịch vụ và những thư trả lời tốt trước đây. Cả hai phần đều là thao tác thiết lập thông thường trên màn hình Project: viết và lưu chỉ dẫn, sau đó dùng nút thêm để tải các tệp kiến thức lên.

## Phép kiểm tra nơi lưu

Thiết lập Project tốt phụ thuộc vào một quyết định phân loại được áp dụng cho từng mục: đây là quy tắc về hành vi hay tài liệu để tham khảo? Với công ty vệ sinh cửa kính, “viết cho chủ nhà bằng từ ngữ dễ hiểu” là hành vi, nên đưa vào chỉ dẫn. Bảng giá là tài liệu, nên đưa vào kho kiến thức.

Phép kiểm tra này quan trọng vì mỗi nơi có đặc điểm mà nơi còn lại không có. Claude áp dụng chỉ dẫn cho mọi chat trong Project. Kiến thức được tham khảo khi công việc cần đến. Khi tài liệu được cập nhật, có thể thay tệp kiến thức bằng một thao tác. Chính sách dán vào chỉ dẫn thì phải được tìm và cắt bỏ bằng tay.

## Hai kiểu lỗi do đặt sai nơi

Lỗi thứ nhất là dán tài liệu tham khảo vào chỉ dẫn, thường được trình bày như sự cẩn thận: đặt toàn bộ chính sách ở nơi Claude không thể bỏ sót. Các quy tắc hành vi khi đó bị chìm trong nội dung đã dán. Khi chính sách được sửa, văn bản cũ mắc lại ở nơi không thể thay thế gọn gàng. Nếu dán điều khoản dịch vụ vào chỉ dẫn, hai quy tắc của công ty sẽ nằm giữa nhiều trang điều khoản.

Lỗi thứ hai theo chiều ngược lại: chôn một quy tắc trong kho kiến thức. Hướng dẫn văn phong của tổ chức được tải lên dưới dạng tài liệu là tài liệu về hành vi, chưa phải chỉ dẫn. Không có gì đánh dấu rằng nó phải chi phối mọi câu trả lời, nên nó chỉ được áp dụng khi Project tình cờ tham khảo đến. Hướng dẫn văn phong của công ty tải dưới dạng kiến thức sẽ chỉ được tuân thủ một số lần. Thỉnh thoảng tuân thủ không phải tiêu chuẩn. Quy tắc mà công việc luôn phụ thuộc vào phải nằm trong chỉ dẫn và được diễn đạt thành hành vi.

## Xây dựng thiết lập từ những gì bạn đang làm

Phương pháp này không cần phân tích mới, vì người đang làm thủ công vốn đã có cả hai danh sách. Những gì bạn giải thích lại ở đầu mọi cuộc trò chuyện là bộ chỉ dẫn: người đọc, giọng văn, định dạng và quy tắc áp dụng thường xuyên. Những gì bạn đính kèm lại là kho kiến thức: chính sách, mẫu và ví dụ trước đây. Ở công ty vệ sinh cửa kính, hai quy tắc trở thành chỉ dẫn, ba tệp trở thành kiến thức. Viết danh sách đầu thành hành vi và tải danh sách sau lên dưới dạng tệp. Sau đó thực hiện nhiệm vụ thật tiếp theo bằng prompt ngắn chỉ nêu nhiệm vụ, ghi lại những gì bạn không còn phải nói lại.

## Trong bài thi

Mục tiêu này bắt đầu sau quyết định dùng Project và kiểm tra việc thiết lập Project tốt. Công việc có cần Project hay không là phán đoán của Lĩnh vực 3. Project nằm ở đâu trong quy trình rộng hơn là nội dung của Lĩnh vực 4. Phần lớn câu hỏi ở đây là phép kiểm tra nơi lưu được đặt trong tình huống; hãy luyện đến khi thành phản xạ. Cả hai lỗi đặt sai nơi đều phổ biến trong thiết lập thực tế và tạo phương án gây nhiễu hiệu quả. Vì phần dẫn bắt đầu sau quyết định đó, “dùng Project” không bao giờ là đáp án đúng ở đây. Phương án quay lại tranh luận chuyện đó đã lạc về Lĩnh vực 3.

### Khái niệm cốt lõi

Khi câu hỏi đưa ra các cách thiết lập khác nhau, hãy áp dụng phép kiểm tra nơi lưu cho từng thành phần trong phần dẫn. Đáp án đúng đưa hành vi vào chỉ dẫn và tài liệu vào kiến thức. Các phương án gây nhiễu đưa ít nhất một thành phần sai chiều, thường dưới danh nghĩa cẩn thận hoặc gọn gàng.

## Những bẫy thường gặp trong bài thi

### Dán tài liệu tham khảo vào chỉ dẫn tùy chỉnh để Claude không thể bỏ sót

Quy tắc hành vi bị chìm trong nội dung đã dán. Khi tài liệu được sửa, văn bản cũ mắc lại trong chỉ dẫn thay vì được thay bằng tệp kiến thức mới. Sự cẩn thận chính là vẻ ngoài của phương án gây nhiễu này.

### Tải quy tắc dùng thường xuyên thành tài liệu kiến thức và mong nó chi phối mọi câu trả lời

Kiến thức là tài liệu Claude tham khảo, không phải hành vi áp dụng thường xuyên. Quy tắc phải đúng mọi lần chỉ được áp dụng đôi lúc nếu không được nêu trong chỉ dẫn. Bảo đảm hành vi nhất quán chính là nhiệm vụ của chỉ dẫn.

### Bỏ Project và giải thích, đính kèm lại mọi thứ trong từng chat để giữ thông tin mới

Tính cập nhật được xử lý bằng cách thay tệp kiến thức khi tài liệu nguồn thay đổi. Cách làm vòng theo từng chat đưa trở lại đúng phần việc lặp mà Project loại bỏ, đồng thời phụ thuộc vào việc mọi người dùng đều nhớ làm.

## Tình huống luyện tập

Thư ký hiệp hội người thuê nhà và cư dân đã quyết định đưa việc xử lý các vụ việc trong khu dân cư cùng tài liệu họp hằng tháng vào một Project và đang thiết lập nó. Cô có hai thành phần: chính sách sửa chữa của hiệp hội và quy tắc mọi lá thư phải nêu cán bộ phụ trách cùng ngày vấn đề sửa chữa được báo. Mỗi thành phần nên nằm ở đâu?

**Phương án A**

Tải chính sách sửa chữa vào kiến thức Project, viết quy tắc nêu cán bộ phụ trách và ngày báo vấn đề vào chỉ dẫn tùy chỉnh.

**Phương án B**

Dán chính sách sửa chữa vào chỉ dẫn tùy chỉnh để Claude không thể bỏ qua; tải ghi chú hướng dẫn ngắn đề cập quy tắc cán bộ phụ trách vào kiến thức Project.

**Phương án C**

Tải cả chính sách sửa chữa và tài liệu nêu quy tắc cán bộ phụ trách thành tệp kiến thức; để trống chỉ dẫn tùy chỉnh để Project linh hoạt.

**Phương án D**

Giữ cả hai ngoài Project, đính kèm lại chính sách và nhắc lại quy tắc ở đầu mỗi chat mới, vì tài liệu vừa dán luôn là phiên bản hiện hành.

## Bài tập thực hành: Phân loại một tháng công việc thủ công vào hai nơi lưu

**Thời gian:** 25 phút.

### Bạn sẽ học được

- Cách nhận ra bộ chỉ dẫn ẩn trong những gì bạn giải thích lại ở mỗi chat.
- Cách nhận ra kho kiến thức ẩn trong những gì bạn đính kèm lại.
- Cách áp dụng phép kiểm tra nơi lưu cho các mục chưa rõ.
- Cách xác nhận thiết lập hiệu quả qua những gì bạn không còn phải nói lại.

### Bước 1 — Chọn công việc lặp lại hiện đang làm trong chat thông thường

Chọn việc mà bạn phải giải thích lại bối cảnh và đính kèm lại tệp mỗi lần.

**Vì sao:** Hai danh sách Project cần vốn đã tồn tại trong thói quen thủ công. Công việc lặp lại giúp nhìn ra chúng.

**Kết quả cần thấy:** Một dòng nêu nhiệm vụ và tần suất lặp lại.

### Bước 2 — Viết hai danh sách từ ký ức về các chat gần nhất

Danh sách thứ nhất gồm những gì bạn giải thích lại: người đọc, giọng văn, định dạng, quy tắc thường xuyên. Danh sách thứ hai gồm những gì đính kèm lại: chính sách, mẫu, ví dụ và dữ liệu.

**Vì sao:** Danh sách giải thích lại là bộ chỉ dẫn; danh sách đính kèm lại là kho kiến thức. Chính hành vi của bạn đã thực hiện việc phân loại.

**Kết quả cần thấy:** Hai danh sách được viết ra: một về hành vi, một về tài liệu.

### Bước 3 — Tạo Project và đưa mỗi danh sách vào nơi phù hợp

Viết danh sách đầu vào chỉ dẫn tùy chỉnh theo dạng hành vi; tải danh sách sau làm kiến thức Project.

**Vì sao:** Diễn đạt chỉ dẫn thành hành vi giúp kiểm tra được; tải tài liệu thật lên hữu ích hơn mô tả lại.

**Kết quả cần thấy:** Bộ chỉ dẫn đã lưu và kho kiến thức đã có tài liệu trên màn hình Project.

### Bước 4 — Áp dụng phép kiểm tra nơi lưu cho từng mục chưa rõ

Hỏi đây là quy tắc hành vi hay tài liệu tham khảo. Di chuyển mục đang nằm sai phần.

**Vì sao:** Những mục chưa rõ là nơi thiết lập thực tế hay sai; phép kiểm tra giải quyết từng trường hợp bằng một câu hỏi.

**Kết quả cần thấy:** Ít nhất một mục được di chuyển hoặc ghi chú rằng mọi mục đều đã ở đúng nơi.

### Bước 5 — Thực hiện nhiệm vụ thật tiếp theo bằng prompt ngắn chỉ nêu nhiệm vụ

Ghi lại những gì không còn phải giải thích.

**Vì sao:** Bằng chứng của thiết lập tốt là prompt ngắn lại. Điều vẫn phải giải thích thuộc một trong hai nơi lưu.

**Kết quả cần thấy:** Đầu ra đầu tiên tương đương tiêu chuẩn thông thường của bạn, từ prompt ngắn hơn nhiều.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Project là gì? — *What are projects?*
- Tôi có thể tạo và quản lý Project như thế nào? — *How can I create and manage projects?*
- Hạn mức sử dụng và giới hạn độ dài hoạt động như thế nào? — *How do usage and length limits work?*
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [4.5 — Truyền đạt giá trị và giới hạn cho các bên liên quan](4-5-communicating-value-limitations.vi.md).
- **Bài tiếp theo:** [5.2 — Quản lý kiến thức tải lên và trình kết nối](5-2-uploads-and-connectors.vi.md).
