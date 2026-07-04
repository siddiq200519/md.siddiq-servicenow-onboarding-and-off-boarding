# Data Transfer & Storage Management

**Project:** Automated Employee Onboarding & Offboarding System  
**Phase:** Data Transfer & Automation Implementation

---

## Overview

The system manages request information by persisting onboarding and offboarding details within a custom **Employee Lifecycle** data table infrastructure. This table structure maintains comprehensive records containing personnel details, request specifications, and processing status.

Service Portal form inputs from the **Onboard/Offboard Employee** catalog entry automatically transfer to **u_employee_lifecycle** table fields through Flow Designer workflow automation.

---

---

## Data Persistence Architecture

Employee lifecycle information persists in the **Employee Lifecycle custom table** with connections to user profiles and catalog input variables.

### Data Elements Captured

- Employee Identification
- Employee Full Name
- Organizational Department
- Manager/Supervisor Assignment
- Request Classification (Onboarding / Offboarding)
- Commencement Date
- Departure Date
- Assigned Equipment & Assets
- System Access Revocation Information
- Request Processing Status

This approach enables comprehensive tracking and analytics for lifecycle activities.

---

---

## Automated Variable Transfer

Workflow automation captures service portal inputs from the **Onboard/Offboard Employee** catalog and automatically transfers them to **u_employee_lifecycle** table fields.

This mechanism ensures that every request submission automatically generates or updates a corresponding structured record.

---

## Implementation Procedure

### Step 1: Flow Engine Setup

- Access **Flow Designer** within ServiceNow
- Establish a new automation workflow for lifecycle requests

### Step 2: Trigger Configuration

- Configure trigger activation on **catalog item submission events**
- Specify the target as **Onboard/Offboard Employee** catalog item

### Step 3: Variable Extraction

- Integrate the **Get Catalog Variables** operation
- Extract submitted values including:
  - Employee Identification Number
  - Manager/Supervisor
  - Organizational Department
  - Commencement/Departure Dates
  - Equipment & Asset Requirements
  - System Access Parameters

### Step 4: Record Creation Logic

- Integrate the **Create/Update Record** operation
- Designate **Employee Lifecycle (u_employee_lifecycle)** as target table

### Step 5: Field Transfer Mapping

- Access the **Add Fields (+)** option
- Establish transfer mappings from catalog variables to table fields:
  - Employee ID → Employee ID field
  - Department → Department field  
  - Manager → Manager field
  - Commencement Date → Joining Date field
  - Departure Date → Exit Date field

---

## Projected Results

- Comprehensive storage organization for request submissions and lifecycle details
- Automatic generation or modification of structured records on submission
- Dependable tracking of employee lifecycle activities
- Enhanced reporting and workflow automation capabilities

---
