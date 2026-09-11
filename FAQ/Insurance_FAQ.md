         
##                Insurance Plugin FAQ

Q1: What does the Insurance Plugin do?

A: It lets Shopline merchants offer buyers an opt-in shipping insurance at checkout. When a buyer selects insurance, the merchant is charged a premium from their pre-funded wallet; upon fulfillment, each package is automatically insured with Cathay Insurance. Merchants can then file claims, track payouts, and receive monthly commissions — all within the plugin.

---

Q2: How do I get started?

A: Install the plugin from the Shopline App Market → complete the first-entry service agreement → ask the platform operator to enable **Insurance permission** for your store and configure a charge plan → fill in **Insured Certificate** information in Settings → General → add at least one **Payout Account** → top up your **Wallet** → confirm all six items in Settings → Connections → **Setup Checklist** show green. Once the checklist is clear, insurance activates automatically on new orders.

---

Q3: What is the Wallet and how does charging work?

A: The **Wallet** is a prepaid balance account (in USD) that funds insurance premiums. When a buyer selects insurance and the order is fulfilled, the system deducts the calculated premium from your wallet balance automatically. The premium equals **max(fixed amount, order amount × percentage rate, minimum charge)** — whichever is highest among the three values configured by the platform operator. If your wallet balance is insufficient at the time of shipment, the package enters a **Pending** queue and is insured automatically once you top up; no manual re-submission is needed.

---

Q4: What are the wallet top-up options and how does payment work?

A: Top-up is done in fixed increments: **$100 / $300 / $500 / $1,000 / $3,000 / $5,000 / $10,000 USD**. Click **Recharge** in the Wallet page → select an amount → complete payment via Shopline's payment flow using your store's bound payment method. Funds are credited to your wallet balance immediately after Shopline confirms payment. The wallet balance is held on the platform and used to settle premiums with Cathay Insurance on your behalf.

---

Q5: What is "Auto cancel" and when does it trigger?

A: **Auto cancel** is a setting (configured by the platform operator) that automatically cancels a policy and refunds the premium to your wallet if a package has not been fulfilled within **30 days** of the order being insured. It does **not** apply to packages that have already been shipped. The refunded amount returns to your wallet balance; any associated commission credit is clawed back at the time of refund.

---

Q6: How do I file an insurance claim?

A: Go to **Policies → Issued policies** → find the package you want to claim → click **Claim** (visible only when the Tracking column shows **Has Tracking**) → select a payout account → submit supporting evidence. The claim status changes to **SUBMITTED** and enters Cathay Insurance's review process. If rejected, you may submit **one appeal** on the same policy. If the appeal is also rejected, no further appeals are permitted; contact support via the platform's support email for further assistance.

---

Q7: What happens if a claim is rejected with a specific reason code?

A: If Cathay Insurance rejects a claim for a reason listed in the platform's **auto-refund reject reasons** configuration, the system automatically **cancels the policy and refunds the premium** to your wallet. If the rejection reason is not in that list, the policy remains cancelled without an automatic refund; you may appeal once. Any commission that was credited for the original policy is clawed back upon cancellation regardless of the rejection reason.

---

Q8: What are Commissions and when are they paid?

A: **Commissions** are a percentage of the Cathay Insurance actual premium (not the amount charged to you) that the platform returns to your wallet each month. The commission rate is set per store by the platform operator and may be updated; a rate change takes effect the following calendar day and does not affect policies already settled. Commissions are calculated on the **5th of each month** for all paid policies from the prior month and credited to your wallet automatically. If a policy is later refunded after commission has been credited, the commission is **clawed back** (deducted from your wallet balance).


---

Q9: What should I do if the Setup Checklist shows a red item after installation?

A: Each item maps to a specific fix: **Service agreement not confirmed** → re-open the plugin and complete the confirmation modal. **Charge plan not configured** or **Insurance permission not enabled** → contact the platform operator to configure your store in the admin console. **Insured certificate missing** → fill in Settings → General → Insured Certificate. **Insurance product not bound** → contact technical support. **Webhooks not subscribed** → click **Resubscribe** in Settings → Connections. All six items must be green before automatic insurance will function.