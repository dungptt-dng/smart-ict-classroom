# Nhật ký kiểm thử – AI Điều Phối Lớp Học Tin Học (phiên bản 1)

Ngày kiểm thử: 28/10/2026 · Người thực hiện: Claude (kiểm thử kỹ thuật trên trình duyệt, máy chủ tĩnh cục bộ) · Dữ liệu: **dữ liệu minh họa**, không phải số liệu lớp học thật.

Đường dẫn ứng dụng (riêng tư, chỉ chủ tài khoản mở được cho tới khi chia sẻ): https://claude.ai/artifact/Ln5sj415uNe76Mup71s9D1

## Kết quả theo 8 kịch bản

| # | Kịch bản | Kết quả | Ghi chú |
|---|---|---|---|
| 1 | Thiết lập buổi học | Đạt | Để trống tên bài → báo "Nhập tên bài học."; số nhóm 40 > sĩ số → báo lỗi, không cho áp dụng. |
| 2 | Nhập số nhóm, số máy | Đạt | 28 HS / 7 nhóm / 4 máy → chia 7 nhóm × 4 HS; khi đã có tiến độ, hiện hộp xác nhận trước khi chia lại. |
| 3 | Đề xuất phương án điều phối (quy tắc) | Đạt | Tính số lượt, số đợt, lượt máy/nhóm; cảnh báo lượt chưa đều kèm gợi ý cụ thể (7 lượt hoặc 8 nhóm); cảnh báo "Bước 3" không đủ thời gian máy với 5 nhóm. |
| 4 | Giao nhiệm vụ | Đạt | Thêm (có kiểm tra thiếu dữ liệu), sửa, xóa (có xác nhận), giao cho tất cả, đổi thứ tự, lọc theo hình thức. |
| 5 | Luân phiên máy / tại chỗ, đổi vai | Đạt | Lịch hiển thị nhóm lên máy và nhiệm vụ tại chỗ từng lượt; vai TT/ĐD/KT/BC xoay sau mỗi lượt máy. |
| 6 | Cập nhật tiến độ | Đạt | Đổi trạng thái 3 mức; tự báo "Chậm 1 nhiệm vụ", "Xong sớm"; đánh dấu cần hỗ trợ; nhận xét được lưu; đồng hồ đếm ngược chạy. |
| 7 | Trợ lý AI | Đạt (gọi thật do giáo viên xác nhận) | Đã kiểm thử: dựng dữ liệu gửi AI cho cả 7 chức năng (không chứa mã/tên học sinh); chế độ thủ công (dán câu trả lời, đọc JSON nhiệm vụ, thêm vào ngân hàng, lưu vào báo cáo); xử lý lỗi từ chối quyền. Luồng gọi AI được thử bằng hàm giả lập để kiểm tra mã; gọi Claude thật do giáo viên thử trên claude.ai (xem mục dưới). |
| 8 | Báo cáo cuối buổi | Đạt | Thống kê, bảng theo nhóm/nhiệm vụ, nhật ký; tạo nội dung .html/.csv; nhập .json (tệp hỏng bị từ chối); "Buổi học mới" xóa tiến độ, giữ nhiệm vụ. |

## Lỗi đã phát hiện và sửa trong lúc kiểm thử
- Lỗi khởi động khi mở ngoài claude.ai (biến dùng trước khi khai báo) → đã sửa.
- Thanh tiến độ hiển thị thành hình bầu dục lớn → đã sửa.
- Gợi ý "số lượt" sai khi số nhóm không chia hết → đã viết lại công thức.
- Dữ liệu minh họa đặt sai lượt hiện tại → đã sửa thành Lượt 2.

## Kiểm thử gọi Claude thật
- 28/10/2026: giáo viên mở link trên claude.ai, bấm cho phép và gửi yêu cầu cho trợ lý AI; giáo viên xác nhận AI trả lời bình thường. (Chưa lưu ảnh chụp màn hình làm minh chứng – cần chụp khi quay video.)

## Chưa kiểm thử
- Tải tệp qua hộp thoại tải xuống của claude.ai.
- Dùng trong lớp học thật.
