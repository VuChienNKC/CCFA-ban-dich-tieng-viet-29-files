# 5.3 — Tạo chỉ dẫn cấp hệ thống hiệu quả

- **Lĩnh vực (Domain):** 5
- **Nhiệm vụ (Task):** 5.3
- **Tên bài gốc:** Creating Effective System-Level Instructions
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/5-configuration-knowledge/5-3-system-level-instructions)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Trong chứng nhận này, **chỉ dẫn cấp hệ thống (system-level instructions)** là những quy tắc dùng thường xuyên mà con người viết bằng tiếng Anh thông thường. Chúng nằm ở một trong ba nơi: thiết lập claude.ai, Project hoặc thiết lập tổ chức dành cho người quản trị. Ở đây không có lớp kỹ thuật nào bên dưới.

Người quản lý văn phòng tại một công ty thợ khóa nhỏ dùng Claude cho email khách hàng, báo giá gửi chủ nhà cho thuê và hướng dẫn an ninh nhà ở. Một số quy tắc áp dụng cho bản thân cô, một số cho báo giá, một số cho mọi người trong công ty và một số chỉ cho tuần này. Hai lựa chọn quyết định quy tắc có hiệu quả hay không: đặt từng quy tắc ở đâu và diễn đạt như thế nào.

## Ba cấp, ba phạm vi

Mỗi cấp có người quản lý và phạm vi áp dụng; cả ba đều được tài liệu ghi nhận.

### Cấp tài khoản (Account-wide)

Thiết lập claude.ai có ô mang nhãn **Instructions for Claude**. Mọi nội dung viết ở đó áp dụng cho tất cả cuộc trò chuyện của bạn. Nội dung được gợi ý mang tính cá nhân, xuyên suốt công việc, chẳng hạn cách tiếp cận ưa thích, thuật ngữ thường dùng và sở thích giao tiếp chung.

### Cấp Project (Project-level)

Chỉ dẫn của Project chỉ điều chỉnh câu trả lời trong các chat thuộc Project đó.

### Cấp tổ chức (Organisation-level)

Trên các gói Team và Enterprise, Owner và Primary Owner có thể đặt chỉ dẫn tổ chức. Claude tuân theo chúng trong mọi cuộc trò chuyện trên toàn tổ chức.

Khi các cấp chồng lấn, chỉ dẫn tổ chức được ưu tiên. Chỉ dẫn cá nhân vẫn áp dụng cho những gì chỉ dẫn tổ chức không đề cập. Quy tắc của Owner về câu kết email được ưu tiên hơn quy tắc riêng của cô. Quy tắc chính tả của cô vẫn áp dụng vì tổ chức không đặt gì về chính tả.

Điểm thực hành nằm ở vai trò, không phải cơ chế. Thành viên thông thường không đặt chỉ dẫn tổ chức. Vì vậy, quy tắc cần áp dụng cho toàn tổ chức là yêu cầu gửi đến người quản trị không gian làm việc. Nếu muốn mọi bản nháp của đồng nghiệp đều không ghi địa chỉ nhà khách hàng, cô yêu cầu Owner thêm quy tắc đó.

## Câu hỏi về vị trí đặt

Đặt từng quy tắc bằng cách hỏi nó đúng với phạm vi nào. Quy tắc ảnh hưởng mọi chat ở cấp của nó, nên hai phạm vi phải khớp nhau.

- **Đúng với bạn trong toàn bộ công việc:** Ngôn ngữ, tóm tắt trước hoặc mặc định viết cho người không chuyên — đặt ở cấp tài khoản.
- **Đúng với một nhóm công việc:** Người đọc, quy ước định dạng và quy tắc thường xuyên của nhóm việc đó — đặt trong chỉ dẫn Project.
- **Đúng với mọi người trong tổ chức:** Dùng chỉ dẫn tổ chức, yêu cầu thông qua Owner của không gian làm việc.
- **Chỉ đúng với việc hôm nay:** Không phải chỉ dẫn thường xuyên ở cấp nào; đó là một phần prompt hôm nay.

