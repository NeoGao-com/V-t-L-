---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Toán tử mô-men xung lượng

> [!abstract] Ý chính
> Toán tử mô-men xung lượng $\hat{\vec L} = \hat{\vec r}\times\hat{\vec p}$ là toán tử sinh của phép quay, với các giao hoán tử $[\hat L_i,\hat L_j] = i\hbar\varepsilon_{ijk}\hat L_k$ — từ đó suy ra phổ $l(l+1)\hbar^2$ cho $\hat L^2$ và $m\hbar$ cho $\hat L_z$, và hàm riêng góc chung là các hàm cầu $Y_{lm}(\theta,\phi)$.

## Phát biểu / Định nghĩa

Trong tọa độ Descartes:

$\hat{\vec L} = \hat{\vec r}\times\hat{\vec p}, \qquad \hat L_x = \hat y\hat p_z - \hat z\hat p_y,\; \dots$ (hoán vị vòng)

Trong tọa độ cầu (dùng khi tách biến, xem [[Phương trình Schrödinger trong trường xuyên tâm]]):

$\hat L_z = -i\hbar\dfrac{\partial}{\partial\phi}, \qquad \hat L^2 = -\hbar^2\left[\dfrac{1}{\sin\theta}\dfrac{\partial}{\partial\theta}\left(\sin\theta\dfrac{\partial}{\partial\theta}\right) + \dfrac{1}{\sin^2\theta}\dfrac{\partial^2}{\partial\phi^2}\right]$

**Các hệ thức giao hoán** (tựa đại số Lie $so(3)$):

1. $[\hat L_i, \hat L_j] = i\hbar\,\varepsilon_{ijk}\hat L_k$ — ba thành phần **không** đo đồng thời được (trừ khi $l=0$, xem [[Đo đồng thời các đại lượng trong cơ học lượng tử]]).
2. $[\hat L^2, \hat L_i] = 0$ — bình phương mô-men giao hoán với mọi thành phần.

**Trị riêng:**

$\hat L^2\,|l\,m\rangle = l(l+1)\hbar^2\,|l\,m\rangle, \qquad \hat L_z\,|l\,m\rangle = m\hbar\,|l\,m\rangle$

với $l = 0,1,2,\dots$ và $m = -l,\,-l+1,\dots,\,+l$ — **lượng tử hóa mô-men xung lượng**, đồng thời là nguồn gốc của [[Thí nghiệm - Stern-Gerlach]] (chùm nguyên tử tách thành $2l+1$ vệt rời rạc).

**Hàm riêng góc — hàm cầu $Y_{lm}(\theta,\phi)$** (chuẩn hóa trên mặt cầu):

$Y_{00} = \dfrac{1}{\sqrt{4\pi}},\qquad Y_{10} = \sqrt{\dfrac{3}{4\pi}}\cos\theta,\qquad Y_{1\pm1} = \mp\sqrt{\dfrac{3}{8\pi}}\sin\theta\,e^{\pm i\varphi},$

$Y_{20} = \sqrt{\dfrac{5}{16\pi}}\,(3\cos^2\theta - 1),\; \dots$

Tính chất: trực chuẩn $\displaystyle\int Y_{l'm'}^*Y_{lm}\,d\Omega = \delta_{ll'}\delta_{mm'}$; tính chẵn lẻ $P\,Y_{lm} = (-1)^l\,Y_{lm}$.

**Toán tử bậc thang:**

$\hat L_\pm = \hat L_x \pm i\hat L_y, \qquad \hat L_\pm|l\,m\rangle = \hbar\sqrt{l(l+1) - m(m\pm1)}\;|l,\,m\pm1\rangle$

— từ $|l,l\rangle$ hạ dần để dựng toàn bộ đa tuyến $2l+1$ trạng thái.

## Suy luận từ đâu

- Tiên đề gốc: lượng tử hóa thay xung lượng $\hat{\vec p} = -i\hbar\vec\nabla$ ([[Các toán tử cơ bản trong cơ học lượng tử]]).
- Công cụ toán: đại số Lie và giao hoán tử ([[Lý thuyết nhóm]], [[Suy ra hệ thức bất định từ giao hoán]]); phương trình vi phân của hàm cầu (liên quan [[Phương trình đạo hàm riêng (PDE)]]).

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: Stern–Gerlach cho $2l+1$ vệt (với spin riêng là $2s+1$); sự phụ thuộc $l(l+1)\hbar^2$ khớp cấu trúc mức và quy tắc chọn lọc của [[Quang phổ]] nguyên tử; hiệu ứng Zeeman tách theo $m$.
- Trường hợp không còn đúng: $\hat{\vec L}$ là mô-men **orbital** — hạt có spin $\hat{\vec S}$ (mô-men nội tại) không biểu diễn được qua $\hat{\vec r}\times\hat{\vec p}$; khi ghép spin–quỹ đạo, lượng bảo toàn là $\hat{\vec J} = \hat{\vec L} + \hat{\vec S}$ chứ không phải từng phần.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Trường xuyên tâm]]
- [[Phương trình Schrödinger trong trường xuyên tâm]]
- [[Đo đồng thời các đại lượng trong cơ học lượng tử]]
- [[Các toán tử cơ bản trong cơ học lượng tử]]
- [[Thí nghiệm - Stern-Gerlach]]

## Câu hỏi mở

- Vì sao $l$ chỉ nhận số nguyên — còn spin bán nguyên $s = \dfrac{1}{2}$ thì sao? (Hàm cầu không mô tả spin: $SU(2)$ thay cho $SO(3)$.)
- Tại sao $\hat L_z$ được chọn để cùng $\hat L^2$ — và hệ quả gì nếu chọn một thành phần khác? (Tương đương do đối xứng quay; mọi thành phần đều "tốt như nhau".)