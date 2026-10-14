<p align="center">
  <a href="https://strikeos.site">
    <img src="./strike-logo.png" alt="StrikeOS" width="760">
  </a>
</p>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/VERSION-1.0.1-5B21FF?style=for-the-badge">
  <img alt="Windows" src="https://img.shields.io/badge/WINDOWS-10%20%7C%2011-0078D4?style=for-the-badge&logo=windows11&logoColor=white">
  <img alt="AME Playbook" src="https://img.shields.io/badge/AME-PLAYBOOK-202020?style=for-the-badge">
  <img alt="Status" src="https://img.shields.io/badge/STATUS-STABLE-10B981?style=for-the-badge">
</p>

<p align="center">
  <img alt="Supported builds" src="https://img.shields.io/badge/BUILD-19045%20%7C%2026100%20%7C%2026200-2563EB?style=flat-square">
  <img alt="Architecture" src="https://img.shields.io/badge/ARCH-x64-6D28D9?style=flat-square">
  <img alt="Profiles" src="https://img.shields.io/badge/PROFILE-STANDARD%20%7C%20PERFORMANCE-E11D48?style=flat-square">
</p>

<p align="center"><strong>Tinh gọn Windows cho chơi game, giữ lại các thành phần bảo mật cốt lõi.</strong></p>

<p align="center">
  <a href="https://strikeos.site">Website</a> ·
  <a href="https://discord.gg/strikeos">Discord</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/releases">Releases</a> ·
  <a href="#cài-đặt">Cài đặt</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/issues">Báo lỗi</a>
</p>

---

## Giới thiệu

**SuperStrike X1** là AME Playbook dùng để cấu hình và tinh gọn trực tiếp trên bản cài Windows bạn đang sử dụng. Đây **không phải là bản Windows tùy chỉnh (custom ISO)** và hoàn toàn không yêu cầu bạn phải cài lại hệ điều hành.

Playbook cung cấp 2 chế độ cấu hình (**Standard** và **Performance**), đi kèm các tùy chọn gỡ bỏ ứng dụng không cần thiết, tắt các dịch vụ nền hao tài nguyên và hỗ trợ cài đặt sẵn trình duyệt web theo nhu cầu.

Mục tiêu cốt lõi của SuperStrike X1 là: **giảm tải tiến trình chạy ngầm, ổn định độ trễ thời gian thực (frametime/DPC latency), nhưng tuyệt đối giữ lại Windows Defender, DEP, Secure Boot và các thành phần bảo mật cần thiết để tương thích hoàn toàn với các hệ thống Anti-cheat hiện đại.**

---

## Cảnh báo và miễn trừ trách nhiệm

> **SuperStrike X1 là bản thử nghiệm, được cung cấp “nguyên trạng” (AS IS). Chỉ tiếp tục nếu bạn hiểu các thay đổi và chấp nhận rủi ro.**

