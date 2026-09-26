---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Dao động tử điều hòa ba chiều

> [!abstract] Ý chính
> Dao động tử điều hòa đẳng hướng ba chiều có năng lượng $E = \hbar\omega\left(N + \dfrac{3}{2}\right)$ với $N = n_x + n_y + n_z$, suy biến bậc $\dfrac{(N+1)(N+2)}{2}$ — phổ cách đều, suy biến cao hơn mức cần thiết cho đối xứng quay, và là mô hình cơ bản của mô hình vỏ hạt nhân và phonon ba chiều.

## Phát biểu / Định nghĩa

Thế năng đẳng hướng: $V(\vec r) = \dfrac{1}{2}m\omega^2 r^2 = \dfrac{1}{2}m\omega^2(x^2 + y^2 + z^2)$

Nhờ [[Tách biến trong phương trình Schrödinger ba chiều]] và bài toán một chiều trong [[Dao động tử điều hòa lượng tử]]:

$E = \hbar\omega\left(n_x + n_y + n_z + \dfrac{3}{2}\right) = \hbar\omega\left(N + \dfrac{3}{2}\right)$

$\psi_{n_xn_yn_z}(x,y,z) = \psi_{n_x}(x)\,\psi_{n_y}(y)\,\psi_{n_z}(z)$ (tích ba hàm Hermite–Gauss)

**Suy biến:** năng lượng chỉ phụ thuộc $N = n_x + n_y + n_z$; số bộ $(n_x,n_y,n_z)$ không âm có tổng $N$ là:

$g(N) = \dfrac{(N+1)(N+2)}{2}$

Ví dụ: $N = 0$: $g=1$ (mức thấp nhất); $N = 1$: $g=3$; $N = 2$: $g=6$.

**Đối xứng quay:** với thế cầu $V(r)$, có thể dùng tọa độ cầu, nghiệm dạng $R_{nl}(r)Y_{lm}(\theta,\phi)$; năng lượng vẫn chỉ phụ thuộc $N$ — suy biến $\dfrac{(N+1)(N+2)}{2}$ **lớn hơn** suy biến quay $2l+1$ của mỗi $l$: cùng một $N$ chứa nhiều $l$ khác nhau (suy biến "ngẫu nhiên" do đối xứng $SU(3)$ ẩn).

**Năng lượng điểm không:** số hạng $\dfrac{3}{2}\hbar\omega$ — tổng của ba dao động phương.

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng với thế cầu bậc hai; quan hệ giao hoán ba chiều $[\hat x_i,\hat p_j] = i\hbar\delta_{ij}$.
- Công cụ toán: tách biến Descartes; toán tử sinh–hủy ba chiều $\hat a_i = \sqrt{\dfrac{m\omega}{2\hbar}}\left(\hat x_i + \dfrac{i\hat p_i}{m\omega}\right)$; tổ hợp chỉnh hợp lặp để đếm $g(N)$.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: mô hình vỏ (shell model) của hạt nhân — các số ma thuật vỏ đóng; phonon quang trong tinh thể; phổ của chấm lượng tử gần cầu.
- Trường hợp không còn đúng: thế hạt nhân thực lệch khỏi dao động tử thuần túy ($V \propto r^2$ không đúng ở xa và gần), cần thêm số hạng spin–quỹ đạo để tách suy biến; thế dị hướng ($\omega_x \ne \omega_y$) phá vỡ cấu trúc đều và suy biến.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Dao động tử điều hòa lượng tử]]
- [[Tách biến trong phương trình Schrödinger ba chiều]]
- [[Giếng thế ba chiều]]
- [[Nghiệm dừng của phương trình Schrödinger]]

## Câu hỏi mở

- Vì sao suy biến $\dfrac{(N+1)(N+2)}{2}$ "ẩn" nhiều hơn đối xứng quay — nhóm đối xứng nào sinh ra nó? ($SU(3)$, liên hệ với cấu trúc đại số của ba toán tử sinh–hủy.)
- So sánh suy biến của dao động tử 3D với [[Giếng thế ba chiều]] — mô hình nào gần thế hạt nhân thực hơn và vì sao?