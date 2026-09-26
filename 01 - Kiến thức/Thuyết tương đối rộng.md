---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: tương-đối
trạng-thái: ổn-định
created: 2026-09-25
---

# Thuyết tương đối rộng

> [!abstract] Ý chính
> Einstein 1915: khối lượng và năng lượng làm **cong không-thời gian** — hấp dẫn không phải là lực mà là *hình học*: vật thể rơi theo đường "thẳng nhất có thể" (trắc địa) trong không-thời gian cong.

## Nội dung

- **Biến trường:** $g_{\mu\nu}(x)$ — tensor metric xác định khoảng cách $ds^2 = g_{\mu\nu}dx^\mu dx^\nu$ tại mỗi điểm không-thời gian. Không-thời gian phẳng (tương đối hẹp) có $g_{\mu\nu} = \eta_{\mu\nu} = \text{diag}(1,-1,-1,-1)$; có vật chất thì $g_{\mu\nu}$ cong.
- **Phương trình trường Einstein:**
  $G_{\mu\nu} + \Lambda g_{\mu\nu} = \dfrac{8\pi G}{c^4} T_{\mu\nu}$
  - $G_{\mu\nu}$: tensor Einstein — đo độ cong của không-thời gian (từ [[Giải tích Tensor]]).
  - $T_{\mu\nu}$: tensor năng lượng–xung lượng — "nguồn": mật độ năng lượng, áp suất, lưu lượng năng lượng.
  - $\Lambda$: hằng số vũ trụ — ứng với năng lượng tối, chi phối sự giãn nở tăng tốc của vũ trụ (xem [[Nguyên lý Vũ trụ học]]).
- **Trắc địa:** vật tự do chuyển động theo trắc địa của không-thời gian cong; độ lệch giữa các trắc địa lân cận chính là lực thủy triều (tensor Ricci — xem [[Hình học vi phân]]).

## Bảng dự đoán và bằng chứng

| Dự đoán | Giá trị | Bằng chứng |
| --- | --- | --- |
| Dịch chuyển perihelion Sao Thủy | ~43″/thế kỷ | Đo chính xác từ thế kỷ 19, khớp nghiệm Schwarzschild |
| Ánh sáng lệch gần Mặt Trời | 1,75″ | [[Thí nghiệm - Nhật thực Eddington 1919]] |
| Giãn thời gian hấp dẫn | đồng hồ thấp chạy chậm hơn | GPS phải hiệu chỉnh ~46 μs/ngày |
| Sóng hấp dẫn | từ va chạm lỗ đen | LIGO 2015 (Nobel Vật lý 2017) |

## Ví dụ vật lý cụ thể

- **Lỗ đen:** vật có bán kính nhỏ hơn bán kính Schwarzschild $r_s = \dfrac{2GM}{c^2}$ sụp thành lỗ đen: Mặt Trời có $r_s \approx 3$ km, Trái Đất có $r_s \approx 9$ mm. Không gì — kể cả ánh sáng — thoát khỏi $r_s$.
- **Giãn thời gian hấp dẫn:** đồng hồ càng gần khối lượng lớn chạy càng chậm. Vệ tinh GPS ở độ cao ~20.200 km chạy nhanh hơn mặt đất ~46 μs/ngày; cộng với hiệu ứng tương đối hẹp (chậm ~7 μs/ngày, xem [[Biến đổi Einstein]]), hệ thống phải hiệu chỉnh ~38 μs/ngày — nếu không, GPS lệch ~10 km mỗi ngày.
- **Sóng hấp dẫn:** gia tốc của khối lượng lớn làm không-thời gian gợn sóng lan truyền với tốc độ $c$; LIGO 2015 đo trực tiếp sóng từ vụ hợp nhất hai lỗ đen ~30 khối lượng Mặt Trời — mở ra "thiên văn học sóng hấp dẫn".

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: perihelion Sao Thủy, lệch ánh sáng (Eddington 1919), giãn thời gian hấp dẫn (GPS, Pound–Rebka), sóng hấp dẫn (LIGO/Virgo), ảnh lỗ đen (Event Horizon Telescope — M87, 2019).
- Trường hợp không còn đúng: tại kỳ dị trung tâm lỗ đen và thời điểm Vụ Nổ Lớn, độ cong trở nên vô hạn — lý thuyết sụp đổ, cần lý thuyết **hấp dẫn lượng tử** chưa hoàn thiện.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Thuyết tương đối hẹp]]: nền tảng không-thời gian phẳng.
- [[Nguyên lý tương đương]]: nền móng để mở rộng sang không gian cong.
- [[Nguyên lý Vũ trụ học]]: năng lượng tối $\Lambda$ và tỷ lệ thành phần vũ trụ.
- [[Thí nghiệm - Michelson-Morley]]: nền tảng cho không-thời gian không cố định.
- [[Thí nghiệm - Nhật thực Eddington 1919]]: bằng chứng đầu tiên về độ cong ánh sáng.
- [[Hình học vi phân]] · [[Giải tích Tensor]]: metric, tensor Ricci — ngôn ngữ toán của phương trình Einstein.

## Câu hỏi mở

- Tại sao $\Lambda$ quan sát được nhỏ đến mức ~$10^{-120}$ lần giá trị dự đoán từ vật lý lượng tử? ("Bài toán hằng số vũ trụ" — một trong những vấn đề lớn nhất của vật lý hiện đại.)
- Điều gì xảy ra tại kỳ dị trung tâm lỗ đen? — mọi định luật vật lý đổ vỡ; cần hấp dẫn lượng tử.
- Làm thế nào lượng tử hóa được chính trường $g_{\mu\nu}$ để hợp nhất với cơ học lượng tử? (Lý thuyết dây, hấp dẫn lượng tử vòng... — vẫn mở.)