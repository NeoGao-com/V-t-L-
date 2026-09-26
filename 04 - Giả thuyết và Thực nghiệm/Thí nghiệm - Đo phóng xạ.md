---
tags:
  - vật-lý/thực-nghiệm
type: thực-nghiệm
domain: hạt-lý
loại: thí-nghiệm
trạng-thái: ổn-định
created: 2026-09-25
---

# Thí nghiệm - Đo phóng xạ

> [!abstract] Mục đích
> Xác định **hệ số suy giảm** (attenuation coefficient) của vật liệu đối với bức xạ ion hóa và đo **bề dày giảm nửa** (half-value layer, HVL) — cơ sở của an toàn bức xạ và thiết kế che chắn phòng xạ trị.

## Thiết kế & kết quả

- **Nguồn:** đồng vị phóng xạ kín (ví dụ $^{60}$Co phát gamma, $^{210}$Po phát alpha).
- **Bố trí:** đặt nguồn và detector (ống Geiger–Muller hoặc nhấp nháy NaI) ở hai bên tấm chắn vật liệu có bề dày $x$ tăng dần; đo cường độ $I$ còn lại.
- **Quy luật suy giảm:** $I = I_0 e^{-\mu x}$ → vẽ $\ln I$ theo $x$ được đường thẳng có độ dốc $-\mu$.
- **Bề dày giảm nửa (HVL):** bề dày làm cường độ giảm còn một nửa: $HVL = \dfrac{\ln 2}{\mu}$.
- **Kết quả ví dụ:**
  - Chì (Pb) với gamma của $^{60}$Co: $\mu \approx 1{,}2$ cm$^{-1}$ → $HVL \approx 0{,}58$ cm.
  - Nhôm (Al) với alpha: HVL chỉ vài mm (alpha dễ bị chặn).

## Ứng dụng thực tế

- **Y tế:** tính bề dày chì cho phòng xạ trị.
- **An toàn:** giám sát liều bức xạ môi trường tại nhà máy hạt nhân.
- **Kiểm định:** quy đổi giới hạn liều cá nhân hàng năm (20 mSv) sang bề dày bêtông/chì cần thiết.

## Liên kết

- [[MOC - Giả thuyết và Thực nghiệm]]
- [[Cấu tạo hạt nhân]] · [[Phóng xạ]] · [[Ứng dụng & an toàn]]
- [[Xử lý sai số thực nghiệm]]: sai số đếm thống kê, khớp tuyến tính $\ln I$ theo $x$.