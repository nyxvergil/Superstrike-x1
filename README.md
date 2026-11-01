<div align="center">
  <picture>
    <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/bannerstrike.png" alt="SuperStrike Banner" width="800" height="auto">
  </picture>

  <p>
    <a href="https://github.com/nyxvergil/Superstrike-x1/releases">
      <img src="https://img.shields.io/badge/PHI%C3%8AN%20B%E1%BA%A2N-v1.0.1-5B21FF?style=for-the-badge&logo=windows11&logoColor=white" alt="Phiên bản v1.0.1">
    </a>
    <img src="https://img.shields.io/badge/H%E1%BB%86%20%C4%90I%E1%BB%80U%20H%C3%80NH-WINDOWS%2010%20%2F%2011-0d0d10?style=for-the-badge&logo=windows11&logoColor=white" alt="Windows">
    <img src="https://img.shields.io/badge/KI%E1%BA%BEN%20TR%C3%9AC-AMD64-5B21FF?style=for-the-badge" alt="Kiến trúc">
    <img src="https://img.shields.io/badge/ANTI--CHEAT-T%C6%AF%C6%A0NG%20TH%C3%8DCH-0d0d10?style=for-the-badge&logo=riotgames&logoColor=5B21FF" alt="Anti-Cheat">
    <a href="https://discord.gg/StrikeOS">
      <img src="https://img.shields.io/badge/Discord-StrikeOS-0d0d10?style=for-the-badge&logo=discord&logoColor=white&labelColor=5B21FF" alt="Discord">
    </a>
    <a href="https://strikeos.site">
      <img src="https://img.shields.io/badge/Website-strikeos.site-0d0d10?style=for-the-badge&logo=cloudflare&logoColor=5B21FF" alt="Website">
    </a>
  </p>
</div>

---

<div align="center">

<table align="center" width="85%">
<tr>
<td width="65%" align="left">

<h3>Tối ưu hóa Windows cho Hiệu năng và Độ ổn định</h3>

SuperStrike X1 là bộ kịch bản cấu hình tinh giản Windows dạng mã nguồn mở, hoạt động thông qua nền tảng <strong>AME Wizard</strong>.

<br>

Được thiết kế nhằm mục tiêu <strong>cải thiện tính ổn định thời gian xuất khung hình (frametime) và giảm thiểu độ trễ hệ thống</strong>:
áp dụng các tinh chỉnh kernel thực tế, cân bằng ngắt phần cứng (MSI Mode) và tích hợp sẵn các tập lệnh khôi phục nguyên trạng.

<br>

Toàn bộ quy trình mang tính <strong>tự nguyện (100% opt-in)</strong>: người dùng chủ động lựa chọn thành phần cần tinh chỉnh và giữ lại các dịch vụ cần thiết.
Các cơ chế an toàn gồm Windows Defender, Riot Vanguard (CFG/DEP) và hệ thống Windows Update được duy trì hoạt động bình thường.
Hệ thống chỉ cần khởi động lại một lần sau khi hoàn tất.

<br>

<strong>Ổn định khung hình · Giảm độ trễ · Tương thích Anti-Cheat · Dễ dàng hoàn tác</strong>

</td>
<td width="35%" align="center">

<img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/playbook_cube.png" width="200" alt="SuperStrike Playbook">

</td>
</tr>
</table>

</div>

---

> [!NOTE]
> **Cam kết tính thực tế:** Không áp dụng các thiết lập registry ảo hoặc ép tắt MPO gây lỗi hiển thị. Mọi tùy chỉnh đều hướng tới việc giảm độ trễ ngắt DPC và hạn chế xung đột luồng xử lý nền.

---

## 1. Dữ liệu Đo kiểm Thực tế (Benchmark)

Thử nghiệm được thực hiện trên cùng một cấu hình phần cứng, ghi lại qua vòng lặp cố định 60 giây trong **GTA5VN / FiveM (`GTASVN_GameProcess.exe`)**:

<p align="center">
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/benchmark.png" width="820" alt="Dữ liệu đo kiểm thời gian xuất khung hình">
</p>

| Chỉ số Đo lường | Windows Mặc định (Gốc) | SuperStrike X1 (Sau tinh chỉnh) | Chênh lệch Thực tế |
| :--- | :---: | :---: | :---: |
| **FPS Trung bình (Average FPS)** | 174.61 FPS | **253.61 FPS** | **+45.2%** |
| **1% Low FPS (Chỉ số giật lag)** | 20.66 FPS | **173.88 FPS** | **+741.6%** (Khắc phục hiện tượng khựng khung hình) |
| **FPS Thấp nhất (Minimum FPS)** | 16.98 FPS | **83.81 FPS** | **+393.5%** |
| **Độ lệch Frametime (StDev)** | 32.18 ms | **27.19 ms** | **-4.99 ms** (Độ ổn định nhịp khung hình cao hơn) |
| **Tổng số khung hình (60s)** | 10,478 frames | **15,217 frames** | **+4,739 frames** |
| **Số tiến trình nền khi nghỉ (Idle)** | 160–180+ | **~70–85** | Giảm khoảng 55% |

