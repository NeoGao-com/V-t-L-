---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Phân tích thứ nguyên

> [!abstract] Công cụ để làm gì
> Phân tích thứ nguyên chú ý đến **đơn vị vật lý** (m, s, kg, A...) thay vì con số — nó cho phép *suy luận hình dạng công thức* trước khi tính, *kiểm tra* kết quả sau khi tính, và *dự đoán* quan hệ tỉ lệ mà không cần giải phương trình. Kỹ thuật rẻ nhất và nhanh nhất trong hộp công cụ vật lý.

## Định nghĩa

- **Thứ nguyên** của các đại lượng cơ bản: độ dài $[L]$, thời gian $[T]$, khối lượng $[M]$, nhiệt độ $[\Theta]$, dòng điện $[I]$, lượng chất $[N]$, cường độ sáng $[I_v]$ (ký hiệu chuẩn SI là cd; **không** dùng $J$ vì $J$ đã là jul).

Bảng thứ nguyên thường gặp:

| Đại lượng | Thứ nguyên | Đơn vị SI |
| --- | --- | --- |
| Vận tốc | $[LT^{-1}]$ | m/s |
| Gia tốc | $[LT^{-2}]$ | m/s² |
| Lực | $[MLT^{-2}]$ | N |
| Năng lượng | $[ML^2T^{-2}]$ | J |
| Công suất | $[ML^2T^{-3}]$ | W |
| Áp suất | $[ML^{-1}T^{-2}]$ | Pa |
| Tần số góc | $[T^{-1}]$ | rad/s |

- **Nguyên tắc vàng:** mọi phương trình vật lý đúng đều **đồng nhất về thứ nguyên** — hai vế phải cùng đơn vị; $\sin$, $\ln$, $e^x$ chỉ nhận đối số không thứ nguyên.
- **Định lý Buckingham Π:** quan hệ giữa $n$ đại lượng có thể viết thành quan hệ giữa $n - k$ tổ hợp không thứ nguyên (với $k$ đại lượng cơ bản độc lập).

## Ý nghĩa hình học

- Tưởng tượng "trục đơn vị" của không gian đại lượng: mỗi đại lượng là một "véc-tơ số mũ" $(L, T, M)$; đồng nhất thứ nguyên là hai véc-tơ phải trùng — kiểm tra "hướng" trước khi kiểm tra "độ lớn". Đại lượng không thứ nguyên là "véc-tơ số 0" — thuộc về hình học tỉ lệ, an toàn đưa vào hàm số.

## Ý nghĩa vật lý

- **Ví dụ mẫu — chu kỳ con lắc (Buckingham bằng tay):** giả sử $T = l^\alpha g^\beta m^\gamma$, đồng nhất $[T] = [L]^{\alpha}[LT^{-2}]^\beta [M]^\gamma$ → $\gamma = 0$ (khối lượng biến mất!), $\alpha + \beta = 0$, $-2\beta = 1$ → $T \sim \sqrt{l/g}$. Thứ nguyên **loại khối lượng ra** trước khi làm vật lý — vì sao [[Con lắc đơn]] không phụ thuộc khối lượng.
- Cùng thủ tục: tốc độ vũ trụ cấp 1 $v \sim \sqrt{GM/r}$ ([[Vệ tinh và tốc độ vũ trụ]], [[Định luật vạn vật hấp dẫn]]); lực hướng tâm $F \sim mv^2/r$ ([[Lực hướng tâm]], [[Chuyển động tròn đều]]).
- **Thứ nguyên quyết định dạng định luật:** nếu hấp dẫn có hằng số $G$ thứ nguyên $[M^{-1}L^3T^{-2}]$, muốn lực $[MLT^{-2}]$ từ $[M][M]/[L^2]$ thì buộc phải nhân $G$ — luật nghịch đảo bình phương là "hình dạng duy nhất" hợp thứ nguyên giữa hai khối lượng cách nhau $r$ ([[Định luật vạn vật hấp dẫn]]); [[Định luật Coulomb]] tương tự với $k_e$.
- **Đối số hàm phải không thứ nguyên:** trong $x = A\sin(\omega t + \varphi)$, mọi thứ trong $\sin$ có đơn vị rad — viết $\sin(\omega t)$ với $\omega$ tần số góc chứ không phải tần số $f$; vi phạm điều này là nguồn lỗi "đau thương" trong công thức ([[Dao động điều hòa]], [[Lượng giác]]).
- **Đại lượng không thứ nguyên để so sánh họ hệ:** tỉ số $v/c$ quyết định "cổ điển hay tương đối tính", $v/v_{âm thanh}$ (số Mach) quyết định chế độ dòng khí — các đại lượng vô thứ nguyên là "máy phân loại" hiện tượng ([[Sóng cơ]], [[Sóng âm]]).
- **Đánh giá độ lớn:** năng lượng liên kết hạt nhân ~ $mc^2$ ≈ GeV thay vì vài eV nguyên tử — thang năng lượng của một hiện tượng đọc thẳng từ thứ nguyên ([[Cấu tạo hạt nhân]], [[Phản ứng phân hạch]]).
- **Kiểm tra kết quả tức thì:** bất kỳ đáp số nào ra sai thứ nguyên đều sai chắc chắn — "máy phát hiện lỗi" miễn phí cho mọi bài toán ([[Công và công suất]], [[Động năng]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Con lắc đơn]] · [[Vệ tinh và tốc độ vũ trụ]]: công thức suy từ thứ nguyên (khối lượng biến mất).
- [[Định luật vạn vật hấp dẫn]] · [[Định luật Coulomb]]: dạng lực bị "ép" bởi thứ nguyên hằng số.
- [[Công và công suất]] · [[Động năng]]: kiểm tra nhanh kết quả.
- [[Chuyển động tròn đều]] · [[Lực hướng tâm]]: $F \sim mv^2/r$ từ thứ nguyên.
- [[Cấu tạo hạt nhân]] · [[Phản ứng phân hạch]]: ước lượng thang năng lượng $mc^2$.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Logarit]] (log-log để đọc số mũ thứ nguyên) · [[Đại số tuyến tính]] (véc-tơ số mũ) · [[Lượng giác]] (đối số rad) · [[Hệ tọa độ]] · [[Xử lý sai số thực nghiệm]] (đơn vị trong đo đạc)

## Câu hỏi mở

- Phân tích thứ nguyên suy được *hệ số* bằng 1, $4\pi^2$, $\frac{1}{2}$... không? (Gợi ý: không — hệ số là "phần tinh tế" cần lý thuyết hoặc thực nghiệm; thứ nguyên chỉ cho khung, như $T = 2\pi\sqrt{l/g}$ với hệ số $2\pi$ phải đến từ giải phương trình.)
- Vì sao phương trình lượng tử lại cần $\hbar$ làm "thước thứ nguyên"? (Gợi ý: không có $\hbar$, từ vị trí–động lượng không ghép được thành tác dụng — so sánh với $c$ trong tương đối: mỗi hằng số nền tảng "đóng khung" một lớp hiện tượng mới.)
- Giữa hệ SI (7 đơn vị cơ bản) và hệ tự nhiên ($c = \hbar = G = 1$), thứ nguyên "biến mất" như thế nào — và vì sao vẫn cần "thứ nguyên dư" như năng lượng để đếm bậc tự do? (Gợi ý: số chiều độc lập là điều kiện để định lý Buckingham Π "chạy".)