# 3.1 — Lựa chọn tính năng Claude phù hợp

- **Lĩnh vực (Domain):** 3
- **Nhiệm vụ (Task):** 3.1
- **Tên bài gốc:** Selecting the Right Claude Product Feature
- **Nguồn:** [Bài học gốc](https://claudecertificationguide.com/ccao-f/learn/3-product-model-selection/3-1-product-feature-selection)

*Học nội dung này qua hình thức tương tác.*

## Những điều bạn cần biết

Claude cung cấp bốn cách xử lý công việc. **Trò chuyện thông thường (ordinary chat)** là một cuộc trò chuyện riêng lẻ. Trung tâm trợ giúp mô tả **Project** là không gian làm việc độc lập với lịch sử trò chuyện và kho kiến thức riêng. **Research** dành cho câu hỏi cần tổng hợp câu trả lời từ nhiều nguồn bên ngoài và trả về báo cáo có trích dẫn. **Artifact** là nội dung độc lập hiển thị trong cửa sổ riêng bên cạnh cuộc trò chuyện. Phần lớn mọi người chọn tính năng theo thói quen. Thay vào đó, hãy nhận diện đặc điểm nhiệm vụ trước khi viết bất kỳ prompt nào.

Chủ một tiệm làm tóc có bốn việc. Cô cần một thư trả lời khiếu nại của khách. Mỗi tuần, cô viết thông báo nhắc lịch hẹn từ cùng bảng giá và văn phong của tiệm. Cô muốn biết các tiệm khác xử lý khoản đặt cọc khi khách không đến như thế nào, có nguồn để người cùng kinh doanh kiểm tra. Mỗi quý, cô chỉnh sửa một tờ hướng dẫn chăm sóc sau dịch vụ cho các thợ làm tóc. Bốn câu hỏi giúp phân loại: công việc làm một lần hay lặp lại? Nó độc lập hay liên tục cần cùng một bối cảnh dùng thường xuyên? Nó được dùng một lần hay sẽ chỉnh sửa và tái sử dụng? Claude có thể trả lời từ những gì bạn cung cấp hay phải thu thập câu trả lời từ nguồn bên ngoài? Mỗi tính năng phục vụ một dạng công việc.

## Trò chuyện thông thường là lựa chọn mặc định

Một câu hỏi riêng lẻ, một bản nháp hoặc phân tích tài liệu được đính kèm ngay lúc đó không cần không gian làm việc riêng, tìm kiếm theo cơ chế tác tử hay hình thức nội dung độc lập. Trò chuyện thông thường xử lý ngay được và thường là lựa chọn phù hợp hơn mức những người đam mê tính năng nâng cao thừa nhận. Thư trả lời khiếu nại thuộc dạng này.

## Project: Bối cảnh dùng chung cho công việc lặp lại

Một Project lưu giữ hai loại tài nguyên dùng thường xuyên. **Chỉ dẫn (instructions)** định hướng câu trả lời của Claude trong mọi cuộc trò chuyện bên trong không gian làm việc. **Kho kiến thức (knowledge base)** chứa tài liệu đã tải lên mà Claude dùng làm thông tin nền cho các cuộc trò chuyện đó. Chỉ thiết lập một lần, cả hai áp dụng cho mọi cuộc trò chuyện trong Project. Dấu hiệu nhận biết là cùng tài liệu nền, sở thích cố định và tài liệu làm việc được cần đến qua nhiều cuộc trò chuyện. Dán lại cùng bối cảnh từ chat này sang chat khác là làm thủ công công việc vốn phù hợp với Project. Tính năng này tồn tại để chấm dứt cách làm vòng ấy. Project sẽ chứa bảng giá và văn phong mà chủ tiệm dán lại mỗi tuần.

## Research: Tổng hợp đa nguồn có trích dẫn

Trong Research, Claude hoạt động theo cơ chế tác tử (agent), thực hiện nhiều lượt tìm kiếm nối tiếp, mỗi lượt dựa vào kết quả trước. Báo cáo tổng hợp có trích dẫn để người đọc kiểm tra các phát hiện. Các dấu hiệu gồm: khảo sát toàn cảnh một lĩnh vực, tìm hiểu cách các đơn vị khác làm việc, tổng quan tình hình hiện tại và đối tượng đọc muốn biết các phát hiện đến từ đâu. Câu hỏi về khoản đặt cọc phù hợp với Research. Research không phải cách nâng cấp chất lượng cho mọi câu hỏi thông thường. Nhiệm vụ có thể trả lời từ tài liệu bạn đã có không được lợi gì từ nó, vì không có gì cần thu thập thêm.

## Artifact: Sản phẩm có vòng đời riêng

Claude tạo artifact khi đầu ra quan trọng, độc lập, hoàn chỉnh và có khả năng được biên tập, tinh chỉnh hoặc tái sử dụng ngoài cuộc trò chuyện. Điều kiện cuối là dấu hiệu chủ đạo: sản phẩm còn được sử dụng sau cuộc trò chuyện đã tạo ra nó. Ví dụ gồm tờ tài liệu tham khảo được sửa mỗi quý hoặc kế hoạch được chia sẻ và cập nhật. Mỗi sản phẩm nên tồn tại như một phiên bản thống nhất phát triển qua các lần sửa, thay vì những mảnh nội dung rải rác trong lịch sử trò chuyện. Bạn tinh chỉnh artifact bằng cách yêu cầu Claude thay đổi hoặc sửa một tin nhắn trước đó để phân nhánh chat với các artifact riêng. Bạn có thể quay lại artifact và chia sẻ bản đã hoàn thiện. Tờ hướng dẫn chăm sóc sau dịch vụ phù hợp với dạng này.

## Một dấu hiệu chủ đạo

Công việc thực tế có thể kết hợp các tính năng. Project có thể chứa các cuộc trò chuyện tạo artifact. Báo cáo Research có thể làm nền cho tài liệu tồn tại dưới dạng artifact và được chỉnh mỗi quý. Báo cáo của tiệm về khoản đặt cọc có thể làm cơ sở cho một chính sách đặt cọc được lưu dưới dạng artifact.

## Trong bài thi

Mục tiêu này kiểm tra việc chọn tính năng bằng cách đọc đặc điểm nhiệm vụ. Bài thi không kiểm tra các cách kết hợp. Mỗi câu đưa ra một công việc với một dấu hiệu chủ đạo: bối cảnh lặp lại, trích dẫn đa nguồn, sản phẩm cần chỉnh sửa qua nhiều vòng hoặc công việc đơn giản làm một lần. Đáp án sai luôn là tính năng có thật nhưng dùng cho sai dạng việc. Trò chuyện thông thường cần được nhìn nhận đúng, vì bài thi cũng coi đó là lựa chọn hợp lệ. Khi dấu hiệu chủ đạo trong phần dẫn là công việc đơn giản làm một lần, trò chuyện thông thường là đáp án chuyên nghiệp, dù các tính năng khác mạnh đến đâu. Bài thi sẵn sàng chọn phương án đơn giản nhất làm đáp án đúng.

Viết chỉ dẫn của Project và chọn lọc kho kiến thức thuộc Lĩnh vực 5; ở đây, kỹ năng được kiểm tra là nhận ra tính lặp lại. Kiểm tra trích dẫn của báo cáo Research là kỹ năng thuộc Lĩnh vực 2. Chọn giữa câu trả lời trực tiếp trong chat, bảng và tài liệu là câu hỏi về định dạng của Lĩnh vực 2. Trong mục tiêu này, artifact là nơi phù hợp cho sản phẩm cần tinh chỉnh và tái sử dụng.

### Khái niệm cốt lõi

Tìm dấu hiệu chủ đạo trước rồi ghép tính năng. Bối cảnh dùng chung lặp lại hướng đến Project; câu trả lời tổng hợp đa nguồn có trích dẫn hướng đến Research; sản phẩm có vòng đời riêng hướng đến artifact; công việc độc lập làm một lần hướng đến trò chuyện thông thường.

## Những bẫy thường gặp trong bài thi

### Đề xuất Research cho câu hỏi có thể trả lời từ tài liệu người dùng đã có

Research dành cho câu trả lời cần được thu thập từ nhiều nguồn bên ngoài. Khi phần dẫn đã cung cấp tài liệu, tìm kiếm theo cơ chế tác tử là bước vòng do chọn sai công cụ. Trò chuyện thông thường với tài liệu đính kèm là đáp án chuyên nghiệp.

### Đưa mọi thứ vào Project hoặc Research để tối đa hóa chất lượng

Tính năng cần tổ chức nhiều nhất không phải tính năng an toàn nhất. Công việc đơn giản làm một lần không được lợi gì từ không gian làm việc riêng hoặc báo cáo đa nguồn, và trò chuyện thông thường là một đáp án đúng hợp lệ ở mục tiêu này. Dấu hiệu chủ đạo quyết định, không phải mức độ cao cấp của tính năng.

### Xem việc dán lại cùng bối cảnh vào mọi chat là sự cẩn thận

Cách làm vòng thủ công khiến bạn phải trả chi phí thiết lập Project mỗi lần thay vì chỉ một lần. Khi phần dẫn mô tả cùng tài liệu và sở thích được cung cấp lặp đi lặp lại qua nhiều chat, đáp án đúng chuyển công việc đó vào Project.

## Tình huống luyện tập

Thư ký một hội đồng địa phương có bốn công việc: chu trình lập chương trình họp và biên bản hằng tháng luôn cần quy chế làm việc, danh sách thành viên và quy ước định dạng của hội đồng; một báo cáo làm một lần về cách năm hội đồng lân cận quản lý danh sách chờ thuê đất làm vườn, có nguồn để các thành viên hội đồng kiểm tra; một câu hỏi riêng lẻ của cư dân về hạn chót xin trợ cấp; và danh sách liên hệ khẩn cấp được cập nhật mỗi quý, chia sẻ với mọi thành viên. Cô muốn mỗi việc chỉ dùng tính năng vừa đủ, không tạo Project cho việc không lặp lại và không phải cung cấp lại thông tin bằng tay. Kế hoạch nào ghép đúng tính năng với công việc?

**Phương án A**

Tạo một Project chứa cả bốn công việc, vì giữ mọi nhiệm vụ của hội đồng trong một không gian làm việc đơn giản hơn việc quyết định tính năng riêng cho từng việc khi phát sinh.

**Phương án B**

Dùng Research cho cả báo cáo về đất làm vườn và câu hỏi hạn chót xin trợ cấp; xuất mọi đầu ra thành artifact có thể chia sẻ để cả bốn công việc đều có cùng mức độ chặt chẽ tối đa.

**Phương án C**

Dùng Project cho chu trình chương trình họp và biên bản hằng tháng, Research cho báo cáo về năm hội đồng, trò chuyện thông thường cho câu hỏi hạn chót xin trợ cấp và tạo, cập nhật danh sách liên hệ dưới dạng artifact.

**Phương án D**

Làm mọi thứ trong trò chuyện thông thường, dán quy chế làm việc và danh sách thành viên vào mỗi tháng, đồng thời dựng lại danh sách liên hệ từ cuộc trò chuyện cũ mỗi quý.

## Bài tập thực hành: Rà soát cách bạn chọn tính năng

**Thời gian:** 20 phút.

### Bạn sẽ học được

- Cách nhận diện đặc điểm nhiệm vụ trước khi chọn tính năng.
- Cách gọi tên dấu hiệu chủ đạo quyết định từng tính năng.
- Cách phát hiện cách làm vòng thủ công trong thói quen làm việc của mình.
- Cách quyết định khi nào công việc lặp lại nên có Project.

### Bước 1 — Liệt kê năm cuộc trò chuyện Claude gần nhất trong công việc

Dùng chính những cuộc trò chuyện thực tế của bạn.

**Vì sao:** Cuộc trò chuyện thật làm lộ thói quen thật. Danh sách dựng lên dễ khiến bài tập trông tốt hơn thực tế.

**Kết quả cần thấy:** Năm mô tả dài một dòng về các nhiệm vụ thực tế bạn đã thực hiện gần đây.

### Bước 2 — Gắn nhãn tính năng lẽ ra nên dùng

Với mỗi nhiệm vụ, chọn trò chuyện thông thường, chat trong Project, Research hoặc artifact cho đầu ra.

**Vì sao:** Gắn nhãn buộc bạn thực hiện quyết định lựa chọn mà mục tiêu này kiểm tra, lần lượt từng nhiệm vụ.

**Kết quả cần thấy:** Mỗi nhiệm vụ trong năm nhiệm vụ được gắn nhãn tính năng.

### Bước 3 — Nêu dấu hiệu chủ đạo quyết định mỗi nhãn

Chọn giữa bối cảnh dùng chung lặp lại, tổng hợp đa nguồn có trích dẫn, sản phẩm có thể chia sẻ và tinh chỉnh qua nhiều vòng hoặc công việc đơn giản làm một lần.

**Vì sao:** Phần dẫn câu hỏi cung cấp dấu hiệu, không cung cấp tên tính năng. Mục đích thực hành là ghép đúng chúng.

**Kết quả cần thấy:** Một dấu hiệu được nêu rõ bên cạnh mỗi nhãn tính năng.

### Bước 4 — Tìm một cách làm vòng thủ công trong thói quen của bạn

Ví dụ: dán lại bối cảnh qua nhiều chat hoặc để một tài liệu cần cập nhật thường xuyên bị chôn trong cuộc trò chuyện cũ. Nêu tính năng chấm dứt cách làm đó.

**Vì sao:** Cách làm vòng là kiểu làm việc không hiệu quả mà bài thi thường trình bày dưới vẻ ngoài cẩn thận. Tìm ra trường hợp của chính mình giúp bạn nhận ra nó trong phần dẫn câu hỏi.

**Kết quả cần thấy:** Một câu mô tả cách làm vòng cùng tính năng thay thế.

### Bước 5 — Ghi nhận Project cần tạo cho công việc lặp lại rồi dừng ở đó

Nếu một công việc lặp lại nên có Project, hãy ghi lại để thiết lập sau. Cấu hình Project tốt là kỹ năng sẽ học ở phần sau.

**Vì sao:** Mục tiêu này kết thúc ở quyết định lựa chọn. Chỉ dẫn và việc chọn lọc kiến thức thuộc Lĩnh vực 5.

**Kết quả cần thấy:** Ghi chú nêu tên Project bạn sẽ tạo và công việc lặp lại mà nó phục vụ.

## Tài liệu tham khảo

Các tài liệu của **Anthropic** được liệt kê trong bản gốc:

- Project là gì? — *What are projects?*
- Sử dụng Research trên Claude — *Use research on Claude*.
- Phân tích hiệu quả chiến dịch — *Analyze campaign performance*.
- Artifact là gì và sử dụng như thế nào? — *What are artifacts and how do I use them?*
- Khi nào nên dùng tìm kiếm web, suy nghĩ mở rộng và Research? — *When should I use web search, extended thinking, and research?*
- Hướng dẫn thi Claude Certified Associate – Foundations — *Claude Certified Associate – Foundations Exam Guide*.

## Điều hướng trong tài liệu gốc

- Ôn luyện lĩnh vực này.
- Bài tập thực hành.
- Tài liệu tra cứu nhanh.
- Bảng thuật ngữ.
- **Bài trước:** [2.6 — Chọn lọc thông tin và lựa chọn định dạng đầu ra](2-6-output-formats-curation.vi.md).
- **Bài tiếp theo:** Phân biệt các loại mô hình Claude — *Differentiating Between Claude Model Types*.
