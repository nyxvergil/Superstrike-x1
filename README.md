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

<p align="center"><strong>Tinh gọn Windows cho chơi game. Giữ lại các thành phần bảo mật cốt lõi.</strong></p>

<p align="center">
  <a href="https://strikeos.site">Website</a> ·
  <a href="https://discord.gg/strikeos">Discord</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/releases">Releases</a> ·
  <a href="#cài-đặt">Cài đặt</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/issues">Báo lỗi</a>
</p>

---

## Giới thiệu

SuperStrike X1 là AME Playbook áp dụng trực tiếp lên Windows đang sử dụng, không phải bản Windows tùy chỉnh và không yêu cầu cài lại hệ điều hành. Playbook tập trung giảm ứng dụng và hoạt động nền không cần thiết, đồng thời giữ lại Windows Defender, Firewall và các thành phần bảo mật quan trọng.

Đây là **bản thử nghiệm**. Các build bên dưới là phạm vi mục tiêu được khai báo; kết quả có thể khác theo Edition, driver, phần cứng và phần mềm trên từng máy. Kiểm tra cú pháp và bài thử tự động không thay thế việc chạy thử trên Windows thật.

## Windows mục tiêu

| Hệ điều hành | Phiên bản | Build |
|---|---:|---:|
| Windows 10 64-bit | 22H2 | `19045` |
| Windows 11 64-bit | 24H2 | `26100` |
| Windows 11 64-bit | 25H2 | `26200` |

Build ngoài danh sách sẽ bị từ chối. Không chạy trên bản Windows tùy chỉnh, máy chủ hoặc thiết bị do tổ chức quản lý nếu chưa được quản trị viên cho phép.

## Chế độ

### Standard

Cấu hình tinh gọn cơ bản. Playbook xử lý ứng dụng, dịch vụ, tác vụ nền và một số thiết lập Windows đã chọn; một số mục có thể được bật hoặc tắt trong trang lựa chọn. Không có mức FPS, RAM hay số tiến trình được bảo đảm.

### Performance

Bao gồm Standard và các bước bổ sung cho lưu trữ, mạng, nguồn điện, thiết bị đồ họa và độ trễ, như TRIM, RSS, TCP Auto-Tuning, HAGS, MSI Mode, HPET/BCD, Timer Resolution và đặt lại Winsock/IP.

Một số thiết lập phụ thuộc thiết bị hoặc driver; có thể không áp dụng được hoặc không cải thiện kết quả trên máy của bạn. Đặt lại Winsock/IP có thể làm gián đoạn mạng hoặc ảnh hưởng VPN và cấu hình mạng riêng. Hãy đo FPS, 1% Low, 0.1% Low và Frame Time trước/sau trên cùng điều kiện nếu muốn đánh giá tác động.

## Lựa chọn bổ sung

Tùy trang lựa chọn trong AME Wizard, người dùng có thể chọn gỡ OneDrive, Xbox/Game Bar, tắt Windows Search hoặc một số dịch vụ Bluetooth, in/scan và cảm ứng; đồng thời có thể chọn cài Brave, Firefox hoặc Chrome. Chỉ chọn tắt chức năng phần cứng nếu máy không sử dụng thiết bị đó. Gỡ Xbox/Game Bar có thể ảnh hưởng Game Pass, ghi hình hoặc tính năng liên quan.

## Gaming Runtime

Playbook kiểm tra Visual C++ 2015–2022 x86/x64, DirectX Legacy và .NET Framework 3.5. Thành phần đã có sẽ được bỏ qua; thành phần còn thiếu được lấy từ nguồn Microsoft và kiểm tra chữ ký khi có trình cài tương ứng. Nếu tải xuống, TLS, chữ ký hoặc nguồn cài Windows không khả dụng, thành phần có thể được báo là chưa cài và Playbook tiếp tục. Nếu trình cài hoặc servicing bị treo quá thời hạn, Playbook có thể dừng để tránh khởi chạy thêm tiến trình cài đặt chồng lấp.

## Cài đặt

1. Xác nhận phiên bản và build bằng `winver`.
2. Sao lưu dữ liệu quan trọng; ưu tiên tạo System Image hoặc Snapshot có thể khôi phục.
3. Tải AME Wizard và tệp `.apbx` từ các liên kết chính thức ở đầu trang hoặc mục Releases.
4. Mở AME Wizard, nạp tệp `.apbx`, chọn Standard hoặc Performance và kiểm tra kỹ các lựa chọn bổ sung.
5. Không tắt máy, đóng Wizard hoặc chạy công cụ tối ưu khác khi Playbook đang hoạt động.
6. Đọc toàn bộ kết quả, xử lý cảnh báo, rồi khởi động lại nếu được yêu cầu.

## Cảnh báo và miễn trừ trách nhiệm

> **Đây là phần mềm thử nghiệm, được cung cấp “nguyên trạng” (AS IS). Chỉ tiếp tục nếu bạn đã hiểu các giới hạn dưới đây và chấp nhận tự quyết định việc sử dụng. Nếu không đồng ý, không tải hoặc chạy Playbook.**

