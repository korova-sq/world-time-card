# Release v1.2.0

**Title:** v1.2.0 — Renamed to World Time Card (`world-time-card`)

## Notes

### ⚠️ Breaking change: the card has been renamed

To avoid a clash with another card in the HACS catalog, the card, its editor and the repository now use unique names.

| | Before | Now |
|---|---|---|
| Card type | `custom:world-clock-card` | `custom:world-time-card` |
| JS file | `world-clock-card.js` | `world-time-card.js` |
| Repository | `korova-sq/world-clock-card` | `korova-sq/world-time-card` |

**How to migrate**
1. In HACS, remove the old card and install **World Time Card** again (or re-download it).
2. If you installed it manually, change the resource URL to `/local/world-time-card.js`.
3. In your dashboards, change `type: custom:world-clock-card` to `type: custom:world-time-card`.

All options and all `--wc-*` card-mod variables are unchanged.

### Fixes
- The editor hint now correctly says **up to two** secondary time zones (it said three).
- Small hardening: the background image URL is sanitized before it is used in CSS, and the overlay value is always handled as a number.

---

**Commit message (<50 chars):** `Rename to world-time-card, fix tz hint (v1.2.0)`
