<p align="center">
  <a href="https://strikeos.site">
    <img src="./strike-logo.png" alt="SuperStrike X1" width="760">
  </a>
</p>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/VERSION-1.0.0-5B21FF?style=for-the-badge">
  <img alt="Windows" src="https://img.shields.io/badge/WINDOWS-10%20%7C%2011-0078D4?style=for-the-badge">
  <img alt="AME Playbook" src="https://img.shields.io/badge/AME-PLAYBOOK-202020?style=for-the-badge">
  <img alt="Defender retained" src="https://img.shields.io/badge/DEFENDER-RETAINED-16A34A?style=for-the-badge">
  <a href="./LICENSE"><img alt="License details" src="https://img.shields.io/badge/LICENSE-DETAILS-4B5563?style=for-the-badge"></a>
</p>

<p align="center">
  <img alt="Supported builds" src="https://img.shields.io/badge/BUILD-19045%20%7C%2026100%20%7C%2026200-2563EB?style=flat-square">
  <img alt="Architecture" src="https://img.shields.io/badge/ARCH-x64-6D28D9?style=flat-square">
  <img alt="Profiles" src="https://img.shields.io/badge/PROFILES-STANDARD%20%7C%20PERFORMANCE-E11D48?style=flat-square">
  <img alt="Revision" src="https://img.shields.io/badge/REV-PERFORMANCE12--VI-2563EB?style=flat-square">
  <img alt="Status" src="https://img.shields.io/badge/STATUS-TEST-F59E0B?style=flat-square">
</p>

<p align="center"><strong>Playbook tinh gọn Windows hiệu năng cao, tối ưu hóa độ ổn định cho phần cứng.</strong></p>

<p align="center">
  <a href="https://strikeos.site">Website</a> ·
  <a href="https://discord.gg/strikeos">Discord</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/releases">Releases</a> ·
  <a href="#cài-đặt">Cài đặt</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/issues">Báo lỗi</a>
</p>

---

## Giới thiệu

**SuperStrike X1** là AME Playbook tinh gọn trực tiếp trên Windows hiện tại mà không cần cài lại Windows. Dự án tập trung loại bỏ bloatware, tắt telemetry và Processes chạy ngầm, duy trì frametime phẳng đều và giải phóng tối đa tài nguyên phần cứng.

* **Phiên bản:** `1.0.0`
* **Triết lý:** Ưu tiên frametime và độ bền bỉ dài hạn, loại bỏ rác ngầm nhưng giữ nguyên tính toàn vẹn của Windows...

---

## ⚠️ Cảnh báo & Miễn trừ trách nhiệm

> [!WARNING]
> Playbook can thiệp sâu vào nhân hệ điều hành. **Yêu cầu sao lưu dữ liệu toàn vẹn trước khi chạy** (Restore Point không thể thay thế bản sao lưu gốc). Playbook không tự sao lưu và chưa hỗ trợ hoàn tác (undo) toàn bộ.

