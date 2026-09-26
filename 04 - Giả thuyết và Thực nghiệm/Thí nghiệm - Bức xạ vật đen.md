---
tags:
  - vật-lý/thực-nghiệm
type: thực-nghiệm
domain: lượng-tử
loại: thí-nghiệm
trạng-thái: ổn-định
created: 2026-09-25
---

# Thí nghiệm - Bức xạ vật đen

> [!abstract] Mục đích
> Bức xạ nhiệt phát ra từ một "vật đen" (vật hấp thụ hoàn toàn) tuân theo phân bố phổ nào — và phát hiện (1900) rằng nó **không thể giải thích bằng vật lý cổ điển**, buộc Planck đưa ra giả thuyết năng lượng lượng tử: nền móng của cơ học lượng tử.

## Thiết kế

- **Bối cảnh:** vật đen lý tưởng hấp thụ mọi bức xạ, khi nung nóng phát bức xạ nhiệt chỉ phụ thuộc **nhiệt độ** (không phụ thuộc vật liệu) — "hốc bức xạ" (hộp kín đục lỗ nhỏ) là hiện thực hóa chuẩn.
- **Dụng cụ:** hốc nung ở nhiệt độ $T$ chuẩn hóa; lăng kính/cách tử phân ly phổ; detector đo phân bố cường độ theo bước sóng $I(\lambda, T)$.
- **Cách đo:** so phổ đo được với các công thức lý thuyết — Rayleigh–Jeans (cổ điển) và Wien (kinh nghiệm vạch ngắn) đều chỉ khớp một phần.

## Kết quả & kết luận

| Định luật | Công thức | Khớp thực nghiệm |
| --- | --- | --- |
| Rayleigh–Jeans (1900) | $I \propto T/\lambda^4$ | Chỉ sóng dài; **sai hoàn toàn sóng ngắn** ($I \to \infty$ — "thảm họa tử ngoại") |
| Wien (1896) | $I \propto \lambda^{-5}e^{-hc/(\lambda k_B T)}$ | Chỉ sóng ngắn; sóng dài thiếu hụt |
| **Planck (14-12-1900)** | $I = \dfrac{2hc^2}{\lambda^5}\dfrac{1}{e^{hc/(\lambda k_B T)} - 1}$ | **Khớp toàn phổ** với $h$ duy nhất |

- Công thức Planck ra đời bằng giả thuyết năng lượng lượng tử $E = nh\nu$ — dữ kiện thực nghiệm buộc phải có $h$.
- **Định luật dịch chuyển Wien:** $\lambda_{max} T = b = 2{,}898\times10^{-3}$ m·K.

## Ví dụ số kiểm chứng được

- **Mặt Trời** ($T \approx 5778$ K): $\lambda_{max} = b/T \approx 501$ nm — đúng giữa ánh sáng nhìn thấy (vì sao mắt ta tiến hóa tinh chỉnh vào "cửa sổ Mặt Trời").
- **Cơ thể người** (310 K): $\lambda_{max} \approx 9{,}4\ \mu$m — hồng ngoại nhiệt (camera nhiệt đo được chính phổ này).
- **CMB** (2,725 K): $\lambda_{max} \approx 1{,}06$ mm — vi sóng: chính là phổ vật đen hoàn hảo nhất đo được ([[Quan sát - Bức xạ phông vi sóng vũ trụ (CMB)]], [[Nguyên lý Vũ trụ học]]).

## Ảnh hưởng lên lý thuyết

- Mở đầu cơ học lượng tử: [[Giả thuyết - Lượng tử năng lượng Planck]] → photon → Bohr → Schrödinger ([[Tiên đề cơ học lượng tử]]).
- Đặt nền cho thiên văn phổ học (nhiệt độ sao từ $\lambda_{max}$), đo nhiệt độ từ xa (nhiệt kế bức xạ, camera hồng ngoại).
- Chứng minh một mẫu: thí nghiệm đẩy lý thuyết tới giới hạn cổ điển và buộc "giả thuyết vô lý" trở thành nền tảng — biểu tượng của vòng lặp [[MOC - Giả thuyết và Thực nghiệm]].

## Liên kết

- [[MOC - Giả thuyết và Thực nghiệm]]
- [[MOC - Kiến thức Vật lý]]
- [[Giả thuyết - Lượng tử năng lượng Planck]] · [[Mẫu nguyên tử Bohr]] · [[Quan sát - Bức xạ phông vi sóng vũ trụ (CMB)]] · [[Nguyên lý Vũ trụ học]] · [[Nhiệt độ và thang nhiệt độ]]

## Câu hỏi mở

- Phân bố Rayleigh–Jeans (phân phối liên tục) sai ở đâu? (Gợi ý: ở tần số cao số mode $2\nu^2/c^2$ tăng không giới hạn và mỗi mode nhận $k_BT$ — không có cơ chế nào chặn; Planck chặn bằng $e^{h\nu/k_BT}$ thay cho 1 trong mẫu số — "mỗi mode chỉ nhận năng lượng khi $h\nu \sim k_BT$".)
- Vì sao phổ vật đen CMB chuẩn tới 1 phần 10⁵ — điều đó chứng minh điều gì về bản chất vũ trụ sơ khai ([[Quan sát - Bức xạ phông vi sóng vũ trụ (CMB)]])?