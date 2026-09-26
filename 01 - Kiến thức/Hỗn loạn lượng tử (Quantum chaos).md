---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Hỗn loạn lượng tử (Quantum chaos)

> [!abstract] Ý chính
> Nghiên cứu hệ lượng tử có giới hạn cổ điển **hỗn loạn** (nhạy cảm với điều kiện ban đầu). Vì nguyên lý bất định làm mờ quỹ đạo, hỗn loạn lượng tử không nhìn qua quỹ đạo mà qua **thống kê phổ năng lượng**: mức năng lượng hệ hỗn loạn "đẩy nhau" (Wigner–Dyson), hệ khả tích phân bố ngẫu nhiên (Poisson).

## Nội dung

- **Khái niệm cốt lõi:** hệ lượng tử "hỗn loạn" nếu Hamiltonian cổ điển tương ứng có số mũ Lyapunov $\lambda_L > 0$ — nhưng câu hỏi trở thành: dấu vết của sự hỗn loạn đó nằm ở đâu trong phổ lượng tử?
- **Hai phỏng đoán nền tảng (giữa thế kỷ 20→80):**
  - **Berry–Tabor (1977):** hệ **khả tích** → thống kê mức kiểu **Poisson** (mức độc lập, có thể trùng nhau).
  - **Bohigas–Giannoni–Schmit (1984):** hệ **hỗn loạn** → thống kê mức kiểu **Wigner–Dyson** (mức đẩy nhau, tuyệt đối không trùng).
- **Ba lớp đối xứng Wigner–Dyson:** GOE (bất biến đảo thời gian), GUE (có từ trường phá đảo thời gian), GSE (spin bán nguyên) — ma trận ngẫu nhiên RMT là công cụ chuẩn.
- **Phương pháp bán cổ điển:** quan hệ vết Gutzwiller nối phổ năng lượng với tổng các quỹ đạo tuần hoàn cổ điển.

## Bảng: phân biệt hai chế độ phổ

| Đặc điểm | Hệ khả tích (Poisson) | Hệ hỗn loạn (Wigner–Dyson, GOE) |
| --- | --- | --- |
| Số mức lân cận | độc lập, dễ "dính" nhau | đẩy nhau mạnh |
| Tỉ số khoảng cách mức liên tiếp $\langle r \rangle$ | $2\ln2 - 1 \approx 0{,}386$ | $4 - 2\sqrt3 \approx 0{,}536$ |
| Ví dụ | dao động điều hòa, bóng bàn hình chữ nhật | stadium billiard (Bunimovich), nguyên tử trong từ trường mạnh |

## Ví dụ vật lý cụ thể

- **Kicked rotor:** nguyên tử (hoặc sóng vi ba trong khoang) bị "đá" bởi xung tuần hoàn — tham số đá tăng dần từ khả tích sang hỗn loạn; đo trực tiếp $\langle r \rangle$ chuyển 0,39 → 0,53. Đây là hệ chuẩn của hỗn loạn lượng tử cũng như **định xứ động lực học (dynamical localization)** — anh em lượng tử của Anderson localization.
- **Sẹo lượng tử (quantum scars, Heller 1984):** mật độ xác suất cục bộ hàm sóng tập trung quanh quỹ đạo tuần hoàn không ổn định — dấu vết hỗn loạn "sống" trong eigenfunction, đo được trên stadium billiard thực tế (viên bi graphene, vi cộng hưởng quang học).
- **OTOC và giới hạn Maldacena–Shenker–Stanford (2016):** tốc độ lan tỏa thông tin định lượng bằng out-of-time-ordered correlator tăng $e^{\lambda_L t}$ với **$\lambda_L \le 2\pi k_B T/\hbar$** — lỗ đen đạt tới giới hạn này ("fast scrambler") — cầu nối trực tiếp với [[Nguyên lý Holography (AdS-CFT)]].

## Suy luận từ đâu

- Từ cơ học cổ điển phi tuyến (Lyapunov, Poincaré) + cơ học lượng tử ([[Tiên đề cơ học lượng tử]]): quỹ đạo vô nghĩa ở thang $\hbar$, phải đổi ngôn ngữ sang thống kê phổ — nền tảng từ công trình Wigner (1930s, mô hình hạt nhân) và Berry, Bohigas, Gutzwiller.
- Trong giới hạn $\hbar \to 0$ hệ lượng tử trở về cổ điển (nguyên lý tương ứng của [[Nguyên lý bất định Heisenberg]]); hỗn loạn lượng tử là nơi hai thế giới gặp nhau.

## Kiểm chứng & giới hạn

- Kiểm chứng: stadium billiard (microwave cavity thực nghiệm, số liệu khớp GOE tới sai số nhỏ), kicked rotor nguyên tử, dữ liệu mức năng lượng hạt nhân nặng (Wigner), phân tử phức tạp.
- **Giới hạn:** "hỗn loạn lượng tử" không có định nghĩa thống nhất cho hệ trực tiếp (không có quỹ đạo!); thống kê phổ chỉ bắt được hỗn loạn trong kỳ vọng thống kê; hệ ít bậc tự do và hệ nhiều hạt có hành vi khác nhau (nhiều hệ nhiều hạt tương tác yếu → Poisson dù "hỗn loạn" cổ điển).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Nguyên lý bất định Heisenberg]]: ranh giới giữa miêu tả lượng tử và cổ điển.
- [[Tiên đề cơ học lượng tử]]: khung lý thuyết nền.
- [[Lý thuyết trường lượng tử (QFT)]]: hỗn loạn trong không gian pha liên hệ với dòng tái chuẩn hóa.
- [[Nguyên lý Holography (AdS-CFT)]]: giới hạn scrambling — lỗ đen như hệ hỗn loạn nhanh nhất.

## Câu hỏi mở

- Vì sao hệ lượng tử nhiều hạt tương tác yếu (ví dụ khí nguyên tử trung hòa) thường cho thống kê Poisson thay vì Wigner–Dyson? (Gợi ý: tương tác yếu → nhiễu loạn kém trộn phổ → tính khả tích "hiệu dụng".)
- Lỗ đen là fast scrambler ở giới hạn $\lambda_L = 2\pi k_B T/\hbar$ — mọi hệ hỗn loạn lượng tử đều có giới hạn này, nhưng có hệ vật chất "thật" nào chạm giới hạn ngoài lỗ đen (ví dụ chất lỏng holographic) và điều đó nói gì về bản chất thời gian?