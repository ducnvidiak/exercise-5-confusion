# Bộ Prompts Hướng Dẫn Tái Tạo Dự Án (Bootstrap 5 Lab)

Tài liệu này chứa danh sách các prompts được tối ưu hóa tốt nhất để hướng dẫn một trợ lý AI xây dựng dự án này từ đầu theo từng bước khoa học và nhất quán.

---

### 1. Prompt 1: Khởi tạo dự án & Thiết lập Môi trường
```text
Hãy khởi tạo một dự án Web tĩnh sử dụng npm trong thư mục hiện tại.
Thực hiện các công việc sau:
1. Cài đặt các thư viện thiết kế frontend: Bootstrap 5, jQuery và popper.js làm các dependency chính.
2. Cài đặt 'lite-server' làm devDependency phục vụ việc chạy local server tự động tải lại trang.
3. Cấu hình tệp package.json sao cho lệnh "npm start" sẽ kích hoạt chạy 'lite-server'.
4. Tạo tệp .gitignore để bỏ qua thư mục node_modules khi thực hiện quản lý mã nguồn bằng Git.
```

---

### 2. Prompt 2: Xây dựng trang kiểm thử Grid System (`grid.html`)
```text
Hãy xây dựng một trang HTML5 có tên là `grid.html` để kiểm thử hệ thống lưới (Grid System) của Bootstrap 5.
Yêu cầu chi tiết:
1. Nhúng Bootstrap CSS và JS từ thư mục node_modules.
2. Thiết kế thanh điều hướng cố định phía trên (fixed-top navbar) có màu tối (bg-dark) chứa các liên kết đến các trang trong dự án: Home (index.html), Grid Test (active), First Page, FPT Page và Students.
3. Tạo phần Header xám nhạt (Jumbotron kiểu cũ) có tiêu đề "Let's test the grid!" được căn lề trái. Cần đẩy Header xuống (margin-top) để không bị che bởi navbar cố định.
4. Thiết lập phần nội dung chính gồm 3 dòng (rows) không có khoảng giãn lề giữa các cột (sử dụng class g-0 của Bootstrap 5). Mỗi ô (col) có viền mỏng màu xám nhạt, nền xám nhạt và nội dung ghi chữ "col" căn giữa:
   - Dòng 1: Gồm 2 cột bằng nhau (col-6).
   - Dòng 2: Gồm 3 cột bằng nhau (col-4).
   - Dòng 3: Gồm 4 cột bằng nhau (col-3).
5. Thêm Footer đơn giản dưới chân trang hiển thị thông tin "Created by [Tên của bạn]!" được in đậm, cỡ chữ lớn và căn giữa trên nền xám.
```

---

### 3. Prompt 3: Thiết kế trang giới thiệu công nghệ (`first_page.html`)
```text
Hãy thiết kế một trang web có tên là `first_page.html` giới thiệu về các công nghệ Web cốt lõi.
Yêu cầu thiết kế:
1. Sử dụng Bootstrap 5 làm framework giao diện chính.
2. Thêm Navbar đồng bộ với dự án (mục First Page ở trạng thái active).
3. Thiết kế Header ở trên cùng có màu nền xám nhạt và tiêu đề căn giữa: "My First Bootstrap Page".
4. Ở giữa trang, hiển thị 3 hình ảnh biểu tượng đại diện cho: HTML5, CSS3 và Bootstrap xếp cạnh nhau trên một hàng (sử dụng lưới col-12 col-md-4 cho mỗi cột).
   - Ảnh các biểu tượng được căn giữa, tự động co giãn linh hoạt (img-fluid) và giới hạn chiều cao tối đa khoảng 200px.
   - Thêm hiệu ứng CSS hiệu tác (micro-interactions) để khi di chuột qua (hover), các hình ảnh này sẽ phóng to nhẹ (scale 1.05) một cách mượt mà.
5. Thêm một Footer màu tối (bg-dark) ở dưới cùng hiển thị dòng chữ bản quyền ví dụ "© Copyright [Năm] Con Fusion" căn giữa. Sử dụng thuộc tính d-flex flex-column min-vh-100 trên thẻ body để đảm bảo footer luôn nằm sát đáy trang kể cả khi nội dung ít.
```

---

### 4. Prompt 4: Tạo cấu trúc khung trang Đại học FPT (`fpt.html`)
```text
Hãy xây dựng một trang web có tên là `fpt.html` làm khung giao diện cơ sở mang phong cách Đại học FPT.
Yêu cầu:
1. Tích hợp Bootstrap 5 và thanh điều hướng liên kết hệ thống (mục FPT Page ở trạng thái active).
2. Tạo phần Header phía trên mang phong cách thương hiệu: màu nền cam đặc trưng (#f27024), có tiêu đề lớn "FPT UNIVERSITY" và mô tả ngắn gọn màu trắng.
3. Phần thân trang (main content) được để trống dưới dạng container trống để chuẩn bị bổ sung nội dung sau này.
4. Thêm một Footer đơn giản dưới đáy trang hiển thị dòng chữ bản quyền: "© [Năm] Website. All rights reserved." nằm trên nền tối hoặc xám.
```

