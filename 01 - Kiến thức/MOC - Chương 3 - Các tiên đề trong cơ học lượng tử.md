---
tags:
  - vật-lý/moc
type: moc
created: 2026-09-25
---

# MOC - Chương 3 - Các tiên đề trong cơ học lượng tử

> [!abstract] Mục tiêu chương
> Cơ học lượng tử không bắt đầu từ một phương trình mà từ một bộ tiên đề. Chương này hệ thống hóa bộ tiên đề: trạng thái mang thông tin, đại lượng vật lý là toán tử tự liên hợp, phép đo cho xác suất theo quy tắc Born, và từ đó suy ra giới hạn đo đồng thời cùng hệ thức bất định Heisenberg.

## Bản đồ chương

| Phần | Vấn đề trung tâm | Kết quả then chốt |
| --- | --- | --- |
| 1 | Vì sao cần bộ tiên đề? | Cơ học lượng tử như một bộ luật dự đoán, không phải một phương trình sóng |
| 2 | Trạng thái chứa thông tin gì? | Vector trạng thái trong không gian Hilbert, hàm sóng là biểu diễn của nó |
| 3 | Đại lượng vật lý được biểu diễn thế nào? | Toán tử tự liên hợp trên miền tác dụng |
| 4 | Phép đo cho biết điều gì? | Trị riêng, xác suất Born, cập nhật trạng thái, trị trung bình |
| 5 | Có thể đo đồng thời hai đại lượng không? | Hàm riêng chung và điều kiện commutator bằng không |
| 6 | Giới hạn độ chính xác là gì? | Robertson, Robertson–Schrödinger và bất định tọa độ–xung lượng |

## Ký hiệu dùng trong chương

- $\mathcal H$: không gian Hilbert của các trạng thái.
- $|\psi\rangle$: trạng thái chuẩn hóa; $\langle\phi|$: bra liên hợp.
- $\hat A$: toán tử đại diện cho đại lượng vật lý $A$.
- $\mathcal D(\hat A)$: miền tác dụng của toán tử.
- $\hat P_a$: toán tử chiếu lên kết quả đo $a$.
- $[\hat A,\hat B]=\hat A\hat B-\hat B\hat A$: commutator.
- $\Delta\hat A=\hat A-\langle A\rangle I$: toán tử sai lệch.

> [!warning] Quy ước quan trọng
> Trạng thái vật lý là một **điểm trên tia** của $\mathcal H$: $|\psi\rangle$ và $e^{i\theta}|\psi\rangle$ mô tả cùng một trạng thái. Vì vậy không thể coi mọi vector khác 0 là trạng thái, và không thể gắn trực giác “vị trí trong không gian” cho ket.

---

## 1. Mở đầu

### 1.1. Vì sao không thể bắt đầu bằng một phương trình

Cơ học cổ điển bắt đầu từ định luật Newton $m\vec a=\vec F$ và dự đoán chắc chắn vị trí tại mọi thời điểm. Cơ học lượng tử bắt đầu tự hỏi: **một trạng thái vật lý được mã hóa thế nào**, và **phép đo trích ra loại thông tin gì từ nó**. Câu hỏi này không có câu trả lời bằng một phương trình duy nhất, vì phương trình Schrödinger chỉ cho ta biết trạng thái tiến hóa **giữa** hai lần đo, không cho ta biết trạng thái ban đầu hay cách đo nó.

### 1.2. Vai trò của bộ tiên đề

Bộ tiên đề đóng hai vai trò:

- **Tính đầy đủ:** nó chỉ ra mọi thứ mà lý thuyết cần phải có, không cần thêm giả định ẩn.
- **Tính kiểm chứng:** mỗi tiên đề đều gắn với một loại thực nghiệm kiểm tra được.

Bảng dưới đây tóm tắt bốn tiên đề mà chương này sẽ mở rộng từ A1–A5 trong [[Tiên đề cơ học lượng tử]]:

| Mã | Tiên đề | Nội dung ngắn |
| --- | --- | --- |
| I | Trạng thái và thông tin | Trạng thái là vector đơn vị trong $\mathcal H$ |
| II | Các đại lượng động lực | Đại lượng vật lý là toán tử tự liên hợp |
| III | Tính chất thống kê | Phép đo cho trị riêng với xác suất Born |
| — | Suy ra (không phải tiên đề) | Bất định Heisenberg là **hệ quả** của I–III cộng với giao hoán |

