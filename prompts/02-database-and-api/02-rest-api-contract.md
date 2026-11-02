# 🌐 Prompt 2.2: Thiết Kế Chuẩn Giao Tiếp RESTful API (API Contract)

> **Mục tiêu**: Lên danh sách toàn bộ các đường link API (Endpoints) kết nối giữa Giao diện (Frontend) và Hệ thống xử lý (Backend), quy định rõ gửi đi cái gì và nhận về cái gì theo chuẩn JSON.

---

## 📝 Nội Dung Prompt

```text
[BỐI CẢNH]
Tôi đang xây dựng giao tiếp API cho ứng dụng: [Tên dự án, ví dụ: Ứng dụng Quản lý Câu lạc bộ Học sinh].
Các thực thể chính: [Ví dụ: Thành viên, Hoạt động/Sự kiện, Điểm danh].

[VAI TRÒ]
Bạn là Kiến trúc sư API (API Architect) tuân thủ nghiêm ngặt nguyên tắc RESTful API chuẩn quốc tế.

[NHIỆM VỤ CỦA BẠN]
Hãy thiết kế tài liệu API Specification chi tiết với bảng tổng hợp gồm các cột:
1. Phương thức HTTP (GET, POST, PUT, DELETE).
2. Đường dẫn Endpoint (ví dụ: `/api/v1/members`, `/api/v1/activities/:id`).
3. Mô tả chức năng (Thêm mới, xem chi tiết, cập nhật, xóa).
4. Quyền truy cập (Public ai cũng gọi được, hay Phải đăng nhập, hay Chỉ Admin).

Với mỗi API quan trọng, hãy cung cấp ví dụ cụ thể:
- Request Body (Dữ liệu gửi lên dạng JSON).
- Success Response (Mã 200/201 kèm dữ liệu JSON trả về).
- Error Response (Mã 400/401/404/500 kèm thông báo lỗi rõ ràng).

[QUY CHUẨN ĐẦU RA]
Định dạng JSON chuẩn chuẩn hoá:
```json
{
  "success": true,
  "message": "Thông báo thân thiện",
  "data": { ... }
}
```
Kèm giải thích dễ hiểu cho học sinh mới học về REST API: "GET để lấy, POST để tạo, PUT để sửa, DELETE để xóa".
```

---

[⬅️ Quay lại Danh mục Prompt](../../README.md)
