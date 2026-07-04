# User Interaction Workflow

**Project:** Automated Employee Onboarding & Offboarding System  
**Phase:** User Navigation & Interaction Patterns

---

## Overview

This documentation illustrates how end users navigate the ServiceNow portal interface to originate lifecycle requests. The user journey encompasses portal access, catalog item discovery, form completion, and automated request initiation. Upon submission, users receive tracking identifiers and confirmation notifications via email.

---

## User Journey Steps

### Phase 1: Authentication

- Authenticate to your **ServiceNow Personal Developer Instance (PDI)**

---

### Phase 2: Instance URL Retrieval

- Record the instance domain URL from your current session

*Example format:*

```
https://dev190678.service-now.com
```

---

### Phase 3: Portal Access

- Enter the instance URL into browser navigation
- Append **/sp** path segment to instance domain

*Sample URL format:*

```
https://dev190678.service-now.com/sp
```

This URL will launch the **Service Portal** interface.

---

### Phase 4: Catalog Discovery

- Use the portal search functionality to locate **Network Requests** or the specific catalog request item

---

### Phase 5: Form Completion

- Open the request form display
- Supply all mandatory information fields:
  - Employee Full Name
  - Employee Identification Number
  - Organizational Department Assignment
  - Request Category (Onboarding / Offboarding)
  - Commencement Date or Departure Date

---

### Phase 6: Request Submission

- Click **Submit** after completing all mandatory fields

---

### Phase 7: Request Generation

- System generates **new request record** in the platform
- Request receives **unique identifier number** for reference and tracking

---

### Phase 8: Confirmation Communication

- Submitter receives **confirmation email notification** confirming successful request submission
- Request enters **automated approval and workflow processing stages**

---

## Projected Outcomes

- Users can efficiently originate lifecycle requests via the Service Portal
- Request submissions automatically generate tracking identifiers
- Submitters receive email confirmations for tracking and reference
- Workflow orchestration launches automatically upon successful submission

---

