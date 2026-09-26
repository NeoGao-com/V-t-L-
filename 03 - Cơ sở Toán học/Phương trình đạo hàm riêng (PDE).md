---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Phương trình đạo hàm riêng (PDE)

> [!abstract] Công cụ để làm gì
> Phương trình đạo hàm riêng (PDE) mô tả **trường** — đại lượng phụ thuộc nhiều biến độc lập (thời gian + không gian). Trong khi [[Phương trình vi phân]] (ODE) mô tả chuyển động của "hạt", PDE mô tả "biển": sóng, nhiệt, điện từ, hàm sóng lượng tử. Toàn bộ vật lý trường đứng trên vài loại PDE kinh điển.

## Định nghĩa

- **PDE:** phương trình chứa đạo hàm riêng của hàm nhiều biến, ví dụ $u(x, t)$ với $\dfrac{\partial u}{\partial t}$, $\dfrac{\partial^2 u}{\partial x^2}$.
- **Bậc và tính tuyến tính:** giống ODE; phương trình tuyến tính được giải bằng chồng chất nghiệm ([[Đại số tuyến tính]]).
- **Điều kiện biên + điều kiện đầu** quyết định nghiệm duy nhất — khác ODE chỉ cần điều kiện đầu. Điều kiện biên có hai loại chính: **Dirichlet** (chốt giá trị $u$ ở mép — ví dụ hai đầu dây buộc chặt, $u = 0$) và **Neumann** (chốt đạo hàm — ví dụ đầu mút thanh cách nhiệt).

Phân loại theo dạng toán tử bậc hai — mỗi "họ" mang một lý tính vật lý hoàn toàn khác:

| Dạng | Phương trình mẫu | Đặc điểm | Hiện tượng |
| --- | --- | --- | --- |
| **Hyperbol** | $\dfrac{\partial^2 u}{\partial t^2} = v^2 \nabla^2 u$ | Gốc nhị thức mẫu $c^2t^2 - x^2$; đảo thời gian $t \to -t$ **giữ nguyên** | Sóng — truyền có tốc độ hữu hạn |
| **Parabol** | $\dfrac{\partial u}{\partial t} = D \nabla^2 u$ | Gốc $t$ bậc một; đảo thời gian **phá vỡ** phương trình | Khuếch tán — lan chậm, bất khả đảo |
| **Elliptic** | $\nabla^2 u = 0$ | Không có thời gian; bài toán "cân bằng" | Trường tĩnh — nhiễu ảnh hưởng toàn miền tức thời |

- Bốn "ông lớn": phương trình **sóng**, **khuếch tán (nhiệt)**, **Laplace/Poisson** và **Schrödinger** $i\hbar\dfrac{\partial \Psi}{\partial t} = \hat H \Psi$.

## Ý nghĩa hình học

- Nghiệm là một "mặt" (hoặc "mặt trải phim theo thời gian") trong không gian nhiều chiều; điều kiện biên "đóng khung" mặt đó ở mép, điều kiện đầu chốt hình dạng ban đầu.
- **Đường đặc trưng (characteristics):** thông tin trên mặt nghiệm truyền dọc theo những đường riêng. Sóng có đặc trưng nghiêng ("vùng ảnh hưởng" có hình nón) — vì sao nhiễu ở đây chỉ chạm tới vùng kia sau thời gian $d/v$; nhiệt không có đặc trưng hữu hạn — vì sao "ấm" lan ra khắp nơi mọi lúc (dù yếu dần). Một bức tranh chung giải thích mọi khác biệt giữa sóng và nhiệt.
- **Tách biến ≈ khai triển vector:** nghiệm viết thành tổng các "mode" $u_n(x) T_n(t)$, mỗi mode là nghiệm riêng ứng với tần số $\omega_n$ — giống khai triển một vector theo cơ sở trực giao ([[Đại số tuyến tính]], [[Không gian Hilbert]]).

## Ý nghĩa vật lý

