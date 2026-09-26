---
tags:
  - vật-lý/moc
type: moc
created: 2026-09-25
---

# MOC - Chương 1 - Cơ sở vật lý của cơ học lượng tử

> [!abstract] Mục tiêu chương
> Theo dõi chuỗi bằng chứng buộc vật lý cổ điển chuyển sang vật lý lượng tử: từ phổ bức xạ vật đen, hiệu ứng quang điện và tán Compton đến sóng vật chất, hàm sóng xác suất và chuyển động của bó sóng.

## Bản đồ chương

| Phần | Vấn đề trung tâm | Bằng chứng hoặc khái niệm then chốt |
| --- | --- | --- |
| 1 | Vì sao vật lý cổ điển không còn đủ? | Hành vi không liên tục, giao thoa và xác suất ở thang vi mô |
| 2 | Tính hạt của bức xạ bắt đầu từ đâu? | Bức xạ vật đen, Stefan–Boltzmann, Rayleigh–Jeans, Planck |
| 3 | Ánh sáng truyền năng lượng thế nào? | Hiệu ứng quang điện và giả thuyết photon của Einstein |
| 4 | Photon có động lượng như thế nào? | Hiệu ứng Compton |
| 5 | Vật chất có tính sóng không? | Lưỡng tính sóng–hạt, de Broglie, Davisson–Germer |
| 6 | Trạng thái lượng tử được mô tả ra sao? | Hàm sóng, quy tắc Born, chuẩn hóa, điều kiện biên |
| 7 | Bó sóng định xứ chuyển động thế nào? | Tốc độ pha, tốc độ nhóm, lan giãn và bất định |

## Ký hiệu dùng trong chương

- $\nu$: tần số; $\omega=2\pi\nu$: tần số góc.
- $\lambda=2\pi/k$: bước sóng; $k$: số sóng.
- $h$: hằng số Planck; $\hbar=h/(2\pi)$.
- $k_B$: hằng số Boltzmann; $T$: nhiệt độ kelvin.
- $E_K$: năng lượng động học; $E$: năng lượng dùng trong quan hệ pha.
- $p=|\vec p|$: độ lớn động lượng.
- $\psi(\vec r,t)$: hàm sóng; $|\psi|^2$: mật độ xác suất.

> [!warning] Quy ước quan trọng
> $h\nu=\hbar\omega$ và $p=\hbar k=h/\lambda$. Không được trộn $\nu$ với $\omega$, hoặc số sóng $k$ với bước sóng $\lambda=2\pi/k$.

---

## 1. Các đặc điểm của vật lý học cổ điển

### 1.1. Giả định nền

- Trạng thái vật lý được mô tả bằng vị trí, vận tốc và các trường liên tục.
- Quỹ đạo và định luật tiến triển có thể xác định: với trạng thái ban đầu và trường ngoại tác dụng, trạng thái tương lai được suy ra từ định luật.
- Năng lượng có thể biến thiên liên tục; không có bước năng lượng tối thiểu phổ quát.
- Trạng thái cơ học là một điểm trong không gian pha, không phải một vectơ trạng thái trong không gian Hilbert.
- Các đại lượng đo được được gán sẵn một giá trị trong mô tả trạng thái cổ điển.

### 1.2. Phạm vi hiệu lực

Vật lý cổ điển mô tả rất tốt khi:

- đối tượng có kích thước lớn hơn nhiều bước sóng de Broglie;
- hành động cơ học đặc trưng $S\gg\hbar$;
- hiệu ứng lượng tử nhỏ so với sai số quan sát;
- dao động nhiều chu kỳ, nhiều hạt hoặc ở nhiệt độ cao đủ để các dao động lượng tử bị kích thích dày đặc.

### 1.3. Những giới hạn buộc phải sửa đổi

| Hiện tượng | Dự đoán cổ điển | Mâu thuẫn thực nghiệm |
| --- | --- | --- |
| Phổ bức xạ vật đen | Rayleigh–Jeans tiên tới vô hạn ở sóng ngắn | Phổ đo suy giảm, không tiên tới vô hạn |
| Hiệu ứng quang điện | Năng lượng tích luỹ theo cường độ, không có ngưỡng | Có ngưỡng tần số; năng lượng electron tăng theo tần số |
| Va chạm nguyên tử | Năng lượng truyền liên tục | Năng lượng truyền theo các bước rời |
| Giao thoa và nhiễu xạ electron | Hạt chỉ có quỹ đạo | Electron tạo vân giao thoa |
| Phổ nguyên tử | Dao động liên tục | Chỉ xuất hiện một số vạch rời rạc |

