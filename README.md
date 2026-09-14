<p align="center">
  <a href="https://strikeos.site">
    <img src="./strike-logo.png" alt="SuperStrike X1" width="760">
  </a>
</p>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/VERSION-1.0.1-5B21FF?style=for-the-badge">
  <img alt="Windows" src="https://img.shields.io/badge/WINDOWS-10%20%7C%2011-0078D4?style=for-the-badge&logo=windows11&logoColor=white">
  <img alt="AME Playbook" src="https://img.shields.io/badge/AME-PLAYBOOK-202020?style=for-the-badge">
  <img alt="Defender Retained" src="https://img.shields.io/badge/DEFENDER-RETAINED-16A34A?style=for-the-badge&logo=windowsdefender&logoColor=white">
  <a href="./LICENSE"><img alt="License" src="https://img.shields.io/badge/LICENSE-MIT-4B5563?style=for-the-badge"></a>
</p>

<p align="center">
  <img alt="Supported builds" src="https://img.shields.io/badge/BUILD-19045%20%7C%2026100%20%7C%2026200-2563EB?style=flat-square">
  <img alt="Architecture" src="https://img.shields.io/badge/ARCH-x64-6D28D9?style=flat-square">
  <img alt="Profiles" src="https://img.shields.io/badge/PROFILES-STANDARD%20%7C%20PERFORMANCE-E11D48?style=flat-square">
  <img alt="Anti-Cheat Ready" src="https://img.shields.io/badge/ANTI--CHEAT-100%25%20COMPATIBLE-059669?style=flat-square">
</p>

<p align="center"><strong>Tinh gọn để chơi game. Giữ lại những gì Windows và Anti-cheat thực sự cần.</strong></p>

<p align="center">
  <a href="https://strikeos.site">🌐 Website</a>
  •
  <a href="https://discord.gg/strikeos">💬 Discord</a>
  •
  <a href="../../releases">📥 Tải về (Releases)</a>
  •
  <a href="#-hướng-dẫn-cài-đặt">📖 Hướng dẫn</a>
  •
  <a href="#-báo-cáo-lỗi--hỗ-trợ">🛠️ Báo lỗi</a>
</p>

---

## ⚠️ Lưu ý quan trọng (Disclaimer)

