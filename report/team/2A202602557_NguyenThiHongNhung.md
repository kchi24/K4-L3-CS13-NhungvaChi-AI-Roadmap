# Báo cáo cá nhân — CS13 Lộ trình sản phẩm AI

## 1. Thông tin thành viên

- Họ tên: Nguyễn Thị Hồng Nhung
- MSSV: 2A202602557
- Nhóm và đề CS13: Nhóm NhungvaChi · Đề 1: SổSạch — Trợ lý đọc hoá đơn đầu vào

## 2. Phần việc phụ trách

- Phụ trách chính: Checkpoint 1 & Checkpoint 3 (Trang `0_Đầu vào`, `1_Danh sách việc` cột B–E, và trang `2_Mức tự động`).
- Đồng phụ trách: Xây dựng cấu trúc Bảng lộ trình và Slide lãnh đạo (Trang `3_Bảng lộ trình` và `5_Slide lãnh đạo`).

## 3. Đóng góp cụ thể

- Phân tích hồ sơ Đề 1 (SổSạch), xác định định nghĩa "1 việc" là 1 hoá đơn được đọc, đối chiếu và nhập vào phần mềm kế toán.
- Thiết lập 7 giả thuyết công việc định lượng cho Đề 1, bảo đảm tất cả đều có chỉ số và ngưỡng số cụ thể.
- Xây dựng 4 mức tự động hoá (Mức 0 đến Mức 3), thiết lập các cổng đánh giá kiểm thử chất lượng (Quality Gate) với cỡ mẫu từ 500 đến 2.000 ca, cam kết 0 lỗi sai mã số thuế và 0 lỗi sai tiền.
- Tính toán tỷ lệ duyệt của kế toán viên công ty (từ 100% ở Mức 0 xuống 20% ở Mức 1, 10% ở Mức 2 và 5% ở Mức 3), đưa biên lợi nhuận gộp từ 24,46% lên 68,79% (Mức 1), 74,33% (Mức 2) và 77,10% (Mức 3), vượt ngưỡng an toàn 60%.

## 4. Bằng chứng

- Trang `1_Danh sách việc`: Cột B–E dòng 5–11.
- Trang `2_Mức tự động`: Cột C–I dòng 5–8 và kiểm tra biên gộp cột K–L.
- Trang `3_Bảng lộ trình`: Tầng Bây giờ (Cột B dòng 5–12).
- File bài làm chính: `NhungvaChi_CS13.xlsx` trong repo nhóm.

## 5. Tự đánh giá

- **Điều hiểu rõ:** Hiểu sâu về cách thiết kế Cổng đánh giá (Quality Gate) và mối quan hệ trực tiếp giữa mức độ tự động hóa với bài toán kinh tế (Unit Economics). AI không thể thay thế người ngay lập tức mà phải hạ dần tỷ lệ can thiệp của con người thông qua các chốt chặn kiểm thử độ tin cậy.
- **Giả định cần kiểm chứng:** Cần kiểm chứng tỷ lệ cờ thừa thực tế trong tuần đầu thử nghiệm với chị Hạnh (mục tiêu $\le 10\%$) để đảm bảo không gây phiền toái khiến kế toán viên quá tải và bỏ dùng sản phẩm.
