# Layout Strategy - MetricsHub Dashboard

## Lý do Lựa chọn Công nghệ Dàn trang

CSS Grid và Flexbox không phải là hai công cụ cạnh tranh mà hỗ trợ lẫn nhau theo nguyên tắc: **"CSS Grid sinh ra để làm Layout tổng thể (2D), Flexbox sinh ra để làm Component chi tiết (1D)"**.

### 1. CSS Grid (Không gian 2D)
CSS Grid quản lý giao diện đồng thời theo **cả hai trục (Hàng & Cột)**. Do đó, Grid là lựa chọn hoàn hảo cho các cấu trúc bố cục bất đối xứng như **Bento Dashboard**. Nó cho phép các phần tử con chiếm chính xác vị trí (`span 2 rows`, `span 2 cols`) mà không cần tạo các thẻ HTML bọc ngoài trung gian (`div soup`), giữ cấu trúc DOM phẳng và cực kỳ tối ưu.

### 2. Flexbox (Không gian 1D)
Flexbox quản lý phần tử theo **một trục đơn lẻ (Hàng hoặc Cột)** và hoạt động theo cơ chế *Content-first* (kích thước tự co giãn theo nội dung bên trong). Vì vậy, Flexbox được dùng cho **Navbar** để các liên kết tự động phân bổ khoảng cách dựa trên độ dài của văn bản (dù là tiếng Anh hay tiếng Đức) mà không gây vỡ hoặc tràn giao diện.
