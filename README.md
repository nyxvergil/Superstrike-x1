<p align="center">
  <a href="https://github.com/nyxvergil/Superstrike-x1">
    <img src="./strike-logo.png" alt="SuperStrike X1" width="720">
  </a>
</p>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/Phiên_bản-v1.0.1-5B21FF?style=for-the-badge">
  <img alt="Windows" src="https://img.shields.io/badge/Windows-10_%7C_11_(x64)-0078D4?style=for-the-badge&logo=windows11&logoColor=white">
  <img alt="AME Playbook" src="https://img.shields.io/badge/AME-Playbook-202020?style=for-the-badge">
  <img alt="Mã nguồn mở" src="https://img.shields.io/badge/Mã_nguồn-Cộng_đồng-10B981?style=for-the-badge">
</p>

<p align="center">
  <img alt="Bản dựng hỗ trợ" src="https://img.shields.io/badge/Build-19045_%7C_26100_%7C_26200-2563EB?style=flat-square">
  <img alt="Kiến trúc" src="https://img.shields.io/badge/Kiến_trúc-x64-6D28D9?style=flat-square">
  <img alt="Chế độ" src="https://img.shields.io/badge/Chế_độ-Standard_%7C_Performance-E11D48?style=flat-square">
</p>

<p align="center">
  <strong>Giải pháp tinh gọn Windows hướng đến độ trễ thấp và tính ổn định, bảo toàn hệ thống bảo mật cốt lõi.</strong>
</p>

<p align="center">
  <a href="https://github.com/nyxvergil/Superstrike-x1">Mã nguồn</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/releases">Tải bản phát hành</a> ·
  <a href="#-hướng-dẫn-cài-đặt">Hướng dẫn cài đặt</a> ·
  <a href="#-khuyến-cáo--giới-hạn-kỹ-thuật">Khuyến cáo</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/issues">Đóng góp ý kiến & Báo lỗi</a>
</p>

---

## 📌 Giới thiệu dự án

