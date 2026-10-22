# 1.3 — Tinh chỉnh prompt qua nhiều vòng để cải thiện đầu ra

- **Lĩnh vực (Domain):** 1
- **Nhiệm vụ (Task):** 1.3
- **Tên bài gốc:** Iterating Prompts to Improve Output
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/1-prompting-task-execution/1-3-prompt-iteration)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Đầu ra đầu tiên — câu trả lời đầu tiên của Claude cho một prompt — là một bản nháp. Prompt xác định nhiệm vụ chính là bản giao việc. **Phản hồi (feedback)** là chỉ dẫn tiếp theo bạn gửi về đầu ra đó. **Tinh chỉnh qua nhiều vòng (iteration)** là chu trình: đầu ra, phản hồi cụ thể, đầu ra tốt hơn. Đây là nhịp làm việc bình thường, không phải dấu hiệu thất bại. Hướng dẫn bắt đầu sử dụng trong Trung tâm trợ giúp nói rõ: đừng ngại tinh chỉnh prompt hoặc đặt câu hỏi tiếp nối. Những người tận dụng Claude hiệu quả nhất dự trù một hoặc hai vòng phản hồi cho mỗi nhiệm vụ. Những người tận dụng kém nhất thường chấp nhận ngay bản đầu tiên tầm thường hoặc bỏ công cụ sau một lần thử.

Tại một phòng khám nha khoa, người quản lý nhờ Claude viết thư nhắc bệnh nhân đã đến lịch khám định kỳ. Bản nháp có đủ các phần cần thiết nhưng giọng văn cứng nhắc, quá dài và đầy thuật ngữ lâm sàng.

## Phản hồi chỉ rõ điểm chưa đạt

Trung tâm trợ giúp liệt kê phản hồi là một cách chính thức để khắc phục câu trả lời không hữu ích: cung cấp chỉ dẫn tiếp nối, làm rõ yêu cầu hoặc yêu cầu viết lại. “Làm hay hơn rồi thử lại” chỉ tái tạo vấn đề, vì cuộc trò chuyện không nhận thêm thông tin mới. Giả sử người quản lý viết: “Rút xuống 200 từ, giữ đoạn nói về chi phí và bỏ các tính từ mang tính quảng cáo.” Cách này khắc phục được vấn đề vì từng vế đều chỉ rõ một điểm chưa đạt.

Phản hồi tốt thực hiện một trong ba việc:

- Bổ sung một ràng buộc còn thiếu, chẳng hạn người đọc, định dạng hoặc điều cần tránh.
- Sửa một cách hiểu sai.
- Thu hẹp phạm vi.

Cả ba đều dựa trên việc chẩn đoán vấn đề. Hãy xác định khoảng cách giữa đầu ra và nhu cầu, rồi diễn đạt thẳng, rõ ràng. Một cách kiểm tra nhanh hữu ích là đối chiếu đầu ra với năm thành phần của bản giao việc ban đầu. Điểm chưa đạt thường nằm ở chỗ một thành phần còn sơ sài hoặc bị thiếu. Prompt một dòng của người quản lý chưa từng nêu đối tượng đọc.

Yêu cầu các phiên bản khác nhau cũng là một hình thức tinh chỉnh. Người quản lý có thể yêu cầu ba phiên bản của đoạn mở đầu: trang trọng, gần gũi như trò chuyện và mang tính khẩn trương. Claude trở thành công cụ tạo phương án, còn người quản lý là người đánh giá. Đây thường là cách nhanh nhất để tìm được sắc thái diễn đạt phù hợp khi bạn biết có gì đó chưa ổn nhưng chưa gọi tên được vấn đề.

## Tinh chỉnh hay giao việc lại?

