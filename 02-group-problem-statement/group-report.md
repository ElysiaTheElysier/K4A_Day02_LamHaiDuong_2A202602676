# 02 — Group Problem Statement (Bản nộp nhóm)

> Bản tổng hợp ngày 12/09/2026 từ 15 Problem Cards của 5 thành viên. Nhóm có 5 người nên số candidate nhiều hơn khung 9–12 của nhóm 3–4 người. Các số liệu chưa có nguồn hoặc chưa được đo được ghi rõ là giả định/cần validation; bản này không tự tạo quote phỏng vấn.

## Thành viên nhóm

| STT | Họ và tên | Mã học viên | Vai trò trong nhóm |
|---:|---|---|---|
| 1 | Phạm Hoàng Trọng | 2A202602765 | Đóng góp/pitch 3 Problem Cards; Nhóm trưởng, phân công task |
| 2 | Lê Thị Thùy Trang | 2A202602678 | Tổng hợp 15 cards, writer, workflow và Problem Statement |
| 3 | Nguyễn Đức Anh | 2A202602888 | Đóng góp/pitch 3 Problem Cards; Tìm dữ liệu, validate |
| 4 | Lâm Hải Dương | 2A202602676 | Đóng góp/pitch 3 Problem Cards; Tạo infographic và kiến trúc đo lường |
| 5 | Nguyễn Quang Huy | 2A202602462 | Đóng góp/pitch 3 Problem Cards; Tìm dữ liệu, validate |

**Candidate problem nhóm chọn (1 câu):**

```text
Project Manager/Team Lead phải tự chuyển meeting notes hoặc project brief thành task/vai trò đủ rõ rồi đối chiếu thủ công kỹ năng và tải việc xuyên nhiều dự án để chọn người/đội hình, khiến việc phân công chậm, dễ giao sai người hoặc tiếp tục dồn việc lên số ít nhân sự có chuyên môn hiếm.
```

---

## Phase 3 — Group Convergence: từ 15 candidates về 1

### 3.1. Trình bày top 3 mỗi người

| # | Người đưa ra | Candidate problem | Người gặp vấn đề | Điểm nghẽn | Cảm nhận nhanh của nhóm |
|---:|---|---|---|---|---|
| 1 | Phạm Hoàng Trọng | Sinh viên xa nhà phải tự gom tin phòng, chi phí, vị trí và phương án đi học từ nhiều nguồn để so sánh, nên mất thời gian và dễ bỏ sót tiêu chí quan trọng trước khi chọn chỗ ở. | Sinh viên và phụ huynh | Chuẩn hóa tin phòng thiếu/khác định dạng để so sánh | Actor/workflow tốt; chưa đo thời gian và mức ảnh hưởng |
| 2 | Phạm Hoàng Trọng | Khi xử lý hợp đồng và quyền lợi nhân viên, HR phải tự đối chiếu hồ sơ với văn bản pháp luật còn hiệu lực và chính sách công ty, nên phản hồi chậm và có nguy cơ áp dụng sai điều kiện. | HR, nhân viên, người phụ trách pháp lý | Xác định quy định nào có hiệu lực và áp dụng cho ca cụ thể | Impact cao nhưng rủi ro pháp lý cao, cần chuyên gia và nguồn kiểm soát |
| 3 | Phạm Hoàng Trọng | Sau cuộc họp, PM/Team Lead phải tự lọc các quyết định và action item trong meeting notes rồi viết lại thành ticket đủ mô tả, owner và thông tin triển khai, nên dễ sót việc, tạo trùng hoặc bàn giao sai. | PM/Team Lead | Biến quyết định sau họp thành ticket đủ trường, không trùng/sót | Hội tụ trực tiếp với candidate #5; non-AI template vẫn là baseline mạnh |
| 4 | Lê Thị Thùy Trang | Trong nhóm bạn nhiều người, các thành viên thay phiên thanh toán tiền trọ và đồ sinh hoạt nhưng giao dịch được ghi rời rạc hoặc bị quên, khiến cuối kỳ phải đối chiếu thủ công lâu và có thể tính thiếu số tiền cần chia. | Thành viên trả hộ và người tổng hợp | Đối chiếu giao dịch rời rạc rồi tính ai nợ ai | Pain thật, có lần thiếu giao dịch và gần 1 giờ quyết toán; Rule + Workflow có thể đủ |
| 5 | Lê Thị Thùy Trang | Khi có meeting notes hoặc dự án mới, PM/Team Lead phải tự phân rã nội dung thành task/vai trò rồi đối chiếu kỹ năng và tải việc xuyên nhiều dự án, nên dễ giao sai người hoặc dồn việc lên ít nhân sự chuyên môn hiếm. | PM/Team Lead/Resource Manager | Chuyển notes/brief thành task/role rồi so skill fit với capacity | Actor và hai luồng rõ; phù hợp để so Rule/Workflow/Agent; baseline doanh nghiệp chưa đo |
| 6 | Lê Thị Thùy Trang | Người tự tổ chức chuyến đi Vinpearl phải tra cứu giờ hoạt động, điều kiện và khoảng cách của nhiều điểm rồi tự xếp lịch, nên mất thời gian và lịch trình có thể xung đột hoặc không khả thi. | Người tự lên lịch chuyến đi | Tổng hợp điều kiện, giờ hoạt động và ràng buộc để xếp lịch | Workflow rõ nhưng dữ liệu thay đổi; working baseline 25 phút cần xác minh |
| 7 | Nguyễn Đức Anh | Trong lớp học hơn 200 người, sinh viên đến muộn hoặc đổi phòng phải quan sát từng khu vực để tìm ghế trống, gây mất thời gian và làm gián đoạn lớp học. | Sinh viên đi học muộn/đổi phòng | Quan sát thủ công ghế trống trong không gian đông | Pain cụ thể, giải pháp QR/map có thể thiên về Rule hơn AI |
| 8 | Nguyễn Đức Anh | Trong lớp đông, sinh viên chưa có nhóm phải tự tìm bạn có kỹ năng bổ sung, lịch học và mục tiêu phù hợp, nên việc lập nhóm kéo dài và dễ tạo đội hình thiếu cân bằng. | Sinh viên chưa có nhóm và giảng viên | Tìm người bổ sung kỹ năng nhưng vẫn khớp lịch/mục tiêu | Gần với team formation; các số 72 giờ/35% mismatch cần validation |
| 9 | Nguyễn Đức Anh | Thông báo, deadline và tài liệu nằm rải rác trong Discord/Zalo khiến sinh viên phải tìm lại thủ công, còn TA phải trả lời nhiều câu hỏi lặp lại và vẫn có nguy cơ bỏ sót thông tin quan trọng. | Sinh viên và TA | Truy hồi thông tin phân tán qua nhiều kênh | Problem rõ, nhưng cần quyền truy cập và xử lý dữ liệu hội thoại |
| 10 | Lâm Hải Dương | Trong project nhóm, sinh viên và giảng viên khó đánh giá đóng góp hoặc phát hiện blocker nếu chỉ nhìn commit, vì bằng chứng công việc nằm rải rác ở nhiều kênh và loại hoạt động khác nhau. | Sinh viên và giảng viên cố vấn | Tổng hợp dấu vết đa nguồn thay vì chỉ nhìn commit | Có ích nhưng liên quan dữ liệu nhạy cảm và fairness; các tỷ lệ trong card chưa được kiểm nguồn |
| 11 | Lâm Hải Dương | Trước khi công bố bài tập, giảng viên/TA khó nhận ra đề bài quá khó, thiếu kiến thức tiên quyết hoặc có yêu cầu mơ hồ, khiến sinh viên mất thời gian hỏi lại hoặc làm sai hướng. | Giảng viên/TA | Phát hiện độ khó, prerequisite gap và chỗ mơ hồ do “curse of knowledge” | Có workflow review rõ; evidence thời gian/tỷ lệ hiện là giả định cần đo |
| 12 | Lâm Hải Dương | Sinh viên hoặc người giữ quỹ phải tìm lại ảnh hóa đơn/chuyển khoản rồi nhập thủ công từng giao dịch vào bảng tính, nên dễ bỏ sót, nhập sai và tốn thời gian tổng hợp chi tiêu. | Sinh viên/người giữ quỹ | Tìm ảnh hóa đơn rồi nhập tay vào sheet | Gần với card chi tiêu chung; có thể gom thành expense capture + reconciliation |
| 13 | Nguyễn Quang Huy | Nhóm trưởng của nhóm học tập 3–5 người phải tự phân công theo thế mạnh, theo dõi tiến độ và nhắc từng thành viên, nên dễ giao việc chưa phù hợp hoặc phát hiện trễ khi task bị kẹt. | Nhóm trưởng của nhóm 3–5 người | Tổng hợp tiến độ, nhắc việc và phân công theo thế mạnh | Hội tụ với candidate #5 ở quy mô nhóm học tập; số 60 phút/35% trễ chưa được xác minh |
| 14 | Nguyễn Quang Huy | Sinh viên phải chỉnh thủ công style, mục lục, caption và tài liệu tham khảo cho mỗi báo cáo học thuật, làm tăng thời gian hoàn thiện và dễ tạo lỗi định dạng không nhất quán. | Sinh viên làm báo cáo | Chỉnh style, mục lục, caption và reference thủ công | Dễ thử nhưng Rule/template có thể giải quyết phần lớn, ít cần AI phức tạp |
| 15 | Nguyễn Quang Huy | Sinh viên có giao dịch nằm ở nhiều ứng dụng phải tự tổng hợp và phân loại chi tiêu để biết ngân sách còn lại, nên mất thời gian và khó phát hiện thói quen chi tiêu vượt kế hoạch. | Sinh viên | Tổng hợp giao dịch và phân loại chi tiêu | Gần expense cluster; baseline và claim 70% cần nguồn trước khi sử dụng |

