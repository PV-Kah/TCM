# VietHoaConfig
Chỉ Cần Tải File index.php về up lên host là dùng bình thường
https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb

Bước 1: Mở Terminal bằng tổ hợp phím Ctrl + Alt + T.
Bước 2: Di chuyển đến thư mục chứa tệp .deb mà bạn đã tải xuống. Ví dụ:
Copy
cd ~/Downloads
Bước 3: Cài đặt Chrome bằng lệnh dpkg với dòng lệnh chi tiết sau:
Copy
sudo dpkg -i google-chrome-stable_current_amd64.deb
Bước 4: Nếu gặp lỗi phụ thuộc, bạn sử dụng lệnh apt để cài đặt các gói phụ thuộc cần thiết:
Copy
sudo apt install -f
Bước 5: Để xác nhận cài đặt Chrome thành công, bạn nhập lệnh sau:
Copy
google-chrome --version
