# 🔐 Prompt 4.2: Tích Hợp Xác Thực Người Dùng (Đăng Ký, Đăng Nhập, Auth JWT / Supabase)

> **Mục tiêu**: Hướng dẫn xây dựng tính năng Đăng ký, Đăng nhập, Mã hóa mật khẩu bảo mật (bcrypt), Tạo thẻ bài đăng nhập (JWT token hoặc Supabase Auth) và Phân quyền (Role-based Authorization: Admin / User / Học sinh / Giáo viên).

---

## 📝 Nội Dung Prompt

```text
[BỐI CẢNH]
Tôi cần xây dựng hệ thống Xác thực và Phân quyền (Authentication & Authorization) cho ứng dụng: [Tên dự án].
Công nghệ sử dụng: [Node.js + Express + JWT + bcrypt / HOẶC Supabase Auth].
Đối tượng người dùng có 2 phân quyền:
1. `USER` (Học sinh/Người dùng thông thường).
2. `ADMIN` (Ban quản trị/Thầy cô giáo quản lý).

[VAI TRÒ]
Bạn là Chuyên gia Bảo mật Ứng dụng Web (Web Application Security Specialist). Bạn luôn đặt tiêu chí an toàn thông tin lên hàng đầu (bảo vệ chống hack, băm mật khẩu chuẩn, ngăn chặn tấn công giả mạo token).

[NHIỆM VỤ CỦA BẠN]
1. Viết API Đăng ký tài khoản (`POST /api/auth/register`):
   - Nhận vào: `email`, `password`, `fullName`.
   - Kiểm tra xem email đã tồn tại trong hệ thống chưa.
   - Băm mật khẩu an toàn bằng `bcrypt` (độ phức tạp salt rounds = 10), tuyệt đối không lưu mật khẩu trần dạng chữ thường.
   - Lưu vào cơ sở dữ liệu.
2. Viết API Đăng nhập (`POST /api/auth/login`):
   - Nhận vào: `email`, `password`.
   - Kiểm tra email và so khớp mật khẩu đã băm.
   - Nếu đúng: Ký và phát hành JSON Web Token (JWT) có hạn sử dụng (ví dụ: 7 ngày).
   - Nếu sai: Trả về thông báo chung "Email hoặc mật khẩu không chính xác" (tránh lộ thông tin email có tồn tại hay không).
3. Viết Middleware Xác thực và Phân quyền:
   - `verifyToken`: Kiểm tra xem người dùng có mang theo thẻ JWT hợp lệ trong Header (`Authorization: Bearer <token>`) không.
   - `requireAdmin`: Chỉ cho phép người dùng có `role === 'ADMIN'` đi tiếp vào các trang quản lý.
4. Viết Endpoint kiểm tra thông tin cá nhân: `GET /api/auth/me` để Frontend lấy thông tin người dùng đang đăng nhập.

[GIẢI THÍCH CHO NGƯỜI MỚI]
Giải thích cơ chế JWT token bằng hình ảnh đời thường: "JWT giống như chiếc vòng đeo tay check-in ở công viên nước, đeo vào là đi qua được các cổng soát vé".
```

---

[⬅️ Quay lại Danh mục Prompt](../../README.md)
