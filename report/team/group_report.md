# Báo cáo nhóm — CS13 Lộ trình sản phẩm AI

## 1. Thông tin nhóm

- Tên nhóm: NhungvaChi
- Đề CS13: Đề 1 · SổSạch — Trợ lý đọc hoá đơn đầu vào cho văn phòng kế toán dịch vụ
- Thành viên: xem [team/TEAM.md](../../team/TEAM.md) (Nguyễn Thị Hồng Nhung & Thân Thị Kim Chi).

## 2. Mục tiêu và cách tiếp cận

- **Mục tiêu:** Xây dựng lộ trình 12 tháng chuyển đổi sản phẩm SổSạch từ giai đoạn thử nghiệm Bản 2 (đã qua cổng phát hành) sang tự động hóa từng phần, đưa biên lợi nhuận gộp từ 24,46% lên trên 70%, đồng thời phòng ngừa biến cố kinh tế (hết tiền ở tháng 7).
- **Cách tiếp cận:** Tiếp cận theo tư duy Sản phẩm AI dựa trên giả thuyết và dữ liệu:
  - Định nghĩa "1 việc" thống nhất xuyên suốt: 1 hoá đơn được đọc, đối chiếu và nhập vào phần mềm kế toán.
  - Chấm điểm ưu tiên RICE-AI có tính đến sẵn sàng dữ liệu, sẵn sàng đánh giá và rủi ro bị nền tảng "nuốt".
  - Tăng dần mức tự động hóa đi kèm với Quality Gate chặt chẽ (0 lỗi mã số thuế, 0 lỗi tiền) và kiểm soát chi phí người duyệt.

## 3. Giải pháp

- **Việc chọn làm trước (0–3 tháng):**
  1. Nhập tự động hoá đơn điện tử từ tệp gốc XML/PDF (Hạng 1).
  2. Đối chiếu mã số thuế người bán qua API (Hạng 2).
  3. Đọc ảnh hoá đơn giấy bằng Bản 2 (Hạng 3).
  4. Gắn cờ hoá đơn nghi ngờ cần người xem (Hạng 4).
  5. Kiểm chứng gói phí với 30% văn phòng dùng nhiều để bảo vệ doanh thu (Hạng 5).
- **Mức tự động & Cổng đánh giá:**
  - Nâng từ Mức 0 lên Mức 1 sau khi đạt cổng kiểm thử: Tỷ lệ đạt $\ge 97\%$ trên $\ge 500$ hóa đơn thật, 0 sai mã số thuế, 0 sai tiền, do Chị Hạnh ký duyệt.
  - Giảm tỷ lệ người duyệt của công ty từ 100% xuống 20% (Mức 1), 10% (Mức 2) và 5% (Mức 3).

## 4. Kết quả

- **File Excel bài làm:** [`NhungvaChi_CS13.xlsx`](../../NhungvaChi_CS13.xlsx)
- **Trạng thái tự kiểm tra:** Đạt **8/8** mục tại trang `6_Tự kiểm tra`.
- **Chỉ số kinh tế chủ chốt:**
  - Chi phí mỗi việc: 1.704 đ (Mức 0) $\rightarrow$ 704 đ (Mức 1) $\rightarrow$ 579 đ (Mức 2) $\rightarrow$ 516,5 đ (Mức 3).
  - Biên lợi nhuận gộp: 24,46% (Mức 0) $\rightarrow$ **68,79% (Mức 1)** $\rightarrow$ **74,33% (Mức 2)** $\rightarrow$ **77,10% (Mức 3)** (Vượt xa ngưỡng tối thiểu 60%).
- **Slide lãnh đạo:** Hoàn thiện 5 ô nội dung súc tích ($\le 60$ từ/ô) và thiết kế 1 slide trình bày tổng quan.

## 5. Khó khăn và cách xử lý

- *Khó khăn:* Rủi ro kế toán viên bị quá tải do tỷ lệ cờ thừa cao và rủi ro bị các mô hình AI nền tảng miễn phí thay thế tính năng.
- *Cách xử lý:* Tinh chỉnh ngưỡng nhạy của thuật toán gắn cờ (mục tiêu cờ thừa $\le 10\%$); loại bỏ hoàn toàn ý tưởng làm chatbot trả lời luật thuế chung (`Không làm`); tập trung năng lực vào xử lý chuyên sâu dữ liệu hóa đơn Việt Nam và đối soát thuế API.

## 6. Tổng hợp đóng góp

Xem chi tiết phân công và đóng góp tại [team/TEAM.md](../../team/TEAM.md).

## 7. Hạn chế và hướng cải thiện

- *Hạn chế:* Dữ liệu định khoản tài khoản kế toán khách hàng chưa có sẵn, phải hoãn tính năng gợi ý tài khoản hạch toán sang giai đoạn 6–12 tháng.
- *Mốc rà soát:* Thực hiện rà soát nghiêm ngặt vào các mốc Ngày 30, Ngày 60 và Ngày 90 (đặc biệt kiểm chứng ngưỡng dừng doanh thu 3,71 triệu đồng ở ngày 90).

## 8. Tài liệu tham khảo

- Hồ sơ tình huống Đề 1 (SổSạch) và Slide bài giảng CS13 AI Roadmap.
- Luật Trí tuệ nhân tạo số 134/2025/QH15.
