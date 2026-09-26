---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Curl

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Curl (rot) đo "độ xoáy" của một trường vector tại từng điểm: **tuần hoàn của trường quanh một đường cong khép kín tí xíu**, theo định luật Stokes là bằng **thông lượng curl qua mặt bề giới hạn** bề mặt đó (chia cho diện tích mặt bề khi co về 0). Nó là nửa còn lại của phương trình Maxwell ($\nabla\times\vec E = -\partial\vec B/\partial t$), là máy dò "trường có thế không" ($\nabla\times\vec F = 0$ ⟺ $\vec F = -\nabla U$), và là vận tốc góc của mọi dòng xoáy.

## Định nghĩa

Với trường vector $\vec A$:

$\nabla\times\vec A = \det\begin{pmatrix} \hat i & \hat j & \hat k \\ \partial_x & \partial_y & \partial_z \\ A_x & A_y & A_z \end{pmatrix}$ ([[Hệ tọa độ Descartes]])

Trong [[Hệ tọa độ cầu]]:

$\nabla\times\vec A = \dfrac{1}{r\sin\theta}\left[\dfrac{\partial}{\partial\theta}(A_\varphi\sin\theta) - \dfrac{\partial A_\theta}{\partial\varphi}\right]\hat e_r + \dfrac{1}{r}\left[\dfrac{1}{\sin\theta}\dfrac{\partial A_r}{\partial\varphi} - \dfrac{\partial}{\partial r}(rA_\varphi)\right]\hat e_\theta + \dfrac{1}{r}\left[\dfrac{\partial}{\partial r}(rA_\theta) - \dfrac{\partial A_r}{\partial\theta}\right]\hat e_\varphi$

Trong [[Hệ tọa độ trụ]]:

$\nabla\times\vec A = \left[\dfrac{1}{\rho}\dfrac{\partial A_z}{\partial\varphi} - \dfrac{\partial A_\varphi}{\partial z}\right]\hat e_\rho + \left[\dfrac{\partial A_\rho}{\partial z} - \dfrac{\partial A_z}{\partial\rho}\right]\hat e_\varphi + \dfrac{1}{\rho}\left[\dfrac{\partial}{\partial\rho}(\rho A_\varphi) - \dfrac{\partial A_\rho}{\partial\varphi}\right]\hat k$

Ý nghĩa vi phân tích (định lý Stokes): $\nabla\times\vec A \cdot \hat n = \lim_{S\to 0}\dfrac{1}{S}\oint \vec A\cdot d\vec l$ — lưu số trên vòng tí xíu chia cho diện tích ([[Định lý Gauss & Stokes]]).

## Ý nghĩa vật lý

- **Máy đo xoáy:** đặt một chong chóng nhỏ vào trường — nó quay nhanh nhất theo hướng của curl. Dòng chảy xoáy quanh một xoáy nước có $\nabla\times\vec v \neq 0$; dòng thẳng đều có curl bằng 0. Vận tốc góc của chất lỏng: $\vec\omega = \dfrac{1}{2}\nabla\times\vec v$.
- **Tiêu chuẩn trường thế:** trường bảo toàn ⟺ $\nabla\times\vec F = 0$ ⟺ $\vec F = -\nabla U$ với một thế năng nào đó (liên kết chặt với [[Gradient]]); khi đó $\oint\vec F\cdot d\vec l = 0$ — công không phụ thuộc đường đi ([[Thế năng]]).
- **Điện từ:** $\nabla\times\vec E = -\partial\vec B/\partial t$ (cảm ứng điện từ — [[Từ thông và hiện tượng cảm ứng điện từ]]), $\nabla\times\vec B = \mu_0\vec j + \mu_0\varepsilon_0\partial\vec E/\partial t$ (sửa của Maxwell — dòng điện sinh từ trường xoáy, [[Từ trường của các dòng điện]], [[Phương trình Maxwell]]).
- **Trường quay mềm:** sóng điện từ trong chân không có curl của $\vec E$ và $\vec B$ khác 0 và vuông góc nhau — curl là "chất xúc tác" tạo ra trường kia khi trường này biến thiên, lan truyền thành sóng ([[Điện từ trường]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Phương trình Maxwell]]: hai phương trình cuối là câu trả lời cho "curl của $\vec E$ và $\vec B$ bằng gì?".
- [[Từ thông và hiện tượng cảm ứng điện từ]]: từ trường biến thiên sinh điện trường xoáy.
- [[Từ trường của các dòng điện]]: $\nabla\times\vec B = \mu_0\vec j$ — định luật Ampère dạng điểm.
- [[Thế năng]]: curl bằng 0 là điều kiện để tồn tại thế năng.
- [[Điện trường]] tĩnh: $\nabla\times\vec E = 0$ — điện trường tĩnh là trường thế, đường sức không khép kín.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Giải tích Vector (Grad, Div, Curl)]]
- [[Gradient]]
- [[Divergence]]
- [[Định lý Gauss & Stokes]]
- [[Vector]]

## Câu hỏi mở

- Phân tích Helmholtz: mọi trường vector hội tụ đủ nhanh = phần div (thế vô hướng) + phần curl (thế vector). Điều này nói gì về số dữ kiện cần để "dựng lại" một trường vật lý từ dữ liệu đo? ([[Hàm Green]].)
- Vì sao curl "chỉ có nghĩa" trong 3 chiều (và 7 chiều qua tích chéo)? — hai chiều chỉ còn một thành phần: curl 2D $= \partial_x A_y - \partial_y A_x$ có quan hệ gì với phép quay?