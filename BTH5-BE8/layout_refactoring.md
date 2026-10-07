# Báo cáo Phân tích Kiến trúc Dàn trang - CreativeChronicle

## Tác hại của `position: absolute` đối với Responsive Design

Kỹ thuật cũ sử dụng `position: absolute` gán cứng chiều cao (`height: 400px`) đã tách hoàn toàn các phần tử ảnh khỏi luồng hiển thị tự nhiên (Document Flow) của DOM. Khi thu nhỏ màn hình di động, các hình ảnh không thể tự thu co hay tính toán lại vị trí, dẫn đến hiện tượng các lớp ảnh tràn ra ngoài khung chứa cha và đè bẹp lên văn bản bài viết bên dưới.

## CSS Grid - Giải pháp Cứu cánh cho Mosaic Gallery

CSS Grid giải quyết triệt để vấn đề này nhờ cơ chế quản lý không gian 2 chiều (Hàng & Cột) đồng thời. Bằng cách định nghĩa `grid-template-columns: 2fr 1fr` kết hợp `grid-row: span 2`, các bức ảnh tự động khớp vào vị trí khảm nghệ thuật mà vẫn giữ nguyên luồng DOM. Khi thay đổi kích thước màn hình, Grid tự động tính toán lại dòng/cột thông qua Media Queries, đảm bảo nội dung bên dưới luôn tự động đẩy xuống mượt mà mà không lo đè lấp.
