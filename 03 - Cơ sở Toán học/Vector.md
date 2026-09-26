---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Vector

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Vector là ngôn ngữ bắt buộc của mọi đại lượng vật lý: vị trí, vận tốc, gia tốc, lực, động lượng, mô-men. Giá trị cốt lõi của nó không phải là "có hướng", mà là **hai phép nhân cực kỳ tiện lợi** — nhân vô hướng cho ra đại lượng vô hướng, nhân hữu hướng cho ra một vector vuông góc — nhờ đó mọi bài toán tưởng hình học đều quy về đại số.

## Định nghĩa

- Vector $\vec a$ trong không gian có **độ lớn** $|\vec a|$ và **hướng**; hai vector bằng nhau khi có cùng độ lớn và cùng hướng — độc lập với hệ toạ độ. Vector chỉ đổi khi đổi hệ toạ độ, còn đại lượng vô hướng thì không ([[Tính tương đối của chuyển động]]).
- Phân tích theo một cơ sở trực giao: $\vec a = a_x\hat i + a_y\hat j + a_z\hat k$, trong đó $a_x = \vec a\cdot\hat i$ là **hình chiếu** (thành phần) của $\vec a$.

**Tích vô hướng** — kết quả là số vô hướng:

$$\vec a\cdot\vec b = |\vec a||\vec b|\cos\theta = a_xb_x + a_yb_y + a_zb_z$$

- $A = \vec F\cdot d\vec s$ — công của lực; $P = \vec F\cdot\vec v$ — công suất tức thời ([[Công và công suất]]).
- Bằng 0 ⟺ vuông góc — tiêu chuẩn kiểm tra trực giao (ví dụ $\vec F\cdot\vec v = 0$ với lực [[Lực hướng tâm]] trên chuyển động tròn đều).

**Tích hữu hướng** — kết quả là vector vuông góc với cả hai, có chiều theo quy tắc bàn tay phải:

$$\vec a\times\vec b,\qquad |\vec a\times\vec b| = |\vec a||\vec b|\sin\theta$$

- $\vec M = \vec r\times\vec F$ — mô-men lực ([[Chuyển động quay của vật rắn]]).
- $d\vec A = \vec n\,dA$ — vector diện tích có hướng, nền tảng của mọi định luật Gauss/Stokes.
- Tích chập bậc ba: $\vec a\cdot(\vec b\times\vec c)$ là **định thức** (thể tích có dấu của hình bình hành $\vec a,\vec b,\vec c$); $(\vec a\times\vec b)\times\vec c$ cho vector theo định lý BAC–CAB.

**Quy tắc tính vi phân:** $\dfrac{d}{dt}(\vec a\cdot\vec b) = \dot{\vec a}\cdot\vec b + \vec a\cdot\dot{\vec b}$ và $\dfrac{d}{dt}(\vec a\times\vec b) = \dot{\vec a}\times\vec b + \vec a\times\dot{\vec b}$ — giữ nguyên dấu "+" vì cả hai phép nhân đều song tuyến.

Trong hệ toạ độ cong, bộ đơn vị cơ sở $\hat e_1,\hat e_2,\hat e_3$ vẫn trực giao đơn vị, nhưng **thay đổi theo vị trí** — đó là lý do gradient, curl phải có hệ số $1/r$, $1/(r\sin\theta)$ trong [[Hệ tọa độ cầu]] và [[Hệ tọa độ trụ]].

## Ý nghĩa vật lý

- **Đổi hướng cũng là có gia tốc:** vật đi đều trên đường tròn vẫn có gia tốc hướng tâm $\vec a = -\dfrac{v^2}{R}\hat e_r$ ([[Lực hướng tâm]], [[Chuyển động tròn đều]]).
- **Cộng vận tốc tương đối:** $\vec v_{13} = \vec v_{12} + \vec v_{23}$ — nền của [[Tính tương đối của chuyển động]].
- **Lực là vector:** tổng các lực bằng 0 là điều kiện cân bằng ([[Cân bằng của vật rắn]]).
- **Bảo toàn mô-men:** mô-men tổng bằng 0 khi tổng lực bằng 0 và tổng mô-men ngẫu lực bằng 0.
- **Tính chất vectơ của spin:** $\vec S$ cộng theo quy tắc vector chứ không phải số học ([[Spin của hạt vi mô]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Động lượng]]: $\vec p = m\vec v$ — đổi đơn vị từ cơ sang lượng tử vẫn là vector.
- [[Lực Lorentz]]: $\vec F = q(\vec E + \vec v\times\vec B)$ — tích hữu hướng sinh ra lực từ.
- [[Động năng]] · [[Công và công suất]]: năng lượng là tích vô hướng với độ dời chuyển.
- [[Giải tích Tensor]]: khi hệ toạ độ cong, cơ sở thay đổi và cần hệ số Jacobi.
- [[Cơ học Hamilton]]: $\vec p = \nabla_{\vec q}S$ — gradient sinh ra vector từ hàm vô hướng.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Lượng giác]] · [[Số phức]] · [[Hệ tọa độ]] · [[Giải tích Vector (Grad, Div, Curl)]] · [[Gradient]]

## Câu hỏi mở

- Tại sao ba định lượng — độ dài, vector, và góc — lại đủ để xác định mọi hình học trong không gian ba chiều, nhưng không đủ trong không gian bốn chiều?
- Nếu $\vec a\times\vec b = \vec c$, liệu $\vec c$ có duy nhất khi cho trước $\vec a,\vec b$ không?
- Vì sao ba định lý Newton phải viết bằng vector mới đúng vận đạo? (Gợi ý: xem [[Các định luật Newton]].)
