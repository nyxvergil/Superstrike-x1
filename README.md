<p align="center">
  <a href="https://strikeos.site">
    <img src="./strike-logo.png" alt="StrikeOS" width="760">
  </a>
</p>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/VERSION-2.0.17-5B21FF?style=for-the-badge">
  <img alt="Windows" src="https://img.shields.io/badge/WINDOWS-10%20%7C%2011-0078D4?style=for-the-badge&logo=windows11&logoColor=white">
  <img alt="AME Playbook" src="https://img.shields.io/badge/AME-PLAYBOOK-202020?style=for-the-badge">
  <img alt="Status" src="https://img.shields.io/badge/STATUS-TEST-F59E0B?style=for-the-badge">
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

SuperStrike X1 là AME Playbook cấu hình Windows đang sử dụng, không phải bản Windows tùy chỉnh và không yêu cầu cài lại hệ điều hành. Playbook có hai chế độ Standard và Performance, kèm các lựa chọn gỡ ứng dụng, tắt một số chức năng và cài trình duyệt.

## Cảnh báo và miễn trừ trách nhiệm

> SuperStrike X1 là bản thử nghiệm, được cung cấp “nguyên trạng” (AS IS). Chỉ tiếp tục nếu bạn hiểu các thay đổi và chấp nhận rủi ro.

- Playbook thay đổi ứng dụng, dịch vụ, tác vụ và cài đặt Windows. Có thể phát sinh lỗi, mất chức năng hoặc gián đoạn mạng. Playbook không tạo bản sao lưu và không hoàn tác toàn bộ; hãy tạo System Image hoặc bản sao lưu có thể khôi phục trước khi chạy.
- Phiên bản được liệt kê là phạm vi build mục tiêu, không bảo đảm đã kiểm thử trên mọi Edition, phần cứng, driver hay phần mềm. Lỗi ở bước bắt buộc hoặc tiến trình quá thời hạn có thể khiến AME Wizard dừng. “Completed” không có nghĩa mọi tùy chọn đều đã áp dụng.
- Không bảo đảm FPS, 1% Low, 0.1% Low, độ trễ, mức dùng RAM, số tiến trình hoặc khả năng tương thích với mọi game và Anti-cheat. Việc giữ lại thành phần bảo mật không phải chứng nhận từ nhà phát hành game.
- Không khuyến nghị dùng trên máy chủ, máy làm việc quan trọng hoặc thiết bị thuộc Domain/MDM nếu chưa được quản trị viên cho phép. Bạn cần có quyền quản trị và quyền thực hiện thay đổi trên thiết bị.
- Chỉ tải bản phát hành từ Releases của repository được liên kết trên [strikeos.site](https://strikeos.site/). Đối chiếu SHA-256 nếu có công bố. Không chạy bản đã chỉnh sửa hoặc đóng gói lại từ nguồn khác. Các Runtime tải trong quá trình cài đặt đến từ nhà cung cấp tương ứng và nằm ngoài kiểm soát của dự án.
- Việc tải và sử dụng là quyết định của bạn. Trong phạm vi pháp luật cho phép, dự án không chịu trách nhiệm cho thiệt hại phát sinh từ việc sử dụng hoặc không thể sử dụng Playbook. Nội dung này không loại trừ quyền của người dùng hay trách nhiệm mà pháp luật không cho phép miễn trừ. Đây không phải tư vấn pháp lý.
- Hỗ trợ lỗi qua GitHub Issues hoặc Discord theo khả năng duy trì dự án; không cam kết thời gian phản hồi, sửa lỗi hoặc lịch cập nhật. Khi gửi log công khai, hãy xóa mật khẩu, token, khóa sản phẩm và thông tin cá nhân.

## Windows hỗ trợ

| Hệ điều hành | Phiên bản | Build |
|---|---:|---:|
| Windows 10 64-bit | 22H2 | `19045` |
| Windows 11 64-bit | 24H2 | `26100` |
| Windows 11 64-bit | 25H2 | `26200` |

Các build khác không nằm trong phạm vi hỗ trợ và có thể bị từ chối. Không dùng trên Windows đã được công cụ khác tùy chỉnh nếu chưa hiểu rõ các thay đổi trước đó.

## Chế độ

### Standard

Áp dụng cấu hình Windows cơ bản, gồm các thay đổi về ứng dụng, dịch vụ và hoạt động nền. Một số lựa chọn được hiển thị riêng trong AME Wizard.

### Performance

Bao gồm Standard và các thiết lập bổ sung cho lưu trữ, mạng, nguồn điện, đồ họa và độ trễ: TRIM, RSS, TCP Auto-Tuning, RSC, HAGS, MSI Mode, HPET/BCD, Timer Resolution và đặt lại Winsock/IP cùng bộ nhớ đệm DNS.

Các mục phụ thuộc phần cứng, driver và cấu hình mạng; không phải mục nào cũng áp dụng được hoặc cải thiện hiệu năng. Đặt lại Winsock/IP có thể làm gián đoạn kết nối và ảnh hưởng VPN, IP tĩnh hoặc cấu hình mạng riêng. Nên đo trước và sau trên cùng máy, cùng điều kiện.

## Lựa chọn trong AME Wizard

- **OneDrive, Xbox/Game Bar và Windows Search:** được tích sẵn. Bỏ chọn nếu muốn giữ các thành phần này. Việc gỡ Xbox/Game Bar có thể ảnh hưởng Game Pass, ghi hình hoặc tính năng liên quan.
- **Bluetooth, in/scan và bàn phím cảm ứng/viết tay:** mặc định không chọn. Hai lựa chọn đầu có thể tắt dịch vụ và driver liên quan sau khi xác nhận. Lựa chọn cảm ứng/viết tay tắt dịch vụ `TabletInputService`; không gỡ phần cứng hay driver cảm ứng.
- **Trình duyệt:** mặc định không cài. Nếu bật, chọn Brave, Firefox hoặc Chrome.

## Gaming Runtime

Playbook kiểm tra Visual C++ 2015–2022 x86/x64, DirectX Legacy và .NET Framework 3.5; thành phần đã có sẽ được bỏ qua. Thành phần còn thiếu được cài từ nguồn của Microsoft. Nếu không tải được hoặc Windows không có nguồn cài cần thiết, Runtime có thể được ghi nhận là chưa cài và các bước tiếp tục. Nếu trình cài đặt hoặc Windows servicing vượt thời hạn chờ, AME Wizard có thể dừng để tránh chạy chồng tiến trình cài đặt.

## Cài đặt

1. Dùng `winver` để xác nhận phiên bản Windows nằm trong danh sách hỗ trợ.
2. Sao lưu dữ liệu; ưu tiên tạo System Image hoặc bản sao lưu có thể khôi phục.
3. Tải AME Wizard và tệp `.apbx` từ nguồn chính thức.
4. Mở `.apbx` bằng AME Wizard, chọn chế độ và kiểm tra kỹ các tùy chọn.
5. Trong khi chạy, không tắt máy, đóng Wizard hoặc chạy thêm công cụ tối ưu khác.
6. Đọc kết quả và cảnh báo; khởi động lại nếu được yêu cầu.

## Báo lỗi

Tạo [GitHub Issue](https://github.com/nyxvergil/Superstrike-x1/issues) hoặc liên hệ qua [Discord](https://discord.gg/strikeos). Gửi phiên bản Windows, cấu hình máy, chế độ và lựa chọn đã dùng cùng log AME Wizard. Xóa thông tin nhạy cảm trước khi đăng.

---

<p align="center"><strong>SuperStrike X1 · StrikeOS</strong></p>
