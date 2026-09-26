---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Định luật Rayleigh-Jeans

> [!abstract] Ý chính
> Vật lý cổ điển dự đoán cường độ bức xạ vật đen tỷ lệ với $1/\lambda^4$ ở miền sóng dài. Công thức đúng trong điều kiện $h\nu\ll k_BT$ nhưng dẫn tới cường độ vô hạn ở bước sóng ngắn: “thảm họa tử ngoại”.

## Dạng theo bước sóng

Trong cách ghi bức xạ phổ theo phương:

$B_{\lambda,\mathrm{RJ}}(T)\approx\frac{2ck_BT}{\lambda^4}$.

Trong cách ghi theo tần số:

$B_{\nu,\mathrm{RJ}}(T)\approx\frac{2\nu^2k_BT}{c^2}$.

Hai dạng mô tả cùng phổ nhưng phải dùng đúng biến đo và đúng hệ số chuyển đổi phổ.

## Điều kiện áp dụng

Định luật Rayleigh–Jeans là giới hạn sóng dài hoặc nhiệt độ cao của phương trình Planck:

$h\nu\ll k_BT$

hay

$hc\ll\lambda k_BT$.

Khi điều kiện này đúng, lượng tử năng lượng $h\nu$ rất nhỏ so với năng lượng nhiệt tiêu chuẩn $k_BT$, nên lượng tử hóa gần như không ảnh hưởng đến năng lượng trung bình của dao động.

## Cơ sở vật lý cổ điển

Theo định luật phân bố năng lượng đều của cơ học cổ điển, mỗi dao động tử bậc cao nhận trung bình năng lượng $k_BT$. Khi tính số mode trên mỗi đoạn phổ:

- theo tần số, số mode chứa năng lượng tăng như $\nu^2$;
- theo bước sóng, cường độ tăng như $1/\lambda^4$.

Vấn đề nằm ở chỗ số mode tần số cao không bị một nguyên lý vật lý nào chặn lại, trong khi cơ học cổ điển vẫn gán cho mỗi mode năng lượng $k_BT$.

## Thảm họa tử ngoại

Nếu công thức được dùng vô hạn khi $\lambda\to0$, ta có:

$B_{\lambda,\mathrm{RJ}}\to\infty$.

Dự đoán này không chỉ sai về số lượng; nó còn dẫn tới năng lượng toàn phổ vô hạn nếu lấy tích phân tới bước sóng bằng không. Đây là “thảm họa tử ngoại”.

Các cách cắt phổ bằng một bước sóng tối thiểu chỉ che giấu mâu thuẫn bằng tham số cắt tuỳ ý, không giải thích dữ liệu ở toàn phổ.

## Quan hệ với Planck và Wien

Công thức Planck:

$B_{\lambda}(T)=\frac{2hc^2}{\lambda^5}\frac{1}{\exp\!\left(\frac{hc}{\lambda k_BT}\right)-1}$.

Từ đó:

- Nếu $\frac{hc}{\lambda k_BT}\ll1$, mẫu số xấp xỉ $\frac{hc}{\lambda k_BT}$ và Planck trở về Rayleigh–Jeans.
- Nếu $\frac{hc}{\lambda k_BT}\gg1$, $\exp(x)\gg1$ và Planck trở về dạng Wien:
  $B_{\lambda,\mathrm{Wien}}\approx\frac{2hc^2}{\lambda^5}\exp\!\left(-\frac{hc}{\lambda k_BT}\right)$.

Planck vì thế hợp nhất miền sóng dài của Rayleigh–Jeans với sự suy giảm theo số mũ ở miền sóng ngắn.

## Kiểm chứng & giới hạn

- Thực nghiệm: Rayleigh–Jeans khớp tốt với phổ hồng ngoại xa ở nhiệt độ thường nhưng sai rõ ở sóng ngắn.
- Giới hạn: đây là phép giới hạn của vật lý cổ điển, dùng để làm nổi bật giới hạn cơ bản của định luật phân bố năng lượng đều.
- Với bước sóng vô cùng nhỏ, mô hình vật lý cổ điển còn cần kiểm tra ở thang tương đối tính; công thức Rayleigh–Jeans thông thường đã hỏng trước đó vì lượng tử hóa.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[MOC - Chương 1 - Cơ sở vật lý của cơ học lượng tử]]
- [[Bức xạ nhiệt và vật đen tuyệt đối]]
- [[Định luật Stefan-Boltzmann]]
- [[Giả thuyết - Lượng tử năng lượng Planck]]
- [[Thí nghiệm - Bức xạ vật đen]]
- [[Nguyên lý thứ hai nhiệt động lực học]]

## Câu hỏi mở

- Tại sao số mode tần số cao tăng nhanh hơn khả năng cung cấp năng lượng hữu hạn của hệ?
- Nếu thay định luật phân bố đều bằng một phân bố khác, phải thay đổi điều gì để phục hồi công thức Planck?
- Có một hằng số cắt bước sóng nào tự nhiên suy ra từ vật lý cổ điển không?
