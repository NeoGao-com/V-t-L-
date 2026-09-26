---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: xác-suất
trạng-thái: ổn-định
created: 2026-09-25
---

# Tiên đề về tính đẳng xác suất tiên nghiệm

> [!abstract] Ý chính
> Khi không có thông tin nào thiên vị, mọi trạng thái khả dĩ của hệ đều có xác suất như nhau (nguyên lý lý do không đầy đủ của Laplace) — nền tảng của cơ học thống kê (Boltzmann: $S = k\ln W$) và của suy luận Bayes với prior "vô thông tin".

## Nội dung

- **Công thức Bayes:**
  $P(\theta | \text{dữ liệu}) = \frac{P(\text{dữ liệu} | \theta)\, P(\theta)}{P(\text{dữ liệu})}$
  - $P(\theta)$: xác suất tiên nghiệm (prior).
  - $P(\text{dữ liệu} | \theta)$: hàm khả năng (likelihood).
  - $P(\text{dữ liệu})$: bằng chứng (evidence).
- **Quy trình thực hành:**
  1. Chọn prior (uninformative theo đẳng xác suất, hoặc informed từ kiến thức cũ).
  2. Xây likelihood từ mô hình vật lý (nhiễu Gaussian, đếm Poisson...).
  3. Tính hậu nghiệm (posterior) bằng MCMC hoặc tích phân giải tích.
  4. Trích xuất ước lượng (kỳ vọng, median, khoảng tin cậy).

## Bảng các prior thường dùng

| Prior | Dạng | Đặc điểm |
| --- | --- | --- |
| Uniform (đẳng xác suất) | $p(\theta) = \text{const}$ | Trung lập trong khoảng chọn |
| Jeffreys | $p(\theta) \propto \sqrt{I(\theta)}$ | Bất biến khi đổi biến (thang log, tỉ lệ...) |
| Conjugate (chuẩn, beta, gamma...) | trùng họ với likelihood | Tính giải tích thuận tiện |

## Ví dụ vật lý cụ thể

- **Tiên đề+entropy trong nhiệt học:** $N$ phân tử khí, mọi cách xếp (vi trạng thái) là đẳng xác suất. Với $N = 10$ phân tử trong bình 2 ngăn: số cách chia 5–5 là $C(10,5) = 252$ trên tổng $2^{10} = 1024$ → xác suất ≈ 24,6%; xác suất cả 10 cùng một ngăn chỉ $2/1024 \approx 0{,}2\%$. Với $N \sim 10^{23}$, mọi "cấu hình gọn" gần như không bao giờ xảy ra — đây chính là nền của [[Entropy]] $S = k\ln W$ và [[Nguyên lý thứ hai nhiệt động lực học]] (đếm $W$ là bài toán [[Toán tổ hợp]]).
- **Ước lượng tham số vũ trụ:** Planck dùng khung Bayesian để lấy posterior của $\Omega_\Lambda$, $\Omega_m$, $H_0$... từ dữ liệu CMB.
- **Vật lý hạt tại LHC:** posterior của khối lượng Higgs từ histogram khối lượng bốn lepton — prior uniform trên thang log (Jeffreys) cho khoảng tin cậy bất biến.
- **Kiểm định mô hình:** tỉ số posterior odds dùng để so sánh ΛCDM với mô hình thay thế.

## Kiểm chứng & giới hạn

- Thực nghiệm: cơ học thống kê khớp với mọi quan sát nhiệt (phân bố Maxwell, entropy khí); suy luận Bayes là công cụ chuẩn trong phân tích dữ liệu vật lý hiện đại (LIGO, Planck, LHC).
- Trường hợp không còn đúng: khi có thông tin thiên vị thực sự (đối xứng của hệ, định luật bảo toàn...) thì "đẳng xác suất" phải thay bằng phân bố tương ứng; chọn khoảng uniform không bất biến khi đổi biến — Jeffreys prior sửa chỗ này.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Xác suất thống kê]]: phân phối xác suất cơ bản.
- [[Entropy]]: đẳng xác suất tiên nghiệm liên hệ với cực đại entropy.
- [[Toán tổ hợp]]: đếm số trạng thái $W$ trong các bài phân bố.

## Câu hỏi mở

- Khi nào nguyên lý đẳng xác suất thất bại — và thay vào đó nên dùng prior nào? (Ví dụ: Jeffreys prior bất biến với phép đổi biến; nhưng ngay cả Jeffreys cũng có tranh luận ở chiều nhiều tham số.)
- Prior "vô thông tin" có thực sự trung lập không, hay mọi prior đều mang một giả định ngầm? (Gợi ý: uniform trên $[0,1]$ khác uniform trên thang log $[10^{-3}, 10^3]$ — kết quả posterior khác nhau khi dữ liệu ít.)