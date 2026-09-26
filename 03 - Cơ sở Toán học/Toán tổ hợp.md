---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Toán tổ hợp

> [!abstract] Công cụ để làm gì
> Toán tổ hợp là nghệ thuật **đếm** — đếm số cách sắp xếp, chọn lựa, phân phối. Trong vật lý nó là cây cầu từ thế giới vi mô (hàng tỉ phân tử) lên thế giới vĩ mô (nhiệt độ, entropy): mọi đại lượng nhiệt động đều là câu chuyện "đếm xem có bao nhiêu vi trạng thái".

## Định nghĩa

- **Hoán vị / chỉnh hợp / tổ hợp:** số cách sắp xếp có thứ tự ($n!$, $A_n^k$) và chọn lựa không thứ tự:
  $C_n^k = \dfrac{n!}{k!\,(n-k)!}$
- **Khai triển nhị thức:** $(a + b)^n = \sum_{k=0}^{n} C_n^k\, a^{n-k} b^k$ — hệ số là đúng số cách chọn (tam giác Pascal).
- **Phân phối $N$ hạt vào các ô:** số vi trạng thái $W$ — đây là "mẫu số" của mọi tính toán thống kê.
- **Xấp xỉ Stirling** (bắt buộc khi $N$ khổng lồ, ví dụ $10^{23}$):
  $\ln N! \approx N\ln N - N$

## Ý nghĩa hình học

- Tổ hợp là đếm trên **lưới** (Pascal): mỗi bước chọn trái/phải tạo một đường đi, và $C_n^k$ đếm số đường đi.
- Trong không gian nhiều chiều, tổ hợp trở thành đếm cách "phân phối" — trực giác quan trọng khi đếm trạng thái hạt.

## Ý nghĩa vật lý

- **Entropy = log số vi trạng thái:** $S = k_B \ln W$ — công thức Boltzmann khắc trên mộ ông. Nhiệt tự truyền từ nóng sang lạnh vì trạng thái "đều" có $W$ lớn hơn hẳn ([[Entropy]], [[Nguyên lý thứ hai nhiệt động lực học]]).
- **Cách đếm quyết định loại thống kê:**
  - Hạt *phân biệt được* (cổ điển) → thống kê Maxwell–Boltzmann: $W = \dfrac{N!}{\prod n_i!}$.
  - Hạt *không phân biệt được* → thống kê Bose–Einstein và Fermi–Dirac — lý do [[Nguyên lý loại trừ Pauli]] cấm hai fermion cùng trạng thái, định hình [[Mô hình chuẩn (Standard Model)]].
- **Thống kê phân tử khí:** đếm cách phân phối vận tốc/tọa độ của các phân tử → phân bố vận tốc Maxwell và định luật khí ([[Thuyết động học phân tử]], [[Chất khí và khí lý tưởng]]).
- **Chuyển động vĩ mô là "kết quả trung bình"** của vô số va chạm vi mô ngẫu nhiên — [[Chuyển động Brown]], [[Nội năng]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Entropy]]: $S = k_B \ln W$ — cầu nối trực tiếp giữa tổ hợp và nhiệt động lực học.
- [[Thuyết động học phân tử]] · [[Chất khí và khí lý tưởng]]: phân bố vận tốc Maxwell là bài toán đếm.
- [[Nguyên lý loại trừ Pauli]] · [[Mô hình chuẩn (Standard Model)]]: thống kê fermion/boson bắt nguồn từ cách đếm hạt đồng nhất.
- [[Nội năng]] · [[Chuyển động Brown]]: trung bình thống kê của chuyển động phân tử.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Xác suất thống kê]] · [[Logarit]] · [[Entropy]] · [[Thuyết động học phân tử]] · [[Nguyên lý thứ hai nhiệt động lực học]] · [[Nguyên lý loại trừ Pauli]]

## Câu hỏi mở

- Vì sao phân bố Maxwell–Boltzmann lại "tự nhiên" nhất trong mọi cách đếm? (Gợi ý: cực đại $W$ dưới ràng buộc năng lượng cố định — liên hệ [[Phép tính biến phân]].)
- Khi hạt phải đếm theo kiểu "không phân biệt được", entropy cổ điển sai đi bao nhiêu và vì sao cần hệ số $1/N!$? (Gợi ý: nghịch lý Gibbs.)