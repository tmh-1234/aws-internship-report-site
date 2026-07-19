---
title: "Blog 3"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 3.3. </b> "
---
# Tổng kết hành trình xây dựng GreenLens Kids cùng First Cloud AI Journey

Chào mọi người, chúng mình là sinh viên CNTT từ HUTECH và VJIT, hiện đang tham gia chương trình First Cloud AI Journey. Qua hai bài viết trước, chúng mình đã chia sẻ chi tiết về quá trình tối ưu kiến trúc serverless và những kinh nghiệm khi xây dựng tầng ứng dụng. Ở bài blog thứ ba này, tụi mình muốn đúc kết lại toàn bộ chặng đường vừa qua và những giá trị cốt lõi mà nhóm đã tích lũy được từ lúc bắt đầu cho đến khi dự án hình thành.

## 1. Tư duy hệ thống quyết định chất lượng sản phẩm

Nhìn lại toàn bộ dự án, tụi mình nhận thấy một sơ đồ kiến trúc dù hoàn chỉnh đến đâu cũng sẽ trở nên vô nghĩa nếu thiếu đi năng lực triển khai. Những tính năng bảo mật hệ thống như AWS Cognito hay Web Application Firewall chỉ thực sự phát huy tác dụng khi nhóm nắm vững cách phân quyền IAM, quản lý biến môi trường an toàn và kiểm soát tốt tài nguyên sử dụng. Việc kết nối chặt chẽ giữa tư duy thiết kế tổng thể và kỹ năng lập trình chi tiết chính là chìa khóa giúp GreenLens Kids vận hành trơn tru và tối ưu chi phí.

## 2. Rèn luyện sự nhạy bén khi xử lý sự cố

Quá trình làm dự án mang lại cho nhóm rất nhiều bài học đắt giá qua những sự cố nằm ngoài dự tính. Từ việc xử lý tình huống cạn kiệt credit phải cấu hình lại môi trường cloud sang tài khoản mới, thiết lập mạng Docker để chạy DynamoDB nội bộ, cho đến những lúc cùng team frontend rà soát nguyên nhân không đồng bộ dữ liệu, chính những rào cản kỹ thuật này đã ép cả đội phải làm quen với việc đọc log hệ thống, khoanh vùng lỗi nhanh chóng và đưa ra giải pháp khắc phục triệt để.

## 3. Trưởng thành nhờ những đánh giá chuyên môn

Dự án chắc chắn sẽ không thể hoàn thiện nếu thiếu đi sự định hướng từ ban cố vấn. Những lời nhận xét nghiêm khắc, đi thẳng vào vấn đề của các mentor đã giúp nhóm thay đổi hoàn toàn cách tiếp cận công nghệ. Tụi mình rèn luyện được thói quen không bao giờ thỏa hiệp với rủi ro bảo mật, đồng thời luôn đặt bài toán chi phí lên bàn cân trước khi quyết định tích hợp bất kỳ dịch vụ mới nào vào hệ thống.

## Kết luận

Chương trình First Cloud AI Journey đã khép lại nhưng những trải nghiệm thu về thực sự là một hành trang quý giá. Nhóm đã có cơ hội trải qua một quy trình làm sản phẩm đầy đủ, từ khâu phác thảo sơ đồ, bảo mật hệ thống, xử lý lỗi hạ tầng cho đến tích hợp AI để hoàn thiện ứng dụng. Xin cảm ơn ban tổ chức, các mentor và toàn thể đồng đội đã cùng nhau nỗ lực vượt qua vô vàn thử thách kỹ thuật để đưa GreenLens Kids đến vạch đích.