> [!success] Cách hiểu đúng
> Vật lý lượng tử không đơn giản là “vật lý cổ điển sai hoàn toàn”; nó là lý thuyết tổng quát hơn, trong đó vật lý cổ điển xuất hiện như một giới hạn thích hợp.

---

## 2. Tính chất hạt của bức xạ

### 2.1. Bức xạ nhiệt và vật đen tuyệt đối

Bức xạ nhiệt phát sinh khi vật có nhiệt độ. Vật đen tuyệt đối hấp thụ mọi bức xạ chiếu vào và là chuẩn để nghiên cứu phổ nhiệt.

- Hốc bức xạ là mô hình thực nghiệm gần với vật đen tuyệt đối.
- Phổ phụ thuộc vào $T$ và khác nhau theo bước sóng hay tần số.
- Định luật dịch chuyển Wien:
  $\lambda_{\max}T=2{,}898\times10^{-3}\ \mathrm{m\,K}$.
- Xem [[Bức xạ nhiệt và vật đen tuyệt đối]] và [[Thí nghiệm - Bức xạ vật đen]].

### 2.2. Định luật Stefan–Boltzmann

Tổng công suất trên mỗi đơn vị diện tích của vật đen là:

$M=\sigma T^4$,

$\sigma=5{,}670374419\times10^{-8}\ \mathrm{W\,m^{-2}\,K^{-4}}$.

Định luật này cho toàn phổ, không cho phân bố cường độ theo bước sóng. Với vật thật:

$M=\varepsilon\sigma T^4$.

Xem [[Định luật Stefan-Boltzmann]].

### 2.3. Định luật Rayleigh–Jeans và sự khủng hoảng ở miền tử ngoại

Trong miền sóng dài $h\nu\ll k_BT$, vật lý cổ điển cho:

$B_\lambda(T)\approx\frac{2ck_BT}{\lambda^4}$

hoặc theo tần số:

$B_\nu(T)\approx\frac{2\nu^2k_BT}{c^2}$.

Khi $\lambda\to0$, công thức dự đoán $B_\lambda\to\infty$: đây là **thảm họa tử ngoại**. Nguyên nhân là cơ học cổ điển cho phép số mode tần số cao tăng không giới hạn nhưng vẫn gán mỗi mode năng lượng trung bình $k_BT$.

Xem [[Định luật Rayleigh-Jeans]].

### 2.4. Thuyết lượng tử năng lượng của Planck

Planck giả thiết dao động tử trao đổi năng lượng theo bước $h\nu$:

$E_n=nh\nu$, $n=0,1,2,\ldots$

Đây là cách ghi lịch sử, tính năng lượng tương đối so với trạng thái nền. Trong mô hình dao động tử lượng tử đầy đủ, năng lượng toàn phần là $E_n=(n+\tfrac12)h\nu$; bước nhảy vẫn là $h\nu$.

Năng lượng trung bình của dao động tử là:

$\overline E=\frac{h\nu}{\exp(h\nu/k_BT)-1}$.

Từ đó thu được phổ Planck theo bước sóng:

$B_\lambda(T)=\frac{2hc^2}{\lambda^5}\frac{1}{\exp\!\left(\frac{hc}{\lambda k_BT}\right)-1}$.

Công thức cho:

- $h\nu\ll k_BT$: trở về Rayleigh–Jeans;
- $h\nu\gg k_BT$: bức xạ bị suy giảm theo số mũ, khớp dạng Wien.

> [!info] Giới hạn lịch sử
> Planck mới lượng tử hóa năng lượng của **dao động tử**. Ông chưa khẳng định rằng chính trường điện từ luôn gồm các hạt photon. Bước tiếp theo là của Einstein.

Xem [[Giả thuyết - Lượng tử năng lượng Planck]].

---

## 3. Thuyết lượng tử ánh sáng của Einstein

### 3.1. Hiệu ứng quang điện

