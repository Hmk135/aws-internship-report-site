---
title: "Sự kiện 23/5/2026 - FCAJ Community Day"
date: 2026-05-23
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

# Trải nghiệm của tôi tại FCAJ Community Day

Vào ngày 23 tháng 5 năm 2026, tôi cùng một người bạn đã tham gia sự kiện FCAJ Community Day. Sự kiện mang đến một loạt các bài thuyết trình đa dạng, đề cập đến mọi thứ từ hạ tầng AWS (như CloudFront) cho đến các ứng dụng AI thực tế (như tính tất định của LLM, tối ưu hóa ngữ cảnh và kiến trúc Multi-Agent cho doanh nghiệp). Trong bài báo cáo này, tôi sẽ làm nổi bật những kiến thức giá trị nhất mà mình thu nhận được và cách tôi dự định áp dụng chúng vào công việc thực tế.

## Tổng quan các phiên chia sẻ

- Tịnh: **Context Is Everything**.
- Phạm Ngô Hải Anh: **Friendly AI Assistant with Amazon Quick**.
- Nguyễn Tuấn Thịnh: **From Edge to Origin**.
- Team VIB: **36 Hours with LotusHacks**.
- Đào Đức: **Non-Determinism of Deterministic LLM Settings**.
- Cát Vy: **Enterprise-Grade Multi-Agent System**.

## Những bài học và kiến thức trọng tâm

### Kỹ năng Prompting: Chất lượng quan trọng hơn Số lượng
Tôi từng nghĩ rằng cung cấp cho AI càng nhiều văn bản thì kết quả trả về sẽ càng tốt. Tuy nhiên, phiên chia sẻ này đã nhấn mạnh rằng sự chính xác quan trọng hơn nhiều. Một ngữ cảnh (context) được chuẩn bị tốt chỉ nên chứa các mục tiêu cụ thể, các ràng buộc và dữ liệu cần thiết. Việc nhồi nhét vào prompt những thông tin không liên quan không chỉ gây lãng phí token mà còn làm mô hình bị phân tâm. Khái niệm "Bộ não AI thứ hai" (Second AI Brain) — một hệ thống truy xuất chỉ lấy những ghi chú hoặc tài liệu có liên quan cao nhất trước khi đưa chúng cho AI — đã đặc biệt truyền cảm hứng cho tôi trong việc quản lý tài liệu của các dự án lớn.

### Tầm quan trọng của việc kiểm soát quyền truy cập dữ liệu trong AI
Bài thuyết trình về Amazon Quick đã cho thấy sức mạnh của các trợ lý AI doanh nghiệp trong việc xử lý các tác vụ như lên lịch, soạn thảo email và tóm tắt cuộc họp. Tuy nhiên, bài học lớn nhất đối với tôi là nhu cầu cấp thiết về bảo mật. Một AI nội bộ của công ty phải được quản lý chặt chẽ bằng các biện pháp kiểm soát truy cập dựa trên vai trò (Role-based access controls) để đảm bảo người dùng chỉ có thể truy vấn những thông tin mà họ được cấp phép xem một cách rõ ràng.

### CloudFront như một công cụ Bảo mật và Tối ưu Hiệu suất
Phiên chia sẻ này cực kỳ liên quan đến công việc của tôi trong dự án RecruitPro. Mặc dù tôi đã biết CloudFront được sử dụng để lưu bộ nhớ đệm (caching) nội dung tại các edge location, tôi mới học được rằng nó cũng quan trọng không kém trong việc bảo mật và tối ưu hóa chi phí. Bằng cách tích hợp với AWS WAF và AWS Shield, cùng với việc bắt buộc sử dụng HTTPS, CloudFront hoạt động như một lá chắn vững chắc, đảm bảo máy chủ gốc (origin server) hiếm khi bị phơi nhiễm trực tiếp với lưu lượng truy cập internet.

### Chiến lược Hackathon: Ít nhưng chất (Less is More)
Team VIB đã chia sẻ hành trình xây dựng "UTMorpho" trong suốt 36 giờ của sự kiện LotusHacks. Họ đã phải vật lộn với giới hạn token, sự mệt mỏi và kết quả đầu ra không đáng tin cậy của AI. Bước đột phá của họ đến khi họ ngừng cố gắng xây dựng một bộ tính năng đồ sộ và thay vào đó tập trung vào việc hoàn thiện một tính năng chỉnh sửa cốt lõi duy nhất. Điều này dạy cho tôi rằng việc trình diễn một chức năng duy nhất, chỉn chu và hoạt động mượt mà sẽ tốt hơn rất nhiều so với việc mang đến một ứng dụng cồng kềnh, nhiều tính năng nhưng lại đầy lỗi.

