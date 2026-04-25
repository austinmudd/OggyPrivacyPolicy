# Privacy Policy for Oggy

**Effective date:** [TODO: insert date you publish this — e.g., May 1, 2026]

## Plain-English summary

Oggy is built to respect your privacy. The app stores everything you create — buttons, photos, settings, your PIN — locally on your device. It does not have a server, does not collect analytics, does not show ads, and does not share your data with anyone. The only third party involved is the in-app purchase system (Google Play Billing via RevenueCat) used if you choose to buy the optional unlock.

If you have any questions about this policy, email **OggyAppTeam@gmail.com**.

---

## What information Oggy stores on your device

Oggy stores the following on your device only — never on a server, and never transmitted to us:

- The buttons you create, including the text spoken, the label, the chosen color, and the chosen emoji or photo
- Your app settings: voice selection, speech rate, speech pitch, grid layout preferences, theme
- Your parental-control PIN, stored as a one-way hash (the PIN itself is never saved in plain text)
- Whether biometric unlock (Face ID / fingerprint) is enabled

This data is stored using on-device storage (MMKV). It is included in your normal device backup if you have one configured (e.g., Google Drive backup), but Oggy does not initiate or receive that backup.

## What Oggy does *not* collect

- We do not collect personal information about you, your children, or anyone else.
- We do not collect device identifiers, advertising IDs, or fingerprints.
- We do not collect crash reports or analytics.
- We do not collect location data.
- We do not show ads.
- We do not sell or share data with third parties for advertising.
- We do not require an account.

## Permissions Oggy uses, and why

When you grant these permissions, the data captured stays on your device. Oggy does not transmit any of it.

- **Photo library access** — only used when you tap "Photo" on the symbol picker. The photo you select is copied into Oggy's private app storage to use as a button image.
- **Camera access** — only used when you tap "Camera" on the symbol picker. The photo you take is saved to Oggy's private app storage.
- **Biometric authentication** — used to unlock the parental-controls section. Oggy never sees the biometric data itself; the operating system handles authentication and reports back only success or failure.

You can revoke any of these permissions at any time in your device's Settings, and Oggy will continue to function (the relevant feature simply won't be available until you re-grant the permission).

## Microphone and speech recognition

Oggy does not use the microphone or perform speech recognition. The text-to-speech feature speaks text *out* using the voices already installed on your device — it does not listen.

## In-app purchases

Oggy offers a one-time in-app purchase ("Unlock full access") that removes the 12-button limit and grants access to future paid features. This purchase is processed by:

- **Google Play Billing** — operated by Google. See Google's privacy policy at https://policies.google.com/privacy
- **RevenueCat** — used to verify and restore purchases across devices. RevenueCat receives a non-personal user identifier and the purchase event. See RevenueCat's privacy policy at https://www.revenuecat.com/privacy

We do not see your payment method, billing address, or any personally identifying purchase information.

## Children's privacy

Oggy is designed for use by and with children, including children under 13. Because Oggy does not collect personal information from anyone — children or adults — it complies with COPPA and similar children's privacy regulations by design. We do not knowingly collect any personal data from children, and there is no account, profile, or login in the app where such data could be entered.

## Data retention

All app data is retained locally on your device until you uninstall the app. Uninstalling Oggy permanently removes all locally-stored data unless you have a system backup that includes app data.

## Your rights

Because we don't store your data on any server, there's nothing for us to access, correct, or delete on your behalf. To remove all data Oggy stores, uninstall the app from your device.

For purchase-related data held by Google or RevenueCat, please contact those providers directly per their privacy policies linked above.

## Changes to this policy

If we ever change this policy in a way that materially affects what data Oggy stores or transmits, we will update the "Effective date" at the top and notify users via the app's release notes on the next update. The current policy is always available in the app under Settings → About → Privacy policy.

## Contact

Questions, concerns, or requests:

**Email:** OggyAppTeam@gmail.com

---

## Notes for whoever's hosting this

- Update the "Effective date" at the top before publishing.
- The URL of the hosted version goes in:
  - `.env` → `EXPO_PUBLIC_PRIVACY_POLICY_URL`
  - Play Console → App content → Privacy policy
- Free hosting options:
  - **GitHub Pages** — push this Markdown file to a public repo with a `_config.yml`, get `https://username.github.io/oggy-legal/privacy-policy.html` for free, edit anytime
  - **Vercel** — drop into a Next.js project, deploy in 60 seconds with a custom subdomain
  - **Notion** — paste contents into a public Notion page, set to "Share to web"
  - **Google Sites** — free, no code, looks fine
- Whichever you pick: keep the URL stable. Changing it later requires updating Play Console + the app, which is mildly annoying.
