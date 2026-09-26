---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Xác suất thống kê

> [!abstract] Công cụ để làm gì
> Vật lý nhiệt mô tả hệ hàng tỉ tỉ phân tử ($N \sim 10^{23}$) — không thể (và không cần) theo dõi từng phân tử. Xác suất thống kê là cầu nối từ **vi mô hỗn loạn** lên **vĩ mô chắc chắn**: số hạt càng lớn, các định luật thống kê càng trở nên "sắt thép".

## Định nghĩa

- **Xác suất và giá trị trung bình:** với phân bố $p_i$ của biến $X$, trung bình $\overline X = \sum_i p_i X_i$; **phương sai** $\sigma^2 = \overline{X^2} - \overline{X}^2$ đo độ phân tán, $\sigma$ là độ lệch chuẩn.
- **Định luật số lớn:** trung bình của $N$ phép đo độc lập hội tụ về giá trị kỳ vọng; độ lệch chuẩn của trung bình giảm như $1/\sqrt{N}$.
- **Phân bố Maxwell:** tỉ lệ phân tử ở mỗi khoảng vận tốc là hàm xác định theo nhiệt độ — ngẫu nhiên từng hạt, chắc chắn ở mức tập thể.

## Ý nghĩa hình học

- Phân bố xác suất là "bản đồ khối lượng" trên trục giá trị: chỗ nào cao thì kết quả đo hay rơi vào đó; $\sigma$ là "bề rộng" của bản đồ.
- Biến thiên $1/\sqrt{N}$ có nghĩa: chồng nhiều phép đo độc lập lên nhau, "ngọn đồi" càng hẹp và càng cao — trực giác của chuyển động Brown hội tụ về vĩ mô.

## Ý nghĩa vật lý

- [[Thuyết động học phân tử]]: áp suất = trung bình va chạm; nhiệt độ = động năng trung bình $\overline{W_đ} = \dfrac{3}{2}kT$ — đại lượng vĩ mô là trung bình thống kê ([[Nhiệt độ và thang nhiệt độ]]).
- [[Entropy]]: $S = k\ln W$ — "trạng thái vĩ mô có nhiều trạng thái vi mô hơn thì xác suất cao hơn" là lý do [[Nguyên lý thứ hai nhiệt động lực học]] chỉ tăng entropy; giải thích "mũi tên thời gian" và vì sao quá trình thuận nghịch chỉ là lý tưởng hóa.
- **Lượng tử — xác suất là bản chất:** $P = |\langle \phi | \psi \rangle|^2$ — xác suất đo không phải vì thiếu thông tin mà là luật của tự nhiên ([[Không gian Hilbert]], [[Tiên đề cơ học lượng tử]], [[Nguyên lý chồng chất lượng tử]]).
- **Quá trình ngẫu nhiên trong đo đạc:** phân rã phóng xạ là quá trình Poisson — mỗi hạt phân rã độc lập, thống kê đếm tuân theo phân bố ([[Phóng xạ]], [[Thí nghiệm - Đo phóng xạ]]).
- **Bức xạ vật đen:** Planck kết hợp thống kê với lượng tử hóa năng lượng để ra phổ đúng — [[Thí nghiệm - Bức xạ vật đen]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Thuyết động học phân tử]] · [[Nhiệt độ và thang nhiệt độ]]: trung bình thống kê của chuyển động phân tử.
- [[Entropy]] · [[Nguyên lý thứ hai nhiệt động lực học]]: xác suất vi trạng thái quyết định chiều tự diễn biến.
- [[Không gian Hilbert]] · [[Tiên đề cơ học lượng tử]]: xác suất lượng tử từ biên độ sóng.
- [[Xác suất và trị trung bình]] — bản chuyên biệt cho quy tắc Born, trị trung bình và phương sai.
- [[Phóng xạ]] · [[Thí nghiệm - Đo phóng xạ]]: thống kê đếm của quá trình ngẫu nhiên.
- [[Tiên đề về tính đẳng xác suất tiên nghiệm]]: giả định nền của mọi phân bố khi thiếu thông tin.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Toán tổ hợp]] (đếm vi trạng thái) · [[Logarit]] (entropy) · [[Entropy]] · [[Thuyết động học phân tử]] · [[Không gian Hilbert]] · [[Nguyên lý thứ hai nhiệt động lực học]]

## Câu hỏi mở

- Vì sao $1/\sqrt{N}$ lại xuất hiện ở khắp nơi — từ sai số đo đạc đến chuyển động Brown? (Gợi ý: định lý giới hạn trung tâm — tổng nhiều biến ngẫu nhiên độc lập luôn tiến về phân bố chuẩn.)
- Xác suất cổ điển ("thiếu thông tin") và xác suất lượng tử ("bản chất") khác nhau ở điểm mấu chốt nào? (Gợi ý: giao thoa — xác suất lượng tử cộng biên độ, không cộng xác suất.)