<p align="center">
  <a href="https://strikeos.site">
    <img src="./strike-logo.png" alt="StrikeOS" width="760">
  </a>
</p>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/VERSION-2.0.17-5B21FF?style=for-the-badge">
  <img alt="Windows" src="https://img.shields.io/badge/WINDOWS-10%20%7C%2011-0078D4?style=for-the-badge">
  <img alt="AME Playbook" src="https://img.shields.io/badge/AME-PLAYBOOK-202020?style=for-the-badge">
  <img alt="Architecture" src="https://img.shields.io/badge/ARCH-x64-6D28D9?style=for-the-badge">
</p>

<p align="center">
  <strong>Tinh gọn Windows cho máy chơi game.</strong>
</p>

<p align="center">
  <a href="https://strikeos.site">🌐 Website</a>
  ·
  <a href="https://discord.gg/strikeos">💬 Discord</a>
</p>

## 🎮 SuperStrike X1 là gì?

SuperStrike X1 là Playbook chạy bằng AME Wizard, áp dụng các thay đổi trực tiếp lên Windows đang dùng. Bạn không cần cài lại Windows để sử dụng.

Tôi làm dự án này để giảm những thứ chạy nền không cần đến trên máy chơi game. Mục tiêu là bớt hoạt động nền và cải thiện độ phản hồi, có theo dõi FPS, 1% Low, 0.1% Low và Frame Time khi kiểm thử.

Process thấp là một chỉ số để theo dõi. Nó không tự chứng minh rằng game sẽ chạy nhanh hơn. Tôi cũng không đặt ra một con số FPS hay mức RAM mà mọi máy đều phải đạt.

## 🪟 Windows được hỗ trợ

| Hệ điều hành | Phiên bản | Build |
|---|---|---|
| Windows 10 x64 | 22H2 | `19045` |
| Windows 11 x64 | 24H2 | `26100` |
| Windows 11 x64 | 25H2 | `26200` |

Playbook kiểm tra Build trước khi chạy. Các Build ngoài danh sách sẽ bị từ chối.

Danh sách hỗ trợ không có nghĩa mọi Edition, Driver và cấu hình phần cứng đều đã được kiểm thử.

## 🔧 Playbook thay đổi những gì?

- Gỡ bớt ứng dụng và thành phần Windows không cần dùng.
- Điều chỉnh dịch vụ và Scheduled Task để giảm hoạt động nền.
- Giảm thu thập dữ liệu, quảng cáo và nội dung đề xuất của Windows.
- Điều chỉnh một số thiết lập hệ thống, mạng, nguồn điện và phần cứng.
- Kiểm tra và cài Runtime còn thiếu.
- Cài Brave, Firefox hoặc Chrome nếu bạn chọn.

Windows Defender và Firewall được giữ lại. Playbook không chủ động vô hiệu hóa dịch vụ của Vanguard, Easy Anti-Cheat, BattlEye hoặc EA AntiCheat.

Điều đó không phải cam kết tương thích với mọi game hay mọi bản cập nhật Anti-cheat. Nếu gặp lỗi, hãy gửi Log kèm tên game và cấu hình máy.

## ⚙️ Standard và Performance

| Chế độ | Nội dung |
|---|---|
| **Standard** | Các thay đổi cơ bản về Debloat và hoạt động nền. Đây là chế độ tôi chọn làm mặc định. |
| **Performance** | Bao gồm Standard, thêm các thiết lập về mạng, nguồn điện và phần cứng được liệt kê bên dưới. |

Performance có thêm TRIM, RSS, TCP Auto-Tuning, thiết lập Card mạng, Power Plan, Core Parking, HAGS, MSI Mode, HPET, Timer Resolution và đặt lại Winsock/IP. Một số mục phụ thuộc vào phần cứng và trạng thái hệ thống.

> [!WARNING]
> Performance không mặc nhiên nhanh hơn Standard. Các thay đổi về HPET, Timer, nguồn điện hoặc mạng có thể cho kết quả ngược lại trên một số máy. Chế độ này có sử dụng tiện ích Timer Resolution chạy nền và đặt lại cấu hình Winsock/IP.

Nếu chọn Performance, hãy đo cùng một game, cùng thiết lập và cùng điều kiện trước và sau khi áp dụng. Tôi ưu tiên kết quả đo thực tế hơn số lượng Tweak đã bật.

## 🧩 Các mục có thể chọn

