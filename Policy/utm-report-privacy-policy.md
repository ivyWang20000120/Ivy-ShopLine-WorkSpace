# UTM Report — Privacy Policy

This policy applies only to services provided by UTM Report (hereinafter "the App" or "we").

Last updated : 2026-06-15
Effective date : 2026-06-15
Operator : Chengdu Silk Software Co., Ltd. (成都思而科软件有限公司)
Official website : [https://www.silksoftware.com.cn/](https://www.silksoftware.com.cn/)



Welcome to UTM Report (hereinafter "the App" or "we"). The App is designed for Shopline merchants and provides the following main capabilities:

- **UTM data reporting**: aggregating and displaying UTM campaign data including traffic source, medium, campaign name, content, and keyword dimensions.
- **Conversion funnel analysis**: tracking user behavior from visit through add-to-cart, checkout initiation, to completed order, with conversion rate calculation.
- **Sales result reporting**: presenting sales amount, order volume, average order value, and new vs. returning customer breakdowns by UTM source.
- **Behavioral data collection**: capturing product detail page views, average session duration, and average browsing depth via front-end JavaScript tracking embedded in the merchant storefront.
- **Filter and date range selection**: supporting flexible filtering by UTM source, medium, campaign name, and custom date ranges.

This Privacy Policy explains how we collect, use, store, share, and protect merchant data and merchant customer data, and describes related rights and choices.

---



## 1. Scope

This policy applies to services we provide through:

- installation, authorization, configuration, and use of the App in the Shopline admin;
- our websites, help pages, and merchant support related to the App;
- API and webhook processing between Shopline and our servers to deliver the capabilities described above;
- front-end JavaScript tracking scripts injected into the merchant storefront for behavioral data collection;
- data synchronization required to read UTM attribution, conversion funnel metrics, and sales results through Shopline APIs.

---



## 2. Our Role in Processing Data

In most cases, for merchant store data and merchant customer data, the merchant typically determines the purposes and means of processing; we mainly act as a service provider for the merchant and process data according to the merchant's authorization and instructions. For merchant account information, billing information (if applicable), support communications, app runtime logs, front-end behavioral event data, and security audit records, we may process such information as an independent controller or processor to provide, maintain, and protect the App.

If you are a merchant's customer (an end consumer) and wish to exercise rights related to behavioral tracking or order data, we generally recommend contacting the merchant first; where permitted by applicable law, we will assist the merchant as needed.

---



## 3. Information We Collect



### 3.1 Information collected via Shopline or merchant authorization

Depending on the permissions granted at installation and the features you use, we may collect:

**(1) Store and merchant account information**

- store name, storefront domain, store ID, merchant ID
- merchant admin identifiers made available by Shopline for embedded apps
- app installation, authorization, and configuration status; OAuth tokens or equivalent credentials (stored on the server only)
- billing, plan, subscription, or service activation information (if applicable)

**(2) UTM attribution data**

- UTM parameters: utm_source, utm_medium, utm_campaign, utm_content, utm_term
- landing page URL path associated with each UTM session
- last-click attribution records with a 30-day rolling attribution window

**(3) Conversion funnel and behavioral data**

- unique visitor count (UV) per UTM dimension
- add-to-cart user count, checkout initiation count, completed checkout count
- conversion rate, bounce rate
- product detail page click count per UTM source (collected via front-end script)
- session duration per visitor per UTM source (collected via front-end script)
- page view count per visitor session per UTM source (collected via front-end script)

**(4) Sales and order data**

- sales amount (total_sales) and settlement currency code
- order count, average order value
- buyer count segmented by buyer type (new vs. returning customer)
- country / region dimension associated with each UTM record

**(5) Front-end behavioral tracking data**

- anonymous visitor identifier (visitor_id) generated client-side; not linked to real identity
- page type (e.g., product detail page), page URL, entry timestamp, exit timestamp, and page sequence index within a session
- UTM parameters read from the sl_utm cookie at the time of each tracked event
- above events are reported to our servers and associated with the corresponding UTM source for aggregated reporting only

**(6) Configuration**

- selected date range, active filter conditions, enabled report columns



### 3.2 Information you provide to us

When configuring or using the App, you may provide:

- support tickets, emails, online communications, and feedback you send us
- exports or attachments you choose to provide for troubleshooting (if the feature is available)



### 3.3 Admin, device, and usage information

When you use the App within Shopline admin, our related web pages, or when storefront visitors interact with the embedded tracking script, we may collect:

- IP address, browser type, device type, operating system, access time
- page paths, referrer, language preferences
- cookies, local storage, session identifiers, or similar technologies
- data used for sessions, authentication, security, troubleshooting, and performance



### 3.4 Information we generally do not collect

Unless necessary for the service and lawfully authorized, we do not proactively collect sensitive personal information unrelated to the App's functions. The front-end tracking script uses only anonymous visitor identifiers and does not collect names, email addresses, phone numbers, or payment information. We do not store full payment card numbers or CVV; payment processing is typically performed by Shopline or compliant payment providers.

---



## 4. How We Use Information

We use data only as needed to provide the App, perform contracts, comply with legal obligations, and maintain platform security. Main purposes include:

### 4.1 UTM reporting and data aggregation

- retrieve conversion funnel metrics and sales result data from Shopline APIs by UTM dimension
- aggregate front-end behavioral event data (product detail views, session duration, browsing depth) per UTM source using anonymous visitor identifiers
- calculate derived metrics: visitor share, sales share, new customer count, new customer share, average session duration, average browsing depth
- apply last-click attribution logic with a 30-day rolling window to assign sessions and orders to the correct UTM source
- render line charts, filterable tables, and summary cards within the merchant admin dashboard



### 4.2 Security, verification, and risk control

- validate authorization and API calls
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
- **Consent**: where consent is required, based on merchant or end-user consent; merchants are responsible for obtaining any consent required from their storefront visitors for front-end behavioral tracking
- **Legal obligation**: regulatory, compliance, or data-protection obligations

---



## 6. Cookies and Similar Technologies

When you use the App within Shopline admin or our related web pages, we may use cookies, pixels, local storage, or similar technologies to maintain sessions, save preferences, authenticate and secure sessions, and record errors and performance.

The front-end tracking script reads the **sl_utm** cookie set by Shopline to obtain UTM attribution information, and uses an anonymous **visitor_id** stored in local storage or a first-party cookie to associate behavioral events within a session. No cross-site tracking or third-party advertising cookies are used. You can manage cookies in your browser; disabling some cookies may affect certain features.

---



## 7. How We Share Information

We do not sell merchant data or merchant customer data.

- **Service providers**: we may share necessary data with providers such as Shopline and cloud/hosting/database/CDN/monitoring/logging/email vendors
- **At your direction**: data retrieved from Shopline APIs and front-end behavioral events are used solely to generate the UTM reports displayed within the App
- **Legal or security needs**: to comply with law, court orders, regulators, or law enforcement; to protect rights and safety; to prevent fraud, abuse, or unauthorized access
- **Corporate transactions**: in mergers, acquisitions, restructurings, asset sales, financing, or similar events, data may transfer as part of the transaction; recipients must continue to handle data lawfully

---



## 8. Data Retention

We follow a "minimum necessary, retain as needed" approach. After uninstalling the App or terminating service, non-essential data may be deleted or anonymized within 90 days; data required for audit or compliance may be retained longer.

Front-end behavioral event data (product detail views, session duration, browsing depth) collected via the tracking script is retained in aggregated form only; raw event records are deleted after aggregation is complete, typically within 7 days of collection.

UTM report logs and aggregated metrics may be retained as needed for consistency and dispute handling.

---



## 9. International Transfers

Information may be transferred to, stored in, or processed in countries or regions outside your jurisdiction (for example: regions where our hosting providers and Shopline process data). We apply reasonable safeguards as required by applicable law.

---



## 10. Security

We use HTTPS/TLS, access controls, authentication, logging, backups, and disaster recovery. OAuth / access tokens are stored on the server only and never exposed to the client. The front-end tracking script transmits data over HTTPS only. No internet transmission or electronic storage is ever fully secure.

---



## 11. Your Rights

Where applicable law grants rights, you or merchant customers may have access, rectification, erasure, restriction, withdrawal of consent, portability, or complaint to a regulator. Merchants may contact us at [apps@silksoftware.com](mailto:apps@silksoftware.com); end consumers should usually contact the merchant first.

---



## 12. Uninstall and Deletion

When you uninstall the App, terminate service, or request deletion, we will handle requests in line with applicable law and platform requirements. Upon uninstall, the front-end tracking script will no longer be injected into the storefront, and new behavioral events will cease to be collected. For deletion requests, contact [apps@silksoftware.com](mailto:apps@silksoftware.com) with subject line: **Data Deletion Request / 数据删除请求**.

---



## 13. Third-Party Sites and Services

The App relies on Shopline APIs to retrieve conversion funnel and sales data, and may link to other third-party sites or services; each has its own privacy policy. Please review their notices before use.

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