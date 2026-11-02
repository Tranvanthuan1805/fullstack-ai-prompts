# 🗄️ Prompt 2.1: Thiết Kế Bảng Dữ Liệu Chuẩn (Database Schema Design)

> **Mục tiêu**: Hướng dẫn AI thiết kế cấu trúc bảng cơ sở dữ liệu (PostgreSQL, Supabase, MySQL) hoàn chỉnh, có khóa chính (Primary Key), khóa ngoại (Foreign Key), các ràng buộc và lệnh SQL sẵn sàng chạy.

---

## 📝 Nội Dung Prompt

```text
[BỐI CẢNH]
Tôi đang làm phần lưu trữ dữ liệu cho ứng dụng: [Tên dự án, ví dụ: Hệ thống thi trắc nghiệm trực tuyến cho học sinh].
Dự án có các đối tượng dữ liệu cần lưu như: [Ví dụ: Người dùng/Học sinh, Môn học, Đề thi, Câu hỏi trắc nghiệm, Lịch sử làm bài và Điểm số].
Tôi dự định dùng Cơ sở dữ liệu: [Supabase / PostgreSQL / MySQL / SQLite].

[VAI TRÒ]
Bạn là Chuyên gia Thiết kế Cơ sở Dữ liệu (Database Architect) giàu kinh nghiệm. Bạn luôn tuân thủ các nguyên tắc chuẩn hóa dữ liệu, tối ưu truy vấn và đặt tên bảng, cột theo chuẩn quốc tế.

[NHIỆM VỤ CỦA BẠN]
1. Thiết kế Danh sách các Bảng (Tables) kèm mô tả:
   - Tên bảng (dạng số nhiều, chữ thường, ví dụ: `users`, `quizzes`, `questions`, `quiz_submissions`).
   - Danh sách các cột: Tên cột, Kiểu dữ liệu (UUID, VARCHAR, INT, TIMESTAMP, BOOLEAN, JSONB,...), Ràng buộc (NOT NULL, UNIQUE, DEFAULT), Ý nghĩa của cột.
   - Xác định rõ Khóa chính (Primary Key) và Khóa ngoại (Foreign Key) tạo liên kết giữa các bảng.
2. Vẽ sơ đồ quan hệ thực thể (ERD Diagram) bằng cú pháp Mermaid:
   - Thể hiện rõ quan hệ 1-1, 1-Nhiều (1-N) hoặc Nhiều-Nhiều (N-N).
3. Cung cấp toàn bộ câu lệnh SQL (DDL):
   - Mã lệnh `CREATE TABLE ...` hoàn chỉnh, có sẵn `created_at` tự động lấy thời gian hiện tại.
   - Thiết lập chỉ mục (Indexes) cho các cột thường xuyên tìm kiếm.
   - Sẵn sàng để copy dán chạy ngay trong SQL Editor của Supabase hoặc DBeaver.

[LƯU Ý]
- Giải thích bằng tiếng Việt dễ hiểu vì sao lại liên kết bảng như vậy để người mới học hiểu được bản chất.
```

---

[⬅️ Quay lại Danh mục Prompt](../../README.md)
