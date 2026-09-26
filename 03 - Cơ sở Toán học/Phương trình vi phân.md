---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Phương trình vi phân

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Phương trình vi phân là bản "công thức hoá" của định luật vật lý: nó nói rõ quan hệ giữa một đại lượng và **tốc độ thay đổi** của nó. Mọi định luật cơ học cổ điển — Newton, năng lượng, bảo toàn — đều là phương trình vi phân khi diễn đạt bằng toán giải tích. Ngược lại, **giải** phương trình vi phân là biến luật vật lý thành quỹ đạo cụ thể.

## Định nghĩa

- Phương trình chứa ẩn hàm $x(t)$ và các đạo hàm của nó. **Bậc** = số đạo hàm lớn nhất.
- **Bài toán điều kiện đầu (IVP):** cho thêm điều kiện ban đầu (vị trí, vận tốc tại $t=0$) → nghiệm duy nhất. Đây là dạng đúng của vật lý: biết trạng thái hiện tại là xác định được tương lai.
- **Bài toán điều kiện biên (BVP):** cho giá trị ở hai đầu, ví dụ dây đàn rung hai đầu cố định — nghiệm có thể không tồn tại hoặc không duy nhất.

**Điều kiện tồn tại – duy nhất (Picard–Lindelöf):** nếu $f(x,t)$ và $\partial f/\partial x$ liên tục quanh điểm ban đầu thì có **đúng một** nghiệm. Đây là hình thức toán học của định lý tiên đoán: quy luật xác định thì không có hai lịch sử khác nhau cùng xuất phát từ một trạng thái.

### Phương trình tuyến tính

Dạng $a_nx^{(n)} + \dots + a_1x' + a_0x = b(x)$ — hầu hết phương trình trong vật lý rơi vào đây. Ba bước giải:

1. **Phương trình đồng nhất** ($b=0$): thử $x = e^{\lambda t}$ → **phương trình đặc trưng** $\lambda^n + \dots = 0$.
   - Nghiệm phức $\lambda = \pm i\omega$ cho cặp dao động: $e^{\pm i\omega t} \to \cos\omega t,\ \sin\omega t$ — toàn bộ [[Dao động điều hòa]].
   - Nghiệm thực âm $\lambda = -\gamma$ → **tắt dần** theo hàm mũ.
   - Nghiệm lặp $\lambda$ kép → nhân thêm $t$ ($te^{-\gamma t}$) — biên độ vẫn giảm.
2. **Phương trình không đồng nhất:** thế hàm đặc biệt vào dạng chưa có phương pháp.
3. **Cộng nghiệm riêng** để thoả điều kiện đầu — đó chính là ý nghĩa của hai hằng số tích phân trong $x = A\cos\omega t + B\sin\omega t$.

**Cộng hưởng:** nếu tần số cưỡng bức trùng tần số riêng, nghiệm phải có dạng $t\sin\omega_0 t$ — biên độ **vô hạn** trong mô hình không mất ([[Dao động tắt dần - Cưỡng bức - Cộng hưởng]]).

## Ý nghĩa vật lý

- **Newton dạng vi phân:** $\vec F = m\dfrac{d\vec v}{dt}$ — biết lực là biết phương trình điều khiển toàn bộ chuyển động ([[Định luật II Newton]]).
- **Dao động lò xo:** $m\ddot x + kx = 0 \to x = A\cos(\omega t+\varphi)$ với $\omega = \sqrt{k/m}$ — nền của [[Con lắc lò xo]] và [[Con lắc đơn]].
- **Vận tốc giới hạn:** $m\dfrac{dv}{dt} = mg - kv$ — bậc một, tách được, nghiệm tiến tới hằng số.
- **Tuổi thọ phân rã:** $\dfrac{dN}{dt} = -\lambda N$ cho $N = N_0e^{-\lambda t}$ ([[Phóng xạ]]).
- **Mạch RLC:** $L\dfrac{di}{dt} + Ri + \dfrac{q}{C} = 0$ — nghiệm phức cho trở kháng $Z$ ([[Mạch RLC và trở kháng]]).
- **Tách biến trong Schrödinger:** $i\hbar\dfrac{\partial\psi}{\partial t} = \hat H\psi$ là hệ phương trình vi phân theo thời gian, dùng để tách miền ([[Tách biến trong phương trình Schrödinger ba chiều]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Các định luật Newton]] · [[Định luật II Newton]]: định luật vật lý ở dạng toán giải tích.
- [[Định lý Noether]]: đạo hàm bậc nhất từ nguyên lý biến đổi → bất biến của phương trình vi phân Lagrange.
- [[Hàm Green]]: lời giải tổng quát của phương trình tuyến tính với điều kiện đầu.
- [[Cơ học Hamilton]]: hệ phương trình chuẩn hoá $qdot = \partial H/\partial p$ — dạng chuẩn của hệ phương trình vi phân hạng nhất.
- [[Phương trình trạng thái khí lý tưởng]]: quan hệ giữa các biến trạng thái là tích phân của phương trình vi phân điều chỉnh.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Đạo hàm]] · [[Tích phân]] · [[Số phức]] · [[Phép biến đổi Laplace]]
- [[Phương trình đạo hàm riêng (PDE)]]

## Câu hỏi mở

- Vì sao "cùng một phương trình, khác điều kiện đầu" lại cho hai kịch bản hoàn toàn khác nhau — và điều đó có đúng là "quy luật không tất định thế giới" không?
- Phương trình không tuyến tính (ví dụ chuyển động dưới lực hấp dẫn, [[Trọng lực]]) có "phương pháp giải tổng quát" nào không, hay phải trao đổi giữa tính chính xác và tính giải tích?
- Cộng hưởng có thật sự vô hạn trong vật lý không, nếu luôn có mất năng lượng? (Gợi ý: [[Xử lý sai số thực nghiệm]].)
- Hàm nào là "hàm riêng" của phương trình vi phân tự phụ thuộc? (Gợi ý: xem [[Toán tử trong cơ học lượng tử]].)
