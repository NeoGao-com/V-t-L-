---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Trạng thái lượng tử

> [!abstract] Công cụ để làm gì
> Tiên đề I của cơ học lượng tử nói rằng trạng thái là một vector trong không gian Hilbert. Note này làm rõ ba điều thường gây nhầm: trạng thái là **tia** chứ không phải vector, thông tin nằm ở **cách biểu diễn** chứ không phải ở giá trị của hàm sóng, và không phải mọi trạng thái đều là hàm sóng thuần nhất.

## 2.1. Trạng thái là một tia trong không gian Hilbert

Một trạng thái lượng tử được biểu diễn bởi ket đơn vị:

$\langle\psi|\psi\rangle=1$;

trong đó $|\psi\rangle=e^{i\theta}|\psi_0\rangle$ và $e^{i\theta}|\psi_0\rangle$ mô tả cùng một trạng thái vật lý, vì mọi xác suất đều không đổi khi nhân với một pha toàn cục:

$|e^{i\theta}\psi_0|^2=|\psi_0|^2$.

Vì vậy đơn vị thực sự của mô tả là **đường thẳng** $\mathbb C|\psi_0\rangle$ hay **tia** $|\psi_0\rangle$, chứ không phải từng ket riêng lẻ. Hệ quả trực tiếp: trạng thái không có “vị trí” trong không gian Hilbert theo nghĩa hình học thông thường, nên các hình ảnh như “hạt đứng yên tại một điểm” chỉ là ẩn dụ.

Xem [[Không gian Hilbert]] và [[Ký hiệu Dirac]].

## 2.2. Thông tin nằm ở cách biểu diễn

Cùng một tia trạng thái có thể được viết theo nhiều cơ sở khác nhau, và mỗi cách viết phả lộ một loại thông tin khác nhau:

| Cơ sở | Biểu diễn | Thông tin thu được |
| --- | --- | --- |
| Vị trí | $\psi(\vec r)=\langle\vec r|\psi\rangle$ | phân bố vị trí |
| Xung lượng | $c(p)=\langle p|\psi\rangle$ | phân bố động lượng |
| Năng lượng | $c_E=\langle E|\psi\rangle$ | phân bố mức năng lượng |
| Mô-men xung lượng | $\langle l,m|\psi\rangle$ | số lượng tử orbital |

Như vậy “trạng thái” là dữ liệu gốc, còn hàm sóng chỉ là một bản tóm tắt trong cơ sở đã chọn. Đổi cơ sở là đổi cách hỏi, không đổi thực tại lượng tử. Xem [[Hàm sóng]] và [[Biến đổi Fourier]].

Một cách viết không phụ thuộc cơ sở là **toán tử mật độ**:

$\rho=|\psi\rangle\langle\psi|$;

toán tử này không đổi khi nhân $|\psi\rangle$ với một pha toàn cục, và vì vậy là mô tả trực tiếp của tia trạng thái.

## 2.3. Trạng thái thuần và trạng thái hỗn

Không phải mọi trạng thái vật lý đều là ket thuần. Khi hệ được chuẩn bị bằng cách lấy ngẫu nhiên một trong nhiều ket với xác suất $w_i$, trạng thái được mô tả bởi toán tử mật độ hỗn:

$\rho=\sum_iw_i|\psi_i\rangle\langle\psi_i|$;

với $\sum_iw_i=1$ và các ket $|\psi_i\rangle$ trực giao. Trong trường hợp này, kỳ vọng của đại lượng $A$ là trung bình của các kỳ vọng thành phần:

$\langle A\rangle=\sum_iw_i\langle\psi_i|\hat A|\psi_i\rangle$;

và $\langle\hat A^2\rangle$ cũng được trung bình tương ứng, nên phương sai luôn lớn hơn hay bằng trung bình các phương sai thành phần. Đây là dấu hiệu toán học để phân biệt trạng thái hỗn với trạng thái thuần.

