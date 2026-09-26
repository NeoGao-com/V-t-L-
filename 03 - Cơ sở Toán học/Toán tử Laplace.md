---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Toán tử Laplace

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Toán tử Laplace $\nabla^2 = \nabla\cdot\nabla$ là "đạo hàm bậc hai tổng hợp" của trường tại một điểm — độ cong trung bình theo mọi hướng. Nó là toán tử động năng của cơ học lượng tử ($\hat K = -\dfrac{\hbar^2}{2m}\nabla^2$) và nằm trong trái tim của mọi phương trình sóng, khuếch tán, điện tĩnh.

## Định nghĩa

Với trường vô hướng $f(x,y,z)$:

$\nabla^2 f = \dfrac{\partial^2 f}{\partial x^2} + \dfrac{\partial^2 f}{\partial y^2} + \dfrac{\partial^2 f}{\partial z^2}$ ([[Hệ tọa độ Descartes]])

Trong [[Hệ tọa độ cầu]] $(r,\theta,\varphi)$:

$\nabla^2 f = \dfrac{1}{r^2}\dfrac{\partial}{\partial r}\left(r^2\dfrac{\partial f}{\partial r}\right) + \dfrac{1}{r^2\sin\theta}\dfrac{\partial}{\partial\theta}\left(\sin\theta\dfrac{\partial f}{\partial\theta}\right) + \dfrac{1}{r^2\sin^2\theta}\dfrac{\partial^2 f}{\partial\varphi^2}$

Trong [[Hệ tọa độ trụ]] $(\rho,\varphi,z)$:

$\nabla^2 f = \dfrac{1}{\rho}\dfrac{\partial}{\partial\rho}\left(\rho\dfrac{\partial f}{\partial\rho}\right) + \dfrac{1}{\rho^2}\dfrac{\partial^2 f}{\partial\varphi^2} + \dfrac{\partial^2 f}{\partial z^2}$

Hàm riêng: $e^{i\vec k\cdot\vec r}$ (sóng phẳng) với $\nabla^2 e^{i\vec k\cdot\vec r} = -|\vec k|^2 e^{i\vec k\cdot\vec r}$ — nền của [[Biến đổi Fourier]]. (Dùng $|\vec k|^2 = k_x^2+k_y^2+k_z^2$ chứ không phải $k^2$ khi $\vec k$ là vectơ.)

## Ý nghĩa vật lý

- **Vận hành như "độ cong trung bình":** $\nabla^2 f > 0$ nghĩa là điểm đang "lõm" so với trung bình hàng xóm (thung lũng bị san bằng khi khuếch tán) — tín hiệu để phương trình nhiệt $\partial_t T = D\nabla^2 T$ "làm phẳng" mọi nhọn gai.
- **Nguồn gốc toán tử động năng:** trong cơ học lượng tử $\hat H = -\dfrac{\hbar^2}{2m}\nabla^2 + V(\vec r)$ ([[Phương trình Schrödinger]]) — phần Laplace sinh từ $p^2/2m$ khi thay $\hat{\vec p} = -i\hbar\nabla$ ([[Các toán tử cơ bản trong cơ học lượng tử]]).
- **Phương trình Laplace & Poisson:** $\nabla^2 V = 0$ (chân không) và $\nabla^2 V = -\rho/\varepsilon_0$ (Poisson) điều khiển trường thế tĩnh điện, hấp dẫn ([[Điện thế và hiệu điện thế]], [[Định luật Gauss (điện)]]).
- **Bất biến quay:** vì thang đo theo mọi hướng như nhau, $\nabla^2$ không đổi dưới phép quay — nên $\hat K$ giao hoán với $\hat{\vec L}$: nguồn của tính $\hat{\vec L}$ bảo toàn trong trường xuyên tâm ([[Toán tử mô-men xung lượng]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Phương trình Schrödinger]]: dạng cầu của $\nabla^2$ biến bài toán nguyên tử thành phương trình bán kính + góc ([[Trường xuyên tâm]], [[Nguyên tử Hydro]]).
- [[Dao động tử điều hòa lượng tử]]: $\nabla^2$ phân cực dẫn tới tách biến và bậc năng lượng đều.
- [[Phương trình đạo hàm riêng (PDE)]]: sóng, nhiệt, Schrödinger đều là "phương trình chứa $\nabla^2$".
- [[Phương trình Maxwell]]: sóng điện từ trong chân không rút về $\nabla^2\vec E = \mu_0\varepsilon_0\,\partial^2\vec E/\partial t^2$.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Gradient]]
- [[Hệ tọa độ cầu]]
- [[Hệ tọa độ trụ]]
- [[Hệ tọa độ Descartes]]
- [[Đạo hàm]]

## Câu hỏi mở

- $\nabla^2$ bất biến quay nhưng $\partial^2/\partial x^2$ thì không — vì sao "tổng bình phương các đạo hàm riêng" lại là đại lượng vô hướng? (Liên hệ metric và tensor — [[Giải tích Tensor]], [[Hình học vi phân]].)
- Hàm riêng của $\nabla^2$ trong hộp (phổ gián đoạn) so với sóng phẳng (phổ liên tục) — phổ của toán tử quyết định gì về hệ vật lý? ([[Giếng thế vô hạn]], [[Hạt tự do trong cơ học lượng tử]].)