# LQA End Report — Sample (Sanitized)

> **Note:** This is a fictional sample created to demonstrate reporting structure and QA methodology.
> No real client, product, or tester data is included.

**Project:** [PROD] Rewards Feature - LQA Naturalization & Content Accuracy
**Run:** Sample Run #01 - French (FR-FR)
**Testers:** 4
**Date:** Sample Date

---

## TL;DR

Overall localization quality was **strong**, with 3 of 4 testers passing at 90%+ accuracy. The most common issue category was **UI text truncation** in the rewards summary screen, followed by minor **tone/register mismatches** in push notification copy (formal vs. informal "vous/tu" inconsistency). No blocking or critical bugs were found. One tester's run was excluded due to a login/access issue and was not counted toward the scoring average.

---

## Patterns Identified

| Pattern | Frequency | Severity | Notes |
|---|---|---|---|
| Truncated button/label text | 3/4 testers | Medium | Occurs on rewards summary screen at default device width |
| Inconsistent formality (vous/tu) | 2/4 testers | Low | Push notifications mix formal and informal register |
| Currency formatting inconsistency | 1/4 testers | Low | Decimal separator not localized in one screen |
| Untranslated placeholder string | 1/4 testers | Medium | Single string left in source language on error state |

---

## Scoring Summary

| Tester | Screens Reviewed | Issues Found | Pass Rate | Status |
|---|---|---|---|---|
| Tester A | 24 | 2 | 95.8% | ✅ Pass |
| Tester B | 24 | 3 | 91.7% | ✅ Pass |
| Tester C | 24 | 5 | 87.5% | ⚠️ Pass w/ notes |
| Tester D | - | - | - | ❌ Excluded (access issue) |

**Average pass rate (excluding excluded run):** 91.7%

---

## Recommendations

1. Adjust button/label containers to accommodate longer French strings (French text typically runs 15–20% longer than English source).
2. Standardize formality register across all notification copy,  recommend "vous" for consistency with existing in-app tone.
3. Localize the currency/decimal separator on the flagged screen.
4. Fix the untranslated placeholder string on the error state before next release.

---

*This report follows a standard TL;DR → Patterns → Scoring Summary structure used for compiling multi-tester localization QA evaluation runs into a single client-ready deliverable.*
