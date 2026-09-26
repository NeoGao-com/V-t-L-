---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Đại số tuyến tính

> [!abstract] Công cụ để làm gì
> Đại số tuyến tính nghiên cứu vector, không gian, ánh xạ tuyến tính và bài toán trị riêng $A\vec x = \lambda \vec x$. Nó là xương sống của **nguyên lý chồng chất** — lý do mọi hệ tuyến tính trong vật lý đều "cộng được" và "phân rã được" thành những mode cơ bản.

## Định nghĩa

- **Không gian vector:** tập hợp có phép cộng và nhân vô hướng thỏa các tiên đề (mô hình hóa bởi [[Vector]]). Không gian càng nhiều "chiều" thì càng nhiều thông tin độc lập cần để mô tả trạng thái.
- **Ánh xạ tuyến tính (ma trận):** $A(\vec u + \vec v) = A\vec u + A\vec v$, $A(c\vec u) = c A\vec u$ — "giữ nguyên cấu trúc cộng". Ma trận $m \times n$ là ánh xạ từ không gian $n$ chiều sang $m$ chiều.
- **Cơ sở và đổi cơ sở:** cơ sở trực chuẩn là bộ "đơn vị đo" độc lập; biểu diễn của cùng một vector trong các cơ sở khác nhau liên hệ qua ma trận đổi cơ sở.
- **Trị riêng / vector riêng:** $A\vec x = \lambda \vec x$ — vector chỉ bị **co/giãn**, không bị đổi phương khi tác dụng bởi $A$.
- **Định thức:** hệ số "thể tích" bị co/giãn khi $A$ tác dụng; định thức bằng 0 ⇔ ánh xạ suy biến (mất chiều). **Vết:** tổng trị riêng — bất biến khi đổi cơ sở.

## Ý nghĩa hình học

- Mọi ánh xạ tuyến tính **khả nghịch** đều phân rã được thành **quay + co/giãn dọc trục chính** (phân rã SVD: $A = U\Sigma V^{T}$) — không cần thao tác cắt. Ánh xạ **tất định** mới cần thêm chiều co lại về không, và cho phép cắt (shear).
- Tìm trị riêng là tìm những hướng mà ánh xạ chỉ "kéo dài" mà không đổi phương — những hướng đó chính là các mode riêng tự nhiên của hệ.

## Ý nghĩa vật lý

- **Chồng chất = tuyến tính:** hai nghiệm cộng lại vẫn là nghiệm — gốc của [[Tổng hợp dao động]], [[Giao thoa sóng]] và [[Nguyên lý chồng chất lượng tử]].
- **Số phức là đại số tuyến tính 2 chiều:** $z = a + ib$ tương ứng ma trận quay–co giãn, $\begin{pmatrix}a & -b \\ b & a\end{pmatrix}$ → công cụ giải [[Mạch RLC và trở kháng]] bằng phasor.
- **Bài toán trị riêng = "âm thanh riêng" của hệ:** mode dao động riêng ([[Sóng dừng]], [[Chuyển động quay của vật rắn]]), mức năng lượng — nền tảng của [[Tiên đề cơ học lượng tử]] (trạng thái = vector, quan sát = toán tử, kết quả đo = trị riêng).
- **Đối xứng dạng ma trận:** trạng thái phân cực ánh sáng biểu diễn bằng vector và ma trận Jones ([[Ký hiệu Jones]], [[Phân cực ánh sáng]]); biểu diễn nhóm ([[Lý thuyết nhóm]]) cũng là đại số ma trận.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Tiên đề cơ học lượng tử]]: hàm sóng là vector; phương trình Schrödinger là bài toán trị riêng năng lượng.
- [[Tổng hợp dao động]] · [[Giao thoa sóng]]: dao động phức tạp = tổng các mode riêng (liên hệ [[Biến đổi Fourier]]).
- [[Mẫu nguyên tử Bohr]] · [[Quang phổ]]: các mức năng lượng rời rạc là tập trị riêng.
- [[Ký hiệu Jones]] · [[Phân cực ánh sáng]]: ma trận Jones đổi trạng thái phân cực.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Vector]] · [[Số phức]] · [[Không gian Hilbert]] · [[Ký hiệu Dirac]] · [[Giải tích Tensor]] · [[Lý thuyết nhóm]] · [[Tiên đề cơ học lượng tử]]
- [[Toán tử trong cơ học lượng tử]] — phép biến đổi tuyến tính, trị riêng và toán tử tự liên hợp.

## Câu hỏi mở

- Vì sao các đại lượng đo được trong lượng tử luôn là trị riêng *thực*? (Gợi ý: toán tử tương ứng phải là toán tử Hermite trong [[Không gian Hilbert]].)
- Khi không gian vô hạn chiều, trực giác "đếm chiều" còn đúng không? (Gợi ý: chuỗi Fourier là một vector vô hạn tọa độ — [[Biến đổi Fourier]].)