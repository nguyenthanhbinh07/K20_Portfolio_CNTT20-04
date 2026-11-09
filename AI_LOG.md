# Nhật ký sử dụng AI

## Bối cảnh và dữ kiện ban đầu

- Tài liệu ban đầu trong `README.md` chỉ có tên repository và mô tả ngắn; thiếu hướng dẫn chạy, kiểm tra và liên kết minh chứng.
- Ghi chú ban đầu trong tệp này là “sai đường dẫn css / không hiện avatar”.
- Đối chiếu mã nguồn: `index.html` liên kết `style.css` ở thư mục gốc trong khi tệp thực tế là `css/style.css`; ảnh được gọi là `assets/f.jpg` nhưng tài nguyên hiện có là `assets/avatar.svg`.
- Repository có hai trang HTML: portfolio ở `index.html` và trang kết quả form ở `ket-qua.html`. Form dùng GET cùng xác thực HTML5, không có backend.
- URL GitHub Pages theo tên tài khoản/repository trả về 404 khi được kiểm tra ngày 09/11/2026. Đây là quan sát tại thời điểm kiểm tra, không phải bằng chứng về cài đặt Pages trong repository.

## Nhận định trước khi dùng AI

Ghi chú hiện có đã quy lỗi hiển thị CSS cho đường dẫn; kiểm tra tệp xác nhận đường dẫn trong HTML không khớp cấu trúc thư mục. Ảnh không hiển thị vì tham chiếu tới tệp không có trong repository. Có thể sửa bằng các tài nguyên đã có, không cần tạo ảnh hoặc CSS mới.

## Công cụ và nội dung trao đổi

- **Công cụ:** AI assistant trong VS Code (Copilot SDK).
- **Yêu cầu/prompt được dùng:** cập nhật `README.md`, `AI_LOG.md` và tạo `RELEASE_NOTES.md` cho bản bàn giao v7; nội dung phải theo sản phẩm thực tế, ghi nhận đúng trạng thái kiểm tra và không tạo kết quả chưa thực hiện.
- **Gợi ý của AI:** kiểm tra các HTML/CSS/tài nguyên và thông tin Git; sửa đường dẫn sai dựa trên tệp thực có; nêu rõ URL Pages đang 404 thay vì khẳng định đã xuất bản; mô tả đúng hành vi GET của form.
- **Quyết định:** thực hiện hai sửa đường dẫn đã được dữ kiện xác nhận; ghi tài liệu theo các trang, trường form và tài nguyên hiện hữu; ghi Pages là chưa xác nhận xuất bản. Không khẳng định form gửi email/lưu dữ liệu và không bịa minh chứng hoặc kết quả chạy thử.

## Phần đã sửa

- Trong `index.html`, đổi CSS sang `css/style.css`.
- Trong `index.html`, đổi ảnh đại diện sang tài nguyên sẵn có `assets/avatar.svg`.
- Viết lại `README.md` với cấu trúc, hướng dẫn chạy local, luồng kiểm tra, hồ sơ và minh chứng; ghi rõ trạng thái Pages.
- Tạo `RELEASE_NOTES.md` mô tả phạm vi bản v7 và mã nguồn liên quan.

## Cách thử lại và kết quả

- Chạy kiểm tra tĩnh trên hai trang HTML: tất cả đường dẫn CSS/ảnh cục bộ đều trỏ tới tệp tồn tại; xác nhận form có `action="ket-qua.html"`, `method="get"`, họ tên tối thiểu 2 ký tự, email kiểu email và lời nhắn dài 10–500 ký tự.
- Chạy máy chủ HTTP tĩnh cục bộ và yêu cầu trang chủ, trang kết quả, CSS cùng bốn ảnh: cả bảy đường dẫn đều trả HTTP 200.
- Kiểm tra URL Pages: trả về HTTP 404 ngày 09/11/2026; chưa thể xác nhận triển khai công khai.
- Chưa kiểm thử thao tác trực tiếp trong trình duyệt hoặc gửi form; các bước này được hướng dẫn trong `README.md` và cần thực hiện khi bàn giao.
