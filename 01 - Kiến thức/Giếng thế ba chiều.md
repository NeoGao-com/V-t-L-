---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Giếng thế ba chiều

> [!abstract] Ý chính
> Hạt giam trong hộp lập phương vô hạn có năng lượng $E = \dfrac{\pi^2\hbar^2}{2mL^2}(n_x^2 + n_y^2 + n_z^2)$ với suy biến bằng số hoán vị của bộ $(n_x,n_y,n_z)$ — nền tảng cho các mô hình hộp lượng tử, chấm lượng tử 0D và mô hình Fermi của hạt nhân.

## Phát biểu / Định nghĩa

Thế năng: $V = 0$ trong hình hộp $0 < x,y,z < L$; $V = \infty$ bên ngoài. Nhờ [[Tách biến trong phương trình Schrödinger ba chiều]]:

$\psi_{n_xn_yn_z}(x,y,z) = \left(\dfrac{2}{L}\right)^{3/2}\sin\dfrac{n_x\pi x}{L}\,\sin\dfrac{n_y\pi y}{L}\,\sin\dfrac{n_z\pi z}{L}, \qquad n_x,n_y,n_z = 1,2,3,\dots$

$E_{n_xn_yn_z} = \dfrac{\pi^2\hbar^2}{2mL^2}\left(n_x^2 + n_y^2 + n_z^2\right)$

**Suy biến của hộp lập phương** (mọi chiều bằng nhau): năng lượng chỉ phụ thuộc $N = n_x^2 + n_y^2 + n_z^2$; số trạng thái suy biến bằng số cách sắp xếp các số nguyên khác nhau trong bộ $(n_x,n_y,n_z)$:

- $N = 3$: bộ $(1,1,1)$ — không suy biến (trạng thái cơ bản).
- $N = 6$: bộ $(1,1,2)$ với 3 hoán vị — suy biến bậc 3.
- $N = 9$: bộ $(2,2,1)$ với 3 hoán vị — suy biến bậc 3.
- $N = 14$: bộ $(1,2,3)$ với 6 hoán vị — suy biến bậc 6.

**Mật độ trạng thái:** với $N$ lớn, số trạng thái có $N \le N_0$ xấp xỉ $\dfrac{1}{8}\cdot\dfrac{4\pi}{3}k_{N_0}^3/\dfrac{\pi^3}{L^3}$ — tức thể tích của 1/8 khối cầu trong không gian $(n_x,n_y,n_z)$, đây là cơ sở tính số trạng thái của khí Fermi.

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng với điều kiện biên triệt tiêu trên 6 mặt hộp.
- Công cụ toán: tách biến ([[Tách biến trong phương trình Schrödinger ba chiều]]), tổ hợp và hoán vị để đếm suy biến; xấp xỉ khối cầu trong không gian số lượng tử.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: chấm lượng tử 0D — phổ phát quang rời rạc gán theo $(n_x,n_y,n_z)$; mô hình hộp giải thích định tính cấu trúc mức của các cụm kim loại nhỏ; mô hình Fermi (proton/neutron trong hộp) cho năng lượng Fermi của hạt nhân cỡ 20–40 MeV.
- Trường hợp không còn đúng: hộp là mô hình đơn giản hóa — thế hạt nhân thực là giếng hữu hạn bán kính hữu hạn, electron thực chịu thế Coulomb; suy biến đối xứng lập phương bị phá vỡ trong hộp chữ nhật ($L_x \ne L_y \ne L_z$).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Giếng thế hai chiều]]
- [[Tách biến trong phương trình Schrödinger ba chiều]]
- [[Giếng thế vô hạn]]
- [[Dao động tử điều hòa ba chiều]]

## Câu hỏi mở

- Vì sao suy biến tăng khi $N$ lớn — liên hệ gì với đối xứng lập phương và nhóm các phép quay của khối lập phương?
- Khi hộp lập phương bị biến dạng nhẹ, các mức suy biến tách thế nào? (Khởi đầu của lí thuyết nhiễu loạn suy biến.)