---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Chuỗi Taylor & xấp xỉ

> [!abstract] Công cụ để làm gì
> Chuỗi Taylor khai triển một hàm trơn thành tổng đa thức quanh một điểm — cho phép **thay "cái khó tính" bằng "cái dễ tính"**: mọi phép gần đúng trong vật lý (dao động nhỏ, thấp tốc độ, trường yếu, quang học gần trục...) đều là cắt chuỗi Taylor giữ lại vài số hạng đầu với sai số đã lượng hóa được.

## Định nghĩa

Chuỗi Taylor của hàm $f$ quanh điểm $a$:

$f(x) = \sum_{n=0}^{\infty} \dfrac{f^{(n)}(a)}{n!}\, (x - a)^n = f(a) + f'(a)(x-a) + \dfrac{f''(a)}{2}(x-a)^2 + \cdots$

- **Khai triển Maclaurin** ($a = 0$) thường dùng:

| Hàm | Khai triển | Giữ bậc nhất |
| --- | --- | --- |
| $e^x$ | $1 + x + \dfrac{x^2}{2!} + \dfrac{x^3}{3!} + \cdots$ | $1 + x$ |
| $\sin x$ | $x - \dfrac{x^3}{3!} + \dfrac{x^5}{5!} - \cdots$ | $x$ |
| $\cos x$ | $1 - \dfrac{x^2}{2!} + \dfrac{x^4}{4!} - \cdots$ | $1 - \dfrac{x^2}{2}$ |
| $(1+x)^n$ | $1 + nx + \dfrac{n(n-1)}{2}x^2 + \cdots$ | $1 + nx$ |
| $\ln(1+x)$ | $x - \dfrac{x^2}{2} + \dfrac{x^3}{3} - \cdots$ | $x$ |

- **Số hạng bậc nhất** là **tuyến tính hóa** — tiếp tuyến thay cho đường cong tại $a$; số hạng bậc hai bổ sung "độ cong".
- **Phần dư (Lagrange):** sai số khi cắt ở bậc $k$ là $R_k = \dfrac{f^{(k+1)}(\xi)}{(k+1)!}(x-a)^{k+1}$ với $\xi$ nằm giữa $a$ và $x$ — vừa cho biết **độ lớn sai số**, vừa cho biết xấp xỉ tốt khi $(x-a)$ nhỏ.

## Ý nghĩa hình học

- Gần một điểm, mọi đường cong trơn đều "trông như" đường thẳng (bậc 1), parabola (bậc 2) — giống như nhìn Trái Đất thấy phẳng khi đứng gần.
- Cắt ở bậc càng cao, đồ thị đa thức càng "ôm khít" đường cong trong vùng lân cận; phần dư đo khoảng cách giữa đường cong thật và đa thức cắt cụt.

## Ý nghĩa vật lý

- **Dao động nhỏ = tuyến tính hóa thế năng:** quanh vị trí cân bằng $V(x) \approx V(0) + \tfrac{1}{2}V''(0)\,x^2 = \tfrac{1}{2}kx^2$ — mọi cân bằng bền đều "ngửi thấy" dao động điều hòa ([[Dao động điều hòa]], [[Lực đàn hồi]], [[Thế năng]]); con lắc đơn chỉ điều hòa vì $\sin\theta \approx \theta$ bậc nhất, và tiết diện quang học của [[Thấu kính]]/[[Mắt và các tật của mắt]] cũng hoạt động trong giới hạn "góc nhỏ, gần trục".
- **Giới hạn cổ điển của tương đối:** với $v \ll c$, hệ số Lorentz $\gamma = (1 - v^2/c^2)^{-1/2} \approx 1 + \dfrac{v^2}{2c^2}$ — dùng nhị thức $(1+x)^n$ — mọi công thức Einstein trở về Newton ([[Biến đổi Einstein]], [[Thuyết tương đối hẹp]]).
- **Khai triển đa cực:** thế của phân bố điện tích ở xa có thể khai triển theo bậc — số hạng đầu là điện tích tổng, số hạng kế (bậc một của khoảng cách) mô tả lưỡng cực — nguồn gốc cách nghĩ "điện tích gộp + lưỡng cực + tứ cực..." ([[Điện trường]], [[Điện thế và hiệu điện thế]]).
- **Nguyên tắc nhiễu loạn:** khi phần "nhiễu" nhỏ, khai triển quanh nghiệm đã biết; cùng tinh thần, phương pháp số giải [[Phương trình vi phân]] (tuyến tính hóa từng bước) dựa trên đúng ý tưởng tiếp tuyến này.
- **Xấp xỉ có kiểm soát:** mọi "gần đúng bậc nhất/bậc hai" trong sách giáo khoa đều là cắt chuỗi ở một bậc tường minh — ví dụ [[Sự nở vì nhiệt]] chỉ giữ số hạng bậc nhất theo nhiệt độ.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Con lắc đơn]] · [[Dao động điều hòa]]: $\sin\theta \approx \theta$, thế năng điều hòa quanh cân bằng.
- [[Lực đàn hồi]] · [[Thế năng]]: tuyến tính hóa lực/thế quanh điểm cân bằng.
- [[Biến đổi Einstein]] · [[Thuyết tương đối hẹp]]: giới hạn $v \ll c$ của hệ số $\gamma$.
- [[Thấu kính]] · [[Mắt và các tật của mắt]]: quang học gần trục — góc nhỏ $\approx$ sin, tan.
- [[Sự nở vì nhiệt]]: khai triển bậc nhất theo nhiệt độ.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Đạo hàm]] · [[Tích phân]] · [[Số phức]] (Euler $e^{i\theta} = \cos\theta + i\sin\theta$ là hệ quả của Maclaurin) · [[Phương trình vi phân]] · [[Đại số tuyến tính]]

## Câu hỏi mở

- Chuỗi Taylor của một hàm có thể "không hội tụ" (ví dụ $e^{-1/x^2}$ tại 0) — vậy việc cắt chuỗi bừa bãi có thể sai như thế nào trong vật lý? (Gợi ý: "hàm phẳng" — mọi đạo hàm đều bằng 0 tại điểm khai triển nhưng hàm không phải hằng số.)
- Khi nào phải giữ số hạng bậc hai thay vì chỉ bậc nhất? (Gợi ý: số hạng bậc nhất triệt tiêu do đối xứng — ví dụ thế năng tại cân bằng $V'(0) = 0$.)
- Vì sao phần dư cần $f^{(k+1)}(\xi)$ với $\xi$ "nằm giữa" — và điều đó giới hạn gì cho việc ước lượng sai số khi chỉ biết đạo hàm tại một điểm?