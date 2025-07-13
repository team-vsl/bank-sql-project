# Banking SQL Sample Project

## 📘 Mô tả
Thiết lập một database mẫu từ dữ liệu marketing ngân hàng trên Kaggle. Bao gồm:
- Tạo database `bank_marketing`
- Tạo bảng `bank_data`
- Chèn 4521 dòng dữ liệu thực tế (Lý do em chèn thẳng trực tiếp nội dung CSV thành các câu lệnh vì em muốn tối ưu hóa việc import file CSV trong SSMS do nó chậm/lỗi nên trong SQL e sử dụng câu lệnh INSERT INTO để chèn dữ liệu luôn trong script SQL)

## 🗃️ Cấu trúc thư mục
- `data/bank.csv`: Dữ liệu nguồn gốc (Kaggle)
- `scripts/import_full_data.sql`: Script tạo database, table, insert dữ liệu
- `README.md`: Tài liệu hướng dẫn

## ▶️ Hướng dẫn chạy
1. Mở SQL Server Management Studio (SSMS)
2. Mở file `scripts/import_full_data.sql`
3. Nhấn **F5** hoặc **Excute** để thực thi
4. Kiểm tra dữ liệu:
   ```sql
   SELECT COUNT(*) FROM bank_data;
   SELECT TOP 10 * FROM bank_data;
