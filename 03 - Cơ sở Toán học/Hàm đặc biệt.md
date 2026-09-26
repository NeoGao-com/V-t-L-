---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Hàm đặc biệt

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Khi giải phương trình vi phân, nghiệm tổng quát không phải hàm lượng giác hay hàm mũ — nó là **hàm đặc biệt**. Hàm Legendre mô tả trạng thái của nguyên tử, hàm Bessel mô tả sóng trong cột ống và màng rung, hàm Hermite mô tả dao động tử điều hòa, hàm Airy mô tả vùng tiếp giáp giữa miền cấm và miền cho phép. Vault này dùng $Y_{lm}$, $J_m$, $L_n$, $H_n$ ở nhiều nơi mà chưa có note nào giải thích chúng — note này lấp đúng lỗ hổng đó.

## Định nghĩa

Hàm đặc biệt được định nghĩa bởi **phương trình vi phân** mà chúng là nghiệm, chứ không phải bằng công thức tường minh. Mỗi họ hàm ứng với một **trường vật lý** khác nhau.

### Đa thức lực Legendre $P_n(x)$ — hình cầu, đối xứng cầu

Định nghĩa bằng phương trình Legendre:

$$\dfrac{d}{dx}\left[(1-x^2)\dfrac{dP_n}{dx}\right] + n(n+1)P_n = 0, \qquad \int_{-1}^{1}P_n(x)P_m(x)\,dx = \dfrac{2}{2n+1}\delta_{nm}$$

- $P_0 = 1$, $P_1 = x$, $P_2 = \dfrac{1}{2}(3x^2 - 1)$
- **Sinh từ bài toán vật lý:** với $\theta$ là góc giữa $\vec r$ và trục $z$, $\cos\theta = x$ thì $P_n(\cos\theta)$ là sóng tĩnh ứng với trạng thái có mô-men động lượng $l = n$.
- **Trực giao trên đoạn $[-1,1]$** với trọng số đẳng nhất — đó là lý do các hệ số khai triển có dạng tích phân với trọng số $1$.

### Hàm Bessel $J_m(x)$ — sóng tròn, cột ống, màng rung

$$\dfrac{d^2y}{dx^2} + \dfrac{1}{x}\dfrac{dy}{dx} + \left(1 - \dfrac{m^2}{x^2}\right)y = 0$$

- $J_0, J_1, J_2,\dots$ đánh số bằng **nghiệm gần 0** dạng sê-ri; $J_{-m}$ và $J_m$ không độc lập.
- Nghiệm tổng quát: $y = C_1J_m(x) + C_2Y_m(x)$ với $Y_m$ là Bessel loại hai.
- **Bessel cầu** $j_l(kr)$, $y_l(kr)$ thay cho Legendre khi có **cả** đối xứng cầu và điều kiện biên tại $r=0$ (bài toán nguyên tử Hydro, [[Phương trình Schrödinger trong trường xuyên tâm]]).
- Với $\cos\theta = x$ và hệ tọa độ cầu: $Y_{lm}(\theta,\varphi) = \sqrt{\dfrac{2l+1}{4\pi}\dfrac{(l-m)!}{(l+m)!}}P_l^m(\cos\theta)e^{im\varphi}$ — **hàm cầu cầu**.

### Hàm Legendre liên kết $P_l^m$ và $Y_{lm}$

$$P_l^m(x) = (-1)^m(1-x^2)^{m/2}\dfrac{d^mP_l(x)}{dx^m}$$

Dấu $(-1)^m$ chỉ là quy ước lựa chọn pha để các hệ số trở thuận tiện. Trực giao: $\int Y_{lm}^*Y_{l'm'}\,d\Omega = \delta_{ll'}\delta_{mm'}$ — **cơ sở trực giao đầy đủ của $L^2(S^2)$**, tức mọi hàm sóng trên mặt cầu đều khai triển được trong cơ sở này.

### Hàm Hermite $H_n(x)$ — dao động tử điều hòa

Phương trình Hermite: $y'' - 2x\,y' + 2n\,y = 0$. Với $n$ nguyên không âm, một nghiệm là **đa thức** $H_n(x)$ ($H_0 = 1$, $H_1 = 2x$, $H_2 = 4x^2 - 2$); với $n$ không nguyên, nghiệm là các hàm Hermite $H_n(x)$ và $H_n(-x)$ — đó là hàm lượng giác tổng quát hoá.