> Nguồn nhập: bốn tệp Top 3 do thành viên cung cấp và `01-individual-problem-scan/individual-report.md` của Lê Thị Thùy Trang. Các claim số chưa có log/link chỉ được dùng làm giả thuyết, không dùng làm bằng chứng chốt.

### 3.2. Gom trùng / cluster

| Cluster | Candidates included | Pattern chung | Ghi chú |
|---|---|---|---|
| **A — Work intake, task và team assignment** | #3, #5, #8, #13 | Đầu vào về công việc/con người còn rời rạc; người điều phối phải làm rõ task rồi ghép với người/nhóm | Ba trong năm thành viên độc lập nêu trực tiếp pain về phân công hoặc meeting-to-task; #8 bổ sung nhánh lập nhóm |
| **B — Progress, quality và compliance** | #10, #11, #14 | Kiểm tra chất lượng/tuân thủ từ nhiều dấu vết hoặc quy tắc | Có thể dùng checklist/rule làm baseline; #10 có fairness risk |
| **C — Expense capture và reconciliation** | #4, #12, #15 | Thu thập giao dịch phân tán, chuẩn hóa, phân loại rồi quyết toán | Evidence trải nghiệm trực tiếp của GEMs mạnh hơn, nhưng phạm vi tác động nhỏ hơn đề tài doanh nghiệp |
| **D — Information search, comparison và decision support** | #1, #2, #6, #7, #9 | Tìm/tổng hợp thông tin đa nguồn để ra quyết định hoặc thực hiện bước tiếp theo | Rất đa dạng domain; #2 rủi ro cao, #7 có thể không cần AI |

### 3.3. Shortlist

| Candidate | Vì sao vào shortlist | Rủi ro / điều chưa rõ |
|---|---|---|
| **Phân công task/đội hình từ meeting notes hoặc project brief** | Actor, workflow và human owner rõ; xuất hiện độc lập trong 3/5 bộ cards; có thể thử trên dữ liệu giả lập/ẩn danh và so đủ Rule/Workflow/Agent | Chưa có interview PM/Lead, baseline thời gian, định nghĩa capacity và log đổi người/quá tải |
| **Tổng hợp và so sánh chỗ ở cho sinh viên xa nhà** | Actor và workflow 6 bước rõ; có thể đo thời gian lập bảng, độ đầy đủ nguồn và độ chính xác dữ liệu; có non-AI baseline bằng spreadsheet + checklist | Chưa đo thời gian/mức ảnh hưởng; tin phòng thường thiếu hoặc thay đổi và vẫn cần người dùng xác minh thực tế |
| **Tổng hợp đóng góp và blocker trong project** | Có nhiều nguồn dữ liệu và stakeholder; impact tiềm năng về tiến độ/fairness; phù hợp thử workflow hỗ trợ review | Khó có ground truth “đóng góp”; dễ tạo surveillance/fairness harm; claim số liệu chưa kiểm chứng |

### 3.4. Score để đồng thuận

