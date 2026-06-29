# osTicket: End-to-End Ticketing System Deployment

## Objective
The goal of this lab was to deploy and configure an IT Service Management (ITSM) solution to handle user support requests. This project demonstrates the ability to manage the full lifecycle of a ticket—from submission to resolution—in a simulated corporate environment.

## Environment
* **Platform:** osTicket (Open-source ITSM)
* **Infrastructure:** VirtualBox (Internal Network)
* **Operating System:** Windows Server / Windows 10)
* **Stack:** PHP, MySQL/MariaDB, Apache/IIS

## Lab Workflow: Step-by-Step

### 1. Infrastructure Preparation
* Installed and configured the web server (Apache/IIS) and database management system (MySQL).
* Verified PHP requirements to ensure compatibility with the osTicket core files.
* Configured VirtualBox network settings to ensure the VM remained isolated yet reachable for testing.

### 2. osTicket Installation
* Downloaded and extracted the osTicket core files to the web root directory.
* Configured the `ost-config.php` file and established a connection to the MySQL database.
* Performed the initial web-based setup to initialize the system and create the administrative account.

### 3. Help Desk Configuration
* **Agents & Roles:** Defined IT staff roles and permissions to ensure least privilege access.
* **Help Topics:** Categorized support requests (e.g., "Hardware Issue," "Software Installation," "Password Reset") to automate routing.
* **SLA Policies:** Established Service Level Agreements to define response times for "Priority 1" vs. "Normal" tickets.

### 4. Ticket Lifecycle Simulation
* **User Submission:** Submitted test tickets from a secondary VM to simulate an end-user experience.
* **Routing & Escalation:** Verified that tickets were automatically routed to the correct department based on the Help Topic.
* **Resolution:** Performed the full lifecycle of a ticket: *Open -> Assignment -> Internal Note -> Resolution -> Closing.*

## Proof of Implementation
*(Replace the following with your actual file names)*
* **Admin Dashboard:** ![Admin Dashboard](admin-dashboard.png)
* **Ticket View:** ![Ticket View](agent-view.png)

## Key Learnings
* **ITSM Fundamentals:** Gained hands-on experience in how ticketing systems act as the "source of truth" for IT departments.
* **Troubleshooting:** Resolved database connectivity errors by validating user permissions in MySQL.
* **Process Automation:** Understood the impact of SLAs and Help Topics on reducing mean time to resolution (MTTR).
