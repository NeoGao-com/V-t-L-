---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Giải tích Tensor

> [!abstract] Công cụ để làm gì
> Tensor là đại lượng "nhiều chỉ số" biến đổi theo một quy luật cố định khi đổi hệ tọa độ — thứ giữ cho **định luật vật lý giữ nguyên hình dạng trong mọi hệ quy chiếu**. Đây là ngôn ngữ bắt buộc của thuyết tương đối.

## Định nghĩa

- Bậc (hạng) của tensor = số chỉ số: vô hướng hạng 0, vector hạng 1 ($V^\mu$), ma trận hạng 2 ($T^{\mu\nu}$).
- **Quy luật biến đổi (hạng 2):**
  $T'^{\mu\nu} = \Lambda^\mu_{\ \alpha}\, \Lambda^\nu_{\ \beta}\, T^{\alpha\beta}$
  với $\Lambda$ là ma trận chuyển hệ tọa độ. Quy ước tổng Einstein: chỉ số lặp là tổng ngầm.
- **Metric $g_{\mu\nu}$** — "thước đo" khoảng cách trong không-thời gian: $ds^2 = g_{\mu\nu} dx^\mu dx^\nu$; dùng để nâng/hạ chỉ số và co (contract) chỉ số — hai chỉ số chạm nhau là phép "nhân + cộng chéo" cho ra đại lượng bất biến.

## Ý nghĩa hình học

- Tensor là **đối tượng hình học độc lập với tọa độ**: vector không đổi khi ta xoay giấy kẻ ô, chỉ có con số biểu diễn đổi theo quy luật tương ứng — tensor là "bản đồ ứng xử" đó.
- Metric mang hình học: $g_{\mu\nu}$ phẳng (Minkowski) ↔ không-thời gian đặc biệt; $g_{\mu\nu}$ cong ↔ có hấp dẫn — vì "gần nhau" là khái niệm do metric quyết định.

## Ý nghĩa vật lý

- **Bất biến khi đổi hệ quy chiếu:** một phương trình viết bằng tensor giữ nguyên dạng khi chuyển hệ — đúng tinh thần [[Nguyên lý tương đối Galileo]] và [[Thuyết tương đối hẹp]]; phương trình có tensor ở cả hai vế là "luật" còn số đo cụ thể là "cái nhìn của từng quan sát viên".
- **4-vector không-thời gian:** $x^\mu = (ct, x, y, z)$ — thời gian và không gian trộn thành một thực thể; từ đây có giãn thời gian, co chiều dài và động lượng 4-vector $p^\mu = (E/c, \vec p)$ cho $E^2 = p^2c^2 + m^2c^4$ ([[Thuyết tương đối hẹp]], [[Biến đổi Einstein]]).
- **Trường điện từ gói trong một tensor:** $F^{\mu\nu}$ chứa đồng thời $\vec E$ và $\vec B$ — hai "vẻ ngoài" của cùng một thực thể, thay đổi khi quan sát viên chuyển động ([[Điện từ trường]]); Maxwell viết gọn thành hai dòng tensor ([[Phương trình Maxwell]]).
- **Tương đối rộng:** $g_{\mu\nu}$ trở thành "trường hấp dẫn"; phương trình Einstein $G_{\mu\nu} + \Lambda g_{\mu\nu} = \dfrac{8\pi G}{c^4} T_{\mu\nu}$ nối hình học (vế trái) với vật chất–năng lượng (vế phải) — [[Thuyết tương đối rộng]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Thuyết tương đối hẹp]] · [[Biến đổi Einstein]]: 4-vector và bất biến Lorentz.
- [[Điện từ trường]]: tensor trường $F^{\mu\nu}$ hợp nhất $\vec E$ và $\vec B$.
- [[Phương trình Maxwell]]: dạng hiệp biến gọn nhất của bốn phương trình.
- [[Thuyết tương đối rộng]]: metric cong là trường hấp dẫn.
- [[Giải tích Vector (Grad, Div, Curl)]]: vector là trường hợp riêng hạng 1.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Vector]] · [[Hệ tọa độ]] · [[Đại số tuyến tính]] · [[Thuyết tương đối hẹp]] · [[Thí nghiệm - Michelson-Morley]] · [[Thuyết tương đối rộng]]

## Câu hỏi mở

- Khi metric $g_{\mu\nu}$ *không* phẳng (không gian cong), tensor vẫn giữ nguyên quy luật biến đổi — con đường dẫn từ [[Thuyết tương đối hẹp]] đến hấp dẫn (tương đối rộng) đi qua đạo hàm hiệp biến, thứ "sửa" đạo hàm thường để vẫn là tensor. Vì sao cần sửa?
- "Chỉ số lặp là tổng ngầm" nghe như ký hiệu — nhưng nó tương ứng đúng với phép toán nào trong [[Đại số tuyến tính]]? (Gợi ý: tích ma trận và vết.)