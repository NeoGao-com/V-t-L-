---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Nghiệm dừng của phương trình Schrödinger

> [!abstract] Ý chính
> Khi thế năng không phụ thuộc thời gian, phương trình Schrödinger có các nghiệm riêng dạng $\Psi_n(\vec r,t) = \psi_n(\vec r)e^{-iE_n t/\hbar}$ với phổ năng lượng thực, trực giao và mọi trạng thái khác là chồng chập của các nghiệm dừng này.

## Phát biểu / Định nghĩa

Nghiệm dừng sinh ra từ phép tách biến $\Psi(\vec r,t) = \psi(\vec r)\,T(t)$:

- Phương trình theo thời gian: $T(t) = e^{-iEt/\hbar}$, chỉ phụ thuộc năng lượng.
- Phương trình không phụ thuộc thời gian: $\hat H\psi_n(\vec r) = E_n\psi_n(\vec r)$ (xem [[Phương trình Schrödinger]]).

**Tính chất cơ bản của hệ nghiệm dừng:**

1. **Năng lượng thực:** $\hat H$ là toán tử Hermit nên $E_n\in\mathbb R$; nghiệm dừng tồn tại cho mọi thời gian mà không phai.
2. **Trạng thái dừng:** mật độ $|\Psi_n|^2 = |\psi_n|^2$ không đổi theo thời gian; trị trung bình của mọi đại lượng không phụ thuộc thời gian $\langle\hat A\rangle$ là hằng số.
3. **Trực giao:** $\langle\psi_m|\psi_n\rangle = \delta_{mn}$ với các mức khác nhau ($E_m\neq E_n$); các mức suy biến có thể trực giao hóa theo Gram–Schmidt.
4. **Đầy đủ:** nghiệm tổng quát là chồng chập tuyến tính $\Psi(\vec r,t) = \sum_n c_n\psi_n(\vec r)e^{-iE_n t/\hbar}$, với $c_n = \langle\psi_n|\Psi(\vec r,0)\rangle$ xác định bởi trạng thái ban đầu — hệ quả của [[Nguyên lý chồng chất lượng tử]].
5. **Phổ:** trạng thái liên kết ($E < V(\infty)$) cho phổ gián đoạn, trạng thái tán xạ cho phổ liên tục; tổng có thể chuyển thành tích phân.

## Suy luận từ đâu

- Tiên đề gốc: tiên đề tiến hóa (Schrödinger) và tính Hermit của toán tử quan sát trong [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]].
- Công cụ toán: bài toán trị riêng của toán tử Hermit trong [[Không gian Hilbert]] — định lí phổ, trực giao và đầy đủ của hệ hàm riêng.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: mức năng lượng gián đoạn của nguyên tử qua [[Quang phổ]] vạch; [[Thí nghiệm - Franck-Hertz]] chứng minh các mức dừng tồn tại và chỉ hấp thụ đúng lượng tử năng lượng.
- Trường hợp không còn đúng: khi $\hat H$ phụ thuộc thời gian (thế biến thiên) không tồn tại nghiệm dừng — cần dùng lý thuyết nhiễu loạn phụ thuộc thời gian; chồng chập của hai mức suy biến có thể cho trạng thái có $\langle\hat A\rangle$ dao động (không "dừng" theo nghĩa thường).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Phương trình Schrödinger]]
- [[Trạng thái lượng tử]]
- [[Phép đo lượng tử]]
- [[Không gian Hilbert]]
- [[Nguyên lý chồng chất lượng tử]]

## Câu hỏi mở

- Vì sao trạng thái dừng "dừng" trong khi năng lượng của hạt vẫn xác định — mâu thuẫn với dao động không? (Vì xác suất và trị trung bình không đổi, không phải tọa độ hạt đứng yên.)
- Tại sao mức suy biến cần trực giao hóa lại — và khi nào khối (block) suy biến không thể tách?