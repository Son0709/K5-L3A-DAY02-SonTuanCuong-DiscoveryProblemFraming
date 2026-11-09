# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: SonTuanCuong 
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi giao nhiệm vụ cho thành viên và họ đã làm một khoảng thời gian, người giao việc muốn biết họ đã xong bao nhiêu % nhiệm vụ và phần đó đóng góp bao nhiêu % vào dự án, để kịp điều chỉnh trước deadline (candidate #2)
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | Sơn | Khi bắt đầu mỗi tuần, tôi muốn gom tất cả deadline trong tuần từ nhiều môn vào 1 chỗ, để dễ dàng nắm bắt được lịch và không bỏ sót môn nào. | Tôi, sinh viên học nhiều môn | Bước 2: tìm thông báo rải rác trong chat, 10 phút/lần | (Cương): Làm sao để gom lại được tất cả deadline trong nhiều ứng dụng. (Tuấn): Làm sao để có thể biết đâu là deadline đâu là bài tập |
| 2 | Sơn | Khi tôi giao một nhiệm vụ cho thành viên trong nhóm và họ đã làm một khoảng thời gian, tôi muốn biết họ đã xong bao nhiêu % nhiệm vụ và phần đó đóng góp bao nhiêu % vào dự án, để kịp điều chỉnh việc trước deadline | PM, Leader và các thành viên nhận việc | Bước 4–5: không có đơn vị chung để tính "%" nên câu trả lời mơ hồ, 10 phút chờ và hỏi lại mỗi lần; 2-3 lần hỏi lại/ngày | (Tuấn): Bổ sung chức năng: cá nhân dành thời gian bao lâu để hoàn thiện phần việc của mình được giao. (Tuấn & Cương) Làm sao để thành viên có thể sắp xếp được lịch dù đã có ứng dụng|
| 3 | Sơn | Khi tôi định học tiếng Trung 2 tiếng mỗi ngày, tôi muốn có sẵn khung giờ còn trống trong tuần, để giữ được thói quen đều thay vì bỏ buổi | Tôi | Bước 2: không xếp được khung giờ cố định, 60-75 phút/lần; chỉ thực hiện được 7-8/14 buổi trong 2 tuần gần nhất | (Tuấn & Cương): trên thị trường đã có nhiều ứng dụng tương tự như vậy, và nguyên nhân chính vẫn là việc nhàm chán do học 1 mình |
| 4 | Tuấn | Khi có một ý tưởng mới còn mơ hồ, tôi muốn có sẵn user story và tiêu chí nghiệm thu rõ ràng trước khi code, để AI không code sai hướng rồi phải làm lại | Vibe Coder, Khách hàng nhận sản phẩm | Bước 4–6, vòng “sinh code, thấy sai, giải thích lại”: yêu cầu chỉ rõ dần sau khi đã có code sai, nên tốn công gấp đôi | (Sơn & Cương): Vậy khác biệt gì so với những con AI hiện tại như ChatGPT, Claude,... |
| 5 | Tuấn | Khi nhận yêu cầu từ khách hàng, tôi muốn tìm được skill phù hợp hoặc tạo nhanh skill mới đúng yêu cầu đó, để AI làm đúng quy trình ngay từ đầu thay vì tôi giải thích lại mỗi lần | Vibe Coder | Bước 2–3 (tìm không ra hoặc không biết skill nào vừa) và bước 4–6 (không có cách kiểm thử skill ngoài chạy thật) | (Cương): nếu tạo skill thì những con AI hiện tại vẫn có khả năng xảy ra, thì liệu có thể sinh skill tốt hơn không. (Sơn): Số liệu thống kê nào có thể đánh giá được skill sinh ra. |
| 6 | Tuấn | Khi PM hỏi tính năng này mất bao lâu, họ muốn có ước lượng đáng tin, để cam kết với khách | PM, Khách hàng, Dev | Bước 2: ước lượng dựa trên bản demo, bỏ sót phần “ẩn” sau demo | (Sơn): "Thời gian đáng tin" lấy từ những thông số nào |
| 7 | Cương | Khi mở notebook để bắt đầu một bài lab mới, tôi muốn biết đoạn code đầu tiên cần viết, để bắt tay vào làm ngay thay vì đọc đi đọc lại đề | Tôi, học viên khóa AI thực chiến, mới học Python/ML, làm lab trên Google Colab | Bước 3, nghĩ cách chia bài thành các bước code: khoảng 8 phút/bài (ước lượng). Hiểu từng khái niệm nhưng chưa biết nên code phần nào trước, phần nào sau | (Sơn): có sinh code gợi ý không hay là chỉ sinh câu hỏi ôn tập. (Tuấn): Nếu bài lab không có nội dung trong bài giảng thì sao? |
| 8 | Cương | Khi chuẩn bị trước buổi học, tôi muốn nắm được ý chính của tài liệu dài, để vào lớp theo kịp bài | Tôi, học viên khóa AI thực chiến, học 4–5 buổi/tuần, chưa có nhiều nền tảng thực tế về AI | Bước 4, tra khái niệm chưa hiểu: khoảng 30 phút/buổi (ước lượng). Gặp khái niệm mới phải dừng đọc để tra, tra xong quay lại đọc tiếp | (Sơn): Đọc ở đây là nắm rõ hết lý thuyết, hay chỉ cần biết trong slide có những phần nào quan trọng? (Tuấn): Có tổng hợp lại kiến thức không |
| 9 | Cương | Khi tự viết lại một đoạn code từng chạy được nhờ tham khảo, tôi muốn nhớ được cách viết, để không phụ thuộc vào code có sẵn | Tôi, học viên mới học AI, thường tham khảo code mẫu hoặc code do ChatGPT gợi ý khi bị kẹt | Bước 2, tự viết lại: 10–15 phút cố gắng nhưng không viết được, phải bỏ cuộc và mở lại code cũ (ước lượng) | (Sơn): AI có tự sinh code không hay chỉ gợi ý.|

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A — Nắm và giữ kế hoạch thời gian | #1 Gom deadline nhiều môn, #2 Biết % tiến độ của thành viên, #3 Xếp khung giờ học tiếng Trung đều đặn, #6 Ước lượng thời gian đáng tin cho PM | Thông tin về thời gian (hạn nộp, giờ rảnh, tiến độ, thời lượng) nằm rải rác hoặc chỉ là ước lượng cảm tính, nên người làm không biết chắc mình đang ở đâu so với kế hoạch và hạn chót |
| B — Từ yêu cầu mơ hồ đến bước đầu tiên làm được | #4 User story và tiêu chí nghiệm thu trước khi code, #5 Tìm hoặc tạo skill đúng yêu cầu khách, #7 Biết đoạn code đầu tiên của bài lab | Có yêu cầu hoặc đề bài nhưng chưa rõ cần làm gì trước, làm gì sau; phải đoán, làm thử rồi sửa lại, nên tốn công làm đi làm lại |
| C — Hiểu và ghi nhớ kiến thức học | #8 Nắm ý chính tài liệu dài trước buổi học, #9 Nhớ cách viết lại đoạn code đã chạy được | Người học tiếp nhận kiến thức nhưng không giữ lại hoặc không hiểu đủ để tự dùng lại, nên phải tra cứu và quay lại đọc nhiều lần |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm số phút mỗi tuần mà học viên/thành viên nhóm mất vào việc tìm lại, đoán và làm lại khi thực hiện bài học và dự án nhóm
├── Opportunity: Hạn nộp, giờ rảnh, tiến độ và thời lượng nằm rải rác hoặc chỉ là ước lượng 
│     cảm tính, không biết chắc mình đang ở đâu so với kế hoạch và hạn chót
├── Opportunity B: Có yêu cầu hoặc đề bài nhưng chưa rõ cần làm gì trước, làm gì sau,
│     nên phải đoán, làm thử rồi sửa lại
└── Opportunity C: Tiếp nhận kiến thức nhưng không giữ lại hoặc không đủ hiểu để tự dùng lại,
      nên phải tra cứu và đọc lại nhiều lần

     ✗ "Dashboard tiến độ thành viên"           ← solution, gạch khỏi tầng này
     ✗ "Ứng dụng nhắc giờ học / lịch chung"     ← solution, gạch khỏi tầng này
     ✗ "AI sinh user story / sinh code gợi ý"   ← solution, gạch khỏi tầng này
     ✗ "Công cụ tóm tắt tài liệu dài"           ← solution, gạch khỏi tầng này
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- Dashboard tiến độ thành viên (từ candidate #2): là công cụ, không phải pain. Pain thật là không biết chắc tiến độ.
- Ứng dụng nhắc giờ học, lịch chung (từ candidate #1, #3): là công cụ. Pain thật là thông tin thời gian rải rác và không giữ được khung giờ cố định.
- AI sinh user story, sinh code gợi ý (từ candidate #4, #7, #9): là giải pháp. Pain thật là yêu cầu mơ hồ và không biết bắt đầu từ đâu.
- Công cụ tóm tắt tài liệu dài (từ candidate #8): là công cụ. Pain thật là mất nhiều thời gian tra cứu khi đọc.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| #2 Biết % tiến độ của thành viên | 4 | 4 | 3 | 3 | 4 | 4 | 5 | **27** |
| #1 Gom deadline nhiều môn | 4 | 5 | 3 | 4 | 3 | 4 | 5 | **28** |
| #7 Biết đoạn code đầu tiên của bài lab | 5 | 4 | 2 | 2 | 4 | 3 | 4 | **24** |

**Candidate được chọn:** #2 — Biết thành viên đã xong bao nhiêu % nhiệm vụ được giao và đóng góp bao nhiêu % vào dự án

**Vì sao chọn:** Cả nhóm đều làm việc nhóm nên cùng gặp vấn đề này (không chỉ một người); bottleneck là một bước cụ thể (bước 4–5: thành viên trả lời tiến độ bằng cảm tính, người giao việc tự quy đổi %); đo được bằng số lần hỏi lại tiến độ (2–3 lần/ngày), số phút chờ (10 phút/lần) và độ lệch giữa % báo cáo với % thực tế; nhóm hiểu domain vì đang trải nghiệm hằng ngày.

**Vì sao loại các candidate còn lại:** 
- #3 (thói quen học tiếng Trung): Tuấn và Cương chỉ ra đã có nhiều ứng dụng tương tự và nguyên nhân chính là nhàm chán khi học một mình, không phải xếp lịch.
- #4, #5, #7, #9 (liên quan đến code và skill): đã có công cụ AI như ChatGPT và Claude làm gần đúng việc đó; chưa trả lời được khác biệt so với công cụ hiện có.

**Xử lý bất đồng (nếu có):** Điểm tổng của #1 (28) cao hơn #2 (27) một điểm, nhưng nhóm chọn #2. Lý do cần nhóm xác nhận bằng lập luận thật của mình, gợi ý: #1 có thể giải bằng một lịch chung duy nhất (No AI/Rule) và không còn nhiều điều để kiểm chứng, còn #2 vẫn chưa rõ "%" nên định nghĩa thế nào, đây là câu hỏi đáng kiểm chứng ở CP4. 

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Người giao việc ở nhóm khác cũng phải hỏi lại tiến độ nhiều lần mỗi ngày, mất thời gian chờ trả lời | Value | 5 | 2 | ✅ |
| 2 | Bottleneck là thiếu đơn vị chung để tính "%", không phải thiếu công cụ theo dõi việc (bảng task có sẵn chưa giải quyết được) | Value | 5 | 2 | ✅ |
| 3 | Thành viên chấp nhận cập nhật tiến độ đều đặn (ví dụ cuối mỗi buổi làm) mà không thấy bị giám sát | Usability | 4 | 1 | ✅ |
| 4 | Phần lớn nhiệm vụ nhóm chia được thành đầu việc nhỏ có tiêu chí "xong" rõ ràng để tính % | Feasibility | 5 | 2 | ✅ |
| 5 | % thành viên tự báo lệch đáng kể so với % thực tế (nếu lệch ít thì không đáng giải) | Value | 4 | 2 | Sau |
| 6 | Người giao việc sẽ duy trì cách theo dõi mới đều đặn, không bỏ sau vài tuần | Viability | 3 | 1 | Sau |


Giả định nhóm kiểm chứng trong buổi này: **#1, #2, #3, #4** 

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn. Mỗi thành viên phỏng vấn 1 người, ghi 1 Interview Snapshot ngay sau buổi phỏng vấn.

**Kịch bản câu hỏi dùng chung**:

1. Lần gần nhất bạn giao hoặc nhận một việc trong dự án nhóm là khi nào? Kể lại từng bước chuyện đó diễn ra.
2. Sau khi giao việc, bạn biết việc đó xong tới đâu bằng cách nào? Lần gần nhất bạn hỏi lại tiến độ là khi nào, mất bao lâu để có câu trả lời?
3. Có lần nào người ta báo "gần xong" nhưng thực tế chưa xong không? Chuyện gì đã xảy ra, bạn phát hiện ra lúc nào?
4. Hiện bạn đang theo dõi việc bằng công cụ hay cách nào? Đã thử công cụ nào chưa, vì sao còn dùng hoặc bỏ?
5. Khi phải báo cáo tiến độ cho người giao việc, bạn thường làm thế nào? Có điều gì khiến việc đó khó hoặc khó chịu không?
6. Bạn đã bao giờ chia một việc lớn thành các phần nhỏ để tính xem xong bao nhiêu chưa? Lần gần nhất thì sao?
7. Bạn có thể cho mình xem cách bạn đang ghi tiến độ (bảng, tin nhắn, ghi chú) được không?

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

**Snapshot 1** (người phỏng vấn: Sơn)

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Nhóm trưởng dự án, làm việc với nhân viên thực tập mới |
| Câu nói đáng nhớ nhất (nguyên văn) | khi hỏi tiến độ, các bạn mới thường trả lời "sắp xong", nhưng gần đến ngày bàn giao mới biết thành viên chưa xong được 60% công việc được giao |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Khoảng 1 tháng trước. Hỏi tiến độ nhận được câu trả lời "sắp xong", đến sát ngày bàn giao mới phát hiện thành viên chưa xong 60% phần việc |
| Hiện đang xử lý bằng cách nào (workaround)? | Đẩy nhanh tiến độ và đưa thêm thành viên vào dự án |
| Mất bao lâu, bao lần? | 1–2 lần/dự án; thường chỉ phát hiện gần cuối deadline; mỗi lần tốn thêm 1–2 ngày để bù |
| Insight / opportunity rút ra | Người giao việc phát hiện trễ quá muộn |

**Snapshot 2** (người phỏng vấn: Tuấn)

| Trường | Nội dung |
|---|---|
 Người được hỏi (vai trò, không ghi tên thật) | Học viên |
| Câu nói đáng nhớ nhất (nguyên văn) | Mình dùng file GG Sheet để theo dõi tiến độ làm việc  |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Tháng trước, làm trễ deadline với khách hàng |
| Hiện đang xử lý bằng cách nào (workaround)? | Mỗi khi xong tick chọn trạng thái trên gg sheet |
| Mất bao lâu, bao lần? | Tốn thời gian lặp lại |
| Insight / opportunity rút ra | Bám sát vào dự án |


**Snapshot 3** (người phỏng vấn: Cương)

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Trưởng nhóm phát triển phần mềm trong một dự án đồ án sinh viên (Role: Project Leader / Người giao việc) |
| Câu nói đáng nhớ nhất (nguyên văn) | "Đang làm" nhưng đến lúc demo mới thấy dậm chân tại chỗ. |
| Vấn đề gần nhất | Thành viên báo 70% cho module pipeline, nhưng đến demo phần API còn chưa xong, cả đội phải thức đêm sửa. |
| Workaround | Ghi task trên Jira/Notion, nhưng cập nhật chậm; vẫn phải hỏi lại và đoán % bằng cảm tính. |
| Mất thời gian | 2–3 lần hỏi/ngày, mỗi lần 10–15 phút; thêm 2–3 ngày khắc phục trễ. |
| Insight | Không thiếu nơi ghi task, mà thiếu thước đo % hoàn thành rõ ràng để không phụ thuộc vào lời nói ước chừng. |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|

**Nhóm đã sửa problem thế nào sau kiểm chứng:**
Thu hẹp từ "tự động hóa báo cáo tiến độ" thành "soạn nháp nhận định và quy đổi % từ task có sẵn", giảm thời gian hỏi lại. Đồng thời bổ sung cách không dùng AI: template chuẩn hóa + dashboard trực quan cho leadership xem tổng quan nhanh. Giả định #3 về cập nhật đều đặn vẫn cần kiểm chứng thêm trong pilot.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Jira Burndown & Velocity Chart | https://www.atlassian.com/agile/project-management/metrics | Bước 4–5: Theo dõi khối lượng công việc còn lại và tự động quy đổi % hoàn thành dựa trên story points. | Cung cấp số liệu rõ ràng, khách quan theo thời gian thực, giảm thiểu việc phải hỏi han thủ công. | Quá cồng kềnh, cấu hình phức tạp, đòi hỏi team phải cập nhật trạng thái liên tục nếu không số liệu sẽ sai lệch hoàn toàn. | Cần giữ cơ chế cập nhật đơn giản, tránh tạo thêm gánh nặng thủ tục hành chính cho thành viên nhóm. |
| Linear Cycle Progress & Scope Tracking | https://linear.app/blog/progress-tracking | Bước 4: Tự động cảnh báo tiến độ bị lệch (scope creep) và tính toán tỷ lệ đóng góp của từng sub-task vào dự án chung. | Giao diện cực kỳ tối giản, tốc độ nhanh, tập trung cao độ vào việc theo dõi tiến độ công việc của từng cá nhân. | Thiếu tính năng phân tích sâu hoặc gợi ý định tính bằng AI để giải thích vì sao tiến độ lại bị chậm. | Nên học hỏi thiết kế tối giản của Linear để thành viên không thấy ngại mỗi khi cần cập nhật trạng thái công việc. |
| Standuply (Slack/Teams Bot for Agile Teams) | https://www.standuply.com/ | Bước 2–3: Tự động thu thập báo cáo tiến độ không đồng bộ (async standup) qua khung chat hằng ngày. | Tự động hóa hoàn toàn câu hỏi "Hôm nay bạn làm được gì?" trực tiếp trên công cụ chat quen thuộc của team. | Dễ gây cảm giác bị giám sát quá mức khiến thành viên thấy phiền phức hoặc trả lời đối phó. | Tích hợp quy trình lấy thông tin qua kênh chat nhưng cần làm nhẹ nhàng, biến nó thành công cụ hỗ trợ thay vì kiểm soát. |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
