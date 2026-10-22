# 5.4 — Thông báo, duy trì và cập nhật cấu hình

- **Lĩnh vực (Domain):** 5
- **Nhiệm vụ (Task):** 5.4
- **Tên bài gốc:** Informing, Maintaining, and Updating Configurations
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/5-configuration-knowledge/5-4-maintaining-configurations)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

**Cấu hình (configuration)** là thiết lập của Project: chỉ dẫn tùy chỉnh và kho kiến thức. Claude áp dụng chỉ dẫn cho mọi chat trong Project. Mọi tài liệu tải vào kho kiến thức cũng được sử dụng xuyên suốt các chat trong Project. Giữ cấu hình đúng có ba trách nhiệm: **thông báo, duy trì và cập nhật**. Công việc là kiểm tra theo lịch, chọn lọc thay vì tích lũy và nhớ đến những người cấu hình đang phục vụ.

Một cửa hàng thú cưng đã thiết lập tốt Project từ năm ngoái để trả lời khách hàng. Kho kiến thức chứa bảng giá và chính sách đổi trả. Từ đó không ai đụng đến.

## Ba cách một thiết lập tốt xuống cấp

**Kiến thức lỗi thời.** Tệp tải lên là bản chụp tại một thời điểm; không có gì thông báo rằng nguồn đã được thay thế. Đầu ra tiếp tục trích chính sách, giá hoặc quy trình cũ một cách hoàn toàn tự tin. Ở cửa hàng thú cưng, bảng giá năm ngoái vẫn trả lời các câu hỏi giá.

**Chỉ dẫn lỗi thời.** Chúng áp dụng cho mọi chat, dù hoàn cảnh được mô tả còn tồn tại hay không. Khi người đọc hoặc định dạng thay đổi, quy tắc vẫn tiếp tục áp đặt hoàn cảnh cũ.

**Phạm vi mở rộng dần.** Project hoạt động tốt thu hút công việc lân cận. Mỗi phần thêm vào làm loãng chỉ dẫn viết cho công việc gốc đến khi chúng không còn phù hợp phần nào.

Cả ba nhìn từ bên trong Project đều có vẻ ổn, nên bảo trì phải được lên lịch. Nếu chỉ chờ tín hiệu mới kiểm tra, tín hiệu ấy sẽ không tự xuất hiện.

## Loại bỏ, không tích lũy

Khi tài liệu bị thay thế, hãy bỏ bản cũ. Đừng thêm bản mới cạnh nó. Tính đầy đủ là ưu điểm của kho lưu trữ. Project đang làm việc cần đúng một câu trả lời cho câu hỏi phiên bản nào hiện hành. Kho kiến thức giữ cả hai không cho Claude cách biết điều đó. Cửa hàng tải bảng giá mới và xóa bản cũ.

Hai phương án trung gian đều không phù hợp: tệp ghi chú giải thích bản nào có hiệu lực hoặc chỉ dẫn bảo Claude ưu tiên tài liệu mới hơn. Cả hai đều vá vòng quanh một vấn đề lẽ ra kho kiến thức không nên có.

Sau khi thay tài liệu, cũng đọc lại chỉ dẫn để tìm quy tắc được viết theo câu chữ cũ. Quy tắc thường xuyên trích thời hạn thông báo cũ có thể tồn tại lâu hơn tệp mà nó xuất phát. Ở cửa hàng thú cưng, đó có thể là thời hạn đổi trả năm ngoái.

## Thông báo là bước của con người

Khi đồng nghiệp dùng chung Project, thay đổi không được thông báo sẽ tạo đầu ra họ không giải thích được rồi mất lòng tin. Người thực hiện thay đổi hiếm khi có mặt lúc điều đó xảy ra.

Tài liệu ghi nhận một thông tin về thông báo: thành viên nhận email khi Project lần đầu được chia sẻ với họ. Không có loại thông báo nào được tài liệu ghi nhận cho những lần sửa kiến thức hoặc chỉ dẫn sau đó. Vì vậy, nói với cộng tác viên điều gì thay đổi và khi nào luôn là bước con người phải làm.

Ngày thay đổi quan trọng ngang nội dung thay đổi vì giúp xác định vị trí của công việc đang xử lý. Thư nháp tuần trước có thể được nhận diện là trước lần sửa, thay vì gây tranh luận. Người quản lý cửa hàng cho nhân viên biết tệp nào thay đổi và vào ngày nào. Với gói hỗ trợ cùng chỉnh sửa, nhiều người có thể có quyền sửa một Project. Điều đó càng làm việc thông báo thay đổi trở nên quan trọng.

## Thói quen bảo trì

Thói quen hiệu quả có ba phần.

