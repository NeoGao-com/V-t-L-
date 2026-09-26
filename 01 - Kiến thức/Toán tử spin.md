---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Toán tử spin

> [!abstract] Ý chính
> Spin tuân cùng đại số giao hoán như mômen quỹ đạo, nhưng số lượng tử $s$ có thể bán nguyên: với $s = \tfrac{1}{2}$, toán tử spin là $\hat{\vec S} = \tfrac{\hbar}{2}\vec\sigma$ với **ma trận Pauli** $\sigma_x, \sigma_y, \sigma_z$ — trạng thái là spinor hai thành phần $\chi = \begin{pmatrix}\alpha\\\beta\end{pmatrix}$ (hàm spin), quay theo nửa góc dưới $SU(2)$.

## Phát biểu / Định nghĩa

**4.1. Toán tử spin và hàm spin của hạt vi mô:**

Toán tử $\hat{\vec S} = (\hat S_x, \hat S_y, \hat S_z)$ thỏa **cùng đại số** với [[Toán tử mô-men xung lượng|mômen quỹ đạo]]:

$[\hat S_i, \hat S_j] = i\hbar\,\varepsilon_{ijk}\,\hat S_k, \qquad \hat{\vec S}^2|s,m_s\rangle = s(s+1)\hbar^2|s,m_s\rangle, \qquad \hat S_z|s,m_s\rangle = m_s\hbar|s,m_s\rangle$

- Khác $\hat{\vec L}$: $s$ nhận cả bán nguyên ($\tfrac{1}{2}, \tfrac{3}{2}, \dots$) — đại số cho phép; $\hat S_i$ tác dụng lên **không gian spin** (chiều $2s+1$), không phải không gian tọa độ.
- Trạng thái đầy đủ của hạt: tích hàm sóng tọa độ × **hàm spin**: $\Psi(\vec r, t)\,\chi$ hay spinor $\Psi(\vec r,t) = \begin{pmatrix}\psi_\uparrow(\vec r,t)\\ \psi_\downarrow(\vec r,t)\end{pmatrix}$ (liên hệ [[Biểu diễn các trạng thái lượng tử]], [[Hàm sóng]]).

**4.2. Spin $\tfrac12$ và ma trận Pauli:**

Với cơ sở $|+\rangle = |\tfrac12,\tfrac12\rangle$, $|-\rangle = |\tfrac12,-\tfrac12\rangle$:

$\hat S_z = \dfrac{\hbar}{2}\sigma_z, \qquad \sigma_x = \begin{pmatrix}0&1\\1&0\end{pmatrix},\ \ \sigma_y = \begin{pmatrix}0&-i\\i&0\end{pmatrix},\ \ \sigma_z = \begin{pmatrix}1&0\\0&-1\end{pmatrix}$

**Tính chất** ([[Biểu diễn ma trận của toán tử]]):

- $\sigma_x^2 = \sigma_y^2 = \sigma_z^2 = I$; $\mathrm{Tr}\,\sigma_i = 0$; $\det\sigma_i = -1$.
- Phản giao hoán $\{\sigma_i,\sigma_j\} = 2\delta_{ij}I$; giao hoán $[\sigma_i,\sigma_j] = 2i\varepsilon_{ijk}\sigma_k$.
- Đồng nhất thức: $(\vec\sigma\cdot\vec a)(\vec\sigma\cdot\vec b) = \vec a\cdot\vec b\,I + i\vec\sigma\cdot(\vec a\times\vec b)$.
- Vector riêng: $\sigma_z|+\rangle = |+\rangle$, $\sigma_z|-\rangle = -|-\rangle$; $\sigma_x|+\rangle_x = |+\rangle_x$ với $|+\rangle_x = \tfrac{1}{\sqrt2}\bigl(|+\rangle + |-\rangle\bigr)$ — mọi spinor $\chi = \alpha|+\rangle + \beta|-\rangle$, $|\alpha|^2 + |\beta|^2 = 1$.
- **Phép quay spinor:** $\hat U(\vec n,\varphi) = e^{-i\varphi\,\vec\sigma\cdot\vec n/2}$ — **quay góc $\varphi$ ⟹ hàm spin quay $\varphi/2$**; quay $2\pi$ đưa $\chi \to -\chi$ (dấu trừ toàn cục — vô hại vật lý): spinor là biểu diễn $SU(2)$, che phủ bội 2 của $SO(3)$ ([[Sự chuyển biểu diễn và phép biến đổi unita]]).

**4.3. Hàm spin:**

- Hai electron đôi spin: trạng thái đối xứng/phản đối xứng — bộ ba triplet ($S = 1$) và đơn singlet ($S = 0$):

  $|1,1\rangle = |++\rangle,\ \ |1,0\rangle = \tfrac{1}{\sqrt2}\bigl(|\uparrow\downarrow\rangle + |\downarrow\uparrow\rangle\bigr),\ \ |1,-1\rangle = |--\rangle;\ \ \ |0,0\rangle = \tfrac{1}{\sqrt2}\bigl(|\uparrow\downarrow\rangle - |\downarrow\uparrow\rangle\bigr)$

- **Phương trình Pauli** (hạt trong từ trường có spin): $i\hbar\partial_t\Psi = \left[\dfrac{(\hat{\vec p} - e\vec A)^2}{2m_e} + \mu_B\,\vec\sigma\cdot\vec B\right]\Psi$ — tiền thân phi tương đối tính của phương trình Dirac ([[Lý thuyết trường lượng tử (QFT)]]).

## Suy luận từ đâu

- Tiên đề gốc: toán tử quan sát Hermit và không gian trạng thái ([[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]); spin kế thừa đại số $so(3)$ từ [[Toán tử mô-men xung lượng]].
- Công cụ: [[Biểu diễn ma trận của toán tử]], [[Đại số tuyến tính]], [[Ký hiệu Dirac]].

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: Stern–Gerlach (hai eigenvalue $\pm\hbar/2$ — [[Thí nghiệm - Stern-Gerlach]]); ma trận Pauli dự đoán đúng xác suất lọc spin qua chuỗi S-G nghiêng góc; $g_s = 2$ từ phương trình Pauli–Dirac khớp đo ([[Spin của hạt vi mô]]); triplet/singlet phân biệt qua cấu trúc siêu tinh tế của helium và [[Hiệu ứng Zeeman]].
- Trường hợp không còn đúng: với $s > \tfrac12$ (hạt nhân, $J$) cần ma trận $(2s+1)\times(2s+1)$ lớn hơn — Pauli chỉ đúng cho spin $\tfrac12$; ghép nhiều spin cần cộng mômen (hệ số Clebsch–Gordan); trong QFT tương đối tính, spin gắn liền phản hạt và ma trận Dirac bậc 4.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Spin của hạt vi mô]]
- [[Toán tử mô-men xung lượng]]
- [[Biểu diễn ma trận của toán tử]]
- [[Hệ hạt đồng nhất]]
- [[Thí nghiệm - Stern-Gerlach]]

## Câu hỏi mở

- Spinor quay $2\pi$ đổi dấu — vậy nếu "lượng tử hóa" phép quay bằng chuỗi S-G, ta có phân biệt được trạng thái $|\chi\rangle$ và $-|\chi\rangle$ không? (Gợi ý: giao thoa neutron — kiểm chứng dấu spinor ở thực tế.)
- $\vec\sigma\cdot\vec B$ trong phương trình Pauli là "chiếu spin lên từ trường" — tổng quát cho từ trường phụ thuộc thời gian và không gian (GP lệch pha, qubit) phát triển ra sao?