# Báo Cáo Phân Tích Kỹ Thuật Dàn Trang (Layout Refactoring Report)

### 1. Tác hại của `position: absolute` và `float` đối với Responsive Design

- **Triệt tiêu chiều cao (Height Collapse):** `position: absolute` đưa phần tử ra khỏi luồng hiển thị bình thường (Normal Flow). Phần tử cha không thể tính toán được chiều cao của các phần tử con bên trong, dẫn đến chiều cao của container bị đưa về `0`, làm cho nội dung văn bản bên dưới bị kéo đẩy đè bẹp lên ảnh.
- **Tính toán cứng nhắc:** Thuộc tính `float` yêu cầu xử lý chống vỡ dòng (Clearfix) phức tạp và phải tính toán phần trăm width thủ công (`width: 23%`). Khi màn hình thay đổi kích thước, phần thừa dư ra dù chỉ $1\text{px}$ cũng khiến thẻ bị rớt dòng méo mó.

### 2. CSS Grid - Giải pháp cứu cánh cho Mosaic Gallery

- CSS Grid cho phép định nghĩa không gian 2 chiều (hàng và cột) cùng lúc. Thuộc tính `grid-row: span 2` giúp ảnh chính tự động chiếm 2 hàng mà không làm đứt gãy luồng văn bản bên dưới.
- Khi chuyển sang màn hình di động, chỉ cần điều chỉnh `grid-template-columns: 1fr` trong `@media`, toàn bộ ảnh sẽ xếp chồng dọc gọn gàng mà không đè lên bất kỳ nội dung nào.
