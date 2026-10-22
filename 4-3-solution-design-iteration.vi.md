# 4.3 — Hỗ trợ thiết kế, phát triển và tinh chỉnh giải pháp

- **Lĩnh vực (Domain):** 4
- **Nhiệm vụ (Task):** 4.3
- **Tên bài gốc:** Supporting Solution Design, Development and Iteration
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/4-workflow-integration/4-3-solution-design-iteration)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

**Tinh chỉnh giải pháp qua nhiều vòng (solution iteration)** là cải thiện sản phẩm bàn giao qua nhiều lượt, với Claude làm đối tác soạn thảo. Trong chứng nhận này, giải pháp là quy trình, mẫu biểu, tài liệu hướng dẫn, phương án, thiết kế dịch vụ, biểu mẫu hoặc kế hoạch. Giải pháp ở đây không phải phần mềm. Mỗi vòng được kiểm tra theo một tiêu chí: một phép thử rút ra từ yêu cầu đã xác lập ở bài 4.1.

Hãy xét một quán cà phê mà chủ quán muốn có danh sách kiểm tra mở cửa thứ Bảy cho một nhân viên pha chế làm một mình. Yêu cầu nêu đối tượng sử dụng và những tình huống danh sách phải xử lý được, chẳng hạn sữa được giao muộn. Bản nháp đầu tiên của Claude có thể dùng được.

## Vì sao đáng thực hiện vòng lặp?

Trước đây, việc tinh chỉnh tốn kém nên mọi người thường bảo vệ bản nháp đầu tiên. Chi phí tạo phương án khác là lý lẽ phản đối việc xem thêm phương án. Claude thay đổi bài toán chi phí. Phiên bản thứ hai và thứ ba chỉ mất vài phút, nên bạn có thể dành công sức xem xét chúng. So sánh ba phương án cụ thể là cách thiết kế tốt hơn tranh luận quanh một phương án. Câu hỏi của chủ quán chuyển từ danh sách có tốt không sang phiên bản nào đáp ứng được yêu cầu. Sự chuyển đổi ấy là trọng tâm mục tiêu này. Nó chỉ hiệu quả khi bạn vẫn sẵn sàng bỏ các phiên bản. Bản nháp ít tốn công có thể được bỏ mà không cần thủ tục; phiên bản không ai quá gắn bó có thể được kiểm tra trung thực.

## Mỗi vòng có một tiêu chí được nêu rõ

Mỗi vòng cần một tiêu chí cụ thể lấy từ yêu cầu. Điều này phân biệt tinh chỉnh có mục tiêu với chỉnh sửa tùy hứng. “Làm tốt hơn” tạo ra thứ khác, chưa chắc tốt hơn. Không có thông tin mới thì lần sửa không có mục tiêu. Vì cùng lý do, cách khắc phục câu trả lời không hữu ích mà Trung tâm trợ giúp nêu là phản hồi cụ thể thay vì chỉ yêu cầu thử lại. “Điều chỉnh để phương án này vẫn hoạt động trong ngày mưa” là thay đổi có thể kiểm tra.

Thực hiện mỗi vòng theo một tiêu chí, kiểm tra kết quả chỉ theo tiêu chí đó và giữ phiên bản đạt. Chủ quán yêu cầu danh sách vẫn dùng được khi sữa giao muộn, rồi chỉ kiểm tra điều đó. Hai phiên bản được đánh giá bằng cùng phép thử có thể được xếp hạng. Hai phiên bản đánh giá bằng cảm nhận tổng thể chỉ dẫn đến tranh luận. Khóa AI Fluency của Anthropic gọi nhịp làm việc này là **Vòng lặp Mô tả – Phân định (Description–Discernment Loop)**: mô tả nhu cầu, đánh giá kết quả nhận được, tinh chỉnh rồi lặp lại.

## Biết khi nào nên dừng

Dừng khi các thay đổi còn lại chỉ là sở thích thay vì mức độ đáp ứng yêu cầu. Trau chuốt sản phẩm đã đạt yêu cầu lấy mất thời gian mà vấn đề tiếp theo cần. Nó cũng mở đường cho lỗi tinh tế hơn: phiên bản trôi chảy, tự tin có thể thay thế phiên bản mà người dùng thực sự cần. Vì vậy, hãy kiểm tra theo yêu cầu và người dùng, không theo việc câu chữ đọc hay đến đâu.

Nếu một vòng cho thấy chính yêu cầu đã sai, bước tiếp theo phải là xem lại yêu cầu, không phải tạo thêm bản nháp. Không lượng sửa đổi nào khắc phục được sản phẩm nhắm sai mục tiêu. Giả sử chủ quán biết thực tế có hai nhân viên mở cửa thứ Bảy. Yêu cầu cần được viết lại trước mọi bản nháp tiếp theo. Dù vòng lặp kết thúc theo cách nào, hãy nêu lý do dừng trong một dòng. Gọi tên lý do giúp lần thực hiện sau giữ được tính thực chất.

