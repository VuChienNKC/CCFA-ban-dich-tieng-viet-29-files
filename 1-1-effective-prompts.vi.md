# 1.1 — Tạo prompt hiệu quả cho công việc nghiệp vụ và kỹ thuật

- **Lĩnh vực (Domain):** 1
- **Nhiệm vụ (Task):** 1.1
- **Tên bài gốc:** Creating Effective Prompts for Business and Technical Tasks
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/1-prompting-task-execution/1-1-effective-prompts)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Prompt là bản giao việc bạn cung cấp cho Claude: nhiệm vụ cùng mọi thông tin cần thiết để thực hiện nhiệm vụ đó. Viết bản giao việc tốt không phải là một kỹ năng kỹ thuật; đó chính là kỹ năng bạn dùng khi giao việc cho đồng nghiệp. Mọi mục tiêu khác trong chương trình chứng nhận này đều được xây dựng trên nền tảng đó. Một bản giao việc tốt cung cấp đầu vào để sáu lĩnh vực còn lại phát huy tác dụng. Không có tính năng, lựa chọn mô hình hay bước khắc phục sự cố nào có thể cứu được một bản giao việc kém.

Người quản lý văn phòng của một công ty thi công mái nhà muốn Claude soạn bản cập nhật dài một trang về các công việc trong tháng này cho hai giám đốc. Phiên bản yêu cầu chỉ có một dòng là: “Viết gì đó về các công việc trong tháng này.”

## Tư duy giao việc

Anthropic hướng dẫn bạn xem Claude như một nhân viên mới rất giỏi: có năng lực cao, nhưng chưa biết gì về công ty, dự án hay tiêu chuẩn của bạn cho đến khi bạn cung cấp thông tin. Trung tâm trợ giúp cũng đưa ra hình ảnh tương tự cho người dùng trò chuyện: một cộng tác viên vừa được thuê, cần những chỉ dẫn thật cụ thể. Khi một prompt không hiệu quả, trung tâm trợ giúp khuyên bạn diễn giải lại yêu cầu như thể đang nói với người hoàn toàn không có kiến thức nền về điều bạn muốn nhờ họ làm.

Một prompt hiệu quả chứa càng nhiều bối cảnh càng tốt, vì Claude làm việc dựa trên những gì được cung cấp. Giống như khi giao việc tốt, prompt cần bao quát nhiệm vụ, thông tin nền, đối tượng tiếp nhận, định dạng và tiêu chí của một kết quả tốt. Cả nhân viên mới ở công ty thi công mái nhà lẫn Claude đều không tự biết công việc nào đã bị chậm tiến độ.

## Năm thành phần

Một prompt nghiệp vụ đầy đủ có năm thành phần.

### 1. Nhiệm vụ (Task)

Nêu chính xác điều bạn muốn thực hiện, bằng một động từ và một sản phẩm đầu ra. “Soạn bản cập nhật dự án dài một trang cho ban chỉ đạo” là một nhiệm vụ. “Giúp tôi với dự án của tôi” thì chưa phải. Nhiệm vụ của người quản lý văn phòng là tạo bản cập nhật dài một trang về các công việc trong tháng này cho các giám đốc.

### 2. Bối cảnh (Context)

Đây là những thông tin nền Claude không thể tự biết: người đọc là ai, tài liệu dùng để làm gì, những gì đã được quyết định và các ràng buộc cần tuân thủ. Với nhiệm vụ viết, prompt cần nêu yêu cầu, đối tượng đọc và các ý chính.

### 3. Tài liệu nguồn (Source material)

Dán hoặc đính kèm đầu vào thực tế, chẳng hạn báo cáo, ghi chép cuộc họp hoặc dữ liệu. Đừng mô tả lại chúng theo trí nhớ. Claude làm việc từ những gì được cung cấp; một bản tóm tắt theo trí nhớ sẽ đưa thêm sai sót và thiếu sót vốn không có trong tài liệu thật. claude.ai chấp nhận tài liệu, bảng tính và hình ảnh, nên bạn có thể cung cấp trực tiếp đầu vào thực tế. Công ty thi công mái nhà đính kèm các phiếu công việc thay vì kể lại theo trí nhớ.

