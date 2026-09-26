---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Phương trình tích phân

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Phương trình tích phân thay "đạo hàm của hàm số" bằng "giá trị của hàm tích phân theo một trục biến" — và chính vì vậy nó xuất hiện ở mọi nơi có **tích lũy theo lịch sử**: đường truyền, khuếch tán, va chạm, phổ. Nó cũng là cách hình thức hóa [[Hàm Green]] như một bài toán đảo ngược.

## Định nghĩa

Ẩn số là một hàm, và phương trình ràng buộc hàm đó thông qua một tích phân.

- **Volterra (bậc hai, cận dưới biến):**
  $$f(x) = g(x) + \lambda\int_{a}^{x} K(x,t)f(t)\,dt$$
  Lời giải duy nhất theo dãy: $f = g + \lambda Kg + \lambda^2K^2g + \dots$ — hội tụ khi $|\lambda|$ nhỏ.
- **Fredholm (cận cố định):**
  $$f(x) = g(x) + \lambda\int_a^b K(x,t)f(t)\,dt$$
  Có thể **không** có lời giải duy nhất. Khi $K$ lặp lại, lời giải không duy nhất, hoặc không tồn tại — và đó là hiện tượng cộng hưởng.
- **Hạt nhân tách được (separable kernel):** $K(x,t) = X(x)T(t)$ ⟹ bài toán rút về một hệ đại số hữu hạn trong các hệ số của $g$.

**Toán tử nghịch đảo (resolvent kernel):** đặt

$$f(x) = g(x) + \lambda\int_a^b R_\lambda(x,t)g(t)\,dt, \qquad R_\lambda = K + \lambda K R_\lambda$$

Tích phân với hạt nhân $R_\lambda$ là **nghịch đảo** của $(I - \lambda K)$ trong không gian hàm: vì $(I-\lambda K)^{-1} = \mathbb{1} + \lambda R_\lambda$. Nối với [[Hàm Green]]: hàm Green của $Ly = f$ chính là $G = L^{-1}$, còn ở đây ta có $(I-\lambda K)^{-1}$ — cùng một ý tưởng "nghịch đảo một toán tử", chỉ khác ở chỗ $K$ có phải là một tích phân hay một vi phân, và hệ số giữa resolvent với $G$ phụ thuộc quy ước chuẩn hoá cùng điều kiện biên.

Điểm quyết định: nếu $K$ là toán tử **tự phụ hợp** trên $L^2$ (hạt nhân liên tục, đối xứng Hermite, bậc hai lẻ hữu hạn) thì các trị riêng của nó là **thực** — nên bài toán tích phân lại trở về bài toán trị riêng đã quen thuộc, tức quy về [[Toán tử trong cơ học lượng tử]].

## Ý nghĩa vật lý

- **Tán xạ và va chạm:** biên độ tán xạ là tích phân đôi của hàm nhân với sóng tới và sóng ra. Tổng các đường đi — mỗi đường đi một lần tán xạ — chính là dãy Neumann ở trên. Xem [[Va chạm]], [[Thí nghiệm - Tán xạ Rutherford]].
- **Bức xạ:** công thức dipole $P \propto \ddot{d}$ là kết quả tích phân theo lịch sử chuyển động electron; ký hiệu $e^{-i\omega t}$ gộp toàn bộ phần lịch sử đó vào pha.
- **Quang điện kế (hàm truyền bám):** $\psi_{\rm out} = \psi_{\rm in} + \int K\,\psi_{\rm in}$ — bản chất lượng tử của tán xạ.
- **Phổ phát xạ:** cường độ tại tần số $\omega$ là tích phần của tín hiệu theo thời gian — nguyên lý bất định thời gian–tần số nói tích phân này rộng bằng $1/\Delta\omega$. Xem [[Biến đổi Fourier]], [[Quang phổ]].
- **Khuếch tán và truyền âm:** trường tại điểm nhận là tích phân đóng của trường tại mọi điểm phát, trọng số là hàm nhân độ nhạy cảm.
- **Dao động tắt dần:** khi hệ số phụ thuộc thời gian, việc giải bằng tích phân theo phép biến đổi Laplace là cùng một ý tưởng — xem [[Phép biến đổi Laplace]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Hàm Green]]: hạt nhân của phương trình tích phân là hàm Green.
- [[Va chạm]]: tổng các đường đi tán xạ là tích phân Neumann.
- [[Biến đổi Fourier]]: hạt nhân tích phân với $K(x,t) = e^{i\omega t}$ cho ra phép biến đổi Fourier như một trường hợp riêng.
- [[Lý thuyết trường lượng tử (QFT)]]: hàm truyền bám là hàm Green của toán tử Hamilton.
- [[Cơ học Hamilton]]: quỹ đạo trong không gian pha là đồ thị nghiệm của một hệ phương trình vi phân tích phân.
- [[Toán tử trong cơ học lượng tử]]: toán tử nghịch đảo $(I-\lambda K)^{-1}$ chính là toán tử phổ của hàm toán tử.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Tích phân]] · [[Phương trình vi phân]] · [[Phương trình đạo hàm riêng (PDE)]]

## Câu hỏi mở

- Khi nào một phương trình tích phân Fredholm **không** có lời giải duy nhất — và điều đó có phải là hiện tượng vật lý nào không? (Gợi ý: xem [[Cộng hưởng điện]].)
- Vì sao hạt nhân đối xứng lại bảo đảm trị riêng thực? (Gợi ý: dùng [[Đại số tuyến tính]].)
- Phương trình tích phân khác phương trình vi phân ở chỗ nào về mặt **thông tin**? Cái nào giữ lịch sử nhiều hơn?
- Toán tử nghịch đảo $(I-\lambda K)^{-1}$ có liên hệ gì với $\dfrac{1}{1-\lambda}$ của một con số vô hướng? (Gợi ý: xem [[Chuỗi lũy thừa & Frobenius]].)
