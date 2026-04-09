# FIT4012 - Report 1 Page
## Lab 01 - CIA & Risk: Hệ thống lưu điểm

### 1. Mục tiêu bài lab
- Nhận diện tài sản cần bảo vệ trong một hệ thống thông tin đơn giản.
- Phân biệt Confidentiality, Integrity, Availability.
- Xác định threat, vulnerability, mitigation.
- Thực hành workflow GitHub cơ bản để nhận và nộp bài.

### 2. Cách làm
- Đọc bối cảnh và xác định các thành phần quan trọng của hệ thống.
- Phân tích từng sự cố theo bộ ba CIA.
- Chọn sự cố B để phân tích sâu hơn theo threat - vulnerability - mitigation.
- Hoàn thiện bài làm trong repo và commit/push lên GitHub.

### 3. Kết quả chính
**Assets:**
- Dữ liệu người dùng (thông tin cá nhân, tài khoản, mật khẩu)
- Cơ sở dữ liệu hệ thống (điểm số sinh viên, giao dịch, hồ sơ)
- Hệ thống máy chủ và ứng dụng
- Mạng và kết nối hệ thống

**CIA mapping:**
- Sự cố A → Confidentiality (Tính bảo mật)
(Ví dụ: lộ thông tin người dùng, rò rỉ dữ liệu)
- Sự cố B → Integrity (Tính toàn vẹn)
(Ví dụ: sửa điểm sinh viên, thay đổi dữ liệu)
- Sự cố C → Availability (Tính sẵn sàng)
(Ví dụ: hệ thống bị sập, không truy cập được)

**Phân tích sự cố B:**
- Threat: Hacker hoặc người dùng nội bộ cố ý chỉnh sửa dữ liệu (ví dụ: sửa điểm sinh viên, thay đổi số dư tài khoản).
- Vulnerability: Hệ thống phân quyền kém (ai cũng có thể sửa dữ liệu)
                 Không có cơ chế kiểm tra/ghi log thay đổi
                 Thiếu xác thực mạnh (mật khẩu yếu, không có xác thực 2 lớp)
- Mitigation: 
    + Áp dụng phân quyền truy cập chặt chẽ (Role-Based Access Control)
    + Ghi log và theo dõi mọi thay đổi dữ liệu
    + Sử dụng xác thực mạnh (2FA, mật khẩu mạnh)
    + Kiểm tra dữ liệu đầu vào và sử dụng cơ chế kiểm tra toàn vẹn (hash, checksum)
### 4. Kết luận ngắn
(4-6 dòng: em học được gì từ bài lab này, phần nào khó nhất, điều gì cần chú ý khi phân tích một sự cố an toàn thông tin.)
<<<<<<< HEAD
- Qua bài lab này, em hiểu rõ hơn về ba yếu tố quan trọng trong an toàn thông tin là Confidentiality, Integrity và Availability. Em cũng học được cách xác định tài sản cần bảo vệ và phân tích một sự cố dựa trên threat, vulnerability và mitigation. Phần khó nhất là phân biệt rõ giữa các yếu tố trong CIA vì đôi khi chúng liên quan đến nhau. Khi phân tích sự cố, cần xác định đúng mục tiêu bị ảnh hưởng và nguyên nhân gốc rễ. Điều quan trọng là phải đề xuất biện pháp phòng chống phù hợp và thực tế.
=======
- Qua bài lab này, em hiểu rõ hơn về ba yếu tố quan trọng trong an toàn thông tin là Confidentiality, Integrity và Availability. Em cũng học được cách xác định tài sản cần bảo vệ và phân tích một sự cố dựa trên threat, vulnerability và mitigation. Phần khó nhất là phân biệt rõ giữa các yếu tố trong CIA vì đôi khi chúng liên quan đến nhau. Khi phân tích sự cố, cần xác định đúng mục tiêu bị ảnh hưởng và nguyên nhân gốc rễ. Điều quan trọng là phải đề xuất biện pháp phòng chống phù hợp và thực tế.
>>>>>>> da02069 (Complete Lab 1 answers)
