---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Toán tử trong cơ học lượng tử

> [!abstract] Công cụ để làm gì
> Toán tử là cách biểu diễn một đại lượng quan sát như một phép biến đổi tuyến tính trên không gian trạng thái. Bài toán trị riêng của toán tử cho biết những kết quả đo có thể xảy ra; tính tự liên hợp và trực giao của hệ trị riêng bảo đảm xác suất có nghĩa vật lý.

## Khái niệm toán tử

Một toán tử $\hat A$ là ánh xạ tuyến tính từ miền $\mathcal D(\hat A)$ trong không gian Hilbert $\mathcal H$ sang một không gian đích:

$\hat A:\mathcal D(\hat A)\to\mathcal H$.

Trong cơ sở $\{|n\rangle\}$, toán tử có thể biểu diễn bằng ma trận $A_{mn}$:

$A_{mn}=\langle m|\hat A|n\rangle$.

Với toán tử không bị chặn như $\hat p$ hoặc $\hat H$, các hàm sóng được phép tác dụng phải nằm trong miền tác dụng; nếu bỏ qua miền, nhiều phép toán và phép lấy đạo hàm có thể không hợp lệ.

## Các phép toán trên toán tử

| Phép toán | Ký hiệu | Ý nghĩa |
| --- | --- | --- |
| Tổng | $\hat A+\hat B$ | Cộng tác dụng của hai đại lượng |
| Nhân với số | $c\hat A$ | Tập hợp con của các toán tử |
| Hợp (tích toán tử) | $\hat A\hat B$ | Tác dụng tuần tự $\hat B$ rồi $\hat A$; thứ tự có ý nghĩa |
| Liên hợp | $\hat A^\dagger$ | Ánh xạ đi kèm tích vô hướng |
| Commutator | $[\hat A,\hat B]=\hat A\hat B-\hat B\hat A$ | Đo mức không giao hoán |

Tích vô hướng hai vector là một đại lượng vô hướng, không phải một phép toán toán tử mới.

## Hàm riêng và trị riêng

Nếu tồn tại vector khác 0 $|a\rangle$ sao cho:

$\hat A|a\rangle=a|a\rangle$,

thì $|a\rangle$ là hàm hoặc ket riêng, còn $a$ là trị riêng. Các giá trị trả về khi đo đại lượng vật lý là trị riêng của toán tử tương ứng, theo cách diễn giải chuẩn của cơ học lượng tử.

Nếu trạng thái chuẩn bị là:

$|\psi\rangle=\sum_nc_n|a_n\rangle$,

thì xác suất đo $a_n$ là:

$p_n=|c_n|^2=|\langle a_n|\psi\rangle|^2$.

## Suy biện của trị riêng

Một trị riêng có thể có nhiều hàm riêng độc lập. Tập các vector ứng với cùng trị riêng $a$ là một không gian con, gọi là không gian riêng. Trong đó có thể chọn một cơ sở trực chuẩn, chẳng hạn cơ sở riêng của mô-men xung lượng trong trường tâm.

Suy biện không phải lỗi: nó phản ánh nhiều trạng thái độc lập có cùng một giá trị đo được. Với toán tử tự liên hợp, các không gian ứng với các trị riêng khác nhau vẫn trực giao.

## Toán tử tuyến tính

Toán tử $\hat A$ là tuyến tính nếu:

$\hat A(a|\psi\rangle+b|\chi\rangle)=a\hat A|\psi\rangle+b\hat A|\chi\rangle$.

Tính tuyến tính làm cho phương trình Schrödinger và các phép đo đều tôn trọng nguyên lý chồng chất. Một tổ hợp các trạng thái vẫn là một trạng thái hợp lệ, miễn tổ hợp được chuẩn hóa nếu cần.

## Toán tử Hermite

Toán tử $\hat A$ được gọi là Hermite nếu:

$\hat A^\dagger=\hat A$.

Với điều kiện này, các trị riêng có thể chọn là số thực và tích vô hướng $\langle\psi|\hat A|\psi\rangle$ là thực. Đây là điều kiện cơ bản để đại lượng được gắn với một phép đo có xác suất không âm.

Khi miền tác dụng không đơn giản, thuật ngữ toán học chính xác hơn là **tự liên hợp** kèm điều kiện về miền; phân biệt với cách gọi Hermite là cần thiết cho các toán tử không bị chặn.

## Hàm toán tử

Nếu $\hat A|a\rangle=a|a\rangle$, ta định nghĩa hàm của toán tử bằng:

$f(\hat A)|a\rangle=f(a)|a\rangle$.