Quy tắc dùng chính tả Anh và tóm tắt trước đúng với toàn bộ công việc của cô, nên đặt ở cấp tài khoản. “Để phí đến tận nơi thành một dòng riêng” đúng với báo giá gửi chủ nhà cho thuê: đặt ở Project đó. Thông tin tăng giá tuần này nằm trong prompt tuần này.

Đặt sai gây thiệt hại theo cả hai hướng. Đưa quy tắc Project lên cấp tài khoản làm thay đổi mọi cuộc trò chuyện không liên quan. Quy tắc phí đến tận nơi sẽ xuất hiện trong hướng dẫn an ninh. Giữ quy tắc áp dụng mọi nơi ở cấp Project lại khiến phải sao chép và bảo trì trong từng Project cần nó. Quy tắc chính tả sẽ cần một bản trong mọi Project.

## Hành vi, không chỉ là mong muốn

Chỉ dẫn hữu ích phải kiểm tra được: người khác có thể nhận ra đã tuân thủ hay chưa. “Giữ mỗi mục dưới 90 giây khi đọc thành tiếng” có thể được thực hiện đúng hoặc sai. “Hãy hấp dẫn” không chỉ ra cách hành xử khác với cách công việc vốn sẽ diễn ra. Nó không nêu hành vi nên không có gì để kiểm tra.

Phép thử cho từng dòng: đồng nghiệp mới có thể làm theo và tạo đúng điều bạn muốn không? Nếu chưa, đó mới là mong muốn, chưa phải chỉ dẫn. “Nghe đáng tin cậy” không vượt qua phép thử với báo giá của cô. “Đặt giá và phí đến tận nơi trong hai dòng đầu” thì có. Các mong muốn chung chung cũng làm bộ chỉ dẫn chật thêm và tạo cảm giác bao quát giả tạo.

## Ngắn gọn, có ưu tiên tốt hơn dài và bao trùm mọi thứ

Chỉ dẫn thường xuyên áp dụng cho mọi chat trong phạm vi, nên chỉ chứa điều đúng mọi lần. Quy tắc chỉ đúng với một nhiệm vụ làm sai lệch các nhiệm vụ khác. Bộ chỉ dẫn gom chi tiết riêng từng nhiệm vụ dần không còn mô tả công việc mà bắt đầu mô tả nhiệm vụ mới nhất. Đưa ghi chú tăng giá vào Project báo giá, mọi báo giá sau sẽ nhắc đến cho đến khi có người xóa.

Độ dài cũng tương tự. Bộ ngắn có ưu tiên được tuân thủ đáng tin cậy hơn bộ dài cố bao trùm mọi thứ. Khi điều gì cũng là quy tắc, chúng cạnh tranh nhau; quy tắc bị bỏ qua chưa chắc là quy tắc bạn muốn bỏ. Khi bộ chỉ dẫn vượt quá lượng đồng nghiệp có thể nhớ, hãy nhóm và sắp ưu tiên. Thêm một quy tắc nữa không khắc phục được. Project báo giá có thể nhóm theo giá, câu chữ và bố cục, ưu tiên giá trước.

**Styles** là điều khiển riêng cho cách định dạng và truyền đạt câu trả lời, xem ghi chú bên dưới. Từ sự phân biệt đó, có thể hiểu Styles không phải nơi đặt quy tắc về nội dung cốt lõi.

## Trong bài thi

Mục tiêu này kiểm tra hai phán đoán: quy tắc đúng ở cấp nào và cách diễn đạt có thể kiểm tra. Điểm về vai trò tương tự Lĩnh vực 4: chuyển xử lý thay vì tự ứng biến. Ranh giới giữa chỉ dẫn thường xuyên với prompt hôm nay là ranh giới rõ nhất với Lĩnh vực 1. Mong muốn chung chung là phương án gây nhiễu đặc trưng, vì “bảo nó rõ ràng và chuyên nghiệp” luôn nghe như lời khuyên hợp lý.

### Khái niệm cốt lõi

