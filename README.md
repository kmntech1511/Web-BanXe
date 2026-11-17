# Xây dựng website bán xe Honda

## Thông tin đề tài

- **Tên đề tài:** Xây dựng website bán xe Honda
- **Mục tiêu:** Xây dựng nền tảng website giới thiệu và bán xe Honda.

## Nhóm sinh viên thực hiện

| STT | Họ tên | Mã số sinh viên | Mã lớp |
|---:|---|---:|---|
| 1 | Thạch Ngọc Phú | 110123039 | Chưa cung cấp |
| 2 | Trương Quang Khải | 110123019 | Chưa cung cấp |
| 3 | Ngô Thanh Trà | 110123189 | Chưa cung cấp |

## Công nghệ sử dụng

- **PHP** — phát triển ứng dụng phía máy chủ.
- **SQL Server** — hệ quản trị cơ sở dữ liệu.
- **Docker** — đóng gói và chạy các dịch vụ của dự án.

## Cấu trúc dự án

```text
.
├── database/                  # Dự kiến lưu các tệp liên quan đến dữ liệu
├── docker/
│   └── php/
│       └── Dockerfile          # Vị trí cấu hình môi trường PHP
├── public/
│   ├── admin/                  # Khu vực quản trị
│   ├── api/                    # Khu vực API
│   └── upload/
│       └── product/            # Hình ảnh sản phẩm được tải lên
├── src/
│   ├── config/                 # Cấu hình ứng dụng
│   └── includes/
│       ├── admin/              # Thành phần trang quản trị
│       └── frontend/           # Thành phần giao diện khách hàng
├── .env.example                # Mẫu biến môi trường
├── compose.yml                 # Cấu hình Docker Compose
└── README.md
```

## Cài đặt và triển khai

### Yêu cầu

- Git
- Docker và Docker Compose
- SQL Server (có thể chạy trong Docker khi cấu hình dịch vụ cơ sở dữ liệu)

### Lấy mã nguồn

```bash
git clone https://github.com/kmntech1511/Web-BanXe.git
cd Web-BanXe
```

### Cấu hình và khởi chạy

Khi các cấu hình của dự án đã được bổ sung, quy trình triển khai dự kiến:

1. Tạo file `.env` từ `.env.example` và điền các thông tin kết nối cơ sở dữ liệu theo cấu hình của ứng dụng.
2. Cấu hình dịch vụ PHP và SQL Server trong `compose.yml`.
3. Khởi chạy các dịch vụ:

   ```bash
   docker compose up --build -d
   ```

4. Truy cập địa chỉ web được ánh xạ trong cấu hình Docker Compose.
5. Dừng các dịch vụ khi không sử dụng:

   ```bash
   docker compose down
   ```

> **Lưu ý:** Dự án hiện mới có cấu trúc thư mục ban đầu. `compose.yml`, `docker/php/Dockerfile` và `.env.example` đang trống; mã nguồn ứng dụng, cấu hình kết nối SQL Server và hướng dẫn truy cập chưa được triển khai. Vì vậy, các bước khởi chạy Docker ở trên là quy trình dự kiến và hiện chưa thể chạy thành công. Cần bổ sung các cấu hình và mã nguồn tương ứng trước khi triển khai.
