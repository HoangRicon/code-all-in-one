# Quy trình code 1 lệnh cho AI Agent Coding (Dịch thuật đơn giản từ src Trung Quốc)

Quy trình phát triển chuyên nghiệp: **Spec → Plan → Design → Implement → Verify**

1 LỆNH DÙNG CHO MỌI TÌNH HUỐNG TRONG LẬP TRÌNH
---

## Cài đặt

Tải folder `skills/` và `rules/`về, copy vào `.cursor` hoặc `.agent` hoặc . gì đó của IDE bạn sử dụng trong thư mục home:

Nếu AI Agent của IDE hỗ trợ thao tác với file hệ thống, bạn có thể yêu cầu nó tự cài đặt.


---

## 5 Module cốt lõi

| Project | GitHub | Role |
|---------|--------|---------|------|
| Spec-Kit | `github/spec-kit` | Spec-driven framework (uv) |
| OpenSpec | `Fission-AI/OpenSpec`  | Lightweight workflow (npm) |
| Superpowers | `obra/superpowers` | TDD + review + subagents |
| planning-with-files | `OthmanAdi/planning-with-files` | File-based planning |
| ui-ux-pro-max | `nextlevelbuilder/ui-ux-pro-max-skill` | UI/UX design system |

---
## Workflow

```
SPEC FIRST (/super-spec)
    ↓ G1 Gate
PLAN (planning-with-files)
    ↓ G2 Gate
DESIGN UI (ui-ux-pro-max) [tùy chọn]
    ↓ G3 Gate
IMPLEMENT (subagent-driven + TDD)
    ↓ G4 Gate
VERIFY (verification-before-completion)
    ↓
FINISH (finishing-a-development-branch)
```
Ở mỗi GATE check Pass?
 ├── Yes → Finish
 └── No  → Back to Plan / Implement
---

## Cách sử dụng

### Commands

| Lệnh | Mô tả |
|------|--------|
| `/super-spec` hoặc `/spec-first-superpowers` | Full workflow (auto mode + auto complexity) |
| `/super-spec force-spec-kit` | Bắt buộc chọn Spec-Kit mode |
| `/super-spec force-openspec` | Bắt buộc chọn OpenSpec mode |
| `/super-spec reset` | Reset mode selection |
| `/super-spec upgrade` | Check & update all integrated projects |

### Luồng hoạt động

```
/super-spec
    ↓
Chọn Mode → Đánh giá Độ phức tạp → Khôi phục Session (auto)
    ↓
Viết Spec (G1, inline spec review)
    ↓
Lên kế hoạch (G2, inline plan review + file structure mapping)
    ↓
Thiết kế UI/UX (G3, tùy chọn, v2.5.0 intelligent design system)
    ↓
Implement theo TDD (G4, model selection + implementer status)
    ↓
Archive (+ MemPalace persistence)
```

---

## Quick Start

1. Copy `skills/` vào `~/.cursor/` hoặc `~/.agent/`
2. Gõ `/super-spec` hoặc `/spec-first-superpowers`  để bắt đầu
3. Làm theo các Gates (G1→G2→G3→G4)

---

**Version:** 2026.07.29
