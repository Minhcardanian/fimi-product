# QUIZ PLATFORM – FUNCTIONAL SPECIFICATION & COMPENSATION PLAN

## 1. TỔNG QUAN DỰ ÁN

Xây dựng nền tảng quiz chuyên nghiệp với các tính năng:
- Tạo đề & làm bài
- Quản lý nhóm lớp học
- Tích hợp AI tạo câu hỏi từ tài liệu (Thầy Hùng phụ trách AI backend, host nội bộ)
- Hệ thống phân loại người dùng, thanh toán, lưu kết quả
- Giao diện webapp responsive, tối giản, tinh gọn, hướng đến người dùng mobile

> 🤝 **Nhân sự chính**:
> - **Minh**: Phát triển frontend, backend, giao diện người dùng  
> - **Thầy Hùng**: Phụ trách AI backend (Python, host nội bộ)  
> - **Cộng tác viên**: Được giao các chức năng cụ thể theo milestone

---

## 2. DANH SÁCH CHỨC NĂNG & CHI PHÍ THEO MODULE

| Mã  | Tính năng                  | Mô tả kỹ thuật                                      | Giao diện            | Độ phức tạp | Giá đề xuất (VNĐ) |
|-----|----------------------------|-----------------------------------------------------|----------------------|-------------|-------------------|
| F1  | Đăng ký / Đăng nhập        | Firebase Auth / Supabase                            | Login UI             | Trung bình  | 800.000           |
| F2  | Dashboard người dùng       | Danh sách quiz đã tạo/làm, loại tài khoản           | UI đơn giản          | Dễ          | 500.000           |
| F3  | Tạo & quản lý quiz         | CRUD quiz, lưu DB, publish/private                  | Quiz form UI         | Trung bình  | 1.200.000         |
| F4  | Làm quiz + chấm điểm       | Countdown, chọn đáp án, chấm tự động                | Giao diện quiz       | Khá cao    | 1.500.000         |
| F5  | Tích hợp AI quiz           | Nhận link → gửi Thầy Hùng → render quiz             | Form + preview       | Cao         | 2.000.000         |
| F6  | Quản lý lớp học            | Tạo nhóm, mời thành viên, gán quiz                  | UI lớp học           | Trung bình  | 1.200.000         |
| F7  | Thống kê kết quả           | Theo quiz, theo lớp, hiển thị bảng điểm             | Bảng kết quả         | Trung bình  | 1.000.000         |
| F8  | Thanh toán & phân quyền    | Stripe/Momo + quản lý gói Free/Paid                   | Form + logic         | Trung bình  | 1.200.000         |
| F9  | Admin dashboard           | Quản lý người dùng, quiz, thống kê hệ thống         | UI quản trị          | Trung bình  | 1.000.000         |
| F10 | Email thông báo kết quả    | Gửi mail tự động sau khi làm quiz (Resend/Brevo)     | Không cần UI         | Dễ          | 500.000           |

---

## 3. MÔ HÌNH HỢP TÁC

### Option A – Trả theo từng chức năng (khuyến khích giai đoạn đầu)
- Mỗi module được giao task11. TRIỂN KHAI

> Xác nhận các chức năng ưu tiên để triển khai ngay:  
> - Chọn phương thức thanh toán: **Trả theo chức năng** hay **Chia doanh thu**.  
> - Sắp xếp thứ tự ưu tiên dựa trên milestone.  
> - Minh sẽ tổng hợp và tạo tài liệu hợp đồng, kanban công việc và tracking kết quả.

---
