---
title: "Worklog Tuần 10"
date: 2024-01-01
weight: 2
chapter: false
pre: " <b> 1.10. </b> "
---
### Mục tiêu tuần 10:

* Tích hợp các công cụ hỗ trợ tiếp cận multi-sensory để hướng dẫn người chơi nhỏ tuổi.
* Tinh chỉnh các interactive gaming mechanics và bộ tính điểm (score calculators).

### Các công việc cần triển khai trong tuần này:
| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| ---- | --------- | ------------ | --------------- | -------------- |
| Thứ 2 | Tích hợp Web Speech API (`SpeechSynthesis`) để điều phối các narrated recycling guides được đọc to bởi mascot; triển khai error handling cho các ảnh trống để hoàn tất AI Camera epic. | 22/06/2026 | 22/06/2026 | GitHub |
| Thứ 3 | Phát triển Frontend: Lập trình dynamic item generation từ các backend datasets, xây dựng một descending countdown match timer và một game progress status bar. | 23/06/2026 | 23/06/2026 | GitHub |
| Thứ 4 | Phát triển Frontend: Lập trình các drag-and-drop mechanics cho interactive sorting, tích hợp các comparison checks đối chiếu với item categories để phát hiện các lượt kéo thả chính xác. | 24/06/2026 | 24/06/2026 | GitHub |
| Thứ 5 | Phát triển Frontend: Tích hợp endpoint submissions cho các kết quả trận đấu tới POST `http://localhost:5001/mini-games/trash-sort/results` để lưu trữ user metrics khi hoàn thành hoặc timeout. | 25/06/2026 | 25/06/2026 | GitHub |
| Thứ 6 | Phát triển Frontend: Phát triển dashboard bảng điểm tổng kết trận đấu (match summary scoreboard dashboard), hiển thị các metrics về tổng điểm, số câu đúng vs. sai, thời gian trận đấu, XP nhận được và các unlocked badges. | 26/06/2026 | 26/06/2026 | GitHub |
| Thứ 7 | Kiểm thử các tính năng responsive drag-and-drop trên các thiết bị mobile touch targets thực tế, sửa các coordinate alignment offsets để hoàn tất cột mốc mini-game cốt lõi. | 27/06/2026 | 27/06/2026 | GitHub |
| Chủ Nhật | Tiến hành rà soát mã nguồn (code reviews) và dọn dẹp (prunings) kỹ lưỡng trên các mô-đun AI Camera và Mini-Game để đồng nhất các shared widgets và tối ưu hóa animation frame rates. | 28/06/2026 | 28/06/2026 | GitHub |

### Kết quả đạt được tuần 10:

* Triển khai các tính năng text-to-speech qua Web Speech API.
* Triển khai các drag-and-drop mechanics với live timers.
* Kết nối thành công score logging endpoint.