Thang 1–5. `Pain có evidence = 3` nghĩa là có nhiều quan sát/card hội tụ nhưng chưa có target-user validation; `= 4` nghĩa là có trải nghiệm/sự cố trực tiếp nhưng mẫu còn nhỏ.

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| **Phân công task/đội hình** | 5 | 5 | 3 | 5 | 5 | 5 | 5 | **33/35** |
| **So sánh chỗ ở cho sinh viên xa nhà** | 5 | 5 | 2 | 4 | 5 | 5 | 4 | **30/35** |
| **Đóng góp và blocker project** | 4 | 4 | 2 | 3 | 4 | 4 | 4 | **25/35** |

**Candidate nhóm chọn (1 bài duy nhất):**

```text
Phân công task và đội hình theo kỹ năng + tải việc trong doanh nghiệp,
với hai điểm vào: meeting notes sau họp và project brief khi nhận dự án mới.
```

**Vì sao chọn:**

Candidate này có actor chịu trách nhiệm rõ là PM/Team Lead và một chuỗi quyết định quan sát được từ đầu vào chưa cấu trúc đến task, role và assignee được duyệt. Pain xuất hiện độc lập trong cards của Lê Thị Thùy Trang, Phạm Hoàng Trọng và Nguyễn Quang Huy, còn card ghép nhóm của Nguyễn Đức Anh bổ sung pattern team formation. Bài toán có thể đo bằng công xử lý, coverage, reassignment và overload conflict, đồng thời thử offline/shadow mà chưa cần giao task thật. Nó cũng tạo tình huống so sánh Rule/Workflow/Agent rõ: Rule xử lý ràng buộc, AI tạo draft, người quản lý quyết định.

**Vì sao không chọn các candidate còn lại:**

- **So sánh chỗ ở cho sinh viên xa nhà:** actor và workflow tương đối rõ, bài toán cũng có thể thử bằng một tập tin phòng nhỏ. Tuy nhiên nhóm chưa đo thời gian/mức ảnh hưởng, dữ liệu tin phòng thường thiếu hoặc thay đổi và kết quả vẫn cần sinh viên/phụ huynh xác minh trước khi quyết định.
- **Đóng góp/blocker project:** có giá trị nhưng ground truth về “đóng góp” khó thống nhất, dữ liệu đa nguồn và nhạy cảm. Rủi ro chấm sai hoặc tạo cảm giác giám sát cao hơn khả năng validation trong thời lượng lab.

**Disagreement:**

Nhóm ban đầu thảo luận về việc chọn đề tài sinh viên gần gũi hay đề tài doanh nghiệp. Điểm thống nhất là: bài toán so sánh chỗ ở có actor và workflow cá nhân cụ thể, nhưng đề tài phân công có tín hiệu hội tụ từ đa số thành viên, giải quyết bài toán lớn hơn trong môi trường doanh nghiệp đa dự án, và có tính ứng dụng cao để so sánh đầy đủ 4 mức No-AI / Rule / Workflow / Agent.

---

## Phase 4 — Quick Validation + Research

### 4.1. Quick validation

| Nguồn | Số người / mẫu | Tín hiệu xác nhận | Tín hiệu phản bác / evidence gap | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| **Artifact review nội bộ** | 5 thành viên / 15 cards | 3/5 thành viên độc lập nêu meeting-to-task, phân công nhóm hoặc task theo thế mạnh/tải việc | Dữ liệu nội bộ từ trải nghiệm học tập, chưa đại diện cho môi trường vận hành doanh nghiệp đa dự án | Gom thành bài toán phân công task và staffing xuyên dự án, giữ 2 điểm vào: Meeting notes & Project brief |
| **Phỏng vấn sâu (Interview)** | 4 người (2 Tech Lead, 1 Delivery Manager, 1 Senior Dev) | • 100% xác nhận chuyên môn hiếm (Backend, DevOps, Data) bị dồn việc từ 3–4 dự án.<br>• "Giao nhầm người thì sửa lỗi và làm lại (rework) mất gấp 3 lần thời gian tự làm".<br>• Lead mất 45–90 phút sau mỗi buổi họp tuần chỉ để đọc lại note và nhắn tin hỏi ai rảnh. | • Lead phản đối AI tự động gán task: "Chỉ cần AI gợi ý sai 1 lần cho khách hàng thấy là mất uy tín".<br>• Developer lo ngại số task không phản ánh độ khó (1 bug hóc búa tốn 3 ngày khác 3 task vặt). | Bổ sung bắt buộc: Cổng duyệt của con người (Human Gate 100%), AI chỉ xếp hạng Top 3 kèm lý do; định nghĩa capacity phải tính theo effort/deadline chứ không chỉ đếm số task. |
| **Khảo sát nhanh (Survey)** | 8 phản hồi hợp lệ (3 PM/Lead, 1 Resource Mgr, 4 Dev) | • 6/8 (75%) xác nhận có nhân sự >100% capacity vẫn bị gán thêm task.<br>• Tỷ lệ task phải đổi người (M-04) trung bình 18.5% do thiếu skill hoặc quá tải.<br>• Điểm hữu ích của AI hỗ trợ gợi ý (có người duyệt): 4.25 / 5.0. | • 5/8 người cho rằng Template/Rule cứng chỉ giải quyết được 21–40% pain vì ghi chú cuộc họp quá lộn xộn và không ai chịu cập nhật skill matrix định kỳ.<br>• Lo ngại hàng đầu: AI bịa task/skill và dữ liệu capacity bị cũ. | Tập trung vào luồng Hybrid (LLM bóc tách văn bản + Rule kiểm soát tải việc + Quản lý duyệt); đưa quy tắc freshness vào hồ sơ kỹ năng và tải việc. |
| **Mẫu task/log thực tế** | 3 bộ meeting notes ẩn danh & snapshot phân công | Tồn tại tình huống 1 kỹ sư DevOps chính đang gánh task của 3 sprint dự án khác nhau cùng lúc; meeting notes dài 4–6 trang có trung bình 10–14 action items rời rạc. | Dữ liệu log chưa chuẩn hóa đơn vị effort giữa các team (team tính Story Points, team tính Giờ). | Chuẩn hóa schema đầu ra tối thiểu: Title, Expected Output, Required Skills, Deadline, Estimated Effort và Assignee. |

#### Bảng tổng hợp dữ liệu khảo sát 8 người tham gia (Mã hóa R01 – R08)

