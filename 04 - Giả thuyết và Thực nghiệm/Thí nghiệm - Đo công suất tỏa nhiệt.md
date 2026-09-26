---
tags:
  - vật-lý/thực-nghiệm
type: thực-nghiệm
domain: nhiệt-học
loại: thí-nghiệm
trạng-thái: ổn-định
created: 2026-09-25
---

# Thí nghiệm - Đo công suất tỏa nhiệt

> [!abstract] Mục đích
> Đo công suất bức xạ nhiệt $P(T)$ mà một vật phát ra theo nhiệt độ, kiểm chứng định luật Stefan–Boltzmann ($P \propto T^4$) và khớp phổ với định luật Planck — từ đó đo các hằng số vật lý $\sigma$, $k_B$ và $h$; minh chứng trực tiếp [[Nguyên lý bảo toàn năng lượng]] (nhiệt bức xạ là một dạng năng lượng).

## Thiết kế

- **Ý tưởng:** ở trạng thái cân bằng, công suất điện cấp vào dây đốt đúng bằng công suất bức xạ đi ra: $P_{bức xạ} = UI$.
- **Dụng cụ:** dây tóc/khối vật nung trong buồng chân không (loại dẫn nhiệt đối lưu); nguồn + ampe kế + vôn kế để đo $P$; nhiệt kế bức xạ/ngẫu nhiệt để đo $T$; cách tử + detector đo phổ $I(\lambda, T)$.
- **Cách đo:** (1) cố định $U$, $I$ → $P$; đợi cân bằng → $T$; lặp với nhiều dòng; (2) vẽ $P$ theo $T^4$ — đường thẳng qua gốc tọa độ chứng minh định luật Stefan–Boltzmann; (3) phân phổ $I(\lambda,T)$ ở từng $T$ → khớp công thức Planck.

## Kết quả & kết luận

- **Stefan–Boltzmann:** $P = \varepsilon \sigma A (T^4 - T_0^4)$, $\sigma = 5{,}67\times10^{-8}$ W·m⁻²·K⁻⁴ — hệ số góc của $P$ vs $T^4$ cho $\sigma$ (Stefan 1879 thực nghiệm, Boltzmann 1884 lý thuyết).
- **Planck:** $I(\nu, T) = \dfrac{2h\nu^3}{c^2}\dfrac{1}{e^{h\nu/(k_B T)} - 1}$ — khớp toàn phổ cho ra $h = 6{,}626\times10^{-34}$ J·s và $k_B = 1{,}381\times10^{-23}$ J/K.
- **Kiểm chứng số:** dây tóc có $A = 1\times10^{-5}$ m², $\varepsilon \approx 1$:

| $T$ (K) | $T^4$ (K⁴) | $P_{bức xạ} = \sigma A T^4$ |
| --- | --- | --- |
| 500 | $6{,}3\times10^{10}$ | 0,04 W |
| 1000 | $1{,}0\times10^{12}$ | 0,57 W |
| 1500 | $5{,}1\times10^{12}$ | 2,9 W |
| 2000 | $1{,}6\times10^{13}$ | 9,1 W |
| 2500 | $3{,}9\times10^{13}$ | 22 W |
| 3000 | $8{,}1\times10^{13}$ | 46 W |

→ tăng 2 lần nhiệt độ = tăng **16 lần** công suất: kiểm chứng định luật rất nhạy, dễ phát hiện độ lệch so với $T^4$.

## Ảnh hưởng lên lý thuyết

- Đo hằng số tự nhiên độc lập với cơ học: $\sigma$, $k_B$, $h$ từ *nhiệt* — nối thí nghiệm với [[Nội năng]], [[Entropy]] và [[Nguyên lý thứ hai nhiệt động lực học]].
- Bức xạ vật đen + đo công suất là tiền đề trực tiếp của [[Giả thuyết - Lượng tử năng lượng Planck]] và [[Thí nghiệm - Bức xạ vật đen]].
- Ứng dụng: định cỡ đèn sợi đốt/LED, thiết kế tản nhiệt (bức xạ chiếm phần lớn ở $T \gtrsim 600$ K), đo nhiệt độ phòng xa (nhiệt kế hồng ngoại), mô hình khí hậu (cân bằng bức xạ Trái Đất).

## Liên kết

- [[MOC - Giả thuyết và Thực nghiệm]]
- [[MOC - Kiến thức Vật lý]]
- [[Nguyên lý bảo toàn năng lượng]] · [[Nội năng]] · [[Chuyển động Brown]] · [[Thí nghiệm - Bức xạ vật đen]] · [[Giả thuyết - Lượng tử năng lượng Planck]] · [[Nguyên lý thứ hai nhiệt động lực học]] · [[Entropy]] · [[Nhiệt độ và thang nhiệt độ]] · [[Xử lý sai số thực nghiệm]] · [[Quan sát - Bức xạ phông vi sóng vũ trụ (CMB)]]

## Câu hỏi mở

- Vì sao đo $k_B$ qua phổ bức xạ (định luật Planck) chính xác hơn đo qua nhiễu Johnson–Nyquist trong điện trở? (Gợi ý: phổ bức xạ có đỉnh sắc nét ở $\nu_{max} \propto T$ — độ nhạy cao; nhiễu tiếng ồn điện trở nhỏ và dễ bị nhiễm bởi nhiễu thiết bị — hiện nay $k_B$ đo chính xác nhất bằng acoustic gas thermometry.)
- Vì sao vật $T \to 0$ vẫn có thể bức xạ điện từ (hệ quả điểm không của dao động tử)? (Gợi ý: năng lượng điểm không $\frac12 h\nu$ trong [[Giả thuyết - Lượng tử năng lượng Planck]] — nhưng chưa quan sát được bức xạ điểm không do detector hấp thụ lẫn nhau.)