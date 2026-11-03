# New Order Update

1. SKU Code / Particulars is now a direct text field. Typing an exact SKU code and pressing Tab (or moving focus) triggers Streamlit rerun and resolves the matching Item Master SKU and WSP Rate. Unknown SKU codes are not allowed to save.
2. Discount is entered as a percentage (for example 5, 10, 15). The value is stored in the existing `order_items.discount` column as a percentage. Discount is validated between 0 and 100.
3. Row amount is calculated as `WSP Rate × Quantity × (1 - Discount / 100)`. PDF item amounts, order history amounts, and report amount calculations use the percentage discount.
4. Live Total Qty and Total Amount cards appear above Packaging. Total Amount is calculated after each row's percentage discount.

No database schema change is required. Existing discount values will now be interpreted as percentages, so this update is intended for the clean go-live order set after the demo order reset. Take a database backup before deploying.
