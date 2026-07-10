---
title: "Bản đề xuất"
date: 2026-07-09
weight: 2
chapter: false
pre: " <b> 2. </b> "
---

# Budget Tracker
## Personal Finance Management Web Application
### AI-Powered Expense Tracking & Financial Intelligence
**Báo cáo Dự Án AWS Serverless + Google Gemini AI**

---

### 1. Tóm tắt điều hành
**Budget Tracker** là một ứng dụng quản lý tài chính cá nhân được thiết kế để giúp người dùng theo dõi thu nhập, chi tiêu và ngân sách. Ứng dụng tích hợp trí tuệ nhân tạo (AI) qua **Google Gemini API** để tự động phân loại giao dịch, phân tích chi tiêu và đưa ra gợi ý tài chính thông minh. Nền tảng được xây dựng trên kiến trúc **AWS Serverless**, đảm bảo tính mở rộng cao, chi phí vận hành thấp và độ tin cậy tối đa.

Ứng dụng cung cấp:
- Dashboard theo dõi tài chính thời gian thực.
- Quản lý giao dịch với tính năng upload hóa đơn.
- Thiết lập và theo dõi ngân sách theo danh mục.
- Báo cáo chi tiêu với biểu đồ phân tích.
- Chatbot AI để tư vấn tài chính và trả lời câu hỏi.
- Thông báo thông minh qua email (vượt ngân sách, chi tiêu bất thường).

---

### 2. Tuyên bố vấn đề
#### 2.1 Vấn Đề Hiện Tại
Người dùng hiện tại gặp nhiều thách thức khi quản lý tài chính cá nhân:
- Phải nhập dữ liệu chi tiêu thủ công, tốn thời gian.
- Khó phân loại giao dịch một cách nhất quán.
- Thiếu cái nhìn sâu sắc về các thói quen chi tiêu.
- Không có hệ thống cảnh báo khi vượt ngân sách.
- Khó nhận được lời khuyên tài chính được cá nhân hóa.

#### 2.2 Giải Pháp Đề Xuất
Budget Tracker cung cấp giải pháp toàn diện bằng cách:
- Tự động phân loại giao dịch bằng AI (Google Gemini).
- Hiển thị dashboard trực quan với dữ liệu thời gian thực.
- Phân tích chi tiêu tự động và phát hiện xu hướng.
- Gửi cảnh báo khi chi tiêu vượt ngân sách.
- Cung cấp chatbot AI tư vấn tài chính 24/7.
- Hoạt động trên AWS Serverless (chi phí thấp, độ tin cậy cao).

#### 2.3 Lợi Ích & Giá Trị
- Tiết kiệm 5-10 giờ/tháng nhập dữ liệu thủ công.
- Cải thiện kỷ luật tài chính nhờ cảnh báo tự động.
- Phát hiện cơ hội tiết kiệm qua phân tích chi tiêu.
- Đạt mục tiêu tài chính nhanh hơn nhờ lời khuyên AI.
- Giao diện thân thiện, dễ sử dụng cho mọi cấp độ.

*Chi phí & ROI:*
- Chi phí phát triển ước tính: $5,000 - $8,000 (một lần).
- Chi phí vận hành hàng tháng: $50-100 USD (AWS + Gemini).
- ROI: Nếu là dự án thương mại (freemium model), hoàn vốn trong 6-12 tháng.

---

### 3. Kiến trúc giải pháp
Budget Tracker sử dụng kiến trúc AWS Serverless với tích hợp Google Gemini API, được thiết kế cho khả năng mở rộng, chi phí tối ưu và độ tin cậy cao.

![Budget Tracker Architecture](/images/2-Proposal/sodo.jpg)

#### 3.1 Stack Công Nghệ
- **Frontend:** ReactJS + Tailwind CSS (Giao diện web hiện đại, responsive).
- **Backend:** C# .NET 8 (ASP.NET Core) Lambda functions xử lý business logic.
- **Database:** Amazon DynamoDB (NoSQL) lưu trữ dữ liệu người dùng, giao dịch, ngân sách.
- **API Gateway:** Amazon API Gateway (REST) định tuyến request tới Lambda functions.
- **Authentication:** Amazon Cognito + JWT xác thực người dùng an toàn.
- **Storage:** Amazon S3 lưu trữ hóa đơn và tệp đính kèm.
- **Queue:** Amazon SQS xử lý bất đồng bộ thông báo.
- **AI:** Google Gemini API phân loại giao dịch, phân tích chi tiêu, chatbot.
- **Notifications:** Amazon SNS gửi email thông báo tới người dùng.
- **Monitoring:** Amazon CloudWatch logging, metrics, alarms.
- **CDN:** Amazon CloudFront phân phối nội dung tĩnh nhanh.
- **DNS:** Amazon Route 53 quản lý tên miền.
- **Security:** AWS WAF bảo vệ chống DDoS, SQL injection, XSS.