> [!note] Một điểm dễ nhầm
> Tiên đề I dùng từ **trạng thái** chứ không dùng từ **vật thể**. Vật thể là một hệ nhiều hạt có thể ở trong chồng chất của nhiều trạng thái; bản thân “vật thể” không phải là một vector trong $\mathcal H$ của một hạt.

Xem [[Hàm sóng]] và [[Không gian Hilbert]] cho phần hình thức. Khái niệm trạng thái như tia, toán tử mật độ và trạng thái hỗn được trình bày trong [[Trạng thái lượng tử]].

## 2. Tiên đề I: Trạng thái và thông tin

### 2.1. Trạng thái là gì

Trạng thái của một hệ lượng tử tại một thời điểm là một vector đơn vị:

$\langle\psi|\psi\rangle=1$,

trong không gian Hilbert $\mathcal H$. Trong biểu diễn tọa độ, vector này được viết thành hàm sóng $\psi(\vec r,t)$, và cùng một trạng thái có thể có nhiều biểu diễn khác nhau tùy cơ sở.

### 2.2. Thông tin nằm ở đâu

Thông tin về hệ **không nằm trong giá trị của ψ**, mà nằm trong cách ψ biểu diễn được trong một cơ sở đã chọn. Chẳng hạn, trong cơ sở vị trí, biên độ $\psi(\vec r,t)$ cho biết phân bố vị trí; trong cơ sở năng lượng, các hệ số khai triển cho biết phân bố năng lượng. Cùng một trạng thái, nhưng hai bản tóm tắt khác nhau.

Biểu diễn theo cơ sở trạng thái riêng của $\hat A$ là:

$|\psi\rangle=\sum_n c_n|a_n\rangle$;

trong đó các hệ số $c_n$ là biên độ chồng chất với các trạng thái riêng. Xem [[Ký hiệu Dirac]].

### 2.3. Chồng chất và tính đơn vị

Điều kiện chuẩn hóa $\sum_n|c_n|^2=1$ (hoặc $\int|\psi|^2\,d^3r=1$) nói rằng tổng xác suất của mọi kết quả có thể xảy ra bằng 1. Chồng chất cho phép nhiều kết quả cùng có xác suất khác 0 trong cùng một trạng thái — đây là điểm khác biệt căn bản với trực giác cổ điển. Xem [[Nguyên lý chồng chất lượng tử]].

## 3. Tiên đề II: Các đại lượng động lực

### 3.1. Đại lượng vật lý như một toán tử

Mỗi đại lượng vật lý quan sát được, như năng lượng hay mô-men động lượng, được gắn với một toán tử tuyến tính $\hat A$ trên $\mathcal H$. Bản chất vật lý của tiên đề nằm ở điều kiện tự liên hợp:

$\hat A^\dagger=\hat A$;

điều kiện này bảo đảm trị riêng là số thực và kỳ vọng là số thực, tức là phép đo có xác suất không âm. Xem [[Toán tử trong cơ học lượng tử]].

### 3.2. Miền tác dụng

Với toán tử không bị chặn như $\hat x$ hay $\hat p$, không phải mọi hàm vuông giao đều được phép tác dụng. Toán tử được xác định trên một miền con $\mathcal D(\hat A)$; các điều kiện biên quyết định miền này. Xem [[Các toán tử cơ bản trong cơ học lượng tử]].

### 3.3. Bảng đối chiếu đại lượng và toán tử

| Đại lượng vật lý | Toán tử | Ghi chú |
| --- | --- | --- |
| Tọa độ | $\hat x_j\psi=x_j\psi$ | phép nhân |
| Xung lượng | $\hat p_x=-i\hbar\dfrac{\partial}{\partial x}$ | toán tử vi phân |
| Năng lượng | $\hat H=\hat{\mathbf p}^{\,2}/(2m)+V$ | Hamiltonian |
| Mô-men xung lượng | $\hat{\mathbf L}=\hat{\mathbf r}\times\hat{\mathbf p}$ | toán tử giả (pseudo-vector) |

