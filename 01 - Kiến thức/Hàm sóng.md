---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Hàm sóng

> [!abstract] Ý chính
> Hàm sóng $\psi(\mathbf r,t)$ là đại lượng phức mô tả trạng thái lượng tử. Mật độ xác suất đo vị trí là $|\psi|^2$, còn sự chồng chất các biên độ tạo ra giao thoa.

## 1. Phương trình Schrödinger

Đối với hạt phi tương đối tính, bỏ qua spin, phương trình Schrödinger thời gian phụ thuộc là:

$i\hbar\frac{\partial\psi}{\partial t}=-\frac{\hbar^2}{2m}\nabla^2\psi+V(\mathbf r,t)\psi$.

Trong đó:

- $\hbar=h/(2\pi)$;
- $\nabla^2$ là toán tử Laplace;
- $V(\mathbf r,t)$ là thế năng;
- phương trình có tính đến phụ thuộc thời gian.

Phương trình Schrödinger là định nghĩa toán học của sự phát triển trạng thái lượng tử, không phải chỉ là một phương trình sóng kinh điển.

## 2. Hàm sóng của hạt tự do

Với hạt tự do, $V=0$. Trong không gian ba chiều, nghiệm sóng phẳng ứng với động lượng $\mathbf p$ có dạng:

$\Psi_{\mathbf p}(\mathbf r,t)=A\exp\!\left[\frac{i}{\hbar}(\mathbf p\cdot\mathbf r-Et)\right]$,

trong đó $|\mathbf p|=\hbar k$ và $E$ là năng lượng liên quan với pha thời gian.

Hệ quả trực tiếp:

- quan hệ de Broglie: $\lambda=2\pi/k=h/|\mathbf p|$;
- quan hệ Planck: $E=h\nu=\hbar\omega$.

Sóng phẳng mô tả trạng thái có động lượng xác định, nhưng phân bố đều trong không gian và không thể chuẩn hóa trên toàn bộ không gian. Vì vậy trạng thái định xứ thực tế phải là tổng liên hợp của nhiều sóng phẳng: [[Bó sóng lượng tử]].

Khi dùng năng lượng động học trong pha, hằng số $m_0c^2$ có thể bị bỏ vì nó chỉ tạo một pha toàn cục theo thời gian.

## 3. Ý nghĩa thống kê theo quy tắc Born

Xác suất tìm hạt trong thể tích $d^3r$ quanh điểm $\mathbf r$ là:

$dP=|\psi(\mathbf r,t)|^2\,d^3r$.

Xác suất tìm hạt trong miền $V$ là:

$P(\mathbf r\in V,t)=\int_V|\psi(\mathbf r,t)|^2\,d^3r$.

Các điểm chính:

- $\psi$ phức; $|\psi|^2$ là đại lượng thực không âm.
- Một pha toàn cục $e^{i\theta}$ không đổi vật lý: $e^{i\theta}\psi$ có cùng mọi xác suất và cùng kết quả phép đo.
- Không thể đo trực tiếp $\psi$ như một trường vật chất.
- Giao thoa xuất phát từ việc cộng các biên độ trước khi lấy mô đô, không phải từ việc các hạt cơ học cùng truyền sóng vật chất.
- Quy tắc cho xác suất kết quả lặp lại trên cùng trạng thái chuẩn bị; với một hệ đơn lẻ, nó không phải lời tiên đoán chắc chắn từng sự kiện.

## 4. Chuẩn hóa hàm sóng

Một hàm sóng đại lện được chuẩn hóa nếu tổng xác suất tìm hạt bằng một:

$\int_{\text{toàn không gian}}|\psi(\mathbf r,t)|^2\,d^3r=1$.

Nếu $\int|\psi|^2\,d^3r=N$ hữu hạn và khác không, có thể chia $\psi$ cho $\sqrt N$.

Ý nghĩa:

- tổng xác suất bằng một;
- $[|\psi|^2]=L^{-3}$ và $[\psi]=L^{-3/2}$ trong ba chiều;
- phép nhân hàm sóng với một hằng số phức toàn cục không ảnh hưởng vật lý.

Phương trình Schrödinger với Hamiltonian Hermitian bảo toàn chuẩn hóa khi các điều kiện biên cho phép dòng xác suất thoát ra ở biên bằng không.

Đối với thế năng chỉ phụ thuộc vị trí, dòng xác suất là:

