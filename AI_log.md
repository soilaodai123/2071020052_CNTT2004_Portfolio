Không hiện ảnh
Không đúng đường dẫn
Bug ở đâu đó

## Kết quả kiểm tra và xử lý

Ngày kiểm tra: 2026-10-30

- **Ảnh không hiển thị / sai đường dẫn:** chưa tái hiện được trên GitHub Pages. Các ảnh đại diện và ảnh dự án tải thành công (HTTP 200); đường dẫn `assets/...` khớp với các tệp hiện có. Nếu lỗi vẫn xảy ra ở máy hoặc trình duyệt khác, cần kiểm tra URL yêu cầu, trạng thái Network và Console tại môi trường đó.
- **CSS local có khối chưa đóng:** trong `css/style.css`, thiếu dấu `}` trước các selector `body`, `.hero-inner` và `.button:hover` để đóng lần lượt các khối `html`, `.hero` và `.button`. Sửa tối thiểu là thêm mỗi dấu `}` tại các vị trí đó.
- **Bản local và bản GitHub Pages không đồng nhất:** logo hiển thị trên trang online là “Việt Anh”, khác nội dung trong `index.html` local (“Đỗ Văn Dũng”). Cần xác minh nhánh/commit đang được GitHub Pages triển khai trước khi đồng bộ.

Trạng thái: đã ghi nhận các kết quả kiểm tra và cách sửa tối thiểu; chưa chỉnh sửa mã nguồn, nên các lỗi CSS nêu trên chưa được xác nhận là đã sửa.
