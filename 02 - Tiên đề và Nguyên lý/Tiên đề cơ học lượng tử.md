---
tags:
  - vật-lý/tiên-đề
type: tiên-đề
domain: lượng-tử
category: Vật lý Hiện đại
trạng-thái: ổn-định
created: 2026-09-25
---

# Tiên đề cơ học lượng tử

> [!abstract] Phát biểu tiên đề
> Cơ học lượng tử được xây dựng từ một bộ tiên đề chặt chẽ: trạng thái là vector trong không gian Hilbert, quan sát là toán tử Hermite, đo lường trả về trị riêng với xác suất Born, trạng thái tiến hóa theo phương trình Schrödinger. Lưỡng tính sóng–hạt, lượng tử hoá và bất định đều là **hệ quả** của bộ tiên đề này.

## Vì sao đây là tiên đề

- Đây là **bộ tiên đề tối thiểu** sinh ra toàn bộ cơ học lượng tử: mọi kết quả tính được đều là hệ quả toán học của A1–A5, không cần thêm giả thiết nào.
- Không thể rút gọn bộ này xuống cơ học cổ điển: A3 và A4 (kết quả đo rời rạc, xác suất) là nội dung **mới** chưa có gì tương ứng trong vật lý cổ điển.
- Lưu ý về tính độc lập: A1–A5 là lựa chọn một hình thức hóa. [[Lý thuyết trường lượng tử (QFT)]] dựng lại chúng từ các nguyên lý sâu hơn, và hình thức luận đường tích phần Feynman cho kết quả tương đương — nên đây là **tiên đề theo nghĩa hệ quả**, không phải theo nghĩa duy nhất.

## Bằng chứng ủng hộ (thực nghiệm / quan sát)

- **Quang phổ nguyên tử hydro:** các mức $E_n = -13{,}6/n^2$ eV là trị riêng giải được chính xác của $\hat H$ — kiểm chứng mạnh nhất cho A2–A5.
- **Nhiễu xạ electron:** [[Thí nghiệm - Davisson-Germer]] cho thấy bước sóng de Broglie — hàm sóng là đối tượng thật, không phải hình ảnh.
- **Khe đôi electron đơn:** bắn từng electron một, vân giao thoa vẫn hiện — minh hoạ trực tiếp A1 (chồng chất) + A4 (xác suất).
- **Hiệu ứng quang điện, phổ hồng–luys, phổ tia X liên tục:** chỉ giải thích được nếu năng lượng trao đổi **lượng tử hoá**.

## Nhánh kiến thức xây trên nó

**Các tiên đề:**

- **A1 — Trạng thái:** vector đơn vị $|\psi\rangle$ trong [[Không gian Hilbert]], thường biểu diễn bằng hàm sóng $\Psi(x,t)$.
- **A2 — Quan sát:** mỗi đại lượng vật lý ứng với một toán tử tuyến tính **Hermite** $\hat A$.
- **A3 — Kết quả đo:** đo $\hat A$ luôn trả về một trị riêng $a_n$ của nó.
- **A4 — Xác suất (Born):** xác suất đo được $a_n$ là $P_n = |\langle a_n | \psi \rangle|^2$.
- **A5 — Tiến hóa:** giữa các lần đo, trạng thái tiến hóa theo [[Phương trình Schrödinger]] $i\hbar\,\partial_t|\psi\rangle = \hat H|\psi\rangle$.

| Đại lượng | Toán tử | Ghi chú |
| --- | --- | --- |
| Vị trí $x$ | $\hat x = x$ | nhân với tọa độ |
| Động lượng $p$ | $\hat p = -i\hbar\dfrac{\partial}{\partial x}$ | đạo hàm theo tọa độ |
| Năng lượng $E$ | $\hat H = -\dfrac{\hbar^2}{2m}\nabla^2 + V$ | Hamiltonian — xem [[Cơ học Hamilton]] |
| Mô-men động lượng $L$ | $\hat L = \hat r \times \hat p$ | lượng tử hoá: $l = 0, 1, 2, \dots$ |

Các toán tử **không giao hoán**: $[\hat x, \hat p] = i\hbar$ — đây là nguồn gốc của [[Nguyên lý bất định Heisenberg]], không phải vì máy đo kém.

**Hệ quả nổi bật:**

- **Lưỡng tính sóng–hạt:** bước sóng de Broglie $\lambda = \dfrac{h}{p}$.
- **Lượng tử hoá tự nhiên:** trong hố thế vô hạn, $E_n = \dfrac{n^2h^2}{8mL^2}$ xuất hiện từ điều kiện biên $\psi(0) = \psi(L) = 0$ — không cần giả định quỹ đạo như [[Mẫu nguyên tử Bohr]].
- **Chồng chất:** vì tiến hóa (A5) tuyến tính, trạng thái có thể là tổ hợp — xem [[Nguyên lý chồng chất lượng tử]].

## Liên kết

- [[MOC - Tiên đề và Nguyên lý]]
- [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]: khai triển chi tiết theo cấu trúc A1–A5.
- [[Cơ sở toán học của cơ học lượng tử]]: bản đồ công cụ toán học của A1–A5.
- [[Phương trình Schrödinger]] · [[Không gian Hilbert]] · [[Đại số tuyến tính]]
- [[Cơ học Hamilton]] · [[Thuyết tương đối hẹp]]
- [[Nguyên lý bất định Heisenberg]] · [[Nguyên lý chồng chất lượng tử]] · [[Nguyên lý loại trừ Pauli]]
- [[Mẫu nguyên tử Bohr]] · [[Thí nghiệm - Davisson-Germer]]

## Câu hỏi mở

- Bài toán đo lường: A5 mô tả tiến hóa tất định nhưng kết quả đo lại ngẫu nhiên (A3, A4) — "sụp đổ" xảy ra ở đâu và vì sao?
- Vì sao xác suất là $|c_n|^2$ chứ không phải $|c_n|$? Quy tắc Born được thực nghiệm xác nhận nhưng chưa suy ra được từ các tiên đề khác.
- Có thể thay "vector trong Hilbert" bằng cấu trúc khác mà vẫn cho cùng dự đoán không?