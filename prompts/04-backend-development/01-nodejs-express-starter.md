# ⚙️ Prompt 4.1: Khởi Tạo Server Backend Nhanh Gọn (Node.js & Express)

> **Mục tiêu**: Ra lệnh cho AI tạo một máy chủ Backend hoàn chỉnh bằng Node.js và Express từ con số 0, có cấu trúc thư mục rõ ràng, xử lý CORS, đọc file môi trường `.env` và kết nối cơ sở dữ liệu.

---

## 📝 Nội Dung Prompt

```text
[BỐI CẢNH]
Tôi đang bắt đầu xây dựng phần Backend cho ứng dụng web của mình: [Tên dự án].
Tôi sử dụng môi trường Node.js với Express.js.
Tôi là người mới bắt đầu, cần cấu trúc code sạch sẽ, dễ mở rộng và dễ hiểu nhất.

[VAI TRÒ]
Bạn là Kỹ sư Backend Cấp cao (Senior Backend Engineer) am hiểu sâu sắc về kiến trúc ứng dụng Node.js hiện đại, bảo mật và hiệu năng cao.

[NHIỆM VỤ CỦA BẠN]
1. Hướng dẫn từng bước lệnh terminal để tôi khởi tạo project:
   - Các lệnh `npm init` và `npm install` các thư viện thiết yếu (`express`, `cors`, `dotenv`, `helmet`, `morgan`).
2. Thiết kế cấu trúc thư mục chuẩn (Clean Architecture):
   ```text
   src/
   ├── controllers/  (Xử lý logic từng tính năng)
   ├── routes/       (Định tuyến các đường link API)
   ├── middlewares/  (Bộ lọc kiểm tra lỗi và bảo mật)
   ├── config/       (Cấu hình Database và biến môi trường)
   └── server.js     (Điểm khởi chạy chính của ứng dụng)
   ```
3. Viết mã nguồn hoàn chỉnh cho file `src/server.js`:
   - Cấu hình Middleware cơ bản (xử lý JSON, giải quyết vấn đề chặn tên miền CORS, ghi log request bằng morgan).
   - Một endpoint kiểm tra tình trạng server: `GET /api/health` trả về trạng thái "OK" và thời gian hiện tại.
   - Cơ chế bắt lỗi tập trung (Global Error Handler) để server không bao giờ bị sập đột ngột khi xảy ra ngoại lệ.
4. Cung cấp file mẫu `.env.example` và hướng dẫn cách khởi chạy server bằng lệnh `node` hoặc `nodemon`.

[YÊU CẦU ĐẶC BIỆT]
Mỗi file code đều có dòng chú thích tiếng Việt giải thích công dụng của từng dòng để học sinh mới tiếp cận cũng hiểu vì sao cần viết như thế.
```

---

[⬅️ Quay lại Danh mục Prompt](../../README.md)

