---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Suy ra hệ thức bất định từ giao hoán

> [!abstract] Công cụ để làm gì
> Bất định Heisenberg không phải một giả định về độ chính xác của thiết bị, mà là hệ quả toán học của việc hai toán tử không giao hoán. Note này suy ra bất định Robertson từ bất đẳng thức Cauchy–Schwarz, rồi chuyển sang tọa độ–xung lượng.

## 6.1. Đặt bài toán

Với toán tử tự liên hợp $\hat A$ và trạng thái chuẩn hóa $|\psi\rangle$, đặt toán tử sai lệch:

$\Delta\hat A=\hat A-\langle A\rangle I$;

trong đó $\langle A\rangle=\langle\psi|\hat A|\psi\rangle$ là số thực. Độ bất định là độ dài của vector này trong chuẩn Hilbert:

$(\Delta A)^2=\|\Delta\hat A|\psi\rangle\|^2=\langle\Delta\hat A^2\rangle$;

là số thực không âm. Ý nghĩa vật lý: $(\Delta A)^2$ chính là kỳ vọng của bình phương độ lệch giữa kết quả đo và trị trung bình. Xem [[Xác suất và trị trung bình]].

## 6.2. Bước then chốt: Cauchy–Schwarz trong không gian Hilbert

Với hai vector bất kỳ $|\varphi\rangle$ và $|\chi\rangle$, bất đẳng thức Cauchy–Schwarz cho:

$|\langle\varphi|\chi\rangle|^2\leq\|\varphi\|^2\|\chi\|^2$;

và bất thức dạng chuẩn của $\hat A$:

$\langle\varphi|\hat A^2|\varphi\rangle\geq|\langle\varphi|\hat A|\varphi\rangle|^2$.

Chọn $\varphi=\Delta\hat B|\psi\rangle$ và $\chi=\Delta\hat A|\psi\rangle$:

$\|\Delta\hat B|\psi\rangle\|^2\|\Delta\hat A|\psi\rangle\|^2\geq|\langle\psi|\Delta\hat B^\dagger\Delta\hat A|\psi\rangle|^2$;

tức là

$(\Delta A)^2(\Delta B)^2\geq\left|\langle\psi|\Delta\hat B^\dagger\Delta\hat A|\psi\rangle\right|^2$;

trong đó $\Delta\hat B^\dagger=\Delta\hat B$ vì $\hat B$ tự liên hợp. Biểu thức $\langle\psi|\Delta\hat B^\dagger\Delta\hat A|\psi\rangle$ là **hiệp phương sai** (covariance) của hai đại lượng trong trạng thái đang xét; nó luôn tách được thành thành phần giao hoán và phản giao hoán:

$\Delta\hat B\Delta\hat A=\dfrac12\left(\{\Delta\hat A,\Delta\hat B\}+[\Delta\hat B,\Delta\hat A]\right)$.

## 6.3. Hệ thức Robertson

Bỏ qua phần giao — vì nó là số hữu hạn và có thể bằng 0 — ta thu được hệ thức Robertson:

$(\Delta A)^2(\Delta B)^2\geq\dfrac14\left|\langle[\hat A,\hat B]\rangle\right|^2$;

hay ở dạng căn:

$\Delta A\,\Delta B\geq\dfrac12\left|\langle[\hat A,\hat B]\rangle\right|$.

Đây là bản tổng quát của mọi bất định lượng tử. Chú ý rằng vế phải là **kỳ vọng** của commutator trong trạng thái đang xét, chứ không phải commutator thuần; với $[\hat x,\hat p]=i\hbar$ thì kỳ vọng là hằng số nên bất định trở thành hằng số tuyệt đối.

## 6.4. Hệ thức Robertson–Schrödinger

Giữ lại phần giao cho ta dạng mạnh hơn:

$(\Delta A)^2(\Delta B)^2\geq\dfrac14\left|\langle[\hat A,\hat B]\rangle\right|^2+\dfrac14\left|\langle\{\Delta\hat A,\Delta\hat B\}\rangle\right|^2$;

trong đó $\{\hat X,\hat Y\}=\hat X\hat Y+\hat Y\hat X$ là anticommutator. Với dạng này, điều kiện đạt cực tiểu nghiêm hơn: trạng thái phải thỏa mãn đồng thời

$(\hat A-\langle A\rangle I)|\psi\rangle=i\lambda(\hat B-\langle B\rangle I)|\psi\rangle$;

với $\lambda$ thực. Khi đó cả hai thành phần bên phải đều đạt giá trị lớn nhất theo bất đẳng thức Cauchy–Schwarz.

## 6.5. Trạng thái bất định tối thiểu

