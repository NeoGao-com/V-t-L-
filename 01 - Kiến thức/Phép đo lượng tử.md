---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Phép đo lượng tử

> [!abstract] Công cụ để làm gì
> Tiên đề III biến trạng thái thành dữ liệu thực nghiệm: phép đo một đại lượng chỉ cho ra trị riêng, và xác suất của mỗi trị riêng là bình phương biên độ. Note này hệ thống hóa tiên đề này cho cả hai loại phổ, giải thích cập nhật trạng thái sau đo, và chỉ ra điều gì xảy ra khi đo lặp lại.

## 4.1. Nội dung tiên đề đo lường

Với đại lượng vật lý $A$ được gắn với toán tử tự liên hợp $\hat A$, tiên đề đo lường gồm ba mệnh đề:

- **Kết quả đo là trị riêng:** phép đo $\hat A$ chỉ có thể cho một trị riêng $a$ nào đó, tức là $\hat A|a\rangle=a|a\rangle$.
- **Xác suất theo quy tắc Born:** nếu trạng thái chuẩn bị là $|\psi\rangle$, xác suất nhận kết quả $a$ là $p(a)=|\langle a|\psi\rangle|^2$.
- **Cập nhật trạng thái:** sau khi đo được $a$ với xác suất khác 0, trạng thái trở thành $\hat P_a|\psi\rangle/\sqrt{p(a)}$.

Điểm thứ ba là điểm khác biệt lớn nhất so với đo lượng tử trong thí nghiệm cổ điển: phép đo không chỉ lấy thông tin, mà còn thay đổi hệ. Xem [[Tiên đề cơ học lượng tử]] và [[Toán tử trong cơ học lượng tử]].

## 4.2. Phổ trị riêng gián đoạn

Khi phổ rời rạc, trạng thái khai triển trong cơ sở trực chuẩn gồm các hàm riêng:

$|\psi\rangle=\sum_n c_n|a_n\rangle$;

nên xác suất từng kết quả là:

$p_n=|c_n|^2$, và $\sum_n p_n=1$ theo điều kiện chuẩn hóa.

Đây là dạng quen thuộc của quy tắc Born: mức năng lượng của hạt trong hố thế vô hạn, mức năng lượng của dao động tử, các mức nguyên tử hydro đều là các trị riêng rời rạc của $\hat H$.

> [!note] Cơ sở riêng không duy nhất khi suy biện
> Khi một trị riêng bị suy biện, cách chọn cơ sở riêng trong không gian riêng không duy nhất. Tuy nhiên xác suất đo tổng các trạng thái riêng ứng với cùng một giá trị là bất biến, nên kết quả thực nghiệm không phụ thuộc lựa chọn cơ sở.

## 4.3. Phổ trị riêng liên tục

Khi phổ liên tục, ví dụ động lượng của hạt tự do, không thể tổng theo chỉ số rời rạc. Khi đó dùng **mật độ xác suất**:

$p(a)=|\langle a|\psi\rangle|^2$;

trong đó các ket $|a\rangle$ là ket tổng quát hóa thỏa quan hệ chuẩn $\langle a|a'\rangle=\delta(a-a')$. Xác suất đo trong một khoảng nhỏ là:

$\mathbb P(a\in[a,a+da])=|\langle a|\psi\rangle|^2\,da$;

nên xác suất của một điểm đơn lẻ bằng 0, và mọi câu hỏi dạng “giá trị chính xác là bao nhiêu” đều vô nghĩa với phổ liên tục. Xem [[Hàm Dirac delta]].

Trong biểu diễn tọa độ, cùng nội dung đó được viết bằng hàm sóng:

$|\psi(\vec r)|^2$ là mật độ xác suất vị trí, và $\int_V|\psi|^2\,d^3r$ là xác suất tìm hạt trong miền $V$. Xem [[Hàm sóng]].

## 4.4. Trị trung bình trong phép đo một đại lượng

Lặp lại cùng một cách chuẩn bị trạng thái và đo nhiều lần, trung bình các kết quả cho:

$\langle A\rangle=\sum_n p_na_n=\langle\psi|\hat A|\psi\rangle$;

với phổ liên tục, tổng được thay bằng tích phân theo mật độ xác suất. Phương sai là:

$(\Delta A)^2=\langle A^2\rangle-\langle A\rangle^2$;

và khi trạng thái là hỗn, các kỳ vọng phải được trung bình theo trọng số trạng thái thành phần. Xem [[Xác suất và trị trung bình]].

Kỳ vọng là trung tâm phân bố kết quả, không phải kết quả chắc chắn của một lần đo đơn lẻ; sai số của phép đo đơn lẻ chính là $\Delta A$.

## 4.5. Toán tử chiếu và đo lặp lại

Toán tử chiếu lên kết quả đo $a$ là $\hat P_a=|a\rangle\langle a|$, thỏa $\hat P_a^2=\hat P_a=\hat P_a^\dagger$. Với trạng thái chuẩn bị, xác suất đo $a$ có thể viết gọn:

$p(a)=\langle\psi|\hat P_a|\psi\rangle$;

nên toán tử đo tương ứng là $\hat E=\sum_na_n\hat P_a$ cho phổ rời rạc. Hệ quả trực tiếp: **đo lại ngay** cho kết quả chắc chắn là $a$, vì

$\hat P_a\left(\frac{\hat P_a|\psi\rangle}{\sqrt{p(a)}}\right)=\frac{\hat P_a|\psi\rangle}{\sqrt{p(a)}}$.

Tính chắc chắn này chính là điểm phân biệt phép đo lượng tử với việc lấy trung bình nhiều lần; nó không có nghĩa trạng thái trở về trạng thái trước khi đo.

## 4.6. Phép đo không theo phép chiếu

Các mệnh đề trên mô tả **phép đo theo phép chiếu**, trong đó kết quả là một trị riêng rời rạc. Trong thực nghiệm, thiết bị đo thường chỉ cho biết trạng thái đã đo là ket nào, chẳng hạn khi phân tích theo một cơ sở con, mà không đủ thông tin để gán một trị riêng cụ thể. Trường hợp đó mô tả bằng phép đo tổng quát với các toán tử hiệu ứng:

$E_f=\langle f|\hat\Pi|f\rangle\geq0$, và $\sum_fE_f=I$;

trong đó $\hat\Pi$ là toán tử đo tổng quát, không nhất thiết là một toán tử chiếu. Vì vậy không phải phép đo nào cũng làm trạng thái “nhảy” tới một hàm riêng.

## 4.7. Ví dụ: Stern–Gerlach

Nguyên tử bạc đi qua nam châm không đồng nhất tách thành hai vùng tương ứng với hai giá trị của $\hat S_z$. Đây là bằng chứng trực tiếp cho ba mệnh đề của tiên đề đo:

- kết quả đo chỉ có hai giá trị, dù trạng thái ban đầu là chồng chất của cả hai;
- xác suất mỗi giá trị là bình phương biên độ thành phần;
- sau một lần đo, trạng thái là hàm riêng ứng với kết quả, nên đo lại cho kết quả chắc chắn.

Xem [[Thí nghiệm - Stern-Gerlach]].

## Ý nghĩa vật lý

- **Đo là thu thập xác suất, không phải đọc giá trị ẩn:** cùng một trạng thái cho ra một phân bố kết quả khi lặp lại nhiều lần.
- **Phụ thuộc thiết bị đo:** đổi cơ sở đo là đổi tập kết quả và tập xác suất, dù trạng thái không đổi. Đó là nội dung bất biến của toán tử chiếu.
- **Sau đo, tính lượng tử bị giới hạn trong không gian kết quả:** trạng thái sau phép đo là vector trong không gian con, nên các phép đo tương thích với nhau cho kết quả chắc chắn.
- **Tính lặp lại được là tiêu chuẩn kiểm chứng:** mọi mô hình đo lường phải tái tạo được việc đo lặp lại cho cùng một kết quả.

## Kiểm chứng & giới hạn

- Thực nghiệm: Stern–Gerlach xác nhận cả ba mệnh đề; quang phổ hấp thụ xác nhận dạng rời rạc của đo năng lượng.
- Phép đo theo phép chiếu là mô hình lý tưởng; phần lớn thiết bị thực tế được mô tả gần đúng bằng phép đo tổng quát.
- Với trạng thái hỗn, các công thức xác suất phải dùng $\rho$ thay vì $|\psi\rangle\langle\psi|$.
- Các tiên đề này mô tả đo lường lý tưởng; hiệu ứng phi đo và tương tác không tức thời với thiết bị cần mô hình mở rộng.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]
- [[Tiên đề cơ học lượng tử]]: tiên đề A3 và A4.
- [[Trạng thái lượng tử]] · [[Hàm sóng]] · [[Nguyên lý chồng chất lượng tử]]
- [[Toán tử trong cơ học lượng tử]] · [[Không gian Hilbert]] · [[Ký hiệu Dirac]]
- [[Xác suất và trị trung bình]] · [[Hàm Dirac delta]]

## Câu hỏi mở

1. Vì sao xác suất của một kết quả cụ thể bằng 0 lại không có nghĩa là kết quả đó không tồn tại?
2. Tại sao các kết quả đo có thể không tạo thành một tập rời rạc đếm được, và điều đó thay đổi câu hỏi "giá trị là bao nhiêu" ra sao?
3. Vì sao đo lặp lại cho kết quả chắc chắn, trong khi trạng thái sau đo không trở về trạng thái trước đó?
4. Phép đo tổng quát cho phép một loại "kết quả" nào mà phép chiếu không mô tả được?
5. Nếu thiết bị đo chỉ giữ lại một phần thông tin, liệu có thể thu hẹp không gian con mà vẫn giữ tính lặp lại được không?
