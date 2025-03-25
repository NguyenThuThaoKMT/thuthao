# thuthao
Bài tập 2 của sv: K225480106060- Nguyễn Thu Thảo- Hệ quản trị cơ sở dữ liệu
DEADLINE: 23H59 NGÀY 25/03/2025

ĐIỀU KIỆN: (ĐÃ LÀM XONG BÀI 1)
1. Đã cài đặt SQL Server 2022 Dev.
2. Đã cài đặt SQL Managerment Studio bản mới nhất.
3. Đã kết nối từ SQL Managerment Studio vào SQL Server.
4. Đã có tài khoản github, biết cách tạo repository(kho lưu trữ) cho phép truy cập public.

BÀI TOÁN:
- Tạo csdl quan hệ với tên QLSV gồm các bảng sau:
  + SinhVien(#masv,hoten,NgaySinh)
  + Lop(#maLop,tenLop)
  + GVCN(#@maLop,#@magv,#HK)
  + LopSV(#@maLop,#@maSV,ChucVu)
  + GiaoVien(#magv,hoten,NgaySinh,@maBM)
  + BoMon(#MaBM,tenBM,@maKhoa)
  + Khoa(#maKhoa,tenKhoa)
  + MonHoc(#mamon,Tenmon,STC)
  + LopHP(#maLopHP,TenLopHP,HK,@maMon,@maGV)
  + DKMH(#@maLopHP,#@maSV,DiemTP,DiemThi,PhanTramThi)

YÊU CẦU:
1. Thực hiện các hành động sau trên giao diện đồ hoạ để tạo cơ sở dữ liệu cho bài toán:
  + Tạo database mới, mô tả các tham số(nếu có) trong quá trình.
  + Tạo các bảng dữ liệu với các trường như mô tả, chọn kiểu dữ liệu phù hợp với thực tế (tự tìm hiểu)
  + Mỗi bảng cần thiết lập PK, FK(s) và CK(s) nếu cần thiết. (chú ý dấu # và @: # là chỉ PK, @ chỉ FK)
2. Chuyển các thao tác đồ hoạ trên thành lệnh SQL tương đương. lưu tất cả các lệnh SQL trong file: Script_DML.sql

Bước 1: Đăng nhập vào tài khoản SQL Server
![image](https://github.com/user-attachments/assets/9e312a7d-f4f4-453c-a4c4-4a2aad8c1666)
Bước 2: Tạo database
![image](https://github.com/user-attachments/assets/a4c3d273-8f53-475b-8192-87dbe6184b78)
![image](https://github.com/user-attachments/assets/9b39a6c6-3492-4e8c-87a2-580baaf00d9c)
Bước 3: Tạo bảng
![image](https://github.com/user-attachments/assets/eea88d91-fd4f-46ae-ac12-32cfd4b77c55)
![image](https://github.com/user-attachments/assets/8c28c038-bad5-4ab4-8d05-fad4eb54f780)
![image](https://github.com/user-attachments/assets/91d0cc73-40e3-4124-8c55-e4c51ca937e2)
![image](https://github.com/user-attachments/assets/5fafcb39-4af8-40d5-97d6-913a49e6265d)
![image](https://github.com/user-attachments/assets/f0f920bc-a587-42b8-960d-0fc698b28abf)
![image](https://github.com/user-attachments/assets/bf793b53-519b-4d6a-af64-7875550594a6)
![image](https://github.com/user-attachments/assets/f0d56e17-d4f4-46bd-bb5f-561bdc6fe7ad)
![image](https://github.com/user-attachments/assets/549130e6-89e2-4f6e-a441-50bc7e90cbbf)
![image](https://github.com/user-attachments/assets/06e1d12f-120a-4fb8-820e-b3b1abb33dfa)
![image](https://github.com/user-attachments/assets/da40ccc8-0df2-4c16-ab22-36ef7bfa3e43)
![image](https://github.com/user-attachments/assets/085dcdbf-ba91-4b97-ae12-1f24fa5870de)
Bước 4: Tạo Check Constraints
![image](https://github.com/user-attachments/assets/d6508a5f-143a-43df-9d34-d8272e7b6403)
![image](https://github.com/user-attachments/assets/9c5ad45a-1460-402e-8a7f-643e359c8d12)
![image](https://github.com/user-attachments/assets/99aff209-6012-42fa-86e1-3536dbb060a0)
Bước 5: Đặt khóa chính
![image](https://github.com/user-attachments/assets/b3bc660b-5e28-466a-a17e-594474d0fb9b)
![image](https://github.com/user-attachments/assets/a4d550dc-392a-4e2e-8316-fdbad7d60513)
Bước 6: Đặt khóa ngoại
![image](https://github.com/user-attachments/assets/a7332fd7-0ff4-4bea-a407-8e0c47f36520)
![image](https://github.com/user-attachments/assets/b494bbb4-4b38-44be-a0c4-db4f5dc09ca2)
Bước 7: Chuyển từ thao tác đồ họa sang lệnh SQL
![image](https://github.com/user-attachments/assets/178891d2-2806-4c83-8dda-dd5bf7be2de4)
![image](https://github.com/user-attachments/assets/72b14b65-0def-4cea-9d9a-9c99738cfcec)
![image](https://github.com/user-attachments/assets/ec8d2375-5bfa-4d5c-a22f-d3c17e3f2397)
![image](https://github.com/user-attachments/assets/5426b4b1-0208-4331-809b-deaeac4ad9b1)
![image](https://github.com/user-attachments/assets/194f2f3c-d38c-40ae-99ce-a03d166cb6ab)
![image](https://github.com/user-attachments/assets/7994a0c6-dced-4e8b-bc99-fccda367502b)
![image](https://github.com/user-attachments/assets/24b92140-272d-466f-9861-7636b9aacc20)
![image](https://github.com/user-attachments/assets/9932ab0b-2cb7-40bf-b480-894d8d834b30)
![image](https://github.com/user-attachments/assets/abda6dab-1cb5-4af2-9b1f-1556c3e2f27e)