> [!WARNING]
> Playbook thay đổi sâu vào Windows. Hãy tạo **bản sao lưu hệ thống và dữ liệu quan trọng** trước khi sử dụng. Restore Point chỉ là biện pháp bổ sung, không thay thế bản sao lưu đầy đủ.
>
> - **Việc sử dụng Playbook** là quyết định tự nguyện của bạn. Hãy đọc kỹ các thay đổi, cân nhắc rủi ro và sao lưu trước khi chạy. Quyết định này không làm mất các quyền hợp pháp của bạn hoặc miễn trừ trách nhiệm của bên phát triển theo pháp luật áp dụng.
> - **Không khuyến nghị:** Sử dụng trên máy chủ, máy làm việc quan trọng, thiết bị thuộc Domain/MDM khi chưa được quản trị viên cho phép, hoặc Windows đã qua can thiệp bằng công cụ khác. Không chạy khi chưa có bản sao lưu hay sử dụng tệp từ nguồn không xác minh được.
> - **Hiệu năng và tương thích:** Không cam kết mức FPS, độ trễ, RAM, số Process cố định hoặc tương thích với mọi Driver, game và Anti-cheat. Giữ lại dịch vụ bảo mật không đồng nghĩa được bên thứ ba chứng nhận.
> -  **Hỗ trợ và cập nhật:** Tiếp nhận lỗi qua [Discord](https://discord.gg/strikeos) theo khả năng duy trì dự án, không cam kết thời gian xử lý hay lịch cập nhật. Đọc hướng dẫn Release trước khi chạy chồng phiên bản. Dịch vụ trả phí tuân theo thỏa thuận riêng.
> - **Nguồn tải chính thức:** Chỉ tải Playbook từ Releases của repository được liên kết trên [strikeos.site](https://strikeos.site). Đối chiếu SHA256 nếu bản phát hành có công bố. StrikeOS không chủ động tích hợp virus, keylogger, botnet hoặc chức năng đánh cắp dữ liệu. Bản do bên thứ ba chỉnh sửa hoặc đóng gói lại không được xem là bản chính thức; StrikeOS không kiểm soát hay bảo đảm tính toàn vẹn của các bản đó. Nếu phát hiện dấu hiệu bất thường, hãy ngừng chạy và báo lại kèm nguồn tải, tên tệp, SHA256 và cảnh báo bảo mật để xác minh.
---

## 🎮 Giới thiệu SuperStrike X1

Chào mọi người, **SuperStrike X1** là dự án đầu tiên mình đóng gói và phát hành sau một thời gian tự tìm hiểu, tham khảo và thử nghiệm các cách Tinh chỉnh Windows để phù hợp  cho nhu cầu chơi game.

Mình muốn Windows bớt những thứ chạy nền không cần dùng, đồng thời giữ lại các chức năng và thành phần bảo mật cần thiết. Khả năng tương thích với game và Anti-cheat là điều mình ưu tiên, nhưng vẫn cần kiểm thử trên từng cấu hình thực tế.

Đây là dự án đầu tay nên sẽ còn thiếu sót. Mình mong nhận được góp ý thẳng thắn, cả những trường hợp chạy tốt lẫn những lỗi gặp phải. Việc sửa lỗi và cập nhật sẽ dựa trên phản hồi thực tế cùng thời gian mình có thể dành cho dự án.

Nếu gặp vấn đề hoặc có đề xuất, hãy nhắn qua [Discord](https://discord.gg/strikeos) hoặc tạo [Issue](https://github.com/nyxvergil/Superstrike-x1/issues). Khi báo lỗi, gửi kèm cấu hình máy và Log để mình có cơ sở kiểm tra.

Cảm ơn mọi người đã dành thời gian dùng thử và góp ý.

---

## 🪟 Khả năng tương thích

| Hệ điều hành | Phiên bản | Build hỗ trợ | Trạng thái |
|---|:---:|:---:|:---:|
| **Windows 10 64-bit** | 22H2 | `19045` | ✅ Tương thích chính thức |
| **Windows 11 64-bit** | 24H2 | `26100` | ✅ Tương thích chính thức |
| **Windows 11 64-bit** | 25H2 | `26200` | ✅ Thử nghiệm & Hỗ trợ |

> [!NOTE]
> Để tránh xung đột hệ thống, Playbook sẽ **tự động từ chối chạy** trên các bản Build không nằm trong danh sách kiểm thử trên.

---

## ⚙️ Các chế độ cấu hình

### 🛡️ Standard — Cấu hình mặc định

- Gỡ ứng dụng theo danh sách, giảm Telemetry và điều chỉnh dịch vụ, tác vụ nền.
- Áp dụng thiết lập hiệu năng của Gaming Lean, gồm bộ nhớ, ưu tiên foreground, FTH và BCD/timer.
- Điều chỉnh Game DVR và các thiết lập giao diện.
- Bluetooth và in ấn chỉ bị tắt khi chọn tùy chọn tương ứng. Windows Search được tích tắt sẵn; hãy bỏ chọn nếu còn dùng.

### 🚀 Performance — Thêm thiết lập mạng và phần cứng

- Bao gồm các thay đổi của **Standard**.
- **Mạng:** Bật RSS, đặt TCP Auto-Tuning về `normal`, tắt RSC và chỉnh một số thuộc tính Card mạng khi có hỗ trợ. Reset Winsock/IP và xóa DNS cache.
- **Nguồn điện:** Chọn High Performance trên Desktop; điều chỉnh Core Parking có phân biệt Laptop và trạng thái dùng nguồn.
- **Đồ họa:** Ghi thiết lập bật HAGS; bật MSI Mode cho GPU/Card mạng được chọn khi đã có khóa cấu hình tương ứng.
- **Storage:** Kiểm tra và bật TRIM khi cần, không chạy Defrag trong lúc cài.
- **Timer:** Ép HPET qua BCD và tạo tác vụ chạy tiện ích nền yêu cầu Timer Resolution 0,5 ms.

> [!WARNING]
> Performance không bảo đảm nhanh hơn Standard. Hiệu quả phụ thuộc phần cứng và Driver. Hãy lưu cấu hình IP/DNS riêng trước khi chạy và đo hiệu năng trước/sau. Chọn Standard sau Performance không hoàn tác toàn bộ các thay đổi.
---

## 🧩 Tùy chọn bổ sung (Optional Components)

Trước khi bấm chạy, bạn có thể tùy ý chọn bật/tắt các thành phần:

- [ ] **Gỡ OneDrive hoàn toàn:** Tự động di chuyển dữ liệu cá nhân (Desktop, Documents, Pictures) về thư mục cục bộ an toàn trước khi gỡ.
- [ ] **Gỡ bỏ Xbox & Game Bar:** Dành cho game thủ không dùng Xbox App / Cloud Gaming.
- [ ] **Tắt Windows Search Indexing:** Giảm tải đọc/ghi ổ cứng (chức năng tìm kiếm tên file vẫn hoạt động bình thường).
- [ ] **Vô hiệu hóa Bluetooth:** Dành cho máy PC để bàn không có card Bluetooth.
- [ ] **Vô hiệu hóa Print & Fax Spooler:** Tắt toàn bộ tiến trình liên quan đến in ấn/quét tài liệu.
- [ ] **Cài đặt trình duyệt ưa thích:** Tùy chọn cài sạch **Brave**, **Firefox** hoặc **Google Chrome**.

---

## 📦 Gaming Runtimes

Playbook tự động quét và chuẩn đoán các thư viện game cần thiết. Thành phần nào đã có sẽ được giữ nguyên; thành phần thiếu sẽ được tải và cài đặt trực tiếp từ **máy chủ Microsoft (có chữ ký số hợp lệ)**:

- **Visual C++ Redistributable (2015–2022)** cả x86 và x64.
- **DirectX End-User Runtimes (Legacy 9.0c / June 2010)**.
- **.NET Framework 3.5 / 4.8**.

*Ghi chú: Nếu hệ thống không có mạng hoặc nguồn tải Microsoft gặp sự cố, Playbook sẽ đánh dấu `SkippedNoSource` và tiếp tục quá trình mà không tạo báo cáo thành công giả.*

---

## 🔍 Chi tiết các dịch vụ được tối ưu

SuperStrike X1 tắt bỏ các tiến trình và dịch vụ nền không có tác dụng trong quá trình chơi game nhằm giải phóng CPU cycle và RAM.

<details>
<summary>👉 <strong>Nhấn vào đây để xem danh sách dịch vụ bị vô hiệu hóa</strong></summary>

| Tên Dịch vụ (Service) | Mục đích / Lý do vô hiệu hóa |
| :--- | :--- |
| **DiagTrack** (Connected User Experiences) | Dịch vụ thu thập Telemetry và gửi dữ liệu chẩn đoán về Microsoft. |
| **dmwappushservice** | Kênh gửi dữ liệu WAP Push telemetry. |
| **DPS / WdiServiceHost / WdiSystemHost** | Hệ thống chẩn đoán Diagnostic Policy Service chạy ngầm định kỳ. |
| **SysMain** (Superfetch) | Tự động cache ứng dụng vào RAM; thường gây nghẽn I/O trên SSD khi chơi game. |
| **MapsBroker** | Dịch vụ tải và đồng bộ bản đồ ngoại tuyến của Windows. |
| **RetailDemo** | Dịch vụ demo gian hàng bán lẻ (hoàn toàn vô dụng). |
| **RemoteRegistry** | Cho phép chỉnh sửa Registry từ xa (vừa tốn tài nguyên, vừa là lỗ hổng bảo mật). |
| **SensrSvc / SensorDataService** | Nhận diện cảm biến xoay màn hình (không cần thiết trên Desktop PC). |
| **WSearch** *(Tùy chọn)* | Dịch vụ lập chỉ mục tệp (Indexing); tắt để giải phóng I/O đĩa. |
| **Print Spooler** *(Tùy chọn)* | Hàng đợi in ấn; tắt nếu máy không kết nối máy in. |
| **bthserv / BTAGService** *(Tùy chọn)* | Dịch vụ kết nối Bluetooth; chỉ tắt khi người dùng chọn tắt Bluetooth. |

</details>

---

## 📖 Hướng dẫn cài đặt

### Checklist chuẩn bị
1. Đảm bảo Windows **không còn bản cập nhật nào đang chờ khởi động lại** (Pending Update).
2. Tạm thời tắt **Tamper Protection** trong *Windows Security > Virus & threat protection settings* (Bắt buộc để AME Wizard có quyền ghi Registry hệ thống).
3. Tạo một **Điểm khôi phục (System Restore Point)** hoặc Backup dữ liệu quan trọng.
4. Cắm sạc nguồn đầy đủ (đối với laptop).

### Các bước thực hiện

```mermaid
graph LR
A[Tải AME Wizard] --> B[Tải SuperStrike.apbx]
B --> C[Kéo thả vào Wizard]
C --> D[Chọn Standard / Performance]
D --> E[Khởi động lại máy]
