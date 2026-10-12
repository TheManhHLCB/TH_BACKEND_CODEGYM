# AI Prompt Log

### Prompt 1 (Brainstorming Concept 1D vs 2D)

- **User Prompt:** "Khi tôi cần một bố cục mà một phần tử con (Child) phải chiếm chính xác 2 hàng và 2 cột (span 2 rows, 2 columns) đan xen với các phần tử nhỏ khác, tôi nên chọn CSS Grid hay Flexbox? Tại sao Flexbox lại chật vật với yêu cầu này?"
- **AI Response:** Phân tích sự khác biệt giữa Flexbox (1D) và Grid (2D). Giải thích Flexbox chỉ quản lý 1 trục tại 1 thời điểm nên muốn làm span 2 hàng bắt buộc phải dùng div lồng nhau (Div Soup), còn CSS Grid hỗ trợ `grid-column: span` và `grid-row: span` trực tiếp trên các phần tử đồng cấp.

### Prompt 2 (Tìm hiểu Bootstrap Grid System)

- **User Prompt:** "Trong Bootstrap 5, sự khác biệt giữa lớp col-sm-4 và col-md-4 là gì? Tại sao tôi nên dùng Bootstrap thay vì tự viết CSS Grid cho một phần tử đơn giản như 3 cột Bảng giá?"
- **AI Response:** Giải thích Breakpoints trong Bootstrap (sm >= 576px, md >= 768px). Việc dùng `col-12 col-md-4` giúp cột tự động responsive 100% width trên mobile và chia 3 cột trên tablet/desktop mà không phải tự duy trì media query thuần.

### Prompt 3 (Tối ưu khoảng cách bằng gap)

- **User Prompt:** "Làm thế nào để sử dụng thuộc tính gap trong cả CSS Grid và Flexbox để thay thế margin lộn xộn?"
- **AI Response:** Hướng dẫn sử dụng `gap: 15px` trực tiếp lên Container của cả Grid lẫn Flexbox, loại bỏ hoàn toàn các thủ thuật gỡ bỏ margin phần tử cuối (`:last-child`).
