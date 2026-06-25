# Hướng dẫn sử dụng — ĐI CÙNG TAKICO

Game kiosk offline · Honda HEAD Tân Kiều · Howls Studio

**Trang tải & demo:** [https://pnctriet.github.io/takico/](https://pnctriet.github.io/takico/)

---

## Lưu ý chung

Sau khi tải, giải nén và **copy nguyên thư mục** (USB, Desktop, máy booth). Không cần cài Python, Node hay Internet khi chơi. Cần webcam + Chrome/Edge (macOS: thêm Safari).

| Nền tảng | Link tải |
|----------|----------|
| Windows | [Tải bản Windows](https://drive.google.com/uc?export=download&id=1r_ZOj8mbE80N7qAM9cg-Xv3frU9yH9Jd) |
| macOS | [Tải bản macOS](https://drive.google.com/uc?export=download&id=1EJq0eqr13ymJ8i-cgnW4dbWKafdF-vQj) |

---

## Windows

### Nội dung gói

| File / thư mục | Mô tả |
|----------------|--------|
| `Play Takico.bat` | Double-click để chơi |
| `Stop Takico.bat` | Thoát game |
| `_game` | Dữ liệu game — không xóa/đổi tên (có thể bị ẩn) |
| `GUIDE.md` | Hướng dẫn chi tiết |

### Bắt đầu

1. Double-click `Play Takico.bat`
2. SmartScreen cảnh báo → **More info** → **Run anyway**
3. Cho phép **Camera** trong Chrome/Edge
4. Chạm màn hình chờ hoặc nhấn **SPACE** để bắt đầu

### Thoát / chơi lại

| Thao tác | Cách làm |
|----------|----------|
| Thoát | Chạy `Stop Takico.bat` hoặc đóng cửa sổ Takico Server |
| Chơi lại | Chạy lại `Play Takico.bat` |

### Yêu cầu

- Windows 10/11 (64-bit), Chrome hoặc Edge, webcam
- Không cần Internet sau khi copy gói

### Booth / kiosk

- Camera cách người chơi **1,5–2,5 m**
- Tắt chế độ ngủ màn hình trong sự kiện

### Xử lý lỗi

| Lỗi | Cách xử lý |
|-----|------------|
| `.bat` không chạy | Chạy quyền admin; kiểm tra antivirus |
| Missing `_game` | Copy lại **nguyên thư mục windows** |
| Lỗi camera | Chrome → biểu tượng khóa → Camera → Allow |
| Port 8765 bận | Chạy `Stop Takico.bat` rồi mở lại |

---

## macOS

### Nội dung gói

| File | Mô tả |
|------|--------|
| `Play Takico.app` | Double-click để chơi |
| `GUIDE.md` | Hướng dẫn chi tiết |
| `VERSION.txt` | Thông tin bản build |

Toàn bộ dữ liệu game nằm **trong** `Play Takico.app` — không mở/sửa file bên trong.

### Bắt đầu

1. Double-click `Play Takico.app`
2. Lần đầu (Gatekeeper): Right-click → **Open** → **Open**
3. Hoặc Terminal: `xattr -cr /đường/dẫn/tới/macos` rồi mở lại
4. Cho phép **Camera** khi trình duyệt hỏi
5. Chạm màn hình chờ hoặc nhấn **SPACE**

### Thoát / chơi lại

| Thao tác | Cách làm |
|----------|----------|
| Thoát | **Cmd+Q** hoặc menu Play Takico → Quit |
| Chơi lại | Double-click `Play Takico.app` |

### Yêu cầu

- macOS 11+, Chrome / Edge / Safari, webcam
- Không cần Internet sau khi copy gói

### Booth / kiosk

- Camera cách người chơi **1,5–2,5 m**, tránh ngược sáng
- Một người trong khung hình; tắt ngủ màn hình

### Xử lý lỗi

| Lỗi | Cách xử lý |
|-----|------------|
| App không mở | Right-click → Open; hoặc `xattr -cr` trên thư mục macos |
| "App is damaged" | Chạy `xattr -cr`; chỉ mở qua `Play Takico.app` |
| Lỗi camera | Chrome → biểu tượng khóa → Camera → Allow |

---

Howls Studio · Honda HEAD Tân Kiều · ĐI CÙNG TAKICO
