---
tags:
  - vật-lý/tiên-đề
type: tiên-đề
domain: cơ-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Nguyên lý tác dụng tối thiểu

> [!abstract] Phát biểu tiên đề
> Tự nhiên không chọn quỹ đạo cụ thể, mà chọn **con đường làm cực trị của hàm tác dụng** $S = \displaystyle\int_{t_1}^{t_2} L\,dt$ trong không gian cấu hình. Đây là một nguyên lý thống nhất toàn vật lý: từ đường thẳng ngắn nhất, định luật khúc xạ, cơ học Newton, cho tới quỹ đạo trong không–thời gian cong và hình thức luận lượng tử.

## Vì sao đây là tiên đề

- Đây là **tầng sâu hơn cả định luật Newton**: chọn $L = T - V$ thì phương trình Euler–Lagrange $\dfrac{\partial L}{\partial q} - \dfrac{d}{dt}\dfrac{\partial L}{\partial \dot q} = 0$ tự tái tạo $\vec F = m\vec a$. Tức là toàn bộ cơ học Newton là hệ quả của nguyên lý này, không phải ngược lại.
- Nó trả lời câu hỏi mà các định luật lực không trả lời được: **tại sao các định luật tự nhiên lại có dạng như vậy** — vì chúng đều là phương trình Euler–Lagrange của một tác dụng nào đó.
- Nó **thống nhất nhiều lĩnh vực** bằng cùng một công thức, nên được xem là một trong những nguyên lý nền sâu nhất của vật lý.

## Bằng chứng ủng hộ (thực nghiệm / quan sát)

- **Toàn bộ cơ học cổ điển** là hệ quả trực tiếp: mọi bài toán cơ học giải được bằng Euler–Lagrange đều khớp với lời giải Newton.
- **Con lắc đơn:** với $L = T - V = \frac{1}{2}ml^2\dot\theta^2 - mgl(1-\cos\theta)$, Euler–Lagrange cho $\ddot\theta + \dfrac{g}{l}\sin\theta = 0$ → chu kỳ dao động nhỏ $\omega = \sqrt{g/l}$, đúng như kết quả trực tiếp từ [[Các định luật Newton]] và khớp thực nghiệm của [[Con lắc đơn]].
- **Quỹ đạo hành tinh trong thuyết tương đối rộng:** trắc địa từ cực trị thời gian riêng tái tạo đúng sai số tiến độ quỹ đạo cành Kim tinh quan sát bằng kính viễn thông — bằng chứng thực nghiệm mạnh nhất của nguyên lý ngoài cơ học.
- **Khúc xạ:** tác dụng cùng dạng với [[Nguyên lý Fermat]] sinh ra định luật Snell, khớp thực nghiệm.

## Nhánh kiến thức xây trên nó

| Lĩnh vực | "Tác dụng" cực trị | Kết quả |
| --- | --- | --- |
| Hình học | $S = \int ds$ (độ dài) | Trắc địa: đường thẳng trong không gian phẳng |
| Quang học | Thời gian truyền | Định luật khúc xạ Snell, phản xạ |
| Cơ học cổ điển | $S = \int (T - V)\,dt$ | $\vec F = m\vec a$ của [[Các định luật Newton]] |
| Tương đối rộng | $S = \int ds$ (thời gian riêng) | Trắc địa: quỹ đạo rơi tự do — [[Thuyết tương đối rộng]] |
| Cơ học lượng tử | Pha đường đi $e^{iS/\hbar}$ | Mọi đường đi đều đóng góp — hình thức luận Feynman |

- [[Cơ học Lagrange]] và [[Cơ học Hamilton]]: hai hình thức luận suy ra từ tác dụng.
- [[Phép tính biến phân]]: toán học của bài toán cực trị.
- [[Định lý Noether]]: mỗi đối xứng của tác dụng sinh ra một đại lượng bảo toàn.

## Liên kết

- [[MOC - Tiên đề và Nguyên lý]]
- [[Phép tính biến phân]]
- [[Định lý Noether]]
- [[Nguyên lý Fermat]]
- [[Nguyên lý bảo toàn năng lượng]]
- [[Nguyên lý bảo toàn động lượng]]
- [[Các định luật Newton]]
- [[Cơ học Lagrange]] · [[Cơ học Hamilton]]
- [[Con lắc đơn]]
- [[Thuyết tương đối rộng]]

## Câu hỏi mở

- Vì sao tự nhiên "tối ưu hoá một con đường" — tại sao định luật dạng cực trị lại tương đương với định luật lực địa phương?
- Ở thang lượng tử, mọi đường đi đều đóng góp pha $e^{iS/\hbar}$ — vì sao giới hạn cổ điển $\hbar \to 0$ chỉ để lại đường cực trị?
- Nếu tìm được hiện tượng **không** diễn tả được bằng tác dụng, vật lý còn đúng không?