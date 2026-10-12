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

<p align="center"><strong>Tinh gọn Windows cho chơi game, đồng thời giữ lại các thành phần bảo mật cốt lõi.</strong></p>

<p align="center">
  <a href="https://strikeos.site">Website</a> ·
  <a href="https://discord.gg/strikeos">Discord</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/releases">Releases</a> ·
  <a href="#cài-đặt">Cài đặt</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/issues">Báo lỗi</a>
</p>

---

## 🎮 Giới thiệu

SuperStrike X1 là AME Playbook áp dụng lên Windows bạn đang dùng. Không cần cài lại hệ điều hành và đây không phải bản Windows tùy chỉnh. Playbook tập trung giảm một số ứng dụng, dịch vụ và hoạt động nền; Windows Defender, Firewall cùng các thành phần bảo mật cốt lõi được giữ lại.

Đây là **bản thử nghiệm**. Các build bên dưới là những phiên bản được khai báo hỗ trợ, nhưng chưa thể đại diện cho mọi cấu hình. Kết quả còn tùy Edition, driver, phần cứng và phần mềm trên máy. Kiểm tra tự động không thay thế việc thử nghiệm trên Windows thật.

## ⚠️ Cảnh báo và miễn trừ trách nhiệm

> **Đây là phần mềm thử nghiệm, được cung cấp “nguyên trạng” (AS IS). Hãy đọc các giới hạn dưới đây trước khi chạy. Nếu không đồng ý, vui lòng không sử dụng Playbook.**

