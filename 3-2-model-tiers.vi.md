# 3.2 — Phân biệt các loại mô hình Claude

- **Lĩnh vực (Domain):** 3
- **Nhiệm vụ (Task):** 3.2
- **Tên bài gốc:** Differentiating Between Claude Model Types
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/3-product-model-selection/3-2-model-tiers)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Mục tiêu này nêu ba họ mô hình: **Haiku, Sonnet và Opus**. Mỗi họ là một cấp mô hình (tier), và giữa các cấp có sự đánh đổi thực tế giữa tốc độ, chi phí và chiều sâu xử lý. Nhóm Haiku là cấp có chi phí thấp nhất. Anthropic xếp nhóm này là nhanh nhất và mô tả nó được xây dựng cho nhiệm vụ có khối lượng lớn, nhạy với độ trễ. Nhóm Opus là cấp có năng lực suy luận cao nhất, dành cho công việc phức tạp, có ảnh hưởng hệ trọng. Nhóm Sonnet cung cấp sự kết hợp tốt nhất giữa tốc độ và trí thông minh: cấp giữa cân bằng, phù hợp làm lựa chọn mặc định hằng ngày. Không có cấp nào là “cấp tốt duy nhất”. Mỗi cấp đều là lựa chọn đúng cho công việc phù hợp với thế mạnh của nó.

Một người bán hoa có hai việc: chuẩn hóa 300 mục sản phẩm theo cùng mẫu trên website và đối chiếu hai báo cáo có một phần mâu thuẫn của hai nhà bán buôn để đưa ra một khuyến nghị đặt hàng thống nhất.

## Sự đánh đổi

Phía có năng lực cao hơn cần nhiều thời gian hơn cho mỗi câu trả lời. Lựa chọn mô hình cũng là một trong những yếu tố quyết định hạn mức sử dụng bị tiêu thụ nhanh đến đâu. Phía nhanh hơn đổi lấy tốc độ bằng việc không phù hợp với những nhiệm vụ đòi hỏi cao nhất. Dùng Opus cho từng mục sản phẩm của cửa hàng hoa sẽ mất nhiều thời gian hơn mà không mang lại lợi ích tương ứng.

## Năng lực có nghĩa là gì?

Năng lực ở đây là chiều sâu xử lý công việc đòi hỏi cao: tháo gỡ sự mơ hồ và mâu thuẫn, suy luận nhiều bước, tổng hợp các nguồn không hoàn toàn thống nhất và soạn nội dung mà một sai lệch tinh tế về cách diễn đạt có thể gây hậu quả thực tế. Điều đó không có nghĩa là tốt hơn trong mọi việc, nên cấp cao nhất không phải lựa chọn cho tất cả nhiệm vụ. Với công việc thường lệ, được đặc tả rõ, các cấp nhẹ hơn tạo ra đúng những gì nhiệm vụ cần và nhanh hơn. Các mục sản phẩm của cửa hàng hoa là việc thường lệ; khuyến nghị đặt hàng từ báo cáo của các nhà bán buôn thì không.

Không được khẳng định cấp nhẹ hơn có chất lượng ngang cấp mạnh hơn ở công việc đòi hỏi cao; tài liệu không đưa ra khẳng định đó. Cấp nhẹ hơn có chỗ đứng nhờ phù hợp nhiệm vụ cùng quy trình kiểm tra, không nhờ sự tương đương về năng lực.

## Đọc các dấu hiệu trong nhiệm vụ

Dấu hiệu phù hợp cấp nhẹ hơn gồm: khối lượng lớn, công việc thường lệ và lặp lại, biến đổi đơn giản như định dạng lại, trích xuất hoặc chuẩn hóa, tốc độ quan trọng và từng đầu ra riêng lẻ ít hệ trọng. Những đầu ra này vẫn được kiểm tra chọn mẫu, vì kỷ luật rà soát của Lĩnh vực 2 không bao giờ được bỏ qua. Dấu hiệu cần cấp có năng lực cao nhất gồm: sự mơ hồ, mâu thuẫn cần tháo gỡ, phán đoán kéo theo hệ quả, tổng hợp phức tạp và công việc mà một kết luận sai tinh tế gây thiệt hại lớn hơn thời gian bỏ thêm. Khi không nhóm dấu hiệu nào chiếm ưu thế, cấp giữa cân bằng là lựa chọn hằng ngày.

Quy mô không quyết định; bản chất công việc mới quyết định. Chuẩn hóa một danh sách dài theo cùng mẫu vẫn là việc của cấp nhẹ hơn, bất kể có bao nhiêu dòng. Đối chiếu hai báo cáo không hoàn toàn thống nhất để tạo một khuyến nghị duy nhất là việc của cấp mạnh hơn, dù trang kết quả cuối cùng ngắn đến đâu. Các mục sản phẩm của cửa hàng hoa được giao cho cấp nhẹ hơn và kiểm tra chọn mẫu; khuyến nghị dài một trang được giao cho Opus.

## Bộ chọn mô hình

