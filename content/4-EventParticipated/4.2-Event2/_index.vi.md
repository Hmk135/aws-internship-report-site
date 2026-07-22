---
title: "Sự kiện 11/7/2026 - Bảo mật, Giám sát & Chứng chỉ AWS"
date: 2026-07-11
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---

# Những bài học từ sự kiện ngày 11 tháng 7

Vào ngày 11 tháng 7 năm 2026, tôi đã tham dự một sự kiện chuyên sâu về chứng chỉ đám mây, giám sát hệ thống và bảo mật ứng dụng bằng AI. Phiên chia sẻ này mang đến các chiến lược thực tế để vượt qua các bài thi AWS và góc nhìn sâu sắc về việc bảo mật các ứng dụng web hiện đại bằng các tác nhân AI tự trị (autonomous agents).

## Tổng quan các phiên chia sẻ

- Diễn giả (Huy): **Inside The Exam: AWS Cloud Practitioner**.
- Nguyễn Huỳnh Sơn: **SLA and Monitoring - From SLA to Monitoring what really matters**.
- Thịnh Nguyễn: **Securing Your Web Apps With AWS Security Agent**.

## Những kiến thức trọng tâm

### Bí quyết chinh phục kỳ thi AWS Cloud Practitioner
Sự kiện đã chia sẻ những "Mẹo & Thủ thuật" (Tips & Tricks) rất giá trị cho kỳ thi:
- **Phương pháp loại trừ (Elimination technique):** Các câu hỏi thường có 4 đáp án, trong đó có 2 đáp án là các dịch vụ "bịa ra" hoặc hoàn toàn không liên quan; loại trừ chúng trước sẽ giúp tăng cơ hội chọn đúng lên 50%.
- **Đừng nghĩ quá phức tạp (Don't overthink):** Bài thi Cloud Practitioner tập trung vào kiến thức nền tảng. Nếu một câu hỏi có vẻ yêu cầu cấu hình quá phức tạp, khả năng cao là bạn đang làm phức tạp hóa vấn đề, hãy chọn đáp án đơn giản và trực diện nhất.
- **Cạm bẫy ngôn ngữ (Language pitfalls):** Bài thi tiếng Anh có thể đánh lừa người đọc, do đó diễn giả khuyên nên làm nổi bật ngay các từ khóa mang tính quyết định khi đọc câu hỏi như "Not" (Không), "Least cost" (Chi phí thấp nhất) hay "Most scalable" (Khả năng mở rộng cao nhất).

### Giám sát hệ thống thực chất
Anh Nguyễn Huỳnh Sơn nhấn mạnh việc dịch chuyển góc nhìn từ các con số SLA tiêu chuẩn sang việc giám sát những chỉ số thực sự quan trọng đối với hệ thống và doanh nghiệp.

### Vượt qua "Nút thắt Bảo mật"
Anh Thịnh Nguyễn chỉ ra rằng các bài kiểm tra thâm nhập (penetration testing) thủ công truyền thống rất tốn thời gian (mất hàng tuần) và đắt đỏ (chi phí theo ngày của các hacker chuyên nghiệp rất cao). Nó cũng thiếu tính nhất quán vì độ bao phủ phụ thuộc vào tâm trạng hoặc kỹ năng của người kiểm tra, dẫn đến chi phí vận hành cao, lên tới khoảng 20 nghìn đô la cho các dịch vụ đánh giá bên thứ ba.

### Bảo mật bằng AI với Frontier Agent
Để giải quyết nút thắt này, "Frontier Agent" đã được giới thiệu. Nó có các đặc điểm:
- **Lập luận tự trị (Autonomous Reasoning):** Được hỗ trợ bởi Amazon Bedrock, nó có thể tự lên kế hoạch và thực thi các tác vụ bảo mật mà không cần con người can thiệp.
- **Bao phủ toàn vòng đời (Full Lifecycle):** Nó xử lý từ Đánh giá thiết kế (Design Review), Bảo mật mã nguồn, cho đến Kiểm thử thâm nhập chủ động (Active Pentesting).
- **Phát hiện có thể xác thực (Verifiable Findings):** Khác với các chatbot LLM thông thường, nó xác minh các lỗ hổng bằng cách cố gắng khai thác chúng trên thực tế.
- **Đánh giá Thiết kế Bảo mật (Design Security Review):** Bạn có thể tải lên các file Markdown hoặc mã Terraform để agent đối chiếu với các bộ tiêu chuẩn (Managed Packs) như PCI DSS, NIST CSF, AWS Well-Architected nhằm kiểm tra xem thiết kế có đáp ứng các "Yêu cầu" bảo mật hay không. Tính năng này cung cấp gói Free Tier miễn phí 200 lượt đánh giá/tháng.

### Những hạn chế của AI Security Agents
Dù rất mạnh mẽ, các tác nhân AI cũng có những hạn chế chí mạng:
- **Rào cản xác thực (Auth Blocks):** Việc áp dụng MFA (Xác thực đa yếu tố), Sinh trắc học (Biometrics) hay mTLS sẽ chặn đứng agent ngay lập tức.
- **Lỗi logic (Logic Flaws):** Agent rất khó phát hiện các gian lận về logic nghiệp vụ (business-logic fraud) nếu thiếu ngữ cảnh sâu sát.
- **Tích lũy giờ làm (Task-Hour Accumulation):** Các ứng dụng phức tạp sẽ làm agent đốt thời gian rất nhanh, do đó việc giám sát (monitoring) là bắt buộc.

## Những hành động có thể áp dụng ngay
- Luôn gạch dưới các ràng buộc chính như "Least cost" (Chi phí thấp nhất) hay "Most scalable" khi phân tích các bài toán Cloud hoặc đề thi.
- Vượt ra khỏi các chỉ số SLA cơ bản để thiết lập giám sát những gì thực sự ảnh hưởng đến "sức khỏe" hệ thống.
- Tận dụng tính năng Đánh giá Thiết kế Bảo mật tự động đối chiếu với các chuẩn như AWS Well-Architected.
- Áp dụng các rào cản xác thực mạnh như MFA và Sinh trắc học, vì chúng cực kỳ hiệu quả trong việc chặn đứng các tác nhân tấn công tự động.

## Ứng dụng vào dự án RecruitPro
Các chiến lược làm bài thi sẽ trực tiếp giúp tôi đạt được chứng chỉ AWS trong thời gian tới. Đối với RecruitPro, tôi sẽ thiết kế lại các dashboard trên CloudWatch để giám sát những chỉ số thực sự quan trọng thay vì chỉ đo lường uptime cơ bản. Hơn nữa, việc biết được MFA có thể vô hiệu hóa AI agent càng củng cố quyết định của tôi trong việc áp dụng xác thực khắt khe cho trang quản trị backend của dự án.

## Minh chứng tham gia
![My photo at FCAJ Community Day](</images/4-EventParticipated/4.2-Event2/Picture3.jpg>)

![Photo taken during the event](</images/4-EventParticipated/4.2-Event2/picture4.jpg>)

## Kết luận
Sự kiện này là sự kết hợp hoàn hảo giữa phát triển nghề nghiệp (mẹo thi chứng chỉ) và kiến thức kỹ thuật nâng cao (AI Security Agent). Nó giúp tôi mở rộng tầm mắt về tương lai của quy trình kiểm thử tự động, đồng thời khẳng định lại tầm quan trọng bền vững của các phương pháp bảo mật nền tảng như MFA.