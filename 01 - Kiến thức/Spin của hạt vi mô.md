---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: lượng-tử
trạng-thái: ổn-định
created: 2026-09-25
---

# Spin của hạt vi mô

> [!abstract] Ý chính
> Electron (và mọi fermion) có mômen động lượng **nội tại** $\vec s$ với $s = \tfrac{1}{2}$: không đo được qua chuyển động quỹ đạo, không phải "tự quay" vật chất — chỉ hiện diện qua mômen từ $\mu_s = -g_s\mu_B m_s$ với $g_s \approx 2$; thí nghiệm Stern–Gerlach ($l = 0$ mà vẫn tách hai vệt $\pm\mu_B$) là chứng cứ trực tiếp.

## Phát biểu / Định nghĩa

**3.1. Thí nghiệm Stern–Gerlach:**

Nguyên tử trung hòa (bạc) qua từ trường không đồng nhất; cổ điển dự đoán một vệt trải liên tục, kết quả là **hai vệt rời rạc** $\mu_z = \pm\mu_B$. Vì trạng thái cơ bản của bạc có $l = 0$ (không có mômen quỹ đạo), hai vệt phải sinh từ **mômen từ nội tại** — chi tiết: [[Thí nghiệm - Stern-Gerlach]].

**3.2. Spin của hạt vi mô:**

- **Định nghĩa:** electron, proton, neutron có spin $s = \frac{1}{2}$; photon có $s = 1$; pion, Higgs $s = 0$ (xem [[Mô hình chuẩn (Standard Model)]]). Hình chiếu lên trục đo: $m_s = \pm\frac{1}{2}$, số chiếu $2s + 1 = 2$.
- **Số lượng tử spin** $s$ cố định cho từng loại hạt; với hệ nhiều electron, tổng spin $\vec S$ tuân phép cộng mômen xung lượng ([[Toán tử spin]]).
- **Mômen từ spin:** $\hat{\vec\mu}_s = -g_s\,\mu_B\,\dfrac{\hat{\vec s}}{\hbar}$, với $g_s \approx 2{,}0023$ — **hệ số Landé dị thường** của electron; $g_s \approx 2$ là tiên đoán phương trình Dirac, chênh $a_e = \dfrac{g_s-2}{2} \approx 0{,}00115965$ là hiệu chỉnh QED ([[Lý thuyết trường lượng tử (QFT)]]).
- **Tại sao không phải "tự quay":** mô hình quay cổ điển với mômen quán tính electron đòi hỏi vận tốc xích đạo $v \gg c$; hơn nữa spin không viết được qua $\hat{\vec r}\times\hat{\vec p}$ ([[Toán tử mô-men xung lượng]] mục Giới hạn) — spin là thuộc tính nội tại, chỉ có ở vũ trụ lượng tử tương đối tính.
- **Nguyên lý spin–thống kê:** spin bán nguyên ⟹ fermion; spin nguyên ⟹ boson (xem [[Nguyên lý loại trừ Pauli]], [[Lý thuyết trường lượng tử (QFT)]]).

## Suy luận từ đâu

- Thực nghiệm gốc: [[Thí nghiệm - Stern-Gerlach]] (1922); đề xuất Goudsmit–Uhlenbeck (1925); hệ số 2 từ phương trình Dirac (1928); phân rã $g_s$ từ QED.
- Cấu trúc toán: spin là biểu diễn bán nguyên của nhóm quay — $SU(2)$ chứ không $SO(3)$ ([[Toán tử spin]], [[Sự chuyển biểu diễn và phép biến đổi unita]]).

## Kiểm chứng & giới hạn

- Thực nghiệm xác nhận: Stern–Gerlach (2 vệt); $\mu_s = 1{,}001\mu_B$ đo cực chính xác bằng bẫy Penning ($a_e$ khớp QED tới 12 chữ số trong công thức — kiểm tra tinh tế nhất của QED); cấu trúc tinh tế của phổ hydro và hiệu ứng Zeeman bất thường ([[Hiệu ứng Zeeman]], [[Quang phổ]]); cộng hưởng spin điện tử; neutron có mômen từ $\mu_n = -1{,}91\mu_N$ (mang điện tích quark tích lũy) — spin hiện diện cả ở hạt trung hòa.
- Trường hợp không còn đúng: khái niệm "hướng spin xác định" sụp khi hai chiếu chồng chập (đo thành phần khác phá vỡ trạng thái — [[Nguyên lý bất định Heisenberg]]); trong QFT, spin gắn với biểu diễn Lorentz và phản hạt có spin ngược ([[Lý thuyết trường lượng tử (QFT)]]).

## Liên kết

- [[MOC - Kiến thức Vật lý]]
- [[Thí nghiệm - Stern-Gerlach]]
- [[Toán tử mô-men xung lượng]]
- [[Mômen động lượng quỹ đạo và mômen từ quỹ đạo]]
- [[Hiệu ứng Zeeman]]
- [[Nguyên lý loại trừ Pauli]]

## Câu hỏi mở

- Vì sao hệ số Landé của electron gần với 2 chứ không phải đúng 2 — và câu trả lời QED đến từ chi tiết nào? (Hiệu chỉnh Schwinger $\alpha/2\pi$.)
- Nếu spin biến mất khỏi thế giới (s = 0 cho mọi hạt), những hiện tượng nào sẽ sụp đổ? (Bảng tuần hoàn, liên kết hóa học, từ tính vĩnh cửu, sao neutron...)