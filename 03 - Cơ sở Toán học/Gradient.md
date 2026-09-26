---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Gradient

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Gradient biến một trường vô hướng thành một trường vector — hướng mà đại lượng đó tăng nhanh nhất và tốc độ tăng. Nó là cầu nối thế năng → lực ($\vec F = -\nabla U$), điện thế → điện trường ($\vec E = -\nabla V$), và là "độ dốc" đằng sau mọi dòng chảy do chênh lệch.

## Định nghĩa

Với trường vô hướng $f(\vec r)$, gradient là vector có thành phần là đạo hàm riêng:

$\nabla f = \dfrac{\partial f}{\partial x}\hat i + \dfrac{\partial f}{\partial y}\hat j + \dfrac{\partial f}{\partial z}\hat k$ ([[Hệ tọa độ Descartes]])

Trong [[Hệ tọa độ cầu]]: $\nabla f = \dfrac{\partial f}{\partial r}\hat e_r + \dfrac{1}{r}\dfrac{\partial f}{\partial\theta}\hat e_\theta + \dfrac{1}{r\sin\theta}\dfrac{\partial f}{\partial\varphi}\hat e_\varphi$

Trong [[Hệ tọa độ trụ]]: $\nabla f = \dfrac{\partial f}{\partial\rho}\hat e_\rho + \dfrac{1}{\rho}\dfrac{\partial f}{\partial\varphi}\hat e_\varphi + \dfrac{\partial f}{\partial z}\hat k$

Vi phân toàn phần: $df = \nabla f \cdot d\vec l$ — gradient là "đạo hàm có hướng tổng hợp": $\nabla f \cdot \hat u$ = tốc độ thay đổi khi đi theo hướng $\hat u$.

## Ý nghĩa vật lý

- **Mũi tên "lên dốc nhanh nhất":** độ lớn $|\nabla f|$ là tốc độ tăng cực đại, hướng vuông góc các mặt đẳng trị $f = \text{const}$ — dùng để vẽ đường sức (điện thế, nhiệt độ, độ cao).
- **Sinh lực và điện trường:** $\vec F = -\nabla U$ ([[Thế năng]]) — lực hướng "xuống dốc" thế năng; $\vec E = -\nabla V$ ([[Điện thế và hiệu điện thế]]) — dấu trừ là quy ước quyết định chiều dòng.
- **Định lý cơ bản cho thế:** nếu $\vec F = \nabla\phi$ thì $\oint\vec F\cdot d\vec l = 0$ (công không phụ thuộc đường) — tương đương với $\nabla\times\vec F = 0$ ([[Curl]]); đây là tiêu chuẩn nhận diện trường thế.
- **Lượng tử:** định lý Ehrenfest cho $\dfrac{d\langle\hat{\vec p}\rangle}{dt} = -\langle\nabla V\rangle$ — chuyển động của trung bình xung lượng theo gradient thế ([[Định lý Ehrenfest]]).
- **Dòng chảy do chênh lệch:** dòng nhiệt $\vec j = -k\nabla T$, dòng hạt $\vec j = -D\nabla n$ — "vạn vật chảy xuống dốc của gradient".

## Kiến thức vật lý đang sử dụng công cụ này

- [[Thế năng]]: $\vec F = -\nabla U$ — lực bảo toàn là âm gradient thế năng.
- [[Điện thế và hiệu điện thế]]: $\vec E = -\nabla V$; mặt đẳng thế vuông góc đường sức.
- [[Định lý Ehrenfest]]: gradient thế điều khiển sự thay đổi trung bình xung lượng.
- [[Điện trường]]: từ $V(r)$ suy ra $\vec E$ qua gradient cầu hoặc trụ theo đối xứng.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Giải tích Vector (Grad, Div, Curl)]]
- [[Divergence]]
- [[Curl]]
- [[Đạo hàm]]
- [[Vector]]

## Câu hỏi mở

- Gradient là biểu diễn "đạo hàm ngoài" của dạng vi phân bậc 0 — vì sao nó giúp mọi trường thế đều đẹp trong không gian cong? ([[Giải tích Tensor]], [[Hình học vi phân]].)
- Dấu trừ trong $\vec F = -\nabla U$ thực chất là quy ước — nếu đổi dấu, điều gì trong [[Dao động điều hòa]] thay đổi?