---

## 2. Các Nhóm Tối ưu Cốt lõi

- **Gộp tiến trình dịch vụ SvcHost:** Gom nhóm hơn 160 dịch vụ nền phân tán vào các tiến trình dùng chung phù hợp, giảm thiểu tần suất chuyển đổi ngữ cảnh CPU (CPU context-switching).
- **Tối ưu phần cứng & mạng:** Vô hiệu hóa tính năng tiết kiệm điện cổng mạng (EEE, Green Ethernet) và cơ chế gom gói trễ (LSO, RSC) nhằm đẩy nhanh tốc độ phản hồi gói tin. Thiết lập chế độ ngắt MSI (Message Signaled Interrupts) mức độ ưu tiên cao cho card mạng và GPU.
- **Quản lý bộ nhớ & phân trang động:** Khóa nhân hệ thống (kernel executive) vào RAM trên các thiết bị sở hữu $\ge$ 12GB RAM nhằm hạn chế tình trạng trễ do truy xuất ổ đĩa; tự động duy trì cơ chế phân trang mặc định trên hệ thống ít RAM.
- **Tuân thủ chuẩn DirectFlip & WDDM 3.0+:** Giữ nguyên tính năng Tăng tốc GPU bằng phần cứng (HAGS) và cơ chế hiển thị DirectFlip gốc. Không áp dụng các biện pháp ép tắt MPO thiếu an toàn.
- **Điều phối tài nguyên Windows Defender:** Giữ nguyên khả năng bảo vệ theo thời gian thực nhưng giới hạn mức sử dụng CPU tối đa khi quét định kỳ ở ngưỡng 15%, đồng thời hỗ trợ loại trừ các thư mục chứa tệp nén trò chơi phổ biến.

---

## 3. Cấu hình Giao diện & Hiệu ứng

Lược bỏ các hiệu ứng cuộn và chuyển động cửa sổ không cần thiết, nhưng vẫn bảo toàn độ sắc nét của văn bản và trải nghiệm sử dụng hàng ngày:

<p align="center">
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/visual_effects_preset.png" width="380" alt="Cấu hình hiệu ứng giao diện">
</p>

*Giữ nguyên cơ chế làm mịn chữ ClearType, ảnh thu nhỏ (thumbnail) của tệp tin và đổ bóng biểu tượng. Giảm tải quá trình dựng hình của giao diện.*

---

## 4. Các Tùy chọn Trong AME Wizard

Tất cả các hộp kiểm đều ở trạng thái **không chọn theo mặc định**. Hệ thống không tự ý gỡ bỏ bất kỳ thành phần nào nếu chưa có xác nhận từ người dùng:

| Trang | Danh mục | Nội dung Tùy chọn | Thiết lập Mặc định |
| :---: | :--- | :--- | :---: |
| **1** | Hồ sơ tối ưu | `Hiệu năng (Performance)` / `Tiêu chuẩn (Standard)` | Hiệu năng |
| **2** | Ứng dụng tích hợp | `Microsoft Edge`, `Microsoft OneDrive`, `Xbox & Game Bar` | Tùy chọn chủ động (Opt-in) |
| **3** | Tính năng AI & Bảng tin | `Widgets & Tin tức`, `Copilot, Recall & Windows AI` | Tùy chọn chủ động (Opt-in) |
| **4** | Giao diện hệ thống | `Tắt độ trong suốt (Transparency)`, `Menu chuột phải cổ điển (Win 10)` | Tùy chọn chủ động (Opt-in) |
| **5** | Thiết bị & Dịch vụ phụ trợ | `Chỉ mục tìm kiếm (Indexing)`, `Bluetooth`, `Dịch vụ in (Print Spooler)`, `Bàn phím cảm ứng` | Tùy chọn chủ động (Opt-in) |
| **6** | Trình duyệt Web | `Không cài đặt`, `Brave`, `Mozilla Firefox`, `Google Chrome` | Tùy chọn (Brave có sẵn) |

---

## 5. Tự động Nhận diện Máy bàn (Desktop) & Máy tính xách tay (Laptop)

Hệ thống tự động phát hiện dạng phần cứng trong quá trình thiết lập để áp dụng thông số phù hợp:

| Tính năng | Cấu hình cho Máy bàn (Desktop) | Cấu hình cho Laptop |
| :--- | :---: | :---: |
| **Chế độ nguồn khi cắm sạc (AC)** | Hiệu năng cao (Bỏ đỗ lõi CPU - 100% Unparked) | Cân bằng tối ưu cho tác vụ chơi game |
| **Chế độ nguồn khi dùng pin (DC)** | Không áp dụng | Cân bằng tiết kiệm pin tiêu chuẩn |
| **Tiết kiệm điện USB & D3Cold** | Tắt (Loại bỏ độ trễ phản hồi của chuột/phím) | Giữ nguyên (Tránh tiêu hao pin lúc chờ) |
| **Cơ chế dựng hình đồ họa** | HAGS + Ưu tiên trực tiếp GPU rời | HAGS + Đảm bảo chuyển đổi đồ họa kép an toàn |

---

## 6. Bộ Công cụ Hoàn tác Sau Cài đặt (PostInstall)

Mọi thay đổi đều có thể bật/tắt nhanh chóng thông qua các tập lệnh tiện ích được đặt tại thư mục `C:\Users\Public\Desktop\PostInstall\`:

| Tập lệnh | Chức năng thực hiện |
| :--- | :--- |
| `Toggle-Power-Plan.bat` | Chuyển đổi linh hoạt giữa các gói nguồn: Ultimate, High Performance và Balanced |
| `Toggle-VBS-Core-Isolation.bat` | Bật hoặc tắt tính năng Bảo mật dựa trên ảo hóa (VBS / HVCI) |
| `Toggle-Windows-Defender.bat` | Bật hoặc tắt cơ chế Bảo vệ thời gian thực và Gửi mẫu phân tích đám mây |
| `Toggle-Windows-Update.bat` | Bật hoặc tạm dừng các tác vụ tự động tải bản cập nhật và tối ưu phân phối mạng |
| `Toggle-MPO-HAGS.bat` | Kiểm tra trạng thái và điều chỉnh Multi-Plane Overlay (MPO) cùng tính năng HAGS |
| `DirectFlip-CPU-Hybrid.bat` | Kiểm tra trạng thái hiển thị DirectFlip và cơ chế phân phối luồng CPU |
| `Toggle-WiFi-Bluetooth.bat` | Khôi phục nhanh các dịch vụ kết nối Wi-Fi, Bluetooth và ghép đôi thiết bị không dây |
| `Toggle-Print-Spooler.bat` | Khôi phục ngay dịch vụ hỗ trợ máy in (Print Spooler) |
| `Restore-Visual-Effects.bat` | Đưa toàn bộ hiệu ứng hình ảnh và hoạt ảnh Windows về trạng thái ban đầu |

---

## 7. Hướng dẫn Cài đặt

<p align="center">
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/1.PNG" width="410" alt="SuperStrike trong AME Wizard">
  &nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/2.PNG" width="410" alt="Lựa chọn cấu hình">
</p>

1. Tải tệp `Superstrike-x1.apbx` từ mục [Releases](https://github.com/nyxvergil/Superstrike-x1/releases) và công cụ [AME Wizard Beta](https://download.ameliorated.io/AME%20Beta.zip).
2. Nhấp chuột phải vào `AME Wizard.exe`, chọn **Run as Administrator**.
3. Kéo thả tệp `Superstrike-x1.apbx` vào giao diện của AME Wizard (nhập mật khẩu giải mã: `malte` nếu có yêu cầu).
4. Tích chọn các thành phần theo đúng nhu cầu sử dụng của bạn, sau đó nhấn **Next**.
5. Khởi động lại máy tính sau khi phần mềm báo hoàn thành.

---

## 8. Khả năng Tương thích Anti-Cheat & Phiên bản Hệ điều hành

### Hoạt động an toàn với các hệ thống Anti-Cheat
Chỉ tác động vào các tầng cấu hình tiêu chuẩn của hệ điều hành. Các cơ chế bảo vệ nhân quan trọng (CFG, DEP, xác thực chữ ký số driver) được giữ nguyên vẹn:
- **Riot Vanguard** (VALORANT, League of Legends)
- **Easy Anti-Cheat** (Fortnite, Apex Legends, Rust)
- **BattlEye** (Rainbow Six Siege, PUBG, Destiny 2)
- **FACEIT Anti-Cheat** (Counter-Strike 2)
- **Ricochet** (Call of Duty: Warzone)

### Phiên bản Windows được hỗ trợ (Kiến trúc AMD64 / x64)

<p align="center">
  <img src="https://img.shields.io/badge/Windows%2010-22H2%20(Build%2019045)-5B21FF?style=flat-square&logo=windows11&logoColor=white" alt="Windows 10 22H2">
  <img src="https://img.shields.io/badge/Windows%2011-23H2%20(Build%2022631)-5B21FF?style=flat-square&logo=windows11&logoColor=white" alt="Windows 11 23H2">
  <img src="https://img.shields.io/badge/Windows%2011-24H2%20(Build%2026100)-5B21FF?style=flat-square&logo=windows11&logoColor=white" alt="Windows 11 24H2">
  <img src="https://img.shields.io/badge/Windows%2011-25H2%20(Build%2026200)-5B21FF?style=flat-square&logo=windows11&logoColor=white" alt="Windows 11 25H2">
</p>

---

## 9. Câu hỏi Thường gặp (FAQ)

<details>
<summary><strong>Vì sao VBS (Bảo mật Dựa trên Ảo hóa) được đề xuất tắt trong cấu hình chơi game?</strong></summary>

Cơ chế Tính toàn vẹn bộ nhớ (HVCI) và VBS vận hành một lớp ảo hóa nền của CPU, có thể làm giảm từ 5% đến 15% mức 1% Low FPS trong các tựa game thi đấu phụ thuộc nhiều vào CPU. Tính năng này được tắt để tối ưu hóa độ mượt khung hình, nhưng bạn hoàn toàn có thể kích hoạt lại bất kỳ lúc nào bằng tệp `Toggle-VBS-Core-Isolation.bat`.
</details>

<details>
<summary><strong>SuperStrike có làm hỏng tính năng cập nhật Windows Update không?</strong></summary>

Không. Cơ chế dịch vụ nền (servicing stack) của Windows vẫn được giữ lại. Nếu muốn chủ động bật hoặc tạm hoãn các bản cập nhật driver tự động, bạn có thể sử dụng công cụ `Toggle-Windows-Update.bat` trong thư mục PostInstall.
</details>

<details>
<summary><strong>Nếu tôi cần dùng lại Bluetooth, Wi-Fi hoặc Máy in thì xử lý thế nào?</strong></summary>

Trong bước cài đặt, bạn chỉ cần giữ nguyên trạng thái không chọn cho các mục này. Trường hợp đã lỡ tắt, bạn chỉ cần chạy tệp `Toggle-WiFi-Bluetooth.bat` hoặc `Toggle-Print-Spooler.bat` trong thư mục PostInstall ngoài màn hình Desktop để kích hoạt lại tức thì.
</details>

---

## 10. Tuyên bố Miễn trừ Trách nhiệm (Disclaimer)

> [!IMPORTANT]
> **Vui lòng đọc kỹ trước khi sử dụng:**
> 1. **Mục đích chia sẻ:** Playbook này được xây dựng và chia sẻ với mục đích nghiên cứu, tối ưu hóa trải nghiệm cá nhân dựa trên các thông số đo lường thực tế.
> 2. **Sự biến thiên hiệu năng:** Kết quả kiểm thử thực tế có thể có sự khác biệt nhất định phụ thuộc vào cấu hình phần cứng cụ thể, phiên bản BIOS/Driver, điều kiện nhiệt độ và môi trường phần mềm của từng hệ thống.
> 3. **Khuyến cáo sao lưu:** Mặc dù bộ tinh chỉnh đã được thử nghiệm kỹ lưỡng về độ ổn định, người dùng luôn được khuyến nghị chủ động sao lưu các dữ liệu quan trọng hoặc tạo điểm khôi phục hệ thống (System Restore Point) trước khi tiến hành can thiệp sâu vào hệ điều hành.
> 4. **Trách nhiệm người dùng:** Người dùng hoàn toàn tự chịu trách nhiệm đối với các rủi ro phát sinh trong quá trình vận hành thiết bị cá nhân hoặc xung đột không tương thích do các phần mềm bên thứ ba gây ra.

---

## Liên kết & Xác thực Tệp tin

<p align="center">
  <a href="https://strikeos.site">
    <img src="https://img.shields.io/badge/Website-strikeos.site-5B21FF?style=flat-square&logo=googlechrome&logoColor=white" alt="Website">
  </a>
  <a href="https://discord.gg/StrikeOS">
    <img src="https://img.shields.io/badge/Discord-StrikeOS-5B21FF?style=flat-square&logo=discord&logoColor=white" alt="Discord">
  </a>
  <a href="https://github.com/nyxvergil/Superstrike-x1">
    <img src="https://img.shields.io/badge/GitHub-Superstrike--x1-0d0d10?style=flat-square&logo=github&logoColor=white" alt="GitHub">
  </a>
</p>

```
SHA256: 00B7EC7999CC0792D25EC5628F44AE3823ADE0B66546A1EA156EF5B74E884EA4  Superstrike-x1.apbx
```

<p align="center">
  <sub>© 2026 StrikeOS · SuperStrike X1 · Kiến trúc Tối ưu hóa Thực nghiệm</sub>
</p>
