# Privacy Policy for DishSense.AI

**Last Updated:** April 26, 2026

Welcome to DishSense.AI! This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you use our mobile application (the "App") and related services (collectively, the "Service"). Please read this Privacy Policy carefully. If you do not agree with the terms of this Privacy Policy, please do not access or use the App.

---

## 1. Information We Collect

We may collect information about you in a variety of ways. The information we may collect via the App includes:

### A. Personal Data
* **Account Information:** When you register, we collect authentication information through third-party providers (such as Google Sign-In), which may provide us with your name, email address, and profile picture. We do not receive or store your Google account password.
* **User-Generated Content:** To provide our core services, we collect the photos and images of food that you upload or capture using your device's camera. These images are processed by AI services and stored in Google Cloud Storage.
* **Camera and Photo Library Access:** With your permission, the App accesses your device's camera (to capture food photos) and photo library (to import existing photos). You can revoke these permissions at any time through your device's system settings; doing so will disable the corresponding features.
* **Profile and Goal Data:** We store your daily macronutrient goals (calories, protein, carbohydrates, fat), your custom macro presets, and — for premium subscribers who enable Macro Cycling — a per-day weekly goal schedule.
* **Referral Data:** When you sign up via a referral link from another user (or via the Google Play Install Referrer mechanism), we record the referring account so we can credit referral rewards to both accounts. Referral codes are not personally identifiable on their own.

### B. Financial and Subscription Data
* **In-App Purchases (Bites & Bursts):** If you purchase "Bites" or "Bursts" credit bundles within the App, your payment is processed directly by the Google Play Store. We do not collect, store, or have access to your full payment card number or direct billing information. We receive transaction receipt data (purchase token, order ID, product ID, purchase state, timestamp) solely to grant you the purchased credits and verify transactional integrity.
* **DishSense.AI Pro Subscription:** Premium subscriptions are sold through Google Play Billing and managed via our subscription provider, **RevenueCat**. We store your subscription status (`isPremium`), the date you first subscribed (`premiumSince`), and your current entitlement expiry date (`premiumExpiresAt`). RevenueCat receives a stable, app-specific user identifier mapped from your Google authentication ID, along with subscription lifecycle events (purchase, renewal, cancellation, expiration, billing issues). RevenueCat does not receive your name, email, or photo content.

### C. Automatically Collected Data
* **Device and Usage Information:** We may automatically collect certain information when you use the App, such as your device type, operating system version, unique device identifiers, IP address, and data regarding your interaction with the App (e.g., features used, screens viewed, session duration). This data is used for diagnostics, fraud prevention, and service improvement.
* **Activity Timestamps:** We record an approximate `lastActiveAt` timestamp (updated at most once per hour) so we can provide accurate session continuity, support requests, and detect abandoned accounts.
* **Application Event Logs:** Operational events such as analysis errors, purchase failures, authentication failures, and webhook reconciliation outcomes are recorded against your account ID. These records are automatically deleted **30 days** after creation and are used solely for diagnostics, fraud prevention, and customer support.
* **Crash Reports and Diagnostics:** The App may automatically collect technical error and crash data to help us identify and fix bugs.

### D. Push Notifications
* **Notification Tokens:** With your permission, we register a push notification token (issued by Google Firebase / FCM via Expo) so we can notify you when an asynchronous task you initiated — such as a meal analysis — has completed. We currently send transactional notifications only; we do not send marketing notifications. We store up to 20 tokens per account (one per device); older tokens are pruned automatically. You may opt out of receiving push notifications at any time through your device settings.

### E. AI-Generated Meal Data
For each meal you log, we store the original photo and the AI-generated outputs derived from it: ingredient list, ingredient amounts, calorie and macronutrient estimates, satiety score (1–10), dietary tags (e.g., "Vegan", "Keto"), nutritional flags (e.g., "High Sodium"), processing-level classification (Unprocessed / Minimally Processed / Processed / Ultra-Processed), the URL of the generated "exploded view" image, and a deterministic ingredient-fingerprint hash used to cache results and reduce redundant processing. **All AI-generated values are estimates only — see Section 10.**

---

## 2. How We Use Your Information

We use the information we collect to operate, maintain, and improve the Service. Specifically, we may use information collected about you to:

