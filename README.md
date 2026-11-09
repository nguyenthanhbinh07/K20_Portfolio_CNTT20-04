# Nguyễn Thanh Bình — Portfolio CV

Portfolio CV tĩnh giới thiệu thông tin, kỹ năng, dự án học tập và form liên hệ của Nguyễn Thanh Bình (Công nghệ Thông tin 20-04).

## Liên kết

- **Mã nguồn:** [nguyenthanhbinh07/K20_Portfolio_CNTT20-04](https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04)
- **Hồ sơ tác giả:** [github.com/nguyenthanhbinh07](https://github.com/nguyenthanhbinh07)
- **GitHub Pages:** [nguyenthanhbinh07.github.io/K20_Portfolio_CNTT20-04](https://nguyenthanhbinh07.github.io/K20_Portfolio_CNTT20-04/)

> **Tình trạng xuất bản:** URL Pages ở trên là địa chỉ dự kiến theo tên tài khoản và repository. Khi kiểm tra ngày 09/11/2026, URL trả về 404; vì vậy bản web hiện chưa được xác nhận là đã xuất bản. Để xuất bản, vào **Settings → Pages**, chọn triển khai từ nhánh `main` và thư mục gốc (`/root`), rồi kiểm tra lại URL sau khi GitHub hoàn tất triển khai.

## Sản phẩm

Website HTML/CSS tĩnh, không cần cơ sở dữ liệu hay backend. Trang chủ có các mục Giới thiệu, Kỹ năng, Dự án, Học tập và Liên hệ; trang kết quả cho biết form đã được trình duyệt kiểm tra và gửi theo phương thức GET. Giao diện có bố cục responsive cho màn hình nhỏ.

Form chỉ dùng để thực hành: không gửi email, không lưu dữ liệu lên máy chủ. Các trường nhập được đưa vào URL bởi phương thức GET, vì vậy không nhập thông tin nhạy cảm.

## Cấu trúc thư mục

```text
.
├── index.html          # Portfolio và form liên hệ
├── ket-qua.html        # Trang kết quả sau khi gửi form
├── README.md           # Hướng dẫn dự án
├── AI_LOG.md           # Nhật ký sử dụng AI và quyết định
├── RELEASE_NOTES.md    # Ghi chú bàn giao v7
├── css/
│   └── style.css       # Giao diện, responsive và trạng thái tương tác
└── assets/
    ├── avatar.svg      # Ảnh đại diện minh họa
    ├── du-an-1.svg     # Minh họa dự án C++
    ├── du-an-2.svg     # Minh họa portfolio
    └── du-an-3.svg     # Minh họa website thực hành
```

## Chạy trên máy

1. Tải hoặc clone repository:

   ```powershell
   git clone https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04.git
   cd K20_Portfolio_CNTT20-04
   ```

2. Dùng Python 3 để chạy máy chủ tĩnh tại thư mục gốc:

   ```powershell
   py -m http.server 8000
   ```

3. Mở `http://localhost:8000/` trong trình duyệt. Dừng máy chủ bằng `Ctrl+C`.

Có thể mở `index.html` trực tiếp, nhưng chạy máy chủ cục bộ giúp kiểm tra các đường dẫn tương đối như khi xuất bản.

## Cách kiểm tra trang và chức năng

1. Trên trang chủ, kiểm tra menu cuộn tới từng mục; xác nhận CSS được tải và ảnh đại diện cùng ba ảnh minh họa dự án hiển thị.
2. Cuộn tới **Học tập** để xem bảng học phần.
3. Tại **Liên hệ**, thử gửi form để kiểm tra xác thực HTML5:
   - Họ tên bắt buộc, ít nhất 2 ký tự.
   - Email bắt buộc và phải đúng định dạng email.
   - Lời nhắn bắt buộc, từ 10 đến 500 ký tự.
4. Nhập dữ liệu hợp lệ và gửi: trình duyệt chuyển tới `ket-qua.html`; trang này giải thích rằng không có email được gửi và dữ liệu không được lưu trên máy chủ. Với GET, dữ liệu có thể xuất hiện trên thanh địa chỉ.
5. Dùng **Quay lại liên hệ** hoặc menu trên trang kết quả để trở về trang chủ.
6. Thu nhỏ cửa sổ trình duyệt để kiểm tra bố cục responsive.

## Hồ sơ và minh chứng

- [Trang chủ và nội dung portfolio](https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04/blob/main/index.html)
- [Trang kết quả form](https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04/blob/main/ket-qua.html)
- [CSS giao diện](https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04/blob/main/css/style.css)
- [Tài nguyên ảnh](https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04/tree/main/assets)
- [Nhật ký AI](./AI_LOG.md) · [Ghi chú bàn giao v7](./RELEASE_NOTES.md)

Các liên kết GitHub trên là minh chứng mã nguồn; URL Pages hiện chưa hoạt động theo lần kiểm tra nêu trên. Các liên kết GitHub dưới thẻ dự án trong trang chủ hiện trỏ tới hồ sơ cá nhân, không phải repository riêng của từng dự án.
