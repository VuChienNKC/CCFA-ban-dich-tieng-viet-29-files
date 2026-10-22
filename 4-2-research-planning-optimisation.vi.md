# 4.2 — Sử dụng Claude cho nghiên cứu, lập kế hoạch và tối ưu hóa quy trình

- **Lĩnh vực (Domain):** 4
- **Nhiệm vụ (Task):** 4.2
- **Tên bài gốc:** Using Claude for Research, Planning and Process Optimisation
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/4-workflow-integration/4-2-research-planning-optimisation)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

**Nghiên cứu (research)** thu thập và tổng hợp tài liệu bên ngoài, giúp bạn bắt đầu từ thông tin đã có thay vì một màn hình trắng. **Lập kế hoạch (planning)** biến mục tiêu thành các bước có thứ tự. **Tối ưu hóa quy trình (process optimisation)** tìm và sửa bước làm chậm quy trình. Cả ba có chung một cách làm: Claude tạo phiên bản ban đầu, còn bạn chịu trách nhiệm về phán đoán sau đó.

Hãy xét một công ty môi giới bất động sản mà người quản lý dùng Claude cho cả ba việc: tìm hiểu cách các công ty khác định giá, lên kế hoạch cuối tuần đón khách xem nhà và xử lý tình trạng cho thuê chậm.

## Nghiên cứu ở hai quy mô

Sản phẩm hỗ trợ nghiên cứu ở hai quy mô, và Trung tâm trợ giúp chỉ rõ ranh giới. **Tìm kiếm web** phù hợp với câu hỏi sự kiện đơn giản có thể trả lời bằng một hoặc hai lượt tra cứu. **Chế độ Research** thực hiện nhiều lượt tìm kiếm nối tiếp, mỗi lượt dựa vào kết quả trước. Nó khám phá các góc độ khác nhau của câu hỏi và xử lý có hệ thống những vấn đề còn mở. Kết quả có trích dẫn và phù hợp công việc lớn hơn, cần nhiều nguồn. Ở công ty môi giới, tra một quy định cho thuê dùng tìm kiếm web; khảo sát cách định giá dùng Research.

Giá trị nằm ở độ bao quát và tốc độ. Giới hạn là mọi thông tin quan trọng phải được kiểm tra trước khi bất kỳ ai nhắc lại, dù có trích dẫn hay không: trích dẫn cho biết phát hiện đến từ đâu, không chứng minh phát hiện đúng.

## Kế hoạch được xây dựng từ những ràng buộc đã nêu

Một kế hoạch ban đầu hữu ích hơn trang giấy trắng. Claude đặc biệt giỏi ở việc bao quát đầy đủ. Hỏi kế hoạch đang thiếu gì, bạn sẽ nhận được các mối phụ thuộc, vấn đề về trình tự và bước mọi người hay quên.

Claude cũng sẽ tự tin lập kế hoạch mà không tính đến các ràng buộc bạn chưa đề cập, vì nó không biết chúng: lối vào duy nhất bảo đảm khả năng tiếp cận, tình nguyện viên không làm được Chủ nhật hoặc phòng bị trùng lịch đặt. Không có gì trong đầu ra cảnh báo rằng kế hoạch được xây dựng khi thiếu những thông tin ấy. Kế hoạch đón khách xem nhà không nêu ràng buộc có thể xếp một nhân viên tư vấn giao dịch vốn không làm Chủ nhật vào các buổi xem nhà Chủ nhật. Đó là kế hoạch hư cấu nhưng đọc lên có vẻ chuyên nghiệp, nguy hiểm hơn kế hoạch rõ ràng kém vì khiến người đọc tin tưởng.

Biện pháp khắc phục ít tốn công. Hướng dẫn thiết kế prompt cho nghiệp vụ của Anthropic khuyên xem Claude như thực tập sinh trong ngày đầu, cần chỉ dẫn rõ ràng, tường minh và đủ chi tiết cần thiết. Muốn có kế hoạch hữu ích, hãy đưa các ràng buộc thực tế vào bản giao việc, rồi yêu cầu nêu những giả định làm nền tảng cho kế hoạch. Giả định được viết ra là giả định bạn có thể sửa.

## Vòng lặp tối ưu hóa

Claude tạo giả thuyết về những chỗ quy trình chậm, dễ xảy ra trục trặc hoặc bị trùng lặp. Nó không thể cho biết giả thuyết nào đúng vì chưa từng quan sát quy trình của bạn vận hành. Dữ liệu mới quyết định. Vòng lặp có bốn bước:

1. Mô tả quy trình và các ràng buộc.
2. Yêu cầu những điểm nghẽn có thể có và bằng chứng để xác nhận từng điểm.
3. Thu thập bằng chứng đó.
4. Thay đổi bước mà bằng chứng chỉ ra là có vấn đề.

Bằng chứng được thu thập sau khi đã nêu các giả thuyết để bạn biết đang tìm gì. Bằng chứng phải có trước mọi thay đổi để thay đổi có mục tiêu. Với việc cho thuê của công ty môi giới, Claude có thể đề xuất nguyên nhân là thẩm tra người thuê chậm hoặc chủ nhà phê duyệt muộn; các mốc thời gian từng giai đoạn trong chính hồ sơ công ty sẽ quyết định.

