---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Hàng rào thế và hiệu ứng đường ngầm

> [!abstract] Ý chính
> Hạt có năng lượng $E < V_0$ vẫn có thể xuyên qua một hàng rào thế với xác suất $T \propto e^{-2\kappa a}$ — hiệu ứng đường ngầm (tunneling) thuần túy lượng tử, giải thích phân rã alpha, phản ứng nhiệt hạch trong sao và là nguyên lý của kính hiển vi quét xuyên hầm (STM).

## Phát biểu / Định nghĩa

Thế năng: $V(x) = V_0$ với $0 < x < a$; $V = 0$ hai bên. Xét $E < V_0$:

- Miền I ($x<0$): sóng tới + phản xạ; miền III ($x>a$): sóng truyền qua.
- Miền II (trong hàng rào): $\psi \propto A e^{\kappa x} + B e^{-\kappa x}$ với $\kappa = \dfrac{\sqrt{2m(V_0-E)}}{\hbar}$ — không phải dao động mà là **khuếch giảm**.

Khớp điều kiện biên tại hai mặt $x=0$ và $x=a$ cho hệ số truyền qua chính xác:

$T = \dfrac{1}{1 + \dfrac{V_0^2\sinh^2(\kappa a)}{4E(V_0-E)}}$

Với hàng rào cao và rộng ($\kappa a \gg 1$): $T \approx 16\,\dfrac{E}{V_0}\left(1-\dfrac{E}{V_0}\right)e^{-2\kappa a}$ — giảm **theo hàm mũ** theo bề rộng và $\sqrt{m(V_0-E)}$.

**Hàng rào thế dạng tùy ý** $V(x)$ (công thức Gamow–Condon–Gurney):

$T \approx \exp\left[-\dfrac{2}{\hbar}\displaystyle\int_{x_1}^{x_2}\sqrt{2m\big(V(x)-E\big)}\,dx\right]$

**Ứng dụng tiêu biểu:**

1. **Phân rã alpha:** hạt $\alpha$ trong nhân xuyên rào Coulomb — chu kỳ bán rã nhạy hàm mũ với năng lượng (định luật Geiger–Nuttall).
2. **Nhiệt hạch trong sao:** hai hạt nhân xuyên rào Coulomb — đây là lý do phản ứng xảy ra ở nhiệt độ thấp hơn nhiều so với năng lượng Gamow.
3. **Kính hiển vi quét xuyên hầm (STM):** dòng điện xuyên hầm qua khe chân không, $T \propto e^{-2\kappa d}$ với $d$ là khoảng cách — nhạy cỡ Å cho độ phân giải nguyên tử.
4. Diode đường hầm (Esaki), hiệu ứng Josephson, chuyển mạch trong flash memory.

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng, thâm nhập vùng cấm trong [[Chuyển động một chiều trong cơ học lượng tử]], bảo toàn dòng [[Mật độ dòng xác suất]].
- Công cụ toán: hàm hyperbolic $\sinh(\kappa a)$; tích phân của công thức Gamow; khớp 4 hệ số tại 2 biên.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: ảnh STM với độ phân giải nguyên tử; sự phụ thuộc chu kỳ phân rã alpha vào năng lượng (log–log tuyến tính Geiger–Nuttall); phóng xạ từ trường không làm lệch hạt $\alpha$ đã thoát khỏi nhân — xác nhận cơ chế xuyên hầm.
- Trường hợp không còn đúng: với hàng rào mỏng và $E \approx V_0$, công thức xấp xỉ mũ không dùng được (cần $T$ chính xác, khi $\kappa a \ll 1$ thì $T\to 1$); khi có tán xạ không đàn hồi trong rào (mất kết hợp), phải dùng ma trận mật độ.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Thế bậc thang]]
- [[Giếng thế hữu hạn]]
- [[Phóng xạ]]
- [[Mật độ dòng xác suất]]

## Câu hỏi mở

- Hạt xuyên hầm "mất bao lâu" để xuyên qua rào? (Tranh luận về thời gian tunneling — đo bằng xung attosecond.)
- Với hàng rào đôi có cộng hưởng xuyên hầm — hiện tượng tương tự vì sao xuất hiện ở [[Dao động tử điều hòa lượng tử|trạng thái dừng]]?