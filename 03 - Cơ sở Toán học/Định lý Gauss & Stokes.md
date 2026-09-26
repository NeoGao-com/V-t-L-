---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Định lý Gauss & Stokes

> [!abstract] Công cụ để làm gì
> Hai định lý cầu nối giữa mô tả **địa phương** (div, curl — "tại một điểm") và **toàn cục** (thông lượng, lưu số — "trên miền lớn"). Chúng biến các phương trình Maxwell dạng vi phân thành dạng tích phân tính được bằng đối xứng.

## Định nghĩa

- **Định lý Gauss (divergence):** thông lượng ra khỏi mặt kín bằng tích phân divergence trong thể tích.
  $\iiint_V (\nabla \cdot \vec A)\, dV = \oint_S \vec A \cdot d\vec S$
- **Định lý Stokes (curl):** lưu số quanh đường cong kín bằng thông lượng của curl qua mặt chắn.
  $\iint_S (\nabla \times \vec A) \cdot d\vec S = \oint_C \vec A \cdot d\vec l$

## Ý nghĩa hình học

- **Gauss:** "tổng lượng sản sinh bên trong" = "tổng lượng chảy ra qua biên" — cách nói toàn cục của khái niệm nguồn; một mặt kín "nhìn từ xa" chỉ thấy tổng nguồn chứ không thấy chi tiết bên trong.
- **Stokes:** "tổng độ xoáy trên mặt" = "vòng quay đo được dọc theo đường biên" — quay một vòng quanh mép, ta cộng được tất cả curl bên trong; bề mặt chỉ là "màng chắn", rút về phẳng hay phồng lên đều cho cùng kết quả.

## Ý nghĩa vật lý

- **Gauss → luật Gauss điện:** $\oint_S \vec E \cdot d\vec S = \dfrac{Q_{trong}}{\varepsilon_0}$ — thông lượng điện trường qua mặt kín chỉ phụ thuộc điện tích bên trong ([[Định luật Gauss (điện)]]). Nhờ đó tính được $\vec E$ của đối xứng cầu/trụ/phẳng mà không cần tích phân từng điện tích; là nguồn gốc của luật nghịch đảo bình phương trong [[Định luật Coulomb]].
- **Stokes → luật Faraday:** $\oint_C \vec E \cdot d\vec l = -\dfrac{d\Phi_B}{dt}$ — suất điện động (lưu số của $\vec E$) bằng tốc độ biến thiên từ thông ([[Suất điện động cảm ứng]], [[Từ thông và hiện tượng cảm ứng điện từ]], [[Định luật Faraday về cảm ứng điện từ]]).
- **Gauss với hấp dẫn:** $\oint_S \vec g \cdot d\vec S = -4\pi G M_{trong}$ — cùng cấu trúc toán học, đổi vai trò điện tích → khối lượng ([[Định luật vạn vật hấp dẫn]]).

## Kiến thức vật lý đang sử dụng công cụ này

- [[Định luật Gauss (điện)]]: chọn mặt Gauss đối xứng để tính $\vec E$ mà không cần tích phân từng điện tích.
- [[Phương trình Maxwell]]: dạng tích phân (cảm nhận, đo đạc) ↔ dạng vi phân (tính toán, địa phương).
- [[Suất điện động cảm ứng]]: Stokes giải thích vì sao từ thông biến thiên sinh điện trường xoáy.
- [[Định luật vạn vật hấp dẫn]]: định lý Gauss áp vào trường hấp dẫn.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Tích phân]] · [[Giải tích Vector (Grad, Div, Curl)]] · [[Định luật Gauss (điện)]] · [[Phương trình Maxwell]] · [[Định luật Coulomb]]

## Câu hỏi mở

- Vì sao "thông lượng" và "lưu số" lại là hai đại lượng duy nhất xuất hiện trong Maxwell? (Gợi ý: chúng là hai cách duy nhất để tích phân trường vector bậc 1 trong không gian 3D.)
- Từ Gauss điện suy ra nếu $Q = 0$ bên trong thì $\vec E$ có thể khác không — vậy thông tin về trường bên trong nằm ở đâu? (Gợi ý: cần thêm điều kiện biên và curl của trường.)