# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: SonTuanCuong 
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn: Khi giao nhiệm vụ cho thành viên và họ đã làm một khoảng thời gian, người giao việc muốn biết họ đã xong bao nhiêu % nhiệm vụ và phần đó đóng góp bao nhiêu % vào dự án, để kịp điều chỉnh trước deadline
- Quyết định cuối: Go

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
|Phỏng vấn|4|3/4 phải tự báo cáo “xong bao nhiêu %” bằng cảm tính, cuối ngày mới nhớ lại|1/4 nói chat nhóm báo cáo nhanh là đủ, sợ bị đo đếm thành áp lực|
|Phỏng vấn|2|2/2 phải tổng hợp tay từ Jira/Excel/chat để biết ai làm gì. Cả hai muốn biết ai đang quá tải|1/2 nói chỉ cần xem task Done trên board, không cần thêm % đóng góp|
|Phỏng vấn|2|2/2 muốn biết dự án đang tới đâu, cần con số tiến độ tổng thể|2/2 không quan tâm từng người, chỉ quan tâm tiến độ và tính năng giao đúng hạn|

**Nhóm đã sửa problem thế nào sau kiểm chứng:**
Thu hẹp từ "tự động hóa báo cáo tiến độ" thành "soạn nháp nhận định và quy đổi % từ task có sẵn", giảm thời gian hỏi lại. Đồng thời bổ sung cách không dùng AI: template chuẩn hóa + dashboard trực quan cho leadership xem tổng quan nhanh. Giả định #3 về cập nhật đều đặn vẫn cần kiểm chứng thêm trong pilot.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| Trello: checklist trong thẻ việc | https://support.atlassian.com/trello/docs/adding-checklists-to-cards/ | Bước theo dõi tiến độ của từng đầu việc: chia việc thành các mục nhỏ và xem % mục đã xong | Trang chính thức nói mặt sau thẻ có thanh tiến độ cho biết % mục đã tick, mặt trước hiển thị số mục, và thanh chuyển xanh khi xong hết | Tiến độ chỉ nằm trong một thẻ và một checklist; trang không nói gì về tổng hợp tiến độ nhiều thẻ hay nhiều người. Thành viên vẫn phải tự tick, không chống được việc báo "gần xong" | Cách làm "chia đầu việc nhỏ, tính % theo số mục xong" đã có sẵn và miễn phí; nhóm không cần tự xây phần này. Khoảng trống còn lại là tổng hợp theo người và theo dự án |
| Notion: Relations & rollups | https://www.notion.com/help/relations-and-rollups | Bước tính tiến độ cả dự án từ các task con (rollup từ bảng task lên bảng dự án) | Rollup tổng hợp dữ liệu của các task liên kết; trang chính thức liệt kê "Percent empty" và "Percent not empty" (% task có hoặc không có giá trị ở một thuộc tính) | Trang chỉ nêu % theo việc có giá trị hay không, không nêu "Percent checked" hay % theo từng trạng thái. Muốn ra % hoàn thành thật cần nhóm tự cấu hình cho thuộc tính "Xong", và vẫn do thành viên cập nhật | Có thể tự dựng bảng tiến độ bằng công cụ có sẵn mà không cần viết phần mềm. Điểm quyết định là định nghĩa "xong" của từng đầu việc, không phải công cụ |

**Kết luận research:**

```text
Việc "chia đầu việc nhỏ và tính % theo số đầu việc xong" đã có sẵn trong công cụ phổ biến (Trello, Notion, Asana).
Nhóm chưa có lý do tự xây một công cụ mới cho bước tính %. Hướng cần kiểm chứng tiếp: định nghĩa "xong" cho từng đầu việc và tín hiệu sớm để phát hiện thành viên chậm.
```


---

**Kết luận Research**
- Thực trạng: Phần lớn quy trình đã có công cụ làm tốt (Jira, Linear, Standuply). Không có lý do để tự xây agent.
- Hướng hợp lý: Rule lấy số liệu thô → AI soạn nháp narrative (dùng Atlassian Rovo hoặc prompt chuẩn) → trưởng nhóm kiểm duyệt → trưởng nhóm gửi.
- Điểm đổi mới: Khác hoàn toàn định hướng ban đầu ("xây công cụ AI viết báo cáo"), nhóm thu hẹp AI lại chỉ làm nhiệm vụ soạn nháp nhận định từ dữ liệu sẵn có.

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — 5 bước, 5/5 bước thủ công; mỗi lần hỏi tiến độ mất khoảng 10 phút chờ, lặp 2–3 lần/ngày

