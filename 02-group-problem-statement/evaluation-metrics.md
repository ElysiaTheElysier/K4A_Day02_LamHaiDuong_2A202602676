# Khung Đo Lường & Bộ Chỉ Số Đánh Giá: Hệ Thống Phân Bổ Nguồn Lực Doanh Nghiệp
## (Enterprise Resource Allocation & Capacity Planning System Metrics)

> **Dự án:** Hệ thống Phân bổ Nguồn lực & Giao việc thông minh theo Kỹ năng và Tải việc (Smart Resource & Task Allocation System)  
> **Áp dụng cho 2 luồng:** (1) Phân bổ task lẻ sau cuộc họp (*Micro-allocation*) và (2) Lập đội hình nhân sự cho dự án mới (*Macro-staffing*)  
> **Trạng thái tài liệu:** Khung kỹ thuật nghiệm thu & thẩm định hiệu quả thực tế (Evaluation Framework v2.0)

---

## 1. Tổng quan triết lý đo lường Phân bổ Nguồn lực (Resource Allocation Philosophy)

Một hệ thống phân bổ nguồn lực (Resource Allocation) thất bại nếu chỉ tối ưu một chiều:
- Nếu chỉ tối ưu **"Đúng kỹ năng" (Skill-fit)**: Các chuyên gia giỏi nhất sẽ bị quá tải (Burnout), trở thành điểm nghẽn duy nhất (*Single Point of Failure*), trong khi các nhân sự khác không có việc làm (*Underutilization*).
- Nếu chỉ tối ưu **"Ai đang rảnh thì giao" (Capacity-only)**: Công việc sẽ bị giao sai người, dẫn đến việc phải tìm hiểu lại từ đầu, làm lại (*Rework*), và trễ hạn bàn giao dự án.

Do đó, khung đo lường này thiết lập **bộ chỉ số cân bằng đa mục tiêu (Multi-Objective Optimization)** xoay quanh 4 trục:

```text
                                  [ TỐC ĐỘ PHÂN BỔ ]
                             (Staffing Lead Time / TTO)
                                        ▲
                                        │
           [ ĐỘ KHỚP NĂNG LỰC ] ◄───────┼───────► [ CÂN BẰNG TẢI VIỆC ]
           (Skill Fit Accuracy)         │         (Capacity & Utilization)
                                        ▼
                               [ AN TOÀN & BẢO MẬT ]
                               (RBAC & Zero Hallucination)
```

---

## 2. Bảng tổng hợp các chỉ số cốt lõi (Core Metrics Summary)

| Nhóm chỉ số | Tên chỉ số | Ký hiệu | Mục tiêu kỳ vọng (Target) | Bên chịu trách nhiệm |
|---|---|:---:|:---:|:---:|
| **Hiệu suất vận hành** | Thời gian phân bổ task từ meeting | **M-01: TTO** | **Giảm $\ge 30\%$** thời gian | Project Manager / Team Lead |
| | Thời gian lập đội hình dự án mới | **M-02: TTT** | **Giảm $\ge 30\%$** thời gian | Resource Manager / PM |
| | Tỷ lệ hoàn tất phân công trong 24h | **M-03: AC24** | **$\ge 95\%$** action item có owner | PM / Project Owner |
| | Tỷ lệ phải tái phân bổ (Re-allocation) | **M-04: RAR** | **Giảm $\ge 20\%$** so với baseline | Team Lead / Nhân sự |
| **Cân bằng tải việc** | Chỉ số tập trung quá tải chuyên môn | **C-01: OCI** | Giảm độ lệch tải việc $\ge 25\%$ | Resource Manager |
| | Tỷ lệ quá tải nhân sự (>100% capacity)| **C-02: OAR** | **$< 5\%$** tổng số nhân sự | PM / HR Lead |
| | Tỷ lệ xung đột lịch giữa các dự án | **C-03: CSC** | **$= 0$** sau khi chốt lịch | Resource Manager |
| **Độ khớp kỹ năng** | Độ chính xác ghép nối kỹ năng | **S-01: SMA** | **$\ge 85\%$** khớp năng lực | Tech Lead / Domain Expert |
| | Tỷ lệ ứng viên Top 3 được duyệt | **S-02: P@3** | **$\ge 80\%$** lần gợi ý | Project Manager |
| **Chất lượng AI** | Recall bóc tách Action Items/Roles | **A-01: AIR** | **$\ge 90\%$** (Critical $= 100\%$) | AI Engineer |
| | Trích xuất căn cứ thực tế (No Fake ID)| **A-02: HFR** | **$= 0\%$** bịa đặt dữ kiện | AI Engineer |
| **An toàn & Rào chắn** | Tự động giao việc trái phép | **G-01: UAA** | **Tuyệt đối $= 0$** | System Architect |
| | Vi phạm bảo mật & phân quyền RBAC | **G-02: RBV** | **Tuyệt đối $= 0$** | Security Officer |

