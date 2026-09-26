---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Cơ học Lagrange

> [!abstract] Công cụ để làm gì
> Khung cơ học thay thế "lực" bằng "năng lượng": hệ chuyển động theo đường làm cực tiểu tác dụng $S = \int L\,dt$ với $L = T - V$ — các định luật Newton suy ra từ một hàm vô hướng duy nhất, bất biến khi chọn tọa độ.

## Định nghĩa

- **Tọa độ suy rộng:** bộ $q_1, q_2, ...$ tối thiểu đủ để xác định cấu hình hệ — có thể là góc, chiều dài dây, tọa độ cong... (không nhất thiết là Descartes).
- **Lagrangian:** $L(q, \dot q, t) = T - V$ (động năng trừ thế năng), với $\dot q$ là vận tốc suy rộng.
- **Tác dụng:** $S[q] = \int_{t_1}^{t_2} L(q, \dot q, t)\, dt$.
- **Phương trình Euler–Lagrange:**
  $\frac{\partial L}{\partial q_i} - \frac{d}{dt}\frac{\partial L}{\partial \dot q_i} = 0$
  là điều kiện để $S$ cực trị — phần thân của [[Phép tính biến phân]] và [[Nguyên lý tác dụng tối thiểu]].

## Ý nghĩa hình học

- Lagrangian là một hàm trên "không gian cấu hình" (mọi tư thế khả dĩ của hệ); quỹ đạo thực là đường làm cực trị tác dụng trong không gian đó.
- Sức mạnh nằm ở chỗ $L$ là **vô hướng**: đổi tọa độ thoải mái (quay, cong, trượt) mà phương trình chuyển động giữ nguyên dạng — luật vật lý không lệ thuộc "thước đo".

## Ý nghĩa vật lý

- Với $L = T - V$ trong tọa độ Descartes, Euler–Lagrange trả lại đúng $\vec F = m\vec a$ — xem [[Các định luật Newton]] và [[Định luật II Newton]].
- Chọn tọa độ suy rộng hợp lý (góc, chiều dài dây, v.v.) khiến bài toán có ràng buộc trở nên tự nhiên, không cần phân tích lực phản lực — ví dụ mẫu: [[Con lắc đơn]] (một tọa độ $\theta$), [[Con lắc lò xo]].
- **Đối xứng & bảo toàn:** $L$ không phụ thuộc $q$ (đối xứng dịch chuyển) ↔ động lượng suy rộng $\partial L / \partial \dot q$ bảo toàn; không phụ thuộc $t$ ↔ năng lượng bảo toàn — định lý [[Định lý Noether]].
- **Khuếch đại lên trường:** thay $L$ bằng mật độ Lagrangian $\mathcal{L}$, tác dụng là tích phân theo không-thời gian → phương trình trường (Schrödinger, Maxwell, QFT) — [[Lý thuyết trường lượng tử (QFT)]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Nguyên lý tác dụng tối thiểu]] — nền triết lý "tự nhiên chọn đường cực trị".
- [[Phép tính biến phân]] — công cụ toán để suy ra phương trình chuyển động.
- [[Định lý Noether]] — đối xứng của $L$ sinh lượng bảo toàn (năng lượng, động lượng).
- [[Con lắc đơn]] · [[Con lắc lò xo]] · [[Chuyển động quay của vật rắn]] — ví dụ tọa độ suy rộng trong thực tế.
- [[Lý thuyết trường lượng tử (QFT)]] — bản nâng cấp "trường" của cùng khung.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Nguyên lý tác dụng tối thiểu]] · [[Phép tính biến phân]] · [[Định lý Noether]] · [[Các định luật Newton]] · [[Lý thuyết nhóm]]

## Câu hỏi mở

- Mọi hệ vật lý có viết được dưới dạng Lagrangian không? (Ma sát cần $L$ dạng tổng quát hơn; cơ học lượng tử và trường dùng Lagrangian density — [[Lý thuyết trường lượng tử (QFT)]].)
- Nếu Newton và Lagrange mô tả cùng một hệ, lợi ích thực sự của Lagrange là gì ngoài "đẹp hơn"? (Gợi ý: quán tính—lực hư cấu biến mất khi dùng tọa độ phi quán tính; tiện cho hệ ràng buộc.)