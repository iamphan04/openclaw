# OpenClaw 🦞 — Trợ lý AI cá nhân trên các thiết bị của bạn

<p align="center">
  <img src="https://raw.githubusercontent.com/openclaw/openclaw/main/docs/assets/openclaw-banner-dark.png" alt="OpenClaw — Trợ lý AI cá nhân" />
</p>

<p align="center">
  <a href="https://github.com/openclaw/openclaw/actions/workflows/ci.yml"><img src="https://img.shields.io/github/actions/workflow/status/openclaw/openclaw/ci.yml?branch=main&style=flat-square&label=CI" alt="CI"></a>
  <a href="https://www.npmjs.com/package/openclaw"><img src="https://img.shields.io/npm/v/openclaw?style=flat-square&label=npm" alt="Phiên bản npm"></a>
  <a href="https://nodejs.org"><img src="https://img.shields.io/node/v/openclaw?style=flat-square" alt="Phiên bản Node.js"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-green?style=flat-square" alt="Giấy phép MIT"></a>
</p>

**OpenClaw** là dự án trợ lý AI mã nguồn mở có thể chạy trên máy tính cá nhân và kết nối với các nền tảng nhắn tin như Telegram, WhatsApp, Discord, Slack và nhiều dịch vụ khác.

Dự án cung cấp một Gateway để quản lý phiên làm việc, công cụ, sự kiện và kết nối giữa trợ lý AI với các kênh giao tiếp.

