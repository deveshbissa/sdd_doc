graph TD;
    A[Users] -->|Browse, Order| B[E-Commerce System]
    B -->|Manage Payments| C[Payment Gateway]
    B -->|Check Stock| D[Inventory System]
    B -->|Send Orders| E[Shipping Provider]
    F[Admin] -->|Manage Products| B
