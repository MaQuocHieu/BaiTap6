# Bài tập 6: Hệ quản trị CSDL
## Chủ đề: Câu lệnh Select
## Yêu cầu bài tập: 

1. Hãy nêu các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
2. dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)
3. nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
6. nhập sql để tìm xem có những sv nào trùng tên với em?
7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC)

##  Các Bước : import dữ liệu từ sv_tnut.sql vào SQL Server

1. Mở SQL Server Management Studio (SSMS).
2. Tạo một cơ sở dữ liệu mới 
3. Chọn cơ sở dữ liệu đó trong dropdown trên thanh công cụ SSMS.
4. Mở file sv_tnut.sql:
Vào File > Open > File..., chọn file .sql.
Hoặc kéo file vào SSMS.
5. Chạy script bằng cách bấm Execute (hoặc phím tắt F5).
6. Kiểm tra lại dữ liệu: Xem các bảng có được tạo và có dữ liệu chưa bằng

## 2 dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)
![Screenshot 2025-04-25 165219](https://github.com/user-attachments/assets/a9b265e6-3504-4a21-9016-c6577f492e8e)
 ## 3 nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
 ![Screenshot 2025-04-25 165237](https://github.com/user-attachments/assets/0b3f00a7-797e-4c39-a3e9-79edd7aa99d2)
 ### 4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
 ![Screenshot 2025-04-25 165317](https://github.com/user-attachments/assets/0fac8e36-fd71-4dc5-9573-ce060d3e05d6)
 ### 5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
![Screenshot 2025-04-25 165445](https://github.com/user-attachments/assets/19ec2ca6-c1fa-4694-90c7-466e6b6f24a0)
### 6. nhập sql để tìm xem có những sv nào trùng tên với em?
![Screenshot 2025-04-25 165543](https://github.com/user-attachments/assets/62198711-9620-4fe4-8dfe-2b7a6438a7b5)
### 7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
![Screenshot 2025-04-25 165643](https://github.com/user-attachments/assets/098866c0-4d4d-426c-b64b-45776d58063d)
### 8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
![Screenshot 2025-04-25 165954](https://github.com/user-attachments/assets/eadf9bbe-938a-4e66-9d17-0019d6c4e0be)
### 9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
![Screenshot 2025-04-25 170103](https://github.com/user-attachments/assets/7057b8e7-6286-4c27-a1c9-8af9f43eb88d)
### 10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC)
![Screenshot 2025-04-25 170344](https://github.com/user-attachments/assets/75a44bd9-3f15-4a1d-8e69-3f9973f4fc11)

 ## Vướng mắc chính:
1. Trong bảng SV không có cột gioitinh (giới tính).
2. Cần suy luận giới tính nữ dựa vào:
3. Họ đệm là Thị (rất phổ biến với nữ ở Việt Nam).
4 Hoặc tên gọi phổ biến của nữ.
 ## Chi tiết cách làm:
1. Xác định ngành KMT:
- Nhận thấy cột lop chứa mã lớp → dùng LIKE '%KMT%' để lọc lớp thuộc ngành KMT.
2. Xác định nữ:
- Truy vấn dựa vào họ đệm hodem LIKE N'%Thị%'.
- Ngoài ra, bổ sung thêm lọc theo những cái tên phổ biến của nữ như Mỹ, Tuyết, Thảo, Yến,...
3. Ghép điều kiện lại bằng OR:
- Dùng OR để mở rộng khả năng lọc nữ: ai có hodem chứa Thị hoặc ten nằm trong danh sách tên nữ thì đều được tính là nữ.