---

## 3. Đặc tả chi tiết từng chỉ số đo lường

### Nhóm 1: Chỉ số Tốc độ & Hiệu quả Vận hành (Velocity & Operational Efficiency)

#### 1.1. `M-01: Meeting Time-to-Owner (TTO)` — Thời gian gán việc sau họp
* **Ý nghĩa:** Đo lường tốc độ chuyển đổi từ ghi chú cuộc họp (văn bản phi cấu trúc) thành các task có người nhận và deadline rõ ràng.
* **Công thức tính:**
  $$\text{TTO} = t_{\text{task\_approved}} - t_{\text{meeting\_ended}}$$
  *(Đo theo giá trị trung vị Median và phân vị P90 để loại bỏ ngoại lai)*.
* **Baseline cần đo:** Thời gian trung bình hiện tại khi Lead phải làm thủ công (thường mất 2–4 tiếng sau buổi họp).
* **Mục tiêu Pilot:** **Giảm $\ge 30\%$** thời gian so với baseline.

#### 1.2. `M-02: Project Time-to-Approved-Team (TTT)` — Thời gian chốt đội hình dự án
* **Ý nghĩa:** Đo lường thời gian từ lúc nhận Project Brief (yêu cầu dự án) đến khi danh sách đội hình (team roster) được Resource Manager và PM ký duyệt.
* **Công thức tính:**
  $$\text{TTT} = t_{\text{team\_approved}} - t_{\text{brief\_received}}$$
* **Mục tiêu Pilot:** **Giảm $\ge 30\%$** thời gian thương lượng và tìm kiếm nhân sự giữa các phòng ban.

#### 1.3. `M-04: Re-allocation Rate (RAR)` — Tỷ lệ phải đổi người sau phân công
* **Ý nghĩa:** Đo lường mức độ "chính xác ngay từ đầu". Nếu hệ thống giao nhầm người thiếu kỹ năng hoặc người đang quá tải, task sẽ bị từ chối hoặc phải đổi người (*Reassign*), gây lãng phí thời gian handoff.
* **Công thức tính:**
  $$\text{RAR} = \frac{N_{\text{reassigned}}}{N_{\text{total\_assigned}}} \times 100\%$$
* **Mục tiêu Pilot:** Giảm ít nhất **$20\%$ tương đối** so với cách giao việc cảm tính hiện tại.

---

### Nhóm 2: Chỉ số Cân bằng Tải việc & Chống Kiệt sức (Workload & Capacity Balance)

#### 2.1. `C-01: Overload Concentration Index (OCI)` — Chỉ số tập trung quá tải
* **Ý nghĩa:** Đo lường mức độ dồn việc vào số ít nhân sự có chuyên môn hiếm (ví dụ: công ty có 4 dự án nhưng chỉ có 3 chuyên gia Cloud/AI).
* **Công thức tính:**
  $$\text{OCI} = \frac{\sum \text{Effort giao cho nhóm nhân sự đang ở mức } > 100\% \text{ Capacity}}{\sum \text{Tổng effort của toàn bộ dự án}} \times 100\%$$
