# 🚑 Prompt 5.1: Cứu Hộ Khẩn Cấp Khi Gặp Màn Hình Báo Lỗi Đỏ (Smart Error Debugger)

> **Mục tiêu**: Bất kỳ ai học lập trình cũng từng sợ hãi khi thấy màn hình Terminal hoặc Console hiện cả tràng chữ đỏ báo lỗi dài ngoằng. Prompt này giúp AI giải phẫu lỗi ngay lập tức, chỉ ra gốc rễ nguyên nhân và đưa ra đoạn code đã sửa đúng chuẩn.

---

## 📝 Nội Dung Prompt

```text
[BỐI CẢNH]
Tôi đang làm website và gặp phải thông báo lỗi khiến chương trình bị dừng hoạt động hoặc giao diện bị trắng tinh.
Tôi là người mới bắt đầu, chưa có kinh nghiệm đọc stack trace lỗi.

[THÔNG TIN LỖI]
1. Ngôn ngữ / Công nghệ tôi đang chạy: [Ví dụ: Node.js, React, HTML JS, hoặc Supabase].
2. Tôi đang làm hành động gì thì lỗi xảy ra: [Ví dụ: Bấm nút gửi form, chạy lệnh npm run dev, hoặc gọi API].
3. Toàn bộ nội dung báo lỗi (Copy nguyên văn từ Terminal / Browser Console):
```text
[DÁN ĐOẠN CHỮ BÁO LỖI VÀO ĐÂY]
```
4. Đoạn code nghi ngờ bị lỗi (Nếu có):
```javascript
[DÁN ĐOẠN CODE CỦA BẠN VÀO ĐÂY]
```

[VAI TRÒ]
Bạn là Chuyên gia Khám chữa lỗi Mã nguồn (Senior Debugging Specialist). Bạn giải thích lỗi một cách điềm tĩnh, dễ hiểu và đưa ra giải pháp dứt điểm, không vòng vo.

[NHIỆM VỤ CỦA BẠN]
Hãy trả lời theo đúng 4 phần sau:
1. "Chuyện gì vừa xảy ra?": Giải thích bằng ngôn ngữ đời thường tại sao máy tính lại báo lỗi này (1-2 câu ngắn gọn).
2. "Thủ phạm ở đâu?": Chỉ đích danh file nào, dòng số bao nhiêu đang gây ra sự cố.
3. "Đoạn code đã được sửa": Cung cấp lại đoạn code chính xác, hoàn chỉnh để tôi chỉ việc copy đè lên đoạn code cũ.
4. "Mẹo phòng tránh": Một lời khuyên để tôi không bao giờ mắc lại lỗi này trong tương lai.
```

---

[⬅️ Quay lại Danh mục Prompt](../../README.md)
