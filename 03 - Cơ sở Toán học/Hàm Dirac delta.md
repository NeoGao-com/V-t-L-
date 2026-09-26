---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Hàm Dirac delta

> [!abstract] Công cụ để làm gì
> Hàm Dirac delta là "xung" cực hẹp, cực cao nhưng có diện tích đúng bằng 1 — công cụ mô hình hóa **nguồn điểm** (điện tích điểm, lực tức thời, va chạm), trái tim của định nghĩa [[Hàm Green]], và là "đơn vị đo" của mọi trạng thái vị trí liên tục trong [[Tiên đề cơ học lượng tử]].

## Định nghĩa

$\delta(x - x_0)$ là phân bố thỏa hai tính chất:

$\delta(x - x_0) = 0 \ \text{với } x \ne x_0, \qquad \int_{-\infty}^{\infty} \delta(x - x_0)\, dx = 1$

- **Tính chất sàng lọc:** $\int f(x)\, \delta(x - x_0)\, dx = f(x_0)$ — "chọc" đúng giá trị hàm tại điểm.
- **Hàm bước Heaviside:** $\delta(x) = \dfrac{d}{dx}\Theta(x)$ — delta là "đạo hàm của bậc thang dựng đứng".
- **Tỉ lệ (scaling):** $\delta(ax) = \dfrac{\delta(x)}{|a|}$ — co giãn trục làm đổi "chiều cao" để giữ diện tích 1.
- **Đạo hàm của delta:** $\int f(x)\,\delta'(x-x_0)\,dx = -f'(x_0)$ — chuyển "chọc" sang đạo hàm của hàm (công cụ của lý thuyết phân tán).
- **Biểu diễn Fourier:** $\delta(x) = \dfrac{1}{2\pi}\int_{-\infty}^{\infty} e^{ikx}\, dk$ — vô hạn sóng phẳng cùng pha "cộng hưởng" về một điểm ([[Biến đổi Fourier]]).

## Ý nghĩa hình học và cách hình dung

- Một "kim" thẳng đứng vô hạn tại $x_0$ có diện tích 1: càng hẹp thì càng cao để giữ đúng diện tích — mô hình giới hạn chuẩn của phân bố hẹp dần, ví dụ Gauss $\dfrac{1}{\sqrt{2\pi\sigma^2}}e^{-x^2/(2\sigma^2)}$ khi $\sigma \to 0$ (liên hệ [[Xác suất thống kê]]).
- Về bản chất $\delta$ **không phải hàm** thông thường mà là phân bố (distribution): chỉ có nghĩa khi nằm dưới dấu tích phân với một hàm "tử tế" $f$.

## Ý nghĩa vật lý

- **Điện tích điểm:** mật độ điện tích là $\rho(\vec r) = q\,\delta^3(\vec r)$; trong tọa độ cầu $\delta^3(\vec r) = \dfrac{\delta(r)}{4\pi r^2}$ — chính dạng này làm [[Định luật Gauss (điện)]] phục hồi đúng luật nghịch đảo bình phương của [[Định luật Coulomb]] cho điện tích điểm tại tâm.
- **Hàm Green:** định nghĩa $L G = \delta$ — đáp ứng của hệ với "một nhát búa" tại đúng một điểm; nguồn bất kỳ $f$ là chập các nhát búa đó lại ([[Hàm Green]]).
- **Xung lực / va chạm:** lực tức thời $F(t) = J\,\delta(t - t_0)$; tính chất sàng lọc cho $\Delta p = \int F\,dt = J$ — [[Va chạm]], [[Nguyên lý bảo toàn động lượng]].
- **Lượng tử — trạng thái vị trí liên tục:** $\langle x | x' \rangle = \delta(x - x')$ là "bảng tra" trực chuẩn của cơ sở vị trí; trạng thái "ở đúng $x_0$" và sóng phẳng là hai đầu của cùng một biến đổi Fourier — nền hình học của [[Nguyên lý bất định Heisenberg]] ([[Không gian Hilbert]]).
- **Phân bố xác suất liên tục:** trong [[Xác suất thống kê]], delta cung cấp ngôn ngữ cho các phân bố rời rạc như một điểm xác định và giúp nối liền các trường hợp rời rạc–liên tục.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Hàm Green]]: định nghĩa $L G = \delta$ và tích chập nghiệm.
- [[Điện tích và bảo toàn điện tích]] · [[Điện trường]] · [[Định luật Coulomb]]: mật độ điện tích điểm, luật $1/r^2$ từ [[Định luật Gauss (điện)]].
- [[Va chạm]] · [[Nguyên lý bảo toàn động lượng]]: xung lực tức thời.
- [[Tiên đề cơ học lượng tử]] · [[Không gian Hilbert]]: chuẩn hóa trạng thái vị trí liên tục $\langle x | x' \rangle = \delta(x-x')$.
- [[Xác suất thống kê]]: ngôn ngữ phân bố thống nhất rời rạc–liên tục.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Biến đổi Fourier]] (biểu diễn tích phân của delta) · [[Đạo hàm]] (đạo hàm của delta, hàm bước) · [[Tích phân]] · [[Hàm Green]] · [[Không gian Hilbert]] · [[Ký hiệu Dirac]] · [[Xác suất thống kê]]

## Câu hỏi mở

- Vì "không phải hàm thật", delta đặt ra giới hạn gì cho việc *nhân* hai phân bố (ví dụ $\delta(x)^2$)? (Gợi ý: trong lý thuyết trường lượng tử cần chính quy hóa — nguồn gốc các kỹ thuật renormalization.)
- Điện tích "điểm" với mật độ delta có năng lượng tự thân vô hạn — vấn đề này hé lộ điều gì về giới hạn của mô hình hóa điểm trong vật lý?
- $\delta'(x)$ "chọc" vào đạo hàm của hàm — công cụ này cần thiết khi nào trong bài toán tán xạ và điều kiện biên? (Gợi ý: khai triển đa cực, mô hình "vách cứng" trong [[Tiên đề cơ học lượng tử]].)