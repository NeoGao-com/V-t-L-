---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Đối xứng và các định luật bảo toàn

> [!abstract] Ý chính
> Mỗi phép đối xứng liên tục của không-thời gian (dịch chuyển, quay, dịch thời gian) được biểu diễn bằng toán tử unita giao hoán với Hamiltonian — và sinh ra một tích phân chuyển động tương ứng: động lượng, mô-men động lượng, năng lượng; bản lượng tử của định lý Noether.

## Phát biểu / Định nghĩa

**Đối xứng = toán tử unita:** mọi phép biến đổi đối xứng của hệ lượng tử được biểu diễn bởi toán tử unita $\hat U$ (định lý Wigner) với $[\hat H, \hat U] = 0$ — tính chất vật lý không đổi dưới phép biến đổi.

**Đối xứng liên tục** có dạng $\hat U(\varepsilon) = e^{-i\varepsilon\hat A/\hbar}$ với $\hat A$ Hermit là **toán tử sinh** (generator). Điều kiện $[\hat H,\hat A] = 0$ đồng nhất với điều kiện tích phân chuyển động ([[Tích phân chuyển động]]):

**Bảng tương ứng đối xứng ↔ định luật bảo toàn:**

| Đối xứng không-thời gian | Ý nghĩa | Toán tử sinh | Định luật bảo toàn |
| --- | --- | --- | --- |
| Dịch chuyển không gian $x\to x+a$ | Không gian đồng nhất — không có vị trí tuyệt đối | $\hat p$ | Động lượng ([[Nguyên lý bảo toàn động lượng]]) |
| Dịch chuyển thời gian $t\to t+\tau$ | Thời gian đồng nhất — không có mốc thời gian tuyệt đối | $\hat H$ | Năng lượng ([[Nguyên lý bảo toàn năng lượng]]) |
| Quay $\vec r \to R\vec r$ | Không gian đẳng hướng — không có phương ưu tiên | $\hat{\vec L}$ | Mô-men động lượng |

Ví dụ: thế $V = 0$ (hạt tự do) bất biến với mọi phép dịch ⟹ $\hat p$ bảo toàn; thế xuyên tâm $V(r)$ bất biến với phép quay ⟹ $\hat{\vec L}$ bảo toàn — đó là lý do electron trong nguyên tử có số lượng tử $l$, $m$ ổn định.

**Suy biến do đối xứng:** nếu $[\hat H,\hat U]=0$ và $|E\rangle$ là trạng thái dừng thì $\hat U|E\rangle$ cũng dừng cùng năng lượng — nhiều trạng thái cùng $E$. Điều này sinh suy biến ở [[Dao động tử điều hòa ba chiều]] ($SU(3)$) và [[Giếng thế ba chiều]] (hoán vị tọa độ).

**Đối xứng rời rạc:** đảo không gian (parity) $\hat P\,\psi(\vec r) = \psi(-\vec r)$ không phải đối xứng liên tục — không cho lượng bảo toàn kiểu Noether, nhưng cho số lượng tử chẵn/lẻ (thấy trong nghiệm của [[Chuyển động một chiều trong cơ học lượng tử]] khi $V$ đối xứng).

## Suy luận từ đâu

- Tiên đề gốc: các tiên đề của [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]] — tính trạng thái qua biểu diễn unita; [[Tích phân chuyển động]] cho điều kiện $[\hat H,\hat A]=0$.
- Công cụ toán: [[Lý thuyết nhóm]] (nhóm Lie, toán tử sinh), [[Định lý Noether]] (bản cổ điển), đối ứng Poisson → giao hoán tử trong [[Cơ học Hamilton]].

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: bảo toàn động lượng trong tán xạ; bảo toàn năng lượng với độ chính xác rất cao; số lượng tử $l$, $m$ quan sát qua [[Quang phổ]]; suy biến mức năng lượng của hạt trong trường xuyên tâm/đối xứng khớp nhóm đối xứng.
- Trường hợp không còn đúng: khi đối xứng bị **phá vỡ tường minh** (từ trường ngoài phá đối xứng quay → tách vạch Zeeman; tương tác yếu vi phạm parity); khi bị phá vỡ **tự phát** (cơ chế Higgs trong [[Mô hình chuẩn (Standard Model)]]) — lượng bảo toàn mất hoặc biến dạng; đối xứng rời rạc không sinh Noether charge.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Tích phân chuyển động]]
- [[Định lý Noether]]
- [[Lý thuyết nhóm]]
- [[Nguyên lý bảo toàn năng lượng]]
- [[Nguyên lý bảo toàn động lượng]]
- [[Dao động tử điều hòa ba chiều]]

## Câu hỏi mở

- "Bảo toàn theo nghĩa trung bình" và "bảo toàn từng trạng thái" khác nhau thế nào khi đối xứng chỉ đúng một phần (ví dụ đối xứng quay bị từ trường yếu phá)?
- Vì sao đối xứng dịch thời gian sinh năng lượng — còn đối xứng Lorentz (tương đối hẹp) sinh ra những lượng bảo toàn nào thêm? (Gợi ý: bảo toàn của tâm chuyển động — mở rộng đối xứng không-thời gian sang [[Thuyết tương đối hẹp]].)