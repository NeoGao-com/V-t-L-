---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Bó sóng lượng tử

> [!abstract] Ý chính
> Bó sóng là trạng thái định xứ tạo bởi tổng liên hợp liên tục nhiều sóng phẳng. Bao bọc hoặc đỉnh của một bó hẹp dịch gần theo **tốc độ nhóm** tại $k_0$, còn các điểm pha dịch theo tốc độ pha; độ rộng vị trí và động lượng không thể đồng thời tùy ý nhỏ.

## 1. Bó sóng định xứ

Một sóng phẳng ứng với $k$ xác định có:

$p=\hbar k$.

Nó mô tả động lượng xác định nhưng phân bố vị trí trải trên toàn không gian. Bó sóng kết hợp một dải số sóng quanh $k_0$:

$\psi(x,t)=\int_{-\infty}^{\infty}\widetilde\psi(k,0)\,e^{i[kx-\omega(k)t]}\,dk$ với điều kiện chuẩn hóa

$\int_{-\infty}^{\infty}|\widetilde\psi(k,0)|^2\,dk=1$.

Trong phép tính tích phân, quy ước có thể dùng $\frac{dk}{2\pi}$ và hằng số chuẩn hóa tương ứng; ý nghĩa vật lý không đổi.

- Bó hẹp về vị trí cần dải $k$ rộng, nên $\Delta p_x=\hbar\Delta k_x$ lớn.
- Bó có dải $k$ hẹp giữ được động lượng gần $p_0=\hbar k_0$, nhưng bị kéo dài trong không gian.
- Vì vậy trạng thái định xứ phải hy sinh một phần xác định của động lượng.

## 2. Bó sóng và hệ thức bất định

Từ $p_x=\hbar k_x$ suy ra:

$\Delta p_x=\hbar\Delta k_x$.

Hệ thức bất định trong không gian số sóng là:

$\Delta x\,\Delta k_x\geq\frac12$.

Do đó:

- bó càng hẹp về vị trí, dải số sóng càng rộng và độ bất định động lượng càng lớn;
- bó càng hẹp về động lượng, bó định xứ càng dài;
- không thể chuẩn bị một bó đồng thời có $\Delta x$ và $\Delta p_x$ đều nhỏ tuỳ ý.

Bó sóng cho thấy bất định là thuộc tính của trạng thái trước phép đo, không chỉ là giới hạn do máy đo.

## 3. Chuyển động của bó sóng

### 3.1. Tốc độ pha và tốc độ nhóm

Tốc độ pha của thành phần sóng phẳng là:

$v_{\mathrm{ph}}=\frac{\omega}{k}$.

Tốc độ nhóm là:

$v_g=\frac{d\omega}{dk}$.

Ý nghĩa:

- điểm có cùng pha trong từng thành phần dịch với $v_{\mathrm{ph}}$;
- điểm cực đại hoặc bao bọc của một bó hẹp dịch gần $v_g$;
- vì các thành phần có tốc độ nhóm $v_g(k)$ khác nhau, bó tự tán khi quan hệ $\omega(k)$ không tuyến tính.

### 3.2. Hạt tự do phi tương đối tính

Dùng quan hệ năng lượng–số sóng:

$\omega(k)=\frac{\hbar k^2}{2m}$.

Suy ra:

$v_{\mathrm{ph}}=\frac{\omega}{k}=\frac{\hbar k}{2m}=\frac{v}{2}$

và

$v_g=\frac{d\omega}{dk}=\frac{\hbar k}{m}=v=\frac{p}{m}$.

Với bó hẹp quanh $k_0$, **vận tốc nhóm của bó tự do bằng vận tốc cơ học của hạt**: $v_g(k_0)=p_0/m=v$. Khi dùng năng lượng động học ở trên, vận tốc pha bằng một nửa vận tốc hạt, nhưng vận tốc pha không đại diện cho chuyển động của vật hay tốc độ truyền thông.

Hằng số $m_0c^2$ chỉ tạo pha toàn cục theo thời gian nên có thể bỏ khỏi biểu thức pha mà không ảnh hưởng mật độ xác suất. Chỉ khi dùng năng lượng tương đối đầy đủ $E=\sqrt{p^2c^2+m_0^2c^4}$ thì mới thu được quan hệ tương đối tính $v_{\mathrm{ph}}=c^2/v$ ở mục sau.

### 3.3. Hạt tự do có xét tương đối tính

Dùng năng lượng toàn phần:

$E=\sqrt{p^2c^2+m_0^2c^4}$ và $\omega=E/\hbar$.

