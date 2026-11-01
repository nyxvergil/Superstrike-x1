<div align="center">
  <picture>
    <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/bannerstrike.png" alt="SuperStrike Banner" width="800" height="auto">
  </picture>

  <p>
    <a href="https://github.com/nyxvergil/Superstrike-x1/releases">
      <img src="https://img.shields.io/badge/Phi%C3%AAn_b%E1%BA%A3n-v1.0.1-5B21FF?style=for-the-badge&logo=windows11&logoColor=white" alt="Phiên bản v1.0.1">
    </a>
    <img src="https://img.shields.io/badge/H%E1%BB%87_%C4%91i%E1%BB%81u_h%C3%A0nh-Windows_10_%2F_11-0d0d10?style=for-the-badge&logo=windows11&logoColor=white" alt="Windows">
    <img src="https://img.shields.io/badge/Ki%E1%BA%BFn_tr%C3%BAc-AMD64-5B21FF?style=for-the-badge" alt="Kiến trúc">
    <img src="https://img.shields.io/badge/Anti--Cheat-T%C6%B0%C6%A1ng_th%C3%ADch-0d0d10?style=for-the-badge&logo=riotgames&logoColor=5B21FF" alt="Anti-Cheat">
    <a href="https://discord.gg/StrikeOS">
      <img src="https://img.shields.io/badge/Discord-StrikeOS-0d0d10?style=for-the-badge&logo=discord&logoColor=white&labelColor=5B21FF" alt="Discord">
    </a>
    <a href="https://strikeos.site">
      <img src="https://img.shields.io/badge/Trang_ch%E1%BB%A7-strikeos.site-0d0d10?style=for-the-badge&logo=cloudflare&logoColor=5B21FF" alt="Website">
    </a>
  </p>
</div>

---

<div align="center">

<table align="center" width="85%">
<tr>
<td width="65%" align="left">

<h3>Tinh chỉnh Windows cho Độ trễ thấp và Khung hình Ổn định</h3>

SuperStrike X1 là bộ kịch bản cấu hình tinh giản Windows dạng mã nguồn mở dành cho công cụ <strong>AME Wizard</strong>.

<br>

Dự án tập trung vào việc tinh giản các dịch vụ chạy ngầm không cần thiết và tối ưu cơ chế xử lý ngắt phần cứng, nhằm cải thiện độ ổn định thời gian xuất khung hình (frametime) khi chơi game:
áp dụng các tinh chỉnh kernel thực tế, cân bằng ngắt thiết bị (MSI Mode) và tích hợp sẵn công cụ hoàn tác.

<br>

Quy trình hoàn toàn mang tính <strong>tự nguyện (Opt-in)</strong>: người dùng chủ động lựa chọn những thành phần cần thiết lập và giữ lại các dịch vụ phục vụ công việc.
Windows Defender, Riot Vanguard (CFG/DEP) và cơ chế cập nhật của Windows Update được giữ nguyên vẹn.
Hệ thống chỉ cần khởi động lại một lần sau khi hoàn tất.

<br>

<strong>Độ trễ thấp · Khung hình ổn định · Tương thích Anti-Cheat · Sẵn sàng hoàn tác</strong>

</td>
<td width="35%" align="center">

<img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/playbook_cube.png" width="200" alt="SuperStrike Playbook">

</td>
</tr>
</table>

</div>

---

> [!NOTE]
> **Định hướng tinh chỉnh:** Tập trung can thiệp vào độ trễ ngắt DPC và hạn chế xung đột luồng xử lý nền. Không can thiệp ép tắt MPO và không sử dụng các thiết lập registry ép xung ảo có thể gây lỗi hiển thị.

---

## 1. Dữ liệu Đo kiểm Thực tế (Benchmark)

Thử nghiệm được thực hiện trên cùng một cấu hình phần cứng, ghi lại qua vòng lặp cố định 60 giây bằng công cụ **PresentMon** trong tựa game **GTA5VN / FiveM (`GTASVN_GameProcess.exe`)**:

