---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Lý thuyết trường lượng tử (QFT)

> [!abstract] Ý chính
> Mở rộng của cơ học lượng tử kết hợp thuyết tương đối hẹp: mỗi loại hạt là một kích thích cục bộ của trường lượng tử; sinh–hủy hạt được mô tả bằng toán tử — khung lý thuyết thành công nhất của vật lý (độ chính xác 10⁻¹²) và là nền tảng của [[Mô hình chuẩn (Standard Model)]].

## Nội dung

- **Quan điểm cốt lõi:** mỗi loại hạt ↔ một toán tử trường $\hat\phi(x)$; trạng thái nhiều hạt sống trong không gian Fock; toán tử sinh $a^\dagger$ và hủy $a$ tạo/xóa một kích thích (hạt).
- **Phương trình chính:**
  - Mật độ Lagrangian $\mathcal{L}(\phi, \partial_\mu\phi)$ → phương trình trường Euler–Lagrange (tinh thần của [[Nguyên lý tác dụng tối thiểu]], tổng quát hóa sang trường).
  - **Tích phân đường đi:** biên độ $\langle f|i\rangle = \int \mathcal{D}\phi\, e^{iS[\phi]}$, $S = \int \mathcal{L}\, d^4x$ — mọi "con đường" của trường đều đóng góp.
  - **Tái chuẩn hóa:** hấp thụ phân kỳ vi mô vào khối lượng/điện tích đo được → dự đoán hữu hạn ở mọi bậc vòng.

## Bảng: hệ thức giao hoán và thống kê

| Loại hạt | Hệ thức | Hệ quả |
| --- | --- | --- |
| Boson (photon, gluon, W, Z, Higgs...) | $[a, a^\dagger] = 1$ | Nhiều hạt cùng trạng thái — laser, ngưng tụ Bose–Einstein |
| Fermion (electron, quark...) | $\{c, c^\dagger\} = 1$ | Tối đa 1 hạt/trạng thái — [[Nguyên lý loại trừ Pauli]], bảng tuần hoàn |

**Định lý spin–thống kê:** spin nguyên ↔ giao hoán (boson), spin bán nguyên ↔ phản giao hoán (fermion) — một trong những kết quả hệ quả nhất của QFT tương đối tính.

## Bảng hằng số tương tác chạy (running coupling)

| Thang năng lượng | QED $\alpha_{em}$ | QCD $\alpha_s$ |
| --- | --- | --- |
| ~1 GeV (cận hồng ngoại) | ~1/137 | ~0,3 |
| $M_Z \approx 91$ GeV | ~1/128 | 0,118 |
| Xu hướng | tăng dần (cực Landau) | giảm dần — **tự do tiệm cận** (Nobel 2004) |

## Ví dụ vật lý cụ thể

- **Mô men từ dị thường electron:** QED dự đoán $a_e = \frac{g-2}{2} = 0{,}001159652181\ldots$ — khớp thực nghiệm tới **10⁻¹²**, phép dự đoán chính xác nhất trong lịch sử vật lý. Bản thân phép tính là chuỗi giản đồ Feynman hàng nghìn vòng.
- **Muon g−2 (Fermilab):** đo muon lệch dự đoán SM ~4,2σ — ứng viên hàng đầu của vật lý mới (nếu không phải lỗi hệ thống của $\alpha_s$/hadronic contributions).
- **Tự do tiệm cận và giam giữ:** ở năng lượng cao quark gần như tự do (va chạm LHC: jet); ở năng lượng thấp lực mạnh mạnh dần → quark giam trong hadron.

## Suy luận từ đâu

- = Cơ học lượng tử + thuyết tương đối hẹp ([[Thuyết tương đối hẹp]]): năng lượng $E = mc^2$ cho phép sinh/hủy hạt → "số hạt" không còn là hằng số, bắt buộc chuyển từ sóng→trường.
- Tích phân đường đi nối trực tiếp với [[Nguyên lý tác dụng tối thiểu]]: trong QFT **mọi** đường đóng góp, không chỉ đường cực trị.

## Kiểm chứng & giới hạn

- Kiểm chứng: QED (g−2), QCD (jets, cấu trúc nucleon), mô hình điện yếu ($W$, $Z$, Higgs), hiệu ứng lượng tử hóa trong vật chất ngưng tụ (hiệu ứng Casimir, Hall lượng tử).
- **Giới hạn:** chưa kết hợp được hấp dẫn (cần [[Thuyết tương đối rộng]] + lượng tử — vẫn chưa có lý thuyết hoàn chỉnh); 19 tham số SM đo thực nghiệm; QED có cực Landau ở năng lượng cực cao (chỉ là thang Planck nên không thực tế).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Mô hình chuẩn (Standard Model)]]: ứng dụng QFT thành công nhất.
- [[Nguyên lý Holography (AdS-CFT)]]: đối ngẫu gauge/hấp dẫn, AdS ↔ CFT.
- [[Thuyết tương đối hẹp]]: QFT trong không-thời gian Minkowski.
- [[Cố định gauge (Gauge fixing)]]: kỹ thuật xử lý thừa bậc tự do.
- [[Nguyên lý tác dụng tối thiểu]]: tích phân đường đi khởi nguồn từ tác dụng.
- [[Nguyên lý loại trừ Pauli]]: hệ quả spin–thống kê của fermion.

## Câu hỏi mở

- Lượng tử hóa hấp dẫn: QFT chuẩn (lặp giản đồ) phân kỳ không tái chuẩn hóa được — con đường đúng là chuỗi, vòng lặp hay thứ khác? (Liên hệ [[Nguyên lý Holography (AdS-CFT)]]: hấp dẫn có thể là hệ quả của QFT biên.)
- Vì sao 19 tham số của Mô hình chuẩn có giá trị như vậy — chúng có phải là đầu ra của một lý thuyết sâu hơn (landscape, anthropic) không?
- Sinh/hủy hạt có thực sự "từ hư không" trong chân không lượng tử — và bảo toàn năng lượng được đảm bảo thế nào khi xét năng lượng chân không (vấn đề hằng số vũ trụ, lệch 120 bậc)?