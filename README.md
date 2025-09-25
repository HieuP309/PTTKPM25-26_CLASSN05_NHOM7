#  Quản Lý Thư Viện – Library Management (Nhóm 7)

Dự án **Quản Lý Thư Viện** là một ứng dụng Java desktop giúp quản lý hoạt động thư viện (sách, độc giả, mượn – trả, tài khoản) theo kiến trúc 3 lớp (DAL – BUS – GUI).  
Ứng dụng được phát triển bằng **Java (Swing)** và sử dụng **MySQL** làm cơ sở dữ liệu.  
**Nhóm thực hiện: Nhóm 7**

---

##  Mục lục
- [Giới thiệu](#giới-thiệu)
- [Chức năng chính](#chức-năng-chính)
- [Kiến trúc hệ thống](#kiến-trúc-hệ-thống)
- [Yêu cầu hệ thống](#yêu-cầu-hệ-thống)
- [Cài đặt](#cài-đặt)
- [Cấu hình cơ sở dữ liệu](#cấu-hình-cơ-sở-dữ-liệu)
- [Chạy ứng dụng](#chạy-ứng-dụng)
- [Thư viện sử dụng](#thư-viện-sử-dụng)
- [Đóng góp](#đóng-góp)
- [Nhóm thực hiện](#nhóm-thực-hiện)
- [Giấy phép](#giấy-phép)

---

## Giới thiệu
Ứng dụng hỗ trợ cán bộ thư viện quản lý:
- Thông tin sách
- Thông tin độc giả
- Quản lý mượn – trả
- Quản lý tài khoản đăng nhập

Ứng dụng được thiết kế gọn nhẹ, giao diện thân thiện, dễ triển khai trong môi trường nội bộ.

---

## Chức năng chính
###  Quản lý Sách
- Thêm, sửa, xóa, tìm kiếm sách.
- Quản lý số lượng, tình trạng sách.

###  Quản lý Độc giả
- Thêm, sửa, xóa, tìm kiếm độc giả.
- Theo dõi tình trạng thẻ, hạn sử dụng.

###  Quản lý Mượn – Trả
- Tạo phiếu mượn, phiếu trả.
- Theo dõi hạn trả, tình trạng quá hạn.

###  Quản lý Tài khoản
- Đăng nhập / đăng xuất.
- Phân quyền (thủ thư, quản trị).

---

## Kiến trúc hệ thống
Dự án áp dụng kiến trúc **3 Layer**:
- **DAL (Data Access Layer):** Lớp truy xuất dữ liệu MySQL.
- **BUS (Business Logic Layer):** Xử lý nghiệp vụ, kiểm tra điều kiện.
- **GUI (Presentation Layer):** Giao diện người dùng Java Swing.

Cấu trúc thư mục:
```
Quan-Ly-Thu-Vien-Library-Management/
 ├─ Design/
 ├─ Documents/
 ├─ SRC/
 ├─ CHANGELOG.md
 └─ README.md
```

---

## Yêu cầu hệ thống
- **JDK 8+** (hoặc JDK 21 nếu đã nâng cấp).
- **IntelliJ IDEA** hoặc **Eclipse** để chạy mã nguồn.
- **MySQL Server** (port 3306 hoặc 3307 tùy cấu hình).
- Các thư viện `.jar` trong thư mục `libs`.

---

## Cài đặt
1. Clone hoặc tải về dự án:
   ```bash
      https://github.com/HieuP309/PTTKPM25-26_CLASSN05_NHOM7
   ```
2. Mở dự án bằng IntelliJ IDEA.
3. Thiết lập SDK cho dự án (JDK 8+).
4. Đảm bảo thư viện `.jar` trong thư mục `libs` đã được add vào Project Structure > Libraries.

---

## Cấu hình cơ sở dữ liệu
1. Cài đặt MySQL Server.
2. Mở file script SQL (nếu có) trong thư mục `sql/` để tạo database và các bảng.
3. Kiểm tra thông tin kết nối trong mã (host, port, user, password).
4. Nếu MySQL chạy ở port khác (vd 3307), chỉnh sửa file cấu hình `my.ini` hoặc code kết nối.

---

## Chạy ứng dụng
- Chạy class **Main** trong thư mục GUI.
- Đăng nhập bằng tài khoản mặc định (nếu có) hoặc tạo tài khoản mới trong DB.

---

## Thư viện sử dụng
- **MySQL Connector/J** – Kết nối MySQL.
- **Apache POI / POI-OOXML** – Xuất Excel.
- **JCalendar** – Chọn ngày.
- **JFreeChart** – Biểu đồ thống kê.

---

## Đóng góp
Để đóng góp vào dự án:
1. Fork dự án.
2. Tạo branch mới.
3. Commit thay đổi và tạo Pull Request.

---

## Nhóm thực hiện

**Nhóm 7:**

| Họ và tên              |
|------------------------|
| Đào Bá Phương Ninh     |
| Nguyễn Trí Chung       |
| Phạm Văn Hoàn          |
| Nguyễn Văn Hiếu        |
| Nguyễn Ngọc An         |

---

## Giấy phép
Dự án phát hành dưới giấy phép MIT.
