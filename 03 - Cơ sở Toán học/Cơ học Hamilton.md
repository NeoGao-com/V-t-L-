---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Cơ học Hamilton

> [!abstract] Công cụ để làm gì
> Cơ học Hamilton "xắp xếp lại" cơ học Lagrange thành **không gian pha** — mỗi trạng thái của hệ là một điểm, tiến hóa là một dòng chảy. Đây là hình thức trực tiếp nhất để bước sang cơ học lượng tử: $\hat H$ trong phương trình Schrödinger chính là Hamiltonian cổ điển được "nâng cấp" thành toán tử.

## Định nghĩa

- **Biến đổi Legendre:** từ tọa độ suy rộng $q$ và vận tốc $\dot q$ của [[Cơ học Lagrange]], định nghĩa **động lượng suy rộng** $p_i = \dfrac{\partial L}{\partial \dot q_i}$ và **Hamiltonian**
  $H(q, p, t) = \sum_i p_i \dot q_i - L$
  — đổi biến từ $(q, \dot q)$ sang $(q, p)$.
- **Phương trình Hamilton:** thay Euler–Lagrange bậc hai bằng **2 phương trình bậc nhất** đối xứng:
  $\dot q_i = \dfrac{\partial H}{\partial p_i}, \qquad \dot p_i = -\dfrac{\partial H}{\partial q_i}$
- **Không gian pha:** không gian $2n$ chiều $(q_1...q_n, p_1...p_n)$; mỗi trạng thái một điểm, mỗi quỹ đạo một đường dòng chảy không cắt nhau.
- **Móc Poisson:** $\{A, B\} = \sum_i \left(\dfrac{\partial A}{\partial q_i}\dfrac{\partial B}{\partial p_i} - \dfrac{\partial A}{\partial p_i}\dfrac{\partial B}{\partial q_i}\right)$ — công cụ đo "giao hoán" của hai đại lượng.

So sánh hai khung nhìn cùng một hệ:

| | Lagrange | Hamilton |
| --- | --- | --- |
| Biến | $(q, \dot q)$ | $(q, p)$ |
| Số PTVP | $n$ phương trình bậc 2 | $2n$ phương trình bậc 1 |
| Phương trình | Euler–Lagrange $\dfrac{d}{dt}\dfrac{\partial L}{\partial \dot q_i} = \dfrac{\partial L}{\partial q_i}$ | $\dot q_i = \partial H/\partial p_i$, $\dot p_i = -\partial H/\partial q_i$ |
| Bức tranh | Quỹ đạo trong không gian cấu hình | Dòng chảy trong không gian pha |
| Sức mạnh nhất | PTVP bậc 2 thân thiện với cơ cổ điển | Cấu trúc bảo toàn + cầu nối lượng tử/thống kê |

## Ý nghĩa hình học

- Không gian pha "đóng gói" vị trí và động lượng thành một bức tranh trọn vẹn: quỹ đạo tuần hoàn là vòng kín, dao động tắt dần là xoắn ốc vào điểm cân bằng.
- $H$ là "năng lượng" của bức tranh: dòng chảy không gian pha chảy dọc theo mặt $H = \text{const}$.
- **Định lý Liouville:** dòng chảy Hamilton **bảo toàn thể tích** không gian pha — "chất lỏng" trạng thái không thể bị nén, chỉ bị xoắn thành sợi mảnh. Đây là nguồn gốc hình học của việc các quỹ đạo "gần nhau thì ở gần nhau" mãi (trước khi có hỗn loạn) và là nền móng của cơ học thống kê.

## Ý nghĩa vật lý

- **Ví dụ mẫu — dao động điều hòa:** $H = \dfrac{p^2}{2m} + \dfrac{1}{2}kx^2$; không gian pha là họ **ellipse** đồng tâm (mỗi ellipse một năng lượng), quỹ đạo chạy vòng quanh đều — trực quan đẹp hơn nhiều so với phương trình chuyển động. Với con lắc đơn, $H = \dfrac{p^2}{2ml^2} - mgl\cos\theta$: năng lượng thấp → ellipse; năng lượng chạm đỉnh → **đường phân cách (separatrix)** mà trên đó con lắc "ngả mệt" xuống hồi lâu ([[Con lắc đơn]], [[Dao động điều hòa]]).
- **Cầu nối lượng tử trực tiếp nhất:** lượng tử hóa "kinh điển" là thay $p \to -i\hbar\partial/\partial q$ vào $H$ → toán tử $\hat H$; phương trình Hamilton trở thành phương trình Schrödinger ([[Tiên đề cơ học lượng tử]], [[Phương trình Schrödinger]]).
- **Móc Poisson là "tiền thân" của giao hoán tử:** $\{A, B\}$ cổ điển ↔ $[\hat A, \hat B]/i\hbar$ lượng tử — nền của [[Nguyên lý bất định Heisenberg]] (các đại lượng móc Poisson khác không là không giao hoán).
- **Bảo toàn = đối xứng:** $H$ không phụ thuộc $q_i$ → $p_i$ bảo toàn — cách nhìn Hamilton của định lý [[Định lý Noether]]; tổng quát: $\dot A = \{A, H\}$.
- **Nền của nhiệt động lực học thống kê:** thể tích không gian pha bảo toàn + xoắn sợi mảnh → dù vi mô xác định, nhìn thô ở vĩ mô vẫn là phân bố xác suất ([[Xác suất thống kê]], [[Thuyết động học phân tử]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Tiên đề cơ học lượng tử]] · [[Phương trình Schrödinger]]: Hamiltonian là toán tử năng lượng.
- [[Nguyên lý bất định Heisenberg]]: móc Poisson ↔ giao hoán tử.
- [[Cơ học Lagrange]]: hai khung nhìn cùng một hệ — Lagrange cho phương trình chuyển động, Hamilton cho cấu trúc không gian pha.
- [[Định lý Noether]]: bảo toàn qua sự "lờ đi" biến của $H$.
- [[Dao động điều hòa]] · [[Con lắc đơn]] · [[Cơ năng]]: $H = T + V$ là năng lượng toàn phần; ellipse và separatrix trong không gian pha.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Cơ học Lagrange]] · [[Phép tính biến phân]] · [[Định lý Noether]] · [[Tiên đề cơ học lượng tử]] · [[Phương trình Schrödinger]] · [[Lý thuyết nhóm]] (đối xứng ↔ bảo toàn)

## Câu hỏi mở

- Vì sao hệ có $n$ phương trình Lagrange bậc hai lại "tương đương" hệ $2n$ phương trình Hamilton bậc nhất — và lợi ích thực sự của không gian pha là gì? (Gợi ý: nhìn "trạng thái" thay vì "quỹ đạo" — thay đổi cách đặt câu hỏi trong cơ học thống kê và lượng tử.)
- Lượng tử hóa "thay $p$ bằng đạo hàm" hoạt động tốt ở tọa độ Descartes nhưng hỏng khi đổi tọa độ cong — vì sao? (Gợi ý: móc Poisson không đổi trong mọi phép biến đổi chính tắc; lịch sử của lượng tử hóa hình học.)
- Liouville bảo toàn thể tích, vậy entropy **tăng** ở đâu ra trong cơ học thống kê? (Gợi ý: thể tích bảo toàn nhưng "đám mây" trạng thái xoắn thành sợi mảnh vô hạn — thông tin "tinh" trở thành nhiệt khi ta chỉ nhìn thô — liên hệ [[Nguyên lý thứ hai nhiệt động lực học]].)