Các hệ thức giao hoán giữa những toán tử này sẽ quyết định phần 5 và 6 của chương.

## 4. Tiên đề III: Tính chất thống kê trong lượng tử

### 4.1. Phép đo cho trị riêng

Khi đo đại lượng $\hat A$ trên hệ đang ở trạng thái $|\psi\rangle$, kết quả đo chỉ có thể là một trị riêng của $\hat A$:

$\hat A|a_n\rangle=a_n|a_n\rangle$.

Điểm mấu chốt: tập các kết quả đo **không** phải một danh sách đóng trước bởi lý thuyết, mà là tập trị riêng của toán tử tương ứng. Với toán tử có phổ rời rạc, đó là một tập đếm được; với toán tử có phổ liên tục, đó là một tập dữ liệu liên tục. Đây là nội dung của hai mục kế tiếp.

### 4.2. Trường hợp đại lượng động lực có phổ trị riêng gián đoạn

Khi phổ rời rạc, trạng thái khai triển trong cơ sở trực chuẩn gồm các hàm riêng:

$|\psi\rangle=\sum_n c_n|a_n\rangle$;

và xác suất đo được trị riêng $a_n$ là **bình phương biên độ**:

$p_n=|c_n|^2=|\langle a_n|\psi\rangle|^2$.

Đây là hình thức rời rạc của quy tắc Born. Ví dụ là mức năng lượng của hạt trong hố thế vô hạn, nơi $n$ chỉ nhận các giá trị nguyên dương.

### 4.3. Trường hợp đại lượng động lực có phổ trị riêng liên tục

Khi phổ liên tục, ví dụ động lượng của hạt tự do, không thể tổng theo chỉ số rời rạc. Thay vào đó dùng mật độ xác suất:

$p(a)=|\langle a|\psi\rangle|^2$;

trong đó $\langle a|\psi\rangle$ là hệ số khai triển theo ket tổng quát hóa $|a\rangle$, và $\langle a|a'\rangle=\delta(a-a')$. Xác suất đo trong một khoảng nhỏ là:

$\mathbb P(a\in[a,a+da])=|c(a)|^2\,da$;

nên xác suất của một điểm đơn lẻ bằng 0. Xem [[Hàm Dirac delta]].

### 4.4. Trị trung bình trong phép đo một đại lượng động lực

Lặp lại cùng một phép chuẩn bị và đo nhiều lần, trung bình các kết quả dẫn tới kỳ vọng toán học:

$\langle A\rangle=\sum_n p_na_n=\langle\psi|\hat A|\psi\rangle$;

với phổ liên tục, tổng được thay bằng tích phân theo mật độ. Kỳ vọng không phải giá trị chắc chắn của một lần đo đơn lẻ, mà là trung tâm của phân bố kết quả. Xem [[Xác suất và trị trung bình]].

### 4.5. Cập nhật trạng thái sau đo

Sau khi đo được kết quả $a$ với xác suất khác 0, trạng thái mới là trạng thái chiếu lên không gian riêng tương ứng:

$|\psi'\rangle=\frac{\hat P_a|\psi\rangle}{\sqrt{p_a}}$.

Đây là nội dung toán tử chiếu. Một phép đo lặp lại ngay sau đó với cùng thiết bị cho kết quả chắc chắn là $a$. Chi tiết về toán tử chiếu, phép đo tổng quát và đo lặp lại: [[Phép đo lượng tử]].

> [!example] Cập nhật trạng thái qua toán tử chiếu
> Với $\hat P_a=|a\rangle\langle a|$, ta có $\hat P_a^2=\hat P_a=\hat P_a^\dagger$, nên toán tử chiếu là một phép chiếu vuông góc idempotent. Nếu trạng thái ban đầu là chồng chất của nhiều trị riêng, phép đo sẽ loại bỏ các thành phần trực giao với kết quả.

## 5. Sự đo đồng thời các đại lượng động lực

### 5.1. Khái niệm hàm riêng chung

Nếu một hàm $|u\rangle$ thỏa mãn đồng thời:

$\hat A|u\rangle=a|u\rangle$ và $\hat B|u\rangle=b|u\rangle$;

