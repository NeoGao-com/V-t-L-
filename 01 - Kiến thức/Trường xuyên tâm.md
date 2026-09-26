---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Trường xuyên tâm

> [!abstract] Ý chính
> Thế năng chỉ phụ thuộc khoảng cách $V(\vec r) = V(r)$ (trường xuyên tâm/có tâm) có đối xứng quay hoàn toàn — nên $\hat{\vec L}$ giao hoán với $\hat H$: mô-men xung lượng là tích phân chuyển động, trạng thái dừng được đặc trưng bởi ba số lượng tử $(E, l, m)$ và suy biến bậc $2l+1$.

## Phát biểu / Định nghĩa

**1.1. Khái niệm trường xuyên tâm:**

Trường xuyên tâm là trường thế năng bất biến dưới mọi phép quay quanh một điểm cố định (tâm):

$V(\vec r) = V(r), \qquad r = |\vec r|$

Ví dụ: lực Coulomb $V = -\dfrac{kZe^2}{r}$ của nguyên tử, lực hấp dẫn $V = -\dfrac{GMm}{r}$, thế đàn hồi $V = \dfrac{1}{2}m\omega^2r^2$.

**1.2. Bảo toàn đại lượng quay:** vì $V(r)$ bất biến khi quay, Hamiltonian cũng vậy: $[\hat{\vec L}, \hat H] = 0$ cho từng thành phần — hệ quả của [[Đối xứng và các định luật bảo toàn]] (đối xứng quay ↔ bảo toàn mô-men xung lượng). Nhờ đó $\hat H$, $\hat L^2$, $\hat L_z$ có hệ hàm riêng chung ([[Đo đồng thời các đại lượng trong cơ học lượng tử]]) — không cần đo đạc thêm, ba đại lượng này luôn xác định đồng thời.

**1.3. Các đặc điểm của hạt chuyển động trong trường xuyên tâm:**

1. **Ba số lượng tử đặc trưng trạng thái:** năng lượng $E$, mô-men xung lượng toàn phần $l$ (với $l(l+1)\hbar^2$) và hình chiếu $m\hbar$; trạng thái ký hiệu $|n\,l\,m\rangle$.
2. **Suy biến $2l+1$:** với mỗi mức $E_{nl}$ có $2l+1$ trạng thái ứng với $m = -l,\dots,+l$ — do năng lượng không phụ thuộc phương của $\hat{\vec L}$ (không gian đẳng hướng). Trạng thái $l=0$ (orbital $s$) không suy biến.
3. **Chuyển động trở về "một chiều hiệu dụng":** động năng quay tách khỏi động năng bán kính (xem [[Phương trình Schrödinger trong trường xuyên tâm]]) — bài toán 3D qui về phương trình bán kính một chiều.
4. **Tính chẵn lẻ:** hàm sóng có parity $(-1)^l$ — đổi dấu hay không khi đảo không gian, giúp giải thích quy tắc chọn lọc.
5. **Cổ điển tương ứng:** mô-men xung lượng cố định → quỹ đạo nằm trong một mặt phẳng vuông góc với $\vec L$ (chuyển động Kepler quen thuộc, liên hệ [[Chuyển động quay của vật rắn]]).

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng ([[Phương trình Schrödinger]]); điều kiện tích phân chuyển động $[\hat H,\hat A]=0$ trong [[Tích phân chuyển động]].
- Công cụ toán: [[Lý thuyết nhóm]] (đối xứng quay $SO(3)$), tính chất toán tử $\hat{\vec L}$ ([[Toán tử mô-men xung lượng]]).

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: mô-men xung lượng lượng tử hóa đo trực tiếp qua [[Thí nghiệm - Stern-Gerlach]]; suy biến $2l+1$ thấy trong vạch [[Quang phổ]] của nguyên tử (tách bởi từ trường → hiệu ứng Zeeman); thế Coulomb của [[Nguyên tử Hydro]] là áp dụng hoàn hảo.
- Trường hợp không còn đúng: trường không xuyên tâm (nguyên tử nhiều electron — tương tác electron–electron phá đối xứng quay một phần; tinh thể có trục ưu tiên); khi có spin–quỹ đạo, $\hat{\vec L}$ không còn riêng lẻ bảo toàn (chỉ $\hat{\vec J} = \hat{\vec L} + \hat{\vec S}$).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Toán tử mô-men xung lượng]]
- [[Phương trình Schrödinger trong trường xuyên tâm]]
- [[Đối xứng và các định luật bảo toàn]]
- [[Đo đồng thời các đại lượng trong cơ học lượng tử]]
- [[Nguyên tử Hydro]]

## Câu hỏi mở

- Vì sao $E_{nl}$ (của thế Coulomb) không phụ thuộc $l$ — suy biến $l$ có phải do đối xứng quay sinh ra không? (Không — đây là đối xứng ẩn họ Runge–Lenz, xem [[Nguyên tử Hydro]].)
- Quỹ đạo cổ điển "giam trong mặt phẳng" tương ứng lượng tử với điều gì — và vì sao xác suất lượng tử lại không tập trung trên một mặt phẳng? (Chồng chập $m$ làm mất mặt phẳng khi không đo $L_z$.)