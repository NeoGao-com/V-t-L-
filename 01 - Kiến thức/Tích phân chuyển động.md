---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Tích phân chuyển động

> [!abstract] Ý chính
> Một quan sát $\hat A$ (không phụ thuộc thời gian tường minh) là tích phân chuyển động khi và chỉ khi $[\hat H,\hat A] = 0$ — khi đó không chỉ trị trung bình mà toàn bộ phân bố xác suất của các giá trị $a_k$ đều bất biến theo thời gian; năng lượng luôn là một tích phân chuyển động.

## Phát biểu / Định nghĩa

Từ phương trình Heisenberg ([[Đạo hàm của toán tử theo thời gian]]):

$\dfrac{d\hat A}{dt} = 0 \iff [\hat H, \hat A] = 0 \quad\text{(với }\dfrac{\partial\hat A}{\partial t} = 0\text{)}$

**Hệ quả quan trọng — mạnh hơn bảo toàn trị trung bình:**

1. $\dfrac{d\langle\hat A\rangle}{dt} = 0$ — trị trung bình không đổi với mọi trạng thái.
2. **Phân bố xác suất bất biến:** gọi $\hat P_k$ là projector lên không gian riêng của $a_k$; vì $[\hat H,\hat P_k] = 0$ và $P_k$ khai triển được trong cơ sở chung của $\hat H,\hat A$:

   $P(a_k, t) = \langle\psi(t)|\hat P_k|\psi(t)\rangle = \sum_n |c_{nk}|^2 = \text{hằng số}$

   Xác suất đo được mỗi giá trị $a_k$ không đổi theo thời gian — đúng nghĩa "đại lượng bảo toàn", không chỉ mức trung bình.
3. Số lượng tử tương ứng là hằng số chuyển động: $E$, $p$ (hạt tự do), $L_z$ (thế xuyên tâm), $\hat N$ (số hạt của [[Dao động tử điều hòa lượng tử]])...
4. Tính đo đồng thời: vì $[\hat H, \hat A] = 0$, tồn tại cơ sở chung — đo $A$ cùng lúc với năng lượng không làm nhiễu ([[Đo đồng thời các đại lượng trong cơ học lượng tử]]).

**Ví dụ:**

| Hệ | Tích phân chuyển động | Lý do |
| --- | --- | --- |
| Hạt tự do | $\hat p$, $\hat E$ | $[\hat H,\hat p]=0$ vì $V=0$ |
| Thế xuyên tâm $V(r)$ | $\hat{\vec L}$ (từng thành phần) | $[\hat H, \hat L_i] = 0$ do đối xứng quay |
| Dao động tử điều hòa | $\hat N = \hat a^\dagger\hat a$ | $[\hat H,\hat N] = 0$ |
| Mọi hệ kín | $\hat H$ | tự giao hoán — năng lượng luôn bảo toàn |

## Suy luận từ đâu

- Tiên đề gốc: phương trình tiến hóa (A5) và tiên đề đo lường — xác suất $P(a_k,t)$ được cho bởi projector trong [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]].
- Công cụ toán: giao hoán tử và cơ sở trực giao chung của hai toán tử Hermit ([[Đo đồng thời các đại lượng trong cơ học lượng tử]], [[Không gian Hilbert]]).

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: số lượng tử $l$, $m$ của electron trong nguyên tử không đổi khi không có nhiễu loạn (tần số [[Quang phổ]] vạch ổn định); động lượng của hạt tự do bảo toàn qua tán xạ đàn hồi (nhiễu xạ electron, neutron đàn hồi); tuổi thọ của trạng thái dừng vì $[\hat H,\hat H]=0$.
- Trường hợp không còn đúng: hệ mở hoặc khi đo lường ([[Phép đo lượng tử]] phá vỡ trạng thái); $\hat H$ phụ thuộc thời gian (thế bật/tắt) thì không có tích phân chuyển động tĩnh; đối xứng rời rạc (parity) cho số lượng tử nhưng không sinh "lượng bảo toàn" kiểu Noether.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Đạo hàm của toán tử theo thời gian]]
- [[Đối xứng và các định luật bảo toàn]]
- [[Đo đồng thời các đại lượng trong cơ học lượng tử]]
- [[Trạng thái lượng tử]]
- [[Nghiệm dừng của phương trình Schrödinger]]

## Câu hỏi mở

- $[\hat H,\hat A]=0$ nhưng $\hat A$ vẫn có phân bố xác suất "nhảy" khi đo năng lượng đầu tiên — vậy sự bảo toàn bị phá vỡ ở đâu trong quy trình đo?
- Điều kiện $[\hat H,\hat A]=0$ có phải là điều kiện cần và đủ cho mọi $P(a_k,t)$ hằng số không? (Gợi ý: suy luận ngược từ $P(a_k,t)$ hằng ⟹ $\hat P_k$ bảo toàn ⟹ ...)