### Sự khó lường ngay cả ở mức Temperature Zero
Một trong những sự thật đáng ngạc nhiên nhất mà tôi học được là việc cài đặt temperature của LLM về 0 không đảm bảo 100% các câu trả lời sẽ giống hệt nhau ở mọi lần. Các yếu tố như kiến trúc GPU, tính toán song song và quá trình phân lô (batching) có thể tạo ra những sai số nhỏ. Do đó, đối với các hệ thống production (môi trường thực tế), chúng ta phải dựa vào các ràng buộc nghiêm ngặt (như định dạng JSON) và việc xác thực đầu ra một cách mạnh mẽ thay vì mặc định cho rằng hành vi của mô hình là hoàn toàn mang tính tất định.

### Quản lý luồng công việc Multi-Agent trong doanh nghiệp
Sử dụng quy trình đánh giá tín dụng của một startup làm ví dụ thực tế, phiên chia sẻ này đã chứng minh cách các tác nhân AI (AI agents) khác nhau (xử lý tài chính, rủi ro, phân tích đội ngũ, v.v.) có thể cộng tác dưới quyền của một agent "quản lý". Mặc dù sự chuyên môn hóa này giúp tăng tốc độ xử lý các tác vụ phức tạp, việc triển khai một hệ thống như vậy trong một doanh nghiệp thực tế đòi hỏi các rào chắn (guardrails) cực kỳ nghiêm ngặt. Hệ thống cần có nhật ký kiểm toán (audit logs) toàn diện, các biện pháp bảo vệ quyền riêng tư dữ liệu và sự giám sát của con người — điều này làm nổi bật khoảng cách rất lớn giữa một bản demo AI đơn giản và một hệ thống sẵn sàng đưa vào vận hành thực tế.

## Những hành động có thể áp dụng ngay

- Chỉ cung cấp cho mô hình AI ngữ cảnh có tính mục tiêu cao, tránh việc đẩy toàn bộ dữ liệu vào (data dumps).
- Rõ ràng về kết quả mong muốn, định dạng và các ràng buộc khi viết prompt.
- Tận dụng CloudFront không chỉ để tăng tốc độ mà còn để che giấu và bảo vệ máy chủ gốc.
- Trong các dự án có thời gian hạn hẹp, ưu tiên xây dựng một tính năng cốt lõi thật vững chắc thay vì nhiều tính năng chưa hoàn thiện.
- Không bao giờ mặc định rằng đầu ra của LLM là cố định; luôn phải lập trình để xác thực lại kết quả.
- Đảm bảo ranh giới phân quyền nghiêm ngặt và kiểm toán chặt chẽ khi triển khai các công cụ AI Agent.

## Ứng dụng vào dự án RecruitPro

Những kiến thức về CloudFront có thể áp dụng ngay lập tức vào dự án RecruitPro của tôi. Tôi dự định sẽ cấu hình lại chiến lược caching của dự án, hạn chế quyền truy cập trực tiếp vào backend origin và tìm hiểu thêm về việc tích hợp AWS WAF. Ngoài ra, khi triển khai các tính năng AI, tôi sẽ áp dụng một cách tiếp cận nghiêm ngặt hơn nhiều đối với việc cấu trúc prompt và xác thực đầu ra để đảm bảo độ tin cậy cho toàn hệ thống.

## Minh chứng tham gia

![My photo at FCAJ Community Day](</images/4-EventParticipated/4.1-Event1/Picture1.png>)

![Photo taken during the event](</images/4-EventParticipated/4.1-Event1/picture2.jpg>)

## Kết luận

Việc tham dự FCAJ Community Day thực sự là một trải nghiệm vô cùng đáng giá. Sự kiện mang đến sự kết hợp hoàn hảo giữa các phương pháp thực hành tốt nhất về hạ tầng đám mây (CloudFront) và các chiến lược phát triển AI thực tế (hành vi của LLM và quản trị Multi-Agent). Hiện tại, tôi đã hiểu rõ ràng hơn rằng AI trong thế giới thực đòi hỏi sự kiểm soát và xác thực cực kỳ khắt khe, đây cũng là những khái niệm mà tôi rất háo hức được áp dụng trong các dự án hiện tại và tương lai của mình.