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
  <a href="#hướng-dẫn-cài-đặt">Cài đặt</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/issues">Báo lỗi</a>
</p>

---

## Giới thiệu

**SuperStrike X1** là AME Playbook dùng để cấu hình và tinh gọn trực tiếp trên bản cài Windows bạn đang sử dụng. Đây **không phải là bản Windows tùy chỉnh (custom ISO)** và hoàn toàn không yêu cầu bạn phải cài lại hệ điều hành.

Playbook cung cấp 2 chế độ cấu hình (**Standard** và **Performance**), đi kèm các tùy chọn gỡ bỏ ứng dụng không cần thiết, tắt các dịch vụ nền hao tài nguyên và hỗ trợ cài đặt sẵn trình duyệt web theo nhu cầu.

Mục tiêu cốt lõi của SuperStrike X1 là: **giảm tải tiến trình chạy ngầm, ổn định độ trễ thời gian thực (frametime/DPC latency), nhưng giữ lại các thành phần bảo mật cần thiết (DEP, Secure Boot, Windows Defender mặc định) để duy trì khả năng tương thích với các hệ thống Anti-cheat hiện đại.**

---

## Cảnh báo và miễn trừ trách nhiệm

> **SuperStrike X1 được cung cấp theo nguyên tắc “nguyên trạng” (AS IS). Người dùng tự chịu trách nhiệm khi áp dụng trên thiết bị.**

