---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: cơ-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Con lắc kép

> [!abstract] Ý chính
> Hai con lắc nối tiếp nhau tạo ra chuyển động **tuần hoàn về cấu trúc nhưng không bao giờ lặp lại**: một hệ cơ học cổ điển thuần túy (chỉ cần định luật Newton) lại không thể dự báo lâu dài. Đây là ví dụ hiện hình dễ làm nhất của **hỗn loạn quyết định (deterministic chaos)**.

## Phát biểu / Định nghĩa

Con lắc kép gồm con lắc khối lượng $m_1$, chiều dài $l_1$, treo khối lượng $m_2$ bằng thanh $l_2$ ở đầu dưới. Hai góc lệch $\theta_1, \theta_2$ tạo thành hệ hai bậc tự do; Lagrangian:

$L = \frac{1}{2}(m_1+m_2)l_1^2\dot\theta_1^2 + \frac{1}{2}m_2 l_2^2 \dot\theta_2^2 + m_2 l_1 l_2 \dot\theta_1\dot\theta_2\cos(\theta_1-\theta_2) + (m_1+m_2)gl_1\cos\theta_1 + m_2gl_2\cos\theta_2$

Phương trình chuyển động (hai ODE phi tuyến, ràng buộc chặt vào nhau):

$(m_1+m_2)\,l_1\,\ddot\theta_1 + m_2\,l_2\,\ddot\theta_2\cos(\theta_1-\theta_2) + m_2\,l_2\,\dot\theta_2^2\sin(\theta_1-\theta_2) + (m_1+m_2)\,g\sin\theta_1 = 0$

$m_2\,l_2\,\ddot\theta_2 + m_2\,l_1\,\ddot\theta_1\cos(\theta_1-\theta_2) - m_2\,l_1\,\dot\theta_1^2\sin(\theta_1-\theta_2) + m_2\,g\sin\theta_2 = 0$

Khác với [[Dao động điều hòa|con lắc đơn]] (tuyến tính hóa được), phương trình này **không có nghiệm tổng quát kín** và cực kỳ nhạy với điều kiện đầu: khác biệt $10^{-6}$ rad ở $\theta_1$ phóng đại theo cấp số nhân theo thời gian (số mũ Lyapunov dương) → sau vài chu kỳ, hai quỹ đạo không còn tương quan.

## Suy luận từ đâu

- Tiên đề gốc: [[Các định luật Newton]] — không cần giả định gì ngoài cơ học cổ điển.
- Công cụ toán: tọa độ suy rộng & phương trình Euler–Lagrange — xem [[Cơ học Lagrange]], [[Phương trình vi phân]].
- Họ hàng gần: [[Hỗn loạn lượng tử (Quantum chaos)]] — cùng hiện tượng "sai số phóng đại", nhưng bên kia là cơ học cổ điển.

## Kiểm chứng & giới hạn

- **Thực nghiệm dễ lặp lại:** con lắc kép thật (hoặc mô phỏng số) luôn cho quỹ đạo đổi mới không hồi quy — đối chiếu trực tiếp với dự đoán số.
- **Giới hạn:** với biên độ nhỏ, hệ tuyến tính hóa về dao động điều hòa thường (không hỗn loạn); hỗn loạn chỉ xuất hiện ở năng lượng đủ lớn. Hỗn loạn ≠ ngẫu nhiên — hệ vẫn **quyết định**: dựa cùng điều kiện đầu, kết quả lặp lại y hệt.
- Vì nhạy cảm cực độ, dự báo dài hạn bằng số là bất khả thi về thực hành (cần độ chính xác vượt mọi phép đo) — nguồn gốc "giới hạn khả dự báo" của cơ học cổ điển, chứ không phải cơ học lượng tử mới có.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Dao động điều hòa]] · [[Cơ năng]] · [[Hỗn loạn lượng tử (Quantum chaos)]] · [[Thí nghiệm - Con lắc Foucault]] · [[Cơ học Lagrange]]

## Câu hỏi mở

- Số mũ Lyapunov của hệ phụ thuộc tỷ số $m_2/m_1$ và $l_2/l_1$ thế nào? Vùng tham số nào làm hệ "quay lại" hành vi tuần hoàn?
- Liên hệ chính xác với [[Hỗn loạn lượng tử (Quantum chaos)]] qua tham số nào — hay chỉ là phép loại suy?