# 4.4 — Tích hợp Claude vào quy trình làm việc hiện có

- **Lĩnh vực (Domain):** 4
- **Nhiệm vụ (Task):** 4.4
- **Tên bài gốc:** Integrating Claude into Existing Workflows
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/4-workflow-integration/4-4-integrating-existing-workflows)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Trong chứng nhận này, **tích hợp (integration)** đặt câu hỏi con người đưa công việc đến Claude ở bước nào của quy trình hiện có và quy trình có giữ nguyên cấu trúc hay không. Từ này không mang nghĩa kết nối kỹ thuật giữa các hệ thống. **Bổ trợ (augment)** là giao cho Claude một bước chậm. **Thiết kế lại (redesign)** là thay đổi chính quy trình. **Chuyển xử lý (escalate)** là chuyển công việc vượt phạm vi vai trò Associate cho người khác.

Hãy xét một tiệm giặt khô. Mỗi thứ Hai, người quản lý tổng hợp các yêu cầu bồi thường do hư hỏng của tuần trước. Khách để quần áo chưa đến lấy được gửi thư nhắc.

## Bổ trợ: Làm tốt hơn một bước

Khi Claude đảm nhiệm bước chậm, mọi phần khác giữ nguyên cấu trúc. Việc tổng hợp mất 10 phút thay vì một giờ. Người quản lý vẫn chịu trách nhiệm và công việc của người khác không thay đổi. Vì vậy, bổ trợ ít tốn kém, có thể đảo ngược và dễ giải thích với đồng nghiệp. Nếu không hiệu quả, người quản lý quay lại tự viết. Đây là lựa chọn phù hợp thường xuyên hơn nhiều so với phương án tham vọng. Phần lớn cách tích hợp thành công ở cấp Associate là làm tốt hơn một bước.

## Thiết kế lại: Thử nghiệm quy mô nhỏ trước

Trong thiết kế lại, quy trình thay đổi vì ràng buộc từng định hình nó đã không còn. Cá nhân hóa thư nhắc từng mất 20 phút, nên tiệm giặt khô gửi một thư chung. Khi chỉ mất hai phút, cách tiếp cận phân tầng trước đây không ai đề xuất trở nên khả thi.

Thiết kế lại ít gặp hơn và có quy mô lớn hơn, nên cần thử nghiệm trước khi triển khai rộng. Hướng dẫn triển khai doanh nghiệp của Anthropic chia giai đoạn áp dụng theo cách này: một nhóm thử nghiệm được theo dõi phản hồi trong nhiều tuần trước khi mở rộng, đồng thời xác định người thúc đẩy áp dụng trong từng nhóm. Tiệm giặt khô thử thư theo từng cấp trên một đợt khách trước. Triển khai đồng loạt không đo lường được gì, không còn nhóm đối chiếu và đặt mọi thứ vào rủi ro cùng lúc.

## Điểm kiểm soát của con người

Tìm bước ra quyết định và giữ con người ở bước đó. Tích hợp thất bại khi bước kiểm tra bị bỏ. Kiểm tra không tạo đầu ra hữu hình nên trông như lãng phí với người thiết kế lại chỉ dựa trên sơ đồ. Người quản lý tiệm giặt khô ký duyệt từng thư trước khi gửi. Điểm kiểm soát cũng khiến việc bổ trợ có thể được áp dụng nhanh một cách an toàn. Người vốn ký duyệt thư vẫn tiếp tục ký duyệt, nên phán đoán chưa từng rời khỏi quy trình.

## Ranh giới của vai trò Associate

Một số yêu cầu vượt khỏi vai trò này vì cần triển khai kỹ thuật: các hệ thống trao đổi với nhau, dữ liệu tự di chuyển hoặc quy trình được xây để chạy không cần người hiện diện. Giả sử chủ tiệm muốn thư nhắc được gửi qua đêm, trực tiếp từ hệ thống bán hàng tại quầy. Điều đó cần kết nối hệ thống bán hàng với công cụ gửi thư và là công việc kỹ thuật. Cách làm chuyên nghiệp là chuyển cho Claude Developer hoặc Architect kèm mô tả rõ bằng văn bản về nhu cầu quy trình. Mô tả tốt nhu cầu chính là đóng góp của Associate. Chuyển xử lý không phải thất bại mà là hiểu phạm vi công việc của mình.

**Trình kết nối (connectors)** cho phép Claude lấy dữ liệu và thực hiện hành động trong các dịch vụ đã kết nối. Chúng hoạt động trong cuộc trò chuyện khi yêu cầu của con người cần đến chúng. Tài liệu Google Workspace nêu Claude chỉ truy cập dữ liệu khi bạn hỏi rõ một câu hoặc yêu cầu hành động cần dữ liệu đó. Trong những tính năng bài thi bao quát, như chat, Project, Research, artifact và connector, công việc được thực hiện khi con người yêu cầu.

