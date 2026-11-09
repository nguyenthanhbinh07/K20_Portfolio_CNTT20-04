# Release notes — Portfolio V8

## 1. Thông tin phiên bản

- **Tên sản phẩm theo yêu cầu bàn giao:** Portfolio CV – Nguyễn Thanh Bình
- **Phiên bản tài liệu:** V8.
- **Repository:** [nguyenthanhbinh07/K20_Portfolio_CNTT20-04](https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04).
- **Website GitHub Pages:** [nguyenthanhbinh07.github.io/K20_Portfolio_CNTT20-04](https://nguyenthanhbinh07.github.io/K20_Portfolio_CNTT20-04/).
- **Tag/commit phát hành V8:** chưa xác minh; repository hiện không có Git tag V8.

> **Cần xác nhận tên trước khi phát hành:** yêu cầu bàn giao ghi “Trần Việt Anh”, nhưng README và nội dung website hiện tại ghi “Nguyễn Thanh Bình”. Ghi chú này giữ tên theo yêu cầu, không thay đổi hay khẳng định lại danh tính trong mã nguồn.

## 2. Tổng quan phiên bản

Portfolio là website tĩnh giới thiệu cá nhân, kỹ năng, dự án học tập, quá trình học tập và thông tin liên hệ. Repository có trang portfolio và trang kết quả biểu mẫu. V8 được dùng làm nhãn cho tài liệu bàn giao; do chưa có tag hoặc commit được xác nhận là bản phát hành V8, trạng thái phát hành chính thức chưa được xác minh.

## 3. Nội dung nổi bật

- Commit `88fc5a8` trên `origin/main` có thay đổi `index.html`, `css/style.css` và bốn tệp SVG trong `assets/`.
- Changelog hiện chưa xác định được các thay đổi đó tương ứng với V8 hay có tag phát hành nào; vì vậy không gán thêm tính năng hoặc nâng cấp cụ thể cho V8.

## 4. Cách truy cập

1. Mở [website GitHub Pages](https://nguyenthanhbinh07.github.io/K20_Portfolio_CNTT20-04/). Trạng thái truy cập chưa được xác minh ổn định; nếu không mở được, dùng bản local.
2. Clone repository:

   ```powershell
   git clone https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04.git
   cd K20_Portfolio_CNTT20-04
   ```

3. Mở `index.html` bằng Live Server trong VS Code, hoặc chạy `py -m http.server 8000` ở thư mục dự án rồi truy cập `http://localhost:8000/`.

## 5. Tài liệu bàn giao

- [README.md](./README.md) — hướng dẫn sử dụng, chạy và kiểm tra.
- [CHANGELOG.md](./CHANGELOG.md) — lịch sử thay đổi và những điểm chưa xác minh phiên bản.
- [docs/AI_LOG.md](./docs/AI_LOG.md) — nhật ký sử dụng AI.
- [docs/evidence-index.md](./docs/evidence-index.md) — danh mục minh chứng và kết quả kiểm thử.

## 6. Giới hạn đã biết

- Biểu mẫu chỉ xác thực phía trình duyệt và chuyển dữ liệu bằng GET tới `ket-qua.html`; không gửi email, không lưu dữ liệu trên máy chủ, và dữ liệu có thể xuất hiện trên URL.
- GitHub Pages chưa được xác nhận hoạt động ổn định. Các lần kiểm tra được ghi nhận khác nhau; cần kiểm tra lại trong cửa sổ ẩn danh.
- Thư mục minh chứng hiện chưa có ảnh kiểm thử.
- Chưa có Git tag V7, V8 hoặc V8.1; ngày phát hành và commit phát hành V8 chưa được xác minh.
- Tên sản phẩm yêu cầu khác tên hiện có trong README và website; cần xác nhận trước khi phát hành công khai.