- **Sóng dừng trên dây cố định hai đầu — ví dụ mẫu:** điều kiện biên Dirichlet $u(0,t)=u(L,t)=0$ buộc độ dài chứa nguyên số nửa bước sóng → tần số riêng $f_n = n\dfrac{v}{2L}$; bậc $n$ cao hơn chỉ "thêm bụng sóng". Chính thủ tục này tạo nên các nốt và âm bội của [[Sóng dừng]] trên dây đàn và ống sáo ([[Sóng cơ]], [[Sóng âm]]).
- **Điện từ:** bốn phương trình Maxwell tách ra phương trình sóng cho $\vec E$, $\vec B$ trong chân không với $v = c$ — ánh sáng là nghiệm sóng của PDE, không cần "môi trường" nào để truyền ([[Phương trình Maxwell]], [[Điện từ trường]], [[Sóng điện từ và thang sóng điện từ]]).
- **Lượng tử:** phương trình Schrödinger là PDE tuyến tính — nguyên lý chồng chất, gói sóng, và toán tử Hamilton $\hat H$ ([[Phương trình Schrödinger]], [[Tiên đề cơ học lượng tử]]).
- **Dẫn nhiệt:** nhiệt độ biến thiên theo phương trình khuếch tán — nhiệt "không truyền sóng" mà lan dần, và quá trình đó bất khả đảo ([[Nhiệt lượng và cách truyền nhiệt]]).
- **Bộ công cụ giải:**
  - **Tách biến → chuỗi modes:** dây rung, ống sáo, hộp cộng hưởng — ra các tần số riêng là "phổ" của hệ ([[Sóng dừng]]).
  - **Biến đổi Fourier:** biến PDE thành ODE (đạo hàm $\partial/\partial x \to ik$) — đại số hóa như [[Biến đổi Fourier]] mô tả.
  - **Hàm Green:** với nguồn điểm $\delta$, nghiệm của bài toán nguồn bất kỳ là tích chập — cùng tinh thần [[Hàm Green]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Phương trình Maxwell]]: PDE bậc nhất cho trường; hệ quả là phương trình sóng.
- [[Phương trình Schrödinger]]: PDE nền của cơ học lượng tử, nghiệm mode = mức năng lượng.
- [[Sóng cơ]] · [[Sóng dừng]] · [[Sóng âm]]: phương trình sóng với điều kiện biên Dirichlet.
- [[Nhiệt lượng và cách truyền nhiệt]]: phương trình khuếch tán — bất khả đảo thời gian.
- [[Điện từ trường]] · [[Sóng điện từ và thang sóng điện từ]]: sóng điện từ lan truyền với $v = c$.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Phương trình vi phân]] (ODE — trường hợp đặc biệt 1 biến) · [[Giải tích Vector (Grad, Div, Curl)]] (toán tử $\nabla^2$) · [[Biến đổi Fourier]] · [[Hàm Green]] · [[Chuỗi Taylor & xấp xỉ]] · [[Đại số tuyến tính]] · [[Phương trình Schrödinger]]

## Câu hỏi mở

- Vì sao nhiệt "khuếch tán" còn sóng thì "truyền"? (Gợi ý: phương trình nhiệt bất khả đảo theo thời gian — liên hệ entropy, [[Nguyên lý thứ hai nhiệt động lực học]].)
- Phương trình sóng cho tốc độ truyền $v$ — còn phương trình Schrödinger "truyền" cái gì và tốc độ bao nhiêu? (Gợi ý: gói sóng — nhóm vs pha, [[Lưỡng tính sóng-hạt]].)
- Tách biến hoạt động tốt khi miền "đẹp" (hình chữ nhật, cầu...). Miền méo mó thì sao — và vì sao từng [[Thí nghiệm - Đo phóng xạ]]-kiểu bài toán "không tách được" buộc phải dùng số? (Gợi ý: giá trị riêng của toán tử Laplace trên miền tùy ý — cầu nối với [[Đại số tuyến tính]] số chiều vô hạn.)