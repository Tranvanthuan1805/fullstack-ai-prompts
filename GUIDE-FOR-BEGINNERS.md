# 🎓 Cẩm Nang Vỡ Lòng: Website Hoạt Động Thế Nào & Bắt AI Làm Web Cho Bạn
> *Dành riêng cho các bạn học sinh cấp 3, sinh viên năm nhất và người mới bắt đầu từ con số 0.*

---

Chào bạn! Nếu bạn đang đọc bài viết này, có thể bạn chưa từng viết một dòng code nào trong đời, hoặc bạn từng thử học lập trình nhưng thấy quá khô khan với những thuật ngữ khó hiểu. 

Đừng lo! Hãy quên đi những giáo trình dày cộm. Bài viết này sẽ giải thích mọi thứ theo cách đời thường nhất, giúp bạn hiểu bản chất của một website và cách ra lệnh cho AI (Claude, Gemini, ChatGPT) làm việc thay bạn.

---

## 🥤 1. Website Fullstack là gì? (Hình tượng quán Trà Sữa)

Hãy tưởng tượng một website giống như **một Quán Trà Sữa hiện đại**:

```
[ Khách hàng (Bạn / Người dùng) ]
           │
           ▼ (1. Nhìn Menu, bấm gọi món)
┌───────────────────────────────────────────────┐
│              FRONTEND (MẶT TIỀN)              │
│ - Không gian quán đẹp, bảng hiệu neon lung linh│
│ - Màn hình cảm ứng để bấm chọn món, chọn size │
│ - Nút "Đặt món", "Thanh toán"                 │
└──────────────────────┬────────────────────────┘
                       │
                       ▼ (2. Nhân viên chạy bàn / shipper chuyển đơn)
              ┌─────────────────┐
              │  API (GIAO HẸN) │
              └────────┬────────┘
                       │
                       ▼ (3. Đưa đơn vào quầy pha chế)
┌───────────────────────────────────────────────┐
│              BACKEND (NHÀ BẾP)                │
│ - Quầy pha chế xử lý công thức trà sữa        │
│ - Máy tính tiền kiểm tra xem khách đủ tiền ko │
│ - Đóng nắp ly, in nhãn dán, kiểm tra đơn hàng │
└──────────────────────┬────────────────────────┘
                       │
                       ▼ (4. Lấy nguyên liệu, lưu lịch sử đơn hàng)
┌───────────────────────────────────────────────┐
│              DATABASE (KHO CHỨA)              │
│ - Tủ lạnh trữ trà, thạch, trân châu, sữa      │
│ - Cuốn sổ kế toán ghi lại danh sách khách hàng│
│ - Tên đăng nhập & Mật khẩu của tài khoản VIP  │
└───────────────────────────────────────────────┘
```

Tóm lại:
1. **Frontend (Giao diện người dùng)**: Là tất cả những gì mắt bạn nhìn thấy trên màn hình điện thoại hoặc máy tính (nút bấm, màu sắc, hình ảnh, chữ viết).
2. **Backend (Hậu trường xử lý)**: Là bộ não vận hành ngầm bên dưới mà người dùng không nhìn thấy (kiểm tra mật khẩu có đúng không, tính tổng tiền giỏ hàng, gửi email xác nhận).
3. **Database (Cơ sở dữ liệu)**: Là chiếc tủ kho lưu trữ thông tin lâu dài (bài viết, tài khoản học sinh, điểm số, lịch sử chat).
4. **API (Cầu nối)**: Là người đưa thư chuyển dữ liệu qua lại giữa Frontend và Backend.
5. **Fullstack**: Là người (hoặc hệ thống) có thể làm được **cả Frontend lẫn Backend và Database**. Và giờ đây, **AI sẽ là người làm Fullstack cho bạn**!

---

## 🛠️ 2. Bộ đồ nghề bạn cần chuẩn bị (100% Miễn Phí)

Bạn không cần mua máy tính xịn hay phần mềm đắt tiền. Chỉ cần máy tính kết nối Internet và chuẩn bị các tài khoản sau:

