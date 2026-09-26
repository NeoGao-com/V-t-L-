---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: nhiệt-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Phương trình van der Waals

> [!abstract] Ý chính
> Hiệu chỉnh phương trình khí lý tưởng cho khí thực bằng hai tham số: $a$ (lực hút giữa phân tử làm giảm áp suất) và $b$ (thể tích chiếm chỗ của phân tử làm giảm khoảng trống) — giải thích được hiện tượng hóa lỏng và điểm tới hạn mà khí lý tưởng bất lực.

## Phát biểu / Định nghĩa

- **Khí lý tưởng:** $pV = nRT$ — xem [[Phương trình trạng thái khí lý tưởng]].
- **Van der Waals (1873):**
  $\left(p + \frac{a n^2}{V^2}\right)(V - nb) = nRT$
  - $a$: tham số lực hút giữa các phân tử — phân tử gần thành bình bị kéo ngược vào trong, áp suất đo được nhỏ đi $a n^2/V^2$.
  - $b$: thể tích chiếm chỗ của 1 mol phân tử — khoảng trống thực chỉ còn $V - nb$.
- Khi $a = b = 0$, hoặc khí đủ loãng ($V$ lớn), phương trình trở về khí lý tưởng.

## Bảng tham số một số khí

| Khí | $a$ (Pa·m⁶/mol²) | $b$ (10⁻⁶ m³/mol) | $T_c$ thực (K) |
| --- | --- | --- | --- |
| H₂ | 0,0248 | 26,6 | 33,2 |
| N₂ | 0,137 | 38,7 | 126,2 |
| CO₂ | 0,364 | 42,7 | 304,1 |
| H₂O | 0,553 | 30,5 | 647,1 |

Quy luật: phân tử càng lớn/tương tác càng mạnh (H₂O, CO₂) thì $a$, $b$ càng lớn — khí càng dễ hóa lỏng.

## Điểm tới hạn

Từ phương trình van der Waals suy ra (điểm uốn của đường đẳng nhiệt):

$T_c = \frac{8a}{27Rb}, \quad p_c = \frac{a}{27b^2}$

**Kiểm tra số với CO₂:** $T_c = \dfrac{8\times0{,}364}{27\times8{,}314\times42{,}7\times10^{-6}} \approx 304$ K ($T_c$ thực = 304,1 K) và $p_c \approx 7{,}4$ MPa ≈ 73 atm (thực ≈ 73,8 bar) — khớp ấn tượng với thực nghiệm cho một mô hình đơn giản.

Hiểu ý nghĩa: trên $T_c$ khí **không hóa lỏng được dù nén tới đâu** — dưới $T_c$, đường đẳng nhiệt có vùng uốn (khớp quan sát hóa lỏng; nhánh không ổn định được thay bằng đường nằm ngang theo quy tắc Maxwell).

## Ví dụ vật lý cụ thể

- **Chai khí CO₂ lỏng:** ở 300 K (dưới $T_c$ = 304 K), CO₂ có thể tồn tại lỏng + hơi trong bình nén — khí lý tưởng không giải thích được.
- **Khí heli lỏng:** $T_c$ của He chỉ ~5,2 K — phải làm lạnh dưới 5 K heli mới hóa lỏng được (thành tựu Kamerlingh Onnes 1908).
- **Hệ số nén $z = pV/nRT$:** khí lý tưởng có $z = 1$; khí thực $z < 1$ ở áp suất vừa (hút chiếm ưu thế) và $z > 1$ ở áp suất cao (thể tích chiếm chỗ chiếm ưu thế) — đo $z$ cho phép xác định $a$, $b$.

## Suy luận từ đâu

- Tiên đề gốc: [[Nguyên lý thứ nhất nhiệt động lực học]] — phương trình trạng thái là quan hệ khép kín giữa $p, V, T$.
- Công cụ toán: [[Xác suất thống kê]] — mô hình phân tử có kích thước hữu hạn và tương tác hút; khớp với [[Thuyết động học phân tử]] khi bỏ hiệu chỉnh.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: dự đoán điểm tới hạn, hóa lỏng, hệ số nén — khớp định tính và bán định lượng với khí thực ở áp suất vừa phải.
- Trường hợp không còn đúng: áp suất rất cao hoặc gần điểm tới hạn (cần phương trình chính xác hơn: virial, Redlich–Kwong, Soave...); pha lỏng đậm đặc và lực liên phân tử phức tạp ngoài phạm vi mô hình.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Phương trình trạng thái khí lý tưởng]] · [[Chất khí và khí lý tưởng]] · [[Nội năng]] · [[Nhiệt độ và thang nhiệt độ]] · [[Nguyên lý thứ nhất nhiệt động lực học]]
- [[Thuyết động học phân tử]]: nền tảng vi mô của mô hình khí.

## Câu hỏi mở

- Từ $a, b$ của một chất, có thể suy ra trực tiếp nhiệt độ bay hơi hoặc cấu trúc phân tử không? (Liên hệ lực liên phân tử và xác suất thống kê.)
- Vì sao ở áp suất cao, $z$ tăng vượt 1 — "thể tích chiếm chỗ" có phải là hiệu ứng thực của kích thước phân tử hay chỉ là tham số khớp số liệu? (Gợi ý: ở áp suất cao, lực đẩy tầm ngắn chiếm ưu thế.)