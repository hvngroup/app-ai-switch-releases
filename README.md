# HVN AI Switch — bản phát hành

HVN AI Switch là ứng dụng nằm trên thanh menu (macOS) hoặc khay hệ thống (Windows, Linux)
để đổi nhanh giữa nhiều tài khoản **Claude Code**, **Codex**, **Cursor** và
**Antigravity**, xem hạn mức của từng tài khoản và tự động chuyển trước khi hết.

Repo này chỉ chứa bản phát hành và kênh cập nhật của ứng dụng. Mã nguồn được quản lý
riêng tại HVN GROUP.

## Tải về

Tải bản mới nhất ở trang [Releases](https://github.com/hvngroup/app-ai-switch-releases/releases/latest):

| Máy | File |
|---|---|
| Mac chip Apple (M1 trở lên) | `HVNAISwitch-macos-arm64.dmg` |
| Mac Intel | `HVNAISwitch-macos-x64.dmg` |
| Windows 10/11 (64-bit) | `HVNAISwitch-windows-x64-setup.exe` hoặc bản portable `.zip` |
| Windows 11 trên chip ARM | `HVNAISwitch-windows-arm64-setup.exe` hoặc bản portable `.zip` |
| Linux (x64) | `HVNAISwitch-linux-x64.AppImage` hoặc `HVNAISwitch-linux-x64.deb` |

Dòng lệnh `hvn-switch` có gói riêng (`hvn-switch-cli-*.tar.gz`). Mỗi file có một file
`.sha256` đi kèm để đối chiếu. File `.sig` và `latest.json` dành cho trình cập nhật của
ứng dụng.

## Cài đặt

**macOS.** Mở file `.dmg`, kéo **HVN AI Switch** vào **Applications** rồi mở. Bản phát hành
được ký bằng Developer ID của HVN GROUP và đã qua notarize của Apple. Ứng dụng nằm trên
thanh menu, không có biểu tượng ở Dock cho tới khi mở cửa sổ.

Nếu một bản cũ chưa notarize bị macOS chặn: bấm **Done** (đừng bấm **Move to Trash**), vào
**System Settings → Privacy & Security** và bấm **Open Anyway**. Nếu macOS báo ứng dụng
"is damaged", chạy lệnh sau trong Terminal rồi mở lại:
`xattr -dr com.apple.quarantine "/Applications/HVN AI Switch.app"`

**Windows.** Chạy file setup. SmartScreen báo ứng dụng lạ thì bấm **More info → Run
anyway**.

**Linux.** AppImage: `chmod +x HVNAISwitch-linux-x64.AppImage` rồi chạy. Gói `.deb`:
`sudo apt install ./HVNAISwitch-linux-x64.deb`. Biểu tượng trên thanh hệ thống cần
AppIndicator (GNOME: cài extension AppIndicator).

## Cập nhật

Bản cài bằng setup (Windows), bản trong Applications (Mac) và AppImage (Linux) tự tìm và
cài bản mới từ repo này. Bản portable và gói `.deb` cập nhật bằng tay.

**Đang dùng bản 0.6 hoặc 0.7?** Các bản này tìm cập nhật ở địa chỉ cũ, nay không còn dùng.
Hãy tải bản mới nhất ở trên về và cài đè một lần; từ đó ứng dụng tự cập nhật từ repo này.
Tài khoản và cài đặt được giữ nguyên.

## Báo lỗi và hỗ trợ

- Báo lỗi hoặc góp ý: mở [issue](https://github.com/hvngroup/app-ai-switch-releases/issues/new/choose).
  Ghi kèm phần **Cài đặt → Giới thiệu → Sao chép thông tin** của ứng dụng.
- Lỗ hổng bảo mật: gửi qua
  [security advisory riêng](https://github.com/hvngroup/app-ai-switch-releases/security/advisories/new),
  đừng mở issue công khai. Cách ứng dụng xử lý dữ liệu: [SECURITY.md](SECURITY.md).
- Hỗ trợ kỹ thuật: kythuat@hvn.vn · Hotline 024.9999.7777

## Giấy phép

MIT kèm Commons Clause: được dùng, sửa và chia sẻ miễn phí, giữ thông báo giấy phép, nhưng
không được bán. Xem [LICENSE](LICENSE).

---

HVN GROUP · [hvn.vn](https://hvn.vn)
