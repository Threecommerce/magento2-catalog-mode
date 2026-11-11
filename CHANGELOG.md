# Changelog

## [1.1.0] - 2026-11-11

- Quote expiry: *Valid Until* date on each request, set automatically when the status becomes *Quote Sent*
  (new setting *Quote Validity (Days)*, default 30) and editable by hand; hourly cron sets the new *Expired*
  status after that date, with an optional email to the customer. The date is shown in the admin, in the
  grid, in *My Quote Requests* and in the update email.
- Response time: the first reply of the store (status change or message to the customer) is recorded and
  shown on the request with the elapsed time.
- Quote to order: *Order #* field on the request (link to the order when it exists) and new
  *Converted to Order* status, set automatically when an order number is entered.
- KPI table above the requests grid: requests received, awaiting first reply, average first reply time,
  quotes sent, converted to orders, quote-to-order rate and expired quotes (30 / 90 days, all time).
- New grid columns: *Valid Until*, *Order #*, *First Reply* (hidden by default).

## 1.0.2 - 2026-10-30

- Metadata: license in `composer.json` is now `proprietary` (commercial module), no functional change.

## 1.0.1 - 2026-10-26

- Fix: the "View" action column of the requests grid was empty (custom column did not write into the grid data).

## 1.0.0 - 2026-10-19

- First Threecommerce release (`Threecommerce_CatalogMode`, `threecommerce/m2-catalog-mode`), moved from `MageOS_CatalogMode`: namespace, ACL, tables (`tc_quote_request*`) and CSS classes (`tc-*`) renamed, configuration paths unchanged.

## Earlier work - 2026-10-06 (as MageOS_CatalogMode, never released)

- Per store view catalog mode: purchasing off, catalog still browsable.
- Price display: show, recommended retail price (msrp) only, or hidden with a custom text.
- Optional restriction to selected customer groups.
- Quote request mode: cart stays available, the checkout sends a quote request instead of placing an order.
- Admin: Sales > Quote Requests grid, detail page, status changes and replies emailed to the customer.
- Customer account: "My Quote Requests" list and detail.