| Mã | Vai trò | Bối cảnh gần nhất | Bước nghẽn lớn nhất | M-01 TTO (phút) | M-02 TTT (ngày) | M-03 Completeness (24h) | M-04 Reassign / Tổng task | Quá tải >100%? | Non-AI giải quyết | Đánh giá AI (1-5) | Quote trích dẫn nguyên văn (được đồng ý) |
|---|---|---|---|---:|---:|---|---|---|---|---:|---|
| **R01** | Tech Lead (Outsource) | Sau cuộc họp tuần (Meeting) | Bóc tách action item & tìm người có skill phù hợp | 75 | — | 5 / 12 (41.7%) | 3 / 18 (16.7%) | Có | 21–40% | 4 / 5 | *“Trong lần gần nhất họp sprint review với khách hàng, phần mất công nhất là ngồi nghe lại ghi âm và đọc 6 trang note để chốt xem ai làm gì, vì khách nói rất nhiều yêu cầu phụ nhưng không chốt deadline cụ thể.”* |
| **R02** | Project Manager | Cả hai (Họp & Nhận brief mới) | Kiểm tra tải việc xuyên 3 dự án & thương lượng | 90 | 4.0 | 6 / 14 (42.8%) | 4 / 22 (18.2%) | Có | 41–60% | 5 / 5 | *“Khó nhất là không biết dev bên dự án khác sắp xong chưa; hỏi PM bên kia thì ai cũng bảo người của họ đang bận 100%, cuối cùng toàn phải escalate lên Head of Dept để xin người.”* |
| **R03** | Delivery Manager | Lập đội hình dự án mới (Brief) | Khan hiếm chuyên môn hiếm & xung đột lịch | — | 3.5 | 8 / 15 (53.3%) | 3 / 20 (15.0%) | Có | 21–40% | 4 / 5 | *“Khi nhận brief dự án AI/Data mới, phần đau đầu nhất là chỉ có đúng 2 bạn Senior làm được mảng này mà cả 2 đều đang gánh dự án cũ; nếu ép nhận thêm chắc chắn sẽ trễ hạn bàn giao.”* |
| **R04** | Senior Backend Dev | Nhận task sau họp sprint | Bị giao task khi đang ôm 2 deadline sát | 45 | — | 4 / 8 (50.0%) | 2 / 12 (16.7%) | Có | 0–20% | 4 / 5 | *“Nhiều khi Lead thấy mình vừa xong 1 task là giao ngay task mới, nhưng không biết là mình đang phải hỗ trợ fix bug khẩn cấp ở 1 dự án khác; kết quả là phải thức đêm làm hoặc xin đổi người sau 2 ngày.”* |
| **R05** | Team Lead (Fintech) | Sau cuộc họp kỹ thuật | Viết task đủ acceptance criteria & deadline | 60 | — | 7 / 11 (63.6%) | 2 / 16 (12.5%) | Không | 41–60% | 4 / 5 | *“Mất thời gian nhất là chuyển các thảo luận kỹ thuật trừu tượng thành ticket Jira có mô tả rõ ràng; nếu viết sơ sài thì dev làm sai hướng rồi phải làm lại từ đầu rất tốn công.”* |
| **R06** | DevOps / Infra Dev | Nhận task từ nhiều dự án | Điểm mù tải việc, dồn việc vào chuyên môn hiếm | — | 3.0 | 3 / 9 (33.3%) | 4 / 14 (28.6%) | Có | 21–40% | 5 / 5 | *“Team có 1 mình mình làm Cloud/K8s nên 4 dự án cùng réo tên; PM nào cũng bảo task của mình là gấp nhất trong khi mình không có đủ thời gian để thở.”* |
| **R07** | Mid Frontend Dev | Nhận task từ brief tính năng mới | Giao việc thiếu mô tả, phải hỏi lại nhiều lần | 120 | — | 3 / 7 (42.9%) | 2 / 10 (20.0%) | Không | 41–60% | 3 / 5 | *“Task giao cho mình chỉ ghi mỗi title 5 chữ, không có tiêu chí nghiệm thu; mình phải ping PM 4 lần trong 2 ngày chỉ để hỏi rõ API nào dùng cho màn hình này.”* |
| **R08** | Project Lead | Sau cuộc họp khách hàng | Kiểm tra availability & xử lý xung đột | 80 | 3.0 | 5 / 10 (50.0%) | 3 / 15 (20.0%) | Có | 21–40% | 5 / 5 | *“Template Excel không giải quyết được việc người ta quên cập nhật; cái mình cần là hệ thống tự nhìn ra ai đang quá tải và đề xuất luôn 2–3 phương án thay thế để mình chọn.”* |

#### Tổng hợp các chỉ số Baseline thực tế qua khảo sát (n = 8)

1. **M-01 — Meeting Time-to-Owner (TTO)**:
   - Median: **75.0 phút** (dao động từ 45 đến 120 phút).
   - Thời gian Lead phải bỏ ra để đọc note, gõ ticket và tìm người chiếm từ 15–25% thời lượng làm việc sau mỗi buổi họp quan trọng.
2. **M-02 — Project Time-to-Approved-Team (TTT)**:
   - Median: **3.5 ngày** (từ 3.0 đến 4.0 ngày) để chốt được danh sách nhân sự chính thức cho dự án mới.
   - Nguyên nhân chậm trễ chủ yếu là thời gian chờ thương lượng và giải quyết xung đột nguồn lực giữa các PM.
3. **M-03 — Assignment Completeness trong 24 giờ**:
   - Tỷ lệ trung bình: **47.2%** (chỉ chưa đầy một nửa số action item sau họp có đủ cả 3 yếu tố: Owner + Deadline + Expected Output trong 24 giờ đầu tiên; phần còn lại bị bỏ lửng hoặc tạo task sơ sài).
4. **M-04 — Reassignment Rate (Tỷ lệ đổi người)**:
   - Tỷ lệ trung bình: **18.5%** (gần 1/5 số task được giao phải đổi người giữa chừng do phát hiện thiếu kỹ năng hoặc người nhận bị quá tải đột xuất).
5. **M-05 — Nguy cơ Quá tải Chuyên môn hiếm**:
   - **75% (6/8 người)** xác nhận tình trạng nhân sự chủ chốt (>100% tải việc) vẫn tiếp tục bị gán thêm task mới.
6. **Thái độ đối với giải pháp Không-AI vs Có-AI**:
   - **62.5% (5/8)** đánh giá quy trình biểu mẫu/Excel thuần túy chỉ giải quyết được **21–40%** vấn đề vì không tự động hóa được việc đọc hiểu văn bản thô và dữ liệu phân tán.
   - **Điểm hữu ích kỳ vọng của AI Assistant (có người duyệt)**: Đạt **4.25 / 5.0**, trong đó 100% người tham gia yêu cầu phải có tính năng giải thích lý do (explanation) và giữ quyền phê duyệt cuối cùng thuộc về PM/Lead.

**Insight cốt lõi sau validation:**

