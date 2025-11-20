## So sánh React và JavaScript thuần

## Giới thiệu bài học

Bài học này so sánh hai cách xây dựng cùng một ứng dụng web: sử dụng **React** và sử dụng **JavaScript thuần** (vanilla JavaScript). Mục đích là chứng minh rằng React cung cấp mô hình tư duy đơn giản hơn (simpler mental model) và cách thức dễ dàng hơn để xây dựng ứng dụng web phức tạp.[reddit+2](https://www.reddit.com/r/webdev/comments/atgke2/react_vs_vanilla_js_when_to_use_each_of_them/)​

## Demo ứng dụng mẫu

- Hai ứng dụng web cơ bản có cùng chức năng: các tab có thể click để thay đổi nội dung hiển thị bên dưới[asynclabs+1](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
    
- Một phiên bản được xây dựng bằng React, phiên bản còn lại bằng vanilla JavaScript[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
    
- Demo được xây dựng trên **CodeSandbox** - môi trường phát triển code trên trình duyệt (in-browser cloud-based code editor), cho phép làm việc với React mà không cần cài đặt phần mềm trên máy cục bộ[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
    
- Các link đến demo được đính kèm trong bài giảng để học viên có thể thử nghiệm và chỉnh sửa code[distantjob](https://distantjob.com/blog/vanillajs-vs-react/)​
    

## Phiên bản Vanilla JavaScript

## Cấu trúc file

- **index.html**: chứa các phần tử HTML hiển thị phần lớn trang web[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
    
- **index.js**: chịu trách nhiệm lấy các button, thêm click listeners, và cập nhật UI khi button được click[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
    

## Cách hoạt động

- Thiết lập click listeners cho các button[asynclabs+1](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
    
- Khi button được click, một function được thực thi để:
    
    - Xóa CSS class `active` khỏi tất cả button, sau đó thêm vào button vừa được click (event target)[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
        
    - Hiển thị nội dung bên dưới button bằng cách load dữ liệu từ mảng `content` (chứa các mảng lồng nhau bên trong)[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
        
    - Truyền nội dung đã chọn vào function `displayContent`, trong đó:
        
        - Tạo một chuỗi string chứa các phần tử `<li>` dưới dạng text[asynclabs](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
            
        - Tạo phần tử `<ul>` (unordered list)[flatlogic](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
            
        - Xóa nội dung cũ trong vùng `tabContent`[distantjob](https://distantjob.com/blog/vanillajs-vs-react/)​
            
        - Thêm chuỗi list content vào list dưới dạng `innerHTML`[dev](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
            
        - Append list đó vào `tabContent` để hiển thị lên màn hình[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
            

## Nhận xét

- Đây là ứng dụng khá đơn giản nhưng vẫn cần **khá nhiều code** để hoạt động đúng cách[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
    
- Có thể viết code theo nhiều cách khác nhau, nhưng cách tiếp cận được chọn là dễ hiểu và dễ theo dõi nhất[asynclabs+1](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
    

## Phiên bản React

## Cấu trúc file

- **index.html** (trong thư mục public): khá trống rỗng, phần body chỉ chứa một `<div>` với id `root`, không có nội dung bên trong[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
    
- **index.js**: điểm bắt đầu của React, chọn div có id `root` và React tiếp quản div đó để kiểm soát nội dung[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
    
- **app.js**: chứa code quan trọng nhất[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
    

## Đặc điểm code React

## Kết hợp HTML và JavaScript

- Trong function `App`, có đoạn HTML code xuất hiện bên trong - điều này không phải là tính năng mặc định của JavaScript[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
    
- Thông thường, việc thêm HTML vào file JavaScript sẽ gây lỗi[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
    
- Trong React project, điều này hoạt động nhờ cách project được thiết lập từ đầu[asynclabs+1](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
    
- Đây là một trong những **tính năng chính của React**: có thể kết hợp (blend) HTML và JavaScript code[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
    

## Nội dung trong app.js

- Tất cả HTML code với header, buttons, và unordered list (trước đây nằm trong index.html của vanilla version) giờ đều nằm trong một file JavaScript duy nhất[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
    
- Các JavaScript instructions (chỉ thị) từ vanilla version **không còn xuất hiện** trong React version[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
    
- Thay vào đó, chỉ có HTML code với các phần tử động (dynamic elements) được kết hợp vào HTML[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
    

## Cách React xử lý tương tác

- Code định nghĩa các **states** (trạng thái) khác nhau của các phần tử HTML[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
    
- Ví dụ: button sẽ nhận CSS class `active` nếu điều kiện `activeContentIndex === 0` được đáp ứng, ngược lại sẽ nhận empty class (không có CSS class)[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
    
- Các button khác có điều kiện tương tự[asynclabs+1](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
    

## Hiển thị nội dung tab

- Có unordered list dưới dạng HTML trong JavaScript[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
    
- Nội dung động được load từ mảng lồng nhau (nested array) trong mảng `content`, tùy thuộc vào button nào được click[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
    
- Phụ thuộc vào biến `activeContentIndex`[asynclabs+1](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
    
- Tất cả các string items trong mảng lồng đó được tự động chuyển thành list items (`<li>`) - điều không hoạt động trong vanilla JavaScript nhưng hoạt động trong React[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
    
- Các list items được thêm vào unordered list[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
    

## useState Hook

- `activeContentIndex` giống như một biến (variable), được tạo và kiểm soát bởi tính năng React gọi là **useState**[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
    
- useState tạo ra một **biến động do React quản lý** (dynamic React-managed variable) có thể được cập nhật thông qua function `setActiveContentIndex`[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
    
- Function này được sử dụng cho các click listeners, được thêm trực tiếp vào buttons ngay trong HTML code[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
    

## Cơ chế cập nhật UI của React

- Biến `activeContentIndex` thay đổi và ảnh hưởng đến cách UI hiện tại trông như thế nào[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
    
- React **theo dõi biến này** (watches this variable)[asynclabs+1](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
    
- Mỗi khi biến thay đổi, React:
    
    - Kiểm tra HTML code[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
        
    - Kiểm tra tất cả các điều kiện (conditions)[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
        
    - Thực thi code và xem liệu có dẫn đến UI khác so với UI đã render trước đó không[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
        
- Nếu cần UI khác, React tự động cập nhật UI[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
    
- React thực hiện tất cả những việc này **tự động**[asynclabs+1](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
    

## Declarative vs Imperative Code

## Declarative Code (React)

- Khi làm việc với React, bạn viết **code declarative** (mã khai báo)[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
    
- **Định nghĩa**: bạn định nghĩa trạng thái UI mục tiêu (target UI state hoặc states), không phải các bước cần thiết để đến đó[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
    
- React sẽ tự tìm ra cách để đạt được mục tiêu và thực hiện các bước cần thiết[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
    
- Đây là khái niệm quan trọng cần hiểu và ghi nhớ về cách React hoạt động[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
    

## Imperative Code (Vanilla JavaScript)

- Khi viết vanilla JavaScript, bạn viết **code imperative** (mã mệnh lệnh), không phải declarative[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
    
- **Định nghĩa**: bạn không định nghĩa mục tiêu mà thay vào đó định nghĩa từng bước cần thiết để đến đó[asynclabs+1](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
    
- Trong ví dụ demo, điều này **rõ ràng rườm rà và khó khăn hơn nhiều**[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
    
- Mặc dù ví dụ rất cơ bản và đơn giản, vẫn phải tìm ra rất nhiều bước để đạt được hành vi mong muốn[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
    
- **Dễ quên một bước** hoặc tạo ra lỗi trong quá trình[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
    
- Việc cập nhật code và xử lý button thứ 4 cũng có thể trở nên **phức tạp không cần thiết**[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
    

## So sánh tổng quan

## Vanilla JavaScript

- **Ưu điểm**: kiểm soát hoàn toàn, nhẹ, không có dependencies[asynclabs+2](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
    
- **Nhược điểm**:
    
    - Phải viết từng bước chi tiết (step-by-step instructions)[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
        
    - Cồng kềnh và khó khăn ngay cả với ví dụ đơn giản[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
        
    - Dễ gây lỗi[asynclabs+1](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
        
    - Khó bảo trì khi dự án phát triển[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
        

## React

- **Ưu điểm**:
    
    - Code gọn gàng (lean), ít code hơn cần viết[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
        
    - React tự động xử lý việc cập nhật UI[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
        
    - React sử dụng JavaScript ngầm để cập nhật UI[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
        
    - Chỉ cần định nghĩa điều kiện (conditions), trạng thái mục tiêu (target states) và khi nào states thay đổi[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
        
    - React sẽ lo phần còn lại[asynclabs+1](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)​
        
- **Kết luận**: React cung cấp cách tiếp cận tốt hơn để xây dựng ứng dụng phức tạp[distantjob+1](https://distantjob.com/blog/vanillajs-vs-react/)​
    

## Ghi chú thêm

- Yêu cầu kiến thức JavaScript cơ bản để hiểu code[dev+1](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)​
    
- Nếu gặp khó khăn hiểu code JavaScript, nên tham khảo thêm tài liệu JavaScript cơ bản hoặc phần JavaScript refresher trong khóa học[dhiwise+1](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)​
    
- Tất cả chi tiết về cách viết React code sẽ được học kỹ hơn trong các bài sau[flatlogic+1](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)​
    

1. [https://www.reddit.com/r/webdev/comments/atgke2/react_vs_vanilla_js_when_to_use_each_of_them/](https://www.reddit.com/r/webdev/comments/atgke2/react_vs_vanilla_js_when_to_use_each_of_them/)
2. [https://distantjob.com/blog/vanillajs-vs-react/](https://distantjob.com/blog/vanillajs-vs-react/)
3. [https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb](https://dev.to/purushoth_26/react-vs-vanilla-javascript-what-to-choose-in-2025-5ejb)
4. [https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/](https://www.asynclabs.co/blog/software-development/vanilla-javascript-vs-react-choosing-the-right-tool-for-web-development/)
5. [https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers](https://www.dhiwise.com/post/vanilla-javascript-vs-react-whats-right-for-developers)
6. [https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/](https://flatlogic.com/blog/vanilla-js-vs-react-js-featured-based-comparison-to-find-the-best-javascript-technology/)
7. [https://www.youtube.com/watch?v=dnHpcsiPINA](https://www.youtube.com/watch?v=dnHpcsiPINA)
8. [https://forum.freecodecamp.org/t/react-vs-vanilla-js/449908](https://forum.freecodecamp.org/t/react-vs-vanilla-js/449908)
9. [https://javascript.plainenglish.io/react-vs-vanilla-javascript-when-should-you-stop-using-frameworks-075cca68b475](https://javascript.plainenglish.io/react-vs-vanilla-javascript-when-should-you-stop-using-frameworks-075cca68b475)