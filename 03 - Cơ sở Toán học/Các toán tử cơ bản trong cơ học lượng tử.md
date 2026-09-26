---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Các toán tử cơ bản trong cơ học lượng tử

> [!abstract] Công cụ để làm gì
> Các toán tử tọa độ, xung lượng, năng lượng và mô-men xung lượng là cách lượng tử hóa những đại lượng cơ bản của cơ học. Hệ thức giao hoán giữa chúng giải thích trực tiếp nhiều tính chất đặc trưng của trạng thái và phép đo lượng tử.

## Toán tử tọa độ

Trong cơ sở vị trí, tọa độ được biểu diễn bằng phép nhân:

$\hat x_j\psi(x)=x_j\psi(x)$;

$\hat{\mathbf r}\psi(\vec r)=\vec r\,\psi(\vec r)$.

Toán tử tọa độ là ví dụ đơn giản nhất về toán tử đo được. Trạng thái vị trí $|x\rangle$ là ket tổng quát hóa, thỏa:

$\hat x|x\rangle=x|x\rangle$;

$\langle x|x'\rangle=\delta(x-x')$.

Kỳ vọng của tọa độ trong hàm sóng là:

$\langle\hat{\mathbf r}\rangle=\int_{\mathbb R^3}\vec r\,|\psi(\vec r)|^2\,d^3r$.

## Toán tử xung lượng

Trong biểu diễn tọa độ:

$\hat p_x=-i\hbar\dfrac{\partial}{\partial x}$,

$\hat{\mathbf p}=-i\hbar\nabla$.

Sóng phẳng:

$\psi_p(x)=A e^{ipx/\hbar}$

là trạng thái riêng tổng quát hóa của $\hat p_x$ với trị riêng $p$, nhưng không chuẩn hóa được trên toàn trục. Các trạng thái có xác suất vị trí tập trung ở miền hữu hạn phải là tổ hợp của nhiều sóng phẳng.

Các điều kiện biên, như tuần hoàn hay bằng 0 tại các đầu vô hạn, quy định tập trạng thái hàm sóng hợp lệ.

## Toán tử năng lượng

Với một hạt phi tương đối tính trong trường thế $V(\vec r,t)$:

$\hat H=\frac{\hat{\mathbf p}^{\,2}}{2m}+V(\vec r,t)=-\dfrac{\hbar^2}{2m}\nabla^2+V(\vec r,t)$.

Phương trình Schrödinger trong ký hiệu trạng thái là:

$i\hbar\dfrac{\partial}{\partial t}|\psi\rangle=\hat H|\psi\rangle$.

Nếu $\hat H$ không phụ thuộc thời gian, trạng thái năng lượng tĩnh thỏa:

$\hat H|E\rangle=E|E\rangle$.

Các trị riêng $E$ là các mức năng lượng được phép. Khi $\hat H$ không phụ thuộc thời gian, phương trình $\hat H\psi=E\psi$ chỉ mô tả trạng thái năng lượng tĩnh, không phải mọi trạng thái tổng quát.

Với nhiều hạt, Hamiltonian chứa tổng các bình phương động lượng và thế tương tác; khi vận tốc tiến gần tốc độ ánh sáng cần thay bằng phương trình Dirac.

## Toán tử mô-men xung lượng

Mô-men xung lượng orbital được định nghĩa bằng tích vector vị trí với động lượng:

$\hat{\mathbf L}=\hat{\mathbf r}\times\hat{\mathbf p}=-i\hbar\vec r\times\nabla$.

Các thành phần trong hệ tọa độ là:

$\hat L_x=-i\hbar\left(y\dfrac{\partial}{\partial z}-z\dfrac{\partial}{\partial y}\right)$;

$\hat L_y=-i\hbar\left(z\dfrac{\partial}{\partial x}-x\dfrac{\partial}{\partial z}\right)$;

$\hat L_z=-i\hbar\left(x\dfrac{\partial}{\partial y}-y\dfrac{\partial}{\partial x}\right)$.

Chúng thỏa:

$[\hat L_i,\hat L_j]=i\hbar\varepsilon_{ijk}\hat L_k$;

$\hat L^2=\hat L_x^2+\hat L_y^2+\hat L_z^2$.

Trong hệ quanh gốc, các số lượng tử orbital là:

$l=0,1,2,\ldots$;

$m_l=-l,-l+1,\ldots,l$;

$\hat L^2$ có trị riêng $l(l+1)\hbar^2$ và $\hat L_z$ có trị riêng $m_l\hbar$.

Spin là mô-men xung lượng nội tại, dùng các toán tử $\hat S_i$ và được ghép với orbital trong toán tử tổng $\hat{\mathbf J}=\hat{\mathbf L}+\hat{\mathbf S}$.

