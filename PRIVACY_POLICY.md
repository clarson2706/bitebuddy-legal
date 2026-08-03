# BiteBuddy Privacy Policy

Version: privacy_v4 · Effective: August 3, 2026

BiteBuddy helps you understand your nutrition by estimating what's in the food you log. Food and nutrition data can be sensitive, so this policy explains exactly what we collect, why, and what we never do with it.

## 1. Data we collect

**Account data.** Email address, a hashed password (managed by our authentication provider), and an internal account ID.

**Profile and goal data.** Optional display name, age, sex selection used for estimates, height, weight, goal weight and date, activity level, primary goal, and the daily calorie/macro targets calculated from them. This information is health-adjacent and is used only to personalize your plan and estimates.

**Food photos and scan inputs.** Photos you take or import, barcode numbers, nutrition-label photos, text descriptions, and voice-derived transcripts. Photos are compressed on your device, sent securely for analysis, and are **not stored on our servers** — they are processed to produce an estimate and are not retained as images after the request completes. Voice audio is transcribed on-device by Apple's speech recognition; we receive only the text.

**Food logs, verified nutrition, and estimates.** The foods you save: names, portions, nutrition values, source labels (for example AI estimate, barcode lookup, nutrition label, USDA data, manual entry, or verified restaurant menu), confidence and review flags, your corrections and edits, meal types, and timestamps.

**Weight entries.** If you use the Progress tab, the weight and date you log to track your trend over time. This is health-adjacent information used only to show your own chart and progress toward your goal weight.

**Meal Advisor context.** If you use the "What should I eat?" advisor, whatever you tell it — a restaurant name, foods you say you have on hand, or a menu/photo description — plus your remaining calorie/macro targets and stated goal for that request. This is sent to produce a suggestion and is not saved as a running log; it is only retained as part of standard request logging (see Device and diagnostic data).

**Restaurant menu reference data.** BiteBuddy stores public restaurant menu and nutrition reference data, such as item names, calories, macros, source URLs, source dates, and whether an item is active. This reference data is not personal data unless you choose to log a recommendation to your own account.

**Usage and progress data.** Scan counts (used to enforce Free/Pro limits), XP/streak/level progress, and cached weekly/monthly report summaries.

**Subscription data.** Subscription status and entitlement (via RevenueCat and Apple). We never see your full payment details; Apple processes payments.

**Device and diagnostic data.** Basic request logs (timestamps, request IDs, error codes) needed to operate and secure the service. Our logs are written to exclude photos, tokens, emails, and food contents.

**Advertising and attribution data — only if you allow tracking.** If BiteBuddy asks for permission to track and you allow it, we share your device's advertising identifier (IDFA) and a small set of app events with TikTok so we can tell which advertisements brought people to BiteBuddy. The events are: installing the app, opening it, creating an account, starting a subscription trial, and completing a purchase. They record that the action happened — they never include your food logs, photos, weight, goals, or health-adjacent data. **If you decline, no advertising identifier and no attribution events are shared, and BiteBuddy works exactly the same.** You can change your answer at any time in iOS Settings → Privacy & Security → Tracking.

We do **not** collect your precise location or contacts.

## 2. How we use data

- To provide the service: analyze scans, calculate estimates, store your logs, show progress and reports.
- To personalize: your profile targets shape estimates, insights, and reports.
- To enforce plan limits and prevent abuse (scan quotas, rate limits).
- To provide support and maintain security.
- To measure advertising, if you allow tracking: to learn which advertisements led to installs, account creation, and subscriptions, so we do not waste money on advertising that does not work.

We do **not** sell your personal data for money, and we do not use your photos, food logs, weight, goals, or any other health-adjacent data for advertising — none of it is shared with TikTok or any other advertising company.

Sharing an advertising identifier with TikTok for attribution and retargeting counts as "sharing" personal information for cross-context behavioural advertising under California law, and as targeted advertising under some other state laws. **Declining the tracking prompt, or turning tracking off in iOS Settings, opts you out of it entirely.**

## 3. AI processing

