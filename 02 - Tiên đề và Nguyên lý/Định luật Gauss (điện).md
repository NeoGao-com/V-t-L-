---
tags:
  - vật-lý/tiên-đề
type: tiên-đề
domain: điện-từ
trạng-thái: ổn-định
created: 2026-09-25
---

# Định luật Gauss (điện)

> [!abstract] Phát biểu tiên đề
> Thông lượng điện trường qua mặt kín tỉ lệ với điện tích chứa trong: $\oint \vec E \cdot d\vec S = \dfrac{Q_{\text{trong}}}{\varepsilon_0}$ — "điện trường 'chảy' ra khỏi một thể tích chỉ do điện tích bên trong".

## Nội dung

- Là dạng **tích phân** của [[Định luật Coulomb]] (tương đương, nhưng mạnh hơn vì dùng được cho phân bố điện tích bất kỳ).
- Dùng tính $E$ khi đối xứng cao: mặt cầu (điện tích điểm/quả cầu), mặt trụ (dây dài), mặt phẳng (bản lớn → điện trường đều của [[Tụ điện]]).
- Công cụ: [[Tích phân]] mặt + [[Định lý Gauss & Stokes]] — cần vận dụng đối xứng trước khi tích phân.

## Bảng: ứng dụng theo đối xứng

| Phân bố | Mặt Gauss | Kết quả |
| --- | --- | --- |
| Điện tích điểm $Q$ | Mặt cầu bán kính $r$ | $E = \dfrac{1}{4\pi\varepsilon_0}\dfrac{Q}{r^2}$ |
| Dây dài $\lambda$ | Mặt trụ bán kính $r$ | $E = \dfrac{\lambda}{2\pi\varepsilon_0 r}$ |
| Mặt phẳng vô hạn $\sigma$ | Hộp trụ xuyên mặt phẳng | $E = \dfrac{\sigma}{2\varepsilon_0}$ |
| Tụ phẳng (2 bản) | Hộp trụ với 1 bản | $E = \dfrac{\sigma}{\varepsilon_0}$ |

## Ví dụ số kiểm chứng được

- **Quả cầu bán kính $R = 0{,}1$ m tích $Q = 1\ \mu$C:** ngoài mặt cầu ở $r = 0{,}2$ m: $E = \dfrac{kQ}{r^2} = \dfrac{9\times10^9 \cdot 10^{-6}}{0{,}04} \approx 2{,}25\times10^5$ N/C — khớp phép đo điện trường bằng cảm ứng điện.
- **Tại sao vật dẫn "rỗng an toàn" (lồng Faraday):** $Q_{\text{trong}} = 0$ trong lòng vật dẫn → $E = 0$ bên trong — nguyên lý chống sét và phòng thí nghiệm chống nhiễu.

## Vì sao đây là tiên đề / vị trí

- Tương đương [[Định luật Coulomb]] nhưng phát biểu **phi địa phương** (toàn mặt kín) — mạnh hơn vì dùng được cho phân bố bất kỳ mà không cần tích phân từng cặp điện tích.
- Là phương trình thứ nhất trong [[Phương trình Maxwell]] — một trong bốn phương trình nền của điện từ học.

## Mở rộng

- Bản "anh em" cho từ trường: thông lượng từ qua mặt kín **luôn bằng 0** (không có điện tích từ) — khác biệt cấu trúc giữa $E$ và $B$ (xem [[Từ trường và cảm ứng từ]]); nếu một ngày phát hiện đơn cực từ, phương trình đồng nhất này sẽ đổi dạng.

## Bằng chứng ủng hộ (thực nghiệm / quan sát)

- **Cân xoắn Coulomb (1785):** phép đo lực tương tác cho kết quả giống hệt dự đoán của dạng tích phân — xem [[Thí nghiệm - Cân xoắn Coulomb]].
- **Lồng Faraday:** khi đặt vật dẫn có điện tích bên trong lồng, điện trường bên trong bằng 0. Đây là kiểm chứng trực tiếp rằng thông lượng qua mặt kín chỉ phụ thuộc điện tích bên trong chứ không phụ thuộc nội dung bên ngoài.
- **Đo điện trường bằng phép cảm ứng tĩnh điện** với độ chính xác cao ở nhiều hình học: kết quả luôn khớp $E = kQ/r^2$, $\sigma/(2\varepsilon_0)$ hay $\sigma/\varepsilon_0$ tùy trường hợp đối xứng trong bảng ở trên.
- **Phương pháp ảnh điện** dùng phương trình Poisson (dạng vi phân của định luật này) dự báo chính xác phân bố trường quanh vật dẫn phức tạp — dùng thành công trong thiết kế chip.

## Nhánh kiến thức xây trên nó

- Tĩnh điện học: [[Điện trường]], [[Tụ điện]], sạch điện tĩnh.
- Mạch điện: ở dạng giới hạn tĩnh cho [[Định luật Kirchhoff]] — điện tích không tích tụ tại nút chính là hệ quả của phương trình liên tục.
- Công cụ toán: [[Tích phân]] mặt, [[Định lý Gauss & Stokes]], [[Phương trình đạo hàm riêng (PDE)]].
- Nền của [[Phương trình Maxwell]] cùng ba phương trình còn lại.

## Kiểm chứng & giới hạn

- Kiểm chứng gián tiếp qua mọi hệ quả của [[Định luật Coulomb]] (thí nghiệm Coulomb 1785, cân xoắn; kiểm chứng trực tiếp hiện đại bằng phép đo $E$ với độ chính xác cao).
- Giới hạn: phát biểu tích phân phải tính được mặt Gauss — bài toán không đối xứng phải về dạng vi phân $\nabla \cdot \vec E = \rho/\varepsilon_0$ và giải số.

## Liên kết

- [[MOC - Tiên đề và Nguyên lý]]
- [[Định luật Coulomb]] · [[Điện trường]] · [[Tích phân]] · [[Phương trình Maxwell]] · [[Tụ điện]] · [[Định lý Gauss & Stokes]] · [[Từ trường và cảm ứng từ]]

## Câu hỏi mở

- Nếu tồn tại đơn cực từ, phương trình $\oint \vec B \cdot d\vec S = 0$ phải đổi thành gì, và vì sao cho tới nay mọi tìm kiếm (Dirac monopole, LHC, tia vũ trụ) đều trống rỗng — cấu trúc lý thuyết nào đang bảo vệ sự vắng mặt đó?