* **Mục tiêu Pilot:** **OCI giảm $\ge 25\%$**, hệ thống chủ động đề xuất giải pháp thay thế (chia nhỏ task, ghép cặp mentoring, hoặc cảnh báo capacity gap).

#### 2.2. `C-02: Over-allocation Rate (OAR)` — Tỷ lệ nhân sự quá tải
* **Ý nghĩa:** Tỷ lệ phần trăm nhân viên bị giao khối lượng công việc vượt quá số giờ làm việc tiêu chuẩn trong tuần (ví dụ: $> 40$ giờ/tuần hoặc $> 100\%$ capacity).
* **Công thức tính:**
  $$\text{OAR} = \frac{\text{Số nhân viên có } \text{Allocated Hours} > \text{Standard Capacity}}{\text{Tổng số nhân sự trong tổ chức}} \times 100\%$$
* **Ngưỡng kiểm soát (Threshold):** Duy trì **$< 5\%$** trong suốt thời gian diễn ra dự án.

#### 2.3. `C-03: Cross-Project Scheduling Conflict (CSC)` — Xung đột lịch chéo
* **Ý nghĩa:** Đo số trường hợp một nhân sự bị xếp lịch tham gia vào 2 deadline quan trọng hoặc 2 buổi release trùng giờ nhau ở 2 dự án khác nhau.
* **Ngưỡng bắt buộc:** **$= 0$** (Quy tắc deterministic rule trên hệ thống phải tự động chặn đứng xung đột này).

---

### Nhóm 3: Chỉ số Chất lượng Ghép nối Kỹ năng (Skill Matching & Placement Quality)

#### 3.1. `S-01: Skill Match Accuracy (SMA)` — Độ chính xác khớp kỹ năng
* **Ý nghĩa:** Đánh giá mức độ tương thích giữa bộ kỹ năng yêu cầu của task (Required Skills) với hồ sơ kỹ năng thực tế của nhân sự được phân công (Skill Profile).
* **Công thức tính:**
  $$\text{SMA} = \frac{1}{N} \sum_{i=1}^{N} \text{CosineSimilarity}(\vec{S}_{\text{task\_required}}, \vec{S}_{\text{employee\_verified}})$$
* **Mục tiêu Pilot:** Đạt điểm tương đồng ngữ nghĩa $\ge 0.85$ (tương đương $\ge 85\%$ mức độ khớp năng lực thực tế).

#### 3.2. `S-02: Top-3 Candidate Acceptance Precision (P@3)` — Tỷ lệ duyệt Top 3
* **Ý nghĩa:** Tỷ lệ các lần mà người quản lý (Lead/PM) chọn người thực hiện task nằm trong danh sách Top 3 ứng viên do AI đề xuất.
* **Công thức tính:**
  $$\text{P@3} = \frac{\text{Số lần người được chọn nằm trong Top 3 AI đề xuất}}{\text{Tổng số lần phân công}} \times 100\%$$
* **Mục tiêu Pilot:** Đạt **$\ge 80\%$**, chứng minh các đề xuất của AI có giá trị tham khảo thực tế cao, không vô nghĩa.

---

### Nhóm 4: Chỉ số Chất lượng AI & Trích xuất Dữ liệu (AI Extraction & Reasoning)

#### 4.1. `A-01: Action-Item & Role Extraction Recall`
* **Ý nghĩa:** Khả năng của LLM trong việc đọc meeting note/brief và bóc tách đầy đủ tất cả các đầu việc/vai trò cần làm mà không bị bỏ sót.
* **Công thức tính:**
  $$\text{Recall} = \frac{\text{Số action items AI tìm thấy đúng}}{\text{Tổng số action items thực tế do 2 chuyên gia thẩm định}} \times 100\%$$
* **Mục tiêu:** $\ge 90\%$ với các task thông thường; **$100\%$ đối với các task trọng yếu (Critical Action Items)**.

