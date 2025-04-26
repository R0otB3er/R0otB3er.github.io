---
title: "UH Form Management System"
excerpt: "Role-based web application for digital form processing at University of Houston"
collection: portfolio
---

**Technologies**: Python, Flask, SQL (Azure), HTML/CSS  
**Role**: Frontend Development & System Debugging  
**Links**: [Video](https://youtu.be/PkIRe9yX56g) [Repository](https://github.com/gnguyen2/Chilliwack)

A secure form management system designed to streamline document workflows across University of Houston departments. The application features:

### Tiered Access Control
- **Basic Users**:  
  - Digitally sign and submit department-specific forms  
  - Track submission status (pending/approved/rejected)  
  - View/download PDF versions of completed forms  

- **Privileged Users (Department-Level)**:  
  - Review and approve/reject submissions within their department    

- **Administrators**:  
  - Manage user roles and permissions across all departments  
  - "Master Department" admins gain system-wide visibility  
  - Monitor all form activity and system health  

### Technical Implementation
- **Frontend**: Responsive HTML/CSS interfaces with dynamic form rendering  
- **Backend**: Flask DB Management, utilizing Microsoft API for login authentication  
- **Data Layer**: Azure-hosted SQL database storing: 
  - Form templates/submissions (PDF generation)  
  - Departmental relationships  

**Key Features**:
- Departmental isolation with master override capability  
- PDF generation/download for all form types  
- Audit-compliant record keeping  
- Azure-based horizontal scalability  