Ánh sáng chiếu vào bề mặt kim loại có thể làm electron thoát ra. Nếu dùng lý thuyết sóng liên tục, năng lượng phải tích luỹ dần; thực nghiệm cho thấy hiệu ứng xuất hiện gần như tức thời khi tần số vượt ngưỡng.

Xem [[Hiệu ứng quang điện]].

### 3.2. Các định luật quang điện

1. Có tần số ngưỡng $\nu_0$; nếu $\nu<\nu_0$, tăng cường độ cũng không làm electron thoát trong mô hình đơn photon.
2. Động năng cực đại phụ thuộc tuyến tính với tần số, không phụ thuộc cường độ.
3. Cường độ tăng làm số electron thoát mỗi đơn vị thời gian tăng; dòng quang điện bão hòa thay đổi theo số photon tới.

Định luật Einstein cho:

$K_{\max}=h\nu-\phi$ khi $h\nu\geq\phi$,

trong đó $\phi$ là công thoát. Tần số ngưỡng và điện thế hãm thỏa:

$\phi=h\nu_0$, $eV_h=K_{\max}$.

### 3.3. Thuyết lượng tử ánh sáng của Einstein

Einstein đề xuất rằng ánh sáng gồm các lượng tử năng lượng, gọi là photon:

$E_\gamma=h\nu=\frac{hc}{\lambda}$.

Từ quan hệ tương đối tính $E^2=p^2c^2+m_0^2c^4$ với $m_0=0$, suy ra:

$p_\gamma=\frac{E_\gamma}{c}=\frac{h}{\lambda}=\hbar k$.

Một photon trao năng lượng trong một tương tác cơ bản. Cường độ sóng xác định số photon tới mỗi đơn vị thời gian, còn mỗi photon mang cùng năng lượng $h\nu$.

Xem [[Giả thuyết - Hạt ánh sáng (Photon)]].

---

## 4. Hiệu ứng Compton

Tán xạ photon trên electron tự do ban đầu đứng yên làm thay đổi cả năng lượng và động lượng của photon:

$h\nu+m_ec^2=h\nu'+E_e$,

$\vec p_\gamma=\vec p_\gamma'+\vec p_e$.

Kết quả thực nghiệm:

$\Delta\lambda=\lambda'-\lambda=\lambda_C(1-\cos\theta)$,

$\lambda_C=\frac{h}{m_ec}\approx2{,}426\times10^{-12}\ \mathrm{m}$.

Độ dịch không phụ thuộc bước sóng tới, chỉ phụ thuộc vào góc tán và đạt cực đại $2\lambda_C$ khi $\theta=\pi$. Công thức trực tiếp kiểm chứng $p_\gamma=h/\lambda$.

Xem [[Hiệu ứng Compton]].

---

## 5. Giả thuyết De Broglie — tính chất sóng của hạt vật chất

### 5.1. Lưỡng tính sóng–hạt của ánh sáng

| Bố trí hoặc hiện tượng | Mặt thể hiện chủ yếu |
| --- | --- |
| Giao thoa, nhiễu xạ, khe đôi | Sóng |
| Hiệu ứng quang điện, tán Compton, đếm photon rời rạc | Hạt |

Ánh sáng không phải lúc “là sóng”, lúc khác “là hạt”. Bố trí thí nghiệm và phép đo quyết định mặt tính chất được thể hiện. Xem [[Lưỡng tính sóng-hạt]].

### 5.2. Giả thuyết de Broglie về sóng vật chất

De Broglie mở rộng quan hệ Planck–Einstein cho mọi hạt:

$\boxed{\lambda=\frac{h}{p}=\frac{2\pi}{k}}$.

Phi tương đối tính:

$\lambda=\frac{h}{mv}$.

Tương đối tính:

$\lambda=\frac{h}{\gamma m_0v}$.

Sóng vật chất là biên độ xác suất, không phải sóng cơ của vật chất uốn lượn. Xem [[Giả thuyết - Sóng de Broglie]].

### 5.3. Thí nghiệm kiểm chứng giả thuyết de Broglie

Trong thí nghiệm Davisson–Germer, electron gia tốc qua hiệu điện thế $V$ có:

$p=\sqrt{2m_e eV}$ và

