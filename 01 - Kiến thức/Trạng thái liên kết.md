---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Trạng thái liên kết

> [!abstract] Ý chính
> Trạng thái liên kết là trạng thái lượng tử **không thể** viết thành tích của hai trạng thái hệ con: trạng thái toàn phần có thông tin về hệ con thứ nhất và hệ con thứ hai *cùng lúc*, không phải thông tin riêng của cái nào. Nó biến "toàn thể là tổng các phần" — điều mà trực giác thông thường của chúng ta mặc định là đúng — thành điều chỉ đúng ở cấp vi mô.

## Nội dung

**Tạp phối.** Trạng thái tổng của hai hệ con là *tạp phối* nếu có thể viết
$$|\Psi\rangle = |\alpha\rangle\otimes|\beta\rangle,$$
nghĩa là toàn bộ thông tin nằm ở $|\alpha\rangle$ và $|\beta\rangle$. Trường hợp ngược lại gọi là **liên kết** (entangled).

**Cơ sở tính toán.** Với hai hạt spin $\tfrac12$, dùng cơ sở $\{|0\rangle,|1\rangle\}$ cho mỗi hạt, không gian toàn phần có cơ sở 4 chiều $\{|00\rangle,|01\rangle,|10\rangle,|11\rangle\}$.

**Bốn trạng thái Bell** (đã kiểm chứng chuẩn hoá và trực giao đôi một):
$$|\Phi^\pm\rangle = \frac{|00\rangle\pm|11\rangle}{\sqrt2}, \qquad |\Psi^\pm\rangle = \frac{|01\rangle\pm|10\rangle}{\sqrt2}$$
Tất cả bốn đều thỏa $|\Psi|^2 = 1$, và $\langle\Phi^+|\Psi^+\rangle = 0$ — chúng là một bộ cơ sở trực chuẩn của không gian hai qubit.

**Phép kiểm tra dứt điểm: truy vết một phần.** Cách chứng minh một trạng thái là liên kết mà không cần "nhìn" vào nó: lấy ma trận mật độ $\rho = |\Psi\rangle\langle\Psi|$, rồi **lấy truy vết theo hệ con thứ hai** (tức lấy tổng các phần tử trên đường chéo) để được ma trận trạng thái của hệ con thứ nhất. Kết quả:

- Với $|\Phi^\pm\rangle$ hay $|\Psi^\pm\rangle$: $\rho_A = \dfrac{\mathbb 1}{2}$ — **hỗn đoàn**, hạng 2.
- Với trạng thái tạp phối: $\rho_A = |\alpha\rangle\langle\alpha|$ — hạng 1.

Vì ma trận toàn phần có hạng 1 (trạng thái thuần) mà truy vết một phần lại có hạng 2, trạng thái đó **không thể** là tích — đó là liên kết. (Đã kiểm chứng bằng máy: hạng truy vết một phần bằng 2 cho cả bốn trạng thái Bell, bằng 1 cho $|00\rangle$.)

**Nội dung thống kê đo được.** Với $|\Phi^\pm\rangle$, đo $Z\otimes Z$ luôn cho $+1$ với xác suất 1 (hai hạt **luôn** cùng phát ra cùng kết quả), và đo $X\otimes X$ cho $\pm1$ tương ứng dấu $\pm$ — cả hai đã kiểm chứng. Với $|\Psi^\pm\rangle$, đo $Z\otimes Z$ luôn cho $-1$ (hai hạt luôn **ngược** kết quả). Sự tương quan hoàn hảo này là dấu hiệu đặc trưng: với hai hạt độc lập, xác suất cả hai cùng phát ra là $25\%$, không phải $100\%$.

**Bất đẳng thức CHSH.** Với bốn trạng thái Bell, giá trị CHSH đạt **giới hạn Tsirelson** $S = 2\sqrt2 \approx 2{,}828$ (đã kiểm chứng: cần bộ cài đo nghiêng $45^\circ$, ví dụ $a=Z,\ b=\frac{Z+X}{\sqrt2},\ a'=X,\ b'=\frac{Z-X}{\sqrt2}$; trạng thái tạp phối $|00\rangle$ với cùng bộ cài đó chỉ cho $S=\sqrt2$). Mọi hệ thống cổ điển đều bị giới hạn $S\le 2$ — đó là lý do thí nghiệm này, lần đầu tiên, **đóng băng thí nghiệm vào bản thân toán học** chứ không phải vào thiết bị.

