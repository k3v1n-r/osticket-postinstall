# osTicket Post-Installation Guide
This guide provides step-by-step instructions to configure osTicket after installation.

## Admin & End-User Access
- **Admin/Analyst Login Page:** [http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php)
- **End Users osTicket URL:** [http://localhost/osTicket](http://localhost/osTicket)

## Table of Contents
 1.  Roles.
 2.  Departments.
 3.  Teams.
 4.  General Settings.
 5.  Agents.
 6.  Users.
 7.  SLA.
 8.  Help Topics.

## 1. Configure Roles
- **Path:** `Admin Panel -> Agents -> Roles`
![Path to Roles](images/Screenshot(22).png)
- Click on `Add New Role`.
![Adding Role](images/Screenshot(23).png)
- Name the role (e.g., `Root Admin`).
![Naming the Role](images/Screenshot(24).png)
- Assign specific permissions based on responsibilities (e.g., ability to delete tickets, manage users, etc.).
![Assigning Permissions](images/Screenshot(25).png)
- Click `Add Role` to apply changes.

## 2. Configure Departments
- **What it does:** Segments ticket handling by department to ensure proper delegation.
- **Path:** `Admin Panel -> Agents -> Departments`
![Adding Departments](images/Screenshot(29).png)
- Click `Add New Department`.
- Name the department (e.g., `SysAdmins`).
- Set the department manager and define ticket visibility rules.
![Naming and Setting Department's Configuration](images/Screenshot(31).png)
- Click `Create Dept`.

## 3. Configure Teams
- **What it does:** Allows agents from different departments to collaborate on tickets.
- **Path:** `Admin Panel -> Agents -> Teams`
- Click `Add New Team`.
- Configure Team.
- Assign agents.
- Click `Create Team`.

## 4. Allow Anyone to Create Tickets
- **What it does:** Determines whether users need to register before submitting tickets.
- **Path:** `Admin Panel -> Settings -> User Settings`
![Adding Users](images/Screenshot(34).png)
- Set the desired authentication settings for users
![Configuring General User Permissions](images/Screenshot(35).png)
- You may add, edit, or delete templates for various user-end webpages.
![User Templates](images/Screenshot(37).png)
- Click `Save Changes`.

## 5. Configure Agents
- **What it does:** Assigns employees (agents) to handle tickets based on expertise.
- **Path:** `Admin Panel -> Agents -> Agents`
![Creating New Agents](images/Screenshot(38).png)
- Click `Add New Agent`.
- Enter agent details (Name, Email, Username, etc.).
- Configure the agent to the appropriate department.
![Department Configuration](images/Screenshot(40).png)
- Enable permissions for the agent.
![Permissions Configuration](images/Screenshot(41).png)
- Choose what team the agent is part of.
![Assigning Teams](images/Screenshot(42).png)
- Click `Create`.

## 6. Configure Users
- **What it does:** Registers end users (customers) who will submit support tickets.
- **Path:** `Agent Panel -> Users -> Add New`
- Click `Add New User`.
- Enter user details (Name, Email, Username, etc.).
- Click `Create User`.

## 7. Configure SLA
- **What it does:** Establishes response and resolution times for tickets based on priority.
- **Path:** `Admin Panel -> Manage -> SLA`
![Adding SLA](images/Screenshot(44).png)
- Click `Add New SLA Plan`.
- SLA Examples:
  ![SLA Example](images/Screenshot(46).png)
  - `Sev-A`: Grace Period: `1 hour`, Schedule: `24/7` (Critical issues, e.g., system outage)
  - `Sev-B`: Grace Period: `4 hours`, Schedule: `24/7` (High-priority issues, e.g., server performance degradation)
  - `Sev-C`: Grace Period: `8 hours`, Schedule: `Business Hours` (Routine issues, e.g., password resets)
  ![SLA Examples](images/Screenshot(47).png)
- Click `Add Plan`.

## 8. Configure Help Topics
- **What it does:** Categorizes ticket topics for better organization and routing.
- **Path:** `Admin Panel -> Manage -> Help Topics`
![Adding Help Topics](images/Screenshot(48).png)
- Click `Add New Help Topic`.
- Enter a topic name (e.g., `Password Reset`)
![Help Topic Example](images/Screenshot(50).png).
- Set department and auto-assignment settings if necessary (e.g., password resets automatically go to Help Desk).
![Config](images/Screenshot(51).png)
- Configure forms that the user will need to fill.
![Config](images/Screenshot(52).png)
- Click `Add Topic`.

## Troubleshooting
If you encounter issues, ensure:
- Proper permissions are assigned to agents and users.
- Ticket creation settings match your organization’s needs.
- SLAs and Help Topics are configured correctly.
- Departments and teams are set up correctly.
