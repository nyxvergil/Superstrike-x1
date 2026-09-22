<p align="center">
  <a href="https://strikeos.site">
    <img src="./strike-logo.png" alt="SuperStrike X1" width="760">
  </a>
</p>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/VERSION-1.0.0-5B21FF?style=for-the-badge">
  <img alt="Windows" src="https://img.shields.io/badge/WINDOWS-10%20%7C%2011-0078D4?style=for-the-badge">
  <img alt="AME Playbook" src="https://img.shields.io/badge/AME-PLAYBOOK-202020?style=for-the-badge">
  <img alt="Defender retained" src="https://img.shields.io/badge/DEFENDER-RETAINED-16A34A?style=for-the-badge">
  <a href="./LICENSE"><img alt="License details" src="https://img.shields.io/badge/LICENSE-DETAILS-4B5563?style=for-the-badge"></a>
</p>

<p align="center">
  <img alt="Supported builds" src="https://img.shields.io/badge/BUILD-19045%20%7C%2026100%20%7C%2026200-2563EB?style=flat-square">
  <img alt="Architecture" src="https://img.shields.io/badge/ARCH-x64-6D28D9?style=flat-square">
  <img alt="Profiles" src="https://img.shields.io/badge/PROFILES-STANDARD%20%7C%20PERFORMANCE-E11D48?style=flat-square">
  <img alt="Revision" src="https://img.shields.io/badge/REV-PERFORMANCE12--VI-2563EB?style=flat-square">
  <img alt="Status" src="https://img.shields.io/badge/STATUS-TEST-F59E0B?style=flat-square">
</p>

<p align="center"><strong>Tinh gọn Windows cho máy chơi game.</strong></p>

<p align="center">
  <a href="https://strikeos.site">Website</a> ·
  <a href="https://discord.gg/strikeos">Discord</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/releases">Tải về</a> ·
  <a href="#cai-dat">Cài đặt</a> ·
  <a href="https://github.com/nyxvergil/Superstrike-x1/issues">Báo lỗi</a>
</p>

---

## Giới thiệu

**SuperStrike X1** giúp bạn tinh gọn Windows đang sử dụng thông qua AME Wizard, không cần cài lại hệ điều hành.

Bạn có thể chọn chế độ cấu hình, gỡ các ứng dụng không dùng và giảm hoạt động nền. Để đánh giá hiệu quả trên máy của mình, hãy so sánh FPS, 1% Low, 0.1% Low và Frame Time trước và sau khi chạy.

**Phiên bản: 2.0.17 — Performance12-vi Test.**

## Lưu ý trước khi sử dụng

> [!WARNING]
> Playbook thay đổi sâu vào Windows. Hãy sao lưu hệ thống và dữ liệu trước khi chạy; Restore Point không thay thế bản sao lưu đầy đủ. Playbook không tự sao lưu và chưa có hoàn tác toàn bộ.

