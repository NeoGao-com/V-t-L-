---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Hệ tọa độ trụ

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Tọa độ trụ $(\rho, \varphi, z)$ là "Descartes trong mặt phẳng + góc quay": thích hợp mọi bài toán có một trục đối xứng — dây dẫn thẳng, solenoid dài, ống quang, dây lượng tử. Tách biến theo trụ làm xuất hiện hàm Bessel $J_m$ — "họ hàm sin/cos" của bài toán tròn.

## Định nghĩa

Quy ước: $\rho$ — bán kính từ trục $z$ ra ($\rho \ge 0$); $\varphi$ — góc phương vị từ trục $x$; $z$ — độ cao giống Descartes:

$x = \rho\cos\varphi, \qquad y = \rho\sin\varphi, \qquad z = z$

- Phần tử độ dài: $d\vec l = d\rho\,\hat e_\rho + \rho\,d\varphi\,\hat e_\varphi + dz\,\hat k$ — chỉ hai trong ba vector đơn vị đổi hướng theo vị trí.
- Phần tử thể tích: $dV = \rho\,d\rho\,d\varphi\,dz$ — nhân tử $\rho$ (cung dài $\rho\,d\varphi$).
- Gradient: $\nabla f = \dfrac{\partial f}{\partial\rho}\hat e_\rho + \dfrac{1}{\rho}\dfrac{\partial f}{\partial\varphi}\hat e_\varphi + \dfrac{\partial f}{\partial z}\hat k$.
- [[Toán tử Laplace]]: $\nabla^2 f = \dfrac{1}{\rho}\dfrac{\partial}{\partial\rho}\left(\rho\dfrac{\partial f}{\partial\rho}\right) + \dfrac{1}{\rho^2}\dfrac{\partial^2 f}{\partial\varphi^2} + \dfrac{\partial^2 f}{\partial z^2}$.

## Ý nghĩa vật lý

- **Đối xứng trục:** vấn đề giữ nguyên khi quay quanh $z$ — hàm sóng/trường không phụ thuộc $\varphi$ (hoặc phụ thuộc qua pha $e^{im\varphi}$ với $m$ nguyên, gắn với $\hat L_z$ khi thêm $z$ vào [[Toán tử mô-men xung lượng]]).
- **Hàm Bessel thay sin/cos:** phương trình $\rho$-chiều chứa $1/\rho$ không dẫn tới $\sin, \cos$ mà tới hàm Bessel $J_m(k\rho)$ — "họ dao động" của đĩa tròn, cáp đồng trục, sợi quang, trống tròn; nút của $J_m$ cho tần số riêng.
- **Trường cảm ứng:** dây dẫn thẳng dài ⟹ $\vec B$ có cấu trúc trụ quanh dây ([[Từ trường của các dòng điện]]); mặt Gauss kiểu trụ quanh dây/trụ là phép chọn khôn ngoan cho [[Định luật Gauss (điện)]].
- **Lượng tử:** giếng trụ/mặt phẳng đối xứng trục tách thành $R(\rho) e^{im\varphi} Z(z)$ — đường dẫn tự nhiên cho dây lượng tử và nguyên tử trong từ trường đều (nền của [[Hiệu ứng Zeeman]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Từ trường của các dòng điện]]: $\vec B = \dfrac{\mu_0 I}{2\pi\rho}\hat e_\varphi$ — đường tròn $\hat e_\varphi$ quanh dây.
- [[Định luật Gauss (điện)]]: bề mặt trụ — điện trường dây tích điện $E \propto 1/\rho$.
- [[Phương trình Schrödinger]]: tách biến khi thế có đối xứng trục.
- [[Toán tử Laplace]]: dạng trụ của toán tử cho mọi hệ trục đối xứng.
- [[Hệ tọa độ Descartes]]: trụ hạn chế về Descartes khi "mở" mặt phẳng (khai triển) — ánh xạ $\varphi \to x'$.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Hệ tọa độ]]
- [[Hệ tọa độ cầu]]
- [[Hệ tọa độ Descartes]]
- [[Toán tử Laplace]]
- [[Chuyển động tròn đều]]

## Câu hỏi mở

- Vì sao "sin/cos" của bài toán tròn lại là $J_m$ chứ không phải $\sin(m\varphi)$? (Gợi ý: quay lại dạng $\partial_\rho^2 + (1/\rho)\partial_\rho$ — phương trình Bessel.)
- Hàm Bessel có tính trực giao như sin/cos không — cơ sở nào cho khai triển hàm theo $\rho$ trong ống trụ? ([[Phương trình đạo hàm riêng (PDE)]].)