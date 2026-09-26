---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Đạo hàm của toán tử theo thời gian

> [!abstract] Ý chính
> Trong bức tranh Heisenberg, toán tử (quan sát) mang sự phụ thuộc thời gian theo phương trình $\dfrac{d\hat A}{dt} = \dfrac{\partial\hat A}{\partial t} + \dfrac{i}{\hbar}[\hat H, \hat A]$ — đối xứng "ảnh" của phương trình Schrödinger, và là bản lượng tử của phương trình Hamilton $\dot A = \{A, H\}$.

## Phát biểu / Định nghĩa

Phương trình Schrödinger cho biết **trạng thái** $|\psi(t)\rangle$ biến đổi theo thời gian qua toán tử tiến hóa unita $U(t) = e^{-i\hat H t/\hbar}$. Nhưng trị trung bình $\langle\hat A\rangle = \langle\psi(t)|\hat A|\psi(t)\rangle$ có thể mô tả tương đương bằng cách dồn thời gian vào toán tử — **bức tranh Heisenberg**:

$\hat A_H(t) = e^{i\hat H t/\hbar}\,\hat A_S\, e^{-i\hat H t/\hbar}$

Đạo hàm hai vế cho **phương trình Heisenberg**:

$\dfrac{d\hat A_H}{dt} = \dfrac{\partial\hat A_H}{\partial t} + \dfrac{i}{\hbar}\,[\hat H, \hat A_H]$

trong đó $\dfrac{\partial\hat A}{\partial t}$ là phần phụ thuộc thời gian tường minh (do bên ngoài điều khiển, không phải do tiến hóa nội tại).

**Ví dụ cơ bản** (bức tranh Schrödinger, lấy trung bình sau):

- Vận tốc: $\dot{\hat x} = \dfrac{i}{\hbar}[\hat H, \hat x] = \dfrac{\hat p}{m}$ — vận tốc lượng tử là $\dfrac{\hat p}{m}$.
- Lực: $\dot{\hat p} = \dfrac{i}{\hbar}[\hat H, \hat p] = -\dfrac{\partial V(\hat x)}{\partial \hat x}$ — định luật II Newton dạng toán tử.
- Spin trong từ trường: $\dfrac{d\hat{\vec S}}{dt} = \dfrac{i}{\hbar}[\hat H, \hat{\vec S}] = \vec\omega \times \hat{\vec S}$ với $\vec\omega = -\gamma\vec B$ — tuế sai Larmor.

**Đối ứng cổ điển:** phép thay Poisson → giao hoán tử $[\,\cdot\,,\,\cdot\,] \to i\hbar\{\cdot,\cdot\}$ biến $\dot A = \{A,H\}$ của [[Cơ học Hamilton]] thành phương trình Heisenberg.

## Suy luận từ đâu

- Tiên đề gốc: tiên đề tiến hóa (A5) với toán tử tiến hóa unita $U(t)$ trong [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]; [[Phương trình Schrödinger]].
- Công cụ toán: [[Toán tử trong cơ học lượng tử]], giao hoán tử (xem [[Suy ra hệ thức bất định từ giao hoán]]); [[Cơ học Hamilton]] cho móc Poisson.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: tuế sai Larmor của spin đo bằng NMR/ESR, chu kỳ đúng $\omega_L = \gamma B$; nghiệm trung bình của phương trình toán tử khớp [[Định lý Ehrenfest]] với chuyển động cổ điển.
- Trường hợp không còn đúng: khi $\hat H$ phụ thuộc thời gian, $U(t)$ không còn dạng mũ đơn giản (cần chuỗi Dyson); hệ mở (có môi trường) không mô tả bằng toán tử unita — dùng ma trận mật độ với phương trình Liouville $\dot{\hat\rho} = -\dfrac{i}{\hbar}[\hat H, \hat\rho]$ (khác dấu với phương trình Heisenberg).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Định lý Ehrenfest]]
- [[Tích phân chuyển động]]
- [[Đối xứng và các định luật bảo toàn]]
- [[Toán tử trong cơ học lượng tử]]
- [[Cơ học Hamilton]]

## Câu hỏi mở

- Vì sao phương trình Heisenberg của toán tử và phương trình Liouville của ma trận mật độ khác dấu — và dấu đảo tương ứng với vai trò "biến độc lập" nào trong hai bức tranh?
- Khi $[\hat H,\hat A] = 0$ thì $\hat A$ không đổi — nếu $\dfrac{\partial\hat A}{\partial t} \ne 0$ (ví dụ $\hat A = t\hat H$) thì kết luận còn đúng không?