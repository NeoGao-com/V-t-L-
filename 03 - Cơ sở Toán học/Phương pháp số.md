---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Phương pháp số

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Hầu hết phương trình vi phân trong vật lý **không có lời giải tường minh** — và điều đó không phải giới hạn của toán học, chỉ là giới hạn của đôi bàn tay. Phương pháp số biến bài toán giải tích thành bài toán có thể máy tính thực hiện. Nhánh quan trọng nhất là tích phân số: nó biến một tích phân "không lấy được bằng tay" thành một tổng hữu hạn, và là nền tảng của mọi mô phỏng vật lý tính toán.

## Định nghĩa

### Tích phân số — chuyển tích phân thành tổng

$$\int_a^b f(x)\,dx = \lim_{n\to\infty}\sum_{i}f(x_i)\,\Delta x \;\Longrightarrow\; \sum_{i}f(x_i)\,\Delta x \quad (n \text{ đủ lớn})$$

Các cách chọn điểm mẫu, mỗi cách một hệ số:

| Quy tắc | Vị trí điểm | Hệ số | Bậc chính xác |
| --- | --- | --- | --- |
| Hình chữ nhật | $x_i$ | $1$ | 1 |
| Trung tâm | $x_i + \frac{\Delta x}{2}$ | $1$ | 2 |
| Simpson | $x_i, x_i+\frac{\Delta x}{2}, x_i+\Delta x$ | $\frac{1}{6}(1,4,1)$ | 4 |
| Gauss | điểm tối ưu | trọng số Gauss | cao |

Sai số của quy tắc bậc $p$ **giảm** theo lũy thừa của bước: sai số *cục bộ* trên một đoạn là $O\!\big(f^{(p+1)}\,(\Delta x)^{p+1}\big)$. Vì phải ghép $N\approx\dfrac{b-a}{\Delta x}$ đoạn, sai số *toàn cục* chỉ còn $O\!\big(f^{(p)}\,(\Delta x)^{p}\big)$ — đó là lý do quy tắc bậc 2 (hình thang, trung tâm) hội tụ nhanh hơn hẳn quy tắc bậc 1, và mỗi bậc thêm tốn một lần đánh giá hàm.

### Tích phân Monte Carlo

$$\int f\,dV \approx \dfrac{V}{N}\sum_{i=1}^{N} f(\vec r_i),\quad \vec r_i \sim \text{phân bố đều trên } V$$

Sai số giảm như $\dfrac{1}{\sqrt N}$ — **chậm hơn nhiều** so với $N^{-2}$ của quy tắc trung tâm, nhưng độ phức tạp chỉ tăng theo số chiều $\dim$ chứ không theo bậc đạo hàm. Với hệ số hằng tương đương, Monte Carlo bắt đầu thắng ở số chiều cao ($\dim \gtrsim 4$); ở số chiều thấp và hàm cần lấy tích phân chính xác, quy tắc Gauss vẫn hơn. Xem [[Toán tổ hợp]].

### Giải phương trình vi phân

- **Euler tiến:** $\vec x_{n+1} = \vec x_n + \Delta t\,\vec f(\vec x_n,t_n)$ — sai số bậc 1.
- **Runge–Kutta 4 (RK4):** sai số bậc 4 với 4 lần đánh giá hàm — lựa chọn mặc định trong mô phỏng cơ học.
- Với hệ bảo toàn năng lượng (như [[Con lắc kép]]), phương pháp symplectic giữ **đúng cấu trúc bất biến** của dòng chảy trên mặt phẳng năng lượng, nên sai số năng lượng chỉ **dao động quanh** giá trị thật chứ không tích luỹ theo thời gian. Đây là lý do mô phỏng quỹ đạo dài hạn (hệ Mặt Trời–Trái Đất) **phải** dùng phương pháp symplectic — phương pháp thông thường với cùng bước thời gian sẽ làm quỹ đạo xoắn ốc và mất bảo toàn.

## Ý nghĩa vật lý

- **Cơ học chuyển động nhiều vật thể:** tích phân tương tác đôi một là $O(N^2)$ — lý do cần dùng cây Barnes–Hut thay vì tích trực tiếp. Xem [[Trọng lực]], [[Cấu trúc tinh thể]].
- **Mô phỏng va chạm và vật lý hạt:** dùng Monte Carlo để lấy mẫu chuỗi phóng xạ và va chạm neutron. Xem [[Thí nghiệm - Khám phá neutron (Chadwick)]].
- **Tính sóng âm, khí động lực học, mô phỏng vùng âm thanh:** toàn bộ dựa trên lưới rời rạc — tức là rời rạc hóa phương trình vi phân riêng. Xem [[Sóng âm]], [[Tĩnh học chất lỏng]].
- **Tối ưu tham số trong vật lý — hoá học — sinh học:** thuật toán ngẫu nhiên (di truyền, tôi luyện) tìm cực tiểu của hàm mất mát bằng cách đánh giá nó ở nhiều bộ tham số ngẫu nhiên — đắt nhưng không cần viết đạo hàm.
- **Kiểm chứng số học:** mô phỏng Monte Carlo của phương trình trường lượng tử trên lưới là chuẩn vàng để đối chiếu thí nghiệm.
- **Sai số và ổn định số:** sai số làm tròn tích luỹ theo bước, còn **không ổn định** (bước quá lớn) thì phá vỡ ngay — hai thứ rất khác nhau. Xem [[Xử lý sai số thực nghiệm]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Phương trình vi phân]]: phương pháp số là cách giải khi không có lời giải tường minh.
- [[Phương trình đạo hàm riêng (PDE)]]: lưới rời rạc là cách chuẩn hoá PDE thành hệ đại số tuyến tính khổng lồ.
- [[Tích phân]]: mọi tích phân khó đều có thể chuyển thành tổng.
- [[Xác suất thống kê]]: Monte Carlo là ứng dụng trực tiếp của lấy mẫu ngẫu nhiên.
- [[Phân tích thứ nguyên]]: kiểm tra đơn vị vẫn là bước bắt buộc trước khi so sánh với thực nghiệm.
- [[Con lắc kép]]: mô phỏng chaos, phương pháp symplectic tránh sai số tích luỹ.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Tích phân]] · [[Phương trình vi phân]] · [[Đại số tuyến tính]] · [[Chuỗi Taylor & xấp xỉ]]
- [[Phân tích nhân khảo]]

## Câu hỏi mở

- Vì sao sai số của RK4 theo $\Delta t^4$ nhưng của Monte Carlo chỉ theo $1/\sqrt N$? (Gợi ý: xem [[Xác suất thống kê]].)
- Làm sao chọn bước thời gian để mô phỏng bền vững một hệ cơ học lượng tử trong thời gian dài? (Gợi ý: nghĩ về [[Định lý Ehrenfest]].)
- Có thể đánh giá sai số mà không biết nghiệm tường minh không? (Gợi ý: dùng [[Xử lý sai số thực nghiệm]].)
- Tại sao phương pháp đa cấp lại hiệu quả hơn cả phương pháp có hằng số tốt nhất? (Gợi ý: xem [[Chuỗi lũy thừa & Frobenius]].)
