# vietnamese-food-api
# 🍜 Vietnamese Food & Drink API (API Ẩm Thực Việt Nam)

Kho dữ liệu mở miễn phí (JSON API) tổng hợp các món ăn và đồ uống đặc trưng của ẩm thực Việt Nam, bao gồm tên món, vùng miền, danh mục, hình ảnh, nguyên liệu và hướng dẫn chế biến chi tiết bằng tiếng Việt.

Dự án được tạo ra nhằm giúp cộng đồng lập trình viên dễ dàng tích hợp dữ liệu ẩm thực Việt Nam vào các ứng dụng Mobile (Flutter, React Native, Android, iOS) hoặc Web mà không tốn chi phí duy trì server.

## 🚀 API Endpoints

### 1. Lấy toàn bộ danh sách món ăn & đồ uống
* **Method:** `GET`
* **Endpoint:**
```text
https://raw.githubusercontent.com/dangduycuong/vietnamese-food-api/main/vietnamese_foods.json
```

### 2. Đường dẫn hình ảnh (Base Image URL)
Ghép đường dẫn gốc dưới đây với tên file trong trường `"thumb"` của mỗi món:
```text
https://raw.githubusercontent.com/dangduycuong/vietnamese-food-api/main/images/<tên-file-ảnh>
```
**Ví dụ:** ```text
https://raw.githubusercontent.com/dangduycuong/vietnamese-food-api/main/images/pho_bo.jpg
```

## 📦 Cấu trúc dữ liệu (JSON Schema)

```json
{
  "items": [
    {
      "id": "vn_01",
      "name": "Phở Bò Hà Nội",
      "category": "Món Nước",
      "area": "Miền Bắc",
      "thumb": "pho_bo.jpg",
      "ingredients": [
        "500g bánh phở tươi",
        "300g thịt bò tái"
      ],
      "instructions": "1. Xương bò rửa sạch..."
    }
  ]
}
```

## 🤝 Đóng góp dữ liệu (Contribute)
Hoan nghênh mọi đóng góp để làm phong phú thêm bản đồ ẩm thực Việt Nam! Bạn có thể tạo **Pull Request** hoặc mở **Issue** để bổ sung thêm các món ăn đặc sản vùng miền khác.

## 📄 Giấy phép (License)
Dữ liệu được chia sẻ miễn phí cho mục đích học tập và phát triển ứng dụng cộng đồng.
