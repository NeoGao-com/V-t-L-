---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Biểu diễn Schrödinger, Heisenberg và tương tác

> [!abstract] Ý chính
> Ba "bức tranh" (picture) chỉ khác nhau ở chỗ phân chia sự tiến hóa thời gian giữa trạng thái và toán tử: Schrödinger quay trạng thái, Heisenberg quay toán tử ($i\hbar\dot F = [F,H]$), tương tác (Dirac) quay cả hai theo phần phân tách $H = H_0 + V$ — chúng đơn nguyên tương đương, nên cho kết quả đo như nhau.

## Phát biểu / Định nghĩa

Cả ba biểu diễn đều dựa trên phép chuyển biểu diễn phụ thuộc thời gian ([[Sự chuyển biểu diễn và phép biến đổi unita]]) — chỉ là "đổi bảng tọa độ" theo thời gian:

**9.1. Biểu diễn Schrödinger (mặc định):**

Trạng thái tiến hóa, toán tử đứng yên:

$i\hbar\,\dfrac{\partial}{\partial t}|\psi_S(t)\rangle = \hat H\,|\psi_S(t)\rangle, \qquad \dfrac{d\hat F_S}{dt} = 0$

Nghiệm: $|\psi_S(t)\rangle = e^{-iHt/\hbar}|\psi_S(0)\rangle$ ([[Phương trình Schrödinger dạng ma trận]]).

**9.2. Biểu diễn Heisenberg:**

Toán tử tiến hóa, trạng thái đứng yên — tương tự [[Cơ học Hamilton|hàm theo thời gian trong cơ học cổ điển]]:

$\hat F_H(t) = e^{iHt/\hbar}\,\hat F_S\,e^{-iHt/\hbar}, \qquad |\psi_H\rangle = |\psi_S(0)\rangle$

$i\hbar\,\dfrac{d\hat F_H}{dt} = [\hat F_H, \hat H] + i\hbar\,\dfrac{\partial \hat F_H}{\partial t}$ (xem [[Đạo hàm của toán tử theo thời gian]])

Tiện lợi: toán tử bảo toàn là $\hat F$ giao hoán với $\hat H$ ([[Tích phân chuyển động]]); trực tiếp liên hệ giao hoán tử với cổ điển ([[Định lý Ehrenfest]]).

**9.3. Biểu diễn tương tác (Dirac):**

Tách $\hat H = \hat H_0 + \hat V$ ($\hat H_0$ "dễ" — thường là phần không nhiễu loạn). Biến đổi unita ngược với phần tự do:

$|\psi_I(t)\rangle = e^{iH_0 t/\hbar}\,|\psi_S(t)\rangle, \qquad \hat F_I(t) = e^{iH_0 t/\hbar}\,\hat F_S(t)\,e^{-iH_0 t/\hbar}$

$i\hbar\,\dfrac{\partial}{\partial t}|\psi_I(t)\rangle = \hat V_I(t)\,|\psi_I(t)\rangle, \qquad \hat V_I(t) = e^{iH_0 t/\hbar}\,\hat V_S\,e^{-iH_0 t/\hbar}$

— trạng thái chỉ tiến hóa do **phần tương tác**, toán tử quay theo $H_0$: nền tảng của [[Đối xứng và các định luật bảo toàn|lý thuyết nhiễu loạn phụ thuộc thời gian]], quy tắc vàng Fermi, [[Phép đo lượng tử|biên độ chuyển mức]] trong [[Quang phổ]] và tán xạ.

**Bảng so sánh (đại lượng đo $\langle\hat F\rangle$ là một trong ba):**

| Picture | Trạng thái | Toán tử | Phương trình chuyển động |
| --- | --- | --- | --- |
| Schrödinger | $|\psi_S(t)\rangle = e^{-iHt/\hbar}|\psi_S(0)\rangle$ | $\hat F_S$ (tĩnh) | $i\hbar\,\partial_t|\psi\rangle = H|\psi\rangle$ |
| Heisenberg | $|\psi_H\rangle$ (tĩnh) | $\hat F_H(t) = e^{iHt/\hbar}\hat F_S e^{-iHt/\hbar}$ | $i\hbar\,\dot F = [F,H] + i\hbar\,\partial F/\partial t$ |
| Tương tác | $|\psi_I(t)\rangle = e^{iH_0t/\hbar}|\psi_S(t)\rangle$ | $\hat F_I(t) = e^{iH_0t/\hbar}\hat F_S e^{-iH_0t/\hbar}$ | $i\hbar\,\partial_t|\psi_I\rangle = V_I|\psi_I\rangle$ |

## Suy luận từ đâu

- Tiên đề gốc: tiên đề tiến hóa ([[Phương trình Schrödinger]]) + ý tưởng phép biến đổi unita ([[Sự chuyển biểu diễn và phép biến đổi unita]]) — cùng một tiên đề, ba cách "chia cắt" thời gian.
- Công cụ toán: nhóm unita $e^{-iHt/\hbar}$, giao hoán tử; khai triển nhiễu loạn (chuỗi Dyson) trong [[Đại số tuyến tính|mũ ma trận]] khi $H$ phụ thuộc thời gian.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: mọi tiên đoán (xác suất chuyển, phổ, tỉ số nhánh) tính được bằng cả ba picture cho cùng số — ví dụ tính tán xạ trong Heisenberg vs nhiễu loạn trong tương tác đều khớp đo; động lực qubit trong X-quang/laser dùng picture tương tác.
- Trường hợp không còn đúng: khi $H_0$ không tách được sạch (tương tác mạnh, nhiễu loạn mất hiệu lực — QCD, phân tử phân ly) picture tương tác mất tiện ích; hệ hở/môi trường cần siêu toán tử và phương trình Markovian (Lindblad) ngoài ba picture này.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Sự chuyển biểu diễn và phép biến đổi unita]]
- [[Phương trình Schrödinger dạng ma trận]]
- [[Đạo hàm của toán tử theo thời gian]]
- [[Tích phân chuyển động]]
- [[Định lý Ehrenfest]]

## Câu hỏi mở

- "Phần tách $H_0 + V$" là quy ước của người tính — vậy có tồn tại "phần tách tự nhiên" không? (Bức tranh trực giao Heisenberg–Dirac trong lý thuyết trường chọn $H_0$ làm trường tự do.)
- Trong Heisenberg picture, toán tử bảo toàn giao hoán với $H$ — nhưng [[Nguyên lý bất định Heisenberg|bất định năng lượng–thời gian]] được nhìn thế nào nếu thời gian chỉ là tham số, không phải toán tử?