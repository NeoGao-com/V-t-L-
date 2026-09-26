---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: nhiệt-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Định luật Stefan-Boltzmann

> [!abstract] Ý chính
> Tổng công suất bức xạ của một bề mặt đen tỷ lệ với lũy thừa bốn của nhiệt độ: $M=\sigma T^4$. Đây là định luật thực nghiệm về **toàn phổ**, không cho biết cường độ tại từng bước sóng.

## Phát biểu

Với diện tích đen tuyệt đối $S$ ở nhiệt độ $T$:

$P=\sigma S T^4$

hay trên một đơn vị diện tích:

$M=\frac{P}{S}=\sigma T^4$

trong đó hằng số Stefan–Boltzmann là

$\sigma=5{,}670374419\times10^{-8}\ \mathrm{W\,m^{-2}\,K^{-4}}$.

Đơn vị của $\sigma$ là $\mathrm{W\,m^{-2}\,K^{-4}}$.

## Vật thật và hệ số phát xạ

Bề mặt thật có thể phát:

$M=\varepsilon\sigma T^4$

với $\varepsilon$ là **độ phát xạ** (emissivity), $0\leq\varepsilon\leq1$. Vật đen tuyệt đối có $\varepsilon=1$.

Với bề mặt xám khuếch tán, $\varepsilon$ không đổi theo bước sóng, hệ số nhìn bằng một và hốc đen bao quanh ở nhiệt độ $T_0$, **công suất thuần** là:

$P_{\text{thuần}}=\varepsilon\sigma S\left(T^4-T_0^4\right)$.

Do đó không nên gọi $\sigma T^4$ là “tốc độ mất nhiệt thuần” nếu chưa trừ bức xạ môi trường.

## Hệ quả so sánh

Với cùng diện tích, cùng vật liệu và cùng điều kiện môi trường:

$\frac{M_2}{M_1}=\left(\frac{T_2}{T_1}\right)^4$.

- Tăng nhiệt độ gấp đôi làm công suất bức xạ tăng $2^4=16$ lần.
- Nhiệt độ phải dùng kelvin; dùng nhiệt độ °C trong $T^4$ là sai.
- Khi gần $0\ \mathrm{K}$, lực bức xạ tiến tới 0 theo $T^4$.

## Từ phổ Planck đến định luật Stefan-Boltzmann

Tích phân phổ Planck theo bước sóng:

$M(T)=\int_0^\infty M_\lambda(T)\,d\lambda=\sigma T^4$.

Như vậy Stefan–Boltzmann là hệ quả tích phân của công thức Planck, trong khi Rayleigh–Jeans chỉ là giới hạn miền sóng dài của công thức đó.

Nếu dùng mật độ năng lượng bức xạ đẳng hướng $u(T)$ trong chân không, quan hệ tương ứng là:

$u(T)=\frac{4\sigma}{c}T^4$.

Không được đồng nhất $u(T)$ với $M(T)$ vì chúng khác đơn vị và khác cách tính trên diện tích.

## Kiểm chứng & giới hạn

- Thực nghiệm: phổ Planck tích phân khớp tổng công suất đo trong phạm vi nhiệt độ khá rộng.
- Phạm vi: pháp tuyến tối đa hữu ích khi vật ở trong chân không; trong khí quyển phải dùng các hệ số truyền và phát xạ chọn lọc.
- Giới hạn thực hành: ở nhiệt độ rất thấp, công thức dự đoán công suất rất nhỏ nên nhiễu tầng nhiệt và bức xạ nền có thể chiếm ưu thế.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[MOC - Chương 1 - Cơ sở vật lý của cơ học lượng tử]]
- [[Bức xạ nhiệt và vật đen tuyệt đối]]
- [[Giả thuyết - Lượng tử năng lượng Planck]]
- [[Thí nghiệm - Bức xạ vật đen]]
- [[Nhiệt lượng và cách truyền nhiệt]]

## Câu hỏi mở

- Vì sao tích phân toàn phổ của công thức Planck lại dẫn đến $M\propto T^4$?
- Nhiệt kế hồng ngoại đo công suất theo một vùng phổ; vì sao cần hiệu chỉnh theo độ phát xạ thay vì áp trực tiếp $\sigma T^4$?
- Trong không gian có bức xạ nền, vì sao không thể suy ra nhiệt độ chỉ từ một phép đo công suất tuyệt đối?
