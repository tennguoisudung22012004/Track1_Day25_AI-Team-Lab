# Track1_Day25_AI-Team-Lab

- Team: Rosbag 
- Thành viên (3–5 người):Nguyễn Phạm Oanh Oanh, Hoàng Bích Ngọc 
- Tên dự án:
Bối cảnh giả định: Trong bài Lab, team được giả định là nhóm sáng lập phát triển Rosbag Doctor thành sản phẩm B2B cho các tổ chức phát triển và tích hợp robot sử dụng ROS 2. Kỹ sư là người dùng chính trong quy trình chẩn đoán; hệ thống có ba role Engineer, Admin và User để phân quyền phân tích, quản trị và khai thác kết quả.Team đang ở giai đoạn tiền thương mại hóa, có bản sản phẩm ban đầu và cần kiểm chứng hiệu quả trên quy trình gỡ lỗi thực tế trước khi mở rộng bán hàng. Khách hàng mục tiêu ban đầu là công ty phát triển hoặc tích hợp robot sử dụng ROS 2, có đội kỹ thuật nhỏ. Kỹ sư ROS 2 là người sử dụng và đánh giá sản phẩm; CTO là người bảo trợ kỹ thuật và duyệt ngân sách pilot trong phạm vi thẩm quyền.

# Bối cảnh và Mục tiêu dự án

1. Bối cảnh đã chọn

| Thành phần | Chi tiết |
| :--- | :--- |
| **Team** | Team sáng lập sản phẩm B2B Rosbag Doctor |
| **Khách hàng mục tiêu ban đầu** | Công ty phát triển hoặc tích hợp robot sử dụng ROS 2, có đội kỹ thuật riêng |
| **Người đánh giá và đề xuất mua** | Robotics Lead hoặc Engineering Manager, phối hợp với kỹ sư dùng thử |
| **Người duyệt mua dự kiến** | Head of Engineering hoặc CTO có thẩm quyền ngân sách; cần xác minh ở từng khách hàng |

2. Mục tiêu hiện tại: trong 1–3 tháng tới team đang cố đạt điều gì?

* **Triển khai pilot:** Triển khai tại 1 công ty robotics sử dụng ROS 2, với 3–5 Engineer tham gia thử nghiệm trong 4 tuần.
* **Hoàn thiện MVP cho pilot:** Vận hành đầy đủ core workflow: `upload rosbag` -> `analysis` -> xem `evidence` và `AI recommendations` -> `Engineer review` -> `export report`. Kiểm thử role-based access control cho Engineer/Admin/User, không còn critical bug gây gián đoạn core workflow, truy cập sai quyền.
* **Kiểm chứng chất lượng AI:** Xây dựng evaluation dataset gồm tối thiểu 30 rosbag cases có ground truth (kết luận tham chiếu) được domain expert xác nhận. Đạt precision $\ge 85\%$, recall $\ge 80\%$ cho anomaly detection (phát hiện bất thường) trong phạm vi hỗ trợ; $\ge 80\%$ AI recommendations được Engineer đánh giá là hữu ích để chọn bước kiểm tra tiếp theo.
* **Chứng minh giá trị sử dụng:** Giảm ít nhất 25% thời gian từ khi mở rosbag - xác định bước kiểm tra tiếp theo, so với baseline trên các cases tương đương; đạt điểm hữu ích trung bình $\ge 4/5$ từ Engineer tham gia pilot.
* **Kiểm chứng khả năng thương mại hóa:** Ký 1 paid pilot agreement với khách hàng, có budget approval, scope và acceptance criteria rõ ràng. Sau pilot, có quyết định tiếp tục sử dụng trả phí hoặc các điều kiện cụ thể để chuyển sang commercial contract.
* **Đánh giá unit economics:** Ghi nhận AI inference cost (chi phí suy luận), data processing cost, storage cost và support cost trong pilot; xây dựng pricing dự kiến đạt gross margin $\ge 50\%$ tại mức sử dụng đã thống nhất với khách hàng.

- Link sản phẩm/demo (nếu có): https://ctrlshiftn-hrd3ayfue2eqgvee.eastasia-01.azurewebsites.net/

## Bài nộp

File: `Day25_AI-Team-Lab_Rosbag.pdf`
