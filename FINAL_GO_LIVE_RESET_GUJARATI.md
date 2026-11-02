# Final Go-Live Reset — Demo Order Cleanup

આ update માં Admin Panel / Utilities હેઠળ `Final Go-Live Reset` tab ઉમેર્યું છે.

## Reset શું delete કરે છે?
- `order_dispatches` — તમામ dispatched entries
- `order_size_cancellations` — તમામ cancellation entries
- `order_item_sizes` — order ની size/quantity rows
- `order_items` — order ની SKU rows
- `orders` — બધા order headers

## શું સુરક્ષિત રહે છે?
- `parties` — Party Master
- `agents` — Agent Master
- `sku_master` — Item Master / SKU
- `users` — Admin, Member, Staff અને Agent login accounts

Reset ફક્ત Main Admin કરી શકે છે. પહેલાં Full Backup ZIP download કરવો, પછી exact phrase `DELETE ALL ORDERS` લખવું અને confirmation checkbox tick કરવું જરૂરી છે.

બધા orders delete થયા પછી નવા Order Number માટે fallback 2100 રાખ્યો છે; તેથી નવો Order Number 2101 થશે. Existing orders હોય તો numbering MAX(order_no)+1 પ્રમાણે આગળ વધશે.

**મહત્વપૂર્ણ:** Live database ના records app code upload કરતાં જ આપમેળે delete થતા નથી. Admin એ deployment પછી Final Go-Live Reset tab માંથી એકવાર આ action ચલાવવો પડશે.