### 4. Đặc tả đầu ra (Output specification)

Nêu định dạng, độ dài, giọng văn và cấu trúc. Ví dụ: mỗi nhóm công việc có ba ý gạch đầu dòng, giọng văn trung lập, dưới 400 từ.

### 5. Ví dụ mẫu, khi cần tuân thủ tiêu chuẩn

Một tài liệu trước đây theo đúng văn phong của tổ chức hữu ích hơn ba đoạn văn mô tả văn phong ấy. Anthropic xem ví dụ là một trong những cách đáng tin cậy nhất để định hướng định dạng, giọng văn và cấu trúc. Với công ty thi công mái nhà, bản cập nhật của tháng trước chính là tài liệu mẫu.

## Xác định vai trò và đối tượng đọc

Mở đầu prompt bằng một vai trò, chẳng hạn “Trong vai một chuyên viên truyền thông nhân sự”, sẽ định hướng từ vựng, giọng văn và các ưu tiên. Anthropic lưu ý rằng ngay cả một câu xác định vai trò cũng tạo ra khác biệt.

Việc nêu rõ đối tượng đọc làm thay đổi đầu ra nhiều hơn phần lớn những chỉnh sửa nhỏ trong chỉ dẫn. Cùng một nội dung phân tích cần được trình bày khác nhau cho hội đồng quản trị và cho nhóm dự án. Claude sẽ điều chỉnh nếu biết ai sẽ đọc, vì vậy bản giao việc của công ty thi công mái nhà nêu rõ người đọc là các giám đốc. Giải thích lý do đằng sau một yêu cầu cũng giúp nhận được câu trả lời sát mục tiêu hơn.

## Sự cụ thể mang lại điều gì?

Prompt mơ hồ tạo ra đầu ra chung chung và cần sửa lại nhiều. Nêu cụ thể định dạng đầu ra mong muốn cùng các ràng buộc giúp Claude tạo kết quả tốt hơn. Dành một phút cho bản giao việc có thể tiết kiệm một vòng làm lại. Hướng dẫn sử dụng chính thức cũng đồng ý: hãy cụ thể, ngắn gọn, đồng thời rà soát và chỉnh sửa prompt trước khi gửi. Lần thực hiện đầu tiên với một bản giao việc tốt tốn ít thời gian và hạn mức sử dụng hơn việc sửa đi sửa lại. Yêu cầu một dòng của công ty thi công mái nhà không cung cấp phiếu công việc, người đọc hay định dạng.

## Công việc kỹ thuật ở cấp độ Associate

“Kỹ thuật” không đồng nghĩa với viết mã. Ở cấp độ này, đó có thể là nhờ Claude viết công thức bảng tính, thực hiện lượt phân tích dữ liệu đơn giản ban đầu hoặc soạn bản nháp tài liệu kỹ thuật. Kỹ năng vẫn như nhau: giao việc rõ ràng. Người quản lý văn phòng có thể viết: “Tôi cần một công thức đánh dấu mọi hóa đơn quá hạn thanh toán trên 30 ngày; đây là mẫu dữ liệu.”

## Trong bài thi

Đáp án sai thường lặp lại ở mục tiêu này là prompt một dòng như “Viết gì đó về kết quả quý III của chúng tôi”, được xem là chấp nhận được vì Claude sẽ tự hiểu phải làm gì. Claude không thể làm vậy: không có thành phần nào trong năm thành phần được cung cấp đủ để dựa vào. Bản giao việc về công thức ở trên đã đáp ứng phần việc của Lĩnh vực 1; độ tinh tế của công thức không phải điều câu hỏi đang kiểm tra.

### Khái niệm cốt lõi

