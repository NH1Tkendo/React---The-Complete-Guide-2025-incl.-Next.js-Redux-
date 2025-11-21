## Thiết lập môi trường dự án (Project Setup)

## Các phương pháp tiếp cận

Có hai cách để bắt đầu làm việc với dự án mẫu:

1. **Môi trường trực tuyến (CodeSandbox)**:
    
    - Sử dụng liên kết được cung cấp trong tài liệu khóa học.
        
    - **Ưu điểm**: Không cần cấu hình thủ công, hệ thống tự động cài đặt và chạy máy chủ.
        
2. **Môi trường cục bộ (Local Environment)**:
    
    - Tải xuống và giải nén tệp tin dự án đính kèm.
        
    - Mở thư mục bằng trình soạn thảo mã (ví dụ: Visual Studio Code).
        

## Hướng dẫn chạy dự án cục bộ (Local Setup)

Nếu chọn làm việc trên máy tính cá nhân, bạn cần thực hiện các bước sau trong **Terminal**:

## 1. Cài đặt thư viện phụ thuộc

- Chạy lệnh:
    
    bash
    
    `npm install`
    
- **Mục đích**: Tải và cài đặt các gói bên thứ ba cần thiết (thư viện React, công cụ build).
    
- **Lý do**: Mã React mặc định không thể chạy trực tiếp trên trình duyệt, cần các công cụ build để chuyển đổi.
    
- **Lưu ý**: Chỉ cần thực hiện lệnh này một lần duy nhất khi bắt đầu dự án.
    

## 2. Khởi chạy máy chủ phát triển (Development Server)

- Chạy lệnh:
    
    bash
    
    `npm run dev`
    
- **Chức năng**: Khởi động server và cung cấp địa chỉ localhost để xem trước ứng dụng.
    
- **Cơ chế hoạt động**: Quy trình này sẽ theo dõi (watch) mã nguồn và tự động tải lại trang web khi có thay đổi. Cần giữ cửa sổ Terminal này luôn hoạt động trong quá trình lập trình.
    

## 3. Quản lý Server

- **Dừng server**: Nhấn tổ hợp phím `Ctrl + C` trong Terminal.
    
- **Khởi động lại**: Chạy lại lệnh `npm run dev` khi muốn tiếp tục làm việc.