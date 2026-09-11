# Shipping Insurance — Privacy Policy

This policy applies only to services provided by Shipping Insurance (hereinafter "the App" or "we").

Last updated : 2026-08-13
Effective date : 2026-08-13
Operator : Chengdu Silk Software Co., Ltd. (成都思而科软件有限公司)
Official website : [https://www.silksoftware.com.cn/](https://www.silksoftware.com.cn/)



Welcome to Shipping Insurance (hereinafter "the App" or "we"). The App is designed for Shopline merchants and provides the following main capabilities:

- **Shipping insurance opt-in widget**: displays an insurance selection component at checkout and in the cart, allowing buyers to opt in to shipping insurance for their order.
- **Automated premium billing and wallet management**: collects insurance premiums from merchants via a prepaid wallet; automatically deducts the calculated premium when an order is fulfilled.
- **Package-level policy issuance**: upon shipment, submits each package to Cathay Insurance via API to issue an individual insurance policy; tracks logistics status via 17TRACK.
- **Claims and appeals management**: allows merchants to file insurance claims and submit appeals directly within the plugin; processes Cathay Insurance review outcomes and updates policy status accordingly.
- **Payout and commission tracking**: records approved claim payouts and their settlement progress; calculates and credits monthly commissions to the merchant wallet based on Cathay Insurance actual premiums.

This Privacy Policy explains how we collect, use, store, share, and protect merchant data and merchant customer data, and describes related rights and choices.

---



## 1. Scope

This policy applies to services we provide through:

- installation, authorization, configuration, and use of the App in the Shopline admin;
- the independent operator console (Insurance Ops) used by platform staff;
- our websites, help pages, and merchant support related to the App;
- storefront checkout and cart pages where the insurance opt-in widget is enabled;
- API and webhook processing between Shopline, Cathay Insurance, 17TRACK, and our servers to deliver the capabilities described above;
- wallet, billing, policy, and payout data processing required to operate the insurance service.

---



## 2. Our Role in Processing Data

In most cases, for merchant store data and merchant customer data, the merchant typically determines the purposes and means of processing; we mainly act as a service provider for the merchant and process data according to the merchant's authorization and instructions. For merchant account information, billing information (if applicable), support communications, app runtime logs, insurance policy records, wallet transaction records, and security audit records, we may process such information as an independent controller or processor to provide, maintain, and protect the App.

If you are a merchant's customer (an end consumer) and wish to exercise rights related to your personal data, we generally recommend contacting the merchant first; where permitted by applicable law, we will assist the merchant as needed.

---



## 3. Information We Collect



### 3.1 Information collected via Shopline or merchant authorization

Depending on the permissions granted at installation and the features you use, we may collect:

**(1) Store and merchant account information**

- store name, storefront domain, store ID, merchant ID
- merchant admin identifiers made available by Shopline for embedded apps
- app installation, authorization, and configuration status; OAuth tokens or equivalent credentials (stored on the server only)
- billing, plan, subscription, or service activation information (if applicable)

**(2) Order and fulfillment data**

- order number, order status, payment status, cancellation status
- product name, product type, quantity, unit price, order total, order currency
- shipment information: package number, tracking number, carrier, fulfillment timestamp

**(3) Insurance billing and wallet data**

- calculated premium amount per order and per package (in original currency and USD equivalent)
- wallet balance, top-up records (amount, Shopline billing reference), and transaction history
- billing records: bill number, pay status, insurance status, refund records

**(4) Policy data**

- package-level policy number issued by Cathay Insurance
- insured amount, Cathay Insurance actual premium (in original currency and USD)
- policy status (active, refunded), claim status, appeal status
- logistics tracking status retrieved from 17TRACK

**(5) Claims and payout data**

- claim submission details: selected payout account, evidence submitted
- Cathay Insurance claim review outcome and reason codes
- payout number, claim number, payout amount, payout status

**(6) Commission data**

- commission number, settlement month, commission rate, commission amount, credit status

**(7) Merchant configuration data**

- insured certificate information: company name, certificate type, certificate number, contact name, contact telephone
- payout accounts: account type (Alipay / WeChat Pay / Bank), account holder name, encrypted account number, category, bank BIC code
- storefront widget settings: opt-in default, per-language copy, accent color, widget placement selectors
- charge plan settings (read from operator console): fixed amount, percentage rate, minimum charge, auto-cancel toggle



### 3.2 Information you provide to us

When configuring or using the App, you may provide:

- support tickets, emails, online communications, and feedback you send us
- exports or attachments you choose to provide for troubleshooting (if the feature is available)



### 3.3 Admin, device, and usage information

When you use the App within Shopline admin, our related web pages, or when buyers interact with the insurance widget on checkout or cart pages, we may collect:

- IP address, browser type, device type, operating system, access time
- page paths, referrer, language preferences
- cookies, local storage, session identifiers, or similar technologies
- data used for sessions, authentication, security, troubleshooting, and performance



### 3.4 Information we generally do not collect

Unless necessary for the service and lawfully authorized, we do not proactively collect sensitive personal information unrelated to the App's functions. We do not store full payment card numbers or CVV; payment processing is typically performed by Shopline or compliant payment providers. Payout account numbers are stored in encrypted form and displayed only as masked values in the interface.

---



## 4. How We Use Information

We use data only as needed to provide the App, perform contracts, comply with legal obligations, and maintain platform security. Main purposes include:

### 4.1 Insurance operations and Shopline integration

- display the insurance opt-in widget on the storefront checkout and cart pages via Shopline ScriptTag injection
- receive and process Shopline order webhooks (orders/create, orders/updated, orders/paid, orders/cancelled, appsubscription/paid) to trigger premium billing, refunds, and policy lifecycle events
- calculate and deduct insurance premiums from the merchant wallet upon order fulfillment
- submit package-level insurance applications to Cathay Insurance API and record issued policy numbers
- query logistics tracking status from 17TRACK and associate it with policies
- process claim submissions and appeals; relay outcomes from Cathay Insurance to update policy and payout records
- calculate and credit monthly commissions to merchant wallets; claw back commissions on refunded policies
- operate the operator console (Insurance Ops) to configure per-store charge plans, commission rates, exchange rate markups, and risk alert thresholds



### 4.2 Security, verification, and risk control

- validate Shopline OAuth authorization and Cathay Insurance API credentials
- monitor abnormal requests, error logs, abuse, and security risks
- operate risk alert monitoring: if a store's monthly claim-to-premium ratio exceeds the configured threshold, send alert notifications to designated operator email addresses
- troubleshoot and maintain stability and audit trails



### 4.3 Customer support and product improvement

- respond to merchant inquiries, incidents, and implementation support
- measure usage and stability; generate aggregated operational dashboards for operator use
- use de-identified or aggregated data for performance, UX, and product iteration



### 4.4 Legal and compliance

- comply with applicable financial services, insurance intermediary, and data protection regulations
- comply with laws, court orders, regulators, or government requests
- handle lawful requests for access, correction, deletion, or restriction
- perform contracts, disputes, audits, and compliance management

---



## 5. Legal Bases for Processing

Where required by applicable law, such bases may include:

- **Contract**: processing necessary to provide the App to merchants, to operate the wallet and billing service, and to submit and manage insurance policies with Cathay Insurance on behalf of merchants
- **Legitimate interests**: security, fraud prevention, risk monitoring, commission calculation, product improvement, and support
- **Legal obligation**: compliance with applicable insurance intermediary regulations and data-protection obligations
- **Consent**: where consent is required, based on merchant or end-user consent

---



## 6. Cookies and Similar Technologies

When you use the App within Shopline admin or our related web pages, we may use cookies, pixels, local storage, or similar technologies to maintain sessions, save preferences, authenticate and secure sessions, and record errors and performance. You can manage cookies in your browser; disabling some cookies may affect certain features.

---



## 7. How We Share Information

We do not sell merchant data or merchant customer data.

- **Cathay Insurance**: order, package, and shipment data necessary to issue policies, process claims, and settle payouts is transmitted to Cathay Insurance via their API. Cathay Insurance operates as an independent data controller for insurance policy issuance and claims decisions.
- **17TRACK**: package tracking numbers are submitted to 17TRACK to retrieve logistics status. 17TRACK operates as an independent service provider with its own privacy policy.
- **Shopline**: data is transmitted to Shopline to implement order webhooks, app billing (wallet top-up via Shopline's one-time purchase billing capability), storefront widget injection, and OAuth authorization flows.
- **Service providers**: we may share necessary data with providers such as cloud/hosting/database/CDN/monitoring/logging/email vendors and exchange rate data providers (e.g., Open Exchange Rates)
- **Legal or security needs**: to comply with law, court orders, regulators, or law enforcement; to protect rights and safety; to prevent fraud, abuse, or unauthorized access
- **Corporate transactions**: in mergers, acquisitions, restructurings, asset sales, financing, or similar events, data may transfer as part of the transaction; recipients must continue to handle data lawfully

---



## 8. Data Retention

We follow a "minimum necessary, retain as needed" approach. After uninstalling the App or terminating service, non-essential configuration data (widget settings, certificate information, payout account records) may be deleted or anonymized within 90 days. Insurance policy records, wallet transaction records, billing records, payout records, and commission records are retained for a minimum of **5 years** (or longer if required by applicable insurance or financial regulations) to satisfy regulatory and audit requirements. These records will not be deleted solely due to App uninstallation.

---



## 9. International Transfers

Information may be transferred to, stored in, or processed in countries or regions outside your jurisdiction (for example: regions where our hosting providers, Shopline, Cathay Insurance, and 17TRACK process data). We apply reasonable safeguards as required by applicable law.

---



## 10. Security

We use HTTPS/TLS, access controls, authentication, logging, backups, and disaster recovery. OAuth tokens and Cathay Insurance API credentials are stored on the server only and never exposed to the client. Payout account numbers are stored encrypted and displayed only in masked form. No internet transmission or electronic storage is ever fully secure.

---



## 11. Your Rights

Where applicable law grants rights, you or merchant customers may have access, rectification, erasure, restriction, withdrawal of consent, portability, or complaint to a regulator.

Please note: insurance policy records and financial transaction records subject to regulatory retention requirements may be exempt from the right to erasure during the mandatory retention period.

Merchants may contact us at [apps@silksoftware.com](mailto:apps@silksoftware.com); end consumers should usually contact the merchant first.

---



## 12. Uninstall and Deletion

When you uninstall the App, terminate service, or request deletion, we will handle requests in line with applicable law and platform requirements. Non-essential configuration data will be deleted or anonymized within 90 days. Policy, financial, and audit records subject to regulatory retention requirements will be retained as described in Section 8.

For deletion requests, contact [apps@silksoftware.com](mailto:apps@silksoftware.com) with subject line: **Data Deletion Request / 数据删除请求**.

---



## 13. Third-Party Sites and Services

The App relies on the following third-party services, each of which operates under its own privacy policy:

- **Shopline** — e-commerce platform providing order management, webhook events, OAuth authorization, and app billing
- **Cathay Insurance (国泰财险)** — insurance underwriter providing policy issuance, claims review, and payout settlement via API
- **17TRACK** — logistics tracking service providing package status queries
- **Open Exchange Rates** — exchange rate data provider used to calculate USD-equivalent premium amounts

Please review their notices before use.

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