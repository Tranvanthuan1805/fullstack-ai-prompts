# 🧪 Prompt 5.3: Tự Động Viết Kiểm Thử Tự Động (Unit Test Generator)

> **Mục tiêu**: Một lập trình viên chuyên nghiệp luôn có các đoạn test tự động để đảm bảo sau khi thêm tính năng mới, các tính năng cũ không bị hỏng (regression bugs). Prompt này bắt AI viết bài kiểm tra tự động chạy trong 1 giây.

---

## 📝 Nội Dung Prompt

```text
[BỐI CẢNH]
Tôi vừa hoàn thành một hàm chức năng / component trong dự án: [Tên dự án].
Công nghệ kiểm thử: [Jest / Vitest / Pytest / Cypress].

[ĐOẠN CODE CẦN VIẾT TEST]
```javascript
[DÁN ĐOẠN CODE HÀM HOẶC COMPONENT VÀO ĐÂY]
```

[VAI TRÒ]
Bạn là Kỹ sư Đảm bảo Chất lượng Phần mềm (Senior QA / Test Automation Engineer). Bạn luôn suy nghĩ về các kịch bản người dùng thao tác quái chiêu nhất để tìm ra lỗi tiềm ẩn.

[NHIỆM VỤ CỦA BẠN]
Hãy viết trọn bộ mã nguồn Unit Test bao gồm:
1. Trường hợp bình thường (Happy Path): Dữ liệu đầu vào đúng chuẩn thì kết quả trả về phải chính xác.
2. Trường hợp biên (Boundary Cases): Số 0, số âm, chuỗi rỗng `""`, giá trị `null` hoặc `undefined`.
3. Trường hợp dữ liệu sai (Negative / Error Cases): Nhập sai kiểu dữ liệu, vượt quá độ dài cho phép thì hệ thống phải ném ra lỗi mong đợi.
4. Hướng dẫn lệnh chạy test trên terminal (ví dụ: `npm test`) và cách đọc kết quả test xanh lá cây (PASS).
```

---

[⬅️ Quay lại Danh mục Prompt](../../README.md)

