---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Cơ sở toán học của cơ học lượng tử

> [!abstract] Mục tiêu chương
> Chương này xây dựng ngôn ngữ toán học cần thiết để biến các quan sát vật lý thành dự đoán chính xác: xác suất cho kết quả đo, không gian Hilbert cho trạng thái, toán tử tự liên hợp cho đại lượng quan sát và hệ thức giao hoán cho tính bất định.

## Bản đồ chương

| Phần | Vấn đề trung tâm | Công cụ hoặc kết quả then chốt |
| --- | --- | --- |
| 1 | Làm sao mô tả kết quả đo ngẫu nhiên? | Xác suất, trị trung bình, phương sai và quy tắc Born |
| 2 | Trạng thái lượng tử sống ở đâu? | Không gian vector phức, tích vô hướng, không gian Hilbert, cơ sở và ký hiệu Dirac |
| 3 | Đại lượng quan sát được biểu diễn thế nào? | Toán tử, trị riêng, toán tử tự liên hợp, hàm toán tử và toán tử chiếu |
| 4 | Các toán tử vật lý cơ bản là gì? | $\hat x$, $\hat p$, $\hat H$, $\hat L$ và các hệ thức giao hoán |

## Mục tiêu học tập

Sau chương này, cần phân biệt được:

1. xác suất cổ điển với xác suất lượng tử;
2. giá trị trung bình của một phép đo với giá trị trung bình theo thời gian của một quỹ đạo;
3. không gian Hilbert với một không gian vector chưa đầy đủ;
4. toán tử tự liên hợp với toán tử chỉ đơn giản là ma trận;
5. hệ thức giao hoán với bất định Heisenberg.

## Ký hiệu dùng trong chương

- $\mathcal H$: không gian Hilbert của các trạng thái.
- $|\psi\rangle$: ket, một vector trạng thái.
- $\langle\phi|$: bra, là toán tử liên hợp của ket $|\phi\rangle$.
- $\langle\phi|\psi\rangle$: tích vô hướng, vừa là biên độ chồng chất vừa là cơ sở của xác suất.
- $\hat A$: toán tử đại diện cho đại lượng quan sát $A$.
- $\langle A\rangle=\langle\psi|\hat A|\psi\rangle$: trị trung bình lượng tử.
- $(\Delta A)^2=\langle(\hat A-\langle A\rangle I)^2\rangle$: phương sai.
- $\mathcal D(\hat A)$: miền tác dụng của toán tử.
- $[\hat A,\hat B]=\hat A\hat B-\hat B\hat A$: commutator.

> [!warning] Quy ước quan trọng
> Không gọi mọi vector trong một không gian vector đều là trạng thái lượng tử. Trạng thái vật lý là vector **đơn vị** trong $\mathcal H$, còn các đại lượng đo được phải được biểu diễn bởi toán tử tự liên hợp, thường được gọi ngắn gọn là toán tử Hermite.

---

## 1. Xác suất và trị trung bình

### 1.1. Biến cố ngẫu nhiên và xác suất

Một thí nghiệm lặp lại có một tập các kết quả có thể xảy ra, gọi là không gian mẫu $\Omega$. Mỗi tập con $E\subseteq\Omega$ là một biến cố. Xác suất là một hàm $\mathbb P(E)$ thỏa các tính chất:

- $\mathbb P(E)\geq0$;
- $\mathbb P(\Omega)=1$;
- xác suất các biến cố không chồng lấy cộng được: $\mathbb P(\bigcup_i E_i)=\sum_i\mathbb P(E_i)$ khi các $E_i$ rời nhau.

Với biến rời rạc $X$ nhận các giá trị $x_n$, phân bố chuẩn hóa có dạng:

$\mathbb P(X=x_n)=p_n\geq0,\qquad\sum_n p_n=1$.

Với biến liên tục, xác suất được biểu diễn bằng mật độ $p(x)$:

$\mathbb P(X\in[a,b])=\int_a^b p(x)\,dx,\qquad\int_{-\infty}^{+\infty}p(x)\,dx=1$.

