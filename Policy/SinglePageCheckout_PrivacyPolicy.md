# Single Page Checkout — Privacy Policy

This policy applies only to services provided by Single Page Checkout (hereinafter "the App" or "we").

Last updated : 2026-07-09
Effective date : 2026-07-09
Operator : Chengdu Silk Software Co., Ltd. (成都思而科软件有限公司)
Official website : [https://www.silksoftware.com.cn/](https://www.silksoftware.com.cn/)



Welcome to Single Page Checkout (hereinafter "the App" or "we"). The App is designed for Shopline EP-plan merchants and provides the following main capabilities:

- **Landing page visual editor**: an in-app editor that allows merchants to build and publish immersive advertorial landing pages — including product binding, theme colors, CTA buttons, feature lists, countdown timers, sticky bars, and bottom banners — without modifying Shopline theme code.
- **Checkout UI extension**: injects product images and customer reviews configured per landing page into the Shopline native checkout page via `customAttributes`, helping increase buyer confidence at the point of payment.
- **Shipping Insurance**: appends a configurable insurance line item to every checkout initiated from an App landing page; merchants may bind an existing product or auto-create a virtual product for this purpose.
- **Multi-page management**: supports creating multiple independent landing pages with separate Storefront URLs, each independently publishable or unpublishable.

This Privacy Policy explains how we collect, use, store, share, and protect merchant data and merchant customer data, and describes related rights and choices.

---

## 1. Scope

This policy applies to services we provide through:

- installation, authorization, configuration, and use of the App in the Shopline admin;
- landing pages published to merchant storefronts via the App;
- our websites, help pages, and merchant support related to the App;
- API and webhook processing between Shopline and our servers to deliver the capabilities described above;
- checkout customization data processing required to render the Checkout UI extension.

---

## 2. Our Role in Processing Data

In most cases, for merchant store data and merchant customer data, the merchant typically determines the purposes and means of processing; we mainly act as a service provider for the merchant and process data according to the merchant's authorization and instructions. For merchant account information, billing information (if applicable), support communications, app runtime logs, landing page configuration data, and security audit records, we may process such information as an independent controller or processor to provide, maintain, and protect the App.

If you are a merchant's customer (an end consumer) who has visited a landing page or completed a checkout initiated by this App, and you wish to exercise rights related to your personal data, we generally recommend contacting the merchant first; where permitted by applicable law, we will assist the merchant as needed.

---

## 3. Information We Collect

### 3.1 Information collected via Shopline or merchant authorization

Depending on the permissions granted at installation and the features you use, we may collect:

**(1) Store and merchant account information**

- store name, storefront domain, store ID, merchant ID
- merchant admin identifiers made available by Shopline for embedded apps
- app installation, authorization, and configuration status; OAuth tokens or equivalent credentials (stored on the server only)
- billing, plan, subscription, or service activation information (if applicable)
- Shopline plan type (used to verify EP plan eligibility for Checkout UI extension)

**(2) Product and variant data**

- product title, variant title, variant ID, SKU
- product images, pricing (price and compare_at_price fields)
- inventory status, product publish status
- the above data is read via the Shopline API solely to power landing page product display and checkout link generation; we do not store product data independently beyond what is needed for active landing page configuration

**(3) Landing page configuration data**

- page title, handle (URL identifier), publish status
- editor configuration: theme color, button style, body content (rich text), feature list items, CTA text and animation settings, countdown end time, sticky bar settings, bottom banner content, guarantee text
- Checkout Tab configuration: checkout extension image URL, customer review entries (reviewer name and review content)
- Shipping Insurance binding: bound product/variant ID and price

**(4) Checkout-related data (passed via customAttributes to Shopline checkout)**

- landing page identifier and checkout extension image URL
- customer review entries (reviewer name and review content) associated with the active landing page
- Shipping Insurance variant ID and quantity (when Shipping Insurance is enabled)

The above data is passed to the Shopline native checkout page via `customAttributes` and is not independently persisted by us beyond the landing page configuration already stored.

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

We do not collect end-consumer personal information (names, addresses, emails, phone numbers) directly — consumer data entered at Shopline checkout is handled entirely by Shopline and the merchant's selected payment and fulfillment providers. Unless necessary for the service and lawfully authorized, we do not proactively collect sensitive personal information unrelated to the App's functions. We do not store full payment card numbers or CVV; payment processing is typically performed by Shopline or compliant payment providers.

---

## 4. How We Use Information

We use data only as needed to provide the App, perform contracts, comply with legal obligations, and maintain platform security. Main purposes include:

### 4.1 Landing page delivery and Shopline checkout integration

- render and serve merchant-configured landing pages on Shopline storefronts, including product images, pricing, feature lists, countdown timers, and CTA buttons
- read product and variant data from Shopline to populate landing page product cards and generate cart permalink checkout links
- pass landing page configuration (product images, customer reviews, Shipping Insurance variant) to the Shopline Checkout UI extension via `customAttributes` so that the extension can display this content within the native checkout flow
- append the configured Shipping Insurance line item (quantity 1) to checkout sessions initiated from App landing pages, when the feature is enabled by the merchant
- auto-create or bind a virtual product in the merchant's Shopline store for use as the Shipping Insurance line item, at the merchant's direction

### 4.2 Security, verification, and risk control

- validate authorization and API calls
- verify EP plan status to gate access to Checkout UI extension features
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

- **Contract**: processing necessary to provide the App to merchants, including delivering landing pages, integrating with Shopline checkout, and managing merchant configurations
- **Legitimate interests**: security, fraud prevention, EP plan verification, product improvement, and support
- **Consent**: where consent is required, based on merchant or end-user consent
- **Legal obligation**: regulatory, compliance, or data-protection obligations

---

## 6. Cookies and Similar Technologies

When you use the App within Shopline admin or our related web pages, we may use cookies, pixels, local storage, or similar technologies to maintain sessions, save preferences, authenticate and secure sessions, and record errors and performance. You can manage cookies in your browser; disabling some cookies may affect certain features.

---

## 7. How We Share Information

We do not sell merchant data or merchant customer data.

- **Service providers**: we may share necessary data with providers such as Shopline and cloud/hosting/database/CDN/monitoring/logging/email vendors
- **Shopline platform**: landing page configuration data (product images, customer reviews, Shipping Insurance variant) is passed to the Shopline Checkout UI extension via `customAttributes` as a core feature of the App; the Shopline native checkout page then displays this content to end consumers
- **At your direction**: the Shipping Insurance virtual product is created in your Shopline store via the Admin API at the merchant's explicit request
- **Legal or security needs**: to comply with law, court orders, regulators, or law enforcement; to protect rights and safety; to prevent fraud, abuse, or unauthorized access
- **Corporate transactions**: in mergers, acquisitions, restructurings, asset sales, financing, or similar events, data may transfer as part of the transaction; recipients must continue to handle data lawfully

---

## 8. Data Retention

We follow a "minimum necessary, retain as needed" approach. Landing page configuration data (page content, product bindings, Checkout Tab settings, Shipping Insurance binding) is retained for as long as the App is installed and the merchant's account is active. After uninstalling the App or terminating service, non-essential configuration data may be deleted or anonymized within 90 days.

Product and variant data fetched from Shopline is not independently stored beyond what is necessary to render active landing page configurations; it is refreshed from the Shopline API on demand.

---

## 9. International Transfers

Information may be transferred to, stored in, or processed in countries or regions outside your jurisdiction (for example: regions where our hosting providers and Shopline process data). We apply reasonable safeguards as required by applicable law.

---

## 10. Security

We use HTTPS/TLS, access controls, authentication, logging, backups, and disaster recovery. OAuth / access tokens are stored on the server only and never exposed to the client. No internet transmission or electronic storage is ever fully secure.

---

## 11. Your Rights

Where applicable law grants rights, you or merchant customers may have access, rectification, erasure, restriction, withdrawal of consent, portability, or complaint to a regulator. Merchants may contact us at [apps@silksoftware.com](mailto:apps@silksoftware.com); end consumers should usually contact the merchant first regarding any personal data processed as part of a Shopline checkout or order.

---

## 12. Uninstall and Deletion

When you uninstall the App, terminate service, or request deletion, we will handle requests in line with applicable law and platform requirements. Non-essential configuration data will be deleted or anonymized within 90 days of uninstallation.

Note: the Shipping Insurance virtual product created in your Shopline store by the App will **not** be automatically deleted upon uninstallation. Merchants should manually remove or archive this product in their Shopline admin if it is no longer needed.

For deletion requests, contact [apps@silksoftware.com](mailto:apps@silksoftware.com) with subject line: **Data Deletion Request / 数据删除请求**.

---

## 13. Third-Party Sites and Services

The App relies on Shopline and cloud infrastructure providers and may link to other third-party sites or services; each has its own privacy policy. Shopline processes all checkout, payment, and order data independently. Please review [Shopline's Privacy Policy](https://shopline.com/privacy) and other relevant notices before use.

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