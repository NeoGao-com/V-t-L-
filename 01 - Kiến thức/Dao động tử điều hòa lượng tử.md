---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Dao động tử điều hòa lượng tử

> [!abstract] Ý chính
> Dao động tử điều hòa lượng tử có phổ đều $E_n = \hbar\omega\left(n + \dfrac{1}{2}\right)$, kể cả năng lượng điểm không $\dfrac{\hbar\omega}{2}$, và được giải gọn bằng đại số toán tử sinh–hủy — đây là mô hình nền cho mọi hệ dao động nhỏ: phonon, dao động phân tử, mode trường điện từ.

## Phát biểu / Định nghĩa

Hamilton: $\hat H = \dfrac{\hat p^2}{2m} + \dfrac{1}{2}m\omega^2\hat x^2$

**Phương pháp đại số (ladder):** định nghĩa toán tử sinh $\hat a^\dagger$ và hủy $\hat a$:

$\hat a = \sqrt{\dfrac{m\omega}{2\hbar}}\left(\hat x + \dfrac{i\hat p}{m\omega}\right), \qquad \hat a^\dagger = \sqrt{\dfrac{m\omega}{2\hbar}}\left(\hat x - \dfrac{i\hat p}{m\omega}\right)$

với $[\hat a,\hat a^\dagger] = 1$ và $\hat H = \hbar\omega\left(\hat N + \dfrac{1}{2}\right)$, $\hat N = \hat a^\dagger\hat a$ (toán tử số hạt — xem [[Toán tử trong cơ học lượng tử]]).

**Phổ năng lượng:**

$E_n = \hbar\omega\left(n + \dfrac{1}{2}\right), \qquad n = 0,1,2,\dots$

- Trạng thái cơ bản $E_0 = \dfrac{\hbar\omega}{2} > 0$ — **năng lượng điểm không**, hệ không bao giờ đứng yên dù ở nhiệt độ 0 (hệ quả trực tiếp của [[Nguyên lý bất định Heisenberg]]).
- Mức cách đều nhau $\Delta E = \hbar\omega$ — khác giếng vuông ($E \propto n^2$).

**Hàm sóng (biểu diễn tọa độ):**

$\psi_n(x) = \dfrac{1}{\sqrt{2^n n!}}\left(\dfrac{m\omega}{\pi\hbar}\right)^{1/4} H_n\left(\sqrt{\dfrac{m\omega}{\hbar}}\,x\right) e^{-\frac{m\omega x^2}{2\hbar}}$

với $H_n$ là đa thức Hermite: $H_0 = 1$, $H_1 = 2\xi$, $H_2 = 4\xi^2 - 2$...

**Tính chất:**

- Trạng thái cơ bản là Gaussian; trạng thái $n$ có đúng $n$ nút, tính chẵn lẻ $(-1)^n$.
- $\langle x\rangle = \langle p\rangle = 0$, nhưng $\sigma_x\sigma_p = \left(n+\dfrac{1}{2}\right)\hbar \ge \dfrac{\hbar}{2}$ — trạng thái cơ bản đạt **bất đẳng thức bất định cực tiểu**.
- Giới hạn cổ điển: với $n$ lớn, mật độ xác suất dồn về các điểm dừng cổ điển (biên chuyển động) — tương ứng với con lắc chậm ở biên.

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng với $V = \dfrac{1}{2}m\omega^2x^2$; quan hệ giao hoán $[\hat x,\hat p] = i\hbar$.
- Công cụ toán: đại số toán tử sinh–hủy (giao hoán tử), đa thức Hermite và chuỗi lũy thừa (phương pháp Frobenius).

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: dãy vạch hấp thụ hồng ngoại cách đều của dao động phân tử (phổ dao động hóa học); phonon và nhiệt dung Debye của chất rắn; năng lượng điểm không thể hiện qua hiệu ứng Casimir (lực hút giữa hai bản dẫn do mode điện từ chân không).
- Trường hợp không còn đúng: thế thực luôn có phần phi điều hòa (morse, anharmonic) làm mức không còn cách đều — nếu chưa đo được, xem cách xử lý trong [[Quang phổ]]; với biên độ lớn, dao động tử chuyển thành chuyển động tự do hay giếng khác.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Dao động điều hòa]]
- [[Chuyển động một chiều trong cơ học lượng tử]]
- [[Toán tử trong cơ học lượng tử]]
- [[Nguyên lý bất định Heisenberg]]
- [[Giếng thế vô hạn]]

## Câu hỏi mở

- Trạng thái kết hợp (coherent state) $|\alpha\rangle$ là "dao động tử cổ điển nhất" — vì sao độ bất định của nó cực tiểu và tâm bó theo quỹ đạo cổ điển?
- Điều gì xảy ra với phổ khi ta thêm số hạng $x^4$ vào thế? (Dịch mức và phá vỡ đều đặn — điểm khởi đầu của lý thuyết nhiễu loạn.)