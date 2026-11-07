# Hình nền Sunset Park cho Claude (Hòa ♥ Thảo)

Cặp đôi ngồi ghế công viên ngắm hoàng hôn, dòng chữ **Hòa ♥ Thảo**, cho app **Claude Desktop**. Bản sửa từ [aqua2409z/pixel-chat-themes](https://github.com/aqua2409z/pixel-chat-themes) (MIT).

Repo gồm:

| File | Dùng để |
|---|---|
| `claude-pixel-themes.user.js` | Hình nền **toàn màn hình** (chạy trong DevTools của app) |
| `pixel-themes/` | Plugin lệnh `/nen` cho tab Code: khung cảnh bên cạnh, viền màu tin nhắn |

## Cài trên máy mới

Cần: app Claude Desktop, [Git for Windows](https://git-scm.com/download/win), và đăng nhập GitHub tài khoản có quyền xem repo này.

### 1. Plugin `/nen`

Mở terminal (PowerShell) và chạy:

```
claude plugin install pixel-themes --marketplace tranhoa2602/pixel-nen
```

Lần đầu Git sẽ mở trình duyệt để đăng nhập GitHub. Cài xong, mở một phiên Code mới và gõ `/nen sunset`.

Hoặc trong app: tab **Code** → **+** cạnh ô chat → **Plugins** → **Add marketplace** → nhập `tranhoa2602/pixel-nen` → chọn **pixel-themes** → **Add plugin**.

### 2. Hình nền toàn màn hình (làm 1 lần)

1. Trong app Claude: menu **☰** → **Help** → **Troubleshooting** → **Enable Developer Mode**. Thoát hẳn app rồi mở lại.
2. Trên GitHub, mở file `claude-pixel-themes.user.js` của repo này → bấm nút **Copy raw file** (biểu tượng hai ô vuông chồng nhau).
3. Bấm vào cửa sổ app Claude, nhấn `Ctrl + Alt + I` để mở DevTools.
4. Tab **Sources** → cột trái bấm `»` cạnh **Page** → **Snippets** → **+ New snippet** → đặt tên `pixel` → Enter.
5. Bấm vào khung bên phải, `Ctrl + V`, rồi `Ctrl + S`. Nhấn `Ctrl + Enter` để chạy thử.
6. Nhấn `Alt + T` và chọn **Sunset Park**.

Nếu DevTools chặn dán: tắt bộ gõ tiếng Việt, gõ tay `allow pasting` vào tab **Console**, Enter, rồi dán lại.

### Mỗi lần mở lại app

`Ctrl + Alt + I` → `Ctrl + P` → gõ `!pixel` → Enter → đóng DevTools.

## Cập nhật khi repo có bản mới

```
claude plugin marketplace update pixel-nen-local
claude plugin update pixel-themes@pixel-nen-local
```

Hình nền: chép lại file `claude-pixel-themes.user.js` vào Snippet `pixel`, `Ctrl + S`, thoát hẳn app rồi mở lại.
