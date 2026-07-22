---
title: "Nhật ký Tuần 11"
date: 2026-06-26
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

{{% notice warning %}}
 **Lưu ý:** Nội dung dưới đây ghi chép lại các hoạt động học tập và thực hành đã hoàn thành trong tuần, được sử dụng cho báo cáo nhật ký công việc cá nhân.
{{% /notice %}}

### Mục tiêu Tuần 11:
- Triển khai giám sát hệ thống (monitoring) sử dụng Amazon CloudWatch.
- Tăng cường bảo mật ứng dụng bằng AWS WAF.
- Thực hiện kiểm thử lần cuối cho hệ thống RecruitPro.

### Các công việc thực hiện trong tuần:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 26/06/2026 | Khám phá CloudWatch Metrics và Logs cho EC2, RDS, và ALB. | 26/06/2026 | 26/06/2026 | Tổng quan CloudWatch |
| 27/06/2026 – 28/06/2026 | Tạo một CloudWatch Dashboard tùy chỉnh để theo dõi CPU của EC2 và số lượng kết nối DB. | 27/06/2026 | 28/06/2026 | Cấu hình Dashboard |
| 29/06/2026 | Thiết lập CloudWatch Alarms để gửi email thông báo (qua SNS) nếu CPU vượt mức 80%. | 29/06/2026 | 29/06/2026 | AWS SNS & CloudWatch |
| 30/06/2026 – 01/07/2026 | Cấu hình AWS WAF (Web Application Firewall) Web ACL và gắn nó vào CloudFront. | 30/06/2026 | 01/07/2026 | Các quy tắc AWS WAF |
| 02/07/2026 | Tiến hành kiểm thử hệ thống: tải file lên, truy xuất dữ liệu, và kiểm tra các luật chặn của WAF. | 02/07/2026 | 02/07/2026 | Kiểm thử Ứng dụng |

### Kết quả đạt được trong Tuần 11:
- Xây dựng giải pháp giám sát chủ động để tự động theo dõi sức khỏe hệ thống.
- Bổ sung một lớp bảo mật cực kỳ quan trọng bằng cách lọc các luồng truy cập web độc hại với AWS WAF.
- Đảm bảo hệ thống RecruitPro đã hoạt động đầy đủ chức năng, ổn định và an toàn.