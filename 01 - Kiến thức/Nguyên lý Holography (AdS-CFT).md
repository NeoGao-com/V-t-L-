---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Nguyên lý Holography (AdS-CFT)

> [!abstract] Ý chính
> Đối ngẫu giữa một lý thuyết hấp dẫn trong không-thời gian Anti-de Sitter chiều $d+1$ (AdS$_{d+1}$) và một lý thuyết trường conformal ở biên (CFT$_d$): "khối bên trong" cong 4D tương đương với một QFT không hấp dẫn ở biên — thông tin của hệ hấp dẫn mã hóa trên mặt biên, một phiên bản mạnh của nguyên lý holographic ('t Hooft–Susskind, 1993–95; Maldacena 1997).

## Nội dung

- **Tương ứng AdS$_{d+1}$/CFT$_d$:** mỗi tương tác hấp dẫn trong bulk (khối) có tương ứng một–một với một toán tử của QFT ở biên. Từ điển đối ngẫu: metric bulk ↔ tensor ứng suất biên; trường vô hướng khối lượng $m$ ↔ toán tử chiều $\Delta$ với $\Delta(\Delta - d) = m^2 L^2$.
- **Nguyên lý holographic:** entropy tối đa của vùng không gian tỉ lệ **diện tích** biên, không phải thể tích — cực đoan hơn nữa: hấp dẫn + QFT trong bulk = QFT không hấp dẫn ở biên (không cần "bên trong" riêng).
- **Entropy lỗ đen (Bekenstein–Hawking):**
  $S = \dfrac{k_B c^3 A}{4 G \hbar}$
  entropy tỉ lệ diện tích chân trời; công thức Ryu–Takayanagi mở rộng sang entropy vướng víu: $S_{EE} = \dfrac{diện\,tích\,mặt\,cực\,tiểu}{4G}$.

## Bảng: đối ngẫu AdS ↔ CFT

| Trong bulk (hấp dẫn, $d+1$ chiều) | Ở biên (CFT, $d$ chiều) |
| --- | --- |
| Hấp dẫn, lỗ đen | Trạng thái nhiệt của QFT |
| Metric | Tensor ứng suất-năng lượng $\langle T_{\mu\nu}\rangle$ |
| Trường vô hướng | Toán tử (nguyên tố) tương ứng |
| Hình học chuẩn (geodesic, mặt cực tiểu) | Entropy vướng víu, hàm tương quan |
| Nhiệt động lỗ đen | Nhiệt động QFT |

## Ví dụ vật lý cụ thể

- **Giới hạn KSS (vật lý vật chất ngưng tụ):** nhớt/entropy của plasma quark–gluon tại RHIC/LHC thỏa $\eta/s \ge \hbar/(4\pi k_B) \approx 6{,}08\times10^{-13}$ Pa·s — gần chạm tới hạn (so nước ~10⁻³ Pa·s) — AdS/CFT dự đoán đúng "chất lỏng hoàn hảo nhất" mà thực nghiệm đo được.
- **Kim loại lạ (strange metal):** điện trở suất tỉ lệ tuyến tính theo nhiệt độ (không phải $T^2$ của Fermi liquid) — mô tả được bằng đối ngẫu holographic thay vì lý thuyết nhiễu loạn.
- **Nghịch lý thông tin lỗ đen:** entropy vướng víu của bức xạ Hawking tuân theo đường Page nếu dùng công thức holographic; hiệu chỉnh entropy dư (island formula) mở đường giải nghịch lý — kết quả giải thưởng Physics Breakthrough 2021.

## Suy luận từ đâu

- Từ cơ học nhiệt động lỗ đen (Bekenstein 1972, Hawking 1974): nếu lỗ đen có entropy $\sim A/4$, thì hệ hấp dẫn mạnh mô tả được bằng bậc tự do trên biên ít hơn nhiều → 't Hooft, Susskind đặt thành nguyên lý (1993–95).
- Maldacena (1997) chứng minh cụ thể cho $\mathcal{N}=4$ SYM ở biên ↔ chuỗi IIB trên AdS$_5\times S^5$ — khởi đầu lĩnh vực "gauge/gravity duality".

## Kiểm chứng & giới hạn

- Kiểm chứng: đối ngẫu khớp trong các trường hợp có thể tính hai phía (hàm tương quan, nhiệt động lỗ đen Schwarzschild–AdS); dự đoán $\eta/s$ khớp dữ liệu QGP; lý thuyết chuỗi khớp các giới hạn bán cổ điển.
- **Giới hạn:** AdS có $\Lambda < 0$ — vũ trụ của ta có $\Lambda > 0$ (de Sitter, xem [[Nguyên lý Vũ trụ học]]); chưa có chứng minh đầy đủ cho mọi CFT; áp dụng vào vật chất ngưng tụ còn định tính.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Lý thuyết trường lượng tử (QFT)]]: gốc rễ của đối ngẫu.
- [[Mô hình chuẩn (Standard Model)]]: QFT gauge — đối ngẫu gauge/hấp dẫn áp dụng được.
- [[Nguyên lý bất định Heisenberg]]: giới hạn thông tin–năng lượng ở biên (bất đẳng thức holo).
- [[Entropy]]: Bekenstein–Hawking mở rộng khái niệm entropy sang lỗ đen.

## Câu hỏi mở

- Vũ trụ của ta (de Sitter, $\Lambda > 0$) có đối ngẫu holographic không — hay "holography chỉ đúng với AdS"? (Vấn đề dS/CFT chưa giải.)
- Lỗ đen có "cắt–dán" (island) thông tin như công thức entropy chỉ ra — nhưng cơ chế vi mô thực sự (lượng tử hóa hấp dẫn) là gì khi lý thuyết chuỗi chưa hoàn chỉnh?
- Nghịch lý thông tin có buộc chúng ta từ bỏ unitarity hoặc locality — và ý nghĩa với nền tảng cơ học lượng tử ([[Tiên đề cơ học lượng tử]]) như thế nào?