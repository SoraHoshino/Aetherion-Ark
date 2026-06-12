# Aetherion Ark

Userscript cho **Magic Garden**.

Hiện có 2 phiên bản:

* **Aetherion Ark 1.0**: bản nhẹ, chỉ tập trung vào **Auto Buy shop**.
* **Aetherion Ark 2.0**: bản **Full Mod Menu**, có nhiều công cụ hỗ trợ hơn ngoài Auto Buy.

Made by **Raizel**.

Script hoạt động trên:

```text
Magic Garden Web
Discord Web
Magic Circle
Starweaver
```

Không hoạt động trên app desktop nếu app không hỗ trợ userscript.

---

## Phiên bản

### Aetherion Ark 1.0 — Stock Buyer

Bản 1.0 là bản nhẹ, chỉ có chức năng chính là **theo dõi shop và tự động mua item đã chọn khi shop còn hàng**.

Phù hợp cho người chỉ cần auto buy đơn giản, không cần mod menu nhiều chức năng.

Tải bản 1.0 tại đây:
[Aetherion Ark 1.0 - Stock Buyer](https://github.com/SoraHoshino/Aetherion-Ark/raw/refs/heads/main/aetherion-ark-1.0.user.js)

---

### Aetherion Ark 2.0 — Full Mod Menu

Bản 2.0 là bản mod menu đầy đủ hơn, có nhiều chức năng hỗ trợ trong game ngoài Auto Buy.

Phù hợp cho người muốn dùng nhiều công cụ hơn trong một menu tổng hợp.

Tải bản 2.0 tại đây:
[Aetherion Ark 2.0 - Full Mod Menu](https://github.com/SoraHoshino/Aetherion-Ark/raw/refs/heads/main/aetherion-ark-2.0.user.js)

---

## Cài đặt cho người mới

### Bước 1: Cài Tampermonkey

1. Mở Google.
2. Tìm kiếm:

```text
Tampermonkey Chrome Web Store
```

3. Mở trang Tampermonkey trên Chrome Web Store.
4. Bấm:

```text
Thêm vào Chrome / Add to Chrome
```

5. Bấm tiếp:

```text
Thêm tiện ích / Add extension
```

Sau khi cài xong, góc phải trình duyệt sẽ có biểu tượng tiện ích hình mảnh ghép.

---

### Bước 2: Bật quyền cho Tampermonkey

1. Nhìn góc phải trên Chrome, bấm biểu tượng **mảnh ghép**.
2. Tìm **Tampermonkey**.
3. Có thể bấm ghim để hiện icon Tampermonkey ra ngoài thanh công cụ.
4. Mở trang quản lý tiện ích bằng cách nhập vào thanh địa chỉ:

```text
chrome://extensions
```

5. Bật:

```text
Chế độ nhà phát triển / Developer mode
```

6. Tìm **Tampermonkey**.
7. Bấm:

```text
Chi tiết / Details
```

8. Bật:

```text
Cho phép tập lệnh của người dùng / Allow User Scripts
```

9. Ở phần quyền truy cập trang web, chọn:

```text
Trên tất cả trang web / On all sites
```

Nếu không muốn bật cho tất cả trang, có thể chỉ cho phép riêng các trang Magic Garden.

---

### Bước 3: Cài script

Chọn phiên bản muốn dùng:

[Aetherion Ark 1.0 - Stock Buyer](https://github.com/SoraHoshino/Aetherion-Ark/raw/refs/heads/main/aetherion-ark-1.0.user.js)

[Aetherion Ark 2.0 - Full Mod Menu](https://github.com/SoraHoshino/Aetherion-Ark/raw/refs/heads/main/aetherion-ark-2.0.user.js)

Sau khi bấm link, Tampermonkey sẽ tự mở trang cài đặt.

Bấm:

```text
Install / Cài đặt
```

Nếu đã cài bản cũ, bấm:

```text
Reinstall / Cài lại
```

---

### Bước 4: Mở game

1. Vào Magic Garden.
2. Reload trang bằng:

```text
Ctrl + F5
```

3. Chờ bảng / menu của script hiện lên trong game.

---

# Aetherion Ark 1.0 - Stock Buyer

## Chức năng chính

Bản 1.0 chỉ tập trung vào **Auto Buy shop**.

Hỗ trợ:

```text
Tự động quét shop
Tự động mua item đã chọn khi còn hàng
Thêm hoặc xóa item khỏi danh sách mua
Mua nhanh một lần
Bật hoặc tắt Auto Mode
Chọn thời gian quét shop
Chọn số lượng mua tối đa
Xem log mua hàng
Xem thống kê số item đã mua và coin đã dùng
```

Hỗ trợ các nhóm item:

```text
Seed
Egg
Tool
Decor
```

---

## Cách dùng bản 1.0

1. Vào game và chờ panel hiện lên.
2. Chọn item muốn mua trong danh sách.
3. Bấm nút:

```text
+
```

4. Bấm **Mua nhanh** nếu muốn quét shop ngay một lần.
5. Bật **Auto: ON** nếu muốn script tự quét theo chu kỳ.

---

## Tùy chọn bản 1.0

### Quét mỗi

Chọn thời gian giữa mỗi lần quét shop.

Ví dụ:

```text
5s
1m
3m
5m
10m
```

### Mua tối đa

Chọn số lượng tối đa mỗi item trong một lần quét.

Ví dụ:

```text
1
3
5
10
20
Max Stock
```

Nếu chọn **Max Stock**, script sẽ mua theo số lượng còn lại trong shop.

Ví dụ:

```text
Mua tối đa = 10
Shop chỉ còn 3 item
Script chỉ mua tối đa 3 item
```

---

## Log thường gặp bản 1.0

```text
Đã mua
Mua thành công.

Hết hàng
Shop không còn item đó.

Túi đồ đầy
Inventory đã đầy, script dừng mua.

Lỗi lấy dữ liệu shop
Script chưa đọc được dữ liệu shop.

Không mua được
Game không xác nhận stock giảm hoặc inventory tăng.
```

---

# Aetherion Ark 2.0 - Full Mod Menu

## Chức năng chính

Bản 2.0 là bản **Full Mod Menu**, nhiều chức năng hơn bản 1.0.

Có thể bao gồm nhiều công cụ hỗ trợ như:

```text
Auto Buy / Stock Buyer
Công cụ liên quan inventory
Công cụ liên quan pet
Công cụ liên quan garden
Công cụ notifier / thông báo
Một số tiện ích hỗ trợ chơi Magic Garden
```

Bản 2.0 phù hợp với người muốn dùng nhiều tính năng trong một menu tổng hợp.

---

## Lưu ý về bản 2.0

```text
Bản 2.0 có nhiều chức năng hơn nên file sẽ nặng hơn bản 1.0.
Nếu chỉ cần auto mua shop đơn giản, nên dùng bản 1.0.
Nếu muốn dùng full mod menu, dùng bản 2.0.
```

---

## Cập nhật script

Khi có bản mới, mở lại link bản muốn cài:

[Aetherion Ark 1.0 - Stock Buyer](https://github.com/SoraHoshino/Aetherion-Ark/raw/refs/heads/main/aetherion-ark-1.0.user.js)

[Aetherion Ark 2.0 - Full Mod Menu](https://github.com/SoraHoshino/Aetherion-Ark/raw/refs/heads/main/aetherion-ark-2.0.user.js)

Tampermonkey sẽ hiện màn hình cập nhật.

Bấm:

```text
Reinstall / Cài lại
```

Sau đó vào lại game và nhấn:

```text
Ctrl + F5
```

---

## Lưu ý chung

```text
Script cần đọc game state để hoạt động.
Nếu Magic Garden thay đổi cấu trúc code nội bộ, một số chức năng có thể cần cập nhật lại.
Hãy kiểm tra kỹ danh sách item và số lượng mua trước khi bật Auto Mode.
Không nên cài cùng lúc quá nhiều script có chức năng giống nhau để tránh bị xung đột.
Sử dụng script theo trách nhiệm cá nhân.
```
