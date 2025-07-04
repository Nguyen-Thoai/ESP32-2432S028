# ESP32-2432S028

![ESP32-2432S028](https://github.com/user-attachments/assets/87d8700e-05d0-4437-8973-575b42c71f6d)

Cấu hình chế độ Wi-Fi thân thiện với người dùng: Cách cấu hình chế độ được kích hoạt bằng cách nhấn giữ nút BOOT (hoặc một nút được xác định chỉ cho GPIO0) trong 1,5 giây, đặc biệt hữu ích khi thiết bị chưa được cấu hình hoặc cần thay đổi mạng Wi-Fi.

Giao diện web trực tuyến: Khi cấu hình ở chế độ, ESP32 tự động hoạt động như một điểm truy cập Wi-Fi (SSID: "ESP32-2432S028", Mật khẩu: "wificonfig") và khởi động máy chủ web người dùng có thể truy cập bằng trình duyệt web (từ điện thoại hoặc máy tính) tại địa chỉ 192.168.4.1 (hoặc bất kỳ trang web nào nhờ DNS chuyển hướng) để nhập SSID và mật khẩu của mạng Wi-Fi mong muốn.

Giám sát cường độ tín hiệu Wi-Fi (RSSI) theo thời gian thực: Hiển thị hiện tại RSSI: Hiển thị rõ ràng giá trị RSSI bằng số (ví dụ: -45 dBm) ở góc trên màn hình.

Mã hóa màu sắc thông minh: Giá trị RSSI được biểu thị bằng màu sắc trực quan (Xanh lá: tốt, Vàng: trung bình, Đỏ: yếu) giúp người dùng nhanh chóng nắm bắt chất lượng kết nối.

Hiển thị lịch sử RSSI: Biểu đồ đường dẫn hiển thị biến RSSI trong thời gian gần nhất 60 giây, cho phép theo dõi độ ổn định của tín hiệu.

Đồ thị tham chiếu chuyên nghiệp: Đường tham chiếu dBm: Đồ thị được cố định theo tham chiếu chiều ngang ở các mức 0dBm, -20dBm, -40dBm, -60dBm, -80dBm và -100dBm.

Hiển thị thông tin chi tiết về quá trình kết nối (đang kết nối, kết nối thành công, địa chỉ IP).

Cảnh báo mất kết nối: Tự động hiển thị "MẤT KẾT NỐI WIFI!" khi thiết bị không thể duy trì kết nối với mạng cấu hình.

Cảnh báo tín hiệu yếu: Hiển thị cảnh báo "TÍN HIỆU RẤT YẾU!" đính kèm giá trị SSID và RSSI khi tín hiệu giảm xuống dưới -90 dBm, giúp người dùng biết được vấn đề phù hợp.

Đồng bộ thời gian tự động (NTP): Thiết bị tự động kết nối với máy chủ NTP công cộng (time.google.com) để cập nhật và hiển thị thời gian chính xác trên màn hình, tiện ích tăng cường.

Lưu trữ thông tin an toàn: Thông tin Wi-Fi được lưu trữ vĩnh viễn trong bộ nhớ flash của ESP32 bằng thư viện tùy chọn, đảm bảo thiết bị tự động kết nối lại sau mỗi lần khởi động.

Phản hồi ngay lập tức: Giao diện web cung cấp phản hồi trạng thái kết nối ngay lập tức sau khi gửi thông tin, cùng với đếm ngược trước khi khởi động lại thiết bị.

*Công nghệ sử dụng: Vi điều khiển: ESP32 (lý tưởng cho các bo mạch phát triển như ESP32-WROOM-32, ESP32-DevKitC, hoặc các bo mạch có màn hình như 2432S028).

Đường tham chiếu thời gian: Các đường dọc nhỏ được vẽ mỗi 5 giây, cung cấp thời gian rõ ràng trên lịch sử biểu tượng.

Màn hình hiển thị: Màn hình màu TFT (ST7789) được điều khiển qua giao tiếp SPI.

Thư viện đồ họa: Adafruit_GFX và U8g2_for_Adafruit_GFX.

Kết nối mạng: WiFi thư viện của ESP-IDF.

Máy chủ Web/DNS: Library WebServer và DNSServer (chọn chế độ cấu hình).

Đồng bộ thời gian: NTPClient và WiFiUdp.

Lưu trữ dữ liệu: Tùy chọn (giúp lưu cấu hình vĩnh viễn).

Ứng dụng tiềm năng: Giám sát chất lượng Wi-Fi gia đình/văn phòng giúp xác định các "chế độ" hoặc khu vực có tín hiệu yếu, tối ưu hóa vị trí đặt bộ định tuyến hoặc thiết bị mở rộng sóng.

Phát triển và thử nghiệm IoT: Cung cấp công cụ trực quan để theo dõi cường độ tín hiệu của các thiết bị IoT trong quá trình phát triển.

Giáo dục và học tập: Là một dự án thú vị để tìm hiểu về ESP32, Wi-Fi, giao diện đồ họa và nhúng máy chủ web.

Công cụ kỹ thuật mạng: Hỗ trợ kiểm tra nhanh và đánh giá tín hiệu Wi-Fi tại các địa điểm khác nhau.

Ưu điểm: Trực quan cao Đồ họa và màu sắc giúp người dùng dễ dàng hiểu được trạng thái tín hiệu.

Dễ dàng cấu hình: Loại giao diện web bỏ cài đặt lại cho mỗi lần thay đổi mạng.

Độc lập: Sau khi cấu hình, thiết bị hoạt động độc lập mà không cần kết nối với máy tính.

Giá thành hợp lý: Dựa trên ESP32 và màn hình TFT giá rẻ.

Hỗ trợ tiếng Việt: Giúp người dùng Việt Nam dễ dàng sử dụng.
