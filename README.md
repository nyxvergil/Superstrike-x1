<p align="center">
  <a href="https://strikeos.site">
    <img src="./strike-logo.png" alt="StrikeOS" width="760">
  </a>
</p>

<p align="center">
  <strong>Tinh gọn Windows cho máy chơi game.</strong>
</p>

<p align="center">
  <img alt="Version" src="https://img.shields.io/badge/VERSION-2.0.17-5B21FF?style=for-the-badge">
  <img alt="Revision" src="https://img.shields.io/badge/REV-PERFORMANCE12--VI-2563EB?style=for-the-badge">
  <img alt="Status" src="https://img.shields.io/badge/STATUS-TEST-F59E0B?style=for-the-badge">
  <img alt="AME" src="https://img.shields.io/badge/AME-PLAYBOOK-202020?style=for-the-badge">
</p>

<p align="center">
  <a href="https://strikeos.site">🌐 Website</a>
  &nbsp;·&nbsp;
  <a href="https://discord.gg/strikeos">💬 Discord</a>
  &nbsp;·&nbsp;
  <a href="#cai-dat">📥 Cài đặt</a>
  &nbsp;·&nbsp;
  <a href="#ho-tro">🛠️ Hỗ trợ</a>
</p>

---

## 🎮 Giới thiệu

**SuperStrike X1** là Playbook tối ưu Windows qua AME Wizard, áp dụng trực tiếp trên hệ điều hành đang dùng.

Tôi phát triển StrikeOS để giảm hoạt động nền và điều chỉnh Windows cho nhu cầu chơi game. Process thấp là mục tiêu, nhưng hiệu năng thực tế vẫn phải đo bằng FPS, 1% Low, 0.1% Low và Frame Time.

## 🪟 Windows hỗ trợ

| Hệ điều hành | Phiên bản | Build |
|:---|:---:|:---:|
| Windows 10 x64 | 22H2 | `19045` |
| Windows 11 x64 | 24H2 | `26100` |
| Windows 11 x64 | 25H2 | `26200` |

Đây là **bản test**. Không phải mọi Edition, Driver và cấu hình máy đều đã được kiểm thử.

## ✨ Chức năng

- Gỡ ứng dụng và một số thành phần Windows không cần dùng.
- Điều chỉnh dịch vụ, Scheduled Task và Service Host để giảm hoạt động nền.
- Giảm quảng cáo, nội dung đề xuất và thu thập dữ liệu.
- Áp dụng hình nền, ảnh tài khoản và chính sách màn hình khóa khi có ảnh đi kèm.
- Tự kiểm tra Visual C++, DirectX Legacy và .NET Framework 3.5.
- Cho phép cài Brave, Firefox hoặc Chrome.

Giữ lại Defender, Firewall, Store/App Installer và Edge/WebView. Không chủ động tắt Windows Update hoặc các dịch vụ Anti-cheat.

## ⚙️ Chế độ

| Chế độ | Nội dung |
|:---|:---|
| 🛡️ **Standard** | Cấu hình nền Gaming Lean: Debloat, dịch vụ, bộ nhớ, FTH và BCD/timer. Đây là lựa chọn mặc định. |
| 🚀 **Performance** | Thêm TRIM, RSS, TCP Auto-Tuning, tắt RSC, thiết lập Card mạng, nguồn điện, Core Parking, HAGS và MSI Mode theo điều kiện thiết bị. Có ép HPET, tiện ích Timer Resolution chạy nền và reset Winsock/IP, DNS cache. |

> [!WARNING]
> Performance không mặc nhiên nhanh hơn Standard. Kết quả phụ thuộc phần cứng; một số thay đổi có thể tăng điện năng hoặc giảm hiệu năng. Chạy Standard sau Performance không hoàn tác các thay đổi trước đó.

## 🧩 Tùy chọn

| Lựa chọn | Mặc định |
|:---|:---:|
| Gỡ OneDrive | ✅ |
| Gỡ Xbox và Game Bar | ✅ |
| Tắt Windows Search | ✅ |
| Tắt Bluetooth | ⬜ |
| Tắt in, quét tài liệu | ⬜ |
| Tắt cảm ứng, bút và máy tính bảng | ⬜ |
| Cài trình duyệt | ⬜ |

Bỏ chọn những chức năng bạn còn dùng. Sao lưu tệp OneDrive về máy trước khi gỡ.

<a id="cai-dat"></a>

## 📥 Cài đặt

1. Sao lưu hệ thống hoặc tạo Snapshot trên máy ảo.
2. Tải `.apbx` từ **Releases**, đọc ghi chú của bản phát hành.
3. Mở bằng **AME Wizard**, chọn chế độ và các tùy chọn.
4. Chờ hoàn tất rồi khởi động lại Windows.

Cần Internet, quyền quản trị viên và nguồn điện ổn định. Không chạy đồng thời Windows Update, trình cài Driver hoặc công cụ tối ưu khác.

> [!NOTE]
> Runtime đã có sẽ được bỏ qua. Nếu thiếu nguồn hoặc cài thất bại, Log có thể ghi `Unavailable` hoặc `SkippedNoSource` và Playbook vẫn tiếp tục. Completed không có nghĩa mọi Runtime đã cài đủ.

## 📊 Kỳ vọng và khôi phục

Không cam kết mức FPS, RAM, số Process cố định hoặc tương thích mọi bản cập nhật Anti-cheat. Hãy đo trước và sau trên cùng cấu hình.

Playbook **không tự sao lưu và chưa có hoàn tác toàn bộ**. Muốn trở về đúng trạng thái ban đầu, dùng bản sao lưu hệ thống hoặc Snapshot.

<a id="ho-tro"></a>

## 🛠️ Hỗ trợ

Báo lỗi qua **GitHub Issues** hoặc **Discord**, kèm:

- Tên tệp `.apbx`, Build Windows và cấu hình máy.
- Chế độ, các tùy chọn đã chọn và cách tái hiện lỗi.
- Log đầy đủ của AME Wizard; báo cáo Post-boot nếu có.

Tôi ưu tiên lỗi Action và lỗi mất chức năng có thể tái hiện. Hỗ trợ miễn phí theo khả năng duy trì dự án, không cam kết thời gian phản hồi hoặc tối ưu riêng từng máy.

## 📌 Cập nhật

Bản mới và hướng dẫn nâng cấp được công bố trong **Releases**, không có lịch cố định hay cơ chế tự cập nhật riêng.

Đọc hướng dẫn trước khi chạy chồng phiên bản. Windows Update và Driver có thể thay đổi một số thiết lập; không cần tự động chạy lại Playbook sau mỗi lần cập nhật.

## 📚 Nguồn tham khảo

Tham khảo cách tổ chức và triển khai từ **AtlasOS, XOS, FSOS, INSIDEXOS, Atom, SapphireOS**; bố cục README tham khảo **ReviOS**.

StrikeOS không đại diện hoặc được bảo trợ bởi các dự án trên. Mã nguồn bên thứ ba chịu điều kiện giấy phép tương ứng.

## 📄 Giấy phép

Xem [LICENSE](./LICENSE). StrikeOS không cung cấp khóa sản phẩm hoặc công cụ kích hoạt Windows.

---

<p align="center">
  <strong>SuperStrike X1 · StrikeOS</strong>
</p>
