# Project Log: Portfolio Website (Serhii Hirus)

## Current Status & Next Steps
- **Status**: Removed link from AI Strategy Co-pilot header; converted `hirus.systems` project attribution into clean text without border/pill frame; completely removed proprietary internal engine terminology (`Strategy Lab Engine`, `Strategy & StrategyResult`, `Strategy Blueprint`, `_generate_signals`, `sl_price`) in favor of standard algorithmic engineering concepts.
- **Brand Palette (Apps only)**:
  - AI Strategy Co-pilot: Tech Red (`#dc2626`)
  - Automated Content Creator: Telegram Blue (`#0088cc`)
  - AI-copilot для CRM: Emerald Green (`#059669`)
- **Local Preview**: Running on `http://localhost:8000`.
- **Next Steps**: Await user visual inspection and feedback.

## Architectural Decisions & Changelog
- **2026-10-22**: Removed proprietary engine jargon across descriptions, i18n, prompts, and code templates (`Strategy Lab`, `StrategyResult`, `Strategy Blueprint`, `_generate_signals`, `sl_price`) in favor of industry-standard terms (VectorBT, risk parameters, signal execution logic, Stop-Loss).
- **2026-10-22**: Removed clickable link and arrow icon from the `AI Strategy Co-pilot` header title; removed border and background card styling from the `hirus.systems` attribution text.
- **2026-10-22**: Returned all text styles across all 3 case slides (headings, subtitles, row titles, bold text, code tags, badge references, and tabs) to the site's default typography. Scoped custom brand colors exclusively to the respective interactive application containers (`.sc-app`, `.ph`, `.crm`).
- **2026-10-22**: Removed colored box-shadows on `.sl-copilot .lid`, `.sl-content .ph`, and `.sl-crm .lid` (reverted to Apple-style neutral shadows), and enabled `overflow: hidden` on `.sl` to prevent any neighboring slide bleed or colored halos at the bottom.
- **2026-10-22**: Scoped `--accent` per slide container and set `.sl-crm .prog i` to emerald green (`#059669`) for the AI deal scoring recalculation loader in CRM demo.
- **2026-10-22**: Updated Telegram bot command button pulse animation (`@keyframes tgPulse`) and hover shadow from orange (`rgba(255, 90, 31, ...)`) to Telegram blue (`rgba(0, 136, 204, ...)`).
- **2026-10-22**: Assigned distinct brand colors to projects: Red for Strategy Co-pilot, Telegram Blue for Content Creator, and Emerald for CRM. Added ambient glows, tab highlights, and highlighted text per theme.
- **2026-10-22**: Integrated direct live link and personal project attribution to `hirus.systems` in the AI Strategy Co-pilot header and case notes across EN, UA, RU.
- **2026-10-22**: Reordered projects carousel: placed AI Strategy Co-pilot in first position so visitors immediately see the specialized AI agent demo on page load.
- **2026-10-22**: Unified LLM references to Claude API (Anthropic) across project descriptions, subheaders, and i18n dictionaries.
- **2026-10-22**: Expanded clarification loop to 3 sequential steps to reflect genuine slot-filling agent behavior rather than a 1-shot interaction.
- **2026-10-22**: Integrated production `Strategy` & `StrategyResult` contracts to reflect authentic quant engineering capabilities rather than generic mocks.
- **2026-10-22**: Added `# Strategy Blueprint` stage in chat flow to mirror real two-phase agent design (logic confirmation before AST compilation).
- **2026-10-22**: Embedded exact indicator dependencies and vectorized EOD exit masks (`exits = bar_date != bar_date.shift(-1)`) to eliminate look-ahead bias.
- **2026-10-22**: Replaced complex 2-column studio with single-column minimalist chat flow in white and orange tones per `app.hirus.systems`.
- **2026-10-22**: Hardened I18N across EN, UA, RU with dynamic language switching for all interactive states and input placeholders.
