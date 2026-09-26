---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: nhiệt-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Thuyết động học phân tử

> [!abstract] Ý chính
> Nhiệt là **chuyển động hỗn loạn của phân tử**. Thuyết này suy ra tính chất nhiệt từ cơ học của từng phân tử: áp suất do va chạm, nhiệt độ tỉ lệ động năng trung bình — cầu nối giữa cơ học cổ điển và nhiệt học.

## Các kết quả cơ bản (khí lý tưởng)

- Áp suất theo vận tốc căn quân phương $\bar v$: $p = \dfrac{1}{3}\rho\bar v^2$ (mật độ khối lượng $\rho$).
- Động năng trung bình một phân tử: $\overline{W_đ} = \dfrac{3}{2}kT$ với $k = 1{,}38\times10^{-23}$ J/K (hằng số Boltzmann) → **nhiệt độ tuyệt đối là thước đo động năng trung bình của phân tử**.
- Khí đơn nguyên tử: nội năng $U = \dfrac{3}{2}nRT$ (xem [[Nội năng]]).
- Tốc độ phân tử không đều nhau — tuân theo phân bố Maxwell; $\bar v$ ở đây là vận tốc căn quân phương $\sqrt{\langle v^2\rangle}$.

## Bảng tốc độ căn quân phương ở 300 K

| Khí | Khối lượng mol | $v_{rms} = \sqrt{\dfrac{3RT}{M}}$ | Hệ quả |
| --- | --- | --- | --- |
| Heli (He) | 4 g/mol | ≈ 1.370 m/s | Nhẹ + nhanh → thoát khí quyển dần |
| Nitơ (N₂) | 28 g/mol | ≈ 520 m/s | Tốc độ âm thanh trong không khí (~340 m/s) cùng bậc |
| Oxy (O₂) | 32 g/mol | ≈ 480 m/s | — |
| CO₂ | 44 g/mol | ≈ 410 m/s | Nặng hơn, chậm hơn |

Động năng trung bình ở 300 K: $\frac{3}{2}kT \approx 6{,}2\times10^{-21}$ J ≈ 0,039 eV — cùng bậc năng lượng kích thích phân tử.

## Ví dụ vật lý cụ thể

- **Áp suất khí:** 1 mol ở 273 K chiếm 22,4 L chứa $N_A \approx 6×10^{23}$ phân tử, mỗi phân tử va chạm thành bình cỡ $10^9$–$10^{10}$ lần/giây — áp suất ~1 atm là kết quả trung bình của hàng tỉ tỉ va chạm.
- **Bay hơi:** phân tử thoát khỏi bề mặt khi chuyển động đủ nhanh để thắng lực liên kết — nhiệt độ càng cao, "đuôi" phân bố Maxwell càng nhiều phân tử nhanh → bay hơi nhanh hơn.
- **Vì sao He thoát khí quyển:** $v_{rms}$ của He ở tầng cao có thể chạm mốc vận tốc thoát (~11 km/s vẫn còn xa, nhưng đuôi phân bố kéo dài và va chạm hiếm giúp một phần thoát) — giải thích He trong khí quyển Trái Đất rất hiếm.

## Suy luận từ đâu

- Dùng cơ học của [[Các định luật Newton]] cho từng phân tử (va chạm đàn hồi — [[Va chạm]]), rồi lấy trung bình: công cụ là [[Xác suất thống kê]].
- Bằng chứng thực nghiệm trực tiếp: [[Quan sát - Chuyển động Brown]].

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: đo $v_{rms}$ bằng chùm phân tử (kinetic molecular beams), [[Chuyển động Brown]], tốc độ âm thanh, nhiệt dung khí đơn nguyên tử.
- Trường hợp không còn đúng: phân tử có cấu trúc nội tại (quay, dao động) — nhiệt dung cao hơn $\frac{3}{2}R$; khí thực cần [[Phương trình van der Waals]]; ở nhiệt độ rất thấp, lượng tử hóa mức quay làm nhiệt dung H₂ giảm xuống (bài toán kinh điển của vật lý lượng tử).

## Vì sao quan trọng

- Giải thích: áp suất, nhiệt độ, [[Sự chuyển thể]] (phá vỡ liên kết), bay hơi, khuếch tán.
- Mở đường đến **vật lý thống kê**: cơ sở vi mô cho [[Nguyên lý thứ hai nhiệt động lực học]] qua [[Entropy]].

## Liên kết

- [[Chất khí và khí lý tưởng]] · [[Nhiệt độ và thang nhiệt độ]] · [[Quan sát - Chuyển động Brown]] · [[Xác suất thống kê]] · [[Nội năng]] · [[Va chạm]] · [[MOC - Kiến thức Vật lý]]
- [[Phương trình van der Waals]]: hiệu chỉnh cho khí thực (kích thước + lực hút phân tử).
- [[Entropy]]: mối liên hệ $S = k\ln W$ suy ra từ trạng thái vi mô.

## Câu hỏi mở

- Tại sao trung bình lại ổn định đến mức $p, T$ là đại lượng vĩ mô chắc chắn? → do số phân tử cực lớn ($N \sim 10^{23}$), dao động thống kê bé — ý tưởng trung tâm của [[Xác suất thống kê]].
- Vì sao định luật phân bố đều năng lượng (equipartition) dự đoán nhiệt dung của H₂ cao hơn thực tế ở nhiệt độ thấp? (Gợi ý: mức quay bị lượng tử hóa — chỉ "bật" khi $kT$ đủ lớn so với khoảng cách mức.)