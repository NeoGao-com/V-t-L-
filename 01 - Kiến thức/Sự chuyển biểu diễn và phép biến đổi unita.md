---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Sự chuyển biểu diễn và phép biến đổi unita

> [!abstract] Ý chính
> Đổi cơ sở = phép biến đổi unita: cột trạng thái quay $\vec c' = S\vec c$, ma trận toán tử biến đổi đồng dạng $F' = SFS^\dagger$ — phép quay trong không gian Hilbert bảo toàn mọi kết quả vật lý (trị riêng, tích vô hướng, vết) vì vật lý không phụ thuộc "bảng tọa độ" ta chọn.

## Phát biểu / Định nghĩa

**8.1. Sự chuyển biểu diễn:**

Cho hai cơ sở trực chuẩn $\{|n\rangle\}$ và $\{|n'\rangle\}$; ma trận chuyển cơ sở (unita):

$S_{n'n} = \langle n'|n\rangle, \qquad S^\dagger S = SS^\dagger = I$

**8.2. Biến đổi của trạng thái (hàm sóng):**

$c'_n = \sum_m S_{nm}\,c_m, \qquad \vec c' = S\,\vec c$

Ví dụ quen thuộc: đổi từ biểu diễn tọa độ sang xung lượng là phép biến đổi Fourier $\varphi(p) = \dfrac{1}{\sqrt{2\pi\hbar}}\displaystyle\int\psi(x)e^{-ipx/\hbar}dx$ ([[Biến đổi Fourier]], [[Biểu diễn các trạng thái lượng tử]]).

**8.3. Biến đổi của toán tử:**

Bảo toàn phần tử ma trận $\langle n'|\hat F|n'\rangle' \leftrightarrow \langle n|\hat F|n\rangle$ đòi hỏi:

$F' = S\,F\,S^{\dagger}$ (phép biến đổi đồng dạng — similarity transformation)

Ví dụ: chéo hóa $\hat H$ trong cơ sở khởi đầu (tùy ý) thành ma trận chéo năng lượng bằng cách chọn $S$ làm cột vector riêng.

**8.4. Tính chất của phép biến đổi unita:**

1. Bảo toàn tích vô hướng: $\langle\psi'|\varphi'\rangle = \langle\psi|\varphi\rangle$ — xác suất chuyển không đổi.
2. **Phổ bất biến:** $F'$ và $F$ có cùng trị riêng (phương trình đặc trưng $\det(F - \lambda I)$ bất biến) — năng lượng, mức phổ không đổi khi đổi biểu diễn.
3. Vết bất biến: $\mathrm{Tr}\,F' = \mathrm{Tr}\,F$ — hữu ích cho $\langle\hat F\rangle = \mathrm{Tr}(\rho F)$.
4. Bảo toàn hệ thức giao hoán: $[F',G'] = [F,G]'$ — cấu trúc đại số (ví dụ $[\hat x,\hat p] = i\hbar$) độc lập biểu diễn.
5. Unita = "phép quay" trong [[Không gian Hilbert]]: giữ nguyên độ dài và góc; lũy thừa $S = e^{i\hat G}$ với $\hat G$ Hermit (toán tử sinh — liên hệ [[Đối xứng và các định luật bảo toàn]]).
6. Nếu $S(t)$ phụ thuộc thời gian: thu được sự chuyển giữa các "bức tranh" (picture) — mở đầu [[Biểu diễn Schrödinger, Heisenberg và tương tác]].

## Suy luận từ đâu

- Tiên đề gốc: không gian trạng thái Hilbert và trạng thái là vector ([[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]) — bất biến của vật lý dưới chọn cơ sở là một đối xứng "tọa độ".
- Công cụ toán: [[Đại số tuyến tính]] (đổi cơ sở, ma trận nghịch đảo, chuẩn hóa trực giao), [[Ký hiệu Dirac]], [[Không gian Hilbert]].

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: cùng một phổ thu được từ nhiều cơ sở tính khác nhau (tọa độ, xung lượng, hàm cầu, LCAO...) — kết quả đo không đổi, đúng dự đoán bất biến unita; chéo hóa số ma trận $N\times N$ cho mức phân tử khớp [[Quang phổ]].
- Trường hợp không còn đúng: cơ sở không đầy đủ (cắt cụt) làm phép đổi cơ sở chỉ gần đúng; biến đổi không unita (phép co, chuẩn hóa lại) thay đổi thể hiện vật lý — dùng có chủ đích cho mô hình hiệu dụng.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Biểu diễn các trạng thái lượng tử]]
- [[Biểu diễn ma trận của toán tử]]
- [[Phương trình Schrödinger dạng ma trận]]
- [[Biểu diễn Schrödinger, Heisenberg và tương tác]]
- [[Không gian Hilbert]]

## Câu hỏi mở

- Phép "chéo hóa" một ma trận Hermit luôn thực hiện được — vậy đâu là thứ không thể biến đổi đi bởi unita? (Bất biến unita: phổ, vết, chuẩn... — "không gian riêng" là cấu trúc thật.)
- Đối xứng (đơn nguyên) và "đổi biểu diễn" (cũng đơn nguyên) — ranh giới giữa chúng là gì? (Một bên không đổi vật lý, nhóm biến đổi do tự nhiên; một bên là quy ước tọa độ của ta.)