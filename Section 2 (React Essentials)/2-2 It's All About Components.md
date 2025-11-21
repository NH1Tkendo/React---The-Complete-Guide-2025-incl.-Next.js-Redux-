## Thành phần (Components) trong React

## Khái niệm cốt lõi

- **Tầm quan trọng**: Đây là khái niệm cốt lõi nhất mà mọi ứng dụng React đều cần, bất kể độ phức tạp.
    
- **Định nghĩa**: Thành phần (Components) là các khối xây dựng có khả năng tái sử dụng (reusable building blocks) do lập trình viên tạo ra, sau đó kết hợp lại để xây dựng nên toàn bộ giao diện người dùng (User Interface - UI).
    
- **Bản chất**: Một Component gói gọn mã HTML, CSS (nếu có) và logic JavaScript liên quan để định nghĩa và điều khiển một phần cụ thể của UI.
    
- **Quy mô**: Kích thước của một component (lớn hay nhỏ) phụ thuộc vào quyết định của lập trình viên.
    

## Tại sao nên sử dụng Components?

Việc chia nhỏ UI thành các Components mang lại nhiều lợi ích vượt trội so với cách viết code truyền thống:

## 1. Khả năng tái sử dụng (Reusability)

- Cho phép sử dụng lại cùng một đoạn mã (HTML markup, style, logic) ở nhiều vị trí khác nhau trong UI.
    
- **Ví dụ**: Trong dự án demo, component "Core Concept" được sử dụng 4 lần, chỉ thay đổi dữ liệu cấu hình đầu vào.
    

## 2. Quản lý mã nguồn và Bảo trì (Maintainability)

- Giúp chia nhỏ các giao diện phức tạp thành các phần nhỏ dễ quản lý hơn.
    
- Tránh việc phải làm việc với các tệp HTML khổng lồ, khó điều hướng.
    
- Khi cần thay đổi, chỉ cần sửa tại một nơi (trong component) thay vì sửa ở nhiều chỗ rải rác, giúp giảm thiểu lỗi.
    

## 3. Tổ chức mã (Code Organization)

- **Vấn đề cũ**: Trước đây, markup nằm trong file HTML, logic nằm trong file JS. Khi sửa logic, phải chuyển qua lại giữa các file và dễ quên cập nhật HTML tương ứng, gây lỗi.
    
- **Giải pháp React**: Các mã liên quan chặt chẽ được lưu trữ cùng nhau trong một Component, giúp đơn giản hóa quy trình phát triển.
    

## 4. Phân tách mối quan tâm (Separation of Concerns)

- Mỗi component đảm nhiệm một vai trò riêng biệt (ví dụ: component chuyên xuất thông tin, component chuyên xử lý nhập liệu).
    
- Giúp cấu trúc dự án rõ ràng và hỗ trợ tốt cho làm việc nhóm (mỗi lập trình viên phụ trách một nhóm tính năng).
    

## Ghi chú thêm

- Tư duy "Giao diện là tập hợp các Components" không chỉ độc quyền ở React.
    
- Nó xuất hiện trong hầu hết các framework hiện đại khác như **Angular**, **Vue**, **Svelte**, và cả trong phát triển ứng dụng di động như **Flutter**.`