**Thứ nhất, người phụ trách được nêu tên.** “Nên có ai đó giữ thông tin mới” nghĩa là không ai làm. Project bị lệch dần thường hóa ra không có người phụ trách. Cửa hàng giao trách nhiệm cho người quản lý.

**Thứ hai, mốc rà soát gắn với sự kiện định kỳ thật:** số liệu hằng quý, đợt cập nhật chính sách hoặc bắt đầu mùa. Lời nhắc lịch gắn vào việc vốn diễn ra sẽ được kích hoạt. Ý định chung chung thì không. Cửa hàng rà Project mỗi khi có bảng giá mới.

**Thứ ba, chủ động coi việc loại bỏ là một bước rà soát.** Nội dung được thêm tự nhiên suốt năm. Việc xóa chỉ xảy ra khi ai đó hỏi mục nào đã bị thay thế và mục nào chưa từng dùng.

## Trong bài thi

Hướng dẫn nêu ba trách nhiệm. Mọi tình huống thi của mục tiêu này đều có cùng dạng Project: từng được thiết lập tốt nhưng sau đó lệch dần. Cập nhật là phần ít mang tính quyết định nhất, vì việc này dễ thực hiện một khi đã nhận ra vấn đề. Thông báo được nêu rõ, nhưng gần như mọi người đều bỏ qua.

Có hai ranh giới. Phần dẫn mở đầu bằng đầu ra kém và hỏi điều gì đã sai thuộc Lĩnh vực 7. Project được duy trì hoàn hảo vẫn tạo bản nháp đầu tiên cần xác minh sự thật theo Lĩnh vực 2.

### Bẫy chỉ thêm vào

Phương án giữ cả hai phiên bản có vẻ kỹ lưỡng, cẩn thận. Chính vì thế nó sai: áp bản năng lưu trữ vào công cụ đang làm việc. Đáp án đúng loại bản bị thay thế, rà lại chỉ dẫn và báo cho người sử dụng Project.

### Ghi chú về nguồn

Không có bài viết Anthropic nào đề cập chỉnh sửa cấu hình đã lưu hoặc thông báo cho cộng tác viên rằng nó thay đổi. Bài học dựa trên cách diễn đạt mục tiêu trong hướng dẫn thi, thực hành nghề nghiệp thông thường và thông báo chia sẻ duy nhất được ghi nhận.

## Những bẫy thường gặp trong bài thi

### Tải tài liệu sửa đổi nhưng giữ bản cũ, đôi khi kèm ghi chú bản nào hiện hành

Không có gì xác định cho Claude bản nào có hiệu lực, nên đầu ra có thể trích một trong hai. Project làm việc cần một phiên bản hiện hành và bản cũ được loại bỏ. Tính đầy đủ thuộc kho lưu trữ, không thuộc kho kiến thức làm việc.

### Thêm chỉ dẫn yêu cầu Claude ưu tiên tài liệu mới

Đây là vá chỉ dẫn để đi vòng qua kho kiến thức lẽ ra chỉ cần được chọn lọc. Tài liệu bị thay thế không có lý do ở lại Project đang làm việc. Chính bản vá trở thành quy tắc nữa có thể lỗi thời và cần bảo trì.

### Giả định hệ thống sẽ báo đồng nghiệp cấu hình đã thay đổi

Thông báo duy nhất được ghi nhận là email khi Project lần đầu được chia sẻ. Không có thông báo nào được ghi nhận cho các chỉnh sửa kiến thức hoặc chỉ dẫn sau đó. Vì vậy, đáp án đúng luôn để con người thông báo cộng tác viên.

## Tình huống luyện tập

Một quỹ quản lý trạm quan sát chim có Project mà thư ký phụ trách đặt chỗ cùng hai thành viên ban quản lý dùng cho thư từ đặt chỗ lưu trú qua đêm. Điều khoản đặt chỗ được sửa tháng 3. Các thư bắt đầu trích thời hạn báo hủy cũ; thư ký thấy cả hai bản điều khoản trong kiến thức Project. Quỹ muốn tiếp tục dùng Project làm không gian xử lý đặt chỗ. Cô nên làm gì?

**Phương án A**

Loại điều khoản đã bị thay thế, kiểm tra chỉ dẫn xem có quy tắc viết theo câu chữ cũ không, báo hai thành viên còn lại điều gì thay đổi và khi nào.

**Phương án B**

Ngừng dùng Project cho thư đặt chỗ; để mỗi thành viên đính kèm điều khoản hiện hành vào mọi chat mới.

**Phương án C**

Tải lại bản tháng 3 và thêm dòng vào chỉ dẫn tùy chỉnh yêu cầu Claude ưu tiên tài liệu mới hơn khi hai bản không thống nhất.

