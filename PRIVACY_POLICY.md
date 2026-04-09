# Privacy Policy for DishSense.AI

**Last Updated:** April 9, 2026

Welcome to DishSense.AI! This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you use our mobile application (the "App") and related services (collectively, the "Service"). Please read this Privacy Policy carefully. If you do not agree with the terms of this Privacy Policy, please do not access or use the App.

---

## 1. Information We Collect

We may collect information about you in a variety of ways. The information we may collect via the App includes:

### A. Personal Data
* **Account Information:** When you register, we collect authentication information through third-party providers (such as Google Sign-In), which may provide us with your name, email address, and profile picture. We do not receive or store your Google account password.
* **User-Generated Content:** To provide our core services, we collect the photos and images of food that you upload or capture using your device's camera. These images are processed by AI services and stored in Google Cloud Storage.

### B. Financial Data
* **In-App Purchases:** If you purchase "Coins" or credits within the App, your payment is processed directly by the Google Play Store. We do not collect, store, or have access to your full payment card number or direct billing information. We receive transaction receipt data solely to grant you the purchased credits and verify transactional integrity.

### C. Automatically Collected Data
* **Device and Usage Information:** We may automatically collect certain information when you use the App, such as your device type, operating system version, unique device identifiers, IP address, and data regarding your interaction with the App (e.g., features used, screens viewed, session duration). This data is used for diagnostics, fraud prevention, and service improvement.
* **Crash Reports and Diagnostics:** The App may automatically collect technical error and crash data to help us identify and fix bugs.

### D. Push Notifications
* **Notification Data:** With your permission, we may send push notifications to your device to inform you when your meal analysis is complete or for other service-related updates. Notification tokens are stored securely and used solely to deliver notifications. You may opt out of receiving push notifications at any time through your device settings.

---

## 2. How We Use Your Information

We use the information we collect to operate, maintain, and improve the Service. Specifically, we may use information collected about you to:

* **Provide Core AI Services:** Transmit your uploaded food images to third-party AI services (Google Cloud Vertex AI) to analyze food content, generate approximate macronutrient and nutritional estimates, and produce "exploded-view" culinary composites. **Please note: all AI-generated nutritional data is an approximation only.** See Section 10 for full details.
* **Manage Your Account:** Create and manage your account, process login and authentication, and maintain your usage profile.
* **Process Transactions:** Verify in-app purchases through the Google Play Store, manage your Coin balance, and enforce our "No Success, No Charge" policy.
* **Deliver Notifications:** Send push notifications regarding analysis completion and service updates.
* **Improve Our Services:** Analyze aggregated usage trends and technical performance data to improve the App's functionality, reliability, and user experience.
* **Comply with Legal Obligations:** Respond to lawful requests from public authorities and comply with applicable laws and regulations.
* **Prevent Fraud and Abuse:** Detect, investigate, and prevent fraudulent transactions, abuse, and other harmful or illegal activity.

---

## 3. Disclosure of Your Information

We do not sell your personal information. We may share information we have collected in the following circumstances:

* **Third-Party Service Providers:** We share data with vendors and service providers that perform services on our behalf, including:
  * **Google Cloud Vertex AI** — AI image analysis and content generation
  * **Google Cloud Storage** — Secure storage of uploaded images
  * **Google Cloud Run** — Backend API hosting
  * **MongoDB Atlas** — Database services
  * **Upstash** — In-memory caching and queue management
  * **Google Firebase / FCM** — Push notification delivery
  * **Google Play Billing** — In-app purchase processing

  These providers are contractually obligated to use your data only to provide services to us and in accordance with this Privacy Policy.

* **Business Transfers:** If DishSense.AI is involved in a merger, acquisition, asset sale, or similar transaction, your information may be transferred as a business asset. We will provide notice before your personal information is transferred and becomes subject to a different privacy policy.

* **By Law or to Protect Rights:** We may disclose your information if required to do so by law, court order, or governmental authority, or if we believe disclosure is necessary to: (a) comply with a legal obligation; (b) protect and defend our rights or property; (c) prevent or investigate possible wrongdoing in connection with the Service; (d) protect the personal safety of users of the Service or the public; or (e) protect against legal liability.

* **With Your Consent:** We may share your information for any other purpose with your prior explicit consent.

---

## 4. Data Security

We implement administrative, technical, and physical security measures designed to protect your personal information from unauthorized access, use, alteration, and disclosure:

* All data in transit is encrypted using TLS/HTTPS.
* Authentication is secured via signed JSON Web Tokens (JWT) with server-side validation.
* API secrets, credentials, and keys are managed dynamically using Google Cloud Secret Manager — no secrets are hardcoded in the application.
* Access to production systems is restricted to authorized personnel only.