[1 Giao nhiệm vụ trong chat: 3'] → [2 Thành viên làm việc: ví dụ 120']
→ [3 Người giao việc nhắn hỏi "xong tới đâu rồi?": 4']
→ [4 Thành viên trả lời bằng ước lượng cảm tính ("sắp xong"): 10' chờ và hỏi lại mỗi lần] ← BOTTLENECK
→ [5 Người giao việc tự quy đổi thành % so với dự án: 3']

Hệ quả (từ phỏng vấn nhóm trưởng): gần ngày bàn giao mới phát hiện thành viên chưa xong (ví dụ 60% chưa xong),
1–2 lần/dự án, tốn thêm 1–2 ngày để bù.
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | Người giao việc (trưởng nhóm) | Yêu cầu của dự án | Nhiệm vụ gửi trong chat, chưa có tiêu chí "xong" | 3 phút/lần giao | Thường chỉ mô tả bằng lời, không chia đầu việc nhỏ |
| 2 | Thành viên nhận việc | Nhiệm vụ được giao | Phần việc đang làm dở | Ví dụ 120 phút/đợt làm | Không ai theo dõi trong lúc làm |
| 3 | Người giao việc | Nhu cầu biết tiến độ | Tin nhắn hỏi tiến độ | 4 phút/lần; 2–3 lần/ngày | Phải chủ động hỏi, thành viên ít tự báo |
| 4 | Thành viên | Cảm nhận của bản thân về phần đã làm | Câu trả lời ước lượng ("sắp xong") | 10 phút chờ và hỏi lại mỗi lần | Không có đơn vị chung để tính "%" nên câu trả lời mơ hồ; chuyển giao: thành viên → người giao việc |
| 5 | Người giao việc | Câu trả lời mơ hồ của thành viên | % tự quy đổi so với cả dự án | 3 phút/lần | Chuyển giao: không có bước kiểm; lệch chỉ lộ ra sát ngày bàn giao |


### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — 4 bước: 1 Rule, 1 AI, 2 Con người

[1 Giao nhiệm vụ chuẩn hóa] → [2 Rule thu thập task thô] → [3 AI soạn nháp narrative] → [4 Trưởng nhóm kiểm duyệt và gửi đi]
```

| Bước | Actor / Cơ chế | Input | Output | Phân loại | Ghi chú / Boundary & Fallback |
|---:|---|---|---|---|---|
| 1 | Người giao việc | Yêu cầu dự án | Nhiệm vụ chia thành sub-task có tiêu chí hoàn thành rõ ràng | Con người | Boundary: con người định nghĩa task; AI không tự đổi scope hoặc deadline. |
| 2 | Rule | Trạng thái task trong bảng công việc | Số liệu thô: % task hoàn thành, số lượng còn lại, tiến độ theo người | Rule | Tự động thu thập theo thời gian thực hoặc theo định kỳ; không suy diễn ngữ nghĩa. |
| 3 | AI (Rovo / prompt chuẩn) | Dữ liệu thô từ Bước 2 | Bản nháp nhận định tiến độ và % đóng góp | AI | AI chỉ tóm tắt, giải thích ngắn gọn và viết narrative; không thay đổi dữ liệu gốc hoặc tự quyết định deadline. |
| 4 | Trưởng nhóm | Bản nháp từ AI | Báo cáo tiến độ đã được kiểm duyệt và gửi đi | Con người (HITL) | Fallback: nếu AI sai, trưởng nhóm sửa tay bằng template trắng hoặc dùng dashboard trực quan thay cho AI. |

**Bottleneck chính sau khi cải thiện:** Giảm từ việc “đoán % bằng cảm tính” sang “xem dữ liệu thô và trưởng nhóm duyệt lịch sử” — vẫn cần người thực hiện cập nhật task 1 cách sơ bộ và rõ ràng để dữ liệu đáng tin. |

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 | 4 | Theo sơ đồ 4.1 và 4.2. Sơ đồ 4.2 không liệt kê "thành viên làm việc" và "thành viên cập nhật task"; nếu tính cả hai thì là 5 → 6. Lợi ích nằm ở thời gian và độ tin cậy của %, không nằm ở số bước |
| Tổng thời gian (không tính 120' làm việc) | 34–51'/ngày + 3'/lần giao | khoảng 8'/ngày + khoảng 10'/lần giao | Trước: (4' hỏi + 10' chờ + 3' quy đổi) × 2–3 lần/ngày. Sau: Rule + AI khoảng 1', trưởng nhóm duyệt khoảng 5', thành viên cập nhật task khoảng 2', 1 lần/ngày. Giao việc lâu hơn vì phải chia sub-task và ghi tiêu chí "xong" |
| Số bước thủ công | 5/5 | 2/4 | Còn lại: người giao việc chia task và trưởng nhóm duyệt. Ngoài 4 bước, thành viên vẫn phải cập nhật task bằng tay |
| Bottleneck chính | Bước 4: thành viên trả lời "sắp xong" theo cảm tính, 10' chờ và hỏi lại mỗi lần; lệch chỉ lộ ra sát ngày bàn giao, tốn thêm 1–2 ngày để bù | Thành viên cập nhật task đúng và đều; trưởng nhóm duyệt nháp khoảng 5' | Trưởng nhóm duyệt là điểm kiểm soát chất lượng nên chấp nhận được. Việc cập nhật đều thuộc giả định #3, chưa kiểm chứng, sẽ theo dõi trong pilot |
| Rủi ro mới phát sinh | — | (1) AI diễn giải sai hoặc bịa nhận định; (2) task bị đánh dấu "xong" quá sớm khiến % sai nhưng trông như chính xác; (3) Rule tính mọi task ngang nhau nên % đóng góp lệch khi task khác độ lớn; (4) thành viên thấy bị giám sát | (1) AI không đổi dữ liệu gốc, trưởng nhóm duyệt trước khi gửi; nếu sai thì dùng template trắng hoặc dashboard. (2) Tiêu chí "xong" đặt từ bước 1. (3) Người giao việc chia sub-task cỡ tương đương. (4) 1/4 người được phỏng vấn đã lo bị đo đếm thành áp lực, cần kiểm chứng thêm |

Cột "Trước" lấy từ mục 4.1. Cột "Sau" là ước lượng của nhóm vì chưa chạy thử, sẽ bấm giờ trong pilot để xác nhận.

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Trưởng nhóm đồ án sinh viên hoặc dự án nhỏ (3–6 thành viên), người giao việc và chịu trách nhiệm bàn giao đúng hạn |
| **Quy trình** | Giao nhiệm vụ trong chat → thành viên làm việc → trưởng nhóm nhắn hỏi "xong tới đâu rồi?" → thành viên trả lời bằng ước lượng → trưởng nhóm tự quy đổi thành % nhiệm vụ và % tiến độ dự án |
| **Bottleneck** | Bước 4: thành viên trả lời theo cảm tính ("sắp xong") vì không có đơn vị chung để tính %, mỗi lần mất khoảng 10 phút chờ và hỏi lại |
| **Impact** | 34–51 phút/ngày cho mỗi trưởng nhóm (17 phút/lần × 2–3 lần/ngày). Việc chậm chỉ lộ ra sát ngày bàn giao, 1–2 lần/dự án, tốn thêm 1–3 ngày để bù (Snapshot 1 và 3) |
| **Success Metric** (baseline → target, cách đo) | Tổng thời gian theo dõi tiến độ mỗi ngày. **Baseline:** 34–51 phút/ngày (tính từ mục 4.1, theo mô tả của nhóm và phỏng vấn, chưa bấm giờ). **Target:** dưới 15 phút/ngày. **Cách đo:** trong 2 tuần pilot, trưởng nhóm bấm giờ thời gian hỏi, chờ, quy đổi hoặc duyệt; thành viên ghi số phút cập nhật task; cộng lại theo ngày để không tính thiếu phần việc chuyển sang thành viên |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | **AI không được:** thay đổi dữ liệu gốc (trạng thái task, scope, deadline); tự giao lại việc hoặc chuyển task giữa các thành viên. **HITL:** trưởng nhóm kiểm tra mọi bản nhận định của AI trước khi gửi cho người khác; nếu AI sai thì viết tay bằng template trắng hoặc xem dashboard |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

Phản biện từ AI (Claude), chỉ nêu lỗ hổng, không viết lại:

- Metric chỉ đo tốc độ. Nếu thời gian giảm nhưng % vẫn sai thì trưởng nhóm vẫn phát hiện trễ; cần chỉ số nào để đo độ chính xác
- Baseline chưa bấm giờ, và 10 phút chờ không phải thời gian trưởng nhóm thực sự làm việc. Gộp vào có làm baseline cao hơn thực tế không
- Snapshot 2 đã dùng Google Sheet để tick trạng thái mà vẫn trễ deadline. Bottleneck có thật là thiếu đơn vị tính %, hay là thiếu cập nhật và theo dõi
- "% nhiệm vụ" được tính thế nào khi các đầu việc khác độ lớn?

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ phức tạp thấp**. Phần tính % có độ mơ hồ thấp, phần viết nhận định có độ mơ hồ cao → Workflow có AI ở một bước.

Vì sao:

- **Phức tạp thấp:** 4 bước cố định (mục 4.2), không rẽ nhánh, nguồn chính chỉ là bảng task.
- **Mơ hồ thấp (tính %):** sub-task có tiêu chí "xong" thì % chỉ là phép đếm, có đúng/sai rõ.
- **Mơ hồ cao (nhận định):** "ai có nguy cơ trễ, vì sao" có nhiều cách viết đúng và phải đọc ghi chú tự do của thành viên (ví dụ "còn kẹt API" ở Snapshot 3).

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Chia nhiệm vụ thành sub-task có tiêu chí "xong", thành viên tick cuối mỗi buổi làm | Nhóm nhỏ, ít việc song song | Vẫn phải hỏi và tự cộng tay; Snapshot 2 tick trên Sheet mà vẫn trễ | **Dùng cho bước 1** |
| **Rule** | Trello checklist / Notion rollup tự tính % theo nhiệm vụ, người, dự án; gắn cờ khi sub-task chưa xong mà sắp tới hạn | Chỉ cần con số (1/2 người được hỏi nói xem task Done là đủ) | Thấy số nhưng không thấy lý do chậm; % sai nếu tick "xong" quá sớm | **Dùng cho bước 2** |
| **Workflow** | Rule tính % và cờ → AI soạn nháp nhận định → trưởng nhóm duyệt rồi gửi | Phải tổng hợp nhiều việc và ghi chú tự do (2/2 người phải tổng hợp tay từ Jira/Excel/chat) | AI diễn giải sai, bịa lý do, bỏ qua cờ | **Chọn** |
| **Agent** | AI tự đọc chat, tự đánh giá, tự nhắc thành viên, tự chia lại việc | Khi không đoán trước được bước tiếp theo | Vượt boundary mục 5; tăng cảm giác bị giám sát | Không chọn |

**Mức chọn:** **Workflow**. Lõi là No AI (bước 1) và Rule (bước 2); AI chỉ soạn nháp ở bước 3, không tính số, không tự gắn cờ.

**Vì sao không chọn mức đơn giản hơn:** No AI + Rule giải được phần chính của bottleneck (thiếu đơn vị tính %). Nhưng Snapshot 2 và 3 cho thấy con số chưa đủ: có % mà vẫn trễ, vì lý do chậm nằm trong ghi chú tự do, Rule không đọc được. Bằng chứng này mới có 1–2 người, nên pilot chạy **tuần 1 chỉ Rule, tuần 2 mới thêm AI**; nếu AI không giúp giảm thời gian thì quay về Rule (ngưỡng ở mục 8). Không chọn Agent vì các bước đã cố định và mọi quyết định điều chỉnh là của trưởng nhóm.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Nháp nhận định dưới 150 từ: % dự án và từng nhiệm vụ (chép từ Rule), giải thích mọi cờ kèm lý do từ ghi chú, điểm cần hỏi lại |
| **Judgment** — con người cân nhắc, quyết định gì? | Trưởng nhóm xác định cờ nào là chậm thật, có cần điều chỉnh phân công không, phần nào gửi ra ngoài nhóm |
| **Action** — hành động cuối cùng là gì, ai làm? | Trưởng nhóm sửa nháp, gửi cập nhật, nhắn riêng thành viên nếu cần. AI không gửi tin, không sửa bảng task |
| **Outcome** — đo kết quả bằng gì? | Thời gian theo dõi/ngày (34–51' → dưới 15'); số lần hỏi lại/ngày (2–3); số lần phát hiện chậm sát bàn giao (1–2/dự án); tỉ lệ nháp phải viết lại |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | Kết quả Rule (sub-task, người làm, deadline, trạng thái, %, cờ) + ghi chú của thành viên. **Chưa có sẵn**: hiện việc giao trong chat, chưa chia sub-task; chỉ có sau khi bước 1 chạy được |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Phần trưởng nhóm sửa trong nháp; cờ bị đánh dấu "báo nhầm"; các lần chậm lộ ra ở demo mà nháp không nêu |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? **Augment.** Các hành động sau khi biết tiến độ (đẩy nhanh, thêm người ở Snapshot 1) đều do trưởng nhóm quyết; 1/4 người được hỏi sợ bị đo đếm thành áp lực, nên AI không được tự đánh giá hay tự nhắc thành viên.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? **Bỏ sót tệ hơn.** Phát hiện chậm quá muộn tốn thêm 1–3 ngày (Snapshot 1, 3), còn báo nhầm chỉ tốn một lần hỏi lại. Xử lý: cờ do Rule gắn nên AI không làm mất cờ được; tiêu chí đánh giá bắt nháp nêu đủ mọi cờ; cờ viết theo nhiệm vụ, không theo người, để giảm áp lực khi báo nhầm.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Trưởng nhóm đồ án sinh viên hoặc dự án nhỏ (3–6 thành viên), người giao việc và chịu trách nhiệm bàn giao đúng hạn |
| **Quy trình** | Giao nhiệm vụ trong chat → thành viên làm việc → trưởng nhóm nhắn hỏi "xong tới đâu rồi?" → thành viên trả lời bằng ước lượng → trưởng nhóm tự quy đổi thành % nhiệm vụ và % tiến độ dự án |
| **Bottleneck** | Bước 4: thành viên trả lời theo cảm tính ("sắp xong") vì không có đơn vị chung để tính %, mỗi lần mất khoảng 10 phút chờ và hỏi lại |
| **Impact** | 34–51 phút/ngày cho mỗi trưởng nhóm (17 phút/lần × 2–3 lần/ngày). Việc chậm chỉ lộ ra sát ngày bàn giao, 1–2 lần/dự án, tốn thêm 1–3 ngày để bù (Snapshot 1 và 3) |
| **Success Metric** (baseline → target, cách đo) | **(1) Tổng thời gian theo dõi tiến độ mỗi ngày.** **Baseline:** 34–51 phút/ngày (tính từ mục 4.1, theo mô tả của nhóm và phỏng vấn, chưa bấm giờ). **Target:** dưới 15 phút/ngày. **Cách đo:** trong 2 tuần pilot, trưởng nhóm bấm giờ thời gian hỏi, chờ, quy đổi hoặc duyệt; thành viên ghi số phút cập nhật task; cộng lại theo ngày. **(2) Độ chính xác của %: tỉ lệ sub-task đã tick "xong" mà thật sự xong.** **Baseline:** chưa có, đo trong tuần 1 pilot. **Target:** từ 90%. **Cách đo:** mỗi tuần trưởng nhóm kiểm thử 5 sub-task đã tick "xong", đối chiếu với tiêu chí "xong" đặt ở bước 1 |
| **Boundary** | **AI không được:** thay đổi dữ liệu gốc (trạng thái task, scope, deadline); tự giao lại việc hoặc chuyển task giữa các thành viên; tính số hoặc tự gắn cờ; gửi tin hoặc sửa bảng task; tự đánh giá hay tự nhắc thành viên. **HITL:** trưởng nhóm kiểm tra mọi bản nhận định của AI trước khi gửi cho người khác; nếu AI sai thì viết tay bằng template trắng hoặc xem dashboard |
| **AI intervention point** | Bước 3 của quy trình tương lai (mục 4.2): sau khi Rule tính % và gắn cờ, trước khi trưởng nhóm duyệt. Chạy 1 lần/ngày, và chỉ chạy được sau khi bước 1 đã chia sub-task |
| **Mức chọn** | **Workflow.** Lõi là No AI (bước 1) và Rule (bước 2); AI chỉ soạn nháp ở bước 3. Pilot tuần 1 chỉ Rule, tuần 2 mới thêm AI |
| **Rủi ro & người kiểm tra** | AI diễn giải sai, bịa lý do, bỏ qua cờ → trưởng nhóm kiểm mọi bản nháp trước khi gửi; cờ do Rule gắn nên AI không làm mất cờ được. Task bị đánh dấu "xong" quá sớm → tiêu chí "xong" đặt từ bước 1, trưởng nhóm kiểm thử 5 sub-task đã tick "xong" mỗi tuần. Task khác độ lớn làm lệch % → người giao việc chia sub-task cỡ tương đương. Thành viên thấy bị giám sát → cờ viết theo nhiệm vụ, không theo người |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Success Metric | Chỉ đo tổng thời gian theo dõi tiến độ | Thêm độ chính xác của %: tỉ lệ sub-task đã tick "xong" mà thật sự xong | Phản biện ở mục 5: nếu thời gian giảm nhưng % vẫn sai thì trưởng nhóm vẫn phát hiện trễ |
| Boundary | AI không đổi dữ liệu gốc, không tự giao lại hay chuyển task | Thêm: AI không tính số, không tự gắn cờ, không gửi tin, không sửa bảng task, không tự đánh giá hay tự nhắc thành viên | Mục 6.2 và 6.3 chọn Workflow, số và cờ thuộc về Rule, hành động thuộc về trưởng nhóm; mục 6.4: 1/4 người được hỏi sợ bị đo đếm thành áp lực |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Đủ cờ | Mọi cờ Rule đã gắn đều được nêu trong nháp | Thiếu dù chỉ 1 cờ thì cả bản nháp không đạt |
| 2 | Không bịa lý do | Mọi lý do truy được về ghi chú của thành viên; cờ không có ghi chú được ghi là chưa có ghi chú và đưa vào điểm cần hỏi lại | Có lý do không xuất hiện trong ghi chú |
| 3 | Không đánh giá cá nhân | Viết theo nhiệm vụ; nêu tên người phụ trách nhiệm vụ vẫn đạt | Có câu đánh giá thành viên, ví dụ làm chậm, thiếu cố gắng |
| 4 | Đúng số liệu | Mọi con số khớp kết quả Rule | Có số AI tự tính hoặc làm tròn khác Rule |
| 5 | Đúng độ dài và cấu trúc | Dưới 150 từ, có % dự án và từng nhiệm vụ, giải thích cờ, điểm cần hỏi lại | Từ 150 từ trở lên hoặc thiếu phần |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Trung bình | Pain có thật: phát hiện chậm sát bàn giao tốn thêm 1–3 ngày, 2/2 người phải tổng hợp tay. Nhưng 1/2 người nói xem task Done là đủ, và Snapshot 2 đã dùng Google Sheet mà vẫn trễ, nên chưa chắc giá trị nằm ở bước AI hơn là ở Rule. Mẫu mới 1–2 người |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Trung bình | Trưởng nhóm chỉ sửa nháp dưới 150 từ nên dễ dùng. Rủi ro nằm ở thành viên: phải cập nhật task đều (giả định #3 chưa kiểm chứng) và 1/4 người được hỏi sợ bị đo đếm thành áp lực |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Trung bình | Công cụ có sẵn (Trello, Notion). Nhưng nghiên cứu mới xác nhận Trello hiển thị % checklist trong một thẻ, chưa xác nhận tự tổng hợp % theo người và dự án; Notion chỉ liệt kê "Percent empty / not empty". Dữ liệu đầu vào chưa có sẵn: hiện việc giao trong chat, chưa chia sub-task, chỉ có sau khi bước 1 chạy được |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Trung bình | Chưa kiểm chi phí và gói của Rovo hoặc Power-Up trả phí; chưa biết có được đưa nội dung chat, ghi chú của thành viên vào công cụ AI không. Người vận hành là trưởng nhóm, nhưng chưa thấy bằng chứng họ duy trì cập nhật đều sau vài tuần |

### 8.2. Kết luận

**Quyết định:** **Go, phạm vi nhỏ.**

**Lý do:** Cả 4 rủi ro ở mục 8.1 đều Trung bình, không có rủi ro Cao, và đều kiểm được ngay trong pilot. Rule chạy trước nên nếu bước AI thất bại, nhóm vẫn giữ được phần giải bottleneck chính (đơn vị tính %).

**Nếu Go — pilot nhỏ nhất:** 1 nhóm đồ án 3–6 người, 2 tuần, dùng Trello checklist miễn phí và một prompt chuẩn, không trả phí.

- **Tuần 1 (No AI + Rule):** chia sub-task có tiêu chí "xong", thành viên tick và ghi 1 dòng ghi chú mỗi buổi; trưởng nhóm bấm giờ theo dõi để có baseline thật.
- **Tuần 2 (thêm AI):** hỏi thành viên đồng ý đưa ghi chú vào AI trước; AI soạn nháp mỗi ngày, trưởng nhóm duyệt và chấm theo 5 tiêu chí ở mục 7.

**Nếu Not Yet — cần kiểm chứng gì trước:** Không áp dụng (giả định #3, #6 được kiểm trong tuần 1).

**Nếu No-Go — nên làm gì thay AI:** Không áp dụng. Dự phòng: giữ No AI + Rule, trưởng nhóm viết cập nhật bằng template.

**Ngưỡng dừng:**

- Hết tuần 1, thành viên không cập nhật ở quá nửa số ngày → không bật AI, quay về CP4 kiểm lại giả định #3.
- Sau tuần 2, thời gian theo dõi không thấp hơn tuần 1 hoặc phải viết lại trên 70% bản nháp → bỏ AI, giữ Rule.
- Có 1 bản nháp thiếu cờ hoặc sai số lọt qua bước duyệt → dừng AI ngay.
- Sau 2 tuần, thời gian vẫn từ 34 phút/ngày trở lên hoặc độ chính xác % dưới 70% → dừng giải pháp, quay về CP4 (bottleneck có thể là thiếu cập nhật, không phải thiếu đơn vị tính %).

---

## 9. Hạn chế và hướng tiếp theo

**Hạn chế**

- **Bằng chứng còn mỏng:** nhóm mới có 3 Interview Snapshot chi tiết (2 trưởng nhóm, 1 học viên), chưa đủ để khái quát cho mọi nhóm nhỏ.
- **Baseline chưa đo thật:** 34–51 phút/ngày được tính từ mô tả và phỏng vấn, chưa bấm giờ, và đang gộp cả 10 phút chờ vốn không phải thời gian trưởng nhóm thực sự làm việc.
- **Lý do cần AI chưa có bằng chứng trực tiếp:** Rule đã giải phần chính của bottleneck; bước AI dựa vào ghi chú tự do của thành viên, nhưng chưa có phỏng vấn nào cho thấy thành viên sẽ viết ghi chú này.
- **Giả định về hành vi chưa kiểm chứng:** thành viên có cập nhật đều mà không thấy bị giám sát không (#3), trưởng nhóm có duy trì cách theo dõi mới không (#6).
- **Cách tính % còn thô:** Rule tính mọi sub-task ngang nhau nên "% đóng góp" có thể lệch khi các việc khác độ lớn.
- **Công cụ và dữ liệu chưa xác nhận:** chưa rõ Trello hoặc Notion có tổng hợp được % theo người và dự án không; chưa kiểm chi phí Rovo hoặc Power-Up trả phí; chưa biết có được đưa ghi chú của thành viên vào công cụ AI không.
- **Pilot có giới hạn đo:** 2 tuần chưa đủ để đo số lần phát hiện chậm sát bàn giao, và chỉ số độ chính xác chỉ dựa trên 5 sub-task mỗi tuần.

**Hướng tiếp theo**

1. Tuần 1 pilot chỉ chạy No AI + Rule: bấm giờ để có baseline thật, tách thời gian làm và thời gian chờ, đo baseline độ chính xác của %.
2. Trước tuần 2, xác nhận khả năng tổng hợp của Trello hoặc Notion, chi phí và quyền đưa ghi chú vào công cụ AI.
3. Tuần 2 thêm bước AI: chấm từng bản nháp theo 5 tiêu chí ở mục 7, đồng thời ghi lại thành viên có thật sự viết ghi chú không và AI có giúp giảm thời gian so với tuần 1 không.
4. Phỏng vấn thêm trưởng nhóm và thành viên nhận việc, gồm cả người chỉ cần xem task Done, để xác định nhóm nào chỉ cần Rule.
5. Chốt cách tính % đóng góp khi các việc khác độ lớn.
6. Nếu tiếp tục sau pilot, theo dõi trọn một dự án để đo số lần phát hiện chậm sát bàn giao.

## 10. Tài liệu tham khảo

- Slide bài giảng 
