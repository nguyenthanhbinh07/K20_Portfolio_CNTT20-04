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

## Thông tin chung

- **Tên dự án:** Portfolio V8 — Nguyễn Thanh Bình.
- **Mục đích sử dụng AI:** hỗ trợ rà soát dự án, soạn và sắp xếp tài liệu bàn giao; đối chiếu nội dung tài liệu với mã nguồn và lịch sử Git.
- **Phạm vi hỗ trợ:** đọc cấu trúc repository, HTML/CSS và lịch sử Git; đề xuất và cập nhật README, changelog, chỉ mục minh chứng và nhật ký AI. AI không thay thế việc kiểm thử thực tế, xác nhận của người thực hiện hoặc quyết định phát hành.

## Nhật ký sử dụng AI

| Thời gian | Công cụ AI | Nội dung yêu cầu | Kết quả sử dụng | Người kiểm tra |
|---|---|---|---|---|
| 09/11/2026 | AI assistant trong VS Code (Copilot SDK) | Rà soát đường dẫn tài nguyên và hoàn thiện tài liệu bàn giao Portfolio. | Đối chiếu HTML với tài nguyên; ghi nhận sửa đường dẫn CSS/ảnh và kết quả kiểm tra đã được nêu trong phần lịch sử phía trên. | Người thực hiện; xác nhận độc lập chưa được ghi nhận. |
| 09/11/2026 | AI assistant trong VS Code (Copilot SDK) | Tạo cấu trúc `docs/`, chuyển nhật ký AI và bổ sung danh mục minh chứng. | Tạo `docs/AI_LOG.md`, `docs/evidence-index.md` và thư mục `docs/evidence/`; thư mục minh chứng hiện chỉ có `.gitkeep`. | Người thực hiện; xác nhận độc lập chưa được ghi nhận. |
| 09/11/2026 | AI assistant trong VS Code (Copilot SDK) | Cập nhật README cho Portfolio V8 dựa trên nội dung repository. | Cập nhật `README.md` về chức năng, cách chạy, cấu trúc, kiểm tra và giới hạn; kiểm tra whitespace bằng `git diff --check`. | Người thực hiện; xác nhận độc lập chưa được ghi nhận. |
| 09/11/2026 | AI assistant trong VS Code (Copilot SDK) | Đối chiếu Git history và hoàn thiện changelog, không tự gán ngày phát hành hoặc tag. | Cập nhật `CHANGELOG.md`; ghi nhận lịch sử commit và nêu rõ chưa tìm thấy tag v7, v8, v8.1. Kiểm tra whitespace bằng `git diff --check`. | Người thực hiện; xác nhận độc lập chưa được ghi nhận. |
| 09/11/2026 | AI assistant trong VS Code (Copilot SDK) | Bổ sung thông tin chung, bảng nhật ký và đánh giá việc dùng AI. | Bổ sung nội dung trong tệp này; giữ nguyên các phần nhật ký có sẵn và nêu rõ dữ kiện ngày 30/10 chưa tìm thấy để đối chiếu. | Người thực hiện; xác nhận độc lập chưa được ghi nhận. |

### Tính toàn vẹn của nhật ký trước đây

Yêu cầu hiện tại đề cập nhật ký kiểm tra ngày 30/10/2026, gồm kết quả CSS, trang `ket-qua.html` và mã phản hồi HTTP. Tuy nhiên, nội dung `docs/AI_LOG.md` đang có và các phiên bản của `AI_LOG.md` tìm thấy trong lịch sử Git đều không chứa mục ngày này; ghi nhận kiểm tra đang có mang ngày 09/11/2026. Vì vậy, không thể chép lại hoặc xác nhận nguyên văn kết quả và từng mã HTTP của ngày 30/10 từ nguồn hiện có. Phần nhật ký đã có ở trên được giữ nguyên; cần bản ghi gốc để bổ sung chính xác thông tin ngày 30/10.

## Đánh giá việc sử dụng AI

- **AI đã hỗ trợ:** rà soát nội dung repository và Git, soạn/cập nhật tài liệu, sắp xếp nhật ký và chỉ mục minh chứng.
- **Cần kiểm tra bằng mã nguồn thực tế:** đường dẫn CSS và ảnh, cấu hình form và trang kết quả, công nghệ sử dụng, cấu trúc thư mục; các nội dung này không nên chỉ dựa vào đề xuất của AI.
- **Kết quả đã được kiểm tra trong quá trình làm việc:** nội dung HTML/CSS và tài nguyên hiện có được đối chiếu; trạng thái Git/tag được truy vấn; các lần cập nhật README và CHANGELOG đã chạy `git diff --check`. Ghi nhận HTTP 200/404 được giữ theo nhật ký trước đó, không được chạy lại trong lần cập nhật này.
- **Chưa xác minh:** nhật ký kiểm tra ngày 30/10/2026 và các mã phản hồi HTTP tương ứng; xác nhận độc lập của sinh viên đối với các kết quả do AI ghi; trạng thái phát hành và hoạt động GitHub Pages sau thời điểm đã nêu.
- **Trách nhiệm cuối cùng:** sinh viên chịu trách nhiệm kiểm tra nội dung, kiểm thử website, xác nhận minh chứng và phê duyệt mọi nội dung trước khi bàn giao hoặc phát hành. Đề xuất của AI không tự nó chứng minh rằng một thao tác hay kiểm thử đã được thực hiện.