$\vec j=\frac{\hbar}{m}\operatorname{Im}(\psi^*\nabla\psi)$,

và nó tuân theo phương trình liên tục:

$\frac{\partial|\psi|^2}{\partial t}+\nabla\cdot\vec j=0$.

## 5. Điều kiện tiêu chuẩn và điều kiện biên

Hàm sóng vật lý phải:

1. **Vuông giao được:** $\int|\psi|^2\,d^3r<\infty$; sau chuẩn hóa, tích phân bằng một.
2. **Đơn trị:** không có hai giá trị khác nhau tại cùng một điểm vật lý.
3. **Đủ trơn tru theo thế năng:** nếu $V$ hữu hạn và liên tục, $\psi$ cùng các đạo hàm cần thiết liên tục; tại điểm có bước nhảy thế năng hữu hạn phải xét điều kiện ghép riêng.
4. **Thỏa điều kiện biên:** ví dụ $\psi=0$ tại tường vô hạn, chu kỳ trên vòng tròn, hoặc tại vô cùng phải vuông giao được và các số hạng dòng biên phải triệt tiêu khi áp dụng bảo toàn dòng xác suất.
5. **Thỏa điều kiện giao tại điểm nhảy thế hữu hạn:** $\psi$ và $\partial\psi/\partial x$ liên tục nếu thế năng chỉ nhảy hữu hạn.

Những điều kiện này loại các nghiệm toán học không thể biểu diễn một trạng thái vật lý.

## 6. Nhận giá trị trung bình

Với đại lượng vật lý $A$ gắn với toán tử $\hat A$:

$\langle A\rangle=\int\psi^*\hat A\psi\,d^3r$,

Với toán tử quan sát tự liên hợp và mô-men bậc hai hữu hạn, sai số chuẩn hóa là:

$\Delta A=\sqrt{\langle A^2\rangle-\langle A\rangle^2}$.

Các toán tử cơ bản gồm:

$\hat x_i=x_i$, $\hat p_i=-i\hbar\frac{\partial}{\partial x_i}$, $\hat H=-\frac{\hbar^2}{2m}\nabla^2+V$.

Hệ quả trực tiếp là bất định Heisenberg: $\Delta x\,\Delta p_x\geq\hbar/2$.

## Kiểm chứng & giới hạn

- Quy tắc Born được kiểm chứng qua thí nghiệm giao thoa, phân bố va chạm và nhiều phép chuẩn bị trạng thái lặp lại.
- Có thể đo phân bố xác suất, không đo trực tiếp $\psi$ hoặc pha toàn cục.
- Hàm sóng trong vật lý lượng tử không phải lời giải của phương trình sóng cổ điển; mối liên hệ với trường cổ điển cần qua giới hạn lượng tử và phương pháp bán cổ điển.
- Nhiều hạt tương tác cần cơ học lượng tử nhiều hạt; lý thuyết trường lượng tử trở nên cần thiết khi có tạo/hủy hạt hoặc mô tả trường ở thang năng lượng cao.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[MOC - Chương 1 - Cơ sở vật lý của cơ học lượng tử]]
- [[Phương trình Schrödinger]]
- [[Bó sóng lượng tử]]
- [[Tiên đề cơ học lượng tử]]
- [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]: MOC Chương 3 — hàm sóng là biểu diễn tọa độ của tiên đề I.
- [[Trạng thái lượng tử]]: khái niệm trạng thái, toán tử mật độ, trạng thái hỗn.
- [[Nguyên lý bất định Heisenberg]]
- [[Nguyên lý chồng chất lượng tử]]
- [[Xác suất thống kê]]
- [[Biến đổi Fourier]]
- [[Không gian Hilbert]]

## Câu hỏi mở

- Vì sao thay đổi pha toàn cục của $\psi$ không ảnh hưởng xác suất nhưng một pha cục bộ lại có thể tạo giao thoa?
- Chuẩn hóa được bảo toàn bởi điều kiện nào trên Hamiltonian và điều kiện biên?
- Vì sao sóng phẳng không chuẩn hóa được lại là nghiệm hợp lệ của phương trình Schrödinger tự do?
- Khi nào sự tiêu tán của bó sóng chỉ là hiệu ứng lượng tử, và khi nào có thể bỏ qua trong mô tả vật thể vĩ mô?
