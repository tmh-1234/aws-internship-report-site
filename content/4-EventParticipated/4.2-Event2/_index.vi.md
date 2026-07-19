---
title: "Sự kiện 2"
date: 2026-07-10
weight: 2
chapter: false
pre: " <b> 4.2. </b> "
---
# Báo cáo Sự kiện: "FCAJ Community Day"

### Mục tiêu của Sự kiện

* Kết nối khoảng cách giữa vận hành IT cốt lõi và các mô hình tiên phong về điện toán đám mây, bảo mật thông minh và AI.
* Nghiên cứu thực hành công nghệ đóng gói container và kiến trúc mạng nâng cao giúp tối ưu hiệu suất hệ thống.
* Giới thiệu các quy trình bảo mật và truy xuất dữ liệu hiện đại xoay quanh công nghệ Học máy và GraphRAG.
* Đưa ra lộ trình sự nghiệp thực tế, tư duy vận hành bài bản và khung làm việc nhóm hiệu quả cho các kỹ sư công nghệ.

### Diễn giả nổi bật

* **Bảo Huỳnh** – Docker - A containerization technology
* **Lê Hoàng Gia Đại** – Combining AWS WAF with Machine Learning for Cyber Attack Detection on AWS
* **Nguyễn Quốc Bảo** – Topic: Multiplayer in the Cloud: Connecting Godot Clients with AWS WebSockets
* **Trương Huy Phước** – Topic: Cách làm việc nhóm hiệu quả
* **Việt Phát** – Topic: AWS Neptune for Building a Graph Knowledge Base for GraphRAG
* **Vinh Trần** – Topic: Từ IT Helpdesk lên Senior Sysadmin: Hành trình tự học và Lộ trình dịch chuyển sang Cloud/DevOps

### Điểm nhấn chính

#### Docker - A containerization technology

* Trình bày một góc nhìn so sánh kiến trúc toàn diện giữa Máy ảo (VM) truyền thống nặng nề và Container nhẹ nhàng.
* Giải thích cách các container chia sẻ chung hệ điều hành host để khởi động chỉ trong vài mili-giây và giảm thiểu tối đa tài nguyên tiêu thụ.
* Làm nổi bật triết lý lõi "đóng gói một lần, chạy ở mọi nơi" của Docker nhằm tinh gọn quy trình triển khai phần mềm.

#### Combining AWS WAF with Machine Learning for Cyber Attack Detection on AWS

* Chi tiết hóa cách xây dựng Hệ thống phát hiện xâm nhập mạng (NIDS) dựa trên Học máy để bảo vệ hạ tầng đám mây.
* Đạt độ chính xác cao lên đến 95.86% nhờ sử dụng mô hình LightGBM được huấn luyện trên tập dữ liệu CSE-CIC-IDS2018.
* Vượt qua các rào cản dựa trên luật (rule-based) của giải pháp AWS WAF truyền thống khi đối phó với các cuộc tấn công zero-day phức tạp.

#### Topic: Multiplayer in the Cloud: Connecting Godot Clients with AWS WebSockets

* Khám phá kiến trúc mạng thời gian thực kết nối các client game Godot 4 thông qua mạng đám mây bền bỉ.
* Sử dụng giải pháp AWS WebSockets kết hợp cùng API Gateway, Lambda và DynamoDB để quản lý trạng thái người chơi đang hoạt động.
* Giải quyết các bài toán hạ tầng cloud thực tế như xử lý kết nối ảo (GoneException) và vạch ra lộ trình nâng cấp lên AWS GameLift.

#### Topic: Cách làm việc nhóm hiệu quả

* Đúc kết "4 Nguyên tắc Vàng" trong phối hợp đội ngũ: Mục tiêu chung, Đúng người đúng việc, Giao tiếp cởi mở và Trách nhiệm cá nhân.
* Tối ưu hóa các đường ống quản lý dự án bằng cách tích hợp trực tiếp các công cụ tự động hóa vào quy trình làm việc của nhóm.
* Minh họa việc giao tiếp chuẩn DevOps qua việc cấu hình tự động gửi thông báo từ GitLab và ClickUp đồng bộ vào Discord.

#### Topic: AWS Neptune for Building a Graph Knowledge Base for GraphRAG

