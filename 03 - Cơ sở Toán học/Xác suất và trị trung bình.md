---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Xác suất và trị trung bình

> [!abstract] Công cụ để làm gì
> Xác suất mô tả kết quả của các phép chuẩn bị và đo lặp lại; trị trung bình và phương sai biến kết quả ngẫu nhiên thành những đại lượng có thể so sánh. Trong cơ học lượng tử, quy tắc Born biến biên độ chồng chất thành xác suất, còn toán tử Hermite biến bài toán đo thành bài toán trị riêng.

## Biến cố ngẫu nhiên và xác suất

Một thí nghiệm lặp lại có tập các kết quả có thể xảy ra, gọi là không gian mẫu $\Omega$. Một tập con $E\subseteq\Omega$ là biến cố. Xác suất $\mathbb P(E)$ thỏa:

- $\mathbb P(E)\geq0$;
- $\mathbb P(\Omega)=1$;
- nếu các $E_i$ rời nhau thì $\mathbb P(\bigcup_iE_i)=\sum_i\mathbb P(E_i)$.

Với biến rời rạc $X$ nhận giá trị $x_n$:

$\mathbb P(X=x_n)=p_n\geq0,\qquad\sum_np_n=1$.

Với biến liên tục, dùng mật độ xác suất $p(x)$:

$\mathbb P(X\in[a,b])=\int_a^bp(x)\,dx,\qquad\int_{-\infty}^{+\infty}p(x)\,dx=1$.

Với phân bố liên tục thông thường, xác suất của một điểm đơn lẻ bằng 0. Trong lượng tử, xác suất một kết quả cụ thể có thể bằng 0 mà không có nghĩa là kết quả đó không tồn tại; nó chỉ không được trạng thái đang chuẩn bị sinh ra.

## Đại lượng ngẫu nhiên

Đại lượng ngẫu nhiên là hàm số gắn mỗi kết quả của thí nghiệm với một giá trị. Với phân bố rời rạc:

$\mathbb E[X]=\sum_n p_nx_n$;

với phân bố liên tục:

$\mathbb E[X]=\int_{-\infty}^{+\infty}xp(x)\,dx$.

Một biến ngẫu nhiên nói chung có thể phức, nhưng đại lượng vật lý quan sát được phải được gắn với toán tử tự liên hợp nên trị trung bình của nó là số thực.

Trong cơ học lượng tử, hàm sóng $\psi(x)$ không phải là một giá trị của đại lượng. Nó là biểu diễn của trạng thái; giá trị trung bình được tính bằng toán tử đại lượng trên trạng thái đó.

## Trị trung bình trong phép đo một đại lượng ngẫu nhiên

Giả sử đại lượng $A$ có các kết quả đo $a_n$ với xác suất $p_n$. Khi lặp lại cùng một cách chuẩn bị trạng thái:

$\langle A\rangle=\sum_np_na_n$.

Trong cơ sở trạng thái riêng:

$|\psi\rangle=\sum_nc_n|a_n\rangle,\qquad\sum_n|c_n|^2=1$;

$p_n=|c_n|^2=|\langle a_n|\psi\rangle|^2$;

$\langle A\rangle=\sum_np_na_n=\langle\psi|\hat A|\psi\rangle$.

Trong cơ sở tọa độ:

$\langle A\rangle=\int_{\mathbb R^3}\psi^*(\vec r)\,\hat A\,\psi(\vec r)\,d^3r$.

Đây là trung bình của một tập thống kê các lần chuẩn bị giống nhau. Một phép đo đơn lẻ có thể cho một kết quả khác trung bình; trị trung bình không phải dự đoán chắc chắn cho từng sự kiện.

## Độ lệch ra khỏi trị trung bình

Với kết quả đo rời rạc $a_n$, độ lệch là:

$\delta a_n=a_n-\langle A\rangle$.

Bình phương độ lệch tương ứng là:

$\delta a_n^2=(a_n-\langle A\rangle)^2$.

Trong ngôn ngữ toán tử, đặt:

$\Delta\hat A=\hat A-\langle A\rangle I$.

$\Delta\hat A$ là toán tử sai lệch, còn độ lệch chuẩn là số:

$\Delta A=\sqrt{\langle(\Delta\hat A)^2\rangle}$.

Vì vậy không nên đồng nhất ký hiệu $\Delta\hat A$ với $\Delta A$ khi đang nói về toán tử và đại lượng đo được.

## Trị trung bình của bình phương độ lệch

Phương sai là trị trung bình của bình phương độ lệch:

$(\Delta A)^2=\mathbb E[(A-\mathbb E[A])^2]=\langle A^2\rangle-\langle A\rangle^2$.

Với toán tử tự liên hợp, phương sai là số thực không âm. Khi các đại lượng giao hoán, phương sai riêng mô tả được độ rộng phân bố kết quả của từng phép đo. Khi chúng không giao hoán, cần xét thêm commutator và phần giao.

Bất định Heisenberg là một hệ quả:

$\Delta x\,\Delta p_x\geq\frac{\hbar}{2}$.

Tổng quát hơn, Robertson–Schrödinger cho:

$(\Delta A)^2(\Delta B)^2\geq\frac14|\langle[\hat A,\hat B]\rangle|^2+\frac14|\langle\{\Delta\hat A,\Delta\hat B\}\rangle|^2$.

## Ví dụ rời rạc

Giả sử một phép đo có hai kết quả $A=+1$ và $A=-1$ với xác suất lần lượt là $p_+=0{,}7$ và $p_-=0{,}3$. Khi đó:

$\langle A\rangle=0{,}7(1)+0{,}3(-1)=0{,}4$;

$\langle A^2\rangle=1$;

$(\Delta A)^2=1-0{,}4^2=0{,}84$, nên $\Delta A\approx0{,}917$.

Kết quả trung bình không có nghĩa mỗi lần đo đều cho $0{,}4$; nó là giá trị trung tâm của phân bố kết quả.

## Quan hệ với cơ học lượng tử

- Quy tắc Born: $p_n=|\langle a_n|\psi\rangle|^2$ là bước chuyển từ biên độ phức sang xác suất thực.
- Trị trung bình: $\langle\hat A\rangle=\langle\psi|\hat A|\psi\rangle$ là cách tính trung bình lượng tử.
- Phương sai và bất định: phương sai cho biết mức tập trung của kết quả quanh trung bình, còn giao hoán quyết định giới hạn tối thiểu.
- Quy tắc lặp lại nhiều lần là cầu nối giữa xác suất toán học và định luật số lớn, nhưng một trạng thái lượng tử không có sẵn quỹ đạo cổ điển để lấy trung bình theo thời gian.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Cơ sở toán học của cơ học lượng tử]]
- [[Xác suất thống kê]] — xác suất và định luật số lớn trong vật lý nhiệt.
- [[Không gian Hilbert]] — không gian trạng thái và tích vô hướng.
- [[Ký hiệu Dirac]] — biểu diễn các hệ số xác suất bằng bra–ket.
- [[Toán tử trong cơ học lượng tử]] — quan hệ giữa toán tử, trị riêng và trị trung bình.
- [[Hàm sóng]] · [[Tiên đề cơ học lượng tử]] · [[Nguyên lý bất định Heisenberg]]

## Câu hỏi mở

1. Vì sao xác suất lượng tử không thể được giải thích hoàn toàn như “chúng ta chưa biết trạng thái chính xác”?
2. Vì sao phương sai của một toán tử Hermite luôn là số thực không âm?
3. Hai đại lượng không giao hoán có thể có phương sai tùy ý nhỏ không?
4. Phần giao trong Robertson–Schrödinger phản ánh điều gì về trạng thái lượng tử?