**Trạng thái trong bản gốc, kiểm tra ngày 14 tháng 10 năm 2026:** Claude Cowork, không được hướng dẫn thi nêu tên, có tác vụ theo lịch. Khóa học Cowork của Anthropic cho biết tác vụ chỉ dùng các connector của bạn có thể chạy từ xa vào thời gian đã đặt. Trong bài thi, yêu cầu công việc tự chạy vẫn được chuyển xử lý vì bài thi xem đó là triển khai kỹ thuật vượt vai trò này.

## Nơi lưu công việc lặp lại

Công việc lặp lại nên nằm trong Project thay vì một cuộc trò chuyện kéo dài mãi. Project là không gian làm việc độc lập có lịch sử chat và kiến thức riêng. Khi chat tiến gần giới hạn độ dài, Trung tâm trợ giúp khuyên mở chat mới hoặc dùng Project. Việc tổng hợp thứ Hai được đưa vào đó. Với gói hỗ trợ chia sẻ, Project cho nhóm một môi trường chung chứa tài liệu và chỉ dẫn. Chat trong Project không được chia sẻ mặc định. Thành viên nhìn thấy nội dung, kiến thức và chỉ dẫn của Project. Cuộc trò chuyện riêng của mỗi người vẫn riêng tư trừ khi họ chọn chia sẻ. Quyết định công việc nên nằm trong Project thuộc mục tiêu này. Cấu hình Project và duy trì chỉ dẫn, kiến thức thuộc Lĩnh vực 5.

## Trong bài thi

Hiểu đúng nghĩa tích hợp giúp trả lời nhiều câu hỏi. Phương án gây nhiễu thường là tích hợp theo nghĩa kỹ thuật. Đáp án đúng là tích hợp theo nghĩa của bài học này. Hãy nhận biết các từ trong phần dẫn báo hiệu triển khai kỹ thuật và cần chuyển xử lý: “tự động”, “không cần ai”, “trực tiếp từ hệ thống”, “qua đêm”.

### Bước nhảy sang tự động hóa

Kết nối Claude trực tiếp vào hệ thống hoặc thiết lập để chạy không có người giám sát là phương án gây nhiễu điển hình của lĩnh vực này và không phải đáp án đúng. Chuyển xử lý vì yêu cầu là triển khai kỹ thuật, vượt phạm vi vai trò và những tính năng bài thi bao quát. Không được giải thích việc chuyển xử lý bằng khẳng định rằng không sản phẩm Claude nào có thể thực hiện công việc ấy. Tác vụ theo lịch của Cowork, không được hướng dẫn thi nêu tên, có thể chạy một số việc vào thời gian định sẵn.

## Những bẫy thường gặp trong bài thi

### Tự ứng biến giải pháp tự động hóa thay vì chuyển xử lý

Kết nối các hệ thống, tự động xuất bản và luồng xử lý chạy không có người giám sát là triển khai kỹ thuật, vượt vai trò Associate và các tính năng bài thi bao quát. Phiên bản tự chế có thể lỗi âm thầm khi không ai ở đó để phát hiện. Cách làm chuyên nghiệp là bản giao việc chuyển xử lý rõ ràng cho Claude Developer hoặc Architect.

### Thiết kế lại toàn bộ quy trình cùng lúc

Triển khai ôm đồm khiến nếu thất bại thì mọi thứ thất bại cùng nhau và không học được điều gì. Thiết kế lại cần thử nghiệm trước trên một phần, có đo lường, đúng như cách hướng dẫn triển khai của Anthropic chia giai đoạn áp dụng.

### Tối ưu đến mức loại bỏ bước kiểm tra

Điểm kiểm soát của con người không tạo đầu ra hữu hình, nên có vẻ lãng phí trên sơ đồ. Đây lại là nơi chứa phán đoán của quy trình. Bỏ nó đi, lỗi đầu tiên không được phát hiện sẽ quyết định danh tiếng của việc tích hợp.

## Tình huống luyện tập

Trợ lý biên tập của một tờ báo địa phương tổng hợp trang sự kiện hằng tuần từ thông tin các địa điểm gửi qua email. Đồng nghiệp đề xuất để Claude tự thu thập danh sách từ website của các địa điểm qua đêm và xuất bản trang hoàn chỉnh mà không ai cần can thiệp. Trợ lý vẫn muốn tiết kiệm thời gian cho trang tuần này, có người đọc mọi mục trước khi đăng. Nên phản hồi thế nào?

**Phương án A**

Đồng ý và dành cả tuần thử các connector đến khi Claude có thể thu thập danh sách từ các địa điểm và tạo trang mỗi đêm không cần ai tham gia.

**Phương án B**

Từ chối mọi việc dùng Claude cho trang, vì một mục sai ngày hoặc giờ sẽ làm giảm uy tín tờ báo với độc giả và các địa điểm.

**Phương án C**

Chuyển phương án chạy qua đêm cho nhóm kỹ thuật kèm ghi chú về nhu cầu quy trình; trong lúc đó dùng Claude định dạng lại các nội dung gửi qua email để con người kiểm tra.

**Phương án D**

