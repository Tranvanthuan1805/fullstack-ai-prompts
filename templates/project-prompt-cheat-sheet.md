# 📋 Tờ Phao Cứu Sinh Prompt (Prompt Engineering Cheat Sheet)
> *Lưu lại file này hoặc in ra bàn học để dùng bất cứ khi nào bạn chat với Claude, Gemini hoặc ChatGPT!*

---

## ⚡ 1. Các "Câu Lệnh Thần Chú" (One-Liner Magic Prompts)

Dưới đây là những câu lệnh ngắn nhưng có uy lực cực lớn để nắn chỉnh câu trả lời của AI:

| Mục đích | Câu lệnh mẫu bạn copy dán ngay |
| :--- | :--- |
| **Bắt AI viết code đầy đủ, không cắt xén** | *"Hãy viết đầy đủ toàn bộ mã nguồn từ đầu đến cuối, KHÔNG dùng chú thích như '// viết tiếp code ở đây' hay '// code cũ giữ nguyên'."* |
| **Bắt AI giải thích dễ hiểu** | *"Hãy giải thích nguyên lý đoạn code trên như đang giảng bài cho học sinh cấp 3 yêu thích công nghệ."* |
| **Bắt AI tự rà soát lỗi trước khi đưa code** | *"Trước khi đưa ra code, hãy tự kiểm tra lại các trường hợp ngoại lệ (Edge cases), lỗi cú pháp và lỗi bảo mật phổ biến."* |
| **Yêu cầu giao diện đẹp, hiện đại** | *"Sử dụng Tailwind CSS với phong cách thiết kế tối giản, bo tròn góc (rounded-2xl), đổ bóng mềm (soft shadows) và hiệu ứng chuyển động mượt mà."* |
| **Chia nhỏ công việc phức tạp** | *"Đừng viết code vội. Hãy liệt kê cho tôi danh sách 5 bước cần thực hiện để tôi xác nhận từng bước một."* |
| **Fix lỗi nhanh khi bị crash** | *"Tôi nhận được thông báo lỗi sau trong console: `[Dán lỗi vào đây]`. Hãy giải thích vì sao bị lỗi và đưa ra đoạn code đã sửa hoàn chỉnh."* |

---

## 🎯 2. Khung Prompt Chuẩn (5 Khối C-P-G-C-O)

Mỗi khi bạn muốn AI làm một tính năng quan trọng, hãy điền theo form mẫu này:

```text
[BỐI CẢNH - CONTEXT]
Tôi đang phát triển một website [Tên hoặc loại website, ví dụ: Web câu lạc bộ bóng đá của trường].
Đối tượng sử dụng là [Ví dụ: học sinh và thầy cô giáo].

[VAI TRÒ - PERSONA]
Bạn là một Lập trình viên Fullstack giàu kinh nghiệm, chuyên về [Next.js / Node.js / HTML Tailwind CSS] và là một người thầy hướng dẫn tận tâm.

[MỤC TIÊU - GOAL]
Hãy viết cho tôi tính năng: [Mô tả tính năng, ví dụ: Form đăng ký thành viên có kiểm tra họ tên, email, số áo thi đấu].

[RÀNG BUỘC - CONSTRAINTS]
1. Mã nguồn viết gọn trong 1 file HTML có nhúng Tailwind CSS qua CDN.
2. Kiểm tra dữ liệu hợp lệ (Validation): Tên không được để trống, email phải đúng định dạng.
3. Khi người dùng bấm Gửi thành công, hiển thị một Modal thông báo chúc mừng đẹp mắt.
4. Có chú thích tiếng Việt giải thích từng khối code.

[ĐẦU RA - OUTPUT]
Cung cấp toàn bộ mã nguồn hoàn chỉnh, sẵn sàng chạy ngay khi mở bằng trình duyệt web.
```

---

## 🤖 3. Lưu ý riêng cho từng dòng AI

### 🧠 Với Claude (Claude 3.7 / 3.5 Sonnet)
- **Điểm mạnh nhất**: Viết code Frontend cực kỳ đẹp, thẩm mỹ cao; tư duy kiến trúc và logic sâu sắc; hiểu văn cảnh dài.
- **Mẹo tối ưu**: Hãy đưa cho Claude cả file code hiện tại của bạn và yêu cầu *"Hãy giữ nguyên phong cách code và thêm tính năng X vào đúng vị trí"*.

### ⚡ Với Google Gemini (Gemini 2.5 / 1.5 Pro)
- **Điểm mạnh nhất**: Xử lý ngữ cảnh cực lớn (hàng triệu tokens), đọc hiểu tài liệu PDF, phân tích toàn bộ repository mã nguồn, tra cứu thông tin cập nhật mới nhất.
- **Mẹo tối ưu**: Bạn có thể nén toàn bộ project hoặc dán nhiều file code cùng lúc vào Gemini và yêu cầu *"Tìm điểm nghẽn hiệu năng và các lỗi tiềm ẩn trong toàn bộ dự án này"*.

### 💻 Với Cursor / Windsurf / GitHub Copilot
- **Điểm mạnh nhất**: Tự động chỉnh sửa trực tiếp vào file trong máy tính, đọc hiểu toàn bộ workspace của bạn.
- **Mẹo tối ưu**: Luôn tạo file `.cursorrules` ở thư mục gốc để dạy AI hiểu quy chuẩn code của riêng bạn.

---

⭐ **Bấm Star cho repo và Follow [@Tranvanthuan1805](https://github.com/Tranvanthuan1805) để cập nhật thêm nhiều bí kíp mới!**