- **Thay đổi hệ thống:** Playbook thay đổi ứng dụng, dịch vụ, tác vụ và cài đặt Windows. Có thể phát sinh lỗi, mất chức năng hoặc gián đoạn mạng. Playbook không tạo bản sao lưu và không hoàn tác toàn bộ; hãy tạo System Image hoặc bản sao lưu có thể khôi phục trước khi chạy.
- **Phạm vi kiểm thử:** Phiên bản được liệt kê là phạm vi build mục tiêu, không bảo đảm đã kiểm thử trên mọi Edition, phần cứng, driver hay phần mềm. Lỗi ở bước bắt buộc hoặc tiến trình quá thời hạn có thể khiến AME Wizard dừng. “Completed” không có nghĩa mọi tùy chọn đều đã áp dụng.
- **Không cam đoan số liệu ảo:** Không bảo đảm FPS, 1% Low, 0.1% Low, độ trễ, mức dùng RAM, số tiến trình hoặc khả năng tương thích với mọi game và Anti-cheat. Việc giữ lại thành phần bảo mật không phải chứng nhận từ nhà phát hành game.
- **Môi trường sử dụng:** Không khuyến nghị dùng trên máy chủ, máy làm việc quan trọng hoặc thiết bị thuộc Domain/MDM nếu chưa được quản trị viên cho phép. Bạn cần có quyền quản trị và quyền thực hiện thay đổi trên thiết bị.
- **Nguồn tải an toàn:** Chỉ tải bản phát hành từ Releases của repository được liên kết trên [strikeos.site](https://strikeos.site/). Đối chiếu SHA-256 nếu có công bố. Không chạy bản đã chỉnh sửa hoặc đóng gói lại từ nguồn khác. Các Runtime tải trong quá trình cài đặt đến từ nhà cung cấp tương ứng và nằm ngoài kiểm soát của dự án.
- **Trách nhiệm pháp lý:** Việc tải và sử dụng là quyết định của bạn. Trong phạm vi pháp luật cho phép, dự án không chịu trách nhiệm cho thiệt hại phát sinh từ việc sử dụng hoặc không thể sử dụng Playbook. Nội dung này không loại trừ quyền của người dùng hay trách nhiệm mà pháp luật không cho phép miễn trừ. Đây không phải tư vấn pháp lý.
- **Hỗ trợ & Bảo mật thông tin:** Hỗ trợ lỗi qua GitHub Issues hoặc Discord theo khả năng duy trì dự án; không cam kết thời gian phản hồi, sửa lỗi hoặc lịch cập nhật. Khi gửi log công khai, hãy xóa mật khẩu, token, khóa sản phẩm và thông tin cá nhân.

---

## Windows hỗ trợ

| Hệ điều hành | Phiên bản | Build mục tiêu | Tình trạng |
|---|---:|---:|:---:|
| **Windows 10 64-bit** | 22H2 | `19045` | Hỗ trợ chính thức |
| **Windows 11 64-bit** | 24H2 | `26100` | Hỗ trợ chính thức |
| **Windows 11 64-bit** | 25H2 | `26200` | Hỗ trợ thử nghiệm |

> [!IMPORTANT]
> Chỉ áp dụng trên các bản cài đặt Windows x64 chính thức nguyên bản từ Microsoft. Các bản Windows đã bị mod sâu (Ghost, Lite, ReviOS, AtlasOS...) có thể đã bị gỡ mất các component phục vụ servicing khiến AME Wizard báo lỗi và dừng tiến trình.

---

## Chế độ hoạt động (Profiles)

Trong bước thiết lập của AME Wizard, bạn sẽ chọn 1 trong 2 chế độ:

### 1. Standard Profile
Phù hợp cho máy tính dùng hỗn hợp (chơi game kết hợp học tập, làm việc hằng ngày):
* Gỡ bỏ các ứng dụng rác mặc định của Microsoft, tắt các luồng thu thập dữ liệu chẩn đoán (telemetry) ngầm.
* Tắt các dịch vụ chạy ngầm không cần thiết, giảm tải chu kỳ CPU khi máy ở trạng thái rảnh rỗi.
* Giữ nguyên cơ chế quản lý năng lượng gốc, không can thiệp sâu vào driver hay cấu hình mạng.

### 2. Performance Profile *(Dành riêng cho máy chơi Game)*
Bao gồm toàn bộ thiết lập của **Standard**, kèm theo các tinh chỉnh tối ưu phần cứng và độ trễ:
* **Bộ đếm thời gian (Hardware TSC):** Đồng bộ hóa xung nhịp BCD với `disabledynamictick yes`, `useplatformtick yes` và `tscsyncpolicy enhanced`. Tuyệt đối **không ép bật HPET** (`useplatformclock`) để đảm bảo hệ thống sử dụng bộ đếm Invariant TSC trực tiếp trên CPU, triệt tiêu hiện tượng giật cục (micro-stutter).
* **Độ phân giải Timer (0.5ms):** Tích hợp tiến trình dịch vụ C# độc quyền `StrikeTimerResolution` (0.5ms) chạy ngầm từ lúc đăng nhập, tăng tần suất phản hồi khung hình và giảm độ trễ nhập liệu chuột/bàn phím.
* **Đồ họa & Hiển thị:** Bật Hardware-accelerated GPU Scheduling (HAGS), mở khóa DirectX Flip Model (`SwapEffectUpgradeEnable = 1`) giúp game chạy chế độ Borderless/Windowed có độ trễ tiệm cận Fullscreen độc quyền.
* **Ngắt thiết bị (MSI Mode):** Tự động chuyển đổi chế độ ngắt Message Signaled Interrupts (MSI) cho GPU và Card mạng PCIe để phân bổ ngắt mượt hơn, tránh xung đột IRQ dòng truyền thống.
* **Quản lý Nguồn điện (Desktop):** Tự động nhận diện thiết bị. Nếu là Desktop, playbook kích hoạt High Performance, bỏ Core Parking (`CPMINCORES 100`) và giữ CPU luôn sẵn sàng xử lý. Nếu là Laptop, playbook **giữ nguyên thiết lập pin** để tránh quá nhiệt và hao pin.
* **Tinh chỉnh Card mạng LAN vật lý:** Tắt các cơ chế tiết kiệm điện và gom gói tin gây trễ (RSC, EEE, Flow Control, Interrupt Moderation). Đồng thời giữ nguyên cơ chế **TCP Window Auto-Tuning** tự nhiên của Windows để đảm bảo tốc độ tải file và tải game đạt tối đa băng thông mạng cáp quang.
* **Đặt lại mạng:** Làm sạch bộ nhớ đệm DNS, đặt lại Winsock và TCP/IP để triệt tiêu các thiết lập mạng lỗi từ trước.

---

## Tùy chọn trong AME Wizard

Các mục được hiển thị riêng biệt để bạn chủ động quyết định theo thói quen sử dụng:

* **OneDrive, Xbox/Game Bar và Windows Search:** được tích sẵn. Bỏ chọn nếu muốn giữ các thành phần này. Việc gỡ Xbox/Game Bar có thể ảnh hưởng Game Pass, ghi hình hoặc tính năng liên quan.
* **Bluetooth, in/scan và bàn phím cảm ứng/viết tay:** mặc định không chọn. Hai lựa chọn đầu có thể tắt dịch vụ và driver liên quan sau khi xác nhận. Lựa chọn cảm ứng/viết tay tắt dịch vụ `TabletInputService`; không gỡ phần cứng hay driver cảm ứng.
* **Trình duyệt:** mặc định không cài. Nếu bật, chọn Brave, Firefox hoặc Chrome.

---

## Gaming Runtime

Playbook kiểm tra Visual C++ 2015–2022 x86/x64, DirectX Legacy và .NET Framework 3.5; thành phần đã có sẽ được bỏ qua. Thành phần còn thiếu được cài từ nguồn chính thức của Microsoft kèm xác thực chữ ký Authenticode. Nếu không tải được hoặc Windows không có nguồn cài cần thiết, Runtime có thể được ghi nhận là chưa cài và các bước tiếp tục. Nếu trình cài đặt hoặc Windows servicing vượt thời hạn chờ, AME Wizard có thể dừng để tránh chạy chồng tiến trình cài đặt.

---

## Hướng dẫn cài đặt

1. Nhấn `Win + R`, gõ `winver` để xác nhận hệ điều hành nằm trong danh sách hỗ trợ (`19045`, `26100` hoặc `26200`).
2. Sao lưu dữ liệu; ưu tiên tạo System Image hoặc bản sao lưu có thể khôi phục.
3. Tải AME Wizard và tệp `.apbx` (hoặc `.zip`) từ nguồn chính thức.
4. Mở tệp bằng AME Wizard, chọn chế độ (**Standard** hoặc **Performance**) và kiểm tra kỹ các tùy chọn.
5. Trong khi chạy, không tắt máy, đóng Wizard hoặc chạy thêm công cụ tối ưu khác.
6. Đọc kết quả và cảnh báo; khởi động lại máy tính khi được yêu cầu để các thiết lập phần cứng và driver có hiệu lực.

---

## Báo lỗi và Đóng góp

Tạo [GitHub Issue](https://github.com/nyxvergil/Superstrike-x1/issues) hoặc liên hệ qua [Discord](https://discord.gg/strikeos). Gửi phiên bản Windows, cấu hình máy, chế độ và lựa chọn đã dùng cùng log AME Wizard (hoặc file log tại `%ProgramData%\StrikeOS\Logs`). Vui lòng xóa thông tin nhạy cảm trước khi đăng.

---

<p align="center"><strong>SuperStrike X1 · StrikeOS</strong></p>
