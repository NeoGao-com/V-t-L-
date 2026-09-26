---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Định lý Ehrenfest

> [!abstract] Ý chính
> Trị trung bình của các đại lượng lượng tử tuân theo đúng phương trình chuyển động cổ điển: $m\dfrac{d^2\langle x\rangle}{dt^2} = -\left\langle\dfrac{\partial V}{\partial x}\right\rangle$ — cơ học lượng tử khớp với cơ học cổ điển "theo nghĩa trung bình" khi bó sóng hẹp, đây là biểu hiện định lượng của nguyên lí tương ứng.

## Phát biểu / Định nghĩa

Lấy trung bình hai vế phương trình Heisenberg (xem [[Đạo hàm của toán tử theo thời gian]]) trong một trạng thái bất kỳ:

$\dfrac{d}{dt}\langle\hat A\rangle = \dfrac{i}{\hbar}\langle[\hat H, \hat A]\rangle + \left\langle\dfrac{\partial\hat A}{\partial t}\right\rangle$

**Hệ quả trực tiếp** với $\hat A = \hat x$ và $\hat A = \hat p$:

$m\dfrac{d\langle x\rangle}{dt} = \langle p\rangle, \qquad \dfrac{d\langle p\rangle}{dt} = -\left\langle\dfrac{\partial V}{\partial x}\right\rangle$

gộp lại thành **dạng Newton của trị trung bình**:

$m\dfrac{d^2}{dt^2}\langle x\rangle = -\left\langle\dfrac{\partial V}{\partial x}\right\rangle$

**Chuyển về cơ học cổ điển:** nếu bó sóng đủ hẹp để thế năng gần như tuyến tính quanh $\langle x\rangle$:

$\left\langle\dfrac{\partial V}{\partial x}\right\rangle \approx \dfrac{\partial V}{\partial x}\Big|_{\langle x\rangle} = V'(\langle x\rangle)$

thì $\langle x\rangle(t)$ thỏa đúng $\ddot{\langle x\rangle} = -\dfrac{1}{m}V'(\langle x\rangle)$ — quỹ đạo của "tâm bó sóng" là quỹ đạo cổ điển.

**Trường hợp đúng chính xác:** khi $V$ bậc hai (dao động tử, rơi tự do trong trường đều, hạt tự do) thì $\langle V'\rangle = V'(\langle x\rangle)$ đúng mọi lúc — tâm bó luôn đi theo đường cổ điển, ví dụ trạng thái kết hợp của [[Dao động tử điều hòa lượng tử]].

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger / phương trình Heisenberg — dạng toán tử của [[Đạo hàm của toán tử theo thời gian]]; [[Trạng thái lượng tử]] cho ý nghĩa trị trung bình.
- Công cụ toán: giao hoán tử $[\hat H,\hat x] = -\dfrac{i\hbar}{m}\hat p$; khai triển Taylor của $V(\hat x)$.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: tâm bó sóng của electron hay neutron lan truyền đúng theo quỹ đạo cổ điển (thí nghiệm Davisson–Germer, chùm neutron trong trường trọng lực); trạng thái kết hợp của dao động tử đi theo quỹ đạo cổ điển trong mạch cộng hưởng lượng tử.
- Trường hợp không còn đúng: với thế phi điều hòa, $\langle V'(x)\rangle \ne V'(\langle x\rangle)$ — độ rộng bó ảnh hưởng quỹ đạo tâm; định lý chỉ mô tả **trị trung bình**, không phải từng phép đo đơn lẻ (thăng giáng lượng tử vẫn tồn tại, liên quan [[Nguyên lý bất định Heisenberg]]).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Đạo hàm của toán tử theo thời gian]]
- [[Định luật II Newton]]
- [[Bó sóng lượng tử]]
- [[Dao động tử điều hòa lượng tử]]
- [[Tích phân chuyển động]]

## Câu hỏi mở

- Vì sao phương trình trung bình không lặp lại được cho momen bậc cao (ví dụ phương trình của $\langle x^2\rangle$ chứa $\langle x^3\rangle$ v.v.) — và khi nào bộ phương trình này "đóng kín"?
- Định lý Ehrenfest dạng quay (cho $\langle\hat L\rangle$) suy ra tiến động cổ điển như thế nào — và giới hạn tương ứng cho spin?