**However, please be aware that no security system is impenetrable.** While we have taken reasonable steps to protect your information, we cannot guarantee the absolute security of any data you transmit to us or that is stored on our systems. You provide personal information at your own risk.

---

## 5. Data Retention and Deletion

We retain your personal information and uploaded images only for as long as necessary to fulfill the purposes outlined in this Privacy Policy, or as required or permitted by applicable law.

**Account Deletion:** You may request the deletion of your account and associated data at any time from within the App settings. Upon receiving a deletion request:

* Your account is deactivated immediately.
* All associated account data, authentication records, and uploaded images are scheduled for **permanent, irreversible deletion 14 days** after the request.
* During this 14-day grace period, you may log back in to cancel the deletion and fully restore your account.
* After the 14-day period has elapsed, all data is permanently removed and **cannot be recovered**.

Certain data may be retained for longer periods where required by law (e.g., financial transaction records) or for legitimate business purposes such as fraud prevention and security.

---

## 6. Your Privacy Rights

Depending on your location, you may have certain rights regarding your personal information:

### California Residents (CCPA/CPRA)
If you are a California resident, you have the right to:
* **Know** what personal information we collect, use, disclose, or sell about you.
* **Delete** personal information we have collected from you (subject to certain exceptions).
* **Correct** inaccurate personal information we hold about you.
* **Opt-Out** of the sale or sharing of your personal information. We do not sell personal information.
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

To exercise any of these rights, please contact us using the information in Section 11. We will respond to verified requests within the timeframes required by applicable law.

---

## 7. International Data Transfers

DishSense.AI is developed and operated by a company based in **Israel**. Your information is stored and processed on infrastructure provided by Google Cloud Platform, located primarily in the United States. If you are accessing the App from outside these countries, please be aware that your information may be transferred to, stored, and processed in Israel, the United States, or other countries where our service providers operate. These countries may have data protection laws that differ from the laws of your country.

Israel is recognized by the European Commission as providing an **adequate level of data protection**, which facilitates lawful transfers of personal data from the EU/EEA to Israel. For transfers to the United States (via Google Cloud infrastructure), we rely on appropriate safeguards such as Standard Contractual Clauses approved by the European Commission.

---

## 8. Third-Party Links and Services

The App may integrate with or link to third-party services (e.g., Google Sign-In). This Privacy Policy does not apply to the practices of those third parties. We encourage you to review the privacy policies of any third-party services you interact with through the App.

---

## 9. Children's Privacy

The App is not directed to children under the age of 13 (or 16 where applicable under local law). We do not knowingly collect personal information from children under these ages. If you become aware that a child has provided us with personal information without parental consent, please contact us immediately. If we become aware that we have collected personal information from a child in violation of applicable law, we will take steps to remove that information promptly.

---

## 10. AI Processing and Nutritional Data — Important Notice

DishSense.AI uses artificial intelligence to analyze food images and generate nutritional and macronutrient estimates. **You must understand the following limitations:**

* **Estimates are approximate.** AI-generated nutritional values (calories, protein, carbohydrates, fat, and other macronutrients) are estimates only. They may not reflect the actual nutritional content of your specific meal.
* **Results may vary significantly** depending on ingredient sourcing, preparation methods, cooking techniques, portion sizes, and visual presentation of food.
* **Not a medical or dietary tool.** AI nutritional analysis provided by DishSense.AI is intended for general informational and entertainment purposes only. It is **not** intended to constitute medical advice, dietary guidance, clinical nutrition assessment, or any form of healthcare service.
* **Do not rely on this App** for managing medical conditions, eating disorders, food allergies, diabetes, or any other health condition requiring precise nutritional monitoring.
* **Consult a professional.** If you have health conditions requiring specific dietary management, please consult a licensed healthcare provider, registered dietitian, or nutritionist.

The collection and AI processing of your food images is subject to this Privacy Policy and governed by the data practices of our AI service providers, including Google Cloud Vertex AI.

---

## 11. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes to our practices or for operational, legal, or regulatory reasons. We will alert you about material changes by updating the "Last Updated" date at the top of this Privacy Policy. We encourage you to review this Privacy Policy periodically. Your continued use of the App after changes are posted constitutes your acceptance of the updated Privacy Policy.

---

## 12. Contact Us

If you have questions, concerns, or requests regarding this Privacy Policy or our data practices, please contact us at:

**DishSense.AI**  
Email: dishsenseai@gmail.com

We will make every effort to respond to your inquiry promptly and in accordance with applicable law.