#### 3.2 Quy Trình Kiến Trúc
1. Route 53 giải quyết tên miền.
2. CloudFront phân phối React app (HTML, CSS, JS) từ S3.
3. React app gọi API Gateway qua Axios.
4. API Gateway định tuyến tới Lambda C# .NET 8.
5. Lambda xử lý request: xác thực qua Cognito, đọc/ghi DynamoDB, gọi Gemini API.
6. Xử lý bất đồng bộ: Lambda gửi thông báo vào SQS -> SNS gửi email.
7. CloudWatch theo dõi logs và metrics.

---

### 4. Triển khai kỹ thuật
#### 4.1 Các Giai Đoạn Phát Triển
- **Giai Đoạn 1: Nghiên Cứu & Thiết Kế Kiến Trúc** (2 tuần): Thiết kế kiến trúc AWS, chọn tech stack, tạo wireframe.
- **Giai Đoạn 2: Setup & Cơ Sở Hạ Tầng** (2 tuần): Cấu hình AWS services (DynamoDB, S3, Lambda, Cognito), thiết lập CI/CD.
- **Giai Đoạn 3: Phát Triển Backend & Frontend** (6-8 tuần): Xây dựng Lambda handlers (C# .NET 8), React components, tích hợp Gemini API.
- **Giai Đoạn 4: Kiểm Thử & Triển Khai** (3-4 tuần): Unit tests, integration tests, UAT, triển khai production.

#### 4.2 Yêu Cầu Kỹ Thuật Chi Tiết
- **Frontend (ReactJS):** JavaScript, React Hooks, Context API / Zustand, Tailwind CSS, Axios, Recharts.
- **Backend (C# .NET 8):** ASP.NET Core Web API trên AWS Lambda, DynamoDB context, FluentValidation, Dependency Injection & Async/await.

---

### 5. Lộ trình & Mốc triển khai
- Tuần 1-2: Thiết kế kiến trúc, wireframe.
- Tuần 3-4: Cấu hình AWS, CI/CD, repo.
- Tuần 5-7: Lambda handlers cơ bản, DynamoDB, Dashboard, Transactions page (MVP).
- Tuần 8-10: Tích hợp Gemini, notifications, Budgets, Reports, AI Chatbox.
- Tuần 11-12: Unit tests, integration tests, UAT (70%+ coverage).
- Tuần 13: Triển khai production, monitoring.

---

### 6. Ước tính ngân sách
*Chi phí phát triển:*
- Backend: 160 giờ ($8,000)
- Frontend: 120 giờ ($5,400)
- DevOps: 40 giờ ($2,200)
- Testing & QA: 60 giờ ($2,700)
- PM: 30 giờ ($1,800)
- Documentation: 20 giờ ($800)
- **TỔNG CỘNG:** 430 giờ - $21,700

*Chi phí vận hành hàng tháng:*
- AWS Lambda: $5
- DynamoDB: $8
- S3: $2
- CloudFront: $3
- API Gateway: $2
- CloudWatch: $1
- Cognito: $0 (Free Tier)
- SNS: $1
- Gemini API: $20
- Route 53 & Others: $2
- **TỔNG CỘNG:** $44/tháng ($528/năm)

---

### 7. Đánh giá rủi ro & Giảm thiểu
- **Vượt timeline:** Sử dụng Agile sprint 2 tuần, standup hàng ngày, ưu tiên MVP trước.
- **Lỗi AI Gemini:** Cho phép người dùng chỉnh sửa category được gợi ý, fallback về "Other" nếu lỗi.
- **Lỗi bảo mật:** AWS WAF bảo vệ DDoS, Cognito xử lý authentication, mã hóa dữ liệu TLS.

---

### 8. Kỳ vọng & Kết quả
- Tự động hóa phân loại giao dịch bằng AI với độ chính xác >= 95%.
- Dashboard thời gian thực, thời gian tải trang < 2 giây.
- Chatbot AI tư vấn tài chính hoạt động 24/7.
- Khả năng mở rộng tới hàng triệu người dùng nhờ kiến trúc Serverless.