- $H_n$ trực giao với **trọng số** $e^{-x^2}$: $\int_{-\infty}^{\infty}H_nH_m e^{-x^2}dx = 0$ khi $n \ne m$. Hệ quả trực tiếp: các mức năng lượng của dao động tử điều hòa lượng tử [[Dao động tử điều hòa lượng tử]] bị trực giao, và vì vậy các hàm sóng không giao nhau.

### Hàm Laguerre $L_n(x)$ — dao động tử điều hòa hai chiều

Nghiệm của $xy'' + (1-x)y' + ny = 0$; trực giao với trọng số $e^{-x}$ trên $[0,\infty)$ xuất hiện trong bài toán hai chiều, khi tách phương trình Laplace trong [[Hệ tọa độ cầu]].

### Hàm Airy $Ai(x), Bi(x)$ — bản lề giữa miền cấm và miền cho phép

$$y'' - x\,y = 0$$

Đây là hàm **bản lề** của cơ học lượng tử: ở miền $x<0$ (trong giếng thế) lời giải dao động, ở miền $x>0$ (ngoài giếng) lời giải suy giảm theo mũ. Chính nó nối liền hai thế giới đó mà không cần chuyển miền — xem [[Giếng thế hữu hạn]].

## Ý nghĩa vật lý

- **Nguyên tử Hydro:** $\psi_{nlm} = R_{nl}(r)\,Y_{lm}(\theta,\varphi)$ — Legendre tách góc, Bessel tách bán kính; số lượng tử $l, m$ chính là số bậc của đa thức Legendre ([[Nguyên tử Hydro]]).
- **Dao động tử điều hòa:** $n$ bậc Hermite cho mức năng lượng thứ $n$ ([[Dao động tử điều hòa lượng tử]]).
- **Màng trống, ống âm, kéo dây:** nghiệm Bessel với điều kiện biên tạo ra **tần số riêng rời rạc** — hòa âm ức dụng; với điều kiện biên Dirichlet dùng hàm sin, với Neumann dùng hàm cos.
- **Giếng thế hữu hạn:** hàm Airy cho phép giải bài toán hữu hạn mà không cần bỏ qua hiệu ứng xuyên tường ([[Hàng rào thế và hiệu ứng đường ngầm]]).
- **Đa thức Legendre trong vật lý:** khai triển đa thức Legendre là cách chuẩn hoá tương tác đa cực — mọi thế có đối xứng cầu đều khai triển được trong cơ sở $P_l$ trong [[Trường xuyên tâm]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Phương trình Schrödinger trong trường xuyên tâm]]: tách biến cầu cho ra Legendre và Bessel cầu.
- [[Nguyên tử Hydro]]: trạng thái tổng quát là tích của một hàm bán kính và một hàm cầu $Y_{lm}$.
- [[Dao động tử điều hòa lượng tử]] · [[Dao động tử điều hòa ba chiều]]: đa thức Hermite và Laguerre.
- [[Giếng thế hữu hạn]] · [[Hàng rào thế và hiệu ứng đường ngầm]]: hàm Airy ở vùng nối tiếp giáp.
- [[Trường xuyên tâm]]: mọi đa thức Legendre là hình chiếu của $\hat L^2$ lên trục $z$.
- [[Toán tử mô-men xung lượng]]: $L^2$ và $L_z$ trong cơ sở $|l,m\rangle$ chính là cơ sở $Y_{lm}$.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Phương trình vi phân]] · [[Chuỗi lũy thừa & Frobenius]] · [[Đại số tuyến tính]]
- [[Hệ tọa độ cầu]] · [[Phương trình đạo hàm riêng (PDE)]]

## Câu hỏi mở

- Vì sao các hàm này được gọi là "đặc biệt" khi chúng xuất hiện ở khắp mọi nơi — và vì sao chúng lại **không** có công thức tường minh giống như $\sin$ hay $e^x$? (Gợi ý: xem [[Chuỗi Taylor & xấp xỉ]].)
- Sự trực giao có trọng số của Legendre, Hermite và Laguerre lấy từ đâu — tại sao ba họ này đều có nó, còn Bessel thì không?
- Vì sao nhóm xoay cầu $SO(3)$ lại sinh ra hệ các hàm cầu $Y_{lm}$? (Gợi ý: xem [[Lý thuyết nhóm]].)
- Có những hàm nào trong vật lý hiện đại chưa tìm được dạng khép kín tương ứng?