Khi câu hỏi thi so sánh các prompt, hãy đếm các thành phần. Đáp án đúng gần như luôn bổ sung nhiệm vụ, bối cảnh, tài liệu nguồn, đặc tả đầu ra hoặc ví dụ còn thiếu. Các phương án gây nhiễu chỉ trau chuốt câu chữ và để nguyên chỗ thiếu.

## Những bẫy thường gặp trong bài thi

### Chấp nhận prompt một dòng vì cho rằng Claude sẽ tự hiểu

Claude không có những thông tin bối cảnh mà ngay cả một đồng nghiệp cũng cần. Vì vậy, đầu ra sẽ chung chung và người dùng phải trả giá cho phần giao việc bị bỏ qua bằng công sức làm lại. Đáp án đúng giao việc đầy đủ; nêu cụ thể ngay từ đầu là cách khắc phục đã được tài liệu hướng dẫn ghi nhận.

### Chọn phương án trau chuốt câu chữ nhưng vẫn bỏ trống thông tin thực sự còn thiếu

Phần dẫn của câu hỏi ở mục tiêu này thường chỉ ra một thành phần còn thiếu: không có đối tượng đọc, tài liệu nguồn hoặc định dạng. Chỉnh sửa chỉ dẫn mang tính hình thức không lấp được chỗ thiếu đó. Chính vì vậy, đây là phương án gần đúng hấp dẫn nhưng không phải đáp án đúng.

### Tự viết toàn bộ sản phẩm rồi chỉ dùng Claude để soát lỗi

Cách này có vẻ cẩn thận nhưng chưa tận dụng hết công cụ. Soạn bản nháp từ một bản giao việc tốt chính là công việc Claude làm tốt. Chỉ dùng để soát lỗi đồng nghĩa với bỏ lỡ lợi ích tiết kiệm thời gian; bài thi xem đây là cách dùng công cụ hời hợt, chưa khai thác hết khả năng.

## Tình huống luyện tập

Một điều phối viên phụ trách cơ sở vật chất cần Claude soạn thông báo nội bộ giới thiệu hệ thống đặt chỗ bàn làm việc mới cho toàn bộ nhân viên làm việc tại văn phòng. Cô có hướng dẫn sử dụng của nhà cung cấp và muốn có bản nháp có thể gửi đi mà không phải tự sửa lại hoặc yêu cầu Claude chỉnh thêm nhiều vòng. Prompt nào chuẩn bị cho công việc tốt nhất?

**Phương án A**

Trước tiên yêu cầu Claude mô tả cách các hệ thống đặt chỗ bàn làm việc thường hoạt động, rồi để Claude soạn thông báo theo định dạng mà nó thấy phù hợp nhất. Chỉ cung cấp hướng dẫn sử dụng, đối tượng đọc và sở thích về giọng văn trong các lượt trao đổi sau nếu bản nháp đầu tiên bỏ sót những điều này.

**Phương án B**

Gửi một dòng yêu cầu viết thông báo về hệ thống đặt chỗ bàn làm việc, giữ yêu cầu ngắn để Claude có không gian sáng tạo, rồi dự định chọn những phần tốt nhất từ nội dung nhận được.

**Phương án C**

Đính kèm hướng dẫn sử dụng dài một trang, nêu rõ đối tượng đọc là toàn bộ nhân viên làm việc tại văn phòng, xác định mục tiêu là giảm sự bối rối trong tuần đầu tiên và yêu cầu giọng văn thân thiện nhưng dứt khoát, dài 300 từ, có phần tóm tắt ba ý gạch đầu dòng ở đầu.

**Phương án D**

Tự viết thông báo từ hướng dẫn sử dụng và chỉ nhờ Claude kiểm tra chính tả, ngữ pháp, giọng văn của văn bản hoàn chỉnh trước khi gửi cho nhân viên.

## Bài tập thực hành: Viết bản giao việc gồm năm thành phần

**Thời gian:** 20 phút.

### Bạn sẽ học được

