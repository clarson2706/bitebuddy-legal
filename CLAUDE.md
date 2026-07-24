# CLAUDE.md — BiteBuddy published legal mirror

Loaded automatically at session start in this repo. Last verified: 2026-07-24.

## Do not edit this repository

Every `.md` file here is **generated**. The canonical copies live in `clarson2706/BiteBuddyMVP`
under `/Legal`, and `.github/workflows/publish-legal.yml` in that repo copies them here on every
merge to `main` that touches them.

Edit a document here and your change will be silently overwritten by the next publish.

**To change legal text:** edit `BiteBuddyMVP/Legal/<doc>.md`, bump the matching version constant in
`BiteBuddyMVP/BiteBuddyMVP/Features/Legal/LegalSheet.swift`, open a PR there, and merge it.
Publishing happens on its own.

## Why this repo matters more than its size suggests

This is the **public legal surface of a shipping App Store app**. Every in-app "Privacy Policy" and
"Terms of Service" link points at `blob/main/` here. What is on `main` is what users read and what
Apple sees.

## The version invariant

The version identifier at the top of each document must match what the app records consent
against in `LegalSheet.swift`. On 2026-07-24 they did not: the app was filing consent against
`privacy_v3` and `terms_v2` while this repo still served `privacy_v2` and `terms_v1`, because the
two copies were maintained by hand. Users were consenting to a version they could not read.

That is the entire reason publishing is automated now.

## Never publish these

`LEGAL_RISK_AUDIT.md` and `APP_STORE_PRIVACY_NOTES.md` exist in `BiteBuddyMVP/Legal/` and are
**internal** — the first is a draft for attorney review. They must never appear here. The publish
workflow fails the build if they do.

## Approval gate

Merging anything to `main` in this repo publishes user-facing legal copy. **That is always
Connor's call**, without exception.

## The five published documents

`TERMS_OF_SERVICE` · `PRIVACY_POLICY` · `AI_NUTRITION_ESTIMATE_CONSENT` ·
`MEDICAL_AND_NUTRITION_DISCLAIMER` · `SUBSCRIPTION_TERMS`

Support contact and account-deletion instructions live in `README.md`, which is also the landing
page people reach from the App Store listing.
