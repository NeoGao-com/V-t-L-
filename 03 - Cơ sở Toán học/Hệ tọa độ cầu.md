---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Hệ tọa độ cầu

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Tọa độ cầu $(r, \theta, \varphi)$ là "ngôn ngữ mẹ đẻ" của mọi bài toán có đối xứng quanh một tâm — trường xuyên tâm, nguyên tử Hydro, sóng từ nguồn điểm. Nó biến hàm sóng thành tích hàm bán kính × hàm cầu $Y_{lm}$, và phần tử thể tích $r^2\sin\theta\,dr\,d\theta\,d\varphi$ điều khiển mật độ xác suất electron.

## Định nghĩa

Quy ước vật lý: $r$ — bán kính ($r \ge 0$); $\theta$ — góc cực **từ trục $z$** ($0\le\theta\le\pi$); $\varphi$ — góc phương vị từ trục $x$ ($0\le\varphi<2\pi$):

$x = r\sin\theta\cos\varphi, \qquad y = r\sin\theta\sin\varphi, \qquad z = r\cos\theta$

- Phần tử độ dài: $d\vec l = dr\,\hat e_r + r\,d\theta\,\hat e_\theta + r\sin\theta\,d\varphi\,\hat e_\varphi$ — vector đơn vị **đổi hướng theo vị trí** (khác [[Hệ tọa độ Descartes]]).
- Phần tử thể tích: $dV = r^2\sin\theta\,dr\,d\theta\,d\varphi$; góc khối $d\Omega = \sin\theta\,d\theta\,d\varphi$.
- Gradient: $\nabla f = \dfrac{\partial f}{\partial r}\hat e_r + \dfrac{1}{r}\dfrac{\partial f}{\partial\theta}\hat e_\theta + \dfrac{1}{r\sin\theta}\dfrac{\partial f}{\partial\varphi}\hat e_\varphi$.
- [[Toán tử Laplace]]: $\nabla^2 f = \dfrac{1}{r^2}\dfrac{\partial}{\partial r}\left(r^2\dfrac{\partial f}{\partial r}\right) + \dfrac{1}{r^2\sin\theta}\dfrac{\partial}{\partial\theta}\left(\sin\theta\dfrac{\partial f}{\partial\theta}\right) + \dfrac{1}{r^2\sin^2\theta}\dfrac{\partial^2 f}{\partial\varphi^2}$.

## Ý nghĩa vật lý

- **Đối xứng tâm trở nên hiển nhiên:** $V(\vec r) = V(r)$ — mọi hướng là như nhau; tách biến bán kính × góc đưa phương trình Schrödinger về phương trình bán kính cho $u(r) = rR(r)$ ([[Phương trình Schrödinger trong trường xuyên tâm]]).
- **Hàm cầu $Y_{lm}(\theta,\varphi)$:** hàm riêng chung của $\hat{\vec L}^2$ và $\hat L_z$ xuất hiện tự nhiên như phần góc — lượng tử hóa không gian ([[Toán tử mô-men xung lượng]], [[Thí nghiệm - Stern-Gerlach]]).
- **Nhân tử $r^2$ trong $dV$:** mật độ xác suất bán kính của electron là $P(r) = r^2|R(r)|^2$ (khác $|R|^2$!) — đỉnh 1s tại bán kính Bohr $a_0$ chỉ xuất hiện nhờ yếu tố thể tích ([[Sự phân bố electron trong nguyên tử Hydro]]).
- **Trường Coulomb:** số mũ $e^{-kr}$ tách được, suy biến $n^2$ của nguyên tử Hydro ([[Nguyên tử Hydro]]); sóng pháp tuyến từ nguồn điểm cũng lan cầu đối xứng.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Trường xuyên tâm]]: đại số sử dụng tọa độ cầu cho mọi thế $V(r)$.
- [[Nguyên tử Hydro]]: nghiệm $R_{nl}(r)Y_{lm}$ — ba số lượng tử $(n,l,m)$ sinh từ tách biến cầu.
- [[Toán tử mô-men xung lượng]]: $Y_{lm}$ và tính $l(l+1)\hbar^2$, $m\hbar$.
- [[Điện trường]] từ [[Điện tích và bảo toàn điện tích|điện tích điểm]]: $\vec E = \dfrac{q}{4\pi\varepsilon_0 r^2}\hat e_r$ — mọi đại lượng chỉ phụ thuộc $r$.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Hệ tọa độ]]
- [[Hệ tọa độ trụ]]
- [[Hệ tọa độ Descartes]]
- [[Toán tử Laplace]]
- [[Lượng giác]]

## Câu hỏi mở

- Tại $\theta = 0, \pi$ (trục $z$), $\varphi$ không xác định — "điểm kỳ dị tọa độ" này ảnh hưởng thế nào tới điều kiện biên của $Y_{lm}$? (Hàm cầu vẫn trơn vì là hàm của $\cos\theta$.)
- Hành vi $r \to 0$ của phương trình bán kính đòi hỏi $u(0) = 0$ — vì sao chỉ mình tọa độ cầu "phơi bày" điều kiện này, còn Descartes giấu nó? ([[Phương trình Schrödinger trong trường xuyên tâm]].)