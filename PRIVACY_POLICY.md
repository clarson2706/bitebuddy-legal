# BiteBuddy Privacy Policy

Version: privacy_v1 · Effective: July 5, 2026

BiteBuddy helps you understand your nutrition by estimating what's in the food you log. Food and nutrition data can be sensitive, so this policy explains exactly what we collect, why, and what we never do with it.

## 1. Data we collect

**Account data.** Email address, a hashed password (managed by our authentication provider), and an internal account ID.

**Profile and goal data.** Optional display name, age, sex selection used for estimates, height, weight, goal weight and date, activity level, primary goal, and the daily calorie/macro targets calculated from them. This information is health-adjacent and is used only to personalize your plan and estimates.

**Food photos and scan inputs.** Photos you take or import, barcode numbers, nutrition-label photos, text descriptions, and voice-derived transcripts. Photos are compressed on your device, sent securely for analysis, and are **not stored on our servers** — they are processed to produce an estimate and are not retained as images after the request completes. Voice audio is transcribed on-device by Apple's speech recognition; we receive only the text.

**Food logs and estimates.** The foods you save: names, portions, nutrition values, AI confidence and review flags, your corrections and edits, meal types, and timestamps.

**Usage and progress data.** Scan counts (used to enforce Free/Pro limits), XP/streak/level progress, and cached weekly/monthly report summaries.

**Subscription data.** Subscription status and entitlement (via RevenueCat and Apple). We never see your full payment details; Apple processes payments.

**Device and diagnostic data.** Basic request logs (timestamps, request IDs, error codes) needed to operate and secure the service. Our logs are written to exclude photos, tokens, emails, and food contents.

We do **not** collect your precise location, contacts, or advertising identifiers, and we do not track you across other companies' apps or websites.

## 2. How we use data

- To provide the service: analyze scans, calculate estimates, store your logs, show progress and reports.
- To personalize: your profile targets shape estimates, insights, and reports.
- To enforce plan limits and prevent abuse (scan quotas, rate limits).
- To provide support and maintain security.

We do **not** sell your personal data, and we do not use your photos, food logs, or health-adjacent data for advertising.

## 3. AI processing

Food photos, label photos, descriptions, corrections, and relevant profile targets are sent to our server, which forwards them to Google's Gemini API to produce nutrition estimates, and may query the USDA FoodData Central and Open Food Facts databases. AI estimates can be inaccurate; the app asks you to review them. **We do not use your data to train AI models, and we have not authorized our AI vendors to train on it.** This relies on our Gemini API usage being on Google's paid tier, which excludes prompts and images from model training and human review; confirm billing is active on the underlying Google Cloud project before each release.

## 4. Service providers

- **Supabase** — authentication, database, and serverless functions (hosting of your account, logs, and settings).
- **Google Gemini API** — AI nutrition estimation.
- **USDA FoodData Central / Open Food Facts** — public nutrition databases (they receive food queries/barcodes, never your identity).
- **RevenueCat and Apple** — subscription management and payment.

Each provider receives only what it needs to perform its function.

## 5. Storage and security

Data is stored with Supabase in the United States (AWS us-east-2 via Supabase). Data in transit is encrypted with TLS. Access to user rows is enforced by database row-level security so accounts can only read and write their own data. Auth sessions on your device are stored in the iOS Keychain. No system is perfectly secure, and we cannot guarantee absolute security.

## 6. Retention

Your data is retained while your account is active. Scan photos are not retained after analysis. Deleted food logs are removed immediately. When you delete your account, we delete your food logs, saved foods, goals, reports, usage counters, XP history, entitlement records, and profile identifiers, and we ask RevenueCat to delete your subscriber record. A minimal, de-identified deletion audit record (with no user ID) may be kept to prove the deletion happened. Signing up again with the same email starts a fresh account and does not restore old data.

## 7. Deleting your account

Profile → Delete Account permanently deletes your account inside the app — no email or support ticket required. You may also request deletion at clarson2706@gmail.com.

## 8. Your rights

Depending on where you live (for example under GDPR or the California privacy laws), you may have rights to access, correct, export, or delete your personal data, and to object to certain processing. The app itself provides viewing, editing, and deletion. For anything else, contact clarson2706@gmail.com. We do not discriminate against you for exercising your rights.

## 9. Children

BiteBuddy requires users to be at least 16 years old. We do not knowingly collect data from anyone under 16. If you believe a child under 16 has an account, contact clarson2706@gmail.com and we will delete it.

## 10. App Store privacy labels

Our App Store privacy disclosures list: Health & Fitness data, Photos (processed, not retained), Name, Email, User ID, and Other User Content — all linked to your account, none used for tracking.

## 11. Changes

If we materially change this policy, we will present the new version in the app and require re-acceptance before continued use.

## 12. Contact

Connor Larson (sole proprietor), doing business as BiteBuddy · clarson2706@gmail.com. We do not maintain a public mailing address; contact us by email for any privacy request.
