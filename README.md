# BT2_Mobile
Bài tập 02 của sinh viên: K225480106057 - Phạm Mạnh Quỳnh - môn Phát triển ứng dụng trên thiết bị di động

# BÀI TẬP 2 – XÂY DỰNG ỨNG DỤNG ANDROID BẰNG ANDROID STUDIO

## Tên ứng dụng

**Món Ăn Offline**

---

# 1. Giới thiệu

Ứng dụng cho phép người dùng xem danh sách các món ăn Việt Nam.

Dữ liệu được chuẩn bị trước dưới dạng file JSON và đóng gói sẵn trong ứng dụng để sử dụng offline.

---

# 2. Cấu trúc Project

  <img width="579" height="723" alt="Screenshot 2026-06-11 222329" src="https://github.com/user-attachments/assets/f5b1e267-35d1-4027-890c-3ce5f383808a" />


# 3. AndroidManifest.xml

## Mô tả

Manifest dùng để:

* Khai báo Activity
* Cấu hình ứng dụng
* Quản lý quyền truy cập

# 4. MainActivity

## Chức năng

* Khởi tạo Activity
* Đọc dữ liệu JSON
* Xử lý sự kiện click
* Hiển thị dữ liệu

Sử dụng:

* onCreate()
* JSONArray
* JSONObject
* StringBuilder

**Ảnh file MainActivity.java**
<img width="1919" height="1079" alt="Screenshot 2026-06-11 223530" src="https://github.com/user-attachments/assets/86dd9275-a500-43d0-86c8-9df963979089" />

---

# 5. activity_main.xml

## Chức năng

Thiết kế giao diện ứng dụng.

Sử dụng:

* LinearLayout
* Button
* TextView
* ScrollView

Ví dụ:

**Ảnh file activity_main.xml**
<img width="1919" height="1058" alt="Screenshot 2026-06-11 223542" src="https://github.com/user-attachments/assets/4dcc8607-8f16-4e97-91bb-404da22afdc9" />

# 6. strings.xml

## Chức năng

Lưu nội dung giao diện.

Ưu điểm:

* Không hardcode
* Hỗ trợ đa ngôn ngữ

**Ảnh file strings.xml**
<img width="1919" height="1076" alt="Screenshot 2026-06-11 223558" src="https://github.com/user-attachments/assets/2f4d89ab-fb34-4e46-9ab6-5527bbe18ff2" />

# 7. strings.xml (English)

Thư mục:

```plaintext
values-en/
```

Android tự động đổi giao diện theo ngôn ngữ thiết bị.

**Ảnh strings.xml tiếng Anh**
<img width="1919" height="1079" alt="Screenshot 2026-06-11 223604" src="https://github.com/user-attachments/assets/689c937f-0bb3-4efc-bb3b-e7a6434f4dcd" />

# 8. colors.xml + colors-night.xml

## Chức năng

Quản lý màu sắc.

Hỗ trợ:

* Light Mode
* Dark Mode

**Ảnh file colors.xml**
<img width="1919" height="1079" alt="Screenshot 2026-06-11 223547" src="https://github.com/user-attachments/assets/b9714b81-dc21-49dd-a4db-a4c679fad2fa" />

**Ảnh Dark Mode**
<img width="1919" height="1077" alt="Screenshot 2026-06-11 223552" src="https://github.com/user-attachments/assets/8a3ed32d-4c97-4095-834c-9c43b99f43e6" />

---

# 9. Dữ liệu chuẩn bị trước – recipes.json

## Nội dung

Lưu thông tin:

* tên món
* thời gian
* nguyên liệu
* hướng dẫn

Đặt tại:

```plaintext
res/raw/recipes.json
```

**Ảnh file recipes.json**
<img width="1919" height="1079" alt="Screenshot 2026-06-11 223536" src="https://github.com/user-attachments/assets/a0e7641c-0a2c-4151-b747-aeeb810fcf67" />

# 10. Thuật toán xử lý

```plaintext
Đọc file JSON
↓

Parse dữ liệu

↓

Lặp từng món

↓

Ghép nội dung

↓

Hiển thị lên TextView
```

# 11. Kết quả chạy chương trình

### Màn hình ban đầu
<img width="1080" height="2280" alt="Screenshot_2026-06-12-10-52-36-564_com example btl_app" src="https://github.com/user-attachments/assets/6eb53102-321c-42c9-bff3-f99e5d4b1a13" />

### Sau khi nhấn nút
<img width="1080" height="2280" alt="Screenshot_2026-06-11-22-33-34-865_com example btl_app" src="https://github.com/user-attachments/assets/4fd6d703-ffcc-40da-b189-76f93cf0d684" />
<img width="1080" height="2280" alt="Screenshot_2026-06-11-22-33-39-415_com example btl_app" src="https://github.com/user-attachments/assets/5105aeb7-0d55-4d22-8dda-cfdf3fc407e8" />
<img width="1080" height="2280" alt="Screenshot_2026-06-11-22-33-44-114_com example btl_app" src="https://github.com/user-attachments/assets/f985be96-0873-460a-b3dd-3d5a2db06a6b" />
<img width="1080" height="2280" alt="Screenshot_2026-06-11-22-33-53-850_com example btl_app" src="https://github.com/user-attachments/assets/829ff483-7d8d-4b30-ac9d-8fcbd7d1abef" />

### Chế độ Dark Mode
<img width="1080" height="2280" alt="Screenshot_2026-06-12-10-50-51-969_com example btl_app" src="https://github.com/user-attachments/assets/8247dd83-0a52-4913-baf3-888bb785c2b1" />

# 12. Kết luận

Ứng dụng đã:

✔ Đọc dữ liệu từ file JSON

✔ Hoạt động offline

✔ Thiết kế bằng XML

✔ Xử lý sự kiện bằng Java

✔ Hỗ trợ đa ngôn ngữ

✔ Hỗ trợ Dark Mode
