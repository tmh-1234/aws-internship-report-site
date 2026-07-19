---
title: "Blog 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.2. </b> "
---
# Hành trình phát triển tầng ứng dụng Cloud cùng First Cloud AI Journey

Dù đã được trang bị nền tảng công nghệ thông tin từ chương trình đào tạo tại trường, việc đối mặt với bài toán triển khai một hệ thống serverless trên môi trường AWS vẫn mang lại vô vàn bỡ ngỡ. Nhờ tham gia chương trình First Cloud AI Journey, nhóm We Are One chúng mình mới có cơ hội chuyển từ những mớ lý thuyết khô khan trên giảng đường sang việc làm một dự án cloud thực tế với nhiều bài toán hóc búa.

## 1. Xây dựng nền móng từ những bước cơ bản nhất

Hành trình của nhóm không bắt đầu bằng những dòng code phức tạp, mà từ những bước làm quen với hệ sinh thái AWS. Những ngày đầu tiên là khoảng thời gian chật vật với việc thiết lập tài khoản AWS Free Tier, thậm chí phải tạo các support case để giải quyết lỗi không xác thực được số điện thoại và thẻ thanh toán.

Nhóm đã cùng nhau học qua các module của AWS Study Group, hoàn thành hàng loạt bài lab thực hành AWS SimuLearn từ Cloud Computing Essentials, NoSQL Database cho đến Core Security Concepts. Quá trình này giúp cả đội hoàn thành trọn vẹn 12 bài lab và lấy được chứng chỉ AWS Cloud Practitioner, tạo bước đệm vững chắc để tiến lên tầng ứng dụng.

## 2. Tiến vào tầng ứng dụng và giải quyết bài toán kiến trúc cục bộ

Thay vì chỉ thao tác trên giao diện Console, nhóm bắt đầu nghiên cứu sâu hơn về kiến trúc FastAPI kết hợp AWS và thiết lập giải pháp giả lập môi trường cloud ngay trên local. Những kiến thức mới liên tục được áp dụng như xây dựng Dockerfile tối ưu và cấu hình `docker-compose.yml` tích hợp container DynamoDB Local.

Nhóm cũng học cách thiết lập Docker Networking và Docker Volumes để lưu trữ dữ liệu DB bền vững. Đi kèm với đó là việc quản lý biến môi trường an toàn và sử dụng thư viện Boto3 để viết mã nguồn kết nối, thiết kế Data Schema cho các luồng xử lý cốt lõi như tính điểm XP hay cập nhật trạng thái người dùng. Quá trình này giúp cả nhóm hiểu rõ cách một ứng dụng backend giao tiếp với hạ tầng cloud, cách đóng gói ứng dụng và tư duy chuẩn hóa dữ liệu.

## 3. Vượt qua những sự cố thực tế

Làm dự án đồng nghĩa với việc phải đối mặt với những rủi ro không lường trước. Một sự cố đáng nhớ là khi hệ thống API đột ngột ngừng phản hồi. Sau khi phân tích, nhóm phát hiện nguyên nhân là do tài khoản AWS chính đã cạn kiệt Free Credit. Cả đội phải nhanh chóng khởi tạo môi trường cloud mới, thiết lập lại các quyền IAM, chuyển đổi toàn bộ tài nguyên hạ tầng và khắc phục các lỗi Access Denied phát sinh.

Bên cạnh đó, nhóm cũng dành nhiều thời gian gỡ lỗi các vấn đề như không đồng bộ trạng thái nhân vật giữa DynamoDB và giao diện ứng dụng, hay việc xử lý sai lệch định dạng JSON giữa backend và frontend.

## 4. Nâng tầm trải nghiệm người dùng với các dịch vụ AI

Quá trình học hỏi tại FCAJ đạt đến độ chín khi nhóm bắt đầu tích hợp các dịch vụ AI vào luồng xử lý. Trong tính năng AI Camera, nhóm không chỉ xử lý logic nhận diện ảnh mà còn trực tiếp phối hợp với frontend để tối ưu hóa UX. Cụ thể, tụi mình đã hỗ trợ ánh xạ dữ liệu phức tạp từ backend sang giao diện màn hình kết quả.

Ngoài ra, nhóm còn đề xuất và tích hợp thành công Web Speech API để tạo giọng nói cho linh vật, tự động ghép chuỗi văn bản hướng dẫn tái chế để đọc kết quả cho các bé. Việc render động các thẻ nội dung giáo dục về tác động môi trường dựa trên dữ liệu JSON trả về cũng được xử lý mượt mà.

## Kết luận

Chương trình First Cloud AI Journey không chỉ cung cấp tài nguyên, mà còn là một môi trường để nhóm áp dụng kiến thức vào thực tế. Từ những sinh viên chỉ quen với code trên máy tính cá nhân, nay chúng mình đã biết cách thiết kế kiến trúc, xử lý lỗi hạ tầng, và tích hợp AI để giải quyết một bài toán giáo dục môi trường trọn vẹn. Xin gửi lời cảm ơn chân thành đến ban tổ chức và các anh chị mentor đã tạo ra một sân chơi học tập vô giá.
