---
title: "Sự kiện 4: FCAJ Meetup 25/07/2026 (Buổi 2)"
date: 2026-07-25
weight: 4
chapter: false
pre: " <b> 4.4. </b> "
---

# BÁO CÁO THU HOẠCH: SỰ KIỆN FCAJ MEETUP - 25/07/2026 (BUỔI 2)

### 1. Mục đích và ý nghĩa của việc tham gia sự kiện
- **Mục đích:** Nghiên cứu sâu về các chủ đề Operations (giám sát CloudWatch, log retention) và Cloud Security (IAM Least Privilege, AWS WAF rules, CI/CD deployment pipelines).
- **Ý nghĩa:** Định hình tư duy DevOps chuyên nghiệp và đảm bảo các tiêu chuẩn bảo mật chuẩn doanh nghiệp cho hệ thống Budget Tracker.

### 2. Danh sách diễn giả khách mời
- **Anh Nguyễn Gia Hưng:** AWS Solution Architect, Mentor trưởng tại FCAJ.
- **Anh Hoàng Trọng:** Senior Cloud Engineer, chuyên gia bảo mật đám mây.
- **Thành viên nhóm CCK:** Thảo luận về phương pháp tích hợp CI/CD và quy tắc bảo mật.

### 3. Tổng hợp nội dung nổi bật từ các phiên chia sẻ
#### 3.1 Giám sát hệ thống và Quản lý Logs (AWS CloudWatch)
- **Giải pháp:** Thiết lập CloudWatch Dashboard để giám sát hiệu năng CPU, RAM của EC2 và số lượng request, thời gian thực thi của AWS Lambda.
- **Tối ưu:** Cấu hình Log Retention Policy trong 14 ngày thay vì vô hạn nhằm giảm chi phí lưu trữ không đáng có.

#### 3.2 Bảo mật hạ tầng Cloud và CI/CD Pipeline
- **Bảo mật:** Cấu hình các rules trên AWS WAF bảo vệ API Gateway khỏi các cuộc tấn công SQL Injection và Cross-Site Scripting (XSS). Thiết lập IAM Roles theo nguyên tắc Least Privilege (quyền tối thiểu).
- **CI/CD:** Xây dựng GitHub Actions workflow để tự động đóng gói, chạy unit test và deploy code backend lên AWS Lambda mỗi khi có commit mới trên nhánh main.

### 4. Kiến thức và kỹ năng ghi nhận được
- **Kiến thức:** Nắm rõ cách quản lý log, thiết lập cảnh báo CloudWatch Alarm và cơ chế hoạt động của WAF. Hiểu luồng hoạt động của CI/CD pipeline.
- **Kỹ năng:** Cấu hình an toàn bảo mật cho tài nguyên AWS và tự động hóa quy trình triển khai sản phẩm.

### 5. Một số hình ảnh ghi nhận tại sự kiện (Buổi 2)

<div style="display: flex; gap: 10px; flex-wrap: wrap;">
  <img src="/images/event/event25072026/z8081559005936_2ddf7e0e613c84763453dd6c592aba3d.jpg" width="45%" />
  <img src="/images/event/event25072026/z8081559011917_e254dd8712e70611fe2d4626917cf471.jpg" width="45%" />
</div>

---

### 6. Bài học rút ra & Đánh giá chung
- **Bài học:** Một sản phẩm tốt không chỉ cần chạy đúng tính năng mà còn cần được giám sát hiệu quả và bảo vệ an toàn trước các nguy cơ tấn công mạng.
- **Đánh giá:** Buổi học trang bị đầy đủ các kỹ năng thực tế về vận hành (Ops) và bảo mật (Security), giúp nhóm tự tin vận hành ứng dụng trên Cloud.
