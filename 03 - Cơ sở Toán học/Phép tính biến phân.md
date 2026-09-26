---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Phép tính biến phân

> [!abstract] Công cụ để làm gì
> Phép tính biến phân tìm **hàm số** làm cực trị một tích phân — thay vì tìm điểm $x$ làm cực trị một hàm số (đạo hàm thường). Đây là ngôn ngữ của các "nguyên lý cực trị" trong vật lý: tự nhiên chọn con đường làm cực tiểu (hoặc cực đại) một đại lượng.

## Định nghĩa

Bài toán: tìm hàm $q(t)$ làm cực trị phiếm hàm $S[q] = \int_{t_1}^{t_2} L(q, \dot q, t)\, dt$.

- **Biến phân:** thay $q(t)$ bằng $q(t) + \varepsilon \eta(t)$ (với $\eta$ triệt tiêu ở biên) và đòi hỏi $\dfrac{dS}{d\varepsilon}\big|_{\varepsilon = 0} = 0$.
- Nghiệm thỏa **phương trình Euler–Lagrange**:
  $\dfrac{\partial L}{\partial q} - \dfrac{d}{dt}\dfrac{\partial L}{\partial \dot q} = 0$

## Ý nghĩa hình học

- Đạo hàm thường tìm điểm cực trị trên **đường cong** (đạo hàm bằng 0); biến phân tìm **đường đi cực trị trong "không gian các đường đi"** — quanh đường làm cực trị, mọi nhiễu loạn nhỏ đều không đổi $S$ ở bậc nhất.
- Trực giác "nước chảy xuống dốc": đạo hàm thường là tìm đáy thung lũng; biến phân là tìm lòng suối — đường mà nước chọn giữa vô số đường có thể.

## Ý nghĩa vật lý

- **Nguyên lý Fermat:** ánh sáng chọn đường đi mất ít thời gian nhất → định luật khúc xạ Snell và [[Phản xạ toàn phần]] là hệ quả trực tiếp của cùng một nguyên lý ([[Nguyên lý Fermat]], [[Khúc xạ ánh sáng]]).
- **Nguyên lý tác dụng tối thiểu:** với $L = T - V$, Euler–Lagrange suy ra đúng các định luật Newton — cơ học "sinh ra" từ một đại lượng vô hướng duy nhất ([[Nguyên lý tác dụng tối thiểu]], [[Cơ học Lagrange]], [[Các định luật Newton]]).
- **Nguyên lý Huygens:** mỗi điểm trên mặt sóng là nguồn sóng cầu — cách nói khác của "sóng chọn đường tự nhiên nhất" ([[Nguyên lý Huygens]]).
- **Đối xứng & bảo toàn:** đối xứng liên tục của $L$ kéo theo lượng bảo toàn (dịch thời gian → năng lượng; dịch không gian → động lượng; quay → mô-men động lượng) — định lý [[Định lý Noether]].
- **Mở rộng:** cực tiểu "đường đi" giữa hai điểm trong không-thời gian cong cho quỹ đạo trắc địa — con đường của thuyết tương đối rộng.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Nguyên lý Fermat]] · [[Khúc xạ ánh sáng]] · [[Phản xạ toàn phần]]: định luật khúc xạ là hệ quả của cực trị thời gian truyền.
- [[Nguyên lý tác dụng tối thiểu]] · [[Cơ học Lagrange]]: Euler–Lagrange là trường hợp đặc biệt khi $L = T - V$.
- [[Định lý Noether]]: đối xứng của tác dụng sinh định luật bảo toàn.
- [[Thuyết tương đối rộng]]: trắc địa = cực trị tác dụng trong không-thời gian cong.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Đạo hàm]] · [[Tích phân]] · [[Cơ học Lagrange]] · [[Nguyên lý Fermat]] · [[Nguyên lý tác dụng tối thiểu]] · [[Định lý Noether]] · [[Thuyết tương đối rộng]]

## Câu hỏi mở

- Vì sao phép tính này thường cho nghiệm duy nhất cho một bài toán vật lý, trong khi cơ học Newton chỉ cho $\vec F = m\vec a$? (Gợi ý: nguyên lý tổng quát hơn — định luật Newton là hệ quả khi $L = T - V$.)
- Giới hạn của khung biến phân là gì? (Ma sát, lực không bảo toàn, hệ có $\ddot q$ — Lagrangian cần dạng tổng quát hơn hoặc phải xử lý riêng.)