Khi đầu ra đã gần đạt, hãy tinh chỉnh. Tiếp tục trong cuộc trò chuyện hiện tại và đưa ra chỉ dẫn bổ sung có trọng tâm. Đôi khi, đầu ra cho thấy prompt ban đầu đã sai: giao sai nhiệm vụ, đặt vấn đề sai hướng hoặc thiếu bối cảnh. Khi đó, hãy viết lại bản giao việc và bắt đầu cuộc trò chuyện mới, thay vì vá một sự hiểu nhầm qua sáu lượt trao đổi tiếp nối. Một chuỗi sửa đổi dài làm bối cảnh được chuyển tiếp trong cuộc trò chuyện trở nên rối. Mỗi bản vá cũng chống lại cách đặt vấn đề ban đầu thay vì sửa tận gốc.

Việc phán đoán sai xảy ra theo cả hai hướng. Một là liên tục vá một bản giao việc vốn đã yêu cầu sai điều cần làm. Hai là bỏ một cuộc trò chuyện chỉ còn cần một chỉnh sửa cụ thể là hoàn tất. Nếu lá thư của người quản lý chỉ cần từ ngữ dễ hiểu hơn, một lượt chỉ dẫn tiếp nối là đủ.

## Ba cách phản ứng với một bản nháp chưa đạt

Với bản nháp có cấu trúc ổn nhưng chưa đúng mục tiêu, có ba cách phản ứng. Yêu cầu thử lại mơ hồ như “Chưa đúng lắm, thử lại đi” sẽ tạo ra cùng thiếu sót, vì không có thông tin mới được đưa vào cuộc trò chuyện. Chỉ dẫn tiếp nối có trọng tâm nêu rõ giọng văn, các cụm từ cần tránh và người đọc mà văn bản hướng đến. Nó tạo ra bản sửa đổi dùng được, vì mỗi điểm chưa đạt được nêu tên đều cho lần viết lại một mục tiêu cụ thể. Người quản lý nêu rõ: giọng văn ấm áp, không dùng thuật ngữ lâm sàng và người đọc là bệnh nhân.

Cách thứ ba là giao việc lại, dành cho trường hợp vấn đề thực sự nằm ở prompt một dòng ban đầu. Một prompt hiệu quả chứa càng nhiều bối cảnh càng tốt, trong khi một dòng cung cấp rất ít. Hãy giao việc lại đầy đủ, đính kèm hướng dẫn văn phong và nêu đối tượng đọc ngay từ đầu. Điều này vừa sửa được loạt nội dung hiện tại, vừa cải thiện mọi loạt nội dung về sau.

## Giữ lại cách diễn đạt đã có hiệu quả

Khi hai vòng phản hồi cuối cùng giúp đầu ra đạt yêu cầu, chính những phản hồi đã sửa được bản nháp là các chỉ dẫn mà prompt ban đầu còn thiếu. Hãy đưa chúng trở lại prompt, để lần dùng sau của prompt có thể tái sử dụng bắt đầu từ nền tảng đã được cải thiện. Loạt thư tiếp theo của người quản lý sẽ bắt đầu bằng prompt nêu rõ giọng văn, từ ngữ dễ hiểu và đối tượng đọc là bệnh nhân.

## Trong bài thi

Bài thi kiểm tra chất lượng phản hồi và thứ tự ưu tiên giữa ba cách phản ứng. Chỉ dẫn tiếp nối có trọng tâm luôn được đánh giá cao hơn yêu cầu thử lại mơ hồ. Bạn cần nhận ra khi nào giao việc lại là lựa chọn làm việc chuyên nghiệp. Câu hỏi khai thác cả hai hướng phán đoán sai. Khi công việc lặp lại mỗi tuần, việc đưa cách diễn đạt của prompt thành cấu hình dùng thường xuyên, chẳng hạn phần chỉ dẫn của một Project, thuộc Lĩnh vực 5. Lĩnh vực 1 dừng ở việc tinh chỉnh yêu cầu đang xử lý và giữ lại các chỉ dẫn đã chứng minh được giá trị.

### Vì sao nên bắt đầu lại trong một cuộc trò chuyện mới?

