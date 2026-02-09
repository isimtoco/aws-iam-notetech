**AWS Identity and Access Management (IAM) Architecture for Multi-Department Organization  
# NoteTech
NoteTech is a growing technology services company that requires enterprise-grade access management to protect sensitive data across departments including employee records, financial data, marketing campaigns, and customer applications.

# Project Overview:
Designed and implemented role-based access control (RBAC) system for NoteTech, a simulated company with 10-users and 6 different departments. This project demonstrates identity and access managemnt principles including least privilege enforcement, multi-factor authentication (MFA), and password security policies. 

# Key Metrics
- Users Managed: 10 users
- Departments: 6 (Engineering, HR, Finance, IT, Marketing, Admin)
- AWS Managed Policies: 9
- MFA Coverage: Admin Tier

# User Distribution 
| Department  | Users | Key Permissions |
|-------------|-------|-----------------|
| Admin       | 1     | Full Access + MFA Required |
| Engineering | 2     | S3 Read-Only |
| Finance     | 1     | Billing View-Only |
| HR          | 2     | IAM Read-Only |
| IT          | 2     | Infrastructure Monitoring (Read-Only) |
| Marketing   | 2     | S3 Full, SES Full, Analytics View |

# Employee Roster:
- Valentine Edwards (Admin-MFA enabled)
- Jake Miller (Engineering)
- Abigail Sutton (Engineering)
- Warren Zhao (Finance)
- Rose Lee (HR)
- Luca Rivera (HR)
- Alex Sharpe (IT)
- River Garcia (IT)
- Bella Robinson (Marketing)
- Emily Jenner (Marketing)

# Security Controls Implemented
### 1. Least Privilege Enforcement
- Group-based permissions (no individual user policies)
- Role-specific access segregation
- Read-only access preferred where appropriate

### 2. Multi-Factor Authentication (MFA)
- Enabled MFA for administrative account (valentina.edwards)
- TOTP-based authentication (Google Authenticator)
- To improve the project, expand to other deparmtents

### 3. Password Security Policy 
- Minimum password length: 15 characters
- Complexity requirements: uppercase, lowercase, numbers, symbols
- Password history: Prevents reuse of last 5 passwords
- Account lockout: Protection against brute-force attacks

### 4. Access Testing & Validation
Validated security across 4 comprehensive test scenarios:
- Marketing cannot access billing data
- Finance can access billing data
- Engineering cannot access EC2 infrastructure
- IT can view (but not modify) EC2 instances
- **Test Results:** 100% compliance with least privilege design 