**Phương án D**

Thêm tệp ghi chú vào kho kiến thức nói bản tháng 3 là hiện hành; giữ cả hai bản để Project có hồ sơ đầy đủ về cách điều khoản đã thay đổi.

## Bài tập thực hành: Rà soát ba lượt

**Thời gian:** 30 phút.

### Bạn sẽ học được

- Cách rà chỉ dẫn để tìm mong muốn chung chung, quy tắc lỗi thời và câu chữ không còn cơ sở áp dụng.
- Cách phân biệt kiến thức hiện hành, bị thay thế và chưa từng dùng.
- Cách xác định người phụ trách và gắn lần rà tiếp theo với sự kiện thật.
- Cách viết ghi chú thay đổi một câu mà cộng tác viên cần.

### Bước 1 — Mở Project đang dùng và cam kết rà trong ba lượt

Dùng Project hiện có hoặc Project đã tạo ở những bài tập trước của lĩnh vực này.

**Vì sao:** Sự lệch dần khó nhìn thấy trong sử dụng hằng ngày. Chỉ rà soát có chủ đích mới làm nó lộ ra.

**Kết quả cần thấy:** Chỉ dẫn và danh sách kiến thức được mở cạnh nhau.

### Bước 2 — Lượt một: Kiểm tra từng dòng chỉ dẫn tùy chỉnh

Đó là hành vi đồng nghiệp có thể làm theo, mong muốn chung chung hay quy tắc viết cho tình huống đã qua? Viết lại hoặc xóa tương ứng.

**Vì sao:** Chỉ dẫn lỗi thời vì tồn tại lâu hơn hoàn cảnh nó mô tả. Rà soát là lúc quy tắc không còn cơ sở áp dụng cuối cùng được phát hiện.

**Kết quả cần thấy:** Bộ chỉ dẫn ngắn hơn, mọi dòng đều kiểm tra được và vẫn đúng hiện tại.

### Bước 3 — Lượt hai: Kiểm tra từng mục trong kho kiến thức

Mục đó hiện hành, đã bị thay thế hay chưa thực sự dùng? Loại bản bị thay thế thay vì thêm ghi chú cạnh nó; loại mọi thứ chưa từng cần.

**Vì sao:** Loại bỏ là bước không tự nhiên diễn ra. Tài liệu bị thay thế là một cách tạo ra câu trả lời sai đầy tự tin.

**Kết quả cần thấy:** Danh sách kiến thức được tinh gọn, chỉ một phiên bản cho mỗi tài liệu, có ghi ngày tải.

### Bước 4 — Lượt ba: Xử lý những phần chưa có người phụ trách

Ghi ai phụ trách Project, sự kiện định kỳ thật nào kích hoạt lần rà tiếp theo và một câu bạn sẽ gửi cho mọi người dùng khác để mô tả vừa thay đổi gì, khi nào.

**Vì sao:** Người phụ trách cụ thể và yếu tố kích hoạt thật khiến lần rà tiếp theo diễn ra. Ghi chú thay đổi thực hiện đúng phần thông báo.

**Kết quả cần thấy:** Người phụ trách, mốc kích hoạt có ngày và ghi chú thay đổi một câu sẵn sàng gửi.

### Bước 5 — Nếu chưa nêu được người phụ trách, xem đó là phát hiện

Thống nhất với những người dùng khác ai chịu trách nhiệm trước khi kết thúc rà soát.

**Vì sao:** Project lệch dần thường hóa ra không có người phụ trách. Khắc phục điều đó có giá trị lâu dài hơn từng chỉnh sửa riêng ở lượt một và hai.

**Kết quả cần thấy:** Một người cụ thể gắn trách nhiệm với Project, kể cả chính bạn.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Quản lý khả năng hiển thị và chia sẻ Project — *Manage project visibility and sharing*.
- Tôi có thể tạo và quản lý Project như thế nào? — *How can I create and manage projects?*
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

**Ghi chú của tác giả bài gốc:** Không có bài viết Anthropic nào đề cập chỉnh sửa cấu hình đã lưu, loại tệp kiến thức hoặc thông báo thay đổi cho cộng tác viên. Bài học dựa trên mục tiêu trong hướng dẫn thi và thực hành tiêu chuẩn; bài viết về chia sẻ ghi nhận thông báo duy nhất đó.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [5.3 — Tạo chỉ dẫn cấp hệ thống hiệu quả](5-3-system-level-instructions.vi.md).
- **Bài tiếp theo:** Nhận diện trường hợp sử dụng phù hợp và không phù hợp — *Identifying Appropriate and Inappropriate Use Cases*.
