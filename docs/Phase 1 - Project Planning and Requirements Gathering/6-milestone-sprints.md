# Milestone and Sprint Plan

## Key Milestones

### **Milestone 1: Event and Dish Management (Backend)**
- **Goal**: Build the core backend functionality for managing events and dishes.
- **Features**:
  - CRUD operations for events and dishes.
  - GraphQL setup and resolvers for `Event`, `Dish`, and `User`.
  - Relationships: `Event` ↔ `Dish` via `EventDishes`.
- **Estimated Time**: 7-8 days.

---

### **Milestone 2: Order Creation and Updates (Backend and Frontend)**
- **Goal**: Implement order functionality, including placing, updating, and managing orders.
- **Features**:
  - **Backend**:
    - GraphQL resolvers for `Order` and `OrderItems`.
    - Validations for quantities, deadlines, and payments.
  - **Frontend**:
    - Pages for placing and managing orders.
    - Integration of Apollo Client for GraphQL.
- **Estimated Time**: 10-12 days.

---

### **Milestone 3: Reports and Financial Summaries**
- **Goal**: Develop reporting and financial summary functionalities.
- **Features**:
  - **Backend**:
    - GraphQL resolvers for reports (e.g., total sales, loans, net profit).
  - **Frontend**:
    - Pages for viewing reports with dynamic charts (e.g., Chart.js or Recharts).
- **Estimated Time**: 5-6 days.

---

## Sprint Plan

### **Sprint 1: Requirements Gathering and Wireframes (2-3 Days)**  
- **Status**: In Progress
- **Deliverables**:
  - Finalized requirements document.
  - Completed wireframes for all core features.
  - Approval of the ERD and technical architecture.
- **Tasks**:
  - Review requirements and refine any gaps.
  - Finalize the technical architecture and data relationships.
  - Build wireframes for all pages.

---

### **Sprint 2: Backend for Event and Dish Management (7-8 Days)**  
- **Deliverables**:
  - Rails API setup with GraphQL.
  - CRUD for `User`, `Event`, `Dish`, and `EventDishes`.
  - TDD setup using RSpec and FactoryBot.
- **Tasks**:
  - Create models and relationships based on the ERD.
  - Implement GraphQL resolvers for event and dish management.
  - Write RSpec tests for all backend functionality.

---

### **Sprint 3: Frontend for Event and Dish Management (5-6 Days)**  
- **Deliverables**:
  - React app setup with TypeScript and Apollo Client.
  - Pages for event and dish management.
  - Basic UI with placeholders for other features.
- **Tasks**:
  - Create the React app with TypeScript.
  - Build pages for managing events and dishes.
  - Connect to the backend using Apollo Client.

---

### **Sprint 4: Order Functionality (Backend and Frontend) (10-12 Days)**  
- **Deliverables**:
  - Backend: Order and payment functionality with GraphQL.
  - Frontend: Pages for placing and managing orders.
  - Validations for order deadlines and payments.
- **Tasks**:
  - Add GraphQL resolvers for `Order` and `OrderItems`.
  - Create pages for placing and editing orders.
  - Implement dynamic price calculations in the frontend.

---

### **Sprint 5: Reports and Financial Summaries (5-6 Days)**  
- **Deliverables**:
  - Backend: GraphQL endpoints for reports.
  - Frontend: Charts and financial summaries.
  - UAT Deployment ready.
- **Tasks**:
  - Build backend resolvers for financial summaries.
  - Create frontend pages for viewing reports.
  - Deploy to UAT and test end-to-end functionality.

---

## Overall Timeline

| **Week**  | **Sprint**                          | **Key Deliverables**                   |
|-----------|-------------------------------------|----------------------------------------|
| Week 1    | Sprint 1                            | Requirements, wireframes, architecture |
| Week 1-2  | Sprint 2                            | Backend for event/dish management      |
| Week 2    | Sprint 3                            | Frontend for event/dish management     |
| Week 2-3  | Sprint 4                            | Order functionality (backend + frontend) |
| Week 3-4  | Sprint 5                            | Reports, financial summaries, UAT ready |

---

## Current Progress: Sprint 1 (12/11/2024)
- **Focus**: Completing wireframes and finalizing requirements.
- **Status**: Ongoing.