Đây là **bản fork cá nhân** từ dự án [OpenClaw gốc](https://github.com/openclaw/openclaw), phục vụ mục đích học tập, tìm hiểu kiến trúc AI Agent và thử nghiệm phát triển các tính năng mới.

> **Lưu ý:** Các tính năng tùy chỉnh được đề cập trong phần định hướng phát triển là ý tưởng dự kiến, không đồng nghĩa chúng đã được triển khai trong repository này.

## 🎯 Mục tiêu dự án

- Tìm hiểu cách xây dựng và vận hành một trợ lý AI cá nhân.
- Nghiên cứu kiến trúc Gateway, phiên hội thoại, công cụ và hệ thống mở rộng.
- Thực hành cài đặt, cấu hình, kiểm thử và phát triển dự án mã nguồn mở.
- Từng bước thử nghiệm các tính năng hỗ trợ học tập và nghiên cứu bằng tiếng Việt.

## 💡 Ý tưởng phát triển: ResearchMate VN

Một hướng phát triển dự kiến là **ResearchMate VN** — trợ lý AI hỗ trợ sinh viên trong quá trình tìm kiếm, đọc và tìm hiểu tài liệu nghiên cứu.

Các tính năng có thể phát triển theo từng giai đoạn:

- **Tóm tắt bài báo khoa học:** trình bày nội dung chính bằng tiếng Việt.
- **Phân tích nghiên cứu:** xác định mục tiêu, phương pháp, dữ liệu, kết quả và hạn chế của bài báo.
- **Tìm kiếm tài liệu:** gợi ý từ khóa để tìm các nghiên cứu liên quan.
- **Quản lý ghi chú:** lưu thông tin nghiên cứu dưới dạng Markdown.
- **Hỗ trợ học tập:** giải thích thuật ngữ và khái niệm AI/NLP bằng ngôn ngữ dễ hiểu.

Đây là định hướng thử nghiệm nhằm tận dụng kiến trúc mở rộng của OpenClaw, không phải danh sách tính năng đã hoàn thành.

## ✨ Các khả năng chính của OpenClaw

Tùy thuộc vào cấu hình, mô hình AI và công cụ được bật, OpenClaw hỗ trợ:

- **Trò chuyện với AI:** tương tác thông qua các kênh nhắn tin được hỗ trợ.
- **Gateway:** quản lý phiên làm việc, sự kiện, công cụ và kết nối.
- **Nhiều nhà cung cấp mô hình:** lựa chọn dịch vụ AI hoặc mô hình cục bộ tương thích.
- **Tools và Skills:** mở rộng khả năng của trợ lý thông qua công cụ và quy trình chuyên biệt.
- **Plugins:** tích hợp thêm chức năng theo kiến trúc mở rộng.
- **Giao diện điều khiển:** quản lý và tương tác qua Control UI, CLI hoặc TUI.

Tìm hiểu thêm tại [tài liệu OpenClaw](https://docs.openclaw.ai/).

## 🧱 Kiến trúc tổng quan

- **Gateway:** lớp điều khiển trung tâm, quản lý phiên, công cụ, sự kiện và kết nối.
- **Channels:** kết nối trợ lý với các nền tảng nhắn tin.
- **Control UI / CLI / TUI:** giao diện để cấu hình và tương tác với Gateway.
- **Model Providers:** cung cấp mô hình AI để xử lý yêu cầu.
- **Tools, Skills và Plugins:** bổ sung khả năng cho trợ lý.

Tài liệu tham khảo:

- [Kiến trúc hệ thống](https://docs.openclaw.ai/concepts/architecture)
- [Gateway](https://docs.openclaw.ai/gateway)
- [Kênh giao tiếp](https://docs.openclaw.ai/channels)
- [Tools và Skills](https://docs.openclaw.ai/tools)
- [Plugins](https://docs.openclaw.ai/plugins)

## ⚙️ Cài đặt

OpenClaw hỗ trợ nhiều phương thức cài đặt tùy hệ điều hành. Hãy xem [hướng dẫn cài đặt chính thức](https://docs.openclaw.ai/install) để kiểm tra yêu cầu phiên bản mới nhất.

### macOS, Linux hoặc WSL2

```bash
curl -fsSL https://openclaw.ai/install.sh | bash
```

### Windows PowerShell

```powershell
iwr -useb https://openclaw.ai/install.ps1 | iex
```

### Cài đặt bằng npm

Nếu máy đã cài Node.js phiên bản tương thích:

```bash
npm install -g openclaw@latest --allow-scripts=openclaw
```

Các yêu cầu về phiên bản Node.js và npm có thể thay đổi. Hãy ưu tiên làm theo [tài liệu cài đặt](https://docs.openclaw.ai/install).

## 🚀 Khởi tạo và sử dụng

Sau khi cài đặt, chạy trình hướng dẫn cấu hình:

```bash
openclaw onboard --install-daemon
```

Kiểm tra trạng thái Gateway:

```bash
openclaw gateway status
```

Mở giao diện điều khiển:

```bash
openclaw dashboard
```

Làm theo hướng dẫn để cấu hình nhà cung cấp mô hình AI và kết nối các kênh cần sử dụng.

Tham khảo [hướng dẫn bắt đầu](https://docs.openclaw.ai/start/getting-started) nếu gặp vấn đề trong quá trình thiết lập.

## 🧑‍💻 Phát triển từ mã nguồn

Repository sử dụng **pnpm workspace**. Không dùng `npm install` tại thư mục gốc để cài toàn bộ dự án.

```bash
git clone https://github.com/iamphan04/openclaw.git
cd openclaw
pnpm install
pnpm build
pnpm ui:build
```

Đây là quy trình phát triển cơ bản; tùy phiên bản, dự án có thể yêu cầu thêm công cụ hoặc bước cấu hình.

- [Hướng dẫn thiết lập môi trường](https://docs.openclaw.ai/start/setup)
- [Hướng dẫn đóng góp](CONTRIBUTING.md)

## 🔐 Bảo mật và quyền riêng tư

Trợ lý AI có thể được cấp quyền sử dụng công cụ trên máy chạy Gateway. Vì vậy, cần cấu hình cẩn thận trước khi sử dụng.

- Xem tin nhắn và nội dung từ bên ngoài là dữ liệu không đáng tin cậy.
- Không đưa token, khóa API hoặc mật khẩu vào mã nguồn công khai.
- Kiểm tra quyền của Tools, Skills và Plugins trước khi bật.
- Không mở Gateway ra Internet hoặc cho người khác sử dụng nếu chưa hiểu rõ cơ chế xác thực và bảo mật.
- Đọc hướng dẫn sandbox trước khi thử nghiệm công cụ có thể tác động đến hệ thống.

Tài liệu bảo mật:

- [Hướng dẫn bảo mật](https://docs.openclaw.ai/gateway/security)
- [Hướng dẫn sandbox](https://docs.openclaw.ai/gateway/sandboxing)
- [Quy trình xử lý khi Gateway bị lộ](https://docs.openclaw.ai/gateway/security/exposure-runbook)

## 🗺️ Lộ trình phát triển dự kiến

Các mục dưới đây là kế hoạch tham khảo. Chỉ đánh dấu hoàn thành sau khi đã triển khai và kiểm tra thực tế.

- [ ] Cài đặt và chạy OpenClaw trong môi trường phát triển.
- [ ] Tìm hiểu cấu trúc Gateway, Tools, Skills và Plugins.
- [ ] Xây dựng một Skill thử nghiệm.
- [ ] Thử nghiệm quy trình đọc và tóm tắt tài liệu nghiên cứu.
- [ ] Lưu kết quả và ghi chú dưới dạng Markdown.
- [ ] Viết kiểm thử và ghi lại giới hạn của các tính năng thử nghiệm.

## 📚 Tài liệu tham khảo

| Nội dung | Liên kết |
|---|---|
| Trang chủ | [openclaw.ai](https://openclaw.ai) |
| Tài liệu chính thức | [docs.openclaw.ai](https://docs.openclaw.ai) |
| Hướng dẫn bắt đầu | [Getting Started](https://docs.openclaw.ai/start/getting-started) |
| Nhà cung cấp mô hình AI | [Model Providers](https://docs.openclaw.ai/concepts/model-providers) |
| CLI | [CLI Reference](https://docs.openclaw.ai/cli) |
| Skills | [Skills](https://docs.openclaw.ai/tools/skills) |
| Plugins | [Plugins](https://docs.openclaw.ai/plugins) |
| Đóng góp | [CONTRIBUTING.md](CONTRIBUTING.md) |

## 🙌 Nguồn gốc dự án

Repository này được fork từ [openclaw/openclaw](https://github.com/openclaw/openclaw). OpenClaw là dự án mã nguồn mở được phát triển bởi đội ngũ và cộng đồng của dự án gốc.

Bản fork này không đại diện cho dự án chính thức và có thể khác với phiên bản gốc theo thời gian.

Vui lòng tham khảo các tệp giấy phép và thông báo bản quyền trong repository trước khi phân phối hoặc chỉnh sửa mã nguồn.

- **Dự án gốc:** https://github.com/openclaw/openclaw
- **Tài liệu:** https://docs.openclaw.ai
- **Giấy phép:** [LICENSE](LICENSE)
- **Thông báo mã nguồn bên thứ ba:** [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md)

---

<p align="center">
  Được xây dựng để học hỏi, thử nghiệm và phát triển trợ lý AI cá nhân 🦞
</p>
