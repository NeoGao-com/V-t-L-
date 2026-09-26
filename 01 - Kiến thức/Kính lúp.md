---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: quang-học
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Kính lúp

> [!abstract] Ý chính
> Kính lúp là một [[Thấu kính]] lợi với hình ảnh ảo thu nhỏ về phía mắt, dùng để **phóng đại góc** chứ không phải phóng đại kích thước ảnh. Vì vậy nó là công cụ quang học đầu tiên của loài người, và cũng là công cụ cho thấy đo lường bao giờ cần một *đơn vị tham chiếu* — ở đây là khoảng cách cận cảnh $D = 25$ cm.

## Nội dung

- **Công thức thấu kính mỏng** (dùng chung cho kính lúp, kính lùi, thấu kính của máy ảnh):
  $$\frac{1}{f} = \frac{1}{p} + \frac{1}{q}$$
  quy ước $p > 0$ khoảng cách vật thể, $q > 0$ cho ảnh thật (ngược phía sau kính) và $q < 0$ cho **ảnh ảo** (cùng phía với vật thể). Kính lúp luôn tạo **ảnh ảo**, nên luôn dùng $q < 0$.

- **Nguyên lý phóng đại góc.** Mắt người không nhìn thấy vật thể nhỏ hơn một góc xác định — góc đó quy định bởi khoảng cách **cận cảnh** $D \approx 25$ cm: đối tượng ở $D$ có góc nhìn tối đa, và đó là "bản chuẩn" để so sánh. Công suất phóng đại góc:
  $$M = \frac{\alpha'}{\alpha_0} = \frac{D}{p}$$
  với $p$ là khoảng cách từ kính tới vật thể (mắt áp sát kính). **Chú ý: phóng đại góc, không phải phóng đại kích thước ảnh** — hai đại lượng này chỉ trùng nhau ở một trường hợp duy nhất bên dưới.

- **Hai chế độ dùng:**

  | Chế độ | Điều kiện | $p$ | $M$ |
  | --- | --- | --- | --- |
  | Mắt thả lỏng (ảnh ở vô cùng) | $p = f$ | $f$ | $\dfrac{D}{f}$ |
  | Ảnh ảo ở điểm cận cảnh | $q = -D$ | $\dfrac{fD}{D+f}$ | $1+\dfrac{D}{f}$ |

  Chế độ thứ hai cho $M$ lớn hơn nhưng mỏi mắt hơn — đó là lý do người ta chỉ "nhìn chặt" qua kính lúp khi cần.

- **Ví dụ số.** Kính lúp tiêu cự $f = 5$ cm, $D = 25$ cm:
  - thả lỏng: $p = 5$ cm, $M = \dfrac{25}{5} = 5$
  - chặt: $p = \dfrac{25\times 5}{30} = \dfrac{25}{6} \approx 4{,}17$ cm, $M = 1 + 5 = 6$

  Lưu ý $p < f$ trong chế độ chặt: vật thể phải nằm **bên trong** tiêu điểm, nếu đặt đúng $p = f$ thì ảnh chạy ra vô cùng và mắt phải "cò" mãi mới thấy.

- **Giới hạn thực tế — mắt, không phải kính.** Mắt người phân giải được khoảng **1 phút cung** ($\approx 3\times10^{-4}$ rad). Ở $f = 5$ cm, vật thể nhỏ nhất nhìn được là
  $$d_{\min} \approx f\,\theta_{\text{mắt}} \approx 5\times 3\times10^{-4}\,\text{cm} \approx 15\,\mu\text{m}.$$
  Mua kính lúp $f = 1$ cm chỉ nâng lên $\approx 3\,\mu\text{m}$. Đây là lý do kính lúp điện tử (màn hình + camera) đánh bại kính quang học thuần: nó không còn bị giới hạn bởi độ phân giải mắt người.

## Ý nghĩa vật lý

- **Mắt là một thấu kính đang điều tiêu:** khoảng cách cận cảnh $D \approx 25$ cm chính là lấy từ giới hạn tiêu cự tối thiểu của thể thủy tinh — mắt người "lấy nét gần" được vì thuỷ tinh thể đủ mềm. Với người già, độ chuyển động giảm và cận cảnh lùi ra → cận thị; trẻ em cận cảnh rất gần → viễn thị.
- **Kính lúp như thiết bị đo:** vì nó đo *góc*, nó tuân theo giới hạn nhiễu của dữ liệu: góc đo càng nhỏ thì sai số tương đối càng lớn. Kính lúp không tăng thông tin, nó chỉ đưa thông tin lên gần mức mắt còn đọc nổi.
- **Sự "không phân giải được" là thuộc tính của người quan sát, không phải của vật:** cùng một vật thể, với người có kính lúp và người không, là hai vật thể khác nhau về mặt *quan sát được* — bài học trung tâm của [[Thí nghiệm - Khám phá neutron (Chadwick)]] nơi hạt trung tính chỉ hiện ra dưới kính hiển vi.

## Kiểm chứng & giới hạn

- **Thực nghiệm xác nhận:** nhiều kính lúp dùng chung, $D$ đo bằng cách đưa mắt từ từ lại gần chữ in cho tới khi thấy rõ nhất.
- **Trường hợp không còn đúng:** công thức thấu kính mỏng hỏng khi bán kính cong không nhỏ so với $f$ (kính hội tụ dày, kính thuỷ tinh mắt). Cũng không mô tả được hiệu ứng nhiễu xạ ở kính lúp rất tốt.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Thấu kính]]: kính lúp chỉ là một trường hợp đặc biệt có ảnh ảo.
- [[Mắt và các tật của mắt]]: cơ quan quang học tự nhiên mà kính lúp hỗ trợ.
- [[Lượng giác]]: góc nhìn nhỏ là điều kiện để công thức phóng đại góc tuyến tính hoá được.
- [[Sóng âm]]: cùng nguyên lý nhiễu xạ, dùng để đo kích thước bằng "kính lúp" siêu âm.
- [[Phân tích thứ nguyên]]: kiểm tra nhanh $1/f = 1/p + 1/q$ — cả ba phải cùng thứ nguyên $1/\text{cm}$.

## Câu hỏi mở

- Vì sao kính lúp "phóng đại góc" lại không làm ta nhìn thấy chi tiết mới, dù ảnh trên võng mạc to hơn nhiều lần?
- Có thể chế tạo kính lúp vượt giới hạn 1 phút cung bằng quang học thuần (không dùng điện tử) không?
- Vì sao dải phổ mà mắt nhìn thấy lại hẹp như vậy, và kính lúp có thể mở rộng nó ra sao?
