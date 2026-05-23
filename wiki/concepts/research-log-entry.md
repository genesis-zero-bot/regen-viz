---
title: "Research Log Entry"
type: concept
status: active
updated: 2026-05-23
---

# Research Log Entry

Standardized format for capturing research artifacts before Telegram delivery.

## Fields

**Date:** YYYY-MM-DD (auto from session)

**Topic:** One line. What this research is about in plain language.

**Question:** What prompted it. Not the URL — the underlying question.

**Key Findings:** 3-6 bullets. What transfers. Each should be actionable, not just informational.

**Regenerative Community Application:** Specific. Which community, which module, which problem.

**Next Steps:** 1-3 concrete actions. Not "more research."

**Related:** Links to prior research or wiki pages that this connects to.

**Saved:** Checkboxes — Wiki / Knowledge Graph / GitHub

## Workflow Order

1. Research log entry created FIRST (before Telegram send)
2. Wiki source page created
3. Knowledge graph capture (capture.sh with log entry as doc)
4. ADR if architectural decision emerges
5. Telegram message last (output only)

## Usage

The log entry gates artifact selection. Fields determine:
- Wiki only: topic is reference material
- KG capture: concepts/relations worth preserving
- ADR: architectural decision being formalized
- Spec/Gherkin: behavior being specified

Telegram is output, not storage. If it stays in Telegram only, research is wasted.

## References

- wiki/sources/dca-forum.md (DCAF research as example)
- docs/adr/0010-data-centric-myuconet-knowledge-layer.md (ADR from research)