- Cách diễn đạt nhiệm vụ bằng một động từ và một sản phẩm đầu ra.
- Cách cung cấp bối cảnh Claude không thể tự biết.
- Cách đính kèm tài liệu nguồn thực tế thay vì mô tả lại.
- Cách quy định định dạng, độ dài, giọng văn và cấu trúc.
- Cách dùng một tài liệu mẫu để xác lập tiêu chuẩn.

### Bước 1 — Chọn một công việc thực tế lặp lại trong công việc của bạn

Chẳng hạn một báo cáo, bản thông tin tóm lược hoặc email bạn tạo hằng tuần.

**Vì sao:** Với công việc bạn hiểu rõ, những chỗ thiếu trong bản giao việc sẽ dễ nhận ra. Bạn có thể biết ngay khi đầu ra chưa đạt tiêu chuẩn của mình.

**Kết quả cần thấy:** Một dòng nêu nhiệm vụ, sản phẩm đầu ra và tần suất thực hiện.

### Bước 2 — Viết câu giao việc và bổ sung bối cảnh

Viết câu giao việc bằng một động từ và một sản phẩm đầu ra. Sau đó thêm bối cảnh Claude không thể tự biết: người đọc, mục đích, những gì đã quyết định và các ràng buộc.

**Vì sao:** Câu giao việc và bối cảnh là hai thành phần thường thiếu nhất trong prompt yếu, đồng thời cũng là hai thành phần dễ bổ sung nhất.

**Kết quả cần thấy:** Một câu giao việc cùng ba hoặc bốn dòng bối cảnh mà một đồng nghiệp mới sẽ cần trong ngày đầu tiên.

### Bước 3 — Đính kèm hoặc dán tài liệu nguồn thực tế

Dùng báo cáo, ghi chép hoặc dữ liệu thật, thay vì bản tóm tắt chúng theo trí nhớ.

**Vì sao:** Claude làm việc dựa trên những gì được cung cấp. Mô tả theo trí nhớ đưa thêm sai sót và thiếu sót vốn không có trong tài liệu thật.

**Kết quả cần thấy:** Các tệp thật hoặc nội dung được dán nằm trong cuộc trò chuyện cùng với bản giao việc.

### Bước 4 — Đặc tả đầu ra và đính kèm một tài liệu mẫu

Nêu định dạng, độ dài, giọng văn, cấu trúc và đính kèm một tài liệu trước đây theo đúng văn phong của tổ chức.

**Vì sao:** Ví dụ là một trong những cách đáng tin cậy nhất để định hướng định dạng, giọng văn và cấu trúc. Một mẫu hữu ích hơn nhiều đoạn mô tả.

**Kết quả cần thấy:** Đặc tả đầu ra dài một hoặc hai dòng cùng một tài liệu mẫu đính kèm.

### Bước 5 — Chạy prompt và so sánh bản nháp

So sánh bản nháp với lần viết đầu tiên thông thường của bạn, đồng thời ghi nhận thành phần nào đã mang lại giá trị.

**Vì sao:** Việc so sánh cho thấy từng phần trong bản giao việc mang lại điều gì, từ đó giúp bạn hình thành thói quen giao việc tốt.

**Kết quả cần thấy:** Một bản nháp đầu tiên gần với mức có thể phát hành hơn rõ rệt so với kết quả từ prompt một dòng.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Bắt đầu sử dụng Claude — *Get started with Claude*.
- Giới thiệu về thiết kế prompt — *Introduction to prompt design*.
- Prompt của tôi không tạo ra câu trả lời hữu ích — *My prompt isn't giving me a helpful answer*.
- Các phương pháp tốt nhất khi viết prompt — *Prompting best practices*.
- Tải tệp lên Claude — *Upload files to Claude*.
- Các phương pháp sử dụng hạn mức hiệu quả — *Usage limit best practices*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài tiếp theo:** [1.2 — Chia nhỏ yêu cầu phức tạp](1-2-task-decomposition.vi.md).
