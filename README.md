RETOFISH-Electronic (PCB, Schematic, BOM)
Thiết kế mạch điện tử cho robot cho cá ăn RETOFISH – bản Offline v1. Repo chứa sơ đồ nguyên lý, PCB, BOM, file Gerber sẵn sàng sản xuất, cùng hướng dẫn lắp ráp và kiểm thử.
License: CC BY-NC-SA 4.0 — cho phép dùng/học/chia sẻ phi thương mại. Mọi hoạt động thương mại cần sự đồng ý bằng văn bản của RETOBOTS. Xem thêm ở phần License & Thương hiệu.

Thành phần & giao tiếp chính
- MCU: ESP32 DevKit (NodeMCU-32S/DevKitC).
- RTC: DS1307 (I²C – SDA/SCL).
- Màn hình: TFT 1.47" SPI (họ ST77xx – SCK/MOSI/DC/CS/RST/BL).
- Rotary Encoder: 2 kênh + nút SW.
- LED trạng thái: LED RGB (điều khiển PWM).
- Động cơ: 28BYJ-48 (5V) + ULN2003 (driver Darlington) hoặc dùng bo ULN2003 rời qua header.
- Nguồn: 5V (cho động cơ/board) + 3.3V (logic ESP32). Chung mass (GND).
Lưu ý nguồn: 28BYJ-48 tiêu thụ ~200–300 mA/coil. Không cấp toàn bộ tải động cơ từ 3.3V của ESP32. Dùng 5V riêng cho động cơ, GND chung với ESP32. ULN2003 tích hợp diode clamp bảo vệ xung ngược cuộn dây.

Mở & chỉnh sửa (EasyEDA)
- Cài/đăng nhập EasyEDA (web hoặc desktop).
- Vào thư mục easyeda/ → mở file <project>.json / .epro.
- Sửa đổi schematic/PCB theo nhu cầu.
- Chạy DRC trước khi xuất Gerber.

Đóng góp (Contributing)
- Mọi đóng góp được cấp phép lại theo CC BY-NC-SA 4.0.
Quy trình:
- Mở Issue mô tả thay đổi (sơ đồ/footprint/DFM).
- Tạo nhánh feat/... hoặc fix/....
- Đính kèm ảnh before/after, ảnh 3D/DRC report.
- Mở Pull Request – yêu cầu DRC sạch, lỗ/footprint hợp lý, nêu rõ ảnh hưởng.
- Xem thêm CONTRIBUTING.md & CODE_OF_CONDUCT.md.

License & Thương hiệu
License: Creative Commons Attribution–NonCommercial–ShareAlike 4.0 (CC BY-NC-SA 4.0).
SPDX: CC-BY-NC-SA-4.0
Chỉ phi thương mại. Hoạt động thương mại cần sự đồng ý bằng văn bản của RETOBOTS 

Thương hiệu: Tên & logo RETOBOTS/RETOFISH là tài sản của RETOBOTS™. Vui lòng xem TRADEMARKS.md.

Liên hệ hợp tác thương mại: retobots.contact@gmail.com

Mục tiêu của repo này là giúp học sinh & cộng đồng dễ dàng tiếp cận thiết kế mạch thực chiến. Cảm ơn bạn đã cùng đóng góp!