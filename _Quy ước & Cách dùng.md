---
tags:
  - vật-lý/moc
type: moc
created: 2026-09-25
---

# Quy ước & Cách dùng

> [!info] Đọc một lần, dùng mãi
> Note này quy định "luật chơi" để bộ não lớn lên mạch lạc thay vì thành bãi rác thông tin.

## Cấu trúc thư mục

```
Vật lý/
├── Não bộ Vật lý.md              ← trung tâm, bắt đầu từ đây
├── _Quy ước & Cách dùng.md       ← note này
├── 01 - Kiến thức/               ← khái niệm, định luật dẫn xuất
├── 02 - Tiên đề và Nguyên lý/    ← nền móng, điểm xuất phát
├── 03 - Cơ sở Toán học/          ← công cụ toán
├── 04 - Giả thuyết và Thực nghiệm/
├── 05 - Nhà khoa học và Lịch sử/ ← con người + mạch hình thành kiến thức
└── _Templates/                   ← mẫu tạo note nhanh
```

## Quy tắc đặt tên

- **Kiến thức:** tên khái niệm, ví dụ `Định luật II Newton`.
- **Tiên đề:** tên định luật/nguyên lý nền, ví dụ `Các định luật Newton`.
- **Toán học:** tên công cụ, ví dụ `Đạo hàm`.
- **Thực nghiệm:** tiền tố loại + tên, ví dụ `Thí nghiệm - Mặt phẳng nghiêng của Galileo`, `Giả thuyết - Vật nặng rơi nhanh hơn`.
- **Nhân vật:** tên đầy đủ (`Albert Einstein`); cặp cùng một thí nghiệm viết chung (`Otto Stern và Walther Gerlach`).
- **Lịch sử:** tiền tố `Lịch sử hình thành`, ví dụ `Lịch sử hình thành cơ học lượng tử`.
- **MOC:** tiền tố `MOC -`, đặt đầu thư mục của trụ cột.

## Quy tắc liên kết

- Luôn liên kết note mới về **MOC của trụ cột** và **ít nhất 2 note khác**.
- Liên kết chéo 4 trụ cột theo bộ ba quen thuộc: *kiến thức → tiên đề → công cụ toán*, và *kiến thức ↔ thực nghiệm*.
- Không sợ liên kết đỏ — chúng chính là danh sách việc cần làm tiếp theo.

## Từ điển thuộc tính (properties)

| Thuộc tính   | Ý nghĩa                     | Giá trị                                                                                                                                                                    |
| ------------ | --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `tags`       | Trụ cột của note            | `vật-lý/kiến-thức`, `vật-lý/tiên-đề`, `vật-lý/toán-học`, `vật-lý/thực-nghiệm`, `vật-lý/nhân-vật`, `vật-lý/lịch-sử`, `vật-lý/moc`, `vật-lý/lộ-trình`, `vật-lý/công-cụ` |
| `type`       | Loại note                   | `kiến-thức`, `tiên-đề`, `toán-học`, `thực-nghiệm`, `nhân-vật`, `lịch-sử`, `moc`, `lộ-trình`, `công-cụ` |
| `domain`     | Phân ngành vật lý           | 11 giá trị chuẩn: `cơ-học`, `nhiệt-học`, `dao-động-sóng`, `điện-từ`, `điện-tử`, `quang-học`, `điện-kỹ-thuật`, `hạt-lý`, `lượng-tử`, `tương-đối`, `xác-suất`             |
| `loại`       | Dạng note thực nghiệm       | `thí-nghiệm`, `giả-thuyết`, `quan-sát`                                                                                                                                     |
| `trạng-thái` | Độ chín của note            | `mầm`, `đang-phát-triển`, `ổn-định`                                                                                                                                        |
| `created`    | Ngày tạo (template tự điền) | `YYYY-MM-DD`                                                                                                                                                               |

**Quy tắc áp dụng `domain`:**

- **Bắt buộc** với `kiến-thức` (template đã có `domain: phải-điền`).
- **Khuyến khích** với `tiên-đề` và `thực-nghiệm` — gán theo lĩnh vực nội dung (vd: thí nghiệm Hertz → `điện-từ`, giả thuyết de Broglie → `lượng-tử`).
- **Không dùng** với `toán-học` (công cụ xuyên ngành), `moc`, `lộ-trình`, `công-cụ`; với `nhân-vật` và `lịch-sử` thì **bắt buộc** — gán theo lĩnh vực đóng góp chính (vd: Einstein → `tương-đối`, Stern-Gerlach → `lượng-tử`, mạch dao động/sóng → `dao-động-sóng`). Dashboard sẽ tự cờ note thiếu domain.
- Giá trị domain chỉ được lấy trong danh sách 11 chuẩn ở trên — tự đặt giá trị mới là vi phạm.
- `trạng-thái` chỉ dùng cho 6 type nội dung (`kiến-thức`, `tiên-đề`, `toán-học`, `thực-nghiệm`, `nhân-vật`, `lịch-sử`); các type định hướng (`moc`, `lộ-trình`, `công-cụ`) không mang trạng thái.

## Quy tắc ghi nguồn

- **Không dùng property `nguồn`** — ghi nguồn ngay trong note, tại dòng `Ý chính` hoặc `Kiểm chứng & giới hạn`, khi note trích một phát biểu/tư liệu cụ thể.
- Cách viết gọn: `(Ferraris, 1885)`, `(Vật lý đại cương, Hà Nội 2008)` hoặc đường dẫn bài viết, đặt ngay sau câu.
- Mục đích: khi đọc lại, biết đi đâu để đào sâu hay kiểm chứng. Vault này là bộ não học tập, không phải thư viện trích dẫn.

## Vòng đời một note

1. **mầm** — mới gieo, có thể chỉ là tiêu đề + 1–2 dòng.
2. **đang-phát-triển** — đã có nội dung chính và liên kết đầy đủ.
3. **ổn-định** — nội dung chắc chắn; còn bổ sung thì sửa, không viết lại.

## Mẹo vận hành

- **Bãi ươm:** ý mới chưa đủ chất viết 1–2 dòng vào [[Bãi ươm]] thay vì tạo note vội; khi chín, tạo note thật và xóa dòng.
- **Graph View:** lọc theo tag `vật-lý/...` để xem riêng từng trụ cột hoặc toàn bộ bộ não.
- **Bases dashboard:** mở [[Bases - Dashboard Vật lý.base]] để nhìn toàn cảnh vault theo trụ/domain/trạng thái; nhúng view vào note nào cũng được bằng `![[Bases - Dashboard Vật lý.base#View]]`. Ý nghĩa 3 view "cảnh báo": `Cần chăm` = note đang ở `mầm`/`đang-phát-triển` (radar việc nên chăm hôm nay — rỗng nghĩa là mọi nội dung đã ổn-định); `Thiếu domain` = note thuộc trụ nội dung chưa có domain hợp lệ; `Mồ côi` = note chưa ai link tới (dựa trên `file.backlinks` — có thể trễ nhịp). View `Mới gieo` = 30 note mới nhất trong vòng 30 ngày (radar review tuần).
- **Tìm nhanh:** `Ctrl+O` tìm theo tên note; `Ctrl+Shift+F` tìm theo nội dung.

> [!info] Bases là core plugin — đã bật sẵn
> Bases là core plugin của Obsidian (không phải plugin cộng đồng) và đã bật trong vault này (`.obsidian/core-plugins.json` → `bases: true`). Mở [[Bases - Dashboard Vật lý.base]] là dùng được ngay; bật/tắt tại **Settings → Core plugins → Bases**.