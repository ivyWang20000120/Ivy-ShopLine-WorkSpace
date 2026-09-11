# Member Custom Points — Privacy Policy

This policy applies only to services provided by Member Custom Points (hereinafter "the App" or "we").

Last updated : 2026-04-17
Effective date : 2026-04-17
Operator : Chengdu Silk Software Co., Ltd. (成都思而科软件有限公司)
Official website : [https://www.silksoftware.com.cn/](https://www.silksoftware.com.cn/)



Welcome to Member Custom Points (hereinafter "the App" or "we"). The App is designed for Shopline merchants and provides the following main capabilities:

- **Custom points rules**: merchants configure a fixed amount of extra points to be awarded after purchase for specified products, and may enable or disable each rule.
- **Order event processing**: the App receives Shopline webhooks related to orders and payment, completes signature verification, and issues points after payment is completed.
- **Merchant admin capabilities**: rule lists and filtering, and setting product-specific points rules for specific products.

This Privacy Policy explains how we collect, use, store, share, and protect merchant data and merchant customer data, and describes related rights and choices.

---

## 1. Scope

This policy applies to services we provide through:

- installation, authorization, configuration, and use of the App in the Shopline admin;
- our websites, help pages, and merchant support related to the App;
- API and webhook processing between Shopline and our servers to deliver the capabilities described above;
- data synchronization required to read products, receive orders, and update member points through Shopline.

---

## 2. Our Role in Processing Data

In most cases, for merchant store data and merchant customer data, the merchant typically determines the purposes and means of processing; we mainly act as a service provider for the merchant and process data according to the merchant's authorization and instructions. For merchant account information, billing information (if applicable), support communications, app runtime logs, and security audit records, we may process such information as an independent controller or processor to provide, maintain, and protect the App.

If you are a merchant's customer (an end consumer) and wish to exercise rights related to orders or member points, we generally recommend contacting the merchant first; where permitted by applicable law, we will assist the merchant as needed.

---

## 3. Information We Collect

### 3.1 Information collected via Shopline or merchant authorization

Depending on the permissions granted at installation and the features you use, we may collect:

**(1) Store and merchant account information**

- store name, storefront domain, store ID, merchant ID
- merchant admin identifiers made available by Shopline for embedded apps (e.g., name, email)
- app installation, authorization, and configuration status; OAuth tokens or equivalent credentials (stored on the server only)
- billing, plan, subscription, or service activation information (if applicable)

**(2) Product and catalog data**

- product ID, name, SKU/variants (as needed), images, categories
- fields required to match order line items to rules

**(3) Orders, fulfillment, and customer/member data**

- order number, order status, and status fields related to paid status and fulfillment/shipping
- line items, quantities, product identifiers, and amounts required to evaluate rules
- customer/member identifiers necessary to issue points through Shopline's member system (e.g., customer or member IDs provided by the platform)
- limited contact or profile fields only where included in Shopline payloads and minimally necessary for issuing points or logging

**(4) Configuration**

- rule configuration (product–points mapping), enabled/disabled status, and global issuance timing (Paid / Fulfilled)

### 3.2 Information you provide to us

When configuring or using the App, you may provide:

- support tickets, emails, online communications, and feedback you send us
- exports or attachments you choose to provide for troubleshooting (if the feature is available)

### 3.3 Admin, device, and usage information

When you use the App within Shopline admin or our related web pages, we may collect:

- IP address, browser type, device type, operating system, access time
- page paths, referrer, language preferences
- cookies, local storage, session identifiers, or similar technologies
- data used for sessions, authentication, security, troubleshooting, and performance

### 3.4 Information we generally do not collect

Unless necessary for the service and lawfully authorized, we do not proactively collect sensitive personal information unrelated to the App's functions. We do not store full payment card numbers or CVV; payment processing is typically performed by Shopline or compliant payment providers.

---

## 4. How We Use Information

We use data only as needed to provide the App, perform contracts, comply with legal obligations, and maintain platform security. Main purposes include:

### 4.1 Custom points rules and Shopline integration

- enable merchants to create, edit, enable, disable, or delete product-based points rules
- query product information to configure rules
- receive and verify webhooks and apply Paid / Fulfilled logic (including product-defined boundaries such as no issuance on partial shipment)
- match line items to rules and call Shopline's official points update APIs
- implement idempotency (e.g., no duplicate points for the same order and rule under the same issuance semantics)
- write logs and optional dashboards for operations and audit

### 4.2 Security, verification, and risk control

- validate authorization and API calls
- verify webhook signatures as required by Shopline and, within supported scope, guard against replay or tampering
- monitor abnormal requests, error logs, abuse, and security risks
- troubleshoot and maintain stability and audit trails

### 4.3 Customer support and product improvement

- respond to merchant inquiries, incidents, and implementation support
- measure usage and stability
- use de-identified or aggregated data for performance, UX, and product iteration

### 4.4 Legal and compliance

- comply with laws, court orders, regulators, or government requests
- handle lawful requests for access, correction, deletion, or restriction
- perform contracts, disputes, audits, and compliance management

---

## 5. Legal Bases for Processing

Where required by applicable law, such bases may include:

- **Contract**: processing necessary to provide the App to merchants
- **Legitimate interests**: security, fraud prevention, product improvement, and support
- **Consent**: where consent is required, based on merchant or end-user consent
- **Legal obligation**: regulatory, compliance, or data-protection obligations

---

## 6. Cookies and Similar Technologies

When you use the App within Shopline admin or our related web pages, we may use cookies, pixels, local storage, or similar technologies to maintain sessions, save preferences, authenticate and secure sessions, and record errors and performance. You can manage cookies in your browser; disabling some cookies may affect certain features.

---

## 7. How We Share Information

We do not sell merchant data or merchant customer data.

- **Service providers**: we may share necessary data with providers such as Shopline and cloud/hosting/database/CDN/monitoring/logging/email vendors
- **At your direction**: when you use the App, we process and transmit data to Shopline within the necessary scope to implement points issuance and related operations
- **Legal or security needs**: to comply with law, court orders, regulators, or law enforcement; to protect rights and safety; to prevent fraud, abuse, or unauthorized access
- **Corporate transactions**: in mergers, acquisitions, restructurings, asset sales, financing, or similar events, data may transfer as part of the transaction; recipients must continue to handle data lawfully

---

## 8. Data Retention

We follow a "minimum necessary, retain as needed" approach. After uninstalling the App or terminating service, non-essential data may be deleted or anonymized within 90 days; data required for audit or compliance may be retained longer.

Whether refunds or order cancellation trigger reversal or adjustment of points depends on product implementation and Shopline capabilities; related records may be retained as needed for consistency and dispute handling.

---

## 9. International Transfers

Information may be transferred to, stored in, or processed in countries or regions outside your jurisdiction (for example: regions where our hosting providers and Shopline process data). We apply reasonable safeguards as required by applicable law.

---

## 10. Security

We use HTTPS/TLS, access controls, authentication, logging, backups, and disaster recovery. OAuth / access tokens are stored on the server only and never exposed to the client. No internet transmission or electronic storage is ever fully secure.

---

## 11. Your Rights

Where applicable law grants rights, you or merchant customers may have access, rectification, erasure, restriction, withdrawal of consent, portability, or complaint to a regulator. Merchants may contact us at [apps@silksoftware.com](mailto:apps@silksoftware.com); end consumers should usually contact the merchant first.

---

## 12. Uninstall and Deletion

When you uninstall the App, terminate service, or request deletion, we will handle requests in line with applicable law and platform requirements. For deletion requests, contact [apps@silksoftware.com](mailto:apps@silksoftware.com) with subject line: **Data Deletion Request / 数据删除请求**.

---

## 13. Third-Party Sites and Services

The App relies on Shopline and may link to other third-party sites or services; each has its own privacy policy. Please review their notices before use.

---

## 14. Children's Privacy

The App is intended for Shopline merchants and business workflows, not children. If you believe we collected information in error, contact us at [apps@silksoftware.com](mailto:apps@silksoftware.com).

---

## 15. Changes to This Policy

We may update this policy for feature or legal changes. For material changes we will notify you by reasonable means such as our website, in-app notices, or email. The updated version takes effect from the "last updated" date shown on this page.

---

## 16. Contact Us

Company name : Chengdu Silk Software Co., Ltd. (成都思而科软件有限公司)
Email : [apps@silksoftware.com](mailto:apps@silksoftware.com)
Address: 3rd Floor, Building E2-1, Tianfu Software Park, Wuhou District, Chengdu
Website: [https://www.silksoftware.com.cn/](https://www.silksoftware.com.cn/)

---

Copyright © 2026 Chengdu Silk Software Co., Ltd. (成都思而科软件有限公司). All Rights Reserved.