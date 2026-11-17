# Website bán xe máy Honda

Đây là bộ khung ban đầu cho một website bán xe máy Honda. Dự án hiện chưa có mã nguồn ứng dụng hoặc chức năng hoàn chỉnh; các thư mục đang được chuẩn bị để phát triển tiếp.

## Cấu trúc dự án

```text
.
├── database/                  # Dự kiến lưu các tệp liên quan đến dữ liệu
├── docker/
│   └── php/
│       └── Dockerfile          # Vị trí dự kiến cấu hình môi trường PHP
├── public/
│   ├── admin/                  # Khu vực quản trị
│   ├── api/                    # Khu vực API
│   └── upload/
│       └── product/            # Hình ảnh sản phẩm được tải lên
├── src/
│   ├── config/                 # Cấu hình ứng dụng
│   └── includes/
│       ├── admin/              # Thành phần dùng cho trang quản trị
│       └── frontend/           # Thành phần dùng cho giao diện khách hàng
├── .env.example                # Mẫu biến môi trường
├── compose.yml                 # Vị trí dự kiến cấu hình Docker Compose
└── README.md
```

## Tình trạng hiện tại

Các thư mục và tệp cấu hình mới được tạo làm khung ban đầu. Chưa có hướng dẫn cài đặt hoặc chạy ứng dụng vì mã nguồn PHP, cấu hình Docker và các thiết lập môi trường chưa được bổ sung.

## Phát triển tiếp

Khi bắt đầu triển khai, hãy bổ sung cấu hình môi trường và Docker, sau đó xây dựng các phần giao diện, API, quản trị và dữ liệu tương ứng.
