---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Số phức

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Số phức $z = a + bi$ thâu tóm **biên độ + pha** vào một con số duy nhất. Nhân với $e^{i\omega t}$ là quay một góc trên mặt phẳng phức, và lấy đạo hàm theo thời gian chỉ là nhân với $i\omega$. Đó là lý do mọi hệ dao động, mọi mạch xoay chiều và cả hàm sóng đều được viết bằng nó: nó biến phép tích phân vi phân thành **phép nhân**.

## Định nghĩa

$$\mathbb{C} = \{a + bi \mid a,b\in\mathbb{R}\},\qquad i^2 = -1$$

- **Mô đun** $|z| = \sqrt{a^2+b^2}$, **argument** $\arg z = \varphi$; dạng cực: $z = r(\cos\varphi + i\sin\varphi) = re^{i\varphi}$ theo [[Lượng giác]].
- **Số phức liên hợp** $\bar z = a - bi$, với $z\bar z = |z|^2$ ⟹ $z^{-1} = \dfrac{\bar z}{|z|^2}$ — công thức này là nền để tìm nghịch đảo trong [[Mạch RLC và trở kháng]].
- **Các phép toán** giống hệt cộng/trừ nhân trên cặp $(a,b)$ — cộng/trừ theo quy tắc [[Vector]]; nhân/chia thì nhân/cộng **mô đun**, cộng/trừ **pha**.
- **Quy tắc de Moivre:** $(\cos\varphi + i\sin\varphi)^n = \cos n\varphi + i\sin n\varphi$ — nhờ đó mọi nghiệm bậc $n$ của đa thức là $re^{2\pi ik/n}$, và $i^n$ lặp theo chu kỳ $1, i, -1, -i$.

**Hàm mũ phức là ngôn ngữ của dao động:** với $z(t) = Ze^{i\omega t}$,

$$\frac{dz}{dt} = i\omega z, \qquad \int z\,dt = \frac{z}{i\omega}$$

Hệ quả: phương trình vi phân tuyến tính hệ số hằng trở thành **phương trình đại số** trong $i\omega$ ([[Phương trình vi phân]]).

Hàm phức khác ứng dụng ở mức tương đương: hàm phân tích giải tích, các phương pháp **tích phân đường trong mặt phẳng phức** (dùng bán kính và số dư cực) để đánh giá tích phân thực khó, và [[Chuỗi Taylor & xấp xỉ]] trong miền $|z| < R$.

## Ý nghĩa vật lý

- **Mạch xoay chiều (phasor):** đại lượng điện xoay chiều $\tilde U = U_0e^{i(\omega t + \varphi)}$ có **biên độ và pha không đổi theo thời gian** — nên phép cộng điện áp trở thành phép cộng số phức.
- **Trở kháng phức:** $Z = R + i\left(\omega L - \dfrac{1}{\omega C}\right)$, định luật Ohm "lười biếng" $U = ZI$ — giải cả mạch trong vài dòng. **Cộng hưởng** xảy ra khi phần ảo bằng 0 ($Z$ thuần thực, dòng cực đại) — [[Cộng hưởng điện]].
- **Mạch dao động LC:** nghiệm $q(t) = q_0e^{i\omega_0t}$ với $\omega_0 = 1/\sqrt{LC}$ — nền của [[Mạch dao động LC]].
- **Tổng hợp dao động:** cộng các số phức cùng tần số, rồi đọc lại $|Z|$ làm biên độ và $\arg Z$ làm pha — nhanh và chính xác hơn cộng bằng [[Lượng giác]].
- **Giải dao động tắt dần:** nghiệm $e^{(-\gamma + i\omega)t}$ cho ta **cùng lúc** cả suy giảm lẫn dao động.
- **Sóng và hàm sóng:** $\psi \propto e^{i(\vec k\cdot\vec r - \omega t)}$ — mô tả sóng phẳng; nền của [[Biến đổi Fourier]] và [[Hàm sóng]].
- **Cộng hưởng trong lý thuyết tản phạt:** hàm truyền bám theo cực của mặt phẳng phức năng lượng.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Dòng điện xoay chiều và giá trị hiệu dụng]]: giá trị hiệu dụng là mô đun của phasor chia $\sqrt2$.
- [[Tổng hợp dao động]]: phương pháp phasor — công cụ số 1 khi cộng nhiều dao động cùng tần số.
- [[Biến đổi Fourier]]: đổi tích phân thực thành tích phân trên trục $i\omega$.
- [[Phép biến đổi Laplace]]: miền tần số phức $s = \sigma + i\omega$ giải thích bằng ngôn ngữ này.
- [[Mạch RLC và trở kháng]] · [[Mạch điện ba pha]]: số phức cho phép tính cả mạch ba pha chỉ bằng một phép nhân.
- [[Lý thuyết trường lượng tử (QFT)]]: hàm truyền bám $e^{-iEt/\hbar}$ là hàm mũ phức.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Lượng giác]] · [[Vector]] · [[Phương trình vi phân]] · [[Logarit]] · [[Đại số tuyến tính]]
- [[Biến đổi Fourier]] · [[Phép biến đổi Laplace]]

## Câu hỏi mở

- Vì sao số phức "đóng" tập các số phức, nhưng lại **không** khép kín với phép lấy căn bậc hai và phép logarit? (Gợi ý: vì sao phương trình $z^2 = -1$ có hai nghiệm, còn $\ln(-1)$ thì sao?)
- Toán tử trong cơ học lượng tử là ma trận phức — điều gì sẽ hỏng nếu ta chỉ dùng số thực? (Gợi ý: xem [[Ký hiệu Dirac]].)
- Nếu ta nhân mọi phương trình vật lý vào cùng một hằng số phức $i$, kết quả có còn là vật lý không? (Gợi ý: xem [[Sự chuyển biểu diễn và phép biến đổi unita]].)
- Vì sao số phức là trường tối thiểu chứa $\mathbb{R}$ mà vẫn cho phép xác định nghiệm của mọi đa thức? (Gợi ý: so sánh với [[Lý thuyết nhóm]].)
