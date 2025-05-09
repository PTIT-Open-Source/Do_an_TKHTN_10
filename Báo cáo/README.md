# 🔌 Thiết kế nhà thông minh sử dụng công nghệ BLE Mesh

> **Mô tả ngắn gọn:** Dự án thiết kế hệ thống nhà thông minh sử dụng công nghệ BLE Mesh. Hệ thống giúp điều khiển và giám sát các thiết bị trong nhà một cách linh hoạt, không cần kết nối Wi-Fi, phù hợp cho các ứng dụng IoT chi phí thấp.

## Mục Lục
- [Giới thiệu](#giới-thiệu)
- [Thông số kỹ thuật](#thông-số-kỹ-thuật)
- [Danh sách linh kiện](#danh-sách-linh-kiện)
- [Sơ đồ nguyên lý và PCB](#sơ-đồ-nguyên-lý-và-pcb)
- [Hướng dẫn lắp ráp](#hướng-dẫn-lắp-ráp)
- [Lập trình firmware](#lập-trình-firmware)
- [Cài đặt môi trường](#cài-đặt-môi-trường)
- [Cách sử dụng](#cách-sử-dụng)
- [Kiểm thử](#kiểm-thử)
- [Ảnh/Video demo](#ảnhvideo-demo)
- [Đóng góp](#đóng-góp)

## Giới Thiệu

- Dự án xây dựng một hệ thống nhà thông minh dựa trên công nghệ BLE Mesh, cho phép các thiết bị như công tắc, đèn, cảm biến khí gas, cảm biến cửa... giao tiếp với nhau trong mạng lưới không dây, không cần kết nối Internet liên tục. Mỗi thiết bị có thể đóng vai trò client, server hoặc relay trong hệ thống mesh.

- Người dùng chính là các hộ gia đình, văn phòng nhỏ, hoặc các khu căn hộ muốn triển khai giải pháp điều khiển thiết bị điện thông minh, tiết kiệm điện và đảm bảo an toàn (ví dụ: phát hiện rò rỉ khí gas hoặc mở cửa trái phép).

- Thiết kế phục vụ mục đích giáo dục, nghiên cứu và có thể mở rộng thành sản phẩm thương mại. Hệ thống giúp sinh viên, nhà phát triển hoặc doanh nghiệp nhỏ hiểu rõ về ứng dụng thực tiễn của BLE Mesh trong tự động hóa tòa nhà.

## Thông Số Kỹ Thuật

| Thành phần     | Thông tin               |
|----------------|-------------------------|
| MCU            | ESP32-WROOM-32          |
| Nguồn vào      | 5V qua USB hoặc DC      |
| Kết nối        | Bluetooth               |
| Kích thước PCB | Không có                |

---

## Danh Sách Linh Kiện

| Tên linh kiện             | Số lượng | Ghi chú                    |
|---------------------------|----------|----------------------------|
| ESP32 DevKit v1           | 3        | Vi điều khiển chính        |
| LED                       | 1        | LED đơn                    |
| Nút nhấn                  | 1        | Điều khiển thủ công        |

## Sơ đồ Nguyên lý và PCB ( Không có )

## Hướng dẫn lắp ráp ( Không có )

## Lập trình firmware

- Ngôn ngữ: C.
- Công cụ: Visual Code, ESP-IDF Terminal.

##  Cài đặt môi trường
### Cài đặt Microsoft Visual Studio Code 
- Truy cập trang chính thức: [Visual studio Code](https://code.visualstudio.com/).
- Nhấn nút **Download for Windows** hoặc chọn hệ điều hành khác (macOs, Linux).
		
Cài đặt 
- Chạy file .exe vừa tải về.
- Tích chọn các tùy chọn cần thiết ( **Add to PATH**, **Register as default editor**).
- Nhấn **Next** và hoàn tất cài đặt.
		
Cài các tiện ích cần thiết
- **C/C++**
- **PlatformIO**
- **ESP-IDF** ( Nếu không cài trong Extension thì có thể cài riêng ở ngoài).
### Cài đặt ESP-IDF thủ công
- Truy cập trang chính thức: [ESP-IDF](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html).
- Chọn hệ điều hành của bạn:
	- **Windows**
	- **Linux**
	- **MacOS**
- Cài đặt ( ở đây đang cài trên Windows)
- Sau khi vào theo đường link trên, kéo xuống chọn download( ảnh minh họa)
![alt](anh_1.png)
- Tiếp đến chọn **Windows Installer Download**
![alt](anh_2.png)
- Chọn phiên bản mà bạn muốn rồi nhấn down( ở đây mình dùng ver 5.2.5)
![alt](anh_3.png)


		
		
		

