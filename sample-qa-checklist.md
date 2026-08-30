# Pre-Release QA Checklist (Sample)

This is a fictional example of a quick reference smoke test checklist, the kind you'd run through right before a release build goes out.

**Project:** Mobile Banking App
**Release:** v2.4.0
**Checked By:** Sample QA Tester
**Date:** Sample Date

---

## Core Functionality
- [ ] App launches without crashing on a cold start
- [ ] Login with valid credentials succeeds
- [ ] Login with invalid credentials shows the correct error
- [ ] Biometric login (Face ID / Fingerprint) works where enabled
- [ ] Session timeout logs the user out correctly

## Fund Transfer (this release's main focus)
- [ ] Internal transfer completes successfully
- [ ] External transfer completes successfully
- [ ] Insufficient balance shows the correct error and doesn't process the transfer
- [ ] Transfer confirmation screen shows the correct amount and recipient
- [ ] A receipt or confirmation is generated and shows up in history

## Cross Platform Consistency
- [ ] iOS matches the expected design
- [ ] Android matches the expected design
- [ ] Web matches the expected design
- [ ] No text gets cut off on smaller screen sizes

## Regression (making sure nothing else broke)
- [ ] Account balance shows correctly after a transfer
- [ ] Transaction history updates in real time
- [ ] Notifications still trigger correctly for other account actions
- [ ] No new crashes in unrelated parts of the app (spot checked)

## Localization Spot Check
- [ ] No untranslated or placeholder text visible
- [ ] Currency formatting is correct for the locale
- [ ] No text truncation in the non-English locales tested

## Sign Off
- [ ] All Critical and High severity bugs from this cycle are fixed or waived by dev/PM
- [ ] Build is approved for release

---

A checklist like this is meant to be a fast, final pass right before release. It's not a replacement for full test case execution, more of a safety net to catch anything broken at the last minute.
