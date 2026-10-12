# AI Prompt Log

### Prompt 1 (Tìm hiểu CSS Grid & Responsive Gallery)

- **User Prompt:** "Làm thế nào để tạo bố cục ảnh khảm (Mosaic Gallery) với 1 ảnh lớn bên trái chiếm 2 hàng và 2 ảnh nhỏ xếp dọc bên phải bằng CSS Grid? Khi lên mobile thì chuyển thành 1 cột như thế nào?"
- **AI Response:** Hướng dẫn tạo grid container với `grid-template-columns: 2fr 1fr`, đặt `grid-row: span 2` cho ảnh chính. Cung cấp media query `max-width: 768px` để chuyển `grid-template-columns` về `1fr`.

### Prompt 2 (Khai thác Bootstrap Flex Utilities)

- **User Prompt:** "Có thể dùng các class có sẵn của Bootstrap 5 để căn giữa theo chiều dọc avatar, tên tác giả và nhóm nút chia sẻ trên cùng một dòng mà không cần viết CSS thuần không?"
- **AI Response:** Gợi ý sử dụng các class utility: `d-flex`, `align-items-center`, `justify-content-between`, `gap-3`, kết hợp `flex-wrap` để tự động xuống dòng khi màn hình quá nhỏ.

### Prompt 3 (Chống đè ảnh bằng object-fit)

- **User Prompt:** "Khi dùng CSS Grid cho khối ảnh có kích thước cố định, làm sao để ảnh không bị méo tỉ lệ (stretch/distort)?"
- **AI Response:** Giải thích thuộc tính `object-fit: cover` kết hợp `width: 100%` và `height: 100%` để ảnh tự co gián đẹp mắt mà không bị biến dạng.
