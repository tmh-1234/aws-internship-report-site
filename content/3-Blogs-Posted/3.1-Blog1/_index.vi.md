---
title: "Blog 1"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.1. </b> "
---
# Quá trình hoàn thiện kiến trúc Serverless cho dự án GreenLens Kids qua những kinh nghiệm thực tế

Chào mọi người, chúng mình là Nhóm We Are One tham gia chương trình First Cloud AI Journey của AWS. Hôm nay, mình muốn chia sẻ với cộng đồng một vài kinh nghiệm thực chiến khi thiết kế kiến trúc hệ thống cho GreenLens Kids. Đây là dự án nhóm mình xây dựng dựa trên AWS Serverless, ứng dụng AI và Gamification để hướng dẫn trẻ em phân loại rác.

Dưới đây là những bài học cốt lõi nhóm đúc kết được sau các phiên technical review với ban cố vấn và tiến hành tinh chỉnh lại sơ đồ ban đầu.

---

## 1. Rủi ro an ninh ẩn sau mục tiêu tối ưu hóa trải nghiệm

Để các bé thao tác dễ dàng nhất, nhóm ban đầu quyết định bỏ qua bước đăng nhập. Tuy nhiên, các anh chị Mentor đã phân tích một lỗ hổng chí mạng. Việc thiếu đi cơ chế xác thực sẽ khiến các endpoint, đặc biệt là AI Camera, rất dễ bị lạm dụng hoặc gặp tình trạng tấn công từ chối dịch vụ. Hậu quả là dự án có thể cạn kiệt ngân sách tài nguyên AWS một cách nhanh chóng. Để khắc phục, nhóm đã triển khai Guest Access của AWS Cognito nhằm định danh thiết bị an toàn, kết hợp thêm AWS WAF phía sau API Gateway để kiểm soát lưu lượng và chặn các request độc hại.

---

## 2. Khắc phục sự phân mảnh trong quy hoạch luồng dữ liệu

Kiến trúc ban đầu của nhóm thiết lập các Lambda function khá rời rạc chỉ để kết nối với kho lưu trữ S3. Luồng quản trị hệ thống cũng bị tách biệt hoàn toàn khỏi cơ sở dữ liệu chung khiến tổng thể trở nên thiếu đồng bộ. Nhờ những đánh giá chuyên môn chi tiết, nhóm đã quy hoạch lại toàn bộ sơ đồ theo các tầng chuẩn chỉnh để dễ quản lý và mở rộng hơn, bao gồm Presentation Layer, API Layer, Application Layer, Data Layer và External AI Services.

---

## 3. Hiểu đúng về cơ chế điều phối của các dịch vụ AWS

Ở phiên bản sơ khai, nhóm đã thiết kế luồng xử lý để Amazon Rekognition và Amazon Bedrock tự động tương tác trực tiếp với nhau, đồng thời đặt thêm Amazon ElastiCache vào luồng một cách thiếu hợp lý. Sau khi nghiên cứu kỹ lại tài liệu kỹ thuật, nhóm quyết định tinh gọn toàn bộ hệ thống. AWS Lambda được đưa về đúng bản chất của một kiến trúc Serverless hướng sự kiện, đóng vai trò trung tâm điều phối logic giữa ứng dụng và các dịch vụ AI bên ngoài.

---

## Bài học rút ra và kết luận

Trải qua quá trình liên tục rút kinh nghiệm, sửa chữa và hoàn thiện, cả team mới thực sự nhận ra rằng thiết kế architecture không chỉ đơn thuần là kết nối các service lại với nhau để đáp ứng đủ tính năng. Bài toán cốt lõi và cũng thách thức nhất luôn nằm ở việc tìm ra điểm trade-off hợp lý giữa trải nghiệm người dùng, khả năng tối ưu chi phí và giới hạn bảo mật của toàn hệ thống.

Xin gửi lời cảm ơn chân thành đến ban tổ chức First Cloud AI Journey cùng các anh chị Mentor đã luôn tận tâm theo sát dự án. Những review khắt khe nhưng bám sát thực tế đã giúp nhóm củng cố nền tảng tư duy vững chắc, giúp tụi mình tự tin và sẵn sàng hơn cho các dự án thực tiễn sắp tới.
![alt text](../architecture.png)