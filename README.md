# Superpowers Skills for Cursor AI Agent

Quy trình phát triển chuyên nghiệp: **Spec → Plan → Design → Implement → Verify**

---

## Cài đặt

Tải folder `skills/` và `rules/`về, copy vào `.cursor` hoặc `.agent` trong thư mục home:


---

## Integrated Projects

| Project | GitHub | Version | Role |
|---------|--------|---------|------|
| Spec-Kit | `github/spec-kit` | v0.7.1 | Spec-driven framework (uv) |
| OpenSpec | `Fission-AI/OpenSpec` | v1.2.0 | Lightweight workflow (npm) |
| Superpowers | `obra/superpowers` | v5.0.7 | TDD + review + subagents |
| planning-with-files | `OthmanAdi/planning-with-files` | v2.30.0 | File-based planning |
| ui-ux-pro-max | `nextlevelbuilder/ui-ux-pro-max-skill` | v2.5.0 | UI/UX design system |

---

## 5 Skill Chính

### 1. spec-first-superpowers
**Orchestrator** - Điều khiển toàn bộ workflow

- `/super-spec` - Bắt đầu với auto mode detection
- Auto-select: Spec-Kit vs OpenSpec
- Quality Gates (G1-G4) - Không cho phép skip phases
- Commands: `/super-spec`, `/super-spec force-spec-kit`, `/super-spec force-openspec`, `/super-spec upgrade`

### 2. planning-with-files
**Planning** - Lưu progress vào file

- Tạo `task_plan.md`, `findings.md`, `progress.md`
- Hooks tự động cập nhật progress
- Recovery sau `/clear`
- Scripts: `init-session`, `check-complete`, `attest-plan`

### 3. subagent-driven-development
**Implementation** - Execute plan với subagents

- Fresh subagent per task
- Two-stage review: Spec compliance → Code quality
- Continuous execution (không pause)
- Status: DONE / DONE_WITH_CONCERNS / NEEDS_CONTEXT / BLOCKED

### 4. test-driven-development
**TDD** - Red-Green-Refactor cycle

- RED: Write failing test
- GREEN: Write minimal code
- REFACTOR: Clean up
- Iron Law: Không code không có failing test

### 5. systematic-debugging
**Debug** - Root cause investigation

- 4 Phases: Root Cause → Pattern → Hypothesis → Implementation
- Iron Law: Không fix không có root cause
- 3-Strike protocol

---

## Workflow

```
SPEC FIRST (/super-spec)
    ↓ G1 Gate
PLAN (planning-with-files)
    ↓ G2 Gate
DESIGN UI (ui-ux-pro-max) [optional]
    ↓ G3 Gate
IMPLEMENT (subagent-driven + TDD)
    ↓ G4 Gate
VERIFY (verification-before-completion)
    ↓
FINISH (finishing-a-development-branch)
```

---

## Quick Start

1. Copy `skills/` vào `~/.agents`
2. Gõ `/super-spec` để bắt đầu
3. Làm theo các Gates (G1→G2→G3→G4)

---

**Version:** 2026.07.29
