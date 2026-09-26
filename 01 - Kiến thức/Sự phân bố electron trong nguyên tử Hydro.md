---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Sự phân bố electron trong nguyên tử Hydro

> [!abstract] Ý chính
> Xác suất tìm thấy electron phân tích thành phần bán kính $P(r)\,dr = |u(r)|^2dr$ (đỉnh 1s tại bán kính Bohr $a_0$) và phần góc $|Y_{lm}|^2$ (hình cầu cho $s$, hình tạ cho $p$, bốn cánh cho $d$...) — đây là "orbital" mà hóa học dùng để xây dựng bảng tuần hoàn.

## Phát biểu / Định nghĩa

Từ hàm sóng chuẩn hóa $\psi_{nlm} = R_{nl}(r)Y_{lm}$ ([[Nguyên tử Hydro]]), mật độ xác suất trong thể tích $dV = r^2dr\,d\Omega$:

$|\psi_{nlm}|^2\,dV = \underbrace{|R_{nl}|^2 r^2 dr}_{P_{nl}(r)\,dr}\;\cdot\;\underbrace{|Y_{lm}|^2\,d\Omega}_{\text{phần góc}}$

**4.1. Phân bố theo bán kính** $P_{nl}(r) = r^2|R_{nl}(r)|^2 = |u_{nl}(r)|^2$:

1. **Trạng thái 1s:** $P_{10}(r) = \dfrac{4r^2}{a_0^3}e^{-2r/a_0}$ — **cực đại duy nhất tại $r = a_0$**: bán kính Bohr xuất hiện tự nhiên như "bán kính khả dĩ nhất", không phải quỹ đạo vẽ sẵn.
2. **Trị trung bình:** $\langle r\rangle_{nl} = \dfrac{a_0}{2}\left[3n^2 - l(l+1)\right]$; với 1s: $\langle r\rangle = \dfrac{3}{2}a_0$ — khác điểm cực đại (phân bố lệch, đuôi dài).
3. **Hình dạng:** $n$ tăng → phân bố lan rộng (tỉ lệ $n^2$); trạng thái $l$ cao có đỉnh đẩy ra xa (thế ly tâm — [[Phương trình Schrödinger trong trường xuyên tâm]]); số nút $n - l - 1$.
4. Xác suất tại gốc $|R_{nl}(0)|^2$ chỉ khác 0 khi $l = 0$ — hệ quả quan trọng cho hiệu ứng chụp electron và tương tác siêu tinh tế.

**4.2. Phân bố theo góc** $|Y_{lm}(\theta,\phi)|^2$:

- **Không phụ thuộc $\phi$:** $|Y_{lm}|^2$ chỉ có trục $z$ được chọn ($\hat L_z$ xác định) — đối xứng quanh trục $z$; theo $\theta$ có $l - |m|$ nút.
- Hình dạng điển hình ([[Toán tử mô-men xung lượng]] cho $Y_{lm}$):
  - $s$ ($l=0$): **hình cầu** đẳng hướng, $|Y_{00}|^2 = \dfrac{1}{4\pi}$.
  - $p$ ($l=1$): **hình tạ** dọc theo trục (cực đại theo $\theta$ phù hợp $m$).
  - $d$ ($l=2$): bốn cánh trong mặt phẳng (hoặc hai hình tạ theo trục cho $m=0$).
- Chồng chập các $m$ (trạng thái không phải hàm riêng của $\hat L_z$) làm mất đối xứng trục — ví dụ orbital lai hóa $sp^3$ trong hóa học.

**Ứng dụng:** khái niệm orbital s/p/d quyết định liên kết hóa học và cấu trúc bảng tuần hoàn; tiết diện hiệu dụng trong nguyên tử phụ thuộc sự phân bố này (ví dụ $|R_{nl}(0)|^2 \propto \dfrac{Z^3}{n^3}$ cho trạng thái $s$).

## Suy luận từ đâu

- Tiên đề gốc: quy tắc Born cho mật độ xác suất $|\psi|^2$ ([[Phép đo lượng tử]], [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]).
- Công cụ toán: tọa độ cầu ([[Hệ tọa độ]]), tích phân Gauss và hàm gamma, hàm cầu ([[Toán tử mô-men xung lượng]]).

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: kích thước nguyên tử đo bằng tán xạ electron (đường kính cỡ $\sim 2a_0$) khớp $\langle r\rangle$; ảnh orbital $d$ chụp bằng kính hiển vi lực/quét mũi dò; quy tắc chọn lọc bắt nguồn từ tích phân $|Y_{lm}|^2$ với mô-men lưỡng cực ([[Quang phổ]]).
- Trường hợp không còn đúng: với nguyên tử nhiều electron, "orbital" chỉ là xấp xỉ trường trung bình (thế không xuyên tâm, electron tương quan); khi đo liên tục, phân bố bị nhiễu loạn — không còn $\psi_{nlm}$ thuần.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Nguyên tử Hydro]]
- [[Toán tử mô-men xung lượng]]
- [[Phép đo lượng tử]]
- [[Quang phổ]]
- [[Mẫu nguyên tử Bohr]]

## Câu hỏi mở

- "Đám mây electron" có phải biểu diễn chính xác nhất của nguyên tử — hay còn cần mô tả theo dòng xác suất ([[Mật độ dòng xác suất]]) để hiểu trạng thái dừng?
- Vì sao hóa học lại "sống" ở lớp vỏ ngoài — mối liên hệ định lượng giữa $\langle r\rangle_{nl}$ và bán kính hiệu dụng của bảng tuần hoàn?