Trong cơ học lượng tử, xác suất không chỉ là cách che giấu sự thiếu thông tin. Quy tắc Born là quy luật về cách một trạng thái đã chuẩn bị sinh ra các kết quả đo.

Xem [[Xác suất và trị trung bình]] và [[Xác suất thống kê]].

### 1.2. Đại lượng ngẫu nhiên

Đại lượng ngẫu nhiên là một hàm số gắn mỗi kết quả của thí nghiệm với một giá trị. Nếu $X$ nhận giá trị $x_n$ với xác suất $p_n$, trị trung bình là:

$\mathbb E[X]=\sum_n p_nx_n$.

Với phân bố liên tục:

$\mathbb E[X]=\int_{-\infty}^{+\infty}x\,p(x)\,dx$.

Một đại lượng vật lý lượng tử có thể được gắn với một toán tử Hermite; khi đó trị trung bình phải là số thực, dù hàm sóng và biên độ có thể phức.

### 1.3. Trị trung bình trong phép đo một đại lượng ngẫu nhiên

Giả sử $\hat A|a_n\rangle=a_n|a_n\rangle$, với $\{a_n\}$ là các trị riêng. Nếu trạng thái chuẩn bị là

$|\psi\rangle=\sum_n c_n|a_n\rangle,\qquad\sum_n|c_n|^2=1$,

thì xác suất đo $a_n$ là $|c_n|^2$. Vì vậy:

$p_n=|c_n|^2=|\langle a_n|\psi\rangle|^2$;

$\langle A\rangle=\sum_n p_na_n=\langle\psi|\hat A|\psi\rangle$.

Trong biểu diễn tọa độ:

$\langle A\rangle=\int_{\mathbb R^3}\psi^*(\vec r)\,\hat A\,\psi(\vec r)\,d^3r$.

Trị trung bình ở đây là trung bình trên tập thống kê các lần chuẩn bị cùng một trạng thái, không phải trung bình của một quỹ đạo cổ điển duy nhất.

### 1.4. Độ lệch ra khỏi trị trung bình

Với kết quả đo $a_n$, độ lệch khỏi trị trung bình là $\delta a_n=a_n-\langle A\rangle$. Bình phương độ lệch ngẫu nhiên là:

$\delta a_n^2=(a_n-\langle A\rangle)^2$.

Trong ngôn ngữ toán tử, đặt:

$\Delta\hat A=\hat A-\langle A\rangle I$.

Độ lệch chuẩn không phải một toán tử, mà là căn bậc hai của giá trị trung bình của bình phương độ lệch:

$\Delta A=\sqrt{\langle(\Delta\hat A)^2\rangle}$.

### 1.5. Trị trung bình của bình phương độ lệch

Phương sai là trị trung bình của bình phương độ lệch:

$(\Delta A)^2=\langle A^2\rangle-\langle A\rangle^2$.

Với toán tử tự liên hợp, biểu thức này không âm và là số thực. Khi hai đại lượng không giao hoán, phương sai riêng không đủ để mô tả mọi giới hạn; cần xét cả commutator. Robertson–Schrödinger cung cấp các hệ thức mạnh hơn, trong đó có điều kiện cộng giao.

Bất định Heisenberg là trường hợp đặc biệt:

$\Delta x\,\Delta p_x\geq\frac{\hbar}{2}$.

---

## 2. Không gian Hilbert

### 2.1. Không gian tuyến tính

Không gian vector phức $V$ có các phép cộng vector và nhân với số phức, thỏa các tính chất phân bố và kết hợp. Mỗi hệ cơ sở biểu diễn cùng một vector bằng một bộ toạ độ khác nhau. Xem [[Đại số tuyến tính]].

### 2.2. Không gian Hilbert

Không gian Hilbert là không gian vector phức có tích vô hướng và **đầy đủ**: mọi dãy Cauchy đều có giới hạn trong không gian. Không gian của các hàm vuông giao trên $\mathbb R^3$, ký hiệu $L^2(\mathbb R^3)$, là ví dụ quan trọng cho hàm sóng.