Bạn chọn mô hình trong giao diện trò chuyện, không phải trong cấu hình kỹ thuật. Nhấp tên mô hình rồi chọn một mô hình khác đang có sẵn. Bạn có thể thay đổi ở bất kỳ thời điểm nào trong cuộc trò chuyện, và thay đổi có hiệu lực từ câu trả lời tiếp theo của Claude. Bộ chọn hiển thị những mô hình tài khoản của bạn được phép dùng; danh sách thay đổi theo gói và, trong môi trường làm việc, theo những gì tổ chức đã bật.

Vì vậy, lựa chọn cấp mô hình không phải cam kết cố định một lần. Trong cùng một công việc, phần chuẩn bị thường lệ có thể chạy trên cấp nhẹ hơn, còn phần tổng hợp khó dùng cấp có năng lực cao nhất. Người bán hoa có thể trích điều kiện của từng nhà bán buôn bằng Haiku, rồi chuyển sang Opus để đưa ra khuyến nghị. Không bao giờ mở bộ chọn chỉ phục vụ được nhiệm vụ trung bình và khiến cả hai đầu của phổ công việc không được xử lý phù hợp. Mặc định cố định phản ánh trạng thái tài khoản, không phải quyết định về công việc của bạn.

## Trong bài thi

Hướng dẫn thi nêu ba họ mô hình. Mục tiêu này tồn tại vì không có cấp nào phù hợp mọi nhiệm vụ. Bài thi kiểm tra khả năng đọc đúng yêu cầu thực tế của nhiệm vụ, không dựa vào mức độ danh giá; đây là kỹ năng vẫn có giá trị dù danh sách mô hình thay đổi. Trong chính câu hỏi mẫu của hướng dẫn, một lượng lớn bản nháp ngắn, thường lệ, mà tốc độ và chi phí quan trọng hơn suy luận sâu được ghép với mô hình nhanh hơn, chi phí thấp hơn. “Luôn dùng mô hình cao nhất” là một đáp án sai được nêu rõ.

### Bẫy chọn theo mức độ danh giá

“Dự án này quan trọng” không biến một nhiệm vụ thường lệ thành việc cần cấp cao nhất. Tầm quan trọng thuộc về dự án; mức độ đòi hỏi thuộc về nhiệm vụ. Bài thi chọn cấp phù hợp với nhiệm vụ trước mắt. Định dạng lại thường lệ trong một dự án chủ lực vẫn chỉ là định dạng lại thường lệ.

Tên mô hình cụ thể và danh sách hiện hành thay đổi theo thời gian và nên được đặt trong tài liệu tra cứu nhanh.

## Những bẫy thường gặp trong bài thi

### Chọn mô hình mạnh nhất cho mọi việc vì công việc quan trọng

Đây là lựa chọn theo mức độ danh giá. Phần giải thích câu hỏi mẫu trong hướng dẫn gọi việc luôn dùng mô hình cao nhất là lãng phí ngân sách chi phí và độ trễ. Công việc thường lệ, khối lượng lớn không cần chiều sâu; tầm quan trọng của dự án không làm mọi nhiệm vụ trong đó trở nên đòi hỏi cao.

### Giao việc rõ ràng cần chiều sâu cho cấp nhanh nhất vì cho rằng chỉ là viết

Đây là tiết kiệm sai chỗ. Yêu cầu chất lượng phụ thuộc hậu quả nếu sai: đầu ra ngắn nhưng chứa phán đoán, mâu thuẫn hoặc hệ quả chính là nơi cấp mạnh hơn xứng đáng với thời gian cần thêm, dù gõ văn bản đó nhanh đến đâu.

### Chấp nhận phương án nói cấp nhẹ hơn cho chất lượng tương đương ở công việc đòi hỏi cao

Tài liệu không khẳng định các cấp tương đương và không đáp án đúng nào dựa vào điều đó. Cấp nhẹ hơn được lựa chọn vì phù hợp nhiệm vụ cùng quy trình kiểm tra. Khi phần dẫn đòi hỏi chiều sâu, phương án dùng cấp nhẹ hơn là sai dù được diễn đạt tự tin đến đâu.

## Tình huống luyện tập

Một hợp tác xã năng lượng cộng đồng có một nhân viên hành chính với hai việc song song: chuẩn hóa 600 hồ sơ thành viên theo cùng định dạng địa chỉ và soạn phản hồi của hợp tác xã cho đợt tham vấn quy định phức tạp, trong đó ba thành viên hội đồng quản trị đưa ra định hướng có phần mâu thuẫn. Cô phải giữ chi phí công việc thường lệ thấp nhất có thể mà không làm giảm chất lượng lập trường của hợp tác xã. Nên phân công mô hình thế nào?

**Phương án A**

Dùng mô hình mạnh nhất cho hồ sơ thành viên vì độ chính xác dữ liệu quan trọng ở quy mô đó; dùng mô hình nhanh nhất cho phản hồi tham vấn vì một lá thư được tạo ra nhanh.

**Phương án B**

Xử lý 600 hồ sơ bằng mô hình nhanh nhất, chi phí thấp hơn và kiểm tra chọn mẫu; soạn phản hồi tham vấn quy định bằng mô hình có năng lực cao nhất.

