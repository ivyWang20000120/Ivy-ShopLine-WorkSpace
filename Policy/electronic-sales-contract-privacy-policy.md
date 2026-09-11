# Electronic Sales Contract — Privacy Policy

This policy applies only to services provided by Electronic Sales Contract (hereinafter "the App" or "we").

Last updated : 2026-06-30
Effective date : 2026-06-30
Operator : Chengdu Silk Software Co., Ltd. (成都思而科软件有限公司)
Official website : [https://www.silksoftware.com.cn/](https://www.silksoftware.com.cn/)



Welcome to Electronic Sales Contract (hereinafter "the App" or "we"). The App is designed for Shopline merchants and provides the following main capabilities:

- **Electronic contract generation**: automatically renders the Preliminary Information Form and Distance Sales Contract based on real-time checkout data (buyer information, product details, amounts, etc.).
- **Mandatory consent mechanism**: requires consumers to read and agree to both contracts before payment can proceed, ensuring compliance with Turkish remote sales regulations.
- **Contract storage and order binding**: upon successful payment, generates contract PDFs, stores them permanently, and binds contract IDs to the corresponding Shopline order via extension fields.
- **Multi-channel contract access**: consumers can view signed contracts via order confirmation email or the storefront order detail page; merchants can access contracts via the plugin's merchant portal.

This Privacy Policy explains how we collect, use, store, share, and protect merchant data and merchant customer data, and describes related rights and choices.

---



## 1. Scope

This policy applies to services we provide through:

- installation, authorization, configuration, and use of the App in the Shopline admin;
- our websites, help pages, and merchant support related to the App;
- API and webhook processing between Shopline and our servers to deliver the capabilities described above;
- checkout event data processing required to render contract content;
- contract PDF generation, storage, and retrieval operations.

---



## 2. Our Role in Processing Data

In most cases, for merchant store data and merchant customer data, the merchant typically determines the purposes and means of processing; we mainly act as a service provider for the merchant and process data according to the merchant's authorization and instructions. For merchant account information, billing information (if applicable), support communications, app runtime logs, generated contract PDFs, and security audit records, we may process such information as an independent controller or processor to provide, maintain, and protect the App.

If you are a merchant's customer (an end consumer) and wish to exercise rights related to your contracts or personal data contained within contracts, we generally recommend contacting the merchant first; where permitted by applicable law, we will assist the merchant as needed.

---



## 3. Information We Collect



### 3.1 Information collected via Shopline or merchant authorization

Depending on the permissions granted at installation and the features you use, we may collect:

**(1) Store and merchant account information**

- store name, storefront domain, store ID, merchant ID
- merchant admin identifiers made available by Shopline for embedded apps
- app installation, authorization, and configuration status; OAuth tokens or equivalent credentials (stored on the server only)
- billing, plan, subscription, or service activation information (if applicable)

**(2) Consumer checkout data (collected at time of purchase for contract generation)**

- receiver name, delivery address, phone number
- buyer email address, billing address
- Turkish Republic ID number (collected via custom form field at checkout)
- tax office information (collected via custom form field at checkout)

**(3) Order and product data**

- order number, order status
- product name, product type, quantity, unit price (including VAT)
- discount / coupon amount, shipping fee, order total, product subtotal (excluding shipping)
- order date

**(4) Generated contract data**

- Preliminary Information Form PDF content and unique contract ID
- Distance Sales Contract PDF content and unique contract ID
- buyer signature (receiver name) and contract date
- contract IDs written to Shopline order extension fields

**(5) Configuration**

- seller information, fixed content templates, enabled/disabled variable field settings, multi-language content configurations



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

### 4.1 Contract generation and Shopline integration

- render Preliminary Information Form and Distance Sales Contract content using real-time checkout event data (CheckoutDetailInit / CheckoutDetailUpdate)
- enforce the mandatory consent mechanism: preventing payment submission when both contracts have not been agreed to
- generate and permanently store contract PDFs upon successful payment; contract content is locked and immutable after generation
- write contract unique IDs to Shopline order extension fields to enable order-contract traceability
- inject contract PDF links into Shopline transactional emails or send supplementary notification emails
- provide contract access via storefront order detail pages and merchant plugin portal



### 4.2 Security, verification, and risk control

- validate authorization and API calls
- monitor abnormal requests, error logs, abuse, and security risks
- troubleshoot and maintain stability and audit trails



### 4.3 Customer support and product improvement

- respond to merchant inquiries, incidents, and implementation support
- measure usage and stability
- use de-identified or aggregated data for performance, UX, and product iteration



### 4.4 Legal and compliance

- comply with Turkish remote sales law and applicable data protection regulations
- comply with laws, court orders, regulators, or government requests
- handle lawful requests for access, correction, deletion, or restriction
- perform contracts, disputes, audits, and compliance management

---



## 5. Legal Bases for Processing

Where required by applicable law, such bases may include:

- **Contract**: processing necessary to provide the App to merchants and to fulfill Turkish remote sales compliance requirements on behalf of merchants
- **Legal obligation**: compliance with Turkish remote sales law (and other applicable regulations) requiring consumer consent to Preliminary Information Form and Distance Sales Contract prior to payment
- **Legitimate interests**: security, fraud prevention, product improvement, and support
- **Consent**: where consent is required, based on merchant or end-user consent

---



## 6. Contract Data Retention and Immutability

Given the legal nature of the contracts generated by this App:

- Contract PDFs are stored permanently and immutably once generated; content cannot be modified by any party (including merchants, Silk, or consumers) after generation.
- Contract data is retained for a minimum of **5 years** (or longer if required by applicable law or merchant request) to satisfy Turkish legal requirements for remote sales contracts.
- Contract IDs and associated order binding records are retained for the same period.
- Merchant configuration data (fixed content templates, field settings) may be deleted or anonymized within 90 days of App uninstallation; however, contract PDFs that have already been generated will not be affected by uninstallation.

---



## 7. Cookies and Similar Technologies

When you use the App within Shopline admin or our related web pages, we may use cookies, pixels, local storage, or similar technologies to maintain sessions, save preferences, authenticate and secure sessions, and record errors and performance. You can manage cookies in your browser; disabling some cookies may affect certain features.

---



## 8. How We Share Information

We do not sell merchant data or merchant customer data.

- **Service providers**: we may share necessary data with providers such as Shopline and cloud/hosting/database/CDN/monitoring/logging/email vendors (e.g., AWS S3 or equivalent)
- **At your direction**: data transmitted to Shopline to implement contract ID binding, transactional email injection, and order detail page display operations
- **Consumer access**: contract PDF links are provided to consumers via order confirmation email and storefront order detail pages; this is a core feature of the App
- **Legal or security needs**: to comply with law, court orders, regulators, or law enforcement; to protect rights and safety; to prevent fraud, abuse, or unauthorized access
- **Corporate transactions**: in mergers, acquisitions, restructurings, asset sales, financing, or similar events, data may transfer as part of the transaction; recipients must continue to handle data lawfully

---



## 9. Data Retention

We follow a "minimum necessary, retain as needed" approach. After uninstalling the App or terminating service, non-essential configuration data may be deleted or anonymized within 90 days; **contract PDFs and associated records are subject to the extended retention period described in Section 6** and will not be deleted solely due to App uninstallation.

---



## 10. International Transfers

Information may be transferred to, stored in, or processed in countries or regions outside your jurisdiction (for example: regions where our hosting providers and Shopline process data). We apply reasonable safeguards as required by applicable law.

---



## 11. Security

We use HTTPS/TLS, access controls, authentication, logging, backups, and disaster recovery. OAuth / access tokens are stored on the server only and never exposed to the client. Contract PDFs are stored in access-controlled object storage with server-side encryption; access is limited to authenticated requests only. No internet transmission or electronic storage is ever fully secure.

---



## 12. Your Rights

Where applicable law grants rights, you or merchant customers may have access, rectification, erasure, restriction, withdrawal of consent, portability, or complaint to a regulator.

Please note: given that contract PDFs are legally required records under Turkish remote sales law, the right to erasure may be subject to limitations during the mandatory retention period.

Merchants may contact us at [apps@silksoftware.com](mailto:apps@silksoftware.com); end consumers should usually contact the merchant first.

---



## 13. Uninstall and Deletion

When you uninstall the App, terminate service, or request deletion, we will handle requests in line with applicable law and platform requirements. Non-essential configuration data will be deleted or anonymized within 90 days. Contract PDFs subject to legal retention requirements will be handled as described in Section 6.

For deletion requests, contact [apps@silksoftware.com](mailto:apps@silksoftware.com) with subject line: **Data Deletion Request / 数据删除请求**.

---



## 14. Third-Party Sites and Services

The App relies on Shopline and may interact with transactional email services; each has its own privacy policy. Please review their notices before use.

---



## 15. Children's Privacy

The App is intended for Shopline merchants and business workflows, not children. If you believe we collected information in error, contact us at [apps@silksoftware.com](mailto:apps@silksoftware.com).

---



## 16. Changes to This Policy

We may update this policy for feature or legal changes. For material changes we will notify you by reasonable means such as our website, in-app notices, or email. The updated version takes effect from the "last updated" date shown on this page.

---



## 17. Contact Us

Company name : Chengdu Silk Software Co., Ltd. (成都思而科软件有限公司)
Email : [apps@silksoftware.com](mailto:apps@silksoftware.com)
Address: 3rd Floor, Building E2-1, Tianfu Software Park, Wuhou District, Chengdu
Website: [https://www.silksoftware.com.cn/](https://www.silksoftware.com.cn/)

---

Copyright © 2026 Chengdu Silk Software Co., Ltd. (成都思而科软件有限公司). All Rights Reserved.