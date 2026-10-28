# BÀI LÀM – HACKATHON 01

- **Mã đề:** 21
- **Họ tên:** Lê Quang Hào
- **Lớp:** CNTT1
- **Link repository:** 
- **Hệ điều hành (Windows/macOS):** 

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
mkdir docs,media,data,logs,backup   
ls -Force    
rm .\temp_293.tmp     
cp .\logo_qua_luu_niem.PNG .\backup
mv .\logo_qua_luu_niem.PNG .\media\  
cd logs 
ls
cd..
```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

 Directory: C:\Users\lequanghao\Downloads\starter-kit (4)\starter-kit\Qua Luu Niem Website FINAL


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/28/2026   8:14 AM                backup
d-----        10/28/2026   7:54 AM                data
d-----        10/28/2026   8:07 AM                docs
d-----        10/28/2026   9:05 AM                logs
d-----        10/28/2026   8:22 AM                media
------        10/27/2026   1:32 AM             74 .env
-a----        10/27/2026   1:32 AM           2224 bai_lam.md

```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell

Get-Content .\logs\gift.log | Select-String "ERROR" | Measure-Object | Select-Object -ExpandProperty Count
get-Content .\logs\auto_report.txt
```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text

```

## 4.4. Thao tác với tài liệu Markdown (README.md)

> README.md được chấm trực tiếp trên file `README.md` ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [x] Heading 1: tên dự án
- [x] Mô tả ngắn có cả **in đậm** và *in nghiêng*
- [x] Bảng `Thư mục | Nội dung`, ít nhất 3 dòng dữ liệu
- [x] Code block chứa lệnh PowerShell/Terminal liệt kê nội dung dự án
- [x ] Task list ít nhất 2 công việc, có ít nhất 1 mục đã hoàn thành
- [x ] Blockquote nhắc không upload `.env`

## 4.5. Chạy script auto_report (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
# Ghi lệnh và

```

### Kết quả hiển thị

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.6. Đếm số dòng lỗi

### Lệnh

```shell
Get-Content .\logs\gift.log | Select-String "ERROR" | Measure-Object | Select-Object -ExpandProperty Count

```

### Kết quả đếm (Windows: giá trị Count; macOS: con số in ra)

```text
7

```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
"=== TONG HOP LOG ===" | Set-Content .\logs\daily_report.txt
Get-Content .\logs\gift.log | Select-String "WARNING" | Add-Content .\logs\tong_hop.txt
(Get-Content .\logs\gift.log | Select-String "ERROR" | Measure-Object).Count | Add-Content .\logs\daily_report.txt
Get-Content .\logs\daily_report.txt
```

### Nội dung file logs/tong_hop.txt

```text
=== TONG HOP LOG ===
7
```

## 4.8. Excel

> Phần Excel được chấm trực tiếp trên file `data/don_qua_thang_12.xlsx`, không cần ghi vào đây.