Không gian vector chỉ có tích vô hướng nhưng chưa đầy đủ được gọi là *pre-Hilbert*; tính đầy đủ là điều kiện cần để các giới hạn của chuỗi trạng thái không làm trạng thái vượt ra ngoài miền mô tả.

### 2.3. Ký hiệu Dirac

Ký hiệu Dirac viết trạng thái và toán tử bằng ket, bra:

$|\psi\rangle,\qquad \langle\phi|,\qquad \langle\phi|\psi\rangle$.

Trong cơ sở vị trí liên tục:

$|\psi\rangle=\int dx\,\psi(x)|x\rangle$;

$\psi(x)=\langle x|\psi\rangle$;

$\langle x|x'\rangle=\delta(x-x')$.

Cơ sở vị trí là các ket tổng quát hoá, không phải từng vector Hilbert chuẩn hóa riêng. Xem [[Ký hiệu Dirac]] và [[Hàm Dirac delta]].

### 2.4. Một số tính chất của tích vô hướng

Với quy ước vật lý, tích vô hướng tuyến tính theo đối số thứ hai:

$\langle a\phi+b\chi|\psi\rangle=a^*\langle\phi|\psi\rangle+b^*\langle\chi|\psi\rangle$;

$\langle\psi|a\phi+b\chi\rangle=a\langle\psi|\phi\rangle+b\langle\psi|\chi\rangle$.

Các tính chất còn lại gồm:

- đối xứng liên hợp: $\langle\phi|\psi\rangle^*=\langle\psi|\phi\rangle$;
- dương xác định: $\langle\psi|\psi\rangle\geq0$ và bằng 0 chỉ khi $|\psi\rangle=0$;
- chuẩn: $\|\psi\|=\sqrt{\langle\psi|\psi\rangle}$;
- bất đẳng thức Cauchy–Schwarz: $|\langle\phi|\psi\rangle|\leq\|\phi\|\|\psi\|$.

Hai ket trực giao nếu $\langle\phi|\psi\rangle=0$.

### 2.5. Chiều và cơ sở của không gian Hilbert

Một cơ sở trực chuẩn vô hạn có các tính chất:

$\langle m|n\rangle=\delta_{mn},\qquad \sum_n|n\rangle\langle n|=I$.

Khi đó:

$|\psi\rangle=\sum_n\langle n|\psi\rangle|n\rangle$;

$\| \psi \|^2=\sum_n|\langle n|\psi\rangle|^2$.

Với cơ sở liên tục, tổng được thay bằng tích phân. Không gian Hilbert dùng trong cơ học lượng tử thường có chiều vô hạn đếm được; khái niệm “số chiều” lúc này cần được hiểu theo nghĩa đại số, không phải đếm trực tiếp các hướng trong không gian Euclid.

---

## 3. Toán tử trong cơ học lượng tử

### 3.1. Khái niệm toán tử

Toán tử $\hat A$ là một ánh xạ tuyến tính từ một miền $\mathcal D(\hat A)$ trong không gian Hilbert sang không gian đích. Trong toán học, cần ghi miền tác dụng; trong các bài toán cơ bản thường bỏ qua chi tiết này và coi toán tử là hàm tác dụng trên một miền con đủ rộng.

### 3.2. Các phép toán trên toán tử

Các phép toán chính gồm tổng, nhân với số, hợp (tích toán tử), liên hợp và commutator:

$\hat A+\hat B$, $c\hat A$, $\hat A\hat B$, $\hat A^\dagger$, $[\hat A,\hat B]$.

Tích của hai toán tử mô tả hai phép biến đổi liên tiếp, nên thứ tự thành phần có ý nghĩa: $\hat p=-i\hbar\partial_x$ biến hàm sóng thành đạo hàm của nó, còn $\hat H=\hat p^2/(2m)+V$ biến hàm sóng thành vế phải của phương trình Schrödinger.

### 3.3. Hàm riêng và trị riêng

