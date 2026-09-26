---
tags:
  - vật-lý/tiên-đề
type: tiên-đề
domain: điện-từ
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Định luật Ampère về lực từ

> [!abstract] Phát biểu tiên đề
> Hai dây thẳng dài, mang dòng điện $I_1$ và $I_2$, song song cách nhau $khoảng cách $d$, **lực từ trên mỗi đơn vị dài** của mỗi dây có độ lớn:
>
> $\dfrac{F}{L} = \dfrac{\mu_0 I_1 I_2}{2\pi d}$
>
> Dòng điện **cùng chiều** thì hai dây **hút** nhau, **ngược chiều** thì **đẩy** nhau.

## Vì sao đây là tiên đề

- Cùng cấp trúc với [[Định luật Coulomb]] (điện tích tĩnh) và [[Định luật vạn vật hấp dẫn]] (khối lượng): cả ba đều là lực nghịch bình phương khoảng cách. Việc lực từ cũng tuân theo cùng quy luật là bằng chứng mạnh rằng **lực từ không phải là một loại lực riêng biệt** mà là hiệu ứng của trường điện từ.
- Kết hợp với định luật lực Lorentz $d\vec F = I\,d\vec l \times \vec B$, nó là cầu nối giữa [[Điện tích và bảo toàn điện tích]] và [[Từ trường và cảm ứng từ]]: *dòng điện* là nguồn của *từ trường*.
- Mức độ độc lập: đây là phương trình thứ tư của [[Phương trình Maxwell]] (dạng tích phân của phương trình Ampère–Maxwell), nên về mặt hệ quả nó **không độc lập** với bốn phương trình Maxwell. Tuy nhiên với dòng điện **tĩnh**, nó đóng vai trò một định luật thực nghiệm gốc, đứng cùng cấp với định luật lực tĩnh điện.

## Bằng chứng ủng hộ (thực nghiệm / quan sát)

- **Oersted (1820):** dòng điện làm lệch kim nam châm — lần đầu chứng minh từ trường có nguồn gốc điện. Ampère lập tức phát triển thành định luật lực (1820–1826).
- **Thí nghiệm dây song song:** hai dây cùng chiều hút, ngược chiều đẩy — quan sát được trực tiếp với hai dây mềm treo song song, và dùng cơ để đo lực hút cảm ứng.
- **Định nghĩa ampe (SI, 2019):** hệ SI được định nghĩa lại quanh hằng số hằng, còn ampe vẫn là đơn vị cơ sở gắn với dòng điện, nên mối liên hệ giữa dòng điện và từ trường là chỗ bám hiệu chuẩn tuyệt đối của SI.
- **Động cơ và nam châm:** lực từ giữ hai cuộn dây đối diện là cơ chế cơ bản của [[Máy phát điện xoay chiều]] và mọi máy điện.

## Nhánh kiến thức xây trên nó

- **Từ trường do dòng điện sinh ra:**
  - Dây thẳng vô hạn: $B = \dfrac{\mu_0 I}{2\pi r}$ tại khoảng cách $r$.
  - Vòng tròn bán kính $R$, tại tâm: $B = \dfrac{\mu_0 I}{2R}$.
- **Mô-men lực từ** trên vòng dây trong từ trường đều: $\tau = IAB = I\pi R^2 B$, dẫn tới nguyên lý cực đại nhỏ nhất của từ thông trong nam châm.
- **Định luật Ampère (dạng tích phân):** $\displaystyle\oint \vec B\cdot d\vec l = \mu_0 I_{\text{trong}}$ — chỉ dùng được khi đối xứng cho phép, cùng kỹ thuật với [[Định lý Gauss & Stokes]] và [[Định luật Gauss (điện)]].
- Dùng để tính từ trường của cuộn dây, [[Tụ điện]], mạch song song trong [[Mạch điện và các phần tử mạch]].

## Giới hạn

- Phép so sánh "định luật Ampère" với "định luật Ampère–Maxwell" là nguồn nhầm lẫn phổ biến: bản gốc của Ampère (1826) **không** có dòng điện dịch và **không** mô tả được trường điện từ. Sự phân biệt này là chính [[Định luật Faraday về cảm ứng điện từ]] đòi hỏi.
- Phần dẫn xuất từ hình học dây thẳng giả định dây **dài vô hạn**; dây thực tế cần xét cả đầu dây.

## Liên kết

- [[MOC - Tiên đề và Nguyên lý]]
- [[Phương trình Maxwell]]
- [[Định luật Coulomb]] · [[Định luật vạn vật hấp dẫn]] · [[Định luật Faraday về cảm ứng điện từ]] · [[Định luật Gauss (điện)]]
- [[Từ trường và cảm ứng từ]] · [[Điện từ trường]] · [[Lực Lorentz]]
- [[Điện tích và bảo toàn điện tích]] · [[Dòng điện và cường độ dòng điện]]
- [[Máy phát điện xoay chiều]] · [[Mạch điện và các phần tử mạch]] · [[Tụ điện]]
- [[Định lý Gauss & Stokes]] · [[Sóng điện từ và thang sóng điện từ]]

## Câu hỏi mở

- Vì sao lực từ giữa hai dây tuân theo nghịch bình phương khoảng cách, khi dòng điện lại là nguồn trường "tĩnh" — điều đó có được giải thích thuần từ cấu trúc trường không?
- Trường từ của một dòng điện thật sự khác gì so với trường của hai "cặp điện tích" chuyển động?