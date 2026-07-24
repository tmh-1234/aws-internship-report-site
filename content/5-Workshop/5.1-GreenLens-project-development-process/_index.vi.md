---
title: "Quy trình phát triển dự án GreenLens"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 5.1. </b> "
---

#### Tổng quan

Dự án GreenLens được phát triển bởi một nhóm bốn thành viên. Vinh giữ vai trò trưởng nhóm và phụ trách backend development, core business logic, quản lý tài khoản AWS, cấu hình các dịch vụ AWS, và triển khai hệ thống lên AWS. Lợi cũng tham gia vào phần backend, còn Phúc và tôi phụ trách frontend development.

#### Lưu ý

Phần này tóm tắt quy trình phát triển dự án và cách nhóm đã tổ chức công việc trong GreenLens. Nội dung được trình bày theo dạng một chương báo cáo để có thể chèn vào mục Workshop một cách thống nhất.

#### Nội dung

1. [Giới thiệu](#1-giới-thiệu)
2. [Chuẩn bị dự án](#2-chuẩn-bị-dự-án)
3. [Lập kế hoạch công việc và tổ chức triển khai](#3-lập-kế-hoạch-công-việc-và-tổ-chức-triển-khai)
4. [Phát triển Frontend](#4-phát-triển-frontend)
5. [Phát triển Backend](#5-phát-triển-backend)
6. [Thiết lập AWS và triển khai](#6-thiết-lập-aws-và-triển-khai)
7. [Kiểm thử và tích hợp](#7-kiểm-thử-và-tích-hợp)
8. [Phối hợp làm việc và quản lý mã nguồn](#8-phối-hợp-làm-việc-và-quản-lý-mã-nguồn)
9. [Rà soát cuối cùng và bàn giao](#9-rà-soát-cuối-cùng-và-bàn-giao)
10. [Kết luận](#10-kết-luận)

## 1. Giới thiệu

GreenLens là một dự án được xây dựng theo mô hình làm việc nhóm với trách nhiệm được phân chia rõ ràng cho từng thành viên. Dự án được thực hiện từ ngày 1/6/2026 đến ngày 6/7/2026, theo một quy trình có cấu trúc từ phân tích yêu cầu, lập kế hoạch công việc, phát triển, kiểm thử cho đến triển khai cuối cùng.

## 2. Chuẩn bị dự án

Ngay từ đầu dự án, nhóm đã cùng xem xét yêu cầu và thảo luận về định hướng tổng thể của website. Giai đoạn chuẩn bị này giúp chúng tôi xác định phạm vi công việc, hiểu rõ chức năng cần xây dựng và thống nhất cách làm trước khi bước vào triển khai.

- Backend development, business logic, quản lý AWS và triển khai được giao cho Vinh và Lợi.
- Frontend development được giao cho Phúc và tôi.
- Tất cả công việc đều được tạo và theo dõi trên Jira.
- Mã nguồn được quản lý trên GitHub để hỗ trợ cộng tác và kiểm soát phiên bản.

Việc phân chia trách nhiệm sớm giúp nhóm có thể làm việc song song và tránh nhầm lẫn trong các giai đoạn sau.

## 3. Lập kế hoạch công việc và tổ chức triển khai

Công việc của dự án được chia nhỏ thành nhiều task và ghi nhận trên Jira. Mỗi task đều có mô tả rõ ràng, người phụ trách và trạng thái để nhóm có thể theo dõi tiến độ trong suốt quá trình làm việc. Điều này giúp chúng tôi tổ chức công việc tốt hơn, phát hiện sớm các điểm nghẽn và đảm bảo không bỏ sót chức năng quan trọng nào.
GitHub được dùng làm nơi lưu trữ mã nguồn chính. Các thành viên commit code theo đúng task được giao, giúp việc review thay đổi, quản lý phiên bản và tích hợp giữa frontend với backend trở nên nhất quán hơn.

## 4. Phát triển Frontend

Phúc và tôi tập trung vào phần frontend của hệ thống. Công việc của họ bao gồm xây dựng giao diện người dùng, triển khai các trang chính, xử lý tương tác và kết nối giao diện với các API backend. Frontend được phát triển song song với backend để hai phần có thể đồng bộ liên tục.
Trong giai đoạn này, nhóm chú ý đến tính dễ sử dụng và tính nhất quán để website mang lại trải nghiệm rõ ràng và mượt mà cho người dùng.

## 5. Phát triển Backend

Ở phía backend, Lợi và Vinh phát triển phần logic cốt lõi của dự án và triển khai các API mà frontend sử dụng. Công việc này bao gồm xử lý business rules, tiếp nhận request, trả response và đảm bảo luồng dữ liệu giữa client và server luôn chính xác, ổn định.
Ngoài logic ứng dụng, Vinh còn quản lý tài khoản AWS và cấu hình các dịch vụ AWS cần thiết cho dự án. Điều này giúp backend có thể được triển khai và vận hành trong một môi trường cloud ổn định.

## 6. Thiết lập AWS và triển khai

Sau khi các tính năng chính hoàn thành, hệ thống được chuẩn bị để triển khai lên AWS. Vinh phụ trách thiết lập môi trường cloud, cấu hình các dịch vụ cần thiết và deploy ứng dụng để website có thể chạy trong một môi trường gần với production.
Giai đoạn triển khai này rất quan trọng vì nó biến dự án từ một hệ thống chạy local thành một hệ thống được host trên cloud, giúp việc truy cập và kiểm thử thực tế hơn.

## 7. Kiểm thử và tích hợp

Khi frontend và backend đã được kết nối, nhóm tiến hành kiểm thử tích hợp để xác nhận các thành phần hoạt động đúng với nhau. Chúng tôi kiểm tra các luồng sử dụng chính, rà soát giao tiếp giữa frontend và backend và sửa các lỗi phát hiện trong quá trình test.

- Chức năng được kiểm thử end to end.
- Sự tích hợp giữa frontend và backend được xác minh.
- Các lỗi phát hiện trong quá trình kiểm thử được ghi nhận và sửa thông qua các task trên Jira.

Giai đoạn này giúp cải thiện độ ổn định và đảm bảo hệ thống sẵn sàng cho bàn giao cuối cùng.

## 8. Phối hợp làm việc và quản lý mã nguồn

Trong suốt dự án, Jira và GitHub đóng vai trò trung tâm trong việc phối hợp giữa các thành viên. Jira giúp theo dõi tiến độ và phân công công việc, còn GitHub cung cấp một cách an toàn và minh bạch để quản lý mã nguồn. Hai công cụ này giúp việc cộng tác dễ dàng hơn và giảm rủi ro chồng chéo hoặc mất thay đổi.

## 9. Rà soát cuối cùng và bàn giao

Trước khi kết thúc dự án, nhóm thực hiện rà soát cuối cùng các tính năng đã triển khai, kiểm tra trạng thái deploy trên AWS và xác nhận rằng các luồng sử dụng quan trọng hoạt động đúng như mong đợi. Việc rà soát cuối cùng này giúp đảm bảo dự án đã sẵn sàng để bàn giao và trình bày.
Tài liệu dự án, repository mã nguồn và lịch sử task đều được sắp xếp gọn gàng để hệ thống có thể được bảo trì và mở rộng trong tương lai. Điều này cũng giúp việc xem lại quy trình phát triển và giải thích từng phần của hệ thống trở nên dễ dàng hơn.

## 10. Kết luận

Nhìn chung, dự án GreenLens được hoàn thành theo một quy trình rõ ràng và có tổ chức. Nhóm làm việc với trách nhiệm được phân chia cụ thể, duy trì giao tiếp nhất quán và sử dụng hiệu quả Jira và GitHub để quản lý task cũng như mã nguồn. Nhờ đó, dự án đã được phát triển thành công trong khung thời gian dự kiến từ ngày 1/6/2026 đến ngày 6/7/2026.

GitHub: [Kho lưu trữ GreenLens](https://github.com/2280603697NguyenQuangVinh/Greenlens)
Demo trực tiếp: [Bản triển khai GreenLens](https://main.d32rydccx28td4.amplifyapp.com/)
