---
title: "Nhật ký Tuần 8"
date: 2026-06-05
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

{{% notice warning %}}
 **Lưu ý:** Nội dung dưới đây ghi chép lại các hoạt động học tập và thực hành đã hoàn thành trong tuần, được sử dụng cho báo cáo nhật ký công việc cá nhân.
{{% /notice %}}

### Mục tiêu Tuần 8:
- Triển khai lớp cơ sở dữ liệu một cách bảo mật bên trong VPC tùy chỉnh.
- Khởi chạy máy chủ EC2 backend trong private subnet.
- Thiết lập kết nối thành công giữa backend và database.

### Các công việc thực hiện trong tuần:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 05/06/2026 | Tạo DB Subnet Group gom chung hai private DB subnets bên trong RecruitPro-VPC. | 05/06/2026 | 05/06/2026 | RDS Console |
| 06/06/2026 – 07/06/2026 | Khởi chạy RDS MySQL instance gắn vào private DB subnets. | 06/06/2026 | 07/06/2026 | AWS Management Console |
| 08/06/2026 | Triển khai một Bastion Host tại Public Subnet để truy cập vào mạng nội bộ. | 08/06/2026 | 08/06/2026 | SSH Agent forwarding |
| 09/06/2026 – 10/06/2026 | Khởi chạy EC2 Backend trong Private App Subnet và kết nối thông qua Bastion Host. | 09/06/2026 | 10/06/2026 | Định tuyến mạng |
| 11/06/2026 | Cài đặt MySQL Client trên EC2 Backend và kiểm tra kết nối thành công đến RDS endpoint. | 11/06/2026 | 11/06/2026 | Linux CLI |

### Kết quả đạt được trong Tuần 8:
- Triển khai thành công một cơ sở dữ liệu hoàn toàn riêng tư (private) không thể truy cập từ bên ngoài.
- Nắm vững khái niệm Bastion Host (Jump Box) để quản trị hệ thống nội bộ một cách an toàn.
- Xác nhận đường truyền kết nối nội bộ giữa lớp Ứng dụng (Application tier) và lớp Dữ liệu (Database tier).