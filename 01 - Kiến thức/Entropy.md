---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: nhiệt-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Entropy

> [!abstract] Ý chính
> Entropy đo **mức độ hỗn loạn** — số trạng thái vi mô $W$ tương ứng với một trạng thái vĩ mô: $S = k\ln W$. Trong hệ cô lập, entropy **không bao giờ giảm**: đó chính là "mũi tên thời gian".

## Định nghĩa

- Định nghĩa thống kê (Boltzmann): $S = k\ln W$ ($k$: hằng số Boltzmann; $W$: số cách sắp xếp vi mô của cùng một trạng thái vĩ mô) — đếm $W$ là bài toán [[Toán tổ hợp]], tính bằng [[Logarit]].
- Định nghĩa nhiệt động (quá trình thuận nghịch): $\Delta S = \dfrac{Q}{T}$.
- Nguyên lý II qua entropy: $\Delta S \ge 0$ với hệ cô lập — tự diễn biến luôn đi theo chiều nhiều trạng thái vi mô hơn (xem [[Nguyên lý thứ hai nhiệt động lực học]]).

## Bảng entropy của các quá trình cơ bản

| Quá trình | Công thức $\Delta S$ | Ví dụ số |
| --- | --- | --- |
| Giãn tự do khí lý tưởng | $nR\ln\dfrac{V_2}{V_1}$ | 1 mol khí, thể tích gấp đôi: $\approx 5{,}8$ J/K |
| Trộn hai khí khác nhau | $nR\ln 2$ | $\approx 5{,}8$ J/K mỗi mol — không thể thu hồi |
| Truyền nhiệt $Q$ từ $T_1$ sang $T_2 < T_1$ | $Q\left(\dfrac{1}{T_2} - \dfrac{1}{T_1}\right)$ | 1 kJ từ 300 K sang 280 K: $\approx 0{,}24$ J/K |
| Nóng chảy | $\dfrac{mL}{T_{nc}}$ | 1 kg nước đá ở 273 K: $\approx 1{,}22$ kJ/K |

## Vì sao entropy chỉ tăng

- Trạng thái vĩ mô có $W$ lớn thì **xác suất xuất hiện cao hơn** ([[Xác suất thống kê]]): khí tự dãn vào toàn bộ bình chứa chứ không tự co lại — không phải vì "không thể" mà vì "gần như không bao giờ".
- Ví dụ điển hình: $N$ phân tử khí, xác suất tất cả cùng nằm nửa trái bình là $1/2^N$. Với $N \sim 10^{23}$, con số này nhỏ hơn mọi khả năng quan sát được — **không bao giờ thấy** khí tự co lại một nửa bình.

## Ý nghĩa

- Ấn định **chiều của thời gian**: quá trình có chiều thuận là chiều entropy tăng.
- Giới hạn hiệu suất động cơ nhiệt: $H \le 1 - \dfrac{T_2}{T_1}$ — xem [[Động cơ nhiệt và máy lạnh]].
- Góc độ thông tin: $S = k\ln W$ chính là lượng thông tin còn thiếu để biết chính xác hệ đang ở trạng thái vi mô nào.

## Kiểm chứng & giới hạn

- Thực nghiệm: mọi quá trình tự diễn biến tăng entropy (khuếch tán, trộn, dãn khí, tan băng) — đo trực tiếp bằng nhiệt lượng kế.
- Giới hạn: hệ lượng tử vướng víu đòi hỏi entropy von Neumann; entropy lỗ đen Bekenstein–Hawking $S = \dfrac{A}{4\ell_{Pl}^2}$ là mở rộng sâu của công thức Boltzmann — vẫn là biên giới nghiên cứu nhiệt động–thông tin.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Nguyên lý thứ hai nhiệt động lực học]]: phát biểu động học của cùng định luật.
- [[Logarit]]: công cụ chuyển tích số $W$ thành tổng $S$.
- [[Xác suất thống kê]]: trạng thái vĩ mô có $W$ lớn thì xác suất xuất hiện cao.
- [[Toán tổ hợp]]: đếm $W$ trong các bài toán phân bố phân tử.
- [[Động cơ nhiệt và máy lạnh]]: giới hạn hiệu suất suy từ entropy.

## Câu hỏi mở

- Vũ trụ có chạy tới "cái chết nhiệt" (entropy cực đại, mọi chênh lệch nhiệt độ biến mất) không? — vấn đề mở trong vũ trụ học (xem [[Nguyên lý Vũ trụ học]]).
- Vì sao vũ trụ **bắt đầu** với entropy thấp đến vậy? (Mọi quá trình đều "ăn" chênh lệch nhiệt độ — nguồn gốc entropy thấp ban đầu chưa được giải thích trọn vẹn.)
- Entropy lỗ đen $S = A/4\ell_{Pl}^2$ gợi ý thông tin biến mất khi vật chất rơi vào lỗ đen — mâu thuẫn với cơ học lượng tử, hay chính là chìa khóa của hấp dẫn lượng tử?