# FPT University & Ristorante Con Fusion - Bootstrap 5 Project Lab

Dự án web front-end thực hành các tính năng cốt lõi của framework **Bootstrap 5** kết hợp các công nghệ web cơ bản (HTML5, CSS3) với chủ đề thương hiệu trường Đại học FPT và nhà hàng Con Fusion.

**Tác giả:** Nguyễn Sỹ Đức  
**Phiên bản:** 1.0.0

---

## 📂 Cấu trúc dự án (Project Structure)

Dự án bao gồm các tệp tin chính sau:

*   **`index.html` (Trang chủ / Dashboard):** Trang tổng quan tích hợp thẻ hướng dẫn trực quan (Guide Cards) liên kết đến 4 trang thực hành con cùng chân trang (Footer) chuyên nghiệp chứa mạng xã hội và thông tin liên hệ.
*   **`grid.html` (Thử nghiệm Grid):** Trang thực hành chia lưới không khoảng cách (gutterless `g-0`) thể hiện khả năng phản hồi tự động trên các độ phân giải màn hình khác nhau.
*   **`first_page.html` (Core Tech Intro):** Trang giới thiệu 3 trụ cột thiết kế giao diện (HTML5, CSS3, Bootstrap) có hiệu ứng phóng to (hover zoom) động khi di chuột qua.
*   **`fpt.html` (FPT Basic Layout):** Giao diện cơ sở tối giản mang thương hiệu trường Đại học FPT làm nền tảng bố cục.
*   **`students.html` (Quản lý sinh viên):** Trang cổng thông tin sinh viên FPT (Nguyễn Thảo Vy, Trần Anh Tuấn, Lê Mai Anh, Phạm Minh Thư) với bố cục 2x2, ảnh chân dung tỷ lệ dọc 3:4, hệ thống nút điểm danh (Absent / Present) và footer chi tiết đồng bộ màu cam FPT.
*   **`prompts.md` (Tài liệu gợi ý AI):** Bộ 6 câu lệnh (prompts) tiếng Việt được thiết kế tối ưu để hướng dẫn AI sinh mã nguồn tái tạo dự án này từ đầu.
*   **`assets/images/`:** Thư mục lưu trữ tài nguyên hình ảnh (biểu tượng công nghệ, logo FPT, ảnh sinh viên, banner).

---

## 🛠️ Công nghệ sử dụng (Tech Stack)

*   **Core:** HTML5, CSS3
*   **CSS Framework:** Bootstrap 5
*   **Libraries:** jQuery (Slim), Popper.js
*   **Icon Fonts:** FontAwesome 6 (CDN)
*   **Dev Server:** `lite-server` (Node.js)

---

## 🚀 Hướng dẫn khởi chạy dự án (How to Run)

### Yêu cầu hệ thống
*   Đã cài đặt **Node.js** và **NPM** trên máy tính.

### Các bước cài đặt & Chạy ứng dụng

1.  **Cài đặt các gói thư viện phụ thuộc:**
    Mở Terminal tại thư mục `conFusion` và chạy lệnh sau để tải Bootstrap, jQuery và Popper.js về `node_modules`:
    ```bash
    npm install
    ```

2.  **Khởi động máy chủ phát triển (Development Server):**
    Chạy lệnh sau để kích hoạt máy chủ `lite-server`:
    ```bash
    npm start
    ```

3.  **Xem kết quả:**
    Trình duyệt sẽ tự động mở trang chủ tại địa chỉ:
    👉 **[http://localhost:3000](http://localhost:3000)**

---

## 📝 Danh sách ảnh cần cung cấp thêm (Assets Needed)
Để trang quản lý sinh viên `students.html` hiển thị hoàn thiện nhất, bạn hãy bổ sung các tệp tin hình ảnh sau vào thư mục `assets/images/`:
*   `fpt-banner.jpg`: Ảnh biểu ngữ nhóm sinh viên áo cam.
*   `DE160182.jpg`: Ảnh thẻ sinh viên Nguyễn Thảo Vy.
*   `DE160488.png`: Ảnh thẻ sinh viên Nguyễn Sỹ Đức.
*   `DE160547.jpg`: Ảnh thẻ sinh viên Lê Mai Anh.
*   `DE170049.jpg`: Ảnh thẻ sinh viên Phạm Minh Thư.

---

## 🤖 Bộ gợi ý tạo mã (AI Prompts)

Dự án tích hợp tệp **[prompts.md](./prompts.md)** chứa 6 bước gợi ý (prompts) chi tiết và tối ưu hóa cao. Bạn có thể sao chép các câu lệnh này cung cấp cho các trợ lý lập trình AI (ChatGPT, Claude, Gemini, Antigravity,...) để tái sinh tự động toàn bộ mã nguồn hoặc các mô-đun riêng lẻ của dự án này một cách trực quan và đồng bộ nhất.