**Phương án C**

Dùng mô hình nhanh nhất cho cả hai việc, vì hồ sơ là công việc thường lệ và phản hồi tham vấn chỉ là soạn thảo thông thường khi đã dán đủ quan điểm của ba thành viên hội đồng.

**Phương án D**

Dùng mô hình mạnh nhất cho cả hai, vì danh tiếng của hợp tác xã với toàn bộ thành viên phụ thuộc vào công việc này và mô hình tốt nhất tối đa hóa chất lượng ở mọi chỗ.

## Bài tập thực hành: Ghép các nhiệm vụ trong tuần với cấp mô hình

**Thời gian:** 25 phút.

### Bạn sẽ học được

- Cách gắn nhãn nhiệm vụ: thường lệ với khối lượng lớn, công việc hằng ngày ở cấp giữa hoặc tổng hợp có ảnh hưởng hệ trọng.
- Cách kiểm tra bộ chọn để biết tài khoản của bạn có những mô hình nào.
- Cách chạy nhiệm vụ thường lệ trên cấp nhẹ hơn và kiểm tra chất lượng theo mẫu.
- Cách nêu lợi ích của chiều sâu với nhiệm vụ thực sự đòi hỏi cao.

### Bước 1 — Liệt kê các nhiệm vụ Claude trong tuần làm việc gần nhất

Gắn cho mỗi nhiệm vụ một nhãn: thường lệ với khối lượng lớn, công việc hằng ngày ở cấp giữa hoặc tổng hợp có ảnh hưởng hệ trọng.

**Vì sao:** Ba nhãn này tương ứng với các nhóm dấu hiệu trong phần dẫn câu hỏi thi. Thực hành trên công việc của bạn giúp nhận ra chúng nhanh hơn.

**Kết quả cần thấy:** Danh sách ngắn các nhiệm vụ thực tế, mỗi nhiệm vụ có một trong ba nhãn.

### Bước 2 — Đối chiếu cấp cần dùng với cấp đã dùng và mở bộ chọn

Với từng nhiệm vụ, ghi cấp mà yêu cầu thực tế đòi hỏi và cấp bạn đã sử dụng. Sau đó mở bộ chọn mô hình để xác nhận tài khoản có những mô hình nào.

**Vì sao:** Chênh lệch giữa cấp cần dùng và cấp thực tế cho thấy thói quen giữ nguyên một thiết lập.

**Kết quả cần thấy:** Hai cột cấp mô hình cho mỗi nhiệm vụ, cùng danh sách mô hình hiện hiển thị trong bộ chọn.

### Bước 3 — Chạy lại một nhiệm vụ thường lệ trên cấp nhẹ hơn

Kiểm tra một mẫu đầu ra theo tiêu chuẩn chất lượng của bạn.

**Vì sao:** Phù hợp nhiệm vụ cùng quy trình kiểm tra là cơ sở dùng cấp nhẹ hơn. Kiểm tra chọn mẫu khiến lựa chọn trở nên chuyên nghiệp thay vì chỉ đơn thuần rẻ.

**Kết quả cần thấy:** Đầu ra vượt qua kiểm tra mẫu và được tạo nhanh hơn thiết lập bạn thường dùng.

### Bước 4 — Chọn nhiệm vụ gần đây đòi hỏi cao nhất

Viết một câu về lợi ích mà cấp mạnh hơn đã mang lại hoặc có thể mang lại, trong khi tốc độ không thể thay thế.

**Vì sao:** Nêu lợi ích trong một câu giúp kiểm tra nhiệm vụ thực sự cần chiều sâu hay chỉ khiến bạn cảm thấy quan trọng.

**Kết quả cần thấy:** Một câu nêu lợi ích cụ thể: tháo gỡ mâu thuẫn, giữ được sắc thái tinh tế hoặc tránh một hệ quả.

### Bước 5 — Đánh dấu lựa chọn theo mức độ danh giá và gắn nhãn lại

Tìm những nhiệm vụ bạn chọn theo mức độ danh giá thay vì yêu cầu thực tế, rồi ghi lại cấp thực sự cần dùng.

**Vì sao:** Chọn theo mức độ danh giá là đáp án sai thường lặp lại ở mục tiêu này. Phát hiện nó trong tuần của mình giúp bạn tránh nó khi đọc phần dẫn câu hỏi.

**Kết quả cần thấy:** Ít nhất một lần gắn nhãn lại trung thực, hoặc xác nhận tuần đó thực sự không có trường hợp nào như vậy.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Tổng quan các mô hình — *Models overview*.
- Thay đổi mô hình, mức nỗ lực và thiết lập suy nghĩ — *Change the model, effort, and thinking settings*.
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [3.1 — Lựa chọn tính năng Claude phù hợp](3-1-product-feature-selection.vi.md).
- **Bài tiếp theo:** [3.3 — Lựa chọn mô hình phù hợp với chi phí, tốc độ và chất lượng](3-3-cost-speed-quality.vi.md).
