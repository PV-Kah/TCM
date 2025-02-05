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
--------------------------------------------------------
Cài đặt Vivaldi bằng wget và APT
Để cài đặt Vivaldi bằng wget và APT, trước tiên, hãy đảm bảo rằng wget có trên laptop của bạn. Để làm điều này, hãy mở terminal và chạy lệnh sau:

wget --version
Nếu lệnh này trả về số phiên bản, điều đó có nghĩa là hệ thống của bạn đã có wget và bạn có thể tiến hành bước tiếp theo. Nếu không thấy số phiên bản, bạn có thể cài đặt wget bằng lệnh sau:

sudo apt install wget
Bước tiếp theo là thêm khóa công khai của kho Vivaldi vào hệ thống. Để làm việc này, hãy chạy các lệnh sau trong terminal:

wget -qO- https://repo.vivaldi.com/archive/linux_signing_key.pub
sudo apt-key add linux_signing_key.pub
Bây giờ, thêm kho lưu trữ cho Vivaldi với:

traceroute azmc.vn
sudo add-apt-repository 'deb https://repo.vivaldi.com/archive/deb/ stable main'
Cuối cùng, chạy lệnh dưới đây để cập nhật kho lưu trữ hệ thống của bạn và cài đặt Vivaldi:

sudo apt update && sudo apt install vivaldi-stable
Khi được nhắc, hãy nhập y và nhấn Enter.

Sau khi cài đặt xong, bạn có thể khởi chạy Vivaldi từ menu Ứng dụng (Applications).
