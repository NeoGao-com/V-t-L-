---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Divergence

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Divergence đo "độ chảy ra" của một trường vector tại từng điểm: thể tích tí xíu quanh điểm đó mất chất lỏng hay nhận chất lỏng bao nhiêu (trên mỗi đơn vị thể tích). Nó gắn trường với nguồn của nó: $\nabla\cdot\vec E = \rho/\varepsilon_0$, và với định luật bảo toàn: $\partial\rho/\partial t + \nabla\cdot\vec j = 0$.

## Định nghĩa

Với trường vector $\vec A$, divergence là trường vô hướng:

$\nabla\cdot\vec A = \dfrac{\partial A_x}{\partial x} + \dfrac{\partial A_y}{\partial y} + \dfrac{\partial A_z}{\partial z}$ ([[Hệ tọa độ Descartes]])

Trong [[Hệ tọa độ cầu]]: $\nabla\cdot\vec A = \dfrac{1}{r^2}\dfrac{\partial}{\partial r}(r^2 A_r) + \dfrac{1}{r\sin\theta}\dfrac{\partial}{\partial\theta}(\sin\theta\,A_\theta) + \dfrac{1}{r\sin\theta}\dfrac{\partial A_\varphi}{\partial\varphi}$

Trong [[Hệ tọa độ trụ]]: $\nabla\cdot\vec A = \dfrac{1}{\rho}\dfrac{\partial}{\partial\rho}(\rho A_\rho) + \dfrac{1}{\rho}\dfrac{\partial A_\varphi}{\partial\varphi} + \dfrac{\partial A_z}{\partial z}$

Ý nghĩa vi phân tích: $\nabla\cdot\vec A = \lim_{V\to 0}\dfrac{1}{V}\oint_S \vec A\cdot d\vec S$ — thông lượng toàn phần chia cho thể tích ([[Định lý Gauss & Stokes]]).

## Ý nghĩa vật lý

- **Nguồn và chìm:** $\nabla\cdot\vec A > 0$ tại điểm có "vòi phun" (nguồn), $< 0$ có "cống hút" (chìm), $= 0$ trường xuyên qua mà không sinh không diệt (không chịu nén: $\nabla\cdot\vec v = 0$ cho chất lỏng không nén được).
- **Điện tích là nguồn của điện trường:** $\nabla\cdot\vec E = \rho/\varepsilon_0$ (dạng vi phân [[Định luật Gauss (điện)]]); tích phân toàn thể tích cho $Q_{\text{trong}}/\varepsilon_0$ — phát biểu "nguyên bản" của định luật Gauss.
- **Không có từ tích đơn cực:** $\nabla\cdot\vec B = 0$ — đường sức từ khép kín, không đáy không đỉnh ([[Từ trường và cảm ứng từ]]).
- **Định luật bảo toàn (liên tục):** nếu $\vec j$ là dòng gì đó và $\rho$ là mật độ thì $\partial\rho/\partial t + \nabla\cdot\vec j = 0$ — điện tích, xác suất, khối lượng đều tuân theo: đại lượng chỉ di chuyển, không sinh ra ở giữa dòng.
- **Lượng tử:** xác suất cũng bảo toàn — phương trình liên tục cho $\partial|\psi|^2/\partial t + \nabla\cdot\vec j = 0$ ([[Mật độ dòng xác suất]]); $\vec j = \dfrac{\hbar}{2mi}(\psi^*\nabla\psi - \psi\nabla\psi^*)$.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Định luật Gauss (điện)]]: dạng điểm và dạng tích phân — hai mặt của cùng div.
- [[Phương trình Maxwell]]: $\nabla\cdot\vec E = \rho/\varepsilon_0$ và $\nabla\cdot\vec B = 0$ — hai trong bốn phương trình.
- [[Mật độ dòng xác suất]]: liên tục của xác suất trong cơ học lượng tử.
- [[Từ trường và cảm ứng từ]]: đường sức từ khép kín (div bằng 0).
- [[Điện từ trường]]: sóng điện từ có $\nabla\cdot\vec E = \nabla\cdot\vec B = 0$ trong chân không — trường "không nguồn" lan truyền.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Giải tích Vector (Grad, Div, Curl)]]
- [[Gradient]]
- [[Curl]]
- [[Định lý Gauss & Stokes]]
- [[Vector]]

## Câu hỏi mở

- Div của trường điện tích điểm: $\nabla\cdot\left(\dfrac{\hat e_r}{r^2}\right) = 4\pi\delta(\vec r)$ — vì sao nguồn điểm lại "ép" ta dùng [[Hàm Dirac delta]]?
- Nếu $\nabla\cdot\vec A = 0$ với mọi nơi, liệu $\vec A$ luôn viết được thành $\nabla\times\vec B$ hay không — và điều đó nói gì về biểu diễn $\vec B = \nabla\times\vec A$? ([[Điện từ trường]].)