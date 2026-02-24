# Nghiên cứu Khai thác và Phòng chống lỗ hổng SQL Injection (DVWA)

## 📌 Giới thiệu dự án
Đây là dự án nghiên cứu chuyên sâu về lỗ hổng bảo mật Web phổ biến nhất - **SQL Injection**. Nội dung tập trung vào việc thực hành khai thác thực tế trên môi trường **DVWA (Damn Vulnerable Web Application)** và đề xuất các giải pháp khắc phục triệt để.

## 🛠️ Các nội dung chính đã thực hiện
* **Môi trường thử nghiệm:** Triển khai hệ thống Lab với DVWA, sử dụng cơ sở dữ liệu MySQL.
* **Kỹ thuật khai thác thực tế:**
    * **SQL Injection (Low level):** Khai thác trực tiếp qua tham số đầu vào không được kiểm soát.
    * **SQL Injection (Medium level):** Vượt qua các bộ lọc cơ bản bằng kỹ thuật thay đổi phương thức truyền tin (POST/GET).
    * **Kỹ thuật cao cấp:** Sử dụng `ORDER BY`, `UNION SELECT` để trích xuất cấu trúc database, tên bảng, cột và dữ liệu nhạy cảm của người dùng.
* **Giải pháp bảo mật & Khắc phục:**
    * Phân tích cơ chế chống tấn công ở mức độ **Low** trong DVWA.
    * Đề xuất sử dụng kỹ thuật **Prepared Statements** để ngăn chặn triệt để mã độc.

## 📂 Tài liệu đính kèm
* [Báo cáo chi tiết (PDF)](./An%20Ninh%20Mạng%20Nhóm%2014.pdf)

## 📚 Tài liệu nghiên cứu chính (Technical References)

Dự án được thực hiện dựa trên việc nghiên cứu và áp dụng các kỹ thuật từ các nguồn uy tín sau:

### 🇻🇳 Nguồn tiếng Việt:
* **WhiteHat Forum (2021):** [Khai thác Error Based SQL Injection](https://whitehat.vn/threads/sql-injection-khai-thac-error-based-sql-injection.5664/). Đây là nguồn tham khảo chính cho phần thực hành tấn công dựa trên lỗi hiển thị.

### 🌎 Nguồn tiếng Anh (Kỹ thuật chuyên sâu):
* **OWASP (2021):** [A03:2021 – Injection](https://owasp.org/Top10/2021/A03_2021-Injection/). Tiêu chuẩn toàn cầu về bảo mật ứng dụng Web.
* **The Web Application Hacker's Handbook:** *Stuttard & Pinto (2011)*. Cuốn "sách gối đầu giường" của dân Pentest để tìm kiếm lỗ hổng bảo mật.
* **SQL Injection Attacks and Defense:** *Clarke, J. (2012)*. Cung cấp các kịch bản phòng thủ thực tế mà dự án đã áp dụng (Prepared Statements).
* **Advanced SQL Injection:** *Anley, C. (2002)*. Nghiên cứu các kỹ thuật tấn công nâng cao trong môi trường SQL Server.
---
**Người thực hiện:** Biden001 và các thành viên
**Chuyên ngành:** Mạng máy tính