Thiết kế lại toàn bộ hoạt động danh sách sự kiện một lần: bản in, web và mạng xã hội đều từ cùng tài liệu gửi đến và ra mắt đồng thời.

## Bài tập thực hành: Lập sơ đồ một quy trình bạn phụ trách

**Thời gian:** 45 phút.

### Bạn sẽ học được

- Cách phân loại từng bước: bổ trợ, thiết kế lại, chuyển xử lý hoặc chỉ con người.
- Cách viết bản giao việc chuyển xử lý dùng được cho Developer hoặc Architect.
- Cách chọn phần bổ trợ có tỷ lệ thời gian tiết kiệm so với rủi ro tốt nhất.
- Cách đo lường việc tích hợp trung thực trong hai tuần.

### Bước 1 — Chọn quy trình lặp lại và viết các bước từ đầu đến cuối

Chọn quy trình bạn có thể mô tả cho đồng nghiệp mới trong năm phút.

**Vì sao:** Quyết định tích hợp được đưa ra theo từng bước. Không liệt kê được các bước thì không thể chủ động tích hợp.

**Kết quả cần thấy:** Danh sách đánh số từ yếu tố khởi động đến đầu ra hoàn tất, bao gồm các bước không chính thức.

### Bước 2 — Gắn một nhãn cho mỗi bước

- **Bổ trợ:** Con người đưa bước này đến Claude ngay hôm nay.
- **Thiết kế lại:** Bước này tồn tại vì trước đây có công việc tốn kém.
- **Chuyển xử lý:** Cần triển khai kỹ thuật, như các hệ thống trao đổi hoặc quy trình chạy không có người hiện diện.
- **Chỉ con người:** Đây là nơi ra quyết định.

**Vì sao:** Bốn nhãn là toàn bộ khung quyết định của mục tiêu được áp dụng vào việc thật.

**Kết quả cần thấy:** Mỗi bước có đúng một nhãn.

### Bước 3 — Viết bản giao việc hai câu cho từng bước cần chuyển xử lý

Viết điều bạn sẽ giao cho Claude Developer: quy trình cần gì và phần nào phải giữ con người.

**Vì sao:** Mô tả rõ nhu cầu là đóng góp của Associate cho công việc vượt bộ công cụ của mình. Viết ra giúp kiểm tra bạn có hiểu quy trình không.

**Kết quả cần thấy:** Mỗi bước cần chuyển xử lý có bản giao việc mà Developer có thể dựa vào hành động mà không cần họp.

### Bước 4 — Chọn một phần bổ trợ tốt nhất và chạy trong hai tuần

Chọn phần có tỷ lệ thời gian tiết kiệm so với rủi ro tốt nhất, giữ nguyên điểm kiểm soát con người tại vị trí cũ.

**Vì sao:** Làm tốt hơn một bước và đo lường là cách tích hợp thành công. Kỷ luật thử nghiệm vẫn áp dụng ngay cả ở quy mô này.

**Kết quả cần thấy:** Hai tuần quy trình vận hành với một bước được bổ trợ, các phần khác không đổi.

### Bước 5 — Đo lường trung thực và ghi nhận khả năng thiết kế lại

Ghi trước, sau và cách bạn biết. Nêu những điểm cần xem xét thiết kế lại khi bước đó giờ đã ít tốn công.

**Vì sao:** Đo lường trung thực làm đầu vào cho mục tiêu 4.5; bước ít tốn công có thể đã loại bỏ ràng buộc từng định hình quy trình.

**Kết quả cần thấy:** Bản ghi ba dòng: trước, sau, bằng chứng; kèm phương án thiết kế lại đáng thử nghiệm nếu có.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Project là gì? — *What are projects?*
- Quản lý khả năng hiển thị và chia sẻ Project — *Manage project visibility and sharing*.
- Dùng connector để mở rộng khả năng của Claude — *Use connectors to extend Claude's capabilities*.
- Sử dụng connector Google Workspace — *Use Google Workspace connectors*.
- Hạn mức sử dụng và giới hạn độ dài hoạt động như thế nào? — *How do usage and length limits work?*
- Hướng dẫn quản trị Claude Enterprise — *Claude Enterprise Administrator Guide*.
- Giới thiệu Claude Cowork: Claude Cowork có thể làm gì cho bạn — *Introduction to Claude Cowork: What Claude Cowork can do for you*.
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

**Ghi chú của tác giả bài gốc về Cowork:** Chỉ dùng cho ghi chú tình trạng hiện tại; hướng dẫn thi không nêu Cowork.

**Ghi chú của tác giả bài gốc về hướng dẫn thi:** Các nhận định về thực hành nghề nghiệp là phán đoán của tác giả, không phải hướng dẫn của Anthropic.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [4.3 — Hỗ trợ thiết kế, phát triển và tinh chỉnh giải pháp](4-3-solution-design-iteration.vi.md).
- **Bài tiếp theo:** [4.5 — Truyền đạt giá trị và giới hạn cho các bên liên quan](4-5-communicating-value-limitations.vi.md).
