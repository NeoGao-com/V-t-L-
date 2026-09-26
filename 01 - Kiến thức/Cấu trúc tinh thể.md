---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: điện-tử
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Cấu trúc tinh thể

> [!abstract] Ý chính
> Cấu trúc tinh thể là cách các nguyên tử xếp hàng lặp đi lặp lại theo một quy luật — mô tả bằng **ba vectơ cơ sở** $\vec a_1,\vec a_2,\vec a_3$. Mọi tính chất điện tử của vật rắn (dải năng lượng, điện dẫn, từ tính) đều là hệ quả của hình học này, chứ không phải của bản chất nguyên tử đơn lẻ.

## Nội dung

- **Mạng tinh thể:** mọi điểm nguyên tử đều có dạng
  $$\vec R = n_1\vec a_1 + n_2\vec a_2 + n_3\vec a_3, \qquad n_i \in \mathbb{Z}$$
  Ba vectơ $\vec a_i$ gọi là **vectơ nguyên thủy**, và thể tích nguyên thủy là
  $$V = \vec a_1\cdot\left(\vec a_2\times\vec a_3\right).$$
  Thể tích này cũng là **mật độ điểm mạng** (số node trên mỗi đơn vị thể tích = $1/V$) — đại lượng duy nhất quyết định hàng loạt tính chất như nhiệt dung, số lượng carrier.

- **Mạng nghịch đảo (mạng đối ứng):** định nghĩa bằng phép "chiếu" mạng thật vào không gian momentum:
  $$\vec b_1 = \frac{2\pi\,\vec a_2\times\vec a_3}{V}, \qquad \vec b_2 = \frac{2\pi\,\vec a_3\times\vec a_1}{V}, \qquad \vec b_3 = \frac{2\pi\,\vec a_1\times\vec a_2}{V}$$
  và thoả điều kiện trực giao đôi $\vec a_i\cdot\vec b_j = 2\pi\,\delta_{ij}$ (đã kiểm chứng bằng tích phân vector). Mạng nghịch đảo là mạng thật nhìn qua phép biến đổi Fourier — vì vậy có thể dùng cùng một bộ hình học cho cả miền không gian lẫn miền momentum.

- **Cơ sở nguyên thủy (primitive basis):** các trạng thái Bloch viết được thành tổng điện tử phẳng
  $$\psi_{n\vec k}(\vec r) = \frac{1}{\sqrt V}e^{i(\vec k\cdot\vec r)}$$
  với $\vec k$ chạy trong vùng Brillouin đầu tiên. Hệ số $1/\sqrt V$ chính là chuẩn hoá theo thể tích nguyên thủy.

- **Hệ tinh thể & mạng Bravais:** có **7** hệ tinh thể (lục phương, vuông phương, tứ phương, trực tâm, đơn phương, hai phương, ba phương), ứng với **14** mạng Bravais. Phân biệt cần thiết vì hệ vuông phương có thể có 3 mạng khác nhau (P, I, F) khác nhau về hình học *và* về số node.

- **Khoảng cách mặt phẳng:** với mạng vuông phương cạnh $a$, các mặt phẳng song song cắt trục tại các điểm nguyên $(h,k,l)$ cách nhau
  $$d_{hkl} = \frac{a}{\sqrt{h^2+k^2+l^2}}.$$
  Mặt phẳng càng "dày đặc" ($h^2+k^2+l^2$ lớn) thì $d$ càng nhỏ.

- **Điều kiện nhiễu xạ Bragg:** sóng bức xạ chỉ cộng hưởng khi
  $$2d_{hkl}\sin\theta = n\lambda \quad\Longleftrightarrow\quad \sin\theta = \frac{n\lambda\sqrt{h^2+k^2+l^2}}{2a}$$
  (đây chính là điều kiện có nghiệm khi $\dfrac{n\lambda\sqrt{h^2+k^2+l^2}}{2a}\le1$ — đó là điều kiện **loại** mặt phẳng, nền tảng của phương pháp phân tích cấu trúc bằng nhiễu xạ).

## Ý nghĩa vật lý

- **Vì sao kim loại dẫn điện còn cách điện thì không:** mỗi dải năng lượng cho phép số trạng thái bằng số electron, tính theo số node trên mỗi đơn vị thể tích. Dải cho phép chứa electron → dẫn; dải hẹp bị chéo với dải valen → cách điện. **Chỉ cần đếm số node**, tức là dùng $V$ của hình học mạng.
- **Đàn tính dẻo:** số phẳng cắt chạy nhiều nhất là phẳng nguyên tử có mật độ cao nhất, tức phẳng có $d_{hkl}$ nhỏ nhất — lực cắt dẽ bẻ tinh thể theo đúng phẳng đó. Độ dẻo do **hình học mạng** quyết định, không phải do lực liên kết.
- **Nhiễu xạ Rơgen:** đo vị trí và cường độ vạch nhiễu xạ là đo trực tiếp $\vec b_i$ — đây là cách duy nhất đo "thấy" mạng nghịch đảo.
- **Dao động mạng (phonon):** âm thanh trong rắn là tập hợp các mode dao động quanh các node; nhánh nhạy cảm nhất trong phổ âm thanh là nhánh quang âm, và nó truy ngược lại **vân đồng nhất** của cấu trúc tinh thể.
- **Cơ sở toán:** cấu trúc tinh thể là ví dụ kinh điển cho việc một đối xứng rời rạc sinh ra một tập phép biến đổi lặp lại vô hạn — nối trực tiếp [[Lý thuyết nhóm]] với [[Toán tổ hợp]] (đếm số cách tô màu mạng, bản chất của [[Đại số tuyến tính]]).

## Kiểm chứng & giới hạn

- **Thực nghiệm xác nhận:** nhiễu xạ Rơgen đo đúng các giá trị $d_{hkl}$ dự đoán; giản dịch hồi pha cho thấy phổ điện tử phụ thuộc mạng đo được.
- **Trường hợp không còn đúng:** mô hình "node bất biến" hỏng khi — nhiệt độ cao (chất rắn nóng chảy), có tập phối (biến đổi liên tục theo cấu trúc bậc cao), vật liệu không tuần hoàn (kính, polymer, thủy tinh) khi đó phải dùng **hàm phân bố cặp đối xức** thay cho mô hình mạng rời rạc.

## Liên kết

- [[MOC - Kiến thức Vật lý]] · [[MOC - Cơ sở Toán học]]
- [[Lý thuyết nhóm]]: nguồn gốc của 14 mạng Bravais từ nhóm đối xứng không gian.
- [[Sóng âm]]: dao động mạng và nhánh quang âm.
- [[Vector]]: ba vectơ nguyên thủy là cách bố trục tọa độ khắp không gian.
- [[Tích phân]]: chuẩn hoá hàm sóng Bloch theo thể tích nguyên thủy $V$.
- [[Hình học vi phân]]: mặt phẳng, mặt cong và cách tính diện tích bằng [[Tích phân]].
- [[Phân tích nhân khảo]]: mở rộng cấu trúc tinh thể theo tham số nhỏ (ví dụ pha tạp chất loãng).

## Câu hỏi mở

- Vì sao các mạng Bravais lại đúng là 14, và con số 14 có "tự nhiên" từ nhóm đối xứng không?
- Có thể suy ra dải năng lượng chỉ từ hình học mạng (mà không cần biết thế tâm) được không, và sai số sẽ lớn cỡ nào?
- Vì sao graphene (dải Dirac bằng phẳng, Dirac cone) là trường hợp hiếm — điều kiện nào về mạng và liên kết hoá học đã cho phép nó?
