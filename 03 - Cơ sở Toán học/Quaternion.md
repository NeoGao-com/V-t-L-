---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Quaternion

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Quaternion là cách mở rộng số phức bằng **hai thành phần ảo thay vì một**, đổi lại mất đi tính giao hoàn nhưng giữ lại tính đối xứng xoay ba chiều một cách trọn vẹn. Vật lý dùng nó ở ba chỗ: mô tả **spin** (spinor), biểu diễn **đại số suy giảm** của toán tử spin, và mô tả phép quay trong không gian ba chiều không cần nhúng vào phức. Cơ học Hamilton từng chính là thế giới quaternion.

## Định nghĩa

$$\mathbb{H} = \{w + x\hat i + y\hat j + z\hat k \mid w,x,y,z\in\mathbb{R}\}$$

với các quy tắc nhân **không** giao hoàn:

$$\hat i^2 = \hat j^2 = \hat k^2 = \hat i\hat j\hat k = -1,\qquad \hat j\hat k = \hat i = -\hat k\hat j$$

- Mỗi quaternion có **phần thực** $w$ và **phần ảo** $\vec v$ (một quaternion thuần: $w=0$).
- Liên hệ với ma trận $2\times2$ phức: $w+x\hat i+y\hat j+z\hat k \longleftrightarrow \begin{pmatrix} w-iz & y+ix \\ ix-y & w+iz\end{pmatrix}$ — ánh xạ này **bảo toàn phép nhân** ($\phi(q_1q_2)=\phi(q_1)\phi(q_2)$), nên toán tử spin trong lý thuyết lượng tử chính là quaternion.
- **Chuẩn hoá:** $q^{-1} = \dfrac{\bar q}{|q|^2}$ với $\bar q = w - x\hat i - y\hat j - z\hat k$ — giống hệt số phức.
- **Quaternion lấy lũy thừa:** $q^n = |q|^n\left(\cos n\alpha + \hat n\sin n\alpha\right)$, cùng công thức de Moivre như ở [[Số phức]].

**Phép quay.** Với quaternion đơn vị $q = \cos\frac{\alpha}{2} + \hat n\sin\frac{\alpha}{2}$ (góc quay nửa!), vector $\vec v$ được quay bởi phép biến đổi $\vec v' = q\vec v\,q^{-1}$. Công thức khai triển:

$$\vec v' = \vec v\cos\alpha + (\hat n\times\vec v)\sin\alpha + \hat n(\hat n\cdot\vec v)(1-\cos\alpha)$$

**Đẳng vị nhóm:** mọi quaternion đơn vị tạo thành nhóm $SU(2)$, và nó phủ lên $SO(3)$ **hai tầng** — mỗi phép quay ứng với $q$ và $-q$. Chính nhân tố $-1$ đó là "spin kép $\tfrac12$" của lý thuyết lượng tử: cùng một phép quay được mô tả bởi **hai** quaternion $q$ và $-q$ (tức là $\pm\left(\cos\frac{\alpha}{2}+\hat n\sin\frac{\alpha}{2}\right)$, cùng giá trị để quay nhưng đối dấu), và sự phân biệt giữa hai đó là dữ liệu vật lý chứ không chỉ là quy ước toán học. Xem [[Spin của hạt vi mô]], [[Lý thuyết nhóm]].

## Ý nghĩa vật lý

- **Spin là quaternion:** toán tử spin $\hat S_x,\hat S_y,\hat S_z$ thỏa mãn $[\hat S_i,\hat S_j] = i\hbar\epsilon_{ijk}\hat S_k$ — cùng cấu trúc nhân của $\hat i,\hat j,\hat k$. Do đó $\hat S_x \sim \frac{\hbar}{2}\hat i$ và bộ ba toán tử sinh ra đúng nhóm $SU(2)$, còn toán tử quay trong không gian ba chiều sinh ra $SO(3)$ — spin chỉ là "pha kép" của nó.
- **Đại số Pauli:** $\hat\sigma_i$ là các ma trận Hermiti $2\times2$ thỏa mãn $\hat\sigma_i\hat\sigma_j = \delta_{ij}\mathbb{1} + i\epsilon_{ijk}\hat\sigma_k$ (chú ý số hạng $\delta_{ij}\mathbb{1}$: đơn vị phải là **ma trận đơn vị**, không phải số thuần) — hệ quả trực tiếp của việc nhúng quaternion $SU(2)$ vào ma trận. Xem [[Toán tử spin]].
- **Trạng thái spinor:** hạt spin $\tfrac12$ có **hai** trạng thái nội tại $(\alpha,\beta)^T$ ứng với $m_s = \pm\tfrac12$. Đây là **một biến phụ thêm**, không phải sự thay thế cho toạ độ không gian ba chiều: trạng thái đầy đủ là hàm sóng hai thành phần $\psi_\uparrow(\vec r)$, $\psi_\downarrow(\vec r)$ trên không gian vị trí, mỗi thành phần mang một spinor hằng số. Ý tưởng cốt lõi ở [[Hàm sóng]].
- **Cơ học Hamilton:** Hamilton phát minh quaternion trong khi tìm phép nhân "giống phức" cho bộ ba ảo — thứ mà số phức không đủ sức làm. Xem [[Cơ học Hamilton]].
- **Điện tử học tinh thể:** spin–orbit, hằng số $g$ và từ đốn, phân bố hướng spin trong tinh thể ferromagnet.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Toán tử spin]]: ba toán tử sinh ra một cấu trúc nhân giống quaternion.
- [[Spin của hạt vi mô]] · [[Thí nghiệm - Stern-Gerlach]]: lưỡng tính kép của spin, và vì sao gói spin bị phủ đôi.
- [[Lý thuyết nhóm]]: đẳng vị giữa $SU(2)$ và $SO(3)$, lớp phủ hai tầng.
- [[Hàm sóng]]: spinor là biến phụ nội tại hai trạng thái, nhân với hàm sóng vị trí $\psi(\vec r)$ chứ không thay thế nó.
- [[Cơ học Hamilton]]: quaternion là "phức ba chiều" mà Hamilton dùng để mô tả vận tốc.
- [[Đối xứng và các định luật bảo toàn]]: nhóm quay $SO(3)$ sinh ra bảo toàn mô-men động lượng.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Số phức]] · [[Đại số tuyến tính]] · [[Lý thuyết nhóm]] · [[Giải tích Tensor]]

## Câu hỏi mở

- Tại sao mọi phép quay trong không gian ba chiều đều thực hiện được bằng quaternion, nhưng lý thuyết lượng tử lại cần **gấp đôi**? (Gợi ý: xem [[Sự chuyển biểu diễn và phép biến đổi unita]].)
- Vì sao quaternion không thể thay thế số phức trong điện học, dù nó "đầy đủ hơn"? (Gợi ý: xem [[Mạch RLC và trở kháng]].)
- Có thể xây dựng "số siêu phức" với ba thành phần ảo không, và điều gì sẽ hỏng?
- Làm sao nhóm quaternion tạo ra trường vectơ ứng với Tứ phương Klein? (Gợi ý: xem [[Nguyên lý Holography (AdS-CFT)]].)
