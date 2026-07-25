---
title: "Sự kiện 3 và 4: FCAJ Meetup 25/07/2026 (Sự kiện này được tính là 2 buổi tham gia)"
date: 2026-07-25
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# BÁO CÁO THU HOẠCH: SỰ KIỆN FCAJ MEETUP - 25/07/2026 (TÍNH CHO 2 BUỔI)

### 1. Mục đích và ý nghĩa của việc tham gia sự kiện
- **Mục đích:** Nghiên cứu các giải pháp AI thực tiễn (Generative AI), mô hình thiết kế cơ sở dữ liệu phi quan hệ (NoSQL Single Table Design), cùng quy trình vận hành và bảo mật hạ tầng trên AWS (CloudWatch, CI/CD, WAF).
- **Ý nghĩa:** Tiếp thu các kiến thức thực tế từ chuyên gia để hoàn thiện hệ thống, tối ưu hóa database và xây dựng các lớp bảo vệ chuẩn doanh nghiệp cho sản phẩm **Budget Tracker**.

### 2. Danh sách diễn giả khách mời
- **Anh Nguyễn Gia Hưng:** AWS Solution Architect, Mentor trưởng tại FCAJ.
- **Anh Hoàng Trọng:** Senior Cloud Engineer, chuyên gia bảo mật và cơ sở dữ liệu.
- **Thành viên nhóm CCK:** Thảo luận, báo cáo tiến độ và demo các giải pháp kỹ thuật.

### 3. Tổng hợp nội dung nổi bật từ các phiên chia sẻ

#### 3.1 Ứng dụng Generative AI & Tối ưu DynamoDB (Nội dung Buổi 1)
- **Generative AI:** Kết hợp **Google Gemini API** và AWS Lambda để phân tích tự động các giao dịch chi tiêu thô của người dùng thành cấu trúc JSON định dạng chuẩn.
- **Single Table Design:** Gộp chung tất cả các entities (Users, Transactions, Budgets) vào một bảng DynamoDB duy nhất. Cấu hình PK/SK và GSIs tối ưu để giảm thiểu thao tác quét bảng (Scan), nâng cao tốc độ truy xuất dữ liệu.

#### 3.2 Vận hành, Bảo mật Cloud & CI/CD Pipeline (Nội dung Buổi 2)
- **Giám sát (AWS CloudWatch):** Thiết lập dashboard theo dõi tài nguyên EC2/Lambda và cấu hình chính sách lưu giữ logs (Log Retention) trong 14 ngày để tiết kiệm chi phí.
- **Bảo mật và CI/CD:** Cấu hình rules trên AWS WAF ngăn chặn các tấn công SQLi/XSS vào API Gateway. Đồng thời thiết lập GitHub Actions workflow tự động chạy test và deploy code backend Lambda mỗi khi có thay đổi trên repository.

### 4. Kiến thức và kỹ năng ghi nhận được
- **Tư duy hệ thống:** Khả năng kết hợp linh hoạt giữa các mô hình lưu trữ NoSQL và dịch vụ AI trong một kiến trúc Serverless gọn nhẹ.
- **Kỹ năng thực thi:** Cách thức thiết lập hạ tầng bảo mật an toàn, tự động hóa quy trình phân phối sản phẩm (CI/CD) và giám sát trạng thái hệ thống.

### 5. Một số hình ảnh ghi nhận tại sự kiện (2 buổi)

<div style="display: flex; gap: 10px; flex-wrap: wrap;">
  <img src="/images/event/event25072026/z8081558998082_592cfa3f54a416ce19c1f478f9736317.jpg" width="45%" />
  <img src="/images/event/event25072026/z8081559005717_afd71e384ff8ac57e2aeb1bd2dd72d11.jpg" width="45%" />
  <img src="/images/event/event25072026/z8081559005936_2ddf7e0e613c84763453dd6c592aba3d.jpg" width="45%" />
  <img src="/images/event/event25072026/z8081559011917_e254dd8712e70611fe2d4626917cf471.jpg" width="45%" />
</div>

---

### 6. Bài học rút ra & Đánh giá chung
- **Bài học:** Một hệ thống Cloud hoàn chỉnh cần đáp ứng tốt cả 3 yếu tố: Tính năng (AI/DB), Vận hành tối ưu (Operations/CI/CD) và Bảo mật nghiêm ngặt (Security).
- **Đánh giá:** Buổi học tích hợp 2-trong-1 rất bổ ích, cung cấp trọn vẹn bức tranh thực tế về quy trình phát triển và vận hành phần mềm trên môi trường Cloud chuyên nghiệp.
