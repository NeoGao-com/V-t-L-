---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Hạt tự do trong cơ học lượng tử

> [!abstract] Ý chính
> Hạt tự do ($V = 0$) có phổ năng lượng liên tục $E = \dfrac{\hbar^2k^2}{2m}$, nghiệm là sóng phẳng $e^{ikx}$ không chuẩn hóa được theo nghĩa thông thường — trạng thái vật lý thực tế là bó sóng (chồng chập sóng phẳng) dịch chuyển với vận tốc nhóm $v = \dfrac{p}{m}$ và giãn rộng theo thời gian.

## Phát biểu / Định nghĩa

Phương trình Schrödinger dừng với $V(x) = 0$:

$-\dfrac{\hbar^2}{2m}\psi''(x) = E\psi(x)$

- Nghiệm: $\psi_k(x) = Ae^{ikx} + Be^{-ikx}$ với $k = \dfrac{\sqrt{2mE}}{\hbar}$, $E = \dfrac{\hbar^2k^2}{2m} \ge 0$ — **phổ liên tục**, mọi $E > 0$ đều cho phép, mỗi mức hai nghiệm độc lập (chẵn $e^{\pm ikx}$).
- Nghiệm chuẩn hóa delta: $\psi_p(x) = \dfrac{1}{\sqrt{2\pi\hbar}}\,e^{ipx/\hbar}$ thỏa $\langle\psi_p|\psi_{p'}\rangle = \delta(p-p')$ — dùng tích phân Fourier thay cho chuẩn hóa thông thường.
- Sóng phẳng thuần túy $e^{i(kx-\omega t)}$ với $\omega = \dfrac{\hbar k^2}{2m}$: mật độ $|\Psi|^2$ không đổi trên toàn trục, **không đại diện hạt ở một chỗ**; đây là trạng thái động lượng chính xác (xung lượng xác định, vị trí hoàn toàn bất định — [[Nguyên lý bất định Heisenberg]]).

**Trạng thái vật lý: bó sóng.** Chồng chập các sóng phẳng:

$\Psi(x,t) = \dfrac{1}{\sqrt{2\pi\hbar}}\displaystyle\int\varphi(p)\,e^{i(px-Et)/\hbar}\,dp$

- Hạt định xứ nơi $p \approx p_0$; bó dịch chuyển với vận tốc nhóm $v_g = \left.\dfrac{d\omega}{dk}\right|_{k_0} = \dfrac{\hbar k_0}{m} = \dfrac{p_0}{m}$.
- Bó **giãn rộng** tuyến tính theo thời gian: $\sigma_x(t) = \sqrt{\sigma_{x0}^2 + \left(\dfrac{\sigma_p t}{m}\right)^2}$ — hệ quả tán sắc $\omega = \omega(k)$ bậc hai (xem [[Bó sóng lượng tử]]).

## Suy luận từ đâu

- Tiên đề gốc: phương trình Schrödinger dừng với $V = 0$; tiên đề động lượng $\hat p = -i\hbar\dfrac{\partial}{\partial x}$.
- Công cụ toán: tích phân Fourier và hàm delta Dirac ([[Biến đổi Fourier]], [[Hàm Dirac delta]]).

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: lan truyền chùm electron/neutron tự do (nhiễu xạ, giao thoa sóng vật chất) khớp với bó sóng; vận tốc nhóm đo được bằng thời gian bay đúng $p/m$.
- Trường hợp không còn đúng: sóng phẳng lý tưởng không tồn tại trong thực tế (không chuẩn hóa được, chiếm toàn không gian); khi có thế bên ngoài, nghiệm tự do chỉ là phép xấp xỉ cục bộ.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Bó sóng lượng tử]]
- [[Lưỡng tính sóng-hạt]]
- [[Biến đổi Fourier]]
- [[Hàm Dirac delta]]
- [[Chuyển động một chiều trong cơ học lượng tử]]

## Câu hỏi mở

- Một bó sóng lan truyền trong không gian tự do có "tan biến" hoàn toàn — hay chỉ mật độ giảm vì giãn rộng? (Bảo toàn xác suất, chỉ phân bố loãng ra.)
- Vì sao hạt tự do không có mức năng lượng gián đoạn — và điều gì xảy ra khi giam trong hộp hữu hạn? (Xem [[Giếng thế vô hạn]].)