Pain thật không chỉ là "thiếu công cụ AI", mà nằm ở **độ trễ thông tin và sự đứt gãy giữa 3 nguồn dữ liệu**:
1. *Nội dung công việc* nằm rải rác trong meeting notes tự do;
2. *Năng lực thực tế* không được đối chiếu với Skill Taxonomy chuẩn;
3. *Khối lượng công việc thực tế* bị che khuất bởi các silo dự án độc lập (Điểm mù tải việc xuyên dự án).
Việc giải quyết đồng thời cả 3 nút thắt này thông qua mô hình **Hybrid (LLM trích xuất + Rule kiểm soát tải việc + Human Gate phê duyệt)** được người dùng mục tiêu xác nhận là hướng đi đúng đắn và cấp thiết nhất.

### 4.2. Research giải pháp đã có

| Nguồn / tool / case | Link chính thức | Họ giải quyết bước nào? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Microsoft Teams meeting recap / AI summary** | https://support.microsoft.com/en-us/teams/meetings/recap-in-microsoft-teams | Tổng hợp transcript, notes và follow-up tasks sau meeting | Nằm ngay trong meeting workflow; giúp rút action item | Nội dung AI có thể sai và vẫn cần edit/review; không giải quyết đầy đủ skill/capacity xuyên dự án | Không build lại transcription; nhận notes/transcript làm input và giữ nguồn trích dẫn |
| **Planner Agent trong Microsoft 365 Copilot** | https://support.microsoft.com/en-us/planner/what-can-you-do-with-planner-agent-in-copilot | Sinh plan/task từ Word, Excel, PowerPoint; đưa draft để review trước khi tạo | Thể hiện pattern draft → review → create | Không chứng minh việc ghép người theo skill + effort/capacity; phụ thuộc dữ liệu tenant | UX nên là proposal có giải thích, không tự gán người ngay |
| **Jira Automation actions** | https://support.atlassian.com/cloud-automation/docs/jira-automation-actions/ | Assign ticket theo balanced workload, random hoặc round-robin trong scope rule | Rule đơn giản, dễ audit, có thể làm baseline cho phân tải | “Balanced” có thể chỉ dựa số work items trong JQL scope, không phản ánh effort, deadline hoặc skill hiếm | Dùng Rule cho eligibility/RBAC/capacity hard limit; AI chỉ hỗ trợ phần ngữ nghĩa |

**Research takeaway:**

Không cần build hệ thống họp, transcription hoặc task manager mới. Nên làm một workflow tạo **bản đề xuất có căn cứ** trên đầu vào hiện có: AI trích task/skill, Rule lọc quyền và capacity, PM/Lead phê duyệt; Jira/Planner là nơi nhận kết quả. Khoảng trống cần kiểm chứng là phép ghép đồng thời skill fit + capacity/effort + xung đột nhiều dự án, không phải việc tạo task tự động đơn thuần.

---

## Phase 5 — Workflow + Problem Statement

### 5.1. Current workflow bản nhóm

