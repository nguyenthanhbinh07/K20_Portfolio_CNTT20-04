# CHANGELOG

Lịch sử dưới đây dựa trên nội dung repository, commit và trạng thái làm việc hiện tại. Các tiêu đề V8.1 và V8 được giữ theo yêu cầu, nhưng Git chưa có tag xác nhận việc phát hành hoặc gán phiên bản cho các thay đổi này.

## [V8.1] – Chưa xác minh

### Added

- Thêm `CHANGELOG.md`.
- Thêm `docs/evidence-index.md` và thư mục `docs/evidence/`; thư mục hiện chỉ có `.gitkeep`, chưa có ảnh hoặc tệp minh chứng.

### Changed

- Cập nhật `README.md` với nội dung Portfolio V8, hướng dẫn chạy, cấu trúc repository và ghi chú kiểm thử.
- Chuyển nhật ký AI từ `AI_LOG.md` ở thư mục gốc sang `docs/AI_LOG.md`.
- Cập nhật `RELEASE_NOTES.md` để tham chiếu vị trí tài liệu mới.

### Fixed

- Chưa ghi nhận sửa lỗi mã nguồn thuộc nhóm thay đổi này.

### Notes

- Các thay đổi tài liệu trên hiện có trong working tree nhưng chưa được commit trên nhánh `main`; chưa có căn cứ xác nhận đây là nội dung phát hành V8.1.
- Chưa có ảnh minh chứng trong `docs/evidence/`.

### Chưa kiểm tra

- Chưa xác minh V8.1 là phiên bản đã phát hành hay ngày phát hành.
- Chưa xác minh các thay đổi tài liệu ở trên được gán cho V8 hay V8.1.

## [V8] – Ngày commit: 2026-11-09; ngày phát hành chưa xác minh

### Added

- Không thấy tệp mới trong commit `88fc5a8` so với commit cha `cc871c0`.

### Changed

- Commit `88fc5a8` thay đổi `index.html`, `css/style.css` và nội dung bốn tệp SVG trong `assets/`.

### Fixed

- Không ghi nhận mục sửa lỗi riêng biệt trong thông tin commit; tiêu đề commit không mô tả lỗi cụ thể.

### Notes

- `88fc5a8` có ngày commit 2026-11-09 và hiện là commit trên `origin/main`; commit không ghi tên phiên bản.
- Nhánh `main` tại `bbc71d7` và `origin/main` tại `88fc5a8` cùng xuất phát từ `cc871c0`, không phải quan hệ kế tiếp nhau. Vì vậy không thể dùng thứ tự hai commit này để khẳng định V8 rồi V8.1.

### Chưa kiểm tra

- Chưa xác minh commit `88fc5a8` có phải bản phát hành V8 hoặc ngày commit có phải ngày phát hành.
- Chưa xác minh mục đích nội dung cụ thể của các thay đổi HTML, CSS và SVG ngoài việc các tệp này được sửa trong commit.

## [V7] – Ngày ghi nhận: 2026-11-09; ngày phát hành chưa xác minh

### Added

- Thêm hướng dẫn dự án và `RELEASE_NOTES.md` theo nội dung commit `bbc71d7`.
- Bổ sung nội dung `AI_LOG.md` và thông tin sử dụng/chạy thử được ghi trong tài liệu.

### Changed

- Cập nhật `README.md` với hướng dẫn chạy, cấu trúc, chức năng và các giới hạn đã ghi nhận.
- Cập nhật tham chiếu tài nguyên trong `index.html`.

### Fixed

- Sửa tham chiếu CSS của trang chủ sang `css/style.css`.
- Sửa ảnh đại diện sang `assets/avatar.svg`, thay cho đường dẫn ảnh không có trong repository.

### Notes

- `RELEASE_NOTES.md` ghi phiên bản bàn giao v7 và ngày cập nhật 09/11/2026; commit `bbc71d7` có ngày 2026-11-09.
- Chưa có Git tag xác nhận v7 hoặc ngày phát hành.

### Chưa kiểm tra

- Chưa xác minh v7 đã được phát hành chính thức.
- Chưa có tag v7, v8 hoặc v8.1 trong danh sách Git tag tại thời điểm lập changelog.
