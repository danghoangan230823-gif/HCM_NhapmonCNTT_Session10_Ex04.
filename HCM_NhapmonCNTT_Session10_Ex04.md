# Bài 4 : Thiết kế Prompt tối ưu cho AI Assistant
## 🌱 Mô hình IPO trong trang trại thông minh
> Câu trả lời của AI sau khi áp dụng Prompt trong file `prompt.md`.
## 1. IPO là gì? 
Mục đích: Huy động nguồn vốn lớn, nâng cao uy tín thương hiệu và chuyển từ công ty tư nhân thành công ty đại chúng.

Lợi ích: Dễ gọi vốn dài hạn, tăng tính thanh khoản cho cổ đông sáng lập.

Thách thức: Phải minh bạch báo cáo tài chính, tốn chi phí pháp lý và giảm quyền kiểm soát của ban sáng lập.
### Hãy bắt đầu từ nồi cơm điện 🍚
- Đầu tiên **cho gạo, nước và bấm nút** -> đó là **input** (đầu vào)
- Nồi **làm nóng, canh nhiệt độ, tính thời gian** → đó là **Process** (Xử lý)
- Nồi **cho ra cơm chín** → đó là **Output** (Đầu ra)

**IPO** chỉ là cách chia một hệ thống thành 3 bước: **nhận vào → xử lý → trả ra**.
## 2. Áp dụng vào trang trại: tưới cây tự động 💧
Tình huống: vườn rau cần tưới nước khi đất khô.

| 📥 Input (Đầu vào) | ⚙️ Process (Xử lý) | 📤 Output (Đầu ra) |
|---|---|---|
| Độ ẩm đất | So sánh với mức cần thiết: đất khô không | Bật hoặc tắt máy bơm nước |

## 3. Sơ đồ luồng
```
Đổ ẩm đất -> đất khô mất cần? -> Bật máy bơm
(Input)      (Process)           (Output)
```

Nếu đất đã đủ ẩm, bước Xử lý quyết định **không làm gì**, và máy bơm tắt.

## 4. Vì sao phải chia 3 khối?

- Dễ **hiểu**: mỗi khối chỉ làm một việc
- Dễ **sửa lỗi**: bơm không chạy thì biết kiểm tra từ khối nào
- Dễ **mở rộng**: muốn tưới theo giờ, chỉ cần thêm Input mới
## 5. ✅ Tự kiểm tra

- [ ] Trong ví dụ nồi cơm, đâu là Input, Process, Output?
- [ ] Trong vườn rau, cái gì đóng vai trò Process?
- [ ] Nếu muốn bật đèn khi trời tối, Input sẽ là gì?

<details>
<summary>Xem gợi ý đáp án</summary>

1. Input: gạo, nước, nút bấm. Process: làm nóng và canh nhiệt. Output: cơm chín.
2. Bước so sánh độ ẩm đất với mức cần thiết.
3. Độ sáng của môi trường.

</details>
