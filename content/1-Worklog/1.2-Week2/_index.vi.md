---
title: "Nhật ký Tuần 2"
date: 2026-04-24
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

{{% notice warning %}}
 **Lưu ý:** Nội dung dưới đây ghi chép lại các hoạt động học tập và thực hành đã hoàn thành trong tuần, được sử dụng cho báo cáo nhật ký công việc cá nhân.
{{% /notice %}}

### Mục tiêu Tuần 2:
- Phân biệt Object Storage và Block Storage.
- Thực hành thực tế với dịch vụ Amazon S3.
- Triển khai một trang web tĩnh (static website) sử dụng S3 bucket.

### Các công việc thực hiện trong tuần:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 24/04/2026 | Nghiên cứu các tính năng của Amazon S3, các lớp lưu trữ (storage classes) và quy tắc đặt tên bucket. | 24/04/2026 | 24/04/2026 | Tài liệu AWS S3 |
| 25/04/2026 – 26/04/2026 | Tạo S3 bucket mới, tải lên các file thử nghiệm và quản lý Object Ownership. | 25/04/2026 | 26/04/2026 | AWS Management Console |
| 27/04/2026 | Cấu hình Bucket Policies để cấp quyền đọc công khai (public read) cho các object cụ thể. | 27/04/2026 | 27/04/2026 | S3 Policy Generator |
| 28/04/2026 – 29/04/2026 | Bật tính năng Static Website Hosting trên S3 và tải lên một mẫu HTML/CSS cơ bản. | 28/04/2026 | 29/04/2026 | <https://cloudjourney.awsstudygroup.com/> |
| 30/04/2026 | Kiểm tra truy cập trang web qua URL endpoint của S3 và tìm hiểu tính năng S3 Versioning. | 30/04/2026 | 30/04/2026 | Trình duyệt web / S3 Console |

### Kết quả đạt được trong Tuần 2:
- Phân biệt được các lớp lưu trữ S3 khác nhau (Standard, Glacier).
- Viết và áp dụng thành công JSON Bucket Policies.
- Lưu trữ và chạy thành công một trang web tĩnh hoàn toàn bằng Amazon S3 mà không cần máy chủ.