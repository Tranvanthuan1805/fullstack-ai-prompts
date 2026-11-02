# ⏱️ Dự Án Thực Hành 15 Phút: "Sổ Tay Bài Tập Thông Minh"
> *Dành cho người mới: Tự tay tạo ra một ứng dụng Web có lưu dữ liệu thực tế mà không cần học code trước!*

---

## 🎯 Mục tiêu dự án
Chỉ sau 15 phút, bạn sẽ có một trang web mang tên **"Sổ Tay Bài Tập Về Nhà Thông Minh"** chạy ngay trên máy tính của bạn với các tính năng:
- ✅ Thêm bài tập mới (Tên môn học, hạn nộp, mức độ ưu tiên: Cao / Vừa / Thấp).
- ✅ Đánh dấu bài tập đã hoàn thành (gạch ngang và đổi màu).
- ✅ Xóa bài tập cũ.
- ✅ Tự động lưu vào máy tính (Dù bạn tắt máy hay tải lại trang, dữ liệu vẫn còn nguyên nhờ `localStorage`!).
- ✅ Giao diện hiện đại, có chế độ Sáng / Tối (Dark mode).

---

## 🚀 Cách thực hiện trong 3 bước siêu đơn giản

### Bước 1: Tạo một file trắng trên máy tính
1. Tạo một thư mục mới trên máy tính (ví dụ tên là `so-tay-hoc-tap`).
2. Mở Notepad hoặc VS Code, tạo một file mới và lưu lại với tên: `index.html`.

---

### Bước 2: Copy Prompt dưới đây và gửi cho Claude hoặc Gemini

Hãy copy toàn bộ đoạn văn bản bên dưới, mở **Claude.ai** hoặc **Gemini** và dán vào:

```text
Bạn là một Chuyên gia Lập trình Web Fullstack và một Giáo viên Tin học nhiệt tình.
Tôi là một học sinh cấp 3 muốn tạo một website nhỏ mang tên "Sổ Tay Bài Tập Về Nhà Thông Minh".

Yêu cầu kỹ thuật:
1. Hãy viết tất cả trong DUY NHẤT 1 file HTML (đã bao gồm giao diện CSS bằng Tailwind CSS qua CDN và mã xử lý JavaScript).
2. Các tính năng cần có:
   - Một thanh tiêu đề đẹp mắt có biểu tượng sách vở và nút chuyển chế độ Giao diện Sáng / Tối.
   - Form nhập: Tên bài tập, Chọn môn học (Toán, Lý, Hóa, Văn, Anh, Tin, Khác), Hạn nộp (ngày giờ), và Mức độ khẩn cấp (Quan trọng, Bình thường).
   - Nút "Thêm bài tập" có hiệu ứng nhấp chuột đẹp mắt.
   - Danh sách bài tập hiển thị dạng thẻ (Card) gọn gàng. Mỗi thẻ có:
     + Nút checkbox để đánh dấu "Đã làm xong".
     + Thẻ nhãn môn học có màu sắc riêng biệt.
     + Nút thùng rác màu đỏ để xóa bài tập.
   - Tự động lưu tất cả dữ liệu vào localStorage của trình duyệt để không bị mất khi F5 hoặc tắt máy.
   - Bộ lọc xem: "Tất cả", "Chưa hoàn thành", "Đã xong".
3. Thiết kế:
   - Hiện đại, bo góc mềm mại (rounded-2xl), màu sắc trẻ trung (xanh pastel, tím nhẹ), hỗ trợ tốt cả trên điện thoại lẫn máy tính.
4. Chú thích tiếng Việt rõ ràng ở các đoạn quan trọng để tôi học hỏi.

Hãy cung cấp toàn bộ mã nguồn file index.html đầy đủ từ thẻ <!DOCTYPE html> đến </html>, không viết tắt, sẵn sàng để tôi lưu và chạy ngay.
```

---

### Bước 3: Dán code vào file và mở lên xem thành quả!
1. Khi AI trả lời xong, bạn bấm nút **Copy Code** của AI.
2. Dán toàn bộ nội dung đó vào file `index.html` bạn đã tạo ở Bước 1.
3. Bấm **Ctrl + S** (lưu lại).
4. Nhấp đúp chuột vào file `index.html` $\rightarrow$ Trình duyệt web (Chrome, Edge, Cốc Cốc) sẽ mở lên!
5. 🎉 **Chúc mừng bạn! Bạn vừa tạo xong một ứng dụng web hoàn chỉnh cho riêng mình!**

---

## 🌟 Thử thách nâng cấp (Học thêm cùng AI)
Sau khi web đã chạy ngon lành, hãy thử nhắn tiếp cho AI:
- *"Hãy thêm tính năng đếm ngược thời gian (Countdown) cho các bài tập sắp đến hạn nộp nhé!"*
- *"Hãy thêm âm thanh chúc mừng 'ting ting' mỗi khi tôi bấm hoàn thành một bài tập!"*

---

⭐ **Thấy dễ và thú vị đúng không? Hãy quay lại trang chủ và tặng 1 ⭐ Star cho repo nhé!**
👉 [Quay lại Trang Chủ README](../../README.md)
