---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Nguyên lý chồng chất lượng tử

> [!abstract] Ý chính
> Trạng thái lượng tử là tổ hợp tuyến tính có pha xác định của các trạng thái thành phần; bình phương biên độ của tổng **không bằng** tổng bình phương các biên độ — số hạng chéo giao thoa chính là chỗ lượng tử khác cổ điển nhất.

## Nội dung

- **Khái niệm:** tổng có trọng số của các hàm sóng thành phần: $\Psi_{total} = \sum_n c_n \Psi_n$, với hệ số phức $c_n = |c_n| e^{i\phi_n}$ — nói theo [[Đại số tuyến tính]], đây là khai triển theo một cơ sở của [[Không gian Hilbert]].
- **Vì sao xác suất không cộng tính:** $P = |\Psi_1 + \Psi_2|^2 = P_1 + P_2 + 2\,\text{Re}(c_1^*c_2\Psi_1^*\Psi_2)$ — số hạng chéo phụ thuộc độ lệch pha $\phi_2 - \phi_1$: cùng pha thì tăng, ngược pha thì triệt tiêu.
- **Điều kiện thấy vân:** các thành phần phải **kết hợp pha** với nhau (coherence). Khi mất liên hệ pha, số hạng chéo trung bình bằng 0 → trở về tổng xác suất cổ điển (decoherence).

## Bảng biểu hiện chồng chất

| Hệ | Chồng chất của | Hệ quả quan sát |
| --- | --- | --- |
| Electron qua 2 khe | $|\text{khe 1}\rangle + e^{i\varphi}|\text{khe 2}\rangle$ | Vân giao thoa — mỗi electron tự giao thoa với chính nó |
| Photon phân cực | $|H\rangle + |V\rangle$ (phân cực 45°) | Photon luôn qua thấu kính phân cực đặt 45° |
| Qubit | $\alpha|0\rangle + \beta|1\rangle$, $|\alpha|^2 + |\beta|^2 = 1$ | Nền tảng của tính toán lượng tử |
| Nguyên tử hai mức | $|g\rangle + e^{-i\omega t}|e\rangle$ | Dao động Rabi — cơ sở của đồng hồ nguyên tử |

## Ví dụ vật lý cụ thể

- **Khe đôi electron đơn:** bắn từng electron một — vân giao thoa hiện dần sau nhiều sự kiện, vì trạng thái mỗi electron là chồng chất của hai đường đi. Kiểm chứng trực tiếp A1 + A4 của [[Tiên đề cơ học lượng tử]].
- **Bước sóng electron:** electron gia tốc bởi hiệu điện thế 100 V có $\lambda = \dfrac{h}{\sqrt{2meV}} \approx 0{,}12$ nm — cùng bậc khoảng cách nguyên tử, nên nhiễu xạ qua mạng tinh thể quan sát được (xem [[Thí nghiệm - Davisson-Germer]]).
- **Laser:** hàng tỉ photon cùng một trạng thái chồng chất đồng pha — cường độ cộng kết hợp ($N^2$ thay vì $N$) giúp tia laser định hướng mạnh và đơn sắc.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: khe đôi electron (Tonomura 1989), nhiễu xạ neutron và phân tử lớn, chồng chất trạng thái siêu dẫn.
- Trường hợp không còn đúng: tương tác với môi trường phá vỡ kết hợp pha (decoherence) — giải thích vì sao vật vĩ mô không bao giờ thể hiện chồng chất rõ rệt.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Tiên đề cơ học lượng tử]]: chồng chất là cách khai triển trạng thái trên cơ sở các trạng thái cơ bản.
- [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]: tiên đề I — biên độ chồng chất là “thông tin” của trạng thái.
- [[Trạng thái lượng tử]]: khung khái niệm của chồng chất — tia trạng thái, toán tử mật độ.
- [[Phương trình Schrödinger]]: tính tuyến tính của phương trình là nguồn gốc của chồng chất.
- [[Dao động điều hòa]]: hệ dao động tuyến tính tuân theo nguyên lý chồng chất.
- [[Giao thoa sóng]]: biểu hiện cổ điển của nguyên lý chồng chất.
- [[Không gian Hilbert]] · [[Đại số tuyến tính]]: tổ hợp tuyến tính, cơ sở, khai triển — khung đại số của chồng chất.

## Câu hỏi mở

- Phiên bản vĩ mô "mèo Schrödinger" (chồng chất sống–chết) chưa từng quan sát thấy — decoherence diễn ra nhanh cỡ nào và có chặn được không?
- Vì sao tự nhiên dùng **số phức** làm hệ số $c_n$ chứ không phải số thực? (Lý thuyết "chồng chất thực" cho dự đoán sai khác có thể kiểm tra được.)
- Sức mạnh của tính toán lượng tử đến từ "nhiều trạng thái cùng lúc" hay từ giao thoa có kiểm soát giữa các biên độ?