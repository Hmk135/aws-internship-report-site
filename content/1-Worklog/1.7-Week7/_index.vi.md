---
title: "Nhật ký Tuần 7"
date: 2026-05-29
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

{{% notice warning %}}
 **Lưu ý:** Nội dung dưới đây ghi chép lại các hoạt động học tập và thực hành đã hoàn thành trong tuần, được sử dụng cho báo cáo nhật ký công việc cá nhân.
{{% /notice %}}

### Mục tiêu Tuần 7:
- Thiết kế một mạng VPC bảo mật, tùy chỉnh riêng cho dự án RecruitPro.
- Triển khai kiến trúc 3 lớp với các mạng con: Public, Private App và Private DB.
- Thiết lập các luồng định tuyến (routing) chính xác bằng Internet Gateway và NAT Gateway.

### Các công việc thực hiện trong tuần:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 29/05/2026 | Tạo `RecruitPro-VPC` với dải mạng CIDR `10.10.0.0/16` tại region `ap-southeast-1`. | 29/05/2026 | 29/05/2026 | Cài đặt AWS VPC |
| 30/05/2026 | Khởi tạo 2 Public Subnets, 2 Private App Subnets, và 2 Private DB Subnets trải ra hai AZs. | 30/05/2026 | 30/05/2026 | Bảng quy hoạch subnet |
| 31/05/2026 | Gắn Internet Gateway (IGW) vào VPC và tạo một NAT Gateway kèm theo Elastic IP. | 31/05/2026 | 31/05/2026 | Hướng dẫn AWS Networking |
| 01/06/2026 – 02/06/2026 | Cấu hình Route Table cho Public (hướng ra IGW) và Private (hướng ra NAT Gateway). | 01/06/2026 | 02/06/2026 | Cấu hình Route Table |
| 03/06/2026 | Tạo các Security Groups cốt lõi cho ALB (Public), EC2 (Private) và RDS (Private). | 03/06/2026 | 03/06/2026 | Chính sách Security Group |
| 04/06/2026 | Kiểm tra các kết nối subnet và đảm bảo DB subnets không thể kết nối ra internet. | 04/06/2026 | 04/06/2026 | VPC reachability analyzer |

### Kết quả đạt được trong Tuần 7:
- Xây dựng thành công một nền tảng mạng độc lập, an toàn và có tính sẵn sàng cao cho RecruitPro.
- Hiểu cách che chắn các máy chủ ứng dụng và cơ sở dữ liệu nội bộ khỏi sự truy cập trực tiếp từ public.
- Móc nối chính xác các Security Groups để RDS chỉ chấp nhận kết nối từ backend EC2.