---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Phương trình Schrödinger

> [!abstract] Ý chính
> Phương trình nền tảng của cơ học lượng tử phi tương đối tính — mô tả hàm sóng $\Psi$ tiến triển theo thời gian dưới tác dụng của toán tử Hamilton $\hat H$. Vai trò của nó với cơ học lượng tử giống như $\vec F = m\vec a$ với cơ học cổ điển: mọi hệ lượng tử đều tuân theo.

## Nội dung

- **Phương trình phụ thuộc thời gian:**
  $i\hbar \dfrac{\partial}{\partial t}\Psi(x,t) = \hat{H}\Psi(x,t)$
  với $\hat{H} = -\dfrac{\hbar^2}{2m}\nabla^2 + V(x)$ (động năng + thế năng).
- **Phương trình không phụ thuộc thời gian (trạng thái dừng):**
  $\hat{H}\psi_n(x) = E_n\psi_n(x)$
  - $\psi_n$ là hàm riêng của năng lượng, $E_n$ là trị riêng năng lượng — đây là một bài toán trị riêng của [[Đại số tuyến tính]].
- **Quan sát quan trọng:**
  - $|\Psi(x,t)|^2$ là mật độ xác suất tìm thấy hạt tại $x$ ở thời điểm $t$ (quy tắc Born).
  - Phương trình **tuyến tính** → nghiệm chồng chất được (xem [[Nguyên lý chồng chất lượng tử]]).
  - Bất định Heisenberg $\Delta x \Delta p \ge \hbar/2$ là hệ quả của cấu trúc toán tử.
  - Về mặt toán, đây là một [[Phương trình đạo hàm riêng (PDE)]]: bậc nhất theo thời gian, bậc hai theo tọa độ; phương trình dừng là bài toán trị riêng elliptic.

## Suy luận từ đâu

- Tiên đề gốc: tiên đề tiến hóa trong [[Tiên đề cơ học lượng tử]] — $\hat H$ là toán tử Hamilton, nghiệm dừng là bài toán trị riêng của toán tử Hermit (xem [[Trạng thái lượng tử]]).
- Công cụ toán: giải tích (đạo hàm, toán tử $\nabla$), [[Đại số tuyến tính]] cho bài toán trị riêng, [[Phương trình đạo hàm riêng (PDE)]] cho cấu trúc phương trình.

## Bảng các hệ giải được chính xác

| Hệ | Thế năng $V(x)$ | Mức năng lượng $E_n$ | Hàm sóng đặc trưng |
| --- | --- | --- | --- |
| Hố thế vô hạn | $0$ trong $[0, L]$ | $\dfrac{n^2h^2}{8mL^2}$ | $\sin\dfrac{n\pi x}{L}$ |
| Dao động tử điều hòa | $\frac{1}{2}m\omega^2x^2$ | $\hbar\omega\left(n + \frac{1}{2}\right)$ | Đa thức Hermite × gaussian |
| Nguyên tử hydro | $-\dfrac{ke^2}{r}$ | $-\dfrac{13{,}6}{n^2}$ eV | Đa thức Laguerre × $e^{-r/a_0}$ |

Điểm chung: **lượng tử hóa năng lượng tự động xuất hiện** từ điều kiện biên/chuẩn hóa — không cần giả định thêm như mẫu Bohr.

## Ví dụ vật lý cụ thể

- **Electron trong hố thế $L = 1$ nm:** $E_1 \approx 0{,}38$ eV; $E_4 = 16E_1 \approx 6{,}0$ eV. Hố càng nhỏ, năng lượng càng cao — giải thích vì sao chấm lượng tử (quantum dot) đổi màu phát quang theo kích thước.
- **Dao động tử:** mức thấp nhất $E_0 = \frac{1}{2}\hbar\omega$ khác 0 — "năng lượng điểm không" (zero-point energy), nguồn gốc dao động của mạng tinh thể (phonon) và hiệu ứng Casimir.
- **Nguyên tử hydro:** dự đoán $E_n = -13{,}6/n^2$ eV khớp với quang phổ vạch hydro (dãy Lyman, Balmer) tới ~8 chữ số — thành công đầu tiên của cơ học lượng tử.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: quang phổ hydro, hiệu ứng xuyên hầm (tunnel) trong [[Phóng xạ]] alpha và diode đường hầm, chấm lượng tử.
- Trường hợp không còn đúng: hạt nhanh ($v \sim c$) cần phương trình Dirac (kết hợp tương đối hẹp); số hạt thay đổi cần lý thuyết trường lượng tử.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Tiên đề cơ học lượng tử]]: note mẹ chứa bộ tiên đề và bài giải chi tiết.
- [[Nguyên lý chồng chất lượng tử]]: tính tuyến tính của phương trình cho phép chồng chất nghiệm.
- [[Nguyên lý bất định Heisenberg]]: giới hạn đo lường lượng tử.
- [[Mẫu nguyên tử Bohr]]: mức năng lượng là trị riêng $E_n$ của các trạng thái riêng $\psi_n$ — Bohr chỉ là trường hợp gần đúng.
- [[Cơ học Hamilton]]: toán tử $\hat H$ là Hamiltonian cổ điển được lượng tử hóa — cầu nối trực tiếp từ cơ học cổ điển.
- [[Phương trình đạo hàm riêng (PDE)]]: cấu trúc toán học của phương trình.
- [[Mật độ dòng xác suất]]: bảo toàn xác suất suy ra từ phương trình.
- [[Nghiệm dừng của phương trình Schrödinger]]: tính chất của các nghiệm riêng.
- [[Chuyển động một chiều trong cơ học lượng tử]]: khung chung cho các bài toán 1D (giếng thế, bậc thang, hàng rào, dao động tử).
- [[Tách biến trong phương trình Schrödinger ba chiều]]: chuyển bài toán 3D về ba bài toán 1D.

## Câu hỏi mở

- Vì sao phương trình dùng hệ số $i$ (số thuần ảo) — hàm sóng bắt buộc phải phức? Có thể xây dựng cơ học lượng tử với hàm sóng thực thuần túy không?
- "Sụp đổ hàm sóng" $\Psi \to \psi_n$ khi đo lường diễn ra thế nào, nếu phương trình tiến hóa là tất định? (Bài toán đo lường — chưa có lời giải thống nhất.)
- Thay $i\hbar\partial_t$ bằng đạo hàm bậc hai theo thời gian (như sóng cổ điển) thì thu được gì? — phương trình Klein–Gordon, tiên đoán phản hạt, nhưng cũng sinh nghiệm năng lượng âm bất thường.