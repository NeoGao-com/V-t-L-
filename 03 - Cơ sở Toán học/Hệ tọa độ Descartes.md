---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Hệ tọa độ Descartes

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Hệ tọa độ vuông góc $(x, y, z)$ có ba vector đơn vị **cố định** và "mảnh đất" không cong — nó là hệ duy nhất tách bài toán đa chiều thành các bài toán một chiều độc lập (hộp lượng tử, ném xiên), và là "hệ mặc định" mà mọi hệ cong đều quy về.

## Định nghĩa

- Tọa độ: $(x, y, z) \in \mathbb{R}^3$; vector đơn vị $\hat i, \hat j, \hat k$ **không đổi** ở mọi điểm.
- Phần tử độ dài: $d\vec l = dx\,\hat i + dy\,\hat j + dz\,\hat k$; khoảng cách $ds^2 = dx^2 + dy^2 + dz^2$ (metric chéo cổ điển).
- Phần tử thể tích: $dV = dx\,dy\,dz$ (tích Descartes, không có nhân tử như hệ cong).
- [[Toán tử Laplace]]: $\nabla^2 f = \dfrac{\partial^2 f}{\partial x^2} + \dfrac{\partial^2 f}{\partial y^2} + \dfrac{\partial^2 f}{\partial z^2}$.

## Ý nghĩa vật lý

- **Đối xứng tịnh tiến:** các vector đơn vị không đổi ⟹ lấy đạo hàm của vector không cần đạo hàm của vector đơn vị — thích hợp bài toán có đối xứng tịnh tiến (hộp, mạng tinh thể, sóng phẳng).
- **Tách độc lập:** chuyển động theo $x$ không can thiệp vào $y$ khi lực phân tích theo trục — "siêu năng lực" của phép phân tích lực ([[Chuyển động ném]], mặt phẳng nghiêng, [[Dao động tử điều hòa ba chiều|dao động tử ba chiều đẳng hướng]]).
- **Lượng tử:** hàm riêng của $\hat p$ trong Descartes là sóng phẳng $e^{i\vec p\cdot\vec r/\hbar}$; hộp 3D tách thành $\sin(k_x x)\sin(k_y y)\sin(k_z z)$ với $E = E_x + E_y + E_z$ ([[Giếng thế ba chiều]], [[Tách biến trong phương trình Schrödinger ba chiều]]).
- **Khi không nên dùng:** bài toán có đối xứng cầu/tâm (nguyên tử, hành tinh, sóng từ nguồn điểm) — các hàm sóng trở nên rối khi viết bằng $(x,y,z)$; phải dùng [[Hệ tọa độ cầu]]/[[Hệ tọa độ trụ]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Chuyển động cơ và hệ quy chiếu]]: hệ quy chiếu Descartes là khung đo vị trí mặc định.
- [[Giếng thế ba chiều]]: hộp vuông — tách biến ba chiều, phổ $E \propto n_x^2 + n_y^2 + n_z^2$.
- [[Bó sóng lượng tử]]: tổ hợp sóng phẳng $e^{ikx}$ tích phân Fourier — "cộng sóng phẳng nên vị trí".
- [[Vector]]: cộng/trừ vector bằng thành phần $(x,y,z)$ ([[Đại số tuyến tính]]).

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Hệ tọa độ]]
- [[Hệ tọa độ cầu]]
- [[Hệ tọa độ trụ]]
- [[Toán tử Laplace]]
- [[Đạo hàm]]

## Câu hỏi mở

- Vì sao "tách được ba hướng" là tài sản hiếm — bài toán nào trong vật lý có đối xứng chỉ đủ yếu để tách trong Descartes nhưng không trong hệ cong? (Ví dụ: dao động tử đẳng hướng tách được cả Descartes lẫn cầu nhưng bậc suy biến khác nhau.)
- "Tọa độ" của một điểm là quy ước, nhưng "khoảng cách" thì không — hệ Descartes phẳng có gì đặc biệt hơn hệ cong về phương diện song song (song song phải cứng — affine)?