- **Ảnh hưởng đến hệ thống:** Playbook thay đổi cài đặt Windows, ứng dụng, dịch vụ, tác vụ và một số thiết lập mạng/phần cứng. Lỗi hoặc mất chức năng có thể xảy ra; trong trường hợp nghiêm trọng, bạn có thể phải sửa chữa hoặc cài lại Windows. Playbook không tự sao lưu và không hoàn tác đầy đủ. Restore Point không thay thế System Image hoặc bản sao lưu riêng.
- **Tình trạng kiểm thử:** Các build được liệt kê là phạm vi hỗ trợ dự kiến, không có nghĩa mọi Edition, máy OEM, driver hay trạng thái Windows đã được thử. Một số lỗi tùy chọn chỉ được ghi cảnh báo để các bước khác tiếp tục; lỗi ở bước bắt buộc hoặc tiến trình cài đặt quá thời hạn vẫn có thể khiến AME Wizard dừng. Trạng thái “Completed” không đồng nghĩa mọi tùy chọn đã áp dụng thành công.
- **Hiệu năng:** Không bảo đảm mức FPS, 1% Low, 0.1% Low, độ trễ, RAM, số tiến trình hay mức cải thiện cụ thể. Kết quả thay đổi theo cấu hình, driver, game và phần mềm đang chạy.
- **Game và Anti-cheat:** Giữ lại thành phần bảo mật của Windows không đồng nghĩa được nhà phát hành game chứng nhận. Không thể bảo đảm tương thích hoặc tránh cảnh báo/khóa tài khoản. Hãy kiểm tra yêu cầu của game và Anti-cheat trước khi dùng.
- **Máy không nên dùng để thử:** Tránh máy chủ, máy làm việc quan trọng, máy thuộc Domain/MDM hoặc máy đang được hỗ trợ từ xa. Trên máy chính, hãy tạo bản sao lưu có thể khôi phục và chuẩn bị phương án xử lý nếu Windows hoặc mạng gặp sự cố.
- **Tệp tải xuống:** Chỉ tải từ Releases của repository được liên kết trên [strikeos.site](https://strikeos.site/) và đối chiếu SHA-256 nếu có công bố. Không chạy tệp đã chỉnh sửa, đóng gói lại hoặc lấy từ nguồn không xác minh. Runtime được tải từ nhà cung cấp tương ứng; StrikeOS không kiểm soát máy chủ hay các thay đổi từ bên thứ ba. Nếu hash không khớp hoặc tệp bị cảnh báo, đừng chạy và hãy báo để kiểm tra.
- **Trách nhiệm khi sử dụng:** Bạn cần có quyền hợp pháp và quyền quản trị trên thiết bị, xem lại các lựa chọn trước khi xác nhận và tự sao lưu dữ liệu. Khi gửi log, hãy xóa mật khẩu, token, khóa sản phẩm và thông tin cá nhân.
- **Giới hạn trách nhiệm:** Trong phạm vi pháp luật cho phép, người dùng tự chịu trách nhiệm về quyết định tải và chạy Playbook cũng như các rủi ro có thể phát sinh, gồm mất dữ liệu, gián đoạn công việc hoặc lỗi hệ thống/thiết bị. Nội dung này không loại trừ quyền của người dùng hay trách nhiệm mà pháp luật không cho phép miễn trừ. Thỏa thuận dịch vụ riêng, nếu có, áp dụng cho dịch vụ tương ứng.
- **Hỗ trợ:** Báo lỗi qua GitHub Issues hoặc Discord. Nhóm phát triển tiếp nhận và xử lý theo khả năng; không cam kết thời gian phản hồi, sửa lỗi hay lịch cập nhật. Hãy đọc ghi chú phát hành trước khi nâng cấp và không chạy chồng phiên bản nếu chưa có hướng dẫn.

Thông tin này giải thích phạm vi và rủi ro sử dụng, không thay thế tư vấn pháp lý. Muốn dùng làm điều khoản pháp lý chính thức, chủ dự án nên nhờ luật sư rà soát theo nơi phát hành.

## 🪟 Windows mục tiêu

| Hệ điều hành | Phiên bản | Build |
|---|---:|---:|
| Windows 10 64-bit | 22H2 | `19045` |
| Windows 11 64-bit | 24H2 | `26100` |
| Windows 11 64-bit | 25H2 | `26200` |

Build ngoài danh sách sẽ bị từ chối. Không chạy trên Windows đã được bên thứ ba tùy chỉnh. Với thiết bị do tổ chức quản lý, cần có sự cho phép của quản trị viên.

## ⚙️ Chế độ

### Standard

Cấu hình cơ bản, gồm các thay đổi ứng dụng, dịch vụ, tác vụ nền và thiết lập Windows. Một số mục có thể chọn trong AME Wizard. Không có mức FPS, RAM hay số tiến trình cố định được bảo đảm.

### Performance

Bao gồm Standard và một số thiết lập bổ sung về lưu trữ, mạng, nguồn điện, đồ họa và độ trễ: TRIM, RSS, TCP Auto-Tuning, HAGS, MSI Mode, HPET/BCD, Timer Resolution và đặt lại Winsock/IP.

Các thiết lập này phụ thuộc thiết bị và driver; chúng có thể không áp dụng được hoặc không cải thiện hiệu năng. Đặt lại Winsock/IP có thể làm gián đoạn kết nối hoặc ảnh hưởng VPN và cấu hình mạng riêng. Muốn so sánh, hãy đo trước và sau trong cùng điều kiện.

## Lựa chọn bổ sung

Trong AME Wizard, bạn có thể chọn gỡ OneDrive, Xbox/Game Bar, tắt Windows Search, hoặc tắt một số dịch vụ Bluetooth, in/scan và bàn phím cảm ứng/viết tay. Có thể chọn cài Brave, Firefox hoặc Chrome. Các lựa chọn OneDrive, Xbox/Game Bar và Windows Search được tích sẵn; hãy bỏ chọn nếu muốn giữ lại. Bluetooth và in/scan mặc định không bị tắt. Tùy chọn bàn phím cảm ứng/viết tay chỉ tắt `TabletInputService`, không tắt phần cứng hoặc driver màn hình cảm ứng. Gỡ Xbox/Game Bar có thể ảnh hưởng Game Pass và chức năng ghi hình.

## Gaming Runtime

Playbook kiểm tra Visual C++ 2015–2022 x86/x64, DirectX Legacy và .NET Framework 3.5. Thành phần đã có sẽ được bỏ qua. Thành phần còn thiếu được tải từ nguồn Microsoft và kiểm tra chữ ký khi có thể. Nếu tải xuống, kết nối bảo mật hoặc nguồn cài Windows không sẵn có, Runtime có thể được ghi nhận là chưa cài và các bước khác tiếp tục. Nếu trình cài hoặc Windows servicing vượt thời hạn chờ, AME Wizard có thể dừng để tránh chạy thêm tiến trình cài đặt cùng lúc.

<a id="cài-đặt"></a>

## 📖 Cài đặt

1. Kiểm tra phiên bản và build bằng `winver`.
2. Sao lưu dữ liệu; nên tạo System Image hoặc Snapshot có thể khôi phục.
3. Tải AME Wizard và `.apbx` từ các liên kết chính thức ở đầu trang hoặc mục Releases.
4. Mở AME Wizard, nạp `.apbx`, chọn chế độ và rà lại các tùy chọn.
5. Trong khi chạy, không tắt máy, đóng Wizard hoặc chạy thêm công cụ tối ưu.
6. Đọc kết quả và cảnh báo. Khởi động lại nếu được yêu cầu.

## 🛠️ Báo lỗi

Khi tạo Issue, gửi phiên bản, Edition và build Windows; cấu hình phần cứng; chế độ và lựa chọn đã dùng; cùng toàn bộ log AME Wizard. Nếu có, đính kèm báo cáo sau khởi động lại. Xóa thông tin nhạy cảm trước khi đăng công khai.

---

<p align="center"><strong>SuperStrike X1 · StrikeOS</strong></p>
