# 3.3 — Lựa chọn mô hình phù hợp với chi phí, tốc độ và chất lượng

- **Lĩnh vực (Domain):** 3
- **Nhiệm vụ (Task):** 3.3
- **Tên bài gốc:** Aligning Model Choice with Cost, Speed and Quality
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/3-product-model-selection/3-3-cost-speed-quality)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Mục tiêu 3.2 đã giải thích các cấp mô hình. Mỗi lần chọn giữa chúng, bạn chi ba loại “đồng tiền”: chi phí, thời gian và chiều sâu. **Chi phí** là hạn mức sử dụng của gói, không phải hóa đơn tính theo từng lần dùng. **Tốc độ** là thời gian chờ mỗi câu trả lời, đặc biệt đáng kể khi chạy nhiều lần. **Chất lượng** là chiều sâu trong công việc đòi hỏi cao, như mục tiêu 3.2 đã định nghĩa: xử lý sự mơ hồ, dung hòa mâu thuẫn và đưa ra phán đoán một cách an toàn. Kỹ năng cần có là xác định nhiệm vụ cần nguồn lực nào rồi chỉ chi đúng mức cần thiết.

Chủ một cửa hàng cá chiên và khoai tây chiên dùng Claude cho hai việc. Một việc là tạo 500 phản hồi đánh giá khách hàng, chỉ khác nhau ở tên và món ăn. Việc còn lại là soạn một thư trả lời chính quyền địa phương sau đợt kiểm tra vệ sinh.

## Ba câu hỏi để xác định nguồn lực cần ưu tiên

Hãy hỏi ba câu theo thứ tự: Sai ở đây gây hậu quả gì? Công việc sẽ chạy bao nhiêu lần? Ai đang chờ câu trả lời? Các câu trả lời xác định nguồn lực cần ưu tiên. Thiếu chúng, lựa chọn chỉ dựa trên cảm giác thay vì quyết định có yêu cầu được nêu rõ. Với phản hồi đánh giá của cửa hàng: lỗi ít tốn kém, chạy 500 lần, không ai đang chờ. Với thư trả lời về vệ sinh: lỗi gây hậu quả lớn, chạy một lần, chính quyền địa phương đang chờ.

## Chi phí nghĩa là hạn mức sử dụng

Trung tâm trợ giúp liệt kê lựa chọn mô hình, mức nỗ lực, độ dài cuộc trò chuyện hiện tại và kích thước tệp đính kèm trong số những yếu tố quyết định hạn mức bị tiêu thụ nhanh đến đâu. Hạn mức có giới hạn, nên mỗi nhiệm vụ bị chi quá mức đều lấy đi nguồn lực của những nhiệm vụ phía sau. Tạo phản hồi đánh giá trên mô hình nặng nhất sẽ tiêu thụ hạn mức mà thư trả lời về vệ sinh cần dùng.

## Khối lượng nhân tác động của chi phí và tốc độ

Chạy một lần, chênh lệch giữa các cấp chỉ là vài giây và một phần nhỏ hạn mức. Chạy 500 lần, cùng chênh lệch đó quyết định công việc có hoàn thành trong hôm nay hay không và hạn mức có đủ dùng cả tuần hay không. Công việc thường lệ với khối lượng lớn, như phản hồi đánh giá, phù hợp với cấp nhẹ hơn.

Công việc khối lượng lớn trên cấp nhanh cần được kiểm tra chọn mẫu, vì trách nhiệm xác minh của Lĩnh vực 2 không bao giờ được bỏ qua. Cách làm này mở rộng hợp lý: chủ cửa hàng đọc kiểm tra một mẫu các phản hồi. Sự kết hợp ấy khiến lựa chọn trở nên chuyên nghiệp thay vì chỉ rẻ.

## Mức độ hệ trọng làm tăng yêu cầu chất lượng

Mức độ hệ trọng tác động theo một trục khác. Một số đầu ra riêng lẻ làm căn cứ cho quyết định có ảnh hưởng lớn và cần chiều sâu: hồ sơ gửi cơ quan quản lý, thư nhạy cảm về pháp lý hoặc khuyến nghị mà hội đồng quản trị sẽ dựa vào để hành động. Vài giây tiết kiệm được bằng cấp nhẹ hơn không đáng gì so với hậu quả của một kết luận sai tinh tế. “Chỉ có một lá thư” là nhận xét đúng nhưng không liên quan, vì một lá thư kéo theo hệ quả đòi hỏi cao hơn 500 lá thư không có hệ quả tương tự. Yêu cầu chất lượng phụ thuộc hậu quả nếu sai, không phụ thuộc mức độ danh giá của nhiệm vụ. Sau đó, đầu ra có ảnh hưởng hệ trọng vẫn phải được người đủ năng lực chuyên môn rà soát, bất kể mô hình nào đã soạn. Thư trả lời về vệ sinh cần cấp mạnh hơn và người kiểm tra đủ năng lực.

## Tách khối lượng công việc hỗn hợp

