---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Biến đổi Fourier

> [!abstract] Công cụ để làm gì
> Biến đổi Fourier tách một tín hiệu thành tổng các sóng hình sin — "kính quang phổ" để nhìn mọi dao động dưới dạng thành phần tần số. Cùng một hiện tượng có hai góc nhìn: miền thời gian (hay không gian) và miền tần số.

## Định nghĩa

**Chuỗi Fourier** (tín hiệu tuần hoàn chu kỳ $T$): phân rã thành tổng họa âm
$f(t) = \sum_{n=-\infty}^{\infty} c_n\, e^{i n \omega_0 t}, \qquad \omega_0 = \dfrac{2\pi}{T}$

**Biến đổi Fourier** (tín hiệu bất kỳ, thuận và nghịch đảo):
$\hat f(\omega) = \int_{-\infty}^{\infty} f(t)\, e^{-i\omega t}\, dt$
$f(t) = \dfrac{1}{2\pi}\int_{-\infty}^{\infty} \hat f(\omega)\, e^{i\omega t}\, d\omega$

- $|\hat f(\omega)|$ gọi là **phổ biên độ** — mỗi tần số hiện ra như một đỉnh phổ.
- **Một xung hẹp trong thời gian → phổ rộng; sóng sin thuần túy → một vạch** (đối ngẫu thời gian–tần số, liên hệ [[Số phức]]).
- **Định lý Parseval:** $\int |f|^2 dt = \dfrac{1}{2\pi}\int |\hat f|^2 d\omega$ — năng lượng tín hiệu bảo toàn khi đổi cơ sở.
- **Tích chập:** biến đổi Fourier biến tích chập thành phép nhân thường — $\widehat{f * g} = \hat f \cdot \hat g$ — lý do hàm Green dùng tích chập để "cộng" đáp ứng ([[Hàm Green]]).

## Ý nghĩa hình học

- Đổi cơ sở trực chuẩn: tín hiệu là một vector, các sóng $e^{i\omega t}$ là một cơ sở trực giao; biến đổi Fourier chỉ là chiếu vector lên từng trục tần số (cùng tinh thần [[Đại số tuyến tính]], [[Không gian Hilbert]]).
- Đối ngẫu "hẹp–rộng": sản phẩm độ rộng thời gian × độ rộng tần số có cận dưới $\Delta t\, \Delta \omega \gtrsim 1$ — cùng nguồn gốc toán học với bất định.

## Ý nghĩa vật lý

- **Cùng một hiện tượng, hai góc nhìn:** dao động trong không gian-thời gian hay trong không gian tần số — [[Dao động điều hòa]], [[Sóng cơ]], [[Sóng điện từ và thang sóng điện từ]].
- **Nguyên lý chồng chất:** mọi tín hiệu (kể cả không tuần hoàn) đều là chồng chất của vô số dao động điều hòa — [[Tổng hợp dao động]]; âm thanh có "âm sắc" riêng vì phổ họa âm khác nhau — [[Sóng âm]].
- **Nhiễu xạ = "Fourier quang học":** phân bố ánh sáng sau khe là biến đổi Fourier của khe — [[Nhiễu xạ ánh sáng]], [[Giao thoa ánh sáng]].
- **Gói sóng trong lượng tử:** hàm sóng cục bộ = chồng chất các sóng phẳng; độ rộng vị trí và động lượng liên hệ ngược nhau → mầm của [[Nguyên lý bất định Heisenberg]] ([[Lưỡng tính sóng-hạt]], [[Phương trình Schrödinger]]).
- Máy phân tích quang phổ thực chất là "máy tính Fourier bằng lăng kính/cách tử" — [[Quang phổ]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Quang phổ]]: vạch quang phổ mã hóa cấu trúc năng lượng của nguyên tử.
- [[Mạch dao động LC]] · [[Mạch RLC và trở kháng]]: mạch tuyến tính "lọc" tín hiệu theo tần số — mỗi tần số đáp ứng riêng (hàm truyền).
- [[Sóng dừng]] · [[Sóng âm]]: tín hiệu thực = tổng các mode điều hòa.
- [[Nguyên lý bất định Heisenberg]]: đối ngẫu thời gian–tần số của cùng một cấu trúc toán.
- [[Hàm Green]]: tích chập trong miền thời gian ↔ phép nhân trong miền tần số.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Số phức]] · [[Tích phân]] · [[Đại số tuyến tính]] · [[Không gian Hilbert]] · [[Dao động điều hòa]] · [[Sóng điện từ và thang sóng điện từ]] · [[Hàm Green]]

## Câu hỏi mở

- Một xung rất ngắn cần phổ rất rộng — đây có phải mầm của hệ thức bất định Heisenberg $\Delta t\,\Delta \omega \gtrsim 1$ khi áp vào [[Tiên đề cơ học lượng tử]]?
- Biến đổi Fourier dùng hàm mũ $e^{i\omega t}$ — nếu dùng cơ sở khác (sóng wavelet, gói Gauss) thì sẽ thắng được gì ở các bài toán có tín hiệu cục bộ cả hai đầu?