- **Không cam kết tuyệt đối:** FPS, RAM, số lượng Processes và độ tương thích (driver, game, anti-cheat) phụ thuộc vào phần cứng thực tế của bạn. Đây là phiên bản thử nghiệm.
- **Giới hạn môi trường:** TUYỆT ĐỐI KHÔNG dùng cho máy chủ, máy tính doanh nghiệp (Domain/MDM) hoặc các bản Windows đã bị chỉnh sửa bởi bên thứ ba (modded OS).
- **Miễn trừ trách nhiệm:** Người dùng hoàn toàn tự chịu trách nhiệm khi quyết định áp dụng Playbook. StrikeOS được miễn trừ mọi trách nhiệm pháp lý đối với các lỗi phát sinh, xung đột phần mềm hoặc mất mát dữ liệu.
- **Bảo mật nguồn tải:** Chỉ sử dụng file tải trực tiếp từ [strikeos.site](https://strikeos.site) và kiểm tra đúng checksum SHA256. Ngừng chạy ngay lập tức nếu mã hash không khớp hoặc file có dấu hiệu bị can thiệp.

---

## Khả năng tương thích

Kiểm tra bằng lệnh `winver` trước khi chạy. Playbook chỉ hỗ trợ các build x64 sau:

| Hệ điều hành | Phiên bản | Build hỗ trợ |
| :--- | :---: | :---: |
| **Windows 10** | 22H2 | `19045` |
| **Windows 11** | 24H2 | `26100` |
| **Windows 11** | 25H2 | `26200` |

---

## Cấu hình tối ưu (Profiles)

Mặc định giữ lại: **Windows Defender, Firewall, Microsoft Store và Edge/WebView**. Không can thiệp dịch vụ Anti-Cheat.

### 1. Standard (Khuyên dùng)
- Cấu hình cân bằng, an toàn tuyệt đối cho mọi nhu cầu sử dụng hàng ngày và làm việc.
- Dọn sạch bloatware, tắt telemetry và giải phóng tài nguyên nền.
- Giữ nguyên độ ổn định gốc của Windows, cắm là chạy không cần tinh chỉnh thêm.

### 2. Performance (Chuyên sâu)
*Bao gồm toàn bộ cấu hình Standard và bổ sung:*
- Dành riêng cho máy chỉ chơi game, muốn vắt kiệt hiệu năng phần cứng.
- **Power Plan:** Kích hoạt High Performance (Desktop) và tối ưu Core Parking theo nguồn cấp.
- **Thiết bị:** Tự động bật HAGS và MSI Mode cho GPU/NIC đủ điều kiện.
- **Storage & Latency:** Kiểm tra kích hoạt TRIM, ép HPET qua BCD và ghim Timer Resolution 0.500 ms.

---

## Tùy chọn thành phần

| Thành phần | Mặc định | Lưu ý |
| :--- | :---: | :--- |
| **Gỡ OneDrive** | Bật | Cần tải dữ liệu quan trọng về ổ đĩa cục bộ trước khi chạy. |
| **Gỡ Xbox & Game Bar** | Bật | Ảnh hưởng Game Pass và tính năng ghi hình. |
| **Tắt Windows Search** | Bật | Giảm tải nền ổ cứng và CPU. |
| **Tắt Bluetooth** | Tắt | Bật nếu máy bàn không dùng thiết bị Bluetooth. |
| **Tắt dịch vụ In / Scan** | Tắt | Tắt nếu không dùng máy in (`Spooler`). |
| **Tắt Cảm ứng & Pen** | Tắt | Tắt trên Desktop thường để giảm tiến trình thừa. |
| **Cài Trình duyệt** | Tắt | Tùy chọn cài sạch Brave, Chrome hoặc Firefox. |

<details>
<summary><strong>Chi tiết các dịch vụ được tinh chỉnh</strong></summary>

- **Telemetry & Diagnostic:** `DiagTrack`, `dmwappushservice`, `DPS`, `diagsvc`, `WerSvc`, `wercplsupport`.
- **Dịch vụ nền:** `SysMain`, `MapsBroker`, `RetailDemo`, `RemoteRegistry`, `Fax`, `OneSyncSvc`, `WpnService`.
- **Dịch vụ theo tùy chọn:** `WSearch` (Search), `bthserv` (Bluetooth), `Spooler` (Print), `TabletInputService` (Touch).

</details>

---

## Runtime tích hợp

Playbook tự động kiểm tra và bổ sung các thư viện hệ thống cần thiết:
- **Visual C++ Redistributable (2015–2022 x86/x64)**
- **DirectX End-User Runtimes (June 2010)**
- **.NET Framework 3.5**

---

<a id="cài-đặt"></a>

## Quy trình cài đặt

1. Kiểm tra Build Windows (`winver`) và cập nhật hoàn tất các update đang chờ.
2. Tải [AME Wizard](https://amelabs.io) và file `.apbx` từ mục [Releases](https://github.com/nyxvergil/Superstrike-x1/releases).
3. Khởi chạy `.apbx` thông qua AME Wizard bằng quyền Administrator.
4. Chọn Profile (`Standard` hoặc `Performance`) và tích chọn các thành phần mong muốn.
5. Chờ hoàn tất quá trình thiết lập và khởi động lại máy.

---

## Hỗ trợ & Đóng góp

- **Báo lỗi:** Mở [GitHub Issues](https://github.com/nyxvergil/Superstrike-x1/issues), cung cấp phiên bản Windows (`winver`), thông số phần cứng và đính kèm file log (nhớ xóa bỏ thông tin cá nhân hoặc token trước khi gửi).
- **Cộng đồng:** Tham gia trao đổi, thảo luận trực tiếp tại [Discord Cộng đồng](https://discord.gg/strikeos).
- **Phạm vi hỗ trợ:** Hỗ trợ kỹ thuật được duy trì trong khả năng của đội ngũ phát triển. Đối với các gói dịch vụ tùy biến có phí, quyền lợi sẽ áp dụng theo thỏa thuận riêng.
- **Cập nhật:** Các phiên bản mới kèm changelog được phát hành chính thức tại thẻ Releases. Playbook không hỗ trợ tự cập nhật ngầm.

---

## Nguồn tham khảo & Giấy phép

Dự án học hỏi cách cấu trúc và triển khai từ các playbook đi trước: **AtlasOS, ReviOS, XOS, FSOS, Atom, SapphireOS**.

<sub>StrikeOS là dự án độc lập, không đại diện hoặc chịu sự ủy quyền từ các bên nêu trên. Chi tiết xem tại [LICENSE](./LICENSE) và tài liệu giấy phép đi kèm. Dự án tuyệt đối không cung cấp khóa sản phẩm hay công cụ kích hoạt Windows.</sub>

---

<p align="center"><strong>SuperStrike X1 · StrikeOS</strong></p>
