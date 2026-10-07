# AI Prompt Log - MetricsHub Refactoring

## Prompt 1: Đánh giá Bento Box Layout
- **Prompt:** "Khi tôi cần một bố cục mà một phần tử con (Child) phải chiếm chính xác 2 hàng và 2 cột (span 2 rows, 2 columns) đan xen với các phần tử nhỏ khác, tôi nên chọn CSS Grid hay Flexbox? Tại sao Flexbox lại chật vật với yêu cầu này?"
- **Mục đích:** Xác định lý do tại sao cấu trúc Legacy dùng Flexbox lồng nhau bị vỡ trên iPad và đưa ra giải pháp CSS Grid phẳng.

## Prompt 2: So sánh Bootstrap Grid
- **Prompt:** "Trong Bootstrap 5, sự khác biệt giữa lớp col-sm-4 và col-md-4 là gì? Tại sao tôi nên dùng Bootstrap thay vì tự viết CSS Grid cho một phần tử đơn giản như 3 cột Bảng giá?"
- **Mục đích:** Hiểu về điểm ngắt breakpoint (768px cho `col-md-4`) để đảm bảo khu vực Bảng giá tự động xếp chồng chuẩn responsive mà không tốn công viết Media Queries thuần.

## Prompt 3: Tối ưu hoá khoảng cách
- **Prompt:** "Làm thế nào để sử dụng thuộc tính `gap` hỗ trợ chung cho cả CSS Grid và Flexbox nhằm thay thế cho thuộc tính `margin` rườm rà?"
- **Mục đích:** Loại bỏ hoàn toàn các dòng CSS căn chỉnh `margin: 5px` của code cũ, tạo khoảng cách chuẩn xác, nhất quán cho cả Navbar và Bento Box.