<p align="center">
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/benchmark.png" width="820" alt="Dữ liệu đo kiểm thời gian xuất khung hình">
</p>

| Thông số Đo lường (PresentMon) | Windows Mặc định (Gốc) | SuperStrike X1 (Sau tinh chỉnh) | Chênh lệch Thực tế |
| :--- | :---: | :---: | :---: |
| **FPS Trung bình (Average FPS)** | 174.61 FPS | **253.61 FPS** | **+45.2%** |
| **1% Low FPS (Độ ổn định khung hình)** | 20.66 FPS | **173.88 FPS** | **+741.6%** |
| **FPS Thấp nhất (Minimum FPS)** | 16.98 FPS | **83.81 FPS** | **+393.5%** |
| **Độ lệch chuẩn Frametime (StDev)** | 32.18 ms | **27.19 ms** | **-4.99 ms** |
| **Tổng số khung hình kết xuất (60s)** | 10,478 | **15,217** | **+4,739** |
| **Số tiến trình nền khi nghỉ (Idle)** | ~160–180 | **~70–85** | Giảm ~55% |

> *Lưu ý: Kết quả trên phản ánh dữ liệu đo kiểm trong môi trường thử nghiệm cụ thể. Hiệu năng thực tế sẽ thay đổi tùy thuộc vào cấu hình phần cứng, phiên bản trình điều khiển và ứng dụng của từng máy tính.*

---

## 2. Các Nhóm Tinh chỉnh Kỹ thuật

- **Gộp tiến trình dịch vụ SvcHost:** Gom nhóm các dịch vụ nền phân tán vào các tiến trình dùng chung phù hợp, giúp giảm thiểu tần suất chuyển đổi ngữ cảnh CPU (CPU context-switching).
- **Phần cứng mạng & ngắt thiết bị:** Vô hiệu hóa các tính năng tiết kiệm điện cổng mạng (EEE, Green Ethernet) và cơ chế gom gói trễ (LSO, RSC). Cấu hình chế độ ngắt MSI (Message Signaled Interrupts) mức ưu tiên cao cho card mạng và GPU.
- **Bộ nhớ & phân trang động:** Khóa nhân hệ thống (kernel executive) trực tiếp vào RAM trên máy có từ 12GB RAM trở lên nhằm hạn chế trễ do truy xuất ổ đĩa; tự động duy trì cơ chế phân trang mặc định trên hệ thống ít RAM.
- **Tuân thủ chuẩn DirectFlip & WDDM 3.0+:** Giữ nguyên tính năng Tăng tốc GPU bằng phần cứng (HAGS) và cơ chế hiển thị DirectFlip gốc; không can thiệp ép tắt MPO.
- **Điều phối tài nguyên Windows Defender:** Duy trì tính năng bảo vệ theo thời gian thực của Defender, giới hạn mức sử dụng CPU tối đa khi quét định kỳ ở mức 15% và thêm danh sách loại trừ cho các thư mục trò chơi phổ biến.

---

## 3. Cấu hình Giao diện & Hiệu ứng

Lược bớt các hoạt ảnh chuyển động cửa sổ không cần thiết nhằm giảm tải cho bộ phận kết xuất giao diện (DWM), đồng thời vẫn bảo đảm độ nét của văn bản và trải nghiệm sử dụng hàng ngày:

<p align="center">
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/visual_effects_preset.png" width="380" alt="Cấu hình hiệu ứng giao diện">
</p>

- **Giữ lại:** Cơ chế làm mịn chữ ClearType, ảnh thu nhỏ xem trước (thumbnails) của tập tin và bóng đổ biểu tượng.
- **Lược bỏ:** Hoạt ảnh thu phóng cửa sổ, hiệu ứng trượt danh mục và bóng đổ con trỏ chuột.

---

## 4. Các Tùy chọn Trong AME Wizard

Tất cả các hộp kiểm đều ở trạng thái **không chọn theo mặc định**. Người dùng chủ động quyết định việc giữ lại hay loại bỏ:

| Trang | Danh mục | Nội dung Tùy chọn | Thiết lập Mặc định |
| :---: | :--- | :--- | :---: |
| **1** | Hồ sơ cấu hình | `Hiệu năng (Performance)` hoặc `Tiêu chuẩn (Standard)` | Hiệu năng |
| **2** | Ứng dụng tích hợp | `Microsoft Edge`, `Microsoft OneDrive`, `Xbox Game Bar` | Không chọn (Giữ lại) |
| **3** | Tính năng AI & Bảng tin | `Widgets & Tin tức`, `Copilot, Recall & Windows AI` | Không chọn (Giữ lại) |
| **4** | Giao diện hệ thống | `Tắt độ trong suốt (Transparency)`, `Menu chuột phải cổ điển (Windows 10)` | Không chọn (Giữ lại) |
| **5** | Thiết bị & Dịch vụ phụ trợ | `Chỉ mục tìm kiếm (Indexing)`, `Bluetooth`, `Dịch vụ in (Print Spooler)` | Không chọn (Giữ lại) |
| **6** | Trình duyệt Web | `Không cài đặt`, `Brave Browser`, `Google Chrome`, `Mozilla Firefox` | Tùy chọn |

---

## 5. Tự động Nhận diện Máy bàn (Desktop) & Laptop

Hệ thống tự động phát hiện dạng thiết bị trong quá trình thiết lập để áp dụng thông số quản lý nguồn phù hợp:

| Tính năng | Cấu hình cho Máy bàn (Desktop) | Cấu hình cho Laptop |
| :--- | :---: | :---: |
| **Chế độ nguồn khi cắm sạc (AC)** | Hiệu năng cao (Bỏ đỗ lõi CPU - 100% Unparked) | Cân bằng tối ưu cho tác vụ chơi game |
| **Chế độ nguồn khi dùng pin (DC)** | Không áp dụng | Cân bằng tiết kiệm pin tiêu chuẩn |
| **Tiết kiệm điện USB & D3Cold** | Tắt (Loại bỏ độ trễ phản hồi của chuột/bàn phím) | Giữ nguyên (Tránh tiêu hao pin lúc chờ) |
| **Cơ chế dựng hình đồ họa** | HAGS + Ưu tiên trực tiếp GPU rời | HAGS + Đảm bảo chuyển đổi đồ họa kép an toàn |

---

## 6. Bộ Công cụ Hoàn tác Sau Cài đặt (PostInstall)

