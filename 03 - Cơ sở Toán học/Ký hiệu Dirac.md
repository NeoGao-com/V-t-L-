---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Ký hiệu Dirac

> [!abstract] Công cụ để làm gì
> Ký hiệu Dirac biểu diễn vector trạng thái, toán tử, tích vô hướng và phép chiếu bằng những ký hiệu nhất quán. Nó làm cho quy tắc Born, điều kiện trực chuẩn và phép tính xác suất trở nên cô đọng mà vẫn giữ được ý nghĩa toán học.

## Ket và bra

Với một vector $|\psi\rangle$ trong không gian Hilbert, $\langle\psi|$ là vector đôi, tức là một hàm tuyến tính trên các ket. Tích vô hướng được viết:

$\langle\phi|\psi\rangle$.

Theo quy ước vật lý, inner product tuyến tính theo đối số thứ hai, do đó:

$\langle a\phi+b\chi|\psi\rangle=a^*\langle\phi|\psi\rangle+b^*\langle\chi|\psi\rangle$;

$\langle\psi|a\phi+b\chi\rangle=a\langle\psi|\phi\rangle+b\langle\psi|\chi\rangle$.

Hệ quả là liên hợp:

$\langle\psi|\phi\rangle^*=\langle\phi|\psi\rangle$.

Bra không phải là một trạng thái vật lý khác; nó là phần đối của ket trong phép tích vô hướng.

## Khai triển trong cơ sở

Cho cơ sở trực chuẩn $\{|n\rangle\}$, ta có:

$|\psi\rangle=\sum_n\langle n|\psi\rangle|n\rangle$;

$\langle n|m\rangle=\delta_{nm}$.

Hệ số $c_n=\langle n|\psi\rangle$ là biên độ chồng chất. Với trạng thái chuẩn hóa:

$\sum_n|c_n|^2=1$.

Tổng hoàn chỉnh có ý nghĩa là:

$I=\sum_n|n\rangle\langle n|$;

$\hat A=\sum_na_n|a_n\rangle\langle a_n|$ khi phổ rời rạc.

## Ký hiệu toán tử

Với toán tử $\hat A$:

$\hat A|\psi\rangle=|A\psi\rangle$;

$\langle\psi|\hat A=(\hat A^\dagger|\psi\rangle)^\dagger$;

$\langle\phi|\hat A|\psi\rangle$ là biểu diễn của toán tử trong cơ sở đã chọn.

Phép tích vô hướng với một ket không chuẩn hóa cho biên độ tương đối; nếu chuẩn hóa thì bình phương nó là xác suất theo quy tắc Born.

## Cơ sở tọa độ liên tục

Trong cơ sở vị trí:

$|\psi\rangle=\int dx\,\psi(x)|x\rangle$;

$\psi(x)=\langle x|\psi\rangle$;

$\langle x|\psi\rangle^*=\langle\psi|x\rangle$.

Các ket $|x\rangle$ là ket tổng quát hóa, được định nghĩa theo quan hệ delta:

$\langle x|x'\rangle=\delta(x-x')$;

$I=\int dx\,|x\rangle\langle x|$.

Xem [[Hàm Dirac delta]]. Delta là phân bố, không phải một hàm thông thường có giá trị tại từng điểm.

## Toán tử chiếu

Nếu $|a\rangle$ đã chuẩn hóa, toán tử chiếu lên kết quả $a$ là:

$\hat P_a=|a\rangle\langle a|$.

Nó có tính chất:

$\hat P_a^2=\hat P_a=\hat P_a^\dagger$;

$\operatorname{Ran}\hat P_a=\operatorname{span}\{|a\rangle\}$;

$\langle\psi|\hat P_a|\psi\rangle=|\langle a|\psi\rangle|^2$.

Thành phần được chiếu là $\hat P_a|\psi\rangle$, còn trạng thái chuẩn hóa sau khi đo $a$ là:

$|\psi_a\rangle=\frac{\hat P_a|\psi\rangle}{\sqrt{p_a}}$, với $p_a>0$.

## Hệ nhiều hạt

Trạng thái nhiều hạt được biểu diễn trong không gian tích tensor. Trạng thái tách được có dạng:

$|\Psi\rangle=|\psi_1\rangle\otimes|\psi_2\rangle\otimes\cdots$;

trạng thái tổng quát là một tổ hợp của các trạng thái cơ sở; các trạng thái thuộc loại này có thể không tách được. Khi đó các toán tử tác dụng trên một hạt được mở rộng bằng tensor với đơn vị trên các hạt còn lại. Cơ sở tọa độ nhiều hạt dùng sản phập $\delta(\vec x_1-\vec x_1')\delta(\vec x_2-\vec x_2')\cdots$.

## Quy ước và cảnh báo

- Dấu $|x\rangle$ không có nghĩa xác suất tọa độ bằng 0 hay 1; đó là ký hiệu của trạng thái tổng quát hóa.
- Một ket có thể được nhân với một pha toàn cục $e^{i\theta}$ mà không đổi trạng thái vật lý.
- Phép đo không đơn giản là “xoá thông tin”; cập nhật trạng thái sau đo được biểu diễn bằng toán tử chiếu trong cách diễn giải chuẩn.
- Ký hiệu Dirac không tự xác nhận mọi tính chất toán học; cần kiểm tra miền tác dụng khi làm việc với toán tử không bị chặn.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Hàm sóng]] — $\psi = \langle\vec x|\psi\rangle$ là ket liên tục, thực chất là ket trong $\mathcal H$.
- [[Phương trình Schrödinger]] — $i\hbar|\dot\psi\rangle = \hat H|\psi\rangle$ viết bằng ký hiệu Dirac trở nên gọn và trực quan về vận hành.
- [[Nguyên lý bất định Heisenberg]] — $[\hat x,\hat p] = i\hbar$ là hệ thức giao hoán viết trong ký hiệu ket.
- [[Nguyên lý bất định Heisenberg]] (đo lường) — kết quả đo là trị riêng; toán tử chiếu mô tả cách trạng thái sụp xuống sau phép đo.
- [[Trạng thái liên kết]] / hệ nhiều hạt — tensor product của các ket đơn hạt.

## Liên kết
- [[Cơ sở toán học của cơ học lượng tử]]
- [[Không gian Hilbert]]
- [[Đại số tuyến tính]]
- [[Hàm Dirac delta]]
- [[Toán tử trong cơ học lượng tử]]
- [[Xác suất và trị trung bình]]
- [[Tiên đề cơ học lượng tử]]

## Câu hỏi mở

1. Vì sao không thể coi $|x\rangle$ là một vector Hilbert chuẩn hóa thông thường?
2. Quan hệ $\langle x|x'\rangle=\delta(x-x')$ biểu diễn điều gì về biến đổi tọa độ–xung lượng?
3. Tích tensor khác tích phân của các trạng thái như thế nào?
4. Tại sao một toán tử chiếu mô tả được cập nhật sau đo nhưng không tự giải thích toàn bộ vấn đề đo lường?
