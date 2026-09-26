---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Tích phân

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Tích phân là phép toán **cộng dồn** — từ "tốc độ thay đổi" khôi phục lại "lượng tích lũy". Nó biến định luật vi phân (cục bộ, tức thời) thành định luật toàn cục (tích lũy theo cả quãng thời gian, cả không gian), và đo dòng chảy xuyên qua một mặt hay một đường cong.

## Định nghĩa

- **Tích phân Riemann:** $\displaystyle\int_a^b f(x)\,dx = \lim_{n\to\infty}\sum_{i=1}^{n} f(x_i^*)\,\Delta x_i$ với $\Delta x = (b-a)/n$. Hình học: diện tích có dấu dưới đồ thị.
- **Định lý cơ bản của giải tích (FTC):** $\displaystyle\int_a^b \dfrac{df}{dx}\,dx = f(b) - f(a)$ — phép tích phân là phép **ngược** của [[Đạo hàm]]. Nhờ đó, nghiệm của phương trình vi phân có thể tìm bằng cách tích phân: $v = \dfrac{dx}{dt} \Rightarrow x(t) = \int v\,dt + C$.
- **Tích phân bất định (improper):** khi khoảng tích hữu hạn, ví dụ $\displaystyle\int_0^\infty e^{-x}dx = 1$, $\displaystyle\int_{-\infty}^{\infty}e^{-x^2/2}dx = \sqrt{2\pi}$ — nền của phân bố Gauss.
- **Kỹ thuật tính:** đổi biến $\displaystyle\int f(g(x))g'(x)dx = \int f(u)du$; tích phân từng phần $\displaystyle\int u\,dv = uv - \int v\,du$.

Tích phần theo hình học khác — mỗi dạng đo "lượng đi qua" một đối tượng:

| Dạng | Công thức | Ý nghĩa |
| --- | --- | --- |
| Đường cong $C$ | $\displaystyle\int_C \vec F\cdot d\vec l$ | công của lực dọc theo đường đi |
| Mặt $S$ | $\displaystyle\iint_S \vec F\cdot d\vec S$ | thông lượng của trường xuyên mặt |
| Thể tích $V$ | $\displaystyle\iiint_V f\,dV$ | tổng khối lượng, mật độ, năng lượng |

Với hệ tọa độ cong, "vi phân" mang yếu tố co giãn: $dV = r^2\sin\theta\,dr\,d\theta\,d\varphi$ trong [[Hệ tọa độ cầu]], $dV = \rho\,d\rho\,d\varphi\,dz$ trong [[Hệ tọa độ trụ]].

## Ý nghĩa vật lý

- **Quãng đường là tích phân vận tốc:** $s = \displaystyle\int_{t_1}^{t_2}v(t)\,dt$ — toàn bộ [[Chuyển động thẳng biến đổi đều]] đều đạo ra từ đây (xem [[Tích phân chuyển động]]).
- **Công là tích phân lực theo đường:** $A = \displaystyle\int \vec F\cdot d\vec s$; khi $\vec F$ bảo toàn thì công phụ thuộc **đường đi** và cho ra [[Thế năng]] — hệ quả trực tiếp của [[Định lý Gauss & Stokes]].
- **Định lượng từ dòng chảy:** $\Phi = \displaystyle\iint_S \vec B\cdot d\vec S$ là từ thông ([[Từ thông và hiện tượng cảm ứng điện từ]]); $\displaystyle\iint_S \vec j\cdot d\vec S$ là dòng điện qua một mặt cắt.
- **Tích lũy động lượng (xung lực):** $\displaystyle\int \vec F\,dt = \Delta\vec p$ — bảo toàn trong [[Va chạm]] khi lực tức thời bù trừ nhau.
- **Vận tốc giới hạn:** từ $m\dfrac{dv}{dt} = mg - kv$ suy ra $v_\infty = \dfrac{mg}{k}$ bằng cách lấy giới hạn khi $\dfrac{dv}{dt}\to 0$ ([[Lực ma sát]]).
- **Nhiệt lượng và công nén khí:** $Q = \displaystyle\int C\,dT$, $A = \displaystyle\int p\,dV$ ([[Công của khối khí]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Tích phân chuyển động]]: quãng đường, quãng đường tròn, chu kỳ.
- [[Công và công suất]] · [[Thế năng]]: công và thế năng là tích phân của lực.
- [[Định lý Gauss & Stokes]]: tích phân mặt và tích phân đường được quy về cùng một dạng.
- [[Điện thế và hiệu điện thế]]: $V = \displaystyle\int\vec E\cdot d\vec l$ cho hiệu điện thế.
- [[Phương trình trạng thái khí lý tưởng]] · [[Nhiệt lượng và cách truyền nhiệt]]: các đại lượng thể tích đều là tích phân mật độ.
- [[Entropy]] · [[Xác suất thống kê]]: tích phân của hàm mật độ xác suất là kỳ vọng.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Đạo hàm]] · [[Phương trình vi phân]] · [[Giải tích Vector (Grad, Div, Curl)]] · [[Định lý Gauss & Stokes]]
- [[Toán tử Laplace]] · [[Phương trình đạo hàm riêng (PDE)]]

## Câu hỏi mở

- Vì sao tích phân của một hàm lẻ trên khoảng đối xứng bằng 0, nhưng tích phân hàm **chẵn** lại không nhất thiết cho con số "không có ý nghĩa"? (Gợi ý: hãy nghĩ về trọng lượng riêng và thể tích.)
- Vì sao tích phân trên đường cong lại phụ thuộc **hướng** đi, trong khi tích phân mặt thì không?
- Điều gì xảy ra nếu hàm bị tích phân không liên tục? (Gợi ý: xem [[Hàm Dirac delta]] — một phân bố chưa bao giờ có điểm nào bằng 0 hay vô hạn.)
