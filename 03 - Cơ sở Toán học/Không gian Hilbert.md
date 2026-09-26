---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Không gian Hilbert

> [!abstract] Công cụ để làm gì
> Không gian Hilbert là không gian vector phức có tích vô hướng và tính đầy đủ. Nó là không gian trạng thái chuẩn của cơ học lượng tử: hàm sóng là một vector, phép đo được biểu diễn bằng toán tử và khai triển trạng thái là phép tổng hoặc tích phân theo một cơ sở.

## Không gian vector phức

Một không gian vector phức $V$ trên $\mathbb C$ có các phép cộng vector và nhân với số phức, thỏa các tính chất của một không gian vector. Một hệ cơ sở $\{|\alpha\rangle\}_{\alpha\in A}$ cho phép biểu diễn duy nhất:

$|\psi\rangle=\sum_{\alpha\in A}c_\alpha|\alpha\rangle$.

Khi $\psi$ và $\chi$ là hai vector, độ dài, góc và trực giao chỉ có ý nghĩa một cách tự nhiên sau khi bổ sung tích vô hướng. Xem [[Đại số tuyến tính]].

### Tích vô hướng

Với quy ước tuyến tính theo đối số thứ hai, tích vô hướng là:

$\langle\phi|\psi\rangle=\phi^\dagger\psi$;

$\langle\psi|\phi\rangle=\langle\phi|\psi\rangle^*$;

$\langle a\phi+b\chi|\psi\rangle=a^*\langle\phi|\psi\rangle+b^*\langle\chi|\psi\rangle$;

$\langle\psi|a\phi+b\chi\rangle=a\langle\psi|\phi\rangle+b\langle\psi|\chi\rangle$.

Tích vô hướng cho một số phức; vì vậy hệ quy tắc Born dùng bình phương độ lớn:

$|\langle\phi|\psi\rangle|^2=\langle\phi|\psi\rangle\langle\psi|\phi\rangle\geq0$.

Các tính chất còn lại gồm đối xứng liên hợp, dương xác định và bất đẳng thức Cauchy–Schwarz.

## Không gian Hilbert

Không gian Hilbert $\mathcal H$ là một không gian vector phức đầy đủ với tích vô hướng. “Đầy đủ” nghĩa là mọi dãy Cauchy trong $\mathcal H$ đều có một giới hạn thuộc $\mathcal H$.

Dãy Cauchy $(\psi_n)$ thỏa:

$\|\psi_n-\psi_m\|^2=\langle\psi_n-\psi_m|\psi_n-\psi_m\rangle\to0\ \text{khi } m,n\to\infty$.

Điều kiện này bảo đảm các xấp xỉ bằng phép chiếu, chuỗi hội tụ và các phép giới hạn toán học không tạo ra vector “ở ngoài” không gian mô tả.

### Ví dụ: không gian hàm vuông giao

Không gian

$L^2(\mathbb R^3)=\left\{\psi:\int_{\mathbb R^3}|\psi(\vec r)|^2\,d^3r<\infty\right\}$

với tích vô hướng

$\langle\phi|\psi\rangle=\int_{\mathbb R^3}\phi^*(\vec r)\psi(\vec r)\,d^3r$

là một không gian Hilbert sau khi xác định hai hàm bằng nhau nếu chúng khác nhau chỉ trên một tập đo đo bằng không.

Hàm sóng phải thuộc miền phù hợp của từng toán tử khi tính $\hat p$ hoặc $\hat H$; không phải mọi hàm vuông giao đều tự động thuộc miền đạo hàm.

## Ký hiệu Dirac

Ký hiệu Dirac viết ket, bra và tích vô hướng:

$|\psi\rangle$, $\langle\phi|$, $\langle\phi|\psi\rangle$.

Bra là hàm liên hợp của một ket theo quy ước tích vô hướng ở trên. Với toán tử $\hat A$, có thể dùng các phép tương tác:

$\langle\psi|\hat A|\phi\rangle$;

$\langle\psi|\phi\rangle=\psi^\dagger\phi$;

$\hat A^\dagger$ là toán tử liên hợp, thỏa:

$\langle\psi|\hat A|\phi\rangle=\langle\phi|\hat A^\dagger|\psi\rangle^*$.

### Cơ sở rời rạc

Nếu $\{|\alpha\rangle\}_{\alpha\in A}$ là cơ sở trực chuẩn, thì:

$\langle\alpha|\beta\rangle=\delta_{\alpha\beta}$,

$|\psi\rangle=\sum_{\alpha\in A}\langle\alpha|\psi\rangle|\alpha\rangle$;

$\|\psi\|^2=\sum_{\alpha\in A}|\langle\alpha|\psi\rangle|^2$.

Dự án trên một vector $|n\rangle$ là:

$\hat P_n=|n\rangle\langle n|$;

$\hat P_n|\psi\rangle=\langle n|\psi\rangle|n\rangle$.

### Cơ sở liên tục

Trong biểu diễn tọa độ:

$|\psi\rangle=\int dx\,\psi(x)|x\rangle$;

$\psi(x)=\langle x|\psi\rangle$;

$\langle x|x'\rangle=\delta(x-x')$.

Tương tự, trong biểu diễn xung lượng:

$|\psi\rangle=\int dp\,c(p)|p\rangle$;

$\langle p|p'\rangle=\delta(p-p')$.

Các ket $|x\rangle$ và $|p\rangle$ là ket tổng quát hóa; chúng không phải các vector Hilbert chuẩn hóa riêng lẻ. Tính đầy đủ của không gian cho phép biểu diễn và giới hạn các trạng thái thích hợp.

Xem [[Ký hiệu Dirac]] và [[Hàm Dirac delta]].

