# Financial Health Diagnostic & Operational Audit

### 📌 Tổng Quan Dự Án
Dự án này tập trung vào việc phân tích chuyên sâu và đánh giá toàn diện **Sức khỏe tài chính doanh nghiệp** dựa trên tập dữ liệu thương mại điện tử ngành thời trang chuỗi 10 năm. Thông qua việc đào sâu các chỉ số tài chính cốt lõi, nhóm nghiên cứu đã bóc trần các lỗ hổng vận hành gây tổn thất dòng tiền, định lượng mức độ xói mòn lợi nhuận ròng và đề xuất các chiến lược tối ưu hóa để kiến tạo lộ trình tăng trưởng bền vững (Healthy Growth).

### ⚠️ Bài Toán Kinh Doanh: Nghịch Lý Tăng Trưởng & Chất Lượng Lợi Nhuận
Khi phân tích bức tranh tài chính tổng thể, doanh nghiệp bộc lộ một "nghịch lý tăng trưởng" cực kỳ nguy hiểm: Quy mô doanh thu mở rộng ấn tượng (tăng mạnh từ xấp xỉ 0.7 tỷ lên đỉnh điểm hơn 2.0 tỷ VND), nhưng sức khỏe tài chính thực tế lại suy thoái nghiêm trọng từ bên trong. 

Trong khi Biên lợi nhuận gộp (Gross Margin %) được kiểm soát khá tốt ở mức ổn định (11–16%), thì Biên lợi nhuận ròng (Net Margin %) lại lao dốc không phanh, chạm đáy nguy hiểm ở mức **1.7%** vào năm 2021. Khoảng trống ngày càng rộng này chứng minh một lượng tài sản khổng lồ đã bị bốc hơi do các loại **chi phí ẩn** phát sinh từ hệ thống vận hành.

### 🔍 Các Phát Hiện Cốt Lõi Về Sức Khỏe Tài Chính
Nhằm tái cấu trúc và chữa lành dòng lợi nhuận ròng, quy trình phân tích đã đi sâu mổ xẻ 3 tác nhân trực tiếp phá hủy Net Margin:

1. **Khủng hoảng Lợi nhuận do Chiến lược Khuyến mãi (Promotion Erosion):**
   * Doanh nghiệp đang bị phụ thuộc vào các đợt giảm giá phá hủy biên lợi nhuận. Chiến dịch giảm giá theo % (Percentage) chiếm tới 35.2% tỷ trọng, mang lại sản lượng cao nhất nhưng lợi nhuận ròng thu về lại chạm đáy (chỉ vỏn vẹn ~2,000 VND/đơn).
   * Ngược lại, chiến dịch giảm giá cố định (Fixed) tạo ra mức lợi nhuận ròng **cao gấp 3.5 lần** nhóm Percentage trên cùng một quy mô 100 đơn hàng nhưng lại bị bỏ quên (chỉ chiếm 3.2% tỷ trọng).
   * Phân tích đường xu hướng cảnh báo: Nếu tiếp tục đẩy mạnh cường độ chiết khấu Percentage lên vùng 15-20%, biên lợi nhuận sẽ chạm ranh giới hòa vốn (2%).

2. **Xói mòn Dòng tiền từ Tổn thất Hoàn hàng (Returns & Leakage):**
   * Hệ thống ghi nhận khoản tổn thất lớn lên đến 510.6M VND từ các đơn hàng bị hoàn trả. Đây thực chất là "doanh thu tạm thời" trên sổ sách chứ không phải dòng tiền thật.
   * Áp dụng nguyên lý Pareto định lượng được: `wrong_size` (sai kích cỡ - 34.6%), `defective` (hàng lỗi - 20.3%) và `not_as_described` (sai mô tả - 17.8%) tổng cộng chiếm tới **73.6% tổng giá trị hoàn trả**. Lỗi này phân bố đều trên toàn danh mục, chứng tỏ đây là lỗi hệ thống quy trình.
   * Dự báo cho thấy nếu chuẩn hóa Size Chart để giảm tỷ lệ hoàn hàng do sai size xuống mức 20%, doanh nghiệp sẽ bảo toàn và tiết kiệm được **13.5M VND/ngày**.

3. **Chôn vùi Dòng vốn vào "Tồn kho Chết" (Stockout & Overstock):**
   * Tình trạng cháy hàng (Stockout) ở các mã hàng chủ lực gây thất thoát 238.7M VND. Tỷ lệ đáp ứng đơn hàng (Fill rate) tổng thể 96% đã tạo ra **"Hiệu ứng che giấu số trung bình" (Average Masking Effect)**, che đậy việc nhóm sản phẩm bán chạy (Hero SKUs) bị thiếu hàng nghiêm trọng, chiếm 81.2% tổng thất thoát.
   * Ngược lại, doanh nghiệp đang bị **chôn vùi 40.51 tỷ VND vào "Vốn chết" (Dead capital)** với 1,169 SKU quá tải hàng tồn liên tiếp ≥3 tháng do bộ phận mua sắm (Procurement) không phản ứng kịp với tín hiệu bán chậm từ thị trường. Chi phí cơ hội bốc hơi tương đương ~3,387M VND/năm.

### 🛠️ Công Nghệ Sử Dụng
* **Cloud Database:** Supabase (PostgreSQL) phục vụ truy vấn nâng cao, lưu trữ và kết hợp các bảng dữ liệu thành phần.
* **Data Analytics:** Python (Pandas, NumPy) dùng để tính toán xu hướng, xử lý các logic kiểm toán tài chính và phân tích thống khai phá.

### 📁 Cấu Trúc Kho Lưu Trữ (Repository Structure)
```text
corporate-financial-health-analysis/
│
├── data/                           <- Thư mục chứa các file data
│ 
│
├── EDA.ipynb                       <- Notebook xử lý toàn bộ quy trình phân tích dữ liệu
├── Báo cáo tóm tắt.pdf             <- Báo cáo tóm tắt kết quả phân tích
└── README.md                       <- Tài liệu hướng dẫn dự án và phân tích bối cảnh tài chính
