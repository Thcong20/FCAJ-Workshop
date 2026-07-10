---
title: "Sự kiện 1: FCAJ Meetup 13/06/2026"
date: 2026-07-09
weight: 1
chapter: false
pre: " <b> 4.1. </b> "
---

# BÁO CÁO THU HOẠCH: SỰ KIỆN FCAJ MEETUP - 13/06/2026

### 1. Mục đích và ý nghĩa của việc tham gia sự kiện
- **Mục đích:** Kết nối với cộng đồng kỹ sư công nghệ, tiếp cận các giải pháp thực tế về thiết kế hệ thống có khả năng mở rộng (Scalable Systems) và tối ưu hóa hạ tầng trên đám mây (AWS).
- **Ý nghĩa:** Giúp chuyển hóa kiến thức lý thuyết thành tư duy thực chiến trong phát triển phần mềm hiện đại và định hướng giải quyết các bài toán kỹ thuật phức tạp của doanh nghiệp.

### 2. Danh sách diễn giả khách mời
- **Anh Đạt & Anh Cường:** Các chuyên gia tư vấn giải pháp Cloud (AWS Solution Architects).
- **Anh Hoàng Trọng:** Kỹ sư hệ thống cấp cao (Senior Systems Engineer) chuyên sâu về tối ưu hiệu năng.
- **Kiên & Thọ:** Đại diện nhóm kỹ thuật, chia sẻ dự án thực tế.
- **Hiếu Nghị:** Điều phối viên.

### 3. Tổng hợp nội dung nổi bật từ các phiên chia sẻ
#### 3.1 Thiết kế và tối ưu hóa hệ thống (Case Study: URL Shortening Service)
- **Vấn đề:** Thiết kế dịch vụ rút gọn đường dẫn chịu tải cao, độ trễ thấp khi truy cập tăng đột biến.
- **Giải pháp:** Sử dụng hạ tầng Serverless AWS: DynamoDB (lưu trữ Key-Value tốc độ cao), API Gateway và AWS Lambda giúp tự động mở rộng (Scalability) và tối ưu chi phí.

#### 3.2 Tư duy thiết kế hệ thống hiện đại
- **Loose Coupling (Giảm sự phụ thuộc):** Chuyển từ gọi API đồng bộ sang kiến trúc hướng sự kiện (Event-driven Architecture).
- **Caching Strategy:** Sử dụng các chiến lược cache để giảm tải cho DB và tăng tốc phản hồi.

### 4. Kiến thức và kỹ năng ghi nhận được
- **Tư duy kỹ thuật:** Biết cách lựa chọn giải pháp phù hợp giữa EC2, ECS/Fargate hay Serverless Lambda tùy nhu cầu.
- **Kỹ năng thực thi:** Cách sử dụng Infrastructure as Code (IaC) để tự động hóa triển khai hạ tầng.
- **Tư duy giải quyết vấn đề:** Sự cân bằng giữa tính năng, chi phí vận hành và khả năng bảo trì.

### 5. Một số hình ảnh ghi nhận tại sự kiện

<div style="display: flex; gap: 10px; flex-wrap: wrap;">
  <img src="/images/event/event13062026/z8026049403589_0707f922b7486e821c8c55e8772dbc14.jpg" width="30%" />
  <img src="/images/event/event13062026/z8026049412780_47148cba587d835d2dc0517c08af21ca.jpg" width="30%" />
  <img src="/images/event/event13062026/z8026049416705_087c02494abbc6679f64a87a0d906bba.jpg" width="30%" />
</div>

---

### 6. Bài học rút ra & Đánh giá chung
- **Bài học:** "Sự linh hoạt là chìa khóa". Hệ thống cần được thiết kế để dễ dàng thích ứng với sự thay đổi của nghiệp vụ (Business-first).
- **Đánh giá:** Buổi Meetup cực kỳ bổ ích, giúp xóa nhòa khoảng cách giữa trường học và thực tế. Hy vọng các buổi tiếp theo sẽ có phần thực hành Hands-on code trực tiếp.
