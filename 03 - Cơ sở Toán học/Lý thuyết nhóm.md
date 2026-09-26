---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Lý thuyết nhóm

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Ngôn ngữ toán của đối xứng: nhóm mô tả các phép biến đổi giữ nguyên cấu trúc của hệ — đối xứng liên tục kéo theo định luật bảo toàn ([[Định lý Noether]]), còn đối xứng gauge xây dựng nên các tương tác cơ bản của [[Mô hình chuẩn (Standard Model)]].

## Định nghĩa

- **Nhóm:** tập $G$ với phép toán $\circ$ thỏa bốn tiên đề: kín, kết hợp, có phần tử đơn vị, mọi phần tử có nghịch đảo.
- **Nhóm Lie:** nhóm liên tục (ví dụ phép quay $SO(3)$) — cấu trúc địa phương quy về **đại số Lie** (các vector sinh, "sinh" ra mọi phép biến đổi của nhóm qua phép lũy thừa ma trận $e^{i\theta T}$).
- **Biểu diễn:** ánh xạ từ nhóm vào ma trận tác dụng lên không gian vector — trạng thái lượng tử "sống" trong các biểu diễn bất khả quy của nhóm đối xứng.

## Ý nghĩa hình học

- Nhóm là "sách hướng dẫn" các phép biến đổi không làm đổi hình: xoay bông tuyết $60^\circ$ giữ nguyên hình — tập mọi phép quay như vậy lập thành nhóm đối xứng của hình.
- Nhóm Lie liên tục như "xoay dần dần": mỗi tham số liên tục (góc quay, độ dịch) là một "kim la bàn" sinh ra toàn bộ nhóm — trực giác quan trọng để nối với [[Định lý Noether]] (mỗi kim la bàn = một lượng bảo toàn).

## Ý nghĩa vật lý

- **Đối xứng không-thời gian:** dịch chuyển → bảo toàn động lượng; quay → bảo toàn mô-men động lượng; dịch thời gian → bảo toàn năng lượng (hệ quả của [[Định lý Noether]], liên hệ [[Nguyên lý bảo toàn năng lượng]], [[Nguyên lý bảo toàn động lượng]]).
- **Đối xứng gauge trong [[Mô hình chuẩn (Standard Model)]]:** $U(1)$ (điện từ), $SU(2)$ (tương tác yếu), $SU(3)$ (tương tác mạnh) — mỗi nhóm sinh ra trường lực tương ứng; cấu trúc nhóm quyết định số hạt truyền tương tác và cách chúng "trộn".
- **Cơ học lượng tử:** phép biến đổi đối xứng được biểu diễn bởi toán tử unita; phân loại trạng thái theo các biểu diễn (spin từ $SU(2)$, hạt ↔ phản hạt).
- **Đối xứng hoán vị:** đổi chỗ hai hạt đồng nhất là một phép đối xứng → chỉ có hai loại biểu diễn (đối xứng/bất đối xứng) ứng với boson/fermion — nguồn gốc [[Nguyên lý loại trừ Pauli]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Đại số tuyến tính]] — nền tảng của biểu diễn ma trận.
- [[Mô hình chuẩn (Standard Model)]] — gauge symmetry của ba tương tác cơ bản.
- [[Định lý Noether]] · [[Nguyên lý bảo toàn năng lượng]] · [[Nguyên lý bảo toàn động lượng]] — đối xứng và bảo toàn.
- [[Cơ học Lagrange]] — dạng Lagrangian bất biến dưới nhóm đối xứng.
- [[Nguyên lý loại trừ Pauli]] — thống kê hạt từ nhóm hoán vị.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Đại số tuyến tính]] · [[Định lý Noether]] · [[Mô hình chuẩn (Standard Model)]] · [[Nguyên lý bảo toàn năng lượng]] · [[Nguyên lý loại trừ Pauli]] · [[Cơ học Lagrange]]

## Câu hỏi mở

- Vì sao các nhóm gauge của mô hình chuẩn lại đúng là $U(1) \times SU(2) \times SU(3)$? (Không có nguyên lý tiên nghiệm bắt buộc — một trong những câu hỏi mở trung tâm của vật lý cơ bản.)
- Đối xứng bị **phá vỡ tự phát** (cơ chế Higgs) khác gì đối xứng bị phá vỡ tường minh, và vì sao điều đó lại sinh ra khối lượng? ([[Mô hình chuẩn (Standard Model)]])