## Bài tập thực hành đầu tiên với React

## Mục tiêu bài học

- Bắt tay vào làm việc thực tế (get hands dirty) và bắt đầu làm việc với ứng dụng React đầu tiên, mặc dù chưa biết nhiều về React[w3schools+1](https://www.w3schools.com/react/react_usestate.asp)​
    
- Áp dụng những kiến thức đã thấy từ các bài trước để giải quyết bài tập thực hành[legacy.reactjs+1](https://legacy.reactjs.org/docs/hooks-state.html)​
    

## Chuẩn bị bài tập

- Giảng viên cung cấp một **demo app mới đã cập nhật** thông qua link đính kèm trong bài giảng[w3schools+1](https://www.w3schools.com/react/react_usestate.asp)​
    
- Ứng dụng này được host trên CodeSandbox, tương tự như ví dụ trước[react+1](https://react.dev/reference/react/useState)​
    
- **Điểm khác biệt**: mảng `content` đã được cập nhật, có thêm một mảng lồng thứ tư (fourth nested array) bên trong[logrocket+1](https://blog.logrocket.com/guide-usestate-react/)​
    
- Mảng lồng thứ tư này sẽ quan trọng cho bài tập[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-usestate-hook/)​
    

## Yêu cầu bài tập

- **Nhiệm vụ**: Thêm một button thứ tư với bất kỳ text nào bạn chọn (không quan trọng)[react+1](https://react.dev/reference/react/useState)​
    
- **Hành vi mong đợi**: Khi button thứ tư được click, nội dung cho button này (entry thứ tư trong mảng `content`) phải được load và hiển thị lên màn hình[legacy.reactjs+1](https://legacy.reactjs.org/docs/hooks-state.html)​
    

## Độ khó của bài tập

- Thực hiện bài tập này sẽ **khó khăn** (challenging) vì học viên chưa thực sự biết React[logrocket+1](https://blog.logrocket.com/guide-usestate-react/)​
    
- Giảng viên khuyến khích học viên tạm dừng video và thử tự giải quyết trước khi xem lời giải[react+1](https://react.dev/reference/react/useState)​
    
- Nếu không giải được cũng **không sao** (no worries) vì mới chỉ bắt đầu và chưa học React đầy đủ[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-usestate-hook/)​
    

## Hướng dẫn giải bài tập

## Bước 1: Sử dụng phiên bản đã cập nhật

- Đảm bảo sử dụng phiên bản đã cập nhật từ link đính kèm, có entry bổ sung trong mảng[w3schools+1](https://www.w3schools.com/react/react_usestate.asp)​
    

## Bước 2: Thêm button mới

- Di chuyển xuống phần buttons trong menu[legacy.reactjs+1](https://legacy.reactjs.org/docs/hooks-state.html)​
    
- **Copy** một trong các button hiện có[logrocket+1](https://blog.logrocket.com/guide-usestate-react/)​
    
- **Paste** button đó vào trong menu, có thể ở cuối menu (vị trí không quan trọng)[react+1](https://react.dev/reference/react/useState)​
    
- Đặt text cho button, ví dụ: "React vs JS" (text tùy chọn)[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-usestate-hook/)​
    

## Bước 3: Phát hiện vấn đề

- Khi click button mới, xuất hiện **hành vi lạ** (strange behavior): button thứ 3 và thứ 4 đều active cùng lúc[w3schools+1](https://www.w3schools.com/react/react_usestate.asp)​
    
- Nội dung của button thứ 3 được load[legacy.reactjs+1](https://legacy.reactjs.org/docs/hooks-state.html)​
    
- **Nguyên nhân**: do copy button thứ 3 và giữ nguyên toàn bộ logic của button đó[logrocket+1](https://blog.logrocket.com/guide-usestate-react/)​
    

## Bước 4: Điều chỉnh logic

## Cập nhật click listener

- Trong function được thực thi khi click xảy ra, cần set `activeContentIndex` thành **3** để chọn item thứ tư trong mảng `content`[geeksforgeeks+2](https://www.geeksforgeeks.org/reactjs/reactjs-usestate-hook/)​
    
- **Lý do**: trong JavaScript, mảng bắt đầu với index 0, nên index 3 sẽ trỏ đến item thứ tư[legacy.reactjs+2](https://legacy.reactjs.org/docs/hooks-state.html)​
    
- Điều này đảm bảo ở phía dưới code sẽ sử dụng item thứ tư trong mảng thông qua index 3[w3schools+1](https://www.w3schools.com/react/react_usestate.asp)​
    

## Cập nhật điều kiện CSS class

- Trong điều kiện (condition), cần so sánh `activeContentIndex` với **3**[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-usestate-hook/)​
    
- Đảm bảo button này chỉ nhận CSS class `active` khi content index bằng 3[logrocket+1](https://blog.logrocket.com/guide-usestate-react/)​
    

## Bước 5: Hoàn thành

- Đó là **tất cả những gì cần làm**[react+1](https://react.dev/reference/react/useState)​
    
- Sau khi save, có thể reload (mặc dù không bắt buộc)[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-usestate-hook/)​
    
- Giờ có thể chọn button này và xem nội dung cho button, chỉ button này được active[w3schools+1](https://www.w3schools.com/react/react_usestate.asp)​
    
- Tất cả các button đều hoạt động đúng như mong đợi, bao gồm cả button thứ tư[legacy.reactjs+1](https://legacy.reactjs.org/docs/hooks-state.html)​
    

## Ý nghĩa bài tập

- Đã "làm bẩn tay" (got hands dirty) - bắt tay vào thực hành[logrocket+1](https://blog.logrocket.com/guide-usestate-react/)​
    
- Đã viết những dòng code React đầu tiên[react+1](https://react.dev/reference/react/useState)​
    
- Đã giải quyết bài tập thực hành[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-usestate-hook/)​
    

## Ghi chú quan trọng

- Nếu không tự giải được bài tập, điều đó **hoàn toàn bình thường** (absolutely fine) và **đúng như kỳ vọng** (absolutely to be expected)[w3schools+1](https://www.w3schools.com/react/react_usestate.asp)​
    
- Lý do: học viên chưa thực sự học React, giảng viên chưa dạy React[legacy.reactjs+1](https://legacy.reactjs.org/docs/hooks-state.html)​
    
- Chỉ mới được xem một ví dụ cơ bản đầu tiên[logrocket+1](https://blog.logrocket.com/guide-usestate-react/)​
    
- Khóa học sẽ dạy React từ nền tảng (from the ground up)[react+1](https://react.dev/reference/react/useState)​
    
- **Không cần lo lắng** nếu chưa tự làm được[geeksforgeeks+1](https://www.geeksforgeeks.org/reactjs/reactjs-usestate-hook/)​
    

## Kiến thức kỹ thuật liên quan

## Về useState Hook

- `useState` là React Hook cho phép thêm state vào functional components[w3schools+2](https://www.w3schools.com/react/react_usestate.asp)​
    
- Trả về một mảng gồm hai giá trị: state hiện tại và function để cập nhật state[kinsta+2](https://kinsta.com/blog/usestate-react/)​
    
- Cú pháp: `const [state, setState] = useState(initialState)`[kinsta+2](https://kinsta.com/blog/usestate-react/)​
    
- Khi state thay đổi, React tự động re-render component[strapi+2](https://strapi.io/blog/react-usestate-hook-guide-best-practices)​
    

1. [https://www.w3schools.com/react/react_usestate.asp](https://www.w3schools.com/react/react_usestate.asp)
2. [https://react.dev/reference/react/useState](https://react.dev/reference/react/useState)
3. [https://legacy.reactjs.org/docs/hooks-state.html](https://legacy.reactjs.org/docs/hooks-state.html)
4. [https://www.geeksforgeeks.org/reactjs/reactjs-usestate-hook/](https://www.geeksforgeeks.org/reactjs/reactjs-usestate-hook/)
5. [https://blog.logrocket.com/guide-usestate-react/](https://blog.logrocket.com/guide-usestate-react/)
6. [https://kinsta.com/blog/usestate-react/](https://kinsta.com/blog/usestate-react/)
7. [https://strapi.io/blog/react-usestate-hook-guide-best-practices](https://strapi.io/blog/react-usestate-hook-guide-best-practices)
8. [https://hygraph.com/blog/usestate-react](https://hygraph.com/blog/usestate-react)
9. [https://www.youtube.com/watch?v=SpDG283b4bw](https://www.youtube.com/watch?v=SpDG283b4bw)
10. [https://www.freecodecamp.org/news/introduction-to-react-hooks/](https://www.freecodecamp.org/news/introduction-to-react-hooks/)