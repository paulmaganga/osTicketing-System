# osTicket: End-to-End Ticketing System Deployment

## Objective
The goal of this lab was to deploy and configure an IT Service Management (ITSM) solution to handle user support requests. This project demonstrates the ability to manage the full lifecycle of a ticket—from submission to resolution—in a simulated corporate environment.

## Environment
* **Platform:** osTicket (Open-source ITSM)
* **Infrastructure:** VirtualBox (Internal Network)
* **Operating System:** Windows Server / Windows 10)
* **Stack:** PHP, MySQL/MariaDB, Apache/IIS
* <img width="1721" height="903" alt="osTicket" src="https://github.com/user-attachments/assets/8e3c5bb4-a1fd-4cae-99cb-2d8dd7f5db83" />


## Lab Workflow: Step-by-Step

### 1. Infrastructure Preparation
* Installed and configured the web server (Apache/IIS) and database management system (MySQL).
* Verified PHP requirements to ensure compatibility with the osTicket core files.
* Configured VirtualBox network settings to ensure the VM remained isolated yet reachable for testing.

### 2. osTicket Installation
* Downloaded and extracted the osTicket core files to the web root directory.
* Configured the `ost-config.php` file and established a connection to the MySQL database.
* Performed the initial web-based setup to initialize the system and create the administrative account.
* <img width="1472" height="921" alt="osTicket Installation" src="https://github.com/user-attachments/assets/71d76bb9-abbb-4aaf-89e6-85aefa4de42f" />


### 3. Help Desk Configuration
* **Agents & Roles:** Defined IT staff roles and permissions to ensure least privilege access.
* **Help Topics:** Categorized support requests (e.g., "Hardware Issue," "Software Installation," "Password Reset") to automate routing.
* **SLA Policies:** Established Service Level Agreements to define response times for "Priority 1" vs. "Normal" tickets.

### 4. Ticket Lifecycle Simulation
* **User Submission:** Submitted test tickets from a secondary VM to simulate an end-user experience.
* **Routing & Escalation:** Verified that tickets were automatically routed to the correct department based on the Help Topic.
* **Resolution:** Performed the full lifecycle of a ticket: *Open -> Assignment -> Internal Note -> Resolution -> Closing.*
* <img width="1642" height="872" alt="Ticket Initiated" src="https://github.com/user-attachments/assets/04582ac9-0c47-4f05-8ee6-cedce42363d4" />
<img width="1448" height="926" alt="Help Desk-Ticket received" src="https://github.com/user-attachments/assets/12b9636e-a942-4030-9db6-51f83fa26b15" />
<img width="1505" height="546" alt="Ticket status changed" src="https://github.com/user-attachments/assets/7e5d2bb1-58db-442a-aecb-09a31a2a0964" />


## Key Learnings
* **ITSM Fundamentals:** Gained hands-on experience in how ticketing systems act as the "source of truth" for IT departments.
* **Troubleshooting:** Resolved database connectivity errors by validating user permissions in MySQL.
* **Process Automation:** Understood the impact of SLAs and Help Topics on reducing mean time to resolution (MTTR).
