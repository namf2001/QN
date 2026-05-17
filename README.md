# 🏥 B2B Website Sales Consultant - Agent Skill & SEO Guide

Chào mừng bạn đến với Repository dự án **QN**. Dự án hiện đã được tích hợp bộ kỹ năng **B2B Website Sales Consultant (b2b-web-sales)** giúp Agent tự động hóa quy trình phân tích website khách hàng, xây dựng bộ từ khóa SEO chuyển đổi (chuyên biệt cho ngách Y tế/YMYL) và soạn thảo tài liệu chốt sale sắc bén.

---

## 📂 Cấu Trúc Bộ Skill (Folder `.agents/skills/b2b-web-sales`)

Bộ kỹ năng được thiết kế theo nguyên lý **Progressive Disclosure** để tối ưu hóa ngữ cảnh và tốc độ xử lý của Agent:

```
.agents/skills/b2b-web-sales/
├── SKILL.md                 # Trọng tâm chính, định nghĩa Quy trình 4 bước chốt sale.
└── references/
    ├── keyword-framework.md  # Công thức chấm điểm & lọc từ khóa chuyển đổi (YMYL).
    ├── seo-plan-template.md  # Kế hoạch SEO mẫu (Tuyến tiền liệt & Són tiểu).
    └── outreach-templates.md # Mẫu Proposal, Kịch bản gọi điện & Cold Email.
```

---

## 🛠️ Hướng Dẫn Sử Dụng Bộ Skill Cho Agent

Khi chat với Agent (Antigravity hoặc các Agent tương thích), bạn có thể kích hoạt bộ kỹ năng này bằng các câu lệnh (prompts) đơn giản theo cấu trúc dưới đây:

### 1. Phân tích đối thủ / Khách hàng tiềm năng (Audit & Pitch)
Để yêu cầu Agent quét và chỉ ra lỗi trên web cũ của khách hàng nhằm mục đích chào hàng làm lại web:
> **Prompt:** *"Hãy chạy quy trình b2b-web-sales để phân tích website của đối thủ `[tên_miền_đối_thủ]` (hoặc website khách hàng `[tên_miền_của_khách]`). Hãy chỉ ra các lỗi UI/UX di động và lỗi SEO E-E-A-T của họ."*

### 2. Tạo Kế hoạch SEO & Bộ từ khóa chuyển đổi (Keyword Strategy)
Để yêu cầu Agent tạo bảng từ khóa vàng kèm điểm ưu tiên dựa trên công thức chấm điểm:
> **Prompt:** *"Hãy lập kế hoạch SEO tổng thể và bảng từ khóa ngách cho bệnh lý `[Tên_Bệnh_Lý]` tại khu vực `[Tỉnh_Thành]`. Áp dụng công thức chấm điểm YMYL Keyword Scoring từ skill b2b-web-sales."*

### 3. Soạn tài liệu chốt sale (Outreach Package)
Để Agent soạn kịch bản gọi điện thoại hoặc viết email tiếp cận Giám đốc/Trưởng phòng Marketing phòng khám:
> **Prompt:** *"Hãy viết một Cold Email và một kịch bản Telesale sắc bén chào hàng dịch vụ nâng cấp Website cho phòng khám `[Tên_Phòng_Khám]`. Nhấn mạnh vào dịch vụ nổi bật `[Tên_Dịch_Vụ]` của họ và xử lý từ chối khi họ nói 'đã có web chạy ổn rồi'."*

---

## 📐 Nguyên Tắc Chiến Lược Cốt Lõi (Cần Ghi Nhớ)

Khi tư vấn làm lại website cho phòng khám, luôn hướng Agent tuân thủ 3 nguyên tắc:
1.  **Bán giải pháp chuyển đổi, không bán giao diện:** Trọng tâm thuyết phục là tăng tỉ lệ bệnh nhân đặt lịch hẹn (CRO).
2.  **Công thức chấm điểm từ khóa chuyển đổi:**
    $$\text{Điểm Ưu Tiên} = (\text{Volume} \times 10\%) + (\text{Intent} \times 50\%) + (\text{KD đảo ngược} \times 40\%)$$
3.  **Tâm lý học hành vi y tế:**
    *   *Bệnh lý nam giới (Tuyến tiền liệt...):* Giao diện cần thể hiện rõ thông tin Bác sĩ uy tín (E-E-A-T), giọng điệu nội dung **quyết đoán, khoa học**.
    *   *Bệnh lý nhạy cảm (Són tiểu...):* Cần widget **đăng ký ẩn danh riêng tư** trên di động, giọng điệu nội dung **thấu hiểu, đồng cảm**.
