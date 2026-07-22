---
title: "Nhật ký Tuần 9"
date: 2026-06-12
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---



### Mục tiêu Tuần 9:
- Chuẩn bị EC2 Backend để chạy ứng dụng.
- Triển khai source code dự án RecruitPro và các thư viện cần thiết.
- Cấp quyền cho EC2 truy cập và tải file lên S3 một cách an toàn thông qua IAM Roles.

### Các công việc thực hiện trong tuần:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 12/06/2026 | Tạo một IAM Role cấp quyền truy cập S3 và gắn vào máy chủ EC2 Backend. | 12/06/2026 | 12/06/2026 | IAM Roles cho EC2 |
| 13/06/2026 – 14/06/2026 | Cài đặt Java (JDK) và các môi trường chạy cần thiết trên EC2 Backend. | 13/06/2026 | 14/06/2026 | Trình quản lý gói Linux |
| 15/06/2026 | Chuyển file build `.jar` và script khởi tạo SQL vào máy chủ EC2 private. | 15/06/2026 | 15/06/2026 | SCP / WinSCP |
| 16/06/2026 – 17/06/2026 | Import database schema vào RDS và cấu hình file `application.properties` của ứng dụng. | 16/06/2026 | 17/06/2026 | Source Code Dự án |
| 18/06/2026 | Tạo dịch vụ `systemd` để chạy ứng dụng Spring Boot ngầm và an toàn. | 18/06/2026 | 18/06/2026 | Tài liệu systemd |

### Kết quả đạt được trong Tuần 9:
- Loại bỏ hoàn toàn việc phải lưu cứng (hardcode) thông tin xác thực AWS bằng cách sử dụng IAM Roles.
- Khởi động thành công ứng dụng backend và xác nhận hệ thống chạy ổn định.
- Học cách quản lý các tiến trình chạy ngầm (background processes) trên Linux bằng `systemd`.