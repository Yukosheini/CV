<div align="center">

# Bùi Trung Đức · Personal CV

**Website cá nhân · Hành trình học lập trình · FIT4014**

Một không gian giới thiệu bản thân, chia sẻ sở thích và kết nối,
được xây dựng bằng HTML, CSS và JavaScript thuần.

[Giới thiệu](#giới-thiệu) · [Tính năng](#tính-năng) · [Cách chạy](#cách-chạy) · [Liên hệ](#liên-hệ)

</div>

---

## Giới thiệu

Xin chào, mình là **Bùi Trung Đức**, sinh viên ngành Công nghệ Thông tin. Đây là website cá nhân đầu tiên của mình, được xây dựng trong quá trình học môn **Thiết kế Web — FIT4014**.

Dự án là nơi mình thực hành xây dựng giao diện, tổ chức nội dung và bổ sung các tương tác bằng JavaScript. Website kết hợp thông tin cá nhân, sở thích, những cột mốc học tập và thời khóa biểu trong một giao diện thống nhất với tông màu tím – xanh.

## Tính năng

| Trang | Nội dung chính |
| --- | --- |
| **Trang cá nhân** | Ảnh đại diện, lời giới thiệu và liên kết mạng xã hội. |
| **Sở thích & Thành tựu** | Sở thích âm nhạc, gaming, các cột mốc cá nhân và hiệu ứng đếm số. |
| **Thời khóa biểu** | Lịch học theo tuần, hiển thị trạng thái và thời gian liên quan đến tiết học theo đồng hồ thiết bị. |
| **Liên hệ** | Liên kết điện thoại, Zalo, Facebook, GitHub và biểu mẫu gửi lời nhắn qua Formspree. |

### Điểm nhấn giao diện

- Chuyển đổi giao diện **sáng / tối**, lưu lựa chọn bằng `localStorage`.
- Nền gradient chuyển động và các thẻ nội dung mang hiệu ứng kính mờ.
- Hiệu ứng xuất hiện, hover, con trỏ tùy chỉnh và hạt trang trí.
- Hiệu ứng nghiêng 3D trên một số khối nội dung.
- Bố cục có điều chỉnh cho màn hình nhỏ bằng CSS media queries.

## Công nghệ

| Công nghệ | Vai trò |
| --- | --- |
| **HTML5** | Cấu trúc và nội dung của các trang. |
| **CSS3** | Bố cục, màu sắc, responsive và animation. |
| **JavaScript thuần** | Xử lý tương tác, giao diện sáng/tối, thời khóa biểu và gửi biểu mẫu. |
| **Web APIs** | Sử dụng `localStorage`, `IntersectionObserver`, `requestAnimationFrame` và `fetch`. |
| **Formspree** | Dịch vụ bên ngoài tiếp nhận dữ liệu từ biểu mẫu liên hệ. |

Dự án là website tĩnh, không yêu cầu framework, cài đặt npm hay bước build. CSS và JavaScript hiện chủ yếu được viết trực tiếp trong từng tệp HTML; thư mục `css/` cũng có tệp `style.css`.

## Cấu trúc tệp

Đặt `README.md` cùng cấp với `index.html` ở thư mục gốc của repository.

| Đường dẫn | Mô tả |
| --- | --- |
| `README.md` | Tài liệu giới thiệu và hướng dẫn sử dụng dự án. |
| `index.html` | Trang giới thiệu cá nhân. |
| `hello.html` | Trang sở thích và thành tựu. |
| `Schedule.html` | Trang thời khóa biểu; giữ nguyên chữ **S** viết hoa. |
| `contact.html` | Trang liên hệ và biểu mẫu Formspree. |
| `css/style.css` | Tệp CSS có trong mã nguồn. |
| `assets/images/avatar.jpg` | Ảnh đại diện. |
| `assets/images.jfif` | Hình ảnh dùng làm favicon. |

## Cách chạy

### Mở trực tiếp

1. Tải mã nguồn về máy và giải nén nếu cần.
2. Mở thư mục chứa `index.html`.
3. Mở `index.html` bằng trình duyệt và sử dụng thanh điều hướng để chuyển trang.

### Chạy bằng máy chủ cục bộ

Nếu máy đã có Python, mở terminal tại thư mục chứa `index.html` và chạy:

```bash
python -m http.server 8000
```

Sau đó truy cập **http://localhost:8000**. Nhấn `Ctrl + C` trong terminal để dừng máy chủ. Trên hệ thống dùng lệnh `python3`, thay `python` bằng `python3`.

> Biểu mẫu liên hệ cần kết nối Internet và endpoint Formspree hoạt động. Mã nguồn đã cấu hình endpoint trong thuộc tính `action` của biểu mẫu ở `contact.html`; việc gửi và nhận thư thực tế phụ thuộc vào cấu hình dịch vụ.

## Tùy chỉnh nội dung

- **Thông tin cá nhân:** chỉnh sửa `index.html`.
- **Ảnh đại diện:** thay `assets/images/avatar.jpg` hoặc cập nhật đường dẫn ảnh trong HTML.
- **Sở thích và thành tựu:** chỉnh sửa `hello.html`; các bộ đếm sử dụng giá trị `data-target` được khai báo sẵn, không phải dữ liệu thống kê trực tiếp.
- **Lịch học:** chỉnh sửa bảng trong `Schedule.html`, bao gồm tên môn, phòng học và các thuộc tính `data-day`, `data-start`, `data-end`.
- **Liên hệ:** cập nhật các liên kết và endpoint Formspree trong `contact.html` nếu sử dụng dự án cho người khác.
- **Giao diện:** chỉnh sửa các biến màu trong `:root` và phần `[data-theme="dark"]` của từng trang.

## Hướng phát triển

Các mục dưới đây là định hướng, chưa phải tính năng đã hoàn thành:

- [ ] Tách CSS và JavaScript dùng chung để giảm lặp mã.
- [ ] Bổ sung khu vực giới thiệu dự án và sản phẩm học tập.
- [ ] Cải thiện khả năng truy cập bằng bàn phím và hỗ trợ giảm chuyển động.
- [ ] Hoàn thiện xử lý thời khóa biểu để bỏ qua các ô không có môn học.
- [ ] Bổ sung ảnh chụp giao diện và liên kết website sau khi triển khai.

## Liên hệ

**Bùi Trung Đức** · Sinh viên Công nghệ Thông tin

- **GitHub:** [@yukosheini](https://github.com/yukosheini)
- **Các kênh khác:** xem trang [Liên hệ](contact.html) trong mã nguồn hoặc mở trang tương ứng khi chạy website.

---

<div align="center">

**Cảm ơn bạn đã ghé thăm dự án!**  
Mỗi lần cải thiện website là một bước tiến trong hành trình học lập trình của mình.

</div>
