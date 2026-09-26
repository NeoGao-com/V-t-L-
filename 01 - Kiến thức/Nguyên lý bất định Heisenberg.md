---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Nguyên lý bất định Heisenberg

> [!abstract] Ý chính
> Không thể đo chính xác đồng thời vị trí và động lượng của một hạt lượng tử vượt qua ngưỡng do hằng số Planck quy định — đây là tính chất nội tại của vật lý vi mô, không phải hạn chế kỹ thuật của dụng cụ đo.

## Biểu thức toán học

$\Delta x \cdot \Delta p \ge \frac{\hbar}{2}$

với $\hbar = h / 2\pi$. Nguyên nhân sâu xa: các toán tử $\hat x$ và $\hat p$ **không giao hoán** — $[\hat x, \hat p] = i\hbar$ (xem [[Tiên đề cơ học lượng tử]] và [[Đại số tuyến tính]]).

Dạng tổng quát cho mọi cặp liên hợp: $\Delta A \cdot \Delta B \ge \frac{1}{2}\left|\langle[\hat A, \hat B]\rangle\right|$.

## Bảng các cặp đại lượng liên hợp

| Cặp liên hợp | Hệ thức | Ví dụ ứng dụng |
| --- | --- | --- |
| Vị trí – động lượng | $\Delta x \Delta p \ge \hbar/2$ | Giới hạn độ phân giải kính hiển vi |
| Năng lượng – thời gian | $\Delta E\,\Delta t \sim \hbar$ (ước lượng) | Bề rộng vạch phổ; thời gian sống của trạng thái, không phải cặp toán tử chuẩn |
| Góc quay – mô-men động lượng $z$ | $\Delta\varphi\,\Delta L_z \ge \hbar/2$ | Mô-men quay orbital quanh trục $z$ |

## Ví dụ vật lý cụ thể

- **Electron trong hố 1 nm:** $\Delta x \sim 1$ nm → $\Delta p \ge \dfrac{\hbar}{2\Delta x} \approx 5{,}3 \times 10^{-26}$ kg·m/s → $\Delta v \approx 58$ km/s. Một electron "đứng yên" trong hố nhỏ thực ra luôn chuyển động náo loạn — đây là nguồn gốc năng lượng điểm không ($E_1 \approx 0{,}38$ eV khi giải đầy đủ bằng [[Phương trình Schrödinger]]).
- **Hạt bụi 1 μg, $\Delta x$ = 1 μm:** $\Delta v \approx 5 \times 10^{-20}$ m/s — nhỏ hơn mọi tốc độ đo được. Giải thích vì sao vĩ mô **không bao giờ thấy** bất định: hiệu ứng giảm như $1/(m\Delta x)$.
- **Vạch phổ có bề rộng:** trạng thái kích thích sống $\Delta t \sim 10^{-8}$ s có năng lượng bất định ở mức $\Delta E\sim\hbar/\Delta t\approx1{,}05\times10^{-26}$ J ≈ $6{,}6\times10^{-8}$ eV — nguyên nhân vạch quang phổ không "mảnh" tuyệt đối. Đây là quan hệ ước lượng giữa bề rộng phổ và thời gian sống, không phải một bất định Robertson chuẩn với toán tử thời gian; hệ số phụ thuộc quy ước về bề rộng vạch.

## Bản chất

- Bất định là **tính chất cơ bản của tự nhiên** ở thang vi mô, không phải do thiết bị đo kém (nếu máy đo hoàn hảo, bất định vẫn còn).
- Hệ quả: không tồn tại đồng thời "vị trí chính xác" và "động lượng chính xác" — khái niệm quỹ đạo như đường kẻ trong [[Mẫu nguyên tử Bohr]] chỉ là xấp xỉ.

## Kiểm chứng & giới hạn

- Thực nghiệm: mọi kiểm nghiệm của cơ học lượng tử (quang phổ, khe đôi, hiệu ứng quang điện, [[Thí nghiệm - Franck-Hertz]]...) đều nhất quán với hệ thức; chưa từng có vi phạm nào.
- Trường hợp không còn đúng: ở thang Planck ($\sim 10^{-35}$ m), bất định vị trí–động lượng đủ lớn để "bẻ cong" không-thời gian — cần lý thuyết hấp dẫn lượng tử để nói tiếp.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Tiên đề cơ học lượng tử]]: note mẹ chứa bộ tiên đề và lời giải chi tiết.
- [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]: MOC Chương 3 — bất định như hệ quả của bộ tiên đề.
- [[Suy ra hệ thức bất định từ giao hoán]]: chứng minh Robertson từ bất đẳng thức Cauchy–Schwarz.
- [[Phương trình Schrödinger]]: nghiệm của phương trình tự động thỏa mãn bất định.
- [[Đại số tuyến tính]]: bất định xuất phát từ tính không giao hoán của toán tử.
- [[Mẫu nguyên tử Bohr]]: các mức năng lượng bị giới hạn bởi nguyên lý bất định.
- [[Quang phổ]]: bề rộng vạch phổ từ $\Delta E\Delta t$.
- [[Lưỡng tính sóng-hạt]]: bất định là mặt toán học của lưỡng tính.
- [[Bó sóng lượng tử]]: minh họa trực giác bằng sự phân tán số sóng và lan giãn của bó.
- [[MOC - Chương 1 - Cơ sở vật lý của cơ học lượng tử]]: bản đồ các bằng chứng dẫn tới cơ học lượng tử.

## Câu hỏi mở

- Trạng thái nén (squeezed state) có "lách" được bất định không? (Không — chỉ nén sai số về một chiều để đổi lấy chiều kia; tích hai sai số không đổi.)
- Nếu chấp nhận bất định là nội tại, thì "hiện thực khách quan độc lập với phép đo" còn ý nghĩa gì? (Vấn đề triết học nền tảng của cơ học lượng tử.)
- Tại thang Planck, bất định vị trí làm không-thời gian "sủi bọt" — hình học cổ điển có còn áp dụng được không?