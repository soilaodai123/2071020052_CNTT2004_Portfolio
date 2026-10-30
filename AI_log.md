Không hiện ảnh
Không đúng đường dẫn
# Báo cáo chẩn đoán

Ngày kiểm tra: 2026-10-30

Phạm vi: `index.html`, `ket-qua.html`, `css/style.css` và thư mục `assets/`.

Không phát hiện lỗi cú pháp HTML/CSS bằng bộ kiểm tra hiện có. Chưa sửa các file mã nguồn; các mục dưới đây là đề xuất.

## Các vấn đề và đề xuất

1. **Tên hiển thị không nhất quán:** logo trên trang chủ ghi "Việt Anh", trong khi tiêu đề trang, phần giới thiệu và trang kết quả đều ghi "Đỗ Văn Dũng". Đề xuất đổi logo trang chủ cho thống nhất.

2. **Ảnh đại diện:** `index.html` tham chiếu `assets/avt.jpg` và file này hiện có trong thư mục `assets/`. Ba ảnh dự án cũng tồn tại đúng tên được tham chiếu. Vì vậy, hiện chưa thấy sai đường dẫn trong mã nguồn. Nếu trình duyệt vẫn không hiện ảnh, hãy kiểm tra Console/Network, bảo đảm mở trang từ thư mục dự án và tên file khớp chính xác chữ hoa/chữ thường.

3. **Ảnh dự án không khớp nội dung:** ảnh `assets/du-an-2.svg` có nhãn "Dự án 2 – Flutter", nhưng thẻ dự án tương ứng mô tả "Portfolio CV cá nhân". Đề xuất thay ảnh hoặc sửa nhãn trong ảnh để khớp mô tả.

4. **Trang kết quả thiếu kiểu trình bày riêng:** `ket-qua.html` dùng các lớp `result-main` và `result-panel`, nhưng `css/style.css` chưa định nghĩa kiểu cho hai lớp này. Đề xuất bổ sung khoảng cách, giới hạn chiều rộng và cách trình bày phù hợp để nội dung không dính sát phần đầu trang.

5. **Form đưa dữ liệu lên URL:** form dùng `method="get"`; email và lời nhắn sẽ xuất hiện trong query string. Trang đã cảnh báo hành vi này, phù hợp với bài thực hành, nhưng không nên dùng cho dữ liệu thật. Nếu triển khai thực tế, cần xử lý qua máy chủ bằng POST và tránh lưu dữ liệu nhạy cảm không cần thiết.

6. **Liên kết dự án chưa hoàn chỉnh:** các địa chỉ GitHub trong phần dự án chỉ là văn bản và còn ghi "liên kết cần cập nhật". Đề xuất thay bằng URL chính xác và dùng thẻ liên kết nếu dự án đã được công khai.

7. **Chân trang trang kết quả chưa đồng bộ:** câu "Toi la sieu du bi." thiếu dấu tiếng Việt và khác nội dung chân trang trang chủ. Đề xuất sửa nội dung và thống nhất cách ghi tên/chân trang.

## Kết luận về ghi chú ảnh

Ghi chú ban đầu "Không hiện ảnh / Không đúng đường dẫn" chưa khớp với trạng thái file hiện tại: các đường dẫn ảnh trong HTML đều trỏ đến file đang tồn tại. Cần kiểm tra trực tiếp trên trình duyệt nếu lỗi hiển thị vẫn còn.