## Artifact và các nhánh

Cơ chế sản phẩm hỗ trợ vòng lặp này nằm ở artifact. Nội dung đáng kể, độc lập được đưa vào cửa sổ riêng. Bạn sửa bằng cách yêu cầu Claude thay đổi artifact. Để so sánh hai phương án cụ thể, hãy sửa tin nhắn đã tạo bản nháp. Thao tác đó tạo phiên bản khác của cuộc trò chuyện với các artifact riêng, còn nhánh gốc giữ nguyên bản nháp đầu tiên. Chủ quán có danh sách thứ hai mà không mất bản đầu. So sánh hai nhánh tốt hơn tin vào trí nhớ về vòng trước, vì trí nhớ thường thiên vị phiên bản xuất hiện sau cùng. Giữ yêu cầu trong tầm nhìn khi so sánh. Các nhánh cho thấy phiên bản; chỉ yêu cầu mới quyết định phiên bản nào thắng.

## Trong bài thi

Thí sinh thường nhầm mục tiêu này với Lĩnh vực 1. Tinh chỉnh prompt để có câu trả lời tốt hơn thuộc mục tiêu 1.3. Tinh chỉnh giải pháp với Claude làm đối tác soạn thảo thuộc 4.3: cùng vòng lặp nhưng áp dụng lên đối tượng khác.

### Khái niệm cốt lõi

Khi phần dẫn của mục tiêu 4.3 đưa ra bản nháp đầu tiên có thể dùng được, đáp án đúng nêu một tiêu chí rút từ yêu cầu rồi kiểm tra bản sửa theo tiêu chí ấy. Các phương án gây nhiễu trau chuốt không có tiêu chí, tạo nhiều phiên bản rồi chọn bằng cảm giác hoặc đưa bản nháp chưa kiểm tra vào sử dụng thật. Khi phần dẫn cho thấy chính yêu cầu sai, đáp án đúng quay lại xem xét yêu cầu.

## Những bẫy thường gặp trong bài thi

### Liên tục yêu cầu “làm tốt hơn” mà không nêu tiêu chí

Mỗi vòng tạo phiên bản khác nhau nhưng không bản nào chứng minh được là tốt hơn, vì lần sửa không có mục tiêu. Đáp án đúng nêu một tiêu chí từ yêu cầu rồi kiểm tra kết quả theo tiêu chí đó. Tạo lại cho đến khi cảm thấy ổn chỉ là hoạt động, chưa phải tiến bộ.

### Viết lại sản phẩm trong khi yêu cầu đã sai

Không lượng sửa đổi nào khắc phục được sản phẩm nhắm sai mục tiêu. Khi phần dẫn cho thấy yêu cầu đã không phù hợp, cách làm chuyên nghiệp là quay lại công việc của bài 4.1. Mọi vòng viết lại tiếp theo đều là phương án gây nhiễu.

### Để phiên bản viết hay nhất đánh bại phiên bản phù hợp

Trôi chảy không đồng nghĩa phù hợp. Phiên bản được kiểm tra theo yêu cầu và người dùng, không theo văn phong của nhau. Bản nháp thân thiện, tự tin nhưng bỏ lỡ ràng buộc bắt buộc chính là phiên bản bài thi yêu cầu bạn loại bỏ.

## Tình huống luyện tập

Điều phối viên tiệc tại khu vui chơi bắn súng laser đang thiết kế trình tự chương trình cho gói tiệc sinh nhật mới. Yêu cầu đã cố định: trẻ từ 7 đến 11 tuổi, hướng dẫn an toàn trước khi bất kỳ ai chơi, ăn uống trong phòng tiệc và hoàn thành trong khung 90 phút. Bản nháp đầu tiên của Claude có thể dùng được. Cô muốn vòng hai tạo ra phiên bản có thể đánh giá rõ là đạt hoặc không đạt, trước khi bất kỳ buổi tiệc thật nào dựa vào nó. Vòng hai nên thực hiện thế nào?

**Phương án A**

Dùng nguyên bản nháp cho các buổi tiệc cuối tuần này, xem các buổi thật là vòng kiểm tra rồi điều chỉnh sau.

**Phương án B**

Yêu cầu Claude làm trình tự chương trình vui hơn, trau chuốt hơn và tiếp tục tạo lại đến khi có phiên bản cảm thấy phù hợp.

**Phương án C**

Mở chat mới cho từng bản nháp, thu thập năm trình tự chương trình khác nhau rồi chọn bản đọc hay nhất về tổng thể.

**Phương án D**