* **Provide Core AI Services:** Transmit your uploaded food images to third-party AI services (Google Cloud Vertex AI, Gemini family models) to analyze food content, generate approximate macronutrient and nutritional estimates, satiety scores, dietary tags, nutritional flags, processing-level classifications, and "exploded view" culinary composites. **All AI-generated outputs are approximations only.** See Section 10 for full details.
* **Manage Your Account and Subscription:** Create and manage your account, process login and authentication, maintain your usage profile, and grant or revoke premium feature access based on your subscription state as reported by RevenueCat.
* **Process Transactions:** Verify in-app purchases through the Google Play Store, manage your Bites and Bursts balances, enforce our "No Success, No Charge" policy, and credit referral rewards.
* **Generate and Deliver Weekly Reports (Premium):** For active premium subscribers, we automatically compile a weekly PDF nutrition summary from the meals you logged during the past 7 days. The report includes your macro adherence profile, food-quality breakdown, satiety metrics, and embedded copies of the "exploded view" images for the meals included. The PDF is delivered to the email address associated with your Google Sign-In account. The report is informational only and is not a medical document — see Section 10.
* **Deliver Notifications:** Send push notifications regarding analysis completion and other transactional service updates.
* **Service Operations and Analytics:** Authorized personnel may access individual and aggregated account data — including display name, email, currency balances, subscription status, purchase history, referral relationships, last-active timestamps, and deletion reasons — for support, fraud prevention, billing reconciliation, and product analytics.
* **Improve Our Services:** Analyze aggregated usage trends and technical performance data to improve the App's functionality, reliability, and user experience.
* **Comply with Legal Obligations:** Respond to lawful requests from public authorities and comply with applicable laws and regulations.
* **Prevent Fraud and Abuse:** Detect, investigate, and prevent fraudulent transactions, referral abuse, and other harmful or illegal activity.

### Lawful Bases (GDPR / UK GDPR)
Where the GDPR or UK GDPR applies, our lawful bases for processing are:
* **Performance of a contract** — for providing the core App, processing purchases, managing subscriptions, generating analyses you request, and delivering weekly reports to subscribers.
* **Legitimate interests** — for fraud prevention, security, diagnostics, service improvement, and aggregated analytics, balanced against your privacy rights.
* **Consent** — for camera/photo library access, push notifications, and any optional features that require it. You may withdraw consent at any time through your device settings or App settings.
* **Legal obligation** — where we must retain transactional records for tax or financial compliance.

---

## 3. Disclosure of Your Information

We do not sell your personal information. We may share information we have collected with the following categories of third-party service providers, each of whom is contractually obligated to use your data only to provide services to us and in accordance with this Privacy Policy:

* **Google Cloud Vertex AI** (Gemini family models) — AI image analysis, nutritional estimation, and image generation
* **Google Cloud Storage** — Secure storage of uploaded and AI-generated images
* **Google Cloud Run** — Backend API hosting
* **Google Cloud Functions and Cloud Scheduler** — Scheduled jobs, including weekly PDF report generation
* **Google Cloud Secret Manager** — Credentials and API key storage
* **MongoDB Atlas** — Primary database
* **Upstash** — In-memory caching and queue management for asynchronous processing
* **Google Firebase / FCM** — Push notification delivery
* **Google Play Billing** — In-app purchase and subscription processing
* **RevenueCat** — Subscription state management, entitlement reconciliation, and webhook delivery
* **Google Workspace / Gmail SMTP** — Transactional email delivery (e.g., weekly report PDFs) over TLS-encrypted connections
* **Google Sign-In** — Authentication

**Other disclosure circumstances:**

* **Business Transfers:** If DishSense.AI is involved in a merger, acquisition, asset sale, or similar transaction, your information may be transferred as a business asset. We will provide notice before your personal information is transferred and becomes subject to a different privacy policy.
* **By Law or to Protect Rights:** We may disclose your information if required to do so by law, court order, or governmental authority, or if we believe disclosure is necessary to: (a) comply with a legal obligation; (b) protect and defend our rights or property; (c) prevent or investigate possible wrongdoing in connection with the Service; (d) protect the personal safety of users of the Service or the public; or (e) protect against legal liability.
* **With Your Consent:** We may share your information for any other purpose with your prior explicit consent.

