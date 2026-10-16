# CS13 — Lộ trình sản phẩm AI · Nhóm NhungvaChi

**AI in Action · Track 1 · Khóa 4 · Chiều 16/10/2026**

- **Tên nhóm:** NhungvaChi
- **Đề bài:** Đề 1 · SổSạch — Trợ lý đọc hoá đơn đầu vào cho văn phòng kế toán dịch vụ
- **Thành viên nhóm:**
  - Nguyễn Thị Hồng Nhung — MSSV: 2A202602557
  - Thân Thị Kim Chi — MSSV: 2A202602797
- **Link repo bài làm:** [https://github.com/kchi24/K4-L3-CS13-NhungvaChi-AI-Roadmap]

---

## 1. Danh sách sản phẩm nộp bài (Deliverables)

1. **File Excel bài làm chính:** [`NhungvaChi_CS13.xlsx`](NhungvaChi_CS13.xlsx)
   - Hoàn thành đầy đủ từ CP1 đến CP5.
   - Trang `6_Tự kiểm tra` đạt **8/8 tiêu chí Đạt**.
2. **Slide lãnh đạo (PDF):** [`NhungvaChi_CS13_SlideLanhDao.pdf`](NhungvaChi_CS13_SlideLanhDao.pdf)
   - Bản trình chiếu 1 slide tone sáng, súc tích dành cho Ban Lãnh đạo.
3. **Phân công & đóng góp thành viên:** [`team/TEAM.md`](team/TEAM.md)
4. **Báo cáo nhóm & báo cáo cá nhân:**
   - Báo cáo nhóm: [`report/team/group_report.md`](report/team/group_report.md)
   - Báo cáo cá nhân: [`report/team/2A202602557_NguyenThiHongNhung.md`](report/team/2A202602557_NguyenThiHongNhung.md)
   - Báo cáo cá nhân: [`report/team/2A202602797_ThanThiKimChi.md`](report/team/2A202602797_ThanThiKimChi.md)

---

## 2. Tóm tắt giải pháp & Kết quả chính

### Định nghĩa & Bài toán kinh tế
- **1 việc:** 1 hoá đơn được đọc, đối chiếu và nhập vào phần mềm kế toán.
- **Doanh thu bình quân:** 3.970.000 đ / 1.760 việc $\approx$ 2.256 đ/việc.

### Các mức tự động hóa & Biên lợi nhuận gộp
| Mức | Tên mức | Tỷ lệ người duyệt | Chi phí 1 việc | Biên gộp | Cổng đánh giá chuyển mức |
|:---:|---|:---:|:---:|:---:|---|
| **0** | Gợi ý | 100% | 1.704 đ | 24,46% | Mức khởi đầu Bản 2 (đã qua cổng phát hành) |
| **1** | Hỗ trợ có duyệt | **20%** | **704 đ** | **68,79%** | Đạt $\ge 97\%$ trên $\ge 500$ ca thật; 0 sai MST; 0 sai tiền (Chị Hạnh duyệt) |
| **2** | Tự động một phần | **10%** | **579 đ** | **74,33%** | Đúng $\ge 98\%$ trên $\ge 1.000$ ca; cờ thừa $\le 10\%$; 0 lỗi MST (Anh Tùng duyệt) |
| **3** | Tự động có giám sát | **5%** | **516,5 đ** | **77,10%** | Khớp dữ liệu $\ge 99\%$ trên $\ge 2.000$ ca; khiếu nại $< 0,1\%$ |

### Lộ trình 3 tầng (Bây giờ / Tiếp theo / Sau này)
- **Bây giờ (0–3 tháng):** Nhập tự động tệp gốc + Đối chiếu MST qua API + Đọc ảnh Bản 2 + Gắn cờ ca nghi ngờ.
  - *Điều kiện dừng:* **NẾU doanh thu bình quân dưới 3,71 triệu/văn phòng trong 2 tháng liên tiếp trên ít nhất 10 văn phòng THÌ dừng mở rộng.**
- **Tiếp theo (3–6 tháng):** Tự động hóa 90% hóa đơn thường (Mức 2, biên 74,3%), mở rộng bộ đề lên 500 ca, thu thập dữ liệu hạch toán từ 20 doanh nghiệp khách hàng.
- **Sau này (6–12 tháng):** Thử nghiệm Mức 3 (biên 77,1%) và triển khai gợi ý tài khoản hạch toán. Loại bỏ chatbot tư vấn thuế (rủi ro nuốt 0,9).

---

## 3. Kết quả tự kiểm tra (8/8 Đạt)

1. Số việc đã chấm điểm: **7 việc** ($\ge 5$) $\rightarrow$ **Đạt**
2. Việc được giữ lại thiếu giả thuyết/chỉ số: **0** $\rightarrow$ **Đạt**
3. Số mức tự động có cổng bằng con số (Mức 1–3): **3 mức** ($\ge 2$) $\rightarrow$ **Đạt**
4. Bảng lộ trình: tầng Bây giờ đủ: **8/8 ô** $\rightarrow$ **Đạt**
5. Điều kiện dừng tầng Bây giờ có con số: **Có** $\rightarrow$ **Đạt**
6. Căn cứ kinh tế có con số: **Có** $\rightarrow$ **Đạt**
7. Slide lãnh đạo: số ô đạt: **5/5 ô** ($\le 60$ từ) $\rightarrow$ **Đạt**
8. Số mức tự động có biên lợi nhuận $\ge 60\%$: **3 mức** ($\ge 1$) $\rightarrow$ **Đạt**