| Công cụ | Công dụng | Link đăng ký miễn phí |
| :--- | :--- | :--- |
| **Claude.ai** | AI viết code logic và giao diện cực kỳ thông minh | [claude.ai](https://claude.ai) |
| **Google Gemini** | AI giải thích kiến thức, tìm kiếm và sửa lỗi siêu nhanh | [gemini.google.com](https://gemini.google.com) |
| **VS Code** hoặc **Cursor** | Phần mềm để dán code vào và chạy thử trên máy | [code.visualstudio.com](https://code.visualstudio.com) |
| **GitHub** | Nơi cất giữ mã nguồn của bạn trên đám mây | [github.com](https://github.com) |
| **Vercel** | Nơi đưa website lên mạng có tên miền `.vercel.app` cho bạn bè vào xem | [vercel.com](https://vercel.com) |

---

## 🧭 3. Quy trình 3 bước "Bắt AI làm web"

### Bước 1: Nói cho AI biết bạn muốn làm cái gì (Bối cảnh & Ý tưởng)
Đừng nói chung chung: *"Hãy làm cho tôi một web bán hàng"*. AI sẽ làm ra một thứ rất nhàm chán hoặc nửa vời.
Thay vào đó, hãy nói:
> *"Tôi muốn làm một website cho Câu lạc bộ Sách của trường THPT tôi đang học. Web cần có trang chủ giới thiệu top 5 cuốn sách hay nhất tuần này, có nút để các bạn học sinh bấm 'Mượn sách' và để lại tên, lớp, số điện thoại."*

### Bước 2: Dùng bộ Prompt trong repo này theo đúng thứ tự
Vào thư mục `prompts/` của repo này, mở file tương ứng:
1. Đầu tiên, dùng prompt trong thư mục `01-ideation-and-specs` để AI vẽ ra kế hoạch.
2. Dùng prompt trong `02-database-and-api` để định hình dữ liệu lưu trữ.
3. Dùng prompt trong `03-frontend-development` để AI code ra giao diện HTML/CSS/JS.
4. Mở file HTML đó trên trình duyệt (chỉ cần nhấp đúp chuột là web mở lên!).

### Bước 3: Xem kết quả và yêu cầu AI sửa đổi (Co-work)
Nếu thấy nút màu xanh chưa đẹp, hoặc chữ hơi nhỏ:
> *"Hãy đổi màu nút 'Mượn sách' thành màu cam gradient nổi bật hơn, và phóng to chữ tiêu đề lên một chút cho dễ đọc nhé."*

---

## 💡 4. Những bí kíp sống còn khi làm việc với AI

1. **Đừng bao giờ bắt AI làm toàn bộ web khổng lồ trong 1 câu lệnh duy nhất**:
   - Hãy chia nhỏ ra: Làm trang chủ trước $\rightarrow$ làm trang chi tiết sau $\rightarrow$ làm form liên hệ $\rightarrow$ nối cơ sở dữ liệu.
2. **Khi gặp lỗi (chữ đỏ báo lỗi xuất hiện)**:
   - Đừng hoảng sợ! Copy toàn bộ dòng chữ lỗi đó kèm ảnh chụp màn hình (nếu có), mở prompt `05-debugging-and-testing/01-smart-error-debugger.md` và dán cho AI. AI sẽ chỉ ra ngay dòng nào bị sai và cách sửa trong 5 giây!
3. **Luôn yêu cầu AI giải thích**:
   - Nếu thấy dòng code nào khó hiểu, bạn chỉ cần gõ: *"Hãy giải thích cho một học sinh lớp 11 hiểu đoạn code trên làm nhiệm vụ gì bằng ví dụ thực tế"*. Bạn sẽ vừa có sản phẩm chạy được, vừa hiểu sâu kiến thức!

---

## 🚀 Bây giờ hãy bắt đầu!

👉 Hãy mở ngay [**templates/sample-project-todo-app/README.md**](templates/sample-project-todo-app/README.md) để tự tay làm ra website đầu tiên trong đời chỉ với 15 phút!
