# Database Design

The database uses six main tables exported from the final MySQL dump.

| Table | Purpose | Key Fields |
|---|---|---|
| `category_table` | Stores product categories. | CategoryID, CategoryName |
| `inventory_table` | Tracks stock levels and inventory quantities. | InventoryID, Quantity_Sold, Quantity_on_Order, Current_Stock_Levels, ProductID(FK) |
| `product_table` | Stores product details and links products to suppliers/categories. | Product ID, Product Name, Description, Price, SupplierID(FK)... |
| `sales_table` | Stores sales transaction information. | Sales Transaction ID, Date, Time, Total Sales Amount |
| `sold_relationship_table` | Links sales transactions to products sold. | ProductID(FK), Sales_TransactionID(FK), Quantities |
| `supplier_table` | Stores supplier contact and address details. | SupplierID, Supplier_Name, Address, Contact_Number |

Primary and foreign keys were used to keep the data connected and reduce duplication. The design supports product management, supplier tracking, inventory control and sales reporting.

---

Inventory Management Database System  
Prepared by **Deacon George**  
Version 1.0  
