# 🏪 Marketplace Platform – Store & Supporter Discovery System

A feature-rich multi-role marketplace system built using **ASP.NET Core** and **Angular**, enabling customers to discover local or delivery-based stores, browse and order products, and manage payments, while allowing store owners to operate digital storefronts with full automation and zero admin intervention.

---

## 🚀 Features

### 🧑‍💼 User Account & Onboarding
- New users can register using a **secondary phone number or email**.
- Logged-in users see a **personalized homepage** with:
  - Service summaries
  - Notifications
  - Store filters based on **location** and **availability**

---

### 🛒 Customer Experience

#### 🗺️ Store/Supporter Discovery
- Filter stores by:
  - **Physical proximity** (with "Nearby" toggle)
  - **Store category** (e.g., equestrian, livestock)
- Standalone store interfaces with **name**, **photo**, and **address**

#### 🛍️ Product Browsing & Ordering
- Filter products by:
  - **Price**, **size**, **color**, **brand**
- Add **"Arab products"** to cart
- Choose delivery providers filtered by:
  - **System-nominated matches** (e.g., sheep require livestock delivery)
  - **Service coverage areas**

#### 💳 Payment & Fees
- Pay at checkout when "exiting the mall"
- Transparent breakdown of:
  - Product costs
  - Delivery charges
  - Wasted costs (e.g., cancellation fees)
- **Real-time order/delivery notifications**

---

### 🏪 Store Owner Management

#### Store Setup
- Create a store with:
  - Name, photo, address
  - Delivery areas
- Store appears as a **standalone business**

#### Product & Order Operations
- Dashboard to manage inventory (add/edit/remove)
- Instant alerts for:
  - Product or **lesson** orders
- Subject to **3 types of late fees**:
  - Dispatch delays
  - Delivery delays
  - Response delays

#### Dispute Resolution
- **Customers and store owners** can file disputes
- Entirely handled by the **automated system**

---

### ⚙️ System Automation
- **Auto-nominated delivery** based on product type
- Late fees are applied **automatically** without admin
- **Payments handled** at checkout
- No admin interface – all issues and fees are **system-managed**

---

## 🧭 Key Workflows

### 🔁 Customer Journey
`Login → Filter stores → Browse products → Add to cart → Select delivery → Pay upon exit`

### 🛍️ Store Owner Journey
`Create store → Add products → Get order alerts → Fulfill orders → Handle complaints`

### ⚖️ Complaint Workflow
`User/store files complaint → System notifies counterparty → Automated resolution`

---

## 🛠 Tech Stack

| Layer                | Technology |
|---------------------|------------|
| Backend             | ASP.NET Core  |
| Frontend            | Angular |
| Database            | TransactSQL |
| Caching             | Redis |
| ORM                 | Entity Framework Core |
| API Testing         | Swagger |
| State Management    | CQRS with MediatR |
| Mapping             | AutoMapper |
| Authentication      | ASP.NET Identity |
| Real-time Messaging | SignalR |
| Deployment          | CI/CD Pipelines |
| Architecture        | Clean Architecture + CQRS/MediatR |

---

## 🧱 Architecture

The system is structured using **Clean Architecture** principles with a **CQRS** pattern powered by **MediatR**, ensuring:

- **Separation of concerns**
- **Scalability and maintainability**
- **Modular testing and extensibility**

> The backend communicates with the Angular frontend via RESTful APIs, supports real-time messaging through SignalR, and uses Redis for performance-boosting caching.

---

## 🧪 API Documentation

The project includes **interactive API documentation** via Swagger. After running the backend:

```bash
https://localhost:<port>/swagger
````

Explore endpoints for user registration, store/product management, orders, payments, and disputes.

---

## 🚧 Setup & Contribution

1. **Clone the repository**
2. Set up both projects:

   * `.NET Core backend`
   * `Angular frontend`
3. Configure:

   * TransactSQL connection strings
   * Redis and Identity setup
4. Run migrations and seed data 
5. Launch the backend, then the Angular app

> 💡 Contributions welcome – please fork and submit a pull request.

---

## 📬 Contact

If you have any questions, feel free to reach out or open an issue.

---
