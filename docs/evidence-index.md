# Danh mục minh chứng và kiểm thử — Portfolio V8

## Tệp minh chứng hiện có

Đã kiểm tra toàn bộ `docs/evidence/`. Thư mục hiện chỉ có `.gitkeep`; không có ảnh minh chứng. Cả chín tên được đề nghị dưới đây đều chưa tồn tại, vì vậy không tạo liên kết ảnh giả:

- `01-github-repository.png`
- `02-readme.png`
- `03-changelog.png`
- `04-evidence-index.png`
- `05-github-tags.png`
- `06-portfolio-website.png`
- `07-responsive-375px.png`
- `08-navigation.png`
- `09-ket-qua-form.png`

## Bảng kiểm thử mới

Các kiểm tra mới trong bảng được thực hiện ngày 09/11/2026. Kết quả tương tác trình duyệt là trên bản chạy local; chúng không chứng minh trạng thái triển khai hoặc trải nghiệm ở chế độ ẩn danh.

| STT | Nội dung kiểm thử | Phương pháp | Kết quả | Minh chứng |
|---:|---|---|---|---|
| 1 | Truy cập website GitHub Pages trong cửa sổ ẩn danh | Gửi yêu cầu HTTP tới URL Pages; không thực hiện được kiểm tra trong cửa sổ ẩn danh. | **CHƯA KIỂM TRA** — yêu cầu HTTP mới trả 200 và nội dung có tiêu đề Portfolio, nhưng lượt mở bằng browser báo lỗi tải trang; chưa xác nhận trong cửa sổ ẩn danh. Nhật ký trước đó cùng ngày ghi HTTP 404. | [Website GitHub Pages](https://nguyenthanhbinh07.github.io/K20_Portfolio_CNTT20-04/); chưa có ảnh. |
| 2 | Kiểm tra giao diện Portfolio | Mở bản local trong browser; kiểm tra nội dung trang, CSS và trạng thái tải ảnh. | **ĐẠT** — trang hiển thị nội dung portfolio, CSS được áp dụng và 4 ảnh tải không lỗi. Chỉ xác nhận trên browser/môi trường kiểm tra này. | [index.html](../index.html), [style.css](../css/style.css); chưa có ảnh. |
| 3 | Kiểm tra menu điều hướng | Nhấp mục “Kỹ năng” trên trang local và kiểm tra fragment URL. | **ĐẠT** — điều hướng tới `#ky-nang`. | [index.html](../index.html); chưa có ảnh. |
| 4 | Kiểm tra responsive tại chiều rộng 375px | Đặt browser viewport rộng 375px và kiểm tra chiều rộng nội dung. | **ĐẠT** — viewport 375px, nội dung không tràn ngang. | [style.css](../css/style.css); chưa có ảnh. |
| 5 | Kiểm tra README trên GitHub | Mở README ở trang repository GitHub và đối chiếu với bản local. | **KHÔNG ĐẠT** — GitHub hiển thị README cũ; các nội dung Portfolio V8 và hướng dẫn Live Server trong bản local chưa xuất hiện trên GitHub. | [README trên GitHub](https://github.com/nguyenthanhbinh07/K20_Portfolio_CNTT20-04#readme), [README local](../README.md); chưa có ảnh. |
| 6 | Kiểm tra CHANGELOG | Đối chiếu tệp local với cây `origin/main`. | **KHÔNG ĐẠT** — `CHANGELOG.md` có trong working tree nhưng chưa có trong `origin/main`. | [CHANGELOG.md](../CHANGELOG.md); chưa có ảnh. |
| 7 | Kiểm tra Git tag v7 và v8 | Liệt kê Git tag trong repository. | **KHÔNG ĐẠT** — không tìm thấy Git tag nào, gồm v7 và v8. | Kết quả `git tag --list`; chưa có ảnh. |
| 8 | Kiểm tra CSS và đường dẫn tài nguyên | Đối chiếu đường dẫn cục bộ trong hai HTML với tệp; yêu cầu HTTP tới trang, CSS và ảnh trên máy chủ local. | **ĐẠT** — các tham chiếu CSS/ảnh tồn tại; `index.html`, `ket-qua.html`, CSS và bốn ảnh đều trả HTTP 200 trên máy chủ local. | [index.html](../index.html), [ket-qua.html](../ket-qua.html), [style.css](../css/style.css); chưa có ảnh. |
| 9 | Kiểm tra trang `ket-qua.html` | Trên browser local, thử xác thực form rồi gửi dữ liệu hợp lệ bằng GET. | **ĐẠT** — form trống bị trình duyệt chặn; dữ liệu hợp lệ chuyển tới trang kết quả và tiêu đề trang hiển thị. Không kiểm tra gửi email hoặc lưu máy chủ; mã nguồn nêu rõ không có các chức năng đó. | [ket-qua.html](../ket-qua.html), [index.html](../index.html); chưa có ảnh. |

## Kết quả kiểm tra đã ghi trước đó

Nhật ký hiện có ghi ngày 09/11/2026 rằng:

- Kiểm tra tĩnh cho thấy các đường dẫn CSS và ảnh trong hai trang HTML trỏ tới tệp có trong repository; cấu hình form dùng GET và các ràng buộc HTML5 như mô tả trong [index.html](../index.html).
- Trên máy chủ HTTP tĩnh local, trang chủ, trang kết quả, CSS và bốn ảnh trả HTTP 200.
- URL GitHub Pages được ghi nhận trả HTTP 404.
- Chưa kiểm thử thao tác biểu mẫu trực tiếp trong browser vào thời điểm ghi nhật ký đó.

Các ghi nhận trên được giữ riêng với kết quả kiểm thử mới ở bảng. Yêu cầu có nhắc đến kết quả lịch sử ngày 30/10/2026, nhưng ngày này và các mã HTTP tương ứng không có trong `docs/AI_LOG.md`, chỉ mục minh chứng hiện có hoặc lịch sử Git đã kiểm tra. Không thể khôi phục chính xác dữ liệu đó từ repository hiện tại; cần bản ghi gốc để bổ sung, không suy diễn từ kết quả ngày 09/11.

## Kết luận và việc cần bổ sung

- **Đã kiểm tra:** giao diện trên browser local, điều hướng menu, responsive ở viewport 375px, tài nguyên cục bộ, CSS, xác thực form và chuyển tới trang kết quả. Yêu cầu HTTP mới tới GitHub Pages trả 200 nhưng chưa xác nhận bằng cửa sổ ẩn danh.
- **Hạn chế hiện tại:** không có ảnh minh chứng; lượt mở Pages trong browser báo lỗi tải trang; kiểm tra Pages trong cửa sổ ẩn danh chưa thực hiện. README V8 và CHANGELOG trong working tree chưa có trên `origin/main`; repository chưa có tag v7/v8.
- **Cần kiểm tra/bổ sung:** mở Pages trong cửa sổ ẩn danh và ghi lại kết quả; xác nhận bản README/CHANGELOG được hiển thị sau khi cập nhật GitHub; tạo và xác minh tag chỉ khi phát hành thực tế; chụp, lưu ảnh minh chứng sau mỗi lần kiểm thử; cung cấp bản ghi gốc ngày 30/10/2026 nếu cần lưu kết quả lịch sử đó.
