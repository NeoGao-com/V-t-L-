---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Hiệu ứng Zeeman

> [!abstract] Ý chính
> Từ trường ngoài phá đối xứng quay của nguyên tử: năng lượng thêm $\Delta E = \mu_B B\,m_l$ tách mỗi mức vào $2l+1$ mức con (Zeeman thường — từ mômen từ quỹ đạo), và khi spin tham gia thành $2J+1$ mức con với hệ số $g_J$ (Zeeman bất thường) — quang phổ tách vạch này chính là "kính lúp" đo từ trường và là bằng chứng của spin.

## Phát biểu / Định nghĩa

**2. Sự tách mức năng lượng của nguyên tử Hydro trong từ trường:**

Từ trường đều $\vec B = B\hat z$ bổ sung nhiễu loạn $\hat H' = -\hat{\vec\mu}\cdot\vec B = \mu_B B\,\dfrac{\hat L_z}{\hbar}$ (theo [[Mômen động lượng quỹ đạo và mômen từ quỹ đạo]]), làm tách mức năng lượng:

$E_{nlm_l} = E_n + \mu_B B\,m_l, \qquad m_l = -l,\dots,+l$

- Mỗi mức $E_n$ (ứng $l$) tách thành $2l+1$ mức con cách đều nhau $\Delta E = \mu_B B$ — gọi là **Zeeman thường**.
- Kèm quy tắc chọn lọc $\Delta m_l = 0,\ \pm1$: mỗi vạch quang phổ trở thành **bộ ba Zeeman** ($\pi$ không phân cực/cân bằng, $\sigma^\pm$ phân cực tròn) — xem [[Quang phổ]].
- Cực tiểu bậc $\mu_B B \sim 5{,}8\times10^{-5}$ eV cho $B = 1$ T — rất nhỏ so với khoảng cách mức $E_n$ ($\sim 13{,}6$ eV): phân giải cần quang phổ kế độ phân giải cao.

**Zeeman bất thường (có spin):**

Khi kể [[Spin của hạt vi mô]], mômen từ toàn phần $\vec\mu = \vec\mu_L + \vec\mu_s$ với $g_s \approx 2$ không cùng tỉ lệ từ–cơ; với trường yếu, lượng bảo toàn là $\hat{\vec J} = \hat{\vec L} + \hat{\vec S}$ và:

$\Delta E = g_J\,\mu_B B\,m_J, \qquad g_J = 1 + \dfrac{J(J+1) + S(S+1) - L(L+1)}{2J(J+1)}$ (hệ số Landé)

- $g_J$ phụ thuộc $L, S, J$ ⟹ tách nhiều vạch hơn $2l+1$ — thực nghiệm "bất thường" thời 1896–1925 mãi giải thích được sau khi spin ra đời (thực ra mới là trường hợp phổ biến nhất).
- Trường mạnh (Paschen–Back): $\vec L$ và $\vec S$ tách rời, $\Delta E = \mu_B B(m_l + 2m_s)$.

## Suy luận từ đâu

- Tiên đề gốc: nhiễu loạn bậc nhất $\Delta E = \langle nlm|\hat H'|nlm\rangle$ (lý thuyết nhiễu loạn dừng — [[Toán tử mô-men xung lượng]], [[Nguyên tử Hydro]]).
- Công cụ: [[Mômen động lượng quỹ đạo và mômen từ quỹ đạo]], tính phổ của $\hat L_z$; quy tắc chọn lọc từ phần tử ma trận ([[Phép đo lượng tử]]).

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: vạch D của natri và các mức hydro trong từ trường tách đúng $\mu_B B$; **đo từ trường sao/bằng việc phân tích quang phổ Zeeman** (từ trường Mặt Trời $\sim 0{,}1$–$0{,}4$ T, sao từ $\sim 10^8$ T); độ tách này là công cụ chuẩn của thiên văn học và plasma.
- Trường hợp không còn đúng: cần thêm cấu trúc tinh tế (spin–quỹ đạo) và siêu tinh tế (spin hạt nhân) khi $B$ yếu cỡ mức $\mu_B B \ll$ khoảng cách tinh tế; trong trường rất mạnh ($B \gtrsim 10^4$ T, sao neutron) cả Zeeman lẫn cấu trúc tinh tế bị trộn — cần phổ đầy đủ nhiễu loạn bậc hai (phần trăm).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Mômen động lượng quỹ đạo và mômen từ quỹ đạo]]
- [[Spin của hạt vi mô]]
- [[Nguyên tử Hydro]]
- [[Quang phổ]]
- [[Toán tử mô-men xung lượng]]

## Câu hỏi mở

- Zeeman bất thường đã "thách thức" cơ học lượng tử non trẻ 1896–1925 — lý thuyết vector model ($g_J$) của Landé đã được hình thành thế nào trước khi spin được chấp nhận?
- Ở sao neutron ($B\sim10^8$–$10^{11}$ T), cách nào để tính phổ "đảo ngược" — khi $\mu_B B$ vượt cả năng lượng liên kết Coulomb?