* Giải quyết điểm yếu thiếu khả năng tư duy bắc cầu (multi-hop reasoning) của hệ thống RAG sử dụng vector truyền thống.
* Giới thiệu mô hình GraphRAG giúp khám phá các mối quan hệ thực thể chuyên sâu và hỗ trợ tư duy xuyên tài liệu phức tạp.
* So sánh giữa hướng đi Managed hoàn toàn (Bedrock Knowledge Bases + Neptune Analytics) và hướng đi tùy chỉnh sử dụng LlamaIndex cùng Claude 3.5 Sonnet.

#### Topic: Từ IT Helpdesk lên Senior Sysadmin: Hành trình tự học và Lộ trình dịch chuyển sang Cloud/DevOps

* Chia sẻ lộ trình sự nghiệp thực tế định hướng cho kỹ sư đi từ Helpdesk khởi điểm lên các vai trò Senior Sysadmin và DevOps.
* Nhấn mạnh tầm quan trọng của việc tự học thực hành thông qua các phòng lab Linux để làm chủ năng lực hạ tầng cốt lõi.
* Xây dựng tư duy vận hành kỷ luật hướng đến tính ổn định cao, đúc kết qua câu khẩu hiệu "không bao giờ thử nghiệm trên môi trường production".
* Dịch chuyển thành công từ hạ tầng on-premise truyền thống sang các giải pháp cloud-native hiện đại sử dụng AWS, Terraform và CI/CD.

### Bài học cốt lõi

#### Phát triển nghề nghiệp
* **Sản phẩm thực tế (Portfolio)** được xây dựng qua các phòng lab tự học có giá trị lớn hơn nhiều so với việc chỉ tích lũy chứng chỉ lý thuyết thuần túy.
* Thăng tiến lên các vị trí kỹ sư chuyên sâu đòi hỏi sự tích lũy kỹ năng cốt lõi kết hợp với tinh thần chủ động học hỏi không ngừng.

#### Hiện đại hóa kiến trúc
* Nâng cấp hạ tầng từ on-premise thủ công hoặc VM cồng kềnh sang container đám mây mang lại hiệu quả vượt trội về mặt tài nguyên.
* Khả năng mở rộng ứng dụng hiện đại phụ thuộc lớn vào các kết nối WebSockets bền vững và hạ tầng dạng mã code (IaC) tự động.

#### Bảo mật thông minh
* Các quy tắc tường lửa tĩnh dựa trên dấu hiệu (signature-based) không còn đủ sức ngăn chặn các mối đe dọa mạng tinh vi ngày nay.
* Tích hợp các mô hình Học máy phân tích hành vi là lớp phòng thủ thích ứng bắt buộc phải có chống lại các lỗ hổng zero-day.

#### Truy xuất ngữ cảnh nâng cao
* Việc đưa cấu trúc GraphRAG vào quy trình xử lý của Mô hình ngôn ngữ lớn (LLM) giúp loại bỏ các điểm mù ngữ cảnh của giải pháp vector thuần túy.
* Kết hợp đồ thị tri thức với LLM cho phép hệ thống doanh nghiệp thực hiện các lập luận bắc cầu phức tạp trên kho tài liệu đồ sộ.

#### Tối ưu hóa quy trình
* Triển khai thành công các dự án enterprise luôn đòi hỏi một tư duy vận hành chỉn chu đi kèm tài liệu hệ thống (runbook) rõ ràng.
* Đồng bộ hóa các công cụ phát triển như GitLab, ClickUp với các kênh giao tiếp giúp giảm ma sát vận hành và tối đa hóa hiệu suất đội ngũ.

### Kế hoạch hành động & Ứng dụng thực tế

* Tự xây dựng các phòng lab Linux và môi trường cloud cá nhân để dịch chuyển kỹ năng từ on-premise sang thực hành cloud-native.
* Áp dụng đóng gói Docker vào quy trình triển khai để tối ưu hóa việc sử dụng tài nguyên và tăng tính linh hoạt cho ứng dụng.
* Nghiên cứu các mô hình Học máy như LightGBM để bổ trợ và gia cố thêm cho hệ thống tường lửa ứng dụng web truyền thống.
* Thử nghiệm với AWS WebSockets và API Gateway nhằm xây dựng các kiến trúc backend thời gian thực có khả năng mở rộng tốt cho ứng dụng.
* Thiết lập các cổng webhook thông báo tự động giữa công cụ quản lý công việc và nền tảng chat để tối ưu độ minh bạch trong nhóm.
* Đánh giá kiến trúc GraphRAG sử dụng LlamaIndex hoặc các dịch vụ AWS managed để nâng cấp hệ thống tìm kiếm tri thức nội bộ.

