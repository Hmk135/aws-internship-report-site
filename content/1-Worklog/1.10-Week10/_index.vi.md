---
title: "Nhật ký Tuần 10"
date: 2026-06-19
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---


### Mục tiêu Tuần 10:
- Đưa ứng dụng private ra bên ngoài một cách bảo mật.
- Cấu hình Application Load Balancer (ALB).
- Tích hợp CloudFront để tối ưu hóa việc phân phối nội dung toàn cầu.

### Các công việc thực hiện trong tuần:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 19/06/2026 | Tạo Target Group trỏ đến máy chủ EC2 Backend ở trong private subnet (port 8080). | 19/06/2026 | 19/06/2026 | Cấu hình Target Group |
| 20/06/2026 – 21/06/2026 | Khởi tạo Application Load Balancer ở lớp Public Subnets và gắn Target Group vào. | 20/06/2026 | 21/06/2026 | Thiết lập ALB |
| 22/06/2026 | Kiểm tra xác nhận các API của ứng dụng có thể gọi thành công qua tên miền DNS của ALB. | 22/06/2026 | 22/06/2026 | Postman / Browser |
| 23/06/2026 – 24/06/2026 | Tạo CloudFront Distribution dùng ALB làm máy chủ gốc (origin server). | 23/06/2026 | 24/06/2026 | Tài liệu CloudFront |
| 25/06/2026 | Điều chỉnh CloudFront cache behaviors và cấp phép cho các phương thức HTTP cụ thể (GET, POST). | 25/06/2026 | 25/06/2026 | Chiến lược Caching |

### Kết quả đạt được trong Tuần 10:
- Hoàn thiện lớp mạng tiếp xúc công khai (public exposure layer) của kiến trúc 3-tier.
- Định tuyến thành công lưu lượng internet từ ngoài vào sâu bên trong EC2 private thông qua ALB.
- Ứng dụng CloudFront Edge locations (kiến thức từ sự kiện Community Day) để tăng tốc độ phản hồi của ứng dụng.