---

## 4. Data Security

We implement administrative, technical, and physical security measures designed to protect your personal information from unauthorized access, use, alteration, and disclosure:

* All data in transit is encrypted using TLS/HTTPS.
* Authentication is secured via signed JSON Web Tokens (JWT) with server-side validation.
* API secrets, credentials, and keys are managed dynamically using Google Cloud Secret Manager — no secrets are hardcoded in the application.
* Webhooks from third-party providers (e.g., RevenueCat) are authenticated using shared secrets and constant-time comparison to prevent timing attacks.
* Access to production systems is restricted to authorized personnel only.
* Weekly report PDFs are generated server-side in an isolated environment. Embedded meal images are re-decoded and re-encoded through a vetted image-processing library before being inserted into the PDF, so that EXIF metadata and any non-image bytes (including potential polyglot payloads) are stripped. PDFs are transmitted to your email address over TLS-encrypted SMTP.

**However, please be aware that no security system is impenetrable.** While we have taken reasonable steps to protect your information, we cannot guarantee the absolute security of any data you transmit to us or that is stored on our systems. **Once a weekly report email or any other communication leaves our infrastructure, the security of your email account, device, and any antivirus or scanning tools is your responsibility.** You provide personal information at your own risk.

---

## 5. Data Retention and Deletion

We retain your personal information and uploaded images only for as long as necessary to fulfill the purposes outlined in this Privacy Policy, or as required or permitted by applicable law.

**Retention classes:**

* **Account, profile, meal, and image data** — retained for the life of your account; deleted on account deletion as described below.
* **Application Event Logs** (errors, purchase failures, authentication failures) — automatically deleted **30 days** after creation.
* **Account Deletion Reasons** — collected anonymously when you delete your account (without a link back to the deleted user) and automatically removed **90 days** after collection. We use these solely to improve the product.
* **Purchase and subscription records** — may be retained for a longer period (typically up to 7 years) where required by tax, accounting, or financial-compliance laws.

**Account Deletion:** You may request the deletion of your account and associated data at any time from within the App settings. Upon receiving a deletion request:

* Your account is deactivated immediately and you are signed out.
* All associated account data, authentication records, meal records, and uploaded images are scheduled for **permanent, irreversible deletion 14 days** after the request.
* During this 14-day grace period, you may log back in to cancel the deletion and fully restore your account.
* After the 14-day period has elapsed, all data is permanently removed and **cannot be recovered**, except for purchase records retained for legal/financial compliance and anonymous deletion-reason entries.

---

## 6. Your Privacy Rights

Depending on your location, you may have certain rights regarding your personal information:

### California Residents (CCPA/CPRA)
If you are a California resident, you have the right to:
* **Know** what personal information we collect, use, disclose, or sell about you.
* **Delete** personal information we have collected from you (subject to certain exceptions).
* **Correct** inaccurate personal information we hold about you.
* **Opt-Out of Sale or Sharing.** **We do not sell or share personal information** as those terms are defined under the CCPA/CPRA.
* **Limit Use of Sensitive Personal Information.** We do not use sensitive personal information for purposes beyond those permitted by the CCPA without your consent.
* **Non-Discrimination:** We will not discriminate against you for exercising any of your CCPA rights.

### EEA, UK, and Switzerland Residents (GDPR)
If you are located in the European Economic Area, the United Kingdom, or Switzerland, you have the right to:
* **Access** a copy of the personal data we hold about you.
* **Rectification** of inaccurate or incomplete personal data.
* **Erasure** ("right to be forgotten") of your personal data in certain circumstances.
* **Restriction** of the processing of your personal data.
* **Data Portability** — receive your data in a structured, machine-readable format.
* **Object** to processing based on legitimate interests.
* **Withdraw Consent** at any time where processing is based on your consent, without affecting the lawfulness of prior processing.
* **Lodge a Complaint** with a supervisory authority in your country of residence.

To exercise any of these rights, please contact us using the information in Section 12. We will respond to verified requests within the timeframes required by applicable law.

---

## 7. International Data Transfers

