# Nhật ký sử dụng AI

Ngày: 2026-10-30

## Vấn đề và dữ kiện ban đầu

Ban đầu ghi nhận hiện tượng “không hiện ảnh”, nghi ngờ sai đường dẫn nhưng
chưa xác định được lỗi cụ thể. Ghi chú kiểm tra trước đó cho biết các đường
dẫn ảnh trong HTML dùng `assets/...`, tên tệp khớp với tài nguyên trong thư
mục `assets/`; lần kiểm tra được ghi lại lúc đó không tái hiện lỗi ảnh trên
GitHub Pages. Ghi chú cũ cũng nêu khác biệt giữa tên trên trang đã xuất bản
("Việt Anh") và nội dung mã nguồn local ("Đỗ Văn Dũng"). Các quan sát online
này là kết quả được ghi trong ghi chú trước, không phải kết quả kiểm tra lại
trong lần cập nhật nhật ký này.

## Nhận định trước khi hỏi AI

Tôi nghĩ lỗi có thể do đường dẫn ảnh hoặc do bản GitHub Pages chưa cập nhật,
nhưng chưa có dữ liệu Network/Console từ trình duyệt gặp lỗi để kết luận.

## Công cụ và gợi ý từ AI

- **Công cụ:** trợ lý AI trong VS Code; xem mã HTML, CSS, README và ghi chú
  kiểm tra hiện có.
- **Yêu cầu ban đầu (tóm tắt):** kiểm tra tình trạng ảnh không hiển thị và
  đường dẫn không đúng.
- **Gợi ý đã được ghi nhận:** kiểm tra các đường dẫn/tệp ảnh, kiểm tra bản
  GitHub Pages và nhánh/commit được triển khai; ghi chú cũ còn đề xuất bổ sung
  dấu `}` cho một số khối CSS.

## Quyết định và lý do

Tôi không áp dụng đề xuất thêm dấu `}` chỉ dựa trên ghi chú cũ. Khi xem lại
`css/style.css` hiện có, các khối `html`, `.hero`, `.button` và
`.button:hover` đều đã có dấu đóng; thêm dấu đóng lần nữa không có căn cứ và
có thể làm sai cấu trúc CSS. Tôi giữ nguyên phần HTML/CSS, vì chưa có lỗi ảnh
nào được tái hiện trong lần kiểm tra này và chưa có dữ liệu trình duyệt tại
môi trường phát sinh lỗi.

Khi cập nhật README, tôi cũng quyết định giữ lời cảnh báo về form GET: form
chỉ chuyển tới trang kết quả thực hành, không gửi email hay lưu trên máy chủ,
và nội dung được nhập có thể xuất hiện trên URL. README ghi rõ các liên kết
dự án mẫu là nội dung cần cập nhật thay vì giới thiệu chúng như sản phẩm đã
xác minh.

## Phần đã sửa

- Mở rộng `README.md` với mô tả sản phẩm, thông tin tác giả, liên kết repo và
  GitHub Pages, cấu trúc thư mục, hướng dẫn chạy local và cách kiểm tra trang
  cùng form.
- Đổi tên nhật ký từ `AI_log.md` thành `AI_LOG.md` theo tên thống nhất trong
  yêu cầu và cập nhật liên kết trong README.
- Không sửa `index.html` hoặc `css/style.css` trong các thay đổi của nhật ký
  này.

## Thử lại và kết quả

- Đã kiểm tra URL GitHub Pages trong lần cập nhật README trước: phản hồi
  HTTP 200. Đây chỉ xác nhận trang chủ truy cập được, không xác nhận mọi ảnh
  hay chức năng hoạt động trên mọi trình duyệt.
- Đã xem lại các khối CSS liên quan nêu trên; dấu đóng khối hiện diện.
- Sau khi đổi tên, kiểm tra lại liên kết README và chạy `git diff --check`;
  chưa kiểm tra thủ công form trên trình duyệt trong lần cập nhật nhật ký này.

Nếu lỗi ảnh còn xảy ra, bước tiếp theo là mở Developer Tools ở trình duyệt
gặp lỗi, kiểm tra URL và trạng thái tải của từng ảnh trong Network, cùng lỗi
liên quan trong Console; sau đó đối chiếu với tên và chữ hoa/thường của tệp
trong repository.
