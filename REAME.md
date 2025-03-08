Em sử dụng cấu trúc three-layer.
Các phương thức trong ProductController xử lý yêu cầu từ người dùng và trả về view.
ProductController:
+ getAllProduct(page, size, model)
+ searchProducts(keyword, model)
+ filterProducts(minPrice, maxPrice, model)

ServiceProduct:
+ getAllProducts(pageable)
+ searchProducts(keyword)
+ filterProductsByPrice(minPrice, maxPrice)
  
RepositoryProduct:
+ getAllProducts(pageable)
+ searchProducts(keyword)
+ filterProductsByPrice(minPrice, maxPrice)
Các phương thức trong ServiceProduct chứa logic nghiệp vụ và gọi các phương thức trong RepositoryProduct.
Các phương thức trong RepositoryProduct truy xuất và thao tác với dữ liệu từ ProductDB (hoặc cơ sở dữ liệu).




![image](https://github.com/user-attachments/assets/3263ccbe-c8a3-4dbf-9cb9-122f33f28842)