Dấu bằng trong Robertson xảy ra khi $\Delta\hat A|\psi\rangle$ và $\Delta\hat B|\psi\rangle$ tỷ lệ với nhau. Trường hợp quan trọng nhất là **trạng thái cơ sở của dao động tử**, với hàm sóng:

$\psi_0(x)=\left(\frac{m\omega}{\pi\hbar}\right)^{1/4}e^{-m\omega x^2/(2\hbar)}$;

trong đó $\Delta x\,\Delta p=\hbar/2$. Như vậy bất định không phải luôn lớn hơn mức tối thiểu: có những trạng thái “sạch” đạt đúng giới hạn.

> [!note] Tên gọi
> Trạng thái đạt dấu bằng được gọi là trạng thái bất định tối thiểu (minimum-uncertainty state). Đây là lý do trạng thái cơ bản của dao động tử, vốn đã là trạng thái riêng năng lượng thấp nhất, lại là trạng thái bất định tối thiểu cho cặp $(x,p)$.

## 6.6. Vì sao không có hệ thức năng lượng–thời gian chuẩn

Bất định Robertson yêu cầu hai toán tử tự liên hợp trên cùng một miền và có mô-men bậc hai hữu hạn. Thời gian trong phương trình Schrödinger là tham số tiến hóa, không phải toán tử tự liên hợp, nên không thể áp máy móc hệ thức này cho cặp $(E,t)$. Quan hệ thực nghiệm

$\Delta E\,\Delta t\sim\dfrac{\hbar}{2}$

là một **ước lượng** dựa trên thời gian sống của trạng thái và bề rộng vạch phổ, không phải một hệ thức bất định chuẩn. Xem [[Nguyên lý bất định Heisenberg]].

## Ý nghĩa vật lý

- **Bất định là hệ quả của giao hoán:** mọi giới hạn đo đồng thời đều truy về commutator, không cần giả định độ chính xác thiết bị.
- **Commutator cho biết mức bất định tối thiểu:** khi $|\langle[\hat A,\hat B]\rangle|$ lớn, hai đại lượng “không tương thích” mạnh và bất định không thể nhỏ.
- **Trạng thái tối ưu có ý nghĩa thiết kế:** trạng thái bất định tối thiểu được dùng trong khuếch đại lượng tử, nén trạng thái và thiết kế laser, nơi cần giảm nhiễu pha.
- **Thang vĩ mô thoát bất định:** vì $\Delta p=\hbar/(2\Delta x)$ nghịch đảo với khối lượng và độ rộng vùng giam, các vật thể lớn không bao giờ thể hiện bất định rõ rệt trong thực nghiệm.

## Kiểm chứng & giới hạn

- Thực nghiệm: mọi phép đo cặp tọa độ–động lượng đều tuân thủ giới hạn; hệ quả thấy rõ ở hiệu ứng tán và hiệu ứng Compton; xem [[Hiệu ứng Compton]].
- Hệ thức yêu cầu mô-men bậc hai tồn tại: với trạng thái không thuộc miền toán tử, $\Delta A$ có thể bằng vô hạn và hệ thức mất ý nghĩa.
- Với toán tử không bị chặn, phải xét miền tác dụng cụ thể; phát biểu “giao hoán” trên giấy chưa đủ bảo đảm các điều kiện giả thiết của Robertson.
- Hệ thức chỉ là cận dưới, không phải công thức tính độ bất định; phần giao Robertson–Schrödinger có thể làm cận dưới lớn hơn đáng kể, thậm chí vô hạn.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]: MOC Chương 3 — bất định như hệ quả của bộ tiên đề.
- [[Nguyên lý bất định Heisenberg]]: các ví dụ định lượng và bảng cặp đại lượng.
- [[Đo đồng thời các đại lượng trong cơ học lượng tử]]: quan hệ giữa giao hoán và hàm riêng chung.
- [[Xác suất và trị trung bình]] · [[Các toán tử cơ bản trong cơ học lượng tử]] · [[Toán tử trong cơ học lượng tử]]
- [[Dao động điều hòa]] · [[Hiệu ứng Compton]]

## Câu hỏi mở

1. Bất đẳng thức Cauchy–Schwarz giữ vai trò gì khi thiết lập hệ thức Robertson, và vì sao bước này là nguồn gốc thực sự của giới hạn?
2. Vì sao phần giao Robertson–Schrödinger có thể làm cận dưới tăng lên rất lớn, thậm chí vô hạn?
3. Có những cặp toán tử nào mà commutator bằng không nhưng vẫn không tìm được hệ hàm riêng chung thực dụng?
4. Trạng thái bất định tối thiểu có ý nghĩa gì khi bị ràng buộc bởi đồng thời một điều kiện khác, ví dụ là hàm riêng năng lượng?
5. Nếu thay bằng các toán tử có miền tác dụng khác nhau, hệ thức Robertson còn giữ nguyên hình dạng không?
