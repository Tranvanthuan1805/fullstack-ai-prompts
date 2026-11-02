# 📊 Prompt 3.3: Dựng Dashboard Quản Trị Hiện Đại (Admin Dashboard)

> **Mục tiêu**: Tạo trang tổng quan quản trị (Dashboard) chuyên nghiệp như các hệ thống của tập đoàn lớn, có biểu đồ tương tác, thống kê số liệu tăng trưởng, bảng dữ liệu lọc và tìm kiếm nhanh.

---

## 📝 Nội Dung Prompt

```text
[BỐI CẢNH]
Tôi cần xây dựng một trang Quản trị (Admin Dashboard) cho: [Tên dự án, ví dụ: Hệ thống Quản lý Học sinh và Điểm danh của Lớp học].
Người sử dụng: Thầy cô giáo chủ nhiệm, Ban cán sự lớp hoặc Quản trị viên.

[VAI TRÒ]
Bạn là Kiến trúc sư Giao diện Quản trị Cấp cao (Senior Dashboard Designer) chuyên xây dựng các hệ thống SaaS và CRM triệu người dùng.

[YÊU CẦU CÔNG NGHỆ]
- Viết trong 1 file HTML duy nhất kết hợp Tailwind CSS qua CDN.
- Sử dụng Chart.js qua CDN (`<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>`) để vẽ biểu đồ trực quan.

[CẤU TRÚC GIAO DIỆN QUẢN TRỊ]
1. Sidebar bên trái:
   - Logo trường/lớp, Menu điều hướng (Tổng quan, Học sinh, Điểm danh, Báo cáo thống kê, Cài đặt).
   - Thông tin tài khoản admin ở góc dưới kèm nút Đăng xuất.
2. Topbar bên trên:
   - Thanh tìm kiếm thông minh (Search bar).
   - Nút chuông thông báo (có chấm đỏ số thông báo mới).
   - Avatar người dùng và nút chuyển giao diện Tối/Sáng.
3. Khu vực nội dung chính:
   - 4 Thẻ KPI (Metric Cards):
     + Thẻ 1: Tổng số học sinh (Kèm % tăng giảm so với tháng trước).
     + Thẻ 2: Tỷ lệ chuyên cần / có mặt hôm nay (Ví dụ: 98.5%).
     + Thẻ 3: Số bài tập đã nộp đúng hạn.
     + Thẻ 4: Điểm trung bình cả lớp (Kèm biểu đồ mini).
   - Khối Biểu đồ (Charts):
     + Biểu đồ đường (Line Chart): Diễn biến điểm số học tập qua từng tuần.
     + Biểu đồ tròn (Doughnut Chart): Cơ cấu học lực (Giỏi, Khá, Trung bình).
   - Bảng Dữ liệu (Data Table):
     + Danh sách học sinh: Ảnh đại diện, Họ tên, Mã học sinh, Lớp, Điểm số, Trạng thái (Đang học / Nghỉ phép), Thao tác (Xem / Sửa / Xóa).
     + Có ô tìm kiếm học sinh theo tên và bộ lọc theo lớp.
     + Phân trang (Pagination) ở dưới chân bảng.

[YÊU CẦU ĐẦU RA]
File HTML hoàn chỉnh, có sẵn dữ liệu mẫu để mở lên là thấy biểu đồ hoạt động và hiển thị dữ liệu sống động ngay lập tức.
```

---

[⬅️ Quay lại Danh mục Prompt](../../README.md)
