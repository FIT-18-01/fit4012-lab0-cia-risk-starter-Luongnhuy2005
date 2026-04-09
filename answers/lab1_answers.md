# Lab 01 Answers
## CIA & Risk: Hệ thống lưu điểm

**Họ và tên:** Lương Như Ý

**MSSV:** 1871020680

**Lớp/Nhóm:** CNTT 18-01 / Nhóm

---

## 1. Assets
Liệt kê ít nhất 2 assets cần bảo vệ.

- Asset 1: Dữ liệu (Data)
- Asset 2: Hệ thống/phần mềm (System & Software)
- Asset 3 (nếu có): Người dùng (Users)

---

## 2. Mapping CIA
Ghép từng sự cố với CIA.

- Sự cố A ->Lộ dữ liệu khách hàng
            Hacker đánh cắp mật khẩu
Ghép: Rò rỉ dữ liệu → Confidentiality
- Sự cố B ->Sửa điểm sinh viên
            Thay đổi số dư tài khoản ngân hàng
Ghép: Dữ liệu bị thay đổi → Integrity
- Sự cố C ->Website bị sập
            Bị tấn công DDoS làm không truy cập được
Ghép: Hệ thống không truy cập được → Availability

---

## 3. Phân tích sự cố B
- Threat: Hacker xâm nhập hệ thống và chỉnh sửa dữ liệu
          Nhân viên nội bộ sửa dữ liệu trái phép
          Malware (phần mềm độc hại) thay đổi dữ liệu
          Lỗi phần mềm làm sai lệch dữ liệu
- Vulnerability:Hệ thống phân quyền yếu (ai cũng có thể sửa dữ liệu)
                Không có cơ chế kiểm tra tính toàn vẹn (hash, checksum)
                Mật khẩu yếu, không có xác thực nhiều lớp (MFA)
                Không ghi log hoặc không kiểm tra log
                Phần mềm còn lỗi (bug), chưa được cập nhật
- Mitigation:Phân quyền truy cập chặt chẽ (RBAC)
              Sử dụng hash/checksum để phát hiện thay đổi dữ liệu
              Áp dụng xác thực nhiều yếu tố (MFA)
              Ghi log và theo dõi hoạt động hệ thống
              Backup dữ liệu định kỳ
              Cập nhật, vá lỗi phần mềm thường xuyên

---

## 4. Reflection
Viết 5-7 dòng.
Qua sự cố liên quan đến Integrity, em nhận thấy việc bảo vệ tính toàn vẹn dữ liệu là vô cùng quan trọng trong mọi hệ thống thông tin. Nếu dữ liệu bị thay đổi sai lệch, hậu quả không chỉ ảnh hưởng đến người dùng mà còn gây thiệt hại lớn cho tổ chức. Em hiểu rằng không chỉ hacker mà cả lỗi hệ thống hay con người cũng có thể làm mất tính toàn vẹn. Vì vậy, cần áp dụng các biện pháp như phân quyền, kiểm tra dữ liệu và sao lưu thường xuyên. Bên cạnh đó, việc giám sát và ghi log cũng rất cần thiết để phát hiện sớm sự cố. Qua bài này, em nhận thức rõ hơn vai trò của bảo mật trong thực tế.


---

## 5. Bonus Flag
`FIT4012{A-?-B-?-C-?}`

Flag của em:
A-C-B-I-C-A
