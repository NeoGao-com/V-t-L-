---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Nguyên tử Hydro

> [!abstract] Ý chính
> Giải phương trình Schrödinger cho thế Coulomb $V = -\dfrac{Ze^2}{4\pi\varepsilon_0 r}$ cho phổ năng lượng gián đoạn $E_n = -\dfrac{13{,}6\,Z^2}{n^2}$ eV khớp chính xác với công thức Bohr, nhưng hàm sóng đầy đủ $\psi_{nlm}$ còn mang thêm thông tin về mô-men xung lượng — mô hình Bohr đúng về năng lượng, sai về quỹ đạo.

## Phát biểu / Định nghĩa

Với $V(r) = -\dfrac{Ze^2}{4\pi\varepsilon_0 r}$ (hạt nhân tích $Ze$), phương trình bán kính ([[Phương trình Schrödinger trong trường xuyên tâm]]) giải được chính xác với phương pháp chuỗi.

**3.1. Giá trị âm của năng lượng — trạng thái liên kết:**

- Năng lượng $E < 0$: electron bị "giam" bởi Coulomb — phổ gián đoạn; $E > 0$: electron tự do — phổ liên tục (trạng thái ion hóa).
- Mức càng âm càng bền; cần năng lượng $\Delta E = 0 - E_1$ để ion hóa từ trạng thái cơ bản.

**3.2. Năng lượng và hàm sóng:**

$E_n = -\dfrac{me^4Z^2}{2\hbar^2(4\pi\varepsilon_0)^2}\,\dfrac{1}{n^2} = -\dfrac{13{,}6\,Z^2}{n^2}\ \text{eV}, \qquad n = 1,2,3,\dots$

với $n$ là **số lượng tử chính**; $E_n$ không phụ thuộc $l$, $m$ (suy biến bậc $n^2$ — tổng $\sum_{l=0}^{n-1}(2l+1) = n^2$).

Hàm sóng (bán kính Bohr $a_0 = \dfrac{4\pi\varepsilon_0\hbar^2}{me^2} \approx 0{,}529$ Å):

$\psi_{nlm}(r,\theta,\phi) = R_{nl}(r)\,Y_{lm}(\theta,\phi)$

với $R_{nl}$ chứa đa thức Laguerre suy rộng, số mũ $e^{-Zr/na_0}$ và hệ số $Z^{3/2}$. Vài trạng thái đầu ($Z=1$):

| $(n,l,m)$ | $\psi_{nlm}$ |
| --- | --- |
| $(1,0,0)$ | $\dfrac{1}{\sqrt{\pi a_0^3}}\,e^{-r/a_0}$ |
| $(2,0,0)$ | $\dfrac{1}{4\sqrt{2\pi a_0^3}}\left(2 - \dfrac{r}{a_0}\right)e^{-r/2a_0}$ |
| $(2,1,m)$ | $\dfrac{1}{4\sqrt{2\pi a_0^3}}\,\dfrac{r}{a_0}\,e^{-r/2a_0}\,Y_{1m}(\theta,\phi)$ |

- **Ion tương tự hydro:** $He^+$ ($Z=2$), $Li^{2+}$ ($Z=3$)... — năng lượng tỉ lệ $Z^2$, kích thước tỉ lệ $\dfrac{1}{Z}$ (bán kính đặc trưng $\dfrac{a_0}{Z}$).
- Số nút bán kính: $n - l - 1$; parity $(-1)^l$.

**3.3. Kết luận:**

1. **Khớp Bohr:** công thức năng lượng trùng mẫu Bohr ([[Mẫu nguyên tử Bohr]]) — Bohr đúng về các mức, sai về bản chất "quỹ đạo hình học".
2. **Vượt Bohr:** mô-men xung lượng $l(l+1)\hbar^2$ và hình chiếu $m\hbar$ là hằng số chuyển động phụ — mỗi mức $n$ gồm nhiều trạng thái khác $l,m$; kết quả khớp [[Quang phổ]] hydro tới ~8 chữ số.
3. **Suy biến $n^2$ và đối xứng ẩn:** năng lượng không phụ thuộc $l$ không phải do đối xứng quay (chỉ cho $2l+1$) — mà do vector Runge–Lenz, đối xứng $SO(4)$/$SU(2)\times SU(2)$ (xem [[Đối xứng và các định luật bảo toàn]]).
4. **Giới hạn của mô hình:** mô hình một electron — không kể spin, hiệu ứng tương đối tính (cấu trúc tinh tế), dịch chuyển Lamb (QED), tương tác với từ trường (Zeeman).

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng + thế Coulomb ([[Trường xuyên tâm]], [[Phương trình Schrödinger trong trường xuyên tâm]]).
- Công cụ toán: phương pháp chuỗi (Frobenius) cho phương trình bán kính — yêu cầu chuỗi chấm dứt ⟹ lượng tử hóa $n$; đa thức Laguerre; [[Toán tử mô-men xung lượng]] và hàm cầu.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: dãy Lyman, Balmer, Paschen với độ chính xác cao ([[Quang phổ]], [[Thí nghiệm - Franck-Hertz]]); năng lượng ion hóa hydro $13{,}6$ eV đo được trực tiếp.
- Trường hợp không còn đúng: cấu trúc tinh tế (tách mức do spin–quỹ đạo, thứ tự $\alpha^4mc^2$); dịch chuyển Lamb (cần QED); nguyên tử nhiều electron — thế không còn xuyên tâm thuần túy, $E$ phụ thuộc $l$ (chữ ký của bảng tuần hoàn).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Mẫu nguyên tử Bohr]]
- [[Phương trình Schrödinger trong trường xuyên tâm]]
- [[Trường xuyên tâm]]
- [[Sự phân bố electron trong nguyên tử Hydro]]
- [[Quang phổ]]

## Câu hỏi mở

- Vì sao nguyên tử hydro lại "tình cờ" có suy biến $n^2$ — điều gì phân biệt thế $1/r$ với mọi thế xuyên tâm khác? (Đối xứng Runge–Lenz bảo toàn cả hướng lệch tâm quỹ đạo.)
- Một electron ở trạng thái dừng có "chuyển động" quanh hạt nhân không — và mật độ xác suất thực sự cho thấy hình ảnh nào? (Xem [[Sự phân bố electron trong nguyên tử Hydro]].)