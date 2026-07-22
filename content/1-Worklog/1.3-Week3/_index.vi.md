---
title: "Nhật ký Tuần 3"
date: 2026-05-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---



### Mục tiêu Tuần 3:
- Nắm vững kiến thức cơ bản về Amazon EC2 (Elastic Compute Cloud) và EBS.
- Thực hành kết nối vào EC2 bằng SSH và hiểu về Key Pairs.
- Cài đặt một web server cơ bản trên máy chủ Linux.

### Các công việc thực hiện trong tuần:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 01/05/2026 | Xem lại các dòng máy EC2 (t2, t3) và Amazon Machine Images (AMI). | 01/05/2026 | 01/05/2026 | Tổng quan AWS EC2 |
| 02/05/2026 – 03/05/2026 | Khởi tạo một máy chủ EC2 Amazon Linux 2023 và tạo mới một Key Pair `.pem`. | 02/05/2026 | 03/05/2026 | AWS EC2 Console |
| 04/05/2026 | Kết nối vào máy chủ EC2 bằng SSH (thông qua Termius/MobaXterm). | 04/05/2026 | 04/05/2026 | Cấu hình SSH Client |
| 05/05/2026 | Cấu hình Security Groups để cho phép truy cập SSH (port 22) và HTTP (port 80). | 05/05/2026 | 05/05/2026 | Quy tắc Security Group |
| 06/05/2026 – 07/05/2026 | Cài đặt Apache Web Server (`httpd`), khởi động dịch vụ và kiểm tra trang web mặc định. | 06/05/2026 | 07/05/2026 | Các lệnh Linux CLI |

### Kết quả đạt được trong Tuần 3:
- Thành thạo các bước khởi tạo EC2 và hiểu vai trò của Security Groups như một tường lửa ảo.
- Kết nối an toàn vào một máy chủ đám mây bằng giao thức SSH.
- Chuyển đổi thành công một máy chủ Linux thô thành một web server hoạt động được.