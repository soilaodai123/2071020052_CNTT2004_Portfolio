# Portfolio cá nhân - Đỗ Văn Dũng

Portfolio CV cá nhân được xây dựng bằng HTML5 và CSS3 cho học phần Thiết kế
web. Trang giới thiệu thông tin, kỹ năng, các dự án học tập, quá trình học tập
và thông tin liên hệ; giao diện có các bố cục thích ứng với màn hình khác nhau.

## Thông tin

- **Tác giả:** Đỗ Văn Dũng
- **Môn học:** CNTT2004 - Thiết kế web
- **Mã sinh viên:** 2071020052
- **Mã nguồn:** [GitHub repository](https://github.com/soilaodai123/2071020052_CNTT2004_Portfolio)
- **Sản phẩm đã xuất bản:** [GitHub Pages](https://soilaodai123.github.io/2071020052_CNTT2004_Portfolio/)
- **Hồ sơ tác giả:** [github.com/soilaodai123](https://github.com/soilaodai123)
- **Minh chứng và ghi chú kiểm tra:** [AI_LOG.md](./AI_LOG.md)
- **Ghi chú bàn giao V7:** [RELEASE_NOTES.md](./RELEASE_NOTES.md)

## Cấu trúc thư mục

```text
.
├── index.html       # Trang portfolio chính
├── ket-qua.html     # Trang kết quả sau khi gửi form liên hệ
├── README.md        # Giới thiệu dự án và hướng dẫn kiểm tra
├── RELEASE_NOTES.md # Ghi chú bàn giao phiên bản V7
├── css/
│   └── style.css    # Kiểu dáng và bố cục responsive
├── assets/
│   ├── avt.jpg      # Ảnh đại diện
│   ├── avatar.svg   # Tài nguyên ảnh đại diện
│   ├── du-an-1.svg  # Hình minh họa dự án C++
│   ├── du-an-2.svg  # Hình minh họa portfolio
│   └── du-an-3.svg  # Hình minh họa thực hành HTML/CSS
└── AI_LOG.md       # Nhật ký sử dụng AI và ghi chú kiểm tra
```

## Chạy trên máy cá nhân

Đây là website tĩnh, không cần cài đặt thư viện hay biên dịch.

1. Tải hoặc clone repository về máy.
2. Mở terminal tại thư mục gốc của dự án.
3. Chạy máy chủ HTTP đơn giản:

   ```powershell
   py -m http.server 8000
   ```

4. Mở <http://localhost:8000> trong trình duyệt. Để dừng máy chủ, nhấn
   `Ctrl+C` trong terminal.

Cũng có thể mở trực tiếp `index.html`; dùng máy chủ cục bộ sẽ mô phỏng cách
truy cập trang đã xuất bản sát hơn.

## Nguồn và xuất bản

Mã nguồn được quản lý trong repository GitHub ở trên. Bản triển khai hiện có
thể truy cập qua GitHub Pages tại liên kết sản phẩm. Trang sử dụng phông Inter
từ Google Fonts khi có kết nối Internet; các tệp HTML, CSS và hình minh họa
nằm trong repository.

## Cách kiểm tra trang và chức năng

1. **Trang chính:** mở `index.html` hoặc URL GitHub Pages. Kiểm tra các phần
   Giới thiệu, Kỹ năng, Dự án, Học tập và Liên hệ; thử các liên kết trên menu
   để chuyển tới từng phần.
2. **Hiển thị:** kiểm tra ảnh đại diện và ba hình minh họa dự án; thu nhỏ cửa
   sổ trình duyệt để xem bố cục trên màn hình hẹp.
3. **Kiểm tra form:** tại phần Liên hệ, thử gửi form để trống, nhập email
   không hợp lệ hoặc lời nhắn dưới 10 ký tự. Trình duyệt sẽ yêu cầu sửa dữ
   liệu theo các ràng buộc HTML; form yêu cầu họ tên tối thiểu 2 ký tự, email
   hợp lệ và lời nhắn từ 10 đến 500 ký tự.
4. **Trang kết quả:** nhập dữ liệu hợp lệ rồi chọn **Gửi lời nhắn**. Trình
   duyệt chuyển tới `ket-qua.html`; dùng liên kết **Quay lại liên hệ** để
   trở lại trang chính. Đây là form minh họa: không gửi email và không lưu
   thông tin trên máy chủ. Phương thức GET đưa dữ liệu đã nhập vào URL, vì vậy
   không nên điền thông tin nhạy cảm.

## Lưu ý

Các URL GitHub hiển thị trong thẻ dự án trên portfolio hiện là nội dung mẫu
được ghi rõ là cần cập nhật; chúng không phải liên kết tới mã nguồn thực của
các dự án đó.