$\lambda=\frac{h}{\sqrt{2m_e eV}}\approx\frac{12{,}27}{\sqrt{V}}\ \text{Å}$ (xấp xỉ phi tương đối tính, với $V$ tính bằng volt).

Chùm electron nhiễu xạ trên tinh thể niken và tạo cực đại tán xạ đúng với bước sóng dự đoán. Sau đó, giao thoa electron qua hai khe, kính hiển vi điện tử và nhiễu xạ neutron cũng xác nhận tính sóng của vật chất.

Xem [[Thí nghiệm - Davisson-Germer]].

---

## 6. Hàm sóng của hạt vi mô — ý nghĩa thống kê

### 6.1. Hàm sóng của hạt tự do

Phương trình Schrödinger một chiều:

$i\hbar\frac{\partial\psi}{\partial t}=-\frac{\hbar^2}{2m}\frac{\partial^2\psi}{\partial x^2}$.

Nghiệm sóng phẳng:

$\Psi_{\vec p}(\vec r,t)=A\exp\!\left[\frac{i}{\hbar}(\vec p\cdot\vec r-Et)\right]$.

Sóng phẳng có $p$ xác định nhưng trải trên toàn không gian, nên trạng thái định xứ phải dùng tổng liên hợp của nhiều số sóng. Xem [[Hàm sóng]] và [[Phương trình Schrödinger]].

### 6.2. Ý nghĩa thống kê của hàm sóng

Theo quy tắc Born:

$dP=|\psi|^2\,d^3r$,

$P_V=\int_V|\psi|^2\,d^3r$.

Hàm sóng phức; mật độ xác suất là thực không âm. Giao thoa là cộng các biên độ trước khi lấy mô đô, và pha toàn cục không đổi kết quả phép đo. Xem [[Xác suất thống kê]].

### 6.3. Sự chuẩn hóa hàm sóng

Điều kiện chuẩn hóa:

$\int|\psi(\vec r,t)|^2\,d^3r=1$.

Nếu tích phân bằng $N$ hữu hạn và khác không, hàm sóng được chia cho $\sqrt N$. Chuẩn hóa bảo đảm tổng xác suất bằng một.

Với thế năng chỉ phụ thuộc vị trí, dòng xác suất là:

$\vec j=\frac{\hbar}{m}\operatorname{Im}(\psi^*\nabla\psi)$.

### 6.4. Điều kiện tiêu chuẩn của hàm sóng

Hàm sóng vật lý phải vuông giao được, đơn trị, thuộc miền của Hamiltonian và thỏa điều kiện biên. Tính trơn tru được quy định bởi thế năng: với thế năng hữu hạn liên tục, hàm sóng và các đạo hàm cần thiết phải liên tục. Ví dụ:

- tường vô hạn: $\psi=0$ tại tường;
- miền vô hạn: $\psi$ phải vuông giao được; khi áp dụng bảo toàn dòng, dòng biên phải triệt tiêu;
- vòng tròn: điều kiện chu kỳ;
- điểm nhảy thế hữu hạn: $\psi$ và $\partial\psi/\partial x$ liên tục.

Xem [[Hàm sóng]].

---

## 7. Bó sóng

### 7.1. Bó sóng định xứ

Bó sóng là tổng liên hợp của một dải số sóng quanh $k_0$:

$\psi(x,t)=\int\widetilde\psi(k,0)e^{i[kx-\omega(k)t]}\,dk$.

Mỗi số sóng gắn với động lượng $p=\hbar k$. Bó hẹp về vị trí có dải $k$ rộng, nên động lượng kém xác định; đó là trạng thái định xứ vật lý. Xem [[Bó sóng lượng tử]].

### 7.2. Bó sóng và hệ thức bất định

Vì $\Delta p_x=\hbar\Delta k_x$:

$\Delta x\,\Delta p_x=\hbar\Delta x\,\Delta k_x\geq\frac{\hbar}{2}$.

Bó càng hẹp về vị trí càng có độ bất định động lượng lớn; bó càng hẹp về động lượng càng kéo dài trong không gian. Xem [[Nguyên lý bất định Heisenberg]].

### 7.3. Chuyển động của bó sóng

Tốc độ pha và tốc độ nhóm:

$v_{\mathrm{ph}}=\frac{\omega}{k}$, $v_g=\frac{d\omega}{dk}$.

Các điểm cùng pha dịch theo $v_{\mathrm{ph}}$, còn bao bọc của bó hẹp dịch gần theo $v_g$.

**Hạt tự do phi tương đối tính:**

$\omega(k)=\frac{\hbar k^2}{2m}$,

$v_{\mathrm{ph}}=\frac{v}{2}$, $v_g=v=\frac{p}{m}$.

Đối với bó tự do hẹp, vận tốc cơ học của hạt được biểu hiện bằng vận tốc nhóm, không phải vận tốc pha. Vận tốc pha không đại diện cho vận tốc vật hay tốc độ truyền thông.

**Hạt tự do tương đối tính:**

$v_g=\frac{pc^2}{E}=v$, $v_{\mathrm{ph}}=\frac{c^2}{v}$.

Do đó $v_{\mathrm{ph}}v_g=c^2$. Vận tốc pha có thể vượt $c$ mà không vi phạm tương đối tính vì nó không truyền thông tin.

**Lan giãn:** vì các thành phần có tốc độ nhóm khác nhau, bó thay đổi hình dạng. Với bó Gaussian tối ưu, tâm chuyển động đều:

$\langle x\rangle(t)=x_0+\frac{p_0}{m}t$,

nhưng bề rộng tăng:

$(\Delta x)^2(t)=\sigma_0^2+\left(\frac{\hbar t}{2m\sigma_0}\right)^2$.

Bó vẫn bão hòa bất định Heisenberg. Vì “tốc độ nhóm = vận tốc hạt” chỉ là kết luận đơn giản cho bó tự do hẹp, trong thế có thế phải xét cả lực và chế độ dao động của tâm bó.

---

## Chuỗi lý luận của chương

1. Phổ vật đen không thể giải thích bằng cơ học cổ điển.
2. Planck lượng tử hóa năng lượng dao động tử và thu được đúng toàn phổ.
3. Hiệu ứng quang điện buộc Einstein giả thiết photon có năng lượng $h\nu$.
4. Compton chứng minh photon còn mang động lượng $h/\lambda$.
5. de Broglie mở rộng quan hệ sóng–hạt cho vật chất.
6. Giao thoa và nhiễu xạ chứng minh hạt có mặt sóng.
7. Hàm sóng và bó sóng mô tả trạng thái lượng tử, xác suất và chuyển động của hạt.

> [!tip] Kết nối với giới hạn cổ điển
> Khi dải số sóng của bó hẹp lại, các thành phần có tốc độ nhóm gần nhau, bó ít lan và tâm bó tiến gần vận tốc cổ điển. Khi hiệu ứng lượng tử nhỏ hơn sai số quan sát, bộ mô tả cổ điển là giới hạn thực dụng của bộ mô tả lượng tử.

## Câu hỏi tự kiểm

1. Vì sao Rayleigh–Jeans không thể mô tả toàn phổ bức xạ vật đen?
2. Phân biệt lượng tử năng lượng của Planck với photon của Einstein.
3. Tại sao cường độ ánh sáng không quyết định $K_{\max}$ trong hiệu ứng quang điện đơn photon?
4. Vì sao độ dịch Compton độc lập với bước sóng photon tới?
5. Phân biệt mặt sóng và mặt hạt của ánh sáng bằng ví dụ thí nghiệm.
6. Vì sao sóng phẳng không phải trạng thái chuẩn hóa trên toàn không gian?
7. Cho biết ý nghĩa thống kê chính xác của $|\psi|^2$.
8. Giải thích tại sao bó sóng vừa định xứ tốt vừa có động lượng bất định.
9. Vì sao vận tốc pha có thể vượt tốc độ ánh sáng mà không làm mất nguyên lý tương đối tính?
10. Vì sao với một bó rộng, vận tốc nhóm tại $k_0$ không mô tả đầy đủ chuyển động của từng thành phần bó?

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[MOC - Giả thuyết và Thực nghiệm]]
- [[Tiên đề cơ học lượng tử]]
- [[Phương trình Schrödinger]]
- [[Nguyên lý bất định Heisenberg]]
- [[Biến đổi Fourier]]
- [[Xác suất thống kê]]