- **Thay đổi hệ thống:** Playbook can thiệp vào ứng dụng, dịch vụ, tác vụ và Registry của Windows. Luôn tạo **System Restore Point** hoặc bản sao lưu hình ảnh hệ thống (System Image) trước khi thực hiện.
- **Phạm vi kiểm thử:** Phiên bản được thiết kế cho các bản dựng mục tiêu đã công bố, nhưng không thể bao quát toàn bộ các phiên bản driver, phần cứng hay phần mềm đặc thù của bên thứ ba.
- **Không cam đoan số liệu ảo:** Dự án không đưa ra bất kỳ bảo đảm nào về các con số FPS ảo, mức dùng RAM cố định hay tỉ lệ giảm độ trễ cụ thể. Hiệu năng thực tế phụ thuộc trực tiếp vào cấu hình phần cứng (CPU, GPU, RAM), nhiệt độ vận hành và driver của từng máy.
- **Rủi ro công cụ tự chọn:** Thư mục Post-Install có chứa các tùy chọn nâng cao cho phép tắt Windows Defender hoặc tạm dừng Windows Update. Đây là những can thiệp sâu vào cơ chế tự bảo vệ của Windows; chỉ kích hoạt khi bạn hiểu rõ rủi ro an ninh mạng và có giải pháp thay thế phù hợp.
- **Môi trường sử dụng:** Không khuyến nghị áp dụng trên máy chủ, máy tính kế toán/ngân hàng, thiết bị doanh nghiệp thuộc Domain/MDM hoặc máy làm việc quan trọng.
- **Nguồn tải an toàn:** Chỉ tải tệp phát hành từ Releases chính thức của repository hoặc [strikeos.site](https://strikeos.site/). Vui lòng đối chiếu mã băm SHA-256 trước khi thực thi.

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
* Gỡ bỏ các ứng dụng UWP rác mặc định của bên thứ ba, vô hiệu hóa các luồng thu thập dữ liệu chẩn đoán (telemetry) ngầm.
* Tắt các dịch vụ chạy ngầm không cần thiết, giảm tải chu kỳ CPU khi máy ở trạng thái rảnh rỗi.
* Giữ nguyên cơ chế quản lý năng lượng gốc, không can thiệp sâu vào driver hay cấu hình mạng.

### 2. Performance Profile *(Dành riêng cho máy chơi Game)*
Bao gồm toàn bộ thiết lập của **Standard**, kèm theo các tinh chỉnh chuyên sâu về phần cứng và độ trễ:
* **Đồng hồ hệ thống (Hardware Invariant TSC):** Tinh chỉnh cấu hình BCD với `disabledynamictick yes` và `tscsyncpolicy enhanced`. Tuyệt đối **không ép bật HPET** (`useplatformclock`) và loại bỏ `useplatformtick` để hệ thống đọc trực tiếp bộ đếm thời gian phần cứng trên CPU, hạn chế hiện tượng giật cục (micro-stutter).
* **Độ phân giải Timer (0.5ms):** Tích hợp tiến trình dịch vụ chuyên dụng `StrikeTimerResolution` (0.5ms) chạy ngầm từ lúc đăng nhập, ổn định tần số ngắt thời gian thực và giảm độ trễ nhập liệu chuột/bàn phím.
* **Đồ họa & Hiển thị:** Bật Hardware-accelerated GPU Scheduling (HAGS) trên phần cứng hỗ trợ; tối ưu hóa DirectX Flip Model (`SwapEffectUpgradeEnable = 1`) giúp game chạy chế độ Borderless/Windowed có độ trễ tiệm cận Fullscreen độc quyền.
* **Ngắt thiết bị (MSI Mode):** Tự động chuyển đổi chế độ ngắt Message Signaled Interrupts (MSI) cho GPU và Card mạng PCIe tương thích để phân bổ ngắt mượt mà hơn, tránh xung đột chia sẻ đường IRQ truyền thống.
* **Quản lý Nguồn điện (Desktop/Laptop):** Tự động nhận diện thiết bị. Nếu là Desktop, playbook áp dụng gói năng lượng hiệu năng cao, bỏ Core Parking (`CPMINCORES 100`) để CPU luôn sẵn sàng phản hồi. Nếu là Laptop, playbook **giữ nguyên thiết lập pin gốc** để tránh quá nhiệt và hao pin.
* **Tinh chỉnh Card mạng LAN vật lý:** Tắt các cơ chế gom gói tin gây trễ (RSC) và các cơ chế tiết kiệm điện gây gián đoạn đường truyền (EEE, Flow Control, Interrupt Moderation). Đồng thời giữ nguyên cơ chế **TCP Window Auto-Tuning** tự nhiên của Windows để đảm bảo tốc độ tải file và tải game đạt tối đa băng thông cáp quang.
* **Bảo toàn mạng cá nhân:** Playbook **không tự ý reset card mạng** trong quá trình cài đặt, bảo toàn nguyên vẹn địa chỉ IP tĩnh và máy chủ DNS cá nhân của người dùng.

---

## Tùy chọn trong AME Wizard

Các mục được hiển thị riêng biệt để bạn chủ động quyết định theo nhu cầu sử dụng:

* **OneDrive, Xbox/Game Bar và Windows Search Indexing:** **Mặc định KHÔNG chọn** (`IsChecked="false"`) nhằm đảm bảo an toàn tuyệt đối. Chỉ tích chọn nếu bạn thực sự muốn gỡ bỏ hoặc vô hiệu hóa các thành phần này.
* **Bluetooth, In/Scan và Bàn phím cảm ứng:** Mặc định không chọn. Hai lựa chọn đầu có thể tắt dịch vụ và driver liên quan sau khi bạn xác nhận.
* **Trình duyệt Web:** Mặc định không cài sẵn. Nếu cần, bạn có thể tích chọn cài đặt tự động Brave, Firefox hoặc Google Chrome (được tải trực tiếp từ máy chủ chính thức của hãng).

---

## Thư mục công cụ StrikeOS Post-Install

Sau khi hoàn tất cài đặt, Playbook sẽ triển khai thư mục `StrikeOS Post-Install` ra ngoài Desktop:
- **Control Panel.bat:** Bảng điều khiển trung tâm giúp quản lý và bật/tắt nhanh các tính năng.
- **1. Trình Duyệt Web:** Hỗ trợ tải và cài đặt nhanh các trình duyệt thông dụng khi cần.
- **2. Tối Ưu Gaming:** Công cụ kiểm tra HAGS, DWM MPO Fix, gói nguồn điện chuyên dụng, công cụ tinh chỉnh chuột/bàn phím và mạng.
- **3. Bảo Mật & Update:** Tùy chọn nâng cao bật/tắt Windows Defender và tạm dừng Windows Update (kèm cảnh báo an ninh và kiểm tra quyền quản trị).
- **4. Dọn Dẹp Hệ Thống:** Script giải phóng bộ nhớ đệm (Memory Trim), dọn Shader Cache, Temp/Prefetch và công cụ đặt lại card mạng / DNS thủ công khi gặp sự cố mạng.
- **5. Khắc Phục Sự Cố:** Hỗ trợ phục hồi nhanh dịch vụ Máy in, Bluetooth, Wi-Fi, sửa lỗi bàn phím tiếng Việt (UniKey/EVKey), và bộ công cụ Sao lưu / Khôi phục Registry & BCD có tích hợp *Windows System Restore* (`rstrui.exe`).
- **6. Công Cụ Chuyên Sâu:** Tích hợp sẵn các tiện ích phân tích: *NVCleanstall, Custom Resolution Utility (CRU), hidusbf (ép xung chuột), DevManView, Process Explorer*.

---

## Cơ chế an toàn & Kiểm toán (v1.0.1)

SuperStrike X1 v1.0.1 áp dụng các quy chuẩn an toàn chặt chẽ:
- **Xác minh tệp 1:1 & So khớp SHA-256:** Script [`DeployPostInstall.ps1`](file:///E:/Superstrike-x1/Executables/DeployPostInstall.ps1) đối chiếu từng tệp giữa nguồn và đích. Khi dọn dẹp thư mục trùng lặp trên Desktop người dùng, script **chỉ xóa tệp mẫu trùng khớp 100% mã băm SHA-256 với bản gốc**, bảo vệ tuyệt đối mọi tệp người dùng đã chỉnh sửa hay thư mục sao lưu cá nhân (`Registry_Backup`).
- **Nhánh triển khai dự phòng không ghi đè:** Nếu Public Desktop bị lỗi phân quyền, script sẽ chuyển hướng triển khai sang User Desktop mà **không dùng `-Force` ghi đè**, giữ nguyên vẹn các tệp người dùng đang có.
- **Kiểm toán trung thực (Audit):** Script [`StrikeAudit.ps1`](file:///E:/Superstrike-x1/Executables/StrikeAudit.ps1) tự động kiểm tra trạng thái dịch vụ lõi, BCD, RAM khả dụng và xuất báo cáo JSON chi tiết tại `%ProgramData%\StrikeOS\Reports`. Hệ thống sử dụng mã thoát phân biệt (`exit 0`: thành công, `exit 10`: cảnh báo, `exit 1`: lỗi nghiêm trọng) kết hợp cơ chế `errorAction: Halt` của AME Wizard để ngăn chặn hoàn toàn tình trạng báo hoàn tất giả khi có lỗi thực tế.

---

## Gaming Runtime

Playbook tự động kiểm tra sự hiện diện của Visual C++ 2015–2022 x86/x64, DirectX Legacy June 2010 và .NET Framework 3.5; các thành phần đã có sẵn sẽ được bỏ qua. Các gói còn thiếu được tải trực tiếp từ máy chủ chính thức của Microsoft kèm xác thực chữ ký số Authenticode.

---

## Hướng dẫn cài đặt

1. Nhấn `Win + R`, gõ `winver` để xác nhận hệ điều hành thuộc danh sách hỗ trợ (`19045`, `26100` hoặc `26200`).
2. Sao lưu dữ liệu quan trọng; tạo System Restore Point trước khi chạy.
3. Tải công cụ [AME Wizard](https://ameliorated.io/) và tệp `Superstrike-x1.apbx` từ [Releases chính thức](https://github.com/nyxvergil/Superstrike-x1/releases).
4. Mở **AME Wizard** với quyền Administrator, kéo tệp `.apbx` vào giao diện và nhập mật khẩu Playbook: `malte`.
5. Lựa chọn cấu hình (**Standard** hoặc **Performance**) và kiểm tra kỹ các tùy chọn gỡ bỏ trước khi tiếp tục.
6. Trong suốt quá trình chạy, không tắt máy hoặc mở các phần mềm tối ưu khác. Khởi động lại máy tính khi nhận được thông báo hoàn tất.

---

## Tệp phát hành & Mã băm (SHA-256)

Vui lòng kiểm tra mã băm SHA-256 sau khi tải về để đảm bảo tệp nguyên bản:

| Tên tệp | Định dạng | Dung lượng | SHA-256 Checksum |
|---|:---:|:---:|---|
| **`Superstrike-x1.apbx`** | AME Playbook (Khuyên dùng) | 9.13 MB | `49456B083ED141A5A2DA9B97D99DAC272F16C2D02A3DF01E92BC36A58BC95131` |
| **`Superstrike-x1.zip`** | Mã nguồn / Lưu trữ | 10.07 MB | `364F0E120B6279A6A97C0195D5CE36E3BB6BD0B507F9FD7620EB4BABCA117F28` |

> 🔑 **Mật khẩu AME Playbook:** `malte`

---

## Báo lỗi và Đóng góp

Mọi đóng góp và phản hồi kỹ thuật đều được hoan nghênh:
- Tạo [GitHub Issue](https://github.com/nyxvergil/Superstrike-x1/issues) kèm thông tin: phiên bản Windows (`winver`), cấu hình máy, chế độ cài đặt đã chọn và tệp log tại `%ProgramData%\StrikeOS\Logs`.
- Trao đổi và nhận trợ giúp từ cộng đồng tại [Discord StrikeOS](https://discord.gg/strikeos).
- Vui lòng kiểm tra và xóa bỏ các thông tin định danh cá nhân trước khi đăng tải tệp log công khai.

---

<p align="center"><strong>SuperStrike X1 · StrikeOS</strong></p>
