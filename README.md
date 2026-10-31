# SubNova – Subscription Management System

One platform to run plans, subscriptions and recurring billing for a subscription business (Brightloop Software case study).

## How to run
No install needed. Open `index.html` in Chrome or Edge.

## Demo logins
| Role | Email | Password |
|---|---|---|
| Admin | admin@brightloop.com | Admin@12345 |
| Staff | staff@brightloop.com | Staff@12345 |
| Customer | Click "Create account" | Any password with 9+ characters, upper, lower and a special character |

## Features
- **Accounts and roles:** unique email, password rules, reset link, admin / staff / customer portal. Only the admin can add staff.
- **Catalog:** products with variants (e.g. Brand: Odoo +560), tax rule per product, plans with daily / weekly / monthly / yearly billing, minimum quantity, availability dates, and per-plan switches for auto-close, close early, pause and renew.
- **Subscriptions:** quotation templates, numbered subscriptions, Draft → Quotation → Confirmed → Active → Closed. Customers can subscribe from the portal.
- **Billing:** one-click billing run creates invoices from subscriptions with tax and discounts filled in. Each period is billed only once. Invoices go Draft → Confirmed → Paid, with cancel, send and print.
- **Discounts:** admin-only fixed or percentage rules with minimums, dates and usage limits, for products or whole subscriptions. Applied automatically on the next invoice.
- **Payments:** recorded by method, amount, date and note against an invoice. Outstanding and overdue invoices are flagged.
- **Finance dashboard:** active subscriptions, monthly recurring revenue, revenue collected, outstanding, overdue invoices, date filters.
- **Plan fee:** the plan price is added as a fee line on every invoice, next to the product lines.
- **Admin tools:** edit and delete products, plans, taxes and discounts (items in use are protected). CSV export of invoices and subscriptions. Revenue chart. Overdue reminders.
- **Customer portal:** customers subscribe, accept quotes, view invoices and pay them online (simulated).
- **Auto-close:** plans set to close on their own close once the expiry passes and all periods are billed.
- **Performance:** admin can load 3,000 demo subscriptions; pages build in well under 2 seconds (time shown at the bottom of each page).

## Tech
Single-file HTML, CSS and vanilla JavaScript. Data is stored in the browser (localStorage).

## Limitations and next steps
- Move storage to a backend (Node or Django) with a database and hashed passwords.
- Send real emails for password reset and invoices.
- Real payment gateway integration.
- Hash passwords and add server-side permission checks.
