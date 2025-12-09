# 🐞 Bug Report Template – QA Defect Documentation

This folder contains a **standardized, industry-grade Bug Report Template** used for logging defects during manual, API, and database testing. The format follows best practices used in enterprise QA teams and aligns with Jira, Azure DevOps, and GitHub Issues workflows.

---

# 📄 Included File

| File Name                   | Description                                                                                                                |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------- |
| **BugReport_Template.xlsx** | Excel-based defect reporting template including severity, priority, steps, expected vs actual results, and workflow fields |

---

# 🎯 Purpose of This Template

This template ensures:

* Clear, consistent defect reporting
* Easy reproduction of bugs by developers
* Standardized format for interviews & QA assessments
* Strong documentation practices for your GitHub portfolio
* Tracking Severity, Priority, Root Cause, Fix Version, etc.

---

# 🧱 Bug Report Fields Explained

Each defect entry includes the following fields:

### **🔹 Bug ID**

Unique identifier (e.g., BUG-LOGIN-001).

### **🔹 Title**

Short, clear summary of the defect.

### **🔹 Module**

(Login / Signup / CRM Contacts / API / SQL)

### **🔹 Severity**

* **Blocker** – Testing halted
* **Critical** – Major functionality broken
* **Major** – Important feature not working
* **Minor** – Low impact functional issue
* **Trivial** – Cosmetic/UI issue

### **🔹 Priority**

* **High** – Must be fixed before release
* **Medium** – Fix in next sprint
* **Low** – Fix when time permits

### **🔹 Environment**

(QA / Staging / Production, browser version, OS)

### **🔹 Preconditions**

Setup required before executing the steps.

### **🔹 Steps to Reproduce**

Clear, numbered steps for developers to follow.

### **🔹 Expected Result**

Correct behavior as per requirements.

### **🔹 Actual Result**

What actually happened (the defect).

### **🔹 Attachment / Evidence**

* Screenshot
* Video
* Logs
* API response

### **🔹 Root Cause (Developer)**

Why the bug occurred.

### **🔹 Fix Version**

Release version containing the fix.

### **🔹 Status Workflow**

```
Open → In Progress → Fixed → Retest → Closed
                 ↘ Rejected / Deferred / Duplicate
```

### **🔹 Retest Result**

Pass/Fail result after developer fix.

---

# 📝 Example Bug Report

```
Bug ID: BUG-SIGNUP-009  
Title: OTP field accepts alphabetic characters  
Module: Signup  
Severity: Major  
Priority: High  
Environment: QA (Chrome 123)

Preconditions:
- User is on the Signup → OTP Verification screen.

Steps:
1. Enter mobile number and request OTP  
2. In the OTP input field, enter "AB12CD"  
3. Submit

Expected Result:
OTP field should restrict input to numeric digits only.

Actual Result:
OTP field accepts alphabetic characters.

Status: Open  
Attachments: screenshot_otp_issue.png
```

---


