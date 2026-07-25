---
title: "Sự kiện 3: FCAJ Meetup 25/07/2026 (Buổi 1)"
date: 2026-07-25
weight: 3
chapter: false
pre: " <b> 4.3. </b> "
---

# BÁO CÁO THU HOẠCH: SỰ KIỆN FCAJ MEETUP - 25/07/2026 (BUỔI 1)

### 1. Mục đích và ý nghĩa của việc tham gia sự kiện
- **Mục đích:** Nghiên cứu và trao đổi về các công nghệ AI tiên tiến (Generative AI) và phương pháp tối ưu hóa cơ sở dữ liệu phi quan hệ (NoSQL Single Table Design) trên môi trường AWS thực tế.
- **Ý nghĩa:** Tiếp thu kinh nghiệm thực chiến từ các Mentor để hoàn thiện chức năng phân tích chi tiêu thông minh cho dự án **Budget Tracker**.

### 2. Danh sách diễn giả khách mời
- **Anh Nguyễn Gia Hưng:** AWS Solution Architect, Mentor trưởng tại FCAJ.
- **Anh Hoàng Trọng:** Senior Cloud Engineer, chuyên gia về giải pháp cơ sở dữ liệu.
- **Thành viên nhóm CCK:** Báo cáo tiến độ và demo các giải pháp AI tích hợp.

### 3. Tổng hợp nội dung nổi bật từ các phiên chia sẻ
#### 3.1 Ứng dụng Generative AI trong Fintech
- **Công nghệ:** Sử dụng **Google Gemini API** kết hợp với AWS Lambda để xử lý và phân loại tự động các giao dịch tài chính dựa trên mô tả thô.
- **Giải pháp:** Thiết lập prompt tối ưu để AI trả về định dạng JSON chuẩn giúp frontend dễ dàng render biểu đồ chi tiêu mà không tốn công xử lý thủ công.

#### 3.2 Tối ưu hóa Database với DynamoDB Single Table Design
- **Phương pháp:** Thay vì thiết kế nhiều bảng quan hệ, nhóm gộp chung tất cả các entity (Users, Transactions, Budgets) vào một bảng duy nhất nhằm giảm số lượng request đọc/ghi và tiết kiệm chi phí vận hành.
- **Kỹ thuật:** Định nghĩa rõ ràng PK/SK và tạo thêm các Global Secondary Indexes (GSIs) để hỗ trợ các truy vấn lọc động.

### 4. Kiến thức và kỹ năng ghi nhận được
- **Kiến thức:** Hiểu rõ cơ chế hoạt động và cách tối ưu hóa chi phí gọi Gemini API. Nắm chắc nguyên lý hoạt động của Single Table Design trên DynamoDB.
- **Kỹ năng:** Có khả năng thiết kế mô hình khóa chính/khóa phụ tối ưu cho các bài toán truy xuất dữ liệu lớn.

### 5. Một số hình ảnh ghi nhận tại sự kiện (Buổi 1)

<div style="display: flex; gap: 10px; flex-wrap: wrap;">
  <img src="/images/event/event25072026/z8081558998082_592cfa3f54a416ce19c1f478f9736317.jpg" width="45%" />
  <img src="/images/event/event25072026/z8081559005717_afd71e384ff8ac57e2aeb1bd2dd72d11.jpg" width="45%" />
</div>

---

### 6. Bài học rút ra & Đánh giá chung
- **Bài học:** Việc tối ưu hóa cấu trúc cơ sở dữ liệu ngay từ ban đầu đóng vai trò cực kỳ quan trọng đối với khả năng chịu tải và chi phí của các ứng dụng Serverless.
- **Đánh giá:** Buổi học mang tính thực tiễn cao, giúp nhóm giải quyết được nút thắt lớn trong việc thiết kế database cho sản phẩm.
