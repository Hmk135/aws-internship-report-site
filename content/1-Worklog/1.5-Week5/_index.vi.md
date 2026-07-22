---
title: "Nhật ký Tuần 5"
date: 2026-05-15
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

{{% notice warning %}}
 **Lưu ý:** Nội dung dưới đây ghi chép lại các hoạt động học tập và thực hành đã hoàn thành trong tuần, được sử dụng cho báo cáo nhật ký công việc cá nhân.
{{% /notice %}}

### Mục tiêu Tuần 5:
- Hiểu các khái niệm về tính sẵn sàng cao (High Availability) trong điện toán đám mây.
- Học cách phân phối lưu lượng truy cập bằng Application Load Balancer (ALB).
- Cấu hình Target Group cho nhiều máy chủ EC2.

### Các công việc thực hiện trong tuần:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 15/05/2026 | Tìm hiểu các loại Elastic Load Balancing (ELB) và khái niệm Target Groups. | 15/05/2026 | 15/05/2026 | Hướng dẫn AWS ELB |
| 16/05/2026 – 17/05/2026 | Khởi tạo hai máy chủ EC2 độc lập ở hai Availability Zones khác nhau để thử nghiệm. | 16/05/2026 | 17/05/2026 | AWS EC2 Console |
| 18/05/2026 | Cấu hình script user-data để hiển thị hostname riêng biệt trên mỗi web server EC2. | 18/05/2026 | 18/05/2026 | Shell scripting |
| 19/05/2026 – 20/05/2026 | Tạo Target Group, đăng ký hai máy chủ EC2 vào nhóm và kiểm tra health checks. | 19/05/2026 | 20/05/2026 | AWS Console |
| 21/05/2026 | Thiết lập Application Load Balancer và kiểm tra việc phân phối traffic qua tên miền DNS của ALB. | 21/05/2026 | 21/05/2026 | Kiểm tra trên trình duyệt |

### Kết quả đạt được trong Tuần 5:
- Hiểu được tầm quan trọng của việc phân tán khối lượng công việc qua nhiều Availability Zones.
- Cấu hình thành công một ALB để định tuyến lưu lượng HTTP đồng đều cho nhiều máy chủ backend.
- Học được cách Health Checks tự động ngăn chặn việc gửi traffic đến các máy chủ đang bị lỗi.