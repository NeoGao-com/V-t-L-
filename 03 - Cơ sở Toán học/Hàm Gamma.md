---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Hàm Gamma

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Hàm Gamma là phép mở rộng của phép tính giai thừa ra toàn bộ trục số thực, và là "hàm mũ e" của thế giới hàm. Nó xuất hiện ở những chỗ tưởng như vô cùng xa lạ: nhiệt dung, hệ số truyền bám, chuẩn hoá phân phối xác suất, hằng số hấp dẫn, và giải pháp của phương trình vi phân siêu lược.

## Định nghĩa

$$\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}\,dt \quad (\mathrm{Re}\,z > 0)$$

- Quan hệ **giai thừa:** $\Gamma(n) = (n-1)!$ cho $n$ nguyên dương, nên $\Gamma(n+1) = n\Gamma(n)$ — phép đệ quy giống hệt giai thừa.
- $\Gamma\left(\tfrac12\right) = \sqrt{\pi}$ — hằng số làm cho phân bố Gauss chuẩn hoá vừa đẹp: $\displaystyle\int_{-\infty}^{\infty}e^{-x^2}dx = \sqrt\pi$.
- Hàm Beta tương ứng: $B(p,q) = \dfrac{\Gamma(p)\Gamma(q)}{\Gamma(p+q)}$ — tích phân ba chiều và beta, nền của phân phối Dirichlet.
- **Hàm Gamma chuẩn hoá** phân phối xác suất: $f(x) = \dfrac{x^{\alpha-1}e^{-x/\theta}}{\Gamma(\alpha)\theta^{\alpha}}$ — mọi phân phối Gamma đều là gia đình này.

**Xấp xỉ Stirling** — công cụ thực hành quan trọng nhất khi $n$ lớn:

$$\ln n! = n\ln n - n + \dfrac12\ln(2\pi n) + O\!\left(\dfrac1n\right)$$

Đây là kết quả ta dùng mỗi khi cần $\ln N!$ với $N \sim 10^{23}$ (số phân tử trong một mol). Xem [[Toán tổ hợp]].

## Ý nghĩa vật lý

- **Chuẩn hoá và trạng thái:** mọi đại lượng tổng các trạng thái liên tục đều cần tích phân hàm mũ suy giảm; $\Gamma$ là kết quả của tích phân đó. Ví dụ phân bố tốc độ Maxwell suy ra từ tích phân tạo $\Gamma\left(\tfrac32\right)$ với $h$ và $k_B$ — [[Thuyết động học phân tử]].
- **Nhiệt dung của tinh thể Debye:** $C \propto\int_0^{\Theta_D} \dfrac{x^2}{e^{x/\theta}-1}dx$, và chính tích phân này được tính bằng $\Gamma$ — [[Nội năng]].
- **Phân rã phóng xạ liên tiếp:** thời gian chờ trước một lần phóng xạ có phân phối mũ, và tích phân tổng các bước dẫn tới $\Gamma$ — [[Phóng xạ]].
- **Thống kê:** tổng nhiều biến độc lập cùng phân phối cho phân phối Gamma; tổng nhiều biến chuẩn hoá cho phân phối chuẩn — [[Xác suất thống kê]].
- **Phương trình vi phân siêu lược:** các nghiệm như $e^{-1/x^2}$ mà cũng là nghiệm của phương trình vi phân bậc cao — nói chung, hàm Gamma là chuẩn cho các bài toán trường hợp riêng.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Entropy]]: $S = k_B\ln W$ và $\ln N! \approx N\ln N - N$ — Stirling là phép xấp xỉ Gamma hầu hết người học vật lý dùng.
- [[Thuyết động học phân tử]]: phân bố tốc độ Maxwell là hằng số chuẩn hoá tích phân tử Gamma.
- [[Xác suất thống kê]]: hàm mật độ chuẩn hoá bằng $\Gamma$ cho mọi phân phối liên tục cơ bản.
- [[Nội năng]]: tích phánh tích phân Gamma mô tả nhiệt dung.
- [[Phóng xạ]]: hàm phân bố thời gian chờ là hàm mũ; chuỗi phóng xạ liên tiếp dẫn tới Gamma.
- [[Mô hình chuẩn (Standard Model)]]: hằng số và hệ số chuẩn hoá từ các tích phân trường lượng tử.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Tích phân]] · [[Toán tổ hợp]] · [[Logarit]] · [[Chuỗi lũy thừa & Frobenius]] · [[Xác suất thống kê]]

## Câu hỏi mở

- Vì sao $\Gamma\left(\tfrac12\right) = \sqrt\pi$ lại xuất hiện "tình cờ" trong tích phân Gauss? (Gợi ý: thử tọa độ cầu trong [[Hệ tọa độ cầu]].)
- Stirling sai số bao nhiêu khi $n = 10^{6}$? Có đáng để lấy thêm số hạng không?
- Tại sao phân phối Poisson hội tụ về phân phối Gauss, và vai trò của $\Gamma$ trong phép giới hạn đó là gì? (Gợi ý: xem [[Xác suất và trị trung bình]].)
- Tích phân $\int_0^\infty x^{z-1}e^{-x}dx$ hội tụ khi nào? Có liên hệ gì với [[Đại số tuyến tính]] không?
