---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Phương trình khuếch tán

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Phương trình khuếch tán là **định luật cân bằng cho sự phân tán**: nó mô tả mật độ của chất khí loãng, nhiệt, hay xác suất như một đại lượng vừa tỏa ra theo không gian vừa lan chuyển. Nó là hiện tượng học của hàng nghìn phân tử va chạm ngẫu nhiên, nhưng lại viết được bằng vài ký hiệu. Biến thể Fokker–Planck bổ sung nhiễu ngẫu nhiên và trở thành phương trình nền cho mọi bài toán khuếch tán với nhiễu.

## Định nghĩa

**Phương trình khuếch tán (đơn giản, không kèm dòng):**

$$\dfrac{\partial c}{\partial t} = D\nabla^2 c$$

Trong đó $c(\vec r,t)$ là mật độ cần khuếch tán, $D$ là hệ số khuếch tán, có **thứ nguyên** $\mathrm{m^2/s}$. Với hạt cầu bán kính $R$ lơ lửng trong chất lỏng nhớt, định luật Stokes–Einstein cho $D = \dfrac{k_BT}{6\pi\eta R}$ — chú ý phải có $R$, nếu thiếu thì $k_BT/\eta$ ra đơn vị $\mathrm{m^3/s}$, sai thứ nguyên. Hai vế nói rõ: **vế phải** làm đẳng hóa độ chênh, **vế trái** theo dõi mật độ.

**Phương trình khuếch tán–đối lưu (advection):** $\dfrac{\partial c}{\partial t} + \vec u\cdot\nabla c = D\nabla^2 c$ — khối lượng vật chất vừa bị gió cuốn đi vừa bị nhiễu loãng.

**Phương trình Fokker–Planck (có nhiễu ngẫu nhiên):**

$$\dfrac{\partial P}{\partial t} = -\dfrac{\partial}{\partial x}\left[A(x)P\right] + \frac12\dfrac{\partial^2}{\partial x^2}\left[B(x)P\right]$$

$A(x)$ là độ lệch (drift), $B(x)$ là hệ số khuếch tán tức thời. Trong trường hợp thuần **nhiễu trắc** ($A=0$, $B$ hằng), nó quy lại đúng phương trình khuếch tán — nên Fokker–Planck là phần mở rộng đúng đắn, không phải một thứ khác.

**Quy trình ngẫu nhiên tương đương (định lý Itô):** mọi phương trình Fokker–Planck đều tương đương với một hàm trang bị

$$dx = A(x)\,dt + \sqrt{B(x)}\,\xi(t)$$

trong đó $\xi(t)$ là nhiễu trắc đơn vị ($\langle\xi(t)\xi(t')\rangle = \delta(t-t')$). Vậy lời giải của phương trình phân phối chính là **quỹ đạo của một hạt đơn lẻ** trong nhiễu — một trong những ý tưởng đẹp nhất của vật lý thống kê.

Đối với tiền đề đo lường trực tiếp:

$$P(x,t) = \frac{1}{\sqrt{2\pi\sigma^2}}\exp\!\left(-\frac{(x-x_0)^2}{2\sigma^2}\right),\qquad \sigma^2 = 2Dt$$

## Ý nghĩa vật lý

- **Chuyển động Brown:** hạt phủ phiếu trong dung dịch bị va chạm liên tục; vị trí trung bình $\langle x\rangle = x_0$ **đứng yên**, còn phương sai tăng tuyến tính theo thời gian: $\langle (x-\langle x\rangle)^2\rangle = 2Dt$ — đó chính là hiện tượng tự khuếch tán, thứ định luật Einstein giải thích bằng thuyết động học phân tử ([[Chuyển động Brown]]).
- **Truyền nhiệt:** nhiệt chảy từ nóng sang lạnh theo $q = -k\nabla T$; đó là phương trình khuếch tán với mật độ nhiệt ([[Nhiệt lượng và cách truyền nhiệt]]).
- **Khuếch tán hạt trong kim loại:** quy trình trượt bám giống hệt phân tử đi trong pha rắn.
- **Giải pháp tĩnh trong vận tốc giới hạn:** khi $\vec u$ là hàm của vị trí, phương trình cho phép tìm trạng thái đứng yên của dòng chảy.
- **Nhiệt động lực học:** một trong những định lý bảo toàn nền tảng chính là đẳng cân bằng chi tiết của phương trình khuếch tán — dòng nhiệt tự cân bằng, cân bằng chi tiết trong cơ học Gibbs.
- **Quy mô lan truyền trong không gian ba chiều:** $D$ là hằng số (chỉ phụ thuộc nhiệt độ và môi trường), nhưng **khoảng cách khuếch tán** thì $\propto\sqrt{t}$: hạt đi được quãng đường $\sqrt{2Dt}$ sau thời gian $t$. Chính $\sqrt{t}$ đó là dấu hiệu của bước ngẫu nhiên — đi $n$ bước ngắn $l$ thì quãng đường $\sim l\sqrt n$, không phải $nl$.

## Kiến thức vật lý đang sử dụng công cụ này

- [[Chuyển động Brown]]: hiện tượng ngẫu nhiên rõ ràng nhất mà định luật xác định được.
- [[Thuyết động học phân tử]]: suy ra phương trình khuếch tán từ cơ chế va chạm ở cấp độ phân tử.
- [[Nhiệt lượng và cách truyền nhiệt]]: truyền nhiệt là khuếch tán.
- [[Phương trình trạng thái khí lý tưởng]] · [[Chất khí và khí lý tưởng]]: trạng thái cân bằng là nghiệm tĩnh.
- [[Xác suất thống kê]] · [[Xác suất và trị trung bình]]: mật độ xác suất là hàm cần khuếch tán.
- [[Tĩnh học chất lỏng]]: trường tốc độ trong chất lỏng là nghiệm tĩnh của phương trình Navier–Stokes, phương trình đối lưu–khuếch tán.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Toán tử Laplace]] · [[Phương trình đạo hàm riêng (PDE)]]

## Câu hỏi mở

- Vì sao một hạt đơn lẻ có quỹ đạc rối loạn không thể dự đoán, nhưng **mật độ** của vô số hạt thì tuân theo phương trình tất định? (Gợi ý: xem [[Entropy]].)
- Nếu giảm kích thước không gian, $D$ thay đổi thế nào — và vì sao điều đó lại làm hạt lan chậm hơn? (Gợi ý: dùng [[Phân tích thứ nguyên]].)
- Có thể suy ra phương trình khuếch tán từ định luật cân bằng chi tiết một cách trực tiếp không? (Gợi ý: xem [[Nguyên lý thứ nhất nhiệt động lực học]].)
- Trong vũ trụ, vật lý khuếch tán mở rộng thành "chuyển động vũ trụ" theo nghĩa nào? (Gợi ý: xem [[Giả thuyết - Vụ Nổ Lớn (Big Bang)]].)
