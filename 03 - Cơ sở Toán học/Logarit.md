---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Logarit

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Logarit biến **phép nhân thành phép cộng** và **lũy thừa thành phép nhân**. Trong vật lý, nó xuất hiện ở đúng những chỗ đại lượng trải nhiều bậc độ lớn — chênh lệch vài đơn vị là thay đổi hàng nghìn lần: mức cường độ âm, entropy, hằng số phân rã, pháp tuyến khứ ống, điện thế hóa học.

## Định nghĩa

$$\log_a b = x \iff a^x = b, \qquad a > 0,\ a \ne 1,\ b > 0$$

- **Logarit tự nhiên** $\ln x = \log_e x$ với $e \approx 2{,}71828$ — cơ sở duy nhất xuất hiện trong đạo hàm và tích phân: $\dfrac{d}{dx}\ln x = \dfrac1x$ và $\displaystyle\int\dfrac{dx}{x} = \ln|x| + C$. Mọi cơ sở khác chỉ là $\log_a b = \dfrac{\ln b}{\ln a}$.
- $e$ là giới hạn $\displaystyle\lim_{n\to\infty}\left(1+\dfrac1n\right)^n$ — cơ sở của **lãi kép liên tục**, và là cơ sở tự nhiên của mọi hàm mũ suy giảm.
- **Tính chất:** $\ln(xy) = \ln x + \ln y$; $\ln\dfrac{x}{y} = \ln x - \ln y$; $\ln x^r = r\ln x$ ($x>0$).

> [!warning] Cạm bẫy thứ nguyên
> $\ln$ chỉ nhận **đại lượng vô hướng**. Viết $\ln(5\ \text{m})$ là vô nghĩa — phải viết $\ln\dfrac{L}{L_0}$ với một chuẩn $L_0$. Đó là lý do mọi thang đo thực nghiệm đều là **tỉ số so với một mốc tham chiếu** ($I_0$, $W_0$, $p_0$), và là lý do $S = k_B\ln W$ hợp lệ: $W$ là số trạng thái, vốn vô hướng. Xem [[Phân tích thứ nguyên]].

## Ý nghĩa vật lý

- **Entropy nhiệt động:** $S = k_B\ln W$ — vì $W$ nhân lên khi ghép hai hệ độc lập, $\ln$ biến phép nhân thành phép cộng nên entropy cộng được ([[Entropy]]). Đây là chỗ hẹn gặp đẹp nhất giữa toán học và vật lý.
- **Quy luật phân rã:** $N = N_0e^{-\lambda t}$ ⟺ $\ln N = \ln N_0 - \lambda t$ — nên **tuổi thọ trung bình** $1/\lambda$ chính là thang đo tự nhiên của phóng xạ ([[Phóng xạ]]).
- **Mức cường độ âm:** $L = 10\lg\dfrac{I}{I_0}$ dB; cảm giác thính gần như **tuyến tính theo logarit** vì tế bào lông biểu bão hòa theo mũ — xem [[Sóng âm]] và [[Mắt và các tật của mắt]].
- **Pháp tuyến khứ ống:** $I = I_0e^{-\varepsilon c\ell}$ → $A = \lg\dfrac{I_0}{I} = \varepsilon c\ell/2{,}303$ — hấp thụ phụ thuộc **tuyến tính với số mũ khử**, đó là định luật Beer–Lambert.
- **Cân bằng hóa học:** phương trình Nernst $E = E^0 + \dfrac{RT}{nF}\ln Q$ — thế điện phụ thuộc logarit tỉ số hoạt động.
- **Sóng âm và độ lớn thiên văn:** hiệu ứng Doppler đổi tần số theo *tỉ số* $v/c$, và độ sáng sao đo bằng thang logarit.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Entropy]]: $S = k_B\ln W$ — cầu nối trực tiếp giữa logarit và nhiệt động lực học.
- [[Toán tổ hợp]]: $\ln N!$ là cách viết tắt của $\sum\ln n$ — nền cho xấp xỉ Stirling trong thống kê lượng tử.
- [[Phóng xạ]]: nửa vòng đời là ứng với $\ln 2/\lambda$.
- [[Xác suất thống kê]]: phân bố Gauss có đuôi suy giảm theo mũ, tức đuôi của nó là hàm mũ của khoảng cách — dùng $\ln$ để tuyến tính hóa.
- [[Sóng âm]]: phản ứng của tai nghe là gần tuyến tính theo $\lg I$.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Số phức]] · [[Xác suất thống kê]] · [[Toán tổ hợp]] · [[Phép biến đổi Laplace]]
- [[Chuỗi Taylor & xấp xỉ]]

## Câu hỏi mở

- Vì sao trong vật lý, "một hằng số phụ thuộc đơn vị đo" (như $k_B$) luôn đi kèm một **logarit của một tỉ số vô hướng**? (Gợi ý: xem [[Phân tích thứ nguyên]].)
- Nếu tai nghe có phản ứng gần tuyến tính theo $\lg I$, còn một người bình thường nghe theo thang decibel, thì điều gì suy ra về cách tai **hoạt động về mặt sinh lý**? (Gợi ý: xem [[Mắt và các tật của mắt]].)
- Tại sao tuổi thọ trung bình của một tập thể hạt phân rã lại là $1/\lambda$ chứ không phải $\ln 2/\lambda$? (Gợi ý: phân biệt thời tối thiểu và trung vị.)
- Logarit trên số phức có nhiều giá trị — vì sao? (Gợi ý: xem [[Số phức]].)
