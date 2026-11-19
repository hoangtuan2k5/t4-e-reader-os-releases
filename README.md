# T4 e-reader OS

Bản cài T4 e-reader OS cho KOReader trên Kindle Paperwhite 1.

## Tải bản mới nhất

- [Tải bản Online](https://github.com/hoangtuan2k5/t4-e-reader-os-releases/releases/latest/download/t4-e-reader-os-online.zip) — đọc, học, cờ vua và kết nối Agent/Vault.
- [Tải bản Offline](https://github.com/hoangtuan2k5/t4-e-reader-os-releases/releases/latest/download/t4-e-reader-os-offline.zip) — đọc, học và cờ vua trên Kindle.
- [Xem ghi chú bản mới nhất](https://github.com/hoangtuan2k5/t4-e-reader-os-releases/releases/latest)

Các liên kết trên tự trỏ đến bản ổn định mới nhất khi kho phát hành có bản công khai.

## Cài trên Kindle

1. Thoát KOReader rồi kết nối Kindle với máy tính bằng USB.
2. Giải nén ZIP đã chọn vào `koreader/plugins/`. Kiểm tra đường dẫn `koreader/plugins/t4-e-reader-os.koplugin/main.lua`.
3. Nếu nâng cấp qua USB, sao lưu thư mục plugin cũ ra ngoài `plugins/` trước khi thay. Giữ dữ liệu trong `koreader/settings/learningos/`. Nếu dùng Agent, sao chép lại `secrets.lua` của bản Online.
4. Mở KOReader và chọn **T4 e-reader OS** từ menu.

Sau khi cài bản hỗ trợ OTA, kết nối Wi-Fi và vào **Cài đặt → Cập nhật T4**. Cả hai bản tự chọn đúng gói cập nhật và yêu cầu khởi động lại KOReader sau khi cài.
