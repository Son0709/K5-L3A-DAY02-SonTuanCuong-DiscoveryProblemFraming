# Báo cáo cá nhân — 2A202603680_DangDucCuong

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:
- MSSV:
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:
- Link repo nhóm:

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

Tôi scan 5 problem từ quá trình học khóa AI thực chiến (chủ yếu từ bài lab lọc tin nhắn rác bằng ML, DL, Embedding và LLM).

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi mở notebook để bắt đầu một bài lab mới, tôi muốn biết đoạn code đầu tiên cần viết, để bắt tay vào làm ngay thay vì đọc đi đọc lại đề | Tôi (học viên mới học AI) | 15–20 phút/bài mới gõ được dòng đầu tiên, 4–5 buổi/tuần (ước lượng) |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi đã hiểu Bag of Words, tôi muốn biết dùng hàm nào để biến tin nhắn thành vector, để chuyển lý thuyết thành code mà không phải đoán | Tôi | Lab lọc tin nhắn rác: tra cứu 1–3 lần (ước lượng) |
| 3 | Tốn thời gian | Khi ghép bước xử lý dữ liệu với bước huấn luyện mô hình, tôi muốn đầu ra bước trước khớp đầu vào bước sau, để chạy trọn quy trình không lỗi | Tôi | Lab lọc tin nhắn rác: dưới 15 phút/lần sửa lỗi ghép (ước lượng) |
| 4 | Lặp lại | Khi tự viết lại một đoạn code từng chạy được nhờ tham khảo, tôi muốn nhớ được cách viết, để không phụ thuộc vào code có sẵn | Tôi | 2–3 lần từ đầu khóa (ước lượng) |
| 5 | Tốn thời gian | Khi chuẩn bị trước buổi học, tôi muốn nắm được ý chính của tài liệu dài, để vào lớp theo kịp bài | Tôi | 75 phút/buổi (khoảng 30 phút là tra khái niệm chưa hiểu), 4–5 buổi/tuần → khoảng 300–375 phút/tuần (ước lượng) |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Tôi tự nêu trước vấn đề "hiểu lý thuyết nhưng khó áp dụng vào code" cùng 5 biểu hiện. Vì không nhớ rõ từng lần, tôi nhờ AI đưa danh sách tình huống thường gặp để gợi nhớ, rồi nhờ AI thu hẹp và diễn đạt lại thành Job Story. Các con số là ước lượng của tôi.
- **Giữ lại:** 5 dòng ở bảng trên, đều là tình huống tôi đã gặp.
- **Bỏ:** lỗi cài môi trường Colab, tìm lại code cũ, không biết thứ tự các bước, so sánh mô hình (tôi chưa gặp). Ba ý khác tôi có gặp nhưng chưa có số liệu nên chưa đưa vào: chia Train/Validation/Test, giải thích code mẫu, đọc hiểu Precision/Recall/F1.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Bắt đầu viết code cho bài lab (#1) | Đúng vấn đề gốc "hiểu lý thuyết nhưng khó áp dụng vào code"; lặp lại 4–5 lần/tuần; có điểm bắt đầu và kết thúc rõ (mở notebook → gõ dòng đầu tiên), dễ tự bấm giờ | Số phút mới là ước lượng; chưa biết một checklist khung chung có đủ giải quyết không |
| 2 | Đọc tài liệu trước buổi học (#5) | Tốn thời gian nhất: khoảng 300–375 phút/tuần; bước nghẽn rõ (tra khái niệm chưa hiểu, khoảng 30 phút/buổi) | Đọc kỹ có thể là thời gian học cần thiết; giảm thời gian có thể làm giảm mức hiểu |
| 3 | Không tự viết lại được code đã từng chạy (#4) | Cùng pattern với card #1 nhưng kẹt ở thời điểm khác (sau khi đã tham khảo); mỗi lần mất khoảng 40 phút | Tần suất thấp (2–3 lần từ đầu khóa); có thể nhóm sẽ gộp với card #1 |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi mở notebook để bắt đầu một bài lab mới, tôi muốn biết đoạn code đầu tiên cần viết, để bắt tay vào làm ngay thay vì đọc đi đọc lại đề |
| Actor | Tôi, học viên khóa AI thực chiến, mới học Python/ML, làm lab trên Google Colab |
| Thời điểm / bối cảnh | Đầu mỗi bài lab, khi đã có đề và đã học lý thuyết liên quan (ví dụ lab lọc tin nhắn rác: Bag of Words, Logistic Regression, MLP, Embedding, KNN, chia Train/Validation/Test, Precision/Recall/F1) |
| Quy trình hiện tại (3–7 bước) | 1. Đọc đề lab (3') · 2. Xem lại lý thuyết liên quan (3') · 3. Nghĩ cách chia bài thành các bước code (8') · 4. Tìm hàm/thư viện cần dùng, tra Google hoặc hỏi ChatGPT (3') · 5. Gõ dòng code đầu tiên (1') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3, nghĩ cách chia bài thành các bước code: khoảng 8 phút/bài (ước lượng). Hiểu từng khái niệm nhưng chưa biết nên code phần nào trước, phần nào sau |
| Impact (nếu không giải thì sao) | Khoảng 18 phút/bài trước khi gõ được dòng đầu tiên × 4–5 buổi/tuần ≈ 70–90 phút/tuần; riêng bước nghẽn khoảng 32–40 phút/tuần (ước lượng). Có lần đọc xong vẫn phải hỏi lại mới bắt đầu được |
| Success metric (baseline → target) | **Baseline:** khoảng 18 phút từ lúc mở notebook đến lúc gõ dòng code đầu tiên (ước lượng, sẽ bấm giờ thật ở 2 buổi lab tới). **Target:** dưới 10 phút (mục tiêu đề xuất). **Cách đo:** tự ghi giờ mở notebook và giờ gõ dòng code đầu tiên ở mỗi bài lab trong 2 tuần |
| Phương án không dùng AI | Checklist khung chung cho bài lab ML (đọc dữ liệu → tiền xử lý → biến đổi dữ liệu → chia dữ liệu → huấn luyện → đánh giá); viết các bước bằng lời vào notebook trước khi code |
| Giả thuyết về AI (nếu có) | Chỉ cân nhắc nếu checklist không đủ: công cụ AI gợi ý khung các bước cho đề bài cụ thể (không đưa code hoàn chỉnh), tôi tự viết code cho từng bước |
| Cảm nhận nhanh | No AI (checklist có thể đã đủ, cần thử trước) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 18 phút/bài (ước lượng)

[1 Đọc đề: 3'] → [2 Xem lại lý thuyết: 3']
→ [3 Nghĩ cách chia bài thành các bước code: 8'] ← BOTTLENECK
→ [4 Tìm hàm/thư viện: 3'] → [5 Gõ dòng code đầu tiên: 1']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi chuẩn bị trước buổi học, tôi muốn nắm được ý chính của tài liệu dài, để vào lớp theo kịp bài |
| Actor | Tôi, học viên khóa AI thực chiến, học 4–5 buổi/tuần, chưa có nhiều nền tảng thực tế về AI |
| Thời điểm / bối cảnh | Trước mỗi buổi học, khi đọc tài liệu khóa học của buổi đó (có nhiều khái niệm mới như Embedding, LLM, RAG) |
| Quy trình hiện tại (3–7 bước) | 1. Mở tài liệu buổi học (2') · 2. Đọc lướt toàn bộ (8') · 3. Đọc kỹ từng phần (25') · 4. Tra khái niệm chưa hiểu bằng Google hoặc ChatGPT (30') · 5. Ghi chú ý chính (10') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 4, tra khái niệm chưa hiểu: khoảng 30 phút/buổi (ước lượng). Gặp khái niệm mới phải dừng đọc để tra, tra xong quay lại đọc tiếp |
| Impact (nếu không giải thì sao) | 75 phút/buổi × 4–5 buổi/tuần ≈ 300–375 phút/tuần; riêng bước tra khái niệm khoảng 120–150 phút/tuần (ước lượng) |
| Success metric (baseline → target) | **Baseline:** 75 phút/buổi, trong đó khoảng 30 phút tra khái niệm (ước lượng). **Target:** thời gian tra khái niệm dưới 15 phút/buổi (mục tiêu đề xuất), **và** mức hiểu không giảm: trước khi đọc tự đặt 3 câu hỏi về bài, sau khi đọc tự trả lời đúng cả 3. **Cách đo:** tự ghi giờ và ghi kết quả 3 câu hỏi sau mỗi buổi trong 2 tuần |
| Phương án không dùng AI | Tự lập bảng thuật ngữ (khái niệm → giải thích ngắn → link tài liệu) và dùng lại qua các buổi; đọc mục lục và phần tóm tắt trước; đặt 3 câu hỏi cần trả lời trước khi đọc |
| Giả thuyết về AI (nếu có) | Công cụ AI liệt kê khái niệm mới trong tài liệu và giải thích ngắn kèm ví dụ trước khi tôi đọc; tôi vẫn đọc kỹ tài liệu gốc và kiểm lại giải thích |
| Cảm nhận nhanh | Workflow (cần kiểm: bảng thuật ngữ tự lập có thể đã đủ) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 75 phút/buổi (ước lượng)

[1 Mở tài liệu: 2'] → [2 Đọc lướt: 8'] → [3 Đọc kỹ: 25']
→ [4 Tra khái niệm chưa hiểu: 30'] ← BOTTLENECK
→ [5 Ghi chú: 10']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi tự viết lại một đoạn code từng chạy được nhờ tham khảo, tôi muốn nhớ được cách viết, để không phụ thuộc vào code có sẵn |
| Actor | Tôi, học viên mới học AI, thường tham khảo code mẫu hoặc code do ChatGPT gợi ý khi bị kẹt |
| Thời điểm / bối cảnh | Hôm sau hoặc vài ngày sau khi làm xong một phần lab, khi cần tự viết lại đoạn code đó |
| Quy trình hiện tại (3–7 bước) | 1. Mở bài cần viết lại (2') · 2. Tự viết lại, bị kẹt (10–15') · 3. Mở lại code cũ hoặc hỏi lại (10') · 4. Hiểu lại và viết xong (15') |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2, tự viết lại: 10–15 phút cố gắng nhưng không viết được, phải bỏ cuộc và mở lại code cũ (ước lượng) |
| Impact (nếu không giải thì sao) | Khoảng 40 phút mỗi lần, đã xảy ra 2–3 lần từ đầu khóa → khoảng 80–120 phút (ước lượng). Code chạy được nhưng tôi chưa thật sự hiểu, nên không chắc tự làm được khi không có code tham khảo |
| Success metric (baseline → target) | **Baseline:** 2–3 lần phải mở lại code cũ hoặc hỏi lại từ đầu khóa (ước lượng). **Target:** 0 lần trong 2 tuần tới (mục tiêu đề xuất). **Cách đo:** sau mỗi bài lab, chọn 1 đoạn code đã tham khảo, hôm sau tự viết lại không nhìn và ghi lại có viết được không |
| Phương án không dùng AI | Sau khi tham khảo, gõ lại đoạn code mà không nhìn; ghi bằng lời mình mỗi dòng làm gì; tự viết lại vào hôm sau như bài ôn |
| Giả thuyết về AI (nếu có) | Công cụ AI đặt câu hỏi kiểm tra về đoạn code thay vì đưa code; tôi tự trả lời và tự viết |
| Cảm nhận nhanh | Chưa biết |

**Liên hệ với card #1:** cùng pattern "hiểu lý thuyết nhưng khó tự viết code". Card #1 kẹt lúc **bắt đầu** bài lab; card #3 kẹt lúc **tự viết lại sau khi đã tham khảo**. Nếu nhóm gộp ở CP3, card #3 là dữ liệu bổ sung cho card #1.

Quy trình nháp hiện tại:

```text
HIỆN TẠI — khoảng 40 phút mỗi lần xảy ra (ước lượng)

[1 Mở bài cần viết lại: 2']
→ [2 Tự viết lại, bị kẹt: 10–15'] ← BOTTLENECK
→ [3 Mở lại code cũ / hỏi lại: 10'] → [4 Hiểu lại và viết xong: 15']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Đúng vấn đề tôi gặp nhiều nhất khi học ("hiểu lý thuyết nhưng khó áp dụng vào code"), lặp lại mỗi buổi lab, có điểm bắt đầu và kết thúc rõ nên dễ bấm giờ.
- Câu hỏi muốn nhóm phản biện: Các bạn có kẹt ở bước "chia bài thành các bước code" giống tôi không? Nếu có một checklist khung chung cho bài lab ML, thời gian bắt đầu có giảm được một nửa không?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: Baseline 15–20 phút chỉ dựa trên trí nhớ, chưa bấm giờ thật | Đồng ý | Ghi rõ "ước lượng" trong baseline; thêm kế hoạch bấm giờ thật ở 2 buổi lab tới vào success metric |
| Card #1: Chưa chắc bước 3 là bottleneck, có thể kẹt ở bước 4 (tìm hàm) | Không đồng ý | Khi nhớ lại, phần lớn thời gian là nghĩ nên code phần nào trước (khoảng 8'); tìm hàm chỉ khoảng 3' và trong lab lọc tin nhắn rác chỉ tra 1–3 lần (CP1 dòng #2). Giữ bước 3 là bottleneck |
| Card #1: Có thể đang nhảy sang AI sớm; checklist khung chung có thể đã đủ | Đồng ý | Đổi cảm nhận nhanh từ "Chưa biết" sang "No AI"; giả thuyết về AI chỉ cân nhắc nếu checklist không đủ |
| Card #2: 75 phút đọc có thể là thời gian học cần thiết, chưa chắc là pain; metric chỉ đo thời gian, không đo mức hiểu | Đồng ý | Thu hẹp bottleneck về đúng bước tra khái niệm (30'), không cắt thời gian đọc kỹ; thêm metric mức hiểu (tự trả lời đúng 3 câu hỏi đặt trước khi đọc) |
| Card #3: Tần suất thấp (2–3 lần), có thể chỉ là hệ quả của card #1, nên gộp với card #1? | Đồng ý một phần | Giữ card #3 vì bottleneck khác thời điểm (tự viết lại sau khi tham khảo); thêm ghi chú "Liên hệ với card #1" để nhóm có thể gộp ở CP3 |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | | | | |
| CP2 Problem Card | | | | |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
