# Portfolio V8 — Nguyễn Thanh Bình

## 1. Giới thiệu dự án

Portfolio V8 là website tĩnh giới thiệu bản thân, kỹ năng, các dự án học tập, quá trình học tập và thông tin liên hệ của Nguyễn Thanh Bình, sinh viên ngành Công nghệ Thông tin 20-04. Website được xây dựng để người xem portfolio, giảng viên và nhà tuyển dụng có thể tham khảo thông tin và sản phẩm học tập.

## 2. Demo

- **Website:** [https://nguyenthanhbinh07.github.io/K20_Portfolio_CNTT20-04/](https://nguyenthanhbinh07.github.io/K20_Portfolio_CNTT20-04/)
- **Repository:** [https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04](https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04)

**Lưu ý về website trực tuyến:** URL GitHub Pages là địa chỉ dự kiến. Lần kiểm tra được ghi nhận ngày 09/11/2026, địa chỉ này trả về HTTP 404, nên chưa thể xác nhận website đang được xuất bản. Có thể mở bản chạy cục bộ theo hướng dẫn bên dưới.

## 3. Chức năng chính

- **Giới thiệu cá nhân:** tên, vai trò sinh viên, định hướng học lập trình và mục tiêu tìm hiểu AI và Security.
- **Kỹ năng:** các kỹ năng C++ cơ bản, HTML5, CSS3, Visual Studio Code, Git/GitHub và làm việc nhóm.
- **Dự án:** giới thiệu bài tập C++ cơ bản, portfolio cá nhân và website thực hành HTML/CSS. Liên kết trong các thẻ dự án hiện dẫn tới hồ sơ GitHub cá nhân, không phải repository riêng của từng dự án.
- **Quá trình học tập:** bảng học kỳ, học phần tiêu biểu và sản phẩm tương ứng.
- **Thông tin liên hệ:** email, hồ sơ GitHub và lớp học.
- **Biểu mẫu và trang kết quả:** biểu mẫu trong `index.html` dùng xác thực HTML5 phía trình duyệt: họ tên bắt buộc và ít nhất 2 ký tự, email bắt buộc đúng định dạng, lời nhắn bắt buộc từ 10 đến 500 ký tự. Khi gửi hợp lệ, biểu mẫu dùng phương thức GET để chuyển tới `ket-qua.html`. Trang kết quả thông báo biểu mẫu đã qua bước kiểm tra của trình duyệt; không có email nào được gửi và dữ liệu không được lưu trên máy chủ. Do dùng GET, dữ liệu nhập có thể xuất hiện trên URL — không gửi thông tin nhạy cảm.

## 4. Công nghệ sử dụng

- **HTML5:** cấu trúc hai trang và xác thực cơ bản cho biểu mẫu.
- **CSS3:** định dạng giao diện, hiệu ứng và bố cục responsive.
- **Google Fonts:** nạp phông Inter từ Google Fonts; cần kết nối Internet để tải phông này.
- **Git và GitHub:** quản lý và lưu trữ repository.
- **GitHub Pages:** địa chỉ dự kiến để xuất bản website; trạng thái hoạt động chưa được xác nhận như ghi chú ở mục Demo.

Dự án không sử dụng framework hoặc thư viện JavaScript.

## 5. Hướng dẫn truy cập và chạy dự án

### Truy cập website trực tuyến

1. Mở [website Portfolio](https://nguyenthanhbinh07.github.io/K20_Portfolio_CNTT20-04/). Nếu URL chưa hoạt động, hãy chạy bản cục bộ theo các bước sau.

### Clone và mở bằng VS Code

1. Mở PowerShell hoặc Terminal và clone repository:

   ```powershell
   git clone https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04.git
   ```

2. Chuyển vào thư mục dự án:

   ```powershell
   cd K20_Portfolio_CNTT20-04
   ```

3. Mở thư mục hiện tại bằng Visual Studio Code:

   ```powershell
   code .
   ```

### Chạy website

1. **Dùng Live Server:** trong VS Code, cài extension Live Server nếu chưa có; mở `index.html`, nhấp chuột phải và chọn **Open with Live Server**. Trang mở tại địa chỉ localhost do extension cung cấp.
2. **Hoặc dùng Python:** từ thư mục gốc của repository, chạy:

   ```powershell
   py -m http.server 8000
   ```

3. Mở `http://localhost:8000/` trong trình duyệt. Để xem trang kết quả, gửi biểu mẫu hợp lệ hoặc mở `http://localhost:8000/ket-qua.html`.
4. Khi dùng máy chủ Python, quay lại cửa sổ lệnh và nhấn `Ctrl+C` để dừng máy chủ.

## 6. Cấu trúc thư mục

```text
K20_Portfolio_CNTT20-04/
├── assets/
│   ├── avatar.svg
│   ├── du-an-1.svg
│   ├── du-an-2.svg
│   └── du-an-3.svg
├── css/
│   └── style.css
├── docs/
│   ├── evidence/
│   ├── AI_LOG.md
│   └── evidence-index.md
├── CHANGELOG.md
├── README.md
├── RELEASE_NOTES.md
├── index.html
└── ket-qua.html
```

`assets/` chứa ảnh đại diện và hình minh họa dự án; `css/style.css` định dạng cả trang chủ và trang kết quả. `docs/evidence/` dành cho các minh chứng, còn `docs/evidence-index.md` là danh mục minh chứng hiện có.

## 7. Kiểm thử và giới hạn

### Đã kiểm tra

- Theo ghi nhận kiểm tra ngày 09/11/2026, các tham chiếu CSS và ảnh cục bộ trong hai trang HTML trỏ tới tệp có trong repository.
- Theo ghi nhận, máy chủ HTTP tĩnh cục bộ trả HTTP 200 cho trang chủ, trang kết quả, CSS và bốn ảnh.
- Đã đối chiếu cấu hình form trong mã HTML: `action="ket-qua.html"`, `method="get"` và các ràng buộc `required`, `minlength`, `maxlength`, `type="email"`.
- URL GitHub Pages đã được kiểm tra và trả về HTTP 404 tại thời điểm nêu trên.

### Chưa kiểm tra hoặc còn giới hạn

- Chưa xác nhận website đã triển khai thành công trên GitHub Pages; cần kiểm tra lại URL sau khi cấu hình Pages.
- Chưa kiểm thử thao tác biểu mẫu trực tiếp trong trình duyệt với dữ liệu hợp lệ và không hợp lệ; hướng dẫn ở mục Chức năng chính mô tả các ràng buộc theo mã nguồn.
- Chưa kiểm tra trực quan trên nhiều trình duyệt hoặc thiết bị. CSS có các breakpoint responsive, nhưng điều đó không thay thế việc kiểm thử thực tế.
- Biểu mẫu chỉ là phần thực hành phía trình duyệt; không gửi email, không lưu dữ liệu và dữ liệu GET có thể xuất hiện trên thanh địa chỉ.
- Các liên kết GitHub của thẻ dự án hiện trỏ tới hồ sơ cá nhân.

## 8. Tài liệu liên quan

- [CHANGELOG.md](./CHANGELOG.md) — lịch sử thay đổi.
- [RELEASE_NOTES.md](./RELEASE_NOTES.md) — ghi chú bàn giao.
- [docs/AI_LOG.md](./docs/AI_LOG.md) — nhật ký sử dụng AI.
- [docs/evidence-index.md](./docs/evidence-index.md) — danh mục minh chứng.
