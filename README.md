# Enterprise Power Platform Portfolio

Welcome to my Microsoft Power Platform repository. This portfolio showcases production-ready low-code applications, automated workflows, and relational data architecture designed to solve real-world enterprise operations challenges.

---

## 📱 Applications & Solutions Summary

### 1. Help Desk Management System
* **Folder Location:** [`/apps/HelpDeskSystem`](./apps/HelpDeskSystem)
* **Architecture:** Canvas App, Dataverse Tables, System Views, Role-Based Access Controls
* **Core Functionality:** 
  * End-to-end IT service request logging, ticket status tracking, and priority categorization.
  * Centralized dashboard for support agents to manage, assign, and resolve user tickets efficiently.

---

### 2. Check-In / Check-Out Inventory Management
* **Folder Location:** [`/apps/InventoryManagement`](./apps/InventoryManagement)
* **Architecture:** Canvas App, SharePoint Custom Lists (`Shared Equipment`, `Equipment List Log`)
* **Core Functionality:**
  * Real-time tracking of shared company equipment, active loans, and return status logs.
  * Prevents double-booking and maintains an accurate audit history for inventory assets.

---

### 3. Event Approval System & Automated Workflow
* **Folder Location:** [`/apps/ApprovalApp`](./apps/ApprovalApp)
* **Architecture:** Canvas App, Power Automate Cloud Flow (`Events Approval Workflow`), SharePoint List (`Events Info`)
* **Core Functionality:**
  * Request submission system integrated with an automated multi-stage decision workflow.
  * **Automated Flow Logic (`Events Approval Workflow`):**
    1. **Trigger:** Fires when an event record is created or modified in `Events Info`.
    2. **Approval Request:** Dispatches an approval card and waits for manager response.
    3. **Decision Handling:** Evaluates decision status via condition branches.
    4. **Execution:** Updates the SharePoint record status dynamically and sends target HTTP requests to SharePoint to update permissions and site actions upon approval.

---

## 🛠️ Repository Architecture & Standards

This repository follows professional Power Platform Application Lifecycle Management (ALM) practices:

* **Source Control:** Solutions are exported as unmanaged packages and unpacked into readable JSON/YAML source code using the Power Platform CLI (`pac`).
* **Version Control:** All Canvas App components, Power Fx formulas, and Power Automate flow definition files are tracked using Git.
* **Separation of Data & Logic:** Environment schemas are documented directly alongside the application files, allowing seamless deployment to clean environments.

---

## 👤 Author & Contact

**Christian Joubert**  
* **Email:** [joubertchristian24@gmail.com](mailto:joubertchristian24@gmail.com)
* **LinkedIn:** [linkedin.com/in/christian-joubert-a925ba251](https://www.linkedin.com/in/christian-joubert-a925ba251/)
* **GitHub Repository:** [ChristianJoubert-dev/PowerPlatform-Portfolio](https://github.com/ChristianJoubert-dev/PowerPlatform-Portfolio)