# Changelog

Tất cả các thay đổi quan trọng trong dự án này sẽ được ghi lại tại đây.  
Định dạng dựa trên [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

- Cập nhật hướng dẫn cài đặt, sửa lỗi nhỏ trong giao diện.
- Nâng cấp driver MySQL lên phiên bản mới hơn.
- Bổ sung sơ đồ UML Use Case đầy đủ.

## [1.0.0] - 2025-08-18
### Added
- Phát hành lần đầu dự án **Quản Lý Thư Viện**.
- Tổ chức dự án theo mô hình 3 lớp (DAL, BUS, GUI).
- Module **Quản lý sách**: thêm, sửa, xóa, tìm kiếm sách.
- Module **Quản lý độc giả**: thêm, sửa, xóa, tìm kiếm độc giả.
- Module **Quản lý mượn trả**: cho phép mượn, trả sách, quản lý hạn trả.
- Tích hợp MySQL làm cơ sở dữ liệu, cấu hình trong file `my.ini`.
- Giao diện Java Swing cơ bản, form đăng nhập/thủ thư.

### Fixed
- Sửa lỗi kết nối MySQL mặc định (port 3306/3307).
- Cập nhật thư viện `.jar` (MySQL Connector, POI, JCalendar) vào thư mục `libs`.

### Security
- Thêm xác thực người dùng cơ bản khi đăng nhập.