Cùng hướng dẫn đó khuyên tiếp cận công việc như nhà khoa học: thường xuyên thử nghiệm và tinh chỉnh, đồng thời kết hợp việc viết prompt với chuyên gia nghiệp vụ của tổ chức thay vì chỉ tin riêng một phía.

## Chọn sai điểm nghẽn

Sai lầm tốn kém nhất là tối ưu một bước vốn không phải yếu tố hạn chế. Bạn tiêu ngân sách và sự sẵn sàng thay đổi cho thứ đang hoạt động ổn. Điều này thường bắt nguồn từ việc xem giả thuyết nghe hợp lý nhất là giả thuyết đã được xác nhận. Nguyên nhân có vẻ hợp lý và nguyên nhân thật trùng nhau đủ thường xuyên để cám dỗ bạn, nhưng không đủ thường xuyên để tránh tốn kém. Bằng chứng phân biệt chúng thường chỉ cần một ngày để thu thập. Mua dịch vụ thẩm tra nhanh hơn khi các mốc thời gian cho thấy chủ nhà phê duyệt muộn chỉ tiêu tiền của công ty và giữ nguyên sự chậm trễ.

## Trong bài thi

Bài thi kiểm tra phán đoán, không phải phiên bản ban đầu. Mọi đáp án đúng trong mục tiêu này hoặc cung cấp sự thật Claude không thể biết, hoặc kiểm tra trước khi hành động. Các phương án gây nhiễu thường xem đầu ra trôi chảy là sản phẩm đã hoàn tất. Lĩnh vực 3 quyết định tính năng nào thực hiện nghiên cứu; mục tiêu này kiểm tra cách làm việc xung quanh nó. Kiểm tra phát hiện trước khi nhắc lại là kỷ luật của Lĩnh vực 2.

### Dấu hiệu của cách làm chuyên nghiệp

Trong phần dẫn của mục tiêu này, đáp án đúng kiểm tra bằng chứng trước khi thay đổi bất cứ điều gì: thời gian xử lý mùa trước, hồ sơ sử dụng hoặc nhật ký khiếu nại. Các phương án gây nhiễu xây lại quy trình dựa trên lập luận trôi chảy hoặc dùng tính năng mạnh hơn khi vấn đề thực sự là thiếu dữ kiện tại chỗ.

## Những bẫy thường gặp trong bài thi

### Xem kế hoạch hợp lý, có cấu trúc tốt là kế hoạch đã được kiểm tra

Tính hợp lý là đặc điểm của câu chữ; tính phù hợp thực tế đến từ ràng buộc và dữ kiện người lập kế hoạch cung cấp. Kế hoạch không có ràng buộc thật sẽ thất bại khi gặp sự kiện thật. Đáp án đúng nêu ràng buộc từ đầu hoặc đối chiếu bản nháp với chúng trước khi tin dùng.

### Thay đổi quy trình chỉ dựa vào giả thuyết nghe thuyết phục nhất

Các điểm nghẽn Claude đề xuất là giả thuyết, chưa phải chẩn đoán: nó chưa từng quan sát quy trình vận hành. Hành động theo giả thuyết hợp lý nhất sẽ tiêu tiền cho bước chưa bị bằng chứng nào chỉ ra là có vấn đề. Đáp án đúng thu thập bằng chứng trước.

### Dùng thêm nghiên cứu thay cho bằng chứng tại chỗ

Trích dẫn từ nơi khác không xác định được nguyên nhân nào đúng trong quy trình của bạn. Khi câu hỏi là vì sao quy trình này vận hành như vậy, bằng chứng quyết định là dữ liệu tại chỗ. Không lượng tổng hợp bên ngoài nào thay thế được; dùng tính năng mạnh hơn không đồng nghĩa với trả lời được câu hỏi.

## Tình huống luyện tập

Điều phối viên chương trình cho thuê xe đạp của một thành phố liên tục nghe rằng các trạm ở vùng ngoại ô có nhiều người đi làm vào thành phố đã hết xe lúc 8 giờ sáng. Cô mô tả chương trình cho Claude, và Claude đề xuất bốn nguyên nhân hợp lý: vòng điều chuyển xe ban đêm kết thúc quá sớm; hai trạm khu dân cư cùng phục vụ một cụm văn phòng; bảo dưỡng cuối tuần khiến xe chưa được đưa trở lại hoạt động vào thứ Hai; người dùng đến trạm đầy thì tiếp tục đạp xe đi. Chỉ số liệu của chính chương trình mới xác định được nguyên nhân đang xảy ra; cô sẽ không hành động theo giả thuyết nào trước khi có kết quả. Bước tiếp theo chuyên nghiệp là gì?

**Phương án A**

Thêm ngay vòng điều chuyển xe thứ hai vào buổi sáng, vì nguyên nhân đầu Claude nêu là hợp lý nhất và khiếu nại xuất hiện vào buổi sáng.

