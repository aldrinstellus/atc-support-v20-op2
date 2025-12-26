# PROJECT SAVEPOINT: V20-OP2 Clone Session
**Date:** 2025-12-26
**Time:** 4:55 PM (UTC+4)
**Session:** Windows Laptop Development
**Project:** atc-support-v20-op2
**GitHub:** https://github.com/aldrinstellus/atc-support-v20-op2

---

## Session Summary

This session continued from the V20 UI fixes session. After fixing bugs in V20, the project was cloned to V20-OP2 as an independent development branch.

## What Was Done

### 1. V20-OP2 Clone Created
- Cloned `atc-support-v20` to `atc-support-v20-op2`
- Created new GitHub repo: `aldrinstellus/atc-support-v20-op2`
- Updated package.json name to `atc-support-v20-op2`
- Full git history preserved

### 2. Dev Servers Running
| Project | Port | Status |
|---------|------|--------|
| V18 | 3019 | Running |
| V20 | 3020 | Running |
| V20-OP2 | 3021 | Running |

### 3. Browser Automation Best Practices Documented

Added comprehensive guide to `CLAUDE.md` covering:

#### Tool Selection Guide
| Tool | Best For |
|------|----------|
| Chrome DevTools MCP | Debugging with existing logins/sessions |
| Puppeteer MCP | Clean isolated testing, screenshots |
| Playwright MCP | Multi-browser, accessibility snapshots |

#### Decision Flow
1. Need existing login/session? → Chrome DevTools MCP
2. Need clean isolated test? → Puppeteer MCP
3. Need accessibility snapshots? → Playwright MCP
4. Need multi-browser? → Playwright MCP
5. Default for debugging → Chrome DevTools MCP
6. Fallback → Puppeteer MCP

### 4. Memory MCP Updated
- Saved "Browser Automation Best Practices" entity
- Available for quick recall in future sessions

---

## Files Modified

| File | Location | Changes |
|------|----------|---------|
| `CLAUDE.md` | `C:\Users\Administrator\` | Added browser automation best practices |
| `package.json` | v20-op2 | Updated project name |
| `CLAUDE.md` | v20-op2 | Updated GitHub references |

---

## Git Status

### V20-OP2 Commits
```
a3157ab chore: Update project name to atc-support-v20-op2
bcb186b docs: Add savepoint for V20 UI fixes session
0bbd261 docs: Add file editing best practices
eb94e65 Add sidebar toggle and theme toggle
c65da44 Fix mode switcher hydration issue
07a70d3 Fix duplicate chat input layer
```

### Claude-Sync Updates
- `CLAUDE.md` with browser automation best practices

---

## Verified Working

- V20-OP2 running on http://localhost:3021
- All UI fixes present (sidebar toggle, theme toggle, mode switcher)
- Puppeteer MCP successfully took screenshot
- All 3 dev servers running in parallel

---

## Key Learnings

### Browser Automation Tools
- **Chrome DevTools MCP** connects to YOUR existing Chrome (keeps sessions)
- **Puppeteer MCP** launches isolated Chromium (clean state)
- **Playwright MCP** best for accessibility snapshots

### File Editing (from earlier session)
- Never use bash heredoc for JSX/TSX (escapes backticks)
- Always use Edit tool for modifications
- Re-read file if Edit fails with "modified" error

---

**Session Status:** COMPLETE
**All Changes:** DOCUMENTED