Food photos, label photos, descriptions, corrections, and relevant profile targets are sent to our server, which forwards them to Google's Gemini API to produce nutrition estimates, and may query the USDA FoodData Central and Open Food Facts databases. AI estimates can be inaccurate; the app asks you to review them. **We do not use your data to train AI models, and we have not authorized our AI vendors to train on it.** This relies on our Gemini API usage being on Google's paid tier, which excludes prompts and images from model training and human review; confirm billing is active on the underlying Google Cloud project before each release.

**Meal Advisor** uses trust levels. For supported restaurants, BiteBuddy first checks its verified restaurant menu database and may rank exact menu items using deterministic scoring and, when configured, Gemini for wording/ranking only. Exact item names and nutrition values for verified recommendations come from the stored menu reference rows, not from model text. For foods you say you have on hand, menu photos, or restaurants without verified menu coverage, Meal Advisor may use Gemini to generate an estimate. Future online lookup features may use restaurant names or menu item text as search queries to find public nutrition sources. In every non-verified case, the app labels the result as an estimate or sourced lookup and asks you to review it before saving. The same no-training terms described above apply to AI processing.

## 4. Service providers

- **Supabase** — authentication, database, and serverless functions (hosting of your account, logs, and settings).
- **Google Gemini API** — AI nutrition estimation and Meal Advisor suggestions, including ranking/explanation help for verified menu options and estimate-only suggestions when verified data is unavailable.
- **USDA FoodData Central / Open Food Facts** — public nutrition databases (they receive food queries/barcodes, never your identity).
- **RevenueCat and Apple** — subscription management and payment.
- **TikTok** — advertising measurement, and only if you allow tracking. TikTok receives your advertising identifier and the attribution events listed in Section 1. It does not receive your email, food logs, photos, weight, or goals. TikTok acts as an independent controller of this data under its own [privacy policy](https://www.tiktok.com/legal/privacy-policy).

Each provider receives only what it needs to perform its function.

## 5. Storage and security

Data is stored with Supabase in the United States (AWS us-east-2 via Supabase). Data in transit is encrypted with TLS. Access to user rows is enforced by database row-level security so accounts can only read and write their own data. Auth sessions on your device are stored in the iOS Keychain. No system is perfectly secure, and we cannot guarantee absolute security.

## 6. Retention

Your data is retained while your account is active. Scan photos are not retained after analysis. Deleted food logs are removed immediately. When you delete your account, we delete your food logs, weight entries, saved foods, goals, reports, usage counters, XP history, entitlement records, and profile identifiers, and we ask RevenueCat to delete your subscriber record. A minimal, de-identified deletion audit record (with no user ID) may be kept to prove the deletion happened. Signing up again with the same email starts a fresh account and does not restore old data.

## 7. Deleting your account

Profile → Delete Account permanently deletes your account inside the app — no email or support ticket required. You may also request deletion at clarson2706@gmail.com.

## 8. Your rights

Depending on where you live (for example under GDPR or the California privacy laws), you may have rights to access, correct, export, or delete your personal data, and to object to certain processing. The app itself provides viewing, editing, and deletion. For anything else, contact clarson2706@gmail.com. We do not discriminate against you for exercising your rights.

**Opting out of advertising measurement.** Decline the tracking prompt, or turn BiteBuddy off under iOS Settings → Privacy & Security → Tracking. That is the complete opt-out: no advertising identifier and no attribution events leave your device. It has no effect on anything else in the app.

## 9. Children

BiteBuddy requires users to be at least 16 years old. We do not knowingly collect data from anyone under 16. If you believe a child under 16 has an account, contact clarson2706@gmail.com and we will delete it.

## 10. App Store privacy labels

Our App Store privacy disclosures list: Health & Fitness data, Photos (processed, not retained), Name, Email, User ID, Purchases, and Other User Content — all linked to your account and none used for tracking — plus, under "Data Used to Track You", your Device ID (advertising identifier) and Product Interaction, which are shared with TikTok for advertising measurement only when you allow tracking.

## 11. Changes

If we materially change this policy, we will present the new version in the app and require re-acceptance before continued use.

## 12. Contact

Connor Larson (sole proprietor), doing business as BiteBuddy · clarson2706@gmail.com. We do not maintain a public mailing address; contact us by email for any privacy request.
