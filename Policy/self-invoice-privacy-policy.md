# Enterprise Self-Invoicing — Privacy Policy

This policy applies only to services provided by Enterprise Self-Invoicing (hereinafter "the App" or "we").

Last updated : 2026-07-20
Effective date : 2026-07-20
Operator : Chengdu Silk Software Co., Ltd. (成都思而科软件有限公司)
Official website : [https://www.silksoftware.com.cn/](https://www.silksoftware.com.cn/)



Welcome to Enterprise Self-Invoicing (hereinafter "the App" or "we"). The App is designed for Shopline merchants selling into European markets and provides the following main capabilities:

- **Compliant e-invoice generation**: automatically generates machine-readable electronic invoices (PDF + XML/UBL) based on each country's applicable invoicing rules once an order reaches the merchant-configured invoicing trigger.
- **Consumer invoice information collection**: collects personal or business invoice details from consumers at checkout, with per-country tax-ID format validation.
- **Forward and reverse invoice management**: automatically issues reverse (credit note) invoices when an order is refunded or cancelled, sharing a single continuous numbering sequence with forward invoices.
- **Multi-country configuration**: lets merchants configure tax-ID validation rules, invoicing triggers, invoice numbering, and invoice templates (branding, legal entity information, field visibility, language) independently for each enabled country/market.

This Privacy Policy explains how we collect, use, store, share, and protect merchant data and merchant customer data, and describes related rights and choices.

---



## 1. Scope

This policy applies to services we provide through:

- installation, authorization, configuration, and use of the App in the Shopline admin;
- our websites, help pages, and merchant support related to the App;
- API and webhook processing between Shopline and our servers to deliver the capabilities described above;
- checkout event data processing required to collect invoice information and render invoice content;
- invoice PDF/XML generation, storage, and retrieval operations.

---



## 2. Our Role in Processing Data

In most cases, for merchant store data and merchant customer data, the merchant typically determines the purposes and means of processing; we mainly act as a service provider for the merchant and process data according to the merchant's authorization and instructions. For merchant account information, billing information (if applicable), support communications, app runtime logs, generated invoice files, and security audit records, we may process such information as an independent controller or processor to provide, maintain, and protect the App.

If you are a merchant's customer (an end consumer) and wish to exercise rights related to invoices or personal data contained within invoices, we generally recommend contacting the merchant first; where permitted by applicable law, we will assist the merchant as needed.

---



## 3. Information We Collect



### 3.1 Information collected via Shopline or merchant authorization

Depending on the permissions granted at installation and the features you use, we may collect:

**(1) Store and merchant account information**

- store name, storefront domain, store ID, merchant ID
- merchant admin identifiers made available by Shopline for embedded apps
- app installation, authorization, and configuration status; OAuth tokens or equivalent credentials (stored on the server only)
- billing, plan, subscription, or service activation information (if applicable)

**(2) Consumer checkout invoice data (collected at time of purchase for invoice generation)**

- invoice type selected (personal or business)
- personal tax identification number (optional field, format validated per the merchant's country configuration)
- company name, VAT/company tax identification number, and company address (business invoices)
- buyer name, billing address, shipping address, and shipping country

**(3) Order and product data**

- order number, order status
- product name and description (including bundled/gift item names shown on the invoice line)
- quantity, unit price excluding tax, applicable tax rate and tax amount
- discounts, order-level promotions, and points redemption applied to each product line
- invoice total amount, payment date, and fulfillment/shipping date

**(4) Generated invoice data**

- invoice PDF (visual) and XML/UBL (machine-readable) content
- unique invoice number, invoice type (forward or reverse/credit note)
- for reverse invoices: the linked original invoice number and original invoice date
- invoice status (pending, issued, voided, or generation failed) and issue date

**(5) Configuration**

- enabled countries/markets, per-country tax-ID validation rules (length, character type), invoicing trigger settings (payment completed / fulfillment completed)
- invoice numbering rules, tax rates synced from the merchant's Shopline tax settings
- invoice template settings: brand logo, legal entity information (registered name, address, registration number, tax number, VAT ID, legal representative, WEEE registration number), field visibility, field ordering, and multi-language label configurations



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

Unless necessary for the service and lawfully authorized, we do not proactively collect sensitive personal information unrelated to the App's functions. We do not store full payment card numbers or CVV; payment processing is typically performed by Shopline or compliant payment providers. We do not verify the authenticity of tax identification numbers or VAT numbers with any tax authority — the App performs format validation only, based on rules configured by the merchant.

---



## 4. How We Use Information

We use data only as needed to provide the App, perform contracts, comply with legal obligations, and maintain platform security. Main purposes include:

### 4.1 Invoice generation and Shopline integration

- present the invoice information form at checkout and dynamically validate tax-ID/VAT format based on the consumer's shipping country and the merchant's configured rules
- listen to Shopline order webhooks (payment_success / fulfillment_created) and generate a forward invoice once the merchant-configured invoicing trigger is reached, provided invoice information was collected for that order
- calculate the tax-exclusive amount and tax amount for each product line using tax rates synced from the merchant's Shopline tax settings, and apply discounts and points redemption at the product-line level
- assign each invoice a unique, globally sequential invoice number (forward and reverse invoices share one sequence) and generate both PDF and XML/UBL formats
- automatically generate a reverse (credit note) invoice, linked to the original forward invoice, when an order is cancelled or refunded (in whole or in part)
- provide a merchant-facing invoice records dashboard for querying, filtering, previewing, and exporting invoice data



### 4.2 Security, verification, and risk control

- validate authorization and API calls
- monitor abnormal requests, error logs, abuse, and security risks
- troubleshoot and maintain stability and audit trails



### 4.3 Customer support and product improvement

- respond to merchant inquiries, incidents, and implementation support
- measure usage and stability
- use de-identified or aggregated data for performance, UX, and product iteration



### 4.4 Legal and compliance

- comply with EU e-invoicing mandates and applicable member-state VAT/tax retention regulations, and applicable data protection regulations
- comply with laws, court orders, regulators, or government requests
- handle lawful requests for access, correction, deletion, or restriction
- perform contracts, disputes, audits, and compliance management

---



## 5. Legal Bases for Processing

Where required by applicable law, such bases may include:

- **Contract**: processing necessary to provide the App to merchants and to fulfill EU e-invoicing compliance requirements on behalf of merchants
- **Legal obligation**: compliance with EU VAT Directive requirements and applicable member-state regulations requiring the issuance, format, and retention of machine-readable electronic invoices
- **Legitimate interests**: security, fraud prevention, product improvement, and support
- **Consent**: where consent is required, based on merchant or end-user consent

---



## 6. Invoice Data Retention and Immutability

Given the legal nature of the invoices generated by this App:

- Once generated, invoice PDF and XML/UBL content is stored and is not edited; corrections to an issued invoice are made exclusively through a reverse (credit note) invoice, never by altering the original invoice record.
- Invoice data is retained for a minimum of **10 years** (or longer if required by the applicable EU member state's VAT/tax retention rules) to satisfy legal requirements for electronic invoices.
- Invoice numbers, reverse-invoice linkage records, and the associated numbering sequence are retained for the same period to preserve global sequence continuity.
- Merchant configuration data (template settings, tax-ID validation rules, numbering rules) may be deleted or anonymized within 90 days of App uninstallation; however, invoices that have already been generated will not be affected by uninstallation.

---



## 7. Cookies and Similar Technologies

When you use the App within Shopline admin or our related web pages, we may use cookies, pixels, local storage, or similar technologies to maintain sessions, save preferences, authenticate and secure sessions, and record errors and performance. You can manage cookies in your browser; disabling some cookies may affect certain features.

---



## 8. How We Share Information

We do not sell merchant data or merchant customer data.

- **Service providers**: we may share necessary data with providers such as Shopline and cloud/hosting/database/CDN/monitoring/logging/email vendors (e.g., AWS S3 or equivalent)
- **At your direction**: data transmitted to Shopline to synchronize tax rates, write invoice-related order data, and display invoice records on merchant-facing pages
- **Consumer access**: invoice PDF/XML files are made available to consumers or merchants via the plugin's invoice records interface; this is a core feature of the App
- **Legal or security needs**: to comply with law, court orders, regulators, or law enforcement; to protect rights and safety; to prevent fraud, abuse, or unauthorized access
- **Corporate transactions**: in mergers, acquisitions, restructurings, asset sales, financing, or similar events, data may transfer as part of the transaction; recipients must continue to handle data lawfully

---



## 9. Data Retention

We follow a "minimum necessary, retain as needed" approach. After uninstalling the App or terminating service, non-essential configuration data may be deleted or anonymized within 90 days; **invoice PDFs, XML/UBL files, and associated records are subject to the extended retention period described in Section 6** and will not be deleted solely due to App uninstallation.

---



## 10. International Transfers

Information may be transferred to, stored in, or processed in countries or regions outside your jurisdiction (for example: regions where our hosting providers and Shopline process data). We apply reasonable safeguards as required by applicable law, including for transfers of personal data outside the European Economic Area.

---



## 11. Security

We use HTTPS/TLS, access controls, authentication, logging, backups, and disaster recovery. OAuth / access tokens are stored on the server only and never exposed to the client. Invoice PDFs and XML/UBL files are stored in access-controlled object storage with server-side encryption; access is limited to authenticated requests only. No internet transmission or electronic storage is ever fully secure.

---



## 12. Your Rights

Where applicable law grants rights, you or merchant customers may have access, rectification, erasure, restriction, withdrawal of consent, portability, or complaint to a regulator.

Please note: given that invoice records are legally required documents under EU e-invoicing and VAT retention rules, the right to erasure may be subject to limitations during the mandatory retention period.

Merchants may contact us at [apps@silksoftware.com](mailto:apps@silksoftware.com); end consumers should usually contact the merchant first.

---



## 13. Uninstall and Deletion

When you uninstall the App, terminate service, or request deletion, we will handle requests in line with applicable law and platform requirements. Non-essential configuration data will be deleted or anonymized within 90 days. Invoices subject to legal retention requirements will be handled as described in Section 6.

For deletion requests, contact [apps@silksoftware.com](mailto:apps@silksoftware.com) with subject line: **Data Deletion Request / 数据删除请求**.

---



## 14. Third-Party Sites and Services

The App relies on Shopline (including its checkout, order, and tax-settings APIs) and cloud infrastructure providers to deliver the service; each has its own privacy policy. Please review their notices before use.

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