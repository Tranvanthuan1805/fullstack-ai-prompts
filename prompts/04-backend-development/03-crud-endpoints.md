# 🔄 Prompt 4.3: Viết Trọn Bộ Xử Lý Thêm - Sửa - Xóa - Lấy Dữ Liệu (CRUD Operations)

> **Mục tiêu**: CRUD (Create - Read - Update - Delete) là xương sống của 95% website trên thế giới. Prompt này bắt AI viết trọn vẹn toàn bộ các hàm xử lý dữ liệu chuẩn chỉ, có phân trang, tìm kiếm và kiểm tra dữ liệu đầu vào.

---

## 📝 Nội Dung Prompt

```text
[BỐI CẢNH]
Tôi cần xây dựng bộ xử lý CRUD (Thêm, Đọc, Sửa, Xóa) cho thực thể: [Tên đối tượng, ví dụ: Bài viết thông báo / Sản phẩm / Danh sách thành viên CLB].
Backend: [Node.js Express / Next.js Server Actions / Python FastAPI].
Cơ sở dữ liệu: [PostgreSQL / Supabase / MySQL / MongoDB].

[VAI TRÒ]
Bạn là Kỹ sư Lập trình Backend Cấp cao, viết code theo tiêu chuẩn Clean Code, tách biệt tầng điều khiển (Controller), tầng dịch vụ (Service) và tầng truy vấn dữ liệu (Repository / Query).

[NHIỆM VỤ CỦA BẠN]
Hãy viết trọn bộ mã nguồn cho các chức năng sau:
1. `GET /api/items`: Lấy danh sách có hỗ trợ:
   - Phân trang (Pagination: `page`, `limit`).
   - Tìm kiếm từ khóa theo tên (Search: `?q=...`).
   - Sắp xếp (Sort theo ngày tạo mới nhất hoặc cũ nhất).
2. `GET /api/items/:id`: Lấy chi tiết 1 bản ghi theo ID (Xử lý trường hợp không tìm thấy trả về lỗi 404).
3. `POST /api/items`: Tạo mới bản ghi:
   - Kiểm tra dữ liệu đầu vào (Validation) đầy đủ trước khi lưu.
   - Trả về mã thành công 201 Created kèm dữ liệu vừa tạo.
4. `PUT /api/items/:id`: Cập nhật thông tin bản ghi.
5. `DELETE /api/items/:id`: Xóa bản ghi (hoặc Soft Delete chuyển trạng thái `is_deleted = true`).

[TIÊU CHUẨN CODE]
- Luôn bọc trong khối `try...catch` để bắt mọi ngoại lệ.
- Trả về chuẩn JSON đồng nhất: `{ success: true, message: "...", data: ... }`.
- Ghi chú tiếng Việt rõ ràng từng bước.
```

---

[⬅️ Quay lại Danh mục Prompt](../../README.md)
