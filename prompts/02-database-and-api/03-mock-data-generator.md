# 🎲 Prompt 2.3: Tự Động Sinh Dữ Liệu Mẫu (Mock Data Generator Tiếng Việt)

> **Mục tiêu**: Khi mới làm website, bạn chưa có người dùng thật. Prompt này giúp AI tự động tạo ra hàng chục dòng dữ liệu mẫu thuần Việt (họ tên, trường học, điểm số, bài viết) để dán vào cơ sở dữ liệu hoặc test giao diện ngay lập tức.

---

## 📝 Nội Dung Prompt

```text
[BỐI CẢNH]
Tôi đang hoàn thiện giao diện và thử nghiệm tính năng cho dự án: [Tên dự án, ví dụ: Ứng dụng thi đua nề nếp lớp học cấp 3].
Tôi cần dữ liệu giả lập (Mock Data) sinh động, gần gũi với đời sống học sinh và người Việt Nam.

[VAI TRÒ]
Bạn là Kỹ sư Dữ liệu (Data Engineer) kiêm Chuyên gia Kiểm thử (QA Tester). Bạn có khả năng tạo dữ liệu mẫu cực kỳ chân thực, phong phú, đa dạng và không bị trùng lặp vô lý.

[NHIỆM VỤ CỦA BẠN]
Hãy sinh cho tôi tập dữ liệu mẫu gồm [Số lượng, ví dụ: 10 - 20 bản ghi] cho các bảng: [Tên bảng hoặc đối tượng, ví dụ: Học sinh, Điểm rèn luyện, Vi phạm/Khen thưởng].

Yêu cầu về dữ liệu:
1. Tên người: Họ và tên tiếng Việt chuẩn (Nguyễn Văn An, Trần Thị Mai, Lê Quốc Huy,...), có cả nam lẫn nữ.
2. Thông tin phụ trợ: Email hợp lệ (`an.nguyen@school.edu.vn`), số điện thoại đầu số Việt Nam (`0912...`, `0988...`), địa chỉ/lớp học chân thực (12A1, 11B2, THPT Chuyên Hà Nội - Amsterdam,...).
3. Ngày tháng: Trải dài từ tháng trước đến hiện tại, có giờ phút logic.
4. Trường hợp đặc biệt (Edge Cases): Cố tình tạo 1-2 dòng có tên siêu dài, tên có dấu cách thừa, hoặc điểm số 10 tròn trĩnh để kiểm tra giao diện có bị vỡ khung không.

[ĐỊNH DẠNG ĐẦU RA]
Cung cấp dữ liệu dưới cả 2 dạng:
1. Mảng JSON (`[ { "id": 1, ... }, ... ]`) để dán trực tiếp vào code JavaScript / React.
2. Câu lệnh SQL `INSERT INTO ... VALUES (...)` để chạy thẳng vào Database.
```

---

[⬅️ Quay lại Danh mục Prompt](../../README.md)
