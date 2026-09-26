---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: quang-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Ký hiệu Jones

> [!abstract] Ý chính
> Ký hiệu Jones (Jones calculus) biểu diễn trạng thái phân cực bằng vector hai thành phần phức và thấu kính/linh kiện bằng ma trận 2×2 — công cụ tuyến tính mạnh cho hệ quang học nhiều tầng, giữ đầy đủ thông tin pha (khác [[Ký hiệu Stokes]]).

## Nội dung

- **Vector Jones:** $\vec E = \begin{pmatrix} E_x \\ E_y \end{pmatrix}$ với $E_x, E_y$ là biên độ **phức** (chứa cả pha) của hai thành phần điện trường. Cường độ $I = |E_x|^2 + |E_y|^2$ (thường chuẩn hóa $I = 1$).
- **Ma trận Jones:** mỗi linh kiện (kính phân cực, bản bước sóng, bộ quay) là ma trận 2×2; ánh sáng ra: $\vec E_{out} = M\,\vec E_{in}$.
- **Hệ nhiều linh kiện:** nhân ma trận **từ phải sang trái** theo thứ tự ánh sáng đi qua:
  $\vec E_{out} = M_3\, M_2\, M_1\, \vec E_{in}$

## Bảng các vector và ma trận thường dùng

| Linh kiện / trạng thái | Biểu diễn Jones |
| --- | --- |
| Phân cực thẳng trục x | $\begin{pmatrix} 1 \\ 0 \end{pmatrix}$ |
| Phân cực thẳng trục y | $\begin{pmatrix} 0 \\ 1 \end{pmatrix}$ |
| Phân cực thẳng góc $\theta$ | $\begin{pmatrix} \cos\theta \\ \sin\theta \end{pmatrix}$ |
| Phân cực tròn (quy ước $+i$) | $\frac{1}{\sqrt2}\begin{pmatrix} 1 \\ \pm i \end{pmatrix}$ |
| Kính phân cực trục x | $\begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix}$ |
| Bản $\lambda/2$ (trục x) | $\begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$ |
| Bản $\lambda/4$ (trục x) | $\begin{pmatrix} 1 & 0 \\ 0 & i \end{pmatrix}$ (hoặc $-i$ — tùy quy ước) |
| Bộ quay góc $\theta$ | $R(\theta) = \begin{pmatrix} \cos\theta & -\sin\theta \\ \sin\theta & \cos\theta \end{pmatrix}$ |

## Ví dụ vật lý cụ thể

- **Tạo phân cực tròn:** ánh sáng qua kính phân cực 45° → $\vec E_{in} = \frac{1}{\sqrt2}\binom{1}{1}$; qua bản $\lambda/4$ trục x:
  $\begin{pmatrix} 1 & 0 \\ 0 & i \end{pmatrix} \frac{1}{\sqrt2}\binom{1}{1} = \frac{1}{\sqrt2}\binom{1}{i}$
  → phân cực tròn (dấu pha $i$ quyết định chiều quay).
- **Bản $\lambda/2$ xoay hướng phân cực:** với phân cực thẳng làm góc $\theta$ so với trục nhanh, bản $\lambda/2$ quay hướng đi **$2\theta$** — dùng để điều khiển không phụ thuộc hướng đầu vào (ví dụ khóa laser).
- **Kiểm tra hai kính chéo nhau bằng Jones:** $M_{90} M_0 = \begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix}\begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix} = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$ — ma trận không → không có ánh sáng ra, đúng Malus với $\theta = 90°$.

## Suy luận từ đâu

- Là ứng dụng trực tiếp của đại số tuyến tính ([[Đại số tuyến tính]]): trạng thái = vector, linh kiện = toán tử, hợp hệ = tích ma trận — cùng tinh thần với ma trận trong cơ học lượng tử (xem [[Tiên đề cơ học lượng tử]]).
- Liên hệ [[Ký hiệu Stokes]] (với ánh sáng hoàn toàn phân cực):
  $S_0 = |E_x|^2 + |E_y|^2,\qquad S_1 = |E_x|^2 - |E_y|^2$
  $S_2 = E_x E_y^* + E_x^* E_y = 2\operatorname{Re}(E_x E_y^*),\qquad S_3 = i\big(E_x E_y^* - E_x^* E_y\big)$

## Kiểm chứng & giới hạn

- Kiểm chứng: mọi hệ phân cực tuyến tính (polarizer, bản bước sóng, màng mỏng) đo bằng phép nhân ma trận đều khớp thực nghiệm.
- **Giới hạn:** Jones chỉ mô tả ánh sáng **hoàn toàn phân cực** — không xử lý được ánh sáng không phân cực/ phân cực một phần (ánh sáng Mặt Trời, bầu trời); khi đó phải dùng [[Ký hiệu Stokes]] (ma trận Mueller 4×4).
- Ma trận pha phụ thuộc quy ước dấu (trục nhanh/chậm, chiều tròn phải/trái) — phải ghi rõ quy ước khi dùng.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Phân cực ánh sáng]]: ký hiệu Jones là công cụ toán học để mô tả phân cực.
- [[Giao thoa ánh sáng]]: phân cực ảnh hưởng đến hình ảnh giao thoa.
- [[Ký hiệu Stokes]]: dùng khi chỉ cần độ phân cực, không cần pha — bổ trợ cho Jones trong đo lường.
- [[Đại số tuyến tính]]: ma trận là nền tảng của phép tính Jones.

## Câu hỏi mở

- Vì sao trong đo lường quang học người ta thường dùng tham số Stokes hơn là vector Jones? (Gợi ý: Stokes đo được trực tiếp bằng cường độ, không cần pha chính xác; detector không giữ pha.)
- Jones xử lý được ánh sáng hoàn toàn phân cực — ma trận Mueller 4×4 (bản thân là tổng quát hóa Stokes) giải quyết phân cực một phần bằng cách nào, và vì sao 4 tham số là đủ?