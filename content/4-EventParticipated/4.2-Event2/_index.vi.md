---
title: "Event 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 4.2. </b> "
---

# Bài thu hoạch "FCAJ Community Day"

### Mục Đích Của Sự Kiện

- Kết nối các thành viên trong cộng đồng First Cloud AI Journey (FCJ) để chia sẻ kinh nghiệm dự án thực tế
- Tạo không gian cho các bạn intern/mentee và cộng đồng AWS trình bày các sản phẩm, dự án liên quan đến AI, hạ tầng cloud
- Khuyến khích trao đổi kiến thức giữa nhiều mảng khác nhau: prompt/context engineering, AI assistant, kiến trúc cloud, LLM, kinh nghiệm làm product/hackathon
- Tăng cường kết nối giữa intern, mentor và cộng đồng AWS Study Group nói chung

### Danh Sách Diễn Giả & Chủ Đề

- **Tinh Truong** – Platform Engineer, GoTymeX – "Context Is Everything: Making AI Actually Work for You"
- **Pham Ng. Hai Anh** – AWS Community Builder, G-AsiaPacific Vietnam – "Friendly AI Assistant w/ Amazon Quick"
- **Nguyen Tuan Thinh** – DevOps Engineer, First Cloud AI Journey – "From Edge To Origin: CloudFront as Your Foundation"
- **Team VIB** – "36 hrs with LotusHacks – Building UTMorpho from Idea to Reality"
- **Duc Dao** – Solution Architect, Cloud Kinetics – "Non-Determinism of 'Deterministic' LLM Settings"
- **Vy Lam** – Senior Business Systems Analyst, VPBank – "Enterprise-Grade Multi-Agent System: The Case of Startup Credit Scoring"

### Nội Dung Nổi Bật

#### Context Is Everything: Making AI Actually Work for You

- Lập luận rằng các mô hình AI hiện nay đã đủ mạnh, phần còn thiếu thường nằm ở **context** (bối cảnh) cung cấp cho model
- Làm rõ "context" gồm những gì: mục tiêu, dữ liệu/môi trường, các ràng buộc, và các dẫn chứng liên quan
- Chỉ ra các lỗi thường gặp khi làm việc với AI, ví dụ vấn đề "internet pull" (model lấy thông tin chung trên internet thay vì dùng đúng context của bạn) và việc lặp lại cho AI những gì nó đã biết

#### Friendly AI Assistant w/ Amazon Quick

- Mô tả một ngày làm việc điển hình của business user có thể trở nên khó khăn nếu thiếu công cụ AI phù hợp
- Giới thiệu **Amazon Quick Suite**, giải pháp mới của AWS để xây dựng trải nghiệm agentic AI thân thiện cho người dùng doanh nghiệp

#### From Edge To Origin: CloudFront as Your Foundation

- Định vị Amazon CloudFront không chỉ là một dịch vụ CDN, mà còn là **nền tảng (foundation)** giúp bảo vệ và tối ưu hóa ứng dụng
- Trình bày các thách thức thường gặp, cách CloudFront hoạt động, các khả năng về chi phí, bảo mật, độ bền vững và hiệu năng, cùng các use case/best practice thực tế

#### Xây dựng UTMorpho trong 36 giờ tại LotusHacks

- Chia sẻ kinh nghiệm đưa một ý tưởng sản phẩm từ concept thành prototype hoạt động được trong 36 giờ hackathon
- Nhấn mạnh tầm quan trọng của việc scope công việc rõ ràng, chia việc hợp lý trong team và lặp nhanh dưới áp lực thời gian

#### Non-Determinism of "Deterministic" LLM Settings

- Dựa trên nghiên cứu của Atil et al. (2024) từ Penn State University & Comcast AI Technologies
- Giải thích cách LLM chọn token tiếp theo, vai trò của temperature, top-p và top-k
- Lý giải vì sao ngay cả khi cấu hình ở chế độ tưởng như "deterministic", output của LLM vẫn có thể không ổn định, và các chiến lược giảm thiểu (mitigation) vấn đề này

#### Enterprise-Grade Multi-Agent System: The Case of Startup Credit Scoring