thì $|u\rangle$ là **hàm riêng chung** của $\hat A$ và $\hat B$, ứng với hai trị riêng $a$ và $b$. Khi đó, một phép đo $\hat A$ cho $a$ và một phép đo $\hat B$ cho $b$ không mâu thuẫn với nhau.

### 5.2. Điều kiện để hai đại lượng động lực đồng thời được xác định

Điều kiện đủ để hai toán tử tự liên hợp có cơ sở hàm riêng chung là chúng giao hoán:

$[\hat A,\hat B]=\hat A\hat B-\hat B\hat A=0$.

Đây là **điều kiện đủ, không phải điều kiện cần**. Hai toán tử không giao hoán vẫn có thể chia sẻ một số hàm riêng chung; ví dụ $\hat L_x$ và $\hat L_z$ không giao hoán ($[\hat L_x,\hat L_z]=-i\hbar\hat L_y$), nhưng trạng thái $l=0$ (orbital $s$) vẫn là hàm riêng chung của cả ba thành phần mô-men xung lượng với trị riêng $0$. Tuy nhiên, khi $[\hat A,\hat B]\neq0$ và phổ rời rạc không suy biến, hai toán tử **không thể** có hệ hàm riêng chung đầy đủ, nên không thể chuẩn bị một trạng thái xác định đồng thời cả $a$ lẫn $b$. Xem [[Toán tử trong cơ học lượng tử]].

### 5.3. Hệ quả: bất định là hệ quả của giao hoán

Khi $[\hat x,\hat p]=i\hbar\neq0$, tọa độ và xung lượng không có hàm riêng chung. Không thể chuẩn bị một trạng thái mà $\Delta x=0$ và $\Delta p=0$ cùng lúc. Đó là hạt giống của hệ thức bất định ở phần 6. Chi tiết về hàm riêng chung và điều kiện giao hoán: [[Đo đồng thời các đại lượng trong cơ học lượng tử]].

## 6. Hệ thức bất định Heisenberg

### 6.1. Độ bất định trong phép đo một đại lượng động lực

Độ bất định của đại lượng $A$ là căn bậc hai của kỳ vọng bình phương sai lệch:

$\Delta A=\sqrt{\langle(\Delta\hat A)^2\rangle}$, với $\Delta\hat A=\hat A-\langle A\rangle I$.

Nó đo mức độ tập trung của phân bố kết quả đo quanh trị trung bình; điều kiện $\Delta A=0$ chỉ xảy ra khi trạng thái là hàm riêng của $\hat A$.

### 6.2. Hệ thức bất định trong phép đo hai đại lượng động lực

Với hai toán tử tự liên hợp có mô-men bậc hai hữu hạn, hệ thức Robertson cho:

$(\Delta A)^2(\Delta B)^2\geq\dfrac14\left|\langle[\hat A,\hat B]\rangle\right|^2$;

và dạng mạnh hơn, Robertson–Schrödinger, thêm phần giao:

$(\Delta A)^2(\Delta B)^2\geq\dfrac14\left|\langle[\hat A,\hat B]\rangle\right|^2+\dfrac14\left|\langle\{\Delta\hat A,\Delta\hat B\}\rangle\right|^2$.

Trạng thái đạt cực tiểu của Robertson là trạng thái mà $\Delta\hat A$ và $\Delta\hat B$ tỉ lệ với nhau. Xem [[Nguyên lý bất định Heisenberg]]. Chứng minh đầy đủ từ bất đẳng thức Cauchy–Schwarz: [[Suy ra hệ thức bất định từ giao hoán]].

### 6.3. Hệ thức bất định giữa tọa độ và xung lượng

Vì $[\hat x,\hat p]=i\hbar$, kỳ vọng của commutator là hằng số tự liên hợp, nên:

$\Delta x\,\Delta p\geq\frac{\hbar}{2}$.

Dấu bằng đạt được bởi các trạng thái Gaussian tối thiểu, ví dụ hàm sóng trạng thái cơ sở của dao động tử. Hệ thức này không nói rằng máy đo kém, mà là hệ quả toán học của việc $\hat x$ và $\hat p$ không giao hoán trên cùng miền. Xem [[Nguyên lý bất định Heisenberg]].