Nếu:

$\hat A|a_n\rangle=a_n|a_n\rangle$,

thì $|a_n\rangle$ là hàm riêng hoặc ket riêng, còn $a_n$ là trị riêng. Trong cơ học lượng tử, các trị riêng của một đại lượng đo được là các kết quả đo có thể xảy ra.

### 3.4. Sự suy biến của trị riêng

Một trị riêng $a$ có thể ứng với nhiều ket riêng độc lập. Không gian riêng ứng với $a$ được gọi là eigenspace. Trong eigenspace cần chọn một cơ sở trực chuẩn; cách chọn cơ sở không phải duy nhất, nhưng các trị riêng khác nhau vẫn cho các không gian trực giao.

### 3.5. Toán tử tuyến tính

Tính chất tuyến tính là:

$\hat A(a|\psi\rangle+b|\chi\rangle)=a\hat A|\psi\rangle+b\hat A|\chi\rangle$.

Tuyến tính làm cho phương trình tiến hóa và nguyên lý chồng chất có dạng phù hợp; một tổ hợp các trạng thái vẫn là một trạng thái hợp lệ.

### 3.6. Toán tử Hermite

Điều kiện liên hợp là:

$\hat A^\dagger=\hat A$.

Với toán tử tự liên hợp, các trị riêng có thể chọn là số thực và các hàm riêng ứng với trị riêng khác nhau có thể trực giao. Khi miền tác dụng không đơn giản, thuật ngữ toán học chính xác hơn là **tự liên hợp** kèm điều kiện về miền; “Hermite” là cách gọi thông dụng trong vật lý.

### 3.7. Hàm toán tử

Với một toán tử tự liên hợp, hàm của toán tử được định nghĩa trên các hàm riêng:

$f(\hat A)|a_n\rangle=f(a_n)|a_n\rangle$.

Nhờ đó có thể định nghĩa các hàm như $e^{\hat A}$ và $\hat A^{-1}$ (khi phổ không chứa 0), cũng như toán tử tiến hóa thời gian

$e^{-i\hat Ht/\hbar}$

trong [[Phương trình Schrödinger]].

### 3.8. Toán tử nghịch đảo và toán tử đơn nguyên

Toán tử nghịch đảo thỏa $\hat A^{-1}\hat A=I$ và $\hat A\hat A^{-1}=I$ nếu phổ không chứa 0. Một toán tử đơn nguyên thỏa:

$\hat U^\dagger\hat U=\hat U\hat U^\dagger=I$;

khi đó $\hat U^{-1}=\hat U^\dagger$ và $\hat U$ bảo toàn tích vô hướng, tức là bảo toàn xác suất.

### 3.9. Các tính chất của toán tử Hermite

Toán tử tự liên hợp có các tính chất quan trọng:

- $\langle\psi|\hat A|\psi\rangle$ là số thực;
- phổ trị riêng là số thực;
- với phổ rời rạc, có thể chọn hệ hàm riêng trực chuẩn;
- $\langle\phi|\hat A|\phi\rangle\geq0$ nếu $\hat A$ dương;
- nếu $\hat A\geq0$ thì mọi trị riêng của $\hat A$ cũng không âm.

### 3.10. Điều kiện trực chuẩn của hàm riêng

Với phổ rời rạc, chọn:

$\langle a_m|a_n\rangle=\delta_{mn}$.

Với phổ liên tục, các hàm riêng thường được chuẩn hóa theo delta, ví dụ $\langle p|p'\rangle=\delta(p-p')$, thay vì tích phân từ $-\infty$ đến $+\infty$ bằng 1. Tổng hoàn chỉnh $\sum_n|a_n\rangle\langle a_n|=I$ chỉ dùng cho phổ rời rạc; với phổ liên tục phải dùng tích phân.

### 3.11. Toán tử chiếu

Với một ket đã chuẩn hóa $|a\rangle$, toán tử chiếu là:

$\hat P_a=|a\rangle\langle a|$.

Nó thỏa:

$\hat P_a^2=\hat P_a=\hat P_a^\dagger$;

và $\hat P_a|\psi\rangle$ là thành phần của trạng thái trong hướng $|a\rangle$. Sau khi đo được kết quả $a$ với xác suất khác 0, trạng thái mới là $\hat P_a|\psi\rangle/\sqrt{p_a}$.

Xem [[Toán tử trong cơ học lượng tử]].

---

## 4. Các toán tử cơ bản trong cơ học lượng tử

### 4.1. Toán tử tọa độ

Trong cơ sở vị trí:

$\hat x_j\psi(x)=x_j\psi(x)$, hoặc $\hat{\mathbf r}\psi(\vec r)=\vec r\,\psi(\vec r)$.

Vị trí là ví dụ đơn giản nhất về một toán tử nhân với tọa độ. Tọa độ liên tục không phải một tập trị riêng chuẩn hóa theo nghĩa thông thường; nó dùng các ket tổng quát hóa $|\vec x\rangle$.

### 4.2. Toán tử xung lượng

Trong không gian tọa độ:

$\hat p_x=-i\hbar\dfrac{\partial}{\partial x}$, $\hat{\mathbf p}=-i\hbar\nabla$.

Sóng phẳng $e^{ipx/\hbar}$ là ket tổng quát hóa của động lượng. Điều kiện biên quyết định các trạng thái riêng hợp lệ, ví dụ điều kiện tuần hoàn hoặc biên Dirichlet.

### 4.3. Toán tử năng lượng

Với một hạt phi tương đối tính trong trường thế $V(\vec r,t)$:

$\hat H=\hat{\mathbf p}^{\,2}/(2m)+V(\vec r,t)=-\dfrac{\hbar^2}{2m}\nabla^2+V(\vec r,t)$.

Phương trình Schrödinger:

$i\hbar\dfrac{\partial}{\partial t}|\psi\rangle=\hat H|\psi\rangle$.

Nếu $\hat H$ không phụ thuộc thời gian, các trạng thái riêng thỏa $\hat H|E\rangle=E|E\rangle$ và mô tả năng lượng tĩnh.

### 4.4. Toán tử mô-men xung lượng

Toán tử mô-men xung lượng orbital là:

$\hat{\mathbf L}=\hat{\mathbf r}\times\hat{\mathbf p}=-i\hbar\vec r\times\nabla$.

Trong hệ tọa độ, các thành phần có dạng $\hat L_x=-i\hbar(y\partial_z-z\partial_y)$ và các hoán vị của nó. Chúng thỏa:

$[\hat L_i,\hat L_j]=i\hbar\varepsilon_{ijk}\hat L_k$.

Với hệ quanh gốc, các số lượng tử orbital là $l=0,1,2,\ldots$ và $m_l=-l,\ldots,l$.

### 4.5. Hệ thức giao hoán giữa các toán tử

| Cặp toán tử | Hệ thức giao hoán | Ý nghĩa |
| --- | --- | --- |
| Tọa độ–tọa độ | $[\hat x_i,\hat x_j]=0$ | Các hướng tọa độ giao hoán |
| Xung lượng–xung lượng | $[\hat p_i,\hat p_j]=0$ | Các thành phần xung lượng giao hoán |
| Tọa độ–xung lượng | $[\hat x_i,\hat p_j]=i\hbar\delta_{ij}$ | Không thể chuẩn bị vị trí và xung lượng cùng xác định |
| Mô-men xung lượng | $[\hat L_i,\hat L_j]=i\hbar\varepsilon_{ijk}\hat L_k$ | Các phép quay không giao hoán như các toán tử ma trận |
| Động lượng–Hamilton | $[\hat H,\hat p_i]=i\hbar\,\partial_iV$ — đúng với mọi thế tĩnh $V=V(\vec r)$ khi $m$ hằng | Chỉ giao hoán khi $\partial_iV=0$ |

Hệ thức Robertson–Schrödinger cho hai toán tử tự liên hợp có mô-men bậc hai hữu hạn:

$(\Delta A)^2(\Delta B)^2\geq\dfrac14|\langle[\hat A,\hat B]\rangle|^2+\dfrac14\left|\langle\{\hat A-\langle A\rangle I,\hat B-\langle B\rangle I\}\rangle\right|^2$.

Xem [[Các toán tử cơ bản trong cơ học lượng tử]].

---

## Mối liên hệ với Chương 1

- Phổ vật đen và xác suất: [[Giả thuyết - Lượng tử năng lượng Planck]] dùng trạng thái dao động tử và phân bố nhiệt.
- Quy tắc Born: xác suất lượng tử là xác suất của biên độ chồng chất, không phải trung bình thống kê của một quỹ đạo cổ điển.
- Hàm sóng: $\psi(x)$ là biểu diễn của một vector trạng thái trong cơ sở vị trí; xem [[Hàm sóng]].
- Hệ thức giao hoán: $[\hat x,\hat p]=i\hbar$ là nguồn gốc toán học của [[Nguyên lý bất định Heisenberg]].
- Phương trình Schrödinger: là phép tiến hóa bằng toán tử Hamiltonian trong không gian Hilbert.

## Kiểm chứng & giới hạn

- Các trị riêng rời rạc là mức năng lượng của hố thế, dao động tử và nguyên tử; xem [[Phương trình Schrödinger]].
- Trong không gian vô hạn chiều, nhiều toán tử vật lý là toán tử không bị chặn và cần xét miền tác dụng, không chỉ xét công thức trên giấy.
- Ký hiệu Dirac với $|x\rangle$ và các hàm riêng của phổ liên tục dùng phân bố, không phải hàm thông thường.
- Hệ thức giao hoán chỉ trực tiếp dùng để suy ra bất định khi mô-men bậc hai tồn tại và trạng thái nằm trong miền của các toán tử.
- Cơ sở toán học này là nền cho cơ học lượng tử phi tương đối tính; hạt nhanh và hệ nhiều hạt cần các mở rộng như Dirac hoặc lý thuyết trường.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[MOC - Cơ sở Toán học]]
- [[MOC - Chương 1 - Cơ sở vật lý của cơ học lượng tử]]
- [[Xác suất và trị trung bình]]
- [[Không gian Hilbert]]
- [[Ký hiệu Dirac]]
- [[Toán tử trong cơ học lượng tử]]
- [[Các toán tử cơ bản trong cơ học lượng tử]]
- [[Tiên đề cơ học lượng tử]] · [[Hàm sóng]] · [[Phương trình Schrödinger]] · [[Nguyên lý bất định Heisenberg]]
- [[Đại số tuyến tính]] · [[Biến đổi Fourier]] · [[Hàm Dirac delta]] · [[Cơ học Hamilton]]

## Câu hỏi tự kiểm

1. Vì sao trị trung bình lượng tử phải được tính trên tập các lần chuẩn bị, không phải bằng cách lấy trung bình một đường truyền?
2. Tích vô hướng có tính chất nào làm cho các trạng thái lượng tử không thể được coi như các số thực đơn giản?
3. Vì sao cần điều kiện đầy đủ của không gian Hilbert?
4. Khác biệt giữa nghiệm của toán tử và một trị riêng đo được là gì?
5. Suy biến trị riêng có làm mất tính trực giao của các trạng thái năng lượng không?
6. Vì sao $\hat p=-i\hbar\partial_x$ là toán tử, không chỉ là một cách viết phép nhân?
7. Hệ thức $[\hat x_i,\hat p_j]=i\hbar\delta_{ij}$ cho biết điều gì về giới hạn đồng thời của hai đại lượng?
8. Vì sao thời gian không được xử lý như một toán tử tự liên hợp đơn giản trong phương trình Schrödinger?
9. Liên hệ giữa toán tử chiếu và quy tắc cập nhật trạng thái sau phép đo là gì?
10. Khi nào cần phân biệt toán tử Hermite với toán tử tự liên hợp theo nghĩa toán học chặt chẽ?
