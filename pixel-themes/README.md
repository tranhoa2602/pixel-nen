# pixel-themes (bản `/nen`)

Plugin cho **tab Code của app Claude Desktop**. Đây là bản sửa từ [aqua2409z/pixel-chat-themes](https://github.com/aqua2409z/pixel-chat-themes): đổi lệnh thành `/nen`, thêm theme **Sunset Park** (Hòa ♥ Thảo) và bỏ dải cảnh trên ô chat.

| Lệnh | Kết quả |
|---|---|
| `/nen` | Mở bảng chọn theme |
| `/nen sunset`, `/nen hoang hon`, `/nen koi`… | Đổi theme |
| `/nen side` | Mở khung cảnh bên cạnh |
| `/nen tint` | Bật/tắt viền màu quanh tin nhắn |
| `/nen off` | Tắt |

```
hooks/register.tsx   lệnh /nen, bảng chọn, khung bên cạnh, tô màu tin nhắn
hooks/scenes.ts      10 cảnh pixel dạng SVG tự chuyển động
tests/pixel.test.tsx kiểm thử
```

Kiểm tra: `claude plugin validate .` và `claude plugin test .`

Giấy phép [MIT](../LICENSE), giữ nguyên ghi công tác giả gốc aqua2409z.
