# VietQR BIDV từ Excel — GitHub Pages

Website tĩnh đọc Excel ngay trong trình duyệt, tạo link ảnh VietQR theo từng dòng, cho xem QR, sao chép link, tải CSV danh sách link và tải tất cả ảnh thành ZIP.

## Cài lên GitHub Pages
1. Tạo repository mới, ví dụ `vietqr-bidv-excel`.
2. Chọn **Add file → Upload files**, tải `index.html` lên thư mục gốc và bấm **Commit changes**.
3. Vào **Settings → Pages**.
4. Chọn **Deploy from a branch**, branch `main`, folder `/(root)`, bấm **Save**.
5. Sau khi xuất bản, website thường có địa chỉ `https://TEN-TAI-KHOAN.github.io/vietqr-bidv-excel/`.

## Cách sử dụng
1. Mở website, chọn file Excel.
2. Chọn trang tính, xác nhận dòng tiêu đề và ánh xạ đúng 4 cột: số tài khoản BIDV người nhận (cột bạn gọi là “Mã người chuyển”), tên, số tiền, nội dung.
3. Nhấn **Tạo mã QR**.
4. Mở ảnh, sao chép link, tải danh sách link CSV hoặc tải ZIP ảnh.

## Quan trọng về lưu trữ và quyền riêng tư
- GitHub Pages là website tĩnh, không thể tự ghi ảnh được tải lên vào repository. Link QR trong trang này là URL ảnh từ `img.vietqr.io`, không phải ảnh được lưu vĩnh viễn trong GitHub.
- Nút ZIP tải các ảnh về máy tính. Muốn link ảnh do bạn sở hữu và lưu bền vững, cần thêm dịch vụ lưu trữ ảnh có API upload hoặc backend có xác thực.
- File Excel được đọc ở trình duyệt, nhưng khi tạo ảnh QR, thông tin tài khoản, tên, số tiền và nội dung được gửi qua URL đến `img.vietqr.io`. Chỉ dùng với dữ liệu bạn được phép xử lý; không tải file Excel thật hoặc link chứa dữ liệu tài khoản lên repository công khai.
- Mã BIN BIDV được đặt là `970418`. Luôn quét thử và xác minh người nhận, số tiền, nội dung trước khi thanh toán.
- Thư viện đọc Excel và ZIP được tải từ CDN; cần Internet.
