---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Giếng thế vô hạn

> [!abstract] Ý chính
> Hạt giam trong hộp thế vô hạn một chiều có phổ gián đoạn $E_n = \dfrac{n^2\pi^2\hbar^2}{2mL^2}$ với hàm sóng hình sin thuần túy — mô hình đơn giản nhất của sự lượng tử hóa năng lượng do điều kiện biên, và là nền của mọi giếng lượng tử thực tế.

## Phát biểu / Định nghĩa

Thế năng: $V(x) = 0$ với $0 < x < L$; $V(x) = \infty$ ngoài khoảng đó. Hạt không thể ra ngoài nên điều kiện biên: $\psi(0) = \psi(L) = 0$.

Nghiệm trong giếng (từ [[Phương trình Schrödinger]] dừng với $V=0$, xem [[Hạt tự do trong cơ học lượng tử]]):

$\psi_n(x) = \sqrt{\dfrac{2}{L}}\,\sin\dfrac{n\pi x}{L}, \qquad E_n = \dfrac{n^2\pi^2\hbar^2}{2mL^2} = \dfrac{n^2h^2}{8mL^2}, \quad n = 1,2,3,\dots$

**Tính chất:**

- Năng lượng gián đoạn, tỉ lệ $n^2$; $n=1$ thấp nhất: $E_1 = \dfrac{\pi^2\hbar^2}{2mL^2} > 0$ — hạt bị giam không bao giờ đứng yên (mâu thuẫn với cơ học cổ điển).
- Hàm sóng trực giao chuẩn hóa: $\langle\psi_m|\psi_n\rangle = \delta_{mn}$; trạng thái $n$ có $n-1$ nút bên trong (đúng [[Chuyển động một chiều trong cơ học lượng tử|định lí nút]]).
- **Giếng đối xứng** (tâm ở gốc, $x \in [-a,a]$, bề rộng $2a$): mức chẵn $\psi_n \propto \cos\dfrac{n\pi x}{2a}$ ($n$ lẻ), mức lẻ $\psi_n \propto \sin\dfrac{n\pi x}{2a}$ ($n$ chẵn), năng lượng $E_n = \dfrac{n^2\pi^2\hbar^2}{8ma^2}$. Tính chẵn lẻ được dự đoán từ $V(x)=V(-x)$ — dời gốc tọa độ không đổi phổ.
- Giới hạn cổ điển: $\dfrac{\Delta E_n}{E_n} = \dfrac{2n+1}{n^2}\to 0$ khi $n$ lớn — phổ "liền" dần, khớp nguyên lí tương ứng.

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng với điều kiện biên $\psi(0)=\psi(L)=0$ (thế vô hạn ⟺ hàm sóng triệt tiêu tại biên).
- Công cụ toán: nghiệm tổng quát $A\sin kx + B\cos kx$, điều kiện biên cho lượng tử hóa $k_n = \dfrac{n\pi}{L}$; lượng giác.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: chấm lượng tử (quantum dot) bán dẫn — bước sóng phát quang phụ thuộc kích thước $L$ đúng tỉ lệ $\dfrac{1}{L^2}$; giếng lượng tử trong laser bán dẫn cũng là giếng hữu hạn tiến tới giới hạn này.
- Trường hợp không còn đúng: tường vô hạn là lí tưởng hóa — giếng thực luôn hữu hạn, cho hàm sóng "rỉ" ra ngoài ([[Giếng thế hữu hạn]]); với giếng kích thước cỡ nguyên tử, hiệu ứng khối lượng hiệu dụng và thế không còn thuần túy hình chữ nhật.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Chuyển động một chiều trong cơ học lượng tử]]
- [[Giếng thế hữu hạn]]
- [[Nghiệm dừng của phương trình Schrödinger]]
- [[Nguyên lý bất định Heisenberg]]

## Câu hỏi mở

- Thế vô hạn có vi phạm điều kiện liên tục của $\psi'$ không? (Tại tường, $\psi'$ gián đoạn nhảy vô hạn — hệ quả của bước thế vô hạn.)
- Vì sao $E \propto n^2$ nhưng dao động tử có $E \propto n$ — khác biệt do hình dạng thế nào? (So với [[Dao động tử điều hòa lượng tử]].)