#### 4.2. `A-02: Hallucinated Fact Rate (HFR)` — Tỷ lệ ảo giác dữ kiện
* **Ý nghĩa:** Đảm bảo AI không tự bịa ra nhân sự không tồn tại, không tự chế deadline khi trong biên bản họp không đề cập, và không bịa ra kỹ năng chưa được kiểm chứng.
* **Ngưỡng bắt buộc:** **$= 0\%$**. Mọi dữ kiện suy luận thiếu nguồn đều bắt buộc phải được gắn tag `Unknown / Needs Clarification`.

---

### Nhóm 5: Rào chắn An toàn & Phân quyền (Guardrails & Security Zero-Tolerance)

* **`G-01: Unauthorized Auto-Assignment = 0`**: Tuyệt đối không cho phép AI tự động kích hoạt API giao task vào cơ sở dữ liệu khi chưa có thao tác bấm duyệt (*Explicit Click Approval*) của Project Manager.
* **`G-02: RBAC & Data Privacy Breach = 0`**: Hệ thống không bao giờ được phép gửi thông tin lương, đánh giá nhân sự cá nhân hoặc nội dung cuộc họp mật của dự án A sang cho PM của dự án B không có thẩm quyền.
* **`G-03: Hallucinated Employee ID = 0`**: Toàn bộ mã nhân viên (Employee ID) được đề xuất bắt buộc phải nằm trong snapshot dữ liệu nhân sự thật do Backend cung cấp.

---

## 4. Quy trình thu thập và nghiệm thu theo từng pha (Telemetry & Verification Plan)

```text
[BƯỚC 1: Thu thập Baseline (2 tuần đầu)]
  • Đo TTO thủ công: Ghi nhận thời gian kết thúc meeting và thời gian task xuất hiện trên Jira/Trello.
  • Đếm số task bị Reassign và phỏng vấn lý do đổi người (thiếu skill hay quá tải).
        ↓
[BƯỚC 2: Kiểm thử Offline trên Gold Dataset]
  • Chuẩn bị 20 meeting notes và 5 project briefs mẫu đã ẩn danh.
  • Chạy script đo lường Recall (A-01), Độ chính xác trích xuất (A-02) và Độ trễ gợi ý.
        ↓
[BƯỚC 3: Thử nghiệm Chế độ Bóng (Shadow Mode)]
  • Hệ thống âm thầm sinh đề xuất Top 3; PM vẫn phân công bằng tay như bình thường.
  • Đo chỉ số Agreement Rate: Tỷ lệ quyết định của PM trùng khớp với gợi ý của AI.
        ↓
[BƯỚC 4: Pilot Trực tiếp có Kiểm soát (Live Pilot)]
  • Áp dụng trên 1 team (khoảng 10–15 nhân sự, 2–3 dự án song song).
  • Đo toàn bộ các chỉ số TTO, TTT, Reassignment Rate và khảo sát độ hài lòng của nhân viên.
```

---

## 5. Tiêu chuẩn dừng khẩn cấp (Circuit Breaker Trigger)

Hệ thống phân bổ nguồn lực sẽ tự động **ngắt kết nối AI và quay về phân công thủ công hoàn toàn** nếu xảy ra một trong các điều kiện sau:
1. Phát hiện $\ge 1$ lỗi vi phạm bảo mật phân quyền (RBAC Breach) hoặc tự động giao task trái phép.
2. Tỷ lệ Reassignment Rate trong đợt Pilot cao hơn $15\%$ so với cách làm thủ công cũ.
3. Tỷ lệ Project Manager bấm nút từ chối toàn bộ danh sách gợi ý (`Reject All Recommendations`) vượt quá $40\%$ trong 10 phiên liên tiếp.
4. Ghi nhận phản ánh từ nhân sự về việc bị AI dồn việc quá tải liên tục mà không có sự kiểm duyệt của con người.

---

*Tài liệu đặc tả này cung cấp cơ sở định lượng vững chắc nhất để chứng minh giá trị kinh doanh (Business ROI) và tính an toàn của Hệ thống Phân bổ Nguồn lực trước hội đồng thẩm định.*
