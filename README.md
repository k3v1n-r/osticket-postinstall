# osTicket Post-Installation Guide
This guide provides step-by-step instructions to configure osTicket after installation.

## Admin & End-User Access
- **Admin/Analyst Login Page:** [http://localhost/osTicket/scp/login.php](http://localhost/osTicket/scp/login.php)
- **End Users osTicket URL:** [http://localhost/osTicket](http://localhost/osTicket)

## Configuration Steps
### 1. Configure Roles
- **What it does:** Defines permission levels for different agents.
- **Path:** `Admin Panel -> Agents -> Roles`
- Click on `Add New Role`.
- Name the role (e.g., `Root Admin`).
- Assign specific permissions based on responsibilities (e.g., ability to delete tickets, manage users, etc.).
- Click `Add Role` to apply changes.

### 2. Configure Departments
- **What it does:** Segments ticket handling by department to ensure proper delegation.
- **Path:** `Admin Panel -> Agents -> Departments`
- Click `Add New Department`.
- Name the department (e.g., `SysAdmins`).
- Set the department manager and define ticket visibility rules.
- Click `Create Dept`.

### 3. Configure Teams
- **What it does:** Allows agents from different departments to collaborate on tickets.
- **Path:** `Admin Panel -> Agents -> Teams`
- Click `Add New Team`.
- Configure Team.
- Assign agents.
- Click `Save`.

### 4. Allow Anyone to Create Tickets
- **What it does:** Determines whether users need to register before submitting tickets.
- **Path:** `Admin Panel -> Settings -> User Settings`
- Set the desired authentication settings for users
- You may add, edit, or delete templates for various user-end webpages.
- Click `Create Team`.

### 5. Configure Agents
- **What it does:** Assigns employees (agents) to handle tickets based on expertise.
- **Path:** `Admin Panel -> Agents -> Agents`
- Click `Add New Agent`.
- Enter agent details (Name, Email, Username, etc.).
- Configure the agent to the appropriate department.
- Enable permissions for the agent.
- Choose what team the agent is part of.
- Click `Create`.

### 6. Configure Users
- **What it does:** Registers end users (customers) who will submit support tickets.
- **Path:** `Agent Panel -> Users -> Add New`
- Click `Add New User`.
- Enter user details (Name, Email, Username, etc.).
- Click `Create User`.

### 7. Configure SLA
- **What it does:** Establishes response and resolution times for tickets based on priority.
- **Path:** `Admin Panel -> Manage -> SLA`
- Click `Add New SLA Plan`.
- SLA Examples:
  - `Sev-A`: Grace Period: `1 hour`, Schedule: `24/7` (Critical issues, e.g., system outage)
  - `Sev-B`: Grace Period: `4 hours`, Schedule: `24/7` (High-priority issues, e.g., server performance degradation)
  - `Sev-C`: Grace Period: `8 hours`, Schedule: `Business Hours` (Routine issues, e.g., password resets)
- Click `Add Plan`.

### 8. Configure Help Topics
- **What it does:** Categorizes ticket topics for better organization and routing.
- **Path:** `Admin Panel -> Manage -> Help Topics`
- Click `Add New Help Topic`.
- Enter a topic name (e.g., `Password Reset`).
- Set department and auto-assignment settings if necessary (e.g., password resets automatically go to Help Desk).
- Configure forms that the user will need to fill.
- Click `Add Topic`.

## Troubleshooting
If you encounter issues, ensure:
- Proper permissions are assigned to agents and users.
- Ticket creation settings match your organization’s needs.
- SLAs and Help Topics are configured correctly.
- Departments and teams are set up correctly.
