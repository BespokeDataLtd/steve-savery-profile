## 💳 Harley Therapy – Automated Billing System with Braintree (2019–2024)

**Role:** Solution Designer & Lead Developer  
**Tech:** FileMaker Pro, Braintree, MySQL (firewalled), MJML email templates, payment tokenisation

- Replaced a **manual, fragmented billing workflow** that relied on PayPal, BACS, and therapist honesty to track cash payments, cancellations, and missed appointments.
- Introduced full **automated billing**, integrating FileMaker with **Braintree Payments** via secure tokenisation and custom MySQL intermediary for sensitive data isolation.
- Built logic to:
  - Generate secure email payment requests with MJML-formatted HTML templates.
  - Allow clients to choose an existing payment method or register a new one (card or PayPal).
  - Automatically trigger payments **48 hours before a session**, respecting the cancellation policy.
  - Notify clients if payment failed and optionally cancel the session if unresolved.
- Enabled **prepayment for sessions**, eliminating the need to chase payment after sessions took place.
- Automated therapist payouts by deducting platform fees and therapist-specific charges upfront — **no more invoicing or chasing therapists for room/admin fees**.
- Protected payment token data using a **read/write-separated MySQL database**, firewalled to accept:
  - `Read/write` only from Braintree's servers
  - `Read-only` access from the public payment front-end
  - No direct access from FileMaker or the general web
- Ensured security and resilience — system **remains breach-free** to this day.

---

### 🧩 Business Impact

- Reduced therapist and client debt-chasing by **~90%**
- Freed up significant administration time for business growth tasks
- Eliminated billing discrepancies and human error
- Supported growth in online bookings with fully automated, secure transactions