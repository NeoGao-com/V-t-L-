---
tags:
  - vật-lý/tiên-đề
type: tiên-đề
domain: điện-kỹ-thuật
category: Vật lý Ứng dụng & Liên ngành
trạng-thái: ổn-định
created: 2026-09-25
---

# Định luật Kirchhoff

> [!abstract] Phát biểu tiên đề
> Hai định luật "hiến pháp" của lý thuyết mạch, là hệ quả trực tiếp của hai nguyên lý bảo toàn:
>
> - **Định luật nút (KCL):** tổng dòng điện vào một nút bằng tổng dòng điện ra — điện tích không tích tụ tại nút, xem [[Điện tích và bảo toàn điện tích]].
> - **Định luật vòng (KVL):** tổng đại số hiệu điện thế quanh một vòng kín bằng 0 — năng lượng bảo toàn, điện thế là hàm đơn trị, xem [[Điện thế và hiệu điện thế]].

## Vì sao đây là tiên đề

- **Quan trọng về mặt kỹ thuật hơn là tiên đề vật lý:** đây là hai phương trình ràng buộc cơ bản của **mọi** mạch điện, được cài đặt trực tiếp vào phần mềm mô phỏng.
- **Mức độ độc lập: đây là định luật hệ quả, không phải tiên đề gốc.** KCL là hình thức mạch của bảo toàn điện tích; KVL là hình thức mạch của [[Nguyên lý bảo toàn năng lượng]]. Nó được giữ trong trụ này vì thực tế dạy như một trong những "tiên đề" cơ bản của mạch — đọc MOC sẽ thấy nó được xếp ở nhóm định luật hệ quả.
- Suy ra được từ giới hạn tĩnh của [[Phương trình Maxwell]]: khi kích thước mạch nhỏ so với bước sóng, trường coi như **thông số tập trung** → dòng chỉ chảy trong dây, điện áp tồn tại ở hai đầu phần tử.

## Bằng chứng ủng hộ (thực nghiệm / quan sát)

- Mọi phép đo mạch điện trên thực tế đều tuân theo KCL và KVL; sai lệch quan sát được luôn thuộc về **sai lầm đo** hoặc **mô hình xấp xỉ sai**, không phải ngoại lệ của định luật.
- Kirchhoff đã dùng chúng để tính **cầu cân bằng Wheatstone** (1847) — một trong những ứng dụng mô hình mạch đầu tiên, kết quả khớp thực nghiệm đo cân bằng nhánh cầu.
- Trong mô hình mạch tuyến tính: $N_{nút} - 1$ phương trình KCL cộng $N_{vòng}$ phương trình KVL cho **hệ thống nghiệm duy nhất** — đây là lý do phương pháp không còn ngẫu nhiên, mọi nghiệm đều tính được.

## Nhánh kiến thức xây trên nó

- Phương pháp giải mạch: phương pháp mạch nhánh, phương pháp nút trọng tâm, phương pháp nguồn tương đương, định lý Thevenin/Norton.
- Mạch AC: trở kháng, phức số, công suất phản kháng.
- Tầng dưới của [[Mạch điện và các phần tử mạch]].

## Liên kết

- [[MOC - Tiên đề và Nguyên lý]]
- [[Điện tích và bảo toàn điện tích]]
- [[Nguyên lý bảo toàn năng lượng]]
- [[Điện thế và hiệu điện thế]]
- [[Mạch điện và các phần tử mạch]]
- [[Phương trình Maxwell]]
- [[Sóng điện từ và thang sóng điện từ]]

## Câu hỏi mở

- Tần số nào làm mô hình thông số tập trung mất hiệu lực, và khi đó cần bổ sung phần tử phân bố nào?
- KVL còn đúng không khi mạch chứa tụ điện/điện cảm với điện trường biến thiên theo thời gian?
