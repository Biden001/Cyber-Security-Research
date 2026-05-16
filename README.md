# 🌐 Đồ Án An Ninh Mạng: Nghiên Cứu & Khai Thác SQL Injection Trên DVWA (Nhóm 14)

![Topic](https://img.shields.io/badge/Topic-SQL%20Injection-red?style=flat-down&logo=probot&logoColor=white)
![Environment](https://img.shields.io/badge/Environment-DVWA%20Lab-orange?style=flat-down&logo=securityscorecard&logoColor=white)
![Language](https://img.shields.io/badge/Stack-PHP%20%26%20MySQL-blue?style=flat-down&logo=php&logoColor=white)

Một dự án nghiên cứu và thực nghiệm giả lập về lỗ hổng bảo mật ứng dụng web nguy hiểm hàng đầu (SQL Injection) trên môi trường Damn Vulnerable Web Application (DVWA), từ đó đưa ra các giải pháp lập trình an toàn để vá lỗi và bảo vệ hệ thống.

---

### 🎯 Mục Đích Dự Án
* **Hiểu rõ bản chất lỗ hổng:** Nghiên cứu một cách hệ thống về khái niệm, cơ chế hoạt động và mức độ nguy hiểm của các dạng tấn công SQL Injection đối với an toàn dữ liệu web.
* **Mô phỏng thực tế nhằm nhận thức:** Xây dựng một môi trường lab giả lập để mô phỏng trực quan các kịch bản xâm nhập điển hình của hacker.
* **Đề xuất giải pháp phòng vệ:** Phân tích mã nguồn tồn tại lỗ hổng, đề xuất phương pháp tối ưu giúp lập trình viên và quản trị viên phòng chống tấn công một cách triệt để.

---

### 🛠️ Chức Năng & Nội Dung Thực Nghiệm Chính

1. **Phân tích phân loại các dạng lỗi SQLi:**
   * Nghiên cứu chi tiết kỹ thuật khai thác của các dạng lỗi phổ biến: *Authentication Bypass, Error-based, Union-based, và Blind SQL Injection (Boolean-based, Time-based)*.

2. **Thực nghiệm Vượt qua Đăng nhập (Login Bypass):**
   * Giả lập kịch bản tấn công vào form login của DVWA (mức độ bảo mật thấp). Sử dụng chuỗi ký tự đặc biệt (ví dụ: `admin' #`) để bẻ gãy logic xác thực của câu lệnh SQL, đăng nhập thành công mà không cần mật khẩu.

3. **Thực nghiệm Khai thác & Trích xuất Dữ liệu (Union-based):**
   * Lợi dụng toán tử `UNION` để kết hợp các câu lệnh truy vấn độc hại, ép giao diện ứng dụng hiển thị thông tin nhạy cảm cấu trúc cơ sở dữ liệu.
   * Thực hiện quy trình dò tìm số cột, lấy thông tin phiên bản máy chủ, liệt kê bảng/cột và trích xuất thành công dữ liệu tài khoản kèm chuỗi băm mật khẩu (Hash MD5).

4. **Xây dựng Giải pháp Vá lỗi & Phòng thủ Chuyên sâu:**
   * Khẳng định và triển khai kỹ thuật **Prepared Statement (Truy vấn tham số hóa)** làm lá chắn lõi để tách biệt hoàn toàn mã điều khiển và dữ liệu đầu vào.
   * Đề xuất các giải pháp bảo mật nhiều lớp: Kiểm soát dữ liệu đầu vào, ẩn thông tin debug lỗi, thiết lập Tường lửa ứng dụng web (WAF) và hệ thống phát hiện/ngăn chặn xâm nhập IDS/IPS.

---

### 💻 Công Nghệ & Công Cụ Sử Dụng
* **Môi trường giả lập:** DVWA (Damn Vulnerable Web Application)
* **Nền tảng ứng dụng:** Ngôn ngữ lập trình PHP & Hệ quản trị cơ sở dữ liệu MySQL
* **Công cụ hỗ trợ đề xuất:** SQLMap, Burp Suite, OWASP ZAP

---

### 👥 Thành Viên Thực Hiện
* **Sinh viên thực hiện (Nhóm 14):** Đoàn Quang Huy và các người cộng sự.
