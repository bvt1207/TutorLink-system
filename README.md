<!-- Banner -->
<p align="center">
  <a href="https://www.uit.edu.vn/" title="Trường Đại học Công nghệ Thông tin" style="border: none;">
    <img src="https://i.imgur.com/WmMnSRt.png" alt="Trường Đại học Công nghệ Thông tin | University of Information Technology">
  </a>
</p>

<h1 align="center"><b>PHÁT TRIỂN ỨNG DỤNG WEB</b></h>

## THÀNH VIÊN NHÓM

| STT |   MSSV   |              Họ và Tên |                  Email |
| --- | :------: | ---------------------: | ---------------------: |
| 1   | 23521410 |          Bùi Văn Thạch | 23521410@gm.uit.edu.vn |
| 2   | 23520527 |        Nguyễn Bá Hoàng | 23520527@gm.uit.edu.vn |
| 3   | 23520697 | Nguyễn Quốc Nhật Khang | 23520697@gm.uit.edu.vn |
| 4   | 23521393 |           Trần Hữu Tâm | 23521393@gm.uit.edu.vn |
| 5   | 23521449 |       Nguyễn Đắc Thành | 23521449@gm.uit.edu.vn |

## GIỚI THIỆU MÔN HỌC

- **Tên môn học:** Thiết kế hệ thống thương mại điện tử
- **Mã môn học:** EC312
- **Mã lớp:** EC312.Q11
- **Năm học:** HK1 (2025 - 2026)
- **Giảng viên**: ThS.Trình Trọng Tín

## Stocument-IS207.P21

Đồ án cuối kỳ môn Thiết kế hệ thống thương mại điện tử EC312.Q11 - thầy Trình Trọng Tín

# 🎓 TutorLink - E-Commerce System for Tutor Connection

[![School](https://img.shields.io/badge/UIT-University%20of%20Information%20Technology-blue)](https://www.uit.edu.vn/)
[![Role](https://img.shields.io/badge/Role-Product%20Owner%20%2F%20System%20Design-orange)](#)

## 📌 Tổng quan sản phẩm (Product Overview)

**TutorLink** là một nền tảng thương mại điện tử dịch vụ, giải quyết bài toán kết nối giữa Gia sư (Sinh viên) và Phụ huynh. Dự án tập trung vào việc minh bạch hóa chất lượng gia sư và tối ưu quy trình thanh toán, quản lý lớp học.

- **Vấn đề:** Phụ huynh khó tìm gia sư uy tín; Gia sư khó quản lý lịch dạy và học phí.
- **Giải pháp:** Hệ thống khớp lệnh (matching) thông minh, tích hợp ví điện tử và quản lý tiến độ học tập.

---

## 🛠 Tư duy hệ thống & Thiết kế (System Design)

### 1. Luồng nghiệp vụ chính (Critical User Journeys)

Hệ thống được thiết kế dựa trên 3 luồng chính:

- **Luồng kết nối:** Phụ huynh đăng yêu cầu -> Hệ thống gợi ý Gia sư -> Phỏng vấn & Chốt lớp.
- **Luồng tài chính:** Nạp tiền -> Giữ tiền hộ (Escrow) -> Giải ngân sau mỗi buổi học/tháng.
- **Luồng kiểm soát:** Admin xác thực bằng cấp/CCCD của gia sư trước khi cho phép hoạt động.

### 2. Mô hình dữ liệu (ERD)

Hệ thống quản lý các thực thể phức tạp bao gồm:

- **Users & Profiles:** Phân quyền đa vai trò (Parent, Tutor, Admin).
- **Transactions:** Lưu vết lịch sử nạp/rút và thanh toán lớp học.
- **Course Management:** Quản lý trạng thái lớp (Pending, Ongoing, Completed).

---

## ✨ Tính năng nổi bật (Key Features)

| Tính năng                   | Mô tả cho Nhà tuyển dụng                                            |
| :-------------------------- | :------------------------------------------------------------------ |
| **Hệ thống ví điện tử**     | Quản lý số dư, xử lý giao dịch an toàn giữa phụ huynh và gia sư.    |
| **Matching Logic**          | Bộ lọc thông minh theo khu vực, môn học và mức giá.                 |
| **Bảng điều khiển (Admin)** | Theo dõi chỉ số tăng trưởng (Số lớp mới, Doanh thu, Tỷ lệ hủy lớp). |
| **Xác thực hồ sơ**          | Quy trình phê duyệt nghiêm ngặt để đảm bảo chất lượng đầu vào.      |

---

## 💻 Công nghệ sử dụng

- **Backend:** Node.js, Express.js (Xử lý logic nghiệp vụ và API).
- **Frontend:** React.js, Tailwind CSS (Tối ưu trải nghiệm người dùng cuối).
- **Database:** MongoDB (Lưu trữ linh hoạt thông tin hồ sơ và giao dịch).

---

## 📂 Cấu trúc dự án

```text
├── backend/            # Business Logic & System Architecture
│   ├── models/         # Cấu trúc thực thể dữ liệu (Core Logic)
│   ├── controllers/    # Xử lý luồng nghiệp vụ
│   └── routes/         # Hệ thống Endpoints của sản phẩm
└── frontend/           # Interface & User Experience
```
