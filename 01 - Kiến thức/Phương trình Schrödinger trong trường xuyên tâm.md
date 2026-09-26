---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Phương trình Schrödinger trong trường xuyên tâm

> [!abstract] Ý chính
> Trong trường xuyên tâm, tách biến cầu tách phương trình Schrödinger thành phương trình góc (hàm cầu $Y_{lm}$ — nghiệm chung của $\hat L^2,\hat L_z$) và phương trình bán kính một chiều với thế hiệu dụng chứa số hạng ly tâm $\dfrac{\hbar^2 l(l+1)}{2mr^2}$ — bài toán 3D thu về dao động một chiều với điều kiện biên $u(0)=0$.

## Phát biểu / Định nghĩa

**2.1. Tách biến — phương trình bán kính và phương trình góc:**

Với $V(\vec r) = V(r)$, trong tọa độ cầu:

$\psi(r,\theta,\phi) = R(r)\,Y_{lm}(\theta,\phi) = \dfrac{u(r)}{r}\,Y_{lm}(\theta,\phi)$

- **Phương trình góc** đã được giải trọn vẹn bởi hàm cầu ([[Toán tử mô-men xung lượng]]): $\hat L^2Y_{lm} = l(l+1)\hbar^2Y_{lm}$.
- **Phương trình bán kính** cho $u(r) = rR(r)$:

$-\dfrac{\hbar^2}{2m}\,u''(r) + V_{\text{hd}}(r)\,u(r) = E\,u(r), \qquad V_{\text{hd}}(r) = V(r) + \dfrac{\hbar^2 l(l+1)}{2mr^2}$

số hạng $\dfrac{\hbar^2 l(l+1)}{2mr^2}$ là **thế ly tâm** — tương tự động năng quay cổ điển $\dfrac{L^2}{2mr^2}$, đẩy hạt ra xa tâm và càng mạnh khi $l$ lớn.

**2.2. Khảo sát phương trình bán kính:**

1. **Điều kiện biên:** tại $r=0$, $u(0) = 0$ (đảm bảo $R$ hữu hạn; với $l>0$, $u \sim r^{l+1}$); tại $r\to\infty$: $u \to 0$ với trạng thái liên kết ($E<0$), $u$ dao động với phổ liên tục với $E>0$.
2. **Phổ gián đoạn:** giống bài toán một chiều ([[Chuyển động một chiều trong cơ học lượng tử]]), trạng thái liên kết đếm được, ký hiệu bởi **số lượng tử chính $n$** và $l$: $E = E_{nl}$.
3. **Số nút:** hàm bán kính có $n - l - 1$ nút (thế Coulomb); trạng thái càng cao nút càng nhiều.
4. **Mỗi mức suy biến $2l+1$** theo $m$ ([[Trường xuyên tâm]]); tổng trên $l$ cho suy biến bậc $n^2$ với thế Coulomb (đối xứng ẩn, xem [[Nguyên tử Hydro]]).
5. **Chuẩn hóa:** $\displaystyle\int_0^\infty |u(r)|^2\,dr = 1$ cùng $\displaystyle\int |Y_{lm}|^2\,d\Omega = 1$.
6. **Thế hiệu dụng với $V(r) = -\dfrac{k}{r}$:** hút mạnh ở $r$ nhỏ, ly tâm đẩy ở $r$ nhỏ → cực tiểu $V_{\text{hd}}$ tồn tại với $l>0$; số trạng thái liên kết hữu hạn cho mỗi $l$.

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng 3 chiều ([[Phương trình Schrödinger]]); đối xứng quay cho $[\hat H,\hat L^2,\hat L_z]=0$ ([[Trường xuyên tâm]]).
- Công cụ toán: tách biến trong tọa độ cầu ([[Tách biến trong phương trình Schrödinger ba chiều]] — tổng quát hóa cho $V(r)$), hàm cầu, phương trình vi phân thường bậc hai với điểm kỳ dị đều (phương pháp chuỗi Frobenius).

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: cấu trúc mức của [[Nguyên tử Hydro]] và ion tương tự; thế ly tầm giải thích tại sao electron $l$ cao khó "chạm" hạt nhân (liên hệ giả thuyết chụp electron $e^-$ trong phân rã $\beta$ — xác suất tại $r=0$ tỉ lệ $|R_{nl}(0)|^2$, khác 0 chỉ khi $l=0$).
- Trường hợp không còn đúng: thế có điểm kỳ dị mạnh hơn $1/r^2$ (rơi vào tâm — cần xử lý đặc biệt); khi thế phụ thuộc góc hoặc không phải $V(r)$, tách biến cầu không còn hiệu lực (cần thế khác hoặc giải số).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Trường xuyên tâm]]
- [[Toán tử mô-men xung lượng]]
- [[Nguyên tử Hydro]]
- [[Tách biến trong phương trình Schrödinger ba chiều]]
- [[Chuyển động một chiều trong cơ học lượng tử]]

## Câu hỏi mở

- Số hạng ly tâm giống hệt thế $1/r^2$ — vì sao không gây "rơi vào tâm" dù $l$ nhỏ? (Biên $u(0)=0$ loại nghiệm kỳ dị.)
- Khi $E>0$ (tán xạ), phương trình bán kính cho pha tán xạ theo $l$ — vai trò của $V_{\text{hd}}$ trong việc xác định tiết diện tán xạ là gì? (Mở đường sang lý thuyết tán xạ.)