Mọi thay đổi đều có thể bật/tắt linh hoạt thông qua các tập lệnh được đặt tại thư mục `C:\Users\Public\Desktop\PostInstall\`:

| Tập lệnh (.bat) | Chức năng thực hiện |
| :--- | :--- |
| `Toggle-Power-Plan.bat` | Chuyển đổi linh hoạt giữa các gói nguồn: Ultimate, High Performance và Balanced |
| `Toggle-Windows-Defender.bat` | Bật hoặc tắt tính năng bảo vệ theo thời gian thực của Windows Defender |
| `Toggle-Windows-Update.bat` | Bật hoặc tạm hoãn tính năng cập nhật tự động Windows Update |
| `Toggle-WiFi-Bluetooth.bat` | Khôi phục lại các dịch vụ mạng không dây Wi-Fi và kết nối Bluetooth |
| `Toggle-Print-Spooler.bat` | Khôi phục nhanh dịch vụ hỗ trợ máy in (Print Spooler) |
| `Toggle-VBS-Core-Isolation.bat` | Bật hoặc tắt tính năng Bảo mật dựa trên ảo hóa (VBS / HVCI) |
| `Toggle-MPO-HAGS.bat` | Kiểm tra trạng thái và điều chỉnh Multi-Plane Overlay (MPO) cùng tính năng HAGS |
| `DirectFlip-CPU-Hybrid.bat` | Kiểm tra trạng thái hiển thị DirectFlip và cơ chế phân phối luồng CPU |
| `Restore-Visual-Effects.bat` | Khôi phục toàn bộ hiệu ứng hình ảnh giao diện về mặc định ban đầu |

---

## 7. Hướng dẫn Cài đặt

<p align="center">
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/1.PNG" width="410" alt="SuperStrike trong AME Wizard">
  &nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/nyxvergil/Superstrike-x1/main/assest/2.PNG" width="410" alt="Lựa chọn cấu hình">
</p>

1. Tải tệp playbook `Superstrike-x1.apbx` từ mục [Releases](https://github.com/nyxvergil/Superstrike-x1/releases) và công cụ [AME Wizard Beta](https://download.ameliorated.io/AME%20Beta.zip).
2. Nhấp chuột phải vào `AME Wizard.exe`, chọn **Run as Administrator**.
3. Kéo thả tệp `Superstrike-x1.apbx` vào giao diện của AME Wizard (nhập mật khẩu giải mã: `malte` nếu có yêu cầu).
4. Xem xét và tích chọn các thành phần theo đúng nhu cầu sử dụng, sau đó nhấn **Next**.
5. Khởi động lại máy tính sau khi quy trình hoàn tất.

---

## 8. Khả năng Tương thích

### Hoạt động an toàn với các hệ thống Anti-Cheat
Playbook chỉ can thiệp vào các tầng cấu hình tiêu chuẩn của hệ điều hành, không sửa đổi các tệp tin hệ thống và tuân thủ chữ ký số driver:
- **Riot Vanguard** (VALORANT, League of Legends)
- **Easy Anti-Cheat** (Fortnite, Apex Legends, Rust)
- **BattlEye** (Rainbow Six Siege, PUBG, Destiny 2)
- **FACEIT Anti-Cheat** (Counter-Strike 2)
- **Ricochet** (Call of Duty: Warzone)

### Phiên bản Windows được hỗ trợ (Kiến trúc 64-bit / x64)

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
> 1. **Mục đích chia sẻ:** Playbook này được xây dựng và chia sẻ với mục đích nghiên cứu, hỗ trợ tối ưu hóa cấu hình Windows cho nhu cầu cá nhân.
> 2. **Sự biến thiên hiệu năng:** Dữ liệu thử nghiệm mang tính chất tham khảo. Kết quả thực tế sẽ có sự khác biệt nhất định tùy thuộc vào cấu hình phần cứng cụ thể, phiên bản BIOS/Driver, điều kiện nhiệt độ và môi trường phần mềm của từng máy tính.
> 3. **Khuyến cáo sao lưu:** Người dùng luôn được khuyến nghị chủ động tạo điểm khôi phục hệ thống (System Restore Point) hoặc sao lưu các dữ liệu quan trọng trước khi tiến hành cài đặt bất kỳ bản tinh chỉnh nào.
> 4. **Trách nhiệm người dùng:** Người dùng tự chịu trách nhiệm đối với thiết bị của mình. Tác giả không chịu trách nhiệm đối với các rủi ro mất mát dữ liệu, lỗi phần mềm hoặc các xung đột phát sinh do phần mềm của bên thứ ba trong quá trình sử dụng.

---

## Liên kết & Xác thực Tệp tin

<p align="center">
  <a href="https://strikeos.site">
    <img src="https://img.shields.io/badge/Trang_ch%E1%BB%A7-strikeos.site-5B21FF?style=flat-square&logo=googlechrome&logoColor=white" alt="Website">
  </a>
  <a href="https://discord.gg/StrikeOS">
    <img src="https://img.shields.io/badge/Discord-StrikeOS-5B21FF?style=flat-square&logo=discord&logoColor=white" alt="Discord">
  </a>
  <a href="https://github.com/nyxvergil/Superstrike-x1">
    <img src="https://img.shields.io/badge/GitHub-Superstrike--x1-0d0d10?style=flat-square&logo=github&logoColor=white" alt="GitHub">
  </a>
</p>

```text
Tên tệp: Superstrike-x1.apbx
SHA256 : 00B7EC7999CC0792D25EC5628F44AE3823ADE0B66546A1EA156EF5B74E884EA4
```

<p align="center">
  <sub>© 2026 StrikeOS · SuperStrike X1 · Windows Optimization Playbook</sub>
</p>
