# Authorization & Access Management

**Project:** Automated Employee Onboarding & Offboarding System  
**Phase:** Security & Permission Management

---

## Overview

Role-Based Access Control mechanisms protect confidential employee lifecycle information from unauthorized access. ServiceNow automatically generates four foundational Access Control List rules when custom tables are created. This project leverages these default ACLs with customized configurations to establish comprehensive access restrictions.

Access Control List configurations govern **view, modify, create, and delete** operations on Employee Lifecycle records. Access grants follow user role assignments, ensuring only authorized stakeholders can view or modify specific information.

---

---

## Access Control Architecture

### Default ACL Framework

When the **Employee Lifecycle** custom table gets created, ServiceNow automatically generates these ACL rules:

- Create ACL
- Read ACL
- Write ACL
- Delete ACL

These ACLs form the foundation for record-level permission management.

---

---

## Role-Specific Access Rules

Access Control Lists restrict data access based on user role assignments and departmental responsibilities.

### HR Personnel Access

- Can generate new onboarding and offboarding request submissions
- Can view and modify employee lifecycle records

### Management Personnel Access

- Can view employee lifecycle records related to their team assignments
- Can authorize (approve/deny) lifecycle request submissions

### IT Department Access

- Can access system-related task assignments and account creation activities
- Possess limited read access to lifecycle records

### Facilities Department Access

- Can view facility-related task assignments and resource allocation activities

### Security Department Access

- Can manage access permissions and administer security protocols

---

---

## Configuration Implementation

1. Access **System Security → Access Control (ACL)** menu
2. Click **New** to create or adjust access control rules
3. Select the target **Employee Lifecycle table**
4. Choose the operation type to configure:
   - Read capability
   - Write capability
   - Create capability
   - Delete capability
5. Assign the required **role assignments** to control access
6. Finalize and verify the ACL configuration

---

## Projected Outcomes

- Employee lifecycle records remain protected from unauthorized access
- Sensitive employee information receives appropriate confidentiality protections
- Access restrictions follow job roles and departmental boundaries
- Overall platform security posture and compliance status improve

---
