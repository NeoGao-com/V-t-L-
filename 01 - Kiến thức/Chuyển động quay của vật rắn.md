---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: cơ-học
category: Vật lý Cổ điển
trạng-thái: ổn-định
created: 2026-09-25
---

# Chuyển động quay của vật rắn

> [!abstract] Ý chính
> "Định luật II Newton cho chuyển động quay": moment lực $M$ gây gia tốc góc $\gamma$, tỉ lệ với **moment quán tính** $I$: $M = I\gamma$, với $I = \sum m_i r_i^2$ đóng vai trò "khối lượng quay" — phụ thuộc cách phân bố khối lượng quanh trục.

## Bảng đối chiếu tịnh tiến ↔ quay

| Đại lượng tịnh tiến | Đại lượng quay | Quan hệ |
| --- | --- | --- |
| Khối lượng $m$ | Moment quán tính $I = \sum m_ir_i^2$ | $I$: "khối lượng quay" |
| Lực $\vec F$ | Moment lực $\vec M = \vec r \times \vec F$ | $\vec M = I\vec\gamma$ |
| Động lượng $\vec p = m\vec v$ | Moment động lượng $\vec L = I\vec\omega$ | $\vec L$ bảo toàn khi $M = 0$ |
| Động năng $\frac{1}{2}mv^2$ | Động năng quay $\frac{1}{2}I\omega^2$ | — |
| Định luật II $F = ma$ | $M = I\gamma$ | áp dụng cho trục cố định |

## Bảng moment quán tính của vật thường gặp

| Vật (quanh trục đi qua tâm) | $I$ |
| --- | --- |
| Vành mảnh | $mR^2$ |
| Đĩa đặc | $\frac{1}{2}mR^2$ |
| Thanh dài $L$ | $\frac{1}{12}mL^2$ |
| Cầu đặc | $\frac{2}{5}mR^2$ |

Quy tắc chung: khối lượng càng rải xa trục, $I$ càng lớn — cùng khối lượng, vành "khó quay" hơn đĩa. Với trục song song cách tâm đoạn $d$: $I = I_{cm} + md^2$ (định lý trục song song).

## Ví dụ vật lý cụ thể

- **Trượt băng nghệ thuật:** khi ép tay vào người, $I$ giảm ~3 lần → $\omega$ tăng ~3 lần ($L = I\omega$ bảo toàn khi moment ngoại lực ≈ 0). Duỗi tay ra lại chậm.
- **Bánh đà lưu trữ năng lượng:** đĩa thép $m = 200$ kg, $R = 0{,}5$ m → $I = \frac{1}{2}mR^2 = 25$ kg·m². Quay 3.000 vòng/phút ($\omega = 314$ rad/s): $W = \frac{1}{2}I\omega^2 \approx 1{,}2$ MJ và $L = I\omega \approx 7.850$ kg·m²/s — dùng làm nguồn năng lượng đệm trong xe buýt lai, hoặc ổn định tần số lưới điện.
- **Con quay hồi chuyển:** moment lực đặt vuông góc với trục quay không tăng $\omega$ mà **quay trục** (tuế sai) — nguyên lý của la bàn con quay trên máy bay.

## Hệ quả trực quan

- Vận động viên trượt băng xoay tít khi ép tay vào người (giảm $I$ → tăng $\omega$, $L$ bảo toàn).
- Vật có khối lượng rải xa trục ($I$ lớn) khó quay hơn — bánh đà, vô lăng.

## Kiểm chứng & giới hạn

- Thực nghiệm: bảo toàn $L$ (trượt băng, vòng quay ghế xoay tạ), con quay, định luật II quay đo bằng máy Atwood có ròng rọc có $I$ đáng kể ([[Thí nghiệm - Máy Atwood]]).
- Trường hợp không còn đúng: trục không cố định và vật rắn quay tự do trong không gian cần dùng tensor quán tính; ở thang lượng tử, $L$ lượng tử hóa thành $l(l+1)\hbar^2$ (xem [[Tiên đề cơ học lượng tử]]).

## Liên kết

- [[Cân bằng của vật rắn]] · [[Vector]] · [[Các định luật Newton]] · [[Động năng]] · [[MOC - Kiến thức Vật lý]]
- [[Định luật II Newton]]: $M = I\gamma$ là "bản quay" của $F = ma$.
- [[Định lý Noether]]: bảo toàn $L$ xuất phát từ đối xứng quay của không gian.
- [[Chuyển động tròn đều]]: trường hợp riêng $\omega$ không đổi.

## Câu hỏi mở

- Vì sao moment lực đặt vuông góc trục quay làm **đổi hướng trục** thay vì tăng tốc độ quay? (Gợi ý: $\vec M = d\vec L/dt$ — $\vec L$ đổi hướng, độ lớn không đổi: tuế sai.)
- Tại sao $L$ bảo toàn mà không "sinh" hay "mất" — đối xứng nào của không gian đảm bảo điều đó? ([[Định lý Noether]]: tính đẳng hướng của không gian.)