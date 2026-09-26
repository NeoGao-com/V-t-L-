---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Đo đồng thời các đại lượng trong cơ học lượng tử

> [!abstract] Công cụ để làm gì
> Hai đại lượng vật lý có thể được xác định đồng thời khi và chỉ khi tồn tại trạng thái là hàm riêng chung của cả hai toán tử. Commutator bằng không là điều kiện đủ thuận tiện để dựng cơ sở hàm riêng chung, và cũng là nguồn gốc trực tiếp của mọi giới hạn bất định.

## 5.1. Hàm riêng chung là gì

Gọi $|u\rangle$ là **hàm riêng chung** của hai toán tử $\hat A$ và $\hat B$ nếu tồn tại hai số $a$ và $b$ sao cho:

$\hat A|u\rangle=a|u\rangle$ và $\hat B|u\rangle=b|u\rangle$.

Trong trạng thái này, phép đo $\hat A$ chắc chắn cho $a$ và phép đo $\hat B$ chắc chắn cho $b$. Về mặt thống kê, phân bố kết quả của cả hai đại lượng đều là delta tại một điểm, nên không có mâu thuẫn giữa hai phép đo.

Ví dụ chuẩn là trạng thái $|l,m\rangle$ của nguyên tử hydro: nó là hàm riêng chung của $\hat H$ (với $E_{nl}$) và của $\hat L^2$, $\hat L_z$ (với $l(l+1)\hbar^2$ và $m\hbar$).

## 5.2. Commutator bằng không là điều kiện đủ

Nếu $\hat A$ và $\hat B$ là toán tử tự liên hợp **giao hoán**:

$[\hat A,\hat B]=\hat A\hat B-\hat B\hat A=0$;

thì chúng có thể chọn chung một cơ sở hàm riêng trực chuẩn. Ý tưởng rất đơn giản: nếu $\hat B|u\rangle=b|u\rangle$ thì

$\hat A(\hat B|u\rangle)=b\hat A|u\rangle$ và $(\hat B\hat A)|u\rangle=b\hat A|u\rangle$;

từ $[\hat A,\hat B]=0$ suy ra $\hat B\hat A|u\rangle=\hat A\hat B|u\rangle=b\hat A|u\rangle$, nên $\hat A|u\rangle$ cũng là hàm riêng của $\hat B$ với cùng trị riêng $b$. Vậy không gian riêng của $\hat B$ được $\hat A$ bảo toàn, và bằng quy trình lặp lại ta dựng được hệ hàm riêng chung.

## 5.3. Giao hoán là điều kiện đủ nhưng không phải điều kiện cần

Cần phân biệt hai mệnh đề:

| Mệnh đề | Loại | Nội dung |
| --- | --- | --- |
| Giao hoán | **Đủ** | $[\hat A,\hat B]=0$ thì có cơ sở hàm riêng chung |
| Không giao hoán | **Không đủ để loại trừ** | $[\hat A,\hat B]\neq0$ không có nghĩa là không tồn tại hàm riêng chung nào |

Có những cặp không giao hoán vẫn chia sẻ một số trạng thái chung, miễn là commutator triệt tiêu ngay trên trạng thái đó: nếu $\hat A|v\rangle=a|v\rangle$ và $\hat B|v\rangle=b|v\rangle$ thì $[\hat A,\hat B]|v\rangle=(ab-ba)|v\rangle=0$. Ví dụ $\hat L_x$ và $\hat L_z$ không giao hoán ($[\hat L_x,\hat L_z]=-i\hbar\hat L_y$), nhưng trạng thái $l=0$ (orbital $s$ của nguyên tử hydro) là hàm riêng chung của cả ba thành phần mô-men xung lượng với trị riêng $0$. Các trạng thái chung như vậy chỉ là một bộ phận nhỏ: chúng không lập thành một cơ sở đầy đủ của không gian Hilbert khi $[\hat A,\hat B]\neq0$.

Vì vậy, khi gặp một cặp không giao hoán, kết luận đúng là **không thể chuẩn bị một trạng thái xác định đồng thời cả hai đại lượng với mọi tổ hợp trị riêng**, chứ không phải “không có trạng thái nào đo được cả hai”.

## 5.4. Khi nào chắc chắn không thể đo đồng thời

Với phổ rời rạc không suy biện, kết luận mạnh hơn là đúng: nếu $[\hat A,\hat B]\neq0$ thì không tồn tại cơ sở hàm riêng chung, nên **không** thể chuẩn bị trạng thái mà $\Delta A=0$ và $\Delta B=0$ đồng thời. Đây chính là lập luận dẫn tới bất định tọa độ–xung lượng, vì $[\hat x,\hat p]=i\hbar\neq0$.

