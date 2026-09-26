---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: quang-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Phân cực ánh sáng

> [!abstract] Ý chính
> Phân cực ánh sáng mô tả hướng dao động của trường điện trong [[Sóng điện từ và thang sóng điện từ]] — hiện tượng thể hiện rõ tính sóng của ánh sáng, là cơ sở của kính phân cực, màn hình LCD, kính râm, và đo lường quang học hiện đại.

## Nội dung

- **Bản chất:** ánh sáng là sóng ngang; hướng dao động của $\vec E$ quyết định trạng thái phân cực.
- **Phân cực thẳng:** $\vec E$ dao động theo một phương cố định.
  - Cường độ qua bộ phân cực: $I = I_0 \cos^2\theta$ — định luật Malus; $\theta = 90°$ → $I = 0$ (hai kính chéo nhau triệt tiêu).
- **Phân cực tròn:** tổng của hai phân cực thẳng cùng biên độ, lệch pha $\pm\pi/2$ → đầu mút $\vec E$ vẽ đường tròn; dấu pha quyết định chiều quay (phải/trái).
- **Phân cực elip:** tổng của hai phân cực thẳng biên độ khác nhau, lệch pha tùy ý — trạng thái tổng quát nhất.
- **Cách tạo phân cực:**
  - Hấp thụ chọn lọc (kính Polaroid — chuỗi polymer định hướng),
  - Phản xạ tại góc Brewster (tan $\theta_B = n_2/n_1$; với thủy tinh $n = 1{,}5$ → $\theta_B \approx 56{,}3°$ — tia phản xạ phân cực hoàn toàn vuông góc mặt phẳng tới),
  - Lưỡng chiết (tinh thể calcite: hai chiết suất theo hai trục → tách tia thường/tia bất thường),
  - Bản bước sóng $\lambda/4$, $\lambda/2$ (tạo lệch pha điều khiển được).

## Bảng: trạng thái phân cực

| Trạng thái | Điều kiện của $\vec E$ | Tạo bằng | Mô tả bằng |
| --- | --- | --- | --- |
| Thẳng | dao động 1 phương | kính phân cực, Brewster | vector Jones thực |
| Tròn | thành phần bằng nhau, lệch pha $\pm\pi/2$ | polarizer 45° + bản $\lambda/4$ | $J = \frac{1}{\sqrt2}\binom{1}{\pm i}$ |
| Elip | biên độ khác, pha tùy ý | bản $\lambda/4$ + polarizer góc tùy ý | tổng quát |

## Ví dụ vật lý cụ thể

- **"Nghịch lý" ba kính phân cực:** hai kính chéo nhau (90°) triệt tiêu hoàn toàn; nhưng chèn kính thứ ba ở 45° vào giữa thì ánh sáng lại lọt qua: qua kính 1 (0°) → $I_0/2$; qua kính 2 (45°) → nhân $\cos^2 45° = 1/2$; qua kính 3 (90°) → nhân tiếp $1/2$ → $I = I_0/8$. Mỗi kính "xoay" dần hướng phân cực — minh họa Malus tuần tự.
- **Bầu trời và ong:** ánh sáng Mặt Trời tán xạ bởi khí quyển bị phân cực một phần theo phương vuông góc tia tới — ong định hướng bằng bầu trời phân cực kể cả khi trời râm; mắt thường thấy khi nhìn qua kính phân cực xoay (bầu trời sáng/tối đổi chỗ).
- **Kính 3D rạp chiếu:** hai hình ảnh phân cực vuông góc nhau, kính cũng phân cực vuông góc → mỗi mắt chỉ nhận đúng ảnh của mình.
- **Vật lý sóng vô tuyến:** ăng-ten thu chỉ nhận đúng điện trường song song với phương ăng-ten — xoay ăng-ten 90° sẽ mất tín hiệu (ứng dụng ngay của Malus).

## Kiểm chứng & giới hạn

- Kiểm chứng: định luật Malus đo bằng photodiode; góc Brewster; phân cực CMB (xem [[Ký hiệu Stokes]]).
- Ánh sáng **không phân cực** (đèn sợi đốt, Mặt Trời trực tiếp): hướng $\vec E$ thay đổi hỗn loạn nhanh — mô tả bằng vector Jones tổng không được; phải dùng [[Ký hiệu Stokes]] (không cần pha).
- Ở mức lượng tử: một photon đơn có trạng thái phân cực riêng; phép đo qua kính phân cực cho kết quả xác suất (liên hệ [[Nguyên lý chồng chất lượng tử]]) — nhưng các ứng dụng cổ điển trên vẫn đúng vì số photon khổng lồ.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Sóng điện từ và thang sóng điện từ]]: ánh sáng là sóng điện từ.
- [[Giao thoa ánh sáng]]: phân cực ảnh hưởng đến vân giao thoa.
- [[Nhiễu xạ ánh sáng]]: kính phân cực trước detector giúp giảm nhiễu.
- [[Ký hiệu Jones]] · [[Ký hiệu Stokes]]: toán học mô tả trạng thái phân cực.
- [[Nguyên lý chồng chất lượng tử]]: phân cực photon đơn ở mức lượng tử.

## Câu hỏi mở

- Vì sao kim loại có thể tạo bộ phân cực tốt nhờ hiệu ứng Kerr và Faraday? (Gợi ý: dao động cộng hưởng của electron tự do hấp thụ chọn lọc theo phương — nhưng chi tiết trường điện từ trong dây dẫn phức tạp hơn nhiều.)
- Tia phản xạ ở góc Brewster phân cực vuông góc mặt phẳng tới — vì sao tia khúc xạ **không bao giờ phân cực hoàn toàn**, chỉ phân cực một phần? (Gợi ý: xấp xỉ biên độ Fresnel — giải thích đầy đủ cần phương trình Maxwell tại biên.)