**Phương án B**

Hỏi Claude bằng chứng nào xác nhận hoặc loại trừ từng nguyên nhân, rồi lấy dữ liệu chuyến đi và đỗ xe của chương trình trước khi thay đổi bất cứ điều gì.

**Phương án C**

Chạy lại cùng câu hỏi trong Research để bốn nguyên nhân dự kiến có trích dẫn hỗ trợ từ các chương trình xe đạp của thành phố khác.

**Phương án D**

Nhờ Claude thiết kế lại mạng trạm theo luồng đi làm, xem các trạm hết xe buổi sáng là bằng chứng đủ cho thấy bố trí hiện tại đã thất bại.

## Bài tập thực hành: Lập kế hoạch hai lần rồi tìm điểm nghẽn thực sự

**Thời gian:** 40 phút.

### Bạn sẽ học được

- Cách các ràng buộc được nêu rõ thay đổi mức hữu ích của kế hoạch ban đầu.
- Cách nhận diện lỗi kế hoạch hư cấu nhưng đọc lên có vẻ chuyên nghiệp.
- Cách thực hiện vòng lặp mô tả, giả thuyết, bằng chứng, thay đổi.
- Cách kiểm tra dữ liệu có chỉ vào bước bạn vốn dự đoán hay không.

### Bước 1 — Chọn một công việc sắp tới có ràng buộc thực tế

Ví dụ: sự kiện, lịch trực, đợt ra mắt hoặc bất kỳ công việc nào bạn thực sự phụ trách.

**Vì sao:** Bài tập chỉ hiệu quả khi bạn biết ràng buộc thật đủ rõ để phát hiện kế hoạch phớt lờ chúng.

**Kết quả cần thấy:** Một công việc được nêu tên và ghi riêng ba ràng buộc quan trọng nhất.

### Bước 2 — Nhờ Claude lập kế hoạch ban đầu hai lần

Lần đầu không nêu ràng buộc; lần sau viết rõ ba ràng buộc thực tế quan trọng nhất.

**Vì sao:** So sánh làm lộ lỗi cốt lõi của mục tiêu: kế hoạch không có ràng buộc đọc lên vẫn chuyên nghiệp như kế hoạch có ràng buộc.

**Kết quả cần thấy:** Hai kế hoạch trôi chảy, khác nhau đúng ở những chỗ ràng buộc của bạn có tác động.

### Bước 3 — Liệt kê điều kế hoạch không có ràng buộc đã làm sai

Chỉ ra những chỗ sai nhưng đọc lên vẫn hoàn toàn có lý.

**Vì sao:** Gọi tên các chi tiết hư cấu giúp hình thành phản xạ kiểm tra kế hoạch bằng dữ kiện thay vì độ trôi chảy.

**Kết quả cần thấy:** Ba hoặc bốn lỗi cụ thể mà người không biết ràng buộc sẽ không nhận ra.

### Bước 4 — Chọn quy trình có vẻ chậm và yêu cầu giả thuyết cùng bằng chứng

Mô tả quy trình từ đầu đến cuối cho Claude. Yêu cầu bốn điểm nghẽn có thể có và bằng chứng để xác nhận hoặc loại trừ từng điểm.

**Vì sao:** Đây là nửa đầu vòng lặp tối ưu hóa: giả thuyết cùng bằng chứng giúp quyết định giữa chúng.

**Kết quả cần thấy:** Bốn nguyên nhân dự kiến, mỗi nguyên nhân gắn với một bằng chứng cụ thể có thể thu thập.

### Bước 5 — Thu thập một bằng chứng trong tuần này

Ghi lại dữ liệu có chỉ vào bước bạn vốn dự đoán hay không.

**Vì sao:** Khoảng cách giữa điểm nghẽn dự đoán và điểm nghẽn có bằng chứng chính là bài học; phần lớn mọi người sẽ bất ngờ ít nhất một lần.

**Kết quả cần thấy:** Một dữ liệu thực tế và kết luận một dòng: dự đoán được xác nhận hoặc dự đoán sai.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Sử dụng Research trên Claude — *Use research on Claude*.
- Khi nào nên dùng tìm kiếm web, suy nghĩ mở rộng và Research? — *When should I use web search, extended thinking, and research?*
- Thiết kế prompt để nâng cao hiệu quả kinh doanh — *Prompt engineering for business performance*.
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

**Ghi chú của tác giả bài gốc:** Không có tài liệu Anthropic nào đề cập tối ưu hóa quy trình như một kỹ năng nghiệp vụ. Bài học dựa trên mục tiêu trong hướng dẫn thi và thực hành tiêu chuẩn; các bài viết trên chỉ hỗ trợ những điểm mà chúng được trích dẫn cho.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [4.1 — Phân tích yêu cầu và trường hợp sử dụng](4-1-requirements-and-use-cases.vi.md).
- **Bài tiếp theo:** [4.3 — Hỗ trợ thiết kế, phát triển và tinh chỉnh giải pháp](4-3-solution-design-iteration.vi.md).
