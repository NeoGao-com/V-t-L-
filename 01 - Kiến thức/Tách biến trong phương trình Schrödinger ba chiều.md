---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Tách biến trong phương trình Schrödinger ba chiều

> [!abstract] Ý chính
> Khi thế năng tách được $V(\vec r) = V_x(x) + V_y(y) + V_z(z)$, phương trình Schrödinger ba chiều tách thành ba phương trình một chiều độc lập với hàm sóng là tích $\psi(x,y,z) = X(x)Y(y)Z(z)$ và năng lượng là tổng $E = E_x + E_y + E_z$ — đây là phương pháp giải mọi bài toán hộp thế và dao động tử trong không gian 3 chiều.

## Phát biểu / Định nghĩa

Phương trình Schrödinger dừng 3 chiều:

$-\dfrac{\hbar^2}{2m}\left(\dfrac{\partial^2\psi}{\partial x^2} + \dfrac{\partial^2\psi}{\partial y^2} + \dfrac{\partial^2\psi}{\partial z^2}\right) + V(x,y,z)\psi = E\psi$

Nếu $V(x,y,z) = V_x(x) + V_y(y) + V_z(z)$, thử nghiệm dạng tích:

$\psi(x,y,z) = X(x)\,Y(y)\,Z(z)$

thì phương trình tách thành **ba phương trình một chiều**:

$-\dfrac{\hbar^2}{2m}X'' + V_x X = E_x X, \qquad\text{(và tương tự cho } y, z\text{)}$

với điều kiện $E = E_x + E_y + E_z$. Mỗi phương trình một chiều là bài toán đã biết trong [[Chuyển động một chiều trong cơ học lượng tử]].

**Cách xây dựng bộ nghiệm đầy đủ:**

1. Giải từng bài toán 1D, thu bộ số lượng tử $n_x, n_y, n_z$ và năng lượng $E_{n_x}, E_{n_y}, E_{n_z}$.
2. Hàm sóng toàn phần: $\psi_{n_xn_yn_z} = X_{n_x}(x)\,Y_{n_y}(y)\,Z_{n_z}(z)$; năng lượng: $E = E_{n_x} + E_{n_y} + E_{n_z}$.
3. Chuẩn hóa từng thành phần thì tích tự động chuẩn hóa.

**Suy biến:** nhiều bộ $(n_x, n_y, n_z)$ khác nhau có thể cho cùng $E$ (ví dụ hộp lập phương có $(1,2,1)$, $(2,1,1)$ cùng năng lượng — xem [[Giếng thế ba chiều]]). Suy biến này là dấu hiệu của đối xứng (hộp đều, thế đẳng hướng).

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng ([[Phương trình Schrödinger]]) trong 3 chiều, tính chất của [[Nghiệm dừng của phương trình Schrödinger]].
- Công cụ toán: phương pháp tách biến — chia phương trình đạo hàm riêng cho $\psi$ rồi tách từng biến; các phương trình vi phân thường một chiều.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: mật độ trạng thái của khí electron 2D/GaAs 2DEG và chấm lượng tử 0D khớp dự đoán từ hộp tách biến; phổ hấp thụ của chấm lượng tử được gán đúng các số lượng tử $(n_x,n_y,n_z)$.
- Trường hợp không còn đúng: thế không tách được (ví dụ thế Coulomb $V \propto -\dfrac{1}{r}$, thế có số hạng chéo $xy$) không tách được trong tọa độ Descartes — cần tọa độ cầu hoặc giải số.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Giếng thế hai chiều]]
- [[Giếng thế ba chiều]]
- [[Dao động tử điều hòa ba chiều]]
- [[Phương trình Schrödinger]]
- [[Phương trình đạo hàm riêng (PDE)]]

## Câu hỏi mở

- Thế tách được trong tọa độ Descartes nhưng không tách được trong tọa độ cầu thì giải bằng cách nào?
- Khi hộp mất đối xứng ($L_x \ne L_y \ne L_z$), suy biến biến mất hay chỉ giảm bớt — và còn sót lại suy biến "ngẫu nhiên" nào?