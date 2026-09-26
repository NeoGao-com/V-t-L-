---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Giếng thế hữu hạn

> [!abstract] Ý chính
> Giếng thế hữu hạn độ sâu $V_0$ cho một số hữu hạn trạng thái liên kết, hàm sóng thoát ra vùng ngoài và khuếch giảm theo hàm mũ — đây là mô hình thực tế của giếng lượng tử trong vật liệu bán dẫn, đồng thời cho thấy trạng thái liên kết yếu luôn tồn tại trong 1D dù $V_0$ nhỏ tùy ý.

## Phát biểu / Định nghĩa

Thế năng: $V(x) = -V_0$ với $|x| < a$; $V(x) = 0$ với $|x| > a$ ($V_0 > 0$). Có hữu hạn trạng thái liên kết $E < 0$.

Trong giếng ($|x|<a$): $\psi'' + k^2\psi = 0$, $\;k = \dfrac{\sqrt{2m(E+V_0)}}{\hbar}$
Ngoài giếng ($|x|>a$): $\psi'' - \kappa^2\psi = 0$, $\;\kappa = \dfrac{\sqrt{2m(-E)}}{\hbar}$ (khuếch giảm: $\psi \propto e^{-\kappa|x|}$).

Điều kiện liên tục của $\psi$ và $\psi'$ tại $x = \pm a$ cho hai phương trình siêu việt (với $ka$, $\kappa a$ là các đại lượng không thứ nguyên):

- Mức **chẵn**: $\tan(ka) = \dfrac{\kappa}{k}$
- Mức **lẻ**: $\cot(ka) = -\dfrac{\kappa}{k}$

Giải bằng đồ thị: giao điểm của các nhánh tang/côtang với đường tròn $k^2 + \kappa^2 = \dfrac{2mV_0}{\hbar^2}$.

**Kết quả chính:**

1. **Luôn có ít nhất một trạng thái liên kết** trong 1D với $V_0 > 0$ bất kỳ (mức chẵn thấp nhất tồn tại với mọi $V_0$). Mức lẻ đầu tiên xuất hiện khi $ka \ge \dfrac{\pi}{2}$, tức $V_0 \ge \dfrac{\pi^2\hbar^2}{8ma^2}$.
2. Số trạng thái hữu hạn; khi $V_0 \to \infty$ tái tạo [[Giếng thế vô hạn]]: $k\to\dfrac{n\pi}{2a}$, $E_n \to \dfrac{n^2\pi^2\hbar^2}{8ma^2}$.
3. Số nút vẫn theo định lí nút; tính chẵn lẻ xen kẽ từ mức dưới cùng (thế đối xứng).
4. Hàm sóng thâm nhập vùng cấm với độ sâu $1/\kappa$; xác suất ngoài giếng giảm khi $V_0$ tăng.

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng + điều kiện nối tiếp (khớp $\psi$, $\psi'$ tại biên) — nguyên tắc của [[Chuyển động một chiều trong cơ học lượng tử]].
- Công cụ toán: phương trình vi phân tuyến tính, hàm lượng giác và siêu việt, giải phương trình nghiệm bằng đồ thị.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: giếng lượng tử GaAs/AlGaAs — số mức liên kết và năng lượng suy từ quang phổ hấp thụ phù hợp phương trình siêu việt; trạng thái bề mặt và mức bẫy trong kim loại/bán dẫn cũng là nghiệm kiểu giếng hữu hạn.
- Trường hợp không còn đúng: giếng nhiều lớp hay thế biến đổi trơn cần giải số (phương pháp truyền ma trận chuyển); với $V_0$ quá nhỏ so với $\dfrac{\hbar^2}{2ma^2}$ chỉ còn một mức sát 0.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Giếng thế vô hạn]]
- [[Chuyển động một chiều trong cơ học lượng tử]]
- [[Thế bậc thang]]
- [[Hàng rào thế và hiệu ứng đường ngầm]]

## Câu hỏi mở

- Khi $V_0$ tăng dần, thứ tự các mức chẵn và lẻ chuyển hóa về giếng vô hạn thế nào — và vì sao mức lẻ "sinh sau"?
- Giếng hữu hạn đối xứng và bất đối xứng ($V(x)$ khác nhau hai bên) khác nhau ra sao về số mức liên kết? (Bất đối xứng không còn tính chẵn lẻ.)