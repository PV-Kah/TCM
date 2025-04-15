# VietHoaConfig
Chỉ Cần Tải File index.php về up lên host là dùng bình thường

🔧 Bước 1: Cài các gói cần thiết
bash
Sao chép
Chỉnh sửa
sudo apt update
sudo apt install curl ca-certificates gnupg lsb-release wget -y
🧩 Bước 2: Thêm kho Waydroid PPA (Ubuntu/Debian)
bash
Sao chép
Chỉnh sửa
curl https://repo.waydro.id | sudo bash
Lệnh này sẽ thêm repo + key cho Waydroid tự động.

📦 Bước 3: Cài Waydroid
bash
Sao chép
Chỉnh sửa
sudo apt install waydroid -y
📥 Bước 4: Tải image Android gốc
bash
Sao chép
Chỉnh sửa
sudo waydroid init
Lệnh này sẽ tải và thiết lập system image (LineageOS based)

▶️ Bước 5: Khởi động Waydroid
bash
Sao chép
Chỉnh sửa
waydroid session start
waydroid show-full-ui
Hoặc dùng waydroid show-full-ui để chạy giao diện Android

🛠 Một số lệnh hữu ích khác:

Lệnh	Mô tả
waydroid status	Kiểm tra trạng thái
waydroid shell	Mở terminal bên trong Android
waydroid app list	Liệt kê các app Android
waydroid app launch <package>	Mở app theo package name
⚙️ Cài GApps (CH Play, Google Services – không chính thức)
Cài đặt qua bên thứ ba như MindTheGapps hoặc [OpenGApps], nhưng cần patch và cẩn thận.

🧯 Gỡ cài đặt (nếu cần)
bash
Sao chép
Chỉnh sửa
sudo waydroid container stop
sudo apt purge waydroid -y
sudo rm -rf /var/lib/waydroid
Nếu bạn dùng Arch Linux hoặc Manjaro, có thể cài qua AUR:

bash
Sao chép
Chỉnh sửa
yay -S waydroid
