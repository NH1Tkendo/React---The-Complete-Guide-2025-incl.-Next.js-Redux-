## Cấu trúc tệp và Cú pháp JSX

## Phân tích luồng dữ liệu trong dự án

- **`index.html`**: Tệp này khá trống và không chứa nội dung hiển thị thực tế (như hình ảnh, tiêu đề).
    
    - Vai trò: Chỉ đóng vai trò là điểm nạp (entry point) và tải tệp JavaScript `index.jsx`.
        
    - Cơ chế: React chịu trách nhiệm "kết xuất" (rendering) nội dung lên màn hình thông qua JavaScript thay vì HTML thuần túy.
        
- **`src/index.jsx`**: Tệp nhập (entry file) của ứng dụng React, nó thực hiện việc import các thành phần từ `App.jsx`.
    
- **`src/App.jsx`**: Chứa mã nguồn định nghĩa giao diện người dùng (markup) thực tế mà ta nhìn thấy trên màn hình.
    

## JSX (JavaScript Syntax Extension)

- **Khái niệm**: Là cú pháp mở rộng của JavaScript cho phép viết mã đánh dấu HTML (HTML markup) ngay bên trong các tệp JavaScript.
    
- **Đuôi mở rộng**: Các tệp sử dụng cú pháp này thường có đuôi `.jsx`.
    
- **Khả năng tương thích**: Trình duyệt web (Browsers) **không hỗ trợ** JSX trực tiếp.
    
- **Cơ chế hoạt động**: Máy chủ phát triển (Development server) sẽ âm thầm chuyển đổi mã JSX thành mã JavaScript tiêu chuẩn mà trình duyệt có thể hiểu được trước khi tải trang.
    

## Quy tắc tạo React Component

Trong React, một **Thành phần (Component)** thực chất chỉ là một hàm JavaScript (JavaScript function). Tuy nhiên, để React nhận diện đúng là một Component, hàm này phải tuân thủ 2 quy tắc quan trọng:

1. **Quy tắc đặt tên**: Tên hàm **phải bắt đầu bằng chữ cái in hoa** (Uppercase character).
    
    - Ví dụ: `App`, `Header`, `UserCard`.
        
2. **Giá trị trả về**: Hàm bắt buộc phải **trả về (return)** một giá trị có thể hiển thị được (renderable value), thường là mã JSX/HTML mô tả giao diện.
![[React-Component.png]]

javascript

`// Ví dụ một React Component hợp lệ function App() {   return (    <div>      <h1>Hello World</h1>    </div>  ); }`