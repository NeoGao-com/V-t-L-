---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Mật độ dòng xác suất

> [!abstract] Ý chính
> Bên cạnh mật độ xác suất $\rho = |\Psi(\vec r,t)|^2$, còn tồn tại một đại lượng **dòng xác suất** $\vec J$ sao cho xác suất được bảo toàn cục bộ qua phương trình liên tục $\dfrac{\partial \rho}{\partial t} + \vec\nabla\cdot\vec J = 0$.

## Phát biểu / Định nghĩa

Với hàm sóng $\Psi(\vec r,t)$, "vận tốc" chảy của xác suất được định nghĩa bởi vectơ mật độ dòng xác suất:

$\vec J(\vec r,t) = \dfrac{\hbar}{2mi}\left(\Psi^*\vec\nabla\Psi - \Psi\vec\nabla\Psi^*\right) = \dfrac{1}{m}\,\mathrm{Re}\!\left(\Psi^*\hat{\vec p}\,\Psi\right)$

- Trong một chiều: $J = \dfrac{\hbar}{2mi}\left(\Psi^*\dfrac{\partial\Psi}{\partial x} - \Psi\dfrac{\partial\Psi^*}{\partial x}\right)$.
- Với sóng phẳng $\Psi = Ae^{i(kx-\omega t)}$: $J = |A|^2\dfrac{\hbar k}{m} = |A|^2 v$, tức xác suất chảy cùng vận tốc nhóm $v = \dfrac{p}{m}$.
- **Phương trình liên tục** (suy ra trực tiếp từ phương trình Schrödinger phụ thuộc thời gian):

$\dfrac{\partial\rho}{\partial t} + \vec\nabla\cdot\vec J = 0$

Tích phân trên toàn không gian (với $\Psi \to 0$ khi $r\to\infty$) cho bảo toàn toàn cục: $\dfrac{d}{dt}\int\rho\,dV = 0$, nghĩa là **số hạt được bảo toàn**.

## Suy luận từ đâu

- Tiên đề gốc: tiên đề về hàm sóng và xác suất (Born) trong [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]] — $\rho = |\Psi|^2$ là mật độ xác suất; [[Phương trình Schrödinger]] mô tả tiến hóa.
- Công cụ toán: đạo hàm riêng và định lí Gauss; lấy $\Psi^*\times$ (phương trình Schrödinger) trừ liên hợp phức rồi rút gọn.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: bảo toàn điện tích trong các thí nghiệm tán xạ chùm electron — tổng dòng phản xạ + truyền qua luôn bằng dòng tới (thấy ở [[Thế bậc thang]] và [[Hàng rào thế và hiệu ứng đường ngầm]]); dòng xác suất chính là cơ sở để tính cường độ trong kính hiển vi quét xuyên hầm (STM).
- Trường hợp không còn đúng: mô tả xác suất đơn hạt không còn đúng khi có tạo/hủy hạt (cần lý thuyết trường lượng tử); với trạng thái dừng có hàm sóng thực thì $J = 0$ — trạng thái "đứng yên" thật sự, không có dòng.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Phương trình Schrödinger]]
- [[Hàm sóng]]
- [[Thế bậc thang]]
- [[Hàng rào thế và hiệu ứng đường ngầm]]

## Câu hỏi mở

- Dòng xác suất của một chồng chập có phải bằng tổng các dòng thành phần không? (Không — có số hạng giao thoa, đây là nguồn gốc của giao thoa lượng tử.)
- Có thể đo trực tiếp $\vec J$ hay chỉ gián tiếp qua dòng hạt tới detector?