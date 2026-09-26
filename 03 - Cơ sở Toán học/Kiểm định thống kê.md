---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Kiểm định thống kê

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Mỗi phép đo đều cho một con số cộng với một sai số — nhưng "sai số bao nhiêu thì đủ để khẳng định một cái gì đó" là câu hỏi toán học riêng. Kiểm định thống kê trả lời chính xác câu hỏi đó: **dữ liệu có thực sự bác bỏ giả thuyết không, hay chỉ là nhiễu ngẫu nhiên?** Đây là bước cuối và bước quyết định của mọi vòng lặp giả thuyết → dự đoán → đo đạc → kết luận.

## Định nghĩa

**Ước lượng chặn (fit):** với dữ liệu $\{x_i, y_i\}$ và mô hình có tham số, tìm tham số tối ưu. Trường hợp tuyến tính:

$$y = a + bx \quad\Rightarrow\quad b = \frac{\sum_i(x_i-\bar x)(y_i-\bar y)}{\sum_i(x_i-\bar x)^2},\qquad a = \bar y - b\bar x$$

Sai số chuẩn của $b$ là $\sigma_b = \dfrac{s}{\sqrt{\sum_i(x_i-\bar x)^2}}$ với $s$ là độ lệch chuẩn dư — nên **sai số giảm khi tăng số điểm đo**. Xem [[Xử lý sai số thực nghiệm]].

**Vùng tin cậy:** khoảng chứa giá trị thật $b_0$ ở mức tin cậy $1-\alpha$ (thường 95%):

$$b_0 = b \pm t_{\alpha/2,\nu}\,\sigma_b$$

Ở đây $t_{\alpha/2,\nu}$ là **phân phối Student** với $\nu$ bậc tự do. Với số điểm lớn thì $t_{\alpha/2,\nu}\to 1{,}96$ ở $\alpha=0{,}05$ — con số $1{,}96$ là giới hạn phân phối chuẩn, **không** dùng được khi $\nu$ nhỏ (ví dụ khi chỉ có vài chục phép đo). Đây là chỗ hay sai nhất trong xử lý số liệu thực nghiệm.

**Kiểm định chi-square** — dành cho dữ liệu **phân loại**, tức so sánh số đếm quan sát với dự đoán lý thuyết:

$$\chi^2 = \sum_{i}\frac{(O_i - E_i)^2}{E_i},\qquad \text{bậc tự do } \nu = N - 1 - p$$

với $N$ số nhóm dữ liệu và $p$ số tham số đã ước lượng từ chính dữ liệu đó.

- Nếu $\chi^2 \ll \nu$: mô hình khớp quá tốt, đáng ngờ (có thể dữ liệu bị "làm tròn" hay sai sót phép đo).
- Nếu $\chi^2 \gg \nu$: mô hình bị bác bỏ.
- Đây là con đường kinh điển mà mọi phép thực nghiệm vật lý đi: số liệu Planck, hiệu ứng Compton, hiệu ứng quang điện đều được kiểm tra bằng $\chi^2$.

**Phép kiểm định giả thuyết:** từ một bất đẳng thức suy ra một đại lượng có **phân phối đã biết**, rồi tính xác suất quan sát được dữ liệu hiện có là bao nhiêu. Nếu xác suất đó nhỏ hơn $\alpha$ thì bác bỏ giả thuyết — nhưng **không** bao giờ "chứng minh" giả thuyết đúng (xem [[Giả thuyết - Ether vũ trụ]]).

**Sai lầm hệ thống và sai số ngẫu nhiên:** sai số ngẫu nhiên giảm theo $\dfrac{1}{\sqrt N}$; sai lầm hệ thống **không** giảm theo bất kỳ cách nào. Thử lặp lại phép đo không phát hiện được sai lầm hệ thống — đó là điểm mấu chốt của khoa học thực nghiệm.

## Ý nghĩa vật lý

- **Xác nhận thực nghiệm:** mọi phát hiện vật lý đều dừng ở "dữ liệu phù hợp với mô hình trong sai số đo được" — không đi được xa hơn. Xem [[Thí nghiệm - Bức xạ vật đen]], [[Thí nghiệm - Franck-Hertz]].
- **Hiệu ứng nhỏ:** mọi hiệu ứng cần tìm — Compton, Zeeman, Hall — đều là câu hỏi "tín hiệu có lớn hơn nhiễu và sai số không?" Xem [[Hiệu ứng Compton]], [[Hiệu ứng Zeeman]].
- **Lý thuyết hóa học:** trạng thái cân bằng dự đoán tỉ lệ cân bằng; số liệu thực nghiệm là phép kiểm tra của nó. Xem [[Phương trình trạng thái khí lý tưởng]].
- **Bản chất sóng:** số liệu giao thoa khớp với dự đoán cường độ, và khác bao nhiêu phần trăm mới đủ gọi là "bác bỏ thuyết sóng"? Xem [[Thí nghiệm - Hai khe Young]], [[Ánh sáng và bản chất sóng]].
- **Mô hình và độ sâu:** thí nghiệm Michelson–Morley có thể loại trừ tới mức nào, và vì sao phát hiện âm động lượng ether lại là bằng chứng mạnh? Xem [[Thí nghiệm - Michelson-Morley]], [[Thuyết tương đối hẹp]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Xử lý sai số thực nghiệm]]: nền tảng về sai số và ước lượng tham số mà note này mở rộng thành kiểm định.
- [[Xác suất thống kê]] · [[Xác suất và trị trung bình]]: phân phối dùng để tính xác suất quan sát.
- [[Mắt và các tật của mắt]]: ngưỡng nhận biết thị giác chính là một bài kiểm định thống kê.
- [[Phân tích thứ nguyên]]: trước khi so sánh với lý thuyết, mọi đại lượng phải cùng đơn vị.
- [[Quan sát - Bức xạ phông vi sóng vũ trụ (CMB)]]: phân tích dữ liệu vũ trụ là một bài kiểm định thống kê quy mô lớn.
- [[Giả thuyết - Ether vũ trụ]]: ví dụ điển hình về bằng chứng không thể bác bỏ tuyệt đối.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Xác suất thống kê]] · [[Xử lý sai số thực nghiệm]] · [[Toán tổ hợp]] · [[Hàm Gamma]]
- [[Phương pháp số]]

## Câu hỏi mở

- Vì sao không thể bằng thực nghiệm nào "chứng minh" một lý thuyết vật lý đúng? (Gợi ý: xem [[Giả thuyết - Ether vũ trụ]].)
- Một thí nghiệm âm tính với $\chi^2$ nhỏ hơn bậc tự do nói lên điều gì về dữ liệu? (Gợi ý: nghĩ về sai lầm hệ thống.)
- Vì sao sai số ngẫu nhiên giảm theo $1/\sqrt N$ chứ không phải $1/N$? (Gợi ý: xem [[Xác suất thống kê]].)
- Có thể kiểm định một mô hình thống kê bằng dữ liệu mà bản thân nó sinh ra không? (Gợi ý: xem [[Phương pháp số]].)
