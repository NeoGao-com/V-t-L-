---
tags:
  - vật-lý/toán-học
type: toán-học
trạng-thái: ổn-định
created: 2026-09-25
---

# Lượng giác

> [!abstract] Công cụ này dùng để làm gì trong vật lý
> Lượng giác là cầu nối giữa hình học và đại số: nó cho phép chuyển một bài toán hình học (hình học tam giác, đường tròn) thành một biểu thức đại số có thể tính. Ba nơi dùng nhiều nhất: **phân rã vector theo hướng**, **mô tả dao động**, và **diễn đạt chuyển động tròn**.

## Định nghĩa

- Trên đường tròn đơn vị, góc $\theta$ đo bằng **chiều dài cung tương ứng** (bán kính = 1). Từ đó: $\sin\theta$ = tung độ, $\cos\theta$ = hoành độ, $\tan\theta = \dfrac{\sin\theta}{\cos\theta}$.
- **Đơn vị radian:** $2\pi\ \text{rad} = 360^\circ$, $1\ \text{rad} \approx 57{,}3^\circ$. Radian không phải lựa chọn thẩm mỹ — nó là đơn vị **duy nhất** mà các đạo hàm trở nên đơn giản: $\dfrac{d}{d\theta}\sin\theta = \cos\theta$ chỉ đúng khi tính bằng radian (nhân thêm hệ số $\pi/180$ nếu dùng độ).
- Do đó $\omega = \dfrac{\Delta\alpha}{\Delta t}$ trong [[Chuyển động tròn đều]] là tốc độ góc tính bằng radian/s; $f = \omega/2\pi$ là tần số tính bằng vòng/s.

**Đẳng thức nền:**

- $\sin^2\theta + \cos^2\theta = 1$
- Cộng góc: $\sin(\alpha\pm\beta) = \sin\alpha\cos\beta \pm \cos\alpha\sin\beta$; $\cos(\alpha\pm\beta) = \cos\alpha\cos\beta \mp \sin\alpha\sin\beta$
- Nhân đôi: $\sin 2\alpha = 2\sin\alpha\cos\alpha$, $\cos 2\alpha = \cos^2\alpha - \sin^2\alpha = 1 - 2\sin^2\alpha$
- Nửa góc: $\sin\dfrac{\alpha}{2} = \pm\sqrt{\dfrac{1-\cos\alpha}{2}}$, $\cos\dfrac{\alpha}{2} = \pm\sqrt{\dfrac{1+\cos\alpha}{2}}$ — dấu $\pm$ phụ thuộc góc phần tư.
- Tổng → tích: $\cos A + \cos B = 2\cos\dfrac{A+B}{2}\cos\dfrac{A-B}{2}$ — công thức then chốt khi **tổng hợp dao động**.

Giá trị chính xác cần nhớ: $30^\circ \to \tfrac12$, $45^\circ \to \dfrac{\sqrt2}{2}$, $60^\circ \to \dfrac{\sqrt3}{2}$.

## Ý nghĩa vật lý

- **Phân rã thành phần:** trên mặt phẳng nghiêng, $F_{\parallel} = F\cos\alpha$ và $F_{\perp} = F\sin\alpha$ — nền của mọi bài [[Thí nghiệm - Mặt phẳng nghiêng của Galileo]]; cho [[Chuyển động ném]]: $v_{0x} = v_0\cos\alpha$, $v_{0y} = v_0\sin\alpha$.
- **Dao động là hàm lượng giác của thời gian:** $x = A\cos(\omega t + \varphi)$ — biên độ $A$, tần số góc $\omega$, **lệch pha** $\varphi$ xác định trạng thái tại $t=0$ ([[Dao động điều hòa]]).
- **Giao thoa:** điều kiện cực đại là $\Delta d = k\lambda$, cực tiểu là $\Delta d = \left(k+\tfrac12\right)\lambda$ — hiệu đường đi chính là tổng hiệu các đoạn đường, tức tổng các độ lệch pha ([[Giao thoa sóng]]).
- **Quỹ đạo hành tinh và kính lúp:** các định luật Kepler viết bằng lượng giác — quy luật ba định luật, tham khảo [[Quan sát - Chuyển động của các hành tinh]].
- **Kính láp và lăng kính:** góc lệch, góc chiết suất — [[Kính lúp]], [[Lăng kính]].

## Kiến thức vật lý đang sử dụng công cụ này

- [[Vector]]: tích vô hưừng và tích hữu hướng đều viết bằng $\cos\theta$ và $\sin\theta$.
- [[Tổng hợp dao động]]: cộng hai dao động cùng tần số bằng công thức tổng → tích, rồi đọc lại biên độ và pha.
- [[Dòng điện xoay chiều và giá trị hiệu dụng]]: dùng phasor — biến hàm thời gian $\cos(\omega t + \varphi)$ thành số phức cố định theo thời gian.
- [[Con lắc đơn]]: góc lệch nhỏ dẫn tới chuyển động gần đúng là hàm lượng giác.
- [[Sóng dừng]]: các sóng đi và phản chiếu lệch pha $\pi$ vì dấu của phản xạ.

## Liên kết

- [[MOC - Cơ sở Toán học]]
- [[Số phức]] · [[Vector]] · [[Hệ tọa độ]] · [[Định lý Gauss & Stokes]] · [[Chuỗi Taylor & xấp xỉ]]

## Câu hỏi mở

- Vì sao lượng giác hyperbol ($\sinh, \cosh$) lại xuất hiện tự nhiên trong bài toán tốc độ ánh sáng biến thiên theo chiều cao? (Gợi ý: xem [[Thuyết tương đối hẹp]].)
- Nếu dùng **độ** thay vì radian trong công thức $\omega t$, hằng số nào phải xuất hiện? Vì sao điều đó làm công thức xấu đi?
- Tại sao tổng hợp hai dao động lại cần đến công thức "tổng thành tích"? (Gợi ý: nghĩ về việc biểu diễn chúng trong [[Số phức]].)
- Lượng giác cầu giải quyết vấn đề hình học nào mà lượng giác phẳng không giải được? (Gợi ý: xem [[Hệ tọa độ cầu]].)
