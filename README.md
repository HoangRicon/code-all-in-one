# Quy trình code 1 lệnh cho AI Agent Coding

Quy trình phát triển chuyên nghiệp: **Spec → Plan → Design → Implement → Verify**

---

## Cài đặt

Tải folder `skills/` và `rules/`về, copy vào `.cursor` hoặc `.agent` trong thư mục home:


---

## 5 Skill chính

| Project | GitHub | Version | Role |
|---------|--------|---------|------|
| Spec-Kit | `github/spec-kit` | v0.7.1 | Spec-driven framework (uv) |
| OpenSpec | `Fission-AI/OpenSpec` | v1.2.0 | Lightweight workflow (npm) |
| Superpowers | `obra/superpowers` | v5.0.7 | TDD + review + subagents |
| planning-with-files | `OthmanAdi/planning-with-files` | v2.30.0 | File-based planning |
| ui-ux-pro-max | `nextlevelbuilder/ui-ux-pro-max-skill` | v2.5.0 | UI/UX design system |

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

---

## Cách sử dụng

### Commands

| Lệnh | Mô tả |
|------|--------|
| `/super-spec` | Full workflow (auto mode + auto complexity) |
| `/super-spec force-spec-kit` | Force Spec-Kit mode |
| `/super-spec force-openspec` | Force OpenSpec mode |
| `/super-spec reset` | Reset mode selection |
| `/super-spec upgrade` | Check & update all integrated projects |

### Luồng hoạt động

```
/super-spec
    ↓
Mode Selection → Complexity Triage → Session Recovery (auto)
    ↓
Specification (G1, inline spec review)
    ↓
Persistent Planning (G2, inline plan review + file structure mapping)
    ↓
UI/UX Design (G3, conditional, v2.5.0 intelligent design system)
    ↓
TDD Implementation (G4, model selection + implementer status)
    ↓
Archive (+ MemPalace persistence)
```

---

## Quick Start

1. Copy `skills/` vào `~/.cursor/` hoặc `~/.agent/`
2. Gõ `/super-spec` để bắt đầu
3. Làm theo các Gates (G1→G2→G3→G4)

---

**Version:** 2026.07.29
