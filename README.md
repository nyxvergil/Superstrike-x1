<h1 align="center">
  <a href="https://strikeos.site"><img src="assets/strike-logo.png" alt="StrikeOS" width="800"></a>
</h1>

<p align="center"><strong>Playbook tinh gọn Windows dành cho gaming, hiệu năng và khả năng tương thích Anti-cheat.</strong></p>

<p align="center">
  <a href="https://strikeos.site">🌐 Website</a>
  •
  <a href="https://discord.gg/strikeos">💬 Discord</a>
  •
  <a href="#cách-cài-đặt">📖 Hướng dẫn cài đặt</a>
  •
  <a href="#báo-lỗi">🛠️ Báo lỗi</a>
</p>

SuperStrike X1 là Playbook tối ưu Windows dành cho Gamming. Dự án tập trung giảm Process nền, cải thiện Latency, giữ Framerate ổn định và hạn chế ảnh hưởng đến FPS, 1% Low và 0.1% Low.

Playbook hoạt động trên Windows đang sử dụng, không yêu cầu cài lại Windows và Bắt buộc là bản window được hỗ trợ dưới đây.

## Hệ điều hành hỗ trợ

- Windows 10 22H2 64-bit — Build `19045`.
- Windows 11 24H2 64-bit — Build `26100`.
- Windows 11 25H2 64-bit — Build `26200`.

Các phiên bản và Build khác sẽ bị từ chối để tránh áp dụng cài đặt không tương thích.

## Mục tiêu

- Giảm số Process và Services chạy nền không cần thiết.
- Giảm mức sử dụng RAM khi máy ở trạng thái nghỉ.
- Cải thiện Latency và độ phản hồi khi chơi game.
- Hạn chế giật khựng, ưu tiên sự ổn định của Framerate và Frame Time.
- Giữ Windows Defender và các thành phần bảo mật cần thiết.
- Hướng đến khả năng tương thích với Vanguard, Easy Anti-Cheat, BattlEye và EA AntiCheat...
- Không kèm Toolbox, gói Post-install hoặc phần mềm quảng cáo. Và Các phần mềm Kích hoạt Window.

Kết quả thực tế phụ thuộc vào phần cứng, Driver, phiên bản Windows, phần mềm đang cài và từng trò chơi. Playbook không thể bảo đảm một mức FPS, RAM hoặc số Process giống nhau trên mọi máy.

## Chế độ tối ưu

### Standard

Chế độ mặc định, phù hợp với phần lớn người dùng. Standard áp dụng các thiết lập tinh gọn, quyền riêng tư, dịch vụ, tác vụ nền và tối ưu hệ thống đã được kiểm tra mà không bật nhóm Tweak/Action nâng cao.

### Performance

Bao gồm toàn bộ thiết lập của Standard và bổ sung:

- Kiểm tra và bật TRIM khi cần.
- Bật RSS, đặt TCP Auto-Tuning về `normal` và tắt RSC.
- Điều chỉnh một số thuộc tính của Card mạng khi Driver hỗ trợ.
- Cấu hình Power Plan theo loại thiết bị.
- Điều chỉnh Core Parking trên máy bàn.
- Bật HAGS khi có Card đồ họa phù hợp.
- Bật MSI Mode cho GPU và Card mạng khi thiết bị đã hỗ trợ.
- Áp dụng HPET và thiết lập BCD dành cho chế độ Performance.
- Chạy Timer Resolution ở mức `0.5 ms` bằng tác vụ nền của StrikeOS.
- Đặt lại Winsock và cấu hình IP, sau đó xóa DNS Cache.

Performance không phải lúc nào cũng nhanh hơn trên mọi cấu hình. Nên đo FPS, 1% Low, 0.1% Low và Frame Time trước và sau khi áp dụng.

## Thành phần tùy chọn

Người dùng có thể lựa chọn:

- Gỡ OneDrive.
- Gỡ các thành phần Xbox và Game Bar.
- Tắt lập chỉ mục Windows Search.
- Tắt Bluetooth khi máy không sử dụng Bluetooth.
- Tắt dịch vụ in và quét khi máy không sử dụng máy in hoặc máy quét.
- Tắt dịch vụ cảm ứng, bút và máy tính bảng khi thiết bị không cần các chức năng này.
- Cài Brave, Mozilla Firefox hoặc Google Chrome.

