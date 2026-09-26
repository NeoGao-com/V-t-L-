---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Cố định gauge (Gauge fixing)

> [!abstract] Ý chính
> Trong lý thuyết gauge, thế vector $A^\mu$ không duy nhất: biến đổi gauge không đổi quan sát vật lý nhưng thay đổi biểu diễn. Cố định gauge thêm điều kiện ràng buộc để triệt thừa bậc tự do, khiến giản đồ Feynman và phép tính hữu hạn, kết quả cuối cùng vẫn bất biến gauge.

## Nội dung

- **Tự do gauge (QED):** $A^\mu \to A^\mu + \partial^\mu \lambda$ không đổi $\vec E$, $\vec B$ — một trường điện từ ứng với **vô số** thế vector (xem [[Phương trình Maxwell]]).
- **Vấn đề khi lượng tử hóa:** photon có 4 thành phần nhưng chỉ 2 trạng thái phân cực thật; các phân cực dọc/thời gian là ảo — không cố định gauge thì propagator suy biến (không khả nghịch), giản đồ Feynman nhận cả trạng thái vô nghĩa.
- **Cố định gauge = thêm điều kiện bổ sung** vào hành động: $S_{gf} = -\frac{1}{2\xi}(\partial_\mu A^\mu)^2$ (họ $R_\xi$), hoặc ràng buộc tọa độ như Coulomb.

## Bảng các gauge phổ biến

| Gauge | Điều kiện | Đặc điểm / dùng khi |
| --- | --- | --- |
| Coulomb | $\nabla \cdot \vec A = 0$ | Tách tĩnh điện trực tiếp; không bất biến Lorentz tường minh |
| Lorenz | $\partial_\mu A^\mu = 0$ | Bất biến Lorentz tường minh — chuẩn cho QED sơ cấp |
| Landau | $\xi = 0$ (họ $R_\xi$) | Không phân cực dọc; tính toán rườm nhưng sạch vật lý |
| Feynman | $\xi = 1$ (họ $R_\xi$) | Propagator photon đơn giản nhất: $-i g_{\mu\nu}/k^2$ |
| Temporal (Weyl) | $A^0 = 0$ | Tiện Hamilton/CR; không Lorentz tường minh |
| Unitarity | dùng trong SM phá vỡ gauge | Không ghost Higgs; tường minh đơn vị |

## Ví dụ vật lý cụ thể

- **Đếm bậc tự do:** QED trong gauge Lorenz: 4 thành phần $A^\mu$ − 1 tự do gauge (chọn $\lambda$) − 1 ràng buộc $\partial_\mu A^\mu = 0$ → 2 phân cực thật của photon. Đây là vì sao photon "chỉ có 2 phân cực" (liên hệ [[Phân cực ánh sáng]]).
- **Photon dọc biến mất:** nếu không cố định gauge, tính toán giản đồ có phân cực dọc đóng góp "ma"; cố định gauge kèm **đồng nhất thức Ward–Takahashi** chứng tỏ chúng triệt tiêu trong mọi S-matrix vật lý.
- **Faddeev–Popov ghost:** trong QCD ($SU(3)$), định thức sinh ra khi cố định gauge cho thêm hạt ma (ghost) chạy trong vòng kín — bắt buộc để bảo toàn đơn vị; QED cũng có ghost nhưng không đóng góp vào vòng.

## Suy luận từ đâu

- Từ tính bất biến gauge của điện từ ([[Phương trình Maxwell]]): đại lượng thật là $\vec E$, $\vec B$ và $F_{\mu\nu} = \partial_\mu A_\nu - \partial_\nu A_\mu$, không phải $A^\mu$.
- Kỹ thuật Faddeev–Popov (1967) là cầu nối từ cố định gauge sang tích phân đường đi của [[Lý thuyết trường lượng tử (QFT)]]; việc chọn hàm Green phù hợp liên quan mật thiết [[Hàm Green]].

## Kiểm chứng & giới hạn

- Kiểm chứng: kết quả vật lý (S-matrix, tiết diện tán xạ) **đồng nhất ở mọi gauge** — đối chiếu tính toán $e^+e^- \to \mu^+\mu^-$ trong gauge Coulomb vs Feynman cho cùng đáp số; thực nghiệm khớp QED tới 10⁻¹² (xem [[Lý thuyết trường lượng tử (QFT)]]).
- **Giới hạn:** cố định gauge dùng được khi tự do gauge "đóng nhưng không khớp" chuẩn; với instanton/topology không tầm thường (bài toán Gribov) một điều kiện gauge không phủ toàn bộ không gian cấu hình — cần xử lý tinh tế hơn.

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Lý thuyết trường lượng tử (QFT)]]: bước tiền thân trước khi lượng tử hóa trường.
- [[Phương trình Maxwell]]: tính bất biến gauge của điện từ.
- [[Hàm Green]]: cố định gauge đi kèm việc chọn hàm Green phù hợp.
- [[Phân cực ánh sáng]]: photon có đúng 2 phân cực vật lý.

## Câu hỏi mở

- Vì sao gauge Lorenz là lựa chọn phổ biến nhất trong các tính toán QED sơ cấp? (Gợi ý: cân bằng giữa điều kiện ràng buộc và tính bất biến Lorentz tường minh.)
- Bài toán Gribov (ảnh hưởng của topology lên cố định gauge trong QCD) chưa giải quyết đầy đủ — liệu có gauge nào "tốt trên toàn cầu" cho $SU(3)$ mà vẫn tiện tính toán không?