- Gỡ OneDrive.
- Gỡ Xbox và Game Bar.
- Tắt Windows Search indexing.
- Tắt dịch vụ Bluetooth.
- Tắt dịch vụ in và quét tài liệu.
- Tắt dịch vụ cảm ứng, bút và máy tính bảng.
- Cài một trình duyệt.

Đọc từng mục trước khi chọn. Nếu còn dùng Bluetooth, máy in, cảm ứng hoặc Xbox/Game Bar, hãy giữ lại chức năng đó. Sao lưu những tệp OneDrive cần dùng về máy trước khi gỡ.

## 📦 Runtime

Playbook kiểm tra các thành phần sau:

- Visual C++ 2015–2022 x86 và x64.
- DirectX Legacy.
- .NET Framework 3.5.

Thành phần đã có sẽ được bỏ qua. Thành phần còn thiếu được cài khi có nguồn phù hợp.

> [!NOTE]
> Nếu không tải được hoặc thiếu nguồn cài đặt, Log sẽ ghi `Unavailable` hoặc `SkippedNoSource`. Playbook có thể tiếp tục, nhưng Runtime đó vẫn chưa được cài. Hãy kiểm tra Log nếu game còn báo thiếu thư viện.

## 📖 Cài đặt

Bạn cần Windows thuộc danh sách hỗ trợ, tài khoản quản trị viên, AME Wizard và kết nối Internet. Nếu dùng Laptop, hãy cắm sạc.

> [!CAUTION]
> Sao lưu trước khi chạy. Với máy ảo, hãy tạo Snapshot. Với máy thật, bản sao lưu hệ thống sẽ hữu ích khi cần quay lại trạng thái trước đó.

1. Tải tệp `.apbx` trong mục **Releases** của repository này.
2. Mở AME Wizard và kéo thả tệp vào cửa sổ ứng dụng.
3. Chọn Standard hoặc Performance, sau đó chọn những chức năng bạn muốn gỡ hoặc tắt.
4. Làm theo hướng dẫn và chờ quá trình hoàn tất.
5. Khởi động lại Windows.

Trong lúc chạy, không mở thêm công cụ tối ưu, trình cài Driver, DISM hoặc Windows Update. Không tắt máy giữa chừng.

Sau khi khởi động lại, chờ khoảng 10–15 phút để các tác vụ sau khởi động ổn định rồi hãy đo Process, RAM và hiệu năng.

## ↩️ Quay lại cấu hình cũ

Hiện không có nút hoàn tác toàn bộ Playbook.

Một số thiết lập có thể chỉnh lại, nhưng ứng dụng hoặc thành phần đã gỡ có thể cần cài lại từ nguồn Windows. Nếu muốn trở về đúng trạng thái trước khi chạy, hãy khôi phục bản sao lưu hệ thống hoặc Snapshot đã tạo.

## 🛠️ Báo lỗi

Tạo Issue và gửi các thông tin sau:

- Phiên bản Playbook hoặc tên tệp `.apbx`.
- Phiên bản, Edition và Build Windows.
- Chế độ đã chọn cùng các tùy chọn đã đánh dấu.
- Log đầy đủ của AME Wizard.
- Cấu hình máy và cho biết bạn dùng máy thật hay máy ảo.
- Báo cáo Post-boot nếu vấn đề liên quan đến Process, RAM hoặc dịch vụ.

Nếu lỗi xuất hiện trong game, ghi thêm tên game, Anti-cheat và cách tái hiện.

> [!TIP]
> Đừng chỉ gửi dòng “Playbook halted” cuối cùng. Nguyên nhân thường nằm ở các dòng phía trước.

Xóa thông tin cá nhân, Token và khóa sản phẩm khỏi Log trước khi đăng công khai.

## 📚 Nguồn tham khảo

Trong quá trình phát triển, tôi tham khảo cách tổ chức và triển khai của AtlasOS, XOS, FSOS, INSIDEXOS, Atom và SapphireOS. Phần trình bày README có tham khảo ReviOS.

StrikeOS không đại diện và không được bảo trợ bởi các dự án này. Việc liệt kê nguồn tham khảo cũng không có nghĩa StrikeOS áp dụng toàn bộ thiết lập của họ.

## 📄 Giấy phép

Xem [LICENSE](./LICENSE) để biết điều kiện sử dụng và phân phối mã nguồn. Các phần mã từ bên thứ ba, nếu có, chịu điều kiện giấy phép tương ứng.

SuperStrike X1 không cung cấp khóa sản phẩm hoặc công cụ kích hoạt Windows. Bạn cần có giấy phép phù hợp cho Windows đang sử dụng.
