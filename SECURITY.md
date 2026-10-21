# Bảo mật

## Báo lỗ hổng

Vui lòng **không mở issue công khai**. Gửi riêng tới **kythuat@hvn.vn** hoặc qua
[GitHub Security Advisories](https://github.com/hvngroup/app-ai-switch-releases/security/advisories/new),
kèm phiên bản bị ảnh hưởng và các bước tái hiện. HVN GROUP phản hồi trong vài ngày làm việc và
ghi công người báo trong release notes nếu anh/chị muốn.

Không gửi kèm token, file đăng nhập (`.credentials.json`, `auth.json`), file trong
`~/.pitstop/vault/`, dữ liệu nội bộ hay dữ liệu khách hàng.

## Ứng dụng xử lý dữ liệu thế nào

- **Login được lưu trên máy:** login của từng tài khoản được mã hoá AES-256-GCM trong
  `~/.pitstop/vault/`; khoá nằm trong macOS Keychain, Windows Credential Manager hoặc keyring
  của Linux. Chỉ chủ tài khoản máy đọc được các thư mục này.
- **Login chỉ gửi tới nơi đã cấp nó** (Anthropic, OpenAI hoặc Cursor) để đọc mức dùng của
  tài khoản đó, và khi bật Warm-up, một tin nhắn ngắn cho mỗi tài khoản Claude Code đã chọn.
  Không có máy chủ của HVN và không thu thập dữ liệu sử dụng.
- **Các kết nối khác:** mỗi ngày tải bảng giá công khai của LiteLLM từ GitHub (không gửi gì),
  và nếu không tắt **Cập nhật**, vài giờ một lần xem bản phát hành mới nhất ở repo này.
- **Cập nhật:** chỉ cài khi người dùng đồng ý, và chỉ khi gói cài mang chữ ký bằng khoá
  cập nhật của HVN. Bản macOS được ký Developer ID của HVN GROUP và notarize bởi Apple.

## Phiên bản được hỗ trợ

Chỉ bản phát hành mới nhất được vá lỗi.

---

HVN GROUP · hvn.vn