## Mối liên hệ với Chương 1 và Chương 2

- Chương 1 cung cấp **bằng chứng thực nghiệm**: phổ vật đen, hiệu ứng quang điện, tán Compton, lưỡng tính sóng-hạt — mọi bằng chứng này đều được giải thích gọn nhất bởi bộ tiên đề ở chương này.
- Chương 2 cung cấp **ngôn ngữ toán học**: không gian Hilbert, ký hiệu Dirac, toán tử tự liên hợp và phân rã phổ — nền tảng để phát biểu chính xác từng tiên đề.
- Bất định Heisenberg, lưỡng tính sóng-hạt và lượng tử hóa đều là **hệ quả** của bộ tiên đề, không phải tiên đề độc lập.

## Kiểm chứng & giới hạn

- Quy tắc Born và các mức năng lượng rời rạc được kiểm chứng bằng phổ hấp thụ và phổ phát xạ của nguyên tử; xem [[Thí nghiệm - Franck-Hertz]] và [[Quang phổ]].
- Cập nhật trạng thái sau đo được kiểm chứng bằng thí nghiệm lặp lại Stern–Gerlach; xem [[Thí nghiệm - Stern-Gerlach]].
- Bất định Heisenberg được kiểm chứng qua hiệu ứng tán, hiệu ứng Compton và giới hạn độ phân giải thiết bị; xem [[Hiệu ứng Compton]].
- Bộ tiên đề này chỉ mô tả hệ phi tương đối tính, một hạt, không tương tác mạnh với trường. Hệ nhiều hạt cần thêm cấu trúc tích tensor và nguyên lý Pauli; hạt tốc độ cao cần phương trình Dirac.
- Hệ thức Robertson yêu cầu mô-men bậc hai tồn tại và trạng thái nằm trong miền của cả hai toán tử; với các toán tử không bị chặn, điều kiện này không tự động thoả.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[MOC - Chương 1 - Cơ sở vật lý của cơ học lượng tử]]
- [[Cơ sở toán học của cơ học lượng tử]]
- [[Tiên đề cơ học lượng tử]]: note mẹ chứa bộ tiên đề A1–A5.
- [[Trạng thái lượng tử]] · [[Phép đo lượng tử]] · [[Đo đồng thời các đại lượng trong cơ học lượng tử]] · [[Suy ra hệ thức bất định từ giao hoán]]: các note nền tảng của chương.
- [[Hàm sóng]] · [[Nguyên lý chồng chất lượng tử]] · [[Nguyên lý bất định Heisenberg]]
- [[Không gian Hilbert]] · [[Ký hiệu Dirac]] · [[Toán tử trong cơ học lượng tử]] · [[Các toán tử cơ bản trong cơ học lượng tử]]
- [[Xác suất và trị trung bình]] · [[Hàm Dirac delta]]

## Câu hỏi tự kiểm

1. Vì sao không thể coi “vật thể” là một vector của không gian Hilbert của một hạt?
2. Thông tin về trạng thái nằm ở đâu: trong giá trị của hàm sóng hay trong cách biểu diễn theo cơ sở?
3. Vì sao tiên đề II yêu cầu toán tử tự liên hợp chứ không chỉ là toán tử tuyến tính bất kỳ?
4. Vì sao tập kết quả đo phải là tập trị riêng của toán tử chứ không phải một danh sách dự đoán trước?
5. Trong trường hợp phổ liên tục, vì sao dùng mật độ xác suất thay vì tổng xác suất?
6. Vì sao trị trung bình không phải là kết quả chắc chắn của một phép đo đơn lẻ?
7. Toán tử chiếu giải thích điều gì về cách trạng thái thay đổi sau phép đo?
8. Vì sao $[\hat A,\hat B]=0$ là điều kiện **đủ** chứ không phải điều kiện **cần** cho việc có hàm riêng chung?
9. Vì sao hệ thức bất định Heisenberg là hệ quả của tiên đề chứ không phải một tiên đề độc lập?
10. Khi nào dấu bằng trong hệ thức Robertson được đạt tới, và điều đó nói lên điều gì về trạng thái?
