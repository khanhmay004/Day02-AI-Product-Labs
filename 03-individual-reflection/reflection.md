# Phase 7 — Individual Reflection

> Học viên: Võ Huyền Khánh Mây

---

## 1. AI đã hỗ trợ mình trong lab thế nào?

### Chỗ AI thực sự giúp
- **Brainstorm scan 6 problems**: mình dùng AI để thử 4 lăng kính cho mỗi pain mình đang sống, hỏi "nếu nhìn qua lăng kính Lặp lại thì điểm khó nhất là gì?". AI giúp mình phân biệt được vấn đề "đi tìm ổ cắm" (không phải bài toán AI) khỏi "câu hỏi lặp lại của học viên" (đúng AI fit) — nhanh hơn tự nghĩ.
- **Vẽ workflow Mermaid**: mình mô tả workflow bằng lời, AI generate Mermaid syntax + suggest fallback path mình chưa nghĩ ra (case "TA queue quá tải"). Tiết kiệm ~20'.
- **Sanity check Problem Statement v1**: mình paste v1 và yêu cầu AI critique theo 9 yếu tố b2.pdf. AI bắt được 2 chỗ metric chưa SMART (NPS proxy thiếu baseline cách đo).
- **So sánh tool research**: mình hỏi AI tóm tắt pricing Mendable vs Kapa vs Inkeep — confirm với mình 2 trong 4 tool quá đắt.

### Chỗ AI sai hoặc hời hợt mà mình phải sửa
- **Lúc đầu AI đề xuất "build multi-agent system với 3 agent: Q&A, Logistics, Analytics"** — đúng theo painpoint ban đầu của mình, nhưng đó là **solution-first**. Mình đã từng định cho Agent vào Mức chọn ngay lập tức. Sau khi đọc lại slide.pdf phần "Rule không kém Agent nếu giải đúng bài với ít rủi ro hơn", mình bắt mình tự hỏi: cái này có thật sự cần Agent không? Validate xong thấy 80% câu là low-complexity → chọn Workflow chứ không Agent.
- **AI ban đầu viết Problem Statement v1 quá "đẹp" — như marketing copy**. Mình phải bắt nó cụ thể hơn: actor không phải "TA và học viên", là "4 TA part-time × 10h/tuần / 500 học viên với 3 phân khúc cụ thể". AI giúp khi mình prompt rõ, nhưng nếu không prompt rõ thì nó sẽ viết hời hợt.
- **AI generate quá nhiều risk** (10+ risk khi tôi hỏi). Mình phải tự chọn 6 risk quan trọng nhất và viết mitigation cụ thể.

---

## 2. Vai trò + đóng góp của mình trong nhóm

### Vai trò chính
- **Người viết workflow Mermaid** trước/sau (Phase 5a).
- Tham gia hoàn thành thảo luận


### Nếu được điểm 0-10 cho contribution của mình, mình tự cho **7.5/10**
Vì mình đã pitch, kéo data, defend, viết được phần Workflow + Problem Statement.

---

## 3. Điều mình học được sau lab này

### Bài học cụ thể nhất
**Pain rõ + workflow rõ → tier AI tự lộ ra. Pain mờ + workflow không vẽ được → mọi tier đều sai.**
Ban đầu mình rất hứng "multi-agent system Q&A + Logistics + Analytics" vì nghe cool. Sau khi vẽ workflow cụ thể 7 bước và đếm số câu hỏi từng loại, **80% câu là low-complexity → không cần Agent, Workflow + RAG đủ**. Cùng painpoint, cùng mình, nếu không bắt buộc vẽ workflow + đếm số thì rất có khả năng đã chọn Agent → over-engineer → rủi ro → lãng phí.

### Bài học về AI
- AI giỏi **draft + critique**, nhưng dở **anchor decision bằng data thật**. Cái sau vẫn phải mình làm.
- AI có **bias về phía giải pháp hấp dẫn** (multi-agent, "smart"), không có instinct tự dừng lại để hỏi "có cần thật không".
- AI rất giúp khi mình đã có constraint rõ (ví dụ: "viết theo 9 yếu tố b2.pdf, mỗi yếu tố < 50 từ"). Mơ hồ → output mơ hồ.

### Bài học về làm nhóm
- Challenge **đúng trọng tâm** quan trọng hơn challenge nhiều. Tuấn chỉ hỏi 2 câu nhưng cả 2 đều buộc mình đi kéo data thật.
- Pitcher không nên defend bằng reasoning, nên defend bằng data. Mình tự nhận lúc đầu suýt defend "tao thấy nó lặp lại nhiều mà" 

### Bài học về Rule / Workflow / Agent
- **Rule đã âm thầm có sẵn** (pinned FAQ) và **đang fail** không phải vì Rule yếu, mà vì **discoverability + UX kém** (học viên không scroll). Workflow giải được phần đó (push proactive thay vì pull).
- Mức chọn không phải về "AI có giỏi không", mà là "ai chịu trách nhiệm khi sai + sai thì khắc phục được không". Workflow có HITL rõ → chọn được.

---

## 4. Nếu làm lại, mình sẽ đổi gì?

| Thứ mình sẽ đổi | Vì sao |
|---|---|
| **Đi phỏng vấn TA trực tiếp từ Phase 2**, không đợi Phase 4 | Nếu phỏng vấn sớm, Problem Card của mình ở Phase 2 sẽ có evidence ngay, không phải defend bằng "tao nghĩ là 60%" |
| **Viết Problem Statement v0 ngắn nhưng chân thật** (kiểu "tao chưa biết") thay vì viết v0 hoành tráng | v0 mình viết bị "tỏ ra biết" — chính là dạng solution-first b2.pdf cảnh báo |
| **Set baseline survey instrument trước lab** | Mình target NPS +25% nhưng baseline NPS Q&A chưa có. Đáng lẽ tuần trước lab nên chạy survey baseline. |
| **Không skip phần "phương án không AI"** | Lúc đầu mình bỏ qua "thuê thêm 2 TA" vì nghĩ "đắt, không bền vững". Sau khi list ra so sánh chi phí mới thấy đó là cách quan trọng để justify Workflow tier. |
| **Đặt câu hỏi pitcher khác sớm hơn** | Mình đã challenge Tuấn và Linh OK, nhưng chỉ ở Phase 3. Nếu vào Phase 2 đã có challenge nhẹ thì nhóm có thể loại được #4, #5, #6 nhanh hơn. |

---
