---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: nhiệt-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Chuyển động Brown

> [!abstract] Ý chính
> Chuyển động Brown là chuyển động hỗn loạn không ngừng của các hạt nhỏ li ti lơ lửng trong chất lỏng hoặc chất khí, do va chạm ngẫu nhiên với các phân tử của môi trường — là bằng chứng thực nghiệm quan trọng nhất cho sự tồn tại và chuyển động không ngừng của phân tử.

## Nội dung

- **Quan sát gốc:** Robert Brown (1827) thấy hạt phấn hoa lơ lửng trong nước chuyển động hỗn loạn liên tục dưới kính hiển vi.
- **Lời giải lý thuyết:** Albert Einstein (1905) giải thích bằng thuyết phân tử: các phân tử nước va chạm ngẫu nhiên với hạt tạo ra lực ngẫu nhiên $F(t)$ — kết quả là một **bước đi ngẫu nhiên** (random walk).
- **Kết quả toán học:**
  $\langle (\Delta x)^2 \rangle = 2Dt$
  với $D$ là hệ số khuếch tán, $\langle \cdot \rangle$ là phép lấy trung bình xác suất — **độ dịch chuyển trung bình tỉ lệ với $\sqrt{t}$**, không phải $t$.
- **Hệ số khuếch tán (Stokes–Einstein):**
  $D = \dfrac{k_B T}{6\pi \eta r}$
  với $\eta$ là độ nhớt, $r$ là bán kính hạt, $k_B$ là hằng số Boltzmann.

## Ví dụ vật lý cụ thể

- **Hạt polystyrene $r = 0{,}5\,\mu$m trong nước ở 300 K:** $D = \dfrac{1{,}38\times10^{-23}\times300}{6\pi\times10^{-3}\times0{,}5\times10^{-6}} \approx 4{,}4\times10^{-13}$ m²/s. Sau 1 phút: $\langle\Delta x^2\rangle = 2Dt \approx 5{,}3\times10^{-11}$ m² → dịch chuyển căn quân phương $\sqrt{\langle\Delta x^2\rangle} \approx 7{,}3\,\mu$m — gấp ~15 lần đường kính hạt, dễ quan sát dưới kính hiển vi.
- **Quãng đường thực ≫ độ dịch chuyển:** hạt dịch chuyển 7 μm/1 phút nhưng tổng quãng đường bò ngoằn ngoèo dài hơn hàng nghìn lần — điển hình của bước đi ngẫu nhiên; quỹ đạo là đường fractal, không có tiếp tuyến xác định tại mọi điểm.
- **Đo $k_B$:** dựng đồ thị $\langle(\Delta x)^2\rangle$ theo $t$ → độ dốc $2D$ → $k_B = 6\pi\eta r D/T$. Perrin (1908–1909, Nobel 1926) đo theo cách này, khớp với mọi cách đo khác — xác lập thuyết phân tử và hằng số Avogadro.

## Quan sát quan trọng

- Chuyển động Brown chứng tỏ phân tử tồn tại, chuyển động không ngừng và có kích thước hữu hạn — kiểm chứng trực tiếp [[Thuyết động học phân tử]].
- Đồ thị $\langle (\Delta x)^2 \rangle$ theo $t$ là đường thẳng có độ dốc $2D$ — cách trực tiếp để đo $D$, từ đó suy ra $k_B$.

## Ứng dụng

- **Vật lý thống kê:** mô hình nền cho khuếch tán và phản ứng trong chất lỏng; liên hệ trực tiếp với [[Xác suất thống kê]] và [[Entropy]] (chuyển động hỗn loạn làm tăng entropy).
- **Sinh học:** đo độ linh động của phân tử trong tế bào — kính hiển vi theo dõi hạt nano.
- **Mô phỏng phân tử:** cơ sở của mô phỏng động lực phân tử (molecular dynamics) và lý thuyết nhiễu (fluctuation theory).

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: đo $D$ của Perrin khớp công thức Stokes–Einstein; theo dõi hạt nano hiện đại xác nhận $\langle \Delta x^2\rangle \propto t$.
- Trường hợp không còn đúng: hạt quá nhỏ (cỡ phân tử) — Stokes–Einstein phá vỡ, cần thủy động lực học vi mô; hạt tích điện trong dung dịch muối — lực tĩnh điện (Coulomb) làm sai lệch mô hình (chiều dài Debye hữu hạn); chuyển động "chủ động" của vi sinh vật không phải Brown thuần túy.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Quan sát - Chuyển động Brown]]: bằng chứng thực nghiệm gốc (Brown, 1827).
- [[Thuyết động học phân tử]]: khung lý thuyết giải thích chuyển động Brown.
- [[Nội năng]]: liên hệ với năng lượng chuyển động nhiệt của phân tử.
- [[Entropy]]: chuyển động hỗn loạn làm tăng entropy của hệ.
- [[Xác suất thống kê]]: bước đi ngẫu nhiên, trung bình thống kê.
- [[Thí nghiệm - Đo công suất tỏa nhiệt]]: cả hai đều đo hằng số Boltzmann $k_B$.

## Câu hỏi mở

- Với hạt rất nhỏ (ví dụ virus), lực tĩnh điện (Coulomb) giữa các hạt tích điện có thể làm sai lệch mô hình Stokes–Einstein không? (Gợi ý: độ dài Debye trong dung dịch muối là hữu hạn.)
- Vì sao chuyển động Brown "không bao giờ dừng"? (Gợi ý: nếu dừng, entropy giảm — vi phạm nguyên lý II; năng lượng nhiệt của môi trường vô tận ở thang hạt nhỏ.)
- Vì sao hạt càng nhỏ chuyển động càng dữ dội? (Gợi ý: $D \propto 1/r$ và số va chạm mất cân bằng tỉ lệ $1/\sqrt{N}$ — nhiễu tương đối lớn hơn.)