Lưu ý rằng điều kiện “không suy biện” là quan trọng: khi có suy biện, các phép biến đổi cơ sở trong không gian riêng có thể làm phát sinh nhiều hệ hàm riêng chung hơn, nên kết luận cần được kiểm tra lại. Xem [[Toán tử trong cơ học lượng tử]].

## 5.5. Bảng kiểm tra các cặp đại lượng

| Cặp đại lượng | Commutator | Đo đồng thời? |
| --- | --- | --- |
| $\hat x$ và $\hat p_x$ | $i\hbar$ | Không |
| $\hat x_i$ và $\hat x_j$ | $0$ | Có |
| $\hat p_i$ và $\hat p_j$ | $0$ | Có |
| $\hat L^2$ và $\hat L_z$ | $0$ | Có, với $l,m$ rời rạc |
| $\hat L_z$ và $\hat L_x$ | $i\hbar\hat L_y$ | Không nói chung |
| $\hat H$ và $\hat L_z$ (thế tâm) | $0$ | Có |
| $\hat H$ và $\hat x$ (hố vô hạn) | $\neq0$ | Không |

Bảng cho thấy tính đo đồng thời được là một **đặc tính của đối xứng**, không phải một may mắn của thiết bị. Xem [[Các toán tử cơ bản trong cơ học lượng tử]].

## Ý nghĩa vật lý

- **Đo đồng thời là hệ quả của cấu trúc toán tử:** hai đại lượng tương thích khi chúng thuộc cùng một họ đối xứng, ví dụ tọa độ theo các trục khác nhau.
- **Hệ quả cho vận động:** trạng thái xác định đồng thời vị trí và xung lượng không tồn tại, nên quỹ đạo kiểu cổ điển chỉ là xấp xỉ. Xem [[Mẫu nguyên tử Bohr]].
- **Bất định là hệ quả, không phải tiên đề:** bất định xuất phát từ việc các cặp đại lượng quan trọng đều không giao hoán, chứ không phải từ một giả định độc lập về độ chính xác thiết bị.
- **Đo theo thứ tự cho kết quả phụ thuộc thứ tự:** đo $\hat A$ rồi $\hat B$ không cho cùng kết quả với đo $\hat B$ rồi $\hat A$ khi hai toán tử không giao hoán; đây là biểu hiện thực nghiệm của việc trạng thái bị thay đổi sau mỗi phép đo.

## Kiểm chứng & giới hạn

- Thực nghiệm: hạt trong hố thế vô hạn có $\hat H$ và $\hat x$ không giao hoán, nên không tồn tại trạng thái vừa có năng lượng xác định vừa có vị trí xác định; xem [[Phương trình Schrödinger]].
- Nguyên tử hydro cho ví dụ ngược lại: $\hat H$, $\hat L^2$, $\hat L_z$ giao hoán nên có hệ trạng thái chung $|n,l,m\rangle$.
- Trường hợp không còn đúng: với phổ liên tục hoặc khi trạng thái không nằm trong miền chung của hai toán tử, các kết luận cần được diễn đạt lại bằng toán tử mật độ.
- Các phép đo không tương thích được mô tả bằng toán tử đo tổng quát, và chúng không cùng lúc cho dự đoán chắc chắn. Xem [[Phép đo lượng tử]].

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]: MOC Chương 3 — hàm riêng chung và điều kiện đo đồng thời.
- [[Toán tử trong cơ học lượng tử]] · [[Các toán tử cơ bản trong cơ học lượng tử]]
- [[Nguyên lý bất định Heisenberg]] · [[Phép đo lượng tử]] · [[Trạng thái lượng tử]]
- [[Phương trình Schrödinger]] · [[Mẫu nguyên tử Bohr]]

## Câu hỏi mở

1. Vì sao giao hoán lại dẫn tới việc các không gian riêng được bảo toàn lẫn nhau?
2. Tồn tại hay không những cặp toán tử không giao hoán nhưng vẫn chia sẻ toàn bộ tập hàm riêng, và điều đó có xảy ra với toán tử hữu hạn chiều không?
3. Vì sao suy biện trị riêng làm mềm kết luận “không giao hoán nghĩa là không đo đồng thời được”?
4. Nếu hai đại lượng giao hoán, liệu phép đo đồng thời có luôn cho kết quả chắc chắn với mọi trạng thái chuẩn bị không?