Một trạng thái hỗn không cho biết hệ “đang ở” trạng thái nào; nó mô tả sự thiếu thông tin của người chuẩn bị. Trong thực nghiệm, mọi trạng thái hỗn đều có thể xem là kết quả của tương tác với môi trường, tức là **mất kết hợp** (decoherence). Xem [[Nguyên lý chồng chất lượng tử]].

## 2.4. Entropy von Neumann như một thước đo thông tin

Entropy von Neumann của trạng thái được định nghĩa bằng:

$S(\rho)=-k_B\,\mathrm{Tr}(\rho\ln\rho)$.

Với trạng thái thuần, các trị riêng của $\rho$ là $1$ và $0$, nên $S(\rho)=0$. Entropy chỉ dương khi trạng thái thật sự hỗn, và đạt cực đại $\ln d$ cho trạng thái tối đa hỗn trên không gian chiều $d$. Vì vậy entropy đo **mức không chắc chắn** của trạng thái chứ không đo mức “phức tạp” của nó. Xem [[Entropy]] và [[Nguyên lý thứ hai nhiệt động lực học]].

## Ý nghĩa vật lý

- **Thông tin lượng tử là trạng thái, không phải vị trí:** hàm sóng là toạ độ của một điểm trong không gian Hilbert, nên “trạng thái” có nhiều mức chi tiết khác nhau tùy cơ sở dùng để hỏi.
- **Pha toàn cục không quan sát được:** mọi phép đo chỉ phụ thuộc bình phương biên độ, nên pha toàn cục là mức “trống” của mô tả trạng thái.
- **Trạng thái hỗn là thực tế thường gặp:** mọi chuẩn bị thực nghiệm đều thiếu thông tin ở mức nào đó; mất kết hợp là lý do vật thể vĩ mô không còn chồng chất rõ rệt.
- **Entropy lượng tử nối hai lĩnh vực:** cùng một công thức $S=-k_B\mathrm{Tr}(\rho\ln\rho)$ vừa là entropy của cơ học thống kê, vừa là thước đo thông tin của cơ học lượng tử.

## Kiểm chứng & giới hạn

- Thực nghiệm: thí nghiệm khe đôi electron đơn cho thấy phân bố nhiều sự kiện tạo thành vân giao thoa, tức là hành vi của trạng thái thuần; xem [[Thí nghiệm - Tia âm cực (Thomson)]].
- Không có phép biến đổi đơn vị nào đưa một trạng thái hỗn trở thành thuần nhất; thông tin đã mất trong quá trình hỗn hợp hóa không thể phục hồi bằng tiến hóa đơn vị.
- Toán tử mật độ mô tả được hệ nhiều hạt, hệ tương tác mạnh và các ký hiệu lượng tử, nhưng vượt ra ngoài phạm vi của bộ tiên đề với một hạt phi tương đối tính.
- Mô tả bằng ket giả định trạng thái thuần; với trạng thái hỗn phải dùng $\rho$, và các công thức phổ trong Phép đo lượng tử cần viết lại tương ứng.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]
- [[Cơ sở toán học của cơ học lượng tử]] · [[Không gian Hilbert]] · [[Ký hiệu Dirac]]
- [[Tiên đề cơ học lượng tử]]: tiên đề A1 về trạng thái.
- [[Hàm sóng]] · [[Nguyên lý chồng chất lượng tử]]
- [[Entropy]] · [[Nguyên lý thứ hai nhiệt động lực học]] · [[Xác suất thống kê]]

## Câu hỏi mở

1. Vì sao pha toàn cục lại không quan sát được, và điều đó có liên quan gì tới tính chất của toán tử mật độ không?
2. Trạng thái hỗn khác trạng thái thuần ở điểm nào về mặt thống kê, nếu cả hai cho cùng một tập xác suất kết quả đo từng đại lượng đơn lẻ?
3. Có thể chuẩn bị một trạng thái hỗn bằng cách đo liên tiếp nhiều đại lượng không giao hoán không, và vì sao?
4. Entropy von Neumann có trực giác hình học nào tương ứng với hình học của các trạng thái thuần trong không gian Hilbert không?
