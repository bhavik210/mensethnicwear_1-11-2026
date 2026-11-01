SHUBHVASTRA — Item Master Required Fields Update

Item Master ma have aa 3 fields required che:
1. SKU Name (database ma existing sku_number field sathe mapped; order form ma SKU selection existing rite kaam karse)
2. SKU Under (navi database column)
3. Sale Rate

Add New SKU ane Edit SKU banne ma validation mukyu che. SKU Name ane SKU Under blank hoy to save nahi thay. Sale Rate number field required che (zero allowed, existing behavior pramane).

Existing SQLite/PostgreSQL database mate init_db() ma safe schema migration add kari che. Existing SKU records delete thata nathi; old records mate SKU Under blank default rahe che, ane nava/edit thata records mate required che. Existing order items na saved rates badlata nathi.

Update karta pela database backup lo. GitHub upload karta database file ne replace/delete na karsho.
