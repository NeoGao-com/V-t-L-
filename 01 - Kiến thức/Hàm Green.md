---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Hàm Green

> [!abstract] Ý chính
> Hàm Green là **đáp ứng của hệ tuyến tính đối với một nguồn điểm** — viên gạch cơ bản để xây nghiệm của mọi phương trình vi phân tuyến tính có nguồn. Vì phương trình tuyến tính "cộng được", biết hệ phản ứng với từng nguồn điểm là biết hệ phản ứng với nguồn bất kỳ (nguyên lý chồng chất).

## Nội dung

- **Định nghĩa:** hàm $G(x, x')$ thỏa mãn $L G(x, x') = \delta(x - x')$ với $L$ là toán tử vi phân tuyến tính (ví dụ $L = -\nabla^2 + m^2$ cho phương trình Helmholtz) và $\delta$ là nguồn điểm (hàm Dirac delta).
- **Cách dùng (tích chập):** nghiệm của $L\phi = f$ được viết qua phép chập
  $\phi(x) = \int G(x, x')\, f(x')\, d^3x'$
  — "cộng đáp ứng" của nguồn điểm tại mọi vị trí $x'$ với trọng số bằng nguồn thực $f(x')$.
- **Các hàm Green điển hình:**
  - **Helmholtz 3D:** $G(r) = \dfrac{e^{ikr}}{4\pi r}$ (sóng cầu lan ra).
  - **Có suy giảm:** $G(r) = \dfrac{e^{-\mu r}}{4\pi r}$ (thế Yukawa — tầm tương tác mạnh bị giới hạn bởi $\mu$).
  - **Thế Coulomb:** $G(r) = \dfrac{1}{4\pi r}$ là trường hợp $\mu \to 0$, $k \to 0$ — thế của điện tích điểm, nền của [[Định luật Coulomb]].
  - **Phụ thuộc thời gian:** $G_F(x - x')$ mô tả truyền nhân (propagator) trong QFT.
- **Quan sát quan trọng:** hàm Green biến bài toán vi phân với điều kiện biên thành bài toán tích phân; trong miền tần số, phép chập thành phép nhân ([[Biến đổi Fourier]]).

## Ý nghĩa vật lý

- **"Tiếng vọng" của hệ:** búa đập một nhát (xung $\delta$) → hệ rung theo $G$; đập nhiều nhát bất kỳ → cộng các tiếng vọng lại. Đó là toàn bộ triết lý của hàm Green.
- **Điện tích điểm là nguồn điểm:** thế do một điện tích điểm ([[Điện trường]], [[Định luật Coulomb]]) chính là hàm Green của toán tử Laplace; mọi phân bố điện tích là "chập" các nguồn điểm lại.
- **Propagator trong lượng tử:** xác suất hạt đi từ $x'$ đến $x$ là hàm Green của phương trình Schrödinger — các "biểu đồ Feynman" chỉ là cách tính gần đúng hàm Green này ([[Lý thuyết trường lượng tử (QFT)]]).
- **Chọn gauge = chọn hàm Green:** các lựa chọn gauge khác nhau tương ứng các quy ước hàm Green khác nhau ([[Cố định gauge (Gauge fixing)]]).

## Liên kết

- [[MOC - Kiến thức Vật lý]] · [[MOC - Cơ sở Toán học]]
- [[Lý thuyết trường lượng tử (QFT)]]: hàm Green là công cụ cơ bản để tính biên độ.
- [[Cố định gauge (Gauge fixing)]]: việc chọn gauge đi kèm chọn hàm Green phù hợp.
- [[Phương trình vi phân]]: nguồn gốc trực tiếp của hàm Green.
- [[Giải tích Vector (Grad, Div, Curl)]]: toán tử $\nabla^2$ xuất hiện trong phương trình Helmholtz.
- [[Biến đổi Fourier]]: chập ↔ nhân, cách tính hàm Green gọn nhất.
- [[Hàm Dirac delta]]: nguồn điểm $\delta(x - x')$ — khái niệm trung tâm của định nghĩa hàm Green.
- [[Định luật Coulomb]] · [[Điện trường]]: thế điện tích điểm là hàm Green cơ bản nhất.

## Câu hỏi mở

- Sự khác biệt giữa hàm Green nhân quả (causal — đáp ứng chỉ tồn tại sau khi có nguồn) và hàm Green đối xứng ảnh hưởng thế nào đến điều kiện ban đầu của hệ vật lý?
- Vì sao hàm Green của QFT lại "lan" theo cả hai chiều thời gian? (Gợi ý: hạt ↔ phản hạt trong [[Mô hình chuẩn (Standard Model)]].)