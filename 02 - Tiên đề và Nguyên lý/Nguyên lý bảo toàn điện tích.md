---
tags:
  - vật-lý/tiên-đề
type: tiên-đề
domain: điện-từ
trạng-thái: đang-phát-triển
created: 2026-09-26
---

# Nguyên lý bảo toàn điện tích

> [!abstract] Phát biểu tiên đề
> **Tổng đại số điện tích của một hệ kín là hằng số theo thời gian.** Tương đương ở dạng vi phân: phương trình liên tục
>
> $\nabla\cdot\vec J + \dfrac{\partial \rho}{\partial t} = 0$
>
> Tức **dòng điện vào một vùng bằng dòng điện ra cộng với tốc độ tích tụ điện tích bên trong vùng đó**.

## Vì sao đây là tiên đề

- Đây là nguyên lý bảo toàn **duy nhất** không suy ra được từ cơ học: nó thuộc về cấu trúc của tự nhiên, không phải hệ quả của chuyển động.
- Nó **không độc lập** với hệ Maxwell: lấy phép phân rã phương trình Ampère–Maxwell và dùng $\nabla\cdot(\nabla\times\vec B) = 0$ là thu được ngay phương trình liên tục. Nói cách khác, bảo toàn điện tích là **nội dung ẩn** của cặp phương trình Maxwell.
- Nó **tương đương** với đối xứng gauge $U(1)$ theo [[Định lý Noether]] — nằm ở tầng sâu hơn mọi định luật thực nghiệm về điện.
- Hệ quả thực tiễn: dòng điện tĩnh chỉ tồn tại trong **mạch kín**. Không có "đầu dây tích điện" trong mạch DC — đó là hệ quả trực tiếp của nguyên lý này.

## Bằng chứng ủng hộ (thực nghiệm / quan sát)

- **Thí nghiệm tĩnh điện Faraday:** nạp điện bình, cân đối trên cân điện, đặt trong điện trường — trọng lượng đo được **không đổi** qua mọi thao tác.
- **Chính điện luật phân rã (Faraday, 1833–1834):** các tỉ lệ khối lượng các nguyên tố được giải thích bằng sự bảo toàn điện tích khi tạo ion trong dung dịch — bằng chứng định lượng sớm nhất.
- **Millikan:** đo điện tích nguyên tố $e \approx 1{,}602\times10^{-19}$ C, và mọi điện tích quan sát được đều là **bội nguyên** của $e$ — xem [[Thí nghiệm - Giọt dầu Millikan]].
- **Thí nghiệm tĩnh điện hiện đại (chùm electron ổn định):** bằng chứng trực tiếp nhất cho cả tính lượng tử hoá lẫn bảo toàn điện tích.
- **Va chạm hạt:** trong mọi va chạm đã ghi nhận, tổng điện tích trước và sau luôn bằng 0 — kể cả khi sinh hạt mới, và cả khi tạo cặp hạt–phản hạt.

## Nhánh kiến thức xây trên nó

- **Mạch điện:** định luật nút KCL là hình thức mạch của nguyên lý này → [[Định luật Kirchhoff]]; dòng điện là tốc độ chuyển điện tích qua tiết diện → [[Dòng điện và cường độ dòng điện]].
- **Điện từ:** phương trình liên tục là ràng buộc lên mọi nguồn trường trong [[Phương trình Maxwell]]; phần "trong" là [[Định luật Gauss (điện)]].
- **Hạt nhân và hạt:** bảo toàn điện tích là ràng buộc cứng nhất khi gán nhãn các hạt; phân rã $\beta$ và phản vận hạt chỉ sinh ra được vì tổng điện tích phải bằng 0.
- **Vật lý lý thuyết:** trong [[Lý thuyết trường lượng tử (QFT)]], bảo toàn điện tích được bảo đảm bởi bất biến gauge.

## Giới hạn

- **Bảo toàn điện tích không suy ra được lượng tử hoá điện tích.** Hai điều này độc lập nhau: nguyên lý bảo toàn chỉ nói tổng điện tích không đổi, còn việc điện tích chỉ nhận giá trị là bội số nguyên của $e$ là một **quan sát thực nghiệm** (và trong lý thuyết trường nó còn liên quan tới lực lượng gauge tương tác).
- Nguyên lý này phạm vi hẹp ở chỗ nó gắn với **điện tích điện**, không bao gồm các "đại lượng bảo toàn" khác như baryon hay lepton — xem [[Nguyên lý bảo toàn số khối]].

## Liên kết

- [[MOC - Tiên đề và Nguyên lý]]
- [[Điện tích và bảo toàn điện tích]]: khái niệm điện tích và lượng tử hoá
- [[Phương trình Maxwell]] · [[Định luật Gauss (điện)]] · [[Định luật Kirchhoff]]
- [[Dòng điện và cường độ dòng điện]] · [[Điện trường]] · [[Điện từ trường]]
- [[Thí nghiệm - Giọt dầu Millikan]] · [[Nguyên lý bảo toàn số khối]]
- [[Định lý Noether]] · [[Lý thuyết trường lượng tử (QFT)]]

## Câu hỏi mở

- Vì sao lượng tử hoá điện tích lại xuất hiện từ $\exp(i q\theta/\hbar)$ với $\theta$ là góc toàn cục — tức cấu trúc toạ độ đã áp đặt mức lượng tử hoá lên điện tích chưa?
- Trong thuyết trường, nếu bảo toàn điện tích là hệ quả của gauge, thì điều gì xảy ra nếu ta chọn một lực lượng gauge khác?
- Có thể phân rã trung tính bảo toàn hay không? (Phân rã $\beta$ hai thành phần là bằng chứng mạnh cho tính bất khả xâm phạm của điện tích.)