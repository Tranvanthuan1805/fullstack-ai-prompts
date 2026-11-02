# 🧩 Prompt 3.2: Tạo Component UI Tái Sử Dụng (Responsive UI Components)

> **Mục tiêu**: Bắt AI code từng khối giao diện cụ thể (Thanh điều hướng Navbar có menu mobile, Cửa sổ bật lên Modal, Thẻ thông tin Card, Form nhập liệu có validation) để lắp ráp vào website của bạn.

---

## 📝 Nội Dung Prompt

```text
[BỐI CẢNH]
Tôi đang hoàn thiện giao diện cho website: [Tên dự án].
Tôi cần bạn viết riêng một Component (thành phần giao diện): [Tên component, ví dụ: Hộp thoại Modal thông báo nộp bài thành công / Thanh Menu Navbar thích ứng điện thoại].
Công nghệ sử dụng: [HTML + Tailwind CSS / React + Tailwind CSS / Vue.js].

[VAI TRÒ]
Bạn là Kỹ sư Giao diện (Frontend Component Specialist) với sự tỉ mỉ đến từng pixel, chú trọng trải nghiệm người dùng trên màn hình cảm ứng và khả năng truy cập (Accessibility).

[YÊU CẦU CHI TIẾT CỦA COMPONENT]
1. Thiết kế:
   - Màu sắc chủ đạo: [Ví dụ: Xanh dương indigo và tím violet / Cam san hô năng động].
   - Góc bo: Bo mềm mại (`rounded-2xl`).
   - Đổ bóng nhẹ (`shadow-lg`, `shadow-indigo-100`).
   - Hiệu ứng tương tác: Khi rê chuột vào (hover), bấm (active) đều có hiệu ứng chuyển động mượt mà (transition).
2. Tính năng tương tác (Logic JavaScript):
   - Nếu là Modal: Bấm nút thì mở ra, bấm dấu X hoặc bấm ra ngoài màn hình mờ thì đóng lại, bấm phím Escape (ESC) cũng tự động đóng.
   - Nếu là Menu Mobile: Khi ở màn hình nhỏ có nút 3 gạch (Hamburger icon), bấm vào trượt menu từ trên xuống hoặc từ cạnh sang.
   - Nếu là Form: Khi bấm nút gửi mà chưa nhập gì thì viền đỏ và báo lỗi nhẹ nhàng; khi nhập đủ thì hiện dấu tick xanh.
3. Khả năng tương thích:
   - Hiển thị hoàn hảo trên cả iPhone, máy tính bảng và màn hình desktop 4K.

[YÊU CẦU ĐẦU RA]
Cung cấp đoạn mã sạch, có phân tách rõ ràng phần HTML, CSS và JavaScript. Kèm giải thích cách chèn component này vào bất kỳ file nào trong dự án.
```

---

[⬅️ Quay lại Danh mục Prompt](../../README.md)

