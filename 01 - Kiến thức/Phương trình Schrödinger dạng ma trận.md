---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Phương trình Schrödinger dạng ma trận

> [!abstract] Ý chính
> Chiếu phương trình Schrödinger lên một cơ sở, nó trở thành hệ phương trình vi phân tuyến tính ma trận $i\hbar\dot{\vec c} = H\vec c$ với nghiệm $c(t) = e^{-iHt/\hbar}c(0)$ — toán tử tiến hóa là mũ ma trận unita, và "chéo hóa H" giải trọn bài toán tiến hóa.

## Phát biểu / Định nghĩa

**6. Dạng ma trận của phương trình Schrödinger:**

Trong cơ sở trực chuẩn $\{|n\rangle\}$ với $|\Psi(t)\rangle = \sum_n c_n(t)|n\rangle$ (xem [[Biểu diễn các trạng thái lượng tử]]), phương trình Schrödinger $i\hbar\partial_t|\Psi\rangle = \hat H|\Psi\rangle$ trở thành hệ $N$ (vô hạn) phương trình vi phân tuyến tính:

$i\hbar\,\dfrac{dc_n}{dt} = \sum_m H_{nm}\,c_m(t), \qquad$ viết gọn: $i\hbar\,\dot{\vec c} = H\,\vec c$

với $H_{nm} = \langle n|\hat H|m\rangle$ ([[Biểu diễn ma trận của toán tử]]).

**Nghiệm hình thức:**

$\vec c(t) = U(t)\,\vec c(0), \qquad U(t) = e^{-iHt/\hbar} = \sum_{k=0}^{\infty}\dfrac{(-it/\hbar)^k}{k!}H^k$

- $U(t)$ là **mũ ma trận**: unita ($U^\dagger U = I$), nhóm một tham số $U(t_1)U(t_2) = U(t_1+t_2)$, liên hệ [[Nghiệm dừng của phương trình Schrödinger|toán tử tiến hóa]].
- Chuẩn được bảo toàn: $\|c(t)\|^2 = \|c(0)\|^2$ — xác suất tổng bằng 1 ([[Mật độ dòng xác suất]]).
- **Trong cơ sở năng lượng** ($H_{nm} = E_n\delta_{nm}$): hệ tách rời từng phương trình, $c_n(t) = c_n(0)e^{-iE_nt/\hbar}$ — mỗi hệ số quay pha với tần số góc $\omega_n = E_n/\hbar$ (bổ đề pha thời gian).

**7. Dạng ma trận của phương trình Heisenberg** (tham chiếu — xem chi tiết ở [[Biểu diễn Schrödinger, Heisenberg và tương tác]] và [[Đạo hàm của toán tử theo thời gian]]):

$i\hbar\,\dfrac{dF_{nm}}{dt} = \sum_k\left(F_{nk}H_{km} - H_{nk}F_{km}\right) + i\hbar\,\dfrac{\partial F_{nm}}{\partial t}, \qquad$ tức $i\hbar\,\dot F = [F,H] + i\hbar\,\dfrac{\partial F}{\partial t}$

— dạng ma trận của giao hoán tử; đối xứng về vai trò: Schrödinger quay vector trạng thái, Heisenberg quay ma trận toán tử.

## Suy luận từ đâu

- Tiên đề gốc: tiên đề tiến hóa (A5) — [[Phương trình Schrödinger]]; tính Hermit của $\hat H$ cho $U$ unita.
- Công cụ toán: [[Đại số tuyến tính]] (ma trận, mũ ma trận), hệ ODE tuyến tính ([[Phương trình vi phân]]), [[Biểu diễn ma trận của toán tử]].

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: mọi mô phỏng động lực lượng tử số (mạch lượng tử, phân tử trong xung laser, các vấn đề nhiều mức) đều tích phân trực tiếp $i\hbar\dot{c} = Hc$ trên ma trận hữu hạn — độ chính xác so với đo phổ/thời gian sống khớp nhau.
- Trường hợp không còn đúng: cơ sở hữu hạn không đủ cho phổ liên tục (tán xạ) — cần không gian hàm; khi $\hat H$ phụ thuộc thời gian, $U(t)$ không là mũ đơn giản (chuỗi Dyson sắp thứ tự thời gian); hệ mở cần phương trình Lindblad (ma trận mật độ, không phải vector).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Biểu diễn ma trận của toán tử]]
- [[Biểu diễn các trạng thái lượng tử]]
- [[Sự chuyển biểu diễn và phép biến đổi unita]]
- [[Phương trình Schrödinger]]
- [[Đại số tuyến tính]]

## Câu hỏi mở

- Vì sao $e^{-iHt/\hbar}$ lại là chuỗi lũy thừa của $H$ — và khi nào chuỗi hội tụ chậm (cần thuật toán khác: Krylov, Trotter–Suzuki)?
- Nếu $\hat H$ không Hermit (hệ tiêu tán hiệu quả), $U(t)$ mất tính unita — chuẩn giảm mô tả hiện tượng gì? (Phân rã, tuổi thọ mức.)