---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Đạo hàm

> [!abstract] Công cụ để làm gì
> Đạo hàm là "máy đo tốc độ biến thiên" — thứ ngôn ngữ vật lý dùng để diễn đạt mọi đại lượng tức thời: vận tốc, gia tốc, dòng điện, công suất, tốc độ phân rã... Đạo hàm biến câu chuyện "tổng cộng lại" thành câu chuyện "ngay lúc này".

## Định nghĩa

Đạo hàm của hàm $f(x)$ tại $x$ là giới hạn của tỉ số sai phân khi khoảng cách tiến về 0:

$f'(x) = \lim_{\Delta x \to 0} \dfrac{f(x + \Delta x) - f(x)}{\Delta x}$

- **Đạo hàm riêng:** $\dfrac{\partial f}{\partial x}$ — lấy đạo hàm theo một biến, giữ các biến khác cố định; là viên gạch của gradient, div, curl ([[Giải tích Vector (Grad, Div, Curl)]]) và của nhiệt động lực học.
- **Đạo hàm bậc hai:** $f''(x)$ — tốc độ biến thiên của tốc độ biến thiên (gia tốc, độ cong của đồ thị).
- **Quy tắc chuỗi:** $\dfrac{df}{dt} = \dfrac{df}{dx}\dfrac{dx}{dt}$ — công cụ đổi biến thường trực trong vật lý.

## Ý nghĩa hình học

- $f'(x)$ là **hệ số góc của tiếp tuyến** với đồ thị tại $x$ — độ dốc của "con dốc" tại đúng điểm đó.
- $f''(x)$ nói đồ thị đang "cong lên" hay "cong xuống".

## Ý nghĩa vật lý

- $v = \dfrac{dx}{dt}$ — vận tốc là đạo hàm của vị trí theo thời gian; $a = \dfrac{dv}{dt}$ — gia tốc là đạo hàm của vận tốc ([[Chuyển động thẳng biến đổi đều]], [[Rơi tự do]]).
- $i = \dfrac{dq}{dt}$ — dòng điện là đạo hàm của điện tích dịch chuyển ([[Mạch điện và các phần tử mạch]], [[Tụ điện]]); $P = \dfrac{dW}{dt}$ — công suất tức thời là đạo hàm của công theo thời gian ([[Công và công suất]]).
- **Dao động:** $x = A\cos(\omega t + \varphi)$ → $v$, $a$ lần lượt là đạo hàm bậc một, bậc hai; đạo hàm bậc hai trả về $a = -\omega^2 x$ — mọi dao động được điều khiển bởi phương trình vi phân này ([[Dao động điều hòa]], [[Con lắc lò xo]]).
- **Phân rã:** tốc độ phân rã $-\dfrac{dN}{dt} = \lambda N$ — đạo hàm xuất hiện trong định luật suy giảm phóng xạ ([[Phóng xạ]]).
- **Trường từ thế:** $\vec E = -\nabla V$ — điện trường là (âm) gradient của điện thế, tức họ các đạo hàm riêng ([[Điện thế và hiệu điện thế]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Các định luật Newton]] · [[Định luật II Newton]]: định luật II dạng vi phân $\vec F = m\dfrac{d\vec v}{dt}$.
- [[Dao động điều hòa]] · [[Con lắc lò xo]]: đạo hàm bậc hai quyết định đặc trưng dao động.
- [[Phóng xạ]]: tốc độ phân rã tuân theo phương trình vi phân bậc nhất.
- [[Giải tích Vector (Grad, Div, Curl)]] · [[Phương trình Maxwell]]: đạo hàm riêng là ngôn ngữ của trường.
- [[Công và công suất]] · [[Tụ điện]] · [[Mạch RLC và trở kháng]]: đại lượng tức thời = đạo hàm theo thời gian.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Tích phân]] (phép toán ngược) · [[Phương trình vi phân]] · [[Giải tích Vector (Grad, Div, Curl)]] · [[Định luật II Newton]]

## Câu hỏi mở

- Đạo hàm còn ý nghĩa gì khi chuyển động gián đoạn (va chạm, hấp thụ photon)? (Gợi ý: hàm không khả vi — cần khái niệm suy rộng như phân bố, hàm Dirac delta; liên hệ [[Tiên đề cơ học lượng tử]].)
- Vì sao các định luật vật lý cơ bản đều viết bằng đạo hàm (theo thời gian hoặc không gian) chứ không bằng sai phân? (Gợi ý: tính địa phương và bất biến của luật vật lý.)