- **Có thể ảnh hưởng Windows và dữ liệu.** Playbook thay đổi cài đặt hệ thống, dịch vụ, tác vụ, ứng dụng và một số cấu hình mạng/phần cứng. Có thể phát sinh lỗi, mất chức năng, gián đoạn mạng, lỗi driver hoặc cần sửa chữa/cài đặt lại Windows. Playbook không sao lưu và không hoàn tác đầy đủ mọi thay đổi. Restore Point không thay thế bản sao lưu độc lập.
- **Bản thử nghiệm chưa được xác nhận trên mọi cấu hình.** Khai báo hỗ trợ build không đồng nghĩa mọi Edition, máy OEM, driver, ứng dụng hoặc trạng thái Windows đã được kiểm thử. Kiểm tra tự động không chứng minh Playbook sẽ hoàn tất trên máy của bạn. Một số lỗi phụ được ghi cảnh báo để bước khác tiếp tục; lỗi ở bước bắt buộc, trạng thái không an toàn hoặc tiến trình cài đặt quá thời hạn vẫn có thể làm Wizard dừng. “Completed” không có nghĩa mọi tùy chọn đều áp dụng thành công.
- **Không cam kết hiệu năng.** Không bảo đảm FPS, 1% Low, 0.1% Low, độ trễ, mức RAM, số tiến trình, độ ổn định hoặc mức cải thiện cụ thể. Kết quả tùy thuộc cấu hình máy, phiên bản Windows, driver, game và phần mềm chạy nền.
- **Anti-cheat và dịch vụ bên thứ ba.** Playbook giữ lại các thành phần bảo mật cốt lõi và không chủ động tắt dịch vụ anti-cheat đã nêu trong dự án. Điều đó không phải chứng nhận hoặc bảo đảm tương thích, không bảo đảm tránh cảnh báo/khóa tài khoản và không thay thế quy định của nhà phát hành game. Người dùng cần tự kiểm tra yêu cầu của game và anti-cheat trước khi áp dụng.
- **Máy không phù hợp để thử nghiệm.** Không dùng trên máy chủ, máy làm việc quan trọng, máy thuộc Domain/MDM hoặc máy khách đang được hỗ trợ từ xa. Với máy chính, hãy có bản sao lưu có thể khôi phục và chuẩn bị phương án xử lý nếu Windows hoặc mạng gặp sự cố.
- **Nguồn tải và tệp bên thứ ba.** Chỉ tải bản phát hành từ Releases của repository được liên kết trên [strikeos.site](https://strikeos.site/); đối chiếu SHA-256 do dự án công bố. Không chạy bản đã chỉnh sửa, đóng gói lại hoặc lấy từ nguồn không xác minh. Runtime bên ngoài được tải từ nhà cung cấp tương ứng; StrikeOS không kiểm soát máy chủ, thay đổi, gián đoạn hay sự cố bảo mật của bên thứ ba. Nếu hash không khớp hoặc có cảnh báo bất thường, không chạy tệp và hãy báo lại để xác minh.
- **Trách nhiệm của người dùng.** Người chạy Playbook phải có quyền hợp pháp trên thiết bị, quyền quản trị cần thiết, đọc các lựa chọn trước khi xác nhận và tự bảo vệ dữ liệu. Hãy dừng sử dụng nếu thấy hành vi bất thường; khi báo lỗi, gửi log và thông tin build nhưng xóa mật khẩu, token, khóa sản phẩm và dữ liệu cá nhân trước khi đăng công khai.
- **Giới hạn trách nhiệm.** Trong phạm vi pháp luật cho phép, nhóm StrikeOS không chịu trách nhiệm đối với mất dữ liệu, gián đoạn công việc/dịch vụ, lỗi hệ điều hành, phần mềm hoặc thiết bị phát sinh từ việc tải, lựa chọn, cài đặt hay sử dụng Playbook; người dùng tự chịu trách nhiệm cho quyết định áp dụng và hậu quả có thể dự đoán được. Điều khoản này không loại trừ quyền hoặc trách nhiệm nào mà pháp luật hiện hành không cho phép loại trừ. Nếu có thỏa thuận dịch vụ riêng, thỏa thuận đó được áp dụng cho phạm vi dịch vụ tương ứng.
- **Hỗ trợ và cập nhật.** Báo lỗi qua GitHub Issues hoặc Discord theo khả năng duy trì dự án. Không cam kết thời gian phản hồi, sửa lỗi, hỗ trợ từng cấu hình hay lịch phát hành. Đọc ghi chú của từng bản trước khi cập nhật; không chạy chồng phiên bản nếu chưa có hướng dẫn.

Thông tin này nhằm giúp người dùng hiểu rủi ro và phạm vi hỗ trợ; không thay thế tư vấn pháp lý. Nếu cần điều khoản có hiệu lực pháp lý tại một quốc gia cụ thể, chủ dự án nên nhờ luật sư rà soát.

## Báo lỗi

Khi tạo Issue, hãy gửi phiên bản/Edition/build Windows, cấu hình phần cứng, chế độ và lựa chọn đã dùng, toàn bộ log AME Wizard, cùng báo cáo sau khởi động lại nếu có. Không đăng thông tin nhạy cảm công khai.

---

<p align="center"><strong>SuperStrike X1 · StrikeOS</strong></p>
