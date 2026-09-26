---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Phép biến đổi Laplace

> [!abstract] Công cụ để làm gì
> Biến đổi Laplace là "người anh cả" của [[Biến đổi Fourier]] dành cho các hàm chỉ sống từ $t = 0$: nó **đại số hóa đạo hàm thành phép nhân** và đưa điều kiện đầu vào thẳng công thức — vũ khí giải nhanh các phương trình vi phân của mạch điện và dao động tắt dần.

## Định nghĩa

Biến đổi Laplace thuận:

$\mathcal{L}\{f\}(s) = \int_{0}^{\infty} f(t)\, e^{-st}\, dt, \qquad s = \sigma + i\omega$

Bảng cặp và tính chất chính:

| $f(t)$ | $\mathcal{L}\{f\}$ |
| --- | --- |
| $1$ | $\dfrac{1}{s}$ |
| $t^n\ (n \in \mathbb{N})$ | $\dfrac{n!}{s^{n+1}}$ |
| $e^{at}$ | $\dfrac{1}{s - a}$ |
| $e^{at}\sin(\omega t)$, $e^{at}\cos(\omega t)$ | $\dfrac{\omega}{(s-a)^2+\omega^2}$, $\dfrac{s-a}{(s-a)^2+\omega^2}$ |
| $f'(t)$ | $sF(s) - f(0)$ |
| $f''(t)$ | $s^2 F(s) - sf(0) - f'(0)$ |
| $\displaystyle\int_0^t f(\tau)\,d\tau$ | $\dfrac{F(s)}{s}$ |
| Trễ $f(t-a)\,u(t-a)$ ($a>0$) | $e^{-as}F(s)$ |
| Tích chập $f * g$ | $F(s)\, G(s)$ |
| **Định lý giá trị cuối** (nếu tồn tại giới hạn) | $\lim_{t\to\infty} f(t) = \lim_{s\to0} sF(s)$ |

- **Tính chất chủ lực:** đạo hàm ↔ nhân với $s$ (kèm điều kiện đầu) — biến phương trình vi phân thành **phương trình đại số**; điều kiện đầu "nhảy vào" tự nhiên, không cần đoán nghiệm riêng.
- **Tính chất trễ:** độ trễ thời gian ↔ nhân với $e^{-as}$ — "hàm bước" $u(t)$ mô hình đóng/mở công tắc, xung giới hạn.
- **Giá trị cuối:** hành vi sau "thời gian dài" của hệ nhìn thẳng từ $F(s)$ tại $s \to 0$, không cần biến đổi ngược.
- Giải: biến đổi PTVP → giải đại số → **biến đổi ngược** (bảng + phân tích hàm hữu tỉ).

## Ý nghĩa hình học

- Nhìn một "đường cong sinh trưởng/tắt dần" qua "kính phóng đại hàm mũ": $e^{-st}$ với $s = \sigma + i\omega$ vừa "soi tần số" (giống Fourier) vừa "tắt dần theo thời gian" (cửa sổ $\sigma$) — nên **hàm không hội tụ cho Fourier vẫn hội tụ cho Laplace**, và hành vi quá độ lộ ra ở phần thực $\sigma$ của cực.
- Cực của $F(s)$ trong mặt phẳng phức là "chân dung thời gian": cực $s=a$ sinh ra $e^{at}$; cực phức $a \pm i\omega$ sinh ra dao động tắt dần $e^{at}\sin\omega t$.

## Ý nghĩa vật lý

- **Ví dụ mẫu — đóng khóa mạch RL:** phương trình $L\dfrac{di}{dt} + Ri = E$ với $i(0)=0$; Laplace hóa $Ls\,I(s) + R\,I(s) = \dfrac{E}{s}$ → $I(s) = \dfrac{E}{s(Ls + R)} = \dfrac{E/R}{s} - \dfrac{E/R}{s + R/L}$ → ngay ra dòng quá độ
  $i(t) = \dfrac{E}{R}\left(1 - e^{-Rt/L}\right)$
  — nếu ngồi "đoán nghiệm riêng" theo cách cổ điển sẽ mất nhiều bước hơn ([[Mạch RLC và trở kháng]], [[Mạch điện và các phần tử mạch]], [[Tụ điện]]).
- **Dao động tắt dần:** nghiệm của $\ddot x + 2\beta \dot x + \omega_0^2 x = 0$ có cực $s = -\beta \pm i\sqrt{\omega_0^2 - \beta^2}$; cực nằm bên trái trục ảo ($\beta > 0$) = tắt dần, trên trục ảo = dao động thuần, cực lặp = tới hạn — đọc trực tiếp từ vị trí cực ([[Dao động tắt dần - Cưỡng bức - Cộng hưởng]], [[Con lắc lò xo]]).
- **Hàm truyền (transfer function):** $H(s) = Y(s)/X(s)$ — "đặc tính sinh học" của hệ, chập kích thích vào là được đáp ứng; ngôn ngữ phổ dụng của điều khiển và xử lý tín hiệu.
- **Tương ứng Laplace ↔ Fourier:** $F(s)$ với $s = i\omega$ là biến đổi Fourier của hàm nhân quả — cùng một phổ, thêm "cửa sổ" tắt dần để đảm bảo hội tụ ([[Biến đổi Fourier]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Mạch RLC và trở kháng]] · [[Mạch điện và các phần tử mạch]] · [[Tụ điện]]: đáp ứng quá độ của mạch có lời giải mẫu $RL$.
- [[Dao động tắt dần - Cưỡng bức - Cộng hưởng]] · [[Con lắc lò xo]]: nghiệm tắt dần và cộng hưởng từ cực của $F(s)$.
- [[Phương trình vi phân]]: công cụ giải nhanh PTVP tuyến tính hệ số hằng.
- [[Biến đổi Fourier]]: trường hợp riêng trên trục $s = i\omega$.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Biến đổi Fourier]] · [[Số phức]] (mặt phẳng $s$) · [[Phương trình vi phân]] · [[Mạch RLC và trở kháng]] · [[Hàm Green]] (tích chập trong miền $s$)

## Câu hỏi mở

- Vì sao "cực" của $F(s)$ quyết định cả hành vi quá độ lẫn ổn định của hệ? (Gợi ý: biến đổi ngược là tổng các hàm $e^{s_i t}$ với $s_i$ là cực — "phổ cực" là bản đồ hành vi thời gian.)
- Laplace dùng cho hệ "nhân quả" (chỉ đáp ứng từ $t = 0$) — Fourier dùng cho tín hiệu vô hạn hai chiều. Khi nào hai phép biến đổi cho cùng phổ, khi nào khác? (Gợi ý: hội tụ trên trục ảo — hệ ổn định thì $s = i\omega$ nằm trong miền hội tụ.)
- Định lý giá trị cuối đòi hỏi giới hạn phải tồn tại — khi nào nó *không* áp dụng được và vì sao? (Gợi ý: cực trên trục ảo hay nửa mặt phẳng phải — hệ "dao động mãi" hay "bùng nổ".)