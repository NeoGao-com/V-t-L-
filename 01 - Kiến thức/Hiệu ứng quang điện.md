---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
category: Vật lý Hiện đại
trạng-thái: ổn-định
created: 2026-09-25
---

# Hiệu ứng quang điện

> [!abstract] Ý chính
> Khi ánh sáng có tần số đủ lớn chiếu vào bề mặt kim loại, electron bị bứt ra. Năng lượng photon $h\nu$ phải thắng được công thoát $\phi$ của vật liệu thì electron mới thoát ra — bằng chứng quyết định rằng ánh sáng là các lượng tử (photon), không phải sóng liên tục.

## Nội dung

- **Phương trình Einstein (1905, Nobel 1921):** $h\nu = A + K_{max}$
  - $h$: hằng số Planck ($6{,}626 \times 10^{-34}$ J·s).
  - $A$: công thoát (work function) đặc trưng của vật liệu.
  - $K_{max}$: động năng cực đại của electron thoát ra.
- **Xác nhận bằng thực nghiệm:** Millikan (1916) đo điện thế hãm, chứng minh phương trình Einstein và cho giá trị $h$ khớp với mọi cách đo khác.
- **Ứng dụng:** pin mặt trời và cảm biến quang — năng lượng photon chuyển thành điện năng (hiệu ứng nghịch đảo).

## Bảng tóm tắt

| Đại lượng | Biểu thức | Ý nghĩa |
| --- | --- | --- |
| Năng lượng photon | $h\nu = hc/\lambda$ | Một lượng tử ánh sáng; photon 400 nm ≈ 3,1 eV, 700 nm ≈ 1,8 eV |
| Công thoát | $A$ | Năng lượng tối thiểu để bứt electron khỏi kim loại |
| Động năng cực đại | $K_{max} = h\nu - A$ | Phụ thuộc tần số, **không** phụ thuộc cường độ |
| Tần số ngưỡng | $\nu_0 = A/h$ | Dưới $\nu_0$: không bứt electron dù cường độ rất lớn |

## Bảng công thoát của một số kim loại

| Kim loại | $A$ (eV) | Tần số ngưỡng $\nu_0$ | Vùng bước sóng ngưỡng $\lambda_0$ |
| --- | --- | --- | --- |
| Cesium (Cs) | 1,95 | $4{,}7 \times 10^{14}$ Hz | 637 nm — ánh sáng **đỏ** đã đủ bứt |
| Kali (K) | 2,30 | $5{,}6 \times 10^{14}$ Hz | 540 nm — lục trở lên |
| Kẽm (Zn) | 4,30 | $1{,}0 \times 10^{15}$ Hz | 288 nm — phải là **tử ngoại** |

Bảng này giải thích vì sao cùng một đèn chiếu vào Cs thì bứt electron, chiếu vào Zn thì không — đặc trưng là tần số, không phải cường độ.

## Ví dụ vật lý cụ thể

- **Photon 400 nm chiếu vào Cs ($A = 1{,}95$ eV):** $h\nu \approx 3{,}1$ eV → $K_{max} = 3{,}1 - 1{,}95 = 1{,}15$ eV → điện thế hãm $V_0 = 1{,}15$ V.
- **Vì sao lý thuyết sóng cổ điển thất bại:** sóng cổ điển dự đoán $K_{max}$ tăng theo cường độ sáng và **không có** ngưỡng tần số — thực nghiệm bác bỏ cả hai. Đây là lý do Einstein dùng khái niệm photon (xem [[Giả thuyết - Hạt ánh sáng (Photon)]]).
- **Hiệu ứng tức thời:** cổ điển dự đoán cần giây/phút tích lũy năng lượng; thực tế electron bứt ra trong $\sim 10^{-9}$ s — bằng chứng năng lượng trao đổi trọn gói $h\nu$.
- **Pin mặt trời silicon:** photon phải có $h\nu > 1{,}1$ eV (độ rộng vùng cấm) mới sinh cặp electron–lỗ trống — cùng cơ chế ngưỡng năng lượng.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: Millikan 1916 (định luật 1: $K_{max}$ theo tần số; định luật 2: ngưỡng $\nu_0$; dòng quang điện tỉ lệ cường độ), hiệu ứng tức thời, ông đã dùng chính thiết bị này về sau để đo điện tích electron ([[Thí nghiệm - Giọt dầu Millikan]]) và vận dụng trong [[Phát xạ electron]].
- Trường hợp không còn đúng: mô tả lượng tử đơn giản (một photon – một electron) đúng cho photon đơn năng lượng thấp; ánh sáng cực mạnh (laser chùm xung) cần lý thuyết trường lượng tử để mô tả hấp thụ đa photon.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Phát xạ electron]] · [[Mẫu nguyên tử Bohr]] · [[Giả thuyết - Lượng tử năng lượng Planck]]
- [[Giả thuyết - Hạt ánh sáng (Photon)]]: nguồn gốc khái niệm photon.
- [[Lưỡng tính sóng-hạt]]: quang điện là mặt "hạt" của photon.
- [[Thí nghiệm - Giọt dầu Millikan]]: cùng tác giả, đo điện tích electron từ thiết bị quang điện.

## Câu hỏi mở

- Nếu cường độ sáng quyết định số electron thoát ra còn tần số quyết định $K_{max}$, thì một chùm laser cực mạnh nhưng tần số thấp (đỏ) có bao giờ bứt được electron không? (Câu trả lời cổ điển "có", lượng tử "không" — và hấp thụ đa photon ở chùm cực mạnh lại trả lời "có"!)
- Vì sao electron nhận trọn $h\nu$ chứ không nhận từng phần nhỏ — "lượng tử hóa" này đến từ đâu trong mô tả trường điện từ?
- Có tồn tại công thoát "âm" (electron tự thoát ra khỏi bề mặt sạch khi hấp thụ nhiệt)? — gắn với phát xạ nhiệt electron và hoạt động của đèn chân không.