- **Kết quả:** Không cam kết FPS, RAM, số Process cố định hoặc tương thích với mọi Driver, game và Anti-cheat. Đây là bản thử nghiệm.
- **Phạm vi:** Không khuyến nghị cho máy chủ, máy làm việc quan trọng hoặc thiết bị Domain/MDM khi chưa được quản trị viên cho phép. Windows đã chỉnh sửa bằng công cụ khác có thể phát sinh xung đột.
- **Nguồn tải:** Chỉ dùng Releases được liên kết trên [strikeos.site](https://strikeos.site), đối chiếu SHA256 nếu có. StrikeOS không kiểm soát các bản do bên thứ ba sửa hoặc đóng gói lại. Ngừng chạy và báo lại nếu có dấu hiệu bất thường.
- **Trách nhiệm:** Bạn tự quyết định việc áp dụng sau khi đọc các thay đổi và chuẩn bị bản sao lưu. Các giới hạn trách nhiệm tuân theo giấy phép và pháp luật, không loại trừ quyền hợp pháp của bạn hoặc nghĩa vụ của bên phát triển không được phép miễn trừ.

## Windows hỗ trợ

| Hệ điều hành | Phiên bản | Build |
|:---|:---:|:---:|
| Windows 10 x64 | 22H2 | `19045` |
| Windows 11 x64 | 24H2 | `26100` |
| Windows 11 x64 | 25H2 | `26200` |

Bạn có thể kiểm tra phiên bản Windows bằng lệnh `winver`. Playbook không chạy trên Build ngoài danh sách; một số Edition và cấu hình phần cứng vẫn chưa được kiểm thử.

## Chức năng và chế độ

Playbook gỡ bớt ứng dụng, điều chỉnh dịch vụ và tác vụ nền, giảm quảng cáo và thu thập dữ liệu. Hình nền, ảnh tài khoản và màn hình khóa được thiết lập khi gói có ảnh đi kèm; kết quả màn hình khóa có thể khác nhau theo Edition Windows.

Giữ lại Defender, Firewall, Store/App Installer và Edge/WebView. Không chủ động tắt Windows Update hoặc dịch vụ Anti-cheat; điều này không đồng nghĩa được bên thứ ba chứng nhận tương thích.

### Standard — cấu hình mặc định

Chọn Standard nếu bạn muốn bắt đầu với cấu hình cơ bản của StrikeOS. Chế độ này vẫn thay đổi sâu vào Windows:

- Tinh gọn ứng dụng, dịch vụ, tác vụ nền và giao diện.
- Điều chỉnh bộ nhớ, ưu tiên ứng dụng đang sử dụng, FTH và BCD/timer; tắt chức năng ghi hình Game DVR.
- Gỡ hoặc tắt các chức năng theo lựa chọn của bạn khi cài.

### Performance

Chọn Performance nếu bạn muốn thử thêm các thiết lập dưới đây và sẵn sàng kiểm tra kết quả trên máy của mình. Chế độ này bao gồm toàn bộ Standard.

- **Mạng:** Đặt TCP Auto-Tuning về `normal`, tắt RSC, kiểm tra RSS và điều chỉnh một số thuộc tính Card mạng. Đặt lại Winsock/IP và xóa bộ nhớ đệm DNS.
- **Nguồn điện:** Chọn High Performance trên Desktop; điều chỉnh Core Parking có phân biệt Laptop và chế độ dùng nguồn.
- **Thiết bị:** Thiết lập HAGS và MSI Mode cho GPU/Card mạng đủ điều kiện. Khả năng hoạt động thực tế phụ thuộc phần cứng và Driver.
- **Storage:** Kiểm tra, bật TRIM khi cần; không chạy Defrag.
- **Timer:** Ép HPET qua BCD, tạo tác vụ chạy tiện ích nền yêu cầu Timer Resolution 0,5 ms.

> [!IMPORTANT]
> Performance không bảo đảm nhanh hơn Standard. Lưu lại IP/DNS riêng và đo trước/sau khi áp dụng. Chạy Standard sau Performance không hoàn tác toàn bộ thay đổi.

## Tùy chọn khi cài

Bỏ chọn những chức năng bạn vẫn sử dụng. Ba mục đầu được tích sẵn.

| Lựa chọn | Mặc định |
|:---|:---:|
| Gỡ/tắt các thành phần OneDrive | Đã chọn |
| Gỡ Xbox và Game Bar | Đã chọn |
| Tắt Windows Search | Đã chọn |
| Tắt Bluetooth | Chưa chọn |
| Tắt in và quét tài liệu | Chưa chọn |
| Tắt cảm ứng, bút và máy tính bảng | Chưa chọn |
| Cài Brave, Firefox hoặc Chrome | Chưa chọn |

- **OneDrive:** Hãy tải tệp cần giữ về máy trước khi chọn. Playbook không tự chuyển dữ liệu và một số bản OneDrive có thể vẫn còn sau khi chạy.
- **Xbox và Search:** Việc gỡ/tắt có thể ảnh hưởng Game Pass, ghi hình và tìm kiếm.
- **Trình duyệt:** Nếu phát hiện trình duyệt đã được cài, Playbook sẽ bỏ qua, không cài sạch hoặc xóa hồ sơ của bạn.

<details>
<summary><strong>Các dịch vụ tiêu biểu được điều chỉnh</strong></summary>

| Nhóm | Dịch vụ | Điều kiện |
|:---|:---|:---|
| Chẩn đoán, báo lỗi | DiagTrack, dmwappushservice, DPS, diagsvc, WerSvc, wercplsupport | Cấu hình chung |
| Hệ thống | SysMain, MapsBroker, RetailDemo, RemoteRegistry, Fax | Cấu hình chung |
| Đồng bộ, thông báo | OneSyncSvc, WpnService, WpnUserService | Cấu hình chung |
| Tìm kiếm | WSearch | Chọn tắt Search |
| Xbox | XblAuthManager, XblGameSave, XboxNetApiSvc, XboxGipSvc, GamingServices, GamingServicesNet | Chọn gỡ Xbox |
| In, quét | Spooler, PrintNotify, StiSvc | Chọn tắt in/quét |
| Bluetooth | bthserv, BTAGService, BthAvctpSvc | Chọn tắt Bluetooth |
| Cảm ứng, bút | TabletInputService | Chọn tắt cảm ứng/bút |

Các dịch vụ trên được tắt khi có trên máy và có thể làm mất chức năng tương ứng. Đồng bộ qua OneSyncSvc, thông báo qua WpnService/WpnUserService và Fax bị tắt trong cả hai chế độ. Bạn cần khởi động lại để các thay đổi có hiệu lực đầy đủ.

</details>

## Runtime

Bạn không cần chọn cài riêng Runtime. Cả hai chế độ đều kiểm tra **Visual C++ 2015–2022 x86/x64**, **DirectX Legacy June 2010** và **.NET Framework 3.5**, bỏ qua thành phần được phát hiện đã có.

Visual C++ và DirectX được tải từ Microsoft, có kiểm tra chữ ký bộ cài. Với .NET 3.5, bạn có thể cần bộ cài Windows phù hợp nếu máy thiếu nguồn cài đặt cục bộ.

Nếu Log ghi `Unavailable` hoặc `SkippedNoSource`, thành phần đó chưa được cài thành công. **Completed không có nghĩa mọi Runtime đã cài đủ.** Kiểm tra Log nếu game vẫn báo thiếu thư viện.

<a id="cai-dat"></a>

## Cài đặt

1. Kiểm tra Build Windows, hoàn tất cập nhật đang chạy và khởi động lại nếu được yêu cầu.
2. Sao lưu hệ thống, dữ liệu; tạo Snapshot nếu dùng máy ảo.
3. Tải AME Wizard từ nguồn chính thức và `.apbx` từ Releases của dự án.
4. Mở `.apbx` bằng AME Wizard, chọn chế độ và kiểm tra các mục tích sẵn.
5. Chờ hoàn tất rồi khởi động lại Windows.

Hãy duy trì Internet và nguồn điện ổn định, sử dụng tài khoản có quyền quản trị. Không chạy đồng thời Windows Update, DISM, trình cài Driver hoặc công cụ tối ưu khác. Bạn không cần chủ động tắt Tamper Protection để làm theo hướng dẫn này.

Nếu gặp lỗi, giữ Log trước khi thử lại. Sau khởi động, chờ khoảng 10–15 phút trước khi đo Process, RAM và hiệu năng.

## Hỗ trợ và cập nhật

Gửi [Issue](https://github.com/nyxvergil/Superstrike-x1/issues) hoặc liên hệ [Discord](https://discord.gg/strikeos), kèm tên tệp Playbook, Build Windows, cấu hình máy, tùy chọn đã chọn và Log đầy đủ. Xóa thông tin cá nhân, Token và khóa sản phẩm trước khi đăng.

Bạn có thể nhận hỗ trợ trong khả năng duy trì dự án; không có cam kết thời gian xử lý hay lịch cập nhật cố định. Nếu sử dụng dịch vụ trả phí, phạm vi hỗ trợ tuân theo thỏa thuận riêng.

Bản mới và hướng dẫn nâng cấp được đăng trong Releases. Playbook không tự cập nhật: hãy đọc hướng dẫn trước khi chạy bản mới lên máy đã tối ưu. Bạn không cần chạy lại sau mỗi lần Windows Update.

## Nguồn tham khảo và giấy phép

Tham khảo cách tổ chức và triển khai từ **AtlasOS, XOS, FSOS, INSIDEXOS, Atom, SapphireOS**; bố cục README tham khảo **ReviOS**. StrikeOS không đại diện hoặc được bảo trợ bởi các dự án này.

Xem [LICENSE](./LICENSE) và giấy phép từng thành phần bên thứ ba trong repository. Ghi nguồn không thay thế nghĩa vụ giấy phép. StrikeOS không cung cấp khóa sản phẩm hoặc công cụ kích hoạt Windows.

---

<p align="center"><strong>SuperStrike X1 · StrikeOS</strong></p>
