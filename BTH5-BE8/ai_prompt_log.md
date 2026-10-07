# AI Prompt Log - CreativeChronicle Refactoring

## Prompt 1: Tìm hiểu CSS Grid Template & Spanning
- **Prompt:** "Làm thế nào để tạo một Mosaic Gallery có 1 ảnh lớn bên trái chiếm 2 hàng và 2 ảnh nhỏ xếp chồng bên phải bằng CSS Grid mà không cần dùng `position: absolute`?"
- **Mục đích:** Thay thế hoàn toàn cách làm cũ, chuyển sang `grid-row: span 2` kết hợp `object-fit: cover`.

## Prompt 2: Tìm hiểu Bootstrap Utility Classes
- **Prompt:** "Cách dùng các class tiện ích của Bootstrap 5 như `d-flex`, `align-items-center`, `gap-3` để căn giữa avatar và thông tin tác giả theo chiều dọc nhanh nhất mà không cần viết thêm CSS thuần?"
- **Mục đích:** Tối ưu hóa Vùng 1 (Author Info) để đạt chuẩn Flexbox 1D gọn nhẹ.

## Prompt 3: Cấu hình Breakpoints cho Grid System
- **Prompt:** "Cú pháp chia cột nào trong Bootstrap giúp một danh sách gồm 4 thẻ tự động hiển thị: 4 cột trên Desktop (`col-lg-3`), 2 cột trên Tablet (`col-md-6`), và 1 cột trên Mobile (`col-12`)?"
- **Mục đích:** Đảm bảo Vùng Recommended Articles hiển thị chuẩn xác trên mọi màn hình.