Hai câu hỏi giải quyết gần như mọi tình huống: Quy tắc này đúng với phạm vi nào? Câu trả lời quyết định cấp đặt. Đồng nghiệp mới có thể làm theo và được kiểm tra dựa trên nó không? Câu trả lời quyết định cách diễn đạt. Đáp án đúng đáp ứng cả hai; mỗi phương án gây nhiễu trượt đúng một câu.

### Ghi chú về Styles

Trung tâm trợ giúp chỉ đề cập Styles trong một phép so sánh về định dạng, nên nhận định về quy tắc nội dung là cách hiểu của tác giả, không phải tuyên bố được tài liệu ghi nhận. **Trạng thái trong bản gốc, kiểm tra ngày 30 tháng 9 năm 2026:** Bài viết về cá nhân hóa không còn nhắc Styles; phần so sánh định dạng nêu **Skills** để tùy chỉnh cách Claude định dạng và truyền đạt câu trả lời.

## Những bẫy thường gặp trong bài thi

### Mong muốn được trình bày như chỉ dẫn: chuyên nghiệp, kỹ lưỡng, tạo chất lượng cao

Mong muốn không chỉ ra hành vi khác với mặc định và không thể bị đánh giá là thực hiện sai. Chúng không thay đổi gì nhưng làm chật chỗ của quy tắc có tác dụng. Đáp án đúng nêu hành vi kiểm tra được; phương án mong muốn chung chung là đáp án sai đặc trưng.

### Viết yêu cầu tuần này vào chỉ dẫn thường xuyên

Chỉ dẫn thường xuyên áp dụng cho mọi chat trong phạm vi. Quy tắc chỉ đúng một nhiệm vụ làm sai lệch mọi nhiệm vụ khác cho đến khi có người nhớ xóa. Nó thuộc prompt của nhiệm vụ đó — nơi đặt ranh giới với Lĩnh vực 1.

### Đặt quy tắc một Project ở cấp tài khoản hoặc tự đặt quy tắc toàn tổ chức

Quy tắc cấp tài khoản thay đổi mọi cuộc trò chuyện không liên quan. Chỉ dẫn tổ chức do Owner và Primary Owner đặt trên Team, Enterprise. Cách xử lý đúng của Associate với quy tắc toàn tổ chức là yêu cầu người quản trị, không phải thiết lập cá nhân.

## Tình huống luyện tập

Một biên tập viên tài liệu dễ đọc tại tổ chức từ thiện hỗ trợ người khuyết tật trí tuệ tự lên tiếng bảo vệ quyền lợi đang viết chỉ dẫn Project cho các bản tóm tắt dễ đọc gửi thành viên. Mọi dòng vẫn phải đúng với tài liệu tạo nhiều năm sau. Bộ chỉ dẫn nào tình nguyện viên kiểm tra đầu ra có thể sử dụng?

**Phương án A**

Dùng quy tắc độ dài câu và từ ngữ hằng ngày, thêm một dòng thường xuyên luôn đưa hạn chót khảo sát thành viên hiện tại vào vì thông tin đó quan trọng với thành viên ngay lúc này.

**Phương án B**

Luôn rõ ràng, tôn trọng, dễ tiếp cận và luôn tạo tài liệu dễ đọc chất lượng cao, thực sự hữu ích cho thành viên tổ chức.

**Phương án C**

Giữ câu dưới 15 từ và mỗi câu một ý; dùng từ ngữ hằng ngày; giải thích từ khó trong ngoặc ở lần đầu dùng; kết thúc mỗi bản tóm tắt bằng việc người đọc có thể làm tiếp theo.

**Phương án D**

Đặt quy tắc độ dài câu và từ ngữ hằng ngày trong Instructions for Claude cấp tài khoản thay vì Project, để mọi cuộc trò chuyện cô thực hiện đều theo quy tắc dễ đọc.

## Bài tập thực hành: Kiểm tra chặt chẽ và đặt đúng nơi một bộ chỉ dẫn thực tế

**Thời gian:** 30 phút.

