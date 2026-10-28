# AI Điều Phối Lớp Học Tin Học – Smart ICT Classroom

Ứng dụng web giúp giáo viên Tin học tiểu học tổ chức giờ thực hành trong phòng máy có ít máy hơn số nhóm: chia nhóm, xếp lượt máy công bằng, xoay 4 vai trong nhóm, giao nhiệm vụ trên máy và tại chỗ, theo dõi tiến độ, hỏi trợ lý AI và xuất báo cáo buổi học.

Sản phẩm dự thi Giải thưởng Tiên phong Ứng dụng AI trong Giáo dục Việt Nam 2026 (Bảng A).

## Mở ứng dụng

| Bản | Đường link | Trợ lý AI |
|---|---|---|
| Trên claude.ai | https://claude.ai/artifact/Ln5sj415uNe76Mup71s9D1 | Gọi Claude trực tiếp (cần đăng nhập claude.ai) |
| GitHub Pages | https://dungptt-dng.github.io/smart-ict-classroom/ | Chế độ thủ công: sao chép yêu cầu, dán câu trả lời từ trợ lý AI bên ngoài |

Phần điều phối (chia nhóm, lịch máy, xoay vai, theo dõi, báo cáo) chạy giống nhau ở cả hai bản. Dữ liệu lưu trên trình duyệt của máy đang dùng; sao lưu bằng tệp `.json` trong mục Báo cáo buổi học.

## Nội dung

- `app/ai-dieu-phoi-lop-hoc.html` – toàn bộ ứng dụng trong một tệp HTML (HTML, CSS, JavaScript thuần), không cần cài đặt hay máy chủ.
- `app/KIEM_THU_v1.md` – nhật ký kiểm thử kỹ thuật.
- `ho-so/anh-ung-dung/` – ảnh chụp ứng dụng với dữ liệu minh họa.

## AI và quy tắc lập trình

- **Quy tắc lập trình (không phải AI):** chia nhóm, lịch luân phiên máy, xoay vai, cảnh báo, thống kê tiến độ.
- **AI tạo sinh (Claude, Anthropic):** 7 chức năng trong mục Trợ lý AI – đề xuất điều phối, tạo nhiệm vụ phân hóa, hoạt động tại chỗ khi chờ máy, câu hỏi gợi mở, xử lý nhóm xong sớm/chậm, tổng kết buổi học, hỏi tự do. Mã nguồn không chứa API key.

## Dữ liệu học sinh

Học sinh chỉ được ghi bằng mã (HS01, HS02…). Dữ liệu gửi cho AI chỉ gồm thông tin bài học, tên nhóm, số lượng, trạng thái nhiệm vụ và nhận xét của giáo viên; giáo viên xem được chính xác nội dung trước khi gửi. Dữ liệu có sẵn trong ứng dụng là **dữ liệu minh họa**, không phải số liệu lớp học thật.

## Học liệu

Bài minh họa: Tin học 5 (Kết nối tri thức với cuộc sống) – Bài 4: Cây thư mục; thẻ phân vai, phiếu thực hành “Xây dựng khu lưu trữ thông minh” và câu hỏi thảo luận do giáo viên biên soạn.
