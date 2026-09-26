---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: tương-đối
trạng-thái: ổn-định
created: 2026-09-25
---

# Biến đổi Einstein

> [!abstract] Ý chính
> Biến đổi Lorentz là nền tảng của thuyết tương đối hẹp: biến đổi vị trí, thời gian và động lượng giữa các hệ quy chiếu quán tính chuyển động đều với nhau, giữ bất biến khoảng không-thời gian $s^2 = (ct)^2 - x^2 - y^2 - z^2$.

## Nội dung

- **Các đại lượng 4-vector:**
  - **Vị trí-4:** $x^\mu = (ct, x, y, z)$
  - **Động lượng-4:** $p^\mu = (E/c, p_x, p_y, p_z)$
- **Phép biến đổi Lorentz** (tốc độ $v$ theo trục $x$):
  $t' = \gamma (t - vx/c^2), \quad x' = \gamma (x - vt), \quad y' = y, \quad z' = z$
  với $\gamma = \dfrac{1}{\sqrt{1 - v^2/c^2}}$ là hệ số Lorentz.
- **Các bất biến (invariant):**
  - **Khoảng không-thời gian:** $s^2 = (ct)^2 - x^2 - y^2 - z^2$ không đổi dưới biến đổi Lorentz.
  - **Bình phương động lượng-4:** $E^2 - p^2c^2 = m^2c^4$ — từ đó rút ra $E = \gamma mc^2$ và $pc = \sqrt{E^2 - (mc^2)^2}$.

## Bảng hệ số Lorentz tại các tốc độ

| $v/c$ | $\gamma$ | Hệ quả nổi bật |
| --- | --- | --- |
| 0,1 | 1,005 | Sai khác cổ điển ~0,5% — hầu hết kỹ thuật bỏ qua |
| 0,5 | 1,155 | Giãn thời gian 15,5% — đo được chính xác |
| 0,9 | 2,294 | Thời gian gần gấp đôi — hạt trong máy gia tốc |
| 0,99 | 7,089 | Đời sống hạt nhân dài gấp ~7 lần |
| 0,999 | 22,37 | Muon từ tầng khí quyển trên đạt tới mặt đất |

## Ví dụ vật lý cụ thể

- **Muon trong khí quyển:** muon sinh ra ở độ cao ~10 km với đời sống riêng $\tau_0 = 2{,}2\,\mu s$. Ở $v = 0{,}998c$ ($\gamma \approx 15{,}8$), đời sống trong phòng thí nghiệm kéo dài $\Delta t = \gamma\tau_0 \approx 35\,\mu s$ — bay được $0{,}998c \times 35\,\mu s \approx 10{,}4$ km, đủ chạm mặt đất. Nếu không có giãn thời gian, muon chỉ bay được ~660 m.
- **Đồng hồ GPS:** vệ tinh chuyển động $v \approx 3{,}87$ km/s làm đồng hồ chạy **chậm** ~7 μs/ngày (tương đối hẹp); lên cao làm đồng hồ chạy **nhanh** ~46 μs/ngày (tương đối rộng, xem [[Thuyết tương đối rộng]]). Phải hiệu chỉnh tổng ~38 μs/ngày, nếu không GPS lệch ~10 km mỗi ngày.
- **Động năng tương đối tính:** $K = (\gamma - 1)mc^2$. Với $v \ll c$, khai triển [[Chuỗi Taylor & xấp xỉ]]: $K \approx \dfrac{1}{2}mv^2 + \dfrac{3}{8}\dfrac{mv^4}{c^2}$ — số hạng đầu chính là công thức Newton.

## Giới hạn cổ điển

- Khi $v \ll c$: $\gamma \to 1$, biến đổi Lorentz trở về biến đổi Galileo, $E \to mc^2 + \frac{1}{2}mv^2$ — mọi công thức trở về cơ học Newton.
- Điều kiện áp dụng: **hệ quy chiếu quán tính** (chuyển động thẳng đều). Hệ phi quán tính nằm ngoài phạm vi — cần [[Thuyết tương đối rộng]].

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: đời sống muon (Rossi–Hall 1941), đồng hồ nguyên tử đi máy bay (Hafele–Keating 1971), mọi hạt nhanh trong máy gia tốc phải dùng cơ học tương đối tính.
- Trường hợp không còn đúng: hệ phi quán tính; hấp dẫn mạnh (chuyển sang tương đối rộng).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Thuyết tương đối hẹp]]: biến đổi Lorentz là nền tảng toán học.
- [[Tiên đề thuyết tương đối hẹp]]: hai tiên đề dẫn đến phép biến đổi này.
- [[Nguyên lý bảo toàn năng lượng]]: hệ thức $E = \gamma mc^2$ là hệ quả trực tiếp.
- [[Chuỗi Taylor & xấp xỉ]]: khi $v \ll c$, $\gamma \approx 1 + \dfrac{v^2}{2c^2}$ — mọi công thức trở về Newton.
- [[Thuyết tương đối rộng]]: mở rộng sang hệ phi quán tính và hấp dẫn.

## Câu hỏi mở

- Vì sao $c$ là tốc độ tối đa, không vật chất nào đạt $v > c$? (Gợi ý: nhân quả — với $v > c$ sẽ có hệ quy chiếu thấy nhân quả đảo ngược.)
- Nghịch lý song sinh: người du hành trẻ hơn — vì sao lập luận "hai anh em đối xứng" lại sai? (Gợi ý: người du hành phải quay đầu → hệ có gia tốc, mất đối xứng.)
- $E = \gamma mc^2$ áp dụng cho photon ($m = 0$) thế nào? (Gợi ý: $E = pc$ — khối lượng nghỉ bằng 0, photon không bao giờ đứng yên.)