Cuộc trò chuyện dài hơn tiêu thụ nhiều hạn mức sử dụng hơn. Khi cuộc trò chuyện gần chạm giới hạn độ dài, lời khuyên được tài liệu ghi nhận là mở cuộc trò chuyện mới hoặc dùng Project. Nếu bản giao việc ban đầu sai, bắt đầu lại được khuyến nghị như một cách làm việc chuyên nghiệp, vì chuỗi sửa đổi dài tạo ra điểm xuất phát lộn xộn. Tài liệu chính thức không khẳng định rằng cuộc trò chuyện dài làm giảm chất lượng đầu ra.

## Những bẫy thường gặp trong bài thi

### Yêu cầu thử lại mơ hồ được ngụy trang thành sự chăm chỉ

Tạo lại câu trả lời, đổi nhẹ câu chữ hoặc yêu cầu Claude thử lại đều không bổ sung thông tin mới vào cuộc trò chuyện, nên đầu ra tiếp theo lặp lại thiếu sót cũ. Phản hồi chỉ có tác dụng khi chỉ rõ điểm chưa đạt: đối tượng đọc, giọng văn, độ dài hoặc ràng buộc còn thiếu.

### Vá một bản giao việc sai từ gốc qua nhiều lượt trao đổi

Khi đầu ra cho thấy prompt ban đầu đã yêu cầu sai điều cần làm, mỗi bản vá đều chống lại cách đặt vấn đề thay vì sửa nó. Viết lại bản giao việc và bắt đầu cuộc trò chuyện mới nhanh hơn, đồng thời tạo điểm khởi đầu tốt hơn cho mọi loạt công việc cùng loại về sau.

### Mở cuộc trò chuyện mới khi đầu ra chỉ còn cần một chỉnh sửa cụ thể

Đây là kiểu phán đoán sai theo hướng ngược lại. Bắt đầu lại làm mất bối cảnh và nội dung đã được duyệt mà cuộc trò chuyện hiện tại đang có. Khi đầu ra đã gần đạt, một chỉ dẫn tiếp nối có trọng tâm trong cùng cuộc trò chuyện là lựa chọn ít tốn kém hơn, nhanh hơn và chuyên nghiệp hơn.

## Tình huống luyện tập

Một nhân viên phụ trách hàng hóa bán lẻ nhờ Claude viết mô tả sản phẩm cho danh mục đồ gia dụng theo mùa. Loạt đầu tiên có cấu trúc ổn nhưng chung chung và không đúng giọng văn thương hiệu. Khi dùng lại cùng prompt trong một cuộc trò chuyện mới, kết quả vẫn chung chung như vậy. Cô muốn sửa xong nội dung trong một vòng nữa. Prompt tiếp theo nào hiệu quả nhất?

**Phương án A**

Phản hồi rằng nội dung chưa đúng lắm, yêu cầu Claude thử lại và tiếp tục tạo lại trong cùng cuộc trò chuyện cho đến khi cuối cùng có một loạt nội dung đúng giọng văn.

**Phương án B**

Bắt đầu một cuộc trò chuyện hoàn toàn mới, dán lại đúng prompt một dòng đó và trông chờ cuộc trò chuyện mới tạo ra giọng văn tươi mới, khác biệt hơn cho loạt nội dung.

**Phương án C**

Phản hồi cụ thể, nêu giọng văn cần có, các cụm từ bị lạm dụng cần tránh và nhóm người mua mà danh mục đang hướng đến, rồi chạy lại loạt nội dung.

**Phương án D**

Chấp nhận nội dung là một điểm khởi đầu tạm ổn, rồi tự viết lại giọng văn cho cả 40 mô tả trước khi danh mục được in.

## Bài tập thực hành: Thực hiện hai vòng phản hồi

**Thời gian:** 20 phút.

### Bạn sẽ học được

