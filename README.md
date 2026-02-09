**AWS Identity and Access Management (IAM) Architecture for Multi-Department Organization  
# NoteTech
NoteTech is a growing technology services company that requires enterprise-grade access management to protect sensitive data across departments including employee records, financial data, marketing campaigns, and customer applications.

# Project Overview:
Designed and implemented role-based access control (RBAC) system for NoteTech, a simulated company with 10-users and 6 different departments. This project demonstrates identity and access managemnt principles including least privilege enforcement, multi-factor authentication (MFA), and password security policies. 

# Key Metrics
-Users Managed: 10 users
-Departments: 6 (Engineering, HR, Finance, IT, Marketing, Admin)
-AWS Managed Policies: 9
-MFA Coverage: Admin Tier

# User Distribution 
| Department  | Users | Key Permissions |
|-------------|-------|-----------------|
| Engineering | 2     | S3 Read-Only |
| HR          | 2     | IAM Read-Only |
| Finance     | 1     | Billing View-Only |
| IT          | 2     | Infrastructure Monitoring (Read-Only) |
| Marketing   | 2     | S3 Full, SES Full, Analytics View |
| Admin       | 1     | Full Access + MFA Required |



