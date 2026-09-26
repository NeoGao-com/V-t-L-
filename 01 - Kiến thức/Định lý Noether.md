---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: cơ-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Định lý Noether

> [!abstract] Ý chính
> Mỗi đối xứng liên tục của tác dụng sẽ tương ứng với một đại lượng bảo toàn — cầu nối sâu sắc giữa đối xứng và các định luật bảo toàn cơ bản của vật lý. "Bảo toàn" không phải điều ngẫu nhiên của từng bài toán, mà là chữ ký của cấu trúc đối xứng của tự nhiên.

## Nội dung

- **Cốt lõi:** nếu hệ không đổi dưới một phép biến đổi liên tục (đối xứng của tác dụng $S = \int L\,dt$), thì tồn tại một đại lượng bảo toàn tương ứng — biểu diễn bởi phương trình $\dfrac{dQ}{dt} = 0$ với $Q$ là **sinh** (generator) của phép biến đổi.
- **Ba cặp điển hình:**
  - **Dịch chuyển thời gian** → **Bảo toàn năng lượng** ($E = \text{const}$).
  - **Dịch chuyển không gian** → **Bảo toàn động lượng** ($\vec P = \text{const}$).
  - **Quay hệ tọa độ** → **Bảo toàn mô-men động lượng** ($\vec L = \text{const}$).
- **Chiều ngược lại cũng đúng (định lý Noether đảo):** mỗi lượng bảo toàn tương ứng một đối xứng — dùng để *dò tìm* cấu trúc ẩn của lý thuyết.

## Ý nghĩa vật lý

- Các [[Nguyên lý bảo toàn năng lượng]] và [[Nguyên lý bảo toàn động lượng]] hóa ra là **một** nguyên lý duy nhất nhìn qua hai đối xứng khác nhau — không phải ba định luật riêng rẽ.
- Nói "đối xứng sinh bảo toàn" còn mạnh hơn cả việc tính toán: ta có thể *dự đoán* lượng bảo toàn chỉ bằng cách nhìn vào Lagrangian có phụ thuộc gì không ([[Cơ học Lagrange]]).
- Trong [[Lý thuyết nhóm]]: mỗi tham số liên tục của nhóm đối xứng (góc quay, độ dịch, pha gauge) là một "kim la bàn" ứng với một lượng bảo toàn — nền tảng của cách xây dựng [[Mô hình chuẩn (Standard Model)]].
- **Giới hạn:** chỉ áp dụng cho đối xứng **liên tục**; đối xứng rời rạc (đảo ngược thời gian, gương) không sinh lượng bảo toàn kiểu Noether.

## Liên kết

- [[MOC - Kiến thức Vật lý]] · [[MOC - Cơ sở Toán học]]
- [[Nguyên lý bảo toàn năng lượng]]: áp dụng trực tiếp cho đối xứng dịch chuyển thời gian.
- [[Nguyên lý bảo toàn động lượng]]: đối xứng dịch chuyển không gian.
- [[Cơ học Lagrange]]: khung tác dụng – đối xứng – bảo toàn.
- [[Lý thuyết nhóm]]: đối xứng liên tục được mô tả bằng nhóm Lie.
- [[Mô hình chuẩn (Standard Model)]]: các nhóm gauge và lượng bảo toàn tương ứng.

## Câu hỏi mở

- Đối xứng *rời rạc* (gương, đảo chiều thời gian) không sinh lượng bảo toàn — vậy chúng sinh ra gì? (Gợi ý: số lượng tử như parity, và các định luật bất biến dạng khác.)
- Khi đối xứng bị **phá vỡ tự phát**, lượng bảo toàn "mất" đi thế nào, và điều gì còn sót lại? (Gợi ý: định lý Goldstone, cơ chế Higgs.)