**SuperStrike X1** là một Playbook nguồn mở được thiết kế để thực thi thông qua [AME Wizard](https://ameliorated.io/) trực tiếp trên các bản cài đặt Windows 10 và Windows 11 nguyên bản. 

> [!NOTE]
> Đây **không phải là bản Windows tùy biến sẵn (Custom ISO)**. Dự án can thiệp có kiểm soát vào dịch vụ, tác vụ và cấu hình hệ thống trên chính hệ điều hành hiện tại của bạn, không can thiệp phá vỡ cấu trúc servicing gốc của Microsoft.

Mục tiêu trọng tâm của dự án là **cải thiện độ phản hồi thời gian thực (real-time responsiveness), ổn định nhịp khung hình (frametime consistency) và giảm tải tài nguyên nhàn rỗi**, nhưng kiên định giữ vững nguyên tắc: **bảo toàn các thành phần bảo mật cốt lõi (Windows Defender, DEP, Secure Boot) để duy trì khả năng tương thích cao nhất với các hệ thống phần mềm công việc và Anti-cheat hiện đại.**

---

## 🎯 Định hướng và Nguyên tắc kỹ thuật

Dự án được xây dựng dựa trên 4 nguyên tắc kỹ thuật minh bạch:

1. **Dựa trên dữ liệu và tài liệu kỹ thuật xác thực:**
   Không áp dụng các mẹo Registry "truyền miệng" không rõ cơ chế. Mọi thay đổi đều được tham chiếu từ tài liệu kỹ thuật của Microsoft, whitepaper của các nhà sản xuất phần cứng (Intel, AMD, NVIDIA) và kiểm chứng thực tế qua công cụ giám sát chuyên dụng (Windows Performance Toolkit, LatencyMon).
2. **Ưu tiên sự ổn định lâu dài:**
   Nói không với việc gọt đẽo dịch vụ cực đoan nhằm mục đích "khoe" số tiến trình cực thấp (40–50 tiến trình) để rồi gây lỗi crash phần mềm đồ họa, âm thanh, hay chặn các ứng dụng phổ biến (NVIDIA App, Discord, Steam, Game Bar).
3. **Phân bổ cấu hình theo phần cứng:**
   Hệ thống tự động phân loại máy tính để bàn (Desktop) và máy tính xách tay (Laptop) nhằm áp dụng chính sách năng lượng phù hợp — tuyệt đối không tắt các tính năng quản lý nhiệt/pin trên Laptop để tránh hiện tượng quá nhiệt hay suy giảm tuổi thọ pin.
4. **Cầu thị và liên tục hoàn thiện:**
   Dự án luôn ghi nhận mọi phản hồi từ cộng đồng. Mỗi báo cáo lỗi kỹ thuật đều được đối soát, phân tích nguyên nhân gốc rễ (root cause) và cập nhật minh bạch trong nhật ký phát hành.

---

## 💻 Hệ điều hành hỗ trợ

| Hệ điều hành | Phiên bản | Bản dựng (Build) mục tiêu | Tình trạng hỗ trợ |
|:---|:---:|:---:|:---:|
| **Windows 10 64-bit** | 22H2 | `19045` (từ .3803 trở lên) | Hỗ trợ chính thức |
| **Windows 11 64-bit** | 24H2 | `26100` | Hỗ trợ chính thức |
| **Windows 11 64-bit** | 25H2 | `26200` | Thử nghiệm có chọn lọc |

> [!IMPORTANT]
> Khuyến nghị sử dụng trên các bản cài đặt Windows x64 chính thức, nguyên bản tải từ Microsoft. Các bản Windows đã qua can thiệp sâu trước đó (Ghost, Lite, ISO rút gọn bên thứ ba) có thể đã bị khuyết thiếu các gói servicing nền tảng, khiến quá trình cài đặt qua AME Wizard phát sinh lỗi dừng.

---

## ⚙️ Các chế độ cấu hình (Profiles)

Trong giao diện thiết lập của AME Wizard, người dùng chủ động lựa chọn giữa 2 chế độ:

### 1. Standard Profile
*Phù hợp cho máy tính làm việc tổng hợp, học tập và giải trí hằng ngày:*
- Gỡ bỏ các ứng dụng rác được cài sẵn (Bloatware) và vô hiệu hóa các luồng thu thập dữ liệu chẩn đoán từ xa (Diagnostic Telemetry).
- Tắt các tác vụ bảo trì tự động chạy ngầm trong giờ hoạt động nhằm giảm thiểu giật lag chu kỳ CPU.
- Giữ nguyên cấu hình năng lượng mặc định của Windows, không can thiệp sâu vào driver hay cơ chế mạng.

### 2. Performance Profile
*Dành riêng cho máy tính chơi game và các tác vụ đòi hỏi độ trễ xử lý thấp:*
- Bao gồm toàn bộ tinh chỉnh an toàn của **Standard Profile**.
- **Đồng bộ xung nhịp phần cứng (Hardware TSC):** Cấu hình BCD với `disabledynamictick yes` và `tscsyncpolicy enhanced`, không ép bật HPET ảo (`useplatformclock`) nhằm tận dụng bộ đếm Invariant TSC trực tiếp của CPU, hạn chế hiện tượng giật khung hình siêu nhỏ (micro-stutter).
- **Hỗ trợ định thời gian phản hồi (Timer Resolution):** Tích hợp dịch vụ quản lý định thời `StrikeTimerResolution` duy trì tần suất quét hệ thống ở mức 0.5ms, giúp tín hiệu chuột và bàn phím phản hồi nhạy bén và đều đặn hơn.
- **Tối ưu hóa ngắt thiết bị (MSI Mode):** Tự động chuyển đổi chế độ ngắt dòng Message Signaled Interrupts cho GPU và Card mạng PCIe tương thích, giảm thiểu hiện tượng xung đột hàng đợi IRQ.
- **Đồ họa & Hiển thị:** Kích hoạt Hardware-accelerated GPU Scheduling (HAGS) và mở khóa cơ chế trình chiếu DirectX Flip Model (`SwapEffectUpgradeEnable = 1`), giúp chế độ cửa sổ/không viền có hiệu năng tiệm cận chế độ toàn màn hình độc quyền.
- **Tối ưu hóa hệ thống tệp NTFS:** Tắt cập nhật dấu vết thời gian truy cập (`disablelastaccess 1`), tắt định dạng tên tệp cổ điển 8.3, và thu hồi phân vùng ẩn `Reserved Storage` nhằm giải phóng dung lượng đĩa và giảm thiểu hao mòn ổ cứng SSD.
- **Tối ưu mạng TCP độ trễ thấp:** Tinh chỉnh tần suất phản hồi gói tin (`TcpAckFrequency = 1`, `TcpDelAckTicks = 0`) giúp giảm độ biến động ping (jitter) trong các tựa game thi đấu trực tuyến.
- **Bảo toàn mạng cá nhân:** Không tự ý thực hiện đặt lại mạng (Network Reset) trong quá trình cài đặt tự động, bảo vệ toàn vẹn cấu hình IP tĩnh và DNS của người dùng.

---

## 🎛️ Tùy chọn độc lập trong Wizard

Để tôn trọng quyền kiểm soát của người dùng, các thành phần sau được đưa về trạng thái **Mặc định KHÔNG chọn** (`IsChecked="false"`):

- **OneDrive:** Chỉ gỡ bỏ khi bạn chủ động tích chọn.
- **Xbox & Game Bar:** Chỉ gỡ bỏ khi bạn không có nhu cầu sử dụng Game Pass, ghi hình Xbox DVR hoặc tính năng liên kết tài khoản Xbox.
- **Windows Search Indexing:** Mặc định giữ nguyên dịch vụ tìm kiếm; chỉ tắt khi bạn thực sự muốn tiết kiệm tối đa tài nguyên đĩa trên các máy cấu hình hạn chế.
- **Bluetooth & Dịch vụ in ấn:** Chỉ can thiệp khi người dùng xác nhận không sử dụng các thiết bị ngoại vi này.
- **Trình duyệt Web:** Mặc định không cài đặt thêm. Khi người dùng lựa chọn (Brave, Chrome, Firefox), trình cài đặt sẽ tải trực tiếp gói sạch từ máy chủ chính thức của nhà phát hành.

---

## 🧰 Hộp công cụ hậu cài đặt (Post-Install Toolbox)

Sau khi hoàn tất, một thư mục công cụ tiện ích sẽ được triển khai trực tiếp ngoài Desktop để người dùng dễ dàng quản trị:

* **Quản trị trung tâm (`Control Panel.bat`):** Menu điều khiển tổng hợp để xem trạng thái và bật/tắt nhanh các tính năng thường dùng.
* **Bộ phận Khắc phục sự cố:** 
  - Khôi phục nhanh dịch vụ Máy in, Bluetooth, Wi-Fi.
  - Sửa lỗi gõ tiếng Việt (UniKey / EVKey).
  - Tiện ích khởi động trực tiếp vào UEFI BIOS 1-click.
  - Script khắc phục lỗi khởi chạy của NVIDIA App ([`Sua-Loi-NVIDIA-App.bat`](file:///E:/Superstrike-x1/PostInstall/5.%20Khac%20Phuc%20Su%20Co/Sua-Loi-NVIDIA-App.bat)).
* **Sao lưu & Khôi phục (`Backup.bat` / `Restore.bat`):** Sao lưu cấu hình Registry, BCD và tích hợp trực tiếp Windows System Restore (`rstrui.exe`).
* **An toàn dữ liệu:** Trình triển khai Post-Install sử dụng cơ chế đối chiếu mã băm SHA-256; chỉ dọn dẹp các tệp mẫu trùng lặp và bảo toàn 100% mọi tệp tùy chỉnh hay bản sao lưu cá nhân của bạn.

---

## 🚀 Hướng dẫn cài đặt

1. **Chuẩn bị:** Nhấn tổ hợp phím `Win + R`, nhập `winver` để xác nhận máy tính đang ở bản dựng Windows phù hợp (`19045`, `26100` hoặc `26200`).
2. **Sao lưu:** Tạo điểm khôi phục hệ thống (System Restore Point) hoặc sao lưu dữ liệu quan trọng trước khi tiến hành.
3. **Tải về:** Tải gói phát hành `Superstrike-x1.apbx` và phần mềm [AME Wizard](https://ameliorated.io/) từ nguồn chính thức.
4. **Thực thi:** Kéo thả tệp `.apbx` vào AME Wizard, nhập mật khẩu mở khóa: `malte`.
5. **Cấu hình:** Chọn chế độ phù hợp (**Standard** hoặc **Performance**), tích chọn các mục mong muốn và làm theo hướng dẫn trên màn hình.
6. **Hoàn tất:** Sau khi AME Wizard báo hoàn tất, **khởi động lại máy tính** để các cấu hình phần cứng, driver và dịch vụ hệ thống được kích hoạt đầy đủ.

---

## 📦 Tệp phát hành & Mã băm xác thực (SHA-256)

Người dùng nên kiểm tra mã băm SHA-256 của tệp đã tải về bằng lệnh `Get-FileHash <đường-dẫn-tệp>` trên PowerShell trước khi sử dụng:

| Tên tệp | Định dạng | Dung lượng | SHA-256 Checksum |
|:---|:---:|:---:|:---|
| **`Superstrike-x1.apbx`** | AME Playbook (Khuyên dùng) | 9.13 MB | `22EACAF72039FE52961A22E775AB4CE3EE7BCFA1D42208408C66CB81E62E9107` |
| **`SHA256SUMS.txt`** | Bảng kiểm tra mã băm toàn bộ tệp | < 1 KB | [Xem SHA256SUMS.txt](./SHA256SUMS.txt) |

> 🔑 **Mật khẩu AME Playbook:** `malte`

---

## ⚠️ Khuyến cáo & Giới hạn kỹ thuật

- **Không cam đoan số liệu ảo:** Dự án không đưa ra các tuyên bố phóng đại về tỷ lệ tăng FPS hay các con số cố định. Hiệu năng thực tế phụ thuộc trực tiếp vào năng lực phần cứng (CPU, GPU, RAM, SSD), phiên bản driver và kiến trúc của từng trò chơi.
- **Cung cấp theo nguyên tắc "Nguyên trạng" (AS IS):** Mặc dù các tinh chỉnh được kiểm thử kỹ lưỡng, việc thay đổi sâu cấu hình hệ thống luôn tiềm ẩn rủi ro phát sinh xung đột với một số phần mềm chuyên biệt. Người dùng nên hiểu rõ các thay đổi và tự chịu trách nhiệm khi quyết định áp dụng.
- **Môi trường sử dụng:** Dự án được định hướng cho máy tính cá nhân và chơi game. Không khuyến nghị áp dụng trên máy chủ (Server), máy trạm làm việc đồ họa/dữ liệu quan trọng hoặc máy tính doanh nghiệp quản lý qua Domain/MDM.

---

## 🤝 Đóng góp ý kiến & Báo lỗi

Chúng tôi rất trân trọng sự đóng góp, phản hồi chân thành và các ý kiến xây dựng từ cộng đồng để dự án ngày một hoàn thiện và an toàn hơn:

- **Báo lỗi kỹ thuật:** Vui lòng tạo [GitHub Issue](https://github.com/nyxvergil/Superstrike-x1/issues) kèm theo mô tả chi tiết: phiên bản Windows (`winver`), cấu hình phần cứng, nhật ký lỗi (log file tại `%ProgramData%\StrikeOS\Logs` hoặc nhật ký AME Wizard).
- **Thảo luận & Góp ý:** Tham gia trao đổi kỹ thuật tại [GitHub Discussions](https://github.com/nyxvergil/Superstrike-x1/discussions) hoặc liên hệ qua cộng đồng [Discord](https://discord.gg/strikeos).
- *Lưu ý:* Vui lòng kiểm tra và che/xóa các thông tin cá nhân nhạy cảm (Product Key, tên tài khoản riêng, token) trước khi đính kèm log công khai.

---

<p align="center">
  <strong>SuperStrike X1 · Được phát triển và hoàn thiện cùng cộng đồng.</strong>
</p>
