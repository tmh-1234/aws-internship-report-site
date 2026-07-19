---
title: "Worklog Tuần 8"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.8. </b> "
---
### Mục tiêu tuần 8:

* Đồng bộ và kết nối trực tiếp dữ liệu giữa giao diện người dùng và hệ thống API để lưu trữ thông tin tài khoản nhân vật.

### Các công việc cần triển khai trong tuần này:
| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| --- | --- | ------------ | --------------- | --------------- |
| Thứ 2 | Phát triển Frontend: Tạo cấu trúc và viết module kết nối API khởi tạo hồ sơ nhân vật (POST /child-profiles) vào màn hình Character Creation. | 08/06/2026 | 08/06/2026 | GitHub |
| Thứ 3 | Phát triển Frontend: Đồng bộ hóa logic kết nối API xử lý kết quả Mini Game (POST /mini-game/complete), thiết lập giao diện Loading State trong lúc đợi backend tính toán và lưu lịch sử. | 09/06/2026 | 09/06/2026 | GitHub |
| Thứ 4 | Kiểm thử tích hợp luồng API hồ sơ: Đảm bảo sau khi tùy chỉnh diện mạo nhân vật thành công, Frontend lưu trữ chính xác mã định danh childId vào Local Storage trên thiết bị. | 10/06/2026 | 10/06/2026 | GitHub |
| Thứ 5 | Thực hiện rà soát mã nguồn toàn bộ hệ thống API, nghiệm thu các kịch bản lỗi phản hồi từ cơ sở dữ liệu DynamoDB. | 11/06/2026 | 11/06/2026 | GitHub |
| Thứ 6 | Phát triển Frontend: Thiết kế và viết code hiển thị các hiệu ứng phần thưởng sinh động, các hộp thoại Badge popup thông báo chúc mừng để tăng tính trò chơi hóa (gamification). | 12/06/2026 | 12/06/2026 | GitHub |
| Thứ 7 | Tối ưu hóa hiển thị responsive giao diện màn hình chính và form nhập thông tin, đảm bảo không xảy ra hiện tượng tràn viền (overflow layout) trên các thiết bị màn hình nhỏ. | 13/06/2026 | 13/06/2026 | GitHub |
| Chủ Nhật |  | 14/06/2026 | 14/06/2026 |  |

### Kết quả đạt được tuần 8:

* Tích hợp thành công các endpoint tạo hồ sơ.
* Cài đặt cơ chế lưu mã định danh vào bộ nhớ cục bộ.
