# Release notes — v7

- **Sản phẩm:** Portfolio CV Nguyễn Thanh Bình
- **Phiên bản bàn giao:** v7
- **Ngày cập nhật:** 09/11/2026
- **Tác giả:** Nguyễn Thanh Bình

## Thay đổi chính

- Bổ sung tài liệu dự án với hướng dẫn chạy local, mô tả cấu trúc, chức năng và cách kiểm tra các trang.
- Sửa đường dẫn CSS ở trang chủ để tải đúng `css/style.css`.
- Sửa đường dẫn ảnh đại diện để dùng `assets/avatar.svg`, tệp hiện có trong repository.
- Ghi nhật ký AI và quyết định triển khai trong `AI_LOG.md`.
- Ghi rõ URL GitHub Pages theo dự kiến hiện trả về 404; chưa xác nhận website được xuất bản.

## Lỗi đã sửa

- Trang chủ tham chiếu `style.css` ở thư mục gốc thay vì `css/style.css`.
- Trang chủ tham chiếu `assets/f.jpg`, tệp không có trong repository, nên ảnh đại diện không tải được.

## Mã nguồn liên quan

- [Repository — nhánh main](https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04/tree/main)
- [Commit nền hiện tại: `cc871c0` — Add files via upload](https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04/commit/cc871c0)

`cc871c0` là commit HEAD tại thời điểm lập ghi chú; các sửa đổi v7 trong phiên này chưa được commit. Bản mã chính xác để bàn giao là trạng thái làm việc gồm các thay đổi đang có trong repository, không phải riêng commit nền. Cập nhật liên kết commit sau khi các thay đổi được commit.

## Hạn chế còn lại và bàn giao

- GitHub Pages chưa được xác nhận hoạt động; URL đang trả 404. Bật Pages trong **Settings → Pages**, chọn nhánh `main` và thư mục gốc, chờ triển khai rồi kiểm tra URL.
- Form chỉ thực hành xác thực phía trình duyệt và chuyển dữ liệu bằng GET tới trang kết quả. Không có gửi email hoặc lưu trữ phía máy chủ; dữ liệu có thể lộ trên URL.
- Liên kết GitHub trong các thẻ dự án đang dẫn tới hồ sơ cá nhân, chưa phải mã nguồn riêng của từng dự án.
- Tiếp tục kiểm tra theo các bước trong [README.md](./README.md), đặc biệt tải CSS/ảnh, thử xác thực form với dữ liệu không hợp lệ và hợp lệ, kiểm tra trang kết quả và bố cục màn hình nhỏ.
