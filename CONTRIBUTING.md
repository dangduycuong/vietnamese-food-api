# Hướng dẫn đóng góp dữ liệu (Contributing Guide)

Cảm ơn bạn đã chung tay làm phong phú thêm kho dữ liệu ẩm thực Việt Nam! Để dữ liệu đồng bộ và không gây lỗi cho các ứng dụng đang sử dụng API, vui lòng tuân thủ các quy tắc sau khi tạo Pull Request:

## 1. Quy tắc đặt ID & Tên file ảnh
* **ID (`id`):** Đặt nối tiếp theo số thứ tự cuối cùng trong file `vietnamese_foods.json` (Ví dụ: `vn_13`, `vn_14`...).
* **Hình ảnh (`thumb`):**
  * Tải ảnh vào thư mục `images/`.
  * Tên file viết thường, không dấu, dùng dấu gạch dưới `_` thay cho khoảng trắng (Ví dụ: `bun_dau_mam_tom.jpg`).
  * Định dạng `.jpg`, `.png` hoặc `.webp`, dung lượng tối ưu **dưới 300KB** để tải nhanh trên di động.

## 2. Quy tắc phân loại Danh mục (`category`)
Vui lòng sử dụng một trong các nhóm danh mục có sẵn để bộ lọc trên ứng dụng hiển thị gọn gàng:
* `Món Nước` (Phở, bún, miến, hủ tiếu, cháo...)
* `Món Khô` (Cơm, bún trộn, mì khô, xôi...)
* `Món Cuốn & Bánh` (Bánh mì, gỏi cuốn, bánh xèo, bánh cuốn...)
* `Đồ Uống` (Cà phê, trà, chè, nước ép...)
* `Món Chay` (Các món thuần chay)

## 3. Mẫu JSON chuẩn cho một món mới
```json
{
  "id": "vn_13",
  "name": "Tên Món Ăn",
  "category": "Món Nước",
  "area": "Tên tỉnh thành hoặc vùng miền (VD: Hà Nội, Miền Tây)",
  "thumb": "ten_mon_an.jpg",
  "ingredients": [
    "Định lượng + tên nguyên liệu 1",
    "Định lượng + tên nguyên liệu 2"
  ],
  "instructions": "1. Bước sơ chế...\n2. Bước chế biến...\n3. Trình bày và thưởng thức."
}
```
