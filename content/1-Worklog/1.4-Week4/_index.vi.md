---
title: "Nhật ký Tuần 4"
date: 2026-05-08
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

{{% notice warning %}}
 **Lưu ý:** Nội dung dưới đây ghi chép lại các hoạt động học tập và thực hành đã hoàn thành trong tuần, được sử dụng cho báo cáo nhật ký công việc cá nhân.
{{% /notice %}}

### Mục tiêu Tuần 4:
- Phân biệt cơ sở dữ liệu tự quản lý (DB trên EC2) và cơ sở dữ liệu được quản lý (RDS).
- Khởi tạo một instance Amazon RDS MySQL.
- Thiết lập kết nối từ máy tính cá nhân (local) đến RDS.

### Các công việc thực hiện trong tuần:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 08/05/2026 | Tìm hiểu các dịch vụ Cơ sở dữ liệu của AWS (RDS, DynamoDB) và các trường hợp sử dụng. | 08/05/2026 | 08/05/2026 | Tài liệu AWS RDS |
| 09/05/2026 – 10/05/2026 | Cấu hình và khởi tạo một RDS MySQL instance trong gói Free Tier. | 09/05/2026 | 10/05/2026 | AWS Management Console |
| 11/05/2026 | Điều chỉnh Security Group của RDS để cho phép luồng truy cập MySQL (port 3306) từ IP của tôi. | 11/05/2026 | 11/05/2026 | Cấu hình mạng |
| 12/05/2026 – 13/05/2026 | Cài đặt phần mềm DB client (DBeaver) và kết nối thành công đến endpoint của RDS. | 12/05/2026 | 13/05/2026 | Hướng dẫn sử dụng DBeaver |
| 14/05/2026 | Tạo một database thử nghiệm và chạy các lệnh SQL cơ bản. | 14/05/2026 | 14/05/2026 | Cú pháp MySQL |

### Kết quả đạt được trong Tuần 4:
- Hiểu được lợi ích quản trị khi sử dụng Amazon RDS so với việc tự quản lý cơ sở dữ liệu.
- Khởi tạo và kết nối thành công đến cơ sở dữ liệu MySQL từ xa trên AWS.
- Học cách xử lý thông tin đăng nhập database và cấu hình luật bảo mật an toàn.