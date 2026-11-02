# 🔒 Prompt 6.2: Cẩm Nang Quản Lý Biến Môi Trường (.env) An Toàn (Không Bị Lộ Mật Khẩu)

> **Mục tiêu**: Khi làm web có kết nối API Key, mật khẩu Database hay token bí mật, nếu vô tình đẩy lên GitHub công khai thì kẻ xấu có thể quét và chiếm đoạt tài khoản. Prompt này giúp bạn tạo lá chắn bảo vệ thông tin mật.

---

## 📝 Nội Dung Prompt

```text
[BỐI CẢNH]
Tôi đang kết nối dự án của mình với dịch vụ bên ngoài (ví dụ: Google Gemini API Key, OpenAI API Key, chuỗi kết nối Supabase / MongoDB).
Tôi chuẩn bị đưa code lên GitHub công khai và muốn đảm bảo các khóa bí mật của tôi 100% không bị lộ ra ngoài.

[VAI TRÒ]
Bạn là Chuyên gia An toàn Thông tin và DevOps Cấp cao. Bạn hướng dẫn nguyên tắc thực hành tốt nhất (Best Practices) về quản lý biến môi trường.

[NHIỆM VỤ CỦA BẠN]
1. Hướng dẫn thiết lập file `.gitignore`:
   - Cách tạo file `.gitignore` ở thư mục gốc và các dòng cần có để Git tự động bỏ qua file `.env`.
2. Tạo file mẫu an toàn `.env.example`:
   - Chỉ cho tôi cách tạo file `.env.example` chứa các tên biến giả lập để người khác clone repo về biết cần điền những thông tin gì mà không thấy mật khẩu thật.
3. Cách đọc biến môi trường trong code:
   - Cách gọi `process.env.TEN_BIEN` an toàn trong Node.js / Next.js / Vite.
4. Cách cài đặt biến môi trường khi deploy lên Vercel / Render:
   - Vào mục Settings -> Environment Variables trong trang quản trị Vercel để dán key thật như thế nào?
5. Cảnh báo cấp cứu khẩn cấp:
   - Nếu lỡ tay commit và đẩy file `.env` chứa API Key lên GitHub rồi thì phải xử lý khẩn cấp những bước nào ngay lập tức?
```

---

[⬅️ Quay lại Danh mục Prompt](../../README.md)
