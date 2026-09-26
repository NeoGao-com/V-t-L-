---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Chuỗi lũy thừa & Frobenius

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Phương pháp giải phương trình vi phân bằng chuỗi là công cụ **phổ quát nhất**: nó không cần nghiệm nào đã biết trước, chỉ cần một điểm nào đó mà hệ số phân tích được thành sê-ri. Nó cho ra các đa thức trực giao (Hermite, Laguerre, Legendre), nghiệm Bessel, và chính là phương pháp giải bài toán bán cầu trong [[Phương trình Schrödinger trong trường xuyên tâm]]. Khi phương trình vi phân không tách được, đây là con đường gần như duy nhất.

## Định nghĩa

### Chuỗi lũy thừa (khoảng hội tụ)

$$f(x) = \sum_{n=0}^{\infty} a_n (x-x_0)^n = a_0 + a_1(x-x_0) + a_2(x-x_0)^2 + \dots$$

- Thôi: $\sum_{n\to\infty}$, bán kính hội tụ $R$. Chuỗi chỉ đại diện cho hàm **bên trong** $R$; trên biên thường phải kiểm tra riêng (xem [[Chuỗi Taylor & xấp xỉ]]).
- Tỷ lệ kế tiếp quyết định hội tụ: $|a_{n+1}/a_n| \to L$ thì hội tụ nếu $L < 1$.
- Vì sao quan trọng: một hàm khác việt (chẳng hạn $e^x$, $\sin x$) là **duy nhất** nếu biết đủ số hạng của khai triển Taylor tại một điểm — đó là lý do vật lý dùng khai triển làm "ngôn ngữ chuẩn".

### Phương pháp khai triển sê-ri của phương trình vi phân

Giả sử $y = \sum a_n x^{n + \mu}$ với $\mu$ chưa biết (đây là ý tưởng của Frobenius). Thay vào phương trình và so sánh hệ số từng lũy thừa:

$$a_0 = 0 \Rightarrow \text{"phương trình chỉ hàm"}\; f(\mu) = 0$$

- Nghiệm của phương trình chỉ hàm là các **số mũ** — chúng quyết định dạng hành vi gần điểm $x_0$.
- Trường hợp điển hình: hai nghiệm $\mu_1, \mu_2$ phân biệt nguyên → hai nghiệm độc lập dạng sê-ri. Lặp nguyên $\mu_1 - \mu_2 \in \mathbb{Z}$ → nghiệm thứ hai phải chứa **$\ln x$**; lặp không nguyên → có thể cần sê-ri $x^{\mu}$ và $x^{\mu}\ln x$.

**Kết quả then chốt:** nếu hệ số của phương trình có dạng riêng, nghiệm tổng quát **luôn là sê-ri**. Đây là định lý khẳng định tính phổ quát của phương pháp, và là lý do nó thắng mọi "trick" giải tích khác khi cần một lời giải chắc chắn.

## Ý nghĩa vật lý

- **Đa thức trực giao là sê-ri hữu hạn:** với hệ số thế và hằng số lượng tử đúng, chuỗi ngắt lại ở bậc $n$ — chính xác là các $H_n$, $L_n$, $P_n$ trong [[Hàm đặc biệt]]. Điều kiện "chuỗi ngắt" **không** là thủ thuật: nó là cách **lượng tử hoá** bài toán, vì nó lựa chọn đúng những giá trị năng lượng cho phép trạng thái tồn tại.
- **Tách biến cầu:** phương trình Schrödinger tách theo $\theta$ cho phương trình Legendre, theo $r$ cho phương trình Bessel cầu — cả hai đều giải bằng sê-ri ([[Phương trình Schrödinger trong trường xuyên tâm]]).
- **Bán kínng:** sê-ri khai triện cho các lỗi hình học bậc cao khi cắt bán kính rất nhỏ — xem [[Chuỗi Taylor & xấp xỉ]].
- **Sai số khi xấp xỉ:** giữ $N$ số hạng, sai số $\sim a_N R^N$ — cơ sở định lượng của mọi phép xấp xỉ trong tính tay và mô phỏng.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Phương trình Schrödinger trong trường xuyên tâm]]: tách biến xuyên tâm bằng sê-ri.
- [[Đại số tuyến tính]]: mọi đa thức trực giao tạo thành một cơ sở của không gian hàm — bước đi từ đại số sang giải tích.
- [[Chuỗi Taylor & xấp xỉ]]: nền tảng lý thuyết của cả phương pháp này.
- [[Mạch RLC và trở kháng]]: khai triển sê-ri tại một điểm là cách chọn hệ số trong phương pháp nút thế.
- [[Phương trình vi phân]]: phương pháp giải tổng quát cho hệ tuyến tính cấp cao.
- [[Toán tử trong cơ học lượng tử]]: hàm riêng của toán tử đẳng hương là hàm cầu — khai triển bằng cơ sở trực giao của $L^2(S^2)$.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Chuỗi Taylor & xấp xỉ]] · [[Phương trình vi phân]] · [[Hàm đặc biệt]] · [[Đại số tuyến tính]]
- [[Phương trình đạo hàm riêng (PDE)]]

## Câu hỏi mở

- Điều gì quyết định số mũ $\mu$ tại một điểm bất thường, và vì sao số mũ có thể **phức**? (Gợi ý: nhìn lại cách tách $\beta$ trong [[Hệ tọa độ cầu]].)
- Chuỗi có thể hội tụ tới một hàm **không giải được** phương trình vi phân không? (Gợi ý: dùng [[Chuỗi Taylor & xấp xỉ]] để tìm một hàm phẳng.)
- Tại sao cùng một phương pháp vừa sinh ra các đa thức trực giao vừa sinh ra các hàm Bessel, dù phương trình hoàn toàn khác nhau?
- Trong [[Xử lý sai số thực nghiệm]], chuỗi Taylor giải thích vì sao sai số thường là bậc cao hơn mong đợi?
