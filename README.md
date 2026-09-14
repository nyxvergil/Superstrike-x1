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
> Playbook can thiệp sâu vào Windows. Mặc dù SuperStrike X1 được thiết kế với tiêu chuẩn tương thích và an toàn cao, bạn **bắt buộc phải tạo Điểm khôi phục (Restore Point) hoặc Bản sao lưu hệ thống (System Image)** trước khi sử dụng.
>
> - **Không khuyến nghị:** Sử dụng trên máy chủ, máy làm việc quan trọng, thiết bị thuộc Domain/MDM khi chưa được quản trị viên cho phép, hoặc Windows đã qua can thiệp bằng công cụ khác. Không chạy khi chưa có bản sao lưu hay sử dụng tệp từ nguồn không xác minh được.
> - **Hiệu năng và tương thích:** Không cam kết mức FPS, độ trễ, RAM, số Process cố định hoặc tương thích với mọi Driver, game và Anti-cheat. Giữ lại dịch vụ bảo mật không đồng nghĩa được bên thứ ba chứng nhận.
> -  **Hỗ trợ và cập nhật:** Tiếp nhận lỗi qua Discord theo khả năng duy trì dự án, không cam kết thời gian xử lý hay lịch cập nhật. Đọc hướng dẫn Release trước khi chạy chồng phiên bản. Dịch vụ trả phí tuân theo thỏa thuận riêng.
> - **Nguồn tải chính thức:** Chỉ tải Playbook từ Releases của repository được liên kết trên [strikeos.site](https://strikeos.site). Đối chiếu SHA256 nếu bản phát hành có công bố. StrikeOS không chủ động tích hợp virus, keylogger, botnet hoặc chức năng đánh cắp dữ liệu. Bản do bên thứ ba chỉnh sửa hoặc đóng gói lại không được xem là bản chính thức; StrikeOS không kiểm soát hay bảo đảm tính toàn vẹn của các bản đó. Nếu phát hiện dấu hiệu bất thường, hãy ngừng chạy và báo lại kèm nguồn tải, tên tệp, SHA256 và cảnh báo bảo mật để xác minh.
---

## 🎮 Giới thiệu SuperStrike X1

Chào mọi người, **SuperStrike X1** là sản phẩm đầu tiên mình đóng gói và phát hành sau một thời gian dài tự mày mò, nghiên cứu về cách Windows điều phối tài nguyên và tối ưu độ trễ cho game.

Dự án ra đời với một tiêu chí rất rõ ràng: **Tinh gọn vừa đủ để mượt, nhưng tuyệt đối không phá hỏng hệ thống hay làm hỏng Anti-cheat**. 

Là dự án đầu tay, mình biết sản phẩm chắc chắn sẽ còn những "hạt sạn", lỗi vặt hoặc chưa thể làm hài lòng tất cả mọi cấu hình máy. Vì vậy:
- Mình luôn trân trọng mọi góp ý thẳng thắn, dù là khen hay chê.
- Mình sẽ liên tục học hỏi, tinh chỉnh và update các tính năng thực sự cần thiết trong tương lai dựa trên phản hồi thực tế của các bạn.

Nếu trong quá trình trải nghiệm có phát sinh lỗi hoặc bạn có ý tưởng tối ưu nào hay, hãy hú mình qua [Discord](https://discord.gg/strikeos) hoặc tạo [Issue](../../issues) nhé. Rất mong nhận được sự đồng hành và đóng góp từ cộng đồng!

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

Trong giao diện AME Wizard, bạn có thể lựa chọn 1 trong 2 chế độ phù hợp với nhu cầu:

### 🛡️ Chế độ Standard (Khuyến nghị cho số đông)
- Cân bằng hoàn hảo giữa tính ổn định, độ trễ và sự tiện lợi hàng ngày.
- Gỡ bỏ Bloatware, ứng dụng UWP rác, vô hiệu hóa Telemetry (theo dõi ngầm) và Diagnostics.
- Tắt các dịch vụ chạy ngầm vô bổ, giữ nguyên các tính năng in ấn, Bluetooth và tìm kiếm cơ bản.
- Phù hợp với mọi máy tính vừa dùng làm việc, vừa chơi game.

### 🚀 Chế độ Performance (Dành cho máy thuần Gaming)
- Bao gồm toàn bộ tối ưu của **Standard**.
- **Mạng & Bộ đệm:** TCP Auto-Tuning, RSS (Receive Side Scaling), NetDMA, tinh chỉnh Network Adapter và thiết lập lại Winsock/IP Stack.
- **Phần cứng & Nhân hệ thống:** Bật MSI Mode cho GPU/Network, thiết lập Power Plan tùy chỉnh, Core Parking off, Timer Resolution tối ưu và kích hoạt TRIM cho SSD.
- **Đồ họa:** Đồng bộ HAGS (Hardware-Accelerated GPU Scheduling) và tối ưu hóa Game DVR.

> [!TIP]
> Chế độ **Performance** sẽ đặt lại cấu hình IP/Winsock. Nếu bạn đang cài **IP tĩnh hoặc DNS tùy chỉnh**, hãy lưu lại thông tin để thiết lập lại sau khi máy khởi động.

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