- Trình bày vấn đề structural mismatch trong các hệ thống chấm điểm tín dụng truyền thống khi áp dụng cho startup
- Trình bày case study áp dụng kiến trúc multi-agent để xử lý bài toán credit scoring này một cách đáng tin cậy hơn so với dùng một model đơn lẻ

### Những Gì Học Được

- "Context" (bối cảnh) đưa vào AI quan trọng không kém, đôi khi còn quan trọng hơn, so với việc chọn model nào
- Xây dựng trợ lý AI cho doanh nghiệp không chỉ là bài toán về model — trải nghiệm và luồng làm việc thực tế của business user mới là điều quyết định
- Các quyết định thiết kế liên quan đến edge/CDN (như CloudFront) ảnh hưởng trực tiếp đến hiệu năng thực tế mà người dùng cảm nhận được
- Ngay cả với cấu hình "deterministic", LLM vẫn có thể cho ra kết quả không hoàn toàn ổn định — cần hiểu rõ vai trò của temperature/top-p/top-k để kiểm soát tốt hơn
- Kiến trúc multi-agent đang trở thành một pattern thực tế cho các bài toán doanh nghiệp quá phức tạp để xử lý bằng một lần gọi LLM duy nhất
- Áp lực thời gian kiểu hackathon (36 giờ) buộc phải ưu tiên rõ ràng hơn và ra quyết định nhanh hơn

### Ứng Dụng Vào Công Việc

- Chú ý cung cấp đủ context (mục tiêu, dữ liệu, ràng buộc) khi dùng AI hỗ trợ viết code hoặc tài liệu trong quá trình thực tập
- Tham khảo tư duy "CDN-first" (CloudFront) khi trình bày về cách frontend của CloudDoc được phân phối đến người dùng
- Ghi nhớ vấn đề non-determinism của LLM khi thiết kế các tính năng có dùng AI, để không giả định output luôn giống nhau
- Theo dõi thêm các pattern liên quan đến multi-agent và AI assistant như một hướng phát triển tính năng trong tương lai
- Áp dụng cách tư duy scope và ưu tiên công việc từ LotusHacks vào các giai đoạn làm việc có deadline gấp trong dự án

### Trải nghiệm trong event

Tham gia **FCAJ Community Day** là một cơ hội quý giá để thấy cách các bạn intern và thành viên khác trong cộng đồng áp dụng AI, cloud và kỹ năng xây dựng sản phẩm vào các dự án thực tế ngoài phạm vi thực tập của mình. Một số điểm nổi bật:

#### Học hỏi từ nhiều diễn giả với background đa dạng
- Mỗi diễn giả đến từ một bối cảnh dự án khác nhau, giúp tôi có cái nhìn rộng hơn về việc "build trên AWS" ngoài phạm vi dự án CloudDoc của mình.
- Phần chia sẻ về non-determinism của LLM giúp tôi hiểu rõ hơn một số khái niệm mà trước đây mình chỉ dùng ở mức bề mặt.

#### Trải nghiệm áp lực dự án thực tế
- Câu chuyện LotusHacks của Team VIB là một lời nhắc nhở tốt về việc có thể build được nhiều đến mức nào trong thời gian ngắn nếu scope rõ ràng và team giao tiếp tốt.
- Đây cũng là dịp để tôi nhận ra một prototype chạy được ở giai đoạn đầu có giá trị hơn một bản hoàn hảo nhưng chưa xong.

#### Kết nối và mở rộng mối quan hệ
- Sự kiện tạo cơ hội tự nhiên để gặp gỡ các bạn intern và mentor khác trong cộng đồng FCJ, hữu ích cho việc học hỏi và hợp tác sau này.

#### Một số hình ảnh khi tham gia sự kiện

<img src="/images/4-EventParticipated/4.2-Event2/event-2.jpg" alt="Hình ảnh tại sự kiện FCAJ Community Day" style="max-width: 90%; height: auto;">

> Tổng thể, FCAJ Community Day giúp tôi có góc nhìn rộng hơn về cách kỹ năng AI và cloud được áp dụng ở nhiều team và dự án khác nhau, ngoài phạm vi công việc thực tập của riêng mình.
