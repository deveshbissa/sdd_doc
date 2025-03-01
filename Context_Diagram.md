Context Diagram Description
The system interacts with:

Users – Browsing products, making purchases, and managing accounts.
Payment Gateway – Processing online transactions.
Inventory System – Managing stock levels and updating product availability.
Shipping Provider – Handling order deliveries.
Admin – Managing product listings, orders, and user accounts.

                      +----------------------+
                      |     Admin            |
                      |  (Manage Products)   |
                      +----------+-----------+
                                 |
                                 v
     +--------------------+    +-----------------+
     |  Users            |---->|  E-Commerce     |
     | (Browse, Order)   |     |  System         |
     +--------------------+    +-----------------+
                                 |      |       |
                                 v      v       v
   +-----------------+   +-----------------+   +-------------------+
   | Payment Gateway|<-->| Inventory System|<->| Shipping Provider |
   +-----------------+   +-----------------+   +-------------------+




graph TD;
    A[Users] -->|Browse, Order| B[E-Commerce System]
    B -->|Manage Payments| C[Payment Gateway]
    B -->|Check Stock| D[Inventory System]
    B -->|Send Orders| E[Shipping Provider]
    F[Admin] -->|Manage Products| B