## Hệ thức giao hoán giữa các toán tử

| Cặp toán tử | Hệ thức giao hoán | Hệ quả |
| --- | --- | --- |
| $[\hat x_i,\hat x_j]$ | $0$ | Các hướng tọa độ giao hoán |
| $[\hat p_i,\hat p_j]$ | $0$ | Các thành phần xung lượng giao hoán |
| $[\hat x_i,\hat p_j]$ | $i\hbar\delta_{ij}$ | Không thể chuẩn bị vị trí và xung lượng cùng xác định |
| $[\hat L_i,\hat L_j]$ | $i\hbar\varepsilon_{ijk}\hat L_k$ | Các phép quay tạo cấu trúc Lie |
| $[\hat H,\hat p_i]$ | $i\hbar\,\partial_i V$ — đúng với **mọi** thế tĩnh $V = V(\vec r)$ khi $m$ hằng, không chỉ khi thế tách được | Năng lượng và xung lượng **chỉ** giao hoán khi $\partial_i V = 0$, tức thế không phụ thuộc tọa độ tương ứng |

Các hệ thức giao hoán cần được hiểu trên miền tác dụng phù hợp. Trong hệ không đồng nhất, khi thế và khối lượng biến thiên theo vị trí thì phải tính trực tiếp commutator thay vì dùng các hệ số cố định như trong bảng.

### Bất định từ giao hoán

Với hai toán tử tự liên hợp có mô-men bậc hai hữu hạn:

$\Delta A\,\Delta B\geq\frac12|\langle[\hat A,\hat B]\rangle|$.

Do $[\hat x,\hat p]=i\hbar$ suy ra:

$\Delta x\,\Delta p_x\geq\frac{\hbar}{2}$.

Thời gian trong phương trình Schrödinger về cơ bản là tham số tiến hóa, không phải một toán tử tự liên hợp đơn giản; vì vậy không nên dùng máy móc hệ thức Robertson cho “năng lượng–thời gian”.

## Ví dụ vật lý

- Hạt trong hố thế vô hạn: với $0<x<L$, hàm riêng $\sqrt{2/L}\sin(n\pi x/L)$ và mức năng lượng $E_n=n^2\pi^2\hbar^2/(2mL^2)$ là kết quả của bài toán trị riêng $\hat H$, với $n=1,2,\ldots$.
- Dao động tử: $\hat H$ và các điều kiện biên dẫn đến $E_n=\hbar\omega(n+1/2)$; xem [[Phương trình Schrödinger]].
- Nguyên tử hydro: trị riêng năng lượng phụ thuộc vào số lượng tử chính; mô-men xung lượng cung cấp các trạng thái phụ thuộc $l,m_l$.
- Chuẩn delta của vị trí và xung lượng cho thấy vì sao hai cơ sở liên tục phải được hiểu bằng phân bố.

## Kiểm chứng & giới hạn

- Toán tử tọa độ và xung lượng là các ví dụ kinh điển về toán tử không bị chặn; cần xét miền tác dụng khi áp dụng lên hàm sóng.
- Công thức Hamiltonian ở trên áp dụng cho hạt phi tương đối tính, không bao gồm hạt phản vật và tương tác trường mạnh.
- Số lượng tử orbital mô tả trung tâm; trường không tâm, tương tác từ trường và cấu trúc tinh thể có thể phá vỡ sự đối xứng quay.
- Các hệ thức giao hoán là nội dung toán học, không phải kết luận rằng máy đo có sai số.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Cơ sở toán học của cơ học lượng tử]]
- [[Toán tử trong cơ học lượng tử]] · [[Không gian Hilbert]] · [[Ký hiệu Dirac]]
- [[Phương trình Schrödinger]] · [[Hàm sóng]] · [[Tiên đề cơ học lượng tử]]
- [[Nguyên lý bất định Heisenberg]] · [[Động lượng]] · [[Cơ học Hamilton]] · [[Mẫu nguyên tử Bohr]]
- [[Hàm Dirac delta]] · [[Biến đổi Fourier]]

## Câu hỏi mở

1. Vì sao toán tử xung lượng cần điều kiện biên để có một tập trạng thái riêng thích hợp?
2. Tại sao $\hat x$ đơn giản hơn $\hat p$ trong cơ sở tọa độ nhưng hai toán tử vẫn không giao hoán?
3. Hamiltonian phụ thuộc thời gian có còn các trạng thái năng lượng tĩnh không?
4. Vì sao cần cả $\hat L^2$ và $\hat L_z$ để mô tả trạng thái orbital?
5. Hệ thức giao hoán nào giải thích trực tiếp bất định vị trí–xung lượng?
