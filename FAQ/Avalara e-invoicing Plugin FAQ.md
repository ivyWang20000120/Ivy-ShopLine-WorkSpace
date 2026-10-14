<h1 align="center">Avalara e-invoicing Plugin FAQ</h1>

Q1: What does the Avalara e-invoicing Plugin do?

A: It helps SHOPLINE merchants collect invoice details at checkout, apply market-specific rules, and manage electronic invoices through Avalara. Where configured, merchants can also manage e-waybills through the selected solution, review documents by order and fulfillment, download available PDFs, track processing history, and submit invoice-change requests.

Q2: What must be configured before the App can issue documents?

A: Connect Avalara in **Settings → Avalara**, sync the applicable rules in **Market Rules**, complete the seller's required compliance details in **Market Config**, and confirm the market's trigger and invoice settings. For markets using an independent e-waybill, select a solution and make every required item in the **E-waybill Config** readiness checklist ready before applying the preset.

Q3: What is the difference between automatic and manual invoicing?

A: **Automatic invoicing** submits eligible workflows to Avalara under the configured market rules. With automatic invoicing disabled, the App is in **manual invoicing** mode and merchants follow their offline invoicing plan; changing modes does not automatically submit historical orders. To process historical records after switching back to automatic, preview eligible records first, then queue selected records or a batch.

Q4: When are forward and reverse invoices triggered?

A: Triggers are configured by country in **Market Rules** and may use events such as **Order paid**, **Each fulfillment**, or **Refund completed**. The active rule determines the timing for that market. A refund or cancellation creates a reverse-document workflow only when the applicable rule and market configuration call for it.

Q5: How does Turkey's e-Arşiv fallback work?

A: When **Auto e-Arşiv fallback** is enabled for Turkey, a buyer who requests e-Fatura but is not registered in the applicable GİB/Avalara directory may be routed to e-Arşiv instead of having the invoice attempt fail. This fallback is conditional on the configured market and buyer eligibility; it is not a general fallback for other countries.

Q6: Why can one order show several documents, and how do I find them?

A: Documents are grouped by **fulfillment**, so each shipment batch can have its own invoice attempt or waybill. In **Documents**, search by order number, document number, or customer and filter by status, type, source, market, or date; open the order to review each fulfillment's details and select **Download PDF** on an available document. Enable **Include archived failed attempts** to include failed attempts in the record view.

Q7: Why is an e-waybill not ready, and what if a payment method or carrier is unmapped?

A: Check the **E-waybill Config** readiness preview for missing global enablement, seller VKN, sender alias, number series, default carrier mapping, trigger, or required contract status; correct the configuration, preview again, and apply the selected preset. For a fulfillment, use **Recheck e-waybill eligibility** before retrying. An unmapped payment method retains the original SHOPLINE field and uses UBL payment-means code **30**; an unmatched carrier uses the **__default__** row, which should contain the intended default legal name and tax number.

Q8: Can I correct an issued invoice, and who approves the change?

A: A user with **Create invoice modification requests** permission can choose **Request modification** or submit from **Modify Invoice**, providing a proposed profile and reason. A separate user with **Approve or reject modification requests** permission reviews the request; assign these permissions to appropriate requester and reviewer roles. In the documented UAT environment, approval records the decision but does not execute the Avalara-side credit-and-reissue flow.

Q9: What does the product SN/IMEI option do?

A: When **Add product SN/IMEI to invoice product names** is enabled, available serial-number or IMEI data is appended to product names on newly generated automatic forward invoices. The generated name is fixed at creation and does not change when the Avalara-side record or PDF is later viewed.

Q10: How do email links and activity history work?

A: When **Plugin email notification** is enabled, Settings can generate SHOPLINE email-template HTML with an invoice PDF link; when disabled, the generated HTML contains an informational message without the link. Copy the generated HTML into SHOPLINE's email editor for the change to take effect. Review order and document events in the **Complete order timeline**, or search **Operation Logs** by order, actor, action, and date; modification requests also have their own audit timeline.
