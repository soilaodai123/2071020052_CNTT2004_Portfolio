# Release notes - Portfolio cá nhân V7

- **Tên sản phẩm:** Portfolio CV cá nhân - Đỗ Văn Dũng
- **Phiên bản bàn giao:** V7
- **Ngày cập nhật:** 2026-10-30
- **Tác giả:** Đỗ Văn Dũng

## Mã nguồn bàn giao

Snapshot bàn giao là working tree hiện tại của repository, gồm các tệp:

- [Trang portfolio](./index.html)
- [Trang kết quả form](./ket-qua.html)
- [CSS](./css/style.css)
- [README hướng dẫn](./README.md)
- [Nhật ký AI](./AI_LOG.md)

Repository: [soilaodai123/2071020052_CNTT2004_Portfolio](https://github.com/soilaodai123/2071020052_CNTT2004_Portfolio).

**Commit nền tại thời điểm ghi chú:** [`d9e5625`](https://github.com/soilaodai123/2071020052_CNTT2004_Portfolio/commit/d9e562585f3c83da10c08007620d58ad9a4cbf4c) trên nhánh `main`. Commit này có trước các cập nhật README và nhật ký V7 hiện tại; các cập nhật bàn giao chưa được commit hoặc push. Vì vậy, liên kết commit là mốc nền tham chiếu, không phải một revision GitHub đã chứa toàn bộ snapshot bàn giao. Để có liên kết cố định tới đúng bản mã trên GitHub, cần commit và push snapshot này rồi cập nhật ghi chú với commit mới.

## Thay đổi chính

- Bổ sung README tiếng Việt với mô tả sản phẩm, thông tin tác giả, cấu trúc
  thư mục, cách chạy local và hướng dẫn kiểm tra các phần chính cùng form.
- Viết lại nhật ký thành [AI_LOG.md](./AI_LOG.md), nêu dữ kiện, nhận định,
  gợi ý AI, quyết định, thay đổi và giới hạn kiểm tra.
- Bổ sung ghi chú bàn giao phiên bản V7 này.

## Lỗi đã sửa

- Sửa thiếu tài liệu hướng dẫn và nhật ký chưa thể hiện rõ quyết định của
  sinh viên; chuẩn hóa tên nhật ký thành `AI_LOG.md`.
- Không có sửa lỗi runtime HTML/CSS trong đợt cập nhật tài liệu này. Lỗi ảnh
  chưa được tái hiện; ghi chú trước đó về dấu ngoặc CSS không khớp với các
  khối CSS hiện có, nên không thêm dấu đóng dư.

## Kiểm tra đã thực hiện

- Xác nhận trang GitHub Pages trả về HTTP 200 trong lần cập nhật README trước;
  điều này không xác nhận mọi nội dung hoặc chức năng của trang.
- Xem lại các khối CSS được nêu trong ghi chú cũ và xác nhận dấu đóng khối
  hiện diện.
- Chạy `git diff --check` sau khi cập nhật README và nhật ký; không có lỗi
  khoảng trắng được báo cáo.
- Chưa kiểm thử form thủ công trên trình duyệt trong đợt cập nhật này.

## Hạn chế còn lại

- Form liên hệ chỉ dùng GET để chuyển tới trang kết quả; không gửi email,
  không lưu dữ liệu và có thể làm lộ nội dung nhập trong URL. Không nhập dữ
  liệu nhạy cảm.
- Liên kết GitHub trong các thẻ dự án là nội dung mẫu, chưa phải liên kết tới
  mã nguồn các dự án.
- Phông Inter lấy từ Google Fonts và cần kết nối Internet để tải.
- Phiên bản V7 ở đây là nhãn bàn giao; tiêu đề tài liệu trong `index.html`
  vẫn ghi “Portfolio V5” và chưa được đổi trong đợt này.
- Nhật ký trước đó ghi nhận trang GitHub Pages và mã local có nội dung khác
  nhau. URL Pages đã được xác nhận truy cập được, nhưng chưa đối chiếu lại
  toàn bộ nội dung đang triển khai với snapshot này.

## Tiếp tục kiểm tra và bàn giao

1. Chạy local theo hướng dẫn trong [README.md](./README.md), mở trang chính,
   kiểm tra menu, ảnh, bố cục màn hình hẹp, xác thực form và trang kết quả.
2. Khi lỗi ảnh xuất hiện, kiểm tra URL yêu cầu, trạng thái ảnh trong Network,
   Console và cách viết hoa/thường tên tệp.
3. Nếu cần bản bàn giao có thể dẫn tới bằng một liên kết Git cố định, commit
   và push đúng snapshot hiện tại rồi thay liên kết commit nền ở trên bằng
   commit mới.
4. Sau khi xác minh nội dung được triển khai, cập nhật URL Pages và kết quả
   kiểm tra nếu cần.