Không chọn tắt một nhóm phần cứng nếu máy vẫn đang sử dụng thiết bị tương ứng.

## Gaming Runtime

Playbook tự kiểm tra các thành phần sau:

- Microsoft Visual C++ 2015–2022 x86.
- Microsoft Visual C++ 2015–2022 x64.
- DirectX Legacy Runtime.
- .NET Framework 3.5.

Thành phần đã có sẽ được bỏ qua. Thành phần còn thiếu chỉ được cài từ nguồn Microsoft và bộ cài phải có chữ ký hợp lệ.

DirectX Legacy và .NET Framework 3.5 là thành phần bổ sung. Nếu nguồn tải không truy cập được, chứng chỉ TLS không hợp lệ hoặc Windows không có nguồn `sources\sxs`, Playbook sẽ ghi trạng thái `Unavailable` hoặc `SkippedNoSource` rồi tiếp tục tối ưu. Playbook không bỏ qua kiểm tra chứng chỉ và không báo cài thành công khi thực tế chưa cài.

## Tương thích Anti-cheat

SuperStrike X1 không chủ động vô hiệu hóa:

- Windows Defender.
- Secure Boot.
- DEP và các biện pháp bảo vệ tiến trình.
- BFE và Windows Firewall.
- Device Guard hoặc Credential Guard.
- Dịch vụ của Vanguard, Easy Anti-Cheat, BattlEye và EA AntiCheat.

Khả năng tương thích còn phụ thuộc vào yêu cầu của từng trò chơi và từng phiên bản Anti-cheat. Hãy giữ Windows, Driver và Anti-cheat ở phiên bản phù hợp với trò chơi.

## Cách cài đặt




## Lưu ý trước khi sử dụng

- Playbook không tự tạo bản sao lưu toàn bộ Windows.
- Không chạy đồng thời Windows Update, DISM, trình cài Driver hoặc công cụ tối ưu khác.
- Không ép tắt AME Wizard khi một thành phần hệ thống đang được xử lý.
- Winsock và cấu hình mạng chỉ được đặt lại trong chế độ Performance.
- Một số thay đổi chỉ có hiệu lực sau khi khởi động lại.
- Nên thử trên máy ảo hoặc Windows mới trước khi áp dụng cho máy đang sử dụng hằng ngày.

## Cấu trúc dự án

```text
.
├── assets
│   └── strike-logo.png
├── README.md
├── playbook.conf
├── playbook.png
├── Configuration
│   ├── main.yml
│   └── Tasks
├── Executables
└── Images
```

- `assets`: hình ảnh dùng cho trang GitHub, không được đóng gói vào Playbook.
- `README.md`: tài liệu giới thiệu và hướng dẫn sử dụng.
- `playbook.conf`: thông tin Playbook và các lựa chọn hiển thị trong AME Wizard.
- `Configuration`: thứ tự chạy và toàn bộ Action tối ưu.
- `Executables`: Helper chỉ dành cho phần cần nhận diện hệ thống hoặc xử lý nhiều bước.
- `Images`: hình ảnh dùng cho trang lựa chọn trình duyệt.

## Báo lỗi

Khi tạo Issue, vui lòng cung cấp:

- Phiên bản và Build Windows.
- Edition đang sử dụng.
- Chế độ Standard hoặc Performance.
- Các lựa chọn đã đánh dấu trong AME Wizard.
- Toàn bộ Log của AME Wizard, không chỉ dòng lỗi cuối.
- Báo cáo Post-boot nếu lỗi liên quan đến Process, RAM hoặc dịch vụ.
- Mô tả máy thật hay máy ảo và cấu hình phần cứng chính.

Không đăng khóa sản phẩm, mật khẩu, Token, địa chỉ thư điện tử hoặc thông tin cá nhân vào Issue công khai.

## Liên hệ

- Website: [strikeos.site](https://strikeos.site)
- Discord: `.gg/strikeos`

---

SuperStrike X1 được phát triển bởi StrikeOS.
