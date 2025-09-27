# 🌐 Local Passport Website

---

## 📑 Mục lục

- [⚙️ Cài đặt & Chạy dự án](#️-cài-đặt--chạy-dự-án)
- [⚙️ Set Up Session với FileStore](#️-set-up-nơi-lưu-trữ-cho-session-bằng-filestore)
- [🚫 Truy cập `/profile` khi chưa đăng nhập](#-truy-cập-profile-khi-chưa-đăng-nhập)
- [📝 Tạo tài khoản](#-tiến-hành-tạo-tài-khoản)
- [🔑 Đăng nhập](#-đăng-nhập-trên-website)
- [💾 Lưu trữ Session trong FileStore](#-lưu-trữ-thông-tin-đăng-nhập-ở-filestore)
- [🚪 Đăng xuất](#-đăng-xuất)

---

## ⚙️ Cài đặt & Chạy dự án

### 📦 Cài đặt dependencies

```bash
npm install
```

### 📂 Cài đặt session-file-store

```bash
npm install session-file-store
```

### ▶️ Chạy dự án

```bash
node app.js
```

---

## ⚙️ Set Up nơi lưu trữ cho session bằng **FileStore**

📸 Minh họa: <img src="./asset/img/image1.png" alt="Cấu hình FileStore"/>

---

## 🚫 Truy cập `/profile` khi chưa đăng nhập

🎥 Demo: <video controls src="./asset/img/1.gif" title="Demo"></video>

👉 **Kết quả:**
Bị chuyển hướng lại trang **login** vì chưa đăng nhập.

---

## 📝 Tiến hành tạo tài khoản

- Thông tin test:

  ```json
  {
    "username": "lyhoangnghiem",
    "password": "123456"
  }
  ```

📸 Giao diện tạo tài khoản: <img src="./asset/img/image2.png" alt="Form đăng ký"/>

### ✍️ Tạo tài khoản thông qua giao diện website

<img src="./asset/img/image3.png" alt="Tạo tài khoản web"/>

### 🗄️ Kiểm tra database đã có thông tin chưa

<img src="./asset/img/image4.png" alt="Kiểm tra DB"/>

---

## 🔑 Đăng nhập trên website

- Thông tin test:

  ```json
  {
    "username": "lyhoangnghiem",
    "password": "123456"
  }
  ```

📸 Giao diện đăng nhập: <img src="./asset/img/image5.png" alt="Form đăng nhập"/>

### ✅ Khi đăng nhập thành công → vào **trang chủ**

<img src="./asset/img/image6.png" alt="Trang chủ sau khi login"/>

---

## 💾 Lưu trữ thông tin đăng nhập ở FileStore

📸 Kết quả khi đăng nhập thành công: <img src="./asset/img/image7.png" alt="Session trong FileStore"/>

### ❌ Khi đăng nhập thất bại (sai mật khẩu)

<img src="./asset/img/image8.png" alt="Login thất bại"/>

---

## 🚪 Đăng xuất

👉 Sau khi đăng xuất:

- Session trong **FileStore** bị xóa ✅
- Người dùng bị chuyển hướng về trang login.

📸 Minh họa: <img src="./asset/img/image9.png" alt="Đăng xuất thành công"/>
