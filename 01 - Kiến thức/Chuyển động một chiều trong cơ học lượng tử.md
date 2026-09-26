---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Chuyển động một chiều trong cơ học lượng tử

> [!abstract] Ý chính
> Với chuyển động một chiều, phương trình Schrödinger dừng là bài toán Sturm–Liouville: phổ liên kết không suy biến, trạng thái kích thích thứ n có đúng n nút, và với thế đối xứng các nghiệm chẵn lẻ xen kẽ — đây là khung chung cho mọi bài toán một chiều (giếng thế, bậc thang, hàng rào, dao động tử).

## Phát biểu / Định nghĩa

Phương trình Schrödinger không phụ thuộc thời gian một chiều:

$-\dfrac{\hbar^2}{2m}\psi''(x) + V(x)\psi(x) = E\psi(x)$

**Các tính chất cơ bản:**

1. **Không suy biến:** trạng thái liên kết một chiều không suy biến. Giả sử có $\psi_1,\psi_2$ cùng năng lượng, Wronskian $W = \psi_1\psi_2' - \psi_2\psi_1'$ là hằng số; với điều kiện biên triệt tiêu $W=0$, nên $\psi_1 \propto \psi_2$.

2. **Định lí nút:** nghiệm liên kết thứ $n$ (đếm từ $n=0$ là trạng thái cơ bản) có **đúng $n$ nút** — hàm sóng cơ bản không có nút, mức $n=1$ có 1 nút, v.v. (hệ quả của lí thuyết dao động Sturm–Liouville).

3. **Tính chẵn lẻ:** nếu $V(x) = V(-x)$ (thế đối xứng), các nghiệm dừng có thể chọn là hàm chẵn hoặc lẻ, xen kẽ từ dưới lên: mức dưới cùng chẵn, kế tiếp lẻ...

4. **Phổ:** trạng thái liên kết ($E < V(\pm\infty)$) gián đoạn và đếm được; trạng thái tán xạ ($E > V(\pm\infty)$) liên tục (liên quan bài toán [[Thế bậc thang]]).

5. **Điều kiện biên:** với thế hữu hạn, $\psi$ và $\psi'$ liên tục; với thế nhảy vô hạn (tường cứng) chỉ cần $\psi$ liên tục; với thế delta $V = -\alpha\delta(x)$ thì $\psi$ liên tục còn $\psi'$ nhảy một lượng $-\dfrac{2m\alpha}{\hbar^2}\psi(0)$.

6. **Xuyên vào vùng cấm:** khi $E < V$, nghiệm khuếch giảm là tổ hợp $e^{\pm\kappa x}$ với $\kappa = \dfrac{\sqrt{2m(V-E)}}{\hbar}$ — độ sâu thâm nhập $1/\kappa$ (cơ sở của [[Hàng rào thế và hiệu ứng đường ngầm]]).

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng (tiên đề tiến hóa) trong [[Phương trình Schrödinger]]; tính chất của nghiệm dừng trong [[Nghiệm dừng của phương trình Schrödinger]].
- Công cụ toán: lí thuyết Sturm–Liouville — Wronskian, định lí dao động; phương trình vi phân tuyến tính cấp hai.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: mọi kết quả lượng tử hóa trong 1D (giếng, hàng rào, dao động tử) đều khớp — từ phổ hấp thụ của chấm lượng tử nano đến cấu trúc vùng của giếng lượng tử trong laser bán dẫn.
- Trường hợp không còn đúng: suy biến có thể quay lại khi thêm chiều (2D/3D), spin, hoặc thế phụ thuộc thời gian; định lí nút không áp dụng cho trạng thái tán xạ liên tục.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Phương trình Schrödinger]]
- [[Hạt tự do trong cơ học lượng tử]]
- [[Giếng thế vô hạn]]
- [[Giếng thế hữu hạn]]
- [[Thế bậc thang]]
- [[Hàng rào thế và hiệu ứng đường ngầm]]
- [[Dao động tử điều hòa lượng tử]]

## Câu hỏi mở

- Vì sao trong 1D luôn có ít nhất một trạng thái liên kết với thế hút yếu bất kỳ — nhưng trong 3D thì không (thế yếu quá thì không)? (Nổi bật khi so sánh với bài toán 3 chiều.)
- Định lí nút còn đúng với thế phụ thuộc năng lượng hiệu dụng hay không?