---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Giếng thế hai chiều

> [!abstract] Ý chính
> Hạt giam trong hộp thế vô hạn hai chiều có năng lượng $E = \dfrac{\pi^2\hbar^2}{2m}\left(\dfrac{n_x^2}{L_x^2} + \dfrac{n_y^2}{L_y^2}\right)$ với trạng thái $(n_x,n_y)$ — ví dụ đầu tiên cho thấy suy biến xuất hiện khi hộp đối xứng và là mô hình của chấm lượng tử hai chiều.

## Phát biểu / Định nghĩa

Thế năng: $V = 0$ trong hình chữ nhật $0 < x < L_x$, $0 < y < L_y$; $V = \infty$ bên ngoài.

Nhờ [[Tách biến trong phương trình Schrödinger ba chiều]] (áp dụng cho hai chiều), hàm sóng là tích của hai bài toán một chiều:

$\psi_{n_xn_y}(x,y) = \dfrac{2}{\sqrt{L_xL_y}}\,\sin\dfrac{n_x\pi x}{L_x}\,\sin\dfrac{n_y\pi y}{L_y}, \qquad n_x, n_y = 1,2,3,\dots$

$E_{n_xn_y} = \dfrac{\pi^2\hbar^2}{2m}\left(\dfrac{n_x^2}{L_x^2} + \dfrac{n_y^2}{L_y^2}\right)$

**Tính chất:**

- Mỗi chiều đóng góp độc lập như giếng 1D ([[Giếng thế vô hạn]]), năng lượng là **tổng** các phần.
- Trạng thái cơ bản $(1,1)$ không suy biến.
- **Suy biến do đối xứng:** khi $L_x = L_y$ (hộp vuông), $E \propto n_x^2 + n_y^2$; các cặp hoán vị $(1,2)$ và $(2,1)$ cùng năng lượng — suy biến bậc 2. Khi $L_x \ne L_y$ suy biến này biến mất.
- Số nút: trạng thái $(n_x,n_y)$ có $n_x - 1$ nút dọc và $n_y - 1$ nút ngang.
- Giới hạn cổ điển: hệ quả tương tự [[Giếng thế vô hạn]] — mật độ xác suất dồn về vùng biên biên khi số lượng tử lớn.

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng 3 chiều với điều kiện biên triệt tiêu trên biên hình chữ nhật.
- Công cụ toán: tách biến; nghiệm sin điều kiện biên; tổ hợp các số nguyên $(n_x,n_y)$.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: electron bị giam trong chấm lượng tử dạng đĩa và giếng lượng tử 2D của chất bán dẫn — phổ hấp thụ và phát quang gán được các mức $(n_x,n_y)$; kích thước giảm làm năng lượng tăng như $\dfrac{1}{L^2}$.
- Trường hợp không còn đúng: chấm thực tế có hình dạng tròn hoặc thế mềm (không phải hộp vuông vô hạn), làm suy biến đối xứng bị tách — cần mô hình thế hữu hạn hoặc giải số; nếu có từ trường đều, còn xuất hiện các trạng thái Landau hoàn toàn khác.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Tách biến trong phương trình Schrödinger ba chiều]]
- [[Giếng thế ba chiều]]
- [[Giếng thế vô hạn]]
- [[Nghiệm dừng của phương trình Schrödinger]]

## Câu hỏi mở

- Với hộp vuông, suy biến $(1,2)/(2,1)$ xuất phát từ phép đối xứng nào — và nhóm đối xứng của hộp có bao nhiêu phần tử?
- Tại sao suy biến lại "vô tình" xuất hiện khi $\dfrac{L_x^2n_x^2}{L_y^2n_y^2}$ đúng bằng tỉ số chính phương? (Suy biến ngẫu nhiên kiểu cộng hưởng.)