DishSense.AI is developed and operated by a company based in **Israel**. Your information is stored and processed on infrastructure provided by Google Cloud Platform, located primarily in the United States. If you are accessing the App from outside these countries, please be aware that your information may be transferred to, stored, and processed in Israel, the United States, or other countries where our service providers operate. These countries may have data protection laws that differ from the laws of your country.

Israel is recognized by the European Commission as providing an **adequate level of data protection**, which facilitates lawful transfers of personal data from the EU/EEA to Israel. For transfers to the United States (via Google Cloud and other US-based service providers), we rely on appropriate safeguards such as Standard Contractual Clauses approved by the European Commission, together with supplementary technical and organizational measures.

---

## 8. Third-Party Links and Services

The App may integrate with or link to third-party services (e.g., Google Sign-In, Google Play Store, RevenueCat). This Privacy Policy does not apply to the practices of those third parties. We encourage you to review the privacy policies of any third-party services you interact with through the App.

---

## 9. Children's Privacy

The App is not directed to children under the age of 16. We do not knowingly collect personal information from children under 16. In jurisdictions that set a lower age of digital consent, we still apply 16 as our minimum unless local law mandates otherwise. If you become aware that a child has provided us with personal information without parental consent, please contact us immediately. If we become aware that we have collected personal information from a child in violation of applicable law, we will take steps to remove that information promptly.

---

## 10. AI Processing and Nutritional Data — Important Notice

DishSense.AI uses artificial intelligence to analyze food images and generate nutritional and macronutrient estimates, satiety scores, dietary tags, nutritional flags, and processing-level classifications. **You must understand the following limitations:**

* **All AI outputs are approximate.** Calorie, protein, carbohydrate, fat, satiety score, dietary tag (e.g., vegan, keto, gluten-free), nutritional flag (e.g., high sodium), and processing-level (NOVA-style) outputs are AI-generated estimates only. They may not reflect the actual nutritional content, ingredient list, or dietary classification of your specific meal.
* **Dietary-classification labels are especially uncertain.** A "Gluten-Free" or "Dairy-Free" tag, for example, is an AI guess based on visible ingredients. Cross-contamination, hidden ingredients, and brand-specific recipes mean these tags must **never** be relied upon by anyone with celiac disease, food allergies, intolerances, or any other condition where ingredient certainty is medically important.
* **Results may vary significantly** depending on ingredient sourcing, preparation methods, cooking techniques, portion sizes, and the visual presentation of food.
* **Not a medical or dietary tool.** AI nutritional analysis provided by DishSense.AI is intended for general informational and entertainment purposes only. It is **not** intended to constitute medical advice, dietary guidance, clinical nutrition assessment, or any form of healthcare service.
* **Weekly PDF reports are auto-generated summaries.** The weekly report we email to premium subscribers is compiled automatically from the AI-generated meal data described above. It inherits all of the inaccuracies of the underlying data and compounds them across a week of meals. The report is **not** a medical document, clinical assessment, dietary plan, diagnostic tool, or therapeutic intervention. It is **not** a substitute for advice from a licensed physician, registered dietitian, certified nutritionist, or other qualified healthcare professional, and it must not be presented to a healthcare provider as if it were clinical data.
* **Do not rely on the App** for managing diabetes, eating disorders, food allergies, intolerances, metabolic conditions, weight-loss programs supervised by a clinician, or any other condition requiring precise nutritional monitoring.
* **Consult a professional.** If you have any health condition, allergy, or dietary restriction requiring specific dietary management, please consult a licensed healthcare provider, registered dietitian, or nutritionist directly.

The collection and AI processing of your food images is subject to this Privacy Policy and governed by the data practices of our AI service providers, including Google Cloud Vertex AI.

---

## 11. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes to our practices or for operational, legal, or regulatory reasons. We will alert you about material changes by updating the "Last Updated" date at the top of this Privacy Policy and, where appropriate, by an in-app notice. We encourage you to review this Privacy Policy periodically. Your continued use of the App after changes are posted constitutes your acceptance of the updated Privacy Policy.

---

## 12. Contact Us

If you have questions, concerns, or requests regarding this Privacy Policy or our data practices, please contact us at:

**DishSense.AI**
Email: dishsenseai@gmail.com

We will make every effort to respond to your inquiry promptly and in accordance with applicable law.
