---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Giải tích Vector (Grad, Div, Curl)

> [!abstract] Công cụ để làm gì
> Ba phép toán vi phân trên trường vector — gradient, divergence, curl — là "ngôn ngữ địa phương" của mọi trường vật lý: điện trường, từ trường, dòng chảy. Cả [[Phương trình Maxwell]] gói gọn trong bốn dòng viết bằng chúng.

## Định nghĩa

Với trường vô hướng $f$ và trường vector $\vec A$:

- **Gradient:** $\nabla f = \dfrac{\partial f}{\partial x}\hat i + \dfrac{\partial f}{\partial y}\hat j + \dfrac{\partial f}{\partial z}\hat k$ — vector hướng theo chiều $f$ tăng nhanh nhất, độ lớn = tốc độ tăng.
- **Divergence:** $\nabla \cdot \vec A = \dfrac{\partial A_x}{\partial x} + \dfrac{\partial A_y}{\partial y} + \dfrac{\partial A_z}{\partial z}$ — đo "độ chảy ra" của trường tại một điểm (nguồn > 0, chìm < 0).
- **Curl:** $\nabla \times \vec A = \begin{vmatrix} \hat i & \hat j & \hat k \\ \partial_x & \partial_y & \partial_z \\ A_x & A_y & A_z \end{vmatrix}$ — đo "độ xoáy" của trường quanh điểm đó.
- **Laplacian** (hợp thành của div và grad): $\nabla^2 f = \nabla \cdot (\nabla f)$ — "độ cong trung bình" của $f$, xuất hiện trong phương trình truyền sóng và nhiệt.

## Ý nghĩa hình học

- **Grad** = hướng lên dốc nhanh nhất trên "bản đồ" $f$ (như gradient nhiệt độ, gradient độ cao).
- **Div** = lượng "chất lỏng" chảy ra từ một thể tích tí xíu quanh điểm, chia cho thể tích đó.
- **Curl** = "vòng quay" của trường quanh điểm, đo bằng lưu số trên một vòng tí xíu chia cho diện tích (kim của chong chóng quay nhanh nhất khi đặt theo hướng của curl).

## Ý nghĩa vật lý

- **Gradient sinh lực:** lực bảo toàn bằng âm gradient của thế năng, $\vec F = -\nabla U$ — [[Thế năng]]; điện trường là âm gradient điện thế, $\vec E = -\nabla V$ — [[Điện thế và hiệu điện thế]], [[Điện trường]].
- **Divergence gắn với nguồn:** $\nabla \cdot \vec E = \rho / \varepsilon_0$ — điện tích là nguồn của điện trường ([[Định luật Gauss (điện)]]); $\nabla \cdot \vec B = 0$ — không có "từ tích đơn cực".
- **Curl gắn với xoáy:** $\nabla \times \vec B = \mu_0 \vec j$ — dòng điện tạo từ trường xoáy ([[Từ trường và cảm ứng từ]], [[Từ trường của các dòng điện]]); $\nabla \times \vec E = -\partial \vec B / \partial t$ — từ trường biến thiên tạo điện trường xoáy ([[Từ thông và hiện tượng cảm ứng điện từ]]).
- **Sóng điện từ:** trường có **cả** div và curl bằng 0 trong chân không lan truyền thành sóng — [[Điện từ trường]], [[Sóng điện từ và thang sóng điện từ]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Phương trình Maxwell]]: cả bốn phương trình là câu trả lời cho "div và curl của $\vec E$, $\vec B$ bằng gì?".
- [[Điện thế và hiệu điện thế]] · [[Thế năng]]: dùng gradient để đi từ trường về thế (và ngược lại).
- [[Điện từ trường]] · [[Sóng điện từ và thang sóng điện từ]]: trường biến thiên lan truyền — bản chất sóng của điện từ.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Vector]] · [[Đạo hàm]] · [[Tích phân]] · [[Định lý Gauss & Stokes]] · [[Phương trình Maxwell]] · [[Hàm Green]]
- Ba toán tử chi tiết (kể cả trong [[Hệ tọa độ cầu]] và [[Hệ tọa độ trụ]]): [[Gradient]] · [[Divergence]] · [[Curl]] · [[Toán tử Laplace]]

## Câu hỏi mở

- Trường không có divergence và không có curl thì có dạng gì? (Gợi ý: sóng điện từ trong chân không — [[Điện từ trường]].)
- Phân tích Helmholtz nói trường vector tổng quát = phần "nguồn" (div) + phần "xoáy" (curl). Điều này nói gì về số lượng dữ kiện cần để xác định một trường vật lý?