Công việc thực tế pha trộn nhiều dạng. Hãy tách theo mức độ đòi hỏi thay vì chạy tất cả với một thiết lập. Phần thường lệ số lượng lớn dùng cấp nhanh và kiểm tra chọn mẫu. Phần cốt lõi khó dùng cấp mạnh hơn và được rà soát thích hợp. Bộ chọn mô hình khiến việc tách này dễ thực hiện: có thể đổi mô hình bất kỳ lúc nào trong cuộc trò chuyện, có hiệu lực từ câu trả lời tiếp theo.

Có ba đáp án sai thường lặp lại. **Tối đa chất lượng ở mọi chỗ** phải trả chi phí cho chiều sâu ở công việc không cần đến, và sự lãng phí cộng dồn theo khối lượng. **Tối thiểu chi phí ở mọi chỗ** đưa đầu ra hời hợt vào những công việc mà lỗi gây thiệt hại lớn. **Vòng lặp nâng cấp mô hình** chạy lại đầu ra chưa đạt trên các mô hình ngày càng nặng. Nó xem bản giao việc mơ hồ là vấn đề của mô hình, trong khi bản giao việc mơ hồ thất bại ở mọi cấp. Sửa bản giao việc là cách xử lý của Lĩnh vực 1, không nâng cấp mô hình nào thay thế được. Nếu bản giao việc cho thư vệ sinh chưa từng nêu người đọc, mọi cấp đều bỏ lỡ yêu cầu đó.

## Trong bài thi

Phần dẫn yêu cầu bạn định giá nhiệm vụ thực tế bằng ba loại nguồn lực này. Câu hỏi mẫu của hướng dẫn chọn mô hình nhanh hơn, chi phí thấp hơn cho công việc soạn thảo đơn giản, khối lượng lớn. Bẫy thường gặp là để yếu tố khối lượng chi phối nhầm quyết định vốn phải dựa trên mức độ hệ trọng.

### Khái niệm cốt lõi

Khối lượng nhân tác động của chi phí và tốc độ; mức độ hệ trọng làm tăng yêu cầu chất lượng. Khi phần dẫn trộn cả hai dạng, đáp án đúng gần như luôn tách công việc. Phần số lượng lớn dùng cấp nhanh cùng kiểm tra chọn mẫu. Phần kéo theo hệ quả dùng cấp mạnh hơn cùng quy trình rà soát thích hợp.

## Những bẫy thường gặp trong bài thi

### Chọn cấp nhanh cho đầu ra hệ trọng vì chỉ có một lá thư

Mức độ hệ trọng quyết định yêu cầu chất lượng, không phải khối lượng. Một đầu ra làm căn cứ cho quyết định có ảnh hưởng lớn đòi hỏi cao hơn hàng trăm đầu ra thường lệ; vài giây tiết kiệm bằng cấp nhẹ hơn không đáng gì so với hậu quả của kết luận sai tinh tế.

### Chọn cấp cao nhất cho phần thường lệ số lượng lớn vì công việc quan trọng

Tầm quan trọng không tự chuyển từ dự án sang mọi nhiệm vụ bên trong. Biến đổi thường lệ với khối lượng lớn cần tốc độ, chi phí thấp và kiểm tra chọn mẫu. Trả chi phí cho chiều sâu hàng trăm lần không mang lại điều nhiệm vụ cần.

### Chuyển sang mô hình nặng hơn khi lỗi thực sự nằm ở bản giao việc mơ hồ

Bản giao việc mơ hồ thất bại ở mọi cấp, nên vòng lặp nâng cấp chỉ tốn thêm thời gian và hạn mức để nhận ra lại điều đó. Khi phần dẫn cho thấy prompt thiếu người đọc, ràng buộc hoặc tài liệu nguồn, cách xử lý đúng là sửa bản giao việc — thuộc Lĩnh vực 1 — thay vì nâng cấp mô hình.

## Tình huống luyện tập

Một hiệp hội điền kinh cấp vùng đang chuẩn bị đêm trao giải hằng năm: 500 thư mời cá nhân hóa chỉ khác tên, câu lạc bộ và nội dung thi đấu; cùng một lá thư khó gửi cho câu lạc bộ bị đình chỉ do thiếu sót trong việc bảo vệ người tham gia (safeguarding), đòi hỏi giọng văn, độ chính xác và sự thận trọng về những khía cạnh liên quan pháp lý. Chi phí thư mời phải thấp nhất có thể, còn mọi biện pháp giúp thư đình chỉ an toàn hơn đều không được cắt giảm. Nhân viên hành chính nên thực hiện hai việc thế nào?

**Phương án A**

Chạy cả hai trên mô hình có năng lực cao nhất, vì đêm trao giải là sự kiện chủ lực của hiệp hội và không phần nào được trông như sản phẩm chất lượng thấp.

**Phương án B**

Chạy cả hai trên mô hình nhanh hơn, vì thư mời rõ ràng là việc số lượng lớn, còn thư đình chỉ chỉ có một lá thư, hoàn toàn nằm trong khả năng của bất kỳ mô hình nào.

