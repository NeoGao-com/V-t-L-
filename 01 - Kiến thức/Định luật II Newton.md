---
tags:
  - vật-lý/kiến-thức
type: kiến-thức
domain: cơ-học
category: Vật lý Cổ điển
trạng-thái: ổn-định
created: 2026-09-25
---

# Định luật II Newton

> [!abstract] Ý chính
> Gia tốc của vật tỉ lệ thuận với lực tổng hợp tác dụng và tỉ lệ nghịch với khối lượng: $\vec F = m\vec a$. Dạng tổng quát $\vec F = \dfrac{d\vec p}{dt}$ còn đúng cả khi khối lượng thay đổi (tên lửa).

## Phát biểu & công thức

Trong hệ quy chiếu quán tính:

$\vec F_{\text{tổng hợp}} = m\vec a$

với $F$ là lực tổng hợp (N), $m$ là khối lượng (kg), $\vec a$ là gia tốc (m/s²) — luôn cùng phương, cùng chiều với lực tổng hợp.

Dạng tổng quát (đúng cả khi $m$ thay đổi, ví dụ tên lửa đốt nhiên liệu): $\vec F = \dfrac{d\vec p}{dt}$.

## Bảng: dạng lực → chuyển động kết quả

| Dạng lực | Biểu thức | Chuyển động kết quả | Ví dụ thực tế |
| --- | --- | --- | --- |
| Không đổi | $F = \text{const}$ | Biến đổi đều ($a = \text{const}$) | Rơi tự do, [[Thí nghiệm - Mặt phẳng nghiêng của Galileo]] |
| Đàn hồi | $F = -kx$ | [[Dao động điều hòa]] | [[Con lắc lò xo]] |
| Cản nhớt | $F = -bv$ | Tắt dần, đạt vận tốc tới hạn | Rơi trong chất lỏng ([[Thí nghiệm - Giọt dầu Millikan]]) |
| Hấp dẫn | $F = GMm/r^2$ | Quỹ đạo elip (Kepler) | [[Vệ tinh và tốc độ vũ trụ]], hành tinh |

Một định luật duy nhất tạo ra toàn bộ thư viện chuyển động — mẹo bài tập luôn là: nhận diện **dạng lực** rồi mới viết phương trình.

## Ví dụ vật lý cụ thể

- **Ô tô:** lực kéo $F = 6$ kN, khối lượng 1,5 tấn → $a = 6000/1500 = 4$ m/s². Muốn xe 1.200 kg đạt 100 km/h (27,8 m/s) trong 10 s cần $a = 2{,}78$ m/s² → $F \approx 3{,}3$ kN.
- **Thang máy:** trọng lực tương tác với gia tốc hệ — xem [[Lực quán tính]]; khi tăng tốc lên $a = 2$ m/s², người 70 kg chịu lực sàn $N = m(g+a) \approx 826$ N thay vì 686 N.
- **Tên lửa:** dùng dạng $F = dp/dt$ — lực đẩy $F = \dot m v_{phụt}$; đẩy 50 kg khí/giây với tốc độ 2,5 km/s cho lực đẩy 125 kN.

## Suy luận từ đâu

- **Tiên đề gốc:** định luật thứ hai trong [[Các định luật Newton]] — tiên đề của cơ học cổ điển, không suy ra được, chỉ kiểm chứng bằng thực nghiệm.
- **Công cụ toán:** [[Đạo hàm]] — dạng vi phân $\vec F = m\dfrac{d\vec v}{dt}$; nghiệm thường là [[Phương trình vi phân]].

## Kiểm chứng & giới hạn

- **Tiền đề lịch sử:** [[Thí nghiệm - Mặt phẳng nghiêng của Galileo]] chứng minh vật chuyển động gia tốc đều dưới lực không đổi — bước đệm trực tiếp đến định luật II.
- **Giới hạn:** chỉ đúng khi $v \ll c$ — ở tốc độ cao phải dùng động lượng tương đối tính $\vec p = \gamma m\vec v$ ([[Thuyết tương đối hẹp]]); ở thang nguyên tử, khái niệm "lực" nhường chỗ cho toán tử Hamilton và [[Phương trình Schrödinger]].

## Liên kết

- [[Các định luật Newton]] · [[Đạo hàm]] · [[Thí nghiệm - Mặt phẳng nghiêng của Galileo]] · [[MOC - Kiến thức Vật lý]]
- [[Định luật III Newton]]: lực luôn là cặp — $m\vec a$ của vật này đi kèm phản lực lên vật kia.
- [[Lực quán tính]]: định luật II trong hệ phi quán tính.
- [[Thuyết tương đối hẹp]]: giới hạn tốc độ cao.

## Câu hỏi mở

- Vì sao định luật chỉ đúng trong hệ quy chiếu quán tính? → xem [[MOC - Tiên đề và Nguyên lý]]
- Dạng $\vec F = dp/dt$ đúng cho tên lửa (khối lượng đổi) nhưng $\vec F = m\vec a$ thì sai — ranh giới chính xác nằm ở đâu khi viết phương trình chuyển động?
- Khái niệm "lực" còn là đại lượng cơ bản ở thang lượng tử không, hay chỉ là hệ quả của thế năng trong [[Cơ học Hamilton]]? (Ví dụ: electron trong nguyên tử "chịu lực" gì?)