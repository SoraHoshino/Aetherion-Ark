# Aetherion Ark

Userscript cho **Magic Garden** giúp theo dõi shop và tự động mua các item đã chọn khi shop còn hàng.

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

## Cài đặt cho người mới

### Bước 1: Cài Tampermonkey

1. Mở Google.
2. Search:

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

Sau khi cài xong, trên góc phải trình duyệt sẽ có biểu tượng tiện ích hình mảnh ghép.

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

8. Bật mục:

```text
Cho phép tập lệnh của người dùng / Allow User Scripts
```

9. Ở mục quyền truy cập trang web, chọn:

```text
Trên tất cả trang web / On all sites
```

Hoặc cho phép riêng các trang Magic Garden nếu không muốn bật cho tất cả.

---

### Bước 3: Cài script Aetherion Ark

Mở link cài đặt:

```text
https://raw.githubusercontent.com/SoraHoshino/Aetherion-Ark/refs/heads/main/aetherion-ark-1.0.user.js
```

Tampermonkey sẽ tự mở trang cài đặt.

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

3. Chờ bảng **Aetherion Ark** hiện lên trong game.

---

## Chức năng chính

Aetherion Ark hỗ trợ:

```text
Tự động quét shop
Tự động mua item đã chọn khi còn hàng
Thêm / xóa item khỏi danh sách mua
Mua nhanh một lần
Bật / tắt Auto Mode
Chọn thời gian quét shop
Chọn số lượng mua tối đa
Xem log mua hàng
Xem thống kê số item đã mua và coin đã dùng
```

Script hỗ trợ các nhóm item:

```text
Seed
Egg
Tool
Decor
```

Có hỗ trợ thêm một số item shop event như:

```text
Dawn shop
Snow / Winter shop
```

Ví dụ:

```text
Dawn Egg
Snow Egg
Winter Egg
Frozen Potion
Chilled Potion
Ube
Dawnbreaker
Snowdrop
Poinsettia
```

---

## Cách dùng

1. Vào game và chờ panel **Aetherion Ark** hiện lên.
2. Chọn item muốn mua trong danh sách.
3. Bấm nút `+` để thêm item.
4. Bấm **Mua nhanh** nếu muốn quét shop ngay một lần.
5. Bật **Auto: ON** nếu muốn script tự quét theo chu kỳ.

---

## Tùy chọn

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
=> Script chỉ mua tối đa 3 item
```

---

## Các nút trên panel

```text
Auto: ON/OFF
Bật hoặc tắt tự động quét shop.

Mua nhanh
Quét shop và mua ngay một lần.

Nút giỏ hàng
Mua riêng item đó một lần.

Nút xóa
Xóa item khỏi danh sách.

Nút thùng rác
Reset thống kê mua hàng.
```

---

## Log thường gặp

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

## Cập nhật script

Khi có bản mới, mở lại link:

```text
https://raw.githubusercontent.com/SoraHoshino/Aetherion-Ark/refs/heads/main/aetherion-ark-1.0.user.js
```

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

## Lưu ý

Script cần đọc game state để biết shop còn hàng hay không.

Nếu Magic Garden thay đổi cấu trúc code nội bộ, một số chức năng có thể cần cập nhật lại.

Hãy kiểm tra danh sách item và số lượng mua trước khi bật Auto Mode.

Sử dụng script theo trách nhiệm cá nhân.
