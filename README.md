API test with Postman

# Phân tích tài liệu API
API được chọn là DogAPI, đây là API cung cấp cho người dùng thông tin về các giống chó và hình ảnh của chúng.

-Base URL: https://dog.ceo/api/breeds
-Các endpoint chính:
  o	List all breed: /list/all
  o	Get random dog image: /image/random
  o	Get images by breed: /{{breed_name}}/image
  o Get sub-breed list: /{{breed_name}}/list
# Các trường hợp kiểm thử
Trường hợp 1: Tra cứu tất cả các giống chó
- Endpoint: https://dog.ceo/api/breeds/list/all
- Expect: Thông tin về tất cả giống chó, mã trạng thái 200
  ![image](https://github.com/singuyenvan0206/Postman_learn/assets/96609459/9a447c35-a2eb-4303-a197-995af7d9c7ee)
Trường hợp 2: Tra cứu ảnh chú chó bất kì
- Endpoint: https://dog.ceo/api/breeds/image/random
- Expect: Link dẫn đến ảnh chú chó bất kỳ, mã trạng thái 200
 ![image](https://github.com/singuyenvan0206/Postman_learn/assets/96609459/794e9056-cc7a-4d0f-80bd-e584cc339eb5)
Trường hợp 3: Tra cứu giống chó không tồn tại
- Endpoint: https://dog.ceo/api/breed/nonebreed/images
- Expect: Thông báo không tìm thấy giống chó, mã trạng thái 404
  ![image](https://github.com/singuyenvan0206/Postman_learn/assets/96609459/a5ae1116-73b4-4669-b15b-e283f8a20a14)

# Báo Cáo Kiểm Thử
Mục Tiêu Kiểm Thử:

Xác định và xác thực các phản hồi của DogAPI dựa trên các truy vấn khác nhau.
Phạm Vi Kiểm Thử:

Các điểm cuối liên quan đến việc lấy dữ liệu về chó.
Kết Quả Kiểm Thử:

Tất cả các trường hợp kiểm thử được thực hiện và kết quả phù hợp với mong đợi.
API hoạt động đúng với giống chó hợp lệ và xử lý các lỗi một cách thích hợp khi cung cấp dữ liệu không hợp lệ.
Khuyến Nghị:

API hoạt động tốt và xử lý các lỗi đúng cách. Khuyến nghị duy trì tài liệu chi tiết và cung cấp các ví dụ cụ thể để hỗ trợ người dùng API.