Khi đó:

$v_g=\frac{d\omega}{dk}=\frac{pc^2}{E}=v$,

$v_{\mathrm{ph}}=\frac{\omega}{k}=\frac{c^2}{v}$.

Vì thế:

$v_{\mathrm{ph}}v_g=c^2$.

Vận tốc pha có thể lớn hơn $c$ nhưng không mang thông tin mới; vận tốc nhóm vẫn bằng vận tốc hạt và nhỏ hơn $c$. Không có nghịch lý tương đối tính.

### 3.4. Lan giãn của bó Gaussian

Một bó Gaussian tối ưu tại $t=0$ có:

$\psi(x,0)=\frac{1}{(2\pi\sigma_0^2)^{1/4}}\exp\!\left[-\frac{(x-x_0)^2}{4\sigma_0^2}+\frac{ip_0x}{\hbar}\right]$.

Trong đó:

$\Delta x(0)=\sigma_0$, $\Delta p_x=\frac{\hbar}{2\sigma_0}$.

Dưới tác động phương trình Schrödinger tự do, vị trí trung bình chuyển động đều:

$\langle x\rangle(t)=x_0+\frac{p_0}{m}t$,

còn bó giãn theo:

$(\Delta x)^2(t)=\sigma_0^2+\left(\frac{\hbar t}{2m\sigma_0}\right)^2$.

Bó Gaussian tối ưu vẫn bão hòa bất định Heisenberg:

$\Delta x(t)\Delta p_x=\frac{\hbar}{2}$.

Vì vậy bó vừa lan vừa giữ sản phẩm bất định ở giá trị tối thiểu.

## 4. Nhận xét vật lý

- Đỉnh hoặc tâm của một bó hẹp được theo dõi trong thí nghiệm thường dịch gần với $v_g(k_0)$.
- Các sóng phẳng thành phần đều thuộc cùng hạt lượng tử; “tán sắc bó sóng” không có nghĩa các hạt sinh ra hay biến mất.
- Bó lan vì có nhiều động lượng cùng lúc, ứng với nhiều tốc độ nhóm khác nhau.
- Với dải số sóng hẹp, dùng một $v_g$ tại $k_0$ mô tả chuyển động bao bọc rất tốt. Với dải rộng, các thành phần có thể phân khuỷa rõ rệt.
- Bó không thể đồng thời có $\Delta k=0$ và định xứ hữu hạn; nếu $\Delta k=0$ thì bó trở thành sóng phẳng trải vô hạn.

## 5. Kết nối với giới hạn cổ điển

- Khi dải số sóng hẹp, các thành phần có tốc độ nhóm gần nhau và bó ít lan; vận tốc nhóm tiến gần vận tốc cổ điển.
- Với vật thể vĩ mô, bước sóng de Broglie cực nhỏ, nên coi động lượng gần như xác định và chuyển động theo quy luật cổ điển.
- Bất định vẫn tồn tại về nguyên tắc, nhưng $\Delta x\,\Delta p$ có thể nhỏ đến mức không quan sát được bằng thực nghiệm thông thường.

## Kiểm chứng & giới hạn

- Thí nghiệm truyền bó sóng của hạt tự do quan sát sự lan giãn trong không khí và làm rõ tính sóng của hạt.
- Bó hẹp giúp liên hệ trực giữa vận tốc nhóm và vận tốc hạt rõ ràng hơn sóng phẳng.
- Trong thế giới trường hoặc nhiều hạt, “bó sóng” có thể phải dùng cấu hình trạng thái phức tạp hơn hàm sóng một hạt.
- Trong thế có thế, vận tốc nhóm không luôn đơn giản bằng vận tốc cơ học tức thời; cần xét cả lực và chế độ dao động của tâm bó.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[MOC - Chương 1 - Cơ sở vật lý của cơ học lượng tử]]
- [[Hàm sóng]]
- [[Phương trình Schrödinger]]
- [[Giả thuyết - Sóng de Broglie]]
- [[Nguyên lý bất định Heisenberg]]
- [[Nguyên lý chồng chất lượng tử]]
- [[Biến đổi Fourier]]
- [[Động lượng]]

## Câu hỏi mở

- Vì sao bó hẹp ở $k$ lại phải dài trong không gian?
- Tốc độ nhóm có luôn là vận tốc truyền thông của bó trong mọi hệ không?
- Vì sao thêm năng lượng tĩnh vào pha không thay đổi mật độ xác suất?
- Bó Gaussian tối ưu lan giãn theo quy luật nào khi thời gian tiến tới vô cùng?