- Cách chẩn đoán khoảng cách giữa đầu ra và nhu cầu.
- Cách viết phản hồi chỉ rõ điểm chưa đạt.
- Cách yêu cầu các phiên bản theo những sắc thái diễn đạt được nêu tên để chọn hướng đi.
- Cách đưa phản hồi có hiệu quả trở lại prompt có thể tái sử dụng.

### Bước 1 — Chọn một đầu ra chưa làm bạn hài lòng

Dùng đầu ra gần đây của Claude từng khiến bạn thất vọng, hoặc chạy bản giao việc gồm năm thành phần từ mục tiêu 1.1 và dùng bản nháp đầu tiên.

**Vì sao:** Thực hành phản hồi cần một điểm chưa đạt thực tế để chẩn đoán. Ví dụ dựng lên dễ khiến bài tập có vẻ thành công hơn thực tế.

**Kết quả cần thấy:** Bản nháp đầu tiên trước mặt bạn cùng prompt đã tạo ra nó.

### Bước 2 — Chẩn đoán điểm chưa đạt

Nêu cụ thể điều gì khác với nhu cầu của bạn, chẳng hạn đối tượng đọc, giọng văn, độ dài, phạm vi hoặc một ràng buộc còn thiếu.

**Vì sao:** Chẩn đoán là kỹ năng được kiểm tra. Phản hồi chỉ có thể chỉ ra một điểm chưa đạt sau khi bạn xác định được điểm đó.

**Kết quả cần thấy:** Một hoặc hai câu viết ra các điểm chưa đạt cụ thể, thay vì cảm giác chung rằng có gì đó không đúng.

### Bước 3 — Viết phản hồi rõ ràng và thực hiện lần sửa đầu tiên

Nêu rõ từng điểm chưa đạt rồi yêu cầu sửa.

**Vì sao:** Phản hồi cụ thể tạo mục tiêu cho việc sửa đổi. Phản hồi mơ hồ chỉ tái tạo vấn đề.

**Kết quả cần thấy:** Bản sửa đổi tiến gần yêu cầu hơn theo cách có thể đánh giá được ở những điểm bạn đã nêu.

### Bước 4 — Chẩn đoán lại và thực hiện vòng thứ hai

Nếu đang lựa chọn giữa các hướng đi, hãy yêu cầu các phiên bản theo những sắc thái diễn đạt được nêu tên.

**Vì sao:** Vòng thứ hai giúp hình thành nhịp làm việc: đầu ra, phản hồi cụ thể, đầu ra tốt hơn. Các phiên bản lựa chọn giúp bạn đóng vai trò người đánh giá thay vì người trực tiếp biên tập.

**Kết quả cần thấy:** Bản sửa đổi thứ hai hoặc một bộ phiên bản có gắn nhãn, đã đủ gần yêu cầu để bạn hoàn thiện bằng tay.

### Bước 5 — Đưa phản hồi có giá trị trở lại prompt

Ghi lại từng phản hồi đã đưa ra, đánh dấu phần lẽ ra nên có trong prompt ban đầu và đưa chúng vào phiên bản prompt có thể tái sử dụng.

**Vì sao:** Phản hồi sửa được bản nháp chính là chỉ dẫn prompt ban đầu còn thiếu. Đưa nó trở lại prompt biến một lần sửa lỗi thành tài sản dùng về sau.

**Kết quả cần thấy:** Một prompt đã chỉnh sửa, có tích hợp các phản hồi, được lưu tại nơi bạn giữ ghi chép làm việc.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Bắt đầu sử dụng Claude — *Get started with Claude*.
- Prompt của tôi không tạo ra câu trả lời hữu ích — *My prompt isn't giving me a helpful answer*.
- Hạn mức sử dụng và giới hạn độ dài hoạt động như thế nào? — *How do usage and length limits work?*

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [1.2 — Chia nhỏ yêu cầu phức tạp](1-2-task-decomposition.vi.md).
- **Bài tiếp theo:** [1.4 — Điều chỉnh chiến lược theo loại nhiệm vụ](1-4-task-type-strategies.vi.md).