Nhờ vậy có thể định nghĩa:

$e^{\hat A}$, $\log\hat A$ khi phù hợp, $\hat A^{-1}$ khi 0 không thuộc phổ, và toán tử tiến hóa:

$U(t)=e^{-i\hat Ht/\hbar}$.

Đối với phổ liên tục, định nghĩa được hiểu theo tích phân theo phổ thay vì tổng rời rạc.

## Toán tử nghịch đảo và toán tử đơn nguyên

Toán tử nghịch đảo thỏa:

$\hat A^{-1}\hat A=\hat A\hat A^{-1}=I$;

điều kiện cần thiết là $0$ không thuộc phổ của $\hat A$.

Toán tử đơn nguyên thỏa:

$\hat U^\dagger\hat U=\hat U\hat U^\dagger=I$.

Vì vậy:

$\hat U^{-1}=\hat U^\dagger$;

$\langle U\psi|U\chi\rangle=\langle\psi|\chi\rangle$.

Toán tử đơn nguyên biểu diễn phép biến đổi bảo toàn tích vô hướng, nên bảo toàn tổng xác suất trong các phép biến đổi trạng thái.

## Các tính chất của toán tử Hermite

Đối với toán tử tự liên hợp trên miền thích hợp:

- $\langle\psi|\hat A|\psi\rangle\in\mathbb R$;
- phổ là số thực;
- có thể chọn hệ trị riêng trực giao nếu phổ rời rạc;
- nếu $\hat A\geq0$ thì $\langle\psi|\hat A|\psi\rangle\geq0$;
- nếu $\hat A\geq0$ thì mọi trị riêng của $\hat A$ cũng không âm.

Các tính chất này biến bài toán toán học thành một bài toán đo lường có xác suất thực.

## Điều kiện trực chuẩn của hàm riêng

Với phổ rời rạc, hàm riêng có thể chọn trực chuẩn:

$\langle a_m|a_n\rangle=\delta_{mn}$.

Với phổ liên tục, dùng chuẩn delta:

$\langle p|p'\rangle=\delta(p-p')$;

$\langle x|x'\rangle=\delta(x-x')$.

Do đó $\int_{-\infty}^{+\infty}|\psi(x)|^2dx=1$ là điều kiện chuẩn hóa của hàm sóng. Sóng phẳng không thể chuẩn hóa trên toàn trục, nên phải dùng ket tổng quát hóa.

## Toán tử chiếu

Với ket chuẩn hóa $|a\rangle$:

$\hat P_a=|a\rangle\langle a|$;

$\hat P_a^2=\hat P_a=\hat P_a^\dagger$;

$\operatorname{Ran}\hat P_a=\operatorname{span}\{|a\rangle\}$.

Toán tử chiếu là hình chiếu vuông góc lên một không gian con. Sau khi đo được kết quả $a$, trạng thái được chuẩn hóa theo thành phần chiếu:

$|\psi_a\rangle=\frac{\hat P_a|\psi\rangle}{\sqrt{p_a}}$, với $p_a=|\langle a|\psi\rangle|^2>0$.

Xem [[Ký hiệu Dirac]].

## Kiểm chứng & giới hạn

- Bài toán trị riêng của $\hat H$ giải các mức năng lượng của hố thế, dao động tử và nguyên tử; xem [[Phương trình Schrödinger]].
- Toán tử tự liên hợp trên miền không bị chặn cần phân biệt với một ma trận Hermite hữu hạn; điều kiện biên quyết định cả miền tác dụng lẫn cấu trúc phổ.
- Tích phân theo phổ liên tục không nên bị hiểu là tổng rời rạc của các ket thông thường.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Cơ sở toán học của cơ học lượng tử]]
- [[Không gian Hilbert]] · [[Ký hiệu Dirac]] · [[Đại số tuyến tính]]
- [[Xác suất và trị trung bình]]
- [[Các toán tử cơ bản trong cơ học lượng tử]]
- [[Tiên đề cơ học lượng tử]] · [[Hàm sóng]] · [[Phương trình Schrödinger]] · [[Nguyên lý bất định Heisenberg]]

## Câu hỏi mở

1. Vì sao điều kiện tự liên hợp quan trọng hơn việc toán tử chỉ có các phần tử ma trận thực?
2. Khi nào một trị riêng bị suy biện và làm thay đổi cách chọn cơ sở?
3. Vì sao hàm của một toán tử được định nghĩa tốt nhất bằng phổ của nó?
4. Toán tử chiếu giải thích được điều gì của phép đo và không giải thích được điều gì?
