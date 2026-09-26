---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Thế bậc thang

> [!abstract] Ý chính
> Hạt tới một bậc thế $V_0$: với $E > V_0$ bị phản xạ một phần dù cổ điển thì truyền qua toàn bộ; với $E < V_0$ phản xạ toàn phần nhưng hàm sóng vẫn thâm nhập vùng cấm theo hàm mũ — hiệu ứng thuần túy lượng tử, không có dòng truyền qua.

## Phát biểu / Định nghĩa

Thế năng: $V(x) = 0$ với $x < 0$; $V(x) = V_0$ với $x > 0$. Hạt tới từ trái với năng lượng $E$.

**Trường hợp 1 — $E > V_0$:** nghiệm hai bên là sóng phẳng với

$k_1 = \dfrac{\sqrt{2mE}}{\hbar} \quad(\text{miền } x<0), \qquad k_2 = \dfrac{\sqrt{2m(E-V_0)}}{\hbar} \quad(\text{miền } x>0)$

Khớp $\psi$, $\psi'$ tại $x=0$ (xem [[Chuyển động một chiều trong cơ học lượng tử]]):

- Hệ số phản xạ: $R = \left(\dfrac{k_1 - k_2}{k_1 + k_2}\right)^2$
- Hệ số truyền qua: $T = \dfrac{4k_1k_2}{(k_1+k_2)^2}$, và $R + T = 1$ (bảo toàn dòng — [[Mật độ dòng xác suất]])

Dù $E > V_0$, vẫn có xác suất phản xạ $R > 0$ (trừ khi $V_0 = 0$) — điều cổ điển không có.

**Trường hợp 2 — $E < V_0$:** ở $x > 0$, $\psi \propto e^{-\kappa x}$ với $\kappa = \dfrac{\sqrt{2m(V_0-E)}}{\hbar}$:

- $R = 1$, $T = 0$ — phản xạ toàn phần, **không có dòng** trong vùng cấm.
- Nhưng mật độ xác suất $\propto e^{-2\kappa x}$ vẫn khác 0: hạt "thấm" vào vùng cấm độ sâu $1/\kappa$ rồi quay lại — tương tự sóng ánh sáng phản xạ toàn phần với sóng rò evanescent.

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng + điều kiện nối tiếp tại $x=0$; dòng xác suất phải liên tục.
- Công cụ toán: nghiệm tổ hợp $e^{\pm ikx}$ ([[Hạt tự do trong cơ học lượng tử]]), hệ hai phương trình đại số cho $R$, $T$.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: hệ số phản xạ của electron tại rào thế kim loại/bán dẫn (hàm công), phản xạ neutron chậm trên bề mặt chất lỏng — đo $R$ khớp công thức bậc thang; tương ứng quang học: hệ số Fresnel tại mặt phân cách hai môi trường.
- Trường hợp không còn đúng: với $E$ rất gần $V_0$ ($k_2\to 0$) xấp xỉ sóng phẳng kém chính xác, cần kể cả nghiệm không tiệm cận; bậc thang nghiêng dần mất tính phản xạ dị hướng — cần giải số hoặc xấp xỉ WKB.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Mật độ dòng xác suất]]
- [[Hàng rào thế và hiệu ứng đường ngầm]]
- [[Giếng thế hữu hạn]]
- [[Chuyển động một chiều trong cơ học lượng tử]]

## Câu hỏi mở

- Khi $E < V_0$ và phản xạ toàn phần, hạt "nán lại" bao lâu trong vùng cấm? (Có độ trễ pha, liên quan thời gian trễ tunneling.)
- Vì sao hệ số phản xạ cổ điển bằng 0 nhưng lượng tử khác 0 — nguồn gốc của $R$ nằm ở tính chất nào của sóng? (Không khớp đạo hàm tại biên khi $k_1 \ne k_2$.)