---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Biểu diễn các trạng thái lượng tử

> [!abstract] Ý chính
> Trạng thái lượng tử là một vector trừu tượng trong không gian Hilbert — "biểu diễn" chỉ là bộ tọa độ của vector đó trong một cơ sở đã chọn: biểu diễn năng lượng dùng các hệ số $c_n = \langle n|\psi\rangle$, biểu diễn xung lượng dùng hàm $\varphi(p)$ là biến đổi Fourier của $\psi(x)$; đổi biểu diễn là đổi cách hỏi, không đổi thực tại lượng tử.

## Phát biểu / Định nghĩa

**1. Khái niệm về biểu diễn:**

Chọn một cơ sở trực chuẩn đầy đủ $\{|n\rangle\}$ của [[Không gian Hilbert]] (thường là hệ hàm riêng chung của một bộ đầy đủ các quan sát giao hoán — xem [[Đo đồng thời các đại lượng trong cơ học lượng tử]]). Trạng thái $|\psi\rangle$ được mô tả bằng bộ **hệ số khai triển**:

$c_n = \langle n|\psi\rangle, \qquad |\psi\rangle = \sum_n c_n\,|n\rangle, \qquad \sum_n |c_n|^2 = 1$

Bộ $(c_1, c_2, \dots)$ là "bộ tọa độ" của $|\psi\rangle$ trong cơ sở đó — cùng một trạng thái, vô số biểu diễn khác nhau. Xác suất đo được giá trị riêng $a_n$ là $|c_n|^2$ ([[Phép đo lượng tử]]).

**2.1. Biểu diễn năng lượng:**

Cơ sở $\{|\varphi_n\rangle\}$ là các trạng thái dừng $\hat H|\varphi_n\rangle = E_n|\varphi_n\rangle$. Khi đó:

$\Psi(t) = \sum_n c_n(t)\,|\varphi_n\rangle, \qquad c_n(t) = c_n(0)\,e^{-iE_n t/\hbar}$

— mỗi hệ số quay với pha riêng của mức $E_n$; $|c_n(t)|^2 = |c_n(0)|^2$ không đổi (xác suất của mỗi mức bảo toàn, phù hợp [[Nghiệm dừng của phương trình Schrödinger]]).

**2.2. Biểu diễn xung lượng:**

Cơ sở liên tục $\{|p\rangle\}$ (chuẩn hóa delta: $\langle p|p'\rangle = \delta(p-p')$ — [[Hàm Dirac delta]]):

$\varphi(p,t) = \langle p|\Psi(t)\rangle = \dfrac{1}{\sqrt{2\pi\hbar}}\displaystyle\int_{-\infty}^{\infty}\Psi(x,t)\,e^{-ipx/\hbar}\,dx$

và nghịch đảo: $\Psi(x,t) = \dfrac{1}{\sqrt{2\pi\hbar}}\displaystyle\int\varphi(p,t)\,e^{ipx/\hbar}\,dp$ — $\varphi(p)$ **là biến đổi Fourier** của $\psi(x)$ ([[Biến đổi Fourier]]). Hệ quả:

- $|\varphi(p)|^2\,dp$: xác suất đo được xung lượng quanh $p$ — đối xứng hoàn toàn với $|\psi(x)|^2\,dx$.
- Parseval: $\displaystyle\int|\psi|^2\,dx = \int|\varphi|^2\,dp = 1$ — biểu diễn bảo toàn chuẩn.
- $\hat x$ và $\hat p$ là cặp biến liên hợp Fourier ⟹ độ rộng hai biểu diễn tỉ lệ nghịch: nguồn gốc toán học của [[Nguyên lý bất định Heisenberg]].

## Suy luận từ đâu

- Tiên đề gốc: không gian trạng thái là [[Không gian Hilbert]], trạng thái là vector (tiên đề 1–2 trong [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]); khai triển theo hàm riêng của toán tử quan sát.
- Công cụ toán: [[Đại số tuyến tính]] (cơ sở, tọa độ), tích phân Fourier ([[Biến đổi Fourier]], [[Hàm Dirac delta]]), [[Ký hiệu Dirac]].

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: hệ số $c_n$ quyết định xác suất chuyển mức — đo qua cường độ vạch [[Quang phổ]]; biểu diễn xung lượng dùng khắp trong tán xạ (biên độ tán xạ là hàm theo $p$).
- Trường hợp không còn đúng: cơ sở phải là hệ đầy đủ — thiếu thành phần (ví dụ quên spin trong không gian con) làm khai triển sai; với trạng thái hỗn hợp (không thuần) cần [[Trạng thái lượng tử|ma trận mật độ]] thay vì vector.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Trạng thái lượng tử]]
- [[Không gian Hilbert]]
- [[Ký hiệu Dirac]]
- [[Biến đổi Fourier]]
- [[Phép đo lượng tử]]
- [[Biểu diễn ma trận của toán tử]]

## Câu hỏi mở

- Biểu diễn tọa độ $\psi(x)$, xung lượng $\varphi(p)$ và năng lượng $c_n$: cái nào "thật nhất"? (Cả ba chỉ là tọa độ — nhưng mỗi phép đo buộc ta "xem" bằng đúng "hệ tọa độ" của máy đo.)
- Vì sao $\hat x$ và $\hat p$ "liên hợp Fourier" — có thể xây cặp liên hợp khác tương tự (năng lượng–thời gian) không? (Gợi ý: giới hạn khác về phổ/số đo.)