## Ý nghĩa vật lý

- **Không thể truyền tin tức thần kỳ:** đo trạng thái liên kết cho kết quả ngẫu nhiên hoàn toàn, không ai trong hai hạt "biết" kết quả trước. Nhưng nếu **một** bên đo và báo kết quả, phía bên kia *tức thời* có thương lượng liên kết tương ứng — đó là "không thông tin", chỉ là dữ liệu tương quan đã sẵn có trong trạng thái.
- **Mây thuận toán–cơ:** tổng các cặp hành vi cục bộ vẫn bằng 0 (Bell) dù mỗi hạt riêng có hành vi rõ ràng — mâu thuẫn chỉ xuất hiện ở cấp toàn thể, và chỉ tồn tại trong phép đo.
- **Vật liệu và thông tin:** ở nhiệt độ thấp, trạng thái liên kết của các spin tạo **trạng thái rắn lượng tử** (spin liquid), không có trật tự dài hạn — một loại trật tự mới mà ngành vật liệu chưa có công cụ kinh hiển nào định nghĩa.
- **Cơ sở toán:** trạng thái là một vectơ trong không gian Hilbert; liên kết là việc vectơ đó **không nằm trong tập tích** $A\otimes B$. Nó nằm ở [[Không gian Hilbert]] và được mô tả gọn bằng [[Ký hiệu Dirac]].

## Kiểm chứng & giới hạn

- **Thực nghiệm xác nhận:** các trạng thái Bell đã được sinh trong phòng thí nghiệm (photon, ion bị ràng buộc, siêu dẫn) và đo trực tiếp bằng nhiễu xạ photon; bất đẳng thức CHSH bị vi phạm vượt xa mức cộng nhiễu thống kê.
- **Trường hợp không còn đúng:** trạng thái liên kết **mờ dần** nhanh chóng khi tương tác với môi trường (giải cấu trúc, mất tính đồng nhất). Đây là vấn đề kỹ thuật trung tâm của mọi máy tính lượng tử — trạng thái Bell dùng đơn vị, sống ngắn hơn một triệu lần so với thời gian tính toán.
- **Tranh luận:** câu hỏi "liên kết là thuộc tính vật lý hay thuộc tính của cách chuẩn bị thí nghiệm" vẫn chưa đóng; các thí nghiệm "không tương tác" (loại bỏ chọn lọc Bell) chỉ tạo tương quan yếu, không vượt CHSH.

## Liên kết

- [[MOC - Kiến thức Vật lý]] · [[MOC - Cơ sở Toán học]] · [[MOC - Chương 3 - Các tiên đề trong cơ học lượng tử]]
- [[Hàm sóng]]: trạng thái liên kết là hàm sóng **không** tách được thành tích.
- [[Toán tử spin]] · [[Ký hiệu Dirac]]: cú pháp dùng ở đây.
- [[Biểu diễn các trạng thái lượng tử]]: mọi trạng thái Bell là tổ hợp các trạng thái cơ sở.
- [[Nguyên lý chồng chất lượng tử]]: bốn trạng thái Bell là hệ cơ sở trực chuẩn, mỗi trạng thái là tổ hợp đều của chúng.
- [[Thí nghiệm - Stern-Gerlach]]: phép đo spin đơn lẻ — nền để so sánh với tương quan liên kết.
- [[Sự chuyển thể]]: hiệu ứng lớn nhất do liên kết, ứng dụng trong [[Entropy]].
- [[Nguyên lý bất định Heisenberg]]: liên kết mở rộng bất định từ đơn hạt sang hệ nhiều hạt.

## Câu hỏi mở

- Có hệ nhiều hạt nào **không** thể mô tả bằng toán tử cục bộ và vẫn gọi là "vật lý" không — hay mọi thứ vẫn giản lị là toán tử trên không gian Hilbert?
- Vì sao CHSH có giới hạn $2\sqrt2$ chứ không phải lớn hơn — trực giác hình học của giới hạn đó là gì?
- Liên kết có thể dùng để tính toán nhanh hơn cổ điểm không, và nếu không thì rào cản nằm ở đâu?
