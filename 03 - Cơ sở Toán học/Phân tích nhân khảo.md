---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Phân tích nhân khảo

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Phân tích nhân khảo trả lời câu hỏi khác với giải tích: **"khi tham số nhỏ đi thì nghiệm hành xử ra sao?"**. Nó không cần lời giải tường minh — chỉ cần thứ bậc trước và thứ bậc của nhân tố nhỏ. Đó là công cụ quyết định trong hầu hết các bài toán vật lý thực tế: xấp xỉ gần bằng không, bán kính khối cầu lớn, thời gian mở rộng nhỏ, hành động tâm bán kính lớn, hiệu ứng đường ngầm sóng phẳng. Phương pháp WKB là biến thể nổi tiếng nhất.

## Định nghĩa

$$\phi(\varepsilon) \sim a_0 + a_1\varepsilon + a_2\varepsilon^2 + a_3\varepsilon^3 + \dots,\qquad \varepsilon\to 0$$

Viết $\sim$ ở đây **không** phải "tỷ lệ hai vế tiến tới 1" (điều đó chỉ đúng khi $a_0\neq0$ và ta chỉ giữ lại số hạng dẫn). Ý nghĩa đúng là: **sau khi cắt ở số hạng bậc $N$, phần dư nhỏ hơn bậc đó**,
$$\phi(\varepsilon) - \sum_{n=0}^{N} a_n\varepsilon^n = o(\varepsilon^N).$$
Đây là điểm khác biệt cốt lõi so với [[Chuỗi Taylor & xấp xỉ]] — ở đó sai số là hàng hữu hạn, ở đây sai số **tiêu biến theo chính tham số nhỏ**, và ta đổi lấy khả năng giải bài toán không có lời giải tường minh.

**Cân bằng trội (dominant balance):** với $\varepsilon\to 0$, số hạng nào trong phương trình lớn nhất sẽ chi phối. Nếu không có sự hủy giữa hai số hạng, ta cân bằng chúng để tìm thứ bậc của nghiệm. Ví dụ $\varepsilon y^2 - y + \varepsilon = 0$ có **hai** nhánh nghiệm, mỗi nhánh đòi hỏi một cân bằng khác nhau:
- Cân bằng $\varepsilon y^2$ với $-y$ ⟹ $y \sim \dfrac{1}{\varepsilon}$: nhánh lớn, phương sai $\varepsilon$ nhỏ hơn hẳn và bị bỏ.
- Cân bằng $-y$ với $+\varepsilon$ ⟹ $y \sim \varepsilon$: nhánh nhỏ, lúc này $\varepsilon y^2 = O(\varepsilon^3)$ nhỏ hơn nữa nên bỏ.

Cốt lõi: **một phương trình có thể sinh nhiều tỉ lệ thứ bậc khác nhau cùng lúc**, và việc phải đoán xem nghiệm nào "nhỏ" chính là lý do phương pháp này dễ sai ở tay người mới.

**Cấp số hạng và phép thế "bóng đen":** với dạng điển hình có nhân tố nhỏ và tham số lớn, ta thế $x = \varepsilon y$ (hoặc $\varphi = e^{-\lambda u}$) rồi giải bài toán ở $\varepsilon = 0$, và sửa từng bậc.

## Phương pháp WKB

Giải phương trình Schrödinger với thế biến đổi chậm:

$$-\dfrac{\hbar^2}{2m}\psi'' + V(x)\psi = E\psi \;\Longrightarrow\; \psi(x) \approx \frac{C}{\sqrt{p(x)}}\exp\!\left[\pm\frac{i}{\hbar}\int^x p(x')\,dx'\right],\quad p = \sqrt{2m[E - V(x)]}$$

- Điều kiện áp dụng: $V$ thay đổi chậm trên **thang bước sóng cục bộ** $\lambda = 2\pi\hbar/p$, tức $|\lambda'|\ll 1$. Với $p' = -mV'/p$ thì điều kiện này viết thành $\dfrac{\hbar m|V'|}{p^3}\ll 1$, tức $\boxed{|V'| \ll \dfrac{p^3}{m\hbar}}$.
- Mũ $\exp\!\left[+\dfrac{i}{\hbar}\int^x p\,dx\right]$: hành vi **dao động** — vùng cho phép $V<E$, sóng đứng.
- Mũ $\exp\!\left[-\dfrac{i}{\hbar}\int^x p\,dx\right]$ ở vùng cấm (mang tính $e^{-S/\hbar}$): hành vi **lỗi**, biên mất theo cấp số mũ.
- Tại **điểm lập (turning point)** $V = E$: $p\to 0$ nên bước sóng $\lambda = 2\pi\hbar/p$ bị **chạy ra vô hạn** đồng thời tiền tố $1/\sqrt{p}$ nổ tung — WKB hỏng đúng chỗ đó. Sửa bằng nối liếp Airy — chính là hàm Airy trong [[Hàm đặc biệt]], cầu nối giữa vùng cho phép và vùng cấm.

## Ý nghĩa vật lý

- **Xấp xỉ gần bằng không:** $\sqrt{1+x} \approx 1 + x/2$ khi $|x|\ll 1$ — và $\sqrt{1+x} \approx 1/\sqrt x$ khi $x\to\infty$. Cùng một hàm, hai giới hạn khác nhau, hai vật lý khác nhau.
- **Trường yếu:** mọi trường điện từ, từ trường, trọng trường đều là trường yếu, nên khai triển theo $\varepsilon$ cho công thức dùng được ngay. Xem [[Điện từ trường]], [[Trọng lực]].
- **Cơ học lượng tử:** hành vi sóng phẳng ở năng lượng cao, hành vi lỗi ở vùng cấm, và **nối liếp Airy** ở vùng nối — nền tảng của lý thuyết phản xạ (và cả hiệu ứng giảm chấn khi có khuếch tán).
- **Hiệu ứng đường ngầm:** hành vi xuyên tường là $e^{-S/\hbar}$, hiệu ứng tắt theo cấp số mũ $\hbar$ — thứ bậc cao nhất có ý nghĩa. Xem [[Hàng rào thế và hiệu ứng đường ngầm]].
- **Giản nén dữ liệu:** nhịp tim, thị giác, hành vi giá là giải phương trình khuếch tán ở thời gian dài, ở đó trạng thái quên hết chi tiết — chỉ vài số hạng đầu trong khai triển nhân khảo là đủ.
- **Tán xạ với năng lượng cao:** phương pháp lý thuyết mở rộng, nơi góc phân tán được lấy từ thế bậc đầu tiên trong khai triển.
- **Độ dài tương đối trong lý thuyết tương đối:** so sánh tốc độ hạt với $c$ — cũng là một dạng phân tích nhân khảo trong tham số $v/c$.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Hàng rào thế và hiệu ứng đường ngầm]]: $S = \int\sqrt{2m(V-E)}\,dx$ trong mũ $e^{-S/\hbar}$ là hẳn nhân khảo thuần.
- [[Giếng thế hữu hạn]] · [[Giếng thế vô hạn]]: hành vi giảm chấn ở vùng cấm là hành vi nhân khảo thuần.
- [[Trường xuyên tâm]]: ở lực hấp dẫn, hiệu ứng tương đối tính chỉ bậc $v^2/c^2$.
- [[Phân tích thứ nguyên]] · [[Thí nghiệm - Mặt phẳng nghiêng của Galileo]]: giới hạn góc nhỏ là một dạng nhân khảo.
- [[Chuỗi Taylor & xấp xỉ]]: quan hệ nhân khảo luôn dựa trên khai triển, nhưng chấp nhận sai số bậc 0.
- [[Thuyết tương đối hẹp]]: khai triển theo $v^2/c^2$ là phân tích nhân khảo chuẩn.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Chuỗi Taylor & xấp xỉ]] · [[Phương trình vi phân]] · [[Hàm đặc biệt]] · [[Phương trình khuếch tán]]

## Câu hỏi mở

- Vì sao WKB cho công thức hợp lệ ở vùng cho phép lại **hỏng** chính tại điểm lập? (Gợi ý: xem [[Giải tích Vector (Grad, Div, Curl)]] để hiểu vì sao thang bước sóng co về 0.)
- Trong [[Định luật Rayleigh-Jeans]] và [[Định luật Stefan-Boltzmann]], các điều kiện tiên quyết chính là các giới hạn nhân khảo nào?
- Có thể suy ra phương pháp WKB một cách trực tiếp từ [[Phương pháp số]] không?
- Vì sao không một phương pháp xấp xỉ nào cho lời giải đúng ở mọi giá trị tham số? (Gợi ý: xem [[Phân tích thứ nguyên]].)
