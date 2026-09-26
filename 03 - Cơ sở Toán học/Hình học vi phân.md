---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Hình học vi phân

> [!abstract] Công cụ để làm gì
> Hình học vi phân nghiên cứu **không gian cong** bằng công cụ giải tích: trên mỗi điểm có một "không gian tiếp xúc" phẳng mà ta do đạc địa phương, rồi ghép các mảnh phẳng lại thành bức tranh toàn cục. Đây là ngôn ngữ duy nhất đủ mạnh để viết [[Thuyết tương đối rộng]] — nơi hấp dẫn chính là độ cong của không-thời gian.

## Định nghĩa

- **Đa tạp (manifold):** không gian cục bộ "trông như" $\mathbb{R}^n$ — mỗi vùng nhỏ có tấm bản đồ riêng (giống bản đồ Trái Đất phẳng từng tờ).
- **Metric $g_{\mu\nu}$:** "thước đo" độ dài trên từng điểm: $ds^2 = g_{\mu\nu} dx^\mu dx^\nu$ — mang toàn bộ thông tin hình học ([[Giải tích Tensor]]).
- **Liên thông (connection) và đạo hàm hiệp biến:** cách "soi đường thẳng" trên mặt cong — đạo hàm thường không còn là tensor; phải bù thêm số hạng liên thông $\Gamma^\mu_{\alpha\beta}$.
- **Độ cong (curvature):** tensor Riemann $R^\mu_{\ \nu\rho\sigma}$ đo độ cong nội tại; co chỉ số ra **tensor Ricci** $R_{\mu\nu}$ và **vô hướng Ricci** $R$.
- **Trắc địa (geodesic):** đường "thẳng nhất có thể" trên mặt cong — cực tiểu độ dài, là quỹ đạo tự do của hạt (liên hệ [[Phép tính biến phân]]).

Bản đồ khái niệm ↔ vai trò trong thuyết tương đối rộng:

| Khái niệm | Vai trò trong GR |
| --- | --- |
| Metric $g_{\mu\nu}$ | "Trường hấp dẫn" — nguồn quyết định độ cong và nhịp đồng hồ |
| Liên thông $\Gamma$ | "Thế" hấp dẫn — chi phối quỹ đạo rơi tự do (gia tốc hiệu dụng) |
| Độ cong (Ricci $R_{\mu\nu}$) | "Thủy triều" — gia tốc tương đối giữa các trắc địa lân cận |
| Trắc địa | Quỹ đạo của hạt tự do và tia sáng |
| Đa tạp 4 chiều | Không-thời gian — "sân khấu" chung của vật chất |

## Ý nghĩa hình học

- Trái Đất là đa tạp 2 chiều: trên quả địa cầu, hai kinh tuyến "song song" ở xích đạo lại **gặp nhau** ở cực — song song chỉ đúng cục bộ; độ cong "uốn" các khái niệm song song/thẳng thành khái niệm địa phương.
- **Đo độ cong nội tại từ bên trong:** tổng góc tam giác trên mặt cầu $> 180^\circ$ (độ cong dương, độ dư tỉ lệ diện tích tam giác); trên mặt "yên ngựa" $< 180^\circ$ (độ cong âm); chu vi vòng tròn bán kính $r$ thì nhỏ hơn $2\pi r$. Không cần nhìn từ ngoài — đây là độ cong nội tại, thứ duy nhất có nghĩa vật lý.
- **Trắc địa trong đời thường:** đường bay xuyên Đại Tây Dương trông "cong" trên bản đồ phẳng nhưng là đường ngắn nhất thật sự trên mặt cầu — trắc địa là "đường thẳng của không gian cong".

## Ý nghĩa vật lý

- **Hấp dẫn = hình học:** [[Nguyên lý tương đương]] nói lực hấp dẫn cục bộ biến mất trong hệ rơi tự do — gợi ý hấp dẫn không phải "lực" mà là **hình dạng không-thời gian**; vật rơi chỉ đi theo trắc địa ([[Thuyết tương đối rộng]]).
- **Phương trình Einstein:** $G_{\mu\nu} + \Lambda g_{\mu\nu} = \dfrac{8\pi G}{c^4} T_{\mu\nu}$ — nối **hình học** (vế trái, từ tensor Ricci) với **vật chất–năng lượng** (vế phải). Hệ số $8\pi G/c^4$ không phải tùy tiện: nó khớp thứ nguyên (Ricci nghịch đảo diện tích, $T$ mật độ năng lượng) để phương trình suy về đúng định luật Newton trong trường yếu ([[Giải tích Tensor]]).
- **Ánh sáng cong theo không-thời gian:** tia sáng là trắc địa null — độ lệch dự đoán $1{,}75''$ qua rìa Mặt Trời, xác nhận bởi [[Thí nghiệm - Nhật thực Eddington 1919]].
- **Trắc địa = nguyên lý cực trị:** hạt tự do đi theo trắc địa, "đường ngắn nhất" trong không-thời gian cong — mở rộng của nguyên lý tác dụng tối thiểu ([[Phép tính biến phân]], [[Nguyên lý tác dụng tối thiểu]]).
- **Giới hạn phẳng:** khi $g_{\mu\nu}$ là metric Minkowski $ds^2 = -c^2dt^2 + dx^2 + dy^2 + dz^2$, toàn bộ máy móc trở về thuyết tương đối hẹp — khung chung cho cả hai lý thuyết ([[Thuyết tương đối hẹp]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Thuyết tương đối rộng]]: phương trình Einstein, trắc địa, độ cong và hấp dẫn.
- [[Nguyên lý tương đương]]: điểm khởi đầu triết lý của hấp dẫn-hình học.
- [[Giải tích Tensor]]: ngôn ngữ bắt buộc (chỉ số, metric, liên thông).
- [[Thí nghiệm - Nhật thực Eddington 1919]]: độ lệch ánh sáng — kiểm chứng thực nghiệm.
- [[Phép tính biến phân]] · [[Nguyên lý tác dụng tối thiểu]]: trắc địa từ cực trị tác dụng.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Giải tích Tensor]] · [[Hệ tọa độ]] · [[Phép tính biến phân]] · [[Chuỗi Taylor & xấp xỉ]] (phẳng cục bộ, khai triển quanh điểm) · [[Thuyết tương đối rộng]] · [[Thuyết tương đối hẹp]]

## Câu hỏi mở

- "Độ cong nội tại" (người ở trên mặt cong tự đo được — ví dụ tổng góc tam giác) khác gì "độ cong ngoại tại" (cần nhìn từ không gian ngoài)? Vì sao theo GR chỉ độ cong nội tại có nghĩa vật lý? (Gợi ý: không-thời gian không "nằm trong" không gian nào lớn hơn.)
- Phương trình Einstein ngụ ý trường hấp dẫn chính là metric — vậy "sóng hấp dẫn" là sóng của cái gì, và vì sao nó truyền năng lượng? (Gợi ý: gợn sóng của $g_{\mu\nu}$ trong chân không — độ cong "tự truyền" như sóng của chính không-thời gian.)
- Vì sao số chiều của đa tạp không-thời gian lại chặn số dạng "lý thuyết hấp dẫn" hợp lệ — và metric dương/âm (signature) ảnh hưởng gì đến hình dạng nón ánh sáng? (Gợi ý: nhân quả — trắc địa null phân tách "trong nón" và "ngoài nón".)