# Privacy Policy for Gifty

**Last updated: May 18, 2026**

This Privacy Policy describes how Gifty ("we", "our", or "the App") collects, uses, and shares information when you use our mobile application. Gifty is developed and operated by **Abror Gafurov** (the "Developer"), an independent app developer based in Uzbekistan.

By using Gifty, you agree to the practices described in this Policy. If you do not agree, please do not use the App.

---

## 1. Information We Collect

Gifty is designed to be **privacy-first**. You can use the App **without creating an account, providing your name, email, or any other identifying information**. The data we process is limited to the following categories:

### 1.1 Anonymous Identifiers (required for the App to work)

- **Device Identifier** (UUID): a randomly generated value stored in the iOS Keychain on your device. It is used to enforce free-trial limits and prevent abuse. It is not linked to your Apple ID, email, or name.
- **Anonymous Firebase Authentication ID**: a server-side unique identifier created automatically by Firebase. Used to associate your gift history with your device.
- **Adapty Profile ID**: a unique identifier used by our in-app purchase analytics provider (Adapty Inc.) to associate purchases with your anonymous profile.

### 1.2 Gift Personalization Data (provided by you in onboarding)

You voluntarily enter information about the **recipient** of the gift, such as:

- Relationship (e.g., mom, friend, colleague)
- Approximate age and gender (optional)
- Occasion (e.g., birthday, anniversary)
- Interests
- Budget range
- Restrictions or preferences

This data is sent to our backend (Firebase Cloud Functions) and then to OpenAI's API to generate personalized gift suggestions. **We do not store the gift recipient's name or any directly identifying information about the recipient.**

### 1.3 Purchase Information

When you buy a consumable in-app purchase (Gift Packs), Apple processes the transaction. We receive **transaction confirmation only** (transaction ID, product ID, purchase date) via the Adapty SDK and our server-to-server webhook. **We never see your payment method, credit card, or billing details** — those are handled exclusively by Apple.

### 1.4 Diagnostic Data

- Crash reports and error diagnostics may be collected via **Firebase Crashlytics**. They contain technical information such as iOS version, device model, and crash stack traces — no personal content.
- Standard mobile attribution data (IDFV, optional IDFA if you grant App Tracking permission) is sent to Adapty for purchase analytics.

---

## 2. How We Use Your Information

We use the data described above for the following limited purposes:

| Data | Purpose |
|---|---|
| Device ID, Firebase UID | Enforce the 3-free-generation lifetime trial; prevent abuse |
| Gift personalization data | Generate gift suggestions via OpenAI's API |
| Adapty Profile ID + transaction data | Track in-app purchases, credit Gift Packs to your account |
| Diagnostic data | Fix bugs, improve app stability |

We **do not**:

- Sell your data to third parties
- Use your data for advertising or profiling
- Share your gift history with anyone
- Store passwords or biometric data
- Access your contacts, photos, or location

---

## 3. Third-Party Services

Gifty relies on the following third-party services. Each has its own privacy policy:

| Service | Purpose | Privacy Policy |
|---|---|---|
| Apple Inc. (App Store, StoreKit) | App distribution, in-app purchases | https://www.apple.com/legal/privacy/ |
| Google Firebase (Auth, Firestore, Cloud Functions, App Check, Crashlytics) | Anonymous backend authentication, data storage, server-side AI proxy | https://firebase.google.com/support/privacy |
| OpenAI L.L.C. | AI-powered gift generation and product image creation | https://openai.com/policies/privacy-policy |
| Adapty Inc. | In-app purchase analytics, paywall configuration | https://adapty.io/privacy/ |

Gift personalization data is processed by OpenAI under their data-handling policies. Per OpenAI's API terms, your prompt data **is not used to train their models**.

---

## 4. Data Retention

- **Device-based free-trial counter**: kept indefinitely on our backend, tied to your device identifier. This prevents repeated free-trial abuse via reinstallation.
- **Gift history**: stored under your anonymous Firebase user ID until you delete it.
- **Purchase history**: stored to track your Gift Pack balance.

You can delete all your account data at any time via the **Delete Account** option in the Profile settings of the App. This permanently removes your gift history, Pack balance, and Firebase authentication record.

---

## 5. Your Rights (GDPR / CCPA / DSA)

If you reside in the European Union, United Kingdom, California, or another jurisdiction granting data protection rights, you have the right to:

- **Access** the data we hold about you
- **Delete** your data (use **Delete Account** in the App, or contact us)
- **Object** to processing
- **Data portability**

Because Gifty collects only anonymous, non-identifying data tied to your device, most of these rights are exercised by simply uninstalling the App and using Delete Account.

To exercise these rights or for any privacy concerns, contact us at the email below.

---

## 6. Children's Privacy

Gifty is rated **4+** but is not directed at children under 13. We do not knowingly collect personal information from children. If you believe a child has provided us with such data, please contact us and we will promptly delete it.

---

## 7. International Data Transfers

Our backend services (Firebase Cloud Functions, Firestore) are hosted in the **United States** (Google Cloud `us-central1` region). OpenAI processes data in the **United States**. By using the App, you consent to these international transfers.

---

## 8. Security

We use industry-standard security practices:

- All network traffic is encrypted via HTTPS / TLS 1.3
- Server endpoints are protected by Firebase App Check (Apple App Attest)
- Backend secrets (OpenAI key, Adapty webhook secret) are stored in Google Secret Manager
- Apple StoreKit handles all payment data; we never have access to it

---

## 9. Changes to This Policy

We may update this Privacy Policy from time to time. Material changes will be communicated via an in-app notice or App Store release notes. The "Last updated" date at the top of this page reflects the most recent revision.

---

## 10. Contact

If you have questions or concerns about this Privacy Policy, please contact:

**Abror Gafurov**
Email: abrorgafurov@icloud.com
Address: Ogohiy 48, Fergana 150100, Uzbekistan

---
