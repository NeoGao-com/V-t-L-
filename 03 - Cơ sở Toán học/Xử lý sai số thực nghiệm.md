---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Xử lý sai số thực nghiệm

> [!abstract] Công cụ để làm gì
> Thước đo không bao giờ cho con số đúng tuyệt đối — mỗi phép đo là một ước lượng kèm độ bất định. Xử lý sai số là bộ quy tắc biến "đám mây số liệu" thành **kết luận có căn cứ**: giá trị trung tâm, độ bất định, và biết khi nào kết quả đáng tin. Đây là cầu nối giữa công cụ toán và trụ cột thực nghiệm.

## Định nghĩa

- **Độ chính xác (accuracy) vs độ phân giải (precision):** chính xác = gần giá trị thật (không sai số hệ thống); phân giải = lặp lại khít nhau (sai số ngẫu nhiên nhỏ). Bắn trúng hồng tâm đều tăm tắp mới là tốt — chỉ "đều tăm tắp" mà lệch tâm là "phân giải cao, chính xác thấp".
- **Sai số tuyệt đối / tương đối:** $A \pm \Delta A$ và $\dfrac{\Delta A}{A}$; viết $\Delta A$ với **tối đa 2 chữ số có nghĩa**.
- **Giá trị tốt nhất:** trung bình cộng $\overline A = \dfrac{1}{N}\sum A_i$; độ bất định của trung bình:
  $\Delta \overline A \approx \dfrac{\sigma}{\sqrt{N}}$
  với $\sigma$ là độ lệch chuẩn — lợi ích của việc đo nhiều lần chỉ tăng như $\sqrt{N}$ (liên hệ [[Xác suất thống kê]]).
- **Truyền sai số:** với $q = q(x, y, z)$ từ các đại lượng đo độc lập:
  $\Delta q = \sqrt{\left(\dfrac{\partial q}{\partial x}\Delta x\right)^2 + \left(\dfrac{\partial q}{\partial y}\Delta y\right)^2 + \left(\dfrac{\partial q}{\partial z}\Delta z\right)^2}$
  — hệ quả thực hành: với tích/thương thì **cộng bình phương sai số tương đối**.
- **Hồi quy tuyến tính (bình phương tối thiểu):** khớp $y = ax + b$ qua các điểm đo; hệ số $a, b$ kèm sai số riêng — còn "độ thẳng" của dữ liệu đo bằng hệ số tương quan $R^2$.

## Ý nghĩa hình học

- Mỗi phép đo là một chấm trên trục số; $N$ lần đo tạo "đám mây" — tâm là giá trị tốt nhất, bán kính là $\Delta A$. Đo thêm chỉ làm đám mây *đậm đặc* hơn, **không dời được tâm** nếu có sai số hệ thống — đó là lý do hai loại sai số phải xử lý khác nhau.
- Khớp đường thẳng là kéo một đường đi xuyên đám mây điểm sao cho tổng bình phương khoảng cách dọc $y$ là nhỏ nhất; mỗi điểm vẽ thêm **thanh sai số** (error bar) để thấy đường khớp có "tự tin" hay không.

## Ý nghĩa vật lý

- **Sai số ngẫu nhiên vs hệ thống — hai kẻ thù khác chiến thuật:** ngẫu nhiên (đọc lệch, rung, nhiễu) giảm được bằng đo nhiều lần; hệ thống (thang đo sai, mất nhiệt có quy luật) thì lặp lại bao nhiêu cũng không phát hiện — bài học lớn của [[Thí nghiệm - Giọt dầu Millikan]] (phải hiệu chỉnh hệ số nhớt) và [[Thí nghiệm - Cân xoắn Cavendish]] (đo hằng số $G$ cực nhạy với nhiễu hệ thống).
- **Đủ tốt so với hiệu ứng cần đo:** kết luận chỉ vững khi sai số nhỏ hơn hẳn hiệu ứng — [[Thí nghiệm - Đo nhiệt dung riêng]] phải bù mất nhiệt đủ nhỏ so với nhiệt lượng nhận; [[Thí nghiệm - Máy Atwood]] phải giảm ma sát ròng rọc dưới mức đáng kể so với sai số đo thời gian.
- **Thống kê đếm của phóng xạ:** phân rã là quá trình ngẫu nhiên → sai số đếm $\approx \sqrt{N}$ (Poisson); tách tín hiệu khỏi phông nền phải so sánh trong phạm vi sai số ([[Thí nghiệm - Đo phóng xạ]], [[Phóng xạ]]).
- **Tuyến tính hóa để kiểm chứng định luật:** khí lý tưởng $pV = \text{const}$ → vẽ $p$ theo $1/V$; độ thẳng của đồ thị (gần $R^2 \to 1$) là bằng chứng định lượng của định luật ([[Định luật Boyle-Mariotte]], [[Phương trình trạng thái khí lý tưởng]]).
- **Ví dụ mẫu — đo $g$ bằng con lắc đơn:** $T = 2\pi\sqrt{l/g}$ → $g = 4\pi^2 l / T^2$; sai số tương đối của $g$ là tổng bình phương sai số của $l$ và $T$ — cho thấy vì sao nên đo $T$ nhiều chu kỳ liên tiếp (giảm $\Delta T$) ([[Con lắc đơn]], [[Trọng lực]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Thí nghiệm - Đo nhiệt dung riêng]] · [[Thí nghiệm - Đo công suất tỏa nhiệt]]: bù trừ nhiệt, sai số hệ thống.
- [[Thí nghiệm - Đo phóng xạ]]: thống kê đếm $\sqrt{N}$ và tách tín hiệu khỏi phông.
- [[Thí nghiệm - Giọt dầu Millikan]] · [[Thí nghiệm - Cân xoắn Cavendish]]: hiệu chỉnh hệ thống, đo đại lượng cực nhỏ.
- [[Thí nghiệm - Máy Atwood]]: khống chế sai số hệ thống (ma sát) trong đo gia tốc.
- [[Con lắc đơn]] · [[Trọng lực]]: ví dụ truyền sai số qua phép đo gián tiếp.
- [[Định luật Boyle-Mariotte]] · [[Phương trình trạng thái khí lý tưởng]]: tuyến tính hóa để kiểm chứng.
- [[Xác suất thống kê]]: cơ sở lí thuyết của trung bình và $1/\sqrt{N}$.

## Liên kết

- [[MOC - Cơ sở Toán học]] · [[MOC - Giả thuyết và Thực nghiệm]]
- [[Xác suất thống kê]] · [[Toán tổ hợp]] · [[Đạo hàm]] (truyền sai số dùng đạo hàm riêng) · [[Logarit]] (thang log khi sai số tương đối)

## Câu hỏi mở

- Làm sao phát hiện sai số hệ thống khi không có "chuẩn vàng" để so? (Gợi ý: đổi dụng cụ, đổi phương pháp, đối chiếu các phép đo độc lập — nguyên tắc của đo $G$ và đo $e$ trong lịch sử.)
- Sai số đếm phóng xạ $\sqrt{N}$ đến từ đâu, và vì sao nó lại đúng bằng độ lệch chuẩn của phân bố Poisson? (Gợi ý: mỗi hạt là một biến ngẫu nhiên độc lập — [[Xác suất thống kê]].)
- Khi các đại lượng đo **không độc lập** (tương quan với nhau), công thức truyền sai số cần thêm gì? (Gợi ý: số hạng hiệp phương sai — và vì sao việc trừ hai số gần bằng nhau lại "phóng đại" sai số tương đối.)