### Bạn sẽ học được

- Cách viết lại mong muốn chung chung thành hành vi kiểm tra được.
- Cách đặt từng quy tắc ở cấp phù hợp với phạm vi áp dụng.
- Cách chuyển yêu cầu quy tắc toàn tổ chức qua người quản trị.
- Cách rút gọn bộ chỉ dẫn đến mức đồng nghiệp có thể nhớ.

### Bước 1 — Lấy bộ chỉ dẫn Project bạn đang dùng

Hoặc soạn bộ chỉ dẫn cho Project đã tạo trong bài tập 5.1.

**Vì sao:** Bài tập cần bộ thật với thiếu sót thật. Ví dụ dựng lên dễ làm kết quả kiểm tra trông tốt hơn thực tế.

**Kết quả cần thấy:** Toàn bộ bộ chỉ dẫn trước mặt, mỗi quy tắc một dòng.

### Bước 2 — Áp dụng phép thử đồng nghiệp mới cho từng dòng

Họ có thể làm theo và tạo điều bạn muốn không? Viết lại mong muốn thành hành vi bạn thực sự kiểm tra; xóa dòng chỉ nhắc lại mặc định.

**Vì sao:** Khả năng kiểm tra phân biệt chỉ dẫn với mong muốn. Nhắc lại mặc định chỉ tăng độ dài mà không thay đổi gì.

**Kết quả cần thấy:** Mọi dòng còn lại đều nêu việc có thể thấy rõ là được thực hiện hoặc thực hiện sai.

### Bước 3 — Gắn phạm vi và chuyển từng dòng về đúng cấp

Đánh dấu: đúng mọi lần với công việc này, đúng với bạn ở mọi nơi hoặc chỉ đúng với nhiệm vụ gần đây. Chuyển quy tắc mọi nơi vào Instructions for Claude cấp tài khoản; chuyển dòng riêng từng việc về prompt nhiệm vụ.

**Vì sao:** Đặt đúng nơi là một nửa mục tiêu. Quy tắc thuộc cấp phù hợp với phạm vi; đặt sai gây thiệt hại theo cả hai hướng.

**Kết quả cần thấy:** Mỗi dòng có nhãn cấp; ít nhất một dòng được chuyển ra khỏi bộ Project.

### Bước 4 — Viết yêu cầu cho quy tắc toàn tổ chức nếu có

Viết một câu bạn sẽ gửi người quản trị không gian làm việc thay vì tự tìm cách đặt.

**Vì sao:** Chỉ dẫn tổ chức do Owner và Primary Owner thiết lập. Đóng góp chuyên nghiệp là yêu cầu được diễn đạt rõ.

**Kết quả cần thấy:** Một câu nêu quy tắc và lý do nên áp dụng cho mọi cuộc trò chuyện trong tổ chức.

### Bước 5 — Nhóm và sắp ưu tiên nếu bộ còn quá dài

Nếu vượt lượng đồng nghiệp có thể nhớ, chia thành ba hoặc bốn nhóm và đặt quy tắc quan trọng nhất trước.

**Vì sao:** Khi điều gì cũng là quy tắc, chúng cạnh tranh nhau. Nhóm và ưu tiên giúp chủ động quyết định quy tắc nào được ưu tiên thay vì để ngẫu nhiên.

**Kết quả cần thấy:** Bộ ngắn, có nhóm, có thứ tự; những quy tắc bạn coi trọng nhất ở đầu.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Hiểu các tính năng cá nhân hóa của Claude — *Understanding Claude's personalization features*.
- Đặt chỉ dẫn tổ chức — *Set organization instructions*.
- Project là gì? — *What are projects?*
- Tôi có thể tạo và quản lý Project như thế nào? — *How can I create and manage projects?*
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [5.2 — Quản lý kiến thức tải lên và trình kết nối](5-2-uploads-and-connectors.vi.md).
- **Bài tiếp theo:** [5.4 — Thông báo, duy trì và cập nhật cấu hình](5-4-maintaining-configurations.vi.md).