Sửa theo một tiêu chí được nêu rõ, chẳng hạn chương trình vẫn vận hành được khi khách đến muộn 15 phút, rồi kiểm tra kết quả chỉ theo tiêu chí đó.

## Bài tập thực hành: Ba vòng, ba tiêu chí

**Thời gian:** 35 phút.

### Bạn sẽ học được

- Cách viết yêu cầu trước bản nháp đầu tiên.
- Cách thực hiện một vòng sửa theo đúng một tiêu chí được nêu rõ.
- Cách so sánh phiên bản bằng cách phân nhánh cuộc trò chuyện.
- Cách nhận ra điểm dừng và vấn đề ở chính yêu cầu.

### Bước 1 — Chọn sản phẩm bàn giao thực tế bạn phụ trách

Ví dụ: mẫu biểu, danh sách kiểm tra, trang hướng dẫn hoặc kế hoạch.

**Vì sao:** Phán đoán điểm dừng chỉ hiệu quả với công việc mà bạn thực sự hiểu người dùng và các ràng buộc.

**Kết quả cần thấy:** Một sản phẩm được nêu tên, có đối tượng đọc thực tế đang cần nó.

### Bước 2 — Viết yêu cầu trước trong ba đến năm dòng

Nêu dành cho ai, phải xử lý được những tình huống nào và các ràng buộc bắt buộc.

**Vì sao:** Tiêu chí đến từ yêu cầu. Không có yêu cầu, mọi vòng sau đều trở thành “làm tốt hơn” chung chung.

**Kết quả cần thấy:** Ghi chú yêu cầu ngắn mà đồng nghiệp có thể dùng để kiểm tra bản nháp.

### Bước 3 — Tạo bản nháp đầu tiên rồi thực hiện vòng hai theo một tiêu chí

Lấy bản nháp từ Claude; sau đó chạy vòng hai theo đúng một tiêu chí được nêu rõ từ yêu cầu và ghi đạt hoặc không đạt.

**Vì sao:** Một tiêu chí mỗi vòng giúp thay đổi có thể kiểm tra. Ba tiêu chí cùng lúc khiến bạn không biết thay đổi nào khắc phục điều gì.

**Kết quả cần thấy:** Một phiên bản sửa và kết luận đạt hoặc không đạt đối với tiêu chí đã nêu.

### Bước 4 — Thực hiện vòng ba theo tiêu chí thứ hai và so sánh trực tiếp

Phân nhánh chat từ tin nhắn vòng hai hoặc giữ các bản sao đặt cạnh nhau để so sánh thay vì tin vào trí nhớ.

**Vì sao:** So sánh phiên bản cụ thể là phương pháp thiết kế. Trí nhớ thường thiên vị phiên bản xuất hiện sau cùng.

**Kết quả cần thấy:** Hai hoặc ba phiên bản được so sánh trực tiếp, xác định rõ bản được giữ lại.

### Bước 5 — Dừng và viết một dòng giải thích

Hoặc các thay đổi còn lại chỉ là sở thích, nghĩa là đã hoàn thành; hoặc xuất hiện vấn đề ở yêu cầu, nghĩa là bước tiếp theo phải xem lại yêu cầu thay vì tạo bản nháp khác.

**Vì sao:** Gọi tên lý do dừng xây dựng khả năng phán đoán mà mục tiêu thực sự kiểm tra.

**Kết quả cần thấy:** Một câu: hoàn thành vì đã đáp ứng yêu cầu, hoặc tạm dừng vì yêu cầu cần làm lại.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Artifact là gì và sử dụng như thế nào? — *What are artifacts and how do I use them?*
- Prompt của tôi không tạo ra câu trả lời hữu ích — *My prompt isn't giving me a helpful answer*.
- AI Fluency: Khung năng lực và nền tảng — *AI Fluency: Framework and Foundations*.
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

**Ghi chú của tác giả bài gốc về AI Fluency:** Tên các thành phần là tên mô-đun của khóa học; phần giải thích ngắn cho từng thành phần là cách tác giả diễn giải nội dung khóa học.

**Ghi chú của tác giả bài gốc về phạm vi nguồn:** Không có tài liệu Anthropic nào đề cập thiết kế và tinh chỉnh sản phẩm bàn giao nghiệp vụ. Bài học dựa trên mục tiêu trong hướng dẫn thi và thực hành thiết kế tiêu chuẩn; bài viết về artifact giải thích cơ chế sản phẩm.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [4.2 — Sử dụng Claude cho nghiên cứu, lập kế hoạch và tối ưu hóa quy trình](4-2-research-planning-optimisation.vi.md).
- **Bài tiếp theo:** [4.4 — Tích hợp Claude vào quy trình làm việc hiện có](4-4-integrating-existing-workflows.vi.md).
