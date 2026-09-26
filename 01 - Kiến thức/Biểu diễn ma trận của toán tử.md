---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Biểu diễn ma trận của toán tử

> [!abstract] Ý chính
> Trong một cơ sở đã chọn, mỗi toán tử là một ma trận với phần tử $F_{nm} = \langle n|\hat F|m\rangle$: trị trung bình thành tích $c^\dagger F c$, và phương trình trị riêng thành bài toán đại số $\det(F - \lambda I) = 0$ — toàn bộ cơ học lượng tử trở thành đại số tuyến tính ma trận.

## Phát biểu / Định nghĩa

**3. Biểu diễn ma trận của toán tử:**

Trong cơ sở trực chuẩn $\{|n\rangle\}$ (xem [[Biểu diễn các trạng thái lượng tử]]), toán tử $\hat F$ được đặc trưng bởi ma trận (vô hạn) các **phần tử ma trận**:

$F_{nm} = \langle n|\hat F|m\rangle$

Tác dụng lên trạng thái thành phép nhân ma trận: $(\hat F|\psi\rangle)_n = \sum_m F_{nm}c_m$.

**3.1. Phổ gián đoạn:** $F_{nm}$ là ma trận vô hạn thường; trong cơ sở riêng của chính $\hat F$: $F_{nm} = a_n\delta_{nm}$ — **ma trận chéo** với trị riêng trên đường chéo (ví dụ $\hat H$ trong cơ sở năng lượng: $H_{nm} = E_n\delta_{nm}$).

**3.2. Phổ liên tục:** phần tử ma trận thành "hạt nhân" (kernel):

$(\hat F\psi)(p) = \displaystyle\int F(p,p')\,\psi(p')\,dp', \qquad F(p,p') = \langle p|\hat F|p'\rangle$

- Toán tử tọa độ trong biểu diễn xung lượng: $\hat x \to i\hbar\dfrac{\partial}{\partial p}$; toán tử xung lượng: $p\,\delta(p-p')$.
- Hàm riêng chuẩn hóa delta ([[Hàm Dirac delta]]) thay cho cột hữu hạn — khai triển thành tích phân ([[Biến đổi Fourier]]).

**4. Trị trung bình dưới dạng ma trận:**

$\langle\hat F\rangle = \langle\psi|\hat F|\psi\rangle = \sum_{nm} c_n^*\,F_{nm}\,c_m = c^\dagger F c$

- Trong cơ sở riêng của $\hat F$: $\langle\hat F\rangle = \sum_n |c_n|^2 a_n$ — trung bình có trọng số $|c_n|^2$ ([[Phép đo lượng tử]]).
- Dạng mật độ: $\langle\hat F\rangle = \mathrm{Tr}(\hat\rho\hat F)$ với $\rho_{nm} = c_nc_m^*$ — mở đường sang ma trận mật độ cho trạng thái hỗn hợp ([[Trạng thái lượng tử]]).

**5. Phương trình trị riêng dạng ma trận:**

$\hat F|f\rangle = f|f\rangle \;\Longleftrightarrow\; F\,c = f\,c$

— bài toán trị riêng ma trận: nghiệm không tầm thường khi

$\det(F - fI) = 0$ (phương trình đặc trưng/secular)

Giải tìm trị riêng $f$, thế ngược tìm vector riêng $c$; nếu phổ suy biến thì ứng với $k$ vector độc lập cho một không gian riêng chiều $k$. Đây là cách "số hóa" mọi bài toán cơ học lượng tử (cơ sở cắt về $N$ chiều ⟹ ma trận $N\times N$ giải bằng máy tính — nền của hóa học lượng tử tính toán).

## Suy luận từ đâu

- Tiên đề gốc: toán tử quan sát là Hermit trên [[Không gian Hilbert]] ([[Toán tử trong cơ học lượng tử]]); tiên đề đo lường cho trị trung bình ([[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]).
- Công cụ toán: [[Đại số tuyến tính]] — ma trận, định thức, trị riêng, vết; [[Ký hiệu Dirac]] cho các phần tử ma trận.

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: mọi tính toán phổ ([[Quang phổ]], chấm lượng tử, phân tử) giải bằng phương pháp ma trận — tốc độ phá nhiễu/matrix diagonalization khớp đo; ma trận $\hat H$ dùng trong phương pháp LCAO của hóa học lượng tử.
- Trường hợp không còn đúng: cơ sở cắt cụt phải đủ lớn (hội tụ chậm với hàm sóng kỳ dị); phổ liên tục làm ma trận thành toán tử tích phân — tiện hơn khi làm việc trực tiếp trong không gian hàm.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Biểu diễn các trạng thái lượng tử]]
- [[Đại số tuyến tính]]
- [[Toán tử trong cơ học lượng tử]]
- [[Không gian Hilbert]]
- [[Phương trình Schrödinger dạng ma trận]]

## Câu hỏi mở

- Ma trận vô hạn và ma trận hữu hạn khác nhau ở điểm nào bản chất (hội tụ chuẩn, phổ, vết)? (Ví dụ $\mathrm{Tr}[\hat x,\hat p]$ nghịch lý trong ma trận vô hạn.)
- Có thể "tọa độ hóa" bất kỳ toán tử phi Hermit (phân rã, hấp thụ) thành ma trận không — và trị riêng phức nghĩa gì về mặt vật lý? (Năng lượng phức = tuổi thọ hữu hạn.)