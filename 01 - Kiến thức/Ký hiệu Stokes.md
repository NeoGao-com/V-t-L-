---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: quang-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Ký hiệu Stokes

> [!abstract] Ý chính
> Ký hiệu Stokes là bộ bốn số ($S_0, S_1, S_2, S_3$) mô tả trạng thái phân cực — **đo được trực tiếp bằng cường độ** qua các phép đo tích phân, xử lý được cả ánh sáng không phân cực và phân cực một phần (điều vector Jones không làm được).

## Nội dung

- **Định nghĩa bốn tham số Stokes:**
  - $S_0 = I$ — cường độ tổng.
  - $S_1 = I_0 - I_{90}$ — hiệu cường độ giữa hai hướng phân cực thẳng (0° và 90°).
  - $S_2 = I_{45} - I_{135}$ — hiệu cường độ giữa hai hướng phân cực chéo (+45° và −45°).
  - $S_3 = I_R - I_L$ — hiệu giữa cường độ phân cực tròn phải và tròn trái (cần thêm bản $\lambda/4$ trước bộ phân cực khi đo).
- **Độ phân cực:**
  $P = \dfrac{\sqrt{S_1^2 + S_2^2 + S_3^2}}{S_0}, \qquad 0 \le P \le 1$
  - $P = 1$: hoàn toàn phân cực; $P = 0$: không phân cực; $0 < P < 1$: phân cực một phần.

## Bảng: Stokes vector cho các trạng thái chuẩn

| Trạng thái | $(S_0, S_1, S_2, S_3)$ |
| --- | --- |
| Không phân cực | $(I, 0, 0, 0)$ |
| Thẳng trục x (0°) | $(I, I, 0, 0)$ |
| Thẳng trục y (90°) | $(I, -I, 0, 0)$ |
| Thẳng chéo 45° | $(I, 0, I, 0)$ |
| Tròn (một chiều) | $(I, 0, 0, \pm I)$ — dấu theo chiều quay |

## Ví dụ vật lý cụ thể

- **Đo phân cực kế thực tế:** quay bộ phân cực, chụp cường độ ở các góc: $S_1 = I_0 - I_{90}$, $S_2 = I_{45} - I_{135}$; đặt bản $\lambda/4$ trước đo được $S_3$. Từ đó suy ra $P$ và hướng phân cực — đây là nguyên lý mọi polarimeter.
- **Bầu trời:** ánh sáng tán xạ khí quyển phân cực một phần ($P$ cỡ 0,3–0,9 thay đổi theo hướng nhìn) — Stokes là cách chuẩn để đo và hiển thị bản đồ phân cực bầu trời (định hướng cho ong, robot, máy bay).
- **Phân cực CMB:** bản đồ nền vi sóng vũ trụ có hai mode phân cực E-mode và B-mode; đo Stokes rồi tách mode B (chỉ phát ra bởi sóng hấp dẫn nguyên thủy) — mục tiêu của các kính thiên văn vô tuyến thế hệ mới (liên hệ [[Nguyên lý Vũ trụ học]]).

## Suy luận từ đâu

- **Liên hệ với [[Ký hiệu Jones]]** (ánh sáng hoàn toàn phân cực, $\vec E = (E_x, E_y)$):
  $S_1 = |E_x|^2 - |E_y|^2,\quad S_2 = 2\operatorname{Re}(E_x E_y^*),\quad S_3 = i(E_x E_y^* - E_x^* E_y)$
  Stokes giữ **cường độ** (không pha tuyệt đối) nên xử lý được chùm hỗn hợp/không kết hợp — tổng quát hơn Jones.
- Định nghĩa qua phép đo cường độ (không cần detector nhạy pha) là lý do Stokes thống trị trong viễn thám và thiên văn.

## Kiểm chứng & giới hạn

- Kiểm chứng: phân cực kế cho kết quả khớp định luật Malus và khớp chuyển đổi Jones→Stokes với chùm laser phân cực hoàn toàn; CMB polarization đo bởi Planck/BICEP.
- **Giới hạn:** Stokes không chứa pha — không mô tả được hiệu ứng cần pha tuyệt đối (giao thoa kết hợp giữa hai chùm) → phải dùng vector Jones; dấu $S_3$ phụ thuộc quy ước chiều quay (phải/trái) — cần ghi rõ khi công bố.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Phân cực ánh sáng]]: tham số Stokes là một cách mô tả phân cực bên cạnh vector Jones.
- [[Ký hiệu Jones]]: giữ pha — bổ trợ cho Stokes khi cần kết hợp hai formalism.
- [[Giao thoa ánh sáng]]: phân cực ảnh hưởng đến hình ảnh giao thoa của nhiều nguồn.
- [[Nhiễu xạ ánh sáng]]: bộ phân cực trước detector giúp giảm nhiễu.
- [[Nguyên lý Vũ trụ học]]: mode B của phân cực CMB do sóng hấp dẫn nguyên thủy.

## Câu hỏi mở

- Vì sao trong viễn thám và thiên văn người ta thường dùng tham số Stokes hơn là vector Jones? (Gợi ý: Stokes đo bằng cường độ, không cần pha chính xác — dễ thực hiện với detector không đồng pha.)
- Mode B của phân cực CMB nếu xác nhận sẽ là bằng chứng trực tiếp của sóng hấp dẫn từ Vụ Nổ Lớn — nhưng nhiễu nền tiền thiên hà (foreground) làm phức tạp việc tách B-mode như thế nào trong thực tế?