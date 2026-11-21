# T4 e-reader OS

## Tải T4 e-reader OS

[**Tải bản cài mới nhất**](https://github.com/hoangtuan2k5/t4-e-reader-os-releases/releases/latest/download/t4-e-reader-os-offline.zip) · [Xem các bản phát hành](https://github.com/hoangtuan2k5/t4-e-reader-os-releases/releases/latest)

Giải nén vào thư mục `koreader/plugins/`, rồi mở T4 từ menu KOReader.

Bản cài T4 e-reader OS cho KOReader trên Kindle Paperwhite 1.

## Chơi cờ trực tuyến

[![Chơi cờ trên web](https://img.shields.io/badge/CH%C6%A0I%20C%E1%BB%9C%20TR%C3%8AN%20WEB-chess.hoangtuan.dev-9a571f?style=for-the-badge)](https://chess.hoangtuan.dev)

**[Mở sảnh cờ T4](https://chess.hoangtuan.dev)** để tìm trận, mời bạn bằng mã phòng hoặc xem ván đang diễn ra. Sau ván, dùng **Phân tích Stockfish** để xem lại nước đi và thử các biến. Bản web đang trong giai đoạn thử nghiệm.

> **Trên Kindle, dùng T4 v1.4.0 trở lên.** Kết nối Wi-Fi, vào **Cài đặt → Cập nhật T4** rồi khởi động lại KOReader. Nếu cài lần đầu, tải gói cài ở đầu trang.

1. Mở **Cờ vua → Chơi trực tuyến** và đăng nhập bằng tài khoản web hoặc tạo tài khoản trên Kindle.
2. Chọn **Tìm trận** để ghép trong khoảng **±500 Elo**, **Vào theo ID** để nhập mã phòng, hoặc **Bạn bè** để tìm bằng `@username` hay ID người chơi rồi rủ đấu.
3. Sau ván, chọn **Phân tích** để xem lại các nước và biến Stockfish.

T4 hỗ trợ chơi trực tuyến khi có Wi-Fi và luyện cờ trên thiết bị.

<a href="screenshots/chess-online-lobby.png"><img src="screenshots/chess-online-lobby.png" width="224" alt="Sảnh Chơi trực tuyến trên Kindle Paperwhite 1"></a>

## Cài trên Kindle

1. Thoát KOReader rồi kết nối Kindle với máy tính bằng USB.
2. Giải nén ZIP đã chọn vào `koreader/plugins/`. Kiểm tra đường dẫn `koreader/plugins/t4-e-reader-os.koplugin/main.lua`.
3. Nếu nâng cấp qua USB, sao lưu thư mục plugin cũ ra ngoài `plugins/` trước khi thay. Giữ dữ liệu trong `koreader/settings/learningos/`.
4. Mở KOReader và chọn **T4 e-reader OS** từ menu.

Sau khi cài bản hỗ trợ OTA, kết nối Wi-Fi và vào **Cài đặt → Cập nhật T4**. T4 chọn gói cập nhật và yêu cầu khởi động lại KOReader sau khi cài.


## Kho puzzle

Mở **Cờ vua → Kho puzzle → Tải thêm qua Wi-Fi** để tải gói. T4 có 5.000 bài đi kèm và có thể luyện nhiều gói đã cài cùng lúc. [Tải gói puzzle theo Elo hoặc Binpack đầy đủ](https://github.com/hoangtuan2k5/t4-e-reader-os-releases/releases/tag/puzzle-packs-v1)

## Xem lại và phân tích ván cờ

Sau khi đánh máy, bấm **Xem lại ván** hoặc mở ván đã kết thúc trong **Cờ vua → Lịch sử**. Bấm **Phân tích** để chạy Stockfish trên thiết bị. Có thể dừng và tiếp tục phần phân tích đang dở. Khi xong, **Kết quả phân tích** hiển thị độ chính xác cả ván của Trắng và Đen, tính từ các nước được Stockfish chấm điểm. Bấm **Xem danh sách nước đi**, rồi chạm vào số ở cột **Trắng** hoặc **Đen** để nhảy tới nước đầu tiên của bên đó mang nhãn tương ứng. Trong màn xem lại, có thể chọn từng nước trong danh sách hoặc phát tuần tự. Kết quả từng nước được lưu trên Kindle.

T4 dùng 10 nhãn gồm **Tốt nhất**, **Xuất sắc**, **Khá**, **Thiếu chính xác**, **Sai lầm**, **Sai lầm nghiêm trọng**, **Bỏ lỡ**, **Then chốt**, **Thiên tài** và **Nước sách**. T4 dùng quy tắc riêng và chạy thêm một lượt tìm kiếm sâu cho ba nhãn chiến thuật. Bảng khai cuộc SQLite được tạo từ [bộ dữ liệu Lichess CC0](https://github.com/lichess-org/chess-openings).

Trong bàn cờ xem lại, chạm quân để xem hướng tấn công, nét đứt bảo vệ và ô kiểm soát. Ô trống được hai bên kiểm soát hiện hai kiếm chéo. Nút **Xem chỉ dẫn** cũng có trong màn Puzzle và Đánh máy. Khi bật, chạm bàn cờ để phân tích thay vì đi quân. Đồng hồ ván đấu và thời gian giải puzzle vẫn chạy.

Ảnh dưới đây được render từ plugin ở độ phân giải 758 × 1024. Bấm từng ảnh để mở kích thước gốc.

| Mở ván đã kết thúc và bấm Phân tích | So sánh độ chính xác cả ván | Lọc nhãn theo Trắng hoặc Đen |
| --- | --- | --- |
| <a href="screenshots/chess-review-start.png"><img src="screenshots/chess-review-start.png" width="224" alt="Mở ván đã kết thúc và bấm Phân tích"></a> | <a href="screenshots/chess-review-results.png"><img src="screenshots/chess-review-results.png" width="224" alt="So sánh độ chính xác cả ván"></a> | <a href="screenshots/chess-review-labels.png"><img src="screenshots/chess-review-labels.png" width="224" alt="Lọc nhãn theo Trắng hoặc Đen"></a> |

| Xem lại, nhảy tới nước đi hoặc phát tuần tự | Hướng dẫn đọc mũi tên và ô kiểm soát | Ván Opera với chỉ dẫn cho năm quân |
| --- | --- | --- |
| <a href="screenshots/chess-review-replay.png"><img src="screenshots/chess-review-replay.png" width="224" alt="Xem lại, nhảy tới nước đi hoặc phát tuần tự"></a> | <a href="screenshots/chess-review-legend.png"><img src="screenshots/chess-review-legend.png" width="224" alt="Hướng dẫn đọc mũi tên và ô kiểm soát"></a> | <a href="screenshots/chess-review-opera.png"><img src="screenshots/chess-review-opera.png" width="224" alt="Ván Opera với chỉ dẫn cho năm quân"></a> |

### So sánh nước đi từ v1.3.0

Mở **So sánh** ngay tại nước đang xem để đối chiếu nước đã đi với lựa chọn của Stockfish. Khi có biến phản đòn, chọn **Đối thủ tận dụng** để xem cách đáp trả. Chạm vào quân cờ để xem các hướng tấn công và bảo vệ liên quan.

<p>
<a href="screenshots/chess-compare-played.png"><img src="screenshots/chess-compare-played.png" width="224" alt="Nước đã đi"></a>
<a href="screenshots/chess-compare-best.png"><img src="screenshots/chess-compare-best.png" width="224" alt="Nước tốt nhất"></a>
<a href="screenshots/chess-compare-reply.png"><img src="screenshots/chess-compare-reply.png" width="224" alt="Đối thủ tận dụng"></a>
</p>

## Giao diện trên Kindle Paperwhite 1

| Trang chủ Online | Trang chủ Offline | Bản tin sáng |
| --- | --- | --- |
| <a href="screenshots/home-online.png"><img src="screenshots/home-online.png" width="224" alt="Trang chủ Online"></a> | <a href="screenshots/home-offline.png"><img src="screenshots/home-offline.png" width="224" alt="Trang chủ Offline"></a> | <a href="screenshots/briefing.png"><img src="screenshots/briefing.png" width="224" alt="Bản tin sáng"></a> |

| Thư viện | Ghi chú sách | Highlight |
| --- | --- | --- |
| <a href="screenshots/reader-library.png"><img src="screenshots/reader-library.png" width="224" alt="Thư viện"></a> | <a href="screenshots/reader-notes.png"><img src="screenshots/reader-notes.png" width="224" alt="Ghi chú sách"></a> | <a href="screenshots/reader-highlights.png"><img src="screenshots/reader-highlights.png" width="224" alt="Highlight"></a> |

| Kho tri thức | Tổng quan học tập | Lộ trình bộ thẻ |
| --- | --- | --- |
| <a href="screenshots/reader-vault.png"><img src="screenshots/reader-vault.png" width="224" alt="Kho tri thức"></a> | <a href="screenshots/study.png"><img src="screenshots/study.png" width="224" alt="Tổng quan học tập"></a> | <a href="screenshots/study-roadmap.png"><img src="screenshots/study-roadmap.png" width="224" alt="Lộ trình bộ thẻ"></a> |

| Ôn từ bằng flashcard | Trắc nghiệm | Việc cần làm |
| --- | --- | --- |
| <a href="screenshots/flashcard.png"><img src="screenshots/flashcard.png" width="224" alt="Ôn từ bằng flashcard"></a> | <a href="screenshots/quiz.png"><img src="screenshots/quiz.png" width="224" alt="Trắc nghiệm"></a> | <a href="screenshots/todo.png"><img src="screenshots/todo.png" width="224" alt="Việc cần làm"></a> |

| Tổng quan cờ vua | Giải puzzle | Đánh với máy |
| --- | --- | --- |
| <a href="screenshots/chess.png"><img src="screenshots/chess.png" width="224" alt="Tổng quan cờ vua"></a> | <a href="screenshots/puzzle.png"><img src="screenshots/puzzle.png" width="224" alt="Giải puzzle"></a> | <a href="screenshots/chess-play.png"><img src="screenshots/chess-play.png" width="224" alt="Đánh với máy"></a> |

| Bàn cờ khi bật Xem chỉ dẫn | Ôn puzzle theo SRS | Lịch sử ván đấu |
| --- | --- | --- |
| <a href="screenshots/chess-hints.png"><img src="screenshots/chess-hints.png" width="224" alt="Bàn cờ khi bật Xem chỉ dẫn"></a> | <a href="screenshots/chess-srs.png"><img src="screenshots/chess-srs.png" width="224" alt="Ôn puzzle theo SRS"></a> | <a href="screenshots/chess-history.png"><img src="screenshots/chess-history.png" width="224" alt="Lịch sử ván đấu"></a> |

| Phiên và tin nhắn Agent | Các yêu cầu chờ duyệt | Cài đặt T4 |
| --- | --- | --- |
| <a href="screenshots/agent.png"><img src="screenshots/agent.png" width="224" alt="Phiên và tin nhắn Agent"></a> | <a href="screenshots/agent-approvals.png"><img src="screenshots/agent-approvals.png" width="224" alt="Các yêu cầu chờ duyệt"></a> | <a href="screenshots/settings.png"><img src="screenshots/settings.png" width="224" alt="Cài đặt T4"></a> |


### Lịch sử puzzle trong v1.3.0

Ảnh xem trước của **Cờ vua → Lịch sử → Puzzle**. Chạm một lượt giải để mở lại bài.

<a href="screenshots/puzzle-history.png"><img src="screenshots/puzzle-history.png" width="280" alt="Lịch sử puzzle trên Kindle"></a>
