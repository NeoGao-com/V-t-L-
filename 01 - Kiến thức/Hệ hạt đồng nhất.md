---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Hệ hạt đồng nhất

> [!abstract] Ý chính
> Các hạt cùng loại là **không phân biệt** — trạng thái chỉ được đối xứng hóa: fermion phản đối xứng (định thức Slater ⟹ nguyên lý loại trừ Pauli), boson đối xứng (mọi hạt dồn cùng mức) — từ đó sinh ra cấu trúc vật chất, liên kết hóa học, laser và áp suất thoái hóa của sao lùn trắng.

## Phát biểu / Định nghĩa

**5.1. Nguyên lý không phân biệt các hạt đồng nhất:**

Hai electron (hay hai photon...) là **bản sao giống hệt nhau** — không có nhãn riêng; đổi chỗ chúng không tạo trạng thái mới. Toán tử hoán vị $\hat P_{12}$ (đổi chỗ hạt 1, 2) giao hoán với Hamiltonian ($[\hat H, \hat P_{12}] = 0$) nên trạng thái là hàm riêng:

$\hat P_{12}\,\Psi(1,2) = \lambda\,\Psi(2,1), \qquad \lambda = \pm 1$ (vì $\hat P_{12}^2 = 1$)

**5.2. Trạng thái đối xứng và phản đối xứng:**

Định lý spin–thống kê ([[Lý thuyết trường lượng tử (QFT)]]) quy định dấu theo spin:

- **Boson** (spin nguyên $0, 1, 2,\dots$: photon, pion, phonon, $^{4}$He): $\lambda = +1$ — hàm sóng **đối xứng**.
- **Fermion** (spin bán nguyên $\tfrac12, \tfrac32,\dots$: electron, proton, neutron, quark): $\lambda = -1$ — hàm sóng **phản đối xứng**.

**5.3. Hàm sóng hệ hạt đồng nhất không tương tác:**

Hai hạt ở trạng thái đơn hạt $\psi_a, \psi_b$:

- **Fermion:** $\Psi(1,2) = \dfrac{1}{\sqrt2}\bigl[\psi_a(1)\psi_b(2) - \psi_a(2)\psi_b(1)\bigr]$ — **định thức Slater** $N$-hạt $\Psi = \dfrac{1}{\sqrt{N!}}\det[\psi_{a_i}(j)]$; nếu $a = b$: $\Psi \equiv 0$ — **nguyên lý loại trừ Pauli** ([[Nguyên lý loại trừ Pauli]]).
- **Boson:** $\Psi(1,2) = \dfrac{1}{\sqrt2}\bigl[\psi_a(1)\psi_b(2) + \psi_a(2)\psi_b(1)\bigr]$ — nhiều hạt dồn cùng $\psi_a$ được (nền của laser, ngưng tụ Bose–Einstein).
- **Tương tác trao đổi:** việc đối xứng hóa làm mật độ xác suất $|\Psi|^2$ có số hạng chéo $\pm\psi_a^*(1)\psi_b^*(2)\psi_a(2)\psi_b(1)$ — tạo năng lượng trao đổi (không phải lực mới, mà hệ quả thống kê) quyết định feromagnetism, liên kết cộng hóa trị ($H_2$), quy tắc Hund.

**5.4. Hệ quả — Nguyên lý loại trừ Pauli:**

- Mỗi trạng thái lượng tử tối đa **một fermion**: electron trong nguyên tử phân bố theo $(n,l,m_l,m_s)$ — tối đa 2 electron/orbital ([[Sự phân bố electron trong nguyên tử Hydro]], [[Nguyên lý loại trừ Pauli]]).
- **Ví dụ helium:** trạng thái cơ bản — $\Psi_{không gian}$ đối xứng (cùng $1s$) buộc $\Psi_{spin}$ phản đối xứng ⟹ **singlet** $S = 0$ (khí trơ, không từ tính); trạng thái kích thích có triplet $S = 1$ *thấp hơn* singlet cùng cấu hình (năng lượng trao đổi dương) — quan sát được trong cấu trúc helium ([[Toán tử spin]]).
- **Khí Fermi thoái hóa:** electron tự do chiếm các mức tới năng lượng Fermi $E_F$ — nguồn của "áp suất thoái hóa" giữ sao lùn trắng, sao neutron không sụp ([[Nguyên lý loại trừ Pauli]]).

## Suy luận từ đâu

- Tiên đề gốc: không gian trạng thái nhiều hạt = tích tensor ([[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]), toán tử hoán vị $\hat P$ ([[Trạng thái lượng tử]]); định lý spin–thống kê từ lý thuyết trường ([[Lý thuyết trường lượng tử (QFT)]]).
- Công cụ: [[Toán tử spin]] (triplet/singlet), [[Đại số tuyến tính]] (định thức Slater), [[Biểu diễn các trạng thái lượng tử]].

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: cấu hình electron qua [[Quang phổ]] và bảng tuần hoàn; helium lỏng: $^{4}$He (boson) siêu chảy ở $2{,}17$ K còn $^{3}$He (fermion) cần ghép cặp ở $10^{-3}$ K — trực tiếp minh họa khác biệt thống kê; giao thoa neutron (đổi nhãn) khớp đối xứng hóa; số hạt photon trong laser dồn mức khớp boson.
- Trường hợp không còn đúng: hạt "phân biệt được" khi khối lượng/điện tích khác nhau (hay xa nhau — nhãn chỉ là quy ước); gần đúng hạt độc lập vỡ khi tương tác mạnh — ví dụ hiệu ứng Kondo, chất lỏng Fermi vs BEC–BCS; ở năng lượng cực cao cần trường thứ cấp (spin–thống kê gắn với phản hạt, QED/QCD).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Nguyên lý loại trừ Pauli]]
- [[Toán tử spin]]
- [[Sự phân bố electron trong nguyên tử Hydro]]
- [[Lý thuyết trường lượng tử (QFT)]]
- [[Spin của hạt vi mô]]

## Câu hỏi mở

- "Nhãn hạt" biến mất nhưng máy tính chọn $N!$ cách sắp xếp — vậy đếm trạng thái trong nhiệt động lực học lượng tử (thừa số Gibbs $1/N!$) liên hệ gì với đối xứng hóa?
- Hệ fermion ở mật độ siêu cao (sao neutron) — áp suất thoái hóa có thể bị "đánh bại" bằng siêu dẫn/BCS ở quy mô sao? (Liên hệ giới hạn Tolman–Oppenheimer–Volkoff.)