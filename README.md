# 🚀 Nhập Vai A.I Simulator (AI-Powered RPG)

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-039BE5?style=for-the-badge&logo=Firebase&logoColor=white)
![Gemini AI](https://img.shields.io/badge/Gemini_AI-4285F4?style=for-the-badge&logo=google-gemini&logoColor=white)

**Nhập Vai A.I Simulator** là một ứng dụng mô phỏng nhập vai đột phá, nơi trí tuệ nhân tạo (AI) đóng vai trò là "Quản trò" (Dungeon Master). Hệ thống tự động kiến tạo thế giới, nhân vật và các tình huống dựa trên sự sáng tạo không giới hạn của người chơi.

---

## 📥 Tải Về Phiên Bản Mới Nhất

Bạn có thể tải ngay bản cập nhật ổn định nhất của dự án tại đây:

[![Tải Bản Mới Nhất](https://img.shields.io/badge/DOWNLOAD-LATEST_VERSION-success?style=for-the-badge&logo=github)](https://github.com/thanhbinh-ic/AI-Roleplay-Simulator/releases/latest)

---

## ✨ Tính Năng Nổi Bật

### 🧠 Trí Tuệ Nhân Tạo Thông Minh
- **Kiến tạo thế giới:** AI tự động gợi ý Tên nhân vật, Kỹ năng, Mục tiêu và Tiểu sử dựa trên bối cảnh bạn chọn.
- **Dungeon Master AI:** Ghi nhớ logic câu chuyện, phản ánh đúng tính cách nhân vật qua từng lựa chọn.

### 🎲 Cơ Chế Gameplay Chi Tiết
- **Hệ thống Xúc xắc (Dice System):** Tính toán tỷ lệ thành công dựa trên chỉ số nhân vật với 5 mức độ từ "Rất thấp" đến "Rất cao".
- **Hệ thống Nhiệm vụ (Quest):** AI giao nhiệm vụ theo thời gian thực, có nhật ký theo dõi tiến độ và phần thưởng tác động trực tiếp đến hành trình.
- **Độ khó Ác Mộng:** Thử thách tối thượng cho người chơi với những hậu quả nghiêm trọng khi lựa chọn sai lầm.

### 💾 Quản Lý Dữ Liệu & Hệ Thống
- **Lưu/Tải linh hoạt:** Hỗ trợ lưu dữ liệu trên Firestore hoặc xuất/nhập file `.json` để chơi trên nhiều thiết bị.
- **Cập nhật tự động:** Hệ thống tự động kiểm tra phiên bản mới qua GitHub Gist để đảm bảo bạn luôn có trải nghiệm tốt nhất.

---

## 🛠 Công Nghệ Sử Dụng

- **Frontend:** React.js, Tailwind CSS (Giao diện hiện đại, mượt mà).
- **Backend/Database:** Firebase Firestore & Authentication.
- **AI Engine:** Google Gemini API (hoặc các mô hình ngôn ngữ lớn tương đương).
- **Version Control:** GitHub Gist API cho hệ thống Update tự động.

---

## 📸 Ảnh Chụp Giao Diện

*(Mẹo: Bạn hãy upload ảnh chụp màn hình vào folder `docs/screenshots` rồi thay link vào đây nhé)*

| Màn Hình Khởi Đầu | Giao Diện Chơi Game |
| :---: | :---: |
| ![Start](https://via.placeholder.com/400x225?text=Initial+Screen) | ![Gameplay](https://via.placeholder.com/400x225?text=Gameplay+Screen) |

---

## 📜 Nhật Ký Cập Nhật (Changelog)

### v2.5 (Trải Nghiệm & Kết Nối) - 07/04/2026
- **QUAN TRỌNG:** Sửa lỗi treo ứng dụng khi kiểm tra phiên bản lúc khởi động.
- **THÊM MỚI:** Nút "Kiểm Tra Cập Nhật" thủ công tại màn hình chính.
- **CẬP NHẬT:** Cơ chế Static Redirect giúp link tải luôn hoạt động chính xác.
- **GIAO DIỆN:** Hiệu ứng Backdrop Blur và animation mượt mà cho Popup thông báo.

> Xem thêm các phiên bản cũ hơn trong mục [Update Log] bên trong ứng dụng.

---

## 🚀 Hướng Dẫn Cài Đặt (Dành cho Developer)

1. **Clone repository:**
   ```bash
   git clone [https://github.com/thanhbinh-ic/AI-Roleplay-Simulator.git](https://github.com/thanhbinh-ic/AI-Roleplay-Simulator.git)


   Cài đặt dependencies:

Bash
npm install
Cấu hình API:

Tạo file .env và thêm các khóa API từ Firebase và Gemini.

Chạy ứng dụng:

Bash
npm start
🤝 Đóng Góp & Ủng Hộ
Nếu bạn yêu thích dự án này, hãy tặng mình một ⭐ Star để ủng hộ nhé!

Tác giả: thanhbinh-ic

Ủng hộ: Bạn có thể nhấn vào nút "Ủng Hộ Tác Giả" trực tiếp trong game.

Dự án được phát triển với niềm đam mê dành cho thể loại RPG và Công nghệ AI.
