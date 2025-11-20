## Tại sao cần môi trường phát triển React?

## Câu hỏi đặt ra

Tại sao cần môi trường CodeSandbox hoặc dự án cục bộ được tạo bằng các công cụ bổ sung như Vite nếu chỉ muốn viết code React? Tại sao không thể chỉ tạo một file HTML và một file JavaScript, tham chiếu script file từ trong HTML file, rồi đặt React code vào script file đó?[react+2](https://react.dev/learn/creating-a-react-app)​

## Lý do 1: JSX không hoạt động trong trình duyệt

## Cú pháp JSX

- Khi viết React code, bạn sẽ sử dụng tính năng đặc biệt **HTML trong JavaScript** (HTML in JavaScript) đã được giới thiệu trước đó trong section này[code-b+1](https://code-b.dev/blog/set-up-react-development-environment)​
    
- Cú pháp này được gọi là **JSX**[geeksforgeeks+2](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​
    
- Sẽ học thêm về JSX trong suốt khóa học[react+1](https://react.dev/learn/creating-a-react-app)​
    

## Vấn đề chính

- **Điều quan trọng cần hiểu**: cú pháp đặc biệt này, mà bạn sẽ sử dụng liên tục trong các dự án React, **không hoạt động trong trình duyệt** (doesn't work in the browser)[code-b+1](https://code-b.dev/blog/set-up-react-development-environment)​
    
- Đây tất nhiên là một vấn đề khá lớn (rather big problem)[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​
    
- Trình duyệt không hỗ trợ JSX một cách tự nhiên (natively)[code-b](https://code-b.dev/blog/set-up-react-development-environment)​
    

## Giải pháp

- Do đó, code bạn viết **phải được chuyển đổi** (must be transformed) thành code có thể chạy trong trình duyệt[react+2](https://react.dev/learn/creating-a-react-app)​
    
- Babel là công cụ thiết yếu để chuyển đổi cú pháp JSX (không được trình duyệt hỗ trợ tự nhiên) thành JavaScript thông thường, giúp render React components một cách chính xác[code-b](https://code-b.dev/blog/set-up-react-development-environment)​
    

## Lý do 2: Tối ưu hóa code

Ngoài việc chuyển đổi JSX, còn cần tối ưu hóa code vì các lý do sau:

## Các kỹ thuật tối ưu hóa

- **Rút ngắn tên biến và hàm** (shorten variable and function names)[react+1](https://react.dev/learn/creating-a-react-app)​
    
- **Xóa khoảng trắng thừa** (remove excess white space)[react+1](https://react.dev/learn/creating-a-react-app)​
    
- Mục tiêu: làm cho code phải tải xuống bởi khách truy cập website **nhỏ nhất có thể** (as small as possible)[code-b+1](https://code-b.dev/blog/set-up-react-development-environment)​
    

## Lợi ích

- **Cải thiện hiệu suất** website (improve the performance of your website)[react+1](https://react.dev/learn/creating-a-react-app)​
    
- Giảm thời gian tải trang[code-b](https://code-b.dev/blog/set-up-react-development-environment)​
    
- Tăng trải nghiệm người dùng[react+1](https://react.dev/learn/creating-a-react-app)​
    

## Vai trò của công cụ build

## Công cụ như Vite

- Đây là lý do tại sao cần tạo dự án React bằng các công cụ bổ sung như Vite[geeksforgeeks+2](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​
    
- **Cuối cùng, chính các công cụ này** (it's then, in the end, those tools) thực hiện chuyển đổi code của bạn thành code có thể được thực thi hiệu quả trong trình duyệt[geeksforgeeks+2](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​
    

## Các chức năng chính

- **Biến đổi code** (transform code): chuyển JSX sang JavaScript thuần[geeksforgeeks+2](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​
    
- **Tối ưu hóa** (optimize): giảm kích thước file, loại bỏ code không dùng[code-b+1](https://code-b.dev/blog/set-up-react-development-environment)​
    
- **Bundle** (đóng gói): kết hợp nhiều file thành ít file hơn để tải nhanh hơn[code-b](https://code-b.dev/blog/set-up-react-development-environment)​
    
- **Hot Module Replacement (HMR)**: cập nhật tức thì khi code thay đổi mà không cần reload toàn bộ trang[digitalocean+1](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-react-project-with-vite)​
    

## Kết luận về cách thiết lập

## Không thể dùng cách đơn giản

- **Không thể** chỉ tạo một HTML file và script file cơ bản[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​
    
- Thay vào đó, **cần** các công cụ bổ sung này[geeksforgeeks+2](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​
    

## Nhưng không quá phức tạp

- **May mắn thay**, như đã thấy trong bài giảng trước, việc tạo dự án với các công cụ này khá đơn giản (pretty straightforward)[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​
    
- Đặc biệt nếu sử dụng môi trường CodeSandbox vì ở đó về cơ bản không phải làm gì cả[react+1](https://react.dev/learn/creating-a-react-app)​
    

## Hỗ trợ trong khóa học

## Starting projects được cung cấp

- Như đã đề cập trong bài giảng trước, trong suốt khóa học, ở tất cả các sections, giảng viên sẽ luôn cung cấp **starting projects** (dự án khởi đầu)[react+1](https://react.dev/learn/creating-a-react-app)​
    
- **Cả hai phiên bản**: CodeSandbox và local version[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​
    

## Lợi ích cho học viên

- Thực tế **không phải tạo bất kỳ dự án nào** (don't have to create any projects at all)[react+1](https://react.dev/learn/creating-a-react-app)​
    
- Thay vào đó có thể sử dụng các starting projects đó và làm việc trong đó[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​
    
- **Tập trung vào** việc học và viết React code (focus on learning and writing React code)[code-b+2](https://code-b.dev/blog/set-up-react-development-environment)​
    

## Tóm tắt các yêu cầu môi trường

|Yêu cầu|Mục đích|
|---|---|
|Node.js|Chạy JavaScript code ngoài trình duyệt, cần cho các công cụ build [geeksforgeeks+3](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​|
|npm/Yarn|Quản lý packages và dependencies [geeksforgeeks+2](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​|
|Build tool (Vite/CRA)|Chuyển đổi JSX, tối ưu hóa code, bundle files [react+2](https://react.dev/learn/creating-a-react-app)​|
|Babel|Chuyển đổi JSX thành JavaScript thông thường [code-b](https://code-b.dev/blog/set-up-react-development-environment)​|
|Code editor (VS Code)|Viết và chỉnh sửa code [code-b+1](https://code-b.dev/blog/set-up-react-development-environment)​|
|Development server|Xem preview và auto-reload khi code thay đổi [geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)​|

## Ghi chú thêm

- Webpack là một công cụ khác thường được sử dụng để tối ưu hóa ứng dụng, xử lý dependencies và assets để có hiệu suất tốt hơn[code-b+1](https://code-b.dev/blog/set-up-react-development-environment)​
    
- React 18 hỗ trợ các trình duyệt hiện đại, trình duyệt cũ có thể cần polyfills cho các tính năng như Promise, Symbol, và Object.assign[legacy.reactjs](https://legacy.reactjs.org/docs/javascript-environment-requirements.html)​
    
- Việc thiết lập môi trường phát triển đúng cách là bước quan trọng đầu tiên để bắt đầu với React một cách hiệu quả[globaltechcouncil+2](https://www.globaltechcouncil.org/react/how-to-set-up-your-react-development-environment/)​
    

1. [https://reactnative.dev/docs/set-up-your-environment](https://reactnative.dev/docs/set-up-your-environment)
2. [https://react.dev/learn/creating-a-react-app](https://react.dev/learn/creating-a-react-app)
3. [https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/](https://www.geeksforgeeks.org/reactjs/reactjs-environment-setup/)
4. [https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Frameworks_libraries/React_getting_started](https://developer.mozilla.org/en-US/docs/Learn_web_development/Core/Frameworks_libraries/React_getting_started)
5. [https://code-b.dev/blog/set-up-react-development-environment](https://code-b.dev/blog/set-up-react-development-environment)
6. [https://www.globaltechcouncil.org/react/how-to-set-up-your-react-development-environment/](https://www.globaltechcouncil.org/react/how-to-set-up-your-react-development-environment/)
7. [https://www.w3schools.com/react/react_getstarted.asp](https://www.w3schools.com/react/react_getstarted.asp)
8. [https://docureacten.github.io/Basic/1-1-Introduction%20to%20React%20and%20Setting%20Up%20Development%20Environment](https://docureacten.github.io/Basic/1-1-Introduction%20to%20React%20and%20Setting%20Up%20Development%20Environment)
9. [https://code.visualstudio.com/docs/nodejs/reactjs-tutorial](https://code.visualstudio.com/docs/nodejs/reactjs-tutorial)
10. [https://legacy.reactjs.org/docs/javascript-environment-requirements.html](https://legacy.reactjs.org/docs/javascript-environment-requirements.html)
11. [https://www.digitalocean.com/community/tutorials/how-to-set-up-a-react-project-with-vite](https://www.digitalocean.com/community/tutorials/how-to-set-up-a-react-project-with-vite)