## Tính chất của tích vô hướng và trực giao

Các tính chất quan trọng là:

- đối xứng liên hợp: $\langle\phi|\psi\rangle^*=\langle\psi|\phi\rangle$;
- dương xác định: $\langle\psi|\psi\rangle\geq0$, và bằng 0 chỉ khi $|\psi\rangle=0$;
- chuẩn: $\|\psi\|=\sqrt{\langle\psi|\psi\rangle}$;
- Cauchy–Schwarz: $|\langle\phi|\psi\rangle|\leq\|\phi\|\|\psi\|$.

Hai ket $|\phi\rangle$ và $|\psi\rangle$ trực giao nếu:

$\langle\phi|\psi\rangle=0$.

Nếu một hệ ket là trực giao và chuẩn, chúng tạo thành một hệ trực chuẩn. Với toán tử tự liên hợp, các hàm riêng ứng với các trị riêng khác nhau có thể được chọn trực giao, kể cả khi có suy biện.

Tích vô hướng cũng giải thích trực giác giao thoa: các biên độ cộng trước khi lấy bình phương, còn xác suất không cộng trực tiếp nếu các trạng thái không trực giao.

## Chiều và cơ sở của không gian Hilbert

Một cơ sở trực chuẩn rời rạc thỏa:

$\langle m|n\rangle=\delta_{mn}$,

$\sum_n|n\rangle\langle n|=I$;

$|\psi\rangle=\sum_n\langle n|\psi\rangle|n\rangle$;

$\|\psi\|^2=\sum_n|\langle n|\psi\rangle|^2$.

Không gian Hilbert vô hạn chiều không được xây dựng chỉ bằng việc lặp lại trực giác hữu hạn chiều: cần xét tích hội tụ trong chuẩn, tính đầy đủ và miền của toán tử.

Với cơ sở liên tục, các tổng được thay bằng tích phân và hệ hoàn chỉnh được hiểu theo nghĩa tích phân. Vì vậy $\delta(x-x')$ là biểu hiện của quan hệ chuẩn giữa các trạng thái vị trí liên tục.

### Tổng hoàn chỉnh

Đối với cơ sở rời rạc, tổng hoàn chỉnh là toán tử đơn vị:

$\sum_n|n\rangle\langle n|=I$.

Với cơ sở liên tục:

$\int dx\,|x\rangle\langle x|=I$;

$\int dp\,|p\rangle\langle p|=I$.

Các tổng và tích phân này cần được hiểu theo nghĩa yếu hoặc theo một thứ tự phân phối phù hợp; chúng không phải tổng điểm thông thường.

## Ý nghĩa vật lý

- **Trạng thái là vector:** $|\psi\rangle$ là một điểm trong $\mathcal H$, còn một hàm sóng là toạ độ của vector trong một cơ sở đã chọn.
- **Quy tắc Born:** xác suất đo trạng thái $|\phi\rangle$ trong $|\psi\rangle$ là $|\langle\phi|\psi\rangle|^2$.
- **Hệ quy tắc Born:** $\langle\psi|\hat A|\psi\rangle$ là trị trung bình lượng tử, không phải trung bình theo thời gian của một quỹ đạo cổ điển.
- **Cơ sở vị trí và xung lượng:** biến đổi Fourier là sự đổi giữa hai cơ sở trong cùng một không gian Hilbert.
- **Bất định Heisenberg:** hệ thức giao hoán giữa tọa độ và xung lượng giới hạn độ chính xác đồng thời của hai đại lượng.
- **Đo lường:** sau khi đo một kết quả, trạng thái được biểu diễn bằng một vector riêng hoặc một tổ hợp trong không gian riêng tương ứng.

## Kiểm chứng & giới hạn

- Tính đầy đủ là lý do dãy hội tụ không dẫn tới một trạng thái “ở ngoài” $\mathcal H$; trong các bài học cơ bản, điều kiện vuông giao và biên thường đủ để biểu diễn hầu hết các hàm sóng.
- Ket liên tục cần phân bố, nên không nên áp dụng trực tiếp các phép tính với vector chuẩn hóa như với một phần tử của cơ sở rời rạc.
- Không phải mọi toán tử đều tự liên hợp; điều kiện miền là thông tin quan trọng khi nghiên cứu toán tử không bị chặn.
- Toán học Hilbert là nền tảng chung; các chi tiết về thời gian, thế năng và nhiều hạt phải được bổ sung bởi các toán tử cụ thể.

## Liên kết

- [[Cơ sở toán học của cơ học lượng tử]]
- [[MOC - Cơ sở Toán học]] · [[Đại số tuyến tính]] · [[Ký hiệu Dirac]] · [[Hàm Dirac delta]]
- [[Tiên đề cơ học lượng tử]] · [[Hàm sóng]] · [[Phương trình Schrödinger]] · [[Nguyên lý bất định Heisenberg]]
- [[Xác suất và trị trung bình]] · [[Toán tử trong cơ học lượng tử]] · [[Các toán tử cơ bản trong cơ học lượng tử]]

## Câu hỏi mở

1. Vì sao một không gian chỉ có phép cộng và nhân vô hướng chưa đủ để trở thành không gian Hilbert?
2. Điều gì thay đổi khi một tổng trạng thái rời rạc được thay bằng một tích phân theo cơ sở liên tục?
3. Vì sao $\delta(x-x')$ phải được hiểu là phân bố chứ không phải một hàm thông thường?
4. Tính đầy đủ giúp lập luận nào về giới hạn của dãy trạng thái?
5. Cơ sở riêng của một toán tử tự liên hợp khác cơ sở của toán tử đó như thế nào khi trị riêng bị suy biện?
