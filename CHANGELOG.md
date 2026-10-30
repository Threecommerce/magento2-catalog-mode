# Changelog

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
