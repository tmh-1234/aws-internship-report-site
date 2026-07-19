---
title: "Worklog Tuần 9"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 1.9. </b> "
---
### Mục tiêu Tuần 9:

* Lập trình các khả năng multi-part camera data streaming để object detection và thiết lập nền tảng cho trò chơi phân loại.

### Nhiệm vụ trong tuần này:
| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày kết thúc | Tài nguyên |
| --- | --- | ------------ | --------------- | --------------- |
| Thứ 2 | Nghiên cứu các thông số kỹ thuật của AI Camera API và cấu hình HTTP clients để xử lý các multi-part Form Data payloads chứa image blobs. | 15/06/2026 | 15/06/2026 | GitHub |
| Thứ 3 | Phát triển Frontend: Khởi chạy triển khai tính năng AI Camera; lập trình native camera triggers và các device media gallery picker components. | 16/06/2026 | 16/06/2026 | GitHub |
| Thứ 4 | Phát triển Frontend: Lập trình chức năng local token lookup để trích xuất `childId` đang hoạt động từ device storage và đính kèm nó cùng với các multipart image streams vào POST `/ai-camera/analyze`. | 17/06/2026 | 17/06/2026 | GitHub |
| Thứ 5 | Phát triển Frontend: Tạo một trạng thái xử lý phân tích trực quan sinh động (Loading State) với các mascot animations thân thiện với trẻ em. | 18/06/2026 | 18/06/2026 | GitHub |
| Thứ 6 | Lập trình `AI Result Screen` để giải nén các classification attributes bao gồm object labels, confidence scores, target categories, và các màu thùng rác tương ứng (`binColor`). | 19/06/2026 | 19/06/2026 | GitHub |
| Thứ 7 | Phát triển Frontend: Triển khai các thẻ giáo dục phong phú bao gồm Recycling Guide Card, Reuse Suggestion Card, và Environmental Impact Card. | 20/06/2026 | 20/06/2026 | GitHub |
| Chủ Nhật | Phát triển Frontend: Khởi tạo layout cho Trash Sorting Mini-Game; kết nối GET `http://localhost:5001/mini-games/trash-sort/items` để fetch động và map các biểu tượng vật phẩm rác cùng với các thùng rác phân loại. | 21/06/2026 | 21/06/2026 | GitHub |

### Thành tựu Tuần 9:

* Lập trình các multipart file-upload pipelines đến các AI analysis APIs.
* Xây dựng các thẻ phản hồi giáo dục trực quan.
* Fetch động các danh sách vật phẩm trò chơi.