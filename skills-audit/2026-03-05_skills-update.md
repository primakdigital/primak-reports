# Skills Update Report — 2026-03-05

## Summary
Skills audit identified 6 gaps between skill content and active operations (state.md 03.03).
3 skills updated. 2 new skills created. Total: 10 skills (was 8).

## Changes Made

### 1. primak-client-intelligence v4.0 -> v5.0
| Item | Before | After |
|------|--------|-------|
| ICA KC | PAUSED (budget gap) | CLOSED (paid) |
| IcanDo | Contract pending | ACTIVE, signed 03.03, 430/hr |
| Momentick | EXIT COMPLETE | ACTIVE (Liberia proposal) |
| Open University | ARCHIVED | ACTIVE (Wed 17:00) |
| Barometer lead | Missing | Added (pricing locked, questionnaire pending) |
| Ifat Lavi lead | Missing | Added (score 95, draft ready) |
| Auto-context triggers | 4 triggers wrong | All corrected |
| Task T012 | Stale (deadline Feb 7) | Replaced with current next action |

### 2. primak-engine-connector v1.0 -> v2.0
- DEPRECATED Google Sheet connector
- Redirected to state.md + Calendar/Gmail MCP
- Legacy Sheet URL preserved as archive reference
- Triggers ("primak status", "morning brief") now read state.md

### 3. primak-pricing-engine v2.1 -> v2.2
- Added Client-Specific Rate Overrides table
- ICA/IcanDo: 430/hr (vs reference 450/hr)
- Formula updated: `TotalHours x [ClientRate or 450]`
- Synced to CLI copy (~/.claude/skills/)

### 4. primak-daily-ops v1.0 (NEW)
- Reads state.md + Calendar + Gmail + AIM Brain
- Produces 3-5 prioritized daily actions
- Triggers: "בוקר טוב", "מה יש היום", "daily"
- Rules: max 5 actions, calendar first, flag stale items, invoice aging alerts
- Integrates with all existing skills

### 5. primak-outreach-tracker v1.0 (NEW)
- 9-stage sequence tracking (INTEL -> DRAFT_READY -> SENT -> WAITING -> REPLIED -> MEETING_SET -> CONNECTED -> STALE -> CLOSED)
- Enforces OSINT-before-draft protocol
- Connector management (Omri, Ayelet, Micha, Didi)
- Escalation logic with time-based triggers
- Decision #3 dependency flagged in every report
- Triggers: "outreach status", "follow-up [name]", "outreach prep [name]"

## Remaining Gaps

| Gap | Priority | Notes |
|-----|----------|-------|
| No financial tracking skill | Low | 3 open invoices, manual tracking in state.md |
| Club D / DriftSense details | Low | Listed as active but no project details in any skill |

## Files Modified
- `/Users/yaniv/primak/_SKILLS/primak-client-intelligence/SKILL.md` (v4.0 -> v5.0)
- `/Users/yaniv/primak/_SKILLS/primak-engine-connector/SKILL.md` (v1.0 -> v2.0 DEPRECATED)
- `/Users/yaniv/primak/_SKILLS/primak-pricing-engine/SKILL.md` (v2.1 -> v2.2)
- `/Users/yaniv/.claude/skills/primak-pricing-engine/SKILL.md` (CLI sync)

## Files Created
- `/Users/yaniv/primak/_SKILLS/primak-daily-ops/SKILL.md` (v1.0)
- `/Users/yaniv/primak/_SKILLS/primak-outreach-tracker/SKILL.md` (v1.0)

---
*Generated manually | PRIMO skills audit v2*
