# Bug Report — Sample

> Fictional example demonstrating bug report structure and detail level.

**Bug ID:** BUG-0142
**Reported By:** Sample Tester
**Date:** Sample Date
**Product/Feature:** Checkout Flow — Promo Code Field
**Environment:** iOS 17.4, iPhone 13, App v3.2.1 (also reproduced on Android 14, Pixel 7)
**Severity:** Medium
**Priority:** High
**Status:** Open

---

## Summary
Promo code field accepts input but does not apply discount when a valid code is entered and "Apply" is tapped a second time after an initial invalid attempt.

## Steps to Reproduce
1. Go to Checkout screen with at least one item in cart
2. Enter an **invalid** promo code (e.g. `TESTCODE123`) and tap **Apply**
3. Observe "Invalid code" error message
4. Clear the field and enter a **valid** promo code (e.g. `SAVE10`)
5. Tap **Apply** again

## Expected Result
Valid discount (10%) is applied to the order total, and a success confirmation is shown.

## Actual Result
Nothing happens — no error, no success message, and the order total remains unchanged. The "Apply" button appears to do nothing on the second tap.

## Additional Notes
- Issue only occurs after a **prior invalid attempt** in the same session. Entering a valid code on the *first* attempt works correctly.
- Reproduced consistently across 5/5 attempts.
- Screenshot/screen recording: [attach here]

## Severity & Priority Justification
**Medium severity** — does not crash the app or block checkout entirely (user can still complete purchase without discount), but directly affects revenue/promo functionality and creates a broken user experience.
**High priority** — affects a core commerce flow and is easily reproducible; likely to affect a large share of users who mistype a code once.

---

*Template structure: Summary → Repro Steps → Expected vs Actual → Notes → Severity/Priority justification. This format keeps reports scannable for developers while giving enough detail to reproduce without back-and-forth.*