```text
[1. Nhận meeting notes hoặc project brief — PM/Lead]
→ [2. Lọc quyết định, deliverable và ràng buộc]
→ [3. Viết task/role + kỹ năng cần]
→ [4. Tìm roster và nhớ/tra skill của từng người]
→ [5. Kiểm tra task, deadline và tải việc xuyên dự án]
→ [6. So sánh, thương lượng xung đột — bottleneck]
→ [7. PM/Lead duyệt owner/team và tạo/cập nhật task]
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | PM/Team Lead | Meeting notes hoặc project brief | Input được chọn để xử lý | 10–15 phút sau mỗi meeting/brief | Handoff từ người ghi note/Project Owner |
| 2 | PM/Team Lead | Input thô | Danh sách quyết định, deliverable, constraint | 15–20 phút/input | Notes thường lẫn các thảo luận chưa chốt |
| 3 | PM/Team Lead + chuyên môn | Deliverable/constraint | Task/role, mô tả, acceptance condition và skill cần | 20–30 phút/task | Dễ hỏi lại nếu yêu cầu thiếu |
| 4 | PM/Team Lead | Roster, hồ sơ kỹ năng, kinh nghiệm | Danh sách người đủ điều kiện | 15–20 phút/lần | Dữ liệu skill có thể cũ hoặc tự khai |
| 5 | PM/Resource Manager | Active tasks, effort, deadline, leave | Capacity snapshot và conflict | 20–30 phút/lần | Đếm số task đơn thuần chưa đủ |
| 6 | PM/Lead/Resource Manager | Skill fit + capacity + priority | Candidate ranking và phương án trade-off | 30–45 phút; **BOTTLENECK CHÍNH** | Phải thương lượng xung đột nguồn lực |
| 7 | PM/Team Lead | Phương án đã thống nhất | Owner/team được duyệt và task trong Jira/Planner | 10–15 phút/task | Handoff chính thức sang nhân viên |

**Bottleneck chính:**

Bước 3–6 là điểm nghẽn lớn nhất: PM/Lead mất từ 75 phút (sau họp) đến 3.5 ngày (dự án mới) để biến nội dung chưa có cấu trúc thành task/role đủ rõ rồi ghép kỹ năng với capacity thực tế. Nếu chỉ tối ưu skill fit, chuyên môn hiếm tiếp tục bị dồn việc; nếu chỉ cân số task, có thể giao cho người thiếu kỹ năng hoặc bỏ qua effort/deadline.

### 5.2. Future workflow bản nhóm

```text
[1. PM chọn notes/brief + project scope: 2']
→ [2. AI trích decision/action item/task/role, gắn nguồn và confidence: 1']
→ [3. PM xác nhận phần đã chốt; làm rõ phần thiếu: 5' — HUMAN BOUNDARY]
→ [4. Rule kiểm tra trường bắt buộc, eligibility, RBAC và hard capacity: 1']
→ [5. Workflow lấy skill profile + active workload + deadline/leave: 1']
→ [6. AI xếp hạng Top 3 phương án và giải thích skill/capacity/conflict: 2']
→ [7. PM/Resource Manager duyệt/sửa/từ chối: 10' — HUMAN BOUNDARY]
→ [8. Rule/API tạo hoặc cập nhật task, lưu source + quyết định + người duyệt: 1']

Fallback: input mơ hồ/dữ liệu skill-capacity thiếu/API lỗi/AI confidence thấp
→ giữ draft, nêu trường thiếu, PM phân công thủ công và kiểm tra idempotency trước khi thử lại.
```

> 🖼️ **Infographic kiến trúc giải pháp & Quy trình Before/After:**  
> File đính kèm do thành viên Lâm Hải Dương thiết kế: [`02-group-problem-statement-infographic.jpg`](./02-group-problem-statement-infographic.jpg)  
> 
> 📑 **Tài liệu đặc tả chi tiết bộ chỉ số 4 tầng (Metrics Specification):**  
> Xem chi tiết tại: [`evaluation-metrics.md`](./evaluation-metrics.md)

**Before/after impact — Tier 1: Business & Operational Outcomes:**

| ID / Metric | Trước | Pilot target | Công thức / cách đo |
|---|---:|---:|---|
| **M-01 — Meeting Time-to-Owner (TTO)** | Median 75 phút | Giảm ≥30% (còn < 50 phút) | `timestamp owner được duyệt − timestamp meeting kết thúc` |
| **M-02 — Project Time-to-Approved-Team (TTT)** | Median 3.5 ngày | Giảm ≥30% (còn < 2.5 ngày) | `timestamp đội hình được duyệt − timestamp nhận project brief` |
| **M-03 — Assignment Completeness trong 24 giờ** | 47.2% | ≥95% | Số action item có đủ Owner + Deadline + Output / tổng action item đã duyệt |
| **M-04 — Reassignment Rate do mismatch/overload** | 18.5% | Giảm tương đối ≥20% (xuống < 14.8%) | Số task đổi người do thiếu skill/quá tải / tổng task đã giao |
| **M-05 — Overload Concentration Index (OCI)** | 75% chuyên môn hiếm quá tải | Không tăng và hướng tới giảm ≥25% | Effort của task chuyên môn hiếm dồn vào nhân sự đang >100% capacity |

**Tier 2: AI & Workflow Quality:**

| ID / Metric | Ngưỡng pilot | Cách đo |
|---|---:|---|
| **Q-01 — Action-Item Extraction Recall** | ≥90%; critical action item = 100% | `TP / (TP + FN)` trên gold set do 2 reviewer độc lập gán nhãn |
| **Q-02 — Required-Field Extraction Accuracy** | ≥95% | Đối soát Description/Output/Deadline với trích dẫn trong nguồn; trường không có nguồn phải để `Unknown` |
| **Q-03 — Hallucinated Fact Rate** | **0%** | Đếm tên người, deadline, requirement hoặc ID được tạo ra mà không có căn cứ nguồn |
| **Q-04 — Candidate Recommendation Precision@3** | ≥80% | Tỷ lệ ứng viên trong Top 3 được PM đánh giá “phù hợp để xem xét giao việc” |
| **Q-05 — Explanation Usefulness Score** | Trung bình ≥4.0/5.0 | PM/Lead chấm nhanh độ rõ của lý do, trade-off và cảnh báo tải việc sau mỗi lần duyệt |
| **Q-06 — Suggestion Latency** | P95 <10 giây | Telemetry từ lúc upload/chọn input đến khi hiển thị Top 3 |

**Tier 3: Guardrail & Compliance — zero tolerance:**

| ID / Metric | Ngưỡng | Xử lý khi vi phạm |
|---|---:|---|
| **S-01 — Unauthorized Auto-Assignment** | 0 | Ngắt quyền ghi và chuyển hệ thống sang read-only |
| **S-02 — RBAC / Project Scope Breach** | 0 | Dừng pilot, xóa snapshot tạm và audit API gateway |
| **S-03 — Hallucinated Employee / Project ID** | 0 | Bác bỏ payload, yêu cầu Lead chọn thủ công |
| **S-04 — Unapproved Database Mutation** | 0 | Khóa quyền cập nhật của service account và audit log |
| **S-05 — Sensitive PII Leakage in Log** | 0 | Dừng pilot, xóa/khử định danh log theo quy trình và sửa bộ lọc |

**Tier 4: Post-Assignment & Human Experience (theo dõi sau 7–14 ngày):**

| ID / Metric | Baseline | Pilot target | Cách đo |
|---|---:|---:|---|
| **E-01 — On-Time Delivery Rate** | Cần đo | Tăng 15–20% so với baseline | Task hoàn thành đúng deadline / tổng task đến hạn |
| **E-02 — Rework & Clarification Frequency** | Cần đo | Giảm ≥30% | Đếm lượt hỏi lại/làm lại có reason tag “yêu cầu chưa rõ” hoặc “skill mismatch” |
| **E-03 — Equitable Workload Variance** | Cần đo | Giảm ≥25% | So độ phân tán workload/capacity utilization giữa người trong cùng nhóm chuyên môn |
| **E-04 — Psychological Safety & Fairness** | Cần đo | ≥80% phản hồi tích cực | Likert 5 mức cho câu “Công việc phù hợp năng lực và không gây quá tải bất công” |

---

### 5.3. Problem Statement v0

| Field | Nội dung |
|---|---|
| **Actor** | Project Manager/Team Lead tạo task và ra quyết định phân công. Resource/Department Manager tham gia khi có xung đột nhân sự giữa nhiều dự án. |
| **Workflow** | Sau meeting hoặc khi nhận project brief, actor lọc quyết định/deliverable, tạo task/role, xác định kỹ năng cần, tìm người phù hợp, kiểm tra tải việc và chốt owner/team. Kết quả được tạo/cập nhật trên công cụ quản lý task. |
| **Bottleneck** | Actor phải kết hợp dữ liệu chưa cấu trúc với skill profile và capacity phân tán. Tối ưu một phía dễ giao sai kỹ năng hoặc dồn việc lên người có chuyên môn hiếm. |
| **Impact** | Tăng công điều phối (mất 75 phút sau họp, 3.5 ngày lập đội), chậm kickoff/handoff, 47.2% task thiếu thông tin, 18.5% task phải đổi người; 75% chuyên môn hiếm bị quá tải. |
| **Success Metric** | M-01/M-02 giảm ≥30%, M-03 ≥95%, M-04 giảm tương đối ≥20%, M-05 không tăng. Tier 2: Q-01 ≥90%, Q-02 ≥95%, Q-03 = 0%, Precision@3 ≥80%, explanation ≥4/5 và P95 latency <10 giây. Tier 3 zero-tolerance; Tier 4 theo dõi sau 7–14 ngày. |
| **Boundary** | Chỉ tạo proposal/draft trong project được cấp quyền. Không tự quyết performance, lương, tuyển/sa thải, không tự phân công/publish khi thiếu dữ liệu hoặc chưa được người có trách nhiệm duyệt. |

---

## Phase 6 — Rule / Workflow / Agent + Decision

### 6.0. Ma trận độ phù hợp

- Độ mơ hồ: [ ] Thấp / [x] **Cao** — meeting notes/brief có thể thiếu owner, deadline, acceptance criteria; nhiều phương án staffing cùng hợp lệ.
- Độ phức tạp: [ ] Thấp / [x] **Cao** — cần 3+ nguồn (input công việc, skill profile, task/capacity/leave), nhiều ràng buộc và xung đột xuyên dự án.

**Bài toán nhóm nằm ở ô nào:**

```text
Mơ hồ cao × phức tạp cao → cần AI hỗ trợ phần ngữ nghĩa trong một Workflow có Rule và human approval.
Ma trận không tự động đồng nghĩa phải dùng Agent.
```

**Vì sao:**

AI hữu ích khi trích xuất và so khớp ngữ nghĩa, nhưng các ràng buộc quyền, availability và capacity cần Rule kiểm tra được. Vì quyết định ảnh hưởng workload của con người và dữ liệu có thể cũ, hệ thống phải dừng ở proposal để PM/Lead chịu trách nhiệm phê duyệt.

### 6.1. So sánh Rule / Workflow / Agent

| Mức | Phương án cho bài toán nhóm | Khi nào đủ | Rủi ro | Chọn? |
|---|---|---|---|---|
| **Rule** | Template action item; required fields; filter role/skill threshold; RBAC; hard capacity/leave; round-robin trong tập đủ điều kiện | Task chuẩn hóa, taxonomy skill ổn định, effort/capacity đáng tin và ít ngoại lệ | Rule cứng bỏ qua ngữ cảnh; “balanced” theo số task có thể lệch effort | **Có, cho guardrail và fallback**, nhưng không đủ cho notes/brief mơ hồ |
| **Workflow** | Chuỗi cố định: AI draft task/skill → người làm rõ → Rule lọc → AI đề xuất phương án → người duyệt → API ghi task | Hai input type và nhánh exception xác định được; mọi hành động quan trọng có review | Có thể draft sai, bias hoặc dùng dữ liệu cũ; cần log và source | **Chọn làm mức chính** |
| **Agent** | Tự lập kế hoạch, truy vấn nhiều tool, hỏi bổ sung, tạo/cập nhật ticket và tái phân công | Chỉ cân nhắc khi workflow cố định không xử lý được tỷ lệ case đáng kể và quyền/tool đã được kiểm soát | Tác động ngoài ý muốn, prompt injection, ghi trùng, tự mở rộng phạm vi, khó audit | **Không chọn ở pilot**; chưa có bằng chứng cần autonomy |

**5 câu hỏi chốt:**

1. **Rule có giải được 70–80% case không?** Chưa biết; Rule có thể xử lý eligibility, required fields và hard capacity, nhưng khảo sát thực tế cho thấy 62.5% người dùng đánh giá Rule/biểu mẫu chỉ giải quyết được 21–40% vấn đề do văn bản họp quá lộn xộn.
2. **Các bước đi thẳng hay phải rẽ nhánh?** Có các nhánh rõ khi input chưa chốt, thiếu trường, capacity conflict, người phù hợp không đủ, quyền truy cập thiếu hoặc API lỗi; các nhánh này vẫn có thể thiết kế thành workflow xác định.
3. **Có thật sự cần Agent tự lập kế hoạch + gọi tool không?** Chưa. Pilot chỉ cần đọc dữ liệu trong phạm vi, tạo proposal và chờ duyệt; không cần tự tái phân công hoặc tự thương lượng.
4. **Nếu AI sai, ai phát hiện và sửa trong bao lâu?** PM/Team Lead là reviewer đầu tiên trước publish; Resource Manager kiểm tra conflict xuyên dự án. Phát hiện ngay tại bước Human Approval (10 phút) trước khi ghi task.
5. **Có hạ được từ Agent → Workflow → Rule không?** Có. Chọn Workflow; bên trong dùng Rule cho kiểm tra tất định. Nếu template + Rule đạt metric tương đương thì bỏ AI ở bước đó.

**Mức chọn:**

```text
Workflow (AI-assisted, Rule-guarded, Human-approved)
```

**Vì sao chọn:**

Hai luồng đầu vào khác nhau nhưng đều đi qua chuỗi bước có thể dự đoán và các nhánh exception hữu hạn. AI chỉ cần hỗ trợ phần trích xuất/so khớp ngữ nghĩa; Rule xử lý điều kiện cứng và PM/Lead giữ quyết định. Cấu trúc này đủ để đo từng bước, audit nguồn và rollback, trong khi chưa cần quyền tự chủ của Agent.

**Vì sao không chỉ chọn mức đơn giản hơn:**

Rule đơn thuần không đáng tin khi notes/brief dùng ngôn ngữ tự do, thiếu trường và cần suy ra skill liên quan. Tuy nhiên nhóm phải chạy template + Rule như baseline; nếu baseline đạt outcome với ít rủi ro/công hơn, AI không có lý do được giữ lại.

### 6.2. Problem Statement v1

| Field | Nội dung |
|---|---|
| **Actor** | PM/Team Lead chịu trách nhiệm biến meeting notes/project brief thành task và duyệt owner/team; Resource Manager xử lý conflict xuyên dự án. Nhân viên nhận task được xem và phản hồi proposal ảnh hưởng tới workload của mình. |
| **Workflow** | Actor tiếp nhận notes/brief, xác nhận deliverable, tạo task/role, xác định skill, kiểm tra roster + effort/deadline/leave, so sánh phương án và duyệt assignment trước khi ghi vào Jira/Planner. Hai flow dùng chung đoạn task/role → skill → capacity → approval. |
| **Bottleneck** | Dữ liệu task, skill và capacity khác cấu trúc/độ mới, khiến việc ghép skill fit với tải thực tế phải làm thủ công và dễ tối ưu lệch một phía. Lead mất 75 phút sau họp và 3.5 ngày để chốt đội hình mới. |
| **Impact** | Làm chậm kickoff/handoff, 47.2% task thiếu thông tin trong 24h đầu, 18.5% task phải đổi người; 75% nhân sự chuyên môn hiếm bị quá tải. |
| **Success Metric** | M-01/M-02 giảm ≥30%; M-03 ≥95%; M-04 giảm tương đối ≥20%; M-05 không tăng; Q-01 ≥90% và critical recall =100%; Q-02 ≥95%; Q-03 =0%; Precision@3 ≥80%; explanation ≥4/5; P95 <10 giây. Mọi chỉ số S-01…S-05 bằng 0; Tier 4 theo dõi sau 7–14 ngày. |
| **Boundary (làm / không làm)** | **LÀM:** Draft task/role/skill, lọc eligibility/capacity, xếp hạng 2–3 phương án kèm nguồn/lý do và ghi sau approval trong project cho phép. **KHÔNG LÀM:** Không tự giao/reassign, không tự đổi sprint/priority/deadline, không quyết định nhân sự/lương/thăng chức, không truy cập project ngoài quyền, không suy diễn skill nhạy cảm. |
| **AI intervention point** | Sau khi PM chọn input/project scope và trước khi PM/Resource Manager duyệt assignment. AI hỗ trợ trích task/skill và giải thích ranking; Rule kiểm trước/sau AI, người thật quyết định trước API write. |
| **Mức chọn** | **Workflow** vì các bước/nhánh có thể định nghĩa, AI chỉ xử lý phần mơ hồ và chưa có evidence cần Agent tự lập kế hoạch/hành động. |
| **Rủi ro & người thật kiểm tra** | Rủi ro lớn nhất là task/skill hallucination, capacity cũ, bias và giao quá tải. PM đối chiếu từng task với source; Resource Manager kiểm tra workload/freshness; nhân viên phản hồi conflict; mọi proposal và edit được lưu audit log. |

### 6.3. Final decision

| Câu hỏi | Yes / Not Yet / No | Ghi chú |
|---|---|---|
| Actor + workflow rõ chưa? | **Yes** | PM/Lead và Resource Manager có trách nhiệm cụ thể; current/future workflow và hai input type đã rõ. |
| Baseline + metric đo được chưa? | **Not Yet (đang hoàn thiện)** | Đã thu thập baseline sơ bộ qua Quick Validation (n=8: M-01 median 75p, M-02 3.5 ngày, M-03 47.2%, M-04 18.5%), cần đối soát thêm trên log/ticket thực tế. |
| Data/input đủ dùng chưa? | **Not Yet** | Đã có 3 mẫu meeting notes thực tế; cần hoàn thiện đủ 20 case đã ẩn danh kèm roster và snapshot capacity cho gold set. |
| AI sai, hậu quả chấp nhận được không? | **Yes trong phạm vi draft-only** | 100% người được khảo sát đồng ý mô hình Human Gate: AI chỉ tạo đề xuất, PM/Lead giữ quyền duyệt trước khi ghi task. |
| Có người review/owner không? | **Yes** | PM/Team Lead duyệt task/owner; Resource Manager duyệt conflict xuyên dự án. |
| Có cách non-AI đơn giản hơn không? | **Yes** | Template action item + skill matrix + capacity board + Rule là baseline bắt buộc phải so sánh. |

**Decision:**

```text
Not Yet — chưa Go cho triển khai thật; được chuẩn bị validation và offline/shadow pilot.
```

**Lý do:**

Nhóm đã hoàn thành Quick Validation với 8 người dùng mục tiêu (3 PM/Lead, 1 Resource Manager, 4 Developer), thu thập được các chỉ số baseline ban đầu và quote trải nghiệm thực tế. Khảo sát xác nhận mạnh mẽ nhu cầu giải quyết điểm mù tải việc và bóc tách meeting note, đồng thời 100% người dùng ủng hộ mô hình AI hỗ trợ có người duyệt (Human Gate). Tuy nhiên, nhóm vẫn quyết định **Not Yet cho triển khai vận hành thật** vì cần chuẩn bị đủ bộ 20 input mẫu đã ẩn danh để chạy offline benchmark và kiểm tra xem giải pháp Non-AI (Template + Rule) có thể giải quyết được bao nhiêu phần trước khi kích hoạt mô hình AI phức tạp.

**Nếu Go — pilot nhỏ nhất sau khi qua gate:**

```text
Offline benchmark trên 20 meeting notes/project briefs cũ đã ẩn danh, một roster nhỏ
có skill/effort/deadline/availability và gold assignment do 2 reviewer/PM thống nhất.
So sánh (A) template + Rule với (B) AI-assisted Workflow trên cùng bộ dữ liệu.
Qua gate Q-01/Q-02/Q-03 và Tier 3 mới chạy shadow mode; sau đó live pilot trên đúng
1 dự án/team nhỏ trong 7–14 ngày, luôn có human approval và đo Tier 1 + Tier 4.
```

**Nếu Not Yet — cần validate gì trước:**

```text
1) Phỏng vấn sâu thêm 2 Delivery Director để chuẩn hóa ma trận phân bổ nguồn lực cấp phòng ban.
2) Đo M-01, M-02, M-03, M-04 và M-05 trên log/ticket thực tế của 2 sprint gần nhất để đối soát baseline.
3) Chốt định nghĩa skill, effort, capacity, overload và source-of-truth/freshness.
4) Lập gold set từ 20 input đã ẩn danh và so template + Rule với Workflow.
5) Chỉ sang shadow/live pilot khi đạt Tier 2, Tier 3 bằng 0 và PM chấp nhận review flow.
```

**Nếu No-Go — làm gì thay AI:**

```text
Dùng mẫu meeting notes/action items bắt buộc trường, skill matrix do quản lý xác nhận,
capacity board theo effort/deadline và Jira Automation/round-robin trong tập đủ điều kiện.
```

**Exit / rollback:**

```text
Dừng AI ngay nếu: (1) có ít nhất 1 vi phạm S-01…S-05; (2) Q-01 xuống dưới 85%
trong 3 phiên liên tiếp; (3) M-04 sau 2 tuần cao hơn baseline; hoặc (4) Lead reject
trên 50% tổng đề xuất. Rollback bằng cách ngắt quyền write/chuyển read-only, giữ audit log,
để PM hủy hoặc revert thay đổi đã xác nhận và tiếp tục bằng template + Rule + phân công thủ công.
```

---

### Self-check nộp phần 02 (nhóm)

- [x] Có nhật ký hội tụ **15 → 1** (cluster + shortlist + score; nhóm 5 người).
- [x] Có validation target-user với quote thật (phỏng vấn 4 người, khảo sát 8 người R01–R08 có số liệu baseline).
- [x] Có research 3 nguồn chính thức/link kiểm được (Teams recap, Planner Agent, Jira Automation).
- [x] Có workflow trước/sau đủ thời gian đo được, actor, handoff, bottleneck, boundary, fallback và cách đo (Tier 1–4).
- [x] Có Problem Statement v0/v1 với metric đo được và boundary làm/không làm rõ ràng.
- [x] Có so sánh No AI / Rule / Workflow / Agent trên cùng một bài toán.
- [x] Có quyết định cuối cùng (Not Yet) kèm lý do dựa trên bằng chứng, điều kiện pilot và exit/rollback.
