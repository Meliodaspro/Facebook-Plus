# Facebook Plus — bản tiếng Việt

Bản mã nguồn Việt hóa từ https://github.com/SHAJON-404/Facebook-Plus.
Đây là tweak cho Facebook iOS, không phải toàn bộ mã nguồn Facebook.

## Thay đổi
- Đặt tiếng Việt làm mặc định cho lần cài mới và sau khi đặt lại cài đặt.
- Thêm Tiếng Việt vào danh sách ngôn ngữ; cài đặt ngôn ngữ đã lưu vẫn được giữ.
- Việt hóa màn hình chào mừng, xác nhận cảm xúc và thao tác đánh dấu tin đã xem.
- Bổ sung tiếng Việt cho tiện ích Safari và chỉnh lại một số thuật ngữ.

## Biên dịch
Cần Theos, SDK iOS và toolchain tương thích theo README.md gốc.
Chạy `git submodule update --init --recursive` trước khi build.
Chạy `./build.sh` để tạo gói .deb.
Để tạo IPA, cần cung cấp IPA Facebook đã giải mã hợp lệ tại
`test/com.facebook.Facebook.ipa` và cài cyan theo hướng dẫn gốc.
Nếu dùng ZIP không chứa git metadata, tải phụ thuộc fishhook từ URL trong .gitmodules.

## Phạm vi kiểm tra
Đã kiểm tra khóa bản dịch, định dạng tham số và các lời gọi chuỗi giao diện.
Chưa biên dịch hoặc chạy trên iPhone: môi trường hiện tại không có Theos/SDK iOS
và chưa có IPA Facebook đầu vào. Không có IPA hay .deb trong gói này.
Ngôn ngữ giao diện Facebook gốc được đặt riêng trong Facebook/iOS.
Giữ nguyên giấy phép GPL-3.0 và thông tin tác giả của dự án gốc.
