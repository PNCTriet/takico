# ĐI CÙNG TAKICO

Game kiosk offline cho sự kiện **Honda HEAD Tân Kiều**, phát triển bởi **Howls Studio**.

Trang landing tải game và hướng dẫn cài đặt cho booth / kiosk — chạy hoàn toàn offline sau khi copy gói, không cần Python, Node hay Internet khi chơi.

## Demo

**Trang tải game (live):** [https://pnctriet.github.io/takico/](https://pnctriet.github.io/takico/)

Mở link trên để xem giao diện tải bản Windows / macOS và hướng dẫn sử dụng.

## Tải game

| Nền tảng | Yêu cầu | Dung lượng | Link tải |
|----------|---------|------------|----------|
| **Windows** | Windows 10/11 (64-bit) | ~74 MB | [Tải bản Windows](https://drive.google.com/uc?export=download&id=1r_ZOj8mbE80N7qAM9cg-Xv3frU9yH9Jd) |
| **macOS** | macOS 11+ | ~74 MB | [Tải bản macOS](https://drive.google.com/uc?export=download&id=1EJq0eqr13ymJ8i-cgnW4dbWKafdF-vQj) |

Mỗi bản gồm **3 chặng / game**. Sau khi tải, giải nén và **copy nguyên thư mục** (USB, Desktop, máy booth). Cần **webcam** và trình duyệt **Chrome** hoặc **Edge** (macOS còn hỗ trợ Safari).

## Cách chơi nhanh

### Windows

1. Double-click `Play Takico.bat`
2. SmartScreen cảnh báo → **More info** → **Run anyway**
3. Cho phép **Camera** trong Chrome/Edge
4. Chạm màn hình chờ hoặc nhấn **SPACE** để bắt đầu

Thoát: chạy `Stop Takico.bat` hoặc đóng cửa sổ Takico Server.

### macOS

1. Double-click `Play Takico.app`
2. Lần đầu (Gatekeeper): Right-click → **Open** → **Open**
3. Cho phép **Camera** khi trình duyệt hỏi
4. Chạm màn hình chờ hoặc nhấn **SPACE**

Thoát: **Cmd+Q** hoặc menu Play Takico → Quit.

Chi tiết đầy đủ, xử lý lỗi và cấu hình booth: xem [GUIDE.md](./GUIDE.md).

## Cấu trúc repo

```
.
├── index.html    # Trang landing tải game (GitHub Pages)
├── README.md     # Giới thiệu dự án (file này)
└── GUIDE.md      # Hướng dẫn chi tiết Windows & macOS
```

## Yêu cầu booth / kiosk

- Camera cách người chơi **1,5–2,5 m**, tránh ngược sáng (macOS)
- Một người trong khung hình
- Tắt chế độ ngủ màn hình trong sự kiện
- Không cần Internet sau khi copy gói

## Phát triển & deploy trang landing

Trang demo chạy qua **GitHub Pages** từ nhánh `main`, file `index.html` ở thư mục gốc.

Để đổi link tải, sửa biến `DOWNLOAD_WINDOWS` và `DOWNLOAD_MACOS` trong `index.html` (hoặc thuộc tính `href` của nút tải). Google Drive: Share → Anyone with link → dùng dạng:

```
https://drive.google.com/uc?export=download&id=FILE_ID
```

Chạy local để xem trước:

```bash
# Python
python3 -m http.server 8080
# Mở http://localhost:8080
```

## Liên hệ & bản quyền

**Howls Studio** · **Honda HEAD Tân Kiều** · ĐI CÙNG TAKICO
