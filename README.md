<p align="center">
  <a href="https://strikeos.site">
    <img src="./strike-logo.png" alt="StrikeOS" width="760">
  </a>
</p>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/VERSION-2.0.17-5B21FF?style=for-the-badge">
  <img alt="Windows" src="https://img.shields.io/badge/WINDOWS-10%20%7C%2011-0078D4?style=for-the-badge&logo=windows11&logoColor=white">
  <img alt="AME Playbook" src="https://img.shields.io/badge/AME-PLAYBOOK-202020?style=for-the-badge">
  <img alt="Defender retained" src="https://img.shields.io/badge/DEFENDER-RETAINED-16A34A?style=for-the-badge&logo=windowsdefender&logoColor=white">
  <a href="./LICENSE"><img alt="License" src="https://img.shields.io/badge/LICENSE-MIT-4B5563?style=for-the-badge"></a>
</p>

<p align="center">
  <img alt="Supported builds" src="https://img.shields.io/badge/BUILD-19045%20%7C%2026100%20%7C%2026200-2563EB?style=flat-square">
  <img alt="Architecture" src="https://img.shields.io/badge/ARCH-x64-6D28D9?style=flat-square">
  <img alt="Profiles" src="https://img.shields.io/badge/PROFILE-STANDARD%20%7C%20PERFORMANCE-E11D48?style=flat-square">
</p>

<p align="center"><strong>Tinh gọn để chơi game. Giữ lại những gì Windows và Anti-cheat thực sự cần.</strong></p>

<p align="center">
  <a href="https://strikeos.site">🌐 Website</a>
  •
  <a href="https://discord.gg/strikeos">💬 Discord</a>
  •
  <a href="#-cài-đặt">📖 Cài đặt</a>
  •
  <a href="#-báo-lỗi">🛠️ Báo lỗi</a>
</p>

## 🎮 Giới thiệu

SuperStrike X1 là Playbook tối ưu Windows dành cho máy chơi game. Dự án tập trung giảm hoạt động nền, cải thiện Latency, giữ Frame Time ổn định và hạn chế ảnh hưởng đến FPS, 1% Low và 0.1% Low.

Playbook áp dụng trực tiếp trên Windows đang sử dụng, không phải bản Windows tùy chỉnh và không yêu cầu cài lại hệ điều hành.

## 🪟 Hệ điều hành hỗ trợ

| Hệ điều hành | Phiên bản | Build |
|---|---:|---:|
| Windows 10 64-bit | 22H2 | `19045` |
| Windows 11 64-bit | 24H2 | `26100` |
| Windows 11 64-bit | 25H2 | `26200` |

Build ngoài danh sách sẽ bị từ chối để tránh áp dụng sai thiết lập.

## ✨ Điểm chính

- Tinh gọn ứng dụng, dịch vụ và tác vụ nền không cần thiết.
- Giảm hoạt động thu thập dữ liệu và nội dung quảng bá của Windows.
- Tối ưu phản hồi hệ thống, mạng, nguồn điện và phần cứng.
- Giữ Windows Defender, Firewall, DEP, Secure Boot và các thành phần bảo mật cốt lõi.
- Không vô hiệu hóa dịch vụ của Vanguard, Easy Anti-Cheat, BattlEye hoặc EA AntiCheat.
- Không kèm Toolbox, phần mềm quảng cáo hoặc gói Post-install.
- Hỗ trợ cài Brave, Firefox hoặc Chrome theo lựa chọn.

## ⚙️ Chế độ

### 🛡️ Standard

Cấu hình mặc định, cân bằng giữa tinh gọn, ổn định và tương thích. Phù hợp với phần lớn máy tính.

### 🚀 Performance

Bao gồm Standard và bổ sung TRIM, RSS, TCP Auto-Tuning, thiết lập Card mạng, Power Plan, Core Parking, HAGS, MSI Mode, HPET, Timer Resolution và đặt lại Winsock/IP.

Performance có thể cho kết quả khác nhau trên từng cấu hình. Hãy đo FPS, 1% Low, 0.1% Low và Frame Time trước khi quyết định sử dụng lâu dài.

## 🧩 Lựa chọn bổ sung

- Gỡ OneDrive.
- Gỡ Xbox và Game Bar.
- Tắt Windows Search.
- Tắt Bluetooth.
- Tắt dịch vụ in và quét tài liệu.
- Tắt cảm ứng, bút và máy tính bảng.
- Cài một trình duyệt được chọn.

Chỉ tắt nhóm phần cứng khi máy không sử dụng thiết bị tương ứng.

## 📦 Gaming Runtime

Playbook kiểm tra Visual C++ 2015–2022 x86/x64, DirectX Legacy và .NET Framework 3.5. Thành phần đã có sẽ được bỏ qua; thành phần còn thiếu chỉ được cài từ nguồn Microsoft có chữ ký hợp lệ.

> [!NOTE]
> Nếu nguồn tải, TLS hoặc `sources\sxs` không khả dụng, Runtime sẽ được ghi là `Unavailable` hoặc `SkippedNoSource`. Playbook vẫn tiếp tục và không báo cài thành công giả.

## 📖 Cài đặt

> [!CAUTION]
> Hãy sao lưu dữ liệu quan trọng hoặc tạo Snapshot trước khi chạy. Không tắt máy, thoát AME Wizard hoặc chạy thêm công cụ tối ưu trong lúc Playbook đang áp dụng.

1. Tải tệp `.apbx` mới nhất từ **Releases**.
2. Mở **AME Wizard**, sau đó kéo thả tệp `.apbx` vào cửa sổ ứng dụng.
3. Chọn **Standard** hoặc **Performance** cùng các mục cần dùng.
4. Xác nhận và chờ Playbook hoàn tất.
5. Khởi động lại Windows, chờ 10–15 phút rồi mới đo Process, RAM và hiệu năng.

## ⚠️ Lưu ý

- Không chạy đồng thời Windows Update, DISM, trình cài Driver hoặc công cụ tối ưu khác.
- Một số thay đổi chỉ có hiệu lực sau khi khởi động lại.
- Winsock và IP chỉ được đặt lại trong chế độ Performance.
- Số Process, RAM và hiệu năng phụ thuộc phần cứng, Driver, Edition và phần mềm đang cài.
- Nên thử trên máy ảo hoặc Windows mới trước khi dùng trên máy chính.

## 🛠️ Báo lỗi

> [!TIP]
> Gửi Log đầy đủ sẽ giúp xác định đúng Action gây lỗi. Không cắt riêng dòng cuối vì thường thiếu nguyên nhân ban đầu.

Khi tạo Issue, hãy gửi:

- Phiên bản, Edition và Build Windows.
- Chế độ đã chọn và các Checkbox đã đánh dấu.
- Toàn bộ Log của AME Wizard.
- Báo cáo Post-boot nếu lỗi liên quan đến Process, RAM hoặc dịch vụ.
- Cấu hình phần cứng chính và thông tin máy thật hoặc máy ảo.

Không đăng mật khẩu, Token, khóa sản phẩm hoặc thông tin cá nhân lên Issue công khai.

---

<p align="center">
  <strong>SuperStrike X1</strong><br>
  Build for performance by StrikeOS.
</p>