**Phương án C**

Soạn thư đình chỉ bằng mô hình nhanh hơn để giữ hạn mức; nếu giọng văn chưa đạt, chạy lại đúng prompt đó trên mô hình mạnh nhất, lặp lại cho đến khi cuối cùng có phiên bản chấp nhận được.

**Phương án D**

Chạy 500 thư mời trên mô hình nhanh hơn, chi phí thấp hơn và kiểm tra chọn mẫu; sau đó soạn thư đình chỉ trên mô hình mạnh nhất, có người đủ năng lực chuyên môn rà soát trước khi gửi.

## Bài tập thực hành: Đánh giá công việc hỗn hợp theo ba loại nguồn lực

**Thời gian:** 25 phút.

### Bạn sẽ học được

- Cách xác định nhiệm vụ cần ưu tiên chi phí, thời gian hay chiều sâu.
- Cách xử lý công việc số lượng lớn trên cấp nhẹ hơn cùng kiểm tra chọn mẫu.
- Cách bố trí chiều sâu xử lý và người đủ năng lực rà soát cho đầu ra hệ trọng.
- Cách phát hiện quyết định theo mức độ danh giá hoặc thói quen dùng một thiết lập cho tất cả trong tuần của mình.

### Bước 1 — Chọn một tuần thực tế có cả hai dạng công việc

Tuần đó cần có nhiệm vụ số lượng lớn với nhiều đầu ra tương tự nhau và một nhiệm vụ riêng lẻ có ảnh hưởng hệ trọng.

**Vì sao:** Công việc hỗn hợp là dạng mà mục tiêu này kiểm tra. Tuần chỉ có một dạng sẽ che khuất quyết định tách công việc.

**Kết quả cần thấy:** Hai nhiệm vụ được nêu tên: một việc số lượng lớn và một việc kéo theo hệ quả.

### Bước 2 — Nêu nguồn lực cần ưu tiên cho mỗi nhiệm vụ

Viết một dòng xác định chi phí, thời gian hoặc chiều sâu là yếu tố cần nhất và giải thích vì sao.

**Vì sao:** Xác định nguồn lực cần ưu tiên là toàn bộ kỷ luật này. Mọi đáp án sai trong mục tiêu đều bỏ qua bước đó.

**Kết quả cần thấy:** Hai lời giải thích, mỗi lời một dòng, nêu một nguồn lực chủ đạo.

### Bước 3 — Chọn cấp cho từng nhiệm vụ và chạy phần số lượng lớn

Thực hiện phần số lượng lớn trên cấp nhẹ hơn, kiểm tra một mẫu theo tiêu chuẩn chất lượng của bạn.

**Vì sao:** Kiểm tra chọn mẫu phân biệt kiểm soát chi phí chuyên nghiệp với việc đưa ra đầu ra chưa được rà soát.

**Kết quả cần thấy:** Đầu ra số lượng lớn vượt qua kiểm tra mẫu và được tạo nhanh hơn rõ rệt.

### Bước 4 — Xác định người rà soát nhiệm vụ hệ trọng

Ghi rõ ai sẽ thực hiện rà soát chuyên môn sau khi cấp mạnh hơn soạn bản nháp.

**Vì sao:** Chiều sâu của bản nháp không hoàn thành thay nghĩa vụ rà soát. Đầu ra kéo theo hệ quả phải được người đủ năng lực kiểm tra, bất kể mô hình nào tạo ra.

**Kết quả cần thấy:** Một người rà soát được nêu tên, có đủ năng lực để phát hiện kết luận sai tinh tế.

### Bước 5 — Rà lại các quyết định trong tuần

Đánh dấu quyết định theo mức độ danh giá hoặc thói quen áp một thiết lập cho tất cả, thay vì dựa trên yêu cầu nhiệm vụ, rồi ghi cách phân công đã sửa.

**Vì sao:** Hai thiết lập đồng loạt — tối đa chất lượng ở mọi chỗ và tối thiểu chi phí ở mọi chỗ — là phương án gây nhiễu thường gặp. Rà lại tuần của mình giúp nhận ra chúng trong phần dẫn câu hỏi.

**Kết quả cần thấy:** Mỗi nhiệm vụ được gắn nhãn theo yêu cầu, theo mức độ danh giá hoặc theo thói quen; hai nhóm sau có cách phân công được sửa lại.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Tổng quan các mô hình — *Models overview*.
- Các phương pháp sử dụng hạn mức hiệu quả — *Usage limit best practices*.
- Thay đổi mô hình, mức nỗ lực và thiết lập suy nghĩ — *Change the model, effort, and thinking settings*.
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [3.2 — Phân biệt các loại mô hình Claude](3-2-model-tiers.vi.md).
- **Bài tiếp theo:** [3.4 — Quản lý giới hạn ngữ cảnh và bộ nhớ: Bắt đầu lại, tóm tắt, lưu giữ](3-4-context-and-memory-management.vi.md).
