---
title: "Zoo Managment Website"
excerpt: "Role-based web application for a fictional Zoo"
collection: portfolio
---

**Technologies**: React, Node.js, Express, SQL (PostgreSQL), HTML/CSS, Azure <br>
**Role**: Full-Stack Development, Team Leader  <br>
**Links**: [Frontend Repository](https://github.com/R0otB3er/frontend) | [Backend Repository](https://github.com/tif-car/backend) <br>

A comprehensive zoo management and visitor engagement web application for a fictional Zoo. The application features:

### Single Login and Tiered Access & Interactions

* **Zoo Visitors**:
    * Browse a searchable, interactive catalog of animal profiles and attractions
    * Purchase tickets and merchandise and select visitation dates
    * Access dynamic daily schedules for keeper talks and animal feedings


* **Staff & Keepers**:
    * Update animal profiles, dietary requirements, and health statuses
    * Manage specific exhibit information, maintenance and daily event times


* **Administrators**:
    * Monitor daily ticket sales and overall park capacity
    * Manage staff roles and system-wide access permissions
    * Oversee backend database records and generate visitor and attraction reports



### Technical Implementation

* **Frontend**: Responsive React-based Single Page Application (SPA) with dynamic state management for the ticketing and cart flows
* **Backend**: Node.js and Express RESTful API handling secure authentication, ticket validation, and business logic
* **Data Layer**: Relational database storing:
    * Animal details, origins, and exhibit coordinates
    * User accounts, staff roles, and transaction history

**Key Features**:
* Decoupled frontend/backend architecture for independent scaling
* Secure Role-Based Access Control (RBAC) for staff and admins
* Digital ticketing and checkout simulation
* Cross-Origin Resource Sharing (CORS) configured for secure cross-server data fetching