#### Suy ngẫm về buổi chia sẻ
* Tham gia FCAJ Community Day mang lại giá trị vô cùng to lớn, làm sáng tỏ nhiều khía cạnh từ vận hành hệ thống chủ động, hiện đại hóa đám mây, bảo mật thông minh cho đến truy xuất AI nâng cao. Sự kết hợp hài hòa giữa lộ trình phát triển cá nhân, bài học kỹ thuật chuyên sâu và khung làm việc nhóm hiệu quả đã mở ra một bản kế hoạch rõ ràng mà tôi có thể áp dụng ngay vào các dự án đám mây sắp tới của mình.

#### Góc nhìn từ chuyên gia trong ngành
* Các diễn giả đã mang đến những góc nhìn cực kỳ thực tế về cách định vị và điều hướng bản thân khi chuyển dịch từ hạ tầng IT truyền thống sang hệ sinh thái cloud-native.
* Các case-study thực tế minh họa trực quan cách kết hợp mô hình kiến trúc hiện đại với quy trình tự động hóa nhằm nâng cao độ tin cậy hệ thống và hiệu suất làm việc.

#### Tiếp cận kỹ thuật
* Hiểu được cách GraphRAG giải quyết các hạn chế về tư duy bắc cầu của RAG dạng vector truyền thống thông qua Bedrock và Neptune.
* Khám phá cách triển khai hệ thống phát hiện xâm nhập mạng NIDS ứng dụng Học máy LightGBM để bảo vệ môi trường cloud trước tấn công zero-day.
* Nắm rõ cách các kỹ sư công nghệ tận dụng kết nối WebSockets bền vững trên AWS để điều phối các kết nối client multiplayer theo thời gian thực.

#### Áp dụng công cụ hiện đại
* Nhận thức Docker là một công cụ không thể thiếu để đóng gói và triển khai ứng dụng dạng container gọn nhẹ, linh hoạt.
* Tích lũy các chiến lược thực tế để nhúng các công cụ tự động hóa hạ tầng như Terraform và đường ống CI/CD vào vận hành hàng ngày.
* Tiếp cận các bản thiết kế kỹ thuật liên quan đến các dịch vụ đám mây managed nâng cao như AWS GameLift, Bedrock Knowledge Bases và Neptune Analytics.

#### Thảo luận mang tính cộng tác
* Môi trường tương tác mở tạo cơ hội tuyệt vời để trao đổi ý tưởng với các chuyên gia quản trị hệ thống, kỹ sư đám mây và những người đam mê AI.
* Các phiên thảo luận về làm việc nhóm hiệu quả đã vạch ra các cột mốc rõ ràng cho sự phát triển cá nhân, tinh thần trách nhiệm và vận hành xuất sắc.
* Buổi chia sẻ củng cố luận điểm rằng thành công dài hạn trong ngành công nghệ đòi hỏi sự kết hợp cân bằng giữa làm chủ kỹ thuật, năng lực thích ứng và giao tiếp tốt.

#### Các nguyên tắc cốt lõi đã học
* Tư duy vận hành kỷ luật ("không bao giờ test trên production") vẫn luôn là yếu tố sống còn để duy trì các hệ thống có tính sẵn sàng cao.
* Kiến trúc đám mây đang tiến hóa mạnh mẽ từ các cụm triển khai tĩnh, cô lập sang các hệ sinh thái tích hợp sâu, thông minh và phản hồi theo thời gian thực.
* Tận dụng học máy phân tích hành vi và các quy trình tự động hóa giúp nhân rộng đáng kể năng lực của cả cá nhân và tập thể.
* Sự sẵn sàng về mặt chuyên môn đòi hỏi sự tập trung đồng đều vào việc làm sản phẩm thực tế, đào sâu chuyên môn và rèn luyện tư duy giải quyết vấn đề linh hoạt.

#### Hình ảnh sự kiện
![alt text](image.png)

> Tóm lại, "FCAJ Community Day" đã mang đến những kiến thức chuyên sâu và thực tế về tư duy kỹ nghệ hiện đại, kiến trúc cloud-native, bảo mật thông minh và tích hợp AI nâng cao. Nhờ các phần trình bày chi tiết từ đội ngũ diễn giả, tôi đã có cái nhìn rõ ràng hơn về cách chuyển dịch từ các hệ thống cũ sang hệ sinh thái đám mây tự động hóa cao. Toàn bộ sự kiện đã truyền động lực mạnh mẽ, thôi thúc tôi không ngừng hoàn thiện bản thân và chủ động áp dụng tự động hóa đám mây vào công việc kỹ thuật hàng ngày.