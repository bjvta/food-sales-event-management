## User Roles and Permissions

### Admin

- Create, update, and delete events.
- Add, update, and delete dishes for events.
- Manage customer orders (view, edit, cancel).
- Track and update dish availability and deliveries.
- View financial reports for events (income, expenses, loans).

### Customer

- Browse events and view available dishes.
- Place orders for dishes.
- Edit orders (up to 1 day before the event).
- Pay for their orders.

---

## User Stories

### Admin Stories

1. As an Admin, I want to create and manage events to sell food for fundraising.
2. As an Admin, I want to update dish availability and track deliveries during the event.
3. As an Admin, I want to view financial reports after the event.
4. As an Admin, I want to manage customer orders to ensure all transactions are tracked.

### Customer Stories

1. As a Customer, I want to browse events and view dishes to decide what to order.
2. As a Customer, I want to place orders for dishes easily.
3. As a Customer, I want to edit my orders up to 1 day before the event.
4. As a Customer, I want to make payments for my orders conveniently.

---

## Validation Rules

### Dish Price

- Must be a positive number.
- Cannot exceed a realistic value (e.g., no dish priced above 1,000 BOB).

### Quantity

- Must be a whole number greater than 0.
- Cannot exceed the available count for the dish.

### Loan Amount

- Must be a positive decimal value.
- Cannot exceed a specified maximum (e.g., budget for an event).

### Order Edit Deadline

- Allow edits to orders only up to 1 day before the event's date.

---

## Glossary

### Dish

- A food item prepared for sale during an event. Each dish has attributes such as `name`, `price`, `available_count`, and `delivered_count`.

### Order

- A request placed by a customer or admin to reserve specific dishes. Orders are associated with a customer and an event.

### Event

- The occasion where the food sale takes place. An event includes details like the date, location, purpose (e.g., charity or building project), and associated dishes.

### Loan

- Funds borrowed to cover the upfront costs of preparing for an event, such as purchasing ingredients. Loans are repaid using proceeds from the event's earnings.

---

## Prioritized List of User Stories and Validation Rules

| **User Role** | **User Story** | **Validation Rules** |
| --- | --- | --- |
| Admin | Create and manage events. | Event `name` and `date` are required. |
|  | Add and update dishes. | Dish `name` and `price` must be valid. |
|  | View financial reports. | Reports must calculate `total_income`, `loans_paid`, and `net_profit`. |
| Customer | Browse events and dishes. | Event must have active status for browsing. |
|  | Place orders for dishes. | `quantity` must not exceed `available_count`. |
|  | Edit orders up to 1 day before the event. | Ensure `event_date - current_date >= 1`. |
|  | Pay for orders. | `amount` must match the total price. |