---

### 5. Prompt 5: Phát triển Cổng thông tin & Điểm danh sinh viên (`students.html`)
```text
Hãy phát triển một trang quản lý thông tin sinh viên chuyên nghiệp có tên là `students.html` bằng Bootstrap 5.
Yêu cầu chi tiết:
1. Tích hợp thanh điều hướng dự án (mục Students ở trạng thái active) và FontAwesome CDN để sử dụng các biểu tượng (icons).
2. Thiết kế phần FPT Top Header ở đầu trang với màu nền cát nhạt (#eddcb9), căn lề thẳng hàng gồm:
   - Cột trái: Logo trường Đại học FPT (fpt-university.png).
   - Cột giữa: Các liên kết thực đơn bằng tiếng Việt đi kèm icon tương ứng: Trang chủ (icon home), Ngành học (icon graduation-cap), Tuyển sinh (icon address-card), Sinh viên (icon list). Các liên kết có màu cam đậm (#d35400).
   - Cột phải: Ô tìm kiếm ghi "Search:" đi kèm ô input màu trắng.
3. Tạo phần Jumbotron biểu ngữ màu cam cam thương hiệu (#f27024) chứa hình ảnh banner lớn (fpt-banner.jpg) được đóng khung trắng có đổ bóng nhẹ xung quanh.
4. Hiển thị đường dẫn Breadcrumb: "Home / Students" ngay dưới banner.
5. Tạo tiêu đề lớn căn giữa: "Students Detail".
6. Thiết kế lưới danh sách sinh viên gồm 4 thẻ sinh viên xếp dạng 2x2 trên desktop (col-12 col-md-6) sử dụng thẻ Card của Bootstrap:
   - Mỗi thẻ card chứa một ảnh thẻ chân dung sinh viên ở phía trên. Thiết lập tỉ lệ khung ảnh chuẩn chân dung là 3:4 (aspect-ratio: 3/4) sử dụng object-fit: cover để ảnh không bị méo.
   - Bên dưới ảnh hiển thị Mã số sinh viên (căn giữa, màu xám).
   - Dòng tiếp theo hiển thị Tên sinh viên (canh trái) và Quê quán (canh phải) bằng chữ in đậm.
   - Thêm phần tùy chọn điểm danh gồm 2 nút radio xếp ngang: "Absent" và "Present".
   - Dưới cùng của mỗi card là nút Submit màu cam bắt mắt (#f27024) chiếm toàn bộ chiều ngang card.
   - Thiết lập dữ liệu mẫu cho 4 sinh viên, trong đó có 1 sinh viên là nam và 3 sinh viên là nữ (Ví dụ: Nguyễn Thảo Vy - DaNang, Nguyễn Sỹ Đức - HaTinh, Lê Mai Anh - Hue, Phạm Minh Thư - DaNang).
7. Thiết kế Footer màu cam (#f27024) đồng bộ với giao diện:
   - Cột trái hiển thị "Our Address" kèm các dòng thông tin liên hệ có icon FontAwesome đi kèm (địa chỉ, điện thoại, fax, email).
   - Cột phải hiển thị dãy biểu tượng mạng xã hội màu trắng xếp ngang (Google+, Facebook, LinkedIn, Twitter, YouTube, Envelope).
   - Dòng dưới cùng hiển thị bản quyền "© Copyright [Năm]".
```

---

### 6. Prompt 6: Xây dựng trang tổng quan điều hướng (`index.html`)
```text
Hãy thiết kế lại trang `index.html` của bạn thành một trang tổng quan (Dashboard) hướng dẫn dự án.
Yêu cầu:
1. Nhúng Bootstrap 5 và FontAwesome CDN cho các biểu tượng.
2. Thêm thanh điều hướng đồng bộ (mục Home ở trạng thái active).
3. Tạo khu vực Jumbotron giới thiệu có màu chuyển sắc gradient hiện đại (như từ xanh đậm sang xanh ngọc) có tiêu đề "Tổng Quan & Hướng Dẫn Dự Án" và đoạn giới thiệu ngắn gọn về bài tập thực hành Bootstrap 5.
4. Thiết lập phần nội dung chính hiển thị 4 thẻ giới thiệu (cấu trúc col-12 col-md-6 col-lg-3) dẫn tới 4 trang con đã tạo (Grid Test, First Page, FPT Page, Students):
   - Mỗi thẻ có nền trắng, đổ bóng nhẹ, chứa một vòng tròn màu nhạt làm nền cho biểu tượng tương ứng ở trên đầu.
   - Hiển thị tên trang, đoạn mô tả ngắn về chức năng chính của trang đó và các badge (nhãn màu) thể hiện các công nghệ sử dụng trong bài tập đó.
   - Dưới cùng thẻ là nút bấm hành động (ví dụ: "Xem trang Grid Test",...) có mũi tên hướng sang phải.
5. Thiết lập phần Footer màu tối (bg-dark) đồng bộ, bao gồm một cột giới thiệu chung, một cột liên kết nhanh đến các bài học (các trang con) và một cột thông tin liên hệ kèm hệ thống icon mạng xã hội.
```
