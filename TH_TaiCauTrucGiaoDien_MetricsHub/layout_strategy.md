# Giải Trình Chiến Lược Dàn Trang (Layout Strategy)

**CSS Grid sinh ra để làm Layout tổng thể (2D), Flexbox sinh ra để làm Component chi tiết (1D):**

- **CSS Grid (Layout 2D):** Cho phép kiểm soát đồng thời cả hàng (Row) và cột (Column). Rất phù hợp làm khung giao diện tổng thể hoặc Dashboard Bento Box, giúp các thẻ con xếp cạnh nhau phẳng (flat DOM) mà không cần tạo nhiều thẻ <div> lồng nhau (tránh Div Soup).
- **Flexbox (Component 1D):** Dựa trên nội dung (Content-driven) theo một chiều duy nhất. Lý tưởng cho việc sắp xếp các phần tử con bên trong một Component như Navbar hay căn giữa nội dung trong một Widget mà không lo vỡ layout khi nội dung (chữ) bị thay đổi độ dài.
- **Bootstrap 12-column:** Cung cấp sẵn hệ thống lưới responsive chuẩn hóa, giúp xây dựng nhanh các thành phần phổ biến như Pricing Card mà không phải tự duy trì Media Queries thủ công.
